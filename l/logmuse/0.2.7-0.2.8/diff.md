# Comparing `tmp/logmuse-0.2.7.tar.gz` & `tmp/logmuse-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logmuse-0.2.7.tar", last modified: Wed Sep  8 19:43:54 2021, max compression
+gzip compressed data, was "logmuse-0.2.8.tar", last modified: Thu Apr  4 15:51:53 2024, max compression
```

## Comparing `logmuse-0.2.7.tar` & `logmuse-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 19:43:54.782585 logmuse-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2021-09-08 19:43:45.000000 logmuse-0.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-08 19:43:45.000000 logmuse-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2021-09-08 19:43:54.782585 logmuse-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      556 2021-09-08 19:43:45.000000 logmuse-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 19:43:54.782585 logmuse-0.2.7/logmuse/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-09-08 19:43:45.000000 logmuse-0.2.7/logmuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-08 19:43:45.000000 logmuse-0.2.7/logmuse/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    14761 2021-09-08 19:43:45.000000 logmuse-0.2.7/logmuse/est.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 19:43:54.782585 logmuse-0.2.7/logmuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2021-09-08 19:43:54.000000 logmuse-0.2.7/logmuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-09-08 19:43:54.000000 logmuse-0.2.7/logmuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-08 19:43:54.000000 logmuse-0.2.7/logmuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-09-08 19:43:54.000000 logmuse-0.2.7/logmuse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 19:43:54.782585 logmuse-0.2.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-09-08 19:43:45.000000 logmuse-0.2.7/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-08 19:43:45.000000 logmuse-0.2.7/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-09-08 19:43:45.000000 logmuse-0.2.7/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-09-08 19:43:54.782585 logmuse-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2021-09-08 19:43:45.000000 logmuse-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:51:53.289098 logmuse-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-04 15:51:45.000000 logmuse-0.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 15:51:45.000000 logmuse-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-04 15:51:53.289098 logmuse-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-04 15:51:45.000000 logmuse-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:51:53.289098 logmuse-0.2.8/logmuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 15:51:45.000000 logmuse-0.2.8/logmuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 15:51:45.000000 logmuse-0.2.8/logmuse/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-04 15:51:45.000000 logmuse-0.2.8/logmuse/est.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:51:53.289098 logmuse-0.2.8/logmuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-04 15:51:53.000000 logmuse-0.2.8/logmuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-04 15:51:53.000000 logmuse-0.2.8/logmuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:51:53.000000 logmuse-0.2.8/logmuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 15:51:53.000000 logmuse-0.2.8/logmuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 15:51:53.000000 logmuse-0.2.8/logmuse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:51:53.289098 logmuse-0.2.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 15:51:45.000000 logmuse-0.2.8/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 15:51:45.000000 logmuse-0.2.8/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 15:51:45.000000 logmuse-0.2.8/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 15:51:45.000000 logmuse-0.2.8/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 15:51:53.289098 logmuse-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-04 15:51:45.000000 logmuse-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:51:53.289098 logmuse-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-04 15:51:45.000000 logmuse-0.2.8/tests/test_add_logging_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-04 15:51:45.000000 logmuse-0.2.8/tests/test_basic_setup_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-04 15:51:45.000000 logmuse-0.2.8/tests/test_logger_via_cli.py
```

### Comparing `logmuse-0.2.7/LICENSE.txt` & `logmuse-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logmuse-0.2.7/PKG-INFO` & `logmuse-0.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: logmuse
-Version: 0.2.7
+Version: 0.2.8
 Summary: Logging setup
 Home-page: https://github.com/databio/logmuse/
 Author: Vince Reuter, Nathan Sheffield
 License: BSD-2-Clause
