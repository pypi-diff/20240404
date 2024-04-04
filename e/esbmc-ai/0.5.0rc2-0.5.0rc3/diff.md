# Comparing `tmp/esbmc_ai-0.5.0rc2.tar.gz` & `tmp/esbmc_ai-0.5.0rc3.tar.gz`

## Comparing `esbmc_ai-0.5.0rc2.tar` & `esbmc_ai-0.5.0rc3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/config.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/README.md
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/config.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/README.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/config.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/logging.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/logging.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/commands/fix_code_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
                     requests_timeout=config.requests_timeout,
                 ),
                 scenario=scenario,
                 source_code_format=config.source_code_format,
                 esbmc_output_type=config.esbmc_output_type,
             )
         except ESBMCTimedOutException:
+            if config.raw_conversation:
+                print_raw_conversation()
             print("error: ESBMC has timed out...")
             sys.exit(1)
 
         print()
 
         max_retries: int = config.fix_code_max_attempts
         for idx in range(max_retries):
@@ -142,14 +144,16 @@
                 esbmc_output = get_esbmc_output_formatted(
                     esbmc_output_type=config.esbmc_output_type,
                     esbmc_output=esbmc_output,
                 )
             except SourceCodeParseError:
                 pass
             except ESBMCTimedOutException:
+                if config.raw_conversation:
+                    print_raw_conversation()
                 print("error: ESBMC has timed out...")
                 sys.exit(1)
 
             # Failure case
             print(f"ESBMC-AI Notice: Failure {idx+1}/{max_retries}: Retrying...")
 
             # Update state
```

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0rc3/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/.gitignore` & `esbmc_ai-0.5.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/LICENSE` & `esbmc_ai-0.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/README.md` & `esbmc_ai-0.5.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/pyproject.toml` & `esbmc_ai-0.5.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc2/PKG-INFO` & `esbmc_ai-0.5.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0rc2
+Version: 0.5.0rc3
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

