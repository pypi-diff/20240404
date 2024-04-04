# Comparing `tmp/esbmc_ai-0.5.0rc0.tar.gz` & `tmp/esbmc_ai-0.5.0rc1.tar.gz`

## Comparing `esbmc_ai-0.5.0rc0.tar` & `esbmc_ai-0.5.0rc1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/config.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/README.md
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/pyproject.toml
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc0/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/config.py
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/README.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc1/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/config.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/esbmc_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
     """For when the code does not compile, gets the error line reported in the clang
     output. This is useful for `esbmc_output_type single`"""
     # TODO Test me
     lines: list[str] = clang_output.splitlines()
     for line in lines:
         # Find the first line containing a filename along with error.
         line_split: list[str] = line.split(":")
+        if len(line_split) < 4:
+            return None
         # Check for the filename
         if line_split[0].endswith(".c") and " error" in line_split[3]:
             return int(line_split[1])
 
     return None
```

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/logging.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/logging.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/solution_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,14 +148,22 @@
             assert code_start <= code_end
 
             solution = solution[code_start:code_end]
         except (ValueError, AssertionError):
             pass
         return solution
 
+    def update_state(
+        self, source_code: Optional[str] = None, esbmc_output: Optional[str] = None
+    ) -> None:
+        if source_code:
+            self.source_code_raw = source_code
+        if esbmc_output:
+            self.esbmc_output = esbmc_output
+
     def generate_solution(self) -> tuple[str, FinishReason]:
         self.push_to_message_stack(HumanMessage(content=self.initial_prompt))
 
         # Format source code
         source_code_formatted: str = get_source_code_formatted(
             source_code_format=self.source_code_format,
             source_code=self.source_code_raw,
@@ -184,10 +192,8 @@
                 assert (
                     err_line
                 ), "fix code command: error line could not be found to apply brutal patch replacement"
                 solution = apply_line_patch(
                     self.source_code_raw, solution, err_line, err_line
                 )
 
-        # Remember it for next cycle
-        self.source_code_raw = solution
         return solution, response.finish_reason
```

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/commands/fix_code_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,61 +83,61 @@
 
         print()
 
         max_retries: int = config.fix_code_max_attempts
         for idx in range(max_retries):
             # Get a response. Use while loop to account for if the message stack
             # gets full, then need to compress and retry.
-            llm_solution: str = ""
             while True:
                 # Generate AI solution
                 self.anim.start("Generating Solution... Please Wait")
                 llm_solution, finish_reason = solution_generator.generate_solution()
                 self.anim.stop()
                 if finish_reason == FinishReason.length:
                     self.anim.start("Compressing message stack... Please Wait")
                     solution_generator.compress_message_stack()
                     self.anim.stop()
                 else:
+                    source_code = llm_solution
                     break
 
             # Print verbose lvl 2
             printvv("\nGeneration:")
             print_horizontal_line(2)
-            printvv(llm_solution)
+            printvv(source_code)
             print_horizontal_line(2)
             printvv("")
 
             # Pass to ESBMC, a workaround is used where the file is saved
             # to a temporary location since ESBMC needs it in file format.
             self.anim.start("Verifying with ESBMC... Please Wait")
             exit_code, esbmc_output = esbmc_load_source_code(
                 file_path=file_name,
-                source_code=llm_solution,
+                source_code=source_code,
                 esbmc_params=config.esbmc_params,
                 auto_clean=config.temp_auto_clean,
                 timeout=config.verifier_timeout,
             )
             self.anim.stop()
 
             # Print verbose lvl 2
             print_horizontal_line(2)
             printvv(esbmc_output)
             print_horizontal_line(2)
 
             # Solution found
             if exit_code == 0:
-                self.on_solution_signal.emit(llm_solution)
+                self.on_solution_signal.emit(source_code)
 
                 if config.raw_conversation:
                     print_raw_conversation()
 
                 printv("ESBMC-AI Notice: Successfully verified code")
 
-                return False, llm_solution
+                return False, source_code
 
             # TODO Move this process into Solution Generator since have (beginning) is done
             # inside, and the other half is done here.
             # Get formatted ESBMC output
             try:
                 esbmc_output = get_esbmc_output_formatted(
                     esbmc_output_type=config.esbmc_output_type,
@@ -147,34 +147,15 @@
                 pass
             except ESBMCTimedOutException:
                 print("error: ESBMC has timed out...")
                 sys.exit(1)
 
             # Failure case
             print(f"ESBMC-AI Notice: Failure {idx+1}/{max_retries}: Retrying...")
-            # If final iteration no need to sleep.
-            if idx < max_retries - 1:
 
-                # Inform solution generator chat about the ESBMC response.
-                # TODO Add option to customize in config.
-                if exit_code != 1:
-                    # The program did not compile.
-                    solution_generator.push_to_message_stack(
-                        message=HumanMessage(
-                            content=f"Here is the ESBMC output:\n\n```\n{esbmc_output}\n```"
-                        )
-                    )
-                else:
-                    solution_generator.push_to_message_stack(
-                        message=HumanMessage(
-                            content=f"Here is the ESBMC output:\n\n```\n{esbmc_output}\n```"
-                        )
-                    )
-
-                solution_generator.push_to_message_stack(
-                    AIMessage(content="Understood.")
-                )
+            # Update state
+            solution_generator.update_state(source_code, esbmc_output)
 
         if config.raw_conversation:
             print_raw_conversation()
 
         return True, "ESBMC-AI Notice: Failed all attempts..."
```

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0rc1/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/.gitignore` & `esbmc_ai-0.5.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/LICENSE` & `esbmc_ai-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/README.md` & `esbmc_ai-0.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/pyproject.toml` & `esbmc_ai-0.5.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc0/PKG-INFO` & `esbmc_ai-0.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0rc0
+Version: 0.5.0rc1
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

