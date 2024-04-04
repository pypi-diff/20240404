# Comparing `tmp/visionone-filesecurity-1.0.2.tar.gz` & `tmp/visionone-filesecurity-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionone-filesecurity-1.0.2.tar", last modified: Wed Nov 22 23:27:06 2023, max compression
+gzip compressed data, was "visionone-filesecurity-1.1.0.tar", last modified: Thu Apr  4 04:43:40 2024, max compression
```

## Comparing `visionone-filesecurity-1.0.2.tar` & `visionone-filesecurity-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:27:06.644244 visionone-filesecurity-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2023-11-22 23:27:06.644244 visionone-filesecurity-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:27:06.640244 visionone-filesecurity-1.0.2/amaas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/amaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/amaas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:27:06.640244 visionone-filesecurity-1.0.2/amaas/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/amaas/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:27:06.640244 visionone-filesecurity-1.0.2/amaas/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/amaas/grpc/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:27:06.640244 visionone-filesecurity-1.0.2/amaas/grpc/exception/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/amaas/grpc/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:27:06.644244 visionone-filesecurity-1.0.2/amaas/grpc/protos/
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-11-22 23:27:05.000000 visionone-filesecurity-1.0.2/amaas/grpc/protos/scan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2023-11-22 23:27:05.000000 visionone-filesecurity-1.0.2/amaas/grpc/protos/scan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-11-22 23:27:05.000000 visionone-filesecurity-1.0.2/amaas/grpc/protos/scan_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-11-22 23:25:59.000000 visionone-filesecurity-1.0.2/amaas/grpc/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-11-22 23:27:06.644244 visionone-filesecurity-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-11-22 23:27:05.000000 visionone-filesecurity-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:27:06.644244 visionone-filesecurity-1.0.2/visionone_filesecurity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2023-11-22 23:27:06.000000 visionone-filesecurity-1.0.2/visionone_filesecurity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-11-22 23:27:06.000000 visionone-filesecurity-1.0.2/visionone_filesecurity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 23:27:06.000000 visionone-filesecurity-1.0.2/visionone_filesecurity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-22 23:27:06.000000 visionone-filesecurity-1.0.2/visionone_filesecurity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-22 23:27:06.000000 visionone-filesecurity-1.0.2/visionone_filesecurity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/grpc/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/grpc/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/grpc/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/grpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-04 04:43:39.000000 visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-04 04:43:39.000000 visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-04 04:43:39.000000 visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/grpc/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/tests/test_aio_client_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/tests/test_client_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/top_level.txt
```

### Comparing `visionone-filesecurity-1.0.2/LICENSE` & `visionone-filesecurity-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.0.2/PKG-INFO` & `visionone-filesecurity-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionone-filesecurity
-Version: 1.0.2
+Version: 1.1.0
 Summary: Trend Micro VisionOne File Security SDK for python
 Home-page: https://github.com/trendmicro/tm-v1-fs-python-sdk
 Author: Trend Micro VisionOne File Security Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -35,26 +35,26 @@
 
    ```sh
    python -m pip install visionone-filesecurity
    ```
 
 ## Obtain an API Key
 
-The File Security SDK requires a valid API Key provided as parameter to the SDK client object. It can accept Trend Vision One API keys. 
+The File Security SDK requires a valid API Key provided as parameter to the SDK client object. It can accept Trend Vision One API keys.
 
 When obtaining the API Key, ensure that the API Key is associated with the region that you plan to use. It is important to note that Trend Vision One API Keys are associated with different regions, please refer to the region flag below to obtain a better understanding of the valid regions associated with the respective API Key.
 
 If you plan on using a Trend Vision One region, be sure to pass in region parameter when running custom program with File Security SDK to specify the region of that API key and to ensure you have proper authorization. The list of supported Trend Vision One regions can be found at API Reference section below.
 
 1. Login to the Trend Vision One.
 2. Create a new Trend Vision One API key:
 
-* Navigate to the Trend Vision One User Roles page.
-* Verify that there is a role with the "Run file scan via SDK" permissions enabled. If not, create a role by clicking on "Add Role" and "Save" once finished.
-* Directly configure a new key on the Trend Vision One API Keys page, using the role which contains the "Run file scan via SDK" permission. It is advised to set an expiry time for the API key and make a record of it for future reference.
+- Navigate to the Trend Vision One User Roles page.
+- Verify that there is a role with the "Run file scan via SDK" permissions enabled. If not, create a role by clicking on "Add Role" and "Save" once finished.
+- Directly configure a new key on the Trend Vision One API Keys page, using the role which contains the "Run file scan via SDK" permission. It is advised to set an expiry time for the API key and make a record of it for future reference.
 
 ## Run SDK
 
 ### Run with File Security SDK examples
 
 1. Go to `/examples/` in current directory.
 
@@ -67,20 +67,22 @@
    ```text
    client_aio.py
    client.py
    ```
 
 3. Current Python examples support following command line arguments
 
