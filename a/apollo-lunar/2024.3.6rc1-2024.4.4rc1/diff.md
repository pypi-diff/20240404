# Comparing `tmp/apollo_lunar-2024.3.6rc1.tar.gz` & `tmp/apollo_lunar-2024.4.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo_lunar-2024.3.6rc1.tar", max compression
+gzip compressed data, was "apollo_lunar-2024.4.4rc1.tar", max compression
```

## Comparing `apollo_lunar-2024.3.6rc1.tar` & `apollo_lunar-2024.4.4rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1089 2024-03-06 02:19:23.161827 apollo_lunar-2024.3.6rc1/LICENSE
--rw-r--r--   0        0        0     4618 2024-03-06 02:19:23.161827 apollo_lunar-2024.3.6rc1/README.md
--rw-r--r--   0        0        0       56 2024-03-06 02:19:23.161827 apollo_lunar-2024.3.6rc1/bap/__init__.py
--rw-r--r--   0        0        0     6034 2024-03-06 02:19:23.161827 apollo_lunar-2024.3.6rc1/lunar/__init__.py
--rw-r--r--   0        0        0    12593 2024-03-06 02:19:23.161827 apollo_lunar-2024.3.6rc1/lunar/cli.py
--rw-r--r--   0        0        0     4502 2024-03-06 02:19:23.161827 apollo_lunar-2024.3.6rc1/lunar/config/__init__.py
--rw-r--r--   0        0        0      255 2024-03-06 02:19:23.161827 apollo_lunar-2024.3.6rc1/lunar/data/__init__.py
--rw-r--r--   0        0        0       58 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/batch/__init__.py
--rw-r--r--   0        0        0     1794 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/batch/batch.py
--rw-r--r--   0        0        0       99 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/batch/models/__init__.py
--rw-r--r--   0        0        0      421 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/batch/models/batch_models.py
--rw-r--r--   0        0        0       55 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/data/__init__.py
--rw-r--r--   0        0        0     8963 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/data/data.py
--rw-r--r--   0        0        0      103 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/datasets/__init__.py
--rw-r--r--   0        0        0     8959 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/datasets/dataset.py
--rw-r--r--   0        0        0      123 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/datasets/models/__init__.py
--rw-r--r--   0        0        0      856 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/datasets/models/dataset_models.py
--rw-r--r--   0        0        0      150 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/datasets/models/params/__init__.py
--rw-r--r--   0        0        0      845 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/datasets/models/params/dynamodb.py
--rw-r--r--   0        0        0       67 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/dynamodb/__init__.py
--rw-r--r--   0        0        0     2853 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/dynamodb/dynamodb.py
--rw-r--r--   0        0        0       58 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/query/__init__.py
--rw-r--r--   0        0        0     3340 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/data/query/query.py
--rw-r--r--   0        0        0     2768 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/lunar_client.py
--rw-r--r--   0        0        0      224 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/ml/__init__.py
--rw-r--r--   0        0        0     5039 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/ml/aidp_service.py
--rw-r--r--   0        0        0     6495 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/ml/edd_service.py
--rw-r--r--   0        0        0      740 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/ml/lunar_model.py
--rw-r--r--   0        0        0     4075 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/ml/model_registry.py
--rw-r--r--   0        0        0      201 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/__init__.py
--rw-r--r--   0        0        0       64 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/channels/__init__.py
--rw-r--r--   0        0        0     7391 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/channels/channel.py
--rw-r--r--   0        0        0      123 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/channels/models/__init__.py
--rw-r--r--   0        0        0      461 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/channels/models/channel_models.py
--rw-r--r--   0        0        0       74 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/experiments/__init__.py
--rw-r--r--   0        0        0     9615 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/experiments/experiment.py
--rw-r--r--   0        0        0      144 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/experiments/models/__init__.py
--rw-r--r--   0        0        0     1768 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/experiments/models/experiment_models.py
--rw-r--r--   0        0        0       85 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/recommendations/__init__.py
--rw-r--r--   0        0        0      124 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/recommendations/models/__init__.py
--rw-r--r--   0        0        0      799 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/recommendations/models/recommendation_models.py
--rw-r--r--   0        0        0     2432 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/lunar/rec/recommendations/recommendation.py
--rw-r--r--   0        0        0     1045 2024-03-06 02:19:23.165827 apollo_lunar-2024.3.6rc1/pyproject.toml
--rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 apollo_lunar-2024.3.6rc1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/LICENSE
+-rw-r--r--   0        0        0     4618 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/README.md
+-rw-r--r--   0        0        0       56 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/bap/__init__.py
+-rw-r--r--   0        0        0     6034 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/lunar/__init__.py
+-rw-r--r--   0        0        0    12593 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/lunar/cli.py
+-rw-r--r--   0        0        0     4502 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/config/__init__.py
+-rw-r--r--   0        0        0      255 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/__init__.py
+-rw-r--r--   0        0        0       58 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/batch/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/batch/batch.py
+-rw-r--r--   0        0        0       99 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/batch/models/__init__.py
+-rw-r--r--   0        0        0      421 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/batch/models/batch_models.py
+-rw-r--r--   0        0        0       55 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/data/__init__.py
+-rw-r--r--   0        0        0     8963 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/data/data.py
+-rw-r--r--   0        0        0      103 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     8959 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/dataset.py
+-rw-r--r--   0        0        0      123 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/dataset_models.py
+-rw-r--r--   0        0        0      150 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/params/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/params/dynamodb.py
+-rw-r--r--   0        0        0       67 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/dynamodb/__init__.py
+-rw-r--r--   0        0        0     2853 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/dynamodb/dynamodb.py
+-rw-r--r--   0        0        0       58 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/query/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/query/query.py
+-rw-r--r--   0        0        0     2768 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/lunar_client.py
+-rw-r--r--   0        0        0      224 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/__init__.py
+-rw-r--r--   0        0        0     7845 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/aidp_service.py
+-rw-r--r--   0        0        0     6495 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/edd_service.py
+-rw-r--r--   0        0        0      740 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/lunar_model.py
+-rw-r--r--   0        0        0     4075 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/model_registry.py
+-rw-r--r--   0        0        0      201 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/channels/__init__.py
+-rw-r--r--   0        0        0     7391 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/channels/channel.py
+-rw-r--r--   0        0        0      123 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/channels/models/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/channels/models/channel_models.py
+-rw-r--r--   0        0        0       74 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/experiments/__init__.py
+-rw-r--r--   0        0        0     9615 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/experiments/experiment.py
+-rw-r--r--   0        0        0      144 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/experiments/models/__init__.py
+-rw-r--r--   0        0        0     1768 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/experiments/models/experiment_models.py
+-rw-r--r--   0        0        0       85 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/models/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/models/recommendation_models.py
+-rw-r--r--   0        0        0     2432 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/recommendation.py
+-rw-r--r--   0        0        0     1045 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 apollo_lunar-2024.4.4rc1/PKG-INFO
```

### Comparing `apollo_lunar-2024.3.6rc1/LICENSE` & `apollo_lunar-2024.4.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/README.md` & `apollo_lunar-2024.4.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/__init__.py` & `apollo_lunar-2024.4.4rc1/lunar/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/cli.py` & `apollo_lunar-2024.4.4rc1/lunar/cli.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/config/__init__.py` & `apollo_lunar-2024.4.4rc1/lunar/config/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/data/batch/batch.py` & `apollo_lunar-2024.4.4rc1/lunar/data/batch/batch.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/data/data/data.py` & `apollo_lunar-2024.4.4rc1/lunar/data/data/data.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/data/datasets/dataset.py` & `apollo_lunar-2024.4.4rc1/lunar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/data/datasets/models/dataset_models.py` & `apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/dataset_models.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/data/datasets/models/params/dynamodb.py` & `apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/params/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/data/dynamodb/dynamodb.py` & `apollo_lunar-2024.4.4rc1/lunar/data/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/data/query/query.py` & `apollo_lunar-2024.4.4rc1/lunar/data/query/query.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/lunar_client.py` & `apollo_lunar-2024.4.4rc1/lunar/lunar_client.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/ml/aidp_service.py` & `apollo_lunar-2024.4.4rc1/lunar/ml/aidp_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Any, Dict
-
 import shlex
 import subprocess
 
 from lunar.config import Config
 from lunar.data import BatchClient
 from lunar.lunar_client import LunarError
 
