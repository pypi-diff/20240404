# Comparing `tmp/LCPDelta-1.1.7.tar.gz` & `tmp/LCPDelta-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LCPDelta-1.1.7.tar", last modified: Tue Mar 12 16:56:35 2024, max compression
+gzip compressed data, was "LCPDelta-1.1.8.tar", last modified: Thu Apr  4 16:06:14 2024, max compression
```

## Comparing `LCPDelta-1.1.7.tar` & `LCPDelta-1.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 16:56:35.225183 LCPDelta-1.1.7/
--rw-rw-rw-   0        0        0      132 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     3425 2024-03-12 16:56:35.221647 LCPDelta-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2819 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/README.md
--rw-rw-rw-   0        0        0      686 2024-03-12 16:49:39.000000 LCPDelta-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 16:56:35.226194 LCPDelta-1.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-12 16:56:34.886041 LCPDelta-1.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-03-12 16:56:35.219644 LCPDelta-1.1.7/src/LCPDelta.egg-info/
--rw-rw-rw-   0        0        0     3425 2024-03-12 16:56:34.000000 LCPDelta-1.1.7/src/LCPDelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2024-03-12 16:56:34.000000 LCPDelta-1.1.7/src/LCPDelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 16:56:34.000000 LCPDelta-1.1.7/src/LCPDelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-03-12 16:56:34.000000 LCPDelta-1.1.7/src/LCPDelta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-12 16:56:34.000000 LCPDelta-1.1.7/src/LCPDelta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-12 16:56:35.005957 LCPDelta-1.1.7/src/lcp_delta/
--rw-rw-rw-   0        0        0       21 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-12 16:56:35.035672 LCPDelta-1.1.7/src/lcp_delta/common/
--rw-rw-rw-   0        0        0       39 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/common/__init__.py
--rw-rw-rw-   0        0        0     3462 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/common/api_helper.py
-drwxrwxrwx   0        0        0        0 2024-03-12 16:56:35.158485 LCPDelta-1.1.7/src/lcp_delta/enact/
--rw-rw-rw-   0        0        0      160 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/enact/__init__.py
--rw-rw-rw-   0        0        0    36094 2024-03-12 16:49:39.000000 LCPDelta-1.1.7/src/lcp_delta/enact/api_helper.py
--rw-rw-rw-   0        0        0     1790 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/enact/chart_helper.py
--rw-rw-rw-   0        0        0     4026 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/enact/credentials_holder.py
--rw-rw-rw-   0        0        0     7938 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/enact/dps_helper.py
-drwxrwxrwx   0        0        0        0 2024-03-12 16:56:35.178721 LCPDelta-1.1.7/src/lcp_delta/enact/response_objects/
--rw-rw-rw-   0        0        0      363 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/enact/response_objects/usage_info.py
-drwxrwxrwx   0        0        0        0 2024-03-12 16:56:35.217672 LCPDelta-1.1.7/src/lcp_delta/flextrack/
--rw-rw-rw-   0        0        0       91 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/flextrack/__init__.py
--rw-rw-rw-   0        0        0     3495 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/flextrack/api_helper.py
--rw-rw-rw-   0        0        0      626 2024-03-12 12:33:55.000000 LCPDelta-1.1.7/src/lcp_delta/global_helper_methods.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:06:14.050181 LCPDelta-1.1.8/
+-rw-rw-rw-   0        0        0      132 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3405 2024-04-04 16:06:14.048179 LCPDelta-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2799 2024-04-04 15:46:25.000000 LCPDelta-1.1.8/README.md
+-rw-rw-rw-   0        0        0      686 2024-04-04 15:46:25.000000 LCPDelta-1.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 16:06:14.051179 LCPDelta-1.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 16:06:13.684678 LCPDelta-1.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 16:06:14.045184 LCPDelta-1.1.8/src/LCPDelta.egg-info/
+-rw-rw-rw-   0        0        0     3405 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 16:06:13.797773 LCPDelta-1.1.8/src/lcp_delta/
+-rw-rw-rw-   0        0        0       21 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:06:13.830601 LCPDelta-1.1.8/src/lcp_delta/common/
+-rw-rw-rw-   0        0        0       39 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/common/__init__.py
+-rw-rw-rw-   0        0        0     3462 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/common/api_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:06:13.982180 LCPDelta-1.1.8/src/lcp_delta/enact/
+-rw-rw-rw-   0        0        0      160 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/__init__.py
+-rw-rw-rw-   0        0        0    46125 2024-04-04 15:58:29.000000 LCPDelta-1.1.8/src/lcp_delta/enact/api_helper.py
+-rw-rw-rw-   0        0        0     1790 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/chart_helper.py
+-rw-rw-rw-   0        0        0     4026 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/credentials_holder.py
+-rw-rw-rw-   0        0        0     7938 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/dps_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:06:14.000387 LCPDelta-1.1.8/src/lcp_delta/enact/response_objects/
+-rw-rw-rw-   0        0        0      363 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/response_objects/usage_info.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:06:14.041552 LCPDelta-1.1.8/src/lcp_delta/flextrack/
+-rw-rw-rw-   0        0        0       91 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/flextrack/__init__.py
+-rw-rw-rw-   0        0        0     3495 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/flextrack/api_helper.py
+-rw-rw-rw-   0        0        0      626 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/global_helper_methods.py
```

### Comparing `LCPDelta-1.1.7/PKG-INFO` & `LCPDelta-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LCPDelta
-Version: 1.1.7
+Version: 1.1.8
 Summary: LCPDelta Python Package
 Author-email: LCP Delta <enact.helpdesk@lcp.uk.com>
 Project-URL: Homepage, https://portal.lcpdelta.com/
 Keywords: LCPDelta,Enact,Flextrack,Storetrack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -102,11 +102,11 @@
     aggregation_types=['Average', 'Average'],
     granularity='Monthly'
 )
 
 response.head
 ```
 
-[Enact_instructions_link]: https://enact.lcp.energy/externalinstructions
+[Enact_instructions_link]: https://api.lcpdelta.com/
 [LCPDelta_data_portal_link]: https://portal.lcpdelta.com/
 [Enact_Homepage]: https://enact.lcpdelta.com/
 [FLEXtrack_Homepage]: https://flextrack.lcpdelta.com/
```

