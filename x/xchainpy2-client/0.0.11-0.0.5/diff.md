# Comparing `tmp/xchainpy2_client-0.0.11.tar.gz` & `tmp/xchainpy2_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2_client-0.0.11.tar", last modified: Thu Apr  4 13:59:54 2024, max compression
+gzip compressed data, was "xchainpy2_client-0.0.5.tar", last modified: Wed Jan  3 16:34:26 2024, max compression
```

## Comparing `xchainpy2_client-0.0.11.tar` & `xchainpy2_client-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-04 13:59:54.237565 xchainpy2_client-0.0.11/
--rw-r--r--   0 tirinox    (501) staff       (20)     1086 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)     1552 2024-04-04 13:59:54.237360 xchainpy2_client-0.0.11/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)      466 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)     1343 2024-04-04 13:59:30.000000 xchainpy2_client-0.0.11/pyproject.toml
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-04-04 13:59:54.237606 xchainpy2_client-0.0.11/setup.cfg
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-04 13:59:54.235509 xchainpy2_client-0.0.11/xchainpy2_client/
--rw-r--r--   0 tirinox    (501) staff       (20)      100 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/xchainpy2_client/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10927 2024-04-04 13:59:30.000000 xchainpy2_client-0.0.11/xchainpy2_client/base_client.py
--rw-r--r--   0 tirinox    (501) staff       (20)      365 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/xchainpy2_client/explorer.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1983 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/xchainpy2_client/fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4772 2024-04-04 11:45:55.000000 xchainpy2_client-0.0.11/xchainpy2_client/models.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-04 13:59:54.236817 xchainpy2_client-0.0.11/xchainpy2_client/test/
--rw-r--r--   0 tirinox    (501) staff       (20)     2102 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/xchainpy2_client/test/mocks.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1500 2024-04-04 11:45:55.000000 xchainpy2_client-0.0.11/xchainpy2_client/test/test_async.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1543 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/xchainpy2_client/test/test_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1410 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/xchainpy2_client/test/test_gas_amount.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5537 2024-03-07 10:37:31.000000 xchainpy2_client-0.0.11/xchainpy2_client/utxo_client.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-04 13:59:54.236986 xchainpy2_client-0.0.11/xchainpy2_client.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)     1552 2024-04-04 13:59:54.000000 xchainpy2_client-0.0.11/xchainpy2_client.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)      548 2024-04-04 13:59:54.000000 xchainpy2_client-0.0.11/xchainpy2_client.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-04-04 13:59:54.000000 xchainpy2_client-0.0.11/xchainpy2_client.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       96 2024-04-04 13:59:54.000000 xchainpy2_client-0.0.11/xchainpy2_client.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       17 2024-04-04 13:59:54.000000 xchainpy2_client-0.0.11/xchainpy2_client.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:34:26.870634 xchainpy2_client-0.0.5/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1086 2023-04-22 16:09:04.000000 xchainpy2_client-0.0.5/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)     1551 2024-01-03 16:34:26.870406 xchainpy2_client-0.0.5/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)      466 2023-05-28 08:08:39.000000 xchainpy2_client-0.0.5/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)     1342 2023-10-09 09:19:57.000000 xchainpy2_client-0.0.5/pyproject.toml
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-01-03 16:34:26.870679 xchainpy2_client-0.0.5/setup.cfg
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:34:26.868717 xchainpy2_client-0.0.5/xchainpy2_client/
+-rw-r--r--   0 tirinox    (501) staff       (20)      100 2023-05-27 07:59:00.000000 xchainpy2_client-0.0.5/xchainpy2_client/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8680 2023-12-30 06:30:04.000000 xchainpy2_client-0.0.5/xchainpy2_client/base_client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      365 2023-07-14 19:19:50.000000 xchainpy2_client-0.0.5/xchainpy2_client/explorer.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2206 2023-10-08 16:10:05.000000 xchainpy2_client-0.0.5/xchainpy2_client/fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4203 2023-12-21 19:23:01.000000 xchainpy2_client-0.0.5/xchainpy2_client/models.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:34:26.869670 xchainpy2_client-0.0.5/xchainpy2_client/test/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1543 2023-07-14 17:45:02.000000 xchainpy2_client-0.0.5/xchainpy2_client/test/test_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5537 2023-12-05 13:30:57.000000 xchainpy2_client-0.0.5/xchainpy2_client/utxo_client.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:34:26.869970 xchainpy2_client-0.0.5/xchainpy2_client.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1551 2024-01-03 16:34:26.000000 xchainpy2_client-0.0.5/xchainpy2_client.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)      440 2024-01-03 16:34:26.000000 xchainpy2_client-0.0.5/xchainpy2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-01-03 16:34:26.000000 xchainpy2_client-0.0.5/xchainpy2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       96 2024-01-03 16:34:26.000000 xchainpy2_client-0.0.5/xchainpy2_client.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       17 2024-01-03 16:34:26.000000 xchainpy2_client-0.0.5/xchainpy2_client.egg-info/top_level.txt
```

### Comparing `xchainpy2_client-0.0.11/LICENSE` & `xchainpy2_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xchainpy2_client-0.0.11/PKG-INFO` & `xchainpy2_client-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_client
-Version: 0.0.11
+Version: 0.0.5
 Summary: XChainPy2 Base Clients
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xchainpy2_client-0.0.11/pyproject.toml` & `xchainpy2_client-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchainpy2_client"
-version = "0.0.11"
+version = "0.0.5"
 authors = [
     { name = "Tirinox", email = "developer@tirinox.ru" },
 ]
 description = "XChainPy2 Base Clients"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["Crypto", "THORChain", "Blockchain", "XChain"]
