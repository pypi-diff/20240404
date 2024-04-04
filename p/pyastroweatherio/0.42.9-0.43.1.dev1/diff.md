# Comparing `tmp/pyastroweatherio-0.42.9.tar.gz` & `tmp/pyastroweatherio-0.43.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.42.9.tar", last modified: Fri Feb  9 05:41:49 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.43.1.dev1.tar", last modified: Thu Apr  4 15:29:42 2024, max compression
```

## Comparing `pyastroweatherio-0.42.9.tar` & `pyastroweatherio-0.43.1.dev1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-02-09 05:41:49.148634 pyastroweatherio-0.42.9/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.42.9/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1037 2024-02-09 05:41:49.148634 pyastroweatherio-0.42.9/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.42.9/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-02-09 05:41:49.144634 pyastroweatherio-0.42.9/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.42.9/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    31416 2024-02-09 05:41:27.000000 pyastroweatherio-0.42.9/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     1901 2023-11-05 13:15:21.000000 pyastroweatherio-0.42.9/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    19372 2023-11-12 11:14:38.000000 pyastroweatherio-0.42.9/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.42.9/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.42.9/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-02-09 05:41:49.148634 pyastroweatherio-0.42.9/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1037 2024-02-09 05:41:49.000000 pyastroweatherio-0.42.9/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-02-09 05:41:49.000000 pyastroweatherio-0.42.9/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-02-09 05:41:49.000000 pyastroweatherio-0.42.9/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-02-09 05:41:49.000000 pyastroweatherio-0.42.9/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-02-09 05:41:49.000000 pyastroweatherio-0.42.9/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-02-09 05:41:49.148634 pyastroweatherio-0.42.9/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1335 2024-02-09 05:41:36.000000 pyastroweatherio-0.42.9/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-04 15:29:42.766053 pyastroweatherio-0.43.1.dev1/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev1/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-04 15:29:42.766053 pyastroweatherio-0.43.1.dev1/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev1/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-04 15:29:42.758052 pyastroweatherio-0.43.1.dev1/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32176 2024-04-04 13:56:28.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3638 2024-04-04 14:01:19.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20083 2024-04-04 14:08:15.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-04 15:29:42.766053 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-04 15:29:42.766053 pyastroweatherio-0.43.1.dev1/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-04 15:28:31.000000 pyastroweatherio-0.43.1.dev1/setup.py
```

### Comparing `pyastroweatherio-0.42.9/LICENSE` & `pyastroweatherio-0.43.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.42.9/PKG-INFO` & `pyastroweatherio-0.43.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.42.9
+Version: 0.43.1.dev1
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.42.9/README.md` & `pyastroweatherio-0.43.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.42.9/pyastroweatherio/client.py` & `pyastroweatherio-0.43.1.dev1/pyastroweatherio/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """Define a client to interact with 7Timer."""
+
 import asyncio
 import json
 import logging
 import os.path
 import math
 from datetime import datetime, timedelta
 from typing import Optional
 from decimal import Decimal
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientError
 
+import pprint
+pp = pprint.PrettyPrinter()
+     
 from pyastroweatherio.const import (
     BASE_URL_SEVENTIMER,
     BASE_URL_MET,
+    HEADERS,
     DEFAULT_TIMEOUT,
     DEFAULT_CACHE_TIMEOUT,
     DEFAULT_ELEVATION,
     DEFAULT_TIMEZONE,
     DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
     DEFAULT_CONDITION_SEEING_WEIGHT,
     DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
+    DEFAULT_CONDITION_WIND_WEIGHT,
+    WIND10M_VALUE,
+    WIND10M_RANGE,
     HOME_LATITUDE,
     HOME_LONGITUDE,
     STIMER_OUTPUT,
     # FORECAST_TYPE_DAILY,
     FORECAST_TYPE_HOURLY,
     MAGNUS_COEFFICIENT_A,
     MAGNUS_COEFFICIENT_B,
@@ -49,14 +57,15 @@
         latitude=HOME_LATITUDE,
         longitude=HOME_LONGITUDE,
         elevation=DEFAULT_ELEVATION,
         timezone_info=DEFAULT_TIMEZONE,
         cloudcover_weight=DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
         seeing_weight=DEFAULT_CONDITION_SEEING_WEIGHT,
         transparency_weight=DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
+        wind_weight=DEFAULT_CONDITION_WIND_WEIGHT,
         uptonight_path="/conf/www",
         test_datetime=None,
     ):
         self._session: ClientSession = session
         self._latitude = latitude
         self._longitude = longitude
         self._elevation = elevation
