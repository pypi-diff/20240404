# Comparing `tmp/sapiopycommons-2024.4.4a175.tar.gz` & `tmp/sapiopycommons-31.2.0.23.12.3.tar.gz`

## Comparing `sapiopycommons-2024.4.4a175.tar` & `sapiopycommons-31.2.0.23.12.3.tar`

### file list

```diff
@@ -1,32 +1,29 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/__init__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/chem/IndigoMolecules.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/chem/Molecules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/chem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/datatype/__init__.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/datatype/attachment_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/eln/__init__.py
--rw-r--r--   0        0        0    54417 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/eln/experiment_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/files/__init__.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/files/file_bridge.py
--rw-r--r--   0        0        0    23142 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/files/file_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/general/__init__.py
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/general/aliases.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/general/custom_report_util.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/general/exceptions.py
--rw-r--r--   0        0        0    29150 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/general/popup_util.py
--rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/general/storage_util.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/general/time_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/processtracking/__init__.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/processtracking/endpoints.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/recordmodel/__init__.py
--rw-r--r--   0        0        0    34338 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/recordmodel/record_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/rules/__init__.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/rules/eln_rule_handler.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/rules/on_save_rule_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/webhook/__init__.py
--rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/src/sapiopycommons/webhook/webhook_handlers.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/LICENSE
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/pyproject.toml
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 sapiopycommons-2024.4.4a175/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/Molecules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/__init__.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/__init__.py
+-rw-r--r--   0        0        0    54417 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/__init__.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_bridge.py
+-rw-r--r--   0        0        0    23142 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/aliases.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/custom_report_util.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/exceptions.py
+-rw-r--r--   0        0        0    29150 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/popup_util.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/time_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/__init__.py
+-rw-r--r--   0        0        0    34338 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/__init__.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/eln_rule_handler.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/on_save_rule_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/__init__.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/LICENSE
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/pyproject.toml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/PKG-INFO
```

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/chem/IndigoMolecules.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/chem/Molecules.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/Molecules.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/datatype/attachment_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/eln/experiment_handler.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/files/file_bridge.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_bridge.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/files/file_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/general/aliases.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/aliases.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 from collections.abc import Iterable
 from typing import Any
 
 from sapiopylib.rest.pojo.DataRecord import DataRecord
-from sapiopylib.rest.pojo.eln.ElnExperiment import ElnExperiment
-from sapiopylib.rest.utils.Protocols import ElnExperimentProtocol
 from sapiopylib.rest.utils.recordmodel.PyRecordModel import PyRecordModel
 from sapiopylib.rest.utils.recordmodel.RecordModelWrapper import WrappedRecordModel, WrappedType
 
 RecordModel = PyRecordModel | WrappedRecordModel | WrappedType
 """Different forms that a record model could take."""
 SapioRecord = DataRecord | RecordModel
 """A record could be provided as either a DataRecord, PyRecordModel, or WrappedRecordModel (WrappedType)."""
 RecordIdentifier = SapioRecord | int
 """A RecordIdentifier is either a record type or an integer for the record's record ID."""
-ExperimentIdentifier = ElnExperimentProtocol | ElnExperiment | int
-"""An ExperimentIdentifier is either an experiment protocol, experiment, or an integer for te experiment's notebook
-ID."""
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class AliasUtil:
     @staticmethod
     def to_data_record(record: SapioRecord) -> DataRecord:
         """
@@ -60,20 +55,7 @@
         field_map_list: list[dict[str, Any]] = []
         for record in records:
             if isinstance(record, DataRecord):
                 field_map_list.append(record.get_fields())
             else:
                 field_map_list.append(record.fields.copy_to_dict())
         return field_map_list
-
-    @staticmethod
-    def to_notebook_id(experiment: ExperimentIdentifier) -> int:
-        """
-        Convert an object that identifies an ELN experiment to its notebook ID.
-
-        :return: The notebook ID for the experiment identifier.
-        """
-        if isinstance(experiment, int):
-            return experiment
-        if isinstance(experiment, ElnExperiment):
-            return experiment.notebook_experiment_id
-        return experiment.get_id()
```

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/general/custom_report_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/custom_report_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/general/exceptions.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/general/popup_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/popup_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/general/time_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/time_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/recordmodel/record_handler.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/rules/eln_rule_handler.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/eln_rule_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/rules/on_save_rule_handler.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/on_save_rule_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/src/sapiopycommons/webhook/webhook_handlers.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/LICENSE` & `sapiopycommons-31.2.0.23.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/README.md` & `sapiopycommons-31.2.0.23.12.3/README.md`

 * *Files identical despite different names*

### Comparing `sapiopycommons-2024.4.4a175/pyproject.toml` & `sapiopycommons-31.2.0.23.12.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopycommons"
-version='2024.04.04a175'
+version='31.2.0.23.12.3'
 authors = [
     { name="Jonathan Steck", email="jsteck@sapiosciences.com" },
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Python API Utilities Package"
 license = "MPL-2.0"
 readme = "README.md"
```

### Comparing `sapiopycommons-2024.4.4a175/PKG-INFO` & `sapiopycommons-31.2.0.23.12.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sapiopycommons
-Version: 2024.4.4a175
+Version: 31.2.0.23.12.3
 Summary: Official Sapio Python API Utilities Package
 Project-URL: Homepage, https://github.com/sapiosciences
 Author-email: Jonathan Steck <jsteck@sapiosciences.com>, Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: sapiopycommons Version: 2024.4.4a175 Summary:
+Metadata-Version: 2.3 Name: sapiopycommons Version: 31.2.0.23.12.3 Summary:
 Official Sapio Python API Utilities Package Project-URL: Homepage, https://
 github.com/sapiosciences Author-email: Jonathan Steck
 sapiosciences.com>, Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
```

