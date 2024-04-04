# Comparing `tmp/umlcharter-0.0.3.tar.gz` & `tmp/umlcharter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umlcharter-0.0.3.tar", last modified: Tue Apr  2 17:37:23 2024, max compression
+gzip compressed data, was "umlcharter-0.0.4.tar", last modified: Thu Apr  4 18:52:17 2024, max compression
```

## Comparing `umlcharter-0.0.3.tar` & `umlcharter-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.981207 umlcharter-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 17:37:12.000000 umlcharter-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-02 17:37:23.981207 umlcharter-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 17:37:12.000000 umlcharter-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:37:23.981207 umlcharter-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-02 17:37:12.000000 umlcharter-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.977207 umlcharter-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:12.000000 umlcharter-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-02 17:37:12.000000 umlcharter-0.0.3/tests/test_sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.977207 umlcharter-0.0.3/umlcharter/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.977207 umlcharter-0.0.3/umlcharter/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/charts/sequence_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/charts/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.977207 umlcharter-0.0.3/umlcharter/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.977207 umlcharter-0.0.3/umlcharter/generators/mermaid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/mermaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/mermaid/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/mermaid/sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.977207 umlcharter-0.0.3/umlcharter/generators/plantuml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/plantuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/plantuml/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/plantuml/sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.981207 umlcharter-0.0.3/umlcharter/generators/zenuml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/zenuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/zenuml/sequence_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/generators/zenuml/zenuml.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 17:37:12.000000 umlcharter-0.0.3/umlcharter/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:37:23.981207 umlcharter-0.0.3/umlcharter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-02 17:37:23.000000 umlcharter-0.0.3/umlcharter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-02 17:37:23.000000 umlcharter-0.0.3/umlcharter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:37:23.000000 umlcharter-0.0.3/umlcharter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:37:23.000000 umlcharter-0.0.3/umlcharter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 18:52:13.000000 umlcharter-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-04 18:52:17.279878 umlcharter-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-04 18:52:13.000000 umlcharter-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:52:17.279878 umlcharter-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-04 18:52:13.000000 umlcharter-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.275878 umlcharter-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-04 18:52:13.000000 umlcharter-0.0.4/tests/test_sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.275878 umlcharter-0.0.4/umlcharter/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/charts/sequence_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/charts/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter/generators/mermaid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/mermaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/mermaid/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/mermaid/sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter/generators/plantuml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/plantuml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/plantuml/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-04 18:52:13.000000 umlcharter-0.0.4/umlcharter/generators/plantuml/sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:52:17.279878 umlcharter-0.0.4/umlcharter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-04 18:52:17.000000 umlcharter-0.0.4/umlcharter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-04 18:52:17.000000 umlcharter-0.0.4/umlcharter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:52:17.000000 umlcharter-0.0.4/umlcharter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 18:52:17.000000 umlcharter-0.0.4/umlcharter.egg-info/top_level.txt
```

### Comparing `umlcharter-0.0.3/LICENSE` & `umlcharter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `umlcharter-0.0.3/PKG-INFO` & `umlcharter-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umlcharter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for quick diagrams creation without a need to learn new DSL
 Home-page: https://github.com/mikalaiyurkin/charter
 Author: Mikalai Yurkin
 Author-email: yurkin.mikalai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,20 +15,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![pypi](https://img.shields.io/pypi/v/umlcharter.svg)
+![versions](https://img.shields.io/pypi/pyversions/umlcharter.svg)
+
 # umlcharter
 Python package for quick diagrams creation without a need to learn a new DSL.
 
-The goal of this package is to provide a tool for a convenient and quick creation of the UML diagrams
-in the popular DSLs like Mermaid, PlantUML, ZenUML, etc using a simple python constructions.
-
-For details about the mentioned DSLs, please refer to the next links:
-- [Mermaid](https://mermaid.js.org/)
-- [PlantUML](https://plantuml.com/)
-- [ZenUML](https://zenuml.com/)
+The goal of this package is to provide a tool for convenient and quick creation of the diagrams as a code
+in the popular DSLs (PlantUML, Mermaid, D2, etc) using simple python constructions.
 
-For the examples of how this package can be used, please check the documentation:
+For the examples of how this package can be used and the list of exactly supported DSLs, 
+please check the documentation:
 - [Sequence Diagrams](docs/sequence_diagram/README.md)
```

### Comparing `umlcharter-0.0.3/setup.py` & `umlcharter-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import re
 
 with open("README.md", "rt") as f:
     long_description = f.read()
 
