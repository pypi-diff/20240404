# Comparing `tmp/llama_index_vector_stores_postgres-0.1.4.post1.tar.gz` & `tmp/llama_index_vector_stores_postgres-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_postgres-0.1.4.post1.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_postgres-0.1.5.tar", max compression
```

## Comparing `llama_index_vector_stores_postgres-0.1.4.post1.tar` & `llama_index_vector_stores_postgres-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       49 2024-03-19 16:06:21.747874 llama_index_vector_stores_postgres-0.1.4.post1/README.md
--rw-r--r--   0        0        0       95 2024-03-19 16:06:21.747874 llama_index_vector_stores_postgres-0.1.4.post1/llama_index/vector_stores/postgres/__init__.py
--rw-r--r--   0        0        0    24756 2024-03-19 16:06:21.747874 llama_index_vector_stores_postgres-0.1.4.post1/llama_index/vector_stores/postgres/base.py
--rw-r--r--   0        0        0     1615 2024-03-19 16:06:21.747874 llama_index_vector_stores_postgres-0.1.4.post1/pyproject.toml
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 llama_index_vector_stores_postgres-0.1.4.post1/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-04-04 19:14:45.829085 llama_index_vector_stores_postgres-0.1.5/README.md
+-rw-r--r--   0        0        0       95 2024-04-04 19:14:45.829085 llama_index_vector_stores_postgres-0.1.5/llama_index/vector_stores/postgres/__init__.py
+-rw-r--r--   0        0        0    25831 2024-04-04 19:14:45.829085 llama_index_vector_stores_postgres-0.1.5/llama_index/vector_stores/postgres/base.py
+-rw-r--r--   0        0        0     1609 2024-04-04 19:14:45.829085 llama_index_vector_stores_postgres-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 llama_index_vector_stores_postgres-0.1.5/PKG-INFO
```

### Comparing `llama_index_vector_stores_postgres-0.1.4.post1/llama_index/vector_stores/postgres/base.py` & `llama_index_vector_stores_postgres-0.1.5/llama_index/vector_stores/postgres/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,35 @@
             {"__tablename__": tablename, "__table_args__": {"schema": schema_name}},
         )
 
     return model
 
 
 class PGVectorStore(BasePydanticVectorStore):
+    """Postgres Vector Store.
+
+    Examples:
+        `pip install llama-index-vector-stores-postgres`
+
+        ```python
+        from llama_index.vector_stores.postgres import PGVectorStore
+
+        # Create PGVectorStore instance
+        vector_store = PGVectorStore.from_params(
+            database="vector_db",
+            host="localhost",
+            password="password",
+            port=5432,
+            user="postgres",
+            table_name="paul_graham_essay",
+            embed_dim=1536  # openai embedding dimension
+        )
+        ```
+    """
+
     from sqlalchemy.sql.selectable import Select
 
     stores_text = True
     flat_metadata = False
 
     connection_string: str
     async_connection_string: str
@@ -367,19 +388,29 @@
             # Expects a list stored in the metadata, and a single value to compare
             return text(
                 f"metadata_::jsonb->'{filter_.key}' "
                 f"{self._to_postgres_operator(filter_.operator)} "
                 f"'[\"{filter_.value}\"]'"
             )
         else:
-            return text(
-                f"metadata_->>'{filter_.key}' "
-                f"{self._to_postgres_operator(filter_.operator)} "
-                f"'{filter_.value}'"
-            )
+            # Check if value is a number. If so, cast the metadata value to a float
+            # This is necessary because the metadata is stored as a string
+            try:
+                return text(
+                    f"(metadata_->>'{filter_.key}')::float "
+                    f"{self._to_postgres_operator(filter_.operator)} "
+                    f"{float(filter_.value)}"
+                )
+            except ValueError:
+                # If not a number, then treat it as a string
+                return text(
+                    f"metadata_->>'{filter_.key}' "
+                    f"{self._to_postgres_operator(filter_.operator)} "
+                    f"'{filter_.value}'"
+                )
 
     def _recursively_apply_filters(self, filters: List[MetadataFilters]) -> Any:
         """
         Returns a sqlalchemy where clause.
         """
         import sqlalchemy
```

### Comparing `llama_index_vector_stores_postgres-0.1.4.post1/pyproject.toml` & `llama_index_vector_stores_postgres-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores postgres integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-postgres"
 readme = "README.md"
-version = "0.1.4.post1"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.20"
 pgvector = "^0.2.4"
 psycopg2-binary = "^2.9.9"
 asyncpg = "^0.29.0"
```

### Comparing `llama_index_vector_stores_postgres-0.1.4.post1/PKG-INFO` & `llama_index_vector_stores_postgres-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-postgres
-Version: 0.1.4.post1
+Version: 0.1.5
 Summary: llama-index vector_stores postgres integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

