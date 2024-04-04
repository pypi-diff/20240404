# Comparing `tmp/python_course_by_ty-0.1.7.tar.gz` & `tmp/python_course_by_ty-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_course_by_ty-0.1.7.tar", last modified: Thu Apr  4 21:45:08 2024, max compression
+gzip compressed data, was "python_course_by_ty-0.1.8.tar", last modified: Thu Apr  4 21:50:42 2024, max compression
```

## Comparing `python_course_by_ty-0.1.7.tar` & `python_course_by_ty-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:45:08.288105 python_course_by_ty-0.1.7/
--rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:45:08.287977 python_course_by_ty-0.1.7/PKG-INFO
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:45:08.287045 python_course_by_ty-0.1.7/python_course_by_ty/
--rw-r--r--   0 tygriffiths   (501) staff       (20)       44 2024-03-04 14:40:28.000000 python_course_by_ty-0.1.7/python_course_by_ty/__init__.py
--rw-r--r--   0 tygriffiths   (501) staff       (20)    88841 2024-04-04 21:43:53.000000 python_course_by_ty-0.1.7/python_course_by_ty/python_course.py
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:45:08.287786 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/
--rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/PKG-INFO
--rw-r--r--   0 tygriffiths   (501) staff       (20)      291 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/SOURCES.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)        1 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/dependency_links.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       31 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/requires.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       20 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/top_level.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       38 2024-04-04 21:45:08.288154 python_course_by_ty-0.1.7/setup.cfg
--rw-r--r--   0 tygriffiths   (501) staff       (20)      731 2024-04-04 21:44:58.000000 python_course_by_ty-0.1.7/setup.py
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:50:42.691753 python_course_by_ty-0.1.8/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:50:42.691634 python_course_by_ty-0.1.8/PKG-INFO
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:50:42.690696 python_course_by_ty-0.1.8/python_course_by_ty/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       44 2024-03-04 14:40:28.000000 python_course_by_ty-0.1.8/python_course_by_ty/__init__.py
+-rw-r--r--   0 tygriffiths   (501) staff       (20)    88841 2024-04-04 21:48:07.000000 python_course_by_ty-0.1.8/python_course_by_ty/python_course.py
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:50:42.691447 python_course_by_ty-0.1.8/python_course_by_ty.egg-info/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:50:42.000000 python_course_by_ty-0.1.8/python_course_by_ty.egg-info/PKG-INFO
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      291 2024-04-04 21:50:42.000000 python_course_by_ty-0.1.8/python_course_by_ty.egg-info/SOURCES.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)        1 2024-04-04 21:50:42.000000 python_course_by_ty-0.1.8/python_course_by_ty.egg-info/dependency_links.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       31 2024-04-04 21:50:42.000000 python_course_by_ty-0.1.8/python_course_by_ty.egg-info/requires.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       20 2024-04-04 21:50:42.000000 python_course_by_ty-0.1.8/python_course_by_ty.egg-info/top_level.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       38 2024-04-04 21:50:42.691806 python_course_by_ty-0.1.8/setup.cfg
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      731 2024-04-04 21:50:02.000000 python_course_by_ty-0.1.8/setup.py
```

### Comparing `python_course_by_ty-0.1.7/python_course_by_ty/python_course.py` & `python_course_by_ty-0.1.8/python_course_by_ty/python_course.py`

 * *Files identical despite different names*

### Comparing `python_course_by_ty-0.1.7/setup.py` & `python_course_by_ty-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python_course_by_ty",
-    version="0.1.7",
+    version="0.1.8",
     description="A package for testing student answers to project questions.",
     url="https://github.com/TyGriffiths/python_course_by_ty",
     author="Ty Griffiths",
     author_email="griffiths.ty@yahoo.com",
     license="GNU General Public License v3.0",
     packages=["python_course_by_ty"],
     install_requires=[
```

