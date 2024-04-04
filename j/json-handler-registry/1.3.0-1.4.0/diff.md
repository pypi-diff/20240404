# Comparing `tmp/json-handler-registry-1.3.0.tar.gz` & `tmp/json-handler-registry-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-handler-registry-1.3.0.tar", last modified: Mon Apr  1 18:19:20 2024, max compression
+gzip compressed data, was "dist/json-handler-registry-1.4.0.tar", last modified: Thu Apr  4 16:47:40 2024, max compression
```

## Comparing `json-handler-registry-1.3.0.tar` & `json-handler-registry-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2024-03-25 18:49:27.000000 json-handler-registry-1.3.0/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       81 2024-03-25 19:02:47.000000 json-handler-registry-1.3.0/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4517 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4000 2024-04-01 18:15:05.000000 json-handler-registry-1.3.0/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-03-31 11:40:57.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2452 2024-03-28 18:09:24.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/decoder.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1281 2024-03-31 11:37:08.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/encoder.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/py.typed
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3939 2024-04-01 17:44:53.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/registry.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      959 2024-04-01 18:16:02.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-01 18:10:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      282 2024-04-01 18:08:41.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/common.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1243 2024-04-01 18:13:30.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/dataclasses_json.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4517 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      676 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-25 19:03:21.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/not-zip-safe
--rw-r--r--   0 pawel     (1000) pawel     (1000)       22 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/setup.cfg
--rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2329 2024-03-25 19:37:00.000000 json-handler-registry-1.3.0/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2024-03-25 18:49:27.000000 json-handler-registry-1.4.0/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       81 2024-03-25 19:02:47.000000 json-handler-registry-1.4.0/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4911 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4394 2024-04-04 16:44:46.000000 json-handler-registry-1.4.0/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-04-04 16:13:08.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2466 2024-04-04 15:46:19.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/decoder.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1295 2024-04-04 15:46:10.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/encoder.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/py.typed
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4551 2024-04-04 16:37:45.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/registry.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      977 2024-04-04 15:59:25.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-01 18:10:20.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      358 2024-04-04 15:57:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/common.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1243 2024-04-01 18:13:30.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/dataclasses_json.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4911 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      676 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-25 19:03:21.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/not-zip-safe
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       22 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/setup.cfg
+-rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2329 2024-03-25 19:37:00.000000 json-handler-registry-1.4.0/setup.py
```

### Comparing `json-handler-registry-1.3.0/LICENSE.txt` & `json-handler-registry-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.3.0/PKG-INFO` & `json-handler-registry-1.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: json-handler-registry
-Version: 1.3.0
-Summary: Standardized way of registering custom JSON serializers/deserializers.
-Home-page: https://bitbucket.org/massultidev/tunit/
-Author: P.J. Grochowski
-Author-email: pawel.grochowski.dev@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI license](https://img.shields.io/pypi/l/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![Downloads](https://static.pepy.tech/badge/json-handler-registry)](https://pepy.tech/project/json-handler-registry)
 
 # JSON Handler Registry
 ---
@@ -32,17 +17,14 @@
 
 ```python
 from typing import Optional
 from json_handler_registry.registry import JsonHandlerRegistry
 from json_handler_registry.encoder import IJsonEncoder, EncodingResult
 from json_handler_registry.decoder import IJsonDecoder
 
-# Enable registry:
-JsonHandlerRegistry.enable()
-
 
 # Implement your custom class encoder:
 class MyJsonEncoder(IJsonEncoder):
     def encodeObject(self, obj: object) -> Optional[EncodingResult]:
         """Convert object to a JSON serializable data.
         Or return ``None`` instead.
         """
@@ -128,18 +110,26 @@
   option=TestEnum.Option2,
   value=Decimal(7)
 )
 
 PackageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
 assert TestDataClass.from_json(testData.to_json()) == testData
 PackageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
+
+# Instead of using 'PackageSupportManager' you can also manually register encoder:
+from json_handler_registry.registry import JsonHandlerRegistry
+from json_handler_registry.support.impl.dataclasses_json import DataClassJsonEncoder
+JsonHandlerRegistry.registerEncoder(DataClassJsonEncoder)
 ```
 
 ### Changelog:
 ---
+- Version: 1.4.0
+    - Preserving registration order of encoders/decoders.
+    - Configurable auto enable/disable registry feature. (Active by default.)
 - Version: 1.3.0
     - Support for `dataclasses-json` package.
     - Debug methods for listing registered encoders/decoders.
 - Version: 1.2.0
     - Guard to prevent registry from being easily overridden when enabled.
 - Version: 1.1.0
     - Registry accepts both type and instance of encoder/decoder.
```

### Comparing `json-handler-registry-1.3.0/README.md` & `json-handler-registry-1.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: json-handler-registry
+Version: 1.4.0
+Summary: Standardized way of registering custom JSON serializers/deserializers.
+Home-page: https://bitbucket.org/massultidev/tunit/
+Author: P.J. Grochowski
+Author-email: pawel.grochowski.dev@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI license](https://img.shields.io/pypi/l/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![Downloads](https://static.pepy.tech/badge/json-handler-registry)](https://pepy.tech/project/json-handler-registry)
 
 # JSON Handler Registry
 ---
@@ -17,17 +32,14 @@
 
 ```python
 from typing import Optional
 from json_handler_registry.registry import JsonHandlerRegistry
 from json_handler_registry.encoder import IJsonEncoder, EncodingResult
 from json_handler_registry.decoder import IJsonDecoder
 
-# Enable registry:
-JsonHandlerRegistry.enable()
-
 
 # Implement your custom class encoder:
 class MyJsonEncoder(IJsonEncoder):
     def encodeObject(self, obj: object) -> Optional[EncodingResult]:
         """Convert object to a JSON serializable data.
         Or return ``None`` instead.
         """
@@ -113,18 +125,26 @@
   option=TestEnum.Option2,
   value=Decimal(7)
 )
 
 PackageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
 assert TestDataClass.from_json(testData.to_json()) == testData
 PackageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
+
+# Instead of using 'PackageSupportManager' you can also manually register encoder:
+from json_handler_registry.registry import JsonHandlerRegistry
+from json_handler_registry.support.impl.dataclasses_json import DataClassJsonEncoder
+JsonHandlerRegistry.registerEncoder(DataClassJsonEncoder)
 ```
 
 ### Changelog:
 ---
+- Version: 1.4.0
+    - Preserving registration order of encoders/decoders.
+    - Configurable auto enable/disable registry feature. (Active by default.)
 - Version: 1.3.0
     - Support for `dataclasses-json` package.
     - Debug methods for listing registered encoders/decoders.
 - Version: 1.2.0
     - Guard to prevent registry from being easily overridden when enabled.
 - Version: 1.1.0
     - Registry accepts both type and instance of encoder/decoder.
```

### Comparing `json-handler-registry-1.3.0/pkg/json_handler_registry/decoder.py` & `json-handler-registry-1.4.0/pkg/json_handler_registry/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
 from abc import ABC
 from collections import deque
 from json import JSONDecoder
-from typing import Any, Callable, Deque, Dict, Optional, Type, Union
+from typing import Any, Callable, Deque, Optional, OrderedDict, Type, Union
 
 _Node = Union[dict, list]
 
 
 class IJsonDecoder(ABC):
     def decodeDict(self, dct: dict) -> Optional[object]:
         """Convert dictionary to your type instance.
@@ -17,15 +17,15 @@
         """
     def decodeStr(self, valueStr: str) -> Optional[object]:
         """Convert string value to your type instance.
         Or return ``None`` instead.
         """
 
 
-DecoderRegistryDict = Dict[Type[IJsonDecoder], IJsonDecoder]
+DecoderRegistryDict = OrderedDict[Type[IJsonDecoder], IJsonDecoder]
 
 
 class _JsonDecoderRegistryProxy(JSONDecoder):
 
     def __init__(
         self,
         registry: DecoderRegistryDict,
```

### Comparing `json-handler-registry-1.3.0/pkg/json_handler_registry/encoder.py` & `json-handler-registry-1.4.0/pkg/json_handler_registry/encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
 from abc import ABC
 from json import JSONEncoder
-from typing import Any, Dict, Optional, Type, Union
+from typing import Any, Optional, OrderedDict, Type, Union
 
 EncodingResult = Union[int, float, str, tuple, list, dict]
 
 
 class IJsonEncoder(ABC):
     def encodeObject(self, obj: object) -> Optional[EncodingResult]:
         """Convert object to a JSON serializable data.
         Or return ``None`` instead.
         """
 
 
-EncoderRegistryDict = Dict[Type[IJsonEncoder], IJsonEncoder]
+EncoderRegistryDict = OrderedDict[Type[IJsonEncoder], IJsonEncoder]
 
 
 class _JsonEncoderRegistryProxy(JSONEncoder):
 
     def __init__(
         self,
         registry: EncoderRegistryDict,
```

### Comparing `json-handler-registry-1.3.0/pkg/json_handler_registry/support/__init__.py` & `json-handler-registry-1.4.0/pkg/json_handler_registry/support/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
-from typing import Dict, List
+from typing import Dict, List, Type
 
 from json_handler_registry.support.impl.common import PackageSupportConfig
 from json_handler_registry.support.impl.dataclasses_json import DataClassJsonSupport
 
 
 class PackageSupportException(Exception):
     pass
 
 
 class PackageSupportManager:
 
-    _PACKAGE_SUPPORT_CONFIGS: Dict[str, PackageSupportConfig] = {
+    _PACKAGE_SUPPORT_CONFIGS: Dict[str, Type[PackageSupportConfig]] = {
         'dataclasses-json': DataClassJsonSupport,
     }
 
     @classmethod
     def getSupportedPackages(cls) -> List[str]:
         return list(cls._PACKAGE_SUPPORT_CONFIGS.keys())
 
     @classmethod
-    def getPackageSupportConfig(cls, package: str) -> PackageSupportConfig:
+    def getPackageSupportConfig(cls, package: str) -> Type[PackageSupportConfig]:
         packageSupportConfigOpt = cls._PACKAGE_SUPPORT_CONFIGS.get(package, None)
         if packageSupportConfigOpt is None:
             raise PackageSupportException(f"There is no builtin support for package: '{package}'")
 
         return packageSupportConfigOpt
```

### Comparing `json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/dataclasses_json.py` & `json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/dataclasses_json.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/PKG-INFO` & `json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-handler-registry
-Version: 1.3.0
+Version: 1.4.0
 Summary: Standardized way of registering custom JSON serializers/deserializers.
 Home-page: https://bitbucket.org/massultidev/tunit/
 Author: P.J. Grochowski
 Author-email: pawel.grochowski.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -32,17 +32,14 @@
 
 ```python
 from typing import Optional
 from json_handler_registry.registry import JsonHandlerRegistry
 from json_handler_registry.encoder import IJsonEncoder, EncodingResult
 from json_handler_registry.decoder import IJsonDecoder
 
-# Enable registry:
-JsonHandlerRegistry.enable()
-
 
 # Implement your custom class encoder:
 class MyJsonEncoder(IJsonEncoder):
     def encodeObject(self, obj: object) -> Optional[EncodingResult]:
         """Convert object to a JSON serializable data.
         Or return ``None`` instead.
         """
@@ -128,18 +125,26 @@
   option=TestEnum.Option2,
   value=Decimal(7)
 )
 
 PackageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
 assert TestDataClass.from_json(testData.to_json()) == testData
 PackageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
+
+# Instead of using 'PackageSupportManager' you can also manually register encoder:
+from json_handler_registry.registry import JsonHandlerRegistry
+from json_handler_registry.support.impl.dataclasses_json import DataClassJsonEncoder
+JsonHandlerRegistry.registerEncoder(DataClassJsonEncoder)
 ```
 
 ### Changelog:
 ---
+- Version: 1.4.0
+    - Preserving registration order of encoders/decoders.
+    - Configurable auto enable/disable registry feature. (Active by default.)
 - Version: 1.3.0
     - Support for `dataclasses-json` package.
     - Debug methods for listing registered encoders/decoders.
 - Version: 1.2.0
     - Guard to prevent registry from being easily overridden when enabled.
 - Version: 1.1.0
     - Registry accepts both type and instance of encoder/decoder.
```

### Comparing `json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/SOURCES.txt` & `json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.3.0/setup.py` & `json-handler-registry-1.4.0/setup.py`

 * *Files identical despite different names*

