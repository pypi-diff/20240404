# Comparing `tmp/py_serializable-1.0.1.tar.gz` & `tmp/py_serializable-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_serializable-1.0.1.tar", max compression
+gzip compressed data, was "py_serializable-1.0.2.tar", max compression
```

## Comparing `py_serializable-1.0.1.tar` & `py_serializable-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,51 @@
--rw-r--r--   0        0        0    11357 2024-02-13 23:23:42.484804 py_serializable-1.0.1/LICENSE
--rw-r--r--   0        0        0     2900 2024-02-13 23:23:42.484804 py_serializable-1.0.1/README.md
--rw-r--r--   0        0        0     3064 2024-02-13 23:24:01.360770 py_serializable-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    57105 2024-02-13 23:24:01.360770 py_serializable-1.0.1/serializable/__init__.py
--rw-r--r--   0        0        0     3409 2024-02-13 23:23:42.484804 py_serializable-1.0.1/serializable/formatters.py
--rw-r--r--   0        0        0     6859 2024-02-13 23:23:42.484804 py_serializable-1.0.1/serializable/helpers.py
--rw-r--r--   0        0        0      153 2024-02-13 23:23:42.484804 py_serializable-1.0.1/serializable/py.typed
--rw-r--r--   0        0        0     4208 1970-01-01 00:00:00.000000 py_serializable-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    61466 2024-03-01 08:21:03.929464 py_serializable-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-03-01 08:21:03.929464 py_serializable-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2900 2024-03-01 08:21:03.929464 py_serializable-1.0.2/README.md
+-rw-r--r--   0        0        0      634 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0      770 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/changelog.rst
+-rw-r--r--   0        0        0     2492 2024-03-01 08:21:29.317480 py_serializable-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0     8933 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/customising-structure.rst
+-rw-r--r--   0        0        0     1883 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/examples.rst
+-rw-r--r--   0        0        0     2897 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/formatters.rst
+-rw-r--r--   0        0        0     5102 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/getting-started.rst
+-rw-r--r--   0        0        0     1529 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0       82 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0     1440 2024-03-01 08:21:03.929464 py_serializable-1.0.2/docs/support.rst
+-rw-r--r--   0        0        0     3379 2024-03-01 08:21:29.317480 py_serializable-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    57105 2024-03-01 08:21:29.317480 py_serializable-1.0.2/serializable/__init__.py
+-rw-r--r--   0        0        0     3409 2024-03-01 08:21:03.929464 py_serializable-1.0.2/serializable/formatters.py
+-rw-r--r--   0        0        0     6859 2024-03-01 08:21:03.929464 py_serializable-1.0.2/serializable/helpers.py
+-rw-r--r--   0        0        0      153 2024-03-01 08:21:03.929464 py_serializable-1.0.2/serializable/py.typed
+-rw-r--r--   0        0        0      694 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3534 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/base.py
+-rw-r--r--   0        0        0     1025 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-1-v1.xml
+-rw-r--r--   0        0        0     1069 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-1-v2.xml
+-rw-r--r--   0        0        0     1037 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-1-v3.xml
+-rw-r--r--   0        0        0     1361 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-1-v4.xml
+-rw-r--r--   0        0        0     1006 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-1.xml
+-rw-r--r--   0        0        0     1010 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-references.json
+-rw-r--r--   0        0        0      767 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-v2.json
+-rw-r--r--   0        0        0      736 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-v3.json
+-rw-r--r--   0        0        0     1010 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-v4.json
+-rw-r--r--   0        0        0      707 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-with-ignored.json
+-rw-r--r--   0        0        0     1006 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case-with-ignored.xml
+-rw-r--r--   0        0        0      712 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-camel-case.json
+-rw-r--r--   0        0        0     1409 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-defaultNS-isset-v4.xml
+-rw-r--r--   0        0        0      718 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-defaultNS-isset.SNAPSHOT.xml
+-rw-r--r--   0        0        0     1659 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-defaultNS-mixed-v4.xml
+-rw-r--r--   0        0        0     1622 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-defaultNS-unset-v4.xml
+-rw-r--r--   0        0        0      914 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-defaultNS-unset.SNAPSHOT.xml
+-rw-r--r--   0        0        0     1072 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-kebab-case-1-v2.xml
+-rw-r--r--   0        0        0     1009 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-kebab-case-1.xml
+-rw-r--r--   0        0        0      714 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-kebab-case.json
+-rw-r--r--   0        0        0     1009 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-snake-case-1.xml
+-rw-r--r--   0        0        0      714 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/fixtures/the-phoenix-project-snake-case.json
+-rw-r--r--   0        0        0    11337 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/model.py
+-rw-r--r--   0        0        0     3635 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/test_formatters.py
+-rw-r--r--   0        0        0     6164 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/test_helpers.py
+-rw-r--r--   0        0        0     7876 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/test_json.py
+-rw-r--r--   0        0        0     1530 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/test_oml.py
+-rw-r--r--   0        0        0     5784 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/test_oml_serializable_property.py
+-rw-r--r--   0        0        0    13860 2024-03-01 08:21:03.929464 py_serializable-1.0.2/tests/test_xml.py
+-rw-r--r--   0        0        0     4208 1970-01-01 00:00:00.000000 py_serializable-1.0.2/PKG-INFO
```

### Comparing `py_serializable-1.0.1/LICENSE` & `py_serializable-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_serializable-1.0.1/README.md` & `py_serializable-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py_serializable-1.0.1/pyproject.toml` & `py_serializable-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "py-serializable"
-version = "1.0.1"
+version = "1.0.2"
 description = "Library for serializing and deserializing Python Objects to and from JSON and XML."
 authors = ["Paul Horton <paul.horton@owasp.org>"]
 maintainers = [
     "Jan Kowalleck <jan.kowalleck@gmail.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/madpah/serializable#readme"
 repository = "https://github.com/madpah/serializable"
 documentation = "https://py-serializable.readthedocs.io/"
 packages = [
     { include = "serializable" }
 ]
+include = [
+  # all is an object -> prevent parse issue with dependabot
+  { path="README.md", format =["sdist"] },
+  { path="CHANGELOG.md", format=["sdist"] },
+  { path="docs", format=["sdist"] },
+  { path="tests", format=["sdist"] },
+]
+exclude = [
+  # exclude dotfiles and dotfolders
+  "**/.*",
+  "docs/_build",
+]
 classifiers = [
     # Trove classifiers - https://packaging.python.org/specifications/core-metadata/#metadata-classifier
     # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Topic :: Software Development',
@@ -43,24 +55,24 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 defusedxml = "^0.7.1"
 
 [tool.poetry.dev-dependencies]
 tox = "4.11.4"
-coverage = "7.4.1"
+coverage = "7.4.3"
 xmldiff = "2.6.3"
 mypy =  "1.8.0"
 autopep8 = "2.0.4"
 isort = "5.13.2"
 flake8 = { version="7.0.0", python=">=3.8.1" }
 flake8-annotations = { version="3.0.1", python=">=3.8.1" }
 flake8-bugbear = { version="24.2.6", python=">=3.8.1" }
 flake8-isort = "6.1.1"
-flake8-quotes = "3.3.2"
+flake8-quotes = "3.4.0"
 flake8-use-fstring = "1.4"
 flake8-logging = "1.5.0"
 
 
 
 [tool.semantic_release]
 # see https://python-semantic-release.readthedocs.io/en/latest/configuration.html
```

### Comparing `py_serializable-1.0.1/serializable/__init__.py` & `py_serializable-1.0.2/serializable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 from typing import Union as Intersection  # isort: skip
 
 # MUST import the whole thing to get some eval/hacks working for dynamic type detection.
 import typing  # noqa: F401 # isort: skip
 
 # !! version is managed by semantic_release
 # do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 _logger = getLogger(__name__)
 _logger.addHandler(NullHandler())
 # make `logger` publicly available, as stable API
 logger = _logger
 """
 The logger. The thing that captures all this package has to say.
```

### Comparing `py_serializable-1.0.1/serializable/formatters.py` & `py_serializable-1.0.2/serializable/formatters.py`

 * *Files identical despite different names*

### Comparing `py_serializable-1.0.1/serializable/helpers.py` & `py_serializable-1.0.2/serializable/helpers.py`

 * *Files identical despite different names*

### Comparing `py_serializable-1.0.1/PKG-INFO` & `py_serializable-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-serializable
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for serializing and deserializing Python Objects to and from JSON and XML.
 Home-page: https://github.com/madpah/serializable#readme
 License: Apache-2.0
 Keywords: serialization,deserialization,JSON,XML
 Author: Paul Horton
 Author-email: paul.horton@owasp.org
 Maintainer: Jan Kowalleck
```

