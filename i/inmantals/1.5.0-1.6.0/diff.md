# Comparing `tmp/inmantals-1.5.0.tar.gz` & `tmp/inmantals-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmantals-1.5.0.tar", last modified: Thu Dec 21 14:49:46 2023, max compression
+gzip compressed data, was "inmantals-1.6.0.tar", last modified: Thu Apr  4 11:53:04 2024, max compression
```

## Comparing `inmantals-1.5.0.tar` & `inmantals-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-21 14:49:46.586600 inmantals-1.5.0/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    10174 2023-12-21 14:49:27.000000 inmantals-1.5.0/LICENSE
--rw-r--r--   0 jenkins    (988) jenkins    (986)     2471 2023-12-21 14:49:46.586600 inmantals-1.5.0/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1732 2023-12-21 14:49:27.000000 inmantals-1.5.0/README.md
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       73 2023-12-21 14:49:27.000000 inmantals-1.5.0/pyproject.toml
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      525 2023-12-21 14:49:46.587600 inmantals-1.5.0/setup.cfg
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1942 2023-12-21 14:49:38.000000 inmantals-1.5.0/setup.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-21 14:49:46.584600 inmantals-1.5.0/src/
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-21 14:49:46.585600 inmantals-1.5.0/src/inmantals/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      627 2023-12-21 14:49:27.000000 inmantals-1.5.0/src/inmantals/__init__.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     9787 2023-12-21 14:49:27.000000 inmantals-1.5.0/src/inmantals/jsonrpc.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     4649 2023-12-21 14:49:36.000000 inmantals-1.5.0/src/inmantals/lsp_types.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1283 2023-12-21 14:49:27.000000 inmantals-1.5.0/src/inmantals/pipeserver.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    36489 2023-12-21 14:49:36.000000 inmantals-1.5.0/src/inmantals/server.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1178 2023-12-21 14:49:27.000000 inmantals-1.5.0/src/inmantals/tcpserver.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-21 14:49:46.586600 inmantals-1.5.0/src/inmantals.egg-info/
--rw-r--r--   0 jenkins    (988) jenkins    (986)     2471 2023-12-21 14:49:46.000000 inmantals-1.5.0/src/inmantals.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      452 2023-12-21 14:49:46.000000 inmantals-1.5.0/src/inmantals.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)        1 2023-12-21 14:49:46.000000 inmantals-1.5.0/src/inmantals.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       73 2023-12-21 14:49:46.000000 inmantals-1.5.0/src/inmantals.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       26 2023-12-21 14:49:46.000000 inmantals-1.5.0/src/inmantals.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       10 2023-12-21 14:49:46.000000 inmantals-1.5.0/src/inmantals.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2023-12-21 14:49:46.586600 inmantals-1.5.0/tests/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    18396 2023-12-21 14:49:36.000000 inmantals-1.5.0/tests/test_smoke.py
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2024-04-04 11:53:04.596393 inmantals-1.6.0/
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)    10174 2024-04-04 11:52:26.000000 inmantals-1.6.0/LICENSE
+-rw-r--r--   0 jenkins    (987) jenkins    (985)     2471 2024-04-04 11:53:04.596393 inmantals-1.6.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)     1732 2024-04-04 11:52:26.000000 inmantals-1.6.0/README.md
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)       73 2024-04-04 11:52:26.000000 inmantals-1.6.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)      525 2024-04-04 11:53:04.597393 inmantals-1.6.0/setup.cfg
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)     1942 2024-04-04 11:52:39.000000 inmantals-1.6.0/setup.py
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2024-04-04 11:53:04.594393 inmantals-1.6.0/src/
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2024-04-04 11:53:04.595393 inmantals-1.6.0/src/inmantals/
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)      627 2024-04-04 11:52:26.000000 inmantals-1.6.0/src/inmantals/__init__.py
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)     9788 2024-04-04 11:52:36.000000 inmantals-1.6.0/src/inmantals/jsonrpc.py
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)     4650 2024-04-04 11:52:36.000000 inmantals-1.6.0/src/inmantals/lsp_types.py
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)     1283 2024-04-04 11:52:26.000000 inmantals-1.6.0/src/inmantals/pipeserver.py
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)    36710 2024-04-04 11:52:36.000000 inmantals-1.6.0/src/inmantals/server.py
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)     1178 2024-04-04 11:52:26.000000 inmantals-1.6.0/src/inmantals/tcpserver.py
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2024-04-04 11:53:04.596393 inmantals-1.6.0/src/inmantals.egg-info/
+-rw-r--r--   0 jenkins    (987) jenkins    (985)     2471 2024-04-04 11:53:04.000000 inmantals-1.6.0/src/inmantals.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)      452 2024-04-04 11:53:04.000000 inmantals-1.6.0/src/inmantals.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)        1 2024-04-04 11:53:04.000000 inmantals-1.6.0/src/inmantals.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)       73 2024-04-04 11:53:04.000000 inmantals-1.6.0/src/inmantals.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)       26 2024-04-04 11:53:04.000000 inmantals-1.6.0/src/inmantals.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)       10 2024-04-04 11:53:04.000000 inmantals-1.6.0/src/inmantals.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (987) jenkins    (985)        0 2024-04-04 11:53:04.596393 inmantals-1.6.0/tests/
+-rw-rw-r--   0 jenkins    (987) jenkins    (985)    19366 2024-04-04 11:52:36.000000 inmantals-1.6.0/tests/test_smoke.py
```

### Comparing `inmantals-1.5.0/LICENSE` & `inmantals-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inmantals-1.5.0/PKG-INFO` & `inmantals-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmantals
-Version: 1.5.0
+Version: 1.6.0
 Summary: Inmanta Language Server
 Home-page: https://github.com/inmanta/vscode-inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License
 Keywords: ide,language-server,vscode,inmanta
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inmantals-1.5.0/README.md` & `inmantals-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `inmantals-1.5.0/setup.cfg` & `inmantals-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `inmantals-1.5.0/setup.py` & `inmantals-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     long_description = f.read()
 
 setup(
     name="inmantals",
     package_dir={"": "src"},
     packages=find_packages("src"),
     install_requires=requires,
-    version="1.5.0",
+    version="1.6.0",
     description="Inmanta Language Server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Inmanta",
     author_email="code@inmanta.com",
     license="Apache Software License",
     url="https://github.com/inmanta/vscode-inmanta",
```

### Comparing `inmantals-1.5.0/src/inmantals/__init__.py` & `inmantals-1.6.0/src/inmantals/__init__.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.5.0/src/inmantals/jsonrpc.py` & `inmantals-1.6.0/src/inmantals/jsonrpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
+
 import asyncio
 import json
 import logging
 import os
 import sys
 from enum import Enum
 from json.decoder import JSONDecodeError
```

### Comparing `inmantals-1.5.0/src/inmantals/lsp_types.py` & `inmantals-1.6.0/src/inmantals/lsp_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
+
 import pkg_resources
 from packaging import version
 from pydantic import FileUrl
 
 PYDANTIC_V2_INSTALLED: bool = version.Version(pkg_resources.get_distribution("pydantic").version) >= version.Version(
     "2.0.0.dev"
 )
```

### Comparing `inmantals-1.5.0/src/inmantals/pipeserver.py` & `inmantals-1.6.0/src/inmantals/pipeserver.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.5.0/src/inmantals/server.py` & `inmantals-1.6.0/src/inmantals/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
+
 import asyncio
 import contextlib
 import json
 import logging
 import os
 import re
 import tempfile
@@ -37,16 +38,17 @@
 import yaml
 from inmanta import compiler, env, module, resources
 from inmanta.agent import handler
 from inmanta.ast import CompilerException, Location, Range
 from inmanta.ast.entity import Entity, Implementation
 from inmanta.config import is_bool
 from inmanta.execute import scheduler
+from inmanta.export import Exporter
 from inmanta.module import Project
-from inmanta.plugins import Plugin
+from inmanta.plugins import Plugin, PluginMeta
 from inmanta.util import groupby
 from inmantals import lsp_types
 from inmantals.jsonrpc import InvalidParamsException, JsonRpcHandler, MethodNotFoundException
 from intervaltree.interval import Interval
 from intervaltree.intervaltree import IntervalTree
 from packaging import version
 
@@ -475,14 +477,17 @@
                         module.Project.set(module.Project(folder.inmanta_project_dir))
                 else:
                     folder.install_project(attach_cf_cache=useCache)
 
             # reset all
             resources.resource.reset()
             handler.Commander.reset()
+            PluginMeta.clear()
+            if hasattr(Exporter, "clear"):  # Remain backwards-compatible with older version of inmanta-core
+                Exporter.clear()
 
             setup_project(self.root_folder)
 
             # can't call compiler.anchormap and compiler.get_types_and_scopes directly because of inmanta/inmanta#2471
 
             compiler_instance: compiler.Compiler = compiler.Compiler()
             (statements, blocks) = compiler_instance.compile()
@@ -563,15 +568,14 @@
                 )
             await self.publish_diagnostics(params)
             await self.handle_module_loading_exception(e)
             logger.exception("Compilation failed")
         except InvalidExtensionSetup as e:
             await self.handle_invalid_extension_setup(e)
             logger.error(e)
