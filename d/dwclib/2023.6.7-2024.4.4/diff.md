# Comparing `tmp/dwclib-2023.6.7.tar.gz` & `tmp/dwclib-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwclib-2023.6.7.tar", max compression
+gzip compressed data, was "dwclib-2024.4.4.tar", max compression
```

## Comparing `dwclib-2023.6.7.tar` & `dwclib-2024.4.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      753 2022-06-09 12:54:18.472933 dwclib-2023.6.7/LICENSE
--rw-r--r--   0        0        0     1263 2022-09-14 11:01:06.119049 dwclib-2023.6.7/README.md
--rw-r--r--   0        0        0      823 2023-06-07 10:28:17.376535 dwclib-2023.6.7/pyproject.toml
--rw-r--r--   0        0        0      433 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/__init__.py
--rw-r--r--   0        0        0       59 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/alerts/__init__.py
--rw-r--r--   0        0        0     2672 2023-03-03 15:13:00.467651 dwclib-2023.6.7/src/dwclib/alerts/alerts.py
--rw-r--r--   0        0        0        0 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/assets/__init__.py
--rw-r--r--   0        0        0   173360 2023-03-03 14:48:35.668082 dwclib-2023.6.7/src/dwclib/assets/alert_ref.csv
--rw-r--r--   0        0        0     1451 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/db.py
--rw-r--r--   0        0        0     1178 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/meta.py
--rw-r--r--   0        0        0     2398 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/numerics.py
--rw-r--r--   0        0        0     1397 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/wave_unfold.py
--rw-r--r--   0        0        0     2178 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/common/waves.py
--rw-r--r--   0        0        0      153 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/__init__.py
--rw-r--r--   0        0        0      917 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/generic.py
--rw-r--r--   0        0        0      820 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/numerics.py
--rw-r--r--   0        0        0      817 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/waves.py
--rw-r--r--   0        0        0     1419 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/waves_convert.py
--rw-r--r--   0        0        0       65 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/numerics/__init__.py
--rw-r--r--   0        0        0     1551 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/numerics/numerics.py
--rw-r--r--   0        0        0       95 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/patients/__init__.py
--rw-r--r--   0        0        0     4141 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/patients/patients.py
--rw-r--r--   0        0        0       56 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/waves/__init__.py
--rw-r--r--   0        0        0     1334 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/waves/waves.py
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 dwclib-2023.6.7/PKG-INFO
+-rw-r--r--   0        0        0      753 2022-06-09 12:54:18.472933 dwclib-2024.4.4/LICENSE
+-rw-r--r--   0        0        0     1679 2024-04-04 20:35:20.780494 dwclib-2024.4.4/README.md
+-rw-r--r--   0        0        0      737 2024-04-04 20:31:28.610432 dwclib-2024.4.4/pyproject.toml
+-rw-r--r--   0        0        0      508 2023-10-15 18:21:30.585978 dwclib-2024.4.4/src/dwclib/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/alerts/__init__.py
+-rw-r--r--   0        0        0     2636 2024-04-04 20:36:22.769018 dwclib-2024.4.4/src/dwclib/alerts/alerts.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/assets/__init__.py
+-rw-r--r--   0        0        0   173360 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/assets/alert_ref.csv
+-rw-r--r--   0        0        0     1346 2023-06-20 11:00:59.901656 dwclib-2024.4.4/src/dwclib/common/db.py
+-rw-r--r--   0        0        0     1315 2023-10-15 18:14:41.791832 dwclib-2024.4.4/src/dwclib/common/meta.py
+-rw-r--r--   0        0        0     2197 2024-04-04 20:21:52.604945 dwclib-2024.4.4/src/dwclib/common/numerics.py
+-rw-r--r--   0        0        0     1298 2023-06-20 14:18:49.043435 dwclib-2024.4.4/src/dwclib/common/wave_unfold.py
+-rw-r--r--   0        0        0     2060 2024-04-04 20:22:17.465118 dwclib-2024.4.4/src/dwclib/common/waves.py
+-rw-r--r--   0        0        0      153 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/dask/__init__.py
+-rw-r--r--   0        0        0      981 2024-01-13 15:37:07.253914 dwclib-2024.4.4/src/dwclib/dask/generic.py
+-rw-r--r--   0        0        0      791 2023-06-20 14:21:34.423133 dwclib-2024.4.4/src/dwclib/dask/numerics.py
+-rw-r--r--   0        0        0      788 2023-06-20 14:21:42.655119 dwclib-2024.4.4/src/dwclib/dask/waves.py
+-rw-r--r--   0        0        0     1419 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/dask/waves_convert.py
+-rw-r--r--   0        0        0       77 2023-10-15 18:21:07.681856 dwclib-2024.4.4/src/dwclib/enumerations/__init__.py
+-rw-r--r--   0        0        0     3214 2024-04-04 20:28:55.460956 dwclib-2024.4.4/src/dwclib/enumerations/enumerations.py
+-rw-r--r--   0        0        0       65 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/numerics/__init__.py
+-rw-r--r--   0        0        0     1530 2023-10-15 18:28:14.976170 dwclib-2024.4.4/src/dwclib/numerics/numerics.py
+-rw-r--r--   0        0        0       95 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/patients/__init__.py
+-rw-r--r--   0        0        0     5350 2024-04-04 20:25:50.818998 dwclib-2024.4.4/src/dwclib/patients/patients.py
+-rw-r--r--   0        0        0       56 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/waves/__init__.py
+-rw-r--r--   0        0        0     1365 2023-08-18 09:13:01.184641 dwclib-2024.4.4/src/dwclib/waves/waves.py
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 dwclib-2024.4.4/PKG-INFO
```

### Comparing `dwclib-2023.6.7/LICENSE` & `dwclib-2024.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.7/README.md` & `dwclib-2024.4.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,27 @@
 Installation through conda greatly simplifies dependency management.
 
 Additionally, Microsoft SQL Server drivers are needed and will need to be installed seperately.
 See here for more information: https://github.com/mkleehammer/pyodbc/wiki
 
 
 ## Changelog
