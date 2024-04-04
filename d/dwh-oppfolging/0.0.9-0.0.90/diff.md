# Comparing `tmp/dwh_oppfolging-0.0.9.tar.gz` & `tmp/dwh_oppfolging-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwh_oppfolging-0.0.9.tar", max compression
+gzip compressed data, was "dwh_oppfolging-0.0.90.tar", max compression
```

## Comparing `dwh_oppfolging-0.0.9.tar` & `dwh_oppfolging-0.0.90.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/LICENSE
--rw-r--r--   0        0        0       23 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/README.md
--rw-r--r--   0        0        0        0 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/__init__.py
--rw-r--r--   0        0        0        0 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/__init__.py
--rw-r--r--   0        0        0     6715 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/brreg_api_v1.py
--rw-r--r--   0        0        0     1837 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/brreg_api_v1_structs.py
--rw-r--r--   0        0        0      268 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/kafka_api_v1.py
--rw-r--r--   0        0        0     7371 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/oracle_api_v1.py
--rw-r--r--   0        0        0      865 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/secrets_api_v1.py
--rw-r--r--   0        0        0     8538 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/ssb_api_v1.py
--rw-r--r--   0        0        0      429 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/apis/ssb_api_v1_structs.py
--rw-r--r--   0        0        0        0 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/db/__init__.py
--rw-r--r--   0        0        0     2008 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/db/sql.py
--rw-r--r--   0        0        0      511 2023-01-11 09:28:29.546086 dwh_oppfolging-0.0.9/dwh_oppfolging/db/table.py
--rw-r--r--   0        0        0      771 2023-01-11 09:28:29.550086 dwh_oppfolging-0.0.9/dwh_oppfolging/misc/__init__.py
--rw-r--r--   0        0        0     1669 2023-01-11 09:28:29.550086 dwh_oppfolging-0.0.9/dwh_oppfolging/misc/datatypes.py
--rw-r--r--   0        0        0     2565 2023-01-11 09:28:29.550086 dwh_oppfolging-0.0.9/dwh_oppfolging/misc/transforms.py
--rw-r--r--   0        0        0      936 2023-01-11 09:28:29.550086 dwh_oppfolging-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.9/setup.py
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/LICENSE
+-rw-r--r--   0        0        0      325 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/README.md
+-rw-r--r--   0        0        0       22 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/__init__.py
+-rw-r--r--   0        0        0       14 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/airflow_api_v1.py
+-rw-r--r--   0        0        0     8543 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v1.py
+-rw-r--r--   0        0        0     4051 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v1_types.py
+-rw-r--r--   0        0        0    17798 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v2.py
+-rw-r--r--   0        0        0     2163 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/dbt_oracle_api_v1.py
+-rw-r--r--   0        0        0      422 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/generic_api_v1.py
+-rw-r--r--   0        0        0      741 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/kafka_api_v1.py
+-rw-r--r--   0        0        0    24608 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/kafka_api_v1_types.py
+-rw-r--r--   0        0        0    11838 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/oracle_api_v1.py
+-rw-r--r--   0        0        0      125 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/oracle_api_v1_types.py
+-rw-r--r--   0        0        0     2371 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/secrets_api_v1.py
+-rw-r--r--   0        0        0     6831 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/ssb_api_v1.py
+-rw-r--r--   0        0        0    11693 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/apis/ssb_api_v1_types.py
+-rw-r--r--   0        0        0        0 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/transforms/__init__.py
+-rw-r--r--   0        0        0     9224 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/transforms/datatypes.py
+-rw-r--r--   0        0        0     9521 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/dwh_oppfolging/transforms/functions.py
+-rw-r--r--   0        0        0     1661 2024-04-04 14:54:32.934125 dwh_oppfolging-0.0.90/pyproject.toml
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 dwh_oppfolging-0.0.90/PKG-INFO
```

### Comparing `dwh_oppfolging-0.0.9/LICENSE` & `dwh_oppfolging-0.0.90/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 NAV IT
+Copyright (c) 2023 NAV IT
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dwh_oppfolging-0.0.9/dwh_oppfolging/apis/brreg_api_v1.py` & `dwh_oppfolging-0.0.90/dwh_oppfolging/apis/brreg_api_v1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# pylint: disable=missing-module-docstring
+"brreg api"
 # pylint: disable=line-too-long
+import logging
 from typing import Generator
 from datetime import datetime
 import gzip
