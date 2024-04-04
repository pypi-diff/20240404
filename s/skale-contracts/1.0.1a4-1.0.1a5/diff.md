# Comparing `tmp/skale-contracts-1.0.1a4.tar.gz` & `tmp/skale-contracts-1.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale-contracts-1.0.1a4.tar", last modified: Fri Mar 15 13:37:43 2024, max compression
+gzip compressed data, was "skale-contracts-1.0.1a5.tar", last modified: Thu Apr  4 15:59:27 2024, max compression
```

## Comparing `skale-contracts-1.0.1a4.tar` & `skale-contracts-1.0.1a5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:37:43.394487 skale-contracts-1.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-15 13:37:43.394487 skale-contracts-1.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-15 13:37:43.394487 skale-contracts-1.0.1a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:37:43.390487 skale-contracts-1.0.1a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:37:43.394487 skale-contracts-1.0.1a4/src/skale_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/project_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/project_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:37:43.394487 skale-contracts-1.0.1a4/src/skale_contracts/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/projects/ima.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/projects/skale_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-15 13:37:32.000000 skale-contracts-1.0.1a4/src/skale_contracts/skale_contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:37:43.394487 skale-contracts-1.0.1a4/src/skale_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-15 13:37:43.000000 skale-contracts-1.0.1a4/src/skale_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-15 13:37:43.000000 skale-contracts-1.0.1a4/src/skale_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 13:37:43.000000 skale-contracts-1.0.1a4/src/skale_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-15 13:37:43.000000 skale-contracts-1.0.1a4/src/skale_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-15 13:37:43.000000 skale-contracts-1.0.1a4/src/skale_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 13:37:41.000000 skale-contracts-1.0.1a4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.634534 skale-contracts-1.0.1a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/src/skale_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/project_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/src/skale_contracts/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/projects/ima.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/projects/skale_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/projects/skale_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/skale_contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 15:59:25.000000 skale-contracts-1.0.1a5/version.txt
```

### Comparing `skale-contracts-1.0.1a4/PKG-INFO` & `skale-contracts-1.0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 1.0.1a4
+Version: 1.0.1a5
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale-contracts-1.0.1a4/setup.cfg` & `skale-contracts-1.0.1a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts/instance.py` & `skale-contracts-1.0.1a5/src/skale_contracts/instance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for instance management"""
 
 from __future__ import annotations
 from abc import ABC, abstractmethod
 import json
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, cast
 from attr import dataclass
+from eth_typing import ChecksumAddress
 from parver import Version as PyVersion
 from semver.version import Version as SemVersion
 
 
 if TYPE_CHECKING:
     from eth_typing import Address
     from web3 import Web3
@@ -20,22 +21,23 @@
 DEFAULT_GET_VERSION_FUNCTION = {
     "type": "function",
     "name": "version",
     "constant": True,
     "stateMutability": "view",
     "payable": False,
     "inputs": [],
-    "outputs": [ { "type": "string", "name": "" } ]
+    "outputs": [{"type": "string", "name": ""}]
 }
 
 
 @dataclass
 class InstanceData:
     """Contains instance data"""
     data: dict[str, str]
+
     @classmethod
     def from_json(cls, data: str) -> InstanceData:
         """Create InstanceData object from json string"""
         return cls(data=json.loads(data))
 
 
 class Instance(ABC):
@@ -75,24 +77,37 @@
                 self._version = str(sem_version)
         return self._version
 
     @property
     def abi(self) -> SkaleAbi:
         """Get abi file of the project instance"""
         if self._abi is None:
-            self._abi = json.loads(self._project.download_abi_file(self.version))
+            self._abi = json.loads(
+                self._project.download_abi_file(self.version)
+            )
         return self._abi
 
     @abstractmethod
-    def get_contract_address(self, name: str) -> Address:
+    def get_contract_address(
+        self,
+        name: str,
+        *args: str | Address | ChecksumAddress
+    ) -> Address:
         """Get address of the contract by it's name"""
 
-    def get_contract(self, name: str) -> Contract:
+    def get_contract(
+            self,
+            name: str,
+            *args: str | Address | ChecksumAddress
+    ) -> Contract:
         """Get Contract object of the contract by it's name"""
-        address = self.get_contract_address(name)
+        address = self.get_contract_address(name, *args)
         return self.web3.eth.contract(address=address, abi=self.abi[name])
 
     # protected
 
