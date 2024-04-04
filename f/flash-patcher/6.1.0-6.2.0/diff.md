# Comparing `tmp/flash_patcher-6.1.0.tar.gz` & `tmp/flash_patcher-6.2.0.tar.gz`

## Comparing `flash_patcher-6.1.0.tar` & `flash_patcher-6.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/antlr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/antlr-copy
--rwxr-xr-x   0        0        0     2226 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/__main__.py
--rwxr-xr-x   0        0        0     2642 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/patcher.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr/PatchfileLexer.g4
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr/PatchfileParser.g4
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/compile/compilation.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/compile/ffdec.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/compile/locate_decomp.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/exception/dependency.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/exception/error_manager.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/exception/error_suppression.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/exception/injection.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/inject/bulk_injection.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/inject/find_content.py
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/inject/single_injection.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/inject/location/constant_injection_location.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/inject/location/injection_location.py
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/inject/location/parser_injection_location.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/parse/common.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/parse/patch.py
--rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/parse/patch_visitor.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/parse/scope.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/util/external_cmd.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/util/file_copy.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/util/file_io.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/.gitkeep
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileLexer.g4
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileLexer.interp
--rw-r--r--   0        0        0    13501 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileLexer.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileLexer.tokens
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParser.g4
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParser.interp
--rw-r--r--   0        0        0    53033 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParser.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParser.tokens
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParserListener.py
--rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParserVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/flash_patcher/antlr_source/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/.gitignore
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/pyproject.toml
--rw-r--r--   0        0        0    11415 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/../README.md
--rw-r--r--   0        0        0    52460 2020-02-02 00:00:00.000000 flash_patcher-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/antlr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/antlr-copy
+-rwxr-xr-x   0        0        0     2226 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/__main__.py
+-rwxr-xr-x   0        0        0     2642 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/patcher.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr/PatchfileLexer.g4
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr/PatchfileParser.g4
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/compile/compilation.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/compile/ffdec.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/compile/locate_decomp.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/exception/dependency.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/exception/error_manager.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/exception/error_suppression.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/exception/injection.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/inject/bulk_injection.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/inject/find_content.py
+-rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/inject/single_injection.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/inject/location/constant_injection_location.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/inject/location/injection_location.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/inject/location/parser_injection_location.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/parse/common.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/parse/patch.py
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/parse/patch_visitor.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/parse/scope.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/util/external_cmd.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/util/file_copy.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/util/file_io.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/.gitkeep
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileLexer.g4
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileLexer.interp
+-rw-r--r--   0        0        0    13501 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileLexer.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileLexer.tokens
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParser.g4
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParser.interp
+-rw-r--r--   0        0        0    53033 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParser.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParser.tokens
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParserListener.py
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParserVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/flash_patcher/antlr_source/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/.gitignore
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11743 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/../README.md
+-rw-r--r--   0        0        0    52788 2020-02-02 00:00:00.000000 flash_patcher-6.2.0/PKG-INFO
```

### Comparing `flash_patcher-6.1.0/Makefile` & `flash_patcher-6.2.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,16 @@
 	@echo "Running pylint on tests..."
 	pylint $(shell git ls-files '../test/*.py') \
 	--disable=missing-module-docstring \
 	--disable=missing-function-docstring \
 	--disable=missing-class-docstring \
 	--disable=import-error \
 	--disable=wrong-import-position \
-	--disable=no-name-in-module
+	--disable=no-name-in-module \
+	--disable=too-many-public-methods
 
 # Run unit tests
 # The find rule creates an __init__.py in all subdirectories, including nested subdirectories
 test: antlr
 	find ../test -type d -exec touch {}/__init__.py \;
 
 	@echo "Running tests..."
