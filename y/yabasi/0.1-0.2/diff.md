# Comparing `tmp/yabasi-0.1.tar.gz` & `tmp/yabasi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yabasi-0.1.tar", last modified: Tue Apr  2 10:20:34 2024, max compression
+gzip compressed data, was "yabasi-0.2.tar", last modified: Thu Apr  4 16:59:00 2024, max compression
```

## Comparing `yabasi-0.1.tar` & `yabasi-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-02 10:20:34.221551 yabasi-0.1/
--rw-r--r--   0 ralf      (1000) priv      (1011)     1357 2024-04-02 10:17:11.000000 yabasi-0.1/LICENSE
--rw-r--r--   0 ralf      (1000) priv      (1011)     2205 2024-04-02 10:20:34.221551 yabasi-0.1/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     1265 2024-04-02 10:05:50.000000 yabasi-0.1/README.rst
--rw-r--r--   0 ralf      (1000) priv      (1011)        4 2024-04-02 10:20:31.000000 yabasi-0.1/VERSION
--rw-r--r--   0 ralf      (1000) priv      (1011)     2547 2024-04-02 09:53:54.000000 yabasi-0.1/pyproject.toml
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2024-04-02 10:20:34.221551 yabasi-0.1/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2921 2024-04-02 09:55:48.000000 yabasi-0.1/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-02 10:20:34.193551 yabasi-0.1/yabasi/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2024-04-02 10:20:31.000000 yabasi-0.1/yabasi/Version.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    32979 2024-04-02 10:07:35.000000 yabasi-0.1/yabasi/bas.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)     3349 2024-03-31 14:44:12.000000 yabasi-0.1/yabasi/tokenizer.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-02 10:20:34.217551 yabasi-0.1/yabasi.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)     2205 2024-04-02 10:20:34.000000 yabasi-0.1/yabasi.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      284 2024-04-02 10:20:34.000000 yabasi-0.1/yabasi.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2024-04-02 10:20:34.000000 yabasi-0.1/yabasi.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       43 2024-04-02 10:20:34.000000 yabasi-0.1/yabasi.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        6 2024-04-02 10:20:34.000000 yabasi-0.1/yabasi.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        7 2024-04-02 10:20:34.000000 yabasi-0.1/yabasi.egg-info/top_level.txt
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-04 16:59:00.154663 yabasi-0.2/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1357 2024-04-02 10:17:11.000000 yabasi-0.2/LICENSE
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2286 2024-04-04 16:59:00.150663 yabasi-0.2/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1327 2024-04-04 16:49:42.000000 yabasi-0.2/README.rst
+-rw-r--r--   0 ralf      (1000) priv      (1011)        4 2024-04-04 16:58:57.000000 yabasi-0.2/VERSION
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2554 2024-04-04 16:57:11.000000 yabasi-0.2/pyproject.toml
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2024-04-04 16:59:00.154663 yabasi-0.2/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2928 2024-04-04 16:57:02.000000 yabasi-0.2/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-04 16:59:00.126664 yabasi-0.2/yabasi/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2024-04-04 16:58:57.000000 yabasi-0.2/yabasi/Version.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    32979 2024-04-02 10:07:35.000000 yabasi-0.2/yabasi/bas.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)     3349 2024-03-31 14:44:12.000000 yabasi-0.2/yabasi/tokenizer.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2024-04-04 16:59:00.146664 yabasi-0.2/yabasi.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2286 2024-04-04 16:58:59.000000 yabasi-0.2/yabasi.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      284 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       43 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       10 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        7 2024-04-04 16:59:00.000000 yabasi-0.2/yabasi.egg-info/top_level.txt
```

### Comparing `yabasi-0.1/LICENSE` & `yabasi-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yabasi-0.1/PKG-INFO` & `yabasi-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yabasi
-Version: 0.1
+Version: 0.2
 Summary: Minimal BASIC interpreter for running MININEC
 Home-page: https://github.com/schlatterbeck/yabasi
 Author: Ralf Schlatterbeck
 Author-email: Ralf Schlatterbeck <rsc@runtux.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/schlatterbeck/yabasi
 Project-URL: Bug Tracker, https://github.com/schlatterbeck/yabasi/issues
@@ -18,31 +18,33 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ply
 
 YABASI -- Yet another BASIC Interpreter
 =======================================
 
 This is a BASIC interpreter for an old dialect of the language used in
 early IBM PCs. It is written in Python. I wrote this over a weekend to
