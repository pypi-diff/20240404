# Comparing `tmp/sirji-tools-0.0.3.tar.gz` & `tmp/sirji-tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-tools-0.0.3.tar", last modified: Thu Apr  4 05:56:51 2024, max compression
+gzip compressed data, was "sirji-tools-0.0.4.tar", last modified: Thu Apr  4 13:10:02 2024, max compression
```

## Comparing `sirji-tools-0.0.3.tar` & `sirji-tools-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.734535 sirji-tools-0.0.3/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1523 2024-04-04 05:56:51.733370 sirji-tools-0.0.3/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1144 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 05:56:51.734798 sirji-tools-0.0.3/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      652 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.715478 sirji-tools-0.0.3/sirji_tools/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.719955 sirji-tools-0.0.3/sirji_tools/config/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/config/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/config/config_loader.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.725445 sirji-tools-0.0.3/sirji_tools/crawler/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/github_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/crawler/web_page_handler.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.727276 sirji-tools-0.0.3/sirji_tools/logger/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/logger/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3587 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/logger/logger.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.728665 sirji-tools-0.0.3/sirji_tools/search/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/search/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/sirji_tools/search/search.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.732336 sirji-tools-0.0.3/sirji_tools.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1523 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-04 05:56:51.000000 sirji-tools-0.0.3/sirji_tools.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:56:51.731514 sirji-tools-0.0.3/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/tests/test_crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/tests/test_logger.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/tests/test_pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-04 05:56:30.000000 sirji-tools-0.0.3/tests/test_search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.016637 sirji-tools-0.0.4/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1614 2024-04-04 13:10:02.015834 sirji-tools-0.0.4/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1222 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 13:10:02.016820 sirji-tools-0.0.4/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      671 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.000570 sirji-tools-0.0.4/sirji_tools/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.004395 sirji-tools-0.0.4/sirji_tools/config/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/config/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/config/config_loader.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.008957 sirji-tools-0.0.4/sirji_tools/crawler/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/github_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/crawler/web_page_handler.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.010009 sirji-tools-0.0.4/sirji_tools/logger/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/logger/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3587 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/logger/logger.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.011130 sirji-tools-0.0.4/sirji_tools/search/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/search/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/sirji_tools/search/search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.014963 sirji-tools-0.0.4/sirji_tools.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1614 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-04 13:10:01.000000 sirji-tools-0.0.4/sirji_tools.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:02.014003 sirji-tools-0.0.4/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/tests/test_crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/tests/test_logger.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/tests/test_pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-04 13:09:44.000000 sirji-tools-0.0.4/tests/test_search.py
```

### Comparing `sirji-tools-0.0.3/LICENSE` & `sirji-tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/PKG-INFO` & `sirji-tools-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
+License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: pypdf2==3.0.1
 Requires-Dist: markdownify==0.11.6
 Requires-Dist: playwright==1.42.0
 
 # sirji-tools
 
-`sirji-tools` is a Python package.
+`sirji-tools` is a PyPI package that provides tools for:
 
-## Installation
+- Crawling (downloading web pages to markdown files)
+- Searching (using the Google Search API for search results)
+- Custom Logging
 
-Install `sirji-tools` quickly with pip:
+## Installation
 
 ```
 pip install sirji-tools
 ```
 
 ## Usage
 
-### Crawl URLs 
+### Crawl URLs
 
 Crawl URLs tool will be used to crawl the web pages and extract the information from the web pages. And store the information for the further processing by researcher.
 
 ```python
 from sirji_tools import crawl_urls
 
 urls = ['https://www.google.com', 'https://www.yahoo.com']
 
 crawl_urls(urls, 'workspace/researcher')
 ```
 
-### Search 
+### Search
 
-Search tool will be used to search the information from the web pages based on the search terms provided. 
+Search tool will be used to search the information from the web pages based on the search terms provided.
 It returns the list of URLs related to the search terms.
 
 ```python
 from sirji_tools import search_for
 
 search_term = 'python programming'
 
@@ -59,8 +62,8 @@
 from sirji_tools.logger import p_logger
 
 p_logger.info("Log line here")
 ```
 
 ## License
 
