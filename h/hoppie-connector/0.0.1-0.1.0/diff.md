# Comparing `tmp/hoppie-connector-0.0.1.tar.gz` & `tmp/hoppie-connector-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppie-connector-0.0.1.tar", last modified: Sun Mar 10 21:58:31 2024, max compression
+gzip compressed data, was "hoppie-connector-0.1.0.tar", last modified: Wed Apr  3 23:09:37 2024, max compression
```

## Comparing `hoppie-connector-0.0.1.tar` & `hoppie-connector-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:58:31.535204 hoppie-connector-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:58:31.531204 hoppie-connector-0.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (127)       70 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/.devcontainer/postCreate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:58:31.531204 hoppie-connector-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:58:31.531204 hoppie-connector-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/.github/workflows/unit-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-10 21:58:31.535204 hoppie-connector-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 21:58:31.535204 hoppie-connector-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:58:31.527204 hoppie-connector-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:58:31.531204 hoppie-connector-0.0.1/src/hoppie_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/src/hoppie_connector/API.py
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/src/hoppie_connector/Messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/src/hoppie_connector/Responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/src/hoppie_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:58:31.531204 hoppie-connector-0.0.1/src/hoppie_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-10 21:58:31.000000 hoppie-connector-0.0.1/src/hoppie_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-10 21:58:31.000000 hoppie-connector-0.0.1/src/hoppie_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 21:58:31.000000 hoppie-connector-0.0.1/src/hoppie_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-10 21:58:31.000000 hoppie-connector-0.0.1/src/hoppie_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-10 21:58:31.000000 hoppie-connector-0.0.1/src/hoppie_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:58:31.531204 hoppie-connector-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/tests/test_AdscMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/tests/test_HoppieMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/tests/test_HoppieResponseParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/tests/test_PeekMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/tests/test_PollMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/tests/test_ProgressMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-10 21:58:26.000000 hoppie-connector-0.0.1/tests/test_TelexMessage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:09:37.376239 hoppie-connector-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:09:37.368239 hoppie-connector-0.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:09:37.368239 hoppie-connector-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:09:37.368239 hoppie-connector-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/.github/workflows/unit-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-03 23:09:37.376239 hoppie-connector-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:09:37.376239 hoppie-connector-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:09:37.368239 hoppie-connector-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:09:37.372239 hoppie-connector-0.1.0/src/hoppie_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/src/hoppie_connector/API.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19693 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/src/hoppie_connector/Messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/src/hoppie_connector/Responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/src/hoppie_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:09:37.376239 hoppie-connector-0.1.0/src/hoppie_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-03 23:09:37.000000 hoppie-connector-0.1.0/src/hoppie_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-03 23:09:37.000000 hoppie-connector-0.1.0/src/hoppie_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:09:37.000000 hoppie-connector-0.1.0/src/hoppie_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 23:09:37.000000 hoppie-connector-0.1.0/src/hoppie_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 23:09:37.000000 hoppie-connector-0.1.0/src/hoppie_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:09:37.376239 hoppie-connector-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_AdscMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_ErrorResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_HoppieAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_HoppieConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_HoppieMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11940 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_HoppieMessageFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_HoppieResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_HoppieResponseParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_HoppieResponseParserFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PeekMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PeekResponseParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PeekSuccessResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PingMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PingResponseParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PingSuccessResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PollMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PollResponseParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_PollSuccessResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_ProgressMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_SuccessResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-03 23:09:31.000000 hoppie-connector-0.1.0/tests/test_TelexMessage.py
```

### Comparing `hoppie-connector-0.0.1/.devcontainer/devcontainer.json` & `hoppie-connector-0.1.0/.devcontainer/devcontainer.json`

 * *Files 18% similar despite different names*

```diff
@@ -9,34 +9,29 @@
 	// Features to add to the dev container. More info: https://containers.dev/features.
 	// "features": {},
 	
 	// Use 'forwardPorts' to make a list of ports inside the container available locally.
 	// "forwardPorts": [],
 
 	// Use 'postCreateCommand' to run commands after the container is created.