-   | Command Line Arguments                 | Value                    | Optional |
-   | :------------------ | :----------------------- | :------- |
-   | --region or -r | The region you obtained your API key.  Value provided must be one of the Vision One regions, e.g. `us-east-1`, `eu-central-1`, `ap-southeast-1`, `ap-southeast-2`, `ap-northeast-1` | Yes, either -r or -a |
-   | --addr or -a   | Trend Vision One File Security server, such as: antimalware.__REGION__.cloudone.trendmicro.com:443 | Yes, either -r or -a      |
-   | --api_key      | Vision One API Key              | No       |
-   | --filename or -f |        File to be scanned            | No       |
+   | Command Line Arguments | Value                                                                                                                                                                               | Optional             |
+   |------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------|
+   | --region or -r         | The region you obtained your API key.  Value provided must be one of the Vision One regions, e.g. `us-east-1`, `eu-central-1`, `ap-southeast-1`, `ap-southeast-2`, `ap-northeast-1` | Yes, either -r or -a |
+   | --addr or -a           | Trend Vision One File Security server, such as: antimalware.__REGION__.cloudone.trendmicro.com:443                                                                                  | Yes, either -r or -a |
+   | --api_key              | Vision One API Key                                                                                                                                                                  | No                   |
+   | --filename or -f       | File to be scanned                                                                                                                                                                  | No                   |
+   | --pml                  | Predictive Machine Learning                                                                                                                                                         | Yes                  |
+   | --tags or -f           | List of tags                                                                                                                                                                        | Yes                  |
 
 4. Run one of the examples.
 
    Make sure to customize the example program by configuring it with the API key from your Vision One account, found in your Vision One Dashboard. Assign the value of your Vision One Region's `API_KEY` to the variable and set `FILENAME` to the desired target file.
 
    ```sh
    python3 client.py -f FILENAME -r us-east-1 --tls true --api_key API_KEY
@@ -97,50 +99,7 @@
    or
 
    using asynchronous IO example program:
 
    ```sh
    python3 client_aio.py -f FILENAME -a antimalware._REGION_.cloudone.trendmicro.com:443 --tls true --api_key API_KEY
    ```
-
-### Code Examples
-
-```python
-import json
-import amaas.grpc
-
-handle = amaas.grpc.init(YOUR_FILE_SECURITY_SERVER, YOUR_VISION_ONE_KEY, True)
-
-result = amaas.grpc.scan_file(args.filename, handle)
-print(result)
-
-result_json = json.loads(result)
-print("Got scan result: %d" % result_json['scanResult'])
-
-amaas.grpc.quit(handle)
-
-```
-
-to use asyncio with  coroutines and tasks,
-
-```python:
-import json
-import pprint
-import asyncio
-import amaas.grpc.aio
-
-async def scan_files():
-   handle = amaas.grpc.aio.init(YOUR_FILE_SECURITY_SERVER, YOUR_VISION_ONE_KEY, True)
-
-   tasks = [asyncio.create_task(amaas.grpc.aio.scan_file(file_name, handle))]
-
-   scan_results = await asyncio.gather(*tasks)
-
-   for scan_result in scan_results:
-      pprint.pprint(json.loads(scan_result))
-
-   await amaas.grpc.aio.quit(handle)
-
-
-asyncio.run(scan_files())
-
-```
```

### Comparing `visionone-filesecurity-1.0.2/README.md` & `visionone-filesecurity-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
    ```sh
    python -m pip install visionone-filesecurity
    ```
 
 ## Obtain an API Key
 
-The File Security SDK requires a valid API Key provided as parameter to the SDK client object. It can accept Trend Vision One API keys. 
+The File Security SDK requires a valid API Key provided as parameter to the SDK client object. It can accept Trend Vision One API keys.
 
 When obtaining the API Key, ensure that the API Key is associated with the region that you plan to use. It is important to note that Trend Vision One API Keys are associated with different regions, please refer to the region flag below to obtain a better understanding of the valid regions associated with the respective API Key.
 
 If you plan on using a Trend Vision One region, be sure to pass in region parameter when running custom program with File Security SDK to specify the region of that API key and to ensure you have proper authorization. The list of supported Trend Vision One regions can be found at API Reference section below.
 
 1. Login to the Trend Vision One.
 2. Create a new Trend Vision One API key:
 
-* Navigate to the Trend Vision One User Roles page.
-* Verify that there is a role with the "Run file scan via SDK" permissions enabled. If not, create a role by clicking on "Add Role" and "Save" once finished.
-* Directly configure a new key on the Trend Vision One API Keys page, using the role which contains the "Run file scan via SDK" permission. It is advised to set an expiry time for the API key and make a record of it for future reference.
+- Navigate to the Trend Vision One User Roles page.
+- Verify that there is a role with the "Run file scan via SDK" permissions enabled. If not, create a role by clicking on "Add Role" and "Save" once finished.
+- Directly configure a new key on the Trend Vision One API Keys page, using the role which contains the "Run file scan via SDK" permission. It is advised to set an expiry time for the API key and make a record of it for future reference.
 
 ## Run SDK
 
 ### Run with File Security SDK examples
 
 1. Go to `/examples/` in current directory.
 
@@ -48,20 +48,22 @@
    ```text
    client_aio.py
    client.py
    ```
 
 3. Current Python examples support following command line arguments
 