```

### Comparing `flash_patcher-6.1.0/flash_patcher/__main__.py` & `flash_patcher-6.2.0/flash_patcher/__main__.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/patcher.py` & `flash_patcher-6.2.0/flash_patcher/patcher.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr/PatchfileLexer.g4` & `flash_patcher-6.2.0/flash_patcher/antlr/PatchfileLexer.g4`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr/PatchfileParser.g4` & `flash_patcher-6.2.0/flash_patcher/antlr/PatchfileParser.g4`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/compile/compilation.py` & `flash_patcher-6.2.0/flash_patcher/compile/compilation.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/compile/ffdec.py` & `flash_patcher-6.2.0/flash_patcher/compile/ffdec.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/exception/error_manager.py` & `flash_patcher-6.2.0/flash_patcher/exception/error_manager.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/exception/error_suppression.py` & `flash_patcher-6.2.0/flash_patcher/exception/error_suppression.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/inject/bulk_injection.py` & `flash_patcher-6.2.0/flash_patcher/inject/bulk_injection.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/inject/find_content.py` & `flash_patcher-6.2.0/flash_patcher/inject/find_content.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/inject/single_injection.py` & `flash_patcher-6.2.0/flash_patcher/inject/single_injection.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/inject/location/constant_injection_location.py` & `flash_patcher-6.2.0/flash_patcher/inject/location/constant_injection_location.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/inject/location/injection_location.py` & `flash_patcher-6.2.0/flash_patcher/inject/location/injection_location.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/inject/location/parser_injection_location.py` & `flash_patcher-6.2.0/flash_patcher/inject/location/parser_injection_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,29 +78,41 @@
     def resolve_function(
         self: ParserInjectionLocation,
         file_content: list[str],
         exception: ErrorManager,
     ) -> int | None:
         """Resolve the injection location if it's a function + offset."""
         line_no = None
+        curly_brace_line = None
+        found_fn = False
+
         for i, line in enumerate(file_content):
             # Do some replacement to ensure that function names are processed correctly
             line = line.replace("(", " ")
             line = line.replace(")", " ")
 
             if line.split()[:2] == ["function", self.context.TEXT_BLOCK().getText()] \
                 or line.split()[:3] == [self.context.TEXT_BLOCK().getText(), "=", "function"]:
                 # We need to add after the specified line
                 line_no = i + 1
+                found_fn = True
+
+            # If there's no function offset, we want to inject after the {,
+            # not the function name line
+            if found_fn and '{' in line:
+                curly_brace_line = i + 1
                 break
 
         if line_no is not None:
             if self.context.INTEGER():
                 line_no += int(self.context.INTEGER().getText())
 
