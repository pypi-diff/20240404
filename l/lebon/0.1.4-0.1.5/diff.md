# Comparing `tmp/lebon-0.1.4.tar.gz` & `tmp/lebon-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lebon-0.1.4.tar", last modified: Thu Apr  4 14:02:19 2024, max compression
+gzip compressed data, was "lebon-0.1.5.tar", last modified: Thu Apr  4 14:21:10 2024, max compression
```

## Comparing `lebon-0.1.4.tar` & `lebon-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:02:19.257116 lebon-0.1.4/
--rw-rw-rw-   0        0        0     1736 2024-04-04 14:02:19.256059 lebon-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2024-04-04 13:58:34.000000 lebon-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 14:02:19.236332 lebon-0.1.4/lebon/
--rw-rw-rw-   0        0        0        0 2024-04-04 12:53:51.000000 lebon-0.1.4/lebon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:02:19.253859 lebon-0.1.4/lebon/assets/
--rw-rw-rw-   0        0        0       30 2024-04-04 12:50:55.000000 lebon-0.1.4/lebon/assets/data.json
--rw-rw-rw-   0        0        0      891 2024-04-04 12:44:33.000000 lebon-0.1.4/lebon/constants.py
--rw-rw-rw-   0        0        0     3084 2024-04-04 12:54:07.000000 lebon-0.1.4/lebon/main.py
--rw-rw-rw-   0        0        0     3021 2024-04-04 12:39:53.000000 lebon-0.1.4/lebon/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:02:19.249147 lebon-0.1.4/lebon.egg-info/
--rw-rw-rw-   0        0        0     1736 2024-04-04 14:02:19.000000 lebon-0.1.4/lebon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-04 14:02:19.000000 lebon-0.1.4/lebon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 14:02:19.000000 lebon-0.1.4/lebon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 14:02:19.000000 lebon-0.1.4/lebon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-04 14:02:19.000000 lebon-0.1.4/lebon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-04 14:02:19.000000 lebon-0.1.4/lebon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 14:02:19.257116 lebon-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      829 2024-04-04 13:59:34.000000 lebon-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:21:10.419913 lebon-0.1.5/
+-rw-rw-rw-   0        0        0     1736 2024-04-04 14:21:10.414912 lebon-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1406 2024-04-04 13:58:34.000000 lebon-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 14:21:10.394686 lebon-0.1.5/lebon/
+-rw-rw-rw-   0        0        0        0 2024-04-04 12:53:51.000000 lebon-0.1.5/lebon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:21:10.414912 lebon-0.1.5/lebon/assets/
+-rw-rw-rw-   0        0        0       30 2024-04-04 12:50:55.000000 lebon-0.1.5/lebon/assets/data.json
+-rw-rw-rw-   0        0        0      891 2024-04-04 12:44:33.000000 lebon-0.1.5/lebon/constants.py
+-rw-rw-rw-   0        0        0     3086 2024-04-04 14:21:00.000000 lebon-0.1.5/lebon/main.py
+-rw-rw-rw-   0        0        0     3021 2024-04-04 12:39:53.000000 lebon-0.1.5/lebon/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:21:10.414912 lebon-0.1.5/lebon.egg-info/
+-rw-rw-rw-   0        0        0     1736 2024-04-04 14:21:10.000000 lebon-0.1.5/lebon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-04 14:21:10.000000 lebon-0.1.5/lebon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 14:21:10.000000 lebon-0.1.5/lebon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 14:21:10.000000 lebon-0.1.5/lebon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-04 14:21:10.000000 lebon-0.1.5/lebon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-04 14:21:10.000000 lebon-0.1.5/lebon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 14:21:10.419913 lebon-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      829 2024-04-04 14:19:09.000000 lebon-0.1.5/setup.py
```

### Comparing `lebon-0.1.4/PKG-INFO` & `lebon-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lebon
-Version: 0.1.4
+Version: 0.1.5
 Summary: You are my sunshine, my only sunshine.
 Author: Lebon James
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lebon-0.1.4/README.md` & `lebon-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lebon-0.1.4/lebon/constants.py` & `lebon-0.1.5/lebon/constants.py`

 * *Files identical despite different names*

### Comparing `lebon-0.1.4/lebon/main.py` & `lebon-0.1.5/lebon/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 subprocess.run(["lebon"])
                 
             else:
                 _ = modify_env(True)
 
                 while True:
                     try:
-                        user_input = str(input(">"))
+                        user_input = str(input("ඞ"))
                         print("\033[H\033[J")
                         
                         if user_input == "":
                             clipboard_content = pyperclip.paste()
                             
                             if len(clipboard_content.strip(" "))<1:
                                 print("Clipboard is empty.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lebon-0.1.4/lebon/utils.py` & `lebon-0.1.5/lebon/utils.py`

 * *Files identical despite different names*

### Comparing `lebon-0.1.4/lebon.egg-info/PKG-INFO` & `lebon-0.1.5/lebon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lebon
-Version: 0.1.4
+Version: 0.1.5
 Summary: You are my sunshine, my only sunshine.
 Author: Lebon James
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lebon-0.1.4/setup.py` & `lebon-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lebon",
-    version="0.1.4",
+    version="0.1.5",
     author="Lebon James",
     description="You are my sunshine, my only sunshine.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["pyperclip", "google-generativeai", "pyautogui"],
     entry_points={
```

