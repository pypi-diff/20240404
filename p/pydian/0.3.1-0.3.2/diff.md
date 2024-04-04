# Comparing `tmp/pydian-0.3.1.tar.gz` & `tmp/pydian-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydian-0.3.1.tar", max compression
+gzip compressed data, was "pydian-0.3.2.tar", max compression
```

## Comparing `pydian-0.3.1.tar` & `pydian-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-10-23 15:32:39.843328 pydian-0.3.1/LICENSE.md
--rw-r--r--   0        0        0      133 2023-10-23 15:32:39.843328 pydian-0.3.1/pydian/__init__.py
--rw-r--r--   0        0        0    14871 2023-11-12 16:34:55.043419 pydian-0.3.1/pydian/dataframes.py
--rw-r--r--   0        0        0     7556 2023-11-06 15:48:54.142241 pydian-0.3.1/pydian/dicts.py
--rw-r--r--   0        0        0     1592 2023-11-05 19:21:26.773600 pydian-0.3.1/pydian/globs.py
--rw-r--r--   0        0        0        0 2023-10-23 15:32:39.843328 pydian-0.3.1/pydian/lib/__init__.py
--rw-r--r--   0        0        0     1360 2023-11-01 14:15:28.822615 pydian-0.3.1/pydian/lib/types.py
--rw-r--r--   0        0        0     3000 2023-10-31 18:28:27.126577 pydian-0.3.1/pydian/lib/util.py
--rw-r--r--   0        0        0     2257 2023-11-05 19:21:26.773600 pydian-0.3.1/pydian/mapper.py
--rw-r--r--   0        0        0     5066 2023-11-05 19:21:26.773600 pydian-0.3.1/pydian/partials.py
--rw-r--r--   0        0        0      657 2023-11-12 16:32:16.745181 pydian-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 pydian-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-27 21:22:50.771826 pydian-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0      133 2023-02-27 19:38:00.361634 pydian-0.3.2/pydian/__init__.py
+-rw-r--r--   0        0        0    14871 2023-11-18 01:22:42.900729 pydian-0.3.2/pydian/dataframes.py
+-rw-r--r--   0        0        0     7556 2023-11-18 01:22:42.900974 pydian-0.3.2/pydian/dicts.py
+-rw-r--r--   0        0        0     1592 2023-11-18 01:22:42.901064 pydian-0.3.2/pydian/globs.py
+-rw-r--r--   0        0        0        0 2023-02-22 00:10:14.742269 pydian-0.3.2/pydian/lib/__init__.py
+-rw-r--r--   0        0        0     1360 2023-11-18 01:22:14.531473 pydian-0.3.2/pydian/lib/types.py
+-rw-r--r--   0        0        0     3000 2023-11-18 01:22:42.901995 pydian-0.3.2/pydian/lib/util.py
+-rw-r--r--   0        0        0     2257 2023-11-18 01:22:42.902194 pydian-0.3.2/pydian/mapper.py
+-rw-r--r--   0        0        0     5066 2023-11-18 01:22:42.902418 pydian-0.3.2/pydian/partials.py
+-rw-r--r--   0        0        0      702 2024-04-03 16:02:20.521013 pydian-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      371 1970-01-01 00:00:00.000000 pydian-0.3.2/PKG-INFO
```

### Comparing `pydian-0.3.1/LICENSE.md` & `pydian-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pydian-0.3.1/pydian/dataframes.py` & `pydian-0.3.2/pydian/dataframes.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.1/pydian/dicts.py` & `pydian-0.3.2/pydian/dicts.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.1/pydian/globs.py` & `pydian-0.3.2/pydian/globs.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.1/pydian/lib/types.py` & `pydian-0.3.2/pydian/lib/types.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.1/pydian/lib/util.py` & `pydian-0.3.2/pydian/lib/util.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.1/pydian/mapper.py` & `pydian-0.3.2/pydian/mapper.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.1/pydian/partials.py` & `pydian-0.3.2/pydian/partials.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.1/pyproject.toml` & `pydian-0.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "pydian"
-version = "0.3.1"
+version = "0.3.2"
 description = "Library for pythonic data interchange"
 authors = ["Eric Pan <eric.pan@stanford.edu>"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 jmespath = "^1.0.1"
+
+[tool.poetry.group.dataframes.dependencies]
 pandas = "^1.5.1"
 
 [tool.poetry.dev-dependencies]
 black = "^23.10.0"
 isort = "^5.12.0"
 mypy = "^1.6.1"
 pytest = "^7.4.3"
```

