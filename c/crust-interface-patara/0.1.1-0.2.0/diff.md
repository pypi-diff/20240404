# Comparing `tmp/crust_interface_patara-0.1.1.tar.gz` & `tmp/crust_interface_patara-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crust_interface_patara-0.1.1.tar", max compression
+gzip compressed data, was "crust_interface_patara-0.2.0.tar", max compression
```

## Comparing `crust_interface_patara-0.1.1.tar` & `crust_interface_patara-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11343 2023-01-31 12:08:54.155146 crust_interface_patara-0.1.1/LICENSE
--rw-r--r--   0        0        0     1862 2023-02-01 08:17:08.712936 crust_interface_patara-0.1.1/README.md
--rw-r--r--   0        0        0       79 2023-01-31 11:36:19.494054 crust_interface_patara-0.1.1/crustinterface/__init__.py
--rw-r--r--   0        0        0     3391 2023-01-31 11:36:19.494054 crust_interface_patara-0.1.1/crustinterface/base.py
--rw-r--r--   0        0        0      233 2023-01-31 11:51:28.443724 crust_interface_patara-0.1.1/crustinterface/constants.py
--rw-r--r--   0        0        0     1744 2023-01-31 11:36:19.494054 crust_interface_patara-0.1.1/crustinterface/decorators.py
--rw-r--r--   0        0        0     2690 2023-01-31 11:36:19.494054 crust_interface_patara-0.1.1/crustinterface/mainnet.py
--rw-r--r--   0        0        0     1313 2023-01-31 11:36:19.494054 crust_interface_patara-0.1.1/crustinterface/shadow.py
--rw-r--r--   0        0        0     1305 2023-02-01 08:17:45.551835 crust_interface_patara-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 crust_interface_patara-0.1.1/setup.py
--rw-r--r--   0        0        0     3194 1970-01-01 00:00:00.000000 crust_interface_patara-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-04 16:40:51.937622 crust_interface_patara-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2648 2024-04-04 17:11:47.353823 crust_interface_patara-0.2.0/README.md
+-rw-r--r--   0        0        0      112 2024-04-04 17:11:47.365822 crust_interface_patara-0.2.0/crustinterface/__init__.py
+-rw-r--r--   0        0        0     3387 2024-04-04 16:59:06.687647 crust_interface_patara-0.2.0/crustinterface/base.py
+-rw-r--r--   0        0        0      235 2024-04-04 16:59:38.379810 crust_interface_patara-0.2.0/crustinterface/constants.py
+-rw-r--r--   0        0        0     1736 2024-04-04 16:59:06.695647 crust_interface_patara-0.2.0/crustinterface/decorators.py
+-rw-r--r--   0        0        0     2690 2024-04-04 16:40:51.937622 crust_interface_patara-0.2.0/crustinterface/mainnet.py
+-rw-r--r--   0        0        0     1318 2024-04-04 17:07:48.929424 crust_interface_patara-0.2.0/crustinterface/parachain.py
+-rw-r--r--   0        0        0     1313 2024-04-04 16:40:51.937622 crust_interface_patara-0.2.0/crustinterface/shadow.py
+-rw-r--r--   0        0        0     1347 2024-04-04 17:25:32.194457 crust_interface_patara-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 crust_interface_patara-0.2.0/setup.py
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 crust_interface_patara-0.2.0/PKG-INFO
```

### Comparing `crust_interface_patara-0.1.1/LICENSE` & `crust_interface_patara-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crust_interface_patara-0.1.1/README.md` & `crust_interface_patara-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 
 `Mainnet` provides Crust interaction functionality to check user balance, calculate file storage price, placing
 file storage order, add tokens to renewal pool and checking replicas count.
 
 ```python
 import time
 from crustinterface import Mainnet
+from substrateinterface import KeypairType
 
 seed = "seed"
-mainnet = Mainnet(seed=seed)
+mainnet = Mainnet(seed=seed, crypto_type=KeypairType.SR25519)
 
 # get any IPFS CID and size
 cid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>
 
 # Check balance
 balance = mainnet.get_balance()
 print(balance)
@@ -53,23 +54,47 @@
 print(replicas)
 
 ```
 
 `Shadow` allows you to perform `Xstorage` extrinsic in Crust Shadow network.
 ```python
 from crustinterface import Shadow
+from substrateinterface import KeypairType
+
 seed = "seed"
-shadow = Shadow(seed=seed)
+shadow = Shadow(seed=seed, crypto_type=KeypairType.SR25519)
 
 # get any IPFS CID and size
 cid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>
 
 print(cid, size)
 
 # Check balance
 balance = shadow.get_balance()
 print(balance)
 
 # Store file in Shadow for CSMs
 file_stored = shadow.store_file(cid, size)
 print(file_stored)
 ```
