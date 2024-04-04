# Comparing `tmp/nablachem-24.2.tar.gz` & `tmp/nablachem-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nablachem-24.2.tar", max compression
+gzip compressed data, was "nablachem-24.4.tar", max compression
```

## Comparing `nablachem-24.2.tar` & `nablachem-24.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2024-01-21 09:39:54.867938 nablachem-24.2/LICENSE
--rw-r--r--   0        0        0      459 2024-01-22 09:10:33.527618 nablachem-24.2/README.md
--rw-r--r--   0        0        0      553 2024-01-22 10:01:40.076550 nablachem-24.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-21 09:41:21.927909 nablachem-24.2/src/nablachem/__init__.py
--rw-r--r--   0        0        0    15645 2024-01-22 09:32:01.727176 nablachem-24.2/src/nablachem/alchemy.py
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 nablachem-24.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-01-21 09:39:54.867938 nablachem-24.4/LICENSE
+-rw-r--r--   0        0        0      559 2024-01-22 10:02:27.526533 nablachem-24.4/README.md
+-rw-r--r--   0        0        0      553 2024-04-04 14:23:12.466569 nablachem-24.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-21 09:41:21.927909 nablachem-24.4/src/nablachem/__init__.py
+-rw-r--r--   0        0        0    12152 2024-04-04 14:19:27.006647 nablachem-24.4/src/nablachem/alchemy.py
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 nablachem-24.4/PKG-INFO
```

### Comparing `nablachem-24.2/LICENSE` & `nablachem-24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nablachem-24.2/pyproject.toml` & `nablachem-24.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nablachem"
-version = "24.2"
+version = "24.4"
 description = "Easy access to research code."
 authors = ["von Rudorff, Guido Falk <vonrudorff@uni-kassel.de>"]
 license = "LGPL"
 readme = "README.md"
 homepage = "https://nablachem.org/code"
 repository = "https://github.com/NablaChem/nablachem"
```

### Comparing `nablachem-24.2/src/nablachem/alchemy.py` & `nablachem-24.4/src/nablachem/alchemy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pandas as pd
 import findiff
 import numpy as np
-import collections
 import math
+import collections
 import itertools as it
-from typing import Union
 
 from scipy.optimize import minimize
 
 
 class Monomial:
     """A single monomial in the multi-dimensional Taylor expansion."""
 
@@ -20,29 +19,32 @@
         prefactor : float
             Weight or coefficient of the monomial.
         powers : dict[str, int], optional
             Involved variables as keys and the exponent as value, by default {}.
         """
         self._powers = powers
         self._prefactor = prefactor
+        self._cached_prefactor = None
 
     def __repr__(self):
         return f"Monomial({self._prefactor}, {self._powers})"
 
     def prefactor(self) -> float:
         """Calculates the Taylor expansion prefactor.
 
         Returns
         -------
         float
             Prefactor for the summation in the Taylor expansion.
         """
-        return self._prefactor / np.prod(
-            [math.factorial(_) for _ in self._powers.values()]
-        )
+        if self._cached_prefactor is None:
+            self._cached_prefactor = self._prefactor / np.prod(
+                [math.factorial(_) for _ in self._powers.values()]
+            )
+        return self._cached_prefactor
 
     def distance(self, pos: dict[str, float], center: dict[str, float]) -> float:
         """Evaluate the distance term of the Taylor expansion.
 
         Parameters
         ----------
         pos : dict[str, float]
@@ -54,15 +56,15 @@
         -------
         float
             Distance
         """
         ret = []
         for column, power in self._powers.items():
             ret.append((pos[column] - center[column]) ** power)
-        return np.prod(ret)
+        return math.prod(ret)
 
 
 class MultiTaylor:
     """Multi-dimensional multi-variate arbitrary order Taylor expansion from any evenly spaced finite difference stencil.
 
     Examples
     --------
@@ -103,14 +105,15 @@
         self._dataframe = dataframe
         self._outputs = outputs
         self._filtered = dataframe
         self._filter = {}
 
     def reset_center(self, **kwargs: float):
         """Sets the expansion center from named arguments for each column."""
+
         self._center = kwargs
 
     def reset_filter(self, **kwargs: float):
         """Sets the filter for the dataframe from named arguments for each column.
 
         All columns which are not filtered and not outputs are considered to be input coordinates.
         """
