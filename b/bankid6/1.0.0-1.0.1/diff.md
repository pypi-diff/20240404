# Comparing `tmp/bankid6-1.0.0.tar.gz` & `tmp/bankid6-1.0.1.tar.gz`

## Comparing `bankid6-1.0.0.tar` & `bankid6-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bankid6-1.0.0/requirements-dev.txt
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bankid6-1.0.0/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bankid6-1.0.0/tox.ini
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/__init__.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/client.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/exceptions.py
--rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/handlers.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/listify.py
--rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/message.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/certs/testCARootCert.pem
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/certs/testCert.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bankid6-1.0.0/src/bankid6/certs/testPrivateKey.pem
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bankid6-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bankid6-1.0.0/tests/factories.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 bankid6-1.0.0/tests/test_client.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bankid6-1.0.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 bankid6-1.0.0/tests/test_handlers.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 bankid6-1.0.0/tests/test_message.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bankid6-1.0.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bankid6-1.0.0/LICENSE
--rw-r--r--   0        0        0    22855 2020-02-02 00:00:00.000000 bankid6-1.0.0/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bankid6-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    23380 2020-02-02 00:00:00.000000 bankid6-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bankid6-1.0.1/requirements-dev.txt
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bankid6-1.0.1/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bankid6-1.0.1/tox.ini
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/__init__.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/client.py
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/exceptions.py
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/handlers.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/listify.py
+-rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/message.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/certs/testCARootCert.pem
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/certs/testCert.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/certs/testPrivateKey.pem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/factories.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/test_client.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/test_handlers.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/test_message.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bankid6-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bankid6-1.0.1/LICENSE
+-rw-r--r--   0        0        0    25492 2020-02-02 00:00:00.000000 bankid6-1.0.1/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bankid6-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    26017 2020-02-02 00:00:00.000000 bankid6-1.0.1/PKG-INFO
```

### Comparing `bankid6-1.0.0/src/bankid6/client.py` & `bankid6-1.0.1/src/bankid6/client.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/src/bankid6/exceptions.py` & `bankid6-1.0.1/src/bankid6/exceptions.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/src/bankid6/handlers.py` & `bankid6-1.0.1/src/bankid6/handlers.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/src/bankid6/listify.py` & `bankid6-1.0.1/src/bankid6/listify.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/src/bankid6/message.py` & `bankid6-1.0.1/src/bankid6/message.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/src/bankid6/certs/testCARootCert.pem` & `bankid6-1.0.1/src/bankid6/certs/testCARootCert.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/src/bankid6/certs/testCert.pem` & `bankid6-1.0.1/src/bankid6/certs/testCert.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/src/bankid6/certs/testPrivateKey.pem` & `bankid6-1.0.1/src/bankid6/certs/testPrivateKey.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/tests/factories.py` & `bankid6-1.0.1/tests/factories.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/tests/test_client.py` & `bankid6-1.0.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/tests/test_exceptions.py` & `bankid6-1.0.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/tests/test_handlers.py` & `bankid6-1.0.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/tests/test_message.py` & `bankid6-1.0.1/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/LICENSE` & `bankid6-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.0/README.md` & `bankid6-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,126 @@
 # bankid6
 
 <br/>
 
 ## Overview
----
 
 A complete implementation of swedish BankID authentication system version 6. It includes initiating/collect/cancel authentication order, User Message and exceptaion handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
 <br/>
 
 ## Installation
----
 
 ```
 pip install bankid6
 ```
 Supports python version 3.6 and later.
+
+<br/>
 <br/>
 
