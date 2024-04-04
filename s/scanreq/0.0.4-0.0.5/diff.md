# Comparing `tmp/scanreq-0.0.4.tar.gz` & `tmp/scanreq-0.0.5.tar.gz`

## Comparing `scanreq-0.0.4.tar` & `scanreq-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.4/requirements-dev.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.4/requirements.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.4/setup.cfg
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.4/src/scanreq/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.4/src/scanreq/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 scanreq-0.0.4/src/scanreq/cli.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 scanreq-0.0.4/src/scanreq/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 scanreq-0.0.4/tests/test_scanner.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.4/LICENSE
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 scanreq-0.0.4/README.md
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 scanreq-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 scanreq-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.5/requirements-dev.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.5/setup.cfg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.5/src/scanreq/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.5/src/scanreq/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 scanreq-0.0.5/src/scanreq/__main__.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 scanreq-0.0.5/src/scanreq/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 scanreq-0.0.5/tests/test_scanner.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 scanreq-0.0.5/README.md
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 scanreq-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 scanreq-0.0.5/PKG-INFO
```

### Comparing `scanreq-0.0.4/.pre-commit-config.yaml` & `scanreq-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.4/src/scanreq/cli.py` & `scanreq-0.0.5/src/scanreq/__main__.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.4/src/scanreq/scanner.py` & `scanreq-0.0.5/src/scanreq/scanner.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.4/tests/test_scanner.py` & `scanreq-0.0.5/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.4/.gitignore` & `scanreq-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.4/LICENSE` & `scanreq-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.4/README.md` & `scanreq-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,31 +21,39 @@
 6. **Update Efficiently**: Ensure your dependencies are up-to-date for smoother compatibility.
 7. **Stay Safe**: Reduce the chance of security vulnerabilities by trimming unnecessary dependencies.
 8. **Stay Legal**: Avoid licensing issues by managing dependencies more effectively.
 9. **Work Together**: Simplify collaboration with a consistent set of dependencies.
 10. **Code Better**: Keep your documentation and codebase cleaner for improved quality.
 
 
+## Installation
+
+
+```console
+pip3 install scanreq
+```
+
+
 ## Usage
 
-```bash
-(env-myproject) ➜  myproject git:(development) ✗ python scan.py -r requirements.txt -p .
+```console
+(env-myproject) ➜  myproject git:(development) ✗ scanreq -r requirements.txt -p .
 
 [i] Please wait! It may take few minutes to complete...
 [i] Scanning unused packages:
  1. Module: rcssmin ---> Package: rcssmin
  2. Module: model_utils ---> Package: django-model-utils
  3. Module: pinax_theme_bootstrap ---> Package: pinax-theme-bootstrap
  4. Module: phonenumbers ---> Package: phonenumbers
 ```
 
 Cool right? 😎
 
-```bash
-(env-myproject) ➜  scan-unused-requirements git:(master) ✗ python scan.py --help
+```console
+(env-myproject) ➜  myproject git:(development) ✗ scanreq --help
 usage: scan.py [-h] [-r REQUIREMENTS] [-p PATH]
 
 Scan for unused Python packages.
 
 optional arguments:
   -h, --help            show this help message and exit
   -r REQUIREMENTS, --requirements REQUIREMENTS
@@ -67,7 +75,8 @@
    - [ ] Option to exclude or ignore some packages
 - [ ] Support multiple python versions
 - [ ] Support CLI - make it as a command
 - [ ] Support multiple devices (Linux, Macbook, and Windows)
 - [ ] Write some tests
 - [ ] Publish to PyPi
 - [ ] Support scan the `pyproject.toml`
+s
```

### Comparing `scanreq-0.0.4/pyproject.toml` & `scanreq-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,29 +22,28 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["importlib_metadata>=7.1.0"]
+scripts.scanreq = "scanreq.__main__:main"
 
 [project.urls]
 Changelog = "https://github.com/agusmakmun/scan-unused-requirements/releases"
 Documentation = "https://github.com/agusmakmun/scanreq"
 Issues = "https://github.com/agusmakmun/scanreq/issues"
 Source = "https://github.com/agusmakmun/scanreq"
 
 [tool.hatch.version]
 path = "src/scanreq/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = ["coverage[toml]>=6.5", "pytest"]
-
 [tool.hatch.envs.default.scripts]
-scanreq = "scanreq.cli:main"
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
```

### Comparing `scanreq-0.0.4/PKG-INFO` & `scanreq-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scanreq
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python tool to scan all unused packages in requirements.txt file for your project.
 Project-URL: Changelog, https://github.com/agusmakmun/scan-unused-requirements/releases
 Project-URL: Documentation, https://github.com/agusmakmun/scanreq
 Project-URL: Issues, https://github.com/agusmakmun/scanreq/issues
 Project-URL: Source, https://github.com/agusmakmun/scanreq
 Author-email: agusmakmun <summon.agus@gmail.com>
 License-Expression: MIT
@@ -49,31 +49,39 @@
 6. **Update Efficiently**: Ensure your dependencies are up-to-date for smoother compatibility.
 7. **Stay Safe**: Reduce the chance of security vulnerabilities by trimming unnecessary dependencies.
 8. **Stay Legal**: Avoid licensing issues by managing dependencies more effectively.
 9. **Work Together**: Simplify collaboration with a consistent set of dependencies.
 10. **Code Better**: Keep your documentation and codebase cleaner for improved quality.
 
 
+## Installation
+
+
+```console
+pip3 install scanreq
+```
+
+
 ## Usage
 
-```bash
-(env-myproject) ➜  myproject git:(development) ✗ python scan.py -r requirements.txt -p .
+```console
+(env-myproject) ➜  myproject git:(development) ✗ scanreq -r requirements.txt -p .
 
 [i] Please wait! It may take few minutes to complete...
 [i] Scanning unused packages:
  1. Module: rcssmin ---> Package: rcssmin
  2. Module: model_utils ---> Package: django-model-utils
  3. Module: pinax_theme_bootstrap ---> Package: pinax-theme-bootstrap
  4. Module: phonenumbers ---> Package: phonenumbers
 ```
 
 Cool right? 😎
 
-```bash
-(env-myproject) ➜  scan-unused-requirements git:(master) ✗ python scan.py --help
+```console
+(env-myproject) ➜  myproject git:(development) ✗ scanreq --help
 usage: scan.py [-h] [-r REQUIREMENTS] [-p PATH]
 
 Scan for unused Python packages.
 
 optional arguments:
   -h, --help            show this help message and exit
   -r REQUIREMENTS, --requirements REQUIREMENTS
@@ -95,7 +103,8 @@
    - [ ] Option to exclude or ignore some packages
 - [ ] Support multiple python versions
 - [ ] Support CLI - make it as a command
 - [ ] Support multiple devices (Linux, Macbook, and Windows)
 - [ ] Write some tests
 - [ ] Publish to PyPi
 - [ ] Support scan the `pyproject.toml`
+s
```

