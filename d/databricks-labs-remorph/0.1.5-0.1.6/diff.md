# Comparing `tmp/databricks_labs_remorph-0.1.5.tar.gz` & `tmp/databricks_labs_remorph-0.1.6.tar.gz`

## Comparing `databricks_labs_remorph-0.1.5.tar` & `databricks_labs_remorph-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,49 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/__about__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/__init__.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/cli.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/config.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/install.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/coverage/__init__.py
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/coverage/commons.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/helpers/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/helpers/execution_time.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/helpers/file_utils.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/helpers/morph_status.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/helpers/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/intermediate/__init__.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/intermediate/dag.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/intermediate/engine_adapter.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/intermediate/root_tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/reconcile/__init__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/reconcile/execute.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/__init__.py
--rw-r--r--   0        0        0    24579 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/databricks.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/dialect_utils.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/local_expression.py
--rw-r--r--   0        0        0    22031 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/snowflake.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/sql_transpiler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/transpiler/__init__.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/databricks/labs/remorph/transpiler/execute.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/LICENSE
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/NOTICE
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/README.md
--rw-r--r--   0        0        0    26941 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/__about__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/__init__.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/cli.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/config.py
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/install.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/__init__.py
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/commons.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/__init__.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/db_sql.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/execution_time.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/file_utils.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/morph_status.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/__init__.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/dag.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/engine_adapter.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/root_tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/__init__.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/constants.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/execute.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/recon_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/__init__.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/data_source.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/databricks.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/oracle.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/connectors/snowflake.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/__init__.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/base.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/hash_query.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/reconcile/query_builder/threshold_query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/__init__.py
+-rw-r--r--   0        0        0    25157 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/databricks.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/dialect_utils.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/local_expression.py
+-rw-r--r--   0        0        0    22324 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/snowflake.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/sql_transpiler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/transpiler/__init__.py
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/databricks/labs/remorph/transpiler/execute.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/NOTICE
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/README.md
+-rw-r--r--   0        0        0    26918 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.6/PKG-INFO
```

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/cli.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 
 from databricks.labs.blueprint.cli import App
 from databricks.labs.blueprint.entrypoint import get_logger
+from databricks.labs.blueprint.installation import Installation
 from databricks.sdk import WorkspaceClient
 
 from databricks.labs.remorph.config import MorphConfig
 from databricks.labs.remorph.reconcile.execute import recon
 from databricks.labs.remorph.transpiler.execute import morph
 
 remorph = App(__file__)
@@ -25,39 +26,44 @@
     output_folder: str,
     skip_validation: str,
     catalog_name: str,
     schema_name: str,
 ):
     """transpiles source dialect to databricks dialect"""
     logger.info(f"user: {w.current_user.me()}")
+    installation = Installation.current(w, 'remorph')
+    default_config = installation.load(MorphConfig)
+
+    # TODO refactor cli based on the default config
 
     if source.lower() not in {"snowflake", "tsql"}:
         raise_validation_exception(
             f"Error: Invalid value for '--source': '{source}' is not one of 'snowflake', 'tsql'. "
         )
     if not os.path.exists(input_sql) or input_sql in {None, ""}:
         raise_validation_exception(f"Error: Invalid value for '--input_sql': Path '{input_sql}' does not exist.")
     if output_folder == "":
-        output_folder = None
+        output_folder = default_config.output_folder if default_config.output_folder else None
     if skip_validation.lower() not in {"true", "false"}:
         raise_validation_exception(
             f"Error: Invalid value for '--skip_validation': '{skip_validation}' is not one of 'true', 'false'. "
         )
 
+    sdk_config = default_config.sdk_config if default_config.sdk_config else None
     config = MorphConfig(
         source=source.lower(),
         input_sql=input_sql,
         output_folder=output_folder,
         skip_validation=skip_validation.lower() == "true",  # convert to bool
         catalog_name=catalog_name,
         schema_name=schema_name,
-        sdk_config=w.config,
+        sdk_config=sdk_config,
     )
 
-    status = morph(config)
+    status = morph(w, config)
 
     print(json.dumps(status))
 
 
 @remorph.command
 def reconcile(w: WorkspaceClient, recon_conf: str, conn_profile: str, source: str, report: str):
     """reconciles source to databricks datasets"""
```

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/install.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/install.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import logging
 import os
