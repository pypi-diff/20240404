# Comparing `tmp/yuag-0.0.59.tar.gz` & `tmp/yuag-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.59.tar", last modified: Tue Apr  2 14:50:53 2024, max compression
+gzip compressed data, was "yuag-0.0.60.tar", last modified: Thu Apr  4 15:32:56 2024, max compression
```

## Comparing `yuag-0.0.59.tar` & `yuag-0.0.60.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:50:53.298126 yuag-0.0.59/
--rw-rw-rw-   0        0        0       52 2024-04-02 14:50:53.296127 yuag-0.0.59/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 14:50:53.298126 yuag-0.0.59/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-04-02 14:50:34.000000 yuag-0.0.59/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:50:53.270919 yuag-0.0.59/yuag/
--rw-rw-rw-   0        0        0     2619 2024-04-01 20:27:54.000000 yuag-0.0.59/yuag/__init__.py
--rw-rw-rw-   0        0        0    30968 2024-04-02 14:19:18.000000 yuag-0.0.59/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:50:53.294132 yuag-0.0.59/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-04-02 14:50:52.000000 yuag-0.0.59/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-02 14:50:53.000000 yuag-0.0.59/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:50:52.000000 yuag-0.0.59/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 14:50:52.000000 yuag-0.0.59/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 15:32:56.071735 yuag-0.0.60/
+-rw-rw-rw-   0        0        0       52 2024-04-04 15:32:56.068737 yuag-0.0.60/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:32:56.071735 yuag-0.0.60/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-04-04 15:32:48.000000 yuag-0.0.60/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:32:56.037712 yuag-0.0.60/yuag/
+-rw-rw-rw-   0        0        0     2619 2024-04-01 20:27:54.000000 yuag-0.0.60/yuag/__init__.py
+-rw-rw-rw-   0        0        0    31119 2024-04-04 15:32:31.000000 yuag-0.0.60/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:32:56.067736 yuag-0.0.60/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-04-04 15:32:55.000000 yuag-0.0.60/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-04 15:32:55.000000 yuag-0.0.60/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:32:55.000000 yuag-0.0.60/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-04 15:32:55.000000 yuag-0.0.60/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.59/yuag/__init__.py` & `yuag-0.0.60/yuag/__init__.py`

 * *Files identical despite different names*

### Comparing `yuag-0.0.59/yuag/yuag.py` & `yuag-0.0.60/yuag/yuag.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,14 +675,23 @@
 
 def removeSpaces(text: str): # إلغاء   المسافات
     text = " ".join(RemoveDuplicates(text.split(" "), 1, 1, ""))
     text = " ".join(removeFromArr(text.split(" "), -1, ""))
     return text.strip()
 
 def replaceText(text: str, replArr: list): # text = "hello word!", replArr = [ ["word", "world"], ["!", "."] ] ==> "hello world."
+    """
+    ```
+    text = "hello word!"
+    replArr = [ ["word", "world"], ["!", "."] ]
+    ```
+    \n\n
+    ==> "hello world."
+    """
+    
     i = 0
     while i < len(replArr):
         text = text.replace(replArr[i][0], replArr[i][1])
         i += 1
 
     return text
```

