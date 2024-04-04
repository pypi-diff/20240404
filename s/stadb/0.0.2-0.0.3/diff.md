# Comparing `tmp/stadb-0.0.2.tar.gz` & `tmp/stadb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadb-0.0.2.tar", last modified: Thu Apr  4 10:55:18 2024, max compression
+gzip compressed data, was "stadb-0.0.3.tar", last modified: Thu Apr  4 14:36:30 2024, max compression
```

## Comparing `stadb-0.0.2.tar` & `stadb-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 10:55:18.839197 stadb-0.0.2/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.2/LICENSE
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-04 10:55:18.839197 stadb-0.0.2/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-04-04 10:42:11.000000 stadb-0.0.2/README.md
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-04-04 10:38:18.000000 stadb-0.0.2/pyproject.toml
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-04 10:55:18.839197 stadb-0.0.2/setup.cfg
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 10:55:18.839197 stadb-0.0.2/src/
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 10:55:18.839197 stadb-0.0.2/src/stadb/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.2/src/stadb/__init__.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1250 2024-04-04 10:27:53.000000 stadb-0.0.2/src/stadb/logger.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     3355 2024-04-04 10:30:39.000000 stadb-0.0.2/src/stadb/postgresql.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)    50745 2024-04-04 10:52:53.000000 stadb-0.0.2/src/stadb/sensorthings.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     7652 2024-04-04 10:34:28.000000 stadb-0.0.2/src/stadb/timescaledb.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     4355 2024-04-04 10:52:53.000000 stadb-0.0.2/src/stadb/utils.py
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 10:55:18.839197 stadb-0.0.2/src/stadb.egg-info/
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/SOURCES.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/dependency_links.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/requires.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/top_level.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.2/src/test.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 14:36:30.600966 stadb-0.0.3/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.3/LICENSE
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-04 14:36:30.600966 stadb-0.0.3/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-04-04 10:42:11.000000 stadb-0.0.3/README.md
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-04-04 14:36:22.000000 stadb-0.0.3/pyproject.toml
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-04 14:36:30.600966 stadb-0.0.3/setup.cfg
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 14:36:30.600966 stadb-0.0.3/src/
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 14:36:30.600966 stadb-0.0.3/src/stadb/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.3/src/stadb/__init__.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1262 2024-04-04 11:35:04.000000 stadb-0.0.3/src/stadb/logger.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     5895 2024-04-04 14:18:57.000000 stadb-0.0.3/src/stadb/postgresql.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    52882 2024-04-04 14:12:35.000000 stadb-0.0.3/src/stadb/sensorthings.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    12469 2024-04-04 12:39:51.000000 stadb-0.0.3/src/stadb/timescaledb.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     4356 2024-04-04 11:29:48.000000 stadb-0.0.3/src/stadb/utils.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 14:36:30.600966 stadb-0.0.3/src/stadb.egg-info/
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/SOURCES.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/dependency_links.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/requires.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/top_level.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.3/src/test.py
```

### Comparing `stadb-0.0.2/LICENSE` & `stadb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stadb-0.0.2/PKG-INFO` & `stadb-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.2
+Version: 0.0.3
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
```

### Comparing `stadb-0.0.2/README.md` & `stadb-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `stadb-0.0.2/pyproject.toml` & `stadb-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 
 
 [project]
 
 name = "stadb"  # REQUIRED, is the only field that cannot be marked as dynamic.
-version = "0.0.2"  # REQUIRED, although can be dynamic
+version = "0.0.3"  # REQUIRED, although can be dynamic
 description = "SensorThings API database connector for advanced functionalities"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["sta", "setuptools", "development", "sensorthings"]
 
 authors = [
```

### Comparing `stadb-0.0.2/src/stadb/logger.py` & `stadb-0.0.3/src/stadb/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.__log_colour = colour
 
     def warning(self, *args):
         mystr = YEL + "[%s] " % self.__logger_name + str(*args) + RST
         self.__logger.warning(mystr)
 
     def error(self, *args, exception=False):
-        mystr = "[%s] " % self.__logger_name + str(*args)
+        mystr = RED + "[%s] " % self.__logger_name + str(*args) + RST
         self.__logger.error(RED + mystr + RST)
         if exception:
             raise ValueError(mystr)
 
     def debug(self, *args):
         mystr = self.__log_colour + "[%s] " % self.__logger_name + str(*args) + RST
         self.__logger.debug(mystr)
