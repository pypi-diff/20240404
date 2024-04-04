# Comparing `tmp/chatmemorydb-0.4.tar.gz` & `tmp/chatmemorydb-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatmemorydb-0.4.tar", last modified: Thu Feb 29 00:04:00 2024, max compression
+gzip compressed data, was "chatmemorydb-0.5.tar", last modified: Thu Apr  4 13:09:29 2024, max compression
```

## Comparing `chatmemorydb-0.4.tar` & `chatmemorydb-0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-29 00:04:00.827048 chatmemorydb-0.4/
--rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-21 19:11:21.000000 chatmemorydb-0.4/LICENSE
--rw-r--r--   0 moro      (1000) moro      (1000)     7449 2024-02-29 00:04:00.827048 chatmemorydb-0.4/PKG-INFO
--rw-r--r--   0 moro      (1000) moro      (1000)     6768 2024-02-28 22:04:17.000000 chatmemorydb-0.4/README.md
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-29 00:04:00.827048 chatmemorydb-0.4/chatmemorydb.egg-info/
--rw-r--r--   0 moro      (1000) moro      (1000)     7449 2024-02-29 00:04:00.000000 chatmemorydb-0.4/chatmemorydb.egg-info/PKG-INFO
--rw-r--r--   0 moro      (1000) moro      (1000)      442 2024-02-29 00:04:00.000000 chatmemorydb-0.4/chatmemorydb.egg-info/SOURCES.txt
--rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-02-29 00:04:00.000000 chatmemorydb-0.4/chatmemorydb.egg-info/dependency_links.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       82 2024-02-29 00:04:00.000000 chatmemorydb-0.4/chatmemorydb.egg-info/requires.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       13 2024-02-29 00:04:00.000000 chatmemorydb-0.4/chatmemorydb.egg-info/top_level.txt
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-29 00:04:00.827048 chatmemorydb-0.4/memory/
--rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-21 19:11:44.000000 chatmemorydb-0.4/memory/__init__.py
--rw-r--r--   0 moro      (1000) moro      (1000)    10056 2024-02-28 23:45:55.000000 chatmemorydb-0.4/memory/brain.py
--rw-r--r--   0 moro      (1000) moro      (1000)     1089 2024-02-22 15:52:05.000000 chatmemorydb-0.4/memory/embeddings.py
--rw-r--r--   0 moro      (1000) moro      (1000)      139 2024-02-21 19:37:35.000000 chatmemorydb-0.4/memory/log_util.py
--rw-r--r--   0 moro      (1000) moro      (1000)     2086 2024-02-22 19:48:44.000000 chatmemorydb-0.4/memory/summarization.py
--rwxrwxrwx   0 moro      (1000) moro      (1000)      650 2024-02-29 00:03:10.000000 chatmemorydb-0.4/pyproject.toml
--rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-02-29 00:04:00.827048 chatmemorydb-0.4/setup.cfg
--rwxrwxrwx   0 moro      (1000) moro      (1000)      668 2024-02-29 00:03:10.000000 chatmemorydb-0.4/setup.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-29 00:04:00.827048 chatmemorydb-0.4/tests/
--rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-21 23:22:48.000000 chatmemorydb-0.4/tests/__init__.py
--rw-r--r--   0 moro      (1000) moro      (1000)      418 2024-02-22 19:48:12.000000 chatmemorydb-0.4/tests/test_embedding_extraction.py
--rw-r--r--   0 moro      (1000) moro      (1000)      167 2024-02-21 23:23:40.000000 chatmemorydb-0.4/tests/test_logger.py
--rw-r--r--   0 moro      (1000) moro      (1000)    10772 2024-02-28 21:58:51.000000 chatmemorydb-0.4/tests/test_memory.py
--rw-r--r--   0 moro      (1000) moro      (1000)     2611 2024-02-22 19:48:34.000000 chatmemorydb-0.4/tests/test_summarization.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:09:29.912795 chatmemorydb-0.5/
+-rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-21 19:11:21.000000 chatmemorydb-0.5/LICENSE
+-rw-r--r--   0 moro      (1000) moro      (1000)     7441 2024-04-04 13:09:29.912795 chatmemorydb-0.5/PKG-INFO
+-rw-r--r--   0 moro      (1000) moro      (1000)     6768 2024-02-28 22:04:17.000000 chatmemorydb-0.5/README.md
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:09:29.912795 chatmemorydb-0.5/chatmemorydb.egg-info/
+-rw-r--r--   0 moro      (1000) moro      (1000)     7441 2024-04-04 13:09:29.000000 chatmemorydb-0.5/chatmemorydb.egg-info/PKG-INFO
+-rw-r--r--   0 moro      (1000) moro      (1000)      442 2024-04-04 13:09:29.000000 chatmemorydb-0.5/chatmemorydb.egg-info/SOURCES.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-04-04 13:09:29.000000 chatmemorydb-0.5/chatmemorydb.egg-info/dependency_links.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       74 2024-04-04 13:09:29.000000 chatmemorydb-0.5/chatmemorydb.egg-info/requires.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       13 2024-04-04 13:09:29.000000 chatmemorydb-0.5/chatmemorydb.egg-info/top_level.txt
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:09:29.912795 chatmemorydb-0.5/memory/
+-rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-21 19:11:44.000000 chatmemorydb-0.5/memory/__init__.py
+-rw-r--r--   0 moro      (1000) moro      (1000)    10056 2024-02-28 23:45:55.000000 chatmemorydb-0.5/memory/brain.py
+-rw-r--r--   0 moro      (1000) moro      (1000)     1089 2024-02-22 15:52:05.000000 chatmemorydb-0.5/memory/embeddings.py
+-rw-r--r--   0 moro      (1000) moro      (1000)      139 2024-02-21 19:37:35.000000 chatmemorydb-0.5/memory/log_util.py
+-rw-r--r--   0 moro      (1000) moro      (1000)     2086 2024-02-22 19:48:44.000000 chatmemorydb-0.5/memory/summarization.py
+-rwxrwxrwx   0 moro      (1000) moro      (1000)      642 2024-04-04 13:09:05.000000 chatmemorydb-0.5/pyproject.toml
+-rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-04-04 13:09:29.912795 chatmemorydb-0.5/setup.cfg
+-rwxrwxrwx   0 moro      (1000) moro      (1000)      660 2024-04-04 13:09:05.000000 chatmemorydb-0.5/setup.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:09:29.912795 chatmemorydb-0.5/tests/
+-rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-21 23:22:48.000000 chatmemorydb-0.5/tests/__init__.py
+-rw-r--r--   0 moro      (1000) moro      (1000)      418 2024-02-22 19:48:12.000000 chatmemorydb-0.5/tests/test_embedding_extraction.py
+-rw-r--r--   0 moro      (1000) moro      (1000)      167 2024-02-21 23:23:40.000000 chatmemorydb-0.5/tests/test_logger.py
+-rw-r--r--   0 moro      (1000) moro      (1000)    10772 2024-02-28 21:58:51.000000 chatmemorydb-0.5/tests/test_memory.py
+-rw-r--r--   0 moro      (1000) moro      (1000)     2611 2024-02-22 19:48:34.000000 chatmemorydb-0.5/tests/test_summarization.py
```

### Comparing `chatmemorydb-0.4/LICENSE` & `chatmemorydb-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.4/PKG-INFO` & `chatmemorydb-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: chatmemorydb
-Version: 0.4
+Version: 0.5
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro/ChatMemory
 Project-URL: Bug Tracker, https://github.com/cnmoro/ChatMemory/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mongita
 Requires-Dist: logzero
 Requires-Dist: sumy
 Requires-Dist: langdetect
