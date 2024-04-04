# Comparing `tmp/devon_agent-0.0.2.tar.gz` & `tmp/devon_agent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.0.2.tar", max compression
+gzip compressed data, was "devon_agent-0.0.3.tar", max compression
```

## Comparing `devon_agent-0.0.2.tar` & `devon_agent-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.2/LICENSE
--rw-r--r--   0        0        0     1371 2024-04-04 01:01:24.013453 devon_agent-0.0.2/README.md
--rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.2/devon_agent/__main__.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.2/devon_agent/agent/__init__.py
--rw-r--r--   0        0        0     5372 2024-04-03 18:52:22.966981 devon_agent-0.0.2/devon_agent/agent/clients/client.py
--rw-r--r--   0        0        0     1375 2024-03-29 20:47:19.808870 devon_agent-0.0.2/devon_agent/agent/clients/test_function_client.py
--rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.2/devon_agent/agent/clients/tool_utils/tools.py
--rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.2/devon_agent/agent/evaluate/evaluate.py
--rw-r--r--   0        0        0      855 2024-04-03 17:56:50.209384 devon_agent-0.0.2/devon_agent/agent/kernel/context.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/__init__.py
--rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/state.py
--rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/state_machine.py
--rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/state_types.py
--rw-r--r--   0        0        0     1744 2024-04-03 17:56:50.210066 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/evaluate.py
--rw-r--r--   0        0        0     1986 2024-04-04 01:02:20.668746 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/reason.py
--rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/terminate.py
--rw-r--r--   0        0        0     1784 2024-04-03 19:12:43.542087 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/tool.py
--rw-r--r--   0        0        0     2738 2024-04-03 17:56:50.210677 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/write.py
--rw-r--r--   0        0        0     5697 2024-04-04 01:02:20.669219 devon_agent-0.0.2/devon_agent/agent/kernel/thread.py
--rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.2/devon_agent/agent/reasoning/reason.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.2/devon_agent/agent/tools/__init__.py
--rw-r--r--   0        0        0     6283 2024-04-03 18:52:22.941743 devon_agent-0.0.2/devon_agent/agent/tools/file_system/fs.py
--rw-r--r--   0        0        0     2240 2024-03-29 20:47:19.811690 devon_agent-0.0.2/devon_agent/agent/tools/file_system/test_fs_tool.py
--rw-r--r--   0        0        0     5141 2024-04-03 18:52:22.942343 devon_agent-0.0.2/devon_agent/agent/tools/git_tool/git_tool.py
--rw-r--r--   0        0        0     1989 2024-03-29 20:47:19.812172 devon_agent-0.0.2/devon_agent/agent/tools/git_tool/test_git_tool.py
--rw-r--r--   0        0        0     4333 2024-04-03 19:14:07.614040 devon_agent-0.0.2/devon_agent/agent/tools/github/github_tool.py
--rw-r--r--   0        0        0     2894 2024-03-29 20:47:19.812588 devon_agent-0.0.2/devon_agent/agent/tools/github/test_github_tool.py
--rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.2/devon_agent/agent/tools/tool_prompts.py
--rw-r--r--   0        0        0     6614 2024-04-03 17:56:50.211870 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/create_diff.py
--rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/diff_types.py
--rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
--rw-r--r--   0        0        0     9283 2024-04-04 01:02:20.669812 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
--rw-r--r--   0        0        0     1785 2024-03-29 20:47:19.813973 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
--rw-r--r--   0        0        0     8227 2024-04-03 18:52:22.943827 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/utils.py
--rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.2/devon_agent/format.py
--rw-r--r--   0        0        0     1077 2024-04-03 18:52:20.747624 devon_agent-0.0.2/devon_agent/main.py
--rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.2/devon_agent/react.py
--rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.2/devon_agent/run.txt
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.2/devon_agent/sandbox/__init__.py
--rw-r--r--   0        0        0     1589 2024-03-29 20:47:19.814941 devon_agent-0.0.2/devon_agent/sandbox/environments.py
--rw-r--r--   0        0        0      928 2024-03-29 20:47:19.815099 devon_agent-0.0.2/devon_agent/sandbox/tool_proxy.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.2/devon_agent/tests/__init__.py
--rw-r--r--   0        0        0     6177 2024-03-29 20:47:19.815436 devon_agent-0.0.2/devon_agent/tests/state_functions.py
--rw-r--r--   0        0        0     1876 2024-03-29 20:47:19.815606 devon_agent-0.0.2/devon_agent/tests/test_diff.py
--rw-r--r--   0        0        0      665 2024-04-04 01:51:49.611979 devon_agent-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 devon_agent-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1371 2024-04-04 01:01:24.013453 devon_agent-0.0.3/README.md
+-rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.3/devon_agent/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.3/devon_agent/agent/__init__.py
+-rw-r--r--   0        0        0     5378 2024-04-04 01:56:29.973522 devon_agent-0.0.3/devon_agent/agent/clients/client.py
+-rw-r--r--   0        0        0     1387 2024-04-04 01:56:29.975197 devon_agent-0.0.3/devon_agent/agent/clients/test_function_client.py
+-rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.3/devon_agent/agent/clients/tool_utils/tools.py
+-rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.3/devon_agent/agent/evaluate/evaluate.py
+-rw-r--r--   0        0        0      873 2024-04-04 01:56:29.933293 devon_agent-0.0.3/devon_agent/agent/kernel/context.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/state.py
+-rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/state_machine.py
+-rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/state_types.py
+-rw-r--r--   0        0        0     1768 2024-04-04 01:56:29.933283 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/evaluate.py
+-rw-r--r--   0        0        0     1998 2024-04-04 01:56:29.932370 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/reason.py
+-rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/terminate.py
+-rw-r--r--   0        0        0     1808 2024-04-04 01:56:29.932353 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/tool.py
+-rw-r--r--   0        0        0     2768 2024-04-04 01:56:29.932381 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/write.py
+-rw-r--r--   0        0        0     5805 2024-04-04 01:56:29.932954 devon_agent-0.0.3/devon_agent/agent/kernel/thread.py
+-rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.3/devon_agent/agent/reasoning/reason.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.3/devon_agent/agent/tools/__init__.py
+-rw-r--r--   0        0        0     6289 2024-04-04 01:56:29.969363 devon_agent-0.0.3/devon_agent/agent/tools/file_system/fs.py
+-rw-r--r--   0        0        0     2276 2024-04-04 01:56:29.938196 devon_agent-0.0.3/devon_agent/agent/tools/file_system/test_fs_tool.py
+-rw-r--r--   0        0        0     5147 2024-04-04 01:56:29.969375 devon_agent-0.0.3/devon_agent/agent/tools/git_tool/git_tool.py
+-rw-r--r--   0        0        0     2013 2024-04-04 01:56:29.969323 devon_agent-0.0.3/devon_agent/agent/tools/git_tool/test_git_tool.py
+-rw-r--r--   0        0        0     4339 2024-04-04 01:56:29.933945 devon_agent-0.0.3/devon_agent/agent/tools/github/github_tool.py
+-rw-r--r--   0        0        0     2930 2024-04-04 01:56:29.934004 devon_agent-0.0.3/devon_agent/agent/tools/github/test_github_tool.py
+-rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.3/devon_agent/agent/tools/tool_prompts.py
+-rw-r--r--   0        0        0     6632 2024-04-04 01:56:29.972647 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/create_diff.py
+-rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/diff_types.py
+-rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
+-rw-r--r--   0        0        0     9283 2024-04-04 01:02:20.669812 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
+-rw-r--r--   0        0        0     1791 2024-04-04 01:56:29.969391 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
+-rw-r--r--   0        0        0     8275 2024-04-04 01:56:29.971937 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/utils.py
+-rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.3/devon_agent/format.py
+-rw-r--r--   0        0        0     1089 2024-04-04 01:56:29.923857 devon_agent-0.0.3/devon_agent/main.py
+-rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.3/devon_agent/react.py
+-rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.3/devon_agent/run.txt
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.3/devon_agent/sandbox/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-04 01:56:29.975187 devon_agent-0.0.3/devon_agent/sandbox/environments.py
+-rw-r--r--   0        0        0      952 2024-04-04 01:56:29.975161 devon_agent-0.0.3/devon_agent/sandbox/tool_proxy.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.3/devon_agent/tests/__init__.py
+-rw-r--r--   0        0        0     6189 2024-04-04 01:56:29.985125 devon_agent-0.0.3/devon_agent/tests/state_functions.py
+-rw-r--r--   0        0        0     1900 2024-04-04 01:56:29.975172 devon_agent-0.0.3/devon_agent/tests/test_diff.py
+-rw-r--r--   0        0        0      726 2024-04-04 01:56:45.966620 devon_agent-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 devon_agent-0.0.3/PKG-INFO
```

### Comparing `devon_agent-0.0.2/LICENSE` & `devon_agent-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/README.md` & `devon_agent-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/agent/clients/client.py` & `devon_agent-0.0.3/devon_agent/agent/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 import os
 from typing import Dict, List, Optional, Any, Union
 
 from anthropic import Anthropic
 from openai import OpenAI
 
