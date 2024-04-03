# Comparing `tmp/communex-0.1.7.tar.gz` & `tmp/communex-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communex-0.1.7.tar", max compression
+gzip compressed data, was "communex-0.1.8.tar", max compression
```

## Comparing `communex-0.1.7.tar` & `communex-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      909 2024-03-23 11:18:25.661457 communex-0.1.7/LICENSE
--rw-r--r--   0        0        0     4575 2024-03-24 19:18:19.153594 communex-0.1.7/README.md
--rw-r--r--   0        0        0     1385 2024-04-03 17:44:02.217963 communex-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      451 2024-03-30 15:42:14.063605 communex-0.1.7/src/communex/__init__.py
--rw-r--r--   0        0        0     1237 2024-04-03 17:43:47.736268 communex-0.1.7/src/communex/_common.py
--rw-r--r--   0        0        0      426 2024-03-23 11:18:25.662457 communex-0.1.7/src/communex/balance.py
--rw-r--r--   0        0        0       41 2024-04-02 20:20:50.841713 communex-0.1.7/src/communex/cli/__init__.py
--rw-r--r--   0        0        0       86 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/__main__.py
--rw-r--r--   0        0        0     1985 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/_common.py
--rw-r--r--   0        0        0     6735 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/balance.py
--rw-r--r--   0        0        0     7590 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/key.py
--rw-r--r--   0        0        0     2406 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/misc.py
--rw-r--r--   0        0        0     6408 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/module.py
--rw-r--r--   0        0        0     5536 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/network.py
--rw-r--r--   0        0        0     1181 2024-04-02 20:25:06.421248 communex-0.1.7/src/communex/cli/root.py
--rw-r--r--   0        0        0     3546 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/subnet.py
--rw-r--r--   0        0        0    91414 2024-03-30 15:44:47.719256 communex-0.1.7/src/communex/client.py
--rw-r--r--   0        0        0      297 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/compat/__init__.py
--rw-r--r--   0        0        0     1120 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/compat/_util.py
--rw-r--r--   0        0        0     5290 2024-03-25 19:42:20.678258 communex-0.1.7/src/communex/compat/key.py
--rw-r--r--   0        0        0     2636 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/compat/storage.py
--rw-r--r--   0        0        0      386 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/compat/types.py
--rw-r--r--   0        0        0      262 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/errors.py
--rw-r--r--   0        0        0     1329 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/key.py
--rw-r--r--   0        0        0    12756 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/misc.py
--rw-r--r--   0        0        0      142 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/module/__init__.py
--rw-r--r--   0        0        0     1533 2024-03-23 14:58:10.559875 communex-0.1.7/src/communex/module/_ip_limiter.py
--rw-r--r--   0        0        0     2059 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/module/_signer.py
--rw-r--r--   0        0        0     2712 2024-03-25 14:07:08.730822 communex-0.1.7/src/communex/module/client.py
--rw-r--r--   0        0        0        0 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/module/example/__init__.py
--rw-r--r--   0        0        0     1562 2024-03-30 16:16:22.622958 communex-0.1.7/src/communex/module/example/gpt.py
--rw-r--r--   0        0        0      544 2024-03-23 11:18:25.664457 communex-0.1.7/src/communex/module/example/openai.py
--rw-r--r--   0        0        0     2086 2024-03-23 11:18:25.664457 communex-0.1.7/src/communex/module/module.py
--rw-r--r--   0        0        0     7676 2024-03-30 16:23:28.999483 communex-0.1.7/src/communex/module/server.py
--rw-r--r--   0        0        0      381 2024-03-23 11:18:25.664457 communex-0.1.7/src/communex/module/stuff.md
--rw-r--r--   0        0        0     2272 2024-03-30 16:12:44.684414 communex-0.1.7/src/communex/types.py
--rw-r--r--   0        0        0     1333 2024-03-23 11:18:25.664457 communex-0.1.7/src/communex/util.py
--rw-r--r--   0        0        0     5606 1970-01-01 00:00:00.000000 communex-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      909 2024-03-23 11:18:25.661457 communex-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4575 2024-03-24 19:18:19.153594 communex-0.1.8/README.md
+-rw-r--r--   0        0        0     1385 2024-04-03 22:10:50.105212 communex-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      451 2024-03-30 15:42:14.063605 communex-0.1.8/src/communex/__init__.py
+-rw-r--r--   0        0        0     1572 2024-04-03 22:10:23.093921 communex-0.1.8/src/communex/_common.py
+-rw-r--r--   0        0        0      426 2024-03-23 11:18:25.662457 communex-0.1.8/src/communex/balance.py
+-rw-r--r--   0        0        0       41 2024-04-02 20:20:50.841713 communex-0.1.8/src/communex/cli/__init__.py
+-rw-r--r--   0        0        0       86 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/__main__.py
+-rw-r--r--   0        0        0     2302 2024-04-03 22:10:23.093921 communex-0.1.8/src/communex/cli/_common.py
+-rw-r--r--   0        0        0     6735 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/balance.py
+-rw-r--r--   0        0        0     7590 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/key.py
+-rw-r--r--   0        0        0     2406 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/misc.py
+-rw-r--r--   0        0        0     6408 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/module.py
+-rw-r--r--   0        0        0     5536 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/network.py
+-rw-r--r--   0        0        0     1449 2024-04-03 22:10:23.093921 communex-0.1.8/src/communex/cli/root.py
+-rw-r--r--   0        0        0     3546 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/subnet.py
+-rw-r--r--   0        0        0    91414 2024-03-30 15:44:47.719256 communex-0.1.8/src/communex/client.py
+-rw-r--r--   0        0        0      297 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/compat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/compat/_util.py
+-rw-r--r--   0        0        0     5290 2024-03-25 19:42:20.678258 communex-0.1.8/src/communex/compat/key.py
+-rw-r--r--   0        0        0     2636 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/compat/storage.py
+-rw-r--r--   0        0        0      386 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/compat/types.py
+-rw-r--r--   0        0        0      262 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/errors.py
+-rw-r--r--   0        0        0     1329 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/key.py
+-rw-r--r--   0        0        0    12756 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/misc.py
+-rw-r--r--   0        0        0      142 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/module/__init__.py
+-rw-r--r--   0        0        0     1533 2024-03-23 14:58:10.559875 communex-0.1.8/src/communex/module/_ip_limiter.py
+-rw-r--r--   0        0        0     2059 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/module/_signer.py
+-rw-r--r--   0        0        0     2712 2024-03-25 14:07:08.730822 communex-0.1.8/src/communex/module/client.py
+-rw-r--r--   0        0        0        0 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/module/example/__init__.py
+-rw-r--r--   0        0        0     1562 2024-03-30 16:16:22.622958 communex-0.1.8/src/communex/module/example/gpt.py
+-rw-r--r--   0        0        0      544 2024-03-23 11:18:25.664457 communex-0.1.8/src/communex/module/example/openai.py
+-rw-r--r--   0        0        0     2086 2024-03-23 11:18:25.664457 communex-0.1.8/src/communex/module/module.py
+-rw-r--r--   0        0        0     7676 2024-03-30 16:23:28.999483 communex-0.1.8/src/communex/module/server.py
+-rw-r--r--   0        0        0      381 2024-03-23 11:18:25.664457 communex-0.1.8/src/communex/module/stuff.md
+-rw-r--r--   0        0        0     2272 2024-03-30 16:12:44.684414 communex-0.1.8/src/communex/types.py
+-rw-r--r--   0        0        0     1333 2024-03-23 11:18:25.664457 communex-0.1.8/src/communex/util.py
+-rw-r--r--   0        0        0     5606 1970-01-01 00:00:00.000000 communex-0.1.8/PKG-INFO
```

### Comparing `communex-0.1.7/LICENSE` & `communex-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/README.md` & `communex-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/pyproject.toml` & `communex-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "communex"
-version = "0.1.7"
+version = "0.1.8"
 description = "A library for Commune network focused on simplicity"
 authors = ["agicommies <info@agicommies.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 comx = "communex.cli:app"
```

### Comparing `communex-0.1.7/src/communex/cli/_common.py` & `communex-0.1.8/src/communex/cli/_common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, Mapping
+from typing import Any, Mapping, Optional
 
 import rich
 import typer
 from rich.console import Console
 from rich.table import Table
 
 
@@ -77,7 +77,19 @@
         table.add_column(key, style="white")
     rows = [*result.values()]
     zipped_rows = [list(column) for column in zip(*rows)]
     for row in zipped_rows:
         table.add_row(*row, style="white")
 
     console.print(table)
+
+def create_use_testnet_getter():
+    use_testnet = False
+    def state_function(testnet: Optional[bool]=None):
+        nonlocal use_testnet
+        if testnet is not None:
+            use_testnet = testnet
+        return use_testnet
+
+    return state_function
+
+get_use_testnet = create_use_testnet_getter()
```

### Comparing `communex-0.1.7/src/communex/cli/balance.py` & `communex-0.1.8/src/communex/cli/balance.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/cli/key.py` & `communex-0.1.8/src/communex/cli/key.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/cli/misc.py` & `communex-0.1.8/src/communex/cli/misc.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/cli/module.py` & `communex-0.1.8/src/communex/cli/module.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/cli/network.py` & `communex-0.1.8/src/communex/cli/network.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/cli/root.py` & `communex-0.1.8/src/communex/cli/root.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,17 +5,24 @@
 
 from .balance import balance_app
 from .key import key_app
 from .misc import misc_app
 from .module import module_app
 from .network import network_app
 from .subnet import subnet_app
+from ._common import get_use_testnet
 
 app = typer.Typer()
 
+balance_app.callback()(get_use_testnet)
+key_app.callback()(get_use_testnet)
+misc_app.callback()(get_use_testnet)
+module_app.callback()(get_use_testnet)
+network_app.callback()(get_use_testnet)
+subnet_app.callback()(get_use_testnet)
 app.add_typer(key_app, name="key", help="Key operations")
 app.add_typer(balance_app, name="balance", help="Balance operations")
 app.add_typer(misc_app, name="misc", help="Other operations")
 app.add_typer(module_app, name="module", help="Module operations")
 app.add_typer(network_app, name="network", help="Network operations")
 app.add_typer(subnet_app, name="subnet", help="Subnet operations")
```

### Comparing `communex-0.1.7/src/communex/cli/subnet.py` & `communex-0.1.8/src/communex/cli/subnet.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/client.py` & `communex-0.1.8/src/communex/client.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/compat/_util.py` & `communex-0.1.8/src/communex/compat/_util.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/compat/key.py` & `communex-0.1.8/src/communex/compat/key.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/compat/storage.py` & `communex-0.1.8/src/communex/compat/storage.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/key.py` & `communex-0.1.8/src/communex/key.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/misc.py` & `communex-0.1.8/src/communex/misc.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/module/_ip_limiter.py` & `communex-0.1.8/src/communex/module/_ip_limiter.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/module/_signer.py` & `communex-0.1.8/src/communex/module/_signer.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/module/client.py` & `communex-0.1.8/src/communex/module/client.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/module/example/gpt.py` & `communex-0.1.8/src/communex/module/example/gpt.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/module/example/openai.py` & `communex-0.1.8/src/communex/module/example/openai.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/module/module.py` & `communex-0.1.8/src/communex/module/module.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/module/server.py` & `communex-0.1.8/src/communex/module/server.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/types.py` & `communex-0.1.8/src/communex/types.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/src/communex/util.py` & `communex-0.1.8/src/communex/util.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.7/PKG-INFO` & `communex-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communex
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for Commune network focused on simplicity
 License: MIT
 Author: agicommies
 Author-email: info@agicommies.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

