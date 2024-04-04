# Comparing `tmp/yfh-sayhi-0.0.2.tar.gz` & `tmp/yfh-sayhi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-ibeq1lyq\yfh-sayhi-0.0.2.tar", last modified: Thu Apr  4 05:26:30 2024, max compression
+gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-eo665t7b\yfh-sayhi-0.0.3.tar", last modified: Thu Apr  4 06:10:19 2024, max compression
```

## Comparing `yfh-sayhi-0.0.2.tar` & `yfh-sayhi-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 05:26:30.671455 yfh-sayhi-0.0.2/
--rw-rw-rw-   0        0        0      413 2024-04-04 05:26:30.670448 yfh-sayhi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-04-04 03:56:38.000000 yfh-sayhi-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 05:26:30.664770 yfh-sayhi-0.0.2/say_hiaaaaaaa221/
--rw-rw-rw-   0        0        0        0 2024-04-04 05:26:00.000000 yfh-sayhi-0.0.2/say_hiaaaaaaa221/__init__.py
--rw-rw-rw-   0        0        0      132 2024-04-04 05:26:00.000000 yfh-sayhi-0.0.2/say_hiaaaaaaa221/test_func.py
--rw-rw-rw-   0        0        0       42 2024-04-04 05:26:30.671455 yfh-sayhi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      626 2024-04-04 05:26:25.000000 yfh-sayhi-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 05:26:30.669278 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/
--rw-rw-rw-   0        0        0      413 2024-04-04 05:26:30.000000 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-04 05:26:30.000000 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 05:26:30.000000 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 05:26:30.000000 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 06:10:19.714802 yfh-sayhi-0.0.3/
+-rw-rw-rw-   0        0        0      413 2024-04-04 06:10:19.708284 yfh-sayhi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-04-04 03:56:38.000000 yfh-sayhi-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 06:10:19.705242 yfh-sayhi-0.0.3/say_hiaaaaaaa2222/
+-rw-rw-rw-   0        0        0       35 2024-04-04 06:09:35.000000 yfh-sayhi-0.0.3/say_hiaaaaaaa2222/__init__.py
+-rw-rw-rw-   0        0        0      114 2024-04-04 06:08:02.000000 yfh-sayhi-0.0.3/say_hiaaaaaaa2222/say.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 06:10:19.714802 yfh-sayhi-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-04-04 05:57:23.000000 yfh-sayhi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:10:19.708284 yfh-sayhi-0.0.3/test/
+-rw-rw-rw-   0        0        0       47 2024-04-04 06:09:35.000000 yfh-sayhi-0.0.3/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:10:19.708284 yfh-sayhi-0.0.3/yfh_sayhi.egg-info/
+-rw-rw-rw-   0        0        0      413 2024-04-04 06:10:19.000000 yfh-sayhi-0.0.3/yfh_sayhi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-04 06:10:19.000000 yfh-sayhi-0.0.3/yfh_sayhi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 06:10:19.000000 yfh-sayhi-0.0.3/yfh_sayhi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-04 06:10:19.000000 yfh-sayhi-0.0.3/yfh_sayhi.egg-info/top_level.txt
```

### Comparing `yfh-sayhi-0.0.2/setup.py` & `yfh-sayhi-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
-import say_hiaaaaaaa221
+
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yfh-sayhi",
-  version="0.0.2",
+  version="0.0.3",
   author="Example Author",
   author_email="author@example.com",
   description="A small example package",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

