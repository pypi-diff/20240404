# Comparing `tmp/axem_dem-0.3.1.tar.gz` & `tmp/axem_dem-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axem_dem-0.3.1.tar", max compression
+gzip compressed data, was "axem_dem-0.4.0.tar", max compression
```

## Comparing `axem_dem-0.3.1.tar` & `axem_dem-0.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    13291 2024-02-23 13:48:13.916078 axem_dem-0.3.1/LICENSE
--rw-r--r--   0        0        0     6008 2024-03-12 14:32:11.417948 axem_dem-0.3.1/README.md
--rw-r--r--   0        0        0       97 2024-02-23 13:48:13.916078 axem_dem-0.3.1/dem/__init__.py
--rw-r--r--   0        0        0     2230 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/__main__.py
--rw-r--r--   0        0        0      745 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/add_cat_cmd.py
--rw-r--r--   0        0        0      826 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/add_host_cmd.py
--rw-r--r--   0        0        0      649 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/add_reg_cmd.py
--rw-r--r--   0        0        0     1131 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/assign_cmd.py
--rw-r--r--   0        0        0     1960 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/clone_cmd.py
--rw-r--r--   0        0        0     1506 2024-03-07 17:34:45.936022 axem_dem-0.3.1/dem/cli/command/cp_cmd.py
--rw-r--r--   0        0        0     8085 2024-03-20 12:54:49.780864 axem_dem-0.3.1/dem/cli/command/create_cmd.py
--rw-r--r--   0        0        0      755 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/del_cat_cmd.py
--rw-r--r--   0        0        0      647 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/del_host_cmd.py
--rw-r--r--   0        0        0      706 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/del_reg_cmd.py
--rw-r--r--   0        0        0     1156 2024-03-20 12:54:49.780864 axem_dem-0.3.1/dem/cli/command/delete_cmd.py
--rw-r--r--   0        0        0      907 2024-03-07 17:34:45.940022 axem_dem-0.3.1/dem/cli/command/export_cmd.py
--rw-r--r--   0        0        0     1716 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/info_cmd.py
--rw-r--r--   0        0        0     2046 2024-03-20 12:54:49.780864 axem_dem-0.3.1/dem/cli/command/init_cmd.py
--rw-r--r--   0        0        0     1112 2024-03-07 17:34:45.940022 axem_dem-0.3.1/dem/cli/command/install_cmd.py
--rw-r--r--   0        0        0      935 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/list_cat_cmd.py
--rw-r--r--   0        0        0     5329 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/list_cmd.py
--rw-r--r--   0        0        0      972 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/list_host_cmd.py
--rw-r--r--   0        0        0      636 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/list_reg_cmd.py
--rw-r--r--   0        0        0     1454 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/load_cmd.py
--rw-r--r--   0        0        0     9025 2024-03-20 12:54:49.780864 axem_dem-0.3.1/dem/cli/command/modify_cmd.py
--rw-r--r--   0        0        0      543 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/rename_cmd.py
--rw-r--r--   0        0        0     2461 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/command/run_cmd.py
--rw-r--r--   0        0        0     1117 2024-03-20 12:54:49.780864 axem_dem-0.3.1/dem/cli/command/uninstall_cmd.py
--rw-r--r--   0        0        0      167 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/console.py
--rw-r--r--   0        0        0    16621 2024-03-07 17:34:45.940022 axem_dem-0.3.1/dem/cli/main.py
--rw-r--r--   0        0        0     2481 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/tui/panel/tool_image_selector.py
--rw-r--r--   0        0        0     3226 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/tui/panel/tool_type_selector.py
--rw-r--r--   0        0        0    12680 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/tui/renderable/menu.py
--rw-r--r--   0        0        0     4411 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/cli/tui/tui_user_output.py
--rw-r--r--   0        0        0     5263 2024-03-20 12:54:49.780864 axem_dem-0.3.1/dem/core/container_engine.py
--rw-r--r--   0        0        0      770 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/core.py
--rw-r--r--   0        0        0     4232 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/data_management.py
--rwxr-xr-x   0        0        0     4562 2024-03-07 17:34:45.940022 axem_dem-0.3.1/dem/core/dev_env.py
--rw-r--r--   0        0        0     4443 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/dev_env_catalog.py
--rw-r--r--   0        0        0     1225 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/exceptions.py
--rw-r--r--   0        0        0     2122 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/hosts.py
--rw-r--r--   0        0        0     9735 2024-03-20 12:54:49.780864 axem_dem-0.3.1/dem/core/platform.py
--rw-r--r--   0        0        0      129 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/properties.py
--rw-r--r--   0        0        0     9340 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/registry.py
--rw-r--r--   0        0        0     2292 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/tool_images.py
--rw-r--r--   0        0        0     2235 2024-02-23 13:48:13.920078 axem_dem-0.3.1/dem/core/user_output.py
--rw-r--r--   0        0        0     1812 2024-03-20 12:57:02.033904 axem_dem-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7373 1970-01-01 00:00:00.000000 axem_dem-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    13291 2024-02-23 13:48:13.916078 axem_dem-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6008 2024-03-12 14:32:11.417948 axem_dem-0.4.0/README.md
+-rw-r--r--   0        0        0       97 2024-02-23 13:48:13.916078 axem_dem-0.4.0/dem/__init__.py
+-rw-r--r--   0        0        0     2330 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/__main__.py
+-rw-r--r--   0        0        0      745 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/add_cat_cmd.py
+-rw-r--r--   0        0        0      826 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/add_host_cmd.py
+-rw-r--r--   0        0        0      649 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/add_reg_cmd.py
+-rw-r--r--   0        0        0     1134 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/assign_cmd.py
+-rw-r--r--   0        0        0     2219 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/clone_cmd.py
+-rw-r--r--   0        0        0     1508 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/cp_cmd.py
+-rw-r--r--   0        0        0     4709 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/command/create_cmd.py
+-rw-r--r--   0        0        0      755 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/del_cat_cmd.py
+-rw-r--r--   0        0        0      647 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/del_host_cmd.py
+-rw-r--r--   0        0        0      706 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/del_reg_cmd.py
+-rw-r--r--   0        0        0     1158 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/delete_cmd.py
+-rw-r--r--   0        0        0      909 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/export_cmd.py
+-rw-r--r--   0        0        0     2002 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/command/info_cmd.py
+-rw-r--r--   0        0        0     2048 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/init_cmd.py
+-rw-r--r--   0        0        0     1173 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/install_cmd.py
+-rw-r--r--   0        0        0      935 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/list_cat_cmd.py
+-rw-r--r--   0        0        0     5427 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/list_cmd.py
+-rw-r--r--   0        0        0      972 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/list_host_cmd.py
+-rw-r--r--   0        0        0      636 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/list_reg_cmd.py
+-rw-r--r--   0        0        0     1431 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/load_cmd.py
+-rw-r--r--   0        0        0     7181 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/command/modify_cmd.py
+-rw-r--r--   0        0        0      545 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/rename_cmd.py
+-rw-r--r--   0        0        0     2372 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/run_cmd.py
+-rw-r--r--   0        0        0     1119 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/uninstall_cmd.py
+-rw-r--r--   0        0        0      167 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/console.py
+-rw-r--r--   0        0        0    16397 2024-03-28 11:53:58.448947 axem_dem-0.4.0/dem/cli/main.py
+-rw-r--r--   0        0        0      790 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/tui/printable_tool_image.py
+-rw-r--r--   0        0        0    10200 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/tui/renderable/menu.py
+-rw-r--r--   0        0        0     4411 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/tui/tui_user_output.py
+-rw-r--r--   0        0        0     5453 2024-04-03 17:47:34.676890 axem_dem-0.4.0/dem/cli/tui/window/dev_env_settings_window.py
+-rw-r--r--   0        0        0     5263 2024-03-28 14:49:12.318896 axem_dem-0.4.0/dem/core/container_engine.py
+-rw-r--r--   0        0        0      770 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/core.py
+-rw-r--r--   0        0        0     4232 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/data_management.py
+-rwxr-xr-x   0        0        0     3020 2024-03-28 11:53:58.448947 axem_dem-0.4.0/dem/core/dev_env.py
+-rw-r--r--   0        0        0     4443 2024-03-25 12:12:59.178746 axem_dem-0.4.0/dem/core/dev_env_catalog.py
+-rw-r--r--   0        0        0     1330 2024-03-28 11:53:58.448947 axem_dem-0.4.0/dem/core/exceptions.py
+-rw-r--r--   0        0        0     2122 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/hosts.py
+-rw-r--r--   0        0        0     9982 2024-03-28 11:53:58.452947 axem_dem-0.4.0/dem/core/platform.py
+-rw-r--r--   0        0        0      129 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/properties.py
+-rw-r--r--   0        0        0     9292 2024-03-29 10:43:36.316870 axem_dem-0.4.0/dem/core/registry.py
+-rw-r--r--   0        0        0     3507 2024-03-28 11:53:58.452947 axem_dem-0.4.0/dem/core/tool_images.py
+-rw-r--r--   0        0        0     2235 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/user_output.py
+-rw-r--r--   0        0        0     1812 2024-04-03 17:54:18.051991 axem_dem-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7373 1970-01-01 00:00:00.000000 axem_dem-0.4.0/PKG-INFO
```

### Comparing `axem_dem-0.3.1/LICENSE` & `axem_dem-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/README.md` & `axem_dem-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/__main__.py` & `axem_dem-0.4.0/dem/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Entry point for dem."""
 # dem/__main__.py
 
 from dem import __command__
 from dem.cli.console import stderr, stdout
-from dem.core.exceptions import RegistryError, ContainerEngineError, InternalError, DataStorageError
+from dem.core.exceptions import RegistryError, ContainerEngineError, InternalError, DataStorageError, \
+                                CatalogError, ToolImageError
 import dem.cli.main
 from dem.core.core import Core
 from dem.core.platform import Platform
 from dem.cli.tui.tui_user_output import TUIUserOutput
 import docker.errors
 import typer
 
@@ -20,15 +21,15 @@
     # Connect the UI to the user output interface
     Core.set_user_output(TUIUserOutput())
 
     try:
         # Load the configuration file
         dem.cli.main.platform.config_file.update()
 
-        # Load the Dev Envs
+        # Load the Dev Env descriptors
         dem.cli.main.platform.load_dev_envs()
 
         # Run the CLI application
         dem.cli.main.typer_cli(prog_name=__command__)
     except LookupError as e:
         stderr.print("[red]" + str(e) + "[/]")
     except RegistryError as e:
@@ -38,16 +39,16 @@
 
         if "Permission denied" in str(e):
             stdout.print("\nHint: Is your user part of the docker group?")
         elif "invalid reference format" in str(e):
             stdout.print("\nHint: The input repository might not exist in the registry.")
         elif "400" in str(e):
             stdout.print("\nHint: The input parameters might not be valid.")
-    except (ContainerEngineError, InternalError) as e:
-        stderr.print("[red]" + str(e) + "[/]")
+    except (ContainerEngineError, InternalError, ToolImageError, CatalogError) as e:
+        stderr.print(f"[red]{str(e)}[/]")
     except DataStorageError as e:
         stderr.print("[red]" + str(e) + "[/]")
         if typer.confirm("Do you want to reset the file?"):
             if "config.json" in str(e):
                 stdout.print("Restoring the original configuration file...")
                 dem.cli.main.platform.config_file.restore()
             elif "dev_env.json" in str(e):
```

### Comparing `axem_dem-0.3.1/dem/cli/command/add_cat_cmd.py` & `axem_dem-0.4.0/dem/cli/command/add_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/add_host_cmd.py` & `axem_dem-0.4.0/dem/cli/command/add_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/add_reg_cmd.py` & `axem_dem-0.4.0/dem/cli/command/add_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/assign_cmd.py` & `axem_dem-0.4.0/dem/cli/command/assign_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,20 @@
     """Assign the given Development Environment to the given project.
 
         Args:
             platform -- the platform
             dev_env_name -- the name of the Development Environment to assign
             project_path -- the path to the project to assign the Development Environment to
     """
+
+
     if not os.path.isdir(project_path):
         stderr.print(f"[red]Error: The {project_path} path does not exist.[/]")
         return
 
     dev_env_to_assign: DevEnv | None = platform.get_dev_env_by_name(dev_env_name)
 
     if dev_env_to_assign is None:
         stderr.print(f"[red]Error: The {dev_env_name} Development Environment does not exist.[/]")
     else:
         platform.assign_dev_env(dev_env_to_assign, project_path)
-        stdout.print(f"\n[green]Successfully assigned the {dev_env_name} Dev Env to the project at{project_path}![/]")
+        stdout.print(f"\n[green]Successfully assigned the {dev_env_name} Dev Env to the project at {project_path}![/]")
```

### Comparing `axem_dem-0.3.1/dem/cli/command/clone_cmd.py` & `axem_dem-0.4.0/dem/cli/command/clone_cmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 """The clone command"""
 # dem/cli/command/clone_cmd.py
 
 import typer
 from dem.core.platform import Platform
 from dem.core.dev_env import DevEnv
+from dem.core.exceptions import PlatformError
 from dem.cli.console import stdout, stderr
 
 def handle_existing_local_dev_env(platform: Platform, local_dev_env: DevEnv) -> None:
     """ Handle the case when the Dev Env already exists locally.
 
         Args:
             platform -- the platform
             local_dev_env -- the existing Dev Env
     """
-    stdout.print("[yellow]The Dev Env already exists. By continuing the local Dev Env will be uninstalled.[/]")
+    stdout.print("[yellow]The Dev Env already exists.[/]")
     typer.confirm("Continue with overwrite?", abort=True)
     
-    # TODO: The Dev Env must be uninstalled before the descriptor gets removed.
+    if local_dev_env.is_installed:
+        typer.confirm("The Dev Env to overwrite is installed. Do you want to uninstall it?", 
+                      abort=True)
+        try:
+            platform.uninstall_dev_env(local_dev_env)
+        except PlatformError as e:
+            stderr.print(f"[red]{str(e)}[/]")
+            raise typer.Abort()
+
     platform.local_dev_envs.remove(local_dev_env)
 
 def execute(platform: Platform, dev_env_name: str) -> None:
     """ Copy the Dev Env's descriptor from the catalog to the local descriptor storage.
 
         If the Dev Env already exists locally, the user will be asked to confirm the overwrite.
 
         Args:
             platform -- the platform
             dev_env_name -- name of the Dev Env to clone
     """
+
+
     catalog_dev_env: DevEnv | None = None
 
     if not platform.dev_env_catalogs.catalogs:
         stderr.print("[red]Error: No Development Environment Catalogs are available to clone from![/]")
         return
 
     for catalog in platform.dev_env_catalogs.catalogs:
```

### Comparing `axem_dem-0.3.1/dem/cli/command/cp_cmd.py` & `axem_dem-0.4.0/dem/cli/command/cp_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,12 +27,14 @@
     new_dev_env = copy.deepcopy(dev_env_to_cp)
     new_dev_env.name = new_dev_env_name
     new_dev_env.is_installed = False
     platform.local_dev_envs.append(new_dev_env)
     platform.flush_descriptors()
 
 def execute(platform: Platform, dev_env_to_cp_name: str, new_dev_env_name: str) -> None:
+
+
     dev_env_to_cp = get_dev_env_to_cp(platform, dev_env_to_cp_name)
 
     if (dev_env_to_cp is not None and
         check_new_dev_env_name_taken(platform,new_dev_env_name) is False):
         cp_given_dev_env(platform, dev_env_to_cp, new_dev_env_name)
```

### Comparing `axem_dem-0.3.1/dem/cli/command/create_cmd.py` & `axem_dem-0.4.0/dem/cli/command/modify_cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,202 +1,186 @@
-"""create CLI command implementation."""
-# dem/cli/command/create_cmd.py
+"""modify CLI command implementation."""
+# dem/cli/command/modify_cmd
 
-import typer
+import copy, typer
 from dem.core.dev_env import DevEnv, DevEnv
-from dem.core.tool_images import ToolImages
+from dem.core.tool_images import ToolImage
 from dem.core.platform import Platform
 from dem.core.exceptions import PlatformError
-from dem.cli.console import stdout, stderr
-from dem.cli.tui.panel.tool_type_selector import ToolTypeSelectorPanel
-from dem.cli.tui.panel.tool_image_selector import ToolImageSelectorPanel
+from dem.cli.console import stderr, stdout
+from dem.cli.tui.renderable.menu import SelectMenu
+from dem.cli.tui.window.dev_env_settings_window import DevEnvSettingsWindow
+from dem.cli.tui.printable_tool_image import PrintableToolImage, convert_to_printable_tool_images
 
-tool_image_statuses = {
-    ToolImages.LOCAL_ONLY: "local",
-    ToolImages.REGISTRY_ONLY: "registry",
-    ToolImages.LOCAL_AND_REGISTRY: "local and registry"
-}
-
-def get_tool_image_list(tool_images: ToolImages) -> list[list[str]]:
+def get_confirm_from_user() -> str:
+    """ Get the confirmation from the user.
+        
+        Returns:
+            the confirmation option
     """
-    Combine the registry and local tool images, and assign the availabilities. 
+    confirm_menu_items = ["confirm", "save as", "cancel"]
+    select_menu = SelectMenu(confirm_menu_items)
+    select_menu.set_title("Are you sure to overwrite the Development Environment?")
+    select_menu.wait_for_user()
+    return select_menu.get_selected()
+
+def handle_user_confirm(confirmation: str, dev_env_local: DevEnv, platform: Platform) -> None:
+    """ Handle the user confirmation.
     
