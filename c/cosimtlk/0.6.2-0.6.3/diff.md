# Comparing `tmp/cosimtlk-0.6.2.tar.gz` & `tmp/cosimtlk-0.6.3.tar.gz`

## Comparing `cosimtlk-0.6.2.tar` & `cosimtlk-0.6.3.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/Makefile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/__about__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/__init__.py
--rw-r--r--   0        0        0    20686 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/_fmu.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/cli.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/client.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/models.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/__init__.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/client.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/config.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/dependencies.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/main.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/routers/__init__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/routers/fmus.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/routers/simulators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/services/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/services/simulator.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/__init__.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/environment.py
--rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/simulator.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/state.py
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/storage.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/utils.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/__init__.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/base.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/fmu.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/generic.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/input.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/oberver.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/stateobserver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/conftest.py
--rwxr-xr-x   0        0        0   881408 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_fmus/__init__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_fmus/test_local_fmu.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_fmus/test_local_fmu_instance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/__init__.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/test_observation_store.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/test_schedule_store.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/test_state.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/test_utils.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/.gitignore
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/LICENCE
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/README.md
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/Makefile
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/__about__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/__init__.py
+-rw-r--r--   0        0        0    20686 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/_fmu.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/cli.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/client.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/models.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/__init__.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/client.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/config.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/dependencies.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/main.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/routers/__init__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/routers/fmus.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/routers/simulators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/services/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/app/services/simulator.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/__init__.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/environment.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/simulator.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/state.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/storage.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/utils.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/__init__.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/base.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/fmu.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/generic.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/input.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/src/cosimtlk/simulation/entities/stateobserver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/conftest.py
+-rwxr-xr-x   0        0        0   881408 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_fmus/__init__.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_fmus/test_local_fmu.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_fmus/test_local_fmu_instance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/__init__.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/test_observation_store.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/test_schedule_store.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/test_state.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/tests/test_simulation/test_storage/test_utils.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/LICENCE
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/README.md
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 cosimtlk-0.6.3/PKG-INFO
```

### Comparing `cosimtlk-0.6.2/Makefile` & `cosimtlk-0.6.3/Makefile`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/_fmu.py` & `cosimtlk-0.6.3/src/cosimtlk/_fmu.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/cli.py` & `cosimtlk-0.6.3/src/cosimtlk/cli.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/client.py` & `cosimtlk-0.6.3/src/cosimtlk/client.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/app/client.py` & `cosimtlk-0.6.3/src/cosimtlk/app/client.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/app/routers/fmus.py` & `cosimtlk-0.6.3/src/cosimtlk/app/routers/fmus.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/app/routers/simulators.py` & `cosimtlk-0.6.3/src/cosimtlk/app/routers/simulators.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/app/services/simulator.py` & `cosimtlk-0.6.3/src/cosimtlk/app/services/simulator.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/environment.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/environment.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/simulator.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/simulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         self._logger = logger or logging.getLogger(__name__)
 
         # Create simulation environment
         self._environment = Environment(initial_time=initial_timestamp)
         self._state = state
 
         # Add entities to the simulation
-        self._current_process = 0
-        self._process_delays = np.linspace(0.005, 0.995, 10000)
+        self._process_delays = np.arange(0.0005, 0.9995, 0.0005)
         self._entities: dict[str, Entity] = {}
         for entity in entities or []:
             self.add_entity(entity)
 
         # Set additional attributes
         for k, v in kwargs.items():
             setattr(self, k, v)
@@ -68,16 +67,15 @@
         if entity.name in self._entities:
             msg = f"Entity with name {entity.name} already exists."
             raise ValueError(msg)
         self._entities[entity.name] = entity
 
         entity.initialize(self)
         for process in entity.processes:
-            start_delayed(self._environment, process(), float(self._process_delays[self._current_process]))
-            self._current_process += 1
+            start_delayed(self._environment, process(), float(self._process_delays[entity.priority]))
         return self
 
     @property
     def entities(self) -> list[Entity]:
         """The entities inside the simulation."""
         return list(self._entities.values())
```

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/state.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/state.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/storage.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/storage.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/utils.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/base.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,46 +18,46 @@
 
     def log(self, level, msg, *args, **kwargs):
         msg = f"{self.entity.ctx.current_datetime}:{self.entity_name}:{msg}"
         self.logger.log(level, msg, *args, **kwargs)
 
 
 class Entity(metaclass=ABCMeta):