-	"postCreateCommand": "./.devcontainer/postCreate.sh",
+	"postCreateCommand": "pip3 install --user --editable .[Test]",
 	
 	// Configure tool-specific properties.
 	"customizations": {
 		"vscode": {
 			"extensions": [
 				"charliermarsh.ruff",
+				"github.vscode-github-actions",
 				"njpwerner.autodocstring",
+				"ryanluker.vscode-coverage-gutters",
 				"tamasfe.even-better-toml"
 			],
 			"settings": {
-				"python.testing.unittestArgs": [
-					"-v",
-					"-s",
-					"./tests",
-					"-p",
-					"test_*.py"
-				],
-				"python.testing.pytestEnabled": false,
-				"python.testing.unittestEnabled": true
+				"python.testing.unittestEnabled": false,
+				"python.testing.pytestEnabled": true
 			}
 		}
 	}
 
 	// Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
 	// "remoteUser": "root"
 }
```

### Comparing `hoppie-connector-0.0.1/.github/dependabot.yml` & `hoppie-connector-0.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `hoppie-connector-0.0.1/.github/workflows/publish-pypi.yml` & `hoppie-connector-0.1.0/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `hoppie-connector-0.0.1/.gitignore` & `hoppie-connector-0.1.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -156,8 +156,11 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # Ruff
-.ruff_cache
+.ruff_cache
+
+# Local settings
+.vscode/
```

### Comparing `hoppie-connector-0.0.1/LICENSE` & `hoppie-connector-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppie-connector-0.0.1/PKG-INFO` & `hoppie-connector-0.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: hoppie-connector
-Version: 0.0.1
-Summary: Python connector for Hoppie's ACARS service 
-Author: islandc_
-License: MIT License
-Project-URL: Repository, https://github.com/islandcontroller/hoppie_connector.git
-Project-URL: Issues, https://github.com/islandcontroller/hoppie_connector/issues
-Project-URL: Documentation, https://github.com/islandcontroller/hoppie_connector/wiki
-Keywords: hoppie,acars,vatsim
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Communications
-Classifier: Topic :: Games/Entertainment :: Simulation
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# hoppie-connector
-
-[![License](https://img.shields.io/github/license/islandcontroller/armcm-devcontainer)](LICENSE) ![PyPI - Version](https://img.shields.io/pypi/v/hoppie-connector)
-
-
-*A Python connector for Hoppie's ACARS service.*
-
-## Installation
-
-Install the module using pip:
-
-    pip install hoppie-connector
-
-Import it in your python script:
-
-```python
-from hoppie_connector import HoppieConnector, HoppieError
-
-cnx = HoppieConnector('<your callsign>', '<your logon code>')
-
-try:
-    # Send telex message
-    cnx.send_telex('<other callsign>', '<message>')
-
-    # Print messages for me
-    messages = cnx.peek()
-    for m_id, msg in messages: 
-        print(msg)
-except HoppieError as e:
-    print(e)
-```
+[build-system]
+requires = [
+    "setuptools>=61.0",
+    "setuptools-scm>=8.0"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "hoppie-connector"
+authors = [
+    {name = "islandc_"},
+]
+description = "Python connector for Hoppie's ACARS service "
+readme = "README.md"
+requires-python = ">=3.12"
+keywords = ["hoppie", "acars", "vatsim"]
+license = {text = "MIT License"}
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Communications",
+    "Topic :: Games/Entertainment :: Simulation",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+dependencies = [
+    "requests>=2.31.0"
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+Test = [
+    "pytest>=8.1",
+    "pytest-cov>=4.1",
+    "responses>=0.25",
+    "ruff>=0.3"
+]
+
+[project.urls]
+Homepage = "https://islandcontroller.github.io/hoppie-connector/"
+Repository = "https://github.com/islandcontroller/hoppie-connector.git"
+Issues = "https://github.com/islandcontroller/hoppie-connector/issues/"
+Documentation = "https://github.com/islandcontroller/hoppie-connector/wiki/"
+
+[tool.setuptools_scm]
+
+[tool.pytest.ini_options]
+addopts = "--cov=hoppie_connector --cov-report=xml --cov-fail-under=100"
+testpaths = ["tests"]
+
+[tool.ruff]
+extend-exclude = ["tests"]
```

### Comparing `hoppie-connector-0.0.1/src/hoppie_connector/API.py` & `hoppie-connector-0.1.0/src/hoppie_connector/API.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,54 @@
 from .Messages import HoppieMessage
-from .Responses import HoppieResponse, HoppieResponseParser
+from .Responses import HoppieResponse, HoppieResponseParserFactory
+from datetime import timedelta
 import requests
 
 class HoppieAPI(object):
-    def __init__(self, logon: str, url: str = 'http://www.hoppie.nl/acars/system/connect.html'):
-        self._url = url
+    """HoppieAPI(logon[, url])
+    
+    Hoppie API connection
+    """
+    _DEFAULT_URL: str = 'https://www.hoppie.nl/acars/system/connect.html'
+
+    def __init__(self, logon: str, url: str | None = None):
+        """Prepare new API connection
+
+        Args:
+            logon (str): Logon code
+            url (str, optional): API URL. Defaults to None.
+        """
+        self._url = url if url is not None else self._DEFAULT_URL
         self._logon = logon
 
-    def connect(self, msg: HoppieMessage) -> HoppieResponse:
-        params = { 'logon': self._logon }
-        params.update(msg.get_msg_params())
+    def connect(self, msg: HoppieMessage) -> tuple[HoppieResponse, timedelta]:
+        """Issue "connect" call to the API
+
+        Args:
+            msg (HoppieMessage): Message data
+
+        Returns:
+            tuple[HoppieResponse, timedelta]: Response data (ASCII string encoding) and delay
+        """
+        if not isinstance(msg, HoppieMessage):
+            raise ValueError('Invalid input message data type')
 
-        req = requests.get(self._url, params)
-        if not req.ok: raise ConnectionError(f"Error {req.status_code}: {req.reason}")
+        match msg.get_msg_type():
+            case HoppieMessage.MessageType.TELEX:
+                params = msg.get_msg_params()
+                data = params.pop('packet')
+                response = requests.post(self._url, params={'logon': self._logon, **params}, data={'packet': data})
+            case _:
+                response = requests.get(self._url, params={'logon': self._logon, **msg.get_msg_params()})
+        
+        if not response.ok: 
+            raise ConnectionError(f"Error {response.status_code}: {response.reason}")
+        
+        parser = HoppieResponseParserFactory().create_parser(msg.get_msg_type())
+        content = response.content.decode('ascii')
+        return (parser.parse(content), response.elapsed)
 
-        response = req.content.decode('ascii')
-        return HoppieResponseParser().parse(response)
+    def __repr__(self) -> str:
+        return f"HoppieAPI(logon={self._logon!r}, url={self._url!r})"
+    
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, HoppieAPI) and (self._logon == __value._logon) and (self._url == __value._url)
```

### Comparing `hoppie-connector-0.0.1/tests/test_HoppieMessage.py` & `hoppie-connector-0.1.0/tests/test_PingMessage.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-from hoppie_connector.Messages import HoppieMessage
+from hoppie_connector.Messages import HoppieMessage, PingMessage
 import unittest
 
-class TestValidHoppieMessage(unittest.TestCase):
-    _EXPECTED_FROM: str = 'CALLSIGN'
-    _EXPECTED_TO: str = 'OPS'
-    _EXPECTED_TYPE: HoppieMessage.MessageType = HoppieMessage.MessageType.TELEX
+class TestValidPingMessage(unittest.TestCase):
+    _EXPECTED_TO: str = 'SERVER'
+    _EXPECTED_TYPE: HoppieMessage.MessageType = HoppieMessage.MessageType.PING
+    _EXPECTED_STATIONS: list[str] = []
     _EXPECTED_PACKET: str = ''
-    _EXPECTED_MSG_PARAM: dict = {
-        'from': _EXPECTED_FROM,
-        'to': _EXPECTED_TO,
-        'type': _EXPECTED_TYPE.value,
-        'packet': _EXPECTED_PACKET
-    }
 
     def setUp(self) -> None:
         super().setUp()
-        self._UUT = HoppieMessage(self._EXPECTED_FROM, self._EXPECTED_TO, self._EXPECTED_TYPE)
+        self._UUT = PingMessage('STATION')
 
-    def test_get_from_name(self):      self.assertEqual(self._EXPECTED_FROM,      self._UUT.get_from_name())
-    def test_get_to_name(self):        self.assertEqual(self._EXPECTED_TO,        self._UUT.get_to_name())
-    def test_get_msg_type(self):       self.assertEqual(self._EXPECTED_TYPE,      self._UUT.get_msg_type())
-    def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET,    self._UUT.get_packet_content())
-    def test_get_msg_params(self):     self.assertEqual(self._EXPECTED_MSG_PARAM, self._UUT.get_msg_params())
+    def test_get_to_name(self):        self.assertEqual(self._EXPECTED_TO,       self._UUT.get_to_name())
+    def test_get_msg_type(self):       self.assertEqual(self._EXPECTED_TYPE,     self._UUT.get_msg_type())
+    def test_get_stations(self):       self.assertEqual(self._EXPECTED_STATIONS, self._UUT.get_stations())
+    def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET,   self._UUT.get_packet_content())
 
-class TestHoppieMessageInputValidation(unittest.TestCase):
-    def test_empty_from_name(self):   self.assertRaises(ValueError, lambda: HoppieMessage('',          'OPS',       HoppieMessage.MessageType.TELEX))
-    def test_empty_to_name(self):     self.assertRaises(ValueError, lambda: HoppieMessage('CALLSIGN',  '',          HoppieMessage.MessageType.TELEX))
-    def test_from_too_long(self):     self.assertRaises(ValueError, lambda: HoppieMessage('123456789', 'OPS',       HoppieMessage.MessageType.TELEX))
-    def test_to_too_long(self):       self.assertRaises(ValueError, lambda: HoppieMessage('CALLSIGN',  '123456789', HoppieMessage.MessageType.TELEX))
-    def test_invalid_from_char(self): self.assertRaises(ValueError, lambda: HoppieMessage('D-ABCD',    'OPS',       HoppieMessage.MessageType.TELEX))
-    def test_invalid_to_char(self):   self.assertRaises(ValueError, lambda: HoppieMessage('CALLSIGN',  'ops',       HoppieMessage.MessageType.TELEX))
-    def test_invalid_type(self):      self.assertRaises(ValueError, lambda: HoppieMessage('CALLSIGN',  'OPS',       0))
-    def test_special_from_all(self):  self.assertIsInstance(HoppieMessage('ALL-CALLSIGNS', 'OPS', HoppieMessage.MessageType.TELEX), HoppieMessage)
-    def test_special_to_all(self):    self.assertIsInstance(HoppieMessage('OPS', 'ALL-CALLSIGNS', HoppieMessage.MessageType.TELEX), HoppieMessage)
+class TestPingMessageInputValidation(unittest.TestCase):
+    def test_invalid_station(self):         self.assertRaises(ValueError, lambda: PingMessage('STATION', '123456789'))
+    def test_invalid_station_in_list(self): self.assertRaises(ValueError, lambda: PingMessage('STATION', ['CALLSIGN', '123456789']))
+    def test_too_many_stations(self):       self.assertRaises(ValueError, lambda: PingMessage('STATION', 25 * ['CALLSIGN']))
+    def test_special_all_stations(self):
+        expected = ['ALL-CALLSIGNS']
+        acutal = PingMessage('STATION', '*')
+        self.assertEqual(expected, acutal.get_stations())
+
+class TestPingMessageRepresentation(unittest.TestCase):
+    def test_repr(self):
+        expected = PingMessage('STATION')
+        actual = eval(repr(expected))
+        self.assertEqual(expected, actual)
```

### Comparing `hoppie-connector-0.0.1/tests/test_PollMessage.py` & `hoppie-connector-0.1.0/tests/test_PeekMessage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-from hoppie_connector.Messages import HoppieMessage, PollMessage
+from hoppie_connector.Messages import HoppieMessage, PeekMessage
 import unittest
 
-class TestValidPollMessage(unittest.TestCase):
+class TestValidPeekMessage(unittest.TestCase):
     _EXPECTED_TO: str = 'SERVER'
-    _EXPECTED_TYPE: HoppieMessage.MessageType = HoppieMessage.MessageType.POLL
+    _EXPECTED_TYPE: HoppieMessage.MessageType = HoppieMessage.MessageType.PEEK
     _EXPECTED_PACKET: str = ''
 
     def setUp(self) -> None:
         super().setUp()
-        self._UUT = PollMessage('OPS')
+        self._UUT = PeekMessage('OPS')
 
     def test_get_to_name(self):  self.assertEqual(self._EXPECTED_TO,   self._UUT.get_to_name())
     def test_get_msg_type(self): self.assertEqual(self._EXPECTED_TYPE, self._UUT.get_msg_type())
+
+class TestPeekMessageRepresentation(unittest.TestCase):
+    def test_repr(self):
+        expected = PeekMessage('OPS')
+        actual = eval(repr(expected))
+        self.assertEqual(expected, actual)
```

### Comparing `hoppie-connector-0.0.1/tests/test_ProgressMessage.py` & `hoppie-connector-0.1.0/tests/test_ProgressMessage.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from hoppie_connector.Messages import HoppieMessage, ProgressMessage
-import datetime
+from datetime import time, timedelta, timezone, UTC
 import unittest
 
 class TestValidProgressMessage(unittest.TestCase):
     _EXPECTED_TYPE: HoppieMessage.MessageType = HoppieMessage.MessageType.PROGRESS
     _EXPECTED_DEP: str = 'EDDF'
     _EXPECTED_ARR: str = 'EDDH'
-    _EXPECTED_OUT: datetime = datetime.datetime(year=2000, month=1, day=1, hour=18, minute=20, second=0, tzinfo=datetime.UTC)
+    _EXPECTED_OUT: time = time(hour=18, minute=20, tzinfo=UTC)
     _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1820'
 
     def setUp(self) -> None:
         super().setUp()
         self._UUT = ProgressMessage('CALLSIGN', 'OPS', self._EXPECTED_DEP, self._EXPECTED_ARR, self._EXPECTED_OUT)
 
     def test_get_msg_type(self):       self.assertEqual(self._EXPECTED_TYPE, self._UUT.get_msg_type())
@@ -19,84 +19,138 @@
     def test_get_time_out(self):       self.assertEqual(self._EXPECTED_OUT, self._UUT.get_time_out())
     def test_get_time_off(self):       self.assertIsNone(self._UUT.get_time_off())
     def test_get_time_on(self):        self.assertIsNone(self._UUT.get_time_on())
     def test_get_time_in(self):        self.assertIsNone(self._UUT.get_time_in())
     def test_get_eta(self):            self.assertIsNone(self._UUT.get_eta())
     def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
 
+class TestValidProgressMessageTimezone(unittest.TestCase):
+    _TIMEZONE = timezone = timezone(timedelta(hours=1))
+    _EXPECTED_OUT: time = time(hour=18, minute=20, tzinfo=_TIMEZONE)
+    _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1720'
+
+    def setUp(self) -> None:
+        super().setUp()
+        self._UUT = ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._EXPECTED_OUT)
+
+    def test_get_time_out(self):       self.assertEqual(self._EXPECTED_OUT, self._UUT.get_time_out())
+    def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
+
+class TestValidProgressMessageNoTimezone(unittest.TestCase):
+    _EXPECTED_OUT: time = time(hour=18, minute=20, tzinfo=None)
+    _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1820'
+
+    def setUp(self) -> None:
+        super().setUp()
+        self._UUT = ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._EXPECTED_OUT)
+
+    def test_get_time_out(self):       self.assertEqual(self._EXPECTED_OUT, self._UUT.get_time_out())
+    def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
+
 class TestValidProgressMessageEta(unittest.TestCase):
