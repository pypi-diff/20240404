# Comparing `tmp/streamlit-ldap-authenticator-0.2.2.tar.gz` & `tmp/streamlit-ldap-authenticator-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-ldap-authenticator-0.2.2.tar", last modified: Wed Mar 27 14:21:31 2024, max compression
+gzip compressed data, was "streamlit-ldap-authenticator-0.2.3.tar", last modified: Thu Apr  4 00:21:21 2024, max compression
```

## Comparing `streamlit-ldap-authenticator-0.2.2.tar` & `streamlit-ldap-authenticator-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 14:21:31.198595 streamlit-ldap-authenticator-0.2.2/
--rw-rw-rw-   0        0        0     1089 2024-02-29 23:36:46.000000 streamlit-ldap-authenticator-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    14306 2024-03-27 14:21:31.196597 streamlit-ldap-authenticator-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    13289 2024-03-27 14:20:42.000000 streamlit-ldap-authenticator-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-27 14:21:31.199595 streamlit-ldap-authenticator-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1505 2024-03-27 14:07:07.000000 streamlit-ldap-authenticator-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 14:21:31.185178 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/
--rw-rw-rw-   0        0        0      308 2024-03-27 14:06:56.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/__init__.py
--rw-rw-rw-   0        0        0    18416 2024-03-27 14:06:56.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/authenticate.py
--rw-rw-rw-   0        0        0    10523 2024-03-27 14:06:56.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/configs.py
--rw-rw-rw-   0        0        0      971 2024-02-29 23:36:46.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/exceptions.py
--rw-rw-rw-   0        0        0     7394 2024-03-27 14:19:10.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/ldap_authenticate.py
-drwxrwxrwx   0        0        0        0 2024-03-27 14:21:31.194180 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator.egg-info/
--rw-rw-rw-   0        0        0    14306 2024-03-27 14:21:31.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-03-27 14:21:31.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 14:21:31.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      231 2024-03-27 14:21:31.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-03-27 14:21:31.000000 streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 00:21:21.680514 streamlit-ldap-authenticator-0.2.3/
+-rw-rw-rw-   0        0        0     1089 2024-02-22 23:54:56.000000 streamlit-ldap-authenticator-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    23576 2024-04-04 00:21:21.674682 streamlit-ldap-authenticator-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    22561 2024-04-04 00:18:12.000000 streamlit-ldap-authenticator-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 00:21:21.680844 streamlit-ldap-authenticator-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1505 2024-04-04 00:18:20.000000 streamlit-ldap-authenticator-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:21:21.639383 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/
+-rw-rw-rw-   0        0        0      308 2024-03-23 04:43:04.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/__init__.py
+-rw-rw-rw-   0        0        0    18464 2024-04-04 00:18:05.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/authenticate.py
+-rw-rw-rw-   0        0        0    10523 2024-03-23 04:42:56.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/configs.py
+-rw-rw-rw-   0        0        0      971 2024-02-22 10:48:27.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/exceptions.py
+-rw-rw-rw-   0        0        0     7428 2024-04-04 00:17:59.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/ldap_authenticate.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:21:21.666118 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/
+-rw-rw-rw-   0        0        0    23576 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      231 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-04 00:21:21.000000 streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator.egg-info/top_level.txt
```

### Comparing `streamlit-ldap-authenticator-0.2.2/LICENSE` & `streamlit-ldap-authenticator-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.2/setup.py` & `streamlit-ldap-authenticator-0.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Author   : Nathan Chen
-# Date     : 27-Mar-2024
+# Date     : 04-Apr-2024
 
 
 from pathlib import Path
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='UTF-8')
 
 setup(
     name='streamlit-ldap-authenticator',
-    version='0.2.2',
+    version='0.2.3',
     author='Nathan Chen',
     author_email='nathan.chen.198@gmail.com',
     description='Authenticate using ldap',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NathanChen198/streamlit-ldap-authenticator',
     packages=find_packages(),
```

### Comparing `streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/authenticate.py` & `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/authenticate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Author    : Nathan Chen
-# Date      : 25-Mar-2024
+# Date      : 04-Apr-2024
 
 
 import time
 import jwt
 import re
 import streamlit as st
 from streamlit_cookies_controller import CookieController
@@ -229,15 +229,15 @@
         default = {'remember': self.__getRememberMe()} if self.cookie_configs is not None else None
         (config, busy_message, error_icon) = self.__getLoginConfig(config)
 
         # Create form
         result = self.ui.signinForm(default, config)
         if result is None: return None
 
-        if self.encryptor is not None: result = self.encryptor.decrypt(result)
+        if self.encryptor is not None and type(result) is str: result = self.encryptor.decrypt(result)
         event = getEvent(result)
         if type(event) is not SigninEvent: return None
 
         self.__setRememberMe(event.remember)
 
         with st.spinner(busy_message):
             username = event.username
@@ -375,15 +375,15 @@
         """
         (config, busy_message, sleep_sec) = self.__getLogoutConfig(config)
 
         # Create form
         result = self.ui.signoutForm(configs=config)
         if result is None: return None
         
-        if self.encryptor is not None: result = self.encryptor.decrypt(result)
+        if self.encryptor is not None and type(result) is str: result = self.encryptor.decrypt(result)
         event = getEvent(result)
         if type(event) is not SignoutEvent: return None
 
         with st.spinner(busy_message):
             if callback is not None:
                 result = callback(event)
                 if result == 'cancel': return
```

### Comparing `streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/configs.py` & `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/configs.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/exceptions.py` & `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlit-ldap-authenticator-0.2.2/streamlit_ldap_authenticator/ldap_authenticate.py` & `streamlit-ldap-authenticator-0.2.3/streamlit_ldap_authenticator/ldap_authenticate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Author    : Nathan Chen
-# Date      : 27-Mar-2024
+# Date      : 04-Apr-2024
 
 
 
 
 
 from ldap3 import Server, Connection
 from ldap3.abstract.entry import Entry
@@ -56,14 +56,15 @@
             otherwise, authentication fail message
         """
 
         server = Server(self.config.server_path, use_ssl=self.config.use_ssl, get_info='ALL')
         conn = Connection(server, username, password, auto_bind=False, auto_referrals=False, raise_exceptions=False)
         try:
             conn.bind()
+            conn.password = None
             if conn.result['result'] != 0: return 'Wrong username or password'
             user = getInfo(conn)
             if user is None: return f"No information found in active directory for '{username}'"
             if additionalCheck is None: return user
 
             result = additionalCheck(conn, user)
             if result == True: return user
```

