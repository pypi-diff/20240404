# Comparing `tmp/llmsmith-0.1.1.tar.gz` & `tmp/llmsmith-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmsmith-0.1.1.tar", max compression
+gzip compressed data, was "llmsmith-0.1.2.tar", max compression
```

## Comparing `llmsmith-0.1.1.tar` & `llmsmith-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.1.1/LICENSE
--rw-r--r--   0        0        0     1120 2024-04-03 04:13:09.876728 llmsmith-0.1.1/README.md
--rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.1.1/llmsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.1.1/llmsmith/job/__init__.py
--rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.1.1/llmsmith/job/base.py
--rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.1.1/llmsmith/job/job.py
--rw-r--r--   0        0        0        0 2024-03-13 07:08:41.469795 llmsmith-0.1.1/llmsmith/llm/__init__.py
--rw-r--r--   0        0        0      840 2024-03-14 08:08:05.921578 llmsmith-0.1.1/llmsmith/llm/base.py
--rw-r--r--   0        0        0     4002 2024-03-15 12:55:51.329681 llmsmith-0.1.1/llmsmith/llm/claude.py
--rw-r--r--   0        0        0     4658 2024-03-15 12:55:51.328266 llmsmith-0.1.1/llmsmith/llm/gemini.py
--rw-r--r--   0        0        0      765 2024-03-15 12:55:51.327162 llmsmith-0.1.1/llmsmith/llm/models.py
--rw-r--r--   0        0        0     3544 2024-03-15 12:55:51.346083 llmsmith-0.1.1/llmsmith/llm/openai.py
--rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.1.1/llmsmith/task/__init__.py
--rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.1.1/llmsmith/task/base.py
--rw-r--r--   0        0        0      229 2024-03-19 10:00:36.806582 llmsmith-0.1.1/llmsmith/task/models.py
--rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.1.1/llmsmith/task/retrieval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.1.1/llmsmith/task/retrieval/vector/__init__.py
--rw-r--r--   0        0        0     3125 2024-04-03 08:48:20.812756 llmsmith-0.1.1/llmsmith/task/retrieval/vector/chromadb.py
--rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.1.1/llmsmith/task/textgen/__init__.py
--rw-r--r--   0        0        0     3017 2024-04-02 09:50:51.208365 llmsmith-0.1.1/llmsmith/task/textgen/claude.py
--rw-r--r--   0        0        0     3008 2024-04-02 09:53:27.121715 llmsmith-0.1.1/llmsmith/task/textgen/gemini.py
--rw-r--r--   0        0        0     3181 2024-04-02 09:53:36.726181 llmsmith-0.1.1/llmsmith/task/textgen/openai.py
--rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.1.1/llmsmith/task/textgen/options/__init__.py
--rw-r--r--   0        0        0     1288 2024-04-03 08:45:01.210357 llmsmith-0.1.1/llmsmith/task/textgen/options/claude.py
--rw-r--r--   0        0        0     1462 2024-04-03 08:45:17.264854 llmsmith-0.1.1/llmsmith/task/textgen/options/gemini.py
--rw-r--r--   0        0        0     2104 2024-04-03 08:45:28.383781 llmsmith-0.1.1/llmsmith/task/textgen/options/openai.py
--rw-r--r--   0        0        0     1022 2024-04-03 10:41:13.550755 llmsmith-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 llmsmith-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1122 2024-04-03 10:55:28.746484 llmsmith-0.1.2/README.md
+-rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.1.2/llmsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.1.2/llmsmith/job/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.1.2/llmsmith/job/base.py
+-rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.1.2/llmsmith/job/job.py
+-rw-r--r--   0        0        0        0 2024-03-13 07:08:41.469795 llmsmith-0.1.2/llmsmith/llm/__init__.py
+-rw-r--r--   0        0        0      840 2024-03-14 08:08:05.921578 llmsmith-0.1.2/llmsmith/llm/base.py
+-rw-r--r--   0        0        0     4006 2024-04-03 10:52:50.577228 llmsmith-0.1.2/llmsmith/llm/claude.py
+-rw-r--r--   0        0        0     4662 2024-04-03 10:53:07.060380 llmsmith-0.1.2/llmsmith/llm/gemini.py
+-rw-r--r--   0        0        0      765 2024-03-15 12:55:51.327162 llmsmith-0.1.2/llmsmith/llm/models.py
+-rw-r--r--   0        0        0     3548 2024-04-03 10:53:30.824465 llmsmith-0.1.2/llmsmith/llm/openai.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.1.2/llmsmith/task/__init__.py
+-rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.1.2/llmsmith/task/base.py
+-rw-r--r--   0        0        0      229 2024-03-19 10:00:36.806582 llmsmith-0.1.2/llmsmith/task/models.py
+-rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.1.2/llmsmith/task/retrieval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.1.2/llmsmith/task/retrieval/vector/__init__.py
+-rw-r--r--   0        0        0     3129 2024-04-03 10:53:39.882995 llmsmith-0.1.2/llmsmith/task/retrieval/vector/chromadb.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.1.2/llmsmith/task/textgen/__init__.py
+-rw-r--r--   0        0        0     3042 2024-04-04 09:07:05.709627 llmsmith-0.1.2/llmsmith/task/textgen/claude.py
+-rw-r--r--   0        0        0      649 2024-04-04 09:30:06.752488 llmsmith-0.1.2/llmsmith/task/textgen/errors.py
+-rw-r--r--   0        0        0     4455 2024-04-04 09:30:06.752620 llmsmith-0.1.2/llmsmith/task/textgen/gemini.py
+-rw-r--r--   0        0        0     3185 2024-04-03 10:54:14.137132 llmsmith-0.1.2/llmsmith/task/textgen/openai.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.1.2/llmsmith/task/textgen/options/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-04 09:30:06.753059 llmsmith-0.1.2/llmsmith/task/textgen/options/claude.py
+-rw-r--r--   0        0        0     1466 2024-04-03 10:54:40.771025 llmsmith-0.1.2/llmsmith/task/textgen/options/gemini.py
+-rw-r--r--   0        0        0     2108 2024-04-03 10:54:48.638547 llmsmith-0.1.2/llmsmith/task/textgen/options/openai.py
+-rw-r--r--   0        0        0     1306 2024-04-04 09:37:14.232387 llmsmith-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 llmsmith-0.1.2/PKG-INFO
```

### Comparing `llmsmith-0.1.1/LICENSE` & `llmsmith-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.1/README.md` & `llmsmith-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## Installation
 
 LLMSmith does not download extra dependencies (like openai, google-generativeai, chromadb etc.) by default. This is to minimize bloat and keep your application package size in check. The recommended way to install LLMSmith is by specifying the extra dependencies explicitly.
 
 For example, if your project is using an OpenAI LLM and Chroma DB vector database, install LLMSmith using the below command.
 
 ```
-pip install llmsmith[openai,chromadb]
+pip install "llmsmith[openai,chromadb]"
 ```
 
 The above command ensures that only the required dependencies (openai and chromadb clients in this case) are downloaded. The rest are ignored, thus reducing the package size.
 
 Here's the list of extra dependencies supported by LLMSmith:
 - `openai`
 - `claude`