-   | Command Line Arguments                 | Value                    | Optional |
-   | :------------------ | :----------------------- | :------- |
-   | --region or -r | The region you obtained your API key.  Value provided must be one of the Vision One regions, e.g. `us-east-1`, `eu-central-1`, `ap-southeast-1`, `ap-southeast-2`, `ap-northeast-1` | Yes, either -r or -a |
-   | --addr or -a   | Trend Vision One File Security server, such as: antimalware.__REGION__.cloudone.trendmicro.com:443 | Yes, either -r or -a      |
-   | --api_key      | Vision One API Key              | No       |
-   | --filename or -f |        File to be scanned            | No       |
+   | Command Line Arguments | Value                                                                                                                                                                               | Optional             |
+   |------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------|
+   | --region or -r         | The region you obtained your API key.  Value provided must be one of the Vision One regions, e.g. `us-east-1`, `eu-central-1`, `ap-southeast-1`, `ap-southeast-2`, `ap-northeast-1` | Yes, either -r or -a |
+   | --addr or -a           | Trend Vision One File Security server, such as: antimalware.__REGION__.cloudone.trendmicro.com:443                                                                                  | Yes, either -r or -a |
+   | --api_key              | Vision One API Key                                                                                                                                                                  | No                   |
+   | --filename or -f       | File to be scanned                                                                                                                                                                  | No                   |
+   | --pml                  | Predictive Machine Learning                                                                                                                                                         | Yes                  |
+   | --tags or -f           | List of tags                                                                                                                                                                        | Yes                  |
 
 4. Run one of the examples.
 
    Make sure to customize the example program by configuring it with the API key from your Vision One account, found in your Vision One Dashboard. Assign the value of your Vision One Region's `API_KEY` to the variable and set `FILENAME` to the desired target file.
 
    ```sh
    python3 client.py -f FILENAME -r us-east-1 --tls true --api_key API_KEY
@@ -78,50 +80,7 @@
    or
 
    using asynchronous IO example program:
 
    ```sh
    python3 client_aio.py -f FILENAME -a antimalware._REGION_.cloudone.trendmicro.com:443 --tls true --api_key API_KEY
    ```
-
-### Code Examples
-
-```python
-import json
-import amaas.grpc
-
-handle = amaas.grpc.init(YOUR_FILE_SECURITY_SERVER, YOUR_VISION_ONE_KEY, True)
-
-result = amaas.grpc.scan_file(args.filename, handle)
-print(result)
-
-result_json = json.loads(result)
-print("Got scan result: %d" % result_json['scanResult'])
-
-amaas.grpc.quit(handle)
-
-```
-
-to use asyncio with  coroutines and tasks,
-
-```python:
-import json
-import pprint
-import asyncio
-import amaas.grpc.aio
-
-async def scan_files():
-   handle = amaas.grpc.aio.init(YOUR_FILE_SECURITY_SERVER, YOUR_VISION_ONE_KEY, True)
-
-   tasks = [asyncio.create_task(amaas.grpc.aio.scan_file(file_name, handle))]
-
-   scan_results = await asyncio.gather(*tasks)
-
-   for scan_result in scan_results:
-      pprint.pprint(json.loads(scan_result))
-
-   await amaas.grpc.aio.quit(handle)
-
-
-asyncio.run(scan_files())
-
-```
```

### Comparing `visionone-filesecurity-1.0.2/amaas/grpc/__init__.py` & `visionone-filesecurity-1.1.0/amaas/grpc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,41 +52,64 @@
     return _init_by_region_util(region, api_key, enable_tls, ca_cert, False)
 
 
 def init(host, api_key=None, enable_tls=False, ca_cert=None):
     return _init_util(host, api_key, enable_tls, ca_cert, False)
 
 
-def _generate_messages(pipeline: _Pipeline, data_reader: BinaryIO, stats: dict) -> None:
+def _generate_messages(pipeline: _Pipeline, data_reader: BinaryIO, bulk: bool, stats: dict) -> None:
+    responses = []
+
     while True:
+        for r in responses:
+            if r[0] == "INIT":
+                response = r[1]
+            elif r[0] == "RUN":
+                offset = r[1]
+                length = r[2]
+                data_reader.seek(offset)
+                chunk = data_reader.read(length)
+                response = scan_pb2.C2S(
+                    stage=scan_pb2.STAGE_RUN,
+                    file_name=None,
+                    rs_size=0,
+                    offset=offset,
+                    chunk=chunk,
+                )
+                stats["total_upload"] = stats.get("total_upload", 0) + len(chunk)
+            else:
+                raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNEXPECTED_CMD_AND_STAGE, "None", r[0])
+            yield response
+
+        responses.clear()
         message = pipeline.get_message()
 
         if message.stage == scan_pb2.STAGE_INIT:
             logger.debug("stage INIT")
-            yield message
+            responses.append(("INIT", message))
         elif message.stage == scan_pb2.STAGE_RUN:
             if message.cmd != scan_pb2.CMD_RETR:
                 raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNEXPECTED_CMD_AND_STAGE, message.cmd, message.stage)
 
-            logger.debug(
-                f"stage RUN, try to read {message.length} at offset {message.offset}")
+            length = []
+            offset = []
 
-            data_reader.seek(message.offset)
-            chunk = data_reader.read(message.length)
+            if bulk:
+                offset = message.bulk_offset[:]
+                length = message.bulk_length[:]
+
+                if len(length) > 1:
+                    logger.debug("bulk transfer triggered")
+            else:
+                offset.append(message.offset)
+                length.append(message.length)
 
-            message = scan_pb2.C2S(
-                stage=scan_pb2.STAGE_RUN,
-                file_name=None,
-                rs_size=0,
-                offset=data_reader.tell(),
-                chunk=chunk)
-
-            stats["total_upload"] = stats.get(
-                "total_upload", 0) + len(chunk)
-            yield message
+            for i in range(len(length)):
+                logger.debug(f"stage RUN, try to read {length[i]} at offset {offset[i]}")
+                responses.append(("RUN", offset[i], length[i]))
         elif message.stage == scan_pb2.STAGE_FINI:
             if message.cmd != scan_pb2.CMD_QUIT:
                 raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNEXPECTED_CMD_AND_STAGE, message.cmd, message.stage)
 
             logger.debug("final stage, quit generating C2S messages...")
             break
         else:
@@ -95,45 +118,49 @@
 
 
 def quit(handle):
     handle.close()
 
 
 def _scan_data(channel: grpc.Channel, data_reader: BinaryIO, size: int, identifier: str, tags: List[str],
-               app_name: str) -> str:
+               pml: bool, feedback: bool) -> str:
     _validate_tags(tags)
     stub = scan_pb2_grpc.ScanStub(channel)
     pipeline = _Pipeline()
     stats = {}
     result = None