```

### Comparing `xchainpy2_client-0.0.11/xchainpy2_client/base_client.py` & `xchainpy2_client-0.0.5/xchainpy2_client/base_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import abc
-import asyncio
 from datetime import datetime
 from decimal import Decimal
 from typing import Optional, List, Union
 
 from xchainpy2_client.explorer import ExplorerProvider
 from xchainpy2_client.models import XcTx, Fees, TxPage, \
-    FeeBounds, RootDerivationPaths, AssetInfo, FeeOption
+    FeeBounds, Fee, RootDerivationPaths, AssetInfo, FeeOption
 from xchainpy2_crypto import validate_mnemonic, derive_private_key
 from xchainpy2_utils import CryptoAmount, Chain, NetworkType, Asset, Amount
 
+INF_FEE = Fee(1_000_000_000_000_000_000)
+
 
 class KeyException(Exception):
     ...
 
 
 class XChainClient(abc.ABC):
     def __init__(self,
                  chain: Chain,
                  network: Optional[NetworkType] = None,
                  phrase: Optional[str] = None,
                  private_key: Union[str, bytes, callable, None] = None,
-                 fee_bound: Optional[FeeBounds] = None,
+                 fee_bound: FeeBounds = FeeBounds(lower=Fee(0), upper=INF_FEE),
                  root_derivation_paths: Optional[RootDerivationPaths] = None,
                  wallet_index=0,
                  ):
         """
         Client has to be initialised with network type and phrase.
         It will throw an error if an invalid phrase has been passed.
 
@@ -36,15 +37,15 @@
         :param fee_bound: Fee bounds
         :param root_derivation_paths: Root derivation paths for private key for each Network type
         :param wallet_index: int (wallet index, default 0) We can derive any number of addresses from a single seed
         """
         self.wallet_index = wallet_index
         self.chain = chain
 
-        self.fee_bound = fee_bound or FeeBounds.infinite()
+        self.fee_bound = fee_bound
         self.root_derivation_paths = root_derivation_paths
 
         self.network = network
         self.set_network(network)
 
         self.explorers = {network: ExplorerProvider('', '', '')}
 
