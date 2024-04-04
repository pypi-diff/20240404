# Comparing `tmp/devon_agent-0.0.3.tar.gz` & `tmp/devon_agent-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.0.3.tar", max compression
+gzip compressed data, was "devon_agent-0.0.4.tar", max compression
```

## Comparing `devon_agent-0.0.3.tar` & `devon_agent-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.3/LICENSE
--rw-r--r--   0        0        0     1371 2024-04-04 01:01:24.013453 devon_agent-0.0.3/README.md
--rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.3/devon_agent/__main__.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.3/devon_agent/agent/__init__.py
--rw-r--r--   0        0        0     5378 2024-04-04 01:56:29.973522 devon_agent-0.0.3/devon_agent/agent/clients/client.py
--rw-r--r--   0        0        0     1387 2024-04-04 01:56:29.975197 devon_agent-0.0.3/devon_agent/agent/clients/test_function_client.py
--rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.3/devon_agent/agent/clients/tool_utils/tools.py
--rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.3/devon_agent/agent/evaluate/evaluate.py
--rw-r--r--   0        0        0      873 2024-04-04 01:56:29.933293 devon_agent-0.0.3/devon_agent/agent/kernel/context.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/__init__.py
--rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/state.py
--rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/state_machine.py
--rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/state_types.py
--rw-r--r--   0        0        0     1768 2024-04-04 01:56:29.933283 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/evaluate.py
--rw-r--r--   0        0        0     1998 2024-04-04 01:56:29.932370 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/reason.py
--rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/terminate.py
--rw-r--r--   0        0        0     1808 2024-04-04 01:56:29.932353 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/tool.py
--rw-r--r--   0        0        0     2768 2024-04-04 01:56:29.932381 devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/write.py
--rw-r--r--   0        0        0     5805 2024-04-04 01:56:29.932954 devon_agent-0.0.3/devon_agent/agent/kernel/thread.py
--rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.3/devon_agent/agent/reasoning/reason.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.3/devon_agent/agent/tools/__init__.py
--rw-r--r--   0        0        0     6289 2024-04-04 01:56:29.969363 devon_agent-0.0.3/devon_agent/agent/tools/file_system/fs.py
--rw-r--r--   0        0        0     2276 2024-04-04 01:56:29.938196 devon_agent-0.0.3/devon_agent/agent/tools/file_system/test_fs_tool.py
--rw-r--r--   0        0        0     5147 2024-04-04 01:56:29.969375 devon_agent-0.0.3/devon_agent/agent/tools/git_tool/git_tool.py
--rw-r--r--   0        0        0     2013 2024-04-04 01:56:29.969323 devon_agent-0.0.3/devon_agent/agent/tools/git_tool/test_git_tool.py
--rw-r--r--   0        0        0     4339 2024-04-04 01:56:29.933945 devon_agent-0.0.3/devon_agent/agent/tools/github/github_tool.py
--rw-r--r--   0        0        0     2930 2024-04-04 01:56:29.934004 devon_agent-0.0.3/devon_agent/agent/tools/github/test_github_tool.py
--rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.3/devon_agent/agent/tools/tool_prompts.py
--rw-r--r--   0        0        0     6632 2024-04-04 01:56:29.972647 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/create_diff.py
--rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/diff_types.py
--rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
--rw-r--r--   0        0        0     9283 2024-04-04 01:02:20.669812 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
--rw-r--r--   0        0        0     1791 2024-04-04 01:56:29.969391 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
--rw-r--r--   0        0        0     8275 2024-04-04 01:56:29.971937 devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/utils.py
--rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.3/devon_agent/format.py
--rw-r--r--   0        0        0     1089 2024-04-04 01:56:29.923857 devon_agent-0.0.3/devon_agent/main.py
--rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.3/devon_agent/react.py
--rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.3/devon_agent/run.txt
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.3/devon_agent/sandbox/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-04 01:56:29.975187 devon_agent-0.0.3/devon_agent/sandbox/environments.py
--rw-r--r--   0        0        0      952 2024-04-04 01:56:29.975161 devon_agent-0.0.3/devon_agent/sandbox/tool_proxy.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.3/devon_agent/tests/__init__.py
--rw-r--r--   0        0        0     6189 2024-04-04 01:56:29.985125 devon_agent-0.0.3/devon_agent/tests/state_functions.py
--rw-r--r--   0        0        0     1900 2024-04-04 01:56:29.975172 devon_agent-0.0.3/devon_agent/tests/test_diff.py
--rw-r--r--   0        0        0      726 2024-04-04 01:56:45.966620 devon_agent-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 devon_agent-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1371 2024-04-04 01:01:24.013453 devon_agent-0.0.4/README.md
+-rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.4/devon_agent/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.4/devon_agent/agent/__init__.py
+-rw-r--r--   0        0        0     5378 2024-04-04 01:56:29.973522 devon_agent-0.0.4/devon_agent/agent/clients/client.py
+-rw-r--r--   0        0        0     1387 2024-04-04 01:56:29.975197 devon_agent-0.0.4/devon_agent/agent/clients/test_function_client.py
+-rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.4/devon_agent/agent/clients/tool_utils/tools.py
+-rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.4/devon_agent/agent/evaluate/evaluate.py
+-rw-r--r--   0        0        0      873 2024-04-04 01:56:29.933293 devon_agent-0.0.4/devon_agent/agent/kernel/context.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/state.py
+-rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/state_machine.py
+-rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/state_types.py
+-rw-r--r--   0        0        0     1792 2024-04-04 01:57:52.376175 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/evaluate.py
+-rw-r--r--   0        0        0     1998 2024-04-04 01:56:29.932370 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/reason.py
+-rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/terminate.py
+-rw-r--r--   0        0        0     1808 2024-04-04 01:56:29.932353 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/tool.py
+-rw-r--r--   0        0        0     2768 2024-04-04 01:56:29.932381 devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/write.py
+-rw-r--r--   0        0        0     5805 2024-04-04 01:56:29.932954 devon_agent-0.0.4/devon_agent/agent/kernel/thread.py
+-rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.4/devon_agent/agent/reasoning/reason.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.4/devon_agent/agent/tools/__init__.py
+-rw-r--r--   0        0        0     6289 2024-04-04 01:56:29.969363 devon_agent-0.0.4/devon_agent/agent/tools/file_system/fs.py
+-rw-r--r--   0        0        0     2276 2024-04-04 01:56:29.938196 devon_agent-0.0.4/devon_agent/agent/tools/file_system/test_fs_tool.py
+-rw-r--r--   0        0        0     5147 2024-04-04 01:56:29.969375 devon_agent-0.0.4/devon_agent/agent/tools/git_tool/git_tool.py
+-rw-r--r--   0        0        0     2013 2024-04-04 01:56:29.969323 devon_agent-0.0.4/devon_agent/agent/tools/git_tool/test_git_tool.py
+-rw-r--r--   0        0        0     4339 2024-04-04 01:56:29.933945 devon_agent-0.0.4/devon_agent/agent/tools/github/github_tool.py
+-rw-r--r--   0        0        0     2930 2024-04-04 01:56:29.934004 devon_agent-0.0.4/devon_agent/agent/tools/github/test_github_tool.py
+-rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.4/devon_agent/agent/tools/tool_prompts.py
+-rw-r--r--   0        0        0     6632 2024-04-04 01:56:29.972647 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/create_diff.py
+-rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/diff_types.py
+-rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
+-rw-r--r--   0        0        0     9283 2024-04-04 01:02:20.669812 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
+-rw-r--r--   0        0        0     1791 2024-04-04 01:56:29.969391 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
+-rw-r--r--   0        0        0     8275 2024-04-04 01:56:29.971937 devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/utils.py
+-rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.4/devon_agent/format.py
+-rw-r--r--   0        0        0     1089 2024-04-04 01:56:29.923857 devon_agent-0.0.4/devon_agent/main.py
+-rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.4/devon_agent/react.py
+-rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.4/devon_agent/run.txt
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.4/devon_agent/sandbox/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-04 01:56:29.975187 devon_agent-0.0.4/devon_agent/sandbox/environments.py
+-rw-r--r--   0        0        0      952 2024-04-04 01:56:29.975161 devon_agent-0.0.4/devon_agent/sandbox/tool_proxy.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.4/devon_agent/tests/__init__.py
+-rw-r--r--   0        0        0     6189 2024-04-04 01:56:29.985125 devon_agent-0.0.4/devon_agent/tests/state_functions.py
+-rw-r--r--   0        0        0     1900 2024-04-04 01:56:29.975172 devon_agent-0.0.4/devon_agent/tests/test_diff.py
+-rw-r--r--   0        0        0      726 2024-04-04 01:58:02.923113 devon_agent-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 devon_agent-0.0.4/PKG-INFO
```

### Comparing `devon_agent-0.0.3/LICENSE` & `devon_agent-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/README.md` & `devon_agent-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/clients/client.py` & `devon_agent-0.0.4/devon_agent/agent/clients/client.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/clients/test_function_client.py` & `devon_agent-0.0.4/devon_agent/agent/clients/test_function_client.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/clients/tool_utils/tools.py` & `devon_agent-0.0.4/devon_agent/agent/clients/tool_utils/tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/evaluate/evaluate.py` & `devon_agent-0.0.4/devon_agent/agent/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/kernel/context.py` & `devon_agent-0.0.4/devon_agent/agent/kernel/context.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/state_machine.py` & `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/state_machine.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/evaluate.py` & `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/evaluate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 import json
 
 from devon_agent.agent.clients.client import LanguageModel, Message
 from devon_agent.agent.evaluate.evaluate import EvaluatePrompts
