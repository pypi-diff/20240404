# Comparing `tmp/dagster-embedded-elt-0.22.9.tar.gz` & `tmp/dagster-embedded-elt-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.22.9.tar", last modified: Fri Mar  8 00:30:54 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.0.tar", last modified: Thu Apr  4 19:54:26 2024, max compression
```

## Comparing `dagster-embedded-elt-0.22.9.tar` & `dagster-embedded-elt-0.23.0.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:30:54.122948 dagster-embedded-elt-0.22.9/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       59 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      723 2024-03-08 00:30:54.122948 dagster-embedded-elt-0.22.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:30:54.118948 dagster-embedded-elt-0.22.9/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:30:54.122948 dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4728 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8294 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    14382 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1050 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:30:54.118948 dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      723 2024-03-08 00:30:53.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      661 2024-03-08 00:30:54.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:30:53.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:30:53.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-08 00:30:53.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-08 00:30:53.000000 dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-03-08 00:30:54.122948 dagster-embedded-elt-0.22.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1360 2024-03-08 00:17:46.000000 dagster-embedded-elt-0.22.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.295620 dagster-embedded-elt-0.23.0/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-04 19:54:26.295620 dagster-embedded-elt-0.23.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.283619 dagster-embedded-elt-0.23.0/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.287619 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.291620 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4931 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    17477 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.283619 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-04-04 19:54:26.295620 dagster-embedded-elt-0.23.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/setup.py
```

### Comparing `dagster-embedded-elt-0.22.9/LICENSE` & `dagster-embedded-elt-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.22.9/PKG-INFO` & `dagster-embedded-elt-0.23.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8,<3.13
+Provides-Extra: test
 License-File: LICENSE
```

### Comparing `dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     multi_asset,
 )
 from dagster._utils.security import non_secure_md5_hash_str
 
 from dagster_embedded_elt.sling.dagster_sling_translator import DagsterSlingTranslator
 from dagster_embedded_elt.sling.sling_replication import SlingReplicationParam, validate_replication
 
+METADATA_KEY_TRANSLATOR = "dagster_embedded_elt/dagster_sling_translator"
+METADATA_KEY_REPLICATION_CONFIG = "dagster_embedded_elt/sling_replication_config"
+
 
 def get_streams_from_replication(
     replication_config: Mapping[str, Any],
 ) -> Iterable[Mapping[str, Any]]:
     """Returns a list of streams and their configs from a Sling replication config."""
     for stream, config in replication_config.get("streams", {}).items():
         if config and config.get("disabled", False):
@@ -67,40 +70,38 @@
                     ),
                 ]
             )
 
             config_path = "/path/to/replication.yaml"
             @sling_assets(replication_config=config_path)
             def my_assets(context, sling: SlingResource):
-                for lines in sling.replicate(
-                    replication_config=config_path,
-                    dagster_sling_translator=DagsterSlingTranslator(),
-                ):
-                    context.log.info(lines)
+                yield from sling.replicate(context=context)
     """
     replication_config = validate_replication(replication_config)
     streams = get_streams_from_replication(replication_config)
-
-    group_name = dagster_sling_translator.get_group_name(replication_config)
     code_version = non_secure_md5_hash_str(str(replication_config).encode())
-    freshness_policy = dagster_sling_translator.get_freshness_policy(replication_config)
-    auto_materialize_policy = dagster_sling_translator.get_auto_materialize_policy(
-        replication_config
-    )
 
     specs: list[AssetSpec] = []
     for stream in streams:
         specs.append(
             AssetSpec(
                 key=dagster_sling_translator.get_asset_key(stream),
                 deps=dagster_sling_translator.get_deps_asset_key(stream),
-                group_name=group_name,
+                description=dagster_sling_translator.get_description(stream),
+                metadata={  # type: ignore
+                    **dagster_sling_translator.get_metadata(stream),
+                    METADATA_KEY_TRANSLATOR: dagster_sling_translator,
+                    METADATA_KEY_REPLICATION_CONFIG: replication_config,
+                },
+                group_name=dagster_sling_translator.get_group_name(stream),
+                freshness_policy=dagster_sling_translator.get_freshness_policy(stream),
+                auto_materialize_policy=dagster_sling_translator.get_auto_materialize_policy(
+                    stream
+                ),
                 code_version=code_version,
-                freshness_policy=freshness_policy,
-                auto_materialize_policy=auto_materialize_policy,
             )
         )
 
     def inner(fn) -> AssetsDefinition:
         asset_definition = multi_asset(
             name=name,
             compute_kind="sling",
```

### Comparing `dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 
 @dataclass
 class DagsterSlingTranslator:
     target_prefix: str = "target"
 
     @public
-    @classmethod
-    def sanitize_stream_name(cls, stream_name: str) -> str:
+    def sanitize_stream_name(self, stream_name: str) -> str:
         """A function that takes a stream name from a Sling replication config and returns a
         sanitized name for the stream.
 
         By default, this removes any non-alphanumeric characters from the stream name and replaces
         them with underscores, while removing any double quotes.
 
         Args:
