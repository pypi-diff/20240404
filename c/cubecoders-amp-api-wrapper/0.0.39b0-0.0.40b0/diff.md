# Comparing `tmp/cubecoders_amp_api_wrapper-0.0.39b0.tar.gz` & `tmp/cubecoders_amp_api_wrapper-0.0.40b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubecoders_amp_api_wrapper-0.0.39b0.tar", last modified: Thu Mar 28 19:11:22 2024, max compression
+gzip compressed data, was "cubecoders_amp_api_wrapper-0.0.40b0.tar", last modified: Wed Apr  3 23:12:58 2024, max compression
```

## Comparing `cubecoders_amp_api_wrapper-0.0.39b0.tar` & `cubecoders_amp_api_wrapper-0.0.40b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-03-28 19:11:22.659348 cubecoders_amp_api_wrapper-0.0.39b0/
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     7281 2024-03-28 19:11:21.000000 cubecoders_amp_api_wrapper-0.0.39b0/CHANGELOG.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    35823 2024-02-19 17:57:42.000000 cubecoders_amp_api_wrapper-0.0.39b0/LICENSE
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       79 2024-03-28 19:08:10.000000 cubecoders_amp_api_wrapper-0.0.39b0/MANIFEST.in
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     5462 2024-03-28 19:11:22.657331 cubecoders_amp_api_wrapper-0.0.39b0/PKG-INFO
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     3603 2024-03-28 17:27:49.000000 cubecoders_amp_api_wrapper-0.0.39b0/README.md
-drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-03-28 19:11:22.496883 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     1628 2024-03-28 19:10:56.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/__init__.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2473 2024-03-28 16:25:01.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/ads.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    78166 2024-03-26 16:30:03.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/adsmodule.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    15526 2024-03-28 16:33:07.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/base.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     1658 2024-03-27 02:49:13.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/bridge.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    77158 2024-03-28 16:55:16.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/core.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)      272 2024-02-22 21:10:24.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/emailsender.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     8195 2024-03-26 15:46:14.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/filebackup.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    23108 2024-03-26 16:10:34.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/filemanager.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2918 2024-03-28 16:48:17.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/instance.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    20228 2024-03-27 15:24:21.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/minecraft.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    36105 2024-03-28 16:33:07.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/types.py
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     3674 2024-02-27 23:58:27.000000 cubecoders_amp_api_wrapper-0.0.39b0/ampapi/util.py
-drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-03-28 19:11:22.562247 cubecoders_amp_api_wrapper-0.0.39b0/cubecoders_amp_api_wrapper.egg-info/
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     5462 2024-03-28 19:11:22.000000 cubecoders_amp_api_wrapper-0.0.39b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)      696 2024-03-28 19:11:22.000000 cubecoders_amp_api_wrapper-0.0.39b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        1 2024-03-28 19:11:22.000000 cubecoders_amp_api_wrapper-0.0.39b0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       59 2024-03-28 19:11:22.000000 cubecoders_amp_api_wrapper-0.0.39b0/cubecoders_amp_api_wrapper.egg-info/requires.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        7 2024-03-28 19:11:22.000000 cubecoders_amp_api_wrapper-0.0.39b0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
-drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-03-28 19:11:22.639199 cubecoders_amp_api_wrapper-0.0.39b0/docs/
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    44207 2024-02-29 23:02:05.000000 cubecoders_amp_api_wrapper-0.0.39b0/docs/ADS_api_spec.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    29522 2024-02-28 00:01:43.000000 cubecoders_amp_api_wrapper-0.0.39b0/docs/Minecraft_api_spec.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    10703 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.39b0/docs/permission_nodes.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    10703 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.39b0/docs/permission_nodes.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     4816 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.39b0/docs/setting_nodes.md
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     4774 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.39b0/docs/setting_nodes.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       59 2024-03-28 18:44:49.000000 cubecoders_amp_api_wrapper-0.0.39b0/requirements.txt
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       38 2024-03-28 19:11:22.659849 cubecoders_amp_api_wrapper-0.0.39b0/setup.cfg
--rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2193 2024-03-28 19:05:44.000000 cubecoders_amp_api_wrapper-0.0.39b0/setup.py
+drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-03 23:12:58.195540 cubecoders_amp_api_wrapper-0.0.40b0/
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     7535 2024-04-03 23:12:56.000000 cubecoders_amp_api_wrapper-0.0.40b0/CHANGELOG.md
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    35823 2024-02-19 17:57:42.000000 cubecoders_amp_api_wrapper-0.0.40b0/LICENSE
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       79 2024-03-28 19:08:10.000000 cubecoders_amp_api_wrapper-0.0.40b0/MANIFEST.in
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     5436 2024-04-03 23:12:58.193957 cubecoders_amp_api_wrapper-0.0.40b0/PKG-INFO
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     3570 2024-04-03 23:06:15.000000 cubecoders_amp_api_wrapper-0.0.40b0/README.md
+drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-03 23:12:58.067871 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     1628 2024-04-03 23:12:06.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/__init__.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2473 2024-04-03 23:06:44.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/ads.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    78168 2024-04-03 23:06:45.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/adsmodule.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    15528 2024-04-03 23:06:46.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/base.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     1660 2024-04-03 23:06:47.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/bridge.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    77162 2024-04-03 23:06:49.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/core.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)      272 2024-04-03 23:06:51.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/emailsender.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     8197 2024-04-03 23:06:52.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/filebackup.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    23110 2024-04-03 23:06:53.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/filemanager.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2918 2024-04-03 23:06:54.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/instance.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    20234 2024-04-03 23:06:54.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/minecraft.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    36107 2024-04-03 23:06:56.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/types.py
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     3678 2024-04-03 23:06:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/ampapi/util.py
+drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-03 23:12:58.118435 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     5436 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)      696 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        1 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       59 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/requires.txt
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        7 2024-04-03 23:12:57.000000 cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-03 23:12:58.182922 cubecoders_amp_api_wrapper-0.0.40b0/docs/
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    44207 2024-02-29 23:02:05.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/ADS_api_spec.md
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    29522 2024-02-28 00:01:43.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/Minecraft_api_spec.md
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    10703 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/permission_nodes.md
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)    10703 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/permission_nodes.txt
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     4816 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/setting_nodes.md
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     4774 2024-02-18 18:04:20.000000 cubecoders_amp_api_wrapper-0.0.40b0/docs/setting_nodes.txt
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       59 2024-03-28 18:44:49.000000 cubecoders_amp_api_wrapper-0.0.40b0/requirements.txt
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)       38 2024-04-03 23:12:58.196279 cubecoders_amp_api_wrapper-0.0.40b0/setup.cfg
+-rwxrwxrwx   0 k8thekat  (1000) k8thekat  (1000)     2195 2024-04-03 23:07:00.000000 cubecoders_amp_api_wrapper-0.0.40b0/setup.py
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/CHANGELOG.md` & `cubecoders_amp_api_wrapper-0.0.40b0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## Version - 0.0.40b - [b055fb3](https://github.com/k8thekat/AMPAPI_Python/commit/b055fb3)
+#### Readme.md
+- Changed TestPypi to Pypi
+	- Updated bash commands for installing package.
+
+#### init.py
+- Version bump `0.0.40b`
+
+#### Overall
+- `isort` imports
+
 ## Version - 0.0.39b - [778bb87](https://github.com/k8thekat/AMPAPI_Python/commit/778bb87)
 #### __init__.py
 - Version bump `0.0.39b`
 - Added `MANIFEST.in`
 
 #### setup.py
 - Re-added requirements.txt
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/LICENSE` & `cubecoders_amp_api_wrapper-0.0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/PKG-INFO` & `cubecoders_amp_api_wrapper-0.0.40b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubecoders_amp_api_wrapper
-Version: 0.0.39b0
+Version: 0.0.40b0
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
@@ -24,21 +24,22 @@
         ### Installing
         ___
         
         *Python 3.9 or higher is required*
         
         To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
         
