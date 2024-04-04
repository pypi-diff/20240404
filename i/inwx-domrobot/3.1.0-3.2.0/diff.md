# Comparing `tmp/inwx-domrobot-3.1.0.tar.gz` & `tmp/inwx-domrobot-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inwx-domrobot-3.1.0.tar", last modified: Tue Apr 21 18:09:32 2020, max compression
+gzip compressed data, was "inwx-domrobot-3.2.0.tar", last modified: Thu Apr  4 11:23:27 2024, max compression
```

## Comparing `inwx-domrobot-3.1.0.tar` & `inwx-domrobot-3.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/INWX/
--rw-rw-r--   0 nick      (1000) nick      (1000)     6614 2020-04-21 18:05:14.000000 inwx-domrobot-3.1.0/INWX/Domrobot.py
--rw-rw-r-x   0 nick      (1000) nick      (1000)       45 2020-01-13 07:08:22.000000 inwx-domrobot-3.1.0/INWX/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3838 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/PKG-INFO
--rw-rw-r-x   0 nick      (1000) nick      (1000)     2313 2020-01-13 07:08:22.000000 inwx-domrobot-3.1.0/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/inwx_domrobot.egg-info/
--rw-rw-r-x   0 nick      (1000) nick      (1000)     3838 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/inwx_domrobot.egg-info/PKG-INFO
--rw-rw-r-x   0 nick      (1000) nick      (1000)      246 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/inwx_domrobot.egg-info/SOURCES.txt
--rw-rw-r-x   0 nick      (1000) nick      (1000)        1 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/inwx_domrobot.egg-info/dependency_links.txt
--rw-rw-r-x   0 nick      (1000) nick      (1000)        9 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/inwx_domrobot.egg-info/requires.txt
--rw-rw-r-x   0 nick      (1000) nick      (1000)        5 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/inwx_domrobot.egg-info/top_level.txt
--rw-rw-r-x   0 nick      (1000) nick      (1000)       79 2020-04-21 18:09:32.000000 inwx-domrobot-3.1.0/setup.cfg
--rw-rw-r-x   0 nick      (1000) nick      (1000)     1334 2020-04-21 18:05:14.000000 inwx-domrobot-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:23:27.531854 inwx-domrobot-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:23:27.531854 inwx-domrobot-3.2.0/INWX/
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-04 11:23:23.000000 inwx-domrobot-3.2.0/INWX/Domrobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 11:23:23.000000 inwx-domrobot-3.2.0/INWX/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-04 11:23:23.000000 inwx-domrobot-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-04 11:23:27.531854 inwx-domrobot-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-04 11:23:23.000000 inwx-domrobot-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:23:27.531854 inwx-domrobot-3.2.0/inwx_domrobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-04 11:23:27.000000 inwx-domrobot-3.2.0/inwx_domrobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-04 11:23:27.000000 inwx-domrobot-3.2.0/inwx_domrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:23:27.000000 inwx-domrobot-3.2.0/inwx_domrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 11:23:27.000000 inwx-domrobot-3.2.0/inwx_domrobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 11:23:27.000000 inwx-domrobot-3.2.0/inwx_domrobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 11:23:27.531854 inwx-domrobot-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-04 11:23:23.000000 inwx-domrobot-3.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `inwx-domrobot-3.1.0/INWX/Domrobot.py` & `inwx-domrobot-3.2.0/INWX/Domrobot.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,35 +6,32 @@
 import string
 import struct
 import sys
 import time
 
 import requests
 
-if sys.version_info.major == 3:
-    import xmlrpc.client
-else:
-    import xmlrpclib
+import xmlrpc.client
 
 
 class ApiType:
     XML_RPC = '/xmlrpc/'
     JSON_RPC = '/jsonrpc/'
 
     def __init__(self):
         pass
 
 
 class ApiClient:
-    CLIENT_VERSION = '3.1.0'
+    CLIENT_VERSION = '3.1.1'
     API_LIVE_URL = 'https://api.domrobot.com'
     API_OTE_URL = 'https://api.ote.domrobot.com'
 
-    def __init__(self, api_url=API_OTE_URL, api_type=ApiType.XML_RPC, language='en', client_transaction_id=None,
-                 debug_mode=False):
+    def __init__(self, api_url: str = API_OTE_URL, api_type=ApiType.XML_RPC, language: str = 'en',
+                 client_transaction_id: str = None, debug_mode: bool = False):
         """
         Args:
             api_url: Url of the api.
             api_type: Type of the api. See ApiType class for all types.
             language: Language for api messages and error codes in responses.
             client_transaction_id: Sent with every request to distinguish your api requests in case you need support.
             debug_mode: Whether requests and responses should be printed out.
@@ -44,24 +41,27 @@
         self.api_type = api_type
         self.language = language
         self.client_transaction_id = client_transaction_id
         self.debug_mode = debug_mode
         self.customer = None
         self.api_session = requests.Session()
 
-    def login(self, username, password, shared_secret=None):
+    def login(self, username: str, password: str, shared_secret: str = None, tfa_token: str = None) -> dict:
         """Performs a login at the api and saves the session cookie for following api calls.
 
         Args:
             username: Your username.
             password: Your password.
             shared_secret: A secret used to generate a secret code to solve 2fa challenges when 2fa is enabled. This is
                 the code/string encoded in the QR-Code you scanned with your google authenticator app when you enabled 2fa.
                 If you don't have this secret anymore, disable and re-enable 2fa for your account but this time save the
                 code/string encoded in the QR-Code.
+            tfa_token: The current (time-based) 2fa code for this account if 2fa is enabled. Usually a 6-digit number.
+                Instead of this, you can also provide shared_secret to have the token calculated automatically.
+                tfa_token is ignored if shared_secret is given.
         Returns:
             The api response body parsed as a dict.
         Raises:
             Exception: Username and password must not be None.
             Exception: Api requests two factor challenge but no shared secret is given. Aborting.
         """
 
@@ -72,17 +72,20 @@
             'lang': self.language,
             'user': username,
             'pass': password
         }
 
         login_result = self.call_api('account.login', params)
         if login_result['code'] == 1000 and 'tfa' in login_result['resData'] and login_result['resData']['tfa'] != '0':
-            if shared_secret is None:
-                raise Exception('Api requests two factor challenge but no shared secret is given. Aborting.')
-            secret_code = self.get_secret_code(shared_secret)
+            if shared_secret is not None:
+                secret_code = self.get_secret_code(shared_secret)
+            elif tfa_token is not None:
+                secret_code = tfa_token
+            else:
+                raise Exception('Api requests two factor challenge but neither shared secret nor current token is given. Aborting.')
             unlock_result = self.call_api('account.unlock', {'tan': secret_code})
             if unlock_result['code'] != 1000:
                 return unlock_result
 
         return login_result
 
     def logout(self):
@@ -93,15 +96,15 @@
         """
 
         logout_result = self.call_api('account.logout')
         self.api_session.close()
         self.api_session = requests.Session()
         return logout_result
 
-    def call_api(self, api_method, method_params=None):
+    def call_api(self, api_method: str, method_params: dict = None) -> dict:
         """Makes an api call.
 
         Args:
             api_method: The name of the method called in the api.
             method_params: A dict of parameters added to the request.
         Returns:
             The api response body parsed as a dict.
@@ -117,46 +120,41 @@
 
         if self.customer:
             method_params['subuser'] = self.customer
         if self.client_transaction_id is not None:
             method_params['clTRID'] = self.client_transaction_id
 
         if self.api_type == ApiType.XML_RPC:
-            if sys.version_info.major == 3:
-                payload = xmlrpc.client.dumps((method_params,), api_method, encoding='UTF-8').replace('\n', '')
-            else:
-                payload = xmlrpclib.dumps((method_params,), api_method, encoding='UTF-8').replace('\n', '')
+            payload = xmlrpc.client.dumps((method_params,), api_method, encoding='UTF-8').replace('\n', '')
         elif self.api_type == ApiType.JSON_RPC:
             payload = str(json.dumps({'method': api_method, 'params': method_params}))
         else:
             raise Exception('Invalid ApiType.')
 
+        request_mime_type = 'application/json' if self.api_type == ApiType.JSON_RPC else 'text/xml'
         headers = {
-            'Content-Type': 'text/xml; charset=UTF-8',
+            'Content-Type': '{}; charset=UTF-8'.format(request_mime_type),
             'User-Agent': 'DomRobot/' + ApiClient.CLIENT_VERSION + ' (Python ' + self.get_python_version() + ')'
         }
 
         response = self.api_session.post(self.api_url + self.api_type, data=payload.encode('UTF-8'),
                                          headers=headers)
         response.raise_for_status()
 
         if self.debug_mode:
             print('Request (' + api_method + '): ' + payload)
             print('Response (' + api_method + '): ' + response.text)
 
         if self.api_type == ApiType.XML_RPC:
-            if sys.version_info.major == 3:
-                return xmlrpc.client.loads(response.text)[0][0]
-            else:
-                return xmlrpclib.loads(response.text)[0][0]
+            return xmlrpc.client.loads(response.text)[0][0]
         elif self.api_type == ApiType.JSON_RPC:
             return response.json()
 
     @staticmethod
-    def get_secret_code(shared_secret):
+    def get_secret_code(shared_secret: str) -> str:
         """Generates a secret code for 2fa with a shared secret.
 
         Args:
             shared_secret: The shared secret used to generate the secret code.
         Returns:
             A secret code used to solve 2fa challenges.
         Raises:
@@ -165,18 +163,21 @@
 
         if shared_secret is None:
             raise Exception('Shared secret must not be None.')
 
         key = base64.b32decode(shared_secret, True)
         msg = struct.pack(">Q", int(time.time()) // 30)
         hmac_hash = hmac.new(key, msg, hashlib.sha1).digest()
-        o = hmac_hash[19] & 15
+        if sys.version_info.major == 3:
+            o = hmac_hash[19] & 15
+        else:
+            o = ord(hmac_hash[19]) & 15
         hmac_hash = (struct.unpack(">I", hmac_hash[o:o + 4])[0] & 0x7fffffff) % 1000000
         return hmac_hash
 
     @staticmethod
-    def get_random_string(size=12):
+    def get_random_string(size: int = 12) -> str:
         return ''.join(random.choice(string.ascii_letters + string.digits) for x in range(size))
 
     @staticmethod
-    def get_python_version():
+    def get_python_version() -> str:
         return '.'.join(tuple(str(x) for x in sys.version_info))
```

