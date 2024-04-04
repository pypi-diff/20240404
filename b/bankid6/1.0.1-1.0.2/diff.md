# Comparing `tmp/bankid6-1.0.1.tar.gz` & `tmp/bankid6-1.0.2.tar.gz`

## Comparing `bankid6-1.0.1.tar` & `bankid6-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bankid6-1.0.1/requirements-dev.txt
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bankid6-1.0.1/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bankid6-1.0.1/tox.ini
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/__init__.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/client.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/exceptions.py
--rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/handlers.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/listify.py
--rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/message.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/certs/testCARootCert.pem
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/certs/testCert.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bankid6-1.0.1/src/bankid6/certs/testPrivateKey.pem
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/factories.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/test_client.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/test_handlers.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 bankid6-1.0.1/tests/test_message.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bankid6-1.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bankid6-1.0.1/LICENSE
--rw-r--r--   0        0        0    25492 2020-02-02 00:00:00.000000 bankid6-1.0.1/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bankid6-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    26017 2020-02-02 00:00:00.000000 bankid6-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bankid6-1.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bankid6-1.0.2/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bankid6-1.0.2/tox.ini
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/__init__.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/client.py
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/exceptions.py
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/handlers.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/listify.py
+-rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/message.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/certs/testCARootCert.pem
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/certs/testCert.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/certs/testPrivateKey.pem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/factories.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/test_client.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/test_handlers.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/test_message.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bankid6-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bankid6-1.0.2/LICENSE
+-rw-r--r--   0        0        0    25681 2020-02-02 00:00:00.000000 bankid6-1.0.2/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bankid6-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    26206 2020-02-02 00:00:00.000000 bankid6-1.0.2/PKG-INFO
```

### Comparing `bankid6-1.0.1/src/bankid6/client.py` & `bankid6-1.0.2/src/bankid6/client.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/src/bankid6/exceptions.py` & `bankid6-1.0.2/src/bankid6/exceptions.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/src/bankid6/handlers.py` & `bankid6-1.0.2/src/bankid6/handlers.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/src/bankid6/listify.py` & `bankid6-1.0.2/src/bankid6/listify.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/src/bankid6/message.py` & `bankid6-1.0.2/src/bankid6/message.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/src/bankid6/certs/testCARootCert.pem` & `bankid6-1.0.2/src/bankid6/certs/testCARootCert.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/src/bankid6/certs/testCert.pem` & `bankid6-1.0.2/src/bankid6/certs/testCert.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/src/bankid6/certs/testPrivateKey.pem` & `bankid6-1.0.2/src/bankid6/certs/testPrivateKey.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/tests/factories.py` & `bankid6-1.0.2/tests/factories.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/tests/test_client.py` & `bankid6-1.0.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/tests/test_exceptions.py` & `bankid6-1.0.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/tests/test_handlers.py` & `bankid6-1.0.2/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/tests/test_message.py` & `bankid6-1.0.2/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/LICENSE` & `bankid6-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.1/README.md` & `bankid6-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 <br/>
 
 ## Overview
 
 A complete implementation of swedish BankID authentication system version 6. It includes initiating/collect/cancel authentication order, User Message and exceptaion handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
 <br/>
+<br/>
 
 ## Installation
 
 ```
 pip install bankid6
 ```
 Supports python version 3.6 and later.
@@ -114,15 +115,15 @@
 ```
 
 <br/>
 <br/>
 
 ## User Guide
 
-### Instantiate `BankIdClient` Class
+### 1. Instantiate `BankIdClient` Class
 
 `BankIdClient` provides functionality to initiate authentication or signing order, collect order result or cancel the order.
 
 Instantiate for `BankIdClient` for test environment.
 ```
 >>> from bankid6 import BankIdClient
 >>> bankid_client = BankIdClient()
@@ -134,16 +135,17 @@
 <br/>
 
 To initialize for a production environment, ensure that the `prod_env` parameter is set to `True`. Additionally, you must provide the file paths for the certificate, the private key associated with the certificate, and the CA certificate.
 ```
 >>> bankid_client = BankIdClient(prod_env=True, cert_pem=<certificate_filepath>, key_pem='<private_key_filepath>', ca_pem=<ca_certificate_filepath>)
 ```
 <br/>
+<br/>
 
