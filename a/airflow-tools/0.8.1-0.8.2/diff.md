# Comparing `tmp/airflow_tools-0.8.1.tar.gz` & `tmp/airflow_tools-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_tools-0.8.1.tar", max compression
+gzip compressed data, was "airflow_tools-0.8.2.tar", max compression
```

## Comparing `airflow_tools-0.8.1.tar` & `airflow_tools-0.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2024-02-26 10:29:12.681236 airflow_tools-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0     8788 2024-04-03 08:24:08.137208 airflow_tools-0.8.1/README.md
--rw-r--r--   0        0        0     1312 2024-04-03 14:37:46.958244 airflow_tools-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/__init__.py
--rw-r--r--   0        0        0       22 2024-04-03 14:50:25.840684 airflow_tools-0.8.1/src/airflow_tools/_version.py
--rw-r--r--   0        0        0     1794 2024-01-18 10:00:14.774290 airflow_tools-0.8.1/src/airflow_tools/compression_utils.py
--rw-r--r--   0        0        0     4426 2024-04-03 08:24:08.197207 airflow_tools-0.8.1/src/airflow_tools/data_lake_facade.py
--rw-r--r--   0        0        0      115 2024-01-03 14:54:38.107397 airflow_tools-0.8.1/src/airflow_tools/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.701235 airflow_tools-0.8.1/src/airflow_tools/filesystems/__init__.py
--rw-r--r--   0        0        0     2298 2024-03-20 11:42:50.252535 airflow_tools-0.8.1/src/airflow_tools/filesystems/filesystem_factory.py
--rw-r--r--   0        0        0      561 2024-04-03 08:24:08.209207 airflow_tools-0.8.1/src/airflow_tools/filesystems/filesystem_protocol.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.713235 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/__init__.py
--rw-r--r--   0        0        0     2382 2024-04-03 14:39:01.369156 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
--rw-r--r--   0        0        0     1974 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
--rw-r--r--   0        0        0     2472 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
--rw-r--r--   0        0        0     1586 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/local_filesystem.py
--rw-r--r--   0        0        0     2185 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/s3_filesystem.py
--rw-r--r--   0        0        0     1396 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/sftp_filesystem.py
--rw-r--r--   0        0        0     3877 2024-02-26 10:29:12.737235 airflow_tools-0.8.1/src/airflow_tools/notifications/slack/webhook.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.1/src/airflow_tools/providers/azure/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/__init__.py
--rw-r--r--   0        0        0     3396 2024-03-20 11:42:50.252535 airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/azure_databricks.py
--rw-r--r--   0        0        0     1619 2024-03-20 11:42:50.268535 airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/azure_file_share.py
--rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.1/src/airflow_tools/providers/data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.1/src/airflow_tools/providers/data_lake/operators/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-03 08:24:08.213207 airflow_tools-0.8.1/src/airflow_tools/providers/data_lake/operators/data_lake.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/__init__.py
--rw-r--r--   0        0        0     5437 2024-04-03 08:24:08.225207 airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/filesystem.py
--rw-r--r--   0        0        0     9233 2024-04-03 14:35:27.096443 airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/providers/http_to_data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
--rw-r--r--   0        0        0     9037 2024-04-03 08:24:08.257207 airflow_tools-0.8.1/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
--rw-r--r--   0        0        0     1108 2024-03-20 11:42:50.268535 airflow_tools-0.8.1/src/airflow_tools/providers/package.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.1/src/airflow_tools/py.typed
--rw-r--r--   0        0        0    10026 1970-01-01 00:00:00.000000 airflow_tools-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-02-26 10:29:12.681236 airflow_tools-0.8.2/LICENSE.txt
+-rw-r--r--   0        0        0     8788 2024-04-03 08:24:08.137208 airflow_tools-0.8.2/README.md
+-rw-r--r--   0        0        0     1312 2024-04-04 14:12:08.276028 airflow_tools-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-04 14:12:08.276028 airflow_tools-0.8.2/src/airflow_tools/_version.py
+-rw-r--r--   0        0        0     1794 2024-01-18 10:00:14.774290 airflow_tools-0.8.2/src/airflow_tools/compression_utils.py
+-rw-r--r--   0        0        0     4426 2024-04-03 08:24:08.197207 airflow_tools-0.8.2/src/airflow_tools/data_lake_facade.py
+-rw-r--r--   0        0        0      115 2024-01-03 14:54:38.107397 airflow_tools-0.8.2/src/airflow_tools/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-26 10:29:12.701235 airflow_tools-0.8.2/src/airflow_tools/filesystems/__init__.py
+-rw-r--r--   0        0        0     2298 2024-03-20 11:42:50.252535 airflow_tools-0.8.2/src/airflow_tools/filesystems/filesystem_factory.py
+-rw-r--r--   0        0        0      561 2024-04-03 08:24:08.209207 airflow_tools-0.8.2/src/airflow_tools/filesystems/filesystem_protocol.py
+-rw-r--r--   0        0        0        0 2024-02-26 10:29:12.713235 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/__init__.py
+-rw-r--r--   0        0        0     2382 2024-04-04 11:13:41.968166 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
+-rw-r--r--   0        0        0     1974 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
+-rw-r--r--   0        0        0     2472 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
+-rw-r--r--   0        0        0     1586 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/local_filesystem.py
+-rw-r--r--   0        0        0     2185 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/s3_filesystem.py
+-rw-r--r--   0        0        0     1396 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/sftp_filesystem.py
+-rw-r--r--   0        0        0     3877 2024-02-26 10:29:12.737235 airflow_tools-0.8.2/src/airflow_tools/notifications/slack/webhook.py
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/providers/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.2/src/airflow_tools/providers/azure/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/__init__.py
+-rw-r--r--   0        0        0     3396 2024-03-20 11:42:50.252535 airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/azure_databricks.py
+-rw-r--r--   0        0        0     1619 2024-03-20 11:42:50.268535 airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/azure_file_share.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.2/src/airflow_tools/providers/data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.2/src/airflow_tools/providers/data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/providers/data_lake/operators/data_lake.py
+-rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/__init__.py
+-rw-r--r--   0        0        0     5437 2024-04-03 08:24:08.225207 airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/filesystem.py
+-rw-r--r--   0        0        0     9802 2024-04-04 14:12:08.276028 airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/providers/http_to_data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     9037 2024-04-03 08:24:08.257207 airflow_tools-0.8.2/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
+-rw-r--r--   0        0        0     1108 2024-03-20 11:42:50.268535 airflow_tools-0.8.2/src/airflow_tools/providers/package.py
+-rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/py.typed
+-rw-r--r--   0        0        0    10026 1970-01-01 00:00:00.000000 airflow_tools-0.8.2/PKG-INFO
```

### Comparing `airflow_tools-0.8.1/LICENSE.txt` & `airflow_tools-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/README.md` & `airflow_tools-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/pyproject.toml` & `airflow_tools-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-tools"
-version = "0.8.1"
+version = "0.8.2"
 
 description = ""
 authors = ["Biel Llobera <biel_llobera@dkl.digital>"]
 readme = "README.md"
 include = ["src/airflow_tools"]
 
 [tool.poetry.dependencies]
