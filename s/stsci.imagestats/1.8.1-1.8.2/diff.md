# Comparing `tmp/stsci.imagestats-1.8.1.tar.gz` & `tmp/stsci.imagestats-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stsci.imagestats-1.8.1.tar", last modified: Fri Mar 22 18:10:23 2024, max compression
+gzip compressed data, was "stsci.imagestats-1.8.2.tar", last modified: Thu Apr  4 06:47:10 2024, max compression
```

## Comparing `stsci.imagestats-1.8.1.tar` & `stsci.imagestats-1.8.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.826041 stsci.imagestats-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.814041 stsci.imagestats-1.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.818041 stsci.imagestats-1.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-22 18:10:23.826041 stsci.imagestats-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.818041 stsci.imagestats-1.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.818041 stsci.imagestats-1.8.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.818041 stsci.imagestats-1.8.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   122264 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    65413 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/_static/stsci_pri_combo_mark_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.818041 stsci.imagestats-1.8.1/docs/exts/
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/exts/numfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.822041 stsci.imagestats-1.8.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/source/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/source/histogram1d.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/docs/source/imagestats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 18:10:23.826041 stsci.imagestats-1.8.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.822041 stsci.imagestats-1.8.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/src/buildHistogram.c
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/src/computeMean.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.814041 stsci.imagestats-1.8.1/stsci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.822041 stsci.imagestats-1.8.1/stsci/imagestats/
--rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/stsci/imagestats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-22 18:10:23.000000 stsci.imagestats-1.8.1/stsci/imagestats/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/stsci/imagestats/histogram1d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.822041 stsci.imagestats-1.8.1/stsci/imagestats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/stsci/imagestats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/stsci/imagestats/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/stsci/imagestats/tests/test_histogram1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/stsci/imagestats/tests/test_imagestats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:10:23.822041 stsci.imagestats-1.8.1/stsci.imagestats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-22 18:10:23.000000 stsci.imagestats-1.8.1/stsci.imagestats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-22 18:10:23.000000 stsci.imagestats-1.8.1/stsci.imagestats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:10:23.000000 stsci.imagestats-1.8.1/stsci.imagestats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:10:23.000000 stsci.imagestats-1.8.1/stsci.imagestats.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-22 18:10:23.000000 stsci.imagestats-1.8.1/stsci.imagestats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 18:10:23.000000 stsci.imagestats-1.8.1/stsci.imagestats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-22 18:10:06.000000 stsci.imagestats-1.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.422521 stsci.imagestats-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.414521 stsci.imagestats-1.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.418521 stsci.imagestats-1.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-04 06:47:10.422521 stsci.imagestats-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.418521 stsci.imagestats-1.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.418521 stsci.imagestats-1.8.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.418521 stsci.imagestats-1.8.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   122264 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    65413 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/_static/stsci_pri_combo_mark_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.418521 stsci.imagestats-1.8.2/docs/exts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/exts/numfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.418521 stsci.imagestats-1.8.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/source/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/source/histogram1d.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/docs/source/imagestats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 06:47:10.422521 stsci.imagestats-1.8.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.422521 stsci.imagestats-1.8.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/src/buildHistogram.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/src/computeMean.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.414521 stsci.imagestats-1.8.2/stsci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.422521 stsci.imagestats-1.8.2/stsci/imagestats/
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/stsci/imagestats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 06:47:10.000000 stsci.imagestats-1.8.2/stsci/imagestats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/stsci/imagestats/histogram1d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.422521 stsci.imagestats-1.8.2/stsci/imagestats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/stsci/imagestats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/stsci/imagestats/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/stsci/imagestats/tests/test_histogram1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/stsci/imagestats/tests/test_imagestats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:47:10.422521 stsci.imagestats-1.8.2/stsci.imagestats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-04 06:47:10.000000 stsci.imagestats-1.8.2/stsci.imagestats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-04 06:47:10.000000 stsci.imagestats-1.8.2/stsci.imagestats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 06:47:10.000000 stsci.imagestats-1.8.2/stsci.imagestats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 06:47:10.000000 stsci.imagestats-1.8.2/stsci.imagestats.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-04 06:47:10.000000 stsci.imagestats-1.8.2/stsci.imagestats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 06:47:10.000000 stsci.imagestats-1.8.2/stsci.imagestats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-04 06:46:59.000000 stsci.imagestats-1.8.2/tox.ini
```

### Comparing `stsci.imagestats-1.8.1/.github/workflows/build.yml` & `stsci.imagestats-1.8.2/.github/workflows/build.yml`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,15 @@
       upload_to_pypi: ${{ (github.event_name == 'release') && (github.event.action == 'released') }}
       targets: |
         # Linux wheels
         - cp3*-manylinux_x86_64
         # MacOS wheels
         - cp3*-macosx_x86_64
         # Until we have arm64 runners, we can't automatically test arm64 wheels
-        - cp3*-macosx_arm64
+        # Disabling this due to permission errors
+        # - cp3*-macosx_arm64
         # Windows wheels
         - cp3*-win32
         - cp3*-win_amd64
       sdist: true
     secrets:
       pypi_token: ${{ secrets.PYPI_PASSWORD_STSCI_MAINTAINER }}
```

