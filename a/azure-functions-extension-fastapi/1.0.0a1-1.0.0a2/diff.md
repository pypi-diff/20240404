# Comparing `tmp/azure-functions-extension-fastapi-1.0.0a1.tar.gz` & `tmp/azure-functions-extension-fastapi-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-functions-extension-fastapi-1.0.0a1.tar", last modified: Tue Mar 19 19:11:34 2024, max compression
+gzip compressed data, was "azure-functions-extension-fastapi-1.0.0a2.tar", last modified: Thu Apr  4 15:47:38 2024, max compression
```

## Comparing `azure-functions-extension-fastapi-1.0.0a1.tar` & `azure-functions-extension-fastapi-1.0.0a2.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0 biwang    (1000) biwang    (1000)        0 2024-03-19 19:11:34.132393 azure-functions-extension-fastapi-1.0.0a1/
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)     1093 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a1/LICENSE
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)       91 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a1/MANIFEST.in
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)      792 2024-03-19 19:11:34.129345 azure-functions-extension-fastapi-1.0.0a1/PKG-INFO
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)        0 2024-03-15 20:14:34.000000 azure-functions-extension-fastapi-1.0.0a1/README.md
-drwxrwxrwx   0 biwang    (1000) biwang    (1000)        0 2024-03-19 19:11:33.890440 azure-functions-extension-fastapi-1.0.0a1/azure/
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)       66 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a1/azure/__init__.py
-drwxrwxrwx   0 biwang    (1000) biwang    (1000)        0 2024-03-19 19:11:33.908254 azure-functions-extension-fastapi-1.0.0a1/azure/functions/
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)       66 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a1/azure/functions/__init__.py
-drwxrwxrwx   0 biwang    (1000) biwang    (1000)        0 2024-03-19 19:11:33.930692 azure-functions-extension-fastapi-1.0.0a1/azure/functions/extension/
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)       66 2024-03-13 22:55:06.000000 azure-functions-extension-fastapi-1.0.0a1/azure/functions/extension/__init__.py
-drwxrwxrwx   0 biwang    (1000) biwang    (1000)        0 2024-03-19 19:11:33.982927 azure-functions-extension-fastapi-1.0.0a1/azure/functions/extension/fastapi/
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)      509 2024-03-15 22:02:09.000000 azure-functions-extension-fastapi-1.0.0a1/azure/functions/extension/fastapi/__init__.py
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)     2736 2024-03-14 20:14:45.000000 azure-functions-extension-fastapi-1.0.0a1/azure/functions/extension/fastapi/web.py
-drwxrwxrwx   0 biwang    (1000) biwang    (1000)        0 2024-03-19 19:11:34.074016 azure-functions-extension-fastapi-1.0.0a1/azure_functions_extension_fastapi.egg-info/
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)      792 2024-03-19 19:11:33.000000 azure-functions-extension-fastapi-1.0.0a1/azure_functions_extension_fastapi.egg-info/PKG-INFO
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)      556 2024-03-19 19:11:33.000000 azure-functions-extension-fastapi-1.0.0a1/azure_functions_extension_fastapi.egg-info/SOURCES.txt
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)        1 2024-03-19 19:11:33.000000 azure-functions-extension-fastapi-1.0.0a1/azure_functions_extension_fastapi.egg-info/dependency_links.txt
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)      170 2024-03-19 19:11:33.000000 azure-functions-extension-fastapi-1.0.0a1/azure_functions_extension_fastapi.egg-info/requires.txt
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)        6 2024-03-19 19:11:33.000000 azure-functions-extension-fastapi-1.0.0a1/azure_functions_extension_fastapi.egg-info/top_level.txt
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)       38 2024-03-19 19:11:34.133392 azure-functions-extension-fastapi-1.0.0a1/setup.cfg
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)     1564 2024-03-19 19:09:39.000000 azure-functions-extension-fastapi-1.0.0a1/setup.py
-drwxrwxrwx   0 biwang    (1000) biwang    (1000)        0 2024-03-19 19:11:34.114861 azure-functions-extension-fastapi-1.0.0a1/tests/
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)      529 2024-03-13 23:05:56.000000 azure-functions-extension-fastapi-1.0.0a1/tests/__init__.py
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)     1065 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a1/tests/test_code_quality.py
--rwxrwxrwx   0 biwang    (1000) biwang    (1000)     4035 2024-03-15 22:02:09.000000 azure-functions-extension-fastapi-1.0.0a1/tests/test_web.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.149836 azure-functions-extension-fastapi-1.0.0a2/
+-rw-rw-rw-   0        0        0     1093 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a2/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6390 2024-04-04 15:47:38.146845 azure-functions-extension-fastapi-1.0.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0     5069 2024-03-27 17:03:54.000000 azure-functions-extension-fastapi-1.0.0a2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.093920 azure-functions-extension-fastapi-1.0.0a2/azure/
+-rw-rw-rw-   0        0        0       66 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a2/azure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.096425 azure-functions-extension-fastapi-1.0.0a2/azure/functions/
+-rw-rw-rw-   0        0        0       66 2024-03-13 21:50:44.000000 azure-functions-extension-fastapi-1.0.0a2/azure/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.098434 azure-functions-extension-fastapi-1.0.0a2/azure/functions/extension/
+-rw-rw-rw-   0        0        0       66 2024-03-13 22:55:06.000000 azure-functions-extension-fastapi-1.0.0a2/azure/functions/extension/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.105088 azure-functions-extension-fastapi-1.0.0a2/azure/functions/extension/fastapi/
+-rw-rw-rw-   0        0        0      627 2024-04-04 15:45:01.000000 azure-functions-extension-fastapi-1.0.0a2/azure/functions/extension/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     4505 2024-04-04 15:39:09.000000 azure-functions-extension-fastapi-1.0.0a2/azure/functions/extension/fastapi/web.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.142836 azure-functions-extension-fastapi-1.0.0a2/azure_functions_extension_fastapi.egg-info/
+-rw-rw-rw-   0        0        0     6390 2024-04-04 15:47:38.000000 azure-functions-extension-fastapi-1.0.0a2/azure_functions_extension_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      651 2024-04-04 15:47:38.000000 azure-functions-extension-fastapi-1.0.0a2/azure_functions_extension_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:47:38.000000 azure-functions-extension-fastapi-1.0.0a2/azure_functions_extension_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2024-04-04 15:47:38.000000 azure-functions-extension-fastapi-1.0.0a2/azure_functions_extension_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-04 15:47:38.000000 azure-functions-extension-fastapi-1.0.0a2/azure_functions_extension_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1575 2024-04-04 15:39:09.000000 azure-functions-extension-fastapi-1.0.0a2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.076861 azure-functions-extension-fastapi-1.0.0a2/samples/
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.127694 azure-functions-extension-fastapi-1.0.0a2/samples/fastapi_samples_streaming_download/
+-rw-rw-rw-   0        0        0     1012 2024-03-27 17:14:27.000000 azure-functions-extension-fastapi-1.0.0a2/samples/fastapi_samples_streaming_download/function_app.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.130692 azure-functions-extension-fastapi-1.0.0a2/samples/fastapi_samples_streaming_upload/
+-rw-rw-rw-   0        0        0     1026 2024-03-27 17:14:27.000000 azure-functions-extension-fastapi-1.0.0a2/samples/fastapi_samples_streaming_upload/function_app.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:47:38.151433 azure-functions-extension-fastapi-1.0.0a2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 15:47:38.138839 azure-functions-extension-fastapi-1.0.0a2/tests/
+-rw-rw-rw-   0        0        0      519 2024-03-27 17:14:26.000000 azure-functions-extension-fastapi-1.0.0a2/tests/__init__.py
+-rw-rw-rw-   0        0        0     8647 2024-04-04 15:39:09.000000 azure-functions-extension-fastapi-1.0.0a2/tests/test_web.py
```

### Comparing `azure-functions-extension-fastapi-1.0.0a1/LICENSE` & `azure-functions-extension-fastapi-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-functions-extension-fastapi-1.0.0a1/azure/functions/extension/fastapi/web.py` & `azure-functions-extension-fastapi-1.0.0a2/azure/functions/extension/fastapi/web.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,160 @@
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License.
 
 from typing import Callable