@@ -68,14 +77,15 @@
         self._weather_data_uptonight = {}
         self._weather_data_seventimer_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
         self._weather_data_metno_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
         self._data_uptonight_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
         self._cloudcover_weight = cloudcover_weight
         self._seeing_weight = seeing_weight
         self._transparency_weight = transparency_weight
+        self._wind_weight = wind_weight
         self._uptonight_path = uptonight_path
         self._test_datetime = test_datetime
 
         self._forecast_data = None
 
         self.req = session
 
@@ -243,14 +253,15 @@
                     .get("precipitation_amount", "")
                 ),
                 # Condition
                 "condition_percentage": await self.calc_condition_percentage(
                     details.get("cloud_area_fraction", -1) / 12.5 + 1,
                     row["seeing"],
                     row["transparency"],
+                    details.get("wind_speed", -1),
                 ),
                 # Uptonight objects
                 "uptonight": await self._get_deepsky_objects(),
             }
 
             items.append(LocationData(item))
             break
@@ -327,22 +338,24 @@
                     item["cloudcover"] = int(details.get("cloud_area_fraction", -1) / 12.5 + 1)
 
                     item["cloud_area_fraction"] = details.get("cloud_area_fraction", -1)
                     item["cloud_area_fraction_high"] = details.get("cloud_area_fraction_high", -1)
                     item["cloud_area_fraction_low"] = details.get("cloud_area_fraction_low", -1)
                     item["cloud_area_fraction_medium"] = details.get("cloud_area_fraction_medium", -1)
                     item["fog_area_fraction"] = details.get("fog_area_fraction", -1)
+                    item["rh2m"] = details.get("relative_humidity", -1)
+                    item["wind_speed"] = details.get("wind_speed", -1)
 
                     item["condition_percentage"] = await self.calc_condition_percentage(
                         item["cloud_area_fraction"] / 12.5 + 1,
                         row["seeing"],
                         row["transparency"],
+                        item["wind_speed"],
                     )
-                    item["rh2m"] = details.get("relative_humidity", -1)
-                    item["wind_speed"] = details.get("wind_speed", -1)
+
                     item["wind_from_direction"] = details.get("wind_from_direction", -1)
                     item["temp2m"] = details.get("air_temperature", -1)
                     item["dewpoint2m"] = details.get("dew_point_temperature", -1)
                     if self._weather_data_metno[metno_index + cnt + i].get("data", {}).get("next_1_hours", {}) == {}:
                         # No more hourly data
                         break
                     if self._weather_data_metno[metno_index + cnt + i].get("data", {}).get("next_6_hours", {}) == {}:
@@ -417,52 +430,56 @@
         start_indexes = []
         # Find start index for two nights and store the indexes
         for idx, row in enumerate(self._forecast_data):
             if row.forecast_time.hour % 24 == sun_next_rising.hour and len(start_indexes) == 0:
                 start_indexes.append(0)
             if row.forecast_time.hour % 24 == sun_next_setting.hour:
                 start_indexes.append(idx)
-            
+
         forecast_data_len = len(self._forecast_data)
         for day in range(0, 2):
             start_forecast_hour = 0
             start_weather = ""
             interval_points = []
-            start_index = start_indexes[day] 
+            start_index = start_indexes[day]
             for idx in range(
                 start_index,
                 start_index + int(math.floor(night_duration_astronomical / 3600) + 2),
             ):
                 if idx >= forecast_data_len:
                     _LOGGER.debug("No more forecast data")
                     break
                 row = self._forecast_data[idx]
 
                 seeing = row.seeing
                 transparency = row.transparency
                 cloud_area_fraction = row.cloud_area_fraction_percentage / 12.5 + 1
