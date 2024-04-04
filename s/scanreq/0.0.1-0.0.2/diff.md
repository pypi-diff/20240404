# Comparing `tmp/scanreq-0.0.1.tar.gz` & `tmp/scanreq-0.0.2.tar.gz`

## Comparing `scanreq-0.0.1.tar` & `scanreq-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.1/requirements.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.1/setup.cfg
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.1/src/scanreq/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.1/src/scanreq/__init__.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 scanreq-0.0.1/src/scanreq/__main__.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 scanreq-0.0.1/src/scanreq/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 scanreq-0.0.1/tests/test_scanner.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.1/LICENSE
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scanreq-0.0.1/README.md
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 scanreq-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 scanreq-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.2/setup.cfg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.2/src/scanreq/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.2/src/scanreq/__init__.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 scanreq-0.0.2/src/scanreq/cli.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 scanreq-0.0.2/src/scanreq/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 scanreq-0.0.2/tests/test_scanner.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scanreq-0.0.2/README.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 scanreq-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 scanreq-0.0.2/PKG-INFO
```

### Comparing `scanreq-0.0.1/.pre-commit-config.yaml` & `scanreq-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.1/src/scanreq/__main__.py` & `scanreq-0.0.2/src/scanreq/cli.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.1/src/scanreq/scanner.py` & `scanreq-0.0.2/src/scanreq/scanner.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.1/tests/test_scanner.py` & `scanreq-0.0.2/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.1/.gitignore` & `scanreq-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.1/LICENSE` & `scanreq-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.1/README.md` & `scanreq-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.1/pyproject.toml` & `scanreq-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["importlib_metadata>=7.1.0"]
-scripts.pipdeptree = "scanreq.__main__:main"
+scripts.pipdeptree = "scanreq.cli:main"
 
 [project.urls]
 Changelog = "https://github.com/agusmakmun/scan-unused-requirements/releases"
 Documentation = "https://github.com/agusmakmun/scanreq"
 Issues = "https://github.com/agusmakmun/scanreq/issues"
 Source = "https://github.com/agusmakmun/scanreq"
```

### Comparing `scanreq-0.0.1/PKG-INFO` & `scanreq-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scanreq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python tool to scan all unused packages in requirements.txt file for your project.
 Project-URL: Changelog, https://github.com/agusmakmun/scan-unused-requirements/releases
 Project-URL: Documentation, https://github.com/agusmakmun/scanreq
 Project-URL: Issues, https://github.com/agusmakmun/scanreq/issues
 Project-URL: Source, https://github.com/agusmakmun/scanreq
 Author-email: agusmakmun <summon.agus@gmail.com>
 License-Expression: MIT
```

