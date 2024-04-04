# Comparing `tmp/metaflow-torchrun-0.0.5.tar.gz` & `tmp/metaflow-torchrun-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-torchrun-0.0.5.tar", last modified: Tue Oct 31 21:55:20 2023, max compression
+gzip compressed data, was "metaflow-torchrun-0.0.6.tar", last modified: Thu Apr  4 18:37:48 2024, max compression
```

## Comparing `metaflow-torchrun-0.0.5.tar` & `metaflow-torchrun-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2023-10-31 21:55:20.730025 metaflow-torchrun-0.0.5/
--rw-r--r--   0 eddie      (501) staff       (20)      175 2023-10-31 21:55:20.728938 metaflow-torchrun-0.0.5/PKG-INFO
--rw-r--r--   0 eddie      (501) staff       (20)     1528 2023-10-28 20:45:59.000000 metaflow-torchrun-0.0.5/README.md
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2023-10-31 21:55:20.726241 metaflow-torchrun-0.0.5/metaflow_extensions/
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2023-10-31 21:55:20.726338 metaflow-torchrun-0.0.5/metaflow_extensions/torchrun/
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2023-10-31 21:55:20.727615 metaflow-torchrun-0.0.5/metaflow_extensions/torchrun/plugins/
--rw-r--r--   0 eddie      (501) staff       (20)       87 2023-10-28 22:15:57.000000 metaflow-torchrun-0.0.5/metaflow_extensions/torchrun/plugins/mfextinit_torchrun.py
--rw-r--r--   0 eddie      (501) staff       (20)     7894 2023-10-31 21:44:33.000000 metaflow-torchrun-0.0.5/metaflow_extensions/torchrun/plugins/torchrun_decorator.py
-drwxr-xr-x   0 eddie      (501) staff       (20)        0 2023-10-31 21:55:20.728559 metaflow-torchrun-0.0.5/metaflow_torchrun.egg-info/
--rw-r--r--   0 eddie      (501) staff       (20)      175 2023-10-31 21:55:20.000000 metaflow-torchrun-0.0.5/metaflow_torchrun.egg-info/PKG-INFO
--rw-r--r--   0 eddie      (501) staff       (20)      300 2023-10-31 21:55:20.000000 metaflow-torchrun-0.0.5/metaflow_torchrun.egg-info/SOURCES.txt
--rw-r--r--   0 eddie      (501) staff       (20)        1 2023-10-31 21:55:20.000000 metaflow-torchrun-0.0.5/metaflow_torchrun.egg-info/dependency_links.txt
--rw-r--r--   0 eddie      (501) staff       (20)       20 2023-10-31 21:55:20.000000 metaflow-torchrun-0.0.5/metaflow_torchrun.egg-info/top_level.txt
--rw-r--r--   0 eddie      (501) staff       (20)       38 2023-10-31 21:55:20.730114 metaflow-torchrun-0.0.5/setup.cfg
--rw-r--r--   0 eddie      (501) staff       (20)      423 2023-10-31 21:55:01.000000 metaflow-torchrun-0.0.5/setup.py
+drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.639755 metaflow-torchrun-0.0.6/
+-rw-r--r--   0 eddie      (501) staff       (20)      175 2024-04-04 18:37:48.639497 metaflow-torchrun-0.0.6/PKG-INFO
+-rw-r--r--   0 eddie      (501) staff       (20)     2908 2023-11-02 22:18:03.000000 metaflow-torchrun-0.0.6/README.md
+drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.636291 metaflow-torchrun-0.0.6/metaflow_extensions/
+drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.636345 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/
+drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.637146 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/
+-rw-r--r--   0 eddie      (501) staff       (20)      147 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/mfextinit_torchrun.py
+drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.638458 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/
+-rw-r--r--   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/__init__.py
+-rw-r--r--   0 eddie      (501) staff       (20)       74 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/constants.py
+-rw-r--r--   0 eddie      (501) staff       (20)     7927 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py
+-rw-r--r--   0 eddie      (501) staff       (20)     1586 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py
+-rw-r--r--   0 eddie      (501) staff       (20)     8923 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py
+-rw-r--r--   0 eddie      (501) staff       (20)     3752 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py
+-rw-r--r--   0 eddie      (501) staff       (20)     1022 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py
+-rw-r--r--   0 eddie      (501) staff       (20)     2835 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py
+drwxr-xr-x   0 eddie      (501) staff       (20)        0 2024-04-04 18:37:48.639191 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/
+-rw-r--r--   0 eddie      (501) staff       (20)      175 2024-04-04 18:37:48.000000 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/PKG-INFO
+-rw-r--r--   0 eddie      (501) staff       (20)      781 2024-04-04 18:37:48.000000 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/SOURCES.txt
+-rw-r--r--   0 eddie      (501) staff       (20)        1 2024-04-04 18:37:48.000000 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/dependency_links.txt
+-rw-r--r--   0 eddie      (501) staff       (20)       20 2024-04-04 18:37:48.000000 metaflow-torchrun-0.0.6/metaflow_torchrun.egg-info/top_level.txt
+-rw-r--r--   0 eddie      (501) staff       (20)       38 2024-04-04 18:37:48.639813 metaflow-torchrun-0.0.6/setup.cfg
+-rw-r--r--   0 eddie      (501) staff       (20)      423 2024-04-04 18:37:40.000000 metaflow-torchrun-0.0.6/setup.py
```

### Comparing `metaflow-torchrun-0.0.5/README.md` & `metaflow-torchrun-0.0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,54 @@
 # Metaflow torchrun decorator