-### Initiate Authentication or Signing Order
+### 2. Initiate Authentication or Signing Order
 
 The `BankIdClient` offers `auth` and `sign` methods to initiate authentication and signing orders, respectively. These methods return a `BankIdStartResponse` object, which contains attributes to easily get the data for QR code and url for launching the BankID app.
 
 ```
 >>> bankid_client = BankIdClient()
 >>> start_response = bankid_client.auth('192.168.0.1')      # Takes IP of end user
 
@@ -184,16 +186,17 @@
 
 These methods have required or optional parameters exactly as described in BankID documentation. These parameters are validated, processed as BankID requires and sent as the data of the request to the BankID.
 
 The returned objects are derived from `BankIdBaseResponse`, parses any BankID response, creating an attribute with the same name as the key of the response data. `BankIdBaseResponse` has attributes related to actual HTTP response. This is also True for `collect` or `cancel`.
 
 See the API Reference section for comprehensive documentation detailing parameters and return values.
 <br/>
+<br/>
 
-### Collect Order Result
+### 3. Collect Order Result
 
 Use `collect` method of `BankIdClient` object to get the order result.
 ```
 >>> from bankid6 import BankIdClient
 >>> bankid_client = BankIdClient()
 
 >>> bankid_client.auth('192.168.0.1')
@@ -269,16 +272,17 @@
     RFA1 = {'test': 'yes'}
     RFA13 = ('<h3>swedish message<h3>', '<h3>english message</h3>')
 
 bankid_client = BankIdClient(messages=MyMessage)
 ```
 Their value can be a dict or a tuple of swedish and english messages. If the value is dict, it is returned as it is from `message` attribute of `BankIdCollectResponse` object.
 <br/>
+<br/>
 
-### Cancel Order
+### 4. Cancel Order
 Use `cancel` mothod of `BankIdClient` object to cancel the order.
 ```
 >>> bankid_client = BankIdClient()
 
 >>> bankid_client.auth('192.168.0.1')
 <class 'bankid6.handlers.BankIdStartResponse'> response status: 200
 response data: {"orderRef": "ccc9b028-4c83-49f8-b5ae-a3bac54a7427", "autoStartToken": "96c45dea-d14c-4bc5-bf30-db4015d39da9", "qrStartToken": "d550a68e-1e4d-4d66-8dce-3c6497c8da73", "qrStartSecret": "4b3bba21-ebaa-4bf4-8856-e66271550b78"}
@@ -293,16 +297,17 @@
 ```
 >>> start_response = BankIdClient().auth('192.168.0.1')
 >>> BankIdClient().auth(orderRef=start_response.orderRef)
 <class 'bankid6.handlers.BankIdCancelResponse'> response status: 200;
 response data: {}
 ```
 <br/>
+<br/>
 
-### Exceptions
+### 5. Exceptions
 
 All methods in `BankIdClient` can raise `BankIdError` or `BankIdValidationError`. 
 
 `BankIdError` is raised when a request is made to BankID server and it returned an error. It has `message` attribute with structure like:
 ```json
 {
     "swedish": "",
@@ -312,60 +317,64 @@
 If the message is available, it indicates that the message should be presented to the customer without any additional action required. Otherwise, the `reason` and `action` attributes can provide information on why the error occurred and what steps need to be taken to address it according to BankID documentation. Attribute `response_data` has the data received from bankid in dict format. See Api Reference section for more functionalities.
 
 
 `BankIdValidationError` is raised before sending the request to BankID if any parameter is invalid.
 
 <br/>
 <br/>
+<br/>
+<br/>
 
 ## API Reference
 
 
 #### class BankIdClient()
-<br/>
 
 ##### def __init__(self, prod_env: bool=False, cert_pem: str=None, key_pem: str=None, ca_pem: str=None, request_timeout: int=None, messages: Messages=Messages, is_mobile: bool=False)
 
 **Parameters:**
 - `prod_env` indicates if it's a production environment. Test or prod urls are chosen based on this. If it is `True` then `key_pem`, `cert_pem` and `ca_pem` are required. Otherwise test certificates which are already included in the package will be used. Any or all of the certificates can also be provided when the value is `False`
 - `cert_pem` file path of the certificate file
 - `key_pem` file path of the private key of the certificate.
 - `ca_pem` file path of CA certificate file
 - `request_timeout` number of seconds to wait for response
 - `messages` class or subclass of `Messages` class to override existing message
 - `is_mobile` if it's being used in a mobile device.
 <br/>
+<br/>
 
 ##### def auth(endUserIp: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None):
 
 Starts the bankid auth process. Use this when only user authentication is needed.
 
 **Parameters:**
 - `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 is allowed.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
