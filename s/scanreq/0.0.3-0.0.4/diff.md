# Comparing `tmp/scanreq-0.0.3.tar.gz` & `tmp/scanreq-0.0.4.tar.gz`

## Comparing `scanreq-0.0.3.tar` & `scanreq-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.3/requirements-dev.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.3/requirements.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.3/setup.cfg
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.3/src/scanreq/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.3/src/scanreq/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 scanreq-0.0.3/src/scanreq/cli.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 scanreq-0.0.3/src/scanreq/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 scanreq-0.0.3/tests/test_scanner.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.3/LICENSE
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scanreq-0.0.3/README.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 scanreq-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 scanreq-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.4/requirements-dev.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.4/setup.cfg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.4/src/scanreq/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.4/src/scanreq/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 scanreq-0.0.4/src/scanreq/cli.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 scanreq-0.0.4/src/scanreq/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 scanreq-0.0.4/tests/test_scanner.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scanreq-0.0.4/README.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 scanreq-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 scanreq-0.0.4/PKG-INFO
```

### Comparing `scanreq-0.0.3/.pre-commit-config.yaml` & `scanreq-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.3/src/scanreq/cli.py` & `scanreq-0.0.4/src/scanreq/cli.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.3/src/scanreq/scanner.py` & `scanreq-0.0.4/src/scanreq/scanner.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.3/tests/test_scanner.py` & `scanreq-0.0.4/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.3/.gitignore` & `scanreq-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.3/LICENSE` & `scanreq-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.3/README.md` & `scanreq-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.3/pyproject.toml` & `scanreq-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,29 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["importlib_metadata>=7.1.0"]
-scripts.pipdeptree = "scanreq.cli:main"
 
 [project.urls]
 Changelog = "https://github.com/agusmakmun/scan-unused-requirements/releases"
 Documentation = "https://github.com/agusmakmun/scanreq"
 Issues = "https://github.com/agusmakmun/scanreq/issues"
 Source = "https://github.com/agusmakmun/scanreq"
 
 [tool.hatch.version]
 path = "src/scanreq/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = ["coverage[toml]>=6.5", "pytest"]
+
 [tool.hatch.envs.default.scripts]
+scanreq = "scanreq.cli:main"
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
```

### Comparing `scanreq-0.0.3/PKG-INFO` & `scanreq-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scanreq
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python tool to scan all unused packages in requirements.txt file for your project.
 Project-URL: Changelog, https://github.com/agusmakmun/scan-unused-requirements/releases
 Project-URL: Documentation, https://github.com/agusmakmun/scanreq
 Project-URL: Issues, https://github.com/agusmakmun/scanreq/issues
 Project-URL: Source, https://github.com/agusmakmun/scanreq
 Author-email: agusmakmun <summon.agus@gmail.com>
 License-Expression: MIT
```

