# Comparing `tmp/webtextcrawler-1.0.1.tar.gz` & `tmp/webtextcrawler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webtextcrawler-1.0.1.tar", last modified: Tue Feb 13 17:42:54 2024, max compression
+gzip compressed data, was "webtextcrawler-1.0.2.tar", last modified: Thu Apr  4 18:08:54 2024, max compression
```

## Comparing `webtextcrawler-1.0.1.tar` & `webtextcrawler-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-13 17:42:54.691544 webtextcrawler-1.0.1/
--rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-13 13:58:03.000000 webtextcrawler-1.0.1/LICENSE
--rw-r--r--   0 moro      (1000) moro      (1000)      519 2024-02-13 17:42:54.691544 webtextcrawler-1.0.1/PKG-INFO
--rwxrwxrwx   0 moro      (1000) moro      (1000)      629 2024-02-13 17:42:49.000000 webtextcrawler-1.0.1/pyproject.toml
--rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-02-13 17:42:54.691544 webtextcrawler-1.0.1/setup.cfg
--rw-r--r--   0 moro      (1000) moro      (1000)      685 2024-02-13 17:42:49.000000 webtextcrawler-1.0.1/setup.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-13 17:42:54.691544 webtextcrawler-1.0.1/webtextcrawler/
--rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-13 13:58:54.000000 webtextcrawler-1.0.1/webtextcrawler/__init__.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-13 17:42:54.691544 webtextcrawler-1.0.1/webtextcrawler/resources/
--rw-r--r--   0 moro      (1000) moro      (1000)     1144 2024-02-13 13:59:13.000000 webtextcrawler-1.0.1/webtextcrawler/resources/language_mapping.pkl
--rw-r--r--   0 moro      (1000) moro      (1000)     3615 2024-02-13 14:01:57.000000 webtextcrawler-1.0.1/webtextcrawler/webtextcrawler.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-13 17:42:54.691544 webtextcrawler-1.0.1/webtextcrawler.egg-info/
--rw-r--r--   0 moro      (1000) moro      (1000)      519 2024-02-13 17:42:54.000000 webtextcrawler-1.0.1/webtextcrawler.egg-info/PKG-INFO
--rw-r--r--   0 moro      (1000) moro      (1000)      326 2024-02-13 17:42:54.000000 webtextcrawler-1.0.1/webtextcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-02-13 17:42:54.000000 webtextcrawler-1.0.1/webtextcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       43 2024-02-13 17:42:54.000000 webtextcrawler-1.0.1/webtextcrawler.egg-info/requires.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       15 2024-02-13 17:42:54.000000 webtextcrawler-1.0.1/webtextcrawler.egg-info/top_level.txt
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 18:08:54.729307 webtextcrawler-1.0.2/
+-rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-13 13:58:03.000000 webtextcrawler-1.0.2/LICENSE
+-rw-r--r--   0 moro      (1000) moro      (1000)      519 2024-04-04 18:08:54.729307 webtextcrawler-1.0.2/PKG-INFO
+-rwxrwxrwx   0 moro      (1000) moro      (1000)      629 2024-04-04 18:08:15.000000 webtextcrawler-1.0.2/pyproject.toml
+-rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-04-04 18:08:54.729307 webtextcrawler-1.0.2/setup.cfg
+-rw-r--r--   0 moro      (1000) moro      (1000)      685 2024-04-04 18:08:25.000000 webtextcrawler-1.0.2/setup.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 18:08:54.729307 webtextcrawler-1.0.2/webtextcrawler/
+-rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-13 13:58:54.000000 webtextcrawler-1.0.2/webtextcrawler/__init__.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 18:08:54.729307 webtextcrawler-1.0.2/webtextcrawler/resources/
+-rw-r--r--   0 moro      (1000) moro      (1000)     1144 2024-02-13 13:59:13.000000 webtextcrawler-1.0.2/webtextcrawler/resources/language_mapping.pkl
+-rw-r--r--   0 moro      (1000) moro      (1000)     4768 2024-04-04 15:36:09.000000 webtextcrawler-1.0.2/webtextcrawler/webtextcrawler.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 18:08:54.729307 webtextcrawler-1.0.2/webtextcrawler.egg-info/
+-rw-r--r--   0 moro      (1000) moro      (1000)      519 2024-04-04 18:08:54.000000 webtextcrawler-1.0.2/webtextcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 moro      (1000) moro      (1000)      326 2024-04-04 18:08:54.000000 webtextcrawler-1.0.2/webtextcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-04-04 18:08:54.000000 webtextcrawler-1.0.2/webtextcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       43 2024-04-04 18:08:54.000000 webtextcrawler-1.0.2/webtextcrawler.egg-info/requires.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       15 2024-04-04 18:08:54.000000 webtextcrawler-1.0.2/webtextcrawler.egg-info/top_level.txt
```

### Comparing `webtextcrawler-1.0.1/LICENSE` & `webtextcrawler-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webtextcrawler-1.0.1/PKG-INFO` & `webtextcrawler-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webtextcrawler
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python project for crawling the web and extracting text.
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro
 Project-URL: Bug Tracker, https://github.com/cnmoro
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `webtextcrawler-1.0.1/pyproject.toml` & `webtextcrawler-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "langdetect", "beautifulsoup4", "requests", "justext"]
+requires = ["setuptools>=61.0", "langdetect", "beautifulsoup4", "requests", "jusText"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webtextcrawler"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Carlo Moro", email="cnmoro@gmail.com" },
 ]
 description = "Python project for crawling the web and extracting text."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `webtextcrawler-1.0.1/setup.py` & `webtextcrawler-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webtextcrawler',
