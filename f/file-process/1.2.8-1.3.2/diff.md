# Comparing `tmp/file_process-1.2.8.tar.gz` & `tmp/file_process-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_process-1.2.8.tar", last modified: Tue Sep 26 20:38:35 2023, max compression
+gzip compressed data, was "file_process-1.3.2.tar", last modified: Thu Apr  4 14:45:45 2024, max compression
```

## Comparing `file_process-1.2.8.tar` & `file_process-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 20:38:35.128596 file_process-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-26 20:38:25.000000 file_process-1.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-09-26 20:38:35.128596 file_process-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-09-26 20:38:25.000000 file_process-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 20:38:35.124595 file_process-1.2.8/file_process/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 20:38:35.124595 file_process-1.2.8/file_process/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/csv/csv_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/csv/csv_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/csv/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/file_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 20:38:35.128596 file_process-1.2.8/file_process/h5ad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/h5ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/h5ad/h5ad_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/h5ad/h5ad_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/h5ad/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-09-26 20:38:25.000000 file_process-1.2.8/file_process/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 20:38:35.124595 file_process-1.2.8/file_process.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-09-26 20:38:34.000000 file_process-1.2.8/file_process.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-09-26 20:38:35.000000 file_process-1.2.8/file_process.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 20:38:34.000000 file_process-1.2.8/file_process.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-09-26 20:38:34.000000 file_process-1.2.8/file_process.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-26 20:38:34.000000 file_process-1.2.8/file_process.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-09-26 20:38:35.128596 file_process-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-09-26 20:38:25.000000 file_process-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:45:45.528460 file_process-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 14:45:42.000000 file_process-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 14:45:45.528460 file_process-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 14:45:42.000000 file_process-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:45:45.528460 file_process-1.3.2/file_process/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:45:45.528460 file_process-1.3.2/file_process/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/csv/csv_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/csv/csv_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/csv/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/file_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:45:45.528460 file_process-1.3.2/file_process/h5ad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/h5ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/h5ad/h5ad_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/h5ad/h5ad_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/h5ad/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 14:45:42.000000 file_process-1.3.2/file_process/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:45:45.528460 file_process-1.3.2/file_process.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 14:45:45.000000 file_process-1.3.2/file_process.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 14:45:45.000000 file_process-1.3.2/file_process.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:45:45.000000 file_process-1.3.2/file_process.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 14:45:45.000000 file_process-1.3.2/file_process.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 14:45:45.000000 file_process-1.3.2/file_process.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 14:45:45.528460 file_process-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-04 14:45:42.000000 file_process-1.3.2/setup.py
```

### Comparing `file_process-1.2.8/LICENSE.txt` & `file_process-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file_process-1.2.8/README.md` & `file_process-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `file_process-1.2.8/file_process/csv/csv_processor.py` & `file_process-1.3.2/file_process/csv/csv_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List, Optional
 from io import BytesIO
+import csv
+import _csv
 
 import pandas as pd
 from numpy import number, nan
 from pandas.errors import ParserError
 
 from file_process.base import FileProcessorBase
 from file_process.constants import PREVIEW_ROWS_COUNT
@@ -13,16 +15,20 @@
 
 
 class CSVFileProcessor(FileProcessorBase):
 
     def __init__(self, file: BytesIO, **kwargs):
         delimiter = kwargs.get('delimiter')
         if not delimiter:
-            reader = pd.read_csv(file, sep=None, iterator=True, nrows=10)
-            delimiter = reader._engine.data.dialect.delimiter  # pylint: disable=protected-access
+            sniffer = csv.Sniffer()
+            data = file.read(4096)
+            try:
+                delimiter = sniffer.sniff(str(data, encoding='utf-8')).delimiter
+            except _csv.Error:
+                delimiter = ","
             file.seek(0)
         self.delimiter = delimiter
         try:
             self.data_df = pd.read_csv(file, sep=self.delimiter)
         except ParserError as exc:
             raise DelimiterError() from exc
 
@@ -37,15 +43,15 @@
 
     def get_var_names(self):
         return list(self.data_df.columns)
 
     def get_preview(self):
         var_names = self.get_var_names()
         obs_preview = self.get_observations(PREVIEW_ROWS_COUNT)
-        return var_names, self.create_tabular_response(obs_preview), None
+        return var_names, self.create_tabular_response(obs_preview), None, None
 
     @staticmethod
     def create_tabular_response(data_df: pd.DataFrame) -> List[dict]:
         if data_df is None:
             return []
         numeric_columns = data_df.select_dtypes(include=number).columns
         rows = data_df.replace({nan: None})
```

### Comparing `file_process-1.2.8/file_process/csv/csv_validator.py` & `file_process-1.3.2/file_process/csv/csv_validator.py`

 * *Files identical despite different names*

### Comparing `file_process-1.2.8/file_process/csv/schemas.py` & `file_process-1.3.2/file_process/csv/schemas.py`

 * *Files identical despite different names*

### Comparing `file_process-1.2.8/file_process/exceptions.py` & `file_process-1.3.2/file_process/exceptions.py`

 * *Files identical despite different names*

### Comparing `file_process-1.2.8/file_process/h5ad/h5ad_processor.py` & `file_process-1.3.2/file_process/h5ad/h5ad_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def get_variables(self, rows_number: Optional[int] = None):
         return self.adata.var.head(n=rows_number)
 
     def get_preview(self):
         target_names = self.get_targets()
         obs_preview = self.get_observations(PREVIEW_ROWS_COUNT)
         var_preview = self.get_variables(PREVIEW_ROWS_COUNT)
-        return target_names, self.create_tabular_response(obs_preview), self.create_tabular_response(var_preview)
+        return target_names, self.create_tabular_response(obs_preview), self.create_tabular_response(var_preview), None
 
     @staticmethod
     def create_tabular_response(data_df: pd.DataFrame) -> List[dict]:
         if data_df is None:
             return []
         data_df = data_df.astype(object)
         rows = data_df.round(2).where(pd.notnull(data_df), None).to_dict(orient='records')
```

### Comparing `file_process-1.2.8/file_process/h5ad/h5ad_validator.py` & `file_process-1.3.2/file_process/h5ad/h5ad_validator.py`

 * *Files identical despite different names*

### Comparing `file_process-1.2.8/file_process.egg-info/SOURCES.txt` & `file_process-1.3.2/file_process.egg-info/SOURCES.txt`

 * *Files identical despite different names*

