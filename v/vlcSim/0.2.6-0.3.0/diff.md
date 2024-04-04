# Comparing `tmp/vlcSim-0.2.6.tar.gz` & `tmp/vlcSim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlcSim-0.2.6.tar", last modified: Thu Mar 28 17:02:36 2024, max compression
+gzip compressed data, was "vlcSim-0.3.0.tar", last modified: Thu Apr  4 17:07:24 2024, max compression
```

## Comparing `vlcSim-0.2.6.tar` & `vlcSim-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:02:36.330506 vlcSim-0.2.6/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-03-28 17:02:25.000000 vlcSim-0.2.6/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     4634 2024-03-28 17:02:36.330506 vlcSim-0.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4152 2024-03-28 17:02:25.000000 vlcSim-0.2.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 17:02:36.330506 vlcSim-0.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-28 17:02:25.000000 vlcSim-0.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:02:36.328506 vlcSim-0.2.6/test/
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-03-28 17:02:25.000000 vlcSim-0.2.6/test/test_receiver.py
--rw-rw-rw-   0 root         (0) root         (0)     4389 2024-03-28 17:02:25.000000 vlcSim-0.2.6/test/test_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-03-28 17:02:25.000000 vlcSim-0.2.6/test/test_vled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:02:36.329506 vlcSim-0.2.6/vlcSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4634 2024-03-28 17:02:36.000000 vlcSim-0.2.6/vlcSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      345 2024-03-28 17:02:36.000000 vlcSim-0.2.6/vlcSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 17:02:36.000000 vlcSim-0.2.6/vlcSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 17:02:36.000000 vlcSim-0.2.6/vlcSim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-28 17:02:36.000000 vlcSim-0.2.6/vlcSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-28 17:02:36.000000 vlcSim-0.2.6/vlcSim.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:02:36.330506 vlcSim-0.2.6/vlcsim/
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-03-28 17:02:25.000000 vlcSim-0.2.6/vlcsim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16654 2024-03-28 17:02:25.000000 vlcSim-0.2.6/vlcsim/controller.py
--rw-rw-rw-   0 root         (0) root         (0)    25100 2024-03-28 17:02:25.000000 vlcSim-0.2.6/vlcsim/scene.py
--rw-rw-rw-   0 root         (0) root         (0)    19981 2024-03-28 17:02:25.000000 vlcSim-0.2.6/vlcsim/simulator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:07:24.278649 vlcSim-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-04 17:07:14.000000 vlcSim-0.3.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     4634 2024-04-04 17:07:24.278649 vlcSim-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4152 2024-04-04 17:07:14.000000 vlcSim-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 17:07:24.279649 vlcSim-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-04-04 17:07:14.000000 vlcSim-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:07:24.276649 vlcSim-0.3.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-04 17:07:14.000000 vlcSim-0.3.0/test/test_receiver.py
+-rw-rw-rw-   0 root         (0) root         (0)     4389 2024-04-04 17:07:14.000000 vlcSim-0.3.0/test/test_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-04-04 17:07:14.000000 vlcSim-0.3.0/test/test_vled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:07:24.277649 vlcSim-0.3.0/vlcSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4634 2024-04-04 17:07:24.000000 vlcSim-0.3.0/vlcSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      345 2024-04-04 17:07:24.000000 vlcSim-0.3.0/vlcSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 17:07:24.000000 vlcSim-0.3.0/vlcSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 17:07:24.000000 vlcSim-0.3.0/vlcSim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-04 17:07:24.000000 vlcSim-0.3.0/vlcSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-04 17:07:24.000000 vlcSim-0.3.0/vlcSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:07:24.278649 vlcSim-0.3.0/vlcsim/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-04 17:07:14.000000 vlcSim-0.3.0/vlcsim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16835 2024-04-04 17:07:14.000000 vlcSim-0.3.0/vlcsim/controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    25223 2024-04-04 17:07:14.000000 vlcSim-0.3.0/vlcsim/scene.py
+-rw-rw-rw-   0 root         (0) root         (0)    22090 2024-04-04 17:07:14.000000 vlcSim-0.3.0/vlcsim/simulator.py
```

### Comparing `vlcSim-0.2.6/LICENSE.md` & `vlcSim-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vlcSim-0.2.6/PKG-INFO` & `vlcSim-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlcSim
-Version: 0.2.6
+Version: 0.3.0
 Summary: Python Package of Event-Oriented Simulation for visible light communication
 Home-page: https://gitlab.com/DaniloBorquez/simvlc/
 Author: Danilo Bórquez-Paredes
 Author-email: danilo.borquez.p@uai.cl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vlcSim-0.2.6/README.md` & `vlcSim-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vlcSim-0.2.6/setup.py` & `vlcSim-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 INSTALL_REQUIRES = ["numpy", "enum34"]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="vlcSim",
