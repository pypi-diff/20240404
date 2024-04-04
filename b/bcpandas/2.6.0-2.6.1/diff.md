# Comparing `tmp/bcpandas-2.6.0.tar.gz` & `tmp/bcpandas-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcpandas-2.6.0.tar", max compression
+gzip compressed data, was "bcpandas-2.6.1.tar", max compression
```

## Comparing `bcpandas-2.6.0.tar` & `bcpandas-2.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2024-02-25 00:26:02.719964 bcpandas-2.6.0/LICENSE
--rw-r--r--   0        0        0    19148 2024-02-25 00:26:02.719964 bcpandas-2.6.0/README.md
--rw-r--r--   0        0        0      563 2024-02-25 00:26:02.719964 bcpandas-2.6.0/bcpandas/__init__.py
--rw-r--r--   0        0        0     2339 2024-02-25 00:26:02.719964 bcpandas-2.6.0/bcpandas/constants.py
--rw-r--r--   0        0        0    17835 2024-02-25 00:26:02.719964 bcpandas-2.6.0/bcpandas/main.py
--rw-r--r--   0        0        0     8576 2024-02-25 00:26:02.719964 bcpandas-2.6.0/bcpandas/utils.py
--rw-r--r--   0        0        0     2545 2024-02-25 00:26:17.048066 bcpandas-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    20256 1970-01-01 00:00:00.000000 bcpandas-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-04 02:40:58.560387 bcpandas-2.6.1/LICENSE
+-rw-r--r--   0        0        0    19148 2024-04-04 02:40:58.560387 bcpandas-2.6.1/README.md
+-rw-r--r--   0        0        0      563 2024-04-04 02:40:58.560387 bcpandas-2.6.1/bcpandas/__init__.py
+-rw-r--r--   0        0        0     2339 2024-04-04 02:40:58.560387 bcpandas-2.6.1/bcpandas/constants.py
+-rw-r--r--   0        0        0    17835 2024-04-04 02:40:58.560387 bcpandas-2.6.1/bcpandas/main.py
+-rw-r--r--   0        0        0     8576 2024-04-04 02:40:58.560387 bcpandas-2.6.1/bcpandas/utils.py
+-rw-r--r--   0        0        0     2545 2024-04-04 02:41:11.984529 bcpandas-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0    20256 1970-01-01 00:00:00.000000 bcpandas-2.6.1/PKG-INFO
```

### Comparing `bcpandas-2.6.0/LICENSE` & `bcpandas-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.0/README.md` & `bcpandas-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.0/bcpandas/__init__.py` & `bcpandas-2.6.1/bcpandas/__init__.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.0/bcpandas/constants.py` & `bcpandas-2.6.1/bcpandas/constants.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.0/bcpandas/main.py` & `bcpandas-2.6.1/bcpandas/main.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.0/bcpandas/utils.py` & `bcpandas-2.6.1/bcpandas/utils.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.6.0/pyproject.toml` & `bcpandas-2.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 description = "High-level wrapper around BCP for high performance data transfers between pandas and SQL Server. No knowledge of BCP required!!"
 keywords = ["bcp", "mssql", "pandas"]
 license = "MIT"
 maintainers = ["Oliver Borchert <me@borchero.com>"]
 name = "bcpandas"
 readme = "README.md"
 repository = "https://github.com/yehoshuadimarsky/bcpandas"
-version = "v2.6.0"
+version = "v2.6.1"
 
 [tool.poetry.plugins."pandas.sql.engine"]
 bcpandas = "bcpandas.main:to_sql"
 
 [tool.poetry.dependencies]
 pandas = ">=1.5"
 pyodbc = "*"
```

### Comparing `bcpandas-2.6.0/PKG-INFO` & `bcpandas-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcpandas
-Version: 2.6.0
+Version: 2.6.1
 Summary: High-level wrapper around BCP for high performance data transfers between pandas and SQL Server. No knowledge of BCP required!!
 Home-page: https://github.com/yehoshuadimarsky/bcpandas
 License: MIT
 Keywords: bcp,mssql,pandas
 Author: yehoshuadimarsky
 Maintainer: Oliver Borchert
 Maintainer-email: me@borchero.com
```

