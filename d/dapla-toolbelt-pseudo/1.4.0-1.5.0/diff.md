# Comparing `tmp/dapla_toolbelt_pseudo-1.4.0.tar.gz` & `tmp/dapla_toolbelt_pseudo-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-1.4.0.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-1.5.0.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-1.4.0.tar` & `dapla_toolbelt_pseudo-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1073 2024-03-22 08:46:55.399304 dapla_toolbelt_pseudo-1.4.0/LICENSE
--rw-r--r--   0        0        0    14605 2024-03-22 08:46:55.399304 dapla_toolbelt_pseudo-1.4.0/README.md
--rw-r--r--   0        0        0     4413 2024-03-22 08:47:06.439360 dapla_toolbelt_pseudo-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1369 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1430 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      994 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/exceptions.py
--rw-r--r--   0        0        0      847 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      781 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0     2042 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      469 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0     8869 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/api_models.py
--rw-r--r--   0        0        0     6385 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0    14600 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/depseudo.py
--rw-r--r--   0        0        0    14278 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/pseudo.py
--rw-r--r--   0        0        0     8724 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/pseudo_commons.py
--rw-r--r--   0        0        0     9240 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/result.py
--rw-r--r--   0        0        0     4188 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     5570 2024-03-22 08:46:55.403304 dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/validation.py
--rw-r--r--   0        0        0    16055 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-04 07:00:45.251307 dapla_toolbelt_pseudo-1.5.0/LICENSE
+-rw-r--r--   0        0        0    16351 2024-04-04 07:00:45.251307 dapla_toolbelt_pseudo-1.5.0/README.md
+-rw-r--r--   0        0        0     4433 2024-04-04 07:00:56.287341 dapla_toolbelt_pseudo-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1443 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      994 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/exceptions.py
+-rw-r--r--   0        0        0      847 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      781 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0     2125 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      543 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0     9856 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/api_models.py
+-rw-r--r--   0        0        0     2747 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/baseclass.py
+-rw-r--r--   0        0        0     6125 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0    14770 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/depseudo.py
+-rw-r--r--   0        0        0    14444 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/pseudo.py
+-rw-r--r--   0        0        0     8468 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/pseudo_commons.py
+-rw-r--r--   0        0        0    19398 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/repseudo.py
+-rw-r--r--   0        0        0     8396 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/result.py
+-rw-r--r--   0        0        0     4188 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     5634 2024-04-04 07:00:45.255307 dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/validation.py
+-rw-r--r--   0        0        0    17801 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.5.0/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/LICENSE` & `dapla_toolbelt_pseudo-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.4.0/README.md` & `dapla_toolbelt_pseudo-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -112,27 +112,26 @@
 result.to_polars()
 ```
 
 A `sid_snapshot_date` can also be specified to validate that the field values can be mapped to a SID at a specific date:
 
 ```python
 from dapla_pseudo import Validator
-from dapla_pseudo.utils import convert_to_date
 import polars as pl
 
 file_path="data/personer.csv"
 dtypes = {"fnr": pl.Utf8, "fornavn": pl.Utf8, "etternavn": pl.Utf8, "kjonn": pl.Categorical, "fodselsdato": pl.Utf8}
 
 df = pl.read_csv(file_path, dtypes=dtypes)
 
 result = (
     Validator.from_polars(df)
     .on_field("fnr")
     .validate_map_to_stable_id(
-        sid_snapshot_date=convert_to_date("2023-08-29")
+        sid_snapshot_date="2023-08-29"
     )
 )
 # Show metadata about the validation (e.g. which version of the SID catalog was used)
 result.metadata
 # Show the field values that didn't have a corresponding SID
 result.to_polars()
 ```
@@ -198,15 +197,14 @@
 df = (
     Pseudonymize.from_polars(df)                            # Specify what dataframe to use
     .on_fields("fornavn")                                   # Select the field to pseudonymize
     .with_default_encryption(custom_key="ssb-common-key-2") # Select the pseudonymization algorithm to apply
     .run()                                         # Apply pseudonymization to the selected field
     .to_polars()                                            # Get the result as a polars dataframe
 )
-pseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")
 
 # Pseudonymize a local file using a custom keyset:
 import json
 custom_keyset = PseudoKeyset(
     encrypted_keyset="CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",
     keyset_info={
         "primaryKeyId": 1234567890,
@@ -230,16 +228,15 @@
     .to_polars()
 )
 ```
 
 ### Depseudonymize
 
 The "Depseudonymize" functions are almost exactly the same as when pseudonymizing.
