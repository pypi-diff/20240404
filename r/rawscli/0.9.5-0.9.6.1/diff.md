# Comparing `tmp/rawscli-0.9.5.tar.gz` & `tmp/rawscli-0.9.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rawscli-0.9.5.tar", last modified: Fri Feb 24 16:38:58 2023, max compression
+gzip compressed data, was "rawscli-0.9.6.1.tar", last modified: Thu Apr  4 12:40:26 2024, max compression
```

## Comparing `rawscli-0.9.5.tar` & `rawscli-0.9.6.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:58.285294 rawscli-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-24 16:38:48.000000 rawscli-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-02-24 16:38:58.285294 rawscli-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-02-24 16:38:48.000000 rawscli-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16862 2023-02-24 16:38:48.000000 rawscli-0.9.5/raws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:58.285294 rawscli-0.9.5/rawscli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-02-24 16:38:58.000000 rawscli-0.9.5/rawscli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-24 16:38:58.000000 rawscli-0.9.5/rawscli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 16:38:58.000000 rawscli-0.9.5/rawscli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-24 16:38:58.000000 rawscli-0.9.5/rawscli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-24 16:38:58.000000 rawscli-0.9.5/rawscli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-24 16:38:58.285294 rawscli-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-24 16:38:48.000000 rawscli-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:40:26.417160 rawscli-0.9.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 12:40:20.000000 rawscli-0.9.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-04 12:40:26.417160 rawscli-0.9.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-04 12:40:20.000000 rawscli-0.9.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16875 2024-04-04 12:40:20.000000 rawscli-0.9.6.1/raws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:40:26.417160 rawscli-0.9.6.1/rawscli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-04 12:40:26.000000 rawscli-0.9.6.1/rawscli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 12:40:26.000000 rawscli-0.9.6.1/rawscli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:40:26.000000 rawscli-0.9.6.1/rawscli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 12:40:26.000000 rawscli-0.9.6.1/rawscli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 12:40:26.000000 rawscli-0.9.6.1/rawscli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 12:40:26.000000 rawscli-0.9.6.1/rawscli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-04 12:40:26.417160 rawscli-0.9.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 12:40:20.000000 rawscli-0.9.6.1/setup.py
```

### Comparing `rawscli-0.9.5/LICENSE` & `rawscli-0.9.6.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Viacheslav Andzhich
+Copyright (c) 2024 Viacheslav Andzhich
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rawscli-0.9.5/PKG-INFO` & `rawscli-0.9.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rawscli
-Version: 0.9.5
+Version: 0.9.6.1
 Summary: A simple tool to manage your AWS credentials
 Home-page: https://github.com/andzhi4/raws
 Author: Viacheslav Andzhich
 Author-email: va.public@protonmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyperclip==1.8.2
 
 [![build status](https://github.com/andzhi4/raws/actions/workflows/matrix-test.yml/badge.svg)](https://github.com/andzhi4/raws/actions/workflows/matrix-test.yml)
 # RAWS
 
 RAWS is a simple AWS Profile Manager with a command-line interface that helps you easily manipulate AWS profiles on your local machine.
 RAWS will lookup location of your AWS credentials file through environment variable `AWS_CREDS_FILE`. If the variable is not set, it will default to `~/.aws/credentials`. You can also override the file location by specifing `--creds_file` argument.
```

### Comparing `rawscli-0.9.5/README.md` & `rawscli-0.9.6.1/README.md`

 * *Files identical despite different names*

### Comparing `rawscli-0.9.5/raws.py` & `rawscli-0.9.6.1/raws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Optional
 import argparse
 import fnmatch
 import os
+import pyperclip  # type: ignore
 import shutil
-import subprocess
 
 """
 A simple tool for AWS profiles management
 TODO: add .aws/config manipulation:
         raws config <profile> <option> <value>
 """
 
 # Version info
 NAME = 'raws'
-VERSION = '0.9.5'
+VERSION = '0.9.6.1'
 DESCRIPTION = 'A simple tool to manage your AWS credentials'
 
 
 # Env variable init to reference the credentials file
 DEFAULT_CREDS_LOCATION = os.path.join(os.path.expanduser('~'), '.aws', 'credentials')
 if 'AWS_CREDS_FILE' not in os.environ\
         or not os.path.isdir(os.path.dirname(os.environ['AWS_CREDS_FILE'])):
@@ -156,15 +156,15 @@
 
             # Last profile
             current_profile = self._build_profile(collected_lines)
             existing_profiles[current_profile.profile_name] = current_profile
             return existing_profiles
 
     def _get_profile_from_clipboard(self) -> AWSProfile:
-        clipboard_text = subprocess.check_output(['pbpaste',]).decode('utf-8')
+        clipboard_text = pyperclip.paste()
         if 'aws_access_key_id' not in clipboard_text:
             raise ValueError('AWS Access Key is not in the clipboard')
         lines = clipboard_text.split('\n')
         prof = self._build_profile(lines)
         return prof
 
     def _get_profile_from_env(self) -> AWSProfile:
@@ -414,9 +414,10 @@
         return 1
 
     return 0
 
 
 # TODO: validate_profile() method to check whether the passed text is valid AWS profile
 # TODO: implement __setattr__()
+# TODO: add stubs for pyperclip
 if __name__ == '__main__':
     raise SystemExit(main())
```

### Comparing `rawscli-0.9.5/rawscli.egg-info/PKG-INFO` & `rawscli-0.9.6.1/rawscli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rawscli
-Version: 0.9.5
+Version: 0.9.6.1
 Summary: A simple tool to manage your AWS credentials
 Home-page: https://github.com/andzhi4/raws
 Author: Viacheslav Andzhich
 Author-email: va.public@protonmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyperclip==1.8.2
 
 [![build status](https://github.com/andzhi4/raws/actions/workflows/matrix-test.yml/badge.svg)](https://github.com/andzhi4/raws/actions/workflows/matrix-test.yml)
 # RAWS
 
 RAWS is a simple AWS Profile Manager with a command-line interface that helps you easily manipulate AWS profiles on your local machine.
 RAWS will lookup location of your AWS credentials file through environment variable `AWS_CREDS_FILE`. If the variable is not set, it will default to `~/.aws/credentials`. You can also override the file location by specifing `--creds_file` argument.
```

### Comparing `rawscli-0.9.5/setup.cfg` & `rawscli-0.9.6.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rawscli
-version = 0.9.5
+version = 0.9.6.1
 description = A simple tool to manage your AWS credentials
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/andzhi4/raws
 author = Viacheslav Andzhich
 author_email = va.public@protonmail.com
 license = MIT
@@ -14,15 +14,17 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 py_modules = raws
-python_requires = >=3.8
+python_requires = >=3.9
+install_requires = 
+	pyperclip==1.8.2
 
 [options.entry_points]
 console_scripts = 
 	raws = raws:main
 
 [bdist_wheel]
 universal = True
```