+                wind_speed = row.wind10m_speed
 
                 if len(interval_points) == 0:
                     forecast_dayname = row.forecast_time.strftime("%A")
                     start_forecast_hour = row.forecast_time.hour
                     start_weather = row.weather6
 
                 _LOGGER.debug(
-                    "Idex: %d, Hour of day: %d, cloud_area_fraction: %s, seeing: %s, transparency: %s, condition: %s",
+                    "Idex: %d, Hour of day: %d, cloud_area_fraction: %s, seeing: %s, transparency: %s, wind_speed: %s, condition: %s",
                     idx,
                     row.forecast_time.hour,
                     str(cloud_area_fraction),
                     str(seeing),
                     str(transparency),
-                    await self.calc_condition_percentage(cloud_area_fraction, seeing, transparency),
+                    str(wind_speed),
+                    await self.calc_condition_percentage(cloud_area_fraction, seeing, transparency, wind_speed),
                 )
 
                 # Calculate Condition
                 if len(interval_points) <= int(math.floor(night_duration_astronomical / 3600)):
-                    interval_points.append(await self.calc_condition_percentage(cloud_area_fraction, seeing, transparency))
+                    interval_points.append(
+                        await self.calc_condition_percentage(cloud_area_fraction, seeing, transparency, wind_speed)
+                    )
 
                 if row.forecast_time.hour == sun_next_rising.hour or idx >= (forecast_data_len - 1):
                     item = {
                         "seventimer_init": init_ts,
                         "dayname": forecast_dayname,
                         "hour": start_forecast_hour,
                         "nightly_conditions": interval_points,
@@ -477,46 +494,57 @@
                         "Nightly conditions day: %s, start hour: %s, nightly conditions: %s, weather: %s, conditions numeric: %s",
                         str(forecast_dayname),
                         str(start_forecast_hour),
                         str(len(interval_points)),
                         str(start_weather),
                         conditions_numeric,
                     )
-                    
+
                     # Test for end of astronomical night. Will get true if we're already at night.
                     if row.forecast_time.hour % 24 == sun_next_rising.hour:
                         break
             start_index += 24
 
         return items
 
-    async def calc_condition_percentage(self, cloudcover, seeing, transparency):
-        """Return condition based on cloud cover, seeing and transparency"""
+    async def calc_condition_percentage(self, cloudcover, seeing, transparency, wind_speed):
+        """Return condition based on cloud cover, seeing, transparency, and wind speed"""
         # Possible Values:
         #   Clouds: 1-9
         #   Seeing: 1-8
         #   Transparency: 1-8
+        #   Wind: 1-8
+
+        wind_speed_value = 0
+        for (start, end), derate in zip(WIND10M_RANGE, WIND10M_VALUE):
+            if start <= wind_speed <= end:
+                wind_speed_value = derate
+
         condition = int(
             100
             - (
                 self._cloudcover_weight * cloudcover
                 + self._seeing_weight * seeing
                 + self._transparency_weight * transparency
+                + self._wind_weight * wind_speed_value
                 - self._cloudcover_weight
                 - self._seeing_weight
                 - self._transparency_weight
+                - self._wind_weight
             )
             * 100
             / (
                 self._cloudcover_weight * 9
                 + self._seeing_weight * 8
                 + self._transparency_weight * 8
+                + self._wind_weight * 8
                 - self._cloudcover_weight
                 - self._seeing_weight
                 - self._transparency_weight
+                - self._wind_weight
             )
         )
         # _LOGGER.debug(
         #     "Calc condition cloudcover: %d(%d), seeing %d(%d), transparency: %d(%d), condition %d",
         #     cloudcover,
         #     self._cloudcover_weight,
         #     seeing,
@@ -624,15 +652,15 @@
             + "&product="
             + str(product)
             + "&output="
             + STIMER_OUTPUT
         )
         try:
             _LOGGER.debug(f"Query url: {url}")
