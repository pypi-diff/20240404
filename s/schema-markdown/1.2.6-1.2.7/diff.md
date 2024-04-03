# Comparing `tmp/schema-markdown-1.2.6.tar.gz` & `tmp/schema-markdown-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-markdown-1.2.6.tar", last modified: Wed Jun 28 14:43:46 2023, max compression
+gzip compressed data, was "schema-markdown-1.2.7.tar", last modified: Wed Apr  3 22:46:50 2024, max compression
```

## Comparing `schema-markdown-1.2.6.tar` & `schema-markdown-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-06-28 14:43:46.566714 schema-markdown-1.2.6/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     4709 2023-06-28 14:43:46.566763 schema-markdown-1.2.6/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     3895 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/README.rst
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)      833 2023-06-28 14:43:46.566977 schema-markdown-1.2.6/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-06-28 14:43:46.565076 schema-markdown-1.2.6/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-06-28 14:43:46.566200 schema-markdown-1.2.6/src/schema_markdown/
--rw-r--r--   0 craighobbs   (501) staff       (20)      578 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/src/schema_markdown/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     6222 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/src/schema_markdown/encode.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    18551 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/src/schema_markdown/parser.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    19055 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/src/schema_markdown/schema.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    11083 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/src/schema_markdown/schema_util.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     4370 2023-06-28 14:21:25.000000 schema-markdown-1.2.6/src/schema_markdown/type_model.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2023-06-28 14:43:46.566623 schema-markdown-1.2.6/src/schema_markdown.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     4709 2023-06-28 14:43:46.000000 schema-markdown-1.2.6/src/schema_markdown.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      406 2023-06-28 14:43:46.000000 schema-markdown-1.2.6/src/schema_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2023-06-28 14:43:46.000000 schema-markdown-1.2.6/src/schema_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       16 2023-06-28 14:43:46.000000 schema-markdown-1.2.6/src/schema_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 22:46:50.130148 schema-markdown-1.2.7/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-04-02 16:27:19.000000 schema-markdown-1.2.7/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     4286 2024-04-03 22:46:50.130089 schema-markdown-1.2.7/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3469 2024-04-03 22:35:36.000000 schema-markdown-1.2.7/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-04-02 16:27:19.000000 schema-markdown-1.2.7/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)      835 2024-04-03 22:46:50.130438 schema-markdown-1.2.7/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 22:46:50.127981 schema-markdown-1.2.7/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 22:46:50.129276 schema-markdown-1.2.7/src/schema_markdown/
+-rw-r--r--   0 craighobbs   (501) staff       (20)      578 2024-04-02 16:27:19.000000 schema-markdown-1.2.7/src/schema_markdown/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     6222 2024-04-02 16:27:19.000000 schema-markdown-1.2.7/src/schema_markdown/encode.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    18551 2024-04-02 16:27:19.000000 schema-markdown-1.2.7/src/schema_markdown/parser.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    19055 2024-04-02 16:27:19.000000 schema-markdown-1.2.7/src/schema_markdown/schema.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    11083 2024-04-02 16:27:19.000000 schema-markdown-1.2.7/src/schema_markdown/schema_util.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     4370 2024-04-02 16:27:19.000000 schema-markdown-1.2.7/src/schema_markdown/type_model.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 22:46:50.129901 schema-markdown-1.2.7/src/schema_markdown.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     4286 2024-04-03 22:46:50.000000 schema-markdown-1.2.7/src/schema_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      405 2024-04-03 22:46:50.000000 schema-markdown-1.2.7/src/schema_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-04-03 22:46:50.000000 schema-markdown-1.2.7/src/schema_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       16 2024-04-03 22:46:50.000000 schema-markdown-1.2.7/src/schema_markdown.egg-info/top_level.txt
```

### Comparing `schema-markdown-1.2.6/LICENSE` & `schema-markdown-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-markdown-1.2.6/PKG-INFO` & `schema-markdown-1.2.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-markdown
-Version: 1.2.6
+Version: 1.2.7
 Summary: A schema definition and validation library
 Home-page: https://github.com/craigahobbs/schema-markdown
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: schema,validate,json
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,133 +13,125 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-schema-markdown
-===============
+# schema-markdown
 
