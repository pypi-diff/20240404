# Comparing `tmp/pkl-python-0.1.10.tar.gz` & `tmp/pkl-python-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkl-python-0.1.10.tar", last modified: Sat Mar 30 06:34:44 2024, max compression
+gzip compressed data, was "pkl-python-0.1.11.tar", last modified: Thu Apr  4 02:24:17 2024, max compression
```

## Comparing `pkl-python-0.1.10.tar` & `pkl-python-0.1.11.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:34:44.467593 pkl-python-0.1.10/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-30 06:34:35.000000 pkl-python-0.1.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-03-30 06:34:44.467593 pkl-python-0.1.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-30 06:34:35.000000 pkl-python-0.1.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:34:44.463593 pkl-python-0.1.10/pkl/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-30 06:34:35.000000 pkl-python-0.1.10/pkl/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-03-30 06:34:35.000000 pkl-python-0.1.10/pkl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-03-30 06:34:35.000000 pkl-python-0.1.10/pkl/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-30 06:34:35.000000 pkl-python-0.1.10/pkl/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-03-30 06:34:35.000000 pkl-python-0.1.10/pkl/msgapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-03-30 06:34:35.000000 pkl-python-0.1.10/pkl/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-03-30 06:34:35.000000 pkl-python-0.1.10/pkl/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:34:44.463593 pkl-python-0.1.10/pkl_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-03-30 06:34:44.000000 pkl-python-0.1.10/pkl_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-30 06:34:44.000000 pkl-python-0.1.10/pkl_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 06:34:44.000000 pkl-python-0.1.10/pkl_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-30 06:34:44.000000 pkl-python-0.1.10/pkl_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-30 06:34:44.000000 pkl-python-0.1.10/pkl_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-30 06:34:35.000000 pkl-python-0.1.10/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:34:44.463593 pkl-python-0.1.10/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-30 06:34:35.000000 pkl-python-0.1.10/scripts/download_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-30 06:34:35.000000 pkl-python-0.1.10/scripts/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 06:34:44.467593 pkl-python-0.1.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-30 06:34:35.000000 pkl-python-0.1.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:34:44.463593 pkl-python-0.1.10/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-30 06:34:35.000000 pkl-python-0.1.10/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-30 06:34:35.000000 pkl-python-0.1.10/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-30 06:34:35.000000 pkl-python-0.1.10/tests/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-30 06:34:35.000000 pkl-python-0.1.10/tests/test_server.py
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.228855 pkl-python-0.1.11/
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1069 2024-03-29 10:49:37.000000 pkl-python-0.1.11/LICENSE
+-rw-r--r--   0 jwyang    (1002) jwyang    (1002)     5982 2024-04-04 02:24:17.228855 pkl-python-0.1.11/PKG-INFO
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     3841 2024-04-04 02:20:34.000000 pkl-python-0.1.11/README.md
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.224855 pkl-python-0.1.11/pkl/
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)        7 2024-04-04 01:41:54.000000 pkl-python-0.1.11/pkl/VERSION
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     3925 2024-04-04 02:17:34.000000 pkl-python-0.1.11/pkl/__init__.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)    12506 2024-04-03 09:53:08.000000 pkl-python-0.1.11/pkl/evaluator_manager.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     4841 2024-04-03 09:01:42.000000 pkl-python-0.1.11/pkl/evaluator_options.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     8111 2024-04-03 02:57:01.000000 pkl-python-0.1.11/pkl/msgapi.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     8637 2024-04-04 01:53:48.000000 pkl-python-0.1.11/pkl/parser.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1780 2024-04-03 06:30:38.000000 pkl-python-0.1.11/pkl/reader.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     4147 2024-04-03 11:02:36.000000 pkl-python-0.1.11/pkl/server.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      658 2024-04-03 09:53:07.000000 pkl-python-0.1.11/pkl/utils.py
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.224855 pkl-python-0.1.11/pkl_python.egg-info/
+-rw-r--r--   0 jwyang    (1002) jwyang    (1002)     5982 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/PKG-INFO
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      515 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/SOURCES.txt
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)        1 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/dependency_links.txt
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)       79 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/requires.txt
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)        4 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/top_level.txt
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1131 2024-04-02 16:55:35.000000 pkl-python-0.1.11/pyproject.toml
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.224855 pkl-python-0.1.11/scripts/
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      978 2024-03-29 10:49:37.000000 pkl-python-0.1.11/scripts/download_binary.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      917 2024-03-29 10:49:37.000000 pkl-python-0.1.11/scripts/eval.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)       38 2024-04-04 02:24:17.228855 pkl-python-0.1.11/setup.cfg
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1939 2024-04-03 10:11:23.000000 pkl-python-0.1.11/setup.py
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.224855 pkl-python-0.1.11/tests/
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      474 2024-04-03 10:48:59.000000 pkl-python-0.1.11/tests/test_evaluator_manager.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      385 2024-04-03 10:33:31.000000 pkl-python-0.1.11/tests/test_load.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      975 2024-04-03 05:39:56.000000 pkl-python-0.1.11/tests/test_parser.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1756 2024-04-04 02:18:03.000000 pkl-python-0.1.11/tests/test_readers.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      102 2024-04-02 21:06:36.000000 pkl-python-0.1.11/tests/test_server.py
```

### Comparing `pkl-python-0.1.10/LICENSE` & `pkl-python-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.10/pkl/msgapi.py` & `pkl-python-0.1.11/pkl/msgapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-from dataclasses import asdict, dataclass, field, is_dataclass
-from typing import Any, Dict, List, Optional, Union
+from __future__ import annotations
+
+from dataclasses import asdict, dataclass
+from typing import Any, Dict, List, Optional
+
+from pkl.evaluator_options import ClientModuleReader, ClientResourceReader, Project
+from pkl.reader import PathElement
 
 CODE_NEW_EVALUATOR = 0x20
 CODE_NEW_EVALUATOR_RESPONSE = 0x21
 CODE_CLOSE_EVALUATOR = 0x22
 CODE_EVALUATE = 0x23
 CODE_EVALUATE_RESPONSE = 0x24
 CODE_EVALUATE_LOG = 0x25