-from agent.kernel.state_machine.state import State
-from agent.kernel.context import BaseStateContext
+from devon_agent.agent.kernel.state_machine.state import State
+from devon_agent.agent.kernel.context import BaseStateContext
 
 from dataclasses import dataclass
 from devon_agent.agent.kernel.context import BaseStateContext
 from devon_agent.agent.kernel.state_machine.states.reason import ReasoningResult
 
 @dataclass
 class EvaluateParameters:
```

### Comparing `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/reason.py` & `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/reason.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/tool.py` & `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/kernel/state_machine/states/write.py` & `devon_agent-0.0.4/devon_agent/agent/kernel/state_machine/states/write.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/kernel/thread.py` & `devon_agent-0.0.4/devon_agent/agent/kernel/thread.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/reasoning/reason.py` & `devon_agent-0.0.4/devon_agent/agent/reasoning/reason.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/file_system/fs.py` & `devon_agent-0.0.4/devon_agent/agent/tools/file_system/fs.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/file_system/test_fs_tool.py` & `devon_agent-0.0.4/devon_agent/agent/tools/file_system/test_fs_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/git_tool/git_tool.py` & `devon_agent-0.0.4/devon_agent/agent/tools/git_tool/git_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/git_tool/test_git_tool.py` & `devon_agent-0.0.4/devon_agent/agent/tools/git_tool/test_git_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/github/github_tool.py` & `devon_agent-0.0.4/devon_agent/agent/tools/github/github_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/github/test_github_tool.py` & `devon_agent-0.0.4/devon_agent/agent/tools/github/test_github_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/tool_prompts.py` & `devon_agent-0.0.4/devon_agent/agent/tools/tool_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/create_diff.py` & `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/create_diff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/diff_types.py` & `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/diff_types.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py` & `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py` & `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/agent/tools/unified_diff/utils.py` & `devon_agent-0.0.4/devon_agent/agent/tools/unified_diff/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/format.py` & `devon_agent-0.0.4/devon_agent/format.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/main.py` & `devon_agent-0.0.4/devon_agent/main.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/sandbox/environments.py` & `devon_agent-0.0.4/devon_agent/sandbox/environments.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/sandbox/tool_proxy.py` & `devon_agent-0.0.4/devon_agent/sandbox/tool_proxy.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/tests/state_functions.py` & `devon_agent-0.0.4/devon_agent/tests/state_functions.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/devon_agent/tests/test_diff.py` & `devon_agent-0.0.4/devon_agent/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.3/pyproject.toml` & `devon_agent-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 package-mode = true
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `devon_agent-0.0.3/PKG-INFO` & `devon_agent-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