```

### Comparing `airflow_tools-0.8.1/src/airflow_tools/compression_utils.py` & `airflow_tools-0.8.2/src/airflow_tools/compression_utils.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/data_lake_facade.py` & `airflow_tools-0.8.2/src/airflow_tools/data_lake_facade.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/filesystems/filesystem_factory.py` & `airflow_tools-0.8.2/src/airflow_tools/filesystems/filesystem_factory.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/filesystems/filesystem_protocol.py` & `airflow_tools-0.8.2/src/airflow_tools/filesystems/filesystem_protocol.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py` & `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py` & `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py` & `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/local_filesystem.py` & `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/local_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/s3_filesystem.py` & `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/s3_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/filesystems/impl/sftp_filesystem.py` & `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/sftp_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/notifications/slack/webhook.py` & `airflow_tools-0.8.2/src/airflow_tools/notifications/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/azure_databricks.py` & `airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/azure_databricks.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/providers/azure/hooks/azure_file_share.py` & `airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/azure_file_share.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/providers/data_lake/operators/data_lake.py` & `airflow_tools-0.8.2/src/airflow_tools/providers/data_lake/operators/data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/filesystem.py` & `airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py` & `airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,29 @@
     from airflow.providers.http.operators.http import SimpleHttpOperator as HttpOperator
 
 from airflow.utils.context import Context
 from airflow.utils.helpers import merge_dicts
 from requests import Response
 
 from airflow_tools.compression_utils import CompressionOptions, compress
-from airflow_tools.filesystems.filesystem_factory import FilesystemFactory
 from airflow_tools.exceptions import ApiResponseTypeError
+from airflow_tools.filesystems.filesystem_factory import FilesystemFactory
 
 if TYPE_CHECKING:
     from requests.auth import AuthBase
 
 SaveFormat = Literal['jsonl']
 
 
 class HttpBatchOperator(HttpOperator):
     def execute(
         self, context: Context, use_new_data_parameters_on_pagination=False
     ) -> Any:
         self.log.info("Calling HTTP method")
+
         response = self.hook.run(
             self.endpoint, self.data, self.headers, self.extra_options
         )
         yield self.process_response(context=context, response=response)
         for response in self.paginate_sync(
             response=response,
             use_new_data_parameters_on_pagination=use_new_data_parameters_on_pagination,
@@ -103,14 +104,15 @@
         'filesystem_conn_id',
         'jmespath_expression',
         'save_format',
     ]
     template_fields_renderers = HttpOperator.template_fields_renderers
 
     json_response_save_format = ['json', 'jsonl']
