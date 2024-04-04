# Comparing `tmp/cmudict-1.0.8.tar.gz` & `tmp/cmudict-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmudict-1.0.8.tar", max compression
+gzip compressed data, was "cmudict-1.0.9.tar", max compression
```

## Comparing `cmudict-1.0.8.tar` & `cmudict-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35147 2022-12-10 22:36:34.102901 cmudict-1.0.8/LICENSE
--rw-r--r--   0        0        0     2322 2022-12-10 22:36:34.102901 cmudict-1.0.8/README.md
--rw-r--r--   0        0        0     1316 2022-12-10 22:36:52.986939 cmudict-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4282 2022-12-10 22:36:34.102901 cmudict-1.0.8/src/cmudict/__init__.py
--rw-r--r--   0        0        0       43 2022-12-10 22:36:35.122905 cmudict-1.0.8/src/cmudict/data/.git
--rw-r--r--   0        0        0     1754 2022-12-10 22:36:35.126905 cmudict-1.0.8/src/cmudict/data/LICENSE
--rw-r--r--   0        0        0     1412 2022-12-10 22:36:35.126905 cmudict-1.0.8/src/cmudict/data/README
--rw-r--r--   0        0        0     2582 2022-12-10 22:36:35.126905 cmudict-1.0.8/src/cmudict/data/README.developer
--rw-r--r--   0        0        0  3618096 2022-12-10 22:36:35.146905 cmudict-1.0.8/src/cmudict/data/cmudict.dict
--rw-r--r--   0        0        0      382 2022-12-10 22:36:35.146905 cmudict-1.0.8/src/cmudict/data/cmudict.phones
--rw-r--r--   0        0        0      281 2022-12-10 22:36:35.146905 cmudict-1.0.8/src/cmudict/data/cmudict.symbols
--rw-r--r--   0        0        0     1747 2022-12-10 22:36:35.146905 cmudict-1.0.8/src/cmudict/data/cmudict.vp
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 cmudict-1.0.8/setup.py
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 cmudict-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-12-10 22:52:57.088816 cmudict-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2322 2022-12-10 22:52:57.088816 cmudict-1.0.9/README.md
+-rw-r--r--   0        0        0     1316 2022-12-10 22:53:14.245051 cmudict-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4282 2022-12-10 22:52:57.088816 cmudict-1.0.9/src/cmudict/__init__.py
+-rw-r--r--   0        0        0       43 2022-12-10 22:52:58.104832 cmudict-1.0.9/src/cmudict/data/.git
+-rw-r--r--   0        0        0     1754 2022-12-10 22:52:58.108832 cmudict-1.0.9/src/cmudict/data/LICENSE
+-rw-r--r--   0        0        0     1412 2022-12-10 22:52:58.108832 cmudict-1.0.9/src/cmudict/data/README
+-rw-r--r--   0        0        0     2582 2022-12-10 22:52:58.108832 cmudict-1.0.9/src/cmudict/data/README.developer
+-rw-r--r--   0        0        0  3618096 2022-12-10 22:52:58.128832 cmudict-1.0.9/src/cmudict/data/cmudict.dict
+-rw-r--r--   0        0        0      382 2022-12-10 22:52:58.128832 cmudict-1.0.9/src/cmudict/data/cmudict.phones
+-rw-r--r--   0        0        0      281 2022-12-10 22:52:58.128832 cmudict-1.0.9/src/cmudict/data/cmudict.symbols
+-rw-r--r--   0        0        0     1747 2022-12-10 22:52:58.128832 cmudict-1.0.9/src/cmudict/data/cmudict.vp
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 cmudict-1.0.9/setup.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 cmudict-1.0.9/PKG-INFO
```

### Comparing `cmudict-1.0.8/LICENSE` & `cmudict-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cmudict-1.0.8/README.md` & `cmudict-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cmudict-1.0.8/pyproject.toml` & `cmudict-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cmudict"
-version = "1.0.8"
+version = "1.0.9"
 description = "A versioned python wrapper package for The CMU Pronouncing Dictionary data files."
 authors = ["David L. Day <david@davidlday.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/prosegrinder/python-cmudict"
 repository = "https://github.com/prosegrinder/python-cmudict"
 readme = "README.md"
 keywords = ["cmudict"]
```

### Comparing `cmudict-1.0.8/src/cmudict/__init__.py` & `cmudict-1.0.9/src/cmudict/__init__.py`

 * *Files identical despite different names*

### Comparing `cmudict-1.0.8/src/cmudict/data/LICENSE` & `cmudict-1.0.9/src/cmudict/data/LICENSE`

 * *Files identical despite different names*

### Comparing `cmudict-1.0.8/src/cmudict/data/README` & `cmudict-1.0.9/src/cmudict/data/README`

 * *Files identical despite different names*

### Comparing `cmudict-1.0.8/src/cmudict/data/README.developer` & `cmudict-1.0.9/src/cmudict/data/README.developer`

 * *Files identical despite different names*

### Comparing `cmudict-1.0.8/src/cmudict/data/cmudict.dict` & `cmudict-1.0.9/src/cmudict/data/cmudict.dict`

 * *Files identical despite different names*

### Comparing `cmudict-1.0.8/src/cmudict/data/cmudict.vp` & `cmudict-1.0.9/src/cmudict/data/cmudict.vp`

 * *Files identical despite different names*

### Comparing `cmudict-1.0.8/setup.py` & `cmudict-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*'], 'cmudict': ['data/*']}
 
 install_requires = \
 ['importlib-metadata>=5.1.0,<6.0.0', 'importlib-resources>=5.10.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'cmudict',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'A versioned python wrapper package for The CMU Pronouncing Dictionary data files.',
     'long_description': "# CMUdict: Python wrapper for cmudict\n\n[![Latest PyPI version](https://img.shields.io/pypi/v/cmudict.svg)](https://pypi.python.org/pypi/cmudict)\n[![GitHub Workflow Status](https://github.com/prosegrinder/python-cmudict/workflows/Python%20CI/badge.svg?branch=main)](https://github.com/prosegrinder/python-cmudict/actions?query=workflow%3A%22Python+CI%22+branch%3Amain)\n\nCMUdict is a versioned python wrapper package for\n[The CMU Pronouncing Dictionary](https://github.com/cmusphinx/cmudict) data\nfiles. The main purpose is to expose the data with little or no assumption on\nhow it is to be used.\n\n## Installation\n\n`cmudict` is available on PyPI. Simply install it with `pip`:\n\n```bash\npip install cmudict\n```\n\n## Usage\n\nThe cmudict data set includes 4 data files: cmudict.dict, cmudict.phones,\ncmudict.symbols, and cmudict.vp. See\n[The CMU Pronouncing Dictionary](https://github.com/cmusphinx/cmudict) for\ndetails on the data. Chances are, if you're here, you already know what's in the\nfiles.\n\nEach file can be accessed through three functions, one which returns the raw\n(string) contents, one which returns a binary stream of the file, and one which\ndoes minimal processing of the file into an appropriate structure:\n\n```python\n>>> import cmudict\n\n>>> cmudict.dict() # Compatible with NLTK\n>>> cmudict.dict_string()\n>>> cmudict.dict_stream()\n\n>>> cmudict.phones()\n>>> cmudict.phones_string()\n>>> cmudict.phones_stream()\n\n>>> cmudict.symbols()\n>>> cmudict.symbols_string()\n>>> cmudict.symbols_stream()\n\n>>> cmudict.vp()\n>>> cmudict.vp_string()\n>>> cmudict.vp_stream()\n```\n\nThree additional functions are included to maintain compatibility with NLTK:\ncmudict.entries(), cmudict.raw(), and cmudict.words(). See the\n[nltk.corpus.reader.cmudict](http://www.nltk.org/_modules/nltk/corpus/reader/cmudict.html)\ndocumentation for details:\n\n```python\n>>> cmudict.entries() # Compatible with NLTK\n>>> cmudict.raw() # Compatible with NLTK\n>>> cmudict.words() # Compatible with NTLK\n```\n\nAnd finally, the license for the cmudict data set is available as well:\n\n```python\n>>> cmudict.license_string() # Returns the cmudict license as a string\n```\n\n## Credits\n\nBuilt on or modeled after the following open source projects:\n\n- [The CMU Pronouncing Dictionary](https://github.com/cmusphinx/cmudict)\n- [NLTK](https://github.com/nltk/nltk)\n",
     'author': 'David L. Day',
     'author_email': 'david@davidlday.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/prosegrinder/python-cmudict',
```

### Comparing `cmudict-1.0.8/PKG-INFO` & `cmudict-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmudict
-Version: 1.0.8
+Version: 1.0.9
 Summary: A versioned python wrapper package for The CMU Pronouncing Dictionary data files.
 Home-page: https://github.com/prosegrinder/python-cmudict
 License: GPL-3.0-or-later
 Keywords: cmudict
 Author: David L. Day
 Author-email: david@davidlday.com
 Requires-Python: >=3.7.2,<4.0.0
```

