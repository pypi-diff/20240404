# Comparing `tmp/piraye-0.4.0.tar.gz` & `tmp/piraye-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piraye-0.4.0.tar", last modified: Wed Feb 14 17:15:06 2024, max compression
+gzip compressed data, was "piraye-0.5.0.tar", last modified: Wed Apr  3 22:35:50 2024, max compression
```

## Comparing `piraye-0.4.0.tar` & `piraye-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.408069 piraye-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-02-14 17:14:58.000000 piraye-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-02-14 17:15:06.408069 piraye-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-02-14 17:14:58.000000 piraye-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.400069 piraye-0.4.0/piraye/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.404069 piraye-0.4.0/piraye/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.404069 piraye-0.4.0/piraye/tasks/normalizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/char_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/character_normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.400069 piraye-0.4.0/piraye/tasks/normalizer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.404069 piraye-0.4.0/piraye/tasks/normalizer/data/alphabets/
--rw-r--r--   0 runner    (1001) docker     (127)    38830 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/data/alphabets/ar.json
--rw-r--r--   0 runner    (1001) docker     (127)   197395 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/data/alphabets/en.json
--rw-r--r--   0 runner    (1001) docker     (127)    41339 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/data/alphabets/fa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.404069 piraye-0.4.0/piraye/tasks/normalizer/data/digits/
--rw-r--r--   0 runner    (1001) docker     (127)    51719 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/data/digits/digits.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.404069 piraye-0.4.0/piraye/tasks/normalizer/data/others/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/data/others/deletions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/data/others/diacritics.json
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/data/others/spaces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.404069 piraye-0.4.0/piraye/tasks/normalizer/data/puncs/
--rw-r--r--   0 runner    (1001) docker     (127)    26238 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/data/puncs/puncs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/multi_lingual_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/normalizer/normalizer_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.404069 piraye-0.4.0/piraye/tasks/punc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/punc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/punc/punctuation_restoration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.408069 piraye-0.4.0/piraye/tasks/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/tokenizer/nltk_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tasks/tokenizer/punc_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-02-14 17:14:58.000000 piraye-0.4.0/piraye/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.408069 piraye-0.4.0/piraye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-02-14 17:15:06.000000 piraye-0.4.0/piraye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-14 17:15:06.000000 piraye-0.4.0/piraye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 17:15:06.000000 piraye-0.4.0/piraye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-14 17:15:06.000000 piraye-0.4.0/piraye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-14 17:15:06.000000 piraye-0.4.0/piraye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-14 17:14:58.000000 piraye-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 17:15:06.408069 piraye-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 17:15:06.408069 piraye-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-14 17:14:58.000000 piraye-0.4.0/tests/test_ml_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-02-14 17:14:58.000000 piraye-0.4.0/tests/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-14 17:14:58.000000 piraye-0.4.0/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-03 22:35:46.000000 piraye-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 22:35:50.120671 piraye-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-03 22:35:46.000000 piraye-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/tasks/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/char_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/character_normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.112671 piraye-0.5.0/piraye/tasks/normalizer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/
+-rw-r--r--   0 runner    (1001) docker     (127)    38830 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/ar.json
+-rw-r--r--   0 runner    (1001) docker     (127)   197395 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41339 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/fa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.116671 piraye-0.5.0/piraye/tasks/normalizer/data/digits/
+-rw-r--r--   0 runner    (1001) docker     (127)    51719 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/digits/digits.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye/tasks/normalizer/data/others/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/others/deletions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/others/diacritics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/others/spaces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye/tasks/normalizer/data/puncs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26238 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/data/puncs/puncs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/multi_lingual_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/normalizer/normalizer_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye/tasks/punc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/punc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/punc/punctuation_restoration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye/tasks/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/tokenizer/nltk_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/tokenizer/punc_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tasks/tokenizer/spacy_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-03 22:35:46.000000 piraye-0.5.0/piraye/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/piraye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 22:35:50.000000 piraye-0.5.0/piraye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-03 22:35:46.000000 piraye-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:35:50.120671 piraye-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:35:50.120671 piraye-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 22:35:46.000000 piraye-0.5.0/tests/test_ml_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-03 22:35:46.000000 piraye-0.5.0/tests/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-03 22:35:46.000000 piraye-0.5.0/tests/test_tokenizer.py
```

### Comparing `piraye-0.4.0/LICENSE` & `piraye-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/PKG-INFO` & `piraye-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piraye
-Version: 0.4.0
+Version: 0.5.0
 Summary: A utility for normalizing persian, arabic and english texts
 Author-email: Hamed Khademi Khaledi <khaledihkh@gmail.com>, HosseiN Khademi khaeldi <hossein@arusha.dev>, Majid Asgiar Bidhendi <majid@arusha.dev>
 Maintainer-email: Arusha Developers <info@arusha.dev>
 License: LGPLv2
 Project-URL: Homepage, https://github.com/arushadev/piraye
 Project-URL: Bug Tracker, https://github.com/arushadev/piraye/issues
 Keywords: NLP,Natural Language Processing,Tokenizing,Normalization
@@ -30,48 +30,49 @@
 Requires-Dist: lingua-language-detector
 Provides-Extra: dev
 Requires-Dist: tqdm; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint==2.17.7; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: spacy; extra == "dev"
 
-# Piraye: NLP Utils
+# Piraye: NLP Utilities
 
 <p align="center">
   <a href="https://pypi.org/project/piraye"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/piraye.svg?maxAge=86400" /></a>
   <a href="https://pypi.org/project/piraye"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/piraye.svg?maxAge=86400" /></a>
   <a href="https://pypi.org/project/piraye"><img alt="License" src="https://img.shields.io/pypi/l/piraye.svg?maxAge=86400" /></a>
+  <a href="https://pepy.tech/project/piraye"><img alt="Downloads" src="https://static.pepy.tech/badge/piraye" /></a>
   <a href="https://github.com/arushadev/piraye/actions/workflows/pylint.yml"><img alt="Pylint" src="https://github.com/arushadev/piraye/actions/workflows/pylint.yml/badge.svg" /></a>
   <a href="https://github.com/arushadev/piraye/actions/workflows/unit-test.yml/badge.svg)](https://github.com/arushadev/piraye/actions/workflows/unit-test.yml"><img alt="Unit Test" src="https://github.com/arushadev/piraye/actions/workflows/unit-test.yml/badge.svg" /></a>
 </p>
 
 
-A utility for normalizing persian, arabic and english texts
+**Piraye** is a Python library designed to facilitate text normalization for Persian, Arabic, and English languages.
 
 ## Requirements
 
 * Python 3.11+
 * nltk 3.4.5+
 
 ## Installation
 
-Install the latest version with pip
+You can install the latest version of Piraye via pip:
+
 `pip install piraye`
 
 ## Usage
 