-The only difference being the lack of a "with_stable_id()"-function.
-This is to say, that you cannot map from Stable ID *back to* FNR as of Jan 2023.
+User can map from Stable ID *back to* FNR.
 
 ```python
 from dapla_pseudo import Depseudonymize
 import polars as pl
 
 file_path="data/personer_pseudonymized.csv"
 dtypes = {"fnr": pl.Utf8, "fornavn": pl.Utf8, "etternavn": pl.Utf8, "kjonn": pl.Categorical, "fodselsdato": pl.Utf8}
@@ -258,26 +255,56 @@
 result_df = (
     Depseudonymize.from_polars(df)                 # Specify what dataframe to use
     .on_fields("fornavn", "etternavn")             # Select multiple fields to depseudonymize
     .with_default_encryption()                     # Select the depseudonymization algorithm to apply
     .run()                                         # Apply depseudonymization to the selected fields
     .to_polars()                                   # Get the result as a polars dataframe
 )
+
+# Example: Depseudonymize Fnr field with SID mapping
+result_df = (
+    Depseudonymize.from_polars(df)                 # Specify what dataframe to use
+    .on_fields("fnr")                              # Select fnr field to depseudonymize
+    .with_stable_id()                              # Select the depseudonymization method (SID mapping) to apply
+    .run()                                         # Apply depseudonymization to the selected fields
+    .to_polars()                                   # Get the result as a polars dataframe
+)
+
 ```
 
 
 _Note that depseudonymization requires elevated access privileges._
 
 ### Repseudonymize
+Repseudonymize can either 1) Change the algorithm used to pseudonymize, and/or 2)
+change the key used in pseudonymization, while keeping the algorithm.
 
 ```python
-
-## TODO
+# Example: Repseudonymize from PAPIS-compatible encryption to Stable ID
+result_df = (
+    Repseudonymize.from_polars(df)                 # Specify what dataframe to use
+    .on_fields("fnr")                              # Select the field to pseudonymize
+    .from_papis_compatible_encryption()            # Select the pseudonymization algorithm previously used
+    .to_stable_id()                                # Select the new pseudonymization rule
+    .run()                                         # Apply pseudonymization to the selected field
+    .to_polars()                                   # Get the result as a polars dataframe
+)
 ```
 
