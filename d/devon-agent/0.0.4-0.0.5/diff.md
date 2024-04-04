# Comparing `tmp/devon_agent-0.0.4.tar.gz` & `tmp/devon_agent-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.0.4.tar", max compression
+gzip compressed data, was "devon_agent-0.0.5.tar", max compression
```

## Comparing `devon_agent-0.0.4.tar` & `devon_agent-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.4/LICENSE
--rw-r--r--   0        0        0     1371 2024-04-04 01:01:24.013453 devon_agent-0.0.4/README.md
--rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.4/devon_agent/__main__.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.4/devon_agent/agent/__init__.py
--rw-r--r--   0        0        0     5378 2024-04-04 01:56:29.973522 devon_agent-0.0.4/devon_agent/agent/clients/client.py
--rw-r--r--   0        0        0     1387 2024-04-04 01:56:29.975197 devon_agent-0.0.4/devon_agent/agent/clients/test_function_client.py
--rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.4/devon_agent/agent/clients/tool_utils/tools.py
--rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.4/devon_agent/agent/evaluate/evaluate.py
--rw-r--r--   0        0        0      873 2024-04-04 01:56:29.933293 devon_agent-0.0.4/devon_agent/agent/kernel/context.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/__init__.py
--rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/state.py
--rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/state_machine.py
--rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/state_types.py
--rw-r--r--   0        0        0     1792 2024-04-04 01:57:52.376175 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/evaluate.py
--rw-r--r--   0        0        0     1998 2024-04-04 01:56:29.932370 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/reason.py
--rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/terminate.py
--rw-r--r--   0        0        0     1808 2024-04-04 01:56:29.932353 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/tool.py
--rw-r--r--   0        0        0     2768 2024-04-04 01:56:29.932381 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/write.py
--rw-r--r--   0        0        0     5805 2024-04-04 01:56:29.932954 devon_agent-0.0.4/devon_agent/agent/kernel/thread.py
--rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.4/devon_agent/agent/reasoning/reason.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.4/devon_agent/agent/tools/__init__.py
--rw-r--r--   0        0        0     6289 2024-04-04 01:56:29.969363 devon_agent-0.0.4/devon_agent/agent/tools/file_system/fs.py
--rw-r--r--   0        0        0     2276 2024-04-04 01:56:29.938196 devon_agent-0.0.4/devon_agent/agent/tools/file_system/test_fs_tool.py
--rw-r--r--   0        0        0     5147 2024-04-04 01:56:29.969375 devon_agent-0.0.4/devon_agent/agent/tools/git_tool/git_tool.py
--rw-r--r--   0        0        0     2013 2024-04-04 01:56:29.969323 devon_agent-0.0.4/devon_agent/agent/tools/git_tool/test_git_tool.py
--rw-r--r--   0        0        0     4339 2024-04-04 01:56:29.933945 devon_agent-0.0.4/devon_agent/agent/tools/github/github_tool.py
--rw-r--r--   0        0        0     2930 2024-04-04 01:56:29.934004 devon_agent-0.0.4/devon_agent/agent/tools/github/test_github_tool.py
--rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.4/devon_agent/agent/tools/tool_prompts.py
--rw-r--r--   0        0        0     6632 2024-04-04 01:56:29.972647 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/create_diff.py
--rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/diff_types.py
--rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
--rw-r--r--   0        0        0     9283 2024-04-04 01:02:20.669812 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
--rw-r--r--   0        0        0     1791 2024-04-04 01:56:29.969391 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
--rw-r--r--   0        0        0     8275 2024-04-04 01:56:29.971937 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/utils.py
--rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.4/devon_agent/format.py
--rw-r--r--   0        0        0     1089 2024-04-04 01:56:29.923857 devon_agent-0.0.4/devon_agent/main.py
--rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.4/devon_agent/react.py
--rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.4/devon_agent/run.txt
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.4/devon_agent/sandbox/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-04 01:56:29.975187 devon_agent-0.0.4/devon_agent/sandbox/environments.py
--rw-r--r--   0        0        0      952 2024-04-04 01:56:29.975161 devon_agent-0.0.4/devon_agent/sandbox/tool_proxy.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.4/devon_agent/tests/__init__.py
--rw-r--r--   0        0        0     6189 2024-04-04 01:56:29.985125 devon_agent-0.0.4/devon_agent/tests/state_functions.py
--rw-r--r--   0        0        0     1900 2024-04-04 01:56:29.975172 devon_agent-0.0.4/devon_agent/tests/test_diff.py
--rw-r--r--   0        0        0      726 2024-04-04 01:58:02.923113 devon_agent-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 devon_agent-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1371 2024-04-04 01:01:24.013453 devon_agent-0.0.5/README.md
+-rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.5/devon_agent/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.5/devon_agent/agent/__init__.py
+-rw-r--r--   0        0        0     5378 2024-04-04 01:56:29.973522 devon_agent-0.0.5/devon_agent/agent/clients/client.py
+-rw-r--r--   0        0        0     1387 2024-04-04 01:56:29.975197 devon_agent-0.0.5/devon_agent/agent/clients/test_function_client.py
+-rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.5/devon_agent/agent/clients/tool_utils/tools.py
+-rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.5/devon_agent/agent/evaluate/evaluate.py
+-rw-r--r--   0        0        0      873 2024-04-04 01:56:29.933293 devon_agent-0.0.5/devon_agent/agent/kernel/context.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/state.py
+-rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/state_machine.py
+-rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/state_types.py
+-rw-r--r--   0        0        0     1792 2024-04-04 01:57:52.376175 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/evaluate.py
+-rw-r--r--   0        0        0     2010 2024-04-04 02:00:23.879608 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/reason.py
+-rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/terminate.py
+-rw-r--r--   0        0        0     1808 2024-04-04 01:56:29.932353 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/tool.py
+-rw-r--r--   0        0        0     2780 2024-04-04 02:00:37.502252 devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/write.py
+-rw-r--r--   0        0        0     5817 2024-04-04 02:01:07.734852 devon_agent-0.0.5/devon_agent/agent/kernel/thread.py
+-rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.5/devon_agent/agent/reasoning/reason.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.5/devon_agent/agent/tools/__init__.py
+-rw-r--r--   0        0        0     6289 2024-04-04 01:56:29.969363 devon_agent-0.0.5/devon_agent/agent/tools/file_system/fs.py
+-rw-r--r--   0        0        0     2276 2024-04-04 01:56:29.938196 devon_agent-0.0.5/devon_agent/agent/tools/file_system/test_fs_tool.py
+-rw-r--r--   0        0        0     5147 2024-04-04 01:56:29.969375 devon_agent-0.0.5/devon_agent/agent/tools/git_tool/git_tool.py
+-rw-r--r--   0        0        0     2013 2024-04-04 01:56:29.969323 devon_agent-0.0.5/devon_agent/agent/tools/git_tool/test_git_tool.py
+-rw-r--r--   0        0        0     4339 2024-04-04 01:56:29.933945 devon_agent-0.0.5/devon_agent/agent/tools/github/github_tool.py
+-rw-r--r--   0        0        0     2930 2024-04-04 01:56:29.934004 devon_agent-0.0.5/devon_agent/agent/tools/github/test_github_tool.py
+-rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.5/devon_agent/agent/tools/tool_prompts.py
+-rw-r--r--   0        0        0     6632 2024-04-04 01:56:29.972647 devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/create_diff.py
+-rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/diff_types.py
+-rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
+-rw-r--r--   0        0        0     9327 2024-04-04 01:59:06.433274 devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
+-rw-r--r--   0        0        0     1791 2024-04-04 01:56:29.969391 devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
+-rw-r--r--   0        0        0     8351 2024-04-04 01:59:32.584542 devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/utils.py
+-rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.5/devon_agent/format.py
+-rw-r--r--   0        0        0     1304 2024-04-04 02:02:12.119917 devon_agent-0.0.5/devon_agent/main.py
+-rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.5/devon_agent/react.py
+-rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.5/devon_agent/run.txt
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.5/devon_agent/sandbox/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-04 01:56:29.975187 devon_agent-0.0.5/devon_agent/sandbox/environments.py
+-rw-r--r--   0        0        0      952 2024-04-04 01:56:29.975161 devon_agent-0.0.5/devon_agent/sandbox/tool_proxy.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.5/devon_agent/tests/__init__.py
+-rw-r--r--   0        0        0     6189 2024-04-04 01:56:29.985125 devon_agent-0.0.5/devon_agent/tests/state_functions.py
+-rw-r--r--   0        0        0     1900 2024-04-04 01:56:29.975172 devon_agent-0.0.5/devon_agent/tests/test_diff.py
+-rw-r--r--   0        0        0      726 2024-04-04 02:02:27.360267 devon_agent-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 devon_agent-0.0.5/PKG-INFO
```

### Comparing `devon_agent-0.0.4/LICENSE` & `devon_agent-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/README.md` & `devon_agent-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/clients/client.py` & `devon_agent-0.0.5/devon_agent/agent/clients/client.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/clients/test_function_client.py` & `devon_agent-0.0.5/devon_agent/agent/clients/test_function_client.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/clients/tool_utils/tools.py` & `devon_agent-0.0.5/devon_agent/agent/clients/tool_utils/tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/evaluate/evaluate.py` & `devon_agent-0.0.5/devon_agent/agent/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/kernel/context.py` & `devon_agent-0.0.5/devon_agent/agent/kernel/context.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/state_machine.py` & `devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/state_machine.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/evaluate.py` & `devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/evaluate.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/reason.py` & `devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/reason.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 import json
 from devon_agent.agent.clients.client import LanguageModel, Message
 from devon_agent.agent.kernel.context import BaseStateContext
 from ..state import State