-be able to run old MININEC_ code. It has almost no error checking (it
+be able to run old MININEC_ code (the linked version of MININEC_
+contains some small fixes). It has almost no error checking (it
 relies on the code being correct not trying to aid you in writing a new
 program in BASIC, I think the world does not need new code in BASIC). If
 you're looking for a working BASIC interpreter, look at the pcbasic_
 implementation, it is also in Python but faithfully reproduces the
 memory limitations of the machines at the time. And it seems to use
 single-precision floating point numbers. This is why I wrote my own
 interpreter: I needed to compare computations in double precision and I
 could not fit some examples into the limited memory of pcbasic_.
 
 I'm probably not going to put much work into improving this code, it has
 achieved the purpose: Running (and debugging in Python) old MININEC_
 code to allow me to compare the computations in BASIC to my
 re-implementation of MININEC_ in Python, pymininec_.
 
-.. _MININEC: https://github.com/Kees-PA3KJ/MiniNec
+.. _MININEC: https://github.com/schlatterbeck/MiniNec
 .. _pcbasic: https://robhagemans.github.io/pcbasic/
 .. _pymininec: https://github.com/schlatterbeck/pymininec
```

### Comparing `yabasi-0.1/README.rst` & `yabasi-0.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 YABASI -- Yet another BASIC Interpreter
 =======================================
 
 This is a BASIC interpreter for an old dialect of the language used in
 early IBM PCs. It is written in Python. I wrote this over a weekend to
-be able to run old MININEC_ code. It has almost no error checking (it
+be able to run old MININEC_ code (the linked version of MININEC_
+contains some small fixes). It has almost no error checking (it
 relies on the code being correct not trying to aid you in writing a new
 program in BASIC, I think the world does not need new code in BASIC). If
 you're looking for a working BASIC interpreter, look at the pcbasic_
 implementation, it is also in Python but faithfully reproduces the
 memory limitations of the machines at the time. And it seems to use
 single-precision floating point numbers. This is why I wrote my own
 interpreter: I needed to compare computations in double precision and I
 could not fit some examples into the limited memory of pcbasic_.
 
 I'm probably not going to put much work into improving this code, it has
 achieved the purpose: Running (and debugging in Python) old MININEC_
 code to allow me to compare the computations in BASIC to my
 re-implementation of MININEC_ in Python, pymininec_.
 
-.. _MININEC: https://github.com/Kees-PA3KJ/MiniNec
+.. _MININEC: https://github.com/schlatterbeck/MiniNec
 .. _pcbasic: https://robhagemans.github.io/pcbasic/
 .. _pymininec: https://github.com/schlatterbeck/pymininec
```

### Comparing `yabasi-0.1/pyproject.toml` & `yabasi-0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 name            = "yabasi"
 dynamic         = ["version"]
 authors         = [{ name="Ralf Schlatterbeck", email="rsc@runtux.com" }, ]
 description     = "Minimal BASIC interpreter for running MININEC"
 readme          = "README.rst"
 license         = {text = "MIT License"}
 requires-python = '>=3.11'
-dependencies    = ['numpy']
+dependencies    = ['numpy', 'ply']
 classifiers     = [
           'Development Status :: 4 - Beta'
         , 'License :: OSI Approved :: MIT License'
         , 'Operating System :: OS Independent'
         , 'Intended Audience :: Science/Research'
         , 'Intended Audience :: Other Audience'
         , 'Topic :: Communications :: Ham Radio'
```

### Comparing `yabasi-0.1/setup.py` & `yabasi-0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     , version          = __version__
     , description      = "Minimal BASIC interpreter for running MININEC"
     , long_description = ''.join (description)
     , long_description_content_type='text/x-rst'
     , license          = license
     , author           = "Ralf Schlatterbeck"
     , author_email     = "rsc@runtux.com"
-    , install_requires = ['numpy']
+    , install_requires = ['numpy', 'ply']
     , packages         = ['yabasi']
     , platforms        = 'Any'
     , url              = "https://github.com/schlatterbeck/yabasi"
     , python_requires  = rq
     , entry_points     = dict
         ( console_scripts =
             [ 'yabasi=yabasi.bas:main'
```

### Comparing `yabasi-0.1/yabasi/bas.py` & `yabasi-0.2/yabasi/bas.py`

 * *Files identical despite different names*

### Comparing `yabasi-0.1/yabasi/tokenizer.py` & `yabasi-0.2/yabasi/tokenizer.py`

 * *Files identical despite different names*

### Comparing `yabasi-0.1/yabasi.egg-info/PKG-INFO` & `yabasi-0.2/yabasi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yabasi
-Version: 0.1
+Version: 0.2
 Summary: Minimal BASIC interpreter for running MININEC
 Home-page: https://github.com/schlatterbeck/yabasi
 Author: Ralf Schlatterbeck
 Author-email: Ralf Schlatterbeck <rsc@runtux.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/schlatterbeck/yabasi
 Project-URL: Bug Tracker, https://github.com/schlatterbeck/yabasi/issues
@@ -18,31 +18,33 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ply
 
 YABASI -- Yet another BASIC Interpreter
 =======================================
 
 This is a BASIC interpreter for an old dialect of the language used in
 early IBM PCs. It is written in Python. I wrote this over a weekend to
-be able to run old MININEC_ code. It has almost no error checking (it
+be able to run old MININEC_ code (the linked version of MININEC_
+contains some small fixes). It has almost no error checking (it
 relies on the code being correct not trying to aid you in writing a new
 program in BASIC, I think the world does not need new code in BASIC). If
 you're looking for a working BASIC interpreter, look at the pcbasic_
 implementation, it is also in Python but faithfully reproduces the
 memory limitations of the machines at the time. And it seems to use
 single-precision floating point numbers. This is why I wrote my own
 interpreter: I needed to compare computations in double precision and I
 could not fit some examples into the limited memory of pcbasic_.
 
 I'm probably not going to put much work into improving this code, it has
 achieved the purpose: Running (and debugging in Python) old MININEC_
 code to allow me to compare the computations in BASIC to my
 re-implementation of MININEC_ in Python, pymininec_.
 
-.. _MININEC: https://github.com/Kees-PA3KJ/MiniNec
+.. _MININEC: https://github.com/schlatterbeck/MiniNec
 .. _pcbasic: https://robhagemans.github.io/pcbasic/
 .. _pymininec: https://github.com/schlatterbeck/pymininec
```

