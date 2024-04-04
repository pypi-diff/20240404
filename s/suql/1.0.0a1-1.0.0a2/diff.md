# Comparing `tmp/suql-1.0.0a1.tar.gz` & `tmp/suql-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.0.0a1.tar", last modified: Wed Apr  3 06:04:47 2024, max compression
+gzip compressed data, was "suql-1.0.0a2.tar", last modified: Thu Apr  4 04:30:18 2024, max compression
```

## Comparing `suql-1.0.0a1.tar` & `suql-1.0.0a2.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-03 06:04:47.165458 suql-1.0.0a1/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.0.0a1/LICENSE
--rw-------   0 oval      (1000) users      (100)     4619 2024-04-03 06:04:47.165458 suql-1.0.0a1/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4165 2024-04-03 06:02:31.000000 suql-1.0.0a1/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-03 06:04:47.165458 suql-1.0.0a1/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1395 2024-04-03 06:04:37.000000 suql-1.0.0a1/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-03 06:04:47.165458 suql-1.0.0a1/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-03 06:04:47.165458 suql-1.0.0a1/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.0.0a1/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17330 2024-04-03 06:02:28.000000 suql-1.0.0a1/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16991 2024-04-03 06:02:28.000000 suql-1.0.0a1/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     7885 2024-04-03 06:02:28.000000 suql-1.0.0a1/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.0.0a1/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)    11962 2024-04-03 06:02:28.000000 suql-1.0.0a1/src/suql/prompt_continuation.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.0.0a1/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-03 06:04:47.165458 suql-1.0.0a1/src/suql.egg-info/
--rw-------   0 oval      (1000) users      (100)     4619 2024-04-03 06:04:47.000000 suql-1.0.0a1/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      370 2024-04-03 06:04:47.000000 suql-1.0.0a1/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-03 06:04:47.000000 suql-1.0.0a1/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      232 2024-04-03 06:04:47.000000 suql-1.0.0a1/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-03 06:04:47.000000 suql-1.0.0a1/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.642725 suql-1.0.0a2/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.0.0a2/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4619 2024-04-04 04:30:18.642725 suql-1.0.0a2/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4165 2024-04-03 06:02:31.000000 suql-1.0.0a2/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-04 04:30:18.642725 suql-1.0.0a2/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1395 2024-04-04 04:29:28.000000 suql-1.0.0a2/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17330 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    16991 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     7885 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)    11962 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.0.0a2/src/suql/prompts/__init__.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.0.0a2/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    59411 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.0.0a2/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-04 04:30:18.638725 suql-1.0.0a2/src/suql.egg-info/
+-rw-------   0 oval      (1000) users      (100)     4619 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      498 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      232 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-04 04:30:18.000000 suql-1.0.0a2/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.0.0a1/LICENSE` & `suql-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a1/PKG-INFO` & `suql-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.0.0a1 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.0.0a2 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
            ************ SSUUQQLL ((SSttrruuccttuurreedd aanndd UUnnssttrruuccttuurreedd QQuueerryy LLaanngguuaaggee))
                          _[[_aa_rr_XX_ii_vv_]]_[[_GG_ii_tt_hh_uu_bb_ _SS_tt_aa_rr_ss_]] ************
```

### Comparing `suql-1.0.0a1/README.md` & `suql-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a1/setup.py` & `suql-1.0.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.0.0a1"
+version = "1.0.0a2"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.0.0a1/src/suql/agent.py` & `suql-1.0.0a2/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a1/src/suql/faiss_embedding.py` & `suql-1.0.0a2/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a1/src/suql/free_text_fcns_server.py` & `suql-1.0.0a2/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a1/src/suql/postgresql_connection.py` & `suql-1.0.0a2/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a1/src/suql/prompt_continuation.py` & `suql-1.0.0a2/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a1/src/suql/utils.py` & `suql-1.0.0a2/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.0.0a1/src/suql.egg-info/PKG-INFO` & `suql-1.0.0a2/src/suql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.0.0a1 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.0.0a2 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
            ************ SSUUQQLL ((SSttrruuccttuurreedd aanndd UUnnssttrruuccttuurreedd QQuueerryy LLaanngguuaaggee))
                          _[[_aa_rr_XX_ii_vv_]]_[[_GG_ii_tt_hh_uu_bb_ _SS_tt_aa_rr_ss_]] ************
```

