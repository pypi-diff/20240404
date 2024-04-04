# Comparing `tmp/security-constraints-1.2.0.tar.gz` & `tmp/security-constraints-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "security-constraints-1.2.0.tar", last modified: Fri Oct 13 15:25:36 2023, max compression
+gzip compressed data, was "security-constraints-1.2.1.tar", last modified: Thu Apr  4 08:51:16 2024, max compression
```

## Comparing `security-constraints-1.2.0.tar` & `security-constraints-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:36.137602 security-constraints-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:36.129602 security-constraints-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:36.133602 security-constraints-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-10-13 15:25:26.000000 security-constraints-1.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-10-13 15:25:26.000000 security-constraints-1.2.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-13 15:25:26.000000 security-constraints-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-13 15:25:26.000000 security-constraints-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17850 2023-10-13 15:25:36.137602 security-constraints-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2023-10-13 15:25:26.000000 security-constraints-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2023-10-13 15:25:26.000000 security-constraints-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-13 15:25:26.000000 security-constraints-1.2.0/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-13 15:25:26.000000 security-constraints-1.2.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 15:25:36.137602 security-constraints-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:36.129602 security-constraints-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:36.133602 security-constraints-1.2.0/src/security_constraints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:26.000000 security-constraints-1.2.0/src/security_constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2023-10-13 15:25:26.000000 security-constraints-1.2.0/src/security_constraints/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2023-10-13 15:25:26.000000 security-constraints-1.2.0/src/security_constraints/github_security_advisory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2023-10-13 15:25:26.000000 security-constraints-1.2.0/src/security_constraints/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:26.000000 security-constraints-1.2.0/src/security_constraints/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:36.133602 security-constraints-1.2.0/src/security_constraints.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17850 2023-10-13 15:25:36.000000 security-constraints-1.2.0/src/security_constraints.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-10-13 15:25:36.000000 security-constraints-1.2.0/src/security_constraints.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 15:25:36.000000 security-constraints-1.2.0/src/security_constraints.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-13 15:25:36.000000 security-constraints-1.2.0/src/security_constraints.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-13 15:25:36.000000 security-constraints-1.2.0/src/security_constraints.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-13 15:25:36.000000 security-constraints-1.2.0/src/security_constraints.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:36.137602 security-constraints-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-10-13 15:25:26.000000 security-constraints-1.2.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 15:25:36.137602 security-constraints-1.2.0/test/system_test/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 15:25:26.000000 security-constraints-1.2.0/test/system_test/sc-conf.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      869 2023-10-13 15:25:26.000000 security-constraints-1.2.0/test/system_test/system_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2023-10-13 15:25:26.000000 security-constraints-1.2.0/test/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2023-10-13 15:25:26.000000 security-constraints-1.2.0/test/test_github_security_advisory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2023-10-13 15:25:26.000000 security-constraints-1.2.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    25957 2023-10-13 15:25:26.000000 security-constraints-1.2.0/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-10-13 15:25:26.000000 security-constraints-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:16.379123 security-constraints-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:16.371122 security-constraints-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:16.375123 security-constraints-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-04 08:51:09.000000 security-constraints-1.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-04 08:51:09.000000 security-constraints-1.2.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-04 08:51:09.000000 security-constraints-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 08:51:09.000000 security-constraints-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-04-04 08:51:16.379123 security-constraints-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-04 08:51:09.000000 security-constraints-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-04 08:51:09.000000 security-constraints-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 08:51:09.000000 security-constraints-1.2.1/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 08:51:09.000000 security-constraints-1.2.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 08:51:16.379123 security-constraints-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:16.375123 security-constraints-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:16.375123 security-constraints-1.2.1/src/security_constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:09.000000 security-constraints-1.2.1/src/security_constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-04 08:51:09.000000 security-constraints-1.2.1/src/security_constraints/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-04 08:51:09.000000 security-constraints-1.2.1/src/security_constraints/github_security_advisory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-04 08:51:09.000000 security-constraints-1.2.1/src/security_constraints/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:09.000000 security-constraints-1.2.1/src/security_constraints/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:16.379123 security-constraints-1.2.1/src/security_constraints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-04-04 08:51:16.000000 security-constraints-1.2.1/src/security_constraints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-04 08:51:16.000000 security-constraints-1.2.1/src/security_constraints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:51:16.000000 security-constraints-1.2.1/src/security_constraints.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 08:51:16.000000 security-constraints-1.2.1/src/security_constraints.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 08:51:16.000000 security-constraints-1.2.1/src/security_constraints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 08:51:16.000000 security-constraints-1.2.1/src/security_constraints.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:16.379123 security-constraints-1.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-04 08:51:09.000000 security-constraints-1.2.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:51:16.379123 security-constraints-1.2.1/test/system_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 08:51:09.000000 security-constraints-1.2.1/test/system_test/sc-conf.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      869 2024-04-04 08:51:09.000000 security-constraints-1.2.1/test/system_test/system_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-04 08:51:09.000000 security-constraints-1.2.1/test/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-04 08:51:09.000000 security-constraints-1.2.1/test/test_github_security_advisory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-04 08:51:09.000000 security-constraints-1.2.1/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27580 2024-04-04 08:51:09.000000 security-constraints-1.2.1/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-04 08:51:09.000000 security-constraints-1.2.1/tox.ini
```

### Comparing `security-constraints-1.2.0/.github/workflows/ci.yaml` & `security-constraints-1.2.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/.github/workflows/publish.yaml` & `security-constraints-1.2.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/.gitignore` & `security-constraints-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/LICENSE` & `security-constraints-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/PKG-INFO` & `security-constraints-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security-constraints
-Version: 1.2.0
+Version: 1.2.1
 Summary: Fetches security vulnerabilities and creates pip-constraints based on them.
 Author: Anton Vikström
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `security-constraints-1.2.0/README.md` & `security-constraints-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/pyproject.toml` & `security-constraints-1.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -74,14 +74,16 @@
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_equality = true
 extra_checks = true
 
 [tool.ruff]
 src = ["src", "test"]
+
+[tool.ruff.lint]
 select = [
   "E",   # pycodestyle
   "F",   # pyflakes
   "UP",  # pyupgrade
   "S",   # flake8-bandit
   "D",   # pydocstyle
   "PT",  # flake8-pytest-style
@@ -111,30 +113,31 @@
   "T20",  # flake8-print
   "TCH",  # flake8-type-checking
 ]
 ignore = [
   "D100", "D102", "D103", "D104", "D105", "D107",
   "PTH123",
   "TRY003", "TRY301",
+  "UP032",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "test/**/*.py" = [
   "S101", "S105",
   "D103",
   "FBT001",
   "SLF001",
   "PLR2004", "PLR0913",
   "ARG001",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 parametrize-names-type = "csv"
 parametrize-values-type = "list"
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "parents"
```

