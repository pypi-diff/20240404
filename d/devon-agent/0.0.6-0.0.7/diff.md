# Comparing `tmp/devon_agent-0.0.6.tar.gz` & `tmp/devon_agent-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.0.6.tar", max compression
+gzip compressed data, was "devon_agent-0.0.7.tar", max compression
```

## Comparing `devon_agent-0.0.6.tar` & `devon_agent-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.6/LICENSE
--rw-r--r--   0        0        0     1467 2024-04-04 02:52:51.583958 devon_agent-0.0.6/README.md
--rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.6/devon_agent/__main__.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.6/devon_agent/agent/__init__.py
--rw-r--r--   0        0        0     5378 2024-04-04 01:56:29.973522 devon_agent-0.0.6/devon_agent/agent/clients/client.py
--rw-r--r--   0        0        0     1387 2024-04-04 01:56:29.975197 devon_agent-0.0.6/devon_agent/agent/clients/test_function_client.py
--rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.6/devon_agent/agent/clients/tool_utils/tools.py
--rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.6/devon_agent/agent/evaluate/evaluate.py
--rw-r--r--   0        0        0      873 2024-04-04 01:56:29.933293 devon_agent-0.0.6/devon_agent/agent/kernel/context.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/__init__.py
--rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/state.py
--rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/state_machine.py
--rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/state_types.py
--rw-r--r--   0        0        0     1792 2024-04-04 01:57:52.376175 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/evaluate.py
--rw-r--r--   0        0        0     2010 2024-04-04 02:00:23.879608 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/reason.py
--rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/terminate.py
--rw-r--r--   0        0        0     1808 2024-04-04 01:56:29.932353 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/tool.py
--rw-r--r--   0        0        0     2780 2024-04-04 02:00:37.502252 devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/write.py
--rw-r--r--   0        0        0     5824 2024-04-04 02:52:20.528986 devon_agent-0.0.6/devon_agent/agent/kernel/thread.py
--rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.6/devon_agent/agent/reasoning/reason.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.6/devon_agent/agent/tools/__init__.py
--rw-r--r--   0        0        0     6289 2024-04-04 01:56:29.969363 devon_agent-0.0.6/devon_agent/agent/tools/file_system/fs.py
--rw-r--r--   0        0        0     2276 2024-04-04 01:56:29.938196 devon_agent-0.0.6/devon_agent/agent/tools/file_system/test_fs_tool.py
--rw-r--r--   0        0        0     5147 2024-04-04 01:56:29.969375 devon_agent-0.0.6/devon_agent/agent/tools/git_tool/git_tool.py
--rw-r--r--   0        0        0     2013 2024-04-04 01:56:29.969323 devon_agent-0.0.6/devon_agent/agent/tools/git_tool/test_git_tool.py
--rw-r--r--   0        0        0     4339 2024-04-04 01:56:29.933945 devon_agent-0.0.6/devon_agent/agent/tools/github/github_tool.py
--rw-r--r--   0        0        0     2930 2024-04-04 01:56:29.934004 devon_agent-0.0.6/devon_agent/agent/tools/github/test_github_tool.py
--rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.6/devon_agent/agent/tools/tool_prompts.py
--rw-r--r--   0        0        0     6632 2024-04-04 01:56:29.972647 devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/create_diff.py
--rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/diff_types.py
--rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
--rw-r--r--   0        0        0     9327 2024-04-04 01:59:06.433274 devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
--rw-r--r--   0        0        0     1791 2024-04-04 01:56:29.969391 devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
--rw-r--r--   0        0        0     8351 2024-04-04 01:59:32.584542 devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/utils.py
--rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.6/devon_agent/format.py
--rw-r--r--   0        0        0     1304 2024-04-04 02:02:12.119917 devon_agent-0.0.6/devon_agent/main.py
--rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.6/devon_agent/react.py
--rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.6/devon_agent/run.txt
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.6/devon_agent/sandbox/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-04 01:56:29.975187 devon_agent-0.0.6/devon_agent/sandbox/environments.py
--rw-r--r--   0        0        0      952 2024-04-04 01:56:29.975161 devon_agent-0.0.6/devon_agent/sandbox/tool_proxy.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.6/devon_agent/tests/__init__.py
--rw-r--r--   0        0        0     6189 2024-04-04 01:56:29.985125 devon_agent-0.0.6/devon_agent/tests/state_functions.py
--rw-r--r--   0        0        0     1900 2024-04-04 01:56:29.975172 devon_agent-0.0.6/devon_agent/tests/test_diff.py
--rw-r--r--   0        0        0      726 2024-04-04 02:53:59.144913 devon_agent-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 devon_agent-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1467 2024-04-04 02:52:51.583958 devon_agent-0.0.7/README.md
+-rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.7/devon_agent/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.7/devon_agent/agent/__init__.py
+-rw-r--r--   0        0        0     5378 2024-04-04 01:56:29.973522 devon_agent-0.0.7/devon_agent/agent/clients/client.py
+-rw-r--r--   0        0        0     1387 2024-04-04 01:56:29.975197 devon_agent-0.0.7/devon_agent/agent/clients/test_function_client.py
+-rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.7/devon_agent/agent/clients/tool_utils/tools.py
+-rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.7/devon_agent/agent/evaluate/evaluate.py
+-rw-r--r--   0        0        0      873 2024-04-04 01:56:29.933293 devon_agent-0.0.7/devon_agent/agent/kernel/context.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/state.py
+-rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/state_machine.py
+-rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/state_types.py
+-rw-r--r--   0        0        0     1792 2024-04-04 01:57:52.376175 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/evaluate.py
+-rw-r--r--   0        0        0     2010 2024-04-04 02:00:23.879608 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/reason.py
+-rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/terminate.py
+-rw-r--r--   0        0        0     1808 2024-04-04 01:56:29.932353 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/tool.py
+-rw-r--r--   0        0        0     2880 2024-04-04 03:02:12.741187 devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/write.py
+-rw-r--r--   0        0        0     5824 2024-04-04 02:52:20.528986 devon_agent-0.0.7/devon_agent/agent/kernel/thread.py
+-rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.7/devon_agent/agent/reasoning/reason.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.7/devon_agent/agent/tools/__init__.py
+-rw-r--r--   0        0        0     6289 2024-04-04 01:56:29.969363 devon_agent-0.0.7/devon_agent/agent/tools/file_system/fs.py
+-rw-r--r--   0        0        0     2276 2024-04-04 01:56:29.938196 devon_agent-0.0.7/devon_agent/agent/tools/file_system/test_fs_tool.py
+-rw-r--r--   0        0        0     5147 2024-04-04 01:56:29.969375 devon_agent-0.0.7/devon_agent/agent/tools/git_tool/git_tool.py
+-rw-r--r--   0        0        0     2013 2024-04-04 01:56:29.969323 devon_agent-0.0.7/devon_agent/agent/tools/git_tool/test_git_tool.py
+-rw-r--r--   0        0        0     4339 2024-04-04 01:56:29.933945 devon_agent-0.0.7/devon_agent/agent/tools/github/github_tool.py
+-rw-r--r--   0        0        0     2930 2024-04-04 01:56:29.934004 devon_agent-0.0.7/devon_agent/agent/tools/github/test_github_tool.py
+-rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.7/devon_agent/agent/tools/tool_prompts.py
+-rw-r--r--   0        0        0     6632 2024-04-04 01:56:29.972647 devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/create_diff.py
+-rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/diff_types.py
+-rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
+-rw-r--r--   0        0        0     9327 2024-04-04 01:59:06.433274 devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
+-rw-r--r--   0        0        0     1791 2024-04-04 01:56:29.969391 devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
+-rw-r--r--   0        0        0     8351 2024-04-04 01:59:32.584542 devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/utils.py
+-rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.7/devon_agent/format.py
+-rw-r--r--   0        0        0     1304 2024-04-04 02:02:12.119917 devon_agent-0.0.7/devon_agent/main.py
+-rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.7/devon_agent/react.py
+-rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.7/devon_agent/run.txt
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.7/devon_agent/sandbox/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-04 01:56:29.975187 devon_agent-0.0.7/devon_agent/sandbox/environments.py
+-rw-r--r--   0        0        0      952 2024-04-04 01:56:29.975161 devon_agent-0.0.7/devon_agent/sandbox/tool_proxy.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.7/devon_agent/tests/__init__.py
+-rw-r--r--   0        0        0     6189 2024-04-04 01:56:29.985125 devon_agent-0.0.7/devon_agent/tests/state_functions.py
+-rw-r--r--   0        0        0     1900 2024-04-04 01:56:29.975172 devon_agent-0.0.7/devon_agent/tests/test_diff.py
+-rw-r--r--   0        0        0      726 2024-04-04 03:02:37.988553 devon_agent-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 devon_agent-0.0.7/PKG-INFO
```

### Comparing `devon_agent-0.0.6/LICENSE` & `devon_agent-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/README.md` & `devon_agent-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/clients/client.py` & `devon_agent-0.0.7/devon_agent/agent/clients/client.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/clients/test_function_client.py` & `devon_agent-0.0.7/devon_agent/agent/clients/test_function_client.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/clients/tool_utils/tools.py` & `devon_agent-0.0.7/devon_agent/agent/clients/tool_utils/tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/evaluate/evaluate.py` & `devon_agent-0.0.7/devon_agent/agent/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/kernel/context.py` & `devon_agent-0.0.7/devon_agent/agent/kernel/context.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/state_machine.py` & `devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/state_machine.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/evaluate.py` & `devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/evaluate.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/reason.py` & `devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/reason.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/tool.py` & `devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/kernel/state_machine/states/write.py` & `devon_agent-0.0.7/devon_agent/agent/kernel/state_machine/states/write.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         self.parameters = parameters
 
     def execute(self, context: WriteContext):
         file_context = context.global_context.load_file_context(context.global_context.fs_root)
         task = context.task
         diff_model = self.parameters.diff_model
         failure_context = []
