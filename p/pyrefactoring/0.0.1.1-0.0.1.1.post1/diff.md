# Comparing `tmp/pyrefactoring-0.0.1.1.tar.gz` & `tmp/pyrefactoring-0.0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefactoring-0.0.1.1.tar", last modified: Sun Mar 31 10:44:07 2024, max compression
+gzip compressed data, was "pyrefactoring-0.0.1.1.post1.tar", last modified: Thu Apr  4 02:04:46 2024, max compression
```

## Comparing `pyrefactoring-0.0.1.1.tar` & `pyrefactoring-0.0.1.1.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.115557 pyrefactoring-0.0.1.1/
--rw-r--r--   0 hieupth    (501) staff       (20)    11357 2024-03-27 12:52:17.000000 pyrefactoring-0.0.1.1/LICENSE
--rw-r--r--   0 hieupth    (501) staff       (20)      806 2024-03-31 10:44:07.115263 pyrefactoring-0.0.1.1/PKG-INFO
--rw-r--r--   0 hieupth    (501) staff       (20)      243 2024-03-27 12:52:17.000000 pyrefactoring-0.0.1.1/README.md
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.114985 pyrefactoring-0.0.1.1/pyrefactoring.egg-info/
--rw-r--r--   0 hieupth    (501) staff       (20)      806 2024-03-31 10:44:07.000000 pyrefactoring-0.0.1.1/pyrefactoring.egg-info/PKG-INFO
--rw-r--r--   0 hieupth    (501) staff       (20)      560 2024-03-31 10:44:07.000000 pyrefactoring-0.0.1.1/pyrefactoring.egg-info/SOURCES.txt
--rw-r--r--   0 hieupth    (501) staff       (20)        1 2024-03-31 10:44:07.000000 pyrefactoring-0.0.1.1/pyrefactoring.egg-info/dependency_links.txt
--rw-r--r--   0 hieupth    (501) staff       (20)        9 2024-03-31 10:44:07.000000 pyrefactoring-0.0.1.1/pyrefactoring.egg-info/top_level.txt
--rw-r--r--   0 hieupth    (501) staff       (20)        1 2024-03-27 14:41:43.000000 pyrefactoring-0.0.1.1/pyrefactoring.egg-info/zip-safe
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.111420 pyrefactoring-0.0.1.1/refactor/
--rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-03-27 12:52:17.000000 pyrefactoring-0.0.1.1/refactor/__init__.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.111556 pyrefactoring-0.0.1.1/refactor/app/
--rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-03-27 13:02:09.000000 pyrefactoring-0.0.1.1/refactor/app/__init__.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.112333 pyrefactoring-0.0.1.1/refactor/app/resources/
--rw-r--r--   0 hieupth    (501) staff       (20)       66 2024-03-27 13:06:21.000000 pyrefactoring-0.0.1.1/refactor/app/resources/__init__.py
--rw-r--r--   0 hieupth    (501) staff       (20)     2045 2024-03-27 12:59:06.000000 pyrefactoring-0.0.1.1/refactor/app/resources/abc.py
--rw-r--r--   0 hieupth    (501) staff       (20)     1810 2024-03-27 12:59:51.000000 pyrefactoring-0.0.1.1/refactor/app/resources/resource.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.113196 pyrefactoring-0.0.1.1/refactor/app/utils/
--rw-r--r--   0 hieupth    (501) staff       (20)       36 2024-03-31 10:35:50.000000 pyrefactoring-0.0.1.1/refactor/app/utils/__init__.py
--rw-r--r--   0 hieupth    (501) staff       (20)     1364 2024-03-31 10:34:12.000000 pyrefactoring-0.0.1.1/refactor/app/utils/semver.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.113795 pyrefactoring-0.0.1.1/refactor/common/
--rw-r--r--   0 hieupth    (501) staff       (20)       33 2024-03-05 18:01:45.000000 pyrefactoring-0.0.1.1/refactor/common/__init__.py
--rw-r--r--   0 hieupth    (501) staff       (20)     1874 2024-03-05 18:02:30.000000 pyrefactoring-0.0.1.1/refactor/common/processor.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.114097 pyrefactoring-0.0.1.1/refactor/dp/
--rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-03-27 12:52:17.000000 pyrefactoring-0.0.1.1/refactor/dp/__init__.py
-drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-03-31 10:44:07.114571 pyrefactoring-0.0.1.1/refactor/dp/creation/
--rw-r--r--   0 hieupth    (501) staff       (20)       33 2024-03-27 12:52:17.000000 pyrefactoring-0.0.1.1/refactor/dp/creation/__init__.py
--rw-r--r--   0 hieupth    (501) staff       (20)     1482 2024-03-27 12:52:17.000000 pyrefactoring-0.0.1.1/refactor/dp/creation/singleton.py
--rw-r--r--   0 hieupth    (501) staff       (20)       38 2024-03-31 10:44:07.115625 pyrefactoring-0.0.1.1/setup.cfg
--rw-r--r--   0 hieupth    (501) staff       (20)      873 2024-03-31 10:41:50.000000 pyrefactoring-0.0.1.1/setup.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.629231 pyrefactoring-0.0.1.1.post1/
+-rw-r--r--   0 hieupth    (501) staff       (20)    11357 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/LICENSE
+-rw-r--r--   0 hieupth    (501) staff       (20)      592 2024-04-04 02:04:46.628970 pyrefactoring-0.0.1.1.post1/PKG-INFO
+-rw-r--r--   0 hieupth    (501) staff       (20)      332 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/README.md
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.628764 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/
+-rw-r--r--   0 hieupth    (501) staff       (20)      592 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/PKG-INFO
+-rw-r--r--   0 hieupth    (501) staff       (20)      593 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/SOURCES.txt
+-rw-r--r--   0 hieupth    (501) staff       (20)        1 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/dependency_links.txt
+-rw-r--r--   0 hieupth    (501) staff       (20)        9 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/top_level.txt
+-rw-r--r--   0 hieupth    (501) staff       (20)        1 2024-04-04 02:04:46.000000 pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/zip-safe
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.626443 pyrefactoring-0.0.1.1.post1/refactor/
+-rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/__init__.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.626856 pyrefactoring-0.0.1.1.post1/refactor/common/
+-rw-r--r--   0 hieupth    (501) staff       (20)       33 2024-03-05 18:01:45.000000 pyrefactoring-0.0.1.1.post1/refactor/common/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     1874 2024-03-05 18:02:30.000000 pyrefactoring-0.0.1.1.post1/refactor/common/processor.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.627134 pyrefactoring-0.0.1.1.post1/refactor/patterns/
+-rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/patterns/__init__.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.627445 pyrefactoring-0.0.1.1.post1/refactor/patterns/creation/
+-rw-r--r--   0 hieupth    (501) staff       (20)       33 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/patterns/creation/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     1482 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/patterns/creation/singleton.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.627729 pyrefactoring-0.0.1.1.post1/refactor/utils/
+-rw-r--r--   0 hieupth    (501) staff       (20)        0 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/__init__.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.628234 pyrefactoring-0.0.1.1.post1/refactor/utils/resources/
+-rw-r--r--   0 hieupth    (501) staff       (20)       62 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/resources/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     2117 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/resources/abs.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     1812 2024-04-03 16:27:03.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/resources/base.py
+drwxr-xr-x   0 hieupth    (501) staff       (20)        0 2024-04-04 02:04:46.628589 pyrefactoring-0.0.1.1.post1/refactor/utils/versioning/
+-rw-r--r--   0 hieupth    (501) staff       (20)       27 2024-04-03 16:27:11.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/versioning/__init__.py
+-rw-r--r--   0 hieupth    (501) staff       (20)     1828 2024-04-03 16:27:11.000000 pyrefactoring-0.0.1.1.post1/refactor/utils/versioning/dot.py
+-rw-r--r--   0 hieupth    (501) staff       (20)       38 2024-04-04 02:04:46.629285 pyrefactoring-0.0.1.1.post1/setup.cfg
+-rw-r--r--   0 hieupth    (501) staff       (20)     2636 2024-04-03 16:26:45.000000 pyrefactoring-0.0.1.1.post1/setup.py
```

### Comparing `pyrefactoring-0.0.1.1/LICENSE` & `pyrefactoring-0.0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrefactoring-0.0.1.1/PKG-INFO` & `pyrefactoring-0.0.1.1.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 Metadata-Version: 2.1
 Name: pyrefactoring
