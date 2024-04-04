# Comparing `tmp/mirascope-0.8.2.tar.gz` & `tmp/mirascope-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirascope-0.8.2.tar", max compression
+gzip compressed data, was "mirascope-0.8.3.tar", max compression
```

## Comparing `mirascope-0.8.2.tar` & `mirascope-0.8.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1072 2024-04-02 23:05:45.065715 mirascope-0.8.2/LICENSE
--rw-r--r--   0        0        0    10093 2024-04-02 23:05:45.065715 mirascope-0.8.2/docs/README.md
--rw-r--r--   0        0        0      472 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/__init__.py
--rw-r--r--   0        0        0      270 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/anthropic/__init__.py
--rw-r--r--   0        0        0     8617 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/anthropic/calls.py
--rw-r--r--   0        0        0     3758 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/anthropic/extractors.py
--rw-r--r--   0        0        0        0 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/anthropic/py.typed
--rw-r--r--   0        0        0     9642 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/anthropic/tools.py
--rw-r--r--   0        0        0     6208 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/anthropic/types.py
--rw-r--r--   0        0        0      453 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/base/__init__.py
--rw-r--r--   0        0        0     3645 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/base/calls.py
--rw-r--r--   0        0        0     8303 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/base/extractors.py
--rw-r--r--   0        0        0     5696 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/base/prompts.py
--rw-r--r--   0        0        0        0 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/base/py.typed
--rw-r--r--   0        0        0     2890 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/base/tools.py
--rw-r--r--   0        0        0     5313 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/base/types.py
--rw-r--r--   0        0        0     5615 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/base/utils.py
--rw-r--r--   0        0        0       97 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/__init__.py
--rw-r--r--   0        0        0      199 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/commands/__init__.py
--rw-r--r--   0        0        0     4213 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/commands/add.py
--rw-r--r--   0        0        0     3002 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/commands/init.py
--rw-r--r--   0        0        0        0 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/commands/py.typed
--rw-r--r--   0        0        0     3101 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/commands/remove.py
--rw-r--r--   0        0        0     2008 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/commands/status.py
--rw-r--r--   0        0        0     2801 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/commands/use.py
--rw-r--r--   0        0        0      118 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/constants.py
--rw-r--r--   0        0        0       86 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/generic/__init__.py
--rw-r--r--   0        0        0      494 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/generic/mirascope.ini.j2
--rw-r--r--   0        0        0     1554 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/generic/prompt_template.j2
--rw-r--r--   0        0        0     1067 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/py.typed
--rw-r--r--   0        0        0     1197 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/schemas.py
--rw-r--r--   0        0        0    24322 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/cli/utils.py
--rw-r--r--   0        0        0     1552 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/enums.py
--rw-r--r--   0        0        0      241 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/gemini/__init__.py
--rw-r--r--   0        0        0     6333 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/gemini/calls.py
--rw-r--r--   0        0        0     3730 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/gemini/extractors.py
--rw-r--r--   0        0        0     4081 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/gemini/tools.py
--rw-r--r--   0        0        0     4666 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/gemini/types.py
--rw-r--r--   0        0        0      239 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/mistral/__init__.py
--rw-r--r--   0        0        0     5900 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/mistral/calls.py
--rw-r--r--   0        0        0     3940 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/mistral/extractors.py
--rw-r--r--   0        0        0        0 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/mistral/py.typed
--rw-r--r--   0        0        0     3896 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/mistral/tools.py
--rw-r--r--   0        0        0     6132 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/mistral/types.py
--rw-r--r--   0        0        0      232 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/openai/__init__.py
--rw-r--r--   0        0        0     6461 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/openai/calls.py
--rw-r--r--   0        0        0     3932 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/openai/extractors.py
--rw-r--r--   0        0        0        0 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/openai/py.typed
--rw-r--r--   0        0        0     3860 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/openai/tools.py
--rw-r--r--   0        0        0     7925 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/openai/types.py
--rw-r--r--   0        0        0        0 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/py.typed
--rw-r--r--   0        0        0      151 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/wandb/__init__.py
--rw-r--r--   0        0        0     9593 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/wandb/wandb.py
--rw-r--r--   0        0        0     1921 2024-04-02 23:05:45.069715 mirascope-0.8.2/mirascope/wandb/weave.py
--rw-r--r--   0        0        0     2763 2024-04-02 23:05:45.073716 mirascope-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    11526 1970-01-01 00:00:00.000000 mirascope-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-04 01:09:48.611045 mirascope-0.8.3/LICENSE
+-rw-r--r--   0        0        0    10093 2024-04-04 01:09:48.611045 mirascope-0.8.3/docs/README.md
+-rw-r--r--   0        0        0      472 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/__init__.py
+-rw-r--r--   0        0        0      270 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/__init__.py
+-rw-r--r--   0        0        0     8732 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/calls.py
+-rw-r--r--   0        0        0     4088 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/py.typed
+-rw-r--r--   0        0        0     9642 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/tools.py
+-rw-r--r--   0        0        0     6705 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/anthropic/types.py
+-rw-r--r--   0        0        0      453 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/__init__.py
+-rw-r--r--   0        0        0     3645 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/calls.py
+-rw-r--r--   0        0        0     8304 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/extractors.py
+-rw-r--r--   0        0        0     5696 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/prompts.py
+-rw-r--r--   0        0        0        0 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/py.typed
+-rw-r--r--   0        0        0     2890 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/tools.py
+-rw-r--r--   0        0        0     5313 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/types.py
+-rw-r--r--   0        0        0     5615 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/base/utils.py
+-rw-r--r--   0        0        0       97 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4213 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/add.py
+-rw-r--r--   0        0        0     3002 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/init.py
+-rw-r--r--   0        0        0        0 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/py.typed
+-rw-r--r--   0        0        0     3101 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/remove.py
+-rw-r--r--   0        0        0     2008 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/status.py
+-rw-r--r--   0        0        0     2801 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/commands/use.py
+-rw-r--r--   0        0        0      118 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/constants.py
+-rw-r--r--   0        0        0       86 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/generic/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/generic/mirascope.ini.j2
+-rw-r--r--   0        0        0     1554 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/generic/prompt_template.j2
+-rw-r--r--   0        0        0     1067 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/py.typed
+-rw-r--r--   0        0        0     1197 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/schemas.py
+-rw-r--r--   0        0        0    24322 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/cli/utils.py
+-rw-r--r--   0        0        0     1552 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/enums.py
+-rw-r--r--   0        0        0      241 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/__init__.py
+-rw-r--r--   0        0        0     6333 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/calls.py
+-rw-r--r--   0        0        0     3730 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/extractors.py
+-rw-r--r--   0        0        0     4081 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/tools.py
+-rw-r--r--   0        0        0     4950 2024-04-04 01:09:48.615045 mirascope-0.8.3/mirascope/gemini/types.py
+-rw-r--r--   0        0        0      239 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/__init__.py
+-rw-r--r--   0        0        0     5900 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/calls.py
+-rw-r--r--   0        0        0     3940 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/py.typed
+-rw-r--r--   0        0        0     3896 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/tools.py
+-rw-r--r--   0        0        0     6389 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/mistral/types.py
+-rw-r--r--   0        0        0      232 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/__init__.py
+-rw-r--r--   0        0        0     9068 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/calls.py
+-rw-r--r--   0        0        0     3932 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/py.typed
+-rw-r--r--   0        0        0     3860 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/tools.py
+-rw-r--r--   0        0        0     9087 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/openai/types.py
+-rw-r--r--   0        0        0        0 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/py.typed
+-rw-r--r--   0        0        0      151 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/wandb/__init__.py
+-rw-r--r--   0        0        0     9593 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/wandb/wandb.py
+-rw-r--r--   0        0        0     1921 2024-04-04 01:09:48.619045 mirascope-0.8.3/mirascope/wandb/weave.py
+-rw-r--r--   0        0        0     2763 2024-04-04 01:09:48.619045 mirascope-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0    11526 1970-01-01 00:00:00.000000 mirascope-0.8.3/PKG-INFO
```

### Comparing `mirascope-0.8.2/LICENSE` & `mirascope-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/docs/README.md` & `mirascope-0.8.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/anthropic/calls.py` & `mirascope-0.8.3/mirascope/anthropic/calls.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,16 @@
         dict[str, Any],
         Optional[list[Type[AnthropicTool]]],
     ]:
         """Overrides the `BaseCall._setup` for Anthropic specific setup."""
         kwargs, tool_types = self._setup(kwargs, AnthropicTool)
         messages = self.messages()
         system_message = ""
