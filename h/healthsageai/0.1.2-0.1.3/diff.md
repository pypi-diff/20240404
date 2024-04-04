# Comparing `tmp/healthsageai-0.1.2.tar.gz` & `tmp/healthsageai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthsageai-0.1.2.tar", last modified: Wed Feb 14 09:05:43 2024, max compression
+gzip compressed data, was "healthsageai-0.1.3.tar", last modified: Thu Apr  4 11:01:03 2024, max compression
```

## Comparing `healthsageai-0.1.2.tar` & `healthsageai-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-02-14 09:05:43.133619 healthsageai-0.1.2/
--rw-r--r--   0 a.groen    (501) staff       (20)    34523 2023-12-01 10:10:21.000000 healthsageai-0.1.2/LICENSE
--rw-r--r--   0 a.groen    (501) staff       (20)    47052 2024-02-14 09:05:43.133366 healthsageai-0.1.2/PKG-INFO
--rw-r--r--   0 a.groen    (501) staff       (20)     5729 2024-02-14 09:04:01.000000 healthsageai-0.1.2/README.md
--rw-r--r--   0 a.groen    (501) staff       (20)     1505 2024-02-14 09:04:57.000000 healthsageai-0.1.2/pyproject.toml
--rw-r--r--   0 a.groen    (501) staff       (20)       38 2024-02-14 09:05:43.133668 healthsageai-0.1.2/setup.cfg
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-02-14 09:05:43.128962 healthsageai-0.1.2/src/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-01-17 13:46:31.000000 healthsageai-0.1.2/src/__init__.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-02-14 09:05:43.128241 healthsageai-0.1.2/src/healthsageai/
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-02-14 09:05:43.130838 healthsageai-0.1.2/src/healthsageai/note_to_fhir/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     2936 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/data_utils.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-02-14 09:05:43.132145 healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     4353 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/datamodels.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3230 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py
--rw-r--r--   0 a.groen    (501) staff       (20)    17354 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/utils.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3660 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/visuals.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-02-14 09:05:43.132582 healthsageai-0.1.2/src/healthsageai/note_to_fhir/inference/
--rw-r--r--   0 a.groen    (501) staff       (20)      104 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/inference/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3315 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/inference/note_to_fhir.py
--rw-r--r--   0 a.groen    (501) staff       (20)     2039 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/parsers.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-02-14 09:05:43.132801 healthsageai-0.1.2/src/healthsageai/note_to_fhir/templates/
--rw-r--r--   0 a.groen    (501) staff       (20)     2480 2024-02-14 08:50:05.000000 healthsageai-0.1.2/src/healthsageai/note_to_fhir/templates/simple.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-02-14 09:05:43.133025 healthsageai-0.1.2/src/healthsageai.egg-info/
--rw-r--r--   0 a.groen    (501) staff       (20)    47052 2024-02-14 09:05:43.000000 healthsageai-0.1.2/src/healthsageai.egg-info/PKG-INFO
--rw-r--r--   0 a.groen    (501) staff       (20)      797 2024-02-14 09:05:43.000000 healthsageai-0.1.2/src/healthsageai.egg-info/SOURCES.txt
--rw-r--r--   0 a.groen    (501) staff       (20)        1 2024-02-14 09:05:43.000000 healthsageai-0.1.2/src/healthsageai.egg-info/dependency_links.txt
--rw-r--r--   0 a.groen    (501) staff       (20)      157 2024-02-14 09:05:43.000000 healthsageai-0.1.2/src/healthsageai.egg-info/requires.txt
--rw-r--r--   0 a.groen    (501) staff       (20)       35 2024-02-14 09:05:43.000000 healthsageai-0.1.2/src/healthsageai.egg-info/top_level.txt
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.142219 healthsageai-0.1.3/
+-rw-r--r--   0 a.groen    (501) staff       (20)    34523 2023-12-01 10:10:21.000000 healthsageai-0.1.3/LICENSE
+-rw-r--r--   0 a.groen    (501) staff       (20)    47022 2024-04-04 11:01:03.141871 healthsageai-0.1.3/PKG-INFO
+-rw-r--r--   0 a.groen    (501) staff       (20)     5699 2024-04-04 09:53:35.000000 healthsageai-0.1.3/README.md
+-rw-r--r--   0 a.groen    (501) staff       (20)     1505 2024-04-04 09:53:35.000000 healthsageai-0.1.3/pyproject.toml
+-rw-r--r--   0 a.groen    (501) staff       (20)       38 2024-04-04 11:01:03.142280 healthsageai-0.1.3/setup.cfg
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.137376 healthsageai-0.1.3/src/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-01-17 13:46:31.000000 healthsageai-0.1.3/src/__init__.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.136272 healthsageai-0.1.3/src/healthsageai/
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.138609 healthsageai-0.1.3/src/healthsageai/note_to_fhir/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     2950 2024-04-04 09:53:35.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/data_utils.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.139954 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     4644 2024-04-04 09:53:35.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/datamodels.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3592 2024-04-04 09:53:35.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py
+-rw-r--r--   0 a.groen    (501) staff       (20)    19893 2024-04-04 09:53:35.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/utils.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3660 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/visuals.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.140696 healthsageai-0.1.3/src/healthsageai/note_to_fhir/inference/
+-rw-r--r--   0 a.groen    (501) staff       (20)      104 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/inference/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3315 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/inference/note_to_fhir.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     2039 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/parsers.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.140916 healthsageai-0.1.3/src/healthsageai/note_to_fhir/templates/
+-rw-r--r--   0 a.groen    (501) staff       (20)     2480 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/templates/simple.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.141260 healthsageai-0.1.3/src/healthsageai.egg-info/
+-rw-r--r--   0 a.groen    (501) staff       (20)    47022 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/PKG-INFO
+-rw-r--r--   0 a.groen    (501) staff       (20)      797 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/SOURCES.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)        1 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/dependency_links.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)      157 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/requires.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)       35 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/top_level.txt
```

### Comparing `healthsageai-0.1.2/LICENSE` & `healthsageai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.2/PKG-INFO` & `healthsageai-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healthsageai
-Version: 0.1.2
+Version: 0.1.3
 Summary: HealthSage AI LLMs, Healthcare genAI platform
 Author-email: HealthSage AI <hello@healthsage.ai>
 Maintainer-email: HealthSage AI <hello@healthsage.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -723,15 +723,15 @@
 ## Inference: Note to FHIR
 
 You can do Note-to-fhir inference using our NoteToFhir class:
 
 ```python
 from healthsageai.note_to_fhir.inference import NoteToFhir13b
 
-model = NoteToFhir13b()  # NoteToFhir8x7b coming soon
+model = NoteToFhir13b()
 model.translate("Patient John Doe lives in Amsterdam")
 ```
 
 
 ## Evaluation of accuracy
 
 Our evaluation tool makes it easy to quantify and inspect the accuracy of generated FHIR resources w.r.t. a ground truth FHIR resource.