+import time
 import webbrowser
 from datetime import timedelta
 from pathlib import Path
 
 from databricks.labs.blueprint.entrypoint import get_logger
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.installer import InstallState
 from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.blueprint.wheels import ProductInfo
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 from databricks.sdk.retries import retried
+from databricks.sdk.service.sql import (
+    CreateWarehouseRequestWarehouseType,
+    EndpointInfoWarehouseType,
+    SpotInstancePolicy,
+)
 
 from databricks.labs.remorph.__about__ import __version__
 from databricks.labs.remorph.config import MorphConfig
 
 logger = logging.getLogger(__name__)
 
 PRODUCT_INFO = ProductInfo(__file__)
+WAREHOUSE_PREFIX = "Remorph Transpiler Validation"
 
 
 class WorkspaceInstaller:
     def __init__(self, prompts: Prompts, installation: Installation, ws: WorkspaceClient):
         if "DATABRICKS_RUNTIME_VERSION" in os.environ:
             msg = "WorkspaceInstaller is not supposed to be executed in Databricks Runtime"
             raise SystemExit(msg)
@@ -46,46 +53,87 @@
     def configure(self) -> MorphConfig:
         try:
             return self._installation.load(MorphConfig)
         except NotFound as err:
             logger.debug(f"Cannot find previous installation: {err}")
         logger.info("Please answer a couple of questions to configure Remorph")
 
+        # default params
+        catalog_name = "transpiler_test"
+        schema_name = "convertor_test"
+        ws_config = None
+
         source_prompt = self._prompts.choice("Select the source", ["snowflake", "tsql"])
         source = source_prompt.lower()
 
         skip_validation = self._prompts.confirm("Do you want to Skip Validation")
 
-        catalog_name = self._prompts.question("Enter catalog_name")
-
-        try:
-            self._catalog_setup.get(catalog_name)
-        except NotFound:
-            self.setup_catalog(catalog_name)
-
-        schema_name = self._prompts.question("Enter schema_name")
-
-        try:
-            self._catalog_setup.get_schema(f"{catalog_name}.{schema_name}")
-        except NotFound:
-            self.setup_schema(catalog_name, schema_name)
+        if not skip_validation:
+            ws_config = self._configure_runtime()
+            catalog_name = self._prompts.question("Enter catalog_name")
+            try:
+                self._catalog_setup.get(catalog_name)
+            except NotFound:
+                self.setup_catalog(catalog_name)
+
+            schema_name = self._prompts.question("Enter schema_name")
+
+            try:
+                self._catalog_setup.get_schema(f"{catalog_name}.{schema_name}")
+            except NotFound:
+                self.setup_schema(catalog_name, schema_name)
 
         config = MorphConfig(
             source=source,
             skip_validation=skip_validation,
             catalog_name=catalog_name,
             schema_name=schema_name,
-            sdk_config=None,
+            sdk_config=ws_config,
         )
 
         ws_file_url = self._installation.save(config)
         if self._prompts.confirm("Open config file in the browser and continue installing?"):
             webbrowser.open(ws_file_url)
         return config
 
