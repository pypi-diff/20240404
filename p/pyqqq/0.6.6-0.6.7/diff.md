# Comparing `tmp/pyqqq-0.6.6.tar.gz` & `tmp/pyqqq-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.6.6.tar", max compression
+gzip compressed data, was "pyqqq-0.6.7.tar", max compression
```

## Comparing `pyqqq-0.6.6.tar` & `pyqqq-0.6.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      588 2024-03-27 01:29:00.427186 pyqqq-0.6.6/README.md
--rw-r--r--   0        0        0      770 2024-04-03 06:51:28.218085 pyqqq-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-27 01:29:00.428734 pyqqq-0.6.6/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681470 pyqqq-0.6.6/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 00:30:01.958621 pyqqq-0.6.6/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39030 2024-04-03 05:52:28.780328 pyqqq-0.6.6/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-27 01:29:00.428888 pyqqq-0.6.6/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    23893 2024-03-21 21:27:23.752968 pyqqq-0.6.6/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-27 03:32:53.313827 pyqqq-0.6.6/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681703 pyqqq-0.6.6/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-03 06:40:50.199892 pyqqq-0.6.6/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-27 01:29:00.429820 pyqqq-0.6.6/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-06 00:30:01.960145 pyqqq-0.6.6/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24236 2024-04-03 06:50:33.478579 pyqqq-0.6.6/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-13 01:10:46.718207 pyqqq-0.6.6/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-27 01:29:00.429926 pyqqq-0.6.6/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-06 03:23:32.374681 pyqqq-0.6.6/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-02 21:29:24.457028 pyqqq-0.6.6/pyqqq/data/daily.py
--rw-r--r--   0        0        0     4732 2024-04-03 05:31:57.184605 pyqqq-0.6.6/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     7295 2024-04-03 04:32:36.601513 pyqqq-0.6.6/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-12 13:30:35.556769 pyqqq-0.6.6/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-06 03:23:38.166158 pyqqq-0.6.6/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-02 21:29:24.457837 pyqqq-0.6.6/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 13:30:35.556892 pyqqq-0.6.6/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-28 02:16:13.684707 pyqqq-0.6.6/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-27 01:29:00.430437 pyqqq-0.6.6/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-02 21:29:24.458374 pyqqq-0.6.6/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-28 02:16:13.684870 pyqqq-0.6.6/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.6.7/README.md
+-rw-r--r--   0        0        0      770 2024-04-04 06:33:48.694307 pyqqq-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.6.7/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.6.7/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.6.7/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39030 2024-04-04 06:07:52.832635 pyqqq-0.6.7/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.6.7/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24011 2024-04-04 06:16:18.908889 pyqqq-0.6.7/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.6.7/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.6.7/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.6.7/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.6.7/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.6.7/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24353 2024-04-04 06:18:28.976735 pyqqq-0.6.7/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.6.7/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.6.7/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.6.7/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.6.7/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     4732 2024-04-04 05:49:48.948126 pyqqq-0.6.7/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     7289 2024-04-04 05:56:05.786196 pyqqq-0.6.7/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.6.7/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.6.7/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.6.7/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.6.7/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.6.7/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.6.7/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.6.7/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.6.7/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.6.7/PKG-INFO
```

### Comparing `pyqqq-0.6.6/README.md` & `pyqqq-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyproject.toml` & `pyqqq-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.6.6"
+version = "0.6.7"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.6.6/pyqqq/__init__.py` & `pyqqq-0.6.7/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.6.7/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
 
     @limit_calls(scope="ebest/t0424", max_calls=1)
     def get_stock_balance(
         self,
         prcgb: int = 1,
         chegb: int = 0,
         dangb: int = 0,
-        charge: int = 1,
+        charge: int = 0,
         cts_expcode: str = "",
         tr_cont_key: str = "",
     ):
         """
         ([주식]계좌) 주식잔고2조회 (t0424)
 
         Args:
```

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.6.7/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.6.7/pyqqq/brokerage/ebest/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     """ 평균 매입 가격 """
     current_price: int
     """ 현재 가격 """
     current_value: int
     """ 현재 가치 """
     current_pnl: Decimal
     """ 현재 손익률 """
+    current_pnl_value: int
+    """ 현재 손익 금액 """
 
 
 @dataclass
 class EBestStockOrder:
     """
     주식 주문 정보를 담는 데이터 클래스입니다.
     """
@@ -180,14 +182,15 @@
                     asset_code=el["expcode"],
                     asset_name=el["hname"],
                     quantity=int(el["janqty"]),
                     average_purchase_price=Decimal(el["pamt"]),
                     current_price=int(el["price"]),
                     current_value=int(el["appamt"]),
                     current_pnl=Decimal(el["sunikrt"]),
+                    current_pnl_value=int(el["dtsunik"]),
                 )
 
                 if position.quantity > 0:
                     result.append(position)
 
             if cts_expcode.strip() == "":
                 fetching = False
```

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.6.7/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.6.7/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.6.7/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.6.7/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.6.7/pyqqq/brokerage/kis/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     """ 평균 매입 가격 """
     current_price: int
     """ 현재 가격 """
     current_value: int
     """ 현재 가치 """
     current_pnl: Decimal
     """ 현재 손익률 """
+    current_pnl_value: int
+    """ 현재 손익 금액 """
 
 
 @dataclass
 class KISStockOrder:
     """
     주식 주문 정보를 담는 데이터 클래스입니다.
     """
@@ -114,15 +116,15 @@
         )
 
         result = {
             "total_balance": int(data["tot_evlu_amt"]),
             "purchase_amount": purchase_amount,
             "evaluated_amount": int(data["evlu_amt_smtl_amt"]),
             "pnl_amount": pnl_amount,
-            "pnl_rate": pnl_amount,
+            "pnl_rate": pnl_rate,
         }
         return result
 
     def get_possible_quantity(self,
                               asset_code: str,
                               order_type: OrderType = OrderType.MARKET,
                               price: int = 0) -> dict:
@@ -208,14 +210,15 @@
                     asset_code=el["pdno"],
                     asset_name=el["prdt_name"],
                     quantity=int(el["hldg_qty"]),
                     average_purchase_price=Decimal(el["pchs_avg_pric"]),
                     current_price=int(el["prpr"]),
                     current_value=int(el["evlu_amt"]),
                     current_pnl=Decimal(el["evlu_pfls_rt"]),
+                    current_pnl_value=el["evlu_pfls_amt"],
                 )
 
                 if position.quantity > 0:
                     result.append(position)
 
             if r["tr_cont"] in ["F", "M"]:
                 tr_cont = "N"
```

### Comparing `pyqqq-0.6.6/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.6.7/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/data/daily.py` & `pyqqq-0.6.7/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/data/domestic.py` & `pyqqq-0.6.7/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/data/realtime.py` & `pyqqq-0.6.7/pyqqq/data/realtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             - bidho (int): 매수호가
             - status (str): 장정보
             - jnilvolume (int): 전일거래량
             - shcode (str): 종목코드
 
     """
 
-    r = requests.get(f"https://qupiato.com/api/domestic-stock/trades")
+    r = requests.get(f"{c.PYQQQ_API_URL}/domestic-stock/trades")
     r.raise_for_status()
 
     data = r.json()
     result = [data[k] for k in data.keys()]
 
     return result
```

### Comparing `pyqqq-0.6.6/pyqqq/datatypes.py` & `pyqqq-0.6.7/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/utils/display.py` & `pyqqq-0.6.7/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/utils/kvstore.py` & `pyqqq-0.6.7/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/utils/limiter.py` & `pyqqq-0.6.7/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/utils/logger.py` & `pyqqq-0.6.7/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/utils/market_schedule.py` & `pyqqq-0.6.7/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/pyqqq/utils/retry.py` & `pyqqq-0.6.7/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.6.6/PKG-INFO` & `pyqqq-0.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.6.6
+Version: 0.6.7
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