+```python
+# Example: Repseudonymize with the same algorithm, but with a different key
+result_df = (
+    Repseudonymize.from_polars(df)                     # Specify what dataframe to use
+    .on_fields("fnr")                                  # Select the field to pseudonymize
+    .from_papis_compatible_encryption()                # Select the pseudonymization algorithm previously used
+    .to_papis_compatible_encryption(key_id="some-key") # Select the new pseudonymization rule
+    .run()                                             # Apply pseudonymization to the selected field
+    .to_polars()                                       # Get the result as a polars dataframe
+)
+```
 ### Datadoc
 
 Datadoc metadata is gathered while pseudonymizing, and can be seen like so:
 
 ```python
 result = (
     Pseudonymize.from_polars(df)
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/pyproject.toml` & `dapla_toolbelt_pseudo-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "1.4.0"
+version = "1.5.0"
 description = "Pseudonymization extensions for Dapla"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
@@ -92,14 +92,15 @@
     "gcsfs.core",
     "dapla",
     "fsspec",
     "fsspec.spec",
     "typeguard",
     "puremagic",
     "google.*",
+    "google.oauth2"
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 force-exclude = true  # Apply excludes to pre-commit
 show-fixes = true
 src = ["src", "tests"]
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 __version__ = version("dapla_toolbelt_pseudo")
 
 from dapla_pseudo.v1.api_models import Field
 from dapla_pseudo.v1.api_models import PseudoKeyset
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.depseudo import Depseudonymize
 from dapla_pseudo.v1.pseudo import Pseudonymize
+from dapla_pseudo.v1.repseudo import Repseudonymize
 from dapla_pseudo.v1.validation import Validator
 
 __all__ = [
     "PseudoClient",
     "Pseudonymize",
     "Depseudonymize",
+    "Repseudonymize",
     "Validator",
     "Field",
     "PseudoKeyset",
 ]
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/exceptions.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/types.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/types.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         )
         return matching_item[1]
     except StopIteration:
         return None
 
 
 def convert_to_date(sid_snapshot_date: t.Optional[date | str]) -> t.Optional[date]:
-    """Converts the SID version date to the 'date' type."""
+    """Converts the SID version date to the 'date' type, if it is a string.
+
+    If None, simply passes the None through the function.
+    """
     if isinstance(sid_snapshot_date, str):
         try:
             return date.fromisoformat(sid_snapshot_date)
         except ValueError as exc:
             raise ValueError(
                 "Version timestamp must be a valid ISO date string (YYYY-MM-DD)"
             ) from exc
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/api_models.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/api_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from humps import camelize
 from pydantic import BaseModel
 from pydantic import ConfigDict
 from pydantic import FieldSerializationInfo
 from pydantic import ValidationError
 from pydantic import field_serializer
+from pydantic import model_serializer
 
 from dapla_pseudo.constants import PredefinedKeys
 from dapla_pseudo.constants import PseudoFunctionTypes
 from dapla_pseudo.constants import UnknownCharacterStrategy
 from dapla_pseudo.models import APIModel
 
 
@@ -184,14 +185,19 @@
     function_type: PseudoFunctionTypes
     kwargs: DaeadKeywordArgs | FF31KeywordArgs | MapSidKeywordArgs | RedactArgs
 
     def __str__(self) -> str:
         """Create the function representation as expected by pseudo service."""
         return f"{self.function_type}({self.kwargs})"
 
+    @model_serializer()
+    def serialize_model(self) -> str:
+        """Serialize the function as expected by the pseudo service."""
+        return f"{self.function_type}({self.kwargs})"
+
 
 class PseudoRule(APIModel):
     """A ``PseudoRule`` defines a pattern, a transformation function, and optionally a friendly name of the rule.
 
     Each rule defines a glob pattern (see https://docs.oracle.com/javase/tutorial/essential/io/fileOps.html#glob)
     that identifies one or multiple fields, and a `func` that will be applied to the matching fields.
 
@@ -212,14 +218,43 @@
     def serialize_func(
         self, func: PseudoFunction, _info: FieldSerializationInfo
     ) -> str:
         """Explicit serialization of the 'func' field to coerce to string before serializing PseudoRule."""
         return str(func)
 
 
+class PseudoFieldRequest(APIModel):
+    """Model of the pseudo field request sent to the service."""
+
+    pseudo_func: PseudoFunction
+    name: str
+    values: list[str]
+    keyset: t.Optional[PseudoKeyset] = None
+
+
+class DepseudoFieldRequest(APIModel):
+    """Model of the depseudo field request sent to the service."""
+
+    pseudo_func: PseudoFunction
+    name: str
+    values: list[str]
+    keyset: t.Optional[PseudoKeyset] = None
+
+
+class RepseudoFieldRequest(APIModel):
+    """Model of the repseudo field request sent to the service."""
+
+    source_pseudo_func: PseudoFunction
+    target_pseudo_func: PseudoFunction
+    name: str
+    values: list[str]
+    source_keyset: t.Optional[PseudoKeyset] = None
+    target_keyset: t.Optional[PseudoKeyset] = None
+
+
 class PseudoConfig(APIModel):
     """PseudoConfig is a container for rules and keysets."""
 
     rules: list[PseudoRule]
     keysets: t.Optional[list[PseudoKeyset]] = None
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 import requests
 from dapla import AuthClient
 from ulid import ULID
 
 from dapla_pseudo.constants import TIMEOUT_DEFAULT
 from dapla_pseudo.constants import Env
 from dapla_pseudo.types import FileSpecDecl
+from dapla_pseudo.v1.api_models import DepseudoFieldRequest
 from dapla_pseudo.v1.api_models import DepseudonymizeFileRequest
 from dapla_pseudo.v1.api_models import Mimetypes
-from dapla_pseudo.v1.api_models import PseudoFunction
-from dapla_pseudo.v1.api_models import PseudoKeyset
+from dapla_pseudo.v1.api_models import PseudoFieldRequest
 from dapla_pseudo.v1.api_models import PseudonymizeFileRequest
+from dapla_pseudo.v1.api_models import RepseudoFieldRequest
 from dapla_pseudo.v1.api_models import RepseudonymizeFileRequest
 
 
 class PseudoClient:
     """Client for interacting with the Dapla Pseudo Service REST API."""
 
     pseudo_op_to_endpoint: t.ClassVar[dict[type, str]] = {
@@ -101,52 +102,40 @@
 
         PseudoClient._handle_response_error(response)
         return response
 
     def _post_to_field_endpoint(
         self,
         path: str,
-        field_name: str,
-        values: list[str],
-        pseudo_func: t.Optional[PseudoFunction],
+        pseudo_field_request: (
+            PseudoFieldRequest | DepseudoFieldRequest | RepseudoFieldRequest
+        ),
         timeout: int,
-        keyset: t.Optional[PseudoKeyset] = None,
         stream: bool = False,
     ) -> requests.Response:
-        request: dict[str, t.Any] = {
-            "request": {
-                "name": field_name,
-                "values": values,
-                "pseudoFunc": str(pseudo_func),
-            }
-        }
-        if keyset:
-            print(keyset.model_dump(by_alias=True))
-            request["request"]["keyset"] = keyset.model_dump(by_alias=True)
-
         response = requests.post(
             url=f"{self.pseudo_service_url}/{path}",
             headers={
                 "Authorization": f"Bearer {self.__auth_token()}",
                 "Content-Type": Mimetypes.JSON.value,
                 "X-Correlation-Id": PseudoClient._generate_new_correlation_id(),
             },
-            json=request,
+            json={"request": pseudo_field_request.model_dump_json(by_alias=True)},
             stream=stream,
             timeout=timeout,
         )
 
         PseudoClient._handle_response_error(response)
         return response
 
     def _post_to_sid_endpoint(
         self,
         path: str,
         values: list[str],
-        sid_snapshot_date: t.Optional[str | date] = None,
+        sid_snapshot_date: t.Optional[date] = None,
         stream: bool = False,
     ) -> requests.Response:
         request: dict[str, t.Collection[str]] = {"fnrList": values}
         response = requests.post(
             url=f"{self.pseudo_service_url}/{path}",
             params={"snapshot": str(sid_snapshot_date)} if sid_snapshot_date else None,
             # Do not set content-type, as this will cause the json to serialize incorrectly
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/depseudo.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/depseudo.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from dapla_pseudo.constants import TIMEOUT_DEFAULT
 from dapla_pseudo.constants import Env
 from dapla_pseudo.constants import PredefinedKeys
 from dapla_pseudo.constants import PseudoFunctionTypes
 from dapla_pseudo.types import FileLikeDatasetDecl
 from dapla_pseudo.utils import convert_to_date
 from dapla_pseudo.v1.api_models import DaeadKeywordArgs
+from dapla_pseudo.v1.api_models import DepseudoFieldRequest
 from dapla_pseudo.v1.api_models import DepseudonymizeFileRequest
 from dapla_pseudo.v1.api_models import FF31KeywordArgs
 from dapla_pseudo.v1.api_models import KeyWrapper
 from dapla_pseudo.v1.api_models import MapSidKeywordArgs
 from dapla_pseudo.v1.api_models import Mimetypes
 from dapla_pseudo.v1.api_models import PseudoConfig
 from dapla_pseudo.v1.api_models import PseudoFunction
@@ -184,22 +185,25 @@
                     field_name (str):  The name of the field.
                     series (pl.Series): The pandas Series containing the values to be pseudonymized.
                     pseudo_func (PseudoFunction): The pseudonymization function to apply to the values.
 
                 Returns:
                     tuple[str,pl.Series]: A tuple containing the field_name and the corresponding series.
                 """
+                request = DepseudoFieldRequest(
+                    pseudo_func=pseudo_func,
+                    keyset=KeyWrapper(self._pseudo_keyset).keyset,
+                    name=field_name,
+                    values=series.to_list(),
+                )
                 data, metadata = pseudonymize_operation_field(
                     path="depseudonymize/field",
-                    field_name=field_name,
-                    values=series.to_list(),
-                    pseudo_func=pseudo_func,
+                    pseudo_field_request=request,
                     timeout=self._timeout,
                     pseudo_client=self._pseudo_client,
-                    keyset=KeyWrapper(self._pseudo_keyset).keyset,
                 )
                 return field_name, data, metadata
 
             dataframe = t.cast(pl.DataFrame, Depseudonymize.dataset)
             # Execute the pseudonymization API calls in parallel
             with ThreadPoolExecutor() as executor:
                 depseudonymized_field: dict[str, pl.Series] = {}
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/pseudo.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/pseudo.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from dapla_pseudo.utils import convert_to_date
 from dapla_pseudo.v1.api_models import DaeadKeywordArgs
 from dapla_pseudo.v1.api_models import FF31KeywordArgs
 from dapla_pseudo.v1.api_models import KeyWrapper
 from dapla_pseudo.v1.api_models import MapSidKeywordArgs
 from dapla_pseudo.v1.api_models import Mimetypes
 from dapla_pseudo.v1.api_models import PseudoConfig
+from dapla_pseudo.v1.api_models import PseudoFieldRequest
 from dapla_pseudo.v1.api_models import PseudoFunction
 from dapla_pseudo.v1.api_models import PseudoKeyset
 from dapla_pseudo.v1.api_models import PseudonymizeFileRequest
 from dapla_pseudo.v1.api_models import PseudoRule
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.pseudo_commons import File
 from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
@@ -183,22 +184,25 @@
                     field_name (str):  The name of the field.
                     series (pl.Series): The pandas Series containing the values to be pseudonymized.
                     pseudo_func (PseudoFunction): The pseudonymization function to apply to the values.
 
                 Returns:
                     tuple[str,pl.Series]: A tuple containing the field_name and the corresponding series.
                 """
+                request = PseudoFieldRequest(
+                    pseudo_func=pseudo_func,
+                    keyset=KeyWrapper(self._pseudo_keyset).keyset,
+                    name=field_name,
+                    values=series.to_list(),
+                )
                 data, metadata = pseudonymize_operation_field(
                     path="pseudonymize/field",
-                    field_name=field_name,
-                    values=series.to_list(),
-                    pseudo_func=pseudo_func,
+                    pseudo_field_request=request,
                     timeout=self._timeout,
                     pseudo_client=self._pseudo_client,
-                    keyset=KeyWrapper(self._pseudo_keyset).keyset,
                 )
                 return field_name, data, metadata
 
             dataframe = t.cast(pl.DataFrame, Pseudonymize.dataset)
             # Execute the pseudonymization API calls in parallel
             with ThreadPoolExecutor() as executor:
                 pseudonymized_field: dict[str, pl.Series] = {}
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/pseudo_commons.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/pseudo_commons.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 
 from dapla_pseudo.exceptions import FileInvalidError
 from dapla_pseudo.exceptions import MimetypeNotSupportedError
 from dapla_pseudo.types import BinaryFileDecl
 from dapla_pseudo.types import FileLikeDatasetDecl
 from dapla_pseudo.types import FileSpecDecl
 from dapla_pseudo.utils import get_file_format_from_file_name
+from dapla_pseudo.v1.api_models import DepseudoFieldRequest
 from dapla_pseudo.v1.api_models import DepseudonymizeFileRequest
 from dapla_pseudo.v1.api_models import Mimetypes
-from dapla_pseudo.v1.api_models import PseudoFunction
-from dapla_pseudo.v1.api_models import PseudoKeyset
+from dapla_pseudo.v1.api_models import PseudoFieldRequest
 from dapla_pseudo.v1.api_models import PseudonymizeFileRequest
+from dapla_pseudo.v1.api_models import RepseudoFieldRequest
 from dapla_pseudo.v1.api_models import RepseudonymizeFileRequest
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.client import _client
 from dapla_pseudo.v1.client import _extract_name
 from dapla_pseudo.v1.supported_file_format import FORMAT_TO_MIMETYPE_FUNCTION
 
 
@@ -216,47 +217,40 @@
         streamed=True,
         file_name=file_name,
     )
 
 
 def pseudonymize_operation_field(
     path: str,
-    field_name: str,
-    values: list[str],
-    pseudo_func: t.Optional[PseudoFunction],
+    pseudo_field_request: (
+        PseudoFieldRequest | DepseudoFieldRequest | RepseudoFieldRequest
+    ),
     timeout: int,
     pseudo_client: PseudoClient,
-    keyset: t.Optional[PseudoKeyset] = None,
 ) -> tuple[pl.Series, RawPseudoMetadata]:
     """Makes pseudonymization API calls for a list of values for a specific field and processes it into a polars Series.
 
     Args:
         path (str): The path to the pseudonymization endpoint.
-        field_name (str): The name of the field being pseudonymized.
-        values (list[str]): The list of values to be pseudonymized.
-        pseudo_func (Optional[PseudoFunction]): The pseudonymization function to apply to the values.
+        pseudo_field_request: The request made to the Psuedo Service.
         timeout (int): The timeout in seconds for the API call.
         pseudo_client (PseudoClient): The instance of the pseudo_client used to make http requests.
-        keyset (Optional[PseudoKeyset], optional): The pseudonymization keyset to use. Defaults to None.
 
     Returns:
         pl.Series: A pandas Series containing the pseudonymized values.
     """
     response: requests.Response = pseudo_client._post_to_field_endpoint(
         path,
-        field_name,
-        values,
-        pseudo_func,
+        pseudo_field_request,
         timeout,
-        keyset,
         stream=True,
     )
     payload = json.loads(response.content.decode("utf-8"))
     data = payload["data"]
     metadata = RawPseudoMetadata(
-        field_name=field_name,
+        field_name=pseudo_field_request.name,
         logs=payload["logs"],
         metrics=payload["metrics"],
         datadoc=payload["datadoc_metadata"]["pseudo_variables"],
     )
 
     return pl.Series(data), metadata
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/result.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/result.py`

 * *Files 16% similar despite different names*

