# Comparing `tmp/opda-0.6.0.tar.gz` & `tmp/opda-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opda-0.6.0.tar", last modified: Mon Mar  4 04:57:30 2024, max compression
+gzip compressed data, was "opda-0.6.1.tar", last modified: Thu Apr  4 02:30:31 2024, max compression
```

## Comparing `opda-0.6.0.tar` & `opda-0.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 04:57:30.607820 opda-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-03-04 04:56:56.000000 opda-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-03-04 04:57:30.607820 opda-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-03-04 04:56:56.000000 opda-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-04 04:57:26.000000 opda-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 04:57:30.607820 opda-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 04:57:30.603820 opda-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 04:57:30.603820 opda-0.6.0/src/opda/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 04:56:56.000000 opda-0.6.0/src/opda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-03-04 04:56:56.000000 opda-0.6.0/src/opda/_approximations.json
--rw-r--r--   0 runner    (1001) docker     (127)    31483 2024-03-04 04:56:56.000000 opda-0.6.0/src/opda/approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-04 04:56:56.000000 opda-0.6.0/src/opda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    32350 2024-03-04 04:56:56.000000 opda-0.6.0/src/opda/nonparametric.py
--rw-r--r--   0 runner    (1001) docker     (127)    51508 2024-03-04 04:56:56.000000 opda-0.6.0/src/opda/parametric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-04 04:56:56.000000 opda-0.6.0/src/opda/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    19308 2024-03-04 04:56:56.000000 opda-0.6.0/src/opda/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 04:57:30.607820 opda-0.6.0/src/opda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-04 04:57:30.000000 opda-0.6.0/src/opda.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 04:57:30.603820 opda-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-04 04:56:56.000000 opda-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 04:57:30.607820 opda-0.6.0/tests/opda/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-04 04:56:56.000000 opda-0.6.0/tests/opda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27012 2024-03-04 04:56:56.000000 opda-0.6.0/tests/opda/test_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-04 04:56:56.000000 opda-0.6.0/tests/opda/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)   135204 2024-03-04 04:56:56.000000 opda-0.6.0/tests/opda/test_nonparametric.py
--rw-r--r--   0 runner    (1001) docker     (127)   123259 2024-03-04 04:56:56.000000 opda-0.6.0/tests/opda/test_parametric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-04 04:56:56.000000 opda-0.6.0/tests/opda/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    49187 2024-03-04 04:56:56.000000 opda-0.6.0/tests/opda/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-04 04:56:56.000000 opda-0.6.0/tests/testcases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:30:31.940542 opda-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-04 02:29:54.000000 opda-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-04 02:30:31.940542 opda-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-04 02:29:54.000000 opda-0.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-04 02:30:27.000000 opda-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 02:30:31.940542 opda-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:30:31.936542 opda-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:30:31.936542 opda-0.6.1/src/opda/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 02:29:54.000000 opda-0.6.1/src/opda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-04-04 02:29:54.000000 opda-0.6.1/src/opda/_approximations.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31483 2024-04-04 02:29:54.000000 opda-0.6.1/src/opda/approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-04 02:29:54.000000 opda-0.6.1/src/opda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32350 2024-04-04 02:29:54.000000 opda-0.6.1/src/opda/nonparametric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51508 2024-04-04 02:29:54.000000 opda-0.6.1/src/opda/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-04 02:29:54.000000 opda-0.6.1/src/opda/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19308 2024-04-04 02:29:54.000000 opda-0.6.1/src/opda/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:30:31.936542 opda-0.6.1/src/opda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 02:30:31.000000 opda-0.6.1/src/opda.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:30:31.936542 opda-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 02:29:54.000000 opda-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:30:31.936542 opda-0.6.1/tests/opda/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 02:29:54.000000 opda-0.6.1/tests/opda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27012 2024-04-04 02:29:54.000000 opda-0.6.1/tests/opda/test_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 02:29:54.000000 opda-0.6.1/tests/opda/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135204 2024-04-04 02:29:54.000000 opda-0.6.1/tests/opda/test_nonparametric.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123259 2024-04-04 02:29:54.000000 opda-0.6.1/tests/opda/test_parametric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-04 02:29:54.000000 opda-0.6.1/tests/opda/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49187 2024-04-04 02:29:54.000000 opda-0.6.1/tests/opda/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-04 02:29:54.000000 opda-0.6.1/tests/testcases.py
```

### Comparing `opda-0.6.0/LICENSE` & `opda-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/PKG-INFO` & `opda-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opda
-Version: 0.6.0
+Version: 0.6.1
 Summary: Design and analyze optimal deep learning models.
 Author-email: Nicholas Lourie <dev@nicholaslourie.com>
 License: Apache-2.0
 Project-URL: Documentation, https://nicholaslourie.github.io/opda
 Project-URL: Source, https://github.com/nicholaslourie/opda
 Project-URL: Issues, https://github.com/nicholaslourie/opda/issues
 Project-URL: Changelog, https://nicholaslourie.github.io/opda/changelog.html
