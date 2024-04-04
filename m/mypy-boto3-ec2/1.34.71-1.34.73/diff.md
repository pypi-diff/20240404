# Comparing `tmp/mypy-boto3-ec2-1.34.71.tar.gz` & `tmp/mypy-boto3-ec2-1.34.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ec2-1.34.71.tar", last modified: Tue Mar 26 19:32:58 2024, max compression
+gzip compressed data, was "mypy-boto3-ec2-1.34.73.tar", last modified: Thu Mar 28 19:34:41 2024, max compression
```

## Comparing `mypy-boto3-ec2-1.34.71.tar` & `mypy-boto3-ec2-1.34.73.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:58.332919 mypy-boto3-ec2-1.34.71/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-26 19:32:10.000000 mypy-boto3-ec2-1.34.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-03-26 19:32:58.332919 mypy-boto3-ec2-1.34.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-03-26 19:32:10.000000 mypy-boto3-ec2-1.34.71/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:58.332919 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-03-26 19:32:10.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-03-26 19:32:10.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-26 19:32:10.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   542226 2024-03-26 19:32:17.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   542223 2024-03-26 19:32:14.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    96541 2024-03-26 19:32:23.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    96541 2024-03-26 19:32:23.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   187422 2024-03-26 19:32:21.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)   187279 2024-03-26 19:32:20.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:10.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   271947 2024-03-26 19:32:20.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   271869 2024-03-26 19:32:18.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-03-26 19:32:39.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-03-26 19:32:33.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-26 19:32:10.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-03-26 19:32:21.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-03-26 19:32:21.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:58.332919 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-03-26 19:32:58.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-26 19:32:58.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:32:58.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:32:58.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 19:32:58.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-26 19:32:58.000000 mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 19:32:58.332919 mypy-boto3-ec2-1.34.71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-26 19:32:10.000000 mypy-boto3-ec2-1.34.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:41.116064 mypy-boto3-ec2-1.34.73/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-28 19:32:12.000000 mypy-boto3-ec2-1.34.73/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-03-28 19:34:41.116064 mypy-boto3-ec2-1.34.73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-03-28 19:32:12.000000 mypy-boto3-ec2-1.34.73/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:41.112064 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-03-28 19:32:12.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-03-28 19:32:12.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-28 19:32:12.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   542226 2024-03-28 19:32:19.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   542223 2024-03-28 19:32:15.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    96595 2024-03-28 19:32:26.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96595 2024-03-28 19:32:25.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   187422 2024-03-28 19:32:23.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   187279 2024-03-28 19:32:22.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 19:32:12.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   271947 2024-03-28 19:32:22.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)   271869 2024-03-28 19:32:20.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-03-28 19:32:42.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-03-28 19:32:36.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 19:32:12.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-03-28 19:32:23.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-03-28 19:32:23.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:34:41.112064 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-03-28 19:34:41.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-28 19:34:41.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:34:41.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:34:41.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 19:34:41.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 19:34:41.000000 mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:34:41.116064 mypy-boto3-ec2-1.34.73/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-28 19:32:12.000000 mypy-boto3-ec2-1.34.73/setup.py
```

### Comparing `mypy-boto3-ec2-1.34.71/LICENSE` & `mypy-boto3-ec2-1.34.73/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/PKG-INFO` & `mypy-boto3-ec2-1.34.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.71
-Summary: Type annotations for boto3.EC2 1.34.71 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.73
+Summary: Type annotations for boto3.EC2 1.34.73 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ec2-1.34.71/README.md` & `mypy-boto3-ec2-1.34.73/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/__init__.py` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/__init__.pyi` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/__main__.py` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EC2 1.34.71\n"
-        "Version:         1.34.71\n"
+        "Type annotations for boto3.EC2 1.34.73\n"
+        "Version:         1.34.73\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.71")
+    print("1.34.73")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/client.py` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/client.pyi` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/literals.py` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1216,14 +1216,15 @@
     "c7gd.12xlarge",
     "c7gd.16xlarge",
     "c7gd.2xlarge",
     "c7gd.4xlarge",
     "c7gd.8xlarge",
     "c7gd.large",
     "c7gd.medium",
