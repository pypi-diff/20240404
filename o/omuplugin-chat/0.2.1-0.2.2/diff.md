# Comparing `tmp/omuplugin_chat-0.2.1.tar.gz` & `tmp/omuplugin_chat-0.2.2.tar.gz`

## Comparing `omuplugin_chat-0.2.1.tar` & `omuplugin_chat-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/src/omuplugin_chat/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/src/omuplugin_chat/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.2/.python-version
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.2/src/omuplugin_chat/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.2/src/omuplugin_chat/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.2/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.2/PKG-INFO
```

### Comparing `omuplugin_chat-0.2.1/src/omuplugin_chat/plugin.py` & `omuplugin_chat-0.2.2/src/omuplugin_chat/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import re
 from typing import List
 
 import iwashi
 from omu import Address, OmuClient
 from omuchat import App
 from omuchat.chat import (
+    AUTHOR_TABLE,
+    CHANNEL_TABLE,
+    CREATE_CHANNEL_TREE_ENDPOINT,
     IDENTIFIER,
-    AuthorsTableKey,
-    ChannelsTableKey,
-    CreateChannelTreeEndpoint,
-    MessagesTableKey,
-    ProviderTableKey,
-    RoomTableKey,
+    MESSAGE_TABLE,
+    PROVIDER_TABLE,
+    ROOM_TABLE,
 )
 from omuchat.model.channel import Channel
 
 app = App(
     IDENTIFIER,
     description="",
     version="0.1.0",
@@ -23,24 +23,24 @@
     license="MIT",
     repository_url="https://github.com/OMUCHAT",
 )
 address = Address("127.0.0.1", 26423)
 client = OmuClient(app, address=address)
 
 
-messages = client.tables.get(MessagesTableKey)
-authors = client.tables.get(AuthorsTableKey)
+messages = client.tables.get(MESSAGE_TABLE)
+authors = client.tables.get(AUTHOR_TABLE)
 messages.set_config({"cache_size": 1000})
 authors.set_config({"cache_size": 500})
-channels = client.tables.get(ChannelsTableKey)
-providers = client.tables.get(ProviderTableKey)
-rooms = client.tables.get(RoomTableKey)
+channels = client.tables.get(CHANNEL_TABLE)
+providers = client.tables.get(PROVIDER_TABLE)
+rooms = client.tables.get(ROOM_TABLE)
 
 
-@client.endpoints.bind(endpoint_type=CreateChannelTreeEndpoint)
+@client.endpoints.bind(endpoint_type=CREATE_CHANNEL_TREE_ENDPOINT)
 async def create_channel_tree(url: str) -> List[Channel]:
     results = await iwashi.visit(url)
     if results is None:
         return []
     channels: List[Channel] = []
     services = await providers.fetch_items()
     for result in results.to_list():
```

### Comparing `omuplugin_chat-0.2.1/pyproject.toml` & `omuplugin_chat-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_chat"
-version = "0.2.1"
+version = "0.2.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