+        if "system" in kwargs and kwargs["system"] is not None:
+            system_message += kwargs.pop("system")
         if messages[0]["role"] == "system":
             system_message += messages.pop(0)["content"]
         if tool_types:
             tool_schemas = kwargs.pop("tools")
             system_message += self._write_tools_system_message(tool_schemas)
             kwargs["stop_sequences"] = ["</function_calls>"]
         if system_message:
```

### Comparing `mirascope-0.8.2/mirascope/anthropic/extractors.py` & `mirascope-0.8.3/mirascope/anthropic/extractors.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 from .types import AnthropicCallParams
 
 logger = logging.getLogger("mirascope")
 
 T = TypeVar("T", bound=ExtractedType)
 
 
+EXTRACT_SYSTEM_MESSAGE = """
+OUTPUT ONLY FUNCTION CALLS WITHOUT ANY ADDITIONAL TEXT.
+You must wrap all invoke calls in the <function_calls> tag.
+ONLY EXTRACT ANSWERS THAT YOU ARE ABSOLUTELY 100% CERTAIN ARE CORRECT.
+""".strip()
+
+
 class AnthropicExtractor(BaseExtractor[AnthropicCall, AnthropicTool, T], Generic[T]):
     '''A class for extracting structured information using Anthropic Claude models.
 
     Example:
 
     ```python
     from typing import Literal, Type
@@ -70,14 +77,15 @@
         Returns:
             The `Schema` instance extracted from the completion.
 
         Raises:
             AttributeError: if there is no tool in the call creation.
             ValidationError: if the schema cannot be instantiated from the completion.
         """
+        kwargs["system"] = EXTRACT_SYSTEM_MESSAGE
         return self._extract(AnthropicCall, AnthropicTool, retries, **kwargs)
 
     async def extract_async(self, retries: int = 0, **kwargs: Any) -> T:
         """Asynchronously extracts `extract_schema` from the Anthropic call response.
 
         The `extract_schema` is converted into an `AnthropicTool`, complete with a
         description of the tool, all of the fields, and their types. This allows us to
@@ -93,10 +101,11 @@
         Returns:
             The `Schema` instance extracted from the completion.
 
         Raises:
             AttributeError: if there is no tool in the call creation.
             ValidationError: if the schema cannot be instantiated from the completion.
         """
+        kwargs["system"] = EXTRACT_SYSTEM_MESSAGE
         return await self._extract_async(
             AnthropicCall, AnthropicTool, retries, **kwargs
         )
```

### Comparing `mirascope-0.8.2/mirascope/anthropic/tools.py` & `mirascope-0.8.3/mirascope/anthropic/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/anthropic/types.py` & `mirascope-0.8.3/mirascope/anthropic/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type classes for interacting with Anthropics's Claude API."""
+
 import xml.etree.ElementTree as ET
 from typing import Any, Callable, Literal, Optional, Type, Union, cast
 
 from anthropic import Anthropic, AsyncAnthropic
 from anthropic._types import Body, Headers, Query
 from anthropic.types import (
     ContentBlockDeltaEvent,
@@ -86,20 +87,29 @@
     print(BookRecommender().call())
     ```
     """
 
     @property
     def tools(self) -> Optional[list[AnthropicTool]]:
         """Returns the tools for the 0th choice message."""
+        if not self.tool_types:
+            return None
+
         if (
-            not self.tool_types
-            or self.response.stop_reason != "stop_sequence"
+            self.response.stop_reason != "stop_sequence"
             or self.response.stop_sequence != "</function_calls>"
         ):
-            return None
+            raise RuntimeError(
+                "Generation stopped before `</function_calls>` stop sequence. "
+                "This is likely due to a limit on output tokens that is too low. "
+                "Note that this could also indicate no tool is beind called, so we "
+                "recommend that you check the output of the call to confirm. "
+                f"Stop Reason: {self.response.stop_reason} "
+                f"Stop Sequence: {self.response.stop_sequence}"
+            )
 
         try:
             root_node = ET.fromstring(
                 f"<wrapper>{self.response.content}</function_calls></wrapper>"
             )
         except ET.ParseError as e:
             raise ValueError("Unable to parse tools from response") from e
```

### Comparing `mirascope-0.8.2/mirascope/base/calls.py` & `mirascope-0.8.3/mirascope/base/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/base/extractors.py` & `mirascope-0.8.3/mirascope/base/extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A base abstract interface for extracting structured information using LLMs."""
+
 import logging
 from abc import ABC, abstractmethod
 from enum import Enum
 from inspect import isclass
 from typing import (
     Annotated,
     Any,
```

### Comparing `mirascope-0.8.2/mirascope/base/prompts.py` & `mirascope-0.8.3/mirascope/base/prompts.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/base/tools.py` & `mirascope-0.8.3/mirascope/base/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/base/types.py` & `mirascope-0.8.3/mirascope/base/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/base/utils.py` & `mirascope-0.8.3/mirascope/base/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/commands/add.py` & `mirascope-0.8.3/mirascope/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/commands/init.py` & `mirascope-0.8.3/mirascope/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/commands/remove.py` & `mirascope-0.8.3/mirascope/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/commands/status.py` & `mirascope-0.8.3/mirascope/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/commands/use.py` & `mirascope-0.8.3/mirascope/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/generic/prompt_template.j2` & `mirascope-0.8.3/mirascope/cli/generic/prompt_template.j2`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/main.py` & `mirascope-0.8.3/mirascope/cli/main.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/schemas.py` & `mirascope-0.8.3/mirascope/cli/schemas.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/cli/utils.py` & `mirascope-0.8.3/mirascope/cli/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/enums.py` & `mirascope-0.8.3/mirascope/enums.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/gemini/calls.py` & `mirascope-0.8.3/mirascope/gemini/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/gemini/extractors.py` & `mirascope-0.8.3/mirascope/gemini/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/gemini/tools.py` & `mirascope-0.8.3/mirascope/gemini/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/gemini/types.py` & `mirascope-0.8.3/mirascope/gemini/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,23 @@
 
     @property
     def tools(self) -> Optional[list[GeminiTool]]:
         """Returns the list of tools for the 0th candidate's 0th content part."""
         if self.tool_types is None:
             return None
 
+        if self.response.candidates[0].finish_reason != 1:  # STOP = 1
+            raise RuntimeError(
+                "Generation stopped before the stop sequence. "
+                "This is likely due to a limit on output tokens that is too low. "
+                "Note that this could also indicate no tool is beind called, so we "
+                "recommend that you check the output of the call to confirm."
+                f"Finish Reason: {self.response.candidates[0].finish_reason}"
+            )
+
         tool_calls = [
             part.function_call for part in self.response.candidates[0].content.parts
         ]
 
         extracted_tools = []
         for tool_call in tool_calls:
             for tool_type in self.tool_types:
@@ -96,22 +105,17 @@
     @property
     def tool(self) -> Optional[GeminiTool]:
         """Returns the 0th tool for the 0th candidate's 0th content part.
 
         Raises:
             ValidationError: if the tool call doesn't match the tool's schema.
         """
-        if self.tool_types is None:
-            return None
-
-        tool_call = self.response.candidates[0].content.parts[0].function_call
-        for tool_type in self.tool_types:
-            if tool_call.name == tool_type.__name__:
-                return tool_type.from_tool_call(tool_call)
-
+        tools = self.tools
+        if tools:
+            return tools[0]
         return None
 
     @property
     def content(self) -> str:
         """Returns the contained string content for the 0th choice."""
         return self.response.candidates[0].content.parts[0].text
```

### Comparing `mirascope-0.8.2/mirascope/mistral/calls.py` & `mirascope-0.8.3/mirascope/mistral/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/mistral/extractors.py` & `mirascope-0.8.3/mirascope/mistral/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/mistral/tools.py` & `mirascope-0.8.3/mirascope/mistral/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/mistral/types.py` & `mirascope-0.8.3/mirascope/mistral/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,14 +100,23 @@
 
         Raises:
             ValidationError: if the tool call doesn't match the tool's schema.
         """
         if not self.tool_types or not self.tool_calls or len(self.tool_calls) == 0:
             return None
 
+        if self.choices[0].finish_reason != "tool_calls":
+            raise RuntimeError(
+                "Finish reason was not `tool_call`, indicating no or failed tool use."
+                "This is likely due to a limit on output tokens that is too low. "
+                "Note that this could also indicate no tool is beind called, so we "
+                "recommend that you check the output of the call to confirm. "
+                f"Finish Reason: {self.choices[0].finish_reason}"
+            )
+
         extracted_tools = []
         for tool_call in self.tool_calls:
             for tool_type in self.tool_types:
                 if tool_call.function.name == tool_type.__name__:
                     extracted_tools.append(tool_type.from_tool_call(tool_call))
                     break
 
@@ -116,22 +125,17 @@
     @property
     def tool(self) -> Optional[MistralTool]:
         """Returns the 0th tool for the 0th choice message.
 
         Raises:
             ValidationError: if the tool call doesn't match the tool's schema.
         """
-        if not self.tool_types or not self.tool_calls or len(self.tool_calls) == 0:
-            return None
-
-        tool_call = self.tool_calls[0]
-        for tool_type in self.tool_types:
-            if self.tool_calls[0].function.name == tool_type.__name__:
-                return tool_type.from_tool_call(tool_call)
-
+        tools = self.tools
+        if tools:
+            return tools[0]
         return None
 
     def dump(self) -> dict[str, Any]:
         """Dumps the response to a dictionary."""
         return {
             "start_time": self.start_time,
             "end_time": self.end_time,
```

### Comparing `mirascope-0.8.2/mirascope/openai/calls.py` & `mirascope-0.8.3/mirascope/openai/calls.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 """A module for calling OpenAI's Chat Completion models."""
 import datetime
-from typing import Any, AsyncGenerator, ClassVar, Generator
+import json
+from typing import Any, AsyncGenerator, ClassVar, Generator, Optional, Type
 
 from openai import AsyncOpenAI, OpenAI
 from openai.types.chat import (
     ChatCompletionAssistantMessageParam,
     ChatCompletionMessageParam,
     ChatCompletionSystemMessageParam,
     ChatCompletionToolMessageParam,
     ChatCompletionUserMessageParam,
 )
+from openai.types.chat.completion_create_params import ResponseFormat
 
 from ..base import BaseCall
 from ..enums import MessageRole
 from .tools import OpenAITool
 from .types import OpenAICallParams, OpenAICallResponse, OpenAICallResponseChunk
 
+JSON_MODE_CONTENT = """
+Extract a valid JSON object instance from to content using the following schema:
+
+{schema}
+""".strip()
+
+
+def _json_mode_content(tool_type: Type[OpenAITool]) -> str:
+    """Returns the formatted `JSON_MODE_CONTENT` with the given tool type."""
+    return JSON_MODE_CONTENT.format(
+        schema=json.dumps(tool_type.model_json_schema(), indent=2)
+    )
+
 
 class OpenAICall(BaseCall[OpenAICallResponse, OpenAICallResponseChunk, OpenAITool]):
     """A base class for calling OpenAI's Chat Completion models.
 
     Example:
 
     ```python
@@ -64,30 +79,33 @@
         Returns:
             A `OpenAICallResponse` instance.
 
         Raises:
             OpenAIError: raises any OpenAI errors, see:
                 https://platform.openai.com/docs/guides/error-codes/api-errors
         """
-        kwargs, tool_types = self._setup(kwargs, OpenAITool)
+        kwargs, tool_types = self._setup_openai_kwargs(kwargs)
         client = OpenAI(api_key=self.api_key, base_url=self.base_url)
         if self.call_params.wrapper is not None:
             client = self.call_params.wrapper(client)
+        messages = self._update_messages_if_json(self.messages(), tool_types)
         start_time = datetime.datetime.now().timestamp() * 1000
         completion = client.chat.completions.create(
-            messages=self.messages(),
+            messages=messages,
             stream=False,
             **kwargs,
         )
-        return OpenAICallResponse(
+        openai_call_response = OpenAICallResponse(
             response=completion,
             tool_types=tool_types,
             start_time=start_time,
             end_time=datetime.datetime.now().timestamp() * 1000,
         )
+        openai_call_response.response_format = self.call_params.response_format
+        return openai_call_response
 
     async def call_async(self, **kwargs: Any) -> OpenAICallResponse:
         """Makes an asynchronous call to the model using this `OpenAICall`.
 
         Args:
             **kwargs: Additional keyword arguments parameters to pass to the call. These
                 will override any existing arguments in `call_params`.
@@ -99,26 +117,29 @@
             OpenAIError: raises any OpenAI errors, see:
                 https://platform.openai.com/docs/guides/error-codes/api-errors
         """
         kwargs, tool_types = self._setup(kwargs, OpenAITool)
         client = AsyncOpenAI(api_key=self.api_key, base_url=self.base_url)
         if self.call_params.wrapper_async is not None:
             client = self.call_params.wrapper_async(client)
+        messages = self._update_messages_if_json(self.messages(), tool_types)
         start_time = datetime.datetime.now().timestamp() * 1000
         completion = await client.chat.completions.create(
-            messages=self.messages(),
+            messages=messages,
             stream=False,
             **kwargs,
         )
-        return OpenAICallResponse(
+        openai_call_response = OpenAICallResponse(
             response=completion,
             tool_types=tool_types,
             start_time=start_time,
             end_time=datetime.datetime.now().timestamp() * 1000,
         )
+        openai_call_response.response_format = self.call_params.response_format
+        return openai_call_response
 
     def stream(self, **kwargs: Any) -> Generator[OpenAICallResponseChunk, None, None]:
         """Streams the response for a call using this `OpenAICall`.
 
         Args:
             **kwargs: Additional keyword arguments parameters to pass to the call. These
                 will override any existing arguments in `call_params`.
@@ -130,21 +151,28 @@
             OpenAIError: raises any OpenAI errors, see:
                 https://platform.openai.com/docs/guides/error-codes/api-errors
         """
         kwargs, tool_types = self._setup(kwargs, OpenAITool)
         client = OpenAI(api_key=self.api_key, base_url=self.base_url)
         if self.call_params.wrapper is not None:
             client = self.call_params.wrapper(client)
+        messages = self._update_messages_if_json(self.messages(), tool_types)
         stream = client.chat.completions.create(
-            messages=self.messages(),
+            messages=messages,
             stream=True,
             **kwargs,
         )
         for chunk in stream:
-            yield OpenAICallResponseChunk(chunk=chunk, tool_types=tool_types)
+            openai_call_response_chunk = OpenAICallResponseChunk(
+                chunk=chunk, tool_types=tool_types
+            )
+            openai_call_response_chunk.response_format = (
+                self.call_params.response_format
+            )
+            yield openai_call_response_chunk
 
     async def stream_async(
         self, **kwargs: Any
     ) -> AsyncGenerator[OpenAICallResponseChunk, None]:
         """Streams the response for an asynchronous call using this `OpenAICall`.
 
         Args:
@@ -158,14 +186,55 @@
             OpenAIError: raises any OpenAI errors, see:
                 https://platform.openai.com/docs/guides/error-codes/api-errors
         """
         kwargs, tool_types = self._setup(kwargs, OpenAITool)
         client = AsyncOpenAI(api_key=self.api_key, base_url=self.base_url)
         if self.call_params.wrapper_async is not None:
             client = self.call_params.wrapper_async(client)
+        messages = self._update_messages_if_json(self.messages(), tool_types)
         stream = await client.chat.completions.create(
-            messages=self.messages(),
+            messages=messages,
             stream=True,
             **kwargs,
         )
         async for chunk in stream:
-            yield OpenAICallResponseChunk(chunk=chunk, tool_types=tool_types)
+            openai_call_response_chunk = OpenAICallResponseChunk(
+                chunk=chunk, tool_types=tool_types
+            )
+            openai_call_response_chunk.response_format = (
+                self.call_params.response_format
+            )
+            yield openai_call_response_chunk
+
+    ############################## PRIVATE METHODS ###################################
+
+    def _setup_openai_kwargs(
+        self,
+        kwargs: dict[str, Any],
+    ) -> tuple[
+        dict[str, Any],
+        Optional[list[Type[OpenAITool]]],
+    ]:
+        """Overrides the `BaseCall._setup` for Anthropic specific setup."""
+        kwargs, tool_types = self._setup(kwargs, OpenAITool)
+        if (
+            self.call_params.response_format == ResponseFormat(type="json_object")
+            and tool_types
+        ):
+            kwargs.pop("tools")
+        return kwargs, tool_types
+
+    def _update_messages_if_json(
+        self,
+        messages: list[ChatCompletionMessageParam],
+        tool_types: Optional[list[type[OpenAITool]]],
+    ) -> list[ChatCompletionMessageParam]:
+        if (
+            self.call_params.response_format == ResponseFormat(type="json_object")
+            and tool_types
+        ):
+            messages.append(
+                ChatCompletionUserMessageParam(
+                    role="user", content=_json_mode_content(tool_type=tool_types[0])
+                )
+            )
+        return messages
```

### Comparing `mirascope-0.8.2/mirascope/openai/extractors.py` & `mirascope-0.8.3/mirascope/openai/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/openai/tools.py` & `mirascope-0.8.3/mirascope/openai/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/openai/types.py` & `mirascope-0.8.3/mirascope/openai/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     ChatCompletionMessageToolCall,
     ChatCompletionToolChoiceOptionParam,
 )
 from openai.types.chat.chat_completion import Choice
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 from openai.types.chat.chat_completion_chunk import ChoiceDelta, ChoiceDeltaToolCall
 from openai.types.chat.chat_completion_message import ChatCompletionMessage
+from openai.types.chat.chat_completion_message_tool_call import Function
 from openai.types.chat.completion_create_params import ResponseFormat
 from pydantic import ConfigDict
 
 from ..base import BaseCallParams, BaseCallResponse, BaseCallResponseChunk
 from .tools import OpenAITool
 
 
@@ -95,14 +96,16 @@
     print(response.choices)
     #> [Choice(finish_reason='stop', index=0, logprobs=None,
     #  message=ChatCompletionMessage(content='The Name of the Wind', role='assistant',
     #  function_call=None, tool_calls=None))]
     ```
     """
 
+    response_format: Optional[ResponseFormat] = None
+
     @property
     def choices(self) -> list[Choice]:
         """Returns the array of chat completion choices."""
         return self.response.choices
 
     @property
     def choice(self) -> Choice:
@@ -127,17 +130,45 @@
     @property
     def tools(self) -> Optional[list[OpenAITool]]:
         """Returns the tools for the 0th choice message.
 
         Raises:
             ValidationError: if a tool call doesn't match the tool's schema.
         """
-        if not self.tool_types or not self.tool_calls:
+        if not self.tool_types:
             return None
 
+        if self.response_format != ResponseFormat(type="json_object"):
+            if not self.tool_calls:
+                return None
+
+            if self.choices[0].finish_reason not in ["tool_calls", "function_call"]:
+                raise RuntimeError(
+                    "Finish reason was not `tool_calls` or `function_call`, indicating "
+                    "no or failed tool use. This is likely due to a limit on output "
+                    "tokens that is too low. Note that this could also indicate no "
+                    "tool is beind called, so we recommend that you check the output "
+                    "of the call to confirm. "
+                    f"Finish Reason: {self.choices[0].finish_reason}"
+                )
+        else:
+            # Note: we only handle single tool calls in JSON mode.
+            tool_type = self.tool_types[0]
+            return [
+                tool_type.from_tool_call(
+                    ChatCompletionMessageToolCall(
+                        id="id",
+                        function=Function(
+                            name=tool_type.__name__, arguments=self.content
+                        ),
+                        type="function",
+                    )
+                )
+            ]
+
         extracted_tools = []
         for tool_call in self.tool_calls:
             for tool_type in self.tool_types:
                 if tool_call.function.name == tool_type.__name__:
                     extracted_tools.append(tool_type.from_tool_call(tool_call))
                     break
 
@@ -146,22 +177,17 @@
     @property
     def tool(self) -> Optional[OpenAITool]:
         """Returns the 0th tool for the 0th choice message.
 
         Raises:
             ValidationError: if the tool call doesn't match the tool's schema.
         """
-        if not self.tool_types or not self.tool_calls or len(self.tool_calls) == 0:
-            return None
-
-        tool_call = self.tool_calls[0]
-        for tool_type in self.tool_types:
-            if self.tool_calls[0].function.name == tool_type.__name__:
-                return tool_type.from_tool_call(tool_call)
-
+        tools = self.tools
+        if tools:
+            return tools[0]
         return None
 
     def dump(self) -> dict[str, Any]:
         """Dumps the response to a dictionary."""
         return {
             "start_time": self.start_time,
             "end_time": self.end_time,
@@ -195,14 +221,16 @@
     #  2
     #   equals
     #
     #  3
     #  .
     """
 
+    response_format: Optional[ResponseFormat] = None
+
     @property
     def choices(self) -> list[ChunkChoice]:
         """Returns the array of chat completion choices."""
         return self.chunk.choices
 
     @property
     def choice(self) -> ChunkChoice:
```

### Comparing `mirascope-0.8.2/mirascope/wandb/wandb.py` & `mirascope-0.8.3/mirascope/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/mirascope/wandb/weave.py` & `mirascope-0.8.3/mirascope/wandb/weave.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.2/pyproject.toml` & `mirascope-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mirascope"
-version = "0.8.2"
+version = "0.8.3"
 description = "LLM toolkit for lightning-fast, high-quality development"
 license = "MIT"
 authors = [
     "William Bakst <william@mirascope.io>",
     "Brendan Kao <brendan@mirascope.io>",
 ]
 readme = "docs/README.md"
```

### Comparing `mirascope-0.8.2/PKG-INFO` & `mirascope-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirascope
-Version: 0.8.2
+Version: 0.8.3
 Summary: LLM toolkit for lightning-fast, high-quality development
 Home-page: https://github.com/Mirascope/mirascope
 License: MIT
 Author: William Bakst
 Author-email: william@mirascope.io
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