```

### Comparing `llmsmith-0.1.1/llmsmith/job/base.py` & `llmsmith-0.1.2/llmsmith/job/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.1/llmsmith/job/job.py` & `llmsmith-0.1.2/llmsmith/job/job.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.1/llmsmith/llm/base.py` & `llmsmith-0.1.2/llmsmith/llm/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.1/llmsmith/llm/claude.py` & `llmsmith-0.1.2/llmsmith/llm/claude.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 try:
     import anthropic
     from anthropic.types.message import Message
     from anthropic._types import NOT_GIVEN
 except ImportError:
     raise ImportError(
-        "The 'anthropic' library is required to use Claude. You can install it with `pip install llmsmith[claude]`"
+        "The 'anthropic' library is required to use Claude. You can install it with `pip install \"llmsmith[claude]\"`"
     )
 
 
 log = logging.getLogger(__name__)
 
 
 class Claude(ChatLLM):
```

### Comparing `llmsmith-0.1.1/llmsmith/llm/gemini.py` & `llmsmith-0.1.2/llmsmith/llm/gemini.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from llmsmith.llm.base import ChatLLM
 from llmsmith.llm.models import LLMChatInput, LLMChatReply, LLMChatResponseContent
 
 try:
     import google.generativeai as genai
 except ImportError:
     raise ImportError(
-        "The 'google.generativeai' library is required to use Gemini. You can install it with `pip install llmsmith[gemini]`"
+        "The 'google.generativeai' library is required to use Gemini. You can install it with `pip install \"llmsmith[gemini]\"`"
     )
 
 
 log = logging.getLogger(__name__)
 
 
 class Gemini(ChatLLM):