-Requires-Dist: openai==1.12.0
+Requires-Dist: openai
 Requires-Dist: minivectordb
 Requires-Dist: text-util-en-pt
 Requires-Dist: numpy
 
 [![codecov](https://codecov.io/gh/cnmoro/ChatMemory/graph/badge.svg?token=B75N22ACYP)](https://codecov.io/gh/cnmoro/ChatMemory)
 
 [![Downloads](https://static.pepy.tech/badge/chatmemorydb)](https://pepy.tech/project/chatmemorydb)
```

### Comparing `chatmemorydb-0.4/README.md` & `chatmemorydb-0.5/README.md`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.4/chatmemorydb.egg-info/PKG-INFO` & `chatmemorydb-0.5/chatmemorydb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: chatmemorydb
-Version: 0.4
+Version: 0.5
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro/ChatMemory
 Project-URL: Bug Tracker, https://github.com/cnmoro/ChatMemory/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mongita
 Requires-Dist: logzero
 Requires-Dist: sumy
 Requires-Dist: langdetect
-Requires-Dist: openai==1.12.0
+Requires-Dist: openai
 Requires-Dist: minivectordb
 Requires-Dist: text-util-en-pt
 Requires-Dist: numpy
 
 [![codecov](https://codecov.io/gh/cnmoro/ChatMemory/graph/badge.svg?token=B75N22ACYP)](https://codecov.io/gh/cnmoro/ChatMemory)
 
 [![Downloads](https://static.pepy.tech/badge/chatmemorydb)](https://pepy.tech/project/chatmemorydb)
```

### Comparing `chatmemorydb-0.4/memory/brain.py` & `chatmemorydb-0.5/memory/brain.py`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.4/memory/embeddings.py` & `chatmemorydb-0.5/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.4/memory/summarization.py` & `chatmemorydb-0.5/memory/summarization.py`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.4/pyproject.toml` & `chatmemorydb-0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "mongita", "logzero", "sumy", "langdetect", "openai==1.12.0", "minivectordb", "text-util-en-pt", "numpy"]
+requires = ["setuptools>=61.0", "mongita", "logzero", "sumy", "langdetect", "openai", "minivectordb", "text-util-en-pt", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatmemorydb"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Carlo Moro", email="cnmoro@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chatmemorydb-0.4/setup.py` & `chatmemorydb-0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chatmemorydb',
-    version='0.4',
+    version='0.5',
     author='Carlo Moro',
     author_email='cnmoro@gmail.com',
     description="Memory",
     packages=find_packages(),
     package_data={
     },
     include_package_data=True,
     install_requires=[
         "mongita",
         "logzero",
         "sumy",
         "langdetect",
-        "openai==1.12.0",
+        "openai",
         "minivectordb",
         "text-util-en-pt",
         "numpy"
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

### Comparing `chatmemorydb-0.4/tests/test_memory.py` & `chatmemorydb-0.5/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.4/tests/test_summarization.py` & `chatmemorydb-0.5/tests/test_summarization.py`

 * *Files identical despite different names*

