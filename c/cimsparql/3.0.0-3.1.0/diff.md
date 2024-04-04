# Comparing `tmp/cimsparql-3.0.0.tar.gz` & `tmp/cimsparql-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cimsparql-3.0.0.tar", max compression
+gzip compressed data, was "cimsparql-3.1.0.tar", max compression
```

## Comparing `cimsparql-3.0.0.tar` & `cimsparql-3.1.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1065 2024-03-19 07:08:04.061572 cimsparql-3.0.0/LICENSE
--rw-r--r--   0        0        0     5330 2024-03-19 07:08:04.061572 cimsparql-3.0.0/README.md
--rw-r--r--   0        0        0       61 2024-03-19 07:08:22.853525 cimsparql-3.0.0/cimsparql/__init__.py
--rw-r--r--   0        0        0     4263 2024-03-19 07:08:04.061572 cimsparql-3.0.0/cimsparql/adaptions.py
--rw-r--r--   0        0        0     1642 2024-03-19 07:08:04.061572 cimsparql-3.0.0/cimsparql/constants.py
--rw-r--r--   0        0        0     9685 2024-03-19 07:08:04.061572 cimsparql-3.0.0/cimsparql/data_models.py
--rw-r--r--   0        0        0    15619 2024-03-19 07:08:04.061572 cimsparql-3.0.0/cimsparql/graphdb.py
--rw-r--r--   0        0        0    28348 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/model.py
--rw-r--r--   0        0        0     5202 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/ac_lines.sparql
--rw-r--r--   0        0        0      221 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/add_mrid.sparql
--rw-r--r--   0        0        0     1761 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/borders.sparql
--rw-r--r--   0        0        0     2073 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/branch_node_withdraw.sparql
--rw-r--r--   0        0        0     1795 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/bus.sparql
--rw-r--r--   0        0        0      984 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/connections.sparql
--rw-r--r--   0        0        0     1291 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/connectivity_nodes.sparql
--rw-r--r--   0        0        0      737 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/converter_hvdc_bidzones.sparql
--rw-r--r--   0        0        0     2337 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/converters.sparql
--rw-r--r--   0        0        0      588 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/coordinates.sparql
--rw-r--r--   0        0        0     2521 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/dc_active_power_flow.sparql
--rw-r--r--   0        0        0      242 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/disconnected.sparql
--rw-r--r--   0        0        0     3063 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/exchange.sparql
--rw-r--r--   0        0        0      792 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/full_model.sparql
--rw-r--r--   0        0        0     2813 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/loads.sparql
--rw-r--r--   0        0        0      287 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/market_dates.sparql
--rw-r--r--   0        0        0      523 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/power_flow.sparql
--rw-r--r--   0        0        0      397 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/ras_equipment.sparql
--rw-r--r--   0        0        0      573 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/regions.sparql
--rw-r--r--   0        0        0     3655 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/series_compensators.sparql
--rw-r--r--   0        0        0      426 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/station_group_code_and_names.sparql
--rw-r--r--   0        0        0      645 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/substation_voltage_level.sparql
--rw-r--r--   0        0        0     2877 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/sv_branch.sparql
--rw-r--r--   0        0        0      245 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/sv_injection.sparql
--rw-r--r--   0        0        0      781 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/switches.sparql
--rw-r--r--   0        0        0     2725 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/synchronous_machines.sparql
--rw-r--r--   0        0        0      318 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
--rw-r--r--   0        0        0     3102 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/three_winding.sparql
--rw-r--r--   0        0        0     1953 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/three_winding_dummy_nodes.sparql
--rw-r--r--   0        0        0     1583 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/three_winding_loss.sparql
--rw-r--r--   0        0        0      363 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/transformer_windings.sparql
--rw-r--r--   0        0        0     1269 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/transformers.sparql
--rw-r--r--   0        0        0     1844 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/transformers_connected_to_converter.sparql
--rw-r--r--   0        0        0     4520 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/two_winding_transformer.sparql
--rw-r--r--   0        0        0     1049 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/two_winding_transformer_angle.sparql
--rw-r--r--   0        0        0      461 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/type_mapper.sparql
--rw-r--r--   0        0        0      814 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/wind_generating_units.sparql
--rw-r--r--   0        0        0      944 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql/winding.sparql
--rw-r--r--   0        0        0     2181 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/sparql_result_json.py
--rw-r--r--   0        0        0     3193 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/templates.py
--rw-r--r--   0        0        0     5510 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/type_mapper.py
--rw-r--r--   0        0        0     1878 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/url.py
--rw-r--r--   0        0        0      626 2024-03-19 07:08:04.065572 cimsparql-3.0.0/cimsparql/value_mapper.py
--rw-r--r--   0        0        0      459 2024-03-19 07:08:04.073572 cimsparql-3.0.0/pkg_data/blazegraph_repo_config.xml
--rw-r--r--   0        0        0      676 2024-03-19 07:08:04.073572 cimsparql-3.0.0/pkg_data/namespaces.json
--rw-r--r--   0        0        0      805 2024-03-19 07:08:04.073572 cimsparql-3.0.0/pkg_data/native_store_config_template.ttl
--rw-r--r--   0        0        0     4357 2024-03-19 07:08:22.853525 cimsparql-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     6104 1970-01-01 00:00:00.000000 cimsparql-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-04 07:57:55.454210 cimsparql-3.1.0/LICENSE
+-rw-r--r--   0        0        0     5330 2024-04-04 07:57:55.454210 cimsparql-3.1.0/README.md
+-rw-r--r--   0        0        0       61 2024-04-04 07:58:15.114306 cimsparql-3.1.0/cimsparql/__init__.py
+-rw-r--r--   0        0        0     4263 2024-04-04 07:57:55.454210 cimsparql-3.1.0/cimsparql/adaptions.py
+-rw-r--r--   0        0        0     1642 2024-04-04 07:57:55.454210 cimsparql-3.1.0/cimsparql/constants.py
+-rw-r--r--   0        0        0     9685 2024-04-04 07:57:55.454210 cimsparql-3.1.0/cimsparql/data_models.py
+-rw-r--r--   0        0        0    15697 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/graphdb.py
+-rw-r--r--   0        0        0    28348 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/model.py
+-rw-r--r--   0        0        0     5202 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/ac_lines.sparql
+-rw-r--r--   0        0        0      221 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/add_mrid.sparql
+-rw-r--r--   0        0        0     1761 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/borders.sparql
+-rw-r--r--   0        0        0     2073 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/branch_node_withdraw.sparql
+-rw-r--r--   0        0        0     1795 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/bus.sparql
+-rw-r--r--   0        0        0      984 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/connections.sparql
+-rw-r--r--   0        0        0     1291 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/connectivity_nodes.sparql
+-rw-r--r--   0        0        0      737 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/converter_hvdc_bidzones.sparql
+-rw-r--r--   0        0        0     2337 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/converters.sparql
+-rw-r--r--   0        0        0      588 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/coordinates.sparql
+-rw-r--r--   0        0        0     2521 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/dc_active_power_flow.sparql
+-rw-r--r--   0        0        0      242 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/disconnected.sparql
+-rw-r--r--   0        0        0     3063 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/exchange.sparql
+-rw-r--r--   0        0        0      792 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/full_model.sparql
+-rw-r--r--   0        0        0     2813 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/loads.sparql
+-rw-r--r--   0        0        0      287 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/market_dates.sparql
+-rw-r--r--   0        0        0      523 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/power_flow.sparql
+-rw-r--r--   0        0        0      397 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/ras_equipment.sparql
+-rw-r--r--   0        0        0      573 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/regions.sparql
+-rw-r--r--   0        0        0     3655 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/series_compensators.sparql
+-rw-r--r--   0        0        0      426 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/station_group_code_and_names.sparql
+-rw-r--r--   0        0        0      645 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/substation_voltage_level.sparql
+-rw-r--r--   0        0        0     2877 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/sv_branch.sparql
+-rw-r--r--   0        0        0      245 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/sv_injection.sparql
+-rw-r--r--   0        0        0      781 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/switches.sparql
+-rw-r--r--   0        0        0     2725 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/synchronous_machines.sparql
+-rw-r--r--   0        0        0      318 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
+-rw-r--r--   0        0        0     3102 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/three_winding.sparql
+-rw-r--r--   0        0        0     1953 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/three_winding_dummy_nodes.sparql
+-rw-r--r--   0        0        0     1583 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/three_winding_loss.sparql
+-rw-r--r--   0        0        0      363 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/transformer_windings.sparql
+-rw-r--r--   0        0        0     1269 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/transformers.sparql
+-rw-r--r--   0        0        0     1844 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/transformers_connected_to_converter.sparql
+-rw-r--r--   0        0        0     4520 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/two_winding_transformer.sparql
+-rw-r--r--   0        0        0     1049 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/two_winding_transformer_angle.sparql
+-rw-r--r--   0        0        0      461 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/type_mapper.sparql
+-rw-r--r--   0        0        0      814 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/wind_generating_units.sparql
+-rw-r--r--   0        0        0      944 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql/winding.sparql
+-rw-r--r--   0        0        0     2181 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/sparql_result_json.py
+-rw-r--r--   0        0        0     3193 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/templates.py
+-rw-r--r--   0        0        0     5510 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/type_mapper.py
+-rw-r--r--   0        0        0     1878 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/url.py
+-rw-r--r--   0        0        0      626 2024-04-04 07:57:55.458211 cimsparql-3.1.0/cimsparql/value_mapper.py
+-rw-r--r--   0        0        0      459 2024-04-04 07:57:55.466210 cimsparql-3.1.0/pkg_data/blazegraph_repo_config.xml
+-rw-r--r--   0        0        0      676 2024-04-04 07:57:55.466210 cimsparql-3.1.0/pkg_data/namespaces.json
+-rw-r--r--   0        0        0      805 2024-04-04 07:57:55.466210 cimsparql-3.1.0/pkg_data/native_store_config_template.ttl
+-rw-r--r--   0        0        0     4357 2024-04-04 07:58:15.114306 cimsparql-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6104 1970-01-01 00:00:00.000000 cimsparql-3.1.0/PKG-INFO
```

### Comparing `cimsparql-3.0.0/LICENSE` & `cimsparql-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/README.md` & `cimsparql-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/adaptions.py` & `cimsparql-3.1.0/cimsparql/adaptions.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/constants.py` & `cimsparql-3.1.0/cimsparql/constants.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/data_models.py` & `cimsparql-3.1.0/cimsparql/data_models.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/graphdb.py` & `cimsparql-3.1.0/cimsparql/graphdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,17 +160,18 @@
 
     x_correlation_id = "x-correlation-id"
 
     def __init__(
         self,
         service_cfg: ServiceConfig | None = None,
         custom_headers: dict[str, str] | None = None,
+        sparql_wrapper: SPARQLWrapper | None = None,
     ) -> None:
         self.service_cfg = service_cfg or ServiceConfig()
