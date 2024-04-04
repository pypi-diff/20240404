# Comparing `tmp/xmlriver-0.13.tar.gz` & `tmp/xmlriver-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlriver-0.13.tar", last modified: Tue Mar 12 11:20:52 2024, max compression
+gzip compressed data, was "xmlriver-0.14.tar", last modified: Thu Apr  4 07:56:47 2024, max compression
```

## Comparing `xmlriver-0.13.tar` & `xmlriver-0.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sharkov    (501) staff       (20)        0 2024-03-12 11:20:52.858619 xmlriver-0.13/
--rw-------   0 sharkov    (501) staff       (20)    35149 2024-03-04 21:23:43.000000 xmlriver-0.13/LICENSE
--rw-r--r--   0 sharkov    (501) staff       (20)     6221 2024-03-12 11:20:52.858711 xmlriver-0.13/PKG-INFO
--rw-r--r--   0 sharkov    (501) staff       (20)     5284 2024-03-12 11:19:33.000000 xmlriver-0.13/README.md
--rw-r--r--   0 sharkov    (501) staff       (20)       38 2024-03-12 11:20:52.858907 xmlriver-0.13/setup.cfg
--rw-r--r--   0 sharkov    (501) staff       (20)     1245 2024-03-12 11:20:08.000000 xmlriver-0.13/setup.py
-drwxr-xr-x   0 sharkov    (501) staff       (20)        0 2024-03-12 11:20:52.857850 xmlriver-0.13/xmlriver/
--rw-------   0 sharkov    (501) staff       (20)      270 2024-03-05 16:43:31.000000 xmlriver-0.13/xmlriver/__init__.py
--rw-------   0 sharkov    (501) staff       (20)     3752 2024-03-04 21:58:12.000000 xmlriver-0.13/xmlriver/exceptions.py
--rw-------   0 sharkov    (501) staff       (20)      459 2024-03-06 10:41:19.000000 xmlriver-0.13/xmlriver/google.py
--rw-------   0 sharkov    (501) staff       (20)     7578 2024-03-12 11:18:13.000000 xmlriver-0.13/xmlriver/xmlriver.py
--rw-------   0 sharkov    (501) staff       (20)      454 2024-03-06 10:41:29.000000 xmlriver-0.13/xmlriver/yandex.py
-drwxr-xr-x   0 sharkov    (501) staff       (20)        0 2024-03-12 11:20:52.858507 xmlriver-0.13/xmlriver.egg-info/
--rw-r--r--   0 sharkov    (501) staff       (20)     6221 2024-03-12 11:20:52.000000 xmlriver-0.13/xmlriver.egg-info/PKG-INFO
--rw-r--r--   0 sharkov    (501) staff       (20)      298 2024-03-12 11:20:52.000000 xmlriver-0.13/xmlriver.egg-info/SOURCES.txt
--rw-r--r--   0 sharkov    (501) staff       (20)        1 2024-03-12 11:20:52.000000 xmlriver-0.13/xmlriver.egg-info/dependency_links.txt
--rw-r--r--   0 sharkov    (501) staff       (20)       31 2024-03-12 11:20:52.000000 xmlriver-0.13/xmlriver.egg-info/requires.txt
--rw-r--r--   0 sharkov    (501) staff       (20)        9 2024-03-12 11:20:52.000000 xmlriver-0.13/xmlriver.egg-info/top_level.txt
+drwxr-xr-x   0 sharkov    (501) staff       (20)        0 2024-04-04 07:56:47.743283 xmlriver-0.14/
+-rw-r--r--   0 sharkov    (501) staff       (20)    35149 2024-03-04 21:23:43.000000 xmlriver-0.14/LICENSE
+-rw-r--r--   0 sharkov    (501) staff       (20)     6221 2024-04-04 07:56:47.743497 xmlriver-0.14/PKG-INFO
+-rw-------   0 sharkov    (501) staff       (20)     5284 2024-03-12 11:19:33.000000 xmlriver-0.14/README.md
+-rw-------   0 sharkov    (501) staff       (20)       38 2024-04-04 07:56:47.743794 xmlriver-0.14/setup.cfg
+-rw-------   0 sharkov    (501) staff       (20)     1245 2024-04-04 07:55:11.000000 xmlriver-0.14/setup.py
+drwxr-xr-x   0 sharkov    (501) staff       (20)        0 2024-04-04 07:56:47.741015 xmlriver-0.14/xmlriver/
+-rw-r--r--   0 sharkov    (501) staff       (20)      270 2024-03-05 16:43:31.000000 xmlriver-0.14/xmlriver/__init__.py
+-rw-r--r--   0 sharkov    (501) staff       (20)     3752 2024-03-04 21:58:12.000000 xmlriver-0.14/xmlriver/exceptions.py
+-rw-r--r--   0 sharkov    (501) staff       (20)      459 2024-03-06 10:41:19.000000 xmlriver-0.14/xmlriver/google.py
+-rw-r--r--   0 sharkov    (501) staff       (20)     7755 2024-04-04 07:53:12.000000 xmlriver-0.14/xmlriver/xmlriver.py
+-rw-------   0 sharkov    (501) staff       (20)      454 2024-03-06 10:41:29.000000 xmlriver-0.14/xmlriver/yandex.py
+drwxr-xr-x   0 sharkov    (501) staff       (20)        0 2024-04-04 07:56:47.743108 xmlriver-0.14/xmlriver.egg-info/
+-rw-------   0 sharkov    (501) staff       (20)     6221 2024-04-04 07:56:44.000000 xmlriver-0.14/xmlriver.egg-info/PKG-INFO
+-rw-------   0 sharkov    (501) staff       (20)      298 2024-04-04 07:56:47.000000 xmlriver-0.14/xmlriver.egg-info/SOURCES.txt
+-rw-------   0 sharkov    (501) staff       (20)        1 2024-04-04 07:56:45.000000 xmlriver-0.14/xmlriver.egg-info/dependency_links.txt
+-rw-------   0 sharkov    (501) staff       (20)       31 2024-04-04 07:56:46.000000 xmlriver-0.14/xmlriver.egg-info/requires.txt
+-rw-------   0 sharkov    (501) staff       (20)        9 2024-04-04 07:56:47.000000 xmlriver-0.14/xmlriver.egg-info/top_level.txt
```

### Comparing `xmlriver-0.13/LICENSE` & `xmlriver-0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlriver-0.13/PKG-INFO` & `xmlriver-0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlriver
-Version: 0.13
+Version: 0.14
 Summary: Пакет для работы с поисковой выдачей Google и Yandex по API через сервис XMLRiver / Package for working with Google and Yandex search results via API via XMLRiver service.
 Home-page: https://github.com/KursHub-ru/xmlriver
 Author: Ivan Sharkov
 Author-email: admin@kurshub.ru
 Project-URL: Documentation, https://github.com/KursHub-ru/xmlriver
 Project-URL: GitHub, https://github.com/KursHub-ru/xmlriver
 Project-URL: Homepage, https://0pl.ru
