# Comparing `tmp/abi3audit-0.0.9.tar.gz` & `tmp/abi3audit-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi3audit-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "abi3audit-0.0.9a0.tar", last modified: Thu Mar 16 14:42:30 2023, max compression
```

## Comparing `abi3audit-0.0.9.tar` & `abi3audit-0.0.9a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1111 2023-10-27 15:00:00.904759 abi3audit-0.0.9/LICENSE
--rw-r--r--   0        0        0     8937 2023-10-27 15:00:00.904759 abi3audit-0.0.9/README.md
--rw-r--r--   0        0        0       47 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/__init__.py
--rw-r--r--   0        0        0      122 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/__main__.py
--rw-r--r--   0        0        0     4342 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_audit.py
--rw-r--r--   0        0        0      328 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_cache.py
--rw-r--r--   0        0        0     8410 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_cli.py
--rw-r--r--   0        0        0     8794 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_extract.py
--rw-r--r--   0        0        0     7762 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_object.py
--rw-r--r--   0        0        0      592 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_state.py
--rw-r--r--   0        0        0        0 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_vendor/__init__.py
--rw-r--r--   0        0        0     7059 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_vendor/asn1_der.py
--rw-r--r--   0        0        0    89948 2023-10-27 15:00:00.904759 abi3audit-0.0.9/abi3audit/_vendor/mach_o.py
--rw-r--r--   0        0        0     2267 2023-10-27 15:00:00.904759 abi3audit-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    10707 1970-01-01 00:00:00.000000 abi3audit-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0     8937 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/README.md
+-rw-r--r--   0        0        0       49 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/__init__.py
+-rw-r--r--   0        0        0      122 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/__main__.py
+-rw-r--r--   0        0        0     4342 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_audit.py
+-rw-r--r--   0        0        0      328 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_cache.py
+-rw-r--r--   0        0        0     8410 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_cli.py
+-rw-r--r--   0        0        0     8794 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_extract.py
+-rw-r--r--   0        0        0     7762 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_object.py
+-rw-r--r--   0        0        0      592 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_state.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_vendor/__init__.py
+-rw-r--r--   0        0        0     7059 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_vendor/asn1_der.py
+-rw-r--r--   0        0        0    89948 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/abi3audit/_vendor/mach_o.py
+-rw-r--r--   0        0        0     2258 2023-03-16 14:42:21.770029 abi3audit-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0    10700 1970-01-01 00:00:00.000000 abi3audit-0.0.9a0/PKG-INFO
```

### Comparing `abi3audit-0.0.9/LICENSE` & `abi3audit-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/README.md` & `abi3audit-0.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/abi3audit/_audit.py` & `abi3audit-0.0.9a0/abi3audit/_audit.py`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/abi3audit/_cli.py` & `abi3audit-0.0.9a0/abi3audit/_cli.py`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/abi3audit/_extract.py` & `abi3audit-0.0.9a0/abi3audit/_extract.py`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/abi3audit/_object.py` & `abi3audit-0.0.9a0/abi3audit/_object.py`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/abi3audit/_state.py` & `abi3audit-0.0.9a0/abi3audit/_state.py`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/abi3audit/_vendor/asn1_der.py` & `abi3audit-0.0.9a0/abi3audit/_vendor/asn1_der.py`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/abi3audit/_vendor/mach_o.py` & `abi3audit-0.0.9a0/abi3audit/_vendor/mach_o.py`

 * *Files identical despite different names*

### Comparing `abi3audit-0.0.9/pyproject.toml` & `abi3audit-0.0.9a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 ]
 dependencies = [
   "abi3info >= 2023.01.27",
   "kaitaistruct ~= 0.10",
   "packaging >= 21.3,< 24.0",
   "pefile >= 2022.5.30",
   "pyelftools >= 0.29",
-  "requests >= 2.28.1,< 2.32.0",
-  "requests-cache >= 0.9.6,< 1.2.0",
-  "rich >= 12.5.1,< 13.7.0",
+  "requests ~= 2.28.1",
+  "requests-cache >= 0.9.6,< 1.1.0",
+  "rich >= 12.5.1,< 13.4.0",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://pypi.org/project/abi3audit/"
 Issues = "https://github.com/trailofbits/abi3audit/issues"
 Source = "https://github.com/trailofbits/abi3audit"
```

### Comparing `abi3audit-0.0.9/PKG-INFO` & `abi3audit-0.0.9a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi3audit
-Version: 0.0.9
+Version: 0.0.9a0
 Summary: Scans Python wheels for abi3 violations and inconsistencies
 Author-email: William Woodruff <william@trailofbits.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -14,17 +14,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Requires-Dist: abi3info >= 2023.01.27
 Requires-Dist: kaitaistruct ~= 0.10
 Requires-Dist: packaging >= 21.3,< 24.0
 Requires-Dist: pefile >= 2022.5.30
 Requires-Dist: pyelftools >= 0.29
-Requires-Dist: requests >= 2.28.1,< 2.32.0
-Requires-Dist: requests-cache >= 0.9.6,< 1.2.0
-Requires-Dist: rich >= 12.5.1,< 13.7.0
+Requires-Dist: requests ~= 2.28.1
+Requires-Dist: requests-cache >= 0.9.6,< 1.1.0
+Requires-Dist: rich >= 12.5.1,< 13.4.0
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: pdoc3 ; extra == "dev"
 Requires-Dist: abi3audit[test,lint] ; extra == "dev"
 Requires-Dist: bandit ; extra == "lint"
 Requires-Dist: black ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
```

