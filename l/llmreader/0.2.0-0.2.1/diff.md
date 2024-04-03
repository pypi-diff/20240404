# Comparing `tmp/llmreader-0.2.0.tar.gz` & `tmp/llmreader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreader-0.2.0.tar", last modified: Wed Apr  3 22:02:28 2024, max compression
+gzip compressed data, was "llmreader-0.2.1.tar", last modified: Wed Apr  3 22:18:07 2024, max compression
```

## Comparing `llmreader-0.2.0.tar` & `llmreader-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:02:28.490057 llmreader-0.2.0/
--rw-r--r--   0 ethanhou   (501) staff       (20)     1068 2024-04-03 05:22:35.000000 llmreader-0.2.0/LICENSE
--rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-03 22:02:28.489897 llmreader-0.2.0/PKG-INFO
--rw-r--r--   0 ethanhou   (501) staff       (20)       56 2024-04-03 21:45:53.000000 llmreader-0.2.0/README.md
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:02:28.488682 llmreader-0.2.0/llmreader.egg-info/
--rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-03 22:02:28.000000 llmreader-0.2.0/llmreader.egg-info/PKG-INFO
--rw-r--r--   0 ethanhou   (501) staff       (20)      212 2024-04-03 22:02:28.000000 llmreader-0.2.0/llmreader.egg-info/SOURCES.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-03 22:02:28.000000 llmreader-0.2.0/llmreader.egg-info/dependency_links.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)        4 2024-04-03 22:02:28.000000 llmreader-0.2.0/llmreader.egg-info/top_level.txt
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:02:28.489461 llmreader-0.2.0/pkg/
--rw-r--r--   0 ethanhou   (501) staff       (20)       34 2024-04-03 21:59:39.000000 llmreader-0.2.0/pkg/__init__.py
--rw-r--r--   0 ethanhou   (501) staff       (20)      788 2024-04-03 21:42:05.000000 llmreader-0.2.0/pkg/blume_injector.py
--rw-r--r--   0 ethanhou   (501) staff       (20)    11003 2024-04-03 20:08:18.000000 llmreader-0.2.0/pkg/injector.py
--rw-r--r--   0 ethanhou   (501) staff       (20)       38 2024-04-03 22:02:28.490102 llmreader-0.2.0/setup.cfg
--rw-r--r--   0 ethanhou   (501) staff       (20)      598 2024-04-03 22:01:52.000000 llmreader-0.2.0/setup.py
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:18:07.920896 llmreader-0.2.1/
+-rw-r--r--   0 ethanhou   (501) staff       (20)     1068 2024-04-03 05:22:35.000000 llmreader-0.2.1/LICENSE
+-rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-03 22:18:07.920742 llmreader-0.2.1/PKG-INFO
+-rw-r--r--   0 ethanhou   (501) staff       (20)       56 2024-04-03 21:45:53.000000 llmreader-0.2.1/README.md
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:18:07.920531 llmreader-0.2.1/llmreader.egg-info/
+-rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-03 22:18:07.000000 llmreader-0.2.1/llmreader.egg-info/PKG-INFO
+-rw-r--r--   0 ethanhou   (501) staff       (20)      190 2024-04-03 22:18:07.000000 llmreader-0.2.1/llmreader.egg-info/SOURCES.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-03 22:18:07.000000 llmreader-0.2.1/llmreader.egg-info/dependency_links.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        7 2024-04-03 22:18:07.000000 llmreader-0.2.1/llmreader.egg-info/requires.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-03 22:18:07.000000 llmreader-0.2.1/llmreader.egg-info/top_level.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)       38 2024-04-03 22:18:07.920941 llmreader-0.2.1/setup.cfg
+-rw-r--r--   0 ethanhou   (501) staff       (20)      532 2024-04-03 22:18:05.000000 llmreader-0.2.1/setup.py
```

### Comparing `llmreader-0.2.0/LICENSE` & `llmreader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmreader-0.2.0/setup.py` & `llmreader-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="llmreader",
-    version="0.2.0",
+    version="0.2.1",
     description="Intercept OpenAI inputs",
     author="Ethan Hou",
     author_email="ethanfhou10@gmail.com",
     packages=find_packages(),
     install_requires=[
-        # Add your package dependencies here
-        # e.g., 'requests >= 2.25.1',
+        'openai'
     ],
     classifiers=[
         # Trove classifiers
         # Full list at https://pypi.org/classifiers/
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

