# Comparing `tmp/qapp-qiskit-0.0.2.tar.gz` & `tmp/qapp-qiskit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qapp-qiskit-0.0.2.tar", last modified: Wed Apr  3 03:24:41 2024, max compression
+gzip compressed data, was "qapp-qiskit-0.0.3.tar", last modified: Thu Apr  4 07:59:52 2024, max compression
```

## Comparing `qapp-qiskit-0.0.2.tar` & `qapp-qiskit-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.499770 qapp-qiskit-0.0.2/
--rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-qiskit-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2122 2024-04-03 03:24:41.496749 qapp-qiskit-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       28 2024-04-01 04:58:29.000000 qapp-qiskit-0.0.2/README.md
--rw-rw-rw-   0        0        0      910 2024-04-03 03:24:04.000000 qapp-qiskit-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.466766 qapp-qiskit-0.0.2/qapp_qiskit/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:21:11.000000 qapp-qiskit-0.0.2/qapp_qiskit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.473747 qapp-qiskit-0.0.2/qapp_qiskit/async_tasks/
--rw-rw-rw-   0        0        0        0 2024-04-02 16:36:28.000000 qapp-qiskit-0.0.2/qapp_qiskit/async_tasks/__init__.py
--rw-rw-rw-   0        0        0     1037 2024-04-02 16:58:38.000000 qapp-qiskit-0.0.2/qapp_qiskit/async_tasks/qiskit_circuit_export_task.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.474748 qapp-qiskit-0.0.2/qapp_qiskit/component/
--rw-rw-rw-   0        0        0        0 2024-04-02 04:27:31.000000 qapp-qiskit-0.0.2/qapp_qiskit/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.477747 qapp-qiskit-0.0.2/qapp_qiskit/component/backend/
--rw-rw-rw-   0        0        0        0 2024-04-02 04:27:41.000000 qapp-qiskit-0.0.2/qapp_qiskit/component/backend/__init__.py
--rw-rw-rw-   0        0        0     2138 2024-04-02 17:06:54.000000 qapp-qiskit-0.0.2/qapp_qiskit/component/backend/qiskit_invocation.py
--rw-rw-rw-   0        0        0     1377 2024-04-02 17:16:41.000000 qapp-qiskit-0.0.2/qapp_qiskit/component/backend/qiskit_job_fetching.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.481748 qapp-qiskit-0.0.2/qapp_qiskit/factory/
--rw-rw-rw-   0        0        0        0 2024-04-02 03:54:49.000000 qapp-qiskit-0.0.2/qapp_qiskit/factory/__init__.py
--rw-rw-rw-   0        0        0     1360 2024-04-02 16:31:16.000000 qapp-qiskit-0.0.2/qapp_qiskit/factory/qiskit_device_factory.py
--rw-rw-rw-   0        0        0     1218 2024-04-02 07:47:59.000000 qapp-qiskit-0.0.2/qapp_qiskit/factory/qiskit_handler_factory.py
--rw-rw-rw-   0        0        0     1265 2024-04-02 16:09:11.000000 qapp-qiskit-0.0.2/qapp_qiskit/factory/qiskit_provider_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.484747 qapp-qiskit-0.0.2/qapp_qiskit/handler/
--rw-rw-rw-   0        0        0        0 2024-04-02 04:40:46.000000 qapp-qiskit-0.0.2/qapp_qiskit/handler/__init__.py
--rw-rw-rw-   0        0        0     1003 2024-04-02 07:47:59.000000 qapp-qiskit-0.0.2/qapp_qiskit/handler/invocation_handler.py
--rw-rw-rw-   0        0        0      884 2024-04-02 07:47:59.000000 qapp-qiskit-0.0.2/qapp_qiskit/handler/job_fetching_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.486749 qapp-qiskit-0.0.2/qapp_qiskit/model/
--rw-rw-rw-   0        0        0        0 2024-04-02 08:36:03.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.490748 qapp-qiskit-0.0.2/qapp_qiskit/model/device/
--rw-rw-rw-   0        0        0        0 2024-04-02 08:36:32.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/device/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-02 11:27:50.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      821 2024-04-02 11:27:50.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0     1245 2024-04-02 11:27:50.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/device/qapp_qiskit_device.py
--rw-rw-rw-   0        0        0     1693 2024-04-02 11:19:03.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/device/qiskit_device.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.494747 qapp-qiskit-0.0.2/qapp_qiskit/model/provider/
--rw-rw-rw-   0        0        0        0 2024-04-02 08:36:25.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1117 2024-04-02 09:36:01.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      868 2024-04-02 09:02:44.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0     1118 2024-04-02 10:07:07.000000 qapp-qiskit-0.0.2/qapp_qiskit/model/provider/qapp_qiskit_provider.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:24:41.495747 qapp-qiskit-0.0.2/qapp_qiskit.egg-info/
--rw-rw-rw-   0        0        0     2122 2024-04-03 03:24:41.000000 qapp-qiskit-0.0.2/qapp_qiskit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2024-04-03 03:24:41.000000 qapp-qiskit-0.0.2/qapp_qiskit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 03:24:41.000000 qapp-qiskit-0.0.2/qapp_qiskit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-04-03 03:24:41.000000 qapp-qiskit-0.0.2/qapp_qiskit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 03:24:41.000000 qapp-qiskit-0.0.2/qapp_qiskit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 03:24:41.499770 qapp-qiskit-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.509833 qapp-qiskit-0.0.3/
+-rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-qiskit-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2122 2024-04-04 07:59:52.505828 qapp-qiskit-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2024-04-01 04:58:29.000000 qapp-qiskit-0.0.3/README.md
+-rw-rw-rw-   0        0        0      910 2024-04-04 07:59:30.000000 qapp-qiskit-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.408831 qapp-qiskit-0.0.3/qapp_qiskit/
+-rw-rw-rw-   0        0        0       66 2024-04-03 10:52:34.000000 qapp-qiskit-0.0.3/qapp_qiskit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.431829 qapp-qiskit-0.0.3/qapp_qiskit/async_tasks/
+-rw-rw-rw-   0        0        0        0 2024-04-02 16:36:28.000000 qapp-qiskit-0.0.3/qapp_qiskit/async_tasks/__init__.py
+-rw-rw-rw-   0        0        0     1037 2024-04-02 16:58:38.000000 qapp-qiskit-0.0.3/qapp_qiskit/async_tasks/qiskit_circuit_export_task.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.435829 qapp-qiskit-0.0.3/qapp_qiskit/component/
+-rw-rw-rw-   0        0        0        0 2024-04-02 04:27:31.000000 qapp-qiskit-0.0.3/qapp_qiskit/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.444830 qapp-qiskit-0.0.3/qapp_qiskit/component/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-02 04:27:41.000000 qapp-qiskit-0.0.3/qapp_qiskit/component/backend/__init__.py
+-rw-rw-rw-   0        0        0     2363 2024-04-04 06:57:12.000000 qapp-qiskit-0.0.3/qapp_qiskit/component/backend/qiskit_invocation.py
+-rw-rw-rw-   0        0        0     1377 2024-04-02 17:16:41.000000 qapp-qiskit-0.0.3/qapp_qiskit/component/backend/qiskit_job_fetching.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.459829 qapp-qiskit-0.0.3/qapp_qiskit/factory/
+-rw-rw-rw-   0        0        0        0 2024-04-02 03:54:49.000000 qapp-qiskit-0.0.3/qapp_qiskit/factory/__init__.py
+-rw-rw-rw-   0        0        0     1360 2024-04-02 16:31:16.000000 qapp-qiskit-0.0.3/qapp_qiskit/factory/qiskit_device_factory.py
+-rw-rw-rw-   0        0        0     1218 2024-04-02 07:47:59.000000 qapp-qiskit-0.0.3/qapp_qiskit/factory/qiskit_handler_factory.py
+-rw-rw-rw-   0        0        0     1265 2024-04-02 16:09:11.000000 qapp-qiskit-0.0.3/qapp_qiskit/factory/qiskit_provider_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.468829 qapp-qiskit-0.0.3/qapp_qiskit/handler/
+-rw-rw-rw-   0        0        0        0 2024-04-02 04:40:46.000000 qapp-qiskit-0.0.3/qapp_qiskit/handler/__init__.py
+-rw-rw-rw-   0        0        0     1003 2024-04-02 07:47:59.000000 qapp-qiskit-0.0.3/qapp_qiskit/handler/invocation_handler.py
+-rw-rw-rw-   0        0        0      884 2024-04-02 07:47:59.000000 qapp-qiskit-0.0.3/qapp_qiskit/handler/job_fetching_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.471830 qapp-qiskit-0.0.3/qapp_qiskit/model/
+-rw-rw-rw-   0        0        0        0 2024-04-02 08:36:03.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.488829 qapp-qiskit-0.0.3/qapp_qiskit/model/device/
+-rw-rw-rw-   0        0        0        0 2024-04-02 08:36:32.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/device/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-02 11:27:50.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      821 2024-04-02 11:27:50.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0     1245 2024-04-02 11:27:50.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/device/qapp_qiskit_device.py
+-rw-rw-rw-   0        0        0     1693 2024-04-02 11:19:03.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/device/qiskit_device.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.498828 qapp-qiskit-0.0.3/qapp_qiskit/model/provider/
+-rw-rw-rw-   0        0        0        0 2024-04-02 08:36:25.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1117 2024-04-02 09:36:01.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      868 2024-04-02 09:02:44.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0     1118 2024-04-02 10:07:07.000000 qapp-qiskit-0.0.3/qapp_qiskit/model/provider/qapp_qiskit_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:59:52.502827 qapp-qiskit-0.0.3/qapp_qiskit.egg-info/
+-rw-rw-rw-   0        0        0     2122 2024-04-04 07:59:52.000000 qapp-qiskit-0.0.3/qapp_qiskit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2024-04-04 07:59:52.000000 qapp-qiskit-0.0.3/qapp_qiskit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 07:59:52.000000 qapp-qiskit-0.0.3/qapp_qiskit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-04-04 07:59:52.000000 qapp-qiskit-0.0.3/qapp_qiskit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 07:59:52.000000 qapp-qiskit-0.0.3/qapp_qiskit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 07:59:52.509833 qapp-qiskit-0.0.3/setup.cfg
```

### Comparing `qapp-qiskit-0.0.2/LICENSE` & `qapp-qiskit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/PKG-INFO` & `qapp-qiskit-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-qiskit
-Version: 0.0.2
+Version: 0.0.3
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -15,15 +15,15 @@
 Keywords: qapp,qapp-qiskit,quantum
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: qapp-common==0.0.6
+Requires-Dist: qapp-common==0.0.7
 Requires-Dist: qiskit==1.0.2
 Requires-Dist: qiskit-aer-gpu==0.13.3
 Requires-Dist: qiskit-ibm-provider==0.10.0
 Requires-Dist: qiskit-ibm-runtime==0.21.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
