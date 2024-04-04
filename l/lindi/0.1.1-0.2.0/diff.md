# Comparing `tmp/lindi-0.1.1.tar.gz` & `tmp/lindi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.1.1.tar", max compression
+gzip compressed data, was "lindi-0.2.0.tar", max compression
```

## Comparing `lindi-0.1.1.tar` & `lindi-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.1.1/LICENSE
--rw-r--r--   0        0        0     3558 2024-03-21 19:32:30.025441 lindi-0.1.1/README.md
--rw-r--r--   0        0        0     1501 2024-03-21 19:32:30.025441 lindi-0.1.1/lindi/LindiH5ZarrStore/FloatJsonEncoder.py
--rw-r--r--   0        0        0    24641 2024-03-21 19:32:30.025441 lindi-0.1.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      136 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     4626 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5ZarrStore/_h5_attr_to_zarr_attr.py
--rw-r--r--   0        0        0     2440 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5ZarrStore/_h5_filters_to_codecs.py
--rw-r--r--   0        0        0     1939 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     1204 2024-03-21 19:32:30.025441 lindi-0.1.1/lindi/LindiH5ZarrStore/_utils.py
--rw-r--r--   0        0        0     9314 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5ZarrStore/_zarr_info_for_h5_dataset.py
--rw-r--r--   0        0        0     3709 2024-03-21 18:16:58.794258 lindi-0.1.1/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py
--rw-r--r--   0        0        0     1045 2024-03-21 18:16:58.794258 lindi-0.1.1/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py
--rw-r--r--   0        0        0        0 2024-03-21 18:16:58.794258 lindi-0.1.1/lindi/LindiH5pyFile/FileSegmentReader/__init__.py
--rw-r--r--   0        0        0     3072 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    10718 2024-03-21 18:16:58.794258 lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0     8155 2024-03-21 18:16:58.794258 lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     5243 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      454 2024-03-21 18:11:00.739060 lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0     5959 2024-03-21 18:16:58.794258 lindi-0.1.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      210 2024-03-21 11:16:09.352672 lindi-0.1.1/lindi/__init__.py
--rw-r--r--   0        0        0      454 2024-03-21 19:32:48.441190 lindi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 lindi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3557 2024-04-04 18:54:34.995198 lindi-0.2.0/README.md
+-rw-r--r--   0        0        0     1501 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/FloatJsonEncoder.py
+-rw-r--r--   0        0        0    24641 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      136 2024-03-21 11:16:09.352672 lindi-0.2.0/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     4626 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_h5_attr_to_zarr_attr.py
+-rw-r--r--   0        0        0     2440 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     1939 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     1204 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_utils.py
+-rw-r--r--   0        0        0     9314 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5ZarrStore/_zarr_info_for_h5_dataset.py
+-rw-r--r--   0        0        0     3709 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py
+-rw-r--r--   0        0        0     1045 2024-03-21 18:16:58.794258 lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:16:58.794258 lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    10718 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0     8155 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     5243 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      454 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0     5959 2024-04-04 18:54:34.995198 lindi-0.2.0/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.2.0/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      210 2024-03-21 11:16:09.352672 lindi-0.2.0/lindi/__init__.py
+-rw-r--r--   0        0        0      625 2024-04-04 18:54:46.263044 lindi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 lindi-0.2.0/PKG-INFO
```

### Comparing `lindi-0.1.1/LICENSE` & `lindi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/README.md` & `lindi-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 - A function for generating a reference file system .zarr.json file from a Zarr store. This is inspired by [kerchunk](https://github.com/fsspec/kerchunk).
 - An h5py-like interface for accessing these Zarr stores that can be used with [pynwb](https://pynwb.readthedocs.io/en/stable/).
 
 This project was inspired by [kerchunk](https://github.com/fsspec/kerchunk) and [hdmf-zarr](https://hdmf-zarr.readthedocs.io/en/latest/index.html) and depends on [zarr](https://zarr.readthedocs.io/en/stable/), [h5py](https://www.h5py.org/), [remfile](https://github.com/magland/remfile) and [numcodecs](https://numcodecs.readthedocs.io/en/stable/).
 
 ## Installation
 
-For now, install from source. Clone this repo and then
+```bash
+pip install lindi
+```
+
+Or install from source
 
 ```bash
 cd lindi
 pip install -e .
 ```
 
 ## Example usage
```

### Comparing `lindi-0.1.1/lindi/LindiH5ZarrStore/FloatJsonEncoder.py` & `lindi-0.2.0/lindi/LindiH5ZarrStore/FloatJsonEncoder.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.2.0/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,27 +436,27 @@
         elif isinstance(item, h5py.Dataset):
             # Datasets do not have subdirectories
             return []
         else:
             return []
 
     def to_file(self, file_name: str, *, file_type: Literal["zarr.json"] = "zarr.json"):
-        """Write a reference file system cooresponding to this store to a file.
+        """Write a reference file system corresponding to this store to a file.
 
         This can then be loaded using LindiH5pyFile.from_reference_file_system(file_name)
         """
         if file_type != "zarr.json":
             raise Exception(f"Unsupported file type: {file_type}")
 
         ret = self.to_reference_file_system()
         with open(file_name, "w") as f:
             json.dump(ret, f, indent=2)
 
     def to_reference_file_system(self) -> dict:
-        """Create a reference file system cooresponding to this store.
+        """Create a reference file system corresponding to this store.
 
         This can then be loaded using LindiH5pyFile.from_reference_file_system(obj)
         """
         if self._h5f is None:
             raise Exception("Store is closed")
         if self._url is None:
             raise Exception("You must specify a url to create a reference file system")
```

### Comparing `lindi-0.1.1/lindi/LindiH5ZarrStore/_h5_attr_to_zarr_attr.py` & `lindi-0.2.0/lindi/LindiH5ZarrStore/_h5_attr_to_zarr_attr.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5ZarrStore/_h5_filters_to_codecs.py` & `lindi-0.2.0/lindi/LindiH5ZarrStore/_h5_filters_to_codecs.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.2.0/lindi/LindiH5ZarrStore/_util.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5ZarrStore/_utils.py` & `lindi-0.2.0/lindi/LindiH5ZarrStore/_utils.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5ZarrStore/_zarr_info_for_h5_dataset.py` & `lindi-0.2.0/lindi/LindiH5ZarrStore/_zarr_info_for_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py` & `lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py` & `lindi-0.2.0/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyFile.py` & `lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyFile.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5pyFile/LindiH5pyGroup.py` & `lindi-0.2.0/lindi/LindiH5pyFile/LindiH5pyGroup.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py` & `lindi-0.2.0/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.1.1/PKG-INFO` & `lindi-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lindi
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -33,15 +33,19 @@
 - A function for generating a reference file system .zarr.json file from a Zarr store. This is inspired by [kerchunk](https://github.com/fsspec/kerchunk).
 - An h5py-like interface for accessing these Zarr stores that can be used with [pynwb](https://pynwb.readthedocs.io/en/stable/).
 
 This project was inspired by [kerchunk](https://github.com/fsspec/kerchunk) and [hdmf-zarr](https://hdmf-zarr.readthedocs.io/en/latest/index.html) and depends on [zarr](https://zarr.readthedocs.io/en/stable/), [h5py](https://www.h5py.org/), [remfile](https://github.com/magland/remfile) and [numcodecs](https://numcodecs.readthedocs.io/en/stable/).
 
 ## Installation
 
-For now, install from source. Clone this repo and then
+```bash
+pip install lindi
+```
+
+Or install from source
 
 ```bash
 cd lindi
 pip install -e .
 ```
 
 ## Example usage
```

