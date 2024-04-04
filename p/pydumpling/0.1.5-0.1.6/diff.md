# Comparing `tmp/pydumpling-0.1.5.tar.gz` & `tmp/pydumpling-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydumpling-0.1.5.tar", last modified: Wed Mar 20 14:14:43 2024, max compression
+gzip compressed data, was "pydumpling-0.1.6.tar", last modified: Thu Apr  4 10:23:11 2024, max compression
```

## Comparing `pydumpling-0.1.5.tar` & `pydumpling-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1092 2024-03-12 12:59:29.680421 pydumpling-0.1.5/LICENSE
--rw-r--r--   0        0        0     4192 2024-03-13 13:41:04.305909 pydumpling-0.1.5/README.md
--rw-r--r--   0        0        0      382 2024-03-18 12:31:53.436401 pydumpling-0.1.5/pydumpling/__init__.py
--rw-r--r--   0        0        0       30 2024-03-12 12:59:29.680421 pydumpling-0.1.5/pydumpling/__main__.py
--rw-r--r--   0        0        0     1568 2024-03-20 13:56:34.658118 pydumpling-0.1.5/pydumpling/cli.py
--rw-r--r--   0        0        0     1120 2024-03-20 13:56:34.658118 pydumpling-0.1.5/pydumpling/debug_dumpling.py
--rw-r--r--   0        0        0     3574 2024-03-13 13:18:59.875960 pydumpling-0.1.5/pydumpling/fake_types.py
--rw-r--r--   0        0        0      769 2024-03-20 13:56:27.158118 pydumpling-0.1.5/pydumpling/helpers.py
--rw-r--r--   0        0        0     2676 2024-03-20 14:14:31.238125 pydumpling-0.1.5/pydumpling/pydumpling.py
--rw-r--r--   0        0        0     4103 2024-03-13 13:46:36.555896 pydumpling-0.1.5/pydumpling/rpdb.py
--rw-r--r--   0        0        0     1180 2024-03-20 14:14:43.858125 pydumpling-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 12:59:29.680421 pydumpling-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      460 2024-03-12 12:59:29.680421 pydumpling-0.1.5/tests/test_debug.py
--rw-r--r--   0        0        0      419 2024-03-12 12:59:29.680421 pydumpling-0.1.5/tests/test_dump.py
--rw-r--r--   0        0        0     4808 1970-01-01 00:00:00.000000 pydumpling-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-03-12 12:59:29.680421 pydumpling-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4451 2024-04-04 10:06:46.491932 pydumpling-0.1.6/README.md
+-rw-r--r--   0        0        0      482 2024-04-04 09:57:53.202084 pydumpling-0.1.6/pydumpling/__init__.py
+-rw-r--r--   0        0        0       30 2024-03-12 12:59:29.680421 pydumpling-0.1.6/pydumpling/__main__.py
+-rw-r--r--   0        0        0     1569 2024-04-04 09:56:09.962114 pydumpling-0.1.6/pydumpling/cli.py
+-rw-r--r--   0        0        0     1148 2024-04-04 09:56:09.962114 pydumpling-0.1.6/pydumpling/debug_dumpling.py
+-rw-r--r--   0        0        0     3601 2024-04-04 09:56:09.962114 pydumpling-0.1.6/pydumpling/fake_types.py
+-rw-r--r--   0        0        0      770 2024-04-04 09:56:09.962114 pydumpling-0.1.6/pydumpling/helpers.py
+-rw-r--r--   0        0        0     2704 2024-04-04 10:16:54.601755 pydumpling-0.1.6/pydumpling/pydumpling.py
+-rw-r--r--   0        0        0     4104 2024-04-04 09:56:09.962114 pydumpling-0.1.6/pydumpling/rpdb.py
+-rw-r--r--   0        0        0     1180 2024-04-04 10:23:11.511648 pydumpling-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-12 12:59:29.680421 pydumpling-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0      460 2024-03-12 12:59:29.680421 pydumpling-0.1.6/tests/test_debug.py
+-rw-r--r--   0        0        0      419 2024-03-12 12:59:29.680421 pydumpling-0.1.6/tests/test_dump.py
+-rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 pydumpling-0.1.6/PKG-INFO
```

### Comparing `pydumpling-0.1.5/LICENSE` & `pydumpling-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydumpling-0.1.5/README.md` & `pydumpling-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     d = 4
     inner()
 
 ```
 
 ### Save the exception traceback.
 
-In the code, find the place where we need to do the `try ... except ...` and use `save_dumpling()`. When we save the dump file, it will default to `${exception filename}:${error lineno}.dump`.
+In the code, find the place where we need to do the `try ... except ...` and use `save_dumpling()`. When we save the dump file, it will default to `${exception filename}-${error lineno}.dump`.
 
 ```python
 from pydumpling import save_dumping
 
 def inner():
     a = 1
     b = "2"
@@ -156,9 +156,29 @@
 
 #### Use command line to do remote pdb debug:
 `python -m pydumpling --rdebug test.deump`
 It will open the debugger on port 4444, then we can access pdb using telnet、netcat... :
 `nc 127.0.0.1 4444`
 ![alt text](static/rpdb.png)
 
+#### Enable global exception catching:
+```python
+from pydumpling import catch_any_exception
+
+catch_any_exception()
+
+def inner():
+    a = 1
+    b = "2"
+    c = a + b  # noqa: F841
+
+
+def outer():
+    inner()
+    
+if __name__ == "__main__":
+    outer()
+   
+```
+
 ## TODO
 - []