@@ -14,261 +19,294 @@
 CODE_LIST_RESOURCES_REQUEST = 0x2A
 CODE_LIST_RESOURCES_RESPONSE = 0x2B
 CODE_LIST_MODULES_REQUEST = 0x2C
 CODE_LIST_MODULES_RESPONSE = 0x2D
 
 
 # Define the base interface for incoming messages
+@dataclass
 class IncomingMessage:
-    pass
+    @classmethod
+    def decode(cls, incoming: List):
+        code, msg = incoming
+
+        if code == CODE_EVALUATE_RESPONSE:
+            return EvaluateResponse(**msg)
+        elif code == CODE_EVALUATE_LOG:
+            return Log(**msg)
+        elif code == CODE_NEW_EVALUATOR_RESPONSE:
+            return CreateEvaluatorResponse(**msg)
+        elif code == CODE_EVALUATE_READ:
+            return EvaluatorReadResourceRequest(**msg)
+        elif code == CODE_EVALUATE_READ_MODULE:
+            return EvaluatorReadModuleRequest(**msg)
+        elif code == CODE_LIST_RESOURCES_REQUEST:
+            return EvaluatorListResourcesRequest(**msg)
+        elif code == CODE_LIST_MODULES_REQUEST:
+            return EvaluatorListModulesRequest(**msg)
+        else:
+            raise ValueError(f"Unknown code: {hex(code)}")
 
 
 @dataclass
 class CreateEvaluatorResponse(IncomingMessage):
+    # A number identifying this request
     requestId: int
+
+    # A number identifying the created evaluator.
     evaluatorId: Optional[int] = None
+
+    # A message detailing why the evaluator was not created.
     error: Optional[str] = None
 
 
 @dataclass
 class EvaluateResponse(IncomingMessage):
-    """
-    A class to represent a response to an evaluation request.
-
-    Attributes:
-    - requestId (int): The requestId of the Evaluate request.
-    - evaluatorId (int): A number identifying the evaluator.
-    - result (Optional[Any]): The evaluation contents, if successful. None if evaluation failed.
-    - error (Optional[str]): A message detailing why evaluation failed. None if evaluation was successful.
-    """
-
+    # The requestId of the Evaluate request
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # The evaluation contents, if successful.
     result: Optional[Any] = None
