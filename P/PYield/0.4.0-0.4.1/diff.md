# Comparing `tmp/pyield-0.4.0.tar.gz` & `tmp/pyield-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.4.0.tar", last modified: Wed Apr  3 08:59:58 2024, max compression
+gzip compressed data, was "pyield-0.4.1.tar", last modified: Thu Apr  4 06:37:26 2024, max compression
```

## Comparing `pyield-0.4.0.tar` & `pyield-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.4.0/LICENSE
--rw-r--r--   0        0        0     3908 2024-03-24 20:00:55.060263 pyield-0.4.0/README.md
--rw-r--r--   0        0        0       22 2024-04-03 00:41:38.271044 pyield-0.4.0/pyield/__about__.py
--rw-r--r--   0        0        0      439 2024-04-03 01:25:29.226587 pyield-0.4.0/pyield/__init__.py
--rw-r--r--   0        0        0     7316 2024-04-03 07:53:40.718668 pyield-0.4.0/pyield/anbima.py
--rw-r--r--   0        0        0    11050 2024-04-03 08:44:15.200333 pyield-0.4.0/pyield/br_calendar.py
--rw-r--r--   0        0        0     2214 2024-04-02 10:06:20.736451 pyield-0.4.0/pyield/br_holidays.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.4.0/pyield/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.4.0/pyield/br_holidays_old.txt
--rw-r--r--   0        0        0     5742 2024-04-03 08:39:31.403271 pyield-0.4.0/pyield/di_futures.py
--rw-r--r--   0        0        0     9684 2024-04-02 10:11:24.407591 pyield-0.4.0/pyield/di_web.py
--rw-r--r--   0        0        0     9546 2024-04-02 10:40:33.557619 pyield-0.4.0/pyield/di_xml.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.4.0/pyield/py.typed
--rw-r--r--   0        0        0     1077 2024-04-03 08:59:58.234881 pyield-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1138 2024-02-23 08:17:20.287259 pyield-0.4.0/tests/test_br_calendar.py
--rw-r--r--   0        0        0     2499 2024-04-03 08:58:18.911442 pyield-0.4.0/tests/test_di.py
--rw-r--r--   0        0        0     5925 1970-01-01 00:00:00.000000 pyield-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3908 2024-03-24 20:00:55.060263 pyield-0.4.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-04 06:35:56.778689 pyield-0.4.1/pyield/__about__.py
+-rw-r--r--   0        0        0      439 2024-04-03 01:25:29.226587 pyield-0.4.1/pyield/__init__.py
+-rw-r--r--   0        0        0     7180 2024-04-04 06:34:56.777051 pyield-0.4.1/pyield/anbima.py
+-rw-r--r--   0        0        0    11050 2024-04-03 08:44:15.200333 pyield-0.4.1/pyield/br_calendar.py
+-rw-r--r--   0        0        0     2214 2024-04-02 10:06:20.736451 pyield-0.4.1/pyield/br_holidays.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.4.1/pyield/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.4.1/pyield/br_holidays_old.txt
+-rw-r--r--   0        0        0     5742 2024-04-03 08:39:31.403271 pyield-0.4.1/pyield/di_futures.py
+-rw-r--r--   0        0        0     9684 2024-04-02 10:11:24.407591 pyield-0.4.1/pyield/di_web.py
+-rw-r--r--   0        0        0     9546 2024-04-02 10:40:33.557619 pyield-0.4.1/pyield/di_xml.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.4.1/pyield/py.typed
+-rw-r--r--   0        0        0     1077 2024-04-04 06:37:26.441092 pyield-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1138 2024-02-23 08:17:20.287259 pyield-0.4.1/tests/test_br_calendar.py
+-rw-r--r--   0        0        0     2499 2024-04-03 08:58:18.911442 pyield-0.4.1/tests/test_di.py
+-rw-r--r--   0        0        0     5925 1970-01-01 00:00:00.000000 pyield-0.4.1/PKG-INFO
```

### Comparing `pyield-0.4.0/LICENSE` & `pyield-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/README.md` & `pyield-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/pyield/anbima.py` & `pyield-0.4.1/pyield/anbima.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,49 +32,47 @@
     if not cl.is_business_day(normalized_date):
         raise ValueError("Reference date must be a business day.")
 
     return normalized_date
 
 
 def get_raw_data(
-    reference_date: str | Timestamp | None = None, is_anbima_member: bool = False
+    reference_date: Timestamp, is_anbima_member: bool = False
 ) -> DataFrame:
     """
     Fetch indicative rates from ANBIMA for a specific date.
 
     Parameters:
     - reference_date (pd.Timestamp): Date for which to fetch the indicative rates.
     - is_anbima_member (bool): Whether the request is being made by an ANBIMA member.
 
     Returns:
     - pd.DataFrame: DataFrame with the indicative rates for the given date.
     """
-    # Process the reference date, defaulting to the previous business day if not provided
-    normalized_date = normalize_date(reference_date)
-
     # Format the date to match the URL format
-    url_date = normalized_date.strftime("%y%m%d")
+    url_date = reference_date.strftime("%y%m%d")
 
     # Set the base URL according to the member status
     base_url = ANBIMA_MEMBER_URL if is_anbima_member else ANBIMA_NON_MEMBER_URL
     # url example: https://www.anbima.com.br/informacoes/merc-sec/arqs/ms231128.txt
     url = f"{base_url}ms{url_date}.txt"
 
     try:
         df = pd.read_csv(
             url,
             sep="@",
             encoding="latin-1",
             skiprows=2,
             decimal=",",
             thousands=".",
+            na_values=["--"],
             dtype_backend="numpy_nullable",
         )
     except HTTPError:
-        error_date = normalized_date.strftime("%d-%m-%Y")
+        error_date = reference_date.strftime("%d-%m-%Y")
         raise ValueError(f"Failed to get ANBIMA rates for {error_date}")
 
     return df
 
 
 def process_raw_data(df_raw: DataFrame) -> DataFrame:
     """
```

### Comparing `pyield-0.4.0/pyield/br_calendar.py` & `pyield-0.4.1/pyield/br_calendar.py`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/pyield/br_holidays.py` & `pyield-0.4.1/pyield/br_holidays.py`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/pyield/br_holidays_new.txt` & `pyield-0.4.1/pyield/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/pyield/br_holidays_old.txt` & `pyield-0.4.1/pyield/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/pyield/di_futures.py` & `pyield-0.4.1/pyield/di_futures.py`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/pyield/di_web.py` & `pyield-0.4.1/pyield/di_web.py`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/pyield/di_xml.py` & `pyield-0.4.1/pyield/di_xml.py`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/pyproject.toml` & `pyield-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
 ]
 dynamic = []
-version = "0.4.0"
+version = "0.4.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.4.0/tests/test_br_calendar.py` & `pyield-0.4.1/tests/test_br_calendar.py`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/tests/test_di.py` & `pyield-0.4.1/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `pyield-0.4.0/PKG-INFO` & `pyield-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
```