-    _EXPECTED_OUT: datetime = datetime.datetime(year=2000, month=1, day=1, hour=18, minute=20, second=0, tzinfo=datetime.UTC)
-    _EXPECTED_ETA: datetime = _EXPECTED_OUT + datetime.timedelta(minutes=5)
+    _EXPECTED_OUT: time = time(hour=18, minute=20, tzinfo=UTC)
+    _EXPECTED_ETA: time = time(hour=18, minute=25, tzinfo=UTC)
     _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1820 ETA/1825'
 
     def setUp(self) -> None:
         super().setUp()
         self._UUT = ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._EXPECTED_OUT, self._EXPECTED_ETA)
 
     def test_get_eta(self):            self.assertEqual(self._EXPECTED_ETA, self._UUT.get_eta())
     def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
 
 class TestValidProgressMessageOff(unittest.TestCase):
-    _EXPECTED_OUT: datetime = datetime.datetime(year=2000, month=1, day=1, hour=18, minute=20, second=0, tzinfo=datetime.UTC)
-    _EXPECTED_OFF: datetime = _EXPECTED_OUT + datetime.timedelta(minutes=5)
+    _EXPECTED_OUT: time = time(hour=18, minute=20, tzinfo=UTC)
+    _EXPECTED_OFF: time = time(hour=18, minute=25, tzinfo=UTC)
     _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1820 OFF/1825'
 
     def setUp(self) -> None:
         super().setUp()
         self._UUT = ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._EXPECTED_OUT, time_off=self._EXPECTED_OFF)
 
     def test_get_time_off(self):       self.assertEqual(self._EXPECTED_OFF, self._UUT.get_time_off())
     def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
 
 class TestValidProgressMessageOffEta(unittest.TestCase):
