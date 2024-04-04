# Comparing `tmp/salientsdk-0.1.3.tar.gz` & `tmp/salientsdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salientsdk-0.1.3.tar", max compression
+gzip compressed data, was "salientsdk-0.1.4.tar", max compression
```

## Comparing `salientsdk-0.1.3.tar` & `salientsdk-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1966 2024-03-29 18:02:05.700395 salientsdk-0.1.3/docs/index.md
--rw-r--r--   0        0        0     3248 2024-04-03 14:12:01.894776 salientsdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       20 2024-02-17 04:02:38.946553 salientsdk-0.1.3/salientsdk/.gitignore
--rw-r--r--   0        0        0     1109 2024-04-03 14:17:07.547244 salientsdk-0.1.3/salientsdk/__init__.py
--rw-r--r--   0        0        0     2166 2024-03-29 16:46:05.139009 salientsdk-0.1.3/salientsdk/constants.py
--rw-r--r--   0        0        0     7758 2024-03-29 16:47:56.698480 salientsdk-0.1.3/salientsdk/data_timeseries_api.py
--rw-r--r--   0        0        0     4359 2024-03-29 16:47:27.548528 salientsdk-0.1.3/salientsdk/downscale_api.py
--rw-r--r--   0        0        0     7855 2024-03-29 16:50:04.435033 salientsdk-0.1.3/salientsdk/forecast_timeseries_api.py
--rw-r--r--   0        0        0     7261 2024-03-28 17:09:58.717716 salientsdk-0.1.3/salientsdk/location.py
--rw-r--r--   0        0        0     3716 2024-03-29 16:53:46.365894 salientsdk-0.1.3/salientsdk/login_api.py
--rw-r--r--   0        0        0     4543 2024-03-29 16:49:19.732040 salientsdk-0.1.3/salientsdk/upload_file_api.py
--rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 salientsdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2650 2024-04-04 00:06:23.848471 salientsdk-0.1.4/docs/index.md
+-rw-r--r--   0        0        0     3213 2024-04-04 00:06:32.068557 salientsdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-04-04 00:06:23.848471 salientsdk-0.1.4/salientsdk/.gitignore
+-rw-r--r--   0        0        0     1721 2024-04-04 00:06:23.848471 salientsdk-0.1.4/salientsdk/__init__.py
+-rw-r--r--   0        0        0     8105 2024-04-04 00:06:23.848471 salientsdk-0.1.4/salientsdk/__main__.py
+-rw-r--r--   0        0        0     1708 2024-04-04 00:06:23.848471 salientsdk-0.1.4/salientsdk/constants.py
+-rw-r--r--   0        0        0     6693 2024-04-04 00:06:23.848471 salientsdk-0.1.4/salientsdk/data_timeseries_api.py
+-rw-r--r--   0        0        0     3329 2024-04-04 00:06:23.848471 salientsdk-0.1.4/salientsdk/downscale_api.py
+-rw-r--r--   0        0        0     6708 2024-04-04 00:06:23.848471 salientsdk-0.1.4/salientsdk/forecast_timeseries_api.py
+-rw-r--r--   0        0        0     4978 2024-04-04 00:06:23.848471 salientsdk-0.1.4/salientsdk/location.py
+-rw-r--r--   0        0        0     4551 2024-04-04 00:06:23.852471 salientsdk-0.1.4/salientsdk/login_api.py
+-rw-r--r--   0        0        0     4542 2024-04-04 00:06:23.852471 salientsdk-0.1.4/salientsdk/upload_file_api.py
+-rw-r--r--   0        0        0     3603 1970-01-01 00:00:00.000000 salientsdk-0.1.4/PKG-INFO
```

### Comparing `salientsdk-0.1.3/docs/index.md` & `salientsdk-0.1.4/docs/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 # Intended Use
 
