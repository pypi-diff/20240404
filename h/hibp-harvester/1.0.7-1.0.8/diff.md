# Comparing `tmp/hibp-harvester-1.0.7.tar.gz` & `tmp/hibp-harvester-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hibp-harvester-1.0.7.tar", last modified: Thu Mar 28 21:14:38 2024, max compression
+gzip compressed data, was "hibp-harvester-1.0.8.tar", last modified: Thu Apr  4 20:29:37 2024, max compression
```

## Comparing `hibp-harvester-1.0.7.tar` & `hibp-harvester-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:14:38.330790 hibp-harvester-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-28 21:14:31.000000 hibp-harvester-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-28 21:14:38.330790 hibp-harvester-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-28 21:14:31.000000 hibp-harvester-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:14:38.330790 hibp-harvester-1.0.7/hibp_harvester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-28 21:14:38.000000 hibp-harvester-1.0.7/hibp_harvester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 21:14:38.000000 hibp-harvester-1.0.7/hibp_harvester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 21:14:38.000000 hibp-harvester-1.0.7/hibp_harvester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 21:14:38.000000 hibp-harvester-1.0.7/hibp_harvester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 21:14:38.000000 hibp-harvester-1.0.7/hibp_harvester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-28 21:14:38.000000 hibp-harvester-1.0.7/hibp_harvester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 21:14:38.330790 hibp-harvester-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-28 21:14:31.000000 hibp-harvester-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:14:38.330790 hibp-harvester-1.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 21:14:31.000000 hibp-harvester-1.0.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-03-28 21:14:31.000000 hibp-harvester-1.0.7/src/hibp_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:29:37.677872 hibp-harvester-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-04 20:29:31.000000 hibp-harvester-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-04 20:29:37.677872 hibp-harvester-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-04 20:29:31.000000 hibp-harvester-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:29:37.677872 hibp-harvester-1.0.8/hibp_harvester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-04 20:29:37.000000 hibp-harvester-1.0.8/hibp_harvester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 20:29:37.000000 hibp-harvester-1.0.8/hibp_harvester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:29:37.000000 hibp-harvester-1.0.8/hibp_harvester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 20:29:37.000000 hibp-harvester-1.0.8/hibp_harvester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 20:29:37.000000 hibp-harvester-1.0.8/hibp_harvester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 20:29:37.000000 hibp-harvester-1.0.8/hibp_harvester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:29:37.677872 hibp-harvester-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-04 20:29:31.000000 hibp-harvester-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:29:37.677872 hibp-harvester-1.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:29:31.000000 hibp-harvester-1.0.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-04 20:29:31.000000 hibp-harvester-1.0.8/src/hibp_harvester.py
```

### Comparing `hibp-harvester-1.0.7/LICENSE` & `hibp-harvester-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hibp-harvester-1.0.7/PKG-INFO` & `hibp-harvester-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hibp-harvester
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python tool to harvest haveibeenpwned.com via domain search
 Home-page: https://github.com/security-companion/hibp-harvester
 Author: Joachim Mammele
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `hibp-harvester-1.0.7/README.md` & `hibp-harvester-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hibp-harvester-1.0.7/hibp_harvester.egg-info/PKG-INFO` & `hibp-harvester-1.0.8/hibp_harvester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hibp-harvester
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python tool to harvest haveibeenpwned.com via domain search
 Home-page: https://github.com/security-companion/hibp-harvester
 Author: Joachim Mammele
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `hibp-harvester-1.0.7/setup.py` & `hibp-harvester-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hibp-harvester",
-    version="1.0.7",
+    version="1.0.8",
     author="Joachim Mammele",
     url="https://github.com/security-companion/hibp-harvester",
     description="A python tool to harvest haveibeenpwned.com via domain search",
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `hibp-harvester-1.0.7/src/hibp_harvester.py` & `hibp-harvester-1.0.8/src/hibp_harvester.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,18 @@
         time.sleep(int(wait_time_seconds))
 
         with session.get(url) as response:
             if not response.ok:
                 if response.status_code == 401:
                     print("API key not valid")
                     sys.exit(1)
+                elif response.status_code == 404:
+                    print("the account could not be found and has therefore not been pwned")
+                    print(url)
+                    return {}
                 else:
                     print(f"response code: {response.status_code}")
                     print(f"response message: {response.message}")
                     sys.exit(1)
             response_json = response.json()
         return response_json
```