-from fastapi import Request as FastApiRequest, Response as FastApiResponse, FastAPI
-from fastapi.responses import (
-    StreamingResponse as FastApiStreamingResponse,
-    HTMLResponse as FastApiHTMLResponse,
-    PlainTextResponse as FastApiPlainTextResponse,
-    RedirectResponse as FastApiRedirectResponse,
-    JSONResponse as FastApiJSONResponse,
-    UJSONResponse as FastApiUJSONResponse,
-    ORJSONResponse as FastApiORJSONResponse,
-    FileResponse as FastApiFileResponse,
-)
-from azure.functions.extension.base import WebServer, WebApp, RequestTrackerMeta, ResponseTrackerMeta, ResponseLabels
+
 import uvicorn
+from azure.functions.extension.base import (
+    RequestSynchronizer,
+    RequestTrackerMeta,
+    ResponseLabels,
+    ResponseTrackerMeta,
+    WebApp,
+    WebServer,
+)
+from fastapi import FastAPI
+from fastapi import Request as FastApiRequest
+from fastapi import Response as FastApiResponse
+from fastapi.responses import FileResponse as FastApiFileResponse
+from fastapi.responses import HTMLResponse as FastApiHTMLResponse
+from fastapi.responses import JSONResponse as FastApiJSONResponse
+from fastapi.responses import ORJSONResponse as FastApiORJSONResponse
+from fastapi.responses import PlainTextResponse as FastApiPlainTextResponse
+from fastapi.responses import RedirectResponse as FastApiRedirectResponse
+from fastapi.responses import StreamingResponse as FastApiStreamingResponse
+from fastapi.responses import UJSONResponse as FastApiUJSONResponse
+from pydantic import BaseModel
+
+
+class RequestSynchronizer(RequestSynchronizer):
+    def sync_route_params(self, request, path_params):
+        # add null checks for request and path_params
+        if request is None:
+            raise TypeError("Request object is None")
+        if path_params is None:
+            raise TypeError("Path parameters are None")
+
+        request.path_params.clear()
+        request.path_params.update(path_params)
+
 
 class Request(metaclass=RequestTrackerMeta):
     request_type = FastApiRequest