-    _EXPECTED_OUT: datetime = datetime.datetime(year=2000, month=1, day=1, hour=18, minute=20, second=0, tzinfo=datetime.UTC)
-    _EXPECTED_OFF: datetime = _EXPECTED_OUT + datetime.timedelta(minutes=5)
-    _EXPECTED_ETA: datetime = _EXPECTED_OFF + datetime.timedelta(minutes=5)
+    _EXPECTED_OUT: time = time(hour=18, minute=20, second=0, tzinfo=UTC)
+    _EXPECTED_OFF: time = time(hour=18, minute=25, tzinfo=UTC)
+    _EXPECTED_ETA: time = time(hour=18, minute=30, tzinfo=UTC)
     _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1820 OFF/1825 ETA/1830'
 
     def setUp(self) -> None:
         super().setUp()
         self._UUT = ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._EXPECTED_OUT, self._EXPECTED_ETA, self._EXPECTED_OFF)
 
     def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
 
 class TestValidProgressMessageOn(unittest.TestCase):
-    _EXPECTED_OUT: datetime = datetime.datetime(year=2000, month=1, day=1, hour=18, minute=20, second=0, tzinfo=datetime.UTC)
-    _EXPECTED_OFF: datetime = _EXPECTED_OUT + datetime.timedelta(minutes=5)
-    _EXPECTED_ON: datetime = _EXPECTED_OFF + datetime.timedelta(minutes=5)
+    _EXPECTED_OUT: time = time(hour=18, minute=20, second=0, tzinfo=UTC)
+    _EXPECTED_OFF: time = time(hour=18, minute=25, tzinfo=UTC)
+    _EXPECTED_ON: time = time(hour=18, minute=30, tzinfo=UTC)
     _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1820 OFF/1825 ON/1830'
 
     def setUp(self) -> None:
         super().setUp()
         self._UUT = ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._EXPECTED_OUT, time_off=self._EXPECTED_OFF, time_on=self._EXPECTED_ON)
 
     def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
 