+- 2024.4.4
+    - Support querying enumerations
+    - Update dependencies
+
+- 2023.6.21
+    - Remove all occurences of naive datetime since dask now support tz-aware
+    - New config file syntax to be compatible with other libraries
+    - Fix a bug when Pleth waveform return all NaN
+
+- 2023.6.7
+    - Support for querying alerts using the read_alerts call
+    - Use the platformdirs package for config file location
+
 - 2022.9.14
     - Support numeric labels and sublabels in read_patients and read_numerics
     - Support to query for multiple patients at once in read_numerics
 
 - 2022.6.23
     - Convert packaging from flit to poetry
     - Add linting and testing with nox, flake8 and safety
```

### Comparing `dwclib-2023.6.7/src/dwclib/assets/alert_ref.csv` & `dwclib-2024.4.4/src/dwclib/assets/alert_ref.csv`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.7/src/dwclib/common/db.py` & `dwclib-2024.4.4/src/dwclib/common/db.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,42 +10,41 @@
     pyodbc.pooling = False
     odbcdriver = pyodbc.drivers()[0]
 except (ImportError, IndexError):
     odbcdriver = None
 
 from sqlalchemy.engine import URL
 
-config_dir = Path(user_config_dir(appname="dwclib", appauthor="larib-data"))
-config_dir.mkdir(parents=True, exist_ok=True)
+config_dir = Path(user_config_dir(appname="larib-data", appauthor="larib-data"))
 configfile = config_dir / "config.ini"
 
 
 if configfile.exists():
     config = ConfigParser()
     config.read(configfile)
-    dwcdriver = config.get('dwclib', 'dwc_driver', fallback=odbcdriver)
+    dwcdriver = config.get('dwc', 'driver', fallback=odbcdriver)
     if dwcdriver is None:
         warn('No ODBC driver found for DWC', RuntimeWarning)
 
     dwcuri = URL.create(
         'mssql+pyodbc',
-        username=config.get('dwclib', 'dwc_user'),
-        password=config.get('dwclib', 'dwc_pass'),
-        host=config.get('dwclib', 'dwc_host'),
-        database=config.get('dwclib', 'dwc_dbname'),
+        username=config.get('dwc', 'user'),
+        password=config.get('dwc', 'pass'),
+        host=config.get('dwc', 'host'),
+        database=config.get('dwc', 'dbname'),
         query={
             "driver": dwcdriver,
             "Encrypt": "no",
         },
     )
 
     pguri = URL.create(
         'postgresql',
-        username=config.get('dwclib', 'dwcmeta_user'),
-        password=config.get('dwclib', 'dwcmeta_pass'),
-        host=config.get('dwclib', 'dwcmeta_host'),
-        database=config.get('dwclib', 'dwcmeta_dbname'),
+        username=config.get('dwcmeta', 'user'),
+        password=config.get('dwcmeta', 'pass'),
+        host=config.get('dwcmeta', 'host'),
+        database=config.get('dwcmeta', 'dbname'),
     )
 else:
     warn(f"Configuration file {configfile} does not exist.", RuntimeWarning)
     dwcuri = None
     pguri = None
```

