# Comparing `tmp/droid_metapatch-0.9.0.tar.gz` & `tmp/droid_metapatch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droid_metapatch-0.9.0.tar", max compression
+gzip compressed data, was "droid_metapatch-1.0.0.tar", max compression
```

## Comparing `droid_metapatch-0.9.0.tar` & `droid_metapatch-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7232 2024-04-04 11:04:29.347160 droid_metapatch-0.9.0/README.md
--rw-r--r--   0        0        0      155 2024-04-04 07:42:22.856150 droid_metapatch-0.9.0/metapatch/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-04 08:10:17.197194 droid_metapatch-0.9.0/metapatch/base.py
--rw-r--r--   0        0        0    10211 2024-04-04 11:14:05.849692 droid_metapatch-0.9.0/metapatch/metapatch.py
--rw-r--r--   0        0        0     6928 2024-04-04 09:31:45.638933 droid_metapatch-0.9.0/metapatch/options.py
--rw-r--r--   0        0        0      697 2024-04-04 09:40:34.183085 droid_metapatch-0.9.0/metapatch/utils.py
--rw-r--r--   0        0        0      425 2024-04-04 10:17:19.653865 droid_metapatch-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     7843 1970-01-01 00:00:00.000000 droid_metapatch-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     8632 2024-04-04 19:33:48.334657 droid_metapatch-1.0.0/README.md
+-rw-r--r--   0        0        0      155 2024-04-04 07:42:22.856150 droid_metapatch-1.0.0/metapatch/__init__.py
+-rw-r--r--   0        0        0     2431 2024-04-04 19:16:50.476894 droid_metapatch-1.0.0/metapatch/base.py
+-rw-r--r--   0        0        0    11020 2024-04-04 19:25:23.451626 droid_metapatch-1.0.0/metapatch/metapatch.py
+-rw-r--r--   0        0        0     6928 2024-04-04 09:31:45.638933 droid_metapatch-1.0.0/metapatch/options.py
+-rw-r--r--   0        0        0      697 2024-04-04 09:40:34.183085 droid_metapatch-1.0.0/metapatch/utils.py
+-rw-r--r--   0        0        0      425 2024-04-04 19:30:50.468212 droid_metapatch-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9243 1970-01-01 00:00:00.000000 droid_metapatch-1.0.0/PKG-INFO
```

### Comparing `droid_metapatch-0.9.0/README.md` & `droid_metapatch-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 # Getting started
 
 A few examples have been distributed with the source code of this library that you may look at to see full implementations.
 
 Before you can write a patch generator, please install this library to your system python environment. Forge does not support virtual environments, so you must install this library somewhere where your default python library can find it.
 
+This library is available from pypi, use `pip install droid-metapatch` to install it.
+
 
 ## Defining your patch generator class
 
 To start, you must define a python `class` that is a subclass of `metapatch.PatchGenerator`.
 
 Inside this class, you must at least define a `title` and a `description`, as well as a method called `generate`.
 
@@ -126,14 +128,15 @@
 ## Writing patches
 
 The following actions are currently supported:
 
 -   Adding controllers
 -   Adding circuits
 -   Adding sections
+-   Adding labels to jacks, buttons and pots
 
 
 ### Adding controllers
 
 ```python
     def add_controller(self, type: str, position: int) -> None:
         """Add a controller at a given position.
@@ -201,14 +204,71 @@
         # Iterate over voices that were defined
         for voicenum in range(1, self.voices + 1):
             self.add_section(f"Voice {voicenum}")
             # Add circuits here.
 ```
 
 