+
+    # A message detailing why evaluation failed.
     error: Optional[str] = None
 
 
 @dataclass
 class Log(IncomingMessage):
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # A number identifying the log level.
+    #
+    # - 0: trace
+    # - 1: warn
     level: int
+
+    # The message to be logged
     message: str
+
+    # A string representing the source location within Pkl code producing this log output.
     frameUri: str
 
 
 @dataclass
 class EvaluatorReadResourceRequest(IncomingMessage):
+    # A number identifying this request.
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # The URI of the resource.
     uri: str
 
 
 @dataclass
 class EvaluatorReadModuleRequest(IncomingMessage):
+    # A number identifying this request.
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # The URI of the module.
     uri: str
 
 
 @dataclass
 class EvaluatorListResourcesRequest(IncomingMessage):
+    # A number identifying this request.
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # The base URI to list resources.
     uri: str
 
 
 @dataclass
 class EvaluatorListModulesRequest(IncomingMessage):
+    # A number identifying this request.
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # The base URI to list modules.
     uri: str
 
 
 @dataclass
 class OutgoingMessage:
-    def to_msg_obj(self):
-        raise NotImplementedError("Subclasses must implement this method.")
+    CODE = None
 
+    def _dict_factory(self, items):
+        return {k: v for k, v in items if v is not None}
 
-def dataclass_to_dict(dc):
-    if not is_dataclass(dc):
-        return dc
-
-    dd = {k: dataclass_to_dict(v) for k, v in asdict(dc).items()}
-    return dd
-
-
-def _filter_dict(dd):
-    if not isinstance(dd, dict):
-        return dd
-    return {k: _filter_dict(v) for k, v in dd.items() if v is not None}
-
-
-def format_message(msg: OutgoingMessage, code: int):
-    # msg_dict = asdict(msg)
-    # filtered_dict = {k: v for k, v in msg_dict.items() if v is not None}
-    msg_dict = dataclass_to_dict(msg)
-    filtered_dict = _filter_dict(msg_dict)
-    msg_obj = [code, filtered_dict]
-    return msg_obj
-
-
-@dataclass
-class ResourceReader:
-    scheme: str
-    has_hierarchical_uris: bool
-    is_globbable: bool
-
-
-@dataclass
-class ModuleReader:
-    scheme: str
-    has_hierarchical_uris: bool
-    is_globbable: bool
-    is_local: bool
+    def to_json(self):
+        assert self.CODE is not None
+        msg = asdict(self, dict_factory=self._dict_factory)
+        obj = [self.CODE, msg]
+        return obj
 
 
 @dataclass
-class Checksums:
-    sha256: str
-
-
-@dataclass
-class PathElement:
-    name: str
-    is_directory: bool
-
-
-@dataclass
-class ProjectOrDependency:
-    package_uri: Optional[str] = None
-    type: str = ""
-    project_file_uri: Optional[str] = None
-    checksums: Optional[Checksums] = None
-    dependencies: Dict[str, "ProjectOrDependency"] = field(default_factory=dict)
-
-
-@dataclass
-class ClientResourceReader:
-    scheme: str
-    hasHierarchicalUris: bool
-    isGlobbable: bool
-
-
-@dataclass
-class ClientModuleReader:
-    scheme: str
-    hasHierarchicalUris: bool
-    isGlobbable: bool
-    isLocal: bool
-
+class CreateEvaluator(OutgoingMessage):
+    CODE = CODE_NEW_EVALUATOR
 
-@dataclass
-class RemoteDependency:
-    type: str = "remote"
-    packageUri: Optional[str] = None
-    checksums: Optional[Checksums] = None
+    # A number identifying this request
+    requestId: int = 0
 
