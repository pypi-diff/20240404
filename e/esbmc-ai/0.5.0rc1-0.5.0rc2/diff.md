# Comparing `tmp/esbmc_ai-0.5.0rc1.tar.gz` & `tmp/esbmc_ai-0.5.0rc2.tar.gz`

## Comparing `esbmc_ai-0.5.0rc1.tar` & `esbmc_ai-0.5.0rc2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/config.py
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/README.md
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/config.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/README.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/config.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/esbmc_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,30 +66,33 @@
     else:
         return None
 
 
 def get_clang_err_line(clang_output: str) -> Optional[int]:
     """For when the code does not compile, gets the error line reported in the clang
     output. This is useful for `esbmc_output_type single`"""
-    # TODO Test me
     lines: list[str] = clang_output.splitlines()
     for line in lines:
         # Find the first line containing a filename along with error.
         line_split: list[str] = line.split(":")
         if len(line_split) < 4:
-            return None
+            continue
         # Check for the filename
         if line_split[0].endswith(".c") and " error" in line_split[3]:
             return int(line_split[1])
 
     return None
 
 
 def get_clang_err_line_index(clang_output: str) -> Optional[int]:
-    return get_clang_err_line(clang_output)
+    line: Optional[int] = get_clang_err_line(clang_output)
+    if line:
+        return line - 1
+    else:
+        return None
 
 
 def esbmc(path: str, esbmc_params: list, timeout: Optional[float] = None):
     """Exit code will be 0 if verification successful, 1 if verification
     failed. And any other number for compilation error/general errors."""
     # Build parameters
     esbmc_cmd = [config.esbmc_path]
```

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/logging.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/logging.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/solution_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,16 @@
             assert code_start != -1
 
             code_end: int = solution[::-1].index("```")
             assert code_start != -1
 
             # -4 = 3 backticks and also the \n before the backticks.
             code_end: int = len(solution) - 4 - code_end
-            assert code_start <= code_end
+            # +1 because of edge cases as in test_get_code_from_solution
+            assert code_start <= code_end + 1
 
             solution = solution[code_start:code_end]
         except (ValueError, AssertionError):
             pass
         return solution
 
     def update_state(
@@ -182,18 +183,19 @@
 
         solution = SolutionGenerator.get_code_from_solution(solution)
 
         # If source code passed to LLM is formatted then we need to recombine to
         # full source code before giving to ESBMC
         match self.source_code_format:
             case "single":
-                err_line: Optional[int] = get_source_code_err_line_idx(
-                    self.esbmc_output
-                )
+                # Get source code error line from esbmc output
+                line: Optional[int] = get_source_code_err_line_idx(self.esbmc_output)
+                if not line:
+                    # Check if it parses
+                    line = get_clang_err_line_index(self.esbmc_output)
+
                 assert (
-                    err_line
+                    line
                 ), "fix code command: error line could not be found to apply brutal patch replacement"
-                solution = apply_line_patch(
-                    self.source_code_raw, solution, err_line, err_line
-                )
+                solution = apply_line_patch(self.source_code_raw, solution, line, line)
 
         return solution, response.finish_reason
```

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/commands/fix_code_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0rc2/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/.gitignore` & `esbmc_ai-0.5.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/LICENSE` & `esbmc_ai-0.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/README.md` & `esbmc_ai-0.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/pyproject.toml` & `esbmc_ai-0.5.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc1/PKG-INFO` & `esbmc_ai-0.5.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0rc1
+Version: 0.5.0rc2
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

