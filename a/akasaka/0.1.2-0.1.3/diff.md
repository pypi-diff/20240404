# Comparing `tmp/akasaka-0.1.2.tar.gz` & `tmp/akasaka-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akasaka-0.1.2.tar", last modified: Tue Apr  2 01:46:34 2024, max compression
+gzip compressed data, was "akasaka-0.1.3.tar", last modified: Thu Apr  4 05:47:09 2024, max compression
```

## Comparing `akasaka-0.1.2.tar` & `akasaka-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:46:34.444293 akasaka-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-02 01:46:24.000000 akasaka-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-02 01:46:34.444293 akasaka-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-02 01:46:24.000000 akasaka-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:46:34.444293 akasaka-0.1.2/akasaka/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 01:46:24.000000 akasaka-0.1.2/akasaka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-02 01:46:24.000000 akasaka-0.1.2/akasaka/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-02 01:46:24.000000 akasaka-0.1.2/akasaka/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-02 01:46:24.000000 akasaka-0.1.2/akasaka/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:46:34.444293 akasaka-0.1.2/akasaka/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:46:24.000000 akasaka-0.1.2/akasaka/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 01:46:24.000000 akasaka-0.1.2/akasaka/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-02 01:46:24.000000 akasaka-0.1.2/akasaka/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:46:34.444293 akasaka-0.1.2/akasaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-02 01:46:34.000000 akasaka-0.1.2/akasaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-02 01:46:34.000000 akasaka-0.1.2/akasaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:46:34.000000 akasaka-0.1.2/akasaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 01:46:34.000000 akasaka-0.1.2/akasaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 01:46:34.000000 akasaka-0.1.2/akasaka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 01:46:34.000000 akasaka-0.1.2/akasaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:46:34.444293 akasaka-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-02 01:46:24.000000 akasaka-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:09.071745 akasaka-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 05:46:59.000000 akasaka-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-04 05:47:09.071745 akasaka-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-04 05:46:59.000000 akasaka-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:09.071745 akasaka-0.1.3/akasaka/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/torch_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/torch_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:09.071745 akasaka-0.1.3/akasaka/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-04 05:46:59.000000 akasaka-0.1.3/akasaka/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:47:09.071745 akasaka-0.1.3/akasaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 05:47:09.000000 akasaka-0.1.3/akasaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:47:09.071745 akasaka-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-04 05:46:59.000000 akasaka-0.1.3/setup.py
```

### Comparing `akasaka-0.1.2/LICENSE` & `akasaka-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.2/PKG-INFO` & `akasaka-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akasaka
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dynamic mutiprocess preprocessing task loader and dispatcher
 Home-page: https://github.com/JeffersonQin/akasaka
 Author: Haoyun Qin
 Author-email: qhy.cis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,32 +30,36 @@
 pip install akasaka
 ```
 
 ## Usage
 
 ```bash
 $ akasaka -H
-usage: akasaka [--num_process NUM_PROCESS] [--chunksize CHUNKSIZE] [-h] [-H] module_path
+usage: akasaka [--num_process NUM_PROCESS] [--chunksize CHUNKSIZE] [--devices DEVICES [DEVICES ...]] [-h] [-H] module_path
 
 Dynamically load a Python class from a module.
 
 positional arguments:
   module_path           The module path in the format "module.submodule.ClassName"
 
 optional arguments:
   --num_process NUM_PROCESS
-                        Number of processes to use (default: number of CPU cores)
+                        Number of processes to use, for normal task (default: number of CPU cores)
   --chunksize CHUNKSIZE
-                        Number of tasks to be sent to a worker process at a time (default: 1)
+                        Number of tasks to be sent to a worker process at a time, for normal task (default: 1)
+  --devices DEVICES [DEVICES ...]
+                        The devices to run the task on, for torch task (default: [])
   -h, --help            Show help message for task and exit
   -H, --hel-akasaka     Show Akasaka help message and exit
 ```
 
 Write a task class of the subclass of `AsakasaTask` and implement needed methods. Take a look at the examples in the [`examples` directory](./examples).
 
+For PyTorch CUDA tasks, you would need to use `AsakasaTorchTask` as the base class. The number of processes is determined by the number of CUDA devices provided.
+
 With akasaka installed, to run the examples, try following commands:
 
 ```bash
 cd examples
 # print.py
 akasaka print.PrintTaskTest --test test_string
 # directory_example/print.py
@@ -65,7 +69,11 @@
 ## Development
 
 To install from source, clone the repository and run
 
 ```bash
 pip install -e .
 ```
+
+## Known Issues
+
+For torch (CUDA) task, you might need to wait for unexpected long time after model loaded before the task can start. Reason to be figured out.
```

### Comparing `akasaka-0.1.2/README.md` & `akasaka-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -15,32 +15,36 @@
 pip install akasaka
 ```
 
 ## Usage
 
 ```bash
 $ akasaka -H