-
+        if context.reasoning_result.create is None:
+            context.reasoning_result.create = []
         modify = context.reasoning_result.modify + [p for p in context.reasoning_result.create if os.path.exists(p)]
         files_to_change = [os.path.join(context.global_context.fs_root, path.strip()) for path in context.reasoning_result.files_to_change if path != '']
 
         print("Read Only: ", context.reasoning_result.read_only)
         print("To Change: ", files_to_change)
 
         read_code_w_line_numbers = {path: data.code for path, data in file_context.file_glob.items() if path in context.reasoning_result.read_only}
```

### Comparing `devon_agent-0.0.6/devon_agent/agent/kernel/thread.py` & `devon_agent-0.0.7/devon_agent/agent/kernel/thread.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/reasoning/reason.py` & `devon_agent-0.0.7/devon_agent/agent/reasoning/reason.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/file_system/fs.py` & `devon_agent-0.0.7/devon_agent/agent/tools/file_system/fs.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/file_system/test_fs_tool.py` & `devon_agent-0.0.7/devon_agent/agent/tools/file_system/test_fs_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/git_tool/git_tool.py` & `devon_agent-0.0.7/devon_agent/agent/tools/git_tool/git_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/git_tool/test_git_tool.py` & `devon_agent-0.0.7/devon_agent/agent/tools/git_tool/test_git_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/github/github_tool.py` & `devon_agent-0.0.7/devon_agent/agent/tools/github/github_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/github/test_github_tool.py` & `devon_agent-0.0.7/devon_agent/agent/tools/github/test_github_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/tool_prompts.py` & `devon_agent-0.0.7/devon_agent/agent/tools/tool_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/create_diff.py` & `devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/create_diff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/diff_types.py` & `devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/diff_types.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py` & `devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py` & `devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/agent/tools/unified_diff/utils.py` & `devon_agent-0.0.7/devon_agent/agent/tools/unified_diff/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/format.py` & `devon_agent-0.0.7/devon_agent/format.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/main.py` & `devon_agent-0.0.7/devon_agent/main.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/sandbox/environments.py` & `devon_agent-0.0.7/devon_agent/sandbox/environments.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/sandbox/tool_proxy.py` & `devon_agent-0.0.7/devon_agent/sandbox/tool_proxy.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/tests/state_functions.py` & `devon_agent-0.0.7/devon_agent/tests/state_functions.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/devon_agent/tests/test_diff.py` & `devon_agent-0.0.7/devon_agent/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.6/pyproject.toml` & `devon_agent-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 package-mode = true
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `devon_agent-0.0.6/PKG-INFO` & `devon_agent-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

