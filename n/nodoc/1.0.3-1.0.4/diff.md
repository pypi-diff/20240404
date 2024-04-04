# Comparing `tmp/nodoc-1.0.3.tar.gz` & `tmp/nodoc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodoc-1.0.3.tar", last modified: Thu Apr  4 07:29:44 2024, max compression
+gzip compressed data, was "nodoc-1.0.4.tar", last modified: Thu Apr  4 07:39:50 2024, max compression
```

## Comparing `nodoc-1.0.3.tar` & `nodoc-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:29:44.012809 nodoc-1.0.3/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       36 2023-12-14 10:37:29.000000 nodoc-1.0.3/MANIFEST.in
--rw-r--r--   0 pengc     (1000) pengc     (1000)     7925 2024-04-04 07:29:44.011809 nodoc-1.0.3/PKG-INFO
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:29:44.008809 nodoc-1.0.3/nodoc/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     7476 2024-02-19 12:33:39.000000 nodoc-1.0.3/nodoc/README.md
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      559 2024-03-26 11:56:53.000000 nodoc-1.0.3/nodoc/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      925 2024-02-19 12:14:58.000000 nodoc-1.0.3/nodoc/const.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:29:44.009809 nodoc-1.0.3/nodoc/database/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       74 2023-12-14 10:08:59.000000 nodoc-1.0.3/nodoc/database/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     1936 2023-12-15 12:21:41.000000 nodoc-1.0.3/nodoc/database/database.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     7786 2023-12-15 12:31:37.000000 nodoc-1.0.3/nodoc/database/vectordb.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:29:44.009809 nodoc-1.0.3/nodoc/debugger/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       89 2023-12-14 10:08:59.000000 nodoc-1.0.3/nodoc/debugger/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     2748 2023-12-14 10:08:59.000000 nodoc-1.0.3/nodoc/debugger/decorator.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:29:44.011809 nodoc-1.0.3/nodoc/document/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      288 2024-03-26 11:56:53.000000 nodoc-1.0.3/nodoc/document/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     8310 2024-03-26 11:56:53.000000 nodoc-1.0.3/nodoc/document/_base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     2824 2024-03-26 11:56:53.000000 nodoc-1.0.3/nodoc/document/base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     3490 2024-03-26 11:56:53.000000 nodoc-1.0.3/nodoc/document/flow_processing.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     8050 2024-03-26 11:56:53.000000 nodoc-1.0.3/nodoc/document/markdown.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      348 2023-12-14 10:08:59.000000 nodoc-1.0.3/nodoc/document/pdf.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:29:44.011809 nodoc-1.0.3/nodoc/post_processing/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       55 2024-03-26 11:56:53.000000 nodoc-1.0.3/nodoc/post_processing/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      577 2024-03-26 11:56:53.000000 nodoc-1.0.3/nodoc/post_processing/_base.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     1924 2024-04-04 06:58:32.000000 nodoc-1.0.3/nodoc/setup.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:29:44.011809 nodoc-1.0.3/nodoc/structure/
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      173 2023-12-14 10:08:59.000000 nodoc-1.0.3/nodoc/structure/__init__.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)     8612 2024-02-19 12:29:29.000000 nodoc-1.0.3/nodoc/structure/doc_tree.py
--rw-rw-r--   0 pengc     (1000) pengc     (1000)    11993 2023-12-15 12:06:54.000000 nodoc-1.0.3/nodoc/structure/tree.py
-drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:29:44.011809 nodoc-1.0.3/nodoc.egg-info/
--rw-r--r--   0 pengc     (1000) pengc     (1000)     7925 2024-04-04 07:29:44.000000 nodoc-1.0.3/nodoc.egg-info/PKG-INFO
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      644 2024-04-04 07:29:44.000000 nodoc-1.0.3/nodoc.egg-info/SOURCES.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)        1 2024-04-04 07:29:44.000000 nodoc-1.0.3/nodoc.egg-info/dependency_links.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)        6 2024-04-04 07:29:44.000000 nodoc-1.0.3/nodoc.egg-info/top_level.txt
--rw-rw-r--   0 pengc     (1000) pengc     (1000)      469 2024-04-04 07:29:37.000000 nodoc-1.0.3/pyproject.toml
--rw-rw-r--   0 pengc     (1000) pengc     (1000)       38 2024-04-04 07:29:44.012809 nodoc-1.0.3/setup.cfg
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.770836 nodoc-1.0.4/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       36 2023-12-14 10:37:29.000000 nodoc-1.0.4/MANIFEST.in
+-rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 07:39:50.769836 nodoc-1.0.4/PKG-INFO
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.766836 nodoc-1.0.4/nodoc/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       39 2024-04-04 07:39:30.000000 nodoc-1.0.4/nodoc/__init__.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.767836 nodoc-1.0.4/nodoc/nodoc/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      559 2024-03-26 11:56:53.000000 nodoc-1.0.4/nodoc/nodoc/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      925 2024-02-19 12:14:58.000000 nodoc-1.0.4/nodoc/nodoc/const.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.767836 nodoc-1.0.4/nodoc/nodoc/database/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       74 2023-12-14 10:08:59.000000 nodoc-1.0.4/nodoc/nodoc/database/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     1936 2023-12-15 12:21:41.000000 nodoc-1.0.4/nodoc/nodoc/database/database.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     7786 2023-12-15 12:31:37.000000 nodoc-1.0.4/nodoc/nodoc/database/vectordb.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.767836 nodoc-1.0.4/nodoc/nodoc/debugger/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       89 2023-12-14 10:08:59.000000 nodoc-1.0.4/nodoc/nodoc/debugger/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     2748 2023-12-14 10:08:59.000000 nodoc-1.0.4/nodoc/nodoc/debugger/decorator.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.768836 nodoc-1.0.4/nodoc/nodoc/document/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      288 2024-03-26 11:56:53.000000 nodoc-1.0.4/nodoc/nodoc/document/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     8310 2024-03-26 11:56:53.000000 nodoc-1.0.4/nodoc/nodoc/document/_base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     2824 2024-03-26 11:56:53.000000 nodoc-1.0.4/nodoc/nodoc/document/base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     3490 2024-03-26 11:56:53.000000 nodoc-1.0.4/nodoc/nodoc/document/flow_processing.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     8050 2024-03-26 11:56:53.000000 nodoc-1.0.4/nodoc/nodoc/document/markdown.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      348 2023-12-14 10:08:59.000000 nodoc-1.0.4/nodoc/nodoc/document/pdf.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.768836 nodoc-1.0.4/nodoc/nodoc/post_processing/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       55 2024-03-26 11:56:53.000000 nodoc-1.0.4/nodoc/nodoc/post_processing/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      577 2024-03-26 11:56:53.000000 nodoc-1.0.4/nodoc/nodoc/post_processing/_base.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     1924 2024-04-04 06:58:32.000000 nodoc-1.0.4/nodoc/nodoc/setup.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.769836 nodoc-1.0.4/nodoc/nodoc/structure/
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      173 2023-12-14 10:08:59.000000 nodoc-1.0.4/nodoc/nodoc/structure/__init__.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)     8612 2024-02-19 12:29:29.000000 nodoc-1.0.4/nodoc/nodoc/structure/doc_tree.py
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)    11993 2023-12-15 12:06:54.000000 nodoc-1.0.4/nodoc/nodoc/structure/tree.py
+drwxrwxr-x   0 pengc     (1000) pengc     (1000)        0 2024-04-04 07:39:50.769836 nodoc-1.0.4/nodoc.egg-info/
+-rw-r--r--   0 pengc     (1000) pengc     (1000)      448 2024-04-04 07:39:50.000000 nodoc-1.0.4/nodoc.egg-info/PKG-INFO
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      760 2024-04-04 07:39:50.000000 nodoc-1.0.4/nodoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)        1 2024-04-04 07:39:50.000000 nodoc-1.0.4/nodoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)        6 2024-04-04 07:39:50.000000 nodoc-1.0.4/nodoc.egg-info/top_level.txt
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)      469 2024-04-04 07:39:44.000000 nodoc-1.0.4/pyproject.toml
+-rw-rw-r--   0 pengc     (1000) pengc     (1000)       38 2024-04-04 07:39:50.770836 nodoc-1.0.4/setup.cfg
```

### Comparing `nodoc-1.0.3/nodoc/__init__.py` & `nodoc-1.0.4/nodoc/nodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/const.py` & `nodoc-1.0.4/nodoc/nodoc/const.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/database/database.py` & `nodoc-1.0.4/nodoc/nodoc/database/database.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/database/vectordb.py` & `nodoc-1.0.4/nodoc/nodoc/database/vectordb.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/debugger/decorator.py` & `nodoc-1.0.4/nodoc/nodoc/debugger/decorator.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/document/_base.py` & `nodoc-1.0.4/nodoc/nodoc/document/_base.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/document/base.py` & `nodoc-1.0.4/nodoc/nodoc/document/base.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/document/flow_processing.py` & `nodoc-1.0.4/nodoc/nodoc/document/flow_processing.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/document/markdown.py` & `nodoc-1.0.4/nodoc/nodoc/document/markdown.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/post_processing/_base.py` & `nodoc-1.0.4/nodoc/nodoc/post_processing/_base.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/setup.py` & `nodoc-1.0.4/nodoc/nodoc/setup.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/structure/doc_tree.py` & `nodoc-1.0.4/nodoc/nodoc/structure/doc_tree.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc/structure/tree.py` & `nodoc-1.0.4/nodoc/nodoc/structure/tree.py`

 * *Files identical despite different names*

### Comparing `nodoc-1.0.3/nodoc.egg-info/SOURCES.txt` & `nodoc-1.0.4/nodoc.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 MANIFEST.in
 pyproject.toml
