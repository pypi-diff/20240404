# Comparing `tmp/mypy-boto3-emr-containers-1.34.70.tar.gz` & `tmp/mypy-boto3-emr-containers-1.34.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-containers-1.34.70.tar", last modified: Mon Mar 25 19:34:00 2024, max compression
+gzip compressed data, was "mypy-boto3-emr-containers-1.34.78.tar", last modified: Thu Apr  4 19:33:17 2024, max compression
```

## Comparing `mypy-boto3-emr-containers-1.34.70.tar` & `mypy-boto3-emr-containers-1.34.78.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:00.825656 mypy-boto3-emr-containers-1.34.70/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-03-25 19:34:00.825656 mypy-boto3-emr-containers-1.34.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:00.825656 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18338 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-03-25 19:33:16.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-03-25 19:33:16.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28154 2024-03-25 19:33:16.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28154 2024-03-25 19:33:16.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:00.825656 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-03-25 19:34:00.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-25 19:34:00.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 19:34:00.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 19:34:00.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-25 19:34:00.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-25 19:34:00.000000 mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 19:34:00.825656 mypy-boto3-emr-containers-1.34.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-25 19:33:15.000000 mypy-boto3-emr-containers-1.34.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18444 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28264 2024-04-04 19:33:02.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28264 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/setup.py
```

### Comparing `mypy-boto3-emr-containers-1.34.70/LICENSE` & `mypy-boto3-emr-containers-1.34.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.34.70/PKG-INFO` & `mypy-boto3-emr-containers-1.34.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.34.70
-Summary: Type annotations for boto3.EMRContainers 1.34.70 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.78
+Summary: Type annotations for boto3.EMRContainers 1.34.78 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-emr-containers-1.34.70/README.md` & `mypy-boto3-emr-containers-1.34.78/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/__init__.py` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/__init__.pyi` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/__main__.py` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRContainers 1.34.70\n"
-        "Version:         1.34.70\n"
+        "Type annotations for boto3.EMRContainers 1.34.78\n"
+        "Version:         1.34.78\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.70")
+    print("1.34.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/client.py` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
+    EKSRequestThrottledException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     RequestThrottledException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
 class EMRContainersClient(BaseClient):
@@ -326,14 +327,15 @@
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
+        eksAccessEntryIntegrated: bool = ...,
     ) -> ListVirtualClustersResponseTypeDef:
         """
         Lists information about the specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_virtual_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_virtual_clusters)
         """
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/client.pyi` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
+    EKSRequestThrottledException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     RequestThrottledException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 class EMRContainersClient(BaseClient):
     """
@@ -323,14 +324,15 @@
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
+        eksAccessEntryIntegrated: bool = ...,
     ) -> ListVirtualClustersResponseTypeDef:
         """
         Lists information about the specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_virtual_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_virtual_clusters)
         """
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/literals.py` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -153,14 +154,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/literals.pyi` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -153,14 +154,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/paginator.py` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,13 +136,14 @@
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
+        eksAccessEntryIntegrated: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/paginator.pyi` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -131,13 +131,14 @@
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: TimestampTypeDef = ...,
         createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
+        eksAccessEntryIntegrated: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/type_defs.py` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,27 +509,29 @@
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": NotRequired[str],
         "containerProviderType": NotRequired[Literal["EKS"]],
         "createdAfter": NotRequired[TimestampTypeDef],
         "createdBefore": NotRequired[TimestampTypeDef],
         "states": NotRequired[Sequence[VirtualClusterStateType]],
+        "eksAccessEntryIntegrated": NotRequired[bool],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListVirtualClustersRequestRequestTypeDef = TypedDict(
     "ListVirtualClustersRequestRequestTypeDef",
     {
         "containerProviderId": NotRequired[str],
         "containerProviderType": NotRequired[Literal["EKS"]],
         "createdAfter": NotRequired[TimestampTypeDef],
         "createdBefore": NotRequired[TimestampTypeDef],
         "states": NotRequired[Sequence[VirtualClusterStateType]],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "eksAccessEntryIntegrated": NotRequired[bool],
     },
 )
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "persistentAppUI": NotRequired[PersistentAppUIType],
         "cloudWatchMonitoringConfiguration": NotRequired[CloudWatchMonitoringConfigurationTypeDef],
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers/type_defs.pyi` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -509,27 +509,29 @@
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": NotRequired[str],
         "containerProviderType": NotRequired[Literal["EKS"]],
         "createdAfter": NotRequired[TimestampTypeDef],
         "createdBefore": NotRequired[TimestampTypeDef],
         "states": NotRequired[Sequence[VirtualClusterStateType]],
+        "eksAccessEntryIntegrated": NotRequired[bool],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListVirtualClustersRequestRequestTypeDef = TypedDict(
     "ListVirtualClustersRequestRequestTypeDef",
     {
         "containerProviderId": NotRequired[str],
         "containerProviderType": NotRequired[Literal["EKS"]],
         "createdAfter": NotRequired[TimestampTypeDef],
         "createdBefore": NotRequired[TimestampTypeDef],
         "states": NotRequired[Sequence[VirtualClusterStateType]],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
+        "eksAccessEntryIntegrated": NotRequired[bool],
     },
 )
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "persistentAppUI": NotRequired[PersistentAppUIType],
         "cloudWatchMonitoringConfiguration": NotRequired[CloudWatchMonitoringConfigurationTypeDef],
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/PKG-INFO` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.34.70
-Summary: Type annotations for boto3.EMRContainers 1.34.70 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.78
+Summary: Type annotations for boto3.EMRContainers 1.34.78 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-emr-containers-1.34.70/mypy_boto3_emr_containers.egg-info/SOURCES.txt` & `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.34.70/setup.py` & `mypy-boto3-emr-containers-1.34.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-containers",
-    version="1.34.70",
+    version="1.34.78",
     packages=["mypy_boto3_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EMRContainers 1.34.70 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.EMRContainers 1.34.78 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

