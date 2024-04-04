# Comparing `tmp/sparkorm-1.2.8-py3-none-any.whl.zip` & `tmp/sparkorm-1.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 33366 bytes, number of entries: 18
+Zip file size: 33760 bytes, number of entries: 18
 -rw-r--r--  2.0 fat     1000 b- defN 80-Jan-01 00:00 sparkorm/__init__.py
 -rw-r--r--  2.0 fat     1277 b- defN 80-Jan-01 00:00 sparkorm/accessors.py
 -rw-r--r--  2.0 fat    14875 b- defN 80-Jan-01 00:00 sparkorm/base_field.py
 -rw-r--r--  2.0 fat     2566 b- defN 80-Jan-01 00:00 sparkorm/exceptions.py
 -rw-r--r--  2.0 fat    19670 b- defN 80-Jan-01 00:00 sparkorm/fields.py
 -rw-r--r--  2.0 fat     3804 b- defN 80-Jan-01 00:00 sparkorm/formatters.py
--rw-r--r--  2.0 fat     1726 b- defN 80-Jan-01 00:00 sparkorm/metadata_types.py
--rw-r--r--  2.0 fat     7987 b- defN 80-Jan-01 00:00 sparkorm/models.py
+-rw-r--r--  2.0 fat     2253 b- defN 80-Jan-01 00:00 sparkorm/metadata_types.py
+-rw-r--r--  2.0 fat     9117 b- defN 80-Jan-01 00:00 sparkorm/models.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 sparkorm/py.typed
 -rw-r--r--  2.0 fat      408 b- defN 80-Jan-01 00:00 sparkorm/schema_builder.py
 -rw-r--r--  2.0 fat     7475 b- defN 80-Jan-01 00:00 sparkorm/schema_merger.py
 -rw-r--r--  2.0 fat    28285 b- defN 80-Jan-01 00:00 sparkorm/struct.py
--rw-r--r--  2.0 fat     6880 b- defN 80-Jan-01 00:00 sparkorm/utils.py
--rw-r--r--  2.0 fat      265 b- defN 80-Jan-01 00:00 sparkorm-1.2.8.dist-info/entry_points.txt
--rw-r--r--  2.0 fat     1099 b- defN 80-Jan-01 00:00 sparkorm-1.2.8.dist-info/LICENSE
--rw-r--r--  2.0 fat    16574 b- defN 80-Jan-01 00:00 sparkorm-1.2.8.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 sparkorm-1.2.8.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1408 b- defN 16-Jan-01 00:00 sparkorm-1.2.8.dist-info/RECORD
-18 files, 115387 bytes uncompressed, 31098 bytes compressed:  73.0%
+-rw-r--r--  2.0 fat     6892 b- defN 80-Jan-01 00:00 sparkorm/utils.py
+-rw-r--r--  2.0 fat      265 b- defN 80-Jan-01 00:00 sparkorm-1.2.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat     1099 b- defN 80-Jan-01 00:00 sparkorm-1.2.9.dist-info/LICENSE
+-rw-r--r--  2.0 fat    16607 b- defN 80-Jan-01 00:00 sparkorm-1.2.9.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 sparkorm-1.2.9.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1408 b- defN 16-Jan-01 00:00 sparkorm-1.2.9.dist-info/RECORD
+18 files, 117089 bytes uncompressed, 31492 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: sparkorm/struct.py
 Comment: 
 
 Filename: sparkorm/utils.py
 Comment: 
 
-Filename: sparkorm-1.2.8.dist-info/entry_points.txt
+Filename: sparkorm-1.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparkorm-1.2.8.dist-info/LICENSE
+Filename: sparkorm-1.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: sparkorm-1.2.8.dist-info/METADATA
+Filename: sparkorm-1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: sparkorm-1.2.8.dist-info/WHEEL
+Filename: sparkorm-1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: sparkorm-1.2.8.dist-info/RECORD
+Filename: sparkorm-1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparkorm/metadata_types.py

```diff
@@ -1,10 +1,12 @@
 from abc import ABC, abstractmethod
 from enum import auto, Enum
-from typing import Optional, Type, Union
+from typing import Optional, Type, Union, NamedTuple
+
+from strenum import StrEnum
 
 
 class DBConfig(ABC):
     @classmethod
     @abstractmethod
     def get_name(cls) -> str:
         ...
@@ -35,29 +37,50 @@
 class SchemaUpdateStatus(Enum):
     """
     Status of the schema update
     """
     CREATED = auto()
     SKIPPED = auto()
     DROPPED_AND_CREATED = auto()
+    REPLACED = auto()
 
+class LocationType(StrEnum):
+    TEXT = auto()
+    AVRO = auto()
+    BINARYFILE = auto()
+    CSV = auto()
+    JSON = auto()
+    PARQUET = auto()
+    ORC = auto()
+    JDBC = auto()
+    DELTA = auto()
+    LIBSVM = auto()
+
+class LocationConfig(NamedTuple):
+    type: LocationType
+    location: str
 
 class MetaConfig(ABC):
     migration_strategy: SchemaMigrationStrategy = NoChangeStrategy()
     db_config: Optional[Union[Type[DBConfig], DBConfig]] = None
     name: str
+    location: Optional[LocationConfig] = None
 
     @classmethod
     def get_name(cls) -> str:
         return cls.name
 
     @classmethod
     def get_db_name(cls) -> Optional[str]:
         if cls.db_config is not None:
             assert issubclass(cls.db_config, DBConfig) or isinstance(cls.db_config, DBConfig), str(cls.db_config.__class__)
             return cls.db_config.get_name()
         return None
 
     @classmethod
-    def _get_migration_strategy(cls) -> SchemaMigrationStrategy:
+    def get_migration_strategy(cls) -> SchemaMigrationStrategy:
         assert isinstance(cls.migration_strategy, SchemaMigrationStrategy)
         return cls.migration_strategy
+
+    @classmethod
+    def get_location(cls) -> Optional[LocationConfig]:
+        return cls.location
```

