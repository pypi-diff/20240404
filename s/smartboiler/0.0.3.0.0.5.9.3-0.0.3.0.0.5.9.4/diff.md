# Comparing `tmp/smartboiler-0.0.3.0.0.5.9.3.tar.gz` & `tmp/smartboiler-0.0.3.0.0.5.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.5.9.3.tar", last modified: Thu Apr  4 10:53:57 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.5.9.4.tar", last modified: Thu Apr  4 12:07:46 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.5.9.3.tar` & `smartboiler-0.0.3.0.0.5.9.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:57.750521 smartboiler-0.0.3.0.0.5.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 10:53:57.750521 smartboiler-0.0.3.0.0.5.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:53:57.750521 smartboiler-0.0.3.0.0.5.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-04 10:53:56.000000 smartboiler-0.0.3.0.0.5.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:57.742521 smartboiler-0.0.3.0.0.5.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:57.746521 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:57.746521 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:57.750521 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/web_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-04 10:53:55.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:57.746521 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 10:53:57.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-04 10:53:57.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:53:57.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 10:53:57.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 10:53:57.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 10:53:57.000000 smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-04 12:07:44.000000 smartboiler-0.0.3.0.0.5.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.132151 smartboiler-0.0.3.0.0.5.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.5.9.3/PKG-INFO` & `smartboiler-0.0.3.0.0.5.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.5.9.3
+Version: 0.0.3.0.0.5.9.4
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.5.9.3/README.md` & `smartboiler-0.0.3.0.0.5.9.4/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/setup.py` & `smartboiler-0.0.3.0.0.5.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.5.9.3',  # Required
+    version='0.0.3.0.0.5.9.4',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/command_line.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/command_line.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/data_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,51 +120,51 @@
 
         # format datetime to YYYY-MM-DDTHH:MM:SSZ
         left_time_interval = f"'{left_time_interval.strftime('%Y-%m-%dT%H:%M:%SZ')}'"
         right_time_interval = f"'{right_time_interval.strftime('%Y-%m-%dT%H:%M:%SZ')}'"
 
         return {
         "water_flow": {
-            "sql_query": f'SELECT mean("value") AS "water_flow_L_per_minute_mean" FROM "{self.db_name}"."autogen"."L/min" WHERE time > {left_time_interval} AND time =< {right_time_interval} GROUP BY time({group_by_time_interval}) FILL(0)',
+            "sql_query": f'SELECT mean("value") AS "water_flow_L_per_minute_mean" FROM "{self.db_name}"."autogen"."L/min" WHERE time > {left_time_interval} AND time <= {right_time_interval} GROUP BY time({group_by_time_interval}) FILL(0)',
             "measurement": "L/min",
         },
         "water_temperature": {
-            "sql_query": f'SELECT mean("value") AS "water_temperature_mean" FROM "{self.db_name}"."autogen"."°C" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND ("entity_id"=\'{self.tmp_output_water_entity_id}\' OR "entity_id"=\'{self.tmp_output_water_entity_id_2}\') GROUP BY time({group_by_time_interval}) FILL(0)',
+            "sql_query": f'SELECT mean("value") AS "water_temperature_mean" FROM "{self.db_name}"."autogen"."°C" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND ("entity_id"=\'{self.tmp_output_water_entity_id}\' OR "entity_id"=\'{self.tmp_output_water_entity_id_2}\') GROUP BY time({group_by_time_interval}) FILL(0)',
             "measurement": "°C",
         },
         "temperature": {
-            "sql_query": f'SELECT mean("temperature") AS "outside_temperature_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND "domain"=\'weather\' AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
+            "sql_query": f'SELECT mean("temperature") AS "outside_temperature_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'weather\' AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
             "measurement": "state",
         },
         "humidity": {
-            "sql_query": f'SELECT mean("humidity") AS "outside_humidity_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND "domain"=\'weather\' AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
+            "sql_query": f'SELECT mean("humidity") AS "outside_humidity_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'weather\' AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
             "measurement": "state",
         },
         "wind_speed": {
-            "sql_query": f'SELECT mean("wind_speed") AS "outside_wind_speed_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
+            "sql_query": f'SELECT mean("wind_speed") AS "outside_wind_speed_mean" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'domov\' GROUP BY time({group_by_time_interval}) FILL(null)',
             "measurement": "state",
         },
         "presence": {
-            "sql_query": f'SELECT count(distinct("friendly_name_str")) AS "device_presence_distinct_count" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND "domain"=\'device_tracker\' AND "state"=\'home\' GROUP BY time({group_by_time_interval}) FILL(0)',
+            "sql_query": f'SELECT count(distinct("friendly_name_str")) AS "device_presence_distinct_count" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "state"=\'home\' GROUP BY time({group_by_time_interval}) FILL(0)',
             "measurement": "state",
         },
         "boiler_water_temperature": {
-            "sql_query": f'SELECT mean("value") AS "boiler_water_temperature_mean" FROM "{self.db_name}"."autogen"."°C" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND "entity_id"=\'{self.tmp_boiler_case_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
+            "sql_query": f'SELECT mean("value") AS "boiler_water_temperature_mean" FROM "{self.db_name}"."autogen"."°C" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'{self.tmp_boiler_case_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
             "measurement": "°C",
         },
         "boiler_relay_status": {
-            "sql_query": f'SELECT last("value") AS "boiler_relay_status" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND "entity_id"=\'{self.relay_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
+            "sql_query": f'SELECT last("value") AS "boiler_relay_status" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'{self.relay_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
             "measurement": "state",
         },
         "device_longitude": {
-            "sql_query": f'SELECT mean("longitude") AS "mean_longitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
+            "sql_query": f'SELECT mean("longitude") AS "mean_longitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
             "measurement": "state",
         },
         "device_latitude": {
-            "sql_query": f'SELECT mean("latitude") AS "mean_latitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time =< {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
+            "sql_query": f'SELECT mean("latitude") AS "mean_latitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
             "measurement": "state",
         },
         
     } 
 
     def haversine_dist(self, x1, x2, y1, y2):
         return haversine((x1, x2), (y1, y2), unit="km")
```

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/machine_learning_forecaster.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/main.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/main.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/optimization.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/optimization.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/static/style.css` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/static/style.css`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/templates/index.html` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/templates/index.html`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/utils.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/utils.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/web_server.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/web_server.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.5.9.3
+Version: 0.0.3.0.0.5.9.4
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.5.9.3/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

