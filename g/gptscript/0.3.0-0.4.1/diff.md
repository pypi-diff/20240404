# Comparing `tmp/gptscript-0.3.0.tar.gz` & `tmp/gptscript-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptscript-0.3.0.tar", last modified: Mon Apr  1 18:42:39 2024, max compression
+gzip compressed data, was "gptscript-0.4.1.tar", last modified: Thu Apr  4 04:01:09 2024, max compression
```

## Comparing `gptscript-0.3.0.tar` & `gptscript-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-01 18:42:39.200501 gptscript-0.3.0/
--rw-r--r--   0 wmaxwell   (501) staff       (20)    10175 2024-03-08 22:16:36.000000 gptscript-0.3.0/LICENSE
--rw-r--r--   0 wmaxwell   (501) staff       (20)    19246 2024-04-01 18:42:39.200240 gptscript-0.3.0/PKG-INFO
--rw-r--r--   0 wmaxwell   (501) staff       (20)     7032 2024-03-08 22:16:36.000000 gptscript-0.3.0/README.md
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-01 18:42:39.199283 gptscript-0.3.0/gptscript/
--rw-r--r--   0 wmaxwell   (501) staff       (20)        0 2024-03-08 22:16:36.000000 gptscript-0.3.0/gptscript/__init__.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     2782 2024-03-08 22:16:36.000000 gptscript-0.3.0/gptscript/command.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)      927 2024-03-08 22:16:36.000000 gptscript-0.3.0/gptscript/exec_utils.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     5452 2024-03-14 21:25:10.000000 gptscript-0.3.0/gptscript/install.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     1867 2024-04-01 18:37:22.000000 gptscript-0.3.0/gptscript/tool.py
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-01 18:42:39.200070 gptscript-0.3.0/gptscript.egg-info/
--rw-r--r--   0 wmaxwell   (501) staff       (20)    19246 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/PKG-INFO
--rw-r--r--   0 wmaxwell   (501) staff       (20)      362 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/SOURCES.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)        1 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/dependency_links.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       64 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/entry_points.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       99 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/requires.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       10 2024-04-01 18:42:39.000000 gptscript-0.3.0/gptscript.egg-info/top_level.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)      802 2024-04-01 18:37:22.000000 gptscript-0.3.0/pyproject.toml
--rw-r--r--   0 wmaxwell   (501) staff       (20)       38 2024-04-01 18:42:39.200533 gptscript-0.3.0/setup.cfg
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-01 18:42:39.199951 gptscript-0.3.0/tests/
--rw-r--r--   0 wmaxwell   (501) staff       (20)     3232 2024-03-08 22:16:36.000000 gptscript-0.3.0/tests/test_gptscript.py
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-04 04:01:09.632605 gptscript-0.4.1/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    10175 2024-03-08 22:16:36.000000 gptscript-0.4.1/LICENSE
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    19243 2024-04-04 04:01:09.632370 gptscript-0.4.1/PKG-INFO
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     7029 2024-04-04 03:59:06.000000 gptscript-0.4.1/README.md
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-04 04:01:09.631341 gptscript-0.4.1/gptscript/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)        0 2024-03-08 22:16:36.000000 gptscript-0.4.1/gptscript/__init__.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     2782 2024-03-08 22:16:36.000000 gptscript-0.4.1/gptscript/command.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      927 2024-03-08 22:16:36.000000 gptscript-0.4.1/gptscript/exec_utils.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     5452 2024-04-04 03:59:06.000000 gptscript-0.4.1/gptscript/install.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     1867 2024-04-01 18:37:22.000000 gptscript-0.4.1/gptscript/tool.py
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-04 04:01:09.632171 gptscript-0.4.1/gptscript.egg-info/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    19243 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/PKG-INFO
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      362 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/SOURCES.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)        1 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/dependency_links.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       64 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/entry_points.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       99 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/requires.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       10 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/top_level.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      802 2024-04-04 03:59:06.000000 gptscript-0.4.1/pyproject.toml
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       38 2024-04-04 04:01:09.632641 gptscript-0.4.1/setup.cfg
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-04 04:01:09.632022 gptscript-0.4.1/tests/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     3232 2024-03-08 22:16:36.000000 gptscript-0.4.1/tests/test_gptscript.py
```

### Comparing `gptscript-0.3.0/LICENSE` & `gptscript-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gptscript-0.3.0/PKG-INFO` & `gptscript-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptscript
-Version: 0.3.0
+Version: 0.4.1
 Summary: Run gptscripts from Python apps
 Author-email: Bill Maxwell <bill@acorn.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -253,15 +253,15 @@
 - `description`: A description of the tool.
 - `tools`: Additional tools associated with the main tool.
 - `max_tokens`: The maximum number of tokens to generate.
 - `model`: The GPT model to use.
 - `cache`: Whether to use caching for responses.
 - `temperature`: The temperature parameter for response generation.
 - `args`: Additional arguments for the tool.