@@ -108,65 +109,41 @@
         elif isinstance(self._private_key, str):
             return self._private_key
         elif isinstance(self._private_key, bytes):
             return self._private_key.hex()
         else:
             return None
 
-    def gas_amount(self, amount: Union[float, str, int, Decimal, Amount]) -> CryptoAmount:
+    def gas_amount(self, amount: Union[float, str, int, Decimal]) -> CryptoAmount:
         """
         Easy way to construct CryptoAmount of gas asset
-        Type int means base amount (like satoshi, wei, 1e-8 rune, etc)
-        Types float and Decimal means asset amount (like btc, eth, rune, etc)
         :param amount: Union[float, str, int, Decimal] amount of asset (not base!)
         :return: CryptoAmount
         """
         return CryptoAmount(Amount.automatic(amount, self._decimal), self._gas_asset)
 
-    def gas_base_amount(self, amount: int) -> CryptoAmount:
-        """
-        Easy way to construct CryptoAmount of gas asset from base units
-        :param amount: base amount of asset (like satoshi, wei, 1e-8 rune, etc); must be int type
-        :return:
-        """
-        assert isinstance(amount, int)
-        return CryptoAmount(Amount.from_base(amount, self._decimal), self._gas_asset)
-
-    def gas_asset_amount(self, amount: Union[float, str, Decimal]) -> CryptoAmount:
-        """
-        Easy way to construct CryptoAmount of gas asset from asset units
-        :param amount: asset amount (like btc, eth, rune, etc); must be float or Decimal type or str
-        :return:
-        """
-        assert isinstance(amount, (float, str, Decimal))
-        return CryptoAmount(Amount.from_asset(amount, self._decimal), self._gas_asset)
-
-    @property
-    def zero_gas_amount(self) -> CryptoAmount:
-        return self.gas_base_amount(0)
-
     async def max_gas_amount(self, balances: List[CryptoAmount] = None) -> CryptoAmount:
         """
-        Calculate maximum amount of Gas asset that you can send to empty your wallet
+        Calculate maximum amount of Gas asset that you can send
         :param balances: (Optional) if you already have your balance, otherwise they will be loaded
         :return: CryptoAmount
         """
         if balances is None:
             balances = await self.get_balance()
 
         gas_balance = next((b for b in balances if b.asset == self._gas_asset), None)
         if not gas_balance:
-            return self.zero_gas_amount  # no gas at all
+            return self.gas_amount(0)  # no gas at all
 
         fees = await self.get_fees()
         fee = fees.fees[FeeOption.FAST]
         max_value = gas_balance.amount.as_asset - fee.as_asset
         if max_value.internal_amount < 0:
             # less than fee
-            return self.zero_gas_amount
+            return self.gas_amount(0)
         else:
             return CryptoAmount(max_value, self._gas_asset)
 
     def set_network(self, network: NetworkType):
         if not network:
             network = NetworkType.MAINNET
         self.network = network