@@ -40,16 +40,17 @@
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest==7.4.4; extra == "test"
 Provides-Extra: package
 Requires-Dist: build==1.0.3; extra == "package"
 Requires-Dist: twine==4.0.2; extra == "package"
 Provides-Extra: ci
-Requires-Dist: nox==2023.4.22; extra == "ci"
 Requires-Dist: lxml==5.1.0; extra == "ci"
+Requires-Dist: nox==2023.4.22; extra == "ci"
+Requires-Dist: requests==2.31.0; extra == "ci"
 Requires-Dist: tomli; python_version < "3.11" and extra == "ci"
 
 =============================
 opda: optimal design analysis
 =============================
 `Docs <https://nicholaslourie.github.io/opda>`_
 | `Source <https://github.com/nicholaslourie/opda>`_
```

### Comparing `opda-0.6.0/README.rst` & `opda-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/pyproject.toml` & `opda-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "opda"
-version = "0.6.0"
+version = "0.6.1"
 authors = [{ name = "Nicholas Lourie", email = "dev@nicholaslourie.com" }]
 description = "Design and analyze optimal deep learning models."
 readme = "README.rst"
 license = {text = "Apache-2.0"}
 requires-python = ">= 3.8"
 dependencies = [
   "numpy >= 1.21",
@@ -60,16 +60,17 @@
   "pytest == 7.4.4",
 ]
 package = [
   "build == 1.0.3",
   "twine == 4.0.2",
 ]
 ci = [
-  "nox == 2023.4.22",
   "lxml == 5.1.0",
+  "nox == 2023.4.22",
+  "requests == 2.31.0",
   "tomli; python_version<'3.11'",  # backwards compatibility (Python < 3.11)
 ]
 
 [project.urls]
 Documentation = "https://nicholaslourie.github.io/opda"
 Source = "https://github.com/nicholaslourie/opda"
 Issues = "https://github.com/nicholaslourie/opda/issues"
```

### Comparing `opda-0.6.0/src/opda/_approximations.json` & `opda-0.6.1/src/opda/_approximations.json`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/src/opda/approximation.py` & `opda-0.6.1/src/opda/approximation.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/src/opda/nonparametric.py` & `opda-0.6.1/src/opda/nonparametric.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/src/opda/parametric.py` & `opda-0.6.1/src/opda/parametric.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/src/opda/random.py` & `opda-0.6.1/src/opda/random.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/src/opda/utils.py` & `opda-0.6.1/src/opda/utils.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/tests/opda/test_approximation.py` & `opda-0.6.1/tests/opda/test_approximation.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/tests/opda/test_nonparametric.py` & `opda-0.6.1/tests/opda/test_nonparametric.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/tests/opda/test_parametric.py` & `opda-0.6.1/tests/opda/test_parametric.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/tests/opda/test_random.py` & `opda-0.6.1/tests/opda/test_random.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/tests/opda/test_utils.py` & `opda-0.6.1/tests/opda/test_utils.py`

 * *Files identical despite different names*

### Comparing `opda-0.6.0/tests/testcases.py` & `opda-0.6.1/tests/testcases.py`

 * *Files identical despite different names*

