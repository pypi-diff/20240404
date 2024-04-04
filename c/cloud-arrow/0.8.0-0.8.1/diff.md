# Comparing `tmp/cloud-arrow-0.8.0.tar.gz` & `tmp/cloud-arrow-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-arrow-0.8.0.tar", last modified: Mon Apr  1 11:33:58 2024, max compression
+gzip compressed data, was "cloud-arrow-0.8.1.tar", last modified: Thu Apr  4 09:51:17 2024, max compression
```

## Comparing `cloud-arrow-0.8.0.tar` & `cloud-arrow-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.143248 cloud-arrow-0.8.0/
--rw-rw-rw-   0        0        0    35821 2023-10-31 09:54:53.000000 cloud-arrow-0.8.0/LICENSE
--rw-rw-rw-   0        0        0    21484 2024-04-01 11:33:58.143248 cloud-arrow-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0    20806 2024-04-01 11:26:49.000000 cloud-arrow-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.107363 cloud-arrow-0.8.0/cloud/
--rw-rw-rw-   0        0        0      162 2024-04-01 09:25:18.000000 cloud-arrow-0.8.0/cloud/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.110377 cloud-arrow-0.8.0/cloud/adls/
--rw-rw-rw-   0        0        0       31 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/adls/__init__.py
--rw-rw-rw-   0        0        0     2359 2024-01-03 10:09:58.000000 cloud-arrow-0.8.0/cloud/adls/adls.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.113387 cloud-arrow-0.8.0/cloud/core/
--rw-rw-rw-   0        0        0      140 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/core/__init__.py
--rw-rw-rw-   0        0        0    19143 2024-03-27 13:40:37.000000 cloud-arrow-0.8.0/cloud/core/core.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.118507 cloud-arrow-0.8.0/cloud/gcsfs/
--rw-rw-rw-   0        0        0       31 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/gcsfs/__init__.py
--rw-rw-rw-   0        0        0     1780 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/gcsfs/gcsfs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.122047 cloud-arrow-0.8.0/cloud/local/
--rw-rw-rw-   0        0        0        0 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/local/__init__.py
--rw-rw-rw-   0        0        0      733 2023-12-28 08:23:41.000000 cloud-arrow-0.8.0/cloud/local/local.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:33:58.141057 cloud-arrow-0.8.0/cloud_arrow.egg-info/
--rw-rw-rw-   0        0        0    21484 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 11:33:57.000000 cloud-arrow-0.8.0/cloud_arrow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-01 11:33:58.144302 cloud-arrow-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1165 2024-04-01 09:28:01.000000 cloud-arrow-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:51:17.420459 cloud-arrow-0.8.1/
+-rw-rw-rw-   0        0        0    35821 2023-10-31 09:54:53.000000 cloud-arrow-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0    21486 2024-04-04 09:51:17.419388 cloud-arrow-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20808 2024-04-04 09:46:49.000000 cloud-arrow-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 09:51:17.386788 cloud-arrow-0.8.1/cloud/
+-rw-rw-rw-   0        0        0      162 2024-04-01 12:33:15.000000 cloud-arrow-0.8.1/cloud/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:51:17.390860 cloud-arrow-0.8.1/cloud/adls/
+-rw-rw-rw-   0        0        0       31 2023-12-28 08:23:41.000000 cloud-arrow-0.8.1/cloud/adls/__init__.py
+-rw-rw-rw-   0        0        0     2359 2024-01-03 10:09:58.000000 cloud-arrow-0.8.1/cloud/adls/adls.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:51:17.394132 cloud-arrow-0.8.1/cloud/core/
+-rw-rw-rw-   0        0        0      140 2023-12-28 08:23:41.000000 cloud-arrow-0.8.1/cloud/core/__init__.py
+-rw-rw-rw-   0        0        0    19143 2024-04-01 12:33:15.000000 cloud-arrow-0.8.1/cloud/core/core.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:51:17.398281 cloud-arrow-0.8.1/cloud/gcsfs/
+-rw-rw-rw-   0        0        0       31 2023-12-28 08:23:41.000000 cloud-arrow-0.8.1/cloud/gcsfs/__init__.py
+-rw-rw-rw-   0        0        0     1780 2023-12-28 08:23:41.000000 cloud-arrow-0.8.1/cloud/gcsfs/gcsfs.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:51:17.401386 cloud-arrow-0.8.1/cloud/local/
+-rw-rw-rw-   0        0        0       43 2024-04-04 09:45:50.000000 cloud-arrow-0.8.1/cloud/local/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-12-28 08:23:41.000000 cloud-arrow-0.8.1/cloud/local/local.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:51:17.409855 cloud-arrow-0.8.1/cloud_arrow.egg-info/
+-rw-rw-rw-   0        0        0    21486 2024-04-04 09:51:17.000000 cloud-arrow-0.8.1/cloud_arrow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-04-04 09:51:17.000000 cloud-arrow-0.8.1/cloud_arrow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 09:51:17.000000 cloud-arrow-0.8.1/cloud_arrow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-04-04 09:51:17.000000 cloud-arrow-0.8.1/cloud_arrow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 09:51:17.000000 cloud-arrow-0.8.1/cloud_arrow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-04 09:51:17.421486 cloud-arrow-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2024-04-04 09:46:31.000000 cloud-arrow-0.8.1/setup.py
```

### Comparing `cloud-arrow-0.8.0/LICENSE` & `cloud-arrow-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.8.0/PKG-INFO` & `cloud-arrow-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-arrow
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python library to provide an Unified cloud storage API for reading and writing parquet and  deltalake files from/to the main cloud provider's object storage using the arrow format
 Home-page: https://github.com/a24lorie/Cloud-Arrow
 Author-email: a24lorie@gmail.com, nachorodriguez79@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
