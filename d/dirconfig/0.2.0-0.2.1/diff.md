# Comparing `tmp/dirconfig-0.2.0.tar.gz` & `tmp/dirconfig-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirconfig-0.2.0.tar", last modified: Wed Apr  3 02:29:41 2024, max compression
+gzip compressed data, was "dirconfig-0.2.1.tar", last modified: Thu Apr  4 21:05:09 2024, max compression
```

## Comparing `dirconfig-0.2.0.tar` & `dirconfig-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 02:29:41.359648 dirconfig-0.2.0/
--rw-rw-rw-   0        0        0     1087 2024-04-03 00:38:18.000000 dirconfig-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2952 2024-04-03 02:29:41.357409 dirconfig-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2374 2024-04-03 02:14:31.000000 dirconfig-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 02:29:41.333912 dirconfig-0.2.0/dirconfig/
--rw-rw-rw-   0        0        0        0 2024-04-03 01:36:27.000000 dirconfig-0.2.0/dirconfig/__init__.py
--rw-rw-rw-   0        0        0     4241 2024-04-03 02:26:39.000000 dirconfig-0.2.0/dirconfig/main.py
-drwxrwxrwx   0        0        0        0 2024-04-03 02:29:41.357409 dirconfig-0.2.0/dirconfig.egg-info/
--rw-rw-rw-   0        0        0     2952 2024-04-03 02:29:41.000000 dirconfig-0.2.0/dirconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 02:29:41.000000 dirconfig-0.2.0/dirconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 02:29:41.000000 dirconfig-0.2.0/dirconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-03 02:29:41.000000 dirconfig-0.2.0/dirconfig.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-04-03 02:29:41.000000 dirconfig-0.2.0/dirconfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 02:29:41.000000 dirconfig-0.2.0/dirconfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 02:29:41.359648 dirconfig-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-04-03 02:29:37.000000 dirconfig-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:05:09.316445 dirconfig-0.2.1/
+-rw-rw-rw-   0        0        0     1087 2024-04-03 00:38:18.000000 dirconfig-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3051 2024-04-04 21:05:09.315445 dirconfig-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2461 2024-04-04 17:49:18.000000 dirconfig-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 21:05:09.282443 dirconfig-0.2.1/dirconfig/
+-rw-rw-rw-   0        0        0        0 2024-04-03 01:36:27.000000 dirconfig-0.2.1/dirconfig/__init__.py
+-rw-rw-rw-   0        0        0     4928 2024-04-04 17:47:55.000000 dirconfig-0.2.1/dirconfig/main.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:05:09.314448 dirconfig-0.2.1/dirconfig.egg-info/
+-rw-rw-rw-   0        0        0     3051 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-04 21:05:09.000000 dirconfig-0.2.1/dirconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 21:05:08.000000 dirconfig-0.2.1/dirconfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 21:05:09.316445 dirconfig-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-04-04 17:38:47.000000 dirconfig-0.2.1/setup.py
```

### Comparing `dirconfig-0.2.0/LICENSE` & `dirconfig-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dirconfig-0.2.0/PKG-INFO` & `dirconfig-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dirconfig
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple directory configuration tool
 Home-page: https://github.com/judahpaul16/dirconfig
 Author: Judah Paul
 Author-email: me@judahpaul.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: watchdog==4.0.0
 
-# dirconfig :open_file_folder:
+# dirconfig ðŸ“‚
  Configure what files should be in what folders using an easy-to-read YAML config file.
 
 ## Features
 
 - **File Organization**: Automatically move files based on their extension from one directory to another.
 - **Notification System** (Future Feature): Get notified regarding specific events specified in the configuration file.
 - **Automated Backups** (Future Feature): Set up scheduled backups for important directories.
@@ -57,14 +57,20 @@
 
 ```sh
 dirconfig start
 ```
 
 This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
 
+To run **dirconfig** as a separate process, use the following command:
+
+```sh
+dirconfig start &
+```
+
 ### Stopping dirconfig
 
 To stop the **dirconfig** daemon, execute:
 
 ```sh
 dirconfig stop
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dirconfig-0.2.0/README.md` & `dirconfig-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# dirconfig :open_file_folder:
+# dirconfig 📂
  Configure what files should be in what folders using an easy-to-read YAML config file.
 
 ## Features
 
 - **File Organization**: Automatically move files based on their extension from one directory to another.
 - **Notification System** (Future Feature): Get notified regarding specific events specified in the configuration file.
 - **Automated Backups** (Future Feature): Set up scheduled backups for important directories.
@@ -41,14 +41,20 @@
 
 ```sh
 dirconfig start
 ```
 
 This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
 
+To run **dirconfig** as a separate process, use the following command:
+
+```sh
+dirconfig start &
+```
+
 ### Stopping dirconfig
 
 To stop the **dirconfig** daemon, execute:
 
 ```sh
 dirconfig stop
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dirconfig-0.2.0/dirconfig/main.py` & `dirconfig-0.2.1/dirconfig/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 from pathlib import Path
 import argparse