### Comparing `LCPDelta-1.1.7/README.md` & `LCPDelta-1.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,11 +83,11 @@
     aggregation_types=['Average', 'Average'],
     granularity='Monthly'
 )
 
 response.head
 ```
 
-[Enact_instructions_link]: https://enact.lcp.energy/externalinstructions
+[Enact_instructions_link]: https://api.lcpdelta.com/
 [LCPDelta_data_portal_link]: https://portal.lcpdelta.com/
 [Enact_Homepage]: https://enact.lcpdelta.com/
 [FLEXtrack_Homepage]: https://flextrack.lcpdelta.com/
```

### Comparing `LCPDelta-1.1.7/pyproject.toml` & `LCPDelta-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LCPDelta"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   { name="LCP Delta", email="enact.helpdesk@lcp.uk.com" },
 ]
 description = "LCPDelta Python Package"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["LCPDelta", "Enact", "Flextrack", "Storetrack"]
```

### Comparing `LCPDelta-1.1.7/src/LCPDelta.egg-info/PKG-INFO` & `LCPDelta-1.1.8/src/LCPDelta.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LCPDelta
-Version: 1.1.7
+Version: 1.1.8
 Summary: LCPDelta Python Package
 Author-email: LCP Delta <enact.helpdesk@lcp.uk.com>
 Project-URL: Homepage, https://portal.lcpdelta.com/
 Keywords: LCPDelta,Enact,Flextrack,Storetrack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -102,11 +102,11 @@
     aggregation_types=['Average', 'Average'],
     granularity='Monthly'
 )
 
 response.head
 ```
 
-[Enact_instructions_link]: https://enact.lcp.energy/externalinstructions
+[Enact_instructions_link]: https://api.lcpdelta.com/
 [LCPDelta_data_portal_link]: https://portal.lcpdelta.com/
 [Enact_Homepage]: https://enact.lcpdelta.com/
 [FLEXtrack_Homepage]: https://flextrack.lcpdelta.com/
```

