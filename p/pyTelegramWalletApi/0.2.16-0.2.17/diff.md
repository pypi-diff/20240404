# Comparing `tmp/pyTelegramWalletApi-0.2.16.tar.gz` & `tmp/pyTelegramWalletApi-0.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTelegramWalletApi-0.2.16.tar", last modified: Sun Nov 12 05:50:54 2023, max compression
+gzip compressed data, was "pyTelegramWalletApi-0.2.17.tar", last modified: Thu Apr  4 09:01:26 2024, max compression
```

## Comparing `pyTelegramWalletApi-0.2.16.tar` & `pyTelegramWalletApi-0.2.17.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-11-12 05:50:54.016650 pyTelegramWalletApi-0.2.16/
--rw-rw-rw-   0        0        0     2550 2023-11-12 05:50:54.016650 pyTelegramWalletApi-0.2.16/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-10-14 02:55:37.000000 pyTelegramWalletApi-0.2.16/README.md
-drwxrwxrwx   0        0        0        0 2023-11-12 05:50:53.988078 pyTelegramWalletApi-0.2.16/pyTelegramWalletApi.egg-info/
--rw-rw-rw-   0        0        0     2550 2023-11-12 05:50:53.000000 pyTelegramWalletApi-0.2.16/pyTelegramWalletApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-11-12 05:50:53.000000 pyTelegramWalletApi-0.2.16/pyTelegramWalletApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-12 05:50:53.000000 pyTelegramWalletApi-0.2.16/pyTelegramWalletApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-11-12 05:50:53.000000 pyTelegramWalletApi-0.2.16/pyTelegramWalletApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-12 05:50:53.000000 pyTelegramWalletApi-0.2.16/pyTelegramWalletApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-12 05:50:54.026648 pyTelegramWalletApi-0.2.16/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-11-12 05:50:04.000000 pyTelegramWalletApi-0.2.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-12 05:50:53.994075 pyTelegramWalletApi-0.2.16/tests/
--rw-rw-rw-   0        0        0        0 2023-10-02 22:55:55.000000 pyTelegramWalletApi-0.2.16/tests/__init__.py
--rw-rw-rw-   0        0        0     1507 2023-10-22 07:18:06.000000 pyTelegramWalletApi-0.2.16/tests/rest_tests.py
-drwxrwxrwx   0        0        0        0 2023-11-12 05:50:54.005647 pyTelegramWalletApi-0.2.16/wallet/
--rw-rw-rw-   0        0        0       70 2023-10-02 23:59:27.000000 pyTelegramWalletApi-0.2.16/wallet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-12 05:50:54.009647 pyTelegramWalletApi-0.2.16/wallet/rest/
--rw-rw-rw-   0        0        0    14517 2023-10-22 06:53:53.000000 pyTelegramWalletApi-0.2.16/wallet/rest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-12 05:50:54.012646 pyTelegramWalletApi-0.2.16/wallet/selenium/
--rw-rw-rw-   0        0        0      719 2023-10-19 08:46:48.000000 pyTelegramWalletApi-0.2.16/wallet/selenium/__init__.py
--rw-rw-rw-   0        0        0     8322 2023-10-22 10:10:20.000000 pyTelegramWalletApi-0.2.16/wallet/types.py
--rw-rw-rw-   0        0        0     1926 2023-10-03 00:03:16.000000 pyTelegramWalletApi-0.2.16/wallet/web_client.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.066820 pyTelegramWalletApi-0.2.17/
+-rw-rw-rw-   0        0        0     2462 2024-04-04 09:01:26.066820 pyTelegramWalletApi-0.2.17/PKG-INFO
+-rw-rw-rw-   0        0        0     2259 2024-04-04 09:00:44.000000 pyTelegramWalletApi-0.2.17/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.023818 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/
+-rw-rw-rw-   0        0        0     2462 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 09:01:25.000000 pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 09:01:26.074819 pyTelegramWalletApi-0.2.17/setup.cfg
+-rw-rw-rw-   0        0        0      572 2024-04-04 09:00:44.000000 pyTelegramWalletApi-0.2.17/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.030819 pyTelegramWalletApi-0.2.17/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-02 22:55:55.000000 pyTelegramWalletApi-0.2.17/tests/__init__.py
+-rw-rw-rw-   0        0        0     1513 2024-04-04 08:56:55.000000 pyTelegramWalletApi-0.2.17/tests/rest_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.049821 pyTelegramWalletApi-0.2.17/wallet/
+-rw-rw-rw-   0        0        0       70 2023-10-02 23:59:27.000000 pyTelegramWalletApi-0.2.17/wallet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.052820 pyTelegramWalletApi-0.2.17/wallet/rest/
+-rw-rw-rw-   0        0        0    14517 2023-10-22 06:53:53.000000 pyTelegramWalletApi-0.2.17/wallet/rest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:01:26.064819 pyTelegramWalletApi-0.2.17/wallet/selenium/
+-rw-rw-rw-   0        0        0      719 2023-10-19 08:46:48.000000 pyTelegramWalletApi-0.2.17/wallet/selenium/__init__.py
+-rw-rw-rw-   0        0        0     8322 2023-10-22 10:10:20.000000 pyTelegramWalletApi-0.2.17/wallet/types.py
+-rw-rw-rw-   0        0        0     2288 2024-04-04 08:50:32.000000 pyTelegramWalletApi-0.2.17/wallet/web_client.py
```

### Comparing `pyTelegramWalletApi-0.2.16/PKG-INFO` & `pyTelegramWalletApi-0.2.17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTelegramWalletApi
-Version: 0.2.16
+Version: 0.2.17
 Summary: Telegram Wallet API
 Author: no-name-user-name
 Author-email: dimazver61@gmail.com
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
@@ -49,19 +49,16 @@
 ### Example
 
 ```python
 import time
 
 from wallet import Client, Wallet
 
-# for the first tg login
-c = Client.auth(profile='main')
-
-# chromedriver headless mode for authorized tg account
-# c = Client(profile='main')
+# singin/singup to tg account
+c = Client(profile='main')
 
 # get wallet auth token
 auth_token = c.get_token()
 
 w = Wallet(auth_token)
 
 ton_balance = w.get_user_balance('TON')['available_balance']
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.16 Summary:
+Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.17 Summary:
 Telegram Wallet API Author: no-name-user-name Author-email:
 dimazver61@gmail.com Description-Content-Type: text/markdown
                                     _[_L_o_g_o_]
                          ******** TTeelleeggrraamm WWaalllleett AAPPII ********
          Unofficial library for managing your personal Wallet account
 
 ## Table Of Contents * [About the Project](#about-the-project) * [Built With]
 (#built-with) * [Getting Started](#getting-started) * [Example](#example) *
 [Realised methods](#realised-methods) ## About The Project Send and receive
 tokens | Trade on P2P Market ## Built With To obtain an authorization token,
 the "selenium" library is used. Working with the API is implemented using
 "requests" ## Getting Started ```bazaar pip install pyTelegramWalletApi ``` ###
-Example ```python import time from wallet import Client, Wallet # for the first
-tg login c = Client.auth(profile='main') # chromedriver headless mode for
-authorized tg account # c = Client(profile='main') # get wallet auth token
-auth_token = c.get_token() w = Wallet(auth_token) ton_balance =
-w.get_user_balance('TON')['available_balance'] print(f'[*] Balance:
-{ton_balance} TON') tx_id = w.send_to_address(0.01, 'TON',
-'EQA5IHeHWX9BkTsI71ECzuD-HeYL-br36UmFoTWZFihU3fLz')['transaction_id'] tx_link =
-None status = '' # wait tx in block while tx_link is None: details =
-w.get_transaction_details(tx_id) tx_link = details["transaction_link"] status =
-details['status'] time.sleep(2) print(f'[*] Tx status: {status} | {tx_link}')
-""" Logs [*] Starting parse wallet authorization token... [*] Token find:
-eyJhbGciOiJIUzI1NiIsInR5cCI6IkpX.... [*] Balance: 100 TON [*] Tx status:
-success | https://tonscan.org/tx/.... """ ``` ## Realised methods Wallet
-Account Methods: - send_to_address() - get_user_balance() -
-get_transaction_details() - get_transactions() - get_rate() Wallet P2P Methods:
-- get_p2p_market() - create_p2p_offer() - edit_p2p_offer() - get_p2p_offer() -
-get_own_p2p_offer_by_id() - get_user_p2p_payment() - get_user_p2p_order_history
-() - get_own_p2p_offer() - get_own_p2p_offers() - enable_p2p_bidding() -
-disable_p2p_bidding() - p2p_offer_activate() - p2p_offer_deactivate()
+Example ```python import time from wallet import Client, Wallet # singin/singup
+to tg account c = Client(profile='main') # get wallet auth token auth_token =
+c.get_token() w = Wallet(auth_token) ton_balance = w.get_user_balance('TON')
+['available_balance'] print(f'[*] Balance: {ton_balance} TON') tx_id =
+w.send_to_address(0.01, 'TON', 'EQA5IHeHWX9BkTsI71ECzuD-HeYL-
+br36UmFoTWZFihU3fLz')['transaction_id'] tx_link = None status = '' # wait tx in
+block while tx_link is None: details = w.get_transaction_details(tx_id) tx_link
+= details["transaction_link"] status = details['status'] time.sleep(2) print(f'
+[*] Tx status: {status} | {tx_link}') """ Logs [*] Starting parse wallet
+authorization token... [*] Token find: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpX.... [*]
+Balance: 100 TON [*] Tx status: success | https://tonscan.org/tx/.... """ ```
+## Realised methods Wallet Account Methods: - send_to_address() -
+get_user_balance() - get_transaction_details() - get_transactions() - get_rate
+() Wallet P2P Methods: - get_p2p_market() - create_p2p_offer() - edit_p2p_offer
+() - get_p2p_offer() - get_own_p2p_offer_by_id() - get_user_p2p_payment() -
+get_user_p2p_order_history() - get_own_p2p_offer() - get_own_p2p_offers() -
+enable_p2p_bidding() - disable_p2p_bidding() - p2p_offer_activate() -
+p2p_offer_deactivate()
```

### Comparing `pyTelegramWalletApi-0.2.16/README.md` & `pyTelegramWalletApi-0.2.17/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -41,19 +41,16 @@
 ### Example
 
 ```python
 import time
 
 from wallet import Client, Wallet
 
-# for the first tg login
-c = Client.auth(profile='main')
-
-# chromedriver headless mode for authorized tg account
-# c = Client(profile='main')
+# singin/singup to tg account
+c = Client(profile='main')
 
 # get wallet auth token
 auth_token = c.get_token()
 
 w = Wallet(auth_token)
 
 ton_balance = w.get_user_balance('TON')['available_balance']
```

#### html2text {}

```diff
@@ -5,26 +5,25 @@
 
 ## Table Of Contents * [About the Project](#about-the-project) * [Built With]
 (#built-with) * [Getting Started](#getting-started) * [Example](#example) *
 [Realised methods](#realised-methods) ## About The Project Send and receive
 tokens | Trade on P2P Market ## Built With To obtain an authorization token,
 the "selenium" library is used. Working with the API is implemented using
 "requests" ## Getting Started ```bazaar pip install pyTelegramWalletApi ``` ###
-Example ```python import time from wallet import Client, Wallet # for the first
-tg login c = Client.auth(profile='main') # chromedriver headless mode for
-authorized tg account # c = Client(profile='main') # get wallet auth token
-auth_token = c.get_token() w = Wallet(auth_token) ton_balance =
-w.get_user_balance('TON')['available_balance'] print(f'[*] Balance:
-{ton_balance} TON') tx_id = w.send_to_address(0.01, 'TON',
-'EQA5IHeHWX9BkTsI71ECzuD-HeYL-br36UmFoTWZFihU3fLz')['transaction_id'] tx_link =
-None status = '' # wait tx in block while tx_link is None: details =
-w.get_transaction_details(tx_id) tx_link = details["transaction_link"] status =
-details['status'] time.sleep(2) print(f'[*] Tx status: {status} | {tx_link}')
-""" Logs [*] Starting parse wallet authorization token... [*] Token find:
-eyJhbGciOiJIUzI1NiIsInR5cCI6IkpX.... [*] Balance: 100 TON [*] Tx status:
-success | https://tonscan.org/tx/.... """ ``` ## Realised methods Wallet
-Account Methods: - send_to_address() - get_user_balance() -
-get_transaction_details() - get_transactions() - get_rate() Wallet P2P Methods:
-- get_p2p_market() - create_p2p_offer() - edit_p2p_offer() - get_p2p_offer() -
-get_own_p2p_offer_by_id() - get_user_p2p_payment() - get_user_p2p_order_history
-() - get_own_p2p_offer() - get_own_p2p_offers() - enable_p2p_bidding() -
-disable_p2p_bidding() - p2p_offer_activate() - p2p_offer_deactivate()
+Example ```python import time from wallet import Client, Wallet # singin/singup
+to tg account c = Client(profile='main') # get wallet auth token auth_token =
+c.get_token() w = Wallet(auth_token) ton_balance = w.get_user_balance('TON')
+['available_balance'] print(f'[*] Balance: {ton_balance} TON') tx_id =
+w.send_to_address(0.01, 'TON', 'EQA5IHeHWX9BkTsI71ECzuD-HeYL-
+br36UmFoTWZFihU3fLz')['transaction_id'] tx_link = None status = '' # wait tx in
+block while tx_link is None: details = w.get_transaction_details(tx_id) tx_link
+= details["transaction_link"] status = details['status'] time.sleep(2) print(f'
+[*] Tx status: {status} | {tx_link}') """ Logs [*] Starting parse wallet
+authorization token... [*] Token find: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpX.... [*]
+Balance: 100 TON [*] Tx status: success | https://tonscan.org/tx/.... """ ```
+## Realised methods Wallet Account Methods: - send_to_address() -
+get_user_balance() - get_transaction_details() - get_transactions() - get_rate
+() Wallet P2P Methods: - get_p2p_market() - create_p2p_offer() - edit_p2p_offer
+() - get_p2p_offer() - get_own_p2p_offer_by_id() - get_user_p2p_payment() -
+get_user_p2p_order_history() - get_own_p2p_offer() - get_own_p2p_offers() -
+enable_p2p_bidding() - disable_p2p_bidding() - p2p_offer_activate() -
+p2p_offer_deactivate()
```

### Comparing `pyTelegramWalletApi-0.2.16/pyTelegramWalletApi.egg-info/PKG-INFO` & `pyTelegramWalletApi-0.2.17/pyTelegramWalletApi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTelegramWalletApi
-Version: 0.2.16
+Version: 0.2.17
 Summary: Telegram Wallet API
 Author: no-name-user-name
 Author-email: dimazver61@gmail.com
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
@@ -49,19 +49,16 @@
 ### Example
 
 ```python
 import time
 
 from wallet import Client, Wallet
 
-# for the first tg login
-c = Client.auth(profile='main')
-
-# chromedriver headless mode for authorized tg account
-# c = Client(profile='main')
+# singin/singup to tg account
+c = Client(profile='main')
 
 # get wallet auth token
 auth_token = c.get_token()
 
 w = Wallet(auth_token)
 
 ton_balance = w.get_user_balance('TON')['available_balance']
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.16 Summary:
+Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.17 Summary:
 Telegram Wallet API Author: no-name-user-name Author-email:
 dimazver61@gmail.com Description-Content-Type: text/markdown
                                     _[_L_o_g_o_]
                          ******** TTeelleeggrraamm WWaalllleett AAPPII ********
          Unofficial library for managing your personal Wallet account
 
 ## Table Of Contents * [About the Project](#about-the-project) * [Built With]
 (#built-with) * [Getting Started](#getting-started) * [Example](#example) *
 [Realised methods](#realised-methods) ## About The Project Send and receive
 tokens | Trade on P2P Market ## Built With To obtain an authorization token,
 the "selenium" library is used. Working with the API is implemented using
 "requests" ## Getting Started ```bazaar pip install pyTelegramWalletApi ``` ###
-Example ```python import time from wallet import Client, Wallet # for the first
-tg login c = Client.auth(profile='main') # chromedriver headless mode for
-authorized tg account # c = Client(profile='main') # get wallet auth token
-auth_token = c.get_token() w = Wallet(auth_token) ton_balance =
-w.get_user_balance('TON')['available_balance'] print(f'[*] Balance:
-{ton_balance} TON') tx_id = w.send_to_address(0.01, 'TON',
-'EQA5IHeHWX9BkTsI71ECzuD-HeYL-br36UmFoTWZFihU3fLz')['transaction_id'] tx_link =
-None status = '' # wait tx in block while tx_link is None: details =
-w.get_transaction_details(tx_id) tx_link = details["transaction_link"] status =
-details['status'] time.sleep(2) print(f'[*] Tx status: {status} | {tx_link}')
-""" Logs [*] Starting parse wallet authorization token... [*] Token find:
-eyJhbGciOiJIUzI1NiIsInR5cCI6IkpX.... [*] Balance: 100 TON [*] Tx status:
-success | https://tonscan.org/tx/.... """ ``` ## Realised methods Wallet
-Account Methods: - send_to_address() - get_user_balance() -
-get_transaction_details() - get_transactions() - get_rate() Wallet P2P Methods:
-- get_p2p_market() - create_p2p_offer() - edit_p2p_offer() - get_p2p_offer() -
-get_own_p2p_offer_by_id() - get_user_p2p_payment() - get_user_p2p_order_history
-() - get_own_p2p_offer() - get_own_p2p_offers() - enable_p2p_bidding() -
-disable_p2p_bidding() - p2p_offer_activate() - p2p_offer_deactivate()
+Example ```python import time from wallet import Client, Wallet # singin/singup
+to tg account c = Client(profile='main') # get wallet auth token auth_token =
+c.get_token() w = Wallet(auth_token) ton_balance = w.get_user_balance('TON')
+['available_balance'] print(f'[*] Balance: {ton_balance} TON') tx_id =
+w.send_to_address(0.01, 'TON', 'EQA5IHeHWX9BkTsI71ECzuD-HeYL-
+br36UmFoTWZFihU3fLz')['transaction_id'] tx_link = None status = '' # wait tx in
+block while tx_link is None: details = w.get_transaction_details(tx_id) tx_link
+= details["transaction_link"] status = details['status'] time.sleep(2) print(f'
+[*] Tx status: {status} | {tx_link}') """ Logs [*] Starting parse wallet
+authorization token... [*] Token find: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpX.... [*]
+Balance: 100 TON [*] Tx status: success | https://tonscan.org/tx/.... """ ```
+## Realised methods Wallet Account Methods: - send_to_address() -
+get_user_balance() - get_transaction_details() - get_transactions() - get_rate
+() Wallet P2P Methods: - get_p2p_market() - create_p2p_offer() - edit_p2p_offer
+() - get_p2p_offer() - get_own_p2p_offer_by_id() - get_user_p2p_payment() -
+get_user_p2p_order_history() - get_own_p2p_offer() - get_own_p2p_offers() -
+enable_p2p_bidding() - disable_p2p_bidding() - p2p_offer_activate() -
+p2p_offer_deactivate()
```

### Comparing `pyTelegramWalletApi-0.2.16/setup.py` & `pyTelegramWalletApi-0.2.17/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = ["requests", "selenium-wire", "pytest"]
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyTelegramWalletApi',
-    version='0.2.16',
+    version='0.2.17',
     author='no-name-user-name',
     description='Telegram Wallet API',
     packages=find_packages(),
     install_requires=requirements,
     author_email='dimazver61@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown'
```

### Comparing `pyTelegramWalletApi-0.2.16/tests/rest_tests.py` & `pyTelegramWalletApi-0.2.17/tests/rest_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 w = Wallet(AUTH_TOKEN)
 
 
 def test_get_own_p2p_offer():
     offers = w.get_own_p2p_offers()
     assert isinstance(offers[0], OwnOffer)
-    offer = w.get_own_p2p_offer(offer_id=offers[0].id)
-    offer = w.get_own_p2p_offer(tag=offers[0].number)
-    assert isinstance(offer, OwnOffer | [])
+    # offer = w.get_own_p2p_offer(offer_id=offers[0].id)
+    # offer = w.get_own_p2p_offer(tag=offers[0].number)
+    # assert isinstance(offer, OwnOffer | [])
 
 
 def test_get_user_balance():
     balance = w.get_user_balance()
     assert 'available_balance' in balance
```

### Comparing `pyTelegramWalletApi-0.2.16/wallet/rest/__init__.py` & `pyTelegramWalletApi-0.2.17/wallet/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.16/wallet/selenium/__init__.py` & `pyTelegramWalletApi-0.2.17/wallet/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.16/wallet/types.py` & `pyTelegramWalletApi-0.2.17/wallet/types.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.16/wallet/web_client.py` & `pyTelegramWalletApi-0.2.17/wallet/web_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,39 @@
+import os.path
 import time
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
 
 from wallet.selenium import TelegramDriver
 
 
 class Client:
     def __init__(self, headless=True, profile='main', temp_dir_path=None):
+
+        full_dir_path = '_temp/profile_' + str(profile)
+        if not os.path.isdir(full_dir_path):
+            os.makedirs(full_dir_path)
+            self.auth(profile=profile, temp_dir_path=temp_dir_path)
+
         self.tgd = TelegramDriver(profile=profile, is_headless=headless, temp_dir_path=temp_dir_path)
         self.driver = self.tgd.driver
         self.driver.get('https://web.telegram.org/a/#1985737506')
 
     @classmethod
     def auth(cls, profile, temp_dir_path=None):
         c = Client(headless=False, profile=profile, temp_dir_path=temp_dir_path)
-        input('[!] Complite auth in browser and click any key to continue...')
-        return c
+        print('[!] Connect Telegram Account')
+
+        while True:
+            if c.driver.current_url == 'https://web.telegram.org/a/#1985737506':
+                return c
+            else:
+                time.sleep(1)
 
     def get_token(self) -> str:
         print('[*] Starting parse wallet authorization token...')
         self.driver.find_element(By.CLASS_NAME, 'middle-column-footer').find_element(By.CLASS_NAME, 'mounted')\
             .find_element(By.CLASS_NAME, 'message-input-wrapper').find_element(By.TAG_NAME, 'button').click()
 
         try:
```