-from agent.reasoning.reason import ReasoningPrompts
+from devon_agent.agent.reasoning.reason import ReasoningPrompts
 
 # 1. Reasoning
     # Identify which files are necessary for the change
     # Create a mapping on a file level of what changes need to be made to each file
     # Review plan
 @dataclass
 class ReasoningParameters:
```

### Comparing `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/tool.py` & `devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/write.py` & `devon_agent-0.0.5/devon_agent/agent/kernel/state_machine/states/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from devon_agent.agent.clients.client import LanguageModel
 from devon_agent.agent.kernel.context import BaseStateContext
 from devon_agent.agent.kernel.state_machine.states.reason import ReasoningResult
 
 from devon_agent.agent.tools.unified_diff.create_diff import generate_unified_diff2
 from devon_agent.agent.tools.unified_diff.utils import apply_diff2
 from ..state import State
-from agent.tools.file_system.fs import FileSystemTool
+from devon_agent.agent.tools.file_system.fs import FileSystemTool
 
 @dataclass
 class WriteParameters:
     diff_model: LanguageModel
 
 @dataclass
 class WriteContext:
```

### Comparing `devon_agent-0.0.4/devon_agent/agent/kernel/thread.py` & `devon_agent-0.0.5/devon_agent/agent/kernel/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from devon_agent.agent.tools.tool_prompts import ToolPrompts
 from devon_agent.agent.tools.unified_diff.create_diff import generate_unified_diff2
 from devon_agent.agent.tools.unified_diff.prompts.udiff_prompts import UnifiedDiffPrompts
 from devon_agent.agent.tools.unified_diff.utils import apply_diff2
 from devon_agent.sandbox.environments import EnvironmentProtocol
 from devon_agent.format import reformat_code
 from devon_agent.agent.reasoning.reason import ReasoningPrompts