@@ -15,17 +15,17 @@
 Requires-Dist: gcsfs
 Requires-Dist: s3fs
 Requires-Dist: azure-identity
 Requires-Dist: fsspec
 Requires-Dist: deltalake
 
 <p style="text-align: center;">
-   Feb 2024 <br/>
+   April 2024 <br/>
    Alfredo Lorie Bernardo, Ignacio Rodriguez Sanchez <br/>
-   version 0.8.0
+   version 0.8.1
 </p>
 
 # Cloud Arrow
 Python Library to read and write Parquet and Deltalake files from the main Cloud Providers 
 Object-Store and Local Filesystem
 
 ## Introduction
```

### Comparing `cloud-arrow-0.8.0/README.md` & `cloud-arrow-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p style="text-align: center;">
-   Feb 2024 <br/>
+   April 2024 <br/>
    Alfredo Lorie Bernardo, Ignacio Rodriguez Sanchez <br/>
-   version 0.8.0
+   version 0.8.1
 </p>
 
 # Cloud Arrow
 Python Library to read and write Parquet and Deltalake files from the main Cloud Providers 
 Object-Store and Local Filesystem
 
 ## Introduction
```

### Comparing `cloud-arrow-0.8.0/cloud/adls/adls.py` & `cloud-arrow-0.8.1/cloud/adls/adls.py`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.8.0/cloud/core/core.py` & `cloud-arrow-0.8.1/cloud/core/core.py`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.8.0/cloud/gcsfs/gcsfs.py` & `cloud-arrow-0.8.1/cloud/gcsfs/gcsfs.py`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.8.0/cloud/local/local.py` & `cloud-arrow-0.8.1/cloud/local/local.py`

 * *Files identical despite different names*

### Comparing `cloud-arrow-0.8.0/cloud_arrow.egg-info/PKG-INFO` & `cloud-arrow-0.8.1/cloud_arrow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-arrow
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python library to provide an Unified cloud storage API for reading and writing parquet and  deltalake files from/to the main cloud provider's object storage using the arrow format
 Home-page: https://github.com/a24lorie/Cloud-Arrow
 Author-email: a24lorie@gmail.com, nachorodriguez79@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
@@ -15,17 +15,17 @@
 Requires-Dist: gcsfs
 Requires-Dist: s3fs
 Requires-Dist: azure-identity
 Requires-Dist: fsspec
 Requires-Dist: deltalake
 
 <p style="text-align: center;">
-   Feb 2024 <br/>
+   April 2024 <br/>
    Alfredo Lorie Bernardo, Ignacio Rodriguez Sanchez <br/>
-   version 0.8.0
+   version 0.8.1
 </p>
 
 # Cloud Arrow
 Python Library to read and write Parquet and Deltalake files from the main Cloud Providers 
 Object-Store and Local Filesystem
 
 ## Introduction
```

### Comparing `cloud-arrow-0.8.0/setup.py` & `cloud-arrow-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cloud-arrow',
-    version='0.8.0',
+    version='0.8.1',
     authors='Alfredo Lorie, Ignacio Rodriguez',
     author_email='a24lorie@gmail.com, nachorodriguez79@gmail.com',
     description="""Python library to provide an Unified cloud storage API for reading and writing parquet and  deltalake files from/to the main cloud provider's object storage using the arrow format""",
     long_description=open('README.md', encoding='UTF-8').read(),
     long_description_content_type='text/markdown',
     license='GNU',
     url='https://github.com/a24lorie/Cloud-Arrow',
```

