# Comparing `tmp/vcx_py-1.1.4.tar.gz` & `tmp/vcx_py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcx_py-1.1.4.tar", last modified: Tue Apr  2 17:15:30 2024, max compression
+gzip compressed data, was "vcx_py-1.2.0.tar", last modified: Thu Apr  4 15:21:54 2024, max compression
```

## Comparing `vcx_py-1.1.4.tar` & `vcx_py-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-02 17:15:30.152453 vcx_py-1.1.4/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1075 2024-03-15 22:12:30.000000 vcx_py-1.1.4/LICENSE
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4626 2024-04-02 17:15:30.152453 vcx_py-1.1.4/PKG-INFO
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4336 2024-04-01 14:03:55.000000 vcx_py-1.1.4/README.md
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)       38 2024-04-02 17:15:30.152453 vcx_py-1.1.4/setup.cfg
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      931 2024-04-02 17:15:27.000000 vcx_py-1.1.4/setup.py
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-02 17:15:30.152453 vcx_py-1.1.4/vcx_py/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      792 2024-03-18 23:09:16.000000 vcx_py-1.1.4/vcx_py/__init__.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)    10366 2024-04-02 17:15:09.000000 vcx_py-1.1.4/vcx_py/client.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     2365 2024-03-21 19:20:57.000000 vcx_py-1.1.4/vcx_py/constants.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1695 2024-03-22 19:04:00.000000 vcx_py-1.1.4/vcx_py/schema.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3065 2024-03-28 19:39:06.000000 vcx_py-1.1.4/vcx_py/utils.py
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-02 17:15:30.152453 vcx_py-1.1.4/vcx_py.egg-info/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4626 2024-04-02 17:15:30.000000 vcx_py-1.1.4/vcx_py.egg-info/PKG-INFO
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      235 2024-04-02 17:15:30.000000 vcx_py-1.1.4/vcx_py.egg-info/SOURCES.txt
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        1 2024-04-02 17:15:30.000000 vcx_py-1.1.4/vcx_py.egg-info/dependency_links.txt
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        7 2024-04-02 17:15:30.000000 vcx_py-1.1.4/vcx_py.egg-info/top_level.txt
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-04 15:21:54.796413 vcx_py-1.2.0/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1075 2024-03-15 22:12:30.000000 vcx_py-1.2.0/LICENSE
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4522 2024-04-04 15:21:54.796413 vcx_py-1.2.0/PKG-INFO
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4232 2024-04-04 15:19:55.000000 vcx_py-1.2.0/README.md
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)       38 2024-04-04 15:21:54.796413 vcx_py-1.2.0/setup.cfg
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      931 2024-04-04 15:20:57.000000 vcx_py-1.2.0/setup.py
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-04 15:21:54.796413 vcx_py-1.2.0/vcx_py/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      859 2024-04-04 15:01:28.000000 vcx_py-1.2.0/vcx_py/__init__.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)    10652 2024-04-04 14:59:46.000000 vcx_py-1.2.0/vcx_py/client.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     2857 2024-04-04 15:17:22.000000 vcx_py-1.2.0/vcx_py/constants.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1695 2024-03-22 19:04:00.000000 vcx_py-1.2.0/vcx_py/schema.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3682 2024-04-04 15:00:42.000000 vcx_py-1.2.0/vcx_py/utils.py
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-04 15:21:54.796413 vcx_py-1.2.0/vcx_py.egg-info/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4522 2024-04-04 15:21:54.000000 vcx_py-1.2.0/vcx_py.egg-info/PKG-INFO
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      235 2024-04-04 15:21:54.000000 vcx_py-1.2.0/vcx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        1 2024-04-04 15:21:54.000000 vcx_py-1.2.0/vcx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        7 2024-04-04 15:21:54.000000 vcx_py-1.2.0/vcx_py.egg-info/top_level.txt
```

### Comparing `vcx_py-1.1.4/LICENSE` & `vcx_py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.4/PKG-INFO` & `vcx_py-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcx_py
-Version: 1.1.4
+Version: 1.2.0
 Summary: A simple python client for the VirgoCX API
 Home-page: https://www.github.com/aarjaneiro/vcx_py
 Author: Aaron Janeiro Stone
 Author-email: aaron@thequant.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -152,26 +152,20 @@
 ```
 
 ## Warnings
 
 Note that due to CloudFlare protection, this version of the client attempts to access the API through its
 IP address and not the domain name. Should the IP address change, the client will need to be updated.
 Moreover, you will receive `InsecureRequestWarning` warnings when using the client until this issue is resolved.
-To suppress these warnings, you can use the following code:
+To suppress these warnings, you can use the following to disable such warnings from being emitted by this package:
 
 ```python
