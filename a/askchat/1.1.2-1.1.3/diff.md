# Comparing `tmp/askchat-1.1.2.tar.gz` & `tmp/askchat-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askchat-1.1.2.tar", last modified: Sun Mar 24 09:10:44 2024, max compression
+gzip compressed data, was "askchat-1.1.3.tar", last modified: Thu Apr  4 13:38:48 2024, max compression
```

## Comparing `askchat-1.1.2.tar` & `askchat-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 09:10:44.254174 askchat-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-24 09:10:32.000000 askchat-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-24 09:10:32.000000 askchat-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-24 09:10:44.254174 askchat-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-03-24 09:10:32.000000 askchat-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 09:10:44.254174 askchat-1.1.2/askchat/
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-24 09:10:32.000000 askchat-1.1.2/askchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-24 09:10:32.000000 askchat-1.1.2/askchat/ask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-03-24 09:10:32.000000 askchat-1.1.2/askchat/askenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-03-24 09:10:32.000000 askchat-1.1.2/askchat/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 09:10:44.254174 askchat-1.1.2/askchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-24 09:10:43.000000 askchat-1.1.2/askchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-24 09:10:44.000000 askchat-1.1.2/askchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 09:10:43.000000 askchat-1.1.2/askchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-24 09:10:43.000000 askchat-1.1.2/askchat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 09:10:43.000000 askchat-1.1.2/askchat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-24 09:10:43.000000 askchat-1.1.2/askchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-24 09:10:43.000000 askchat-1.1.2/askchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-24 09:10:44.254174 askchat-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-24 09:10:32.000000 askchat-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 09:10:44.254174 askchat-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-24 09:10:32.000000 askchat-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-24 09:10:32.000000 askchat-1.1.2/tests/test_askchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-24 09:10:32.000000 askchat-1.1.2/tests/test_askenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:38:48.648183 askchat-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 13:38:40.000000 askchat-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 13:38:40.000000 askchat-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-04 13:38:48.648183 askchat-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-04 13:38:40.000000 askchat-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:38:48.648183 askchat-1.1.3/askchat/
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-04 13:38:40.000000 askchat-1.1.3/askchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 13:38:40.000000 askchat-1.1.3/askchat/ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-04 13:38:40.000000 askchat-1.1.3/askchat/askenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-04 13:38:40.000000 askchat-1.1.3/askchat/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:38:48.648183 askchat-1.1.3/askchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-04 13:38:48.648183 askchat-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-04 13:38:40.000000 askchat-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:38:48.648183 askchat-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 13:38:40.000000 askchat-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-04 13:38:40.000000 askchat-1.1.3/tests/test_askchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-04 13:38:40.000000 askchat-1.1.3/tests/test_askenv.py
```

### Comparing `askchat-1.1.2/LICENSE` & `askchat-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `askchat-1.1.2/PKG-INFO` & `askchat-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: askchat
-Version: 1.1.2
+Version: 1.1.3
 Summary: Interact with ChatGPT in terminal via chattool
 Home-page: https://github.com/cubenlp/askchat
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: UNKNOWN
 Keywords: askchat
```

### Comparing `askchat-1.1.2/README.md` & `askchat-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `askchat-1.1.2/askchat/__init__.py` & `askchat-1.1.3/askchat/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 """Top-level package for askchat."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 
 import asyncio
 from pathlib import Path
 import click
+from dotenv import set_key
+import os
 
 # Main environment file
 CONFIG_PATH = Path.home() / ".askchat"
 CONFIG_FILE = CONFIG_PATH / ".env"
 MAIN_ENV_PATH = Path.home() / '.askchat' / '.env'
 ENV_PATH = Path.home() / '.askchat' / 'envs'
 