-    def __init__(self, name: str, attributes: dict | None = None) -> None:
+    def __init__(self, name: str, priority: int) -> None:
         """Entity base class that defines the interface for all entities.
 
         Abstract base class for all entities in the simulation. An entity is
         a component that can be scheduled in the simulation environment.
         It must implement the `processes` method that returns a list of
         processes that should be scheduled.
         The order of the processes in the list is the order in which they
         will be scheduled in case they should fire exactly the same time.
 
         Args:
             name: Name of the entity for identification purposes.
-            attributes: Dictionary of attributes that can be used to store.
+            priority: Priority of the entity in task scheduling.
         """
         self._name = name
-        self._attributes = attributes or {}
+        self._priority = priority
         self._context: Simulator | None = None
         self._logger: EntityLogger | None = None
 
     def __repr__(self):
         """Representation of the entity."""
         return f"<{self.__class__.__name__}: {self.name}>"
 
     @property
     def name(self) -> str:
         """Name of the entity."""
         return self._name
 
     @property
-    def attributes(self) -> dict:
-        """Attributes of the entity."""
-        return self._attributes
+    def priority(self) -> int:
+        """Priority of the entity in task scheduling."""
+        return self._priority
 
     @property
     def ctx(self) -> Simulator:
         """Simulation environment."""
         if self._context is None:
             msg = "Entity has not been initialized yet."
             raise RuntimeError(msg)
@@ -141,8 +141,8 @@
     def generate(self):
         for arrival_time in self._generate_interarrival_time():
             timeout = self.wait_for(arrival_time)
             yield timeout
             entity = self.build_entity()
             self._build_count += 1
             self.ctx.add_entity(entity)
-            self.log.debug(f"created entity={entity} with attributes={entity.attributes}")
+            self.log.debug(f"created entity={entity} with priority={entity.priority}")
```

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/fmu.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/fmu.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,33 +13,39 @@
     from cosimtlk.simulation import Simulator
 
 
 class FMUEntity(Entity):
     def __init__(
         self,
         name: str,
+        priority: int,
         *,
         fmu: FMUBase,
         start_values: dict[str, FMUInputType],
         fmu_step_size: int,
         simulation_step_size: int,
-        namespace: str | None = None,
-        input_namespace: str = "inputs",
-        output_namespace: str = "outputs",
     ):
-        super().__init__(name)
+        """An entity that simulates an FMU.
+
+        Args:
+            name: The name of the entity.
+            priority: The priority of the entity in the simulation.
+            fmu: The FMU to simulate.
+            start_values: The initial values of the FMU.
+            fmu_step_size: The step size of the FMU.
+            simulation_step_size: The step size of the simulation.
+        """
+        super().__init__(name, priority)
         self.fmu = fmu
         self.fmu_instance = None
         self.start_values = start_values
         self.fmu_step_size = fmu_step_size
         self.simulation_step_size = simulation_step_size
-
-        self.namespace = namespace or self.name
-        self.input_namespace = namespaced(self.namespace, input_namespace)
-        self.output_namespace = namespaced(self.namespace, output_namespace)
+        self.input_namespace = namespaced(self.name, "inputs")
+        self.output_namespace = namespaced(self.name, "outputs")
 
     @property
     def processes(self) -> list[Callable[[], Generator]]:
         return [self.simulation_process]
 
     def _store_outputs(self, outputs, namespace: str):
         state = {namespaced(namespace, k): v for k, v in outputs.items()}
```

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/generic.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/generic.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 from cosimtlk.simulation.entities import Entity
 
 
 class GenericProcess(Entity):
     def __init__(
         self,
         name: str,
+        priority: int,
         func: Callable,
         *,
         scheduler: Callable,
         **kwargs,
     ):
         """A generic entity that can schedule the given function.
 
         Args:
             name: Name of the controller for identification purposes.
+            priority: Priority of the controller in task scheduling.
             func: The function to be scheduled.
             scheduler: A scheduler function that returns a generator such as 'every' or 'cron' from utils.
         """
-        super().__init__(name)
+        super().__init__(name, priority)
         self.scheduler = scheduler
         self._func = func
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     @property
     def processes(self) -> list[Callable[[], Generator]]:
