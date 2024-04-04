# Comparing `tmp/incremental_backup-1.0.1.tar.gz` & `tmp/incremental_backup-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incremental_backup-1.0.1.tar", last modified: Sun Feb 25 08:14:41 2024, max compression
+gzip compressed data, was "incremental_backup-1.1.0.tar", last modified: Thu Apr  4 09:57:56 2024, max compression
```

## Comparing `incremental_backup-1.0.1.tar` & `incremental_backup-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.231241 incremental_backup-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-02-25 08:14:41.231241 incremental_backup-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.227241 incremental_backup-1.0.1/incremental_backup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.227241 incremental_backup-1.0.1/incremental_backup/_utility/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/_utility/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/_utility/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.227241 incremental_backup-1.0.1/incremental_backup/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/backup/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/backup/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/backup/sum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.227241 incremental_backup-1.0.1/incremental_backup/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.231241 incremental_backup-1.0.1/incremental_backup/cli/command/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/cli/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/cli/command/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/cli/command/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/cli/command/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/cli/command/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/cli/command/restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.231241 incremental_backup-1.0.1/incremental_backup/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/meta/complete_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/meta/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/meta/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/meta/start_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/path_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/incremental_backup/restore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.231241 incremental_backup-1.0.1/incremental_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-02-25 08:14:41.000000 incremental_backup-1.0.1/incremental_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-25 08:14:41.000000 incremental_backup-1.0.1/incremental_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 08:14:41.000000 incremental_backup-1.0.1/incremental_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-25 08:14:41.000000 incremental_backup-1.0.1/incremental_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 08:14:41.231241 incremental_backup-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 08:14:41.231241 incremental_backup-1.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/test/test_path_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)    26292 2024-02-25 08:14:27.000000 incremental_backup-1.0.1/test/test_restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.527178 incremental_backup-1.1.0/incremental_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.527178 incremental_backup-1.1.0/incremental_backup/_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/_utility/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/_utility/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.527178 incremental_backup-1.1.0/incremental_backup/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/backup/sum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.527178 incremental_backup-1.1.0/incremental_backup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/incremental_backup/cli/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/command/restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/incremental_backup/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/complete_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/meta/start_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/path_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/incremental_backup/restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/incremental_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-04 09:57:56.000000 incremental_backup-1.1.0/incremental_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-04 09:57:56.000000 incremental_backup-1.1.0/incremental_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:57:56.000000 incremental_backup-1.1.0/incremental_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 09:57:56.000000 incremental_backup-1.1.0/incremental_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:57:56.531178 incremental_backup-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/test/test_path_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/test/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26292 2024-04-04 09:57:52.000000 incremental_backup-1.1.0/test/test_restore.py
```

### Comparing `incremental_backup-1.0.1/LICENCE.txt` & `incremental_backup-1.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/PKG-INFO` & `incremental_backup-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incremental_backup
-Version: 1.0.1
+Version: 1.1.0
 Summary: Incremental file backup tool
 Author-email: Reece Jones <reece.jones131@gmail.com>
 Project-URL: Homepage, https://github.com/MC-DeltaT/IncrementalBackup2
 Project-URL: Issues, https://github.com/MC-DeltaT/IncrementalBackup2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `incremental_backup-1.0.1/README.md` & `incremental_backup-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/backup/backup.py` & `incremental_backup-1.1.0/incremental_backup/backup/backup.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/backup/filesystem.py` & `incremental_backup-1.1.0/incremental_backup/backup/filesystem.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/backup/plan.py` & `incremental_backup-1.1.0/incremental_backup/backup/plan.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/backup/sum.py` & `incremental_backup-1.1.0/incremental_backup/backup/sum.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/cli/command/backup.py` & `incremental_backup-1.1.0/incremental_backup/cli/command/backup.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/cli/command/command.py` & `incremental_backup-1.1.0/incremental_backup/cli/command/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     @staticmethod
     def add_arg_subparser(subparser, /) -> None:
         """Adds the argparse subparser for the command."""
 
         raise NotImplementedError()
 
+    # TODO: pass args as a struct for backwards compatibility
     def __init__(self, arguments: argparse.Namespace, /) -> None:
         """
             :param arguments: The parsed command line arguments object acquired from argparse.
         """
 
     def run(self) -> None:
         """Executes the command."""
