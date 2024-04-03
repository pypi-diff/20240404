# Comparing `tmp/llmreader-0.2.2.tar.gz` & `tmp/llmreader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreader-0.2.2.tar", last modified: Wed Apr  3 22:21:32 2024, max compression
+gzip compressed data, was "llmreader-0.2.3.tar", last modified: Wed Apr  3 22:26:36 2024, max compression
```

## Comparing `llmreader-0.2.2.tar` & `llmreader-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:21:32.297964 llmreader-0.2.2/
--rw-r--r--   0 ethanhou   (501) staff       (20)     1068 2024-04-03 05:22:35.000000 llmreader-0.2.2/LICENSE
--rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-03 22:21:32.297835 llmreader-0.2.2/PKG-INFO
--rw-r--r--   0 ethanhou   (501) staff       (20)       56 2024-04-03 21:45:53.000000 llmreader-0.2.2/README.md
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:21:32.296625 llmreader-0.2.2/llmreader/
--rw-r--r--   0 ethanhou   (501) staff       (20)       41 2024-04-03 22:20:44.000000 llmreader-0.2.2/llmreader/__init__.py
--rw-r--r--   0 ethanhou   (501) staff       (20)      509 2024-04-03 22:21:15.000000 llmreader-0.2.2/llmreader/inject.py
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:21:32.297634 llmreader-0.2.2/llmreader.egg-info/
--rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-03 22:21:32.000000 llmreader-0.2.2/llmreader.egg-info/PKG-INFO
--rw-r--r--   0 ethanhou   (501) staff       (20)      232 2024-04-03 22:21:32.000000 llmreader-0.2.2/llmreader.egg-info/SOURCES.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-03 22:21:32.000000 llmreader-0.2.2/llmreader.egg-info/dependency_links.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)        7 2024-04-03 22:21:32.000000 llmreader-0.2.2/llmreader.egg-info/requires.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)       10 2024-04-03 22:21:32.000000 llmreader-0.2.2/llmreader.egg-info/top_level.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)       38 2024-04-03 22:21:32.298014 llmreader-0.2.2/setup.cfg
--rw-r--r--   0 ethanhou   (501) staff       (20)      532 2024-04-03 22:21:31.000000 llmreader-0.2.2/setup.py
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:26:36.894878 llmreader-0.2.3/
+-rw-r--r--   0 ethanhou   (501) staff       (20)     1068 2024-04-03 05:22:35.000000 llmreader-0.2.3/LICENSE
+-rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-03 22:26:36.894717 llmreader-0.2.3/PKG-INFO
+-rw-r--r--   0 ethanhou   (501) staff       (20)       56 2024-04-03 21:45:53.000000 llmreader-0.2.3/README.md
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:26:36.893442 llmreader-0.2.3/llmreader/
+-rw-r--r--   0 ethanhou   (501) staff       (20)       41 2024-04-03 22:20:44.000000 llmreader-0.2.3/llmreader/__init__.py
+-rw-r--r--   0 ethanhou   (501) staff       (20)      775 2024-04-03 22:24:28.000000 llmreader-0.2.3/llmreader/inject.py
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-03 22:26:36.894498 llmreader-0.2.3/llmreader.egg-info/
+-rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-03 22:26:36.000000 llmreader-0.2.3/llmreader.egg-info/PKG-INFO
+-rw-r--r--   0 ethanhou   (501) staff       (20)      232 2024-04-03 22:26:36.000000 llmreader-0.2.3/llmreader.egg-info/SOURCES.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-03 22:26:36.000000 llmreader-0.2.3/llmreader.egg-info/dependency_links.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        7 2024-04-03 22:26:36.000000 llmreader-0.2.3/llmreader.egg-info/requires.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)       10 2024-04-03 22:26:36.000000 llmreader-0.2.3/llmreader.egg-info/top_level.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)       38 2024-04-03 22:26:36.894926 llmreader-0.2.3/setup.cfg
+-rw-r--r--   0 ethanhou   (501) staff       (20)      532 2024-04-03 22:26:25.000000 llmreader-0.2.3/setup.py
```

### Comparing `llmreader-0.2.2/LICENSE` & `llmreader-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmreader-0.2.2/setup.py` & `llmreader-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="llmreader",
-    version="0.2.2",
+    version="0.2.3",
     description="Intercept OpenAI inputs",
     author="Ethan Hou",
     author_email="ethanfhou10@gmail.com",
     packages=find_packages(),
     install_requires=[
         'openai'
     ],
```