+    # Regex patterns to determine which modules are allowed for import.
+    #
+    # API version of the CLI's `--allowed-modules` flag
+    allowedModules: Optional[List[str]] = None
+
+    # Regex patterns to dettermine which resources are allowed to be read.
+    #
+    # API version of the CLI's `--allowed-resources` flag
+    allowedResources: Optional[List[str]] = None
+
+    # Register client-side module readers.
+    clientModuleReaders: Optional[List[ClientModuleReader]] = None
+
+    # Register client-side resource readers.
+    clientResourceReaders: Optional[List[ClientResourceReader]] = None
+
+    # Directories, ZIP archives, or JAR archives
+    # to search when resolving `modulepath:` URIs.
+    #
+    # API version of the CLI's `--module-path` flag.
+    modulePaths: Optional[List[str]] = None
+
+    # Environment variable to set.
+    #
+    # API version of the CLI's `--env-var` flag.
+    env: Optional[Dict[str, str]] = None
+
+    # External properties to set.
+    #
+    # API version of the CLI's `--properties` flag.
+    properties: Optional[Dict[str, str]] = None
+
+    # Duration, in seconds, after which evaluation of a source module will be timed out.
+    #
+    # API version of the CLI's `--timeout` flag.
+    timeoutSeconds: Optional[int] = None
+
+    # Restricts access to file-based modules and resources to those located under the root directory.
+    rootDir: Optional[str] = None
+
+    # The cache directory for storing packages.
+    cacheDir: Optional[str] = None
+
+    # The format to generate.
+    #
+    # This sets the `pkl.outputFormat` external property.
+    outputFormat: Optional[str] = None
 
-@dataclass
-class Project:
-    projectFileUri: str
-    packageUri: Optional[str] = None
-    type: str = "local"
-    dependencies: Dict[str, Union["Project", RemoteDependency]] = field(
-        default_factory=dict
-    )
-
-
-@dataclass
-class CreateEvaluator(OutgoingMessage):
-    requestId: int
-    allowedModules: Optional[List[str]] = field(default=None)
-    allowedResources: Optional[List[str]] = field(default=None)
-    clientModuleReaders: Optional[List[ClientModuleReader]] = field(default=None)
-    clientResourceReaders: Optional[List[ClientResourceReader]] = field(default=None)
-    modulePaths: Optional[List[str]] = field(default=None)
-    env: Optional[Dict[str, str]] = field(default=None)
-    properties: Optional[Dict[str, str]] = field(default=None)
-    timeoutSeconds: Optional[int] = field(default=None)
-    rootDir: Optional[str] = field(default=None)
-    cacheDir: Optional[str] = field(default=None)
-    outputFormat: Optional[str] = field(default=None)
-    project: Optional[Project] = field(default=None)
-
-    def to_msg_obj(self):
-        return format_message(self, CODE_NEW_EVALUATOR)
+    # The project dependency settings.
+    project: Optional[Project] = None
 
 
 @dataclass
 class CloseEvaluator(OutgoingMessage):
-    evaluatorId: int
+    CODE = CODE_CLOSE_EVALUATOR
 
-    def to_msg_obj(self):
-        return format_message(self, CODE_CLOSE_EVALUATOR)
+    # A number identifying this evaluator.
+    evaluatorId: int
 
 
 @dataclass
 class EvaluateRequest(OutgoingMessage):
-    """
-    A class to represent a request for evaluating a module or expression in Pkl.
-
-    Attributes:
-    - requestId: A number identifying this request.
-    - evaluatorId: A number identifying the evaluator.
-    - moduleUri: The absolute URI of the module to be evaluated.
-    - moduleText: The module's contents. If None, Pkl will load the module at runtime.
-    - expr: The Pkl expression to be evaluated within the module. If None, evaluates the whole module.
-    """
-
+    CODE = CODE_EVALUATE
+    # A number identifying this request
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # The absolute URI of the module to be evaluated.
     moduleUri: str
+
+    # The module's contents.
+    #
+    # If [null], Pkl will load the module at runtime.
     moduleText: Optional[str] = None
-    expr: Optional[str] = None
 
-    def to_msg_obj(self):
-        return format_message(self, CODE_EVALUATE)
+    # The Pkl expression to be evaluated within the module.
+    #
+    # If [null], evaluates the whole module.
+    expr: Optional[str] = None
 
 
 @dataclass
 class EvaluatorReadResourceResponse(OutgoingMessage):
+    CODE = CODE_EVALUATE_READ_RESPONSE
+
+    # A number identifying this request.
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # The contents of the resource.
     contents: Optional[bytes] = None
-    error: Optional[str] = None
 
-    def to_msg_obj(self):
-        return format_message(self, CODE_EVALUATE_READ_RESPONSE)
+    # The description of the error that occured when reading this resource.
+    error: Optional[str] = None
 
 
 @dataclass
 class EvaluatorReadModuleResponse(OutgoingMessage):
