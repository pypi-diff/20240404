# Comparing `tmp/aixblock_ml-0.0.3.tar.gz` & `tmp/aixblock_ml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_ml-0.0.3.tar", max compression
+gzip compressed data, was "aixblock_ml-0.0.4.tar", max compression
```

## Comparing `aixblock_ml-0.0.3.tar` & `aixblock_ml-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       11 2024-04-03 07:28:40.006140 aixblock_ml-0.0.3/README.md
--rw-r--r--   0        0        0       84 2024-04-01 06:20:49.108490 aixblock_ml-0.0.3/aixblock_ml/__init__.py
--rw-r--r--   0        0        0     8928 2024-04-03 08:23:03.325146 aixblock_ml-0.0.3/aixblock_ml/api.py
--rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.3/aixblock_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2024-04-01 06:20:49.119434 aixblock_ml-0.0.3/aixblock_ml/default_configs/README.md
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.3/aixblock_ml/default_configs/_wsgi.py
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.3/aixblock_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.3/aixblock_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0     2139 2024-04-04 03:08:16.489392 aixblock_ml-0.0.3/aixblock_ml/default_configs/model.py
--rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.3/aixblock_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.3/aixblock_ml/exceptions.py
--rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.3/aixblock_ml/helpers.py
--rw-r--r--   0        0        0    34692 2024-04-03 08:23:03.374785 aixblock_ml-0.0.3/aixblock_ml/model.py
--rw-r--r--   0        0        0     7487 2024-04-04 02:14:25.160523 aixblock_ml-0.0.3/aixblock_ml/server.py
--rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.3/aixblock_ml/templates/preview.html
--rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.3/aixblock_ml/utils.py
--rw-r--r--   0        0        0      264 2024-04-04 03:15:14.266823 aixblock_ml-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 aixblock_ml-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-04-03 07:28:40.006140 aixblock_ml-0.0.4/README.md
+-rw-r--r--   0        0        0       84 2024-04-04 08:01:18.783734 aixblock_ml-0.0.4/aixblock_ml/__init__.py
+-rw-r--r--   0        0        0     8928 2024-04-03 08:23:03.325146 aixblock_ml-0.0.4/aixblock_ml/api.py
+-rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.4/aixblock_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2024-04-01 06:20:49.119434 aixblock_ml-0.0.4/aixblock_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.4/aixblock_ml/default_configs/_wsgi.py
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.4/aixblock_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.4/aixblock_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0     2139 2024-04-04 03:08:16.489392 aixblock_ml-0.0.4/aixblock_ml/default_configs/model.py
+-rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.4/aixblock_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.4/aixblock_ml/exceptions.py
+-rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.4/aixblock_ml/helpers.py
+-rw-r--r--   0        0        0    34692 2024-04-03 08:23:03.374785 aixblock_ml-0.0.4/aixblock_ml/model.py
+-rw-r--r--   0        0        0     7487 2024-04-04 02:14:25.160523 aixblock_ml-0.0.4/aixblock_ml/server.py
+-rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.4/aixblock_ml/templates/preview.html
+-rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.4/aixblock_ml/utils.py
+-rw-r--r--   0        0        0      313 2024-04-04 08:03:41.454706 aixblock_ml-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 aixblock_ml-0.0.4/PKG-INFO
```

### Comparing `aixblock_ml-0.0.3/aixblock_ml/api.py` & `aixblock_ml-0.0.4/aixblock_ml/api.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/default_configs/README.md` & `aixblock_ml-0.0.4/aixblock_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/default_configs/_wsgi.py` & `aixblock_ml-0.0.4/aixblock_ml/default_configs/_wsgi.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/default_configs/_wsgi.py.tmpl` & `aixblock_ml-0.0.4/aixblock_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/default_configs/docker-compose.yml` & `aixblock_ml-0.0.4/aixblock_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/default_configs/model.py` & `aixblock_ml-0.0.4/aixblock_ml/default_configs/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/exceptions.py` & `aixblock_ml-0.0.4/aixblock_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/helpers.py` & `aixblock_ml-0.0.4/aixblock_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/model.py` & `aixblock_ml-0.0.4/aixblock_ml/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/server.py` & `aixblock_ml-0.0.4/aixblock_ml/server.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.3/aixblock_ml/utils.py` & `aixblock_ml-0.0.4/aixblock_ml/utils.py`

 * *Files identical despite different names*

