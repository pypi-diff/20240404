# Comparing `tmp/lumiwealth-tradier-0.1.6.tar.gz` & `tmp/lumiwealth-tradier-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumiwealth-tradier-0.1.6.tar", last modified: Fri Feb 23 23:28:41 2024, max compression
+gzip compressed data, was "lumiwealth-tradier-0.1.7.tar", last modified: Thu Apr  4 06:16:13 2024, max compression
```

## Comparing `lumiwealth-tradier-0.1.6.tar` & `lumiwealth-tradier-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-02-23 23:28:41.924515 lumiwealth-tradier-0.1.6/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11357 2024-01-10 19:56:47.000000 lumiwealth-tradier-0.1.6/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5541 2024-02-23 23:28:41.924310 lumiwealth-tradier-0.1.6/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4880 2024-01-18 21:05:36.000000 lumiwealth-tradier-0.1.6/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-02-23 23:28:41.918817 lumiwealth-tradier-0.1.6/lumiwealth_tradier/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       43 2024-01-10 19:56:47.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11164 2024-01-22 23:41:14.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier/account.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4479 2024-01-22 23:41:14.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier/base.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18587 2024-01-22 23:41:14.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier/market.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11208 2024-02-23 22:52:40.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier/orders.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      561 2024-01-10 19:56:47.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-02-23 23:28:41.920996 lumiwealth-tradier-0.1.6/lumiwealth_tradier.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5541 2024-02-23 23:28:41.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      518 2024-02-23 23:28:41.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-02-23 23:28:41.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       20 2024-02-23 23:28:41.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       25 2024-02-23 23:28:41.000000 lumiwealth-tradier-0.1.6/lumiwealth_tradier.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-01-10 19:56:47.000000 lumiwealth-tradier-0.1.6/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1258 2024-02-23 23:28:41.925276 lumiwealth-tradier-0.1.6/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      896 2024-02-23 23:24:41.000000 lumiwealth-tradier-0.1.6/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-02-23 23:28:41.923301 lumiwealth-tradier-0.1.6/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-01-10 19:56:47.000000 lumiwealth-tradier-0.1.6/tests/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      636 2024-01-10 19:56:47.000000 lumiwealth-tradier-0.1.6/tests/test_account.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6779 2024-02-23 22:52:40.000000 lumiwealth-tradier-0.1.6/tests/test_market.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4019 2024-02-23 22:52:40.000000 lumiwealth-tradier-0.1.6/tests/test_orders.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-04 06:16:13.860608 lumiwealth-tradier-0.1.7/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11357 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5541 2024-04-04 06:16:13.860543 lumiwealth-tradier-0.1.7/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4880 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-04 06:16:13.858828 lumiwealth-tradier-0.1.7/lumiwealth_tradier/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       43 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11164 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier/account.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4479 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier/base.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18587 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier/market.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    14208 2024-04-04 06:03:23.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier/orders.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      561 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-04 06:16:13.860284 lumiwealth-tradier-0.1.7/lumiwealth_tradier.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5541 2024-04-04 06:16:13.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      518 2024-04-04 06:16:13.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-04 06:16:13.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       20 2024-04-04 06:16:13.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       25 2024-04-04 06:16:13.000000 lumiwealth-tradier-0.1.7/lumiwealth_tradier.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1258 2024-04-04 06:16:13.860895 lumiwealth-tradier-0.1.7/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      896 2024-04-04 06:12:34.000000 lumiwealth-tradier-0.1.7/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-04 06:16:13.860080 lumiwealth-tradier-0.1.7/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/tests/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      636 2024-03-31 04:17:12.000000 lumiwealth-tradier-0.1.7/tests/test_account.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7769 2024-03-31 04:56:13.000000 lumiwealth-tradier-0.1.7/tests/test_market.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7806 2024-04-04 06:04:34.000000 lumiwealth-tradier-0.1.7/tests/test_orders.py
```

### Comparing `lumiwealth-tradier-0.1.6/LICENSE` & `lumiwealth-tradier-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/PKG-INFO` & `lumiwealth-tradier-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumiwealth-tradier
-Version: 0.1.6
+Version: 0.1.7
 Summary: lumiwealth-tradier is a Python package that serves as a wrapper for the Tradier brokerage API. This package simplifies the process of making API requests, handling responses, and performing various trading and account management operations.
 Home-page: https://github.com/Lumiwealth/lumiwealth-tradier
 Author: David MacLeod and Robert Grzesik
 Project-URL: Bug Tracker, https://github.com/Lumiwealth/lumiwealth-tradier/issues
 Keywords: tradier finance api
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lumiwealth-tradier Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: lumiwealth-tradier Version: 0.1.7 Summary:
 lumiwealth-tradier is a Python package that serves as a wrapper for the Tradier
 brokerage API. This package simplifies the process of making API requests,
 handling responses, and performing various trading and account management
 operations. Home-page: https://github.com/Lumiwealth/lumiwealth-tradier Author:
 David MacLeod and Robert Grzesik Project-URL: Bug Tracker, https://github.com/
 Lumiwealth/lumiwealth-tradier/issues Keywords: tradier finance api Requires-
 Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `lumiwealth-tradier-0.1.6/README.md` & `lumiwealth-tradier-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/lumiwealth_tradier/account.py` & `lumiwealth-tradier-0.1.7/lumiwealth_tradier/account.py`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/lumiwealth_tradier/base.py` & `lumiwealth-tradier-0.1.7/lumiwealth_tradier/base.py`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/lumiwealth_tradier/market.py` & `lumiwealth-tradier-0.1.7/lumiwealth_tradier/market.py`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/lumiwealth_tradier/orders.py` & `lumiwealth-tradier-0.1.7/lumiwealth_tradier/orders.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 import re
 from typing import Union
 
 import pandas as pd
 
 from .base import TradierApiBase, TradierApiError
 
