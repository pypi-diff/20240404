# Comparing `tmp/blastpipe-2024.0.2.tar.gz` & `tmp/blastpipe-2024.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.0.2.tar", last modified: Wed Apr  3 02:14:57 2024, max compression
+gzip compressed data, was "blastpipe-2024.0.3.tar", last modified: Thu Apr  4 03:34:55 2024, max compression
```

## Comparing `blastpipe-2024.0.2.tar` & `blastpipe-2024.0.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:14:57.943128 blastpipe-2024.0.2/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)    11661 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    64115 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-03 02:14:57.943128 blastpipe-2024.0.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3214 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1293 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     2943 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8557 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-03 02:01:27.000000 blastpipe-2024.0.2/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:34:55.091736 blastpipe-2024.0.3/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)    11661 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    64567 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-04 03:34:55.091736 blastpipe-2024.0.3/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3214 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     2943 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4648 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8557 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.0.2/.github/workflows/codeql.yml` & `blastpipe-2024.0.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/.github/workflows/dependency-review.yml` & `blastpipe-2024.0.3/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/.github/workflows/ozi.yml` & `blastpipe-2024.0.3/.github/workflows/ozi.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/.github/workflows/scorecards.yml` & `blastpipe-2024.0.3/.github/workflows/scorecards.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/.gitignore` & `blastpipe-2024.0.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
 _scm_version.py
-subprojects/dev
+subprojects/ozi
 .Python
 build*/
 develop-eggs/
 /dist/
 downloads/
 eggs/
 .eggs/
```

### Comparing `blastpipe-2024.0.2/CHANGELOG.md` & `blastpipe-2024.0.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v2024.0.3 (2024-04-04)
+
+### :hammer:
+
+* :hammer: Add install-subprojects option.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@mail.umkc.edu&gt; ([`af8f951`](https://github.com/OZI-Project/blastpipe/commit/af8f9519a11ed5efd9a86fc6089afb543688a46e))
+
+### :pencil2:
+
+* :pencil2: remove subproject folder.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@mail.umkc.edu&gt; ([`727b7d0`](https://github.com/OZI-Project/blastpipe/commit/727b7d0ad55627334ab0f2a919e6d1cc45a24652))
+
+
 ## v2024.0.2 (2024-04-03)
 
 ### :hammer:
 
 * :hammer: Don&#39;t bootstrap OZI if blastpipe is a subproject (for now).
 
 Signed-off-by: rjdbcm &lt;rjdbcm@mail.umkc.edu&gt; ([`0068204`](https://github.com/OZI-Project/blastpipe/commit/006820441f7ac3be090ac02a87fbad2ff0e4bf01))
```

### Comparing `blastpipe-2024.0.2/LICENSE.txt` & `blastpipe-2024.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/NOTICE.md` & `blastpipe-2024.0.3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/PKG-INFO` & `blastpipe-2024.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.0.2
+Version: 2024.0.3
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.2.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.3.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `blastpipe-2024.0.2/README.rst` & `blastpipe-2024.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/__init__.py` & `blastpipe-2024.0.3/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/backports.py` & `blastpipe-2024.0.3/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/backports.pyi` & `blastpipe-2024.0.3/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/buffer.py` & `blastpipe-2024.0.3/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/loop.py` & `blastpipe-2024.0.3/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/malloc.py` & `blastpipe-2024.0.3/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/meson.build` & `blastpipe-2024.0.3/blastpipe/meson.build`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     'mixin.pyi',
     'sequence.pyi',
     'tailcall.pyi',
     'py.typed',
 ]
 foreach file: python_files
     fs.copyfile(file)
-    if not meson.is_subproject()
+    if not meson.is_subproject() or get_option('install-subprojects').enabled()
         python.install_sources(file, subdir: project_name)
     endif
 endforeach
 if false
     executable('source_files', python_files)
 endif
 children = []
```

### Comparing `blastpipe-2024.0.2/blastpipe/mixin.py` & `blastpipe-2024.0.3/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/sequence.py` & `blastpipe-2024.0.3/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/blastpipe/tailcall.py` & `blastpipe-2024.0.3/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/meson.build` & `blastpipe-2024.0.3/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/meson.options` & `blastpipe-2024.0.3/meson.options`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         'pytest-asyncio',
         'pytest-cov',
         'pytest-randomly',
         'pytest-tcpclient',
         'pytest-xdist',
     ]
 )
+option('install-subprojects', type: 'feature', value: 'disabled')
 option('source-to-build', type: 'feature', value: 'auto')
 option('build-dir', type: 'feature',  value: 'auto')
 option('project-name', type: 'feature', value: 'auto')
 option('docs-source',type: 'feature',value: 'auto')
 option('test-source',type: 'feature', value: 'auto')
 option('dist', type: 'feature', value: 'auto')
 option('docs', type: 'feature', value: 'auto')
```

### Comparing `blastpipe-2024.0.2/pyproject.toml` & `blastpipe-2024.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/LICENSE.txt` & `blastpipe-2024.0.3/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.0.3/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.0.3/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/_static/meson.build` & `blastpipe-2024.0.3/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/_templates/layout.html` & `blastpipe-2024.0.3/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/_templates/meson.build` & `blastpipe-2024.0.3/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/conf.cfg` & `blastpipe-2024.0.3/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/index.rst` & `blastpipe-2024.0.3/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/meson.build` & `blastpipe-2024.0.3/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/subprojects/docs/meson.options` & `blastpipe-2024.0.3/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/tests/meson.build` & `blastpipe-2024.0.3/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/tests/test_backports.py` & `blastpipe-2024.0.3/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/tests/test_fuzz.py` & `blastpipe-2024.0.3/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.2/tests/test_tailcall.py` & `blastpipe-2024.0.3/tests/test_tailcall.py`

 * *Files identical despite different names*

