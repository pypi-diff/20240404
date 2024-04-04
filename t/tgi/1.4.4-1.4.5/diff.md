# Comparing `tmp/tgi-1.4.4.tar.gz` & `tmp/tgi-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgi-1.4.4.tar", max compression
+gzip compressed data, was "tgi-1.4.5.tar", max compression
```

## Comparing `tgi-1.4.4.tar` & `tgi-1.4.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7589 2024-03-26 09:03:37.869972 tgi-1.4.4/README.md
--rw-r--r--   0        0        0      780 2024-03-26 09:27:07.745282 tgi-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      771 2024-03-26 09:02:46.583304 tgi-1.4.4/tgi/__init__.py
--rw-r--r--   0        0        0    31577 2024-03-26 09:02:48.956376 tgi-1.4.4/tgi/client.py
--rw-r--r--   0        0        0     2839 2024-03-26 09:02:46.583836 tgi-1.4.4/tgi/errors.py
--rw-r--r--   0        0        0     5579 2024-03-26 09:02:46.583945 tgi-1.4.4/tgi/inference_api.py
--rw-r--r--   0        0        0    12548 2024-03-26 09:02:48.956582 tgi-1.4.4/tgi/types.py
--rw-r--r--   0        0        0     8602 1970-01-01 00:00:00.000000 tgi-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     7589 2024-03-26 09:03:37.869972 tgi-1.4.5/README.md
+-rw-r--r--   0        0        0      780 2024-04-04 18:46:14.593003 tgi-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0      771 2024-03-26 09:33:59.622830 tgi-1.4.5/tgi/__init__.py
+-rw-r--r--   0        0        0    31577 2024-03-26 09:33:59.622993 tgi-1.4.5/tgi/client.py
+-rw-r--r--   0        0        0     2839 2024-03-26 09:33:59.623166 tgi-1.4.5/tgi/errors.py
+-rw-r--r--   0        0        0     5579 2024-03-26 09:33:59.623307 tgi-1.4.5/tgi/inference_api.py
+-rw-r--r--   0        0        0    12548 2024-03-26 09:33:59.623455 tgi-1.4.5/tgi/types.py
+-rw-r--r--   0        0        0     8602 1970-01-01 00:00:00.000000 tgi-1.4.5/PKG-INFO
```

### Comparing `tgi-1.4.4/README.md` & `tgi-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `tgi-1.4.4/pyproject.toml` & `tgi-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgi"
-version = "1.4.4"
+version = "1.4.5"
 description = "Nightly release of Hugging Face Text Generation Python Client"
 license = "Apache-2.0"
 authors = ["Maziyar PANAHI <maziyar.panahi@cnrs.fr>"]
 maintainers = ["Maziyar PANAHI <maziyar.panahi@cnrs.fr>"]
 readme = "README.md"
 homepage = "https://github.com/huggingface/text-generation-inference"
 repository = "https://github.com/huggingface/text-generation-inference"
```

### Comparing `tgi-1.4.4/tgi/__init__.py` & `tgi-1.4.5/tgi/__init__.py`

 * *Files identical despite different names*

### Comparing `tgi-1.4.4/tgi/client.py` & `tgi-1.4.5/tgi/client.py`

 * *Files identical despite different names*

### Comparing `tgi-1.4.4/tgi/errors.py` & `tgi-1.4.5/tgi/errors.py`

 * *Files identical despite different names*

### Comparing `tgi-1.4.4/tgi/inference_api.py` & `tgi-1.4.5/tgi/inference_api.py`

 * *Files identical despite different names*

### Comparing `tgi-1.4.4/tgi/types.py` & `tgi-1.4.5/tgi/types.py`

 * *Files identical despite different names*

### Comparing `tgi-1.4.4/PKG-INFO` & `tgi-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgi
-Version: 1.4.4
+Version: 1.4.5
 Summary: Nightly release of Hugging Face Text Generation Python Client
 Home-page: https://github.com/huggingface/text-generation-inference
 License: Apache-2.0
 Author: Maziyar PANAHI
 Author-email: maziyar.panahi@cnrs.fr
 Maintainer: Maziyar PANAHI
 Maintainer-email: maziyar.panahi@cnrs.fr
```