### Comparing `dwclib-2023.6.7/src/dwclib/common/meta.py` & `dwclib-2024.4.4/src/dwclib/common/meta.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import pandas as pd
 from dask.dataframe.utils import make_meta
 
 
-def build_numerics_meta(naive_datetime=True):
-    tz = None if naive_datetime else 'UTC'
-    idx = pd.DatetimeIndex([], name='TimeStamp', tz=tz)
+def build_numerics_meta():
+    idx = pd.DatetimeIndex([], name='TimeStamp', tz='UTC')
     dtypes = {
         'PatientId': 'string',
         'Label': 'string',
         'SubLabel': 'string',
         'Value': 'float32',
     }
     mdf = pd.DataFrame({k: [] for k in dtypes.keys()}, index=idx)
     mdf = mdf.astype(dtype=dtypes)
     return make_meta(mdf)
 
 
-def build_waves_meta(naive_datetime=True):
-    tz = None if naive_datetime else 'UTC'
-    idx = pd.DatetimeIndex([], name='TimeStamp', tz=tz)
+def build_waves_meta():
+    idx = pd.DatetimeIndex([], name='TimeStamp', tz='UTC')
     dtypes = {
         'PatientId': 'string',
         'Label': 'string',
         'WaveSamples': 'object',
         'SamplePeriod': 'int32',
         'CAU': 'float64',
         'CAL': 'float64',
@@ -30,11 +28,22 @@
         'CSL': 'int32',
     }
     mdf = pd.DataFrame({k: [] for k in dtypes.keys()}, index=idx)
     mdf = mdf.astype(dtype=dtypes)
     return make_meta(mdf)
 
 
+def build_enumerations_meta():
+    idx = pd.DatetimeIndex([], name='TimeStamp', tz='UTC')
+    dtypes = {
+        'PatientId': 'string',
+        'Label': 'string',
+        'Value': 'string',
+    }
+    mdf = pd.DataFrame({k: [] for k in dtypes.keys()}, index=idx)
+    mdf = mdf.astype(dtype=dtypes)
+    return make_meta(mdf)
+
+
 numerics_meta = build_numerics_meta()
-numerics_meta_tz = build_numerics_meta(naive_datetime=False)
 waves_meta = build_waves_meta()
-waves_meta_tz = build_waves_meta(naive_datetime=False)
+enumerations_meta = build_enumerations_meta()
```

### Comparing `dwclib-2023.6.7/src/dwclib/common/numerics.py` & `dwclib-2024.4.4/src/dwclib/common/numerics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from datetime import datetime
 from typing import List, Union
 
 import pandas as pd
-from dwclib.common.meta import numerics_meta, numerics_meta_tz
 from pandas.api.types import is_list_like
 from sqlalchemy import MetaData, Table, create_engine, join, select
 
+from dwclib.common.meta import numerics_meta
+
 
 def run_numerics_query(
     uri: str,
     dtbegin: Union[str, datetime],
     dtend: Union[str, datetime],
     patientids: Union[None, str, List[str]],
     labels: List[str],
     sublabels: List[str],
-    naive_datetime: bool = False,
 ) -> pd.DataFrame:
     engine = create_engine(uri)
     q = build_numerics_query(engine, dtbegin, dtend, patientids, labels, sublabels)
 
     with engine.connect() as conn:
         df = pd.read_sql(q, conn, index_col='TimeStamp')
     engine.dispose()
     if len(df) == 0:
