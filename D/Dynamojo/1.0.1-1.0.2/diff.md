# Comparing `tmp/dynamojo-1.0.1.tar.gz` & `tmp/dynamojo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamojo-1.0.1.tar", max compression
+gzip compressed data, was "dynamojo-1.0.2.tar", max compression
```

## Comparing `dynamojo-1.0.1.tar` & `dynamojo-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4600 2024-04-03 21:45:32.767591 dynamojo-1.0.1/README.md
--rw-r--r--   0        0        0      449 2024-04-03 21:30:22.401274 dynamojo-1.0.1/dynamojo/__init__.py
--rwxr-xr-x   0        0        0    20356 2024-04-03 21:31:37.755246 dynamojo-1.0.1/dynamojo/base.py
--rw-r--r--   0        0        0       89 2024-04-03 20:38:31.250208 dynamojo-1.0.1/dynamojo/boto.py
--rw-r--r--   0        0        0     2098 2024-04-03 21:30:22.427738 dynamojo-1.0.1/dynamojo/config.py
--rw-r--r--   0        0        0      445 2024-04-03 20:38:31.251170 dynamojo-1.0.1/dynamojo/exceptions.py
--rw-r--r--   0        0        0     4404 2024-04-03 21:30:22.449865 dynamojo-1.0.1/dynamojo/index.py
--rw-r--r--   0        0        0     1991 2024-04-03 21:30:22.437078 dynamojo-1.0.1/dynamojo/utils.py
--rw-r--r--   0        0        0      643 2024-04-03 21:47:15.479763 dynamojo-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 dynamojo-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4600 2024-04-03 21:48:11.818044 dynamojo-1.0.2/README.md
+-rw-r--r--   0        0        0      449 2024-04-03 21:30:22.401274 dynamojo-1.0.2/dynamojo/__init__.py
+-rwxr-xr-x   0        0        0    20343 2024-04-03 21:48:00.570599 dynamojo-1.0.2/dynamojo/base.py
+-rw-r--r--   0        0        0       89 2024-04-03 20:38:31.250208 dynamojo-1.0.2/dynamojo/boto.py
+-rw-r--r--   0        0        0     2098 2024-04-03 21:30:22.427738 dynamojo-1.0.2/dynamojo/config.py
+-rw-r--r--   0        0        0      445 2024-04-03 20:38:31.251170 dynamojo-1.0.2/dynamojo/exceptions.py
+-rw-r--r--   0        0        0     4404 2024-04-03 21:30:22.449865 dynamojo-1.0.2/dynamojo/index.py
+-rw-r--r--   0        0        0     1991 2024-04-03 21:30:22.437078 dynamojo-1.0.2/dynamojo/utils.py
+-rw-r--r--   0        0        0      643 2024-04-03 21:48:41.376507 dynamojo-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 dynamojo-1.0.2/PKG-INFO
```

### Comparing `dynamojo-1.0.1/README.md` & `dynamojo-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Dynamojo
 
 ---
 ###  :exclamation: Important Notice :exclamation:
 Version 1.0.0 is an important update that introduces breaking changes:
-  * Pydantic dependency is not at 2.x
+  * Pydantic dependency is now at 2.x
     * `DynamojoBase._config` attribute is now `DynamojoBase.__config__`
   * The following methods are now async:
     * `DynamojoBase.delete`
     * `DynamojoBase.fetch`
     * `DynamojoBase.query`
     * `DynamojoBase.save`
     * `DynamojoBase.update`
```

### Comparing `dynamojo-1.0.1/dynamojo/base.py` & `dynamojo-1.0.2/dynamojo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Dict, List, TypeVar, Union
 
 from boto3.dynamodb.conditions import (
     AttributeBase,
     ConditionBase,
     ConditionExpressionBuilder,
 )
-from pydantic import BaseModel, PrivateAttr
+from pydantic import BaseModel
 
 from .boto import DYNAMOCLIENT
 from .index import Index, Lsi
 from .config import DynamojoConfig
 from .exceptions import StaticAttributeError, IndexNotFoundError
 from .utils import Delta, TYPE_SERIALIZER, TYPE_DESERIALIZER
```

### Comparing `dynamojo-1.0.1/dynamojo/config.py` & `dynamojo-1.0.2/dynamojo/config.py`

 * *Files identical despite different names*

### Comparing `dynamojo-1.0.1/dynamojo/index.py` & `dynamojo-1.0.2/dynamojo/index.py`

 * *Files identical despite different names*

### Comparing `dynamojo-1.0.1/dynamojo/utils.py` & `dynamojo-1.0.2/dynamojo/utils.py`

 * *Files identical despite different names*

### Comparing `dynamojo-1.0.1/pyproject.toml` & `dynamojo-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "Dynamojo"
-version = "1.0.1"
-description = "ORM For dynamodb"
+version = "1.0.2"
+description = "ORM For Dynamodb"
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 homepage = "https://github.com/mathewmoon/dynamojo"
 repository = "https://github.com/mathewmoon/dynamojo"
 
 readme = "README.md"
 packages = [{include = "dynamojo", from = "."}]
```

### Comparing `dynamojo-1.0.1/PKG-INFO` & `dynamojo-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Dynamojo
-Version: 1.0.1
-Summary: ORM For dynamodb
+Version: 1.0.2
+Summary: ORM For Dynamodb
 Home-page: https://github.com/mathewmoon/dynamojo
 Author: Mathew Moon
 Author-email: me@mathewmoon.net
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.56,<2.0.0)
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 
 # Dynamojo
 
 ---
 ###  :exclamation: Important Notice :exclamation:
 Version 1.0.0 is an important update that introduces breaking changes:
-  * Pydantic dependency is not at 2.x
+  * Pydantic dependency is now at 2.x
     * `DynamojoBase._config` attribute is now `DynamojoBase.__config__`
   * The following methods are now async:
     * `DynamojoBase.delete`
     * `DynamojoBase.fetch`
     * `DynamojoBase.query`
     * `DynamojoBase.save`
     * `DynamojoBase.update`
```