### Comparing `security-constraints-1.2.0/src/security_constraints/common.py` & `security-constraints-1.2.1/src/security_constraints/common.py`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/src/security_constraints/github_security_advisory.py` & `security-constraints-1.2.1/src/security_constraints/github_security_advisory.py`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/src/security_constraints/main.py` & `security-constraints-1.2.1/src/security_constraints/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,17 @@
     return vulnerabilities
 
 
 def sort_vulnerabilities(
     vulnerabilities: List[SecurityVulnerability],
 ) -> List[SecurityVulnerability]:
     """Sort vulnerabilities into the order they should appear in the constraints."""
-    return sorted(vulnerabilities, key=lambda v: v.package)
+    sorted_vulnerabilities = sorted(vulnerabilities, key=lambda v: v.identifier)
+    sorted_vulnerabilities.sort(key=lambda v: v.package)
+    return sorted_vulnerabilities
 
 
 def get_safe_version_constraints(
     vulnerability: SecurityVulnerability,
 ) -> PackageConstraints:
     """Invert range of a vulnerability into constraints specifying unaffected versions.
```

### Comparing `security-constraints-1.2.0/src/security_constraints.egg-info/PKG-INFO` & `security-constraints-1.2.1/src/security_constraints.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security-constraints
-Version: 1.2.0
+Version: 1.2.1
 Summary: Fetches security vulnerabilities and creates pip-constraints based on them.
 Author: Anton Vikström
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `security-constraints-1.2.0/src/security_constraints.egg-info/SOURCES.txt` & `security-constraints-1.2.1/src/security_constraints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/test/conftest.py` & `security-constraints-1.2.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/test/system_test/system_test.sh` & `security-constraints-1.2.1/test/system_test/system_test.sh`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/test/test_common.py` & `security-constraints-1.2.1/test/test_common.py`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/test/test_github_security_advisory.py` & `security-constraints-1.2.1/test/test_github_security_advisory.py`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/test/test_integration.py` & `security-constraints-1.2.1/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `security-constraints-1.2.0/test/test_main.py` & `security-constraints-1.2.1/test/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,20 +325,67 @@
                     identifier="GHSA-1",
                     package="pystuff",
                     vulnerable_range="= 1.0",
                 ),
             ],
         ),
         ([], []),
+        (
+            [
+                SecurityVulnerability(
+                    name="CVE-2",
+                    identifier="GHSA-2",
+                    package="pybanana",
+                    vulnerable_range="= 2.0",
+                ),
+                SecurityVulnerability(
+                    name="CVE-3U",
+                    identifier="GHSA-3",
+                    package="pypeel",
+                    vulnerable_range="< 3.0dev1",
+                ),
+                SecurityVulnerability(
+                    name="CVE-1",
+                    identifier="GHSA-1",
+                    package="pybanana",
+                    vulnerable_range="= 1.0",
+                ),
+            ],
+            [
+                SecurityVulnerability(
+                    name="CVE-1",
+                    identifier="GHSA-1",
+                    package="pybanana",
+                    vulnerable_range="= 1.0",
+                ),
+                SecurityVulnerability(
+                    name="CVE-2",
+                    identifier="GHSA-2",
+                    package="pybanana",
+                    vulnerable_range="= 2.0",
+                ),
+                SecurityVulnerability(
+                    name="CVE-3U",
+                    identifier="GHSA-3",
+                    package="pypeel",
+                    vulnerable_range="< 3.0dev1",
+                ),
+            ],
+        ),
     ],
+    ids=["sort by package", "empty", "sub-sort by identifier"],
 )
 def test_sort_vulnerabilities(
     vulnerabilities: List[SecurityVulnerability], expected: List[SecurityVulnerability]
 ) -> None:
+    original_vulnerabilities = vulnerabilities.copy()
     assert sort_vulnerabilities(vulnerabilities=vulnerabilities) == expected
+    assert (
+        vulnerabilities == original_vulnerabilities
+    ), "input list was altered in-place"
 
 
 @pytest.mark.parametrize(
     "db_names, config, expected",
     [
         (
             ["FakeDB"],
```