-from agent.evaluate.evaluate import EvaluatePrompts
+from devon_agent.agent.evaluate.evaluate import EvaluatePrompts
 from anthropic import Anthropic
 from devon_agent.agent.clients.client import GPT4, ClaudeHaiku, ClaudeOpus, ClaudeSonnet, Message
 import json
 import traceback
 import xmltodict
 from .state_machine.state_machine import StateMachine
 from .state_machine.state_types import StateType
```

### Comparing `devon_agent-0.0.4/devon_agent/agent/reasoning/reason.py` & `devon_agent-0.0.5/devon_agent/agent/reasoning/reason.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/file_system/fs.py` & `devon_agent-0.0.5/devon_agent/agent/tools/file_system/fs.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/file_system/test_fs_tool.py` & `devon_agent-0.0.5/devon_agent/agent/tools/file_system/test_fs_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/git_tool/git_tool.py` & `devon_agent-0.0.5/devon_agent/agent/tools/git_tool/git_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/git_tool/test_git_tool.py` & `devon_agent-0.0.5/devon_agent/agent/tools/git_tool/test_git_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/github/github_tool.py` & `devon_agent-0.0.5/devon_agent/agent/tools/github/github_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/github/test_github_tool.py` & `devon_agent-0.0.5/devon_agent/agent/tools/github/test_github_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/tool_prompts.py` & `devon_agent-0.0.5/devon_agent/agent/tools/tool_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/create_diff.py` & `devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/create_diff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/diff_types.py` & `devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/diff_types.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py` & `devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,29 +118,29 @@
 +++ mathweb/flask/app.py
 @@ -10,1 +10,1 @@ 
 client_ip = "192.168.23.104"
 
 
 WRONG:
 @@ -0,0 +1,7 @@