+    def _configure_runtime(self) -> dict[str, str]:
+        if self._prompts.confirm("Do you want to use SQL Warehouse for validation?"):
+            warehouse_id = self._configure_warehouse()
+            return {"warehouse_id": warehouse_id}
+
+        if self._ws.config.cluster_id:
+            logger.info(f"Using cluster {self._ws.config.cluster_id} for validation")
+            return {"cluster": self._ws.config.cluster_id}
+
+        cluster_id = self._prompts.question("Enter a valid cluster_id to proceed")
+        return {"cluster": cluster_id}
+
+    def _configure_warehouse(self):
+        def warehouse_type(_):
+            return _.warehouse_type.value if not _.enable_serverless_compute else "SERVERLESS"
+
+        pro_warehouses = {"[Create new PRO SQL warehouse]": "create_new"} | {
+            f"{_.name} ({_.id}, {warehouse_type(_)}, {_.state.value})": _.id
+            for _ in self._ws.warehouses.list()
+            if _.warehouse_type == EndpointInfoWarehouseType.PRO
+        }
+        warehouse_id = self._prompts.choice_from_dict(
+            "Select PRO or SERVERLESS SQL warehouse to run validation on", pro_warehouses
+        )
+        if warehouse_id == "create_new":
+            new_warehouse = self._ws.warehouses.create(
+                name=f"{WAREHOUSE_PREFIX} {time.time_ns()}",
+                spot_instance_policy=SpotInstancePolicy.COST_OPTIMIZED,
+                warehouse_type=CreateWarehouseRequestWarehouseType.PRO,
+                cluster_size="Small",
+                max_num_clusters=1,
+            )
+            warehouse_id = new_warehouse.id
+        return warehouse_id
+
     @retried(on=[NotFound], timeout=timedelta(minutes=5))
     def setup_catalog(self, catalog_name: str):
         allow_catalog_creation = self._prompts.confirm(
             f"""Catalog {catalog_name} not found.\
                     \nDo you want to create a new one?"""
         )
         if not allow_catalog_creation:
```

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/uninstall.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/uninstall.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/coverage/commons.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/commons.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/helpers/execution_time.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/execution_time.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/helpers/file_utils.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/helpers/file_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/intermediate/dag.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/dag.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/intermediate/engine_adapter.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/engine_adapter.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/intermediate/root_tables.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/intermediate/root_tables.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/databricks.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/databricks.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,45 +82,36 @@
 def _lateral_view(self, expression: exp.Lateral) -> str:
     str_lateral_view = "LATERAL VIEW"
     str_outer = "OUTER"
     str_explode = "EXPLODE("
     str_pfx = f"{str_lateral_view} {str_explode}"
     str_alias = ")"
 
-    for expr, _, _ in expression.walk(bfs=True, prune=lambda *_: False):
-        match expr:
-            case exp.Explode():
-                if expr.key.upper() != "EXPLODE":
-                    continue
-                for node, _, _ in expr.walk(bfs=True, prune=lambda *_: False):
-                    if not isinstance(node, exp.Kwarg):
-                        continue
-                    if not isinstance(node.this, exp.Var):
-                        continue
-
-                    node_name = str(node.this).upper()
-                    match node_name:
-                        case "INPUT":
-                            # Added if block to handle Dynamic variables `${}`
-                            node_expr = f"{node.expression}".replace("@", "$")
-                            if "PARSE_JSON" in node_expr:
-                                node_expr = node_expr.replace("PARSE_JSON", "FROM_JSON")
-                                msg = (
-                                    f"***Warning***: you need to explicitly specify "
-                                    f"`SCHEMA` for column(s) in `{node_expr}`"
-                                )
-                                logger.warning(msg)
-                            str_pfx = str_pfx + node_expr
-                        case "PATH":
-                            str_pfx = str_pfx + f".{node.expression}".replace("'", "").replace('"', "`")
-                        case "OUTER":
-                            str_pfx = str_pfx.replace(str_lateral_view, f"{str_lateral_view} {str_outer}")
-                            # [TODO]: Implement for options: RECURSIVE and MODE
-            case exp.TableAlias():
-                str_alias = str_alias + f" AS {expr.name}"
+    this = expression.args['this']
+    alias = expression.args['alias']
+    # [TODO]: Implement for options: RECURSIVE and MODE
+    # view = expression.args['view']
+    # outer = expression.args['outer']
+    # cross_apply = expression.args['cross_apply']
+    if isinstance(this, exp.Explode):
+        explode_expr = this
+        if isinstance(explode_expr.this, exp.Kwarg):
+            str_pfx = str_pfx + self.sql(explode_expr.this, 'expression')
+            if not isinstance(explode_expr.this.expression, exp.ParseJSON):
+                str_pfx = str_pfx.replace("{", "").replace("}", "")
+
+        for expr in explode_expr.expressions:
+            node = str(expr.this).upper()
+            if node == "PATH":
+                str_pfx = str_pfx + "." + self.sql(expr, 'expression').replace("'", "")
+            if node == "OUTER":
+                str_pfx = str_pfx.replace(str_lateral_view, f"{str_lateral_view} {str_outer}")
+
+        if isinstance(alias, exp.TableAlias):
+            str_alias = str_alias + f" AS {alias.name}"
 
     return self.sql(str_pfx + str_alias)
 
 
 # [TODO] Add more datatype coverage https://docs.databricks.com/sql/language-manual/sql-ref-datatypes.html
 def _datatype_map(self, expression) -> str:
     if expression.this in [exp.DataType.Type.VARCHAR, exp.DataType.Type.NVARCHAR, exp.DataType.Type.CHAR]:
@@ -235,15 +226,16 @@
     """
     Converts `PARSE_JSON` function to `FROM_JSON` function.
     Schema is a mandatory argument for Databricks `FROM_JSON` function
     [FROM_JSON](https://docs.databricks.com/en/sql/language-manual/functions/from_json.html)
     Need to explicitly specify the Schema {<COL_NAME>_SCHEMA} in the current execution environment
     """
     expr_this = self.sql(expr, "this")
-    column = expr_this.replace("'", "").upper()
+    # use column name as prefix or use JSON_COLUMN_SCHEMA when the expression is nested
+    column = expr_this.replace("'", "").upper() if isinstance(expr.this, exp.Column) else "JSON_COLUMN"
     conv_expr = self.func("FROM_JSON", expr_this, f"{{{column}_SCHEMA}}")
     warning_msg = (
         f"***Warning***: you need to explicitly specify `SCHEMA` for `{column}` column in expression: `{conv_expr}`"
     )
     logger.warning(warning_msg)
     return conv_expr
 
@@ -373,14 +365,15 @@
             local_expression.ToObject: rename_func("TO_JSON"),
             exp.ToBase64: rename_func("BASE64"),
             local_expression.ToNumber: _to_number,
             local_expression.UUID: _uuid,
             local_expression.DateTrunc: _parse_date_trunc,
             exp.ApproxQuantile: rename_func("APPROX_PERCENTILE"),
             exp.TimestampTrunc: timestamptrunc_sql,
