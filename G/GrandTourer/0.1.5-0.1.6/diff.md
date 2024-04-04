# Comparing `tmp/grandtourer-0.1.5.tar.gz` & `tmp/grandtourer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grandtourer-0.1.5.tar", max compression
+gzip compressed data, was "grandtourer-0.1.6.tar", max compression
```

## Comparing `grandtourer-0.1.5.tar` & `grandtourer-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1344 2023-12-25 22:34:22.986681 grandtourer-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-12-01 11:17:30.754755 grandtourer-0.1.5/grandtourer/__init__.py
--rw-r--r--   0        0        0     2834 2024-03-06 22:46:17.830601 grandtourer-0.1.5/grandtourer/cli.py
--rw-r--r--   0        0        0      533 2024-03-06 22:46:35.116714 grandtourer-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 grandtourer-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1348 2024-04-04 18:28:20.058367 grandtourer-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-12-01 11:17:30.754755 grandtourer-0.1.6/grandtourer/__init__.py
+-rw-r--r--   0        0        0     2817 2024-04-04 18:28:23.770367 grandtourer-0.1.6/grandtourer/cli.py
+-rw-r--r--   0        0        0      517 2024-04-04 18:28:22.179761 grandtourer-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2119 1970-01-01 00:00:00.000000 grandtourer-0.1.6/PKG-INFO
```

### Comparing `grandtourer-0.1.5/README.md` & `grandtourer-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # GrandTourer
 
-GrandTourer is a CLI tool for easily launching applications on MacOS with a two letter command: `gt`. It's a drop-in replacement for `open -a`, but without the need for precise capitalisation, spacing, and first words like "Microsoft" or "Adobe" if you have multiple applications from them.
+GrandTourer is a CLI tool for easily launching GUI applications on MacOS with a two letter command: `gt`. It's a drop-in replacement for `open -a`, but without the need for precise capitalisation, spacing, and first words like "Microsoft" or "Adobe" if you have multiple applications from them.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GrandTourer. GrandTourer requires Python >=3.8.
 
 ```shell
 $ pip install grandtourer
```

### Comparing `grandtourer-0.1.5/grandtourer/cli.py` & `grandtourer-0.1.6/grandtourer/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pythonads
 import click
 import os
 import subprocess
 
 def get_applications_dict():
 
     applications_dict = {}
```

### Comparing `grandtourer-0.1.5/pyproject.toml` & `grandtourer-0.1.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "GrandTourer"
-version = "0.1.5"
-description = "GrandTourer is a CLI tool for easily launching applications on MacOS with a two letter command: gt"
+version = "0.1.6"
+description = "GrandTourer is a CLI tool for easily launching GUI applications on MacOS with a two letter command: gt"
 authors = ["WillDenby <119456795+WillDenby@users.noreply.github.com>"]
-readme = "README.md"
+readme = "README.md" 
 repository = "https://github.com/WillDenby/GrandTourer"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.7"
-pythonads = "^0.1.0"
 
 [tool.poetry.scripts]
 gt = "grandtourer.cli:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grandtourer-0.1.5/PKG-INFO` & `grandtourer-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: GrandTourer
-Version: 0.1.5
-Summary: GrandTourer is a CLI tool for easily launching applications on MacOS with a two letter command: gt
+Version: 0.1.6
+Summary: GrandTourer is a CLI tool for easily launching GUI applications on MacOS with a two letter command: gt
 Home-page: https://github.com/WillDenby/GrandTourer
 Author: WillDenby
 Author-email: 119456795+WillDenby@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: pythonads (>=0.1.0,<0.2.0)
 Project-URL: Repository, https://github.com/WillDenby/GrandTourer
 Description-Content-Type: text/markdown
 
 # GrandTourer
 
-GrandTourer is a CLI tool for easily launching applications on MacOS with a two letter command: `gt`. It's a drop-in replacement for `open -a`, but without the need for precise capitalisation, spacing, and first words like "Microsoft" or "Adobe" if you have multiple applications from them.
+GrandTourer is a CLI tool for easily launching GUI applications on MacOS with a two letter command: `gt`. It's a drop-in replacement for `open -a`, but without the need for precise capitalisation, spacing, and first words like "Microsoft" or "Adobe" if you have multiple applications from them.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GrandTourer. GrandTourer requires Python >=3.8.
 
 ```shell
 $ pip install grandtourer
```