## sparkorm/models.py

```diff
@@ -6,23 +6,27 @@
 from pyspark.sql.types import (
     StructType,
 )
 from streamerate import stream
 
 from sparkorm.base_field import PARTITIONED_BY_KEY
 from sparkorm.exceptions import TableUpdateError
-from sparkorm.metadata_types import DBConfig, NoChangeStrategy, SchemaMigrationStrategy, DropAndCreateStrategy, SchemaUpdateStatus
+from sparkorm.metadata_types import DBConfig, NoChangeStrategy, SchemaMigrationStrategy, DropAndCreateStrategy, SchemaUpdateStatus, MetaConfig, LocationConfig, \
+    LocationType
 from sparkorm.struct import Struct
 from sparkorm.utils import spark_struct_to_sql_string, convert_to_struct_type
 
 
 class BaseModel(Struct):
-    VALID_METADATA_ATTRS = {"name", "db_config", "migration_strategy", "includes"}
+    VALID_METADATA_ATTRS = {"name", "db_config", "migration_strategy", "includes", "location"}
     SQL_NAME = "NAME"
 
+    class Meta(MetaConfig):
+        pass
+
     def __init__(self, spark: SparkSession):
         super().__init__()
         self._spark = spark
 
     def __init_subclass__(cls, /, **kwargs):
         if hasattr(cls, "Meta"):
             attributes = {k: v for k, v in vars(cls.Meta).items() if not callable(v) and not k.startswith("_")}
@@ -82,37 +86,54 @@
         If the table exists, but has a different structure, an exception will be raised.
         Returns True if the table already exists and has the correct structure.
         """
         full_name = self.get_full_name()
         spark_schema = self.get_spark_schema()
 
         if self._spark.catalog.tableExists(tableName=self.get_name(), dbName=self.get_db_name()):
+            if hasattr(self.Meta, "location") and self.Meta.location is not None:
+                self.create(or_replace=True)
+                return SchemaUpdateStatus.REPLACED
             table_columns = self._spark.catalog.listColumns(tableName=self.get_name(), dbName=self.get_db_name())
             struct_type = convert_to_struct_type(table_columns)
             if struct_type != spark_schema:
                 migration_strategy = self._get_migration_strategy()
                 if isinstance(migration_strategy, DropAndCreateStrategy):
                     self.drop()
-                    self.create()
+                    self.create(or_replace=False)
                     return SchemaUpdateStatus.DROPPED_AND_CREATED
                 raise TableUpdateError(
                     f"Table {full_name} already exists with different schema. "
                     f"Existing schema: {struct_type}, "
                     f"Expected schema: {spark_schema}"
                 )
             return SchemaUpdateStatus.SKIPPED
         else:
             self.create()
             return SchemaUpdateStatus.CREATED
 
-    def create(self) -> None:
+    def create(self, or_replace: bool = False) -> None:
         """
         Raises exception if the table already exists.
         """
         full_name = self.get_full_name()
+        if hasattr(self.Meta, 'location'):
+            location = self.Meta.location
+        else:
+            location = None
+        if location is not None:
+            assert isinstance(location, LocationConfig), f"Invalid location: {location}"
+            assert isinstance(location.type, LocationType), f"Invalid location type: {location.type}"
+            assert isinstance(location.location, str), f"Invalid location: {location.location}"
+            location_type = location.type
+            location_str = location.location
+            or_replace_str = " OR REPLACE" if or_replace else ""
+            create_statement = f"CREATE{or_replace_str} TABLE {full_name} USING {location_type} LOCATION '{location_str}'"
+            self._spark.sql(create_statement)
+            return
         spark_schema = self.get_spark_schema()
 
         fields = spark_schema.fields
         column_names = stream(fields).map(spark_struct_to_sql_string).mkString(",")
         create_statement = f"CREATE TABLE {full_name} ({column_names})"
         partitioned_by_fields = [
             field.name for field in fields if field.metadata.get(PARTITIONED_BY_KEY, False) is True
```

## sparkorm/utils.py

```diff
@@ -130,15 +130,15 @@
         field_reprs.append(field_repr)
 
     db_config = db_config_map[db_name]
     if db_config is not None:
         db_config_val = f"db_config = {db_config.__name__}"
     else:
         db_config_val = ''
-    meta_repr = f"""   class Meta:\n       name = "{table_name}"\n"""
+    meta_repr = f"""   class Meta(MetaConfig):\n       name = "{table_name}"\n"""
     if db_config_val:
         meta_repr += f"       {db_config_val}\n"
     class_fields = "\n".join(field_reprs)
     class_template = f"""
 class {class_name}(TableModel):
 {meta_repr}
 {class_fields}
```

## Comparing `sparkorm-1.2.8.dist-info/LICENSE` & `sparkorm-1.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparkorm-1.2.8.dist-info/METADATA` & `sparkorm-1.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sparkorm
-Version: 1.2.8
+Version: 1.2.9
 Summary: SparkORM: Python Spark SQL & DataFrame schema management and basic Object Relational Mapping.
 Home-page: https://github.com/asuiu/sparkorm
 License: MIT
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: StrEnum (>=0.4.0)
 Requires-Dist: pyspark (>=3.0,<4.0)
 Requires-Dist: streamerate (>=1,<2)
 Project-URL: Repository, https://github.com/asuiu/sparkorm
 Description-Content-Type: text/markdown
 
 # SparkORM ✨
```