+class OrderLeg:
+    def __init__(self, option_symbol: str, side: str, quantity: int, price: float = None):
+        self.option_symbol = option_symbol
+        self.side = side
+        self.quantity = quantity
+        self.price = price
+
 
 class Orders(TradierApiBase):
     def __init__(self, account_number, auth_token, is_paper=True):
         TradierApiBase.__init__(self, account_number, auth_token, is_paper)
 
         # Order endpoint
         self.ORDER_ENDPOINT = f"v1/accounts/{self.ACCOUNT_NUMBER}/orders"  # POST
@@ -46,15 +53,17 @@
         :param order_id:  Order ID reported by the order() or order_option() functions
         :param include_tag:  Include the tag column in the DataFrame. Default is True.
         :return:
         """
         payload = {
             "includeTags": include_tag,
         }
-        data = self.request(endpoint=f"{self.ORDER_ENDPOINT}/{order_id}", params=payload)
+        data = self.request(
+            endpoint=f"{self.ORDER_ENDPOINT}/{order_id}", params=payload
+        )
         if "order" not in data:
             return pd.DataFrame()
 
         return pd.json_normalize(data["order"])
 
     def get_orders(self, include_tag=True) -> pd.DataFrame:
         """
@@ -230,33 +239,113 @@
             "symbol": asset_symbol.upper(),
             "option_symbol": option_symbol.upper(),
             "side": side.lower(),
             "quantity": int(quantity),
             "type": order_type.lower(),
             "duration": duration.lower(),
         }
-        self._update_order_payload(payload, limit_price, order_type, stop_price, tag)
+        payload = self._update_order_payload(
+            payload, limit_price, order_type, stop_price, tag
+        )
 
+        # Send the request to the Tradier API
         response = self.send(self.ORDER_ENDPOINT, payload)