```

### Comparing `healthsageai-0.1.2/README.md` & `healthsageai-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ## Inference: Note to FHIR
 
 You can do Note-to-fhir inference using our NoteToFhir class:
 
 ```python
 from healthsageai.note_to_fhir.inference import NoteToFhir13b
 
-model = NoteToFhir13b()  # NoteToFhir8x7b coming soon
+model = NoteToFhir13b()
 model.translate("Patient John Doe lives in Amsterdam")
 ```
 
 
 ## Evaluation of accuracy
 
 Our evaluation tool makes it easy to quantify and inspect the accuracy of generated FHIR resources w.r.t. a ground truth FHIR resource.
```

### Comparing `healthsageai-0.1.2/pyproject.toml` & `healthsageai-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "healthsageai"
-version = "0.1.2"
+version = "0.1.3"
 description = "HealthSage AI LLMs, Healthcare genAI platform"
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 license = {file = "LICENSE"}
```

### Comparing `healthsageai-0.1.2/src/healthsageai/note_to_fhir/data_utils.py` & `healthsageai-0.1.3/src/healthsageai/note_to_fhir/data_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if isinstance(v, dict):
             dd[k] = drop_snomed_loinc(v)
         elif isinstance(v, list) and k != "coding":
             # note: Nones in lists are not dropped
             dd[k] = [drop_snomed_loinc(vv) if isinstance(vv, dict) else vv
                             for vv in v]
         elif k == 'coding' and isinstance(v, list):