-        self.sparql = self.create_sparql_wrapper()
+        self.sparql = sparql_wrapper or SPARQLWrapper(self.service_cfg.url)
         self.sparql.setReturnFormat(JSON)
         self.sparql.setMethod(POST)
         self.sparql.setCredentials(self.service_cfg.user, self.service_cfg.passwd)
         if self.service_cfg.timeout:
             self.sparql.setTimeout(self.service_cfg.timeout)
         self._update_sparql_parameters()
         if custom_headers:
```

### Comparing `cimsparql-3.0.0/cimsparql/model.py` & `cimsparql-3.1.0/cimsparql/model.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/ac_lines.sparql` & `cimsparql-3.1.0/cimsparql/sparql/ac_lines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/borders.sparql` & `cimsparql-3.1.0/cimsparql/sparql/borders.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/branch_node_withdraw.sparql` & `cimsparql-3.1.0/cimsparql/sparql/branch_node_withdraw.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/bus.sparql` & `cimsparql-3.1.0/cimsparql/sparql/bus.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/connections.sparql` & `cimsparql-3.1.0/cimsparql/sparql/connections.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/connectivity_nodes.sparql` & `cimsparql-3.1.0/cimsparql/sparql/connectivity_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/converter_hvdc_bidzones.sparql` & `cimsparql-3.1.0/cimsparql/sparql/converter_hvdc_bidzones.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/converters.sparql` & `cimsparql-3.1.0/cimsparql/sparql/converters.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/coordinates.sparql` & `cimsparql-3.1.0/cimsparql/sparql/coordinates.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/dc_active_power_flow.sparql` & `cimsparql-3.1.0/cimsparql/sparql/dc_active_power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/exchange.sparql` & `cimsparql-3.1.0/cimsparql/sparql/exchange.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/full_model.sparql` & `cimsparql-3.1.0/cimsparql/sparql/full_model.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/loads.sparql` & `cimsparql-3.1.0/cimsparql/sparql/loads.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/power_flow.sparql` & `cimsparql-3.1.0/cimsparql/sparql/power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/regions.sparql` & `cimsparql-3.1.0/cimsparql/sparql/regions.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/series_compensators.sparql` & `cimsparql-3.1.0/cimsparql/sparql/series_compensators.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/substation_voltage_level.sparql` & `cimsparql-3.1.0/cimsparql/sparql/substation_voltage_level.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/sv_branch.sparql` & `cimsparql-3.1.0/cimsparql/sparql/sv_branch.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/switches.sparql` & `cimsparql-3.1.0/cimsparql/sparql/switches.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/synchronous_machines.sparql` & `cimsparql-3.1.0/cimsparql/sparql/synchronous_machines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/three_winding.sparql` & `cimsparql-3.1.0/cimsparql/sparql/three_winding.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/three_winding_dummy_nodes.sparql` & `cimsparql-3.1.0/cimsparql/sparql/three_winding_dummy_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/three_winding_loss.sparql` & `cimsparql-3.1.0/cimsparql/sparql/three_winding_loss.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/transformers.sparql` & `cimsparql-3.1.0/cimsparql/sparql/transformers.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/transformers_connected_to_converter.sparql` & `cimsparql-3.1.0/cimsparql/sparql/transformers_connected_to_converter.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/two_winding_transformer.sparql` & `cimsparql-3.1.0/cimsparql/sparql/two_winding_transformer.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/two_winding_transformer_angle.sparql` & `cimsparql-3.1.0/cimsparql/sparql/two_winding_transformer_angle.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/wind_generating_units.sparql` & `cimsparql-3.1.0/cimsparql/sparql/wind_generating_units.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql/winding.sparql` & `cimsparql-3.1.0/cimsparql/sparql/winding.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/sparql_result_json.py` & `cimsparql-3.1.0/cimsparql/sparql_result_json.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/templates.py` & `cimsparql-3.1.0/cimsparql/templates.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/type_mapper.py` & `cimsparql-3.1.0/cimsparql/type_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/url.py` & `cimsparql-3.1.0/cimsparql/url.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/cimsparql/value_mapper.py` & `cimsparql-3.1.0/cimsparql/value_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/pkg_data/namespaces.json` & `cimsparql-3.1.0/pkg_data/namespaces.json`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/pkg_data/native_store_config_template.ttl` & `cimsparql-3.1.0/pkg_data/native_store_config_template.ttl`

 * *Files identical despite different names*

### Comparing `cimsparql-3.0.0/pyproject.toml` & `cimsparql-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cimsparql"
-version = "3.0.0"
+version = "3.1.0"
 description = "CIM query utilities"
 readme = "README.md"
 authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>"]
 repository = "https://github.com/statnett/cimsparql.git"
 include = ["pkg_data/*"]
 exclude = ["tests/*"]
```

### Comparing `cimsparql-3.0.0/PKG-INFO` & `cimsparql-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cimsparql
-Version: 3.0.0
+Version: 3.1.0
 Summary: CIM query utilities
 Home-page: https://github.com/statnett/cimsparql.git
 Author: Statnett Datascience
 Author-email: Datascience.Drift@Statnett.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