```diff
@@ -194,32 +194,12 @@
         """
         return self._datadoc.model_dump_json()
 
     def _datadoc_from_raw_metadata_fields(
         self,
         raw_metadata: list[dict[str, Any]],
     ) -> t.Optional[PseudoVariable]:
-        if len(raw_metadata) == 1:  # Only one element in list if NOT using SID-mapping
-            return PseudoVariable.model_validate(raw_metadata[0])
-        elif len(raw_metadata) == 2 and any(
-            "stable_identifier_type" in pseudo_var for pseudo_var in raw_metadata
-        ):  # SID-mapping
-            sid_metadata = next(
-                pseudo_var
-                for pseudo_var in raw_metadata
-                if "stable_identifier_type" in pseudo_var
-            )
-            encrypt_metadata = next(
-                pseudo_var
-                for pseudo_var in raw_metadata
-                if "stable_identifier_type" not in pseudo_var
-            )
-            pseudo_variable = PseudoVariable.model_validate(encrypt_metadata)
-            pseudo_variable.stable_identifier_type = sid_metadata[
-                "stable_identifier_type"
-            ]
-            pseudo_variable.stable_identifier_version = sid_metadata[
-                "stable_identifier_version"
-            ]
-            return pseudo_variable
-        else:
+        if len(raw_metadata) == 0:
             return None
+        elif len(raw_metadata) > 1:
+            print(f"Unexpected length of metadata: {len(raw_metadata)}")
+        return PseudoVariable.model_validate(raw_metadata[0])
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.4.0/src/dapla_pseudo/v1/validation.py` & `dapla_toolbelt_pseudo-1.5.0/src/dapla_pseudo/v1/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any
 from typing import Optional
 
 import pandas as pd
 import polars as pl
 import requests
 
+from dapla_pseudo.utils import convert_to_date
 from dapla_pseudo.utils import get_file_format_from_file_name
 from dapla_pseudo.v1.client import _client
 from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
 from dapla_pseudo.v1.pseudo_commons import RawPseudoMetadata
 from dapla_pseudo.v1.result import Result
 from dapla_pseudo.v1.supported_file_format import read_to_polars_df
 
@@ -111,15 +112,15 @@
 
             Returns:
                 Result: Containing a result dataframe with associated metadata.
             """
             response: requests.Response = _client()._post_to_sid_endpoint(
                 "sid/lookup/batch",
                 self._dataframe[self._field].to_list(),
-                sid_snapshot_date,
+                convert_to_date(sid_snapshot_date),
                 stream=True,
             )
             # The response content is received as a buffered byte stream from the server.
             # We decode the content using UTF-8, which gives us a List[Dict[str]] structure.
             result_json = json.loads(response.content.decode("utf-8"))[0]
             result: Sequence[str] = []
             metadata: list[str] = []
```

