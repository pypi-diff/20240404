# Comparing `tmp/payments_py-0.1.0.tar.gz` & `tmp/payments_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payments_py-0.1.0.tar", max compression
+gzip compressed data, was "payments_py-0.1.1.tar", max compression
```

## Comparing `payments_py-0.1.0.tar` & `payments_py-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-03-15 10:51:16.892868 payments_py-0.1.0/LICENSE
--rw-r--r--   0        0        0      584 2024-03-15 10:51:16.892868 payments_py-0.1.0/README.md
--rw-r--r--   0        0        0      159 2024-03-15 10:51:16.892868 payments_py-0.1.0/payments_py/__init__.py
--rw-r--r--   0        0        0      767 2024-03-15 10:51:16.892868 payments_py-0.1.0/payments_py/environments.py
--rw-r--r--   0        0        0    12926 2024-03-15 10:51:16.892868 payments_py-0.1.0/payments_py/payments.py
--rw-r--r--   0        0        0      162 2024-03-15 10:51:16.892868 payments_py-0.1.0/payments_py/utils.py
--rw-r--r--   0        0        0      419 2024-03-15 10:51:16.892868 payments_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 payments_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-04 14:27:55.166324 payments_py-0.1.1/LICENSE
+-rw-r--r--   0        0        0      584 2024-04-04 14:27:55.166324 payments_py-0.1.1/README.md
+-rw-r--r--   0        0        0      159 2024-04-04 14:27:55.166324 payments_py-0.1.1/payments_py/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-04 14:27:55.166324 payments_py-0.1.1/payments_py/environments.py
+-rw-r--r--   0        0        0    14626 2024-04-04 14:27:55.166324 payments_py-0.1.1/payments_py/payments.py
+-rw-r--r--   0        0        0      229 2024-04-04 14:27:55.166324 payments_py-0.1.1/payments_py/utils.py
+-rw-r--r--   0        0        0      496 2024-04-04 14:27:55.170323 payments_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 payments_py-0.1.1/PKG-INFO
```

### Comparing `payments_py-0.1.0/LICENSE` & `payments_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `payments_py-0.1.0/README.md` & `payments_py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `payments_py-0.1.0/payments_py/environments.py` & `payments_py-0.1.1/payments_py/environments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 from enum import Enum
 
 class Environment(Enum):
+    """
+    Enum class to define the different environments
+
+    Attributes:
+        local: Local environment
+        appStaging: Staging environment
+        appTesting: Testing environment
+        appArbitrum: Arbitrum environment
+        appGnosis: Gnosis environment
+        appMatic: Matic environment
+    """
     local = {"frontend": "http://localhost:3000", "backend": "http://localhost:3200"}
     appStaging = {"frontend": "https://staging.nevermined.app", "backend": "https://one-backend.staging.nevermined.app"}
     appTesting = {"frontend": "https://testing.nevermined.app", "backend": "https://one-backend.testing.nevermined.app"}
     appArbitrum = {"frontend": "https://nevermined.app", "backend": "https://one-backend.arbitrum.nevermined.app"}
     appGnosis = {"frontend": "https://gnosis.nevermined.app", "backend": "https://one-backend.gnosis.nevermined.app"}
     appMatic = {"frontend": "https://matic.nevermined.app", "backend": "https://one-backend.matic.nevermined.app"}
     # Define more environments as needed...
```

### Comparing `payments_py-0.1.0/payments_py/payments.py` & `payments_py-0.1.1/payments_py/payments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from typing import List, Optional
 import requests
 
-from .environments import Environment
-from .utils import snake_to_camel
+from payments_py.environments import Environment
+from payments_py.utils import snake_to_camel
 
 
 class Payments:
     """
     A class representing a payment system.
 
     Attributes:
         session_key (str): The session key for authentication.
         environment (Environment): The environment for the payment system.
         marketplace_auth_token (str, optional): The marketplace authentication token.
         app_id (str, optional): The application ID.
         version (str, optional): The version of the payment system.
 
     Methods:
-        createSubscription: Creates a new subscription.
-        createService: Creates a new service.
-    """
+        create_ubscription: Creates a new subscription.
+        create_service: Creates a new service.
+        create_file: Creates a new file.
+        get_asset_ddo: Gets the asset DDO.
+        get_subscription_balance: Gets the subscription balance.
+        get_service_token: Gets the service token.
+        get_subscription_details: Gets the subscription details.
+        get_service_details: Gets the service details.
+        get_file_details: Gets the file details.
+        get_checkout_subscription: Gets the checkout subscription.     
+        """
 
     def __init__(self, session_key: str, environment: Environment, marketplace_auth_token: Optional[str] = None,
                  app_id: Optional[str] = None, version: Optional[str] = None):
         self.session_key = session_key
         self.environment = environment
         self.app_id = app_id
         self.version = version
@@ -242,14 +250,50 @@
             'Accept': 'application/json',
             'Content-Type': 'application/json'
         }
         url = f"{self.environment.value['backend']}/api/v1/payments/service/token"
         response = requests.post(url, headers=headers, json=body)
         return response
 
+    def get_subscription_associated_services(self, subscription_did: str):
+        """
+        Gets the subscription associated services.
+
+        Args:
+            subscription_did (str): The DID of the subscription.
+
+        Returns:
+            Response: List of DIDs of the associated services.
+        """
+        headers = {
+            'Accept': 'application/json',
+            'Content-Type': 'application/json'
+        }
+        url = f"{self.environment.value['backend']}/api/v1/payments/subscription/services/{subscription_did}/"
+        response = requests.get(url, headers=headers)
+        return response
+    
+    def get_subscription_associated_files(self, subscription_did: str):
+        """
+        Gets the subscription associated files.
+
+        Args:
+            subscription_did (str): The DID of the subscription.
+
+        Returns:
+            Response: List of DIDs of the associated files.
+        """
+        headers = {
+            'Accept': 'application/json',
+            'Content-Type': 'application/json'
+        }
+        url = f"{self.environment.value['backend']}/api/v1/payments/subscription/files/{subscription_did}/"
+        response = requests.get(url, headers=headers)
+        return response
+
     def get_subscription_details(self, subscription_did: str):
         """
         Gets the subscription details.
 
         Args:
             subscription_did (str): The DID of the subscription.
```

### Comparing `payments_py-0.1.0/PKG-INFO` & `payments_py-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: payments-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: enrique
 Author-email: enrique@nevermined.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: lazydocs (>=0.4.8,<0.5.0)
+Requires-Dist: mkdocs (>=1.5.3,<2.0.0)
+Requires-Dist: mkdocs-awesome-pages-plugin (>=2.9.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![banner](https://raw.githubusercontent.com/nevermined-io/assets/main/images/logo/banner_logo.png)](https://nevermined.io)
 
 # Python SDK to interact with the Nevermined Payments Protocol
```

