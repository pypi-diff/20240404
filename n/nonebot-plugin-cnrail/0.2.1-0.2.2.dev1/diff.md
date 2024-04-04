# Comparing `tmp/nonebot_plugin_cnrail-0.2.1.tar.gz` & `tmp/nonebot_plugin_cnrail-0.2.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cnrail-0.2.1.tar", last modified: Thu Apr  4 09:04:51 2024, max compression
+gzip compressed data, was "nonebot_plugin_cnrail-0.2.2.dev1.tar", last modified: Thu Apr  4 17:10:15 2024, max compression
```

## Comparing `nonebot_plugin_cnrail-0.2.1.tar` & `nonebot_plugin_cnrail-0.2.2.dev1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/LICENSE
--rw-r--r--   0        0        0     4601 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/README.md
--rw-r--r--   0        0        0      681 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/__init__.py
--rw-r--r--   0        0        0     3938 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/__main__.py
--rw-r--r--   0        0        0      308 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/config.py
--rw-r--r--   0        0        0     5526 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/data_source.py
--rw-r--r--   0        0        0     5038 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/models.py
--rw-r--r--   0        0        0    15513 2024-04-04 09:04:38.484211 nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/templates/train_table.html.jinja
--rw-r--r--   0        0        0      808 2024-04-04 09:04:51.320196 nonebot_plugin_cnrail-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 nonebot_plugin_cnrail-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/LICENSE
+-rw-r--r--   0        0        0     4601 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/README.md
+-rw-r--r--   0        0        0      686 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/__init__.py
+-rw-r--r--   0        0        0     3938 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/__main__.py
+-rw-r--r--   0        0        0      308 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/config.py
+-rw-r--r--   0        0        0     5526 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/data_source.py
+-rw-r--r--   0        0        0     4830 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/models.py
+-rw-r--r--   0        0        0    15513 2024-04-04 17:10:03.300631 nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/templates/train_table.html.jinja
+-rw-r--r--   0        0        0      813 2024-04-04 17:10:15.252575 nonebot_plugin_cnrail-0.2.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0     5240 1970-01-01 00:00:00.000000 nonebot_plugin_cnrail-0.2.2.dev1/PKG-INFO
```

### Comparing `nonebot_plugin_cnrail-0.2.1/LICENSE` & `nonebot_plugin_cnrail-0.2.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.1/README.md` & `nonebot_plugin_cnrail-0.2.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/__init__.py` & `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.1"
+__version__ = "0.2.2.dev1"
 __plugin_meta__ = PluginMetadata(
     name="CNRail",
     description="查询 12306 列车时刻表",
     usage="使用指令 train -h 查看帮助",
     type="application",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/__main__.py` & `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/data_source.py` & `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/models.py` & `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime, timedelta
 from typing import List, Optional, Union
-
+from nonebot.log import logger
 import pytz
 from pydantic import BaseModel, Field
 
 TZ_SHANGHAI = pytz.timezone("Asia/Shanghai")
 
 
 class TrainSearchData(BaseModel):
@@ -86,34 +86,31 @@
     company_name: str = Field(alias="companyName")
     food_coach_name: Optional[str] = Field(alias="foodCoachName")
     via_stations: List[TrainDetailviaSation] = Field(alias="viaStations")
     cr_type: int = Field(alias="crType")
     routing: TrainDetailRouing
 
     def arrived(self, station_index: int, train_date: str) -> bool:  # 有待修改
-        # logger.debug(f"index: {station_index}, date: {train_date}")
-        # station = self.via_stations[station_index]
-        # arrive_time_str = (
-        #     station.arrival_time
-        #     if station.arrival_time is not None
-        #     else station.departure_time
-        # )
-        # arrive_datetime = (
-        #     datetime.fromisoformat(
-        #         f"{train_date}T{arrive_time_str}",
-        #     )
-        #     + timedelta(days=station.day_index)
-        # ).replace(tzinfo=TZ_SHANGHAI)
-        # if (arrive_datetime.month + 12 * (arrive_datetime.year - datetime.today().year)) > 3:
-        #     arrive_datetime = arrive_datetime.replace(year=arrive_datetime.year - 1)
-        # logger.debug(
-        #     f"arrive: {arrive_time_str}, arrive_datetime: {arrive_datetime}, now: {datetime.now(TZ_SHANGHAI)}, bool: {datetime.now(TZ_SHANGHAI) >= arrive_datetime}",
-        # )
-        # return datetime.now(TZ_SHANGHAI) >= arrive_datetime
-        return False
+        logger.debug(f"index: {station_index}, date: {train_date}")
+        station = self.via_stations[station_index]
+        arrive_time_str = (
+            station.arrival_time
+            if station.arrival_time is not None
+            else station.departure_time
+        )
+        arrive_datetime = (
+            datetime.fromisoformat(
+                f"{train_date}T{arrive_time_str}",
+            )
+            + timedelta(days=station.day_index)
+        ).replace(tzinfo=TZ_SHANGHAI)
+        logger.debug(
+            f"arrive: {arrive_time_str}, arrive_datetime: {arrive_datetime}, now: {datetime.now(TZ_SHANGHAI)}, bool: {datetime.now(TZ_SHANGHAI) >= arrive_datetime}",
+        )
+        return datetime.now(TZ_SHANGHAI) >= arrive_datetime
 
 
 class TrainSNData(BaseModel):
     train_sn: str = Field(alias="trainSN")
     date: str
     train_number: str = Field(alias="trainNumber")
```

### Comparing `nonebot_plugin_cnrail-0.2.1/nonebot_plugin_cnrail/templates/train_table.html.jinja` & `nonebot_plugin_cnrail-0.2.2.dev1/nonebot_plugin_cnrail/templates/train_table.html.jinja`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cnrail-0.2.1/pyproject.toml` & `nonebot_plugin_cnrail-0.2.2.dev1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "nonebot-plugin-alconna>=0.40.1",
     "nonebot-plugin-htmlrender>=0.2.2",
     "jinja2>=3.1.2",
     "pytz>=2023.3.post1",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.2.dev1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail"
```

### Comparing `nonebot_plugin_cnrail-0.2.1/PKG-INFO` & `nonebot_plugin_cnrail-0.2.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cnrail
-Version: 0.2.1
+Version: 0.2.2.dev1
 Summary: NoneBot2 plugin for query the train time table
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail
 Author-Email: student_2333 <lgc2333@126.com>, XieXiLin <support@xiexilin.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-cnrail
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cnrail Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cnrail Version: 0.2.2.dev1 Summary:
 NoneBot2 plugin for query the train time table Home-page: https://github.com/
 lgc-NB2Dev/nonebot-plugin-cnrail Author-Email: student_2333
 126.com>, XieXiLin
 xiexilin.com> License: MIT Project-URL: Homepage, https://github.com/lgc-
 NB2Dev/nonebot-plugin-cnrail Requires-Python: <4.0,>=3.9 Requires-Dist:
 nonebot2>=2.2.0 Requires-Dist: httpx>=0.24 Requires-Dist: nonebot-plugin-
 alconna>=0.40.1 Requires-Dist: nonebot-plugin-htmlrender>=0.2.2 Requires-Dist:
```