-    @abstractmethod
     def _get_version(self) -> str:
-        pass
+        contract = self.web3.eth.contract(
+            address=self.address,
+            abi=[DEFAULT_GET_VERSION_FUNCTION]
+        )
+        return cast(str, contract.functions.version().call())
```

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts/metadata.py` & `skale-contracts-1.0.1a5/src/skale_contracts/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 @dataclass
 class NetworkMetadata:
     """Contains metadata of a network"""
     name: str
     chain_id: int
     path: str
 
+
 @dataclass
 class MetadataFile:
     """Represents file with metadata"""
     networks: list[NetworkMetadata]
 
     @classmethod
     def from_json(cls, data: str) -> MetadataFile:
@@ -29,14 +30,15 @@
         for network in file['networks']:
             networks.append(NetworkMetadata(
                 name=network['name'],
                 chain_id=network['chainId'],
                 path=network['path']))
         return cls(networks)
 
+
 class Metadata:
     """Class to manage SKALE contracts metadata"""
     networks: list[NetworkMetadata]
 
     def __init__(self) -> None:
         self.download()
 
@@ -45,15 +47,18 @@
         metadata_response = requests.get(
             REPOSITORY_URL + METADATA_FILENAME,
             timeout=NETWORK_TIMEOUT
         )
         metadata = MetadataFile.from_json(metadata_response.text)
         self.networks = metadata.networks
 
-    def get_network_by_chain_id(self, chain_id: int) -> Optional[NetworkMetadata]:
+    def get_network_by_chain_id(
+            self,
+            chain_id: int
+    ) -> Optional[NetworkMetadata]:
         """Get network metadata by it's chain id.
         Returns None if there is no such network in the metadata.
         """
         for network in self.networks:
             if network.chain_id == chain_id:
                 return network
         return None
```

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts/network.py` & `skale-contracts-1.0.1a5/src/skale_contracts/network.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 if TYPE_CHECKING:
     from .project import Project
     from .skale_contracts import SkaleContracts
 
 
 class Network:
     """Represents blockchain with deployed smart contracts projects"""
-    def __init__(self, skale_contracts: SkaleContracts, provider: BaseProvider):
+    def __init__(
+            self,
+            skale_contracts: SkaleContracts,
+            provider: BaseProvider
+    ):
         self.web3 = Web3(provider)
         self._skale_contracts = skale_contracts
 
     def get_project(self, name: str) -> Project:
         """Get Project object by it's name"""
         return create_project(self, name)
 
@@ -35,14 +39,19 @@
     def as_listed(self) -> ListedNetwork:
         """Cast to ListedNetwork"""
         return cast(ListedNetwork, self)
 
 
 class ListedNetwork(Network):
     """Network that is listed in the metadata"""
-    def __init__(self, skale_contracts: SkaleContracts, provider: BaseProvider, path: str):
+    def __init__(
+            self,
+            skale_contracts: SkaleContracts,
+            provider: BaseProvider,
+            path: str
+    ):
         super().__init__(skale_contracts, provider)
         self.path = path
 
     def is_listed(self) -> bool:
         """Return if the network is present in the skale-contract repository"""
         return True