+    bulk = True
 
     try:
         metadata = (
-            (APP_NAME_HEADER, app_name),
+            (APP_NAME_HEADER, APP_NAME_FILE_SCAN),
         )
-        responses = stub.Run(_generate_messages(pipeline, data_reader, stats), timeout=timeout_in_seconds,
+        responses = stub.Run(_generate_messages(pipeline, data_reader, bulk, stats), timeout=timeout_in_seconds,
                              metadata=metadata)
         message = scan_pb2.C2S(stage=scan_pb2.STAGE_INIT,
                                file_name=identifier,
                                rs_size=size,
                                offset=0,
                                chunk=None,
+                               trendx=pml,
                                tags=tags,
                                file_sha1="sha1:" + _digest_hex(data_reader, "sha1"),
-                               file_sha256="sha256:" + _digest_hex(data_reader, "sha256"))
+                               file_sha256="sha256:" + _digest_hex(data_reader, "sha256"),
+                               bulk=bulk,
+                               spn_feedback=feedback)
 
         pipeline.set_message(message)
 
         for response in responses:
             if response.cmd == scan_pb2.CMD_RETR:
                 pipeline.set_message(response)
             elif response.cmd == scan_pb2.CMD_QUIT:
                 result = response.result
                 pipeline.set_message(response)
-                logger.debug("receive QUIT, exit loop...\n")
+                logger.debug("receive QUIT, exit loop...")
                 break
             else:
                 logger.debug("unknown command...")
                 raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNKNOWN_CMD, response.cmd)
 
         total_upload = stats.get("total_upload", 0)
         logger.debug(f"total upload {total_upload} bytes")
@@ -149,26 +176,27 @@
             raise AMaasException(AMaasErrorCode.MSG_ID_GRPC_ERROR, rpc_error.code().value[0], rpc_error.details())
     except Exception as err:
         raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNEXPECTED_ERROR, str(err))
 
     return result
 
 
-def scan_file(channel: grpc.Channel, file_name: str, tags: List[str] = None, app_name: str = APP_NAME_FILE_SCAN) -> str:
+def scan_file(channel: grpc.Channel, file_name: str, tags: List[str] = None,
+              pml: bool = False, feedback: bool = False) -> str:
     try:
         f = open(file_name, "rb")
         fid = os.path.basename(file_name)
         n = os.stat(file_name).st_size
     except FileNotFoundError as err:
         logger.debug("File not exist: " + str(err))
         raise AMaasException(AMaasErrorCode.MSG_ID_ERR_FILE_NOT_FOUND, file_name)
     except (PermissionError, IOError) as err:
         logger.debug("Permission error: " + str(err))
         raise AMaasException(AMaasErrorCode.MSG_ID_ERR_FILE_NO_PERMISSION, file_name)
 
-    return _scan_data(channel, f, n, fid, tags, app_name)
+    return _scan_data(channel, f, n, fid, tags, pml, feedback)
 
 
 def scan_buffer(channel: grpc.Channel, bytes_buffer: bytes, uid: str, tags: List[str] = None,
-                app_name: str = APP_NAME_FILE_SCAN) -> str:
+                pml: bool = False, feedback: bool = False) -> str:
     f = io.BytesIO(bytes_buffer)
-    return _scan_data(channel, f, len(bytes_buffer), uid, tags, app_name)
+    return _scan_data(channel, f, len(bytes_buffer), uid, tags, pml, feedback)
```

### Comparing `visionone-filesecurity-1.0.2/amaas/grpc/aio/__init__.py` & `visionone-filesecurity-1.1.0/amaas/grpc/aio/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,65 +36,87 @@
     await handle.close()
 
 
 # https://github.com/grpc/grpc/blob/91083659fa88c938779dd41e57a7f97981b6c9a1/src/python/grpcio_tests/tests_aio/unit/channel_test.py#L180
 
 
 async def _scan_data(channel: grpc.Channel, data_reader: BinaryIO, size: int, identifier: str, tags: List[str],
-                     app_name: str) -> str:
+                     pml: bool, feedback: bool) -> str:
     _validate_tags(tags)
     stub = scan_pb2_grpc.ScanStub(channel)
     stats = {}
     result = None
+    bulk = True
+
     try:
         metadata = (
-            (APP_NAME_HEADER, app_name),
+            (APP_NAME_HEADER, APP_NAME_FILE_SCAN),
         )
         call = stub.Run(timeout=timeout_in_seconds, metadata=metadata)
 
         request = scan_pb2.C2S(stage=scan_pb2.STAGE_INIT,
                                file_name=identifier,
                                rs_size=size,
                                offset=0,
                                chunk=None,
                                tags=tags,
+                               trendx=pml,
                                file_sha1="sha1:" + _digest_hex(data_reader, "sha1"),
-                               file_sha256="sha256:" + _digest_hex(data_reader, "sha256"))
+                               file_sha256="sha256:" + _digest_hex(data_reader, "sha256"),
+                               bulk=bulk,
+                               spn_feedback=feedback)
 
         await call.write(request)
 
         while True:
             response = await call.read()
 
             if response.cmd == scan_pb2.CMD_RETR:
                 if response.stage != scan_pb2.STAGE_RUN:
                     raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNEXPECTED_CMD_AND_STAGE, response.cmd,
                                          response.stage)
