# Comparing `tmp/DmHaloGeometry-0.1.tar.gz` & `tmp/DmHaloGeometry-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DmHaloGeometry-0.1.tar", last modified: Wed Mar 20 19:45:56 2024, max compression
+gzip compressed data, was "DmHaloGeometry-1.1.tar", last modified: Thu Apr  4 20:20:19 2024, max compression
```

## Comparing `DmHaloGeometry-0.1.tar` & `DmHaloGeometry-1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 lmezini    (501) staff       (20)        0 2024-03-20 19:45:56.527617 DmHaloGeometry-0.1/
-drwxr-xr-x   0 lmezini    (501) staff       (20)        0 2024-03-20 19:45:56.527587 DmHaloGeometry-0.1/DmHaloGeometry/
--rw-r--r--   0 lmezini    (501) staff       (20)       60 2024-03-20 19:32:59.414594 DmHaloGeometry-0.1/DmHaloGeometry/__init__.py
--rw-r--r--   0 lmezini    (501) staff       (20)    10140 2024-03-20 19:41:18.641996 DmHaloGeometry-0.1/DmHaloGeometry/halo_orientation.py
--rw-r--r--   0 lmezini    (501) staff       (20)      798 2024-03-20 19:45:56.527668 DmHaloGeometry-0.1/PKG-INFO
--rw-r--r--   0 lmezini    (501) staff       (20)       82 2024-03-20 19:39:24.366592 DmHaloGeometry-0.1/README.txt
--rw-r--r--   0 lmezini    (501) staff       (20)       39 2024-03-20 19:39:41.411970 DmHaloGeometry-0.1/setup.cfg
--rw-r--r--   0 lmezini    (501) staff       (20)     1729 2024-03-20 19:38:30.977086 DmHaloGeometry-0.1/setup.py
+drwxr-xr-x   0 lmezini    (501) staff       (20)        0 2024-04-04 20:20:19.130662 DmHaloGeometry-1.1/
+drwxr-xr-x   0 lmezini    (501) staff       (20)        0 2024-04-04 20:20:19.130636 DmHaloGeometry-1.1/DmHaloGeometry/
+-rw-r--r--   0 lmezini    (501) staff       (20)       60 2024-04-04 19:52:25.587248 DmHaloGeometry-1.1/DmHaloGeometry/__init__.py
+-rw-r--r--   0 lmezini    (501) staff       (20)        0 2024-04-04 19:56:44.393606 DmHaloGeometry-1.1/DmHaloGeometry/halo_orientation.py
+-rw-r--r--   0 lmezini    (501) staff       (20)      798 2024-04-04 20:20:19.130720 DmHaloGeometry-1.1/PKG-INFO
+-rw-r--r--   0 lmezini    (501) staff       (20)      134 2024-04-04 19:52:25.587626 DmHaloGeometry-1.1/README.txt
+-rw-r--r--   0 lmezini    (501) staff       (20)       39 2024-04-04 19:52:25.587718 DmHaloGeometry-1.1/setup.cfg
+-rw-r--r--   0 lmezini    (501) staff       (20)     1729 2024-04-04 20:06:49.201586 DmHaloGeometry-1.1/setup.py
```

### Comparing `DmHaloGeometry-0.1/PKG-INFO` & `DmHaloGeometry-1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: DmHaloGeometry
-Version: 0.1
+Version: 1.1
 Summary: Do geometric computations on dark matter particle data
 Home-page: https://github.com/lmezini/DmHaloGeometry
 Author: Lorena Mezini
 Author-email: lom31@pitt.edu
 License: MIT
-Download-URL: https://github.com/lmezini/DmHaloGeometry/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/lmezini/DmHaloGeometry/archive/refs/tags/v1.1.tar.gz
 Description: UNKNOWN
 Keywords: simulation,dark matter,geometry
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DmHaloGeometry-0.1/setup.py` & `DmHaloGeometry-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 from distutils.core import setup
 setup(
     name='DmHaloGeometry',         # How you named your package folder (MyLib)
     packages=['DmHaloGeometry'],   # Chose the same as "name"
-    version='0.1',      # Start with a small number and increase it with every change you make
+    version='1.1',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Do geometric computations on dark matter particle data',
     author='Lorena Mezini',                   # Type in your name
     author_email='lom31@pitt.edu',      # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/lmezini/DmHaloGeometry',
     # I explain this later on
-    download_url='https://github.com/lmezini/DmHaloGeometry/archive/refs/tags/v_01.tar.gz',
+    download_url='https://github.com/lmezini/DmHaloGeometry/archive/refs/tags/v1.1.tar.gz',
     # Keywords that define your package best
     keywords=['simulation', 'dark matter', 'geometry'],
     install_requires=[            # I get to this in a second
         'numpy',
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