-import requests
-import ijson
-from dwh_oppfolging.misc.transforms import dict_to_string, string_to_sha256_hash, string_to_naive_norwegian_datetime
-from dwh_oppfolging.apis.brreg_api_v1_structs import PagedRequestForEmbeddedList, Update
+import requests # type: ignore
+import ijson # type: ignore
+from dwh_oppfolging.transforms.functions import json_to_string, string_to_sha256_hash, string_to_naive_norwegian_datetime
+from dwh_oppfolging.apis.brreg_api_v1_types import PagedRequestForEmbeddedList, Update, PagedRequestError, UnpagedRequestForEmbeddedList
 
 
 API_VERSION = 1
 API_NAME = "BRREG"
 UNIT_NAME_ENHET = "enheter"
 UNIT_NAME_UNDERENHET = "underenheter"
 
@@ -27,36 +28,37 @@
     """converts brreg date string to datetime"""
     if date is None:
         return None
     converted_date = string_to_naive_norwegian_datetime(date.replace("Z", "+00:00"))
     return converted_date
 
 
-def _build_update_struct(data: dict):
+def _build_update_struct_from_brreg_json(data: dict):
     """returns Update struct"""
     update = Update(
         data["organisasjonsnummer"],
         data["endringstype"],
         _convert_brreg_date(data["dato"]),
     )
     return update
 
 
 def _build_unit_record(update: Update, fact: dict, download_date: datetime):
     """returns row in dict form
     NB: may delete field in fact"""
     fact.pop("_links", None)
     fact.get("organisasjonsform", {}).pop("_links", None)
+    fact.pop("links", None)
     record = {}
     record["organisasjonsnummer"] = update.orgnr
     record["endringstype"] = update.change
     record["oppdatert_tid_kilde"] = update.last_modified
     record["api_versjon"] = API_VERSION
-    record["data"] = dict_to_string(fact)
-    record["sha256_hash"] = string_to_sha256_hash(record["data"] + record["oppdatert_tid_kilde"].isoformat())
+    record["data"] = json_to_string(fact)
+    record["sha256_hash"] = string_to_sha256_hash(record["data"])
     record["lastet_dato"] = download_date
     record["kildesystem"] = API_NAME
     return record
 
 
 def _get_unit_record_from_update_single(update: Update, unit_name: str, download_date: datetime):
     """returns a unit record
@@ -66,90 +68,126 @@
     response = requests.get(url, headers=headers, proxies={}, timeout=100)
     fact = response.json()
     return _build_unit_record(update, fact, download_date)
 
 
 def _get_unit_record_from_update_batch(orgnr_update_lkp: dict[str, Update], unit_name: str, download_date: datetime, page_size: int = 500):
     """Returns {orgnr: record} constructed by searching for details for orgs in given {orgnr: update}
-    NB: the dict of updates may have elements removed.
+    NB: if an orgnr is found, it is popped from the orgnr_update_lkp input dictionary
     Org details will not be found if the org has been deleted at any point in the past,
     as this seems to remove them from the search endpoint.
     """
+    logging.info(f"Making search request for detail/fact with orgnr param size: {len(orgnr_update_lkp)}")
     url = _BASE_URL + "/" + unit_name
     params = {
         "organisasjonsnummer": ",".join(orgnr for orgnr in orgnr_update_lkp),
         "sort": "organisasjonsnummer,ASC",
     }
     headers = _build_headers(unit_name)
     list_key = unit_name
-    orgnr_record_lkp = {}
+    orgnr_record_lkp: dict = {}
     for facts in PagedRequestForEmbeddedList(url, params, headers, {}, page_size, list_key, timeout=100):
         orgnr_record_lkp |= {
             fact["organisasjonsnummer"]:
                 _build_unit_record(orgnr_update_lkp.pop(fact["organisasjonsnummer"]), fact, download_date)
             for fact in facts
         }
 
     return orgnr_record_lkp
 
 
-def get_latest_records_for_unit(download_date: datetime, last_modified_date: datetime, unit_name: str, page_size=500):
+def get_latest_records_for_unit(
+        download_date: datetime,
+        last_modified_date: datetime,
+        unit_name: str, page_size=500,
+        orgnr_search: list[str] | None = None,
+) -> Generator[list, None, None]:
     """params:
         last_modified_date: smallest update date
         unit_name: enheter | undereneheter
-    returns list of records"""
+        orgnr: list[str] | None
+    returns list of records
+    
+    If specified, orgnr is a list of orgnrs,
+    and only these will be searced for. Every orgnr given this way
+    must be associated with the given unit_name.
+    NOTE: when searching for missing orgnr this way, it is recommended
+    to set last_modified_date far back into the past so that you are
+    guaranteed to find at least one update newer than it.
+    """
     url = _BASE_URL + "/oppdateringer/" + unit_name
     headers = _build_headers("oppdatering." + unit_name)
     list_key = "oppdaterte" + unit_name.capitalize()
     params = {"dato": last_modified_date.isoformat(timespec="milliseconds") + "Z"}