-import urllib3
+from vcx_py import STOP_URLLIB_INSECURE_WARN
 
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-```
-
-or you can use the environment variable `PYTHONWARNINGS` to suppress the warnings:
-
-```bash
-export PYTHONWARNINGS="ignore:Unverified HTTPS request"
+STOP_URLLIB_INSECURE_WARN.set()
 ```
 
 ## Paused Trading
 
 It is possible that trading on the exchange is paused. Unfortunately, the client does not have a way to check
 if trading is paused and thus `KeyError` exceptions may be raised when attempting to access keys from the API which
 are omitted in such cases. Eventually we hope to have an endpoint which will allow us to check if trading is paused.
```

### Comparing `vcx_py-1.1.4/README.md` & `vcx_py-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -141,26 +141,20 @@
 ```
 
 ## Warnings
 
 Note that due to CloudFlare protection, this version of the client attempts to access the API through its
 IP address and not the domain name. Should the IP address change, the client will need to be updated.
 Moreover, you will receive `InsecureRequestWarning` warnings when using the client until this issue is resolved.
-To suppress these warnings, you can use the following code:
+To suppress these warnings, you can use the following to disable such warnings from being emitted by this package:
 
 ```python
-import urllib3
+from vcx_py import STOP_URLLIB_INSECURE_WARN
 
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-```
-
-or you can use the environment variable `PYTHONWARNINGS` to suppress the warnings:
-
-```bash
-export PYTHONWARNINGS="ignore:Unverified HTTPS request"
+STOP_URLLIB_INSECURE_WARN.set()
 ```
 
 ## Paused Trading
 
 It is possible that trading on the exchange is paused. Unfortunately, the client does not have a way to check
 if trading is paused and thus `KeyError` exceptions may be raised when attempting to access keys from the API which
 are omitted in such cases. Eventually we hope to have an endpoint which will allow us to check if trading is paused.
```

