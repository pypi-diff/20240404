# Comparing `tmp/srt_trans-1.0.6.tar.gz` & `tmp/srt_trans-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-1.0.6.tar", last modified: Thu Apr  4 19:18:01 2024, max compression
+gzip compressed data, was "srt_trans-1.0.7.tar", last modified: Thu Apr  4 19:27:46 2024, max compression
```

## Comparing `srt_trans-1.0.6.tar` & `srt_trans-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 19:18:01.233057 srt_trans-1.0.6/
--rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     1873 2024-04-04 19:18:01.230050 srt_trans-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2024-04-04 19:01:00.000000 srt_trans-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 19:18:01.234046 srt_trans-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1045 2024-04-04 19:17:53.000000 srt_trans-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:18:01.188693 srt_trans-1.0.6/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.6/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     7470 2024-04-04 19:06:00.000000 srt_trans-1.0.6/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:18:01.225522 srt_trans-1.0.6/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1873 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 19:18:01.000000 srt_trans-1.0.6/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 19:27:46.524698 srt_trans-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1873 2024-04-04 19:27:46.519679 srt_trans-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2024-04-04 19:01:00.000000 srt_trans-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:27:46.524698 srt_trans-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2024-04-04 19:27:21.000000 srt_trans-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:27:46.481453 srt_trans-1.0.7/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.7/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     7587 2024-04-04 19:27:05.000000 srt_trans-1.0.7/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:27:46.519679 srt_trans-1.0.7/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1873 2024-04-04 19:27:46.000000 srt_trans-1.0.7/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 19:27:46.000000 srt_trans-1.0.7/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:27:46.000000 srt_trans-1.0.7/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 19:27:46.000000 srt_trans-1.0.7/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 19:27:46.000000 srt_trans-1.0.7/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 19:27:46.000000 srt_trans-1.0.7/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-1.0.6/LICENSE` & `srt_trans-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.6/PKG-INFO` & `srt_trans-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt_trans
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `srt_trans-1.0.6/README.md` & `srt_trans-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.6/setup.py` & `srt_trans-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
```

### Comparing `srt_trans-1.0.6/srt_trans/cli.py` & `srt_trans-1.0.7/srt_trans/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,18 +120,20 @@
         print(f"{input_file} not exists!")
         return
     
     source_language = "en"      # Source language code (e.g., "en" for English)
     target_language = "zh-CN"   # Target language code (e.g., "zh-CN" for Simple Chinese)
     
     if str(input_file).lower().endswith(".mkv"):
-        video_file = input_file
-        input_file = video_file.replace(".mkv", ".srt")
         track_number = 1
-        if len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
+        video_file = ""
+        if len(sys.argv) == 2:
+            video_file = input_file
+            input_file = video_file.replace(".mkv", ".srt")
+        elif len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
             source_language = sys.argv[3]
             target_language = sys.argv[5]
         elif len(sys.argv) == 8 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang" and sys.argv[6] == "-proxy":
             source_language = sys.argv[3]
             target_language = sys.argv[5]
             proxy = sys.argv[7]
             # Set environment variables (For example: "http://127.0.0.1:8118")
@@ -148,17 +150,18 @@
         else:
             print("Invalid arguments!")
             return
         if not str(track_number).isdigit():
             print("Invalid track_number, it should be an int!")
             return
         extract_subtitles(video_file, input_file, int(track_number))
-
     else:
-        if len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
+        if len(sys.argv) == 2:
+            pass
+        elif len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
             source_language = sys.argv[3]
             target_language = sys.argv[5]
         elif len(sys.argv) == 8 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang" and sys.argv[6] == "-proxy":
             source_language = sys.argv[3]
             target_language = sys.argv[5]
             proxy = sys.argv[7]
             # Set environment variables (For example: "http://127.0.0.1:8118")
```

### Comparing `srt_trans-1.0.6/srt_trans.egg-info/PKG-INFO` & `srt_trans-1.0.7/srt_trans.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-trans
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