```

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts/project.py` & `skale-contracts-1.0.1a5/src/skale_contracts/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,30 +7,38 @@
 
 from .constants import REPOSITORY_URL, NETWORK_TIMEOUT
 from .instance import Instance, InstanceData
 
 if TYPE_CHECKING:
     from eth_typing import Address
     from .network import Network
-    from .project_metadata import ProjectMetadata
 
 
 class Project(ABC):
     """Represents set of smart contracts known as project"""
 
-    def __init__(self, network: Network, metadata: ProjectMetadata) -> None:
+    def __init__(self, network: Network) -> None:
         super().__init__()
         self.network = network
-        self._metadata = metadata
+
+    @staticmethod
+    @abstractmethod
+    def name() -> str:
+        """Name of the project"""
 
     @property
     @abstractmethod
     def github_repo(self) -> str:
         """URL of github repo with the project"""
 
+    @property
+    def folder(self) -> str:
+        """Folder name with instances json files"""
+        return self.name()
+
     def get_instance(self, alias_or_address: str) -> Instance:
         """Create instance object based on alias or address"""
         if self.network.web3.is_address(alias_or_address):
             address = to_canonical_address(alias_or_address)
             return self.create_instance(address)
         alias = alias_or_address
         url = self.get_instance_data_url(alias)
@@ -49,23 +57,24 @@
         response = requests.get(url, timeout=NETWORK_TIMEOUT)
         if response.status_code != 200:
             raise RuntimeError(f"Can't download abi file from {url}")
         return response.text
 
     def get_abi_url(self, version: str) -> str:
         """Calculate URL of ABI file"""
-        return f'{self.github_repo}releases/download/{version}/{self.get_abi_filename(version)}'
+        filename = self.get_abi_filename(version)
+        return f'{self.github_repo}releases/download/{version}/{filename}'
 
     @abstractmethod
     def get_abi_filename(self, version: str) -> str:
         """Return name of a file with ABI"""
 
     def get_instance_data_url(self, alias: str) -> str:
         """Get URL of a file containing address for provided alias"""
         if self.network.is_listed():
             return f'{REPOSITORY_URL}{self.network.as_listed().path}/' + \
-                f'{self._metadata.path}/{alias}.json'
+                f'{self.folder}/{alias}.json'
         raise ValueError('Network is unknown')
 
     @abstractmethod
     def create_instance(self, address: Address) -> Instance:
         """Create instance object based on known address"""
```

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts/projects/ima.py` & `skale-contracts-1.0.1a5/src/skale_contracts/projects/ima.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """Module connects IMA to the SKALE contracts library"""
 
 from __future__ import annotations
-from typing import cast, TYPE_CHECKING
-from eth_typing import Address
+from typing import TYPE_CHECKING
 from eth_utils.address import to_canonical_address
 
 from skale_contracts.constants import PREDEPLOYED_ALIAS
 from skale_contracts.instance import Instance, DEFAULT_GET_VERSION_FUNCTION
 from skale_contracts.project import Project
 
 from .skale_manager import CONTRACT_MANAGER_ABI
 
 
 if TYPE_CHECKING:
+    from eth_typing import Address, ChecksumAddress
     from web3.contract.contract import Contract
 
 MESSAGE_PROXY_ABI = [
     DEFAULT_GET_VERSION_FUNCTION
 ]
 
 
 class ImaInstance(Instance):
     """Represents instance of IMA"""
     def __init__(self, project: Project, address: Address) -> None:
         super().__init__(project, address)
-        self.message_proxy = self.web3.eth.contract(address=address, abi=MESSAGE_PROXY_ABI)
-
-    def _get_version(self) -> str:
-        return cast(str, self.message_proxy.functions.version().call())
+        self.message_proxy = self.web3.eth.contract(
+            address=address,
+            abi=MESSAGE_PROXY_ABI
+        )
 
 
 class ImaProject(Project):
     """Represents IMA project"""
 
     @property
     def github_repo(self) -> str:
@@ -41,82 +41,112 @@
 class MainnetImaInstance(ImaInstance):
     """Represents IMA instance on mainnet"""
 
     def __init__(self, project: Project, address: Address) -> None:
         super().__init__(project, address)
         self._contract_manager: Contract | None = None
 
-    def get_contract_address(self, name: str) -> Address:
+    def get_contract_address(
+            self,
+            name: str, *args: str | Address | ChecksumAddress
+    ) -> Address:
         if name == 'MessageProxyForMainnet':
             return self.address
         if name == 'CommunityPool':
             return to_canonical_address(
-                self.get_contract("MessageProxyForMainnet").functions.communityPool().call()
+                self.get_contract("MessageProxyForMainnet")
+                    .functions.communityPool().call()
             )
         if name == 'Linker':
             return to_canonical_address(
-                self.get_contract("MessageProxyForMainnet").functions.linker().call()
+                self.get_contract("MessageProxyForMainnet")
+                    .functions.linker().call()
             )
         return to_canonical_address(
             self.contract_manager.functions.getContract(name).call()
         )
 
     @property
     def contract_manager(self) -> Contract:
-        """ContractManager contract of a skale-manager instance associated with the IMA"""
+        """ContractManager contract of a skale-manager instance
+associated with the IMA"""
         if self._contract_manager is None:
             self._contract_manager = self.web3.eth.contract(
                 address=to_canonical_address(
                     self.get_contract("MessageProxyForMainnet")
                         .functions.contractManagerOfSkaleManager().call()
                 ),
                 abi=CONTRACT_MANAGER_ABI
             )
         return self._contract_manager
 
 
 class MainnetImaProject(ImaProject):
     """Represents mainnet part of IMA project"""
 