+### Adding labels to jacks, buttons and pots
+
+You can add labels to jacks, buttons and pots with the `add_label` function:
+
+```python
+    def add_label(
+        self, item: str, short_label: str, long_label: Optional[str] = None
+    ) -> None:
+        """Add a label.
+
+        Args:
+            item: string of the thing you want to label, e.g. O1 or G1.2
+            short_label: The short label
+            long_label: Optional longer label
+        """
+```
+
+The item is the item you want to label, and can be anything that supports a label. The short label is mandatory, but the long one can be optional.
+
+For example:
+
+```python
+        def generate(self) -> None:
+            """Generate patch."""
+            self.add_controller("P2B8", 1)
+            self.add_controller("P2B8", 2)
+            self.add_controller("P2B8", 3)
+            self.add_controller("E4", 4)
+            self.add_label("I1", "Input 1", "This is input 1")
+            self.add_label("O1", "Output 1")
+            self.add_label("G2.7", "Gate 7", "Gate jack number 7")
+            self.add_label("E4.3", "Encoder", "Encoder 3 on module 4")
+```
+
+This will generate the following:
+
+```
+#  I1: [Input 1] This is input 1
+
+# OUTPUTS:
+#  O1: [Output 1]
+
+# GATES ON MODULE 2:
+#  G2.7: [Gate 7] Gate jack number 7
+
+# CONTROLLER 4:
+#  E4.3: [Encoder] Encoder 3 on module 4
+
+[P2B8]
+[P2B8]
+[P2B8]
+[E4]
+
+
+```
+
+
 ## Finishing your patch
 
 Once you are done writing your code, you just need to make sure that the patch generator is loaded when executing the module.
 
 This can be done by simply calling `run()` on your class.
 
 ```python
@@ -224,19 +284,14 @@
 
 MyPatch.run()
 ```
 
 This automatically sets up processing of command line arguments, correct argument passing and so on.
 
 
-# Missing features
-
-Currently there is no way to define the labels of jacks and pots. This will come soon.
-
-
 # Getting help
 
 If you have any problems with the library, let me know on the DROID discord server. I&rsquo;m known as eising on that server.
 
 Please note that any support will be on a best effort basis, if I have the time an energy.
 
 If you have found a bug, please create an issue here on github.
```

### Comparing `droid_metapatch-0.9.0/metapatch/metapatch.py` & `droid_metapatch-1.0.0/metapatch/metapatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from abc import abstractmethod
 from typing import (
     Any,
     Dict,
     List,
     Mapping,
     Optional,
-    Tuple,
 )
 
-from .base import Circuit, Controller, Section
+from .base import Circuit, Controller, Label
 from .options import Option, BoolOption, NumberOption, EnumOption, Preset
 from .utils import write_patch_section
 
 DEFAULT_SECTION_NAME = "Generated Patch"
 
 
 def _split_params(params: List[str]) -> Dict[str, str]:
@@ -112,15 +111,15 @@
                 assert issubclass(var, (BoolOption, EnumOption, NumberOption))
                 setattr(self, key, var(value).get_value())
             else:
                 raise ValueError(f"Unknown parameter {key}")
 
         self.circuits: List[Circuit] = []
         self.controllers: List[Controller] = []
-        self.labels: Dict[str, Tuple[str, str]] = {}
+        self.labels: List[Label] = []
         self._section: Optional[str] = None
         # This dictionary stores comments for sections.
         self.sections: Dict[str, Optional[str]] = {}
 
     @classmethod
     def load_preset(cls, preset_name: str) -> "PatchGenerator":
         """Load preset."""