-    version="0.2.6",
+    version="0.3.0",
     license="MIT",
     description="Python Package of Event-Oriented Simulation for visible light communication",
     author="Danilo Bórquez-Paredes",
     author_email="danilo.borquez.p@uai.cl",
     url="https://gitlab.com/DaniloBorquez/simvlc/",
     packages=["vlcsim"],
     install_requires=INSTALL_REQUIRES,
```

### Comparing `vlcSim-0.2.6/test/test_receiver.py` & `vlcSim-0.3.0/test/test_receiver.py`

 * *Files identical despite different names*

### Comparing `vlcSim-0.2.6/test/test_scenario.py` & `vlcSim-0.3.0/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `vlcSim-0.2.6/test/test_vled.py` & `vlcSim-0.3.0/test/test_vled.py`

 * *Files identical despite different names*

### Comparing `vlcSim-0.2.6/vlcSim.egg-info/PKG-INFO` & `vlcSim-0.3.0/vlcSim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlcSim
-Version: 0.2.6
+Version: 0.3.0
 Summary: Python Package of Event-Oriented Simulation for visible light communication
 Home-page: https://gitlab.com/DaniloBorquez/simvlc/
 Author: Danilo Bórquez-Paredes
 Author-email: danilo.borquez.p@uai.cl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vlcSim-0.2.6/vlcsim/controller.py` & `vlcSim-0.3.0/vlcsim/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 The :mod:`vlcsim.controller` module is in charge of managing the connections and the physical sustrate.
 """
 
 from .scene import *
 from enum import Enum
 import math
+import sys
 
 
 class Connection:
     """
     The :class:`vlcsim.controller.Connection` contains the connection information. Each :class:`vlcsim.controller.Connection` object contains an ID connection, the Access Point (AP) that uses the :class:`vlcsim.controller.Connection` object, the receiver connected to the AP, and finally if the connection was successfully allocated.
     """
 
@@ -28,14 +29,23 @@
         self.__receiver = receiver
         self.__allocated = True
         self.__frameSlice = []
         self.__timesAssigned = []
         self.__goalTime = None
         self.__time = time
         self.__capacityRequired = None
+        self.__snr = sys.float_info.min
+
+    @property
+    def snr(self):
+        return self.__snr
+
+    @snr.setter
+    def snr(self, value):
+        self.__snr = value
 
     @property
     def capacityRequired(self) -> float:
         return self.__capacityRequired
 
     @capacityRequired.setter
     def capacityRequired(self, value: float):
```

### Comparing `vlcSim-0.2.6/vlcsim/scene.py` & `vlcSim-0.3.0/vlcsim/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module work with the classes belonging to the Scene. It manages the physical sustrate.
 """
 
 import numpy as np
 import math as m
 from enum import Enum
+import warnings
 
 
 class AccessPoint:
     """
     Class representing a generic access point
     """
 
@@ -830,14 +831,17 @@
     @timeFinished.setter
     def timeFinished(self, value):
         self.__timeFinished = value
 
 
 class Scenario:
     numberOfAPs = 0
+    warnings.filterwarnings(
+        "ignore", message="invalid value encountered in double_scalars"
+    )
 
     def __init__(
         self, width: float, length: float, height: float, nGrids: int, rho: float
     ) -> None:
         self.__length = length  # x
         self.__width = width  # y
         self.__height = height  # z
```

### Comparing `vlcSim-0.2.6/vlcsim/simulator.py` & `vlcSim-0.3.0/vlcsim/simulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,14 +88,17 @@
 
         self.__upper_random_wait = None
         self.__lower_random_wait = None
 
         self.__upper_capacity_required = None
         self.__lower_capacity_required = None
 
+        self.__users_by_vlc = []
+        self.__users_by_rf = []
+
         self.default_values()
 
     def default_values(self):
         self.__initReady = False
         self.__lambdaS = 3
         self.__mu = 10
         self.__seedArrive = 12345
@@ -269,25 +272,50 @@
             % (
                 self.__controller.scenario.length,
                 self.__controller.scenario.width,
                 self.__controller.scenario.height,
             )
         )
 