+import logging
 import signal
 import shutil
 import yaml
 import sys
 import os
 
 observer = None
@@ -47,17 +48,19 @@
                 if not os.path.exists(dest_path):
                     os.makedirs(dest_path)
                 
                 source_file_path = os.path.join(source_path, file)
                 dest_file_path = os.path.join(dest_path, file)
                 shutil.move(source_file_path, dest_file_path)
                 print(f"Moved: {file} -> {dest_file_path}")
+                logging.info(f"Moved: {file} -> {dest_file_path}")
 
 def signal_handler(signum, frame):
     print("\nReceived interrupt signal. Stopping dirconfig...")
+    logging.info("Received interrupt signal. Stopping dirconfig...")
     if observer is not None:
         observer.stop()
         observer.join()  # Ensure all threads are joined
         if os.path.exists(PID_FILE):
             os.remove(PID_FILE)
         sys.exit(0)
 
@@ -89,32 +92,39 @@
 def stop_daemon():
     try:
         with open(PID_FILE, 'r') as f:
             pid = int(f.read())
         os.kill(pid, signal.SIGTERM)
     except FileNotFoundError:
         print("Error: PID file not found. Is the daemon running?")
+        logging.error("Error: PID file not found. Is the daemon running?")
         sys.exit(1)
     except ProcessLookupError:
         print("Error: Process not found. It may have been stopped already.")
+        logging.error("Error: Process not found. It may have been stopped already.")
         sys.exit(1)
 
 def main():
     parser = argparse.ArgumentParser(description='dirconfig Daemon')
     parser.add_argument('action', choices=['start', 'stop'], help='Start or stop the daemon')
     # Default to 'config.yaml' in the current working directory if not specified
     parser.add_argument('--config', help='Path to the configuration file', default='config.yaml')
+    parser.add_argument('--log', help='Path to the log file', default='dirconfig.log')
     args = parser.parse_args()
 
     # Resolve the absolute path of the configuration file
     config_path = os.path.abspath(args.config)
 
+    # Initialize logging to log to a file specified by the --log argument.
+    logging.basicConfig(level=logging.INFO, filename=args.log, filemode='a', format='%(asctime)s - %(levelname)s - %(message)s')
+
     if args.action == 'start':
         if not os.path.exists(config_path):
             print(f"Configuration file not found: {config_path}")
+            logging.error(f"Configuration file not found: {config_path}")
             sys.exit(1)
         start_daemon(config_path)
     elif args.action == 'stop':
         stop_daemon()
 
 if __name__ == "__main__":
     main()
```

### Comparing `dirconfig-0.2.0/dirconfig.egg-info/PKG-INFO` & `dirconfig-0.2.1/dirconfig.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dirconfig
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple directory configuration tool
 Home-page: https://github.com/judahpaul16/dirconfig
 Author: Judah Paul
 Author-email: me@judahpaul.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: watchdog==4.0.0
 
-# dirconfig :open_file_folder:
+# dirconfig ðŸ“‚
  Configure what files should be in what folders using an easy-to-read YAML config file.
 
 ## Features
 
 - **File Organization**: Automatically move files based on their extension from one directory to another.
 - **Notification System** (Future Feature): Get notified regarding specific events specified in the configuration file.
 - **Automated Backups** (Future Feature): Set up scheduled backups for important directories.
@@ -57,14 +57,20 @@
 
 ```sh
 dirconfig start
 ```
 
 This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
 
+To run **dirconfig** as a separate process, use the following command:
+
+```sh
+dirconfig start &
+```
+
 ### Stopping dirconfig
 
 To stop the **dirconfig** daemon, execute:
 
 ```sh
 dirconfig stop
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dirconfig-0.2.0/setup.py` & `dirconfig-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dirconfig",
-    version="0.2.0",
+    version="0.2.1",
     author="Judah Paul",
     author_email="me@judahpaul.com",
     description="A simple directory configuration tool",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/judahpaul16/dirconfig",
     packages=find_packages(),
```