@@ -29,16 +28,15 @@
 
         Examples:
             Using a custom stream name sanitizer:
 
             .. code-block:: python
 
                 class CustomSlingTranslator(DagsterSlingTranslator):
-                    @classmethod
-                    def sanitize_stream_name(cls, stream_name: str) -> str:
+                    def sanitize_stream_name(self, stream_name: str) -> str:
                         return stream_name.replace(".", "")
         """
         return re.sub(r"[^a-zA-Z0-9_.]", "_", stream_name.replace('"', "").lower())
 
     @public
     def get_asset_key(self, stream_definition: Mapping[str, Any]) -> AssetKey:
         """A function that takes a stream definition from a Sling replication config and returns a
@@ -79,15 +77,14 @@
 
         Examples:
             Using a custom mapping for streams:
 
             .. code-block:: python
 
                 class CustomSlingTranslator(DagsterSlingTranslator):
-                    @classmethod
                     def get_asset_key_for_target(self, stream_definition) -> AssetKey:
                         map = {"stream1": "asset1", "stream2": "asset2"}
                         return AssetKey(map[stream_name])
         """
         config = stream_definition.get("config", {}) or {}
         object_key = config.get("object")
         meta = config.get("meta", {})
@@ -103,16 +100,15 @@
 
         # You can override the Sling Replication default object with an object key
         stream_name = object_key or stream_definition["name"]
         sanitized_components = self.sanitize_stream_name(stream_name).split(".")
         return AssetKey([self.target_prefix] + sanitized_components)
 
     @public
-    @classmethod
-    def get_deps_asset_key(cls, stream_definition: Mapping[str, Any]) -> Iterable[AssetKey]:
+    def get_deps_asset_key(self, stream_definition: Mapping[str, Any]) -> Iterable[AssetKey]:
         """A function that takes a stream name from a Sling replication config and returns a
         Dagster AssetKey for the dependencies of the replication stream.
 
         By default, this returns the stream name. For example, a stream named "public.accounts"
         will create an AssetKey named "target_public_accounts" and a dependency named "public_accounts".
 
         Override this function to customize how to map a Sling stream to a Dagster depenency.
@@ -134,81 +130,75 @@
 
         Examples:
             Using a custom mapping for streams:
 
             .. code-block:: python
 
                 class CustomSlingTranslator(DagsterSlingTranslator):
