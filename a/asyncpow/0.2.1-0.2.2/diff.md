# Comparing `tmp/asyncpow-0.2.1.tar.gz` & `tmp/asyncpow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpow-0.2.1.tar", max compression
+gzip compressed data, was "asyncpow-0.2.2.tar", max compression
```

## Comparing `asyncpow-0.2.1.tar` & `asyncpow-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6694 2024-03-30 21:45:26.594922 asyncpow-0.2.1/README.md
--rw-r--r--   0        0        0     1187 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/__init__.py
--rw-r--r--   0        0        0     4916 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/apis/media.py
--rw-r--r--   0        0        0     2768 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/apis/movie.py
--rw-r--r--   0        0        0     4412 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/apis/search.py
--rw-r--r--   0        0        0     2977 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/apis/status.py
--rw-r--r--   0        0        0     2825 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/apis/tv.py
--rw-r--r--   0        0        0     1148 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/const.py
--rw-r--r--   0        0        0     1664 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/exceptions.py
--rw-r--r--   0        0        0     3728 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/models/common.py
--rw-r--r--   0        0        0     2339 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/models/media.py
--rw-r--r--   0        0        0     4022 2024-03-30 21:45:26.594922 asyncpow-0.2.1/asyncpow/models/movie.py
--rw-r--r--   0        0        0     2812 2024-03-30 21:45:26.598922 asyncpow-0.2.1/asyncpow/models/search.py
--rw-r--r--   0        0        0     1517 2024-03-30 21:45:26.598922 asyncpow-0.2.1/asyncpow/models/status.py
--rw-r--r--   0        0        0     3102 2024-03-30 21:45:26.598922 asyncpow-0.2.1/asyncpow/models/tv.py
--rw-r--r--   0        0        0     4264 2024-03-30 21:45:26.598922 asyncpow-0.2.1/asyncpow/overseerr.py
--rw-r--r--   0        0        0        0 2024-03-30 21:45:26.598922 asyncpow-0.2.1/asyncpow/py.typed
--rw-r--r--   0        0        0     4067 2024-03-30 21:45:26.598922 asyncpow-0.2.1/asyncpow/utils/http.py
--rw-r--r--   0        0        0     2919 2024-03-30 21:46:11.182826 asyncpow-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     6694 2024-04-04 17:59:37.992839 asyncpow-0.2.2/README.md
+-rw-r--r--   0        0        0     1187 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/__init__.py
+-rw-r--r--   0        0        0     4916 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/apis/media.py
+-rw-r--r--   0        0        0     2768 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/apis/movie.py
+-rw-r--r--   0        0        0     4412 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/apis/search.py
+-rw-r--r--   0        0        0     2977 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/apis/status.py
+-rw-r--r--   0        0        0     2825 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/apis/tv.py
+-rw-r--r--   0        0        0     1148 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/const.py
+-rw-r--r--   0        0        0     1664 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/exceptions.py
+-rw-r--r--   0        0        0     3728 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/models/common.py
+-rw-r--r--   0        0        0     2339 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/models/media.py
+-rw-r--r--   0        0        0     4022 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/models/movie.py
+-rw-r--r--   0        0        0     2812 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/models/search.py
+-rw-r--r--   0        0        0     1517 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/models/status.py
+-rw-r--r--   0        0        0     3116 2024-04-04 17:59:37.992839 asyncpow-0.2.2/asyncpow/models/tv.py
+-rw-r--r--   0        0        0     4264 2024-04-04 17:59:37.996839 asyncpow-0.2.2/asyncpow/overseerr.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:59:37.996839 asyncpow-0.2.2/asyncpow/py.typed
+-rw-r--r--   0        0        0     4067 2024-04-04 17:59:37.996839 asyncpow-0.2.2/asyncpow/utils/http.py
+-rw-r--r--   0        0        0     2919 2024-04-04 18:00:35.145641 asyncpow-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.2.2/PKG-INFO
```

### Comparing `asyncpow-0.2.1/README.md` & `asyncpow-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/__init__.py` & `asyncpow-0.2.2/asyncpow/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/apis/media.py` & `asyncpow-0.2.2/asyncpow/apis/media.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/apis/movie.py` & `asyncpow-0.2.2/asyncpow/apis/movie.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/apis/search.py` & `asyncpow-0.2.2/asyncpow/apis/search.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/apis/status.py` & `asyncpow-0.2.2/asyncpow/apis/status.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/apis/tv.py` & `asyncpow-0.2.2/asyncpow/apis/tv.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/const.py` & `asyncpow-0.2.2/asyncpow/const.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/exceptions.py` & `asyncpow-0.2.2/asyncpow/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/models/common.py` & `asyncpow-0.2.2/asyncpow/models/common.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/models/media.py` & `asyncpow-0.2.2/asyncpow/models/media.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/models/movie.py` & `asyncpow-0.2.2/asyncpow/models/movie.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/models/search.py` & `asyncpow-0.2.2/asyncpow/models/search.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/models/status.py` & `asyncpow-0.2.2/asyncpow/models/status.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/models/tv.py` & `asyncpow-0.2.2/asyncpow/models/tv.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     createdBy: list[CreatedByModel]
     episodeRunTime: list[int]
     firstAirDate: str
     genres: list[GenreModel]
     homepage: str
     inProduction: bool
     languages: list[str]
-    lastAirDate: str
+    lastAirDate: str | None = None
     lastEpisodeToAir: EpisodeModel | None = None
     name: str
     nextEpisodeToAir: EpisodeModel | None = None
     networks: list[ProductionCompanyModel]
     numberOfEpisodes: int
     numberOfSeasons: int
     originCountry: list[str]
```

### Comparing `asyncpow-0.2.1/asyncpow/overseerr.py` & `asyncpow-0.2.2/asyncpow/overseerr.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/asyncpow/utils/http.py` & `asyncpow-0.2.2/asyncpow/utils/http.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.1/pyproject.toml` & `asyncpow-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncpow"
-version = "0.2.1"
+version = "0.2.2"
 description = "Asynchronous Python Overseerr Wrapper"
 authors = ["Steven Marks - TotalDebug"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/totaldebug/asyncpow"
 repository = "https://github.com/totaldebug/asyncpow"
 classifiers = [
```

### Comparing `asyncpow-0.2.1/PKG-INFO` & `asyncpow-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpow
-Version: 0.2.1
+Version: 0.2.2
 Summary: Asynchronous Python Overseerr Wrapper
 Home-page: https://github.com/totaldebug/asyncpow
 License: MIT
 Keywords: wled,api,async,client
 Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug
 Requires-Python: >=3.12,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asyncpow Version: 0.2.1 Summary: Asynchronous
+Metadata-Version: 2.1 Name: asyncpow Version: 0.2.2 Summary: Asynchronous
 Python Overseerr Wrapper Home-page: https://github.com/totaldebug/asyncpow
 License: MIT Keywords: wled,api,async,client Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug Requires-Python: >=3.12,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.12
```

