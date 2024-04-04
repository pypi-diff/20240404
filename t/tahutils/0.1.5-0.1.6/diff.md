# Comparing `tmp/tahutils-0.1.5.tar.gz` & `tmp/tahutils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahutils-0.1.5.tar", max compression
+gzip compressed data, was "tahutils-0.1.6.tar", max compression
```

## Comparing `tahutils-0.1.5.tar` & `tahutils-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    14198 2024-03-26 15:00:56.791299 tahutils-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     1560 2024-03-26 15:00:56.791299 tahutils-0.1.5/README.md
--rw-r--r--   0        0        0      744 2024-03-26 15:00:56.791299 tahutils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      223 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/__init__.py
--rw-r--r--   0        0        0     2447 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/parse.py
--rw-r--r--   0        0        0     7138 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/spb.py
--rw-r--r--   0        0        0       84 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/tahu/__init__.py
--rw-r--r--   0        0        0     6178 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/tahu/array_packer.py
--rw-r--r--   0        0        0     3008 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/tahu/host_session_establishment.py
--rw-r--r--   0        0        0      140 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/tahu/readme.md
--rw-r--r--   0        0        0    15690 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/tahu/sparkplug_b.py
--rw-r--r--   0        0        0     8621 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/tahu/sparkplug_b_pb2.py
--rw-r--r--   0        0        0        5 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/tahu_version.txt
--rw-r--r--   0        0        0      224 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/types.py
--rw-r--r--   0        0        0     1436 2024-03-26 15:00:56.795299 tahutils-0.1.5/tahutils/utils.py
--rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 tahutils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    14198 2024-04-04 21:19:25.127819 tahutils-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     1560 2024-04-04 21:19:25.127819 tahutils-0.1.6/README.md
+-rw-r--r--   0        0        0      744 2024-04-04 21:19:25.127819 tahutils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      242 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/__init__.py
+-rw-r--r--   0        0        0     2447 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/parse.py
+-rw-r--r--   0        0        0     7782 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/spb.py
+-rw-r--r--   0        0        0       84 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/__init__.py
+-rw-r--r--   0        0        0     6178 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/array_packer.py
+-rw-r--r--   0        0        0     3008 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/host_session_establishment.py
+-rw-r--r--   0        0        0      140 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/readme.md
+-rw-r--r--   0        0        0    15690 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/sparkplug_b.py
+-rw-r--r--   0        0        0     8621 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/sparkplug_b_pb2.py
+-rw-r--r--   0        0        0        5 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu_version.txt
+-rw-r--r--   0        0        0      224 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/types.py
+-rw-r--r--   0        0        0     1436 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/utils.py
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 tahutils-0.1.6/PKG-INFO
```

### Comparing `tahutils-0.1.5/LICENSE.txt` & `tahutils-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.5/README.md` & `tahutils-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.5/pyproject.toml` & `tahutils-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tahutils"
-version = "0.1.5"
+version = "0.1.6"
 description = "Python utilities for Tahu & Sparkplug B."
 authors = ["Justin Dula <justin.dula@intellicintegration.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
     "Operating System :: OS Independent",
```

### Comparing `tahutils-0.1.5/tahutils/parse.py` & `tahutils-0.1.6/tahutils/parse.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.5/tahutils/spb.py` & `tahutils-0.1.6/tahutils/spb.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from functools import cached_property
 from typing import Optional, Union
 
 from tahutils.tahu import sparkplug_b as spb
 from tahutils.types import MetricName, MetricTimes, MetricValues
 from tahutils.utils import convert_enum_keys, flatten_data_dict, process_times
 
-COMMAND_METRICS = {
-	"Node Control/Next Server", 
-	"Node Control/Rebirth", 
-	"Node Control/Reboot"
-}
+class CommandMetric(Enum):
+	NextServer = "Node Control/Next Server"
+	Rebirth = "Node Control/Rebirth"
+	Reboot = "Node Control/Reboot"
+
+COMMAND_METRICS_SET = {m.value for m in CommandMetric}
 
 class SpbModel:
 	def __init__(
 			self, 
 			metrics: dict[MetricName, spb.MetricDataType], 
 			use_aliases: bool=False, 
 			auto_serialize: bool=True,
@@ -24,37 +25,43 @@
 			flattened_dict_delimiter: str = "/"
 		) -> None:
 		self.flatten_states = flatten_states
 		self.flattened_dict_delimiter = flattened_dict_delimiter
 
 		metrics = self._preprocess_dict(metrics)
 		self.metrics = set(metrics.keys())
-		self.metric_types = {k:v for k,v in metrics.items()} | {m: spb.MetricDataType.Boolean for m in COMMAND_METRICS}
+		self.metric_types = {k:v for k,v in metrics.items()} | {m: spb.MetricDataType.Boolean for m in COMMAND_METRICS_SET}
 
 		self.current_values = {}
 
 		self._use_aliases = use_aliases
-		self.all_metrics = COMMAND_METRICS | self.metrics
+		self.all_metrics = COMMAND_METRICS_SET | self.metrics
 		self._metric_to_alias = {metric: i for i, metric in enumerate(self.all_metrics)} \
 			if self._use_aliases else \
 			{metric: None for metric in self.all_metrics}
 		
 		self._alias_to_metric = {i: metric for i, metric in self._metric_to_alias.items()} \
 			if self._use_aliases else None
 
 		self.auto_serialize = auto_serialize
 		self.serialize_cast = serialize_cast
 
-
 		self.node_death_requested = False
 
+		self._last_death = None
+
 	@property
 	def aliasing(self) -> bool:
 		"""Returns whether aliases are being used"""
 		return self._use_aliases
+	
+	@property
+	def last_death(self) -> bytes:
+		"""Returns the last death payload generated by the model"""
+		return self._last_death
 
 	def _preprocess_dict(self, state: MetricValues, is_time: bool = False) -> MetricValues:
 		"""Preprocesses the state, flattening it if enabled, and converting enum keys. Can optionally preprocess times."""
 		r = flatten_data_dict(state, delimiter=self.flattened_dict_delimiter) if self.flatten_states else convert_enum_keys(state)
 		if is_time:
 			r = process_times(r)
 		return r
@@ -80,29 +87,30 @@
 				return self.serialize_cast(p.SerializeToString())
 			return p.SerializeToString()
 		return p
 	
 	def getNodeDeathPayload(self):
 		"""Returns a death payload for the node. This must be requested and sent as part of the connection."""
 		self.node_death_requested = True
-		return self._serialize(spb.getNodeDeathPayload())
-
+		self._last_death = self._serialize(spb.getNodeDeathPayload())
+		return self._last_death
+	
 	def getNodeBirthPayload(self, state: MetricValues, times: MetricTimes = dict(), ignore_missing_node_death: bool = False):
 		"""Returns a birth payload for the given state. State must be set for all metrics. Times can be set for specific metrics, if desired."""
 		state = self._preprocess_dict(state)
 		times = self._preprocess_dict(times, is_time=True)
 		
 		if not ignore_missing_node_death and not self.node_death_requested:
 			raise ValueError("Must request death before requesting new birth")
-		if set(COMMAND_METRICS | state.keys()) != set(self.all_metrics):
+		if set(COMMAND_METRICS_SET | state.keys()) != set(self.all_metrics):
 			raise ValueError("Node birth metrics must be the same as the model's metrics")
 
 		payload = spb.getNodeBirthPayload()
 
-		for metric in COMMAND_METRICS:
+		for metric in COMMAND_METRICS_SET:
 			if metric not in state:
 				state[metric] = False
 
 		for metric, value in state.items():
 			mt = self.metric_types[metric]
 
 			self.current_values[metric] = value
@@ -151,14 +159,23 @@
 			if self.device_id else \
 			f"{self.namespace}/{self.group_id}/%s/{self.edge_node_id}"
 
 	def construct(self, mtype: str):
 		"""Constructs a Sparkplug B topic for the given message type. If a device_id is set, it will be included in the topic."""
 		mtype = mtype.upper()
 		return self.template_string % mtype
+	
+	def construct_device_topic(self, device_id: Optional[str]):
+		"""Constructs and returns an SpbTopic from this one with the given device_id. Can pass `None` to remove the device_id."""
+		return SpbTopic(
+			group_id=self.group_id,
+			edge_node_id=self.edge_node_id,
+			device_id=device_id,
+			namespace=self.namespace
+		)
 
 	@cached_property
 	def nbirth(self):
 		return self.construct("NBIRTH")
 	
 	@cached_property
 	def NBIRTH(self):
```

### Comparing `tahutils-0.1.5/tahutils/tahu/array_packer.py` & `tahutils-0.1.6/tahutils/tahu/array_packer.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.5/tahutils/tahu/host_session_establishment.py` & `tahutils-0.1.6/tahutils/tahu/host_session_establishment.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.5/tahutils/tahu/sparkplug_b.py` & `tahutils-0.1.6/tahutils/tahu/sparkplug_b.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.5/tahutils/tahu/sparkplug_b_pb2.py` & `tahutils-0.1.6/tahutils/tahu/sparkplug_b_pb2.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.5/tahutils/utils.py` & `tahutils-0.1.6/tahutils/utils.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.5/PKG-INFO` & `tahutils-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahutils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python utilities for Tahu & Sparkplug B.
 Author: Justin Dula
 Author-email: justin.dula@intellicintegration.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