+    binary_response_save_format = ['parquet']
 
     def __init__(
         self,
         http_conn_id: str,
         filesystem_conn_id: str,
         filesystem_path: str,
         save_format: SaveFormat = 'jsonl',
@@ -141,14 +143,22 @@
         self.jmespath_expression = jmespath_expression
         self.pagination_function = pagination_function
         self.use_new_data_parameters_on_pagination = (
             use_new_data_parameters_on_pagination
         )
         self.create_file_on_success = create_file_on_success
 
+        if (
+            self.save_format in self.binary_response_save_format
+            and self.compression is not None
+        ):
+            raise ValueError(
+                f'Compression is not supported for binary response save formats: {self.binary_response_save_format}'
+            )
+
     def execute(self, context: 'Context') -> Any:
         http_batch_operator = HttpBatchOperator(
             task_id='http-operator',
             http_conn_id=self.http_conn_id,
             endpoint=self.endpoint,
             method=self.method,
             data=self.data,
@@ -167,21 +177,26 @@
             filesystem_protocol = FilesystemFactory.get_data_lake_filesystem(
                 connection=BaseHook.get_connection(self.filesystem_conn_id),
             )
 
             file_path = self.filesystem_path.rstrip('/') + '/' + self._file_name(i)
 
             filesystem_protocol.write(data, file_path)
-            
-            if self.create_file_on_success is not None and isinstance(self.create_file_on_success, str):
-                success_file_path = self.filesystem_path.rstrip('/') + '/' + self.create_file_on_success
+
+            if self.create_file_on_success is not None and isinstance(
+                self.create_file_on_success, str
+            ):
+                success_file_path = (
+                    self.filesystem_path.rstrip('/') + '/' + self.create_file_on_success
+                )
                 filesystem_protocol.write(BytesIO(), success_file_path)
 
     def _file_name(self, n_part) -> str:
         file_name = f'part{n_part:04}.{self.save_format}'
+
         if self.compression:
             file_name += f'.{self.compression}'
         return file_name
 
     def _response_filter(self, response) -> BytesIO:
         if (
             self.jmespath_expression
@@ -196,14 +211,16 @@
             raise ApiResponseTypeError(
                 'JMESPath expression is only supported for json and jsonl save formats'
             )
 
         elif self.save_format in self.json_response_save_format:
             self.data = response.json()
 
+        elif self.save_format in self.binary_response_save_format:
+            self.data = response.content
         else:
             self.data = response.text
 
         match self.save_format:
             case 'json':
                 return json_to_binary(self.data, self.compression)
 
@@ -214,15 +231,18 @@
                     )
                 return list_to_jsonl(self.data, self.compression)
 
             case 'xml':
                 return xml_to_binary(self.data, self.compression)
 
             case 'parquet':
-                return parquet_to_binary(self.data, self.compression)
+                return self.data
+
+            case 'csv':
+                return csv_to_binary(self.data, self.compression)
 
             case _:
                 raise NotImplementedError(f'Unknown save_format: {self.save_format}')
 
 
 def list_to_jsonl(data: list[dict], compression: 'CompressionOptions') -> BytesIO:
     out = StringIO()
@@ -235,18 +255,18 @@
 def json_to_binary(data: dict, compression: 'CompressionOptions') -> BytesIO:
     json_string = json.dumps(data).encode()
     compressed_json = compress(compression, json_string)
     out = BytesIO(compressed_json)
     return out
 
 
-def parquet_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
-    parquet_df = pd.DataFrame(StringIO(data))
+def csv_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
+    csv_df = pd.read_csv(StringIO(data), sep=',')
     out = BytesIO()
-    parquet_df.to_parquet(out, compression=compression)
+    csv_df.to_csv(out, compression=compression, index=False)
     out.seek(0)
     return out
 
 
 def xml_to_binary(data: str, compression: 'CompressionOptions') -> BytesIO:
     compressed_xml = compress(compression, data.encode())
     out = BytesIO(compressed_xml)
```

### Comparing `airflow_tools-0.8.1/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py` & `airflow_tools-0.8.2/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/src/airflow_tools/providers/package.py` & `airflow_tools-0.8.2/src/airflow_tools/providers/package.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.1/PKG-INFO` & `airflow_tools-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-tools
-Version: 0.8.1
+Version: 0.8.2
 Summary: 
 Author: Biel Llobera
 Author-email: biel_llobera@dkl.digital
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.1 Summary: Author: Biel
+Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.2 Summary: Author: Biel
 Llobera Author-email: biel_llobera@dkl.digital Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: apache-
 airflow (>=2.8,<3.0) Requires-Dist: apache-airflow-providers-amazon
 (>=8.8.0,<9.0.0) Requires-Dist: apache-airflow-providers-microsoft-azure
 (>=8.0.0,<9.0.0) Requires-Dist: apache-airflow-providers-sftp (>=4.8.1,<5.0.0)
```

