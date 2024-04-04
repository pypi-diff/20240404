# Comparing `tmp/gologin-2024.4.3191731.tar.gz` & `tmp/gologin-2024.4.4122950.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gologin-2024.4.3191731.tar", last modified: Wed Apr  3 19:17:32 2024, max compression
+gzip compressed data, was "gologin-2024.4.4122950.tar", last modified: Thu Apr  4 12:29:51 2024, max compression
```

## Comparing `gologin-2024.4.3191731.tar` & `gologin-2024.4.4122950.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/gologin/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/gologin/extensionsManager/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/extensionsManager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/extensionsManager/extensionsManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-create-profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-local.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-pyppeteer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-selenium-multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-selenium.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-selenium_4.11.py
--rw-r--r--   0 runner    (1001) docker     (127)    29398 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/gologin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 19:17:31.000000 gologin-2024.4.3191731/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:51.159204 gologin-2024.4.4122950/gologin/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/gologin/extensionsManager/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/extensionsManager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/extensionsManager/extensionsManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-create-profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-pyppeteer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-selenium-multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-selenium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-selenium_4.11.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29704 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/gologin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-04 12:29:50.000000 gologin-2024.4.4122950/setup.py
```

### Comparing `gologin-2024.4.3191731/PKG-INFO` & `gologin-2024.4.4122950/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gologin
-Version: 2024.4.3191731
+Version: 2024.4.4122950
 Summary: Official GoLogin python package
 Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin
 Author-email: yuri@gologin.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gologin Version: 2024.4.3191731 Summary: Official
+Metadata-Version: 2.1 Name: gologin Version: 2024.4.4122950 Summary: Official
 GoLogin python package Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin Author-email: yuri@gologin.com Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: psutil # pygologin REST API provides programmatic
 access to GoLogin App. Create a new browser profile, get a list of all browser
 profiles, add a browser profile and running # class GoLogin - class for working
 with _g_o_l_o_g_i_n_._c_o_m API # Official Package ## Getting Started GoLogin supports
```

### Comparing `gologin-2024.4.3191731/README.md` & `gologin-2024.4.4122950/README.md`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3191731/gologin/extensionsManager/extensionsManager.py` & `gologin-2024.4.4122950/gologin/extensionsManager/extensionsManager.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3191731/gologin/gologin-create-profile.py` & `gologin-2024.4.4122950/gologin/gologin-create-profile.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3191731/gologin/gologin-local.py` & `gologin-2024.4.4122950/gologin/gologin-local.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3191731/gologin/gologin-pyppeteer.py` & `gologin-2024.4.4122950/gologin/gologin-pyppeteer.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3191731/gologin/gologin-selenium-multiprocess.py` & `gologin-2024.4.4122950/gologin/gologin-selenium-multiprocess.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3191731/gologin/gologin-selenium.py` & `gologin-2024.4.4122950/gologin/gologin-selenium.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3191731/gologin/gologin-selenium_4.11.py` & `gologin-2024.4.4122950/gologin/gologin-selenium_4.11.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3191731/gologin/gologin.py` & `gologin-2024.4.4122950/gologin/gologin.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 from .extensionsManager import ExtensionsManager
 
 API_URL = 'https://api.gologin.com'
 PROFILES_URL = 'https://gprofiles-new.gologin.com/'
 GET_TIMEZONE_URL = 'https://geo.myip.link'
 FILES_GATEWAY = ' https://files-gateway.gologin.com'
 
+class ProtocolException(Exception):
+    def __init__(self, data:dict):
+        self._json =data
+        super().__init__(data.__repr__())
+    @property
+    def json(self) -> dict:
+        return self._json
+
 class GoLogin(object):
     def __init__(self, options):
         self.access_token = options.get('token')
         self.profile_id = options.get('profile_id')
         self.tmpdir = options.get('tmpdir', tempfile.gettempdir())
         self.address = options.get('address', '127.0.0.1')
         self.extra_params = options.get('extra_params', [])
@@ -649,14 +657,16 @@
             profile['storage'] = options.get('storage')
 
         for k, v in options.items():
             profile[k] = v
 
         response = json.loads(requests.post(
             API_URL + '/browser', headers=self.headers(), json=profile).content.decode('utf-8'))
+        if not (response.get('statusCode') is None):
+            raise ProtocolException(response)
         return response.get('id')
 
     def delete(self, profile_id=None):
         profile = self.profile_id if profile_id == None else profile_id
         requests.delete(API_URL + '/browser/' +
                         profile, headers=self.headers())
```

### Comparing `gologin-2024.4.3191731/gologin.egg-info/PKG-INFO` & `gologin-2024.4.4122950/gologin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gologin
-Version: 2024.4.3191731
+Version: 2024.4.4122950
 Summary: Official GoLogin python package
 Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin
 Author-email: yuri@gologin.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gologin Version: 2024.4.3191731 Summary: Official
+Metadata-Version: 2.1 Name: gologin Version: 2024.4.4122950 Summary: Official
 GoLogin python package Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin Author-email: yuri@gologin.com Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: psutil # pygologin REST API provides programmatic
 access to GoLogin App. Create a new browser profile, get a list of all browser
 profiles, add a browser profile and running # class GoLogin - class for working
 with _g_o_l_o_g_i_n_._c_o_m API # Official Package ## Getting Started GoLogin supports
```

### Comparing `gologin-2024.4.3191731/setup.py` & `gologin-2024.4.4122950/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f.readlines()]
 
 setup(
     name='gologin',
-    version='2024.04.03191731',
+    version='2024.04.04122950',
     packages=find_packages(),
     install_requires=install_requires,
     author='GoLogin',
     author_email='yuri@gologin.com',
     description='Official GoLogin python package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