### Comparing `LCPDelta-1.1.7/src/LCPDelta.egg-info/SOURCES.txt` & `LCPDelta-1.1.8/src/LCPDelta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.7/src/lcp_delta/common/api_helper.py` & `LCPDelta-1.1.8/src/lcp_delta/common/api_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.7/src/lcp_delta/enact/api_helper.py` & `LCPDelta-1.1.8/src/lcp_delta/enact/api_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,39 +33,72 @@
 
             option_id `list[str]`: If the selected Series has options, then this is the Enact ID for the requested Option, as defined in the query generator on the "General" tab. If this is not sent, then data for all options will be sent back (but capped to the first 10). Defaults to None.
 
             country_id `str` (optional): The country ID for filtering the data. Defaults to "Gb".
 
             half_hourly_average `bool` (optional): Flag to indicate whether to retrieve half-hourly average data. Defaults to False.
 
+            request_time_zone_id `str` (optional): The time zone ID of the requested time range.
+
+            time_zone_id `str` (optional): The time zone ID of the data to be returned (UTC by default).
+
             parse_datetimes `bool` (optional): Parse returned DataFrame index to DateTime (UTC). Defaults to False.
 
         Note that the arguments required for specific enact data can be found on the site.
 
         Returns:
             Response: The response object containing the series data.
         '''
         endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/Series/Data_V2'
 
         date_from = self.convert_date_time_to_right_format(date_from)
         date_to = self.convert_date_time_to_right_format(date_to)
+        return self.make_series_request(series_id, date_from, date_to, country_id, option_id, half_hourly_average, request_time_zone_id, time_zone_id, parse_datetimes, endpoint)
+
+    def get_series_info(self, series_id : str, country_id : str = None) -> dict:
+        '''Get information about a specific series.
+
+        This method retrieves information about a specific series based on the given series ID. Optional country ID can be provided to filter the series information.
+
+        Args:
+            series_id `str`: This is the Enact ID for the requested series, as defined in the query generator on the "General" tab.
+            country_id `str` (optional): The country ID to filter the series information. Defaults to None. If this is not provided, then details will be displayed for the first country available for this series.
+        '''
+        endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/Series/Info'
+        request_details = {
+            'SeriesId': series_id
+        }
+
+        if country_id is not None:
+            request_details['CountryId'] = country_id
+
+        response = self.post_request(endpoint, request_details)
+        return response
+
+    def make_series_request(self, series_id : str, date_from : datetime, date_to : datetime, country_id : str, option_id : list[str], half_hourly_average : bool, request_time_zone_id : str, time_zone_id : str, parse_datetimes : bool, endpoint : str) -> pd.DataFrame:
+        '''Make request for the series endpoints.
+
+        This method creates the request details from the user request.
+
+        Returns:
+             Response: The response object containing the series data.
+        '''
+        if option_id is not None:
+            if not is_list_of_strings(option_id):
+                raise Exception('Option ID input must be a list of strings')
 
         request_details = {
             'SeriesId': series_id,
             'CountryId': country_id,
             'From': date_from,
             'To': date_to,
+            'OptionId': option_id,
             'halfHourlyAverage': half_hourly_average
         }
 
-        if option_id is not None:
-            if not is_list_of_strings(option_id):
-                raise Exception('Option ID input must be a list of strings')
-            request_details['OptionId'] = option_id
-
         if request_time_zone_id is not None:
             request_details['requestTimeZoneId'] = request_time_zone_id
 
         if time_zone_id is not None:
             request_details['timeZoneId'] = time_zone_id
 
         response = self.post_request(endpoint, request_details)
@@ -79,33 +112,156 @@
                 if parse_datetimes:
                     parse_df_datetimes(df, True, inplace=True)
 
             return df
         except (ValueError, TypeError, IndexError):
             return response
 
-    def get_series_info(self, series_id : str, country_id : str = None) -> dict:
-        '''Get information about a specific series.
+    def get_series_by_fuel(self, series_id : str, date_from : datetime, date_to : datetime, country_id : str, option_id : str, half_hourly_average : bool = False, request_time_zone_id : str = None, time_zone_id : str = None, parse_datetimes : bool = False) -> pd.DataFrame:
+        '''Get series data for a specific plant series ID and a fuel type.
 
-        This method retrieves information about a specific series based on the given series ID. Optional country ID can be provided to filter the series information.
+        This method retrieves the series data for a specific series ID from the Enact API. It allows specifying the date range, option ID, half-hourly average, and country ID.
 
         Args:
             series_id `str`: This is the Enact ID for the requested series, as defined in the query generator on the "General" tab.
-            country_id `str` (optional): The country ID to filter the series information. Defaults to None. If this is not provided, then details will be displayed for the first country available for this series.
+
+            date_from `datetime.datetime`: This is the start of the date-range being requested. Defaults to today's date.
+
+            date_to `datetime.datetime`: This is the end of the date-range being requested. If a single day is wanted, then this will be the same as the From value. Defaults to today's date.
+
+            option_id `str`: This is the fuel option for the request e.g. 'Coal'.
+
+            country_id `str` (optional): The country ID for filtering the data. Defaults to "Gb".
+
+            half_hourly_average `bool` (optional): Flag to indicate whether to retrieve half-hourly average data. Defaults to False.
+
+            request_time_zone_id `str` (optional): The time zone ID of the requested time range.
+
+            time_zone_id `str` (optional): The time zone ID of the data to be returned (UTC by default).
+
+            parse_datetimes `bool` (optional): Parse returned DataFrame index to DateTime (UTC). Defaults to False.
+
+        Note that the arguments required for specific enact data can be found on the site.
+
+        Returns:
+            Response: The response object containing the series data.
         '''
