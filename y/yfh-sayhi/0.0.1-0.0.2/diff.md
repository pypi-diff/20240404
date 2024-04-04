# Comparing `tmp/yfh-sayhi-0.0.1.tar.gz` & `tmp/yfh-sayhi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-fujqyzuo\yfh-sayhi-0.0.1.tar", last modified: Thu Apr  4 05:23:43 2024, max compression
+gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-ibeq1lyq\yfh-sayhi-0.0.2.tar", last modified: Thu Apr  4 05:26:30 2024, max compression
```

## Comparing `yfh-sayhi-0.0.1.tar` & `yfh-sayhi-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 05:23:43.891772 yfh-sayhi-0.0.1/
--rw-rw-rw-   0        0        0      413 2024-04-04 05:23:43.891772 yfh-sayhi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-04-04 03:56:38.000000 yfh-sayhi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 05:23:43.876148 yfh-sayhi-0.0.1/say_hiaaaaaaa221/
--rw-rw-rw-   0        0        0      250 2024-04-04 03:55:26.000000 yfh-sayhi-0.0.1/say_hiaaaaaaa221/__init__.py
--rw-rw-rw-   0        0        0      150 2024-04-04 05:17:03.000000 yfh-sayhi-0.0.1/say_hiaaaaaaa221/test_func.py
--rw-rw-rw-   0        0        0       42 2024-04-04 05:23:43.891772 yfh-sayhi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-04-04 05:23:30.000000 yfh-sayhi-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 05:23:43.891772 yfh-sayhi-0.0.1/yfh_sayhi.egg-info/
--rw-rw-rw-   0        0        0      413 2024-04-04 05:23:43.000000 yfh-sayhi-0.0.1/yfh_sayhi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-04 05:23:43.000000 yfh-sayhi-0.0.1/yfh_sayhi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 05:23:43.000000 yfh-sayhi-0.0.1/yfh_sayhi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 05:23:43.000000 yfh-sayhi-0.0.1/yfh_sayhi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 05:26:30.671455 yfh-sayhi-0.0.2/
+-rw-rw-rw-   0        0        0      413 2024-04-04 05:26:30.670448 yfh-sayhi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-04-04 03:56:38.000000 yfh-sayhi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 05:26:30.664770 yfh-sayhi-0.0.2/say_hiaaaaaaa221/
+-rw-rw-rw-   0        0        0        0 2024-04-04 05:26:00.000000 yfh-sayhi-0.0.2/say_hiaaaaaaa221/__init__.py
+-rw-rw-rw-   0        0        0      132 2024-04-04 05:26:00.000000 yfh-sayhi-0.0.2/say_hiaaaaaaa221/test_func.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 05:26:30.671455 yfh-sayhi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      626 2024-04-04 05:26:25.000000 yfh-sayhi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 05:26:30.669278 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/
+-rw-rw-rw-   0        0        0      413 2024-04-04 05:26:30.000000 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-04 05:26:30.000000 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 05:26:30.000000 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 05:26:30.000000 yfh-sayhi-0.0.2/yfh_sayhi.egg-info/top_level.txt
```

### Comparing `yfh-sayhi-0.0.1/setup.py` & `yfh-sayhi-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
-
+import say_hiaaaaaaa221
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yfh-sayhi",
-  version="0.0.1",
+  version="0.0.2",
   author="Example Author",
   author_email="author@example.com",
   description="A small example package",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

