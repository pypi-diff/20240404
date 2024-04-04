# Comparing `tmp/rbstata-0.1.0.tar.gz` & `tmp/rbstata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbstata-0.1.0.tar", last modified: Thu Apr  4 07:08:35 2024, max compression
+gzip compressed data, was "rbstata-0.1.1.tar", last modified: Thu Apr  4 07:37:03 2024, max compression
```

## Comparing `rbstata-0.1.0.tar` & `rbstata-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-04-04 07:08:35.470153 rbstata-0.1.0/
--rw-r--r--   0 lsys      (1000) lsys      (1000)     1094 2024-04-04 06:04:46.000000 rbstata-0.1.0/LICENSE
--rw-r--r--   0 lsys      (1000) lsys      (1000)    10203 2024-04-04 07:08:35.470153 rbstata-0.1.0/PKG-INFO
--rw-r--r--   0 lsys      (1000) lsys      (1000)     9403 2024-04-04 06:53:00.000000 rbstata-0.1.0/README.md
-drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-04-04 07:08:35.470153 rbstata-0.1.0/rbStata/
--rw-r--r--   0 lsys      (1000) lsys      (1000)       75 2024-04-02 05:18:20.000000 rbstata-0.1.0/rbStata/__init__.py
--rw-r--r--   0 lsys      (1000) lsys      (1000)     8741 2024-04-04 07:08:34.000000 rbstata-0.1.0/rbStata/cli.py
--rw-r--r--   0 lsys      (1000) lsys      (1000)     6224 2024-04-04 06:00:34.000000 rbstata-0.1.0/rbStata/helpers.py
-drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-04-04 07:08:35.470153 rbstata-0.1.0/rbstata.egg-info/
--rw-r--r--   0 lsys      (1000) lsys      (1000)    10203 2024-04-04 07:08:35.000000 rbstata-0.1.0/rbstata.egg-info/PKG-INFO
--rw-r--r--   0 lsys      (1000) lsys      (1000)      338 2024-04-04 07:08:35.000000 rbstata-0.1.0/rbstata.egg-info/SOURCES.txt
--rw-r--r--   0 lsys      (1000) lsys      (1000)        1 2024-04-04 07:08:35.000000 rbstata-0.1.0/rbstata.egg-info/dependency_links.txt
--rw-r--r--   0 lsys      (1000) lsys      (1000)       48 2024-04-04 07:08:35.000000 rbstata-0.1.0/rbstata.egg-info/entry_points.txt
--rw-r--r--   0 lsys      (1000) lsys      (1000)        1 2024-04-04 07:08:35.000000 rbstata-0.1.0/rbstata.egg-info/not-zip-safe
--rw-r--r--   0 lsys      (1000) lsys      (1000)       27 2024-04-04 07:08:35.000000 rbstata-0.1.0/rbstata.egg-info/requires.txt
--rw-r--r--   0 lsys      (1000) lsys      (1000)       14 2024-04-04 07:08:35.000000 rbstata-0.1.0/rbstata.egg-info/top_level.txt
--rw-r--r--   0 lsys      (1000) lsys      (1000)       38 2024-04-04 07:08:35.470153 rbstata-0.1.0/setup.cfg
--rw-r--r--   0 lsys      (1000) lsys      (1000)     1557 2024-04-04 06:58:42.000000 rbstata-0.1.0/setup.py
-drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-04-04 07:08:35.470153 rbstata-0.1.0/tests/
--rw-r--r--   0 lsys      (1000) lsys      (1000)       12 2023-03-05 05:30:23.000000 rbstata-0.1.0/tests/__init__.py
--rw-r--r--   0 lsys      (1000) lsys      (1000)     7377 2024-04-04 07:08:35.000000 rbstata-0.1.0/tests/test_rbstata.py
+drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-04-04 07:37:03.710041 rbstata-0.1.1/
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     1094 2024-04-04 06:04:46.000000 rbstata-0.1.1/LICENSE
+-rw-r--r--   0 lsys      (1000) lsys      (1000)    10352 2024-04-04 07:37:03.710041 rbstata-0.1.1/PKG-INFO
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     9552 2024-04-04 07:30:40.000000 rbstata-0.1.1/README.md
+drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-04-04 07:37:03.710041 rbstata-0.1.1/rbStata/
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       75 2024-04-04 07:36:17.000000 rbstata-0.1.1/rbStata/__init__.py
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     8741 2024-04-04 07:37:03.000000 rbstata-0.1.1/rbStata/cli.py
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     6224 2024-04-04 06:00:34.000000 rbstata-0.1.1/rbStata/helpers.py
+drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-04-04 07:37:03.710041 rbstata-0.1.1/rbstata.egg-info/
+-rw-r--r--   0 lsys      (1000) lsys      (1000)    10352 2024-04-04 07:37:03.000000 rbstata-0.1.1/rbstata.egg-info/PKG-INFO
+-rw-r--r--   0 lsys      (1000) lsys      (1000)      338 2024-04-04 07:37:03.000000 rbstata-0.1.1/rbstata.egg-info/SOURCES.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)        1 2024-04-04 07:37:03.000000 rbstata-0.1.1/rbstata.egg-info/dependency_links.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       48 2024-04-04 07:37:03.000000 rbstata-0.1.1/rbstata.egg-info/entry_points.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)        1 2024-04-04 07:37:03.000000 rbstata-0.1.1/rbstata.egg-info/not-zip-safe
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       27 2024-04-04 07:37:03.000000 rbstata-0.1.1/rbstata.egg-info/requires.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       14 2024-04-04 07:37:03.000000 rbstata-0.1.1/rbstata.egg-info/top_level.txt
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       38 2024-04-04 07:37:03.710041 rbstata-0.1.1/setup.cfg
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     1557 2024-04-04 07:36:09.000000 rbstata-0.1.1/setup.py
+drwxr-xr-x   0 lsys      (1000) lsys      (1000)        0 2024-04-04 07:37:03.710041 rbstata-0.1.1/tests/
+-rw-r--r--   0 lsys      (1000) lsys      (1000)       12 2023-03-05 05:30:23.000000 rbstata-0.1.1/tests/__init__.py
+-rw-r--r--   0 lsys      (1000) lsys      (1000)     7377 2024-04-04 07:37:03.000000 rbstata-0.1.1/tests/test_rbstata.py
```

### Comparing `rbstata-0.1.0/LICENSE` & `rbstata-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rbstata-0.1.0/PKG-INFO` & `rbstata-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbstata
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command-line utility that converts (or roll back) versions of Stata dta data files.
 Home-page: https://github.com/lsys/rbStata
 Author: Lucas Shen
 Author-email: lucas@lucasshen.com
 License: MIT
 Keywords: Stata,Python,cli,compatibility,version
 Classifier: Environment :: Console
