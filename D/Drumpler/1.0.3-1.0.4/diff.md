# Comparing `tmp/Drumpler-1.0.3.tar.gz` & `tmp/Drumpler-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.0.3.tar", last modified: Thu Apr  4 18:16:55 2024, max compression
+gzip compressed data, was "Drumpler-1.0.4.tar", last modified: Thu Apr  4 18:23:03 2024, max compression
```

## Comparing `Drumpler-1.0.3.tar` & `Drumpler-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:16:55.064829 Drumpler-1.0.3/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:16:55.062885 Drumpler-1.0.3/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     3364 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-04 18:16:55.000000 Drumpler-1.0.3/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.3/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     3364 2024-04-04 18:16:55.063812 Drumpler-1.0.3/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     2701 2024-04-04 18:14:59.000000 Drumpler-1.0.3/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:16:55.057236 Drumpler-1.0.3/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.3/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      599 2024-04-03 21:23:08.000000 Drumpler-1.0.3/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     6474 2024-04-03 21:38:26.000000 Drumpler-1.0.3/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.3/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.3/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-04 18:16:55.065108 Drumpler-1.0.3/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-04 18:13:09.000000 Drumpler-1.0.3/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:16:55.061828 Drumpler-1.0.3/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.3/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:23:03.970446 Drumpler-1.0.4/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:23:03.968127 Drumpler-1.0.4/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     3364 2024-04-04 18:23:03.000000 Drumpler-1.0.4/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-04 18:23:03.000000 Drumpler-1.0.4/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-04 18:23:03.000000 Drumpler-1.0.4/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-04 18:23:03.000000 Drumpler-1.0.4/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-04 18:23:03.000000 Drumpler-1.0.4/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.4/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     3364 2024-04-04 18:23:03.969353 Drumpler-1.0.4/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     2701 2024-04-04 18:14:59.000000 Drumpler-1.0.4/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:23:03.961646 Drumpler-1.0.4/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.4/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      599 2024-04-03 21:23:08.000000 Drumpler-1.0.4/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6474 2024-04-03 21:38:26.000000 Drumpler-1.0.4/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.4/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.4/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-04 18:23:03.970669 Drumpler-1.0.4/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-04 18:20:38.000000 Drumpler-1.0.4/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:23:03.966941 Drumpler-1.0.4/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.4/test/test_drumpler.py
```

### Comparing `Drumpler-1.0.3/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.0.4/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.3
+Version: 1.0.4
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.3/LICENSE` & `Drumpler-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.3/PKG-INFO` & `Drumpler-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.3
+Version: 1.0.4
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.3/README.md` & `Drumpler-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.3/drumpler/constants.py` & `Drumpler-1.0.4/drumpler/constants.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.3/drumpler/drumpler.py` & `Drumpler-1.0.4/drumpler/drumpler.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.3/drumpler/mammoth.py` & `Drumpler-1.0.4/drumpler/mammoth.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.3/drumpler/request.py` & `Drumpler-1.0.4/drumpler/request.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.3/setup.py` & `Drumpler-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.0.3',
+    version='1.0.4',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.0.3/test/test_drumpler.py` & `Drumpler-1.0.4/test/test_drumpler.py`

 * *Files identical despite different names*

