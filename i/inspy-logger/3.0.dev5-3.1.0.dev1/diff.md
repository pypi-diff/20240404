# Comparing `tmp/inspy_logger-3.0.dev5.tar.gz` & `tmp/inspy_logger-3.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspy_logger-3.0.dev5.tar", max compression
+gzip compressed data, was "inspy_logger-3.1.0.dev1.tar", max compression
```

## Comparing `inspy_logger-3.0.dev5.tar` & `inspy_logger-3.1.0.dev1.tar`

### file list

```diff
@@ -1,14 +1,39 @@
--rw-r--r--   0        0        0      674 2023-12-16 20:26:28.764394 inspy_logger-3.0.dev5/inspy_logger/__about__.py
--rw-r--r--   0        0        0    10959 2023-12-15 03:05:07.512950 inspy_logger-3.0.dev5/inspy_logger/__init__.py
--rw-r--r--   0        0        0     4239 2023-12-07 05:55:57.981004 inspy_logger-3.0.dev5/inspy_logger/errors/__init__.py
--rw-r--r--   0        0        0     5888 2023-12-11 20:00:16.980614 inspy_logger-3.0.dev5/inspy_logger/helpers/__init__.py
--rw-r--r--   0        0        0     4937 2023-12-14 06:12:18.292256 inspy_logger-3.0.dev5/inspy_logger/helpers/base_classes.py
--rw-r--r--   0        0        0     3693 2023-12-07 05:55:57.982998 inspy_logger-3.0.dev5/inspy_logger/helpers/cache.py
--rw-r--r--   0        0        0    10605 2023-12-07 05:55:57.983995 inspy_logger-3.0.dev5/inspy_logger/helpers/network.py
--rw-r--r--   0        0        0      992 2023-12-07 05:54:44.333226 inspy_logger-3.0.dev5/inspy_logger/manifest.py
--rw-r--r--   0        0        0     2750 2023-12-16 21:12:50.762553 inspy_logger-3.0.dev5/inspy_logger/Scripts/main.py
--rw-r--r--   0        0        0     7414 2023-12-18 22:32:27.455674 inspy_logger-3.0.dev5/inspy_logger/version.py
--rw-r--r--   0        0        0      885 2023-12-07 05:54:44.295896 inspy_logger-3.0.dev5/LICENSE.md
--rw-r--r--   0        0        0     2061 2023-12-19 00:45:49.515905 inspy_logger-3.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     2500 2023-12-07 05:54:44.296909 inspy_logger-3.0.dev5/README.md
--rw-r--r--   0        0        0     4239 1970-01-01 00:00:00.000000 inspy_logger-3.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0      501 2024-03-26 19:46:07.239938 inspy_logger-3.1.0.dev1/inspy_logger/__about__.py
+-rw-r--r--   0        0        0     3421 2024-04-04 00:35:10.880027 inspy_logger-3.1.0.dev1/inspy_logger/__init__.py
+-rw-r--r--   0        0        0     2504 2024-04-02 01:36:41.775167 inspy_logger-3.1.0.dev1/inspy_logger/common/__init__.py
+-rw-r--r--   0        0        0     1067 2024-03-29 01:40:59.779229 inspy_logger-3.1.0.dev1/inspy_logger/common/meta.py
+-rw-r--r--   0        0        0      211 2024-04-02 01:23:15.695772 inspy_logger-3.1.0.dev1/inspy_logger/config/__init__.py
+-rw-r--r--   0        0        0     3798 2024-04-04 02:23:50.449117 inspy_logger-3.1.0.dev1/inspy_logger/config/dirs.py
+-rw-r--r--   0        0        0      440 2024-04-02 01:25:49.145829 inspy_logger-3.1.0.dev1/inspy_logger/config/levels.py
+-rw-r--r--   0        0        0      475 2024-04-02 01:35:35.543818 inspy_logger-3.1.0.dev1/inspy_logger/constants.py
+-rw-r--r--   0        0        0    21612 2024-04-04 00:32:11.168928 inspy_logger-3.1.0.dev1/inspy_logger/engine/__init__.py
+-rw-r--r--   0        0        0     1090 2024-04-01 23:37:24.100399 inspy_logger-3.1.0.dev1/inspy_logger/engine/errors.py
+-rw-r--r--   0        0        0     1374 2024-01-06 00:11:42.646732 inspy_logger-3.1.0.dev1/inspy_logger/engine/handlers.py
+-rw-r--r--   0        0        0     4239 2023-12-07 05:55:57.981004 inspy_logger-3.1.0.dev1/inspy_logger/errors/__init__.py
+-rw-r--r--   0        0        0    15186 2024-04-04 10:49:26.067126 inspy_logger-3.1.0.dev1/inspy_logger/helpers/__init__.py
+-rw-r--r--   0        0        0     5047 2024-01-21 17:17:03.926574 inspy_logger-3.1.0.dev1/inspy_logger/helpers/base_classes.py
+-rw-r--r--   0        0        0     1094 2024-01-05 21:31:57.455076 inspy_logger-3.1.0.dev1/inspy_logger/helpers/command_line/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-21 18:01:40.981091 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/__init__.py
+-rw-r--r--   0        0        0     5054 2024-03-29 22:15:05.177429 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/environment.py
+-rw-r--r--   0        0        0        0 2023-12-24 09:42:32.088107 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/system/__init__.py
+-rw-r--r--   0        0        0     1650 2023-12-24 22:55:21.616920 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/system/processor/__init__.py
+-rw-r--r--   0        0        0      572 2023-12-24 22:25:41.517257 inspy_logger-3.1.0.dev1/inspy_logger/helpers/debug/system/winx/__init__.py
+-rw-r--r--   0        0        0     9257 2024-04-01 21:11:09.678230 inspy_logger-3.1.0.dev1/inspy_logger/helpers/decorators.py
+-rw-r--r--   0        0        0     9924 2024-03-29 22:36:21.862636 inspy_logger-3.1.0.dev1/inspy_logger/helpers/descriptors.py
+-rw-r--r--   0        0        0    10631 2023-12-19 01:27:51.212244 inspy_logger-3.1.0.dev1/inspy_logger/helpers/network.py
+-rw-r--r--   0        0        0     2175 2023-12-25 21:32:04.611127 inspy_logger-3.1.0.dev1/inspy_logger/helpers/units.py
+-rw-r--r--   0        0        0      992 2023-12-07 05:54:44.333226 inspy_logger-3.1.0.dev1/inspy_logger/manifest.py
+-rw-r--r--   0        0        0     2857 2024-03-25 23:00:48.439094 inspy_logger-3.1.0.dev1/inspy_logger/Scripts/main.py
+-rw-r--r--   0        0        0      681 2024-03-29 22:07:26.428504 inspy_logger-3.1.0.dev1/inspy_logger/system/__init__.py
+-rw-r--r--   0        0        0      424 2024-03-29 18:16:16.092498 inspy_logger-3.1.0.dev1/inspy_logger/system/linux.py
+-rw-r--r--   0        0        0      243 2024-03-29 18:16:16.078641 inspy_logger-3.1.0.dev1/inspy_logger/system/mac_os.py
+-rw-r--r--   0        0        0      960 2024-03-30 21:12:18.256135 inspy_logger-3.1.0.dev1/inspy_logger/system/win32.py
+-rw-r--r--   0        0        0        0 2024-01-04 00:54:16.535190 inspy_logger-3.1.0.dev1/inspy_logger/tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 00:55:12.726772 inspy_logger-3.1.0.dev1/inspy_logger/tool/config/__init__.py
+-rw-r--r--   0        0        0     2247 2024-01-06 00:31:51.966217 inspy_logger-3.1.0.dev1/inspy_logger/tool/config/arguments/__init__.py
+-rw-r--r--   0        0        0    14890 2024-04-04 02:33:21.088800 inspy_logger-3.1.0.dev1/inspy_logger/version/__init__.py
+-rw-r--r--   0        0        0       13 2024-04-03 20:20:50.768689 inspy_logger-3.1.0.dev1/inspy_logger/version/VERSION.txt
+-rw-r--r--   0        0        0      885 2023-12-07 05:54:44.295896 inspy_logger-3.1.0.dev1/LICENSE.md
+-rw-r--r--   0        0        0     2304 2024-04-03 21:16:42.776629 inspy_logger-3.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2500 2023-12-07 05:54:44.296909 inspy_logger-3.1.0.dev1/README.md
+-rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 inspy_logger-3.1.0.dev1/PKG-INFO
```

### Comparing `inspy_logger-3.0.dev5/inspy_logger/errors/__init__.py` & `inspy_logger-3.1.0.dev1/inspy_logger/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.0.dev5/inspy_logger/helpers/network.py` & `inspy_logger-3.1.0.dev1/inspy_logger/helpers/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 """
 from __future__ import annotations
 
 # Do our import
 from urllib.parse import quote as url_safe
 
 import requests
-
-from inspy_logger.helpers.cache import TLDCache
+from public_suffix_list import PublicSuffixList
 
 DEFAULT_TEST_HOSTS = [
         ['https', 'inspyre', 'tech'],
         ['https', 'google', 'com']
 ]
 """
 :obj:`list`[:obj:`list`[:obj:`str`]]:
@@ -40,18 +39,19 @@
 """
 
 hosts = []
 """
 :obj:`list`[:obj:`Host`]:
     A list of host objects that will be used to connect to.
 """
+psl = PublicSuffixList()
 
-TLD_CACHE = TLDCache()
+URL_SUFFIXES = psl._suffixes
 
-VALID_TLDS = TLD_CACHE.TLDs
+VALID_TLDS = URL_SUFFIXES
 
 
 class Host():
     def __init__(self, host: list):
 
         # Populate the .__incoming variable with the URL parts
         # provided by the 'host' parameter
@@ -165,15 +165,15 @@
             """
             return self.__tld
 
         @tld.setter
         def tld(self, new):
             if not isinstance(new, str):
                 raise TypeError(f"New value must be a string not {type(new)}")
-            if new not in TLD_CACHE.TLDs:
+            if new not in URL_SUFFIXES:
                 raise ValueError("TLD must be valid!")
 
             self.__tld = new
 
         @property
         def formatted(self):
             """
```

### Comparing `inspy_logger-3.0.dev5/inspy_logger/manifest.py` & `inspy_logger-3.1.0.dev1/inspy_logger/manifest.py`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.0.dev5/LICENSE.md` & `inspy_logger-3.1.0.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.0.dev5/pyproject.toml` & `inspy_logger-3.1.0.dev1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inspy-logger"
-version = "3.0-dev.5"
+version = "3.1.0-dev.1"
 description = "Colorable, scalable logger for CLI"
 authors = ["Taylor-Jayde Blackstone <tayjaybabee@gmail.com>"]
 homepage = 'https://github.com/Inspyre-Softworks/inSPy-Logger'
 repository = 'https://github.com/Inspyre-Softworks/inSPy-Logger'
 documentation = 'https://inspy-logger.readthedocs.io/en/latest/'
 readme = 'README.md'
 license = 'MIT'
@@ -25,29 +25,31 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: System :: Logging',
     'Topic :: Utilities',
     ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-colorlog = "^6.7"
+colorlog = "^6.8.2"
 setuptools-autover = "^1.0.2"
-luddite = "^1.0.1"
-packaging = "^21.0"
+luddite = "^1.0.4"
+packaging = "^24.0"
 appdirs = "^1.4.4"
 colorama = "^0.4.6"
 requests = "^2.28.1"
 humanize = "^4.4.0"
-python-box = "^6.1.0"
-rich = "^13.5.2"
+python-box = "^7.1.1"
+rich = "^13.7.0"
+pypattyrn = "^1.2"
+platformdirs = "^4.2.0"
 
 [tool.poetry.dev-dependencies]
 ptipython = "^1.0.1"
 asciinema = "^2.2.0"
-bpython = "^0.23"
+bpython = "^0.24"
 
 [tool.poetry.scripts]
 inspy-logger-tool = "inspy_logger.Scripts.main:main"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 sphinx-autodoc-typehints = "^1.25.2"
@@ -57,11 +59,19 @@
 autoclasstoc = "^1.6.0"
 sphinx-autodoc-annotation = "^1.0.post1"
 sphinxcontrib-autoprogram = "^0.1.8"
 
 
 [tool.poetry.group.dev.dependencies]
 poetry-plugin-export = "^1.6.0"
+sphinx-autodoc2 = {extras = ["cli"], version = "^0.5.0"}
+mkdocs-material = "^9.5.15"
+sphinx = "^7.2.6"
+sphinx-autobuild = "^2024.2.4"
+
+
+[tool.poetry.group.debug.dependencies]
+pyperclip = "^1.8.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `inspy_logger-3.0.dev5/README.md` & `inspy_logger-3.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `inspy_logger-3.0.dev5/PKG-INFO` & `inspy_logger-3.1.0.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspy-logger
-Version: 3.0.dev5
+Version: 3.1.0.dev1
 Summary: Colorable, scalable logger for CLI
 Home-page: https://github.com/Inspyre-Softworks/inSPy-Logger
 License: MIT
 Keywords: cli,color,logging,log,terminal,console,colorama,colorlog,rich
 Author: Taylor-Jayde Blackstone
 Author-email: tayjaybabee@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -22,21 +22,23 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: colorlog (>=6.7,<7.0)
+Requires-Dist: colorlog (>=6.8.2,<7.0.0)
 Requires-Dist: humanize (>=4.4.0,<5.0.0)
-Requires-Dist: luddite (>=1.0.1,<2.0.0)
-Requires-Dist: packaging (>=21.0,<22.0)
-Requires-Dist: python-box (>=6.1.0,<7.0.0)
+Requires-Dist: luddite (>=1.0.4,<2.0.0)
+Requires-Dist: packaging (>=24.0,<25.0)
+Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
+Requires-Dist: pypattyrn (>=1.2,<2.0)
+Requires-Dist: python-box (>=7.1.1,<8.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: rich (>=13.5.2,<14.0.0)
+Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: setuptools-autover (>=1.0.2,<2.0.0)
 Project-URL: Documentation, https://inspy-logger.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Inspyre-Softworks/inSPy-Logger
 Description-Content-Type: text/markdown
 
 # inSPy-Logger
 ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Inspyre-Softworks/inSPy-Logger/CI?label=CI&logo=github&logoColor=9cf&style=for-the-badge)
```