-    Args:
-        tool_images -- all the tool images
+        Args:
+            confirmation -- the confirmation option
+            dev_env_local -- the local Development Environment
+            platform -- the platform
+
+        Exceptions:
+            typer.Abort -- when the user tries to save as the Dev Env with a taken name or cancels 
+                           the operation
     """
-    tool_image_list = []
+    if confirmation == "cancel":
+        raise typer.Abort()
+
+    if confirmation == "save as":
+        new_dev_env = copy.deepcopy(dev_env_local)
+        new_dev_env.name = typer.prompt("Name of the new Development Environment")
+        
+        check_for_new_dev_env = platform.get_dev_env_by_name(new_dev_env.name)
 
-    for tool_image in tool_images.registry.elements:
-        if tool_image in tool_images.local.elements:
-            tool_image_list.append([tool_image, tool_image_statuses[ToolImages.LOCAL_AND_REGISTRY]])
+        if check_for_new_dev_env is None:
+            platform.local_dev_envs.append(new_dev_env)
         else:
-            tool_image_list.append([tool_image, tool_image_statuses[ToolImages.REGISTRY_ONLY]])
+            stderr.print("[red]The Development Environment already exist.")
+            raise typer.Abort()
 
-    for tool_image in tool_images.local.elements:
-        if tool_image not in tool_images.registry.elements:
-            tool_image_list.append([tool_image, tool_image_statuses[ToolImages.LOCAL_ONLY]])
-
-    return tool_image_list
-
-def handle_tool_type_selector_panel(tool_type_selector_panel: ToolTypeSelectorPanel, 
-                                    dev_env_name: str) -> list[str]:
-    tool_type_selector_panel.tool_type_menu.set_title("What kind of tools would you like to include in [cyan]" + dev_env_name + "[/]?")
-
-    tool_type_selector_panel.wait_for_user()
-
-    if "cancel" in tool_type_selector_panel.cancel_next_menu.get_selection():
-        raise(typer.Abort())
-
-    tool_type_selector_panel.cancel_next_menu.is_selected = False
-
-    return tool_type_selector_panel.tool_type_menu.get_selected_tool_types()
-
-def handle_tool_image_selector_panel(tool_image_selector_panel: ToolImageSelectorPanel, 
-                                     tool_type:str) -> str | None:
-    tool_image_selector_panel.tool_image_menu.set_title("Select tool image for: [yellow]" + tool_type + "[/]")
-    tool_image_selector_panel.wait_for_user()
-
-    if tool_image_selector_panel.back_menu.is_selected is True:
-        # Reset the back menu selection
-        tool_image_selector_panel.back_menu.is_selected = False
-        return None
-    else:
-        tool_image_selector_panel.tool_image_menu.is_selected = False
-        return tool_image_selector_panel.tool_image_menu.get_selected_tool_image()
-
-def get_dev_env_descriptor_from_user(dev_env_name: str, tool_image_list: list[list[str]]) -> dict:
-    current_panel = ToolTypeSelectorPanel(list(DevEnv.supported_tool_types))
-    panel_list = [current_panel]
-
-    tool_index = 0
-    panel_index = 0
-    tool_selection = {}
-    while current_panel is not None:
-        if isinstance(current_panel, ToolTypeSelectorPanel):
-            selected_tool_types = handle_tool_type_selector_panel(current_panel, dev_env_name)
-
-            # Remove the not selected tool type from the tool_selection.
-            for tool_type in list(tool_selection.keys()):
-                if tool_type not in selected_tool_types:
-                    del tool_selection[tool_type]
-
-            if len(panel_list) > 1:
-                current_panel = panel_list[1]
-                current_panel.dev_env_status.reset_table(selected_tool_types)
-            else:
-                current_panel = ToolImageSelectorPanel(tool_image_list, selected_tool_types)
-                panel_list.append(current_panel)
+    platform.flush_descriptors()
 
-            tool_index = 0
-            panel_index = 1
-        else:
-            selected_tool_image = handle_tool_image_selector_panel(current_panel, selected_tool_types[tool_index])
+def get_already_selected_tool_images(dev_env: DevEnv) -> set[str]:
+    """ Get the already selected Tool Images.
+    
+        Args:
+            dev_env -- the Development Environment
+            
+        Returns:
+            the already selected Tool Images
+    """
+    already_selected_tool_images = []
+    for tool in dev_env.tool_image_descriptors:
+        already_selected_tool_images.append(tool["image_name"] + ":" + tool["image_version"])
+
+    return already_selected_tool_images
+
+def remove_missing_tool_images(all_tool_images: dict[str, ToolImage], 
+                               already_selected_tool_images: list[str]) -> None:
+    """ Remove the missing Tool Images from the Development Environment.
+        
+            Args:
+                all_tool_images -- all available Tool Images
+                already_selected_tool_images -- the already selected Tool Images
+            
+            Exceptions:
+                typer.Abort -- if the user doesn't want the removal of the missing Tool Images
+    """
+    tool_images_are_missing = False
+
+    for already_selected_tool_image in already_selected_tool_images:
+        try:
+            all_tool_images[already_selected_tool_image]
+        except KeyError:
+            stderr.print(f"[red]The {already_selected_tool_image} is not available anymore.[/]")
+            already_selected_tool_images.remove(already_selected_tool_image)
+            tool_images_are_missing = True
+    
+    if tool_images_are_missing:
+        typer.confirm("By continuing, the missing tool images will be removed from the Development Environment.", 
+                    abort=True)
+
+def open_dev_env_settings_panel(already_selected_tool_images: list[str], 
+                                printable_tool_images: list[PrintableToolImage]) -> list[str]:
+    """ Open the Development Environment settings panel.
+    
+        Args:
+            already_selected_tool_images -- the already selected Tool Images
+            printable_tool_images -- the printable Tool Images
+        
+        Returns:
+            the selected Tool Images
 