### Comparing `dapla_toolbelt_pseudo-1.4.0/PKG-INFO` & `dapla_toolbelt_pseudo-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 1.4.0
+Version: 1.5.0
 Summary: Pseudonymization extensions for Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -147,27 +147,26 @@
 result.to_polars()
 ```
 
 A `sid_snapshot_date` can also be specified to validate that the field values can be mapped to a SID at a specific date:
 
 ```python
 from dapla_pseudo import Validator
-from dapla_pseudo.utils import convert_to_date
 import polars as pl
 
 file_path="data/personer.csv"
 dtypes = {"fnr": pl.Utf8, "fornavn": pl.Utf8, "etternavn": pl.Utf8, "kjonn": pl.Categorical, "fodselsdato": pl.Utf8}
 
 df = pl.read_csv(file_path, dtypes=dtypes)
 
 result = (
     Validator.from_polars(df)
     .on_field("fnr")
     .validate_map_to_stable_id(
-        sid_snapshot_date=convert_to_date("2023-08-29")
+        sid_snapshot_date="2023-08-29"
     )
 )
 # Show metadata about the validation (e.g. which version of the SID catalog was used)
 result.metadata
 # Show the field values that didn't have a corresponding SID
 result.to_polars()
 ```
@@ -233,15 +232,14 @@
 df = (
     Pseudonymize.from_polars(df)                            # Specify what dataframe to use
     .on_fields("fornavn")                                   # Select the field to pseudonymize
     .with_default_encryption(custom_key="ssb-common-key-2") # Select the pseudonymization algorithm to apply
     .run()                                         # Apply pseudonymization to the selected field
     .to_polars()                                            # Get the result as a polars dataframe
 )
-pseudonymize(file_path="./data/personer.json", fields=["fnr", "fornavn"], key="ssb-common-key-1")
 
 # Pseudonymize a local file using a custom keyset:
 import json
 custom_keyset = PseudoKeyset(
     encrypted_keyset="CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",
     keyset_info={
         "primaryKeyId": 1234567890,
@@ -265,16 +263,15 @@
     .to_polars()
 )
 ```
 
 ### Depseudonymize
 
 The "Depseudonymize" functions are almost exactly the same as when pseudonymizing.