@@ -130,232 +133,135 @@
         Returns
         -------
         pd.DataFrame
             Filtered dataframe.
         """
         return df.loc[(df[list(filter)] == pd.Series(filter)).all(axis=1)]
 
-    def _check_uniqueness(self, df: pd.DataFrame, terms: list[str]):
-        """Checks whether the stencil is unique, i.e. whether sufficiently many columns have been filtered.
-
-        If the raw data contains columns I1, I2, O1, O2, A and B, with all evaluated at different points, then a stencil
-        over the input columns I1, I2 can be evaluated for the output columns O1 and O2 only if columns A and B are filtered
-        such that only one set of values remains for each set of values in the I columns.
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            Stencil dataframe, possibly filtered.
-        terms : list[str]
-            List of columns that should be unique for a given stencil.
-
-        Raises
-        ------
-        ValueError
-            When there are other columns that are not unique.
-        """
-        copy = df.copy()
-
-        # remove variable column
-        for term in terms:
-            del copy[term]
-
-        # remove output columns: they are arbitrary
-        for output in self._outputs:
-            del copy[output]
-
-        copy.drop_duplicates(inplace=True)
-        if len(copy.index) > 1 and len(copy.columns) > 0:
-            print(copy)
-            print(copy.index)
-            print(copy.columns)
-            raise ValueError(f"Terms {terms} are not unique. Is a filter missing?")
-
-    def _split_term(self, term: str, order: int) -> dict[str, int]:
-        """Splits a string-based term into a dictionary based term.
-
-        Keys are the variable names, values are the exponents.
-
-        Parameters
-        ----------
-        term : str
-            String-based term, e.g. A_B_C or A_A_B or A, where the letters are the variable names. All variable names must be given, only for the special case of all variable names being identical, this can be omitted.
-        order : int
-            The total expansion order of this term, i.e. the sum of all exponents.
-
-        Returns
-        -------
-        dict[str, int]
-            Explicit split term representation.
-
-        Raises
-        ------
-        ValueError
-            Wrong order given
-        """
-        parts = term.split("_")
-        if len(parts) == 1:
-            parts = [parts[0]] * order
-        if len(parts) != order:
-            raise ValueError(f"Term {term} has the wrong order.")
-
-        return dict(collections.Counter(parts))
-
-    def _offsets_from_df(
-        self, df: pd.DataFrame, variable_columns: list[str]
-    ) -> tuple[list[tuple[float]], list[float]]:
+    def _offsets(self) -> tuple[np.ndarray, tuple[str]]:
         """Transforms the available data points in the dataframe into stencil offsets.
 
-        Parameters
-        ----------
-        df : pd.DataFrame
-            Stencil, i.e. filtered and subselected data frame.
-        variable_columns : list[str]
-            List of variables to consider.
-
         Returns
         -------
-        tuple[list[tuple[float]], list[float]]
-            Offsets and spacings for the stencil.
-
-        Raises
-        ------
-        ValueError
-            One column is not evenly spaced.
+        tuple[np.ndarray, tuple[str]]
+            Offsets for the stencil and list of variable names in matching order.
         """
-        offsets = np.zeros((len(variable_columns), len(df)), dtype=float)
-        spacings = dict()
-
-        for column in variable_columns:
-            unique_values = np.sort(df[column].unique())
-            spacing = np.diff(unique_values)
-            if not np.allclose(spacing, spacing.mean()):
-                raise ValueError(f"Variable {column} is not evenly spaced.")
-            offsets[variable_columns.index(column)] = (
-                df[column].values - self._center[column]
-            ) / spacing.mean()
-            spacings[column] = spacing.mean()
-
-        return [tuple(_) for _ in offsets.T], [spacings[_] for _ in variable_columns]
-
-    def _build_monomials(self, df: pd.DataFrame, term: str, order: int):
+        variables = [_ for _ in self._filtered.columns if _ not in self._outputs]
+        center = np.array([self._center[_] for _ in variables])
+        offsets = self._filtered[variables].values - center
+        return offsets, tuple(variables)
+
+    def _build_monomials(
+        self, term: tuple[str], shifted: tuple[np.ndarray, tuple[str]]
+    ):
         """Builds all monomials and ensures that the stencil is applicable.
 
         Parameters
         ----------
-        df : pd.DataFrame
-            All filtered input data.
         term : str
             String-based term representation.
-        order : int
-            Expansion order
+        shifted : tuple[np.ndarray, tuple[str]]:
+            Cached version of self._offset()
 
         Raises
         ------
         ValueError