-This repository implements a plugin to run parallel Metaflow tasks as nodes in a torchrun job which can be submitted to AWS Batch or a Kubernetes cluster.
 
+### Introduction
+This repository implements a plugin to run parallel Metaflow tasks as nodes in a [torchrun](https://pytorch.org/docs/stable/elastic/run.html) job which can be submitted to AWS Batch or a Kubernetes cluster.
+
+### Features
+- <b>Automatic torchrun integration:</b> This extension provides a simple and intuitive way to incorporate PyTorch distributed programs in your Metaflow workflows using the `@torchrun` decorator
+- <b>No changes to model code:</b> The `@torchrun` decorator exposes a new method on the Metaflow current object, so you can run your existing torch distributed programs inside Metaflow tasks with no changes in the research code.
+- <b>Run one command:</b> You don't need to log into many nodes and run commands on each. Instead, the `@torchrun` decorator will select arguments for the torchrun command based on the requests in Metaflow compute decorators like number of GPUs. Network addresses are automatically discoverable. 
+- <b>No user-facing subprocess calls:</b> At the end of the day, `@torchrun` is calling a subprocess inside a Metaflow task. Although many Metaflow users do this, it can make code difficult to read for beginners. One major goal of this plugin is to motivate hardening and automating a pattern for submitting subprocess calls inside Metaflow tasks.
+
+### Installation
 You can install it with:
 ```
 pip install metaflow-torchrun
 ```
 
+### Getting Started
 And then you can import it and use in parallel steps:
 ```
 from metaflow import FlowSpec, step, torchrun
 
 ...
-class MinGPT(FlowSpec):
+class MyGPT(FlowSpec):
 
     @step
     def start(self):
         self.next(self.torch_multinode, num_parallel=N_NODES)
 
-    @kubernetes(image="<YOUR-REGISTRY>/min-gpt:2", cpu=N_CPU, gpu=N_GPU, memory=MEMORY, disk=DISK)
-    @torchrun(
-        torchrun_args={"nproc_per_node": N_GPU},
-        entrypoint="main.py" # No changes made to original demo script.
-    )
+    @kubernetes(cpu=N_CPU, gpu=N_GPU, memory=MEMORY)
+    @torchrun
     @step
     def torch_multinode(self):
         ...
+        current.torch.run(
+            entrypoint="main.py", # No changes made to original script.
+            entrypoint_args = {"main-arg-1": "123", "main-arg-2": "777"},
+            nproc_per_node=1,     # edge case of a torchrun arg user-facing.
+        )
+        ...
     ...
 ```
 
-## Examples
+### Examples
 
 | Directory | torch script description |
 | :--- | ---: |
-| [Hello](examples/hello/flow.py) | Each process prints their rank and the world size. |  
-| [Tensor pass](examples/tensor-pass/flow.py) | Main process passes a tensor to the workers. |  
-| [Torch DDP](examples/torch-ddp/flow.py) | A flow that uses a [script from the torchrun tutorials](https://pytorch.org/tutorials/intermediate/ddp_series_multinode.html) on multi-node DDP. |  
-| [MinGPT](examples/min-gpt/flow.py) | A flow that runs a [torchrun GPT demo](https://pytorch.org/tutorials/intermediate/ddp_series_minGPT.html) that simplifies [Karpathy's minGPT](https://github.com/karpathy/minGPT) in a set of parallel Metaflow tasks each contributing their `@resources`. |
+| [Hello](examples/hello/README.md) | Each process prints their rank and the world size. |  
+| [Tensor pass](examples/tensor-pass/README.md) | Main process passes a tensor to the workers. |  
+| [Torch DDP](examples/torch-ddp/README.md) | A flow that uses a [script from the torchrun tutorials](https://pytorch.org/tutorials/intermediate/ddp_series_multinode.html) on multi-node DDP. |  
+| [MinGPT](examples/min-gpt/README.md) | A flow that runs a [torchrun GPT demo](https://pytorch.org/tutorials/intermediate/ddp_series_minGPT.html) that simplifies [Karpathy's minGPT](https://github.com/karpathy/minGPT) in a set of parallel Metaflow tasks each contributing their `@resources`. |
+
+### License 
+`metaflow-torchrun` is distributed under the <u>Apache License</u>.
```