-            if selected_tool_image is None:
-                tool_selection[selected_tool_types[tool_index]] = "<not selected>"
+        Exceptions:
+            typer.Abort -- if the user cancels the operation
+    """
+    dev_env_settings_panel = DevEnvSettingsWindow(printable_tool_images, already_selected_tool_images)
+    dev_env_settings_panel.wait_for_user()
 
-                panel_index -= 1
-                current_panel = panel_list[panel_index]
-                
-                if tool_index != 0:
-                    tool_index -= 1
-            else:
-                tool_selection[selected_tool_types[tool_index]] = selected_tool_image
-
-                tool_index += 1
-                
-                if tool_index == len(selected_tool_types):
-                    break
-
-                panel_index += 1
-                if len(panel_list) > panel_index:
-                    current_panel = panel_list[panel_index]
-                else:
-                    current_panel = ToolImageSelectorPanel(tool_image_list, selected_tool_types)
-                    panel_list.append(current_panel)
-
-                current_panel.dev_env_status.reset_table(selected_tool_types)
-
-            if isinstance(current_panel, ToolImageSelectorPanel):
-                current_panel.dev_env_status.set_tool_image(tool_selection)
-
-    dev_env_descriptor = {
-        "name": dev_env_name,
-        "tools": []
-    }
+    if "cancel" in dev_env_settings_panel.cancel_save_menu.get_selection():
+        raise typer.Abort()
 
-    for tool_type, tool_image in tool_selection.items():
+    return dev_env_settings_panel.tool_image_menu.get_selected_tool_images()
+
+def update_dev_env(dev_env: DevEnv, selected_tool_images: list[str]) -> None:
+    """ Update the Development Environment.
+    
+        Args:
+            dev_env -- the Development Environment
+            selected_tool_images -- the selected Tool Images
+    """
+    dev_env.tool_image_descriptors = []
+
+    for tool_image in selected_tool_images:
         if "/" in tool_image:
             registry, image = tool_image.split("/")
             image_name = registry + '/' + image.split(":")[0]
         else:
             image = tool_image
             image_name = image.split(":")[0]
-        tool_descriptor = {
-            "type": tool_type,
+
+        dev_env.tool_image_descriptors.append({
             "image_name": image_name,
             "image_version": image.split(":")[1]
-        }
-        dev_env_descriptor["tools"].append(tool_descriptor)
+        })
 
-    return dev_env_descriptor
-
-def create_new_dev_env(platform: Platform, new_dev_env_descriptor: dict) -> None:
-    """ Create a new Development Environment.
-        
+def modify_with_tui(platform: Platform, dev_env: DevEnv) -> None:
+    """ Modify the Dev Env with the TUI.
+    
         Args:
             platform -- the platform
-            new_dev_env_descriptor -- the descriptor of the new Development Environment
+            dev_env -- the Development Environment
+            
+        Exceptions:
+            typer.Abort -- if the user cancels the operation
     """
-    new_dev_env = DevEnv(new_dev_env_descriptor)
-    platform.local_dev_envs.append(new_dev_env)
+    already_selected_tool_images = get_already_selected_tool_images(dev_env)
+    remove_missing_tool_images(platform.tool_images.all_tool_images, already_selected_tool_images)
+    printable_tool_images = convert_to_printable_tool_images(platform.tool_images.all_tool_images)
+    selected_tool_images = open_dev_env_settings_panel(already_selected_tool_images, 
+                                                       printable_tool_images)
+    update_dev_env(dev_env, selected_tool_images)
+    confirmation = get_confirm_from_user()
+    handle_user_confirm(confirmation, dev_env, platform)
 
