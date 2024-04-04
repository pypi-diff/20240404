# Comparing `tmp/TokenProbs-0.0.6.tar.gz` & `tmp/TokenProbs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TokenProbs-0.0.6.tar", last modified: Thu Apr  4 00:40:31 2024, max compression
+gzip compressed data, was "TokenProbs-0.0.7.tar", last modified: Thu Apr  4 00:45:24 2024, max compression
```

## Comparing `TokenProbs-0.0.6.tar` & `TokenProbs-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:40:31.352748 TokenProbs-0.0.6/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-0.0.6/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 00:40:31.352156 TokenProbs-0.0.6/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     2999 2024-04-02 20:06:10.000000 TokenProbs-0.0.6/README.md
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-04 00:40:31.352810 TokenProbs-0.0.6/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1194 2024-04-04 00:40:17.000000 TokenProbs-0.0.6/setup.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:40:31.347717 TokenProbs-0.0.6/src/
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:40:31.349579 TokenProbs-0.0.6/src/TokenProbs/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       73 2024-04-04 00:39:58.000000 TokenProbs-0.0.6/src/TokenProbs/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     8847 2024-04-02 22:14:09.000000 TokenProbs-0.0.6/src/TokenProbs/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:40:31.351701 TokenProbs-0.0.6/src/TokenProbs.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-04 00:40:30.000000 TokenProbs-0.0.6/src/TokenProbs.egg-info/top_level.txt
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:45:24.663127 TokenProbs-0.0.7/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-0.0.7/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 00:45:24.662609 TokenProbs-0.0.7/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     2999 2024-04-02 20:06:10.000000 TokenProbs-0.0.7/README.md
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-04 00:45:24.663198 TokenProbs-0.0.7/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1194 2024-04-04 00:45:11.000000 TokenProbs-0.0.7/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:45:24.658911 TokenProbs-0.0.7/src/
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:45:24.662159 TokenProbs-0.0.7/src/TokenProbs.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 00:45:24.660533 TokenProbs-0.0.7/src/TokenProbs.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      215 2024-04-04 00:45:24.660910 TokenProbs-0.0.7/src/TokenProbs.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-04 00:45:24.661362 TokenProbs-0.0.7/src/TokenProbs.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-04 00:45:24.661792 TokenProbs-0.0.7/src/TokenProbs.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-04 00:45:24.662225 TokenProbs-0.0.7/src/TokenProbs.egg-info/top_level.txt
```

### Comparing `TokenProbs-0.0.6/PKG-INFO` & `TokenProbs-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `TokenProbs-0.0.6/README.md` & `TokenProbs-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `TokenProbs-0.0.6/setup.py` & `TokenProbs-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities or other probability-based queries instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="TokenProbs",
     version=VERSION,
```

### Comparing `TokenProbs-0.0.6/src/TokenProbs.egg-info/PKG-INFO` & `TokenProbs-0.0.7/src/TokenProbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

