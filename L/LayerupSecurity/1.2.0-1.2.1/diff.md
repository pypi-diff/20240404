# Comparing `tmp/LayerupSecurity-1.2.0.tar.gz` & `tmp/LayerupSecurity-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LayerupSecurity-1.2.0.tar", last modified: Sat Mar 30 04:40:05 2024, max compression
+gzip compressed data, was "LayerupSecurity-1.2.1.tar", last modified: Thu Apr  4 02:37:24 2024, max compression
```

## Comparing `LayerupSecurity-1.2.0.tar` & `LayerupSecurity-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jamsheed   (501) staff       (20)        0 2024-03-30 04:40:05.123797 LayerupSecurity-1.2.0/
--rw-r--r--   0 jamsheed   (501) staff       (20)     1055 2024-03-16 00:07:33.000000 LayerupSecurity-1.2.0/LICENSE
-drwxr-xr-x   0 jamsheed   (501) staff       (20)        0 2024-03-30 04:40:05.123208 LayerupSecurity-1.2.0/LayerupSecurity.egg-info/
--rw-r--r--   0 jamsheed   (501) staff       (20)     3708 2024-03-30 04:40:05.000000 LayerupSecurity-1.2.0/LayerupSecurity.egg-info/PKG-INFO
--rw-r--r--   0 jamsheed   (501) staff       (20)      339 2024-03-30 04:40:05.000000 LayerupSecurity-1.2.0/LayerupSecurity.egg-info/SOURCES.txt
--rw-r--r--   0 jamsheed   (501) staff       (20)        1 2024-03-30 04:40:05.000000 LayerupSecurity-1.2.0/LayerupSecurity.egg-info/dependency_links.txt
--rw-r--r--   0 jamsheed   (501) staff       (20)       17 2024-03-30 04:40:05.000000 LayerupSecurity-1.2.0/LayerupSecurity.egg-info/requires.txt
--rw-r--r--   0 jamsheed   (501) staff       (20)       17 2024-03-30 04:40:05.000000 LayerupSecurity-1.2.0/LayerupSecurity.egg-info/top_level.txt
--rw-r--r--   0 jamsheed   (501) staff       (20)     3708 2024-03-30 04:40:05.123527 LayerupSecurity-1.2.0/PKG-INFO
--rw-r--r--   0 jamsheed   (501) staff       (20)     2896 2024-03-28 21:02:05.000000 LayerupSecurity-1.2.0/README.md
-drwxr-xr-x   0 jamsheed   (501) staff       (20)        0 2024-03-30 04:40:05.123009 LayerupSecurity-1.2.0/layerup_security/
--rw-r--r--   0 jamsheed   (501) staff       (20)       46 2024-03-16 00:00:34.000000 LayerupSecurity-1.2.0/layerup_security/__init__.py
--rw-r--r--   0 jamsheed   (501) staff       (20)      616 2024-03-16 02:26:17.000000 LayerupSecurity-1.2.0/layerup_security/config.py
--rw-r--r--   0 jamsheed   (501) staff       (20)     4572 2024-03-28 20:57:59.000000 LayerupSecurity-1.2.0/layerup_security/layerup_security.py
--rw-r--r--   0 jamsheed   (501) staff       (20)     1397 2024-03-30 04:39:03.000000 LayerupSecurity-1.2.0/layerup_security/utils.py
--rw-r--r--   0 jamsheed   (501) staff       (20)       38 2024-03-30 04:40:05.123854 LayerupSecurity-1.2.0/setup.cfg
--rw-r--r--   0 jamsheed   (501) staff       (20)      991 2024-03-30 04:33:21.000000 LayerupSecurity-1.2.0/setup.py
+drwxr-xr-x   0 jamsheed   (501) staff       (20)        0 2024-04-04 02:37:24.472158 LayerupSecurity-1.2.1/
+-rw-r--r--   0 jamsheed   (501) staff       (20)     1055 2024-03-16 00:07:33.000000 LayerupSecurity-1.2.1/LICENSE
+drwxr-xr-x   0 jamsheed   (501) staff       (20)        0 2024-04-04 02:37:24.471649 LayerupSecurity-1.2.1/LayerupSecurity.egg-info/
+-rw-r--r--   0 jamsheed   (501) staff       (20)     3708 2024-04-04 02:37:24.000000 LayerupSecurity-1.2.1/LayerupSecurity.egg-info/PKG-INFO
+-rw-r--r--   0 jamsheed   (501) staff       (20)      339 2024-04-04 02:37:24.000000 LayerupSecurity-1.2.1/LayerupSecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 jamsheed   (501) staff       (20)        1 2024-04-04 02:37:24.000000 LayerupSecurity-1.2.1/LayerupSecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 jamsheed   (501) staff       (20)       17 2024-04-04 02:37:24.000000 LayerupSecurity-1.2.1/LayerupSecurity.egg-info/requires.txt
+-rw-r--r--   0 jamsheed   (501) staff       (20)       17 2024-04-04 02:37:24.000000 LayerupSecurity-1.2.1/LayerupSecurity.egg-info/top_level.txt
+-rw-r--r--   0 jamsheed   (501) staff       (20)     3708 2024-04-04 02:37:24.471911 LayerupSecurity-1.2.1/PKG-INFO
+-rw-r--r--   0 jamsheed   (501) staff       (20)     2896 2024-03-28 21:02:05.000000 LayerupSecurity-1.2.1/README.md
+drwxr-xr-x   0 jamsheed   (501) staff       (20)        0 2024-04-04 02:37:24.471323 LayerupSecurity-1.2.1/layerup_security/
+-rw-r--r--   0 jamsheed   (501) staff       (20)       46 2024-03-16 00:00:34.000000 LayerupSecurity-1.2.1/layerup_security/__init__.py
+-rw-r--r--   0 jamsheed   (501) staff       (20)      616 2024-03-16 02:26:17.000000 LayerupSecurity-1.2.1/layerup_security/config.py
+-rw-r--r--   0 jamsheed   (501) staff       (20)     4630 2024-04-04 02:33:45.000000 LayerupSecurity-1.2.1/layerup_security/layerup_security.py
+-rw-r--r--   0 jamsheed   (501) staff       (20)     1397 2024-03-30 04:39:03.000000 LayerupSecurity-1.2.1/layerup_security/utils.py
+-rw-r--r--   0 jamsheed   (501) staff       (20)       38 2024-04-04 02:37:24.472202 LayerupSecurity-1.2.1/setup.cfg
+-rw-r--r--   0 jamsheed   (501) staff       (20)      991 2024-04-04 02:36:51.000000 LayerupSecurity-1.2.1/setup.py
```

### Comparing `LayerupSecurity-1.2.0/LICENSE` & `LayerupSecurity-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LayerupSecurity-1.2.0/LayerupSecurity.egg-info/PKG-INFO` & `LayerupSecurity-1.2.1/LayerupSecurity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LayerupSecurity
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python wrapper for the Layerup Security API.
 Home-page: https://github.com/layerupai/layerup-security-sdk-python
 Author: Layerup
 Author-email: pypi@uselayerup.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LayerupSecurity-1.2.0/PKG-INFO` & `LayerupSecurity-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LayerupSecurity
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python wrapper for the Layerup Security API.
 Home-page: https://github.com/layerupai/layerup-security-sdk-python
 Author: Layerup
 Author-email: pypi@uselayerup.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LayerupSecurity-1.2.0/README.md` & `LayerupSecurity-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `LayerupSecurity-1.2.0/layerup_security/config.py` & `LayerupSecurity-1.2.1/layerup_security/config.py`

 * *Files identical despite different names*

