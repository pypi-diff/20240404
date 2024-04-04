# Comparing `tmp/uagents_ai_engine-0.1.3.tar.gz` & `tmp/uagents_ai_engine-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_ai_engine-0.1.3.tar", max compression
+gzip compressed data, was "uagents_ai_engine-0.1.4.tar", max compression
```

## Comparing `uagents_ai_engine-0.1.3.tar` & `uagents_ai_engine-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      209 2024-03-15 19:58:48.912304 uagents_ai_engine-0.1.3/README.md
--rw-r--r--   0        0        0      394 2024-03-22 11:42:47.916667 uagents_ai_engine-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       89 2024-03-15 19:58:57.112803 uagents_ai_engine-0.1.3/src/ai_engine/__init__.py
--rw-r--r--   0        0        0     4487 2024-03-28 09:54:43.757710 uagents_ai_engine-0.1.3/src/ai_engine/chitchat.py
--rw-r--r--   0        0        0     2284 2024-03-25 05:19:14.446118 uagents_ai_engine-0.1.3/src/ai_engine/dialogue.py
--rw-r--r--   0        0        0     2964 2024-03-28 14:22:24.183225 uagents_ai_engine-0.1.3/src/ai_engine/messages.py
--rw-r--r--   0        0        0      765 2024-03-15 19:58:48.914653 uagents_ai_engine-0.1.3/src/ai_engine/types.py
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 uagents_ai_engine-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-03-15 19:58:48.912304 uagents_ai_engine-0.1.4/README.md
+-rw-r--r--   0        0        0      394 2024-04-04 04:34:53.008543 uagents_ai_engine-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-03-15 19:58:57.112803 uagents_ai_engine-0.1.4/src/ai_engine/__init__.py
+-rw-r--r--   0        0        0     4487 2024-04-04 04:31:33.596581 uagents_ai_engine-0.1.4/src/ai_engine/chitchat.py
+-rw-r--r--   0        0        0     2284 2024-04-04 04:31:33.596720 uagents_ai_engine-0.1.4/src/ai_engine/dialogue.py
+-rw-r--r--   0        0        0     2948 2024-04-04 04:32:05.223246 uagents_ai_engine-0.1.4/src/ai_engine/messages.py
+-rw-r--r--   0        0        0      765 2024-03-15 19:58:48.914653 uagents_ai_engine-0.1.4/src/ai_engine/types.py
+-rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 uagents_ai_engine-0.1.4/PKG-INFO
```

### Comparing `uagents_ai_engine-0.1.3/src/ai_engine/chitchat.py` & `uagents_ai_engine-0.1.4/src/ai_engine/chitchat.py`

 * *Files identical despite different names*

### Comparing `uagents_ai_engine-0.1.3/src/ai_engine/dialogue.py` & `uagents_ai_engine-0.1.4/src/ai_engine/dialogue.py`

 * *Files identical despite different names*

### Comparing `uagents_ai_engine-0.1.3/src/ai_engine/messages.py` & `uagents_ai_engine-0.1.4/src/ai_engine/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pydantic import BaseModel, Field, Extra
 from typing import Optional
 from uagents import Model
 from uuid import UUID, uuid4
-from datetime import datetime, UTC
-from typing import Optional, List, Annotated, Optional, Literal, Union
+from datetime import datetime
+from typing import Optional, List, Optional, Literal, Union
 
 
 # here are some message types that is currently supported by DeltaV
 
 
 class KeyValue(BaseModel):
     """Key value pair for options"""
@@ -46,15 +46,15 @@
     message_id: UUID = Field(
         default_factory=uuid4,
         description="Unique message ID, never ask for this. Ignore this field! It's set automatically.",
     )
 
     # timestamp of the message creation
     timestamp: datetime = Field(
-        default_factory=lambda: datetime.now(UTC),
+        default_factory=lambda: datetime.utcnow(),
         description="Timestamp of the message creation. Ignore this field! It's set automatically.",
     )
 
     class Config:
         extra = Extra.allow
```

### Comparing `uagents_ai_engine-0.1.3/src/ai_engine/types.py` & `uagents_ai_engine-0.1.4/src/ai_engine/types.py`

 * *Files identical despite different names*

### Comparing `uagents_ai_engine-0.1.3/PKG-INFO` & `uagents_ai_engine-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents-ai-engine
-Version: 0.1.3
+Version: 0.1.4
 Summary: Integrating AI-Engine with UAgents
 License: Apache 2.0
 Keywords: uagents,agents,ai,ai-engine,fetch.ai
 Author: Fetch.AI Limited
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