-def create_dev_env(platform: Platform, dev_env_name: str) -> None:
-    """ Create a new Development Environment or overwrite an existing one.
-        
+def execute(platform: Platform, dev_env_name: str) -> None:
+    """ Modify the Development Environment.
+    
         Args:
             platform -- the platform
             dev_env_name -- the name of the Development Environment
-
+            
         Exceptions:
-            Abort -- if the name of the Development Environment contains whitespace characters
+            typer.Abort -- if the user cancels the operation
     """
-    if ' ' in dev_env_name:
-        stderr.print("The name of the Development Environment cannot contain whitespace characters!")
-        raise typer.Abort()
 
-    dev_env_original = platform.get_dev_env_by_name(dev_env_name)
-    if dev_env_original is not None:
-        typer.confirm("The input name is already used by a Development Environment. Overwrite it?", 
-                      abort=True)
-
-        if dev_env_original.is_installed:
-            typer.confirm("The Development Environment is installed, so it can't be overwritten. " + \
-                          "Uninstall it first?", abort=True)
-            try:
-                platform.uninstall_dev_env(dev_env_original)
-            except PlatformError as e:
-                stderr.print(f"[red]{str(e)}[/]")
-                typer.Abort()
-
-    tool_image_list = get_tool_image_list(platform.tool_images)
-    new_dev_env_descriptor = get_dev_env_descriptor_from_user(dev_env_name, tool_image_list)
-    
-    if dev_env_original is not None:
-        dev_env_original.tools = new_dev_env_descriptor["tools"]
-    else:
-        create_new_dev_env(platform, new_dev_env_descriptor)
+    platform.assign_tool_image_instances_to_all_dev_envs()
 
-def execute(platform: Platform, dev_env_name: str) -> None:
-    """ Create a new Development Environment.
-        
-        Args:
-            platform -- the platform
-            dev_env_name -- the name of the Development Environment
+    dev_env = platform.get_dev_env_by_name(dev_env_name)
 
-        Exceptions:
-            Abort -- if the name of the Development Environment contains whitespace characters
-    """
-    create_dev_env(platform, dev_env_name)
-    platform.flush_descriptors()
-    stdout.print(f"The [green]{dev_env_name}[/] Development Environment has been created!")
-    stdout.print("Run [italic]dem install[/] to install it.")
+    if dev_env is None:
+        stderr.print("[red]The Development Environment doesn't exist.")
+        return
+    elif dev_env.is_installed is True:
+        stdout.print("[yellow]The Development Environment is installed, so it can't be modified.[/]")
+        typer.confirm("Do you want to uninstall it first?", abort=True)
+        try:
+            platform.uninstall_dev_env(dev_env)
+        except PlatformError as e:
+            stderr.print(f"[red]{str(e)}[/]")
+            return
+
+    modify_with_tui(platform, dev_env)
+    stdout.print("[green]The Development Environment has been modified successfully![/]")
```

### Comparing `axem_dem-0.3.1/dem/cli/command/del_cat_cmd.py` & `axem_dem-0.4.0/dem/cli/command/del_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/del_host_cmd.py` & `axem_dem-0.4.0/dem/cli/command/del_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/del_reg_cmd.py` & `axem_dem-0.4.0/dem/cli/command/del_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/delete_cmd.py` & `axem_dem-0.4.0/dem/cli/command/delete_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from dem.core.platform import Platform
 from dem.core.dev_env import DevEnv
 from dem.core.exceptions import PlatformError
 from dem.cli.console import stderr, stdout
 import typer
 
 def execute(platform: Platform, dev_env_name: str) -> None:
+
+
     dev_env_to_delete: DevEnv | None = platform.get_dev_env_by_name(dev_env_name)
 
     if dev_env_to_delete is None:
         stderr.print(f"[red]Error: The [bold]{dev_env_name}[/bold] Development Environment doesn't exist.")
     else:
         if dev_env_to_delete.is_installed:
             typer.confirm("The Development Environment is installed. Do you want to uninstall it?",
```

### Comparing `axem_dem-0.3.1/dem/cli/command/export_cmd.py` & `axem_dem-0.4.0/dem/cli/command/export_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     
     if not export_path.endswith(".json"):
         export_path += ".json"
 
     dev_env.export(export_path)
 
 def execute(platform: Platform, dev_env_name: str, export_path: str) -> None:
+
+
     dev_env = platform.get_dev_env_by_name(dev_env_name)
     if dev_env:
         try:
             export(dev_env, export_path)
         except FileNotFoundError:
             stderr.print("[red]Error: Invalid input path.[/]")
     else:
```

### Comparing `axem_dem-0.3.1/dem/cli/command/init_cmd.py` & `axem_dem-0.4.0/dem/cli/command/init_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 def execute(platform: Platform, project_path: str) -> None:
     """ Initialize a project at the given path.
 
         Args:
             platform -- the platform
             project_path -- the path to the project to initialize
     """
+
+
     if not os.path.isdir(project_path):
         stderr.print(f"[red]Error: The {project_path} path does not exist.[/]")
         return
 
     try:
         dev_env = DevEnv(descriptor_path=f"{project_path}/.axem/dev_env_descriptor.json")
     except FileNotFoundError as e:
```

### Comparing `axem_dem-0.3.1/dem/cli/command/install_cmd.py` & `axem_dem-0.4.0/dem/cli/command/install_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     """
         Install the given Development Environment.
         
         Args:
             platform -- the platform
             dev_env_name -- the name of the Development Environment to install
     """
+
+    platform.assign_tool_image_instances_to_all_dev_envs()
+
     dev_env_to_install: DevEnv | None = platform.get_dev_env_by_name(dev_env_name)
 
     if dev_env_to_install is None:
         stderr.print(f"[red]Error: The {dev_env_name} Development Environment does not exist.[/]")
     elif dev_env_to_install.is_installed == True:
         stderr.print(f"[red]Error: The {dev_env_name} Development Environment is already installed.[/]")
     else:
```

### Comparing `axem_dem-0.3.1/dem/cli/command/list_cat_cmd.py` & `axem_dem-0.4.0/dem/cli/command/list_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/list_cmd.py` & `axem_dem-0.4.0/dem/cli/command/list_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """list CLI command implementation."""
 # dem/cli/list_cmd.py
 
 from dem.core.platform import Platform
 from dem.core.dev_env import DevEnv
-from dem.core.tool_images import ToolImages
+from dem.core.tool_images import ToolImage
 from dem.cli.console import stdout, stderr
 from rich.table import Table
 
 (
     DEV_ENV_ORG_NOT_IN_REGISTRY,
     DEV_ENV_ORG_INSTALLED_LOCALLY,
     DEV_ENV_ORG_REINSTALL,
@@ -30,38 +30,46 @@
 dev_env_local_status_messages = {
     DEV_ENV_LOCAL_NOT_AVAILABLE: "[red]Error: Required image is not available![/]",
     DEV_ENV_LOCAL_REINSTALL: "Incomplete local install. The missing images are available in the registry. Use `dem pull` to reinstall.",
     DEV_ENV_LOCAL_INSTALLED: "Installed.",
 }
 
 def get_catalog_dev_env_status(platform: Platform, dev_env: DevEnv) -> str:
-    image_statuses = dev_env.check_image_availability(platform.tool_images)
-    if (ToolImages.NOT_AVAILABLE in image_statuses) or (ToolImages.LOCAL_ONLY in image_statuses):
+    image_statuses = []
+    for tool_image in dev_env.tool_images:
+        image_statuses.append(tool_image.availability)
+
+    if (ToolImage.NOT_AVAILABLE in image_statuses) or (ToolImage.LOCAL_ONLY in image_statuses):
         dev_env_status = dev_env_org_status_messages[DEV_ENV_ORG_NOT_IN_REGISTRY]
-    elif (image_statuses.count(ToolImages.LOCAL_AND_REGISTRY) == len(image_statuses)) and \
+    elif (image_statuses.count(ToolImage.LOCAL_AND_REGISTRY) == len(image_statuses)) and \
             platform.get_dev_env_by_name(dev_env.name):
         dev_env_status = dev_env_org_status_messages[DEV_ENV_ORG_INSTALLED_LOCALLY]
     else:
         if platform.get_dev_env_by_name(dev_env.name):
             dev_env_status = dev_env_org_status_messages[DEV_ENV_ORG_REINSTALL]
         else:
             dev_env_status = dev_env_org_status_messages[DEV_ENV_ORG_READY]
     return dev_env_status
 
-def get_local_dev_env_status(dev_env: DevEnv, tool_images: ToolImages) -> str:
-    image_statuses = dev_env.check_image_availability(tool_images)
-    if (ToolImages.NOT_AVAILABLE in image_statuses):
+def get_local_dev_env_status(dev_env: DevEnv, tool_images: ToolImage) -> str:
+    image_statuses = []
+    for tool_image in dev_env.tool_images:
+        image_statuses.append(tool_image.availability)
+
+    if (ToolImage.NOT_AVAILABLE in image_statuses):
         dev_env_status = dev_env_local_status_messages[DEV_ENV_LOCAL_NOT_AVAILABLE]
-    elif (ToolImages.REGISTRY_ONLY in image_statuses):
+    elif (ToolImage.REGISTRY_ONLY in image_statuses):
         dev_env_status = dev_env_local_status_messages[DEV_ENV_LOCAL_REINSTALL]
     else:
         dev_env_status = dev_env_local_status_messages[DEV_ENV_LOCAL_INSTALLED]
     return dev_env_status
 
 def list_dev_envs(platform: Platform, local: bool, org: bool)-> None:
+
+
     table = Table()
     table.add_column("Development Environment")
     table.add_column("Status")
 
     if ((local == True) and (org == False)):
         if not platform.local_dev_envs:
             stdout.print("[yellow]No installed Development Environments.[/]")
```

### Comparing `axem_dem-0.3.1/dem/cli/command/list_host_cmd.py` & `axem_dem-0.4.0/dem/cli/command/list_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/list_reg_cmd.py` & `axem_dem-0.4.0/dem/cli/command/list_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/cli/command/load_cmd.py` & `axem_dem-0.4.0/dem/cli/command/load_cmd.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,33 +8,35 @@
 
 def check_is_file_exist(param: str | None) -> bool:
     if param is not None:
         return(os.path.isfile(param))     
     else:
         return False
 
-def load_dev_env_to_dev_env_json(dev_env_local_setup: Platform,path_to_dev_env: str) -> bool:
+def load_dev_env_to_dev_env_json(platform: Platform,path_to_dev_env: str) -> bool:
     raw_file = open(path_to_dev_env, "r")   
             
     try:
         dev_env = json.load(raw_file)
         
-        if dev_env_local_setup.get_dev_env_by_name(dev_env["name"]) is not None:
+        if platform.get_dev_env_by_name(dev_env["name"]) is not None:
             stderr.print("[red]Error: The Development Environment exist.[/]")
             return False                       
         else:        
-            new_dev_env = DevEnv(dev_env)
-            dev_env_local_setup.local_dev_envs.append(new_dev_env)
+            new_dev_env: DevEnv = DevEnv(dev_env)
+            platform.local_dev_envs.append(new_dev_env)
     except json.decoder.JSONDecodeError:
        stderr.print("[red]Error: invalid json format.[/]")
        return False                       
     else:
         raw_file.close()
         return True
 
 def execute(platform: Platform, path_to_dev_env: str) -> None:
+
+
     if check_is_file_exist(path_to_dev_env) is True:                
         retval = load_dev_env_to_dev_env_json(platform,path_to_dev_env)        
         if retval == True:
             platform.flush_descriptors()
     else:
         stderr.print("[red]Error: The input file does not exist.[/]")
```

### Comparing `axem_dem-0.3.1/dem/cli/command/rename_cmd.py` & `axem_dem-0.4.0/dem/cli/command/rename_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """rename CLI command implementation."""
 # dem/cli/command/rename_cmd.py
 
 from dem.core.platform import Platform
 from dem.cli.console import stderr
 
 def execute(platform: Platform, dev_env_name_to_rename: str, new_dev_env_name: str) -> None:
+
+
     dev_env_to_rename = platform.get_dev_env_by_name(dev_env_name_to_rename)
 
     if dev_env_to_rename is not None:
         dev_env_to_rename.name = new_dev_env_name
         platform.flush_descriptors()
     else:
         stderr.print("[red]Error: The input Development Environment does not exist.[/]")
```

### Comparing `axem_dem-0.3.1/dem/cli/command/run_cmd.py` & `axem_dem-0.4.0/dem/cli/command/run_cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,30 +28,29 @@
     """ Execute the run command in the given Dev Env context. If something is wrong with the Dev 
         Env the DEM can try to fix it.
 
         Args:
             dev_env_name -- name of the Development Environment
             container_arguments -- arguments passed to the container
     """
-    
+
+
     dev_env_local = platform.get_dev_env_by_name(dev_env_name)
 
     if dev_env_local is None:
         stderr.print("[red]Error: Unknown Development Environment: " + dev_env_name + "[/]")
-        raise(typer.Abort)
+        raise typer.Abort()
     else:
-        # Update the tool images manually.
-        Platform.update_tool_images_on_instantiation = False
         # Only the local images are needed.
-        platform.tool_images.local.update()
+        Platform.local_only = True
 
         missing_tool_images = set()
-        for tool in dev_env_local.tools:
+        for tool in dev_env_local.tool_image_descriptors:
             tool_image = tool["image_name"] + ":" + tool["image_version"]
             # Check if the required tool image exists locally.
-            if tool_image not in platform.tool_images.local.elements:
+            if tool_image not in platform.tool_images.get_local_ones().keys():
                 missing_tool_images.add(tool_image)
 
         if missing_tool_images:
             handle_missing_tool_images(missing_tool_images, dev_env_local, platform)
 
         platform.container_engine.run(container_arguments)
```

### Comparing `axem_dem-0.3.1/dem/cli/command/uninstall_cmd.py` & `axem_dem-0.4.0/dem/cli/command/uninstall_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     """
         Uninstall the given Development Environment.
         
         Args:
             platform -- the platform
             dev_env_name -- the name of the Development Environment to uninstall
     """
+
+
     dev_env_to_uninstall: DevEnv | None = platform.get_dev_env_by_name(dev_env_name)
 
     if dev_env_to_uninstall is None:
         stderr.print(f"[red]Error: The {dev_env_name} Development Environment does not exist.[/]")
     elif not dev_env_to_uninstall.is_installed:
         stderr.print(f"[red]Error: The {dev_env_name} Development Environment is not installed.[/]")
     else:
```

### Comparing `axem_dem-0.3.1/dem/cli/main.py` & `axem_dem-0.4.0/dem/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,24 +176,22 @@
     if platform:
         rename_cmd.execute(platform, dev_env_name,new_dev_env_name)
     else:
         raise InternalError("Error: The platform hasn't been initialized properly!")
 
 @typer_cli.command()
 def modify(dev_env_name: Annotated[str, typer.Argument(help="Name of the Development Environment to modify.",
-                                                       autocompletion=autocomplete_dev_env_name)],
-           tool_type: Annotated[str, typer.Argument(help="The tool type to change.")] = "",
-           tool_image: Annotated[str, typer.Argument(help="The tool image to set for the tool type.")] = "") -> None:
+                                                       autocompletion=autocomplete_dev_env_name)]) -> None:
     """
     Change a tool in a Development Environment.
 
     If the tool type is not specified, the Dev Env settings panel will be opened.
     """
     if platform:
-        modify_cmd.execute(platform, dev_env_name, tool_type, tool_image)
+        modify_cmd.execute(platform, dev_env_name)
     else:
         raise InternalError("Error: The platform hasn't been initialized properly!")
 
 @typer_cli.command()
 def delete(dev_env_name: Annotated[str, typer.Argument(help="Name of the Development Environment to delete.",
                                                        autocompletion=autocomplete_dev_env_name)]) -> None:
     """
