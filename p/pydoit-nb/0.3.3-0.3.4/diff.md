# Comparing `tmp/pydoit_nb-0.3.3.tar.gz` & `tmp/pydoit_nb-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoit_nb-0.3.3.tar", max compression
+gzip compressed data, was "pydoit_nb-0.3.4.tar", max compression
```

## Comparing `pydoit_nb-0.3.3.tar` & `pydoit_nb-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1587 2024-02-15 16:35:39.666695 pydoit_nb-0.3.3/LICENCE
--rw-r--r--   0        0        0     3386 2024-02-15 16:35:39.666695 pydoit_nb-0.3.3/README.md
--rw-r--r--   0        0        0     5401 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      148 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/__init__.py
--rw-r--r--   0        0        0     2893 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/attrs_helpers.py
--rw-r--r--   0        0        0     3835 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/checklist.py
--rw-r--r--   0        0        0      698 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/complete.py
--rw-r--r--   0        0        0     6493 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/config_handling.py
--rw-r--r--   0        0        0     2730 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/config_helpers.py
--rw-r--r--   0        0        0      420 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/config_tools/__init__.py
--rw-r--r--   0        0        0     1574 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/display.py
--rw-r--r--   0        0        0     2332 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/doit_tools.py
--rw-r--r--   0        0        0     5729 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/notebook.py
--rw-r--r--   0        0        0     4250 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/notebook_run.py
--rw-r--r--   0        0        0     4550 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/notebook_step.py
--rw-r--r--   0        0        0        0 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/py.typed
--rw-r--r--   0        0        0     8404 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/serialization.py
--rw-r--r--   0        0        0    16519 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/tasks_copy_source.py
--rw-r--r--   0        0        0     2263 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/tasks_generation.py
--rw-r--r--   0        0        0     1088 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/testing.py
--rw-r--r--   0        0        0     3159 2024-02-15 16:35:39.670695 pydoit_nb-0.3.3/src/pydoit_nb/typing.py
--rw-r--r--   0        0        0     4213 1970-01-01 00:00:00.000000 pydoit_nb-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1587 2024-04-04 06:12:03.136631 pydoit_nb-0.3.4/LICENCE
+-rw-r--r--   0        0        0     3386 2024-04-04 06:12:03.136631 pydoit_nb-0.3.4/README.md
+-rw-r--r--   0        0        0     5401 2024-04-04 06:12:03.136631 pydoit_nb-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      148 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/__init__.py
+-rw-r--r--   0        0        0     2893 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/attrs_helpers.py
+-rw-r--r--   0        0        0     3835 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/checklist.py
+-rw-r--r--   0        0        0      698 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/complete.py
+-rw-r--r--   0        0        0     7287 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/config_handling.py
+-rw-r--r--   0        0        0     2730 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/config_helpers.py
+-rw-r--r--   0        0        0      420 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/config_tools/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/display.py
+-rw-r--r--   0        0        0     2332 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/doit_tools.py
+-rw-r--r--   0        0        0     5729 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/notebook.py
+-rw-r--r--   0        0        0     4250 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/notebook_run.py
+-rw-r--r--   0        0        0     4550 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/notebook_step.py
+-rw-r--r--   0        0        0        0 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/py.typed
+-rw-r--r--   0        0        0     9143 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/serialization.py
+-rw-r--r--   0        0        0    16519 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/tasks_copy_source.py
+-rw-r--r--   0        0        0     2263 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/tasks_generation.py
+-rw-r--r--   0        0        0     1088 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/testing.py
+-rw-r--r--   0        0        0     3159 2024-04-04 06:12:03.140632 pydoit_nb-0.3.4/src/pydoit_nb/typing.py
+-rw-r--r--   0        0        0     4213 1970-01-01 00:00:00.000000 pydoit_nb-0.3.4/PKG-INFO
```

### Comparing `pydoit_nb-0.3.3/LICENCE` & `pydoit_nb-0.3.4/LICENCE`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/README.md` & `pydoit_nb-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/pyproject.toml` & `pydoit_nb-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydoit-nb"
-version = "0.3.3"
+version = "0.3.4"
 description = "Library to support combining jupyter notebooks and pydoit."
 authors = ["Zebedee Nicholls <zebedee.nicholls@climate-resource.com>"]
 readme = "README.md"
 packages = [{include = "pydoit_nb", from = "src"}]
 license = "BSD-3-Clause"
 include = ["LICENCE"]  # not spelt licence, silly US english
```

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/attrs_helpers.py` & `pydoit_nb-0.3.4/src/pydoit_nb/attrs_helpers.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/checklist.py` & `pydoit_nb-0.3.4/src/pydoit_nb/checklist.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/complete.py` & `pydoit_nb-0.3.4/src/pydoit_nb/complete.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/config_handling.py` & `pydoit_nb-0.3.4/src/pydoit_nb/config_handling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """
 Tools for working with configuration
 """
+
 from __future__ import annotations
 
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Any, Callable, TypeVar, cast, overload
 
 import attrs
 import numpy as np
 from attrs import AttrsInstance, evolve, fields
 
 from pydoit_nb.serialization import write_config_in_config_bundle_to_disk
 from pydoit_nb.typing import ConfigBundleCreator, ConfigBundleLike, Converter, NotebookConfigLike
 