-The only difference being the lack of a "with_stable_id()"-function.
-This is to say, that you cannot map from Stable ID *back to* FNR as of Jan 2023.
+User can map from Stable ID *back to* FNR.
 
 ```python
 from dapla_pseudo import Depseudonymize
 import polars as pl
 
 file_path="data/personer_pseudonymized.csv"
 dtypes = {"fnr": pl.Utf8, "fornavn": pl.Utf8, "etternavn": pl.Utf8, "kjonn": pl.Categorical, "fodselsdato": pl.Utf8}
@@ -293,26 +290,56 @@
 result_df = (
     Depseudonymize.from_polars(df)                 # Specify what dataframe to use
     .on_fields("fornavn", "etternavn")             # Select multiple fields to depseudonymize
     .with_default_encryption()                     # Select the depseudonymization algorithm to apply
     .run()                                         # Apply depseudonymization to the selected fields
     .to_polars()                                   # Get the result as a polars dataframe
 )
+
+# Example: Depseudonymize Fnr field with SID mapping
+result_df = (
+    Depseudonymize.from_polars(df)                 # Specify what dataframe to use
+    .on_fields("fnr")                              # Select fnr field to depseudonymize
+    .with_stable_id()                              # Select the depseudonymization method (SID mapping) to apply
+    .run()                                         # Apply depseudonymization to the selected fields
+    .to_polars()                                   # Get the result as a polars dataframe
+)
+
 ```
 
 
 _Note that depseudonymization requires elevated access privileges._
 
 ### Repseudonymize
