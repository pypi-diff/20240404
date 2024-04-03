# Comparing `tmp/runes-cli-0.4.2.tar.gz` & `tmp/runes-cli-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-cli-0.4.2.tar", last modified: Wed Apr  3 19:07:41 2024, max compression
+gzip compressed data, was "runes-cli-0.4.3.tar", last modified: Wed Apr  3 23:45:31 2024, max compression
```

## Comparing `runes-cli-0.4.2.tar` & `runes-cli-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 19:07:41.872396 runes-cli-0.4.2/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35149 2024-03-13 17:06:20.000000 runes-cli-0.4.2/LICENSE
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1341 2024-04-03 19:07:41.872263 runes-cli-0.4.2/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      960 2024-04-02 15:54:01.000000 runes-cli-0.4.2/README.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-03 19:07:41.872430 runes-cli-0.4.2/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)      914 2024-04-03 19:06:22.000000 runes-cli-0.4.2/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 19:07:41.867661 runes-cli-0.4.2/src/
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 19:07:41.871212 runes-cli-0.4.2/src/runes_cli/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 17:06:20.000000 runes-cli-0.4.2/src/runes_cli/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6763 2024-04-03 15:55:07.000000 runes-cli-0.4.2/src/runes_cli/api.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3157 2024-03-13 17:06:20.000000 runes-cli-0.4.2/src/runes_cli/builder.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    32668 2024-04-03 19:04:52.000000 runes-cli-0.4.2/src/runes_cli/cli.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      153 2024-04-02 22:18:02.000000 runes-cli-0.4.2/src/runes_cli/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     8858 2024-04-03 18:17:26.000000 runes-cli-0.4.2/src/runes_cli/containers.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1554 2024-03-31 06:30:26.000000 runes-cli-0.4.2/src/runes_cli/file_uploader.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     2062 2024-04-03 16:26:46.000000 runes-cli-0.4.2/src/runes_cli/models.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6187 2024-03-27 18:35:57.000000 runes-cli-0.4.2/src/runes_cli/persistence.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 19:07:41.872085 runes-cli-0.4.2/src/runes_cli.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1341 2024-04-03 19:07:41.000000 runes-cli-0.4.2/src/runes_cli.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      479 2024-04-03 19:07:41.000000 runes-cli-0.4.2/src/runes_cli.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-03 19:07:41.000000 runes-cli-0.4.2/src/runes_cli.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       45 2024-04-03 19:07:41.000000 runes-cli-0.4.2/src/runes_cli.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       50 2024-04-03 19:07:41.000000 runes-cli-0.4.2/src/runes_cli.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       10 2024-04-03 19:07:41.000000 runes-cli-0.4.2/src/runes_cli.egg-info/top_level.txt
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 23:45:31.867638 runes-cli-0.4.3/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35149 2024-03-13 17:06:20.000000 runes-cli-0.4.3/LICENSE
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1341 2024-04-03 23:45:31.867490 runes-cli-0.4.3/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      960 2024-04-02 15:54:01.000000 runes-cli-0.4.3/README.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-03 23:45:31.867679 runes-cli-0.4.3/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      914 2024-04-03 23:41:58.000000 runes-cli-0.4.3/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 23:45:31.862758 runes-cli-0.4.3/src/
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 23:45:31.866343 runes-cli-0.4.3/src/runes_cli/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 17:06:20.000000 runes-cli-0.4.3/src/runes_cli/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6763 2024-04-03 15:55:07.000000 runes-cli-0.4.3/src/runes_cli/api.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3157 2024-03-13 17:06:20.000000 runes-cli-0.4.3/src/runes_cli/builder.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    32817 2024-04-03 23:34:15.000000 runes-cli-0.4.3/src/runes_cli/cli.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      153 2024-04-02 22:18:02.000000 runes-cli-0.4.3/src/runes_cli/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     8827 2024-04-03 22:37:41.000000 runes-cli-0.4.3/src/runes_cli/containers.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1554 2024-03-31 06:30:26.000000 runes-cli-0.4.3/src/runes_cli/file_uploader.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     2062 2024-04-03 16:26:46.000000 runes-cli-0.4.3/src/runes_cli/models.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6187 2024-03-27 18:35:57.000000 runes-cli-0.4.3/src/runes_cli/persistence.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 23:45:31.867285 runes-cli-0.4.3/src/runes_cli.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1341 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      479 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       45 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       50 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       10 2024-04-03 23:45:31.000000 runes-cli-0.4.3/src/runes_cli.egg-info/top_level.txt
```

### Comparing `runes-cli-0.4.2/LICENSE` & `runes-cli-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.2/PKG-INFO` & `runes-cli-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-cli
-Version: 0.4.2
+Version: 0.4.3
 Summary: A python CLI used to manage the Signals & Sorcery platform
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `runes-cli-0.4.2/README.md` & `runes-cli-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.2/setup.py` & `runes-cli-0.4.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="runes-cli",
-    version="0.4.2",
+    version="0.4.3",
     author="Steve Hiehn",
     author_email="stevehiehn@gmail.com",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
         "click",
```