-from devon.agent.clients.tool_utils.tools import Toolbox
+from devon_agent.agent.clients.tool_utils.tools import Toolbox
 
 import logging
 
 # Create a logger
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)  # Set the log level
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/clients/test_function_client.py` & `devon_agent-0.0.3/devon_agent/agent/clients/test_function_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from devon.agent.clients.client import GPT4, Message
-from devon.agent.clients.tool_utils.tools import Tool, Toolbox
+from devon_agent.agent.clients.client import GPT4, Message
+from devon_agent.agent.clients.tool_utils.tools import Tool, Toolbox
 
 from pydantic import Field
 from openai import OpenAI
 import json
 
 def get_n_day_weather_forecast(
     location: str = Field(..., description="The city and state, e.g. San Francisco, CA"),
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/clients/tool_utils/tools.py` & `devon_agent-0.0.3/devon_agent/agent/clients/tool_utils/tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/agent/evaluate/evaluate.py` & `devon_agent-0.0.3/devon_agent/agent/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/agent/kernel/context.py` & `devon_agent-0.0.3/devon_agent/agent/kernel/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
-from devon.agent.tools.file_system.fs import FileSystemTool
-from devon.agent.tools.git_tool.git_tool import GitTool
-from devon.agent.tools.github.github_tool import GitHubTool
+from devon_agent.agent.tools.file_system.fs import FileSystemTool
+from devon_agent.agent.tools.git_tool.git_tool import GitTool
+from devon_agent.agent.tools.github.github_tool import GitHubTool
 
 @dataclass
 class FileContext:
     file_glob: dict
     file_tree: dict
     file_code_mapping: dict
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/state_machine.py` & `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/state_machine.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/evaluate.py` & `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/evaluate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any
 import json
 
-from devon.agent.clients.client import LanguageModel, Message
-from devon.agent.evaluate.evaluate import EvaluatePrompts
+from devon_agent.agent.clients.client import LanguageModel, Message
+from devon_agent.agent.evaluate.evaluate import EvaluatePrompts
 from agent.kernel.state_machine.state import State
 from agent.kernel.context import BaseStateContext
 
 from dataclasses import dataclass
-from devon.agent.kernel.context import BaseStateContext
-from devon.agent.kernel.state_machine.states.reason import ReasoningResult
+from devon_agent.agent.kernel.context import BaseStateContext
+from devon_agent.agent.kernel.state_machine.states.reason import ReasoningResult
 
 @dataclass
 class EvaluateParameters:
     model: LanguageModel
 
 @dataclass
 class EvaluateContext:
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/reason.py` & `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/reason.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 import json
-from devon.agent.clients.client import LanguageModel, Message
-from devon.agent.kernel.context import BaseStateContext
+from devon_agent.agent.clients.client import LanguageModel, Message
+from devon_agent.agent.kernel.context import BaseStateContext
 from ..state import State
 from agent.reasoning.reason import ReasoningPrompts
 
 # 1. Reasoning
     # Identify which files are necessary for the change
     # Create a mapping on a file level of what changes need to be made to each file
     # Review plan
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/tool.py` & `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 import json
-from devon.agent.clients.client import LanguageModel, Message
-from devon.agent.clients.tool_utils.tools import Toolbox
-from devon.agent.kernel.context import BaseStateContext
+from devon_agent.agent.clients.client import LanguageModel, Message
+from devon_agent.agent.clients.tool_utils.tools import Toolbox
+from devon_agent.agent.kernel.context import BaseStateContext
 from ..state import State
-from devon.agent.tools.tool_prompts import ToolPrompts
+from devon_agent.agent.tools.tool_prompts import ToolPrompts
 
 
 # 1. Tool
 # Identify which files are necessary for the change
 # Create a mapping on a file level of what changes need to be made to each file
 # Review plan
 @dataclass
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/write.py` & `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from dataclasses import dataclass
 import json
 import os
 import traceback
-from devon.agent.clients.client import LanguageModel
-from devon.agent.kernel.context import BaseStateContext
-from devon.agent.kernel.state_machine.states.reason import ReasoningResult
+from devon_agent.agent.clients.client import LanguageModel
+from devon_agent.agent.kernel.context import BaseStateContext
+from devon_agent.agent.kernel.state_machine.states.reason import ReasoningResult
 
-from devon.agent.tools.unified_diff.create_diff import generate_unified_diff2
-from devon.agent.tools.unified_diff.utils import apply_diff2
+from devon_agent.agent.tools.unified_diff.create_diff import generate_unified_diff2
+from devon_agent.agent.tools.unified_diff.utils import apply_diff2
 from ..state import State
 from agent.tools.file_system.fs import FileSystemTool
 
 @dataclass
 class WriteParameters:
     diff_model: LanguageModel
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/kernel/thread.py` & `devon_agent-0.0.3/devon_agent/agent/kernel/thread.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 from pathlib import Path
 from typing import Literal
 
 from openai import OpenAI
 
-from devon.agent.evaluate.evaluate import EvaluatePrompts
-from devon.agent.kernel.context import BaseStateContext
-from devon.agent.kernel.state_machine.states.evaluate import EvaluateContext, EvaluateParameters, EvaluateState
-from devon.agent.kernel.state_machine.states.reason import ReasonState, ReasoningContext, ReasoningParameters
-from devon.agent.kernel.state_machine.states.terminate import TerminateState
-from devon.agent.kernel.state_machine.states.tool import ToolContext, ToolParameters, ToolState
-from devon.agent.kernel.state_machine.states.write import WriteContext, WriteParameters, WriteState
-from devon.agent.tools.git_tool.git_tool import GitTool
-from devon.agent.tools.github.github_tool import GitHubTool
-from devon.agent.tools.file_system.fs import FileSystemTool
-from devon.agent.tools.tool_prompts import ToolPrompts
-from devon.agent.tools.unified_diff.create_diff import generate_unified_diff2
-from devon.agent.tools.unified_diff.prompts.udiff_prompts import UnifiedDiffPrompts
-from devon.agent.tools.unified_diff.utils import apply_diff2
-from devon.sandbox.environments import EnvironmentProtocol
-from devon.format import reformat_code
-from devon.agent.reasoning.reason import ReasoningPrompts
+from devon_agent.agent.evaluate.evaluate import EvaluatePrompts
+from devon_agent.agent.kernel.context import BaseStateContext
+from devon_agent.agent.kernel.state_machine.states.evaluate import EvaluateContext, EvaluateParameters, EvaluateState
+from devon_agent.agent.kernel.state_machine.states.reason import ReasonState, ReasoningContext, ReasoningParameters
+from devon_agent.agent.kernel.state_machine.states.terminate import TerminateState
+from devon_agent.agent.kernel.state_machine.states.tool import ToolContext, ToolParameters, ToolState
+from devon_agent.agent.kernel.state_machine.states.write import WriteContext, WriteParameters, WriteState
+from devon_agent.agent.tools.git_tool.git_tool import GitTool
+from devon_agent.agent.tools.github.github_tool import GitHubTool
+from devon_agent.agent.tools.file_system.fs import FileSystemTool
+from devon_agent.agent.tools.tool_prompts import ToolPrompts
+from devon_agent.agent.tools.unified_diff.create_diff import generate_unified_diff2
+from devon_agent.agent.tools.unified_diff.prompts.udiff_prompts import UnifiedDiffPrompts
+from devon_agent.agent.tools.unified_diff.utils import apply_diff2
+from devon_agent.sandbox.environments import EnvironmentProtocol
+from devon_agent.format import reformat_code
+from devon_agent.agent.reasoning.reason import ReasoningPrompts
 from agent.evaluate.evaluate import EvaluatePrompts
 from anthropic import Anthropic
-from devon.agent.clients.client import GPT4, ClaudeHaiku, ClaudeOpus, ClaudeSonnet, Message
+from devon_agent.agent.clients.client import GPT4, ClaudeHaiku, ClaudeOpus, ClaudeSonnet, Message
 import json
 import traceback
 import xmltodict
 from .state_machine.state_machine import StateMachine
 from .state_machine.state_types import StateType
 
 class Thread:
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/reasoning/reason.py` & `devon_agent-0.0.3/devon_agent/agent/reasoning/reason.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/file_system/fs.py` & `devon_agent-0.0.3/devon_agent/agent/tools/file_system/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 from pydantic import BaseModel, Field
 from typing import List, Dict, Any, Optional
 
-from devon.agent.clients.tool_utils.tools import tool
+from devon_agent.agent.clients.tool_utils.tools import tool
 
 class CodeFile(BaseModel):
     filepath: str
     code: str
     code_with_lines: str
     raw: Optional[str] = None
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/file_system/test_fs_tool.py` & `devon_agent-0.0.3/devon_agent/agent/tools/file_system/test_fs_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from devon.agent.clients.client import GPT4, Message
-from devon.agent.clients.tool_utils.tools import Tool, Toolbox
+from devon_agent.agent.clients.client import GPT4, Message
+from devon_agent.agent.clients.tool_utils.tools import Tool, Toolbox
 
 from pydantic import Field
 from openai import OpenAI
 import json
 import os
 
-from devon.agent.tools.file_system.fs import FileSystemTool
-from devon.agent.tools.git_tool.git_tool import GitManager
-from devon.agent.tools.github.github_tool import GitHubTool
-from devon.agent.tools.directory.directory import DirectoryObserverTool
+from devon_agent.agent.tools.file_system.fs import FileSystemTool
+from devon_agent.agent.tools.git_tool.git_tool import GitManager
+from devon_agent.agent.tools.github.github_tool import GitHubTool
+from devon_agent.agent.tools.directory.directory import DirectoryObserverTool
 
 if __name__ == "__main__":
     tool_bank = Toolbox()
     g = GitManager()
     token = os.getenv("AGENT_GITHUB_TOKEN")
     gh = GitHubTool(token=token)
     directory_tool = DirectoryObserverTool(base_path=".")
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/git_tool/git_tool.py` & `devon_agent-0.0.3/devon_agent/agent/tools/git_tool/git_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import getcwd, path
 from git import Repo
 from typing import List
 from pydantic import Field
-from devon.agent.clients.tool_utils.tools import tool
+from devon_agent.agent.clients.tool_utils.tools import tool
 
 class GitTool:
 
     @tool(name="git_create_repo", description="Clone a Git repository")
     def init_new_repo(self, path: str = Field(..., description="The path to the Git repository")):
         self.repo = Repo.init(path)
         return {"result": f"Git repo at {path}"}
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/git_tool/test_git_tool.py` & `devon_agent-0.0.3/devon_agent/agent/tools/git_tool/test_git_tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from devon.agent.clients.client import GPT4, Message
-from devon.agent.clients.tool_utils.tools import Tool, Toolbox
+from devon_agent.agent.clients.client import GPT4, Message
+from devon_agent.agent.clients.tool_utils.tools import Tool, Toolbox
 
 from pydantic import Field
 from openai import OpenAI
 import json
 
-from devon.agent.tools.file_system.fs import FileSystemTool
-from devon.agent.tools.git_tool.git_tool import GitTool
+from devon_agent.agent.tools.file_system.fs import FileSystemTool
+from devon_agent.agent.tools.git_tool.git_tool import GitTool
 
 def get_n_day_weather_forecast(
     location: str = Field(..., description="The city and state, e.g. San Francisco, CA"),
     format: str = Field("celsius", description="The temperature unit to use. Infer this from the user's location."),
     num_days: int = Field(..., description="The number of days to forecast")
 ) -> str:
     """Get an N-day weather forecast"""
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/github/github_tool.py` & `devon_agent-0.0.3/devon_agent/agent/tools/github/github_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 
 from pydantic import BaseModel, Field
 from typing import List
 
-from devon.agent.clients.tool_utils.tools import tool
+from devon_agent.agent.clients.tool_utils.tools import tool
 
 class GitHubTool(BaseModel):
     token: str = Field(..., description="The GitHub access token")
 
     @tool(
         name="github_search_repositories",
         description="Search for repositories",
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/github/test_github_tool.py` & `devon_agent-0.0.3/devon_agent/agent/tools/github/test_github_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from devon.agent.clients.client import GPT4, Message
-from devon.agent.clients.tool_utils.tools import Tool, Toolbox
+from devon_agent.agent.clients.client import GPT4, Message
+from devon_agent.agent.clients.tool_utils.tools import Tool, Toolbox
 
 from pydantic import Field
 from openai import OpenAI
 import json
 import os
 
-from devon.agent.tools.file_system.fs import FileSystemTool
-from devon.agent.tools.git_tool.git_tool import GitManager
-from devon.agent.tools.github.github_tool import GitHubTool
-from devon.agent.tools.directory.directory import DirectoryObserverTool
+from devon_agent.agent.tools.file_system.fs import FileSystemTool
+from devon_agent.agent.tools.git_tool.git_tool import GitManager
+from devon_agent.agent.tools.github.github_tool import GitHubTool
+from devon_agent.agent.tools.directory.directory import DirectoryObserverTool
 
 def get_n_day_weather_forecast(
     location: str = Field(..., description="The city and state, e.g. San Francisco, CA"),
     format: str = Field("celsius", description="The temperature unit to use. Infer this from the user's location."),
     num_days: int = Field(..., description="The number of days to forecast")
 ) -> str:
     """Get an N-day weather forecast"""
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/tool_prompts.py` & `devon_agent-0.0.3/devon_agent/agent/tools/tool_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/create_diff.py` & `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/create_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import difflib
 import os
-from devon.agent.clients.client import ClaudeOpus, Message
-from devon.agent.tools.unified_diff.diff_types import FileDiff, FileDiff2, Hunk, Hunk2, HunkLine, MultiFileDiff, MultiFileDiff2
+from devon_agent.agent.clients.client import ClaudeOpus, Message
+from devon_agent.agent.tools.unified_diff.diff_types import FileDiff, FileDiff2, Hunk, Hunk2, HunkLine, MultiFileDiff, MultiFileDiff2
 import dotenv
 import re
 
-from devon.agent.tools.unified_diff.prompts.udiff_prompts import UnifiedDiffPrompts
+from devon_agent.agent.tools.unified_diff.prompts.udiff_prompts import UnifiedDiffPrompts
 
 dotenv.load_dotenv()
 
 # def parse_multi_file_diff(diff: str) -> MultiFileDiff:
 #     file_diffs = []
 #     lines = diff.strip().split("\n")
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/diff_types.py` & `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/diff_types.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py` & `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py` & `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import xmltodict
-from devon.agent.tools.unified_diff.utils import UnifiedDiff
+from devon_agent.agent.tools.unified_diff.utils import UnifiedDiff
 
 end_json_symbol = "<END>"
 
 begin_xml = "<root>"
 
 model = UnifiedDiff.model_json_schema()
 data_model = str(xmltodict.unparse({"root": UnifiedDiff.model_json_schema()}, pretty=True))
```

### Comparing `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/utils.py` & `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import difflib
-from devon.agent.tools.unified_diff.create_diff import FileDiff, MultiFileDiff, construct_versions_from_diff_hunk, extract_diffs, parse_multi_file_diff2
+from devon_agent.agent.tools.unified_diff.create_diff import FileDiff, MultiFileDiff, construct_versions_from_diff_hunk, extract_diffs, parse_multi_file_diff2
 import os
 
-from devon.agent.tools.unified_diff.diff_types import MultiFileDiff2
+from devon_agent.agent.tools.unified_diff.diff_types import MultiFileDiff2
 
 def first_and_last_content_lines(lines):
     start = 0
     for i, line in enumerate(lines):
         if line != '':
             start = i
             break
@@ -118,15 +118,15 @@
 +
 </DIFF>
 
 <DIFF>
 --- /dev/null
 +++ agent/kernel/state_machine/state_machine.py
 @@ -0,0 +1,19 @@
-+from devon.agent.kernel.state_machine.state_types import State
++from devon_agent.agent.kernel.state_machine.state_types import State
 +
 +class StateMachine:
 +
 +    def __init__(self, state: State):
 +        self.state = state
 +        self.state_dict = {}
 +
@@ -209,22 +209,22 @@
 +    def execute(self, context):
 +        # Implement termination logic here
 </DIFF>
 
 <DIFF>
 --- agent/kernel/thread.py
 +++ agent/kernel/thread.py
-@@ -10,6 +10,7 @@ from devon.agent.tools.unified_diff.utils import apply_diff, apply_diff2, apply_
- from devon.sandbox.environments import EnvironmentProtocol
- from devon.format import reformat_code
- from devon.agent.reasoning.reason import ReasoningPrompts
+@@ -10,6 +10,7 @@ from devon_agent.agent.tools.unified_diff.utils import apply_diff, apply_diff2, apply_
+ from devon_agent.sandbox.environments import EnvironmentProtocol
+ from devon_agent.format import reformat_code
+ from devon_agent.agent.reasoning.reason import ReasoningPrompts
 +from agent.kernel.state_machine.state_machine import StateMachine
  from agent.evaluate.evaluate import EvaluatePrompts
  from anthropic import Anthropic
- from devon.agent.clients.client import ClaudeHaiku, ClaudeOpus, ClaudeSonnet, Message
+ from devon_agent.agent.clients.client import ClaudeHaiku, ClaudeOpus, ClaudeSonnet, Message
 @@ -40,7 +41,7 @@ class Thread:
              success = False
              failure_context = []
              state_manager = StateMachine(state="reason")
 -            file_system = env.tools.file_system(path=os.getcwd())
 +            state_manager.add_state("reason", ReasonState)
```

### Comparing `devon_agent-0.0.2/devon_agent/format.py` & `devon_agent-0.0.3/devon_agent/format.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.2/devon_agent/main.py` & `devon_agent-0.0.3/devon_agent/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import openai
 import os
 import dotenv
 from anthropic import Anthropic
 
-from devon.agent.kernel.thread import Thread
-from devon.sandbox.environments import LocalEnvironment
+from devon_agent.agent.kernel.thread import Thread
+from devon_agent.sandbox.environments import LocalEnvironment
 
 dotenv.load_dotenv()
 
 def main():
     import argparse
 
     parser = argparse.ArgumentParser(description="Process inputs for the agent.")
```

### Comparing `devon_agent-0.0.2/devon_agent/sandbox/environments.py` & `devon_agent-0.0.3/devon_agent/sandbox/environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import docker
 from typing import Optional
 
-from devon.sandbox.tool_proxy import LocalToolProxy, ToolProxy
+from devon_agent.sandbox.tool_proxy import LocalToolProxy, ToolProxy
 
 """
 This module contains the PythonContainer class, which represents a Docker container running Python.
 
 The primary method of interacting with the container is the `execute` method, which runs a command inside the container and returns the output.
 """
```

### Comparing `devon_agent-0.0.2/devon_agent/sandbox/tool_proxy.py` & `devon_agent-0.0.3/devon_agent/sandbox/tool_proxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 import os
 from typing import List
 
-from devon.agent.clients.tool_utils.tools import Toolbox
-from devon.agent.tools.file_system.fs import FileSystemTool
-from devon.agent.tools.git_tool.git_tool import GitTool
-from devon.agent.tools.github.github_tool import GitHubTool
+from devon_agent.agent.clients.tool_utils.tools import Toolbox
+from devon_agent.agent.tools.file_system.fs import FileSystemTool
+from devon_agent.agent.tools.git_tool.git_tool import GitTool
+from devon_agent.agent.tools.github.github_tool import GitHubTool
 
 
 @dataclass
 class ToolProxy(ABC):
 
     @abstractmethod
     def file_system(self, path) -> FileSystemTool:
```

### Comparing `devon_agent-0.0.2/devon_agent/tests/state_functions.py` & `devon_agent-0.0.3/devon_agent/tests/state_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 import json
 import xmltodict
 from typing import List, Literal, Optional, Union, Any
 
 from anthropic import Anthropic
 from pydantic import BaseModel, Field
-from devon.parsing import parse_code, end_json_symbol, begin_xml
-from devon.agent.tools.unified_diff.utils import UnifiedDiff, xml_to_unified_diff, apply_diff
+from devon_agent.parsing import parse_code, end_json_symbol, begin_xml
+from devon_agent.agent.tools.unified_diff.utils import UnifiedDiff, xml_to_unified_diff, apply_diff
 import dotenv
 
 from format import reformat_code
 from sandbox.shell import Shell
 
 class CodeFile(BaseModel):
     filepath: str
```

### Comparing `devon_agent-0.0.2/devon_agent/tests/test_diff.py` & `devon_agent-0.0.3/devon_agent/tests/test_diff.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from anthropic import Anthropic
 
-from devon.agent.clients.client import ClaudeOpus
-from devon.agent.tools.unified_diff.create_diff import generate_unified_diff
-from devon.agent.tools.unified_diff.prompts.udiff_prompts import UnifiedDiffPrompts
-from devon.agent.tools.unified_diff.utils import apply_diff_to_file
+from devon_agent.agent.clients.client import ClaudeOpus
+from devon_agent.agent.tools.unified_diff.create_diff import generate_unified_diff
+from devon_agent.agent.tools.unified_diff.prompts.udiff_prompts import UnifiedDiffPrompts
+from devon_agent.agent.tools.unified_diff.utils import apply_diff_to_file
 
 import ast
 
 def get_file(file_path):
     try:
         with open(file=file_path) as f:
             code_lines = f.readlines()
```

### Comparing `devon_agent-0.0.2/pyproject.toml` & `devon_agent-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 package-mode = true
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
@@ -23,7 +23,12 @@
 unidiff = "^0.7.5"
 gitpython = "^3.1.42"
 pytest-json-report = "^1.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.poetry.scripts]
+devon = "devon_agent.__main__:main"
+
```

### Comparing `devon_agent-0.0.2/PKG-INFO` & `devon_agent-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