```

### Comparing `llmsmith-0.1.1/llmsmith/llm/models.py` & `llmsmith-0.1.2/llmsmith/llm/models.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.1/llmsmith/llm/openai.py` & `llmsmith-0.1.2/llmsmith/llm/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from llmsmith.llm.models import LLMChatInput, LLMChatReply, LLMChatResponseContent
 
 try:
     import openai
     from openai.types.chat.chat_completion import ChatCompletion
 except ImportError:
     raise ImportError(
-        "The 'openai' library is required to use OpenAI. You can install it with `pip install llmsmith[openai]`"
+        "The 'openai' library is required to use OpenAI. You can install it with `pip install \"llmsmith[openai]\"`"
     )
 
 
 log = logging.getLogger(__name__)
 
 
 class OpenAI(ChatLLM):
```

### Comparing `llmsmith-0.1.1/llmsmith/task/base.py` & `llmsmith-0.1.2/llmsmith/task/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.1.1/llmsmith/task/retrieval/vector/chromadb.py` & `llmsmith-0.1.2/llmsmith/task/retrieval/vector/chromadb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from llmsmith.task.models import TaskInput, TaskOutput
 
 
 try:
     from chromadb import Collection, QueryResult, Where, WhereDocument
 except ImportError:
     raise ImportError(
-        "The 'chromadb-client' library is required to use ChromaDBRetriever. You can install it with `pip install llmsmith[chromadb]`"
+        "The 'chromadb-client' library is required to use ChromaDBRetriever. You can install it with `pip install \"llmsmith[chromadb]\"`"
     )
 
 
 def default_doc_processor(res: QueryResult) -> str:
     """
     Formats the retrieved chromadb documents into below format.
```

### Comparing `llmsmith-0.1.1/llmsmith/task/textgen/claude.py` & `llmsmith-0.1.2/llmsmith/task/textgen/claude.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from typing import List
 
 try:
     import anthropic
     from anthropic.types.message import Message
 except ImportError:
     raise ImportError(
-        "The 'anthropic' library is required to use ClaudeTextGenTask. You can install it with `pip install llmsmith[claude]`"
+        "The 'anthropic' library is required to use ClaudeTextGenTask. You can install it with `pip install \"llmsmith[claude]\"`"
     )
 
 from llmsmith.task.base import Task
 from llmsmith.task.models import TaskInput, TaskOutput
 from llmsmith.task.textgen.options.claude import (
     ClaudeTextGenOptions,
     _completion_create_options_dict,
 )
 
 
 log = logging.getLogger(__name__)
 
 # Default options for text generation using Anthropic's Claude LLMs.
 default_options: ClaudeTextGenOptions = ClaudeTextGenOptions(
-    model="claude-instant-1.2", temperature=0.3
+    model="claude-3-opus-20240229", temperature=0.3, max_tokens=1024
 )
 
 
 class ClaudeTextGenTask(Task[str, str]):
     """
     Task for generating text using Anthropic's Claude Large Language Models (LLMs).