+
+`Parachain` allows you to perform `Xstorage` extrinsic in Crust Polkadot Parachain network.
+```python
+from crustinterface import Parachain
+from substrateinterface import KeypairType
+
+seed = "seed"
+parachain = Parachain(seed=seed, crypto_type=KeypairType.SR25519)
+
+# get any IPFS CID and size
+cid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>
+
+print(cid, size)
+
+# Check balance
+balance = parachain.get_balance()
+print(balance)
+
+# Store file in Shadow for CSMs
+file_stored = parachain.store_file(cid, size)
+print(file_stored)
+```
```

### Comparing `crust_interface_patara-0.1.1/crustinterface/base.py` & `crust_interface_patara-0.2.0/crustinterface/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as tp
 
 from substrateinterface import SubstrateInterface, Keypair, KeypairType
 
-from .constants import CRUST_SS_58_FORMAT, CRUST_MAINNET_ENDPOINT, CRUST_SHADOW_ENDPOINT, CRUST_ROCKY_TESTNET_ENDPOINT
+from .constants import CRUST_SS_58_FORMAT, CRUST_MAINNET_ENDPOINT, CRUST_SHADOW_ENDPOINT, CRUST_PARACHAIN_ENDPOINT
 from .decorators import check_interface_opened
 
 
 class Base:
     """
     Base class with basic functionality for Crust interfaces
     """
@@ -26,16 +26,16 @@
         else:
             self.keypair = None
 
         if chain == "shadow":
             self.remote_ws = CRUST_SHADOW_ENDPOINT
         elif chain == "mainnet":
             self.remote_ws = CRUST_MAINNET_ENDPOINT
-        elif chain == "rocky":
-            self.remote_ws = CRUST_ROCKY_TESTNET_ENDPOINT
+        elif chain == "parachain":
+            self.remote_ws = CRUST_PARACHAIN_ENDPOINT
         else:
             raise ValueError("Invalid chain name. Choose from [shadow, mainnet, rocky].")
 
         self.interface: tp.Optional[SubstrateInterface] = None
 
     @staticmethod
     def create_keypair(seed: str, crypto_type: int = KeypairType.SR25519) -> Keypair:
```

### Comparing `crust_interface_patara-0.1.1/crustinterface/decorators.py` & `crust_interface_patara-0.2.0/crustinterface/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from functools import wraps
 from websocket._exceptions import WebSocketConnectionClosedException
 
 from .constants import (
     CRUST_SS_58_FORMAT,
     CRUST_TYPE_REGISTRY_PRESET,
     CRUST_MAINNET_ENDPOINT,
-    CRUST_ROCKY_TESTNET_ENDPOINT,
+    CRUST_PARACHAIN_ENDPOINT,
 )
 
 
 def check_interface_opened(func):
     """
     Open substrate node connection each time needed.
 
@@ -59,10 +59,10 @@
 
     """
 
     interface_instance.interface = substrate.SubstrateInterface(
         url=interface_instance.remote_ws,
         ss58_format=CRUST_SS_58_FORMAT,
         type_registry_preset=CRUST_TYPE_REGISTRY_PRESET
-        if interface_instance.remote_ws in [CRUST_MAINNET_ENDPOINT, CRUST_ROCKY_TESTNET_ENDPOINT]
+        if interface_instance.remote_ws in [CRUST_MAINNET_ENDPOINT, CRUST_PARACHAIN_ENDPOINT]
         else None
     )
```

### Comparing `crust_interface_patara-0.1.1/crustinterface/mainnet.py` & `crust_interface_patara-0.2.0/crustinterface/mainnet.py`

 * *Files identical despite different names*

### Comparing `crust_interface_patara-0.1.1/crustinterface/shadow.py` & `crust_interface_patara-0.2.0/crustinterface/shadow.py`

 * *Files identical despite different names*

### Comparing `crust_interface_patara-0.1.1/pyproject.toml` & `crust_interface_patara-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "crust-interface-patara"
-version = "0.1.1"
-description = "A simple tool to interact with Crust Shadow and Crust Mainnet. Under development"
+version = "0.2.0"
+description = "A simple tool to interact with Crust Shadow, Crust Polkadot Parachain and Crust Mainnet. Under development"
 authors = ["PaTara43 <p040399@outlook.com>"]
 license = "Apache-2.0"
 
 homepage = "https://github.com/PaTara43/crust-interface-patara"
 repository = "https://github.com/PaTara43/crust-interface-patara"
 documentation = "https://github.com/PaTara43/crust-interface-patara/blob/main/README.md"
 
