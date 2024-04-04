# Comparing `tmp/meteoFrance_data-0.0.0.tar.gz` & `tmp/meteoFrance_data-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteoFrance_data-0.0.0.tar", last modified: Thu Apr  4 12:20:49 2024, max compression
+gzip compressed data, was "meteoFrance_data-1.0.0.tar", last modified: Thu Apr  4 13:00:17 2024, max compression
```

## Comparing `meteoFrance_data-0.0.0.tar` & `meteoFrance_data-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 12:20:47.917744 meteoFrance_data-0.0.0/
--rwxrwxrwx   0 root         (0) root         (0)      418 2024-04-04 12:20:49.188264 meteoFrance_data-0.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5769 2024-04-04 07:39:07.000000 meteoFrance_data-0.0.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)     2321 2024-04-04 12:19:12.000000 meteoFrance_data-0.0.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-04 12:20:49.228267 meteoFrance_data-0.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      695 2024-04-04 12:20:43.000000 meteoFrance_data-0.0.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 12:20:47.935665 meteoFrance_data-0.0.0/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 12:20:47.961551 meteoFrance_data-0.0.0/src/meteoFrance_data.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      418 2024-04-04 12:20:47.000000 meteoFrance_data-0.0.0/src/meteoFrance_data.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      782 2024-04-04 12:20:47.000000 meteoFrance_data-0.0.0/src/meteoFrance_data.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-04 12:20:47.000000 meteoFrance_data-0.0.0/src/meteoFrance_data.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       35 2024-04-04 12:20:47.000000 meteoFrance_data-0.0.0/src/meteoFrance_data.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       16 2024-04-04 12:20:47.000000 meteoFrance_data-0.0.0/src/meteoFrance_data.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 12:20:47.991420 meteoFrance_data-0.0.0/src/meteofrance_api/
--rwxrwxrwx   0 root         (0) root         (0)       97 2024-04-04 07:39:08.000000 meteoFrance_data-0.0.0/src/meteofrance_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       51 2024-04-04 07:39:08.000000 meteoFrance_data-0.0.0/src/meteofrance_api/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    26363 2024-04-04 07:39:08.000000 meteoFrance_data-0.0.0/src/meteofrance_api/client.py
--rwxrwxrwx   0 root         (0) root         (0)     3580 2024-04-04 07:39:08.000000 meteoFrance_data-0.0.0/src/meteofrance_api/const.py
--rwxrwxrwx   0 root         (0) root         (0)      145 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)     5925 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 12:20:48.021289 meteoFrance_data-0.0.0/src/meteofrance_api/model/
--rwxrwxrwx   0 root         (0) root         (0)      480 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/model/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3805 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/model/dictionary.py
--rwxrwxrwx   0 root         (0) root         (0)     4554 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/model/forecast.py
--rwxrwxrwx   0 root         (0) root         (0)     4354 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/model/observation.py
--rwxrwxrwx   0 root         (0) root         (0)     1349 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/model/picture_of_the_day.py
--rwxrwxrwx   0 root         (0) root         (0)     3612 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/model/place.py
--rwxrwxrwx   0 root         (0) root         (0)     3437 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/model/rain.py
--rwxrwxrwx   0 root         (0) root         (0)     8267 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/model/warning.py
--rwxrwxrwx   0 root         (0) root         (0)     1667 2024-04-04 07:39:09.000000 meteoFrance_data-0.0.0/src/meteofrance_api/session.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:00:16.355893 meteoFrance_data-1.0.0/
+-rwxrwxrwx   0 root         (0) root         (0)      418 2024-04-04 13:00:17.609475 meteoFrance_data-1.0.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5769 2024-04-04 07:39:07.000000 meteoFrance_data-1.0.0/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     2133 2024-04-04 12:57:32.000000 meteoFrance_data-1.0.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-04 13:00:17.641477 meteoFrance_data-1.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      716 2024-04-04 13:00:11.000000 meteoFrance_data-1.0.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:00:16.373815 meteoFrance_data-1.0.0/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:00:16.401692 meteoFrance_data-1.0.0/src/meteoFrance_data.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      418 2024-04-04 13:00:16.000000 meteoFrance_data-1.0.0/src/meteoFrance_data.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      782 2024-04-04 13:00:16.000000 meteoFrance_data-1.0.0/src/meteoFrance_data.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-04 13:00:16.000000 meteoFrance_data-1.0.0/src/meteoFrance_data.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       35 2024-04-04 13:00:16.000000 meteoFrance_data-1.0.0/src/meteoFrance_data.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       16 2024-04-04 13:00:16.000000 meteoFrance_data-1.0.0/src/meteoFrance_data.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:00:16.430566 meteoFrance_data-1.0.0/src/meteofrance_api/
+-rwxrwxrwx   0 root         (0) root         (0)       97 2024-04-04 07:39:08.000000 meteoFrance_data-1.0.0/src/meteofrance_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       51 2024-04-04 07:39:08.000000 meteoFrance_data-1.0.0/src/meteofrance_api/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26363 2024-04-04 07:39:08.000000 meteoFrance_data-1.0.0/src/meteofrance_api/client.py
+-rwxrwxrwx   0 root         (0) root         (0)     3580 2024-04-04 07:39:08.000000 meteoFrance_data-1.0.0/src/meteofrance_api/const.py
+-rwxrwxrwx   0 root         (0) root         (0)      145 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)     5925 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-04 13:00:16.462426 meteoFrance_data-1.0.0/src/meteofrance_api/model/
+-rwxrwxrwx   0 root         (0) root         (0)      480 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/model/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3805 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/model/dictionary.py
+-rwxrwxrwx   0 root         (0) root         (0)     4554 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/model/forecast.py
+-rwxrwxrwx   0 root         (0) root         (0)     4354 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/model/observation.py
+-rwxrwxrwx   0 root         (0) root         (0)     1349 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/model/picture_of_the_day.py
+-rwxrwxrwx   0 root         (0) root         (0)     3612 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/model/place.py
+-rwxrwxrwx   0 root         (0) root         (0)     3437 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/model/rain.py
+-rwxrwxrwx   0 root         (0) root         (0)     8267 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/model/warning.py
+-rwxrwxrwx   0 root         (0) root         (0)     1667 2024-04-04 07:39:09.000000 meteoFrance_data-1.0.0/src/meteofrance_api/session.py
```

### Comparing `meteoFrance_data-0.0.0/README.md` & `meteoFrance_data-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/pyproject.toml` & `meteoFrance_data-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [tool.poetry]
-name = "meteofrance-api"
+name = "meteofrance-data"
 version = "1.3.0"
 description = "Python client for Météo-France API."