-+1: from agent.kernel.state_machine.state_machine import State
++1: fromdevon_agent.agent.kernel.state_machine.state_machine import State
 +2: 
 +3: 
 +4: class TerminateState(State):
 +5:     def execute(self, context):
 +6:         # Implement termination logic here
 +7:         pass
 
 CORRECT:
 --- agent/kernel/thread.py
 +++ agent/kernel/thread.py
 @@ -0,0 +1,7 @@
- from agent.kernel.state_machine.state_machine import StateMachine
- from agent.kernel.state_machine.state_types import types
-+from agent.kernel.state_machine.state_machine import State
+ fromdevon_agent.agent.kernel.state_machine.state_machine import StateMachine
+ fromdevon_agent.agent.kernel.state_machine.state_types import types
++fromdevon_agent.agent.kernel.state_machine.state_machine import State
 +
 +
 +class TerminateState(State):
 +    def execute(self, context):
 +        # Implement termination logic here
 +        pass
```

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py` & `devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/utils.py` & `devon_agent-0.0.5/devon_agent/agent/tools/unified_diff/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,74 +155,74 @@
 +        pass
 </DIFF>
 
 <DIFF>
 --- /dev/null
 +++ agent/kernel/state_machine/states/reason.py
 @@ -0,0 +1,5 @@
-+from agent.kernel.state_machine.state import State
++fromdevon_agent.agent.kernel.state_machine.state import State
 +
 +class ReasonState(State):
 +    def execute(self, context):
 +        # Implement reasoning logic here
 </DIFF>
 
 <DIFF>
 --- /dev/null
 +++ agent/kernel/state_machine/states/write.py
 @@ -0,0 +1,5 @@
-+from agent.kernel.state_machine.state import State
++fromdevon_agent.agent.kernel.state_machine.state import State
 +
 +class WriteState(State):
 +    def execute(self, context):
 +        # Implement code writing logic here
 </DIFF>
 
 <DIFF>
 --- /dev/null
 +++ agent/kernel/state_machine/states/execute.py
 @@ -0,0 +1,5 @@
-+from agent.kernel.state_machine.state import State
++fromdevon_agent.agent.kernel.state_machine.state import State
 +
 +class ExecuteState(State):
 +    def execute(self, context):
 +        # Implement code execution logic here
 </DIFF>
 
 <DIFF>
 --- /dev/null
 +++ agent/kernel/state_machine/states/evaluate.py
 @@ -0,0 +1,5 @@
-+from agent.kernel.state_machine.state import State
++fromdevon_agent.agent.kernel.state_machine.state import State
 +
 +class EvaluateState(State):
 +    def execute(self, context):
 +        # Implement code evaluation logic here
 </DIFF>
 
 <DIFF>
 --- /dev/null
 +++ agent/kernel/state_machine/states/terminate.py
 @@ -0,0 +1,5 @@
-+from agent.kernel.state_machine.state import State
++fromdevon_agent.agent.kernel.state_machine.state import State
 +
 +class TerminateState(State):
 +    def execute(self, context):
 +        # Implement termination logic here
 </DIFF>
 
 <DIFF>
 --- agent/kernel/thread.py
 +++ agent/kernel/thread.py
 @@ -10,6 +10,7 @@ from devon_agent.agent.tools.unified_diff.utils import apply_diff, apply_diff2, apply_
  from devon_agent.sandbox.environments import EnvironmentProtocol
  from devon_agent.format import reformat_code
  from devon_agent.agent.reasoning.reason import ReasoningPrompts
-+from agent.kernel.state_machine.state_machine import StateMachine
- from agent.evaluate.evaluate import EvaluatePrompts
++fromdevon_agent.agent.kernel.state_machine.state_machine import StateMachine
+ fromdevon_agent.agentevaluate.evaluate import EvaluatePrompts
  from anthropic import Anthropic
  from devon_agent.agent.clients.client import ClaudeHaiku, ClaudeOpus, ClaudeSonnet, Message
 @@ -40,7 +41,7 @@ class Thread:
              success = False
              failure_context = []
              state_manager = StateMachine(state="reason")
 -            file_system = env.tools.file_system(path=os.getcwd())
```

