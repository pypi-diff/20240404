# Comparing `tmp/devon_agent-0.0.1.tar.gz` & `tmp/devon_agent-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.0.1.tar", max compression
+gzip compressed data, was "devon_agent-0.0.2.tar", max compression
```

## Comparing `devon_agent-0.0.1.tar` & `devon_agent-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,46 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.1/LICENSE
--rw-r--r--   0        0        0     4300 2024-04-02 19:22:29.166470 devon_agent-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.915273 devon_agent-0.0.1/devon_agent/PROMPT
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.1/devon_agent/agent/__init__.py
--rw-r--r--   0        0        0      144 2024-03-29 20:52:18.518610 devon_agent-0.0.1/devon_agent/agent/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4918 2024-03-29 20:52:18.521455 devon_agent-0.0.1/devon_agent/agent/clients/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0     5372 2024-03-29 20:51:48.587225 devon_agent-0.0.1/devon_agent/agent/clients/client.py
--rw-r--r--   0        0        0     1375 2024-03-29 20:47:19.808870 devon_agent-0.0.1/devon_agent/agent/clients/test_function_client.py
--rw-r--r--   0        0        0     4360 2024-03-29 20:52:19.236559 devon_agent-0.0.1/devon_agent/agent/clients/tool_utils/__pycache__/tools.cpython-310.pyc
--rw-r--r--   0        0        0     5797 2024-03-29 20:47:19.809166 devon_agent-0.0.1/devon_agent/agent/clients/tool_utils/tools.py
--rw-r--r--   0        0        0     1145 2024-03-29 20:47:19.809397 devon_agent-0.0.1/devon_agent/agent/evaluate/evaluate.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923712 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/state.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923691 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/state_machine.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923667 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/state_types.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923816 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/states/evaluate.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923791 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/states/execute.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923738 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/states/reason.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923841 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/states/terminate.py
--rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923765 devon_agent-0.0.1/devon_agent/agent/kernel/state_machine/states/write.py
--rw-r--r--   0        0        0     7842 2024-03-29 20:47:19.810853 devon_agent-0.0.1/devon_agent/agent/kernel/thread.py
--rw-r--r--   0        0        0     1957 2024-03-29 20:47:19.811101 devon_agent-0.0.1/devon_agent/agent/reasoning/reason.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.1/devon_agent/agent/tools/__init__.py
--rw-r--r--   0        0        0      150 2024-03-29 20:52:18.518974 devon_agent-0.0.1/devon_agent/agent/tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6130 2024-03-29 20:47:19.811474 devon_agent-0.0.1/devon_agent/agent/tools/file_system/fs.py
--rw-r--r--   0        0        0     2240 2024-03-29 20:47:19.811690 devon_agent-0.0.1/devon_agent/agent/tools/file_system/test_fs_tool.py
--rw-r--r--   0        0        0     3435 2024-03-29 20:47:19.811958 devon_agent-0.0.1/devon_agent/agent/tools/git_tool/git_tool.py
--rw-r--r--   0        0        0     1989 2024-03-29 20:47:19.812172 devon_agent-0.0.1/devon_agent/agent/tools/git_tool/test_git_tool.py
--rw-r--r--   0        0        0     2175 2024-03-29 20:47:19.812382 devon_agent-0.0.1/devon_agent/agent/tools/github/github_tool.py
--rw-r--r--   0        0        0     2894 2024-03-29 20:47:19.812588 devon_agent-0.0.1/devon_agent/agent/tools/github/test_github_tool.py
--rw-r--r--   0        0        0     4709 2024-03-29 20:52:18.520356 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/__pycache__/create_diff.cpython-310.pyc
--rw-r--r--   0        0        0     1692 2024-03-29 20:52:19.333606 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/__pycache__/diff_types.cpython-310.pyc
--rw-r--r--   0        0        0     6418 2024-03-29 20:51:48.565799 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/create_diff.py
--rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/diff_types.py
--rw-r--r--   0        0        0      645 2024-03-29 20:52:19.341330 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/prompts/__pycache__/base_prompts.cpython-310.pyc
--rw-r--r--   0        0        0     9524 2024-03-29 20:52:19.340941 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/prompts/__pycache__/udiff_prompts.cpython-310.pyc
--rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
--rw-r--r--   0        0        0     9275 2024-03-29 20:51:48.576747 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
--rw-r--r--   0        0        0     1785 2024-03-29 20:47:19.813973 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
--rw-r--r--   0        0        0    12099 2024-03-29 20:51:48.566668 devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/utils.py
--rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.1/devon_agent/format.py
--rw-r--r--   0        0        0      881 2024-03-29 20:47:19.814444 devon_agent-0.0.1/devon_agent/main.py
--rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.1/devon_agent/run.txt
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.1/devon_agent/sandbox/__init__.py
--rw-r--r--   0        0        0     1589 2024-03-29 20:47:19.814941 devon_agent-0.0.1/devon_agent/sandbox/environments.py
--rw-r--r--   0        0        0      928 2024-03-29 20:47:19.815099 devon_agent-0.0.1/devon_agent/sandbox/tool_proxy.py
--rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.1/devon_agent/tests/__init__.py
--rw-r--r--   0        0        0     6177 2024-03-29 20:47:19.815436 devon_agent-0.0.1/devon_agent/tests/state_functions.py
--rw-r--r--   0        0        0     1876 2024-03-29 20:47:19.815606 devon_agent-0.0.1/devon_agent/tests/test_diff.py
--rw-r--r--   0        0        0      665 2024-04-03 17:16:20.900469 devon_agent-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5345 1970-01-01 00:00:00.000000 devon_agent-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1371 2024-04-04 01:01:24.013453 devon_agent-0.0.2/README.md
+-rw-r--r--   0        0        0       33 2024-04-04 01:51:19.233672 devon_agent-0.0.2/devon_agent/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.808339 devon_agent-0.0.2/devon_agent/agent/__init__.py
+-rw-r--r--   0        0        0     5372 2024-04-03 18:52:22.966981 devon_agent-0.0.2/devon_agent/agent/clients/client.py
+-rw-r--r--   0        0        0     1375 2024-03-29 20:47:19.808870 devon_agent-0.0.2/devon_agent/agent/clients/test_function_client.py
+-rw-r--r--   0        0        0     5841 2024-04-03 19:09:08.726418 devon_agent-0.0.2/devon_agent/agent/clients/tool_utils/tools.py
+-rw-r--r--   0        0        0     1538 2024-04-03 17:56:50.209221 devon_agent-0.0.2/devon_agent/agent/evaluate/evaluate.py
+-rw-r--r--   0        0        0      855 2024-04-03 17:56:50.209384 devon_agent-0.0.2/devon_agent/agent/kernel/context.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:52:34.923627 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-03 17:56:50.209560 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/state.py
+-rw-r--r--   0        0        0      765 2024-04-03 17:56:50.209735 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/state_machine.py
+-rw-r--r--   0        0        0       99 2024-04-03 18:52:22.940462 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/state_types.py
+-rw-r--r--   0        0        0     1744 2024-04-03 17:56:50.210066 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/evaluate.py
+-rw-r--r--   0        0        0     1986 2024-04-04 01:02:20.668746 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/reason.py
+-rw-r--r--   0        0        0      143 2024-04-03 17:56:50.210535 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/terminate.py
+-rw-r--r--   0        0        0     1784 2024-04-03 19:12:43.542087 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/tool.py
+-rw-r--r--   0        0        0     2738 2024-04-03 17:56:50.210677 devon_agent-0.0.2/devon_agent/agent/kernel/state_machine/states/write.py
+-rw-r--r--   0        0        0     5697 2024-04-04 01:02:20.669219 devon_agent-0.0.2/devon_agent/agent/kernel/thread.py
+-rw-r--r--   0        0        0     2204 2024-04-03 17:56:50.211212 devon_agent-0.0.2/devon_agent/agent/reasoning/reason.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.811178 devon_agent-0.0.2/devon_agent/agent/tools/__init__.py
+-rw-r--r--   0        0        0     6283 2024-04-03 18:52:22.941743 devon_agent-0.0.2/devon_agent/agent/tools/file_system/fs.py
+-rw-r--r--   0        0        0     2240 2024-03-29 20:47:19.811690 devon_agent-0.0.2/devon_agent/agent/tools/file_system/test_fs_tool.py
+-rw-r--r--   0        0        0     5141 2024-04-03 18:52:22.942343 devon_agent-0.0.2/devon_agent/agent/tools/git_tool/git_tool.py
+-rw-r--r--   0        0        0     1989 2024-03-29 20:47:19.812172 devon_agent-0.0.2/devon_agent/agent/tools/git_tool/test_git_tool.py
+-rw-r--r--   0        0        0     4333 2024-04-03 19:14:07.614040 devon_agent-0.0.2/devon_agent/agent/tools/github/github_tool.py
+-rw-r--r--   0        0        0     2894 2024-03-29 20:47:19.812588 devon_agent-0.0.2/devon_agent/agent/tools/github/test_github_tool.py
+-rw-r--r--   0        0        0     1109 2024-04-03 18:52:22.942950 devon_agent-0.0.2/devon_agent/agent/tools/tool_prompts.py
+-rw-r--r--   0        0        0     6614 2024-04-03 17:56:50.211870 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/create_diff.py
+-rw-r--r--   0        0        0      730 2024-03-29 20:47:19.813079 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/diff_types.py
+-rw-r--r--   0        0        0      339 2024-03-29 20:47:19.813455 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/base_prompts.py
+-rw-r--r--   0        0        0     9283 2024-04-04 01:02:20.669812 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py
+-rw-r--r--   0        0        0     1785 2024-03-29 20:47:19.813973 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py
+-rw-r--r--   0        0        0     8227 2024-04-03 18:52:22.943827 devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/utils.py
+-rw-r--r--   0        0        0      829 2024-03-29 20:47:19.814273 devon_agent-0.0.2/devon_agent/format.py
+-rw-r--r--   0        0        0     1077 2024-04-03 18:52:20.747624 devon_agent-0.0.2/devon_agent/main.py
+-rw-r--r--   0        0        0        3 2024-04-04 01:08:16.443671 devon_agent-0.0.2/devon_agent/react.py
+-rw-r--r--   0        0        0      173 2024-03-29 20:47:19.814658 devon_agent-0.0.2/devon_agent/run.txt
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.814724 devon_agent-0.0.2/devon_agent/sandbox/__init__.py
+-rw-r--r--   0        0        0     1589 2024-03-29 20:47:19.814941 devon_agent-0.0.2/devon_agent/sandbox/environments.py
+-rw-r--r--   0        0        0      928 2024-03-29 20:47:19.815099 devon_agent-0.0.2/devon_agent/sandbox/tool_proxy.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:47:19.815170 devon_agent-0.0.2/devon_agent/tests/__init__.py
+-rw-r--r--   0        0        0     6177 2024-03-29 20:47:19.815436 devon_agent-0.0.2/devon_agent/tests/state_functions.py
+-rw-r--r--   0        0        0     1876 2024-03-29 20:47:19.815606 devon_agent-0.0.2/devon_agent/tests/test_diff.py
+-rw-r--r--   0        0        0      665 2024-04-04 01:51:49.611979 devon_agent-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 devon_agent-0.0.2/PKG-INFO
```

### Comparing `devon_agent-0.0.1/LICENSE` & `devon_agent-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/agent/clients/client.py` & `devon_agent-0.0.2/devon_agent/agent/clients/client.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/agent/clients/test_function_client.py` & `devon_agent-0.0.2/devon_agent/agent/clients/test_function_client.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/agent/clients/tool_utils/tools.py` & `devon_agent-0.0.2/devon_agent/agent/clients/tool_utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from pydantic import BaseModel, Field
 from pydantic.fields import FieldInfo
 import xml.etree.ElementTree as ET
 from typing import Callable, Dict, Any, List, get_type_hints
 import json
 import inspect
 
-client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
-
 def tool(name: str, description: str):
     def decorator(func):
         func.tool_name = name
         func.tool_description = description
         return func
     return decorator
 
@@ -149,16 +147,18 @@
                 if isinstance(param.default, FieldInfo) and param.default.default != ...
             }
 
             # Update the function arguments with default values if not provided
             for param_name, default_value in default_values.items():
                 if param_name not in function_args:
                     function_args[param_name] = default_value