-.. |badge-status| image:: https://img.shields.io/pypi/status/schema-markdown
-   :alt: PyPI - Status
-   :target: https://pypi.python.org/pypi/schema-markdown/
-
-.. |badge-version| image:: https://img.shields.io/pypi/v/schema-markdown
-   :alt: PyPI
-   :target: https://pypi.python.org/pypi/schema-markdown/
-
-.. |badge-license| image:: https://img.shields.io/github/license/craigahobbs/schema-markdown
-   :alt: GitHub
-   :target: https://github.com/craigahobbs/schema-markdown/blob/main/LICENSE
-
-.. |badge-python| image:: https://img.shields.io/pypi/pyversions/schema-markdown
-   :alt: PyPI - Python Version
-   :target: https://www.python.org/downloads/
-
-|badge-status| |badge-version| |badge-license| |badge-python|
+[![PyPI - Status](https://img.shields.io/pypi/status/schema-markdown)](https://pypi.org/project/schema-markdown/)
+[![PyPI](https://img.shields.io/pypi/v/schema-markdown)](https://pypi.org/project/schema-markdown/)
+[![GitHub](https://img.shields.io/github/license/craigahobbs/schema-markdown)](https://github.com/craigahobbs/schema-markdown/blob/main/LICENSE)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/schema-markdown)](https://pypi.org/project/schema-markdown/)
 
 schema-markdown is a schema definition and validation library.
 
 
-Links
------
+## Links
 
-- `The Schema Markdown Language <https://craigahobbs.github.io/schema-markdown-js/language/>`__
-- `API Documentation <https://craigahobbs.github.io/schema-markdown/>`__
-- `Source code <https://github.com/craigahobbs/schema-markdown>`__
+- [The Schema Markdown Language](https://craigahobbs.github.io/schema-markdown-js/language/)
+- [API Documentation](https://craigahobbs.github.io/schema-markdown/)
+- [Source code](https://github.com/craigahobbs/schema-markdown)
 
 
-Define a Schema
----------------
+## Define a Schema
 
 Schemas are defined using the
-`Schema Markdown language <https://craigahobbs.github.io/schema-markdown-js/language/>`__,
+[Schema Markdown language](https://craigahobbs.github.io/schema-markdown-js/language/),
 which is parsed by the
-`parse_schema_markdown <https://craigahobbs.github.io/schema-markdown/reference.html#parse-schema-markdown>`__
+[parse_schema_markdown](https://craigahobbs.github.io/schema-markdown/reference.html#parse-schema-markdown)
 function. For example:
 
->>> from schema_markdown import parse_schema_markdown
-...
->>> model_types = parse_schema_markdown('''\
-... # An aggregate numerical operation
-... struct Aggregation
-...
-...     # The aggregation function - default is "Sum"
-...     optional AggregationFunction aggregation
-...
-...     # The numbers to aggregate on
-...     int[len > 0] numbers
-...
-... # An aggregation function
-... enum AggregationFunction
-...     Average
-...     Sum
-... ''')
+~~~ python
+from schema_markdown import parse_schema_markdown
+
+model_types = parse_schema_markdown('''\
+# An aggregate numerical operation
+struct Aggregation
+
+    # The aggregation function - default is "Sum"
+    optional AggregationFunction aggregation
+
+    # The numbers to aggregate on
+    int[len > 0] numbers
 
+# An aggregation function
+enum AggregationFunction
+    Average
+    Sum
+''')
+~~~
 
-Validate using a Schema
------------------------
+
+## Validate using a Schema
 
 To validate an object using the schema, use the
-`validate_type <https://craigahobbs.github.io/schema-markdown/reference.html#validate-type>`__
+[validate_type](https://craigahobbs.github.io/schema-markdown/reference.html#validate-type)
 function. For example:
 
->>> from schema_markdown import validate_type
-...
->>> validate_type(model_types, 'Aggregation', {'numbers': [1, 2, '3', 4]})
+~~~ python
+from schema_markdown import validate_type
+
+validate_type(model_types, 'Aggregation', {'numbers': [1, 2, '3', 4]})
+
 {'numbers': [1, 2, 3, 4]}
+~~~
 
 Notice that the numerical input '3' above is *type-massaged* to the integer 3 by validation.
 
 Validation fails if the object does not match the schema:
 
->>> from schema_markdown import ValidationError
-...
->>> try:
-...     validate_type(model_types, 'Aggregation', {'numbers': [1, 2, 'asdf', 4]})
-... except ValidationError as exc:
-...     str(exc)
+~~~ python
+from schema_markdown import ValidationError
+
+try:
+    validate_type(model_types, 'Aggregation', {'numbers': [1, 2, 'asdf', 4]})
+except ValidationError as exc:
+    str(exc)
+
 "Invalid value 'asdf' (type 'str') for member 'numbers.2', expected type 'int'"
+~~~
 
 Validation also fails if a member constraint is violated:
 
->>> try:
-...     validate_type(model_types, 'Aggregation', {'numbers': []})
-... except ValidationError as exc:
-...     str(exc)
+~~~ python
+try:
+    validate_type(model_types, 'Aggregation', {'numbers': []})
+except ValidationError as exc:
+    str(exc)
+
 "Invalid value [] (type 'list') for member 'numbers', expected type 'array' [len > 0]"
+~~~
 
 
-Document a Schema
------------------
+## Document a Schema
 
 To document the schema, download the
-`documentation application <https://github.com/craigahobbs/schema-markdown-doc#the-schema-markdown-documentation-viewer>`__
+[documentation application](https://github.com/craigahobbs/schema-markdown-doc#the-schema-markdown-documentation-viewer)
 stub and save the type model as JSON:
 
-.. code-block:: sh
-
-   curl -O https://craigahobbs.github.io/schema-markdown-doc/extra/index.html
-   python3 \
-       -c 'from model import model_types; import json; print(json.dumps(model_types))' \
-       > model.json
+~~~ sh
+curl -O https://craigahobbs.github.io/schema-markdown-doc/extra/index.html
+python3 \
+    -c 'from model import model_types; import json; print(json.dumps(model_types))' \
+    > model.json
+~~~
 
 To host locally, start a local static web server:
 
-.. code-block:: sh
-
-   python3 -m http.server
-
+~~~ sh
+python3 -m http.server
+~~~
 
-Development
------------
 
-This package is developed using `python-build <https://github.com/craigahobbs/python-build#readme>`__.
-It was started using `python-template <https://github.com/craigahobbs/python-template#readme>`__ as follows:
+## Development
 
-.. code-block:: sh
+This package is developed using [python-build](https://github.com/craigahobbs/python-build#readme).
+It was started using [python-template](https://github.com/craigahobbs/python-template#readme) as follows:
 
-   template-specialize python-template/template/ schema-markdown/ -k package schema-markdown -k name 'Craig A. Hobbs' -k email 'craigahobbs@gmail.com' -k github 'craigahobbs' -k nomain 1
+~~~ sh
+template-specialize python-template/template/ schema-markdown/ -k package schema-markdown -k name 'Craig A. Hobbs' -k email 'craigahobbs@gmail.com' -k github 'craigahobbs' -k nomain 1
+~~~
```

### Comparing `schema-markdown-1.2.6/setup.cfg` & `schema-markdown-1.2.7/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = schema-markdown
-version = 1.2.6
+version = 1.2.7
 url = https://github.com/craigahobbs/schema-markdown
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = A schema definition and validation library
-long_description = file:README.rst
-long_description_content_type = text/x-rst
+long_description = file:README.md
+long_description_content_type = text/markdown
 keywords = schema, validate, json
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.8
```

### Comparing `schema-markdown-1.2.6/src/schema_markdown/__init__.py` & `schema-markdown-1.2.7/src/schema_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-markdown-1.2.6/src/schema_markdown/encode.py` & `schema-markdown-1.2.7/src/schema_markdown/encode.py`

 * *Files identical despite different names*

### Comparing `schema-markdown-1.2.6/src/schema_markdown/parser.py` & `schema-markdown-1.2.7/src/schema_markdown/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Licensed under the MIT License
-# https://github.com/craigahobbs/schema_markdown/blob/main/LICENSE
+# https://github.com/craigahobbs/schema-markdown/blob/main/LICENSE
 
 """
 Schema Markdown parser
 """
 
 from itertools import chain
 import re
```

### Comparing `schema-markdown-1.2.6/src/schema_markdown/schema.py` & `schema-markdown-1.2.7/src/schema_markdown/schema.py`

 * *Files identical despite different names*

### Comparing `schema-markdown-1.2.6/src/schema_markdown/schema_util.py` & `schema-markdown-1.2.7/src/schema_markdown/schema_util.py`

 * *Files identical despite different names*

### Comparing `schema-markdown-1.2.6/src/schema_markdown/type_model.py` & `schema-markdown-1.2.7/src/schema_markdown/type_model.py`

 * *Files identical despite different names*

### Comparing `schema-markdown-1.2.6/src/schema_markdown.egg-info/PKG-INFO` & `schema-markdown-1.2.7/src/schema_markdown.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-markdown
-Version: 1.2.6
+Version: 1.2.7
 Summary: A schema definition and validation library
 Home-page: https://github.com/craigahobbs/schema-markdown
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: schema,validate,json
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,133 +13,125 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-schema-markdown
-===============
+# schema-markdown
 
-.. |badge-status| image:: https://img.shields.io/pypi/status/schema-markdown
-   :alt: PyPI - Status
-   :target: https://pypi.python.org/pypi/schema-markdown/
-
-.. |badge-version| image:: https://img.shields.io/pypi/v/schema-markdown
-   :alt: PyPI
-   :target: https://pypi.python.org/pypi/schema-markdown/
-
-.. |badge-license| image:: https://img.shields.io/github/license/craigahobbs/schema-markdown
-   :alt: GitHub
-   :target: https://github.com/craigahobbs/schema-markdown/blob/main/LICENSE
-
-.. |badge-python| image:: https://img.shields.io/pypi/pyversions/schema-markdown
-   :alt: PyPI - Python Version
-   :target: https://www.python.org/downloads/
-
-|badge-status| |badge-version| |badge-license| |badge-python|
+[![PyPI - Status](https://img.shields.io/pypi/status/schema-markdown)](https://pypi.org/project/schema-markdown/)
+[![PyPI](https://img.shields.io/pypi/v/schema-markdown)](https://pypi.org/project/schema-markdown/)
+[![GitHub](https://img.shields.io/github/license/craigahobbs/schema-markdown)](https://github.com/craigahobbs/schema-markdown/blob/main/LICENSE)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/schema-markdown)](https://pypi.org/project/schema-markdown/)
 
 schema-markdown is a schema definition and validation library.
 
 
-Links
------
+## Links
 
-- `The Schema Markdown Language <https://craigahobbs.github.io/schema-markdown-js/language/>`__
-- `API Documentation <https://craigahobbs.github.io/schema-markdown/>`__
-- `Source code <https://github.com/craigahobbs/schema-markdown>`__
+- [The Schema Markdown Language](https://craigahobbs.github.io/schema-markdown-js/language/)
+- [API Documentation](https://craigahobbs.github.io/schema-markdown/)
+- [Source code](https://github.com/craigahobbs/schema-markdown)
 
 
-Define a Schema
----------------
+## Define a Schema
 
 Schemas are defined using the
-`Schema Markdown language <https://craigahobbs.github.io/schema-markdown-js/language/>`__,
+[Schema Markdown language](https://craigahobbs.github.io/schema-markdown-js/language/),
 which is parsed by the
-`parse_schema_markdown <https://craigahobbs.github.io/schema-markdown/reference.html#parse-schema-markdown>`__
+[parse_schema_markdown](https://craigahobbs.github.io/schema-markdown/reference.html#parse-schema-markdown)
 function. For example:
 
->>> from schema_markdown import parse_schema_markdown
-...
->>> model_types = parse_schema_markdown('''\
-... # An aggregate numerical operation
-... struct Aggregation
-...
-...     # The aggregation function - default is "Sum"
-...     optional AggregationFunction aggregation
-...
-...     # The numbers to aggregate on
-...     int[len > 0] numbers
-...
-... # An aggregation function
-... enum AggregationFunction
-...     Average
-...     Sum
-... ''')
+~~~ python
+from schema_markdown import parse_schema_markdown
+
+model_types = parse_schema_markdown('''\
+# An aggregate numerical operation
+struct Aggregation
+
+    # The aggregation function - default is "Sum"
+    optional AggregationFunction aggregation
+
+    # The numbers to aggregate on
+    int[len > 0] numbers
 
+# An aggregation function
+enum AggregationFunction
+    Average
+    Sum
+''')
+~~~
 
-Validate using a Schema
------------------------
+
+## Validate using a Schema
 
 To validate an object using the schema, use the
-`validate_type <https://craigahobbs.github.io/schema-markdown/reference.html#validate-type>`__
+[validate_type](https://craigahobbs.github.io/schema-markdown/reference.html#validate-type)
 function. For example:
 
->>> from schema_markdown import validate_type
-...
->>> validate_type(model_types, 'Aggregation', {'numbers': [1, 2, '3', 4]})
+~~~ python
+from schema_markdown import validate_type
+
+validate_type(model_types, 'Aggregation', {'numbers': [1, 2, '3', 4]})
+
 {'numbers': [1, 2, 3, 4]}
+~~~
 
 Notice that the numerical input '3' above is *type-massaged* to the integer 3 by validation.
 
 Validation fails if the object does not match the schema:
 
->>> from schema_markdown import ValidationError
-...
->>> try:
-...     validate_type(model_types, 'Aggregation', {'numbers': [1, 2, 'asdf', 4]})
-... except ValidationError as exc:
-...     str(exc)
+~~~ python
+from schema_markdown import ValidationError
+
+try:
+    validate_type(model_types, 'Aggregation', {'numbers': [1, 2, 'asdf', 4]})
+except ValidationError as exc:
+    str(exc)
+
 "Invalid value 'asdf' (type 'str') for member 'numbers.2', expected type 'int'"
+~~~
 
 Validation also fails if a member constraint is violated:
 
->>> try:
-...     validate_type(model_types, 'Aggregation', {'numbers': []})
-... except ValidationError as exc:
-...     str(exc)
+~~~ python
+try:
+    validate_type(model_types, 'Aggregation', {'numbers': []})
+except ValidationError as exc:
+    str(exc)
+
 "Invalid value [] (type 'list') for member 'numbers', expected type 'array' [len > 0]"
+~~~
 
 
-Document a Schema
------------------
+## Document a Schema
 
 To document the schema, download the
-`documentation application <https://github.com/craigahobbs/schema-markdown-doc#the-schema-markdown-documentation-viewer>`__
+[documentation application](https://github.com/craigahobbs/schema-markdown-doc#the-schema-markdown-documentation-viewer)
 stub and save the type model as JSON:
 
-.. code-block:: sh
-
-   curl -O https://craigahobbs.github.io/schema-markdown-doc/extra/index.html
-   python3 \
-       -c 'from model import model_types; import json; print(json.dumps(model_types))' \
-       > model.json
+~~~ sh
+curl -O https://craigahobbs.github.io/schema-markdown-doc/extra/index.html
+python3 \
+    -c 'from model import model_types; import json; print(json.dumps(model_types))' \
+    > model.json
+~~~
 
 To host locally, start a local static web server:
 
-.. code-block:: sh
-
-   python3 -m http.server
-
+~~~ sh
+python3 -m http.server
+~~~
 
-Development
------------
 
-This package is developed using `python-build <https://github.com/craigahobbs/python-build#readme>`__.
-It was started using `python-template <https://github.com/craigahobbs/python-template#readme>`__ as follows:
+## Development
 
-.. code-block:: sh
+This package is developed using [python-build](https://github.com/craigahobbs/python-build#readme).
+It was started using [python-template](https://github.com/craigahobbs/python-template#readme) as follows:
 
-   template-specialize python-template/template/ schema-markdown/ -k package schema-markdown -k name 'Craig A. Hobbs' -k email 'craigahobbs@gmail.com' -k github 'craigahobbs' -k nomain 1
+~~~ sh
+template-specialize python-template/template/ schema-markdown/ -k package schema-markdown -k name 'Craig A. Hobbs' -k email 'craigahobbs@gmail.com' -k github 'craigahobbs' -k nomain 1
+~~~
```