@@ -13,15 +13,16 @@
 
 keywords = [
     "python",
     "ipfs",
     "web3",
     "substrate",
     "crust",
-    "pypi-package"
+    "pypi-package",
+    "polkadot"
 ]
 
 classifiers = [
     "Operating System :: Unix",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Topic :: Software Development :: Documentation",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `crust_interface_patara-0.1.1/setup.py` & `crust_interface_patara-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['substrate-interface>=1.4.0,<2.0']
 
 setup_kwargs = {
     'name': 'crust-interface-patara',
-    'version': '0.1.1',
-    'description': 'A simple tool to interact with Crust Shadow and Crust Mainnet. Under development',
-    'long_description': '# crust-file-uploader\n\nhttps://crust.network/\nhttps://apps.crust.network/\nhttps://wiki.crust.network/en\nhttps://polkadot.js.org/apps/?rpc=wss%3A%2F%2Frpc-shadow.crust.network%2F#/explorer\n\nThis is a simple tool to pin your files sing Crust Network or Crust Shadow.\n\n## Setup\n### Installation:\n```bash\npip3 install crust-interface-patara\n```\n\n## Features\n\nThe module is divided into `Mainnet` and `Shadow`\n\n`Mainnet` provides Crust interaction functionality to check user balance, calculate file storage price, placing\nfile storage order, add tokens to renewal pool and checking replicas count.\n\n```python\nimport time\nfrom crustinterface import Mainnet\n\nseed = "seed"\nmainnet = Mainnet(seed=seed)\n\n# get any IPFS CID and size\ncid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>\n\n# Check balance\nbalance = mainnet.get_balance()\nprint(balance)\n\n# Check price in Main net. Price in pCRUs\nprice = mainnet.get_appx_store_price(int(size))\nprint(price)\n\n# Store file in Mainnet for CRUs\nfile_stored = mainnet.store_file(cid, size)\nprint(file_stored)\n\n# Add renewal pool\nfile_prepaid = mainnet.add_renewal_pool_balance(cid, price*2)\nprint(file_prepaid)\n\n\n# Get replicas\ntime.sleep(10)\nreplicas = mainnet.get_replicas(cid)\nprint(replicas)\n\n```\n\n`Shadow` allows you to perform `Xstorage` extrinsic in Crust Shadow network.\n```python\nfrom crustinterface import Shadow\nseed = "seed"\nshadow = Shadow(seed=seed)\n\n# get any IPFS CID and size\ncid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>\n\nprint(cid, size)\n\n# Check balance\nbalance = shadow.get_balance()\nprint(balance)\n\n# Store file in Shadow for CSMs\nfile_stored = shadow.store_file(cid, size)\nprint(file_stored)\n```\n',
+    'version': '0.2.0',
+    'description': 'A simple tool to interact with Crust Shadow, Crust Polkadot Parachain and Crust Mainnet. Under development',
+    'long_description': '# crust-file-uploader\n\nhttps://crust.network/\nhttps://apps.crust.network/\nhttps://wiki.crust.network/en\nhttps://polkadot.js.org/apps/?rpc=wss%3A%2F%2Frpc-shadow.crust.network%2F#/explorer\n\nThis is a simple tool to pin your files sing Crust Network or Crust Shadow.\n\n## Setup\n### Installation:\n```bash\npip3 install crust-interface-patara\n```\n\n## Features\n\nThe module is divided into `Mainnet` and `Shadow`\n\n`Mainnet` provides Crust interaction functionality to check user balance, calculate file storage price, placing\nfile storage order, add tokens to renewal pool and checking replicas count.\n\n```python\nimport time\nfrom crustinterface import Mainnet\nfrom substrateinterface import KeypairType\n\nseed = "seed"\nmainnet = Mainnet(seed=seed, crypto_type=KeypairType.SR25519)\n\n# get any IPFS CID and size\ncid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>\n\n# Check balance\nbalance = mainnet.get_balance()\nprint(balance)\n\n# Check price in Main net. Price in pCRUs\nprice = mainnet.get_appx_store_price(int(size))\nprint(price)\n\n# Store file in Mainnet for CRUs\nfile_stored = mainnet.store_file(cid, size)\nprint(file_stored)\n\n# Add renewal pool\nfile_prepaid = mainnet.add_renewal_pool_balance(cid, price*2)\nprint(file_prepaid)\n\n\n# Get replicas\ntime.sleep(10)\nreplicas = mainnet.get_replicas(cid)\nprint(replicas)\n\n```\n\n`Shadow` allows you to perform `Xstorage` extrinsic in Crust Shadow network.\n```python\nfrom crustinterface import Shadow\nfrom substrateinterface import KeypairType\n\nseed = "seed"\nshadow = Shadow(seed=seed, crypto_type=KeypairType.SR25519)\n\n# get any IPFS CID and size\ncid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>\n\nprint(cid, size)\n\n# Check balance\nbalance = shadow.get_balance()\nprint(balance)\n\n# Store file in Shadow for CSMs\nfile_stored = shadow.store_file(cid, size)\nprint(file_stored)\n```\n\n`Parachain` allows you to perform `Xstorage` extrinsic in Crust Polkadot Parachain network.\n```python\nfrom crustinterface import Parachain\nfrom substrateinterface import KeypairType\n\nseed = "seed"\nparachain = Parachain(seed=seed, crypto_type=KeypairType.SR25519)\n\n# get any IPFS CID and size\ncid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>\n\nprint(cid, size)\n\n# Check balance\nbalance = parachain.get_balance()\nprint(balance)\n\n# Store file in Shadow for CSMs\nfile_stored = parachain.store_file(cid, size)\nprint(file_stored)\n```\n',
     'author': 'PaTara43',
     'author_email': 'p040399@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/PaTara43/crust-interface-patara',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `crust_interface_patara-0.1.1/PKG-INFO` & `crust_interface_patara-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: crust-interface-patara
-Version: 0.1.1
-Summary: A simple tool to interact with Crust Shadow and Crust Mainnet. Under development
+Version: 0.2.0
+Summary: A simple tool to interact with Crust Shadow, Crust Polkadot Parachain and Crust Mainnet. Under development
 Home-page: https://github.com/PaTara43/crust-interface-patara
 License: Apache-2.0
-Keywords: python,ipfs,web3,substrate,crust,pypi-package
+Keywords: python,ipfs,web3,substrate,crust,pypi-package,polkadot
 Author: PaTara43
 Author-email: p040399@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -46,17 +46,18 @@
 
 `Mainnet` provides Crust interaction functionality to check user balance, calculate file storage price, placing
 file storage order, add tokens to renewal pool and checking replicas count.
 
 ```python
 import time
 from crustinterface import Mainnet
+from substrateinterface import KeypairType
 
 seed = "seed"
-mainnet = Mainnet(seed=seed)
+mainnet = Mainnet(seed=seed, crypto_type=KeypairType.SR25519)
 
 # get any IPFS CID and size
 cid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>
 
 # Check balance
 balance = mainnet.get_balance()
 print(balance)
@@ -80,16 +81,18 @@
 print(replicas)
 
 ```
 
 `Shadow` allows you to perform `Xstorage` extrinsic in Crust Shadow network.
 ```python
 from crustinterface import Shadow
+from substrateinterface import KeypairType
+
 seed = "seed"
-shadow = Shadow(seed=seed)
+shadow = Shadow(seed=seed, crypto_type=KeypairType.SR25519)
 
 # get any IPFS CID and size
 cid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>
 
 print(cid, size)
 
 # Check balance
@@ -97,7 +100,29 @@
 print(balance)
 
 # Store file in Shadow for CSMs
 file_stored = shadow.store_file(cid, size)
 print(file_stored)
 ```
 
+`Parachain` allows you to perform `Xstorage` extrinsic in Crust Polkadot Parachain network.
+```python
+from crustinterface import Parachain
+from substrateinterface import KeypairType
+
+seed = "seed"
+parachain = Parachain(seed=seed, crypto_type=KeypairType.SR25519)
+
+# get any IPFS CID and size
+cid, size =  "QmbJtyu82TQSHU52AzRMXBENZGQKYqPsmao9dPuTeorPui", 18  # <any way to get an IPFS CID and size. One may use ipfshttpclient2 from IPFS-Toolkit>
+
+print(cid, size)
+
+# Check balance
+balance = parachain.get_balance()
+print(balance)
+
+# Store file in Shadow for CSMs
+file_stored = parachain.store_file(cid, size)
+print(file_stored)
+```
+
```