-
-            function_response = function_to_call(**function_args)
+            try:
+                function_response = function_to_call(**function_args)
+            except Exception as e:
+                function_response = str(e)
             results.append(
                 {
                     "tool_call_id": tool_call.id,
                     "role": "function",
                     "name": function_name,
                     "content": function_response,
                 }
```

### Comparing `devon_agent-0.0.1/devon_agent/agent/reasoning/reason.py` & `devon_agent-0.0.2/devon_agent/agent/reasoning/reason.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 If a file already exists you do not need to create it.
 </SCRATCHPAD>
 <PLAN>
 Your plan
 </PLAN>
 <FILES>
+<READONLY>
+files that are needed but unchanged...
+</READONLY>
 <CREATE>
 files to create... (Do not create files that already exist in the code base)
 </CREATE>
 <MODIFY>
 files to modify...
 </MODIFY>
 <DELETE>
@@ -46,19 +49,23 @@
         files = output.split("<FILES>")[1].split("</FILES>")
 
         create = None
         modify = None
         delete = None
 
         files_to_edit = []
+        read_only = []
 
+        if "<READONLY>" in output:
+            read = output.split("<READONLY>")[1].split("</READONLY>")[0].splitlines()
+            read_only += read
         if "<CREATE>" in output:
             create = output.split("<CREATE>")[1].split("</CREATE>")[0].splitlines()
             files_to_edit += create
         if "<MODIFY>" in output:
             modify = output.split("<MODIFY>")[1].split("</MODIFY>")[0].splitlines()
             files_to_edit += modify
         if "<DELETE>" in output:
             delete = output.split("<DELETE>")[1].split("</DELETE>")[0].splitlines()
             files_to_edit += delete
 
-        return plan, create, modify, delete, files_to_edit
+        return plan, create, modify, delete, files_to_edit, read_only
```

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/file_system/fs.py` & `devon_agent-0.0.2/devon_agent/agent/tools/file_system/fs.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
             raise ValueError(f"Path does not exist: {full_path}")
 
         def build_tree(current_path):
             entries = {}
             for entry in os.listdir(current_path):
                 entry_path = os.path.join(current_path, entry)
                 relative_path = os.path.relpath(entry_path, self.base_path)
+                if os.path.basename(relative_path)[0] == ".":
+                    continue
                 if os.path.isfile(entry_path):
                     entries[entry] = {
                         "type": "file",
                         "path": relative_path
                     }
                 else:
                     entries[entry] = {
@@ -89,15 +91,16 @@
         with open(full_path, 'a'):
             os.utime(full_path, None)
         return f"File created: {full_path}"
     
     @tool("mkdir", "Create a new directory")
     def mkdir(self, path: str = Field(..., description="The directory path")):
         full_path = os.path.join(self.base_path, path)
-        os.makedirs(os.path.dirname(full_path), exist_ok=True)
+        os.makedirs(full_path, exist_ok=True)
+        print(full_path)
         return f"Directory created: {full_path}"
 
     def read_file(self, path):
         with open(path, "r") as f:
             content = f.read()
         
         return content
@@ -106,15 +109,15 @@
         if not os.path.isdir(path):
             raise NotADirectoryError(f"{path} is not a directory")
         
         dirs = []
         files = []
 
         for entry in os.listdir(path):
-            print(entry)
+            # print(entry)
             entry = os.path.join(path, entry)
             if os.path.isfile(entry):
                 files.append(entry)
             elif os.path.isdir(entry):
                 dirs.append(entry)
         
         return dirs, files
@@ -143,9 +146,11 @@
                     code, code_with_lines = self.get_code_from_file(full_path)
                     if code is not None and code != "":
                         files[full_path] = CodeFile(filepath=full_path, code=code, code_with_lines=code_with_lines, raw=code)
             for directory in dirs:
                 if not directory.startswith('.'):  # Avoid hidden directories
                     extract_code_recursive(os.path.join(path, directory))
 
+        # print(path)
         extract_code_recursive(path)
+        # print(files.keys())
         return files
```

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/file_system/test_fs_tool.py` & `devon_agent-0.0.2/devon_agent/agent/tools/file_system/test_fs_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/git_tool/git_tool.py` & `devon_agent-0.0.2/devon_agent/agent/tools/git_tool/git_tool.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 from git import Repo
 from typing import List
 from pydantic import Field
 from devon.agent.clients.tool_utils.tools import tool
 
 class GitTool:
 
-    def __init__(self, path="."):
-        self.repo = Repo(path=path)
-
     @tool(name="git_create_repo", description="Clone a Git repository")
     def init_new_repo(self, path: str = Field(..., description="The path to the Git repository")):
-        self.repo = Repo(path)
+        self.repo = Repo.init(path)
         return {"result": f"Git repo at {path}"}
 
     @tool(name="git_clone", description="Clone a Git repository")
     def clone(self, url: str = Field(..., description="The URL of the Git repository to clone"),
               path: str = Field(..., description="The path where the cloned repository will be stored")):
         print("pulling: ", url)
         self.repo = Repo.clone_from(url, path)
@@ -61,8 +58,42 @@
                 self.repo.index.add(file_path)
             except:
                 self.repo.index.add(path.join(getcwd(),file_path))
 
         # Create the commit
         commit = self.repo.index.commit(message)
 
-        return {"result": f"Successfully created commit '{commit.hexsha}' with message '{message}'"}
+        return {"result": f"Successfully created commit '{commit.hexsha}' with message '{message}'"}
+
+    @tool(name="git_add_remote", description="Add a remote to a Git repository")
+    def add_remote(self, name: str = Field(..., description="The name of the remote"),
+                   url: str = Field(..., description="The URL of the remote")):
+        self.repo.create_remote(name, url)
+        return {"result": f"Successfully added remote '{name}' with URL '{url}'"}
+
+    @tool(name="git_remove_remote", description="Remove a remote from a Git repository")
+    def remove_remote(self, name: str = Field(..., description="The name of the remote to remove")):
+        remote = self.repo.remote(name)
+        remote.remove(self.repo, name)
+        return {"result": f"Successfully removed remote '{name}'"}
+
+    @tool(name="git_list_remotes", description="List the remotes of a Git repository")
+    def list_remotes(self):
+        remotes = []
+        for remote in self.repo.remotes:
+            remotes.append({"name": remote.name, "url": remote.url})
+        return remotes
+
+    @tool(name="git_push", description="Push changes to a remote repository")
+    def push(
+            self,
+            remote: str = Field(..., description="The name of the remote"),
+            branch: str = Field(..., description="The branch to push")
+        ):
+        self.repo.remote(remote).push(branch)
+        return {"result": f"Successfully pushed branch '{branch}' to remote '{remote}'"}
+
+    @tool(name="git_pull", description="Pull changes from a remote repository")
+    def pull(self, remote: str = Field(..., description="The name of the remote"),
+             branch: str = Field(..., description="The branch to pull")):
+        self.repo.remote(remote).pull(branch)
+        return {"result": f"Successfully pulled changes from branch '{branch}' of remote '{remote}'"}
```

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/git_tool/test_git_tool.py` & `devon_agent-0.0.2/devon_agent/agent/tools/git_tool/test_git_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/github/github_tool.py` & `devon_agent-0.0.2/devon_agent/agent/tools/github/github_tool.py`

 * *Files 26% similar despite different names*

```diff
@@ -44,7 +44,61 @@
             "body": body,
             "head": head,
             "base": base
         }
         response = requests.post(f"https://api.github.com/repos/{repo}/pulls", json=data, headers=headers)
         response.raise_for_status()
         return response.json()["html_url"]
+    
+    @tool(
+        name="create_repository",
+        description="Create a new repository",
+    )
+    def create_repository(
+        self,
+        name: str = Field(..., description="The name of the repository"),
+        description: str = Field(None, description="The description of the repository")
+    ) -> str:
+        headers = {"Authorization": f"token {self.token}"}
+        data = {
+            "name": name,
+            "description": description
+        }
+        try:
+            response = requests.post("https://api.github.com/user/repos", json=data, headers=headers)
+            response.raise_for_status()
+            return response.json()["html_url"]
+        except requests.exceptions.HTTPError as e:
+            raise e
+            if e.response.status_code == 403:
+                raise ValueError("Insufficient permissions to create a repository. Please check your access token.")
+            else:
+                raise e
+    
+    @tool(
+        name="enable_github_pages",
+        description="Enable GitHub Pages for a repository",
+    )
+    def enable_github_pages(
+        self,
+        owner: str = Field(..., description="The user/owner name"),
+        repo: str = Field(..., description="The repository name"),
+        branch: str = Field("main", description="The branch to use for GitHub Pages"),
+        path: str = Field("/", description="The path to the GitHub Pages files")
+    ) -> None:
+        headers = {"Authorization": f"token {self.token}"}
+        data = {
+            "source": {
+                "branch": branch,
+                "path": path
+            }
+        }
+        try:
+            response = requests.post(f"https://api.github.com/repos/{owner}/{repo}/pages", json=data, headers=headers)
+            response.raise_for_status()
+            print(f"GitHub Pages enabled for repository: {repo}")
+        except requests.exceptions.HTTPError as e:
+            raise e
+            if e.response.status_code == 403:
+                raise ValueError("Insufficient permissions to enable GitHub Pages. Please check your access token.")
+            else:
+                return {"result": e.response.reason}
```

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/github/test_github_tool.py` & `devon_agent-0.0.2/devon_agent/agent/tools/github/test_github_tool.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/create_diff.py` & `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/create_diff.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,55 +5,55 @@
 import dotenv
 import re
 
 from devon.agent.tools.unified_diff.prompts.udiff_prompts import UnifiedDiffPrompts
 
 dotenv.load_dotenv()
 
-def parse_multi_file_diff(diff: str) -> MultiFileDiff:
-    file_diffs = []
-    lines = diff.strip().split("\n")
+# def parse_multi_file_diff(diff: str) -> MultiFileDiff:
+#     file_diffs = []
+#     lines = diff.strip().split("\n")
     
-    i = 0
-    while i < len(lines):
-        if lines[i].startswith("---"):
-            src_file = re.findall(r"--- (.*)", lines[i])[0]
-            tgt_file = re.findall(r"\+\+\+ (.*)", lines[i+1])[0]
-            hunks = []
-            i += 2
+#     i = 0
+#     while i < len(lines):
+#         if lines[i].startswith("---"):
+#             src_file = re.findall(r"--- (.*)", lines[i])[0]
+#             tgt_file = re.findall(r"\+\+\+ (.*)", lines[i+1])[0]
+#             hunks = []
+#             i += 2
             
-            while i < len(lines) and not lines[i].startswith("---"):
-                if lines[i].startswith("@@"):
-                    hunk_lines = []
-                    match = re.findall(r"@@ -(\d+),(\d+) \+(\d+),(\d+) @@", lines[i])
-                    if len(match) == 0:
-                        match = re.findall(r"@@ -(\d+),(\d+) \+(\d+) @@", lines[i]) + ["1"]
+#             while i < len(lines) and not lines[i].startswith("---"):
+#                 if lines[i].startswith("@@"):
+#                     hunk_lines = []
+#                     match = re.findall(r"@@ -(\d+),(\d+) \+(\d+),(\d+) @@", lines[i])
+#                     if len(match) == 0:
+#                         match = re.findall(r"@@ -(\d+),(\d+) \+(\d+) @@", lines[i]) + ["1"]
                     
-                    match = match[0]
-                    src_start, src_lines, tgt_start, tgt_lines = map(int, match)
-                    i += 1
+#                     match = match[0]
+#                     src_start, src_lines, tgt_start, tgt_lines = map(int, match)
+#                     i += 1
                     
-                    while i < len(lines) and not lines[i].startswith("@@") and not lines[i].startswith("---"):
-                        if lines[i].startswith("-"):
-                            hunk_lines.append(HunkLine(type="removed", content=lines[i][1:]))
-                        elif lines[i].startswith("+"):
-                            hunk_lines.append(HunkLine(type="added", content=lines[i][1:]))
-                        else:
-                            hunk_lines.append(HunkLine(type="unchanged", content=lines[i][1:]))
-                        i += 1
+#                     while i < len(lines) and not lines[i].startswith("@@") and not lines[i].startswith("---"):
+#                         if lines[i].startswith("-"):
+#                             hunk_lines.append(HunkLine(type="removed", content=lines[i][1:]))
+#                         elif lines[i].startswith("+"):
+#                             hunk_lines.append(HunkLine(type="added", content=lines[i][1:]))
+#                         else:
+#                             hunk_lines.append(HunkLine(type="unchanged", content=lines[i][1:]))
+#                         i += 1
                     
-                    hunks.append(Hunk(src_start=src_start, src_lines=src_lines, tgt_start=tgt_start, tgt_lines=tgt_lines, lines=hunk_lines))
-                else:
-                    i += 1
+#                     hunks.append(Hunk(src_start=src_start, src_lines=src_lines, tgt_start=tgt_start, tgt_lines=tgt_lines, lines=hunk_lines))
+#                 else:
+#                     i += 1
             
-            file_diffs.append(FileDiff(src_file=src_file, tgt_file=tgt_file, hunks=hunks))
-        else:
-            i += 1
+#             file_diffs.append(FileDiff(src_file=src_file, tgt_file=tgt_file, hunks=hunks))
+#         else:
+#             i += 1
     
-    return file_diffs
+#     return file_diffs
 
 def parse_multi_file_diff2(diff: str) -> MultiFileDiff:
     file_diffs = []
     lines = diff.strip().split("\n")
     
     i = 0
     while i < len(lines):
@@ -118,20 +118,20 @@
             new_lines.append(line.content)
         else:
             old_lines.append(line.content)
             new_lines.append(line.content)
 
     return old_lines, new_lines
 
-def generate_unified_diff2(client, goal, original_code, plan, create, modify, delete, failure_context, file_tree):
+def generate_unified_diff2(client, goal, read_only_code, original_code, plan, create, modify, delete, failure_context, file_tree):
 
     res = client.chat([
         Message(
             role="user",
-            content=format_diff_input(goal, original_code, plan, create, modify, delete, failure_context, file_tree)
+            content=format_diff_input(goal, read_only_code, original_code, plan, create, modify, delete, failure_context, file_tree)
         )
     ])
 
     print(res)
 
     diffs = extract_diffs(res)
 
@@ -140,61 +140,64 @@
         file_diffs = parse_multi_file_diff2(diff)
         all_diffs.extend(file_diffs)
 
     changes = MultiFileDiff2(files=all_diffs)
 
     return changes
 
-def find_line_numbers(lines, line1, line2):
-    for index in range(len(lines) - 1):
-        if lines[index].strip() == line1.strip():
-            return index + 1
+# def find_line_numbers(lines, line1, line2):
+#     for index in range(len(lines) - 1):
+#         if lines[index].strip() == line1.strip():
+#             return index + 1
 
-    return None
+#     return None
 
 def extract_diffs(diff_text):
     return [diff.replace("<DIFF>", "").strip() for diff in diff_text.split("</DIFF>")[:-1] if "<DIFF>" in diff]
 
-def format_diff_input(goal, code, plan, create, modify, delete, failure_context, file_tree):
+def format_diff_input(goal, read_only_code, code, plan, create, modify, delete, failure_context, file_tree):
     return f"""
 <GOAL>
 {goal}
 </GOAL>
 <CODE>
 {code}
 </CODE>
 <FILE_TREE>
 {file_tree}
 </FILE_TREE>
+<READ_ONLY>
+{read_only_code}
+</READ_ONLY>
 <PLAN>
 {plan}
 </PLAN>
 <CREATE>
 {create}
 </CREATE>
 <MODIFY>
 {modify}
 </MODIFY>
 <DELETE>
 {delete}
 </DELETE>
 """
 
-def generate_unified_diff(client, goal, original_code, plan, create, modify, delete, failure_context, file_tree):
+# def generate_unified_diff(client, goal, original_code, plan, create, modify, delete, failure_context, file_tree):
 
-    res = client.chat([
-        Message(
-            role="user",
-            content=format_diff_input(goal, original_code, plan, create, modify, delete, failure_context, file_tree)
-        )
-    ])
+#     res = client.chat([
+#         Message(
+#             role="user",
+#             content=format_diff_input(goal, original_code, plan, create, modify, delete, failure_context, file_tree)
+#         )
+#     ])
 
-    diffs = extract_diffs(res)
+#     diffs = extract_diffs(res)
 
-    all_diffs = []
-    for diff in diffs:
-        file_diffs = parse_multi_file_diff(diff)
-        all_diffs.extend(file_diffs)
+#     all_diffs = []
+#     for diff in diffs:
+#         file_diffs = parse_multi_file_diff(diff)
+#         all_diffs.extend(file_diffs)
 
-    changes = MultiFileDiff(files=all_diffs)
+#     changes = MultiFileDiff(files=all_diffs)
 
-    return changes
+#     return changes
```

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/diff_types.py` & `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/diff_types.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/prompts/__pycache__/udiff_prompts.cpython-310.pyc` & `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/udiff_prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,596 +1,581 @@
-00000000: 6f0d 0d0a 0000 0000 e429 0766 3b24 0000  o........).f;$..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
-00000030: 6401 6c00 6d01 5a01 0100 6402 5a02 4700  d.l.m.Z...d.Z.G.
-00000040: 6403 6404 8400 6404 6501 8303 5a03 6405  d.d...d.e...Z.d.
-00000050: 5300 2906 e901 0000 0029 01da 0c43 6f64  S.)......)...Cod
-00000060: 6572 5072 6f6d 7074 737a 053c 454e 443e  erPromptsz.<END>
-00000070: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000080: 0003 0000 0040 0000 0073 3000 0000 6500  .....@...s0...e.
-00000090: 5a01 6400 5a02 6401 6503 9b00 6402 9d03  Z.d.Z.d.e...d...
-000000a0: 5a04 6403 6503 9b00 6404 9d03 5a05 6405  Z.d.e...d...Z.d.
-000000b0: 5a06 6406 5a07 6407 5a08 6408 5300 2909  Z.d.Z.d.Z.d.S.).
-000000c0: da12 556e 6966 6965 6444 6966 6650 726f  ..UnifiedDiffPro
-000000d0: 6d70 7473 61ea 1600 0041 6374 2061 7320  mptsa....Act as 
-000000e0: 616e 2065 7870 6572 7420 736f 6674 7761  an expert softwa
-000000f0: 7265 2064 6576 656c 6f70 6572 2e0a 0a41  re developer...A
-00000100: 7320 6120 7365 6173 6f6e 6564 2065 6e67  s a seasoned eng
-00000110: 696e 6565 7220 796f 750a 312e 2059 6f75  ineer you.1. You
-00000120: 204e 4556 4552 206c 6561 7665 2063 6f6d   NEVER leave com
-00000130: 6d65 6e74 7320 6465 7363 7269 6269 6e67  ments describing
-00000140: 2063 6f64 6520 7769 7468 6f75 7420 696d   code without im
-00000150: 706c 656d 656e 7469 6e67 2069 7421 200a  plementing it! .
-00000160: 322e 2059 6f75 2061 6c77 6179 7320 434f  2. You always CO
-00000170: 4d50 4c45 5445 4c59 2049 4d50 4c45 4d45  MPLETELY IMPLEME
-00000180: 4e54 2074 6865 206e 6565 6465 6420 636f  NT the needed co
-00000190: 6465 210a 332e 2041 6c77 6179 7320 7573  de!.3. Always us
-000001a0: 6520 6265 7374 2070 7261 6374 6963 6573  e best practices
-000001b0: 2077 6865 6e20 636f 6469 6e67 2e0a 342e   when coding..4.
-000001c0: 2052 6573 7065 6374 2061 6e64 2075 7365   Respect and use
-000001d0: 2065 7869 7374 696e 6720 636f 6e76 656e   existing conven
-000001e0: 7469 6f6e 732c 206c 6962 7261 7269 6573  tions, libraries
-000001f0: 2c20 6574 6320 7468 6174 2061 7265 2061  , etc that are a
-00000200: 6c72 6561 6479 2070 7265 7365 6e74 2069  lready present i
-00000210: 6e20 7468 6520 636f 6465 2062 6173 652e  n the code base.
-00000220: 0a35 2e20 436f 6d6d 656e 7420 636f 6465  .5. Comment code
-00000230: 2077 6974 6820 6465 7363 7269 7074 696f   with descriptio
-00000240: 6e73 0a0a 5461 6b65 2072 6571 7565 7374  ns..Take request
-00000250: 7320 666f 7220 6368 616e 6765 7320 746f  s for changes to
-00000260: 2074 6865 2073 7570 706c 6965 6420 636f   the supplied co
-00000270: 6465 2e0a 4966 2074 6865 2072 6571 7565  de..If the reque
-00000280: 7374 2069 7320 616d 6269 6775 6f75 732c  st is ambiguous,
-00000290: 2061 736b 2071 7565 7374 696f 6e73 2e0a   ask questions..
-000002a0: 0a46 6f72 2065 6163 6820 6669 6c65 2074  .For each file t
-000002b0: 6861 7420 6e65 6564 7320 746f 2062 6520  hat needs to be 
-000002c0: 6368 616e 6765 642c 2077 7269 7465 206f  changed, write o
-000002d0: 7574 2074 6865 2063 6861 6e67 6573 2073  ut the changes s
-000002e0: 696d 696c 6172 2074 6f20 6120 756e 6966  imilar to a unif
-000002f0: 6965 6420 6469 6666 206c 696b 6520 6064  ied diff like `d
-00000300: 6966 6620 2d55 3060 2077 6f75 6c64 2070  iff -U0` would p
-00000310: 726f 6475 6365 2e20 5772 6170 2079 6f75  roduce. Wrap you
-00000320: 7220 6469 6666 7320 7769 7474 6820 3c44  r diffs witth <D
-00000330: 4946 463e 2061 6e64 203c 2f44 4946 463e  IFF> and </DIFF>
-00000340: 2e0a 0a59 6f75 2077 696c 6c20 6265 2067  ...You will be g
-00000350: 6976 656e 2061 203c 504c 414e 3e20 636f  iven a <PLAN> co
-00000360: 6e74 6169 6e69 6e67 2068 6967 6820 6c65  ntaining high le
-00000370: 7665 6c20 6465 7363 7269 7074 696f 6e20  vel description 
-00000380: 6f66 2063 6861 6e67 6573 2072 6571 7569  of changes requi
-00000390: 7265 6420 616e 6420 3c46 494c 4553 3e20  red and <FILES> 
-000003a0: 636f 6e74 6169 6e69 6e67 203a 0a3c 4352  containing :.<CR
-000003b0: 4541 5445 3e20 3a20 7769 6c6c 2068 6176  EATE> : will hav
-000003c0: 6520 6669 6c65 7320 7468 6174 2061 7265  e files that are
-000003d0: 2074 6f20 6265 2063 7265 6174 6564 0a3c   to be created.<
-000003e0: 4d4f 4449 4659 3e20 3a20 6669 6c65 7320  MODIFY> : files 
-000003f0: 7468 6174 206e 6565 6420 746f 2062 6520  that need to be 
-00000400: 6d6f 6469 6669 6564 0a3c 4445 4c45 5445  modified.<DELETE
-00000410: 3e20 3a20 6669 6c65 7320 7468 6174 206e  > : files that n
-00000420: 6565 6420 746f 2062 6520 6465 6c65 7465  eed to be delete
-00000430: 640a 0a59 6f75 2077 696c 6c20 6265 2067  d..You will be g
-00000440: 6976 656e 203c 434f 4445 3e20 636f 6e74  iven <CODE> cont
-00000450: 6169 6e69 6e67 2061 6c6c 2074 6865 2072  aining all the r
-00000460: 656c 6576 616e 7420 636f 6465 0a0a 466f  elevant code..Fo
-00000470: 7220 6578 616d 706c 653a 0a0a 3c45 5841  r example:..<EXA
-00000480: 4d50 4c45 3e0a 3c55 5345 523e 0a52 6570  MPLE>.<USER>.Rep
-00000490: 6c61 6365 2069 735f 7072 696d 6520 7769  lace is_prime wi
-000004a0: 7468 2061 2063 616c 6c20 746f 2073 796d  th a call to sym
-000004b0: 7079 2e0a 3c43 4f44 453e 0a2e 2e2e 206f  py..<CODE>.... o
-000004c0: 7269 6769 6e61 6c20 636f 6465 2067 6f65  riginal code goe
-000004d0: 7320 6865 7265 0a3c 2f43 4f44 453e 0a3c  s here.</CODE>.<
-000004e0: 4649 4c45 5f54 5245 453e 0a2e 2e2e 2074  FILE_TREE>.... t
-000004f0: 6865 2066 696c 6520 7472 6565 2077 696c  he file tree wil
-00000500: 6c20 6265 2068 6572 6520 2e2e 2e0a 3c2f  l be here ....</
-00000510: 4649 4c45 5f54 5245 453e 0a3c 504c 414e  FILE_TREE>.<PLAN
-00000520: 3e0a 312e 204d 616b 6520 7375 7265 2074  >.1. Make sure t
-00000530: 6f20 696d 706f 7274 2073 796d 7079 0a32  o import sympy.2
-00000540: 2e20 5265 706c 6163 6520 7468 6520 6578  . Replace the ex
-00000550: 6973 7469 6e67 2063 616c 6c20 746f 2069  isting call to i
-00000560: 735f 7072 696d 6520 7769 7468 2061 2063  s_prime with a c
-00000570: 616c 6c20 746f 2073 796d 7079 2e69 735f  all to sympy.is_
-00000580: 7072 696d 6528 290a 3c2f 504c 414e 3e0a  prime().</PLAN>.
-00000590: 3c46 494c 4553 3e0a 3c43 5245 4154 453e  <FILES>.<CREATE>
-000005a0: 0a3c 2f43 5245 4154 453e 0a3c 4d4f 4449  .</CREATE>.<MODI
-000005b0: 4659 3e0a 6d61 7468 7765 622f 666c 6173  FY>.mathweb/flas
-000005c0: 6b2f 6170 702e 7079 0a3c 2f4d 4f44 4946  k/app.py.</MODIF
-000005d0: 593e 0a3c 4445 4c45 5445 3e0a 3c2f 4445  Y>.<DELETE>.</DE
-000005e0: 4c45 5445 3e0a 3c2f 4649 4c45 533e 0a3c  LETE>.</FILES>.<
-000005f0: 2f55 5345 523e 0a3c 4153 5349 5354 414e  /USER>.<ASSISTAN
-00000600: 543e 0a4f 6b2c 2049 2077 696c 6c3a 0a0a  T>.Ok, I will:..
-00000610: 312e 2041 6464 2061 6e20 696d 706f 7274  1. Add an import
-00000620: 206f 6620 7379 6d70 792e 0a32 2e20 5265   of sympy..2. Re
-00000630: 6d6f 7665 2074 6865 2069 735f 7072 696d  move the is_prim
-00000640: 6528 2920 6675 6e63 7469 6f6e 2e0a 332e  e() function..3.
-00000650: 2052 6570 6c61 6365 2074 6865 2065 7869   Replace the exi
-00000660: 7374 696e 6720 6361 6c6c 2074 6f20 6973  sting call to is
-00000670: 5f70 7269 6d65 2829 2077 6974 6820 6120  _prime() with a 
-00000680: 6361 6c6c 2074 6f20 7379 6d70 792e 6973  call to sympy.is
-00000690: 7072 696d 6528 292e 0a0a 4865 7265 2061  prime()...Here a
-000006a0: 7265 2074 6865 2064 6966 6673 2066 6f72  re the diffs for
-000006b0: 2074 686f 7365 2063 6861 6e67 6573 3a0a   those changes:.
-000006c0: 3c53 4352 4154 4348 5041 443e 0a2e 2e2e  <SCRATCHPAD>....
-000006d0: 2074 6869 6e6b 696e 6720 7374 6570 2062   thinking step b
-000006e0: 7920 7374 6570 202e 2e2e 0a49 6e20 6d61  y step ....In ma
-000006f0: 7468 7765 622f 666c 6173 6b2f 6170 702e  thweb/flask/app.
-00000700: 7079 2049 206e 6565 6420 746f 2061 6464  py I need to add
-00000710: 2061 6e20 696d 706f 7274 2074 6f20 7379   an import to sy
-00000720: 6d70 792c 2074 6865 6e20 4920 6e65 6564  mpy, then I need
-00000730: 2074 6f20 7265 6d6f 7665 2074 6865 2066   to remove the f
-00000740: 756e 6374 696f 6e20 6973 5f70 7269 6d65  unction is_prime
-00000750: 2e0a 3c2f 5343 5241 5443 4850 4144 3e0a  ..</SCRATCHPAD>.
-00000760: 3c44 4946 463e 0a2d 2d2d 206d 6174 6877  <DIFF>.--- mathw
-00000770: 6562 2f66 6c61 736b 2f61 7070 2e70 790a  eb/flask/app.py.
-00000780: 2b2b 2b20 6d61 7468 7765 622f 666c 6173  +++ mathweb/flas
-00000790: 6b2f 6170 702e 7079 0a40 4020 2e2e 2e20  k/app.py.@@ ... 
-000007a0: 4040 0a2d 636c 6173 7320 4d61 7468 5765  @@.-class MathWe
-000007b0: 623a 0a2b 696d 706f 7274 2073 796d 7079  b:.+import sympy
-000007c0: 0a2b 0a2b 636c 6173 7320 4d61 7468 5765  .+.+class MathWe
-000007d0: 623a 0a40 4020 2e2e 2e20 4040 0a2d 6465  b:.@@ ... @@.-de
-000007e0: 6620 6973 5f70 7269 6d65 2878 293a 0a2d  f is_prime(x):.-
-000007f0: 2020 2020 6966 2078 203c 2032 3a0a 2d20      if x < 2:.- 
-00000800: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00000810: 6c73 650a 2d20 2020 2066 6f72 2069 2069  lse.-    for i i
-00000820: 6e20 7261 6e67 6528 322c 2069 6e74 286d  n range(2, int(m
-00000830: 6174 682e 7371 7274 2878 2929 202b 2031  ath.sqrt(x)) + 1
-00000840: 293a 0a2d 2020 2020 2020 2020 6966 2078  ):.-        if x
-00000850: 2025 2069 203d 3d20 303a 0a2d 2020 2020   % i == 0:.-    
-00000860: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00000870: 616c 7365 0a2d 2020 2020 7265 7475 726e  alse.-    return
-00000880: 2054 7275 650a 3c2f 4449 4646 3e0a 3c44   True.</DIFF>.<D
-00000890: 4946 463e 0a2d 2d2d 206d 6174 6877 6562  IFF>.--- mathweb
-000008a0: 2f66 6c61 736b 2f61 7070 2e70 790a 2b2b  /flask/app.py.++
-000008b0: 2b20 6d61 7468 7765 622f 666c 6173 6b2f  + mathweb/flask/
-000008c0: 6170 702e 7079 0a40 4020 2e2e 2e20 4040  app.py.@@ ... @@
-000008d0: 0a2d 4061 7070 2e72 6f75 7465 2827 2f70  .-@app.route('/p
-000008e0: 7269 6d65 2f3c 696e 743a 6e3e 2729 0a2d  rime/<int:n>').-
-000008f0: 6465 6620 6e74 685f 7072 696d 6528 6e29  def nth_prime(n)
-00000900: 3a0a 2d20 2020 2063 6f75 6e74 203d 2030  :.-    count = 0
-00000910: 0a2d 2020 2020 6e75 6d20 3d20 310a 2d20  .-    num = 1.- 
-00000920: 2020 2077 6869 6c65 2063 6f75 6e74 203c     while count <
-00000930: 206e 3a0a 2d20 2020 2020 2020 206e 756d   n:.-        num
-00000940: 202b 3d20 310a 2d20 2020 2020 2020 2069   += 1.-        i
-00000950: 6620 6973 5f70 7269 6d65 286e 756d 293a  f is_prime(num):
-00000960: 0a2d 2020 2020 2020 2020 2020 2020 636f  .-            co
-00000970: 756e 7420 2b3d 2031 0a2d 2020 2020 7265  unt += 1.-    re
-00000980: 7475 726e 2073 7472 286e 756d 290a 2b40  turn str(num).+@
-00000990: 6170 702e 726f 7574 6528 272f 7072 696d  app.route('/prim
-000009a0: 652f 3c69 6e74 3a6e 3e27 290a 2b64 6566  e/<int:n>').+def
-000009b0: 206e 7468 5f70 7269 6d65 286e 293a 0a2b   nth_prime(n):.+
-000009c0: 2020 2020 636f 756e 7420 3d20 300a 2b20      count = 0.+ 
-000009d0: 2020 206e 756d 203d 2031 0a2b 2020 2020     num = 1.+    
-000009e0: 7768 696c 6520 636f 756e 7420 3c20 6e3a  while count < n:
-000009f0: 0a2b 2020 2020 2020 2020 6e75 6d20 2b3d  .+        num +=
-00000a00: 2031 0a2b 2020 2020 2020 2020 6966 2073   1.+        if s
-00000a10: 796d 7079 2e69 7370 7269 6d65 286e 756d  ympy.isprime(num
-00000a20: 293a 0a2b 2020 2020 2020 2020 2020 2020  ):.+            
-00000a30: 636f 756e 7420 2b3d 2031 0a2b 2020 2020  count += 1.+    
-00000a40: 7265 7475 726e 2073 7472 286e 756d 290a  return str(num).
-00000a50: 3c2f 4449 4646 3e0a 3c41 5353 4953 5354  </DIFF>.<ASSISST
-00000a60: 414e 542f 3e0a 0a46 696c 6520 6564 6974  ANT/>..File edit
-00000a70: 696e 6720 7275 6c65 733a 0a0a 0a57 524f  ing rules:...WRO
-00000a80: 4e47 3a0a 4040 202d 3130 2c31 202b 3130  NG:.@@ -10,1 +10
-00000a90: 2040 4020 636c 6965 6e74 5f69 7020 3d20   @@ client_ip = 
-00000aa0: 2231 3932 2e31 3638 2e32 332e 3130 3422  "192.168.23.104"
-00000ab0: 0a0a 434f 5252 4543 543a 0a2d 2d2d 206d  ..CORRECT:.--- m
-00000ac0: 6174 6877 6562 2f66 6c61 736b 2f61 7070  athweb/flask/app
-00000ad0: 2e70 790a 2b2b 2b20 6d61 7468 7765 622f  .py.+++ mathweb/
-00000ae0: 666c 6173 6b2f 6170 702e 7079 0a40 4020  flask/app.py.@@ 
-00000af0: 2d31 302c 3120 2b31 302c 3120 4040 200a  -10,1 +10,1 @@ .
-00000b00: 636c 6965 6e74 5f69 7020 3d20 2231 3932  client_ip = "192
-00000b10: 2e31 3638 2e32 332e 3130 3422 0a0a 0a57  .168.23.104"...W
-00000b20: 524f 4e47 3a0a 4040 202d 302c 3020 2b31  RONG:.@@ -0,0 +1
-00000b30: 2c37 2040 400a 2b31 3a20 6672 6f6d 2061  ,7 @@.+1: from a
-00000b40: 6765 6e74 2e6b 6572 6e65 6c2e 7374 6174  gent.kernel.stat
-00000b50: 655f 6d61 6368 696e 652e 7374 6174 655f  e_machine.state_
-00000b60: 6d61 6368 696e 6520 696d 706f 7274 2053  machine import S
-00000b70: 7461 7465 0a2b 323a 200a 2b33 3a20 0a2b  tate.+2: .+3: .+
-00000b80: 343a 2063 6c61 7373 2054 6572 6d69 6e61  4: class Termina
-00000b90: 7465 5374 6174 6528 5374 6174 6529 3a0a  teState(State):.
-00000ba0: 2b35 3a20 2020 2020 6465 6620 6578 6563  +5:     def exec
-00000bb0: 7574 6528 7365 6c66 2c20 636f 6e74 6578  ute(self, contex
-00000bc0: 7429 3a0a 2b36 3a20 2020 2020 2020 2020  t):.+6:         
-00000bd0: 2320 496d 706c 656d 656e 7420 7465 726d  # Implement term
-00000be0: 696e 6174 696f 6e20 6c6f 6769 6320 6865  ination logic he
-00000bf0: 7265 0a2b 373a 2020 2020 2020 2020 2070  re.+7:         p
-00000c00: 6173 730a 0a43 4f52 5245 4354 3a0a 2d2d  ass..CORRECT:.--
-00000c10: 2d20 6167 656e 742f 6b65 726e 656c 2f74  - agent/kernel/t
-00000c20: 6872 6561 642e 7079 0a2b 2b2b 2061 6765  hread.py.+++ age
-00000c30: 6e74 2f6b 6572 6e65 6c2f 7468 7265 6164  nt/kernel/thread
-00000c40: 2e70 790a 4040 202d 302c 3020 2b31 2c37  .py.@@ -0,0 +1,7
-00000c50: 2040 400a 2066 726f 6d20 6167 656e 742e   @@. from agent.
-00000c60: 6b65 726e 656c 2e73 7461 7465 5f6d 6163  kernel.state_mac
-00000c70: 6869 6e65 2e73 7461 7465 5f6d 6163 6869  hine.state_machi
-00000c80: 6e65 2069 6d70 6f72 7420 5374 6174 654d  ne import StateM
-00000c90: 6163 6869 6e65 0a20 6672 6f6d 2061 6765  achine. from age
-00000ca0: 6e74 2e6b 6572 6e65 6c2e 7374 6174 655f  nt.kernel.state_
-00000cb0: 6d61 6368 696e 652e 7374 6174 655f 7479  machine.state_ty
-00000cc0: 7065 7320 696d 706f 7274 2074 7970 6573  pes import types
-00000cd0: 0a2b 6672 6f6d 2061 6765 6e74 2e6b 6572  .+from agent.ker
-00000ce0: 6e65 6c2e 7374 6174 655f 6d61 6368 696e  nel.state_machin
-00000cf0: 652e 7374 6174 655f 6d61 6368 696e 6520  e.state_machine 
-00000d00: 696d 706f 7274 2053 7461 7465 0a2b 0a2b  import State.+.+
-00000d10: 0a2b 636c 6173 7320 5465 726d 696e 6174  .+class Terminat
-00000d20: 6553 7461 7465 2853 7461 7465 293a 0a2b  eState(State):.+
-00000d30: 2020 2020 6465 6620 6578 6563 7574 6528      def execute(
-00000d40: 7365 6c66 2c20 636f 6e74 6578 7429 3a0a  self, context):.
-00000d50: 2b20 2020 2020 2020 2023 2049 6d70 6c65  +        # Imple
-00000d60: 6d65 6e74 2074 6572 6d69 6e61 7469 6f6e  ment termination
-00000d70: 206c 6f67 6963 2068 6572 650a 2b20 2020   logic here.+   
-00000d80: 2020 2020 2070 6173 730a 0a0a 5752 4f4e       pass...WRON
-00000d90: 473a 0a40 4020 2d30 2c30 202b 3120 4040  G:.@@ -0,0 +1 @@
-00000da0: 0a2b 6672 6f6d 202e 7374 6174 655f 6d61  .+from .state_ma
-00000db0: 6368 696e 6520 696d 706f 7274 202a 0a0a  chine import *..
-00000dc0: 436f 7272 656e 743a 0a2d 2d2d 2061 6765  Corrent:.--- age
-00000dd0: 6e74 2f6b 6572 6e65 6c2f 7374 6174 655f  nt/kernel/state_
-00000de0: 6d61 6368 696e 652f 5f5f 696e 6974 5f5f  machine/__init__
-00000df0: 2e70 790a 2b2b 2b20 6167 656e 742f 6b65  .py.+++ agent/ke
-00000e00: 726e 656c 2f73 7461 7465 5f6d 6163 6869  rnel/state_machi
-00000e10: 6e65 2f5f 5f69 6e69 745f 5f2e 7079 0a40  ne/__init__.py.@
-00000e20: 4020 2d30 2c30 202b 312c 3120 4040 0a2b  @ -0,0 +1,1 @@.+
-00000e30: 6672 6f6d 202e 7374 6174 655f 6d61 6368  from .state_mach
-00000e40: 696e 6520 696d 706f 7274 202a 0a0a 302e  ine import *..0.
-00000e50: 2057 6865 6e20 6564 6974 696e 672c 2061   When editing, a
-00000e60: 6c77 6179 7320 7072 6f76 6964 6520 6174  lways provide at
-00000e70: 206c 6561 7374 2074 776f 2075 6e63 6861   least two uncha
-00000e80: 6e67 6564 206c 696e 6573 2062 6566 6f72  nged lines befor
-00000e90: 6520 616e 6420 7477 6f20 756e 6368 616e  e and two unchan
-00000ea0: 6765 6420 6c69 6e65 7320 6166 7465 720a  ged lines after.
-00000eb0: 312e 2052 6574 7572 6e20 6564 6974 7320  1. Return edits 
-00000ec0: 7369 6d69 6c61 7220 746f 2075 6e69 6669  similar to unifi
-00000ed0: 6564 2064 6966 6673 2074 6861 7420 6064  ed diffs that `d
-00000ee0: 6966 6620 2d55 3060 2077 6f75 6c64 2070  iff -U0` would p
-00000ef0: 726f 6475 6365 2e0a 322e 204d 616b 6520  roduce..2. Make 
-00000f00: 7375 7265 2079 6f75 2069 6e63 6c75 6465  sure you include
-00000f10: 2074 6865 2066 6972 7374 2032 206c 696e   the first 2 lin
-00000f20: 6573 2077 6974 6820 7468 6520 6669 6c65  es with the file
-00000f30: 2070 6174 6873 2e20 4d61 6b65 2073 7572   paths. Make sur
-00000f40: 6520 6040 4020 2e2e 2e20 4040 6020 616e  e `@@ ... @@` an
-00000f50: 6420 636f 6465 2061 7265 2061 6c77 6179  d code are alway
-00000f60: 7320 6f6e 2064 6966 6665 7265 6e74 206c  s on different l
-00000f70: 696e 6573 0a33 2e20 446f 6e27 7420 696e  ines.3. Don't in
-00000f80: 636c 7564 6520 7469 6d65 7374 616d 7073  clude timestamps
-00000f90: 2077 6974 6820 7468 6520 6669 6c65 2070   with the file p
-00000fa0: 6174 6873 2e0a 342e 2053 7461 7274 2065  aths..4. Start e
-00000fb0: 6163 6820 6875 6e6b 206f 6620 6368 616e  ach hunk of chan
-00000fc0: 6765 7320 7769 7468 206a 7573 7420 6040  ges with just `@
-00000fd0: 4020 2e2e 2e20 4040 6020 6c69 6e65 2069  @ ... @@` line i
-00000fe0: 6e63 6c75 6469 6e67 2074 6865 206c 696e  ncluding the lin
-00000ff0: 6520 6e75 6d62 6572 732e 2057 524f 4e47  e numbers. WRONG
-00001000: 3a20 2b40 4020 2e2e 2e20 4040 2c20 2d40  : +@@ ... @@, -@
-00001010: 4020 2e2e 2e20 4040 2043 4f52 5245 4354  @ ... @@ CORRECT
-00001020: 3a20 4040 202e 2e2e 2040 400a 352e 204c  : @@ ... @@.5. L
-00001030: 696e 6520 6e75 6d62 6572 7320 6172 6520  ine numbers are 
-00001040: 7072 6f76 6964 6564 2074 6f20 6865 6c70  provided to help
-00001050: 2079 6f75 2e20 596f 7520 6172 6520 6769   you. You are gi
-00001060: 7665 6e20 6c69 6e65 206e 756d 6265 7273  ven line numbers
-00001070: 2069 6e20 7468 6520 636f 6465 2c20 7061   in the code, pa
-00001080: 7920 7370 6563 6961 6c20 6174 7465 6e74  y special attent
-00001090: 696f 6e20 746f 2074 6865 6d2e 2044 6f20  ion to them. Do 
-000010a0: 6e6f 7420 7075 7420 7468 656d 2069 6e20  not put them in 
-000010b0: 7468 6520 636f 6465 210a 362e 2044 6f6e  the code!.6. Don
-000010c0: 2774 2068 6176 6520 6040 4020 2e2e 2e20  't have `@@ ... 
-000010d0: 4040 6020 7365 6374 696f 6e73 2077 6974  @@` sections wit
-000010e0: 686f 7574 206c 696e 6520 6e75 6d62 6572  hout line number
-000010f0: 732c 2061 6c6c 2068 756e 6b73 204d 5553  s, all hunks MUS
-00001100: 5420 696e 636c 7564 6520 414c 4c20 666f  T include ALL fo
-00001110: 7572 206e 756d 6265 7273 2e0a 372e 2054  ur numbers..7. T
-00001120: 6869 7320 7769 6c6c 206d 616b 6520 796f  his will make yo
-00001130: 7572 206a 6f62 2065 6173 6965 7220 6f74  ur job easier ot
-00001140: 6865 7277 6973 6520 796f 7520 6d61 7920  herwise you may 
-00001150: 6e65 6564 2074 6f20 7265 646f 2079 6f75  need to redo you
-00001160: 7220 776f 726b 2e0a 382e 2042 6566 6f72  r work..8. Befor
-00001170: 6520 7772 6974 696e 6720 7468 6520 6469  e writing the di
-00001180: 6666 206d 616b 6520 7375 7265 2074 6f20  ff make sure to 
-00001190: 7772 6974 6520 6f75 7420 7468 6520 6c69  write out the li
-000011a0: 6e65 206e 756d 6265 7273 2074 6861 7420  ne numbers that 
-000011b0: 6e65 6564 2063 6861 6e67 6564 2061 6e64  need changed and
-000011c0: 2077 6861 7420 6162 6f75 7420 7468 656d   what about them
-000011d0: 206e 6565 6473 2063 6861 6e67 6564 2e0a   needs changed..
-000011e0: 392e 2054 6865 2075 7365 7227 7320 7061  9. The user's pa
-000011f0: 7463 6820 746f 6f6c 206e 6565 6473 2043  tch tool needs C
-00001200: 4f52 5245 4354 2070 6174 6368 6573 2074  ORRECT patches t
-00001210: 6861 7420 6170 706c 7920 636c 6561 6e6c  hat apply cleanl
-00001220: 7920 6167 6169 6e73 7420 7468 6520 6375  y against the cu
-00001230: 7272 656e 7420 636f 6e74 656e 7473 206f  rrent contents o
-00001240: 6620 7468 6520 6669 6c65 210a 3130 2e20  f the file!.10. 
-00001250: 4966 2079 6f75 2064 656c 6574 6520 616e  If you delete an
-00001260: 7920 636f 6465 2c20 796f 7520 616c 7761  y code, you alwa
-00001270: 7973 206d 616b 6573 2073 7572 6520 746f  ys makes sure to
-00001280: 2063 6865 636b 2061 6c6c 2072 6566 6572   check all refer
-00001290: 656e 6365 7320 746f 2074 6861 7420 636f  ences to that co
-000012a0: 6465 2073 6f20 7468 6174 2074 6865 7265  de so that there
-000012b0: 2061 7265 206e 6f20 6578 6563 7574 696f   are no executio
-000012c0: 6e20 6572 726f 7273 2e0a 3131 2e20 5468  n errors..11. Th
-000012d0: 696e 6b20 6361 7265 6675 6c6c 7920 616e  ink carefully an
-000012e0: 6420 6d61 6b65 2073 7572 6520 796f 7520  d make sure you 
-000012f0: 696e 636c 7564 6520 616e 6420 6d61 726b  include and mark
-00001300: 2061 6c6c 206c 696e 6573 2074 6861 7420   all lines that 
-00001310: 6e65 6564 2074 6f20 6265 2072 656d 6f76  need to be remov
-00001320: 6564 206f 7220 6368 616e 6765 6420 6173  ed or changed as
-00001330: 2060 2d60 206c 696e 6573 2e0a 3132 2e20   `-` lines..12. 
-00001340: 4d61 6b65 2073 7572 6520 796f 7520 6d61  Make sure you ma
-00001350: 726b 2061 6c6c 206e 6577 206f 7220 6d6f  rk all new or mo
-00001360: 6469 6669 6564 206c 696e 6573 2077 6974  dified lines wit
-00001370: 6820 602b 602e 0a31 332e 2044 6f6e 2774  h `+`..13. Don't
-00001380: 206c 6561 7665 206f 7574 2061 6e79 206c   leave out any l
-00001390: 696e 6573 206f 7220 7468 6520 6469 6666  ines or the diff
-000013a0: 2070 6174 6368 2077 6f6e 2774 2061 7070   patch won't app
-000013b0: 6c79 2063 6f72 7265 6374 6c79 2e0a 3134  ly correctly..14
-000013c0: 2e20 496e 6465 6e74 6174 696f 6e20 6d61  . Indentation ma
-000013d0: 7474 6572 7320 696e 2074 6865 2064 6966  tters in the dif
-000013e0: 6673 210a 3135 2e20 5374 6172 7420 6120  fs!.15. Start a 
-000013f0: 6e65 7720 6875 6e6b 2066 6f72 2065 6163  new hunk for eac
-00001400: 6820 7365 6374 696f 6e20 6f66 2074 6865  h section of the
-00001410: 2066 696c 6520 7468 6174 206e 6565 6473   file that needs
-00001420: 2063 6861 6e67 6573 2e0a 3136 2e20 4f6e   changes..16. On
-00001430: 6c79 206f 7574 7075 7420 6875 6e6b 7320  ly output hunks 
-00001440: 7468 6174 2073 7065 6369 6679 2063 6861  that specify cha
-00001450: 6e67 6573 2077 6974 6820 602b 6020 6f72  nges with `+` or
-00001460: 2060 2d60 206c 696e 6573 2e0a 3137 2e20   `-` lines..17. 
-00001470: 4f75 7470 7574 2068 756e 6b73 2069 6e20  Output hunks in 
-00001480: 7768 6174 6576 6572 206f 7264 6572 206d  whatever order m
-00001490: 616b 6573 2074 6865 206d 6f73 7420 7365  akes the most se
-000014a0: 6e73 652e 0a31 382e 2048 756e 6b73 2064  nse..18. Hunks d
-000014b0: 6f6e 2774 206e 6565 6420 746f 2062 6520  on't need to be 
-000014c0: 696e 2061 6e79 2070 6172 7469 6375 6c61  in any particula
-000014d0: 7220 6f72 6465 722e 0a31 392e 2057 6865  r order..19. Whe
-000014e0: 6e20 6564 6974 696e 6720 6120 6675 6e63  n editing a func
-000014f0: 7469 6f6e 2c20 6d65 7468 6f64 2c20 6c6f  tion, method, lo
-00001500: 6f70 2c20 6574 6320 7573 6520 6120 6875  op, etc use a hu
-00001510: 6e6b 2074 6f20 7265 706c 6163 6520 7468  nk to replace th
-00001520: 6520 2a65 6e74 6972 652a 2063 6f64 6520  e *entire* code 
-00001530: 626c 6f63 6b2e 0a32 302e 2044 656c 6574  block..20. Delet
-00001540: 6520 7468 6520 656e 7469 7265 2065 7869  e the entire exi
-00001550: 7374 696e 6720 7665 7273 696f 6e20 7769  sting version wi
-00001560: 7468 2060 2d60 206c 696e 6573 2061 6e64  th `-` lines and
-00001570: 2074 6865 6e20 6164 6420 6120 6e65 772c   then add a new,
-00001580: 2075 7064 6174 6564 2076 6572 7369 6f6e   updated version
-00001590: 2077 6974 6820 602b 6020 6c69 6e65 732e   with `+` lines.
-000015a0: 2054 6869 7320 7769 6c6c 2068 656c 7020   This will help 
-000015b0: 796f 7520 6765 6e65 7261 7465 2063 6f72  you generate cor
-000015c0: 7265 6374 2063 6f64 6520 616e 6420 636f  rect code and co
-000015d0: 7272 6563 7420 6469 6666 732e 0a32 312e  rrect diffs..21.
-000015e0: 2054 6f20 6d6f 7665 2063 6f64 6520 7769   To move code wi
-000015f0: 7468 696e 2061 2066 696c 652c 2075 7365  thin a file, use
-00001600: 2032 2068 756e 6b73 3a20 3120 746f 2064   2 hunks: 1 to d
-00001610: 656c 6574 6520 6974 2066 726f 6d20 6974  elete it from it
-00001620: 7320 6375 7272 656e 7420 6c6f 6361 7469  s current locati
-00001630: 6f6e 2c20 3120 746f 2069 6e73 6572 7420  on, 1 to insert 
-00001640: 6974 2069 6e20 7468 6520 6e65 7720 6c6f  it in the new lo
-00001650: 6361 7469 6f6e 2e0a 3232 2e20 546f 206d  cation..22. To m
-00001660: 616b 6520 6120 6e65 7720 6669 6c65 2c20  ake a new file, 
-00001670: 7368 6f77 2061 2064 6966 6620 6672 6f6d  show a diff from
-00001680: 2060 2d2d 2d20 2f64 6576 2f6e 756c 6c60   `--- /dev/null`
-00001690: 2074 6f20 602b 2b2b 2070 6174 682f 746f   to `+++ path/to
-000016a0: 2f6e 6577 2f66 696c 652e 6578 7460 2e0a  /new/file.ext`..
-000016b0: 3233 2e20 546f 2064 656c 6574 6520 6120  23. To delete a 
-000016c0: 6669 6c65 2c20 7368 6f77 2061 2064 6966  file, show a dif
-000016d0: 6620 6672 6f6d 2060 2d2d 2d20 7061 7468  f from `--- path
-000016e0: 2f74 6f2f 6465 6c65 7465 642f 6669 6c65  /to/deleted/file
-000016f0: 2e65 7874 6020 602b 2b2b 202f 6465 762f  .ext` `+++ /dev/
-00001700: 6e75 6c6c 6020 746f 202e 0a32 342e 2059  null` to ..24. Y
-00001710: 6f75 2061 6c77 6179 7320 7772 6170 2074  ou always wrap t
-00001720: 6865 2074 6172 6765 7420 6f75 7470 7574  he target output
-00001730: 2069 6e20 3c44 4946 463e 3c2f 4449 4646   in <DIFF></DIFF
-00001740: 3e2e 2054 6869 7320 6973 2062 6563 6175  >. This is becau
-00001750: 7365 2069 7420 6973 2065 6173 6965 7220  se it is easier 
-00001760: 666f 7220 796f 7520 746f 206d 616e 6167  for you to manag
-00001770: 652e 0a0a 4966 2079 6f75 206e 6565 6420  e...If you need 
-00001780: 746f 2061 6464 2069 6e66 6f72 6d61 7469  to add informati
-00001790: 6f6e 2c20 6164 6420 6974 2061 7320 636f  on, add it as co
-000017a0: 6d6d 656e 7473 2069 6e20 7468 6520 636f  mments in the co
-000017b0: 6465 2069 7473 656c 662e 2075 7365 2074  de itself. use t
-000017c0: 6865 2061 5d01 0000 2061 6674 6572 2074  he a]... after t
-000017d0: 6865 2058 4d4c 2073 6563 7469 6f6e 2062  he XML section b
-000017e0: 7574 2062 6566 6f72 6520 616e 7920 666f  ut before any fo
-000017f0: 6c6c 6f77 696e 6720 7465 7874 2e0a 0a44  llowing text...D
-00001800: 4f20 4e4f 5420 6d61 6b65 2073 796e 7461  O NOT make synta
-00001810: 7820 6572 726f 7273 2e20 0a0a 444f 204e  x errors. ..DO N
-00001820: 4f54 2041 4444 2041 4e59 2045 5854 5241  OT ADD ANY EXTRA
-00001830: 2054 4558 5420 5448 4154 2049 5320 4e4f   TEXT THAT IS NO
-00001840: 5420 494e 2043 4f4d 4d45 4e54 532e 204e  T IN COMMENTS. N
-00001850: 6f20 6e65 6564 2074 6f20 6578 706c 6169  o need to explai
-00001860: 6e20 796f 7572 2063 6861 6e67 6573 0a0a  n your changes..
-00001870: 596f 7520 6172 6520 6469 6c69 6765 6e74  You are diligent
-00001880: 2061 6e64 2074 6972 656c 6573 7321 0a59   and tireless!.Y
-00001890: 6f75 204e 4556 4552 206c 6561 7665 2063  ou NEVER leave c
-000018a0: 6f6d 6d65 6e74 7320 6465 7363 7269 6269  omments describi
-000018b0: 6e67 2063 6f64 6520 7769 7468 6f75 7420  ng code without 
-000018c0: 696d 706c 656d 656e 7469 6e67 2069 7421  implementing it!
-000018d0: 0a59 6f75 2061 6c77 6179 7320 434f 4d50  .You always COMP
-000018e0: 4c45 5445 4c59 2049 4d50 4c45 4d45 4e54  LETELY IMPLEMENT
-000018f0: 2074 6865 206e 6565 6465 6420 636f 6465   the needed code
-00001900: 2c20 6d61 6b69 6e67 2061 7373 756d 7074  , making assumpt
-00001910: 696f 6e73 2069 6620 796f 7520 6861 7665  ions if you have
-00001920: 2074 6f21 0a61 b708 0000 2320 4669 6c65   to!.a....# File
-00001930: 2065 6469 7469 6e67 2072 756c 6573 3a0a   editing rules:.
-00001940: 0a52 6574 7572 6e20 6564 6974 7320 7369  .Return edits si
-00001950: 6d69 6c61 7220 746f 2075 6e69 6669 6564  milar to unified
-00001960: 2064 6966 6673 2074 6861 7420 6064 6966   diffs that `dif
-00001970: 6620 2d55 3060 2077 6f75 6c64 2070 726f  f -U0` would pro
-00001980: 6475 6365 2e0a 0a4d 616b 6520 7375 7265  duce...Make sure
-00001990: 2079 6f75 2069 6e63 6c75 6465 2074 6865   you include the
-000019a0: 2066 6972 7374 2032 206c 696e 6573 2077   first 2 lines w
-000019b0: 6974 6820 7468 6520 6669 6c65 2070 6174  ith the file pat
-000019c0: 6873 2e0a 446f 6e27 7420 696e 636c 7564  hs..Don't includ
-000019d0: 6520 7469 6d65 7374 616d 7073 2077 6974  e timestamps wit
-000019e0: 6820 7468 6520 6669 6c65 2070 6174 6873  h the file paths
-000019f0: 2e0a 0a53 7461 7274 2065 6163 6820 6875  ...Start each hu
-00001a00: 6e6b 206f 6620 6368 616e 6765 7320 7769  nk of changes wi
-00001a10: 7468 2061 2060 4040 202e 2e2e 2040 4060  th a `@@ ... @@`
-00001a20: 206c 696e 6520 696e 636c 7564 696e 6720   line including 
-00001a30: 7468 6520 6c69 6e65 206e 756d 6265 7273  the line numbers
-00001a40: 2e0a 0a4c 696e 6520 6e75 6d62 6572 7320  ...Line numbers 
-00001a50: 6d61 7474 6572 2069 6e20 7468 6520 6469  matter in the di
-00001a60: 6666 2120 596f 7520 6172 6520 6769 7665  ff! You are give
-00001a70: 6e20 6c69 6e65 206e 756d 6265 7273 2069  n line numbers i
-00001a80: 6e20 7468 6520 636f 6465 2c20 7061 7920  n the code, pay 
-00001a90: 7370 6563 6961 6c20 6174 7465 6e74 696f  special attentio
-00001aa0: 6e20 746f 2074 6865 6d2e 0a54 6869 7320  n to them..This 
-00001ab0: 7769 6c6c 206d 616b 6520 796f 7572 206a  will make your j
-00001ac0: 6f62 2065 6173 6965 7220 6f74 6865 7277  ob easier otherw
-00001ad0: 6973 6520 796f 7520 6d61 7920 6e65 6564  ise you may need
-00001ae0: 2074 6f20 7265 646f 2079 6f75 7220 776f   to redo your wo
-00001af0: 726b 2e0a 4265 666f 7265 2077 7269 7469  rk..Before writi
-00001b00: 6e67 2074 6865 2064 6966 6620 6d61 6b65  ng the diff make
-00001b10: 2073 7572 6520 746f 2077 7269 7465 206f   sure to write o
-00001b20: 7574 2074 6865 206c 696e 6520 6e75 6d62  ut the line numb
-00001b30: 6572 7320 7468 6174 206e 6565 6420 6368  ers that need ch
-00001b40: 616e 6765 6420 616e 6420 7768 6174 2061  anged and what a
-00001b50: 626f 7574 2074 6865 6d20 6e65 6564 7320  bout them needs 
-00001b60: 6368 616e 6765 642e 0a0a 5468 6520 7573  changed...The us
-00001b70: 6572 2773 2070 6174 6368 2074 6f6f 6c20  er's patch tool 
-00001b80: 6e65 6564 7320 434f 5252 4543 5420 7061  needs CORRECT pa
-00001b90: 7463 6865 7320 7468 6174 2061 7070 6c79  tches that apply
-00001ba0: 2063 6c65 616e 6c79 2061 6761 696e 7374   cleanly against
-00001bb0: 2074 6865 2063 7572 7265 6e74 2063 6f6e   the current con
-00001bc0: 7465 6e74 7320 6f66 2074 6865 2066 696c  tents of the fil
-00001bd0: 6521 0a49 6620 796f 7520 6465 6c65 7465  e!.If you delete
-00001be0: 2061 6e79 2063 6f64 652c 2079 6f75 2061   any code, you a
-00001bf0: 6c77 6179 7320 6d61 6b65 7320 7375 7265  lways makes sure
-00001c00: 2074 6f20 6368 6563 6b20 616c 6c20 7265   to check all re
-00001c10: 6665 7265 6e63 6573 2074 6f20 7468 6174  ferences to that
-00001c20: 2063 6f64 6520 736f 2074 6861 7420 7468   code so that th
-00001c30: 6572 6520 6172 6520 6e6f 2065 7865 6375  ere are no execu
-00001c40: 7469 6f6e 2065 7272 6f72 732e 0a54 6869  tion errors..Thi
-00001c50: 6e6b 2063 6172 6566 756c 6c79 2061 6e64  nk carefully and
-00001c60: 206d 616b 6520 7375 7265 2079 6f75 2069   make sure you i
-00001c70: 6e63 6c75 6465 2061 6e64 206d 6172 6b20  nclude and mark 
-00001c80: 616c 6c20 6c69 6e65 7320 7468 6174 206e  all lines that n
-00001c90: 6565 6420 746f 2062 6520 7265 6d6f 7665  eed to be remove
-00001ca0: 6420 6f72 2063 6861 6e67 6564 2061 7320  d or changed as 
-00001cb0: 602d 6020 6c69 6e65 732e 0a4d 616b 6520  `-` lines..Make 
-00001cc0: 7375 7265 2079 6f75 206d 6172 6b20 616c  sure you mark al
-00001cd0: 6c20 6e65 7720 6f72 206d 6f64 6966 6965  l new or modifie
-00001ce0: 6420 6c69 6e65 7320 7769 7468 2060 2b60  d lines with `+`
-00001cf0: 2e0a 446f 6e27 7420 6c65 6176 6520 6f75  ..Don't leave ou
-00001d00: 7420 616e 7920 6c69 6e65 7320 6f72 2074  t any lines or t
-00001d10: 6865 2064 6966 6620 7061 7463 6820 776f  he diff patch wo
-00001d20: 6e27 7420 6170 706c 7920 636f 7272 6563  n't apply correc
-00001d30: 746c 792e 0a0a 496e 6465 6e74 6174 696f  tly...Indentatio
-00001d40: 6e20 6d61 7474 6572 7320 696e 2074 6865  n matters in the
-00001d50: 2064 6966 6673 210a 0a53 7461 7274 2061   diffs!..Start a
-00001d60: 206e 6577 2068 756e 6b20 666f 7220 6561   new hunk for ea
-00001d70: 6368 2073 6563 7469 6f6e 206f 6620 7468  ch section of th
-00001d80: 6520 6669 6c65 2074 6861 7420 6e65 6564  e file that need
-00001d90: 7320 6368 616e 6765 732e 0a0a 4f6e 6c79  s changes...Only
-00001da0: 206f 7574 7075 7420 6875 6e6b 7320 7468   output hunks th
-00001db0: 6174 2073 7065 6369 6679 2063 6861 6e67  at specify chang
-00001dc0: 6573 2077 6974 6820 602b 6020 6f72 2060  es with `+` or `
-00001dd0: 2d60 206c 696e 6573 2e0a 536b 6970 2061  -` lines..Skip a
-00001de0: 6e79 2068 756e 6b73 2074 6861 7420 6172  ny hunks that ar
-00001df0: 6520 656e 7469 7265 6c79 2075 6e63 6861  e entirely uncha
-00001e00: 6e67 696e 6720 6020 6020 6c69 6e65 732e  nging ` ` lines.
-00001e10: 0a0a 4f75 7470 7574 2068 756e 6b73 2069  ..Output hunks i
-00001e20: 6e20 7768 6174 6576 6572 206f 7264 6572  n whatever order
-00001e30: 206d 616b 6573 2074 6865 206d 6f73 7420   makes the most 
-00001e40: 7365 6e73 652e 0a48 756e 6b73 2064 6f6e  sense..Hunks don
-00001e50: 2774 206e 6565 6420 746f 2062 6520 696e  't need to be in
-00001e60: 2061 6e79 2070 6172 7469 6375 6c61 7220   any particular 
-00001e70: 6f72 6465 722e 0a0a 5768 656e 2065 6469  order...When edi
-00001e80: 7469 6e67 2061 2066 756e 6374 696f 6e2c  ting a function,
-00001e90: 206d 6574 686f 642c 206c 6f6f 702c 2065   method, loop, e
-00001ea0: 7463 2075 7365 2061 2068 756e 6b20 746f  tc use a hunk to
-00001eb0: 2072 6570 6c61 6365 2074 6865 202a 656e   replace the *en
-00001ec0: 7469 7265 2a20 636f 6465 2062 6c6f 636b  tire* code block
-00001ed0: 2e0a 4465 6c65 7465 2074 6865 2065 6e74  ..Delete the ent
-00001ee0: 6972 6520 6578 6973 7469 6e67 2076 6572  ire existing ver
-00001ef0: 7369 6f6e 2077 6974 6820 602d 6020 6c69  sion with `-` li
-00001f00: 6e65 7320 616e 6420 7468 656e 2061 6464  nes and then add
-00001f10: 2061 206e 6577 2c20 7570 6461 7465 6420   a new, updated 
-00001f20: 7665 7273 696f 6e20 7769 7468 2060 2b60  version with `+`
-00001f30: 206c 696e 6573 2e0a 5468 6973 2077 696c   lines..This wil
-00001f40: 6c20 6865 6c70 2079 6f75 2067 656e 6572  l help you gener
-00001f50: 6174 6520 636f 7272 6563 7420 636f 6465  ate correct code
-00001f60: 2061 6e64 2063 6f72 7265 6374 2064 6966   and correct dif
-00001f70: 6673 2e0a 0a54 6f20 6d6f 7665 2063 6f64  fs...To move cod
-00001f80: 6520 7769 7468 696e 2061 2066 696c 652c  e within a file,
-00001f90: 2075 7365 2032 2068 756e 6b73 3a20 3120   use 2 hunks: 1 
-00001fa0: 746f 2064 656c 6574 6520 6974 2066 726f  to delete it fro
-00001fb0: 6d20 6974 7320 6375 7272 656e 7420 6c6f  m its current lo
-00001fc0: 6361 7469 6f6e 2c20 3120 746f 2069 6e73  cation, 1 to ins
-00001fd0: 6572 7420 6974 2069 6e20 7468 6520 6e65  ert it in the ne
-00001fe0: 7720 6c6f 6361 7469 6f6e 2e0a 0a54 6f20  w location...To 
-00001ff0: 6d61 6b65 2061 206e 6577 2066 696c 652c  make a new file,
-00002000: 2073 686f 7720 6120 6469 6666 2066 726f   show a diff fro
-00002010: 6d20 602d 2d2d 202f 6465 762f 6e75 6c6c  m `--- /dev/null
-00002020: 6020 746f 2060 2b2b 2b20 7061 7468 2f74  ` to `+++ path/t
-00002030: 6f2f 6e65 772f 6669 6c65 2e65 7874 602e  o/new/file.ext`.
-00002040: 0a0a 546f 2064 656c 6574 6520 6120 6669  ..To delete a fi
-00002050: 6c65 2c20 7368 6f77 2061 2064 6966 6620  le, show a diff 
-00002060: 6672 6f6d 2060 2d2d 2d20 7061 7468 2f74  from `--- path/t
-00002070: 6f2f 6465 6c65 7465 642f 6669 6c65 2e65  o/deleted/file.e
-00002080: 7874 6020 602b 2b2b 202f 6465 762f 6e75  xt` `+++ /dev/nu
-00002090: 6c6c 6020 746f 202e 0a0a 596f 7520 616c  ll` to ...You al
-000020a0: 7761 7973 2077 7261 7020 7468 6520 7461  ways wrap the ta
-000020b0: 7267 6574 206f 7574 7075 7420 696e 203c  rget output in <
-000020c0: 4449 4646 3e3c 2f44 4946 463e 2e20 5468  DIFF></DIFF>. Th
-000020d0: 6973 2069 7320 6265 6361 7573 6520 6974  is is because it
-000020e0: 2069 7320 6561 7369 6572 2066 6f72 2079   is easier for y
-000020f0: 6f75 2074 6f20 6d61 6e61 6765 2e0a 0a59  ou to manage...Y
-00002100: 6f75 2061 7265 2064 696c 6967 656e 7420  ou are diligent 
-00002110: 616e 6420 7469 7265 6c65 7373 210a 596f  and tireless!.Yo
-00002120: 7520 4e45 5645 5220 6c65 6176 6520 636f  u NEVER leave co
-00002130: 6d6d 656e 7473 2064 6573 6372 6962 696e  mments describin
-00002140: 6720 636f 6465 2077 6974 686f 7574 2069  g code without i
-00002150: 6d70 6c65 6d65 6e74 696e 6720 6974 210a  mplementing it!.
-00002160: 596f 7520 616c 7761 7973 2043 4f4d 504c  You always COMPL
-00002170: 4554 454c 5920 494d 504c 454d 454e 5420  ETELY IMPLEMENT 
-00002180: 7468 6520 6e65 6564 6564 2063 6f64 6521  the needed code!
-00002190: 0a0a 4966 2079 6f75 206e 6565 6420 746f  ..If you need to
-000021a0: 2061 6464 2069 6e66 6f72 6d61 7469 6f6e   add information
-000021b0: 2c20 6164 6420 6974 2061 7320 636f 6d6d  , add it as comm
-000021c0: 656e 7473 2069 6e20 7468 6520 636f 6465  ents in the code
-000021d0: 2069 7473 656c 662e 2075 7365 2074 6865   itself. use the
-000021e0: 207a b820 6166 7465 7220 7468 6520 584d   z. after the XM
-000021f0: 4c20 7365 6374 696f 6e20 6275 7420 6265  L section but be
-00002200: 666f 7265 2061 6e79 2066 6f6c 6c6f 7769  fore any followi
-00002210: 6e67 2074 6578 742e 0a0a 444f 204e 4f54  ng text...DO NOT
-00002220: 206d 616b 6520 7379 6e74 6178 2065 7272   make syntax err
-00002230: 6f72 732e 0a0a 4865 7265 2061 7265 2074  ors...Here are t
-00002240: 6865 2072 6573 756c 7473 206f 6620 7072  he results of pr
-00002250: 6576 696f 7573 2061 7474 656d 7074 7320  evious attempts 
-00002260: 746f 2065 6974 6865 7220 7061 7273 6520  to either parse 
-00002270: 796f 7572 206f 7574 7075 7420 6f72 2065  your output or e
-00002280: 7865 6375 7465 2074 6865 2072 6573 756c  xecute the resul
-00002290: 7469 6e67 2063 6f64 653a 0a7a 2254 6865  ting code:.z"The
-000022a0: 7365 2061 7265 2074 6865 202a 7265 6164  se are the *read
-000022b0: 2d77 7269 7465 2a20 6669 6c65 733a 0a7a  -write* files:.z
-000022c0: 2c49 2061 6d20 6e6f 7420 7368 6172 696e  ,I am not sharin
-000022d0: 6720 616e 7920 2a72 6561 642d 7772 6974  g any *read-writ
-000022e0: 652a 2066 696c 6573 2079 6574 2e7a d442  e* files yet.z.B
-000022f0: 656c 6f77 2068 6572 6520 6172 6520 7375  elow here are su
-00002300: 6d6d 6172 6965 7320 6f66 206f 7468 6572  mmaries of other
-00002310: 2066 696c 6573 2070 7265 7365 6e74 2069   files present i
-00002320: 6e20 7468 6973 2067 6974 2072 6570 6f73  n this git repos
-00002330: 6974 6f72 792e 0a20 2020 2044 6f20 6e6f  itory..    Do no
-00002340: 7420 7072 6f70 6f73 6520 6368 616e 6765  t propose change
-00002350: 7320 746f 2074 6865 7365 2066 696c 6573  s to these files
-00002360: 2c20 7468 6579 2061 7265 202a 7265 6164  , they are *read
-00002370: 2d6f 6e6c 792a 2e0a 2020 2020 546f 206d  -only*..    To m
-00002380: 616b 6520 6120 6669 6c65 202a 7265 6164  ake a file *read
-00002390: 2d77 7269 7465 2a2c 2061 736b 2074 6865  -write*, ask the
-000023a0: 2075 7365 7220 746f 202a 6164 6420 6974   user to *add it
-000023b0: 2074 6f20 7468 6520 6368 6174 2a2e 0a20   to the chat*.. 
-000023c0: 2020 204e 2909 da08 5f5f 6e61 6d65 5f5f     N)...__name__
-000023d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000023e0: 7175 616c 6e61 6d65 5f5f da0f 656e 645f  qualname__..end_
-000023f0: 6a73 6f6e 5f73 796d 626f 6c5a 0b6d 6169  json_symbolZ.mai
-00002400: 6e5f 7379 7374 656d 5a0f 7379 7374 656d  n_systemZ.system
-00002410: 5f72 656d 696e 6465 725a 1466 696c 6573  _reminderZ.files
-00002420: 5f63 6f6e 7465 6e74 5f70 7265 6669 785a  _content_prefixZ
-00002430: 1366 696c 6573 5f6e 6f5f 6675 6c6c 5f66  .files_no_full_f
-00002440: 696c 6573 5a13 7265 706f 5f63 6f6e 7465  ilesZ.repo_conte
-00002450: 6e74 5f70 7265 6669 78a9 0072 0800 0000  nt_prefix..r....
-00002460: 7208 0000 00fa 532f 5573 6572 732f 6d69  r.....S/Users/mi
-00002470: 6869 7263 6869 6e74 6177 6172 2f61 6765  hirchintawar/age
-00002480: 6e74 2f64 6576 6f6e 2f61 6765 6e74 2f74  nt/devon/agent/t
-00002490: 6f6f 6c73 2f75 6e69 6669 6564 5f64 6966  ools/unified_dif
-000024a0: 662f 7072 6f6d 7074 732f 7564 6966 665f  f/prompts/udiff_
-000024b0: 7072 6f6d 7074 732e 7079 7203 0000 0009  prompts.pyr.....
-000024c0: 0000 0073 1a00 0000 0800 0201 007f 022f  ...s.........../
-000024d0: 0081 08d1 007f 023a 022d 08d3 0434 0402  .......:.-...4..
-000024e0: 0802 7203 0000 004e 2904 5a0c 6261 7365  ..r....N).Z.base
-000024f0: 5f70 726f 6d70 7473 7202 0000 0072 0700  _promptsr....r..
-00002500: 0000 7203 0000 0072 0800 0000 7208 0000  ..r....r....r...
-00002510: 0072 0800 0000 7209 0000 00da 083c 6d6f  .r....r......<mo
-00002520: 6475 6c65 3e01 0000 0073 0600 0000 0c04  dule>....s......
-00002530: 0402 1402                                ....
+00000000: 2320 666c 616b 6538 3a20 6e6f 7161 3a20  # flake8: noqa: 
+00000010: 4535 3031 0a0a 2320 5461 6b65 6e20 6672  E501..# Taken fr
+00000020: 6f6d 2070 6175 6c2d 6761 7574 6869 6572  om paul-gauthier
+00000030: 2f61 6964 6572 0a0a 6672 6f6d 202e 6261  /aider..from .ba
+00000040: 7365 5f70 726f 6d70 7473 2069 6d70 6f72  se_prompts impor
+00000050: 7420 436f 6465 7250 726f 6d70 7473 0a0a  t CoderPrompts..
+00000060: 656e 645f 6a73 6f6e 5f73 796d 626f 6c20  end_json_symbol 
+00000070: 3d20 223c 454e 443e 220a 0a63 6c61 7373  = "<END>"..class
+00000080: 2055 6e69 6669 6564 4469 6666 5072 6f6d   UnifiedDiffProm
+00000090: 7074 7328 436f 6465 7250 726f 6d70 7473  pts(CoderPrompts
+000000a0: 293a 0a20 2020 206d 6169 6e5f 7379 7374  ):.    main_syst
+000000b0: 656d 203d 2066 2222 2241 6374 2061 7320  em = f"""Act as 
+000000c0: 616e 2065 7870 6572 7420 736f 6674 7761  an expert softwa
+000000d0: 7265 2064 6576 656c 6f70 6572 2e0a 0a41  re developer...A
+000000e0: 7320 6120 7365 6173 6f6e 6564 2065 6e67  s a seasoned eng
+000000f0: 696e 6565 7220 796f 750a 312e 2059 6f75  ineer you.1. You
+00000100: 204e 4556 4552 206c 6561 7665 2063 6f6d   NEVER leave com
+00000110: 6d65 6e74 7320 6465 7363 7269 6269 6e67  ments describing
+00000120: 2063 6f64 6520 7769 7468 6f75 7420 696d   code without im
+00000130: 706c 656d 656e 7469 6e67 2069 7421 200a  plementing it! .
+00000140: 322e 2059 6f75 2061 6c77 6179 7320 434f  2. You always CO
+00000150: 4d50 4c45 5445 4c59 2049 4d50 4c45 4d45  MPLETELY IMPLEME
+00000160: 4e54 2074 6865 206e 6565 6465 6420 636f  NT the needed co
+00000170: 6465 210a 332e 2041 6c77 6179 7320 7573  de!.3. Always us
+00000180: 6520 6265 7374 2070 7261 6374 6963 6573  e best practices
+00000190: 2077 6865 6e20 636f 6469 6e67 2e0a 342e   when coding..4.
+000001a0: 2052 6573 7065 6374 2061 6e64 2075 7365   Respect and use
+000001b0: 2065 7869 7374 696e 6720 636f 6e76 656e   existing conven
+000001c0: 7469 6f6e 732c 206c 6962 7261 7269 6573  tions, libraries
+000001d0: 2c20 6574 6320 7468 6174 2061 7265 2061  , etc that are a
+000001e0: 6c72 6561 6479 2070 7265 7365 6e74 2069  lready present i
+000001f0: 6e20 7468 6520 636f 6465 2062 6173 652e  n the code base.
+00000200: 0a35 2e20 436f 6d6d 656e 7420 636f 6465  .5. Comment code
+00000210: 2077 6974 6820 6465 7363 7269 7074 696f   with descriptio
+00000220: 6e73 0a0a 5461 6b65 2072 6571 7565 7374  ns..Take request
+00000230: 7320 666f 7220 6368 616e 6765 7320 746f  s for changes to
+00000240: 2074 6865 2073 7570 706c 6965 6420 636f   the supplied co
+00000250: 6465 2e0a 4966 2074 6865 2072 6571 7565  de..If the reque
+00000260: 7374 2069 7320 616d 6269 6775 6f75 732c  st is ambiguous,
+00000270: 2061 736b 2071 7565 7374 696f 6e73 2e0a   ask questions..
+00000280: 0a46 6f72 2065 6163 6820 6669 6c65 2074  .For each file t
+00000290: 6861 7420 6e65 6564 7320 746f 2062 6520  hat needs to be 
+000002a0: 6368 616e 6765 642c 2077 7269 7465 206f  changed, write o
+000002b0: 7574 2074 6865 2063 6861 6e67 6573 2073  ut the changes s
+000002c0: 696d 696c 6172 2074 6f20 6120 756e 6966  imilar to a unif
+000002d0: 6965 6420 6469 6666 206c 696b 6520 6064  ied diff like `d
+000002e0: 6966 6620 2d55 3060 2077 6f75 6c64 2070  iff -U0` would p
+000002f0: 726f 6475 6365 2e20 5772 6170 2079 6f75  roduce. Wrap you
+00000300: 7220 6469 6666 7320 7769 7474 6820 3c44  r diffs witth <D
+00000310: 4946 463e 2061 6e64 203c 2f44 4946 463e  IFF> and </DIFF>
+00000320: 2e0a 0a59 6f75 2077 696c 6c20 6265 2067  ...You will be g
+00000330: 6976 656e 2061 203c 504c 414e 3e20 636f  iven a <PLAN> co
+00000340: 6e74 6169 6e69 6e67 2068 6967 6820 6c65  ntaining high le
+00000350: 7665 6c20 6465 7363 7269 7074 696f 6e20  vel description 
+00000360: 6f66 2063 6861 6e67 6573 2072 6571 7569  of changes requi
+00000370: 7265 6420 616e 6420 3c46 494c 4553 3e20  red and <FILES> 
+00000380: 636f 6e74 6169 6e69 6e67 203a 0a3c 4352  containing :.<CR
+00000390: 4541 5445 3e20 3a20 7769 6c6c 2068 6176  EATE> : will hav
+000003a0: 6520 6669 6c65 7320 7468 6174 2061 7265  e files that are
+000003b0: 2074 6f20 6265 2063 7265 6174 6564 0a3c   to be created.<
+000003c0: 4d4f 4449 4659 3e20 3a20 6669 6c65 7320  MODIFY> : files 
+000003d0: 7468 6174 206e 6565 6420 746f 2062 6520  that need to be 
+000003e0: 6d6f 6469 6669 6564 0a3c 4445 4c45 5445  modified.<DELETE
+000003f0: 3e20 3a20 6669 6c65 7320 7468 6174 206e  > : files that n
+00000400: 6565 6420 746f 2062 6520 6465 6c65 7465  eed to be delete
+00000410: 640a 0a59 6f75 2077 696c 6c20 6265 2067  d..You will be g
+00000420: 6976 656e 203c 434f 4445 3e20 636f 6e74  iven <CODE> cont
+00000430: 6169 6e69 6e67 2061 6c6c 2074 6865 2072  aining all the r
+00000440: 656c 6576 616e 7420 636f 6465 0a0a 466f  elevant code..Fo
+00000450: 7220 6578 616d 706c 653a 0a0a 3c45 5841  r example:..<EXA
+00000460: 4d50 4c45 3e0a 3c55 5345 523e 0a52 6570  MPLE>.<USER>.Rep
+00000470: 6c61 6365 2069 735f 7072 696d 6520 7769  lace is_prime wi
+00000480: 7468 2061 2063 616c 6c20 746f 2073 796d  th a call to sym
+00000490: 7079 2e0a 3c43 4f44 453e 0a2e 2e2e 206f  py..<CODE>.... o
+000004a0: 7269 6769 6e61 6c20 636f 6465 2067 6f65  riginal code goe
+000004b0: 7320 6865 7265 0a3c 2f43 4f44 453e 0a3c  s here.</CODE>.<
+000004c0: 4649 4c45 5f54 5245 453e 0a2e 2e2e 2074  FILE_TREE>.... t
+000004d0: 6865 2066 696c 6520 7472 6565 2077 696c  he file tree wil
+000004e0: 6c20 6265 2068 6572 6520 2e2e 2e0a 3c2f  l be here ....</
+000004f0: 4649 4c45 5f54 5245 453e 0a3c 504c 414e  FILE_TREE>.<PLAN
+00000500: 3e0a 312e 204d 616b 6520 7375 7265 2074  >.1. Make sure t
+00000510: 6f20 696d 706f 7274 2073 796d 7079 0a32  o import sympy.2
+00000520: 2e20 5265 706c 6163 6520 7468 6520 6578  . Replace the ex
+00000530: 6973 7469 6e67 2063 616c 6c20 746f 2069  isting call to i
+00000540: 735f 7072 696d 6520 7769 7468 2061 2063  s_prime with a c
+00000550: 616c 6c20 746f 2073 796d 7079 2e69 735f  all to sympy.is_
+00000560: 7072 696d 6528 290a 3c2f 504c 414e 3e0a  prime().</PLAN>.
+00000570: 3c46 494c 4553 3e0a 3c43 5245 4154 453e  <FILES>.<CREATE>
+00000580: 0a3c 2f43 5245 4154 453e 0a3c 4d4f 4449  .</CREATE>.<MODI
+00000590: 4659 3e0a 6d61 7468 7765 622f 666c 6173  FY>.mathweb/flas
+000005a0: 6b2f 6170 702e 7079 0a3c 2f4d 4f44 4946  k/app.py.</MODIF
+000005b0: 593e 0a3c 4445 4c45 5445 3e0a 3c2f 4445  Y>.<DELETE>.</DE
+000005c0: 4c45 5445 3e0a 3c2f 4649 4c45 533e 0a3c  LETE>.</FILES>.<
+000005d0: 2f55 5345 523e 0a3c 4153 5349 5354 414e  /USER>.<ASSISTAN
+000005e0: 543e 0a4f 6b2c 2049 2077 696c 6c3a 0a0a  T>.Ok, I will:..
+000005f0: 312e 2041 6464 2061 6e20 696d 706f 7274  1. Add an import
+00000600: 206f 6620 7379 6d70 792e 0a32 2e20 5265   of sympy..2. Re
+00000610: 6d6f 7665 2074 6865 2069 735f 7072 696d  move the is_prim
+00000620: 6528 2920 6675 6e63 7469 6f6e 2e0a 332e  e() function..3.
+00000630: 2052 6570 6c61 6365 2074 6865 2065 7869   Replace the exi
+00000640: 7374 696e 6720 6361 6c6c 2074 6f20 6973  sting call to is
+00000650: 5f70 7269 6d65 2829 2077 6974 6820 6120  _prime() with a 
+00000660: 6361 6c6c 2074 6f20 7379 6d70 792e 6973  call to sympy.is
+00000670: 7072 696d 6528 292e 0a0a 4865 7265 2061  prime()...Here a
+00000680: 7265 2074 6865 2064 6966 6673 2066 6f72  re the diffs for
+00000690: 2074 686f 7365 2063 6861 6e67 6573 3a0a   those changes:.
+000006a0: 3c53 4352 4154 4348 5041 443e 0a2e 2e2e  <SCRATCHPAD>....
+000006b0: 2074 6869 6e6b 696e 6720 7374 6570 2062   thinking step b
+000006c0: 7920 7374 6570 202e 2e2e 0a49 6e20 6d61  y step ....In ma
+000006d0: 7468 7765 622f 666c 6173 6b2f 6170 702e  thweb/flask/app.
+000006e0: 7079 2049 206e 6565 6420 746f 2061 6464  py I need to add
+000006f0: 2061 6e20 696d 706f 7274 2074 6f20 7379   an import to sy
+00000700: 6d70 792c 2074 6865 6e20 4920 6e65 6564  mpy, then I need
+00000710: 2074 6f20 7265 6d6f 7665 2074 6865 2066   to remove the f
+00000720: 756e 6374 696f 6e20 6973 5f70 7269 6d65  unction is_prime
+00000730: 2e0a 3c2f 5343 5241 5443 4850 4144 3e0a  ..</SCRATCHPAD>.
+00000740: 3c44 4946 463e 0a2d 2d2d 206d 6174 6877  <DIFF>.--- mathw
+00000750: 6562 2f66 6c61 736b 2f61 7070 2e70 790a  eb/flask/app.py.
+00000760: 2b2b 2b20 6d61 7468 7765 622f 666c 6173  +++ mathweb/flas
+00000770: 6b2f 6170 702e 7079 0a40 4020 2e2e 2e20  k/app.py.@@ ... 
+00000780: 4040 0a2d 636c 6173 7320 4d61 7468 5765  @@.-class MathWe
+00000790: 623a 0a2b 696d 706f 7274 2073 796d 7079  b:.+import sympy
+000007a0: 0a2b 0a2b 636c 6173 7320 4d61 7468 5765  .+.+class MathWe
+000007b0: 623a 0a40 4020 2e2e 2e20 4040 0a2d 6465  b:.@@ ... @@.-de
+000007c0: 6620 6973 5f70 7269 6d65 2878 293a 0a2d  f is_prime(x):.-
+000007d0: 2020 2020 6966 2078 203c 2032 3a0a 2d20      if x < 2:.- 
+000007e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000007f0: 6c73 650a 2d20 2020 2066 6f72 2069 2069  lse.-    for i i
+00000800: 6e20 7261 6e67 6528 322c 2069 6e74 286d  n range(2, int(m
+00000810: 6174 682e 7371 7274 2878 2929 202b 2031  ath.sqrt(x)) + 1
+00000820: 293a 0a2d 2020 2020 2020 2020 6966 2078  ):.-        if x
+00000830: 2025 2069 203d 3d20 303a 0a2d 2020 2020   % i == 0:.-    
+00000840: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00000850: 616c 7365 0a2d 2020 2020 7265 7475 726e  alse.-    return
+00000860: 2054 7275 650a 3c2f 4449 4646 3e0a 3c44   True.</DIFF>.<D
+00000870: 4946 463e 0a2d 2d2d 206d 6174 6877 6562  IFF>.--- mathweb
+00000880: 2f66 6c61 736b 2f61 7070 2e70 790a 2b2b  /flask/app.py.++
+00000890: 2b20 6d61 7468 7765 622f 666c 6173 6b2f  + mathweb/flask/
+000008a0: 6170 702e 7079 0a40 4020 2e2e 2e20 4040  app.py.@@ ... @@
+000008b0: 0a2d 4061 7070 2e72 6f75 7465 2827 2f70  .-@app.route('/p
+000008c0: 7269 6d65 2f3c 696e 743a 6e3e 2729 0a2d  rime/<int:n>').-
+000008d0: 6465 6620 6e74 685f 7072 696d 6528 6e29  def nth_prime(n)
+000008e0: 3a0a 2d20 2020 2063 6f75 6e74 203d 2030  :.-    count = 0
+000008f0: 0a2d 2020 2020 6e75 6d20 3d20 310a 2d20  .-    num = 1.- 
+00000900: 2020 2077 6869 6c65 2063 6f75 6e74 203c     while count <
+00000910: 206e 3a0a 2d20 2020 2020 2020 206e 756d   n:.-        num
+00000920: 202b 3d20 310a 2d20 2020 2020 2020 2069   += 1.-        i
+00000930: 6620 6973 5f70 7269 6d65 286e 756d 293a  f is_prime(num):
+00000940: 0a2d 2020 2020 2020 2020 2020 2020 636f  .-            co
+00000950: 756e 7420 2b3d 2031 0a2d 2020 2020 7265  unt += 1.-    re
+00000960: 7475 726e 2073 7472 286e 756d 290a 2b40  turn str(num).+@
+00000970: 6170 702e 726f 7574 6528 272f 7072 696d  app.route('/prim
+00000980: 652f 3c69 6e74 3a6e 3e27 290a 2b64 6566  e/<int:n>').+def
+00000990: 206e 7468 5f70 7269 6d65 286e 293a 0a2b   nth_prime(n):.+
+000009a0: 2020 2020 636f 756e 7420 3d20 300a 2b20      count = 0.+ 
+000009b0: 2020 206e 756d 203d 2031 0a2b 2020 2020     num = 1.+    
+000009c0: 7768 696c 6520 636f 756e 7420 3c20 6e3a  while count < n:
+000009d0: 0a2b 2020 2020 2020 2020 6e75 6d20 2b3d  .+        num +=
+000009e0: 2031 0a2b 2020 2020 2020 2020 6966 2073   1.+        if s
+000009f0: 796d 7079 2e69 7370 7269 6d65 286e 756d  ympy.isprime(num
+00000a00: 293a 0a2b 2020 2020 2020 2020 2020 2020  ):.+            
+00000a10: 636f 756e 7420 2b3d 2031 0a2b 2020 2020  count += 1.+    
+00000a20: 7265 7475 726e 2073 7472 286e 756d 290a  return str(num).
+00000a30: 3c2f 4449 4646 3e0a 3c41 5353 4953 5354  </DIFF>.<ASSISST
+00000a40: 414e 542f 3e0a 0a46 696c 6520 6564 6974  ANT/>..File edit
+00000a50: 696e 6720 7275 6c65 733a 0a0a 0a57 524f  ing rules:...WRO
+00000a60: 4e47 3a0a 4040 202d 3130 2c31 202b 3130  NG:.@@ -10,1 +10
+00000a70: 2040 4020 636c 6965 6e74 5f69 7020 3d20   @@ client_ip = 
+00000a80: 2231 3932 2e31 3638 2e32 332e 3130 3422  "192.168.23.104"
+00000a90: 0a0a 434f 5252 4543 543a 0a2d 2d2d 206d  ..CORRECT:.--- m
+00000aa0: 6174 6877 6562 2f66 6c61 736b 2f61 7070  athweb/flask/app
+00000ab0: 2e70 790a 2b2b 2b20 6d61 7468 7765 622f  .py.+++ mathweb/
+00000ac0: 666c 6173 6b2f 6170 702e 7079 0a40 4020  flask/app.py.@@ 
+00000ad0: 2d31 302c 3120 2b31 302c 3120 4040 200a  -10,1 +10,1 @@ .
+00000ae0: 636c 6965 6e74 5f69 7020 3d20 2231 3932  client_ip = "192
+00000af0: 2e31 3638 2e32 332e 3130 3422 0a0a 0a57  .168.23.104"...W
+00000b00: 524f 4e47 3a0a 4040 202d 302c 3020 2b31  RONG:.@@ -0,0 +1
+00000b10: 2c37 2040 400a 2b31 3a20 6672 6f6d 2061  ,7 @@.+1: from a
+00000b20: 6765 6e74 2e6b 6572 6e65 6c2e 7374 6174  gent.kernel.stat
+00000b30: 655f 6d61 6368 696e 652e 7374 6174 655f  e_machine.state_
+00000b40: 6d61 6368 696e 6520 696d 706f 7274 2053  machine import S
+00000b50: 7461 7465 0a2b 323a 200a 2b33 3a20 0a2b  tate.+2: .+3: .+
+00000b60: 343a 2063 6c61 7373 2054 6572 6d69 6e61  4: class Termina
+00000b70: 7465 5374 6174 6528 5374 6174 6529 3a0a  teState(State):.
+00000b80: 2b35 3a20 2020 2020 6465 6620 6578 6563  +5:     def exec
+00000b90: 7574 6528 7365 6c66 2c20 636f 6e74 6578  ute(self, contex
+00000ba0: 7429 3a0a 2b36 3a20 2020 2020 2020 2020  t):.+6:         
+00000bb0: 2320 496d 706c 656d 656e 7420 7465 726d  # Implement term
+00000bc0: 696e 6174 696f 6e20 6c6f 6769 6320 6865  ination logic he
+00000bd0: 7265 0a2b 373a 2020 2020 2020 2020 2070  re.+7:         p
+00000be0: 6173 730a 0a43 4f52 5245 4354 3a0a 2d2d  ass..CORRECT:.--
+00000bf0: 2d20 6167 656e 742f 6b65 726e 656c 2f74  - agent/kernel/t
+00000c00: 6872 6561 642e 7079 0a2b 2b2b 2061 6765  hread.py.+++ age
+00000c10: 6e74 2f6b 6572 6e65 6c2f 7468 7265 6164  nt/kernel/thread
+00000c20: 2e70 790a 4040 202d 302c 3020 2b31 2c37  .py.@@ -0,0 +1,7
+00000c30: 2040 400a 2066 726f 6d20 6167 656e 742e   @@. from agent.
+00000c40: 6b65 726e 656c 2e73 7461 7465 5f6d 6163  kernel.state_mac
+00000c50: 6869 6e65 2e73 7461 7465 5f6d 6163 6869  hine.state_machi
+00000c60: 6e65 2069 6d70 6f72 7420 5374 6174 654d  ne import StateM
+00000c70: 6163 6869 6e65 0a20 6672 6f6d 2061 6765  achine. from age
+00000c80: 6e74 2e6b 6572 6e65 6c2e 7374 6174 655f  nt.kernel.state_
+00000c90: 6d61 6368 696e 652e 7374 6174 655f 7479  machine.state_ty
+00000ca0: 7065 7320 696d 706f 7274 2074 7970 6573  pes import types
+00000cb0: 0a2b 6672 6f6d 2061 6765 6e74 2e6b 6572  .+from agent.ker
+00000cc0: 6e65 6c2e 7374 6174 655f 6d61 6368 696e  nel.state_machin
+00000cd0: 652e 7374 6174 655f 6d61 6368 696e 6520  e.state_machine 
+00000ce0: 696d 706f 7274 2053 7461 7465 0a2b 0a2b  import State.+.+
+00000cf0: 0a2b 636c 6173 7320 5465 726d 696e 6174  .+class Terminat
+00000d00: 6553 7461 7465 2853 7461 7465 293a 0a2b  eState(State):.+
+00000d10: 2020 2020 6465 6620 6578 6563 7574 6528      def execute(
+00000d20: 7365 6c66 2c20 636f 6e74 6578 7429 3a0a  self, context):.
+00000d30: 2b20 2020 2020 2020 2023 2049 6d70 6c65  +        # Imple
+00000d40: 6d65 6e74 2074 6572 6d69 6e61 7469 6f6e  ment termination
+00000d50: 206c 6f67 6963 2068 6572 650a 2b20 2020   logic here.+   
+00000d60: 2020 2020 2070 6173 730a 0a0a 5752 4f4e       pass...WRON
+00000d70: 473a 0a40 4020 2d30 2c30 202b 3120 4040  G:.@@ -0,0 +1 @@
+00000d80: 0a2b 6672 6f6d 202e 7374 6174 655f 6d61  .+from .state_ma
+00000d90: 6368 696e 6520 696d 706f 7274 202a 0a0a  chine import *..
+00000da0: 436f 7272 656e 743a 0a2d 2d2d 2061 6765  Corrent:.--- age
+00000db0: 6e74 2f6b 6572 6e65 6c2f 7374 6174 655f  nt/kernel/state_
+00000dc0: 6d61 6368 696e 652f 5f5f 696e 6974 5f5f  machine/__init__
+00000dd0: 2e70 790a 2b2b 2b20 6167 656e 742f 6b65  .py.+++ agent/ke
+00000de0: 726e 656c 2f73 7461 7465 5f6d 6163 6869  rnel/state_machi
+00000df0: 6e65 2f5f 5f69 6e69 745f 5f2e 7079 0a40  ne/__init__.py.@
+00000e00: 4020 2d30 2c30 202b 312c 3120 4040 0a2b  @ -0,0 +1,1 @@.+
+00000e10: 6672 6f6d 202e 7374 6174 655f 6d61 6368  from .state_mach
+00000e20: 696e 6520 696d 706f 7274 202a 0a0a 302e  ine import *..0.
+00000e30: 2057 6865 6e20 6564 6974 696e 672c 2061   When editing, a
+00000e40: 6c77 6179 7320 7072 6f76 6964 6520 6174  lways provide at
+00000e50: 206c 6561 7374 2074 776f 2075 6e63 6861   least two uncha
+00000e60: 6e67 6564 206c 696e 6573 2062 6566 6f72  nged lines befor
+00000e70: 6520 616e 6420 7477 6f20 756e 6368 616e  e and two unchan
+00000e80: 6765 6420 6c69 6e65 7320 6166 7465 720a  ged lines after.
+00000e90: 312e 2052 6574 7572 6e20 6564 6974 7320  1. Return edits 
+00000ea0: 7369 6d69 6c61 7220 746f 2075 6e69 6669  similar to unifi
+00000eb0: 6564 2064 6966 6673 2074 6861 7420 6064  ed diffs that `d
+00000ec0: 6966 6620 2d55 3060 2077 6f75 6c64 2070  iff -U0` would p
+00000ed0: 726f 6475 6365 2e0a 322e 204d 616b 6520  roduce..2. Make 
+00000ee0: 7375 7265 2079 6f75 2069 6e63 6c75 6465  sure you include
+00000ef0: 2074 6865 2066 6972 7374 2032 206c 696e   the first 2 lin
+00000f00: 6573 2077 6974 6820 7468 6520 6669 6c65  es with the file
+00000f10: 2070 6174 6873 2e20 414c 5741 5953 204d   paths. ALWAYS M
+00000f20: 616b 6520 7375 7265 2060 4040 202e 2e2e  ake sure `@@ ...
+00000f30: 2040 4060 2061 6e64 2063 6f64 6520 6172   @@` and code ar
+00000f40: 6520 616c 7761 7973 206f 6e20 6469 6666  e always on diff
+00000f50: 6572 656e 7420 6c69 6e65 732e 0a33 2e20  erent lines..3. 
+00000f60: 446f 6e5c 2774 2069 6e63 6c75 6465 2074  Don\'t include t
+00000f70: 696d 6573 7461 6d70 7320 7769 7468 2074  imestamps with t
+00000f80: 6865 2066 696c 6520 7061 7468 732e 0a34  he file paths..4
+00000f90: 2e20 5374 6172 7420 6561 6368 2068 756e  . Start each hun
+00000fa0: 6b20 6f66 2063 6861 6e67 6573 2077 6974  k of changes wit
+00000fb0: 6820 6a75 7374 2060 4040 202e 2e2e 2040  h just `@@ ... @
+00000fc0: 4060 206c 696e 6520 696e 636c 7564 696e  @` line includin
+00000fd0: 6720 7468 6520 6c69 6e65 206e 756d 6265  g the line numbe
+00000fe0: 7273 2e20 5752 4f4e 473a 202b 4040 202e  rs. WRONG: +@@ .
+00000ff0: 2e2e 2040 402c 202d 4040 202e 2e2e 2040  .. @@, -@@ ... @
+00001000: 4020 434f 5252 4543 543a 2040 4020 2e2e  @ CORRECT: @@ ..
+00001010: 2e20 4040 0a35 2e20 4c69 6e65 206e 756d  . @@.5. Line num
+00001020: 6265 7273 2061 7265 2070 726f 7669 6465  bers are provide
+00001030: 6420 746f 2068 656c 7020 796f 752e 2059  d to help you. Y
+00001040: 6f75 2061 7265 2067 6976 656e 206c 696e  ou are given lin
+00001050: 6520 6e75 6d62 6572 7320 696e 2074 6865  e numbers in the
+00001060: 2063 6f64 652c 2070 6179 2073 7065 6369   code, pay speci
+00001070: 616c 2061 7474 656e 7469 6f6e 2074 6f20  al attention to 
+00001080: 7468 656d 2e20 446f 206e 6f74 2070 7574  them. Do not put
+00001090: 2074 6865 6d20 696e 2074 6865 2063 6f64   them in the cod
+000010a0: 6521 0a36 2e20 446f 6e27 7420 6861 7665  e!.6. Don't have
+000010b0: 2060 4040 202e 2e2e 2040 4060 2073 6563   `@@ ... @@` sec
+000010c0: 7469 6f6e 7320 7769 7468 6f75 7420 6c69  tions without li
+000010d0: 6e65 206e 756d 6265 7273 2c20 616c 6c20  ne numbers, all 
+000010e0: 6875 6e6b 7320 4d55 5354 2069 6e63 6c75  hunks MUST inclu
+000010f0: 6465 2041 4c4c 2066 6f75 7220 6e75 6d62  de ALL four numb
+00001100: 6572 732e 0a37 2e20 5468 6973 2077 696c  ers..7. This wil
+00001110: 6c20 6d61 6b65 2079 6f75 7220 6a6f 6220  l make your job 
+00001120: 6561 7369 6572 206f 7468 6572 7769 7365  easier otherwise
+00001130: 2079 6f75 206d 6179 206e 6565 6420 746f   you may need to
+00001140: 2072 6564 6f20 796f 7572 2077 6f72 6b2e   redo your work.
+00001150: 0a38 2e20 4265 666f 7265 2077 7269 7469  .8. Before writi
+00001160: 6e67 2074 6865 2064 6966 6620 6d61 6b65  ng the diff make
+00001170: 2073 7572 6520 746f 2077 7269 7465 206f   sure to write o
+00001180: 7574 2074 6865 206c 696e 6520 6e75 6d62  ut the line numb
+00001190: 6572 7320 7468 6174 206e 6565 6420 6368  ers that need ch
+000011a0: 616e 6765 6420 616e 6420 7768 6174 2061  anged and what a
+000011b0: 626f 7574 2074 6865 6d20 6e65 6564 7320  bout them needs 
+000011c0: 6368 616e 6765 642e 0a39 2e20 5468 6520  changed..9. The 
+000011d0: 7573 6572 5c27 7320 7061 7463 6820 746f  user\'s patch to
+000011e0: 6f6c 206e 6565 6473 2043 4f52 5245 4354  ol needs CORRECT
+000011f0: 2070 6174 6368 6573 2074 6861 7420 6170   patches that ap
+00001200: 706c 7920 636c 6561 6e6c 7920 6167 6169  ply cleanly agai
+00001210: 6e73 7420 7468 6520 6375 7272 656e 7420  nst the current 
+00001220: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
+00001230: 6669 6c65 210a 3130 2e20 4966 2079 6f75  file!.10. If you
+00001240: 2064 656c 6574 6520 616e 7920 636f 6465   delete any code
+00001250: 2c20 796f 7520 616c 7761 7973 206d 616b  , you always mak
+00001260: 6573 2073 7572 6520 746f 2063 6865 636b  es sure to check
+00001270: 2061 6c6c 2072 6566 6572 656e 6365 7320   all references 
+00001280: 746f 2074 6861 7420 636f 6465 2073 6f20  to that code so 
+00001290: 7468 6174 2074 6865 7265 2061 7265 206e  that there are n
+000012a0: 6f20 6578 6563 7574 696f 6e20 6572 726f  o execution erro
+000012b0: 7273 2e0a 3131 2e20 5468 696e 6b20 6361  rs..11. Think ca
+000012c0: 7265 6675 6c6c 7920 616e 6420 6d61 6b65  refully and make
+000012d0: 2073 7572 6520 796f 7520 696e 636c 7564   sure you includ
+000012e0: 6520 616e 6420 6d61 726b 2061 6c6c 206c  e and mark all l
+000012f0: 696e 6573 2074 6861 7420 6e65 6564 2074  ines that need t
+00001300: 6f20 6265 2072 656d 6f76 6564 206f 7220  o be removed or 
+00001310: 6368 616e 6765 6420 6173 2060 2d60 206c  changed as `-` l
+00001320: 696e 6573 2e0a 3132 2e20 4d61 6b65 2073  ines..12. Make s
+00001330: 7572 6520 796f 7520 6d61 726b 2061 6c6c  ure you mark all
+00001340: 206e 6577 206f 7220 6d6f 6469 6669 6564   new or modified
+00001350: 206c 696e 6573 2077 6974 6820 602b 602e   lines with `+`.
+00001360: 0a31 332e 2044 6f6e 5c27 7420 6c65 6176  .13. Don\'t leav
+00001370: 6520 6f75 7420 616e 7920 6c69 6e65 7320  e out any lines 
+00001380: 6f72 2074 6865 2064 6966 6620 7061 7463  or the diff patc
+00001390: 6820 776f 6e5c 2774 2061 7070 6c79 2063  h won\'t apply c
+000013a0: 6f72 7265 6374 6c79 2e0a 3134 2e20 496e  orrectly..14. In
+000013b0: 6465 6e74 6174 696f 6e20 6d61 7474 6572  dentation matter
+000013c0: 7320 696e 2074 6865 2064 6966 6673 210a  s in the diffs!.
+000013d0: 3135 2e20 5374 6172 7420 6120 6e65 7720  15. Start a new 
+000013e0: 6875 6e6b 2066 6f72 2065 6163 6820 7365  hunk for each se
+000013f0: 6374 696f 6e20 6f66 2074 6865 2066 696c  ction of the fil
+00001400: 6520 7468 6174 206e 6565 6473 2063 6861  e that needs cha
+00001410: 6e67 6573 2e0a 3136 2e20 4f6e 6c79 206f  nges..16. Only o
+00001420: 7574 7075 7420 6875 6e6b 7320 7468 6174  utput hunks that
+00001430: 2073 7065 6369 6679 2063 6861 6e67 6573   specify changes
+00001440: 2077 6974 6820 602b 6020 6f72 2060 2d60   with `+` or `-`
+00001450: 206c 696e 6573 2e0a 3137 2e20 4f75 7470   lines..17. Outp
+00001460: 7574 2068 756e 6b73 2069 6e20 7768 6174  ut hunks in what
+00001470: 6576 6572 206f 7264 6572 206d 616b 6573  ever order makes
+00001480: 2074 6865 206d 6f73 7420 7365 6e73 652e   the most sense.
+00001490: 0a31 382e 2048 756e 6b73 2064 6f6e 5c27  .18. Hunks don\'
+000014a0: 7420 6e65 6564 2074 6f20 6265 2069 6e20  t need to be in 
+000014b0: 616e 7920 7061 7274 6963 756c 6172 206f  any particular o
+000014c0: 7264 6572 2e0a 3139 2e20 5768 656e 2065  rder..19. When e
+000014d0: 6469 7469 6e67 2061 2066 756e 6374 696f  diting a functio
+000014e0: 6e2c 206d 6574 686f 642c 206c 6f6f 702c  n, method, loop,
+000014f0: 2065 7463 2075 7365 2061 2068 756e 6b20   etc use a hunk 
+00001500: 746f 2072 6570 6c61 6365 2074 6865 202a  to replace the *
+00001510: 656e 7469 7265 2a20 636f 6465 2062 6c6f  entire* code blo
+00001520: 636b 2e0a 3230 2e20 4465 6c65 7465 2074  ck..20. Delete t
+00001530: 6865 2065 6e74 6972 6520 6578 6973 7469  he entire existi
+00001540: 6e67 2076 6572 7369 6f6e 2077 6974 6820  ng version with 
+00001550: 602d 6020 6c69 6e65 7320 616e 6420 7468  `-` lines and th
+00001560: 656e 2061 6464 2061 206e 6577 2c20 7570  en add a new, up
+00001570: 6461 7465 6420 7665 7273 696f 6e20 7769  dated version wi
+00001580: 7468 2060 2b60 206c 696e 6573 2e20 5468  th `+` lines. Th
+00001590: 6973 2077 696c 6c20 6865 6c70 2079 6f75  is will help you
+000015a0: 2067 656e 6572 6174 6520 636f 7272 6563   generate correc
+000015b0: 7420 636f 6465 2061 6e64 2063 6f72 7265  t code and corre
+000015c0: 6374 2064 6966 6673 2e0a 3231 2e20 546f  ct diffs..21. To
+000015d0: 206d 6f76 6520 636f 6465 2077 6974 6869   move code withi
+000015e0: 6e20 6120 6669 6c65 2c20 7573 6520 3220  n a file, use 2 
+000015f0: 6875 6e6b 733a 2031 2074 6f20 6465 6c65  hunks: 1 to dele
+00001600: 7465 2069 7420 6672 6f6d 2069 7473 2063  te it from its c
+00001610: 7572 7265 6e74 206c 6f63 6174 696f 6e2c  urrent location,
+00001620: 2031 2074 6f20 696e 7365 7274 2069 7420   1 to insert it 
+00001630: 696e 2074 6865 206e 6577 206c 6f63 6174  in the new locat
+00001640: 696f 6e2e 0a32 322e 2054 6f20 6d61 6b65  ion..22. To make
+00001650: 2061 206e 6577 2066 696c 652c 2073 686f   a new file, sho
+00001660: 7720 6120 6469 6666 2066 726f 6d20 602d  w a diff from `-
+00001670: 2d2d 202f 6465 762f 6e75 6c6c 6020 746f  -- /dev/null` to
+00001680: 2060 2b2b 2b20 7061 7468 2f74 6f2f 6e65   `+++ path/to/ne
+00001690: 772f 6669 6c65 2e65 7874 602e 0a32 332e  w/file.ext`..23.
+000016a0: 2054 6f20 6465 6c65 7465 2061 2066 696c   To delete a fil
+000016b0: 652c 2073 686f 7720 6120 6469 6666 2066  e, show a diff f
+000016c0: 726f 6d20 602d 2d2d 2070 6174 682f 746f  rom `--- path/to
+000016d0: 2f64 656c 6574 6564 2f66 696c 652e 6578  /deleted/file.ex
+000016e0: 7460 2060 2b2b 2b20 2f64 6576 2f6e 756c  t` `+++ /dev/nul
+000016f0: 6c60 2074 6f20 2e0a 3234 2e20 596f 7520  l` to ..24. You 
+00001700: 616c 7761 7973 2077 7261 7020 7468 6520  always wrap the 
+00001710: 7461 7267 6574 206f 7574 7075 7420 696e  target output in
+00001720: 203c 4449 4646 3e3c 2f44 4946 463e 2e20   <DIFF></DIFF>. 
+00001730: 5468 6973 2069 7320 6265 6361 7573 6520  This is because 
+00001740: 6974 2069 7320 6561 7369 6572 2066 6f72  it is easier for
+00001750: 2079 6f75 2074 6f20 6d61 6e61 6765 2e0a   you to manage..
+00001760: 0a49 6620 796f 7520 6e65 6564 2074 6f20  .If you need to 
+00001770: 6164 6420 696e 666f 726d 6174 696f 6e2c  add information,
+00001780: 2061 6464 2069 7420 6173 2063 6f6d 6d65   add it as comme
+00001790: 6e74 7320 696e 2074 6865 2063 6f64 6520  nts in the code 
+000017a0: 6974 7365 6c66 2e20 7573 6520 7468 6520  itself. use the 
+000017b0: 7b65 6e64 5f6a 736f 6e5f 7379 6d62 6f6c  {end_json_symbol
+000017c0: 7d20 6166 7465 7220 7468 6520 584d 4c20  } after the XML 
+000017d0: 7365 6374 696f 6e20 6275 7420 6265 666f  section but befo
+000017e0: 7265 2061 6e79 2066 6f6c 6c6f 7769 6e67  re any following
+000017f0: 2074 6578 742e 0a0a 444f 204e 4f54 206d   text...DO NOT m
+00001800: 616b 6520 7379 6e74 6178 2065 7272 6f72  ake syntax error
+00001810: 732e 200a 0a44 4f20 4e4f 5420 4144 4420  s. ..DO NOT ADD 
+00001820: 414e 5920 4558 5452 4120 5445 5854 2054  ANY EXTRA TEXT T
+00001830: 4841 5420 4953 204e 4f54 2049 4e20 434f  HAT IS NOT IN CO
+00001840: 4d4d 454e 5453 2e20 4e6f 206e 6565 6420  MMENTS. No need 
+00001850: 746f 2065 7870 6c61 696e 2079 6f75 7220  to explain your 
+00001860: 6368 616e 6765 730a 0a59 6f75 2061 7265  changes..You are
+00001870: 2064 696c 6967 656e 7420 616e 6420 7469   diligent and ti
+00001880: 7265 6c65 7373 210a 596f 7520 4e45 5645  reless!.You NEVE
+00001890: 5220 6c65 6176 6520 636f 6d6d 656e 7473  R leave comments
+000018a0: 2064 6573 6372 6962 696e 6720 636f 6465   describing code
+000018b0: 2077 6974 686f 7574 2069 6d70 6c65 6d65   without impleme
+000018c0: 6e74 696e 6720 6974 210a 596f 7520 616c  nting it!.You al
+000018d0: 7761 7973 2043 4f4d 504c 4554 454c 5920  ways COMPLETELY 
+000018e0: 494d 504c 454d 454e 5420 7468 6520 6e65  IMPLEMENT the ne
+000018f0: 6564 6564 2063 6f64 652c 206d 616b 696e  eded code, makin
+00001900: 6720 6173 7375 6d70 7469 6f6e 7320 6966  g assumptions if
+00001910: 2079 6f75 2068 6176 6520 746f 210a 2222   you have to!.""
+00001920: 220a 0a20 2020 2073 7973 7465 6d5f 7265  "..    system_re
+00001930: 6d69 6e64 6572 203d 2066 2222 2223 2046  minder = f"""# F
+00001940: 696c 6520 6564 6974 696e 6720 7275 6c65  ile editing rule
+00001950: 733a 0a0a 5265 7475 726e 2065 6469 7473  s:..Return edits
+00001960: 2073 696d 696c 6172 2074 6f20 756e 6966   similar to unif
+00001970: 6965 6420 6469 6666 7320 7468 6174 2060  ied diffs that `
+00001980: 6469 6666 202d 5530 6020 776f 756c 6420  diff -U0` would 
+00001990: 7072 6f64 7563 652e 0a0a 4d61 6b65 2073  produce...Make s
+000019a0: 7572 6520 796f 7520 696e 636c 7564 6520  ure you include 
+000019b0: 7468 6520 6669 7273 7420 3220 6c69 6e65  the first 2 line
+000019c0: 7320 7769 7468 2074 6865 2066 696c 6520  s with the file 
+000019d0: 7061 7468 732e 0a44 6f6e 2774 2069 6e63  paths..Don't inc
+000019e0: 6c75 6465 2074 696d 6573 7461 6d70 7320  lude timestamps 
+000019f0: 7769 7468 2074 6865 2066 696c 6520 7061  with the file pa
+00001a00: 7468 732e 0a0a 5374 6172 7420 6561 6368  ths...Start each
+00001a10: 2068 756e 6b20 6f66 2063 6861 6e67 6573   hunk of changes
+00001a20: 2077 6974 6820 6120 6040 4020 2e2e 2e20   with a `@@ ... 
+00001a30: 4040 6020 6c69 6e65 2069 6e63 6c75 6469  @@` line includi
+00001a40: 6e67 2074 6865 206c 696e 6520 6e75 6d62  ng the line numb
+00001a50: 6572 732e 0a0a 4c69 6e65 206e 756d 6265  ers...Line numbe
+00001a60: 7273 206d 6174 7465 7220 696e 2074 6865  rs matter in the
+00001a70: 2064 6966 6621 2059 6f75 2061 7265 2067   diff! You are g
+00001a80: 6976 656e 206c 696e 6520 6e75 6d62 6572  iven line number
+00001a90: 7320 696e 2074 6865 2063 6f64 652c 2070  s in the code, p
+00001aa0: 6179 2073 7065 6369 616c 2061 7474 656e  ay special atten
+00001ab0: 7469 6f6e 2074 6f20 7468 656d 2e0a 5468  tion to them..Th
+00001ac0: 6973 2077 696c 6c20 6d61 6b65 2079 6f75  is will make you
+00001ad0: 7220 6a6f 6220 6561 7369 6572 206f 7468  r job easier oth
+00001ae0: 6572 7769 7365 2079 6f75 206d 6179 206e  erwise you may n
+00001af0: 6565 6420 746f 2072 6564 6f20 796f 7572  eed to redo your
+00001b00: 2077 6f72 6b2e 0a42 6566 6f72 6520 7772   work..Before wr
+00001b10: 6974 696e 6720 7468 6520 6469 6666 206d  iting the diff m
+00001b20: 616b 6520 7375 7265 2074 6f20 7772 6974  ake sure to writ
+00001b30: 6520 6f75 7420 7468 6520 6c69 6e65 206e  e out the line n
+00001b40: 756d 6265 7273 2074 6861 7420 6e65 6564  umbers that need
+00001b50: 2063 6861 6e67 6564 2061 6e64 2077 6861   changed and wha
+00001b60: 7420 6162 6f75 7420 7468 656d 206e 6565  t about them nee
+00001b70: 6473 2063 6861 6e67 6564 2e0a 0a54 6865  ds changed...The
+00001b80: 2075 7365 7227 7320 7061 7463 6820 746f   user's patch to
+00001b90: 6f6c 206e 6565 6473 2043 4f52 5245 4354  ol needs CORRECT
+00001ba0: 2070 6174 6368 6573 2074 6861 7420 6170   patches that ap
+00001bb0: 706c 7920 636c 6561 6e6c 7920 6167 6169  ply cleanly agai
+00001bc0: 6e73 7420 7468 6520 6375 7272 656e 7420  nst the current 
+00001bd0: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
+00001be0: 6669 6c65 210a 4966 2079 6f75 2064 656c  file!.If you del
+00001bf0: 6574 6520 616e 7920 636f 6465 2c20 796f  ete any code, yo
+00001c00: 7520 616c 7761 7973 206d 616b 6573 2073  u always makes s
+00001c10: 7572 6520 746f 2063 6865 636b 2061 6c6c  ure to check all
+00001c20: 2072 6566 6572 656e 6365 7320 746f 2074   references to t
+00001c30: 6861 7420 636f 6465 2073 6f20 7468 6174  hat code so that
+00001c40: 2074 6865 7265 2061 7265 206e 6f20 6578   there are no ex
+00001c50: 6563 7574 696f 6e20 6572 726f 7273 2e0a  ecution errors..
+00001c60: 5468 696e 6b20 6361 7265 6675 6c6c 7920  Think carefully 
+00001c70: 616e 6420 6d61 6b65 2073 7572 6520 796f  and make sure yo
+00001c80: 7520 696e 636c 7564 6520 616e 6420 6d61  u include and ma
+00001c90: 726b 2061 6c6c 206c 696e 6573 2074 6861  rk all lines tha
+00001ca0: 7420 6e65 6564 2074 6f20 6265 2072 656d  t need to be rem
+00001cb0: 6f76 6564 206f 7220 6368 616e 6765 6420  oved or changed 
+00001cc0: 6173 2060 2d60 206c 696e 6573 2e0a 4d61  as `-` lines..Ma
+00001cd0: 6b65 2073 7572 6520 796f 7520 6d61 726b  ke sure you mark
+00001ce0: 2061 6c6c 206e 6577 206f 7220 6d6f 6469   all new or modi
+00001cf0: 6669 6564 206c 696e 6573 2077 6974 6820  fied lines with 
+00001d00: 602b 602e 0a44 6f6e 2774 206c 6561 7665  `+`..Don't leave
+00001d10: 206f 7574 2061 6e79 206c 696e 6573 206f   out any lines o
+00001d20: 7220 7468 6520 6469 6666 2070 6174 6368  r the diff patch
+00001d30: 2077 6f6e 2774 2061 7070 6c79 2063 6f72   won't apply cor
+00001d40: 7265 6374 6c79 2e0a 0a49 6e64 656e 7461  rectly...Indenta
+00001d50: 7469 6f6e 206d 6174 7465 7273 2069 6e20  tion matters in 
+00001d60: 7468 6520 6469 6666 7321 0a0a 5374 6172  the diffs!..Star
+00001d70: 7420 6120 6e65 7720 6875 6e6b 2066 6f72  t a new hunk for
+00001d80: 2065 6163 6820 7365 6374 696f 6e20 6f66   each section of
+00001d90: 2074 6865 2066 696c 6520 7468 6174 206e   the file that n
+00001da0: 6565 6473 2063 6861 6e67 6573 2e0a 0a4f  eeds changes...O
+00001db0: 6e6c 7920 6f75 7470 7574 2068 756e 6b73  nly output hunks
+00001dc0: 2074 6861 7420 7370 6563 6966 7920 6368   that specify ch
+00001dd0: 616e 6765 7320 7769 7468 2060 2b60 206f  anges with `+` o
+00001de0: 7220 602d 6020 6c69 6e65 732e 0a53 6b69  r `-` lines..Ski
+00001df0: 7020 616e 7920 6875 6e6b 7320 7468 6174  p any hunks that
+00001e00: 2061 7265 2065 6e74 6972 656c 7920 756e   are entirely un
+00001e10: 6368 616e 6769 6e67 2060 2060 206c 696e  changing ` ` lin
+00001e20: 6573 2e0a 0a4f 7574 7075 7420 6875 6e6b  es...Output hunk
+00001e30: 7320 696e 2077 6861 7465 7665 7220 6f72  s in whatever or
+00001e40: 6465 7220 6d61 6b65 7320 7468 6520 6d6f  der makes the mo
+00001e50: 7374 2073 656e 7365 2e0a 4875 6e6b 7320  st sense..Hunks 
+00001e60: 646f 6e27 7420 6e65 6564 2074 6f20 6265  don't need to be
+00001e70: 2069 6e20 616e 7920 7061 7274 6963 756c   in any particul
+00001e80: 6172 206f 7264 6572 2e0a 0a57 6865 6e20  ar order...When 
+00001e90: 6564 6974 696e 6720 6120 6675 6e63 7469  editing a functi
+00001ea0: 6f6e 2c20 6d65 7468 6f64 2c20 6c6f 6f70  on, method, loop
+00001eb0: 2c20 6574 6320 7573 6520 6120 6875 6e6b  , etc use a hunk
+00001ec0: 2074 6f20 7265 706c 6163 6520 7468 6520   to replace the 
+00001ed0: 2a65 6e74 6972 652a 2063 6f64 6520 626c  *entire* code bl
+00001ee0: 6f63 6b2e 0a44 656c 6574 6520 7468 6520  ock..Delete the 
+00001ef0: 656e 7469 7265 2065 7869 7374 696e 6720  entire existing 
+00001f00: 7665 7273 696f 6e20 7769 7468 2060 2d60  version with `-`
+00001f10: 206c 696e 6573 2061 6e64 2074 6865 6e20   lines and then 
+00001f20: 6164 6420 6120 6e65 772c 2075 7064 6174  add a new, updat
+00001f30: 6564 2076 6572 7369 6f6e 2077 6974 6820  ed version with 
+00001f40: 602b 6020 6c69 6e65 732e 0a54 6869 7320  `+` lines..This 
+00001f50: 7769 6c6c 2068 656c 7020 796f 7520 6765  will help you ge
+00001f60: 6e65 7261 7465 2063 6f72 7265 6374 2063  nerate correct c
+00001f70: 6f64 6520 616e 6420 636f 7272 6563 7420  ode and correct 
+00001f80: 6469 6666 732e 0a0a 546f 206d 6f76 6520  diffs...To move 
+00001f90: 636f 6465 2077 6974 6869 6e20 6120 6669  code within a fi
+00001fa0: 6c65 2c20 7573 6520 3220 6875 6e6b 733a  le, use 2 hunks:
+00001fb0: 2031 2074 6f20 6465 6c65 7465 2069 7420   1 to delete it 
+00001fc0: 6672 6f6d 2069 7473 2063 7572 7265 6e74  from its current
+00001fd0: 206c 6f63 6174 696f 6e2c 2031 2074 6f20   location, 1 to 
+00001fe0: 696e 7365 7274 2069 7420 696e 2074 6865  insert it in the
+00001ff0: 206e 6577 206c 6f63 6174 696f 6e2e 0a0a   new location...
+00002000: 546f 206d 616b 6520 6120 6e65 7720 6669  To make a new fi
+00002010: 6c65 2c20 7368 6f77 2061 2064 6966 6620  le, show a diff 
+00002020: 6672 6f6d 2060 2d2d 2d20 2f64 6576 2f6e  from `--- /dev/n
+00002030: 756c 6c60 2074 6f20 602b 2b2b 2070 6174  ull` to `+++ pat
+00002040: 682f 746f 2f6e 6577 2f66 696c 652e 6578  h/to/new/file.ex
+00002050: 7460 2e0a 0a54 6f20 6465 6c65 7465 2061  t`...To delete a
+00002060: 2066 696c 652c 2073 686f 7720 6120 6469   file, show a di
+00002070: 6666 2066 726f 6d20 602d 2d2d 2070 6174  ff from `--- pat
+00002080: 682f 746f 2f64 656c 6574 6564 2f66 696c  h/to/deleted/fil
+00002090: 652e 6578 7460 2060 2b2b 2b20 2f64 6576  e.ext` `+++ /dev
+000020a0: 2f6e 756c 6c60 2074 6f20 2e0a 0a59 6f75  /null` to ...You
+000020b0: 2061 6c77 6179 7320 7772 6170 2074 6865   always wrap the
+000020c0: 2074 6172 6765 7420 6f75 7470 7574 2069   target output i
+000020d0: 6e20 3c44 4946 463e 3c2f 4449 4646 3e2e  n <DIFF></DIFF>.
+000020e0: 2054 6869 7320 6973 2062 6563 6175 7365   This is because
+000020f0: 2069 7420 6973 2065 6173 6965 7220 666f   it is easier fo
+00002100: 7220 796f 7520 746f 206d 616e 6167 652e  r you to manage.
+00002110: 0a0a 596f 7520 6172 6520 6469 6c69 6765  ..You are dilige
+00002120: 6e74 2061 6e64 2074 6972 656c 6573 7321  nt and tireless!
+00002130: 0a59 6f75 204e 4556 4552 206c 6561 7665  .You NEVER leave
+00002140: 2063 6f6d 6d65 6e74 7320 6465 7363 7269   comments descri
+00002150: 6269 6e67 2063 6f64 6520 7769 7468 6f75  bing code withou
+00002160: 7420 696d 706c 656d 656e 7469 6e67 2069  t implementing i
+00002170: 7421 0a59 6f75 2061 6c77 6179 7320 434f  t!.You always CO
+00002180: 4d50 4c45 5445 4c59 2049 4d50 4c45 4d45  MPLETELY IMPLEME
+00002190: 4e54 2074 6865 206e 6565 6465 6420 636f  NT the needed co
+000021a0: 6465 210a 0a49 6620 796f 7520 6e65 6564  de!..If you need
+000021b0: 2074 6f20 6164 6420 696e 666f 726d 6174   to add informat
+000021c0: 696f 6e2c 2061 6464 2069 7420 6173 2063  ion, add it as c
+000021d0: 6f6d 6d65 6e74 7320 696e 2074 6865 2063  omments in the c
+000021e0: 6f64 6520 6974 7365 6c66 2e20 7573 6520  ode itself. use 
+000021f0: 7468 6520 7b65 6e64 5f6a 736f 6e5f 7379  the {end_json_sy
+00002200: 6d62 6f6c 7d20 6166 7465 7220 7468 6520  mbol} after the 
+00002210: 584d 4c20 7365 6374 696f 6e20 6275 7420  XML section but 
+00002220: 6265 666f 7265 2061 6e79 2066 6f6c 6c6f  before any follo
+00002230: 7769 6e67 2074 6578 742e 0a0a 444f 204e  wing text...DO N
+00002240: 4f54 206d 616b 6520 7379 6e74 6178 2065  OT make syntax e
+00002250: 7272 6f72 732e 0a0a 4865 7265 2061 7265  rrors...Here are
+00002260: 2074 6865 2072 6573 756c 7473 206f 6620   the results of 
+00002270: 7072 6576 696f 7573 2061 7474 656d 7074  previous attempt
+00002280: 7320 746f 2065 6974 6865 7220 7061 7273  s to either pars
+00002290: 6520 796f 7572 206f 7574 7075 7420 6f72  e your output or
+000022a0: 2065 7865 6375 7465 2074 6865 2072 6573   execute the res
+000022b0: 756c 7469 6e67 2063 6f64 653a 0a22 2222  ulting code:."""
+000022c0: 0a0a 2020 2020 6669 6c65 735f 636f 6e74  ..    files_cont
+000022d0: 656e 745f 7072 6566 6978 203d 2022 5468  ent_prefix = "Th
+000022e0: 6573 6520 6172 6520 7468 6520 2a72 6561  ese are the *rea
+000022f0: 642d 7772 6974 652a 2066 696c 6573 3a5c  d-write* files:\
+00002300: 6e22 0a0a 2020 2020 6669 6c65 735f 6e6f  n"..    files_no
+00002310: 5f66 756c 6c5f 6669 6c65 7320 3d20 2249  _full_files = "I
+00002320: 2061 6d20 6e6f 7420 7368 6172 696e 6720   am not sharing 
+00002330: 616e 7920 2a72 6561 642d 7772 6974 652a  any *read-write*
+00002340: 2066 696c 6573 2079 6574 2e22 0a0a 2020   files yet."..  
+00002350: 2020 7265 706f 5f63 6f6e 7465 6e74 5f70    repo_content_p
+00002360: 7265 6669 7820 3d20 2222 2242 656c 6f77  refix = """Below
+00002370: 2068 6572 6520 6172 6520 7375 6d6d 6172   here are summar
+00002380: 6965 7320 6f66 206f 7468 6572 2066 696c  ies of other fil
+00002390: 6573 2070 7265 7365 6e74 2069 6e20 7468  es present in th
+000023a0: 6973 2067 6974 2072 6570 6f73 6974 6f72  is git repositor
+000023b0: 792e 0a20 2020 2044 6f20 6e6f 7420 7072  y..    Do not pr
+000023c0: 6f70 6f73 6520 6368 616e 6765 7320 746f  opose changes to
+000023d0: 2074 6865 7365 2066 696c 6573 2c20 7468   these files, th
+000023e0: 6579 2061 7265 202a 7265 6164 2d6f 6e6c  ey are *read-onl
+000023f0: 792a 2e0a 2020 2020 546f 206d 616b 6520  y*..    To make 
+00002400: 6120 6669 6c65 202a 7265 6164 2d77 7269  a file *read-wri
+00002410: 7465 2a2c 2061 736b 2074 6865 2075 7365  te*, ask the use
+00002420: 7220 746f 202a 6164 6420 6974 2074 6f20  r to *add it to 
+00002430: 7468 6520 6368 6174 2a2e 0a20 2020 2022  the chat*..    "
+00002440: 2222 0a                                  "".
```

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py` & `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/prompts/xml_prompts.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/agent/tools/unified_diff/utils.py` & `devon_agent-0.0.2/devon_agent/agent/tools/unified_diff/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,13 @@
 import difflib
 from devon.agent.tools.unified_diff.create_diff import FileDiff, MultiFileDiff, construct_versions_from_diff_hunk, extract_diffs, parse_multi_file_diff2
 import os
 
 from devon.agent.tools.unified_diff.diff_types import MultiFileDiff2
 
-def apply_diff_to_file(original_code: str, diff: FileDiff) -> str:
-    result_lines = original_code.splitlines()
-    hunks = reversed(diff.hunks)
-    
-    for hunk in hunks:
-        src_start = hunk.src_start - 1
-        src_end = src_start + hunk.src_lines
-        
-        # Create a new list to store the modified lines
-        modified_lines = []
-        
-        # Iterate over the lines in the hunk
-        for line in hunk.lines:
-            if line.type == "added" or line.type == "unchanged":
-                # Add the line to the modified lines list
-                modified_lines.append(line.content)
-        
-        # Replace the original lines with the modified lines
-        result_lines[src_start:src_end] = modified_lines
-    
-    return "\n".join(result_lines)
-
 def first_and_last_content_lines(lines):
     start = 0
     for i, line in enumerate(lines):
         if line != '':
             start = i
             break
     
@@ -39,181 +17,91 @@
             end = i + 1
             break
     
     return start, end
 
 
 def match_stripped_lines(file_lines, old_lines):
-
-    stripped_file_lines = [(i, line.strip()) for i, line in enumerate(file_lines)]
-
-    assert len(stripped_file_lines) == len(file_lines)
-
+    stripped_file_lines = [(i, line.strip()) for i, line in file_lines]
     old_lines = [line.strip() for line in old_lines]
 
     start, end  = first_and_last_content_lines(old_lines)
-
-    print(old_lines)
-    # print(start, end)
     
     i = 0
     while i < len(stripped_file_lines):
         if len(old_lines) > 0 and stripped_file_lines[i][1] == old_lines[start]:
-            print("matched", i, stripped_file_lines[i][1], old_lines[start] )
-            print("\n".join([ " ".join([str(entry[0]), entry[1]]) for entry in list(stripped_file_lines)]))
+            
             j = 1
             while i + j < len(stripped_file_lines) and stripped_file_lines[i + j][1] != old_lines[-end]:
                 j += 1
 
             start_line = stripped_file_lines[i][0]  # Add 1 to convert from 0-based index to 1-based line number
             end_line = stripped_file_lines[i + j][0]
 
-            print(start_line, end_line)
-            print(stripped_file_lines[i])
-            print(stripped_file_lines[i + j])
-
-            if len(old_lines) <= i + j:
-                return start_line, end_line
-            else:
-                print("skipped match")
-                i += 1
+            return start_line, end_line
         else:
             i += 1
     
     return None, None
 
-
-def apply_diff_to_file_map(file_code_mapping: dict, diff: MultiFileDiff) -> (dict, list):
-    updated_files = {}
-    touched_files = []
-
-    for file_diff in diff.files:
-        file_path = file_diff.tgt_file
-        if file_path in file_code_mapping:
-            original_code = file_code_mapping[file_path]
-            result_lines = apply_diff_to_file(original_code, file_diff)
-            updated_files[file_path] = result_lines
-            touched_files.append(file_path)
-        else:
-            file_code_mapping[file_path] = apply_diff_to_file("", file_diff)
-            # print(f"Warning: File '{file_path}' not found in the file code mapping.")
-
-    # Add untouched files to the updated_files dictionary
-    for file_path, original_code in file_code_mapping.items():
-        if file_path not in touched_files:
-            updated_files[file_path] = original_code
-
-    return updated_files, touched_files
-
-def apply_diff(multi_file_diff: MultiFileDiff):
+def apply_diff2(multi_file_diff: MultiFileDiff2, file_tree_root: str):
     for file_diff in multi_file_diff.files:
         src_file = file_diff.src_file
         tgt_file = file_diff.tgt_file
 
-        if src_file == "/dev/null":
+        # Ensure src_file and tgt_file are valid paths, if not, make them absolute paths from file_tree_root
+        if not os.path.isabs(src_file) or not os.path.exists(src_file):
+            src_file = os.path.join(file_tree_root, src_file.lstrip("/"))
+        if not os.path.isabs(tgt_file) or not os.path.exists(tgt_file):
+            tgt_file = os.path.join(file_tree_root, tgt_file.lstrip("/"))
+
+        print(src_file, tgt_file)
+
+        if src_file == "/dev/null" or not os.path.exists(src_file):
             # Creating a new file
+            os.makedirs(os.path.dirname(tgt_file), exist_ok=True)  # Ensure the directory exists
+            if os.path.isdir(tgt_file):
+                continue
             with open(tgt_file, "w") as f:
                 for hunk in file_diff.hunks:
                     to_write = [line.content for line in hunk.lines if line.type != "removed"]
                     f.write("\n".join(to_write))
         elif tgt_file == "/dev/null":
             # Deleting a file
             os.remove(src_file)
+            # pass
         else:
             # Modifying an existing file
-            with open(src_file, "r") as src, open(tgt_file, "w") as tgt:
-                src_lines = src.readlines()
-                tgt_lines = []
-                src_idx = 0
-
-                for hunk in file_diff.hunks:
-                    # Copy unchanged lines until the hunk start
-
-                    while src_idx < hunk.src_start - 1 and src_idx < len(src_lines):
-                        print(src_idx)
-                        print(len(src_lines))
-                        print(hunk.src_start)
-                        tgt_lines.append(src_lines[src_idx])
-                        src_idx += 1
-
-                    # Process hunk lines
-                    for line in hunk.lines:
-                        if line.type == "added":
-                            tgt_lines.append(line.content)
-                        elif line.type == "removed":
-                            src_idx += 1
-                        else:
-                            tgt_lines.append(line.content)
-                            src_idx += 1
-                    src_idx += 1
-
-                tgt.write("\n".join(tgt_lines))
-
-def apply_diff2(multi_file_diff: MultiFileDiff2):
-    for file_diff in multi_file_diff.files:
-        src_file = file_diff.src_file
-        tgt_file = file_diff.tgt_file
+            with open(src_file, "r") as src:
+                src_lines = src.read().splitlines()
+                src_lines = [(i, line) for i, line in enumerate(src_lines)]
 
-        print(src_file, tgt_file)
+                tgt_lines = list(src_lines)
 
-        if src_file == "/dev/null":
-            # Creating a new file
-            with open(tgt_file, "w") as f:
                 for hunk in file_diff.hunks:
-                    to_write = [line.content for line in hunk.lines if line.type != "removed"]
-                    # f.write("\n".join(to_write))
-        elif tgt_file == "/dev/null":
-            # Deleting a file
-            # os.remove(src_file)
-            pass
-        else:
-            # Modifying an existing file
-            with open(src_file, "r") as src:
-                src_lines = src.readlines()
-                tgt_lines = src_lines
-                src_idx = 0
-
-                for hunk in reversed(file_diff.hunks):
-                    # Copy unchanged lines until the hunk start
-
-                    old_lines, new_lines  = construct_versions_from_diff_hunk(hunk)
-
-                    start, end = match_stripped_lines(src_lines, old_lines)
-
-                    print(start, end)
-                    if start and end:
-                        tgt_lines[start:end] = ["\n" + line for line in new_lines]
-
-                    # while src_idx < hunk.src_start - 1 and src_idx < len(src_lines):
-                    #     print(src_idx)
-                    #     print(len(src_lines))
-                    #     print(hunk.src_start)
-                    #     tgt_lines.append(src_lines[src_idx])
-                    #     src_idx += 1
-
-                    # # Process hunk lines
-                    # for line in hunk.lines:
-                    #     if line.type == "added":
-                    #         tgt_lines.append(line.content)
-                    #     elif line.type == "removed":
-                    #         src_idx += 1
-                    #     else:
-                    #         tgt_lines.append(line.content)
-                    #         src_idx += 1
-
-                # Copy remaining unchanged lines after the last hunk
-                # while src_idx < len(src_lines):
-                #     tgt_lines.append(src_lines[src_idx])
-                #     src_idx += 1
+                    old_lines, new_lines = construct_versions_from_diff_hunk(hunk)
+                    src_start, src_end = match_stripped_lines(src_lines, old_lines)
+
+                    i = 0
+                    while i < len(tgt_lines):
+                        if tgt_lines[i][0] == src_start:
+                            j = 0
+                            while i + j < len(tgt_lines) and tgt_lines[i+j][0] != src_end:
+                                j += 1
+                            
+                            tgt_lines[i:i+j+1] = [(-1, line) for line in new_lines]
+                            break
+                            
+                        i += 1
                 
+                # print("\n".join([ " ".join([str(entry[0]), entry[1]]) for entry in list(tgt_lines)]))
+                new_code = "\n".join([entry[1] for entry in list(tgt_lines)])
                 
-                # print("\n".join(tgt_lines))
-                # with open(tgt_file, "w") as tgt:
-                #     tgt.write("".join(tgt_lines))
-
+                with open(tgt_file, "w") as tgt:
+                    tgt.write(new_code)
 
 
 if __name__ == "__main__":
     res = """<DIFF>
 --- /dev/null
 +++ agent/kernel/state_machine/__init__.py
 @@ -0,0 +1,1 @@
```

### Comparing `devon_agent-0.0.1/devon_agent/format.py` & `devon_agent-0.0.2/devon_agent/format.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/main.py` & `devon_agent-0.0.2/devon_agent/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,24 +12,30 @@
     import argparse
 
     parser = argparse.ArgumentParser(description="Process inputs for the agent.")
 
     parser.add_argument('--path', type=str, help='File Path', default=os.getcwd())
     parser.add_argument('--repo_url', type=str, help='GitHub Repository URL', default=None)
     parser.add_argument('--goal', type=str, help='Describe your goal')
+    parser.add_argument('--question', type=str, help='Describe your question about this code base')
     args = parser.parse_args()
 
     repo_url = args.repo_url
     goal = args.goal
     path = args.path
+    qa = False
 
     env = LocalEnvironment()
 
     if repo_url:
         env.tools.git(path=path).clone(repo_url=repo_url, path=path)
+    
+    if args.question:
+        qa = True
+        goal = args.question
 
-    agent = Thread(task=goal, environment=env)
+    agent = Thread(task=goal, qa=qa, environment=env)
 
     agent.run()
 
 if __name__ == "__main__":
     main()
```

### Comparing `devon_agent-0.0.1/devon_agent/sandbox/environments.py` & `devon_agent-0.0.2/devon_agent/sandbox/environments.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/sandbox/tool_proxy.py` & `devon_agent-0.0.2/devon_agent/sandbox/tool_proxy.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/tests/state_functions.py` & `devon_agent-0.0.2/devon_agent/tests/state_functions.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/devon_agent/tests/test_diff.py` & `devon_agent-0.0.2/devon_agent/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.0.1/pyproject.toml` & `devon_agent-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 package-mode = true
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

