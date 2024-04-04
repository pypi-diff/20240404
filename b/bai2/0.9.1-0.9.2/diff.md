# Comparing `tmp/bai2-0.9.1.tar.gz` & `tmp/bai2-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bai2-0.9.1.tar", last modified: Thu Dec 22 10:07:43 2022, max compression
+gzip compressed data, was "bai2-0.9.2.tar", last modified: Fri Jan 13 11:47:11 2023, max compression
```

## Comparing `bai2-0.9.1.tar` & `bai2-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:43.527955 bai2-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2022-12-22 10:07:29.000000 bai2-0.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-22 10:07:29.000000 bai2-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2022-12-22 10:07:43.527955 bai2-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2022-12-22 10:07:29.000000 bai2-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:43.527955 bai2-0.9.1/bai2/
--rwxr-xr-x   0 runner    (1001) docker     (123)      118 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/bai2.py
--rw-r--r--   0 runner    (1001) docker     (123)    47846 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14209 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2022-12-22 10:07:29.000000 bai2-0.9.1/bai2/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:43.527955 bai2-0.9.1/bai2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2022-12-22 10:07:43.000000 bai2-0.9.1/bai2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2022-12-22 10:07:43.000000 bai2-0.9.1/bai2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 10:07:43.000000 bai2-0.9.1/bai2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-22 10:07:43.000000 bai2-0.9.1/bai2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-22 10:07:43.531956 bai2-0.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2022-12-22 10:07:29.000000 bai2-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:43.527955 bai2-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:29.000000 bai2-0.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 10:07:43.527955 bai2-0.9.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-22 10:07:29.000000 bai2-0.9.1/tests/data/account_trailer_amount_blank_example.bai2
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-22 10:07:29.000000 bai2-0.9.1/tests/data/citi_example.bai2
--rw-r--r--   0 runner    (1001) docker     (123)      734 2022-12-22 10:07:29.000000 bai2-0.9.1/tests/data/nwb_example.bai2
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2022-12-22 10:07:29.000000 bai2-0.9.1/tests/test_bai2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23649 2022-12-22 10:07:29.000000 bai2-0.9.1/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2022-12-22 10:07:29.000000 bai2-0.9.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15384 2022-12-22 10:07:29.000000 bai2-0.9.1/tests/test_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:47:11.983683 bai2-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-01-13 11:47:02.000000 bai2-0.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-13 11:47:02.000000 bai2-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-01-13 11:47:11.983683 bai2-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-01-13 11:47:02.000000 bai2-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:47:11.983683 bai2-0.9.2/bai2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/bai2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47846 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-01-13 11:47:02.000000 bai2-0.9.2/bai2/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:47:11.983683 bai2-0.9.2/bai2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-01-13 11:47:11.000000 bai2-0.9.2/bai2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-01-13 11:47:11.000000 bai2-0.9.2/bai2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 11:47:11.000000 bai2-0.9.2/bai2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-13 11:47:11.000000 bai2-0.9.2/bai2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-13 11:47:11.983683 bai2-0.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-01-13 11:47:02.000000 bai2-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:47:11.983683 bai2-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 11:47:02.000000 bai2-0.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:47:11.983683 bai2-0.9.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-13 11:47:02.000000 bai2-0.9.2/tests/data/account_trailer_amount_blank_example.bai2
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-13 11:47:02.000000 bai2-0.9.2/tests/data/citi_example.bai2
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-13 11:47:02.000000 bai2-0.9.2/tests/data/nwb_example.bai2
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-01-13 11:47:02.000000 bai2-0.9.2/tests/test_bai2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23649 2023-01-13 11:47:02.000000 bai2-0.9.2/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-01-13 11:47:02.000000 bai2-0.9.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-01-13 11:47:02.000000 bai2-0.9.2/tests/test_writers.py
```

### Comparing `bai2-0.9.1/LICENSE.txt` & `bai2-0.9.2/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (C) 2022 HM Government (Ministry of Justice Digital & Technology)
+Copyright (C) 2023 HM Government (Ministry of Justice Digital & Technology)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bai2-0.9.1/PKG-INFO` & `bai2-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bai2
-Version: 0.9.1
+Version: 0.9.2
 Summary: BAI2 Parser
 Home-page: https://github.com/ministryofjustice/bai2
 Author: Ministry of Justice Digital & Technology
 Author-email: dev@digital.justice.gov.uk
 License: MIT
 Keywords: bai2 bookkeeping cash management balance reporting
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
 License-File: LICENSE.txt
 
 bai2
 ====
 
 Python module for parsing and writing `BAI2`_ files.
 
