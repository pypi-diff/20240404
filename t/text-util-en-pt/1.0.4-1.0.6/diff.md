# Comparing `tmp/text_util_en_pt-1.0.4.tar.gz` & `tmp/text_util_en_pt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_util_en_pt-1.0.4.tar", last modified: Fri Feb 23 05:17:43 2024, max compression
+gzip compressed data, was "text_util_en_pt-1.0.6.tar", last modified: Thu Apr  4 13:10:28 2024, max compression
```

## Comparing `text_util_en_pt-1.0.4.tar` & `text_util_en_pt-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-23 05:17:43.008925 text_util_en_pt-1.0.4/
--rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-08 21:33:02.000000 text_util_en_pt-1.0.4/LICENSE
--rw-r--r--   0 moro      (1000) moro      (1000)      596 2024-02-23 05:17:43.008925 text_util_en_pt-1.0.4/PKG-INFO
--rwxrwxrwx   0 moro      (1000) moro      (1000)      627 2024-02-23 05:17:13.000000 text_util_en_pt-1.0.4/pyproject.toml
--rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-02-23 05:17:43.008925 text_util_en_pt-1.0.4/setup.cfg
--rw-r--r--   0 moro      (1000) moro      (1000)      744 2024-02-23 05:17:13.000000 text_util_en_pt-1.0.4/setup.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-23 05:17:43.008925 text_util_en_pt-1.0.4/text_util_en_pt/
--rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-08 21:59:15.000000 text_util_en_pt-1.0.4/text_util_en_pt/__init__.py
--rw-r--r--   0 moro      (1000) moro      (1000)    22949 2024-02-23 05:16:48.000000 text_util_en_pt-1.0.4/text_util_en_pt/cleaner.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-23 05:17:43.008925 text_util_en_pt-1.0.4/text_util_en_pt/resources/
--rw-r--r--   0 moro      (1000) moro      (1000)   263066 2024-02-08 21:31:18.000000 text_util_en_pt-1.0.4/text_util_en_pt/resources/english_nltk_tokenizer.pkl
--rw-r--r--   0 moro      (1000) moro      (1000)   400695 2024-02-08 21:31:18.000000 text_util_en_pt-1.0.4/text_util_en_pt/resources/portuguese_nltk_tokenizer.pkl
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-02-23 05:17:43.008925 text_util_en_pt-1.0.4/text_util_en_pt.egg-info/
--rw-r--r--   0 moro      (1000) moro      (1000)      596 2024-02-23 05:17:42.000000 text_util_en_pt-1.0.4/text_util_en_pt.egg-info/PKG-INFO
--rw-r--r--   0 moro      (1000) moro      (1000)      389 2024-02-23 05:17:42.000000 text_util_en_pt-1.0.4/text_util_en_pt.egg-info/SOURCES.txt
--rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-02-23 05:17:42.000000 text_util_en_pt-1.0.4/text_util_en_pt.egg-info/dependency_links.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       16 2024-02-23 05:17:42.000000 text_util_en_pt-1.0.4/text_util_en_pt.egg-info/requires.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       16 2024-02-23 05:17:42.000000 text_util_en_pt-1.0.4/text_util_en_pt.egg-info/top_level.txt
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/
+-rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-08 21:33:02.000000 text_util_en_pt-1.0.6/LICENSE
+-rw-r--r--   0 moro      (1000) moro      (1000)      550 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/PKG-INFO
+-rwxrwxrwx   0 moro      (1000) moro      (1000)      640 2024-04-04 13:07:07.000000 text_util_en_pt-1.0.6/pyproject.toml
+-rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/setup.cfg
+-rw-r--r--   0 moro      (1000) moro      (1000)      757 2024-04-04 13:07:07.000000 text_util_en_pt-1.0.6/setup.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/text_util_en_pt/
+-rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-08 21:59:15.000000 text_util_en_pt-1.0.6/text_util_en_pt/__init__.py
+-rw-r--r--   0 moro      (1000) moro      (1000)    22957 2024-04-04 13:06:45.000000 text_util_en_pt-1.0.6/text_util_en_pt/cleaner.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/text_util_en_pt/resources/
+-rw-r--r--   0 moro      (1000) moro      (1000)   263066 2024-02-08 21:31:18.000000 text_util_en_pt-1.0.6/text_util_en_pt/resources/english_nltk_tokenizer.pkl
+-rw-r--r--   0 moro      (1000) moro      (1000)   400695 2024-02-08 21:31:18.000000 text_util_en_pt-1.0.6/text_util_en_pt/resources/portuguese_nltk_tokenizer.pkl
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/
+-rw-r--r--   0 moro      (1000) moro      (1000)      550 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/PKG-INFO
+-rw-r--r--   0 moro      (1000) moro      (1000)      389 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/SOURCES.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/dependency_links.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       26 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/requires.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       16 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/top_level.txt
```

### Comparing `text_util_en_pt-1.0.4/LICENSE` & `text_util_en_pt-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `text_util_en_pt-1.0.4/PKG-INFO` & `text_util_en_pt-1.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: text_util_en_pt
-Version: 1.0.4
+Version: 1.0.6
 Summary: Python project for text cleaning. Some specifics for English and Portuguese languages.
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro
 Project-URL: Bug Tracker, https://github.com/cnmoro
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: langdetect
-Requires-Dist: nltk
```