+class TestValidProgressMessageOnEta(unittest.TestCase):
+    _EXPECTED_OUT: time = time(hour=18, minute=20, second=0, tzinfo=UTC)
+    _EXPECTED_OFF: time = time(hour=18, minute=25, tzinfo=UTC)
+    _EXPECTED_ON: time = time(hour=18, minute=30, tzinfo=UTC)
+    _EXPECTED_ETA: time = time(hour=18, minute=35, tzinfo=UTC)
+    _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1820 OFF/1825 ON/1830 ETA/1835'
+
+    def setUp(self) -> None:
+        super().setUp()
+        self._UUT = ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._EXPECTED_OUT, self._EXPECTED_ETA, self._EXPECTED_OFF, self._EXPECTED_ON)
+
+    def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
+
 class TestValidProgressMessageIn(unittest.TestCase):
-    _EXPECTED_OUT: datetime = datetime.datetime(year=2000, month=1, day=1, hour=18, minute=20, second=0, tzinfo=datetime.UTC)
-    _EXPECTED_OFF: datetime = _EXPECTED_OUT + datetime.timedelta(minutes=5)
-    _EXPECTED_ON: datetime = _EXPECTED_OFF + datetime.timedelta(minutes=5)
-    _EXPECTED_IN: datetime = _EXPECTED_ON + datetime.timedelta(minutes=5)
+    _EXPECTED_OUT: time = time(hour=18, minute=20, second=0, tzinfo=UTC)
+    _EXPECTED_OFF: time = time(hour=18, minute=25, tzinfo=UTC)
+    _EXPECTED_ON: time = time(hour=18, minute=30, tzinfo=UTC)
+    _EXPECTED_IN: time = time(hour=18, minute=35, tzinfo=UTC)
     _EXPECTED_PACKET: str = 'EDDF/EDDH OUT/1820 OFF/1825 ON/1830 IN/1835'
 
     def setUp(self) -> None:
         super().setUp()
         self._UUT = ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._EXPECTED_OUT, time_off=self._EXPECTED_OFF, time_on=self._EXPECTED_ON, time_in=self._EXPECTED_IN)
 
     def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET, self._UUT.get_packet_content())
 
 class TestProgressMessageInputValidation(unittest.TestCase):
