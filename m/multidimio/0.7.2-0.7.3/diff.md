# Comparing `tmp/multidimio-0.7.2.tar.gz` & `tmp/multidimio-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidimio-0.7.2.tar", max compression
+gzip compressed data, was "multidimio-0.7.3.tar", max compression
```

## Comparing `multidimio-0.7.2.tar` & `multidimio-0.7.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10203 2024-03-12 16:29:06.948711 multidimio-0.7.2/LICENSE
--rw-r--r--   0        0        0     6028 2024-03-12 16:29:06.948711 multidimio-0.7.2/README.md
--rw-r--r--   0        0        0     2747 2024-03-12 16:29:18.480754 multidimio-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      474 2024-03-12 16:29:06.960712 multidimio-0.7.2/src/mdio/__init__.py
--rw-r--r--   0        0        0     2954 2024-03-12 16:29:06.960712 multidimio-0.7.2/src/mdio/__main__.py
--rw-r--r--   0        0        0      127 2024-03-12 16:29:06.960712 multidimio-0.7.2/src/mdio/api/__init__.py
--rw-r--r--   0        0        0    25195 2024-03-12 16:29:06.960712 multidimio-0.7.2/src/mdio/api/accessor.py
--rw-r--r--   0        0        0     8524 2024-03-12 16:29:06.960712 multidimio-0.7.2/src/mdio/api/convenience.py
--rw-r--r--   0        0        0     4451 2024-03-12 16:29:06.960712 multidimio-0.7.2/src/mdio/api/io_utils.py
--rw-r--r--   0        0        0      105 2024-03-12 16:29:06.960712 multidimio-0.7.2/src/mdio/commands/__init__.py
--rw-r--r--   0        0        0     2246 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/commands/copy.py
--rw-r--r--   0        0        0     5007 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/commands/info.py
--rw-r--r--   0        0        0    14703 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/commands/segy.py
--rw-r--r--   0        0        0      529 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/constants.py
--rw-r--r--   0        0        0      141 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/converters/__init__.py
--rw-r--r--   0        0        0     1485 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/converters/exceptions.py
--rw-r--r--   0        0        0     6510 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/converters/mdio.py
--rw-r--r--   0        0        0    20972 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/converters/segy.py
--rw-r--r--   0        0        0      143 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/core/__init__.py
--rw-r--r--   0        0        0     3811 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/core/dimension.py
--rw-r--r--   0        0        0      268 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/core/exceptions.py
--rw-r--r--   0        0        0     3694 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/core/grid.py
--rw-r--r--   0        0        0     2917 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/core/indexing.py
--rw-r--r--   0        0        0     2727 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/core/serialization.py
--rw-r--r--   0        0        0      429 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/core/utils_write.py
--rw-r--r--   0        0        0     1646 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/py.typed
--rw-r--r--   0        0        0       44 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/__init__.py
--rw-r--r--   0        0        0      636 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/_standards_common.py
--rw-r--r--   0        0        0     9384 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/_standards_rev0.py
--rw-r--r--   0        0        0     8514 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/_workers.py
--rw-r--r--   0        0        0    11128 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/blocked_io.py
--rw-r--r--   0        0        0     2048 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/byte_utils.py
--rw-r--r--   0        0        0     9408 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/creation.py
--rw-r--r--   0        0        0     4856 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/ebcdic.py
--rw-r--r--   0        0        0     1946 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/exceptions.py
--rw-r--r--   0        0        0    23385 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/geometry.py
--rw-r--r--   0        0        0     2748 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/headers.py
--rw-r--r--   0        0        0     3561 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/headers_text.py
--rw-r--r--   0        0        0     1118 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/helpers_segy.py
--rw-r--r--   0        0        0     5785 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/ibm_float.py
--rw-r--r--   0        0        0     4958 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/parsers.py
--rw-r--r--   0        0        0     5532 2024-03-12 16:29:06.964712 multidimio-0.7.2/src/mdio/segy/utilities.py
--rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 multidimio-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    10203 2024-04-04 15:57:28.082587 multidimio-0.7.3/LICENSE
+-rw-r--r--   0        0        0     6028 2024-04-04 15:57:28.082587 multidimio-0.7.3/README.md
+-rw-r--r--   0        0        0     2747 2024-04-04 15:57:37.502619 multidimio-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      474 2024-04-04 15:57:28.094587 multidimio-0.7.3/src/mdio/__init__.py
+-rw-r--r--   0        0        0     2954 2024-04-04 15:57:28.094587 multidimio-0.7.3/src/mdio/__main__.py
+-rw-r--r--   0        0        0      127 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/api/__init__.py
+-rw-r--r--   0        0        0    25195 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/api/accessor.py
+-rw-r--r--   0        0        0     8520 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/api/convenience.py
+-rw-r--r--   0        0        0     4451 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/api/io_utils.py
+-rw-r--r--   0        0        0      105 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/commands/__init__.py
+-rw-r--r--   0        0        0     2246 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/commands/copy.py
+-rw-r--r--   0        0        0     5007 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/commands/info.py
+-rw-r--r--   0        0        0    14703 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/commands/segy.py
+-rw-r--r--   0        0        0      529 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/constants.py
+-rw-r--r--   0        0        0      141 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/converters/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/converters/exceptions.py
+-rw-r--r--   0        0        0     6510 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/converters/mdio.py
+-rw-r--r--   0        0        0    20972 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/converters/segy.py
+-rw-r--r--   0        0        0      143 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/__init__.py
+-rw-r--r--   0        0        0     3811 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/dimension.py
+-rw-r--r--   0        0        0      268 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/exceptions.py
+-rw-r--r--   0        0        0     3694 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/grid.py
+-rw-r--r--   0        0        0     2917 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/indexing.py
+-rw-r--r--   0        0        0     2727 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/serialization.py
+-rw-r--r--   0        0        0      429 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/utils_write.py
+-rw-r--r--   0        0        0     1646 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/py.typed
+-rw-r--r--   0        0        0       44 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/__init__.py
+-rw-r--r--   0        0        0      636 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/_standards_common.py
+-rw-r--r--   0        0        0     9384 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/_standards_rev0.py
+-rw-r--r--   0        0        0     8514 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/_workers.py
+-rw-r--r--   0        0        0    11128 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/blocked_io.py
+-rw-r--r--   0        0        0     2048 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/byte_utils.py
+-rw-r--r--   0        0        0     9408 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/creation.py
+-rw-r--r--   0        0        0     4856 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/ebcdic.py
+-rw-r--r--   0        0        0     1946 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/exceptions.py
+-rw-r--r--   0        0        0    23385 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/geometry.py
+-rw-r--r--   0        0        0     2748 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/headers.py
+-rw-r--r--   0        0        0     3561 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/headers_text.py
+-rw-r--r--   0        0        0     1118 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/helpers_segy.py
+-rw-r--r--   0        0        0     5785 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/ibm_float.py
+-rw-r--r--   0        0        0     4958 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/parsers.py
+-rw-r--r--   0        0        0     5532 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/utilities.py
+-rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 multidimio-0.7.3/PKG-INFO
```

### Comparing `multidimio-0.7.2/LICENSE` & `multidimio-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/README.md` & `multidimio-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/pyproject.toml` & `multidimio-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidimio"
-version = "0.7.2"
+version = "0.7.3"
 description = "Cloud-native, scalable, and user-friendly multi dimensional energy data!"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
