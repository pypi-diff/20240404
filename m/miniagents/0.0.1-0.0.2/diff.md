# Comparing `tmp/miniagents-0.0.1.tar.gz` & `tmp/miniagents-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniagents-0.0.1.tar", max compression
+gzip compressed data, was "miniagents-0.0.2.tar", max compression
```

## Comparing `miniagents-0.0.1.tar` & `miniagents-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.1/LICENSE
--rw-r--r--   0        0        0      503 2024-03-27 07:32:21.725319 miniagents-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.1/miniagents/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.1/miniagents/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.1/miniagents/ext/llms/__init__.py
--rw-r--r--   0        0        0     1446 2024-03-27 07:32:21.726119 miniagents-0.0.1/miniagents/ext/llms/anthropic.py
--rw-r--r--   0        0        0     1288 2024-03-27 07:32:21.726251 miniagents-0.0.1/miniagents/miniagents.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.1/miniagents/promisegraph/__init__.py
--rw-r--r--   0        0        0     2228 2024-03-27 07:32:21.726518 miniagents-0.0.1/miniagents/promisegraph/node.py
--rw-r--r--   0        0        0     7950 2024-03-27 07:32:21.726659 miniagents-0.0.1/miniagents/promisegraph/promise.py
--rw-r--r--   0        0        0      262 2024-03-27 07:32:21.726770 miniagents-0.0.1/miniagents/promisegraph/sentinels.py
--rw-r--r--   0        0        0      694 2024-03-27 07:32:21.727656 miniagents-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 miniagents-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.2/LICENSE
+-rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.2/miniagents/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.2/miniagents/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.2/miniagents/ext/llms/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-04 08:27:28.367395 miniagents-0.0.2/miniagents/ext/llms/anthropic.py
+-rw-r--r--   0        0        0     5170 2024-04-04 17:06:05.253979 miniagents-0.0.2/miniagents/miniagents.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.2/miniagents/promisegraph/__init__.py
+-rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.2/miniagents/promisegraph/errors.py
+-rw-r--r--   0        0        0     2228 2024-03-27 07:32:21.726518 miniagents-0.0.2/miniagents/promisegraph/node.py
+-rw-r--r--   0        0        0    12613 2024-04-03 21:42:22.426837 miniagents-0.0.2/miniagents/promisegraph/promise.py
+-rw-r--r--   0        0        0      307 2024-04-02 17:38:48.002385 miniagents-0.0.2/miniagents/promisegraph/sentinels.py
+-rw-r--r--   0        0        0     1748 2024-04-02 21:38:18.181306 miniagents-0.0.2/miniagents/promisegraph/sequence.py
+-rw-r--r--   0        0        0     1482 2024-04-03 21:42:22.427374 miniagents-0.0.2/miniagents/promisegraph/typing.py
+-rw-r--r--   0        0        0      694 2024-03-27 08:48:49.718186 miniagents-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.2/PKG-INFO
```

### Comparing `miniagents-0.0.1/LICENSE` & `miniagents-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.1/miniagents/ext/llms/anthropic.py` & `miniagents-0.0.2/miniagents/ext/llms/anthropic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,62 @@
 """
 This module integrates Anthropic language models with MiniAgents.
 """
 
 from typing import AsyncIterator, Any
 
-from miniagents.miniagents import MessagePromise
+from miniagents.miniagents import MessagePromise, MessageType, MessageSequence, Message
 
 
-def anthropic(schedule_immediately: bool = True, stream: bool = True, **kwargs) -> MessagePromise:
+def anthropic(
+    messages: MessageType,
+    schedule_immediately: bool = True,
+    collect_as_soon_as_possible: bool = True,
+    stream: bool = True,
+    **kwargs,
+) -> MessagePromise:
     """
     Run text generation with Anthropic.
     """
     # pylint: disable=import-outside-toplevel
     import anthropic as anthropic_original
 
-    # TODO Oleksandr: instantiate the client only once but don't import `anthropic` at the module level
+    # TODO Oleksandr: instantiate the client only once (but still don't import `anthropic` at the module level)
     client = anthropic_original.AsyncAnthropic()
 
-    async def msg_piece_producer(_: dict[str, Any]) -> AsyncIterator[str]:
+    async def message_piece_producer(_: dict[str, Any]) -> AsyncIterator[str]:
         # TODO Oleksandr: collect metadata_so_far
+        collected_messages = await MessageSequence.aflatten_and_collect(messages)
+        message_dicts = [_message_to_anthropic_dict(msg) for msg in collected_messages]
+
         if stream:
-            async with client.messages.stream(**kwargs) as response:  # pylint: disable=not-async-context-manager
+            # pylint: disable=not-async-context-manager
+            async with client.messages.stream(messages=message_dicts, **kwargs) as response:
                 async for token in response.text_stream:
                     yield token
         else:
-            response = await client.messages.create(stream=False, **kwargs)
+            response = await client.messages.create(messages=message_dicts, stream=False, **kwargs)
             if len(response.content) != 1:
                 raise RuntimeError(
                     f"exactly one message should have been returned by Anthropic, "
                     f"but {len(response.content)} were returned instead"
                 )
             yield response.content[0].text  # yield the whole text as one "piece"
 
-    return MessagePromise(msg_piece_producer=msg_piece_producer, schedule_immediately=schedule_immediately)
+    return MessagePromise(
+        message_piece_producer=message_piece_producer,
+        schedule_immediately=schedule_immediately,
+        collect_as_soon_as_possible=collect_as_soon_as_possible,
+    )
+
+
+def _message_to_anthropic_dict(message: Message) -> dict[str, Any]:
+    # TODO Oleksandr: introduce a lambda function to derive roles from messages ?
+    try:
+        role = message.role
+    except AttributeError:
+        role = getattr(message, "anthropic_role", "user")
+
+    return {
+        "role": role,
+        "content": message.text,
+    }
```

### Comparing `miniagents-0.0.1/miniagents/promisegraph/node.py` & `miniagents-0.0.2/miniagents/promisegraph/node.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.1/pyproject.toml` & `miniagents-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 119
 
 [tool.coverage.run]
 branch = true
 
 [tool.poetry]
 name = "miniagents"
-version = "0.0.1"
+version = "0.0.2"
 description = """\
 TODO Oleksandr\
 """
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 homepage = "https://github.com/teremterem/MiniAgents"
 readme = "README.md"
 license = "MIT"
```

