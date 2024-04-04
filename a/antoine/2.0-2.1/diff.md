# Comparing `tmp/antoine-2.0.tar.gz` & `tmp/antoine-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antoine-2.0.tar", last modified: Thu Apr  4 14:06:09 2024, max compression
+gzip compressed data, was "antoine-2.1.tar", last modified: Thu Apr  4 14:08:27 2024, max compression
```

## Comparing `antoine-2.0.tar` & `antoine-2.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:06:09.237138 antoine-2.0/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 14:06:09.236924 antoine-2.0/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      260 2024-04-04 14:01:11.000000 antoine-2.0/README.md
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:06:09.236067 antoine-2.0/antoine/
--rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-2.0/antoine/__init__.py
--rw-r--r--   0 antoinebertin   (501) staff       (20)     1443 2024-04-04 13:08:46.000000 antoine-2.0/antoine/app.py
--rw-r--r--   0 antoinebertin   (501) staff       (20)      184 2024-04-04 14:04:27.000000 antoine-2.0/antoine/post_install.py
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:06:09.236686 antoine-2.0/antoine.egg-info/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 14:06:09.000000 antoine-2.0/antoine.egg-info/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      235 2024-04-04 14:06:09.000000 antoine-2.0/antoine.egg-info/SOURCES.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-04 14:06:09.000000 antoine-2.0/antoine.egg-info/dependency_links.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       49 2024-04-04 14:06:09.000000 antoine-2.0/antoine.egg-info/entry_points.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-04 14:06:09.000000 antoine-2.0/antoine.egg-info/top_level.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-04 14:06:09.237177 antoine-2.0/setup.cfg
--rw-r--r--   0 antoinebertin   (501) staff       (20)      607 2024-04-04 14:05:33.000000 antoine-2.0/setup.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:08:27.021785 antoine-2.1/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 14:08:27.021587 antoine-2.1/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      260 2024-04-04 14:01:11.000000 antoine-2.1/README.md
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:08:27.020844 antoine-2.1/antoine/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-2.1/antoine/__init__.py
+-rw-r--r--   0 antoinebertin   (501) staff       (20)     1443 2024-04-04 13:08:46.000000 antoine-2.1/antoine/app.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 14:08:27.021382 antoine-2.1/antoine.egg-info/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 14:08:26.000000 antoine-2.1/antoine.egg-info/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-04 14:08:26.000000 antoine-2.1/antoine.egg-info/SOURCES.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-04 14:08:26.000000 antoine-2.1/antoine.egg-info/dependency_links.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       49 2024-04-04 14:08:26.000000 antoine-2.1/antoine.egg-info/entry_points.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-04 14:08:26.000000 antoine-2.1/antoine.egg-info/top_level.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-04 14:08:27.021819 antoine-2.1/setup.cfg
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      574 2024-04-04 14:07:43.000000 antoine-2.1/setup.py
```

### Comparing `antoine-2.0/antoine/app.py` & `antoine-2.1/antoine/app.py`

 * *Files identical despite different names*

### Comparing `antoine-2.0/setup.py` & `antoine-2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup
 
 setup(
     name='antoine',
-    version='2.0',
+    version='2.1',
     packages=['antoine'],  # 'antoine' is the name of the package
     author='Antoine Bertin',
     author_email='monolok35@gmail.com',
     description='Hiring Antoine is so much fun!',
     url='https://github.com/monolok/antoine/',
     license='MIT',
     entry_points={
         'console_scripts': [
             'hireantoine=antoine.app:main',  # 'antoine' is the name of the package and 'app.py' contains a function 'main'
         ],
     },
     include_package_data=True,
-    install_requires=[],
-    scripts=['post_install.py']
+    install_requires=[]
 )
```