@@ -26,15 +26,15 @@
 python = ">=3.9,<3.13"
 click = "^8.1.7"
 click-params = "^0.5.0"
 zarr = "^2.16.1"
 dask = ">=2023.10.0"
 tqdm = "^4.66.1"
 segyio = "^1.9.3"
-numba = "^0.59.0"
+numba = "^0.59.1"
 psutil = "^5.9.5"
 fsspec = ">=2023.9.1"
 rich = "^13.7.1"
 urllib3 = "^1.26.18" # Workaround for poetry-plugin-export/issues/183
 
 # Extras
 distributed = {version = ">=2023.10.0", optional = true}
```

### Comparing `multidimio-0.7.2/src/mdio/__main__.py` & `multidimio-0.7.3/src/mdio/__main__.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/api/accessor.py` & `multidimio-0.7.3/src/mdio/api/accessor.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/api/convenience.py` & `multidimio-0.7.3/src/mdio/api/convenience.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,14 +160,16 @@
                 chunks=norm_chunks,
                 compressor=trace_compressor,
                 overwrite=overwrite,
                 **CREATE_KW,
             )
         )
 
+    zarr.consolidate_metadata(source.store)
+
     n_dimension = len(data_array.shape)
     dummy_array = zarr.empty_like(data_array, chunks=(MAX_BUFFER,) * n_dimension)
     iterator = ChunkIterator(dummy_array)
 
     return metadata_arrs, data_arrs, live_mask, iterator
 
 
