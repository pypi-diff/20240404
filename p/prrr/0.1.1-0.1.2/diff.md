# Comparing `tmp/prrr-0.1.1.tar.gz` & `tmp/prrr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prrr-0.1.1.tar", max compression
+gzip compressed data, was "prrr-0.1.2.tar", max compression
```

## Comparing `prrr-0.1.1.tar` & `prrr-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3302 2024-04-03 22:18:15.591583 prrr-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-03 22:26:11.976855 prrr-0.1.1/prrr/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-03 22:40:19.220062 prrr-0.1.1/prrr/commands/__pycache__/init.cpython-312.pyc
--rw-r--r--   0        0        0     3726 2024-04-03 22:40:19.229550 prrr-0.1.1/prrr/commands/__pycache__/pr.cpython-312.pyc
--rw-r--r--   0        0        0     1918 2024-04-03 22:26:11.977057 prrr-0.1.1/prrr/commands/init.py
--rw-r--r--   0        0        0     2899 2024-04-03 22:26:11.977404 prrr-0.1.1/prrr/commands/pr.py
--rw-r--r--   0        0        0      397 2024-04-03 22:26:11.977618 prrr-0.1.1/prrr/main.py
--rw-r--r--   0        0        0     1547 2024-04-03 22:40:19.439471 prrr-0.1.1/prrr/utils/__pycache__/git.cpython-312.pyc
--rw-r--r--   0        0        0      172 2024-04-03 22:26:11.977740 prrr-0.1.1/prrr/utils/config_reader.py
--rw-r--r--   0        0        0      756 2024-04-03 22:26:11.977861 prrr-0.1.1/prrr/utils/git.py
--rw-r--r--   0        0        0      469 2024-04-03 22:41:50.304330 prrr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3908 1970-01-01 00:00:00.000000 prrr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3302 2024-04-03 22:18:15.591583 prrr-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 22:26:11.976855 prrr-0.1.2/prrr/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-03 22:40:19.220062 prrr-0.1.2/prrr/commands/__pycache__/init.cpython-312.pyc
+-rw-r--r--   0        0        0     3726 2024-04-03 22:40:19.229550 prrr-0.1.2/prrr/commands/__pycache__/pr.cpython-312.pyc
+-rw-r--r--   0        0        0     1918 2024-04-03 22:26:11.977057 prrr-0.1.2/prrr/commands/init.py
+-rw-r--r--   0        0        0     2899 2024-04-03 22:26:11.977404 prrr-0.1.2/prrr/commands/pr.py
+-rw-r--r--   0        0        0      397 2024-04-03 22:26:11.977618 prrr-0.1.2/prrr/main.py
+-rw-r--r--   0        0        0     1547 2024-04-03 22:40:19.439471 prrr-0.1.2/prrr/utils/__pycache__/git.cpython-312.pyc
+-rw-r--r--   0        0        0      172 2024-04-03 22:26:11.977740 prrr-0.1.2/prrr/utils/config_reader.py
+-rw-r--r--   0        0        0      756 2024-04-03 22:26:11.977861 prrr-0.1.2/prrr/utils/git.py
+-rw-r--r--   0        0        0      575 2024-04-03 22:49:02.780640 prrr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 prrr-0.1.2/PKG-INFO
```

### Comparing `prrr-0.1.1/README.md` & `prrr-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `prrr-0.1.1/prrr/commands/__pycache__/init.cpython-312.pyc` & `prrr-0.1.2/prrr/commands/__pycache__/init.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prrr-0.1.1/prrr/commands/__pycache__/pr.cpython-312.pyc` & `prrr-0.1.2/prrr/commands/__pycache__/pr.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prrr-0.1.1/prrr/commands/init.py` & `prrr-0.1.2/prrr/commands/init.py`

 * *Files identical despite different names*

### Comparing `prrr-0.1.1/prrr/commands/pr.py` & `prrr-0.1.2/prrr/commands/pr.py`

 * *Files identical despite different names*

### Comparing `prrr-0.1.1/prrr/utils/__pycache__/git.cpython-312.pyc` & `prrr-0.1.2/prrr/utils/__pycache__/git.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `prrr-0.1.1/prrr/utils/git.py` & `prrr-0.1.2/prrr/utils/git.py`

 * *Files identical despite different names*

### Comparing `prrr-0.1.1/PKG-INFO` & `prrr-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: prrr
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple CLI tool to help you write better PRs.
+Home-page: https://github.com/oscarnevarezleal/prr
 Author: Oscar Nevarez
 Author-email: fu.wire@gmail.com
 Requires-Python: >=3.9.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gitpython (>=3.1.24,<4.0.0)
+Requires-Dist: openai (==1.16.1)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: typer-config[yaml] (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # prr
```