-    _TIME_1: datetime = datetime.datetime(year=2000, month=1, day=1, hour=18, minute=20, second=0, tzinfo=datetime.UTC)
-    _TIME_2: datetime = _TIME_1 + datetime.timedelta(minutes=5)
-    _TIME_3: datetime = _TIME_2 + datetime.timedelta(minutes=5)
-    _TIME_4: datetime = _TIME_3 + datetime.timedelta(minutes=5)
+    _TIME_1: time = time(hour=18, minute=20, second=0, tzinfo=UTC)
+    _TIME_2: time = time(hour=18, minute=25, second=0, tzinfo=UTC)
+    _TIME_3: time = time(hour=18, minute=30, second=0, tzinfo=UTC)
+    _TIME_4: time = time(hour=18, minute=35, second=0, tzinfo=UTC)
+    _TIME_5: time = time(hour=18, minute=40, second=0, tzinfo=UTC)
 
     def test_invalid_dep_code(self):   self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EH02', 'EDDH', self._TIME_1))
     def test_invalid_arr_code(self):   self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'abc',  self._TIME_1))
+    def test_missing_out(self):        self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', None))
     def test_missing_off(self):        self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_1, time_on=self._TIME_2))
     def test_missing_on(self):         self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_1, time_off=self._TIME_2, time_in=self._TIME_3))
