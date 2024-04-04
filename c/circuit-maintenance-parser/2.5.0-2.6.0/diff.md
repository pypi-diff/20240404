# Comparing `tmp/circuit_maintenance_parser-2.5.0.tar.gz` & `tmp/circuit_maintenance_parser-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuit_maintenance_parser-2.5.0.tar", max compression
+gzip compressed data, was "circuit_maintenance_parser-2.6.0.tar", max compression
```

## Comparing `circuit_maintenance_parser-2.5.0.tar` & `circuit_maintenance_parser-2.6.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0     9113 2024-03-14 10:35:19.053112 circuit_maintenance_parser-2.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      533 2024-03-14 10:35:19.053112 circuit_maintenance_parser-2.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    10174 2024-03-14 10:35:19.053112 circuit_maintenance_parser-2.5.0/LICENSE
--rw-r--r--   0        0        0    22504 2024-03-14 10:35:19.053112 circuit_maintenance_parser-2.5.0/README.md
--rw-r--r--   0        0        0     2789 2024-03-14 10:35:19.053112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/__init__.py
--rw-r--r--   0        0        0     2250 2024-03-14 10:35:19.053112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/cli.py
--rw-r--r--   0        0        0      124 2024-03-14 10:35:19.053112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/constants.py
--rwxr-xr-x   0        0        0  4395375 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/data/worldcities.csv
--rw-r--r--   0        0        0     4226 2024-03-14 10:35:19.053112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/data.py
--rw-r--r--   0        0        0      800 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/errors.py
--rw-r--r--   0        0        0     8757 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/output.py
--rw-r--r--   0        0        0    17108 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parser.py
--rw-r--r--   0        0        0        0 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/__init__.py
--rw-r--r--   0        0        0     2905 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/aquacomms.py
--rw-r--r--   0        0        0     3350 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/aws.py
--rw-r--r--   0        0        0     4248 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/bso.py
--rw-r--r--   0        0        0    10731 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/cogent.py
--rw-r--r--   0        0        0     3802 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/colt.py
--rw-r--r--   0        0        0     3740 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/crowncastle.py
--rw-r--r--   0        0        0     7592 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/equinix.py
--rw-r--r--   0        0        0     3516 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/globalcloudxchange.py
--rw-r--r--   0        0        0     1766 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/google.py
--rw-r--r--   0        0        0     3438 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/gtt.py
--rw-r--r--   0        0        0     4574 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/hgc.py
--rw-r--r--   0        0        0     6373 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/lumen.py
--rw-r--r--   0        0        0     2812 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/megaport.py
--rw-r--r--   0        0        0     2826 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/momentum.py
--rw-r--r--   0        0        0     2935 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/netflix.py
--rw-r--r--   0        0        0     1778 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/openai.py
--rw-r--r--   0        0        0     4305 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/seaborn.py
--rw-r--r--   0        0        0     3926 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/sparkle.py
--rw-r--r--   0        0        0     7922 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/telstra.py
--rw-r--r--   0        0        0     5014 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/turkcell.py
--rw-r--r--   0        0        0     3056 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/verizon.py
--rw-r--r--   0        0        0     6746 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/zayo.py
--rw-r--r--   0        0        0     7830 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/processor.py
--rw-r--r--   0        0        0        0 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/processors/__init__.py
--rw-r--r--   0        0        0    17197 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/provider.py
--rw-r--r--   0        0        0     5385 2024-03-14 10:35:19.069112 circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/utils.py
--rw-r--r--   0        0        0     2983 2024-03-14 10:35:29.405205 circuit_maintenance_parser-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    23813 1970-01-01 00:00:00.000000 circuit_maintenance_parser-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     9918 2024-04-04 13:27:17.441703 circuit_maintenance_parser-2.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      533 2024-04-04 13:27:17.441703 circuit_maintenance_parser-2.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    10174 2024-04-04 13:27:17.441703 circuit_maintenance_parser-2.6.0/LICENSE
+-rw-r--r--   0        0        0    22633 2024-04-04 13:27:17.441703 circuit_maintenance_parser-2.6.0/README.md
+-rw-r--r--   0        0        0     2821 2024-04-04 13:27:17.441703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/__init__.py
+-rw-r--r--   0        0        0     2250 2024-04-04 13:27:17.441703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/cli.py
+-rw-r--r--   0        0        0      124 2024-04-04 13:27:17.441703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/constants.py
+-rwxr-xr-x   0        0        0  4395375 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/data/worldcities.csv
+-rw-r--r--   0        0        0     4226 2024-04-04 13:27:17.441703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/data.py
+-rw-r--r--   0        0        0      800 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/errors.py
+-rw-r--r--   0        0        0     9016 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/output.py
+-rw-r--r--   0        0        0    17328 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parser.py
+-rw-r--r--   0        0        0        0 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     2905 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/aquacomms.py
+-rw-r--r--   0        0        0     3350 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/aws.py
+-rw-r--r--   0        0        0     4248 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/bso.py
+-rw-r--r--   0        0        0    10731 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/cogent.py
+-rw-r--r--   0        0        0     3802 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/colt.py
+-rw-r--r--   0        0        0     3539 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/crowncastle.py
+-rw-r--r--   0        0        0     7592 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/equinix.py
+-rw-r--r--   0        0        0     3516 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/globalcloudxchange.py
+-rw-r--r--   0        0        0     1766 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/google.py
+-rw-r--r--   0        0        0     3438 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/gtt.py
+-rw-r--r--   0        0        0     4574 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/hgc.py
+-rw-r--r--   0        0        0     6373 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/lumen.py
+-rw-r--r--   0        0        0     2812 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/megaport.py
+-rw-r--r--   0        0        0     2826 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/momentum.py
+-rw-r--r--   0        0        0     2935 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/netflix.py
+-rw-r--r--   0        0        0     1778 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/openai.py
+-rw-r--r--   0        0        0     4305 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/seaborn.py
+-rw-r--r--   0        0        0     3926 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/sparkle.py
+-rw-r--r--   0        0        0     7922 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/telstra.py
+-rw-r--r--   0        0        0     5014 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/turkcell.py
+-rw-r--r--   0        0        0     3056 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/verizon.py
+-rw-r--r--   0        0        0     3067 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/windstream.py
+-rw-r--r--   0        0        0     6746 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/zayo.py
+-rw-r--r--   0        0        0     7830 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/processor.py
+-rw-r--r--   0        0        0        0 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/processors/__init__.py
+-rw-r--r--   0        0        0    18613 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/provider.py
+-rw-r--r--   0        0        0     6801 2024-04-04 13:27:17.457703 circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/utils.py
+-rw-r--r--   0        0        0     3058 2024-04-04 13:27:28.041791 circuit_maintenance_parser-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    23946 1970-01-01 00:00:00.000000 circuit_maintenance_parser-2.6.0/PKG-INFO
```

### Comparing `circuit_maintenance_parser-2.5.0/CHANGELOG.md` & `circuit_maintenance_parser-2.6.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 # Changelog
 
