# Comparing `tmp/pynxtools-mpes-0.0.1.tar.gz` & `tmp/pynxtools-mpes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynxtools-mpes-0.0.1.tar", last modified: Tue Feb 20 15:38:56 2024, max compression
+gzip compressed data, was "pynxtools-mpes-0.0.2.tar", last modified: Thu Apr  4 05:52:37 2024, max compression
```

## Comparing `pynxtools-mpes-0.0.1.tar` & `pynxtools-mpes-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:56.596273 pynxtools-mpes-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:56.580273 pynxtools-mpes-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:56.584273 pynxtools-mpes-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:56.584273 pynxtools-mpes-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-20 15:38:56.596273 pynxtools-mpes-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:56.584273 pynxtools-mpes-0.0.1/pynxtools_mpes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/pynxtools_mpes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/pynxtools_mpes/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:56.596273 pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-20 15:38:56.000000 pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-20 15:38:56.000000 pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 15:38:56.000000 pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-20 15:38:56.000000 pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-20 15:38:56.000000 pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-20 15:38:56.000000 pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 15:38:56.596273 pynxtools-mpes-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:56.584273 pynxtools-mpes-0.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:38:56.584273 pynxtools-mpes-0.0.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/tests/data/ELN_metadata_example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/tests/data/config_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/tests/data/eln_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)  6533728 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/tests/data/xarray_saved_small_calibration.h5
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-20 15:38:45.000000 pynxtools-mpes-0.0.1/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.689643 pynxtools-mpes-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.673642 pynxtools-mpes-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 05:52:37.689643 pynxtools-mpes-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/pynxtools_mpes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/pynxtools_mpes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/pynxtools_mpes/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.685643 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:52:37.689643 pynxtools-mpes-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   310749 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/data/Ref_nexus_mpes.log
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/data/config_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/data/eln_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)  6533728 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/data/xarray_saved_small_calibration.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/test_reader.py
```

### Comparing `pynxtools-mpes-0.0.1/.github/workflows/publish.yml` & `pynxtools-mpes-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.1/.github/workflows/pylint.yml` & `pynxtools-mpes-0.0.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.1/.github/workflows/pytest.yml` & `pynxtools-mpes-0.0.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.1/.gitignore` & `pynxtools-mpes-0.0.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -199,8 +199,9 @@
 .pyenv
 *.pyc
 *.txt
 !requirements.txt
 !dev-requirements.txt
 build/
 nexusparser.egg-info/PKG-INFO
-.python-version
+.python-version
+!tests/data/Ref_nexus_mpes.log
```

### Comparing `pynxtools-mpes-0.0.1/PKG-INFO` & `pynxtools-mpes-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-mpes
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Florian Dobener <florian.dobener@physik.hu-berlin.de>, Abeer Aurora <arora@fhi-berlin.mpg.de>, Laurenz Rettig <rettig@fhi-berlin.mpg.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/FAIRmat-NFDI/pynxtools-mpes
 Project-URL: Bug Tracker, https://github.com/FAIRmat-NFDI/pynxtools-mpes/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pynxtools-mpes-0.0.1/dev-requirements.txt` & `pynxtools-mpes-0.0.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.1/pynxtools_mpes/reader.py` & `pynxtools-mpes-0.0.2/pynxtools_mpes/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """MPES reader implementation for the DataConverter."""
 import errno
 import os
 from functools import reduce
-from typing import Any, Tuple
+from typing import Any, Tuple, Union
 
 import h5py
+import numpy as np
 import xarray as xr
 import yaml
 from pynxtools.dataconverter.readers.base.reader import BaseReader
 from pynxtools.dataconverter.readers.utils import (
     FlattenSettings,
     flatten_and_replace,
     parse_flatten_json,
@@ -45,106 +46,116 @@
     "timeStamp": "s",
     "energy": "eV",
     "kx": "1/A",
     "ky": "1/A",
 }
 
 
