# Comparing `tmp/jb_news-2.0.3-py3-none-any.whl.zip` & `tmp/jb_news-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,6 @@
-Zip file size: 4881 bytes, number of entries: 7
--rw-r--r--  2.0 unx     6148 b- defN 24-Feb-11 02:47 .DS_Store
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-27 19:20 jb_news/__init__.py
--rw-r--r--  2.0 unx    11418 b- defN 24-Mar-04 21:22 jb_news/news.py
--rw-r--r--  2.0 unx     2739 b- defN 24-Mar-04 21:36 jb_news-2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-04 21:36 jb_news-2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Mar-04 21:36 jb_news-2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      509 b- defN 24-Mar-04 21:36 jb_news-2.0.3.dist-info/RECORD
-7 files, 20914 bytes uncompressed, 3985 bytes compressed:  80.9%
+Zip file size: 2035 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2739 b- defN 24-Apr-03 23:45 jb_news-2.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 23:45 jb_news-2.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 23:45 jb_news-2.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      297 b- defN 24-Apr-03 23:45 jb_news-2.1.0.dist-info/RECORD
+4 files, 3129 bytes uncompressed, 1453 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -1,22 +1,13 @@
-Filename: .DS_Store
+Filename: jb_news-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: jb_news/__init__.py
+Filename: jb_news-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: jb_news/news.py
+Filename: jb_news-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jb_news-2.0.3.dist-info/METADATA
-Comment: 
-
-Filename: jb_news-2.0.3.dist-info/WHEEL
-Comment: 
-
-Filename: jb_news-2.0.3.dist-info/top_level.txt
-Comment: 
-
-Filename: jb_news-2.0.3.dist-info/RECORD
+Filename: jb_news-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `jb_news-2.0.3.dist-info/METADATA` & `jb_news-2.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jb-news
-Version: 2.0.3
+Version: 2.1.0
 Summary: A comprehensive wrapper for JBlanked's News API, leveraging OpenAI, Machine Learning, and MQL5's Calendar.
 Home-page: https://jblanked.com/news/api/docs/
 Author: JBlanked
 License: MIT
 Description-Content-Type: text/markdown
 
 # JB-News
```

