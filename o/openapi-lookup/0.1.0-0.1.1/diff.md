# Comparing `tmp/openapi_lookup-0.1.0.tar.gz` & `tmp/openapi_lookup-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_lookup-0.1.0.tar", max compression
+gzip compressed data, was "openapi_lookup-0.1.1.tar", max compression
```

## Comparing `openapi_lookup-0.1.0.tar` & `openapi_lookup-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-01-14 02:06:09.805230 openapi_lookup-0.1.0/LICENSE
--rw-r--r--   0        0        0     2784 2024-01-14 04:29:50.949548 openapi_lookup-0.1.0/README.md
--rw-r--r--   0        0        0     2357 2024-01-14 04:29:50.953546 openapi_lookup-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1202 2024-01-14 04:29:50.953546 openapi_lookup-0.1.0/src/openapi_lookup/__init__.py
--rw-r--r--   0        0        0     5309 2024-01-14 04:29:50.953546 openapi_lookup-0.1.0/src/openapi_lookup/cli.py
--rw-r--r--   0        0        0     3571 2024-01-14 04:29:50.953546 openapi_lookup-0.1.0/src/openapi_lookup/openapis.py
--rw-r--r--   0        0        0     4046 1970-01-01 00:00:00.000000 openapi_lookup-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-04 03:09:20.657537 openapi_lookup-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2784 2024-04-04 03:09:20.657537 openapi_lookup-0.1.1/README.md
+-rw-r--r--   0        0        0     2375 2024-04-04 03:09:43.037567 openapi_lookup-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1203 2024-04-04 03:09:43.037567 openapi_lookup-0.1.1/src/openapi_lookup/__init__.py
+-rw-r--r--   0        0        0     5310 2024-04-04 03:09:43.037567 openapi_lookup-0.1.1/src/openapi_lookup/cli.py
+-rw-r--r--   0        0        0     3572 2024-04-04 03:09:43.037567 openapi_lookup-0.1.1/src/openapi_lookup/openapis.py
+-rw-r--r--   0        0        0     4046 1970-01-01 00:00:00.000000 openapi_lookup-0.1.1/PKG-INFO
```

### Comparing `openapi_lookup-0.1.0/LICENSE` & `openapi_lookup-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_lookup-0.1.0/README.md` & `openapi_lookup-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openapi_lookup-0.1.0/pyproject.toml` & `openapi_lookup-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-lookup"
-version = "0.1.0"
+version = "0.1.1"
 description = "A command-line interface to for the open api listings from public-apis/public-apis."
 authors = ["xransum <xransum@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/xransum/openapi-lookup"
 repository = "https://github.com/xransum/openapi-lookup"
 documentation = "https://openapi-lookup.readthedocs.io"
@@ -28,14 +28,15 @@
 nox-poetry = "^1.0.3"
 sphinx-click = "^5.0.1"
 sphinx-rtd-theme = "^1.3.0"
 types-requests = "^2.31.0"
 appdirs = "^1.4.4"
 
 [tool.poetry.dev-dependencies]
+bandit = ">1.7.6"
 pytest = ">=6.2.5"
 coverage = { extras = ["toml"], version = ">=6.3" }
 safety = ">=1.10.3"
 mypy = ">=0.931"
 typeguard = ">=2.13.3"
 xdoctest = { extras = ["colors"], version = ">=0.15.10" }
 sphinx = ">=4.3.2"
```

### Comparing `openapi_lookup-0.1.0/src/openapi_lookup/__init__.py` & `openapi_lookup-0.1.1/src/openapi_lookup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Open API Lookup package."""
+
 import logging
 import os
 from pathlib import Path
 
 
 app_name = "openapi_lookup"
 app_root = Path(__file__).parent.parent.absolute()
```

### Comparing `openapi_lookup-0.1.0/src/openapi_lookup/cli.py` & `openapi_lookup-0.1.1/src/openapi_lookup/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI module."""
+
 import argparse
 from typing import Any, Dict, List
 
 from openapi_lookup import setup_logger, verbosity_levels
 from openapi_lookup.openapis import get_raw_public_apis, parse_rows
```

### Comparing `openapi_lookup-0.1.0/src/openapi_lookup/openapis.py` & `openapi_lookup-0.1.1/src/openapi_lookup/openapis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Github and data handler module."""
+
 import re
 from typing import Any, Dict, List
 
 import requests
 
 
 RAW_PUBLIC_APIS_URL = (
```

### Comparing `openapi_lookup-0.1.0/PKG-INFO` & `openapi_lookup-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-lookup
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command-line interface to for the open api listings from public-apis/public-apis.
 Home-page: https://github.com/xransum/openapi-lookup
 License: MIT
 Author: xransum
 Author-email: xransum@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