@@ -218,27 +217,52 @@
             params: Dictionary of circuit parameters.
             comment: Optional comment for the circuit.
         """
         self.circuits.append(
             Circuit(name=name, parameters=params, comment=comment, section=self.section)
         )
 
+    def add_label(
+        self, item: str, short_label: str, long_label: Optional[str] = None
+    ) -> None:
+        """Add a label.
+
+        Args:
+            item: string of the thing you want to label, e.g. O1 or G1.2
+            short_label: The short label
+            long_label: Optional longer label
+        """
+        self.labels.append(Label.from_item(item, short_label, long_label))
+
+    def _generate_labels(self) -> str:
+        """Generate label strings."""
+        sorted_labels = {}
+        for label in self.labels:
+            if label.heading not in sorted_labels:
+                sorted_labels[label.heading] = []
+            sorted_labels[label.heading].append(label)
+
+        labels = ""
+        for heading, list_labels in sorted_labels.items():
+            labels += f"# {heading.upper()}:\n"
+            for label in list_labels:
+                labels += str(label)
+            labels += "\n"
+
+        return labels
+
     def add_controller(self, type: str, position: int) -> None:
         """Add a controller at a given position.
 
         Args:
             type: Type of controller, e.g. B32
             position: controller position, e.g. 1
         """
         self.controllers.append(Controller(type, position))
 
-    def set_labels(self, labels: Mapping[str, Tuple[str, str]]) -> None:
-        """Set labels of jacks."""
-        self.labels = {**self.labels, **labels}
-
     @property
     def section(self) -> Optional[str]:
         """Get section."""
         return self._section
 
     @section.setter
     def section(self, name: str) -> None:
@@ -289,19 +313,20 @@
 
         return "\n".join(circuits)
 
     def __str__(self) -> str:
         """Output patch as string."""
         self._generate()
 
+        labels = self._generate_labels()
         sorted_controllers = sorted(self.controllers, key=lambda x: x.position)
         controllers = "\n".join([str(controller) for controller in sorted_controllers])
         circuits = self._get_circuits_as_strings()
 
-        return f"{controllers}\n\n{circuits}"
+        return f"{labels}{controllers}\n\n{circuits}"
 
     def _generate(self) -> None:
         """Generate patch.
 
         This is an internal function that ensures that we reset the patch if needed.
         """
         if not self.circuits and not self.controllers:
```

### Comparing `droid_metapatch-0.9.0/metapatch/options.py` & `droid_metapatch-1.0.0/metapatch/options.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-0.9.0/metapatch/utils.py` & `droid_metapatch-1.0.0/metapatch/utils.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-0.9.0/PKG-INFO` & `droid_metapatch-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: droid-metapatch
-Version: 0.9.0
+Version: 1.0.0
 Summary: DROID patch generator
 License: GPL-3.0-only
 Author: Allan Eising
 Author-email: allan@eising.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -24,14 +24,16 @@
 
 # Getting started
 
 A few examples have been distributed with the source code of this library that you may look at to see full implementations.
 
 Before you can write a patch generator, please install this library to your system python environment. Forge does not support virtual environments, so you must install this library somewhere where your default python library can find it.
 
+This library is available from pypi, use `pip install droid-metapatch` to install it.
+
 
 ## Defining your patch generator class
 
 To start, you must define a python `class` that is a subclass of `metapatch.PatchGenerator`.
 
 Inside this class, you must at least define a `title` and a `description`, as well as a method called `generate`.
 
@@ -143,14 +145,15 @@
 ## Writing patches
 
 The following actions are currently supported:
 
 -   Adding controllers
 -   Adding circuits
 -   Adding sections
+-   Adding labels to jacks, buttons and pots
 
 
 ### Adding controllers
 
 ```python
     def add_controller(self, type: str, position: int) -> None:
         """Add a controller at a given position.
@@ -218,14 +221,71 @@
         # Iterate over voices that were defined
         for voicenum in range(1, self.voices + 1):
             self.add_section(f"Voice {voicenum}")
             # Add circuits here.
 ```
 
 
+### Adding labels to jacks, buttons and pots
+
+You can add labels to jacks, buttons and pots with the `add_label` function:
+
+```python
+    def add_label(
+        self, item: str, short_label: str, long_label: Optional[str] = None
+    ) -> None:
+        """Add a label.
+
+        Args:
+            item: string of the thing you want to label, e.g. O1 or G1.2
+            short_label: The short label
+            long_label: Optional longer label
+        """
+```
+
+The item is the item you want to label, and can be anything that supports a label. The short label is mandatory, but the long one can be optional.
+
+For example:
+
+```python
+        def generate(self) -> None:
+            """Generate patch."""
+            self.add_controller("P2B8", 1)
+            self.add_controller("P2B8", 2)
+            self.add_controller("P2B8", 3)
+            self.add_controller("E4", 4)
+            self.add_label("I1", "Input 1", "This is input 1")
+            self.add_label("O1", "Output 1")
+            self.add_label("G2.7", "Gate 7", "Gate jack number 7")
+            self.add_label("E4.3", "Encoder", "Encoder 3 on module 4")
+```
+
+This will generate the following:
+
+```
+#  I1: [Input 1] This is input 1
+
+# OUTPUTS:
+#  O1: [Output 1]
+
+# GATES ON MODULE 2:
+#  G2.7: [Gate 7] Gate jack number 7
+
+# CONTROLLER 4:
+#  E4.3: [Encoder] Encoder 3 on module 4
+
+[P2B8]
+[P2B8]
+[P2B8]
+[E4]
+
+
+```
+
+
 ## Finishing your patch
 
 Once you are done writing your code, you just need to make sure that the patch generator is loaded when executing the module.
 
 This can be done by simply calling `run()` on your class.
 
 ```python
@@ -241,19 +301,14 @@
 
 MyPatch.run()
 ```
 
 This automatically sets up processing of command line arguments, correct argument passing and so on.
 
 
-# Missing features
-
-Currently there is no way to define the labels of jacks and pots. This will come soon.
-
-
 # Getting help
 
 If you have any problems with the library, let me know on the DROID discord server. I&rsquo;m known as eising on that server.
 
 Please note that any support will be on a best effort basis, if I have the time an energy.
 
 If you have found a bug, please create an issue here on github.
```

