# Comparing `tmp/chattool-3.1.3.tar.gz` & `tmp/chattool-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattool-3.1.3.tar", last modified: Sun Mar 24 09:04:19 2024, max compression
+gzip compressed data, was "chattool-3.1.4.tar", last modified: Thu Apr  4 13:18:50 2024, max compression
```

## Comparing `chattool-3.1.3.tar` & `chattool-3.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 09:04:19.929874 chattool-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-24 09:04:09.000000 chattool-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-03-24 09:04:19.929874 chattool-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-24 09:04:09.000000 chattool-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 09:04:19.929874 chattool-3.1.3/chattool/
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/asynctool.py
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/chattype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/functioncall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-24 09:04:09.000000 chattool-3.1.3/chattool/tokencalc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 09:04:19.929874 chattool-3.1.3/chattool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-03-24 09:04:19.000000 chattool-3.1.3/chattool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-24 09:04:19.000000 chattool-3.1.3/chattool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 09:04:19.000000 chattool-3.1.3/chattool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-24 09:04:19.000000 chattool-3.1.3/chattool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 09:04:19.000000 chattool-3.1.3/chattool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-24 09:04:19.000000 chattool-3.1.3/chattool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-24 09:04:19.000000 chattool-3.1.3/chattool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 09:04:19.929874 chattool-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-24 09:04:09.000000 chattool-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:18:50.091374 chattool-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 13:18:37.000000 chattool-3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-04 13:18:50.091374 chattool-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-04 13:18:37.000000 chattool-3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:18:50.091374 chattool-3.1.4/chattool/
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/asynctool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/chattype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/functioncall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-04 13:18:37.000000 chattool-3.1.4/chattool/tokencalc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:18:50.091374 chattool-3.1.4/chattool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-04 13:18:50.000000 chattool-3.1.4/chattool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 13:18:49.000000 chattool-3.1.4/chattool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:18:50.091374 chattool-3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 13:18:37.000000 chattool-3.1.4/setup.py
```

### Comparing `chattool-3.1.3/LICENSE` & `chattool-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/PKG-INFO` & `chattool-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattool
-Version: 3.1.3
+Version: 3.1.4
 Summary: Toolkit for Chat API
 Home-page: https://github.com/cubenlp/chattool
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: <div align="center">
             <a href="https://pypi.python.org/pypi/chattool">
```

### Comparing `chattool-3.1.3/README.md` & `chattool-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/chattool/__init__.py` & `chattool-3.1.4/chattool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Chattool."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '3.1.3'
+__version__ = '3.1.4'
 
 import os, sys, requests
 from .chattype import Chat, Resp
 from .checkpoint import load_chats, process_chats
 from .proxy import proxy_on, proxy_off, proxy_status
 from . import request
 from .tokencalc import model_cost_perktoken, findcost
```

### Comparing `chattool-3.1.3/chattool/asynctool.py` & `chattool-3.1.4/chattool/asynctool.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
                             , chkpoint:str
                             , api_key:str
                             , chat_url:str
                             , max_tries:int=1
                             , nproc:int=1
                             , timeout:int=0
                             , timeinterval:int=0
+                            , showcost:bool=False
                             , **options
                             )->List[bool]:
     """Process messages asynchronously
 
     Args:
         chatlogs (List[List[Dict]]): list of chat logs
         chkpoint (str): checkpoint file
@@ -96,15 +97,15 @@
                                , timeout=timeout)
         ## saving files
         if resp is None: return 0, 0
         chat_log.append(resp.message)
         chat = Chat(chat_log)
         async with locker: # locker | not necessary for normal IO
             chat.save(chkpoint, index=ind)
-        return ind, resp.cost()
+        return ind, resp.cost() if showcost else 0
 
     async with sem, aiohttp.ClientSession() as session:
         tasks = []
         for ind, chat_log in enumerate(chatlogs):
             if chats[ind] is not None: # skip completed chats
                 continue
             tasks.append(
@@ -120,59 +121,60 @@
             responses = await tqdm.asyncio.tqdm.gather(*tasks)
         for ind, cost in responses:
             costs[ind] = cost
         return costs
 
 def async_chat_completion( msgs:Union[List[List[Dict]], str]
                          , chkpoint:str
-                         , model:str='gpt-3.5-turbo'
                          , api_key:Union[str, None]=None
                          , chat_url:Union[str, None]=None
                          , max_tries:int=1
                          , nproc:int=1
                          , timeout:int=0
                          , timeinterval:int=0
                          , clearfile:bool=False
-                         , notrun:bool=False
-                         , msg2log:Union[Callable, None]=None
+                         , wait:bool=False
+                         , showcost:bool=False
                          , data2chat:Union[Callable, None]=None
+                         , msg2log:Union[Callable, None]=None
                          , max_requests:int=-1
                          , ncoroutines:int=1
+                         , notrun:bool=False
                          , **options
                          ):
     """Asynchronous chat completion
 
     Args:
         msgs (Union[List[List[Dict]], str]): list of chat logs or chat message
         chkpoint (str): checkpoint file
         model (str, optional): model to use. Defaults to 'gpt-3.5-turbo'.
         api_key (Union[str, None], optional): API key. Defaults to None.
         max_tries (int, optional): maximum number of requests to make. Defaults to 1.
         nproc (int, optional): number of coroutines. Defaults to 1.
         timeout (int, optional): timeout for the API call. Defaults to 0(no timeout).
         timeinterval (int, optional): time interval between two API calls. Defaults to 0.
         clearfile (bool, optional): whether to clear the checkpoint file. Defaults to False.
