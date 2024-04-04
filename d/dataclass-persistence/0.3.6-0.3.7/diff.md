# Comparing `tmp/dataclass-persistence-0.3.6.tar.gz` & `tmp/dataclass-persistence-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass-persistence-0.3.6.tar", last modified: Fri Mar 22 14:31:01 2024, max compression
+gzip compressed data, was "dataclass-persistence-0.3.7.tar", last modified: Thu Apr  4 12:50:09 2024, max compression
```

## Comparing `dataclass-persistence-0.3.6.tar` & `dataclass-persistence-0.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 14:31:01.288483 dataclass-persistence-0.3.6/
--rw-rw-rw-   0        0        0     1084 2023-11-03 14:01:11.000000 dataclass-persistence-0.3.6/LICENSE
--rw-rw-rw-   0        0        0     1957 2024-03-22 14:31:01.288483 dataclass-persistence-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     1295 2023-11-03 14:01:11.000000 dataclass-persistence-0.3.6/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-22 14:31:01.277480 dataclass-persistence-0.3.6/dataclass_persistence/
--rw-rw-rw-   0        0        0       74 2023-11-03 14:01:11.000000 dataclass-persistence-0.3.6/dataclass_persistence/__init__.py
--rw-rw-rw-   0        0        0    30666 2024-03-22 14:26:51.000000 dataclass-persistence-0.3.6/dataclass_persistence/core.py
-drwxrwxrwx   0        0        0        0 2024-03-22 14:31:01.287485 dataclass-persistence-0.3.6/dataclass_persistence.egg-info/
--rw-rw-rw-   0        0        0     1957 2024-03-22 14:31:01.000000 dataclass-persistence-0.3.6/dataclass_persistence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2024-03-22 14:31:01.000000 dataclass-persistence-0.3.6/dataclass_persistence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 14:31:01.000000 dataclass-persistence-0.3.6/dataclass_persistence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-22 14:31:01.000000 dataclass-persistence-0.3.6/dataclass_persistence.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-22 14:31:01.000000 dataclass-persistence-0.3.6/dataclass_persistence.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 14:31:01.289482 dataclass-persistence-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     5171 2024-03-22 14:27:14.000000 dataclass-persistence-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:50:09.825892 dataclass-persistence-0.3.7/
+-rw-rw-rw-   0        0        0     1084 2023-11-03 14:01:11.000000 dataclass-persistence-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     1957 2024-04-04 12:50:09.825892 dataclass-persistence-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1295 2023-11-03 14:01:11.000000 dataclass-persistence-0.3.7/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-04 12:50:09.813758 dataclass-persistence-0.3.7/dataclass_persistence/
+-rw-rw-rw-   0        0        0       74 2023-11-03 14:01:11.000000 dataclass-persistence-0.3.7/dataclass_persistence/__init__.py
+-rw-rw-rw-   0        0        0    30753 2024-04-04 12:44:59.000000 dataclass-persistence-0.3.7/dataclass_persistence/core.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:50:09.824892 dataclass-persistence-0.3.7/dataclass_persistence.egg-info/
+-rw-rw-rw-   0        0        0     1957 2024-04-04 12:50:09.000000 dataclass-persistence-0.3.7/dataclass_persistence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-04-04 12:50:09.000000 dataclass-persistence-0.3.7/dataclass_persistence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:50:09.000000 dataclass-persistence-0.3.7/dataclass_persistence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 12:50:09.000000 dataclass-persistence-0.3.7/dataclass_persistence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-04 12:50:09.000000 dataclass-persistence-0.3.7/dataclass_persistence.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:50:09.825892 dataclass-persistence-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     5171 2024-04-04 12:34:45.000000 dataclass-persistence-0.3.7/setup.py
```

### Comparing `dataclass-persistence-0.3.6/LICENSE` & `dataclass-persistence-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass-persistence-0.3.6/PKG-INFO` & `dataclass-persistence-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-persistence
-Version: 0.3.6
+Version: 0.3.7
 Summary: Persists information contained in dataclasses.
 Home-page: https://github.com/philipp-mohr/dataclass-persistence
 Author: P.Mohr
 Author-email: philipp.mohr@tuhh.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `dataclass-persistence-0.3.6/README.rst` & `dataclass-persistence-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `dataclass-persistence-0.3.6/dataclass_persistence/core.py` & `dataclass-persistence-0.3.7/dataclass_persistence/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,22 +305,22 @@
     dtype: str
 
     @classmethod
     def from_array(self, array: np.ndarray):
         return NumpyJson(list(array.tolist()), str(array.dtype))
 
 
