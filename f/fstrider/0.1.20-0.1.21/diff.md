# Comparing `tmp/fstrider-0.1.20.tar.gz` & `tmp/fstrider-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fstrider-0.1.20.tar", last modified: Thu Apr  4 13:32:05 2024, max compression
+gzip compressed data, was "fstrider-0.1.21.tar", last modified: Thu Apr  4 15:22:27 2024, max compression
```

## Comparing `fstrider-0.1.20.tar` & `fstrider-0.1.21.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 13:32:00.000000 fstrider-0.1.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-04 13:32:05.049124 fstrider-0.1.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-04 13:32:00.000000 fstrider-0.1.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/fstrider/
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/fs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/fstrider
--rw-r--r--   0 runner    (1001) docker     (127)    23859 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/fstrider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/os.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-04 13:32:00.000000 fstrider-0.1.20/fstrider/ptk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/fstrider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 13:32:05.000000 fstrider-0.1.20/fstrider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 13:32:00.000000 fstrider-0.1.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:32:05.049124 fstrider-0.1.20/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-04 13:32:00.000000 fstrider-0.1.20/tests/test_fstrider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:32:05.049124 fstrider-0.1.20/xontrib/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-04 13:32:00.000000 fstrider-0.1.20/xontrib/fstrider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:22:27.784519 fstrider-0.1.21/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 15:22:23.000000 fstrider-0.1.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-04 15:22:27.784519 fstrider-0.1.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-04 15:22:23.000000 fstrider-0.1.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:22:27.784519 fstrider-0.1.21/fstrider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-04 15:22:23.000000 fstrider-0.1.21/fstrider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 15:22:23.000000 fstrider-0.1.21/fstrider/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 15:22:23.000000 fstrider-0.1.21/fstrider/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-04 15:22:23.000000 fstrider-0.1.21/fstrider/fs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-04 15:22:23.000000 fstrider-0.1.21/fstrider/fstrider
+-rw-r--r--   0 runner    (1001) docker     (127)    23901 2024-04-04 15:22:23.000000 fstrider-0.1.21/fstrider/fstrider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-04 15:22:23.000000 fstrider-0.1.21/fstrider/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-04 15:22:23.000000 fstrider-0.1.21/fstrider/ptk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:22:27.784519 fstrider-0.1.21/fstrider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-04 15:22:27.000000 fstrider-0.1.21/fstrider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-04 15:22:27.000000 fstrider-0.1.21/fstrider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:22:27.000000 fstrider-0.1.21/fstrider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 15:22:27.000000 fstrider-0.1.21/fstrider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 15:22:27.000000 fstrider-0.1.21/fstrider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 15:22:23.000000 fstrider-0.1.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:22:27.784519 fstrider-0.1.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:22:27.784519 fstrider-0.1.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-04 15:22:23.000000 fstrider-0.1.21/tests/test_fstrider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:22:27.784519 fstrider-0.1.21/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-04 15:22:23.000000 fstrider-0.1.21/xontrib/fstrider.py
```

### Comparing `fstrider-0.1.20/LICENSE` & `fstrider-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.20/PKG-INFO` & `fstrider-0.1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstrider
-Version: 0.1.20
+Version: 0.1.21
 Summary: Library of the useful macroses for the xonsh shell.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -145,15 +145,15 @@
 Xonsh xontrib
     ++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18)
     ++ Run fstrider as fast as possible. (0.1.18)
     ++ Keeps history between running fstrider. (0.1.18)
 
 List
     ++ Async monitoring of the list and update if new files created. (0.1.19)
-    ++Add `/` to the end of directory in title and in history.
+    ++Add `/` to the end of directory in title and in history. 
     
 Configuration
     ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
 
 Integration
     "=" to move object from path to the current dir.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fstrider Version: 0.1.20 Summary: Library of the
+Metadata-Version: 2.1 Name: fstrider Version: 0.1.21 Summary: Library of the
 useful macroses for the xonsh shell. Author-email: anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `fstrider-0.1.20/README.md` & `fstrider-0.1.21/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 Xonsh xontrib
     ++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18)
     ++ Run fstrider as fast as possible. (0.1.18)
     ++ Keeps history between running fstrider. (0.1.18)
 
 List
     ++ Async monitoring of the list and update if new files created. (0.1.19)
-    ++Add `/` to the end of directory in title and in history.
+    ++Add `/` to the end of directory in title and in history. 
     
 Configuration
     ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
 
 Integration
     "=" to move object from path to the current dir.
```

### Comparing `fstrider-0.1.20/fstrider/__init__.py` & `fstrider-0.1.21/fstrider/__init__.py`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.20/fstrider/fs.py` & `fstrider-0.1.21/fstrider/fs.py`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.20/fstrider/fstrider.py` & `fstrider-0.1.21/fstrider/fstrider.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,14 +423,15 @@
         :param selected_by_value:
         :param title_msg:
         :param file_msg:
         :param update_list:
         :return:
         """
         self.mode = 'list'
+        p = p if p else self.current_path
         self.set_current_path(p)
         self.set_title(p, msg=title_msg)
         if self.current_path.is_dir() and self.env['os_path_change']:
             os.chdir(self.current_path)
         self.update_list(selected_by_value=selected_by_value, title_msg=title_msg, file_msg=file_msg)
 
     def do_open_with(self, path: Path = None):
```

### Comparing `fstrider-0.1.20/fstrider/os.py` & `fstrider-0.1.21/fstrider/os.py`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.20/fstrider/ptk.py` & `fstrider-0.1.21/fstrider/ptk.py`

 * *Files identical despite different names*

### Comparing `fstrider-0.1.20/fstrider.egg-info/PKG-INFO` & `fstrider-0.1.21/fstrider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstrider
-Version: 0.1.20
+Version: 0.1.21
 Summary: Library of the useful macroses for the xonsh shell.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -145,15 +145,15 @@
 Xonsh xontrib
     ++ Creates alias `fs` (or `fstrider` if `fs` exists). (0.1.18)
     ++ Run fstrider as fast as possible. (0.1.18)
     ++ Keeps history between running fstrider. (0.1.18)
 
 List
     ++ Async monitoring of the list and update if new files created. (0.1.19)
-    ++Add `/` to the end of directory in title and in history.
+    ++Add `/` to the end of directory in title and in history. 
     
 Configuration
     ++ Read env from `os.env`. See `fstrider.env`. (0.1.19)
 
 Integration
     "=" to move object from path to the current dir.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fstrider Version: 0.1.20 Summary: Library of the
+Metadata-Version: 2.1 Name: fstrider Version: 0.1.21 Summary: Library of the
 useful macroses for the xonsh shell. Author-email: anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `fstrider-0.1.20/pyproject.toml` & `fstrider-0.1.21/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fstrider"
-version = "0.1.20"
+version = "0.1.21"
 license = {file = "LICENSE"}
 description = "Library of the useful macroses for the xonsh shell."
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: System :: Shells",
```