@@ -33,58 +34,58 @@
 
 Only Python 3.7+ is supported.
 
 
 Installation
 ------------
 
-.. code-block:: bash
+.. code-block:: shell
 
     pip install bai2
 
 
 Usage
 -----
 
 To use bai2 in a project
 
 .. code-block:: python
 
-    >>> from bai2 import bai2
+    from bai2 import bai2
 
-    >>> # parse from a file
-    >>> with open(<file-path>) as f:
-    >>>     bai2_file = bai2.parse_from_file(f)
+    # parse from a file
+    with open(<file-path>) as f:
+        bai2_file = bai2.parse_from_file(f)
 
-    >>> # parse from a string
-    >>> bai2_file = bai2.parse_from_string(<bai2_as_string>)
+    # parse from a string
+    bai2_file = bai2.parse_from_string(<bai2_as_string>)
 
-    >>> # parse from lines
-    >>> bai2_file = bai2.parse_from_lines(<bai2_as_lines>)
+    # parse from lines
+    bai2_file = bai2.parse_from_lines(<bai2_as_lines>)
 
 
 The ``parse_from_*`` methods return a ``bai2.models.Bai2File`` object which can be used to inspect the parsed data.
 
 To write a BAI2 file:
 
 .. code-block:: python
 
-    >>> from bai2 import bai2
-    >>> from bai2 import models
+    from bai2 import bai2
+    from bai2 import models
 
-    >>> bai2_file = models.Bai2File()
-    >>> bai2_file.header.sender_id = 'EGBANK'
+    bai2_file = models.Bai2File()
+    bai2_file.header.sender_id = 'EGBANK'
 
-    >>> bai2_file.children.append(models.Group())
+    bai2_file.children.append(models.Group())
 
-    >>> transactions = [models.TransactionDetail(amount=100)]
-    >>> bai2_file.children[0].children.append(models.Account(children=transactions))
+    transactions = [models.TransactionDetail(amount=100)]
+    bai2_file.children[0].children.append(models.Account(children=transactions))
 
-    >>> # write to string
-    >>> output = bai2.write(bai2_file)
+    # write to string
+    output = bai2.write(bai2_file)
 
 
 Models
 ------
 
 Models structure::
 
@@ -144,14 +145,17 @@
 Alternatively, run ``python setup.py sdist bdist_wheel upload`` locally.
 Remember to update `History`_.
 
 
 History
 -------
 
+0.9.2 (2023-01-13)
+    Maintenance release, no library changes
+
 0.9.1 (2022-12-22)
     Add support for 829 ‘SEPA Payments’ type code (thanks @podj)
 
 0.9.0 (2022-12-21)
     More lenient parsing where integers are expected (thanks @daniel-butler)
     Add support for 827 & 828 ‘SEPA Payments’ type codes (thanks @podj)
     Remove testing for python versions below 3.7 (the library is still likely to work with 3.6)
@@ -177,13 +181,13 @@
 0.1.0 (2015-08-06)
     Original release
 
 
 Copyright
 ---------
 
-Copyright (C) 2022 HM Government (Ministry of Justice Digital & Technology).
+Copyright (C) 2023 HM Government (Ministry of Justice Digital & Technology).
 See LICENSE.txt for further details.
 
 .. _BAI2: https://www.bai.org/docs/default-source/libraries/site-general-downloads/cash_management_2005.pdf
 .. _GitHub: https://github.com/ministryofjustice/bai2
 .. _PyPi: https://pypi.org/project/bai2/
```

### Comparing `bai2-0.9.1/README.rst` & `bai2-0.9.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,58 +11,58 @@
 
 Only Python 3.7+ is supported.
 
 
 Installation
 ------------
 
-.. code-block:: bash
+.. code-block:: shell
 
     pip install bai2
 
 
 Usage
 -----
 
 To use bai2 in a project
 
 .. code-block:: python
 
-    >>> from bai2 import bai2
+    from bai2 import bai2
 