-            dd[k] = [drop_code(code) if "snomed" in code["system"] or "loinc" in code["system"] else code for code in v]
+            dd[k] = [drop_code(code) if "snomed" in code.get("system","") or "loinc" in code.get("system","") else code for code in v]
         else:
             dd[k] = v
             
     return dd
 
 
 def remove_snomed_loinc_code_for_coding(key, val):
```

### Comparing `healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/datamodels.py` & `healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/datamodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,35 @@
 #  You should have received a copy of the GNU Affero General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pydantic import BaseModel, computed_field, field_validator, Field
 from typing import Any, Optional
 from collections import defaultdict
 
+class FhirValiditionScore(BaseModel):
+    n_nodes: int = 0
+    n_valid_nodes: int = 0
+    n_invalid_nodes: int = 0
+    self_is_valid: Optional[bool] = None
+
+    @computed_field
+    @property
+    def validation_score(self) -> float:
+        if self.n_nodes == 0:
+            return None
+        else:
+            return self.n_valid_nodes / self.n_nodes
+
 
 class FhirScore(BaseModel):
     n_leaves: int = 0  # The number of leaf nodes in this object
     n_additions: int = 0  # n hallucinated leaf nodes, a.k.a. "False Positives"
     n_deletions: int = 0  #  n of missing leaf nodes, a.k.a. "False Negatives"
     n_modifications: int = 0  # n of changes leaf nodes a.k.a. "Mistakes"
     n_matches: int = 0  # n of identical leaf nodes, a.k.a. "True Positives"
-    is_valid: Optional[bool] = None
 
     @computed_field
     @property
     def accuracy(self) -> float:  # The overall accuracy
         if self.n_leaves == 0:
             return None
         return self.n_matches / self.n_leaves
@@ -54,15 +67,14 @@
             return self
         return FhirScore(
             n_leaves=self.n_leaves + other.n_leaves,
             n_additions=self.n_additions + other.n_additions,
             n_deletions=self.n_deletions + other.n_deletions,
             n_modifications=self.n_modifications + other.n_modifications,
             n_matches=self.n_matches + other.n_matches,
-            is_valid=None,
         )
 
     def __radd__(self, other: Any):
         if not isinstance(other, FhirScore):
             return self
         else:
             return self.__add__(other)
```

### Comparing `healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py` & `healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,29 +23,30 @@
     PatientLink,
 )
 from fhir.resources.R4B.address import Address
 from fhir.resources.R4B.codeableconcept import CodeableConcept
 from fhir.resources.R4B.coding import Coding
 from fhir.resources.R4B.humanname import HumanName
 from fhir.resources.R4B.contactpoint import ContactPoint
-from fhir.resources.R4B.encounter import Encounter, EncounterParticipant
+from fhir.resources.R4B.encounter import Encounter, EncounterParticipant, EncounterHospitalization, EncounterLocation, EncounterDiagnosis
 from fhir.resources.R4B.allergyintolerance import AllergyIntolerance, AllergyIntoleranceReaction
 from fhir.resources.R4B.period import Period
 from fhir.resources.R4B.narrative import Narrative
 from fhir.resources.R4B.identifier import Identifier
 from fhir.resources.R4B.bundle import Bundle, BundleEntry
