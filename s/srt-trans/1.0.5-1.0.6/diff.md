# Comparing `tmp/srt_trans-1.0.5.tar.gz` & `tmp/srt_trans-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-1.0.5.tar", last modified: Thu Apr  4 17:39:46 2024, max compression
+gzip compressed data, was "srt_trans-1.0.6.tar", last modified: Thu Apr  4 19:18:01 2024, max compression
```

## Comparing `srt_trans-1.0.5.tar` & `srt_trans-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 17:39:46.529905 srt_trans-1.0.5/
--rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1675 2024-04-04 17:39:46.526140 srt_trans-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1066 2024-04-04 02:09:13.000000 srt_trans-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 17:39:46.529905 srt_trans-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1045 2024-04-04 17:39:33.000000 srt_trans-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 17:39:46.477596 srt_trans-1.0.5/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.5/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     5807 2024-04-04 17:39:04.000000 srt_trans-1.0.5/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 17:39:46.521140 srt_trans-1.0.5/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1675 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 19:18:01.233057 srt_trans-1.0.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1873 2024-04-04 19:18:01.230050 srt_trans-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2024-04-04 19:01:00.000000 srt_trans-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:18:01.234046 srt_trans-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2024-04-04 19:17:53.000000 srt_trans-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:18:01.188693 srt_trans-1.0.6/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.6/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     7470 2024-04-04 19:06:00.000000 srt_trans-1.0.6/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:18:01.225522 srt_trans-1.0.6/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1873 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 19:18:01.000000 srt_trans-1.0.6/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 19:18:00.000000 srt_trans-1.0.6/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-1.0.5/LICENSE` & `srt_trans-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.5/PKG-INFO` & `srt_trans-1.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt_trans
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,22 @@
 
 ```bash
 Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
 Example:
     srt_trans ./test_video.mkv
     srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
     srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118
-    srt_trans ./test/test_file.srt
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-TW
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang ja
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-CN
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
+    srt_trans ./test_video.mkv -track_number 2
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW -track_number 2
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118 -track_number 2
+    srt_trans test_file.srt
+    srt_trans test_file.srt -src_lang en -dest_lang zh-TW
+    srt_trans test_file.srt -src_lang en -dest_lang ja
+    srt_trans test_file.srt -src_lang en -dest_lang zh-CN
+    srt_trans test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
 ```
 
 # Package
 ```bash
 pip install wheel
 python setup.py sdist bdist_wheel
 ```
```

### Comparing `srt_trans-1.0.5/README.md` & `srt_trans-1.0.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 
 ```bash
 Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
 Example:
     srt_trans ./test_video.mkv
     srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
     srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118
-    srt_trans ./test/test_file.srt
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-TW
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang ja
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-CN
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
+    srt_trans ./test_video.mkv -track_number 2
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW -track_number 2
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118 -track_number 2
+    srt_trans test_file.srt
+    srt_trans test_file.srt -src_lang en -dest_lang zh-TW
+    srt_trans test_file.srt -src_lang en -dest_lang ja
+    srt_trans test_file.srt -src_lang en -dest_lang zh-CN
+    srt_trans test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
 ```
 
 # Package
 ```bash
 pip install wheel
 python setup.py sdist bdist_wheel
 ```
```

### Comparing `srt_trans-1.0.5/setup.py` & `srt_trans-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
```

### Comparing `srt_trans-1.0.5/srt_trans/cli.py` & `srt_trans-1.0.6/srt_trans/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from googletrans import Translator
 import pysrt
 import os
 import sys
 import shutil
 import ffmpeg
 
-def extract_subtitles(video_file, output_srt):
+def extract_subtitles(video_file, output_srt, track_number = 1):
     # Extract subtitles using FFmpeg
     try:
         (
             ffmpeg
             .input(video_file)
-            .output(output_srt, f='srt')
+            .output(output_srt, map='s:' + str(track_number - 1))
             .run()
         )
         print(f'Subtitles extracted from {video_file} and saved to {output_srt}')
     except ffmpeg.Error as e:
         print(f'Error: {e}')
 
 
@@ -88,14 +88,17 @@
 def print_usage():
     print("""
         Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
         Example:
             srt_trans ./test_video.mkv
             srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
             srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118
+            srt_trans ./test_video.mkv -track_number 2
+            srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW -track_number 2
+            srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118 -track_number 2
             srt_trans test_file.srt
             srt_trans test_file.srt -src_lang en -dest_lang zh-TW
             srt_trans test_file.srt -src_lang en -dest_lang ja
             srt_trans test_file.srt -src_lang en -dest_lang zh-CN
             srt_trans test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
     """)
 
