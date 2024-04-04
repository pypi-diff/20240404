# Comparing `tmp/pelage-0.1.7.tar.gz` & `tmp/pelage-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelage-0.1.7.tar", max compression
+gzip compressed data, was "pelage-0.1.8.tar", max compression
```

## Comparing `pelage-0.1.7.tar` & `pelage-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2024-03-07 21:02:52.572635 pelage-0.1.7/LICENSE
--rw-r--r--   0        0        0     5017 2024-04-01 08:04:17.807723 pelage-0.1.7/README.md
--rw-r--r--   0        0        0       42 2024-03-09 07:40:35.887285 pelage-0.1.7/pelage/__init__.py
--rw-r--r--   0        0        0    43354 2024-04-01 07:05:25.599000 pelage-0.1.7/pelage/checks.py
--rw-r--r--   0        0        0        0 2024-03-07 20:43:38.400138 pelage-0.1.7/pelage/data/.keep
--rw-r--r--   0        0        0      774 2024-03-22 06:43:08.899733 pelage-0.1.7/pelage/utils.py
--rw-r--r--   0        0        0      602 2024-04-01 08:06:08.508536 pelage-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5665 1970-01-01 00:00:00.000000 pelage-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-07 21:02:52.572635 pelage-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4727 2024-04-04 16:22:53.886116 pelage-0.1.8/README.md
+-rw-r--r--   0        0        0       42 2024-03-09 07:40:35.887285 pelage-0.1.8/pelage/__init__.py
+-rw-r--r--   0        0        0    43450 2024-04-03 18:00:15.892560 pelage-0.1.8/pelage/checks.py
+-rw-r--r--   0        0        0        0 2024-03-07 20:43:38.400138 pelage-0.1.8/pelage/data/.keep
+-rw-r--r--   0        0        0      774 2024-03-22 06:43:08.899733 pelage-0.1.8/pelage/utils.py
+-rw-r--r--   0        0        0      684 2024-04-04 16:24:31.855310 pelage-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 pelage-0.1.8/PKG-INFO
```

### Comparing `pelage-0.1.7/LICENSE` & `pelage-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pelage-0.1.7/pelage/checks.py` & `pelage-0.1.8/pelage/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module containing the main checks for pelage.
 
 Use the syntax `import pelage as plg` rather than `from pelage import checks`
 """
+
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 import polars as pl
 from packaging import version
 from polars.type_aliases import ClosedInterval, IntoExpr, PolarsDataType
 
 from pelage import utils
@@ -1175,16 +1176,17 @@
     │ 3   │
     └─────┘
     Error with the DataFrame passed to the check function:
     -->Unexpected data in `Custom Check`: [(col("a")) != (3)]
     """
     bad_data = data.filter(expresion.not_())
     if not bad_data.is_empty():
+        columns_in_expression = set(expresion.meta.root_names())
         raise PolarsAssertError(
-            df=bad_data,
+            df=bad_data.select(columns_in_expression),
             supp_message=f"Unexpected data in `Custom Check`: {str(expresion)}",
         )
     return data
 
 
 def mutually_exclusive_ranges(
     data: pl.DataFrame,
```

### Comparing `pelage-0.1.7/pelage/utils.py` & `pelage-0.1.8/pelage/utils.py`

 * *Files identical despite different names*

### Comparing `pelage-0.1.7/pyproject.toml` & `pelage-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelage"
-version = "0.1.7"
+version = "0.1.8"
 description = "This package contains a collection of tests to improve your Polars data analysis superpowers"
 authors = ["Alix Tiran-Cappello <alix.tiran-cappello@laposte.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.8, < 3.13"
@@ -16,10 +16,15 @@
 isort = ">=5.13.2"
 ruff = ">=0.3.0"
 pre-commit = "*"
 coverage = ">=7.4.3"
 ipykernel = ">=6.29.3"
 
 
+
+[tool.poetry.group.extras.dependencies]
+seaborn = "^0.13.2"
+pyarrow = "^15.0.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