-The Salient SDK is a convenience wrapper around Salient Predictions' customer-facing  
+The Salient SDK is a python convenience wrapper around Salient Predictions' customer-facing  
 [web API](https://api.salientpredictions.com/v2/documentation/api/).  It also contains utility functions for manipulating and analyzing the data delivered from the API.
 
 # Setting up the SDK
 
 ## Prerequisites 
 
 The Salient SDK requires Python 3.11 to use.   If you have Python installed, you can check your version with:
 
 ```bash
-python --version
+python3 --version
 ```
 
 To get version 3.11:
 
 ```bash
 # Ubuntu:
 sudo apt update
@@ -33,48 +33,58 @@
 ```
 
 ## Installing the SDK
 
 The easiest way to get the Salient SDK is to install it like any other package:
 
 ```bash
-pip install salientsdk
+pip install salientsdk --upgrade
+# to verify version with
+pip show salientsdk
 ```
 
+# Usage
 
+## Command Line
 
+The Salient SDK contains a full command line interface that can access each of the primary
+API functions without even opening python.  You can get help for all options or specific commands:
 
-
-
-
-# Usage
+```bash
+python3 -m salientsdk --help
+python3 -m salientsdk forecast_timeseries --help
+```
 
 To access the Salient API you will need a `username` and `password` provided by
 your Salient representative.  The universal credentials `testusr` and `testpwd` 
 have limited permissions for testing and validation purposes:
 
 ```bash
-python -m salientsdk.data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31 -u testusr -p testpwd
+python3 -m salientsdk data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31 -u testusr -p testpwd
 ```
 
-In a python script:
+## Via Python
+
+In a python 3.11 script, this example code will login and request a historical ERA5 data timeseries.
 
 ```python
 import salientsdk as sk
 import xarray as xr
 import netcdf4
 
 session = sk.login("testusr","testpwd")
-history = sk.data_timeseries(loc = Location(lat=42, lon=-73), field="all", variable="temp")
+history = sk.data_timeseries(loc = Location(lat=42, lon=-73), field="all", variable="temp", session=session)
 print(xr.open_file(history))
 ```
 
+Note that this example uses the limited credentials `testusr` and `testpwd`.  To access the full capabilities of your license, use your Salient-provided credentials.
+
 See all available functions in the [API Reference](api.md).
 
 The [examples](https://github.com/Salient-Predictions/salientsdk/tree/main/examples) directory contains `ipynb` notebooks to help you get started with common operations. 
 
 # License
 
-This SDK is licensed for use by Salient customers [details](LICENSE.md).
+This SDK is licensed for use by Salient customers [details](https://salient-predictions.github.io/salientsdk/LICENSE/).
 
 
 Copyright 2024 [Salient Predictions](https://www.salientpredictions.com/)
```

### Comparing `salientsdk-0.1.3/pyproject.toml` & `salientsdk-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salientsdk"
-version = "0.1.3"
+version = "0.1.4"
 description = "Salient Predictions Software Development Kit"
 authors = ["Salient Predictions <help@salientpredictions.com>"]
 license = "docs/LICENSE.md"
 readme = "docs/index.md"
 keywords = ["weather","climate","forecasting","sdk","salient","s2s"]
 homepage = "https://salientpredictions.com"
 documentation = "https://sdk.salientpredictions.com"
@@ -14,15 +14,15 @@
 # use "poetry add <packagename>" to edit this list
 h5netcdf = "^1.3.0"
 netCDF4 = "^1.6.5"
 pandas = "^2.2.1"
 python = "^3.11"
 requests = "^2.31.0"
 toml = "^0.10.2"
-xarray = {extras = ["h5netcdf"], version = "^2024.2.0"}
+xarray = "^2024.2.0"
 
 [tool.poetry.group.dev.dependencies]
 # use "poetry add --dev <packagename>" to edit this list
 google = "^3.0.0"
 google-cloud-secret-manager = "^2.19.0"
 markdown-include = "^0.8.1"
 mkdocs = "^1.5.3"
```

### Comparing `salientsdk-0.1.3/salientsdk/data_timeseries_api.py` & `salientsdk-0.1.4/salientsdk/data_timeseries_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,41 +7,43 @@
 observed data.  It also includes utility functions for operating on the returned data.
 
 Command line usage example:
 
 ```
 cd ~/salientsdk
 # this will get a single variable in a single file:
-python -m salientsdk.data_timeseries_api -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31
+python -m salientsdk data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31
 # this will get multiple variables in separate files:
-python -m salientsdk.data_timeseries_api -lat 42 -lon -73 -fld all -var temp,precip
+python -m salientsdk data_timeseries -lat 42 -lon -73 -fld all -var temp,precip
 ```
 
 """
 
 import os
 
 import requests
 import xarray as xr
 
-from . import constants, location, login_api
+from .constants import _build_url
+from .location import Location
+from .login_api import get_current_session, get_verify_ssl
 
 
 def data_timeseries(
-    loc: location.Location,
+    loc: Location,
     variable: str = "temp",
     field: str = "anom",
     debias: bool = False,
     start: str = "1950-01-01",
     end: str = "-today",
     format: str = "nc",
     frequency: str = "daily",
     force: bool = False,
-    session: requests.Session = constants.get_current_session(),
-    verify: bool = constants.VERFY_SSL,
+    session: requests.Session = get_current_session(),
+    verify: bool = get_verify_ssl(),
     verbose: bool = False,
     **kwargs,
 ) -> str | dict[str, str]:
     """Get a historical time series of ERA5 data.
 
     This function is a convenience wrapper to the Salient
     [API](https://api.salientpredictions.com/v2/documentation/api/#/Historical/get_data_timeseries).
@@ -131,15 +133,15 @@
         field=field,
         format=format,
         frequency=frequency,
         variable=variable,
         **kwargs,
     )
 
-    (query, file_name) = constants._build_url(endpoint, args)
+    (query, file_name) = _build_url(endpoint, args)
 
     if force or not os.path.exists(file_name):
         if verbose:
             print(f"Downloading {query} to {file_name}")
         with open(file_name, "wb" if format == "nc" else "w") as f:
             result = session.get(query, verify=verify)
             result.raise_for_status()
@@ -182,43 +184,7 @@
     # Would prefer to use xr.open_mfdataset, but we need to pass in the variable name
     # Can convert when history files have a short_name attribute
     # https://salientpredictions.atlassian.net/browse/RD-1184
     hst = xr.merge(
         [__extract_history_fields(files[variable], variable, fields) for variable in files.keys()]
     )
     return hst
-
-
-def _main() -> None:
-    argparser = location.Location.get_argparser(["debias", "force"])
-    argparser.add_argument("-var", "--variable", type=str, default="temp")
-    argparser.add_argument("-fld", "--field", type=str, default="anom")
-    argparser.add_argument("--start", type=str, default="1950-01-01")
-    argparser.add_argument("--end", type=str, default="-today")
-    argparser.add_argument("--format", type=str, default="nc")
-    argparser.add_argument("--frequency", type=str, default="daily")
-
-    args = argparser.parse_args()
-
-    session = login_api._login_from_args(args)
-
-    loc = location.Location._from_args_(args)
-    file_name = data_timeseries(
-        loc=loc,
-        variable=args.variable,
-        field=args.field,
-        debias=args.debias,
-        start=args.start,
-        end=args.end,
-        format=args.format,
-        frequency=args.frequency,
-        force=args.force,
-        verbose=args.verbose,
-        session=session,
-    )
-
-    if args.verbose and isinstance(file_name, str):
-        print(xr.open_dataset(file_name))
-
-
-if __name__ == "__main__":
-    _main()
```

### Comparing `salientsdk-0.1.3/salientsdk/downscale_api.py` & `salientsdk-0.1.4/salientsdk/downscale_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 # Copyright Salient Predictions 2024
 
 """Interface to the Salient data_timeseries API.
 
 Command line usage example:
 ```
 cd ~/salientsdk
-python -m salientsdk.downscale_api -lat 42 -lon -73 --date 2020-01-01
+python -m salientsdk downscale -lat 42 -lon -73 --date 2020-01-01
 ```
 
 """
 
 import os
 from datetime import datetime
 
 import requests
 import xarray as xr
 
-from . import constants, location, login_api
+from .constants import _build_url, get_model_version
+from .location import Location
+from .login_api import get_current_session, get_verify_ssl
 
 
 def downscale(
-    loc: location.Location,
+    loc: Location,
     variables: str = "temp,precip",
     debias: bool = False,
     date: str = "-today",
     members: int = 50,
-    version: str = constants.get_model_version(),
+    version: str = get_model_version(),
     force: bool = False,
-    session: requests.Session = constants.get_current_session(),
-    verify: bool = constants.VERFY_SSL,
+    session: requests.Session = get_current_session(),
+    verify: bool = get_verify_ssl(),
     verbose: bool = False,
     **kwargs,
 ) -> str | list[str]:
     """Temporal downscale of forecasts.
 
     Convert temporally coarse probabilistic forecasts into granular daily ensembles.
     For more detail, see the
@@ -81,15 +83,15 @@
         format=format,
         model=model,
         version=version,
         frequency=frequency,
         **kwargs,
     )
 
-    (query, file_name) = constants._build_url(endpoint, args)
+    (query, file_name) = _build_url(endpoint, args)
 
     if force or not os.path.exists(file_name):
         if verbose:
             print(f"Downloading {query} to {file_name}")
         with open(file_name, "wb" if format == "nc" else "w") as f:
             result = session.get(query, verify=verify)
             result.raise_for_status()
@@ -97,43 +99,7 @@
                 f.write(result.content)
             else:
                 f.write(result.text)
     elif verbose:
         print(f"File {file_name} already exists")
 
     return file_name
-
-
-def _main():
-    argparser = location.Location.get_argparser(["date", "debias", "version", "force"])
-    argparser.add_argument("-var", "--variables", type=str, default="temp,precip")
-    argparser.add_argument("--members", type=int, default=50)
-    # These are currently the only available values.  Not necessary to expose
-    # these as options from the command line.
-    # argparser.add_argument("--format", type=str, default="nc")
-    # argparser.add_argument("--frequency", type=str, default="daily")
-
-    args = argparser.parse_args()
-
-    session = login_api._login_from_args(args)
-
-    loc = location.Location._from_args_(args)
-    file_name = downscale(
-        loc,
-        variables=args.variables,
-        debias=args.debias,
-        date=args.date,
-        members=args.members,
-        version=args.version,
-        # format=args.format,
-        # frequency=args.frequency,
-        force=args.force,
-        verbose=args.verbose,
-        session=session,
-    )
-
-    if args.verbose:
-        print(xr.open_dataset(file_name))
-
-
-if __name__ == "__main__":
-    _main()
```

### Comparing `salientsdk-0.1.3/salientsdk/forecast_timeseries_api.py` & `salientsdk-0.1.4/salientsdk/forecast_timeseries_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,44 +7,47 @@
 probabilistic weather forecasts in subseasonal-to-seasonal timescales.
 
 Command line usage example:
 
 ```
 cd ~/salientsdk
 # this will get a single variable in a single file:
-python -m salientsdk.forecast_timeseries_api -lat 42 -lon -73 --timescale seasonal
+python -m salientsdk forecast_timeseries -lat 42 -lon -73 --timescale seasonal
 # this will get multiple variables in separate files:
-python -m salientsdk.forecast_timeseries_api -lat 42 -lon -73 -var temp,precip --timescale seasonal
+python -m salientsdk forecast_timeseries -lat 42 -lon -73 -var temp,precip --timescale seasonal
 ```
 
 """
 
 import os
 from datetime import datetime
 
 import requests
 import xarray as xr
 
-from . import constants, location, login_api
+from . import login_api
+from .constants import _build_url, get_model_version
+from .location import Location
+from .login_api import get_current_session, get_verify_ssl
 
 
 def forecast_timeseries(
-    loc: location.Location,
+    loc: Location,
     date: str = "-today",
     debias: bool = False,
     field: str = "anom",
     format: str = "nc",
     model: str = "blend",
     reference_clim: str = "30_yr",
     timescale="all",
     variable: str = "temp",
-    version: str = constants.get_model_version(),
+    version: str = get_model_version(),
     force: bool = False,
-    session: requests.Session = constants.get_current_session(),
-    verify: bool = constants.VERFY_SSL,
+    session: requests.Session = get_current_session(),
+    verify: bool = get_verify_ssl(),
     verbose: bool = False,
     **kwargs,
 ) -> str | dict[str, str]:
     """Get time series of S2S meteorological forecasts.
 
     This function is a convenience wrapper to the Salient
     [API](https://api.salientpredictions.com/v2/documentation/api/#/Forecasts/forecast_timeseries).
@@ -62,21 +65,21 @@
             Defaults to `nc` which returns a multivariate NetCDF file.
             Also available: `csv` which returns a CSV file.
         model (str): The model to query.  Defaults to `blend`, which is the Salient blended forecast.
         reference_clim (str):  Reference climatology for calculating anomalies.
             Ignored when `field=vals` since there are no anomalies to calculate.
             Defaults to `30_yr`, which is the 30-year climatology.
         timescale (str): Forecast look-ahead.
-            `sub-seasonal` is 1-5 weeks.  Will return a coordinate `forecast_date_weekly` and
+            - `sub-seasonal` is 1-5 weeks.  Will return a coordinate `forecast_date_weekly` and
                 a data variable `anom_weekly` or `vals_weekly`.
-            `seasonal` is 1-3 months.  Will return a coordinate `forecast_date_monthly` and a
+            - `seasonal` is 1-3 months.  Will return a coordinate `forecast_date_monthly` and a
                 data variable `anom_monthly` or `vals_monthly`.
-            `long-range` is 1-4 quarters.  Will return a coordinate `forecast_date_quarterly` and a
+            - `long-range` is 1-4 quarters.  Will return a coordinate `forecast_date_quarterly` and a
                 data variable `anom_quarterly` or `vals_quarterly`.
-            `all` (default) will include `sub-seasonal`, `seasonal`, and `long-range` timescales
+            - `all` (default) will include `sub-seasonal`, `seasonal`, and `long-range` timescales
         variable (str): The variable to query, defaults to `temp`
             To request multiple variables, separate them with a comma `temp,precip`
             This will download one file per variable
             See the
             [Data Fields](https://salientpredictions.notion.site/Variables-d88463032846402e80c9c0972412fe60)
             documentation for a full list of available historical variables.
         version (str): The model version of the Salient `blend` forecast.
@@ -147,15 +150,15 @@
         reference_clim=reference_clim,
         timescale=timescale,
         variable=variable,
         version=version,
         **kwargs,
     )
 
-    (query, file_name) = constants._build_url(endpoint, args)
+    (query, file_name) = _build_url(endpoint, args)
 
     if force or not os.path.exists(file_name):
         if verbose:
             print(f"Downloading {query} to {file_name}")
         with open(file_name, "wb" if format == "nc" else "w") as f:
             result = session.get(query, verify=verify)
             result.raise_for_status()
@@ -163,46 +166,7 @@
                 f.write(result.content)
             else:
                 f.write(result.text)
     elif verbose:
         print(f"File {file_name} already exists")
 
     return file_name
-
-
-def _main() -> None:
-    argparser = location.Location.get_argparser(["date", "debias", "version", "force"])
-
-    argparser.add_argument("-fld", "--field", type=str, default="anom")
-    argparser.add_argument("-fmt", "--format", type=str, default="nc")
-    argparser.add_argument("-mdl", "--model", type=str, default="blend")
-    argparser.add_argument("-ref", "--reference_clim", type=str, default="30_yr")
-    argparser.add_argument("--timescale", type=str, default="all")
-    argparser.add_argument("-var", "--variable", type=str, default="temp")
-
-    args = argparser.parse_args()
-
-    session = login_api._login_from_args(args)
-
-    loc = location.Location._from_args_(args)
-    file_name = forecast_timeseries(
-        loc,
-        variable=args.variable,
-        field=args.field,
-        date=args.date,
-        debias=args.debias,
-        format=args.format,
-        force=args.force,
-        timescale=args.timescale,
-        model=args.model,
-        version=args.version,
-        reference_clim=args.reference_clim,
-        verbose=args.verbose,
-        session=session,
-    )
-
-    if args.verbose and isinstance(file_name, str):
-        print(xr.open_dataset(file_name))
-
-
-if __name__ == "__main__":
-    _main()
```

### Comparing `salientsdk-0.1.3/salientsdk/upload_file_api.py` & `salientsdk-0.1.4/salientsdk/upload_file_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 
 import json
 import os
 
 import pandas as pd
 import requests
 
-from . import constants, login_api
+from .constants import _build_url
+from .login_api import get_current_session, login
 
 
 def upload_file(
-    file: str, verbose: bool = True, session: requests.Session = constants.get_current_session()
+    file: str, verbose: bool = True, session: requests.Session = get_current_session()
 ) -> None:
     """Uploads a geography file to the Salient API.
 
     An interface to to the Salient
     [upload_file](https://api.salientpredictions.com/v2/documentation/api/#/General/upload_file)
     API endpoint.
 
@@ -33,15 +34,15 @@
         verbose (bool): whether to print status messages.
         session (requests.Session): the session to use for the upload.
 
     """
     if verbose:
         print(f"Uploading {file}")
 
-    (url, loc_file) = constants._build_url("upload_file")
+    (url, loc_file) = _build_url("upload_file")
 
     # do we need to open .zipped shapefiles in 'rb' binary mode?
     req = session.post(url, files={"file": open(file, "r")})
     req.raise_for_status()
     if verbose:
         print(req.text)
 
@@ -52,15 +53,15 @@
     north: float,
     south: float,
     east: float,
     west: float,
     geoname: str,
     force: bool = False,
     verbose: bool = True,
-    session: requests.Session = constants.get_current_session(),
+    session: requests.Session = get_current_session(),
 ) -> str:
     """Upload a bounding box.
 
     Create and upload a GeoJSON shapefile with a rectangular bounding box
     for later use with the `shapefile` location argument.
 
     Args:
@@ -107,15 +108,15 @@
 def upload_location_file(
     lats: list[float],
     lons: list[float],
     names: list[str],
     geoname: str,
     force: bool = False,
     verbose: bool = False,
-    session: requests.Session = constants.get_current_session(),
+    session: requests.Session = get_current_session(),
     **kwargs,
 ) -> str:
     """Upload a vector of locations.
 
     Create and upload a CSV file with a list of locations for
     later use with the `location_file` location argument.
 
@@ -143,15 +144,15 @@
 
     upload_file(geofile, verbose, session)
 
     return geofile
 
 
 if __name__ == "__main__":
-    session = login_api.login()
+    session = login()
 
     geofile = upload_bounding_box(
         west=-109.1, east=-102.0, south=37.8, north=41.0, geoname="Colorado", session=session
     )
 
     # read the JSON geofile
     with open(geofile, "r") as f:
```

### Comparing `salientsdk-0.1.3/PKG-INFO` & `salientsdk-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salientsdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Salient Predictions Software Development Kit
 Home-page: https://salientpredictions.com
 License: docs/LICENSE.md
 Keywords: weather,climate,forecasting,sdk,salient,s2s
 Author: Salient Predictions
 Author-email: help@salientpredictions.com
 Requires-Python: >=3.11,<4.0
@@ -13,33 +13,33 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: h5netcdf (>=1.3.0,<2.0.0)
 Requires-Dist: netCDF4 (>=1.6.5,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: xarray[h5netcdf] (>=2024.2.0,<2025.0.0)
+Requires-Dist: xarray (>=2024.2.0,<2025.0.0)
 Project-URL: Documentation, https://sdk.salientpredictions.com
 Project-URL: Repository, https://github.com/Salient-Predictions/salientsdk
 Description-Content-Type: text/markdown
 
 
 # Intended Use
 
-The Salient SDK is a convenience wrapper around Salient Predictions' customer-facing  
+The Salient SDK is a python convenience wrapper around Salient Predictions' customer-facing  
 [web API](https://api.salientpredictions.com/v2/documentation/api/).  It also contains utility functions for manipulating and analyzing the data delivered from the API.
 
 # Setting up the SDK
 
 ## Prerequisites 
 
 The Salient SDK requires Python 3.11 to use.   If you have Python installed, you can check your version with:
 
 ```bash
-python --version
+python3 --version
 ```
 
 To get version 3.11:
 
 ```bash
 # Ubuntu:
 sudo apt update
@@ -57,49 +57,59 @@
 ```
 
 ## Installing the SDK
 
 The easiest way to get the Salient SDK is to install it like any other package:
 
 ```bash
-pip install salientsdk
+pip install salientsdk --upgrade
+# to verify version with
+pip show salientsdk
 ```
 
+# Usage
 
+## Command Line
 
+The Salient SDK contains a full command line interface that can access each of the primary
+API functions without even opening python.  You can get help for all options or specific commands:
 
-
-
-
-# Usage
+```bash
+python3 -m salientsdk --help
+python3 -m salientsdk forecast_timeseries --help
+```
 
 To access the Salient API you will need a `username` and `password` provided by
 your Salient representative.  The universal credentials `testusr` and `testpwd` 
 have limited permissions for testing and validation purposes:
 
 ```bash
-python -m salientsdk.data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31 -u testusr -p testpwd
+python3 -m salientsdk data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31 -u testusr -p testpwd
 ```
 
-In a python script:
+## Via Python
+
+In a python 3.11 script, this example code will login and request a historical ERA5 data timeseries.
 
 ```python
 import salientsdk as sk
 import xarray as xr
 import netcdf4
 
 session = sk.login("testusr","testpwd")
-history = sk.data_timeseries(loc = Location(lat=42, lon=-73), field="all", variable="temp")
+history = sk.data_timeseries(loc = Location(lat=42, lon=-73), field="all", variable="temp", session=session)
 print(xr.open_file(history))
 ```
 
+Note that this example uses the limited credentials `testusr` and `testpwd`.  To access the full capabilities of your license, use your Salient-provided credentials.
+
 See all available functions in the [API Reference](api.md).
 
 The [examples](https://github.com/Salient-Predictions/salientsdk/tree/main/examples) directory contains `ipynb` notebooks to help you get started with common operations. 
 
 # License
 
-This SDK is licensed for use by Salient customers [details](LICENSE.md).
+This SDK is licensed for use by Salient customers [details](https://salient-predictions.github.io/salientsdk/LICENSE/).
 
 
 Copyright 2024 [Salient Predictions](https://www.salientpredictions.com/)
```