-nodoc/README.md
 nodoc/__init__.py
-nodoc/const.py
-nodoc/setup.py
 nodoc.egg-info/PKG-INFO
 nodoc.egg-info/SOURCES.txt
 nodoc.egg-info/dependency_links.txt
 nodoc.egg-info/top_level.txt
-nodoc/database/__init__.py
-nodoc/database/database.py
-nodoc/database/vectordb.py
-nodoc/debugger/__init__.py
-nodoc/debugger/decorator.py
-nodoc/document/__init__.py
-nodoc/document/_base.py
-nodoc/document/base.py
-nodoc/document/flow_processing.py
-nodoc/document/markdown.py
-nodoc/document/pdf.py
-nodoc/post_processing/__init__.py
-nodoc/post_processing/_base.py
-nodoc/structure/__init__.py
-nodoc/structure/doc_tree.py
-nodoc/structure/tree.py
+nodoc/nodoc/__init__.py
+nodoc/nodoc/const.py
+nodoc/nodoc/setup.py
+nodoc/nodoc/database/__init__.py
+nodoc/nodoc/database/database.py
+nodoc/nodoc/database/vectordb.py
+nodoc/nodoc/debugger/__init__.py
+nodoc/nodoc/debugger/decorator.py
+nodoc/nodoc/document/__init__.py
+nodoc/nodoc/document/_base.py
+nodoc/nodoc/document/base.py
+nodoc/nodoc/document/flow_processing.py
+nodoc/nodoc/document/markdown.py
+nodoc/nodoc/document/pdf.py
+nodoc/nodoc/post_processing/__init__.py
+nodoc/nodoc/post_processing/_base.py
+nodoc/nodoc/structure/__init__.py
+nodoc/nodoc/structure/doc_tree.py
+nodoc/nodoc/structure/tree.py
```