-
         except Exception as e:
             logger.debug(e)
 
             await self.publish_diagnostics(None)
             logger.exception("Compilation failed")
 
     async def handle_invalid_extension_setup(self, e: InvalidExtensionSetup):
```

### Comparing `inmantals-1.5.0/src/inmantals/tcpserver.py` & `inmantals-1.6.0/src/inmantals/tcpserver.py`

 * *Files identical despite different names*

### Comparing `inmantals-1.5.0/src/inmantals.egg-info/PKG-INFO` & `inmantals-1.6.0/src/inmantals.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmantals
-Version: 1.5.0
+Version: 1.6.0
 Summary: Inmanta Language Server
 Home-page: https://github.com/inmanta/vscode-inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License
 Keywords: ide,language-server,vscode,inmanta
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inmantals-1.5.0/tests/test_smoke.py` & `inmantals-1.6.0/tests/test_smoke.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,21 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
+
 import json
 import logging
 import os
 import shutil
 import socket
+import time
 from typing import AsyncIterator, Dict, List, Optional
 
 import pytest
 from tornado.iostream import IOStream
 from tornado.tcpclient import TCPClient
 
 from inmanta import env
@@ -312,36 +314,44 @@
     ret = await client.call("textDocument/didSave")
     result = await client.assert_one(ret)
     # find DEBUG inmanta.execute.scheduler:scheduler.py:196 Anchormap took 0.006730 seconds
     assert "Anchormap took" in caplog.text
     caplog.clear()
 
 