```

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/input.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/input.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 from pandas import DataFrame, Series
 
 from cosimtlk.simulation.entities import Entity
 
 
 class Input(Entity):
-    def __init__(self, name: str, *, values: Series):
+    def __init__(self, name: str, priority: int, *, values: Series):
         """An entity that sets the input of the simulator based on the input date.
 
         Args:
             name: The name of the entity.
             values: The input data as a Series with a DatetimeIndex.
                 The index of the values is used as the time at which the input is set
         """
-        super().__init__(name)
+        super().__init__(name, priority)
         self.values = values
-        self._state = values.name
         self._index = 0
 
     @property
     def processes(self) -> list[Callable[[], Generator]]:
         return [self.set_inputs_process]
 
     def set_inputs_process(self):
@@ -30,32 +29,33 @@
                 break
 
             current_time = self.ctx.current_datetime
             next_point_at = self.values.index[self._index]
 
             if next_point_at <= current_time:
                 current_value = self.values.iloc[self._index]
-                self.log.debug(f"setting {self._state}={current_value}")
-                self.ctx.state[self._state] = current_value
+                self.log.debug(f"setting {self.values.name}={current_value}")
+                self.ctx.state[self.values.name] = current_value
                 self._index += 1
             else:
                 next_point_in = int((next_point_at - current_time).total_seconds())
                 yield self.wait_for(next_point_in)
 
 
 class MultiInput(Entity):
-    def __init__(self, name: str, *, values: DataFrame):
+    def __init__(self, name: str, priority: int, *, values: DataFrame):
         """An entity that sets the input of the simulator based on the input date.
 
         Args:
             name: The name of the entity.
+            priority: The priority of the entity in the simulation.
             values: The input data as a Series with a DatetimeIndex.
                 The index of the values is used as the time at which the input is set
         """
-        super().__init__(name)
+        super().__init__(name, priority)
         self.values = values
         self._index = 0
 
     @property
     def processes(self) -> list[Callable[[], Generator]]:
         return [self.set_inputs_process]
```

### Comparing `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/stateobserver.py` & `cosimtlk-0.6.3/src/cosimtlk/simulation/entities/stateobserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,30 @@
         object.__setattr__(self, "store_as", self.store_as or self.name)
 
 
 class StateObserver(Entity):
     def __init__(
         self,
         name: str,
+        priority: int,
         *,
         measurements: list[Measurement],
         scheduler: Callable,
     ):
         """An entity that stores the current state of the simulation into long term storage.
 
         Args:
             name: The name of the entity.
+            priority: The priority of the entity in the simulation.
             measurements: A mapping of state names to measurement names. The keys are used as
                 the names of the measurements inside the database, while the values determine the state.
             scheduler: A generator function that schedules a function such as `cosimtlk.simulation.utils.every`
                 or `cosimtlk.simulation.utils.cron`.
         """
-        super().__init__(name)
+        super().__init__(name, priority)
         self.measurements = measurements
         self.scheduler = scheduler
 
     @property
     def processes(self) -> list[Callable[[], Generator]]:
         scheduled_process = self.scheduler(self.__class__.sensing_process)
         return [
```

### Comparing `cosimtlk-0.6.2/tests/conftest.py` & `cosimtlk-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu` & `cosimtlk-0.6.3/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/tests/test_fmus/test_local_fmu.py` & `cosimtlk-0.6.3/tests/test_fmus/test_local_fmu.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/tests/test_fmus/test_local_fmu_instance.py` & `cosimtlk-0.6.3/tests/test_fmus/test_local_fmu_instance.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/tests/test_simulation/test_storage/test_observation_store.py` & `cosimtlk-0.6.3/tests/test_simulation/test_storage/test_observation_store.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/tests/test_simulation/test_storage/test_schedule_store.py` & `cosimtlk-0.6.3/tests/test_simulation/test_storage/test_schedule_store.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/tests/test_simulation/test_storage/test_state.py` & `cosimtlk-0.6.3/tests/test_simulation/test_storage/test_state.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/tests/test_simulation/test_storage/test_utils.py` & `cosimtlk-0.6.3/tests/test_simulation/test_storage/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/.gitignore` & `cosimtlk-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/LICENCE` & `cosimtlk-0.6.3/LICENCE`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/README.md` & `cosimtlk-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/pyproject.toml` & `cosimtlk-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.2/PKG-INFO` & `cosimtlk-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosimtlk
-Version: 0.6.2
+Version: 0.6.3
 Summary: Cosimulation toolkit.
 Project-URL: Homepage, https://github.com/attila-balint-kul/cosimulation-toolkit
 Project-URL: Source, https://github.com/attila-balint-kul/cosimulation-toolkit
 Project-URL: Documentation, https://github.com/attila-balint-kul/cosimulation-toolkit#readme
 Project-URL: Issues, https://github.com/attila-balint-kul/cosimulation-toolkit/issues
 Author-email: Attila Balint <attila.balint@kuleuven.be>
 License-Expression: BSD-3-Clause
```

