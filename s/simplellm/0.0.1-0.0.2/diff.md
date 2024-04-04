# Comparing `tmp/simplellm-0.0.1.tar.gz` & `tmp/simplellm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplellm-0.0.1.tar", last modified: Thu Apr  4 11:48:43 2024, max compression
+gzip compressed data, was "simplellm-0.0.2.tar", last modified: Thu Apr  4 11:58:18 2024, max compression
```

## Comparing `simplellm-0.0.1.tar` & `simplellm-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:48:43.644306 simplellm-0.0.1/
--rw-rw-rw-   0        0        0     1093 2024-03-21 13:41:05.000000 simplellm-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      471 2024-04-04 11:48:43.643296 simplellm-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       46 2024-04-04 10:05:51.000000 simplellm-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 11:48:43.645287 simplellm-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      642 2024-04-04 11:43:25.000000 simplellm-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:48:43.603288 simplellm-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:48:43.611302 simplellm-0.0.1/src/simplellm/
--rw-rw-rw-   0        0        0        0 2024-04-04 10:41:18.000000 simplellm-0.0.1/src/simplellm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:48:43.629287 simplellm-0.0.1/src/simplellm/dataloaders/
--rw-rw-rw-   0        0        0       32 2024-04-04 10:37:04.000000 simplellm-0.0.1/src/simplellm/dataloaders/__init__.py
--rw-rw-rw-   0        0        0     2415 2024-04-04 11:43:06.000000 simplellm-0.0.1/src/simplellm/dataloaders/wikipedia_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:48:43.633288 simplellm-0.0.1/src/simplellm/gpt/
--rw-rw-rw-   0        0        0       71 2024-04-04 10:18:05.000000 simplellm-0.0.1/src/simplellm/gpt/__init__.py
--rw-rw-rw-   0        0        0     2652 2024-03-21 09:46:59.000000 simplellm-0.0.1/src/simplellm/gpt/gpt3.py
--rw-rw-rw-   0        0        0      931 2024-03-21 13:38:33.000000 simplellm-0.0.1/src/simplellm/gpt/gpt_trainer.py
--rw-rw-rw-   0        0        0     3053 2024-03-21 13:31:57.000000 simplellm-0.0.1/src/simplellm/gpt/gptbase.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:48:43.636286 simplellm-0.0.1/src/simplellm/llama/
--rw-rw-rw-   0        0        0       46 2024-04-04 10:18:28.000000 simplellm-0.0.1/src/simplellm/llama/__init__.py
--rw-rw-rw-   0        0        0     4769 2024-04-04 10:41:44.000000 simplellm-0.0.1/src/simplellm/llama/llama.py
--rw-rw-rw-   0        0        0     6977 2024-04-04 10:10:19.000000 simplellm-0.0.1/src/simplellm/llama/llamabase.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:48:43.639287 simplellm-0.0.1/src/simplellm/tokenizers/
--rw-rw-rw-   0        0        0       36 2024-04-04 11:13:15.000000 simplellm-0.0.1/src/simplellm/tokenizers/__init__.py
--rw-rw-rw-   0        0        0      785 2024-03-22 14:15:34.000000 simplellm-0.0.1/src/simplellm/tokenizers/abstracttokenizer.py
--rw-rw-rw-   0        0        0     1314 2024-04-04 11:45:43.000000 simplellm-0.0.1/src/simplellm/tokenizers/sptokenizer.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:48:43.642289 simplellm-0.0.1/src/simplellm.egg-info/
--rw-rw-rw-   0        0        0      471 2024-04-04 11:48:43.000000 simplellm-0.0.1/src/simplellm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      656 2024-04-04 11:48:43.000000 simplellm-0.0.1/src/simplellm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:48:43.000000 simplellm-0.0.1/src/simplellm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-04 11:48:43.000000 simplellm-0.0.1/src/simplellm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 11:48:43.000000 simplellm-0.0.1/src/simplellm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 11:58:18.161864 simplellm-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2024-03-21 13:41:05.000000 simplellm-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-04 11:58:18.160849 simplellm-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2024-04-04 11:56:32.000000 simplellm-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 11:58:18.162849 simplellm-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      645 2024-04-04 11:57:29.000000 simplellm-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:58:18.112849 simplellm-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 11:58:18.125846 simplellm-0.0.2/src/simplellm/
+-rw-rw-rw-   0        0        0        0 2024-04-04 10:41:18.000000 simplellm-0.0.2/src/simplellm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:58:18.147848 simplellm-0.0.2/src/simplellm/dataloaders/
+-rw-rw-rw-   0        0        0       32 2024-04-04 10:37:04.000000 simplellm-0.0.2/src/simplellm/dataloaders/__init__.py
+-rw-rw-rw-   0        0        0     2415 2024-04-04 11:43:06.000000 simplellm-0.0.2/src/simplellm/dataloaders/wikipedia_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:58:18.150847 simplellm-0.0.2/src/simplellm/gpt/
+-rw-rw-rw-   0        0        0       71 2024-04-04 10:18:05.000000 simplellm-0.0.2/src/simplellm/gpt/__init__.py
+-rw-rw-rw-   0        0        0     2652 2024-03-21 09:46:59.000000 simplellm-0.0.2/src/simplellm/gpt/gpt3.py
+-rw-rw-rw-   0        0        0      931 2024-03-21 13:38:33.000000 simplellm-0.0.2/src/simplellm/gpt/gpt_trainer.py
+-rw-rw-rw-   0        0        0     3053 2024-03-21 13:31:57.000000 simplellm-0.0.2/src/simplellm/gpt/gptbase.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:58:18.154847 simplellm-0.0.2/src/simplellm/llama/
+-rw-rw-rw-   0        0        0       46 2024-04-04 10:18:28.000000 simplellm-0.0.2/src/simplellm/llama/__init__.py
+-rw-rw-rw-   0        0        0     4769 2024-04-04 10:41:44.000000 simplellm-0.0.2/src/simplellm/llama/llama.py
+-rw-rw-rw-   0        0        0     6977 2024-04-04 10:10:19.000000 simplellm-0.0.2/src/simplellm/llama/llamabase.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:58:18.157846 simplellm-0.0.2/src/simplellm/tokenizers/
+-rw-rw-rw-   0        0        0       36 2024-04-04 11:13:15.000000 simplellm-0.0.2/src/simplellm/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0      785 2024-03-22 14:15:34.000000 simplellm-0.0.2/src/simplellm/tokenizers/abstracttokenizer.py
+-rw-rw-rw-   0        0        0     1314 2024-04-04 11:45:43.000000 simplellm-0.0.2/src/simplellm/tokenizers/sptokenizer.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:58:18.158848 simplellm-0.0.2/src/simplellm.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-04 11:58:18.000000 simplellm-0.0.2/src/simplellm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      656 2024-04-04 11:58:18.000000 simplellm-0.0.2/src/simplellm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 11:58:18.000000 simplellm-0.0.2/src/simplellm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-04 11:58:18.000000 simplellm-0.0.2/src/simplellm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 11:58:18.000000 simplellm-0.0.2/src/simplellm.egg-info/top_level.txt
```

### Comparing `simplellm-0.0.1/LICENSE` & `simplellm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/setup.py` & `simplellm-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='simplellm',
-    version='0.0.1',    
+    version='0.0.2',    
     description='Build LLMs easily',