-        print("=" * 120)
+        print(f"Number of VLeds: {self.__controller.scenario.numberOfVLeds}")
+        print("Positions:")
+        print("        ID  |     X     |     Y    |     Z    |")
+        print("-" * 47)
+        for vled in self.__controller.scenario.vleds:
+            print(
+                "{:>10}  |  {:8.4f} | {:8.4f} | {:8.4f} |".format(
+                    vled.ID, vled.x, vled.y, vled.z
+                )
+            )
+        print()
+        print(f"Number of RFs: {self.__controller.scenario.numberOfRFs}")
+        print("Positions:")
+        print("        ID  |     X     |     Y    |     Z    |")
+        print("-" * 47)
+        for rf in self.__controller.scenario.rfs:
+            print(
+                "{:>10}  |  {:8.4f} | {:8.4f} | {:8.4f} |".format(
+                    rf.ID, rf.x, rf.y, rf.z
+                )
+            )
+        print()
+
+        print("=" * 146)
         print("|  Time  ", end="")
         print("|   Event   ", end="")
         print("|  Receiver   ", end="")
         print("|    X    ", end="")
         print("|    Y    ", end="")
         print("|    Z    ", end="")
         print("|  Access Point (A.C.) ", end="")
         print("|  Goal time  ", end="")
-        print("|  Elapsed time  |")
-        print("=" * 120)
+        print("|  Elapsed time  ", end="")
+        print("|    SNR     ", end="")
+        print("|  Req. Cap. |")
+        print("=" * 146)
 
     def print_row(self, event):
         text = ""
         text = "{:9.4f}".format(event.time) + "|"
         if event.type == Event.event.ARRIVE:
             text += "   ARRIVE  |"
         elif event.type == Event.event.RESUME:
@@ -335,14 +363,16 @@
         #            )
         #        else:
         #            print(
         #                event.time,
         #               event.type,
         #               event.id_connection,
         #           )
+        text += "{:10.2e}".format(event.connection.snr) + "  |"
+        text += "{:10.2e}".format(event.connection.capacityRequired) + "  |"
         print(text)
 
     def event_routine(self):
         self.__current_event = self.__events[0]
         self.__rtn_allocation = None
         self.__clock = self.__current_event.time
         # print()
@@ -391,14 +421,18 @@
             next_status, time, connection = self.__controller.assignConnection(
                 connection, self.__clock
             )
             if (
                 next_status == Controller.nextStatus.RESUME
                 or next_status == Controller.nextStatus.PAUSE
             ):
+                if type(connection.AP) == VLed:
+                    self.__users_by_vlc[connection.AP.ID] += 1
+                elif type(connection.AP) == RF:
+                    self.__users_by_rf[connection.AP.ID] += 1
                 self.__current_event.connection = connection
                 if next_status == Controller.nextStatus.RESUME:
                     for pos in range(len(self.__events) - 1, -1, -1):
                         if self.__events[pos].time <= time:
                             e = Event(
                                 Event.event.RESUME,
                                 time,
@@ -541,21 +575,26 @@
         self.__allocatedConnections = 0
         self.__controller.init()
         if (
             self.__controller.scenario.numberOfVLeds == 0
             and self.__controller.scenario.numberOfRFs == 0
         ):
             raise ("The scenario does not have any Vleds or RFs")
+        for _ in range(self.__controller.scenario.numberOfVLeds):
+            self.__users_by_vlc.append(0)
+        for _ in range(self.__controller.scenario.numberOfRFs):
+            self.__users_by_rf.append(0)
         return
 
     def run(self):
         self.print_initial_info()
         while self.__numberOfConnections <= self.__goalConnections:
             # for i in range(self.__goalConnections):
             self.event_routine()
+        self.aggregated_metrics()
 
     def time_duration(self):
         return self.__time_duration
 
     def get_Blocking_Probability(self):
         blocking = round(
             1 - self.__allocatedConnections / self.__numberOfConnections, 2
@@ -564,7 +603,18 @@
 
     def set_allocation_algorithm(self, alloc_alg):
         self.__controller.allocator = alloc_alg
 
     @property
     def scenario(self):
         return self.__controller.scenario
+
+    def aggregated_metrics(self):
+        print("Number of users connected to each VLed")
+        for i in range(self.__controller.scenario.numberOfVLeds):
+            id = self.__controller.scenario.vleds[i].ID
+            print(f"VLed {id}: {self.__users_by_vlc[id]}")
+
+        print("Number of users connected to each RF")
+        for i in range(self.__controller.scenario.numberOfRFs):
+            id = self.__controller.scenario.rfs[i].ID
+            print(f"RF {id}: {self.__users_by_rf[id]}")
```

