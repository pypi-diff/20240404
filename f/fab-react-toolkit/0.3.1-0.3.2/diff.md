# Comparing `tmp/fab-react-toolkit-0.3.1.tar.gz` & `tmp/fab-react-toolkit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab-react-toolkit-0.3.1.tar", last modified: Thu Apr  4 10:01:31 2024, max compression
+gzip compressed data, was "fab-react-toolkit-0.3.2.tar", last modified: Thu Apr  4 10:07:15 2024, max compression
```

## Comparing `fab-react-toolkit-0.3.1.tar` & `fab-react-toolkit-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:01:31.167357 fab-react-toolkit-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 10:01:31.167357 fab-react-toolkit-0.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:01:31.163357 fab-react-toolkit-0.3.1/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:01:31.163357 fab-react-toolkit-0.3.1/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:01:31.163357 fab-react-toolkit-0.3.1/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:01:31.167357 fab-react-toolkit-0.3.1/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:01:31.167357 fab-react-toolkit-0.3.1/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 10:01:31.000000 fab-react-toolkit-0.3.1/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 10:01:31.000000 fab-react-toolkit-0.3.1/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:01:31.000000 fab-react-toolkit-0.3.1/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 10:01:31.000000 fab-react-toolkit-0.3.1/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-04 10:01:17.000000 fab-react-toolkit-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 10:01:31.167357 fab-react-toolkit-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:07:15.130812 fab-react-toolkit-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 10:07:15.130812 fab-react-toolkit-0.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:07:15.126812 fab-react-toolkit-0.3.2/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:07:15.126812 fab-react-toolkit-0.3.2/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:07:15.130812 fab-react-toolkit-0.3.2/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:07:15.130812 fab-react-toolkit-0.3.2/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:07:15.130812 fab-react-toolkit-0.3.2/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 10:07:15.000000 fab-react-toolkit-0.3.2/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 10:07:15.000000 fab-react-toolkit-0.3.2/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:07:15.000000 fab-react-toolkit-0.3.2/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 10:07:15.000000 fab-react-toolkit-0.3.2/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-04 10:07:06.000000 fab-react-toolkit-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 10:07:15.130812 fab-react-toolkit-0.3.2/setup.cfg
```

### Comparing `fab-react-toolkit-0.3.1/LICENSE` & `fab-react-toolkit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/PKG-INFO` & `fab-react-toolkit-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: A small example package
 Home-page: https://github.com/dttctcs/fab-react-toolkit
 Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fab-react-toolkit-0.3.1/example/app/__init__.py` & `fab-react-toolkit-0.3.2/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/example/app/apis.py` & `fab-react-toolkit-0.3.2/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/example/app/config.py` & `fab-react-toolkit-0.3.2/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/example/app/models.py` & `fab-react-toolkit-0.3.2/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/example/run.py` & `fab-react-toolkit-0.3.2/example/run.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/fab_react_toolkit/__init__.py` & `fab-react-toolkit-0.3.2/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/fab_react_toolkit/api/__init__.py` & `fab-react-toolkit-0.3.2/fab_react_toolkit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/fab_react_toolkit/api/convert.py` & `fab-react-toolkit-0.3.2/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/fab_react_toolkit/apis.py` & `fab-react-toolkit-0.3.2/fab_react_toolkit/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/fab_react_toolkit/filters.py` & `fab-react-toolkit-0.3.2/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/fab_react_toolkit/views.py` & `fab-react-toolkit-0.3.2/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/fab_react_toolkit.egg-info/PKG-INFO` & `fab-react-toolkit-0.3.2/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: A small example package
 Home-page: https://github.com/dttctcs/fab-react-toolkit
 Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fab-react-toolkit-0.3.1/fab_react_toolkit.egg-info/SOURCES.txt` & `fab-react-toolkit-0.3.2/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.1/pyproject.toml` & `fab-react-toolkit-0.3.2/pyproject.toml`

 * *Files identical despite different names*

