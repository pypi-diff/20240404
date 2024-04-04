# Comparing `tmp/unofficial-claude-api-0.3.1.tar.gz` & `tmp/unofficial-claude-api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unofficial-claude-api-0.3.1.tar", last modified: Wed Mar 27 15:05:59 2024, max compression
+gzip compressed data, was "unofficial-claude-api-0.3.2.tar", last modified: Thu Apr  4 21:45:53 2024, max compression
```

## Comparing `unofficial-claude-api-0.3.1.tar` & `unofficial-claude-api-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:05:59.465002 unofficial-claude-api-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-27 15:05:54.000000 unofficial-claude-api-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-03-27 15:05:59.461002 unofficial-claude-api-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-03-27 15:05:54.000000 unofficial-claude-api-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:05:59.461002 unofficial-claude-api-0.3.1/claude2_api/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-27 15:05:54.000000 unofficial-claude-api-0.3.1/claude2_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:05:59.461002 unofficial-claude-api-0.3.1/claude_api/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-27 15:05:54.000000 unofficial-claude-api-0.3.1/claude_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-03-27 15:05:54.000000 unofficial-claude-api-0.3.1/claude_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-27 15:05:54.000000 unofficial-claude-api-0.3.1/claude_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-27 15:05:54.000000 unofficial-claude-api-0.3.1/claude_api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:05:59.465002 unofficial-claude-api-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-27 15:05:54.000000 unofficial-claude-api-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:05:59.461002 unofficial-claude-api-0.3.1/unofficial_claude_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-03-27 15:05:59.000000 unofficial-claude-api-0.3.1/unofficial_claude_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-27 15:05:59.000000 unofficial-claude-api-0.3.1/unofficial_claude_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:05:59.000000 unofficial-claude-api-0.3.1/unofficial_claude_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-27 15:05:59.000000 unofficial-claude-api-0.3.1/unofficial_claude_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 15:05:59.000000 unofficial-claude-api-0.3.1/unofficial_claude_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:45:53.867577 unofficial-claude-api-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 21:45:47.000000 unofficial-claude-api-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-04-04 21:45:53.867577 unofficial-claude-api-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-04 21:45:47.000000 unofficial-claude-api-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:45:53.867577 unofficial-claude-api-0.3.2/claude2_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-04 21:45:47.000000 unofficial-claude-api-0.3.2/claude2_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:45:53.867577 unofficial-claude-api-0.3.2/claude_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-04 21:45:47.000000 unofficial-claude-api-0.3.2/claude_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20500 2024-04-04 21:45:47.000000 unofficial-claude-api-0.3.2/claude_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-04 21:45:47.000000 unofficial-claude-api-0.3.2/claude_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-04 21:45:47.000000 unofficial-claude-api-0.3.2/claude_api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:45:53.867577 unofficial-claude-api-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-04 21:45:47.000000 unofficial-claude-api-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:45:53.867577 unofficial-claude-api-0.3.2/unofficial_claude_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-04-04 21:45:53.000000 unofficial-claude-api-0.3.2/unofficial_claude_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 21:45:53.000000 unofficial-claude-api-0.3.2/unofficial_claude_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:45:53.000000 unofficial-claude-api-0.3.2/unofficial_claude_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 21:45:53.000000 unofficial-claude-api-0.3.2/unofficial_claude_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 21:45:53.000000 unofficial-claude-api-0.3.2/unofficial_claude_api.egg-info/top_level.txt
```

### Comparing `unofficial-claude-api-0.3.1/LICENSE` & `unofficial-claude-api-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unofficial-claude-api-0.3.1/PKG-INFO` & `unofficial-claude-api-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unofficial-claude-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: This unofficial Python API provides access to the conversational capabilities of Anthropic's Claude AI through a simple chat messaging interface.
 Home-page: https://github.com/st1vms/unofficial-claude-api
 Author: st1vms
 Author-email: stefano.maria.salvatore@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,28 +24,28 @@
 - [Installation](#how-to-install)
 - [Requirements](#requirements)
 - [Example Usage](#example-usage)
 - [Tips](#tips)
   - [Retrieving Chat History](#retrieving-chat-history)
   - [Faster Loading](#faster-loading-avoiding-selenium)
   - [Proxies](#proxies)
-  - [Switching model version](#changing-claude-model)
+  - [Changing model version](#changing-claude-model)
 - [Troubleshooting](#troubleshooting)
 - [Donating](#donating)
 
 ## What is this?
 
 This unofficial Python API provides access to the conversational capabilities of Anthropic's Claude AI through a simple chat messaging interface.
 
 While not officially supported by Anthropic, this library can enable interesting conversational applications.
 
 It allows for:
 
 - Creating chat sessions with Claude and getting chat IDs.
-- Sending messages to Claude containing up to 5 attachment files (txt, pdf, csv, etc...) 10 MB each.
+- Sending messages to Claude containing up to 5 attachment files (txt, pdf, csv, png, jpeg, etc...) 10 MB each, images are also supported!
 - Retrieving chat message history, accessing specific chat conversations.
 - Deleting old chats when they are no longer needed.
 - Sending requests through proxies.
 
 ### Some of the key things you can do with Claude through this API
 
 - Ask questions about a wide variety of topics. Claude can chat about current events, pop culture, sports,
@@ -53,14 +53,16 @@
 
 - Get helpful explanations on complex topics. Ask Claude to explain concepts and ideas in simple terms.
 
 - Generate summaries from long text or documents. Just give the filepath as an attachment to Claude and get back a concise summary.
 
 - Receive thoughtful responses to open-ended prompts and ideas. Claude can brainstorm ideas, expand on concepts, and have philosophical discussions.
 
+- Send images and let Claude analyze them for you.
+
 ## How to install
 
 ```shell
 pip install unofficial-claude-api
 ```
 
 ## Uninstallation
@@ -270,27 +272,28 @@
 client = ClaudeAPIClient(session, proxy=socks_proxy)
 ```
 
 __________
 
 ### Changing Claude model
 
-In case you have accounts that are unable to migrate to latest model, you can override the `model_name` string parameter of `ClaudeAPIClient` constructor.
+In case you'd like to change the model used, or you do have accounts that are unable to migrate to latest model, you can override the `model_name` string parameter of `ClaudeAPIClient` constructor like so:
 
 ```py
 from claude_api.client import ClaudeAPIClient
 from claude_api.session import SessionData
 
 session = SessionData(...)
 
 # Defaults to None (latest Claude model)
-# Can be either claude-2.0 or claude-2.1
 client = ClaudeAPIClient(session, model_name="claude-2.0")
 ```
 
+You can retrieve the `model_name` strings from the [official API docs](https://docs.anthropic.com/claude/docs/models-overview#model-comparison)
+
 ## TROUBLESHOOTING
 
 Some common errors that may arise during the usage of this API:
 
 - *Error [400]* (Unable to prepare file attachment):
 
     To fix this error, change the extension of the attachment file to something like .txt, since by default this api will fallback to octet-stream for unknown file extensions, Claude may reject the file data.
```

### Comparing `unofficial-claude-api-0.3.1/README.md` & `unofficial-claude-api-0.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 - [Installation](#how-to-install)
 - [Requirements](#requirements)
 - [Example Usage](#example-usage)
 - [Tips](#tips)
   - [Retrieving Chat History](#retrieving-chat-history)
   - [Faster Loading](#faster-loading-avoiding-selenium)
   - [Proxies](#proxies)
-  - [Switching model version](#changing-claude-model)
+  - [Changing model version](#changing-claude-model)
 - [Troubleshooting](#troubleshooting)
 - [Donating](#donating)
 
 ## What is this?
 
 This unofficial Python API provides access to the conversational capabilities of Anthropic's Claude AI through a simple chat messaging interface.
 
 While not officially supported by Anthropic, this library can enable interesting conversational applications.
 
 It allows for:
 
 - Creating chat sessions with Claude and getting chat IDs.
-- Sending messages to Claude containing up to 5 attachment files (txt, pdf, csv, etc...) 10 MB each.
+- Sending messages to Claude containing up to 5 attachment files (txt, pdf, csv, png, jpeg, etc...) 10 MB each, images are also supported!
 - Retrieving chat message history, accessing specific chat conversations.
 - Deleting old chats when they are no longer needed.
 - Sending requests through proxies.
 
 ### Some of the key things you can do with Claude through this API
 
 - Ask questions about a wide variety of topics. Claude can chat about current events, pop culture, sports,
@@ -35,14 +35,16 @@
 
 - Get helpful explanations on complex topics. Ask Claude to explain concepts and ideas in simple terms.
 
 - Generate summaries from long text or documents. Just give the filepath as an attachment to Claude and get back a concise summary.
 
 - Receive thoughtful responses to open-ended prompts and ideas. Claude can brainstorm ideas, expand on concepts, and have philosophical discussions.
 
+- Send images and let Claude analyze them for you.
+
 ## How to install
 
 ```shell
 pip install unofficial-claude-api
 ```
 
 ## Uninstallation
@@ -252,27 +254,28 @@
 client = ClaudeAPIClient(session, proxy=socks_proxy)
 ```
 
 __________
 
 ### Changing Claude model
 
-In case you have accounts that are unable to migrate to latest model, you can override the `model_name` string parameter of `ClaudeAPIClient` constructor.
+In case you'd like to change the model used, or you do have accounts that are unable to migrate to latest model, you can override the `model_name` string parameter of `ClaudeAPIClient` constructor like so:
 
 ```py
 from claude_api.client import ClaudeAPIClient
 from claude_api.session import SessionData
 
 session = SessionData(...)
 
 # Defaults to None (latest Claude model)
-# Can be either claude-2.0 or claude-2.1
 client = ClaudeAPIClient(session, model_name="claude-2.0")
 ```
 
+You can retrieve the `model_name` strings from the [official API docs](https://docs.anthropic.com/claude/docs/models-overview#model-comparison)
+
 ## TROUBLESHOOTING
 
 Some common errors that may arise during the usage of this API:
 
 - *Error [400]* (Unable to prepare file attachment):
 
     To fix this error, change the extension of the attachment file to something like .txt, since by default this api will fallback to octet-stream for unknown file extensions, Claude may reject the file data.
```

### Comparing `unofficial-claude-api-0.3.1/claude_api/client.py` & `unofficial-claude-api-0.3.2/claude_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,18 +130,14 @@
 
         `proxy` argument is an optional `HTTPProxy` instance,
         holding proxy informations ( ip, port )
 
         Raises `ValueError` in case of failure
 
         """
-        if model_name is not None and model_name not in {"claude-2.0", "claude-2.1"}:
-            raise ValueError(
-                "model_name must be either None or one of 'claude-2.0' or 'claude-2.1' strings"
-            )
 
         self.model_name: str = model_name
         self.timeout: float = timeout
         self.proxy: ClaudeProxyT = proxy
         self.__session: SessionData = session
         if (
             not self.__session
@@ -231,15 +227,15 @@
         return mime_type or "application/octet-stream"
 
     def __prepare_file_attachment(self, fpath: str, chat_id: str) -> dict | None:
         content_type = self.__get_content_type(fpath)
         if content_type == "text/plain":
             return self.__prepare_text_file_attachment(fpath)
 
-        url = f"{self.__BASE_URL}/api/convert_document"
+        url = f"{self.__BASE_URL}/api/{self.__session.organization_id}/upload"
 
         headers = {
             "Host": "claude.ai",
             "User-Agent": self.__session.user_agent,
             "Accept": "*/*",
             "Accept-Language": "en-US,en;q=0.5",
             "Accept-Encoding": "gzip, deflate, br",
@@ -264,15 +260,17 @@
                 url,
                 headers=headers,
                 files=files,
                 timeout=self.timeout,
                 proxies=self.__get_proxy(),
             )
             if response.status_code == 200:
-                return response.json()
+                res = response.json()
+                if "file_uuid" in res:
+                    return res["file_uuid"]
         print(
             f"\n[{response.status_code}] Unable to prepare file attachment -> {fpath}\n"
             f"\nReason: {response.text}\n\n"
         )
         return None
 
     def __check_file_attachments_paths(self, path_list: list[str]):
@@ -548,35 +546,38 @@
         - `error_response` string field, which will be None in case of no errors.
         """
 
         self.__check_file_attachments_paths(attachment_paths)
 
         attachments = []
         if attachment_paths:
-            attachments = [
-                a
-                for a in [
-                    self.__prepare_file_attachment(path, chat_id)
-                    for path in attachment_paths
-                ]
-                if a
-            ]
+            for path in attachment_paths:
+                attachments.append(self.__prepare_file_attachment(path, chat_id))
 
         url = (
             f"{self.__BASE_URL}/api/organizations/"
             + f"{self.__session.organization_id}/chat_conversations/"
             + f"{chat_id}/completion"
         )
 
         payload = {
-            "attachments": attachments,
+            "attachments": [],
             "files": [],
             "prompt": prompt,
             "timezone": self.timezone,
         }
+
+        for a in attachments:
+            if isinstance(a, dict):
+                # Text file attachment
+                payload["attachments"].append(a)
+            elif isinstance(a, str):
+                # Other files uploaded
+                payload["files"].append(a)
+
         if self.model_name is not None:
             payload["model"] = self.model_name
 
         payload = dumps(
             payload,
             indent=None,
             separators=(",", ":"),
```

### Comparing `unofficial-claude-api-0.3.1/claude_api/errors.py` & `unofficial-claude-api-0.3.2/claude_api/errors.py`

 * *Files identical despite different names*

### Comparing `unofficial-claude-api-0.3.1/claude_api/session.py` & `unofficial-claude-api-0.3.2/claude_api/session.py`

 * *Files identical despite different names*

### Comparing `unofficial-claude-api-0.3.1/setup.py` & `unofficial-claude-api-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     encoding="utf-8",
     errors="ignore",
 ) as fp:
     __LONG_DESCRIPTION = fp.read().lstrip().rstrip()
 
 setup(
     name="unofficial-claude-api",
-    version="0.3.1",
+    version="0.3.2",
     author="st1vms",
     author_email="stefano.maria.salvatore@gmail.com",
     description=__DESCRIPTION,
     long_description=__LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/st1vms/unofficial-claude-api",
     packages=find_packages(),
```

### Comparing `unofficial-claude-api-0.3.1/unofficial_claude_api.egg-info/PKG-INFO` & `unofficial-claude-api-0.3.2/unofficial_claude_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unofficial-claude-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: This unofficial Python API provides access to the conversational capabilities of Anthropic's Claude AI through a simple chat messaging interface.
 Home-page: https://github.com/st1vms/unofficial-claude-api
 Author: st1vms
 Author-email: stefano.maria.salvatore@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,28 +24,28 @@
 - [Installation](#how-to-install)
 - [Requirements](#requirements)
 - [Example Usage](#example-usage)
 - [Tips](#tips)
   - [Retrieving Chat History](#retrieving-chat-history)
   - [Faster Loading](#faster-loading-avoiding-selenium)
   - [Proxies](#proxies)
-  - [Switching model version](#changing-claude-model)
+  - [Changing model version](#changing-claude-model)
 - [Troubleshooting](#troubleshooting)
 - [Donating](#donating)
 
 ## What is this?
 
 This unofficial Python API provides access to the conversational capabilities of Anthropic's Claude AI through a simple chat messaging interface.
 
 While not officially supported by Anthropic, this library can enable interesting conversational applications.
 
 It allows for:
 
 - Creating chat sessions with Claude and getting chat IDs.
-- Sending messages to Claude containing up to 5 attachment files (txt, pdf, csv, etc...) 10 MB each.
+- Sending messages to Claude containing up to 5 attachment files (txt, pdf, csv, png, jpeg, etc...) 10 MB each, images are also supported!
 - Retrieving chat message history, accessing specific chat conversations.
 - Deleting old chats when they are no longer needed.
 - Sending requests through proxies.
 
 ### Some of the key things you can do with Claude through this API
 
 - Ask questions about a wide variety of topics. Claude can chat about current events, pop culture, sports,
@@ -53,14 +53,16 @@
 
 - Get helpful explanations on complex topics. Ask Claude to explain concepts and ideas in simple terms.
 
 - Generate summaries from long text or documents. Just give the filepath as an attachment to Claude and get back a concise summary.
 
 - Receive thoughtful responses to open-ended prompts and ideas. Claude can brainstorm ideas, expand on concepts, and have philosophical discussions.
 
+- Send images and let Claude analyze them for you.
+
 ## How to install
 
 ```shell
 pip install unofficial-claude-api
 ```
 
 ## Uninstallation
@@ -270,27 +272,28 @@
 client = ClaudeAPIClient(session, proxy=socks_proxy)
 ```
 
 __________
 
 ### Changing Claude model
 
-In case you have accounts that are unable to migrate to latest model, you can override the `model_name` string parameter of `ClaudeAPIClient` constructor.
+In case you'd like to change the model used, or you do have accounts that are unable to migrate to latest model, you can override the `model_name` string parameter of `ClaudeAPIClient` constructor like so:
 
 ```py
 from claude_api.client import ClaudeAPIClient
 from claude_api.session import SessionData
 
 session = SessionData(...)
 
 # Defaults to None (latest Claude model)
-# Can be either claude-2.0 or claude-2.1
 client = ClaudeAPIClient(session, model_name="claude-2.0")
 ```
 
+You can retrieve the `model_name` strings from the [official API docs](https://docs.anthropic.com/claude/docs/models-overview#model-comparison)
+
 ## TROUBLESHOOTING
 
 Some common errors that may arise during the usage of this API:
 
 - *Error [400]* (Unable to prepare file attachment):
 
     To fix this error, change the extension of the attachment file to something like .txt, since by default this api will fallback to octet-stream for unknown file extensions, Claude may reject the file data.
```

