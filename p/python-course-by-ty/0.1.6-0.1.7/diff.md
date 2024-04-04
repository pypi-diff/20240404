# Comparing `tmp/python_course_by_ty-0.1.6.tar.gz` & `tmp/python_course_by_ty-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_course_by_ty-0.1.6.tar", last modified: Thu Apr  4 21:37:02 2024, max compression
+gzip compressed data, was "python_course_by_ty-0.1.7.tar", last modified: Thu Apr  4 21:45:08 2024, max compression
```

## Comparing `python_course_by_ty-0.1.6.tar` & `python_course_by_ty-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:37:02.823076 python_course_by_ty-0.1.6/
--rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:37:02.822954 python_course_by_ty-0.1.6/PKG-INFO
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:37:02.821440 python_course_by_ty-0.1.6/python_course_by_ty/
--rw-r--r--   0 tygriffiths   (501) staff       (20)       44 2024-03-04 14:40:28.000000 python_course_by_ty-0.1.6/python_course_by_ty/__init__.py
--rw-r--r--   0 tygriffiths   (501) staff       (20)    88802 2024-04-04 21:31:48.000000 python_course_by_ty-0.1.6/python_course_by_ty/python_course.py
-drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:37:02.822748 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/
--rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/PKG-INFO
--rw-r--r--   0 tygriffiths   (501) staff       (20)      291 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/SOURCES.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)        1 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/dependency_links.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       31 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/requires.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       20 2024-04-04 21:37:02.000000 python_course_by_ty-0.1.6/python_course_by_ty.egg-info/top_level.txt
--rw-r--r--   0 tygriffiths   (501) staff       (20)       38 2024-04-04 21:37:02.823129 python_course_by_ty-0.1.6/setup.cfg
--rw-r--r--   0 tygriffiths   (501) staff       (20)      731 2024-04-04 21:35:50.000000 python_course_by_ty-0.1.6/setup.py
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:45:08.288105 python_course_by_ty-0.1.7/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:45:08.287977 python_course_by_ty-0.1.7/PKG-INFO
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:45:08.287045 python_course_by_ty-0.1.7/python_course_by_ty/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       44 2024-03-04 14:40:28.000000 python_course_by_ty-0.1.7/python_course_by_ty/__init__.py
+-rw-r--r--   0 tygriffiths   (501) staff       (20)    88841 2024-04-04 21:43:53.000000 python_course_by_ty-0.1.7/python_course_by_ty/python_course.py
+drwxr-xr-x   0 tygriffiths   (501) staff       (20)        0 2024-04-04 21:45:08.287786 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      484 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/PKG-INFO
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      291 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/SOURCES.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)        1 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/dependency_links.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       31 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/requires.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       20 2024-04-04 21:45:08.000000 python_course_by_ty-0.1.7/python_course_by_ty.egg-info/top_level.txt
+-rw-r--r--   0 tygriffiths   (501) staff       (20)       38 2024-04-04 21:45:08.288154 python_course_by_ty-0.1.7/setup.cfg
+-rw-r--r--   0 tygriffiths   (501) staff       (20)      731 2024-04-04 21:44:58.000000 python_course_by_ty-0.1.7/setup.py
```

### Comparing `python_course_by_ty-0.1.6/python_course_by_ty/python_course.py` & `python_course_by_ty-0.1.7/python_course_by_ty/python_course.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # The notebooks provided to the students will then import this file and make calls to it
 # Each function corresponds to a quiz question in a quiz that is associated with the notebook they are working through
 # If the student's answer is correct, the function will output a keyword or phrase to answer the quiz question with
 # If the answer is incorrect, the function will output a statement telling them their answer was incorrect
 # Risks associated with beginner python students finding answers in this file was felt to be minimal and worth alternatives
 
 # install dependencies
+import pandas as pd
+import numpy as np
 import requests
 from bs4 import BeautifulSoup
 import re
 import omdb
 
 
 # Project 1 Problem 1
```

### Comparing `python_course_by_ty-0.1.6/setup.py` & `python_course_by_ty-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python_course_by_ty",
-    version="0.1.6",
+    version="0.1.7",
     description="A package for testing student answers to project questions.",
     url="https://github.com/TyGriffiths/python_course_by_ty",
     author="Ty Griffiths",
     author_email="griffiths.ty@yahoo.com",
     license="GNU General Public License v3.0",
     packages=["python_course_by_ty"],
     install_requires=[
```

