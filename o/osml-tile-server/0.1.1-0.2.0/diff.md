# Comparing `tmp/osml-tile-server-0.1.1.tar.gz` & `tmp/osml-tile-server-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osml-tile-server-0.1.1.tar", last modified: Fri Feb 16 18:42:16 2024, max compression
+gzip compressed data, was "osml-tile-server-0.2.0.tar", last modified: Thu Apr  4 19:45:09 2024, max compression
```

## Comparing `osml-tile-server-0.1.1.tar` & `osml-tile-server-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.841102 osml-tile-server-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-02-16 18:42:16.841102 osml-tile-server-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-16 18:42:16.845102 osml-tile-server-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.837102 osml-tile-server-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.837102 osml-tile-server-0.1.1/src/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.837102 osml-tile-server-0.1.1/src/aws/osml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.837102 osml-tile-server-0.1.1/src/aws/osml/tile_server/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.837102 osml-tile-server-0.1.1/src/aws/osml/tile_server/lambda/
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/lambda/cleanup_dlq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.841102 osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/aws_services.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/string_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/tile_server_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.841102 osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    21153 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20691 2024-02-16 18:42:05.000000 osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:42:16.841102 osml-tile-server-0.1.1/src/osml_tile_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-02-16 18:42:16.000000 osml-tile-server-0.1.1/src/osml_tile_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-16 18:42:16.000000 osml-tile-server-0.1.1/src/osml_tile_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 18:42:16.000000 osml-tile-server-0.1.1/src/osml_tile_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 18:42:16.000000 osml-tile-server-0.1.1/src/osml_tile_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-16 18:42:16.000000 osml-tile-server-0.1.1/src/osml_tile_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-16 18:42:16.000000 osml-tile-server-0.1.1/src/osml_tile_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.661043 osml-tile-server-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-04 19:45:09.661043 osml-tile-server-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-04 19:45:09.665043 osml-tile-server-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.657043 osml-tile-server-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.657043 osml-tile-server-0.2.0/src/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.657043 osml-tile-server-0.2.0/src/aws/osml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.657043 osml-tile-server-0.2.0/src/aws/osml/tile_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.657043 osml-tile-server-0.2.0/src/aws/osml/tile_server/lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/lambda/cleanup_dlq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.661043 osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/aws_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/log_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/string_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/tile_server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.661043 osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21319 2024-04-04 19:45:04.000000 osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:45:09.661043 osml-tile-server-0.2.0/src/osml_tile_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-04 19:45:09.000000 osml-tile-server-0.2.0/src/osml_tile_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-04 19:45:09.000000 osml-tile-server-0.2.0/src/osml_tile_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:45:09.000000 osml-tile-server-0.2.0/src/osml_tile_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:45:09.000000 osml-tile-server-0.2.0/src/osml_tile_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 19:45:09.000000 osml-tile-server-0.2.0/src/osml_tile_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 19:45:09.000000 osml-tile-server-0.2.0/src/osml_tile_server.egg-info/top_level.txt
```

### Comparing `osml-tile-server-0.1.1/LICENSE` & `osml-tile-server-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osml-tile-server-0.1.1/PKG-INFO` & `osml-tile-server-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-tile-server
-Version: 0.1.1
+Version: 0.2.0
 Summary: The OversightML Tile Server is a lightweight, cloud-based tile server which allows you to quickly pass an image from S3 bucket to get metadata, image statistics, and set of tiles in real-time.
 Author: Amazon Web Services
 Author-email: aws-osml-admin@amazon.com
 License: 
         © 2023 Amazon Web Services, Inc. or its affiliates. All Rights Reserved.
         This AWS Content is provided subject to the terms of the AWS Customer Agreement
         available at http://aws.amazon.com/agreement or other written agreement between
@@ -15,18 +15,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: uvicorn
 Requires-Dist: fastapi
 Requires-Dist: fastapi-versioning
+Requires-Dist: asgi-correlation-id
 Requires-Dist: starlette[full]
 Requires-Dist: cryptography
 Requires-Dist: boto3
 Requires-Dist: geojson>=3.0.0
+Requires-Dist: pydantic>=2.0.0
+Requires-Dist: python-json-logger>=2.0.0
 Requires-Dist: osml-imagery-toolkit>=1.2
 Provides-Extra: test
 Requires-Dist: tox; extra == "test"
 
 # OversightML Tile Server
 
 The OversightML Tile Server (TS) is a lightweight, cloud-based tile server which allows you to quickly pass an image from S3 bucket to get metadata, image statistics, and set of tiles in real-time.
