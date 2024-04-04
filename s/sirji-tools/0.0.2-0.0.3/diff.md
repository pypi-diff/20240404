# Comparing `tmp/sirji-tools-0.0.2.tar.gz` & `tmp/sirji-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-tools-0.0.2.tar", last modified: Wed Apr  3 15:13:08 2024, max compression
+gzip compressed data, was "sirji-tools-0.0.3.tar", last modified: Thu Apr  4 05:56:51 2024, max compression
```

## Comparing `sirji-tools-0.0.2.tar` & `sirji-tools-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.560917 sirji-tools-0.0.2/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1523 2024-04-03 15:13:08.560434 sirji-tools-0.0.2/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1144 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-03 15:13:08.561033 sirji-tools-0.0.2/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      652 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.546487 sirji-tools-0.0.2/sirji_tools/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.549517 sirji-tools-0.0.2/sirji_tools/config/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/config/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/config/config_loader.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.554158 sirji-tools-0.0.2/sirji_tools/crawler/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/github_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/web_page_handler.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.555640 sirji-tools-0.0.2/sirji_tools/logger/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/logger/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3306 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/logger/logger.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.556996 sirji-tools-0.0.2/sirji_tools/search/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/search/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/search/search.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.559866 sirji-tools-0.0.2/sirji_tools.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1523 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.559175 sirji-tools-0.0.2/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/tests/test_crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/tests/test_logger.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/tests/test_pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/tests/test_search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.734535 sirji-tools-0.0.3/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1523 2024-04-04 05:56:51.733370 sirji-tools-0.0.3/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1144 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 05:56:51.734798 sirji-tools-0.0.3/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      652 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.715478 sirji-tools-0.0.3/sirji_tools/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.719955 sirji-tools-0.0.3/sirji_tools/config/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/config/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/config/config_loader.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.725445 sirji-tools-0.0.3/sirji_tools/crawler/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/github_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/web_page_handler.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.727276 sirji-tools-0.0.3/sirji_tools/logger/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/logger/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3587 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/logger/logger.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.728665 sirji-tools-0.0.3/sirji_tools/search/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/search/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/search/search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.732336 sirji-tools-0.0.3/sirji_tools.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1523 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.731514 sirji-tools-0.0.3/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/tests/test_crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/tests/test_logger.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/tests/test_pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/tests/test_search.py
```

### Comparing `sirji-tools-0.0.2/LICENSE` & `sirji-tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/PKG-INFO` & `sirji-tools-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
```

### Comparing `sirji-tools-0.0.2/README.md` & `sirji-tools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/setup.py` & `sirji-tools-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-tools',
-    version='0.0.2',
+    version='0.0.3',
     author='Sirji',
     description='Crawler and search tools used by Sirji.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
     include_package_data=True,  # This includes non-code files specified in MANIFEST.in
```

### Comparing `sirji-tools-0.0.2/sirji_tools/crawler/base.py` & `sirji-tools-0.0.3/sirji_tools/crawler/base.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/sirji_tools/crawler/crawler.py` & `sirji-tools-0.0.3/sirji_tools/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/sirji_tools/crawler/factory.py` & `sirji-tools-0.0.3/sirji_tools/crawler/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/sirji_tools/crawler/github_handler.py` & `sirji-tools-0.0.3/sirji_tools/crawler/github_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/sirji_tools/crawler/pdf_handler.py` & `sirji-tools-0.0.3/sirji_tools/crawler/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/sirji_tools/crawler/web_page_handler.py` & `sirji-tools-0.0.3/sirji_tools/crawler/web_page_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/sirji_tools/logger/logger.py` & `sirji-tools-0.0.3/sirji_tools/logger/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,22 @@
 # Singleton class to create loggers
 class LoggerSingleton:
 
     def __init__(self, file_name, log_level):
         self.logger = self._setup_logger(file_name, log_level)
     
     def _log_folder(self):
-        return os.path.join("workspace", "logs")
+        return os.path.join(self._get_workspace_folder(), '.sirji', "logs")
+    
+    def _get_workspace_folder(self):
+        workspace = os.environ.get("SIRJI_WORKSPACE")
+        if workspace is None:
+            raise ValueError(
+                "SIRJI_WORKSPACE is not set as an environment variable")
+        return workspace
     
     def _log_file_path(self, file_name):
         return os.path.join(self._log_folder(), file_name)
         
     def _setup_logger(self, file_name, log_level):
         # Create a folder named "logs" if it doesn't exist
         if not os.path.exists(self._log_folder()):
```

### Comparing `sirji-tools-0.0.2/sirji_tools/search/search.py` & `sirji-tools-0.0.3/sirji_tools/search/search.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/sirji_tools.egg-info/PKG-INFO` & `sirji-tools-0.0.3/sirji_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
```

### Comparing `sirji-tools-0.0.2/sirji_tools.egg-info/SOURCES.txt` & `sirji-tools-0.0.3/sirji_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/tests/test_crawler.py` & `sirji-tools-0.0.3/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/tests/test_logger.py` & `sirji-tools-0.0.3/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/tests/test_pdf_handler.py` & `sirji-tools-0.0.3/tests/test_pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.2/tests/test_search.py` & `sirji-tools-0.0.3/tests/test_search.py`

 * *Files identical despite different names*