@@ -25,15 +23,15 @@
         db_type: str,
         operation: str,
         target_name: str = None,
         s3_dt: str = None,
         bq_table_partition: str = None,
         write_type: str = "json",
         max_num_files: int = 20,
-    ) -> Dict[str, Any]:
+    ):
         """
         Copy a table from AIDP BigQuery to BAP S3 and Database.
 
         ## Args
 
         - database_name: (str) Database name of Bigquery
         - table_name: (str) Name of a table on Bigquery
@@ -95,23 +93,99 @@
         job_name = f"{target_name}-{operation}"
         job_list = self.batch_client.get_batch_list(job_status_list=BATCH_JOB_CHECK_STATUS_LIST)
 
         if job_name in job_list:
             raise LunarError(code=400, msg=f"Job {job_name} is already submitted to BAP S3")
 
         s3_dt_str = f"dt={s3_dt}/" if s3_dt else ""
+
         s3_bucket_name = f"s3a://lunar-loader-{self.config.ENV.lower()}"
         s3_path = f"{s3_bucket_name}/{db_type}/{target_name}/{s3_dt_str}op={operation}"
 
         # BigQuery to BAP S3
         # 1) BigQuery to spark dataframe
         try:
             bq_df = bq_table_to_df(
                 database_name, table_name, col_list="*", partition=bq_table_partition, spark_session=spark
             )
+        except Exception as e:
+            raise LunarError(code=400, msg=f"Fail to get BigQuery to spark dataframe {str(e)}")
+
+        # 2) spark dataframe to BAP S3
+        num_rows = bq_df.count()
+        num_files = min(max_num_files, int(num_rows / 10000) + 1)  # 10,000건 당 1개 worker로 처리
+        try:
+            print(f"Writing on {s3_path}, '{num_rows}' rows")
+            if write_type == "parquet":
+                bq_df.repartition(num_files).write.mode("overwrite").parquet(s3_path)
+            else:
+                bq_df.repartition(num_files).write.mode("overwrite").json(s3_path)
+        except Exception as e:
+            raise LunarError(code=400, msg=f"Fail to write spark dataframe to BAP S3, Error: {str(e)}")
+
+        process_touch = subprocess.Popen(shlex.split(f"hdfs dfs -touchz {s3_path}/_SUCCESS"))
+        process_touch.wait()
+        if process_touch.returncode != 0:
+            raise LunarError(code=400, msg="Fail to touch '_SUCCESS' file")
+
+        print(f"SUCCESS to write files from BigQuery to BAP S3, counts: {num_rows}")
+
+    def copy_table_to_s3_without_load(
+        self,
+        database_name: str,
+        table_name: str,
+        directory_name: str = None,
+        bq_table_partition: str = None,
+        write_type: str = "parquet",
+        max_num_files: int = 20,
+    ):
+        """
+        Copy a table from AIDP BigQuery to BAP S3. (Not database loading)
+
+        ## Args
+
+        - database_name: (str) Database name of Bigquery
+        - table_name: (str) Name of a table on Bigquery
+        - directory_name: (optional) (str) Name of directory to save on BAP S3
+        - bq_table_partition: (optional) (str) Partition value of table on BigQuery
+        - write_type: (optional) Write type ('json' | (default) 'parquet')
+        - max_num_files: (optional) (int) Maximum number of files to be saved on AWS S3 (default: 10)
+
+        ## Returns
+        dict
+
+        ## Example
+
+        ```python
+        response = copy_table_to_s3_without_load(
+            database_name="apollo",
+            table_name="test_table",
+            directory_name="movie",
+            write_type="parquet"
+            bq_table_partition="2021-09-01",
+        )
+
+        ```
+        """
+
+        from skt.gcp import bq_table_to_df
+        from skt.ye import get_spark
+
+        spark = get_spark()
+        # spark dataframe을 fs로 write 시 _SUCCESS 파일을 자동으로 생성하는 것을 방지
+        spark.conf.set("mapreduce.fileoutputcommitter.marksuccessfuljobs", "false")
+
+        s3_path = f"s3a://aide-bucket-{self.config.ENV.lower()}/{directory_name}"
+
+        # BigQuery to BAP S3
+        # 1) BigQuery to spark dataframe
+        try:
+            bq_df = bq_table_to_df(
+                database_name, table_name, col_list="*", partition=bq_table_partition, spark_session=spark
+            )
         except Exception as e:
             raise LunarError(code=400, msg=f"Fail to get BigQuery to spark dataframe {str(e)}")
 
         # 2) spark dataframe to BAP S3
         num_rows = bq_df.count()
         num_files = min(max_num_files, int(num_rows / 10000) + 1)  # 10,000건 당 1개 worker로 처리
         try:
```

### Comparing `apollo_lunar-2024.3.6rc1/lunar/ml/edd_service.py` & `apollo_lunar-2024.4.4rc1/lunar/ml/edd_service.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/ml/lunar_model.py` & `apollo_lunar-2024.4.4rc1/lunar/ml/lunar_model.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/ml/model_registry.py` & `apollo_lunar-2024.4.4rc1/lunar/ml/model_registry.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/rec/channels/channel.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/channels/channel.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/rec/experiments/experiment.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/rec/experiments/models/experiment_models.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/experiments/models/experiment_models.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/rec/recommendations/models/recommendation_models.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/models/recommendation_models.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/lunar/rec/recommendations/recommendation.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/recommendation.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.3.6rc1/pyproject.toml` & `apollo_lunar-2024.4.4rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apollo-lunar"
-version = "2024.3.6rc1"
+version = "2024.4.4rc1"
 description = "A Python SDK/CLI for Lunar API"
 authors = ["Lunar module <lunar@sktio.io>"]
 readme = "README.md"
 license = "MIT"
 include = [
     "LICENSE",
 ]
```

### Comparing `apollo_lunar-2024.3.6rc1/PKG-INFO` & `apollo_lunar-2024.4.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-lunar
-Version: 2024.3.6rc1
+Version: 2024.4.4rc1
 Summary: A Python SDK/CLI for Lunar API
 License: MIT
 Author: Lunar module
 Author-email: lunar@sktio.io
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