```

### Comparing `stadb-0.0.2/src/stadb/sensorthings.py` & `stadb-0.0.3/src/stadb/sensorthings.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         varname = self.datastream_id_varname[datastream_id]
         return sensor_name, varname
 
     def __initialize_dicts(self):
         """
         Initialize the dicts used for quickly access to relations without querying the database
         """
+        self.info("Initializing internal structures...")
         # DATASTREAM -> SENSOR relation
         query = """
             select "DATASTREAMS"."ID" as datastream_id, "SENSORS"."ID" as sensor_id, "SENSORS"."NAME" as sensor_name, 
             "DATASTREAMS"."NAME" as datastream_name
             from "DATASTREAMS", "SENSORS" 
             where "DATASTREAMS"."SENSOR_ID" = "SENSORS"."ID" order by datastream_id asc;"""
         df = self.dataframe_from_query(query)
@@ -157,14 +158,16 @@
         df = self.dataframe_from_query(f'select "ID", "NAME" from "DATASTREAMS";')
         self.datastream_name_id = dataframe_to_dict(df, "NAME", "ID")
 
         # OBS_PROPERTY NAME -> OBS_PROPERTY ID
         df = self.dataframe_from_query('select "ID", "NAME" from "OBS_PROPERTIES";')
         self.obs_prop_name_id = dataframe_to_dict(df, "NAME", "ID")
 