-from fhir.resources.R4B.organization import Organization
+from fhir.resources.R4B.organization import Organization, OrganizationContact
 from fhir.resources.R4B.practitioner import Practitioner
 from fhir.resources.R4B.procedure import Procedure, ProcedurePerformer
 from fhir.resources.R4B.condition import Condition
 from fhir.resources.R4B.immunization import Immunization, ImmunizationProtocolApplied
 from fhir.resources.R4B.observation import Observation, ObservationComponent
 from fhir.resources.R4B.medication import Medication
 from fhir.resources.R4B.quantity import Quantity
 from fhir.resources.R4B.resource import Resource
+from fhir.resources.R4B.extension import Extension
 
 object_mapping = {
     "Patient": Patient,
     "PatientCommunication": PatientCommunication,
     "PatientContact": PatientContact,
     "PatientLink": PatientLink,
     "Address": Address,
@@ -70,9 +71,14 @@
     "Medication": Medication,
     "Reference": Reference,
     "Quantity": Quantity,
     "Resource": Resource,
     "AllergyIntoleranceReaction": AllergyIntoleranceReaction,
     "ProcedurePerformer": ProcedurePerformer,
     "ImmunizationProtocolApplied": ImmunizationProtocolApplied,
-    "ObservationComponent": ObservationComponent
+    "ObservationComponent": ObservationComponent,
+    "EncounterHospitalization": EncounterHospitalization,
+    "EncounterLocation": EncounterLocation,
+    "OrganizationContact": OrganizationContact,
+    "EncounterDiagnosis": EncounterDiagnosis,
+    "Extension": Extension,
 }
```

### Comparing `healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/utils.py` & `healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 from healthsageai.note_to_fhir.evaluation.fhirmodels import object_mapping
 from typing import List
 import warnings
 from collections import defaultdict
 from pydantic.v1.main import ModelMetaclass
 import pandas as pd
 import itertools
+import numpy as np
+
+MAX_PERMUTATIONS_ARRAY_SIZE = 5  # When all permutations have to be calculated
 
 
 def get_resource_details(Resource) -> List[ElementDetails]:
     """Get the details of a certain fhir resource that are relevant to evaluation in a friendly format.
 
     Args:
         Resource (fhir.resources): Resource Metadata
@@ -140,15 +143,15 @@
 
     Args:
         fhirtype (str): fhirtype as specified by fhir.resources
 
     Returns:
         bool: True if fhirtype is leaf, False otherwise
     """
-    return fhirtype in ["boolean", "integer", "string", "decimal"]
+    return fhirtype in ["boolean", "integer", "string", "decimal", "number"]
 
 
 def map_align_arrays(arr1, arr2):
     """Maps two arrays to each other and aligns them in corresponding order.
 
     Args:
         arr1 (list): list of fhir elements
@@ -156,35 +159,90 @@
 
     Returns:
         arr1, arr2: Where arr1[i] corresponds to arr2[i]
     """
     warnings.warn("NotImplemented; arrays are assumed to be in identical order.")
     return match_list_len(arr1, arr2)
 
-def optimize_array_order(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails, max_perms=5040) -> tuple:
+def optimize_array_order(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails) -> tuple:
+    if len(fhir_true_array) <= MAX_PERMUTATIONS_ARRAY_SIZE:
+        return optimize_array_order_exact(fhir_true_array, fhir_pred_array, element_details)  # scales n!
+    else:
+        return optimize_array_order_approx(fhir_true_array, fhir_pred_array, element_details)  # scales n**2
+
+def optimize_array_order_exact(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails) -> tuple:
     """Finds the list order for fhir_pred the results in the highest accuracy by calculating all permutations
 
     Args:
         fhir_true_array (list): list of Fhir resources
         fhir_pred_array (list): list of Fhir resources to optimize
         element_details (ElementDetails): metadata
-        max_perms (int): maximum permutations to consider, defaults to 5040 (7!)
     """
     assert isinstance(fhir_true_array, list) and isinstance(fhir_pred_array, list), (fhir_true_array, fhir_pred_array)