-        notrun (bool, optional): whether to run the async process. It should be True
-          when use in Jupyter Notebook. Defaults to False.
+        wait (bool, optional): wait for the `await` command. Defaults to False.
         msg2log (Union[Callable, None], optional): function to convert message to chat log.
             Defaults to None.
         data2chat (Union[Callable, None], optional): function to convert data to Chat object.
             Defaults to None.
+        notrun (bool, optional): (Deprecated) wait for the `await` command. Defaults to False.
         max_requests (int, optional): (Deprecated)maximum number of requests to make. Defaults to -1.
         ncoroutines (int, optional): (Deprecated)number of coroutines. Defaults to 1.
 
     Returns:
         List[Dict]: list of responses
     """
-    # convert chatlogs
+    # convert msg to chatlogs
     if data2chat is not None:
         msg2log = lambda data: data2chat(data).chat_log
     elif msg2log is None: # By default, use method from the Chat object
         msg2log = lambda data: Chat(data).chat_log
-    # use nproc instead of ncoroutines
+    # number of coroutines
     nproc = max(nproc, ncoroutines)
     chatlogs = [msg2log(log) for log in msgs]
     if clearfile and os.path.exists(chkpoint):
         os.remove(chkpoint)
     if api_key is None:
         api_key = chattool.api_key
     assert api_key is not None, "API key is not provided!"
@@ -180,26 +182,28 @@
         if chattool.api_base:
             chat_url = os.path.join(chattool.api_base, "chat/completions")
         elif chattool.base_url:
             chat_url = os.path.join(chattool.base_url, "v1/chat/completions")
         else:
             raise Exception("chat_url is not provided!")
     chat_url = chattool.request.normalize_url(chat_url)
+    if 'model' not in options:
+        options['model'] = chattool.model if chattool.model else "gpt-3.5-turbo"
     # run async process
     assert nproc > 0, "nproc must be greater than 0!"
     max_tries = max(max_tries, max_requests)
     args = {
         "chatlogs": chatlogs,
         "chkpoint": chkpoint,
         "api_key": api_key,
         "chat_url": chat_url,
         "max_tries": max_tries,
+        "showcost": showcost,
         "nproc": nproc,
         "timeout": timeout,
         "timeinterval": timeinterval,
-        "model": model,
         **options
     }
-    if notrun: # when use in Jupyter Notebook
+    if notrun or wait: # when use in Jupyter Notebook
         return async_process_msgs(**args) # return the async object
     else:
         return asyncio.run(async_process_msgs(**args))
```

### Comparing `chattool-3.1.3/chattool/chattype.py` & `chattool-3.1.4/chattool/chattype.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/chattool/checkpoint.py` & `chattool-3.1.4/chattool/checkpoint.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/chattool/finetune.py` & `chattool-3.1.4/chattool/finetune.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/chattool/functioncall.py` & `chattool-3.1.4/chattool/functioncall.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/chattool/proxy.py` & `chattool-3.1.4/chattool/proxy.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/chattool/request.py` & `chattool-3.1.4/chattool/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
         gpt_only (bool, optional): whether to return only GPT models. Defaults to True.
 
     Returns:
         List[str]: list of valid models
     """
     headers = {
         "Authorization": "Bearer " + api_key,
-        "Content-Type": "application/json"
     }
     model_response = requests.get(normalize_url(model_url), headers=headers)
     if model_response.status_code == 200:
         data = model_response.json()
         model_list = [model.get("id") for model in data.get("data")]
         return [model for model in model_list if "gpt" in model] if gpt_only else model_list
     else:
@@ -128,15 +127,14 @@
     else:
         raise Exception(resp.text)
 
 def filecontent(api_key:str, base_url:str, fileid:str):
     """Returns the contents of the specified file"""
     headers = {
         "Authorization": "Bearer " + api_key,
-        "Content-Type": "application/json"
     }
     fileurl = normalize_url(os.path.join(base_url, "v1/files", fileid, "content"))
     resp = requests.get(fileurl, headers=headers)
     if resp.status_code == 200:
         return [json.loads(msg) for msg in resp.content.decode().split('\n') if msg]
     else:
         raise Exception(resp.text)
```

### Comparing `chattool-3.1.3/chattool/response.py` & `chattool-3.1.4/chattool/response.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/chattool/tokencalc.py` & `chattool-3.1.4/chattool/tokencalc.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.3/chattool.egg-info/PKG-INFO` & `chattool-3.1.4/chattool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattool
-Version: 3.1.3
+Version: 3.1.4
 Summary: Toolkit for Chat API
 Home-page: https://github.com/cubenlp/chattool
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: <div align="center">
             <a href="https://pypi.python.org/pypi/chattool">
```

### Comparing `chattool-3.1.3/setup.py` & `chattool-3.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '3.1.3'
+VERSION = '3.1.4'
 
 requirements = [
     'Click>=7.0', 'requests>=2.20', "responses>=0.23", 'aiohttp>=3.8',
     'tqdm>=4.60', 'docstring_parser>=0.10', "python-dotenv>=0.17.0"]
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
```