-    url='https://github.com/NikolayBlagoev/ez-llm',
+    url='https://github.com/NikolayBlagoev/simplellm',
     author='Nikolay Blagoev',
     author_email='nickyblagoev@gmail.com',
     license='MIT License',
     install_requires=['datasets',
                       'torch',
                       'sentencepiece'                     
                       ],
```

### Comparing `simplellm-0.0.1/src/simplellm/dataloaders/wikipedia_dataset.py` & `simplellm-0.0.2/src/simplellm/dataloaders/wikipedia_dataset.py`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/src/simplellm/gpt/gpt3.py` & `simplellm-0.0.2/src/simplellm/gpt/gpt3.py`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/src/simplellm/gpt/gpt_trainer.py` & `simplellm-0.0.2/src/simplellm/gpt/gpt_trainer.py`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/src/simplellm/gpt/gptbase.py` & `simplellm-0.0.2/src/simplellm/gpt/gptbase.py`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/src/simplellm/llama/llama.py` & `simplellm-0.0.2/src/simplellm/llama/llama.py`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/src/simplellm/llama/llamabase.py` & `simplellm-0.0.2/src/simplellm/llama/llamabase.py`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/src/simplellm/tokenizers/abstracttokenizer.py` & `simplellm-0.0.2/src/simplellm/tokenizers/abstracttokenizer.py`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/src/simplellm/tokenizers/sptokenizer.py` & `simplellm-0.0.2/src/simplellm/tokenizers/sptokenizer.py`

 * *Files identical despite different names*

### Comparing `simplellm-0.0.1/src/simplellm.egg-info/SOURCES.txt` & `simplellm-0.0.2/src/simplellm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