+        self.datastream_fois = self.get_datastream_fois()
+
     def get_sensor_datastreams(self, sensor_id):
         """
         Returns a dataframe with all datastreams belonging to a sensor
         :param sensor_id: ID of a sensor
         :return: dataframe with datastreams ID, NAME and PROPERTIES
         """
         query = (f'select "ID" as id , "NAME" as name, "THING_ID" as thing_id, "OBS_PROPERTY_ID" AS obs_prop_id,'
@@ -270,14 +273,60 @@
         select_fields = f'"{fields[0]}"'
         for f in fields[1:]:
             select_fields += f', "{f}"'
 
         df = self.dataframe_from_query(f'select {select_fields} from "DATASTREAMS";')
         return dataframe_to_dict(df, "ID", "PROPERTIES")
 
+    def get_datastream_fois(self):
+        """
+        Generates a dictionary with key datastream_id and value foi_id. The FOI is determined by the following rules,
+        from higher priority to lower priority
+            1. Get the ID from the database LAST_FOI_ID
+            2. Look for a FOI that has the name name as the Datastream's THING
+        :return:
+        """
+
+        datastreams_things = self.dict_from_query(
+            'select "ID", "THING_ID" from "DATASTREAMS";'
+        )
+
+        query = '''
+        select "DATASTREAM_ID", "GEN_FOI_ID" from
+            (select "DATASTREAMS"."ID" AS "DATASTREAM_ID", "LOCATION_ID" from
+            "DATASTREAMS" join "THINGS_LOCATIONS" on "DATASTREAMS"."THING_ID" = "THINGS_LOCATIONS"."THING_ID") as q1
+            join
+            "LOCATIONS" as q2
+            on q1."LOCATION_ID" = q2."ID"
+        '''
+        df_gen_fois = self.dict_from_query(query)
+        query = '''
+        select
+            "THINGS"."ID" as thing_id, "FEATURES"."ID" as foi_id 
+        from "FEATURES" 
+        left join "THINGS" 
+        on
+            "THINGS"."NAME" = "FEATURES"."NAME";
+        '''
+        thing_foi = self.dict_from_query(query)
+        datastream_features = {}
+
+        for datastream_id, thing_id in datastreams_things.items():
+            # First option: FOI has been updated in the table
+            if datastream_id in df_gen_fois.keys() and df_gen_fois[datastream_id]:  # could be null...
+                datastream_features[datastream_id] = df_gen_fois[datastream_id]
+                continue
+            # Second option: FOI has the same name than a THING
+            elif thing_id in thing_foi.keys() and thing_foi[thing_id]:  # could be null...
+                datastream_features[datastream_id] = thing_foi[thing_id]
+                continue
+            else:
+                self.warning(f"Could not get FOI for datastream {datastream_id}! this may crash the code later")
+        return datastream_features
+
     def get_last_datastream_timestamp(self, datastream_id):
         """
         Returns a timestamp (pd.Timestamp) with the last data point from a certain datastream. If there's no data
         return None or pd.Timestamp
         """
 
         properties = self.datastream_properties[datastream_id]
@@ -443,16 +492,15 @@
         df = self.dataframe_from_query(query)
         table_names = df["table_name"].values
         if view_name in table_names:
             return True
         return False
 
     def dict_from_query(self, query, debug=False):
-        self.exec_query(query, debug=debug)
-        response = self.cursor.fetchall()
+        response = self.exec_query(query, debug=debug, fetch=True)
         if len(response) == 0:
             return {}
         elif len(response[0]) != 2:
             raise ValueError(f"Expected two fields in response, got {len(response[0])}")
 
         return {key: value for key, value in response}
 
@@ -1146,22 +1194,21 @@
         query = "SELECT \"ID\" FROM public.\"OBSERVATIONS\" ORDER BY \"ID\" DESC LIMIT 1"
         df = self.dataframe_from_query(query)
         #  Check if the table is empty
         if df.empty:
             return 0
         return int(df["ID"].values[0])
 
-def dataframe_to_dict(df, key, value):
-    """
-    Takes two columns of a dataframe and converts it to a dictionary
-    :param df: input dataframe
-    :param key: column name that will be the key
-    :param value: column name that will be the value
-    :return: dict
-    """
-
-    keys = df[key]
-    values = df[value]
-    d = {}
-    for i in range(len(keys)):
-        d[keys[i]] = values[i]
-    return d
+    def get_data_type(self, datastream_id):
+        """
+        Returns the data type of a datastream
+        :param datastream_id: (int) id of the datastream
+        :returns: (data_type: str, average: bool)
+        """
+        props = self.datastream_properties[datastream_id]
+        data_type = props["dataType"]
+        if "averagePeriod" in props.keys():
+            average = True
+        else:
+            average = False
+        return data_type, average
+
```

### Comparing `stadb-0.0.2/src/stadb/timescaledb.py` & `stadb-0.0.3/src/stadb/timescaledb.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 institution: Universitat Politècnica de Catalunya (UPC)
 email: enoc.martinez@upc.edu
 license: MIT
 created: 23/3/21
 """
 
 from .logger import LoggerSuperclass, PRL
-import rich
+import psycopg2
+import pandas as pd
 
 
 class TimescaleDB(LoggerSuperclass):
     def __init__(self, sta_db_connector, logger):
         """
         Creates a TimescaleDB object, which adds timeseries capabilities to the SensorThings Database.
         The following hypertables will be created:
@@ -28,14 +29,15 @@
         detections_table = "detections"
 
         LoggerSuperclass.__init__(self, logger, "TSDB", colour=PRL)
 
         self.db = sta_db_connector
         self.timeseries_hypertable = timeseries_table
         self.profiles_hypertable = profiles_table
+        self.detections_hypertable = detections_table
 
         default_interval = "30days"
 
         if not self.db.check_if_table_exists(self.timeseries_hypertable):
             self.info(f"TimescaleDB, initializing {self.timeseries_hypertable} as a hypertable")
             self.create_timeseries_hypertable(timeseries_table, chunk_interval_time=default_interval)
             self.add_compression_policy(timeseries_table, policy="30d")
@@ -158,22 +160,125 @@
         :param table: hypertable name
         :returns: tuple like (MBytes before, MBytes after, compression ratio)
         """
         df = self.db.dataframe_from_query(f"SELECT * FROM hypertable_compression_stats('{table}');")
         try:
             bytes_before = df["before_compression_total_bytes"].values[0]
         except IndexError:
-            rich.print(f"[yellow]Compression not set for table '{table}'")
+            self.warning(f"Compression not set for table '{table}'")
             bytes_before = -1
         try:
             bytes_after = df["after_compression_total_bytes"].values[0]
         except IndexError:
             bytes_after = -1
         if type(bytes_after) is type(None):
             return 0, 0, 0
         else:
             ratio = bytes_before/bytes_after
             return round(bytes_before/1e6, 2), round(bytes_after/1e6, 2), round(ratio, 2)
 
+    def insert_to_timeseries(self,  timestamp: str, value: float, qc_flag: int, datastream_id: int):
+        """
+        Insert a single data point into the timeseries hypertable
+        """
+        query = f"insert into timeseries (timestamp, value, qc_flag, datastream_id) VALUES('{timestamp}', " \
+                f"{value}, {qc_flag}, {datastream_id})"
+        try:
+            self.db.exec_query(query, fetch=False)
+        except psycopg2.errors.UniqueViolation as e:
+            return str(e)
+        return None
+
+    def insert_to_profiles(self, timestamp: str, depth: float, value: float, qc_flag: int, datastream_id: int, depth_precision=2):
+        """
+        Insert a single data point into the profiles hypertable
+        """
+        depth = round(float(depth), depth_precision)
+        query = f"insert into profiles (timestamp, depth, value, datastream_id) " \
+                 f"VALUES('{timestamp}', {depth}, {value}, {qc_flag}, {datastream_id})"
+        try:
+            self.db.exec_query(query, fetch=False)
+        except psycopg2.errors.UniqueViolation as e:
+            return str(e)
+        return None
+
+    def insert_to_detections(self, timestamp: str, value: int, datastream_id: int):
+        """
+        Insert a single data point into the timeseries hypertable
+        """
+        query = f"insert into detections (timestamp, value, datastream_id) VALUES('{timestamp}', " \
+                f"{value},{datastream_id})"
+        try:
+            self.db.exec_query(query, fetch=False)
+        except psycopg2.errors.UniqueViolation as e:
+            return str(e)
+        return None
+
+    # ---- Get data from hypertables ---- #
+
+    def get_timeseries_data(self, identifier, top=100, skip=0, ascending=True, debug=False, format="dataframe",
+                            filters="", orderby=""):
+        return self.get_data_from_hypertable(self.timeseries_hypertable, identifier, top=top, skip=skip,
+                                             ascending=ascending, debug=debug, format=format, filters=filters,
+                                             orderby=orderby)
+
+    def get_profiles_data(self, identifier, top=100, skip=0, ascending=True, debug=False, format="dataframe",
+                            filters="", orderby=""):
+        return self.get_data_from_hypertable(self.profiles_hypertable, identifier, top=top, skip=skip,
+                                             ascending=ascending, debug=debug, format=format, filters=filters,
+                                             orderby=orderby)
+    def get_detections_data(self, identifier, top=100, skip=0, ascending=True, debug=False, format="dataframe",
+                            filters="", orderby=""):
+        return self.get_data_from_hypertable(self.detections_hypertable, identifier, top=top, skip=skip,
+                                             ascending=ascending, debug=debug, format=format, filters=filters,
+                                             orderby=orderby)
+
+    def get_data_from_hypertable(self, hypertable, identifier, time_start="", time_end="", top=100, skip=0,
+                                 ascending=True, debug=False, format="dataframe", filters="", orderby=""):
+        """
+        Access the raw data table and exports all data between time_start and time_end
+        :param identifier: datastream name (str) or datastream id (int)
+        :param time_start: start time
+        :param time_end: end time (not included)
+        """
+        if type(identifier) is int:
+            pass
+        elif type(identifier) is str:  # if string, convert from name to ID
+            identifier = self.datastreams_ids[identifier]
+
+        query = f"select timestamp, value, qc_flag from {hypertable} where datastream_id = {identifier}"
+
+        if filters:
+            query += f" and {filters} "  # add custom filters
+
+        if time_start:
+            query += f" and timestamp >= '{time_start}'"
+        if time_end:
+            query += f" and timestamp <'{time_end}'"
+
+        if orderby:
+            query += f" {orderby}"
+        else:
+            if ascending:
+                query += " order by timestamp asc"
+            else:
+                query += " order by timestamp desc"
+
+        query = f"select * from ({query}) as e"
+        if skip:
+            query += f" offset {skip}"
+
+        query += f" limit {top};"
+
+        if format == "dataframe":
+            df = self.db.dataframe_from_query(query, debug=debug)
+            df["timestamp"] = pd.to_datetime(df["timestamp"], utc=True)
+            return df.set_index("timestamp")
+        elif format == "list":
+            return self.db.list_from_query(query, debug=debug)
+        else:
+            raise ValueError(f"format {format} not valid!")
+
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `stadb-0.0.2/src/stadb/utils.py` & `stadb-0.0.3/src/stadb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     keys = df[key]
     values = df[value]
     d = {}
     for i in range(len(keys)):
         d[keys[i]] = values[i]
     return d
 
+
 def slice_dataframes(df, max_rows=-1, frequency=""):
     """
     Slices input dataframe into multiple dataframe, making sure than every dataframe has at most "max_rows"
     :param df: input dataframe
     :param max_rows: max rows en every dataframe
     :param frequency: M for month, W for week, etc.
     :return: list with dataframes
```

### Comparing `stadb-0.0.2/src/stadb.egg-info/PKG-INFO` & `stadb-0.0.3/src/stadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.2
+Version: 0.0.3
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
```