+## Quick Start
+
+The following sample script can get you started quickly. There are more functionalities and customization options than what has shown here.
+
+
+```python
+import time
+from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
+
+
+# Instantiate client. is_mobile means if it's starting from mobile device
+# For production environment use parameters: 
+# prod_env=True, cert_pem=<certificate_filepath>, key_pem='<key_filepath>', ca_pem='<ca_filepath>'
+bankid_client = BankIdClient(is_mobile=False)
+
+try:
+
+    # Start the authentication order. other methods are sign, phone_auth, phone_sign
+    # Takes parameters according to BankID documentation
+    start_response = bankid_client.auth('192.168.0.1')
+
+except BankIdError as bie:
+
+    if bie.message:
+        # If the message is available then it's sufficient just to show the message to the user.
+        # No more action is needed. 
+        print("User Message: ", bie.message[Languages.en])
+    
+    else:
+        # reason and action are from bankid documentaion. 
+        # also, response_data, response_status attributes are available
+        raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
+
+# qr_data gives the calculated data to make qr code. 
+# subsequent values can be found from collect method
+print('QR data: ', start_response.qr_data)
+
+# launch url give you the full url which you need to launch BankID app on current device.
+# It changes depending on is_mobile parameter of client
+# redirect="null" by default
+print('Launch url: ', start_response.launch_url(redirect="https://www.google.com"))
+
+
+while True:
+    time.sleep(1)
+
+    try:
+
+        # Collect the status of order which was initiated with auth/sign/phone_auth/phone_sign method
+
+        # It takes optional parameter which is useful if you want to call collect from different client that you use to initiate the order
+        # Optional prameters: orderRef, qrStartToken, qrStartSecret, order_time
+        # These values are available as start_response attributes. e.g start_response.orderRef
+        collect_response = bankid_client.collect()
+    
+    except BankIdError as bie:
+
+        if bie.message:
+            # Same as before
+            print(bie.message[Languages.en])
+            break
+        
+        else:
+            # same as before
+            raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
+
+
+    # CollectStatuses can be used to easily check statuses. No need to copy form documentation. No room for error.
+    if collect_response.status == CollectStatuses.complete:
+
+        # completionData contains all the nested parsed value in python's datatype
+        # the structure is exactly as documentation. e.g collect_response.completionData.user.personalNumber
+        print('Authenticated by: ', collect_response.completionData.user.name)
+        break
+
+    else:
+
+        # Easily check HintCodes against HintCodes class attributes
+        if collect_response.hintCode == HintCodes.outstandingTransaction:
+
+            # collect response also provides calculated QR data to make QR code
+            # If collect method is called from different client instance than where the was initiated
+            # then qrStartToken, qrStartSecret, order_time parameters are needed to supply to collect method to get Calculated QR data
+            print('QR data: ', collect_response.qr_data)
+        
+        # collect response has appropriate messages according to BankID. The message is a dict object.
+        # UseTypes class has attributes describing if the authentication is started via QR code or Auto Staring app on current device
+        # Language class has 'en' and 'sv' attributes
+        print("User Message: ", collect_response.message[UseTypes.qrcode][Languages.en])
+        
+        # failed response also has message which is printed above
+        if collect_response.status == CollectStatuses.failed:
+            break
+
+```
+
+<br/>
+<br/>
 
 ## User Guide
----
 
 ### Instantiate `BankIdClient` Class
 
 `BankIdClient` provides functionality to initiate authentication or signing order, collect order result or cancel the order.
 
 Instantiate for `BankIdClient` for test environment.
 ```
@@ -216,66 +313,15 @@
 
 
 `BankIdValidationError` is raised before sending the request to BankID if any parameter is invalid.
 
 <br/>
 <br/>
 
-## Sample Script
----
-
-```python
-import time
-from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
-
-bankid_client = BankIdClient()
-
-try:
-    start_response = bankid_client.auth('192.168.0.1')
-except BankIdError as bie:
-    if bie.message:
-        print("User Message: ", bie.message[Languages.en])
-    else:
-        raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
-
-print('QR data: ', start_response.qr_data)
-print('Launch url: ', start_response.launch_url())
-
-
-while True:
-    time.sleep(1)
-
-    try:
-        collect_response = bankid_client.collect()
-    except BankIdError as bie:
-        if bie.message:
-            print(bie.message[Languages.en])
-            break
-        else:
-            raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
-
-    if collect_response.status == CollectStatuses.complete:
-        print('Authenticated by: ', collect_response.completionData.user.name)
-        break
-    else:
-        if collect_response.hintCode == HintCodes.outstandingTransaction:
-            print('QR data: ', collect_response.qr_data)
-        
-        print("User Message: ", collect_response.message[UseTypes.qrcode][Languages.en])
-        
-        if collect_response.status == CollectStatuses.failed:
-            break
-
-```
-
-<br/>
-<br/>
-
 ## API Reference
----
 
 
 #### class BankIdClient()
 <br/>
 
 ##### def __init__(self, prod_env: bool=False, cert_pem: str=None, key_pem: str=None, ca_pem: str=None, request_timeout: int=None, messages: Messages=Messages, is_mobile: bool=False)
```