-        endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/Series/Info'
-        request_details = {
-            'SeriesId': series_id
-        }
+        endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/Series/Fuel'
 
-        if country_id is not None:
-            request_details['CountryId'] = country_id
+        date_from = self.convert_date_time_to_right_format(date_from)
+        date_to = self.convert_date_time_to_right_format(date_to)
+        fuel_type = [option_id]
+        return self.make_series_request(series_id, date_from, date_to, country_id, fuel_type, half_hourly_average, request_time_zone_id, time_zone_id, parse_datetimes, endpoint)
 
-        response = self.post_request(endpoint, request_details)
-        return response
+    def get_series_by_zone(self, series_id : str, date_from : datetime, date_to : datetime, country_id : str, option_id : str, half_hourly_average : bool = False, request_time_zone_id : str = None, time_zone_id : str = None, parse_datetimes : bool = False) -> pd.DataFrame:
+        '''Get series data for a specific plant series ID and a zone.
+
+        This method retrieves the series data for a specific series ID from the Enact API. It allows specifying the date range, option ID, half-hourly average, and country ID.
+
+        Args:
+            series_id `str`: This is the Enact ID for the requested series, as defined in the query generator on the "General" tab.
+
+            date_from `datetime.datetime`: This is the start of the date-range being requested. Defaults to today's date.
+
+            date_to `datetime.datetime`: This is the end of the date-range being requested. If a single day is wanted, then this will be the same as the From value. Defaults to today's date.
+
+            option_id `str`: This is the zone option for the request e.g. 'Z1'.
+
+            country_id `str` (optional): The country ID for filtering the data. Defaults to "Gb".
+
+            half_hourly_average `bool` (optional): Flag to indicate whether to retrieve half-hourly average data. Defaults to False.
+
+            request_time_zone_id `str` (optional): The time zone ID of the requested time range.
+
+            time_zone_id `str` (optional): The time zone ID of the data to be returned (UTC by default).
+
+            parse_datetimes `bool` (optional): Parse returned DataFrame index to DateTime (UTC). Defaults to False.
+
+        Note that the arguments required for specific enact data can be found on the site.
+
+        Returns:
+            Response: The response object containing the series data.
+        '''
+        endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/Series/Zone'
+
+        date_from = self.convert_date_time_to_right_format(date_from)
+        date_to = self.convert_date_time_to_right_format(date_to)
+        zone = [option_id]
+        return self.make_series_request(series_id, date_from, date_to, country_id, zone, half_hourly_average, request_time_zone_id, time_zone_id, parse_datetimes, endpoint)
+
+    def get_series_by_owner(self, series_id : str, date_from : datetime, date_to : datetime, country_id : str, option_id : str, half_hourly_average : bool = False, request_time_zone_id : str = None, time_zone_id : str = None, parse_datetimes : bool = False) -> pd.DataFrame:
+        '''Get series data for a specific plant series ID and an owner.
+
+        This method retrieves the series data for a specific series ID from the Enact API. It allows specifying the date range, option ID, half-hourly average, and country ID.
+
+        Args:
+            series_id `str`: This is the Enact ID for the requested series, as defined in the query generator on the "General" tab.
+
+            date_from `datetime.datetime`: This is the start of the date-range being requested. Defaults to today's date.
+
+            date_to `datetime.datetime`: This is the end of the date-range being requested. If a single day is wanted, then this will be the same as the From value. Defaults to today's date.
+
+            option_id `str`: This is the owner option for the request e.g. 'Adela Energy'.
+
+            country_id `str` (optional): The country ID for filtering the data. Defaults to "Gb".
+
+            half_hourly_average `bool` (optional): Flag to indicate whether to retrieve half-hourly average data. Defaults to False.
+
+            request_time_zone_id `str` (optional): The time zone ID of the requested time range.
+
+            time_zone_id `str` (optional): The time zone ID of the data to be returned (UTC by default).
+
+            parse_datetimes `bool` (optional): Parse returned DataFrame index to DateTime (UTC). Defaults to False.
+
+        Note that the arguments required for specific enact data can be found on the site.
+
+        Returns:
+            Response: The response object containing the series data.
+        '''
+        endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/Series/Owner'
+
+        date_from = self.convert_date_time_to_right_format(date_from)
+        date_to = self.convert_date_time_to_right_format(date_to)
+        owner = [option_id]
+        return self.make_series_request(series_id, date_from, date_to, country_id, owner, half_hourly_average, request_time_zone_id, time_zone_id, parse_datetimes, endpoint)
+
+    def get_series_multi_option(self, series_id : str, date_from : datetime, date_to : datetime, country_id : str, option_id : list[str] = None, half_hourly_average : bool = False, request_time_zone_id : str = None, time_zone_id : str = None, parse_datetimes : bool = False) -> pd.DataFrame:
+        '''Get series data for a specific series ID with multiple options available.
+
+        This method retrieves the series data for a specific series ID from the Enact API. It allows specifying the date range, option ID, half-hourly average, and country ID.
+
+        Args:
+            series_id `str`: This is the Enact ID for the requested series, as defined in the query generator on the "General" tab.
+
+            date_from `datetime.datetime`: This is the start of the date-range being requested. Defaults to today's date.
+
+            date_to `datetime.datetime`: This is the end of the date-range being requested. If a single day is wanted, then this will be the same as the From value. Defaults to today's date.
+
+            option_id `str`: Leave this blank to request all possible options for that series. Otherwise, fill the array with the options wanted e.g. ["Coal", "Wind"].
+
+            country_id `str` (optional): The country ID for filtering the data. Defaults to "Gb".
+
+            half_hourly_average `bool` (optional): Flag to indicate whether to retrieve half-hourly average data. Defaults to False.
+
+            request_time_zone_id `str` (optional): The time zone ID of the requested time range.
+
+            time_zone_id `str` (optional): The time zone ID of the data to be returned (UTC by default).
+
+            parse_datetimes `bool` (optional): Parse returned DataFrame index to DateTime (UTC). Defaults to False.
+
+        Note that the arguments required for specific enact data can be found on the site.
+
+        Returns:
+            Response: The response object containing the series data.
+        '''
+        endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/Series/multiOption'
+
+        date_from = self.convert_date_time_to_right_format(date_from)
+        date_to = self.convert_date_time_to_right_format(date_to)
+        return self.make_series_request(series_id, date_from, date_to, country_id, option_id, half_hourly_average, request_time_zone_id, time_zone_id, parse_datetimes, endpoint)
 
     # Plant Details:
     def get_plant_details_by_id(self, plant_id : str) -> dict:
         '''Get details of a plant based on the plant ID.
 
         This method retrieves details of a specific plant based on the provided plant ID.
         Args:
```

### Comparing `LCPDelta-1.1.7/src/lcp_delta/enact/chart_helper.py` & `LCPDelta-1.1.8/src/lcp_delta/enact/chart_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.7/src/lcp_delta/enact/credentials_holder.py` & `LCPDelta-1.1.8/src/lcp_delta/enact/credentials_holder.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.7/src/lcp_delta/enact/dps_helper.py` & `LCPDelta-1.1.8/src/lcp_delta/enact/dps_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.7/src/lcp_delta/flextrack/api_helper.py` & `LCPDelta-1.1.8/src/lcp_delta/flextrack/api_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.7/src/lcp_delta/global_helper_methods.py` & `LCPDelta-1.1.8/src/lcp_delta/global_helper_methods.py`

 * *Files identical despite different names*