-    orgnr_record_lkp = {} # {orgnr from latest update for that orgnr: latest fact for that orgnr}
-    for updates in PagedRequestForEmbeddedList(url, params, headers, {}, page_size, list_key, timeout=100):
+    if orgnr_search is not None:
+        params |= {"organisasjonsnummer": ",".join(orgnr_search)}
+    orgnr_record_lkp: dict = {} # {orgnr from latest update for that orgnr: latest fact for that orgnr}
+
+    try:
+        iter_obj = PagedRequestForEmbeddedList(url, params, headers, {}, page_size, list_key, timeout=100)
+    except PagedRequestError:
+        logging.warning("Using unpaged request, as paged request will fail due to BRREG API limitations")
+        iter_obj = UnpagedRequestForEmbeddedList(url, params, headers, {}, size=page_size, list_key=list_key, timeout=100) # type: ignore
+
+    for updates in iter_obj:
         # only keep the latest updates for each orgnr
         # since updates is already sorted with ascending update id, we can just overwrite
-        orgnr_update_lkp = {update.orgnr: update for update in map(_build_update_struct, updates)}
+        orgnr_update_lkp = {update.orgnr: update for update in map(_build_update_struct_from_brreg_json, updates)}
 
         old_length = len(orgnr_update_lkp)
         orgnr_record_lkp_batch = _get_unit_record_from_update_batch(orgnr_update_lkp, unit_name, download_date)
         new_length = len(orgnr_update_lkp)
-        print(f"found {old_length - new_length} of {old_length} orgs with batched search")
-        print("appending remaining using single requests")
+        logging.info(f"found {new_length} / {old_length} orgs with batched search, remaining will be appened using single requests")
         orgnr_record_lkp_batch |= {
             orgnr: _get_unit_record_from_update_single(update, unit_name, download_date)
             for orgnr, update in orgnr_update_lkp.items()
         }
 
         orgnr_record_lkp |= orgnr_record_lkp_batch
 
-    return list(orgnr_record_lkp.values())
+    # handle orgnr we didn't find any updates for
+    # possibly because it was before update types were introduced, or it has been deleted..
+    if orgnr_search is not None:
+        missing_orgnrs = set(orgnr_search) - orgnr_record_lkp.keys()
+        if len(missing_orgnrs) > 0:
+            logging.warning(f"Found no updates for {len(missing_orgnrs)} requested orgnrs. Facts will be downloaded directly, updates set to unknown")
+            orgnr_record_lkp |= {
+                orgnr: _get_unit_record_from_update_single(
+                            Update(orgnr, "UKJENT", last_modified_date),
+                            unit_name, download_date,
+                        )
+                for orgnr in missing_orgnrs
+            }
+        else:
+            logging.info("All requested orgnrs found.")
+    yield list(orgnr_record_lkp.values())
 
 
-def stream_latest_records_for_unit_from_file(download_date: datetime, unit_name: str, batch_size: int = 1000) -> Generator[list, None, None]:
-    """yields [records] from large file
-        must be run some time after 5
+def stream_latest_records_for_unit_from_file(download_date: datetime, last_modified_date: datetime, unit_name: str, batch_size: int = 1000) -> Generator[list, None, None]:
+    """
+    yields [records] from large file, must be run some time after 5 brreg local time
+    useful for init loading table
     """
-    assert datetime.today().hour > 5, "too early"
-    updated_date_str = datetime.today().replace(hour=5, minute=0, second=0).isoformat(timespec="milliseconds")+"Z"
+    #updated_date_str = last_modified_date.isoformat(timespec="milliseconds")+"Z"
     url = _BASE_URL + "/" + unit_name + "/" + "lastned"
     headers = _build_headers(unit_name, "gzip")
-    print("requesting filestream from api")
+    logging.info("requesting filestream from api")
     with requests.get(url, headers=headers, proxies={}, stream=True, timeout=100) as response:
         response.raise_for_status()
-        print("decompressing filestream")
+        logging.info("decompressing filestream")
         with gzip.open(response.raw, "rb") as file:
             records = []
-            print("iterating over json objects")
+            logging.info("iterating over json objects")
             for record in ijson.items(file, "item"):  # type: ignore
                 records.append(
                     _build_unit_record(
-                        _build_update_struct(
-                            {
-                                "organisasjonsnummer": record["organisasjonsnummer"],
-                                "endringstype": "INIT",
-                                "dato": updated_date_str
-                            }
+                        Update(
+                            record["organisasjonsnummer"],
+                            "FLATFIL",
+                            last_modified_date,
                         ),
                         record,
                         download_date,
                     )
                 )
                 if len(records) >= batch_size:
                     yield records
```

