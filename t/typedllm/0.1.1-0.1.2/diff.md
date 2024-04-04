# Comparing `tmp/typedllm-0.1.1.tar.gz` & `tmp/typedllm-0.1.2.tar.gz`

## Comparing `typedllm-0.1.1.tar` & `typedllm-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.1/HISTORY.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 typedllm-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 typedllm-0.1.1/tests/test_client.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.1.1/tests/test_interop.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 typedllm-0.1.1/tests/test_langchain.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedllm-0.1.1/tests/test_tool.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.1.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.1.1/LICENSE
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.1.1/README.md
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 typedllm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 typedllm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.2/HISTORY.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 typedllm-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 typedllm-0.1.2/tests/test_client.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.1.2/tests/test_interop.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 typedllm-0.1.2/tests/test_langchain.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedllm-0.1.2/tests/test_tool.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.1.2/LICENSE
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.1.2/README.md
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 typedllm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 typedllm-0.1.2/PKG-INFO
```

### Comparing `typedllm-0.1.1/tests/conftest.py` & `typedllm-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.1/tests/test_client.py` & `typedllm-0.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.1/tests/test_interop.py` & `typedllm-0.1.2/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.1/tests/test_tool.py` & `typedllm-0.1.2/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.1/.gitignore` & `typedllm-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.1/LICENSE` & `typedllm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.1/pyproject.toml` & `typedllm-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.1/PKG-INFO` & `typedllm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: typedllm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Pydantic LLM Interface that sparks Joy
 Author-email: Todd Cullen <todd@100-x.ai>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: litellm>=1.34.1
```