### Comparing `runes-cli-0.4.2/src/runes_cli/api.py` & `runes-cli-0.4.3/src/runes_cli/api.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.2/src/runes_cli/builder.py` & `runes-cli-0.4.3/src/runes_cli/builder.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.2/src/runes_cli/cli.py` & `runes-cli-0.4.3/src/runes_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         menu(ctx)
 
 
 def menu(ctx):
     option_title = default_title
     option_tokens = "tokens (set or update your connection token)"
     option_remotes = "runes (run or manage published runes)"
-    option_sources = "rune source code (build runes from published source code)"
+    option_sources = "rune source code (build runes from source code)"
     option_docker = "docker-images (run or publish a local docker-image as a rune)"
     option_account = "account (sign up/in/out)"
     option_config = "config (manage cli configs)"
 
     entry_options = [
         option_tokens,
         option_remotes,
@@ -223,14 +223,15 @@
     clear_screen()
 
     if selected_action == "add your token":
         token = click.prompt("Enter the new token", type=str)
         if not set_or_update_token(token):
             menu(ctx)
 
+        clear_screen()
         click.echo(f"Token has been updated to: {token}")
     elif selected_action == "view current token":
         token = read_token_from_db()
         if token:
             click.echo(f"CURRENT TOKEN: {token}")
         else:
             click.echo("No token found. A token will be generated.")
@@ -413,18 +414,16 @@
     # Attempt to bring the dialog to the front
     root.lift()
     root.attributes("-topmost", True)
     root.after_idle(root.attributes, "-topmost", False)
 
     # Opens the file selection dialog and returns the selected file path
     file_path = askopenfilename(
-        filetypes=[
-            ("Notebook files", "*.ipynb")
-        ]  # This line filters for .ipynb files only
-    )
+        filetypes=[("Notebook files", "*.ipynb")]
+    )  # This line filters for .ipynb files only
     return file_path
 
 
 def source_menu(ctx):
     clear_screen()
 
     title = default_title
@@ -456,14 +455,17 @@
             validate_notebook_source(source_url)
             image_name = get_valid_docker_image_name()
 
             # BUILD THE IMAGE
             try:
                 builder = DockerImageBuilder()
                 builder.build_docker_image(source_url, image_name)
+
+                clear_screen()
+                click.echo(f"Successfully build rune docker image: {image_name}")
             except Exception as e:
                 click.echo(f"Error building the docker image: {e}")
         except Exception as e:
             click.echo(f"Invalid source URL: {e}")
 
         menu(ctx)
     elif selected_action == option_publish:
@@ -557,15 +559,15 @@
             menu(ctx)
 
     else:
         menu(ctx)
 
 
 def remote_menu(ctx):
-    title = "List remotes"
+    title = "List Runes"
     option_menu = "menu"
 
     category_options = [
         option_remote_running,
         option_remote_available,
         option_remote_delete,
         option_menu,
@@ -582,15 +584,20 @@
             menu(ctx)
 
         list_remotes(ctx, selected_category)
 
 
 def docker_menu(ctx):
     title = "Docker image actions"
-    category_options = [option_docker_run_cpu, option_docker_publish, option_menu]
+    category_options = [
+        option_docker_run_cpu,
+        option_docker_run_gpu,
+        option_docker_publish,
+        option_menu,
+    ]
     selected_category = select(
         title,
         choices=category_options,
     ).ask()
 
     clear_screen()
 
@@ -726,23 +733,23 @@
                     if insert_remote_image_info(image_info, access_token):
                         clear_screen()
                         print("Image information successfully registered.")
                     else:
                         clear_screen()
                         print("Failed to register image information.")
 
-                    return
+                    menu(ctx)
                 else:
                     clear_screen()
                     print("Docker image publish failed.")
-                return
+
+                menu(ctx)
             else:
                 clear_screen()
                 print("DID NOT SUCCESSFULLY LOGIN TO DOCKER HUB")
-                return
 
     menu(ctx)
 
 
 def list_remotes(ctx, selected_category):
     remotes = []
```

### Comparing `runes-cli-0.4.2/src/runes_cli/containers.py` & `runes-cli-0.4.3/src/runes_cli/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,16 +143,16 @@
 
     # Run the container
     container = client.containers.run(
         image_name,
         command=command,
         name=name,
         detach=True,
-        # environment={"DN_CLI_TOKEN": token, "PYDEVD_DISABLE_FILE_VALIDATION": 1},
-        environment={"DN_CLI_TOKEN": token, "PYDEVD_DISABLE_FILE_VALIDATION": 1},
+        environment={"DN_CLIENT_TOKEN": token},
+        # environment={"DN_CLIENT_TOKEN": token, "PYDEVD_DISABLE_FILE_VALIDATION": 1},
         device_requests=device_requests,  # Add device requests here
     )
 
     # Get PID of the running container
     container.reload()  # Reload to update attributes
     pid = container.attrs["State"]["Pid"]
```

### Comparing `runes-cli-0.4.2/src/runes_cli/file_uploader.py` & `runes-cli-0.4.3/src/runes_cli/file_uploader.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.2/src/runes_cli/models.py` & `runes-cli-0.4.3/src/runes_cli/models.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.2/src/runes_cli/persistence.py` & `runes-cli-0.4.3/src/runes_cli/persistence.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.4.2/src/runes_cli.egg-info/PKG-INFO` & `runes-cli-0.4.3/src/runes_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-cli
-Version: 0.4.2
+Version: 0.4.3
 Summary: A python CLI used to manage the Signals & Sorcery platform
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