```

### Comparing `llmsmith-0.1.1/llmsmith/task/textgen/gemini.py` & `llmsmith-0.1.2/llmsmith/task/textgen/openai.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,93 @@
 import logging
 from typing import List
 
 try:
-    from google.generativeai import GenerativeModel
-    from google.generativeai.types import GenerateContentResponse
+    import openai
+    from openai.types.chat.chat_completion import ChatCompletion
 except ImportError:
     raise ImportError(
-        "The 'google.generativeai' library is required to use GeminiTextGenTask. You can install it with `pip install llmsmith[gemini]`"
+        "The 'openai' library is required to use OpenAITextGenTask. You can install it with `pip install \"llmsmith[openai]\"`"
     )
 
 from llmsmith.task.base import Task
 from llmsmith.task.models import TaskInput, TaskOutput
-from llmsmith.task.textgen.options.gemini import (
-    GeminiTextGenOptions,
+from llmsmith.task.textgen.options.openai import (
+    OpenAITextGenOptions,
     _completion_create_options_dict,
 )
 
 
 log = logging.getLogger(__name__)
 
-# Default options for text generation using Google's Gemini LLMs.
-default_options: GeminiTextGenOptions = GeminiTextGenOptions()
+# Default options for text generation using OpenAI's LLMs.
+default_options: OpenAITextGenOptions = OpenAITextGenOptions(
+    model="gpt-3.5-turbo", temperature=0.3
+)
 
 
-class GeminiTextGenTask(Task[str, str]):
+class OpenAITextGenTask(Task[str, str]):
     """
-    Task for generating text using Google's Gemini Large Language Models (LLMs).
+    Task for generating text using OpenAI's Large Language Models (LLMs).
 
     :param name: The name of the task.
     :type name: str
-    :param llm: An instance of the Gemini client.
-    :type llm: :class:`google.generativeai.GenerativeModel`
-    :param llm_options: A dictionary of options to pass to the Gemini LLM.
-    :type llm_options: :class:`llmsmith.task.textgen.options.gemini.GeminiTextGenOptions`, optional
+    :param llm: An instance of the Async OpenAI client.
+    :type llm: :class:`openai.AsyncOpenAI`
+    :param llm_options: A dictionary of options to pass to the OpenAI LLM.
+    :type llm_options: :class:`llmsmith.task.textgen.options.openai.OpenAITextGenOptions`, optional
     :raises ValueError: If the name is empty.
     """
 
     def __init__(
         self,
         name: str,
-        llm: GenerativeModel,
-        llm_options: GeminiTextGenOptions = default_options,
+        llm: openai.AsyncOpenAI,
+        llm_options: OpenAITextGenOptions = default_options,
     ) -> None:
         super().__init__(name)
 
-        self.llm: GenerativeModel = llm
-        self.llm_options: GeminiTextGenOptions = llm_options
+        self.llm: openai.AsyncOpenAI = llm
+        self.llm_options: OpenAITextGenOptions = llm_options
 
     async def execute(self, task_input: TaskInput[str]) -> TaskOutput[str]:
         """
-        Generates text using Gemini LLM using the given input.
+        Generates text using OpenAI LLM using the given input.
 
         :param task_input: The input to the task.
         :type task_input: :class:`llmsmith.task.models.TaskInput[str]`
         :raises ValueError: If the content of the task input is not a string.
         :returns: The output of the task.
         :rtype: :class:`llmsmith.task.models.TaskOutput[str]`
         """
         if not isinstance(task_input.content, str):
             log.debug(f"task_input value: {task_input}")
             raise ValueError("task_input.content should be of type 'str'")
 
         llm_input_content: str = task_input.content
 
-        messages_payload: List[dict] = [{"role": "user", "parts": [llm_input_content]}]
+        sys_prompt = (self.llm_options.get("system_prompt") or "").strip()
+        messages_payload: List[dict] = []
+
+        if sys_prompt:
+            messages_payload.append({"role": "system", "content": sys_prompt})
+        messages_payload.append({"role": "user", "content": llm_input_content})
+
         chat_completion_options: dict = _completion_create_options_dict(
             self.llm_options
         )
 
         log.debug(
-            f"Google Gemini chat request: PAYLOAD: {messages_payload}\n OPTIONS: {chat_completion_options}"
+            f"OpenAI chat request: PAYLOAD: {messages_payload}\n OPTIONS: {chat_completion_options}"
         )
 
-        llm_reply: GenerateContentResponse = await self.llm.generate_content_async(
-            contents=messages_payload, **chat_completion_options
+        llm_reply: ChatCompletion = await self.llm.chat.completions.create(
+            messages=messages_payload, **chat_completion_options
         )
 
-        log.debug(f"Google Gemini chat response: {llm_reply}")
+        log.debug(f"OpenAI chat response: {llm_reply}")
 
-        output_content: str = llm_reply.candidates[0].content
+        output_content: str = llm_reply.choices[0].message.content
 
         log.debug(f"task_output value: {output_content}")
 
         return TaskOutput(content=output_content, raw_output=llm_reply)
```

### Comparing `llmsmith-0.1.1/llmsmith/task/textgen/options/claude.py` & `llmsmith-0.1.2/llmsmith/task/textgen/options/claude.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import List, Mapping, TypedDict, Union
 
 try:
     from anthropic.types.message_create_params import Metadata
 except ImportError:
     raise ImportError(
-        "The 'anthropic' library is required to use ClaudeTextGenOptions. You can install it with `pip install llmsmith[claude]`"
+        "The 'anthropic' library is required to use ClaudeTextGenOptions. You can install it with `pip install \"llmsmith[claude]\"`"
     )
 
 
 class ClaudeTextGenOptions(TypedDict):
     """
     A dictionary of options to pass to the Anthropic Claude LLM for text generation.
     The option names are same as the ones used in Anthropic client.
     Refer below links for more info.
-    
+
     * https://github.com/anthropics/anthropic-sdk-python/blob/v0.19.2/src/anthropic/types/message_create_params.py
     * https://docs.anthropic.com/claude/reference/messages_post
     """
 
     model: str
     system: Union[str, None]
     max_tokens: Union[int, None]
@@ -29,8 +29,18 @@
     extra_headers: Mapping[str, Union[str, None]]
     extra_query: Mapping[str, object]
     extra_body: object
     timeout: Union[float, None]
 
 
 def _completion_create_options_dict(options: ClaudeTextGenOptions) -> dict:
-    return {attr: options.get(attr) for attr in ClaudeTextGenOptions.__annotations__}
+    opt = {
+        attr: options.get(attr)
+        for attr in ClaudeTextGenOptions.__annotations__
+        if options.get(attr)
+    }
+    if not opt.get("model"):
+        opt["model"] = "claude-3-opus-20240229"
+    if not opt.get("max_tokens"):
+        opt["max_tokens"] = 1024
+
+    return opt
```

### Comparing `llmsmith-0.1.1/llmsmith/task/textgen/options/gemini.py` & `llmsmith-0.1.2/llmsmith/task/textgen/options/gemini.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 try:
     from google.generativeai.types.generation_types import GenerationConfigType
     from google.generativeai.types.safety_types import SafetySettingOptions
     from google.generativeai.types.content_types import FunctionLibraryType
 except ImportError:
     raise ImportError(
-        "The 'google.generativeai' library is required to use GeminiTextGenOptions. You can install it with `pip install llmsmith[gemini]`"
+        "The 'google.generativeai' library is required to use GeminiTextGenOptions. You can install it with `pip install \"llmsmith[gemini]\"`"
     )
 
 
 class GeminiTextGenOptions(TypedDict):
     """
     A dictionary of options to pass to the Google Gemini LLM for text generation.
     The option names are same as the ones used in Gemini client.
```

### Comparing `llmsmith-0.1.1/llmsmith/task/textgen/options/openai.py` & `llmsmith-0.1.2/llmsmith/task/textgen/options/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     )
     from openai.types.chat.chat_completion_tool_choice_option_param import (
         ChatCompletionToolChoiceOptionParam,
     )
     from openai.types.chat.chat_completion_tool_param import ChatCompletionToolParam
 except ImportError:
     raise ImportError(
-        "The 'openai' library is required to use OpenAITextGenOptions. You can install it with `pip install llmsmith[openai]`"
+        "The 'openai' library is required to use OpenAITextGenOptions. You can install it with `pip install \"llmsmith[openai]\"`"
     )
 
 
 class OpenAITextGenOptions(TypedDict):
     """
     A dictionary of options to pass to the OpenAI LLM for text generation.
     The option names are same as the ones used in OpenAI client (except `system_prompt`, which is an extra).
```

### Comparing `llmsmith-0.1.1/pyproject.toml` & `llmsmith-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [tool.poetry]
 name = "LLMSmith"
-version = "0.1.1"
-description = ""
+version = "0.1.2"
+description = "Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)"
 authors = ["Dheeraj Gopinath <dheeraj.gopinath@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = {version = "^1.13.3", optional = true}
 anthropic = {version = "^0.19.2", optional = true}
 google-generativeai = {version = "^0.4.0", optional = true}
 chromadb-client = {version = "^0.4.25.dev0", optional = true}
 onnxruntime = {version = "^1.17.1", optional = true}
+protobuf = {version = "3.20.3", optional = true}
+tokenizers = {version = "^0.15.2", optional = true}
+python-dotenv = "^1.0.1"
 
 [tool.poetry.extras]
 openai = ["openai"]
 claude = ["anthropic"]
 gemini = ["google-generativeai"]
-chromadb = ["chromadb-client", "onnxruntime"]
-all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime"]
+chromadb = ["chromadb-client", "onnxruntime", "protobuf", "tokenizers"]
+all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.2"
 black = "^24.2.0"
```

### Comparing `llmsmith-0.1.1/PKG-INFO` & `llmsmith-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: LLMSmith
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)
 Author: Dheeraj Gopinath
 Author-email: dheeraj.gopinath@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,14 +16,17 @@
 Provides-Extra: gemini
 Provides-Extra: openai
 Requires-Dist: anthropic (>=0.19.2,<0.20.0) ; extra == "claude" or extra == "all"
 Requires-Dist: chromadb-client (>=0.4.25.dev0,<0.5.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0) ; extra == "gemini" or extra == "all"
 Requires-Dist: onnxruntime (>=1.17.1,<2.0.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: openai (>=1.13.3,<2.0.0) ; extra == "openai" or extra == "all"
+Requires-Dist: protobuf (==3.20.3) ; extra == "chromadb" or extra == "all"
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: tokenizers (>=0.15.2,<0.16.0) ; extra == "chromadb" or extra == "all"
 Description-Content-Type: text/markdown
 
 # 🧰 LLMSmith
 
 ## What is LLMSmith?
 
 **LLMSmith** is a lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs). It allows developers to integrate LLMs into various types of applications, whether they are web applications, GUI applications, or any other kind of application.
@@ -31,15 +34,15 @@
 ## Installation
 
 LLMSmith does not download extra dependencies (like openai, google-generativeai, chromadb etc.) by default. This is to minimize bloat and keep your application package size in check. The recommended way to install LLMSmith is by specifying the extra dependencies explicitly.
 
 For example, if your project is using an OpenAI LLM and Chroma DB vector database, install LLMSmith using the below command.
 
 ```
-pip install llmsmith[openai,chromadb]
+pip install "llmsmith[openai,chromadb]"
 ```
 
 The above command ensures that only the required dependencies (openai and chromadb clients in this case) are downloaded. The rest are ignored, thus reducing the package size.
 
 Here's the list of extra dependencies supported by LLMSmith:
 - `openai`
 - `claude`
```