-                    @classmethod
-                    def get_deps_asset_key(cls, stream_name: str) -> AssetKey:
+                    def get_deps_asset_key(self, stream_name: str) -> AssetKey:
                         map = {"stream1": "asset1", "stream2": "asset2"}
                         return AssetKey(map[stream_name])
 
         """
         config = stream_definition.get("config", {}) or {}
         meta = config.get("meta", {})
         deps = meta.get("dagster", {}).get("deps")
         deps_out = []
         if deps and isinstance(deps, str):
             deps = [deps]
         if deps:
             assert isinstance(deps, list)
             for asset_key in deps:
-                if cls.sanitize_stream_name(asset_key) != asset_key:
+                if self.sanitize_stream_name(asset_key) != asset_key:
                     raise ValueError(
                         f"Deps Asset key {asset_key} for stream {stream_definition['name']} is not "
                         "sanitized. Please use only alphanumeric characters and underscores."
                     )
                 deps_out.append(AssetKey(asset_key.split(".")))
             return deps_out
 
         stream_name = stream_definition["name"]
-        components = cls.sanitize_stream_name(stream_name).split(".")
+        components = self.sanitize_stream_name(stream_name).split(".")
         return [AssetKey(components)]
 
-    @classmethod
     @public
-    def get_description(cls, stream_definition: Mapping[str, Any]) -> Optional[str]:
+    def get_description(self, stream_definition: Mapping[str, Any]) -> Optional[str]:
         config = stream_definition.get("config", {}) or {}
         if "sql" in config:
             return config["sql"]
         meta = config.get("meta", {})
         description = meta.get("dagster", {}).get("description")
         return description
 
-    @classmethod
     @public
-    def get_metadata(cls, stream_definition: Mapping[str, Any]) -> Mapping[str, Any]:
+    def get_metadata(self, stream_definition: Mapping[str, Any]) -> Mapping[str, Any]:
         return {"stream_config": MetadataValue.json(stream_definition.get("config", {}))}
 
-    @classmethod
     @public
-    def get_group_name(cls, stream_definition: Mapping[str, Any]) -> Optional[str]:
+    def get_group_name(self, stream_definition: Mapping[str, Any]) -> Optional[str]:
         config = stream_definition.get("config", {}) or {}
         meta = config.get("meta", {})
         return meta.get("dagster", {}).get("group")
 
-    @classmethod
     @public
     def get_freshness_policy(
-        cls, stream_definition: Mapping[str, Any]
+        self, stream_definition: Mapping[str, Any]
     ) -> Optional[FreshnessPolicy]:
         config = stream_definition.get("config", {}) or {}
         meta = config.get("meta", {})
         freshness_policy_config = meta.get("dagster", {}).get("freshness_policy")
         if freshness_policy_config:
             return FreshnessPolicy(
                 maximum_lag_minutes=float(freshness_policy_config["maximum_lag_minutes"]),
                 cron_schedule=freshness_policy_config.get("cron_schedule"),
                 cron_schedule_timezone=freshness_policy_config.get("cron_schedule_timezone"),
             )
 
-    @classmethod
     @public
     def get_auto_materialize_policy(
-        cls, stream_definition: Mapping[str, Any]
+        self, stream_definition: Mapping[str, Any]
     ) -> Optional[AutoMaterializePolicy]:
         config = stream_definition.get("config", {}) or {}
         meta = config.get("meta", {})
         auto_materialize_policy_config = "auto_materialize_policy" in meta.get("dagster", {})
         if auto_materialize_policy_config:
             return AutoMaterializePolicy.eager()
```

### Comparing `dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,37 @@
 import re
 import sys
 import tempfile
 import time
 import uuid
 from enum import Enum
 from subprocess import PIPE, STDOUT, Popen
-from typing import IO, Any, AnyStr, Dict, Generator, Iterator, List, Optional
+from typing import IO, Any, AnyStr, Dict, Generator, Iterator, List, Optional, Union
 
 import sling
 from dagster import (
+    AssetExecutionContext,
+    AssetMaterialization,
     ConfigurableResource,
     EnvVar,
     MaterializeResult,
+    OpExecutionContext,
     PermissiveConfig,
     get_dagster_logger,
 )
 from dagster._annotations import deprecated, experimental, public
 from dagster._utils.env import environ
 from dagster._utils.warnings import deprecation_warning
 from pydantic import Field
 
-from dagster_embedded_elt.sling.asset_decorator import get_streams_from_replication
+from dagster_embedded_elt.sling.asset_decorator import (
+    METADATA_KEY_REPLICATION_CONFIG,
+    METADATA_KEY_TRANSLATOR,
+    get_streams_from_replication,
+)
 from dagster_embedded_elt.sling.dagster_sling_translator import DagsterSlingTranslator
 from dagster_embedded_elt.sling.sling_replication import SlingReplicationParam, validate_replication
 
 logger = get_dagster_logger()
 
 ANSI_ESCAPE = re.compile(r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])")
 DEPRECATION_WARNING_TEXT = "{name} has been deprecated, use `SlingConnectionResource` for both source and target connections."
@@ -122,71 +129,102 @@
         description="The connection string for the target database.",
         default=None,
     )
 
 
 @public
 class SlingConnectionResource(PermissiveConfig):
-    """A representation a connection to a database or file to be used by Sling. This resource can be used as a source or a target for a Sling sync.
+    """A representation of a connection to a database or file to be used by Sling. This resource can be used as a source or a target for a Sling syncs.
+
+    Reference the Sling docs for more information on possible connection types and parameters: https://docs.slingdata.io/connections
 
-    This resource is responsible for the managing how Sling connects to a resource. To manage how Sling uses this connection (as a source or target), see the specific source_options or target_options in the `build_assets_from_sling_stream` function.
+    The name of the connection is passed to Sling and must match the name of the connection provided in the replication configuration: https://docs.slingdata.io/sling-cli/run/configuration/replication
+    You may provide either a connection string or keyword arguments for the connection.
 
     Examples:
         Creating a Sling Connection for a file, such as CSV or JSON:
 
         .. code-block:: python
 
-             source = SlingConnectionResource(type="file")
+             source = SlingConnectionResource(name="MY_FILE", type="file")
 
         Create a Sling Connection for a Postgres database, using a connection string:
 
         .. code-block:: python
 
-            source = SlingConnectionResource(type="postgres", connection_string=EnvVar("POSTGRES_CONNECTION_STRING"))
-            source = SlingConnectionResource(type="mysql", connection_string="mysql://user:password@host:port/schema")
+            postgres_conn = SlingConnectionResource(name="MY_POSTGRES", type="postgres", connection_string=EnvVar("POSTGRES_CONNECTION_STRING"))
+            mysql_conn = SlingConnectionResource(name="MY_MYSQL", type="mysql", connection_string="mysql://user:password@host:port/schema")
 
-        Create a Sling Connection for a Postgres or Snowflake database, using keyword arguments, as described here:
-        https://docs.slingdata.io/connections/database-connections/postgres
+        Create a Sling Connection for a Postgres or Snowflake database, using keyword arguments:
 
         .. code-block::python
 
-            source = SlingConnectionResource(type="postgres", host="host", user="hunter42", password=EnvVar("POSTGRES_PASSWORD"))
-            source = SlingConnectionResource(type="snowflake", host=EnvVar("SNOWFLAKE_HOST"), user=EnvVar("SNOWFLAKE_USER"), database=EnvVar("SNOWFLAKE_DATABASE"), password=EnvVar("SNOWFLAKE_PASSWORD"), role=EnvVar("SNOWFLAKE_ROLE"))
+            postgres_conn = SlingConnectionResource(
+                name="MY_OTHER_POSRGRES",
+                type="postgres",
+                host="host",
+                user="hunter42",
+                password=EnvVar("POSTGRES_PASSWORD")
+            )
+
+            snowflake_conn = SlingConnectionResource(
+                name="MY_SNOWFLAKE",
+                type="snowflake",
+                host=EnvVar("SNOWFLAKE_HOST"),
+                user=EnvVar("SNOWFLAKE_USER"),
+                database=EnvVar("SNOWFLAKE_DATABASE"),
+                password=EnvVar("SNOWFLAKE_PASSWORD"),
+                role=EnvVar("SNOWFLAKE_ROLE")
+            )
     """
 