-@pytest.mark.timeout(10)
+@pytest.mark.timeout(15)
 @pytest.mark.asyncio
 async def test_working_on_v2_modules(client, caplog):
     """
     Simulate opening a v2 module in vscode. This test makes sure the module is installed in editable mode.
     """
+    start_time = time.time()
+
     if CORE_VERSION < version.Version("5"):
         pytest.skip("Feature not supported below iso5")
 
     caplog.set_level(logging.DEBUG)
 
     module_name = "module-v2"
     path_to_module = os.path.join(os.path.dirname(__file__), "modules", module_name)
 
     env_path = os.path.join(path_to_module, ".env")
     if os.path.isdir(env_path):
         shutil.rmtree(env_path)
         os.makedirs(env_path)
 
+    logging.info(f"Setup completed in {time.time() - start_time:.2f} seconds")
+    part_time = time.time()
+
     venv = env.VirtualEnv(env_path)
     venv.use_virtual_env()
 
+    logging.info(f"VirtualEnv setup completed in {time.time() - part_time:.2f} seconds")
+    part_time = time.time()
+
     assert "inmanta-module-module-v2" not in env.PythonWorkingSet.get_packages_in_working_set()
 
     if CORE_VERSION < version.Version("11.0.0"):
         options = {
             "repos": [
                 {"url": "https://pypi.org/simple", "type": "package"},
             ]
@@ -353,14 +363,18 @@
     ret = await client.call(
         "initialize",
         workspaceFolders=[path_uri],
         rootUri=f"file://{path_to_module}",
         capabilities={},
         initializationOptions=options,
     )
+
+    logging.info(f"Initialization 1 completed in {time.time() - part_time:.2f} seconds")
+    part_time = time.time()
+
     result = await client.assert_one(ret)
     assert result == {
         "capabilities": {
             "textDocumentSync": {
                 "openClose": True,
                 "change": 1,
                 "willSave": False,
@@ -369,25 +383,39 @@
             },
             "hoverProvider": True,
             "definitionProvider": True,
             "referencesProvider": True,
             "workspaceSymbolProvider": {"workDoneProgress": False},
         }
     }
+    logging.info(f"Initialization assert 1 completed in {time.time() - part_time:.2f} seconds")
+    part_time = time.time()
 
     ret = await client.call("initialized")
+
+    logging.info(f"Initialization 2 completed in {time.time() - part_time:.2f} seconds")
+    part_time = time.time()
     result = await client.assert_one(ret)
-    assert "inmanta-module-module-v2" in env.PythonWorkingSet.get_packages_in_working_set()
+    logging.info(f"Initialization assert 2 completed in {time.time() - part_time:.2f} seconds")
+    part_time = time.time()
 
+    assert "inmanta-module-module-v2" in env.PythonWorkingSet.get_packages_in_working_set()
     # find DEBUG inmanta.execute.scheduler:scheduler.py:196 Anchormap took 0.006730 seconds
     assert "Anchormap took" in caplog.text
+
+    logging.info(f"Module assertion completed in {time.time() - part_time:.2f} seconds")
+    part_time = time.time()
     caplog.clear()
 
     ret = await client.call("textDocument/didSave")
     result = await client.assert_one(ret)
+
+    logging.info(f"saved in {time.time() - part_time:.2f} seconds")
+    part_time = time.time()
+
     # find DEBUG inmanta.execute.scheduler:scheduler.py:196 Anchormap took 0.006730 seconds
     assert "Anchormap took" in caplog.text
     caplog.clear()
 
 
 @pytest.mark.skipif(
     lsp_types.PYDANTIC_V2_INSTALLED,
```

