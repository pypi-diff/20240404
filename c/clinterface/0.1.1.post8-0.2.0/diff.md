# Comparing `tmp/clinterface-0.1.1.post8-py3-none-any.whl.zip` & `tmp/clinterface-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 11350 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-13 20:41 clinterface/__init__.py
--rw-r--r--  2.0 unx      940 b- defN 19-Dec-23 05:52 clinterface/charDef.py
--rw-r--r--  2.0 unx      881 b- defN 22-Nov-13 20:08 clinterface/colors.py
--rw-r--r--  2.0 unx     1199 b- defN 19-Dec-23 05:52 clinterface/cursor.py
--rw-r--r--  2.0 unx     1384 b- defN 19-Dec-23 05:52 clinterface/keyhandler.py
--rw-r--r--  2.0 unx     1296 b- defN 22-Nov-15 03:26 clinterface/messages.py
--rw-r--r--  2.0 unx    13519 b- defN 22-Nov-14 02:34 clinterface/prompts.py
--rw-r--r--  2.0 unx     3088 b- defN 19-Dec-23 06:02 clinterface/utils.py
--rw-r--r--  2.0 unx     7652 b- defN 22-Nov-15 03:26 clinterface-0.1.1.post8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2003 b- defN 22-Nov-15 03:26 clinterface-0.1.1.post8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-15 03:26 clinterface-0.1.1.post8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 22-Nov-15 03:26 clinterface-0.1.1.post8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1065 b- defN 22-Nov-15 03:26 clinterface-0.1.1.post8.dist-info/RECORD
-13 files, 33131 bytes uncompressed, 9568 bytes compressed:  71.1%
+Zip file size: 11282 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       21 b- defN 24-Mar-11 02:40 clinterface/__init__.py
+-rw-r--r--  2.0 unx      940 b- defN 24-Mar-10 23:24 clinterface/charDef.py
+-rw-r--r--  2.0 unx      881 b- defN 24-Mar-10 23:24 clinterface/colors.py
+-rw-r--r--  2.0 unx     1199 b- defN 24-Mar-10 23:24 clinterface/cursor.py
+-rw-r--r--  2.0 unx     1384 b- defN 24-Mar-10 23:24 clinterface/keyhandler.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Mar-11 02:40 clinterface/messages.py
+-rw-r--r--  2.0 unx    13507 b- defN 24-Mar-11 02:40 clinterface/prompts.py
+-rw-r--r--  2.0 unx     3196 b- defN 24-Mar-11 02:40 clinterface/utils.py
+-rw-r--r--  2.0 unx     7652 b- defN 24-Apr-04 01:57 clinterface-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1997 b- defN 24-Apr-04 01:57 clinterface-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 01:57 clinterface-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-04 01:57 clinterface-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1036 b- defN 24-Apr-04 01:57 clinterface-0.2.0.dist-info/RECORD
+13 files, 32928 bytes uncompressed, 9560 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: clinterface/prompts.py
 Comment: 
 
 Filename: clinterface/utils.py
 Comment: 
 
-Filename: clinterface-0.1.1.post8.dist-info/LICENSE
+Filename: clinterface-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: clinterface-0.1.1.post8.dist-info/METADATA
+Filename: clinterface-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: clinterface-0.1.1.post8.dist-info/WHEEL
+Filename: clinterface-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: clinterface-0.1.1.post8.dist-info/top_level.txt
+Filename: clinterface-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: clinterface-0.1.1.post8.dist-info/RECORD
+Filename: clinterface-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clinterface/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 7574 696c 7320 696d 706f  from .utils impo
+00000010: 7274 205f 0a                             rt _.
```

## clinterface/messages.py

```diff
@@ -1,44 +1,31 @@
 import sys
+from string import Template
 from .colors import DEFAULT, GREEN, YELLOW, RED
 
-def join_args(f):
-    def wrapper(*args, **kwargs):
-        return f(' '.join(args), ', '.join('{}={}'.format(k, v) for k, v in kwargs.items()))
-    return wrapper
-
-@join_args
-def success(message, details):
+def success(message, details=None):
     if details:
-        formatted_message = '{} ({})'.format(message, details)
+        print(GREEN + "{} ({})".format(message, details) + DEFAULT)
     else:
-        formatted_message = message
-    print(GREEN + formatted_message + DEFAULT)
+        print(GREEN + message + DEFAULT)
 
-@join_args
-def warning(message, details):
+def failure(message, details=None):
     if details:
-        formatted_message = 'Warning: {} ({})'.format(message, details)
+        print(RED + "{} ({})".format(message, details) + DEFAULT)
     else:
-        formatted_message = 'Warning: {}'.format(message)
-    print(YELLOW + formatted_message + DEFAULT)
+        print(RED + message + DEFAULT)
 
-@join_args
-def failure(message, details):
+def warning(message, details=None):
     if details:
-        formatted_message = '{} ({})'.format(message, details)
+        print(YELLOW + "Warning: {} ({})".format(message, details) + DEFAULT)
     else:
-        formatted_message = message
-    print(RED + formatted_message + DEFAULT)
+        print(YELLOW + 'Warning: {}'.format(message) + DEFAULT)
 
-@join_args
-def error(message, details):
+def error(message, details=None):
     if details:
-        formatted_message = '{} ({})'.format(message, details)
+        raise SystemExit(RED + "Error: {} ({})".format(message, details) + DEFAULT)
     else:
-        formatted_message = message
-    raise SystemExit(RED + formatted_message + DEFAULT)
+        raise SystemExit(RED + 'Error: {}'.format(message) + DEFAULT)
 
-@join_args
 def unknown_error(message):
     fcode = sys._getframe(1).f_code
     raise SystemExit(RED + '{}:{} {}'.format(fcode.co_filename, fcode.co_name, message) + DEFAULT)
```

## clinterface/prompts.py

```diff
@@ -97,15 +97,15 @@
     def file_path(self):
         if self.message is None:
             raise ValueError('Message is not set')
         readline.set_completer_delims('\n')
         readline.parse_and_bind('tab: complete')
         readline.set_completer(path_completer())
         while True:
-            print(self.message + ':')
+            print(self.message)
             path = input('').rstrip()
             if path:
                 if os.path.isfile(path):
                     return os.path.normpath(path)
                 elif os.path.exists(path):
                     print('Path "{}" is not a file, try again'.format(path))
                 else:
@@ -113,15 +113,15 @@
     def directory_path(self):
         if self.message is None:
             raise ValueError('Message is not set')
         readline.set_completer_delims('\n')
         readline.parse_and_bind('tab: complete')
         readline.set_completer(path_completer())
         while True:
-            print(self.message + ':')
+            print(self.message)
             path = input('').rstrip()
             if path:
                 if os.path.isdir(path):
                     return os.path.normpath(path)
                 elif os.path.exists(path):
                     print('Path "{}" is not a directory, try again'.format(path))
                 else:
```

## clinterface/utils.py

```diff
@@ -1,17 +1,21 @@
 import os
 import sys
 import tty, termios
 import string
 import shutil
+from string import Template
 from .charDef import *
 from . import colors
 
 COLUMNS, _ = shutil.get_terminal_size()  ## Size of console
 
+def _(message, **kwargs):
+    return Template(message).safe_substitute(kwargs)
+
 def mygetc():
     ''' Get raw characters from input. '''
     fd = sys.stdin.fileno()
     old_settings = termios.tcgetattr(fd)
     try:
         tty.setraw(fd)
         ch = sys.stdin.read(1)
```

## Comparing `clinterface-0.1.1.post8.dist-info/LICENSE` & `clinterface-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clinterface-0.1.1.post8.dist-info/METADATA` & `clinterface-0.2.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinterface
-Version: 0.1.1.post8
+Version: 0.2.0
 Summary: Simple command line interface library
 Home-page: https://github.com/josemvas/clinterface
 License: LGPLv3+
 Keywords: console cli prompt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