```

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/async_tasks/qiskit_circuit_export_task.py` & `qapp-qiskit-0.0.3/qapp_qiskit/async_tasks/qiskit_circuit_export_task.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/component/backend/qiskit_invocation.py` & `qapp-qiskit-0.0.3/qapp_qiskit/component/backend/qiskit_invocation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
     QApp Platform Project qiskit_invocation.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
+from qiskit import QuantumCircuit
 
 from qapp_common.component.backend.invocation import Invocation
 from qapp_common.data.async_task.circuit_export.backend_holder import BackendDataHolder
 from qapp_common.data.async_task.circuit_export.circuit_holder import CircuitDataHolder
 from qapp_common.data.request.invocation_request import InvocationRequest
 from qapp_common.model.provider.provider import Provider
 from qapp_common.config.logging_config import logger
@@ -46,7 +47,13 @@
 
         return QiskitDeviceFactory.create_device(
             provider=provider,
             device_specification=self.backend_information.device_name,
             authentication=self.backend_information.authentication,
             sdk=self.sdk,
         )
+
+    def _get_qubit_amount(self, circuit):
+        if isinstance(circuit, QuantumCircuit):
+            return int(circuit.num_qubits)
+
+        raise Exception("Invalid circuit type!")
```

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/component/backend/qiskit_job_fetching.py` & `qapp-qiskit-0.0.3/qapp_qiskit/component/backend/qiskit_job_fetching.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/factory/qiskit_device_factory.py` & `qapp-qiskit-0.0.3/qapp_qiskit/factory/qiskit_device_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/factory/qiskit_handler_factory.py` & `qapp-qiskit-0.0.3/qapp_qiskit/factory/qiskit_handler_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/factory/qiskit_provider_factory.py` & `qapp-qiskit-0.0.3/qapp_qiskit/factory/qiskit_provider_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/handler/invocation_handler.py` & `qapp-qiskit-0.0.3/qapp_qiskit/handler/invocation_handler.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/handler/job_fetching_handler.py` & `qapp-qiskit-0.0.3/qapp_qiskit/handler/job_fetching_handler.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/model/device/ibm_cloud_device.py` & `qapp-qiskit-0.0.3/qapp_qiskit/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/model/device/ibm_quantum_device.py` & `qapp-qiskit-0.0.3/qapp_qiskit/model/device/ibm_quantum_device.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/model/device/qapp_qiskit_device.py` & `qapp-qiskit-0.0.3/qapp_qiskit/model/device/qapp_qiskit_device.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/model/device/qiskit_device.py` & `qapp-qiskit-0.0.3/qapp_qiskit/model/device/qiskit_device.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/model/provider/ibm_cloud_provider.py` & `qapp-qiskit-0.0.3/qapp_qiskit/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/model/provider/ibm_quantum_provider.py` & `qapp-qiskit-0.0.3/qapp_qiskit/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit/model/provider/qapp_qiskit_provider.py` & `qapp-qiskit-0.0.3/qapp_qiskit/model/provider/qapp_qiskit_provider.py`

 * *Files identical despite different names*

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit.egg-info/PKG-INFO` & `qapp-qiskit-0.0.3/qapp_qiskit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-qiskit
-Version: 0.0.2
+Version: 0.0.3
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -15,15 +15,15 @@
 Keywords: qapp,qapp-qiskit,quantum
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: qapp-common==0.0.6
+Requires-Dist: qapp-common==0.0.7
 Requires-Dist: qiskit==1.0.2
 Requires-Dist: qiskit-aer-gpu==0.13.3
 Requires-Dist: qiskit-ibm-provider==0.10.0
 Requires-Dist: qiskit-ibm-runtime==0.21.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
```

### Comparing `qapp-qiskit-0.0.2/qapp_qiskit.egg-info/SOURCES.txt` & `qapp-qiskit-0.0.3/qapp_qiskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