+    "c7gd.metal",
     "c7gd.xlarge",
     "c7gn.12xlarge",
     "c7gn.16xlarge",
     "c7gn.2xlarge",
     "c7gn.4xlarge",
     "c7gn.8xlarge",
     "c7gn.large",
@@ -1534,14 +1535,15 @@
     "m7gd.12xlarge",
     "m7gd.16xlarge",
     "m7gd.2xlarge",
     "m7gd.4xlarge",
     "m7gd.8xlarge",
     "m7gd.large",
     "m7gd.medium",
+    "m7gd.metal",
     "m7gd.xlarge",
     "m7i-flex.2xlarge",
     "m7i-flex.4xlarge",
     "m7i-flex.8xlarge",
     "m7i-flex.large",
     "m7i-flex.xlarge",
     "m7i.12xlarge",
@@ -1734,14 +1736,15 @@
     "r7gd.12xlarge",
     "r7gd.16xlarge",
     "r7gd.2xlarge",
     "r7gd.4xlarge",
     "r7gd.8xlarge",
     "r7gd.large",
     "r7gd.medium",
+    "r7gd.metal",
     "r7gd.xlarge",
     "r7i.12xlarge",
     "r7i.16xlarge",
     "r7i.24xlarge",
     "r7i.2xlarge",
     "r7i.48xlarge",
     "r7i.4xlarge",
```

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/literals.pyi` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1216,14 +1216,15 @@
     "c7gd.12xlarge",
     "c7gd.16xlarge",
     "c7gd.2xlarge",
     "c7gd.4xlarge",
     "c7gd.8xlarge",
     "c7gd.large",
     "c7gd.medium",
+    "c7gd.metal",
     "c7gd.xlarge",
     "c7gn.12xlarge",
     "c7gn.16xlarge",
     "c7gn.2xlarge",
     "c7gn.4xlarge",
     "c7gn.8xlarge",
     "c7gn.large",
@@ -1534,14 +1535,15 @@
     "m7gd.12xlarge",
     "m7gd.16xlarge",
     "m7gd.2xlarge",
     "m7gd.4xlarge",
     "m7gd.8xlarge",
     "m7gd.large",
     "m7gd.medium",
+    "m7gd.metal",
     "m7gd.xlarge",
     "m7i-flex.2xlarge",
     "m7i-flex.4xlarge",
     "m7i-flex.8xlarge",
     "m7i-flex.large",
     "m7i-flex.xlarge",
     "m7i.12xlarge",
@@ -1734,14 +1736,15 @@
     "r7gd.12xlarge",
     "r7gd.16xlarge",
     "r7gd.2xlarge",
     "r7gd.4xlarge",
     "r7gd.8xlarge",
     "r7gd.large",
     "r7gd.medium",
+    "r7gd.metal",
     "r7gd.xlarge",
     "r7i.12xlarge",
     "r7i.16xlarge",
     "r7i.24xlarge",
     "r7i.2xlarge",
     "r7i.48xlarge",
     "r7i.4xlarge",
```

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/paginator.py` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/paginator.pyi` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/service_resource.py` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/service_resource.pyi` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/type_defs.py` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/type_defs.pyi` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/waiter.py` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2/waiter.pyi` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/PKG-INFO` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.71
-Summary: Type annotations for boto3.EC2 1.34.71 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.73
+Summary: Type annotations for boto3.EC2 1.34.73 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ec2-1.34.71/mypy_boto3_ec2.egg-info/SOURCES.txt` & `mypy-boto3-ec2-1.34.73/mypy_boto3_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.71/setup.py` & `mypy-boto3-ec2-1.34.73/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2",
-    version="1.34.71",
+    version="1.34.73",
     packages=["mypy_boto3_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EC2 1.34.71 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.EC2 1.34.73 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