### Comparing `devon_agent-0.0.4/devon_agent/format.py` & `devon_agent-0.0.5/devon_agent/format.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/main.py` & `devon_agent-0.0.5/devon_agent/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+import sys
 import openai
 import os
 import dotenv
 from anthropic import Anthropic
 
 from devon_agent.agent.kernel.thread import Thread
 from devon_agent.sandbox.environments import LocalEnvironment
 
 dotenv.load_dotenv()
 
 def main():
     import argparse
-
-    parser = argparse.ArgumentParser(description="Process inputs for the agent.")
+    parser = argparse.ArgumentParser(description="Process inputs for the agent.", usage='%(prog)s --goal <goal> [--path <path>] [--repo_url <repo_url>] [--question <question>]')
 
     parser.add_argument('--path', type=str, help='File Path', default=os.getcwd())
     parser.add_argument('--repo_url', type=str, help='GitHub Repository URL', default=None)
-    parser.add_argument('--goal', type=str, help='Describe your goal')
+    parser.add_argument('--goal', type=str, help='Describe your goal', required=True)
     parser.add_argument('--question', type=str, help='Describe your question about this code base')
     args = parser.parse_args()
 
+    if not args.goal and not args.question:
+        parser.print_usage()
+        sys.exit(1)
+
     repo_url = args.repo_url
     goal = args.goal
     path = args.path
     qa = False
 
     env = LocalEnvironment()
```

### Comparing `devon_agent-0.0.4/devon_agent/sandbox/environments.py` & `devon_agent-0.0.5/devon_agent/sandbox/environments.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/sandbox/tool_proxy.py` & `devon_agent-0.0.5/devon_agent/sandbox/tool_proxy.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/tests/state_functions.py` & `devon_agent-0.0.5/devon_agent/tests/state_functions.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/devon_agent/tests/test_diff.py` & `devon_agent-0.0.5/devon_agent/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.4/pyproject.toml` & `devon_agent-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 package-mode = true
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `devon_agent-0.0.4/PKG-INFO` & `devon_agent-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

