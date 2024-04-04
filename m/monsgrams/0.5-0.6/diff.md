# Comparing `tmp/monsgrams-0.5.tar.gz` & `tmp/monsgrams-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.5.tar", last modified: Thu Apr  4 19:03:46 2024, max compression
+gzip compressed data, was "monsgrams-0.6.tar", last modified: Thu Apr  4 19:17:38 2024, max compression
```

## Comparing `monsgrams-0.5.tar` & `monsgrams-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:03:46.488426 monsgrams-0.5/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      627 2024-04-04 19:03:46.484426 monsgrams-0.5/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      446 2024-04-04 19:03:35.000000 monsgrams-0.5/README.md
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:03:46.472426 monsgrams-0.5/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       22 2024-04-04 18:09:05.000000 monsgrams-0.5/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      412 2024-04-04 18:43:28.000000 monsgrams-0.5/monsgrams/api.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     1139 2024-04-04 18:58:08.000000 monsgrams-0.5/monsgrams/main.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:03:46.484426 monsgrams-0.5/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      627 2024-04-04 19:03:45.000000 monsgrams-0.5/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      207 2024-04-04 19:03:46.000000 monsgrams-0.5/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 19:03:46.000000 monsgrams-0.5/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 19:03:46.000000 monsgrams-0.5/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 19:03:46.492426 monsgrams-0.5/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      333 2024-04-04 19:02:38.000000 monsgrams-0.5/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:17:38.956426 monsgrams-0.6/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      615 2024-04-04 19:17:38.952426 monsgrams-0.6/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      434 2024-04-04 19:14:44.000000 monsgrams-0.6/README.md
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:17:38.940426 monsgrams-0.6/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       22 2024-04-04 18:09:05.000000 monsgrams-0.6/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      412 2024-04-04 18:43:28.000000 monsgrams-0.6/monsgrams/api.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     1337 2024-04-04 19:15:40.000000 monsgrams-0.6/monsgrams/main.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:17:38.948426 monsgrams-0.6/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      615 2024-04-04 19:17:38.000000 monsgrams-0.6/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      207 2024-04-04 19:17:38.000000 monsgrams-0.6/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 19:17:38.000000 monsgrams-0.6/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 19:17:38.000000 monsgrams-0.6/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 19:17:38.956426 monsgrams-0.6/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      333 2024-04-04 19:17:04.000000 monsgrams-0.6/setup.py
```

### Comparing `monsgrams-0.5/monsgrams/main.py` & `monsgrams-0.6/monsgrams/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import asyncio
 import aiohttp
 from api import TelegramAPI
 
 class Bot:
-  def __init__(self, token):
-    self.api = TelegramAPI(token)
-    self.commands = {}
-  
-  def get_updates(self, offset=None):
-    url = self.api.base_url + "getUpdates"
-    params = {"offset": offset} if offset else {}
-    async with aiohttp.ClientSession() as session:
-      async with session.get(url, params=params) as response:
-        return response.json()
-  
-  def command(self, name):
-    def decorator(func):
-      self.commands[name] = func
-      return func
-    return decorator
-  
-  async def polling_loop(bot):
-    offset = None
-    while True:
-      updates = await bot.get_updates(offset)
-      for update in updates.get("result", []):
-        offset = update["update_id"] + 1
-        message = update.get("message", {})
-        text = message.get("text", "")
-        chat_id = message.get("chat", {}).get("id")
-        if text.startswith("/"):
-          command_name = text.split()[0][1:]
-          command = bot.commands.get(command_name)
-          if command:
-            await command(bot, chat_id)
-          else:
-            print("not found cmd")
+    def __init__(self, token):
+        self.api = TelegramAPI(token)
+        self.commands = {}
+
+    async def get_updates(self, offset=None):
+        url = self.api.base_url + "getUpdates"
+        params = {"offset": offset} if offset else {}
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, params=params) as response:
+                return await response.json()
+
+    def command(self, name):
+        def decorator(func):
+            self.commands[name] = func
+            return func
+        return decorator
+
+    async def polling_loop(self):
+        offset = None
+        while True:
+            updates = await self.get_updates(offset)
+            for update in updates.get("result", []):
+                offset = update["update_id"] + 1
+                message = update.get("message", {})
+                text = message.get("text", "")
+                chat_id = message.get("chat", {}).get("id")
+                if text.startswith("/"):
+                    command_name = text.split()[0][1:]
+                    command = self.commands.get(command_name)
+                    if command:
+                        await command(self, chat_id)
+                    else:
+                        print("not found cmd")
+
```