-## v.2.5.0 - 2024-03-13
+## v2.6.0 - 2024-04-04
+
+### Added
+
+- [#273](https://github.com/networktocode/circuit-maintenance-parser/pull/273) - Add iCal parsing to GTT/EXA
+- [#280](https://github.com/networktocode/circuit-maintenance-parser/pull/280) - Add new Windstream Parser
+
+### Changed
+
+- [#277](https://github.com/networktocode/circuit-maintenance-parser/pull/277) - Refactor the output validator `validate_empty_circuit`
+- [#281](https://github.com/networktocode/circuit-maintenance-parser/pull/281) Add the ability to support pydantic 1 and 2
+
+### Fixed
+
+- [#272](https://github.com/networktocode/circuit-maintenance-parser/pull/272) - Fix the logic in the output validator `validate_empty_circuit`
+- [#278](https://github.com/networktocode/circuit-maintenance-parser/pull/278) - Increase robustness of Crown Castle parsing
+
+## v2.5.0 - 2024-03-13
 
 ### Added
 
 - [#274](https://github.com/networktocode/circuit-maintenance-parser/pull/274) - Add Global Cloud XChange Parser
 
 ## v2.4.0 - 2024-02-20
```

### Comparing `circuit_maintenance_parser-2.5.0/CONTRIBUTING.md` & `circuit_maintenance_parser-2.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/LICENSE` & `circuit_maintenance_parser-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/README.md` & `circuit_maintenance_parser-2.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,42 +56,46 @@
 
 ### Supported Providers
 
 #### Supported providers using the BCOP standard
 
 - Arelion (previously Telia)
 - EuNetworks
+- EXA (formerly GTT) (\*)
 - NTT
 - PacketFabric
-- Telstra
+- Telstra (\*)
 
 #### Supported providers based on other parsers
 
 - AWS
 - AquaComms
 - BSO
 - Cogent
 - Colt
 - Crown Castle Fiber
 - Equinix
-- EXA (formerly GTT)
+- EXA (formerly GTT) (\*)
 - HGC
 - Global Cloud Xchange
 - Google
 - Lumen
 - Megaport
 - Momentum
 - Netflix (AS2906 only)
 - Seaborn
 - Sparkle
-- Telstra
+- Telstra (\*)
 - Turkcell
 - Verizon
+- Windstream
 - Zayo
 
+(\*) Providers in both lists, with BCOP standard and nonstandard parsers.
+
 > Note: Because these providers do not support the BCOP standard natively, maybe there are some gaps on the implemented parser that will be refined with new test cases. We encourage you to report related **issues**!
 
 #### LLM-powered Parsers
 
 The library supports an optional parser option leveraging Large Language Models (LLM) to provide best-effort parsing when the specific parsers have not been successful.
 
 > Warning: Some of these integrations, such as OpenAI, require of extras installations parameters. Check the [extras section](#extras)
```

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/__init__.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     PacketFabric,
     Seaborn,
     Sparkle,
     Telia,
     Telstra,
     Turkcell,
     Verizon,
+    Windstream,
     Zayo,
 )
 
 SUPPORTED_PROVIDERS = (
     GenericProvider,
     AquaComms,
     Arelion,
@@ -58,14 +59,15 @@
     PacketFabric,
     Seaborn,
     Sparkle,
     Telia,
     Telstra,
     Turkcell,
     Verizon,
+    Windstream,
     Zayo,
 )
 
 SUPPORTED_PROVIDER_NAMES = [provider.get_provider_type() for provider in SUPPORTED_PROVIDERS]
 SUPPORTED_ORGANIZER_EMAILS = [provider.get_default_organizer() for provider in SUPPORTED_PROVIDERS]
```

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/cli.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/cli.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/data/worldcities.csv` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/data/worldcities.csv`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/data.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/data.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/errors.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/errors.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/output.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 """
 
 import json
 from enum import Enum
 
 from typing import List
 
-from pydantic import field_validator, BaseModel, StrictStr, StrictInt, PrivateAttr
+try:
+    from pydantic import field_validator
+except ImportError:
+    # TODO: This exception handling is required for Pydantic 1.x compatibility. To be removed when the dependency is deprecated.
+    from pydantic import validator as field_validator  # type: ignore
+
+
+from pydantic import BaseModel, StrictStr, StrictInt, PrivateAttr
 
 
 class Impact(str, Enum):
     """Types of maintenance impact.
 
     - "NO-IMPACT" indicates that there is no expected impact to services in scope for the maintenance.
     - "REDUCED-REDUNDANCY" indicates that during the maintenance the services in scope are expected to continue
@@ -193,15 +200,15 @@
         return value
 
     @field_validator("circuits")
     @classmethod
     def validate_empty_circuits(cls, value, values):
         """Validate non-cancel notifications have a populated circuit list."""
         values = values.data
-        if len(value) < 1 and str(values["status"]) in ("CANCELLED", "COMPLETED"):
+        if len(value) < 1 and values["status"] not in (Status.CANCELLED, Status.COMPLETED):
             raise ValueError("At least one circuit has to be included in the maintenance")
         return value
 
     @field_validator("end")
     @classmethod
     def validate_end_time(cls, end, values):
         """Validate that End time happens after Start time."""
```

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parser.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,19 @@
 
     # TODO: move it to where it is used, Cogent parser
     _geolocator = Geolocator()
 
     @classmethod
     def get_data_types(cls) -> List[str]:
         """Return the expected data type."""
-        return cls._data_types.get_default()
+        try:
+            return cls._data_types.get_default()
+        except AttributeError:
+            # TODO: This exception handling is required for Pydantic 1.x compatibility. To be removed when the dependency is deprecated.
+            return cls._data_types
 
     @classmethod
     def get_name(cls) -> str:
         """Return the parser name."""
         return cls.__name__
 
     def parser_hook(self, raw: bytes, content_type: str) -> List[Dict]:
```

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/aquacomms.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/aquacomms.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/aws.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/aws.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/bso.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/bso.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/cogent.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/cogent.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/colt.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/colt.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/crowncastle.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/crowncastle.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,19 +52,16 @@
         return [data]
 
     def parse_strong(self, soup, data):
         """Parse the strong tags, to find summary and maintenance ID info."""
         for strong in soup.find_all("strong"):
             if strong.string.strip() == "Ticket Number:":
                 data["maintenance_id"] = strong.next_sibling.strip()
-            if strong.string.strip() == "Description:":
-                summary = strong.parent.next_sibling.next_sibling.contents[0].string.strip()
-                summary = re.sub(r"[\n\r]", "", summary)
-                data["summary"] = summary
-            if strong.string.strip().startswith("Work Description:"):
+            val = strong.string.strip()
+            if val == "Description:" or val.startswith("Work Description:"):
                 for sibling in strong.parent.next_siblings:
                     summary = "".join(sibling.strings)
                     summary = re.sub(r"[\n\r]", "", summary)
                     if summary != "":
                         data["summary"] = summary
                         break
```

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/equinix.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/equinix.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/globalcloudxchange.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/globalcloudxchange.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/google.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/google.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/gtt.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/gtt.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/hgc.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/hgc.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/lumen.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/lumen.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/megaport.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/megaport.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/momentum.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/momentum.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/netflix.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/netflix.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/openai.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/openai.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/seaborn.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/seaborn.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/sparkle.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/sparkle.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/telstra.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/telstra.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/turkcell.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/turkcell.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/verizon.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/verizon.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/parsers/zayo.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/parsers/zayo.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/processor.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/processor.py`

 * *Files identical despite different names*

### Comparing `circuit_maintenance_parser-2.5.0/circuit_maintenance_parser/provider.py` & `circuit_maintenance_parser-2.6.0/circuit_maintenance_parser/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     SubjectParserSeaborn1,
     SubjectParserSeaborn2,
 )
 from circuit_maintenance_parser.parsers.sparkle import HtmlParserSparkle1
 from circuit_maintenance_parser.parsers.telstra import HtmlParserTelstra1, HtmlParserTelstra2
 from circuit_maintenance_parser.parsers.turkcell import HtmlParserTurkcell1
 from circuit_maintenance_parser.parsers.verizon import HtmlParserVerizon1
+from circuit_maintenance_parser.parsers.windstream import HtmlParserWindstream1
 from circuit_maintenance_parser.parsers.zayo import HtmlParserZayo1, SubjectParserZayo1
 from circuit_maintenance_parser.processor import CombinedProcessor, GenericProcessor, SimpleProcessor
 from circuit_maintenance_parser.utils import rgetattr
 
 logger = logging.getLogger(__name__)
 
 
@@ -146,30 +147,46 @@
             (f"Failed creating Maintenance notification for {provider_name}.\nDetails:\n{error_message}"),
             related_exceptions=related_exceptions,
         )
 
     @classmethod
     def get_default_organizer(cls) -> str:
         """Expose default_organizer as class attribute."""
-        return cls._default_organizer.get_default()  # type: ignore
+        try:
+            return cls._default_organizer.get_default()  # type: ignore
+        except AttributeError:
+            # TODO: This exception handling is required for Pydantic 1.x compatibility. To be removed when the dependency is deprecated.
+            return cls._default_organizer
 
     @classmethod
     def get_default_processors(cls) -> List[GenericProcessor]:
         """Expose default_processors as class attribute."""
-        return cls._processors.get_default()  # type: ignore
+        try:
+            return cls._processors.get_default()  # type: ignore
+        except AttributeError:
+            # TODO: This exception handling is required for Pydantic 1.x compatibility. To be removed when the dependency is deprecated.
+            return cls._processors
 
     @classmethod
     def get_default_include_filters(cls) -> Dict[str, List[str]]:
         """Expose include_filter as class attribute."""
-        return cls._include_filter.get_default()  # type: ignore
+        try:
+            return cls._include_filter.get_default()  # type: ignore
+        except AttributeError:
+            # TODO: This exception handling is required for Pydantic 1.x compatibility. To be removed when the dependency is deprecated.
+            return cls._include_filter
 
     @classmethod
     def get_default_exclude_filters(cls) -> Dict[str, List[str]]:
         """Expose exclude_filter as class attribute."""
-        return cls._exclude_filter.get_default()  # type: ignore
+        try:
+            return cls._exclude_filter.get_default()  # type: ignore
+        except AttributeError:
+            # TODO: This exception handling is required for Pydantic 1.x compatibility. To be removed when the dependency is deprecated.
+            return cls._exclude_filter
 
     @classmethod
     def get_extended_data(cls):
         """Return the default data used to extend processed notification data.
 
         It's used when the data is not available in the notification itself
         """
@@ -303,18 +320,21 @@
     _default_organizer = PrivateAttr("noc-noreply@google.com")
 
 
 class GTT(GenericProvider):
     """EXA (formerly GTT) provider custom class."""
 
     # "Planned Work Notification", "Emergency Work Notification"
-    _include_filter = PrivateAttr({EMAIL_HEADER_SUBJECT: ["Work Notification"]})
+    _include_filter = PrivateAttr(
+        {"Icalendar": ["BEGIN"], "ical": ["BEGIN"], EMAIL_HEADER_SUBJECT: ["Work Notification"]}
+    )
 
     _processors: List[GenericProcessor] = PrivateAttr(
         [
+            SimpleProcessor(data_parsers=[ICal]),
             CombinedProcessor(data_parsers=[EmailDateParser, HtmlParserGTT1]),
         ]
     )
     _default_organizer = PrivateAttr("InfraCo.CM@exainfra.net")
 
 
 class HGC(GenericProvider):
@@ -445,14 +465,25 @@
         [
             CombinedProcessor(data_parsers=[EmailDateParser, HtmlParserVerizon1]),
         ]
     )
     _default_organizer = PrivateAttr("NO-REPLY-sched-maint@EMEA.verizonbusiness.com")
 
 
+class Windstream(GenericProvider):
+    """Windstream provider custom class."""
+
+    _processors: List[GenericProcessor] = PrivateAttr(
+        [
+            CombinedProcessor(data_parsers=[EmailDateParser, HtmlParserWindstream1]),
+        ]
+    )
+    _default_organizer = PrivateAttr("wci.maintenance.notifications@windstream.com")
+
+
 class Zayo(GenericProvider):
     """Zayo provider custom class."""
 
     _include_filter = {
         "text/html": ["Maintenance Ticket #"],
         "html": ["Maintenance Ticket #"],
     }
```

### Comparing `circuit_maintenance_parser-2.5.0/pyproject.toml` & `circuit_maintenance_parser-2.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuit-maintenance-parser"
-version = "v2.5.0"
+version = "v2.6.0"
 description = "Python library to parse Circuit Maintenance notifications and return a structured data back"
 authors = ["Network to Code <opensource@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/networktocode/circuit-maintenance-parser"
 repository = "https://github.com/networktocode/circuit-maintenance-parser"
 readme = "README.md"
 keywords = ["parser", "circuit", "maintenance"]
@@ -20,15 +20,15 @@
     "CONTRIBUTING.md",
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = ">=7.1, <9.0"
-pydantic = {version = ">= 2.0.0", extras = ["dotenv"]}
+pydantic = {version =  ">= 1.8.0, != 1.9.*, >= 1.10.4, < 3", extras = ["dotenv"]}
 icalendar = "^5.0.0"
 bs4 = "^0.0.2"
 lxml = "^4.6.2"
 geopy = "^2.1.0"
 timezonefinder = "^6.0.1"
 backoff = "^1.11.1"
 chardet = "^5"
@@ -81,14 +81,17 @@
     | dist
   )/
   | settings.py     # This is where you define files that should not be stylized by black
                      # the root of the project
 )
 '''
 
+[tool.pylint.master]
+ignore-patterns=[".venv"]
+
 [tool.pylint.basic]
 # No docstrings required for private methods (Pylint default), or for test_ functions, or for inner Meta classes.
 no-docstring-rgx="^(_|test_|Meta$)"
 extension-pkg-whitelist = [
     "pydantic",
 ]
```

### Comparing `circuit_maintenance_parser-2.5.0/PKG-INFO` & `circuit_maintenance_parser-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuit-maintenance-parser
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python library to parse Circuit Maintenance notifications and return a structured data back
 Home-page: https://github.com/networktocode/circuit-maintenance-parser
 License: Apache-2.0
 Keywords: parser,circuit,maintenance
 Author: Network to Code
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.8,<4.0
@@ -20,15 +20,15 @@
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: chardet (>=5,<6)
 Requires-Dist: click (>=7.1,<9.0)
 Requires-Dist: geopy (>=2.1.0,<3.0.0)
 Requires-Dist: icalendar (>=5.0.0,<6.0.0)
 Requires-Dist: lxml (>=4.6.2,<5.0.0)
 Requires-Dist: openai (>=1.2.4) ; extra == "openai"
-Requires-Dist: pydantic[dotenv] (>=2.0.0)
+Requires-Dist: pydantic[dotenv] (>=1.10.4,<3)
 Requires-Dist: timezonefinder (>=6.0.1,<7.0.0)
 Project-URL: Repository, https://github.com/networktocode/circuit-maintenance-parser
 Description-Content-Type: text/markdown
 
 # circuit-maintenance-parser
 
 `circuit-maintenance-parser` is a Python library that parses circuit maintenance notifications from Network Service Providers (NSPs), converting heterogeneous formats to a well-defined structured format.
@@ -87,42 +87,46 @@
 
 ### Supported Providers
 
 #### Supported providers using the BCOP standard
 
 - Arelion (previously Telia)
 - EuNetworks
+- EXA (formerly GTT) (\*)
 - NTT
 - PacketFabric
-- Telstra
+- Telstra (\*)
 
 #### Supported providers based on other parsers
 
 - AWS
 - AquaComms
 - BSO
 - Cogent
 - Colt
 - Crown Castle Fiber
 - Equinix
-- EXA (formerly GTT)
+- EXA (formerly GTT) (\*)
 - HGC
 - Global Cloud Xchange
 - Google
 - Lumen
 - Megaport
 - Momentum
 - Netflix (AS2906 only)
 - Seaborn
 - Sparkle
-- Telstra
+- Telstra (\*)
 - Turkcell
 - Verizon
+- Windstream
 - Zayo
 
+(\*) Providers in both lists, with BCOP standard and nonstandard parsers.
+
 > Note: Because these providers do not support the BCOP standard natively, maybe there are some gaps on the implemented parser that will be refined with new test cases. We encourage you to report related **issues**!
 
 #### LLM-powered Parsers
 
 The library supports an optional parser option leveraging Large Language Models (LLM) to provide best-effort parsing when the specific parsers have not been successful.
 
 > Warning: Some of these integrations, such as OpenAI, require of extras installations parameters. Check the [extras section](#extras)
```