@@ -113,36 +116,64 @@
         print_usage()
         return
     input_file = sys.argv[1]
     if not os.path.exists(input_file):
         print(f"{input_file} not exists!")
         return
     
+    source_language = "en"      # Source language code (e.g., "en" for English)
+    target_language = "zh-CN"   # Target language code (e.g., "zh-CN" for Simple Chinese)
+    
     if str(input_file).lower().endswith(".mkv"):
         video_file = input_file
         input_file = video_file.replace(".mkv", ".srt")
-        extract_subtitles(video_file, input_file)
+        track_number = 1
+        if len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
+            source_language = sys.argv[3]
+            target_language = sys.argv[5]
+        elif len(sys.argv) == 8 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang" and sys.argv[6] == "-proxy":
+            source_language = sys.argv[3]
+            target_language = sys.argv[5]
+            proxy = sys.argv[7]
+            # Set environment variables (For example: "http://127.0.0.1:8118")
+            os.environ['http_proxy'] = proxy
+            os.environ['https_proxy'] = proxy
+        elif len(sys.argv) == 10 and sys.argv[2] == "-src_lang"  and sys.argv[4] == "-dest_lang"and sys.argv[6] == "-proxy" and sys.argv[8] == "-track_number":
+            source_language = sys.argv[3]
+            target_language = sys.argv[5]
+            proxy = sys.argv[7]
+            track_number = sys.argv[9]
+            # Set environment variables (For example: "http://127.0.0.1:8118")
+            os.environ['http_proxy'] = proxy
+            os.environ['https_proxy'] = proxy
+        else:
+            print("Invalid arguments!")
+            return
+        if not str(track_number).isdigit():
+            print("Invalid track_number, it should be an int!")
+            return
+        extract_subtitles(video_file, input_file, int(track_number))
+
+    else:
+        if len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
+            source_language = sys.argv[3]
+            target_language = sys.argv[5]
+        elif len(sys.argv) == 8 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang" and sys.argv[6] == "-proxy":
+            source_language = sys.argv[3]
+            target_language = sys.argv[5]
+            proxy = sys.argv[7]
+            # Set environment variables (For example: "http://127.0.0.1:8118")
+            os.environ['http_proxy'] = proxy
+            os.environ['https_proxy'] = proxy
+        else:
+            print("Invalid arguments!")
+            return
     
     pre_process_srt_file(input_file)
 
-    source_language = "en"      # Source language code (e.g., "en" for English)
-    target_language = "zh-CN"   # Target language code (e.g., "zh-CN" for Simple Chinese)
-    if len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
-        source_language = sys.argv[3]
-        target_language = sys.argv[5]
-    if len(sys.argv) == 8 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang" and sys.argv[6] == "-proxy":
-        source_language = sys.argv[3]
-        target_language = sys.argv[5]
-        proxy = sys.argv[7]
-        # Set environment variables (replace with your details)
-        # os.environ['http_proxy'] = "http://127.0.0.1:8118"
-        # os.environ['https_proxy'] = "http://127.0.0.1:8118"
-        os.environ['http_proxy'] = proxy
-        os.environ['https_proxy'] = proxy
-
     output_file = str(input_file).replace(".srt", f".{target_language}.srt")
     translate_result = translate_srt(input_file, output_file, source_language, target_language)
     if not translate_result:
         return
     
     os.remove(input_file)
     shutil.move(output_file, input_file)
```

### Comparing `srt_trans-1.0.5/srt_trans.egg-info/PKG-INFO` & `srt_trans-1.0.6/srt_trans.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-trans
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,22 @@
 
 ```bash
 Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
 Example:
     srt_trans ./test_video.mkv
     srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
     srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118
-    srt_trans ./test/test_file.srt
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-TW
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang ja
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-CN
-    srt_trans ./test/test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
+    srt_trans ./test_video.mkv -track_number 2
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW -track_number 2
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118 -track_number 2
+    srt_trans test_file.srt
+    srt_trans test_file.srt -src_lang en -dest_lang zh-TW
+    srt_trans test_file.srt -src_lang en -dest_lang ja
+    srt_trans test_file.srt -src_lang en -dest_lang zh-CN
+    srt_trans test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
 ```
 
 # Package
 ```bash
 pip install wheel
 python setup.py sdist bdist_wheel
 ```
```