```

### Comparing `axem_dem-0.3.1/dem/cli/tui/renderable/menu.py` & `axem_dem-0.4.0/dem/cli/tui/renderable/menu.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Menu TUI renderable."""
 # dem/cli/tui/renderable/menu.py
 
+from dem.cli.tui.printable_tool_image import PrintableToolImage
 from rich import live, table, align, panel, box
+from rich.console import RenderableType
+
 from readchar import readkey, key
 
 class BaseMenu(table.Table):
     """ Base class for the menus.
     
-        Shouldn't be instantiated directly.
-        
         Class attributes:
             cursor_on -- text that represents the cursor
             cursor_off -- the cursor is not in this cell
     """
     cursor_on = "* "
     cursor_off = "  "
 
@@ -167,21 +168,21 @@
         """
         match input:
             case key.LEFT | 'h':
                 self.move_cursor(self.CURSOR_LEFT)
             case key.RIGHT | 'l':
                 self.move_cursor(self.CURSOR_RIGHT)
 
-class CancelNextMenu(HorizontalMenu):
-    """ Horizontal menu with two items: cancel and next.
+class CancelSaveMenu(HorizontalMenu):
+    """ Horizontal menu with two items: cancel and save.
     
         Class attributes:
             menu_items -- the menu items with rich text formatting
     """
-    menu_items = ("[underline]cancel[/]", "[underline]next[/]")
+    menu_items = ("[underline]cancel[/]", "[underline]save[/]")
     
     def __init__(self) -> None:
         """ Construct a HorizontalMenu with 2 columns and 1 row."""
         super().__init__()
         self.add_row(self.cursor_off + self.menu_items[0], 
                      self.cursor_off + self.menu_items[1])
         self.is_selected = False
@@ -200,131 +201,67 @@
     def get_selection(self) -> str:
         """ Get the selected item.
         
             Return with the selected item.
         """
         return self.columns[self.cursor_pos]._cells[0]
 
-class BackMenu(HorizontalMenu):
-    """ Horizontal menu with a single item: back.
-    
-        Class attributes:
-            menu_item -- the menu item with rich text formatting
-    """
-    menu_item = "[underline]back[/]"
-
-    def __init__(self) -> None:
-        """ Construct a HorizontalMenu with 1 column and 1 row."""
-        super().__init__()
-        self.add_row(self.cursor_off + self.menu_item)
-        self.is_selected = False
-
-    def handle_user_input(self, input: str) -> None:
-        """ Handle user input.
-        
-            Args:
-                input -- the user input (handle enter)
-        """
-        if input is key.ENTER:
-            self.is_selected = True
-
-class ToolTypeMenu(VerticalMenu):
-    """ Vertical menu for the tool type selection.
-    
-        Class attributes:
-            selected -- selected text
-            not_selected -- not selected text
-    """
-    selected = "[green]yes[/]"
-    not_selected = "no"
-
-    def __init__(self, supported_tool_types: list[str]) -> None:
-        """ Construct a VerticalMenu with 2 columns and rows that contain the supported tool types.
-        
-            Args:
-                supported_tool_types -- the supported tool types
-        """
-        super().__init__()
-        self.add_column("Tool types")
-        self.add_column("Selected")
-
-        for index, tool_type in enumerate(supported_tool_types):
-            if (index == 0):
-                # Set the cursor indicator for the first element.
-                self.add_row(self.cursor_on + tool_type, self.not_selected)
-            else:
-                self.add_row(self.cursor_off + tool_type, self.not_selected)
-
-    def preset_selection(self, already_selected: list[str]) -> None:
-        """ Preset the given tool types.
-        
-            Args:
-                already_selected -- list of tool types to set as selected
-        """
-        for row_idx, cell in enumerate(self.columns[0]._cells):
-            if cell[2:] in already_selected:
-                self.columns[1]._cells[row_idx] = self.selected
-
-    def toggle_select(self) -> None:
-        """ Toggle selection at the cursor's position. """
-        if (self.columns[1]._cells[self.cursor_pos] is self.selected):
-            self.columns[1]._cells[self.cursor_pos] = self.not_selected
-        else:
-            self.columns[1]._cells[self.cursor_pos] = self.selected
-
-    def handle_user_input(self, input: str) -> None:
-        """ Handle user input or pass to parent.
-        
-            Args:
-                input -- the user input (handle enter or space)
-        """
-        if (input == key.ENTER) or (input == ' '):
-            self.toggle_select()
-        else:
-            super().handle_user_input(input)
-
-    def get_selected_tool_types(self) -> list[str]:
-        """ Get selected tool types.
-
-            Returns with a list of tool types that are in selected state.
-        """
-        selected_tool_types = []
-        for row_index, cell in enumerate(self.columns[1]._cells):
-            if cell == self.selected:
-                selected_tool_types.append(self.columns[0]._cells[row_index][2:])
-        return selected_tool_types
-
 class ToolImageMenu(VerticalMenu):
