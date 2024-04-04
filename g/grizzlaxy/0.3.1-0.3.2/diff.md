# Comparing `tmp/grizzlaxy-0.3.1.tar.gz` & `tmp/grizzlaxy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzlaxy-0.3.1.tar", max compression
+gzip compressed data, was "grizzlaxy-0.3.2.tar", max compression
```

## Comparing `grizzlaxy-0.3.1.tar` & `grizzlaxy-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-06-22 00:33:43.206354 grizzlaxy-0.3.1/LICENSE
--rw-r--r--   0        0        0      151 2023-06-26 19:43:56.507337 grizzlaxy-0.3.1/README.md
--rw-r--r--   0        0        0      159 2023-11-16 23:39:09.026477 grizzlaxy-0.3.1/grizzlaxy/__init__.py
--rw-r--r--   0        0        0     4502 2024-01-31 22:21:34.053999 grizzlaxy-0.3.1/grizzlaxy/auth.py
--rw-r--r--   0        0        0     9556 2024-03-22 19:31:59.186558 grizzlaxy-0.3.1/grizzlaxy/cli.py
--rw-r--r--   0        0        0        0 2024-03-22 19:57:27.525049 grizzlaxy-0.3.1/grizzlaxy/components/__init__.py
--rw-r--r--   0        0        0     2311 2024-01-30 01:40:07.091697 grizzlaxy-0.3.1/grizzlaxy/find.py
--rw-r--r--   0        0        0      367 2023-09-26 04:06:50.584404 grizzlaxy-0.3.1/grizzlaxy/index-style.css
--rw-r--r--   0        0        0      256 2024-01-30 01:40:07.085191 grizzlaxy-0.3.1/grizzlaxy/index-template.html
--rw-r--r--   0        0        0     1684 2023-12-09 00:51:54.291186 grizzlaxy-0.3.1/grizzlaxy/index.py
--rw-r--r--   0        0        0     4099 2024-01-31 22:33:51.017006 grizzlaxy-0.3.1/grizzlaxy/reload.py
--rw-r--r--   0        0        0     4004 2024-01-31 22:24:52.872729 grizzlaxy-0.3.1/grizzlaxy/utils.py
--rw-r--r--   0        0        0       18 2024-03-27 18:16:25.010088 grizzlaxy-0.3.1/grizzlaxy/version.py
--rw-r--r--   0        0        0      856 2024-03-27 18:16:24.988505 grizzlaxy-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 grizzlaxy-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-22 00:33:43.206354 grizzlaxy-0.3.2/LICENSE
+-rw-r--r--   0        0        0      151 2023-06-26 19:43:56.507337 grizzlaxy-0.3.2/README.md
+-rw-r--r--   0        0        0      159 2023-11-16 23:39:09.026477 grizzlaxy-0.3.2/grizzlaxy/__init__.py
+-rw-r--r--   0        0        0     4502 2024-01-31 22:21:34.053999 grizzlaxy-0.3.2/grizzlaxy/auth.py
+-rw-r--r--   0        0        0     9556 2024-03-22 19:31:59.186558 grizzlaxy-0.3.2/grizzlaxy/cli.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:57:27.525049 grizzlaxy-0.3.2/grizzlaxy/components/__init__.py
+-rw-r--r--   0        0        0     2311 2024-01-30 01:40:07.091697 grizzlaxy-0.3.2/grizzlaxy/find.py
+-rw-r--r--   0        0        0      367 2023-09-26 04:06:50.584404 grizzlaxy-0.3.2/grizzlaxy/index-style.css
+-rw-r--r--   0        0        0      256 2024-01-30 01:40:07.085191 grizzlaxy-0.3.2/grizzlaxy/index-template.html
+-rw-r--r--   0        0        0     1684 2023-12-09 00:51:54.291186 grizzlaxy-0.3.2/grizzlaxy/index.py
+-rw-r--r--   0        0        0     4099 2024-01-31 22:33:51.017006 grizzlaxy-0.3.2/grizzlaxy/reload.py
+-rw-r--r--   0        0        0     4004 2024-01-31 22:24:52.872729 grizzlaxy-0.3.2/grizzlaxy/utils.py
+-rw-r--r--   0        0        0       18 2024-04-04 15:51:21.786846 grizzlaxy-0.3.2/grizzlaxy/version.py
+-rw-r--r--   0        0        0      856 2024-04-04 15:51:21.765707 grizzlaxy-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 grizzlaxy-0.3.2/PKG-INFO
```

### Comparing `grizzlaxy-0.3.1/LICENSE` & `grizzlaxy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.1/grizzlaxy/auth.py` & `grizzlaxy-0.3.2/grizzlaxy/auth.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.1/grizzlaxy/cli.py` & `grizzlaxy-0.3.2/grizzlaxy/cli.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.1/grizzlaxy/find.py` & `grizzlaxy-0.3.2/grizzlaxy/find.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.1/grizzlaxy/index.py` & `grizzlaxy-0.3.2/grizzlaxy/index.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.1/grizzlaxy/reload.py` & `grizzlaxy-0.3.2/grizzlaxy/reload.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.1/grizzlaxy/utils.py` & `grizzlaxy-0.3.2/grizzlaxy/utils.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.3.1/pyproject.toml` & `grizzlaxy-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "grizzlaxy"
-version = "0.3.1"
+version = "0.3.2"
 description = "Create an app from a galaxy of starbears"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 authlib = "^1.2.0"
 httpx = "^0.24.1"
 itsdangerous = "^2.1.2"
-starbear = "^0.1.0"
+starbear = "^0.1.3"
 ovld = "^0.3.2"
 jurigged = "^0.5.5"
 pyyaml = {version = "^6.0.1", optional = true}
 sentry-sdk = {extras = ["starlette"], version = "^1.35.0", optional = true}
 sse-starlette = "^1.8.2"
-gifnoc = "^0.2.1"
+gifnoc = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.3.0"
 ruff = "^0.0.274"
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
```

### Comparing `grizzlaxy-0.3.1/PKG-INFO` & `grizzlaxy-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: grizzlaxy
-Version: 0.3.1
+Version: 0.3.2
 Summary: Create an app from a galaxy of starbears
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: sentry
 Provides-Extra: yaml
 Requires-Dist: authlib (>=1.2.0,<2.0.0)
-Requires-Dist: gifnoc (>=0.2.1,<0.3.0)
+Requires-Dist: gifnoc (>=0.3.0,<0.4.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: itsdangerous (>=2.1.2,<3.0.0)
 Requires-Dist: jurigged (>=0.5.5,<0.6.0)
 Requires-Dist: ovld (>=0.3.2,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0) ; extra == "yaml"
 Requires-Dist: sentry-sdk[starlette] (>=1.35.0,<2.0.0) ; extra == "sentry"
 Requires-Dist: sse-starlette (>=1.8.2,<2.0.0)
-Requires-Dist: starbear (>=0.1.0,<0.2.0)
+Requires-Dist: starbear (>=0.1.3,<0.2.0)
 Description-Content-Type: text/markdown
 
 
 # Grizzlaxy
 
 Define apps in the file hierarchy using starbear and start them under a single server with OAuth and a permissions file using grizzlaxy.
```

