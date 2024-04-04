# Comparing `tmp/causadb-1.5.1.tar.gz` & `tmp/causadb-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.5.1.tar", max compression
+gzip compressed data, was "causadb-1.6.0.tar", max compression
```

## Comparing `causadb-1.5.1.tar` & `causadb-1.6.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      642 2024-04-04 11:22:03.872011 causadb-1.5.1/README.md
--rw-r--r--   0        0        0      115 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-04 11:22:23.680127 causadb-1.5.1/causadb/__version__.py
--rw-r--r--   0        0        0     5189 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/causadb.py
--rw-r--r--   0        0        0     2855 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/account.py
--rw-r--r--   0        0        0     3116 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/data.py
--rwxr-xr-x   0        0        0      962 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/main.py
--rw-r--r--   0        0        0     7085 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/data.py
--rw-r--r--   0        0        0    14837 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/model.py
--rw-r--r--   0        0        0      215 2024-04-04 11:22:03.872011 causadb-1.5.1/causadb/utils.py
--rw-r--r--   0        0        0      695 2024-04-04 11:22:22.856122 causadb-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 causadb-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-04 14:03:28.434420 causadb-1.6.0/README.md
+-rw-r--r--   0        0        0      115 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-04 14:03:46.210371 causadb-1.6.0/causadb/__version__.py
+-rw-r--r--   0        0        0     5189 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/causadb.py
+-rw-r--r--   0        0        0     2855 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/account.py
+-rw-r--r--   0        0        0     3116 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/main.py
+-rw-r--r--   0        0        0     7085 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/data.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/examples/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/examples/heating.py
+-rw-r--r--   0        0        0    14837 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/model.py
+-rw-r--r--   0        0        0      215 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/utils.py
+-rw-r--r--   0        0        0      695 2024-04-04 14:03:45.478371 causadb-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 causadb-1.6.0/PKG-INFO
```

### Comparing `causadb-1.5.1/README.md` & `causadb-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/causadb/causadb.py` & `causadb-1.6.0/causadb/causadb.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/causadb/cli/account.py` & `causadb-1.6.0/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/causadb/cli/data.py` & `causadb-1.6.0/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/causadb/cli/main.py` & `causadb-1.6.0/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/causadb/cli/models.py` & `causadb-1.6.0/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/causadb/cli/utils.py` & `causadb-1.6.0/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/causadb/data.py` & `causadb-1.6.0/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/causadb/model.py` & `causadb-1.6.0/causadb/model.py`

 * *Files identical despite different names*

### Comparing `causadb-1.5.1/pyproject.toml` & `causadb-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.5.1"
+version = "1.6.0"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
```

### Comparing `causadb-1.5.1/PKG-INFO` & `causadb-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.5.1
+Version: 1.6.0
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

