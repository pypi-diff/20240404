# Comparing `tmp/pytest-elk-reporter-0.2.1.tar.gz` & `tmp/pytest-elk-reporter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-elk-reporter-0.2.1.tar", last modified: Wed Jan 20 11:45:35 2021, max compression
+gzip compressed data, was "dist/pytest-elk-reporter-0.2.2.tar", last modified: Sun Jan 24 22:21:53 2021, max compression
```

## Comparing `pytest-elk-reporter-0.2.1.tar` & `pytest-elk-reporter-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-20 11:45:35.469400 pytest-elk-reporter-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-20 11:45:35.465400 pytest-elk-reporter-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-20 11:45:35.469400 pytest-elk-reporter-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1905 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (116)      928 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      751 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1083 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     9918 2021-01-20 11:45:35.469400 pytest-elk-reporter-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7107 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       86 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-20 11:45:35.469400 pytest-elk-reporter-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     7107 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      224 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)    17593 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      156 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       62 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-20 11:45:35.469400 pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9918 2021-01-20 11:45:35.000000 pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      570 2021-01-20 11:45:35.000000 pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-20 11:45:35.000000 pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2021-01-20 11:45:35.000000 pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       27 2021-01-20 11:45:35.000000 pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2021-01-20 11:45:35.000000 pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    18372 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/pytest_elk_reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)       92 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)       67 2021-01-20 11:45:35.469400 pytest-elk-reporter-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-20 11:45:35.469400 pytest-elk-reporter-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1535 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)    14123 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/tests/test_elk_reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1926 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (116)      584 2021-01-20 11:45:33.000000 pytest-elk-reporter-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-24 22:21:53.303294 pytest-elk-reporter-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-24 22:21:53.299294 pytest-elk-reporter-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-24 22:21:53.303294 pytest-elk-reporter-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1905 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      928 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      751 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1083 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     9918 2021-01-24 22:21:53.303294 pytest-elk-reporter-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     7107 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       86 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-24 22:21:53.303294 pytest-elk-reporter-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     7107 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      224 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)    17593 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (116)      156 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       62 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-24 22:21:53.303294 pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     9918 2021-01-24 22:21:53.000000 pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      590 2021-01-24 22:21:53.000000 pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-24 22:21:53.000000 pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2021-01-24 22:21:53.000000 pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       27 2021-01-24 22:21:53.000000 pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       20 2021-01-24 22:21:53.000000 pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    18426 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/pytest_elk_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)       92 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2021-01-24 22:21:53.303294 pytest-elk-reporter-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1747 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-24 22:21:53.303294 pytest-elk-reporter-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     1535 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13524 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/tests/test_elk_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1926 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1237 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/tests/test_xdist.py
+-rw-r--r--   0 runner    (1001) docker     (116)      584 2021-01-24 22:21:48.000000 pytest-elk-reporter-0.2.2/tox.ini
```

### Comparing `pytest-elk-reporter-0.2.1/.github/workflows/tests.yml` & `pytest-elk-reporter-0.2.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/.gitignore` & `pytest-elk-reporter-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/.pre-commit-config.yaml` & `pytest-elk-reporter-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/LICENSE` & `pytest-elk-reporter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/PKG-INFO` & `pytest-elk-reporter-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-elk-reporter
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple plugin to use with pytest
 Home-page: https://github.com/fruch/pytest-elk-reporter
 Author: Israel Fruchter
 Author-email: israel.fruchter@gmail.com
 Maintainer: Israel Fruchter
 Maintainer-email: israel.fruchter@gmail.com
 License: MIT
```

### Comparing `pytest-elk-reporter-0.2.1/README.md` & `pytest-elk-reporter-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/docs/README.md` & `pytest-elk-reporter-0.2.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/pylintrc` & `pytest-elk-reporter-0.2.2/pylintrc`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/PKG-INFO` & `pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-elk-reporter
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple plugin to use with pytest
 Home-page: https://github.com/fruch/pytest-elk-reporter
 Author: Israel Fruchter
 Author-email: israel.fruchter@gmail.com
 Maintainer: Israel Fruchter
 Maintainer-email: israel.fruchter@gmail.com
 License: MIT
```

### Comparing `pytest-elk-reporter-0.2.1/pytest_elk_reporter.egg-info/SOURCES.txt` & `pytest-elk-reporter-0.2.2/pytest_elk_reporter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 pytest_elk_reporter.egg-info/SOURCES.txt
 pytest_elk_reporter.egg-info/dependency_links.txt
 pytest_elk_reporter.egg-info/entry_points.txt
 pytest_elk_reporter.egg-info/requires.txt
 pytest_elk_reporter.egg-info/top_level.txt
 tests/conftest.py
 tests/test_elk_reporter.py
-tests/test_slices.py
+tests/test_slices.py
+tests/test_xdist.py
```

### Comparing `pytest-elk-reporter-0.2.1/pytest_elk_reporter.py` & `pytest-elk-reporter-0.2.2/pytest_elk_reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,18 @@
 
     def get_worker_id(self):
         # based on https://github.com/pytest-dev/pytest-xdist/pull/505
         # (to support older version of xdist)
         worker_id = "default"
         if hasattr(self.config, "workerinput"):
             worker_id = self.config.workerinput["workerid"]
-        if not hasattr(self.config, "workerinput") and self.config.option.dist != "no":
+        if (
+            not hasattr(self.config, "workerinput")
+            and getattr(self.config.option, "dist", "no") != "no"
+        ):
             worker_id = "master"
         return worker_id
 
     def pytest_runtest_logreport(self, report):
         # pylint: disable=too-many-branches
 
         if report.passed:
```

### Comparing `pytest-elk-reporter-0.2.1/setup.py` & `pytest-elk-reporter-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/tests/conftest.py` & `pytest-elk-reporter-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/tests/test_elk_reporter.py` & `pytest-elk-reporter-0.2.2/tests/test_elk_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,36 +389,14 @@
     first_report = json.loads(requests_mock.request_history[0].text)
     assert "mark1" in first_report["markers"]
 
     second_report = json.loads(requests_mock.request_history[1].text)
     assert "mark2" in second_report["markers"]
 
 
-def test_xdist(testdir):  # pylint: disable=redefined-outer-name
-    # create a temporary pytest test module
-    testdir.makepyfile(
-        """
-        import pytest
-        @pytest.mark.mark1
-        def test_1(request):
-            pass
-
-        @pytest.mark.mark2
-        def test_2():
-            pass
-        """
-    )
-
-    result = testdir.runpytest("--es-address=127.0.0.1:9200", "-s", "-v", "-n", "2")
-
-    # fnmatch_lines does an assertion internally
-    result.stdout.fnmatch_lines(["*PASSED*test_xdist.py::test_1 "])
-    result.stdout.fnmatch_lines(["*PASSED*test_xdist.py::test_2 "])
-
-
 def test_user_properties(
     testdir, requests_mock
 ):  # pylint: disable=redefined-outer-name
     # create a temporary pytest test module
     testdir.makepyfile(
         """
         import pytest
```

### Comparing `pytest-elk-reporter-0.2.1/tests/test_slices.py` & `pytest-elk-reporter-0.2.2/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `pytest-elk-reporter-0.2.1/tox.ini` & `pytest-elk-reporter-0.2.2/tox.ini`

 * *Files identical despite different names*