```

### Comparing `pydumpling-0.1.5/pydumpling/cli.py` & `pydumpling-0.1.6/pydumpling/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import os.path
+
 from .debug_dumpling import debug_dumpling, load_dumpling
-from .rpdb import r_post_mortem
 from .helpers import print_traceback_and_except
+from .rpdb import r_post_mortem
 
 DUMP_FILE_EXTENSION: str = ".dump"
 
 
 def validate_file_name(file_name: str) -> str:
     """check file extension name and exists"""
     if not file_name.endswith(DUMP_FILE_EXTENSION):
```

### Comparing `pydumpling-0.1.5/pydumpling/debug_dumpling.py` & `pydumpling-0.1.6/pydumpling/debug_dumpling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 import gzip
+import inspect
 import pdb
-import dill
 import pickle
-from packaging.version import parse
-import inspect
 import types
-from .fake_types import FakeFrame, FakeTraceback, FakeCode
+
+import dill
+from packaging.version import parse
+
+from .fake_types import FakeCode, FakeFrame, FakeTraceback
 
 
 def load_dumpling(filename):
     with gzip.open(filename, "rb") as f:
         try:
             return dill.load(f)
         except Exception:
```

### Comparing `pydumpling-0.1.5/pydumpling/fake_types.py` & `pydumpling-0.1.6/pydumpling/fake_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 import os
 import sys
+
 import dill
 
 
 class FakeType(object):
     @classmethod
     def _safe_repr(cls, v):
         try:
@@ -37,15 +39,15 @@
         if dill is not None:
             try:
                 dill.dumps(v)
                 return v
             except Exception:
                 return cls._safe_repr(v)
         else:
-            from datetime import date, time, datetime, timedelta
+            from datetime import date, datetime, time, timedelta
 
             BUILTIN = (str, unicode, int, long, float, date, time, datetime, timedelta) if sys.version_info.major == 2 \
                 else (str, int, float, date, time, datetime, timedelta)  # noqa: F821
 
             if type(v) in BUILTIN:
                 return v
```

### Comparing `pydumpling-0.1.5/pydumpling/helpers.py` & `pydumpling-0.1.6/pydumpling/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
-from traceback import print_tb, print_exception
+from traceback import print_exception, print_tb
+
 from .pydumpling import save_dumping
 
 
 def print_traceback_and_except(dumpling_result):
     exc_tb = dumpling_result["traceback"]
     except_extra = dumpling_result.get("exc_extra")
     exc_type = except_extra["exc_type"] if except_extra else None
```

### Comparing `pydumpling-0.1.5/pydumpling/pydumpling.py` & `pydumpling-0.1.6/pydumpling/pydumpling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
 import gzip
-import sys
-import dill
+import inspect
 import pickle
+import sys
 import warnings
-import inspect
+
+import dill
+
 from .fake_types import FakeFrame, FakeTraceback
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 
 def save_dumping(filename=None, exc_info=None):
     try:
         if exc_info is None:
             exc_type, exc_value, exc_tb = sys.exc_info()
         else:
```

### Comparing `pydumpling-0.1.5/pydumpling/rpdb.py` & `pydumpling-0.1.6/pydumpling/rpdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pdb
 import socket
-import threading
 import sys
+import threading
+
 from .debug_dumpling import load_dumpling, mock_inspect
 
 DEFAULT_ADDR = "127.0.0.1"
 DEFAULT_PORT = 4444
 
 
 class FileObjectWrapper(object):
```

### Comparing `pydumpling-0.1.5/pyproject.toml` & `pydumpling-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pydumpling"
-version = "0.1.5"
+version = "0.1.6"
 description = "Python post-mortem debugger"
 authors = [
     { name = "cocolato", email = "haiizhu@outlook.com" },
 ]
 dependencies = [
     "dill<1.0.0,>=0.3.2",
     "packaging>=24.0",
```

### Comparing `pydumpling-0.1.5/PKG-INFO` & `pydumpling-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydumpling
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python post-mortem debugger
 Home-page: https://github.com/cocolato/pydumpling
 Author-Email: cocolato <haiizhu@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/cocolato/pydumpling
 Requires-Python: >=3.7
 Requires-Dist: dill<1.0.0,>=0.3.2
@@ -67,15 +67,15 @@
     d = 4
     inner()
 
 ```
 
 ### Save the exception traceback.
 
-In the code, find the place where we need to do the `try ... except ...` and use `save_dumpling()`. When we save the dump file, it will default to `${exception filename}:${error lineno}.dump`.
+In the code, find the place where we need to do the `try ... except ...` and use `save_dumpling()`. When we save the dump file, it will default to `${exception filename}-${error lineno}.dump`.
 
 ```python
 from pydumpling import save_dumping
 
 def inner():
     a = 1
     b = "2"
@@ -174,9 +174,29 @@
 
 #### Use command line to do remote pdb debug:
 `python -m pydumpling --rdebug test.deump`
 It will open the debugger on port 4444, then we can access pdb using telnet、netcat... :
 `nc 127.0.0.1 4444`
 ![alt text](static/rpdb.png)
 
+#### Enable global exception catching:
+```python
+from pydumpling import catch_any_exception
+
+catch_any_exception()
+
+def inner():
+    a = 1
+    b = "2"
+    c = a + b  # noqa: F841
+
+
+def outer():
+    inner()
+    
+if __name__ == "__main__":
+    outer()
+   
+```
+
 ## TODO
 - []
```

