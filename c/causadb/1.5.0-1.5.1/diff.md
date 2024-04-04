# Comparing `tmp/causadb-1.5.0.tar.gz` & `tmp/causadb-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.5.0.tar", max compression
+gzip compressed data, was "causadb-1.5.1.tar", max compression
```

## Comparing `causadb-1.5.0.tar` & `causadb-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      642 2024-04-03 16:57:41.182521 causadb-1.5.0/README.md
--rw-r--r--   0        0        0      115 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-03 16:58:00.026551 causadb-1.5.0/causadb/__version__.py
--rw-r--r--   0        0        0     5189 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/causadb.py
--rw-r--r--   0        0        0     2855 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/account.py
--rw-r--r--   0        0        0     3116 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/data.py
--rwxr-xr-x   0        0        0      743 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/main.py
--rw-r--r--   0        0        0     7085 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/data.py
--rw-r--r--   0        0        0    14837 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/model.py
--rw-r--r--   0        0        0      215 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/utils.py
--rw-r--r--   0        0        0      695 2024-04-03 16:57:59.022549 causadb-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 causadb-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-04 11:22:03.872011 causadb-1.5.1/README.md
+-rw-r--r--   0        0        0      115 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-04 11:22:23.680127 causadb-1.5.1/causadb/__version__.py
+-rw-r--r--   0        0        0     5189 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/causadb.py
+-rw-r--r--   0        0        0     2855 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/account.py
+-rw-r--r--   0        0        0     3116 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/main.py
+-rw-r--r--   0        0        0     7085 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/data.py
+-rw-r--r--   0        0        0    14837 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/model.py
+-rw-r--r--   0        0        0      215 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/utils.py
+-rw-r--r--   0        0        0      695 2024-04-04 11:22:22.856122 causadb-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 causadb-1.5.1/PKG-INFO
```

### Comparing `causadb-1.5.0/README.md` & `causadb-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.5.0/causadb/causadb.py` & `causadb-1.5.1/causadb/causadb.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.0/causadb/cli/account.py` & `causadb-1.5.1/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.0/causadb/cli/data.py` & `causadb-1.5.1/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.0/causadb/cli/main.py` & `causadb-1.5.1/causadb/cli/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import typer
 from typing import Optional
+import requests
 import causadb.cli.account as account
 import causadb.cli.data as data
 import causadb.cli.models as models
+from causadb.cli.utils import CAUSADB_URL
 from causadb import __version__
 
 app = typer.Typer()
 
 
 def version_callback(value: bool):
     if value:
         typer.echo(f"CausaDB CLI v{__version__}")
+        server_version = requests.get(
+            f"{CAUSADB_URL}/version"
+        ).json()["version"]
+        typer.echo(f"CausaDB Server v{server_version}")
+
         raise typer.Exit()
 
 
 @app.callback()
 def cli(
         _: Optional[bool] = typer.Option(
             None, "-v", "--version", callback=version_callback, is_eager=True, help="Print the version of the CausaDB CLI"
```

### Comparing `causadb-1.5.0/causadb/cli/models.py` & `causadb-1.5.1/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.0/causadb/cli/utils.py` & `causadb-1.5.1/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.0/causadb/data.py` & `causadb-1.5.1/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.0/causadb/model.py` & `causadb-1.5.1/causadb/model.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.0/pyproject.toml` & `causadb-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.5.0"
+version = "1.5.1"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
```

### Comparing `causadb-1.5.0/PKG-INFO` & `causadb-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.5.0
+Version: 1.5.1
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