```

### Comparing `osml-tile-server-0.1.1/README.md` & `osml-tile-server-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `osml-tile-server-0.1.1/setup.cfg` & `osml-tile-server-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osml-tile-server
-version = 0.1.1
+version = 0.2.0
 description = The OversightML Tile Server is a lightweight, cloud-based tile server which allows you to quickly pass an image from S3 bucket to get metadata, image statistics, and set of tiles in real-time.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Amazon Web Services
 author_email = aws-osml-admin@amazon.com
 license = 
 	© 2023 Amazon Web Services, Inc. or its affiliates. All Rights Reserved.
@@ -25,18 +25,21 @@
 packages = find_namespace:
 python_requires = >=3.9
 include_package_data = True
 install_requires = 
 	uvicorn
 	fastapi
 	fastapi-versioning
+	asgi-correlation-id
 	starlette[full]
 	cryptography
 	boto3
 	geojson>=3.0.0
+	pydantic>=2.0.0
+	python-json-logger>=2.0.0
 	osml-imagery-toolkit>=1.2
 
 [options.packages.find]
 where = src
 exclude = 
 	test
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/app_config.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/app_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 import os
 from dataclasses import dataclass
 
 from botocore.config import Config
 
 
@@ -25,14 +27,21 @@
     aws_region: str = os.getenv("AWS_DEFAULT_REGION", "us-west-2")
     viewpoint_status_table: str = os.getenv("JOB_TABLE", "TSJobTable")
     viewpoint_request_queue: str = os.getenv("JOB_QUEUE", "TSJobQueue")
     efs_mount_name: str = os.getenv("EFS_MOUNT_NAME", "ts-efs-volume")
     sts_arn: str = os.getenv("STS_ARN", None)
     tile_server_log_level = logging.INFO
 
+    OVERVIEW_FILE_EXTENSION = ".ovr"
+    AUXXML_FILE_EXTENSION = ".aux.xml"
+    METADATA_FILE_EXTENSION = ".metadata"
+    BOUNDS_FILE_EXTENSION = ".bounds"
+    INFO_FILE_EXTENSION = ".geojson"
+    STATISTICS_FILE_EXTENSION = ".stats"
+
 
 @dataclass
 class BotoConfig:
     """
     BotoConfig is a dataclass meant to vend our application the set of boto client configurations required for OSML
 
     The data schema is defined as follows:
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/lambda/cleanup_dlq.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/lambda/cleanup_dlq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import json
 import logging
 import os
 import traceback
 from datetime import datetime, timedelta
 from typing import Any, Dict
 
@@ -15,31 +17,25 @@
     """
     This Lambda function processes SQS queue messages, retrieving and updating the associated items from a DynamoDB
     table. It expects an event object with a "Records" list which includes a 'viewpoint_id'. If viewpoint_id is missing
     or item is not found in the table, it returns a 404 response. If the item is found, its status is updated as
     'FAILED' with an expiry time of current time plus 1 day. If an exception occurs, it's logged and a 500-status code
     is returned with the error message.
 
-    Example usage:
-        event = {
-            "Records": [
-                {
-                    "body": "{\"viewpoint_id\": \"123\"}"
-                }
-            ]
-        }
-        context = {}
-        result = lambda_handler(event, context)
+        Example usage:
+            event = {"Records": [{"body": "{\"viewpoint_id\": \"123\"}"}]}
+            context = {}
+            result = lambda_handler(event, context)
 
-        print(result)
+            print(result)
 
     :param event: The event object that triggered the Lambda function. It contains information about the event source
-        and any data associated with the event.
+                    and any data associated with the event.
     :param context: The runtime information of the Lambda function. It provides methods and properties that allow you to
-        interact with the runtime environment.
+                    interact with the runtime environment.
     :return: A dictionary containing the response status code and body.
     """
 
     # Initialize ddb service
     ts_status_table = os.getenv("JOB_TABLE", "TSJobTable")
     ddb = boto3.resource("dynamodb")
     ddb_table = ddb.Table(ts_status_table)
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/main.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,96 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import sys
 from contextlib import AbstractAsyncContextManager, asynccontextmanager
 from time import sleep
-from typing import Tuple
 
 import uvicorn
+from asgi_correlation_id import CorrelationIdFilter, CorrelationIdMiddleware
 from botocore.exceptions import ClientError
 from cryptography.fernet import Fernet
 from fastapi import FastAPI, status
+from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import HTMLResponse
 from fastapi_versioning import VersionedFastAPI
 from osgeo import gdal
+from pythonjsonlogger.jsonlogger import JsonFormatter
 
 from .app_config import ServerConfig
-from .utils import HealthCheck, initialize_aws_services, initialize_token_key, read_token_key
-from .viewpoint.database import ViewpointStatusTable
-from .viewpoint.queue import ViewpointRequestQueue
+from .utils import (
+    HealthCheck,
+    ThreadingLocalContextFilter,
+    configure_logger,
+    initialize_aws_services,
+    initialize_token_key,
+    read_token_key,
+)
 from .viewpoint.routers import ViewpointRouter
 from .viewpoint.worker import ViewpointWorker
 
 # Configure GDAL to throw Python exceptions on errors
 gdal.UseExceptions()
 
 uvicorn_log_level_lookup = {
     logging.CRITICAL: "critical",
     logging.ERROR: "error",
     logging.WARNING: "warning",
     logging.INFO: "info",
     logging.DEBUG: "debug",
 }
 
-# Configure logger
-logger = logging.getLogger("uvicorn")
-logger.setLevel(ServerConfig.tile_server_log_level)
 
 try:
     aws_ddb, aws_s3, aws_sqs = initialize_aws_services()
 except ClientError as err:
-    logger.error(f"Fatal error occurred while initializing AWS services. Exception: {err}")
-    sys.exit("Fatal error occurred while initializing AWS services. Exiting.")
+    sys.exit(f"Fatal error occurred while initializing AWS services. Exiting. {err}")
+
 
+def configure_tile_server_logging() -> logging.Logger:
+    """
+    This function sets up the logging for the Tile Server.
 
-def initialize_viewpoint_components() -> Tuple[ViewpointStatusTable, ViewpointRequestQueue, ViewpointRouter]:
+    :return: a Logger instance for the async worker to use.
     """
-    Initialize viewpoint-related components.
+    default_formatter = JsonFormatter(fmt="%(asctime)s %(levelname)s %(message)s", datefmt="%Y-%m-%dT%H:%M:%S")
+    correlation_formatter = JsonFormatter(
+        fmt="%(asctime)s %(levelname)s %(correlation_id)s %(message)s",
+        datefmt="%Y-%m-%dT%H:%M:%S",
+    )
+    worker_filter = ThreadingLocalContextFilter(["correlation_id"])
+    access_filter = CorrelationIdFilter(default_value="-")
+    log_level = ServerConfig.tile_server_log_level
+    uvicorn_logger = logging.getLogger("uvicorn")
+    configure_logger(uvicorn_logger, log_level, log_formatter=default_formatter)
+    worker_logger = uvicorn_logger.getChild("worker")
+    configure_logger(worker_logger, log_level, log_formatter=correlation_formatter, log_filter=worker_filter)
+    uvicorn_error_logger = logging.getLogger("uvicorn.error")
+    configure_logger(uvicorn_error_logger, log_level, log_formatter=default_formatter)
+    uvicorn_access_logger = logging.getLogger("uvicorn.access")
+    configure_logger(uvicorn_access_logger, log_level, log_formatter=correlation_formatter, log_filter=access_filter)
 
-    This function creates instances of the ViewpointStatusTable,
-    ViewpointRequestQueue, and ViewpointRouter using initialized AWS services.
+    return worker_logger
 
-    :return: Tuple containing initialized viewpoint components.
 
-    :raises: ClientError if the database client failed to initialize
+def initialize_viewpoint_router() -> ViewpointRouter:
+    """
+    This function creates an instance of a ViewpointRouter using initialized AWS services.
+    Application will exit if the router fails to create.
+
+    :return: An instance of a ViewpointRouter.
     """
     initialize_token_key()
     sleep(1)
 
+    encryptor = Fernet(read_token_key())
     try:
-        database = ViewpointStatusTable(aws_ddb)
+        return ViewpointRouter(aws_ddb, aws_sqs, aws_s3, encryptor)
     except Exception as err:
-        logger.error(f"Fatal error occurred while initializing AWS services. Check your credentials! Exception: {err}")
-        sys.exit("Fatal error occurred while initializing AWS services. Exiting.")
-
-    request_queue = ViewpointRequestQueue(aws_sqs, ServerConfig.viewpoint_request_queue)
-    encryptor = Fernet(read_token_key())
-    router = ViewpointRouter(database, request_queue, aws_s3, encryptor)
-    return database, request_queue, router
+        sys.exit(f"Fatal error occurred while initializing AWS services. Check your credentials! Exiting. {err}")
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI) -> AbstractAsyncContextManager[None] | FastAPI:
     """
     Start the Viewpoint Worker as part of the FastAPI lifespan.
 
@@ -83,24 +103,30 @@
 
     Note:
         aws_s3, viewpoint_database and viewpoint_request_queue should be predefined
         before this function's call.
         They represent your AWS S3 bucket instance,
         your database instance and a queue of requests respectively.
     """
-    viewpoint_worker = ViewpointWorker(viewpoint_request_queue, aws_s3, viewpoint_database, logger)
+    # startup functions before serving requests
+
+    worker_logger = configure_tile_server_logging()
+
+    # create viewpoint worker
+    viewpoint_worker = ViewpointWorker(aws_sqs, aws_s3, aws_ddb, worker_logger)
     viewpoint_worker.start()
     yield
+    # shutdown functions after done serving requests
     viewpoint_worker.join(timeout=20)
 
 
 # Initialize FastAPI app
 app = FastAPI(title="OSML Tile Server")
 
-viewpoint_database, viewpoint_request_queue, viewpoint_router = initialize_viewpoint_components()
+viewpoint_router = initialize_viewpoint_router()
 
 # Include the viewpoint router in the FastAPI app
 app.include_router(viewpoint_router.router)
 
 # Apply API versioning
 app = VersionedFastAPI(
     app,
@@ -109,22 +135,30 @@
     terms_of_service="https://example.com/terms/",
     contact={
         "name": "Amazon Web Services",
         "email": "aws-osml-admin@amazon.com",
         "url": "https://github.com/aws-solutions-library-samples/osml-tile-server/issues",
     },
     license_info={
-        "license": """© 2023 Amazon Web Services, Inc. or its affiliates. All Rights Reserved.
+        "license": """Copyright 2023-2024 Amazon Web Services, Inc. or its affiliates. All Rights Reserved.
         This AWS Content is provided subject to the terms of the AWS Customer Agreement
         available at https://aws.amazon.com/agreement or other written agreement between
         Customer and either Amazon Web Services, Inc. or Amazon Web Services EMEA SARL or both.""",
         "name": "Amazon Web Services",
     },
     lifespan=lifespan,
 )
+app.add_middleware(
+    CORSMiddleware,
+    allow_origins=["*"],
+    allow_methods=["*"],
+    allow_headers=["X-Requested-With", "X-Request-ID"],
+    expose_headers=["X-Request-ID"],
+)
+app.add_middleware(CorrelationIdMiddleware)
 
 
 @app.get("/", response_class=HTMLResponse)
 async def root() -> str:
     """
     Root endpoint for the application.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/aws_services.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/aws_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import traceback
 from datetime import datetime, timezone
 from time import time
 from typing import Dict, Tuple
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/string_enums.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/string_enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from enum import Enum
 
 
 class AutoStringEnum(Enum):
     """
     A class used to represent an Enum where the value of the Enum member is the same as the name of the Enum member.
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/tile_server_utils.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/tile_server_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import threading
 import time
 from contextlib import contextmanager
 from functools import lru_cache
 from math import ceil, log
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/utils/token.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/utils/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2024 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import json
 import logging
 from base64 import b64decode, b64encode
 from os import path
 from typing import Optional
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/database.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import json
-import logging
 from decimal import Decimal
+from logging import Logger, getLogger
 from typing import Any, Dict, Tuple
 
 from boto3.dynamodb.conditions import Attr
 from boto3.resources.base import ServiceResource
 from botocore.exceptions import ClientError
 from fastapi import HTTPException
 
@@ -37,41 +39,40 @@
 
 
 class ViewpointStatusTable:
     """
     A class used to represent the ViewpointStatusTable.
     """
 
-    def __init__(self, aws_ddb: ServiceResource) -> None:
+    def __init__(self, aws_ddb: ServiceResource, logger: Logger = getLogger(__name__)) -> None:
         """
         Initialize the ViewpointStatusTable and validate the table status.
 
         :param aws_ddb: An instance of the AWS DynamoDB service resource.
+        :param logger: An optional logger to use.  If none provided it creates a new one.
         :return: None
         :raises ClientError: If the table does not exist in the specified AWS region.
         """
         self.ddb = aws_ddb
         self.table = self.ddb.Table(ServerConfig.viewpoint_status_table)
-        self.logger = logging.getLogger("uvicorn")
+        self.logger = logger
         try:
             self.table.table_status
         except ClientError:
-            self.logger.error(
-                "{} table does not exist in {}.".format(ServerConfig.viewpoint_status_table, ServerConfig.aws_region)
-            )
+            self.logger.error(f"{ServerConfig.viewpoint_status_table} table does not exist in {ServerConfig.aws_region}.")
             raise
 
     def get_viewpoints(self, limit: int = None, next_token: str = None) -> ViewpointListResponse:
         """
         Get viewpoint items from the dynamodb table, if limit nor next_token are provided, it returns all records.
 
         :param limit: Optional max number of viewpoints requested from dynamodb
         :param next_token: Optional token to begin a query from provided by the previous query response that
                 had more records available
-        :returns The list of available viewpoints in the table.
+        :return: The list of available viewpoints in the table.
         """
         query_params = {"FilterExpression": Attr("viewpoint_status").ne("DELETED")}
         if limit:
             query_params["Limit"] = limit
         if next_token:
             query_params["ExclusiveStartKey"] = {"viewpoint_id": next_token}
         try:
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/models.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from enum import auto
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
 from aws.osml.gdal import RangeAdjustmentType
@@ -36,17 +38,15 @@
     PREVIEW = auto()
     CROP = auto()
     STATISTICS = auto()
 
 
 class ViewpointStatus(str, AutoUnderscoreStringEnum):
     """
-    Provides status options for a viewpoint.
-
-    These states represent the state of processing or readiness for a viewpoint.
+    Provides status options for a viewpoint that represents the state of processing or readiness for a viewpoint.
 
     :cvar NOT_FOUND: Viewpoint isn't found.
     :cvar REQUESTED: Viewpoint requested.
     :cvar UPDATING: Viewpoint updating.
     :cvar READY: Viewpoint ready.
     :cvar DELETED: Viewpoint deleted.
     :cvar FAILED: Viewpoint failed.
@@ -58,17 +58,15 @@
     READY = auto()
     DELETED = auto()
     FAILED = auto()
 
 
 class ViewpointRequest(BaseModel):
     """
-    Represents a request to create or update a viewpoint.
-
-    All fields are required.
+    Represents a request to create or update a viewpoint. All fields are required.
 
     :param bucket_name: The name of the bucket, the Minimum length is 1.
     :param object_key: The key of the object, the Minimum length is 1.
     :param viewpoint_name: The name of the viewpoint, the Minimum length is 1.
     :param tile_size: The tile size, it Should be greater than 0.
     :param range_adjustment: The range adjustment type, the Minimum string length is 1.
     """
@@ -78,16 +76,15 @@
     object_key: str = Field(min_length=1)
     tile_size: int = Field(gt=0)
     range_adjustment: RangeAdjustmentType = Field(min_length=1)
 
 
 class ViewpointModel(BaseModel):
     """
-    Represents the model data for a viewpoint, including its ID, name, status, bucket name, object key, tile size,
-    range adjustment, local object path, and error message.
+    Represents the model data for a viewpoint.
 
     :param viewpoint_id: The ID to associate with the viewpoint.
     :param viewpoint_name: The name of the viewpoint.
     :param viewpoint_status: The status of the viewpoint.
     :param bucket_name: The name of the bucket the images are located in.
     :param object_key: The object is key to associate with the viewpoint.
     :param tile_size: The tile size to use for the viewpoint model.
@@ -116,17 +113,15 @@
 
     items: List[ViewpointModel]
     next_token: Optional[str] = None
 
 
 class ViewpointUpdate(BaseModel):
     """
-    Represents an update operation for a viewpoint.
-
-    This includes fields to update the viewpoint's ID, name, tile size, and range adjustment.
+    Represents the model for a viewpoint update operation.
 
     :param viewpoint_id: The ID of the viewpoint.
     :param viewpoint_name: The name of the viewpoint.
     :param tile_size: The tile size.
     :param range_adjustment: The type of range adjustment.
     """
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/queue.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/queue.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,45 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import json
-import logging
+from logging import Logger, getLogger
 from typing import Dict
 
 from botocore.exceptions import ClientError
 
 
 class ViewpointRequestQueue:
     """
     A class used to represent the ViewpointRequestQueue.
     """
 
-    def __init__(self, aws_sqs, queue_name: str) -> None:
+    def __init__(self, aws_sqs, queue_name: str, logger: Logger = getLogger(__name__)) -> None:
         """
         Initializes a new instance of the ViewpointRequestQueue class which sends messages via Amazon's Simple Queue
         Service (SQS)
 
         :param aws_sqs: AWS SQS client instance.
+        :param logger: An optional logger to use.  If none provided it creates a new one.
         :param queue_name: SQS Queue name to send messages to.
 
         :return: None
         """
 
         self.sqs_client = aws_sqs
         self.queue = self.sqs_client.get_queue_by_name(QueueName=queue_name)
-        self.logger = logging.getLogger("uvicorn")
+        self.logger = logger
 
-    def send_request(self, request: Dict) -> None:
+    def send_request(self, request: Dict, attributes: Dict = None) -> None:
         """
         Send the message to an associated SQS queue.
 
         :param request: A JSON request to assign the SQS message sent.
+        :param attributes: An optional set of attributes to attach to the message.
         :return: None
-        :raises ClientError: if unable to send a message.
         """
         try:
-            self.queue.send_message(MessageBody=json.dumps(request))
+            if attributes:
+                self.queue.send_message(MessageBody=json.dumps(request), MessageAttributes=attributes)
+            else:
+                self.queue.send_message(MessageBody=json.dumps(request))
         except ClientError as error:
             self.logger.error("Unable to send message visibility: {}".format(error))
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/routers.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/routers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import inspect
 import io
 import logging
 import shutil
 from datetime import UTC, datetime, timedelta
 from pathlib import Path
 from secrets import token_hex
 from typing import Any, Dict
 
 import dateutil.parser
+from asgi_correlation_id import correlation_id
 from boto3.resources.base import ServiceResource
 from cryptography.fernet import Fernet
 from fastapi import APIRouter, HTTPException, Query, Response
 from fastapi_versioning import version
 from osgeo import gdalconst
 from starlette.responses import FileResponse, StreamingResponse
 
 from aws.osml.gdal import GDALCompressionOptions, GDALImageFormats, RangeAdjustmentType
+from aws.osml.tile_server.app_config import ServerConfig
 from aws.osml.tile_server.utils import get_media_type, get_tile_factory_pool, perform_gdal_translation
 
-from .common import BOUNDS_FILE_EXTENSION, INFO_FILE_EXTENSION, METADATA_FILE_EXTENSION, STATISTICS_FILE_EXTENSION
 from .database import ViewpointStatusTable
 from .models import (
     ViewpointApiNames,
     ViewpointListResponse,
     ViewpointModel,
     ViewpointRequest,
     ViewpointStatus,
@@ -36,35 +37,36 @@
 class ViewpointRouter:
     """
     A class used to represent the ViewpointRouter.
     """
 
     def __init__(
         self,
-        viewpoint_database: ViewpointStatusTable,
-        viewpoint_queue: ViewpointRequestQueue,
+        aws_ddb: ServiceResource,
+        aws_sqs: ServiceResource,
         aws_s3: ServiceResource,
         encryptor: Fernet,
     ) -> None:
         """
         The `ViewpointRouter` class is responsible for handling API endpoints related to viewpoints.
 
-        :param viewpoint_database: Instance of the ViewpointStatusTable class representing the viewpoint database.
+        :param aws_ddb: Instance of the ServiceResource class representing the AWS DDB service.
 
-        :param viewpoint_queue: Instance of the ViewpointRequestQueue class representing the viewpoint request queue.
+        :param aws_sqs: Instance of the ServiceResource class representing the AWS SQS service.
 
         :param aws_s3: Instance of the ServiceResource class representing the AWS S3 service.
 
         :return: None
         """
-        self.viewpoint_database = viewpoint_database
-        self.viewpoint_queue = viewpoint_queue
+        logger = logging.getLogger("uvicorn.access")
+        self.viewpoint_database = ViewpointStatusTable(aws_ddb, logger)
+        self.viewpoint_queue = ViewpointRequestQueue(aws_sqs, ServerConfig.viewpoint_request_queue, logger)
         self.s3 = aws_s3
         self.encryptor = encryptor
-        self.logger = logging.getLogger("uvicorn")
+        self.logger = logger
 
     @property
     def router(self):
         """
         Initializes a new instance of the ViewpointRouter class.
 
         :return: None
@@ -141,20 +143,21 @@
                 tile_size=viewpoint_request.tile_size,
                 range_adjustment=viewpoint_request.range_adjustment,
                 viewpoint_status=ViewpointStatus.REQUESTED,
                 local_object_path=None,
                 error_message=None,
                 expire_time=None,
             )
+            db_response = self.viewpoint_database.create_viewpoint(new_viewpoint_request)
 
-            # Place this request into SQS, then the worker will pick up in order to
-            # download the image from S3 to Local (TODO rename to EFS once implemented)
-            self.viewpoint_queue.send_request(new_viewpoint_request.model_dump())
+            attributes = {"correlation_id": {"StringValue": correlation_id.get(), "DataType": "String"}}
+            # Place this request into SQS, then the worker will pick up in order to download the image from S3
+            self.viewpoint_queue.send_request(new_viewpoint_request.model_dump(), attributes)
 
-            return self.viewpoint_database.create_viewpoint(new_viewpoint_request)
+            return db_response
 
         @api_router.delete("/{viewpoint_id}")
         def delete_viewpoint(viewpoint_id: str) -> ViewpointModel:
             """
             Remove the file from the EFS and update the database to indicate that it has been deleted.
 
             :param viewpoint_id: Unique viewpoint id to get from the table.
@@ -216,60 +219,68 @@
 
             :return: Viewpoint metadata associated with the viewpoint item from the table.
             """
             viewpoint_item = self.viewpoint_database.get_viewpoint(viewpoint_id)
 
             self._validate_viewpoint_status(viewpoint_item.viewpoint_status, ViewpointApiNames.METADATA)
 
-            return FileResponse(viewpoint_item.local_object_path + METADATA_FILE_EXTENSION, media_type="application/json")
+            return FileResponse(
+                viewpoint_item.local_object_path + ServerConfig.METADATA_FILE_EXTENSION, media_type="application/json"
+            )
 
         @api_router.get("/{viewpoint_id}/bounds")
         def get_bounds(viewpoint_id: str) -> FileResponse:
             """
             Get viewpoint bounds based on provided viewpoint id.
 
             :param viewpoint_id: Unique viewpoint id to get from the table.
 
             :return: Viewpoint bounds for the given table item.
             """
             viewpoint_item = self.viewpoint_database.get_viewpoint(viewpoint_id)
 
             self._validate_viewpoint_status(viewpoint_item.viewpoint_status, ViewpointApiNames.BOUNDS)
 
-            return FileResponse(viewpoint_item.local_object_path + BOUNDS_FILE_EXTENSION, media_type="application/json")
+            return FileResponse(
+                viewpoint_item.local_object_path + ServerConfig.BOUNDS_FILE_EXTENSION, media_type="application/json"
+            )
 
         @api_router.get("/{viewpoint_id}/info")
         def get_info(viewpoint_id: str) -> FileResponse:
             """
             Get viewpoint info based on provided viewpoint id.
 
             :param viewpoint_id: Unique viewpoint id to get from the table.
 
             :return: Viewpoint info associated with the given id.
             """
             viewpoint_item = self.viewpoint_database.get_viewpoint(viewpoint_id)
 
             self._validate_viewpoint_status(viewpoint_item.viewpoint_status, ViewpointApiNames.INFO)
 
-            return FileResponse(viewpoint_item.local_object_path + INFO_FILE_EXTENSION, media_type="application/json")
+            return FileResponse(
+                viewpoint_item.local_object_path + ServerConfig.INFO_FILE_EXTENSION, media_type="application/json"
+            )
 
         @api_router.get("/{viewpoint_id}/statistics")
         def get_statistics(viewpoint_id: str) -> FileResponse:
             """
             Get viewpoint statistics based on provided viewpoint id.
 
             :param viewpoint_id: Unique viewpoint id to get from the table.
 
             :return: Viewpoint statistics associated with the id.
             """
             viewpoint_item = self.viewpoint_database.get_viewpoint(viewpoint_id)
 
             self._validate_viewpoint_status(viewpoint_item.viewpoint_status, ViewpointApiNames.STATISTICS)
 
-            return FileResponse(viewpoint_item.local_object_path + STATISTICS_FILE_EXTENSION, media_type="application/json")
+            return FileResponse(
+                viewpoint_item.local_object_path + ServerConfig.STATISTICS_FILE_EXTENSION, media_type="application/json"
+            )
 
         @api_router.get("/{viewpoint_id}/preview.{img_format}")
         def get_preview(
             viewpoint_id: str,
             img_format: GDALImageFormats = Path(GDALImageFormats.PNG, description="Output image type."),
             max_size: int = 1024,
             width: int = 0,
@@ -423,15 +434,14 @@
 
             :param width: Optional width in px of the desired crop, if provided, max_x will be ignored.
 
             :param height: Optional height in px of the desired crop, if provided, max_y will be ignored.
 
             :return: StreamingResponse of cropped image binary with the appropriate mime type based on the img_format
             """
-
             viewpoint_item = self.viewpoint_database.get_viewpoint(viewpoint_id)
             self._validate_viewpoint_status(viewpoint_item.viewpoint_status, ViewpointApiNames.PREVIEW)
 
             tile_factory_pool = get_tile_factory_pool(
                 img_format,
                 compression,
                 viewpoint_item.local_object_path,
```