### Comparing `text_util_en_pt-1.0.4/pyproject.toml` & `text_util_en_pt-1.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "langdetect", "nltk"]
+requires = ["setuptools>=61.0", "langdetect", "nltk", "langchain"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text_util_en_pt"
-version = "1.0.4"
+version = "1.0.6"
 authors = [
   { name="Carlo Moro", email="cnmoro@gmail.com" },
 ]
 description = "Python project for text cleaning. Some specifics for English and Portuguese languages."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `text_util_en_pt-1.0.4/setup.py` & `text_util_en_pt-1.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='text_util_en_pt',
-    version='1.0.4',
+    version='1.0.6',
     author='Carlo Moro',
     author_email='cnmoro@gmail.com',
     description="Python project for text cleaning. Some specifics for English and Portuguese languages.",
     packages=find_packages(),
     package_data={
         'text_util_en_pt': [
             'resources/english_nltk_tokenizer.pkl',
             'resources/portuguese_nltk_tokenizer.pkl'
         ]
     },
     include_package_data=True,
-    install_requires=["langdetect", "nltk"],
+    install_requires=["langdetect", "nltk", "langchain"],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7',
 )
```

### Comparing `text_util_en_pt-1.0.4/text_util_en_pt/cleaner.py` & `text_util_en_pt-1.0.6/text_util_en_pt/cleaner.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,24 +100,24 @@
 
 def preprocessing(texto):
     replace_dict = {"\t": " ", "<": " ", ">": " ", "‹": " ", "›": " ", "~": " ", "¿": "", 
                     "[": "", "]": "", "%": "", "|": "", "º": "", "+": "", "/": " ", 
                     "\\n": " ", "\\": " ", "“": "\"", "”": "\"", "‘": " ", "’": " ", "�": " "}
     for old_char, new_char in replace_dict.items():
         texto = texto.replace(old_char, new_char)
-    texto = texto.lower()
+    # texto = texto.lower()
     while '  ' in texto:
         texto = texto.replace('  ', ' ')
     while '..' in texto:
         texto = texto.replace('..', '.')
     return texto
 
 def light_preprocessing(text):
     text = preprocessing(text)
-    text = text.lower()
+    # text = text.lower()
     text = text.replace('\xa0', ' ')
     text = re_tree_dots.sub('...', text)
     text = re.sub('\.\.\.', '', text)
     text = re_remove_brackets.sub('', text)
     text = re_changehyphen.sub('-', text)
     text = re_remove_html.sub(' ', text)
     text = re_quotes_1.sub(r'\1"', text)
@@ -196,15 +196,15 @@
         
         sentences[i] = text.strip()
         
     return sentences
 
 def preprocessing1(text):
     """Apply all regex above to a given string."""
-    text = text.lower()
+    # text = text.lower()
     text = text.replace('\xa0', ' ')
     text = re_tree_dots.sub('...', text)
     text = re.sub('\.\.\.', '', text)
     text = re_remove_brackets.sub('', text)
     text = re_changehyphen.sub('-', text)
     text = re_remove_html.sub(' ', text)
     text = re_transform_numbers.sub('0', text)
@@ -230,15 +230,15 @@
     replace_dict = {",": " ", "\t": " ", "©": " ", ";": " ", ":": " ", "_": " ", "<": " ",
                         ">": " ", "‹": " ", "›": " ", "~": " ", "¿": "", "?": "", "(": "",
                         ")": "", "[": "", "]": "", "%": "", "#": "", "|": "", "º": "", 
                         "+": "", "/": " ", "\\n": " ", "\\": " ", "\"": " ", "“": " ", 
                         "”": " ", "‘": " ", "’": " ", "�": " "}
     for old_char, new_char in replace_dict.items():
         texto = texto.replace(old_char, new_char)
-    texto = texto.lower()
+    # texto = texto.lower()
 
     while '  ' in texto:
         texto = texto.replace('  ', ' ')
     
     while '..' in texto:
         texto = texto.replace('..', '.')
```

### Comparing `text_util_en_pt-1.0.4/text_util_en_pt/resources/english_nltk_tokenizer.pkl` & `text_util_en_pt-1.0.6/text_util_en_pt/resources/english_nltk_tokenizer.pkl`

 * *Files identical despite different names*

### Comparing `text_util_en_pt-1.0.4/text_util_en_pt/resources/portuguese_nltk_tokenizer.pkl` & `text_util_en_pt-1.0.6/text_util_en_pt/resources/portuguese_nltk_tokenizer.pkl`

 * *Files identical despite different names*

### Comparing `text_util_en_pt-1.0.4/text_util_en_pt.egg-info/PKG-INFO` & `text_util_en_pt-1.0.6/text_util_en_pt.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: text-util-en-pt
-Version: 1.0.4
+Version: 1.0.6
 Summary: Python project for text cleaning. Some specifics for English and Portuguese languages.
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro
 Project-URL: Bug Tracker, https://github.com/cnmoro
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: langdetect
-Requires-Dist: nltk
```