-        ### TestPypi
+        ### Pypi 
+        -> https://pypi.org/project/cubecoders-amp-api-wrapper/
         ```bash
         # Linux/macOS
-        python3 -m pip install -i https://test.pypi.org/simple/ cubecoders-amp-api-wrapper
+        pip install cubecoders-amp-api-wrapper
         
         # Windows
-        python -m pip install -i https://test.pypi.org/simple/ cubecoders-amp-api-wrapper
+        pip install cubecoders-amp-api-wrapper
         ```
         
         
         ### Quick Example -
         
         ```py
         # You can pull these values from an `.ini` or a `.env` file,
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/README.md` & `cubecoders_amp_api_wrapper-0.0.40b0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 ### Installing
 ___
 
 *Python 3.9 or higher is required*
 
 To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
 
-### TestPypi
+### Pypi 
+-> https://pypi.org/project/cubecoders-amp-api-wrapper/
 ```bash
 # Linux/macOS
-python3 -m pip install -i https://test.pypi.org/simple/ cubecoders-amp-api-wrapper
+pip install cubecoders-amp-api-wrapper
 
 # Windows
-python -m pip install -i https://test.pypi.org/simple/ cubecoders-amp-api-wrapper
+pip install cubecoders-amp-api-wrapper
 ```
 
 
 ### Quick Example -
 
 ```py
 # You can pull these values from an `.ini` or a `.env` file,
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/__init__.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,31 +19,31 @@
    02110-1301, USA. 
 '''
 from __future__ import annotations
 
 __title__ = "CubeCoders AMP API"
 __author__ = "k8thekat"
 __license__ = "GNU"
-__version__ = "0.0.39b"
+__version__ = "0.0.40b"
 __credits__ = "AMP by CubeCoders and associates."
 
+from typing import Literal, NamedTuple
+
 from .ads import *
 from .adsmodule import *
 from .bridge import *
 from .core import *
 from .emailsender import *
-from .filemanager import *
 from .filebackup import *
+from .filemanager import *
 from .instance import *
 from .minecraft import *
 from .types import *
 from .util import *
 
-from typing import NamedTuple, Literal
-
 
 class VersionInfo(NamedTuple):
     Major: int
     Minor: int
     Revision: int
     releaseLevel: Literal["alpha", "beta", "release"]
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/ads.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/ads.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import TYPE_CHECKING, Self, Union
-from .types import Controller, Instance
+
 from .adsmodule import ADSModule
 from .core import Core
 from .emailsender import EmailSenderPlugin
 from .filebackup import LocalFileBackupPlugin
 from .filemanager import FileManagerPlugin
 from .instance import AMPInstance, AMPMinecraftInstance
-
+from .types import Controller, Instance
 
 __all__ = ("ADSInstance",)
 
 
 class ADSInstance(ADSModule, Core, EmailSenderPlugin, LocalFileBackupPlugin, FileManagerPlugin, Controller):
     """
     The ADS class is the top most level of Instances inside of AMP, may also be referred to as the "Controller".
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/adsmodule.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/adsmodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
+
+from dataclasses import fields
 from typing import Union
 
-from .types import *
 from .base import Base
-from dataclasses import fields
+from .types import *
 
 __all__ = ("ADSModule",)
 
 
 class ADSModule(Base):
     """
     Contains the base functions for any `/API/ADSModule/` AMP API endpoints.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/base.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
-from datetime import timedelta
-from typing import Union, Any, TYPE_CHECKING
+
 import json
-import traceback
 import logging
+import traceback
 from dataclasses import fields
-from dataclass_wizard import fromdict
+from datetime import timedelta
+from typing import TYPE_CHECKING, Any, Union
 
 import aiohttp
 from aiohttp import ClientResponse
-
+from dataclass_wizard import fromdict
 from pyotp import TOTP
 
 from ampapi.types import APISession  # 2Factor Authentication Python Module
-from .types import *
+
 from .bridge import Bridge
+from .types import *
 
 if TYPE_CHECKING:
     from typing import Self
 
 __all__ = ("Base",)
 
 FORMAT_DATA: bool = True
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/bridge.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from dataclasses import fields
 from typing import TYPE_CHECKING, Self
+
 from .types import APIParams
-from dataclasses import fields
 
 __all__ = ("Bridge",)
 
 
 class Bridge(APIParams):
     """
     Handles the API login credentials for connecting to AMP.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/core.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
+
 from typing import Any, Union
-from .types import *
+
 from .base import Base
+from .types import *
 
 __all__ = ("Core",)
 
 
 class Core(Base):
     """
     Contains the base functions for any `/API/Core/` AMP API endpoints.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/filebackup.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/filebackup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
+
 from typing import Union
 
-from .types import *
 from .base import Base
+from .types import *
 
 __all__ = ("LocalFileBackupPlugin",)
 
 
 class LocalFileBackupPlugin(Base):
     """
     Contains the base functions for any `/API/LocalFileBackupPlugin/` AMP API endpoints.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/filemanager.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/filemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
+
 from typing import Union
 
+from .base import FORMAT_DATA, Base
 from .types import *
-from .base import Base, FORMAT_DATA
 
 __all__ = ("FileManagerPlugin",)
 
 
 class FileManagerPlugin(Base):
     """
     Contains the base functions for any `/API/FileManagerPlugin/` AMP API endpoints.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/instance.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Union
-from .types import Instance, AppStatus, Updates, State_enum
+
 from .adsmodule import ADSModule
 from .core import Core
 from .emailsender import EmailSenderPlugin
 from .filebackup import LocalFileBackupPlugin
 from .filemanager import FileManagerPlugin
 from .minecraft import MinecraftModule
-
+from .types import AppStatus, Instance, State_enum, Updates
 
 __all__ = ("AMPInstance", "AMPMinecraftInstance")
 
 
 class AMPInstance(Core, EmailSenderPlugin, LocalFileBackupPlugin, FileManagerPlugin, Instance, AppStatus, Updates):
     """
     AMPInstance represents an entire Instance from AMP that is not the main panel.\n
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/minecraft.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/minecraft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
+
 from typing import Any, Union
+
 from dataclass_wizard import fromdict
+
+from .base import FORMAT_DATA, Base
 from .types import *
-from .base import Base, FORMAT_DATA
 
 __all__ = ("MinecraftModule",)
 
 
 class MinecraftModule(Base):
     """
     Contains the base functions for any `/API/MinecraftModule/` AMP API endpoints.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/types.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # API class types
 from __future__ import annotations
-from typing import Any, Union
+
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
+from typing import Any, Union
 
 
 class State_enum(Enum):
     """
     Represents the state of an instance
 
     Author: p0t4t0sandwich -> https://github.com/p0t4t0sandwich/ampapi-py/blob/main/ampapi/types.py
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/ampapi/util.py` & `cubecoders_amp_api_wrapper-0.0.40b0/ampapi/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
-from .core import Core
+
 from pathlib import Path
 from typing import Any
 
+from .core import Core
+
 
 class APIUtil():
     """
     AMP API util functions to parse specific API calls for specific Data.
     """
 
     async def get_node_spec(self, amp: Core) -> str | dict[str, Any] | list | bool | int | None:
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO` & `cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubecoders-amp-api-wrapper
-Version: 0.0.39b0
+Version: 0.0.40b0
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
@@ -24,21 +24,22 @@
         ### Installing
         ___
         
         *Python 3.9 or higher is required*
         
         To install run the below command to install the required pip packages from [Requirements](./requirements.txt)
         
-        ### TestPypi
+        ### Pypi 
+        -> https://pypi.org/project/cubecoders-amp-api-wrapper/
         ```bash
         # Linux/macOS
-        python3 -m pip install -i https://test.pypi.org/simple/ cubecoders-amp-api-wrapper
+        pip install cubecoders-amp-api-wrapper
         
         # Windows
-        python -m pip install -i https://test.pypi.org/simple/ cubecoders-amp-api-wrapper
+        pip install cubecoders-amp-api-wrapper
         ```
         
         
         ### Quick Example -
         
         ```py
         # You can pull these values from an `.ini` or a `.env` file,
```

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt` & `cubecoders_amp_api_wrapper-0.0.40b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/docs/ADS_api_spec.md` & `cubecoders_amp_api_wrapper-0.0.40b0/docs/ADS_api_spec.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/docs/Minecraft_api_spec.md` & `cubecoders_amp_api_wrapper-0.0.40b0/docs/Minecraft_api_spec.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/docs/permission_nodes.md` & `cubecoders_amp_api_wrapper-0.0.40b0/docs/permission_nodes.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/docs/permission_nodes.txt` & `cubecoders_amp_api_wrapper-0.0.40b0/docs/permission_nodes.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/docs/setting_nodes.md` & `cubecoders_amp_api_wrapper-0.0.40b0/docs/setting_nodes.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/docs/setting_nodes.txt` & `cubecoders_amp_api_wrapper-0.0.40b0/docs/setting_nodes.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.39b0/setup.py` & `cubecoders_amp_api_wrapper-0.0.40b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from setuptools import setup
 import re
 
+from setuptools import setup
+
 requirements: list[str] = []
 with open("./requirements.txt") as file:
     requirements = file.read().splitlines()
 
 readme = ''
 with open('./README.md') as file:
     readme: str = file.read()
```