+<br/>
 
 ##### def sign(endUserIp: str, userVisibleData: str, requirement: dict=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)
 
 Starts the bankid sign process. Use this when user is authenticated to sign something.
 
 **Parameters:**
 - `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 is allowed.
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
+<br/>
 
 ##### def phone_auth(personalNumber: str, callInitiator: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)
 
 Initiates an authentication order when the user is talking to the RP over the phone. 
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
@@ -373,14 +382,15 @@
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
+<br/>
 
 ##### def phone_sign(personalNumber, callInitiator, userVisibleData, requirement=None, userNonVisibleData=None, userVisibleDataFormat=None)
 
 Initiates an signing order when the user is talking to the RP over the phone.
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
@@ -388,61 +398,71 @@
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
+<br/>
 
 ##### def collect(orderRef: str=None, qrStartToken: str=None, qrStartSecret: str=None, order_time: int=None)
 
 Collect the result of the `auth`, `sign`, `phone_auth` or `phone_sign` methods. If used from same client instance when order was initiated, it doesn't require any parameters
 
 - `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then corresponding order result will be requested. Usefull when the method is being used from different client instance than where the order was started.
 - `qrStartToken` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `qrStartSecret` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `order_time` *Optional*. *int*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 
 **Return:** `BankIdCollectResponse`
 <br/>
+<br/>
 
 ##### def cancel(orderRef: str=None):
 
 Cancels an ongoing sign or auth order. If used from same client instance when order was initiated, it doesn't require any parameters
 
 - `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then corresponding order result will be requested. Usefull when the method is being used from different client instance than where the order was started.
 
 **Return:** `BankIdCancelResponse`
 
 <br/>
+<br/>
+<br/>
 
 ### class BankIdBaseResponse()
 
 `response`: *requests.Response*. object which was returned from sending the request.
 `status`: *int*. Http response code of the response
 `data`: *dict*. returned data in dict format
 `url`: *str*. The full url where the request was sent
 
 <br/>
+<br/>
+<br/>
 
 ### class BankIdStartResponse(BankIdBaseResponse):
 
 `orderRef`: *str*. Used to collect the status of the order. Parsed from BankID response.
 `autoStartToken`: *str*. Used to compile the start url. Parsed from BankID response.
 `qrStartToken`: *str*. Used to compute the animated QR code. Parsed from BankID response.
 `qrStartSecret`: *str*. Used to compute the animated QR code. Parsed from BankID response.
 `order_time`: *int*. order time in seconds since the Epoch.
 
 <br/>
+<br/>
+<br/>
 
 ### class BankIdPhoneStartResponse(BankIdBaseResponse):
 
 `orderRef`: *str*. Used to collect the status of the order. Parsed from BankID response.
 
 <br/>
+<br/>
+<br/>
 
 ### class BankIdCollectResponse(BankIdBaseResponse)
 
 `orderRef`: *str*. Used to collect the status of the order. Parsed from BankID response.
 `status`: *str*. 'pending' | 'complete' | 'failed'. Parsed from BankID response.
 `hintCode`: *str*. Only present for pending and failed orders. Parsed from BankID response.
 `completionData`: *BankIdCompletionData*. Only present for complete orders. Parsed from BankID response.
@@ -455,50 +475,59 @@
     },
     "onfile": {             # order initiated by starting the bankid app on the same device
         "swedish": "",
         "english": ""
     }
 } 
 ```
+<br/>
 
 ##### class BankIdCompletionData()
 `user`: *BankIdCompletionUserData*. Authenticated user information.
 `device`: *BankIdCompletionDeviceData*. Authenticated user's device information.
 `bankIdIssueDate`: *datatime*. The date the BankID was issued to the user.
 `stepUp`: *str*. Information about extra verifications that were part of the transaction.
 `signature`: *str*. The signature as described in the BankID Signature Profile specification. Base64-encoded.
 `ocspResponse`: *str*. The OCSP response. Base64-encoded. The OCSP response is signed by a certificate that has the same issuer as the certificate being verified. The OSCP response has an extension for Nonce. The nonce is calculated as:
 - SHA-1 hash over the base 64 XML signature encoded as UTF-8.
 - 12 random bytes is added after the hash.
 - The nonce is 32 bytes (20 + 12).
 `json`: *dict*. Completion data in dict format.
+<br/>
 
 ##### class BankIdCompletionUserData()
 `personalNumber`: *str*. The personal identity number.
 `name`: *str*. The given name and surname of the user.
 `givenName`: *str*. The given name of the user.
 `surname`: *str*. The surname of the user.