-with open("umlcharter/metadata.py", "rt") as f:
+with open("umlcharter/__init__.py", "rt") as f:
     version = re.search(r"__version__ = \"(.*?)\"", f.read()).group(1)
 
 setuptools.setup(
     name="umlcharter",
     version=version,
     author="Mikalai Yurkin",
     author_email="yurkin.mikalai@gmail.com",
```

### Comparing `umlcharter-0.0.3/umlcharter/charts/sequence_diagram.py` & `umlcharter-0.0.4/umlcharter/charts/sequence_diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 class ReturnStep(Step):
     text: str
     from_participant: "SequenceDiagramParticipant"
     to_participant: "SequenceDiagramParticipant"
 
 
 @dataclass
+class NoteStep(Step):
+    text: str
+
+
+@dataclass
 class SequenceDiagramParticipant:
     sequence_ref: "SequenceDiagram"
     title: str
 
     def __add_step(
         self, step: typing.Union[ForwardStep, ReturnStep, ParticipantActivationControl]
     ):
@@ -136,14 +141,22 @@
                 f"Sequence diagram already contains participant {title}. "
                 f"All participants must have unique titles."
             )
         participant = SequenceDiagramParticipant(title=title, sequence_ref=self)
         self.__participants.append(participant)
         return participant
 
+    def note(self, text: str) -> None:
+        """
+        Add the note plate with the iven text somewhere inside the diagram
+        :param text:
+        :return:
+        """
+        self.__add_step(NoteStep(text=text))
+
     @contextmanager
     def loop(self, how_many_iterations: str) -> None:
         """
         Explicitly mark the following sequence of steps as performed in the loop
         """
         self.__add_step(
             LoopControl(is_active=True, how_many_iterations=how_many_iterations)
@@ -286,9 +299,9 @@
                 self.__sequence.append(step)
         else:
             self.__sequence.append(step)
 
     def generate(self) -> str:
         return self.__generator.generate_sequence_diagram()
 
-    def __repr__(self):
-        return f"Sequence Diagram ({self.title})"
+    def __str__(self):
+        return self.generate()
```

### Comparing `umlcharter-0.0.3/umlcharter.egg-info/PKG-INFO` & `umlcharter-0.0.4/umlcharter.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umlcharter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for quick diagrams creation without a need to learn new DSL
 Home-page: https://github.com/mikalaiyurkin/charter
 Author: Mikalai Yurkin
 Author-email: yurkin.mikalai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,20 +15,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![pypi](https://img.shields.io/pypi/v/umlcharter.svg)
+![versions](https://img.shields.io/pypi/pyversions/umlcharter.svg)
+
 # umlcharter
 Python package for quick diagrams creation without a need to learn a new DSL.
 
-The goal of this package is to provide a tool for a convenient and quick creation of the UML diagrams
-in the popular DSLs like Mermaid, PlantUML, ZenUML, etc using a simple python constructions.
-
-For details about the mentioned DSLs, please refer to the next links:
-- [Mermaid](https://mermaid.js.org/)
-- [PlantUML](https://plantuml.com/)
-- [ZenUML](https://zenuml.com/)
+The goal of this package is to provide a tool for convenient and quick creation of the diagrams as a code
+in the popular DSLs (PlantUML, Mermaid, D2, etc) using simple python constructions.
 
-For the examples of how this package can be used, please check the documentation:
+For the examples of how this package can be used and the list of exactly supported DSLs, 
+please check the documentation:
 - [Sequence Diagrams](docs/sequence_diagram/README.md)
```

### Comparing `umlcharter-0.0.3/umlcharter.egg-info/SOURCES.txt` & `umlcharter-0.0.4/umlcharter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/test_sequence_diagram.py
 umlcharter/__init__.py
-umlcharter/metadata.py
 umlcharter.egg-info/PKG-INFO
 umlcharter.egg-info/SOURCES.txt
 umlcharter.egg-info/dependency_links.txt
 umlcharter.egg-info/top_level.txt
 umlcharter/charts/__init__.py
 umlcharter/charts/sequence_diagram.py
 umlcharter/charts/types.py
 umlcharter/generators/__init__.py
 umlcharter/generators/base.py
 umlcharter/generators/mermaid/__init__.py
 umlcharter/generators/mermaid/mermaid.py
 umlcharter/generators/mermaid/sequence_diagram.py
 umlcharter/generators/plantuml/__init__.py
 umlcharter/generators/plantuml/plantuml.py
-umlcharter/generators/plantuml/sequence_diagram.py
-umlcharter/generators/zenuml/__init__.py
-umlcharter/generators/zenuml/sequence_diagram.py
-umlcharter/generators/zenuml/zenuml.py
+umlcharter/generators/plantuml/sequence_diagram.py
```

