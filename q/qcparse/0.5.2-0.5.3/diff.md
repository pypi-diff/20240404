# Comparing `tmp/qcparse-0.5.2.tar.gz` & `tmp/qcparse-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcparse-0.5.2.tar", max compression
+gzip compressed data, was "qcparse-0.5.3.tar", max compression
```

## Comparing `qcparse-0.5.2.tar` & `qcparse-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3849 2023-09-28 04:52:50.290173 qcparse-0.5.2/README.md
--rw-r--r--   0        0        0     1151 2023-09-28 04:52:50.290173 qcparse-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      314 2023-09-28 04:52:50.290173 qcparse-0.5.2/qcparse/__init__.py
--rw-r--r--   0        0        0      832 2023-09-28 04:52:50.290173 qcparse-0.5.2/qcparse/cli.py
--rw-r--r--   0        0        0        0 2023-09-28 04:52:50.290173 qcparse-0.5.2/qcparse/encoders/__init__.py
--rw-r--r--   0        0        0     2064 2023-09-28 04:52:50.290173 qcparse-0.5.2/qcparse/encoders/terachem.py
--rw-r--r--   0        0        0      634 2023-09-28 04:52:50.290173 qcparse-0.5.2/qcparse/exceptions.py
--rw-r--r--   0        0        0     3700 2023-09-28 04:52:50.290173 qcparse-0.5.2/qcparse/main.py
--rw-r--r--   0        0        0     5888 2023-09-28 04:52:50.290173 qcparse-0.5.2/qcparse/models.py
--rw-r--r--   0        0        0      758 2023-09-28 04:52:50.294173 qcparse-0.5.2/qcparse/parsers/__init__.py
--rw-r--r--   0        0        0     5101 2023-09-28 04:52:50.294173 qcparse-0.5.2/qcparse/parsers/terachem.py
--rw-r--r--   0        0        0     2505 2023-09-28 04:52:50.294173 qcparse-0.5.2/qcparse/parsers/utils.py
--rw-r--r--   0        0        0     1090 2023-09-28 04:52:50.294173 qcparse-0.5.2/qcparse/utils.py
--rw-r--r--   0        0        0     4511 1970-01-01 00:00:00.000000 qcparse-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     3849 2024-04-04 21:27:31.226002 qcparse-0.5.3/README.md
+-rw-r--r--   0        0        0     1152 2024-04-04 21:27:31.226002 qcparse-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      314 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/cli.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/encoders/__init__.py
+-rw-r--r--   0        0        0     2064 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/encoders/terachem.py
+-rw-r--r--   0        0        0      634 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/exceptions.py
+-rw-r--r--   0        0        0     3700 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/main.py
+-rw-r--r--   0        0        0     5888 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/models.py
+-rw-r--r--   0        0        0      759 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/parsers/__init__.py
+-rw-r--r--   0        0        0     4936 2024-04-04 21:27:31.226002 qcparse-0.5.3/qcparse/parsers/terachem.py
+-rw-r--r--   0        0        0     2505 2024-04-04 21:27:31.230002 qcparse-0.5.3/qcparse/parsers/utils.py
+-rw-r--r--   0        0        0     1090 2024-04-04 21:27:31.230002 qcparse-0.5.3/qcparse/utils.py
+-rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 qcparse-0.5.3/PKG-INFO
```

### Comparing `qcparse-0.5.2/README.md` & `qcparse-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `qcparse-0.5.2/pyproject.toml` & `qcparse-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qcparse"
-version = "0.5.2"
+version = "0.5.3"
 description = "A package for parsing Quantum Chemistry program file outputs into structured qcio data objects."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -13,15 +13,15 @@
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
 isort = "^5.12.0"
 pytest = "^7.2.2"
 pre-commit = "^3.2.0"
 pytest-cov = "^4.0.0"
-black = "^23.3.0"
+black = ">=24.0.0"
 ruff = "^0.0.275"
 
 [tool.poetry.scripts]
 qcparse = "qcparse.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `qcparse-0.5.2/qcparse/cli.py` & `qcparse-0.5.3/qcparse/cli.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.5.2/qcparse/encoders/terachem.py` & `qcparse-0.5.3/qcparse/encoders/terachem.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.5.2/qcparse/exceptions.py` & `qcparse-0.5.3/qcparse/exceptions.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.5.2/qcparse/main.py` & `qcparse-0.5.3/qcparse/main.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.5.2/qcparse/models.py` & `qcparse-0.5.3/qcparse/models.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.5.2/qcparse/parsers/__init__.py` & `qcparse-0.5.3/qcparse/parsers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 
 Use the .utils.regex_search() helper function in place of re.search() to
 ensure that a MatchNotFoundError will be raised in a parser. More sophisticated parsers
 that use re.findall (like terachem.parse_hessian) or rely upon not finding a match may
 implement a different interface, but please strive to follow this basic patterns as much
 as possible.
 """
+
 # Required for parsers to register
 from .terachem import *  # noqa:  F403
```

### Comparing `qcparse-0.5.2/qcparse/parsers/terachem.py` & `qcparse-0.5.3/qcparse/parsers/terachem.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         This function searches the entire document N times for all regex matches where
         N is the number of atoms. This makes the function's code easy to reason about.
         If performance becomes an issues for VERY large Hessians (unlikely) you can
         accelerate this function by parsing all Hessian floats in one pass, like the
         parse_gradient function above, and then doing the math to figure out how to
         properly sequence those values to from the Hessian matrix given TeraChem's
         six-column format for printing out Hessian matrix entries.
-
     """
     # requires .format(int). {{}} values are to escape {15|2} for .format()
     regex = r"(?:\s+{}\s)((?:\s-?\d\.\d{{15}}e[+-]\d{{2}})+)"
     hessian = []
 
     # Match all rows containing Hessian data; one set of rows at a time
     count = 1