+Repseudonymize can either 1) Change the algorithm used to pseudonymize, and/or 2)
+change the key used in pseudonymization, while keeping the algorithm.
 
 ```python
-
-## TODO
+# Example: Repseudonymize from PAPIS-compatible encryption to Stable ID
+result_df = (
+    Repseudonymize.from_polars(df)                 # Specify what dataframe to use
+    .on_fields("fnr")                              # Select the field to pseudonymize
+    .from_papis_compatible_encryption()            # Select the pseudonymization algorithm previously used
+    .to_stable_id()                                # Select the new pseudonymization rule
+    .run()                                         # Apply pseudonymization to the selected field
+    .to_polars()                                   # Get the result as a polars dataframe
+)
 ```
 
+```python
+# Example: Repseudonymize with the same algorithm, but with a different key
+result_df = (
+    Repseudonymize.from_polars(df)                     # Specify what dataframe to use
+    .on_fields("fnr")                                  # Select the field to pseudonymize
+    .from_papis_compatible_encryption()                # Select the pseudonymization algorithm previously used
+    .to_papis_compatible_encryption(key_id="some-key") # Select the new pseudonymization rule
+    .run()                                             # Apply pseudonymization to the selected field
+    .to_polars()                                       # Get the result as a polars dataframe
+)
+```
 ### Datadoc
 
 Datadoc metadata is gathered while pseudonymizing, and can be seen like so:
 
 ```python
 result = (
     Pseudonymize.from_polars(df)
```