-                logger.debug(
-                    f"stage RUN, try to read {response.length} at offset {response.offset}")
+                length = []
+                offset = []
+
+                if bulk:
+                    logger.debug("enter bulk mode")
+                    bulk_count = len(response.bulk_offset)
+
+                    if bulk_count > 1:
+                        logger.debug("bulk transfer triggered")
+
+                    length = response.bulk_length[:]
+                    offset = response.bulk_offset[:]
+                else:
+                    logger.debug("enter non-bulk mode")
+                    length.append(response.length)
+                    offset.append(response.offset)
+
+                for i in range(len(length)):
+                    logger.debug(f"try to read {length[i]} at offset {offset[i]}")
+                    data_reader.seek(offset[i])
+                    chunk = data_reader.read(length[i])
+
+                    request = scan_pb2.C2S(
+                        stage=scan_pb2.STAGE_RUN,
+                        file_name=None,
+                        rs_size=0,
+                        offset=offset[i],
+                        chunk=chunk)
 
-                data_reader.seek(response.offset)
-                chunk = data_reader.read(response.length)
+                    stats["total_upload"] = stats.get(
+                        "total_upload", 0) + len(chunk)
 
-                request = scan_pb2.C2S(
-                    stage=scan_pb2.STAGE_RUN,
-                    file_name=None,
-                    rs_size=0,
-                    offset=data_reader.tell(),
-                    chunk=chunk)
-
-                stats["total_upload"] = stats.get(
-                    "total_upload", 0) + len(chunk)
-                await call.write(request)
+                    await call.write(request)
             elif response.cmd == scan_pb2.CMD_QUIT:
                 if response.stage != scan_pb2.STAGE_FINI:
                     raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNEXPECTED_CMD_AND_STAGE, response.cmd,
                                          response.stage)
                 result = response.result
-                logger.debug("receive QUIT, exit loop...\n")
+                logger.debug("receive QUIT, exit loop...")
                 break
             else:
                 logger.debug("unknown command...")
                 raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNKNOWN_CMD, response.cmd)
 
         await call.done_writing()
 
@@ -113,25 +135,25 @@
     except Exception as err:
         raise AMaasException(AMaasErrorCode.MSG_ID_ERR_UNEXPECTED_ERROR, str(err))
 
     return result
 
 
 async def scan_file(channel: grpc.Channel, file_name: str, tags: List[str] = None,
-                    app_name: str = APP_NAME_FILE_SCAN) -> str:
+                    pml: bool = False, feedback: bool = False) -> str:
     try:
         f = open(file_name, "rb")
         fid = os.path.basename(file_name)
         n = os.stat(file_name).st_size
     except FileNotFoundError as err:
         logger.debug("File not exist: " + str(err))
         raise AMaasException(AMaasErrorCode.MSG_ID_ERR_FILE_NOT_FOUND, file_name)
     except (PermissionError, IOError) as err:
         logger.debug("Permission error: " + str(err))
         raise AMaasException(AMaasErrorCode.MSG_ID_ERR_FILE_NO_PERMISSION, file_name)
-    return await _scan_data(channel, f, n, fid, tags, app_name)
+    return await _scan_data(channel, f, n, fid, tags, pml, feedback)
 
 
 async def scan_buffer(channel: grpc.Channel, bytes_buffer: bytes, uid: str, tags: List[str] = None,
-                      app_name: str = APP_NAME_FILE_SCAN) -> str:
+                      pml: bool = False, feedback: bool = False) -> str:
     f = io.BytesIO(bytes_buffer)
