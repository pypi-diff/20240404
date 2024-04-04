# Comparing `tmp/srt_trans-1.0.1.tar.gz` & `tmp/srt_trans-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-1.0.1.tar", last modified: Thu Apr  4 03:18:03 2024, max compression
+gzip compressed data, was "srt_trans-1.0.2.tar", last modified: Thu Apr  4 03:54:52 2024, max compression
```

## Comparing `srt_trans-1.0.1.tar` & `srt_trans-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 03:18:03.027008 srt_trans-1.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1675 2024-04-04 03:18:03.027008 srt_trans-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1066 2024-04-04 02:09:13.000000 srt_trans-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 03:18:03.027008 srt_trans-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1045 2024-04-04 03:17:13.000000 srt_trans-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:18:02.988954 srt_trans-1.0.1/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.1/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     5034 2024-04-04 03:15:27.000000 srt_trans-1.0.1/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:18:03.027008 srt_trans-1.0.1/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1675 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 03:54:52.148831 srt_trans-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1675 2024-04-04 03:54:52.148831 srt_trans-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2024-04-04 02:09:13.000000 srt_trans-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 03:54:52.148831 srt_trans-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2024-04-04 03:54:34.000000 srt_trans-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:54:52.108773 srt_trans-1.0.2/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.2/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     5045 2024-04-04 03:53:26.000000 srt_trans-1.0.2/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:54:52.147559 srt_trans-1.0.2/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1675 2024-04-04 03:54:51.000000 srt_trans-1.0.2/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 03:54:51.000000 srt_trans-1.0.2/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 03:54:51.000000 srt_trans-1.0.2/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 03:54:51.000000 srt_trans-1.0.2/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 03:54:51.000000 srt_trans-1.0.2/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 03:54:51.000000 srt_trans-1.0.2/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-1.0.1/LICENSE` & `srt_trans-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.1/PKG-INFO` & `srt_trans-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt_trans
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `srt_trans-1.0.1/README.md` & `srt_trans-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.1/setup.py` & `srt_trans-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
```

### Comparing `srt_trans-1.0.1/srt_trans/cli.py` & `srt_trans-1.0.2/srt_trans/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 
 def flatten_list(list_of_lists):
     return [item for sublist in list_of_lists for item in sublist]
 
 
 def translate_lines(translator, lines, source_language, target_language):
-    source_text = "\n❂".join(lines)
+    source_text = "\n@".join(lines)
     translation = translator.translate(source_text, src=source_language, dest=target_language)
-    translated_lines = translation.text.split("\n❂")
+    translated_lines = translation.text.split("\n@")
     return translated_lines
 
 
 def translate_srt(input_file, output_file, source_language, target_language):
     result = True
 
     # Load SRT file
@@ -88,29 +88,29 @@
     """)
 
 
 def pre_process_srt_file(input_file):
     # Load SRT file
     srt_file = pysrt.open(input_file, encoding='utf-8')
     for sub in srt_file:
-        sub.text = str(sub.text).replace("\n", " ").replace("<i>", "").replace("</i>", "")
+        sub.text = str(sub.text).replace("\n", " ").replace("<i>", "").replace("</i>", "").replace("{\\an8}", "")
     srt_file.save(input_file, encoding='utf-8')
 
 
 def main():
     if len(sys.argv) < 2:
         print_usage()
         return
     input_file = sys.argv[1]
     if not os.path.exists(input_file):
         print(f"{input_file} not exists!")
         return
     
     if str(input_file).lower().endswith(".mkv"):
-        video_file = input_file.lower()
+        video_file = input_file
         input_file = video_file.replace(".mkv", ".srt")
         extract_subtitles(video_file, input_file)
     
     pre_process_srt_file(input_file)
 
     source_language = "en"      # Source language code (e.g., "en" for English)
     target_language = "zh-CN"   # Target language code (e.g., "zh-CN" for Simple Chinese)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `srt_trans-1.0.1/srt_trans.egg-info/PKG-INFO` & `srt_trans-1.0.2/srt_trans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-trans
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