+raw_env_text = f""""# Description: Env file for askchat.
+# Current version: {__version__}
+
+# The base url of the API (with suffix /v1)
+# This will override OPENAI_API_BASE_URL if both are set.
+OPENAI_API_BASE=''
+
+# The base url of the API (without suffix /v1)
+OPENAI_API_BASE_URL=''
+
+# Your API key
+OPENAI_API_KEY=''
+
+# The default model name
+# You can use `askchat --all-valid-models` to see supported models
+OPENAI_API_MODEL=''
+"""
+
 # Autocompletion
 # environment name completion
 class EnvNameCompletionType(click.ParamType):
     name = "envname"
     def shell_complete(self, ctx, param, incomplete):
         return [
             click.shell_completion.CompletionItem(path.stem) for path in ENV_PATH.glob(f"{incomplete}*.env")
@@ -38,24 +58,40 @@
         print(char, end='', flush=True)
         msg += char
         await asyncio.sleep(0.01)
     if not msg.endswith('\n'):
         print() # add a newline if the message doesn't end with one
     return msg
 
-def write_config(config_file, api_key, model, base_url, api_base):
-    """Write the environment variables to a config file."""
-    def write_var(f, var, value, desc):
-        value = value if value else ""
-        f.write(f"\n\n# {desc}\n")
-        f.write(f'{var}="{value}"')
+def set_keys(config_file, keys):
+    """Set multiple keys in the config file."""
+    for key, value in keys.items():
+        if value:
+            set_key(config_file, key, value)
+
+def raw_config(config_file:str):
+    """Empty config file."""
+    if not CONFIG_PATH.exists():
+        CONFIG_PATH.mkdir(parents=True)
     with open(config_file, "w") as f:
-        f.write("#Description: Env file for askchat.\n" +\
-                "#Current version: " + __version__)
-        # write the environment table
-        write_var(f, "OPENAI_API_BASE", api_base, "The base url of the API (with suffix /v1)" +\
-                    "\n# This will override OPENAI_API_BASE_URL if both are set.")
-        write_var(f, "OPENAI_API_BASE_URL", base_url, "The base url of the API (without suffix /v1)")
-
-        write_var(f, "OPENAI_API_KEY", api_key, "Your API key")
-        write_var(f, "OPENAI_API_MODEL", model, "The model name\n" +\
-                    "# You can use `askchat --all-valid-models` to see supported models")
+        f.write(raw_env_text)
+
+def init_config(config_file:str):
+    """Initialize the config file with the current environment variables."""
+    raw_config(config_file)
+    set_keys(config_file, {
+        "OPENAI_API_KEY": os.getenv("OPENAI_API_KEY"),
+        "OPENAI_API_MODEL": os.getenv("OPENAI_API_MODEL"),
+        "OPENAI_API_BASE_URL": os.getenv("OPENAI_API_BASE_URL"),
+        "OPENAI_API_BASE": os.getenv("OPENAI_API_BASE"),
+    })
+
+def write_config(config_file, api_key, model, base_url, api_base, overwrite=False):
+    """Write the environment variables to a config file."""
+    if overwrite or not config_file.exists():
+        raw_config(config_file)
+    set_keys(config_file, {
+        "OPENAI_API_KEY": api_key,
+        "OPENAI_API_MODEL": model,
+        "OPENAI_API_BASE_URL": base_url,
+        "OPENAI_API_BASE": api_base,
+    })
```

### Comparing `askchat-1.1.2/askchat/askenv.py` & `askchat-1.1.3/askchat/askenv.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """Create a new environment configuration."""
     config_path = ENV_PATH / f'{name}.env'
     if config_path.exists():
         click.echo(f"Warning: Overwriting existing environment '{name}'.")
         click.confirm("Do you want to continue?", abort=True)
     else:
         click.echo(f"Environment '{name}' created.")
-    write_config(config_path, api_key, model, base_url, api_base)
+    write_config(config_path, api_key, model, base_url, api_base, overwrite=True)
 
 @cli.command()
 @click.argument('name', required=False, type=EnvNameCompletionType())
 @click.option('--default', is_flag=True, help='Delete the default environment configuration')
 def delete(name, default):
     """Delete an environment configuration."""
     if default:
@@ -116,21 +116,15 @@
 def config(name, api_key, base_url, api_base, model):
     """Update default .env values."""
     if not any([api_key, base_url, api_base, model]):
         click.echo("No updates made. Provide at least one option to update.")
         return
     config_path = ENV_PATH / f'{name}.env' if name else MAIN_ENV_PATH
     if not config_path.exists():
-        click.echo(f"Environment '{config_path}' not found.")
+        click.echo(f"Environment '{config_path}' not found." +\
+                   "Use `askenv new` to create a new environment." )
         return
-    if api_key:
-        set_key(config_path, "OPENAI_API_KEY", api_key)
-    if base_url:
-        set_key(config_path, "OPENAI_API_BASE_URL", base_url)
-    if api_base:
-        set_key(config_path, "OPENAI_API_BASE", api_base)
-    if model:
-        set_key(config_path, "OPENAI_API_MODEL", model)
+    write_config(config_path, api_key, model, base_url, api_base)
     click.echo(f"Environment {config_path} updated.")
 
 if __name__ == '__main__':
     cli()
```

### Comparing `askchat-1.1.2/askchat/cli.py` & `askchat-1.1.3/askchat/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from pprint import pprint
 from dotenv import load_dotenv
 import asyncio, os, shutil
 from chattool import Chat, debug_log
 from pathlib import Path
 from askchat import (
-      show_resp, write_config
+      show_resp, write_config, init_config
     , ENV_PATH, MAIN_ENV_PATH
     , CONFIG_PATH, CONFIG_FILE
     , EnvNameCompletionType, ChatFileCompletionType
 )
 
 # Version and Config Path
 VERSION = askchat.__version__
@@ -33,20 +33,18 @@
         load_dotenv(CONFIG_FILE, override=True)
     chattool.load_envs()
 
 # callback functions for general options
 def generate_config_callback(ctx, param, value):
     """Generate a configuration file by environment table."""
     if not value: return
-    api_key, model = os.getenv("OPENAI_API_KEY"), os.getenv("OPENAI_API_MODEL")
-    base_url, api_base = os.getenv("OPENAI_API_BASE_URL"), os.getenv("OPENAI_API_BASE")
     # save the config file
     if os.path.exists(CONFIG_FILE):
         click.confirm(f"Overwrite the existing configuration file {CONFIG_FILE}?", abort=True)
-    write_config(CONFIG_FILE, api_key, model, base_url, api_base)
+    init_config(CONFIG_FILE)
     print("Created config file at", CONFIG_FILE)
     ctx.exit()
 
 def debug_log_callback(ctx, param, value):
     if not value: return
     setup()
     debug_log()
```

### Comparing `askchat-1.1.2/askchat.egg-info/PKG-INFO` & `askchat-1.1.3/askchat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: askchat
-Version: 1.1.2
+Version: 1.1.3
 Summary: Interact with ChatGPT in terminal via chattool
 Home-page: https://github.com/cubenlp/askchat
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: UNKNOWN
 Keywords: askchat
```

### Comparing `askchat-1.1.2/setup.py` & `askchat-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-VERSION = '1.1.2'
+VERSION = '1.1.3'
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-requirements = ['chattool>=3.1.3', "python-dotenv>=0.17.0", 'Click>=8.0']
+requirements = ['chattool>=3.1.4', "python-dotenv>=0.17.0", 'Click>=8.0']
 
 test_requirements = ['pytest>=3']
 
 setup(
     author="Rex Wang",
     author_email='1073853456@qq.com',
     python_requires='>=3.6',
```

### Comparing `askchat-1.1.2/tests/test_askchat.py` & `askchat-1.1.3/tests/test_askchat.py`

 * *Files identical despite different names*

### Comparing `askchat-1.1.2/tests/test_askenv.py` & `askchat-1.1.3/tests/test_askenv.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     
     # Attempt to overwrite the environment, confirming the action
     result = runner.invoke(cli, ["new", env_name, "--api-key", "456"], input="y\n")
     assert "Warning: Overwriting existing environment" in result.output
     assert "Do you want to continue?" in result.output
     # Verify the environment was overwritten by checking if the new API key is in the file
     with open(config_path) as f:
-        assert 'OPENAI_API_KEY="456"' in f.read()
+        assert "OPENAI_API_KEY='456'" in f.read()
 
 def test_list_initially_empty(runner, setup_env):
     """Ensure no environments are listed when none have been created."""
     env_name, config_path = setup_env
     runner.invoke(cli, ["new", env_name, "--api-key", "123"], input="y\n")
     result = runner.invoke(cli, ["list"])
     assert env_name in result.output
```