```

### Comparing `xmlriver-0.13/README.md` & `xmlriver-0.14/README.md`

 * *Files identical despite different names*

### Comparing `xmlriver-0.13/setup.py` & `xmlriver-0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
     name="xmlriver",
-    version="0.13",
+    version="0.14",
     author="Ivan Sharkov",
     author_email="admin@kurshub.ru",
     description="Пакет для работы с поисковой выдачей Google и Yandex по API через сервис XMLRiver / Package for working with Google and Yandex search results via API via XMLRiver service.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/KursHub-ru/xmlriver",
     packages=find_packages(),
```

### Comparing `xmlriver-0.13/xmlriver/exceptions.py` & `xmlriver-0.14/xmlriver/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlriver-0.13/xmlriver/xmlriver.py` & `xmlriver-0.14/xmlriver/xmlriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,26 +119,30 @@
             self.pages = 0 if self.fixtype else int(self.response["found"]["#text"])
 
             groups = self.response["results"]["grouping"]["group"]
             if isinstance(groups, list):
                 documents = [group['doc'] for group in groups]
             else:
                 documents = [groups['doc']]
+
+            rank = 1
             
             for document in documents:
                 tmp = {
+                    'rank': rank,
                     'url' : document.get('url'),
                     'title' : document.get('title'),
                     'pubDate' : document.get('pubDate'),
                     'extendedpassage' : document.get('extendedpassage'),
                     'contenttype': document.get('contenttype'),
                     'breadcrumbs': document.get('breadcrumbs'),
 
                 }
                 self.results.append(tmp)
+                rank += 1
            
 
 
     ### All custom methods ###
 
     def count_results_from_domain(self, domain, **kwargs):
         '''
@@ -195,27 +199,30 @@
         
     def is_url_pessimised(self, url, **kwargs):
         '''
         Check url for existing filetes by inurl:
         '''
         query = 'inurl:' + url
         if self.request(query, **kwargs):
-            return not bool(self.pages)
+            urls = self.get_urls()
+            return False if url in urls else True
         else:
             return None
         
     def is_url_indexed(self, url, **kwargs):
         '''
         Check url for indexing by inurl:
         '''
         query = 'site:' + url
         if self.request(query, **kwargs):
-            return not bool(self.pages)
+            urls = self.get_urls()
+            return True if url in urls else False
         else:
             return None
+    
     def get_onebox_documents(self, query, types, **kwargs):
         '''
         Read: https://xmlriver.com/apidoc/api-organic/#onebox
         types: organic, unknown_onebox, video, images, news, calculator, recipes, translator, related_queries
         '''
         if self.request(query, **kwargs):
             return [document for document in self.results if document['contenttype'] in types]
```

### Comparing `xmlriver-0.13/xmlriver.egg-info/PKG-INFO` & `xmlriver-0.14/xmlriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlriver
-Version: 0.13
+Version: 0.14
 Summary: Пакет для работы с поисковой выдачей Google и Yandex по API через сервис XMLRiver / Package for working with Google and Yandex search results via API via XMLRiver service.
 Home-page: https://github.com/KursHub-ru/xmlriver
 Author: Ivan Sharkov
 Author-email: admin@kurshub.ru
 Project-URL: Documentation, https://github.com/KursHub-ru/xmlriver
 Project-URL: GitHub, https://github.com/KursHub-ru/xmlriver
 Project-URL: Homepage, https://0pl.ru
```