-    >>> # parse from a file
-    >>> with open(<file-path>) as f:
-    >>>     bai2_file = bai2.parse_from_file(f)
+    # parse from a file
+    with open(<file-path>) as f:
+        bai2_file = bai2.parse_from_file(f)
 
-    >>> # parse from a string
-    >>> bai2_file = bai2.parse_from_string(<bai2_as_string>)
+    # parse from a string
+    bai2_file = bai2.parse_from_string(<bai2_as_string>)
 
-    >>> # parse from lines
-    >>> bai2_file = bai2.parse_from_lines(<bai2_as_lines>)
+    # parse from lines
+    bai2_file = bai2.parse_from_lines(<bai2_as_lines>)
 
 
 The ``parse_from_*`` methods return a ``bai2.models.Bai2File`` object which can be used to inspect the parsed data.
 
 To write a BAI2 file:
 
 .. code-block:: python
 
-    >>> from bai2 import bai2
-    >>> from bai2 import models
+    from bai2 import bai2
+    from bai2 import models
 
-    >>> bai2_file = models.Bai2File()
-    >>> bai2_file.header.sender_id = 'EGBANK'
+    bai2_file = models.Bai2File()
+    bai2_file.header.sender_id = 'EGBANK'
 
-    >>> bai2_file.children.append(models.Group())
+    bai2_file.children.append(models.Group())
 
-    >>> transactions = [models.TransactionDetail(amount=100)]
-    >>> bai2_file.children[0].children.append(models.Account(children=transactions))
+    transactions = [models.TransactionDetail(amount=100)]
+    bai2_file.children[0].children.append(models.Account(children=transactions))
 
-    >>> # write to string
-    >>> output = bai2.write(bai2_file)
+    # write to string
+    output = bai2.write(bai2_file)
 
 
 Models
 ------
 
 Models structure::
 
@@ -122,14 +122,17 @@
 Alternatively, run ``python setup.py sdist bdist_wheel upload`` locally.
 Remember to update `History`_.
 
 
 History
 -------
 
+0.9.2 (2023-01-13)
+    Maintenance release, no library changes
+
 0.9.1 (2022-12-22)
     Add support for 829 ‘SEPA Payments’ type code (thanks @podj)
 
 0.9.0 (2022-12-21)
     More lenient parsing where integers are expected (thanks @daniel-butler)
     Add support for 827 & 828 ‘SEPA Payments’ type codes (thanks @podj)
     Remove testing for python versions below 3.7 (the library is still likely to work with 3.6)
@@ -155,13 +158,13 @@
 0.1.0 (2015-08-06)
     Original release
 
 
 Copyright
 ---------
 
-Copyright (C) 2022 HM Government (Ministry of Justice Digital & Technology).
+Copyright (C) 2023 HM Government (Ministry of Justice Digital & Technology).
 See LICENSE.txt for further details.
 
 .. _BAI2: https://www.bai.org/docs/default-source/libraries/site-general-downloads/cash_management_2005.pdf
 .. _GitHub: https://github.com/ministryofjustice/bai2
 .. _PyPi: https://pypi.org/project/bai2/
```

### Comparing `bai2-0.9.1/bai2/bai2.py` & `bai2-0.9.2/bai2/bai2.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/bai2/constants.py` & `bai2-0.9.2/bai2/constants.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/bai2/helpers.py` & `bai2-0.9.2/bai2/helpers.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/bai2/models.py` & `bai2-0.9.2/bai2/models.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/bai2/parsers.py` & `bai2-0.9.2/bai2/parsers.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/bai2/utils.py` & `bai2-0.9.2/bai2/utils.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/bai2/writers.py` & `bai2-0.9.2/bai2/writers.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/bai2.egg-info/PKG-INFO` & `bai2-0.9.2/bai2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bai2
-Version: 0.9.1
+Version: 0.9.2
 Summary: BAI2 Parser
 Home-page: https://github.com/ministryofjustice/bai2
 Author: Ministry of Justice Digital & Technology
 Author-email: dev@digital.justice.gov.uk
 License: MIT
 Keywords: bai2 bookkeeping cash management balance reporting
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
 License-File: LICENSE.txt
 
 bai2
 ====
 
 Python module for parsing and writing `BAI2`_ files.
 