+    synchronizer = RequestSynchronizer()
+
 
 class Response(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.STANDARD
     response_type = FastApiResponse
 
+
 class StreamingResponse(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.STREAMING
     response_type = FastApiStreamingResponse
 
+
 class HTMLResponse(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.HTML
     response_type = FastApiHTMLResponse
 
+
 class PlainTextResponse(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.PLAIN_TEXT
     response_type = FastApiPlainTextResponse
 
+
 class RedirectResponse(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.REDIRECT
     response_type = FastApiRedirectResponse
 
+
 class JSONResponse(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.JSON
     response_type = FastApiJSONResponse
 
+
 class UJSONResponse(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.UJSON
     response_type = FastApiUJSONResponse
 
+
 class ORJSONResponse(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.ORJSON
     response_type = FastApiORJSONResponse
 
+
 class FileResponse(metaclass=ResponseTrackerMeta):
     label = ResponseLabels.FILE
     response_type = FastApiFileResponse
 
 
+class StrResponse(metaclass=ResponseTrackerMeta):
+    label = ResponseLabels.STR
+    response_type = str
+
+
+class DictResponse(metaclass=ResponseTrackerMeta):
+    label = ResponseLabels.DICT
+    response_type = dict
+
+
+class BoolResponse(metaclass=ResponseTrackerMeta):
+    label = ResponseLabels.BOOL
+    response_type = bool
+
+
+class PydanticResponse(metaclass=ResponseTrackerMeta):
+    label = ResponseLabels.PYDANTIC
+    response_type = BaseModel
+
+
+class IntResponse(metaclass=ResponseTrackerMeta):
+    label = ResponseLabels.INT
+    response_type = int
+
+
+class FloatResponse(metaclass=ResponseTrackerMeta):
+    label = ResponseLabels.FLOAT
+    response_type = float
+
+
+class ListResponse(metaclass=ResponseTrackerMeta):
+    label = ResponseLabels.LIST
+    response_type = list
+
+
 class WebApp(WebApp):
     def __init__(self):
         self.web_app = FastAPI()
 
     def route(self, func: Callable):
         # Apply the api_route decorator
         decorated_function = self.web_app.api_route(
             "/{path:path}",
-            methods=["GET", "POST", "PUT", "DELETE", "OPTIONS", "HEAD", "PATCH", "TRACE"]
+            methods=[
+                "GET",
+                "POST",
+                "PUT",
+                "DELETE",
+                "OPTIONS",
+                "HEAD",
+                "PATCH",
+                "TRACE",
+            ],
         )(func)
 
         return decorated_function
 
     def get_app(self):
         return self.web_app
-    
+
 
 class WebServer(WebServer):
     async def serve(self):
-        uvicorn_config = uvicorn.Config(self.web_app, host=self.hostname, port=self.port)
-    
+        uvicorn_config = uvicorn.Config(
+            self.web_app, host=self.hostname, port=self.port
+        )
+
         server = uvicorn.Server(uvicorn_config)
 
-        return await server.serve()
+        return await server.serve()
```

### Comparing `azure-functions-extension-fastapi-1.0.0a1/setup.py` & `azure-functions-extension-fastapi-1.0.0a2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,99 @@
-00000000: 2320 2043 6f70 7972 6967 6874 2028 6329  #  Copyright (c)
-00000010: 204d 6963 726f 736f 6674 2043 6f72 706f   Microsoft Corpo
-00000020: 7261 7469 6f6e 2e20 416c 6c20 7269 6768  ration. All righ
-00000030: 7473 2072 6573 6572 7665 642e 0d0a 2320  ts reserved...# 
-00000040: 204c 6963 656e 7365 6420 756e 6465 7220   Licensed under 
-00000050: 7468 6520 4d49 5420 4c69 6365 6e73 652e  the MIT License.
-00000060: 0d0a 0d0a 6672 6f6d 2073 6574 7570 746f  ....from setupto
-00000070: 6f6c 7320 696d 706f 7274 2073 6574 7570  ols import setup
-00000080: 2c20 6669 6e64 5f70 6163 6b61 6765 730d  , find_packages.
-00000090: 0a0d 0a23 2054 4f44 4f3a 2070 696e 2074  ...# TODO: pin t
-000000a0: 6f20 6578 7420 6261 7365 2076 6572 7369  o ext base versi
-000000b0: 6f6e 2061 6674 6572 2070 7562 6c69 7368  on after publish
-000000c0: 6564 0d0a 0d0a 4558 5452 415f 5245 5155  ed....EXTRA_REQU
-000000d0: 4952 4553 203d 207b 0d0a 2020 2020 2764  IRES = {..    'd
-000000e0: 6576 273a 205b 0d0a 2020 2020 2020 2020  ev': [..        
-000000f0: 2766 6c61 6b65 387e 3d34 2e30 2e31 272c  'flake8~=4.0.1',
-00000100: 0d0a 2020 2020 2020 2020 2766 6c61 6b65  ..        'flake
-00000110: 382d 6c6f 6767 696e 672d 666f 726d 6174  8-logging-format
-00000120: 272c 0d0a 2020 2020 2020 2020 276d 7970  ',..        'myp
-00000130: 7927 2c0d 0a20 2020 2020 2020 2027 7079  y',..        'py
-00000140: 7465 7374 272c 0d0a 2020 2020 2020 2020  test',..        
-00000150: 2770 7974 6573 742d 636f 7627 2c0d 0a20  'pytest-cov',.. 
-00000160: 2020 2020 2020 2027 7265 7175 6573 7473         'requests
-00000170: 3d3d 322e 2a27 2c0d 0a20 2020 2020 2020  ==2.*',..       
-00000180: 2027 636f 7665 7261 6765 272c 0d0a 2020   'coverage',..  
-00000190: 2020 2020 2020 2770 7974 6573 742d 696e        'pytest-in
-000001a0: 7374 6166 6169 6c27 0d0a 2020 2020 5d0d  stafail'..    ].
-000001b0: 0a7d 0d0a 0d0a 7365 7475 7028 0d0a 2020  .}....setup(..  
-000001c0: 2020 6e61 6d65 3d27 617a 7572 652d 6675    name='azure-fu
-000001d0: 6e63 7469 6f6e 732d 6578 7465 6e73 696f  nctions-extensio
-000001e0: 6e2d 6661 7374 6170 6927 2c0d 0a20 2020  n-fastapi',..   
-000001f0: 2076 6572 7369 6f6e 3d27 312e 302e 3061   version='1.0.0a
-00000200: 3127 2c0d 0a20 2020 2061 7574 686f 723d  1',..    author=
-00000210: 2741 7a75 7265 2046 756e 6374 696f 6e73  'Azure Functions
-00000220: 2074 6561 6d20 6174 204d 6963 726f 736f   team at Microso
-00000230: 6674 2043 6f72 702e 272c 0d0a 2020 2020  ft Corp.',..    
-00000240: 6175 7468 6f72 5f65 6d61 696c 3d27 617a  author_email='az
-00000250: 7572 6566 756e 6374 696f 6e73 406d 6963  urefunctions@mic
-00000260: 726f 736f 6674 2e63 6f6d 272c 0d0a 2020  rosoft.com',..  
-00000270: 2020 6465 7363 7269 7074 696f 6e3d 2746    description='F
-00000280: 6173 7441 7069 2050 7974 686f 6e20 776f  astApi Python wo
-00000290: 726b 6572 2065 7874 656e 7369 6f6e 2066  rker extension f
-000002a0: 6f72 2041 7a75 7265 2046 756e 6374 696f  or Azure Functio
-000002b0: 6e73 2e27 2c0d 0a20 2020 2070 6163 6b61  ns.',..    packa
-000002c0: 6765 733d 6669 6e64 5f70 6163 6b61 6765  ges=find_package
-000002d0: 7328 6578 636c 7564 653d 5b0d 0a20 2020  s(exclude=[..   
-000002e0: 2020 2020 2027 617a 7572 652e 6675 6e63       'azure.func
-000002f0: 7469 6f6e 732e 6578 7465 6e73 696f 6e27  tions.extension'
-00000300: 2c20 2761 7a75 7265 2e66 756e 6374 696f  , 'azure.functio
-00000310: 6e73 272c 0d0a 2020 2020 2020 2020 2761  ns',..        'a
-00000320: 7a75 7265 272c 2027 7465 7374 7327 2c20  zure', 'tests', 
-00000330: 2773 616d 706c 6573 270d 0a20 2020 205d  'samples'..    ]
-00000340: 292c 0d0a 2020 2020 636c 6173 7369 6669  ),..    classifi
-00000350: 6572 733d 5b0d 0a20 2020 2020 2020 2027  ers=[..        '
-00000360: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000370: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-00000380: 6963 656e 7365 272c 0d0a 2020 2020 2020  icense',..      
-00000390: 2020 2749 6e74 656e 6465 6420 4175 6469    'Intended Audi
-000003a0: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-000003b0: 7273 272c 0d0a 2020 2020 2020 2020 2750  rs',..        'P
-000003c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003e0: 2033 272c 0d0a 2020 2020 2020 2020 2750   3',..        'P
-000003f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000400: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000410: 2033 2e38 272c 0d0a 2020 2020 2020 2020   3.8',..        
-00000420: 2750 726f 6772 616d 6d69 6e67 204c 616e  'Programming Lan
-00000430: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000440: 3a3a 2033 2e39 272c 0d0a 2020 2020 2020  :: 3.9',..      
-00000450: 2020 274f 7065 7261 7469 6e67 2053 7973    'Operating Sys
-00000460: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
-00000470: 203a 3a20 5769 6e64 6f77 7327 2c0d 0a20   :: Windows',.. 
-00000480: 2020 2020 2020 2027 4f70 6572 6174 696e         'Operatin
-00000490: 6720 5379 7374 656d 203a 3a20 504f 5349  g System :: POSI
-000004a0: 5827 2c0d 0a20 2020 2020 2020 2027 4f70  X',..        'Op
-000004b0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000004c0: 3a20 4d61 634f 5320 3a3a 204d 6163 4f53  : MacOS :: MacOS
-000004d0: 2058 272c 0d0a 2020 2020 2020 2020 2745   X',..        'E
-000004e0: 6e76 6972 6f6e 6d65 6e74 203a 3a20 5765  nvironment :: We
-000004f0: 6220 456e 7669 726f 6e6d 656e 7427 2c0d  b Environment',.
-00000500: 0a20 2020 2020 2020 2027 4465 7665 6c6f  .        'Develo
-00000510: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-00000520: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
-00000530: 7461 626c 6527 2c0d 0a20 2020 205d 2c0d  table',..    ],.
-00000540: 0a20 2020 206c 6963 656e 7365 3d27 4d49  .    license='MI
-00000550: 5427 2c0d 0a20 2020 2070 7974 686f 6e5f  T',..    python_
-00000560: 7265 7175 6972 6573 3d27 3e3d 332e 3827  requires='>=3.8'
-00000570: 2c0d 0a20 2020 2069 6e73 7461 6c6c 5f72  ,..    install_r
-00000580: 6571 7569 7265 733d 5b0d 0a20 2020 2020  equires=[..     
-00000590: 2020 2027 617a 7572 652d 6675 6e63 7469     'azure-functi
-000005a0: 6f6e 732d 6578 7465 6e73 696f 6e2d 6261  ons-extension-ba
-000005b0: 7365 272c 0d0a 2020 2020 2020 2020 2766  se',..        'f
-000005c0: 6173 7461 7069 3d3d 302e 3131 302e 3027  astapi==0.110.0'
-000005d0: 2c0d 0a20 2020 2020 2020 2027 7576 6963  ,..        'uvic
-000005e0: 6f72 6e3d 3d30 2e32 382e 3027 0d0a 2020  orn==0.28.0'..  
-000005f0: 2020 5d2c 0d0a 2020 2020 6578 7472 6173    ],..    extras
-00000600: 5f72 6571 7569 7265 3d45 5854 5241 5f52  _require=EXTRA_R
-00000610: 4551 5549 5245 530d 0a29 0d0a            EQUIRES..)..
+00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
+00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
+00000020: 7570 746f 6f6c 7320 3e3d 2036 312e 3022  uptools >= 61.0"
+00000030: 5d0d 0a62 7569 6c64 2d62 6163 6b65 6e64  ]..build-backend
+00000040: 203d 2022 7365 7475 7074 6f6f 6c73 2e62   = "setuptools.b
+00000050: 7569 6c64 5f6d 6574 6122 0d0a 0d0a 5b70  uild_meta"....[p
+00000060: 726f 6a65 6374 5d0d 0a6e 616d 6520 3d20  roject]..name = 
+00000070: 2261 7a75 7265 2d66 756e 6374 696f 6e73  "azure-functions
+00000080: 2d65 7874 656e 7369 6f6e 2d66 6173 7461  -extension-fasta
+00000090: 7069 220d 0a64 796e 616d 6963 203d 205b  pi"..dynamic = [
+000000a0: 2276 6572 7369 6f6e 225d 0d0a 7265 7175  "version"]..requ
+000000b0: 6972 6573 2d70 7974 686f 6e20 3d20 223e  ires-python = ">
+000000c0: 3d33 2e38 220d 0a61 7574 686f 7273 203d  =3.8"..authors =
+000000d0: 205b 7b20 6e61 6d65 203d 2022 417a 7572   [{ name = "Azur
+000000e0: 6520 4675 6e63 7469 6f6e 7320 7465 616d  e Functions team
+000000f0: 2061 7420 4d69 6372 6f73 6f66 7420 436f   at Microsoft Co
+00000100: 7270 2e22 2c20 656d 6169 6c20 3d20 2261  rp.", email = "a
+00000110: 7a75 7265 6675 6e63 7469 6f6e 7340 6d69  zurefunctions@mi
+00000120: 6372 6f73 6f66 742e 636f 6d22 7d5d 0d0a  crosoft.com"}]..
+00000130: 6465 7363 7269 7074 696f 6e20 3d20 2246  description = "F
+00000140: 6173 7441 7069 2050 7974 686f 6e20 776f  astApi Python wo
+00000150: 726b 6572 2065 7874 656e 7369 6f6e 2066  rker extension f
+00000160: 6f72 2041 7a75 7265 2046 756e 6374 696f  or Azure Functio
+00000170: 6e73 2e22 0d0a 7265 6164 6d65 203d 2022  ns."..readme = "
+00000180: 5245 4144 4d45 2e6d 6422 0d0a 6c69 6365  README.md"..lice
+00000190: 6e73 6520 3d20 7b74 6578 7420 3d20 224d  nse = {text = "M
+000001a0: 4954 204c 6963 656e 7365 227d 0d0a 636c  IT License"}..cl
+000001b0: 6173 7369 6669 6572 733d 205b 0d0a 2020  assifiers= [..  
+000001c0: 2020 2020 2020 274c 6963 656e 7365 203a        'License :
+000001d0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000001e0: 3a20 4d49 5420 4c69 6365 6e73 6527 2c0d  : MIT License',.
+000001f0: 0a20 2020 2020 2020 2027 496e 7465 6e64  .        'Intend
+00000200: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+00000210: 6576 656c 6f70 6572 7327 2c0d 0a20 2020  evelopers',..   
+00000220: 2020 2020 2027 5072 6f67 7261 6d6d 696e       'Programmin
+00000230: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000240: 7468 6f6e 203a 3a20 3327 2c0d 0a20 2020  thon :: 3',..   
+00000250: 2020 2020 2027 5072 6f67 7261 6d6d 696e       'Programmin
+00000260: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000270: 7468 6f6e 203a 3a20 332e 3827 2c0d 0a20  thon :: 3.8',.. 
+00000280: 2020 2020 2020 2027 5072 6f67 7261 6d6d         'Programm
+00000290: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002a0: 5079 7468 6f6e 203a 3a20 332e 3927 2c0d  Python :: 3.9',.
+000002b0: 0a20 2020 2020 2020 2027 5072 6f67 7261  .        'Progra
+000002c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002d0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+000002e0: 272c 0d0a 2020 2020 2020 2020 2750 726f  ',..        'Pro
+000002f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000300: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000310: 2e31 3127 2c0d 0a20 2020 2020 2020 2027  .11',..        '
+00000320: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000330: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
+00000340: 2057 696e 646f 7773 272c 0d0a 2020 2020   Windows',..    
+00000350: 2020 2020 274f 7065 7261 7469 6e67 2053      'Operating S
+00000360: 7973 7465 6d20 3a3a 2050 4f53 4958 272c  ystem :: POSIX',
+00000370: 0d0a 2020 2020 2020 2020 274f 7065 7261  ..        'Opera
+00000380: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
+00000390: 6163 4f53 203a 3a20 4d61 634f 5320 5827  acOS :: MacOS X'
+000003a0: 2c0d 0a20 2020 2020 2020 2027 456e 7669  ,..        'Envi
+000003b0: 726f 6e6d 656e 7420 3a3a 2057 6562 2045  ronment :: Web E
+000003c0: 6e76 6972 6f6e 6d65 6e74 272c 0d0a 2020  nvironment',..  
+000003d0: 2020 2020 2020 2744 6576 656c 6f70 6d65        'Developme
+000003e0: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+000003f0: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+00000400: 6c65 272c 0d0a 2020 2020 5d0d 0a64 6570  le',..    ]..dep
+00000410: 656e 6465 6e63 6965 7320 3d20 5b0d 0a20  endencies = [.. 
+00000420: 2020 2020 2020 2027 617a 7572 652d 6675         'azure-fu
+00000430: 6e63 7469 6f6e 732d 6578 7465 6e73 696f  nctions-extensio
+00000440: 6e2d 6261 7365 272c 0d0a 2020 2020 2020  n-base',..      
+00000450: 2020 2766 6173 7461 7069 3d3d 302e 3131    'fastapi==0.11
+00000460: 302e 3027 2c0d 0a20 2020 2020 2020 2027  0.0',..        '
+00000470: 7576 6963 6f72 6e3d 3d30 2e32 382e 3027  uvicorn==0.28.0'
+00000480: 2c0d 0a20 2020 2020 2020 2027 7079 6461  ,..        'pyda
+00000490: 6e74 6963 3d3d 322e 362e 3427 2c0d 0a20  ntic==2.6.4',.. 
+000004a0: 2020 205d 0d0a 0d0a 5b70 726f 6a65 6374     ]....[project
+000004b0: 2e6f 7074 696f 6e61 6c2d 6465 7065 6e64  .optional-depend
+000004c0: 656e 6369 6573 5d0d 0a64 6576 203d 205b  encies]..dev = [
+000004d0: 0d0a 2020 2020 2770 7974 6573 7427 2c0d  ..    'pytest',.
+000004e0: 0a20 2020 2027 7079 7465 7374 2d63 6f76  .    'pytest-cov
+000004f0: 272c 0d0a 2020 2020 2763 6f76 6572 6167  ',..    'coverag
+00000500: 6527 2c0d 0a20 2020 2027 7079 7465 7374  e',..    'pytest
+00000510: 2d69 6e73 7461 6661 696c 272c 0d0a 2020  -instafail',..  
+00000520: 2020 2770 7265 2d63 6f6d 6d69 7427 0d0a    'pre-commit'..
+00000530: 2020 2020 5d0d 0a0d 0a5b 746f 6f6c 2e73      ]....[tool.s
+00000540: 6574 7570 746f 6f6c 732e 6479 6e61 6d69  etuptools.dynami
+00000550: 635d 0d0a 7665 7273 696f 6e20 3d20 7b61  c]..version = {a
+00000560: 7474 7220 3d20 2261 7a75 7265 2e66 756e  ttr = "azure.fun
+00000570: 6374 696f 6e73 2e65 7874 656e 7369 6f6e  ctions.extension
+00000580: 2e66 6173 7461 7069 2e5f 5f76 6572 7369  .fastapi.__versi
+00000590: 6f6e 5f5f 227d 0d0a 0d0a 5b74 6f6f 6c2e  on__"}....[tool.
+000005a0: 7365 7475 7074 6f6f 6c73 2e70 6163 6b61  setuptools.packa
+000005b0: 6765 732e 6669 6e64 5d0d 0a65 7863 6c75  ges.find]..exclu
+000005c0: 6465 203d 205b 0d0a 2020 2020 2761 7a75  de = [..    'azu
+000005d0: 7265 2e66 756e 6374 696f 6e73 2e65 7874  re.functions.ext
+000005e0: 656e 7369 6f6e 272c 2027 617a 7572 652e  ension', 'azure.
+000005f0: 6675 6e63 7469 6f6e 7327 2c0d 0a20 2020  functions',..   
+00000600: 2027 617a 7572 6527 2c20 2774 6573 7473   'azure', 'tests
+00000610: 272c 2027 7361 6d70 6c65 7327 0d0a 2020  ', 'samples'..  
+00000620: 2020 5d0d 0a0d 0a                          ]....
```