-`sirji-tools` is made available under the MIT License. See the included LICENSE file for more details.
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `sirji-tools-0.0.3/README.md` & `sirji-tools-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # sirji-tools
 
-`sirji-tools` is a Python package.
+`sirji-tools` is a PyPI package that provides tools for:
 
-## Installation
+- Crawling (downloading web pages to markdown files)
+- Searching (using the Google Search API for search results)
+- Custom Logging
 
-Install `sirji-tools` quickly with pip:
+## Installation
 
 ```
 pip install sirji-tools
 ```
 
 ## Usage
 
-### Crawl URLs 
+### Crawl URLs
 
 Crawl URLs tool will be used to crawl the web pages and extract the information from the web pages. And store the information for the further processing by researcher.
 
 ```python
 from sirji_tools import crawl_urls
 
 urls = ['https://www.google.com', 'https://www.yahoo.com']
 
 crawl_urls(urls, 'workspace/researcher')
 ```
 
-### Search 
+### Search
 
-Search tool will be used to search the information from the web pages based on the search terms provided. 
+Search tool will be used to search the information from the web pages based on the search terms provided.
 It returns the list of URLs related to the search terms.
 
 ```python
 from sirji_tools import search_for
 
 search_term = 'python programming'
 
@@ -45,8 +47,8 @@
 from sirji_tools.logger import p_logger
 
 p_logger.info("Log line here")
 ```
 
 ## License
 
-`sirji-tools` is made available under the MIT License. See the included LICENSE file for more details.
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `sirji-tools-0.0.3/setup.py` & `sirji-tools-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-tools',
-    version='0.0.3',
+    version='0.0.4',
     author='Sirji',
     description='Crawler and search tools used by Sirji.',
+    license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
     include_package_data=True,  # This includes non-code files specified in MANIFEST.in
     install_requires=[
         x for x in open("./requirements.txt", "r+").readlines() if x.strip()
```

### Comparing `sirji-tools-0.0.3/sirji_tools/crawler/base.py` & `sirji-tools-0.0.4/sirji_tools/crawler/base.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/sirji_tools/crawler/crawler.py` & `sirji-tools-0.0.4/sirji_tools/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/sirji_tools/crawler/factory.py` & `sirji-tools-0.0.4/sirji_tools/crawler/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/sirji_tools/crawler/github_handler.py` & `sirji-tools-0.0.4/sirji_tools/crawler/github_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/sirji_tools/crawler/pdf_handler.py` & `sirji-tools-0.0.4/sirji_tools/crawler/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/sirji_tools/crawler/web_page_handler.py` & `sirji-tools-0.0.4/sirji_tools/crawler/web_page_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/sirji_tools/logger/logger.py` & `sirji-tools-0.0.4/sirji_tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/sirji_tools/search/search.py` & `sirji-tools-0.0.4/sirji_tools/search/search.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/sirji_tools.egg-info/PKG-INFO` & `sirji-tools-0.0.4/sirji_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
+License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: pypdf2==3.0.1
 Requires-Dist: markdownify==0.11.6
 Requires-Dist: playwright==1.42.0
 
 # sirji-tools
 
-`sirji-tools` is a Python package.
+`sirji-tools` is a PyPI package that provides tools for:
 
-## Installation
+- Crawling (downloading web pages to markdown files)
+- Searching (using the Google Search API for search results)
+- Custom Logging
 
-Install `sirji-tools` quickly with pip:
+## Installation
 
 ```
 pip install sirji-tools
 ```
 
 ## Usage
 
-### Crawl URLs 
+### Crawl URLs
 
 Crawl URLs tool will be used to crawl the web pages and extract the information from the web pages. And store the information for the further processing by researcher.
 
 ```python
 from sirji_tools import crawl_urls
 
 urls = ['https://www.google.com', 'https://www.yahoo.com']
 
 crawl_urls(urls, 'workspace/researcher')
 ```
 
-### Search 
+### Search
 
-Search tool will be used to search the information from the web pages based on the search terms provided. 
+Search tool will be used to search the information from the web pages based on the search terms provided.
 It returns the list of URLs related to the search terms.
 
 ```python
 from sirji_tools import search_for
 
 search_term = 'python programming'
 
@@ -59,8 +62,8 @@
 from sirji_tools.logger import p_logger
 
 p_logger.info("Log line here")
 ```
 
 ## License
 
-`sirji-tools` is made available under the MIT License. See the included LICENSE file for more details.
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `sirji-tools-0.0.3/sirji_tools.egg-info/SOURCES.txt` & `sirji-tools-0.0.4/sirji_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/tests/test_crawler.py` & `sirji-tools-0.0.4/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/tests/test_logger.py` & `sirji-tools-0.0.4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/tests/test_pdf_handler.py` & `sirji-tools-0.0.4/tests/test_pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.3/tests/test_search.py` & `sirji-tools-0.0.4/tests/test_search.py`

 * *Files identical despite different names*