-    name: str = Field(description="The name of the connection.")
-    type: str = Field(description="Type of the source connection. Use 'file' for local storage.")
+    name: str = Field(
+        description="The name of the connection, must match the name in your Sling replication configuration."
+    )
+    type: str = Field(
+        description="Type of the source connection, must match the Sling connection types. Use 'file' for local storage."
+    )
     connection_string: Optional[str] = Field(
-        description="The connection string for the source database.",
+        description="The optional connection string for the source database, if not using keyword arguments.",
         default=None,
     )
 
 
 @experimental
 class SlingResource(ConfigurableResource):
-    """Resource for interacting with the Sling package.
+    """Resource for interacting with the Sling package. This resource can be used to run Sling replications.
+
+    Args:
+        connections (List[SlingConnectionResource]): A list of connections to use for the replication.
+        source_connection (Optional[SlingSourceConnection]): Deprecated, use `connections` instead.
+        target_connection (Optional[SlingTargetConnection]): Deprecated, use `connections` instead.
 
     Examples:
         .. code-block:: python
 
-            from dagster_etl.sling import SlingResource
+            from dagster_etl.sling import SlingResource, SlingConnectionResource
+
             sling_resource = SlingResource(
-                source_connection=SlingSourceConnection(
-                    type="postgres", connection_string=EnvVar("POSTGRES_CONNECTION_STRING")
-                ),
-                target_connection=SlingTargetConnection(
-                    type="snowflake",
-                    host="host",
-                    user="user",
-                    database="database",
-                    password="password",
-                    role="role",
-                ),
+                connections=[
+                    SlingConnectionResource(
+                        name="MY_POSTGRES",
+                        type="postgres",
+                        connection_string=EnvVar("POSTGRES_CONNECTION_STRING"),
+                    ),
+                    SlingConnectionResource(
+                        name="MY_SNOWFLAKE",
+                        type="snowflake",
+                        host=EnvVar("SNOWFLAKE_HOST"),
+                        user=EnvVar("SNOWFLAKE_USER"),
+                        database=EnvVar("SNOWFLAKE_DATABASE"),
+                        password=EnvVar("SNOWFLAKE_PASSWORD"),
+                        role=EnvVar("SNOWFLAKE_ROLE"),
+                    ),
+                ]
             )
