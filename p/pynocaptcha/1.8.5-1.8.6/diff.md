# Comparing `tmp/pynocaptcha-1.8.5.tar.gz` & `tmp/pynocaptcha-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynocaptcha-1.8.5.tar", last modified: Sat Mar 30 04:19:59 2024, max compression
+gzip compressed data, was "pynocaptcha-1.8.6.tar", last modified: Thu Apr  4 16:00:28 2024, max compression
```

## Comparing `pynocaptcha-1.8.5.tar` & `pynocaptcha-1.8.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-03-30 04:19:59.053174 pynocaptcha-1.8.5/
--rw-r--r--   0 esbiya     (501) staff       (20)     1074 2023-03-15 06:31:13.000000 pynocaptcha-1.8.5/LICENSE
--rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-03-30 04:19:59.052991 pynocaptcha-1.8.5/PKG-INFO
--rw-r--r--   0 esbiya     (501) staff       (20)       38 2023-03-15 09:37:56.000000 pynocaptcha-1.8.5/README.md
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-03-30 04:19:59.051012 pynocaptcha-1.8.5/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)     1095 2024-03-28 09:20:29.000000 pynocaptcha-1.8.5/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-03-30 04:19:59.052763 pynocaptcha-1.8.5/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1054 2023-11-15 10:37:10.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)      646 2024-03-19 14:52:16.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/aws.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5258 2024-03-30 04:19:25.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1061 2024-02-27 06:17:10.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)      744 2023-08-14 02:01:08.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/discord.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2088 2024-01-15 06:49:23.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1559 2024-03-30 04:01:26.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/perimeterx.py
--rw-r--r--   0 esbiya     (501) staff       (20)     3077 2023-12-13 01:23:55.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.8.5/pynocaptcha/crackers/tls.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-03-30 04:19:59.051591 pynocaptcha-1.8.5/pynocaptcha.egg-info/
--rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-03-30 04:19:59.000000 pynocaptcha-1.8.5/pynocaptcha.egg-info/PKG-INFO
--rw-r--r--   0 esbiya     (501) staff       (20)      577 2024-03-30 04:19:59.000000 pynocaptcha-1.8.5/pynocaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-03-30 04:19:59.000000 pynocaptcha-1.8.5/pynocaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-03-30 04:19:59.000000 pynocaptcha-1.8.5/pynocaptcha.egg-info/not-zip-safe
--rw-r--r--   0 esbiya     (501) staff       (20)       15 2024-03-30 04:19:59.000000 pynocaptcha-1.8.5/pynocaptcha.egg-info/requires.txt
--rw-r--r--   0 esbiya     (501) staff       (20)       33 2024-03-30 04:19:59.000000 pynocaptcha-1.8.5/pynocaptcha.egg-info/top_level.txt
--rw-r--r--   0 esbiya     (501) staff       (20)       38 2024-03-30 04:19:59.053213 pynocaptcha-1.8.5/setup.cfg
--rw-r--r--   0 esbiya     (501) staff       (20)      845 2024-03-28 09:20:32.000000 pynocaptcha-1.8.5/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-04 16:00:28.697966 pynocaptcha-1.8.6/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1074 2023-03-15 06:31:13.000000 pynocaptcha-1.8.6/LICENSE
+-rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-04 16:00:28.697784 pynocaptcha-1.8.6/PKG-INFO
+-rw-r--r--   0 esbiya     (501) staff       (20)       38 2023-03-15 09:37:56.000000 pynocaptcha-1.8.6/README.md
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-04 16:00:28.694585 pynocaptcha-1.8.6/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1095 2024-03-28 09:20:29.000000 pynocaptcha-1.8.6/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-04 16:00:28.697496 pynocaptcha-1.8.6/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1054 2023-11-15 10:37:10.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      668 2024-04-04 15:59:57.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/aws.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5258 2024-03-30 04:19:25.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1061 2024-02-27 06:17:10.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      744 2023-08-14 02:01:08.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/discord.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2088 2024-01-15 06:49:23.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1559 2024-03-30 04:01:26.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/perimeterx.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     3077 2023-12-13 01:23:55.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.8.6/pynocaptcha/crackers/tls.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-04 16:00:28.695256 pynocaptcha-1.8.6/pynocaptcha.egg-info/
+-rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 esbiya     (501) staff       (20)      577 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/not-zip-safe
+-rw-r--r--   0 esbiya     (501) staff       (20)       15 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/requires.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)       33 2024-04-04 16:00:28.000000 pynocaptcha-1.8.6/pynocaptcha.egg-info/top_level.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)       38 2024-04-04 16:00:28.698004 pynocaptcha-1.8.6/setup.cfg
+-rw-r--r--   0 esbiya     (501) staff       (20)      845 2024-04-04 16:00:21.000000 pynocaptcha-1.8.6/setup.py
```

### Comparing `pynocaptcha-1.8.5/LICENSE` & `pynocaptcha-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/__init__.py` & `pynocaptcha-1.8.6/pynocaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/aws.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/aws.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,8 +26,9 @@
     # 必传参数
     must_check_params = ["href"]
     # 默认可选参数
     option_params = {
         "user_agent": "",
         "only_sense" : False,
         "challenge_url": "",
+        "api_key": ""
     }
```

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/base.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/base.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/discord.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/discord.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/perimeterx.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/perimeterx.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha/crackers/tls.py` & `pynocaptcha-1.8.6/pynocaptcha/crackers/tls.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/pynocaptcha.egg-info/SOURCES.txt` & `pynocaptcha-1.8.6/pynocaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.5/setup.py` & `pynocaptcha-1.8.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 setup(
     name='pynocaptcha',
-    version='1.8.5',
+    version='1.8.6',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

