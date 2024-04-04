# Comparing `tmp/qtlink-1.0.3.tar.gz` & `tmp/qtlink-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.0.3.tar", last modified: Wed Apr  3 13:09:03 2024, max compression
+gzip compressed data, was "qtlink-1.0.4.tar", last modified: Thu Apr  4 02:26:12 2024, max compression
```

## Comparing `qtlink-1.0.3.tar` & `qtlink-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:09:03.053912 qtlink-1.0.3/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      515 2024-04-03 13:09:03.051436 qtlink-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 13:09:03.011731 qtlink-1.0.3/qtlink/
--rw-rw-rw-   0        0        0       96 2024-04-03 13:09:00.000000 qtlink-1.0.3/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:09:03.041366 qtlink-1.0.3/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.0.3/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.0.3/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.0.3/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     1874 2024-04-03 12:51:18.000000 qtlink-1.0.3/qtlink/dialog/dialog_use_table.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:09:03.041366 qtlink-1.0.3/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.3/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     1887 2024-04-03 08:29:47.000000 qtlink-1.0.3/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:09:03.041366 qtlink-1.0.3/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.3/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     5621 2024-04-03 12:28:17.000000 qtlink-1.0.3/qtlink/table/multiple_select_table_controller.py
--rw-rw-rw-   0        0        0     1842 2024-04-03 09:55:09.000000 qtlink-1.0.3/qtlink/table/single_select_table_controller.py
--rw-rw-rw-   0        0        0     6187 2024-04-03 09:55:09.000000 qtlink-1.0.3/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0      182 2024-04-03 06:56:46.000000 qtlink-1.0.3/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:09:03.041366 qtlink-1.0.3/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.0.3/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.0.3/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.0.3/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:09:03.041366 qtlink-1.0.3/qtlink.egg-info/
--rw-rw-rw-   0        0        0      515 2024-04-03 13:09:02.000000 qtlink-1.0.3/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2024-04-03 13:09:03.000000 qtlink-1.0.3/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:09:02.000000 qtlink-1.0.3/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 13:09:02.000000 qtlink-1.0.3/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 13:09:02.000000 qtlink-1.0.3/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 13:09:03.053912 qtlink-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      660 2024-04-03 13:03:40.000000 qtlink-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:26:12.768996 qtlink-1.0.4/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-04 02:26:12.768996 qtlink-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 02:26:12.663324 qtlink-1.0.4/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-04 02:24:16.000000 qtlink-1.0.4/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:26:12.706123 qtlink-1.0.4/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.0.4/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1118 2024-04-03 12:51:18.000000 qtlink-1.0.4/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0      802 2024-04-03 12:51:18.000000 qtlink-1.0.4/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     1874 2024-04-03 12:51:18.000000 qtlink-1.0.4/qtlink/dialog/dialog_use_table.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:26:12.721737 qtlink-1.0.4/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.4/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     1887 2024-04-03 08:29:47.000000 qtlink-1.0.4/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:26:12.752982 qtlink-1.0.4/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.0.4/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     5621 2024-04-03 12:28:17.000000 qtlink-1.0.4/qtlink/table/multiple_select_table_controller.py
+-rw-rw-rw-   0        0        0     1842 2024-04-03 09:55:09.000000 qtlink-1.0.4/qtlink/table/single_select_table_controller.py
+-rw-rw-rw-   0        0        0     6187 2024-04-03 09:55:09.000000 qtlink-1.0.4/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     3645 2024-04-04 02:24:16.000000 qtlink-1.0.4/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:26:12.768996 qtlink-1.0.4/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.0.4/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-04-03 09:55:09.000000 qtlink-1.0.4/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     3501 2024-04-03 09:06:49.000000 qtlink-1.0.4/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:26:12.768996 qtlink-1.0.4/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-04 02:26:12.000000 qtlink-1.0.4/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2024-04-04 02:26:12.000000 qtlink-1.0.4/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 02:26:12.000000 qtlink-1.0.4/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-04 02:26:12.000000 qtlink-1.0.4/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-04 02:26:12.000000 qtlink-1.0.4/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 02:26:12.768996 qtlink-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      660 2024-04-04 02:25:55.000000 qtlink-1.0.4/setup.py
```

### Comparing `qtlink-1.0.3/LICENSE` & `qtlink-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/PKG-INFO` & `qtlink-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.0.3
+Version: 1.0.4
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.0.3/qtlink/dialog/dialog_choice.py` & `qtlink-1.0.4/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink/dialog/dialog_info.py` & `qtlink-1.0.4/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink/dialog/dialog_use_table.py` & `qtlink-1.0.4/qtlink/dialog/dialog_use_table.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.0.4/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink/table/multiple_select_table_controller.py` & `qtlink-1.0.4/qtlink/table/multiple_select_table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink/table/single_select_table_controller.py` & `qtlink-1.0.4/qtlink/table/single_select_table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink/table/table_controller.py` & `qtlink-1.0.4/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink/widgets/drop_widget.py` & `qtlink-1.0.4/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink/widgets/list_widget.py` & `qtlink-1.0.4/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/qtlink.egg-info/PKG-INFO` & `qtlink-1.0.4/qtlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtlink
-Version: 1.0.3
+Version: 1.0.4
 Summary: a ui framework based on pyside6
 Home-page: https://gitee.com/darlingxyz/qtlink
 Author: NanHaiLoong
 Author-email: nanhai@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qtlink-1.0.3/qtlink.egg-info/SOURCES.txt` & `qtlink-1.0.4/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.0.3/setup.py` & `qtlink-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.0.3",
+    version="1.0.4",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6', 'matplotlib', 'numpy'],
```