+            exp.Mod: rename_func("MOD"),
         }
 
         def join_sql(self, expression: exp.Join) -> str:
             """Overwrites `join_sql()` in `sqlglot/generator.py`
             Added logic to handle Lateral View
             """
             op_list = [
@@ -599,7 +592,32 @@
             obj = re.split(r"\s+", expr, maxsplit=2)[0].upper() if expr else ""
             if command in filtered_commands and obj in ignored_objects:
                 return ""
             return f"{command} {expr}"
 
         def currenttimestamp_sql(self, _: exp.CurrentTimestamp) -> str:
             return self.func("CURRENT_TIMESTAMP")
+
+        def update_sql(self, expression: exp.Update) -> str:
+            this = self.sql(expression, "this")
+            set_sql = self.expressions(expression, flat=True)
+            from_sql = self.sql(expression, "from")
+            where_sql = self.sql(expression, "where")
+            returning = self.sql(expression, "returning")
+            order = self.sql(expression, "order")
+            limit = self.sql(expression, "limit")
+
+            if from_sql:
+                from_sql = from_sql.replace("FROM", "USING", 1)
+                where_sql = where_sql.replace("WHERE", "ON")
+
+            if self.RETURNING_END:
+                expression_sql = f"{from_sql}{where_sql}{returning}"
+            else:
+                expression_sql = f"{returning}{from_sql}{where_sql}"
+
+            if from_sql:
+                sql = f"MERGE INTO {this}{expression_sql} WHEN MATCHED THEN UPDATE SET {set_sql}{order}{limit}"
+            else:
+                sql = f"UPDATE {this} SET {set_sql}{expression_sql}{order}{limit}"
+
+            return self.prepend_ctes(expression, sql)
```

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/dialect_utils.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/dialect_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/local_expression.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/local_expression.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/snowflake.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -444,14 +444,18 @@
 
             # iterate through all the tokens if tokens are available
             while self_copy._index < len(self_copy._tokens):
                 self_copy._advance()
                 # get the table alias when FROM token is found
                 if self_copy._match(TokenType.FROM, advance=False):
                     self_copy._advance()  # advance to next token
+                    # break the loop when subquery is found after `FROM` For ex: `FROM (select * from another_table)`
+                    # instead of table name, For ex: `FROM persons p`
+                    if self_copy._match(TokenType.L_PAREN, advance=False):
+                        break
                     self_copy._parse_table_parts()  # parse the table parts
                     table_alias = self_copy._parse_table_alias()  # get to table alias
                     return str(table_alias)
 
             return table_alias
 
         def _json_column_op(self, this, path):
```

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/snow/sql_transpiler.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/snow/sql_transpiler.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/databricks/labs/remorph/transpiler/execute.py` & `databricks_labs_remorph-0.1.6/databricks/labs/remorph/transpiler/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import logging
 import os
 from pathlib import Path
 
+from databricks.sdk import WorkspaceClient
+
 from databricks.labs.remorph.config import MorphConfig
+from databricks.labs.remorph.helpers import db_sql
 from databricks.labs.remorph.helpers.execution_time import timeit
 from databricks.labs.remorph.helpers.file_utils import (
     dir_walk,
     is_sql_file,
     make_dir,
     remove_bom,
 )
 from databricks.labs.remorph.helpers.morph_status import MorphStatus, ValidationError
-from databricks.labs.remorph.helpers.validate import Validate
+from databricks.labs.remorph.helpers.validation import Validator
 from databricks.labs.remorph.snow import dialect_utils
 from databricks.labs.remorph.snow.sql_transpiler import SQLTranspiler
 
 # pylint: disable=unspecified-encoding
 
 logger = logging.getLogger(__name__)
 
 
-def process_file(config: MorphConfig, input_file: str | Path, output_file: str | Path):
+def process_file(config: MorphConfig, validator: Validator, input_file: str | Path, output_file: str | Path):
     source = config.source
-    skip_validation = config.skip_validation
-
     parse_error_list = []
     validate_error_list = []
     no_of_sqls = 0
 
     input_file = Path(input_file)
     output_file = Path(output_file)
 
@@ -40,34 +41,33 @@
     transpiler = SQLTranspiler(source, parse_error_list)  # [TODO] move the object creation outside the loop
     transpiled_sql = transpiler.transpile(sql, str(input_file))
 
     with output_file.open("w") as w:
         for output in transpiled_sql:
             if output:
                 no_of_sqls = no_of_sqls + 1
-                if skip_validation:
+                if config.skip_validation:
                     w.write(output)
                     w.write("\n;\n")
                 else:
-                    validate = Validate(config.sdk_config)
-                    output_string, exception = validate.validate_format_result(config, output)
+                    output_string, exception = validator.validate_format_result(config, output)
                     w.write(output_string)
                     if exception is not None:
                         validate_error_list.append(ValidationError(str(input_file), exception))
             else:
                 warning_message = (
                     f"Skipped a query from file {input_file!s}. "
                     f"Check for unsupported operations related to STREAM, TASK, SESSION etc."
                 )
                 logger.warning(warning_message)
 
     return no_of_sqls, parse_error_list, validate_error_list
 
 
-def process_directory(config: MorphConfig, root: str | Path, base_root: str, files: list[str]):
+def process_directory(config: MorphConfig, validator: Validator, root: str | Path, base_root: str, files: list[str]):
     output_folder = config.output_folder
     parse_error_list = []
     validate_error_list = []
     counter = 0
 
     root = Path(root)
 
@@ -78,98 +78,100 @@
                 output_folder_base = root / "transpiled"
             else:
                 output_folder_base = f'{output_folder.rstrip("/")}/{base_root}'
 
             output_file_name = Path(output_folder_base) / Path(file).name
             make_dir(output_folder_base)
 
-            no_of_sqls, parse_error, validation_error = process_file(config, file, output_file_name)
+            no_of_sqls, parse_error, validation_error = process_file(config, validator, file, output_file_name)
             counter = counter + no_of_sqls
             parse_error_list.extend(parse_error)
             validate_error_list.extend(validation_error)
         else:
             # Only SQL files are processed with extension .sql or .ddl
             pass
 
     return counter, parse_error_list, validate_error_list
 
 
-def process_recursive_dirs(config: MorphConfig):
+def process_recursive_dirs(config: MorphConfig, validator: Validator):
     input_sql = Path(config.input_sql)
     parse_error_list = []
     validate_error_list = []
 
     file_list = []
     counter = 0
     for root, _, files in dir_walk(input_sql):
         base_root = str(root).replace(str(input_sql), "")
         folder = str(input_sql.resolve().joinpath(base_root))
         msg = f"Processing for sqls under this folder: {folder}"
         logger.info(msg)
         file_list.extend(files)
-        no_of_sqls, parse_error, validation_error = process_directory(config, root, base_root, files)
+        no_of_sqls, parse_error, validation_error = process_directory(config, validator, root, base_root, files)
         counter = counter + no_of_sqls
         parse_error_list.extend(parse_error)
         validate_error_list.extend(validation_error)
 
     error_log = parse_error_list + validate_error_list
 
     return MorphStatus(file_list, counter, len(parse_error_list), len(validate_error_list), error_log)
 
 
 @timeit
-def morph(config: MorphConfig):
+def morph(workspace_client: WorkspaceClient, config: MorphConfig):
     """
     Transpiles the SQL queries from one dialect to another.
 
     :param config: The configuration for the morph operation.
+    :param workspace_client: The WorkspaceClient object.
     """
     input_sql = Path(config.input_sql)
     skip_validation = config.skip_validation
     status = []
     result = MorphStatus([], 0, 0, 0, [])
+    validator = None
+    if not config.skip_validation:
+        validator = Validator(db_sql.get_sql_backend(workspace_client, config))
 
     if input_sql.is_file():
         if is_sql_file(input_sql):
             msg = f"Processing for sqls under this file: {input_sql}"
             logger.info(msg)
             if config.output_folder in {None, "None"}:
                 output_folder = input_sql.parent / "transpiled"
             else:
                 output_folder = Path(config.output_folder.rstrip("/"))
 
             make_dir(output_folder)
             output_file = output_folder / input_sql.name
-            no_of_sqls, parse_error, validation_error = process_file(config, input_sql, output_file)
+            no_of_sqls, parse_error, validation_error = process_file(config, validator, input_sql, output_file)
             error_log = parse_error + validation_error
             result = MorphStatus([str(input_sql)], no_of_sqls, len(parse_error), len(validation_error), error_log)
         else:
             msg = f"{input_sql} is not a SQL file."
             logger.warning(msg)
     elif input_sql.is_dir():
-        result = process_recursive_dirs(config)
+        result = process_recursive_dirs(config, validator)
     else:
         msg = f"{input_sql} does not exist."
         logger.error(msg)
         raise FileNotFoundError(msg)
 
     parse_error_count = result.parse_error_count
     validate_error_count = result.validate_error_count
 
     error_list_count = parse_error_count + validate_error_count
-
     if not skip_validation:
         logger.info(f"No of Sql Failed while Validating: {validate_error_count}")
 
+    error_log_file = "None"
     if error_list_count > 0:
         error_log_file = Path.cwd() / f"err_{os.getpid()}.lst"
         with error_log_file.open("a") as e:
             e.writelines(f"{err}\n" for err in result.error_log_list)
-    else:
-        error_log_file = "None"
 
     status.append(
         {
             "total_files_processed": len(result.file_list),
             "total_queries_processed": result.no_of_queries,
             "no_of_sql_failed_while_parsing": parse_error_count,
             "no_of_sql_failed_while_validating": validate_error_count,
```

### Comparing `databricks_labs_remorph-0.1.5/LICENSE` & `databricks_labs_remorph-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/NOTICE` & `databricks_labs_remorph-0.1.6/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/README.md` & `databricks_labs_remorph-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.5/pyproject.toml` & `databricks_labs_remorph-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
-  "databricks-sdk>=0.18,<0.22",
-  "sqlglot==22.4.0",
-  "databricks-labs-blueprint[yaml]>=0.2.3,<0.5.0"
+  "databricks-sdk>=0.18.0",
+  "sqlglot==23.0.1",
+  "databricks-labs-blueprint[yaml]>=0.2.3",
+  "databricks-labs-lsql>=0.2.3",
 ]
 
 [project.urls]
 Documentation = "https://github.com/databrickslabs/remorph"
 Issues = "https://github.com/databrickslabs/remorph/issues"
 Source = "https://github.com/databrickslabs/remorph"
 
@@ -45,15 +46,15 @@
   "pylint-pytest==2.0.0a0",
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-cov>=4.0.0,<5.0.0",
   "black>=23.1.0",
   "ruff>=0.0.243",
   "isort>=2.5.0",
-  "databricks-connect",
+  "databricks-connect"
 ]
 
 [tool.hatch.envs.default.scripts]
 test        = "pytest --cov src --cov-report=xml tests/unit"
 coverage    = "pytest --cov src tests/unit --cov-report=html"
 integration = "pytest --cov src tests/integration --durations 20"
 fmt         = ["isort .",
@@ -128,16 +129,15 @@
 ]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 
 [tool.coverage.report]
-omit = ["src/databricks/labs/remorph/reconcile/*",
-  "src/databricks/labs/remorph/coverage/*",
+omit = ["src/databricks/labs/remorph/coverage/*",
   "src/databricks/labs/remorph/helpers/execution_time.py",
   "__about__.py"]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
```

### Comparing `databricks_labs_remorph-0.1.5/PKG-INFO` & `databricks_labs_remorph-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: databricks-labs-remorph
-Version: 0.1.5
+Version: 0.1.6
 Summary: SQL code converter and data reconcilation tool for accelerating data onboarding to Databricks from EDW, CDW and other ETL sources.
 Project-URL: Documentation, https://github.com/databrickslabs/remorph
 Project-URL: Issues, https://github.com/databrickslabs/remorph/issues
 Project-URL: Source, https://github.com/databrickslabs/remorph
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
-Requires-Dist: databricks-labs-blueprint[yaml]<0.5.0,>=0.2.3
-Requires-Dist: databricks-sdk<0.22,>=0.18
-Requires-Dist: sqlglot==22.4.0
+Requires-Dist: databricks-labs-blueprint[yaml]>=0.2.3
+Requires-Dist: databricks-labs-lsql>=0.2.3
+Requires-Dist: databricks-sdk>=0.18.0
+Requires-Dist: sqlglot==23.0.1
 Description-Content-Type: text/markdown
 
 Databricks Labs Remorph
 ---
 ![Databricks Labs Remorph](docs/remorph-logo.svg)
 
 [![lines of code](https://tokei.rs/b1/github/databrickslabs/remorph)]([https://codecov.io/github/databrickslabs/remorph](https://github.com/databrickslabs/remorph))
```