+try:
+    import pint
+
+    HAS_PINT = True
+except ImportError:  # pragma: no cover
+    HAS_PINT = False
+
 T = TypeVar("T")
 
 
 def insert_path_prefix(config: AI, prefix: Path) -> AI:
     """
     Insert path prefix into config attributes
 
@@ -44,23 +52,50 @@
         attr_value = getattr(config, attr_name)
 
         if isinstance(attr_value, dict):
             evolutions[attr_name] = {
                 update_attr_value(k, prefix): update_attr_value(v, prefix) for k, v in attr_value.items()
             }
 
-        elif not isinstance(attr_value, (str, np.ndarray)) and isinstance(attr_value, Iterable):
+        elif isinstance(attr_value, Iterable) and iterable_values_are_updatable(attr_value):
             evolutions[attr_name] = [update_attr_value(v, prefix) for v in attr_value]
 
         else:
             evolutions[attr_name] = update_attr_value(attr_value, prefix)
 
     return evolve(config, **evolutions)  # type: ignore # no idea why this fails
 
 
+# TODO: test this by testing that a value
+# which has a pint quantity as an attribute
+# doesn't cause insert_path_prefix to explode.
+def iterable_values_are_updatable(value: Iterable[Any]) -> bool:
+    """
+    Determine whether an iterable's values are updatable by :func:`insert_path_prefix`.
+
+    Parameters
+    ----------
+    value
+        Value to check.
+
+    Returns
+    -------
+        ``True`` if ``value``'s elements can be updated by :func:`update_attr_value`,
+        ``False`` otherwise.
+    """
+    to_check = [str, np.ndarray]
+    if HAS_PINT:
+        to_check.append(pint.UnitRegistry.Quantity)
+
+    if isinstance(value, tuple(to_check)):
+        return False
+
+    return True
+
+
 @overload
 def update_attr_value(value: AttrsInstance, prefix: Path) -> AttrsInstance:
     ...  # pragma: no cover
 
 
 @overload
 def update_attr_value(value: Path, prefix: Path) -> Path:
```

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/config_helpers.py` & `pydoit_nb-0.3.4/src/pydoit_nb/config_helpers.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/display.py` & `pydoit_nb-0.3.4/src/pydoit_nb/display.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/doit_tools.py` & `pydoit_nb-0.3.4/src/pydoit_nb/doit_tools.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/notebook.py` & `pydoit_nb-0.3.4/src/pydoit_nb/notebook.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/notebook_run.py` & `pydoit_nb-0.3.4/src/pydoit_nb/notebook_run.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/notebook_step.py` & `pydoit_nb-0.3.4/src/pydoit_nb/notebook_step.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/serialization.py` & `pydoit_nb-0.3.4/src/pydoit_nb/serialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 more care and time than we can put in right now. As two suggestions for
 possible solutions: 1) use a back-end that isn't yaml 2) store information
 about index types etc. in addition to the data frame (pandas itself doesn't do
 this though, which makes us a bit nervous about how hard it could be to do in
 the general case, although specific use cases should be far more tractable and
 easy to test). If you'd like to discuss this more, please raise an issue.
 """
+
 from __future__ import annotations
 
+import warnings
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Any, TypeVar, Union, cast
 
 import cattrs.preconf.pyyaml
 import numpy as np
 import numpy.typing as nptype
@@ -239,40 +241,54 @@
         Returns
         -------
             Unstructured :obj:`pint.UnitRegistry.Quantity`
         """
         if _is_np_scalar(type(inp.magnitude)):
             return (unstructure_np_scalar(inp.magnitude), str(inp.units))
 
-        if isinstance(inp.magnitude, float):
+        if isinstance(inp.magnitude, (float, int)):
             return (inp.magnitude, str(inp.units))
 
         return (unstructure_np_array(inp.magnitude), str(inp.units))
 
     def structure_pint(
         inp: UnstructuredPint, target_type: type[pint.UnitRegistry.Quantity]
     ) -> pint.UnitRegistry.Quantity:
         """
         Structure :obj:`pint.UnitRegistry.Quantity`
 
         Parameters
         ----------
         inp
-            Unstructured data
+            Unstructured data. If this is a string containing a slash,
+            we try and convert it to a fraction but this isn't super safe
+            so we also raise a warning.
 
         target_type
             Type to create
 
         Returns
         -------
             Structured :obj:`pint.UnitRegistry.Quantity`
         """
         # pint not playing nice with mypy
         ur = pint.get_application_registry()  # type: ignore
 
+        if isinstance(inp[0], str) and "/" in inp[0]:
+            msg = (
+                f"Received {inp[0]=}. "
+                "We are assuming that this is meant to be interpreted as a float64. "
+                "It would be safer to put a decimal value into your config, "
+                "or make a merge request to pydoit-nb to make this handling safer."
+            )
+            warnings.warn(msg)
+            toks = inp[0].split("/")
+            mag = np.float64(toks[0]) / float(toks[1])
+            return ur.Quantity(mag, inp[1])  # type: ignore
+
         # Can't do dtype control until pint allows it again with e.g.
         # pint.Quantity[np.array[np.float64]]
         return ur.Quantity(np.array(inp[0]), inp[1])  # type: ignore
 
     def _is_pint(inp: Any) -> bool:
         # I don't love this way of checking, but I couldn't work out how to else to make it work
         return hasattr(inp, "units") & hasattr(inp, "magnitude") & ("pint" in str(inp))
```

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/tasks_copy_source.py` & `pydoit_nb-0.3.4/src/pydoit_nb/tasks_copy_source.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/tasks_generation.py` & `pydoit_nb-0.3.4/src/pydoit_nb/tasks_generation.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/testing.py` & `pydoit_nb-0.3.4/src/pydoit_nb/testing.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/src/pydoit_nb/typing.py` & `pydoit_nb-0.3.4/src/pydoit_nb/typing.py`

 * *Files identical despite different names*

### Comparing `pydoit_nb-0.3.3/PKG-INFO` & `pydoit_nb-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoit-nb
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library to support combining jupyter notebooks and pydoit.
 License: BSD-3-Clause
 Author: Zebedee Nicholls
 Author-email: zebedee.nicholls@climate-resource.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

