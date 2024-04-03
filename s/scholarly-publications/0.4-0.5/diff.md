# Comparing `tmp/scholarly_publications-0.4.tar.gz` & `tmp/scholarly_publications-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scholarly_publications-0.4.tar", last modified: Wed Apr  3 22:14:57 2024, max compression
+gzip compressed data, was "scholarly_publications-0.5.tar", last modified: Wed Apr  3 22:27:48 2024, max compression
```

## Comparing `scholarly_publications-0.4.tar` & `scholarly_publications-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:14:57.171603 scholarly_publications-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 22:14:50.000000 scholarly_publications-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-03 22:14:57.167603 scholarly_publications-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-03 22:14:50.000000 scholarly_publications-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:14:57.167603 scholarly_publications-0.4/scholarly_publications/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 22:14:50.000000 scholarly_publications-0.4/scholarly_publications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-03 22:14:50.000000 scholarly_publications-0.4/scholarly_publications/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-03 22:14:50.000000 scholarly_publications-0.4/scholarly_publications/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:14:57.167603 scholarly_publications-0.4/scholarly_publications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-03 22:14:57.000000 scholarly_publications-0.4/scholarly_publications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 22:14:57.000000 scholarly_publications-0.4/scholarly_publications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:14:57.000000 scholarly_publications-0.4/scholarly_publications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 22:14:57.000000 scholarly_publications-0.4/scholarly_publications.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 22:14:57.000000 scholarly_publications-0.4/scholarly_publications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 22:14:57.000000 scholarly_publications-0.4/scholarly_publications.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:14:57.171603 scholarly_publications-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 22:14:50.000000 scholarly_publications-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:14:57.167603 scholarly_publications-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 22:14:50.000000 scholarly_publications-0.4/tests/test_scholarly_publications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:27:48.019787 scholarly_publications-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 22:27:43.000000 scholarly_publications-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-03 22:27:48.015787 scholarly_publications-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-03 22:27:43.000000 scholarly_publications-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:27:48.015787 scholarly_publications-0.5/scholarly_publications/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 22:27:43.000000 scholarly_publications-0.5/scholarly_publications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-03 22:27:43.000000 scholarly_publications-0.5/scholarly_publications/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-03 22:27:43.000000 scholarly_publications-0.5/scholarly_publications/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:27:48.015787 scholarly_publications-0.5/scholarly_publications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:27:48.019787 scholarly_publications-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 22:27:43.000000 scholarly_publications-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:27:48.015787 scholarly_publications-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 22:27:43.000000 scholarly_publications-0.5/tests/test_scholarly_publications.py
```

### Comparing `scholarly_publications-0.4/LICENSE` & `scholarly_publications-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scholarly_publications-0.4/PKG-INFO` & `scholarly_publications-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scholarly_publications
-Version: 0.4
+Version: 0.5
 Summary: A tool to fetch scholarly publications from Google Scholar by author ID
 Home-page: https://github.com/ezefranca/scholarly_publications
 Author: Ezequiel França
 Author-email: ezequiel.franca@gmail.com
 Project-URL: Bug Reports, https://github.com/ezefranca/scholarly_publications/issues
 Project-URL: Source, https://github.com/ezefranca/scholarly_publications
 Keywords: scholarly publications google scholar fetcher academia
```

### Comparing `scholarly_publications-0.4/README.md` & `scholarly_publications-0.5/README.md`

 * *Files identical despite different names*

### Comparing `scholarly_publications-0.4/scholarly_publications/cli.py` & `scholarly_publications-0.5/scholarly_publications/cli.py`

 * *Files identical despite different names*

### Comparing `scholarly_publications-0.4/scholarly_publications/fetcher.py` & `scholarly_publications-0.5/scholarly_publications/fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 
     return all_publications
 
 def parse_publications(soup):
     publications_list = []
     for row in soup.select('.gsc_a_tr'):
         title_element = row.select_one('.gsc_a_at')
-        title = title_element.text.replace(':', ' -') if title_element else "No title"
+        title = title_element.text if title_element else "No title"
         year_element = row.select_one('.gsc_a_h')
         year = year_element.text if year_element else "No year"
         link = f'https://scholar.google.com{title_element["href"]}' if title_element else "No link"
         citation_element = row.select_one('.gsc_a_ac')
         citations = citation_element.text if citation_element and citation_element.text.strip() else "0"  # Check if text exists and is not empty
 
         publications_list.append({
-            'title': title,
-            'year': year,
-            'link': link,
-            'citations': citations,
+            "title": title,
+            "year": year,
+            "link": link,
+            "citations": citations,
         })
 
     return publications_list
```

### Comparing `scholarly_publications-0.4/scholarly_publications.egg-info/PKG-INFO` & `scholarly_publications-0.5/scholarly_publications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scholarly_publications
-Version: 0.4
+Version: 0.5
 Summary: A tool to fetch scholarly publications from Google Scholar by author ID
 Home-page: https://github.com/ezefranca/scholarly_publications
 Author: Ezequiel França
 Author-email: ezequiel.franca@gmail.com
 Project-URL: Bug Reports, https://github.com/ezefranca/scholarly_publications/issues
 Project-URL: Source, https://github.com/ezefranca/scholarly_publications
 Keywords: scholarly publications google scholar fetcher academia
```

### Comparing `scholarly_publications-0.4/setup.py` & `scholarly_publications-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from io import open
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-version = '0.4'
+version = '0.5'
 
 setup(
     name='scholarly_publications',
     version=version,
     description='A tool to fetch scholarly publications from Google Scholar by author ID',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `scholarly_publications-0.4/tests/test_scholarly_publications.py` & `scholarly_publications-0.5/tests/test_scholarly_publications.py`

 * *Files identical despite different names*

