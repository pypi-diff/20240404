# Comparing `tmp/cosimtlk-0.6.3.tar.gz` & `tmp/cosimtlk-0.6.4.tar.gz`

## Comparing `cosimtlk-0.6.3.tar` & `cosimtlk-0.6.4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/Makefile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/__about__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/__init__.py
--rw-r--r--   0        0        0    20686 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/_fmu.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/cli.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/client.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/models.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/__init__.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/client.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/config.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/dependencies.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/main.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/routers/__init__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/routers/fmus.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/routers/simulators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/services/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/services/simulator.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/__init__.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/environment.py
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/simulator.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/state.py
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/storage.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/utils.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/__init__.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/base.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/fmu.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/generic.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/input.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/stateobserver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/__init__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/conftest.py
--rwxr-xr-x   0        0        0   881408 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_fmus/__init__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_fmus/test_local_fmu.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_fmus/test_local_fmu_instance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/__init__.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/test_observation_store.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/test_schedule_store.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/test_state.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/test_utils.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/.gitignore
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/LICENCE
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/README.md
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/Makefile
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/__about__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/__init__.py
+-rw-r--r--   0        0        0    20686 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/_fmu.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/cli.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/client.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/models.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/__init__.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/client.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/config.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/dependencies.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/main.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/routers/__init__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/routers/fmus.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/routers/simulators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/services/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/app/services/simulator.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/__init__.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/environment.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/simulator.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/state.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/storage.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/utils.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/entities/__init__.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/entities/base.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/entities/fmu.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/entities/generic.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/entities/input.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/entities/source.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/src/cosimtlk/simulation/entities/stateobserver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/conftest.py
+-rwxr-xr-x   0        0        0   881408 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_fmus/__init__.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_fmus/test_local_fmu.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_fmus/test_local_fmu_instance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_simulation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_simulation/test_storage/__init__.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_simulation/test_storage/test_observation_store.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_simulation/test_storage/test_schedule_store.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_simulation/test_storage/test_state.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/tests/test_simulation/test_storage/test_utils.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/LICENCE
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/README.md
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 cosimtlk-0.6.4/PKG-INFO
```

### Comparing `cosimtlk-0.6.3/Makefile` & `cosimtlk-0.6.4/Makefile`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/_fmu.py` & `cosimtlk-0.6.4/src/cosimtlk/_fmu.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/cli.py` & `cosimtlk-0.6.4/src/cosimtlk/cli.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/client.py` & `cosimtlk-0.6.4/src/cosimtlk/client.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/app/client.py` & `cosimtlk-0.6.4/src/cosimtlk/app/client.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/app/routers/fmus.py` & `cosimtlk-0.6.4/src/cosimtlk/app/routers/fmus.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/app/routers/simulators.py` & `cosimtlk-0.6.4/src/cosimtlk/app/routers/simulators.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/app/services/simulator.py` & `cosimtlk-0.6.4/src/cosimtlk/app/services/simulator.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/environment.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/environment.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/simulator.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/state.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/state.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/storage.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/storage.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/utils.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/fmu.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/entities/fmu.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/generic.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/entities/generic.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/input.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/entities/input.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/stateobserver.py` & `cosimtlk-0.6.4/src/cosimtlk/simulation/entities/stateobserver.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/tests/conftest.py` & `cosimtlk-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu` & `cosimtlk-0.6.4/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/tests/test_fmus/test_local_fmu.py` & `cosimtlk-0.6.4/tests/test_fmus/test_local_fmu.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/tests/test_fmus/test_local_fmu_instance.py` & `cosimtlk-0.6.4/tests/test_fmus/test_local_fmu_instance.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/tests/test_simulation/test_storage/test_observation_store.py` & `cosimtlk-0.6.4/tests/test_simulation/test_storage/test_observation_store.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/tests/test_simulation/test_storage/test_schedule_store.py` & `cosimtlk-0.6.4/tests/test_simulation/test_storage/test_schedule_store.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/tests/test_simulation/test_storage/test_state.py` & `cosimtlk-0.6.4/tests/test_simulation/test_storage/test_state.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/tests/test_simulation/test_storage/test_utils.py` & `cosimtlk-0.6.4/tests/test_simulation/test_storage/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/.gitignore` & `cosimtlk-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/LICENCE` & `cosimtlk-0.6.4/LICENCE`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/README.md` & `cosimtlk-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/pyproject.toml` & `cosimtlk-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.3/PKG-INFO` & `cosimtlk-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosimtlk
-Version: 0.6.3
+Version: 0.6.4
 Summary: Cosimulation toolkit.
 Project-URL: Homepage, https://github.com/attila-balint-kul/cosimulation-toolkit
 Project-URL: Source, https://github.com/attila-balint-kul/cosimulation-toolkit
 Project-URL: Documentation, https://github.com/attila-balint-kul/cosimulation-toolkit#readme
 Project-URL: Issues, https://github.com/attila-balint-kul/cosimulation-toolkit/issues
 Author-email: Attila Balint <attila.balint@kuleuven.be>
 License-Expression: BSD-3-Clause
```