@@ -34,15 +34,15 @@
   - Variable labels
   - Data labels
   - Value labels
 
 | | |
 | --- | --- |
 | Package | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rbStata?label=Python%203.6%2B&logo=python&logoColor=white)](https://pypi.org/project/rbStata/) [![PyPI](https://img.shields.io/pypi/v/rbStata?color=blue&label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/rbStata/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/lsys/rbStata?color=blue&label=Latest%20release)](https://github.com/LSYS/rbStata/releases) |
-| Testing/build | [![Coverage](https://codecov.io/github/lsys/rbStata/coverage.svg?branch=main)](https://codecov.io/gh/lsys/rbStata) [![CI](https://github.com/LSYS/rbStata/actions/workflows/build.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/build.yml) [![CLI](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml) [![DocLinks](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml) |
+| Testing/build | [![Coverage](https://codecov.io/github/lsys/rbStata/coverage.svg?branch=main)](https://codecov.io/gh/lsys/rbStata) [![CI](https://github.com/LSYS/rbStata/actions/workflows/build.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/build.yml) [![CLI](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml) [![Pkg-CLI](https://github.com/LSYS/rbStata/actions/workflows/Pkg-CLI.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/Pkg-CLI.yml) [![DocLinks](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml) |
 | Meta | [![DOI](https://zenodo.org/badge/532792769.svg)](https://zenodo.org/doi/10.5281/zenodo.10925080) [![GitHub](https://img.shields.io/github/license/lsys/rbStata?color=purple&label=License)](https://choosealicense.com/licenses/mit/) |
 
 ## Statement of Need
 
 Stata `.dta` data files are not forward compatible. 
 This means you cannot use older versions (e.g., `Stata 13`) to read a `.dta` file exported from newer versions (e.g., `Stata 17`).
```

### Comparing `rbstata-0.1.0/README.md` & `rbstata-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   - Variable labels
   - Data labels
   - Value labels
 
 | | |
 | --- | --- |
 | Package | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rbStata?label=Python%203.6%2B&logo=python&logoColor=white)](https://pypi.org/project/rbStata/) [![PyPI](https://img.shields.io/pypi/v/rbStata?color=blue&label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/rbStata/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/lsys/rbStata?color=blue&label=Latest%20release)](https://github.com/LSYS/rbStata/releases) |
-| Testing/build | [![Coverage](https://codecov.io/github/lsys/rbStata/coverage.svg?branch=main)](https://codecov.io/gh/lsys/rbStata) [![CI](https://github.com/LSYS/rbStata/actions/workflows/build.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/build.yml) [![CLI](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml) [![DocLinks](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml) |
+| Testing/build | [![Coverage](https://codecov.io/github/lsys/rbStata/coverage.svg?branch=main)](https://codecov.io/gh/lsys/rbStata) [![CI](https://github.com/LSYS/rbStata/actions/workflows/build.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/build.yml) [![CLI](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml) [![Pkg-CLI](https://github.com/LSYS/rbStata/actions/workflows/Pkg-CLI.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/Pkg-CLI.yml) [![DocLinks](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml) |
 | Meta | [![DOI](https://zenodo.org/badge/532792769.svg)](https://zenodo.org/doi/10.5281/zenodo.10925080) [![GitHub](https://img.shields.io/github/license/lsys/rbStata?color=purple&label=License)](https://choosealicense.com/licenses/mit/) |
 
 ## Statement of Need
 
 Stata `.dta` data files are not forward compatible. 
 This means you cannot use older versions (e.g., `Stata 13`) to read a `.dta` file exported from newer versions (e.g., `Stata 17`).
```

### Comparing `rbstata-0.1.0/rbStata/cli.py` & `rbstata-0.1.1/rbStata/cli.py`

 * *Files identical despite different names*

### Comparing `rbstata-0.1.0/rbStata/helpers.py` & `rbstata-0.1.1/rbStata/helpers.py`

 * *Files identical despite different names*

### Comparing `rbstata-0.1.0/rbstata.egg-info/PKG-INFO` & `rbstata-0.1.1/rbstata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbstata
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command-line utility that converts (or roll back) versions of Stata dta data files.
 Home-page: https://github.com/lsys/rbStata
 Author: Lucas Shen
 Author-email: lucas@lucasshen.com
 License: MIT
 Keywords: Stata,Python,cli,compatibility,version
 Classifier: Environment :: Console
@@ -34,15 +34,15 @@
   - Variable labels
   - Data labels
   - Value labels
 
 | | |
 | --- | --- |
 | Package | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rbStata?label=Python%203.6%2B&logo=python&logoColor=white)](https://pypi.org/project/rbStata/) [![PyPI](https://img.shields.io/pypi/v/rbStata?color=blue&label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/rbStata/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/lsys/rbStata?color=blue&label=Latest%20release)](https://github.com/LSYS/rbStata/releases) |
-| Testing/build | [![Coverage](https://codecov.io/github/lsys/rbStata/coverage.svg?branch=main)](https://codecov.io/gh/lsys/rbStata) [![CI](https://github.com/LSYS/rbStata/actions/workflows/build.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/build.yml) [![CLI](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml) [![DocLinks](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml) |
+| Testing/build | [![Coverage](https://codecov.io/github/lsys/rbStata/coverage.svg?branch=main)](https://codecov.io/gh/lsys/rbStata) [![CI](https://github.com/LSYS/rbStata/actions/workflows/build.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/build.yml) [![CLI](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/cli-pkg.yml) [![Pkg-CLI](https://github.com/LSYS/rbStata/actions/workflows/Pkg-CLI.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/Pkg-CLI.yml) [![DocLinks](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml/badge.svg)](https://github.com/LSYS/rbStata/actions/workflows/doclinks.yml) |
 | Meta | [![DOI](https://zenodo.org/badge/532792769.svg)](https://zenodo.org/doi/10.5281/zenodo.10925080) [![GitHub](https://img.shields.io/github/license/lsys/rbStata?color=purple&label=License)](https://choosealicense.com/licenses/mit/) |
 
 ## Statement of Need
 
 Stata `.dta` data files are not forward compatible. 
 This means you cannot use older versions (e.g., `Stata 13`) to read a `.dta` file exported from newer versions (e.g., `Stata 17`).
```

### Comparing `rbstata-0.1.0/setup.py` & `rbstata-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "pandas",
     "anyascii",
     "click==8.*",
 ]
 
 setup(
     name="rbstata",
-    version="0.1.0",
+    version="0.1.1",
     description=(
         "A command-line utility that converts (or roll back) versions of Stata dta data files."
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Lucas Shen",
     author_email="lucas@lucasshen.com",
```

### Comparing `rbstata-0.1.0/tests/test_rbstata.py` & `rbstata-0.1.1/tests/test_rbstata.py`

 * *Files identical despite different names*

