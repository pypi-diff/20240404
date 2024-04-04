# Comparing `tmp/nodoc-1.0.6.tar.gz` & `tmp/nodoc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodoc-1.0.6.tar", last modified: Thu Apr  4 08:04:22 2024, max compression
+gzip compressed data, was "nodoc-1.0.7.tar", last modified: Thu Apr  4 08:09:24 2024, max compression
```

## Comparing `nodoc-1.0.6.tar` & `nodoc-1.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.299902 nodoc-1.0.6/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       36 2023-12-14 10:37:29.000000 nodoc-1.0.6/MANIFEST.in
--rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 08:04:22.299902 nodoc-1.0.6/PKG-INFO
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.296902 nodoc-1.0.6/nodoc/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      379 2024-04-04 07:45:42.000000 nodoc-1.0.6/nodoc/__init__.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.297902 nodoc-1.0.6/nodoc/nodoc/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      559 2024-03-26 11:56:53.000000 nodoc-1.0.6/nodoc/nodoc/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      925 2024-02-19 12:14:58.000000 nodoc-1.0.6/nodoc/nodoc/const.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.297902 nodoc-1.0.6/nodoc/nodoc/database/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       74 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/database/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     1936 2023-12-15 12:21:41.000000 nodoc-1.0.6/nodoc/nodoc/database/database.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     7786 2023-12-15 12:31:37.000000 nodoc-1.0.6/nodoc/nodoc/database/vectordb.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.297902 nodoc-1.0.6/nodoc/nodoc/debugger/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       89 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/debugger/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     2748 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/debugger/decorator.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.298902 nodoc-1.0.6/nodoc/nodoc/document/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      331 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     8387 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/_base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     3068 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     3587 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/flow_processing.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)    10250 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/document/markdown.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      348 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/document/pdf.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.298902 nodoc-1.0.6/nodoc/nodoc/post_processing/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       55 2024-03-26 11:56:53.000000 nodoc-1.0.6/nodoc/nodoc/post_processing/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      577 2024-03-26 11:56:53.000000 nodoc-1.0.6/nodoc/nodoc/post_processing/_base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     1924 2024-04-04 06:58:32.000000 nodoc-1.0.6/nodoc/nodoc/setup.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.298902 nodoc-1.0.6/nodoc/nodoc/structure/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      173 2023-12-14 10:08:59.000000 nodoc-1.0.6/nodoc/nodoc/structure/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     8365 2024-04-04 08:03:49.000000 nodoc-1.0.6/nodoc/nodoc/structure/doc_tree.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)    11993 2023-12-15 12:06:54.000000 nodoc-1.0.6/nodoc/nodoc/structure/tree.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:04:22.299902 nodoc-1.0.6/nodoc.egg-info/
--rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 08:04:22.000000 nodoc-1.0.6/nodoc.egg-info/PKG-INFO
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      760 2024-04-04 08:04:22.000000 nodoc-1.0.6/nodoc.egg-info/SOURCES.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)        1 2024-04-04 08:04:22.000000 nodoc-1.0.6/nodoc.egg-info/dependency_links.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)        6 2024-04-04 08:04:22.000000 nodoc-1.0.6/nodoc.egg-info/top_level.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      469 2024-04-04 08:04:09.000000 nodoc-1.0.6/pyproject.toml
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       38 2024-04-04 08:04:22.299902 nodoc-1.0.6/setup.cfg
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.131915 nodoc-1.0.7/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       36 2023-12-14 10:37:29.000000 nodoc-1.0.7/MANIFEST.in
+-rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 08:09:24.131915 nodoc-1.0.7/PKG-INFO
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.127915 nodoc-1.0.7/nodoc/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      379 2024-04-04 08:07:19.000000 nodoc-1.0.7/nodoc/__init__.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.128915 nodoc-1.0.7/nodoc/nodoc/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      559 2024-03-26 11:56:53.000000 nodoc-1.0.7/nodoc/nodoc/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      925 2024-02-19 12:14:58.000000 nodoc-1.0.7/nodoc/nodoc/const.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.129915 nodoc-1.0.7/nodoc/nodoc/database/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       74 2023-12-14 10:08:59.000000 nodoc-1.0.7/nodoc/nodoc/database/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     1936 2023-12-15 12:21:41.000000 nodoc-1.0.7/nodoc/nodoc/database/database.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     7786 2023-12-15 12:31:37.000000 nodoc-1.0.7/nodoc/nodoc/database/vectordb.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.129915 nodoc-1.0.7/nodoc/nodoc/debugger/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       89 2023-12-14 10:08:59.000000 nodoc-1.0.7/nodoc/nodoc/debugger/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     2748 2023-12-14 10:08:59.000000 nodoc-1.0.7/nodoc/nodoc/debugger/decorator.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.130915 nodoc-1.0.7/nodoc/nodoc/document/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      331 2024-04-04 08:03:49.000000 nodoc-1.0.7/nodoc/nodoc/document/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     8387 2024-04-04 08:03:49.000000 nodoc-1.0.7/nodoc/nodoc/document/_base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     3068 2024-04-04 08:03:49.000000 nodoc-1.0.7/nodoc/nodoc/document/base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     3587 2024-04-04 08:03:49.000000 nodoc-1.0.7/nodoc/nodoc/document/flow_processing.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)    10250 2024-04-04 08:03:49.000000 nodoc-1.0.7/nodoc/nodoc/document/markdown.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      348 2023-12-14 10:08:59.000000 nodoc-1.0.7/nodoc/nodoc/document/pdf.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.130915 nodoc-1.0.7/nodoc/nodoc/post_processing/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       55 2024-03-26 11:56:53.000000 nodoc-1.0.7/nodoc/nodoc/post_processing/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      577 2024-03-26 11:56:53.000000 nodoc-1.0.7/nodoc/nodoc/post_processing/_base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     1924 2024-04-04 06:58:32.000000 nodoc-1.0.7/nodoc/nodoc/setup.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.130915 nodoc-1.0.7/nodoc/nodoc/structure/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      173 2023-12-14 10:08:59.000000 nodoc-1.0.7/nodoc/nodoc/structure/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     8365 2024-04-04 08:03:49.000000 nodoc-1.0.7/nodoc/nodoc/structure/doc_tree.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)    11993 2023-12-15 12:06:54.000000 nodoc-1.0.7/nodoc/nodoc/structure/tree.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 08:09:24.131915 nodoc-1.0.7/nodoc.egg-info/
+-rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 08:09:24.000000 nodoc-1.0.7/nodoc.egg-info/PKG-INFO
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      760 2024-04-04 08:09:24.000000 nodoc-1.0.7/nodoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)        1 2024-04-04 08:09:24.000000 nodoc-1.0.7/nodoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)        6 2024-04-04 08:09:24.000000 nodoc-1.0.7/nodoc.egg-info/top_level.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      469 2024-04-04 08:09:03.000000 nodoc-1.0.7/pyproject.toml
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       38 2024-04-04 08:09:24.131915 nodoc-1.0.7/setup.cfg
```

### Comparing `nodoc-1.0.6/nodoc/nodoc/__init__.py` & `nodoc-1.0.7/nodoc/nodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/const.py` & `nodoc-1.0.7/nodoc/nodoc/const.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/database/database.py` & `nodoc-1.0.7/nodoc/nodoc/database/database.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/database/vectordb.py` & `nodoc-1.0.7/nodoc/nodoc/database/vectordb.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/debugger/decorator.py` & `nodoc-1.0.7/nodoc/nodoc/debugger/decorator.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/document/_base.py` & `nodoc-1.0.7/nodoc/nodoc/document/_base.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/document/base.py` & `nodoc-1.0.7/nodoc/nodoc/document/base.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/document/flow_processing.py` & `nodoc-1.0.7/nodoc/nodoc/document/flow_processing.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/document/markdown.py` & `nodoc-1.0.7/nodoc/nodoc/document/markdown.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/post_processing/_base.py` & `nodoc-1.0.7/nodoc/nodoc/post_processing/_base.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/setup.py` & `nodoc-1.0.7/nodoc/nodoc/setup.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/structure/doc_tree.py` & `nodoc-1.0.7/nodoc/nodoc/structure/doc_tree.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc/nodoc/structure/tree.py` & `nodoc-1.0.7/nodoc/nodoc/structure/tree.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.6/nodoc.egg-info/SOURCES.txt` & `nodoc-1.0.7/nodoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