-- `internal_prompt`: Internal prompt for the tool.
+- `internal_prompt`: Boolean defaults to false.
 - `instructions`: Instructions or additional information about the tool.
 - `json_response`: Whether the response should be in JSON format.(If you set this to True, you must say 'json' in the instructions as well.)
 
 ## Primary Functions
 
 Aside from the list methods there are `exec` and `exec_file` methods that allow you to execute a tool and get the responses. Those functions also provide a streaming version of execution if you want to process the output streams in your code as the tool is running.
```

### Comparing `gptscript-0.3.0/README.md` & `gptscript-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 - `description`: A description of the tool.
 - `tools`: Additional tools associated with the main tool.
 - `max_tokens`: The maximum number of tokens to generate.
 - `model`: The GPT model to use.
 - `cache`: Whether to use caching for responses.
 - `temperature`: The temperature parameter for response generation.
 - `args`: Additional arguments for the tool.
-- `internal_prompt`: Internal prompt for the tool.
+- `internal_prompt`: Boolean defaults to false.
 - `instructions`: Instructions or additional information about the tool.
 - `json_response`: Whether the response should be in JSON format.(If you set this to True, you must say 'json' in the instructions as well.)
 
 ## Primary Functions
 
 Aside from the list methods there are `exec` and `exec_file` methods that allow you to execute a tool and get the responses. Those functions also provide a streaming version of execution if you want to process the output streams in your code as the tool is running.
```

### Comparing `gptscript-0.3.0/gptscript/command.py` & `gptscript-0.4.1/gptscript/command.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.3.0/gptscript/exec_utils.py` & `gptscript-0.4.1/gptscript/exec_utils.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.3.0/gptscript/install.py` & `gptscript-0.4.1/gptscript/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # Handle other architectures or set a default/fallback
     arch = "unknown"
     print(f"Warning: Unhandled architecture '{machine}'. This may not be supported.")
 
 gptscript_info = {
     "name": "gptscript",
     "url": "https://github.com/gptscript-ai/gptscript/releases/download/",
-    "version": "v0.2.0",
+    "version": "v0.4.1",
 }
 
 pltfm = {"windows": "windows", "linux": "linux", "darwin": "macOS"}.get(
     platform_name, None
 )
 
 if platform_name == "darwin":
```

### Comparing `gptscript-0.3.0/gptscript/tool.py` & `gptscript-0.4.1/gptscript/tool.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.3.0/gptscript.egg-info/PKG-INFO` & `gptscript-0.4.1/gptscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptscript
-Version: 0.3.0
+Version: 0.4.1
 Summary: Run gptscripts from Python apps
 Author-email: Bill Maxwell <bill@acorn.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -253,15 +253,15 @@
 - `description`: A description of the tool.
 - `tools`: Additional tools associated with the main tool.
 - `max_tokens`: The maximum number of tokens to generate.
 - `model`: The GPT model to use.
 - `cache`: Whether to use caching for responses.
 - `temperature`: The temperature parameter for response generation.
 - `args`: Additional arguments for the tool.
-- `internal_prompt`: Internal prompt for the tool.
+- `internal_prompt`: Boolean defaults to false.
 - `instructions`: Instructions or additional information about the tool.
 - `json_response`: Whether the response should be in JSON format.(If you set this to True, you must say 'json' in the instructions as well.)
 
 ## Primary Functions
 
 Aside from the list methods there are `exec` and `exec_file` methods that allow you to execute a tool and get the responses. Those functions also provide a streaming version of execution if you want to process the output streams in your code as the tool is running.
```

### Comparing `gptscript-0.3.0/pyproject.toml` & `gptscript-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.9.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gptscript"
-version = "0.3.0"
+version = "0.4.1"
 description = "Run gptscripts from Python apps"
 readme = "README.md"
 authors = [{ name = "Bill Maxwell", email = "bill@acorn.io" }]
 license = { file = "LICENSE" }
 dependencies = [
     "certifi==2024.2.2",
     "charset-normalizer==3.3.2",
```

### Comparing `gptscript-0.3.0/tests/test_gptscript.py` & `gptscript-0.4.1/tests/test_gptscript.py`

 * *Files identical despite different names*

