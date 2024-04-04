# Comparing `tmp/easy_utils_dev-2.8.1.tar.gz` & `tmp/easy_utils_dev-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.8.1.tar", last modified: Thu Apr  4 14:47:24 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.8.2.tar", last modified: Thu Apr  4 15:16:59 2024, max compression
```

## Comparing `easy_utils_dev-2.8.1.tar` & `easy_utils_dev-2.8.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:47:24.432451 easy_utils_dev-2.8.1/
--rw-rw-rw-   0        0        0      174 2024-04-04 14:47:24.426597 easy_utils_dev-2.8.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 14:47:24.378123 easy_utils_dev-2.8.1/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.1/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.1/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      339 2024-04-04 13:44:23.000000 easy_utils_dev-2.8.1/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.1/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.1/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.1/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7599 2024-04-04 14:47:15.000000 easy_utils_dev-2.8.1/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.1/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.1/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.1/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.1/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.1/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.1/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 11:55:23.000000 easy_utils_dev-2.8.1/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:47:24.420732 easy_utils_dev-2.8.1/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-04 14:47:24.000000 easy_utils_dev-2.8.1/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2024-04-04 14:47:24.000000 easy_utils_dev-2.8.1/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 14:47:24.000000 easy_utils_dev-2.8.1/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 14:47:24.000000 easy_utils_dev-2.8.1/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-04 14:47:24.000000 easy_utils_dev-2.8.1/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 14:47:24.432451 easy_utils_dev-2.8.1/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-04 14:47:19.000000 easy_utils_dev-2.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:16:59.424538 easy_utils_dev-2.8.2/
+-rw-rw-rw-   0        0        0      174 2024-04-04 15:16:59.419656 easy_utils_dev-2.8.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 15:16:59.361180 easy_utils_dev-2.8.2/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.2/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.2/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      339 2024-04-04 13:44:23.000000 easy_utils_dev-2.8.2/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.2/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.2/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.2/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7708 2024-04-04 15:16:47.000000 easy_utils_dev-2.8.2/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.2/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.2/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.2/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.2/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.2/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.2/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 11:55:23.000000 easy_utils_dev-2.8.2/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:16:59.414785 easy_utils_dev-2.8.2/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-04 15:16:59.000000 easy_utils_dev-2.8.2/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2024-04-04 15:16:59.000000 easy_utils_dev-2.8.2/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:16:59.000000 easy_utils_dev-2.8.2/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 15:16:59.000000 easy_utils_dev-2.8.2/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-04 15:16:59.000000 easy_utils_dev-2.8.2/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:16:59.425534 easy_utils_dev-2.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-04 15:16:53.000000 easy_utils_dev-2.8.2/setup.py
```

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.8.2/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/Events.py` & `easy_utils_dev-2.8.2/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.8.2/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/debugger.py` & `easy_utils_dev-2.8.2/easy_utils_dev/debugger.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.8.2/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/lralib.py` & `easy_utils_dev-2.8.2/easy_utils_dev/lralib.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,33 +43,34 @@
     
     def enableOnScreenDebugPrint( self ) :
         self.logger.enable_print()
 
     def autoRefreshToken(self) :
         self.logger.info(f'Auto refresh token started. waiting for {self.autoRefreshTokenPeriod} refresh ...')
         time.sleep(self.autoRefreshTokenPeriod )
-        self.seLogout()
-        self.seAuthentication()
+        self.logout()
+        self.authentication()
         self.logger.info(f'Auto Token refresh completed.')
 
 
     def authentication(self,autoRefresh=True) :
         self.logger.info('Starting to authenticate with LRA platform ..')
         url = f'{self.baseUrl}/wavesuite/common/auth/realms/wavesuite/protocol/openid-connect/token'
         self.logger.info(f"Authentication Params: username={self.username} password=********")
+        self.logger.info(f"Authentication Params: username={self.username} password={self.password} url={url}")
         payload = {
             'grant_type': 'password',
             'username': self.username ,
             'password': self.password,
             'client_id': 'wp-lra-service',
             'client_secret': 'c74b4dfb-4293-46da-a38a-9fd46fce23b0'
         }
-        headers = {'Content-type': 'x-www-form-urlencoded' }
+        headers = {'Content-type': 'application/x-www-form-urlencoded' }
         self.logger.debug(f'Authentication Payload: {payload}')
-        response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
+        response = requests.post(url , data=payload , headers=headers , verify=False)
         self.logger.info(f'Authentication response code={response.status_code}')
         self.logger.debug(f'raw response in authentication {response.text}')
         if response.status_code != 200 :
             self.logger.error(f'Authentication failed. status_code={response.status_code} {response.text}')
             return
         response = response.json()
         self.accessToken = response['data']['accessToken']
```

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.8.2/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.8.2/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.8.2/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.8.2/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/utils.py` & `easy_utils_dev-2.8.2/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.8.2/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.8.2/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.1/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.8.2/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

