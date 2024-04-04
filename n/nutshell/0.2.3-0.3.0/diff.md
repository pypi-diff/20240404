# Comparing `tmp/nutshell-0.2.3.tar.gz` & `tmp/nutshell-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutshell-0.2.3.tar", max compression
+gzip compressed data, was "nutshell-0.3.0.tar", max compression
```

## Comparing `nutshell-0.2.3.tar` & `nutshell-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1440 2024-04-01 18:23:07.044369 nutshell-0.2.3/README.md
--rw-r--r--   0        0        0      302 2024-04-01 17:36:10.805908 nutshell-0.2.3/nutshell/__init__.py
--rw-r--r--   0        0        0     3604 2024-04-01 17:08:09.751089 nutshell-0.2.3/nutshell/methods.py
--rw-r--r--   0        0        0     2366 2024-04-01 18:10:03.216510 nutshell-0.2.3/nutshell/nutshell_api.py
--rw-r--r--   0        0        0     2227 2024-04-01 17:39:14.853886 nutshell-0.2.3/nutshell/responses.py
--rw-r--r--   0        0        0      620 2024-04-01 18:24:16.792329 nutshell-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2068 1970-01-01 00:00:00.000000 nutshell-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2317 2024-04-04 17:35:01.732667 nutshell-0.3.0/README.md
+-rw-r--r--   0        0        0      560 2024-04-04 15:46:38.654303 nutshell-0.3.0/nutshell/__init__.py
+-rw-r--r--   0        0        0     4613 2024-04-04 15:46:38.582654 nutshell-0.3.0/nutshell/entities.py
+-rw-r--r--   0        0        0     4783 2024-04-04 15:35:35.560828 nutshell-0.3.0/nutshell/methods.py
+-rw-r--r--   0        0        0     2790 2024-04-04 14:02:17.333668 nutshell-0.3.0/nutshell/nutshell_api.py
+-rw-r--r--   0        0        0      777 2024-04-04 14:51:24.636154 nutshell-0.3.0/nutshell/responses.py
+-rw-r--r--   0        0        0      620 2024-04-04 17:53:50.755982 nutshell-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2945 1970-01-01 00:00:00.000000 nutshell-0.3.0/PKG-INFO
```

### Comparing `nutshell-0.2.3/README.md` & `nutshell-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,45 @@
-# Nushell API
+# Nutshell API
 
-This is a work-in-progress attempt at a pythonic API for Nutshell.
+This is a work-in-progress attempt at a pythonic API for querying the Nutshell CRM API. It does not yet support
+modifying data in a Nutshell instance.
 
 ## Installation
 
 ```bash 
 pip install nutshell
 ```
 
 ## Usage
 
-Create desired API calls as Pydantic models, pass the models to the NutshellAPI class, and call the API.
+This package includes four primary modules
+
+- methods: provides Pydantic models for a selection of Nutshell API methods
+    - model naming aligns with the API method names
+- responses: Pydantic models for the responses returned by the API
+    - response models are names with the API method name followed by "Result" (e.g. FindActivityTypes*Result*)
+- entities: enums and Pydantic models to facilitate method creation and parsing results
+- NutshellAPI class: provides a means to batch query the API with multiple methods via asyncio
+    - Must be instantiated with your Nutshell username and API key.
+
+### General flow
+
+- Instantiate API method calls and collect them in an iterable
+- Instantiate NutshellAPI with your Nutshell credentials
+- Pass the method calls iterable to the NutshellAPI instance
+- Call the API
+- Unpack the results
 
 ```python
 import asyncio
 import os
 
 from rich import print
-from dotenv import load_dotenv
 import nutshell as ns
 
-load_dotenv()
-
 single_call = ns.FindActivityTypes()
 
 nut = ns.NutshellAPI(os.getenv("NUTSHELL_USERNAME"), password=os.getenv("NUTSHELL_KEY"))
 nut.api_calls = [single_call]
 call_response = asyncio.run(nut.call_api())
 
 for call in call_response:
@@ -51,8 +65,13 @@
             ActivityTypes(stub=True, id=3, rev='3', entity_type='Activity_Types', name='Email/Log'),
         ]
     )
 )
 ```
 
 All responses have a `result` attribute that contains the data returned by the API. The data is returned as Pydantic
