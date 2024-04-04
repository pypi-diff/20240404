# Comparing `tmp/srt_trans-0.1.2.tar.gz` & `tmp/srt_trans-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-0.1.2.tar", last modified: Thu Apr  4 01:05:08 2024, max compression
+gzip compressed data, was "srt_trans-1.0.0.tar", last modified: Thu Apr  4 02:10:23 2024, max compression
```

## Comparing `srt_trans-0.1.2.tar` & `srt_trans-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 01:05:08.676356 srt_trans-0.1.2/
--rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1490 2024-04-04 01:05:08.674347 srt_trans-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      881 2024-04-04 00:36:54.000000 srt_trans-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 01:05:08.676356 srt_trans-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-04 01:04:26.000000 srt_trans-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:05:08.625591 srt_trans-0.1.2/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-0.1.2/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     3708 2024-04-04 01:02:18.000000 srt_trans-0.1.2/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:05:08.670804 srt_trans-0.1.2/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1490 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 02:10:23.809766 srt_trans-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1675 2024-04-04 02:10:23.807764 srt_trans-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2024-04-04 02:09:13.000000 srt_trans-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 02:10:23.809766 srt_trans-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2024-04-04 02:07:55.000000 srt_trans-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:10:23.766196 srt_trans-1.0.0/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.0/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     4455 2024-04-04 02:10:00.000000 srt_trans-1.0.0/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:10:23.804750 srt_trans-1.0.0/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1675 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-0.1.2/LICENSE` & `srt_trans-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-0.1.2/PKG-INFO` & `srt_trans-1.0.0/srt_trans.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: srt_trans
-Version: 0.1.2
+Name: srt-trans
+Version: 1.0.0
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,14 +19,17 @@
 ## Translage any SubRip file from any source language to any target language, and merger them into the target SubRip(.srt) file.
 
 # How to usage:
 
 ```bash
 Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
 Example:
+    srt_trans ./test_video.mkv
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118
     srt_trans ./test/test_file.srt
     srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-TW
     srt_trans ./test/test_file.srt -src_lang en -dest_lang ja
     srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-CN
     srt_trans ./test/test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
 ```
```

### Comparing `srt_trans-0.1.2/README.md` & `srt_trans-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 ## Translage any SubRip file from any source language to any target language, and merger them into the target SubRip(.srt) file.
 
 # How to usage:
 
 ```bash
 Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
 Example:
+    srt_trans ./test_video.mkv
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118
     srt_trans ./test/test_file.srt
     srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-TW
     srt_trans ./test/test_file.srt -src_lang en -dest_lang ja
     srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-CN
     srt_trans ./test/test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
 ```
```

### Comparing `srt_trans-0.1.2/setup.py` & `srt_trans-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='0.1.2',
+    version='1.0.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
         # List your dependencies here
         'googletrans==3.1.0a0',
-        'pysrt>=1.1.2'
+        'pysrt>=1.1.2',
+        'ffmpeg_python==0.2.0'
     ],
     author='Jack',
     author_email='bumble.zhou@gmail.com',
     description='A simple translator for any SubRip(.srt) files.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/bumblezhou/srt_trans',
```

### Comparing `srt_trans-0.1.2/srt_trans/cli.py` & `srt_trans-1.0.0/srt_trans/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 from googletrans import Translator
 import pysrt
 import os
 import sys
 import shutil
+import ffmpeg
+
+def extract_subtitles(video_file, output_srt):
+    # Extract subtitles using FFmpeg
+    try:
+        (
+            ffmpeg
+            .input(video_file)
+            .output(output_srt, f='srt')
+            .run()
+        )
+        print(f'Subtitles extracted from {video_file} and saved to {output_srt}')
+    except ffmpeg.Error as e:
+        print(f'Error: {e}')
 
 
 def split_list(input_list, chunk_size):
     return [input_list[i:i+chunk_size] for i in range(0, len(input_list), chunk_size)]
 
 
 def flatten_list(list_of_lists):
@@ -40,21 +54,24 @@
 
     # Save translated SRT file
     srt_file.save(output_file, encoding='utf-8')
 
 
 def print_usage():
     print("""
-        Usage: srt_file_translator test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
+        Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
         Example:
-            srt_file_translator test_file.srt
-            srt_file_translator test_file.srt -src_lang en -dest_lang zh-TW
-            srt_file_translator test_file.srt -src_lang en -dest_lang ja
-            srt_file_translator test_file.srt -src_lang en -dest_lang zh-CN
-            srt_file_translator test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
+            srt_trans ./test_video.mkv
+            srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
+            srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118
+            srt_trans test_file.srt
+            srt_trans test_file.srt -src_lang en -dest_lang zh-TW
+            srt_trans test_file.srt -src_lang en -dest_lang ja
+            srt_trans test_file.srt -src_lang en -dest_lang zh-CN
+            srt_trans test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
     """)
 
 
 def pre_process_srt_file(input_file):
     # Load SRT file
     srt_file = pysrt.open(input_file, encoding='utf-8')
     for sub in srt_file:
@@ -67,14 +84,19 @@
         print_usage()
         return
     input_file = sys.argv[1]
     if not os.path.exists(input_file):
         print(f"{input_file} not exists!")
         return
     
+    if str(input_file).lower().endswith(".mkv"):
+        video_file = input_file.lower()
+        input_file = video_file.replace(".mkv", ".srt")
+        extract_subtitles(video_file, input_file)
+    
     pre_process_srt_file(input_file)
 
     source_language = "en"      # Source language code (e.g., "en" for English)
     target_language = "zh-CN"   # Target language code (e.g., "zh-CN" for Simple Chinese)
     if len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
         source_language = sys.argv[3]
         target_language = sys.argv[5]
```

### Comparing `srt_trans-0.1.2/srt_trans.egg-info/PKG-INFO` & `srt_trans-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: srt-trans
-Version: 0.1.2
+Name: srt_trans
+Version: 1.0.0
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,14 +19,17 @@
 ## Translage any SubRip file from any source language to any target language, and merger them into the target SubRip(.srt) file.
 
 # How to usage:
 
 ```bash
 Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
 Example:
+    srt_trans ./test_video.mkv
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
+    srt_trans ./test_video.mkv -src_lang en -dest_lang zh-CN -proxy http://127.0.0.1:8118
     srt_trans ./test/test_file.srt
     srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-TW
     srt_trans ./test/test_file.srt -src_lang en -dest_lang ja
     srt_trans ./test/test_file.srt -src_lang en -dest_lang zh-CN
     srt_trans ./test/test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
 ```
```