-            async with session.request(method, url) as resp:
+            async with session.request(method, url, headers=HEADERS) as resp:
                 resp.raise_for_status()
                 plain = str(await resp.text()).replace("\n", " ")
                 data = json.loads(plain)
 
                 if self._test_mode:
                     json_string = json.dumps(data)
                     with open("debug/" + product + ".json", "w") as outfile:
@@ -674,18 +702,15 @@
         else:
             _LOGGER.debug("Using cached data for Met.no")
 
     async def async_request_met(self, product="met", method="get") -> dict:
         """Make a request against the 7timer API."""
 
         use_running_session = self._session and not self._session.closed
-        headers = {
-            'User-Agent': 'AstroWeather github.com/mawinkler/astroweather'
-            }
-        
+
         if use_running_session:
             session = self._session
         else:
             session = ClientSession(
                 timeout=ClientTimeout(total=DEFAULT_TIMEOUT),
             )
 
@@ -697,15 +722,15 @@
             + "&lat="
             + str("%.1f" % round(self._latitude, 2))
             + "&altitude="
             + str(self._elevation)
         )
         try:
             _LOGGER.debug(f"Query url: {url}")
-            async with session.request(method, url, headers=headers) as resp:
+            async with session.request(method, url, headers=HEADERS) as resp:
                 resp.raise_for_status()
                 # plain = str(await resp.text()).replace("\n", " ")
                 # data = json.loads(plain)
                 data = await resp.json()
 
                 if self._test_mode:
                     json_string = json.dumps(data)
```

### Comparing `pyastroweatherio-0.42.9/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.43.1.dev1/pyastroweatherio/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
     CLOUDCOVER_PLAIN,
     CONDITION,
     CONDITION_PLAIN,
     DEEP_SKY_THRESHOLD,
     LIFTED_INDEX_PLAIN,
     SEEING_PLAIN,
     TRANSPARENCY_PLAIN,
+    WIND10M_PLAIN,
     WIND10M_DIRECTON,
+    WIND10M_VALUE,
+    WIND10M_RANGE,
 )
 
 
 class BaseData:
     """A representation of the base class for AstroWeather Data."""
 
     def __init__(self, data):
@@ -133,14 +136,19 @@
 
     @property
     def wind10m_speed(self) -> float:
         """Return 10m Wind Speed."""
         return self._wind_speed
 
     @property
+    def wind10m_speed_percentage(self) -> int:
+        """Return 10m Wind Speed."""
+        return int((100 + 100 / 7 - self._wind_speed * 100 / 7))
+    
+    @property
     def wind10m_direction(self) -> str:
         """Return 10m Wind Direction."""
         direction = self._wind_from_direction
         direction += 22.5
         direction = direction % 360
         direction = int(direction / 45)  # values 0 to 7
         return WIND10M_DIRECTON[direction]
@@ -251,14 +259,28 @@
         """Return Transparency."""
         transparency = self._transparency
         if transparency >= 1 and transparency <= 8:
             return TRANSPARENCY_PLAIN[self._transparency - 1]
         return None
 
     @property
+    def wind10m_speed_plain(self) -> str:
+        """Return Transparency."""
+        wind10m_speed = self._wind_speed
+        
+        wind_speed_value = 0
+        for (start, end), derate in zip(WIND10M_RANGE, WIND10M_VALUE):
+            if start <= wind10m_speed <= end:
+                wind_speed_value = derate
+                
+        if wind_speed_value >= 1 and wind_speed_value <= 8:
+            return WIND10M_PLAIN[wind_speed_value - 1]
+        return None
+    
+    @property
     def lifted_index_plain(self) -> str:
         """Return Lifted Index."""
 
         trans = {
             -10: LIFTED_INDEX_PLAIN[0],
             -6: LIFTED_INDEX_PLAIN[1],
             -4: LIFTED_INDEX_PLAIN[2],
```

### Comparing `pyastroweatherio-0.42.9/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.43.1.dev1/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.42.9/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.42.9
+Version: 0.43.1.dev1
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.42.9/setup.py` & `pyastroweatherio-0.43.1.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.42.9",
+    version="0.43.1.dev1",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

