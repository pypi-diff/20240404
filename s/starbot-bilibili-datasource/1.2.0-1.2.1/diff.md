# Comparing `tmp/starbot_bilibili_datasource-1.2.0.tar.gz` & `tmp/starbot_bilibili_datasource-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbot_bilibili_datasource-1.2.0.tar", max compression
+gzip compressed data, was "starbot_bilibili_datasource-1.2.1.tar", max compression
```

## Comparing `starbot_bilibili_datasource-1.2.0.tar` & `starbot_bilibili_datasource-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35184 2022-08-20 15:36:38.000000 starbot_bilibili_datasource-1.2.0/LICENSE
--rw-r--r--   0        0        0      569 2024-04-03 16:46:33.465280 starbot_bilibili_datasource-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1755 2024-04-03 16:46:08.314729 starbot_bilibili_datasource-1.2.0/README.md
--rw-r--r--   0        0        0      142 2024-04-03 16:35:42.636048 starbot_bilibili_datasource-1.2.0/starbot_datasource/__init__.py
--rw-r--r--   0        0        0      335 2024-04-03 14:52:03.679583 starbot_bilibili_datasource-1.2.0/starbot_datasource/config.json
--rw-r--r--   0        0        0        0 2023-11-29 15:05:36.521370 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__init__.py
--rw-r--r--   0        0        0      154 2024-03-31 17:12:02.466642 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2805 2024-04-03 16:43:45.795319 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     6890 2024-04-03 16:34:32.148663 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/datasource.cpython-310.pyc
--rw-r--r--   0        0        0      778 2024-03-31 17:12:02.467665 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/event.cpython-310.pyc
--rw-r--r--   0        0        0     7873 2024-03-31 17:12:02.666405 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0     2864 2024-04-03 16:43:20.396992 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/config.py
--rw-r--r--   0        0        0     7131 2024-04-03 14:56:54.518659 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/datasource.py
--rw-r--r--   0        0        0      552 2023-11-29 15:24:08.586640 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/event.py
--rw-r--r--   0        0        0    10672 2024-03-10 17:32:23.632686 starbot_bilibili_datasource-1.2.0/starbot_datasource/core/model.py
--rw-r--r--   0        0        0        0 2023-11-29 15:05:43.778052 starbot_bilibili_datasource-1.2.0/starbot_datasource/exception/__init__.py
--rw-r--r--   0        0        0      159 2024-03-31 17:12:02.859493 starbot_bilibili_datasource-1.2.0/starbot_datasource/exception/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      770 2024-03-31 17:12:02.861536 starbot_bilibili_datasource-1.2.0/starbot_datasource/exception/__pycache__/ApiException.cpython-310.pyc
--rw-r--r--   0        0        0      632 2024-03-31 17:12:02.860533 starbot_bilibili_datasource-1.2.0/starbot_datasource/exception/__pycache__/DataSourceException.cpython-310.pyc
--rw-r--r--   0        0        0      264 2023-11-13 15:14:18.053679 starbot_bilibili_datasource-1.2.0/starbot_datasource/exception/ApiException.py
--rw-r--r--   0        0        0      214 2023-11-29 15:09:01.325994 starbot_bilibili_datasource-1.2.0/starbot_datasource/exception/DataSourceException.py
--rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 starbot_bilibili_datasource-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-08-20 15:36:38.000000 starbot_bilibili_datasource-1.2.1/LICENSE
+-rw-r--r--   0        0        0      567 2024-04-04 17:41:19.302948 starbot_bilibili_datasource-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1755 2024-04-03 16:46:08.314729 starbot_bilibili_datasource-1.2.1/README.md
+-rw-r--r--   0        0        0      142 2024-04-03 16:35:42.636048 starbot_bilibili_datasource-1.2.1/starbot_datasource/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-04 17:03:52.435532 starbot_bilibili_datasource-1.2.1/starbot_datasource/config.json
+-rw-r--r--   0        0        0        0 2023-11-29 15:05:36.521370 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__init__.py
+-rw-r--r--   0        0        0      154 2024-03-31 17:12:02.466642 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2805 2024-04-03 16:43:45.795319 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     6890 2024-04-03 16:34:32.148663 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/datasource.cpython-310.pyc
+-rw-r--r--   0        0        0      778 2024-03-31 17:12:02.467665 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/event.cpython-310.pyc
+-rw-r--r--   0        0        0     7873 2024-03-31 17:12:02.666405 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     2864 2024-04-03 16:43:20.396992 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/config.py
+-rw-r--r--   0        0        0     7131 2024-04-03 14:56:54.518659 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/datasource.py
+-rw-r--r--   0        0        0      552 2023-11-29 15:24:08.586640 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/event.py
+-rw-r--r--   0        0        0    10672 2024-03-10 17:32:23.632686 starbot_bilibili_datasource-1.2.1/starbot_datasource/core/model.py
+-rw-r--r--   0        0        0        0 2023-11-29 15:05:43.778052 starbot_bilibili_datasource-1.2.1/starbot_datasource/exception/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-31 17:12:02.859493 starbot_bilibili_datasource-1.2.1/starbot_datasource/exception/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      770 2024-03-31 17:12:02.861536 starbot_bilibili_datasource-1.2.1/starbot_datasource/exception/__pycache__/ApiException.cpython-310.pyc
+-rw-r--r--   0        0        0      632 2024-03-31 17:12:02.860533 starbot_bilibili_datasource-1.2.1/starbot_datasource/exception/__pycache__/DataSourceException.cpython-310.pyc
+-rw-r--r--   0        0        0      264 2023-11-13 15:14:18.053679 starbot_bilibili_datasource-1.2.1/starbot_datasource/exception/ApiException.py
+-rw-r--r--   0        0        0      214 2023-11-29 15:09:01.325994 starbot_bilibili_datasource-1.2.1/starbot_datasource/exception/DataSourceException.py
+-rw-r--r--   0        0        0     2454 1970-01-01 00:00:00.000000 starbot_bilibili_datasource-1.2.1/PKG-INFO
```

### Comparing `starbot_bilibili_datasource-1.2.0/LICENSE` & `starbot_bilibili_datasource-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/pyproject.toml` & `starbot_bilibili_datasource-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "starbot-bilibili-datasource"
-version = "1.2.0"
+version = "1.2.1"
 description = "StarBot 推送配置数据源"
 keywords = ["starbot", "bilibili", "bot"]
 license = "AGPL-3.0-only"
 authors = ["Starlwr <lwr1104@qq.com>"]
 readme = "README.md"
 repository = "https://github.com/Starlwr/StarBotDataSource"
 packages = [{ include = "starbot_datasource" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 starbot-executor = "^1.4.0"
-pydantic = "^2.5.2"
+pydantic = "^1.9"
 loguru = "^0.7.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `starbot_bilibili_datasource-1.2.0/README.md` & `starbot_bilibili_datasource-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/config.cpython-310.pyc` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/datasource.cpython-310.pyc` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/datasource.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/event.cpython-310.pyc` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/event.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/core/__pycache__/model.cpython-310.pyc` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/core/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/core/config.py` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/core/config.py`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/core/datasource.py` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/core/datasource.py`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/core/event.py` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/core/event.py`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/core/model.py` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/core/model.py`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/exception/__pycache__/ApiException.cpython-310.pyc` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/exception/__pycache__/ApiException.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/starbot_datasource/exception/__pycache__/DataSourceException.cpython-310.pyc` & `starbot_bilibili_datasource-1.2.1/starbot_datasource/exception/__pycache__/DataSourceException.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `starbot_bilibili_datasource-1.2.0/PKG-INFO` & `starbot_bilibili_datasource-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: starbot-bilibili-datasource
-Version: 1.2.0
+Version: 1.2.1
 Summary: StarBot 推送配置数据源
 Home-page: https://github.com/Starlwr/StarBotDataSource
 License: AGPL-3.0-only
 Keywords: starbot,bilibili,bot
 Author: Starlwr
 Author-email: lwr1104@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: pydantic (>=2.5.2,<3.0.0)
+Requires-Dist: pydantic (>=1.9,<2.0)
 Requires-Dist: starbot-executor (>=1.4.0,<2.0.0)
 Project-URL: Repository, https://github.com/Starlwr/StarBotDataSource
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # StarBotDataSource
```

