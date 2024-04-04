# Comparing `tmp/ofdcomparer-1.5.36.tar.gz` & `tmp/ofdcomparer-1.5.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofdcomparer-1.5.36.tar", last modified: Sat Mar  9 15:40:20 2024, max compression
+gzip compressed data, was "ofdcomparer-1.5.37.tar", last modified: Thu Apr  4 19:16:01 2024, max compression
```

## Comparing `ofdcomparer-1.5.36.tar` & `ofdcomparer-1.5.37.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 15:40:20.917817 ofdcomparer-1.5.36/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 13:19:58.000000 ofdcomparer-1.5.36/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1567 2024-03-09 15:40:20.917817 ofdcomparer-1.5.36/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-01 17:56:55.000000 ofdcomparer-1.5.36/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 15:40:20.916817 ofdcomparer-1.5.36/ofdcomparer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 13:19:58.000000 ofdcomparer-1.5.36/ofdcomparer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-12 13:37:12.000000 ofdcomparer-1.5.36/ofdcomparer/allure_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    21525 2024-03-09 15:40:06.000000 ofdcomparer-1.5.36/ofdcomparer/compare_ffd.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-10-19 13:19:58.000000 ofdcomparer-1.5.36/ofdcomparer/configs.py
--rw-rw-rw-   0 root         (0) root         (0)    13980 2024-01-12 14:45:58.000000 ofdcomparer-1.5.36/ofdcomparer/convert.py
--rw-rw-rw-   0 root         (0) root         (0)    39605 2024-02-01 18:04:25.000000 ofdcomparer-1.5.36/ofdcomparer/dto10.py
--rw-rw-rw-   0 root         (0) root         (0)    33848 2024-01-18 12:27:58.000000 ofdcomparer-1.5.36/ofdcomparer/dto_error_descriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8301 2024-01-23 20:47:59.000000 ofdcomparer-1.5.36/ofdcomparer/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    86878 2024-01-12 15:42:14.000000 ofdcomparer-1.5.36/ofdcomparer/libfptr10.py
--rw-rw-rw-   0 root         (0) root         (0)     1563 2024-01-12 13:37:12.000000 ofdcomparer-1.5.36/ofdcomparer/ofd_cri_atol.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-12 14:45:58.000000 ofdcomparer-1.5.36/ofdcomparer/ofd_taxcom.py
--rw-rw-rw-   0 root         (0) root         (0)    39179 2024-01-23 20:47:59.000000 ofdcomparer-1.5.36/ofdcomparer/tags_fn.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2024-03-09 15:40:06.000000 ofdcomparer-1.5.36/ofdcomparer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 15:40:20.917817 ofdcomparer-1.5.36/ofdcomparer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2024-03-09 15:40:20.000000 ofdcomparer-1.5.36/ofdcomparer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2024-03-09 15:40:20.000000 ofdcomparer-1.5.36/ofdcomparer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-09 15:40:20.000000 ofdcomparer-1.5.36/ofdcomparer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-09 15:40:20.000000 ofdcomparer-1.5.36/ofdcomparer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-09 15:40:20.000000 ofdcomparer-1.5.36/ofdcomparer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-09 15:40:20.918817 ofdcomparer-1.5.36/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-03-09 15:40:06.000000 ofdcomparer-1.5.36/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:16:01.445798 ofdcomparer-1.5.37/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 22:27:07.000000 ofdcomparer-1.5.37/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-04 19:16:01.445798 ofdcomparer-1.5.37/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-15 14:23:23.000000 ofdcomparer-1.5.37/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:16:01.442798 ofdcomparer-1.5.37/ofdcomparer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 22:27:07.000000 ofdcomparer-1.5.37/ofdcomparer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/allure_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    21525 2024-04-04 19:15:02.000000 ofdcomparer-1.5.37/ofdcomparer/compare_ffd.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-10-19 22:27:07.000000 ofdcomparer-1.5.37/ofdcomparer/configs.py
+-rw-rw-rw-   0 root         (0) root         (0)    13980 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    39605 2024-03-06 23:14:00.000000 ofdcomparer-1.5.37/ofdcomparer/dto10.py
+-rw-rw-rw-   0 root         (0) root         (0)    33848 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/dto_error_descriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8301 2024-03-06 23:14:00.000000 ofdcomparer-1.5.37/ofdcomparer/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/ofd_cri_atol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/ofd_taxcom.py
+-rw-rw-rw-   0 root         (0) root         (0)    39179 2024-03-06 23:14:00.000000 ofdcomparer-1.5.37/ofdcomparer/tags_fn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-04 19:15:02.000000 ofdcomparer-1.5.37/ofdcomparer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:16:01.444798 ofdcomparer-1.5.37/ofdcomparer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-04 19:16:01.445798 ofdcomparer-1.5.37/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-04 19:15:02.000000 ofdcomparer-1.5.37/setup.py
```

### Comparing `ofdcomparer-1.5.36/PKG-INFO` & `ofdcomparer-1.5.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.36
+Version: 1.5.37
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.36/README.md` & `ofdcomparer-1.5.37/README.md`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer/compare_ffd.py` & `ofdcomparer-1.5.37/ofdcomparer/compare_ffd.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         if rnm is None:
             rnm = self.DTO10.registrationNumber
         if fn is None:
             fn = self.DTO10.fnSerial
         if fd is None:
             fd = self.DTO10.get_fd_from_fn(self.DTO10.get_last_fd_number())
         if bool(changes):
-            fn = self.dict_modifier.change_values_in_dict(fd, changes)
+            fd = self.dict_modifier.change_values_in_dict(fd, changes)
         self.DTO10.wait_for_sent_all_fd()
         self.compare_tags(rnm=rnm, fn=fn, fd=fd)
         self.output_result_to_log()
         if self.is_have_failed():
             return False
         return True
```

