# Comparing `tmp/ehdtd_daemon-0.1.1.tar.gz` & `tmp/ehdtd_daemon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd_daemon-0.1.1.tar", max compression
+gzip compressed data, was "ehdtd_daemon-0.1.2.tar", max compression
```

## Comparing `ehdtd_daemon-0.1.1.tar` & `ehdtd_daemon-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.1/LICENSE
--rw-r--r--   0        0        0     3214 2024-03-29 07:09:48.990259 ehdtd_daemon-0.1.1/README.md
--rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.1/ehdtd_daemon/__init__.py
--rw-r--r--   0        0        0     9627 2024-03-29 05:45:25.916363 ehdtd_daemon-0.1.1/ehdtd_daemon/aux_common_functions.py
--rw-r--r--   0        0        0     7213 2024-03-29 07:27:50.359576 ehdtd_daemon-0.1.1/ehdtd_daemon/bin/ehdtd_daemon.py
--rw-r--r--   0        0        0      730 2024-03-29 05:36:48.878667 ehdtd_daemon-0.1.1/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
--rw-r--r--   0        0        0      705 2024-03-29 07:34:31.857012 ehdtd_daemon-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3984 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3227 2024-03-31 05:25:31.149699 ehdtd_daemon-0.1.2/README.md
+-rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.2/ehdtd_daemon/__init__.py
+-rw-r--r--   0        0        0     9632 2024-04-04 01:41:43.749676 ehdtd_daemon-0.1.2/ehdtd_daemon/aux_common_functions.py
+-rw-r--r--   0        0        0     7213 2024-03-31 05:29:48.675926 ehdtd_daemon-0.1.2/ehdtd_daemon/bin/ehdtd_daemon.py
+-rw-r--r--   0        0        0      582 2024-04-04 01:26:17.025737 ehdtd_daemon-0.1.2/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
+-rw-r--r--   0        0        0      705 2024-04-04 10:26:43.760193 ehdtd_daemon-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.2/PKG-INFO
```

### Comparing `ehdtd_daemon-0.1.1/LICENSE` & `ehdtd_daemon-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.1/README.md` & `ehdtd_daemon-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ### Global Configuration
 
 The global configuration section defines settings that apply to the entire daemon operation.
 
 #### Parameters
 
     log_dir: The directory path for log files. Default is /var/log/ehdtd-daemon.
-    run_dir: The directory path for runtime files. Default is /run.
+    run_dir: The directory path for runtime files. Default is /run/ehdtd-daemon.
     debug: A boolean flag indicating whether to enable debug mode. Default is false.
 
 ### Database Configuration
 
 The database configuration section defines parameters for connecting to the database.
 
 #### Parameters
```

### Comparing `ehdtd_daemon-0.1.1/ehdtd_daemon/__init__.py` & `ehdtd_daemon-0.1.2/ehdtd_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.1/ehdtd_daemon/aux_common_functions.py` & `ehdtd_daemon-0.1.2/ehdtd_daemon/aux_common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,33 +292,35 @@
 def get_config_data(config_file):
     """
     get_config_data
     ===============
 
     """
     result = None
+    default_log_dir = '/var/log/ehdtd-daemon'
+    default_run_dir = '/run/ehdtd-daemon'
 
     config_data = None
     default_config_file = '/etc/ehdtd-daemon/ehdtd-daemon-config.yaml'
     if config_file is not None and isinstance(config_file, str) and os.path.exists(config_file):
         config_data = read_config_yaml(config_file)
     elif os.path.exists(default_config_file):
         config_data = read_config_yaml(default_config_file)
 
     if __check_config_structure(config_data):
         result = config_data
 
         if result['global']['log_dir'] is None or not isinstance(result['global']['log_dir'], str):
-            result['global']['log_dir'] = '/var/log/ehdtd-daemon'
+            result['global']['log_dir'] = default_log_dir
 
         if not os.path.exists(result['global']['log_dir']):
             os.makedirs(result['global']['log_dir'])
 
         if result['global']['run_dir'] is None or not isinstance(result['global']['run_dir'], str):
-            result['global']['run_dir'] = '/run'
+            result['global']['run_dir'] = default_run_dir
 
         if not os.path.exists(result['global']['run_dir']):
             os.makedirs(result['global']['run_dir'])
 
     return result
 
 def is_pid_running(pid):
@@ -328,16 +330,13 @@
 
     """
     result = False
 
     try:
         os.kill(pid, 0)
         result = True
-        # print('ENTRE: 0')
     except OSError:
         result = False
-        # print('ENTRE: 1')
     else:
         result = True
-        # print('ENTRE: 2')
 
     return result
```

### Comparing `ehdtd_daemon-0.1.1/ehdtd_daemon/bin/ehdtd_daemon.py` & `ehdtd_daemon-0.1.2/ehdtd_daemon/bin/ehdtd_daemon.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.1/pyproject.toml` & `ehdtd_daemon-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd-daemon"
-version = "0.1.1"
+version = "0.1.2"
 description = "Daemon script for ehdtd package"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rmalvarezkai/ehdtd_daemon"
 include = ["etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml"]
```

### Comparing `ehdtd_daemon-0.1.1/PKG-INFO` & `ehdtd_daemon-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd-daemon
-Version: 0.1.1
+Version: 0.1.2
 Summary: Daemon script for ehdtd package
 Home-page: https://github.com/rmalvarezkai/ehdtd_daemon
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 ### Global Configuration
 
 The global configuration section defines settings that apply to the entire daemon operation.
 
 #### Parameters
 
     log_dir: The directory path for log files. Default is /var/log/ehdtd-daemon.
-    run_dir: The directory path for runtime files. Default is /run.
+    run_dir: The directory path for runtime files. Default is /run/ehdtd-daemon.
     debug: A boolean flag indicating whether to enable debug mode. Default is false.
 
 ### Database Configuration
 
 The database configuration section defines parameters for connecting to the database.
 
 #### Parameters
```

