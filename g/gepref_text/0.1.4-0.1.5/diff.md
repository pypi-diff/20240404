# Comparing `tmp/gepref_text-0.1.4.tar.gz` & `tmp/gepref_text-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gepref_text-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gepref_text-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gepref_text-0.1.4.tar` & `gepref_text-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rwxr-xr-x   0        0        0      243 2024-04-02 16:37:32.339747 gepref_text-0.1.4/.cicd/scripts.sh
--rw-r--r--   0        0        0      980 2024-04-02 16:37:32.339747 gepref_text-0.1.4/.github/workflows/cd.yml
--rw-r--r--   0        0        0      364 2024-04-02 16:37:32.339747 gepref_text-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      126 2024-04-02 16:37:32.339747 gepref_text-0.1.4/.gitignore
--rw-r--r--   0        0        0        7 2024-04-02 16:37:32.339747 gepref_text-0.1.4/.python-version
--rw-r--r--   0        0        0     1086 2024-04-02 16:37:32.339747 gepref_text-0.1.4/LICENSE
--rw-r--r--   0        0        0      457 2024-04-02 16:37:32.339747 gepref_text-0.1.4/Makefile
--rw-r--r--   0        0        0     1617 2024-04-02 16:37:32.339747 gepref_text-0.1.4/README.md
--rw-r--r--   0        0        0      638 2024-04-02 16:37:32.339747 gepref_text-0.1.4/doc/Makefile
--rw-r--r--   0        0        0    12449 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/_static/gepref_text.svg
--rw-r--r--   0        0        0    20860 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/_static/preprocessor.svg
--rw-r--r--   0        0        0      764 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/conf.py
--rw-r--r--   0        0        0      959 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/gepref_text.rst
--rw-r--r--   0        0        0      521 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/index.rst
--rw-r--r--   0        0        0      251 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/installation.md
--rw-r--r--   0        0        0       70 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/modules.rst
--rw-r--r--   0        0        0     1170 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/usage.rst
--rw-r--r--   0        0        0     1321 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/usage/custom.md
--rw-r--r--   0        0        0      979 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/usage/filtering.md
--rw-r--r--   0        0        0      952 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/usage/normalization.md
--rw-r--r--   0        0        0      744 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/usage/preprocessor.md
--rw-r--r--   0        0        0     1515 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/usage/regex.md
--rw-r--r--   0        0        0     1060 2024-04-02 16:37:32.343747 gepref_text-0.1.4/doc/source/usage/tokenization.md
--rw-r--r--   0        0        0      651 2024-04-02 16:37:32.343747 gepref_text-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 16:37:32.343747 gepref_text-0.1.4/src/gepref_text/__init__.py
--rw-r--r--   0        0        0      525 2024-04-02 16:37:32.343747 gepref_text-0.1.4/src/gepref_text/base.py
--rw-r--r--   0        0        0     2257 2024-04-02 16:37:32.343747 gepref_text-0.1.4/src/gepref_text/filtering.py
--rw-r--r--   0        0        0     1898 2024-04-02 16:37:32.343747 gepref_text-0.1.4/src/gepref_text/normalization.py
--rw-r--r--   0        0        0        0 2024-04-02 16:37:32.343747 gepref_text-0.1.4/src/gepref_text/py.typed
--rw-r--r--   0        0        0     3374 2024-04-02 16:37:32.343747 gepref_text-0.1.4/src/gepref_text/regex_sub.py
--rw-r--r--   0        0        0     1218 2024-04-02 16:37:32.343747 gepref_text-0.1.4/src/gepref_text/tokenization.py
--rw-r--r--   0        0        0        0 2024-04-02 16:37:32.343747 gepref_text-0.1.4/stubs/nltk/__init__.pyi
--rw-r--r--   0        0        0        0 2024-04-02 16:37:32.343747 gepref_text-0.1.4/stubs/nltk/corpus/__init__.pyi
--rw-r--r--   0        0        0       72 2024-04-02 16:37:32.343747 gepref_text-0.1.4/stubs/nltk/corpus/stopwords.pyi
--rw-r--r--   0        0        0      149 2024-04-02 16:37:32.343747 gepref_text-0.1.4/stubs/nltk/tokenize.pyi
--rw-r--r--   0        0        0      895 2024-04-02 16:37:32.343747 gepref_text-0.1.4/test/test_filtering.py
--rw-r--r--   0        0        0     1300 2024-04-02 16:37:32.343747 gepref_text-0.1.4/test/test_normalization.py
--rw-r--r--   0        0        0     2113 2024-04-02 16:37:32.343747 gepref_text-0.1.4/test/test_regex.py
--rw-r--r--   0        0        0      879 2024-04-02 16:37:32.343747 gepref_text-0.1.4/test/test_tokenization.py
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 gepref_text-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0      243 2024-04-04 00:12:21.859655 gepref_text-0.1.5/.cicd/scripts.sh
+-rw-r--r--   0        0        0      980 2024-04-04 00:12:21.859655 gepref_text-0.1.5/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      364 2024-04-04 00:12:21.859655 gepref_text-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      126 2024-04-04 00:12:21.859655 gepref_text-0.1.5/.gitignore
+-rw-r--r--   0        0        0        7 2024-04-04 00:12:21.859655 gepref_text-0.1.5/.python-version
+-rw-r--r--   0        0        0     1086 2024-04-04 00:12:21.859655 gepref_text-0.1.5/LICENSE
+-rw-r--r--   0        0        0      457 2024-04-04 00:12:21.859655 gepref_text-0.1.5/Makefile
+-rw-r--r--   0        0        0     1617 2024-04-04 00:12:21.859655 gepref_text-0.1.5/README.md
+-rw-r--r--   0        0        0      638 2024-04-04 00:12:21.859655 gepref_text-0.1.5/doc/Makefile
+-rw-r--r--   0        0        0    12449 2024-04-04 00:12:21.859655 gepref_text-0.1.5/doc/source/_static/gepref_text.svg
+-rw-r--r--   0        0        0    20860 2024-04-04 00:12:21.859655 gepref_text-0.1.5/doc/source/_static/preprocessor.svg
+-rw-r--r--   0        0        0      764 2024-04-04 00:12:21.859655 gepref_text-0.1.5/doc/source/conf.py
+-rw-r--r--   0        0        0      959 2024-04-04 00:12:21.859655 gepref_text-0.1.5/doc/source/gepref_text.rst
+-rw-r--r--   0        0        0      521 2024-04-04 00:12:21.859655 gepref_text-0.1.5/doc/source/index.rst
+-rw-r--r--   0        0        0      251 2024-04-04 00:12:21.859655 gepref_text-0.1.5/doc/source/installation.md
+-rw-r--r--   0        0        0       70 2024-04-04 00:12:21.859655 gepref_text-0.1.5/doc/source/modules.rst
+-rw-r--r--   0        0        0     1170 2024-04-04 00:12:21.863655 gepref_text-0.1.5/doc/source/usage.rst
+-rw-r--r--   0        0        0     1321 2024-04-04 00:12:21.863655 gepref_text-0.1.5/doc/source/usage/custom.md
+-rw-r--r--   0        0        0      979 2024-04-04 00:12:21.863655 gepref_text-0.1.5/doc/source/usage/filtering.md
+-rw-r--r--   0        0        0      952 2024-04-04 00:12:21.863655 gepref_text-0.1.5/doc/source/usage/normalization.md
+-rw-r--r--   0        0        0      744 2024-04-04 00:12:21.863655 gepref_text-0.1.5/doc/source/usage/preprocessor.md
+-rw-r--r--   0        0        0     1515 2024-04-04 00:12:21.863655 gepref_text-0.1.5/doc/source/usage/regex.md
+-rw-r--r--   0        0        0     1060 2024-04-04 00:12:21.863655 gepref_text-0.1.5/doc/source/usage/tokenization.md
+-rw-r--r--   0        0        0      651 2024-04-04 00:12:21.863655 gepref_text-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 00:12:21.863655 gepref_text-0.1.5/src/gepref_text/__init__.py
+-rw-r--r--   0        0        0      525 2024-04-04 00:12:21.863655 gepref_text-0.1.5/src/gepref_text/base.py
+-rw-r--r--   0        0        0     2779 2024-04-04 00:12:21.863655 gepref_text-0.1.5/src/gepref_text/filtering.py
+-rw-r--r--   0        0        0     1898 2024-04-04 00:12:21.863655 gepref_text-0.1.5/src/gepref_text/normalization.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:12:21.863655 gepref_text-0.1.5/src/gepref_text/py.typed
+-rw-r--r--   0        0        0     3374 2024-04-04 00:12:21.863655 gepref_text-0.1.5/src/gepref_text/regex_sub.py
+-rw-r--r--   0        0        0     1218 2024-04-04 00:12:21.863655 gepref_text-0.1.5/src/gepref_text/tokenization.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:12:21.863655 gepref_text-0.1.5/stubs/nltk/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-04-04 00:12:21.863655 gepref_text-0.1.5/stubs/nltk/corpus/__init__.pyi
+-rw-r--r--   0        0        0       72 2024-04-04 00:12:21.863655 gepref_text-0.1.5/stubs/nltk/corpus/stopwords.pyi
+-rw-r--r--   0        0        0      149 2024-04-04 00:12:21.863655 gepref_text-0.1.5/stubs/nltk/tokenize.pyi
+-rw-r--r--   0        0        0     1320 2024-04-04 00:12:21.863655 gepref_text-0.1.5/test/test_filtering.py
+-rw-r--r--   0        0        0     1300 2024-04-04 00:12:21.863655 gepref_text-0.1.5/test/test_normalization.py
+-rw-r--r--   0        0        0     2113 2024-04-04 00:12:21.863655 gepref_text-0.1.5/test/test_regex.py
+-rw-r--r--   0        0        0      879 2024-04-04 00:12:21.863655 gepref_text-0.1.5/test/test_tokenization.py
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 gepref_text-0.1.5/PKG-INFO
```

### Comparing `gepref_text-0.1.4/.github/workflows/cd.yml` & `gepref_text-0.1.5/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/LICENSE` & `gepref_text-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/README.md` & `gepref_text-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/Makefile` & `gepref_text-0.1.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/_static/gepref_text.svg` & `gepref_text-0.1.5/doc/source/_static/gepref_text.svg`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/_static/preprocessor.svg` & `gepref_text-0.1.5/doc/source/_static/preprocessor.svg`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/conf.py` & `gepref_text-0.1.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/gepref_text.rst` & `gepref_text-0.1.5/doc/source/gepref_text.rst`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/index.rst` & `gepref_text-0.1.5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/usage.rst` & `gepref_text-0.1.5/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/usage/custom.md` & `gepref_text-0.1.5/doc/source/usage/custom.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/usage/filtering.md` & `gepref_text-0.1.5/doc/source/usage/filtering.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/usage/normalization.md` & `gepref_text-0.1.5/doc/source/usage/normalization.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/usage/preprocessor.md` & `gepref_text-0.1.5/doc/source/usage/preprocessor.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/usage/regex.md` & `gepref_text-0.1.5/doc/source/usage/regex.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/doc/source/usage/tokenization.md` & `gepref_text-0.1.5/doc/source/usage/tokenization.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/pyproject.toml` & `gepref_text-0.1.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gepref_text"
-version = "0.1.4"
+version = "0.1.5"
 description = "GEneral PREprocessing Framework for TEXT (gepref_text)"
 authors = [{name="Juan Lara", email="julara@unal.edu.co"}]
 requires-python = ">3.10"
 dependencies = [
 	"gepref==0.1.1",
 	"unidecode==1.3.8",
 	"nltk==3.8.1",
```