-    fhir_pred_child_permutations = [list(permutation) for permutation in itertools.permutations(fhir_pred_array)][:max_perms]
+    fhir_pred_child_permutations = [list(permutation) for permutation in itertools.permutations(fhir_pred_array)]
     max_idx = -1
     max_accuracy = 0.
     for i, permutation in enumerate(fhir_pred_child_permutations):
         score = _get_array_score(fhir_true_array, permutation, element_details)
         if score.accuracy > max_accuracy:
             max_idx = i
             max_accuracy = score.accuracy
     fhir_pred_child_max = fhir_pred_child_permutations[max_idx]
     return fhir_true_array, fhir_pred_child_max
 
+def optimize_array_order_approx(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails) -> tuple:
+    """Finds the list order for fhir_pred the results in the highest accuracy using argmax with penalties
+
+    Args:
+        fhir_true_array (list): _description_
+        fhir_pred_array (list): _description_
+        element_details (ElementDetails): _description_
+
+    Returns:
+        tuple: _description_
+    """
+    accuracy_matrix = pd.DataFrame(0., index=np.arange(len(fhir_true_array)), columns=np.arange(len(fhir_pred_array)))
+    for i_true, fhir_true in enumerate(fhir_true_array):
+        for i_pred, fhir_pred in enumerate(fhir_pred_array):
+            diff = FhirDiff(
+            fhir_true=fhir_true,
+            fhir_pred=fhir_pred,
+            resource_name=element_details.array_item_type,
+            parent=None,
+            key=element_details.key,
+            )
+            diff = _expand_diff_tree(diff)
+            accuracy_matrix.iloc[i_true, i_pred] = diff.score.accuracy
+
+    optimal_order = get_optimal_order(accuracy_matrix)
+    fhir_pred_array_max = []
+    for target_idx in optimal_order:
+        fhir_pred_array_max.append(fhir_pred_array[target_idx])
+
+    return fhir_true_array, fhir_pred_array_max
+
+
+def get_optimal_order(accuracy_matrix):
+    """
+
+    Args:
+        matrix (_type_): _description_
+    """
+    epsilon = 0.01
+    marginal_distribution_pred = accuracy_matrix.mean(axis=0) + epsilon
+    marginal_distribution_true = accuracy_matrix.mean(axis=1) + epsilon
+    joint_distribution = np.dot(np.expand_dims(marginal_distribution_true, axis=1), np.expand_dims(marginal_distribution_pred, axis=0))
+
+    accuracy_ratio_matrix = accuracy_matrix / joint_distribution
+
+    optimal_order = accuracy_ratio_matrix.idxmax(axis=1)
+
+    return optimal_order
+
+
 def _get_array_score(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails) -> FhirScore:
     """Calculate FhirScore of fhir_pred_array in that particular order
 
     Args:
         fhir_true_array (list): list of Fhir resources
         fhir_pred_array (list): list of Fhir resources to optimize
         element_details (ElementDetails): metadata
@@ -280,15 +338,18 @@
 
     Args:
         diff (FhirDiff): comparison object containing the fhir to be compared
 
     Returns:
         FhirComparison: comparison with fhirscore attribute calculated.
     """