-        return numerics_meta if naive_datetime else numerics_meta_tz
+        return numerics_meta
     else:
-        dtidx = pd.to_datetime(df.index, utc=True)
-        df.index = dtidx.to_numpy(dtype='datetime64[ns]') if naive_datetime else dtidx
+        df.index = pd.to_datetime(df.index, utc=True)
         return df.astype(numerics_meta.dtypes.to_dict(), copy=False)
 
 
 def build_numerics_query(engine, dtbegin, dtend, patientids, labels, sublabels):
-    dbmeta = MetaData(bind=engine)
-    nnt = Table(
-        'Numeric_', dbmeta, schema='_Export', autoload=True, autoload_with=engine
-    )
-    nvt = Table(
-        'NumericValue_', dbmeta, schema='_Export', autoload=True, autoload_with=engine
-    )
+    dbmeta = MetaData(schema='_Export')
+    dbmeta.reflect(bind=engine)
+    nnt = Table('Numeric_', dbmeta, autoload=True, autoload_with=engine)
+    nvt = Table('NumericValue_', dbmeta, autoload=True, autoload_with=engine)
 
     nn = select(nnt.c.TimeStamp, nnt.c.Id, nnt.c.Label, nnt.c.SubLabel)
     nn = nn.with_hint(nnt, 'WITH (NOLOCK)')
     nn = nn.where(nnt.c.TimeStamp >= dtbegin)
     nn = nn.where(nnt.c.TimeStamp < dtend)
     if labels:
         nn = nn.where(nnt.c.Label.in_(labels))
@@ -49,15 +45,15 @@
         nn = nn.where(nnt.c.SubLabel.in_(sublabels))
     nn = nn.cte('Numeric')
 
     nv = select(nvt.c.TimeStamp, nvt.c.NumericId, nvt.c.Value, nvt.c.PatientId)
     nv = nv.with_hint(nvt, 'WITH (NOLOCK)')
     nv = nv.where(nvt.c.TimeStamp >= dtbegin)
     nv = nv.where(nvt.c.TimeStamp < dtend)
-    nv = nv.where(nvt.c.Value is not None)
+    nv = nv.where(nvt.c.Value.is_not(None))
     if patientids:
         if is_list_like(patientids):
             nv = nv.where(nvt.c.PatientId.in_(patientids))
         else:
             nv = nv.where(nvt.c.PatientId == patientids)
     nv = nv.cte('NumericValue')
```

### Comparing `dwclib-2023.6.7/src/dwclib/common/wave_unfold.py` & `dwclib-2024.4.4/src/dwclib/common/wave_unfold.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import pandas as pd
-from numba import njit
 
 
-def unfold_row(row: pd.Series, naive_datetime=True) -> pd.Series:
+def unfold_row(row: pd.Series) -> pd.Series:
     # XXX unify following line once we use the same unfold_row function for pandas and dask
     begintime = row.name[0] if isinstance(row.name, tuple) else row.name
     basetime = 1000 * begintime.timestamp()
     msperiod = row['SamplePeriod']
     bytesamples = row['WaveSamples']
     calibs = [row[x] for x in ['CAU', 'CAL', 'CSU', 'CSL']]
     noscale = any([x is None for x in calibs])
@@ -15,26 +14,23 @@
         realvals = wave_unfold(bytesamples, 0, 0, 0, 0)
     else:
         realvals = wave_unfold(bytesamples, *calibs)
     # Generate millisecond index
     timestamps = basetime + msperiod * np.arange(len(realvals))
     # Convert to datetime[64]
     timestamps = pd.to_datetime(timestamps, unit='ms', utc=True)
-    if naive_datetime:
-        timestamps = timestamps.to_numpy(dtype='datetime64[ns]')
     return pd.Series(realvals, index=timestamps)
 
 