+<br/>
 
 ##### class BankIdCompletionDeviceData()
 `ipAddress`: *str*. The IP address of the user agent as the BankID server discovers it. When an order is started with autoStartToken the RP can check that this match the IP they observe to ensure session fixation String.
 `uhi`: *str*. Unique hardware identifier for the users device.
 
 <br/>
+<br/>
+<br/>
 
 #### class BankIdCancelResponse(BankIdBaseResponse)
 ***...***
 
 <br/>
+<br/>
+<br/>
 
 #### class BankIdError(Exception)
 `reason`: *str*. Reason of the exception according to BankID Documentation
 `action`: *str*. What action is needed for this exception according to BankID Documentation
 `message`: *dict*. Message for user.
 `errorCode`: *str*. Error code received in response data
 `response`: *requests.Response*. object which was returned from sending the request.
 `response_status`: *int*. Http response code of the response
 `response_data`: *dict*. returned data in dict format
 
 <br/>
+<br/>
+<br/>
 
 #### class BankIdValidationError(Exception)
 ***...***
```

### Comparing `bankid6-1.0.1/pyproject.toml` & `bankid6-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bankid6"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Amir Ebrahim", email="md.amire02@gmail.com" },
 ]
 description = """
   A complete implementation of swedish BankID version 6. 
   Easily initiate, collect and cancel authentication orders, 
   show user message and handle errors.
```

### Comparing `bankid6-1.0.1/PKG-INFO` & `bankid6-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bankid6
-Version: 1.0.1
+Version: 1.0.2
 Summary:   A complete implementation of swedish BankID version 6.    Easily initiate, collect and cancel authentication orders,    show user message and handle errors.
 Author-email: Amir Ebrahim <md.amire02@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -15,14 +15,15 @@
 
 <br/>
 
 ## Overview
 
 A complete implementation of swedish BankID authentication system version 6. It includes initiating/collect/cancel authentication order, User Message and exceptaion handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
 <br/>
+<br/>
 
 ## Installation
 
 ```
 pip install bankid6
 ```
 Supports python version 3.6 and later.
@@ -127,15 +128,15 @@
 ```
 
 <br/>
 <br/>
 
 ## User Guide
 
-### Instantiate `BankIdClient` Class
+### 1. Instantiate `BankIdClient` Class
 
 `BankIdClient` provides functionality to initiate authentication or signing order, collect order result or cancel the order.
 
 Instantiate for `BankIdClient` for test environment.
 ```
 >>> from bankid6 import BankIdClient
 >>> bankid_client = BankIdClient()
@@ -147,16 +148,17 @@
 <br/>
 
 To initialize for a production environment, ensure that the `prod_env` parameter is set to `True`. Additionally, you must provide the file paths for the certificate, the private key associated with the certificate, and the CA certificate.
 ```
 >>> bankid_client = BankIdClient(prod_env=True, cert_pem=<certificate_filepath>, key_pem='<private_key_filepath>', ca_pem=<ca_certificate_filepath>)
 ```
 <br/>
+<br/>
 
-### Initiate Authentication or Signing Order
+### 2. Initiate Authentication or Signing Order
 
 The `BankIdClient` offers `auth` and `sign` methods to initiate authentication and signing orders, respectively. These methods return a `BankIdStartResponse` object, which contains attributes to easily get the data for QR code and url for launching the BankID app.
 
 ```
 >>> bankid_client = BankIdClient()
 >>> start_response = bankid_client.auth('192.168.0.1')      # Takes IP of end user
 
@@ -197,16 +199,17 @@
 
 These methods have required or optional parameters exactly as described in BankID documentation. These parameters are validated, processed as BankID requires and sent as the data of the request to the BankID.
 
 The returned objects are derived from `BankIdBaseResponse`, parses any BankID response, creating an attribute with the same name as the key of the response data. `BankIdBaseResponse` has attributes related to actual HTTP response. This is also True for `collect` or `cancel`.
 
 See the API Reference section for comprehensive documentation detailing parameters and return values.
 <br/>
+<br/>
 
-### Collect Order Result
+### 3. Collect Order Result
 
 Use `collect` method of `BankIdClient` object to get the order result.
 ```
 >>> from bankid6 import BankIdClient
 >>> bankid_client = BankIdClient()
 
 >>> bankid_client.auth('192.168.0.1')
@@ -282,16 +285,17 @@
     RFA1 = {'test': 'yes'}
     RFA13 = ('<h3>swedish message<h3>', '<h3>english message</h3>')
 
 bankid_client = BankIdClient(messages=MyMessage)
 ```
 Their value can be a dict or a tuple of swedish and english messages. If the value is dict, it is returned as it is from `message` attribute of `BankIdCollectResponse` object.
 <br/>
+<br/>
 
-### Cancel Order
+### 4. Cancel Order
 Use `cancel` mothod of `BankIdClient` object to cancel the order.
 ```
 >>> bankid_client = BankIdClient()
 
 >>> bankid_client.auth('192.168.0.1')
 <class 'bankid6.handlers.BankIdStartResponse'> response status: 200
 response data: {"orderRef": "ccc9b028-4c83-49f8-b5ae-a3bac54a7427", "autoStartToken": "96c45dea-d14c-4bc5-bf30-db4015d39da9", "qrStartToken": "d550a68e-1e4d-4d66-8dce-3c6497c8da73", "qrStartSecret": "4b3bba21-ebaa-4bf4-8856-e66271550b78"}
@@ -306,16 +310,17 @@
 ```
 >>> start_response = BankIdClient().auth('192.168.0.1')
 >>> BankIdClient().auth(orderRef=start_response.orderRef)
 <class 'bankid6.handlers.BankIdCancelResponse'> response status: 200;
 response data: {}
 ```
 <br/>
+<br/>
 
-### Exceptions
+### 5. Exceptions
 
 All methods in `BankIdClient` can raise `BankIdError` or `BankIdValidationError`. 
 
 `BankIdError` is raised when a request is made to BankID server and it returned an error. It has `message` attribute with structure like:
 ```json
 {
     "swedish": "",
@@ -325,60 +330,64 @@
 If the message is available, it indicates that the message should be presented to the customer without any additional action required. Otherwise, the `reason` and `action` attributes can provide information on why the error occurred and what steps need to be taken to address it according to BankID documentation. Attribute `response_data` has the data received from bankid in dict format. See Api Reference section for more functionalities.
 
 
 `BankIdValidationError` is raised before sending the request to BankID if any parameter is invalid.
 
 <br/>
 <br/>
+<br/>
+<br/>
 
 ## API Reference
 
 
 #### class BankIdClient()
-<br/>
 
 ##### def __init__(self, prod_env: bool=False, cert_pem: str=None, key_pem: str=None, ca_pem: str=None, request_timeout: int=None, messages: Messages=Messages, is_mobile: bool=False)
 
 **Parameters:**
 - `prod_env` indicates if it's a production environment. Test or prod urls are chosen based on this. If it is `True` then `key_pem`, `cert_pem` and `ca_pem` are required. Otherwise test certificates which are already included in the package will be used. Any or all of the certificates can also be provided when the value is `False`
 - `cert_pem` file path of the certificate file
 - `key_pem` file path of the private key of the certificate.
 - `ca_pem` file path of CA certificate file
 - `request_timeout` number of seconds to wait for response
 - `messages` class or subclass of `Messages` class to override existing message
 - `is_mobile` if it's being used in a mobile device.
 <br/>
+<br/>
 
 ##### def auth(endUserIp: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None):
 
 Starts the bankid auth process. Use this when only user authentication is needed.
 
 **Parameters:**
 - `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 is allowed.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
+<br/>
 
 ##### def sign(endUserIp: str, userVisibleData: str, requirement: dict=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)
 
 Starts the bankid sign process. Use this when user is authenticated to sign something.
 
 **Parameters:**
 - `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 is allowed.
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
+<br/>
 
 ##### def phone_auth(personalNumber: str, callInitiator: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)
 
 Initiates an authentication order when the user is talking to the RP over the phone. 
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
@@ -386,14 +395,15 @@
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
+<br/>
 
 ##### def phone_sign(personalNumber, callInitiator, userVisibleData, requirement=None, userNonVisibleData=None, userVisibleDataFormat=None)
 
 Initiates an signing order when the user is talking to the RP over the phone.
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
@@ -401,61 +411,71 @@
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
+<br/>
 
 ##### def collect(orderRef: str=None, qrStartToken: str=None, qrStartSecret: str=None, order_time: int=None)
 
 Collect the result of the `auth`, `sign`, `phone_auth` or `phone_sign` methods. If used from same client instance when order was initiated, it doesn't require any parameters
 
 - `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then corresponding order result will be requested. Usefull when the method is being used from different client instance than where the order was started.
 - `qrStartToken` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `qrStartSecret` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `order_time` *Optional*. *int*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 
 **Return:** `BankIdCollectResponse`
 <br/>
+<br/>
 
 ##### def cancel(orderRef: str=None):
 
 Cancels an ongoing sign or auth order. If used from same client instance when order was initiated, it doesn't require any parameters
 
 - `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then corresponding order result will be requested. Usefull when the method is being used from different client instance than where the order was started.
 
 **Return:** `BankIdCancelResponse`
 
 <br/>
+<br/>
+<br/>
 
 ### class BankIdBaseResponse()
 
 `response`: *requests.Response*. object which was returned from sending the request.
 `status`: *int*. Http response code of the response
 `data`: *dict*. returned data in dict format
 `url`: *str*. The full url where the request was sent
 
 <br/>
+<br/>
+<br/>
 
 ### class BankIdStartResponse(BankIdBaseResponse):
 
 `orderRef`: *str*. Used to collect the status of the order. Parsed from BankID response.
 `autoStartToken`: *str*. Used to compile the start url. Parsed from BankID response.
 `qrStartToken`: *str*. Used to compute the animated QR code. Parsed from BankID response.
 `qrStartSecret`: *str*. Used to compute the animated QR code. Parsed from BankID response.
 `order_time`: *int*. order time in seconds since the Epoch.
 
 <br/>
+<br/>
+<br/>
 
 ### class BankIdPhoneStartResponse(BankIdBaseResponse):
 
 `orderRef`: *str*. Used to collect the status of the order. Parsed from BankID response.
 
 <br/>
+<br/>
+<br/>
 
 ### class BankIdCollectResponse(BankIdBaseResponse)
 
 `orderRef`: *str*. Used to collect the status of the order. Parsed from BankID response.
 `status`: *str*. 'pending' | 'complete' | 'failed'. Parsed from BankID response.
 `hintCode`: *str*. Only present for pending and failed orders. Parsed from BankID response.
 `completionData`: *BankIdCompletionData*. Only present for complete orders. Parsed from BankID response.
@@ -468,50 +488,59 @@
     },
     "onfile": {             # order initiated by starting the bankid app on the same device
         "swedish": "",
         "english": ""
     }
 } 
 ```
+<br/>
 
 ##### class BankIdCompletionData()
 `user`: *BankIdCompletionUserData*. Authenticated user information.
 `device`: *BankIdCompletionDeviceData*. Authenticated user's device information.
 `bankIdIssueDate`: *datatime*. The date the BankID was issued to the user.
 `stepUp`: *str*. Information about extra verifications that were part of the transaction.
 `signature`: *str*. The signature as described in the BankID Signature Profile specification. Base64-encoded.
 `ocspResponse`: *str*. The OCSP response. Base64-encoded. The OCSP response is signed by a certificate that has the same issuer as the certificate being verified. The OSCP response has an extension for Nonce. The nonce is calculated as:
 - SHA-1 hash over the base 64 XML signature encoded as UTF-8.
 - 12 random bytes is added after the hash.
 - The nonce is 32 bytes (20 + 12).
 `json`: *dict*. Completion data in dict format.
+<br/>
 
 ##### class BankIdCompletionUserData()
 `personalNumber`: *str*. The personal identity number.
 `name`: *str*. The given name and surname of the user.
 `givenName`: *str*. The given name of the user.
 `surname`: *str*. The surname of the user.
+<br/>
 
 ##### class BankIdCompletionDeviceData()
 `ipAddress`: *str*. The IP address of the user agent as the BankID server discovers it. When an order is started with autoStartToken the RP can check that this match the IP they observe to ensure session fixation String.
 `uhi`: *str*. Unique hardware identifier for the users device.
 
 <br/>
+<br/>
+<br/>
 
 #### class BankIdCancelResponse(BankIdBaseResponse)
 ***...***
 
 <br/>
+<br/>
+<br/>
 
 #### class BankIdError(Exception)
 `reason`: *str*. Reason of the exception according to BankID Documentation
 `action`: *str*. What action is needed for this exception according to BankID Documentation
 `message`: *dict*. Message for user.
 `errorCode`: *str*. Error code received in response data
 `response`: *requests.Response*. object which was returned from sending the request.
 `response_status`: *int*. Http response code of the response
 `response_data`: *dict*. returned data in dict format
 
 <br/>
+<br/>
+<br/>
 
 #### class BankIdValidationError(Exception)
 ***...***
```