-    version='1.0.1',
+    version='1.0.2',
     author='Carlo Moro',
     author_email='cnmoro@gmail.com',
     description="Python project for crawling the web and extracting text.",
     packages=find_packages(),
     package_data={
         'webtextcrawler': [
             'resources/language_mapping.pkl',
         ]
     },
     include_package_data=True,
-    install_requires=["langdetect", "beautifulsoup4", "requests", "justext"],
+    install_requires=["langdetect", "beautifulsoup4", "requests", "jusText"],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7',
 )
```

### Comparing `webtextcrawler-1.0.1/webtextcrawler/resources/language_mapping.pkl` & `webtextcrawler-1.0.2/webtextcrawler/resources/language_mapping.pkl`

 * *Files identical despite different names*

### Comparing `webtextcrawler-1.0.1/webtextcrawler/webtextcrawler.py` & `webtextcrawler-1.0.2/webtextcrawler/webtextcrawler.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,33 +22,39 @@
     return language_mapping.get(raw_lang, '')
 
 def is_valid(url):
     parsed = urlparse(url)
     return bool(parsed.netloc) and bool(parsed.scheme)
 
 def fetch_all_website_links(url, visited):
-    urls = set()
-    domain_name = urlparse(url).netloc
-    soup = BeautifulSoup(requests.get(url, timeout=60).content, "html.parser")
-
-    for a_tag in soup.findAll("a"):
-        href = a_tag.attrs.get("href")
-        if href == "" or href is None:
-            continue
-        href = urljoin(url, href)
-        parsed_href = urlparse(href)
-        href = parsed_href.scheme + "://" + parsed_href.netloc + parsed_href.path
-        if not is_valid(href):
-            continue
-        if href in visited:
-            continue
-        if domain_name not in href:
-            continue
-        urls.add(href)
-    return urls
+    try:
+        urls = set()
+        domain_name = urlparse(url).netloc
+        soup = BeautifulSoup(requests.get(url, timeout=60).content, "html.parser")
+
+        for a_tag in soup.findAll("a"):
+            href = a_tag.attrs.get("href")
+            if href == "" or href is None:
+                continue
+            href = urljoin(url, href)
+            parsed_href = urlparse(href)
+            href = parsed_href.scheme + "://" + parsed_href.netloc + parsed_href.path
+            if not is_valid(href):
+                continue
+            if href in visited:
+                continue
+            if domain_name not in href:
+                continue
+            urls.add(href)
+        
+        urls = [url for url in urls if 'mailto:' not in url and 'tel:' not in url]
+        urls = [url.rstrip('/') for url in urls]
+        return urls
+    except Exception:
+        return []
 
 def extract_text_from_website(url):
     try:
         response = requests.get(url)
         paragraphs = justext.justext(
             html_text = response.content,
             stoplist = '',
@@ -74,54 +80,78 @@
         return ' '.join(final_paragraphs)
     
     except Exception:
         traceback.print_exc()
     
     return ''
 
-def crawl(url, visited=None, max_depth=4):
+def crawl(url, visited=None, max_depth=1, get_links_only=False):
     try:
-        if max_depth == 1:
-            return extract_text_from_website(url)
-        
+        max_depth -= 1
+        if max_depth < 0:
+            max_depth = 0
+
         if visited is None:
-            visited = set()
+            visited = {}
 
         stack = [(url, 0)] # each item in stack is a tuple (url, depth)
         sentences = []
 
         while stack:
             url, depth = stack.pop()
             
-            if len(sentences) > max_depth:
+            if get_links_only and len(visited) >= max_depth:
+
+                # Add back the current url to the stack
+                stack.append((url, depth))
+
+                # Return the first max_depth links
+                # Keeping the "visited" in the return list
+                result = {**visited, **{url: depth for url, depth in stack}}
+
+                # Return the first "max_depth" links
+                return {"links": [{"url": k, "depth": v} for k, v in list(result.items())]}    
+
+            if len(sentences) > max_depth and not get_links_only:
                 break
 
-            if depth > max_depth or url in visited:
+            if depth > max_depth or url in [ k for k, v in visited.items()]:
                 continue
 
-            visited.add(url)
+            visited[url] = depth
 
-            current_sentences = extract_text_from_website(url)
+            if not get_links_only:
+                current_sentences = extract_text_from_website(url)
+
+                if current_sentences:
+                    sentences.append(current_sentences)
 
-            if current_sentences:
-                sentences.append(current_sentences)
-            
             # call crawl recursively to all the internal links
             links = fetch_all_website_links(url, visited)
 
             for link in links:
                 if f'{url} htt' in link:
                     link = link.replace(f'{url} http', 'http')
-                if link not in visited:
+                if link not in [ k for k, v in visited.items()]:
                     stack.append((link, depth + 1))
 
-        return ' \n '.join(sentences)
+        if get_links_only:
+            return {"links": [{"url": k, "depth": v} for k, v in visited.items()]}
+        else:
+            return ' \n '.join(sentences)
     except Exception:
-        pass
-    return ''
+        traceback.print_exc()
+
+    if get_links_only:
+        return {"links": [{
+            "url": url,
+            "depth": 1
+        }]}
+    else:
+        return ""
 
 def extract_text_from_url(url):
     try:
         return crawl(url, max_depth = 1)
     except Exception:
         pass
     return None
```

### Comparing `webtextcrawler-1.0.1/webtextcrawler.egg-info/PKG-INFO` & `webtextcrawler-1.0.2/webtextcrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webtextcrawler
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python project for crawling the web and extracting text.
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro
 Project-URL: Bug Tracker, https://github.com/cnmoro
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

