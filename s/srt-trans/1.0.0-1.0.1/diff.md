# Comparing `tmp/srt_trans-1.0.0.tar.gz` & `tmp/srt_trans-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-1.0.0.tar", last modified: Thu Apr  4 02:10:23 2024, max compression
+gzip compressed data, was "srt_trans-1.0.1.tar", last modified: Thu Apr  4 03:18:03 2024, max compression
```

## Comparing `srt_trans-1.0.0.tar` & `srt_trans-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 02:10:23.809766 srt_trans-1.0.0/
--rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1675 2024-04-04 02:10:23.807764 srt_trans-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1066 2024-04-04 02:09:13.000000 srt_trans-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 02:10:23.809766 srt_trans-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1045 2024-04-04 02:07:55.000000 srt_trans-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 02:10:23.766196 srt_trans-1.0.0/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.0/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     4455 2024-04-04 02:10:00.000000 srt_trans-1.0.0/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 02:10:23.804750 srt_trans-1.0.0/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1675 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 02:10:23.000000 srt_trans-1.0.0/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 03:18:03.027008 srt_trans-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1675 2024-04-04 03:18:03.027008 srt_trans-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2024-04-04 02:09:13.000000 srt_trans-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 03:18:03.027008 srt_trans-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2024-04-04 03:17:13.000000 srt_trans-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:18:02.988954 srt_trans-1.0.1/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.1/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     5034 2024-04-04 03:15:27.000000 srt_trans-1.0.1/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:18:03.027008 srt_trans-1.0.1/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1675 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 03:18:02.000000 srt_trans-1.0.1/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-1.0.0/LICENSE` & `srt_trans-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.0/PKG-INFO` & `srt_trans-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt_trans
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `srt_trans-1.0.0/README.md` & `srt_trans-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.0/setup.py` & `srt_trans-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
```

### Comparing `srt_trans-1.0.0/srt_trans/cli.py` & `srt_trans-1.0.1/srt_trans/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,42 +23,59 @@
     return [input_list[i:i+chunk_size] for i in range(0, len(input_list), chunk_size)]
 
 
 def flatten_list(list_of_lists):
     return [item for sublist in list_of_lists for item in sublist]
 
 
+def translate_lines(translator, lines, source_language, target_language):
+    source_text = "\n❂".join(lines)
+    translation = translator.translate(source_text, src=source_language, dest=target_language)
+    translated_lines = translation.text.split("\n❂")
+    return translated_lines
+
+
 def translate_srt(input_file, output_file, source_language, target_language):
+    result = True
+
     # Load SRT file
     srt_file = pysrt.open(input_file, encoding='utf-8')
     
     lines = [sub.text for sub in srt_file]
     # split all lines into small list of lines(no more than 200 lines in each sub list)
     sub_lines_list = split_list(lines, 200)
 
     # Initialize translator
     translator = Translator()
 
     translated_lines_list = []
     # Loop each each small list of lines, translate them.
     for sub_lines in sub_lines_list:
-        source_text = "@".join(sub_lines)
-        translation = translator.translate(source_text, src=source_language, dest=target_language)
-        translated_lines = translation.text.split("@")
-        translated_lines_list.append(translated_lines)
+        translated_lines = translate_lines(translator, sub_lines, source_language, target_language)
+        if len(translated_lines) == len(sub_lines):
+            translated_lines_list.append(translated_lines)
+        else:
+            print("Can not translate the subtitle correctly.")
+            result = False
+            break
+    
+    if not result:
+        return result
 
     translated_lines = flatten_list(translated_lines_list)
     # Translate each subtitle
     for sub, translated_line in zip(srt_file, translated_lines):
         # Merge the source subtitle and the translated subtitle.
         sub.text = "<font color='#ffff54'>" + sub.text + "</font>" + "\n" + translated_line
 
     # Save translated SRT file
     srt_file.save(output_file, encoding='utf-8')
 
+    return result
+
 
 def print_usage():
     print("""
         Usage: srt_trans test_file.srt [-src_lang en -dest_lang zh-CN -proxy http://youdomain:your_port]
         Example:
             srt_trans ./test_video.mkv
             srt_trans ./test_video.mkv -src_lang en -dest_lang zh-TW
@@ -71,15 +88,15 @@
     """)
 
 
 def pre_process_srt_file(input_file):
     # Load SRT file
     srt_file = pysrt.open(input_file, encoding='utf-8')
     for sub in srt_file:
-        sub.text = str(sub.text).replace("\n", " ")
+        sub.text = str(sub.text).replace("\n", " ").replace("<i>", "").replace("</i>", "")
     srt_file.save(input_file, encoding='utf-8')
 
 
 def main():
     if len(sys.argv) < 2:
         print_usage()
         return
@@ -107,15 +124,17 @@
         # Set environment variables (replace with your details)
         # os.environ['http_proxy'] = "http://127.0.0.1:8118"
         # os.environ['https_proxy'] = "http://127.0.0.1:8118"
         os.environ['http_proxy'] = proxy
         os.environ['https_proxy'] = proxy
 
     output_file = str(input_file).replace(".srt", f".{target_language}.srt")
-    translate_srt(input_file, output_file, source_language, target_language)
+    translate_result = translate_srt(input_file, output_file, source_language, target_language)
+    if not translate_result:
+        return
     
     os.remove(input_file)
     shutil.move(output_file, input_file)
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `srt_trans-1.0.0/srt_trans.egg-info/PKG-INFO` & `srt_trans-1.0.1/srt_trans.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-trans
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