-models based on the API method invoked.
+models based on the API method invoked.
+
+## TODO
+
+- Handle errors returned from API
+- Convenience methods for common queries (Users, Leads, etc.)
```

### Comparing `nutshell-0.2.3/nutshell/nutshell_api.py` & `nutshell-0.3.0/nutshell/nutshell_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from typing import Sequence
 
 import aiohttp
 
-from .methods import _APIMethod
-from .responses import FindUsersResult, GetUserResult, GetAnalyticsReportResult, FindTeamsResult, \
-    FindActivityTypesResult, _APIResponse
+from methods import _APIMethod
+from responses import FindUsersResult, GetUserResult, GetAnalyticsReportResult, FindTeamsResult, \
+    FindActivityTypesResult, _APIResponse, FindStagesetsResult, FindMilestonesResult, FindLeadsResult
 
 
 class NutshellAPI:
     """Class to handle multiple API calls to the Nutshell API"""
     URL = "https://app.nutshell.com/api/v1/json"
 
     def __init__(self, username: str, password: str):
@@ -55,9 +55,15 @@
                     call_response.append((call, GetUserResult(**results[idx])))
                 case "findTeams":
                     call_response.append((call, FindTeamsResult(**results[idx])))
                 case "findActivityTypes":
                     call_response.append((call, FindActivityTypesResult(**results[idx])))
                 case "getAnalyticsReport":
                     call_response.append((call, GetAnalyticsReportResult(**results[idx])))
+                case "findStagesets":
+                    call_response.append((call, FindStagesetsResult(**results[idx])))
+                case "findMilestones":
+                    call_response.append((call, FindMilestonesResult(**results[idx])))
+                case "findLeads":
+                    call_response.append((call, FindLeadsResult(**results[idx])))
 
         return call_response
```

### Comparing `nutshell-0.2.3/pyproject.toml` & `nutshell-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nutshell"
-version = "0.2.3"
+version = "0.3.0"
 description = "Python wrapper on Nutshell CRM JSON RPC API"
 authors = ["Mark Nyberg <bigusdeveloper@gmail.com>"]
 license = "\"MIT\""
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `nutshell-0.2.3/PKG-INFO` & `nutshell-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutshell
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python wrapper on Nutshell CRM JSON RPC API
 License: "MIT"
 Author: Mark Nyberg
 Author-email: bigusdeveloper@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
@@ -12,38 +12,52 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Description-Content-Type: text/markdown
 
-# Nushell API
+# Nutshell API
 
-This is a work-in-progress attempt at a pythonic API for Nutshell.
+This is a work-in-progress attempt at a pythonic API for querying the Nutshell CRM API. It does not yet support
+modifying data in a Nutshell instance.
 
 ## Installation
 
 ```bash 
 pip install nutshell
 ```
 
 ## Usage
 
-Create desired API calls as Pydantic models, pass the models to the NutshellAPI class, and call the API.
+This package includes four primary modules
+
+- methods: provides Pydantic models for a selection of Nutshell API methods
+    - model naming aligns with the API method names
+- responses: Pydantic models for the responses returned by the API
+    - response models are names with the API method name followed by "Result" (e.g. FindActivityTypes*Result*)
+- entities: enums and Pydantic models to facilitate method creation and parsing results
+- NutshellAPI class: provides a means to batch query the API with multiple methods via asyncio
+    - Must be instantiated with your Nutshell username and API key.
+
+### General flow
+
+- Instantiate API method calls and collect them in an iterable
+- Instantiate NutshellAPI with your Nutshell credentials
+- Pass the method calls iterable to the NutshellAPI instance
+- Call the API
+- Unpack the results
 
 ```python
 import asyncio
 import os
 
 from rich import print
-from dotenv import load_dotenv
 import nutshell as ns
 
-load_dotenv()
-
 single_call = ns.FindActivityTypes()
 
 nut = ns.NutshellAPI(os.getenv("NUTSHELL_USERNAME"), password=os.getenv("NUTSHELL_KEY"))
 nut.api_calls = [single_call]
 call_response = asyncio.run(nut.call_api())
 
 for call in call_response:
@@ -70,7 +84,12 @@
         ]
     )
 )
 ```
 
 All responses have a `result` attribute that contains the data returned by the API. The data is returned as Pydantic
 models based on the API method invoked.
+
+## TODO
+
+- Handle errors returned from API
+- Convenience methods for common queries (Users, Leads, etc.)
```