@@ -198,16 +200,14 @@
 
         for array in metadata_arrs_out:
             array[meta_slice] = source._headers[meta_slice]
 
         for array in data_arrs_out:
             array[slice_] = source._traces[slice_]
 
-        zarr.consolidate_metadata(source.store)
-
 
 def rechunk_batch(
     source: MDIOAccessor,
     chunks_list: list[tuple[int, ...]],
     suffix_list: list[str],
     compressor: Codec | None = None,
     overwrite: bool = False,
```

### Comparing `multidimio-0.7.2/src/mdio/api/io_utils.py` & `multidimio-0.7.3/src/mdio/api/io_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/commands/copy.py` & `multidimio-0.7.3/src/mdio/commands/copy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/commands/info.py` & `multidimio-0.7.3/src/mdio/commands/info.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/commands/segy.py` & `multidimio-0.7.3/src/mdio/commands/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/constants.py` & `multidimio-0.7.3/src/mdio/constants.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/converters/exceptions.py` & `multidimio-0.7.3/src/mdio/converters/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/converters/mdio.py` & `multidimio-0.7.3/src/mdio/converters/mdio.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/converters/segy.py` & `multidimio-0.7.3/src/mdio/converters/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/core/dimension.py` & `multidimio-0.7.3/src/mdio/core/dimension.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/core/grid.py` & `multidimio-0.7.3/src/mdio/core/grid.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/core/indexing.py` & `multidimio-0.7.3/src/mdio/core/indexing.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/core/serialization.py` & `multidimio-0.7.3/src/mdio/core/serialization.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/exceptions.py` & `multidimio-0.7.3/src/mdio/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/_standards_common.py` & `multidimio-0.7.3/src/mdio/segy/_standards_common.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/_standards_rev0.py` & `multidimio-0.7.3/src/mdio/segy/_standards_rev0.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/_workers.py` & `multidimio-0.7.3/src/mdio/segy/_workers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/blocked_io.py` & `multidimio-0.7.3/src/mdio/segy/blocked_io.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/byte_utils.py` & `multidimio-0.7.3/src/mdio/segy/byte_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/creation.py` & `multidimio-0.7.3/src/mdio/segy/creation.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/ebcdic.py` & `multidimio-0.7.3/src/mdio/segy/ebcdic.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/exceptions.py` & `multidimio-0.7.3/src/mdio/segy/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/geometry.py` & `multidimio-0.7.3/src/mdio/segy/geometry.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/headers.py` & `multidimio-0.7.3/src/mdio/segy/headers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/headers_text.py` & `multidimio-0.7.3/src/mdio/segy/headers_text.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/helpers_segy.py` & `multidimio-0.7.3/src/mdio/segy/helpers_segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/ibm_float.py` & `multidimio-0.7.3/src/mdio/segy/ibm_float.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/parsers.py` & `multidimio-0.7.3/src/mdio/segy/parsers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/src/mdio/segy/utilities.py` & `multidimio-0.7.3/src/mdio/segy/utilities.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.2/PKG-INFO` & `multidimio-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidimio
-Version: 0.7.2
+Version: 0.7.3
 Summary: Cloud-native, scalable, and user-friendly multi dimensional energy data!
 Home-page: https://mdio.dev
 License: Apache-2.0
 Keywords: mdio,multidimio,seismic,wind,data
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
@@ -24,15 +24,15 @@
 Requires-Dist: bokeh (>=3.2.2,<4.0.0) ; extra == "distributed"
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: click-params (>=0.5.0,<0.6.0)
 Requires-Dist: dask (>=2023.10.0)
 Requires-Dist: distributed (>=2023.10.0) ; extra == "distributed"
 Requires-Dist: fsspec (>=2023.9.1)
 Requires-Dist: gcsfs (>=2023.5.0) ; extra == "cloud"
-Requires-Dist: numba (>=0.59.0,<0.60.0)
+Requires-Dist: numba (>=0.59.1,<0.60.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: s3fs (>=2023.5.0) ; extra == "cloud"
 Requires-Dist: segyio (>=1.9.3,<2.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Requires-Dist: zarr (>=2.16.1,<3.0.0)
```