-authors = ["oncleben31 <oncleben31@gmail.com>", "quentame <polletquentin74@me.com>", "HACF <contact@hacf.fr>"]
 license = "MIT"
-homepage = "https://github.com/hacf-fr/meteofrance-api"
-repository = "https://github.com/hacf-fr/meteofrance-api"
-documentation = "https://meteofrance-api.readthedocs.io"
+homepage = "https://github.com/hacf-fr/meteofrance-data"
+repository = "https://github.com/hacf-fr/meteofrance-data"
+documentation = "https://meteofrance-data.readthedocs.io"
 keywords = ["weather", "weather-api", "meteo"]
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: Production",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
 ]
 
-[tool.poetry.urls]
-Changelog = "https://github.com/hacf-fr/meteofrance-api/releases"
+
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "^2.25.1"
 urllib3 = "^1.26.18"
 pytz = ">=2020.4"
 typing-extensions = {version = ">=3.8.18,<5.0.0", python = "~3.8 || ~3.9 || ~3.10 || ~3.11"}
@@ -53,22 +51,22 @@
 sphinx-rtd-theme = "^1.3.0"
 sphinx-click = "^5.0.1"
 Pygments = "^2.15.0"
 types-requests = "^2.28.11"
 types-pytz = "^2023.3.0"
 
 [tool.poetry.scripts]
-meteofrance-api = "meteofrance_api.__main__:main"
+meteofrance-data = "meteofrance_data.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.run]
 branch = true
-source = ["meteofrance_api"]
+source = ["meteofrance_data"]
 
 [tool.coverage.report]
 show_missing = true
 # fail_under = 100 reduce targetwaiting for tests creation
 fail_under = 90
 
 [tool.mypy]
```

### Comparing `meteoFrance_data-0.0.0/setup.py` & `meteoFrance_data-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='meteoFrance_data',
+    version='1.0.0',
     author='Taoufik Bannour',
     author_email='taoufik.bannour.ext@suez.com',
     description='Un paquet des requêtes des données ouvertes de meteo-france',
     keywords='meteo,france, pypi, package',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `meteoFrance_data-0.0.0/src/meteoFrance_data.egg-info/SOURCES.txt` & `meteoFrance_data-1.0.0/src/meteoFrance_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/client.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/client.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/const.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/const.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/helpers.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/helpers.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/model/dictionary.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/model/dictionary.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/model/forecast.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/model/forecast.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/model/observation.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/model/observation.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/model/picture_of_the_day.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/model/picture_of_the_day.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/model/place.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/model/place.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/model/rain.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/model/rain.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/model/warning.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/model/warning.py`

 * *Files identical despite different names*

### Comparing `meteoFrance_data-0.0.0/src/meteofrance_api/session.py` & `meteoFrance_data-1.0.0/src/meteofrance_api/session.py`

 * *Files identical despite different names*

