# Comparing `tmp/FastWARC-0.8.1.tar.gz` & `tmp/FastWARC-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastWARC-0.8.1.tar", last modified: Fri Dec  3 17:42:22 2021, max compression
+gzip compressed data, was "FastWARC-0.9.0.tar", last modified: Mon Dec  6 13:52:58 2021, max compression
```

## Comparing `FastWARC-0.8.1.tar` & `FastWARC-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 17:42:22.252526 FastWARC-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 17:42:22.244526 FastWARC-0.8.1/FastWARC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-12-03 17:42:22.000000 FastWARC-0.8.1/FastWARC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-12-03 17:42:22.000000 FastWARC-0.8.1/FastWARC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-03 17:42:22.000000 FastWARC-0.8.1/FastWARC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-03 17:42:22.000000 FastWARC-0.8.1/FastWARC.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-03 17:42:22.000000 FastWARC-0.8.1/FastWARC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-12-03 17:42:22.000000 FastWARC-0.8.1/FastWARC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-12-03 17:42:22.252526 FastWARC-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2021-12-03 17:42:09.000000 FastWARC-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 17:42:22.248525 FastWARC-0.8.1/fastwarc/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2021-12-03 17:42:09.000000 FastWARC-0.8.1/fastwarc/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      750 2021-12-03 17:42:09.000000 FastWARC-0.8.1/fastwarc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19061 2021-12-03 17:42:09.000000 FastWARC-0.8.1/fastwarc/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)   704891 2021-12-03 17:42:19.000000 FastWARC-0.8.1/fastwarc/stream_io.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4268 2021-12-03 17:42:09.000000 FastWARC-0.8.1/fastwarc/stream_io.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    32659 2021-12-03 17:42:09.000000 FastWARC-0.8.1/fastwarc/stream_io.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   567433 2021-12-03 17:42:19.000000 FastWARC-0.8.1/fastwarc/tools.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6787 2021-12-03 17:42:09.000000 FastWARC-0.8.1/fastwarc/tools.pyx
--rw-r--r--   0 runner    (1001) docker     (121)  1291735 2021-12-03 17:42:20.000000 FastWARC-0.8.1/fastwarc/warc.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2021-12-03 17:42:09.000000 FastWARC-0.8.1/fastwarc/warc.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    41445 2021-12-03 17:42:09.000000 FastWARC-0.8.1/fastwarc/warc.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      153 2021-12-03 17:42:09.000000 FastWARC-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 17:42:22.248525 FastWARC-0.8.1/resiliparse_common/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_common/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2510 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_common/string_util.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-03 17:42:22.252526 FastWARC-0.8.1/resiliparse_inc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/algorithm.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      338 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/atomic.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/boost_regex.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/cctype.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/cstdlib.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/cstring.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/dlfcn.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/errno.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    31603 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/lexbor.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/lz4frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/lz4hc.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/pthread.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     7365 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/re2.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/stdio.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/string_view.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/time.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      390 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/uchardet.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/unistd.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/utility.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2021-12-03 17:42:09.000000 FastWARC-0.8.1/resiliparse_inc/zlib.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-03 17:42:22.252526 FastWARC-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4326 2021-12-03 17:42:09.000000 FastWARC-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 13:52:58.376367 FastWARC-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 13:52:58.360366 FastWARC-0.9.0/FastWARC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-12-06 13:52:58.000000 FastWARC-0.9.0/FastWARC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-12-06 13:52:58.000000 FastWARC-0.9.0/FastWARC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-06 13:52:58.000000 FastWARC-0.9.0/FastWARC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-06 13:52:58.000000 FastWARC-0.9.0/FastWARC.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-06 13:52:58.000000 FastWARC-0.9.0/FastWARC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-12-06 13:52:58.000000 FastWARC-0.9.0/FastWARC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-12-06 13:52:58.376367 FastWARC-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1818 2021-12-06 13:52:44.000000 FastWARC-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 13:52:58.364367 FastWARC-0.9.0/fastwarc/
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2021-12-06 13:52:44.000000 FastWARC-0.9.0/fastwarc/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2021-12-06 13:52:44.000000 FastWARC-0.9.0/fastwarc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19061 2021-12-06 13:52:44.000000 FastWARC-0.9.0/fastwarc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)   709579 2021-12-06 13:52:55.000000 FastWARC-0.9.0/fastwarc/stream_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4268 2021-12-06 13:52:44.000000 FastWARC-0.9.0/fastwarc/stream_io.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    32659 2021-12-06 13:52:44.000000 FastWARC-0.9.0/fastwarc/stream_io.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)   571968 2021-12-06 13:52:55.000000 FastWARC-0.9.0/fastwarc/tools.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6787 2021-12-06 13:52:44.000000 FastWARC-0.9.0/fastwarc/tools.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)  1293393 2021-12-06 13:52:56.000000 FastWARC-0.9.0/fastwarc/warc.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3526 2021-12-06 13:52:44.000000 FastWARC-0.9.0/fastwarc/warc.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    41445 2021-12-06 13:52:44.000000 FastWARC-0.9.0/fastwarc/warc.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2021-12-06 13:52:44.000000 FastWARC-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 13:52:58.368367 FastWARC-0.9.0/resiliparse_common/
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_common/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2524 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_common/string_util.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 13:52:58.376367 FastWARC-0.9.0/resiliparse_inc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/algorithm.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/atomic.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4743 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/boost_regex.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/cctype.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/cstdlib.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/cstring.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/dlfcn.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/errno.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    31974 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/lexbor.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/lz4frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/lz4hc.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/pthread.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     7365 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/re2.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/stdio.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/string_view.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/time.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/uchardet.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/unistd.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/utility.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1189 2021-12-06 13:52:44.000000 FastWARC-0.9.0/resiliparse_inc/zlib.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-06 13:52:58.376367 FastWARC-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4326 2021-12-06 13:52:44.000000 FastWARC-0.9.0/setup.py
```

### Comparing `FastWARC-0.8.1/FastWARC.egg-info/PKG-INFO` & `FastWARC-0.9.0/FastWARC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastWARC
-Version: 0.8.1
+Version: 0.9.0
 Summary: A high-performance WARC parsing library for Python written in C++/Cython.
 Home-page: https://github.com/chatnoir-eu/chatnoir-resiliparse
 Author: Janek Bevendorff
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `FastWARC-0.8.1/FastWARC.egg-info/SOURCES.txt` & `FastWARC-0.9.0/FastWARC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/PKG-INFO` & `FastWARC-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastWARC
-Version: 0.8.1
+Version: 0.9.0
 Summary: A high-performance WARC parsing library for Python written in C++/Cython.
 Home-page: https://github.com/chatnoir-eu/chatnoir-resiliparse
 Author: Janek Bevendorff
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `FastWARC-0.8.1/README.md` & `FastWARC-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/fastwarc/__init__.pxd` & `FastWARC-0.9.0/fastwarc/__init__.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/fastwarc/__init__.py` & `FastWARC-0.9.0/fastwarc/__init__.py`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/fastwarc/cli.py` & `FastWARC-0.9.0/fastwarc/cli.py`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/fastwarc/stream_io.cpp` & `FastWARC-0.9.0/fastwarc/stream_io.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.25 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-std=c++17",
@@ -35,16 +35,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_25"
+#define CYTHON_HEX_VERSION 0x001D19F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -183,15 +183,15 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -202,15 +202,15 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -221,15 +221,17 @@
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -352,17 +354,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -592,18 +653,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -764,14 +825,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -1341,21 +1403,23 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -13079,14 +13143,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_9stream_io_PythonIOStreamAdapter __pyx_vtable_8fastwarc_9stream_io_PythonIOStreamAdapter;
 
 static PyObject *__pyx_tp_new_8fastwarc_9stream_io_PythonIOStreamAdapter(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_8fastwarc_9stream_io_PythonIOStreamAdapter *p;
   PyObject *o = __pyx_tp_new_8fastwarc_9stream_io_IOStream(t, a, k);
   if (unlikely(!o)) return 0;
@@ -13203,14 +13270,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_9stream_io_BytesIOStream __pyx_vtable_8fastwarc_9stream_io_BytesIOStream;
 
 static PyObject *__pyx_tp_new_8fastwarc_9stream_io_BytesIOStream(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_8fastwarc_9stream_io_BytesIOStream *p;
   PyObject *o = __pyx_tp_new_8fastwarc_9stream_io_IOStream(t, a, k);
   if (unlikely(!o)) return 0;
@@ -13302,14 +13372,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_9stream_io_FileStream __pyx_vtable_8fastwarc_9stream_io_FileStream;
 
 static PyObject *__pyx_tp_new_8fastwarc_9stream_io_FileStream(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_8fastwarc_9stream_io_FileStream *p;
   PyObject *o = __pyx_tp_new_8fastwarc_9stream_io_IOStream(t, a, k);
   if (unlikely(!o)) return 0;
@@ -13406,14 +13479,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_9stream_io_CompressingStream __pyx_vtable_8fastwarc_9stream_io_CompressingStream;
 
 static PyObject *__pyx_tp_new_8fastwarc_9stream_io_CompressingStream(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_8fastwarc_9stream_io_CompressingStream *p;
   PyObject *o = __pyx_tp_new_8fastwarc_9stream_io_IOStream(t, a, k);
   if (unlikely(!o)) return 0;
@@ -13485,14 +13561,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_9stream_io_GZipStream __pyx_vtable_8fastwarc_9stream_io_GZipStream;
 
 static PyObject *__pyx_tp_new_8fastwarc_9stream_io_GZipStream(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_8fastwarc_9stream_io_GZipStream *p;
   PyObject *o = __pyx_tp_new_8fastwarc_9stream_io_CompressingStream(t, a, k);
   if (unlikely(!o)) return 0;
@@ -13619,14 +13698,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_9stream_io_LZ4Stream __pyx_vtable_8fastwarc_9stream_io_LZ4Stream;
 
 static PyObject *__pyx_tp_new_8fastwarc_9stream_io_LZ4Stream(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_8fastwarc_9stream_io_LZ4Stream *p;
   PyObject *o = __pyx_tp_new_8fastwarc_9stream_io_CompressingStream(t, a, k);
   if (unlikely(!o)) return 0;
@@ -13753,14 +13835,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_9stream_io_BufferedReader __pyx_vtable_8fastwarc_9stream_io_BufferedReader;
 
 static PyObject *__pyx_tp_new_8fastwarc_9stream_io_BufferedReader(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_8fastwarc_9stream_io_BufferedReader *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -13889,14 +13974,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"wrap_stream", (PyCFunction)__pyx_pw_8fastwarc_9stream_io_13wrap_stream, METH_O, __pyx_doc_8fastwarc_9stream_io_12wrap_stream},
   {0, 0, 0, 0}
 };
 
@@ -16144,15 +16232,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -16241,38 +16329,39 @@
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -16283,19 +16372,24 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
@@ -17565,14 +17659,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `FastWARC-0.8.1/fastwarc/stream_io.pxd` & `FastWARC-0.9.0/fastwarc/stream_io.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/fastwarc/stream_io.pyx` & `FastWARC-0.9.0/fastwarc/stream_io.pyx`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/fastwarc/tools.cpp` & `FastWARC-0.9.0/fastwarc/tools.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.25 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-std=c++17",
@@ -31,16 +31,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_25"
+#define CYTHON_HEX_VERSION 0x001D19F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -179,15 +179,15 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -198,15 +198,15 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -217,15 +217,17 @@
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -348,17 +350,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -588,18 +649,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -760,14 +821,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -1616,21 +1678,23 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -7164,14 +7228,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static struct __pyx_obj_8fastwarc_5tools___pyx_scope_struct_1_verify_digests *__pyx_freelist_8fastwarc_5tools___pyx_scope_struct_1_verify_digests[8];
 static int __pyx_freecount_8fastwarc_5tools___pyx_scope_struct_1_verify_digests = 0;
 
 static PyObject *__pyx_tp_new_8fastwarc_5tools___pyx_scope_struct_1_verify_digests(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -7286,14 +7353,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static PyObject *__pyx_tp_new___Pyx_EnumMeta(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&PyType_Type)->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
@@ -7415,14 +7485,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -10978,14 +11051,17 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030B00A2
+    0,
+#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -11169,15 +11245,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -11266,38 +11342,39 @@
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -11308,19 +11385,24 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
@@ -12687,17 +12769,21 @@
     exc_state = &self->gi_exc_state;
     if (exc_state->exc_type) {
         #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
         #else
         if (exc_state->exc_traceback) {
             PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
             PyFrameObject *f = tb->tb_frame;
-            Py_XINCREF(tstate->frame);
             assert(f->f_back == NULL);
+            #if PY_VERSION_HEX >= 0x030B00A1
+            f->f_back = PyThreadState_GetFrame(tstate);
+            #else
+            Py_XINCREF(tstate->frame);
             f->f_back = tstate->frame;
+            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -13483,14 +13569,17 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030B00A2
+    0,
+#endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
@@ -13758,14 +13847,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `FastWARC-0.8.1/fastwarc/tools.pyx` & `FastWARC-0.9.0/fastwarc/tools.pyx`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/fastwarc/warc.cpp` & `FastWARC-0.9.0/fastwarc/warc.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.25 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-std=c++17",
@@ -31,16 +31,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_25"
+#define CYTHON_HEX_VERSION 0x001D19F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -179,15 +179,15 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -198,15 +198,15 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
@@ -217,15 +217,17 @@
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -348,17 +350,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -588,18 +649,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -773,14 +834,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -1629,21 +1691,23 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -19552,117 +19616,14 @@
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "resiliparse_common/string_util.pxd":43
- * 
- * 
- * cdef inline string lstrip_str(const string& s) nogil:             # <<<<<<<<<<<<<<
- *     """Strip leading white space from a C++ string."""
- *     cdef const char* start = s.data()
- */
-
-static CYTHON_INLINE std::string __pyx_f_18resiliparse_common_11string_util_lstrip_str(std::string const &__pyx_v_s) {
-  char const *__pyx_v_start;
-  size_t __pyx_v_l;
-  std::string __pyx_r;
-  int __pyx_t_1;
-  std::string __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-
-  /* "resiliparse_common/string_util.pxd":45
- * cdef inline string lstrip_str(const string& s) nogil:
- *     """Strip leading white space from a C++ string."""
- *     cdef const char* start = s.data()             # <<<<<<<<<<<<<<
- *     cdef size_t l = lstrip_c_str(&start, s.size())
- *     if start == s.data():
- */
-  __pyx_v_start = __pyx_v_s.data();
-
-  /* "resiliparse_common/string_util.pxd":46
- *     """Strip leading white space from a C++ string."""
- *     cdef const char* start = s.data()
- *     cdef size_t l = lstrip_c_str(&start, s.size())             # <<<<<<<<<<<<<<
- *     if start == s.data():
- *         return s
- */
-  __pyx_v_l = __pyx_f_18resiliparse_common_11string_util_lstrip_c_str((&__pyx_v_start), __pyx_v_s.size());
-
-  /* "resiliparse_common/string_util.pxd":47
- *     cdef const char* start = s.data()
- *     cdef size_t l = lstrip_c_str(&start, s.size())
- *     if start == s.data():             # <<<<<<<<<<<<<<
- *         return s
- *     return string(start, l)
- */
-  __pyx_t_1 = ((__pyx_v_start == __pyx_v_s.data()) != 0);
-  if (__pyx_t_1) {
-
-    /* "resiliparse_common/string_util.pxd":48
- *     cdef size_t l = lstrip_c_str(&start, s.size())
- *     if start == s.data():
- *         return s             # <<<<<<<<<<<<<<
- *     return string(start, l)
- * 
- */
-    __pyx_r = __pyx_v_s;
-    goto __pyx_L0;
-
-    /* "resiliparse_common/string_util.pxd":47
- *     cdef const char* start = s.data()
- *     cdef size_t l = lstrip_c_str(&start, s.size())
- *     if start == s.data():             # <<<<<<<<<<<<<<
- *         return s
- *     return string(start, l)
- */
-  }
-
-  /* "resiliparse_common/string_util.pxd":49
- *     if start == s.data():
- *         return s
- *     return string(start, l)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  try {
-    __pyx_t_2 = std::string(__pyx_v_start, __pyx_v_l);
-  } catch(...) {
-    #ifdef WITH_THREAD
-    PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
-    #endif
-    __Pyx_CppExn2PyErr();
-    #ifdef WITH_THREAD
-    __Pyx_PyGILState_Release(__pyx_gilstate_save);
-    #endif
-    __PYX_ERR(2, 49, __pyx_L1_error)
-  }
-  __pyx_r = __pyx_t_2;
-  goto __pyx_L0;
-
-  /* "resiliparse_common/string_util.pxd":43
- * 
- * 
- * cdef inline string lstrip_str(const string& s) nogil:             # <<<<<<<<<<<<<<
- *     """Strip leading white space from a C++ string."""
- *     cdef const char* start = s.data()
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_WriteUnraisable("resiliparse_common.string_util.lstrip_str", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 /* "resiliparse_common/string_util.pxd":52
  * 
  * 
  * cdef inline string rstrip_str(const string& s) nogil:             # <<<<<<<<<<<<<<
  *     """Strip leading white space from a C++ string."""
  *     cdef const char* start = s.data()
  */
@@ -22046,14 +22007,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_4warc_WarcRecord __pyx_vtable_8fastwarc_4warc_WarcRecord;
 
 static PyObject *__pyx_tp_new_8fastwarc_4warc_WarcRecord(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_8fastwarc_4warc_WarcRecord *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -22274,14 +22238,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 static struct __pyx_vtabstruct_8fastwarc_4warc_ArchiveIterator __pyx_vtable_8fastwarc_4warc_ArchiveIterator;
 
 static PyObject *__pyx_tp_new_8fastwarc_4warc_ArchiveIterator(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_8fastwarc_4warc_ArchiveIterator *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -22424,14 +22391,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static struct __pyx_obj_8fastwarc_4warc___pyx_scope_struct____iter__ *__pyx_freelist_8fastwarc_4warc___pyx_scope_struct____iter__[8];
 static int __pyx_freecount_8fastwarc_4warc___pyx_scope_struct____iter__ = 0;
 
 static PyObject *__pyx_tp_new_8fastwarc_4warc___pyx_scope_struct____iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -22534,14 +22504,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static struct __pyx_obj_8fastwarc_4warc___pyx_scope_struct_1_genexpr *__pyx_freelist_8fastwarc_4warc___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_8fastwarc_4warc___pyx_scope_struct_1_genexpr = 0;
 
 static PyObject *__pyx_tp_new_8fastwarc_4warc___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_8fastwarc_4warc___pyx_scope_struct_1_genexpr *p;
@@ -22648,14 +22621,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static struct __pyx_obj_8fastwarc_4warc___pyx_scope_struct_2___iter__ *__pyx_freelist_8fastwarc_4warc___pyx_scope_struct_2___iter__[8];
 static int __pyx_freecount_8fastwarc_4warc___pyx_scope_struct_2___iter__ = 0;
 
 static PyObject *__pyx_tp_new_8fastwarc_4warc___pyx_scope_struct_2___iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -22754,14 +22730,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static PyObject *__pyx_tp_new___Pyx_EnumMeta(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&PyType_Type)->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
@@ -22883,14 +22862,17 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030B00A2
+  0, /*tp_inline_values_offset*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"is_warc_10", (PyCFunction)__pyx_pw_8fastwarc_4warc_5is_warc_10, METH_O, __pyx_doc_8fastwarc_4warc_4is_warc_10},
   {"is_warc_11", (PyCFunction)__pyx_pw_8fastwarc_4warc_7is_warc_11, METH_O, __pyx_doc_8fastwarc_4warc_6is_warc_11},
   {"has_block_digest", (PyCFunction)__pyx_pw_8fastwarc_4warc_9has_block_digest, METH_O, __pyx_doc_8fastwarc_4warc_8has_block_digest},
   {"has_payload_digest", (PyCFunction)__pyx_pw_8fastwarc_4warc_11has_payload_digest, METH_O, __pyx_doc_8fastwarc_4warc_10has_payload_digest},
@@ -27005,17 +26987,21 @@
     exc_state = &self->gi_exc_state;
     if (exc_state->exc_type) {
         #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
         #else
         if (exc_state->exc_traceback) {
             PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
             PyFrameObject *f = tb->tb_frame;
-            Py_XINCREF(tstate->frame);
             assert(f->f_back == NULL);
+            #if PY_VERSION_HEX >= 0x030B00A1
+            f->f_back = PyThreadState_GetFrame(tstate);
+            #else
+            Py_XINCREF(tstate->frame);
             f->f_back = tstate->frame;
+            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -27841,14 +27827,17 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030B00A2
+    0,
+#endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
@@ -29130,14 +29119,17 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030B00A2
+    0,
+#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -29342,15 +29334,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -29439,38 +29431,39 @@
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -29481,19 +29474,24 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
@@ -31052,14 +31050,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `FastWARC-0.8.1/fastwarc/warc.pxd` & `FastWARC-0.9.0/fastwarc/warc.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/fastwarc/warc.pyx` & `FastWARC-0.9.0/fastwarc/warc.pyx`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/resiliparse_common/__init__.pxd` & `FastWARC-0.9.0/resiliparse_common/__init__.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/resiliparse_common/string_util.pxd` & `FastWARC-0.9.0/resiliparse_common/string_util.pxd`

 * *Files 5% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 
 
 cdef inline size_t strip_c_str(const char** s_ptr, size_t l) nogil:
     """Strip leading and trailing white space from a C string."""
     return rstrip_c_str(s_ptr, lstrip_c_str(s_ptr, l))
 
 
-cdef inline string lstrip_str(const string& s) nogil:
-    """Strip leading white space from a C++ string."""
-    cdef const char* start = s.data()
-    cdef size_t l = lstrip_c_str(&start, s.size())
-    if start == s.data():
-        return s
-    return string(start, l)
+# cdef inline string lstrip_str(const string& s) nogil:
+#     """Strip leading white space from a C++ string."""
+#     cdef const char* start = s.data()
+#     cdef size_t l = lstrip_c_str(&start, s.size())
+#     if start == s.data():
+#         return s
+#     return string(start, l)
 
 
 cdef inline string rstrip_str(const string& s) nogil:
     """Strip leading white space from a C++ string."""
     cdef const char* start = s.data()
     cdef size_t l = rstrip_c_str(&start, s.size())
     if l == s.size():
```

### Comparing `FastWARC-0.8.1/resiliparse_inc/boost_regex.pxd` & `FastWARC-0.9.0/resiliparse_inc/boost_regex.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/resiliparse_inc/lexbor.pxd` & `FastWARC-0.9.0/resiliparse_inc/lexbor.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -397,20 +397,26 @@
     size_t lxb_dom_collection_length_noi(lxb_dom_collection_t *col)
 
     lxb_dom_element_t * lxb_dom_collection_element_noi(lxb_dom_collection_t *col, size_t idx)
     lxb_dom_collection_t * lxb_dom_collection_destroy(lxb_dom_collection_t *col, bint self_destroy)
 
 
 cdef extern from "<lexbor/css/css.h>" nogil:
-    ctypedef struct lxb_css_parser_t
+    ctypedef struct lxb_css_log_t
     ctypedef struct lxb_css_syntax_tokenizer_t
+    ctypedef struct lxb_css_parser_t:
+        lxb_css_log_t *log
+        lxb_status_t status
+    ctypedef lxb_status_t (*lexbor_serialize_cb_f)(const lxb_char_t *data, size_t len, void *ctx)
 
     lxb_css_parser_t * lxb_css_parser_create()
     lxb_status_t lxb_css_parser_init(lxb_css_parser_t *parser, lxb_css_syntax_tokenizer_t *tkz, lexbor_mraw_t *mraw)
     lxb_css_parser_t * lxb_css_parser_destroy(lxb_css_parser_t *parser, bint self_destroy)
+    lxb_status_t lxb_css_log_serialize(lxb_css_log_t *log, lexbor_serialize_cb_f cb, void *ctx,
+                                       const lxb_char_t *indent, size_t indent_length)
 
 
 cdef extern from "<lexbor/tag/tag.h>" nogil:
     ctypedef enum lxb_tag_id_enum_t:
         LXB_TAG__UNDEF = 0x0000
         LXB_TAG__END_OF_FILE = 0x0001
         LXB_TAG__TEXT = 0x0002
```

### Comparing `FastWARC-0.8.1/resiliparse_inc/lz4frame.pxd` & `FastWARC-0.9.0/resiliparse_inc/lz4frame.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/resiliparse_inc/re2.pxd` & `FastWARC-0.9.0/resiliparse_inc/re2.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/resiliparse_inc/string_view.pxd` & `FastWARC-0.9.0/resiliparse_inc/string_view.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/resiliparse_inc/utility.pxd` & `FastWARC-0.9.0/resiliparse_inc/utility.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/resiliparse_inc/zlib.pxd` & `FastWARC-0.9.0/resiliparse_inc/zlib.pxd`

 * *Files identical despite different names*

### Comparing `FastWARC-0.8.1/setup.py` & `FastWARC-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import distutils.ccompiler
 from distutils.dir_util import copy_tree
 from setuptools import find_packages, setup, Extension
 
 
 # 1. BOILERPLATE -------------------------------------------------------
 
-VERSION = '0.8.1'
+VERSION = '0.9.0'
 ROOT_DIRECTORY = os.path.abspath(os.path.dirname(__file__))
 CXX = distutils.ccompiler.get_default_compiler()
 
 TRACE = bool(int(os.getenv('TRACE', 0)))
 DEBUG = bool(int(os.getenv('DEBUG', 0))) or TRACE
 ASAN = bool(int(os.getenv('ASAN', 0)))
```