### Comparing `LayerupSecurity-1.2.0/layerup_security/layerup_security.py` & `LayerupSecurity-1.2.1/layerup_security/layerup_security.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,21 +76,21 @@
         """
         url = f"{self.config.base_url}/log/error"
         headers = {"Layerup-API-Key": self.config.api_key, "Content-Type": "application/json"}
         data = {"error": error, "messages": messages, "metadata": metadata}
 
         return make_api_call(url, method='POST', headers=headers, data=data)
 
-    def execute_guardrails(self, guardrails, messages, metadata={}):
+    def execute_guardrails(self, guardrails, messages, untrusted_input=None, metadata={}):
         """
         Execute pre-defined guardrails that allow you to send canned responses when a user prompts in a certain way, adding a layer of protection to your LLM calls.
 
         :param guardrails: List of guardrail names to execute.
         :param messages: List of messages in the LLM conversation.
         :param metadata: Optional metadata object for the request.
         :return: The JSON response from the API call.
         """
         url = f"{self.config.base_url}/guardrails/execute"
         headers = {"Layerup-API-Key": self.config.api_key, "Content-Type": "application/json"}
-        data = {"guardrails": guardrails, "messages": messages, "metadata": metadata}
+        data = {"guardrails": guardrails, "messages": messages, "untrusted_input": untrusted_input, "metadata": metadata}
 
         return make_api_call(url, method='POST', headers=headers, data=data)
```

### Comparing `LayerupSecurity-1.2.0/layerup_security/utils.py` & `LayerupSecurity-1.2.1/layerup_security/utils.py`

 * *Files identical despite different names*

### Comparing `LayerupSecurity-1.2.0/setup.py` & `LayerupSecurity-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='LayerupSecurity',
-    version='1.2.0',
+    version='1.2.1',
     author='Layerup',
     author_email='pypi@uselayerup.com',
     description='A Python wrapper for the Layerup Security API.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/layerupai/layerup-security-sdk-python',
     packages=find_packages(),
```