+    @staticmethod
+    def name() -> str:
+        return 'mainnet-ima'
+
     def create_instance(self, address: Address) -> Instance:
         return MainnetImaInstance(self, address)
 
     def get_abi_filename(self, version: str) -> str:
         return f'mainnet-ima-{version}-abi.json'
 
 
 class SchainImaInstance(ImaInstance):
     """Represents IMA instance on schain"""
 
     PREDEPLOYED: dict[str, Address] = {
         name: to_canonical_address(address) for name, address in {
-            'ProxyAdmin':                       '0xd2aAa00000000000000000000000000000000000',
-            'MessageProxyForSchain':            '0xd2AAa00100000000000000000000000000000000',
-            'KeyStorage':                       '0xd2aaa00200000000000000000000000000000000',
-            'CommunityLocker':                  '0xD2aaa00300000000000000000000000000000000',
-            'TokenManagerEth':                  '0xd2AaA00400000000000000000000000000000000',
-            'TokenManagerERC20':                '0xD2aAA00500000000000000000000000000000000',
-            'TokenManagerERC721':               '0xD2aaa00600000000000000000000000000000000',
-            'TokenManagerLinker':               '0xD2aAA00800000000000000000000000000000000',
-            'TokenManagerERC1155':              '0xD2aaA00900000000000000000000000000000000',
-            'TokenManagerERC721WithMetadata':   '0xd2AaA00a00000000000000000000000000000000'
+            'ProxyAdmin':
+                '0xd2aAa00000000000000000000000000000000000',
+            'MessageProxyForSchain':
+                '0xd2AAa00100000000000000000000000000000000',
+            'KeyStorage':
+                '0xd2aaa00200000000000000000000000000000000',
+            'CommunityLocker':
+                '0xD2aaa00300000000000000000000000000000000',
+            'TokenManagerEth':
+                '0xd2AaA00400000000000000000000000000000000',
+            'TokenManagerERC20':
+                '0xD2aAA00500000000000000000000000000000000',
+            'TokenManagerERC721':
+                '0xD2aaa00600000000000000000000000000000000',
+            'TokenManagerLinker':
+                '0xD2aAA00800000000000000000000000000000000',
+            'TokenManagerERC1155':
+                '0xD2aaA00900000000000000000000000000000000',
+            'TokenManagerERC721WithMetadata':
+                '0xd2AaA00a00000000000000000000000000000000'
         }.items()}
 
-    def get_contract_address(self, name: str) -> Address:
+    def get_contract_address(
+            self,
+            name: str,
+            *args: str | Address | ChecksumAddress
+    ) -> Address:
         if name in self.PREDEPLOYED:
             return self.PREDEPLOYED[name]
         raise RuntimeError(f"Can't get address of {name} contract")
 
 
 class SchainImaProject(ImaProject):
     """Represents schain part of IMA project"""
 
+    @staticmethod
+    def name() -> str:
+        return 'schain-ima'
+
     def get_instance(self, alias_or_address: str) -> Instance:
         if alias_or_address == PREDEPLOYED_ALIAS:
-            return self.create_instance(SchainImaInstance.PREDEPLOYED['MessageProxyForSchain'])
+            return self.create_instance(
+                SchainImaInstance.PREDEPLOYED['MessageProxyForSchain']
+            )
         return super().get_instance(alias_or_address)
 
     def create_instance(self, address: Address) -> Instance:
         return SchainImaInstance(self, address)
 
     def get_abi_filename(self, version: str) -> str:
         return f'schain-ima-{version}-abi.json'