-    def __init__(self, tool_images: list[list[str]]) -> None:
+    def __init__(self, printable_tool_images: list[PrintableToolImage],
+                 already_selected_tool_images: list[str]) -> None:
         super().__init__()
+        self.title = "Select the tool images for the Development Environment:"
         self.add_column("Tool images", no_wrap=True)
         self.add_column("Availability", no_wrap=True)
+        self.tool_image_selection = []
 
-        for index, tool_image in enumerate(tool_images):
+        for index, tool_image in enumerate(printable_tool_images):
+            row_content = []
             if (index == 0):
                 # Set the cursor indicator for the first element.
-                self.add_row("* " + tool_image[0], tool_image[1])
+                row_content = "* " + tool_image.name, tool_image.status
             else:
-                self.add_row("  " + tool_image[0], tool_image[1])
+                row_content = "  " + tool_image.name, tool_image.status
 
-        self.is_selected = False
+            if tool_image.name in already_selected_tool_images:
+                self.tool_image_selection.append(tool_image.name)
+                row_content = f"{row_content[0][:2]}[green]{row_content[0][2:]}[/]", str(row_content[1])
+            
+            self.add_row(*row_content)
+    
+    def get_table_width(self) -> int:
+        return sum(self._measure_column)
 
     def handle_user_input(self, input: str) -> None:
-        if input == key.ENTER:
-            self.is_selected = True
+        if input == key.ENTER or input == key.SPACE:
+            selected_cell = self.columns[0]._cells[self.cursor_pos]
+
+            if "[green]" in selected_cell:
+                selected_cell = selected_cell.replace("[green]", "")
+                selected_cell = selected_cell.replace("[/]", "")
+            else:
+                selected_cell = f"{selected_cell[:2]}[green]{selected_cell[2:]}[/]"
+
+            self.columns[0]._cells[self.cursor_pos] = selected_cell
         else:
             super().handle_user_input(input)
 
-    def get_selected_tool_image(self) -> str:
-        return self.columns[0]._cells[self.cursor_pos][2:]
+    def get_selected_tool_images(self) -> list[str]:
+        for cell in self.columns[0]._cells:
+            tool_image_name = cell[2:].replace("[/]", "").replace("[green]", "")
+            if ("[green]" in cell) and (tool_image_name not in self.tool_image_selection):
+                self.tool_image_selection.append(tool_image_name)
+            elif ("[green]" not in cell) and (tool_image_name in self.tool_image_selection):
+                self.tool_image_selection.remove(tool_image_name)
+        
+        return self.tool_image_selection
 
 class SelectMenu(VerticalMenu):
     def __init__(self, selection: list[str]) -> None:
         super().__init__()
-        self.alignment = align.Align(self, align="center", vertical="middle")
         self.show_edge = False
         self.show_lines = False
 
         for index, element in enumerate(selection):
             if (index == 0):
                 # Set the cursor indicator for the first element.
                 self.add_row("* " + element)
@@ -347,37 +284,21 @@
     def get_selected(self) -> str:
         return self.columns[0]._cells[self.cursor_pos][2:]
     
     def set_title(self, title: str) -> None:
         self.width = len(title)
         super().set_title(title)
 
-class DevEnvStatus(panel.Panel):
-    def __init__(self, tool_types: list[str]) -> None:
-        self.outer_table = table.Table(box=None)
-        super().__init__(self.outer_table, title="Development Environment", expand=False)
-        self.aligned_renderable = align.Align(self, vertical="middle")
-        
-        self._fill_table(tool_types)
-    
-    def _fill_table(self, tool_types: list[str]) -> None:
-        panel_height = 3 + len(tool_types) * 4
-        self.height = panel_height
-
-        for tool_type in tool_types:
-            inner_table = table.Table(box=None)
-            inner_table.add_row("[bold]" + tool_type + ":[/]")
-            inner_table.add_row("<not selected>")
-            inner_table.add_row("")
-
-            self.outer_table.add_row(inner_table)
-
-    def reset_table(self, tool_types: list[str]) -> None:
-        self.outer_table = table.Table(box=None)
-        self._fill_table(tool_types)
-        self.renderable = self.outer_table
-
-    def set_tool_image(self, tool_selection: dict) -> None:
-        for tool_type, tool_image in tool_selection.items():
-            for row in self.outer_table.columns[0].cells:
-                if tool_type in row.columns[0]._cells[0]:
-                    row.columns[0]._cells[1] = tool_image
+class DevEnvStatusPanel(table.Table):
+    def __init__(self, selected_tool_images: list[str], height: int, width: int) -> None:
+        super().__init__(title="Dev Env Settings")
+        self.add_column("Selected Tool Images", no_wrap=True)
+
+        if height > 10:
+            height = 10
+
+        for tool_image in selected_tool_images:
+            self.add_row(tool_image)
+
+        if len(selected_tool_images) < height:
+            for _ in range(height - len(selected_tool_images)):
+                self.add_row(" " * width)
```

### Comparing `axem_dem-0.3.1/dem/cli/tui/tui_user_output.py` & `axem_dem-0.4.0/dem/cli/tui/tui_user_output.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/core/container_engine.py` & `axem_dem-0.4.0/dem/core/container_engine.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/core/core.py` & `axem_dem-0.4.0/dem/core/core.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/core/data_management.py` & `axem_dem-0.4.0/dem/core/data_management.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/core/dev_env.py` & `axem_dem-0.4.0/dem/cli/command/create_cmd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,124 +1,123 @@
-"""This module represents a Development Environment."""
-# dem/core/dev_env.py
+"""create CLI command implementation."""
+# dem/cli/command/create_cmd.py
 
