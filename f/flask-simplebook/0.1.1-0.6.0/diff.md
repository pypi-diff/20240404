# Comparing `tmp/flask-simplebook-0.1.1.tar.gz` & `tmp/flask-simplebook-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-simplebook-0.1.1.tar", last modified: Mon Oct 24 18:27:15 2022, max compression
+gzip compressed data, was "flask-simplebook-0.6.0.tar", last modified: Wed Apr  3 23:04:26 2024, max compression
```

## Comparing `flask-simplebook-0.1.1.tar` & `flask-simplebook-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2022-10-24 18:27:15.633260 flask-simplebook-0.1.1/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2437 2022-10-24 18:27:15.633260 flask-simplebook-0.1.1/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1987 2022-10-17 17:05:23.000000 flask-simplebook-0.1.1/README.md
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2022-10-24 18:27:15.633260 flask-simplebook-0.1.1/flask_simplebook.egg-info/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2437 2022-10-24 18:27:15.000000 flask-simplebook-0.1.1/flask_simplebook.egg-info/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      281 2022-10-24 18:27:15.000000 flask-simplebook-0.1.1/flask_simplebook.egg-info/SOURCES.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2022-10-24 18:27:15.000000 flask-simplebook-0.1.1/flask_simplebook.egg-info/dependency_links.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        9 2022-10-24 18:27:15.000000 flask-simplebook-0.1.1/flask_simplebook.egg-info/requires.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       11 2022-10-24 18:27:15.000000 flask-simplebook-0.1.1/flask_simplebook.egg-info/top_level.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2022-10-24 18:27:15.633260 flask-simplebook-0.1.1/setup.cfg
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      862 2022-10-24 18:13:19.000000 flask-simplebook-0.1.1/setup.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2022-10-24 18:27:15.633260 flask-simplebook-0.1.1/simplebook/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3061 2022-10-24 16:24:31.000000 flask-simplebook-0.1.1/simplebook/app.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      272 2022-05-26 16:17:02.000000 flask-simplebook-0.1.1/simplebook/worker.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       73 2022-05-26 16:17:02.000000 flask-simplebook-0.1.1/simplebook/wsgi.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-03 23:04:26.711934 flask-simplebook-0.6.0/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2476 2024-04-03 23:04:26.711934 flask-simplebook-0.6.0/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1987 2022-10-17 17:05:23.000000 flask-simplebook-0.6.0/README.md
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-03 23:04:26.707934 flask-simplebook-0.6.0/flask_simplebook.egg-info/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2476 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      281 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/SOURCES.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/dependency_links.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        9 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/requires.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       11 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/top_level.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2024-04-03 23:04:26.711934 flask-simplebook-0.6.0/setup.cfg
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      862 2024-04-03 23:02:07.000000 flask-simplebook-0.6.0/setup.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-03 23:04:26.707934 flask-simplebook-0.6.0/simplebook/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3061 2022-10-24 16:24:31.000000 flask-simplebook-0.6.0/simplebook/app.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      272 2022-05-26 16:17:02.000000 flask-simplebook-0.6.0/simplebook/worker.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       73 2022-05-26 16:17:02.000000 flask-simplebook-0.6.0/simplebook/wsgi.py
```

### Comparing `flask-simplebook-0.1.1/PKG-INFO` & `flask-simplebook-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: flask-simplebook
-Version: 0.1.1
+Version: 0.6.0
 Summary: flask app for SimpleBook
 Home-page: https://code.librehq.com/ots/mediawiki/SimpleBook
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: flask
+Requires-Dist: rq
 
 # flask-simplebook
 
 This is the flask companion application to the SimpleBook MediaWiki extension.
 
 It handles all the administration of pdf creation.  To that end, it is comprised of
 two parts:
```

### Comparing `flask-simplebook-0.1.1/README.md` & `flask-simplebook-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `flask-simplebook-0.1.1/flask_simplebook.egg-info/PKG-INFO` & `flask-simplebook-0.6.0/flask_simplebook.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: flask-simplebook
-Version: 0.1.1
+Version: 0.6.0
 Summary: flask app for SimpleBook
 Home-page: https://code.librehq.com/ots/mediawiki/SimpleBook
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: flask
+Requires-Dist: rq
 
 # flask-simplebook
 
 This is the flask companion application to the SimpleBook MediaWiki extension.
 
 It handles all the administration of pdf creation.  To that end, it is comprised of
 two parts:
```

### Comparing `flask-simplebook-0.1.1/setup.py` & `flask-simplebook-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setup(
     name="flask-simplebook",
-    version="0.1.1",
+    version="0.6.0",
     description="flask app for SimpleBook",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Open Tech Strategies, LLC",
     author_email="frankduncan@opentechstrategies.com",  # For now, this works
     url="https://code.librehq.com/ots/mediawiki/SimpleBook",
     classifiers=[
```

### Comparing `flask-simplebook-0.1.1/simplebook/app.py` & `flask-simplebook-0.6.0/simplebook/app.py`

 * *Files identical despite different names*