```

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts/projects/skale_manager.py` & `skale-contracts-1.0.1a5/src/skale_contracts/projects/skale_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,97 @@
 """Module connects skale-manager project to the SKALE contracts library"""
 
 from __future__ import annotations
-from typing import cast, TYPE_CHECKING
+from typing import TYPE_CHECKING
 from eth_utils.address import to_canonical_address
 
 from skale_contracts.instance import Instance, DEFAULT_GET_VERSION_FUNCTION
 from skale_contracts.project import Project
 
 
 if TYPE_CHECKING:
-    from eth_typing import Address
+    from eth_typing import Address, ChecksumAddress
     from web3.contract.contract import Contract
 
 SKALE_MANAGER_ABI = [
     {
         "inputs": [],
         "name": "contractManager",
-        "outputs": [{ "internalType": "contract IContractManager", "name": "", "type": "address" }],
+        "outputs": [{
+            "internalType": "contract IContractManager",
+            "name": "",
+            "type": "address"
+        }],
         "stateMutability": "view", "type": "function"
     },
     DEFAULT_GET_VERSION_FUNCTION
 ]
 
 CONTRACT_MANAGER_ABI = [
     {
-        "inputs": [{ "internalType": "string", "name": "name", "type": "string" }],
+        "inputs": [{
+            "internalType": "string",
+            "name": "name",
+            "type": "string"
+        }],
         "name": "getContract",
-        "outputs": [{ "internalType": "address", "name": "contractAddress", "type": "address" }],
+        "outputs": [{
+            "internalType": "address",
+            "name": "contractAddress",
+            "type": "address"
+        }],
         "stateMutability": "view",
         "type": "function"
     }
 ]
 
 
 class SkaleManagerInstance(Instance):
     """Represents instance of skale-manager"""
     def __init__(self, project: Project, address: Address) -> None:
         super().__init__(project, address)
-        self.skale_manager = self.web3.eth.contract(address=address, abi=SKALE_MANAGER_ABI)
-        contract_manager_address: Address = self.skale_manager.functions.contractManager().call()
+        self.skale_manager = self.web3.eth.contract(
+            address=address,
+            abi=SKALE_MANAGER_ABI
+        )
+        contract_manager_address: Address = \
+            self.skale_manager.functions.contractManager().call()
         self.contract_manager: Contract = self.web3.eth.contract(
             address=contract_manager_address,
             abi=CONTRACT_MANAGER_ABI
         )
         self.custom_names = {
             'BountyV2': 'Bounty',
             'TimeHelpersWithDebug':  'TimeHelpers'
         }
 
-    def get_contract_address(self, name: str) -> Address:
+    def get_contract_address(
+            self,
+            name: str,
+            *args: str | Address | ChecksumAddress
+    ) -> Address:
         return to_canonical_address(
-            self.contract_manager.functions.getContract(self._actual_name(name)).call()
+            self.contract_manager.functions.getContract(
+                self._actual_name(name)
+            ).call()
         )
 
-    def _get_version(self) -> str:
-        return cast(str, self.skale_manager.functions.version().call())
-
     def _actual_name(self, name: str) -> str:
         if name in self.custom_names:
             return self.custom_names[name]
         return name
 
 
 class SkaleManagerProject(Project):
     """Represents skale-manager project"""
 
+    @staticmethod
+    def name() -> str:
+        return 'skale-manager'
+
     @property
     def github_repo(self) -> str:
         return 'https://github.com/skalenetwork/skale-manager/'
 
     def create_instance(self, address: Address) -> Instance:
         return SkaleManagerInstance(self, address)
```

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts/skale_contracts.py` & `skale-contracts-1.0.1a5/src/skale_contracts/skale_contracts.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts.egg-info/PKG-INFO` & `skale-contracts-1.0.1a5/src/skale_contracts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 1.0.1a4
+Version: 1.0.1a5
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale-contracts-1.0.1a4/src/skale_contracts.egg-info/SOURCES.txt` & `skale-contracts-1.0.1a5/src/skale_contracts.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 src/skale_contracts/abi.py
 src/skale_contracts/constants.py
 src/skale_contracts/instance.py
 src/skale_contracts/metadata.py
 src/skale_contracts/network.py
 src/skale_contracts/project.py
 src/skale_contracts/project_factory.py
-src/skale_contracts/project_metadata.py
 src/skale_contracts/skale_contracts.py
 src/skale_contracts.egg-info/PKG-INFO
 src/skale_contracts.egg-info/SOURCES.txt
 src/skale_contracts.egg-info/dependency_links.txt
 src/skale_contracts.egg-info/requires.txt
 src/skale_contracts.egg-info/top_level.txt
 src/skale_contracts/projects/__init__.py
 src/skale_contracts/projects/ima.py
+src/skale_contracts/projects/skale_allocator.py
 src/skale_contracts/projects/skale_manager.py
```

