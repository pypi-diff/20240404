# Comparing `tmp/composio_autogen-0.1.66.tar.gz` & `tmp/composio_autogen-0.1.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.66.tar", last modified: Tue Apr  2 18:40:21 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.67.tar", last modified: Thu Apr  4 16:51:04 2024, max compression
```

## Comparing `composio_autogen-0.1.66.tar` & `composio_autogen-0.1.67.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-02 18:40:21.429032 composio_autogen-0.1.66/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3309 2024-04-02 18:40:21.428844 composio_autogen-0.1.66/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.66/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-02 18:40:21.427615 composio_autogen-0.1.66/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.66/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     6977 2024-04-02 18:29:17.000000 composio_autogen-0.1.66/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-02 18:40:21.428654 composio_autogen-0.1.66/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3309 2024-04-02 18:40:21.000000 composio_autogen-0.1.66/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-02 18:40:21.000000 composio_autogen-0.1.66/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-02 18:40:21.000000 composio_autogen-0.1.66/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       42 2024-04-02 18:40:21.000000 composio_autogen-0.1.66/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-02 18:40:21.000000 composio_autogen-0.1.66/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-02 18:35:23.000000 composio_autogen-0.1.66/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-02 18:40:21.429082 composio_autogen-0.1.66/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-02 18:35:24.000000 composio_autogen-0.1.66/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-04 16:51:04.913329 composio_autogen-0.1.67/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3309 2024-04-04 16:51:04.913109 composio_autogen-0.1.67/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.67/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-04 16:51:04.911615 composio_autogen-0.1.67/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.67/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     6977 2024-04-04 16:49:33.000000 composio_autogen-0.1.67/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-04 16:51:04.912873 composio_autogen-0.1.67/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3309 2024-04-04 16:51:04.000000 composio_autogen-0.1.67/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-04 16:51:04.000000 composio_autogen-0.1.67/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-04 16:51:04.000000 composio_autogen-0.1.67/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       42 2024-04-04 16:51:04.000000 composio_autogen-0.1.67/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-04 16:51:04.000000 composio_autogen-0.1.67/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-04 16:50:01.000000 composio_autogen-0.1.67/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-04 16:51:04.913378 composio_autogen-0.1.67/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-04 16:50:01.000000 composio_autogen-0.1.67/setup.py
```

### Comparing `composio_autogen-0.1.66/PKG-INFO` & `composio_autogen-0.1.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.66
+Version: 0.1.67
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.66
+Requires-Dist: composio_core===0.1.67
 Requires-Dist: pyautogen===0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.66/README.md` & `composio_autogen-0.1.67/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.66/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.67/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.66/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.67/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.66
+Version: 0.1.67
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.66
+Requires-Dist: composio_core===0.1.67
 Requires-Dist: pyautogen===0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.66/setup.py` & `composio_autogen-0.1.67/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.66",
+    version="0.1.67",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

