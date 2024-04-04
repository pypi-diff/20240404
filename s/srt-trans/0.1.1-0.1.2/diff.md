# Comparing `tmp/srt_trans-0.1.1.tar.gz` & `tmp/srt_trans-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-0.1.1.tar", last modified: Thu Apr  4 00:39:30 2024, max compression
+gzip compressed data, was "srt_trans-0.1.2.tar", last modified: Thu Apr  4 01:05:08 2024, max compression
```

## Comparing `srt_trans-0.1.1.tar` & `srt_trans-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 00:39:30.894624 srt_trans-0.1.1/
--rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1490 2024-04-04 00:39:30.894624 srt_trans-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      881 2024-04-04 00:36:54.000000 srt_trans-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 00:39:30.894624 srt_trans-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-04 00:39:01.000000 srt_trans-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 00:39:30.845696 srt_trans-0.1.1/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-0.1.1/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     3391 2024-04-04 00:36:54.000000 srt_trans-0.1.1/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 00:39:30.894624 srt_trans-0.1.1/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1490 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 00:39:30.000000 srt_trans-0.1.1/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 01:05:08.676356 srt_trans-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1490 2024-04-04 01:05:08.674347 srt_trans-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2024-04-04 00:36:54.000000 srt_trans-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 01:05:08.676356 srt_trans-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-04 01:04:26.000000 srt_trans-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:05:08.625591 srt_trans-0.1.2/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-0.1.2/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-04-04 01:02:18.000000 srt_trans-0.1.2/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:05:08.670804 srt_trans-0.1.2/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1490 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 01:05:08.000000 srt_trans-0.1.2/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-0.1.1/LICENSE` & `srt_trans-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-0.1.1/PKG-INFO` & `srt_trans-0.1.2/srt_trans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: srt_trans
-Version: 0.1.1
+Name: srt-trans
+Version: 0.1.2
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `srt_trans-0.1.1/README.md` & `srt_trans-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `srt_trans-0.1.1/setup.py` & `srt_trans-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
```

### Comparing `srt_trans-0.1.1/srt_trans/cli.py` & `srt_trans-0.1.2/srt_trans/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 
 def flatten_list(list_of_lists):
     return [item for sublist in list_of_lists for item in sublist]
 
 
 def translate_srt(input_file, output_file, source_language, target_language):
     # Load SRT file
-    subs = pysrt.open(input_file, encoding='utf-8')
-    lines = [sub.text for sub in subs]
+    srt_file = pysrt.open(input_file, encoding='utf-8')
+    
+    lines = [sub.text for sub in srt_file]
     # split all lines into small list of lines(no more than 200 lines in each sub list)
     sub_lines_list = split_list(lines, 200)
 
     # Initialize translator
     translator = Translator()
 
     translated_lines_list = []
@@ -29,42 +30,53 @@
         source_text = "@".join(sub_lines)
         translation = translator.translate(source_text, src=source_language, dest=target_language)
         translated_lines = translation.text.split("@")
         translated_lines_list.append(translated_lines)
 
     translated_lines = flatten_list(translated_lines_list)
     # Translate each subtitle
-    for sub, translated_line in zip(subs, translated_lines):
+    for sub, translated_line in zip(srt_file, translated_lines):
         # Merge the source subtitle and the translated subtitle.
         sub.text = "<font color='#ffff54'>" + sub.text + "</font>" + "\n" + translated_line
 
     # Save translated SRT file
-    subs.save(output_file, encoding='utf-8')
+    srt_file.save(output_file, encoding='utf-8')
 
 
 def print_usage():
     print("""
         Usage: srt_file_translator test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
         Example:
             srt_file_translator test_file.srt
             srt_file_translator test_file.srt -src_lang en -dest_lang zh-TW
             srt_file_translator test_file.srt -src_lang en -dest_lang ja
             srt_file_translator test_file.srt -src_lang en -dest_lang zh-CN
             srt_file_translator test_file.srt -src_lang en -dest_lang fr -proxy http://127.0.0.1:8118
     """)
 
 
+def pre_process_srt_file(input_file):
+    # Load SRT file
+    srt_file = pysrt.open(input_file, encoding='utf-8')
+    for sub in srt_file:
+        sub.text = str(sub.text).replace("\n", " ")
+    srt_file.save(input_file, encoding='utf-8')
+
+
 def main():
     if len(sys.argv) < 2:
         print_usage()
         return
     input_file = sys.argv[1]
     if not os.path.exists(input_file):
         print(f"{input_file} not exists!")
         return
+    
+    pre_process_srt_file(input_file)
+
     source_language = "en"      # Source language code (e.g., "en" for English)
     target_language = "zh-CN"   # Target language code (e.g., "zh-CN" for Simple Chinese)
     if len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
         source_language = sys.argv[3]
         target_language = sys.argv[5]
     if len(sys.argv) == 8 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang" and sys.argv[6] == "-proxy":
         source_language = sys.argv[3]
```

### Comparing `srt_trans-0.1.1/srt_trans.egg-info/PKG-INFO` & `srt_trans-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: srt-trans
-Version: 0.1.1
+Name: srt_trans
+Version: 0.1.2
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