+    CODE = CODE_EVALUATE_READ_MODULE_RESPONSE
+
+    # A number identifying this request.
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
+
+    # The string contents of the module.
     contents: Optional[str] = None
-    error: Optional[str] = None
 
-    def to_msg_obj(self):
-        return format_message(self, CODE_EVALUATE_READ_MODULE_RESPONSE)
+    # The description of the error that occured when reading this resource.
+    error: Optional[str] = None
 
 
 @dataclass
 class EvaluatorListResourcesResponse(OutgoingMessage):
+    CODE = CODE_LIST_RESOURCES_RESPONSE
+
+    # A number identifying this request.
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
-    pathElements: List[PathElement] = field(default_factory=list)
-    error: Optional[str] = None
 
-    def to_msg_obj(self):
-        return format_message(self, CODE_LIST_RESOURCES_RESPONSE)
+    # The elements at the provided base path.
+    pathElements: Optional[List[PathElement]] = None
+
+    # The description of the error that occured when listing elements.
+    error: Optional[str] = None
 
 
 @dataclass
 class EvaluatorListModulesResponse(OutgoingMessage):
+    CODE = CODE_LIST_MODULES_RESPONSE
+
+    # A number identifying this request.
     requestId: int
+
+    # A number identifying this evaluator.
     evaluatorId: int
-    pathElements: List[PathElement] = field(default_factory=list)
-    error: Optional[str] = None
 
-    def to_msg_obj(self):
-        return format_message(self, CODE_LIST_MODULES_RESPONSE)
+    # The elements at the provided base path.
+    pathElements: Optional[List[PathElement]] = None
+
+    # The description of the error that occured when listing elements.
+    error: Optional[str] = None
```

### Comparing `pkl-python-0.1.10/pkl/parser.py` & `pkl-python-0.1.11/pkl/parser.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -76,25 +76,25 @@
 @dataclass
 class DataSize:
     value: float
     unit: Literal["b", "kb", "kib", "mb", "mib", "gb", "gib", "tb", "tib", "pb", "pib"]
 
 
 @dataclass
-class Regex:
-    pattern: str
-
-
-@dataclass
 class IntSeq:
     start: int
     end: int
     step: int
 
 
+@dataclass
+class Regex:
+    pattern: str
+
+
 class Parser:
     def __init__(
         self,
         force_render=False,
         *,
         typed_dynamic_result_type=ResultType.DATACLASS,
         pair_result_type=ResultType.DATACLASS,
```

### Comparing `pkl-python-0.1.10/pyproject.toml` & `pkl-python-0.1.11/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 dynamic = ["version"]
 description = "Python library for Apple's PKL."
 authors = [
     { name = "Jungwoo Yang", email = "jwyang0213@gmail.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "msgpack >= 1.0.8"
 ]
 
 [tool.setuptools.packages.find]
-exclude = ["codegen"]
+include = ["pkl"]
 
 [tool.setuptools.dynamic]
 version = {file = "pkl/VERSION"}
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
```

### Comparing `pkl-python-0.1.10/scripts/download_binary.py` & `pkl-python-0.1.11/scripts/download_binary.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.10/scripts/eval.py` & `pkl-python-0.1.11/scripts/eval.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.10/setup.py` & `pkl-python-0.1.11/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 BINARIES = {
     ("darwin", "64bit"): "pkl-macos-amd64",
     ("darwin", "aarch64"): "pkl-macos-aarch64",
     ("linux", "64bit"): "pkl-linux-amd64",
     ("linux", "aarch64"): "pkl-linux-aarch64",
     ("linux", "64bit", "alpine"): "pkl-alpine-linux-amd64",
 }
-PKL_VERSION = "0.25.2"
+PKL_VERSION = "0.25.3"
 BASE_PATH = "https://github.com/apple/pkl/releases/download/"
 
 
 def detect_system():
     os_name = platform.system().lower()
     arch, _ = platform.architecture()
     return os_name, arch
```

### Comparing `pkl-python-0.1.10/tests/test_parser.py` & `pkl-python-0.1.11/tests/test_parser.py`

 * *Files identical despite different names*