+
+        # Return the response
+        return response["order"]
+
+    def multileg_order(
+        self,
+        symbol: str,
+        order_type: str,
+        duration: str,
+        legs: list[OrderLeg],
+        price: float = None,
+        tag: str = "",
+    ) -> dict:
+        """
+        Place a multi-leg order with the Tradier API.
+
+        :param symbol: The symbol of the underlying asset for the options.
+        :param order_type: The type of order ('market', 'debit', 'credit', 'even').
+        :param duration: The duration of the order ('day', 'gtc', 'pre', 'post').
+        :param legs: A list of OrderLeg objects, each representing one leg of the multi-leg order.
+        :param price: The price for the order, required only for 'debit' and 'credit' orders.
+        :param tag: An optional tag for the order.
+        :return: A dictionary representing the API's response.
+        """
+        # Ensure there are no more than 4 legs
+        if len(legs) > 4:
+            raise ValueError("A multi-leg order can have up to 4 legs.")
+
+        # Start constructing the data payload
+        data = {
+            "class": "multileg",
+            "symbol": symbol.upper(),
+            "type": order_type.lower(),
+            "duration": duration.lower(),
+        }
+
+        if price is not None:
+            data["price"] = price
+
+        if tag:
+            data["tag"] = tag
+
+        # Add the details of each leg to the data payload
+        for index, leg in enumerate(legs):
+            # Check the validity of the leg data
+            if not isinstance(leg, OrderLeg):
+                raise ValueError(f"Leg at index {index} is not an OrderLeg object.")
+
+            if leg.side.lower() not in [
+                "buy_to_open",
+                "buy_to_close",
+                "sell_to_open",
+                "sell_to_close",
+            ]:
+                raise ValueError(
+                    f"Invalid side for leg at index {index}. Must be one of ['buy_to_open', 'buy_to_close', 'sell_to_open', 'sell_to_close']"
+                )
+
+            if not isinstance(leg.quantity, int) or leg.quantity <= 0:
+                raise ValueError(
+                    f"Invalid quantity for leg at index {index}. Must be a positive integer."
+                )
+
+            data[f"option_symbol[{index}]"] = leg.option_symbol.upper()
+            data[f"side[{index}]"] = leg.side.lower()
+            data[f"quantity[{index}]"] = int(leg.quantity)
+
+        # Send the request to the Tradier API
+        response = self.send(self.ORDER_ENDPOINT, data)
+
+        # Return the response
         return response["order"]
 
     @staticmethod
     def _update_order_payload(payload, limit_price, order_type, stop_price, tag):
         if order_type.lower() == "limit" or order_type.lower() == "stop_limit":
             payload["price"] = round(limit_price, 2)
         if order_type.lower() == "stop" or order_type.lower() == "stop_limit":
             payload["stop"] = round(stop_price, 2)
         if tag:
             payload["tag"] = tag
 
+        return payload
+
     def _check_order_inputs(self, duration, limit_price, order_type, stop_price, tag):
         if order_type.lower() not in self.valid_order_types:
-            raise ValueError(f"Invalid order_type. Must be one of {self.valid_order_types}")
+            raise ValueError(
+                f"Invalid order_type. Must be one of {self.valid_order_types}"
+            )
         if duration.lower() not in self.valid_durations:
             raise ValueError(f"Invalid duration. Must be one of {self.valid_durations}")
         if order_type.lower() in ["limit", "stop_limit"] and not limit_price:
             raise ValueError(f"Limit price is required for order_type {order_type}")
         if order_type.lower() in ["stop", "stop_limit"] and not stop_price:
             raise ValueError(f"Stop price is required for order_type {order_type}")
         # Check that 'tag' only has letters, mumbers and dash (-)
         if tag and not re.match(r"^[a-zA-Z0-9-]+$", tag):