-    def test_off_before_out(self):     self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_2, time_off=self._TIME_1))
-    def test_on_before_off(self):      self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_1, time_off=self._TIME_3, time_on=self._TIME_2))
-    def test_in_before_on(self):       self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_1, time_off=self._TIME_2, time_on=self._TIME_4, time_in=self._TIME_3))
-    def test_eta_before_out(self):     self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_2, self._TIME_1))
-    def test_eta_before_off(self):     self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_1, self._TIME_2, self._TIME_3))
-    def test_eta_after_arrival(self):  self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_1, self._TIME_4, self._TIME_2, self._TIME_3))
+    def test_eta_after_arrival(self):  self.assertRaises(ValueError, lambda: ProgressMessage('CALLSIGN', 'OPS', 'EDDF', 'EDDH', self._TIME_1, self._TIME_5, self._TIME_2, self._TIME_3, self._TIME_4))
+
+
+class TestProgressMessageRepresentation(unittest.TestCase):
+    _TIME_1: time = time(hour=18, minute=20, second=0, tzinfo=UTC)
+    _TIME_2: time = time(hour=18, minute=25, second=0, tzinfo=UTC)
+    _TIME_3: time = time(hour=18, minute=30, second=0, tzinfo=UTC)
+    _TIME_4: time = time(hour=18, minute=35, second=0, tzinfo=UTC)
+    
+    def test_repr_out_eta(self):
+        import datetime # used inside eval()
+
+        expected = ProgressMessage('CALLSIGN', 'OPS', 'AAAA', 'BBBB', self._TIME_1, self._TIME_2)
+        actual = eval(repr(expected))
+        self.assertEqual(expected, actual)
+
+    def test_repr_out_off_on_in(self):
+        import datetime # used inside eval()
+
+        expected = ProgressMessage('CALLSIGN', 'OPS', 'AAAA', 'BBBB', self._TIME_1, None, self._TIME_2, self._TIME_3, self._TIME_4)
+        actual = eval(repr(expected))
+        self.assertEqual(expected, actual)
```

### Comparing `hoppie-connector-0.0.1/tests/test_TelexMessage.py` & `hoppie-connector-0.1.0/tests/test_TelexMessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,7 +13,13 @@
     def test_get_msg_type(self):       self.assertEqual(self._EXPECTED_TYPE,    self._UUT.get_msg_type())
     def test_get_message(self):        self.assertEqual(self._EXPECTED_MESSAGE, self._UUT.get_message())
     def test_get_packet_content(self): self.assertEqual(self._EXPECTED_PACKET,  self._UUT.get_packet_content())
 
 class TestTelexMessageInputValidation(unittest.TestCase):
     def test_message_too_long(self):     self.assertRaises(ValueError, lambda: TelexMessage('CALLSIGN', 'OPS', 221 * 'a'))
     def test_invalid_message_char(self): self.assertRaises(ValueError, lambda: TelexMessage('CALLSIGN', 'OPS', 'ä'))
+
+class TestTelexMessageRepresentation(unittest.TestCase):
+    def test_repr(self):
+        expected = TelexMessage('CALLSIGN', 'OPS', 'Message')
+        actual = eval(repr(expected))
+        self.assertEqual(expected, actual)
```