-def res_to_xarray(res, bin_names, bin_axes, metadata=None):
-    """creates a BinnedArray (xarray subclass) out of the given np.array
-    Parameters:
-        res: np.array
-            nd array of binned data
-        bin_names (list): list of names of the binned axes
-        bin_axes (list): list of np.arrays with the values of the axes
+def recursive_parse_metadata(
+    node: Union[h5py.Group, h5py.Dataset],
+) -> dict:
+    """Recurses through an hdf5 file, and parse it into a dictionary.
+
+    Args:
+        node (Union[h5py.Group, h5py.Dataset]): hdf5 group or dataset to parse into
+            dictionary.
+
     Returns:
-        ba: BinnedArray (xarray)
-            an xarray-like container with binned data, axis, and all
-            available metadata
+        dict: Dictionary of elements in the hdf5 path contained in node
     """
-    dims = bin_names
-    coords = {}
-    for name, vals in zip(bin_names, bin_axes):
-        coords[name] = vals
+    if isinstance(node, h5py.Group):
+        dictionary = {}
+        for key, value in node.items():
+            dictionary[key] = recursive_parse_metadata(value)
 
-    xres = xr.DataArray(res, dims=dims, coords=coords)
-
-    for name in bin_names:
+    else:
+        entry = node[...]
         try:
-            xres[name].attrs["unit"] = DEFAULT_UNITS[name]
-        except KeyError:
-            pass
-
-    xres.attrs["units"] = "counts"
-    xres.attrs["long_name"] = "photoelectron counts"
+            dictionary = entry.item()
+            if isinstance(dictionary, (bytes, bytearray)):
+                dictionary = dictionary.decode()
+        except ValueError:
+            dictionary = entry
 
-    if metadata is not None:
-        xres.attrs["metadata"] = metadata
+    return dictionary
 
-    return xres
 
+def h5_to_xarray(faddr: str, mode: str = "r") -> xr.DataArray:
+    """Read xarray data from formatted hdf5 file
 
-def h5_to_xarray(faddr, mode="r"):
-    """Rear xarray data from formatted hdf5 file
     Args:
         faddr (str): complete file name (including path)
-        mode (str): hdf5 read/write mode
+        mode (str, optional): hdf5 read/write mode. Defaults to "r".
+
+    Raises:
+        ValueError: Raised if data or axes are not found in the file.
+
     Returns:
-        xarray (xarray.DataArray): output xarra data
+        xr.DataArray: output xarra data
     """
     with h5py.File(faddr, mode) as h5_file:
         # Reading data array
         try:
-            data = h5_file["binned"]["BinnedData"]
-        except KeyError:
-            print("Wrong Data Format, data not found")
-            raise
+            data = np.asarray(h5_file["binned"]["BinnedData"])
+        except KeyError as exc:
+            raise ValueError(
+                f"Wrong Data Format, the BinnedData was not found.",
+            ) from exc
 
         # Reading the axes
-        axes = []
+        bin_axes = []
         bin_names = []
 
         try:
             for axis in h5_file["axes"]:
-                axes.append(h5_file["axes"][axis])
+                bin_axes.append(h5_file["axes"][axis])
                 bin_names.append(h5_file["axes"][axis].attrs["name"])
-        except KeyError:
-            print("Wrong Data Format, axes not found")
-            raise
+        except KeyError as exc:
+            raise ValueError(
+                f"Wrong Data Format, the axes were not found.",
+            ) from exc
 
         # load metadata
+        metadata = None
         if "metadata" in h5_file:
-
-            def recursive_parse_metadata(node):
-                if isinstance(node, h5py.Group):
-                    dictionary = {}
-                    for key, value in node.items():
-                        dictionary[key] = recursive_parse_metadata(value)
-
-                else:
-                    dictionary = node[...]
-                    try:
-                        dictionary = dictionary.item()
-                        if isinstance(dictionary, (bytes, bytearray)):
-                            dictionary = dictionary.decode()
-                    except ValueError:
-                        pass
-
-                return dictionary
-
             metadata = recursive_parse_metadata(h5_file["metadata"])