-Create an instance of Normalizer with NormalizerBuilder and then call normalize function. Also see list of all available
-configs in [configs](#Configs) section.
+To use Piraye, create an instance of the Normalizer class with NormalizerBuilder and then call the normalize function. You can configure the normalization process using various settings available. Below are two examples demonstrating different approaches:
 
 * Using builder pattern:
 
 ```python
 from piraye import NormalizerBuilder
-from piraye.tasks.normalizer.normalizer_builder import Config
 
 text = "این یک متن تسة اسﺘ       , 24/12/1400 "
 normalizer = NormalizerBuilder().alphabet_fa().digit_fa().punctuation_fa().tokenizing().remove_extra_spaces().build()
 normalizer.normalize(text)  # "این یک متن تست است ، ۲۴/۱۲/۱۴۰۰"
 ```
 
 * Using constructor:
@@ -82,49 +83,52 @@
 
 text = "این یک متن تسة اسﺘ       , 24/12/1400 "
 normalizer = NormalizerBuilder([Config.PUNCTUATION_FA, Config.ALPHABET_FA, Config.DIGIT_FA], remove_extra_spaces=True,
                                tokenization=True).build()
 normalizer.normalize(text)  # "این یک متن تست است ، ۲۴/۱۲/۱۴۰۰"
 ```
 
-Also see [other examples](https://github.com/arushadev/piraye/blob/readme/examples.md)
+You can find more examples [here](https://github.com/arushadev/piraye/blob/readme/examples.md)
 
 ## Configs
 
+Piraye provides various configurations for text normalization. Here's a list of available configurations:
+
 |      Config      |     Function     |                      Description                      |
 |:----------------:|:----------------:|:-----------------------------------------------------:|
-|   ALPHABET_AR    |   alphabet_ar    |         mapping alphabet characters to arabic         |
-|   ALPHABET_EN    |   alphabet_en    |        mapping alphabet characters to english         |
-|   ALPHABET_FA    |   alphabet_fa    |        mapping alphabet characters to persian         |
-|     DIGIT_AR     |     digit_ar     |            convert digits to arabic digits            |
-|     DIGIT_EN     |     digit_en     |           convert digits to english digits            |
-|     DIGIT_FA     |     digit_fa     |           convert digits to persian digits            |
+|   ALPHABET_AR    |   alphabet_ar    |         mapping alphabet characters to Arabic         |
+|   ALPHABET_EN    |   alphabet_en    |        mapping alphabet characters to English         |
+|   ALPHABET_FA    |   alphabet_fa    |        mapping alphabet characters to Persian         |
+|     DIGIT_AR     |     digit_ar     |            convert digits to Arabic digits            |
+|     DIGIT_EN     |     digit_en     |           convert digits to English digits            |
+|     DIGIT_FA     |     digit_fa     |           convert digits to Persian digits            |
 | DIACRITIC_DELETE | diacritic_delete |                 remove all diacritics                 |
 |   SPACE_DELETE   |   space_delete   |                   remove all spaces                   |
 |   SPACE_NORMAL   |   space_normal   | normal spaces ( like NO-BREAK SPACE , Tab and etc...) |
 |    SPACE_KEEP    |    space_keep    |          mapping spaces and not normal them           |
-|  PUNCTUATION_AR  |  punctuation_ar  |      mapping punctuations to arabic punctuations      |
-|  PUNCTUATION_Fa  |  punctuation_fa  |     mapping punctuations to persian punctuations      |
-|  PUNCTUATION_EN  |  punctuation_en  |     mapping punctuations to english punctuations      |
+|  PUNCTUATION_AR  |  punctuation_ar  |      mapping punctuations to Arabic punctuations      |
+|  PUNCTUATION_Fa  |  punctuation_fa  |     mapping punctuations to Persian punctuations      |
+|  PUNCTUATION_EN  |  punctuation_en  |     mapping punctuations to English punctuations      |
 
 Other attributes:
 
-* remove_extra_spaces : append multiple spaces together
-* tokenization : replace punctuation characters that just are tokens
+* remove_extra_spaces: Appends multiple spaces together.
+* tokenization: Replaces punctuation characters which are just tokens.
 
 ## Development
 
-* Install dependencies with `pip install -e .[dev]`
+To set up a development environment, install dependencies with:
+
+`pip install -e .[dev]`
 
 ## License
 
 **GNU Lesser General Public License v2.1**
 
-Primarily used for software libraries, the GNU LGPL requires that derived works be licensed under the same license, but
-works that only link to it do not fall under this restriction. There are two commonly used versions of the GNU LGPL.
-
-See [LICENSE](https://github.com/arushadev/piraye/blob/main/LICENSE)
+Piraye is licensed under the GNU Lesser General Public License v2.1, which primarily applies to software libraries.
+See the [LICENSE](https://github.com/arushadev/piraye/blob/main/LICENSE) file for more details.
 
 ## About ️
 
-[Arusha](https://www.arusha.dev)
+Piraye is maintained by [Arusha](https://www.arusha.dev).
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: piraye Version: 0.4.0 Summary: A utility for
+Metadata-Version: 2.1 Name: piraye Version: 0.5.0 Summary: A utility for
 normalizing persian, arabic and english texts Author-email: Hamed Khademi
 Khaledi
 gmail.com>, HosseiN Khademi khaeldi
 arusha.dev>, Majid Asgiar Bidhendi
 arusha.dev> Maintainer-email: Arusha Developers
 arusha.dev> License: LGPLv2 Project-URL: Homepage, https://github.com/
 arushadev/piraye Project-URL: Bug Tracker, https://github.com/arushadev/piraye/
@@ -17,50 +17,52 @@
 Intelligence Classifier: Topic :: Text Processing Classifier: Topic :: Text
 Processing :: Filters Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic ::
 Utilities Requires-Python: >=3.11 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: nltk Requires-Dist: lingua-language-
 detector Provides-Extra: dev Requires-Dist: tqdm; extra == "dev" Requires-Dist:
 pytest; extra == "dev" Requires-Dist: pylint==2.17.7; extra == "dev" Requires-
-Dist: flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" # Piraye:
-NLP Utils
-          _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_P_y_l_i_n_t_]_[_U_n_i_t_ _T_e_s_t_]
-A utility for normalizing persian, arabic and english texts ## Requirements *
-Python 3.11+ * nltk 3.4.5+ ## Installation Install the latest version with pip
-`pip install piraye` ## Usage Create an instance of Normalizer with
-NormalizerBuilder and then call normalize function. Also see list of all
-available configs in [configs](#Configs) section. * Using builder pattern:
-```python from piraye import NormalizerBuilder from
-piraye.tasks.normalizer.normalizer_builder import Config text = "Ø§ÛÙ ÛÚ©
+Dist: flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
+Dist: spacy; extra == "dev" # Piraye: NLP Utilities
+    _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_P_y_l_i_n_t_]_[_U_n_i_t_ _T_e_s_t_]
+**Piraye** is a Python library designed to facilitate text normalization for
+Persian, Arabic, and English languages. ## Requirements * Python 3.11+ * nltk
+3.4.5+ ## Installation You can install the latest version of Piraye via pip:
+`pip install piraye` ## Usage To use Piraye, create an instance of the
+Normalizer class with NormalizerBuilder and then call the normalize function.
+You can configure the normalization process using various settings available.
+Below are two examples demonstrating different approaches: * Using builder
+pattern: ```python from piraye import NormalizerBuilder text = "Ø§ÛÙ ÛÚ©
 ÙØªÙ ØªØ³Ø© Ø§Ø³ïº , 24/12/1400 " normalizer = NormalizerBuilder
 ().alphabet_fa().digit_fa().punctuation_fa().tokenizing().remove_extra_spaces
 ().build() normalizer.normalize(text) # "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø
 Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` * Using constructor: ```python from piraye import
 NormalizerBuilder from piraye.tasks.normalizer.normalizer_builder import Config
 text = "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Ø© Ø§Ø³ïº , 24/12/1400 " normalizer =
 NormalizerBuilder([Config.PUNCTUATION_FA, Config.ALPHABET_FA, Config.DIGIT_FA],
 remove_extra_spaces=True, tokenization=True).build() normalizer.normalize(text)
-# "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` Also see [other
-examples](https://github.com/arushadev/piraye/blob/readme/examples.md) ##
-Configs | Config | Function | Description | |:----------------:|:--------------
---:|:-----------------------------------------------------:| | ALPHABET_AR |
-alphabet_ar | mapping alphabet characters to arabic | | ALPHABET_EN |
-alphabet_en | mapping alphabet characters to english | | ALPHABET_FA |
-alphabet_fa | mapping alphabet characters to persian | | DIGIT_AR | digit_ar |
-convert digits to arabic digits | | DIGIT_EN | digit_en | convert digits to
-english digits | | DIGIT_FA | digit_fa | convert digits to persian digits | |
-DIACRITIC_DELETE | diacritic_delete | remove all diacritics | | SPACE_DELETE |
-space_delete | remove all spaces | | SPACE_NORMAL | space_normal | normal
-spaces ( like NO-BREAK SPACE , Tab and etc...) | | SPACE_KEEP | space_keep |
-mapping spaces and not normal them | | PUNCTUATION_AR | punctuation_ar |
-mapping punctuations to arabic punctuations | | PUNCTUATION_Fa | punctuation_fa
-| mapping punctuations to persian punctuations | | PUNCTUATION_EN |
-punctuation_en | mapping punctuations to english punctuations | Other
-attributes: * remove_extra_spaces : append multiple spaces together *
-tokenization : replace punctuation characters that just are tokens ##
-Development * Install dependencies with `pip install -e .[dev]` ## License
-**GNU Lesser General Public License v2.1** Primarily used for software
-libraries, the GNU LGPL requires that derived works be licensed under the same
-license, but works that only link to it do not fall under this restriction.
-There are two commonly used versions of the GNU LGPL. See [LICENSE](https://
-github.com/arushadev/piraye/blob/main/LICENSE) ## About ï¸ [Arusha](https://
-www.arusha.dev)
+# "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` You can find
+more examples [here](https://github.com/arushadev/piraye/blob/readme/
+examples.md) ## Configs Piraye provides various configurations for text
+normalization. Here's a list of available configurations: | Config | Function |
+Description | |:----------------:|:----------------:|:-------------------------
+----------------------------:| | ALPHABET_AR | alphabet_ar | mapping alphabet
+characters to Arabic | | ALPHABET_EN | alphabet_en | mapping alphabet
+characters to English | | ALPHABET_FA | alphabet_fa | mapping alphabet
+characters to Persian | | DIGIT_AR | digit_ar | convert digits to Arabic digits
+| | DIGIT_EN | digit_en | convert digits to English digits | | DIGIT_FA |
+digit_fa | convert digits to Persian digits | | DIACRITIC_DELETE |
+diacritic_delete | remove all diacritics | | SPACE_DELETE | space_delete |
+remove all spaces | | SPACE_NORMAL | space_normal | normal spaces ( like NO-
+BREAK SPACE , Tab and etc...) | | SPACE_KEEP | space_keep | mapping spaces and
+not normal them | | PUNCTUATION_AR | punctuation_ar | mapping punctuations to
+Arabic punctuations | | PUNCTUATION_Fa | punctuation_fa | mapping punctuations
+to Persian punctuations | | PUNCTUATION_EN | punctuation_en | mapping
+punctuations to English punctuations | Other attributes: * remove_extra_spaces:
+Appends multiple spaces together. * tokenization: Replaces punctuation
+characters which are just tokens. ## Development To set up a development
+environment, install dependencies with: `pip install -e .[dev]` ## License
+**GNU Lesser General Public License v2.1** Piraye is licensed under the GNU
+Lesser General Public License v2.1, which primarily applies to software
+libraries. See the [LICENSE](https://github.com/arushadev/piraye/blob/main/
+LICENSE) file for more details. ## About ï¸ Piraye is maintained by [Arusha]
+(https://www.arusha.dev).
```

### Comparing `piraye-0.4.0/README.md` & `piraye-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Piraye: NLP Utils
+# Piraye: NLP Utilities
 
 <p align="center">
   <a href="https://pypi.org/project/piraye"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/piraye.svg?maxAge=86400" /></a>
   <a href="https://pypi.org/project/piraye"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/piraye.svg?maxAge=86400" /></a>
   <a href="https://pypi.org/project/piraye"><img alt="License" src="https://img.shields.io/pypi/l/piraye.svg?maxAge=86400" /></a>
+  <a href="https://pepy.tech/project/piraye"><img alt="Downloads" src="https://static.pepy.tech/badge/piraye" /></a>
   <a href="https://github.com/arushadev/piraye/actions/workflows/pylint.yml"><img alt="Pylint" src="https://github.com/arushadev/piraye/actions/workflows/pylint.yml/badge.svg" /></a>
   <a href="https://github.com/arushadev/piraye/actions/workflows/unit-test.yml/badge.svg)](https://github.com/arushadev/piraye/actions/workflows/unit-test.yml"><img alt="Unit Test" src="https://github.com/arushadev/piraye/actions/workflows/unit-test.yml/badge.svg" /></a>
 </p>
 
 
-A utility for normalizing persian, arabic and english texts
+**Piraye** is a Python library designed to facilitate text normalization for Persian, Arabic, and English languages.
 
 ## Requirements
 
 * Python 3.11+
 * nltk 3.4.5+
 
 ## Installation
 
-Install the latest version with pip
+You can install the latest version of Piraye via pip:
+
 `pip install piraye`
 
 ## Usage
 
-Create an instance of Normalizer with NormalizerBuilder and then call normalize function. Also see list of all available
-configs in [configs](#Configs) section.
+To use Piraye, create an instance of the Normalizer class with NormalizerBuilder and then call the normalize function. You can configure the normalization process using various settings available. Below are two examples demonstrating different approaches:
 
 * Using builder pattern:
 
 ```python
 from piraye import NormalizerBuilder
-from piraye.tasks.normalizer.normalizer_builder import Config
 
 text = "این یک متن تسة اسﺘ       , 24/12/1400 "
 normalizer = NormalizerBuilder().alphabet_fa().digit_fa().punctuation_fa().tokenizing().remove_extra_spaces().build()
 normalizer.normalize(text)  # "این یک متن تست است ، ۲۴/۱۲/۱۴۰۰"
 ```
 
 * Using constructor:
@@ -45,49 +45,52 @@
 
 text = "این یک متن تسة اسﺘ       , 24/12/1400 "
 normalizer = NormalizerBuilder([Config.PUNCTUATION_FA, Config.ALPHABET_FA, Config.DIGIT_FA], remove_extra_spaces=True,
                                tokenization=True).build()
 normalizer.normalize(text)  # "این یک متن تست است ، ۲۴/۱۲/۱۴۰۰"
 ```
 
-Also see [other examples](https://github.com/arushadev/piraye/blob/readme/examples.md)
+You can find more examples [here](https://github.com/arushadev/piraye/blob/readme/examples.md)
 
 ## Configs
 
+Piraye provides various configurations for text normalization. Here's a list of available configurations:
+
 |      Config      |     Function     |                      Description                      |
 |:----------------:|:----------------:|:-----------------------------------------------------:|
-|   ALPHABET_AR    |   alphabet_ar    |         mapping alphabet characters to arabic         |
-|   ALPHABET_EN    |   alphabet_en    |        mapping alphabet characters to english         |
-|   ALPHABET_FA    |   alphabet_fa    |        mapping alphabet characters to persian         |
-|     DIGIT_AR     |     digit_ar     |            convert digits to arabic digits            |
-|     DIGIT_EN     |     digit_en     |           convert digits to english digits            |
-|     DIGIT_FA     |     digit_fa     |           convert digits to persian digits            |
+|   ALPHABET_AR    |   alphabet_ar    |         mapping alphabet characters to Arabic         |
+|   ALPHABET_EN    |   alphabet_en    |        mapping alphabet characters to English         |
+|   ALPHABET_FA    |   alphabet_fa    |        mapping alphabet characters to Persian         |
+|     DIGIT_AR     |     digit_ar     |            convert digits to Arabic digits            |
+|     DIGIT_EN     |     digit_en     |           convert digits to English digits            |
+|     DIGIT_FA     |     digit_fa     |           convert digits to Persian digits            |
 | DIACRITIC_DELETE | diacritic_delete |                 remove all diacritics                 |
 |   SPACE_DELETE   |   space_delete   |                   remove all spaces                   |
 |   SPACE_NORMAL   |   space_normal   | normal spaces ( like NO-BREAK SPACE , Tab and etc...) |
 |    SPACE_KEEP    |    space_keep    |          mapping spaces and not normal them           |
-|  PUNCTUATION_AR  |  punctuation_ar  |      mapping punctuations to arabic punctuations      |
-|  PUNCTUATION_Fa  |  punctuation_fa  |     mapping punctuations to persian punctuations      |
-|  PUNCTUATION_EN  |  punctuation_en  |     mapping punctuations to english punctuations      |
+|  PUNCTUATION_AR  |  punctuation_ar  |      mapping punctuations to Arabic punctuations      |
+|  PUNCTUATION_Fa  |  punctuation_fa  |     mapping punctuations to Persian punctuations      |
+|  PUNCTUATION_EN  |  punctuation_en  |     mapping punctuations to English punctuations      |
 
 Other attributes:
 
-* remove_extra_spaces : append multiple spaces together
-* tokenization : replace punctuation characters that just are tokens
+* remove_extra_spaces: Appends multiple spaces together.
+* tokenization: Replaces punctuation characters which are just tokens.
 
 ## Development
 
-* Install dependencies with `pip install -e .[dev]`
+To set up a development environment, install dependencies with:
+
+`pip install -e .[dev]`
 
 ## License
 
 **GNU Lesser General Public License v2.1**
 
-Primarily used for software libraries, the GNU LGPL requires that derived works be licensed under the same license, but
-works that only link to it do not fall under this restriction. There are two commonly used versions of the GNU LGPL.
-
-See [LICENSE](https://github.com/arushadev/piraye/blob/main/LICENSE)
+Piraye is licensed under the GNU Lesser General Public License v2.1, which primarily applies to software libraries.
+See the [LICENSE](https://github.com/arushadev/piraye/blob/main/LICENSE) file for more details.
 
 ## About ️
 
-[Arusha](https://www.arusha.dev)
+Piraye is maintained by [Arusha](https://www.arusha.dev).
+
```

#### html2text {}

```diff
@@ -1,42 +1,44 @@
-# Piraye: NLP Utils
-          _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_P_y_l_i_n_t_]_[_U_n_i_t_ _T_e_s_t_]
-A utility for normalizing persian, arabic and english texts ## Requirements *
-Python 3.11+ * nltk 3.4.5+ ## Installation Install the latest version with pip
-`pip install piraye` ## Usage Create an instance of Normalizer with
-NormalizerBuilder and then call normalize function. Also see list of all
-available configs in [configs](#Configs) section. * Using builder pattern:
-```python from piraye import NormalizerBuilder from
-piraye.tasks.normalizer.normalizer_builder import Config text = "Ø§ÛÙ ÛÚ©
+# Piraye: NLP Utilities
+    _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_P_y_l_i_n_t_]_[_U_n_i_t_ _T_e_s_t_]
+**Piraye** is a Python library designed to facilitate text normalization for
+Persian, Arabic, and English languages. ## Requirements * Python 3.11+ * nltk
+3.4.5+ ## Installation You can install the latest version of Piraye via pip:
+`pip install piraye` ## Usage To use Piraye, create an instance of the
+Normalizer class with NormalizerBuilder and then call the normalize function.
+You can configure the normalization process using various settings available.
+Below are two examples demonstrating different approaches: * Using builder
+pattern: ```python from piraye import NormalizerBuilder text = "Ø§ÛÙ ÛÚ©
 ÙØªÙ ØªØ³Ø© Ø§Ø³ïº , 24/12/1400 " normalizer = NormalizerBuilder
 ().alphabet_fa().digit_fa().punctuation_fa().tokenizing().remove_extra_spaces
 ().build() normalizer.normalize(text) # "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø
 Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` * Using constructor: ```python from piraye import
 NormalizerBuilder from piraye.tasks.normalizer.normalizer_builder import Config
 text = "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Ø© Ø§Ø³ïº , 24/12/1400 " normalizer =
 NormalizerBuilder([Config.PUNCTUATION_FA, Config.ALPHABET_FA, Config.DIGIT_FA],
 remove_extra_spaces=True, tokenization=True).build() normalizer.normalize(text)
-# "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` Also see [other
-examples](https://github.com/arushadev/piraye/blob/readme/examples.md) ##
-Configs | Config | Function | Description | |:----------------:|:--------------
---:|:-----------------------------------------------------:| | ALPHABET_AR |
-alphabet_ar | mapping alphabet characters to arabic | | ALPHABET_EN |
-alphabet_en | mapping alphabet characters to english | | ALPHABET_FA |
-alphabet_fa | mapping alphabet characters to persian | | DIGIT_AR | digit_ar |
-convert digits to arabic digits | | DIGIT_EN | digit_en | convert digits to
-english digits | | DIGIT_FA | digit_fa | convert digits to persian digits | |
-DIACRITIC_DELETE | diacritic_delete | remove all diacritics | | SPACE_DELETE |
-space_delete | remove all spaces | | SPACE_NORMAL | space_normal | normal
-spaces ( like NO-BREAK SPACE , Tab and etc...) | | SPACE_KEEP | space_keep |
-mapping spaces and not normal them | | PUNCTUATION_AR | punctuation_ar |
-mapping punctuations to arabic punctuations | | PUNCTUATION_Fa | punctuation_fa
-| mapping punctuations to persian punctuations | | PUNCTUATION_EN |
-punctuation_en | mapping punctuations to english punctuations | Other
-attributes: * remove_extra_spaces : append multiple spaces together *
-tokenization : replace punctuation characters that just are tokens ##
-Development * Install dependencies with `pip install -e .[dev]` ## License
-**GNU Lesser General Public License v2.1** Primarily used for software
-libraries, the GNU LGPL requires that derived works be licensed under the same
-license, but works that only link to it do not fall under this restriction.
-There are two commonly used versions of the GNU LGPL. See [LICENSE](https://
-github.com/arushadev/piraye/blob/main/LICENSE) ## About ï¸ [Arusha](https://
-www.arusha.dev)
+# "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` You can find
+more examples [here](https://github.com/arushadev/piraye/blob/readme/
+examples.md) ## Configs Piraye provides various configurations for text
+normalization. Here's a list of available configurations: | Config | Function |
+Description | |:----------------:|:----------------:|:-------------------------
+----------------------------:| | ALPHABET_AR | alphabet_ar | mapping alphabet
+characters to Arabic | | ALPHABET_EN | alphabet_en | mapping alphabet
+characters to English | | ALPHABET_FA | alphabet_fa | mapping alphabet
+characters to Persian | | DIGIT_AR | digit_ar | convert digits to Arabic digits
+| | DIGIT_EN | digit_en | convert digits to English digits | | DIGIT_FA |
+digit_fa | convert digits to Persian digits | | DIACRITIC_DELETE |
+diacritic_delete | remove all diacritics | | SPACE_DELETE | space_delete |
+remove all spaces | | SPACE_NORMAL | space_normal | normal spaces ( like NO-
+BREAK SPACE , Tab and etc...) | | SPACE_KEEP | space_keep | mapping spaces and
+not normal them | | PUNCTUATION_AR | punctuation_ar | mapping punctuations to
+Arabic punctuations | | PUNCTUATION_Fa | punctuation_fa | mapping punctuations
+to Persian punctuations | | PUNCTUATION_EN | punctuation_en | mapping
+punctuations to English punctuations | Other attributes: * remove_extra_spaces:
+Appends multiple spaces together. * tokenization: Replaces punctuation
+characters which are just tokens. ## Development To set up a development
+environment, install dependencies with: `pip install -e .[dev]` ## License
+**GNU Lesser General Public License v2.1** Piraye is licensed under the GNU
+Lesser General Public License v2.1, which primarily applies to software
+libraries. See the [LICENSE](https://github.com/arushadev/piraye/blob/main/
+LICENSE) file for more details. ## About ï¸ Piraye is maintained by [Arusha]
+(https://www.arusha.dev).
```

### Comparing `piraye-0.4.0/piraye/__init__.py` & `piraye-0.5.0/piraye/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module includes Normalizer and NormalizerBuilder"""
 from .normalizer import Normalizer
 from .tasks.normalizer.multi_lingual_normalizer import MultiLingualNormalizer
 from .tasks.normalizer.multi_lingual_normalizer_builder import MultiLingualNormalizerBuilder
 from .tasks.normalizer.normalizer_builder import NormalizerBuilder
 from .tasks.tokenizer.nltk_tokenizer import NltkTokenizer
+from .tasks.tokenizer.spacy_tokenizer import SpacyTokenizer
 from .tokenizer import Tokenizer
 
 __all__ = ["Normalizer", "Tokenizer", "NormalizerBuilder", "MultiLingualNormalizer", "MultiLingualNormalizerBuilder",
-           "NltkTokenizer"]
+           "NltkTokenizer", "SpacyTokenizer"]
```

### Comparing `piraye-0.4.0/piraye/normalizer.py` & `piraye-0.5.0/piraye/normalizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
 
 class Normalizer(ABC):
     """
     The Normalizer class is an abstract base class that defines the interface for text normalization. It provides two
-    abstract methods: normalize() and span_normalize(), which can be implemented by subclasses to perform specific
+    abstract methods: normalize() and span_normalize(), subclasses can implement which to perform specific
     normalization tasks.
 
     Example Usage
 
     # Create a subclass of Normalizer
     class MyNormalizer(Normalizer):
 
-        def normalize(self, text: str) -> str:
+        Def normalize (self, text: str) -> str:
             # Implement the normalization logic here
             ...
 
-        def span_normalize(self, text: str) -> List[Tuple[int, int, str]]:
+        Def span_normalize(self, text: str) -> List[Tuple[int, int, str]]:
             # Implement the normalization logic and return spans of normalized tokens
             ...
 
     # Create an instance of the subclass
     normalizer = MyNormalizer()
 
     # Normalize a text
```

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/char_config.py` & `piraye-0.5.0/piraye/tasks/normalizer/char_config.py`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/character_normalizer.py` & `piraye-0.5.0/piraye/tasks/normalizer/character_normalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from __future__ import annotations
 
 from abc import ABC
 from typing import List, Tuple
 
 from .char_config import CharConfig
 from .mappings import MappingDict
-from ..tokenizer.nltk_tokenizer import NltkTokenizer, Tokenizer
+from ..tokenizer.nltk_tokenizer import NltkTokenizer
+from ...tokenizer import Tokenizer
 from ...normalizer import Normalizer
 
 
 # pylint: disable=too-few-public-methods
 class CharacterNormalizer(Normalizer, ABC):
     """
     Impl normalizer by character level normalization
```

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/data/alphabets/ar.json` & `piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/ar.json`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/data/alphabets/en.json` & `piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/en.json`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/data/alphabets/fa.json` & `piraye-0.5.0/piraye/tasks/normalizer/data/alphabets/fa.json`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/data/digits/digits.json` & `piraye-0.5.0/piraye/tasks/normalizer/data/digits/digits.json`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/data/others/diacritics.json` & `piraye-0.5.0/piraye/tasks/normalizer/data/others/diacritics.json`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/data/others/spaces.json` & `piraye-0.5.0/piraye/tasks/normalizer/data/others/spaces.json`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/data/puncs/puncs.json` & `piraye-0.5.0/piraye/tasks/normalizer/data/puncs/puncs.json`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/mappings.py` & `piraye-0.5.0/piraye/tasks/normalizer/mappings.py`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/multi_lingual_normalizer.py` & `piraye-0.5.0/piraye/tasks/normalizer/multi_lingual_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py` & `piraye-0.5.0/piraye/tasks/normalizer/multi_lingual_normalizer_builder.py`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/normalizer/normalizer_builder.py` & `piraye-0.5.0/piraye/tasks/normalizer/normalizer_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import enum
 from typing import List
 
 from .character_normalizer import CharacterNormalizer
 from ...normalizer import Normalizer
+from ...tokenizer import Tokenizer
 
 
 class Config(enum.Enum):
     """
     List of all available configs in this normalizer
     """
     ALPHABET_AR = "alphabet_ar"
@@ -53,14 +54,15 @@
                  tokenization: bool = False):
         """
         Constructor for NormalizerBuilder.
         :param configs: List of normalizer configs to initialize with.
         :param remove_extra_spaces: Whether to remove extra spaces during normalization
         :param tokenization: Whether to tokenize the text during normalization.
         """
+        self.__tokenizer = None
         if configs is None:
             configs = []
         self.__configs = configs
         self.__remove_extra_spaces = remove_extra_spaces
         self.__tokenization = tokenization
 
     def build(self) -> Normalizer:
@@ -70,15 +72,15 @@
         """
         if self.__remove_extra_spaces and \
                 not (Config.SPACE_DELETE in self.__configs or
                      Config.SPACE_KEEP in self.__configs or
                      Config.SPACE_NORMAL in self.__configs):
             self.__configs.append(Config.SPACE_KEEP)
         return CharacterNormalizer([c.value for c in self.__configs],
-                                   self.__remove_extra_spaces, self.__tokenization)
+                                   self.__remove_extra_spaces, self.__tokenization,self.__tokenizer)
 
     def alphabet_ar(self) -> NormalizerBuilder:
         """
         Add Config.ALPHABET_AR to the configuration.
         :return: Self
         """
         self.__configs.append(Config.ALPHABET_AR)
@@ -192,13 +194,14 @@
         """
         Config whether delete remove extra space or not
         :return: Self
         """
         self.__remove_extra_spaces = remove_extra_spaces
         return self
 
-    def tokenizing(self, tokenization: bool = True) -> NormalizerBuilder:
+    def tokenizing(self, tokenization: bool = True, tokenizer: Tokenizer = None) -> NormalizerBuilder:
         """
         Config whether tokenize before normalization or not
         """
         self.__tokenization = tokenization
+        self.__tokenizer = tokenizer
         return self
```

### Comparing `piraye-0.4.0/piraye/tasks/punc/punctuation_restoration.py` & `piraye-0.5.0/piraye/tasks/punc/punctuation_restoration.py`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tasks/tokenizer/nltk_tokenizer.py` & `piraye-0.5.0/piraye/tasks/tokenizer/nltk_tokenizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye/tokenizer.py` & `piraye-0.5.0/piraye/tokenizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/piraye.egg-info/PKG-INFO` & `piraye-0.5.0/piraye.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piraye
-Version: 0.4.0
+Version: 0.5.0
 Summary: A utility for normalizing persian, arabic and english texts
 Author-email: Hamed Khademi Khaledi <khaledihkh@gmail.com>, HosseiN Khademi khaeldi <hossein@arusha.dev>, Majid Asgiar Bidhendi <majid@arusha.dev>
 Maintainer-email: Arusha Developers <info@arusha.dev>
 License: LGPLv2
 Project-URL: Homepage, https://github.com/arushadev/piraye
 Project-URL: Bug Tracker, https://github.com/arushadev/piraye/issues
 Keywords: NLP,Natural Language Processing,Tokenizing,Normalization
@@ -30,48 +30,49 @@
 Requires-Dist: lingua-language-detector
 Provides-Extra: dev
 Requires-Dist: tqdm; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint==2.17.7; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: spacy; extra == "dev"
 
-# Piraye: NLP Utils
+# Piraye: NLP Utilities
 
 <p align="center">
   <a href="https://pypi.org/project/piraye"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/piraye.svg?maxAge=86400" /></a>
   <a href="https://pypi.org/project/piraye"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/piraye.svg?maxAge=86400" /></a>
   <a href="https://pypi.org/project/piraye"><img alt="License" src="https://img.shields.io/pypi/l/piraye.svg?maxAge=86400" /></a>
+  <a href="https://pepy.tech/project/piraye"><img alt="Downloads" src="https://static.pepy.tech/badge/piraye" /></a>
   <a href="https://github.com/arushadev/piraye/actions/workflows/pylint.yml"><img alt="Pylint" src="https://github.com/arushadev/piraye/actions/workflows/pylint.yml/badge.svg" /></a>
   <a href="https://github.com/arushadev/piraye/actions/workflows/unit-test.yml/badge.svg)](https://github.com/arushadev/piraye/actions/workflows/unit-test.yml"><img alt="Unit Test" src="https://github.com/arushadev/piraye/actions/workflows/unit-test.yml/badge.svg" /></a>
 </p>
 
 
-A utility for normalizing persian, arabic and english texts
+**Piraye** is a Python library designed to facilitate text normalization for Persian, Arabic, and English languages.
 
 ## Requirements
 
 * Python 3.11+
 * nltk 3.4.5+
 
 ## Installation
 
-Install the latest version with pip
+You can install the latest version of Piraye via pip:
+
 `pip install piraye`
 
 ## Usage
 
-Create an instance of Normalizer with NormalizerBuilder and then call normalize function. Also see list of all available
-configs in [configs](#Configs) section.
+To use Piraye, create an instance of the Normalizer class with NormalizerBuilder and then call the normalize function. You can configure the normalization process using various settings available. Below are two examples demonstrating different approaches:
 
 * Using builder pattern:
 
 ```python
 from piraye import NormalizerBuilder
-from piraye.tasks.normalizer.normalizer_builder import Config
 
 text = "این یک متن تسة اسﺘ       , 24/12/1400 "
 normalizer = NormalizerBuilder().alphabet_fa().digit_fa().punctuation_fa().tokenizing().remove_extra_spaces().build()
 normalizer.normalize(text)  # "این یک متن تست است ، ۲۴/۱۲/۱۴۰۰"
 ```
 
 * Using constructor:
@@ -82,49 +83,52 @@
 
 text = "این یک متن تسة اسﺘ       , 24/12/1400 "
 normalizer = NormalizerBuilder([Config.PUNCTUATION_FA, Config.ALPHABET_FA, Config.DIGIT_FA], remove_extra_spaces=True,
                                tokenization=True).build()
 normalizer.normalize(text)  # "این یک متن تست است ، ۲۴/۱۲/۱۴۰۰"
 ```
 
-Also see [other examples](https://github.com/arushadev/piraye/blob/readme/examples.md)
+You can find more examples [here](https://github.com/arushadev/piraye/blob/readme/examples.md)
 
 ## Configs
 
+Piraye provides various configurations for text normalization. Here's a list of available configurations:
+
 |      Config      |     Function     |                      Description                      |
 |:----------------:|:----------------:|:-----------------------------------------------------:|
-|   ALPHABET_AR    |   alphabet_ar    |         mapping alphabet characters to arabic         |
-|   ALPHABET_EN    |   alphabet_en    |        mapping alphabet characters to english         |
-|   ALPHABET_FA    |   alphabet_fa    |        mapping alphabet characters to persian         |
-|     DIGIT_AR     |     digit_ar     |            convert digits to arabic digits            |
-|     DIGIT_EN     |     digit_en     |           convert digits to english digits            |
-|     DIGIT_FA     |     digit_fa     |           convert digits to persian digits            |
+|   ALPHABET_AR    |   alphabet_ar    |         mapping alphabet characters to Arabic         |
+|   ALPHABET_EN    |   alphabet_en    |        mapping alphabet characters to English         |
+|   ALPHABET_FA    |   alphabet_fa    |        mapping alphabet characters to Persian         |
+|     DIGIT_AR     |     digit_ar     |            convert digits to Arabic digits            |
+|     DIGIT_EN     |     digit_en     |           convert digits to English digits            |
+|     DIGIT_FA     |     digit_fa     |           convert digits to Persian digits            |
 | DIACRITIC_DELETE | diacritic_delete |                 remove all diacritics                 |
 |   SPACE_DELETE   |   space_delete   |                   remove all spaces                   |
 |   SPACE_NORMAL   |   space_normal   | normal spaces ( like NO-BREAK SPACE , Tab and etc...) |
 |    SPACE_KEEP    |    space_keep    |          mapping spaces and not normal them           |
-|  PUNCTUATION_AR  |  punctuation_ar  |      mapping punctuations to arabic punctuations      |
-|  PUNCTUATION_Fa  |  punctuation_fa  |     mapping punctuations to persian punctuations      |
-|  PUNCTUATION_EN  |  punctuation_en  |     mapping punctuations to english punctuations      |
+|  PUNCTUATION_AR  |  punctuation_ar  |      mapping punctuations to Arabic punctuations      |
+|  PUNCTUATION_Fa  |  punctuation_fa  |     mapping punctuations to Persian punctuations      |
+|  PUNCTUATION_EN  |  punctuation_en  |     mapping punctuations to English punctuations      |
 
 Other attributes:
 
-* remove_extra_spaces : append multiple spaces together
-* tokenization : replace punctuation characters that just are tokens
+* remove_extra_spaces: Appends multiple spaces together.
+* tokenization: Replaces punctuation characters which are just tokens.
 
 ## Development
 
-* Install dependencies with `pip install -e .[dev]`
+To set up a development environment, install dependencies with:
+
+`pip install -e .[dev]`
 
 ## License
 
 **GNU Lesser General Public License v2.1**
 
-Primarily used for software libraries, the GNU LGPL requires that derived works be licensed under the same license, but
-works that only link to it do not fall under this restriction. There are two commonly used versions of the GNU LGPL.
-
-See [LICENSE](https://github.com/arushadev/piraye/blob/main/LICENSE)
+Piraye is licensed under the GNU Lesser General Public License v2.1, which primarily applies to software libraries.
+See the [LICENSE](https://github.com/arushadev/piraye/blob/main/LICENSE) file for more details.
 
 ## About ️
 
-[Arusha](https://www.arusha.dev)
+Piraye is maintained by [Arusha](https://www.arusha.dev).
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: piraye Version: 0.4.0 Summary: A utility for
+Metadata-Version: 2.1 Name: piraye Version: 0.5.0 Summary: A utility for
 normalizing persian, arabic and english texts Author-email: Hamed Khademi
 Khaledi
 gmail.com>, HosseiN Khademi khaeldi
 arusha.dev>, Majid Asgiar Bidhendi
 arusha.dev> Maintainer-email: Arusha Developers
 arusha.dev> License: LGPLv2 Project-URL: Homepage, https://github.com/
 arushadev/piraye Project-URL: Bug Tracker, https://github.com/arushadev/piraye/
@@ -17,50 +17,52 @@
 Intelligence Classifier: Topic :: Text Processing Classifier: Topic :: Text
 Processing :: Filters Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic ::
 Utilities Requires-Python: >=3.11 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: nltk Requires-Dist: lingua-language-
 detector Provides-Extra: dev Requires-Dist: tqdm; extra == "dev" Requires-Dist:
 pytest; extra == "dev" Requires-Dist: pylint==2.17.7; extra == "dev" Requires-
-Dist: flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" # Piraye:
-NLP Utils
-          _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_P_y_l_i_n_t_]_[_U_n_i_t_ _T_e_s_t_]
-A utility for normalizing persian, arabic and english texts ## Requirements *
-Python 3.11+ * nltk 3.4.5+ ## Installation Install the latest version with pip
-`pip install piraye` ## Usage Create an instance of Normalizer with
-NormalizerBuilder and then call normalize function. Also see list of all
-available configs in [configs](#Configs) section. * Using builder pattern:
-```python from piraye import NormalizerBuilder from
-piraye.tasks.normalizer.normalizer_builder import Config text = "Ø§ÛÙ ÛÚ©
+Dist: flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
+Dist: spacy; extra == "dev" # Piraye: NLP Utilities
+    _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_P_y_l_i_n_t_]_[_U_n_i_t_ _T_e_s_t_]
+**Piraye** is a Python library designed to facilitate text normalization for
+Persian, Arabic, and English languages. ## Requirements * Python 3.11+ * nltk
+3.4.5+ ## Installation You can install the latest version of Piraye via pip:
+`pip install piraye` ## Usage To use Piraye, create an instance of the
+Normalizer class with NormalizerBuilder and then call the normalize function.
+You can configure the normalization process using various settings available.
+Below are two examples demonstrating different approaches: * Using builder
+pattern: ```python from piraye import NormalizerBuilder text = "Ø§ÛÙ ÛÚ©
 ÙØªÙ ØªØ³Ø© Ø§Ø³ïº , 24/12/1400 " normalizer = NormalizerBuilder
 ().alphabet_fa().digit_fa().punctuation_fa().tokenizing().remove_extra_spaces
 ().build() normalizer.normalize(text) # "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø
 Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` * Using constructor: ```python from piraye import
 NormalizerBuilder from piraye.tasks.normalizer.normalizer_builder import Config
 text = "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Ø© Ø§Ø³ïº , 24/12/1400 " normalizer =
 NormalizerBuilder([Config.PUNCTUATION_FA, Config.ALPHABET_FA, Config.DIGIT_FA],
 remove_extra_spaces=True, tokenization=True).build() normalizer.normalize(text)
-# "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` Also see [other
-examples](https://github.com/arushadev/piraye/blob/readme/examples.md) ##
-Configs | Config | Function | Description | |:----------------:|:--------------
---:|:-----------------------------------------------------:| | ALPHABET_AR |
-alphabet_ar | mapping alphabet characters to arabic | | ALPHABET_EN |
-alphabet_en | mapping alphabet characters to english | | ALPHABET_FA |
-alphabet_fa | mapping alphabet characters to persian | | DIGIT_AR | digit_ar |
-convert digits to arabic digits | | DIGIT_EN | digit_en | convert digits to
-english digits | | DIGIT_FA | digit_fa | convert digits to persian digits | |
-DIACRITIC_DELETE | diacritic_delete | remove all diacritics | | SPACE_DELETE |
-space_delete | remove all spaces | | SPACE_NORMAL | space_normal | normal
-spaces ( like NO-BREAK SPACE , Tab and etc...) | | SPACE_KEEP | space_keep |
-mapping spaces and not normal them | | PUNCTUATION_AR | punctuation_ar |
-mapping punctuations to arabic punctuations | | PUNCTUATION_Fa | punctuation_fa
-| mapping punctuations to persian punctuations | | PUNCTUATION_EN |
-punctuation_en | mapping punctuations to english punctuations | Other
-attributes: * remove_extra_spaces : append multiple spaces together *
-tokenization : replace punctuation characters that just are tokens ##
-Development * Install dependencies with `pip install -e .[dev]` ## License
-**GNU Lesser General Public License v2.1** Primarily used for software
-libraries, the GNU LGPL requires that derived works be licensed under the same
-license, but works that only link to it do not fall under this restriction.
-There are two commonly used versions of the GNU LGPL. See [LICENSE](https://
-github.com/arushadev/piraye/blob/main/LICENSE) ## About ï¸ [Arusha](https://
-www.arusha.dev)
+# "Ø§ÛÙ ÛÚ© ÙØªÙ ØªØ³Øª Ø§Ø³Øª Ø Û²Û´/Û±Û²/Û±Û´Û°Û°" ``` You can find
+more examples [here](https://github.com/arushadev/piraye/blob/readme/
+examples.md) ## Configs Piraye provides various configurations for text
+normalization. Here's a list of available configurations: | Config | Function |
+Description | |:----------------:|:----------------:|:-------------------------
+----------------------------:| | ALPHABET_AR | alphabet_ar | mapping alphabet
+characters to Arabic | | ALPHABET_EN | alphabet_en | mapping alphabet
+characters to English | | ALPHABET_FA | alphabet_fa | mapping alphabet
+characters to Persian | | DIGIT_AR | digit_ar | convert digits to Arabic digits
+| | DIGIT_EN | digit_en | convert digits to English digits | | DIGIT_FA |
+digit_fa | convert digits to Persian digits | | DIACRITIC_DELETE |
+diacritic_delete | remove all diacritics | | SPACE_DELETE | space_delete |
+remove all spaces | | SPACE_NORMAL | space_normal | normal spaces ( like NO-
+BREAK SPACE , Tab and etc...) | | SPACE_KEEP | space_keep | mapping spaces and
+not normal them | | PUNCTUATION_AR | punctuation_ar | mapping punctuations to
+Arabic punctuations | | PUNCTUATION_Fa | punctuation_fa | mapping punctuations
+to Persian punctuations | | PUNCTUATION_EN | punctuation_en | mapping
+punctuations to English punctuations | Other attributes: * remove_extra_spaces:
+Appends multiple spaces together. * tokenization: Replaces punctuation
+characters which are just tokens. ## Development To set up a development
+environment, install dependencies with: `pip install -e .[dev]` ## License
+**GNU Lesser General Public License v2.1** Piraye is licensed under the GNU
+Lesser General Public License v2.1, which primarily applies to software
+libraries. See the [LICENSE](https://github.com/arushadev/piraye/blob/main/
+LICENSE) file for more details. ## About ï¸ Piraye is maintained by [Arusha]
+(https://www.arusha.dev).
```

### Comparing `piraye-0.4.0/piraye.egg-info/SOURCES.txt` & `piraye-0.5.0/piraye.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,10 +26,11 @@
 piraye/tasks/normalizer/data/others/spaces.json
 piraye/tasks/normalizer/data/puncs/puncs.json
 piraye/tasks/punc/__init__.py
 piraye/tasks/punc/punctuation_restoration.py
 piraye/tasks/tokenizer/__init__.py
 piraye/tasks/tokenizer/nltk_tokenizer.py
 piraye/tasks/tokenizer/punc_tokenizer.py
+piraye/tasks/tokenizer/spacy_tokenizer.py
 tests/test_ml_normalizer.py
 tests/test_normalizer.py
 tests/test_tokenizer.py
```

### Comparing `piraye-0.4.0/pyproject.toml` & `piraye-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "piraye"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
     { name = "Hamed Khademi Khaledi", email = "khaledihkh@gmail.com" },
     { name = "HosseiN Khademi khaeldi", email = "hossein@arusha.dev" },
     { name = "Majid Asgiar Bidhendi", email = "majid@arusha.dev" },
 ]
 maintainers = [
     { name = "Arusha Developers", email = "info@arusha.dev" },
@@ -52,12 +52,12 @@
 exclude = ["tests"]
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [tool.setuptools.package-data]
 piraye = ["**/*.json"]
 
 [project.optional-dependencies]
-dev = ["tqdm", "pytest", "pylint ==2.17.7", "flake8", "pytest"]
+dev = ["tqdm", "pytest", "pylint ==2.17.7", "flake8", "pytest", "spacy"]
 
 [project.urls]
 "Homepage" = "https://github.com/arushadev/piraye"
 "Bug Tracker" = "https://github.com/arushadev/piraye/issues"
```

### Comparing `piraye-0.4.0/tests/test_ml_normalizer.py` & `piraye-0.5.0/tests/test_ml_normalizer.py`

 * *Files identical despite different names*

### Comparing `piraye-0.4.0/tests/test_normalizer.py` & `piraye-0.5.0/tests/test_normalizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # testing Fibonacci number function
 # pylint: skip-file
-
-from ..piraye import NltkTokenizer
+from ..piraye import NltkTokenizer, SpacyTokenizer
 from ..piraye import NormalizerBuilder
 
 
 def test_object():
     norm = NormalizerBuilder().build()
     assert norm is not None
 
@@ -41,14 +40,30 @@
     norm.normalize(text)
     text = " «««« تست "
     norm = NormalizerBuilder().digit_en().punctuation_en().alphabet_fa() \
         .tokenizing().remove_extra_spaces().build()
     norm.normalize(text)
     text = " \" تست '' تست «««« تست "
     norm = NormalizerBuilder().digit_en().punctuation_en().alphabet_fa() \
+        .tokenizing().remove_extra_spaces().build()
+    norm.normalize(text)
+
+
+def test_quotes_spacy():
+    tokenizer = SpacyTokenizer()
+    text = "«"
+    norm = NormalizerBuilder().digit_en().punctuation_en().alphabet_fa() \
+        .tokenizing().remove_extra_spaces().tokenizing(tokenizer=tokenizer).build()
+    norm.normalize(text)
+    text = " «««« تست "
+    norm = NormalizerBuilder().digit_en().punctuation_en().alphabet_fa() \
+        .tokenizing().remove_extra_spaces().build()
+    norm.normalize(text)
+    text = " \" تست '' تست «««« تست "
+    norm = NormalizerBuilder().digit_en().punctuation_en().alphabet_fa() \
         .tokenizing().remove_extra_spaces().build()
     norm.normalize(text)
 
 
 def test_normalizer():
     tokens = NltkTokenizer().word_tokenize('\'\'Y\'"')
     print(tokens)
```

### Comparing `piraye-0.4.0/tests/test_tokenizer.py` & `piraye-0.5.0/tests/test_tokenizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,59 @@
 # testing Fibonacci number function
 # pylint: skip-file
-
-from ..piraye import NltkTokenizer
+from ..piraye import NltkTokenizer, SpacyTokenizer
 
 
 def test_object():
     tokenizer = NltkTokenizer()
     assert tokenizer is not None
 
 
 def test_sample():
     text = "برای تست شماره ۲.۱ نوشته شده است"
     tokenizer = NltkTokenizer()
     assert len(tokenizer.word_tokenize(text)) == 7
 
 
+def test_sample_spacy():
+    text = "برای تست (شماره ۲.۱ نوشته) شده است"
+    tokenizer = SpacyTokenizer()
+    assert len(tokenizer.word_tokenize(text)) == 9
+
+
 def test_double_quotes():
     text = "'\"\"تست\""
     tokenizer = NltkTokenizer()
     assert len(tokenizer.word_tokenize(text)) == 5
 
 
 def test_sentence_tokenizer():
     text = "sentence1 sad. \n asd asd \n asdasd \n sentence 2."
     tokenizer = NltkTokenizer()
     assert len(tokenizer.sentence_tokenize(text)) == 2
     assert len(tokenizer.sentence_span_tokenize(text)) == 2
 
 
+def test_sentence_tokenizer_spacy():
+    text = "sentence1 sad. \n asd asd \n asdasd \n sentence 2."
+    tokenizer = SpacyTokenizer()
+    assert len(tokenizer.sentence_tokenize(text)) == 2
+    assert len(tokenizer.sentence_span_tokenize(text)) == 2
+
+
 def test_double_quotes2():
     text = "«»"
     tokenizer = NltkTokenizer()
     assert len(tokenizer.word_tokenize(text)) == 2
+
+
+def test_link():
+    # To check nltk is functioning wrong for links
+    text = "این یک لینک تست است https://www.google.com "
+    tokenizer = NltkTokenizer()
+    assert len(tokenizer.word_tokenize(text)) != 9
+
+
+def test_link_spacy():
+    text = "این یک لینک، (تست) است https://www.google.com "
+    tokenizer = SpacyTokenizer()
+    assert len(tokenizer.word_tokenize(text)) == 9
```