@@ -33,58 +34,58 @@
 
 Only Python 3.7+ is supported.
 
 
 Installation
 ------------
 
-.. code-block:: bash
+.. code-block:: shell
 
     pip install bai2
 
 
 Usage
 -----
 
 To use bai2 in a project
 
 .. code-block:: python
 
-    >>> from bai2 import bai2
+    from bai2 import bai2
 
-    >>> # parse from a file
-    >>> with open(<file-path>) as f:
-    >>>     bai2_file = bai2.parse_from_file(f)
+    # parse from a file
+    with open(<file-path>) as f:
+        bai2_file = bai2.parse_from_file(f)
 
-    >>> # parse from a string
-    >>> bai2_file = bai2.parse_from_string(<bai2_as_string>)
+    # parse from a string
+    bai2_file = bai2.parse_from_string(<bai2_as_string>)
 
-    >>> # parse from lines
-    >>> bai2_file = bai2.parse_from_lines(<bai2_as_lines>)
+    # parse from lines
+    bai2_file = bai2.parse_from_lines(<bai2_as_lines>)
 
 
 The ``parse_from_*`` methods return a ``bai2.models.Bai2File`` object which can be used to inspect the parsed data.
 
 To write a BAI2 file:
 
 .. code-block:: python
 
-    >>> from bai2 import bai2
-    >>> from bai2 import models
+    from bai2 import bai2
+    from bai2 import models
 
-    >>> bai2_file = models.Bai2File()
-    >>> bai2_file.header.sender_id = 'EGBANK'
+    bai2_file = models.Bai2File()
+    bai2_file.header.sender_id = 'EGBANK'
 
-    >>> bai2_file.children.append(models.Group())
+    bai2_file.children.append(models.Group())
 
-    >>> transactions = [models.TransactionDetail(amount=100)]
-    >>> bai2_file.children[0].children.append(models.Account(children=transactions))
+    transactions = [models.TransactionDetail(amount=100)]
+    bai2_file.children[0].children.append(models.Account(children=transactions))
 
-    >>> # write to string
-    >>> output = bai2.write(bai2_file)
+    # write to string
+    output = bai2.write(bai2_file)
 
 
 Models
 ------
 
 Models structure::
 
@@ -144,14 +145,17 @@
 Alternatively, run ``python setup.py sdist bdist_wheel upload`` locally.
 Remember to update `History`_.
 
 
 History
 -------
 
+0.9.2 (2023-01-13)
+    Maintenance release, no library changes
+
 0.9.1 (2022-12-22)
     Add support for 829 ‘SEPA Payments’ type code (thanks @podj)
 
 0.9.0 (2022-12-21)
     More lenient parsing where integers are expected (thanks @daniel-butler)
     Add support for 827 & 828 ‘SEPA Payments’ type codes (thanks @podj)
     Remove testing for python versions below 3.7 (the library is still likely to work with 3.6)
@@ -177,13 +181,13 @@
 0.1.0 (2015-08-06)
     Original release
 
 
 Copyright
 ---------
 
-Copyright (C) 2022 HM Government (Ministry of Justice Digital & Technology).
+Copyright (C) 2023 HM Government (Ministry of Justice Digital & Technology).
 See LICENSE.txt for further details.
 
 .. _BAI2: https://www.bai.org/docs/default-source/libraries/site-general-downloads/cash_management_2005.pdf
 .. _GitHub: https://github.com/ministryofjustice/bai2
 .. _PyPi: https://pypi.org/project/bai2/
```

### Comparing `bai2-0.9.1/bai2.egg-info/SOURCES.txt` & `bai2-0.9.2/bai2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/setup.py` & `bai2-0.9.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,11 +41,12 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
+    python_requires='>=3.6',  # looser requirement than what's tested
     install_requires=install_requires,
     tests_require=tests_require,
     test_suite='tests',
 )
```

### Comparing `bai2-0.9.1/tests/data/nwb_example.bai2` & `bai2-0.9.2/tests/data/nwb_example.bai2`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/tests/test_bai2.py` & `bai2-0.9.2/tests/test_bai2.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/tests/test_parsers.py` & `bai2-0.9.2/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/tests/test_utils.py` & `bai2-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bai2-0.9.1/tests/test_writers.py` & `bai2-0.9.2/tests/test_writers.py`

 * *Files identical despite different names*