+
         # Segment to change Vset to V in lens voltages
         if "file" in metadata.keys():
             for k in list(metadata["file"]):
                 if "VSet" in k:
                     key = k[:-3]
                     metadata["file"][key] = metadata["file"][k]
                     del metadata["file"][k]
 
-        xarray = res_to_xarray(data, bin_names, axes, metadata)
+        coords = {}
+        for name, vals in zip(bin_names, bin_axes):
+            coords[name] = vals
+
+        xarray = xr.DataArray(data, dims=bin_names, coords=coords)
+
+        for axis in range(len(bin_axes)):
+            try:
+                xarray[bin_names[axis]].attrs["unit"] = h5_file["axes"][
+                    f"ax{axis}"
+                ].attrs["unit"]
+            except (KeyError, TypeError):
+                xarray[bin_names[axis]].attrs["unit"] = DEFAULT_UNITS[bin_names[axis]]
+        try:
+            xarray.attrs["units"] = h5_file["binned"]["BinnedData"].attrs["units"]
+            xarray.attrs["long_name"] = h5_file["binned"]["BinnedData"].attrs[
+                "long_name"
+            ]
+        except (KeyError, TypeError):
+            xarray.attrs["units"] = "counts"
+            xarray.attrs["long_name"] = "photoelectron counts"
+
+        if metadata is not None:
+            xarray.attrs["metadata"] = metadata
+
         return xarray
 
 
 def iterate_dictionary(dic, key_string):
     """Recursively iterate in dictionary and give back its values"""
     keys = key_string.split("/", 1)
     if keys[0] in dic:
@@ -175,15 +186,15 @@
 
 REPLACE_NESTED = {
     "SAMPLE[sample]/chemical_formula": "SAMPLE[sample]/SUBSTANCE[substance]/molecular_formula_hill",
     "source_TYPE[source]/Probe": "source_TYPE[source_probe]",
     "source_TYPE[source]/Pump": "source_TYPE[source_pump]",
     "beam_TYPE[beam]/Probe": "beam_TYPE[beam_probe]",
     "beam_TYPE[beam]/Pump": "beam_TYPE[beam_pump]",
-    "sample_history": "sample_history/notes/description",
+    "sample_history": "sample_history/notes",
     "ELECTRONANALYSER[electronanalyser]/RESOLUTION[momentum_resolution]": (
         "ELECTRONANALYSER[electronanalyser]/momentum_resolution"
     ),
     "ELECTRONANALYSER[electronanalyser]/RESOLUTION[spatial_resolution]": (
         "ELECTRONANALYSER[electronanalyser]/spatial_resolution"
     ),
     "SAMPLE[sample]/gas_pressure": "INSTRUMENT[instrument]/pressure_gauge/value",
@@ -283,15 +294,15 @@
 
 class MPESReader(BaseReader):
     """MPES-specific reader class"""
 
     # pylint: disable=too-few-public-methods
 
     # Whitelist for the NXDLs that the reader supports and can process
-    supported_nxdls = ["NXmpes"]
+    supported_nxdls = ["NXmpes", "NXmpes_arpes"]
 
     def read(  # pylint: disable=too-many-branches
         self,
         template: dict = None,
         file_paths: Tuple[str] = None,
         objects: Tuple[Any] = None,
     ) -> dict:
@@ -346,14 +357,18 @@
 
                         except KeyError:
                             print(
                                 f"[info]: Path {key} not found. "
                                 f"Skipping the entry.",
                             )
 
+                if isinstance(template.get(key), str) and template[key].startswith(
+                    "@link:"
+                ):
+                    template[key] = {"link": template[key][6:]}
             else:
                 # Fills in the fixed metadata
                 template[key] = value
 
         # Filling in ELN metadata and overwriting the common paths by
         # giving preference to the ELN metadata
         for key, value in eln_data_dict.items():
```

### Comparing `pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/PKG-INFO` & `pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-mpes
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Florian Dobener <florian.dobener@physik.hu-berlin.de>, Abeer Aurora <arora@fhi-berlin.mpg.de>, Laurenz Rettig <rettig@fhi-berlin.mpg.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/FAIRmat-NFDI/pynxtools-mpes
 Project-URL: Bug Tracker, https://github.com/FAIRmat-NFDI/pynxtools-mpes/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pynxtools-mpes-0.0.1/pynxtools_mpes.egg-info/SOURCES.txt` & `pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 pynxtools_mpes.egg-info/PKG-INFO
 pynxtools_mpes.egg-info/SOURCES.txt
 pynxtools_mpes.egg-info/dependency_links.txt
 pynxtools_mpes.egg-info/entry_points.txt
 pynxtools_mpes.egg-info/requires.txt
 pynxtools_mpes.egg-info/top_level.txt
 tests/test_reader.py
-tests/data/ELN_metadata_example.yaml
+tests/data/Ref_nexus_mpes.log
 tests/data/config_file.json
 tests/data/eln_data.yaml
 tests/data/xarray_saved_small_calibration.h5
```

### Comparing `pynxtools-mpes-0.0.1/pyproject.toml` & `pynxtools-mpes-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 mpes = "pynxtools_mpes.reader:MPESReader"
 
 [tool.setuptools_scm]
 version_scheme = "no-guess-dev"
 local_scheme = "node-and-date"
 
 [tool.ruff]
-include = ["pynxtools/*.py", "tests/*.py"]
+include = ["pynxtools_mpes/*.py", "tests/*.py"]
 select = [
     "E", # pycodestyle
     "W", # pycodestyle
     "PL", # pylint
 ]
 ignore = [
     "E501", # Line too long ({width} > {limit} characters)
```

### Comparing `pynxtools-mpes-0.0.1/tests/data/config_file.json` & `pynxtools-mpes-0.0.2/tests/data/config_file.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930495936355311%*

 * *Differences: {"'/ENTRY[entry]/INSTRUMENT[instrument]'": "{'RESOLUTION[momentum_resolution]': {'resolution': "*

 * *                                           "'@link:/entry/instrument/electronanalyser/momentum_resolution'}}",*

 * * "'/ENTRY[entry]/INSTRUMENT[instrument]/beam_TYPE[beam_probe]'": "{'associated_source': "*

 * *                                                                 "'/entry/instrument/source_probe'}",*

 * * "'/ENTRY[entry]/INSTRUMENT[instrument]/beam_TYPE[beam_pump]'": "{'associated_source': "*

 * *                        […]*

```diff
@@ -52,15 +52,15 @@
                 "resolution": "@attrs:metadata/instrument/analyzer/spatial_resolution",
                 "resolution/@units": "\u00b5m",
                 "type": "estimated"
             }
         },
         "RESOLUTION[momentum_resolution]": {
             "physical_quantity": "momentum",
-            "resolution": "@attrs:metadata/instrument/analyzer/momentum_resolution",
+            "resolution": "@link:/entry/instrument/electronanalyser/momentum_resolution",
             "resolution/@units": "1/angstrom",
             "type": "estimated"
         },
         "RESOLUTION[temporal_resolution]": {
             "physical_quantity": "time",
             "resolution": 35.0,
             "resolution/@units": "fs",
@@ -181,30 +181,30 @@
             "measurement": "temperature",
             "name": "sample_temperature",
             "value": "@attrs:metadata/file/trARPES:Carving:TEMP_RBV",
             "value/@units": "K"
         }
     },
     "/ENTRY[entry]/INSTRUMENT[instrument]/beam_TYPE[beam_probe]": {
-        "associated_source": "@link:/entry/instrument/source_probe",
+        "associated_source": "/entry/instrument/source_probe",
         "distance": 0.0,
         "distance/@units": "mm",
         "extent": "@attrs:metadata/instrument/beam/probe/extent",
         "extent/@units": "\u00b5m",
         "incident_energy": "@attrs:metadata/instrument/beam/probe/incident_energy",
         "incident_energy/@units": "eV",
         "incident_energy_spread": "@attrs:metadata/instrument/beam/probe/incident_energy_spread",
         "incident_energy_spread/@units": "eV",
         "incident_polarization": "@attrs:metadata/instrument/beam/probe/incident_polarization",
         "incident_polarization/@units": "V^2/mm^2",
         "pulse_duration": "@attrs:metadata/instrument/beam/probe/pulse_duration",
         "pulse_duration/@units": "fs"
     },
     "/ENTRY[entry]/INSTRUMENT[instrument]/beam_TYPE[beam_pump]": {
-        "associated_source": "@link:/entry/instrument/source_pump",
+        "associated_source": "/entry/instrument/source_pump",
         "average_power": "@attrs:metadata/instrument/beam/pump/average_power",
         "average_power/@units": "mW",
         "distance": 0.0,
         "distance/@units": "mm",
         "extent": "@attrs:metadata/instrument/beam/pump/extent",
         "extent/@units": "\u00b5m",
         "fluence": "@attrs:metadata/instrument/beam/pump/fluence",
@@ -219,24 +219,24 @@
         "incident_wavelength/@units": "nm",
         "pulse_duration": "@attrs:metadata/instrument/beam/pump/pulse_duration",
         "pulse_duration/@units": "fs",
         "pulse_energy": "@attrs:metadata/instrument/beam/pump/pulse_energy",
         "pulse_energy/@units": "\u00b5J"
     },
     "/ENTRY[entry]/INSTRUMENT[instrument]/source_TYPE[source_probe]": {
-        "associated_beam": "@link:/entry/instrument/beam_probe",
+        "associated_beam": "/entry/instrument/beam_probe",
         "frequency": "@attrs:metadata/instrument/beam/probe/frequency",
         "frequency/@units": "kHz",
         "mode": "Single Bunch",
         "name": "HHG @ TR-ARPES @ FHI",
         "probe": "photon",
         "type": "HHG laser"
     },
     "/ENTRY[entry]/INSTRUMENT[instrument]/source_TYPE[source_pump]": {
-        "associated_beam": "@link:/entry/instrument/beam_pump",
+        "associated_beam": "/entry/instrument/beam_pump",
         "frequency": "@attrs:metadata/instrument/beam/pump/frequency",
         "frequency/@units": "kHz",
         "mode": "Single Bunch",
         "name": "OPCPA @ TR-ARPES @ FHI",
         "probe": "visible light",
         "type": "Optical Laser"
     },
@@ -357,16 +357,15 @@
         "depends_on": "/entry/sample/transformations/corrected_phi",
         "description": "@attrs:metadata/sample/chemical_formula",
         "gas_pressure": {
             "pressure_gauge": "@link:/entry/instrument/pressure_gauge"
         },
         "name": "@attrs:metadata/sample/chemical_formula",
         "preparation_date": "@attrs:metadata/sample/preparation_date",
-        "sample_history/notes/description": "@attrs:metadata/sample/sample_history",
-        "sample_history/notes/type": "text/plain",
+        "sample_history/notes": "@attrs:metadata/sample/sample_history",
         "situation": "vacuum",
         "temperature": {
             "temperature_sensor": "@link:/entry/instrument/manipulator/temperature_sensor"
         }
     },
     "/ENTRY[entry]/USER[user]": {
         "address": "@attrs:metadata/user0/address",
```

### Comparing `pynxtools-mpes-0.0.1/tests/data/eln_data.yaml` & `pynxtools-mpes-0.0.2/tests/data/eln_data.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -23,22 +23,22 @@
   Manipulator:
     sample_temperature:
       unit: K
       value: 300.0
   Source:
     Probe:
       frequency:
-        unit: kHz
+        unit: KHz
         value: 500.0
       photon_energy:
         unit: eV
         value: 21.7
     Pump:
       frequency:
-        unit: kHz
+        unit: KHz
         value: 500.0
       photon_energy:
         unit: eV
         value: 1.55
   Beam:
     Probe:
       extent:
```

### Comparing `pynxtools-mpes-0.0.1/tests/data/xarray_saved_small_calibration.h5` & `pynxtools-mpes-0.0.2/tests/data/xarray_saved_small_calibration.h5`

 * *Files identical despite different names*