-            No stencil could be built.
+            Could not build stencil.
         ValueError
             Not enough points in the stencil for a given order.
         """
-        variable_columns = list(set(term.split("_")))
-        offsets, spacings = self._offsets_from_df(df, variable_columns)
-        assert len(offsets) == len(set(offsets))
-        terms = self._split_term(term, order)
-        partials = tuple([terms[_] for _ in variable_columns])
+        offsets, ordering = shifted
+
+        term_counter = collections.Counter(term)
+        indices = tuple([term_counter[_] for _ in ordering])
 
+        offsets = tuple(map(tuple, offsets))
         try:
             stencil = findiff.stencils.Stencil(
-                offsets, partials={partials: 1}, spacings=spacings
+                offsets, partials={indices: 1}, spacings=1
             )
         except:
             raise ValueError(f"Could not build stencil for term {term}.")
         if len(stencil.values) == 0:
-            print(df)
-            print(order)
-            print(offsets)
-            print(variable_columns)
-            print(partials)
             raise ValueError(f"Not enough points for term {term}.")
 
         for output in self._outputs:
             weights = [stencil.values[_] if _ in stencil.values else 0 for _ in offsets]
-            values = df[output].values
+            values = self._filtered[output].values
 
             self._monomials[output].append(
                 Monomial(
                     prefactor=np.dot(weights, values),
-                    powers=terms,
+                    powers=dict(term_counter),
                 )
             )
 
-    def _all_terms_up_to(self, order: int) -> dict[int, list[str]]:
+    def _all_terms_up_to(self, order: int) -> tuple[tuple[str]]:
         """For all remaining input columns, find all possible terms entering a Taylor expansion.
 
         Parameters
         ----------
         order : int
             The maximum order of the expansion.
 
         Returns
         -------
-        dict[int, list[str]]
-            Order as key, list of terms as value.
+        tuple[tuple[str]]
+            Series of terms up to the given order, as a tuple of variable names.
         """
-        terms = {}
+        terms = []
         data_columns = [_ for _ in self._filtered.columns if _ not in self._outputs]
         data_columns = [_ for _ in data_columns if not _ in self._filter.keys()]
         for order in range(1, order + 1):
-            terms[order] = [
-                "_".join(_)
-                for _ in it.combinations_with_replacement(data_columns, order)
-            ]
-        return terms
+            for entry in it.combinations_with_replacement(data_columns, order):
+                terms.append(entry)
+        return tuple(terms)
 
-    def build_model(self, orders: Union[int, dict[int, list[str]]]):
+    def build_model(self, orders: int):
         """Sets up the model for a specific expansion order.
 
         Parameters
         ----------
-        orders : Union[int, dict[int, list[str]]]
-            Either int, then all terms are included in the expansion up to this order. Otherwise, a dictionary with the order as key and a list of string-based terms as value.
+        orders : int
+            All terms are included in the expansion up to this order.
 
         Raises
         ------
         NotImplementedError
             Center needs to be given in dataframe.
         ValueError
             Center is not unique.
+        ValueError
+            Duplicate points in the dataset.
         """
         # check center: there can be only one
         center_rows = self._dict_filter(self._dataframe, self._center)
         center_row = self._dict_filter(center_rows, self._filter)
         if len(center_row) == 0:
             raise NotImplementedError(f"Center is not in the dataframe.")
         if len(center_row) > 1:
             raise ValueError(f"Center is not unique.")
 
+        # check for duplicates
+        shifted = self._offsets()
+        if len(self._filtered[list(shifted[1])].drop_duplicates()) != len(
+            self._filtered
+        ):
+            raise ValueError(f"Duplicate points in the dataset.")
+
         # setup constant term
         self._monomials = {k: [Monomial(center_row.iloc[0][k])] for k in self._outputs}
 
-        # accept integer as placeholder
-        if isinstance(orders, int):
-            orders = self._all_terms_up_to(orders)
-
-        # setup other terms
-        for order, terms in orders.items():
-            for term in terms:
-                if order == 1:
-                    other_fields = {k: v for k, v in self._center.items() if k != term}
-                else:
-                    other_fields = {
-                        k: v for k, v in self._center.items() if k not in term
-                    }
-                s = self._dict_filter(self._filtered, other_fields)
-                self._check_uniqueness(s, self._split_term(term, order).keys())
-                self._build_monomials(s, term, order)
+        terms = self._all_terms_up_to(orders)
+        if len(terms) > len(shifted[0]):
+            raise ValueError(
+                f"Not enough points: {len(terms)} required, {len(shifted[0])} given."
+            )
+        for term in terms:
+            self._build_monomials(term, shifted)
 
     def query(self, **kwargs: float) -> float:
         """Evaluate the Taylor expansion at a given point.
 
         Returns
         -------
         float
```

### Comparing `nablachem-24.2/PKG-INFO` & `nablachem-24.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nablachem
-Version: 24.2
+Version: 24.4
 Summary: Easy access to research code.
 Home-page: https://nablachem.org/code
 License: LGPL
 Author: von Rudorff, Guido Falk
 Author-email: vonrudorff@uni-kassel.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
@@ -21,7 +21,15 @@
 ## Purpose
 
 We care about fundamental properties of chemical space and their connection to quantum alchemy for molecules and materials. This repository collects the core algorithms once they are somewhat finalized.
 
 - Library use: This code is meant to be used as a library from other projects and therefore is cleaned up and documented.
 - Supported: Unlike the research project repositories (which are frozen in time), we provide bug fixes for this library.
 
+## Installation
+
+The python package is available via pip:
+
+```
+pip install --upgrade nablachem
+```
+
```

