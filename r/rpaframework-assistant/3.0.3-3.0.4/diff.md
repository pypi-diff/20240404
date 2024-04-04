# Comparing `tmp/rpaframework_assistant-3.0.3.tar.gz` & `tmp/rpaframework_assistant-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_assistant-3.0.3.tar", max compression
+gzip compressed data, was "rpaframework_assistant-3.0.4.tar", max compression
```

## Comparing `rpaframework_assistant-3.0.3.tar` & `rpaframework_assistant-3.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11560 2023-12-05 08:21:31.211231 rpaframework_assistant-3.0.3/LICENSE
--rw-r--r--   0        0        0     2412 2024-04-02 12:28:54.963905 rpaframework_assistant-3.0.3/pyproject.toml
--rw-r--r--   0        0        0      296 2023-12-05 08:21:31.212234 rpaframework_assistant-3.0.3/README.rst
--rw-r--r--   0        0        0    86080 2024-04-02 12:30:04.841860 rpaframework_assistant-3.0.3/RPA_Assistant.libspec
--rw-r--r--   0        0        0       96 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.3/src/RPA/Assistant/__init__.py
--rw-r--r--   0        0        0     3498 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.3/src/RPA/Assistant/background_flet.py
--rw-r--r--   0        0        0     5304 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.3/src/RPA/Assistant/callback_runner.py
--rw-r--r--   0        0        0    12305 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.3/src/RPA/Assistant/flet_client.py
--rw-r--r--   0        0        0    74890 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.3/src/RPA/Assistant/library.py
--rw-r--r--   0        0        0     1597 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.3/src/RPA/Assistant/types.py
--rw-r--r--   0        0        0     3765 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.3/src/RPA/Assistant/utils.py
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 rpaframework_assistant-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11560 2023-12-05 08:21:31.211231 rpaframework_assistant-3.0.4/LICENSE
+-rw-r--r--   0        0        0     2423 2024-04-04 12:48:45.711508 rpaframework_assistant-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0      296 2023-12-05 08:21:31.212234 rpaframework_assistant-3.0.4/README.rst
+-rw-r--r--   0        0        0    86080 2024-04-04 12:50:14.764812 rpaframework_assistant-3.0.4/RPA_Assistant.libspec
+-rw-r--r--   0        0        0       96 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.4/src/RPA/Assistant/__init__.py
+-rw-r--r--   0        0        0     3498 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.4/src/RPA/Assistant/background_flet.py
+-rw-r--r--   0        0        0     5304 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.4/src/RPA/Assistant/callback_runner.py
+-rw-r--r--   0        0        0    12305 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.4/src/RPA/Assistant/flet_client.py
+-rw-r--r--   0        0        0    74890 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.4/src/RPA/Assistant/library.py
+-rw-r--r--   0        0        0     1597 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.4/src/RPA/Assistant/types.py
+-rw-r--r--   0        0        0     3765 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.4/src/RPA/Assistant/utils.py
+-rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 rpaframework_assistant-3.0.4/PKG-INFO
```

### Comparing `rpaframework_assistant-3.0.3/LICENSE` & `rpaframework_assistant-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-3.0.3/pyproject.toml` & `rpaframework_assistant-3.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpaframework-assistant"
-version = "3.0.3"
+version = "3.0.4"
 description = "Interactive UI library for RPA Framework"
 authors = ["RPA Framework <rpafw@robocorp.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 
 homepage = "https://rpaframework.org/"
 documentation = "https://rpaframework.org/"
@@ -31,15 +31,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 robotframework = ">=4.0.0,!=4.0.1,!=6.1.0,<7.0.0"
 # Flet needs `packaging>=23`. Earlier rpaframework-core versions don't allow
 # installing it. This make resolution errors simpler and faster.
 rpaframework-core = "^11.3.1"
-flet="0.4.2"
+robocorp-flet="0.4.2.1"
 # We only need the Literal type on python 3.7 from the module, but it has to be
 # installed on all pythons so the imports work
 typing-extensions = { version = "^4.4.0" }
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
```

### Comparing `rpaframework_assistant-3.0.3/RPA_Assistant.libspec` & `rpaframework_assistant-3.0.4/RPA_Assistant.libspec`

 * *Files 0% similar despite different names*

#### Comparing `rpaframework_assistant-3.0.3/RPA_Assistant.libspec` & `rpaframework_assistant-3.0.4/RPA_Assistant.libspec`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="RPA.Assistant" type="LIBRARY" format="REST" scope="GLOBAL" generated="2024-04-02T12:30:05+00:00" specversion="5" source="./RPA/Assistant/library.py" lineno="58">
+<keywordspec name="RPA.Assistant" type="LIBRARY" format="REST" scope="GLOBAL" generated="2024-04-04T12:50:15+00:00" specversion="5" source="./RPA/Assistant/library.py" lineno="58">
   <version/>
   <doc>The `Assistant` library provides a way to display information to a user
 and request input while a robot is running. It allows building processes
 that require human interaction. Also it offers capabilities of running
 other robots inside the current one and determine what to display to the
 user based on his previous responses.
```

### Comparing `rpaframework_assistant-3.0.3/src/RPA/Assistant/background_flet.py` & `rpaframework_assistant-3.0.4/src/RPA/Assistant/background_flet.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-3.0.3/src/RPA/Assistant/callback_runner.py` & `rpaframework_assistant-3.0.4/src/RPA/Assistant/callback_runner.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-3.0.3/src/RPA/Assistant/flet_client.py` & `rpaframework_assistant-3.0.4/src/RPA/Assistant/flet_client.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-3.0.3/src/RPA/Assistant/library.py` & `rpaframework_assistant-3.0.4/src/RPA/Assistant/library.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-3.0.3/src/RPA/Assistant/types.py` & `rpaframework_assistant-3.0.4/src/RPA/Assistant/types.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-3.0.3/src/RPA/Assistant/utils.py` & `rpaframework_assistant-3.0.4/src/RPA/Assistant/utils.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-3.0.3/PKG-INFO` & `rpaframework_assistant-3.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-assistant
-Version: 3.0.3
+Version: 3.0.4
 Summary: Interactive UI library for RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,dialogs,assistant
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.8,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: flet (==0.4.2)
+Requires-Dist: robocorp-flet (==0.4.2.1)
 Requires-Dist: robotframework (>=4.0.0,!=4.0.1,!=6.1.0,<7.0.0)
 Requires-Dist: rpaframework-core (>=11.3.1,<12.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://rpaframework.org/
 Project-URL: Repository, https://github.com/robocorp/rpaframework
 Description-Content-Type: text/x-rst
```