-from dem.core.tool_images import ToolImages
-import json, os
-
-class DevEnv():
-    """ A Development Environment.
-        
-        Class variables:
-            supported_tool_types -- supported tool types
-    """ 
-    supported_tool_types = ( 
-        "build system",
-        "toolchain",
-        "debugger",
-        "deployer",
-        "test framework",
-        "CI/CD server",
-    )
-
-    def __init__(self, descriptor: dict | None = None, descriptor_path: str | None = None) -> None:
-        """ Init the DevEnv class. 
-        
-            A new instance can be created:
-            - from a Dev Env descriptor
-            - from a descriptor avaialable at the given path.
-
-            Only one of the arguments can be used at a time.
-        
-            Args:
-                descriptor -- the description of the Development Environment from the dev_env.json 
-                              file
-                descriptor_path -- the path of the descriptor file
-
-            Exceptions:
-                ValueError -- if more than one of the arguments is not None
-        """
-
-        # Only one of the arguments can be not None
-        if sum(arg is not None for arg in [descriptor, descriptor_path]) > 1:
-            raise ValueError("Only one of the arguments can be not None.")
-
-        if descriptor_path:
-            if not os.path.exists(descriptor_path):
-                raise FileNotFoundError("dev_env_descriptor.json doesn't exist.")
-            with open(descriptor_path, "r") as file:
-                descriptor = json.load(file)
-
-        self.name: str = descriptor["name"]
-        self.tools: list[dict[str, str]] = descriptor["tools"]
-        descriptor_installed = descriptor.get("installed", "False")
-        if "True" == descriptor_installed:
-            self.is_installed = True
-        else:
-            self.is_installed = False
-
-    def check_image_availability(self, all_tool_images: ToolImages, 
-                                 update_tool_image_store: bool = False,
-                                 local_only: bool = False) -> list:
-        """ Checks the tool image's availability.
-        
-            Updates the "image_status" key for the tool dictionary.
-            Returns with the statuses of the Dev Env tool images.
-
-            Args:
-                all_tool_images -- the images the Dev Envs can access
-                update_tool_images -- update the list of available tool images
-                local_only -- only local images are used
-        """
-        if update_tool_image_store == True:
-            all_tool_images.local.update()
-            if local_only is False:
-                all_tool_images.registry.update()
-
-        local_tool_images = all_tool_images.local.elements
-
-        if local_only is True:
-            registry_tool_images = []
+import typer
+from dem.core.dev_env import DevEnv
+from dem.core.tool_images import ToolImage
+from dem.core.platform import Platform
+from dem.core.exceptions import PlatformError
+from dem.cli.console import stdout, stderr
+from dem.cli.tui.window.dev_env_settings_window import DevEnvSettingsWindow
+from dem.cli.tui.printable_tool_image import convert_to_printable_tool_images
+
+def open_dev_env_settings_panel(all_tool_images: dict[str, ToolImage]) -> list[str]:
+    """ Open the Development Environment settings panel.
+        
+        Args:
+            all_tool_images -- the Tool Images
+
+        Returns:
+            the selected Tool Image names
+    """
+    dev_env_settings_panel = DevEnvSettingsWindow(convert_to_printable_tool_images(all_tool_images))
+    dev_env_settings_panel.wait_for_user()
+
+    if "cancel" in dev_env_settings_panel.cancel_save_menu.get_selection():
+        raise typer.Abort()
+
+    return dev_env_settings_panel.tool_image_menu.get_selected_tool_images()
+
+def create_new_dev_env_descriptor(dev_env_name: str, selected_tool_images: list[str]) -> dict:
+    """ Create a new Development Environment descriptor.
+        
+        Args:
+            dev_env_name -- the name of the Development Environment
+            selected_tool_images -- the selected Tool Images
+
+        Returns:
+            the descriptor of the new Development Environment
+    """
+    dev_env_descriptor = {
+        "name": dev_env_name,
+        "tools": []
+    }
+
+    for tool_image in selected_tool_images:
+        if "/" in tool_image:
+            registry, image = tool_image.split("/")
+            image_name = registry + '/' + image.split(":")[0]
         else:
-            registry_tool_images = all_tool_images.registry.elements
+            image = tool_image
+            image_name = image.split(":")[0]
 
