# Comparing `tmp/srt_trans-0.1.0.tar.gz` & `tmp/srt_trans-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-0.1.0.tar", last modified: Thu Apr  4 00:30:27 2024, max compression
+gzip compressed data, was "srt_trans-0.1.1.tar", last modified: Thu Apr  4 00:39:30 2024, max compression
```

## Comparing `srt_trans-0.1.0.tar` & `srt_trans-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 00:30:27.085389 srt_trans-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-04-02 13:45:48.000000 srt_trans-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1494 2024-04-04 00:30:27.085389 srt_trans-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      850 2024-04-04 00:29:32.000000 srt_trans-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 00:30:27.085389 srt_trans-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1016 2024-04-04 00:29:51.000000 srt_trans-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 00:30:27.049156 srt_trans-0.1.0/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-02 13:33:58.000000 srt_trans-0.1.0/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     3391 2024-04-03 23:23:22.000000 srt_trans-0.1.0/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 00:30:27.074199 srt_trans-0.1.0/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1494 2024-04-04 00:30:26.000000 srt_trans-0.1.0/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 00:30:26.000000 srt_trans-0.1.0/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 00:30:26.000000 srt_trans-0.1.0/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 00:30:26.000000 srt_trans-0.1.0/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-04 00:30:26.000000 srt_trans-0.1.0/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 00:30:26.000000 srt_trans-0.1.0/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 00:39:30.894624 srt_trans-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1490 2024-04-04 00:39:30.894624 srt_trans-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2024-04-04 00:36:54.000000 srt_trans-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 00:39:30.894624 srt_trans-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-04 00:39:01.000000 srt_trans-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:39:30.845696 srt_trans-0.1.1/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-0.1.1/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     3391 2024-04-04 00:36:54.000000 srt_trans-0.1.1/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:39:30.894624 srt_trans-0.1.1/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1490 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-0.1.0/LICENSE` & `srt_trans-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-0.1.0/PKG-INFO` & `srt_trans-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: srt_trans
-Version: 0.1.0
-Summary: A simple translator for any SubRip(.srt) file.
-Home-page: https://github.com/bumblezhou/srt_translator
+Version: 0.1.1
+Summary: A simple translator for any SubRip(.srt) files.
+Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `srt_trans-0.1.0/setup.py` & `srt_trans-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
         # List your dependencies here
         'googletrans==3.1.0a0',
         'pysrt>=1.1.2'
     ],
     author='Jack',
     author_email='bumble.zhou@gmail.com',
-    description='A simple translator for any SubRip(.srt) file.',
+    description='A simple translator for any SubRip(.srt) files.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/bumblezhou/srt_translator',
+    url='https://github.com/bumblezhou/srt_trans',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

### Comparing `srt_trans-0.1.0/srt_trans/cli.py` & `srt_trans-0.1.1/srt_trans/cli.py`

 * *Files identical despite different names*

### Comparing `srt_trans-0.1.0/srt_trans.egg-info/PKG-INFO` & `srt_trans-0.1.1/srt_trans.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: srt-trans
-Version: 0.1.0
-Summary: A simple translator for any SubRip(.srt) file.
-Home-page: https://github.com/bumblezhou/srt_translator
+Version: 0.1.1
+Summary: A simple translator for any SubRip(.srt) files.
+Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

