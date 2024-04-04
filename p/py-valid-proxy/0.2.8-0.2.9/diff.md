# Comparing `tmp/py_valid_proxy-0.2.8.tar.gz` & `tmp/py_valid_proxy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_valid_proxy-0.2.8.tar", max compression
+gzip compressed data, was "py_valid_proxy-0.2.9.tar", max compression
```

## Comparing `py_valid_proxy-0.2.8.tar` & `py_valid_proxy-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1460 2024-04-04 08:02:21.206608 py_valid_proxy-0.2.8/README.md
--rw-r--r--   0        0        0      503 2024-04-04 12:36:13.293788 py_valid_proxy-0.2.8/py_valid_proxy/__init__.py
--rw-r--r--   0        0        0      238 2023-11-20 15:59:28.750899 py_valid_proxy-0.2.8/py_valid_proxy/__main__.py
--rw-r--r--   0        0        0  6266981 2023-11-15 16:20:05.685165 py_valid_proxy-0.2.8/py_valid_proxy/data/GeoLite2-Country.mmdb
--rw-r--r--   0        0        0     2459 2024-04-04 07:46:27.183964 py_valid_proxy-0.2.8/py_valid_proxy/main.py
--rw-r--r--   0        0        0     4128 2024-04-04 07:39:33.487215 py_valid_proxy-0.2.8/py_valid_proxy/valid_proxy.py
--rw-r--r--   0        0        0      524 2024-04-04 12:36:07.145716 py_valid_proxy-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 py_valid_proxy-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1460 2024-04-04 08:02:21.206608 py_valid_proxy-0.2.9/README.md
+-rw-r--r--   0        0        0      503 2024-04-04 15:10:20.716793 py_valid_proxy-0.2.9/py_valid_proxy/__init__.py
+-rw-r--r--   0        0        0      238 2023-11-20 15:59:28.750899 py_valid_proxy-0.2.9/py_valid_proxy/__main__.py
+-rw-r--r--   0        0        0  6266981 2023-11-15 16:20:05.685165 py_valid_proxy-0.2.9/py_valid_proxy/data/GeoLite2-Country.mmdb
+-rw-r--r--   0        0        0     2459 2024-04-04 07:46:27.183964 py_valid_proxy-0.2.9/py_valid_proxy/main.py
+-rw-r--r--   0        0        0     4128 2024-04-04 07:39:33.487215 py_valid_proxy-0.2.9/py_valid_proxy/valid_proxy.py
+-rw-r--r--   0        0        0      524 2024-04-04 15:10:16.188741 py_valid_proxy-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 py_valid_proxy-0.2.9/PKG-INFO
```

### Comparing `py_valid_proxy-0.2.8/README.md` & `py_valid_proxy-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.8/py_valid_proxy/data/GeoLite2-Country.mmdb` & `py_valid_proxy-0.2.9/py_valid_proxy/data/GeoLite2-Country.mmdb`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.8/py_valid_proxy/main.py` & `py_valid_proxy-0.2.9/py_valid_proxy/main.py`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.8/py_valid_proxy/valid_proxy.py` & `py_valid_proxy-0.2.9/py_valid_proxy/valid_proxy.py`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.8/pyproject.toml` & `py_valid_proxy-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-valid-proxy"
-version = "0.2.8"
+version = "0.2.9"
 description = "Valid proxy server ('alive' or 'dead')"
 authors = ["Suvorinov Oleg <suvorinovoleg@yandex.ru>"]
 homepage="https://github.com/suvorinov/py_valid_proxy.git"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `py_valid_proxy-0.2.8/PKG-INFO` & `py_valid_proxy-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-valid-proxy
-Version: 0.2.8
+Version: 0.2.9
 Summary: Valid proxy server ('alive' or 'dead')
 Home-page: https://github.com/suvorinov/py_valid_proxy.git
 Author: Suvorinov Oleg
 Author-email: suvorinovoleg@yandex.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

