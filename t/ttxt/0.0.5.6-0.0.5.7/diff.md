# Comparing `tmp/ttxt-0.0.5.6.tar.gz` & `tmp/ttxt-0.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttxt-0.0.5.6.tar", last modified: Sat Mar 30 03:47:47 2024, max compression
+gzip compressed data, was "ttxt-0.0.5.7.tar", last modified: Thu Apr  4 18:26:50 2024, max compression
```

## Comparing `ttxt-0.0.5.6.tar` & `ttxt-0.0.5.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-03-30 03:47:47.747989 ttxt-0.0.5.6/
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.5.6/LICENSE
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-03-30 03:47:47.747874 ttxt-0.0.5.6/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.5.6/README.md
--rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-03-30 03:47:47.748031 ttxt-0.0.5.6/setup.cfg
--rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-03-30 03:47:39.000000 ttxt-0.0.5.6/setup.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-03-30 03:47:47.739964 ttxt-0.0.5.6/ttxt/
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1040 2024-03-14 11:17:46.000000 ttxt-0.0.5.6/ttxt/__init__.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-03-30 03:47:47.741029 ttxt-0.0.5.6/ttxt/base/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.5.6/ttxt/base/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.5.6/ttxt/base/baseFuturesExchange.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.5.6/ttxt/base/baseSpotExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-03-30 03:47:47.745849 ttxt-0.0.5.6/ttxt/exchanges/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.5.6/ttxt/exchanges/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.5.6/ttxt/exchanges/biconomy.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.5.6/ttxt/exchanges/binance.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.5.6/ttxt/exchanges/bingx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.5.6/ttxt/exchanges/bitget.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.5.6/ttxt/exchanges/bitgetFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.5.6/ttxt/exchanges/bitmart.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    20701 2024-03-30 03:47:36.000000 ttxt-0.0.5.6/ttxt/exchanges/bybit.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.5.6/ttxt/exchanges/bybitFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.5.6/ttxt/exchanges/cryptocom.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.5.6/ttxt/exchanges/gateFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.5.6/ttxt/exchanges/gateio.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.5.6/ttxt/exchanges/huobi.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.5.6/ttxt/exchanges/kucoin.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.5.6/ttxt/exchanges/mexc.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11776 2024-03-22 17:17:12.000000 ttxt-0.0.5.6/ttxt/exchanges/okx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.5.6/ttxt/exchanges/xt.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-03-30 03:47:47.746026 ttxt-0.0.5.6/ttxt/tests/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.5.6/ttxt/tests/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9606 2024-03-30 03:47:36.000000 ttxt-0.0.5.6/ttxt/tests/testExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-03-30 03:47:47.746284 ttxt-0.0.5.6/ttxt/types/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.5.6/ttxt/types/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.5.6/ttxt/types/baseTypes.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-03-30 03:47:47.746979 ttxt-0.0.5.6/ttxt/utils/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.5.6/ttxt/utils/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.5.6/ttxt/utils/general.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.5.6/ttxt/utils/xtUtils.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-03-30 03:47:47.740583 ttxt-0.0.5.6/ttxt.egg-info/
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-03-30 03:47:47.000000 ttxt-0.0.5.6/ttxt.egg-info/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)      844 2024-03-30 03:47:47.000000 ttxt-0.0.5.6/ttxt.egg-info/SOURCES.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-03-30 03:47:47.000000 ttxt-0.0.5.6/ttxt.egg-info/dependency_links.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-03-30 03:47:47.000000 ttxt-0.0.5.6/ttxt.egg-info/top_level.txt
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:26:50.052585 ttxt-0.0.5.7/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.5.7/LICENSE
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-04-04 18:26:50.052448 ttxt-0.0.5.7/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.5.7/README.md
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-04-04 18:26:50.052629 ttxt-0.0.5.7/setup.cfg
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-04-04 18:26:47.000000 ttxt-0.0.5.7/setup.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:26:50.044846 ttxt-0.0.5.7/ttxt/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1040 2024-03-14 11:17:46.000000 ttxt-0.0.5.7/ttxt/__init__.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:26:50.045821 ttxt-0.0.5.7/ttxt/base/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.5.7/ttxt/base/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.5.7/ttxt/base/baseFuturesExchange.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.5.7/ttxt/base/baseSpotExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:26:50.050861 ttxt-0.0.5.7/ttxt/exchanges/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.5.7/ttxt/exchanges/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.5.7/ttxt/exchanges/biconomy.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.5.7/ttxt/exchanges/binance.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.5.7/ttxt/exchanges/bingx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.5.7/ttxt/exchanges/bitget.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.5.7/ttxt/exchanges/bitgetFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.5.7/ttxt/exchanges/bitmart.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    20701 2024-03-30 03:47:36.000000 ttxt-0.0.5.7/ttxt/exchanges/bybit.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.5.7/ttxt/exchanges/bybitFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.5.7/ttxt/exchanges/cryptocom.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.5.7/ttxt/exchanges/gateFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.5.7/ttxt/exchanges/gateio.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.5.7/ttxt/exchanges/huobi.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.5.7/ttxt/exchanges/kucoin.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.5.7/ttxt/exchanges/mexc.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11780 2024-04-04 18:25:40.000000 ttxt-0.0.5.7/ttxt/exchanges/okx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.5.7/ttxt/exchanges/xt.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:26:50.051036 ttxt-0.0.5.7/ttxt/tests/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.5.7/ttxt/tests/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     9606 2024-04-04 18:26:15.000000 ttxt-0.0.5.7/ttxt/tests/testExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:26:50.051279 ttxt-0.0.5.7/ttxt/types/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.5.7/ttxt/types/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.5.7/ttxt/types/baseTypes.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:26:50.051854 ttxt-0.0.5.7/ttxt/utils/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.5.7/ttxt/utils/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.5.7/ttxt/utils/general.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.5.7/ttxt/utils/xtUtils.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-04-04 18:26:50.045379 ttxt-0.0.5.7/ttxt.egg-info/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-04-04 18:26:50.000000 ttxt-0.0.5.7/ttxt.egg-info/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      844 2024-04-04 18:26:50.000000 ttxt-0.0.5.7/ttxt.egg-info/SOURCES.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-04-04 18:26:50.000000 ttxt-0.0.5.7/ttxt.egg-info/dependency_links.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-04-04 18:26:50.000000 ttxt-0.0.5.7/ttxt.egg-info/top_level.txt
```

### Comparing `ttxt-0.0.5.6/LICENSE` & `ttxt-0.0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/__init__.py` & `ttxt-0.0.5.7/ttxt/__init__.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/base/baseFuturesExchange.py` & `ttxt-0.0.5.7/ttxt/base/baseFuturesExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/base/baseSpotExchange.py` & `ttxt-0.0.5.7/ttxt/base/baseSpotExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/biconomy.py` & `ttxt-0.0.5.7/ttxt/exchanges/biconomy.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/binance.py` & `ttxt-0.0.5.7/ttxt/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/bingx.py` & `ttxt-0.0.5.7/ttxt/exchanges/bingx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/bitget.py` & `ttxt-0.0.5.7/ttxt/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/bitgetFutures.py` & `ttxt-0.0.5.7/ttxt/exchanges/bitgetFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/bitmart.py` & `ttxt-0.0.5.7/ttxt/exchanges/bitmart.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/bybit.py` & `ttxt-0.0.5.7/ttxt/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/bybitFutures.py` & `ttxt-0.0.5.7/ttxt/exchanges/bybitFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/cryptocom.py` & `ttxt-0.0.5.7/ttxt/exchanges/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/gateFutures.py` & `ttxt-0.0.5.7/ttxt/exchanges/gateFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/gateio.py` & `ttxt-0.0.5.7/ttxt/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/huobi.py` & `ttxt-0.0.5.7/ttxt/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/kucoin.py` & `ttxt-0.0.5.7/ttxt/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/mexc.py` & `ttxt-0.0.5.7/ttxt/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/exchanges/okx.py` & `ttxt-0.0.5.7/ttxt/exchanges/okx.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,16 @@
             parsedData["asks"] = [[float(d[0]), float(d[1])] for d in orderbookData["asks"]]
         else: parsedData["asks"] = []
         return parsedData
 
     def _parseCreateOrder(self, order):
         parsedOrder = {}
         if order['code'] != "0": raise Exception(order["msg"])
-        order = order['data']
-        parsedOrder["id"] = order.get('ordId', None)
+        order = order['data'][0]
+        parsedOrder["id"] = order['data'][0]['ordId']
         parsedOrder["symbol"] = None
         parsedOrder["price"] = None
         parsedOrder["amount"] = None
         parsedOrder["side"] = None
         parsedOrder["timestamp"] = float(order["outTime"]) if "outTime" in order else None
         parsedOrder["status"] = None
         parsedOrder["orderJson"] = json.dumps(order) if order else None
```

### Comparing `ttxt-0.0.5.6/ttxt/tests/testExchange.py` & `ttxt-0.0.5.7/ttxt/tests/testExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/types/baseTypes.py` & `ttxt-0.0.5.7/ttxt/types/baseTypes.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/utils/general.py` & `ttxt-0.0.5.7/ttxt/utils/general.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt/utils/xtUtils.py` & `ttxt-0.0.5.7/ttxt/utils/xtUtils.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.5.6/ttxt.egg-info/SOURCES.txt` & `ttxt-0.0.5.7/ttxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