-@njit
 def wave_unfold(indata: bytes, cau: float, cal: float, csu: int, csl: int):
     if len(indata) % 2:
         indata = indata[:-1]
     int16le = np.dtype('<i2')
     npindata = np.frombuffer(indata, dtype=int16le)
-    if (csu - csl) != 0:
-        m = (cau - cal) / (csu - csl)
-        b = cau - m * csu
-    else:
+    if any(np.isnan([cau, cal, csu, csl])) or (csu - csl) == 0:
         m = 1
         b = 0
+    else:
+        m = (cau - cal) / (csu - csl)
+        b = cau - m * csu
     outdata = m * npindata.astype(np.float32) + b
     return outdata
```

### Comparing `dwclib-2023.6.7/src/dwclib/common/waves.py` & `dwclib-2024.4.4/src/dwclib/common/waves.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import pandas as pd
 from dwclib.common.meta import waves_meta
 from sqlalchemy import MetaData, Table, create_engine, join, select
 
 
-def run_waves_query(uri, dtbegin, dtend, patientid, labels, naive_datetime=False):
+def run_waves_query(uri, dtbegin, dtend, patientid, labels):
     engine = create_engine(uri)
     q = build_waves_query(engine, dtbegin, dtend, patientid, labels)
 
     with engine.connect() as conn:
         df = pd.read_sql(q, conn, index_col='TimeStamp')
     engine.dispose()
     if len(df) == 0:
         return waves_meta
     else:
-        dtidx = pd.to_datetime(df.index, utc=True)
-        df.index = dtidx.to_numpy(dtype='datetime64[ns]') if naive_datetime else dtidx
+        df.index = pd.to_datetime(df.index, utc=True)
         return df.astype(waves_meta.dtypes.to_dict(), copy=False)
 
 
 def build_waves_query(engine, dtbegin, dtend, patientid, labels):
-    dbmeta = MetaData(bind=engine)
-    wwt = Table('Wave_', dbmeta, schema='_Export', autoload=True, autoload_with=engine)
-    wst = Table(
-        'WaveSample_', dbmeta, schema='_Export', autoload=True, autoload_with=engine
-    )
+    dbmeta = MetaData(schema='_Export')
+    dbmeta.reflect(bind=engine)
+    wwt = Table('Wave_', dbmeta, autoload=True, autoload_with=engine)
+    wst = Table('WaveSample_', dbmeta, autoload=True, autoload_with=engine)
 
     ww = select(
         wwt.c.TimeStamp,
         wwt.c.Id,
         wwt.c.Label,
         wwt.c.SamplePeriod,
         wwt.c.CalibrationAbsUpper.label('CAU'),
@@ -42,15 +40,15 @@
         ww = ww.where(wwt.c.Label.in_(labels))
     ww = ww.cte('Wave')
 
     ws = select(wst.c.TimeStamp, wst.c.WaveId, wst.c.WaveSamples, wst.c.PatientId)
     ws = ws.with_hint(wst, 'WITH (NOLOCK)')
     ws = ws.where(wst.c.TimeStamp >= dtbegin)
     ws = ws.where(wst.c.TimeStamp < dtend)
-    ws = ws.where(wst.c.WaveSamples is not None)
+    ws = ws.where(wst.c.WaveSamples.is_not(None))
     if patientid:
         ws = ws.where(wst.c.PatientId == patientid)
     ws = ws.cte('WaveSample')
 
     j = join(ws, ww, ws.c.WaveId == ww.c.Id)
     q = select(
         ws.c.TimeStamp,
```

### Comparing `dwclib-2023.6.7/src/dwclib/dask/generic.py` & `dwclib-2024.4.4/src/dwclib/dask/generic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from datetime import timedelta
 from itertools import count
 
-from dwclib.common.db import dwcuri
-
+import dask
 import dask.dataframe as dd
 from dask import delayed
+from dwclib.common.db import dwcuri
 
 one_hour = timedelta(hours=1)
+dask.config.set({"dataframe.convert-string": False})
 
 
 def build_divisions(dtbegin, dtend, interval):
     ranges = []
     for i in count():
         beg = dtbegin + i * interval
         end = beg + interval
```

### Comparing `dwclib-2023.6.7/src/dwclib/dask/numerics.py` & `dwclib-2024.4.4/src/dwclib/dask/numerics.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,8 @@
         dtbegin=dtbegin,
         dtend=dtend,
         uri=uri,
         interval=interval,
         patientids=patientids,
         labels=labels,
         sublabels=sublabels,
-        naive_datetime=True,
     )
```

### Comparing `dwclib-2023.6.7/src/dwclib/dask/waves.py` & `dwclib-2024.4.4/src/dwclib/dask/waves.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,9 @@
         meta=waves_meta,
         dtbegin=dtbegin,
         dtend=dtend,
         uri=uri,
         interval=interval,
         patientid=patientid,
         labels=labels,
-        naive_datetime=True,
     )
     return convert_dataframe(ddf, labels, npartitions)
