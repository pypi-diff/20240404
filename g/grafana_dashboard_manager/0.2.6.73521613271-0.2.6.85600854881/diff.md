# Comparing `tmp/grafana_dashboard_manager-0.2.6.73521613271.tar.gz` & `tmp/grafana_dashboard_manager-0.2.6.85600854881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana_dashboard_manager-0.2.6.73521613271.tar", max compression
+gzip compressed data, was "grafana_dashboard_manager-0.2.6.85600854881.tar", max compression
```

## Comparing `grafana_dashboard_manager-0.2.6.73521613271.tar` & `grafana_dashboard_manager-0.2.6.85600854881.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1082 2023-12-28 23:53:22.308305 grafana_dashboard_manager-0.2.6.73521613271/LICENSE
--rw-r--r--   0        0        0     4370 2023-12-28 23:53:22.308305 grafana_dashboard_manager-0.2.6.73521613271/README.md
--rw-r--r--   0        0        0        0 2023-12-28 23:53:22.308305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/__init__.py
--rw-r--r--   0        0        0     3844 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/__main__.py
--rw-r--r--   0        0        0     2258 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/api/auth.py
--rw-r--r--   0        0        0     2084 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/api/rest_client.py
--rw-r--r--   0        0        0      100 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/commands/__init__.py
--rw-r--r--   0        0        0     3251 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/commands/dashboard_download.py
--rw-r--r--   0        0        0     6241 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/commands/dashboard_upload.py
--rw-r--r--   0        0        0      367 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/exceptions.py
--rw-r--r--   0        0        0     3441 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/global_config.py
--rw-r--r--   0        0        0      248 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/grafana/__init__.py
--rw-r--r--   0        0        0     2228 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/grafana/grafana_api.py
--rw-r--r--   0        0        0     4288 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/handlers/api_dashboards.py
--rw-r--r--   0        0        0     3609 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/handlers/api_folders.py
--rw-r--r--   0        0        0     1566 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/handlers/base_handler.py
--rw-r--r--   0        0        0      342 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/models/__init__.py
--rw-r--r--   0        0        0     1184 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/models/dashboard.py
--rw-r--r--   0        0        0      558 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/models/folder.py
--rw-r--r--   0        0        0     3387 2023-12-28 23:53:22.312305 grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/utils.py
--rw-r--r--   0        0        0      873 2023-12-28 23:53:41.492231 grafana_dashboard_manager-0.2.6.73521613271/pyproject.toml
--rw-r--r--   0        0        0     5209 1970-01-01 00:00:00.000000 grafana_dashboard_manager-0.2.6.73521613271/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/LICENSE
+-rw-r--r--   0        0        0     4370 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/__init__.py
+-rw-r--r--   0        0        0     3844 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/__main__.py
+-rw-r--r--   0        0        0     2260 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/api/auth.py
+-rw-r--r--   0        0        0     2086 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/api/rest_client.py
+-rw-r--r--   0        0        0      100 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/commands/__init__.py
+-rw-r--r--   0        0        0     3252 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/commands/dashboard_download.py
+-rw-r--r--   0        0        0     6242 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/commands/dashboard_upload.py
+-rw-r--r--   0        0        0      367 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/exceptions.py
+-rw-r--r--   0        0        0     3442 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/global_config.py
+-rw-r--r--   0        0        0      249 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/grafana/__init__.py
+-rw-r--r--   0        0        0     2229 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/grafana/grafana_api.py
+-rw-r--r--   0        0        0     4289 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/handlers/api_dashboards.py
+-rw-r--r--   0        0        0     3610 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/handlers/api_folders.py
+-rw-r--r--   0        0        0     1567 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/handlers/base_handler.py
+-rw-r--r--   0        0        0      343 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/models/__init__.py
+-rw-r--r--   0        0        0     1185 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/models/dashboard.py
+-rw-r--r--   0        0        0      559 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/models/folder.py
+-rw-r--r--   0        0        0     3388 2024-04-04 19:15:10.463189 grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/utils.py
+-rw-r--r--   0        0        0      857 2024-04-04 19:15:26.467128 grafana_dashboard_manager-0.2.6.85600854881/pyproject.toml
+-rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 grafana_dashboard_manager-0.2.6.85600854881/PKG-INFO
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/LICENSE` & `grafana_dashboard_manager-0.2.6.85600854881/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/README.md` & `grafana_dashboard_manager-0.2.6.85600854881/README.md`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/__main__.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/api/auth.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/api/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 from base64 import b64encode
 from enum import Enum
 
 import httpx
 
 
 class GrafanaAuthType(Enum):
@@ -39,14 +40,15 @@
             token: bearer token auth token (default: {None})
 
         Returns:
             None
 
         Raises:
             ValueError: if provided args does not satisfy the requirements of auth_type
+
         """
         self.auth_type = auth_type
         self.auth_header_prefix = auth_type.value
 
         self.username = username
         self.password = password
         self.token = token
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/api/rest_client.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/api/rest_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import logging
 
 import httpx
 
 logger = logging.getLogger(__name__)
 
 
@@ -21,14 +22,15 @@
 
         Args:
             headers: common headers to apply to all requests
             auth: an httpx auth object
             base_url: url host
             skip_verify: set to true to skip verification of https connection certs
             verbose: increased logging output
+
         """
         self.client = httpx.Client(headers=headers, auth=auth, base_url=base_url, verify=skip_verify)
         self.verbose = verbose
 
     def get(self, resource: str) -> httpx.Response:
         """HTTP GET"""
         return self._make_request("GET", resource)
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/commands/dashboard_download.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/commands/dashboard_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import json
 import logging
 import os
 
 from grafana_dashboard_manager.global_config import GlobalConfig
 from grafana_dashboard_manager.grafana.grafana_api import GrafanaApi
 from grafana_dashboard_manager.models import DashboardFolderLookup, DashboardSearchResult
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/commands/dashboard_upload.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/commands/dashboard_upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import json
 import logging
 from pathlib import Path
 
 from grafana_dashboard_manager.global_config import GlobalConfig
 from grafana_dashboard_manager.grafana.grafana_api import GrafanaApi
 from grafana_dashboard_manager.models.folder import Folder
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/global_config.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/global_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import logging
 from pathlib import Path
 from typing import Callable, Literal
 
 from pydantic import BaseModel, field_validator
 
 logger = logging.getLogger(__name__)
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/grafana/grafana_api.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/grafana/grafana_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import logging
 
 from grafana_dashboard_manager.api.auth import GrafanaAuth, GrafanaAuthType
 from grafana_dashboard_manager.api.rest_client import RestClient
 from grafana_dashboard_manager.handlers.api_dashboards import ApiDashboards
 from grafana_dashboard_manager.handlers.api_folders import ApiFolders
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/handlers/api_dashboards.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/handlers/api_dashboards.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import json
 import logging
 from datetime import datetime
 from pathlib import Path
 
 import httpx
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/handlers/api_folders.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/handlers/api_folders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import logging
 from typing import Type
 
 from grafana_dashboard_manager.api.rest_client import RestClient
 from grafana_dashboard_manager.exceptions import FolderExistsException, FolderNotFoundException, GrafanaApiException
 from grafana_dashboard_manager.handlers.base_handler import BaseHandler
 from grafana_dashboard_manager.models import DashboardSearchResult, Folder
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/handlers/base_handler.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/handlers/base_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import logging
 from typing import Generic, TypeVar
 
 import httpx
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/models/dashboard.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/models/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 # ruff: noqa: D101
 from typing import Literal
 
 from pydantic import BaseModel
 
 
 class DashboardBase(BaseModel):
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/models/folder.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/models/folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 # ruff: noqa: D101
 from datetime import datetime
 
 from pydantic import BaseModel
 
 
 class Folder(BaseModel):
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/grafana_dashboard_manager/utils.py` & `grafana_dashboard_manager-0.2.6.85600854881/grafana_dashboard_manager/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright (c) 2024 BEAM CONNECTIVITY LIMITED
 
 Use of this source code is governed by an MIT-style
 license that can be found in the LICENSE file or at
 https://opensource.org/licenses/MIT.
 """
+
 import logging
 from pathlib import Path
 
 import rich
 import tomllib
 from rich.filesize import decimal
 from rich.logging import RichHandler
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/pyproject.toml` & `grafana_dashboard_manager-0.2.6.85600854881/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "grafana_dashboard_manager"
-version = "0.2.6.73521613271"
+version = "0.2.6.85600854881"
 description = "A cli utility that uses Grafana's HTTP API to easily save and restore dashboards."
 authors = ["Vince Chan <vince@beamconnectivity.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.beamconnectivity.com"
 repository = "https://github.com/Beam-Connectivity/grafana-dashboard-manager"
 keywords = ["grafana", "dashboard", "json"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-rich = "^13.7.0"
-httpx = "^0.25.2"
-pydantic = "^2.5.2"
-ruff = "^0.1.9"
+rich = "^13.7.1"
+httpx = "^0.27.0"
+pydantic = "^2.6.4"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
-ruff = "^0.1.6"
+pytest = "^8.1.1"
+ruff = "^0.3.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 grafana-dashboard-manager = "grafana_dashboard_manager.__main__:app"
```

### Comparing `grafana_dashboard_manager-0.2.6.73521613271/PKG-INFO` & `grafana_dashboard_manager-0.2.6.85600854881/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: grafana_dashboard_manager
-Version: 0.2.6.73521613271
+Version: 0.2.6.85600854881
 Summary: A cli utility that uses Grafana's HTTP API to easily save and restore dashboards.
 Home-page: https://www.beamconnectivity.com
 License: MIT
 Keywords: grafana,dashboard,json
 Author: Vince Chan
 Author-email: vince@beamconnectivity.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: httpx (>=0.25.2,<0.26.0)
-Requires-Dist: pydantic (>=2.5.2,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
-Requires-Dist: ruff (>=0.1.9,<0.2.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Project-URL: Repository, https://github.com/Beam-Connectivity/grafana-dashboard-manager
 Description-Content-Type: text/markdown
 
 # grafana-dashboard-manager
 
 ![CodeQL](https://github.com/Beam-Connectivity/grafana-dashboard-manager/actions/workflows/codeql-analysis.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/grafana_dashboard_manager.svg)](https://badge.fury.io/py/grafana_dashboard_manager)
```

