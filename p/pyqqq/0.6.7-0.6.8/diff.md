# Comparing `tmp/pyqqq-0.6.7.tar.gz` & `tmp/pyqqq-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.6.7.tar", max compression
+gzip compressed data, was "pyqqq-0.6.8.tar", max compression
```

## Comparing `pyqqq-0.6.7.tar` & `pyqqq-0.6.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.6.7/README.md
--rw-r--r--   0        0        0      770 2024-04-04 06:33:48.694307 pyqqq-0.6.7/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.6.7/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.6.7/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.6.7/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39030 2024-04-04 06:07:52.832635 pyqqq-0.6.7/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.6.7/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24011 2024-04-04 06:16:18.908889 pyqqq-0.6.7/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.6.7/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.6.7/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.6.7/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.6.7/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.6.7/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24353 2024-04-04 06:18:28.976735 pyqqq-0.6.7/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.6.7/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.6.7/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.6.7/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.6.7/pyqqq/data/daily.py
--rw-r--r--   0        0        0     4732 2024-04-04 05:49:48.948126 pyqqq-0.6.7/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     7289 2024-04-04 05:56:05.786196 pyqqq-0.6.7/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.6.7/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.6.7/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.6.7/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.6.7/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.6.7/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.6.7/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.6.7/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.6.7/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-28 03:41:58.980653 pyqqq-0.6.8/README.md
+-rw-r--r--   0        0        0      770 2024-04-04 09:57:09.216396 pyqqq-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-28 03:41:58.982907 pyqqq-0.6.8/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 03:59:43.302843 pyqqq-0.6.8/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 03:59:24.168676 pyqqq-0.6.8/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39030 2024-04-04 07:01:54.056230 pyqqq-0.6.8/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-28 03:41:58.983583 pyqqq-0.6.8/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24011 2024-04-04 07:01:54.056815 pyqqq-0.6.8/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 03:41:58.983800 pyqqq-0.6.8/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-03-04 03:59:43.302986 pyqqq-0.6.8/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 02:04:49.386336 pyqqq-0.6.8/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-28 03:41:58.984873 pyqqq-0.6.8/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-07 02:05:26.670417 pyqqq-0.6.8/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24353 2024-04-04 07:01:54.057121 pyqqq-0.6.8/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-22 01:44:28.626559 pyqqq-0.6.8/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-29 07:10:26.944955 pyqqq-0.6.8/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 02:05:26.670533 pyqqq-0.6.8/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-02 05:12:48.319458 pyqqq-0.6.8/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     6627 2024-04-04 09:52:46.291392 pyqqq-0.6.8/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     7289 2024-04-04 07:01:54.057407 pyqqq-0.6.8/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     1254 2024-03-22 01:44:28.626857 pyqqq-0.6.8/pyqqq/datatypes.py
+-rw-r--r--   0        0        0     4547 2024-04-04 09:52:23.392781 pyqqq-0.6.8/pyqqq/test.ipynb
+-rw-r--r--   0        0        0        0 2024-03-07 02:05:26.670737 pyqqq-0.6.8/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:49:01.142004 pyqqq-0.6.8/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-22 01:44:28.626942 pyqqq-0.6.8/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-03-04 03:59:43.304644 pyqqq-0.6.8/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-28 03:41:58.986410 pyqqq-0.6.8/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 02:18:36.457903 pyqqq-0.6.8/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-03-04 03:59:43.304764 pyqqq-0.6.8/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.8/PKG-INFO
```

### Comparing `pyqqq-0.6.7/README.md` & `pyqqq-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyproject.toml` & `pyqqq-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.6.7"
+version = "0.6.8"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.6.7/pyqqq/__init__.py` & `pyqqq-0.6.8/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.6.8/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.6.8/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.6.8/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.6.8/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.6.8/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.6.8/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.6.8/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.6.8/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.6.8/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/data/daily.py` & `pyqqq-0.6.8/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/data/domestic.py` & `pyqqq-0.6.8/pyqqq/data/domestic.py`

 * *Files 21% similar despite different names*

```diff
@@ -98,14 +98,85 @@
 
         df = pd.DataFrame(r.json())
         if not df.empty:
             df.set_index("code", inplace=True)
         return df
 
 
+def get_ticker_info(code: str) -> pd.DataFrame | None:
+    """
+    종목의 기본정보를 조회합니다.
+
+    Args:
+        code (str): 조회할 종목의 코드
+
+    Returns:
+        pd.DataFrame|None: 기본정보 리스트. 데이터가 없으면 None
+
+        - code (str, index): 종목코드
+        - isin (str): 국제 증권 식별 번호
+        - name (str): 이름
+        - market (str): 거래소
+
+    Examples:
+        >>> df = get_ticker_info("005930")
+        >>> print(df)
+                isin  name market
+        code
+        005930  KR7005930003  삼성전자  KOSPI
+    """
+    return _ticker_request('code', code)
+
+
+def find_ticker_info(name: str) -> pd.DataFrame | None:
+    """
+    종목명으로 기본정보를 조회합니다.
+
+    Args:
+        name (str): 조회할 종목의 이름
+
+    Returns:
+        pd.DataFrame|None: 기본정보 리스트. 데이터가 없으면 None, 중복되는 이름이 있으면 최대 20개까지 반환됩니다.
+
+    Examples:
+        >>> df = find_ticker_info("삼성")
+        >>> print(df.head())
+                isin   name market
+        code
+        000810  KR7000810002   삼성화재  KOSPI
+        000815  KR7000811000  삼성화재우  KOSPI
+        001360  KR7001360007   삼성제약  KOSPI
+        005930  KR7005930003   삼성전자  KOSPI
+        005935  KR7005931001  삼성전자우  KOSPI
+    """
+    return _ticker_request('name', name)
+
+
+def _ticker_request(type: str, value: str):
+    url = f"{c.PYQQQ_API_URL}/domestic-stock/tickers"
+    params = {
+        type: value
+    }
+
+    r = _send_request("GET", url, params=params)
+    if r.status_code == 404:
+        return None
+    else:
+        _raise_for_status(r)
+
+    if type == 'code':
+        df = pd.DataFrame([r.json()])
+    else:
+        df = pd.DataFrame(r.json())
+
+    if not df.empty:
+        df.set_index("code", inplace=True)
+    return df
+
+
 @retry(requests.HTTPError)
 def _send_request(method: str, url: str, **kwargs):
     api_key = get_api_key()
     if not api_key:
         raise ValueError("API key is not set")
 
     return requests.request(
```

### Comparing `pyqqq-0.6.7/pyqqq/data/realtime.py` & `pyqqq-0.6.8/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/datatypes.py` & `pyqqq-0.6.8/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/utils/display.py` & `pyqqq-0.6.8/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/utils/kvstore.py` & `pyqqq-0.6.8/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/utils/limiter.py` & `pyqqq-0.6.8/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/utils/logger.py` & `pyqqq-0.6.8/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/utils/market_schedule.py` & `pyqqq-0.6.8/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/pyqqq/utils/retry.py` & `pyqqq-0.6.8/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.7/PKG-INFO` & `pyqqq-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.6.7
+Version: 0.6.8
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

