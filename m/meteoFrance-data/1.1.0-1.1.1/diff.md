# Comparing `tmp/meteoFrance_data-1.1.0.tar.gz` & `tmp/meteoFrance_data-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteoFrance_data-1.1.0.tar", last modified: Thu Apr  4 13:06:47 2024, max compression
+gzip compressed data, was "meteoFrance_data-1.1.1.tar", last modified: Thu Apr  4 13:09:23 2024, max compression
```

## Comparing `meteoFrance_data-1.1.0.tar` & `meteoFrance_data-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:06:45.817804 meteoFrance_data-1.1.0/
--rwxrwxrwx   0 root         (0) root         (0)      418 2024-04-04 13:06:47.011545 meteoFrance_data-1.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5769 2024-04-04 07:39:07.000000 meteoFrance_data-1.1.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)     2241 2024-04-04 13:06:16.000000 meteoFrance_data-1.1.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-04 13:06:47.043547 meteoFrance_data-1.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      716 2024-04-04 13:06:32.000000 meteoFrance_data-1.1.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:06:45.836719 meteoFrance_data-1.1.0/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:06:45.862607 meteoFrance_data-1.1.0/src/meteoFrance_data.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      418 2024-04-04 13:06:45.000000 meteoFrance_data-1.1.0/src/meteoFrance_data.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      782 2024-04-04 13:06:45.000000 meteoFrance_data-1.1.0/src/meteoFrance_data.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-04 13:06:45.000000 meteoFrance_data-1.1.0/src/meteoFrance_data.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       35 2024-04-04 13:06:45.000000 meteoFrance_data-1.1.0/src/meteoFrance_data.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       16 2024-04-04 13:06:45.000000 meteoFrance_data-1.1.0/src/meteoFrance_data.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:06:45.900442 meteoFrance_data-1.1.0/src/meteofrance_api/
--rwxrwxrwx   0 root         (0) root         (0)       97 2024-04-04 07:39:08.000000 meteoFrance_data-1.1.0/src/meteofrance_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       51 2024-04-04 07:39:08.000000 meteoFrance_data-1.1.0/src/meteofrance_api/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    26363 2024-04-04 07:39:08.000000 meteoFrance_data-1.1.0/src/meteofrance_api/client.py
--rwxrwxrwx   0 root         (0) root         (0)     3580 2024-04-04 07:39:08.000000 meteoFrance_data-1.1.0/src/meteofrance_api/const.py
--rwxrwxrwx   0 root         (0) root         (0)      145 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)     5925 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:06:45.928320 meteoFrance_data-1.1.0/src/meteofrance_api/model/
--rwxrwxrwx   0 root         (0) root         (0)      480 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/model/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3805 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/model/dictionary.py
--rwxrwxrwx   0 root         (0) root         (0)     4554 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/model/forecast.py
--rwxrwxrwx   0 root         (0) root         (0)     4354 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/model/observation.py
--rwxrwxrwx   0 root         (0) root         (0)     1349 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/model/picture_of_the_day.py
--rwxrwxrwx   0 root         (0) root         (0)     3612 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/model/place.py
--rwxrwxrwx   0 root         (0) root         (0)     3437 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/model/rain.py
--rwxrwxrwx   0 root         (0) root         (0)     8267 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/model/warning.py
--rwxrwxrwx   0 root         (0) root         (0)     1667 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.0/src/meteofrance_api/session.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:09:21.687326 meteoFrance_data-1.1.1/
+-rwxrwxrwx   0 root         (0) root         (0)      418 2024-04-04 13:09:22.997934 meteoFrance_data-1.1.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5769 2024-04-04 07:39:07.000000 meteoFrance_data-1.1.1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     2241 2024-04-04 13:06:16.000000 meteoFrance_data-1.1.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-04 13:09:23.033936 meteoFrance_data-1.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      716 2024-04-04 13:09:14.000000 meteoFrance_data-1.1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:09:21.706244 meteoFrance_data-1.1.1/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:09:21.764986 meteoFrance_data-1.1.1/src/meteoFrance_data.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      418 2024-04-04 13:09:21.000000 meteoFrance_data-1.1.1/src/meteoFrance_data.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      797 2024-04-04 13:09:21.000000 meteoFrance_data-1.1.1/src/meteoFrance_data.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-04 13:09:21.000000 meteoFrance_data-1.1.1/src/meteoFrance_data.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       35 2024-04-04 13:09:21.000000 meteoFrance_data-1.1.1/src/meteoFrance_data.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       17 2024-04-04 13:09:21.000000 meteoFrance_data-1.1.1/src/meteoFrance_data.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:09:21.794855 meteoFrance_data-1.1.1/src/meteofrance_data/
+-rwxrwxrwx   0 root         (0) root         (0)       97 2024-04-04 07:39:08.000000 meteoFrance_data-1.1.1/src/meteofrance_data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       51 2024-04-04 07:39:08.000000 meteoFrance_data-1.1.1/src/meteofrance_data/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26363 2024-04-04 07:39:08.000000 meteoFrance_data-1.1.1/src/meteofrance_data/client.py
+-rwxrwxrwx   0 root         (0) root         (0)     3580 2024-04-04 07:39:08.000000 meteoFrance_data-1.1.1/src/meteofrance_data/const.py
+-rwxrwxrwx   0 root         (0) root         (0)      145 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)     5925 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:09:21.823728 meteoFrance_data-1.1.1/src/meteofrance_data/model/
+-rwxrwxrwx   0 root         (0) root         (0)      480 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/model/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3805 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/model/dictionary.py
+-rwxrwxrwx   0 root         (0) root         (0)     4554 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/model/forecast.py
+-rwxrwxrwx   0 root         (0) root         (0)     4354 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/model/observation.py
+-rwxrwxrwx   0 root         (0) root         (0)     1349 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/model/picture_of_the_day.py
+-rwxrwxrwx   0 root         (0) root         (0)     3612 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/model/place.py
+-rwxrwxrwx   0 root         (0) root         (0)     3437 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/model/rain.py
+-rwxrwxrwx   0 root         (0) root         (0)     8267 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/model/warning.py
+-rwxrwxrwx   0 root         (0) root         (0)     1667 2024-04-04 07:39:09.000000 meteoFrance_data-1.1.1/src/meteofrance_data/session.py
```

### Comparing `meteoFrance_data-1.1.0/README.md` & `meteoFrance_data-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/pyproject.toml` & `meteoFrance_data-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/setup.py` & `meteoFrance_data-1.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='meteoFrance_data',
-    version='1.1.0',
+    version='1.1.1',
     author='Taoufik Bannour',
     author_email='taoufik.bannour.ext@suez.com',
     description='Un paquet des requêtes des données ouvertes de meteo-france',
     keywords='meteo,france, pypi, package',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `meteoFrance_data-1.1.0/src/meteoFrance_data.egg-info/SOURCES.txt` & `meteoFrance_data-1.1.1/src/meteoFrance_data.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 pyproject.toml
 setup.py
 src/meteoFrance_data.egg-info/PKG-INFO
 src/meteoFrance_data.egg-info/SOURCES.txt
 src/meteoFrance_data.egg-info/dependency_links.txt
 src/meteoFrance_data.egg-info/requires.txt
 src/meteoFrance_data.egg-info/top_level.txt
-src/meteofrance_api/__init__.py
-src/meteofrance_api/__main__.py
-src/meteofrance_api/client.py
-src/meteofrance_api/const.py
-src/meteofrance_api/exceptions.py
-src/meteofrance_api/helpers.py
-src/meteofrance_api/session.py
-src/meteofrance_api/model/__init__.py
-src/meteofrance_api/model/dictionary.py
-src/meteofrance_api/model/forecast.py
-src/meteofrance_api/model/observation.py
-src/meteofrance_api/model/picture_of_the_day.py
-src/meteofrance_api/model/place.py
-src/meteofrance_api/model/rain.py
-src/meteofrance_api/model/warning.py
+src/meteofrance_data/__init__.py
+src/meteofrance_data/__main__.py
+src/meteofrance_data/client.py
+src/meteofrance_data/const.py
+src/meteofrance_data/exceptions.py
+src/meteofrance_data/helpers.py
+src/meteofrance_data/session.py
+src/meteofrance_data/model/__init__.py
+src/meteofrance_data/model/dictionary.py
+src/meteofrance_data/model/forecast.py
+src/meteofrance_data/model/observation.py
+src/meteofrance_data/model/picture_of_the_day.py
+src/meteofrance_data/model/place.py
+src/meteofrance_data/model/rain.py
+src/meteofrance_data/model/warning.py
```

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/client.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/client.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/const.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/const.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/helpers.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/helpers.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/model/dictionary.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/model/dictionary.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/model/forecast.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/model/forecast.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/model/observation.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/model/observation.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/model/picture_of_the_day.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/model/picture_of_the_day.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/model/place.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/model/place.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/model/rain.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/model/rain.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/model/warning.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/model/warning.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-1.1.0/src/meteofrance_api/session.py` & `meteoFrance_data-1.1.1/src/meteofrance_data/session.py`

 * *Files identical despite different names*