```

### Comparing `dwclib-2023.6.7/src/dwclib/dask/waves_convert.py` & `dwclib-2024.4.4/src/dwclib/dask/waves_convert.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.7/src/dwclib/numerics/numerics.py` & `dwclib-2024.4.4/src/dwclib/numerics/numerics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from typing import List, Optional, Union
 
-import numpy as np
 import pandas as pd
+from pandas.api.types import is_list_like
+
 from dwclib.common.db import dwcuri
-from dwclib.common.meta import numerics_meta_tz
+from dwclib.common.meta import numerics_meta
 from dwclib.common.numerics import run_numerics_query
-from pandas.api.types import is_list_like
 
 
 def read_numerics(
     patientids: Union[None, str, List[str]],
     dtbegin: Union[str, datetime],
     dtend: Union[str, datetime],
     labels: Optional[List[str]] = None,
@@ -23,28 +23,28 @@
     if labels is None:
         labels = []
     if sublabels is None:
         sublabels = []
     if is_list_like(patientids) and len(patientids) == 1:
         patientids = patientids[0]
     df = run_numerics_query(uri, dtbegin, dtend, patientids, labels, sublabels)
+    df = df.dropna(axis=0, how='any', subset=['Value'])
+    if not len(df.index):
+        return numerics_meta
     if pivot:
         df = pivot_numerics(df)
     single_patient = patientids is not None and not is_list_like(patientids)
     if single_patient:
         df.columns = df.columns.droplevel(0)
     # Other way to check if there is a single patientid:
     # if len(df.columns.get_level_values(0).drop_duplicates()) == 1:
     return df
 
 
 def pivot_numerics(df: pd.DataFrame) -> Optional[pd.DataFrame]:
-    df = df.dropna(axis=0, how='any', subset=['Value'])
-    if not len(df.index):
-        numerics_meta_tz
     df = df.pivot_table(
         index=df.index,
         columns=['PatientId', 'SubLabel'],
         values='Value',
-        aggfunc=np.nanmax,
+        aggfunc='max',
     )
     return df
```

### Comparing `dwclib-2023.6.7/src/dwclib/patients/patients.py` & `dwclib-2024.4.4/src/dwclib/patients/patients.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,46 @@
 from typing import List, Optional
 
 import pandas as pd
-from dwclib.common.db import pguri
 from sqlalchemy import MetaData, Table, asc, create_engine, func, or_, select
 
 
+from dwclib.common.db import pguri
+
+
 def read_patient(*args, **kwargs) -> Optional[pd.Series]:
+    """Reads a single patient from DWCmeta database.
+
+    Retrieves a pandas series consisting of the patient which matches the search criteria.
+
+    Args:
+        patientid: A DWC patient identifier
+        name: A patient name
+        firstname: A patient first name
+        ipp: A patient lifetime identifier
+        dtbegin: The beginning of available data samples
+        dtend: The end of available data samples
+        clinicalunit: The clinical unit the patient belongs to
+        bedlabel: The bed / room in which the patient stays
+        wavelabels: A list of waveform labels
+        numericlabels: A list of numerics labels
+        uri: Optional sqlalchemy URI for the database if not provided in the config file
+
+    Returns:
+        A pandas series corresponding to a patient stay.
+    """  # noqa: DAR101,DAR102
     res = read_patients(*args, **kwargs, limit=1)
     if len(res):
         return res.iloc[0]
 
 
 def read_patients(
     patientid: str = None,
     name: str = None,
+    firstname: str = None,
     ipp: str = None,
     dtbegin: str = None,
     dtend: str = None,
     clinicalunit: str = None,
     bedlabel: str = None,
     wavelabels: Optional[List[str]] = None,
     numericlabels: Optional[List[str]] = None,
@@ -28,21 +51,23 @@
     """Reads patients from DWCmeta database.
 
     Retrieves a pandas dataframe consisting of individual patients which match the search criteria.
 
     Args:
         patientid: A DWC patient identifier
         name: A patient name
+        firstname: A patient first name
         ipp: A patient lifetime identifier
         dtbegin: The beginning of available data samples
         dtend: The end of available data samples
         clinicalunit: The clinical unit the patient belongs to
         bedlabel: The bed / room in which the patient stays
         wavelabels: A list of waveform labels
         numericlabels: A list of numerics labels
+        numericsublabels: A list of numerics sublabels
         uri: Optional sqlalchemy URI for the database if not provided in the config file
         limit: Maximum number of returned results
 
     Returns:
         A pandas dataframe with each row corresponding to an individual patient stay, indexed by unique DWC patient identifiers.
     """
     if not uri:
@@ -53,76 +78,84 @@
         numericlabels = []
     if numericsublabels is None:
         numericsublabels = []
     q = build_query(
         uri,
         patientid,
         name,
+        firstname,
         ipp,
         dtbegin,
         dtend,
         clinicalunit,
         bedlabel,
         wavelabels,
         numericlabels,
         numericsublabels,
     )
     if limit:
         q = q.limit(limit)
     engine = create_engine(uri)
     with engine.connect() as conn:
         df = pd.read_sql(q, conn, index_col='patientid')
-    df['data_begin'] = df['data_begin'].to_numpy(dtype='datetime64[ns]')
-    df['data_end'] = df['data_end'].to_numpy(dtype='datetime64[ns]')
     return df
 
 
 def build_query(
     uri,
     patientid,
     name,
+    firstname,
     ipp,
     dtbegin,
     dtend,
     clinicalunit,
     bedlabel,
     wavelabels,
     numericlabels,
     numericsublabels,
 ):
     pgdb = create_engine(uri)
-    pgmeta = MetaData(bind=pgdb)
-
+    pgmeta = MetaData()
+    pgmeta.reflect(bind=pgdb)
     t_patients = Table('patients', pgmeta, autoload_with=pgdb)
     p = t_patients.c
     t_patientlabels = Table('patientlabels', pgmeta, autoload_with=pgdb)
     pl = t_patientlabels.c
 
-    if name:
+    if name or firstname:
         # Build a subquery to allow approximate name search
-        subq = select(
-            [
-                t_patients,
+        fields = [t_patients]
+        if name:
+            fields.append(
                 func.levenshtein(func.lower(p.lastname), func.lower(name)).label(
-                    'distance'
-                ),
-            ]
-        ).cte('subq')
-        t_patients = subq
+                    'd_name'
+                )
+            )
+        if firstname:
+            fields.append(
+                func.levenshtein(func.lower(p.firstname), func.lower(firstname)).label(
+                    'd_firstname'
+                )
+            )
+        t_patients = select(*fields).cte()  # Replace Patients table with CTE
         p = t_patients.c
 
-    q = select([t_patients, pl.numericlabels, pl.numericsublabels, pl.wavelabels])
+    q = select(t_patients, pl.numericlabels, pl.numericsublabels, pl.wavelabels)
     q = q.select_from(
         t_patients.join(t_patientlabels, pl.patientid == p.patientid, isouter=True)
     )
     if patientid:
         q = q.where(p.patientid == patientid)
     if name:
-        q = q.where(p.distance < 3)
-        q = q.order_by(asc(p.distance))
+        q = q.where(p.d_name < 3)
+        q = q.order_by(asc(p.d_name))
+    if firstname:
+        q = q.where(p.d_firstname < 3)
+        q = q.order_by(asc(p.d_firstname))
     if ipp:
         q = q.where(p.lifetimeid == ipp)
     if bedlabel:
         q = q.where(p.bedlabel == bedlabel)
     if clinicalunit:
         q = q.where(p.clinicalunit == clinicalunit)
     if dtbegin:
```

### Comparing `dwclib-2023.6.7/src/dwclib/waves/waves.py` & `dwclib-2024.4.4/src/dwclib/waves/waves.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from collections import defaultdict
 from datetime import datetime
 from multiprocessing.pool import ThreadPool
 from typing import List, Optional, Union
 
 import pandas as pd
+
 from dwclib.common.db import dwcuri
-from dwclib.common.meta import waves_meta_tz
+from dwclib.common.meta import waves_meta
 from dwclib.common.wave_unfold import unfold_row
 from dwclib.common.waves import run_waves_query
 
 
 def read_waves(
     patientid: str,
     dtbegin: Union[str, datetime],
@@ -22,20 +23,21 @@
     if labels is None:
         labels = []
     df = run_waves_query(uri, dtbegin, dtend, patientid, labels)
     return unfold_pandas_dataframe(df)
 
 
 def unfold_pandas_dataframe(df: pd.DataFrame) -> pd.DataFrame:
+    # TODO: see if we can efficiently pre-allocate buffer
     databuffer = defaultdict(list)
     for _, row in df.iterrows():
-        srow = unfold_row(row, naive_datetime=False)
+        srow = unfold_row(row)
         databuffer[row['Label']].append(srow)
     if not databuffer:
-        return waves_meta_tz
+        return waves_meta
     concatter = dictconcatter(databuffer)
     with ThreadPool() as pool:
         pool.map(concatter, databuffer.keys())
     return pd.DataFrame(databuffer)
 
 
 def dictconcatter(d) -> pd.DataFrame:
```

### Comparing `dwclib-2023.6.7/PKG-INFO` & `dwclib-2024.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: dwclib
-Version: 2023.6.7
+Version: 2024.4.4
 Summary: Python wrapper to DataWarehouse Connect
 Home-page: https://github.com/larib-data/dwclib
 License: ISC
 Author: Jona Joachim
 Author-email: jona@joachim.cc
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: SQLAlchemy (>=1.4,<1.5)
-Requires-Dist: dask (>=2022)
-Requires-Dist: numba (>=0.57,<0.58)
+Requires-Dist: SQLAlchemy (>=2,<3)
+Requires-Dist: dask[dataframe] (>=2024.4.1,<2025.0.0)
 Requires-Dist: numpy (>=1,<2)
-Requires-Dist: pandas (>=1.4,<3)
-Requires-Dist: platformdirs (>=3.0.0,<4.0.0)
+Requires-Dist: pandas (>=2,<3)
+Requires-Dist: platformdirs (>=3,<4)
+Requires-Dist: pyarrow (>=14)
 Project-URL: Repository, https://github.com/larib-data/dwclib
 Description-Content-Type: text/markdown
 
 # Overview
 Python wrapper to DataWarehouse Connect.
 -   Free software: ISC license
 
@@ -34,14 +33,27 @@
 Installation through conda greatly simplifies dependency management.
 
 Additionally, Microsoft SQL Server drivers are needed and will need to be installed seperately.
 See here for more information: https://github.com/mkleehammer/pyodbc/wiki
 
 
 ## Changelog
+- 2024.4.4
+    - Support querying enumerations
+    - Update dependencies
+
+- 2023.6.21
+    - Remove all occurences of naive datetime since dask now support tz-aware
+    - New config file syntax to be compatible with other libraries
+    - Fix a bug when Pleth waveform return all NaN
+
+- 2023.6.7
+    - Support for querying alerts using the read_alerts call
+    - Use the platformdirs package for config file location
+
 - 2022.9.14
     - Support numeric labels and sublabels in read_patients and read_numerics
     - Support to query for multiple patients at once in read_numerics
 
 - 2022.6.23
     - Convert packaging from flit to poetry
     - Add linting and testing with nox, flake8 and safety
```

