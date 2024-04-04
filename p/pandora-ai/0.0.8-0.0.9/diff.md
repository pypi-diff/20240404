# Comparing `tmp/pandora_ai-0.0.8.tar.gz` & `tmp/pandora_ai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandora_ai-0.0.8.tar", last modified: Sun Jan 28 14:33:28 2024, max compression
+gzip compressed data, was "pandora_ai-0.0.9.tar", last modified: Mon Jan 29 20:28:37 2024, max compression
```

## Comparing `pandora_ai-0.0.8.tar` & `pandora_ai-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-01-28 14:33:28.645895 pandora_ai-0.0.8/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      761 2024-01-21 21:32:55.000000 pandora_ai-0.0.8/LICENSE
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4050 2024-01-28 14:33:28.645895 pandora_ai-0.0.8/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3231 2024-01-28 14:22:02.000000 pandora_ai-0.0.8/README.md
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-01-28 14:33:28.645895 pandora_ai-0.0.8/pandora_ai/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       94 2024-01-28 14:21:37.000000 pandora_ai-0.0.8/pandora_ai/__init__.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        2 2024-01-24 15:03:57.000000 pandora_ai-0.0.8/pandora_ai/config.json
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     7558 2024-01-21 17:10:31.000000 pandora_ai-0.0.8/pandora_ai/console.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    12399 2024-01-17 19:12:36.000000 pandora_ai-0.0.8/pandora_ai/get_text.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1420 2024-01-17 19:13:16.000000 pandora_ai-0.0.8/pandora_ai/get_webdriver.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    75489 2024-01-28 14:33:06.000000 pandora_ai-0.0.8/pandora_ai/pandora_agent.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3291 2024-01-05 15:16:55.000000 pandora_ai-0.0.8/pandora_ai/regex_tools.py
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-01-28 14:33:28.645895 pandora_ai-0.0.8/pandora_ai.egg-info/
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4050 2024-01-28 14:33:28.000000 pandora_ai-0.0.8/pandora_ai.egg-info/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      368 2024-01-28 14:33:28.000000 pandora_ai-0.0.8/pandora_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-01-28 14:33:28.000000 pandora_ai-0.0.8/pandora_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      141 2024-01-28 14:33:28.000000 pandora_ai-0.0.8/pandora_ai.egg-info/requires.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       11 2024-01-28 14:33:28.000000 pandora_ai-0.0.8/pandora_ai.egg-info/top_level.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-01-28 14:33:28.645895 pandora_ai-0.0.8/setup.cfg
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1102 2024-01-28 14:33:16.000000 pandora_ai-0.0.8/setup.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-01-29 20:28:37.323015 pandora_ai-0.0.9/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      761 2024-01-21 21:32:55.000000 pandora_ai-0.0.9/LICENSE
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       30 2024-01-29 20:18:58.000000 pandora_ai-0.0.9/MANIFEST.in
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4050 2024-01-29 20:28:37.319015 pandora_ai-0.0.9/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3231 2024-01-28 14:22:02.000000 pandora_ai-0.0.9/README.md
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-01-29 20:28:37.319015 pandora_ai-0.0.9/pandora_ai/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       94 2024-01-28 14:21:37.000000 pandora_ai-0.0.9/pandora_ai/__init__.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        2 2024-01-24 15:03:57.000000 pandora_ai-0.0.9/pandora_ai/config.json
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     7558 2024-01-21 17:10:31.000000 pandora_ai-0.0.9/pandora_ai/console.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    12399 2024-01-17 19:12:36.000000 pandora_ai-0.0.9/pandora_ai/get_text.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1420 2024-01-17 19:13:16.000000 pandora_ai-0.0.9/pandora_ai/get_webdriver.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    75489 2024-01-28 14:54:58.000000 pandora_ai-0.0.9/pandora_ai/pandora_agent.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3291 2024-01-05 15:16:55.000000 pandora_ai-0.0.9/pandora_ai/regex_tools.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-01-29 20:28:37.319015 pandora_ai-0.0.9/pandora_ai.egg-info/
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4050 2024-01-29 20:28:37.000000 pandora_ai-0.0.9/pandora_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      380 2024-01-29 20:28:37.000000 pandora_ai-0.0.9/pandora_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-01-29 20:28:37.000000 pandora_ai-0.0.9/pandora_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      141 2024-01-29 20:28:37.000000 pandora_ai-0.0.9/pandora_ai.egg-info/requires.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       11 2024-01-29 20:28:37.000000 pandora_ai-0.0.9/pandora_ai.egg-info/top_level.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-01-29 20:28:37.323015 pandora_ai-0.0.9/setup.cfg
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1102 2024-01-29 20:28:14.000000 pandora_ai-0.0.9/setup.py
```

### Comparing `pandora_ai-0.0.8/LICENSE` & `pandora_ai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandora_ai-0.0.8/PKG-INFO` & `pandora_ai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandora_ai
-Version: 0.0.8
+Version: 0.0.9
 Summary: GPT4-powered python interpreter / AI assistant
 Home-page: https://github.com/B4PT0R/pandora_ai
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `pandora_ai-0.0.8/README.md` & `pandora_ai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pandora_ai-0.0.8/pandora_ai/console.py` & `pandora_ai-0.0.9/pandora_ai/console.py`

 * *Files identical despite different names*

### Comparing `pandora_ai-0.0.8/pandora_ai/get_text.py` & `pandora_ai-0.0.9/pandora_ai/get_text.py`

 * *Files identical despite different names*

### Comparing `pandora_ai-0.0.8/pandora_ai/get_webdriver.py` & `pandora_ai-0.0.9/pandora_ai/get_webdriver.py`

 * *Files identical despite different names*

### Comparing `pandora_ai-0.0.8/pandora_ai/pandora_agent.py` & `pandora_ai-0.0.9/pandora_ai/pandora_agent.py`

 * *Files identical despite different names*

### Comparing `pandora_ai-0.0.8/pandora_ai/regex_tools.py` & `pandora_ai-0.0.9/pandora_ai/regex_tools.py`

 * *Files identical despite different names*

### Comparing `pandora_ai-0.0.8/pandora_ai.egg-info/PKG-INFO` & `pandora_ai-0.0.9/pandora_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandora_ai
-Version: 0.0.8
+Version: 0.0.9
 Summary: GPT4-powered python interpreter / AI assistant
 Home-page: https://github.com/B4PT0R/pandora_ai
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `pandora_ai-0.0.8/setup.py` & `pandora_ai-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pandora_ai",
-    version="0.0.8",
+    version="0.0.9",
     author="Baptiste Ferrand",
     author_email="bferrand.maths@gmail.com",
     description="GPT4-powered python interpreter / AI assistant",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/B4PT0R/pandora_ai",
     packages=setuptools.find_packages(),
```