-            raise ValueError(f"Invalid tag {tag}. Must be letters, numbers and dash (-) characters")
+            raise ValueError(
+                f"Invalid tag {tag}. Must be letters, numbers and dash (-) characters"
+            )
```

### Comparing `lumiwealth-tradier-0.1.6/lumiwealth_tradier/tradier.py` & `lumiwealth-tradier-0.1.7/lumiwealth_tradier/tradier.py`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/lumiwealth_tradier.egg-info/PKG-INFO` & `lumiwealth-tradier-0.1.7/lumiwealth_tradier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumiwealth-tradier
-Version: 0.1.6
+Version: 0.1.7
 Summary: lumiwealth-tradier is a Python package that serves as a wrapper for the Tradier brokerage API. This package simplifies the process of making API requests, handling responses, and performing various trading and account management operations.
 Home-page: https://github.com/Lumiwealth/lumiwealth-tradier
 Author: David MacLeod and Robert Grzesik
 Project-URL: Bug Tracker, https://github.com/Lumiwealth/lumiwealth-tradier/issues
 Keywords: tradier finance api
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lumiwealth-tradier Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: lumiwealth-tradier Version: 0.1.7 Summary:
 lumiwealth-tradier is a Python package that serves as a wrapper for the Tradier
 brokerage API. This package simplifies the process of making API requests,
 handling responses, and performing various trading and account management
 operations. Home-page: https://github.com/Lumiwealth/lumiwealth-tradier Author:
 David MacLeod and Robert Grzesik Project-URL: Bug Tracker, https://github.com/
 Lumiwealth/lumiwealth-tradier/issues Keywords: tradier finance api Requires-
 Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `lumiwealth-tradier-0.1.6/lumiwealth_tradier.egg-info/SOURCES.txt` & `lumiwealth-tradier-0.1.7/lumiwealth_tradier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/pyproject.toml` & `lumiwealth-tradier-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/setup.cfg` & `lumiwealth-tradier-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/setup.py` & `lumiwealth-tradier-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="lumiwealth-tradier",
-    version="0.1.6",
+    version="0.1.7",
     author="David MacLeod and Robert Grzesik",
     description="lumiwealth-tradier is a Python package that serves as a wrapper for the Tradier brokerage API. "
     "This package simplifies the process of making API requests, handling responses, and performing various trading "
     "and account management operations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumiwealth-tradier",
```

### Comparing `lumiwealth-tradier-0.1.6/tests/test_account.py` & `lumiwealth-tradier-0.1.7/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `lumiwealth-tradier-0.1.6/tests/test_market.py` & `lumiwealth-tradier-0.1.7/tests/test_market.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,41 @@
         assert df.loc['MSFT']['last'] > 0
         assert 'bad_symbol' not in df.index
 
         with pytest.raises(ValueError):
             tradier.market.get_last_price('bad_symbol')
 
         assert tradier.market.get_last_price('AAPL') > 0
+        
+    def test_quote_options(self, tradier):
+        # Test getting a quote for an option
+        df_expr = tradier.market.get_option_expirations('SPY')
+        assert df_expr is not None
+        expr_date = df_expr.index[0]
+        strike = df_expr.iloc[0]['strikes'][0]
+
+        # Get the option chains
+        df = tradier.market.get_option_chains('SPY', expr_date)
+        assert df is not None
+        assert len(df) > 0
+        assert 'strike' in df.columns
+        assert df.iloc[0]['strike'] > 0
+
+        # Get the option symbols - lookup chains
+        symbol = tradier.market.get_option_symbol('SPY', expr_date, strike, 'call')
+        assert symbol is not None
+        assert isinstance(symbol, str)
+        assert symbol != ''
+        assert re.match(r'SPY\d+C\d+', symbol)
+
+        # Get the quote for the option
+        df = tradier.market.get_quotes([symbol])
+        assert df is not None
+        assert 'last' in df.columns
+        assert df.loc[symbol]['last'] > 0
 
     def test_historical_quote(self, tradier):
         # Multiple row return
         df = tradier.market.get_historical_quotes('SPY', start_date='2023-12-01', end_date='2023-12-07')
         assert df is not None
         assert 'open' in df.columns
         assert df.iloc[0]['open'] > 0
```