-Version: 0.0.1.1
-Summary: Restructuring existing code from a mess into clean code and simple design
+Version: 0.0.1.1.post1
+Summary: Restructuring existing code from a mess into clean code, simple design and performance application
 Home-page: https://gitlab.com/hieupth/pyrefactor
 Author: Hieu Pham
 Author-email: 64821726+hieupth@users.noreply.github.com
 License: Copyright (c) 2023 Hieu Pham
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-# Python Refactoring
-Restructuring existing Python code from a mess into clean code and simple design application.
-## License
-[Apache License 2.0](LICENSE)<br>
-Copyright &copy; 2023 [Hieu Pham](https://github.com/hieupth). All rights reserved.
```

### Comparing `pyrefactoring-0.0.1.1/pyrefactoring.egg-info/PKG-INFO` & `pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 Metadata-Version: 2.1
 Name: pyrefactoring
-Version: 0.0.1.1
-Summary: Restructuring existing code from a mess into clean code and simple design
+Version: 0.0.1.1.post1
+Summary: Restructuring existing code from a mess into clean code, simple design and performance application
 Home-page: https://gitlab.com/hieupth/pyrefactor
 Author: Hieu Pham
 Author-email: 64821726+hieupth@users.noreply.github.com
 License: Copyright (c) 2023 Hieu Pham
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-# Python Refactoring
-Restructuring existing Python code from a mess into clean code and simple design application.
-## License
-[Apache License 2.0](LICENSE)<br>
-Copyright &copy; 2023 [Hieu Pham](https://github.com/hieupth). All rights reserved.
```

### Comparing `pyrefactoring-0.0.1.1/pyrefactoring.egg-info/SOURCES.txt` & `pyrefactoring-0.0.1.1.post1/pyrefactoring.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 setup.py
 pyrefactoring.egg-info/PKG-INFO
 pyrefactoring.egg-info/SOURCES.txt
 pyrefactoring.egg-info/dependency_links.txt
 pyrefactoring.egg-info/top_level.txt
 pyrefactoring.egg-info/zip-safe
 refactor/__init__.py
-refactor/app/__init__.py
-refactor/app/resources/__init__.py
-refactor/app/resources/abc.py
-refactor/app/resources/resource.py
-refactor/app/utils/__init__.py
-refactor/app/utils/semver.py
 refactor/common/__init__.py
 refactor/common/processor.py
-refactor/dp/__init__.py
-refactor/dp/creation/__init__.py
-refactor/dp/creation/singleton.py
+refactor/patterns/__init__.py
+refactor/patterns/creation/__init__.py
+refactor/patterns/creation/singleton.py
+refactor/utils/__init__.py
+refactor/utils/resources/__init__.py
+refactor/utils/resources/abs.py
+refactor/utils/resources/base.py
+refactor/utils/versioning/__init__.py
+refactor/utils/versioning/dot.py
```

### Comparing `pyrefactoring-0.0.1.1/refactor/app/resources/abc.py` & `pyrefactoring-0.0.1.1.post1/refactor/utils/resources/abs.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   Interface of resource which is used for load content from 
   various source such as file, base64 encoded or URL.
   """
 
   def __init__(self, ori: str):
     """
     Class constructor.
-    :param ori: origin source.
+    :param ori: origin source. Can be file, base64 encoded or URL.
     """
     self._ori: str = None
     self._hash: str = None
     self._data: bytes = None
     self._base64: str = None
     self.load(ori)
 
@@ -64,15 +64,15 @@
     """
     return self.hash == md5
 
   @abstractmethod
   def load(self, ori: str):
     """
     Load resource from origin source.
-    :param ori: origin source.
+    :param ori: origin source. Can be file, base64 encoded or URL.
     :return:    loaded resource.
     """
     self._ori = ori
     self._hash = None
     self._data = None
     self._base64 = None
     return self
```

### Comparing `pyrefactoring-0.0.1.1/refactor/app/resources/resource.py` & `pyrefactoring-0.0.1.1.post1/refactor/utils/resources/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
 import urllib.request
 from pathlib import Path
-from refactor.app.resources import ResourceInterface
+from refactor.utils.resources import ResourceInterface
 
 
 def from_file(res: ResourceInterface, ori: str) -> ResourceInterface:
   """
   Load resource data from file.
   :param res: resource to be loaded.
   :param ori: path to file.
```

### Comparing `pyrefactoring-0.0.1.1/refactor/common/processor.py` & `pyrefactoring-0.0.1.1.post1/refactor/common/processor.py`

 * *Files identical despite different names*

### Comparing `pyrefactoring-0.0.1.1/refactor/dp/creation/singleton.py` & `pyrefactoring-0.0.1.1.post1/refactor/patterns/creation/singleton.py`

 * *Files identical despite different names*