-    resource_type = get_resource_type(diff.fhir_true, diff.resource_name)
+    if diff.fhir_true:
+        resource_type = get_resource_type(diff.fhir_true, diff.resource_name)
+    else:
+        resource_type = get_resource_type(diff.fhir_pred, diff.resource_name)
 
     if fhirtype_is_leaf(resource_type):
         diff.score = compare_leaf(diff)
         return diff
 
     Resource = get_resource_class(
         resource_type
@@ -301,15 +362,15 @@
         # Skip if the element is absent in both fhir_true and fhir_pred.
         if (
             element_details.key not in diff.fhir_pred.keys()
             and element_details.key not in diff.fhir_true.keys()
         ):
             continue
         if (
-            element_is_absent(diff.fhir_true[element_details.key]) and element_is_absent(diff.fhir_true[element_details.key])
+            element_is_absent(diff.fhir_true[element_details.key]) and element_is_absent(diff.fhir_pred[element_details.key])
         ):
             continue
 
         # If the element is a struct (dictionary) with arbitrary depth, handle recursively
         if element_details.is_struct:
             _expand_diff_tree_struct(diff, element_details)
             childscore = diff.children[element_details.key].score
@@ -322,14 +383,18 @@
             )
 
         # If the element is a leaf, calculate the score directly
         elif element_details.is_leaf:
             _expand_diff_tree_leaf(diff, element_details)
             childscore = diff.children[element_details.key].score
 
+        else:
+            childscore = FhirScore()
+            warnings.warn(f"Details of element {element_details} could not be determined. \n fhir true: {diff.fhir_true} \n fhir pred: {diff.fhir_pred}")
+
         # Add the child node score to the current score
         diff.score = diff.score + childscore
 
     # diff.score.is_valid = validate_resource(diff.fhir_pred, diff.resource_type)
 
     return diff
 
@@ -456,15 +521,15 @@
         return FhirScore()
     if diff.key == "reference":
         element_true, element_pred = remove_id_from_reference(element_true), remove_id_from_reference(element_pred)
     if element_is_absent(element_pred) and element_is_absent(element_true):
         fhirscore = FhirScore()
     elif element_is_absent(element_pred):
         fhirscore = FhirScore(n_deletions=1, n_leaves=1)  # miss
-    elif element_is_absent(element_pred):
+    elif element_is_absent(element_true):
         fhirscore = FhirScore(n_additions=1, n_leaves=1)  # hallucination
     elif element_true != element_pred:
         fhirscore = FhirScore(n_modifications=1, n_leaves=1)  # mistake
     elif element_true == element_pred:
         fhirscore = FhirScore(n_matches=1, n_leaves=1)  # correct
     return fhirscore
```

### Comparing `healthsageai-0.1.2/src/healthsageai/note_to_fhir/evaluation/visuals.py` & `healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/visuals.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.2/src/healthsageai/note_to_fhir/inference/note_to_fhir.py` & `healthsageai-0.1.3/src/healthsageai/note_to_fhir/inference/note_to_fhir.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.2/src/healthsageai/note_to_fhir/parsers.py` & `healthsageai-0.1.3/src/healthsageai/note_to_fhir/parsers.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.2/src/healthsageai/note_to_fhir/templates/simple.py` & `healthsageai-0.1.3/src/healthsageai/note_to_fhir/templates/simple.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.2/src/healthsageai.egg-info/PKG-INFO` & `healthsageai-0.1.3/src/healthsageai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healthsageai
-Version: 0.1.2
+Version: 0.1.3
 Summary: HealthSage AI LLMs, Healthcare genAI platform
 Author-email: HealthSage AI <hello@healthsage.ai>
 Maintainer-email: HealthSage AI <hello@healthsage.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -723,15 +723,15 @@
 ## Inference: Note to FHIR
 
 You can do Note-to-fhir inference using our NoteToFhir class:
 
 ```python
 from healthsageai.note_to_fhir.inference import NoteToFhir13b
 
-model = NoteToFhir13b()  # NoteToFhir8x7b coming soon
+model = NoteToFhir13b()
 model.translate("Patient John Doe lives in Amsterdam")
 ```
 
 
 ## Evaluation of accuracy
 
 Our evaluation tool makes it easy to quantify and inspect the accuracy of generated FHIR resources w.r.t. a ground truth FHIR resource.
```

### Comparing `healthsageai-0.1.2/src/healthsageai.egg-info/SOURCES.txt` & `healthsageai-0.1.3/src/healthsageai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

