# Comparing `tmp/srt_trans-1.0.4.tar.gz` & `tmp/srt_trans-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-1.0.4.tar", last modified: Thu Apr  4 16:45:46 2024, max compression
+gzip compressed data, was "srt_trans-1.0.5.tar", last modified: Thu Apr  4 17:39:46 2024, max compression
```

## Comparing `srt_trans-1.0.4.tar` & `srt_trans-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 16:45:46.641937 srt_trans-1.0.4/
--rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1675 2024-04-04 16:45:46.639892 srt_trans-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1066 2024-04-04 02:09:13.000000 srt_trans-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 16:45:46.643367 srt_trans-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1045 2024-04-04 16:45:37.000000 srt_trans-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:45:46.597765 srt_trans-1.0.4/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.4/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     5282 2024-04-04 16:43:16.000000 srt_trans-1.0.4/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:45:46.635874 srt_trans-1.0.4/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1675 2024-04-04 16:45:46.000000 srt_trans-1.0.4/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 16:45:46.000000 srt_trans-1.0.4/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 16:45:46.000000 srt_trans-1.0.4/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 16:45:46.000000 srt_trans-1.0.4/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-04-04 16:45:46.000000 srt_trans-1.0.4/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 16:45:46.000000 srt_trans-1.0.4/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 17:39:46.529905 srt_trans-1.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1675 2024-04-04 17:39:46.526140 srt_trans-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2024-04-04 02:09:13.000000 srt_trans-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 17:39:46.529905 srt_trans-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2024-04-04 17:39:33.000000 srt_trans-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 17:39:46.477596 srt_trans-1.0.5/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.5/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     5807 2024-04-04 17:39:04.000000 srt_trans-1.0.5/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 17:39:46.521140 srt_trans-1.0.5/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1675 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 17:39:46.000000 srt_trans-1.0.5/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-1.0.4/LICENSE` & `srt_trans-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.4/PKG-INFO` & `srt_trans-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt_trans
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `srt_trans-1.0.4/README.md` & `srt_trans-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.4/setup.py` & `srt_trans-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
```

### Comparing `srt_trans-1.0.4/srt_trans/cli.py` & `srt_trans-1.0.5/srt_trans/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     return [input_list[i:i+chunk_size] for i in range(0, len(input_list), chunk_size)]
 
 
 def flatten_list(list_of_lists):
     return [item for sublist in list_of_lists for item in sublist]
 
 
+def multi_find(source_text, search_key):
+    return [pos for pos in range(len(source_text)) if source_text.startswith(search_key, pos)]
+
+
 def translate_lines(translator, lines, source_language, target_language):
     lines = [line + '\n' for line in lines]
     source_text = "@@@".join(lines)
     translation = translator.translate(source_text, src=source_language, dest=target_language)
     translated_lines = translation.text.split("@@@")
     translated_lines = [line.replace("@ @@", "@@@").replace("@@ @", "@@@").split("@@@") for line in translated_lines]
     translated_lines = flatten_list(translated_lines)
@@ -53,17 +57,22 @@
     translated_lines_list = []
     # Loop each each small list of lines, translate them.
     for sub_lines in sub_lines_list:
         translated_lines = translate_lines(translator, sub_lines, source_language, target_language)
         if len(translated_lines) == len(sub_lines):
             translated_lines_list.append(translated_lines)
         else:
-            print("Can not translate the subtitle correctly.")
-            result = False
-            break
+            translated_lines = [[sub_line + "\n" for sub_line in (line[:-1].split("\n"))] if len(multi_find(line, "\n")) > 1 else [line] for line in translated_lines]
+            translated_lines = flatten_list(translated_lines)
+            if len(translated_lines) == len(sub_lines):
+                translated_lines_list.append(translated_lines)
+            else:
+                print("Can not translate the subtitle correctly.")
+                result = False
+                break
     
     if not result:
         return result
 
     translated_lines = flatten_list(translated_lines_list)
     # Translate each subtitle
     for sub, translated_line in zip(srt_file, translated_lines):
```

### Comparing `srt_trans-1.0.4/srt_trans.egg-info/PKG-INFO` & `srt_trans-1.0.5/srt_trans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-trans
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