-    return await _scan_data(channel, f, len(bytes_buffer), uid, tags, app_name)
+    return await _scan_data(channel, f, len(bytes_buffer), uid, tags, pml, feedback)
```

### Comparing `visionone-filesecurity-1.0.2/amaas/grpc/exception/__init__.py` & `visionone-filesecurity-1.1.0/amaas/grpc/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.0.2/amaas/grpc/protos/scan_pb2.py` & `visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: amaas/grpc/protos/scan.proto
+# Protobuf Python Version: 4.25.0
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x61maas/grpc/protos/scan.proto\x12\ramaas.scan.v1\"\xb3\x01\n\x03\x43\x32S\x12#\n\x05stage\x18\x01 \x01(\x0e\x32\x14.amaas.scan.v1.Stage\x12\x11\n\tfile_name\x18\x02 \x01(\t\x12\x0f\n\x07rs_size\x18\x03 \x01(\x05\x12\x0e\n\x06offset\x18\x04 \x01(\x05\x12\r\n\x05\x63hunk\x18\x05 \x01(\x0c\x12\x0e\n\x06trendx\x18\x06 \x01(\x08\x12\x11\n\tfile_sha1\x18\x07 \x01(\t\x12\x13\n\x0b\x66ile_sha256\x18\x08 \x01(\t\x12\x0c\n\x04tags\x18\t \x03(\t\"\x7f\n\x03S2C\x12#\n\x05stage\x18\x01 \x01(\x0e\x32\x14.amaas.scan.v1.Stage\x12#\n\x03\x63md\x18\x02 \x01(\x0e\x32\x16.amaas.scan.v1.Command\x12\x0e\n\x06offset\x18\x03 \x01(\x05\x12\x0e\n\x06length\x18\x04 \x01(\x05\x12\x0e\n\x06result\x18\x05 \x01(\t*6\n\x05Stage\x12\x0e\n\nSTAGE_INIT\x10\x00\x12\r\n\tSTAGE_RUN\x10\x01\x12\x0e\n\nSTAGE_FINI\x10\x02*%\n\x07\x43ommand\x12\x0c\n\x08\x43MD_RETR\x10\x00\x12\x0c\n\x08\x43MD_QUIT\x10\x01\x32;\n\x04Scan\x12\x33\n\x03Run\x12\x12.amaas.scan.v1.C2S\x1a\x12.amaas.scan.v1.S2C\"\x00(\x01\x30\x01\x42\x33\n\x1d\x63om.trend.cloudone.amaas.scanZ\x12\x61maas/scanner/baseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x61maas/grpc/protos/scan.proto\x12\ramaas.scan.v1\"\xd7\x01\n\x03\x43\x32S\x12#\n\x05stage\x18\x01 \x01(\x0e\x32\x14.amaas.scan.v1.Stage\x12\x11\n\tfile_name\x18\x02 \x01(\t\x12\x0f\n\x07rs_size\x18\x03 \x01(\x04\x12\x0e\n\x06offset\x18\x04 \x01(\x05\x12\r\n\x05\x63hunk\x18\x05 \x01(\x0c\x12\x0e\n\x06trendx\x18\x06 \x01(\x08\x12\x11\n\tfile_sha1\x18\x07 \x01(\t\x12\x13\n\x0b\x66ile_sha256\x18\x08 \x01(\t\x12\x0c\n\x04tags\x18\t \x03(\t\x12\x0c\n\x04\x62ulk\x18\n \x01(\x08\x12\x14\n\x0cspn_feedback\x18\x0b \x01(\x08\"\xbd\x01\n\x03S2C\x12#\n\x05stage\x18\x01 \x01(\x0e\x32\x14.amaas.scan.v1.Stage\x12#\n\x03\x63md\x18\x02 \x01(\x0e\x32\x16.amaas.scan.v1.Command\x12\x0e\n\x06offset\x18\x03 \x01(\x05\x12\x0e\n\x06length\x18\x04 \x01(\x05\x12\x0e\n\x06result\x18\x05 \x01(\t\x12\x13\n\x0b\x62ulk_offset\x18\x06 \x03(\x05\x12\x13\n\x0b\x62ulk_length\x18\x07 \x03(\x05\x12\x12\n\nsession_id\x18\x08 \x01(\t*6\n\x05Stage\x12\x0e\n\nSTAGE_INIT\x10\x00\x12\r\n\tSTAGE_RUN\x10\x01\x12\x0e\n\nSTAGE_FINI\x10\x02*%\n\x07\x43ommand\x12\x0c\n\x08\x43MD_RETR\x10\x00\x12\x0c\n\x08\x43MD_QUIT\x10\x01\x32;\n\x04Scan\x12\x33\n\x03Run\x12\x12.amaas.scan.v1.C2S\x1a\x12.amaas.scan.v1.S2C\"\x00(\x01\x30\x01\x42\x33\n\x1d\x63om.trend.cloudone.amaas.scanZ\x12\x61maas/scanner/baseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'amaas.grpc.protos.scan_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\035com.trend.cloudone.amaas.scanZ\022amaas/scanner/base'
-  _globals['_STAGE']._serialized_start=358
-  _globals['_STAGE']._serialized_end=412
-  _globals['_COMMAND']._serialized_start=414
-  _globals['_COMMAND']._serialized_end=451
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\035com.trend.cloudone.amaas.scanZ\022amaas/scanner/base'
+  _globals['_STAGE']._serialized_start=457
+  _globals['_STAGE']._serialized_end=511
+  _globals['_COMMAND']._serialized_start=513
+  _globals['_COMMAND']._serialized_end=550
   _globals['_C2S']._serialized_start=48
-  _globals['_C2S']._serialized_end=227
-  _globals['_S2C']._serialized_start=229
-  _globals['_S2C']._serialized_end=356
-  _globals['_SCAN']._serialized_start=453
-  _globals['_SCAN']._serialized_end=512
+  _globals['_C2S']._serialized_end=263
+  _globals['_S2C']._serialized_start=266
+  _globals['_S2C']._serialized_end=455
+  _globals['_SCAN']._serialized_start=552
+  _globals['_SCAN']._serialized_end=611
 # @@protoc_insertion_point(module_scope)