### Comparing `vcx_py-1.1.4/setup.py` & `vcx_py-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from setuptools import setup
 
 setup(
     name='vcx_py',
-    version='1.1.4',
+    version='1.2.0',
     packages=['vcx_py'],
     license='MIT',
     author='Aaron Janeiro Stone',
     author_email='aaron@thequant.ca',
     description='A simple python client for the VirgoCX API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `vcx_py-1.1.4/vcx_py/__init__.py` & `vcx_py-1.2.0/vcx_py/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,11 +4,12 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from .client import VirgoCXClient
-from .constants import KLineType, OrderStatus, OrderType, OrderDirection, Enums
+from .constants import KLineType, OrderStatus, OrderType, OrderDirection, Enums, STOP_URLLIB_INSECURE_WARN
 from .utils import VirgoCXException
 
-__all__ = ["VirgoCXClient", "VirgoCXException", "KLineType", "OrderStatus", "OrderType", "OrderDirection", "Enums"]
+__all__ = ["VirgoCXClient", "VirgoCXException", "KLineType", "OrderStatus", "OrderType", "OrderDirection", "Enums",
+           "STOP_URLLIB_INSECURE_WARN"]
```

### Comparing `vcx_py-1.1.4/vcx_py/client.py` & `vcx_py-1.2.0/vcx_py/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from threading import Lock
 from warnings import warn
 
 import requests as rq
 
 from .constants import ROOT_ADDRESS, VERIFICATION, KLineType, OrderStatus, \
     OrderType, OrderDirection
-from .utils import VirgoCXWarning, VirgoCXException, vcx_sign, result_formatter
+from .utils import VirgoCXWarning, VirgoCXException, vcx_sign, result_formatter, maybe_suppress_insecure
 
 
 class VirgoCXClient:
     """
     A simple python client for the VirgoCX API.
     """
     FMT_DATA = None  # created by first instance
@@ -40,52 +40,57 @@
         with VirgoCXClient.STATIC_LOCK:
             if VirgoCXClient.FMT_DATA is None:
                 VirgoCXClient.FMT_DATA = {v["symbol"]: {"price_decimals": v["priceDecimals"],
                                                         "qty_decimals": v["qtyDecimals"],
                                                         "min_total": v["minTotal"]} for v in
                                           self.tickers()}
 
+    @maybe_suppress_insecure
     @result_formatter()
     def kline(self, symbol: str, period: KLineType):
         """
         Returns the kline data for a given symbol and period.
 
         :param symbol: The symbol to query.
         :param period: How the kline data should be aggregated.
         """
         if isinstance(period, KLineType):
             period = period.value
         return rq.get(f"{self.ENDPOINT}/market/history/kline", params={"symbol": symbol, "period": period},
                       verify=VERIFICATION)
 
+    @maybe_suppress_insecure
     @result_formatter()
     def ticker(self, symbol: str):
         """
         Returns the ticker data for a given symbol.
 
         :param symbol: The symbol to query.
         """
         return rq.get(f"{self.ENDPOINT}/market/detail/merged", params={"symbol": symbol}, verify=VERIFICATION)
 
+    @maybe_suppress_insecure
     @result_formatter()
     def tickers(self):
         """
         Returns the ticker data for all symbols.
         """
         return rq.get(f"{self.ENDPOINT}/market/tickers", verify=VERIFICATION)
 
+    @maybe_suppress_insecure
     @result_formatter()
     def account_info(self):
         """
         Returns the account information.
         """
         payload = {"apiKey": self._api_key()}
         payload["sign"] = self.signer(payload)
         return rq.get(f"{self.ENDPOINT}/member/accounts", params=payload, verify=VERIFICATION)
 
+    @maybe_suppress_insecure
     @result_formatter()
     def query_orders(self, symbol: str, status: Optional[OrderStatus] = None):
         """
         Returns user orders for a given symbol and status.
 
         :param symbol: The symbol to query.
         :param status: Restrict the query to this specific status (optional).
@@ -94,25 +99,27 @@
         if status is not None:
             if isinstance(status, OrderStatus):
                 status = status.value
             payload["status"] = status
         payload["sign"] = self.signer(payload)
         return rq.get(f"{self.ENDPOINT}/member/queryOrder", params=payload, verify=VERIFICATION)
 
+    @maybe_suppress_insecure
     @result_formatter(False)
     def query_trades(self, symbol: str):
         """
         Returns (completed) user trades for a given symbol.
 
         :param symbol: The symbol to query.
         """
         payload = {"apiKey": self._api_key(), "symbol": symbol}
         payload["sign"] = self.signer(payload)
         return rq.get(f"{self.ENDPOINT}/member/queryTrade", params=payload, verify=VERIFICATION)
 
+    @maybe_suppress_insecure
     @result_formatter()
     def place_order(self, symbol: str, category: OrderType, direction: OrderDirection,
                     price: Optional[float] = None, qty: Optional[float] = None,
                     total: Optional[float] = None, handle_conversions: bool = True,
                     **kwargs):
         """
         Places an order.
@@ -209,25 +216,27 @@
         market_price = self.get_discount(symbol=symbol)[0]
         if direction == OrderDirection.BUY:
             market_price = float(market_price["Ask"])
         else:
             market_price = float(market_price["Bid"])
         return market_price
 
+    @maybe_suppress_insecure
     @result_formatter()
     def cancel_order(self, order_id: str):
         """
         Cancels an order.
 
         :param order_id: The ID of the order to cancel.
         """
         payload = {"apiKey": self._api_key(), "id": order_id}
         payload["sign"] = self.signer(payload)
         return rq.post(f"{self.ENDPOINT}/member/cancelOrder", data=payload, verify=VERIFICATION)
 
+    @maybe_suppress_insecure
     @result_formatter()
     def get_discount(self, symbol: Optional[str] = None):
         """
         Returns similar output as `ticker` for a given symbol (or all symbols if one is not provided) with
         your account discount applied to prices.
 
         Note that this method always returns a list of dictionaries, even if only one symbol is queried.
```

### Comparing `vcx_py-1.1.4/vcx_py/constants.py` & `vcx_py-1.2.0/vcx_py/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,48 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from enum import IntEnum
 
+
+class _Flag:
+    """A simple flag class."""
+
+    def __init__(self, value):
+        self._value = value
+
+    def set(self):
+        self._value = True
+
+    def unset(self):
+        self._value = False
+
+    def __bool__(self):
+        return self._value
+
+
 # Because CloudFlare is may block when accessed via the domain name, the IP address is used instead for now.
 ROOT_ADDRESS = "https://3.98.238.66/api"
 """The root address of the VirgoCX API."""
 
 # Once the CloudFlare issue is resolved, the domain name will be used instead of the IP and the following
 # can be set to True.
-VERIFICATION = False
-"""Whether or not to verify the SSL certificate of the VirgoCX API."""
+VERIFICATION = _Flag(False)
+"""
+Whether to verify the SSL certificate of the VirgoCX API.
+Use the `.set()` method to activate this feature.
+"""
+
+STOP_URLLIB_INSECURE_WARN = _Flag(False)
+"""
+Whether to suppress the urllib3 InsecureRequestWarning warning within this package.
+Use the `.set()` method to activate this feature.
+"""
 
 
 class KLineType(IntEnum):
     """
     Enum for the type of kline.
     """
     MINUTE = 1
```

### Comparing `vcx_py-1.1.4/vcx_py/schema.py` & `vcx_py-1.2.0/vcx_py/schema.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.4/vcx_py/utils.py` & `vcx_py-1.2.0/vcx_py/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,16 +5,36 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from hashlib import md5
 from typing import Union
+import warnings
 
-from vcx_py.constants import TYPICAL_KEY_TO_ENUM, ATYPICAL_KEY_TO_ENUM
+import urllib3 as url  # noqa (already comes with requests)
+
+from vcx_py.constants import TYPICAL_KEY_TO_ENUM, ATYPICAL_KEY_TO_ENUM, STOP_URLLIB_INSECURE_WARN
+
+
+def maybe_suppress_insecure(fn: callable) -> callable:
+    """
+    Potentially suppresses urllib3 InsecureRequestWarning warnings.
+
+    This only suppresses the warning within the context of this package.
+    """
+
+    def inner(*args, **kwargs):
+        if STOP_URLLIB_INSECURE_WARN:
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", url.exceptions.InsecureRequestWarning)
+                return fn(*args, **kwargs)
+        return fn(*args, **kwargs)
+
+    return inner
 
 
 class VirgoCXWarning(Warning):
     """
     Base warning for the VirgoCX API.
     """
     pass  # overrides allow for optional fine-grained control
```

### Comparing `vcx_py-1.1.4/vcx_py.egg-info/PKG-INFO` & `vcx_py-1.2.0/vcx_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcx_py
-Version: 1.1.4
+Version: 1.2.0
 Summary: A simple python client for the VirgoCX API
 Home-page: https://www.github.com/aarjaneiro/vcx_py
 Author: Aaron Janeiro Stone
 Author-email: aaron@thequant.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -152,26 +152,20 @@
 ```
 
 ## Warnings
 
 Note that due to CloudFlare protection, this version of the client attempts to access the API through its
 IP address and not the domain name. Should the IP address change, the client will need to be updated.
 Moreover, you will receive `InsecureRequestWarning` warnings when using the client until this issue is resolved.
-To suppress these warnings, you can use the following code:
+To suppress these warnings, you can use the following to disable such warnings from being emitted by this package:
 
 ```python
-import urllib3
+from vcx_py import STOP_URLLIB_INSECURE_WARN
 
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-```
-
-or you can use the environment variable `PYTHONWARNINGS` to suppress the warnings:
-
-```bash
-export PYTHONWARNINGS="ignore:Unverified HTTPS request"
+STOP_URLLIB_INSECURE_WARN.set()
 ```
 
 ## Paused Trading
 
 It is possible that trading on the exchange is paused. Unfortunately, the client does not have a way to check
 if trading is paused and thus `KeyError` exceptions may be raised when attempting to access keys from the API which
 are omitted in such cases. Eventually we hope to have an endpoint which will allow us to check if trading is paused.
```

