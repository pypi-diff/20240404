# Comparing `tmp/pydian-0.3.3a0.tar.gz` & `tmp/pydian-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydian-0.3.3a0.tar", max compression
+gzip compressed data, was "pydian-0.3.4.tar", max compression
```

## Comparing `pydian-0.3.3a0.tar` & `pydian-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-02-27 21:22:50.771826 pydian-0.3.3a0/LICENSE.md
--rw-r--r--   0        0        0      133 2023-02-27 19:38:00.361634 pydian-0.3.3a0/pydian/__init__.py
--rw-r--r--   0        0        0    14871 2023-11-18 01:22:42.900729 pydian-0.3.3a0/pydian/dataframes.py
--rw-r--r--   0        0        0     7556 2023-11-18 01:22:42.900974 pydian-0.3.3a0/pydian/dicts.py
--rw-r--r--   0        0        0     1592 2023-11-18 01:22:42.901064 pydian-0.3.3a0/pydian/globs.py
--rw-r--r--   0        0        0        0 2023-02-22 00:10:14.742269 pydian-0.3.3a0/pydian/lib/__init__.py
--rw-r--r--   0        0        0     1360 2023-11-18 01:22:14.531473 pydian-0.3.3a0/pydian/lib/types.py
--rw-r--r--   0        0        0     3000 2023-11-18 01:22:42.901995 pydian-0.3.3a0/pydian/lib/util.py
--rw-r--r--   0        0        0     2257 2023-11-18 01:22:42.902194 pydian-0.3.3a0/pydian/mapper.py
--rw-r--r--   0        0        0     5066 2023-11-18 01:22:42.902418 pydian-0.3.3a0/pydian/partials.py
--rw-r--r--   0        0        0      735 2024-04-04 14:24:16.289441 pydian-0.3.3a0/pyproject.toml
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 pydian-0.3.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-27 21:22:50.771826 pydian-0.3.4/LICENSE.md
+-rw-r--r--   0        0        0      133 2023-02-27 19:38:00.361634 pydian-0.3.4/pydian/__init__.py
+-rw-r--r--   0        0        0    14871 2023-11-18 01:22:42.900729 pydian-0.3.4/pydian/dataframes.py
+-rw-r--r--   0        0        0     7556 2023-11-18 01:22:42.900974 pydian-0.3.4/pydian/dicts.py
+-rw-r--r--   0        0        0     1592 2023-11-18 01:22:42.901064 pydian-0.3.4/pydian/globs.py
+-rw-r--r--   0        0        0        0 2023-02-22 00:10:14.742269 pydian-0.3.4/pydian/lib/__init__.py
+-rw-r--r--   0        0        0     1360 2023-11-18 01:22:14.531473 pydian-0.3.4/pydian/lib/types.py
+-rw-r--r--   0        0        0     3000 2023-11-18 01:22:42.901995 pydian-0.3.4/pydian/lib/util.py
+-rw-r--r--   0        0        0     2257 2023-11-18 01:22:42.902194 pydian-0.3.4/pydian/mapper.py
+-rw-r--r--   0        0        0     5066 2023-11-18 01:22:42.902418 pydian-0.3.4/pydian/partials.py
+-rw-r--r--   0        0        0      734 2024-04-04 14:30:32.992475 pydian-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 pydian-0.3.4/PKG-INFO
```

### Comparing `pydian-0.3.3a0/LICENSE.md` & `pydian-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pydian-0.3.3a0/pydian/dataframes.py` & `pydian-0.3.4/pydian/dataframes.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.3a0/pydian/dicts.py` & `pydian-0.3.4/pydian/dicts.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.3a0/pydian/globs.py` & `pydian-0.3.4/pydian/globs.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.3a0/pydian/lib/types.py` & `pydian-0.3.4/pydian/lib/types.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.3a0/pydian/lib/util.py` & `pydian-0.3.4/pydian/lib/util.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.3a0/pydian/mapper.py` & `pydian-0.3.4/pydian/mapper.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.3a0/pydian/partials.py` & `pydian-0.3.4/pydian/partials.py`

 * *Files identical despite different names*

### Comparing `pydian-0.3.3a0/pyproject.toml` & `pydian-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydian"
-version = "0.3.3a"
+version = "0.3.4"
 description = "Library for pythonic data interchange"
 authors = ["Eric Pan <eric.pan@stanford.edu>"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 jmespath = "^1.0.1"
 pandas = { version = "^2.0.0", optional = true }
```

