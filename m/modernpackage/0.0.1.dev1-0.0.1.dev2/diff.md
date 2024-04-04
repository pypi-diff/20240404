# Comparing `tmp/modernpackage-0.0.1.dev1.tar.gz` & `tmp/modernpackage-0.0.1.dev2.tar.gz`

## Comparing `modernpackage-0.0.1.dev1.tar` & `modernpackage-0.0.1.dev2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev1/src/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev1/src/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev1/README.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev2/modernpackage/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev2/modernpackage/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev2/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 modernpackage-0.0.1.dev2/PKG-INFO
```

### Comparing `modernpackage-0.0.1.dev1/.gitignore` & `modernpackage-0.0.1.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `modernpackage-0.0.1.dev1/README.md` & `modernpackage-0.0.1.dev2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# package
+# modernpackage
 This package is configured using bleeding edge toolset and serves as an
 example/starting point for another new packages.
 
 ## Development
 Commonly used commands for package development:
 `make check` - run unit tests and linters.
 `make fix` - format code and fix detected fixable issues.
```

### Comparing `modernpackage-0.0.1.dev1/pyproject.toml` & `modernpackage-0.0.1.dev2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "modernpackage"
-version = "0.0.1.dev1"
+version = "0.0.1.dev2"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
 description = "Example package configuration using bleeding edge toolset"
 readme = "README.md"
 requires-python = ">= 3.11"
 classifiers = [
@@ -56,15 +56,15 @@
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "D203",  # one-blank-line-before-class
     "D213",  # multi-line-summary-second-line
     "COM812",  # missing-trailing-comma
     "ISC001",  # single-line-implicit-string-concatenation
-    "ANN101",  # deprecated self annotation
+    "ANN101",  # deprecated requirement to annotate self
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101", "D"]  # allow asserts and no docs in tests
 
 [tool.mypy]
 exclude = ["build", "dist", ".venv", "tests"]
```

### Comparing `modernpackage-0.0.1.dev1/PKG-INFO` & `modernpackage-0.0.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: modernpackage
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Example package configuration using bleeding edge toolset
 Project-URL: homepage, https://github.com/albertas/modernpackage
 Author-email: Albertas Gimbutas <albertasgim@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: pip-audit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
 
-# package
+# modernpackage
 This package is configured using bleeding edge toolset and serves as an
 example/starting point for another new packages.
 
 ## Development
 Commonly used commands for package development:
 `make check` - run unit tests and linters.
 `make fix` - format code and fix detected fixable issues.
```