### Comparing `osml-tile-server-0.1.1/src/aws/osml/tile_server/viewpoint/worker.py` & `osml-tile-server-0.2.0/src/aws/osml/tile_server/viewpoint/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import json
 import logging
 import time
 import traceback
 from datetime import UTC, datetime, timedelta
 from enum import auto
 from logging import Logger
@@ -14,24 +16,22 @@
 from boto3.resources.base import ServiceResource
 from botocore.exceptions import ClientError
 from osgeo import gdal, gdalconst
 
 from aws.osml.gdal import GDALCompressionOptions, GDALImageFormats, RangeAdjustmentType
 from aws.osml.photogrammetry import ImageCoordinate
 from aws.osml.tile_server.app_config import ServerConfig
-from aws.osml.tile_server.utils import AutoLowerStringEnum, TileFactoryPool, get_standard_overviews, get_tile_factory_pool
-
-from .common import (
-    AUXXML_FILE_EXTENSION,
-    BOUNDS_FILE_EXTENSION,
-    INFO_FILE_EXTENSION,
-    METADATA_FILE_EXTENSION,
-    OVERVIEW_FILE_EXTENSION,
-    STATISTICS_FILE_EXTENSION,
+from aws.osml.tile_server.utils import (
+    AutoLowerStringEnum,
+    ThreadingLocalContextFilter,
+    TileFactoryPool,
+    get_standard_overviews,
+    get_tile_factory_pool,
 )
+
 from .database import DecimalEncoder, ViewpointStatusTable
 from .models import ViewpointModel, ViewpointStatus
 from .queue import ViewpointRequestQueue
 
 
 class SupplementaryFileType(str, AutoLowerStringEnum):
     """
@@ -44,34 +44,34 @@
     AUX = auto()
     OVERVIEW = auto()
 
 
 class ViewpointWorker(Thread):
     def __init__(
         self,
-        viewpoint_request_queue: ViewpointRequestQueue,
+        aws_sqs: ServiceResource,
         aws_s3: ServiceResource,
-        viewpoint_database: ViewpointStatusTable,
+        aws_ddb: ServiceResource,
         logger: Logger = logging.getLogger(__name__),
-    ):
+    ) -> None:
         """
         The `__init__` method of the `ViewpointWorker` class initializes a new instance of the `ViewpointWorker`.
 
-        :param viewpoint_request_queue: `ViewpointRequestQueue` class representing the queue for viewpoint requests.
-        :param aws_s3: An instance of the `ServiceResource` class representing the AWS S3 service.
-        :param viewpoint_database: `ViewpointStatusTable` class representing the database for viewpoint status.
-        :param logger: 'Logger' class representing the logger.  Defaults to the default python logger.
+        :param aws_sqs: An instance of the ServiceResource class representing the AWS SQS service.
+        :param aws_s3: An instance of the ServiceResource class representing the AWS S3 service.
+        :param aws_ddb: An instance of the ServiceResource class representing the AWS DDB service.
+        :param logger: Logger class representing the logger.  Defaults to the default python logger.
 
         :return: None
         """
         super().__init__()
         self.daemon = True
-        self.viewpoint_request_queue = viewpoint_request_queue
+        self.viewpoint_request_queue = ViewpointRequestQueue(aws_sqs, ServerConfig.viewpoint_request_queue, logger)
         self.s3 = aws_s3
-        self.viewpoint_database = viewpoint_database
+        self.viewpoint_database = ViewpointStatusTable(aws_ddb, logger)
         self.logger = logger
         self.stop_event = Event()
 
     def join(self, timeout: float | None = ...) -> None:
         """
         Join the ViewpointWorker threads together.
 
@@ -92,16 +92,24 @@
 
         :return: None
         """
         self.logger.info("ViewpointWorker Background Thread Started.")
         while not self.stop_event.is_set():
             self.logger.debug("Scanning for SQS messages")
             try:
-                messages = self.viewpoint_request_queue.queue.receive_messages(WaitTimeSeconds=5)
+                attributes = ["correlation_id"]
+                messages = self.viewpoint_request_queue.queue.receive_messages(
+                    MessageAttributeNames=attributes, WaitTimeSeconds=5
+                )
                 for message in messages:
+                    correlation_id = message.message_attributes.get("correlation_id", {}).get("StringValue")
+                    if correlation_id:
+                        ThreadingLocalContextFilter.set_context({"correlation_id": correlation_id})
+                    else:
+                        ThreadingLocalContextFilter.set_context()
                     self._process_message(message)
 
             except ClientError as err:
                 self.logger.error(f"[Worker Background Thread] {err} / {traceback.format_exc()}")
             except KeyError as err:
                 self.logger.error(f"[Worker Background Thread] {err} / {traceback.format_exc()}")
             except Exception as err:
@@ -125,27 +133,27 @@
         if isinstance(failed, ViewpointStatus):
             viewpoint_item.viewpoint_status = failed
             viewpoint_item.error_message = error_message
         else:
             self._download_supplementary_file(viewpoint_item, SupplementaryFileType.OVERVIEW)
             self._download_supplementary_file(viewpoint_item, SupplementaryFileType.AUX)
 
-    def create_tile_pyramid(self, viewpoint_item: ViewpointModel):
+    def create_tile_pyramid(self, viewpoint_item: ViewpointModel) -> None:
         """
         Main tile pyramid creation function. It creates a tile pyramid for a specific viewpoint item
         by considering its range adjustment and local object path.
 
         :param: The viewpoint item object for which to create the tile pyramid.
         :return: None
         """
         try:
             tile_factory_pool = self.get_default_tile_factory_pool_for_viewpoint(viewpoint_item)
 
-            aux_file_path = Path(viewpoint_item.local_object_path + AUXXML_FILE_EXTENSION)
-            overview_file_path = Path(viewpoint_item.local_object_path + OVERVIEW_FILE_EXTENSION)
+            aux_file_path = Path(viewpoint_item.local_object_path + ServerConfig.AUXXML_FILE_EXTENSION)
+            overview_file_path = Path(viewpoint_item.local_object_path + ServerConfig.OVERVIEW_FILE_EXTENSION)
 
             if not self.stop_event.is_set() and not aux_file_path.is_file():
                 self._calculate_image_statistics(viewpoint_item)
 
             start_time = time.perf_counter()
             with tile_factory_pool.checkout_in_context() as tile_factory:
                 end_time = time.perf_counter()
@@ -319,16 +327,16 @@
         :return: None.
         """
         message_viewpoint_id = viewpoint_item.viewpoint_id
         message_object_key = viewpoint_item.object_key
         message_bucket_name = viewpoint_item.bucket_name
         local_object_path = viewpoint_item.local_object_path
         extension_lookup = {
-            SupplementaryFileType.AUX: AUXXML_FILE_EXTENSION,
-            SupplementaryFileType.OVERVIEW: OVERVIEW_FILE_EXTENSION,
+            SupplementaryFileType.AUX: ServerConfig.AUXXML_FILE_EXTENSION,
+            SupplementaryFileType.OVERVIEW: ServerConfig.OVERVIEW_FILE_EXTENSION,
         }
         try:
             self.logger.info(f"Attempting to download optional {file_type.value} file for {message_viewpoint_id}")
             self.s3.meta.client.download_file(
                 message_bucket_name,
                 message_object_key + extension_lookup[file_type],
                 local_object_path + extension_lookup[file_type],
@@ -358,22 +366,27 @@
             compression,
             viewpoint_item.local_object_path,
             output_type,
             viewpoint_item.range_adjustment,
         )
         return tile_factory_pool
 
-    def _calculate_image_statistics(self, viewpoint_item: ViewpointModel):
-        """NOTE: This code forces GDAL to and compute the statistics / histograms for each band. This can be a
+    def _calculate_image_statistics(self, viewpoint_item: ViewpointModel) -> None:
+        """This code forces GDAL to and compute the statistics / histograms for each band. This can be a
         time-consuming operation, so we want to only do this once. GDAL will write those statistics into a
         .aux.xml file associated with the dataset, but it only appears to do so when the dataset object is
         cleaned up. So this code creates a temporary dataset, forces it to generate the statistics using the
         gdal.Info() command and then closes the dataset to ensure that the auxiliary file is created. This is
         somewhat of a hack but all future calls to gdal.Open (i.e. in the tile factory pool) should be able to
-        read the .aux.xml file and skip the expensive work of generating the statistics."""
+        read the .aux.xml file and skip the expensive work of generating the statistics.
+
+        :param viewpoint_item: the description of the viewpoint item
+        :return: a default tile factory pool
+        """
+
         self.logger.info(f"Calculating Image Statistics for {viewpoint_item.local_object_path}")
         start_time = time.perf_counter()
         temp_ds = gdal.Open(viewpoint_item.local_object_path)
         gdal.Info(temp_ds, stats=True, approxStats=True, computeMinMax=True, reportHistograms=True)
         del temp_ds
         end_time = time.perf_counter()
         self.logger.info(f"METRIC: GDAL Info Time: {end_time - start_time} for {viewpoint_item.local_object_path}")
@@ -395,23 +408,23 @@
         end_time = time.perf_counter()
         self.logger.info(f"METRIC: Sample TileCreate Time: {end_time - start_time} for {viewpoint_item.local_object_path}")
         return image_bytes
 
     @staticmethod
     def _write_metadata(tile_factory: TileFactoryPool, viewpoint_item: ViewpointModel) -> None:
         metadata = tile_factory.raster_dataset.GetMetadata()
-        with open(viewpoint_item.local_object_path + METADATA_FILE_EXTENSION, "w") as md_file:
+        with open(viewpoint_item.local_object_path + ServerConfig.METADATA_FILE_EXTENSION, "w") as md_file:
             md_file.write(json.dumps({"metadata": metadata}))
 
     @staticmethod
     def _write_bounds(tile_factory: TileFactoryPool, viewpoint_item: ViewpointModel) -> None:
         width = tile_factory.raster_dataset.RasterXSize
         height = tile_factory.raster_dataset.RasterYSize
         image_coordinates = [0, 0, width, height]
-        with open(viewpoint_item.local_object_path + BOUNDS_FILE_EXTENSION, "w") as bounds_file:
+        with open(viewpoint_item.local_object_path + ServerConfig.BOUNDS_FILE_EXTENSION, "w") as bounds_file:
             bounds_file.write(json.dumps({"bounds": image_coordinates}))
 
     @staticmethod
     def _write_info(tile_factory: TileFactoryPool, viewpoint_item: ViewpointModel) -> None:
         width = tile_factory.raster_dataset.RasterXSize
         height = tile_factory.raster_dataset.RasterYSize
         coordinates = []
@@ -420,16 +433,16 @@
             coordinates.append((degrees(world_coordinate.longitude), degrees(world_coordinate.latitude)))
         coordinates.append(coordinates[0])
 
         feature = geojson.Feature(
             id=viewpoint_item.viewpoint_name, geometry=geojson.geometry.Polygon([coordinates]), properties={}
         )
         feature_collection = geojson.FeatureCollection(features=[feature])
-        with open(viewpoint_item.local_object_path + INFO_FILE_EXTENSION, "w") as info_file:
+        with open(viewpoint_item.local_object_path + ServerConfig.INFO_FILE_EXTENSION, "w") as info_file:
             info_file.write(geojson.dumps(feature_collection))
 
     @staticmethod
     def _write_statistics(viewpoint_item: ViewpointModel) -> None:
         gdal_options = gdal.InfoOptions(format="json", showMetadata=False)
         gdal_info = gdal.Info(viewpoint_item.local_object_path, options=gdal_options)
-        with open(viewpoint_item.local_object_path + STATISTICS_FILE_EXTENSION, "w") as stats_file:
+        with open(viewpoint_item.local_object_path + ServerConfig.STATISTICS_FILE_EXTENSION, "w") as stats_file:
             stats_file.write(json.dumps({"image_statistics": gdal_info}))
```

### Comparing `osml-tile-server-0.1.1/src/osml_tile_server.egg-info/PKG-INFO` & `osml-tile-server-0.2.0/src/osml_tile_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-tile-server
-Version: 0.1.1
+Version: 0.2.0
 Summary: The OversightML Tile Server is a lightweight, cloud-based tile server which allows you to quickly pass an image from S3 bucket to get metadata, image statistics, and set of tiles in real-time.
 Author: Amazon Web Services
 Author-email: aws-osml-admin@amazon.com
 License: 
         © 2023 Amazon Web Services, Inc. or its affiliates. All Rights Reserved.
         This AWS Content is provided subject to the terms of the AWS Customer Agreement
         available at http://aws.amazon.com/agreement or other written agreement between
@@ -15,18 +15,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: uvicorn
 Requires-Dist: fastapi
 Requires-Dist: fastapi-versioning
+Requires-Dist: asgi-correlation-id
 Requires-Dist: starlette[full]
 Requires-Dist: cryptography
 Requires-Dist: boto3
 Requires-Dist: geojson>=3.0.0
+Requires-Dist: pydantic>=2.0.0
+Requires-Dist: python-json-logger>=2.0.0
 Requires-Dist: osml-imagery-toolkit>=1.2
 Provides-Extra: test
 Requires-Dist: tox; extra == "test"
 
 # OversightML Tile Server
 
 The OversightML Tile Server (TS) is a lightweight, cloud-based tile server which allows you to quickly pass an image from S3 bucket to get metadata, image statistics, and set of tiles in real-time.
```

### Comparing `osml-tile-server-0.1.1/src/osml_tile_server.egg-info/SOURCES.txt` & `osml-tile-server-0.2.0/src/osml_tile_server.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/aws/osml/tile_server/__init__.py
 src/aws/osml/tile_server/app_config.py
 src/aws/osml/tile_server/main.py
+src/aws/osml/tile_server/lambda/__init__.py
 src/aws/osml/tile_server/lambda/cleanup_dlq.py
 src/aws/osml/tile_server/utils/__init__.py
 src/aws/osml/tile_server/utils/aws_services.py
 src/aws/osml/tile_server/utils/health_check.py
+src/aws/osml/tile_server/utils/log_tools.py
 src/aws/osml/tile_server/utils/string_enums.py
 src/aws/osml/tile_server/utils/tile_server_utils.py
 src/aws/osml/tile_server/utils/token.py
 src/aws/osml/tile_server/viewpoint/__init__.py
-src/aws/osml/tile_server/viewpoint/common.py
 src/aws/osml/tile_server/viewpoint/database.py
 src/aws/osml/tile_server/viewpoint/models.py
 src/aws/osml/tile_server/viewpoint/queue.py
 src/aws/osml/tile_server/viewpoint/routers.py
 src/aws/osml/tile_server/viewpoint/worker.py
 src/osml_tile_server.egg-info/PKG-INFO
 src/osml_tile_server.egg-info/SOURCES.txt
```