### Comparing `inwx-domrobot-3.1.0/PKG-INFO` & `inwx-domrobot-3.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,90 @@
 Metadata-Version: 2.1
 Name: inwx-domrobot
-Version: 3.1.0
+Version: 3.2.0
 Summary: INWX API Python Client
 Home-page: https://github.com/inwx/python-client
+Download-URL: https://github.com/inwx/python-client/archive/v3.2.0.tar.gz
 Author: INWX Developer
 Author-email: developer@inwx.de
-License: UNKNOWN
-Download-URL: https://github.com/inwx/python-client/archive/v3.1.0.tar.gz
-Description: <p align="center">
-          <a href="https://www.inwx.com/en/" target="_blank">
-            <img src="https://images.inwx.com/logos/inwx.png">
-          </a>
-        </p>
-        
-        INWX Domrobot Python 3 Client
-        =========
-        You can access all functions of our frontend via our API, which is available via the XML-RPC or JSON-RPC protocol and thus can be easily consumed with all programming languages.
-        
-        There is also an OT&E test system, which you can access via [ote.inwx.com](https://ote.inwx.com/en/). Here you will find the known web interface which is using a test database. On the OT&E system no actions will be charged. So you can test as much as you like there.
-        
-        Documentation
-        ------
-        You can view a detailed description of the API functions in our documentation. You can find the online documentation [by clicking here](https://www.inwx.de/en/help/apidoc).
-        
-        If you still experience any kind of problems don't hesitate to contact our [support via email](mailto:support@inwx.de).
-        
-        Installation
-        -------
-        The recommended way is via pip:
-        
-        ```bash
-        pip install inwx-domrobot
-        ```
-        
-        You can find more information about the package on [pypi.org](https://pypi.org/project/inwx-domrobot).
-        
-        Example
-        -------
-        
-        ```python
-        from INWX.Domrobot import ApiClient
-        
-        username = ''
-        password = ''
-        domain = 'my-test-domain-which-is-definitely-not-registered6737.com'
-        
-        api_client = ApiClient(api_url=ApiClient.API_OTE_URL, debug_mode=True)
-        
-        login_result = api_client.login(username, password)
-        
-        if login_result['code'] == 1000:
-            domain_check_result = api_client.call_api(api_method='domain.check', method_params={'domain': domain})
-        
-            if domain_check_result['code'] == 1000:
-                checked_domain = domain_check_result['resData']['domain'][0]
-        
-                if checked_domain['avail']:
-                    print(domain + ' is still available!')
-                else:
-                    print('Unfortunately, ' + domain + ' is already registered.')
-        
-            else:
-                raise Exception('Api error while checking domain status. Code: ' + str(domain_check_result['code'])
-                                + '  Message: ' + domain_check_result['msg'])
-            api_client.logout()
-        else:
-            raise Exception('Api login error. Code: ' + str(login_result['code']) + '  Message: ' + login_result['msg'])
-        ```
-        
-        You can also have a look at the [example folder](INWX/examples) in the project for even more info.
-        
-        License
-        ----
-        
-        MIT
-        
 Keywords: INWX,API,PYTHON,CLIENT,DOMROBOT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+<p align="center">
+  <a href="https://www.inwx.com/en/" target="_blank">
+    <img src="https://images.inwx.com/logos/inwx.png">
+  </a>
+</p>
+
+INWX Domrobot Python 3 Client
+=========
+You can access all functions of our frontend via our API, which is available via the XML-RPC or JSON-RPC protocol and thus can be easily consumed with all programming languages.
+
+There is also an OT&E test system, which you can access via [ote.inwx.com](https://ote.inwx.com/en/). Here you will find the known web interface which is using a test database. On the OT&E system no actions will be charged. So you can test as much as you like there.
+
+Documentation
+------
+You can view a detailed description of the API functions in our documentation. You can find the online documentation [by clicking here](https://www.inwx.de/en/help/apidoc).
+
+If you still experience any kind of problems don't hesitate to contact our [support via email](mailto:support@inwx.de).
+
+Installation
+-------
+The recommended way is via pip:
+
+```bash
+pip install inwx-domrobot
+```
+
+You can find more information about the package on [pypi.org](https://pypi.org/project/inwx-domrobot).
+
+Example
+-------
+
+```python
+from INWX.Domrobot import ApiClient
+
+username = ''
+password = ''
+domain = 'my-test-domain-which-is-definitely-not-registered6737.com'
+
+api_client = ApiClient(api_url=ApiClient.API_OTE_URL, debug_mode=True)
+
+login_result = api_client.login(username, password)
+
+if login_result['code'] == 1000:
+    domain_check_result = api_client.call_api(api_method='domain.check', method_params={'domain': domain})
+
+    if domain_check_result['code'] == 1000:
+        checked_domain = domain_check_result['resData']['domain'][0]
+
+        if checked_domain['avail']:
+            print(domain + ' is still available!')
+        else:
+            print('Unfortunately, ' + domain + ' is already registered.')
+
+    else:
+        raise Exception('Api error while checking domain status. Code: ' + str(domain_check_result['code'])
+                        + '  Message: ' + domain_check_result['msg'])
+    api_client.logout()
+else:
+    raise Exception('Api login error. Code: ' + str(login_result['code']) + '  Message: ' + login_result['msg'])
+```
+
+You can also have a look at the [example folder](INWX/examples) in the project for even more info.
+
+License
+----
+
+MIT
```

#### html2text {}

```diff
@@ -1,11 +1,20 @@
-Metadata-Version: 2.1 Name: inwx-domrobot Version: 3.1.0 Summary: INWX API
-Python Client Home-page: https://github.com/inwx/python-client Author: INWX
-Developer Author-email: developer@inwx.de License: UNKNOWN Download-URL: https:
-//github.com/inwx/python-client/archive/v3.1.0.tar.gz Description:
+Metadata-Version: 2.1 Name: inwx-domrobot Version: 3.2.0 Summary: INWX API
+Python Client Home-page: https://github.com/inwx/python-client Download-URL:
+https://github.com/inwx/python-client/archive/v3.2.0.tar.gz Author: INWX
+Developer Author-email: developer@inwx.de Keywords:
+INWX,API,PYTHON,CLIENT,DOMROBOT Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
+:: Software Development Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests
                    _[_h_t_t_p_s_:_/_/_i_m_a_g_e_s_._i_n_w_x_._c_o_m_/_l_o_g_o_s_/_i_n_w_x_._p_n_g_]
 INWX Domrobot Python 3 Client ========= You can access all functions of our
 frontend via our API, which is available via the XML-RPC or JSON-RPC protocol
 and thus can be easily consumed with all programming languages. There is also
 an OT&E test system, which you can access via [ote.inwx.com](https://
 ote.inwx.com/en/). Here you will find the known web interface which is using a
 test database. On the OT&E system no actions will be charged. So you can test
@@ -26,17 +35,8 @@
 ['resData']['domain'][0] if checked_domain['avail']: print(domain + ' is still
 available!') else: print('Unfortunately, ' + domain + ' is already
 registered.') else: raise Exception('Api error while checking domain status.
 Code: ' + str(domain_check_result['code']) + ' Message: ' + domain_check_result
 ['msg']) api_client.logout() else: raise Exception('Api login error. Code: ' +
 str(login_result['code']) + ' Message: ' + login_result['msg']) ``` You can
 also have a look at the [example folder](INWX/examples) in the project for even
-more info. License ---- MIT Keywords: INWX,API,PYTHON,CLIENT,DOMROBOT Platform:
-UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
-Intended Audience :: Developers Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4 Classifier: Programming
-Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+more info. License ---- MIT
```

### Comparing `inwx-domrobot-3.1.0/README.md` & `inwx-domrobot-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `inwx-domrobot-3.1.0/inwx_domrobot.egg-info/PKG-INFO` & `inwx-domrobot-3.2.0/inwx_domrobot.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,90 @@
 Metadata-Version: 2.1
 Name: inwx-domrobot
-Version: 3.1.0
+Version: 3.2.0
 Summary: INWX API Python Client
 Home-page: https://github.com/inwx/python-client
+Download-URL: https://github.com/inwx/python-client/archive/v3.2.0.tar.gz
 Author: INWX Developer
 Author-email: developer@inwx.de
-License: UNKNOWN
-Download-URL: https://github.com/inwx/python-client/archive/v3.1.0.tar.gz
-Description: <p align="center">
-          <a href="https://www.inwx.com/en/" target="_blank">
-            <img src="https://images.inwx.com/logos/inwx.png">
-          </a>
-        </p>
-        
-        INWX Domrobot Python 3 Client
-        =========
-        You can access all functions of our frontend via our API, which is available via the XML-RPC or JSON-RPC protocol and thus can be easily consumed with all programming languages.
-        
-        There is also an OT&E test system, which you can access via [ote.inwx.com](https://ote.inwx.com/en/). Here you will find the known web interface which is using a test database. On the OT&E system no actions will be charged. So you can test as much as you like there.
-        
-        Documentation
-        ------
-        You can view a detailed description of the API functions in our documentation. You can find the online documentation [by clicking here](https://www.inwx.de/en/help/apidoc).
-        
-        If you still experience any kind of problems don't hesitate to contact our [support via email](mailto:support@inwx.de).
-        
-        Installation
-        -------
-        The recommended way is via pip:
-        
-        ```bash
-        pip install inwx-domrobot
-        ```
-        
-        You can find more information about the package on [pypi.org](https://pypi.org/project/inwx-domrobot).
-        
-        Example
-        -------
-        
-        ```python
-        from INWX.Domrobot import ApiClient
-        
-        username = ''
-        password = ''
-        domain = 'my-test-domain-which-is-definitely-not-registered6737.com'
-        
-        api_client = ApiClient(api_url=ApiClient.API_OTE_URL, debug_mode=True)
-        
-        login_result = api_client.login(username, password)
-        
-        if login_result['code'] == 1000:
-            domain_check_result = api_client.call_api(api_method='domain.check', method_params={'domain': domain})
-        
-            if domain_check_result['code'] == 1000:
-                checked_domain = domain_check_result['resData']['domain'][0]
-        
-                if checked_domain['avail']:
-                    print(domain + ' is still available!')
-                else:
-                    print('Unfortunately, ' + domain + ' is already registered.')
-        
-            else:
-                raise Exception('Api error while checking domain status. Code: ' + str(domain_check_result['code'])
-                                + '  Message: ' + domain_check_result['msg'])
-            api_client.logout()
-        else:
-            raise Exception('Api login error. Code: ' + str(login_result['code']) + '  Message: ' + login_result['msg'])
-        ```
-        
-        You can also have a look at the [example folder](INWX/examples) in the project for even more info.
-        
-        License
-        ----
-        
-        MIT
-        
 Keywords: INWX,API,PYTHON,CLIENT,DOMROBOT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+<p align="center">
+  <a href="https://www.inwx.com/en/" target="_blank">
+    <img src="https://images.inwx.com/logos/inwx.png">
+  </a>
+</p>
+
+INWX Domrobot Python 3 Client
+=========
+You can access all functions of our frontend via our API, which is available via the XML-RPC or JSON-RPC protocol and thus can be easily consumed with all programming languages.
+
+There is also an OT&E test system, which you can access via [ote.inwx.com](https://ote.inwx.com/en/). Here you will find the known web interface which is using a test database. On the OT&E system no actions will be charged. So you can test as much as you like there.
+
+Documentation
+------
+You can view a detailed description of the API functions in our documentation. You can find the online documentation [by clicking here](https://www.inwx.de/en/help/apidoc).
+
+If you still experience any kind of problems don't hesitate to contact our [support via email](mailto:support@inwx.de).
+
+Installation
+-------
+The recommended way is via pip:
+
+```bash
+pip install inwx-domrobot
+```
+
+You can find more information about the package on [pypi.org](https://pypi.org/project/inwx-domrobot).
+
+Example
+-------
+
+```python
+from INWX.Domrobot import ApiClient
+
+username = ''
+password = ''
+domain = 'my-test-domain-which-is-definitely-not-registered6737.com'
+
+api_client = ApiClient(api_url=ApiClient.API_OTE_URL, debug_mode=True)
+
+login_result = api_client.login(username, password)
+
+if login_result['code'] == 1000:
+    domain_check_result = api_client.call_api(api_method='domain.check', method_params={'domain': domain})
+
+    if domain_check_result['code'] == 1000:
+        checked_domain = domain_check_result['resData']['domain'][0]
+
+        if checked_domain['avail']:
+            print(domain + ' is still available!')
+        else:
+            print('Unfortunately, ' + domain + ' is already registered.')
+
+    else:
+        raise Exception('Api error while checking domain status. Code: ' + str(domain_check_result['code'])
+                        + '  Message: ' + domain_check_result['msg'])
+    api_client.logout()
+else:
+    raise Exception('Api login error. Code: ' + str(login_result['code']) + '  Message: ' + login_result['msg'])
+```
+
+You can also have a look at the [example folder](INWX/examples) in the project for even more info.
+
+License
+----
+
+MIT
```

#### html2text {}

```diff
@@ -1,11 +1,20 @@
-Metadata-Version: 2.1 Name: inwx-domrobot Version: 3.1.0 Summary: INWX API
-Python Client Home-page: https://github.com/inwx/python-client Author: INWX
-Developer Author-email: developer@inwx.de License: UNKNOWN Download-URL: https:
-//github.com/inwx/python-client/archive/v3.1.0.tar.gz Description:
+Metadata-Version: 2.1 Name: inwx-domrobot Version: 3.2.0 Summary: INWX API
+Python Client Home-page: https://github.com/inwx/python-client Download-URL:
+https://github.com/inwx/python-client/archive/v3.2.0.tar.gz Author: INWX
+Developer Author-email: developer@inwx.de Keywords:
+INWX,API,PYTHON,CLIENT,DOMROBOT Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
+:: Software Development Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests
                    _[_h_t_t_p_s_:_/_/_i_m_a_g_e_s_._i_n_w_x_._c_o_m_/_l_o_g_o_s_/_i_n_w_x_._p_n_g_]
 INWX Domrobot Python 3 Client ========= You can access all functions of our
 frontend via our API, which is available via the XML-RPC or JSON-RPC protocol
 and thus can be easily consumed with all programming languages. There is also
 an OT&E test system, which you can access via [ote.inwx.com](https://
 ote.inwx.com/en/). Here you will find the known web interface which is using a
 test database. On the OT&E system no actions will be charged. So you can test
@@ -26,17 +35,8 @@
 ['resData']['domain'][0] if checked_domain['avail']: print(domain + ' is still
 available!') else: print('Unfortunately, ' + domain + ' is already
 registered.') else: raise Exception('Api error while checking domain status.
 Code: ' + str(domain_check_result['code']) + ' Message: ' + domain_check_result
 ['msg']) api_client.logout() else: raise Exception('Api login error. Code: ' +
 str(login_result['code']) + ' Message: ' + login_result['msg']) ``` You can
 also have a look at the [example folder](INWX/examples) in the project for even
-more info. License ---- MIT Keywords: INWX,API,PYTHON,CLIENT,DOMROBOT Platform:
-UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
-Intended Audience :: Developers Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4 Classifier: Programming
-Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+more info. License ---- MIT
```

### Comparing `inwx-domrobot-3.1.0/setup.py` & `inwx-domrobot-3.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-version = '3.1.0'
+version = '3.2.0'
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
@@ -22,17 +22,15 @@
     keywords=['INWX', 'API', 'PYTHON', 'CLIENT', 'DOMROBOT'],
     install_requires=install_requires,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