```

### Comparing `incremental_backup-1.0.1/incremental_backup/cli/command/exception.py` & `incremental_backup-1.1.0/incremental_backup/cli/command/exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Optional
+
+
 __all__ = [
     'CommandArgumentError',
     'CommandError',
     'CommandRuntimeError'
 ]
 
 
@@ -18,18 +21,19 @@
         super().__init__(message)
         self.message = message
 
 
 class CommandArgumentError(CommandError):
     """Indicates that command line arguments are invalid."""
 
-    def __init__(self, message: str, usage: str) -> None:
+    # TODO: remove usage
+    def __init__(self, message: str, usage: Optional[str] = None) -> None:
         """
             :param message: Specific description of the error.
-            :param usage: Program usage information string to display to the user.
+            :param usage: (DEPRECATED) Program usage information string to display to the user.
         """
 
         super().__init__(message)
         self.usage = usage
 
 
 class CommandRuntimeError(CommandError):
```

### Comparing `incremental_backup-1.0.1/incremental_backup/cli/command/registry.py` & `incremental_backup-1.1.0/incremental_backup/cli/command/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from collections.abc import Sequence
 
 from incremental_backup.cli.command.command import Command
 from incremental_backup.cli.command.backup import BackupCommand
 from incremental_backup.cli.command.restore import RestoreCommand
+from incremental_backup.cli.command.prune import PruneCommand
 
 
 __all__ = [
     'COMMAND_CLASSES',
     'get_command_class'
 ]
 
 
 COMMAND_CLASSES: Sequence[type[Command]] = (
     BackupCommand,
-    RestoreCommand
+    RestoreCommand,
+    PruneCommand
 )
 """List of all commands recognised by the program.
     Add or remove commands here.
 """
 
 
 def get_command_class(command_string: str, /) -> type[Command]:
```

### Comparing `incremental_backup-1.0.1/incremental_backup/cli/command/restore.py` & `incremental_backup-1.1.0/incremental_backup/cli/command/restore.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/cli/main.py` & `incremental_backup-1.1.0/incremental_backup/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,45 +27,36 @@
         :return: Process exit code.
     """
 
     # Strip off the "program name" argument.
     arguments = arguments[1:]
 
     try:
-        _api_main(arguments)
+        arg_parser = _get_argument_parser()
+        parsed_arguments = arg_parser.parse_args(arguments)
+        command_class = get_command_class(parsed_arguments.command)
+        command_instance = command_class(parsed_arguments)
+        command_instance.run()
         return EXIT_CODE_SUCCESS
     except CommandArgumentError as e:
-        print(e.usage, file=sys.stderr)
-        print(e.message, file=sys.stderr)
+        if e.usage is None: # TODO: remove when usage is removed
+            arg_parser.print_usage(sys.stderr)
+        else:
+            print(e.usage, file=sys.stderr)
+        print()
+        print(f'{arg_parser.prog}: error: {e.message}', file=sys.stderr)
         return EXIT_CODE_INVALID_ARGUMENTS
     except CommandError as e:
         print_error(str(e))
         return EXIT_CODE_GENERAL_ERROR
     except Exception as e:
         print_error(f'Unhandled exception: {repr(e)}')
         return EXIT_CODE_LOGIC_ERROR
 
 
-def _api_main(arguments: Sequence[str], /) -> None:
-    """API-level entrypoint of the incremental backup program.
-
-        :param arguments: The program command line arguments. Should not include the "program name" zeroth argument.
-        :except CommandArgumentError: If the command line arguments are invalid.
-        :except CommandError: If some other fatal error occurs.
-    """
-
-    arg_parser = _get_argument_parser()
-
-    parsed_arguments = arg_parser.parse_args(arguments)
-
-    command_class = get_command_class(parsed_arguments.command)
-    command_instance = command_class(parsed_arguments)
-    command_instance.run()
-
-
 def _get_argument_parser() -> argparse.ArgumentParser:
     """Creates the command line argument parser. Adds subparsers for each command."""
 
     arg_parser = _ArgumentParser('incremental_backup', description='Incremental backup tool.')
     arg_subparser = arg_parser.add_subparsers(title='commands', required=True, dest='command')
 
     for cls in COMMAND_CLASSES:
@@ -75,16 +66,15 @@
 
 
 class _ArgumentParser(argparse.ArgumentParser):
     """Custom `argparse.ArgumentParser` implementation so we can throw exceptions for invalid arguments instead of
         exiting the process."""
 
     def error(self, message: str) -> NoReturn:
-        full_message = f'{self.prog}: error: {message}'     # Same as base ArgumentParser
-        raise CommandArgumentError(full_message, self.format_usage())
+        raise CommandArgumentError(message)
 
 
 # Process exit codes.
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_INVALID_ARGUMENTS = 1
 EXIT_CODE_GENERAL_ERROR = 2
 EXIT_CODE_LOGIC_ERROR = -1
```

### Comparing `incremental_backup-1.0.1/incremental_backup/meta/complete_info.py` & `incremental_backup-1.1.0/incremental_backup/meta/complete_info.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/meta/manifest.py` & `incremental_backup-1.1.0/incremental_backup/meta/manifest.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/meta/meta.py` & `incremental_backup-1.1.0/incremental_backup/meta/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     name: str
     start_info: BackupStartInfo
     manifest: BackupManifest
 
     # Backup completion information is not here because it is currently not read by the application.
 
 
+# TODO: should refactor and simplify exceptions. Don't need so fine grained.
+
 def read_backup_metadata(backup_directory: StrPath, /) -> BackupMetadata:
     """Reads the metadata of a backup, i.e. the name, start information, and manifest.
 
         :except OSError: If a metadata file could not be read.
         :except BackupStartInfoParseError: If the backup start information file could not be parsed.
         :except BackupManifestParseError: If the backup manifest file could not be parsed.
     """
```

### Comparing `incremental_backup-1.0.1/incremental_backup/meta/start_info.py` & `incremental_backup-1.1.0/incremental_backup/meta/start_info.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/path_exclude.py` & `incremental_backup-1.1.0/incremental_backup/path_exclude.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup/restore.py` & `incremental_backup-1.1.0/incremental_backup/restore.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/incremental_backup.egg-info/PKG-INFO` & `incremental_backup-1.1.0/incremental_backup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incremental_backup
-Version: 1.0.1
+Version: 1.1.0
 Summary: Incremental file backup tool
 Author-email: Reece Jones <reece.jones131@gmail.com>
 Project-URL: Homepage, https://github.com/MC-DeltaT/IncrementalBackup2
 Project-URL: Issues, https://github.com/MC-DeltaT/IncrementalBackup2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `incremental_backup-1.0.1/incremental_backup.egg-info/SOURCES.txt` & `incremental_backup-1.1.0/incremental_backup.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENCE.txt
 README.md
 pyproject.toml
 incremental_backup/__init__.py
 incremental_backup/__main__.py
 incremental_backup/path_exclude.py
+incremental_backup/prune.py
 incremental_backup/restore.py
 incremental_backup.egg-info/PKG-INFO
 incremental_backup.egg-info/SOURCES.txt
 incremental_backup.egg-info/dependency_links.txt
 incremental_backup.egg-info/top_level.txt
 incremental_backup/_utility/__init__.py
 incremental_backup/_utility/console.py
@@ -19,16 +20,18 @@
 incremental_backup/backup/sum.py
 incremental_backup/cli/__init__.py
 incremental_backup/cli/main.py
 incremental_backup/cli/command/__init__.py
 incremental_backup/cli/command/backup.py
 incremental_backup/cli/command/command.py
 incremental_backup/cli/command/exception.py
+incremental_backup/cli/command/prune.py
 incremental_backup/cli/command/registry.py
 incremental_backup/cli/command/restore.py
 incremental_backup/meta/__init__.py
 incremental_backup/meta/complete_info.py
 incremental_backup/meta/manifest.py
 incremental_backup/meta/meta.py
 incremental_backup/meta/start_info.py
 test/test_path_exclude.py
+test/test_prune.py
 test/test_restore.py
```

### Comparing `incremental_backup-1.0.1/pyproject.toml` & `incremental_backup-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "incremental_backup"
 # TODO: update when making changes.
-version = "1.0.1"
+version = "1.1.0"
 authors = [
     { name="Reece Jones", email="reece.jones131@gmail.com" }
 ]
 description = "Incremental file backup tool"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `incremental_backup-1.0.1/test/test_path_exclude.py` & `incremental_backup-1.1.0/test/test_path_exclude.py`

 * *Files identical despite different names*

### Comparing `incremental_backup-1.0.1/test/test_restore.py` & `incremental_backup-1.1.0/test/test_restore.py`

 * *Files identical despite different names*

