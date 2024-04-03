# Comparing `tmp/pandas-indexing-0.4.1.tar.gz` & `tmp/pandas-indexing-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.4.1.tar", last modified: Wed Mar 20 21:31:14 2024, max compression
+gzip compressed data, was "pandas-indexing-0.4.2.tar", last modified: Wed Apr  3 21:59:52 2024, max compression
```

## Comparing `pandas-indexing-0.4.1.tar` & `pandas-indexing-0.4.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:31:14.395246 pandas-indexing-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-20 21:31:14.395246 pandas-indexing-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:31:14.387246 pandas-indexing-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/AUTHORS.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:31:14.387246 pandas-indexing-0.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:31:14.387246 pandas-indexing-0.4.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   400307 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 21:31:14.395246 pandas-indexing-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:31:14.383247 pandas-indexing-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:31:14.391246 pandas-indexing-0.4.1/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:31:14.391246 pandas-indexing-0.4.1/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-20 21:30:55.000000 pandas-indexing-0.4.1/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 21:31:14.391246 pandas-indexing-0.4.1/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-20 21:31:14.000000 pandas-indexing-0.4.1/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-20 21:31:14.000000 pandas-indexing-0.4.1/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 21:31:14.000000 pandas-indexing-0.4.1/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-20 21:31:14.000000 pandas-indexing-0.4.1/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 21:31:14.000000 pandas-indexing-0.4.1/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.712595 pandas-indexing-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-03 21:59:52.712595 pandas-indexing-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.704594 pandas-indexing-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/AUTHORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.704594 pandas-indexing-0.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.704594 pandas-indexing-0.4.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   400307 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:59:52.712595 pandas-indexing-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.700595 pandas-indexing-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.708595 pandas-indexing-0.4.2/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31748 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.708595 pandas-indexing-0.4.2/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.708595 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.4.1/.readthedocs.yaml` & `pandas-indexing-0.4.2/.readthedocs.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Required
 version: 2
 
 # Specify os and python version
 build:
   os: "ubuntu-22.04"
   tools:
-    python: "3.10"
+    python: "3.12"
 
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
 # Optionally build your docs in additional formats such as PDF and ePub
 formats: all
@@ -21,7 +21,8 @@
 # Optionally set the version of Python and requirements required to build your docs
 python:
    install:
       - method: pip
         path: .
         extra_requirements:
             - docs
+            - units
```

### Comparing `pandas-indexing-0.4.1/CHANGELOG.rst` & `pandas-indexing-0.4.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+v0.4.2 (2023-04-03)
+------------------------------------------------------------
+* Add :func:`~core.add_zeros_like` for adding explicit `levels` as 0 values :pull:`51`
+
 v0.4.1 (2023-03-20)
 ------------------------------------------------------------
 * Add :func:`~core.antijoin` for performing anti-joins :pull:`48`
 * Update usage guide for ``antijoin``, but also with more focus on ``extractlevel``
 
 v0.4.0 (2023-12-12)
 ------------------------------------------------------------
```

### Comparing `pandas-indexing-0.4.1/CODE_OF_CONDUCT.md` & `pandas-indexing-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/CONTRIBUTING.rst` & `pandas-indexing-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/LICENSE` & `pandas-indexing-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/PKG-INFO` & `pandas-indexing-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.4.1
+Version: 0.4.2
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
```

### Comparing `pandas-indexing-0.4.1/README.rst` & `pandas-indexing-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/docs/api.rst` & `pandas-indexing-0.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/docs/conf.py` & `pandas-indexing-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.4.2/docs/notebooks/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/pyproject.toml` & `pandas-indexing-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/__init__.py` & `pandas-indexing-0.4.2/src/pandas_indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/accessors.py` & `pandas-indexing-0.4.2/src/pandas_indexing/accessors.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import pandas as pd
 from deprecated.sphinx import deprecated
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.api.extensions import no_default
 
 from . import arithmetics
 from .core import (
+    add_zeros_like,
     aggregatelevel,
     antijoin,
     assignlevel,
     describelevel,
     dropnalevel,
     extractlevel,
     fixindexna,
@@ -204,14 +205,24 @@
         mode: Literal["replace", "append", "return"] = "replace",
         **levels: Dict[str, Sequence[Any]],
     ):
         return aggregatelevel(
             self._obj, agg_func=agg_func, axis=axis, dropna=dropna, mode=mode, **levels
         )
 
+    @doc(add_zeros_like, data="")
+    def add_zeros_like(
+        self,
+        reference: Union[MultiIndex, DataFrame, Series],
+        /,
+        derive: Optional[Dict[str, MultiIndex]] = None,
+        **levels: Sequence[str],
+    ):
+        return add_zeros_like(self._obj, reference=reference, derive=derive, **levels)
+
 
 def _create_forward_binop(op):
     def forward_binop(
         self,
         other: Data,
         assign: Optional[Dict[str, Any]] = None,
         axis: Optional[Axis] = None,
```

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.4.2/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/core.py` & `pandas-indexing-0.4.2/src/pandas_indexing/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1071,7 +1071,68 @@
             return data.combine_first(new_data)
         else:
             return concat([data, new_data], axis=axis, sort=True)
     else:
         raise ValueError(
             f'mode must be "replace", "append" or "return", but is "{mode}"'
         )
+
+
+@doc(
+    data="""
+    data : Data
+        Series or DataFrame to extend with zeros\
+    """
+)
+def add_zeros_like(
+    data: T,
+    reference: Union[MultiIndex, DataFrame, Series],
+    *,
+    derive: Optional[Dict[str, MultiIndex]] = None,
+    **levels: Sequence[str],
+) -> T:
+    """Add explicit `levels` to `data` as 0 values.
+
+    Remaining levels in `data` not found in `levels` or `derive` are taken from
+    `reference` (or its index).
+
+    Parameters
+    ----------\
+    {data}
+    reference : Index
+        expected level labels (like model, scenario combinations)
+    derive : dict
+        derive labels in a level from a multiindex with allowed combinations
+    **levels : [str]
+        which labels should be added to df
+
+    Returns
+    -------
+    DataFrame
+        unsorted data with additional zero data
+    """
+
+    if any(len(labels) == 0 for labels in levels.values()):
+        return data
+
+    if isinstance(reference, (Series, DataFrame)):
+        reference = reference.index
+
+    if derive is None:
+        derive = {}
+
+    target_levels = data.index.names
+    index = reference.pix.unique(
+        target_levels.difference(levels.keys()).difference(derive.keys())
+    )
+
+    zero_index = concat(
+        reduce(
+            lambda ind, d: ind.join(d, how="left"),
+            derive.values(),
+            index.pix.assign(**dict(zip(levels.keys(), labels))),
+        ).reorder_levels(target_levels)
+        for labels in product(*levels.values())
+    )
+    zero_index = antijoin(zero_index, data.index)
+
+    return concat([data, pd.DataFrame(0, index=zero_index, columns=data.columns)])
```

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.4.2/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.4.2/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/selectors.py` & `pandas-indexing-0.4.2/src/pandas_indexing/selectors.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/units.py` & `pandas-indexing-0.4.2/src/pandas_indexing/units.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing/utils.py` & `pandas-indexing-0.4.2/src/pandas_indexing/utils.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.4.2/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.4.1
+Version: 0.4.2
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
```

### Comparing `pandas-indexing-0.4.1/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.4.2/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 CHANGELOG.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-requirements.txt
 docs/AUTHORS.rst
 docs/api.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
```