@@ -214,38 +191,14 @@
         """
         return self.explorers[self.network].get_tx_url(tx_id)
 
     @abc.abstractmethod
     async def get_balance(self, address: str = '') -> List[CryptoAmount]:
         pass
 
-    async def get_gas_balance(self, address: str = '') -> CryptoAmount:
-        """
-        Get the balance of the gas asset for the given address
-        :param address: address (optional)
-        :return: CryptoAmount of the gas asset
-        """
-        balances = await self.get_balance(address)
-        gas_balance = next((b for b in balances if b.asset == self._gas_asset), None)
-        if not gas_balance:
-            return self.zero_gas_amount
-        return gas_balance
-
-    async def has_balance(self, amount: CryptoAmount):
-        """
-        Check if the wallet has enough balance to send the given amount
-        :param amount: amount to send
-        :return: True if the wallet has enough balance, False otherwise
-        """
-        balances = await self.get_balance()
-        balance = next((b for b in balances if b.asset == amount.asset), None)
-        if not balance:
-            return False
-        return balance.amount >= amount.amount
-
     def get_full_derivation_path(self, wallet_index: int) -> str:
         if self.root_derivation_paths:
             # BREAKING CHANGE!
             # return f"{self.root_derivation_paths[self.network]}{wallet_index}'"  # original with apostrophe
             return f"{self.root_derivation_paths[self.network]}{wallet_index}"
         return ''
 
@@ -293,18 +246,10 @@
 
     def get_last_response(self, txid: str):
         return self.last_response_dict.get(txid)
 
     def clear_last_responses(self):
         self.last_response_dict = {}
 
-    @staticmethod
-    async def _call_service(method, *args):
-        return await asyncio.get_event_loop().run_in_executor(
-            None,
-            method,
-            *args
-        )
-
 
 class NoClient(XChainClient, abc.ABC):
     ...
```

### Comparing `xchainpy2_client-0.0.11/xchainpy2_client/fees.py` & `xchainpy2_client-0.0.5/xchainpy2_client/fees.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,7 +67,12 @@
         for k, fee in zip(fee_rates.keys(), all_fees)
     }
 
     return Fees(
         fees=fees,
         type=FeeType.PER_BYTE
     )
+
+
+def check_fee_bounds(fee_bounds: FeeBounds, fee_rate: FeeRate) -> None:
+    if fee_rate < fee_bounds.lower or fee_rate > fee_bounds.upper:
+        raise ValueError(f"Fee outside of predetermined bounds: {str(fee_rate)}")
```

### Comparing `xchainpy2_client-0.0.11/xchainpy2_client/models.py` & `xchainpy2_client-0.0.5/xchainpy2_client/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -80,48 +80,34 @@
 
 class FeeType(Enum):
     FLAT_FEE = 'base'
     PER_BYTE = 'byte'
 
 
 Fee = Amount
-FeeRate = float  # satoshi per kilobyte in Bitcoin and other UTXO chains
-
-INF_FEE = Fee(1_000_000_000_000_000_000)
+FeeRate = float
 
 
 class Fees(NamedTuple):
     type: FeeType
     fees: Dict[FeeOption, Fee]
 
 
 class FeesWithRates(NamedTuple):
     fees: Fees
     rates: FeeRates
 
 
 class FeeBounds(NamedTuple):
-    lower: FeeRate  # satoshi per byte
-    upper: FeeRate  # satoshi per byte
-
-    def check_fee_bounds(self, fee_rate: FeeRate, per_kb: bool = False):
-        """
-        Check if the given fee rate is within the bounds
-        :param fee_rate: fee rate to check, in satoshi per byte
-        :param per_kb: if True, the fee rate is in satoshi per kilobyte. Otherwise, it is in satoshi per byte
-        """
-        if per_kb:
-            fee_rate /= 1000
+    lower: Fee
+    upper: Fee
 
+    def check_fee_bounds(self, fee_rate: FeeRate):
         if fee_rate < self.lower or fee_rate > self.upper:
-            raise ValueError(f"Fee outside of predetermined bounds: {fee_rate}")
-
-    @classmethod
-    def infinite(cls):
-        return FeeBounds(lower=Fee(0), upper=INF_FEE)
+            raise Exception(f"Fee outside of predetermined bounds: {fee_rate}")
 
 
 RootDerivationPaths = Dict[NetworkType, str]
 
 
 class XChainClientParams(NamedTuple):
     network: Optional[NetworkType] = None
```

### Comparing `xchainpy2_client-0.0.11/xchainpy2_client/test/test_fees.py` & `xchainpy2_client-0.0.5/xchainpy2_client/test/test_fees.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_client-0.0.11/xchainpy2_client/utxo_client.py` & `xchainpy2_client-0.0.5/xchainpy2_client/utxo_client.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_client-0.0.11/xchainpy2_client.egg-info/PKG-INFO` & `xchainpy2_client-0.0.5/xchainpy2_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_client
-Version: 0.0.11
+Version: 0.0.5
 Summary: XChainPy2 Base Clients
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