### Comparing `gepref_text-0.1.4/src/gepref_text/base.py` & `gepref_text-0.1.5/src/gepref_text/base.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/src/gepref_text/normalization.py` & `gepref_text-0.1.5/src/gepref_text/normalization.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/src/gepref_text/regex_sub.py` & `gepref_text-0.1.5/src/gepref_text/regex_sub.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/src/gepref_text/tokenization.py` & `gepref_text-0.1.5/src/gepref_text/tokenization.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/test/test_filtering.py` & `gepref_text-0.1.5/test/test_filtering.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import nltk
 import pytest
-from gepref_text.filtering import StopwordFilterStep, TokenLenFilterStep
+from typing import List
+from gepref_text.filtering import (
+        StopwordFilterStep, TokenLenFilterStep, CustomWordFilterStep
+        )
 nltk.download("stopwords")
 
 @pytest.mark.parametrize("text, answer", [
     ("this is a first example of something great", "first example something great"),
     ("i am the man who sold the world", "man sold world"),
     ])
 def test_stopword_filter(text: str, answer: str):
@@ -15,7 +18,15 @@
     ("a bb ccc dddd eeeee ffffff", "ccc dddd eeeee", 3, 5),
     ("a bb ccc dddd eeeee ffffff", "bb ccc dddd", 2, 4),
     ("a bb ccc dddd eeeee ffffff", "a bb ccc dddd eeeee ffffff", 1, 6),
     ])
 def test_tokenlen_filter(text: str, answer: str, min_len: int, max_len: int):
     filter_text = TokenLenFilterStep(min_len=min_len, max_len=max_len)(text)
     assert answer == filter_text
+
+@pytest.mark.parametrize("text, answer, exclude", [
+    ("the text the text is", "the the", ["text", "is"]),
+    ("this is awesome and great", "awesome great", ["this", "is", "and"]),
+    ])
+def test_customword_filter(text: str, answer: str, exclude: List[str]):
+    filter_text = CustomWordFilterStep(exclude=exclude)(text)
+    assert answer == filter_text
```

### Comparing `gepref_text-0.1.4/test/test_normalization.py` & `gepref_text-0.1.5/test/test_normalization.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/test/test_regex.py` & `gepref_text-0.1.5/test/test_regex.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/test/test_tokenization.py` & `gepref_text-0.1.5/test/test_tokenization.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.4/PKG-INFO` & `gepref_text-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gepref_text
-Version: 0.1.4
+Version: 0.1.5
 Summary: GEneral PREprocessing Framework for TEXT (gepref_text)
 Author-email: Juan Lara <julara@unal.edu.co>
 Requires-Python: >3.10
 Requires-Dist: gepref==0.1.1
 Requires-Dist: unidecode==1.3.8
 Requires-Dist: nltk==3.8.1
 Requires-Dist: pydantic==2.6.4
```