-def numpy_dict_to_zip_file(file, dict_heavy):
+def numpy_dict_to_zip_file(file, dict_heavy, compresslevel=2):
     """
     https://stackoverflow.com/questions/40886234/how-to-directly-add-file-to-zip-in-python
     :param file:
     :param dict_heavy:
     :return:
     """
-    with zipfile.ZipFile(file + '.zip', 'w', compression=zipfile.ZIP_DEFLATED, compresslevel=9) as zipped_f:
+    with zipfile.ZipFile(file + '.zip', 'w', compression=zipfile.ZIP_DEFLATED, compresslevel=compresslevel) as zipped_f:
         for key, value in dict_heavy.items():
             if isinstance(value, np.ndarray):
                 container = NumpyJson(dtype=str(value.dtype),
                                       data=value.tolist())
                 zipped_f.writestr(key + '.json', json.dumps(container.__dict__, indent=2))
 
 
@@ -337,24 +337,24 @@
 # class MetaDataSettings:
 #     PRIVATE: Dict[str] = field(default_factory=lambda :{'private': True})# this value is not getting stored or loaded to disk
 #
 
 T = TypeVar('T')
 
 
-def store_files_to_zip(file_path_zip, dict_files: Dict[str, str]):
+def store_files_to_zip(file_path_zip, dict_files: Dict[str, str], compresslevel=2):
     create_parent_dir_if_not_exists(file_path_zip)
     if file_path_zip.suffix != '.zip':
         file_path_with_dot_zip = _custom_with_suffix(file_path_zip, '.zip')
     else:
         file_path_with_dot_zip = file_path_zip
     from io import BytesIO
     data = BytesIO()
     with zipfile.ZipFile(file_path_with_dot_zip, 'w', compression=zipfile.ZIP_DEFLATED,
-                         compresslevel=2) as zipped_f:
+                         compresslevel=compresslevel) as zipped_f:
         for key, value in dict_files.items():
             if key.endswith('npz'):
                 # https://stackoverflow.com/questions/2463770/python-in-memory-zip-library
                 np.savez(data, **value)
                 zipped_f.writestr(key, data.getvalue())
             else:
                 zipped_f.writestr(key, value)
@@ -592,21 +592,21 @@
 
 def create_parent_dir_if_not_exists(file):
     logging.info('write: ' + str(file))
     if not file.parent.exists():
         Path.mkdir(file.parent, parents=True)
         print('Created directory ' + str(file.parent))
 
-def _store_pkl(instance, file, compression=None,**kwargs):
+def _store_pkl(instance, file, compression=None, compresslevel=2,**kwargs):
     create_parent_dir_if_not_exists(file)
     if compression is None:
         with open(file, 'wb') as f:
             pickle.dump(instance, f)
     elif compression =='zip':
-        with zipfile.ZipFile(file, 'w', compression=zipfile.ZIP_DEFLATED, compresslevel=9) as zipped_f:
+        with zipfile.ZipFile(file, 'w', compression=zipfile.ZIP_DEFLATED, compresslevel=compresslevel) as zipped_f:
             zipped_f.writestr(file.stem + '.pkl', pickle.dumps(instance))
     else:
         raise NotImplementedError('Unsupported compression')
 
 
 def replace_ids_with_arrays_in_json_dict(dict_json, dict_arrays):
     if isinstance(dict_json, list):
```

### Comparing `dataclass-persistence-0.3.6/dataclass_persistence.egg-info/PKG-INFO` & `dataclass-persistence-0.3.7/dataclass_persistence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-persistence
-Version: 0.3.6
+Version: 0.3.7
 Summary: Persists information contained in dataclasses.
 Home-page: https://github.com/philipp-mohr/dataclass-persistence
 Author: P.Mohr
 Author-email: philipp.mohr@tuhh.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `dataclass-persistence-0.3.6/setup.py` & `dataclass-persistence-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Package meta-data.
 NAME = 'dataclass-persistence'
 DESCRIPTION = 'Persists information contained in dataclasses.'
 URL = 'https://github.com/philipp-mohr/dataclass-persistence'
 EMAIL = 'philipp.mohr@tuhh.de'
 AUTHOR = 'P.Mohr'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.3.6'
+VERSION = '0.3.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy', 'StrEnum'  # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