-usage: akasaka [--num_process NUM_PROCESS] [--chunksize CHUNKSIZE] [-h] [-H] module_path
+usage: akasaka [--num_process NUM_PROCESS] [--chunksize CHUNKSIZE] [--devices DEVICES [DEVICES ...]] [-h] [-H] module_path
 
 Dynamically load a Python class from a module.
 
 positional arguments:
   module_path           The module path in the format "module.submodule.ClassName"
 
 optional arguments:
   --num_process NUM_PROCESS
-                        Number of processes to use (default: number of CPU cores)
+                        Number of processes to use, for normal task (default: number of CPU cores)
   --chunksize CHUNKSIZE
-                        Number of tasks to be sent to a worker process at a time (default: 1)
+                        Number of tasks to be sent to a worker process at a time, for normal task (default: 1)
+  --devices DEVICES [DEVICES ...]
+                        The devices to run the task on, for torch task (default: [])
   -h, --help            Show help message for task and exit
   -H, --hel-akasaka     Show Akasaka help message and exit
 ```
 
 Write a task class of the subclass of `AsakasaTask` and implement needed methods. Take a look at the examples in the [`examples` directory](./examples).
 
+For PyTorch CUDA tasks, you would need to use `AsakasaTorchTask` as the base class. The number of processes is determined by the number of CUDA devices provided.
+
 With akasaka installed, to run the examples, try following commands:
 
 ```bash
 cd examples
 # print.py
 akasaka print.PrintTaskTest --test test_string
 # directory_example/print.py
@@ -50,7 +54,11 @@
 ## Development
 
 To install from source, clone the repository and run
 
 ```bash
 pip install -e .
 ```
+
+## Known Issues
+
+For torch (CUDA) task, you might need to wait for unexpected long time after model loaded before the task can start. Reason to be figured out.
```

### Comparing `akasaka-0.1.2/akasaka/loader.py` & `akasaka-0.1.3/akasaka/loader.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.2/akasaka/task.py` & `akasaka-0.1.3/akasaka/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     def __init__(self, args) -> None:
         """
         Initialize the task with command line arguments
         args can be passed to ArgumentParser.parse_args() to parse remaining command line arguments.
         """
         pass
 
-    def generate_tasks(self, **kwargs) -> list:
+    def generate_tasks(self) -> list:
         """Generate a list of tasks to be executed."""
         raise NotImplementedError("This method should be implemented in a subclass.")
 
     def is_executed(self, **kwargs) -> bool:
         """Check if the task has already been executed."""
         raise NotImplementedError("This method should be implemented in a subclass.")
```

### Comparing `akasaka-0.1.2/akasaka/utils/io.py` & `akasaka-0.1.3/akasaka/utils/io.py`

 * *Files identical despite different names*

### Comparing `akasaka-0.1.2/akasaka.egg-info/PKG-INFO` & `akasaka-0.1.3/akasaka.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akasaka
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dynamic mutiprocess preprocessing task loader and dispatcher
 Home-page: https://github.com/JeffersonQin/akasaka
 Author: Haoyun Qin
 Author-email: qhy.cis@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,32 +30,36 @@
 pip install akasaka
 ```
 
 ## Usage
 
 ```bash
 $ akasaka -H
-usage: akasaka [--num_process NUM_PROCESS] [--chunksize CHUNKSIZE] [-h] [-H] module_path
+usage: akasaka [--num_process NUM_PROCESS] [--chunksize CHUNKSIZE] [--devices DEVICES [DEVICES ...]] [-h] [-H] module_path
 
 Dynamically load a Python class from a module.
 
 positional arguments:
   module_path           The module path in the format "module.submodule.ClassName"
 
 optional arguments:
   --num_process NUM_PROCESS
-                        Number of processes to use (default: number of CPU cores)
+                        Number of processes to use, for normal task (default: number of CPU cores)
   --chunksize CHUNKSIZE
-                        Number of tasks to be sent to a worker process at a time (default: 1)
+                        Number of tasks to be sent to a worker process at a time, for normal task (default: 1)
+  --devices DEVICES [DEVICES ...]
+                        The devices to run the task on, for torch task (default: [])
   -h, --help            Show help message for task and exit
   -H, --hel-akasaka     Show Akasaka help message and exit
 ```
 
 Write a task class of the subclass of `AsakasaTask` and implement needed methods. Take a look at the examples in the [`examples` directory](./examples).
 
+For PyTorch CUDA tasks, you would need to use `AsakasaTorchTask` as the base class. The number of processes is determined by the number of CUDA devices provided.
+
 With akasaka installed, to run the examples, try following commands:
 
 ```bash
 cd examples
 # print.py
 akasaka print.PrintTaskTest --test test_string
 # directory_example/print.py
@@ -65,7 +69,11 @@
 ## Development
 
 To install from source, clone the repository and run
 
 ```bash
 pip install -e .
 ```
+
+## Known Issues
+
+For torch (CUDA) task, you might need to wait for unexpected long time after model loaded before the task can start. Reason to be figured out.
```

### Comparing `akasaka-0.1.2/setup.py` & `akasaka-0.1.3/setup.py`

 * *Files identical despite different names*