-        image_statuses = []
-        for tool in self.tools:
-            tool_image_name = tool["image_name"] + ':' + tool["image_version"]
-            if (tool_image_name in local_tool_images) and (tool_image_name in registry_tool_images):
-                image_status = ToolImages.LOCAL_AND_REGISTRY
-            elif (tool_image_name in local_tool_images):
-                image_status = ToolImages.LOCAL_ONLY
-            elif (tool_image_name in registry_tool_images):
-                image_status = ToolImages.REGISTRY_ONLY
-            else:
-                image_status = ToolImages.NOT_AVAILABLE
-            image_statuses.append(image_status)
-            tool["image_status"] = image_status
-
-        return image_statuses
-
-    def get_deserialized(self, omit_is_installed: bool = False) -> dict[str, str]:
-        """ Create the deserialized json. 
-        
-            Return the Dev Env as a dict.
-        """
-        dev_env_json_deserialized: dict = {
-            "name": self.name,
-            "tools": self.tools
+        tool_descriptor = {
+            "image_name": image_name,
+            "image_version": image.split(":")[1]
         }
-        
-        if omit_is_installed is False:
-            if self.is_installed:
-                dev_env_json_deserialized["installed"] = "True"
-            else:
-                dev_env_json_deserialized["installed"] = "False"
+        dev_env_descriptor["tools"].append(tool_descriptor)
 
-        return dev_env_json_deserialized
+    return dev_env_descriptor
 
-    def export(self, path: str) -> None:
-        """ Export the Dev Env to a file.
+def create_new_dev_env(platform: Platform, new_dev_env_descriptor: dict) -> None:
+    """ Create a new Development Environment.
         
-            Args:
-                path -- the path of the file to export the Dev Env to
-        """
-        with open(path, "w") as file:
-            json.dump(self.get_deserialized(True), file, indent=4)
+        Args:
+            platform -- the platform
+            new_dev_env_descriptor -- the descriptor of the new Development Environment
+    """
+    dev_env = DevEnv(descriptor=new_dev_env_descriptor)
+    dev_env.assign_tool_image_instances(platform.tool_images)
+    platform.local_dev_envs.append(dev_env)
+
+def create_dev_env(platform: Platform, dev_env_name: str) -> None:
+    """ Create a new Development Environment or overwrite an existing one.
+        
+        Args:
+            platform -- the platform
+            dev_env_name -- the name of the Development Environment
+
+        Exceptions:
+            Abort -- if the name of the Development Environment contains whitespace characters
+    """
+    if ' ' in dev_env_name:
+        stderr.print("The name of the Development Environment cannot contain whitespace characters!")
+        raise typer.Abort()
+
+    dev_env_original = platform.get_dev_env_by_name(dev_env_name)
+    if dev_env_original is not None:
+        typer.confirm("The input name is already used by a Development Environment. Overwrite it?", 
+                      abort=True)
+
+        if dev_env_original.is_installed:
+            typer.confirm("The Development Environment is installed, so it can't be overwritten. " + \
+                          "Uninstall it first?", abort=True)
+            try:
+                platform.uninstall_dev_env(dev_env_original)
+            except PlatformError as e:
+                stderr.print(f"[red]{str(e)}[/]")
+                raise typer.Abort()
+
+    selected_tool_images = open_dev_env_settings_panel(platform.tool_images.all_tool_images)
+    new_dev_env_descriptor = create_new_dev_env_descriptor(dev_env_name, selected_tool_images)
+    
+    if dev_env_original is not None:
+        dev_env_original.tool_image_descriptors = new_dev_env_descriptor["tools"]
+    else:
+        create_new_dev_env(platform, new_dev_env_descriptor)
+
+def execute(platform: Platform, dev_env_name: str) -> None:
+    """ Create a new Development Environment.
+        
+        Args:
+            platform -- the platform
+            dev_env_name -- the name of the Development Environment
+
+        Exceptions:
+            Abort -- if the name of the Development Environment contains whitespace characters
+    """
+    platform.assign_tool_image_instances_to_all_dev_envs()
+
+    create_dev_env(platform, dev_env_name)
+    platform.flush_descriptors()
+    stdout.print(f"The [green]{dev_env_name}[/] Development Environment has been created!")
+    stdout.print("Run [italic]dem install[/] to install it.")
```

### Comparing `axem_dem-0.3.1/dem/core/dev_env_catalog.py` & `axem_dem-0.4.0/dem/core/dev_env_catalog.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/core/exceptions.py` & `axem_dem-0.4.0/dem/core/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     def __init__(self, message: str = "") -> None:
         super().__init__(self.base_message + message)
 
 class RegistryError(Exception):
     """Raised when the communication with registry fails."""
     pass
 
+class ToolImageError(Exception):
+    """Raised when there is a problem with the tool image."""
+    pass
+
 class ContainerEngineError(Exception):
     """Raised when there is a problem with the container engine."""
 
     base_message = "Container engine error: "
 
     def __init__(self, message: str) -> None:
         super().__init__(self.base_message + message)
```

### Comparing `axem_dem-0.3.1/dem/core/hosts.py` & `axem_dem-0.4.0/dem/core/hosts.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/dem/core/platform.py` & `axem_dem-0.4.0/dem/core/platform.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,31 +6,28 @@
 from dem.core.core import Core
 from dem.core.properties import __supported_dev_env_major_version__
 from dem.core.exceptions import DataStorageError, PlatformError, ContainerEngineError
 from dem.core.dev_env_catalog import DevEnvCatalogs
 from dem.core.data_management import LocalDevEnvJSON
 from dem.core.container_engine import ContainerEngine
 from dem.core.registry import Registries
-from dem.core.tool_images import ToolImages
+from dem.core.tool_images import ToolImages, ToolImage
 from dem.core.dev_env import DevEnv
 from dem.core.hosts import Hosts
 
 class Platform(Core):
     """ Representation of the Development Platform:
         - The available tool images.
         - The available Development Environments.
         - External resources.
 
         Class variables:
-            _tool_images -- the available tool images
-            _container_engine -- the container engine
-            _regisitries -- managing the registries
-            update_tool_images_on_instantiation -- can be used to disable tool update if not needed
+            local_only -- work with the local tool images only
     """
-    update_tool_images_on_instantiation = True
+    local_only = False
 
     def _dev_env_json_version_check(self, dev_env_json_major_version: int) -> None:
         """ Check that the json file is supported.
 
             The version is stored as a string in the X.Y format.
             Raises an DataStorageError exception, if the version is not supported.
         """
@@ -43,32 +40,40 @@
         self._dev_env_catalogs: DevEnvCatalogs | None = None
         self._tool_images = None
         self._container_engine = None
         self._registries = None
         self._hosts = None
 
     def load_dev_envs(self) -> None:
-        """ Load the Development Environments from the dev_env.json file."""
+        """ Load the Development Environments from the dev_env.json file.
+        
+            The Dev Envs will only contain the descriptors and not the ToolImage instances.
+        """
         self.dev_env_json = LocalDevEnvJSON()
         self.dev_env_json.update()
         self.version = self.dev_env_json.deserialized["version"]
         self._dev_env_json_version_check(int(self.version.split('.', 1)[0]))
         self.local_dev_envs: list[DevEnv] = []
         for dev_env_descriptor in self.dev_env_json.deserialized["development_environments"]:
             self.local_dev_envs.append(DevEnv(descriptor=dev_env_descriptor))
 
+    def assign_tool_image_instances_to_all_dev_envs(self) -> None:
+        """ Assign the ToolImage instances to all Development Environments."""
+        for dev_env in self.local_dev_envs:
+            dev_env.assign_tool_image_instances(self.tool_images)
+
     @property
     def tool_images(self) -> ToolImages:
         """ The tool images.
 
             The ToolImages() gets instantiated only at the first access.
         """
         if self._tool_images is None:
-            self._tool_images = ToolImages(self.container_engine, self.registries,
-                                          self.update_tool_images_on_instantiation)
+            self._tool_images = ToolImages(self.container_engine, self.registries)
+            self._tool_images.update(local_only=self.local_only)
         return self._tool_images
     
     @property
     def container_engine(self) -> ContainerEngine:
         """ The container engine.
 
             The ContainerEngine() gets instantiated only at the first access.
@@ -140,29 +145,27 @@
 
     def install_dev_env(self, dev_env_to_install: DevEnv) -> None:
         """ Install the Dev Env by pulling the required images.
         
             Args:
                 dev_env_to_install -- the Development Environment to install
         """
-        dev_env_to_install.check_image_availability(self.tool_images, False)
-
-        # First check if the missing images are available in the registries.
-        for tool in dev_env_to_install.tools:
-            if tool["image_status"] == ToolImages.NOT_AVAILABLE:
-                raise PlatformError(f"The {tool['image_name']}:{tool['image_version']} image is not available.")
-
-        for tool in dev_env_to_install.tools:
-            if tool["image_status"] == ToolImages.REGISTRY_ONLY:
-                self.user_output.msg(f"\nPulling image {tool['image_name']}:{tool['image_version']}", 
-                                     is_title=True)
+        # First check if the missing images are available in the registries, so DEM won't start to 
+        # pull the images and then fail.
+        for tool_image in dev_env_to_install.tool_images:
+            if tool_image.availability == ToolImage.NOT_AVAILABLE:
+                raise PlatformError(f"The {tool_image.name} image is not available.")
+
+        for tool_image in dev_env_to_install.tool_images:
+            if tool_image.availability == ToolImage.REGISTRY_ONLY:
+                self.user_output.msg(f"\nPulling image {tool_image.name}", is_title=True)
                 try:                
-                    self.container_engine.pull(f"{tool['image_name']}:{tool['image_version']}")
+                    self.container_engine.pull(tool_image.name)
                 except ContainerEngineError as e:
-                    raise PlatformError(f"Dev Env install failed. Reason: {str(e)}")
+                    raise PlatformError(f"Dev Env install failed. --> {str(e)}")
 
         dev_env_to_install.is_installed = True
         self.flush_descriptors()
 
     def uninstall_dev_env(self, dev_env_to_uninstall: DevEnv) -> None:
         """ Uninstall the Dev Env by removing the images not required anymore.
 
@@ -171,28 +174,28 @@
 
             Exceptions:
                 PlatformError -- if the uninstall fails
         """
         all_required_tool_images = set()
         for dev_env in self.local_dev_envs:
             if (dev_env is not dev_env_to_uninstall) and dev_env.is_installed:
-                for tool in dev_env.tools:
-                    all_required_tool_images.add(tool["image_name"] + ":" + tool["image_version"])
+                for tool_image_descriptor in dev_env.tool_image_descriptors:
+                    all_required_tool_images.add(tool_image_descriptor["image_name"] + ":" + tool_image_descriptor["image_version"])
 
         tool_images_to_remove = set()
-        for tool in dev_env_to_uninstall.tools:
-            tool_image = tool["image_name"] + ":" + tool["image_version"]
-            if tool_image not in all_required_tool_images:
-                tool_images_to_remove.add(tool_image)
+        for tool_image_descriptor in dev_env_to_uninstall.tool_image_descriptors:
+            tool_image_name = tool_image_descriptor["image_name"] + ":" + tool_image_descriptor["image_version"]
+            if tool_image_name not in all_required_tool_images:
+                tool_images_to_remove.add(tool_image_name)
 
-        for tool_image in tool_images_to_remove:
+        for tool_image_name in tool_images_to_remove:
             try:
-                self.container_engine.remove(tool_image)
+                self.container_engine.remove(tool_image_name)
             except ContainerEngineError as e:
-                raise PlatformError(f"Dev Env uninstall failed. <-caused by- {str(e)}")
+                raise PlatformError(f"Dev Env uninstall failed. --> {str(e)}")
             
         dev_env_to_uninstall.is_installed = False
         self.flush_descriptors()
 
     def flush_descriptors(self) -> None:
         """ Writes the deserialized json to the dev_env.json file."""
         # Get the up-to-date deserialized data.
@@ -227,14 +230,15 @@
                 assigned_dev_env -- the Development Environment assigned to the project
         """
         descriptor_path = f"{project_path}/.axem/dev_env_descriptor.json"
         if not os.path.exists(descriptor_path):
             raise FileNotFoundError(f"The {descriptor_path} file does not exist.")
 
         assigned_dev_env = DevEnv(descriptor_path=descriptor_path)
+        assigned_dev_env.assign_tool_image_instances(self.tool_images)
         existing_dev_env = self.get_dev_env_by_name(assigned_dev_env.name)
         if existing_dev_env is not None:
             self.user_output.get_confirm("[yellow]This project is already initialized.[/]", 
                                          "Overwrite it?")
             self.local_dev_envs.remove(existing_dev_env)
 
         self.local_dev_envs.append(assigned_dev_env)
```

### Comparing `axem_dem-0.3.1/dem/core/registry.py` & `axem_dem-0.4.0/dem/core/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Direct access to the registry over HTTP. or using the container engine."""
 # dem/core/registry.py
 
 from dem.core.core import Core
 from dem.core.container_engine import ContainerEngine
-from dem.core.data_management import ConfigFile
 import requests
 from typing import Generator
 from abc import ABC, abstractmethod
 
 class Registry(Core, ABC):
     """ Abstract base class for a registry."""
     def __init__(self, container_engine: ContainerEngine, registry_config: dict) -> None:
```

### Comparing `axem_dem-0.3.1/dem/core/user_output.py` & `axem_dem-0.4.0/dem/core/user_output.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.3.1/pyproject.toml` & `axem_dem-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "axem-dem"
-version = "0.3.1"
+version = "0.4.0"
 description = "Manager for Containerized Development Environments"
 authors = ["Janos Murai <janos.murai@axemsolutions.io>"]
 license = "Eclipse Public License - v2.0"
 readme = "README.md"
 homepage = "https://axemsolutions.io/"
 documentation = "https://axemsolutions.io/dem_doc/"
 repository = "https://github.com/axem-solutions/dem"
```

### Comparing `axem_dem-0.3.1/PKG-INFO` & `axem_dem-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axem-dem
-Version: 0.3.1
+Version: 0.4.0
 Summary: Manager for Containerized Development Environments
 Home-page: https://axemsolutions.io/
 License: Eclipse Public License - v2.0
 Keywords: iot,embedded,edge,development environment,tools,containers
 Author: Janos Murai
 Author-email: janos.murai@axemsolutions.io
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: axem-dem Version: 0.3.1 Summary: Manager for
+Metadata-Version: 2.1 Name: axem-dem Version: 0.4.0 Summary: Manager for
 Containerized Development Environments Home-page: https://axemsolutions.io/
 License: Eclipse Public License - v2.0 Keywords: iot,embedded,edge,development
 environment,tools,containers Author: Janos Murai Author-email:
 janos.murai@axemsolutions.io Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: License :: Other/Proprietary
 License Classifier: Natural Language :: English Classifier: Programming
```