### Comparing `stsci.imagestats-1.8.1/.github/workflows/ci.yml` & `stsci.imagestats-1.8.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/.gitignore` & `stsci.imagestats-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/CHANGELOG.rst` & `stsci.imagestats-1.8.2/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 .. _release_notes:
 
 =============
 Release Notes
 =============
 
-.. 1.8.2 (unreleased)
-   ==================
+
+1.8.2 (04-April-2024)
+=====================
+
+- Bug Fix: Improve handling of floating point accuracy issues that can lead to
+  memory violation on some systems. The fix from [#58] was only partial. [#59]
+
 
 1.8.1 (22-March-2024)
 =====================
 
 - Bug Fix: Improve handling of floating point accuracy issues that can lead to
   memory violation on some systems. [#58]
 
+
 1.8.0 (07-December-2023)
 ========================
 
 - Removed support for Python 3.7 and 3.8. [#52]
 
 - Improvements in the package infrastructure. [#52, 55]
```

### Comparing `stsci.imagestats-1.8.1/CODE_OF_CONDUCT.md` & `stsci.imagestats-1.8.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/LICENSE.txt` & `stsci.imagestats-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/PKG-INFO` & `stsci.imagestats-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsci.imagestats
-Version: 1.8.1
+Version: 1.8.2
 Summary: Compute sigma-clipped statistics on data arrays
 Author: Christopher Hanley
 Author-email: Warren Hack <help@stsci.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/spacetelescope/stsci.imagestats
 Project-URL: Tracker, https://github.com/spacetelescope/stsci.imagestats/issues
 Project-URL: Documentation, https://stsciimagestats.readthedocs.io/en/stable/
```

### Comparing `stsci.imagestats-1.8.1/README.rst` & `stsci.imagestats-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/docs/Makefile` & `stsci.imagestats-1.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/docs/_static/css/custom.css` & `stsci.imagestats-1.8.2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/docs/_static/stsci_pri_combo_mark_white.png` & `stsci.imagestats-1.8.2/docs/_static/stsci_pri_combo_mark_white.png`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/docs/conf.py` & `stsci.imagestats-1.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/docs/exts/numfig.py` & `stsci.imagestats-1.8.2/docs/exts/numfig.py`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/docs/index.rst` & `stsci.imagestats-1.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/docs/make.bat` & `stsci.imagestats-1.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/pyproject.toml` & `stsci.imagestats-1.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/setup.py` & `stsci.imagestats-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/src/buildHistogram.c` & `stsci.imagestats-1.8.2/src/buildHistogram.c`

 * *Files 10% similar despite different names*

```diff
@@ -11,76 +11,77 @@
 #include "numpy/arrayobject.h"
 
 int
 populate1DHist_(float *image, int image_elements, unsigned int *histogram,
                 int histogram_elements, float minValue, float maxValue,
                 float binWidth)
 {
-    int i, idx, allow_max_eq = 0;
+    int i, idx;
     float f, hist_edge, v;
 
     f = 1.0f / binWidth;
     hist_edge = minValue + binWidth * histogram_elements;
-    if ((int) (f * (hist_edge - minValue)) == histogram_elements) {
-        hist_edge *= (1.0f - FLT_EPSILON);
-        allow_max_eq = 1;
-    }
     if (maxValue > hist_edge) {
         maxValue = hist_edge;
     }
-
-    if (allow_max_eq) {
-        for (i = 0; i < image_elements; ++i) {
-            v = image[i];
-            if ((v >= minValue) && (v <= maxValue)) {
-                idx = (int)(f * (v - minValue));
-                ++histogram[idx];
-            }
-        }
-    } else {
-        for (i = 0; i < image_elements; ++i) {
-            v = image[i];
-            if ((v >= minValue) && (v < maxValue)) {
-                idx = (int)(f * (v - minValue));
-                ++histogram[idx];
-            }
+    for (i = 0; i < image_elements; ++i) {
+        v = image[i];
+        if ((v >= minValue) && (v < maxValue)) {
+            idx = (int)(f * (v - minValue));
+            ++histogram[idx];
         }
     }
 
     return 1;
 }
 
 static PyObject *
 populate1DHist(PyObject *obj, PyObject *args)
 {
     PyObject *oimage, *ohistogram;
     PyArrayObject *image, *histogram;
     float minValue, maxValue, binWidth;
-    int status;
+    unsigned int *p, *hdata;
+    int status, size, i;
 
     (void)obj;
 
     if (!PyArg_ParseTuple(args, "OOfff:populate1DHist", &oimage, &ohistogram,
                           &minValue, &maxValue, &binWidth))
         return NULL;
 
     image = (PyArrayObject *)PyArray_ContiguousFromObject(oimage, NPY_FLOAT32,
                                                           1, 2);
 
     if (!image) return NULL;
 
     histogram = (PyArrayObject *)PyArray_ContiguousFromObject(
         ohistogram, NPY_UINT32, 1, 1);
+    if (!histogram) {
+        Py_XDECREF(image);
+        return NULL;
+    }
 
-    if (!histogram) return NULL;
+    size = PyArray_Size((PyObject *)histogram);
+    p = (unsigned int *)calloc(size + 1, sizeof(unsigned int));
+    if (!p) {
+        Py_XDECREF(image);
+        Py_XDECREF(histogram);
+        return NULL;
+    }
 
-    status = populate1DHist_(
-        (float *)PyArray_DATA(image), PyArray_Size((PyObject *)image),
-        (unsigned int *)PyArray_DATA(histogram),
-        PyArray_Size((PyObject *)histogram), minValue, maxValue, binWidth);
+    status = populate1DHist_((float *)PyArray_DATA(image),
+                             PyArray_Size((PyObject *)image), p, size,
+                             minValue, maxValue, binWidth);
+
+    hdata = (unsigned int *)PyArray_DATA(histogram);
+    for (i = 0; i < size; ++i) {
+        hdata[i] += p[i];
+    }
+    free(p);
 
     Py_XDECREF(image);
     Py_XDECREF(histogram);
 
     return Py_BuildValue("i", status);
 }
```

### Comparing `stsci.imagestats-1.8.1/src/computeMean.c` & `stsci.imagestats-1.8.2/src/computeMean.c`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/stsci/imagestats/__init__.py` & `stsci.imagestats-1.8.2/stsci/imagestats/__init__.py`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/stsci/imagestats/histogram1d.py` & `stsci.imagestats-1.8.2/stsci/imagestats/histogram1d.py`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/stsci/imagestats/tests/conftest.py` & `stsci.imagestats-1.8.2/stsci/imagestats/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/stsci/imagestats/tests/test_histogram1d.py` & `stsci.imagestats-1.8.2/stsci/imagestats/tests/test_histogram1d.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,35 @@
     assert diff.sum() == 0
     assert max(np.abs(diff)) <= 1
     assert np.flatnonzero(diff).size < 4
 
     assert np.allclose(h.edges, npedges, rtol=0.0, atol=10.0 * _EPS32)
 
 
+def test_histogram_upper_bin_flt_roundoff(gaussian_image):
+    """ Similar data (limit, binwidth, and nbins => upper histogram edge
+        are relevant) were causing segfault on some Linux machines due to
+        bin index exceeding allocated memory.
+    """
+    mean = gaussian_image.meta['mean']
+    data = 4.0 * (gaussian_image.astype(np.float32).ravel() - mean) + 0.5
+    data[0] = 1.0441159009933472  # data from reported failure
+    minv = -0.380480386316776276
+
+    h = histogram1d(
+        arrayInput=data,
+        nbins=87,
+        binWidth=0.01637466996908188,
+        zeroValue=minv
+    )
+    assert np.sum(h.histogram) == np.sum(
+        np.logical_and(data >= minv, data < 1.0441159009933472)
+    )
+
+
 @pytest.mark.parametrize(
     'value,truth',
     [
         (0.0, [1, 0]),
         (_TINY32, [1, 0]),
         (-_TINY32, [0, 0]),
         (1.0 - _EPS32, [0, 1]),
```

### Comparing `stsci.imagestats-1.8.1/stsci/imagestats/tests/test_imagestats.py` & `stsci.imagestats-1.8.2/stsci/imagestats/tests/test_imagestats.py`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/stsci.imagestats.egg-info/PKG-INFO` & `stsci.imagestats-1.8.2/stsci.imagestats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsci.imagestats
-Version: 1.8.1
+Version: 1.8.2
 Summary: Compute sigma-clipped statistics on data arrays
 Author: Christopher Hanley
 Author-email: Warren Hack <help@stsci.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/spacetelescope/stsci.imagestats
 Project-URL: Tracker, https://github.com/spacetelescope/stsci.imagestats/issues
 Project-URL: Documentation, https://stsciimagestats.readthedocs.io/en/stable/
```

### Comparing `stsci.imagestats-1.8.1/stsci.imagestats.egg-info/SOURCES.txt` & `stsci.imagestats-1.8.2/stsci.imagestats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stsci.imagestats-1.8.1/tox.ini` & `stsci.imagestats-1.8.2/tox.ini`

 * *Files identical despite different names*