### Comparing `ofdcomparer-1.5.36/ofdcomparer/convert.py` & `ofdcomparer-1.5.37/ofdcomparer/convert.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer/dto10.py` & `ofdcomparer-1.5.37/ofdcomparer/dto10.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer/dto_error_descriptions.py` & `ofdcomparer-1.5.37/ofdcomparer/dto_error_descriptions.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer/helpers.py` & `ofdcomparer-1.5.37/ofdcomparer/helpers.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer/ofd_cri_atol.py` & `ofdcomparer-1.5.37/ofdcomparer/ofd_cri_atol.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer/ofd_taxcom.py` & `ofdcomparer-1.5.37/ofdcomparer/ofd_taxcom.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer/tags_fn.py` & `ofdcomparer-1.5.37/ofdcomparer/tags_fn.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer/utils.py` & `ofdcomparer-1.5.37/ofdcomparer/utils.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.36/ofdcomparer.egg-info/PKG-INFO` & `ofdcomparer-1.5.37/ofdcomparer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.36
+Version: 1.5.37
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.36/ofdcomparer.egg-info/SOURCES.txt` & `ofdcomparer-1.5.37/ofdcomparer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 ofdcomparer/allure_helper.py
 ofdcomparer/compare_ffd.py
 ofdcomparer/configs.py
 ofdcomparer/convert.py
 ofdcomparer/dto10.py
 ofdcomparer/dto_error_descriptions.py
 ofdcomparer/helpers.py
-ofdcomparer/libfptr10.py
 ofdcomparer/ofd_cri_atol.py
 ofdcomparer/ofd_taxcom.py
 ofdcomparer/tags_fn.py
 ofdcomparer/utils.py
 ofdcomparer.egg-info/PKG-INFO
 ofdcomparer.egg-info/SOURCES.txt
 ofdcomparer.egg-info/dependency_links.txt
```

### Comparing `ofdcomparer-1.5.36/setup.py` & `ofdcomparer-1.5.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ofdcomparer",
-    version="1.5.36",
+    version="1.5.37",
     long_description=long_description,
     description="Библиотека для сравнивания ФД из ФН и ОФД",
     packages=["ofdcomparer"],
     author_email="k.kabisova@atol.ru",
     install_requires=[
         "requests==2.31.0",
         "requests-toolbelt==1.0.0",
```