-Description: # logmuse
-        
-        [![Build Status](https://travis-ci.org/databio/logmuse.svg?branch=master)](https://travis-ci.org/databio/logmuse)
-        [![Coverage Status](https://coveralls.io/repos/github/vreuter/logmuse/badge.svg?branch=master)](https://coveralls.io/github/vreuter/logmuse?branch=master)
-        
-        Logmuse is a small logging setup package. The point of logmuse is to make it super simple to add CLI-control of logging to your python CLI tool. It just provides a simple interface so that standard arguments can be passed on to the logger.
-        
-        It is only useful for CLI tools.
-        
-        
 Keywords: logging,workflow,logger,logs
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: setuptools
+
+# logmuse
+
+[![Build Status](https://github.com/databio/logmuse/actions/workflows/run-pytest.yml/badge.svg?branch=master)](https://github.com/databio/logmuse/actions/workflows/run-pytest.yml/badge.svg?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/vreuter/logmuse/badge.svg?branch=master)](https://coveralls.io/github/vreuter/logmuse?branch=master)
+
+Logmuse is a small logging setup package. The point of logmuse is to make it super simple to add CLI-control of logging to your python CLI tool. It just provides a simple interface so that standard arguments can be passed on to the logger.
+
+It is only useful for CLI tools.
+
```

### Comparing `logmuse-0.2.7/README.md` & `logmuse-0.2.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # logmuse
 
-[![Build Status](https://travis-ci.org/databio/logmuse.svg?branch=master)](https://travis-ci.org/databio/logmuse)
+[![Build Status](https://github.com/databio/logmuse/actions/workflows/run-pytest.yml/badge.svg?branch=master)](https://github.com/databio/logmuse/actions/workflows/run-pytest.yml/badge.svg?branch=master)
 [![Coverage Status](https://coveralls.io/repos/github/vreuter/logmuse/badge.svg?branch=master)](https://coveralls.io/github/vreuter/logmuse?branch=master)
 
 Logmuse is a small logging setup package. The point of logmuse is to make it super simple to add CLI-control of logging to your python CLI tool. It just provides a simple interface so that standard arguments can be passed on to the logger.
 
 It is only useful for CLI tools.
```

### Comparing `logmuse-0.2.7/logmuse/est.py` & `logmuse-0.2.8/logmuse/est.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,18 +281,20 @@
         handlers.append(logging.StreamHandler(stream_loc))
 
     fine = level <= logging.DEBUG
     get_fmt = (
         (lambda _: fmt)
         if fmt
         else (
-            lambda hdlr: BASIC_LOGGING_FORMAT
-            if plain_format
-            or not (devmode or fine or isinstance(hdlr, logging.FileHandler))
-            else (FULL_DEV_LOGGING_FMT if use_full_names else DEV_LOGGING_FMT)
+            lambda hdlr: (
+                BASIC_LOGGING_FORMAT
+                if plain_format
+                or not (devmode or fine or isinstance(hdlr, logging.FileHandler))
+                else (FULL_DEV_LOGGING_FMT if use_full_names else DEV_LOGGING_FMT)
+            )
         )
     )
 
     fmt_kwargs = {"datefmt": datefmt}
     if style:
         vers = sys.version_info
         if vers < (3, 2):
@@ -325,15 +327,15 @@
     devmode=False,
     verbosity=None,
     fmt=None,
     datefmt=None,
     plain_format=False,
     style=None,
 ):
-    """ Old alias for init_logger for backwards compatibility """
+    """Old alias for init_logger for backwards compatibility"""
     warnings.warn("Please use init_logger in place of setup_logger", DeprecationWarning)
     return init_logger(
         name,
         level,
         stream,
         logfile,
         make_root,
@@ -382,15 +384,15 @@
             "Verbosity must be string or int; got {} ({})".format(
                 verbosity, type(verbosity)
             )
         )
 
 
 class AbsentOptionException(Exception):
-    """ Exception subtype suggesting that client should add log options. """
+    """Exception subtype suggesting that client should add log options."""
 
     def __init__(self, missing_optname):
         likely_reason = (
             "'{}' not in the parsed options; was {} used to "
             "add CLI logging options to an argument parser?".format(
                 missing_optname, "{}.{}".format(__name__, add_logging_options.__name__)
             )
```

### Comparing `logmuse-0.2.7/logmuse.egg-info/PKG-INFO` & `logmuse-0.2.8/logmuse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: logmuse
-Version: 0.2.7
+Version: 0.2.8
 Summary: Logging setup
 Home-page: https://github.com/databio/logmuse/
 Author: Vince Reuter, Nathan Sheffield
 License: BSD-2-Clause
-Description: # logmuse
-        
-        [![Build Status](https://travis-ci.org/databio/logmuse.svg?branch=master)](https://travis-ci.org/databio/logmuse)
-        [![Coverage Status](https://coveralls.io/repos/github/vreuter/logmuse/badge.svg?branch=master)](https://coveralls.io/github/vreuter/logmuse?branch=master)
-        
-        Logmuse is a small logging setup package. The point of logmuse is to make it super simple to add CLI-control of logging to your python CLI tool. It just provides a simple interface so that standard arguments can be passed on to the logger.
-        
-        It is only useful for CLI tools.
-        
-        
 Keywords: logging,workflow,logger,logs
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: setuptools
+
+# logmuse
+
+[![Build Status](https://github.com/databio/logmuse/actions/workflows/run-pytest.yml/badge.svg?branch=master)](https://github.com/databio/logmuse/actions/workflows/run-pytest.yml/badge.svg?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/vreuter/logmuse/badge.svg?branch=master)](https://coveralls.io/github/vreuter/logmuse?branch=master)
+
+Logmuse is a small logging setup package. The point of logmuse is to make it super simple to add CLI-control of logging to your python CLI tool. It just provides a simple interface so that standard arguments can be passed on to the logger.
+
+It is only useful for CLI tools.
+
```

### Comparing `logmuse-0.2.7/setup.py` & `logmuse-0.2.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,52 +5,64 @@
 PKG = "logmuse"
 REQDIR = "requirements"
 
 
 def read_reqs(reqs_name):
     deps = []
     depsfile = os.path.join(REQDIR, "requirements-{}.txt".format(reqs_name))
-    with open(depsfile, 'r') as f:
+    with open(depsfile, "r") as f:
         for l in f:
             if not l.strip():
                 continue
             deps.append(l)
     return deps
 
 
 # Additional keyword arguments for setup().
 extra = {}
 
-extra["install_requires"] = []
+DEPENDENCIES = []
+with open("requirements/requirements-all.txt", "r") as reqs_file:
+    for line in reqs_file:
+        if not line.strip():
+            continue
+        DEPENDENCIES.append(line)
 
-with open(os.path.join(PKG, "_version.py"), 'r') as versionfile:
+extra["install_requires"] = DEPENDENCIES
+
+
+with open(os.path.join(PKG, "_version.py"), "r") as versionfile:
     version = versionfile.readline().split()[-1].strip("\"'\n")
 
 # Handle the pypi README formatting.
-with open('README.md') as f:
+with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name=PKG,
     packages=[PKG],
     version=version,
     description="Logging setup",
     long_description=long_description,
-    long_description_content_type='text/markdown', 
+    long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="logging, workflow, logger, logs",
     url="https://github.com/databio/{}/".format(PKG),
-    author=u"Vince Reuter, Nathan Sheffield",
+    author="Vince Reuter, Nathan Sheffield",
     license="BSD-2-Clause",
     scripts=None,
     include_package_data=True,
     test_suite="tests",
     tests_require=read_reqs("dev"),
-    setup_requires=(["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []),
+    setup_requires=(
+        ["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []
+    ),
     **extra
 )
```

