# Comparing `tmp/dxflow-0.1.0.tar.gz` & `tmp/dxflow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxflow-0.1.0.tar", last modified: Tue Apr  2 22:54:47 2024, max compression
+gzip compressed data, was "dxflow-0.1.1.tar", last modified: Thu Apr  4 00:22:37 2024, max compression
```

## Comparing `dxflow-0.1.0.tar` & `dxflow-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 22:54:47.918417 dxflow-0.1.0/
--rw-rw-rw-   0        0        0     1086 2024-04-02 22:09:18.000000 dxflow-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2371 2024-04-02 22:54:47.911743 dxflow-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1930 2024-04-02 22:09:18.000000 dxflow-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 22:54:47.904737 dxflow-0.1.0/dxflow.egg-info/
--rw-rw-rw-   0        0        0     2371 2024-04-02 22:54:47.000000 dxflow-0.1.0/dxflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2024-04-02 22:54:47.000000 dxflow-0.1.0/dxflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 22:54:47.000000 dxflow-0.1.0/dxflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 22:54:47.000000 dxflow-0.1.0/dxflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-04-02 22:54:38.000000 dxflow-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 22:54:47.918930 dxflow-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1216 2024-04-02 22:15:19.000000 dxflow-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:22:37.048643 dxflow-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2024-04-02 22:09:18.000000 dxflow-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2371 2024-04-04 00:22:37.046644 dxflow-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1930 2024-04-02 22:09:18.000000 dxflow-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 00:22:37.044642 dxflow-0.1.1/dxflow.egg-info/
+-rw-rw-rw-   0        0        0     2371 2024-04-04 00:22:36.000000 dxflow-0.1.1/dxflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-04-04 00:22:36.000000 dxflow-0.1.1/dxflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 00:22:36.000000 dxflow-0.1.1/dxflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-04 00:22:36.000000 dxflow-0.1.1/dxflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-04-04 00:22:14.000000 dxflow-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 00:22:37.048643 dxflow-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2024-04-04 00:22:18.000000 dxflow-0.1.1/setup.py
```

### Comparing `dxflow-0.1.0/LICENSE` & `dxflow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxflow-0.1.0/PKG-INFO` & `dxflow-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxflow
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python SDK for dxflow
 Home-page: https://github.com/diphyx/dxflow_sdk
 Author: DiPhyx Team
 Author-email: DiPhyx Team <info@diphyx.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dxflow-0.1.0/README.md` & `dxflow-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dxflow-0.1.0/dxflow.egg-info/PKG-INFO` & `dxflow-0.1.1/dxflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxflow
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python SDK for dxflow
 Home-page: https://github.com/diphyx/dxflow_sdk
 Author: DiPhyx Team
 Author-email: DiPhyx Team <info@diphyx.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dxflow-0.1.0/setup.py` & `dxflow-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dxflow',
-    version='0.1',
+    version='0.1.1',
     author='DiPhyx Team',
     author_email='info@diphyx.com',
     description='A Python SDK for the DiPhyx cloud computing platform, designed to streamline scientific discovery.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/diphyx/dxflow_sdk',
     py_modules=['dxflow'],  # Specify the module name here
```