-
     """
 
     source_connection: Optional[SlingSourceConnection] = None
     target_connection: Optional[SlingTargetConnection] = None
     connections: List[SlingConnectionResource] = []
     _stdout: List[str] = []
 
@@ -279,15 +317,15 @@
         primary_key: Optional[List[str]] = None,
         update_key: Optional[str] = None,
         source_options: Optional[Dict[str, Any]] = None,
         target_options: Optional[Dict[str, Any]] = None,
         encoding: str = "utf8",
     ) -> Generator[str, None, None]:
         """Runs a Sling sync from the given source table to the given destination table. Generates
-        output lines from the Sling CLI.
+        output lines from the Sling CLI. Deprecated, use `replicate` instead.
         """
         if (
             self.source_connection
             and self.source_connection.type == "file"
             and not source_stream.startswith("file://")
         ):
             source_stream = "file://" + source_stream
@@ -320,23 +358,43 @@
 
             sling_cli = sling.Sling(**config)
             logger.info("Starting Sling sync with mode: %s", mode)
             cmd = sling_cli._prep_cmd()  # noqa: SLF001
 
             yield from self._exec_sling_cmd(cmd, encoding=encoding)
 
-    @public
     def replicate(
         self,
         *,
-        replication_config: SlingReplicationParam,
-        dagster_sling_translator: DagsterSlingTranslator,
+        context: Union[OpExecutionContext, AssetExecutionContext],
+        replication_config: Optional[SlingReplicationParam] = None,
+        dagster_sling_translator: Optional[DagsterSlingTranslator] = None,
         debug: bool = False,
-    ):
-        """Docs go here."""
+    ) -> Generator[Union[MaterializeResult, AssetMaterialization], None, None]:
+        """Runs a Sling replication from the given replication config.
+
+        Args:
+            context: Asset or Op execution context.
+            replication_config: The Sling replication config to use for the replication.
+            dagster_sling_translator: The translator to use for the replication.
+            debug: Whether to run the replication in debug mode.
+
+        Returns:
+            Generator[Union[MaterializeResult, AssetMaterialization], None, None]: A generator of MaterializeResult or AssetMaterialization
+        """
+        # attempt to retrieve params from asset context if not passed as a parameter
+        if not (replication_config or dagster_sling_translator):
+            metadata_by_key = context.assets_def.metadata_by_key
+            first_asset_metadata = next(iter(metadata_by_key.values()))
+            dagster_sling_translator = first_asset_metadata.get(METADATA_KEY_TRANSLATOR)
+            replication_config = first_asset_metadata.get(METADATA_KEY_REPLICATION_CONFIG)
+
+        # if translator has not been defined on metadata _or_ through param, then use the default constructor
+        dagster_sling_translator = dagster_sling_translator or DagsterSlingTranslator()
+
         replication_config = validate_replication(replication_config)
         stream_definition = get_streams_from_replication(replication_config)
 
         with self._setup_config():
             uid = uuid.uuid4()
             temp_dir = tempfile.gettempdir()
             temp_file = os.path.join(temp_dir, f"sling-replication-{uid}.json")
@@ -364,22 +422,29 @@
         for row in results.split("\n"):
             clean_line = self._clean_line(row)
             sys.stdout.write(clean_line + "\n")
             self._stdout.append(clean_line)
 
         end_time = time.time()
 
+        has_asset_def: bool = bool(context and context.has_assets_def)
+
         for stream in stream_definition:
             output_name = dagster_sling_translator.get_asset_key(stream)
-            yield MaterializeResult(
-                asset_key=output_name, metadata={"elapsed_time": end_time - start_time}
-            )
+            if has_asset_def:
+                yield MaterializeResult(
+                    asset_key=output_name, metadata={"elapsed_time": end_time - start_time}
+                )
+            else:
+                yield AssetMaterialization(
+                    asset_key=output_name, metadata={"elapsed_time": end_time - start_time}
+                )
 
     def stream_raw_logs(self) -> Generator[str, None, None]:
-        """Returns the logs from the Sling CLI."""
+        """Returns a generator of raw logs from the Sling CLI."""
         yield from self._stdout
 
 
 def _process_env_vars(config: Dict[str, Any]) -> Dict[str, Any]:
     out = {}
     for key, value in config.items():
         if isinstance(value, dict) and len(value) == 1 and next(iter(value.keys())) == "env":
```

### Comparing `dagster-embedded-elt-0.22.9/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/sling_replication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import lru_cache
 from pathlib import Path
-from typing import Any, Mapping, Union, cast
+from typing import Any, Mapping, Optional, Union, cast
 
 import dagster._check as check
 import yaml
 
 SlingReplicationParam = Union[Mapping[str, Any], str, Path]
 
 
@@ -14,15 +14,16 @@
 
     This function is cached to ensure that we don't read the same path multiple times, which
     creates multiple copies of the parsed manifest in memory.
     """
     return cast(Mapping[str, Any], yaml.safe_load(replication_path.read_bytes()))
 
 