### Comparing `bankid6-1.0.0/pyproject.toml` & `bankid6-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bankid6"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Amir Ebrahim", email="md.amire02@gmail.com" },
 ]
 description = """
   A complete implementation of swedish BankID version 6. 
   Easily initiate, collect and cancel authentication orders, 
   show user message and handle errors.
```

### Comparing `bankid6-1.0.0/PKG-INFO` & `bankid6-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bankid6
-Version: 1.0.0
+Version: 1.0.1
 Summary:   A complete implementation of swedish BankID version 6.    Easily initiate, collect and cancel authentication orders,    show user message and handle errors.
 Author-email: Amir Ebrahim <md.amire02@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -12,31 +12,128 @@
 Description-Content-Type: text/markdown
 
 # bankid6
 
 <br/>
 
 ## Overview
----
 
 A complete implementation of swedish BankID authentication system version 6. It includes initiating/collect/cancel authentication order, User Message and exceptaion handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
 <br/>
 
 ## Installation
----
 
 ```
 pip install bankid6
 ```
 Supports python version 3.6 and later.
+
+<br/>
 <br/>
 
+## Quick Start
+
+The following sample script can get you started quickly. There are more functionalities and customization options than what has shown here.
+
+
+```python
+import time
+from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
+
+
+# Instantiate client. is_mobile means if it's starting from mobile device
+# For production environment use parameters: 
+# prod_env=True, cert_pem=<certificate_filepath>, key_pem='<key_filepath>', ca_pem='<ca_filepath>'
+bankid_client = BankIdClient(is_mobile=False)
+
+try:
+
+    # Start the authentication order. other methods are sign, phone_auth, phone_sign
+    # Takes parameters according to BankID documentation
+    start_response = bankid_client.auth('192.168.0.1')
+
+except BankIdError as bie:
+
+    if bie.message:
+        # If the message is available then it's sufficient just to show the message to the user.
+        # No more action is needed. 
+        print("User Message: ", bie.message[Languages.en])
+    
+    else:
+        # reason and action are from bankid documentaion. 
+        # also, response_data, response_status attributes are available
+        raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
+
+# qr_data gives the calculated data to make qr code. 
+# subsequent values can be found from collect method
+print('QR data: ', start_response.qr_data)
+
+# launch url give you the full url which you need to launch BankID app on current device.
+# It changes depending on is_mobile parameter of client
+# redirect="null" by default
+print('Launch url: ', start_response.launch_url(redirect="https://www.google.com"))
+
+
+while True:
+    time.sleep(1)
+
+    try:
+
+        # Collect the status of order which was initiated with auth/sign/phone_auth/phone_sign method
+
+        # It takes optional parameter which is useful if you want to call collect from different client that you use to initiate the order
+        # Optional prameters: orderRef, qrStartToken, qrStartSecret, order_time
+        # These values are available as start_response attributes. e.g start_response.orderRef
+        collect_response = bankid_client.collect()
+    
+    except BankIdError as bie:
+
+        if bie.message:
+            # Same as before
+            print(bie.message[Languages.en])
+            break
+        
+        else:
+            # same as before
+            raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
+
+
+    # CollectStatuses can be used to easily check statuses. No need to copy form documentation. No room for error.
+    if collect_response.status == CollectStatuses.complete:
+
+        # completionData contains all the nested parsed value in python's datatype
+        # the structure is exactly as documentation. e.g collect_response.completionData.user.personalNumber
+        print('Authenticated by: ', collect_response.completionData.user.name)
+        break
+
+    else:
+
+        # Easily check HintCodes against HintCodes class attributes
+        if collect_response.hintCode == HintCodes.outstandingTransaction:
+
+            # collect response also provides calculated QR data to make QR code
+            # If collect method is called from different client instance than where the was initiated
+            # then qrStartToken, qrStartSecret, order_time parameters are needed to supply to collect method to get Calculated QR data
+            print('QR data: ', collect_response.qr_data)
+        
+        # collect response has appropriate messages according to BankID. The message is a dict object.
+        # UseTypes class has attributes describing if the authentication is started via QR code or Auto Staring app on current device
+        # Language class has 'en' and 'sv' attributes
+        print("User Message: ", collect_response.message[UseTypes.qrcode][Languages.en])
+        
+        # failed response also has message which is printed above
+        if collect_response.status == CollectStatuses.failed:
+            break
+
+```
+
+<br/>
+<br/>
 
 ## User Guide
----
 
 ### Instantiate `BankIdClient` Class
 
 `BankIdClient` provides functionality to initiate authentication or signing order, collect order result or cancel the order.
 
 Instantiate for `BankIdClient` for test environment.
 ```
@@ -229,66 +326,15 @@
 
 
 `BankIdValidationError` is raised before sending the request to BankID if any parameter is invalid.
 
 <br/>
 <br/>
 
-## Sample Script
----
-
-```python
-import time
-from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
-
-bankid_client = BankIdClient()
-
-try:
-    start_response = bankid_client.auth('192.168.0.1')
-except BankIdError as bie:
-    if bie.message:
-        print("User Message: ", bie.message[Languages.en])
-    else:
-        raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
-
-print('QR data: ', start_response.qr_data)
-print('Launch url: ', start_response.launch_url())
-
-
-while True:
-    time.sleep(1)
-
-    try:
-        collect_response = bankid_client.collect()
-    except BankIdError as bie:
-        if bie.message:
-            print(bie.message[Languages.en])
-            break
-        else:
-            raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
-
-    if collect_response.status == CollectStatuses.complete:
-        print('Authenticated by: ', collect_response.completionData.user.name)
-        break
-    else:
-        if collect_response.hintCode == HintCodes.outstandingTransaction:
-            print('QR data: ', collect_response.qr_data)
-        
-        print("User Message: ", collect_response.message[UseTypes.qrcode][Languages.en])
-        
-        if collect_response.status == CollectStatuses.failed:
-            break
-
-```
-
-<br/>
-<br/>
-
 ## API Reference
----
 
 
 #### class BankIdClient()
 <br/>
 
 ##### def __init__(self, prod_env: bool=False, cert_pem: str=None, key_pem: str=None, ca_pem: str=None, request_timeout: int=None, messages: Messages=Messages, is_mobile: bool=False)
```