```

### Comparing `visionone-filesecurity-1.0.2/amaas/grpc/protos/scan_pb2.pyi` & `visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -3,57 +3,67 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Stage(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+    __slots__ = ()
     STAGE_INIT: _ClassVar[Stage]
     STAGE_RUN: _ClassVar[Stage]
     STAGE_FINI: _ClassVar[Stage]
 
 class Command(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+    __slots__ = ()
     CMD_RETR: _ClassVar[Command]
     CMD_QUIT: _ClassVar[Command]
 STAGE_INIT: Stage
 STAGE_RUN: Stage
 STAGE_FINI: Stage
 CMD_RETR: Command
 CMD_QUIT: Command
 
 class C2S(_message.Message):
-    __slots__ = ["stage", "file_name", "rs_size", "offset", "chunk", "trendx", "file_sha1", "file_sha256", "tags"]
+    __slots__ = ("stage", "file_name", "rs_size", "offset", "chunk", "trendx", "file_sha1", "file_sha256", "tags", "bulk", "spn_feedback")
     STAGE_FIELD_NUMBER: _ClassVar[int]
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     RS_SIZE_FIELD_NUMBER: _ClassVar[int]
     OFFSET_FIELD_NUMBER: _ClassVar[int]
     CHUNK_FIELD_NUMBER: _ClassVar[int]
     TRENDX_FIELD_NUMBER: _ClassVar[int]
     FILE_SHA1_FIELD_NUMBER: _ClassVar[int]
     FILE_SHA256_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
+    BULK_FIELD_NUMBER: _ClassVar[int]
+    SPN_FEEDBACK_FIELD_NUMBER: _ClassVar[int]
     stage: Stage
     file_name: str
     rs_size: int
     offset: int
     chunk: bytes
     trendx: bool
     file_sha1: str
     file_sha256: str
     tags: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, stage: _Optional[_Union[Stage, str]] = ..., file_name: _Optional[str] = ..., rs_size: _Optional[int] = ..., offset: _Optional[int] = ..., chunk: _Optional[bytes] = ..., trendx: bool = ..., file_sha1: _Optional[str] = ..., file_sha256: _Optional[str] = ..., tags: _Optional[_Iterable[str]] = ...) -> None: ...
+    bulk: bool
+    spn_feedback: bool
+    def __init__(self, stage: _Optional[_Union[Stage, str]] = ..., file_name: _Optional[str] = ..., rs_size: _Optional[int] = ..., offset: _Optional[int] = ..., chunk: _Optional[bytes] = ..., trendx: bool = ..., file_sha1: _Optional[str] = ..., file_sha256: _Optional[str] = ..., tags: _Optional[_Iterable[str]] = ..., bulk: bool = ..., spn_feedback: bool = ...) -> None: ...
 
 class S2C(_message.Message):
-    __slots__ = ["stage", "cmd", "offset", "length", "result"]
+    __slots__ = ("stage", "cmd", "offset", "length", "result", "bulk_offset", "bulk_length", "session_id")
     STAGE_FIELD_NUMBER: _ClassVar[int]
     CMD_FIELD_NUMBER: _ClassVar[int]
     OFFSET_FIELD_NUMBER: _ClassVar[int]
     LENGTH_FIELD_NUMBER: _ClassVar[int]
     RESULT_FIELD_NUMBER: _ClassVar[int]
+    BULK_OFFSET_FIELD_NUMBER: _ClassVar[int]
+    BULK_LENGTH_FIELD_NUMBER: _ClassVar[int]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     stage: Stage
     cmd: Command
     offset: int
     length: int
     result: str
-    def __init__(self, stage: _Optional[_Union[Stage, str]] = ..., cmd: _Optional[_Union[Command, str]] = ..., offset: _Optional[int] = ..., length: _Optional[int] = ..., result: _Optional[str] = ...) -> None: ...
+    bulk_offset: _containers.RepeatedScalarFieldContainer[int]
+    bulk_length: _containers.RepeatedScalarFieldContainer[int]
+    session_id: str
+    def __init__(self, stage: _Optional[_Union[Stage, str]] = ..., cmd: _Optional[_Union[Command, str]] = ..., offset: _Optional[int] = ..., length: _Optional[int] = ..., result: _Optional[str] = ..., bulk_offset: _Optional[_Iterable[int]] = ..., bulk_length: _Optional[_Iterable[int]] = ..., session_id: _Optional[str] = ...) -> None: ...
```

### Comparing `visionone-filesecurity-1.0.2/amaas/grpc/protos/scan_pb2_grpc.py` & `visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.0.2/amaas/grpc/util.py` & `visionone-filesecurity-1.1.0/amaas/grpc/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 C1_CA_REGION = "ca-1"
 C1_TREND_REGION = "trend-us-1"
 C1_GB_REGION = "gb-1"
 
 C1Regions = [C1_AU_REGION, C1_CA_REGION, C1_DE_REGION, C1_GB_REGION, C1_IN_REGION, C1_JP_REGION, C1_SG_REGION,
              C1_US_REGION, C1_TREND_REGION]
 V1Regions = [AWS_AU_REGION, AWS_DE_REGION, AWS_IN_REGION, AWS_JP_REGION, AWS_SG_REGION, AWS_US_REGION]
-SupportedV1Regions = [AWS_AU_REGION, AWS_DE_REGION, AWS_JP_REGION, AWS_SG_REGION, AWS_US_REGION]
+SupportedV1Regions = V1Regions
 SupportedC1Regions = [C1_AU_REGION, C1_CA_REGION, C1_DE_REGION, C1_GB_REGION, C1_IN_REGION, C1_JP_REGION, C1_SG_REGION,
                       C1_US_REGION]
 
 AllRegions = C1Regions + V1Regions
 AllValidRegions = SupportedC1Regions + SupportedV1Regions
 
 V1ToC1RegionMapping = {AWS_AU_REGION: C1_AU_REGION,
```

### Comparing `visionone-filesecurity-1.0.2/setup.py` & `visionone-filesecurity-1.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-import re
-from os.path import abspath, dirname, join
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-
-base_dir = abspath(dirname(__file__))
-package_name = "amaas"
-
-with open(join(base_dir, package_name, "_version.py")) as f:
-    package_version = re.search(
-        r"__version__\s+=\s+[\"\']([^\"\']+)[\"\']", f.read()
-    ).group(1)
-
-setup(install_requires=['grpcio==1.56.2', 'protobuf==4.23.4'],
-      name="visionone-filesecurity",
-      version=package_version,
-      author="Trend Micro VisionOne File Security Team",
-      description="Trend Micro VisionOne File Security SDK for python",
-      long_description=long_description,
-      long_description_content_type="text/markdown",
-      url="https://github.com/trendmicro/tm-v1-fs-python-sdk",
-      packages=find_namespace_packages(exclude=['tests*', 'examples']),
-      package_data={'amaas': ['grpc/protos/*']},
-      include_package_data=True,
-      classifiers=[
-          'Programming Language :: Python',
-          'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
-          'Programming Language :: Python :: 3.10',
-          'Programming Language :: Python :: 3.11',
-          "License :: OSI Approved :: MIT License",
-],
-    python_requires='>=3.7',
-)
+with open("VERSION", "r") as fh:
+    package_version = fh.read().strip()
+setup(install_requires=['grpcio==1.60.0', 'protobuf==4.25.1'],
+    name="visionone-filesecurity",
+    version=package_version,
+    author="Trend Micro VisionOne File Security Team",
+    description="Trend Micro VisionOne File Security SDK for python",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/trendmicro/tm-v1-fs-python-sdk",
+    packages=find_namespace_packages(exclude=["tests*", "examples"]),
+    package_data={"amaas": ["grpc/protos/*"]},
+    include_package_data=True,
+    classifiers=[
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+    ],
+    python_requires=">=3.7",
+)
```

### Comparing `visionone-filesecurity-1.0.2/visionone_filesecurity.egg-info/PKG-INFO` & `visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionone-filesecurity
-Version: 1.0.2
+Version: 1.1.0
 Summary: Trend Micro VisionOne File Security SDK for python
 Home-page: https://github.com/trendmicro/tm-v1-fs-python-sdk
 Author: Trend Micro VisionOne File Security Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -35,26 +35,26 @@
 
    ```sh
    python -m pip install visionone-filesecurity
    ```
 
 ## Obtain an API Key
 
-The File Security SDK requires a valid API Key provided as parameter to the SDK client object. It can accept Trend Vision One API keys. 
+The File Security SDK requires a valid API Key provided as parameter to the SDK client object. It can accept Trend Vision One API keys.
 
 When obtaining the API Key, ensure that the API Key is associated with the region that you plan to use. It is important to note that Trend Vision One API Keys are associated with different regions, please refer to the region flag below to obtain a better understanding of the valid regions associated with the respective API Key.
 
 If you plan on using a Trend Vision One region, be sure to pass in region parameter when running custom program with File Security SDK to specify the region of that API key and to ensure you have proper authorization. The list of supported Trend Vision One regions can be found at API Reference section below.
 
 1. Login to the Trend Vision One.
 2. Create a new Trend Vision One API key:
 
-* Navigate to the Trend Vision One User Roles page.
-* Verify that there is a role with the "Run file scan via SDK" permissions enabled. If not, create a role by clicking on "Add Role" and "Save" once finished.
-* Directly configure a new key on the Trend Vision One API Keys page, using the role which contains the "Run file scan via SDK" permission. It is advised to set an expiry time for the API key and make a record of it for future reference.
+- Navigate to the Trend Vision One User Roles page.
+- Verify that there is a role with the "Run file scan via SDK" permissions enabled. If not, create a role by clicking on "Add Role" and "Save" once finished.
+- Directly configure a new key on the Trend Vision One API Keys page, using the role which contains the "Run file scan via SDK" permission. It is advised to set an expiry time for the API key and make a record of it for future reference.
 
 ## Run SDK
 
 ### Run with File Security SDK examples
 
 1. Go to `/examples/` in current directory.
 
@@ -67,20 +67,22 @@
    ```text
    client_aio.py
    client.py
    ```
 
 3. Current Python examples support following command line arguments
 
-   | Command Line Arguments                 | Value                    | Optional |
-   | :------------------ | :----------------------- | :------- |
-   | --region or -r | The region you obtained your API key.  Value provided must be one of the Vision One regions, e.g. `us-east-1`, `eu-central-1`, `ap-southeast-1`, `ap-southeast-2`, `ap-northeast-1` | Yes, either -r or -a |
-   | --addr or -a   | Trend Vision One File Security server, such as: antimalware.__REGION__.cloudone.trendmicro.com:443 | Yes, either -r or -a      |
-   | --api_key      | Vision One API Key              | No       |
-   | --filename or -f |        File to be scanned            | No       |
+   | Command Line Arguments | Value                                                                                                                                                                               | Optional             |
+   |------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------|
+   | --region or -r         | The region you obtained your API key.  Value provided must be one of the Vision One regions, e.g. `us-east-1`, `eu-central-1`, `ap-southeast-1`, `ap-southeast-2`, `ap-northeast-1` | Yes, either -r or -a |
+   | --addr or -a           | Trend Vision One File Security server, such as: antimalware.__REGION__.cloudone.trendmicro.com:443                                                                                  | Yes, either -r or -a |
+   | --api_key              | Vision One API Key                                                                                                                                                                  | No                   |
+   | --filename or -f       | File to be scanned                                                                                                                                                                  | No                   |
+   | --pml                  | Predictive Machine Learning                                                                                                                                                         | Yes                  |
+   | --tags or -f           | List of tags                                                                                                                                                                        | Yes                  |
 
 4. Run one of the examples.
 
    Make sure to customize the example program by configuring it with the API key from your Vision One account, found in your Vision One Dashboard. Assign the value of your Vision One Region's `API_KEY` to the variable and set `FILENAME` to the desired target file.
 
    ```sh
    python3 client.py -f FILENAME -r us-east-1 --tls true --api_key API_KEY
@@ -97,50 +99,7 @@
    or
 
    using asynchronous IO example program:
 
    ```sh
    python3 client_aio.py -f FILENAME -a antimalware._REGION_.cloudone.trendmicro.com:443 --tls true --api_key API_KEY
    ```
-
-### Code Examples
-
-```python
-import json
-import amaas.grpc
-
-handle = amaas.grpc.init(YOUR_FILE_SECURITY_SERVER, YOUR_VISION_ONE_KEY, True)
-
-result = amaas.grpc.scan_file(args.filename, handle)
-print(result)
-
-result_json = json.loads(result)
-print("Got scan result: %d" % result_json['scanResult'])
-
-amaas.grpc.quit(handle)
-
-```
-
-to use asyncio with  coroutines and tasks,
-
-```python:
-import json
-import pprint
-import asyncio
-import amaas.grpc.aio
-
-async def scan_files():
-   handle = amaas.grpc.aio.init(YOUR_FILE_SECURITY_SERVER, YOUR_VISION_ONE_KEY, True)
-
-   tasks = [asyncio.create_task(amaas.grpc.aio.scan_file(file_name, handle))]
-
-   scan_results = await asyncio.gather(*tasks)
-
-   for scan_result in scan_results:
-      pprint.pprint(json.loads(scan_result))
-
-   await amaas.grpc.aio.quit(handle)
-
-
-asyncio.run(scan_files())
-
-```
```