@@ -107,38 +106,32 @@
 @parser()
 def parse_nmo(string: str, data_collector: ParsedDataCollector):
     """Parse the number of molecular orbitals TeraChem stdout"""
     regex = r"Total orbitals:\s*(\d+)"
     data_collector.calcinfo_nmo = int(regex_search(regex, string).group(1))
 
 
-def parse_git_commit(string: str) -> str:
-    """Parse TeraChem git commit from TeraChem stdout."""
-    regex = r"Git Version: (\S*)"
-    return regex_search(regex, string).group(1)
+def parse_version_control_details(string: str) -> str:
+    """Parse TeraChem git commit or Hg version from TeraChem stdout."""
+    regex = r"(Git|Hg) Version: (\S*)"
+    return regex_search(regex, string).group(2)
 
 
 def parse_terachem_version(string: str) -> str:
     """Parse TeraChem version from TeraChem stdout."""
     regex = r"TeraChem (v\S*)"
     return regex_search(regex, string).group(1)
 
 
 def parse_version_string(string: str) -> str:
     """Parse version string plus git commit from TeraChem stdout.
 
     Matches format of 'terachem --version' on command line.
     """
-    return f"{parse_terachem_version(string)} [{parse_git_commit(string)}]"
-
-
-@parser()
-def parse_version(string: str, data_collector: ParsedDataCollector):
-    """Parse TeraChem version from TeraChem stdout."""
-    data_collector.extras.program_version = parse_version_string(string)
+    return f"{parse_terachem_version(string)} [{parse_version_control_details(string)}]"
 
 
 def calculation_succeeded(string: str) -> bool:
     """Determine from TeraChem stdout if a calculation completed successfully."""
     regex = r"Job finished:"
     if re.search(regex, string):
         # If any match for a failure regex is found, the calculation failed
```

### Comparing `qcparse-0.5.2/qcparse/parsers/utils.py` & `qcparse-0.5.3/qcparse/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.5.2/qcparse/utils.py` & `qcparse-0.5.3/qcparse/utils.py`

 * *Files identical despite different names*

### Comparing `qcparse-0.5.2/PKG-INFO` & `qcparse-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: qcparse
-Version: 0.5.2
+Version: 0.5.3
 Summary: A package for parsing Quantum Chemistry program file outputs into structured qcio data objects.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.0.0)
 Requires-Dist: qcio (>=0.7.1)
 Description-Content-Type: text/markdown
 
 # qcparse
 
 A library for parsing Quantum Chemistry output files into structured data objects and converting structured input objects into program-native input files. Uses data structures from [qcio](https://github.com/coltonbh/qcio).
```