-def validate_replication(replication: SlingReplicationParam) -> Mapping[str, Any]:
+def validate_replication(replication: Optional[SlingReplicationParam]) -> Mapping[str, Any]:
+    replication = replication or {}
     check.inst_param(replication, "manifest", (Path, str, dict))
 
     if isinstance(replication, str):
         replication = Path(replication)
 
     if isinstance(replication, Path):
         # Resolve the path to ensure a consistent key for the cache
```

### Comparing `dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/PKG-INFO` & `dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8,<3.13
+Provides-Extra: test
 License-File: LICENSE
```

### Comparing `dagster-embedded-elt-0.22.9/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 LICENSE
 MANIFEST.in
 README.md
 integration.yaml
 setup.cfg
 setup.py
 dagster_embedded_elt/__init__.py
+dagster_embedded_elt/py.typed
 dagster_embedded_elt/version.py
 dagster_embedded_elt.egg-info/PKG-INFO
 dagster_embedded_elt.egg-info/SOURCES.txt
 dagster_embedded_elt.egg-info/dependency_links.txt
 dagster_embedded_elt.egg-info/not-zip-safe
 dagster_embedded_elt.egg-info/requires.txt
 dagster_embedded_elt.egg-info/top_level.txt
+dagster_embedded_elt/dlt/__init__.py
+dagster_embedded_elt/dlt/asset_decorator.py
+dagster_embedded_elt/dlt/constants.py
+dagster_embedded_elt/dlt/resource.py
+dagster_embedded_elt/dlt/translator.py
 dagster_embedded_elt/sling/__init__.py
 dagster_embedded_elt/sling/asset_decorator.py
 dagster_embedded_elt/sling/asset_defs.py
 dagster_embedded_elt/sling/dagster_sling_translator.py
 dagster_embedded_elt/sling/resources.py
 dagster_embedded_elt/sling/sling_replication.py
```

### Comparing `dagster-embedded-elt-0.22.9/setup.py` & `dagster-embedded-elt-0.23.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,11 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.6.9", "sling>=1.1.5"],
+    install_requires=["dagster==1.7.0", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
-    extras_require={},
+    extras_require={
+        "test": [
+            "duckdb",
+        ]
+    },
 )
```