+            else:
+                line_no = curly_brace_line
+
             self.verify_line_no(line_no, file_content, exception)
 
         return line_no
 
     def resolve_text(
         self: ParserInjectionLocation,
         file_content: list[str],
```

### Comparing `flash_patcher-6.1.0/flash_patcher/parse/common.py` & `flash_patcher-6.2.0/flash_patcher/parse/common.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/parse/patch.py` & `flash_patcher-6.2.0/flash_patcher/parse/patch.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/parse/patch_visitor.py` & `flash_patcher-6.2.0/flash_patcher/parse/patch_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,13 +259,14 @@
         error_manager = ErrorManager(self.patch_file_name, ctx.start.line)
         ctx_filename = self.scope.resolve_all(ctx.file_name().getText(), error_manager)
 
         script_path = (self.folder / ctx_filename).resolve()
         self.modified_scripts |= get_modified_scripts_of_command(
             ["python3", script_path],
             self.decomp_location,
+            self.scope,
         )
 
     def visitRoot(self: PatchfileProcessor, ctx: PatchfileParser.RootContext) -> set:
         """Root function. Call this when running the visitor."""
         super().visitRoot(ctx)
         return self.modified_scripts
```

### Comparing `flash_patcher-6.1.0/flash_patcher/parse/scope.py` & `flash_patcher-6.2.0/flash_patcher/parse/scope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import copy
 import re
 
 from flash_patcher.exception.error_manager import ErrorManager
 
 class Scope:
     """Maintain scope information to be used in the parser."""
 
@@ -57,7 +58,31 @@
             # If the variable is not found, raise an error
             if resolved_match is None:
                 error_manager.raise_(f"Undefined variable {matched}.", NameError)
 
             resolved_content = resolved_content.replace(matched, resolved_match)
 
         return resolved_content
+
+    def get_config_map(self: Scope) -> map[str, str]:
+        """Get the configuration as a map.
+        This function is primarily used for subscript input.
+        """
+        config = copy.deepcopy(Scope.global_scope)
+
+        for key, val in self.local_scope.items():
+            config[key] = val
+
+        return config
+
+    def get_config(self: Scope) -> str:
+        """Get the configuration in CFG format.
+        This function is primarily used for subscript input.
+        """
+        config_map = self.get_config_map()
+
+        config = ""
+
+        for key, val in config_map.items():
+            config += key + "=" + val + "\n"
+
+        return config
```

### Comparing `flash_patcher-6.1.0/flash_patcher/util/external_cmd.py` & `flash_patcher-6.2.0/flash_patcher/util/external_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Helper module for calling external commands."""
 from os import chdir
 from pathlib import Path
 from subprocess import PIPE, CompletedProcess, run
 import sys
 
+from flash_patcher.parse.scope import Scope
+
 def ask_confirmation() -> None:
     """Prompt the user for confirmation before calling subprocess.run."""
     # ANSI escape code for red color
     red_color_code = "\033[91m"
 
     # ANSI escape code to reset text color
     reset_color_code = "\033[0m"
@@ -23,40 +25,44 @@
 
     if confirmation.strip().lower() != "y":
         print(f"{red_color_code}Aborting.{reset_color_code}")
         sys.exit(1)
 
     # implicitly, else continue execution
 
-def run_with_confirmation_in_dir(args: list, directory: Path) -> CompletedProcess:
+def run_with_confirmation_in_dir(args: list, directory: Path, stdin: str = "") -> CompletedProcess:
     """Run a command in the given directory."""
     ask_confirmation()
 
     cwd = Path.cwd()
     chdir(directory)
-    output = run(args, check=True, stdout=PIPE)
+    output = run(args, check=True, input=stdin, text=True, stdout=PIPE)
     chdir(cwd)
 
     return output
 
 
-def check_output_in_dir(args: list, directory: Path) -> bytes:
+def check_output_in_dir(args: list, directory: Path, stdin: str = "") -> bytes:
     """Run a command in the given directory, and return its output.
     Prompt the user with a security warning first.
     """
 
-    return run_with_confirmation_in_dir(args, directory).stdout
+    return run_with_confirmation_in_dir(args, directory, stdin).stdout
 
-def get_modified_scripts_of_command(args: list, directory: Path) -> set[Path]:
+def get_modified_scripts_of_command(args: list, directory: Path, scope: Scope) -> set[Path]:
     """Run the specified command, and output a set of modified scripts."""
+    process_stdin = scope.get_config()
+
     process_output = check_output_in_dir(
         args,
         directory,
+        stdin=process_stdin,
     )
-    process_output = process_output.decode('utf-8').strip()
+
+    process_output = process_output.strip()
 
     if process_output == "":
         return set()
 
     process_output = process_output.split(",")
 
     modified_scripts = set()
```

### Comparing `flash_patcher-6.1.0/flash_patcher/util/file_copy.py` & `flash_patcher-6.2.0/flash_patcher/util/file_copy.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/util/file_io.py` & `flash_patcher-6.2.0/flash_patcher/util/file_io.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileLexer.g4` & `flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileLexer.g4`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileLexer.interp` & `flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileLexer.interp`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileLexer.py` & `flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileLexer.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParser.g4` & `flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParser.g4`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParser.interp` & `flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParser.interp`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParser.py` & `flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParser.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParserListener.py` & `flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParserListener.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/flash_patcher/antlr_source/PatchfileParserVisitor.py` & `flash_patcher-6.2.0/flash_patcher/antlr_source/PatchfileParserVisitor.py`

 * *Files identical despite different names*

### Comparing `flash_patcher-6.1.0/pyproject.toml` & `flash_patcher-6.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flash-patcher"
 description = "rayyaw's SWF patcher"
-version = "6.1.0"
+version = "6.2.0"
 readme = "../README.md"
 license = { file = "../LICENSE" }
 authors = [
     {name = "rayyaw", email = "rayyawspeedruns@gmail.com"},
     {name = "qtkito", email = "gtcreyon@gmail.com"},
     {name = "GTcreyon", email = "gtcreyon@gmail.com"},
 ]
```

### Comparing `flash_patcher-6.1.0/../README.md` & `flash_patcher-6.2.0/../README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 To apply a patch, run the `flash-patcher` command.
 
 The patcher will take the input SWF, apply the commands specified in the top-level patch file (which must be located in the patch folder), and create the output SWF.
 
 The recommended way to install Flash Patcher is through pip. You can do this with `pip install flash-patcher`.
 
-If you want to build the Flash Patcher .whl file locally, run `cd build && make`. The .whl will be generated in the dist/ folder. The `hatch` pip package is required to run the build. You can also run `make install` to install the package locally. **Note that this will run pip with `--break-system-packages` and `--force-reinstall` options, so use this at your own risk.**
+If you want to build the Flash Patcher .whl file locally, run `cd build && make`. The .whl will be generated in the `dist/` folder. The `hatch` pip package is required to run the build. You can also run `make install` to install the package locally. **Note that this will run pip with `--break-system-packages` and `--force-reinstall` options, so use this at your own risk.**
 
 The command line arguments are as follows:
 
 ### Required arguments
 - `--inputswf`: The input SWF to use. You should create a base hack to avoid issues with Flash deobfuscation.
 - `--folder`: The top-level folder where all your patch files are located.
 - `--stagefile`: The top level patch file's path within the top level folder.
@@ -215,15 +215,25 @@
 
 - Only Python 3 is supported.
 - The name of the Python file must not contain spaces.
 - You must print a list of files that are modified. This list must be comma-separated and formatted in UTF-8.
 
 An example of such a list: `DoAction1.as, DoAction2.as`. Trailing whitespace or newlines are fine, as those will be stripped off.
 
-**Note:** Python files don't support accessing or modifying scoped variables.
+The input to your Python program will be a list of variables in CFG format, passed through stdin. Here is an example of the stdin:
+
+```
+key1=val1
+key2=val2
+
+```
+
+Note that a trailing newline may be present. Also note that both variable names and values may contain any character other than `-` or `=`, and you must handle all appropriate cases.
+
+**Note:** Python files don't support modifying variables.
 
 ### Injection Order
 
 Within each patchfile, the patches will be processed one block at a time, with each command being processed from the top of the file to the bottom. Note that if you are injecting multiple times into the same file, this means that you should inject bottom to top to avoid the line numbers changing as the file is being patched.
 
 ## Licensing
```

### Comparing `flash_patcher-6.1.0/PKG-INFO` & `flash_patcher-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: flash-patcher
-Version: 6.1.0
+Version: 6.2.0
 Summary: rayyaw's SWF patcher
 Project-URL: Documentation, https://github.com/rayyaw/flash-patcher
 Project-URL: Source, https://github.com/rayyaw/flash-patcher
 Project-URL: History, https://github.com/rayyaw/flash-patcher
 Project-URL: Issues, https://github.com/rayyaw/flash-patcher/issues
 Author-email: rayyaw <rayyawspeedruns@gmail.com>, qtkito <gtcreyon@gmail.com>, GTcreyon <gtcreyon@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -719,15 +719,15 @@
 
 To apply a patch, run the `flash-patcher` command.
 
 The patcher will take the input SWF, apply the commands specified in the top-level patch file (which must be located in the patch folder), and create the output SWF.
 
 The recommended way to install Flash Patcher is through pip. You can do this with `pip install flash-patcher`.
 
-If you want to build the Flash Patcher .whl file locally, run `cd build && make`. The .whl will be generated in the dist/ folder. The `hatch` pip package is required to run the build. You can also run `make install` to install the package locally. **Note that this will run pip with `--break-system-packages` and `--force-reinstall` options, so use this at your own risk.**
+If you want to build the Flash Patcher .whl file locally, run `cd build && make`. The .whl will be generated in the `dist/` folder. The `hatch` pip package is required to run the build. You can also run `make install` to install the package locally. **Note that this will run pip with `--break-system-packages` and `--force-reinstall` options, so use this at your own risk.**
 
 The command line arguments are as follows:
 
 ### Required arguments
 - `--inputswf`: The input SWF to use. You should create a base hack to avoid issues with Flash deobfuscation.
 - `--folder`: The top-level folder where all your patch files are located.
 - `--stagefile`: The top level patch file's path within the top level folder.
@@ -903,15 +903,25 @@
 
 - Only Python 3 is supported.
 - The name of the Python file must not contain spaces.
 - You must print a list of files that are modified. This list must be comma-separated and formatted in UTF-8.
 
 An example of such a list: `DoAction1.as, DoAction2.as`. Trailing whitespace or newlines are fine, as those will be stripped off.
 
-**Note:** Python files don't support accessing or modifying scoped variables.
+The input to your Python program will be a list of variables in CFG format, passed through stdin. Here is an example of the stdin:
+
+```
+key1=val1
+key2=val2
+
+```
+
+Note that a trailing newline may be present. Also note that both variable names and values may contain any character other than `-` or `=`, and you must handle all appropriate cases.
+
+**Note:** Python files don't support modifying variables.
 
 ### Injection Order
 
 Within each patchfile, the patches will be processed one block at a time, with each command being processed from the top of the file to the bottom. Note that if you are injecting multiple times into the same file, this means that you should inject bottom to top to avoid the line numbers changing as the file is being patched.
 
 ## Licensing
```

