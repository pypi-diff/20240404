# Comparing `tmp/hyperon_das_atomdb-0.6.1.tar.gz` & `tmp/hyperon_das_atomdb-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das_atomdb-0.6.1.tar", max compression
+gzip compressed data, was "hyperon_das_atomdb-0.6.2.tar", max compression
```

## Comparing `hyperon_das_atomdb-0.6.1.tar` & `hyperon_das_atomdb-0.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1081 2024-03-28 22:11:53.380728 hyperon_das_atomdb-0.6.1/LICENCE
--rw-r--r--   0        0        0     2687 2024-03-28 22:11:53.380728 hyperon_das_atomdb-0.6.1/README.md
--rw-r--r--   0        0        0      306 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/__init__.py
--rw-r--r--   0        0        0      116 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/adapters/__init__.py
--rw-r--r--   0        0        0    20316 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/adapters/ram_only.py
--rw-r--r--   0        0        0    36782 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/adapters/redis_mongo_db.py
--rw-r--r--   0        0        0    19708 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/database.py
--rw-r--r--   0        0        0      877 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/exceptions.py
--rw-r--r--   0        0        0     1122 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/index.py
--rw-r--r--   0        0        0     1052 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/logger.py
--rw-r--r--   0        0        0        0 2024-03-28 22:11:53.384728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/utils/__init__.py
--rw-r--r--   0        0        0     1947 2024-03-28 22:11:53.388728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/utils/expression_hasher.py
--rw-r--r--   0        0        0     1388 2024-03-28 22:11:53.388728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/utils/patterns.py
--rw-r--r--   0        0        0       65 2024-03-28 22:11:53.388728 hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/utils/settings.py
--rw-r--r--   0        0        0     1161 2024-03-28 22:12:05.408748 hyperon_das_atomdb-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3605 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-04 18:20:01.366002 hyperon_das_atomdb-0.6.2/LICENCE
+-rw-r--r--   0        0        0     2687 2024-04-04 18:20:01.366002 hyperon_das_atomdb-0.6.2/README.md
+-rw-r--r--   0        0        0      306 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/adapters/__init__.py
+-rw-r--r--   0        0        0    20316 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/adapters/ram_only.py
+-rw-r--r--   0        0        0    36801 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/adapters/redis_mongo_db.py
+-rw-r--r--   0        0        0    19708 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/database.py
+-rw-r--r--   0        0        0      877 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/exceptions.py
+-rw-r--r--   0        0        0     1122 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/index.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/logger.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/utils/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/utils/expression_hasher.py
+-rw-r--r--   0        0        0     1388 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/utils/patterns.py
+-rw-r--r--   0        0        0       65 2024-04-04 18:20:01.370002 hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/utils/settings.py
+-rw-r--r--   0        0        0     1161 2024-04-04 18:20:10.137940 hyperon_das_atomdb-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3605 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.2/PKG-INFO
```

### Comparing `hyperon_das_atomdb-0.6.1/LICENCE` & `hyperon_das_atomdb-0.6.2/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/README.md` & `hyperon_das_atomdb-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/adapters/ram_only.py` & `hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/adapters/ram_only.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/adapters/redis_mongo_db.py` & `hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/adapters/redis_mongo_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 
 class MongoDBIndex(Index):
     def __init__(self, collection: Collection) -> None:
         self.collection = collection
 
     def create(self, atom_type: str, field: str, **kwargs) -> Tuple[str, Any]:
-        conditionals = None
+        conditionals = {}
 
         for key, value in kwargs.items():
             conditionals = {key: {"$eq": value}}
             break  # only one key-value pair
 
         index_id = f"{atom_type}_{self.generate_index_id(field, conditionals)}"
 
@@ -877,14 +877,16 @@
         field: str,
         type: Optional[str] = None,
         composite_type: Optional[List[Any]] = None,
     ) -> str:
         if type and composite_type:
             raise ValueError("Both type and composite_type cannot be specified")
 
+        kwargs = {}
+
         if type:
             kwargs = {MongoFieldNames.TYPE_NAME: type}
         elif composite_type:
             kwargs = {MongoFieldNames.TYPE: self._calculate_composite_type_hash(composite_type)}
 
         collection = self.mongo_atoms_collection
```

### Comparing `hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/database.py` & `hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/database.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/exceptions.py` & `hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/index.py` & `hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/index.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/logger.py` & `hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/utils/expression_hasher.py` & `hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/utils/expression_hasher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/hyperon_das_atomdb/utils/patterns.py` & `hyperon_das_atomdb-0.6.2/hyperon_das_atomdb/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.1/pyproject.toml` & `hyperon_das_atomdb-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperon-das-atomdb"
-version = "0.6.1"
+version = "0.6.2"
 description = "Persistence layer for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das_atomdb"}]
 
 [tool.poetry.urls]
 "Code" = "https://github.com/singnet/das-atom-db"
```

### Comparing `hyperon_das_atomdb-0.6.1/PKG-INFO` & `hyperon_das_atomdb-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperon-das-atomdb
-Version: 0.6.1
+Version: 0.6.2
 Summary: Persistence layer for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

