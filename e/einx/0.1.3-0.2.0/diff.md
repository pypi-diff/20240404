# Comparing `tmp/einx-0.1.3.tar.gz` & `tmp/einx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einx-0.1.3.tar", last modified: Sun Jan 28 16:39:25 2024, max compression
+gzip compressed data, was "einx-0.2.0.tar", last modified: Thu Apr  4 18:43:18 2024, max compression
```

## Comparing `einx-0.1.3.tar` & `einx-0.2.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-01-28 16:39:25.035385 einx-0.1.3/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     1093 2024-01-17 12:19:00.000000 einx-0.1.3/LICENSE
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6563 2024-01-28 16:39:25.035385 einx-0.1.3/PKG-INFO
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6010 2024-01-27 19:30:54.000000 einx-0.1.3/README.md
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-01-28 16:39:25.031386 einx-0.1.3/einx/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      174 2024-01-19 10:38:25.000000 einx-0.1.3/einx/__init__.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-01-28 16:39:25.031386 einx-0.1.3/einx/backend/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2399 2024-01-21 21:14:28.000000 einx-0.1.3/einx/backend/__init__.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2671 2024-01-21 21:13:06.000000 einx-0.1.3/einx/backend/_jax.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4110 2024-01-23 12:56:11.000000 einx-0.1.3/einx/backend/_numpy.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6639 2024-01-23 13:25:56.000000 einx-0.1.3/einx/backend/_tensorflow.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6164 2024-01-27 18:32:40.000000 einx-0.1.3/einx/backend/_torch.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      780 2024-01-27 17:39:41.000000 einx-0.1.3/einx/backend/base.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    28036 2024-01-23 14:08:15.000000 einx-0.1.3/einx/backend/tracer.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-01-28 16:39:25.035385 einx-0.1.3/einx/expr/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       59 2023-12-14 11:24:25.000000 einx-0.1.3/einx/expr/__init__.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     8595 2023-12-18 08:41:13.000000 einx-0.1.3/einx/expr/solver.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    19348 2024-01-23 11:04:02.000000 einx-0.1.3/einx/expr/stage1.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    35261 2023-12-17 22:40:11.000000 einx-0.1.3/einx/expr/stage2.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    16306 2024-01-14 13:46:39.000000 einx-0.1.3/einx/expr/stage3.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4870 2023-12-17 14:46:32.000000 einx-0.1.3/einx/expr/util.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     3208 2024-01-23 13:11:49.000000 einx-0.1.3/einx/lru_cache.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-01-28 16:39:25.035385 einx-0.1.3/einx/nn/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       55 2024-01-27 18:52:52.000000 einx-0.1.3/einx/nn/__init__.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     7088 2024-01-19 15:30:09.000000 einx-0.1.3/einx/nn/equinox.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     9281 2024-01-19 15:24:22.000000 einx-0.1.3/einx/nn/flax.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      468 2024-01-27 18:55:06.000000 einx-0.1.3/einx/nn/framework.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     7475 2024-01-19 15:19:50.000000 einx-0.1.3/einx/nn/haiku.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     8426 2024-01-27 19:06:56.000000 einx-0.1.3/einx/nn/keras.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4560 2024-01-19 15:07:38.000000 einx-0.1.3/einx/nn/nn.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     9204 2024-01-27 19:06:59.000000 einx-0.1.3/einx/nn/torch.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-01-28 16:39:25.035385 einx-0.1.3/einx/op/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      206 2023-12-15 10:26:29.000000 einx-0.1.3/einx/op/__init__.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6308 2024-01-20 12:35:49.000000 einx-0.1.3/einx/op/arange.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10583 2024-01-20 12:35:54.000000 einx-0.1.3/einx/op/dot.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    15831 2024-01-23 14:24:52.000000 einx-0.1.3/einx/op/elementwise.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    17199 2024-01-27 19:14:53.000000 einx-0.1.3/einx/op/index.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     5837 2024-01-20 12:36:20.000000 einx-0.1.3/einx/op/rearrange.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    11513 2024-01-20 12:36:27.000000 einx-0.1.3/einx/op/reduce.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4632 2024-01-20 12:35:26.000000 einx-0.1.3/einx/op/solve.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     9152 2024-01-23 14:24:07.000000 einx-0.1.3/einx/op/util.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    14810 2024-01-23 13:31:25.000000 einx-0.1.3/einx/op/vmap.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    12361 2024-01-23 12:19:03.000000 einx-0.1.3/einx/op/vmap_with_axis.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2426 2024-01-27 18:53:14.000000 einx-0.1.3/einx/param.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2120 2024-01-16 16:32:14.000000 einx-0.1.3/einx/tree_util.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       98 2024-01-20 12:36:57.000000 einx-0.1.3/einx/types.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-01-28 16:39:25.031386 einx-0.1.3/einx.egg-info/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6563 2024-01-28 16:39:24.000000 einx-0.1.3/einx.egg-info/PKG-INFO
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      972 2024-01-28 16:39:24.000000 einx-0.1.3/einx.egg-info/SOURCES.txt
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)        1 2024-01-28 16:39:24.000000 einx-0.1.3/einx.egg-info/dependency_links.txt
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       59 2024-01-28 16:39:24.000000 einx-0.1.3/einx.egg-info/requires.txt
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)        5 2024-01-28 16:39:24.000000 einx-0.1.3/einx.egg-info/top_level.txt
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       79 2024-01-28 16:39:25.035385 einx-0.1.3/setup.cfg
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      993 2024-01-28 16:12:55.000000 einx-0.1.3/setup.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-01-28 16:39:25.035385 einx-0.1.3/test/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     1755 2023-12-14 11:24:25.000000 einx-0.1.3/test/test_compare_einops.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     9711 2024-01-27 18:40:23.000000 einx-0.1.3/test/test_nn.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    24171 2024-01-23 15:56:08.000000 einx-0.1.3/test/test_shapes.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4880 2024-01-18 17:22:22.000000 einx-0.1.3/test/test_values.py
+drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.670449 einx-0.2.0/
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     1093 2024-01-17 12:19:00.000000 einx-0.2.0/LICENSE
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6628 2024-04-04 18:43:18.670449 einx-0.2.0/PKG-INFO
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6075 2024-04-03 18:50:31.000000 einx-0.2.0/README.md
+drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx/
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      203 2024-03-08 12:29:27.000000 einx-0.2.0/einx/__init__.py
+drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx/backend/
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2722 2024-03-18 09:17:36.000000 einx-0.2.0/einx/backend/__init__.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     3256 2024-04-04 08:32:06.000000 einx-0.2.0/einx/backend/_dask.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2649 2024-04-04 08:32:08.000000 einx-0.2.0/einx/backend/_jax.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4731 2024-04-04 08:32:13.000000 einx-0.2.0/einx/backend/_mlx.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4289 2024-04-04 08:32:16.000000 einx-0.2.0/einx/backend/_numpy.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     7190 2024-04-04 08:32:20.000000 einx-0.2.0/einx/backend/_tensorflow.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     8826 2024-04-04 12:37:53.000000 einx-0.2.0/einx/backend/_torch.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      847 2024-04-04 08:33:01.000000 einx-0.2.0/einx/backend/base.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    30761 2024-04-04 07:52:02.000000 einx-0.2.0/einx/backend/tracer.py
+drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx/expr/
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       59 2023-12-14 11:24:25.000000 einx-0.2.0/einx/expr/__init__.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     9078 2024-03-08 18:36:53.000000 einx-0.2.0/einx/expr/solver.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    27957 2024-03-29 10:45:00.000000 einx-0.2.0/einx/expr/stage1.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    40301 2024-03-29 10:50:18.000000 einx-0.2.0/einx/expr/stage2.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    17055 2024-03-09 11:58:53.000000 einx-0.2.0/einx/expr/stage3.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     5152 2024-03-08 22:56:33.000000 einx-0.2.0/einx/expr/util.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     5745 2024-04-03 21:49:58.000000 einx-0.2.0/einx/lru_cache.py
+drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx/nn/
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       56 2024-03-08 15:08:02.000000 einx-0.2.0/einx/nn/__init__.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     7609 2024-03-29 10:45:00.000000 einx-0.2.0/einx/nn/equinox.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10042 2024-03-29 10:45:00.000000 einx-0.2.0/einx/nn/flax.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      476 2024-03-08 15:13:23.000000 einx-0.2.0/einx/nn/framework.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     8107 2024-04-04 12:39:18.000000 einx-0.2.0/einx/nn/haiku.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     8968 2024-03-29 10:45:00.000000 einx-0.2.0/einx/nn/keras.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4880 2024-03-08 17:33:26.000000 einx-0.2.0/einx/nn/nn.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     9182 2024-03-29 10:10:27.000000 einx-0.2.0/einx/nn/torch.py
+drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.670449 einx-0.2.0/einx/op/
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      207 2024-03-08 15:08:02.000000 einx-0.2.0/einx/op/__init__.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6532 2024-03-09 11:51:38.000000 einx-0.2.0/einx/op/arange.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10953 2024-03-29 10:45:00.000000 einx-0.2.0/einx/op/dot.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    16678 2024-04-04 07:48:15.000000 einx-0.2.0/einx/op/elementwise.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    20042 2024-03-29 10:10:27.000000 einx-0.2.0/einx/op/index.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6007 2024-04-03 21:50:06.000000 einx-0.2.0/einx/op/rearrange.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    12644 2024-03-09 12:24:47.000000 einx-0.2.0/einx/op/reduce.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4943 2024-03-09 12:29:03.000000 einx-0.2.0/einx/op/solve.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10039 2024-04-03 21:49:55.000000 einx-0.2.0/einx/op/util.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    14980 2024-03-09 20:06:11.000000 einx-0.2.0/einx/op/vmap.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    12470 2024-03-29 11:52:50.000000 einx-0.2.0/einx/op/vmap_with_axis.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2512 2024-04-04 12:43:22.000000 einx-0.2.0/einx/param.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     1795 2024-03-08 17:33:26.000000 einx-0.2.0/einx/traceback_util.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2384 2024-03-08 17:33:26.000000 einx-0.2.0/einx/tree_util.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       98 2024-01-20 12:36:57.000000 einx-0.2.0/einx/types.py
+drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx.egg-info/
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6628 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/PKG-INFO
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     1038 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)        1 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       59 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/requires.txt
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)        5 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/top_level.txt
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       79 2024-04-04 18:43:18.670449 einx-0.2.0/setup.cfg
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      993 2024-04-04 18:39:13.000000 einx-0.2.0/setup.py
+drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.670449 einx-0.2.0/test/
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2102 2024-03-09 20:06:07.000000 einx-0.2.0/test/test_compare_einops.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10724 2024-03-09 18:47:00.000000 einx-0.2.0/test/test_nn.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    29230 2024-04-04 12:55:32.000000 einx-0.2.0/test/test_shapes.py
+-rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     5526 2024-03-18 09:21:31.000000 einx-0.2.0/test/test_values.py
```

### Comparing `einx-0.1.3/LICENSE` & `einx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `einx-0.1.3/PKG-INFO` & `einx-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einx
-Version: 0.1.3
+Version: 0.2.0
 Summary: Tensor Operations Expressed in Einstein-Inspired Notation
 Home-page: https://github.com/fferflo/einx
 Author: Florian Fervers
 Author-email: florian.fervers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
 [![PyPI version](https://badge.fury.io/py/einx.svg)](https://badge.fury.io/py/einx)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 einx is a Python library that allows formulating many tensor operations as concise expressions using Einstein notation. It is inspired by [einops](https://github.com/arogozhnikov/einops), but follows a novel and unique design:
 
 - Fully composable and powerful Einstein expressions with `[]`-notation.
 - Support for many tensor operations (`einx.{sum|max|where|add|dot|flip|get_at|...}`) with Numpy-like naming.
-- Easy integration and mixing with existing code. Supports tensor frameworks Numpy, PyTorch, Tensorflow and Jax.
+- Easy integration and mixing with existing code. Supports tensor frameworks Numpy, PyTorch, Tensorflow, Jax and others.
 - Just-in-time compilation of all operations into regular Python functions using Python's [`exec()`](https://docs.python.org/3/library/functions.html#exec).
 
 *Optional:*
 
 - Generalized neural network layers in Einstein notation. Supports PyTorch, Flax, Haiku, Equinox and Keras.
 
 **Getting started:**
@@ -51,30 +51,30 @@
 
 ## What does einx look like?
 
 #### Tensor manipulation
 
 ```python
 import einx
-x = {np.asarray|torch.as_tensor|jnp.asarray|tf.convert_to_tensor}(...) # Create some tensor
+x = {np.asarray|torch.as_tensor|jnp.asarray|...}(...) # Create some tensor
 
-einx.sum("a [b]", x)                              # Sum-reduction along columns
+einx.sum("a [b]", x)                              # Sum-reduction along second axis
 einx.flip("... (g [c])", x, c=2)                  # Flip pairs of values along the last axis
-einx.mean("b [s...] c", x)                        # Global mean-pooling
+einx.mean("b [s...] c", x)                        # Spatial mean-pooling
 einx.sum("b (s [s2])... c", x, s2=2)              # Sum-pooling with kernel_size=stride=2
-einx.add("b... [c]", x, b)                        # Add bias
+einx.add("a, b -> a b", x, y)                     # Outer sum
 
 einx.get_at("b [h w] c, b i [2] -> b i c", x, y)  # Gather values at coordinates
 
 einx.rearrange("b (q + k) -> b q, b k", x, q=2)   # Split
 einx.rearrange("b c, 1 -> b (c + 1)", x, [42])    # Append number to each channel
 
-einx.dot("... [c1|c2]", x, y)                     # Matmul = linear map from c1 to c2 channels
+einx.dot("... [c1->c2]", x, y)                    # Matmul = linear map from c1 to c2 channels
 
-# Vectorizing map
+                                                  # Apply custom operations:
 einx.vmap("b [s...] c -> b c", x, op=np.mean)     # Global mean-pooling
 einx.vmap("a [b], [b] c -> a c", x, y, op=np.dot) # Matmul
 ```
 
 All einx functions simply forward computation to the respective backend, e.g. by internally calling `np.reshape`, `np.transpose`, `np.sum` with the appropriate arguments.
 
 #### Common neural network operations
@@ -90,18 +90,18 @@
 
 # Multi-head attention
 attn = einx.dot("b q (h c), b k (h c) -> b q k h", q, k, h=8)
 attn = einx.softmax("b q [k] h", attn)
 x = einx.dot("b q k h, b k (h c) -> b q (h c)", attn, v)
 
 # Matmul in linear layers
-einx.dot("b...      [c1|c2]",  x, w)              # - Regular
-einx.dot("b...   (g [c1|c2])", x, w)              # - Grouped: Same weights per group
-einx.dot("b... ([g c1|g c2])", x, w)              # - Grouped: Different weights per group
-einx.dot("b  [s...|s2]  c",    x, w)              # - Spatial mixing as in MLP-mixer
+einx.dot("b...      [c1->c2]",  x, w)              # - Regular
+einx.dot("b...   (g [c1->c2])", x, w)              # - Grouped: Same weights per group
+einx.dot("b... ([g c1->g c2])", x, w)              # - Grouped: Different weights per group
+einx.dot("b  [s...->s2]  c",    x, w)              # - Spatial mixing as in MLP-mixer
 ```
 
 See [Common neural network ops](https://einx.readthedocs.io/en/latest/gettingstarted/commonnnops.html) for more examples.
 
 #### Deep learning modules
 
 ```python
@@ -109,18 +109,18 @@
 
 batchnorm       = einn.Norm("[b...] c", decay_rate=0.9)
 layernorm       = einn.Norm("b... [c]") # as used in transformers
 instancenorm    = einn.Norm("b [s...] c")
 groupnorm       = einn.Norm("b [s...] (g [c])", g=8)
 rmsnorm         = einn.Norm("b... [c]", mean=False, bias=False)
 
-channel_mix     = einn.Linear("b... [c1|c2]", c2=64)
-spatial_mix1    = einn.Linear("b [s...|s2] c", s2=64)
-spatial_mix2    = einn.Linear("b [s2|s...] c", s=(64, 64))
-patch_embed     = einn.Linear("b (s [s2|])... [c1|c2]", s2=4, c2=64)
+channel_mix     = einn.Linear("b... [c1->c2]", c2=64)
+spatial_mix1    = einn.Linear("b [s...->s2] c", s2=64)
+spatial_mix2    = einn.Linear("b [s2->s...] c", s=(64, 64))
+patch_embed     = einn.Linear("b (s [s2->])... [c1->c2]", s2=4, c2=64)
 
 dropout         = einn.Dropout("[...]",       drop_rate=0.2)
 spatial_dropout = einn.Dropout("[b] ... [c]", drop_rate=0.2)
 droppath        = einn.Dropout("[b] ...",     drop_rate=0.2)
 ```
 
 See `examples/train_{torch|flax|haiku|equinox|keras}.py` for example trainings on CIFAR10, [GPT-2](https://einx.readthedocs.io/en/latest/gettingstarted/gpt2.html) and [Mamba](https://github.com/fferflo/weightbridge/blob/master/examples/mamba2flax.py) for working example implementations of language models using einx, and [Tutorial: Neural networks](https://einx.readthedocs.io/en/latest/gettingstarted/neuralnetworks.html) for more details.
```

### Comparing `einx-0.1.3/README.md` & `einx-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPI version](https://badge.fury.io/py/einx.svg)](https://badge.fury.io/py/einx)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 einx is a Python library that allows formulating many tensor operations as concise expressions using Einstein notation. It is inspired by [einops](https://github.com/arogozhnikov/einops), but follows a novel and unique design:
 
 - Fully composable and powerful Einstein expressions with `[]`-notation.
 - Support for many tensor operations (`einx.{sum|max|where|add|dot|flip|get_at|...}`) with Numpy-like naming.
-- Easy integration and mixing with existing code. Supports tensor frameworks Numpy, PyTorch, Tensorflow and Jax.
+- Easy integration and mixing with existing code. Supports tensor frameworks Numpy, PyTorch, Tensorflow, Jax and others.
 - Just-in-time compilation of all operations into regular Python functions using Python's [`exec()`](https://docs.python.org/3/library/functions.html#exec).
 
 *Optional:*
 
 - Generalized neural network layers in Einstein notation. Supports PyTorch, Flax, Haiku, Equinox and Keras.
 
 **Getting started:**
@@ -33,30 +33,30 @@
 
 ## What does einx look like?
 
 #### Tensor manipulation
 
 ```python
 import einx
-x = {np.asarray|torch.as_tensor|jnp.asarray|tf.convert_to_tensor}(...) # Create some tensor
+x = {np.asarray|torch.as_tensor|jnp.asarray|...}(...) # Create some tensor
 
-einx.sum("a [b]", x)                              # Sum-reduction along columns
+einx.sum("a [b]", x)                              # Sum-reduction along second axis
 einx.flip("... (g [c])", x, c=2)                  # Flip pairs of values along the last axis
-einx.mean("b [s...] c", x)                        # Global mean-pooling
+einx.mean("b [s...] c", x)                        # Spatial mean-pooling
 einx.sum("b (s [s2])... c", x, s2=2)              # Sum-pooling with kernel_size=stride=2
-einx.add("b... [c]", x, b)                        # Add bias
+einx.add("a, b -> a b", x, y)                     # Outer sum
 
 einx.get_at("b [h w] c, b i [2] -> b i c", x, y)  # Gather values at coordinates
 
 einx.rearrange("b (q + k) -> b q, b k", x, q=2)   # Split
 einx.rearrange("b c, 1 -> b (c + 1)", x, [42])    # Append number to each channel
 
-einx.dot("... [c1|c2]", x, y)                     # Matmul = linear map from c1 to c2 channels
+einx.dot("... [c1->c2]", x, y)                    # Matmul = linear map from c1 to c2 channels
 
-# Vectorizing map
+                                                  # Apply custom operations:
 einx.vmap("b [s...] c -> b c", x, op=np.mean)     # Global mean-pooling
 einx.vmap("a [b], [b] c -> a c", x, y, op=np.dot) # Matmul
 ```
 
 All einx functions simply forward computation to the respective backend, e.g. by internally calling `np.reshape`, `np.transpose`, `np.sum` with the appropriate arguments.
 
 #### Common neural network operations
@@ -72,18 +72,18 @@
 
 # Multi-head attention
 attn = einx.dot("b q (h c), b k (h c) -> b q k h", q, k, h=8)
 attn = einx.softmax("b q [k] h", attn)
 x = einx.dot("b q k h, b k (h c) -> b q (h c)", attn, v)
 
 # Matmul in linear layers
-einx.dot("b...      [c1|c2]",  x, w)              # - Regular
-einx.dot("b...   (g [c1|c2])", x, w)              # - Grouped: Same weights per group
-einx.dot("b... ([g c1|g c2])", x, w)              # - Grouped: Different weights per group
-einx.dot("b  [s...|s2]  c",    x, w)              # - Spatial mixing as in MLP-mixer
+einx.dot("b...      [c1->c2]",  x, w)              # - Regular
+einx.dot("b...   (g [c1->c2])", x, w)              # - Grouped: Same weights per group
+einx.dot("b... ([g c1->g c2])", x, w)              # - Grouped: Different weights per group
+einx.dot("b  [s...->s2]  c",    x, w)              # - Spatial mixing as in MLP-mixer
 ```
 
 See [Common neural network ops](https://einx.readthedocs.io/en/latest/gettingstarted/commonnnops.html) for more examples.
 
 #### Deep learning modules
 
 ```python
@@ -91,18 +91,18 @@
 
 batchnorm       = einn.Norm("[b...] c", decay_rate=0.9)
 layernorm       = einn.Norm("b... [c]") # as used in transformers
 instancenorm    = einn.Norm("b [s...] c")
 groupnorm       = einn.Norm("b [s...] (g [c])", g=8)
 rmsnorm         = einn.Norm("b... [c]", mean=False, bias=False)
 
-channel_mix     = einn.Linear("b... [c1|c2]", c2=64)
-spatial_mix1    = einn.Linear("b [s...|s2] c", s2=64)
-spatial_mix2    = einn.Linear("b [s2|s...] c", s=(64, 64))
-patch_embed     = einn.Linear("b (s [s2|])... [c1|c2]", s2=4, c2=64)
+channel_mix     = einn.Linear("b... [c1->c2]", c2=64)
+spatial_mix1    = einn.Linear("b [s...->s2] c", s2=64)
+spatial_mix2    = einn.Linear("b [s2->s...] c", s=(64, 64))
+patch_embed     = einn.Linear("b (s [s2->])... [c1->c2]", s2=4, c2=64)
 
 dropout         = einn.Dropout("[...]",       drop_rate=0.2)
 spatial_dropout = einn.Dropout("[b] ... [c]", drop_rate=0.2)
 droppath        = einn.Dropout("[b] ...",     drop_rate=0.2)
 ```
 
 See `examples/train_{torch|flax|haiku|equinox|keras}.py` for example trainings on CIFAR10, [GPT-2](https://einx.readthedocs.io/en/latest/gettingstarted/gpt2.html) and [Mamba](https://github.com/fferflo/weightbridge/blob/master/examples/mamba2flax.py) for working example implementations of language models using einx, and [Tutorial: Neural networks](https://einx.readthedocs.io/en/latest/gettingstarted/neuralnetworks.html) for more details.
```

### Comparing `einx-0.1.3/einx/backend/__init__.py` & `einx-0.2.0/einx/backend/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,80 @@
-import sys, einx, threading
+import sys
+import einx
+import threading
 
 from .base import Backend
 
 backends = []
 backend_factories = {}
 lock = threading.Lock()
 
 from ._numpy import numpy
+
 backends.append(numpy)
 
 from ._jax import make_jax_backend
+
 backend_factories["jax"] = make_jax_backend
 
 from ._torch import make_torch_backend
+
 backend_factories["torch"] = make_torch_backend
 
 from ._tensorflow import make_tensorflow_backend
+
 backend_factories["tensorflow"] = make_tensorflow_backend
 
+from ._mlx import make_mlx_backend
+
+backend_factories["mlx"] = make_mlx_backend
+
+from ._dask import make_dask_backend
+
+backend_factories["dask"] = make_dask_backend
+
 from .tracer import tracer
+
 backends.append(tracer)
 
+
 def _update():
     for backend_name in list(backend_factories.keys()):
         if backend_name in sys.modules:
             backend = backend_factories[backend_name]()
             backends.append(backend)
             globals()[backend_name] = backend
             del backend_factories[backend_name]
+
+
 _update()
 
 
 type_to_backend = {}
 
+
 def _get1(tensor):
     tensor_backend = type_to_backend.get(type(tensor), None)
     if tensor_backend is None:
         _update()
 
         if tensor_backend is None:
             for tensor_backend in backends:
-                if isinstance(tensor, tensor_backend.tensor) and not isinstance(tensor, numpy.tensor):
+                if isinstance(tensor, tensor_backend.tensor) and not isinstance(
+                    tensor, numpy.tensor
+                ):
                     break
             else:
                 # Default backend is numpy
                 tensor_backend = numpy
 
         type_to_backend[type(tensor)] = tensor_backend
     return tensor_backend
 
+
 def get(arg):
     with lock:
         if isinstance(arg, str):
             name = arg
             for backend in backends:
                 if backend.name == name:
                     return backend
@@ -63,17 +85,20 @@
             raise ValueError(f"Backend {name} not found")
         else:
             tensors = arg
             if len(tensors) == 1:
                 return _get1(tensors[0])
             backend = None
             for tensor in tensors:
-                if not tensor is None:
+                if tensor is not None:
                     backend2 = _get1(tensor)
                     if backend2 != numpy:
-                        if not backend is None and backend != backend2:
-                            raise ValueError(f"Got tensors with conflicting backends: {backend.__name__} and {backend2.__name__}")
+                        if backend is not None and backend != backend2:
+                            raise ValueError(
+                                "Got tensors with conflicting backends: "
+                                f"{backend.__name__} and {backend2.__name__}"
+                            )
                         backend = backend2
             if backend is None:
                 return numpy
             else:
                 return backend
```

### Comparing `einx-0.1.3/einx/backend/_jax.py` & `einx-0.2.0/einx/backend/_jax.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from functools import partial
 from .base import Backend, associative_binary_to_nary
 
+
 def make_jax_backend():
     import jax as jax_
     import jax.numpy as jnp
+
     class jax(Backend):
-        @staticmethod
         def to_tensor(tensor):
             return jnp.asarray(tensor)
 
         tensor = jnp.ndarray
         name = "jax"
 
-        cast = lambda tensor, dtype: tensor.astype(dtype)
+        def cast(tensor, dtype):
+            return tensor.astype(dtype)
+
         reshape = jnp.reshape
         transpose = jnp.transpose
         broadcast_to = jnp.broadcast_to
         einsum = partial(jnp.einsum, optimize="optimal")
-        dot = jnp.dot
         swapaxes = jnp.swapaxes
         arange = jnp.arange
 
         stack = jnp.stack
         concatenate = jnp.concatenate
 
         zeros = jnp.zeros
@@ -55,18 +57,21 @@
         all = jnp.all
         min = jnp.amin
         max = jnp.amax
         logsumexp = jax_.scipy.special.logsumexp
 
         def get_at(tensor, coordinates):
             return tensor[coordinates]
+
         def set_at(tensor, coordinates, updates):
             return tensor.at[coordinates].set(updates)
+
         def add_at(tensor, coordinates, updates):
             return tensor.at[coordinates].add(updates)
+
         def subtract_at(tensor, coordinates, updates):
             return tensor.at[coordinates].add(-updates)
 
         flip = jnp.flip
         roll = jnp.roll
         softmax = jax_.nn.softmax
         log_softmax = jax_.nn.log_softmax
@@ -80,8 +85,8 @@
         def vmap(op, in_axes, out_axes, input_shapes=None, output_shapes=None):
             return jax_.vmap(op, in_axes, out_axes)
 
         class random:
             def bernoulli(rng, p, shape):
                 return jax_.random.bernoulli(rng, p, shape)
 
-    return jax
+    return jax
```

### Comparing `einx-0.1.3/einx/backend/_numpy.py` & `einx-0.2.0/einx/backend/_numpy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import numpy as np
 from functools import partial
 from .base import Backend, associative_binary_to_nary
 
+
 class numpy(Backend):
-    @staticmethod
     def to_tensor(tensor):
         return np.asarray(tensor)
 
     tensor = np.ndarray
     name = "numpy"
 
-    cast = lambda tensor, dtype: tensor.astype(dtype)
+    def cast(tensor, dtype):
+        return tensor.astype(dtype)
+
     reshape = np.reshape
     transpose = np.transpose
     broadcast_to = np.broadcast_to
     einsum = partial(np.einsum, optimize="optimal")
-    dot = np.dot
     swapaxes = np.swapaxes
     arange = np.arange
 
     stack = np.stack
     concatenate = np.concatenate
 
     zeros = np.zeros
@@ -49,66 +50,86 @@
     std = np.std
     prod = np.prod
     count_nonzero = np.count_nonzero
     any = np.any
     all = np.all
     min = np.amin
     max = np.amax
+
     def logsumexp(x, axis=None, keepdims=False):
         if isinstance(axis, int):
             axis = (axis,)
         x_max1 = np.max(x, axis=axis, keepdims=keepdims)
         x_max2 = x_max1
         if not keepdims:
             for a in sorted(axis):
                 x_max2 = np.expand_dims(x_max2, axis=a)
         return np.log(np.sum(np.exp(x - x_max2), axis=axis, keepdims=keepdims)) + x_max1
 
     def get_at(tensor, coordinates):
         return tensor[coordinates]
+
     def set_at(tensor, coordinates, updates):
         tensor[coordinates] = updates
         return tensor
+
     def add_at(tensor, coordinates, updates):
         tensor[coordinates] += updates
         return tensor
+
     def subtract_at(tensor, coordinates, updates):
         tensor[coordinates] -= updates
         return tensor
 
     flip = np.flip
     roll = np.roll
 
     def softmax(x, axis=None):
         x = x - np.max(x, axis=axis, keepdims=True)
         return np.exp(x) / np.sum(np.exp(x), axis=axis, keepdims=True)
+
     def log_softmax(x, axis=None):
         x = x - np.max(x, axis=axis, keepdims=True)
         return x - np.log(np.sum(np.exp(x), axis=axis, keepdims=True))
 
     sqrt = np.sqrt
-    rsqrt = lambda x: 1.0 / np.sqrt(x)
+
+    def rsqrt(x):
+        return 1.0 / np.sqrt(x)
+
     square = np.square
 
     allclose = np.allclose
 
     def vmap(op, in_axes, out_axes, input_shapes=None, output_shapes=None):
         if not isinstance(in_axes, (tuple, list)) or not isinstance(out_axes, (tuple, list)):
             raise ValueError("in_axes and out_axes must be tuples or lists of integers")
+
         def inner(*args):
             if len(args) != len(in_axes):
                 raise ValueError(f"Expected {len(in_axes)} arguments, got {len(args)}")
-            value = set(arg.shape[axis] for arg, axis in zip(args, in_axes) if not axis is None)
+            value = {arg.shape[axis] for arg, axis in zip(args, in_axes) if axis is not None}
             if len(value) != 1:
-                raise ValueError(f"Expected all arguments to have same size along vmap axis, got {value}")
+                raise ValueError(
+                    f"Expected all arguments to have same size along vmap axis, got {value}"
+                )
             value = value.pop()
             xs_stacks = [[]] * len(out_axes)
             for i in range(value):
-                xs = op(*[arg[(slice(None),) * axis + (i,)] if not axis is None else arg for arg, axis in zip(args, in_axes)])
+                xs = op(*[
+                    arg[(slice(None),) * axis + (i,)] if axis is not None else arg
+                    for arg, axis in zip(args, in_axes)
+                ])
                 if len(xs) != len(out_axes):
-                    raise ValueError(f"Expected {len(out_axes)} arguments from vmapped function, got {len(xs)}")
+                    raise ValueError(
+                        f"Expected {len(out_axes)} arguments from vmapped function, got {len(xs)}"
+                    )
                 for xs_stack, x in zip(xs_stacks, xs):
                     xs_stack.append(x)
-            xs = tuple(np.stack(xs_stack, axis=out_axis) for out_axis, xs_stack in zip(out_axes, xs_stacks))
+            xs = tuple(
+                np.stack(xs_stack, axis=out_axis) for out_axis, xs_stack in zip(out_axes, xs_stacks)
+            )
             return xs
-        inner.__name__ = f"vmap({op.__name__ if '__name__' in dir(op) else str(op)}, in_axes={in_axes}, out_axes={out_axes})"
+
+        inner.__name__ = f"vmap({op.__name__ if '__name__' in dir(op) else str(op)}, "
+        f"in_axes={in_axes}, out_axes={out_axes})"
         return inner
```

### Comparing `einx-0.1.3/einx/backend/_tensorflow.py` & `einx-0.2.0/einx/backend/_tensorflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from functools import partial
 from .base import Backend, associative_binary_to_nary
 
+
 def make_tensorflow_backend():
     import tensorflow as tf
     import tensorflow.experimental.numpy as tnp
 
     def prepare_coordinates_and_update(coordinates, updates):
         if isinstance(coordinates, tuple):
             shape = coordinates[0].shape
@@ -20,38 +21,39 @@
         shape = tf.broadcast_static_shape(updates.shape, coordinates.shape[:-1])
         coordinates = tf.broadcast_to(coordinates, shape + coordinates.shape[-1:])
         updates = tf.broadcast_to(updates, shape)
 
         return coordinates, updates
 
     class tensorflow(Backend):
-        @staticmethod
         def to_tensor(tensor):
             tensor = tf.convert_to_tensor(tensor)
             if any(s is None for s in tensor.shape):
                 raise ValueError("Tensorflow tensors with dynamic shape are not supported")
             return tensor
 
         tensor = tf.Tensor
         name = "tensorflow"
 
         cast = tf.cast
         reshape = tf.reshape
         transpose = tf.transpose
         broadcast_to = tf.broadcast_to
         einsum = partial(tnp.einsum, optimize="optimal")
-        dot = tnp.dot
         swapaxes = tnp.swapaxes
         arange = tnp.arange
 
         stack = tnp.stack
         concatenate = tnp.concatenate
 
-        zeros = lambda shape, dtype="float32": tf.zeros(shape, dtype=dtype)
-        ones = lambda shape, dtype="float32": tf.ones(shape, dtype=dtype)
+        def zeros(shape, dtype="float32"):
+            return tf.zeros(shape, dtype=dtype)
+
+        def ones(shape, dtype="float32"):
+            return tf.ones(shape, dtype=dtype)
 
         add = associative_binary_to_nary(tnp.add)
         subtract = tnp.subtract
         multiply = associative_binary_to_nary(tnp.multiply)
         true_divide = tnp.true_divide
         floor_divide = tnp.floor_divide
         divide = tnp.divide
@@ -77,83 +79,115 @@
         all = tnp.all
         min = tnp.min
         max = tnp.max
         logsumexp = tf.math.reduce_logsumexp
 
         def get_at(tensor, coordinates):
             return tensor[coordinates]
+
         def set_at(tensor, coordinates, updates):
             coordinates, updates = prepare_coordinates_and_update(coordinates, updates)
             return tf.tensor_scatter_nd_update(tensor, coordinates, updates)
+
         def add_at(tensor, coordinates, updates):
             coordinates, updates = prepare_coordinates_and_update(coordinates, updates)
             return tf.tensor_scatter_nd_add(tensor, coordinates, updates)
+
         def subtract_at(tensor, coordinates, updates):
             coordinates, updates = prepare_coordinates_and_update(coordinates, updates)
             return tf.tensor_scatter_nd_sub(tensor, coordinates, updates)
 
         def flip(x, axis):
             if isinstance(axis, int):
                 axis = [axis]
             return tf.reverse(x, axis)
+
         def roll(x, axis, shift):
             if isinstance(axis, int):
                 axis = [axis]
             if isinstance(shift, int):
                 shift = [shift]
             return tf.roll(x, tuple(shift), axis=tuple(axis))
+
         def softmax(x, axis):
             if isinstance(axis, (list, tuple)):
                 if len(axis) != 1:
-                    raise ValueError(f"Tensorflow only supports softmax along a single axis, got {len(axis)} axes")
+                    raise ValueError(
+                        "Tensorflow only supports softmax along a single axis, "
+                        f"got {len(axis)} axes"
+                    )
                 axis = axis[0]
             return tf.nn.softmax(x, axis=axis)
+
         def log_softmax(x, axis):
             if isinstance(axis, (list, tuple)):
                 if len(axis) != 1:
-                    raise ValueError(f"Tensorflow only supports log_softmax along a single axis, got {len(axis)} axes")
+                    raise ValueError(
+                        "Tensorflow only supports log_softmax along a single axis, "
+                        f"got {len(axis)} axes"
+                    )
                 axis = axis[0]
             return tf.nn.log_softmax(x, axis=axis)
 
         sqrt = tf.math.sqrt
         rsqrt = tf.math.rsqrt
         square = tnp.square
 
         allclose = tnp.allclose
 
         def vmap(op, in_axes, out_axes, input_shapes=None, output_shapes=None):
             def inner(*args):
-                # TODO: suboptimal (?) implementation of vmap in tensorflow that transposes the vmapped axis to the front and calls tf.vectorized_map
+                # TODO: suboptimal (?) implementation of vmap in tensorflow that transposes the
+                # vmapped axis to the front and calls tf.vectorized_map
                 if len(args) != len(in_axes):
                     raise ValueError(f"Expected {len(in_axes)} arguments, got {len(args)}")
-                value = set(arg.shape[axis] for arg, axis in zip(args, in_axes) if not axis is None)
+                value = {arg.shape[axis] for arg, axis in zip(args, in_axes) if axis is not None}
                 if len(value) != 1:
-                    raise ValueError(f"Expected all arguments to have same size along vmap axis, got {value}")
+                    raise ValueError(
+                        f"Expected all arguments to have same size along vmap axis, got {value}"
+                    )
                 value = value.pop()
 
                 # Move vmapped axes to front
                 xs = []
                 for arg, axis in zip(args, in_axes):
-                    if not axis is None:
+                    if axis is not None:
                         if axis != 0:
                             perm = [axis] + [a for a in range(len(arg.shape)) if a != axis]
                             arg = tf.transpose(arg, perm=perm)
                     else:
                         arg = arg[tf.newaxis]
                     xs.append(arg)
 
                 xs = tf.vectorized_map(lambda xs: op(*xs), xs)
                 if len(xs) != len(out_axes):
-                    raise ValueError(f"Expected {len(out_axes)} arguments from vmapped function, got {len(xs)}")
+                    raise ValueError(
+                        f"Expected {len(out_axes)} arguments from vmapped function, got {len(xs)}"
+                    )
 
                 # Move vmapped axis to out_axis
-                xs = [tf.transpose(x, perm=[(a + 1 if a < out_axis else (0 if a == out_axis else a)) for a in range(len(x.shape))]) for x, out_axis in zip(xs, out_axes)]
+                xs = [
+                    tf.transpose(
+                        x,
+                        perm=[
+                            (a + 1 if a < out_axis else (0 if a == out_axis else a))
+                            for a in range(len(x.shape))
+                        ],
+                    )
+                    for x, out_axis in zip(xs, out_axes)
+                ]
 
                 return tuple(xs)
-            inner.__name__ = f"vmap({op.__name__ if '__name__' in dir(op) else str(op)}, in_axes={in_axes}, out_axes={out_axes})"
+
+            inner.__name__ = (
+                f"vmap({op.__name__ if '__name__' in dir(op) else str(op)}, "
+                f"in_axes={in_axes}, out_axes={out_axes})"
+            )
             return inner
 
         class random:
             def bernoulli(rng, p, shape):
-                return tf.random.uniform(shape, minval=0.0, maxval=1.0, dtype="float32", seed=rng) <= p
+                return (
+                    tf.random.uniform(shape, minval=0.0, maxval=1.0, dtype="float32", seed=rng) <= p
+                )
 
     return tensorflow
```

### Comparing `einx-0.1.3/einx/backend/tracer.py` & `einx-0.2.0/einx/backend/tracer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 from functools import partial
 import numpy as np
-import operator, einx
+import operator
+import einx
 from .base import Backend
 
+
 def is_leaf(key, x):
-    return (isinstance(x, (tuple, list, np.ndarray)) and all([isinstance(y, (int, np.integer)) for y in x]))
+    return isinstance(x, (tuple, list, np.ndarray)) and all(
+        isinstance(y, (int, np.integer)) for y in x
+    )
+
+
+def to_shape(shape):
+    if isinstance(shape, np.ndarray):
+        return tuple(shape.tolist())
+    elif isinstance(shape, list):
+        return tuple(shape)
+    else:
+        return shape
 
-class Tracer:
+
+class Tensor:
     def __init__(self, shape):
-        if isinstance(shape, np.ndarray):
-            shape = tuple(shape.tolist())
-        elif isinstance(shape, list):
-            shape = tuple(shape)
-        self.shape = shape
+        self.shape = to_shape(shape)
 
     @property
     def ndim(self):
         if self.shape is None:
             raise ValueError("Cannot get ndim of tensor with unknown shape")
         return len(self.shape)
 
     def __getitem__(self, key):
-        if self.shape is None:
-            shape = None
-        else:
-            if isinstance(key, (int, slice)) or key is None:
-                slices = (key,)
-            else:
-                slices = key
-            if len(slices) > len(self.shape):
-                raise ValueError(f"Too many indices for tensor of dimension {len(self.shape)}")
-
-            output_shape = []
-            input_shape = self.shape
-            for s in slices:
-                if isinstance(s, int):
-                    input_shape = input_shape[1:]
-                elif isinstance(s, slice):
-                    start, stop, step = s.indices(input_shape[0])
-                    output_shape.append((stop - start) // step)
-                    input_shape = input_shape[1:]
-                elif s is None:
-                    output_shape.append(1)
-                else:
-                    raise TypeError(f"Invalid key type: {type(slice)}")
-            shape = tuple(output_shape) + tuple(input_shape)
-
-        return OpApplication(operator.getitem, args=[self, key], output_shapes=shape).output_tracers
+        return index(self, key, update=None, op="get_at")
 
     def __add__(self, other):
         return elementwise(self, other, op="add")
 
     def __radd__(self, other):
         return elementwise(other, self, op="add")
 
@@ -110,189 +95,215 @@
 
     def __eq__(self, other):
         return elementwise(self, other, op="equal")
 
     def __ne__(self, other):
         return elementwise(self, other, op="not_equal")
 
-class Input(Tracer):
+
+class Input(Tensor):
     def __init__(self, shape, index, original_type=None):
         super().__init__(shape)
         self.index = index
         self.original_type = original_type
 
     def __str__(self):
-        return f"tracer.Input({self.shape})"
+        return f"Input({self.shape})"
 
     def __hash__(self):
         return 712873 + hash(self.shape) + hash(self.original_type)
 
     def __eq__(self, other):
-        return isinstance(other, Input) and self.shape == other.shape and self.original_type == other.original_type
+        return (
+            isinstance(other, Input)
+            and self.shape == other.shape
+            and self.original_type == other.original_type
+        )
+
 
 class Op:
     def __init__(self, op, tracable):
         assert not isinstance(op, VmappedOp)
         self.op = op
         self.tracable = tracable
 
     @property
     def __name__(self):
-        if "__name" in dir(self.op):
+        if "__name__" in dir(self.op):
             return self.op.__name__
         else:
             return str(self.op)
 
     @property
-    def requires_dynamic_type_check(self):
+    def requires_dynamic_shape_check(self):
         return not self.tracable
 
     def __call__(self, *args, **kwargs):
         assert self.tracable
         if isinstance(self.op, str):
             x = tracer
             for name in self.op.split("."):
                 x = getattr(x, name)
             op = x
         else:
             op = self.op
         return op(*args, **kwargs)
 
+
 class OpApplication:
-    def __init__(self, op, args=[], kwargs={}, output_shapes=None):
+    def __init__(self, op, args=None, kwargs=None, output_shapes=None):
+        if kwargs is None:
+            kwargs = {}
+        if args is None:
+            args = []
         if not isinstance(op, (Op, VmappedOp)):
             op = Op(op, tracable=isinstance(op, str))
-        assert not isinstance(op, Op) or (not op.tracable or isinstance(op.op, str)), f"{op} {op.op}"
+        assert not isinstance(op, Op) or (
+            not op.tracable or isinstance(op.op, str)
+        ), f"{op} {op.op}"
         self.op = op
         self.args = args
         self.kwargs = kwargs
-        self.output_shapes = einx.tree_util.tree_map_with_key(lambda shape, key: tuple(int(i) for i in shape), output_shapes, is_leaf=is_leaf)
-        self.output_tracers = einx.tree_util.tree_map_with_key(lambda shape, key: OpOutput(self, shape, key), self.output_shapes, is_leaf=is_leaf)
-        assert not "backend" in self.kwargs
+        self.output_shapes = einx.tree_util.tree_map_with_key(
+            lambda shape, key: tuple(int(i) for i in shape), output_shapes, is_leaf=is_leaf
+        )
+        self.output_tracers = einx.tree_util.tree_map_with_key(
+            lambda shape, key: OpOutput(self, shape, key), self.output_shapes, is_leaf=is_leaf
+        )
+        assert "backend" not in self.kwargs
 
-class OpOutput(Tracer):
-    def __init__(self, op, shape, key):
+
+class OpOutput(Tensor):
+    def __init__(self, application, shape, key):
         super().__init__(shape)
-        self.op = op
+        self.application = application
         self.key = key
 
+
 def drop_axis(shape, axis):
     if axis is None:
         return shape
     else:
-        return shape[:axis] + shape[axis + 1:]
+        return shape[:axis] + shape[axis + 1 :]
+
 
 class VmappedOp:
     def __init__(self, op, in_axes, out_axes, input_shapes, output_shapes):
         self.in_axes = in_axes
         self.out_axes = out_axes
         self.input_shapes = input_shapes
         self.output_shapes = output_shapes
 
         if not isinstance(op, VmappedOp):
             # Trace vmapped functions again
             if isinstance(op, Op):
                 assert op.tracable
                 op = op.op
-            input_tracers = [einx.backend.tracer.Input(shape, i) for i, shape in enumerate(self.inner_input_shapes)]
+            input_tracers = [Input(shape, i) for i, shape in enumerate(self.inner_input_shapes)]
             output_tracers = op(*input_tracers)
-            op = einx.backend.tracer.Graph(output_tracers, args=input_tracers, kwargs={}, backend=einx.backend.tracer)
+            op = Graph(output_tracers, args=input_tracers, kwargs={}, backend=einx.backend.tracer)
         self.op = op
 
     @property
     def tracable(self):
         return False
 
     @property
-    def requires_dynamic_type_check(self):
+    def requires_dynamic_shape_check(self):
         return False
 
     @property
     def inner_input_shapes(self):
         return [drop_axis(shape, axis) for shape, axis in zip(self.input_shapes, self.in_axes)]
 
     @property
     def inner_output_shapes(self):
         return [drop_axis(shape, axis) for shape, axis in zip(self.output_shapes, self.out_axes)]
 
     def __call__(self, *args, **kwargs):
-        return OpApplication(self, args=args, kwargs=kwargs, output_shapes=self.output_shapes).output_tracers
+        return OpApplication(
+            self, args=args, kwargs=kwargs, output_shapes=self.output_shapes
+        ).output_tracers
 
-class VmappedOpOutput(Tracer):
-    def __init__(self, vmapped_op, index):
-        super().__init__(vmapped_op.output_shapes[index])
-        self.vmapped_op = vmapped_op
-        self.index = index
 
 class Scope:
     def __init__(self, backend, parent_scope=None):
         self.backend = backend
         self.parent_scope = parent_scope
         self.constants = [] if parent_scope is None else None
         self.locals = {}
         self.lines = []
         self.used_functions = set()
 
     @property
     def root_scope(self):
         scope = self
-        while not scope.parent_scope is None:
+        while scope.parent_scope is not None:
             scope = scope.parent_scope
         return scope
 
     def __str__(self):
         string = ""
         string += f"# backend: einx.backend.{self.backend.name}\n"
         for const_name, value in self.root_scope.constants:
             string += f"# {const_name}: {str(type(value))} = {value}\n"
         string += "\n".join(self.lines)
         return string
 
     def exec(self, names):
-        scope_globals = {const_name: value for const_name, value in self.constants}
+        scope_globals = dict(self.constants)
         scope_globals["einx"] = einx
         scope_globals["partial"] = partial
         scope_globals["backend"] = self.backend
         scope_locals = {}
         exec("\n".join(self.lines), scope_globals, scope_locals)
         return einx.tree_util.tree_map(lambda name: scope_locals[name], names)
 
     def get_name_for(self, x):
         if id(x) in self.locals:
             return self.locals[id(x)]
-        elif not self.parent_scope is None:
+        elif self.parent_scope is not None:
             return self.parent_scope.get_name_for(x)
         else:
             return None
 
     def name_exists(self, name):
         if name in self.locals.values():
             return True
-        elif not self.parent_scope is None:
+        elif self.parent_scope is not None:
             return self.parent_scope.name_exists(name)
         else:
             return False
 
     def declare_local_name_for(self, x, prefix="x"):
         if x is None:
-            x = lambda: 1 # Unique new object
+
+            def x():
+                return 1  # Unique new object
+
         i = 0
         while self.name_exists(name := f"{prefix}{i}"):
             i += 1
         self.locals[id(x)] = name
         return name
 
     def define_function(self, graph):
         name = self.declare_local_name_for(graph, prefix="op")
 
         function_scope = Scope(self.backend, parent_scope=self)
 
         lines = []
         output = function_scope.eval(graph.output)
-        lines.insert(0, f"def {name}({', '.join([function_scope.eval(x) for x in graph.input_tracers] + [op + '=' + op for op in function_scope.used_functions])}):")
+        params = [function_scope.eval(x) for x in graph.input_tracers] + [
+            op + "=" + op for op in function_scope.used_functions
+        ]
+        lines.insert(
+            0,
+            f"def {name}({', '.join(params)}):",
+        )
         for line in function_scope.lines:
             lines.append(f"    {line}")
         lines.append(f"    return {output}")
 
         self.lines.extend(lines)
 
         return name
@@ -333,122 +344,227 @@
                     slices = (slices,)
                 assert isinstance(slices, tuple)
                 assert len(slices) > 0
 
                 def slice_to_str(s):
                     if isinstance(s, slice):
                         x = ""
-                        if not s.start is None:
+                        if s.start is not None:
                             x += str(s.start)
                         x += ":"
-                        if not s.stop is None:
+                        if s.stop is not None:
                             x += str(s.stop)
-                        if not s.step is None:
+                        if s.step is not None:
                             x += ":" + str(s.step)
                         return x
                     else:
                         return self.eval(s)
+
                 slices = ", ".join(slice_to_str(s) for s in slices)
 
                 name = self.declare_local_name_for(x)
 
                 line = f"{name} = {tensor}[" + slices + "]"
                 self.lines.append(line)
-            elif x.op.op == "to_tensor" and self.backend != einx.backend.tracer and isinstance(x.args[0], Input) and not x.args[0].original_type is None and issubclass(x.args[0].original_type, self.backend.tensor):
-                # Skip to_tensor op if tensor already has right type
-                name = self.eval(x.args[0])
             else:
                 args = x.args
                 kwargs = x.kwargs
 
                 name = self.declare_local_name_for(x)
 
                 if self.backend == einx.backend.tracer and not isinstance(x.op.op, str):
                     op = self.eval(x.op)
 
                     args = self.eval(args)
                     kwargs = self.eval(kwargs)
 
-                    self.lines.append(f"{name} = backend.apply({op}, args={args}, kwargs={kwargs}, output_shapes={self.eval(x.output_shapes)})")
+                    self.lines.append(
+                        f"{name} = backend.apply({op}, args={args}, kwargs={kwargs}, "
+                        f"output_shapes={self.eval(x.output_shapes)})"
+                    )
                 else:
                     op = self.eval(x.op)
-                    args = [self.eval(a) for a in args] + [f"{k}={self.eval(v)}" for k, v in kwargs.items()]
+                    args = [self.eval(a) for a in args] + [
+                        f"{k}={self.eval(v)}" for k, v in kwargs.items()
+                    ]
                     if op == "einx.param.instantiate":
-                        args += [f"backend=backend"]
+                        args += ["backend=backend"]
                     args = ", ".join(args)
 
                     self.lines.append(f"{name} = {op}(" + args + ")")
 
                 # Shape assertion
-                if self.backend != einx.backend.tracer and x.op.requires_dynamic_type_check:
+                if self.backend != einx.backend.tracer and x.op.requires_dynamic_shape_check:
+
                     def assertion(tracer, shape):
                         self.lines.append(f"assert {self.eval(tracer)}.shape == {self.eval(shape)}")
+
                     einx.tree_util.tree_map(assertion, x.output_tracers, x.output_shapes)
         elif isinstance(x, OpOutput):
-            name = self.eval(x.op)
+            name = self.eval(x.application)
             for k in x.key:
                 name += f"[{self.eval(k)}]"
         elif isinstance(x, VmappedOp):
             old_name = self.eval(x.op)
             name = self.declare_local_name_for(None, prefix="op")
             if self.backend == einx.backend.tracer:
-                self.lines.append(f"{name} = backend.vmap({old_name}, in_axes={self.eval(x.in_axes)}, out_axes={self.eval(x.out_axes)}, input_shapes={self.eval(x.input_shapes)}, output_shapes={self.eval(x.output_shapes)})")
+                self.lines.append(
+                    f"{name} = backend.vmap({old_name}, in_axes={self.eval(x.in_axes)}, "
+                    f"out_axes={self.eval(x.out_axes)}, input_shapes={self.eval(x.input_shapes)}, "
+                    f"output_shapes={self.eval(x.output_shapes)})"
+                )
             else:
-                self.lines.append(f"{name} = backend.vmap({old_name}, in_axes={self.eval(x.in_axes)}, out_axes={self.eval(x.out_axes)})")
-        elif isinstance(x, VmappedOpOutput):
-            name = self.eval(x.op)
-            name = f"{name}[{self.eval(x.index)}]"
+                self.lines.append(
+                    f"{name} = backend.vmap({old_name}, in_axes={self.eval(x.in_axes)}, "
+                    f"out_axes={self.eval(x.out_axes)})"
+                )
         elif isinstance(x, str):
-            name = f"\"{x}\""
+            name = f'"{x}"'
         elif isinstance(x, tuple):
             name = "(" + ", ".join(self.eval(a) for a in x) + ("," if len(x) == 1 else "") + ")"
         elif isinstance(x, list):
             name = "[" + ", ".join(self.eval(a) for a in x) + "]"
         elif isinstance(x, dict):
-            name = "{" + ", ".join(f"\"{k}\": {self.eval(v)}" for k, v in x.items()) + "}"
-        elif isinstance(x, (int, float)):
+            name = "{" + ", ".join(f'"{k}": {self.eval(v)}' for k, v in x.items()) + "}"
+        elif isinstance(x, (int, float, np.integer, np.floating)):
             name = str(x)
         elif isinstance(x, slice):
-            if not x.step is None:
+            if x.step is not None:
                 return f"slice({self.eval(x.start)}, {self.eval(x.stop)}, {self.eval(x.step)})"
-            elif not x.stop is None:
+            elif x.stop is not None:
                 return f"slice({self.eval(x.start)}, {self.eval(x.stop)})"
             else:
                 return f"slice({self.eval(x.start)})"
         elif x is None:
             name = "None"
         else:
             # Add to root scope as constant
             name = self.declare_local_name_for(x, prefix="const")
             self.root_scope.constants.append((name, x))
             self.root_scope.locals[id(x)] = name
-            return name # Don't add to locals
+            return name  # Don't add to locals
 
-        assert not name is None
+        assert name is not None
         self.locals[id(x)] = name
         return name
 
+
+def optimize(output, backend):
+    new_nodes = {}
+
+    def _optimize(node):
+        if id(node) in new_nodes:
+            return new_nodes[id(node)]
+
+        if isinstance(node, OpApplication):
+            if (
+                node.op.op == "reshape"
+                and isinstance(node.args[0], OpOutput)
+                and node.args[0].application.op.op == "reshape"
+            ):
+                # Merge consecutive reshape ops
+                new_node = OpApplication(
+                    "reshape",
+                    args=[node.args[0].application.args[0], node.output_shapes],
+                    output_shapes=node.output_shapes,
+                )
+            elif (
+                node.op.op == "to_tensor"
+                and isinstance(node.args[0], OpOutput)
+                and node.args[0].application.op.op == "to_tensor"
+            ):
+                # Merge consecutive to_tensor ops
+                new_node = _optimize(node.args[0].application)
+            else:
+                new_node = OpApplication(
+                    node.op,
+                    args=[_optimize(a) for a in node.args],
+                    kwargs={k: _optimize(v) for k, v in node.kwargs.items()},
+                    output_shapes=node.output_shapes,
+                )
+        elif isinstance(node, OpOutput):
+            if (
+                node.application.op.op == "to_tensor"
+                and backend != einx.backend.tracer
+                and isinstance(node.application.args[0], Input)
+                and node.application.args[0].original_type is not None
+                and issubclass(node.application.args[0].original_type, backend.tensor)
+            ):
+                # Skip to_tensor op if tensor already has right type
+                new_node = _optimize(node.application.args[0])
+            elif (
+                node.application.op.op == "reshape" and node.application.args[0].shape == node.shape
+            ):
+                # Skip reshape op if tensor already has right shape
+                new_node = _optimize(node.application.args[0])
+            elif (
+                node.application.op.op == "broadcast_to"
+                and node.application.args[0].shape == node.shape
+            ):
+                # Skip broadcast_to op if tensor already has right shape
+                new_node = _optimize(node.application.args[0])
+            elif node.application.op.op == "transpose" and list(node.application.args[1]) == list(
+                range(len(node.shape))
+            ):
+                # Skip transpose op if permutation is identity
+                new_node = _optimize(node.application.args[0])
+            else:
+                new_node = OpOutput(_optimize(node.application), node.shape, node.key)
+        elif isinstance(node, VmappedOp):
+            new_node = VmappedOp(
+                _optimize(node.op),
+                node.in_axes,
+                node.out_axes,
+                node.input_shapes,
+                node.output_shapes,
+            )
+        elif isinstance(node, Op):
+            new_node = Op(_optimize(node.op), tracable=node.tracable)
+        elif isinstance(node, Input):
+            new_node = node
+        elif isinstance(node, Graph):
+            raise AssertionError("TODO")
+        elif isinstance(node, list):
+            new_node = [_optimize(x) for x in node]
+        elif isinstance(node, tuple):
+            new_node = tuple(_optimize(x) for x in node)
+        elif isinstance(node, dict):
+            new_node = {k: _optimize(v) for k, v in node.items()}
+        else:
+            new_node = node
+
+        new_nodes[id(node)] = new_node
+        return new_node
+
+    new_output = _optimize(output)
+    return new_output
+
+
 class Graph:
     def __init__(self, output, args, kwargs, backend):
-        assert any(isinstance(x, Tracer) for x in einx.tree_util.tree_flatten(output)), f"Expected at least one tracer in output, got {output}"
-        self.output = output
+        assert any(
+            isinstance(x, Tensor) for x in einx.tree_util.tree_flatten(output)
+        ), "No output value is traced"
+        self.output = optimize(output, backend)
         self.args = args
         self.kwargs = kwargs
         self.backend = backend
 
         # Get input tracers
         self.input_tracers = []
         index = 0
+
         def map(x):
             nonlocal index
             if isinstance(x, Input):
                 self.input_tracers.append(x)
                 assert x.index == index
                 index += 1
             return x
+
         einx.tree_util.tree_map(map, args)
         einx.tree_util.tree_map(map, kwargs)
 
         # Generate Python code for the graph
         self.scope = Scope(backend)
         name = self.scope.eval(self)
 
@@ -458,17 +574,14 @@
     def __call__(self, *tracer_values):
         return self.op(*tracer_values)
 
     def __str__(self):
         return str(self.scope)
 
 
-
-
-
 def elementwise(*args, op):
     shape = None
     for a in args:
         if "shape" in dir(a):
             if shape is None:
                 shape = a.shape
             else:
@@ -476,39 +589,44 @@
                 while len(shape) < len(shape2):
                     shape = (1,) + shape
                 while len(shape2) < len(shape):
                     shape2 = (1,) + shape2
                 shape = np.maximum(shape, shape2)
     return OpApplication(op, args=args, output_shapes=shape).output_tracers
 
+
 def reduce(tensor, axis=None, *, op=None, **kwargs):
     keepdims = kwargs.get("keepdims", False)
     if axis is None:
         shape = [1] * len(tensor.shape)
     else:
         axes = [axis] if isinstance(axis, int) else axis
         shape = list(tensor.shape)
         if keepdims:
             for a in axes:
                 shape[a] = 1
         else:
-            for a in reversed(sorted(axes)):
+            for a in sorted(axes, reverse=True):
                 del shape[a]
         kwargs = {**kwargs, **{"axis": axis}}
     return OpApplication(op, args=[tensor], kwargs=kwargs, output_shapes=shape).output_tracers
 
+
 def map(tensor, axis, op, *args, **kwargs):
-    return OpApplication(op, args=[tensor], kwargs={**kwargs, **{"axis": axis}}, output_shapes=tensor.shape).output_tracers
+    return OpApplication(
+        op, args=[tensor], kwargs={**kwargs, **{"axis": axis}}, output_shapes=tensor.shape
+    ).output_tracers
+
 
 def index(tensor, coordinates, update=None, op=None):
     if update is None:
         coordinates2 = (coordinates,) if not isinstance(coordinates, tuple) else coordinates
         if len(coordinates2) > len(tensor.shape):
             raise ValueError(f"Too many indices for tensor of dimension {len(tensor.shape)}")
- 
+
         def is_multidim(c):
             if isinstance(c, (slice, int, np.integer)):
                 return False
             elif isinstance(c, list):
                 return True
             else:
                 return c.ndim > 0
@@ -529,152 +647,174 @@
                         is_front = False
                 else:
                     if isinstance(coordinates2[i], slice):
                         back_slices.append(i)
 
             # Broadcast coordinates expressions
             def broadcast(dims):
-                dims = np.asarray(list(set(int(i) for i in dims)))
+                dims = np.asarray(list({int(i) for i in dims}))
                 assert np.all(dims > 0)
                 if len(dims) > 2 or len(dims) == 2 and np.amin(dims) > 1:
-                    raise ValueError(f"Cannot broadcast coordinates")
+                    raise ValueError("Cannot broadcast coordinates")
                 return np.amax(dims)
+
             shapes = [c.shape for c in coordinates2 if not isinstance(c, slice)]
-            if len(set(len(s) for s in shapes)) != 1:
-                raise ValueError(f"Expected all coordinates to have same number of dimensions")
+            if len({len(s) for s in shapes}) != 1:
+                raise ValueError("Expected all coordinates to have same number of dimensions")
             shapes = np.asarray(shapes)
             shape = [broadcast(shapes[:, i]) for i in range(shapes.shape[1])]
 
             # Prepend and append slices
-            shape = tuple([tensor.shape[i] for i in front_slices] + shape + [tensor.shape[i] for i in back_slices])
+            shape = tuple(
+                [tensor.shape[i] for i in front_slices]
+                + shape
+                + [tensor.shape[i] for i in back_slices]
+            )
         else:
             output_shape = []
             input_shape = tensor.shape
             for s in coordinates:
                 if isinstance(s, (int, np.integer)):
                     input_shape = input_shape[1:]
                 elif isinstance(s, slice):
                     start, stop, step = s.indices(input_shape[0])
                     output_shape.append((stop - start) // step)
                     input_shape = input_shape[1:]
                 elif s is None:
                     output_shape.append(1)
-                elif isinstance(s, Tracer) and s.ndim == 0:
+                elif isinstance(s, Tensor) and s.ndim == 0:
                     input_shape = input_shape[1:]
                 else:
                     raise TypeError(f"Invalid coordinate type: {type(s)}")
             shape = tuple(output_shape) + tuple(input_shape)
 
         return OpApplication(op, args=[tensor, coordinates], output_shapes=shape).output_tracers
     else:
-        return OpApplication(op, args=[tensor, coordinates, update], output_shapes=tensor.shape).output_tracers
+        return OpApplication(
+            op, args=[tensor, coordinates, update], output_shapes=tensor.shape
+        ).output_tracers
+
 
 class tracer(Backend):
     Input = Input
-    OpApplication = OpApplication
     Graph = Graph
 
-    @staticmethod
     def to_tensor(tensor):
-        if isinstance(tensor, OpOutput) and tensor.op.op.op == "to_tensor":
-            # Merge consecutive to_tensor ops
-            return OpApplication("to_tensor", args=[tensor.op.args[0]], output_shapes=tensor.shape).output_tracers
-        if isinstance(tensor, Tracer):
-            return OpApplication("to_tensor", args=[tensor], output_shapes=tensor.shape).output_tracers
-        else:
-            return OpApplication("to_tensor", args=[tensor], output_shapes=einx.param.get_shape(tensor)).output_tracers
+        if isinstance(tensor, Tensor):
+            return OpApplication(
+                "to_tensor", args=[tensor], output_shapes=tensor.shape
+            ).output_tracers
+        else:
+            return OpApplication(
+                "to_tensor", args=[tensor], output_shapes=einx.param.get_shape(tensor)
+            ).output_tracers
 
-    tensor = Tracer
+    tensor = Tensor
     name = "tracer"
 
     def op(op, tracable=False):
         if op is None:
             raise TypeError("op cannot be None")
         if isinstance(op, (Op, VmappedOp)):
             return op
         elif isinstance(op, str):
             return Op(op, tracable=True)
         else:
             return Op(op, tracable=tracable)
 
-    def apply(op, args, kwargs, output_shapes):
-        op = tracer.op(op)
+    @classmethod
+    def apply(backend, op, args, kwargs, output_shapes):
+        op = backend.op(op)
         if op.tracable:
             x = op(*args, **kwargs)
+
+            got_output_shapes = einx.tree_util.tree_map(lambda x: x.shape, x)
+
             def assertion(tensor, shape):
-                assert tuple(tensor.shape) == tuple(shape)
+                if tuple(tensor.shape) != tuple(shape):
+                    raise ValueError(
+                        f"Expected shapes {output_shapes} from custom op, got {got_output_shapes}"
+                    )
+
             einx.tree_util.tree_map(assertion, x, output_shapes)
             return x
         else:
-            return OpApplication(op, args=args, kwargs=kwargs, output_shapes=output_shapes).output_tracers
+            return OpApplication(
+                op, args=args, kwargs=kwargs, output_shapes=output_shapes
+            ).output_tracers
 
     def cast(tensor, dtype):
-        return OpApplication("cast", args=[tensor], kwargs={"dtype": dtype}, output_shapes=tensor.shape).output_tracers
+        return OpApplication(
+            "cast", args=[tensor], kwargs={"dtype": dtype}, output_shapes=tensor.shape
+        ).output_tracers
+
     def reshape(tensor, shape):
-        if tensor.shape == shape:
-            return tensor
-        elif isinstance(tensor, OpOutput) and tensor.op.op == "reshape":
-            # Merge consecutive reshapes
-            return OpApplication("reshape", args=[tensor.op.args[0], shape], output_shapes=shape).output_tracers
-        else:
-            return OpApplication("reshape", args=[tensor, shape], output_shapes=shape).output_tracers
+        return OpApplication("reshape", args=[tensor, shape], output_shapes=shape).output_tracers
 
     def transpose(tensor, perm):
         shape = [tensor.shape[i] for i in perm]
         return OpApplication("transpose", args=[tensor, perm], output_shapes=shape).output_tracers
 
     def broadcast_to(tensor, shape):
-        return OpApplication("broadcast_to", args=[tensor, shape], output_shapes=shape).output_tracers
+        return OpApplication(
+            "broadcast_to", args=[tensor, shape], output_shapes=shape
+        ).output_tracers
 
     def einsum(eq, *tensors):
         exprs = eq.split("->")[0].split(",")
         if len(exprs) != len(tensors):
             raise ValueError(f"Expected {len(exprs)} tensors, got {len(tensors)}")
         values = {}
         for i, (expr, tensor) in enumerate(zip(exprs, tensors)):
             expr = expr.strip().replace(" ", "")
             if len(expr) != len(tensor.shape):
-                raise ValueError(f"Expected {len(expr)} axes, got {len(tensor.shape)} for {i}-th (zero-based) input tensor")
+                raise ValueError(
+                    f"Expected {len(expr)} axes, got {len(tensor.shape)} for {i}-th "
+                    "(zero-based) input tensor"
+                )
             for axis, value in zip(expr, tensor.shape):
                 if axis in values:
                     if values[axis] != value:
-                        raise ValueError(f"Got conflicting values for axis {axis}: {values[axis]} and {value}")
+                        raise ValueError(
+                            f"Got conflicting values for axis {axis}: {values[axis]} and {value}"
+                        )
                 else:
                     values[axis] = value
         expr_out = eq.split("->")[-1].strip().replace(" ", "")
         shape_out = tuple(values[axis] for axis in expr_out)
         return OpApplication("einsum", args=[eq, *tensors], output_shapes=shape_out).output_tracers
 
-    def dot(a, b):
-        raise NotImplementedError()
-
     def swapaxes(a, axis1, axis2):
         shape = list(a.shape)
         shape[axis1], shape[axis2] = shape[axis2], shape[axis1]
         return OpApplication("swapaxes", args=[a, axis1, axis2], output_shapes=shape).output_tracers
 
     def arange(n, dtype="int32"):
-        return OpApplication("arange", args=[n], kwargs={"dtype": dtype}, output_shapes=(n,)).output_tracers
+        return OpApplication(
+            "arange", args=[n], kwargs={"dtype": dtype}, output_shapes=(n,)
+        ).output_tracers
 
     def stack(tensors, axis):
         shape = list(tensors[0].shape)
         shape.insert(axis, len(tensors))
         return OpApplication("stack", args=[tensors, axis], output_shapes=shape).output_tracers
 
     def concatenate(tensors, axis):
         shape = list(tensors[0].shape)
         shape[axis] = sum(tensor.shape[axis] for tensor in tensors)
-        return OpApplication("concatenate", args=[tensors, axis], output_shapes=shape).output_tracers
+        return OpApplication(
+            "concatenate", args=[tensors, axis], output_shapes=shape
+        ).output_tracers
 
     def zeros(shape, dtype="float32"):
         return OpApplication("zeros", args=[shape, dtype], output_shapes=shape).output_tracers
+
     def ones(shape, dtype="float32"):
         return OpApplication("ones", args=[shape, dtype], output_shapes=shape).output_tracers
 
-
     add = partial(elementwise, op="add")
     subtract = partial(elementwise, op="subtract")
     multiply = partial(elementwise, op="multiply")
     true_divide = partial(elementwise, op="true_divide")
     floor_divide = partial(elementwise, op="floor_divide")
     divide = partial(elementwise, op="divide")
     logical_and = partial(elementwise, op="logical_and")
@@ -709,21 +849,25 @@
     flip = partial(map, op="flip")
     roll = partial(map, op="roll")
     softmax = partial(map, op="softmax")
     log_softmax = partial(map, op="log_softmax")
 
     def sqrt(tensor):
         return OpApplication("sqrt", args=[tensor], output_shapes=tensor.shape).output_tracers
+
     def rsqrt(tensor):
         return OpApplication("rsqrt", args=[tensor], output_shapes=tensor.shape).output_tracers
+
     def square(tensor):
         return OpApplication("square", args=[tensor], output_shapes=tensor.shape).output_tracers
 
     def allclose(a, b):
         return OpApplication("allclose", args=[a, b], shape=()).output_tracers
 
     def vmap(op, in_axes, out_axes, input_shapes, output_shapes):
         return VmappedOp(op, in_axes, out_axes, input_shapes, output_shapes)
 
     class random:
         def bernoulli(rng, p, shape):
-            return OpApplication("random.bernoulli", args=[rng, p, shape], output_shapes=shape).output_tracers
+            return OpApplication(
+                "random.bernoulli", args=[rng, p, shape], output_shapes=shape
+            ).output_tracers
```

### Comparing `einx-0.1.3/einx/expr/solver.py` & `einx-0.2.0/einx/expr/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import sympy, math
+import sympy
+import math
+
 
 class Expression:
     def __init__(self):
         pass
 
     def __add__(self, other):
         return Sum([self, other])
@@ -12,14 +14,15 @@
 
     def __mul__(self, other):
         return Product([self, other])
 
     def __rmul__(self, other):
         return Product([other, self])
 
+
 class Variable(Expression):
     def __init__(self, id, name):
         Expression.__init__(self)
         self.id = id
         self.name = name
 
     def __iter__(self):
@@ -33,14 +36,15 @@
 
     def __str__(self):
         return f"{self.name}"
 
     def sympy(self):
         return sympy.Symbol(self.id)
 
+
 class Constant(Expression):
     def __init__(self, value):
         Expression.__init__(self)
         self.value = value
 
     def __iter__(self):
         yield self
@@ -53,14 +57,15 @@
 
     def __str__(self):
         return str(self.value)
 
     def sympy(self):
         return self.value
 
+
 class Sum(Expression):
     @staticmethod
     def maybe(children):
         if len(children) == 0:
             return Constant(0)
         elif len(children) == 1:
             return children[0]
@@ -86,14 +91,15 @@
 
     def __str__(self):
         return " + ".join(str(c) for c in self.children)
 
     def sympy(self):
         return sum([c.sympy() for c in self.children])
 
+
 class Product(Expression):
     @staticmethod
     def maybe(children):
         if len(children) == 0:
             return Constant(1)
         elif len(children) == 1:
             return children[0]
@@ -119,103 +125,129 @@
 
     def __str__(self):
         return " * ".join(str(c) for c in self.children)
 
     def sympy(self):
         return math.prod([c.sympy() for c in self.children])
 
+
 def to_term(x):
     if isinstance(x, int):
         return Constant(x)
     else:
         if not isinstance(x, Expression):
-            raise TypeError('Expected Expression, got {}'.format(type(x)))
+            raise TypeError(f"Expected Expression, got {type(x)}")
         return x
 
+
 class SolveException(Exception):
     def __init__(self, message):
         self.message = message
 
+
 def solve(equations):
     equations = [(to_term(t1), to_term(t2)) for t1, t2 in equations]
     equations = [(t1, t2) for t1, t2 in equations if t1 != t2]
     equations = list(set(equations))
-    variables = {v.id: v for terms in equations for term in terms for v in term if isinstance(v, Variable)}
+    variables = {
+        v.id: v for terms in equations for term in terms for v in term if isinstance(v, Variable)
+    }
 
-    ##### Find equivalence classes of variables to speed up sympy solver #####
+    # Find equivalence classes of variables to speed up sympy solver #####
     # Find constant definitions
-    constants = {} # id: constant value
+    constants = {}  # id: constant value
     for t1, t2 in equations:
         if isinstance(t1, Variable) and isinstance(t2, Constant):
             if constants.get(t1.id, t2.value) != t2.value:
-                raise SolveException(f"Found contradictory values {set([constants[t1.id], t2.value])} for expression '{t1.name}'")
+                raise SolveException(
+                    f"Found contradictory values { {constants[t1.id], t2.value} } for "
+                    f"expression '{t1.name}'"
+                )
             constants[t1.id] = t2.value
         elif isinstance(t1, Constant) and isinstance(t2, Variable):
             if constants.get(t2.id, t1.value) != t1.value:
-                raise SolveException(f"Found contradictory values {set([constants[t2.id], t1.value])} for expression '{t2.name}'")
+                raise SolveException(
+                    f"Found contradictory values { {constants[t2.id], t1.value} } for "
+                    f"expression '{t2.name}'"
+                )
             constants[t2.id] = t1.value
         elif isinstance(t1, Constant) and isinstance(t2, Constant):
             if t1.value != t2.value:
-                raise SolveException(f"Found contradictory values {t1.value} != {t2.value} in input equation")
+                raise SolveException(
+                    f"Found contradictory values {t1.value} != {t2.value} in input equation"
+                )
 
     # Find equivalence classes of variables
-    classes = {v: set([v]) for v in variables} # id: set of equivalent ids
+    classes = {v: {v} for v in variables}  # id: set of equivalent ids
     for t1, t2 in equations:
         if isinstance(t1, Variable) and isinstance(t2, Variable):
             assert t1.id in classes and t2.id in classes
             set1 = classes[t1.id]
             set2 = classes[t2.id]
             for t_id in set2:
                 classes[t_id] = set1
                 set1.add(t_id)
 
     # For every class: Use constant if it exists, or create single class variable
-    origvar_to_solvevar = {} # id: Variable or Constant
+    origvar_to_solvevar = {}  # id: Variable or Constant
     for eclass in {id(s): s for s in classes.values()}.values():
         if any(n in constants for n in eclass):
             # Use constant
-            class_constants = set(constants[n] for n in eclass if n in constants)
+            class_constants = {constants[n] for n in eclass if n in constants}
             if len(class_constants) != 1:
-                names = set(variables[a].name for a in eclass)
+                names = {variables[a].name for a in eclass}
                 if len(names) == 1:
-                    raise SolveException(f"Found contradictory values {class_constants} for expression '{next(iter(names))}'")
+                    raise SolveException(
+                        f"Found contradictory values {class_constants} for expression "
+                        f"'{next(iter(names))}'"
+                    )
                 else:
-                    raise SolveException(f"Found contradictory values {class_constants} for equivalent expressions {names}")
+                    raise SolveException(
+                        f"Found contradictory values {class_constants} for equivalent "
+                        f"expressions {names}"
+                    )
             v = Constant(next(iter(class_constants)))
         else:
             # Create new variable for class
-            v = Variable(f"Class-{id(eclass)}", f"Equivalent expressions {set(variables[a].name for a in eclass)}")
+            v = Variable(
+                f"Class-{id(eclass)}",
+                f"Equivalent expressions { {variables[a].name for a in eclass} }",
+            )
         for n in eclass:
-            assert not n in origvar_to_solvevar
+            assert n not in origvar_to_solvevar
             origvar_to_solvevar[n] = v
 
     # Apply to equations
     def replace(t):
         if isinstance(t, Variable) and t.id in origvar_to_solvevar:
             return origvar_to_solvevar[t.id]
         elif isinstance(t, Constant):
             return t
         elif isinstance(t, Sum):
             return Sum.maybe([replace(c) for c in t.children])
         elif isinstance(t, Product):
             return Product.maybe([replace(c) for c in t.children])
         else:
-            assert False
+            raise AssertionError()
+
     equations2 = []
     for t1o, t2o in equations:
         t1 = replace(t1o)
         t2 = replace(t2o)
         if isinstance(t1, Constant) and isinstance(t2, Constant):
             if t1.value != t2.value:
-                raise SolveException(f"Found contradictory values {t1.value} != {t2.value} for same equivalence class")
+                raise SolveException(
+                    f"Found contradictory values {t1.value} != {t2.value} "
+                    "for same equivalence class"
+                )
         elif t1 != t2:
             equations2.append((t1, t2))
     equations = equations2
 
-    ##### Solve remaining equations using sympy #####
+    # Solve remaining equations using sympy #####
     solutions = {}
     if len(equations) > 0:
         sympy_equations = [sympy.Eq(t1.sympy(), t2.sympy()) for t1, t2 in equations]
 
         if all(eq.is_Boolean and bool(eq) for eq in sympy_equations):
             solutions = {}
         else:
@@ -226,23 +258,25 @@
                 variables, solutions = solutions
                 if len(solutions) == 0:
                     raise SolveException("Sympy returned no solutions")
                 elif len(solutions) > 1:
                     raise SolveException("Sympy returned multiple possible solutions")
                 else:
                     solutions = next(iter(solutions))
-                    solutions = {str(k): int(v) for k, v in zip(variables, solutions) if v.is_number}
+                    solutions = {
+                        str(k): int(v) for k, v in zip(variables, solutions) if v.is_number
+                    }
             else:
                 raise SolveException("Sympy returned unexpected result")
 
     # Determine values for original variables in equivalence classes
     orig_solutions = {}
     for k, v in origvar_to_solvevar.items():
         if isinstance(v, Constant):
             orig_solutions[k] = v.value
         elif isinstance(v, Variable):
             if v.id in solutions:
                 orig_solutions[k] = solutions[v.id]
         else:
-            assert False
+            raise AssertionError()
 
-    return orig_solutions
+    return orig_solutions
```

### Comparing `einx-0.1.3/einx/expr/stage1.py` & `einx-0.2.0/einx/expr/stage3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,454 +1,373 @@
-from collections import defaultdict
-import re, uuid
+from . import stage2, solver
+import numpy as np
+from functools import partial
+import einx
+
 
 class Expression:
-    def __init__(self, begin_pos, end_pos):
-        self.begin_pos = begin_pos
-        self.end_pos = end_pos
+    def __init__(self, value):
+        if not isinstance(value, (int, np.int64, np.int32, np.int16, np.int8)):
+            raise TypeError(f"Expected int, got {type(value)}")
+        self.value = int(value)
         self.parent = None
 
     @property
-    def depth(self):
-        if self.parent is None:
-            return 0
-        elif isinstance(self.parent, Ellipsis):
-            return 1 + self.parent.depth
-        else:
-            return self.parent.depth
+    def shape(self):
+        return tuple(x.value for x in self)
+
 
 class Composition(Expression):
-    def __init__(self, inner, begin_pos=-1, end_pos=-1):
-        Expression.__init__(self, begin_pos, end_pos)
-        self.inner = inner
-        self.inner.parent = self
+    @staticmethod
+    def maybe(inner):
+        if len(inner) == 0:
+            return Axis(None, 1)
+        elif isinstance(inner, list):
+            if len(inner) == 1:
+                return inner[0]
+            else:
+                return Composition(List.maybe(inner))
+        elif isinstance(inner, List) and len(inner) == 1:
+            return inner.children[0]
+        else:
+            return Composition(inner)
 
-    def all(self):
-        yield self
-        yield from self.inner.all()
+    def __init__(self, inner):
+        Expression.__init__(self, inner.value)
+        self.inner = inner
+        inner.parent = self
+        assert len(inner) > 0
 
     def __str__(self):
-        return "(" + str(self.inner) + ")"
+        return f"({self.inner})"
 
-    def __deepcopy__(self):
-        return Composition(self.inner.__deepcopy__(), self.begin_pos, self.end_pos)
-
-    def expansion(self):
+    def __len__(self):
         return 1
 
-    @property
-    def direct_children(self):
-        yield self.inner
+    def __iter__(self):
+        yield self
 
-class Marker(Expression):
-    def __init__(self, inner, begin_pos=-1, end_pos=-1):
-        Expression.__init__(self, begin_pos, end_pos)
-        self.inner = inner
-        self.inner.parent = self
+    def __deepcopy__(self):
+        return Composition(self.inner.__deepcopy__())
+
+    def __eq__(self, other):
+        return isinstance(other, Composition) and self.inner == other.inner
+
+    def __hash__(self):
+        return 8716123 + hash(self.inner)
 
     def all(self):
         yield self
         yield from self.inner.all()
 
-    def __str__(self):
-        return "[" + str(self.inner) + "]"
 
-    def __deepcopy__(self):
-        return Marker(self.inner.__deepcopy__(), self.begin_pos, self.end_pos)
+class List(Expression):
+    def maybe(l, *args, **kwargs):
+        if not isinstance(l, list):
+            raise TypeError(f"Expected list, got {type(l)}")
+        if len(l) == 1:
+            return l[0]
+        else:
+            return List(l, *args, **kwargs)
 
-    def expansion(self):
-        return self.inner.expansion()
+    def __init__(self, children):
+        Expression.__init__(self, np.prod([c.value for c in children]).astype(int))
+        self.children = children
+        for c in children:
+            if isinstance(c, List):
+                raise ValueError("List cannot have another List as direct child")
+            c.parent = self
 
-    @property
-    def direct_children(self):
-        yield self.inner
+    def __str__(self):
+        return " ".join([str(c) for c in self.children])
 
-class NamedAxis(Expression):
-    def __init__(self, name, begin_pos=-1, end_pos=-1):
-        Expression.__init__(self, begin_pos, end_pos)
-        self.name = name
+    def __getitem__(self, i):
+        return self.children[i]
 
-    def all(self):
-        yield self
+    def __len__(self):
+        return sum(len(c) for c in self.children)
 
-    def __str__(self):
-        return self.name
+    def __iter__(self):
+        for c in self.children:
+            yield from c
 
     def __deepcopy__(self):
-        return NamedAxis(self.name, self.begin_pos, self.end_pos)
-
-    def expansion(self):
-        return 1
+        return List([c.__deepcopy__() for c in self.children])
 
-    @property
-    def direct_children(self):
-        yield from ()
+    def __eq__(self, other):
+        return isinstance(other, List) and self.children == other.children
 
-class UnnamedAxis(Expression):
-    def __init__(self, value, begin_pos=-1, end_pos=-1):
-        Expression.__init__(self, begin_pos, end_pos)
-        self.value = value
+    def __hash__(self):
+        return 6563 + hash(tuple(self.children))
 
     def all(self):
         yield self
+        for c in self.children:
+            yield from c.all()
 
-    def __str__(self):
-        return str(self.value)
 
-    def __deepcopy__(self):
-        return UnnamedAxis(self.value, self.begin_pos, self.end_pos)
-
-    def expansion(self):
-        return 1
+class Axis(Expression):
+    def __init__(self, name, value):
+        Expression.__init__(self, value)
+        self.name = name if name is not None else f"unnamed.{id(self)}"
 
-    @property
-    def direct_children(self):
-        yield from ()
+    def __repr__(self):
+        return f"Axis({self.name}, {self.value})"
 
-class Ellipsis(Expression):
-    anonymous_variable_name = "_anonymous_ellipsis_axis"
+    def __str__(self):
+        return self.name if not self.is_unnamed else str(self.value)
 
-    def __init__(self, inner, begin_pos=-1, end_pos=-1, ellipsis_id=None):
-        Expression.__init__(self, begin_pos, end_pos)
-        self.inner = inner
-        self.inner.parent = self
-        self.ellipsis_id = uuid.uuid4().int if ellipsis_id is None else ellipsis_id
+    def __len__(self):
+        return 1
 
-    def all(self):
+    def __iter__(self):
         yield self
-        yield from self.inner.all()
-
-    def __str__(self):
-        n = str(self.inner)
-        if isinstance(self.inner, List) and len(self.inner.children) > 1:
-            n = "{" + n + "}"
-        return n + _ellipsis
 
     def __deepcopy__(self):
-        return Ellipsis(self.inner.__deepcopy__(), self.begin_pos, self.end_pos, self.ellipsis_id)
+        return Axis(self.name, self.value)
 
-    def expansion(self):
-        if self.inner.expansion() == 0:
-            return 0
+    def __eq__(self, other):
+        if not isinstance(other, Axis):
+            return False
+        if self.is_unnamed != other.is_unnamed:
+            return False
+        if self.value != other.value:
+            return False
+        if self.is_unnamed:
+            return True
         else:
-            return None
+            return self.name == other.name
 
-    @property
-    def direct_children(self):
-        yield self.inner
-
-class Concatenation(Expression):
-    def maybe(l, *args, **kwargs):
-        if len(l) == 1:
-            return l[0]
-        else:
-            return Concatenation(l, *args, **kwargs)
-
-    def __init__(self, children, begin_pos=-1, end_pos=-1):
-        Expression.__init__(self, begin_pos, end_pos)
-        self.children = children
-        for child in self.children:
-            child.parent = self
+    def __hash__(self):
+        return 9817234 + (hash(self.name) if not self.is_unnamed else 0) + hash(self.value)
 
     def all(self):
         yield self
-        for child in self.children:
-            yield from child.all()
-
-    def __str__(self):
-        return f" + ".join([str(c) for c in self.children])
-
-    def __deepcopy__(self):
-        return Concatenation([c.__deepcopy__() for c in self.children], self.begin_pos, self.end_pos)
-
-    def expansion(self):
-        return 1
 
     @property
-    def direct_children(self):
-        yield from self.children
+    def is_unnamed(self):
+        return self.name.startswith("unnamed.")
 
-class List(Expression):
+
+class Concatenation(Expression):
     @staticmethod
     def maybe(l, *args, **kwargs):
+        if not isinstance(l, list):
+            raise TypeError(f"Expected list, got {type(l)}")
         if len(l) == 1:
             return l[0]
         else:
-            return List(l, *args, **kwargs)
+            return Concatenation(l, *args, **kwargs)
 
-    def __init__(self, children, begin_pos=-1, end_pos=-1):
-        Expression.__init__(self, begin_pos, end_pos)
+    def __init__(self, children):
+        if len(children) == 0:
+            raise ValueError("Concatenation must have at least one child")
+        Expression.__init__(self, np.sum([c.value for c in children]).astype("int32"))
         self.children = children
-        for child in self.children:
-            child.parent = self
-
-    def all(self):
-        yield self
-        for child in self.children:
-            yield from child.all()
+        for c in children:
+            if len(c) != 1:
+                raise ValueError(
+                    "Concatenation can only be used on expressions of length 1, but"
+                    f"got expression '{c}'"
+                )
+            c.parent = self
 
     def __str__(self):
-        return f" ".join([str(c) for c in self.children])
-
-    def __deepcopy__(self):
-        return List([c.__deepcopy__() for c in self.children], self.begin_pos, self.end_pos)
-
-    def expansion(self):
-        child_expansions = [c.expansion() for c in self.children]
-        if any(e is None for e in child_expansions):
-            return None
-        else:
-            return sum(child_expansions)
+        return "+".join([str(c) for c in self.children])
 
-    @property
-    def direct_children(self):
-        yield from self.children
-
-class Choice(Expression):
-    def __init__(self, children, begin_pos=-1, end_pos=-1):
-        Expression.__init__(self, begin_pos, end_pos)
-        self.children = children
-        for child in self.children:
-            child.parent = self
+    def __len__(self):
+        return 1
 
-    def all(self):
+    def __iter__(self):
         yield self
-        for child in self.children:
-            yield from child.all()
-
-    def __str__(self):
-        return f" | ".join([str(c) for c in self.children])
 
     def __deepcopy__(self):
-        return Choice([c.__deepcopy__() for c in self.children], self.begin_pos, self.end_pos)
-
-    def expansion(self):
-        child_expansions = set(c.expansion() for c in self.children)
-        if len(child_expansions) == 1:
-            return child_expansions.pop()
-        else:
-            return None
-
-    @property
-    def direct_children(self):
-        yield from self.children
+        return Concatenation([c.__deepcopy__() for c in self.children])
 
+    def __eq__(self, other):
+        return isinstance(other, Concatenation) and self.children == other.children
 
+    def __hash__(self):
+        return 123 + hash(tuple(self.children))
 
-class Token:
-    def __init__(self, pos, text):
-        self.begin_pos = pos
-        self.end_pos = pos + len(text) 
-        self.text = text
-
-    def __str__(self):
-        return self.text
+    def all(self):
+        yield self
+        for c in self.children:
+            yield from c.all()
 
-    def __repr__(self):
-        return f"Token(\"{self.text}\")"
 
-class ParseError(Exception):
-    def __init__(self, expression, pos, message):
-        self.expression = expression
-        self.pos = pos
-        self.message = message
-        assert self.pos >= 0 and self.pos < len(self.expression)
+class Marker(Expression):
+    def __init__(self, inner):
+        if len(inner) == 0:
+            raise ValueError("Marker cannot have empty list as child")
+        Expression.__init__(self, inner.value)
+        self.inner = inner
+        inner.parent = self
 
     def __str__(self):
-        return self.message + "\nHere: " + self.expression + "\n" + " " * (self.pos + 6) + "^"
+        return f"[{self.inner}]"
 
-_parentheses = {
-    "(": ")",
-    "[": "]",
-}
-_parentheses_front = set(_parentheses.keys())
-_parentheses_back = set(_parentheses.values())
-_disallowed_literals = [",", "->", "\t", "\n", "\r"]
-_nary_ops = ["|", " ", "+"]
-_ellipsis = "..."
-_axis_name = r"[a-zA-Z_][a-zA-Z0-9_]*"
-_literals = _nary_ops + list(_parentheses_front) + list(_parentheses_back) + [_ellipsis]
-
-def parse(text):
-    text = text.strip()
-    for x in _nary_ops:
-        while f" {x}" in text:
-            text = text.replace(f" {x}", x)
-        while f"{x} " in text:
-            text = text.replace(f"{x} ", x)
-    
-
-
-    # Lexer
-    tokens = []
-    start_pos = 0
-    def next_token(end_pos):
-        nonlocal start_pos
-        if start_pos != end_pos:
-            tokens.append(Token(start_pos, text[start_pos:end_pos]))
-            start_pos = end_pos
-
-    pos = 0
-    while pos < len(text):
-        for d in _disallowed_literals:
-            if text[pos:].startswith(d):
-                raise ParseError(text, pos, f"Found disallowed literal '{d}'")
-        for l in _literals:
-            if text[pos:].startswith(l):
-                next_token(pos)
-                next_token(pos + len(l))
-                pos += len(l)
-                break
-        else:
-            pos += 1
-    next_token(pos)
+    def __len__(self):
+        return len(self.inner)
 
-    # Parser
-    def parse(in_tokens, begin_pos):
-        assert isinstance(in_tokens, list)
-        if len(in_tokens) == 0:
-            return List([], begin_pos, begin_pos)
-
-        # Parentheses
-        if isinstance(in_tokens[0], Token) and in_tokens[0].text in _parentheses_front:
-            assert len(in_tokens) >= 2 and isinstance(in_tokens[-1], Token) and in_tokens[-1].text in _parentheses_back
-            if in_tokens[0].text == "(":
-                op = Composition
-            elif in_tokens[0].text == "[":
-                op = Marker
-            else:
-                assert False
-            return op(parse(in_tokens[1:-1], in_tokens[1].begin_pos), in_tokens[0].begin_pos, in_tokens[-1].end_pos)
+    def __iter__(self):
+        yield from self.inner
 
-        # N-ary operators
-        for nary_op in _nary_ops:
-            if any(isinstance(t, Token) and t.text == nary_op for t in in_tokens):
-                out_tokens = []
-                current_tokens = []
-                allow_empty_operands = nary_op != " "
-                for token in in_tokens:
-                    if isinstance(token, Token) and token.text == nary_op:
-                        if allow_empty_operands or len(current_tokens) > 0:
-                            out_tokens.append(parse(current_tokens, current_tokens[0].begin_pos if len(current_tokens) > 0 else token.begin_pos))
-                        current_tokens = []
-                    else:
-                        current_tokens.append(token)
-                if allow_empty_operands or len(current_tokens) > 0:
-                    out_tokens.append(parse(current_tokens, current_tokens[0].begin_pos if len(current_tokens) > 0 else token.begin_pos))
-
-                if nary_op == " ":
-                    op = List
-                elif nary_op == "|":
-                    op = Choice
-                elif nary_op == "+":
-                    op = Concatenation
-                else:
-                    assert False
-                return op(out_tokens, in_tokens[0].begin_pos, in_tokens[-1].end_pos)
-
-        # Ellipsis
-        if isinstance(in_tokens[-1], Token) and in_tokens[-1].text == _ellipsis:
-            if len(in_tokens) == 1:
-                return Ellipsis(NamedAxis(Ellipsis.anonymous_variable_name, in_tokens[0].begin_pos, in_tokens[0].begin_pos), in_tokens[0].begin_pos, in_tokens[0].end_pos)
-            else:
-                assert len(in_tokens) == 2
-                return Ellipsis(parse(in_tokens[:-1], in_tokens[0].begin_pos), in_tokens[0].begin_pos, in_tokens[1].end_pos)
+    def __deepcopy__(self):
+        return Marker(self.inner.__deepcopy__())
 
-        # Axis
-        if len(in_tokens) == 1 and isinstance(in_tokens[0], Token):
-            value = in_tokens[0].text.strip()
-            if value.isdigit():
-                return UnnamedAxis(int(value), in_tokens[0].begin_pos, in_tokens[0].end_pos)
-            else:
-                if not re.fullmatch(_axis_name, in_tokens[0].text):
-                    raise ParseError(text, in_tokens[0].begin_pos, f"Invalid axis name '{in_tokens[0].text}'")
-                return NamedAxis(value, in_tokens[0].begin_pos, in_tokens[0].end_pos)
-
-        if len(in_tokens) == 1:
-            return in_tokens[0]
-
-        assert False
-
-    stack = [[]]
-    for token in tokens:
-        if token.text in _parentheses_front:
-            stack.append([])
-            stack[-1].append(token)
-        elif token.text in _parentheses_back:
-            if len(stack) == 1 or _parentheses[stack[-1][0].text] != token.text:
-                raise ParseError(text, token.begin_pos, f"Unexpected closing parenthesis '{token.text}'")
-            stack[-1].append(token)
-            group = stack.pop()
-            stack[-1].append(parse(group, group[0].begin_pos))
-        else:
-            stack[-1].append(token)
-    if len(stack) > 1:
-        raise ParseError(text, stack[-1][0].begin_pos, f"Unclosed parenthesis '{stack[-1][0].text}'")
-    expression = parse(stack[0], 0)
-
-    # Semantic check: Choice must be inside marker
-    for expr in expression.all():
-        if isinstance(expr, Choice) and (expr.parent is None or not isinstance(expr.parent, Marker)):
-            raise ParseError(text, expr.begin_pos, "Choice with | can only appear inside a [] marker")
-
-    # Semantic check: Choices must have same number of options
-    num = None
-    for expr in expression.all():
-        if isinstance(expr, Choice):
-            n = len(expr.children)
-            if num is None:
-                num = n
-            elif num != n:
-                raise ParseError(text, expr.begin_pos, "Choices must have the same number of options")
-
-    # Semantic check: Axis names can only be used once per expression
-    def traverse(expr, key, axes_by_key):
-        if isinstance(expr, list):
-            for expr in expr:
-                traverse(expr, key, axes_by_key)
-        elif isinstance(expr, NamedAxis):
-            axes_by_key[(key + (expr.name,))].append(expr)
-        elif isinstance(expr, UnnamedAxis):
-            pass
-        elif isinstance(expr, Composition):
-            traverse(expr.inner, key, axes_by_key)
-        elif isinstance(expr, List):
-            traverse(expr.children, key, axes_by_key)
-        elif isinstance(expr, Concatenation):
-            for i, c in enumerate(expr.children):
-                traverse(c, key + ((id(expr), i),), axes_by_key)
-        elif isinstance(expr, Choice):
-            assert False
-        elif isinstance(expr, Marker):
-            traverse(expr.inner, key, axes_by_key)
-        elif isinstance(expr, Ellipsis):
-            traverse(expr.inner, key, axes_by_key)
-        else:
-            raise TypeError(f"Invalid expression type {type(expr)}")
+    def __eq__(self, other):
+        return isinstance(other, Marker) and self.inner == other.inner
 
-    def check(root):
-        axes_by_key = defaultdict(list)
-        traverse(root, (), axes_by_key)
-        for key in list(axes_by_key.keys()):
-            exprs = []
-            for i in range(len(key) + 1):
-                exprs.extend(axes_by_key[key[:i]])
-            if len(exprs) > 1:
-                raise ParseError(text, exprs[1].begin_pos, f"Axis name '{exprs[0].name}' is used more than once in expression '{root}'")
-    if num is None:
-        check(expression)
-    else:
-        for i in range(num):
-            check(choose(expression, i, num))
+    def __hash__(self):
+        return 6433236 + hash(self.inner)
 
-    return expression
+    def all(self):
+        yield self
+        yield from self.inner.all()
 
 
+class SolveValueException(Exception):
+    def __init__(self, exprs1, exprs2, message):
+        self.exprs1 = exprs1
+        self.exprs2 = exprs2
+        self.message = f"Failed to solve values of expressions. {message}\nInput:\n"
+        for expr1, expr2 in zip(exprs1, exprs2):
+            self.message += (
+                f"    '{einx.expr.util._to_str(expr1)} = {einx.expr.util._to_str(expr2)}'\n"
+            )
+        super().__init__(self.message)
+
+
+def solve(exprs1, exprs2):
+    exprs1 = list(exprs1)
+    exprs2 = list(exprs2)
+    if any(
+        expr is not None and not isinstance(expr, stage2.Expression) for expr in exprs1 + exprs2
+    ):
+        raise ValueError("Can only expand stage2.Expression")
+    if len(exprs1) != len(exprs2):
+        raise ValueError("Number of expressions must be equal")
+
+    equations = []
+
+    symbolic_expr_values = {}
+    for root in exprs1 + exprs2:
+        if root is not None:
+            for expr in root.all():
+                symbolic_expr_values[id(expr)] = solver.Variable(
+                    f"symbolic_expr_values[{id(expr)}]", str(expr)
+                )
+
+    # Add equations: Relations between expressions and their children
+    for root in exprs1 + exprs2:
+        if root is not None:
+            for expr in root.all():
+                if isinstance(expr, stage2.List):
+                    equations.append((
+                        solver.Product([symbolic_expr_values[id(c)] for c in expr.children]),
+                        symbolic_expr_values[id(expr)],
+                    ))
+                elif isinstance(expr, stage2.Concatenation):
+                    equations.append((
+                        solver.Sum([symbolic_expr_values[id(c)] for c in expr.children]),
+                        symbolic_expr_values[id(expr)],
+                    ))
+                elif isinstance(expr, stage2.Marker) or isinstance(expr, stage2.Composition):
+                    equations.append((
+                        symbolic_expr_values[id(expr)],
+                        symbolic_expr_values[id(expr.inner)],
+                    ))
+
+    # Add equations: Same root values
+    for root1, root2 in zip(exprs1, exprs2):
+        if root1 is not None and root2 is not None:
+            assert len(root1) == len(root2)
+            for expr1, expr2 in zip(root1, root2):
+                equations.append((
+                    symbolic_expr_values[id(expr1)],
+                    symbolic_expr_values[id(expr2)],
+                ))
+
+    # Add equations: Unnamed axes
+    for root in exprs1 + exprs2:
+        if root is not None:
+            for expr in root.all():
+                if isinstance(expr, stage2.UnnamedAxis):
+                    equations.append((
+                        symbolic_expr_values[id(expr)],
+                        int(expr.value),
+                    ))
+
+    # Add equations: Multiple occurrences of the same named axis must have the same value
+    sympy_axis_values = {}
+    for root in exprs1 + exprs2:
+        if root is not None:
+            for axis in root.all():
+                if isinstance(axis, stage2.NamedAxis):
+                    if axis.name not in sympy_axis_values:
+                        sympy_axis_values[axis.name] = solver.Variable(
+                            f"sympy_axis_values[{axis.name}]", axis.name
+                        )
+                    equations.append((
+                        symbolic_expr_values[id(axis)],
+                        sympy_axis_values[axis.name],
+                    ))
+
+    # Solve
+    try:
+        solutions = solver.solve(equations)
+    except solver.SolveException as e:
+        raise SolveValueException(exprs1, exprs2, str(e)) from e
+    axis_values = {}
+    for k, v in solutions.items():
+        if k.startswith("symbolic_expr_values["):
+            axis_values[int(k[len("symbolic_expr_values[") : -1])] = int(v)
+
+    failed_axes = set()
+    for root in exprs1 + exprs2:
+        if root is not None:
+            for expr in root.all():
+                if isinstance(expr, stage2.NamedAxis):
+                    if id(expr) not in axis_values:
+                        failed_axes.add(str(expr))
+    if len(failed_axes) > 0:
+        raise SolveValueException(exprs1, exprs2, f"Found no unique solutions for {failed_axes}")
+
+    # Map stage2 expressions to stage3 expressions
+    def map(expr):
+        if isinstance(expr, stage2.NamedAxis):
+            assert id(expr) in axis_values
+            if axis_values[id(expr)] <= 0:
+                raise SolveValueException(
+                    exprs1, exprs2, f"Axis '{expr}' has value {axis_values[id(expr)]} <= 0"
+                )
+            return Axis(expr.name, axis_values[id(expr)])
+        elif isinstance(expr, stage2.UnnamedAxis):
+            assert id(expr) in axis_values
+            if axis_values[id(expr)] <= 0:
+                raise SolveValueException(
+                    exprs1, exprs2, f"Axis '{expr}' has value {axis_values[id(expr)]} <= 0"
+                )
+            return Axis(None, axis_values[id(expr)])
+        elif isinstance(expr, stage2.List):
+            return List([map(child) for child in expr.children])
+        elif isinstance(expr, stage2.Concatenation):
+            return Concatenation([map(child) for child in expr.children])
+        elif isinstance(expr, stage2.Marker):
+            return Marker(map(expr.inner))
+        elif isinstance(expr, stage2.Composition):
+            return Composition.maybe(map(expr.inner))
+        else:
+            raise AssertionError(type(expr))
 
+    exprs1 = [map(root) if root is not None else None for root in exprs1]
+    exprs2 = [map(root) if root is not None else None for root in exprs2]
 
+    return exprs1, exprs2
 
 
 def expr_map(f):
     def outer(expr, *args, **kwargs):
         # Wrap the user function to return a list of expressions
         def f2(expr):
             t = f(expr, *args, **kwargs)
@@ -460,125 +379,159 @@
                 return expr, signal
             if isinstance(expr, List):
                 return expr.children, signal
             elif isinstance(expr, Expression):
                 return [expr], signal
             else:
                 raise TypeError(f"Invalid return type {type(expr)}")
+
         return List.maybe(_expr_map(expr, f2))
+
     return outer
 
+
 expr_map.CONTINUE = 1
 expr_map.COPY_AND_STOP = 2
 expr_map.REPLACE_AND_STOP = 3
 expr_map.REPLACE_AND_CONTINUE = 4
 
+
 def _expr_map(expr, f):
     exprs, signal = f(expr)
     if signal == expr_map.REPLACE_AND_STOP:
         assert isinstance(exprs, list)
         return exprs
     elif signal == expr_map.COPY_AND_STOP:
         return [expr.__deepcopy__()]
     elif signal == expr_map.REPLACE_AND_CONTINUE:
         return [c for expr in exprs for c in _expr_map(expr, f)]
 
-    if isinstance(expr, NamedAxis):
-        return [expr.__deepcopy__()]
-    elif isinstance(expr, UnnamedAxis):
+    if isinstance(expr, Axis):
         return [expr.__deepcopy__()]
     elif isinstance(expr, Composition):
-        return [Composition(List.maybe(_expr_map(expr.inner, f)))]
+        return [Composition.maybe(List.maybe(_expr_map(expr.inner, f)))]
     elif isinstance(expr, List):
         return [c2 for c1 in expr.children for c2 in _expr_map(c1, f)]
     elif isinstance(expr, Concatenation):
-        return [Concatenation([List.maybe(_expr_map(c, f)) for c in expr.children])]
-    elif isinstance(expr, Choice):
-        return [Choice([List.maybe(_expr_map(c, f)) for c in expr.children])]
+        children = [List.maybe(_expr_map(c, f)) for c in expr.children]
+        children = [c if len(c) > 0 else Axis(None, 1) for c in children]
+        return [Concatenation(children)]
     elif isinstance(expr, Marker):
         x = _expr_map(expr.inner, f)
         if len(x) == 0:
             # Drop empty marker
             return []
         else:
             return [Marker(List.maybe(x))]
-    elif isinstance(expr, Ellipsis):
-        return [Ellipsis(List.maybe(_expr_map(expr.inner, f)), ellipsis_id=expr.ellipsis_id)]
     else:
         raise TypeError(f"Invalid expression type {type(expr)}")
 
 
-
 @expr_map
-def _choose(expr, index, num):
-    if isinstance(expr, Choice):
-        if len(expr.children) != num:
-            raise ValueError(f"Expected choice with {num} choices, got {len(expr.children)}")
-        return [expr.children[index]], expr_map.REPLACE_AND_CONTINUE
-
-def choose(expr, index, num):
-    if not any(isinstance(expr, Choice) for expr in expr.all()):
-        raise ValueError("Expression does not contain any choices")
-    return _choose(expr, index, num)
+def decompose(expr):
+    if isinstance(expr, Composition):
+        return expr.inner, expr_map.REPLACE_AND_CONTINUE
+    elif isinstance(expr, Concatenation):
+        return None, expr_map.COPY_AND_STOP
+
 
 @expr_map
 def demark(expr):
     if isinstance(expr, Marker):
         return expr.inner, expr_map.REPLACE_AND_CONTINUE
 
+
+@expr_map
+def replace(expr, f):
+    expr = f(expr)
+    if expr is not None:
+        return expr, expr_map.REPLACE_AND_STOP
+
+
+@expr_map
+def remove(expr, pred):
+    if pred(expr):
+        return [], expr_map.REPLACE_AND_STOP
+
+
+def remove_unnamed_trivial_axes(expr):
+    def is_concat_child(expr):  # Do not remove direct children of concatenations
+        return expr.parent is not None and (
+            isinstance(expr.parent, Concatenation)
+            or (isinstance(expr.parent, Marker) and is_concat_child(expr.parent))
+        )
+
+    return remove(
+        expr,
+        lambda expr: isinstance(expr, Axis)
+        and expr.is_unnamed
+        and expr.value == 1
+        and not is_concat_child(expr),
+    )
+
+
+@expr_map
+def mark(expr, pred):
+    if (
+        not isinstance(expr, Marker)
+        and (expr.parent is None or not isinstance(expr.parent, Marker))
+        and pred(expr)
+    ):
+        return Marker(expr.__deepcopy__()), expr_map.REPLACE_AND_CONTINUE
+
+
 def any_parent_is(expr, pred, include_self=True):
     if not include_self:
         if expr.parent is None:
             return False
         expr = expr.parent
-    while not expr is None:
+    while expr is not None:
         if pred(expr):
             return True
         expr = expr.parent
     return False
 
+
 def is_marked(expr):
     return any_parent_is(expr, lambda expr: isinstance(expr, Marker))
 
+
+def is_at_root(expr):
+    return not any_parent_is(expr, lambda expr: isinstance(expr, Composition))
+
+
+def is_flat(expr):
+    return all(
+        not isinstance(expr, Composition) and not isinstance(expr, Concatenation)
+        for expr in expr.all()
+    )
+
+
+def get_axes(expr):
+    return [expr for expr in expr.all() if isinstance(expr, Axis)]
+
+
+def get_named_axes(expr):
+    return [expr for expr in expr.all() if isinstance(expr, Axis) and not expr.is_unnamed]
+
+
 def _get_marked(expr):
-    if isinstance(expr, NamedAxis):
+    if isinstance(expr, Axis):
         return []
-    elif isinstance(expr, UnnamedAxis):
-        return []
-    elif isinstance(expr, Ellipsis):
-        inner = _get_marked(expr.inner)
-        if len(inner) > 0:
-            return [Ellipsis(List.maybe(inner), ellipsis_id=expr.ellipsis_id)]
-        else:
-            return []
     elif isinstance(expr, Marker):
         return [expr.inner.__deepcopy__()]
     elif isinstance(expr, Concatenation):
         return [Concatenation.maybe([x for c in expr.children for x in _get_marked(c)])]
     elif isinstance(expr, Composition):
-        return [Composition(List.maybe(_get_marked(expr.inner)))]
+        return [Composition.maybe(List.maybe(_get_marked(expr.inner)))]
     elif isinstance(expr, List):
         return [List.maybe([x for c in expr.children for x in _get_marked(c)])]
-    elif isinstance(expr, Choice):
-        raise ValueError("Expression cannot contain choice")
     else:
         raise TypeError(f"Invalid expression type {type(expr)}")
 
-def get_marked(expr):
-    return List.maybe(_get_marked(expr))
 
 def get_marked(expr):
     return List.maybe(_get_marked(expr))
 
+
 def get_unmarked(expr):
     return remove(expr, lambda expr: is_marked(expr))
-
-@expr_map
-def replace(expr, f):
-    expr = f(expr)
-    if not expr is None:
-        return expr, expr_map.REPLACE_AND_STOP
-
-@expr_map
-def remove(expr, pred):
-    if pred(expr):
-        return [], expr_map.REPLACE_AND_STOP
```

### Comparing `einx-0.1.3/einx/expr/stage2.py` & `einx-0.2.0/einx/expr/stage2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from . import stage1, solver
-import re, einx
+import re
+import einx
 import numpy as np
 from collections import defaultdict
 
+
 class Expression:
     def __init__(self, ellipsis_indices):
         self.ellipsis_indices = ellipsis_indices
         self.parent = None
 
     @property
     def depth(self):
         return len(self.ellipsis_indices)
 
     @property
     def shape(self):
         return tuple(i[1] for i in self.ellipsis_indices) + (len(self),)
 
+
 class Composition(Expression):
     def __init__(self, inner, ellipsis_indices):
         Expression.__init__(self, ellipsis_indices)
         self.inner = inner
         inner.parent = self
 
     def __str__(self):
@@ -34,14 +37,15 @@
     def __deepcopy__(self):
         return Composition(self.inner.__deepcopy__(), ellipsis_indices=self.ellipsis_indices)
 
     def all(self):
         yield self
         yield from self.inner.all()
 
+
 class List(Expression):
     @staticmethod
     def maybe(l, *args, **kwargs):
         if len(l) == 1:
             return l[0]
         else:
             return List(l, *args, **kwargs)
@@ -59,28 +63,31 @@
         return sum(len(c) for c in self.children)
 
     def __iter__(self):
         for c in self.children:
             yield from c
 
     def __deepcopy__(self):
-        return List([c.__deepcopy__() for c in self.children], ellipsis_indices=self.ellipsis_indices)
+        return List(
+            [c.__deepcopy__() for c in self.children], ellipsis_indices=self.ellipsis_indices
+        )
 
     def all(self):
         yield self
         for c in self.children:
             yield from c.all()
 
+
 class NamedAxis(Expression):
     def __init__(self, name, ellipsis_indices):
         Expression.__init__(self, ellipsis_indices)
         self.name = name
 
         postfix = ""
-        for idx, num in self.ellipsis_indices:
+        for idx, _num in self.ellipsis_indices:
             postfix = postfix + "." + str(idx)
         if not self.name.endswith(postfix):
             self.name = self.name + postfix
 
     def __str__(self):
         return self.name
 
@@ -92,14 +99,15 @@
 
     def __deepcopy__(self):
         return NamedAxis(self.name, ellipsis_indices=self.ellipsis_indices)
 
     def all(self):
         yield self
 
+
 class UnnamedAxis(Expression):
     def __init__(self, value, ellipsis_indices):
         Expression.__init__(self, ellipsis_indices)
         self.value = value
 
     def __str__(self):
         return str(self.value)
@@ -112,46 +120,61 @@
 
     def __deepcopy__(self):
         return UnnamedAxis(self.value, ellipsis_indices=self.ellipsis_indices)
 
     def all(self):
         yield self
 
+
 class Concatenation(Expression):
     def __init__(self, children, ellipsis_indices):
         Expression.__init__(self, ellipsis_indices)
         for c in children:
             if len(c) != 1:
-                raise ValueError(f"Concatenation can only be used on expressions of length 1, but got expression '{c}'")
+                raise ValueError(
+                    "Concatenation can only be used on expressions of length 1, "
+                    f"but got expression '{c}'"
+                )
         self.children = children
         for c in children:
             c.parent = self
 
     def __str__(self):
         return "+".join([str(c) for c in self.children])
 
     def __len__(self):
         return 1
 
     def __iter__(self):
         yield self
 
     def __deepcopy__(self):
-        return Concatenation([c.__deepcopy__() for c in self.children], ellipsis_indices=self.ellipsis_indices)
+        return Concatenation(
+            [c.__deepcopy__() for c in self.children], ellipsis_indices=self.ellipsis_indices
+        )
 
     def all(self):
         yield self
         for c in self.children:
             yield from c.all()
 
+
 class Marker(Expression):
+    @staticmethod
+    def maybe(inner, *args, **kwargs):
+        if len(inner) == 0:
+            return inner
+        else:
+            return Marker(inner, *args, **kwargs)
+
     def __init__(self, inner, ellipsis_indices):
         Expression.__init__(self, ellipsis_indices)
         self.inner = inner
         inner.parent = self
+        assert len(inner) > 0
 
     def __str__(self):
         return f"[{self.inner}]"
 
     def __len__(self):
         return len(self.inner)
 
@@ -162,146 +185,238 @@
         return Marker(self.inner.__deepcopy__(), ellipsis_indices=self.ellipsis_indices)
 
     def all(self):
         yield self
         yield from self.inner.all()
 
 
-class SolveException(Exception):
-    def __init__(self, exprs1, exprs2, expansions1, expansions2, depths1, depths2, message, type):
-        assert len({len(exprs1), len(exprs2), len(expansions1), len(expansions2), len(depths1), len(depths2)}) == 1
+class SolveDepthException(Exception):
+    def __init__(self, exprs1, exprs2, expansions1, expansions2, depths1, depths2, message):
+        assert (
+            len({
+                len(exprs1),
+                len(exprs2),
+                len(expansions1),
+                len(expansions2),
+                len(depths1),
+                len(depths2),
+            })
+            == 1
+        )
         self.exprs1 = exprs1
         self.exprs2 = exprs2
         self.expansions1 = expansions1
         self.expansions2 = expansions2
         self.depths1 = depths1
         self.depths2 = depths2
-        self.message = f"Failed to solve {type} of expressions. {message}\nInput:\n"
-        for expr1, expr2, expansion1, expansion2, depth1, depth2 in zip(exprs1, exprs2, expansions1, expansions2, depths1, depths2):
-            self.message += f"    "
-            self.message += f"{einx.expr.util._to_str(expr1)} (expansion={einx.expr.util._to_str(expansion1)} at depth={depth1})"
-            self.message += f" = "
-            self.message += f"{einx.expr.util._to_str(expr2)} (expansion={einx.expr.util._to_str(expansion2)} at depth={depth2})"
-            self.message += f"\n"
+        self.message = (
+            "Failed to solve for the depth of axes, i.e. the number of outer ellipses.\n"
+            "Equations:\n"
+        )
+        for expr1, expr2 in zip(exprs1, exprs2):
+            if expr1 is not None and expr2 is not None:
+                self.message += "    "
+                self.message += f"{einx.expr.util._to_str(expr1)}"
+                self.message += " = "
+                self.message += f"{einx.expr.util._to_str(expr2)}"
+                self.message += "\n"
+        self.message += f"Reason: {message}"
         super().__init__(self.message)
 
-class SolveDepthException(SolveException):
-    def __init__(self, exprs1, exprs2, expansions1, expansions2, depths1, depths2, message):
-        super().__init__(exprs1, exprs2, expansions1, expansions2, depths1, depths2, message, "depths")
 
-class SolveExpansionException(SolveException):
+class SolveExpansionException(Exception):
     def __init__(self, exprs1, exprs2, expansions1, expansions2, depths1, depths2, message):
-        super().__init__(exprs1, exprs2, expansions1, expansions2, depths1, depths2, message, "expansions")
+        assert (
+            len({
+                len(exprs1),
+                len(exprs2),
+                len(expansions1),
+                len(expansions2),
+                len(depths1),
+                len(depths2),
+            })
+            == 1
+        )
+        self.exprs1 = exprs1
+        self.exprs2 = exprs2
+        self.expansions1 = expansions1
+        self.expansions2 = expansions2
+        self.depths1 = depths1
+        self.depths2 = depths2
+        self.message = "Failed to solve for the number of axes in the expressions.\nEquations:\n"
+        for expr1, expr2 in zip(exprs1, exprs2):
+            if expr1 is not None and expr2 is not None:
+                self.message += "    "
+                self.message += f"{einx.expr.util._to_str(expr1)}"
+                self.message += " = "
+                self.message += f"{einx.expr.util._to_str(expr2)}"
+                self.message += "\n"
+        self.message += f"Reason: {message}"
+        super().__init__(self.message)
+
 
 def solve(exprs1, exprs2, expansions1, expansions2, depths1, depths2):
     exprs1 = list(exprs1)
     exprs2 = list(exprs2)
     expansions1 = list(expansions1)
     expansions2 = list(expansions2)
     depths1 = list(depths1)
     depths2 = list(depths2)
-    if any(not expr is None and not isinstance(expr, stage1.Expression) for expr in exprs1 + exprs2):
+    if any(
+        expr is not None and not isinstance(expr, stage1.Expression) for expr in exprs1 + exprs2
+    ):
         raise ValueError("Can only expand stage1.Expression")
-    if len({len(exprs1), len(exprs2), len(expansions1), len(expansions2), len(depths1), len(depths2)}) != 1:
+    if (
+        len({
+            len(exprs1),
+            len(exprs2),
+            len(expansions1),
+            len(expansions2),
+            len(depths1),
+            len(depths2),
+        })
+        != 1
+    ):
         raise ValueError("Number of expressions, expansions and depths must be equal")
 
-    # Semantic check: Cannot contain choices
-    for root in exprs1 + exprs2:
-        if not root is None and any(isinstance(expr, stage1.Choice) for expr in root.all()):
-            raise ValueError(f"[|] Choice not allowed in expression '{root}'")
-
     # ##### 1. Find expression depths #####
     equations = []
 
     symbolic_expr_depths = {}
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
-                symbolic_expr_depths[id(expr)] = solver.Variable(f"symbolic_expr_depths[{id(expr)}]", str(expr))
+                symbolic_expr_depths[id(expr)] = solver.Variable(
+                    f"symbolic_expr_depths[{id(expr)}]", str(expr)
+                )
 
     # Add equations: Depth relations between subexpressions
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
                 if isinstance(expr, stage1.Ellipsis):
                     # Ellipsis increases depth by one
-                    equations.append((symbolic_expr_depths[id(expr)] + 1, symbolic_expr_depths[id(expr.inner)]))
+                    equations.append((
+                        symbolic_expr_depths[id(expr)] + 1,
+                        symbolic_expr_depths[id(expr.inner)],
+                    ))
                 else:
                     # All other expressions have the same depth as their children
                     for child in expr.direct_children:
-                        equations.append((symbolic_expr_depths[id(expr)], symbolic_expr_depths[id(child)]))
+                        equations.append((
+                            symbolic_expr_depths[id(expr)],
+                            symbolic_expr_depths[id(child)],
+                        ))
 
     # Add equations: Depth arguments
     for root, depth in zip(exprs1 + exprs2, depths1 + depths2):
-        if not root is None and not depth is None:
+        if root is not None and depth is not None:
             equations.append((symbolic_expr_depths[id(root)], depth))
 
     # Add equations: Root depths
     for root1, root2, expansion1, expansion2 in zip(exprs1, exprs2, expansions1, expansions2):
-        if not root1 is None and not root2 is None and not expansion1 is None and not expansion2 is None:
-            equations.append((symbolic_expr_depths[id(root1)] + len(expansion1), symbolic_expr_depths[id(root2)] + len(expansion2)))
+        if (
+            root1 is not None
+            and root2 is not None
+            and expansion1 is not None
+            and expansion2 is not None
+        ):
+            equations.append((
+                symbolic_expr_depths[id(root1)] + len(expansion1),
+                symbolic_expr_depths[id(root2)] + len(expansion2),
+            ))
 
     # Add equations: Multiple occurrences of the same named axis must have the same depth
     symbolic_axis_depths = {}
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for axis in root.all():
                 if isinstance(axis, stage1.NamedAxis):
-                    if not axis.name in symbolic_axis_depths:
-                        symbolic_axis_depths[axis.name] = solver.Variable(f"symbolic_axis_depths[{axis.name}]", axis.name)
-                    equations.append((symbolic_expr_depths[id(axis)], symbolic_axis_depths[axis.name]))
+                    if axis.name not in symbolic_axis_depths:
+                        symbolic_axis_depths[axis.name] = solver.Variable(
+                            f"symbolic_axis_depths[{axis.name}]", axis.name
+                        )
+                    equations.append((
+                        symbolic_expr_depths[id(axis)],
+                        symbolic_axis_depths[axis.name],
+                    ))
 
     # Add equations: Ellipses with the same id must have the same depth
     symbolic_ellipsis_depths = {}
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for ellipsis in root.all():
                 if isinstance(ellipsis, stage1.Ellipsis):
-                    if not ellipsis.ellipsis_id in symbolic_ellipsis_depths:
-                        symbolic_ellipsis_depths[ellipsis.ellipsis_id] = solver.Variable(f"symbolic_ellipsis_depths[{ellipsis.ellipsis_id}]", str(ellipsis))
-                    equations.append((symbolic_expr_depths[id(ellipsis)], symbolic_ellipsis_depths[ellipsis.ellipsis_id]))
+                    if ellipsis.ellipsis_id not in symbolic_ellipsis_depths:
+                        symbolic_ellipsis_depths[ellipsis.ellipsis_id] = solver.Variable(
+                            f"symbolic_ellipsis_depths[{ellipsis.ellipsis_id}]", str(ellipsis)
+                        )
+                    equations.append((
+                        symbolic_expr_depths[id(ellipsis)],
+                        symbolic_ellipsis_depths[ellipsis.ellipsis_id],
+                    ))
 
     # Solve
     try:
         solutions = solver.solve(equations)
     except solver.SolveException as e:
-        raise SolveDepthException(exprs1, exprs2, expansions1, expansions2, depths1, depths2, str(e))
+        raise SolveDepthException(
+            exprs1, exprs2, expansions1, expansions2, depths1, depths2, str(e)
+        ) from e
     expr_depths = {}
     for k, v in solutions.items():
         if k.startswith("symbolic_expr_depths["):
-            expr_depths[int(k[len("symbolic_expr_depths["):-1])] = int(v)
+            expr_depths[int(k[len("symbolic_expr_depths[") : -1])] = int(v)
 
     # Raise exception on missing depths
     failed_exprs = set()
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
-                if not id(expr) in expr_depths:
+                if id(expr) not in expr_depths:
                     failed_exprs.add(str(expr))
     if len(failed_exprs) > 0:
-        raise SolveDepthException(exprs1, exprs2, expansions1, expansions2, depths1, depths2, f"Found no unique solutions for {failed_exprs}")
+        raise SolveDepthException(
+            exprs1,
+            exprs2,
+            expansions1,
+            expansions2,
+            depths1,
+            depths2,
+            f"Found no unique solutions for {failed_exprs}",
+        )
 
     # Raise exception on negative depths
     failed_exprs = set()
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
                 if expr_depths[id(expr)] < 0:
                     failed_exprs.add(str(expr))
     if len(failed_exprs) > 0:
-        raise SolveDepthException(exprs1, exprs2, expansions1, expansions2, depths1, depths2, f"Got negative depths for {failed_exprs}")
-
-    for exprs, expansions, depths in zip([exprs1, exprs2], [expansions1, expansions2], [depths1, depths2]):
+        raise SolveDepthException(
+            exprs1,
+            exprs2,
+            expansions1,
+            expansions2,
+            depths1,
+            depths2,
+            f"Got negative depths for {failed_exprs}",
+        )
+
+    for exprs, expansions, _depths in zip(
+        [exprs1, exprs2], [expansions1, expansions2], [depths1, depths2]
+    ):
         for i in range(len(exprs)):
-            if not exprs[i] is None:
+            if exprs[i] is not None:
                 missing_depth = expr_depths[id(exprs[i])]
                 assert missing_depth >= 0
 
                 # Add missing dimensions to expansions
-                if not expansions[i] is None:
+                if expansions[i] is not None:
                     assert len(expansions[i]) >= 1
                     if missing_depth > 0:
                         expansions[i] = [None] * missing_depth + list(expansions[i])
 
                 # Add missing ellipses around root expressions
                 if missing_depth > 0:
                     for _ in range(missing_depth):
@@ -309,31 +424,37 @@
                         expr_depths[id(exprs[i])] = expr_depths[id(exprs[i].inner)] - 1
 
     # ##### 2. Find ellipsis expansions #####
     equations = []
 
     symbolic_expr_expansions = {}
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
                 for depth in range(expr_depths[id(expr)] + 1):
                     key = (id(expr), depth)
-                    symbolic_expr_expansions[key] = solver.Variable(f"symbolic_expr_expansions[{id(expr)},{depth}]", f"{expr} at depth {depth}")
+                    symbolic_expr_expansions[key] = solver.Variable(
+                        f"symbolic_expr_expansions[{id(expr)},{depth}]", f"{expr} at depth {depth}"
+                    )
 
-    # Add equations: Expansion of an expression at depth d (less than own depth) is equal to the expansion of each child at depth d
+    # Add equations: Expansion of an expression at depth d (less than own depth)
+    # is equal to the expansion of each child at depth d
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
                 for depth in range(expr_depths[id(expr)]):
                     for child in expr.direct_children:
-                        equations.append((symbolic_expr_expansions[(id(expr), depth)], symbolic_expr_expansions[(id(child), depth)]))
+                        equations.append((
+                            symbolic_expr_expansions[(id(expr), depth)],
+                            symbolic_expr_expansions[(id(child), depth)],
+                        ))
 
     # Add equations: Relations between expressions and their children
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
                 depth = expr_depths[id(expr)]
                 if isinstance(expr, stage1.List):
                     v = sum(symbolic_expr_expansions[(id(child), depth)] for child in expr.children)
                 elif isinstance(expr, stage1.Concatenation):
                     v = 1
                 elif isinstance(expr, stage1.NamedAxis):
@@ -343,186 +464,288 @@
                 elif isinstance(expr, stage1.Composition):
                     v = 1
                 elif isinstance(expr, stage1.Marker):
                     v = symbolic_expr_expansions[(id(expr.inner), depth)]
                 elif isinstance(expr, stage1.Ellipsis):
                     v = symbolic_expr_expansions[(id(expr.inner), depth)]
                 else:
-                    assert False, f"{expr}"
+                    raise AssertionError(f"{expr}")
                 equations.append((symbolic_expr_expansions[(id(expr), depth)], v))
 
     # Add equations: Expansions stored in "expansions"
     for expansion1, expansion2, expr1, expr2 in zip(expansions1, expansions2, exprs1, exprs2):
-        if not expansion1 is None and not expansion2 is None:
-            if len(expansion1) != len(expansion2) or any(not e1 is None and not e2 is None and e1 != e2 for e1, e2 in zip(expansion1, expansion2)):
-                raise SolveExpansionException(exprs1, exprs2, expansions1, expansions2, depths1, depths2, 
-                    f"Expansion '{expansion1}' of expression '{expr1}' does not match expansion '{expansion2}' of expression '{expr2}'")
-
-        if not expansion1 is None and not expansion2 is None:
-            expansion = [e1 if not e1 is None else e2 for e1, e2 in zip(expansion1, expansion2)]
-        elif not expansion1 is None:
+        if expansion1 is not None and expansion2 is not None:
+            if len(expansion1) != len(expansion2) or any(
+                e1 is not None and e2 is not None and e1 != e2
+                for e1, e2 in zip(expansion1, expansion2)
+            ):
+                raise SolveExpansionException(
+                    exprs1,
+                    exprs2,
+                    expansions1,
+                    expansions2,
+                    depths1,
+                    depths2,
+                    f"Expansion '{expansion1}' of expression '{expr1}' does not match expansion "
+                    f"'{expansion2}' of expression '{expr2}'",
+                )
+
+        if expansion1 is not None and expansion2 is not None:
+            expansion = [e1 if e1 is not None else e2 for e1, e2 in zip(expansion1, expansion2)]
+        elif expansion1 is not None:
             expansion = expansion1
-        elif not expansion2 is None:
+        elif expansion2 is not None:
             expansion = expansion2
         else:
             expansion = None
 
-        if not expansion is None:
+        if expansion is not None:
             for depth, e in enumerate(expansion):
-                if not e is None:
-                    if not expr1 is None and depth <= expr_depths[id(expr1)]:
+                if e is not None:
+                    if expr1 is not None and depth <= expr_depths[id(expr1)]:
                         equations.append((symbolic_expr_expansions[(id(expr1), depth)], int(e)))
-                    if not expr2 is None and depth <= expr_depths[id(expr2)]:
+                    if expr2 is not None and depth <= expr_depths[id(expr2)]:
                         equations.append((symbolic_expr_expansions[(id(expr2), depth)], int(e)))
 
     # Add equations: Multiple occurrences of the same named axis must have the same expansions
     symbolic_axis_expansions = {}
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for axis in root.all():
                 if isinstance(axis, stage1.NamedAxis):
                     for depth in range(expr_depths[id(axis)] + 1):
-                        if not axis.name in symbolic_axis_expansions:
-                            symbolic_axis_expansions[(axis.name, depth)] = solver.Variable(f"symbolic_axis_expansions[{axis.name},{depth}]", f"{axis.name} at depth {depth}")
-                        equations.append((symbolic_expr_expansions[(id(axis), depth)], symbolic_axis_expansions[(axis.name, depth)]))
+                        if axis.name not in symbolic_axis_expansions:
+                            symbolic_axis_expansions[(axis.name, depth)] = solver.Variable(
+                                f"symbolic_axis_expansions[{axis.name},{depth}]",
+                                f"{axis.name} at depth {depth}",
+                            )
+                        equations.append((
+                            symbolic_expr_expansions[(id(axis), depth)],
+                            symbolic_axis_expansions[(axis.name, depth)],
+                        ))
 
     # Add equations: Ellipses with the same id must have the same expansions
     symbolic_ellipsis_expansions = {}
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for ellipsis in root.all():
                 if isinstance(ellipsis, stage1.Ellipsis):
                     for depth in range(expr_depths[id(ellipsis)] + 1):
-                        if not ellipsis.ellipsis_id in symbolic_ellipsis_expansions:
-                            symbolic_ellipsis_expansions[(ellipsis.ellipsis_id, depth)] = solver.Variable(f"symbolic_ellipsis_expansions[{ellipsis.ellipsis_id},{depth}]", f"{ellipsis} at depth {depth}")
-                        equations.append((symbolic_expr_expansions[(id(ellipsis), depth)], symbolic_ellipsis_expansions[(ellipsis.ellipsis_id, depth)]))
+                        if ellipsis.ellipsis_id not in symbolic_ellipsis_expansions:
+                            symbolic_ellipsis_expansions[(ellipsis.ellipsis_id, depth)] = (
+                                solver.Variable(
+                                    f"symbolic_ellipsis_expansions[{ellipsis.ellipsis_id},{depth}]",
+                                    f"{ellipsis} at depth {depth}",
+                                )
+                            )
+                        equations.append((
+                            symbolic_expr_expansions[(id(ellipsis), depth)],
+                            symbolic_ellipsis_expansions[(ellipsis.ellipsis_id, depth)],
+                        ))
 
     # Add equations: Same root expansions
     for root1, root2 in zip(exprs1, exprs2):
-        if not root1 is None and not root2 is None:
+        if root1 is not None and root2 is not None:
             assert expr_depths[id(root1)] == expr_depths[id(root2)]
             for depth in range(expr_depths[id(root1)] + 1):
-                equations.append((symbolic_expr_expansions[(id(root1), depth)], symbolic_expr_expansions[(id(root2), depth)]))
+                equations.append((
+                    symbolic_expr_expansions[(id(root1), depth)],
+                    symbolic_expr_expansions[(id(root2), depth)],
+                ))
 
     # Solve
     try:
         solutions = solver.solve(equations)
     except solver.SolveException as e:
-        raise SolveExpansionException(exprs1, exprs2, expansions1, expansions2, depths1, depths2, str(e))
+        raise SolveExpansionException(
+            exprs1, exprs2, expansions1, expansions2, depths1, depths2, str(e)
+        ) from e
+
     def to_key(k):
         return int(id_expr), int(depth)
+
     expansion_values = {}
     for k, v in solutions.items():
         if k.startswith("symbolic_expr_expansions["):
-            k = k[len("symbolic_expr_expansions["):-1]
+            k = k[len("symbolic_expr_expansions[") : -1]
             id_expr, depth = str(k).split(",")
             try:
                 id_expr = int(id_expr)
             except ValueError:
                 continue
             depth = int(depth)
             expansion_values[(id_expr, depth)] = int(v)
 
     failed_exprs = set()
     for root in exprs1 + exprs2:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
-                if not (id(root), expr_depths[id(root)]) in expansion_values:
+                if (id(root), expr_depths[id(root)]) not in expansion_values:
                     failed_exprs.add(str(expr))
     if len(failed_exprs) == 1:
-        raise SolveExpansionException(exprs1, exprs2, expansions1, expansions2, depths1, depths2, f"Found no unique solution for '{failed_exprs.pop()}'")
+        raise SolveExpansionException(
+            exprs1,
+            exprs2,
+            expansions1,
+            expansions2,
+            depths1,
+            depths2,
+            f"Found no unique solution for '{failed_exprs.pop()}'",
+        )
     elif len(failed_exprs) > 1:
-        raise SolveExpansionException(exprs1, exprs2, expansions1, expansions2, depths1, depths2, f"Found no unique solutions for {failed_exprs}")
+        raise SolveExpansionException(
+            exprs1,
+            exprs2,
+            expansions1,
+            expansions2,
+            depths1,
+            depths2,
+            f"Found no unique solutions for {failed_exprs}",
+        )
 
     def is_unnamed(expr):
         for expr in expr.all():
             if isinstance(expr, stage1.NamedAxis):
                 return False
         return True
+
     def get_unnamed_value(expr):
         if isinstance(expr, stage1.List):
             return np.prod([get_unnamed_value(child) for child in expr.children]).astype("int")
         elif isinstance(expr, stage1.Concatenation):
             return np.sum([get_unnamed_value(child) for child in expr.children])
         elif isinstance(expr, stage1.NamedAxis):
-            assert False
+            raise AssertionError()
         elif isinstance(expr, stage1.UnnamedAxis):
             return expr.value
         elif isinstance(expr, stage1.Composition):
             return get_unnamed_value(expr.inner)
         elif isinstance(expr, stage1.Marker):
             return get_unnamed_value(expr.inner)
         elif isinstance(expr, stage1.Ellipsis):
             value = get_unnamed_value(expr.inner)
-            if value != 1: # TODO: implement this
-                raise NotImplementedError(f"Found unnamed and unexpanded ellipsis '{expr}'. We currently disallow this case, since it could can take on multiple values ('2...' could have values 2, 4, ...) that should be resolved in the solver and then checked to be consistent with these constraints.")
+            if value != 1:  # TODO: implement this
+                raise NotImplementedError(
+                    f"Found unnamed and unexpanded ellipsis '{expr}'. We currently disallow this "
+                    "case, since it could can take on multiple values ('2...' could have values "
+                    "2, 4, ...) that should be resolved in the solver and then checked to be "
+                    "consistent with these constraints."
+                )
             return 1
         else:
-            assert False, f"{expr}"
+            raise AssertionError(f"{expr}")
 
     # Expand ellipses and map stage1 expressions to stage2 expressions
     def map(expr, ellipsis_indices):
         if isinstance(expr, list):
             return [c for expr in expr for c in map(expr, ellipsis_indices=ellipsis_indices)]
         elif isinstance(expr, stage1.NamedAxis):
             return [NamedAxis(expr.name, ellipsis_indices=ellipsis_indices)]
         elif isinstance(expr, stage1.UnnamedAxis):
             return [UnnamedAxis(expr.value, ellipsis_indices=ellipsis_indices)]
         elif isinstance(expr, stage1.List):
             return map(expr.children, ellipsis_indices=ellipsis_indices)
         elif isinstance(expr, stage1.Concatenation):
-            return [Concatenation([List.maybe(map(c, ellipsis_indices=ellipsis_indices), ellipsis_indices=ellipsis_indices) for c in expr.children], ellipsis_indices=ellipsis_indices)]
+            return [
+                Concatenation(
+                    [
+                        List.maybe(
+                            map(c, ellipsis_indices=ellipsis_indices),
+                            ellipsis_indices=ellipsis_indices,
+                        )
+                        for c in expr.children
+                    ],
+                    ellipsis_indices=ellipsis_indices,
+                )
+            ]
         elif isinstance(expr, stage1.Composition):
-            return [Composition(List.maybe(map(expr.inner, ellipsis_indices=ellipsis_indices), ellipsis_indices=ellipsis_indices), ellipsis_indices=ellipsis_indices)]
+            return [
+                Composition(
+                    List.maybe(
+                        map(expr.inner, ellipsis_indices=ellipsis_indices),
+                        ellipsis_indices=ellipsis_indices,
+                    ),
+                    ellipsis_indices=ellipsis_indices,
+                )
+            ]
         elif isinstance(expr, stage1.Marker):
-            return [Marker(List.maybe(map(expr.inner, ellipsis_indices=ellipsis_indices), ellipsis_indices=ellipsis_indices), ellipsis_indices=ellipsis_indices)]
+            return [
+                Marker.maybe(
+                    List.maybe(
+                        map(expr.inner, ellipsis_indices=ellipsis_indices),
+                        ellipsis_indices=ellipsis_indices,
+                    ),
+                    ellipsis_indices=ellipsis_indices,
+                )
+            ]
         elif isinstance(expr, stage1.Ellipsis):
             key = (id(expr), expr_depths[id(expr)])
             if key in expansion_values:
                 # Ellipsis is expanded
                 expansion = expansion_values[key]
                 if expansion < 0:
-                    raise SolveExpansionException(exprs1, exprs2, expansions1, expansions2, depths1, depths2, f"Ellipsis '{expr}' has negative expansion {expansion}")
-                return [c for i in range(expansion) for c in map(expr.inner, ellipsis_indices=ellipsis_indices + [(i, expansion)])]
+                    raise SolveExpansionException(
+                        exprs1,
+                        exprs2,
+                        expansions1,
+                        expansions2,
+                        depths1,
+                        depths2,
+                        f"Ellipsis '{expr}' has negative expansion {expansion}",
+                    )
+                return [
+                    c
+                    for i in range(expansion)
+                    for c in map(expr.inner, ellipsis_indices=ellipsis_indices + [(i, expansion)])
+                ]
             else:
                 # Ellipsis is not expanded
                 if is_unnamed(expr):
                     # Contains no named axes -> convert to unnamed axis
                     return [UnnamedAxis(get_unnamed_value(expr), ellipsis_indices=ellipsis_indices)]
                 else:
                     # Contains named axes -> convert to named axis
                     return [NamedAxis(str(expr), ellipsis_indices=ellipsis_indices)]
         else:
-            assert False, f"{expr}"
-    exprs1 = [List.maybe(map(root, ellipsis_indices=[]), ellipsis_indices=[]) if not root is None else None for root in exprs1]
-    exprs2 = [List.maybe(map(root, ellipsis_indices=[]), ellipsis_indices=[]) if not root is None else None for root in exprs2]
-
-    return exprs1, exprs2
+            raise AssertionError(f"{expr}")
 
+    exprs1 = [
+        List.maybe(map(root, ellipsis_indices=[]), ellipsis_indices=[])
+        if root is not None
+        else None
+        for root in exprs1
+    ]
+    exprs2 = [
+        List.maybe(map(root, ellipsis_indices=[]), ellipsis_indices=[])
+        if root is not None
+        else None
+        for root in exprs2
+    ]
 
+    return exprs1, exprs2
 
 
 def cse(expressions, cse_concat=True, cse_in_markers=False, verbose=False):
     expressions = list(expressions)
-    if any(not expr is None and not isinstance(expr, Expression) for expr in expressions):
-        raise TypeError(f"Expected expressions to be of type Expression")
+    if any(expr is not None and not isinstance(expr, Expression) for expr in expressions):
+        raise TypeError("Expected expressions to be of type Expression")
 
     # Find possible expressions, identified by their string representation
     str_to_common_expr = defaultdict(list)
     for root in expressions:
-        if not root is None:
+        if root is not None:
             for expr in root.all():
-                if not expr.parent is None:
+                if expr.parent is not None:
                     str_expr = str(expr)
                     str_to_common_expr[str_expr].append([expr])
 
                     if isinstance(expr, List):
                         for start_index in range(len(expr.children)):
                             for end_index in range(start_index, len(expr.children)):
-                                children = expr.children[start_index:end_index + 1]
+                                children = expr.children[start_index : end_index + 1]
                                 str_expr = " ".join([str(c) for c in children])
                                 str_to_common_expr[str_expr].append(children)
 
     if verbose:
         print("CSE: All subexpressions")
         for k in str_to_common_expr.keys():
             print(f"    {k}")
@@ -542,44 +765,56 @@
                         used_axis_names.add(v.name)
 
         if len(used_axis_ids) == 0:
             continue
 
         axes_used_only_in_this_subexpression = True
         for root in expressions:
-            if not root is None:
+            if root is not None:
                 for global_axis in root.all():
                     if isinstance(global_axis, NamedAxis) and global_axis.name in used_axis_names:
-                        axes_used_only_in_this_subexpression = axes_used_only_in_this_subexpression and id(global_axis) in used_axis_ids
+                        axes_used_only_in_this_subexpression = (
+                            axes_used_only_in_this_subexpression
+                            and id(global_axis) in used_axis_ids
+                        )
 
         if axes_used_only_in_this_subexpression:
             common_exprs.add(str_expr)
 
-    common_exprs = [str_to_common_expr[k] for k in common_exprs] # list of common_expr(=list of exprlist)
+    common_exprs = [
+        str_to_common_expr[k] for k in common_exprs
+    ]  # list of common_expr(=list of exprlist)
 
     if verbose:
         print("CSE: Removed expressions with axes that are also used outside the expression")
         for v in common_exprs:
             print(f"    {[' '.join([str(y) for y in x]) for x in v]}")
 
     def remove_duplicates(common_expr):
         new_common_expr = []
         for exprlist1 in common_expr:
             is_duplicate = False
             for exprlist2 in new_common_expr:
-                is_duplicate = is_duplicate or (len(exprlist1) == len(exprlist2) and all(id(expr1) == id(expr2) for expr1, expr2 in zip(exprlist1, exprlist2)))
+                is_duplicate = is_duplicate or (
+                    len(exprlist1) == len(exprlist2)
+                    and all(id(expr1) == id(expr2) for expr1, expr2 in zip(exprlist1, exprlist2))
+                )
             if not is_duplicate:
                 new_common_expr.append(exprlist1)
         return new_common_expr
+
     common_exprs = [remove_duplicates(exprlists) for exprlists in common_exprs]
 
     if verbose:
         print("CSE: Removed duplicates")
         for v in common_exprs:
-            print(f"    {[' '.join([str(y) for y in x]) for x in v]} {[[id(y) for y in x] for x in v]}")
+            print(
+                f"    {[' '.join([str(y) for y in x]) for x in v]} "
+                f"{[[id(y) for y in x] for x in v]}"
+            )
 
     # Remove singletons
     def is_singleton(expr):
         if isinstance(expr, list):
             return len(expr) == 1 and is_singleton(expr[0])
         elif isinstance(expr, List):
             return is_singleton(expr.children)
@@ -587,60 +822,104 @@
             return True
         elif isinstance(expr, UnnamedAxis):
             return True
         elif isinstance(expr, Marker):
             return is_singleton(expr.inner)
         else:
             return False
+
     common_exprs = [common_expr for common_expr in common_exprs if not is_singleton(common_expr[0])]
 
     if verbose:
         print("CSE: Removed singletons")
         for v in common_exprs:
             print(f"    {[' '.join([str(y) for y in x]) for x in v]}")
 
     # Remove expressions with/ in markers
     if cse_in_markers:
-        common_exprs = [common_expr for common_expr in common_exprs if not any(isinstance(expr, Marker) for exprlist in common_expr for expr in exprlist for expr in expr.all())]
+        common_exprs = [
+            common_expr
+            for common_expr in common_exprs
+            if not any(
+                isinstance(expr, Marker)
+                for exprlist in common_expr
+                for expr in exprlist
+                for expr in expr.all()
+            )
+        ]
     else:
-        common_exprs = [common_expr for common_expr in common_exprs if not any(einx.expr.stage2.is_marked(expr) for exprlist in common_expr for expr in exprlist for expr in expr.all())]
+        common_exprs = [
+            common_expr
+            for common_expr in common_exprs
+            if not any(
+                einx.expr.stage2.is_marked(expr)
+                for exprlist in common_expr
+                for expr in exprlist
+                for expr in expr.all()
+            )
+        ]
 
     # Remove expressions that contain concatenations
     if not cse_concat:
-        common_exprs = [common_expr for common_expr in common_exprs if not any(isinstance(expr, Concatenation) for exprlist in common_expr for expr in exprlist for expr in expr.all())]
+        common_exprs = [
+            common_expr
+            for common_expr in common_exprs
+            if not any(
+                isinstance(expr, Concatenation)
+                for exprlist in common_expr
+                for expr in exprlist
+                for expr in expr.all()
+            )
+        ]
 
     if verbose:
         print("CSE: Removed expressions with markers")
         for v in common_exprs:
             print(f"    {[' '.join([str(y) for y in x]) for x in v]}")
 
     # Remove expressions at root level with len > 1
-    common_exprs = [common_expr for common_expr in common_exprs if not (is_at_root(common_expr[0][0]) and (len(common_expr[0]) > 1 or len(common_expr[0][0]) > 1))]
+    common_exprs = [
+        common_expr
+        for common_expr in common_exprs
+        if not (
+            is_at_root(common_expr[0][0])
+            and (len(common_expr[0]) > 1 or len(common_expr[0][0]) > 1)
+        )
+    ]
 
     if verbose:
         print("CSE: Removed subexpressions of root with len > 1")
         for v in common_exprs:
             print(f"    {[' '.join([str(y) for y in x]) for x in v]}")
 
     # Remove subexpressions of subexpressions
     def any_is_parent_of(parent, child):
         if isinstance(parent, list):
             return any(any_is_parent_of(p, child) for p in parent)
         elif isinstance(child, list):
             return any(any_is_parent_of(parent, c) for c in child)
         else:
-            return not child.parent is None and (id(child.parent) == id(parent) or any_is_parent_of(parent, child.parent))
-    common_exprs = [common_expr for common_expr in common_exprs if not any(id(common_expr) != id(common_expr2) and any_is_parent_of(common_expr2, common_expr) for common_expr2 in common_exprs)]
+            return child.parent is not None and (
+                id(child.parent) == id(parent) or any_is_parent_of(parent, child.parent)
+            )
+
+    common_exprs = [
+        common_expr
+        for common_expr in common_exprs
+        if not any(
+            id(common_expr) != id(common_expr2) and any_is_parent_of(common_expr2, common_expr)
+            for common_expr2 in common_exprs
+        )
+    ]
 
     if verbose:
         print("CSE: Removed subexpressions of subexpressions")
         for v in common_exprs:
             print(f"    {[' '.join([str(y) for y in x]) for x in v]}")
 
-    
     # All subexpressions have been found. Now replace them with new Axis objects.
     def replace(expr):
         if isinstance(expr, list) and len(expr) == 1:
             return replace(expr[0])
         if not isinstance(expr, list):
             for idx, common_expr in enumerate(common_exprs):
                 for exprlist in common_expr:
@@ -656,19 +935,19 @@
                 for idx, common_expr in enumerate(common_exprs):
                     for exprlist in common_expr:
                         for j in range(len(exprlist)):
                             if i + j >= len(expr) or id(exprlist[j]) != id(expr[i + j]):
                                 break
                         else:
                             exprlist_found = exprlist
-                    if not exprlist_found is None:
+                    if exprlist_found is not None:
                         break
                 exprlist = exprlist_found
 
-                if not exprlist is None:
+                if exprlist is not None:
                     assert len(exprlist) > 0
                     result.append(NamedAxis(f"cse.{idx}", exprlist[0].ellipsis_indices))
                     i += len(exprlist)
                 else:
                     result.extend(replace(expr[i]))
                     i += 1
 
@@ -676,31 +955,38 @@
         elif isinstance(expr, NamedAxis):
             return [expr.__deepcopy__()]
         elif isinstance(expr, UnnamedAxis):
             return [expr.__deepcopy__()]
         elif isinstance(expr, List):
             return replace(expr.children)
         elif isinstance(expr, Concatenation):
-            return [Concatenation([c2 for c1 in expr.children for c2 in replace(c1)], expr.ellipsis_indices)]
+            return [
+                Concatenation(
+                    [c2 for c1 in expr.children for c2 in replace(c1)], expr.ellipsis_indices
+                )
+            ]
         elif isinstance(expr, Marker):
-            return [Marker(List.maybe(replace(expr.inner), expr.ellipsis_indices), expr.ellipsis_indices)]
+            return [
+                Marker.maybe(
+                    List.maybe(replace(expr.inner), expr.ellipsis_indices), expr.ellipsis_indices
+                )
+            ]
         elif isinstance(expr, Composition):
-            return [Composition(List.maybe(replace(expr.inner), expr.ellipsis_indices), expr.ellipsis_indices)]
+            return [
+                Composition(
+                    List.maybe(replace(expr.inner), expr.ellipsis_indices), expr.ellipsis_indices
+                )
+            ]
         else:
-            assert False
-    return [List.maybe(replace(root), ellipsis_indices=[]) if not root is None else None for root in expressions]
-
-
-
-
-
-
-
-
+            raise AssertionError()
 
+    return [
+        List.maybe(replace(root), ellipsis_indices=[]) if root is not None else None
+        for root in expressions
+    ]
 
 
 def expr_map(f):
     def outer(expr, *args, **kwargs):
         # Wrap the user function to return a list of expressions
         def f2(expr):
             t = f(expr, *args, **kwargs)
@@ -712,22 +998,26 @@
                 return expr, signal
             if isinstance(expr, List):
                 return expr.children, signal
             elif isinstance(expr, Expression):
                 return [expr], signal
             else:
                 raise TypeError(f"Invalid return type {type(expr)}")
+
         return List.maybe(_expr_map(expr, f2))
+
     return outer
 
+
 expr_map.CONTINUE = 1
 expr_map.COPY_AND_STOP = 2
 expr_map.REPLACE_AND_STOP = 3
 expr_map.REPLACE_AND_CONTINUE = 4
 
+
 def _expr_map(expr, f):
     exprs, signal = f(expr)
     if signal == expr_map.REPLACE_AND_STOP:
         assert isinstance(exprs, list)
         return exprs
     elif signal == expr_map.COPY_AND_STOP:
         return [expr.__deepcopy__()]
@@ -746,67 +1036,74 @@
         return [Concatenation([List.maybe(_expr_map(c, f)) for c in expr.children])]
     elif isinstance(expr, Marker):
         x = _expr_map(expr.inner, f)
         if len(x) == 0:
             # Drop empty marker
             return []
         else:
-            return [Marker(List.maybe(x))]
+            return [Marker.maybe(List.maybe(x))]
     else:
         raise TypeError(f"Invalid expression type {type(expr)}")
 
+
 @expr_map
 def demark(expr):
     if isinstance(expr, Marker):
         return expr.inner, expr_map.REPLACE_AND_CONTINUE
 
+
 def any_parent_is(expr, pred, include_self=True):
     if not include_self:
         if expr.parent is None:
             return False
         expr = expr.parent
-    while not expr is None:
+    while expr is not None:
         if pred(expr):
             return True
         expr = expr.parent
     return False
 
+
 def is_at_root(expr):
     return not any_parent_is(expr, lambda expr: isinstance(expr, Composition), include_self=False)
 
+
 def is_marked(expr):
     return any_parent_is(expr, lambda expr: isinstance(expr, Marker))
 
+
 def _get_marked(expr):
     if isinstance(expr, NamedAxis):
         return []
     elif isinstance(expr, UnnamedAxis):
         return []
     elif isinstance(expr, Marker):
         return [expr.inner.__deepcopy__()]
     elif isinstance(expr, Concatenation):
         return [Concatenation.maybe([x for c in expr.children for x in _get_marked(c)])]
     elif isinstance(expr, Composition):
         return [Composition(List.maybe(_get_marked(expr.inner)))]
     elif isinstance(expr, List):
         return [List.maybe([x for c in expr.children for x in _get_marked(c)])]
-    elif isinstance(expr, Choice):
-        raise ValueError("Expression cannot contain choice")
     else:
         raise TypeError(f"Invalid expression type {type(expr)}")
 
+
 def get_marked(expr):
     return List.maybe(_get_marked(expr))
 
+
 def get_unmarked(expr):
     return remove(expr, lambda expr: not is_marked(expr))
 
+
 @expr_map
 def replace(expr, f):
     expr = f(expr)
-    if not expr is None:
+    if expr is not None:
         return expr, expr_map.REPLACE_AND_STOP
 
+
 @expr_map
 def remove(expr, pred):
     if pred(expr):
-        return [], expr_map.REPLACE_AND_STOP
+        return [], expr_map.REPLACE_AND_STOP
```

### Comparing `einx-0.1.3/einx/expr/util.py` & `einx-0.2.0/einx/expr/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,105 +1,131 @@
 from . import stage1, stage2, stage3
 import numpy as np
 import einx
 
+
 def _get_expansion(expr):
     if isinstance(expr, stage1.Expression):
         return (expr.expansion(),)
     elif isinstance(expr, (stage2.Expression, stage3.Expression)):
         return (len(expr),)
     elif isinstance(expr, np.ndarray):
         return tuple(expr.shape)
     else:
         return None
 
+
 def _input_expr(expr):
-    if expr is None or isinstance(expr, (str, stage1.Expression, stage2.Expression, stage3.Expression)):
+    if expr is None or isinstance(
+        expr, (str, stage1.Expression, stage2.Expression, stage3.Expression)
+    ):
         return expr
     else:
         if isinstance(expr, np.ndarray):
             pass
         elif expr == [] or expr == ():
             expr = np.asarray(expr).astype("int32")
         else:
             try:
                 expr = np.asarray(expr)
-            except e:
-                raise ValueError(f"Invalid expression '{expr}'")
+            except Exception as e:
+                raise ValueError(f"Invalid expression '{expr}'") from e
         if not np.issubdtype(expr.dtype, np.integer):
             raise ValueError(f"Invalid expression '{expr}', must be integers")
         expr = " ".join([str(i) for i in expr.flatten()])
         return expr
 
+
 class Equation:
     def __init__(self, expr1, expr2=None, depth1=0, depth2=0):
         self.expr1 = _input_expr(expr1)
         self.expr2 = _input_expr(expr2)
         self.expansion1 = _get_expansion(expr1)
         self.expansion2 = _get_expansion(expr2)
         self.depth1 = depth1
         self.depth2 = None if expr2 is None else depth2
 
     def __repr__(self):
-        return f"{self.expr} = {self.value.tolist()} (expansion={self.expansion} at depth={self.depth})"
+        return f"{self.expr} = {self.value.tolist()} (expansion={self.expansion} at "
+        f"depth={self.depth})"
+
 
-def _to_str(l): # Print numpy arrays in a single line rather than with line breaks
+def _to_str(l):  # Print numpy arrays in a single line rather than with line breaks
     if l is None:
         return "None"
     elif isinstance(l, np.ndarray):
         return str(tuple(l.tolist()))
     elif isinstance(l, list):
         return str(tuple(l))
     else:
         return str(l)
 
-def solve(equations, cse=True, cse_concat=True, cse_in_markers=False, after_stage2=None, verbose=False):
+
+def solve(
+    equations, cse=True, cse_concat=True, cse_in_markers=False, after_stage2=None, verbose=False
+):
     if any(not isinstance(c, Equation) for c in equations):
         raise ValueError("All arguments must be of type Equation")
 
     exprs1 = [t.expr1 for t in equations]
     exprs2 = [t.expr2 for t in equations]
     expansions1 = [t.expansion1 for t in equations]
     expansions2 = [t.expansion2 for t in equations]
     depths1 = [t.depth1 for t in equations]
     depths2 = [t.depth2 for t in equations]
 
     if verbose:
         print("Stage0:")
-        for expr1, expr2, expansion1, expansion2, depth1, depth2 in zip(exprs1, exprs2, expansions1, expansions2, depths1, depths2):
-            print(f"    {_to_str(expr1)} (expansion={_to_str(expansion1)} at depth={depth1}) = {_to_str(expr2)} (expansion={_to_str(expansion2)} at depth={depth2})")
-
-    exprs1 = [(stage1.parse(expr) if isinstance(expr, str) else expr) for expr in exprs1]
-    exprs2 = [(stage1.parse(expr) if isinstance(expr, str) else expr) for expr in exprs2]
-
-    expansions1 = [expansion if not expansion is None else _get_expansion(expr) for expansion, expr in zip(expansions1, exprs1)]
-    expansions2 = [expansion if not expansion is None else _get_expansion(expr) for expansion, expr in zip(expansions2, exprs2)]
+        for expr1, expr2, expansion1, expansion2, depth1, depth2 in zip(
+            exprs1, exprs2, expansions1, expansions2, depths1, depths2
+        ):
+            print(
+                f"    {_to_str(expr1)} (expansion={_to_str(expansion1)} at depth={depth1}) = "
+                f"{_to_str(expr2)} (expansion={_to_str(expansion2)} at depth={depth2})"
+            )
+
+    exprs1 = [(stage1.parse_arg(expr) if isinstance(expr, str) else expr) for expr in exprs1]
+    exprs2 = [(stage1.parse_arg(expr) if isinstance(expr, str) else expr) for expr in exprs2]
+
+    expansions1 = [
+        expansion if expansion is not None else _get_expansion(expr)
+        for expansion, expr in zip(expansions1, exprs1)
+    ]
+    expansions2 = [
+        expansion if expansion is not None else _get_expansion(expr)
+        for expansion, expr in zip(expansions2, exprs2)
+    ]
 
     if verbose:
         print("Stage1:")
-        for expr1, expr2, expansion1, expansion2, depth1, depth2 in zip(exprs1, exprs2, expansions1, expansions2, depths1, depths2):
-            print(f"    {_to_str(expr1)} (expansion={_to_str(expansion1)} at depth={depth1}) = {_to_str(expr2)} (expansion={_to_str(expansion2)} at depth={depth2})")
+        for expr1, expr2, expansion1, expansion2, depth1, depth2 in zip(
+            exprs1, exprs2, expansions1, expansions2, depths1, depths2
+        ):
+            print(
+                f"    {_to_str(expr1)} (expansion={_to_str(expansion1)} at depth={depth1}) = "
+                f"{_to_str(expr2)} (expansion={_to_str(expansion2)} at depth={depth2})"
+            )
 
     exprs1, exprs2 = stage2.solve(exprs1, exprs2, expansions1, expansions2, depths1, depths2)
 
     if verbose:
         print("Stage2:")
         for expr1, expr2 in zip(exprs1, exprs2):
             print(f"    {_to_str(expr1)} = {_to_str(expr2)}")
 
     if cse:
         exprs = stage2.cse(exprs1 + exprs2, cse_concat=cse_concat, cse_in_markers=cse_in_markers)
-        exprs1, exprs2 = exprs[:len(exprs1)], exprs[len(exprs1):]
+        exprs1, exprs2 = exprs[: len(exprs1)], exprs[len(exprs1) :]
 
         if verbose:
             print("Stage2.CSE:")
             for expr1, expr2 in zip(exprs1, exprs2):
                 print(f"    {_to_str(expr1)} = {_to_str(expr2)}")
 
-    if not after_stage2 is None:
+    if after_stage2 is not None:
         return solve(
             equations + after_stage2(exprs1, exprs2),
             cse=cse,
             cse_concat=cse_concat,
             cse_in_markers=cse_in_markers,
             after_stage2=None,
             verbose=verbose,
@@ -107,12 +133,12 @@
 
     exprs1, exprs2 = stage3.solve(exprs1, exprs2)
 
     if verbose:
         print("Stage3:")
         for expr1, expr2 in zip(exprs1, exprs2):
             assert expr1 is None or expr2 is None or expr1.shape == expr2.shape
-            shape = expr1.shape if not expr1 is None else expr2.shape
+            shape = expr1.shape if expr1 is not None else expr2.shape
             shape = " ".join(str(i) for i in shape)
             print(f"    {_to_str(expr1)} = {_to_str(expr2)} = {shape}")
 
     return exprs1
```

### Comparing `einx-0.1.3/einx/nn/equinox.py` & `einx-0.2.0/einx/nn/equinox.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,45 @@
-import einx, jax
+import einx
+import jax
 import equinox as eqx
 from functools import partial
 import jax.numpy as jnp
 from typing import Optional, Callable, Any
 
+# TODO: type annotations
+
+
 def param(module, name=None, init=None, dtype=None, rng=None):
     """Create a tensor factory for Equinox parameters.
 
     Args:
         module: The module to create the parameter in. Must be an instance of ``eqx.Module``.
-        name: Name of the parameter. If ``None``, uses a default name determined from the calling operation. Defaults to ``None``.
-        init: Initializer for the parameter. If ``None``, uses a default init method determined from the calling operation. Defaults to ``None``.
-        dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling module or ``float32`` if it does not exist. Defaults to ``None``.
+        name: Name of the parameter. If ``None``, uses a default name determined from the calling
+            operation. Defaults to ``None``.
+        init: Initializer for the parameter. If ``None``, uses a default init method determined
+            from the calling operation. Defaults to ``None``.
+        dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling
+            module or ``float32`` if it does not exist. Defaults to ``None``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
 
+    name0 = name
+    init0 = init
+    dtype0 = dtype
+
     def equinox_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
+        if name0 is not None:
+            name = name0
+        if init0 is not None:
+            init = init0
+        if dtype0 is not None:
+            dtype = dtype0
+
         if name is None:
             raise ValueError("Must specify name for tensor factory eqx.Module")
 
         if dtype is None:
             if hasattr(module, "dtype"):
                 dtype = module.dtype
             else:
@@ -33,47 +51,53 @@
             if init == "get_at" or init == "rearrange":
                 init = jax.nn.initializers.normal(stddev=0.02)
             elif init == "add":
                 init = jax.nn.initializers.constant(0.0, dtype=dtype)
             elif init == "multiply":
                 init = jax.nn.initializers.constant(1.0, dtype=dtype)
             elif init == "dot":
-                init = jax.nn.initializers.lecun_normal(kwargs["in_axis"], kwargs["out_axis"], kwargs["batch_axis"])
+                init = jax.nn.initializers.lecun_normal(
+                    kwargs["in_axis"], kwargs["out_axis"], kwargs["batch_axis"]
+                )
             else:
                 raise ValueError(f"Don't know which initializer to use for operation '{init}'")
         elif isinstance(init, (int, float)):
             init = jax.nn.initializers.constant(init, dtype=dtype)
 
-        if not vars(module)[name] is None:
+        if vars(module)[name] is not None:
             tensor = vars(module)[name]
         else:
             tensor = vars(module)[name] = init(rng, shape, dtype)
         return tensor
+
     return equinox_param_factory
 
+
 def to_tensor_factory(x):
     return None
 
 
-
-
 class Norm(eqx.Module):
     """Normalization layer.
 
     Args:
-        stats: Einstein string determining the axes along which mean and variance are computed. Will be passed to ``einx.reduce``.
-        params: Einstein string determining the axes along which learnable parameters are applied. Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
+        stats: Einstein string determining the axes along which mean and variance are computed.
+            Will be passed to ``einx.reduce``.
+        params: Einstein string determining the axes along which learnable parameters are applied.
+            Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
         mean: Whether to apply mean normalization. Defaults to ``True``.
         var: Whether to apply variance normalization. Defaults to ``True``.
         scale: Whether to apply a learnable scale according to ``params``. Defaults to ``True``.
         bias: Whether to apply a learnable bias according to ``params``. Defaults to ``True``.
-        epsilon: A small float added to the variance to avoid division by zero. Defaults to ``1e-5``.
+        epsilon: A small float added to the variance to avoid division by zero. Defaults
+            to ``1e-5``.
         fastvar: Whether to use a fast variance computation. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
-        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``, no moving average is applied. Defaults to ``None``.
+        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``,
+            no moving average is applied. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
     stats: str
     params: str
     mean: bool
     var: bool
@@ -83,16 +107,29 @@
     bias: Optional[jax.Array]
     decay_rate: Optional[float]
     epsilon: float
     fastvar: bool
     dtype: str
     kwargs: dict
 
-    def __init__(self, stats: str, params: str = "b... [c]", mean: bool = True, var: bool = True, scale: bool = True, bias: bool = True, decay_rate: Optional[float] = None, epsilon: float = 1e-5, fastvar: bool = True, dtype: Any = "float32", **kwargs: Any):
-        if not decay_rate is None:
+    def __init__(
+        self,
+        stats: str,
+        params: str = "b... [c]",
+        mean: bool = True,
+        var: bool = True,
+        scale: bool = True,
+        bias: bool = True,
+        decay_rate: Optional[float] = None,
+        epsilon: float = 1e-5,
+        fastvar: bool = True,
+        dtype: Any = "float32",
+        **kwargs: Any,
+    ):
+        if decay_rate is not None:
             raise ValueError("Stateful layers are currently not supported in Equinox")
         self.stats = stats
         self.params = params
         self.mean = mean
         self.var = var
         self.use_scale = scale
         self.use_bias = bias
@@ -101,33 +138,35 @@
         self.decay_rate = decay_rate
         self.epsilon = epsilon
         self.fastvar = fastvar
         self.dtype = dtype
         self.kwargs = kwargs
 
     def __call__(self, x, rng=None):
-        x, mean, var = einx.nn.norm(
+        x, _mean, _var = einx.nn.norm(
             x,
             self.stats,
             self.params,
             mean=self.mean,
             var=self.var,
             scale=param(self, name="scale", rng=rng) if self.use_scale else None,
             bias=param(self, name="bias", rng=rng) if self.use_bias else None,
             epsilon=self.epsilon,
             fastvar=self.fastvar,
             **self.kwargs,
         )
         return x
 
+
 class Linear(eqx.Module):
     """Linear layer.
 
     Args:
-        expr: Einstein string determining the axes along which the weight matrix is multiplied. Will be passed to ``einx.dot``.
+        expr: Einstein string determining the axes along which the weight matrix is multiplied.
+            Will be passed to ``einx.dot``.
         bias: Whether to apply a learnable bias. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
     expr: str
     weight: jax.Array
@@ -142,26 +181,29 @@
         self.bias = None
         self.kwargs = kwargs
 
     def __call__(self, x, rng=None):
         return einx.nn.linear(
             x,
             self.expr,
-            bias=param(self, name="bias", rng=rng) if not self.use_bias is None else None,
+            bias=param(self, name="bias", rng=rng) if self.use_bias is not None else None,
             weight=param(self, name="weight", rng=rng),
             **self.kwargs,
         )
 
+
 class Dropout(eqx.Module):
     """Dropout layer.
 
     Args:
-        expr: Einstein string determining the axes along which dropout is applied. Will be passed to ``einx.elementwise``.
+        expr: Einstein string determining the axes along which dropout is applied. Will be
+            passed to ``einx.elementwise``.
         drop_rate: Drop rate.
-        inference: Whether the layer is used in inference mode (i.e. not apply dropout). Defaults to ``False``.
+        inference: Whether the layer is used in inference mode (i.e. not apply dropout). Defaults
+            to ``False``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
     expr: str
     drop_rate: float
     kwargs: dict
     inference: bool
```

### Comparing `einx-0.1.3/einx/nn/flax.py` & `einx-0.2.0/einx/nn/flax.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,113 @@
 import flax.linen as nn
-import einx, flax
+import einx
+import flax
 from functools import partial
 import jax.numpy as jnp
 from typing import Callable, Union, Optional, Any
 
-def param(bound_method: Union[Callable, nn.Module], name: Optional[str] = None, init: Optional[str] = None, dtype: Optional[nn.dtypes.Dtype] = None, col: Optional[str] = None):
+
+def param(
+    bound_method: Union[Callable, nn.Module],
+    name: Optional[str] = None,
+    init: Optional[Any] = None,
+    dtype: Optional[nn.dtypes.Dtype] = None,
+    col: Optional[str] = None,
+):
     """Create a tensor factory for Flax parameters.
 
     Args:
-        bound_method: The bound method of a Flax module, i.e. ``nn.Module.param`` or ``nn.Module.variable``, or a module instance in which case its ``param`` method
-                      is used.
-        name: Name of the parameter. If ``None``, uses a default name determined from the calling operation. Defaults to ``None``.
-        init: Initializer for the parameter. If ``None``, uses a default init method determined from the calling operation. Defaults to ``None``.
-        dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling module or ``float32`` if it does not exist. Defaults to ``None``.
+        bound_method: The bound method of a Flax module, i.e. ``nn.Module.param`` or
+            ``nn.Module.variable``, or a module instance in which case its ``param`` method
+            is used.
+        name: Name of the parameter. If ``None``, uses a default name determined from the calling
+            operation. Defaults to ``None``.
+        init: Initializer for the parameter. If ``None``, uses a default init method determined
+            from the calling operation. Defaults to ``None``.
+        dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling
+            module or ``float32`` if it does not exist. Defaults to ``None``.
         col: The collection name to use when ``bound_method`` is ``nn.Module.variable``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
     if isinstance(bound_method, nn.Module):
         bound_method = bound_method.param
 
+    name0 = name
+    init0 = init
+    dtype0 = dtype
+
     def flax_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
+        if name0 is not None:
+            name = name0
+        if init0 is not None:
+            init = init0
+        if dtype0 is not None:
+            dtype = dtype0
+
         if name is None:
-            raise ValueError("Must specify name for tensor factory flax.linen.Module.{param|variable}")
+            raise ValueError(
+                "Must specify name for tensor factory flax.linen.Module.{param|variable}"
+            )
 
         if init is None:
-            raise ValueError("Must specify init for tensor factory flax.linen.Module.{param|variable}")
+            raise ValueError(
+                "Must specify init for tensor factory flax.linen.Module.{param|variable}"
+            )
         elif isinstance(init, str):
             if init == "get_at" or init == "rearrange":
                 init = nn.initializers.normal(stddev=0.02)
             elif init == "add":
                 init = nn.initializers.zeros_init()
             elif init == "multiply":
                 init = nn.initializers.ones_init()
             elif init == "dot":
-                init = nn.initializers.lecun_normal(kwargs["in_axis"], kwargs["out_axis"], kwargs["batch_axis"])
+                init = nn.initializers.lecun_normal(
+                    kwargs["in_axis"], kwargs["out_axis"], kwargs["batch_axis"]
+                )
             else:
                 raise ValueError(f"Don't know which initializer to use for operation '{init}'")
         elif isinstance(init, (int, float)):
             init = nn.initializers.constant(init, dtype=dtype)
 
         if dtype is None:
             module = bound_method.__self__
             if hasattr(module, "dtype"):
                 dtype = module.dtype
             else:
                 dtype = "float32"
 
         if bound_method.__func__ == nn.Module.param:
-            if not col is None:
+            if col is not None:
                 raise ValueError("col is not accepted for flax.linen.Module.param")
             return bound_method(name, init, shape, dtype)
         elif bound_method.__func__ == nn.Module.variable:
             if col is None:
                 raise ValueError("col must be specified for flax.linen.Module.variable")
             # Assume that variable initialization does not need an rng key by passing None:
             return bound_method(col, name, init, None, shape, dtype).value
         else:
-            raise ValueError(f"Unknown tensor factory flax.linen.Module.{bound_method.__func__.__name__}")
+            raise ValueError(
+                f"Unknown tensor factory flax.linen.Module.{bound_method.__func__.__name__}"
+            )
+
     return flax_param_factory
 
+
 def to_tensor_factory(x):
     if isinstance(x, nn.Module) or (hasattr(x, "__func__") and x.__func__ == nn.Module.param):
         return param(x)
     else:
         return None
 
 
+# Using _ prefix on classes and a separater constructor, since dataclass/nn.Module does
+# not support **kwargs parameter.
 
-# Using _ prefix on classes and a separater constructor, since dataclass/nn.Module does not support **kwargs parameter.
 
 class _Norm(nn.Module):
     stats: str
     params: str = "b... [c]"
     mean: bool = True
     var: bool = True
     scale: bool = True
@@ -82,115 +116,169 @@
     epsilon: float = 1e-5
     fastvar: bool = True
     dtype: nn.dtypes.Dtype = "float32"
     kwargs: dict = None
 
     @nn.compact
     def __call__(self, x, training=None):
-        if not self.decay_rate is None and training is None:
+        if self.decay_rate is not None and training is None:
             raise ValueError("training must be specified when decay_rate is used")
 
-        use_ema = not self.decay_rate is None and (not training or self.is_initializing())
+        use_ema = self.decay_rate is not None and (not training or self.is_initializing())
         x, mean, var = einx.nn.norm(
             x,
             self.stats,
             self.params,
-            mean=param(self.variable, col="stats", name="mean", dtype=self.dtype) if use_ema and self.mean else self.mean,
-            var=param(self.variable, col="stats", name="var", dtype=self.dtype) if use_ema and self.var else self.var,
+            mean=param(self.variable, col="stats", name="mean", dtype=self.dtype)
+            if use_ema and self.mean
+            else self.mean,
+            var=param(self.variable, col="stats", name="var", dtype=self.dtype)
+            if use_ema and self.var
+            else self.var,
             scale=param(self.param, name="scale", dtype=self.dtype) if self.scale else None,
             bias=param(self.param, name="bias", dtype=self.dtype) if self.bias else None,
             epsilon=self.epsilon,
             fastvar=self.fastvar,
-            **(self.kwargs if not self.kwargs is None else {}),
+            **(self.kwargs if self.kwargs is not None else {}),
         )
 
-        update_ema = not self.decay_rate is None and training and not self.is_initializing()
+        update_ema = self.decay_rate is not None and training and not self.is_initializing()
         if update_ema:
             if self.mean:
                 mean_ema = self.variable("stats", "mean", None)
                 mean_ema.value = self.decay_rate * mean_ema.value + (1 - self.decay_rate) * mean
             if self.var:
                 var_ema = self.variable("stats", "var", None)
                 var_ema.value = self.decay_rate * var_ema.value + (1 - self.decay_rate) * var
 
         return x
 
-def Norm(stats: str, params: str = "b... [c]", mean: bool = True, var: bool = True, scale: bool = True, bias: bool = True, decay_rate: Optional[float] = None, epsilon: float = 1e-5, fastvar: bool = True, dtype: nn.dtypes.Dtype = "float32", name: Optional[str] = None, **kwargs: Any):
+
+def Norm(
+    stats: str,
+    params: str = "b... [c]",
+    mean: bool = True,
+    var: bool = True,
+    scale: bool = True,
+    bias: bool = True,
+    decay_rate: Optional[float] = None,
+    epsilon: float = 1e-5,
+    fastvar: bool = True,
+    dtype: nn.dtypes.Dtype = "float32",
+    name: Optional[str] = None,
+    **kwargs: Any,
+):
     """Normalization layer.
 
     Args:
-        stats: Einstein string determining the axes along which mean and variance are computed. Will be passed to ``einx.reduce``.
-        params: Einstein string determining the axes along which learnable parameters are applied. Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
+        stats: Einstein string determining the axes along which mean and variance are computed.
+            Will be passed to ``einx.reduce``.
+        params: Einstein string determining the axes along which learnable parameters are applied.
+            Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
         mean: Whether to apply mean normalization. Defaults to ``True``.
         var: Whether to apply variance normalization. Defaults to ``True``.
         scale: Whether to apply a learnable scale according to ``params``. Defaults to ``True``.
         bias: Whether to apply a learnable bias according to ``params``. Defaults to ``True``.
-        epsilon: A small float added to the variance to avoid division by zero. Defaults to ``1e-5``.
+        epsilon: A small float added to the variance to avoid division by zero. Defaults
+            to ``1e-5``.
         fastvar: Whether to use a fast variance computation. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
-        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``, no moving average is applied. Defaults to ``None``.
+        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``,
+            no moving average is applied. Defaults to ``None``.
         name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    return _Norm(stats, params=params, mean=mean, var=var, scale=scale, bias=bias, decay_rate=decay_rate, epsilon=epsilon, fastvar=fastvar, dtype=dtype, name=name, kwargs=kwargs)
+    return _Norm(
+        stats,
+        params=params,
+        mean=mean,
+        var=var,
+        scale=scale,
+        bias=bias,
+        decay_rate=decay_rate,
+        epsilon=epsilon,
+        fastvar=fastvar,
+        dtype=dtype,
+        name=name,
+        kwargs=kwargs,
+    )
+
 
 class _Linear(nn.Module):
     expr: str
     bias: bool = True
     dtype: nn.dtypes.Dtype = "float32"
     kwargs: dict = None
 
     @nn.compact
     def __call__(self, x):
         return einx.nn.linear(
             x,
             self.expr,
             bias=param(self.param, name="bias", dtype=self.dtype) if self.bias else None,
             weight=param(self.param, name="weight", dtype=self.dtype),
-            **(self.kwargs if not self.kwargs is None else {}),
+            **(self.kwargs if self.kwargs is not None else {}),
         )
 
-def Linear(expr: str, bias: bool = True, dtype: nn.dtypes.Dtype = "float32", name: Optional[str] = None, **kwargs: Any):
+
+def Linear(
+    expr: str,
+    bias: bool = True,
+    dtype: nn.dtypes.Dtype = "float32",
+    name: Optional[str] = None,
+    **kwargs: Any,
+):
     """Linear layer.
 
     Args:
-        expr: Einstein string determining the axes along which the weight matrix is multiplied. Will be passed to ``einx.dot``.
+        expr: Einstein string determining the axes along which the weight matrix is
+            multiplied. Will be passed to ``einx.dot``.
         bias: Whether to apply a learnable bias. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
         name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
     return _Linear(expr, bias=bias, dtype=dtype, name=name, kwargs=kwargs)
 
+
 class _Dropout(nn.Module):
     expr: str
     drop_rate: float
     rng_collection: str = "dropout"
     kwargs: dict = None
 
     @nn.compact
     def __call__(self, x, training):
         if training:
             return einx.nn.dropout(
                 x,
                 self.expr,
                 drop_rate=self.drop_rate,
                 rng=self.make_rng(self.rng_collection),
-                **(self.kwargs if not self.kwargs is None else {}),
+                **(self.kwargs if self.kwargs is not None else {}),
             )
         else:
             return x
 
-def Dropout(expr: str, drop_rate: float, rng_collection: str = "dropout", name: Optional[str] = None, **kwargs: Any):
+
+def Dropout(
+    expr: str,
+    drop_rate: float,
+    rng_collection: str = "dropout",
+    name: Optional[str] = None,
+    **kwargs: Any,
+):
     """Dropout layer.
 
     Args:
-        expr: Einstein string determining the axes along which dropout is applied. Will be passed to ``einx.elementwise``.
+        expr: Einstein string determining the axes along which dropout is applied. Will be passed
+            to ``einx.elementwise``.
         drop_rate: Drop rate.
-        rng_collection: the rng collection name to use when requesting an rng key. Defaults to ``"dropout"``.
+        rng_collection: the rng collection name to use when requesting an rng key. Defaults
+            to ``"dropout"``.
         name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    return _Dropout(expr, drop_rate, rng_collection=rng_collection, name=name, kwargs=kwargs)
+    return _Dropout(expr, drop_rate, rng_collection=rng_collection, name=name, kwargs=kwargs)
```

### Comparing `einx-0.1.3/einx/nn/haiku.py` & `einx-0.2.0/einx/nn/keras.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,168 +1,257 @@
-import haiku as hk
+import keras
 import einx
-from functools import partial
-from haiku._src.base import current_module
-from typing import Any, Callable, Literal, Optional
-
-def param(func: Literal[hk.get_parameter, hk.get_state] = hk.get_parameter, name: Optional[str] = None, init: Optional[Callable] = None, dtype: Optional[Any] = None):
-    """Create a tensor factory for Haiku parameters.
+import inspect
+import numpy as np
+from typing import Any, Callable, Optional
+
+_version = tuple(int(i) for i in keras.__version__.split(".")[:2])
+if _version < (3, 0):
+    raise ImportError(f"einx.nn.keras requires Keras version >= 3, but found {keras.__version__}")
+
+
+def param(
+    layer: keras.layers.Layer,
+    name: Optional[str] = None,
+    init: Optional[Any] = None,
+    dtype: Optional[Any] = None,
+    trainable: bool = True,
+):
+    """Create a tensor factory for Keras parameters.
 
     Args:
-        func: Either ``hk.get_parameter`` or ``hk.get_state``. Defaults to ``hk.get_parameter``.
-        name: Name of the parameter. If ``None``, uses a default name determined from the calling operation. Defaults to ``None``.
-        init: Initializer for the parameter. If ``None``, uses a default init method determined from the calling operation. Defaults to ``None``.
-        dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling module or ``float32`` if it does not exist. Defaults to ``None``.
+        layer: The layer to create the parameter in. Must be an instance of ``keras.layers.Layer``.
+        name: Name of the parameter. If ``None``, uses a default name determined from the
+            calling operation. Defaults to ``None``.
+        init: Initializer for the parameter. If ``None``, uses a default init method determined
+            from the calling operation. Defaults to ``None``.
+        dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling
+            module or ``float32`` if it does not exist. Defaults to ``None``.
+        trainable: Whether the parameter is trainable. Defaults to ``True``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
 
-    def haiku_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
+    name0 = name
+    init0 = init
+    dtype0 = dtype
+
+    def keras_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
+        if name0 is not None:
+            name = name0
+        if init0 is not None:
+            init = init0
+        if dtype0 is not None:
+            dtype = dtype0
+
         if name is None:
-            raise ValueError("Must specify name for tensor factory hk.get_{parameter|state}")
+            raise ValueError("Must specify name for tensor factory keras.layers.Layer")
+
+        if dtype is None:
+            if hasattr(layer, "dtype"):
+                dtype = layer.dtype
+            else:
+                dtype = "float32"
 
         if init is None:
-            raise ValueError("Must specify init for tensor factory hk.get_{parameter|state}")
+            raise ValueError("Must specify init for tensor factory keras.layers.Layer")
         elif isinstance(init, str):
-            if init in "get_at" or init == "rearrange":
-                init = hk.initializers.RandomNormal(stddev=0.02)
+            if init == "get_at" or init == "rearrange":
+                init = keras.initializers.TruncatedNormal(stddev=0.02)
             elif init == "add":
-                init = hk.initializers.Constant(0.0)
+                init = keras.initializers.Constant(0.0)
             elif init == "multiply":
-                init = hk.initializers.Constant(1.0)
+                init = keras.initializers.Constant(1.0)
             elif init == "dot":
-                init = hk.initializers.VarianceScaling(1.0, "fan_in", "truncated_normal", fan_in_axes=kwargs["in_axis"])
+                fan_in = np.prod([shape[i] for i in kwargs["in_axis"]])
+                std = np.sqrt(1.0 / fan_in) / 0.87962566103423978
+                init = keras.initializers.TruncatedNormal(mean=0.0, stddev=std)
             else:
                 raise ValueError(f"Don't know which initializer to use for operation '{init}'")
         elif isinstance(init, (int, float)):
-            init = hk.initializers.Constant(init)
+            init = keras.initializers.Constant(init)
 
-        if dtype is None:
-            module = current_module()
-            if hasattr(module, "dtype"):
-                dtype = module.dtype
-            else:
-                dtype = "float32"
+        if name in vars(layer):
+            tensor = vars(layer)[name]
+        else:
+            tensor = vars(layer)[name] = layer.add_weight(
+                shape=shape,
+                dtype=dtype,
+                initializer=init,
+                name=name,
+                trainable=trainable,
+            )
+        return tensor
+
+    return keras_param_factory
 
-        return func(shape=shape, name=name, dtype=dtype, init=init)
-    return haiku_param_factory
 
 def to_tensor_factory(x):
-    if id(x) == id(hk.get_parameter) or id(x) == id(hk.get_state):
-        return param(x)
-    else:
-        return None
+    return None
+
+
+def einx_backend_for_keras():
+    return einx.backend.get(keras.config.backend())
+
 
-class Norm(hk.Module):
+def is_leaf(x):
+    return isinstance(x, tuple) and all(isinstance(y, int) for y in x)
+
+
+class Layer(keras.layers.Layer):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def build(self, inputs_shape):
+        backend = einx_backend_for_keras()
+        tracers = einx.tree_util.tree_map(
+            lambda shape: backend.zeros(shape=shape, dtype="float32"), inputs_shape, is_leaf=is_leaf
+        )
+
+        if "is_initializing" in inspect.signature(self.call).parameters:
+            self.call(tracers, is_initializing=True)
+        else:
+            self.call(tracers)
+
+
+class Norm(Layer):
     """Normalization layer.
 
     Args:
-        stats: Einstein string determining the axes along which mean and variance are computed. Will be passed to ``einx.reduce``.
-        params: Einstein string determining the axes along which learnable parameters are applied. Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
+        stats: Einstein string determining the axes along which mean and variance are computed.
+            Will be passed to ``einx.reduce``.
+        params: Einstein string determining the axes along which learnable parameters are applied.
+            Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
         mean: Whether to apply mean normalization. Defaults to ``True``.
         var: Whether to apply variance normalization. Defaults to ``True``.
         scale: Whether to apply a learnable scale according to ``params``. Defaults to ``True``.
         bias: Whether to apply a learnable bias according to ``params``. Defaults to ``True``.
-        epsilon: A small float added to the variance to avoid division by zero. Defaults to ``1e-5``.
+        epsilon: A small float added to the variance to avoid division by zero. Defaults
+            to ``1e-5``.
         fastvar: Whether to use a fast variance computation. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
-        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``, no moving average is applied. Defaults to ``None``.
-        name: Name of the module. Defaults to ``None``.
+        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``,
+            no moving average is applied. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(self, stats: str, params: str = "b... [c]", mean: bool = True, var: bool = True, scale: bool = True, bias: bool = True, epsilon: float = 1e-5, fastvar: bool = True, dtype: Any = "float32", decay_rate: Optional[float] = None, name: Optional[str] = None, **kwargs: Any):
-        super().__init__(name=name)
+    def __init__(
+        self,
+        stats: str,
+        params: str = "b... [c]",
+        mean: bool = True,
+        var: bool = True,
+        scale: bool = True,
+        bias: bool = True,
+        epsilon: float = 1e-5,
+        fastvar: bool = True,
+        dtype: Any = "float32",
+        decay_rate: Optional[float] = None,
+        **kwargs: Any,
+    ):
+        super().__init__(dtype=dtype)
         self.stats = stats
         self.params = params
-        self.mean = mean
-        self.var = var
-        self.scale = scale
-        self.bias = bias
+        self.use_mean = mean
+        self.use_var = var
+        self.use_scale = scale
+        self.use_bias = bias
         self.epsilon = epsilon
         self.fastvar = fastvar
-        self.dtype = dtype
         self.decay_rate = decay_rate
         self.kwargs = kwargs
 
-    def __call__(self, x, training=None):
-        if not self.decay_rate is None and training is None:
-            raise ValueError("training must be specified when decay_rate is used")
-
-        use_ema = not self.decay_rate is None and (not training or hk.running_init())
+    def call(self, x, training=None, is_initializing=False):
+        use_ema = self.decay_rate is not None and (not training or is_initializing)
         x, mean, var = einx.nn.norm(
             x,
             self.stats,
             self.params,
-            mean=param(hk.get_state, name="mean") if use_ema and self.mean else self.mean,
-            var=param(hk.get_state, name="var") if use_ema and self.var else self.var,
-            scale=param(hk.get_parameter, name="scale") if self.scale else None,
-            bias=param(hk.get_parameter, name="bias") if self.bias else None,
+            mean=param(self, name="mean", trainable=False)
+            if use_ema and self.use_mean
+            else self.use_mean,
+            var=param(self, name="var", trainable=False)
+            if use_ema and self.use_var
+            else self.use_var,
+            scale=param(self, name="scale", trainable=True) if self.use_scale else None,
+            bias=param(self, name="bias", trainable=True) if self.use_bias else None,
             epsilon=self.epsilon,
             fastvar=self.fastvar,
-            **self.kwargs,
+            **(self.kwargs if self.kwargs is not None else {}),
         )
 
-        update_ema = not self.decay_rate is None and training and not hk.running_init()
+        update_ema = self.decay_rate is not None and training and not is_initializing
         if update_ema:
-            if self.mean:
-                hk.set_state("mean", hk.get_state("mean") * self.decay_rate + mean * (1 - self.decay_rate))
-            if self.var:
-                hk.set_state("var", hk.get_state("var") * self.decay_rate + var * (1 - self.decay_rate))
+            if self.use_mean:
+                self.mean.assign(
+                    keras.ops.cast(
+                        self.decay_rate * self.mean.value + (1 - self.decay_rate) * mean,
+                        self.mean.dtype,
+                    )
+                )
+            if self.use_var:
+                self.var.assign(
+                    keras.ops.cast(
+                        self.decay_rate * self.var.value + (1 - self.decay_rate) * var,
+                        self.var.dtype,
+                    )
+                )
 
         return x
 
-class Linear(hk.Module):
+
+class Linear(Layer):
     """Linear layer.
 
     Args:
-        expr: Einstein string determining the axes along which the weight matrix is multiplied. Will be passed to ``einx.dot``.
+        expr: Einstein string determining the axes along which the weight matrix is multiplied.
+            Will be passed to ``einx.dot``.
         bias: Whether to apply a learnable bias. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
-        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(self, expr: str, bias: bool = True, dtype: Any = "float32", name: Optional[str] = None, **kwargs: Any):
-        super().__init__(name=name)
+    def __init__(self, expr: str, bias: bool = True, dtype: Any = "float32", **kwargs: Any):
+        super().__init__(dtype=dtype)
+
         self.expr = expr
-        self.bias = bias
-        self.dtype = dtype
+        self.use_bias = bias
         self.kwargs = kwargs
 
-    def __call__(self, x):
+    def call(self, x):
         return einx.nn.linear(
             x,
             self.expr,
-            bias=param(hk.get_parameter, name="bias") if self.bias else None,
-            weight=param(hk.get_parameter, name="weight"),
+            bias=param(self, name="bias") if self.use_bias else None,
+            weight=param(self, name="weight"),
             **self.kwargs,
         )
 
-class Dropout(hk.Module):
+
+class Dropout(Layer):
     """Dropout layer.
 
     Args:
-        expr: Einstein string determining the axes along which dropout is applied. Will be passed to ``einx.elementwise``.
+        expr: Einstein string determining the axes along which dropout is applied. Will be
+            passed to ``einx.elementwise``.
         drop_rate: Drop rate.
-        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(self, expr: str, drop_rate: float, name: Optional[str] = None, **kwargs: Any):
-        super().__init__(name=name)
+    def __init__(self, expr: str, drop_rate: float, **kwargs: Any):
+        super().__init__()
+
         self.expr = expr
         self.drop_rate = drop_rate
         self.kwargs = kwargs
 
-    def __call__(self, x, training):
+    def call(self, x, training=None):
         if training:
             return einx.nn.dropout(
                 x,
                 self.expr,
                 drop_rate=self.drop_rate,
-                rng=hk.next_rng_key(),
                 **self.kwargs,
             )
         else:
-            return x
+            return x
```

### Comparing `einx-0.1.3/einx/nn/keras.py` & `einx-0.2.0/einx/nn/haiku.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,202 +1,226 @@
-import keras, einx, inspect
-import numpy as np
-from typing import Any, Callable, Optional
-
-_version = tuple(int(i) for i in keras.__version__.split(".")[:2])
-if _version < (3, 0):
-    raise ImportError(f"einx.nn.keras requires Keras version >= 3, but found {keras.__version__}")
+import haiku as hk
+import einx
+from functools import partial
+from haiku._src.base import current_module
+from typing import Any, Callable, Literal, Optional
 
-def param(layer: keras.layers.Layer, name: Optional[str] = None, init: Optional[Callable] = None, dtype: Optional[Any] = None, trainable: bool = True):
-    """Create a tensor factory for Keras parameters.
+
+def param(
+    func: Literal[hk.get_parameter, hk.get_state] = hk.get_parameter,
+    name: Optional[str] = None,
+    init: Optional[Any] = None,
+    dtype: Optional[Any] = None,
+):
+    """Create a tensor factory for Haiku parameters.
 
     Args:
-        layer: The layer to create the parameter in. Must be an instance of ``keras.layers.Layer``.
-        name: Name of the parameter. If ``None``, uses a default name determined from the calling operation. Defaults to ``None``.
-        init: Initializer for the parameter. If ``None``, uses a default init method determined from the calling operation. Defaults to ``None``.
-        dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling module or ``float32`` if it does not exist. Defaults to ``None``.
-        trainable: Whether the parameter is trainable. Defaults to ``True``.
+        func: Either ``hk.get_parameter`` or ``hk.get_state``. Defaults to ``hk.get_parameter``.
+        name: Name of the parameter. If ``None``, uses a default name determined from the calling
+            operation. Defaults to ``None``.
+        init: Initializer for the parameter. If ``None``, uses a default init method determined
+            from the calling operation. Defaults to ``None``.
+        dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling
+            module or ``float32`` if it does not exist. Defaults to ``None``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
 
-    def keras_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
-        if name is None:
-            raise ValueError("Must specify name for tensor factory keras.layers.Layer")
+    name0 = name
+    init0 = init
+    dtype0 = dtype
+
+    def haiku_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
+        if name0 is not None:
+            name = name0
+        if init0 is not None:
+            init = init0
+        if dtype0 is not None:
+            dtype = dtype0
 
-        if dtype is None:
-            if hasattr(layer, "dtype"):
-                dtype = layer.dtype
-            else:
-                dtype = "float32"
+        if name is None:
+            raise ValueError("Must specify name for tensor factory hk.get_{parameter|state}")
 
         if init is None:
-            raise ValueError("Must specify init for tensor factory keras.layers.Layer")
+            raise ValueError("Must specify init for tensor factory hk.get_{parameter|state}")
         elif isinstance(init, str):
-            if init == "get_at" or init == "rearrange":
-                init = keras.initializers.TruncatedNormal(stddev=0.02)
+            if init in "get_at" or init == "rearrange":
+                init = hk.initializers.RandomNormal(stddev=0.02)
             elif init == "add":
-                init = keras.initializers.Constant(0.0)
+                init = hk.initializers.Constant(0.0)
             elif init == "multiply":
-                init = keras.initializers.Constant(1.0)
+                init = hk.initializers.Constant(1.0)
             elif init == "dot":
-                fan_in = np.prod([shape[i] for i in kwargs["in_axis"]])
-                std = np.sqrt(1.0 / fan_in) / .87962566103423978
-                init = keras.initializers.TruncatedNormal(mean=0.0, stddev=std)
+                init = hk.initializers.VarianceScaling(
+                    1.0, "fan_in", "truncated_normal", fan_in_axes=kwargs["in_axis"]
+                )
             else:
                 raise ValueError(f"Don't know which initializer to use for operation '{init}'")
         elif isinstance(init, (int, float)):
-            init = keras.initializers.Constant(init)
-
-        if name in vars(layer):
-            tensor = vars(layer)[name]
-        else:
-            tensor = vars(layer)[name] = layer.add_weight(
-                shape=shape,
-                dtype=dtype,
-                initializer=init,
-                name=name,
-                trainable=trainable,
-            )
-        return tensor
-    return keras_param_factory
-
-def to_tensor_factory(x):
-    return None
-
+            init = hk.initializers.Constant(init)
 
+        if dtype is None:
+            module = current_module()
+            if hasattr(module, "dtype"):
+                dtype = module.dtype
+            else:
+                dtype = "float32"
 
-def einx_backend_for_keras():
-    return einx.backend.get(keras.config.backend())
+        return func(shape=shape, name=name, dtype=dtype, init=init)
 
-def is_leaf(x):
-    return isinstance(x, tuple) and all([isinstance(y, int) for y in x])
+    return haiku_param_factory
 
-class Layer(keras.layers.Layer):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
 
-    def build(self, inputs_shape):
-        backend = einx_backend_for_keras()
-        tracers = einx.tree_util.tree_map(lambda shape: backend.zeros(shape=shape, dtype="float32"), inputs_shape, is_leaf=is_leaf)
+def to_tensor_factory(x):
+    if id(x) == id(hk.get_parameter) or id(x) == id(hk.get_state):
+        return param(x)
+    else:
+        return None
 
-        if "is_initializing" in inspect.signature(self.call).parameters:
-            self.call(tracers, is_initializing=True)
-        else:
-            self.call(tracers)
 
-class Norm(Layer):
+class Norm(hk.Module):
     """Normalization layer.
 
     Args:
-        stats: Einstein string determining the axes along which mean and variance are computed. Will be passed to ``einx.reduce``.
-        params: Einstein string determining the axes along which learnable parameters are applied. Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
+        stats: Einstein string determining the axes along which mean and variance are computed.
+            Will be passed to ``einx.reduce``.
+        params: Einstein string determining the axes along which learnable parameters are
+            applied. Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
         mean: Whether to apply mean normalization. Defaults to ``True``.
         var: Whether to apply variance normalization. Defaults to ``True``.
         scale: Whether to apply a learnable scale according to ``params``. Defaults to ``True``.
         bias: Whether to apply a learnable bias according to ``params``. Defaults to ``True``.
-        epsilon: A small float added to the variance to avoid division by zero. Defaults to ``1e-5``.
+        epsilon: A small float added to the variance to avoid division by zero. Defaults
+            to ``1e-5``.
         fastvar: Whether to use a fast variance computation. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
-        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``, no moving average is applied. Defaults to ``None``.
+        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``,
+            no moving average is applied. Defaults to ``None``.
+        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
-    def __init__(self, stats: str, params: str = "b... [c]", mean: bool = True, var: bool = True, scale: bool = True, bias: bool = True, epsilon: float = 1e-5, fastvar: bool = True, dtype: Any = "float32", decay_rate: Optional[float] = None, **kwargs: Any):
-        super().__init__(dtype=dtype)
+
+    def __init__(
+        self,
+        stats: str,
+        params: str = "b... [c]",
+        mean: bool = True,
+        var: bool = True,
+        scale: bool = True,
+        bias: bool = True,
+        epsilon: float = 1e-5,
+        fastvar: bool = True,
+        dtype: Any = "float32",
+        decay_rate: Optional[float] = None,
+        name: Optional[str] = None,
+        **kwargs: Any,
+    ):
+        super().__init__(name=name)
         self.stats = stats
         self.params = params
-        self.use_mean = mean
-        self.use_var = var
-        self.use_scale = scale
-        self.use_bias = bias
+        self.mean = mean
+        self.var = var
+        self.scale = scale
+        self.bias = bias
         self.epsilon = epsilon
         self.fastvar = fastvar
+        self.dtype = dtype
         self.decay_rate = decay_rate
         self.kwargs = kwargs
 
-    def call(self, x, training=None, is_initializing=False):
-        use_ema = not self.decay_rate is None and (not training or is_initializing)
+    def __call__(self, x, training=None):
+        if self.decay_rate is not None and training is None:
+            raise ValueError("training must be specified when decay_rate is used")
+
+        use_ema = self.decay_rate is not None and (not training or hk.running_init())
         x, mean, var = einx.nn.norm(
             x,
             self.stats,
             self.params,
-            mean=param(self, name="mean", trainable=False) if use_ema and self.use_mean else self.use_mean,
-            var=param(self, name="var", trainable=False) if use_ema and self.use_var else self.use_var,
-            scale=param(self, name="scale", trainable=True) if self.use_scale else None,
-            bias=param(self, name="bias", trainable=True) if self.use_bias else None,
+            mean=param(hk.get_state, name="mean") if use_ema and self.mean else self.mean,
+            var=param(hk.get_state, name="var") if use_ema and self.var else self.var,
+            scale=param(hk.get_parameter, name="scale") if self.scale else None,
+            bias=param(hk.get_parameter, name="bias") if self.bias else None,
             epsilon=self.epsilon,
             fastvar=self.fastvar,
-            **(self.kwargs if not self.kwargs is None else {}),
+            **self.kwargs,
         )
 
-        update_ema = not self.decay_rate is None and training and not is_initializing
+        update_ema = self.decay_rate is not None and training and not hk.running_init()
         if update_ema:
-            if self.use_mean:
-                self.mean.assign(
-                    keras.ops.cast(
-                        self.decay_rate * self.mean.value + (1 - self.decay_rate) * mean,
-                        self.mean.dtype,
-                    )
+            if self.mean:
+                hk.set_state(
+                    "mean", hk.get_state("mean") * self.decay_rate + mean * (1 - self.decay_rate)
                 )
-            if self.use_var:
-                self.var.assign(
-                    keras.ops.cast(
-                        self.decay_rate * self.var.value + (1 - self.decay_rate) * var,
-                        self.var.dtype,
-                    )
+            if self.var:
+                hk.set_state(
+                    "var", hk.get_state("var") * self.decay_rate + var * (1 - self.decay_rate)
                 )
 
         return x
 
-class Linear(Layer):
+
+class Linear(hk.Module):
     """Linear layer.
 
     Args:
-        expr: Einstein string determining the axes along which the weight matrix is multiplied. Will be passed to ``einx.dot``.
+        expr: Einstein string determining the axes along which the weight matrix is multiplied.
+            Will be passed to ``einx.dot``.
         bias: Whether to apply a learnable bias. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
+        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(self, expr: str, bias: bool = True, dtype: Any = "float32", **kwargs: Any):
-        super().__init__(dtype=dtype)
-
+    def __init__(
+        self,
+        expr: str,
+        bias: bool = True,
+        dtype: Any = "float32",
+        name: Optional[str] = None,
+        **kwargs: Any,
+    ):
+        super().__init__(name=name)
         self.expr = expr
-        self.use_bias = bias
+        self.bias = bias
+        self.dtype = dtype
         self.kwargs = kwargs
 
-    def call(self, x):
+    def __call__(self, x):
         return einx.nn.linear(
             x,
             self.expr,
-            bias=param(self, name="bias") if self.use_bias else None,
-            weight=param(self, name="weight"),
+            bias=param(hk.get_parameter, name="bias") if self.bias else None,
+            weight=param(hk.get_parameter, name="weight"),
             **self.kwargs,
         )
 
-class Dropout(Layer):
+
+class Dropout(hk.Module):
     """Dropout layer.
 
     Args:
-        expr: Einstein string determining the axes along which dropout is applied. Will be passed to ``einx.elementwise``.
+        expr: Einstein string determining the axes along which dropout is applied. Will be
+            passed to ``einx.elementwise``.
         drop_rate: Drop rate.
+        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(self, expr: str, drop_rate: float, **kwargs: Any):
-        super().__init__()
-
+    def __init__(self, expr: str, drop_rate: float, name: Optional[str] = None, **kwargs: Any):
+        super().__init__(name=name)
         self.expr = expr
         self.drop_rate = drop_rate
         self.kwargs = kwargs
 
-    def call(self, x, training=None):
+    def __call__(self, x, training):
         if training:
             return einx.nn.dropout(
                 x,
                 self.expr,
                 drop_rate=self.drop_rate,
+                rng=hk.next_rng_key(),
                 **self.kwargs,
             )
         else:
-            return x
+            return x
```

### Comparing `einx-0.1.3/einx/nn/nn.py` & `einx-0.2.0/einx/nn/nn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,69 @@
 import einx
 from typing import Union, Optional, Any
 
-@einx.lru_cache(trace=lambda t, c: lambda x, stats, params="b... [c]", mean=True, var=True, scale=None, bias=None, epsilon=0, fastvar=True, backend=None, **kwargs:
-    c(t(x), stats, params, t(mean) if not isinstance(mean, bool) and not mean is None else mean, t(var) if not isinstance(var, bool) and not var is None else var,
-        t(scale) if not scale is None else scale, t(bias) if not bias is None else bias, epsilon, fastvar, **kwargs))
-def norm(x: einx.Tensor, stats: str, params: str = "b... [c]", mean: Union[einx.Tensor, bool] = True, var: Union[einx.Tensor, bool] = True, scale: Optional[einx.Tensor] = None, bias: Optional[einx.Tensor] = None, epsilon: float = 0, fastvar: bool = True, backend: Union[einx.Backend, str, None] = None, **kwargs: Any):
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda x,
+    stats,
+    params="b... [c]",
+    mean=True,
+    var=True,
+    scale=None,
+    bias=None,
+    epsilon=0,
+    fastvar=True,
+    backend=None,
+    **kwargs: c(
+        t(x),
+        stats,
+        params,
+        t(mean) if not isinstance(mean, bool) and mean is not None else mean,
+        t(var) if not isinstance(var, bool) and var is not None else var,
+        t(scale) if scale is not None else scale,
+        t(bias) if bias is not None else bias,
+        epsilon,
+        fastvar,
+        **kwargs,
+    )
+)
+def norm(
+    x: einx.Tensor,
+    stats: str,
+    params: str = "b... [c]",
+    mean: Union[einx.Tensor, bool] = True,
+    var: Union[einx.Tensor, bool] = True,
+    scale: Optional[einx.Tensor] = None,
+    bias: Optional[einx.Tensor] = None,
+    epsilon: float = 0,
+    fastvar: bool = True,
+    backend: Union[einx.Backend, str, None] = None,
+    **kwargs: Any,
+):
     if mean is None or var is None:
         raise ValueError("mean and var cannot be None")
     if backend is None:
-        backend = einx.backend.get([x, mean if not isinstance(mean, bool) else None, var if not isinstance(var, bool) else None, scale, bias])
+        backend = einx.backend.get([
+            x,
+            mean if not isinstance(mean, bool) else None,
+            var if not isinstance(var, bool) else None,
+            scale,
+            bias,
+        ])
     elif isinstance(backend, str):
         backend = einx.backend.get(backend)
 
     expr_in, expr_stats = einx.reduce.parse(stats, einx.param.get_shape(x), **kwargs)
     expr_in = einx.expr.stage3.demark(expr_in)
     expr_stats = einx.expr.stage3.demark(expr_stats)
 
     # Instantiate moving averages
-    if not isinstance(mean, bool) and not mean is None:
+    if not isinstance(mean, bool) and mean is not None:
         mean = einx.param.instantiate(mean, shape=expr_stats.shape, backend=backend, init="add")
-    if not isinstance(var, bool) and not var is None:
+    if not isinstance(var, bool) and var is not None:
         var = einx.param.instantiate(var, shape=expr_stats.shape, backend=backend, init="multiply")
 
     # Compute mean and variance
     if isinstance(mean, bool):
         if mean:
             mean = einx.mean(stats, x, **kwargs)
         else:
@@ -40,54 +80,70 @@
                     var = backend.maximum(var, 0)
                 else:
                     var = einx.var(stats, x, **kwargs)
         else:
             var = None
 
     # Normalize mean and variance
-    if not mean is None:
+    if mean is not None:
         x, _ = einx.subtract_stage3([expr_in, expr_stats], [x, mean], expr_in)
-    if not var is None:
+    if var is not None:
         inv_std = backend.rsqrt(var + epsilon)
         x, _ = einx.multiply_stage3([expr_in, expr_stats], [x, inv_std], expr_in)
 
     # Apply scale and bias
-    if not scale is None:
+    if scale is not None:
         x = einx.multiply(params, x, scale, **kwargs)
-    if not bias is None:
+    if bias is not None:
         x = einx.add(params, x, bias, **kwargs)
 
     return x, mean, var
 
-@einx.lru_cache(trace=lambda t, c: lambda x, expr, weight, bias=None, **kwargs:
-    c(t(x), expr, t(weight), t(bias) if not bias is None else None, **kwargs))
-def linear(x: einx.Tensor, expr: str, weight: einx.Tensor, bias: Optional[einx.Tensor], **kwargs: Any):
-    (expr_in1, expr_in2), expr_afterdot = einx.dot.parse(expr, einx.param.get_shape(x), einx.param.get_shape(weight), **kwargs)
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda x, expr, weight, bias=None, **kwargs: c(
+        t(x), expr, t(weight), t(bias) if bias is not None else None, **kwargs
+    )
+)
+def linear(
+    x: einx.Tensor, expr: str, weight: einx.Tensor, bias: Optional[einx.Tensor], **kwargs: Any
+):
+    (_expr_in1, expr_in2), expr_afterdot = einx.dot.parse(
+        expr, einx.param.get_shape(x), einx.param.get_shape(weight), **kwargs
+    )
 
     # Weight matrix multiplication
     x = einx.dot(expr, x, weight, **kwargs)
 
-    if not bias is None:
+    if bias is not None:
         # Bias expression includes all axes in output that are also in weight matrix
-        weight_axes_names = set(a.name for a in expr_in2.all() if isinstance(a, einx.expr.stage3.Axis))
+        weight_axes_names = {a.name for a in expr_in2.all() if isinstance(a, einx.expr.stage3.Axis)}
         expr_bias = []
         for a in expr_afterdot.all():
             if isinstance(a, einx.expr.stage3.Axis) and a.name in weight_axes_names:
                 expr_bias.append(a.__deepcopy__())
         expr_bias = einx.expr.stage3.List(expr_bias)
 
         x, _ = einx.add_stage3([expr_afterdot, expr_bias], [x, bias], expr_afterdot)
 
     return x
 
-@einx.lru_cache(trace=lambda t, c: lambda x, expr, drop_rate, rng=None, **kwargs:
-    c(t(x), expr, drop_rate, t(rng) if not rng is None else None, **kwargs))
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda x, expr, drop_rate, rng=None, **kwargs: c(
+        t(x), expr, drop_rate, t(rng) if rng is not None else None, **kwargs
+    )
+)
 def dropout(x: einx.Tensor, expr: str, drop_rate: float, rng: Any = None, **kwargs: Any):
     backend = einx.backend.get([x])
     keep_rate = 1 - drop_rate
 
-    (expr_in, expr_mask), expr_out = einx.elementwise.parse(expr, einx.param.get_shape(x), None, **kwargs)
+    (expr_in, expr_mask), expr_out = einx.elementwise.parse(
+        expr, einx.param.get_shape(x), None, **kwargs
+    )
 
     drop_mask = backend.random.bernoulli(rng=rng, p=keep_rate, shape=expr_mask.shape)
-    x, _ = einx.where_stage3([expr_mask, expr_in, einx.expr.stage3.List([])], [drop_mask, x, 0], expr_out)
+    x, _ = einx.where_stage3(
+        [expr_mask, expr_in, einx.expr.stage3.List([])], [drop_mask, x, 0], expr_out
+    )
 
     return x / keep_rate
```

### Comparing `einx-0.1.3/einx/nn/torch.py` & `einx-0.2.0/einx/nn/torch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,138 +1,185 @@
-import torch, einx, math
+import torch
+import einx
+import math
 from functools import partial
 import numpy as np
 from typing import Callable, Union, Optional, Any
 
 _version = tuple(int(i) for i in torch.__version__.split(".")[:2])
 if _version < (2, 0):
     raise ImportError(f"einx.nn.torch requires PyTorch version >= 2, but found {torch.__version__}")
 
+
 def _allow_in_graph(func):
     if "compiler" in dir(torch):
         return torch.compiler.allow_in_graph(func)
     else:
         import torch._dynamo as _dynamo
+
         return _dynamo.allow_in_graph(func)
 
-def param(uninitialized: Union[torch.nn.parameter.UninitializedParameter, torch.nn.parameter.UninitializedBuffer], init: Optional[Callable] = None):
+
+def param(
+    uninitialized: Union[
+        torch.nn.parameter.UninitializedParameter, torch.nn.parameter.UninitializedBuffer
+    ],
+    init: Optional[Any] = None,
+):
     """Create a tensor factory for an uninitialized PyTorch parameter or buffer.
 
-    When the tensor factory is invoked, it calls the ``materialize`` method of ``uninitialized`` with the given shape and returns ``uninitialized``.
+    When the tensor factory is invoked, it calls the ``materialize`` method of ``uninitialized``
+        with the given shape and returns ``uninitialized``.
 
     Args:
-        uninitialized: An instance of either ``torch.nn.parameter.UninitializedParameter`` or ``torch.nn.parameter.UninitializedBuffer``.
-        init: Initializer for the parameter. If ``None``, uses a default init method determined from the calling operation. Defaults to ``None``.
+        uninitialized: An instance of either ``torch.nn.parameter.UninitializedParameter`` or
+            ``torch.nn.parameter.UninitializedBuffer``.
+        init: Initializer for the parameter. If ``None``, uses a default init method determined
+            from the calling operation. Defaults to ``None``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
 
+    init0 = init
+
     def torch_param_factory(shape, init=init, **kwargs):
+        if init0 is not None:
+            init = init0
+
         if init is None:
-            raise ValueError("Must specify init for tensor factory torch.nn.parameter.Uninitialized*")
+            raise ValueError(
+                "Must specify init for tensor factory torch.nn.parameter.Uninitialized*"
+            )
         elif isinstance(init, str):
             if init == "get_at" or init == "rearrange":
                 init = partial(torch.nn.init.normal_, std=0.02)
             elif init == "add":
                 init = torch.nn.init.zeros_
             elif init == "multiply":
                 init = torch.nn.init.ones_
             elif init == "dot":
                 fan_in = np.prod([shape[i] for i in kwargs["in_axis"]])
-                std = np.sqrt(1.0 / fan_in) / .87962566103423978
+                std = np.sqrt(1.0 / fan_in) / 0.87962566103423978
                 init = partial(torch.nn.init.trunc_normal_, mean=0.0, std=std, a=-2.0, b=2.0)
             else:
                 raise ValueError(f"Don't know which initializer to use for operation '{init}'")
         elif isinstance(init, (int, float)):
             init = partial(torch.nn.init.constant_, val=init)
 
         with torch.no_grad():
             uninitialized.materialize(shape)
             init(uninitialized)
 
         return uninitialized
+
     return torch_param_factory
 
+
 def to_tensor_factory(x):
-    if isinstance(x, (torch.nn.parameter.UninitializedParameter, torch.nn.parameter.UninitializedBuffer)) and not isinstance(x, torch._subclasses.FakeTensor):
+    if isinstance(
+        x, (torch.nn.parameter.UninitializedParameter, torch.nn.parameter.UninitializedBuffer)
+    ) and not isinstance(x, torch._subclasses.FakeTensor):
         return param(x)
     else:
         return None
 
+
 class Norm(torch.nn.Module):
     """Normalization layer.
 
     Args:
-        stats: Einstein string determining the axes along which mean and variance are computed. Will be passed to ``einx.reduce``.
-        params: Einstein string determining the axes along which learnable parameters are applied. Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
+        stats: Einstein string determining the axes along which mean and variance are computed.
+            Will be passed to ``einx.reduce``.
+        params: Einstein string determining the axes along which learnable parameters are applied.
+            Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
         mean: Whether to apply mean normalization. Defaults to ``True``.
         var: Whether to apply variance normalization. Defaults to ``True``.
         scale: Whether to apply a learnable scale according to ``params``. Defaults to ``True``.
         bias: Whether to apply a learnable bias according to ``params``. Defaults to ``True``.
-        epsilon: A small float added to the variance to avoid division by zero. Defaults to ``1e-5``.
+        epsilon: A small float added to the variance to avoid division by zero. Defaults
+            to ``1e-5``.
         fastvar: Whether to use a fast variance computation. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
-        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``, no moving average is applied. Defaults to ``None``.
+        decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``,
+            no moving average is applied. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(self, stats: str, params: str = "b... [c]", mean: bool = True, var: bool = True, scale: bool = True, bias: bool = True, epsilon: float = 1e-5, fastvar: bool = True, dtype: Union[torch.dtype, str] = "float32", decay_rate: Optional[float] = None, **kwargs: Any):
+    def __init__(
+        self,
+        stats: str,
+        params: str = "b... [c]",
+        mean: bool = True,
+        var: bool = True,
+        scale: bool = True,
+        bias: bool = True,
+        epsilon: float = 1e-5,
+        fastvar: bool = True,
+        dtype: Union[torch.dtype, str] = "float32",
+        decay_rate: Optional[float] = None,
+        **kwargs: Any,
+    ):
         super().__init__()
         self.stats = stats
         self.params = params
         self.use_mean = mean
         self.use_var = var
         self.epsilon = epsilon
         self.fastvar = fastvar
         self.decay_rate = decay_rate
         self.kwargs = kwargs
 
-        if mean and not decay_rate is None:
-            self.register_buffer("mean", torch.nn.parameter.UninitializedBuffer(dtype=vars(torch)[dtype]))
+        if mean and decay_rate is not None:
+            self.register_buffer(
+                "mean", torch.nn.parameter.UninitializedBuffer(dtype=vars(torch)[dtype])
+            )
         else:
             self.mean = None
-        if var and not decay_rate is None:
-            self.register_buffer("var", torch.nn.parameter.UninitializedBuffer(dtype=vars(torch)[dtype]))
+        if var and decay_rate is not None:
+            self.register_buffer(
+                "var", torch.nn.parameter.UninitializedBuffer(dtype=vars(torch)[dtype])
+            )
         else:
             self.var = None
-        self.scale = torch.nn.parameter.UninitializedParameter(dtype=vars(torch)[dtype]) if scale else None
-        self.bias = torch.nn.parameter.UninitializedParameter(dtype=vars(torch)[dtype]) if bias else None
+        self.scale = (
+            torch.nn.parameter.UninitializedParameter(dtype=vars(torch)[dtype]) if scale else None
+        )
+        self.bias = (
+            torch.nn.parameter.UninitializedParameter(dtype=vars(torch)[dtype]) if bias else None
+        )
+
+        self.initialized = False
 
     def forward(self, x):
-        use_ema = not self.decay_rate is None and (not self.training or isinstance(self.mean, torch.nn.parameter.UninitializedBuffer) or isinstance(self.var, torch.nn.parameter.UninitializedBuffer))
+        use_ema = self.decay_rate is not None and (not self.training or not self.initialized)
         x, mean, var = _norm(
             x,
             self.stats,
             self.params,
             mean=self.mean if use_ema and self.use_mean else self.use_mean,
             var=self.var if use_ema and self.use_var else self.use_var,
-            scale=self.scale if not self.scale is None else None,
-            bias=self.bias if not self.bias is None else None,
+            scale=self.scale if self.scale is not None else None,
+            bias=self.bias if self.bias is not None else None,
             epsilon=self.epsilon,
             fastvar=self.fastvar,
             kwargs=self.kwargs,
         )
-        update_ema = not self.decay_rate is None and self.training
+        update_ema = self.decay_rate is not None and self.training
         if update_ema:
             with torch.no_grad():
-                if not mean is None:
-                    if isinstance(self.mean, torch.nn.parameter.UninitializedBuffer):
-                        assert False
-                        # self.mean has not been initialized in einx.nn.norm
-                        param(self.mean, init=torch.nn.init.zeros_)(mean.shape)
-                    self.mean = self.decay_rate * self.mean + (1 - self.decay_rate) * mean
-                if not var is None:
-                    if isinstance(self.var, torch.nn.parameter.UninitializedBuffer):
-                        assert False
-                        # self.var has not been initialized in einx.nn.norm
-                        param(self.var, init=torch.nn.init.ones_)(var.shape)
-                    self.var = self.decay_rate * self.var + (1 - self.decay_rate) * var
+                if mean is not None:
+                    self.mean.copy_(self.decay_rate * self.mean + (1 - self.decay_rate) * mean)
+                if var is not None:
+                    self.var.copy_(self.decay_rate * self.var + (1 - self.decay_rate) * var)
+        if not self.initialized:
+            self.initialized = True
         return x
 
+
 @_allow_in_graph
 def _norm(x, stats, params, mean, var, scale, bias, epsilon, fastvar, kwargs):
     with x.device:
         return einx.nn.norm(
             x,
             stats,
             params,
@@ -142,56 +189,67 @@
             bias=bias,
             epsilon=epsilon,
             fastvar=fastvar,
             backend="torch",
             **kwargs,
         )
 
+
 class Linear(torch.nn.Module):
     """Linear layer.
 
     Args:
-        expr: Einstein string determining the axes along which the weight matrix is multiplied. Will be passed to ``einx.dot``.
+        expr: Einstein string determining the axes along which the weight matrix is multiplied.
+            Will be passed to ``einx.dot``.
         bias: Whether to apply a learnable bias. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(self, expr: str, bias: bool = True, dtype: Union[torch.dtype, str] = "float32", **kwargs: Any):
+    def __init__(
+        self,
+        expr: str,
+        bias: bool = True,
+        dtype: Union[torch.dtype, str] = "float32",
+        **kwargs: Any,
+    ):
         super().__init__()
 
         self.weight = torch.nn.parameter.UninitializedParameter(dtype=vars(torch)[dtype])
         if bias:
             self.bias = torch.nn.parameter.UninitializedParameter(dtype=vars(torch)[dtype])
         else:
             self.bias = None
 
         self.expr = expr
         self.kwargs = kwargs
 
     def forward(self, x):
         return _linear(x, self.expr, self.weight, self.bias, self.kwargs)
 
+
 @_allow_in_graph
 def _linear(x, expr, weight, bias, kwargs):
     with x.device:
         return einx.nn.linear(
             x,
             expr,
             weight,
             bias,
             backend="torch",
             **kwargs,
         )
 
+
 class Dropout(torch.nn.Module):
     """Dropout layer.
 
     Args:
-        expr: Einstein string determining the axes along which dropout is applied. Will be passed to ``einx.elementwise``.
+        expr: Einstein string determining the axes along which dropout is applied. Will be
+            passed to ``einx.elementwise``.
         drop_rate: Drop rate.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
     def __init__(self, expr: str, drop_rate: float, **kwargs: Any):
         super().__init__()
 
@@ -201,17 +259,18 @@
 
     def forward(self, x):
         if self.training:
             return _dropout(x, self.expr, self.drop_rate, self.kwargs)
         else:
             return x
 
+
 @_allow_in_graph
 def _dropout(x, expr, drop_rate, kwargs):
     with x.device:
         return einx.nn.dropout(
             x,
             expr,
             drop_rate=drop_rate,
             backend="torch",
             **kwargs,
-        )
+        )
```

### Comparing `einx-0.1.3/einx/op/arange.py` & `einx-0.2.0/einx/op/arange.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,129 +1,177 @@
 import einx
 from functools import partial
 from . import util
 import numpy as np
 from typing import Union
 import numpy.typing as npt
 
-@einx.lru_cache(trace=lambda t, c: lambda exprs_in, expr_out, backend=None, dtype="int32": c(exprs_in, expr_out, dtype=dtype))
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda exprs_in, expr_out, backend=None, dtype="int32": c(
+        exprs_in, expr_out, dtype=dtype
+    )
+)
 def arange_stage3(expr_in, expr_out, backend, dtype="int32"):
     if isinstance(backend, str):
         backend = einx.backend.get(backend)
     for expr in expr_in.all():
         if isinstance(expr, einx.expr.stage3.Marker):
             raise ValueError("Marker in input expression not allowed")
     for root in [expr_in, expr_out]:
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Concatenation):
                 raise ValueError("Concatenation not allowed")
 
-    marked_axes = [expr for expr in expr_out.all() if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr)]
+    marked_axes = [
+        expr
+        for expr in expr_out.all()
+        if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr)
+    ]
     if len(marked_axes) > 1:
         raise ValueError(f"Expected at most one marked axis, got {len(marked_axes)}")
     ndim = marked_axes[0].value if len(marked_axes) == 1 else 1
 
     expr_in = util.flatten([expr_in])[0]
     expr_out_flat = util.flatten([expr_out])[0]
 
     def replace(expr):
         if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr):
-            expr = einx.expr.stage3.Concatenation([einx.expr.stage3.Axis(None, 1) for _ in range(ndim)])
+            expr = einx.expr.stage3.Concatenation([
+                einx.expr.stage3.Axis(None, 1) for _ in range(ndim)
+            ])
             expr = einx.expr.stage3.Composition(expr)
             return expr
+
     expr_out_flat_withconcat = einx.expr.stage3.replace(expr_out_flat, replace)
     expr_out_flat_withconcat = einx.expr.stage3.demark(expr_out_flat_withconcat)
 
     (tensor,), _ = einx.rearrange_stage3(
         [axis.__deepcopy__() for axis in expr_in],
         [backend.arange(axis.value, dtype=dtype) for axis in expr_in],
-        [expr_out_flat_withconcat]
+        [expr_out_flat_withconcat],
     )
 
     # Unflatten output expressions
-    tensor, = util.unflatten([expr_out_flat], [tensor,], [expr_out], backend)
+    (tensor,) = util.unflatten(
+        [expr_out_flat],
+        [
+            tensor,
+        ],
+        [expr_out],
+        backend=backend,
+    )
 
     return tensor, einx.expr.stage3.demark(expr_out)
 
+
 @einx.lru_cache
 def parse(description, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
 
-    description = description.split("->")
-    if len(description) > 2:
-        raise ValueError("Operation string must contain at most one '->'")
-    if "," in description[0]:
-            raise ValueError("Only a single input expression is allowed")
-
-    if len(description) == 2:
-        if "," in description[1]:
-            raise ValueError("Only a single output expression is allowed")
-        expr_in = einx.expr.stage1.parse(description[0])
-        expr_out = einx.expr.stage1.parse(description[1])
-    else:
-        expr_out = einx.expr.stage1.parse(description[0])
-        expr_in = einx.expr.stage1.get_unmarked(expr_out)
+    op = einx.expr.stage1.parse_op(description)
+
+    # Implicitly determine input expression
+    if len(op) == 1:
+        op = einx.expr.stage1.Op(
+            [
+                einx.expr.stage1.Args([einx.expr.stage1.get_unmarked(op[0][0])]),
+                op[0],
+            ],
+        )
+
+    if len(op[0]) != 1:
+        raise ValueError(f"Expected 1 input expression, but got {len(op[0])}")
+    if len(op[1]) != 1:
+        raise ValueError(f"Expected 1 output expression, but got {len(op[1])}")
+
+    marked_expr_out = einx.expr.stage1.Composition(einx.expr.stage1.get_marked(op[1][0]))
 
-    marked_expr_out = einx.expr.stage1.Composition(einx.expr.stage1.get_marked(expr_out))
     def after_stage2(exprs1, exprs2):
         expr_out = exprs1[1]
-        out_axes = [expr for expr in expr_out.all() if isinstance(expr, (einx.expr.stage2.NamedAxis, einx.expr.stage2.UnnamedAxis))]
+        out_axes = [
+            expr
+            for expr in expr_out.all()
+            if isinstance(expr, (einx.expr.stage2.NamedAxis, einx.expr.stage2.UnnamedAxis))
+        ]
         marked_out_axes = [expr for expr in out_axes if einx.expr.stage2.is_marked(expr)]
         if len(marked_out_axes) > 1:
             raise ValueError(f"Expected at most one marked axis, got {len(marked_out_axes)}")
         ndim = len(out_axes) - len(marked_out_axes)
         return [einx.expr.Equation(marked_expr_out, np.asarray([ndim]))]
 
     expr_in, expr_out = einx.expr.solve(
-            [einx.expr.Equation(expr_in)] \
-          + [einx.expr.Equation(expr_out)] \
-          + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+        [einx.expr.Equation(op[0][0])]
+        + [einx.expr.Equation(op[1][0])]
+        + [
+            einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+            for k, v in parameters.items()
+        ],
         cse=cse,
         after_stage2=after_stage2,
     )[:2]
 
     return expr_in, expr_out
 
-@einx.lru_cache(trace=lambda t, c: lambda description, backend=None, **kwargs: c(description, **kwargs))
-def arange(description: str, *, backend: Union[einx.Backend, str], dtype: str = "int32", cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+@einx.lru_cache(
+    trace=lambda t, c: lambda description, backend=None, **kwargs: c(description, **kwargs)
+)
+def arange(
+    description: str,
+    *,
+    backend: Union[einx.Backend, str],
+    dtype: str = "int32",
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """n-dimensional ``arange`` operation.
 
-    Runs ``backend.arange`` for every axis in ``input``, and stacks the results along the single marked axis in ``output``. Always uses ``start=0`` and ``step=1``.
+    Runs ``backend.arange`` for every axis in ``input``, and stacks the results along the single
+    marked axis in ``output``. Always uses ``start=0`` and ``step=1``.
 
     The `description` argument must meet one of the following formats:
 
     1. ``input -> output``
-        Runs ``backend.arange`` for every axis in ``input``, and stacks the results along the marked axis in ``output``. The values are stacked in the order
-        that the axes appear in ``input``.
+        Runs ``backend.arange`` for every axis in ``input``, and stacks the results along the
+        marked axis in ``output``. The values are stacked in the order that the axes appear
+        in ``input``.
 
     2. ``output``
         Implicitly determines the input expression by removing the marked axis from ``output``.
 
         Example: ``a b [2]`` resolves to ``a b -> a b [2]``
 
     Args:
         description: Description string in Einstein notation (see above).
         backend: Backend to use for all operations.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to True.
-        graph: Whether to return the graph representation of the operation instead of computing the result. Defaults to False.
+        cse: Whether to apply common subexpression elimination to the expressions. Defaults
+            to True.
+        graph: Whether to return the graph representation of the operation instead of computing
+            the result. Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
-        The result of the n-dimensional arange operation if `graph=False`, otherwise the graph representation of the operation.
+        The result of the n-dimensional arange operation if `graph=False`, otherwise the graph
+        representation of the operation.
 
     Examples:
         Arange two-dimensional coordinates:
 
         >>> tensor = einx.arange("a b [2]", a=5, b=6, backend="numpy")
         >>> tensor.shape
         (5, 6, 2)
         >>> tensor[2, 3]
         array([2, 3], dtype=int32)
 
-        Arange two-dimensional coordinates with inverted coordinates (`Cartesian ordering <https://numpy.org/doc/stable/reference/generated/numpy.meshgrid.html>`_:
+        Arange two-dimensional coordinates with inverted coordinates (`Cartesian ordering
+        <https://numpy.org/doc/stable/reference/generated/numpy.meshgrid.html>`_:
         First axis of tensor corresponds to second coordinate along stacked axis and vice versa.):
 
         >>> tensor = einx.arange("a b -> b a [2]", a=5, b=6, backend="numpy")
         >>> tensor.shape
         (6, 5, 2)
         >>> tensor[2, 3]
         array([3, 2], dtype=int32)
@@ -132,8 +180,10 @@
 
         >>> einx.arange("a", a=5, backend="numpy").shape
         (5,)
     """
     expr_in, expr_out = parse(description, cse=cse, **parameters)
     tensor, expr_out = arange_stage3(expr_in, expr_out, backend=backend, dtype=dtype)
     return tensor
+
+
 arange.parse = parse
```

### Comparing `einx-0.1.3/einx/op/dot.py` & `einx-0.2.0/einx/op/dot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,187 +1,255 @@
 import einx
 from . import util
 import numpy as np
 from typing import Union
 import numpy.typing as npt
 
-@einx.lru_cache(trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, backend=None: c(exprs_in, [t(x) for x in tensors_in], expr_out))
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, backend=None: c(
+        exprs_in, [t(x) for x in tensors_in], expr_out
+    )
+)
 def dot_stage3(exprs_in, tensors_in, expr_out, backend=None):
     if backend is None:
         backend = einx.backend.get(tensors_in)
     elif isinstance(backend, str):
         backend = einx.backend.get(backend)
     if any(isinstance(expr, einx.expr.stage3.Concatenation) for expr in expr_out.all()):
         raise ValueError("Output expression cannot contain concatenations")
     for root in list(exprs_in) + [expr_out]:
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Marker):
-                raise ValueError(f"Marker is not allowed")
+                raise ValueError("Marker is not allowed")
             if isinstance(expr, einx.expr.stage3.Concatenation):
                 raise ValueError("Concatenation not allowed")
 
     # Call tensor factories
     output_axis_names = {a.name for a in expr_out.all() if isinstance(a, einx.expr.stage3.Axis)}
+
     def get_fans(idx):
-        other_input_axis_names = {a.name for i, expr_in in enumerate(exprs_in) for a in expr_in.all() if i != idx and isinstance(a, einx.expr.stage3.Axis)}
+        other_input_axis_names = {
+            a.name
+            for i, expr_in in enumerate(exprs_in)
+            for a in expr_in.all()
+            if i != idx and isinstance(a, einx.expr.stage3.Axis)
+        }
         in_axis = []
         out_axis = []
         batch_axis = []
         for i, child in enumerate(exprs_in[idx]):
-            any_in_other_input = any(isinstance(a, einx.expr.stage3.Axis) and a.name in other_input_axis_names for a in child.all())
-            any_in_output = any(isinstance(a, einx.expr.stage3.Axis) and a.name in output_axis_names for a in child.all())
+            any_in_other_input = any(
+                isinstance(a, einx.expr.stage3.Axis) and a.name in other_input_axis_names
+                for a in child.all()
+            )
+            any_in_output = any(
+                isinstance(a, einx.expr.stage3.Axis) and a.name in output_axis_names
+                for a in child.all()
+            )
             if any_in_other_input and not any_in_output:
                 in_axis.append(i)
             elif any_in_output and not any_in_other_input:
                 out_axis.append(i)
             else:
                 batch_axis.append(i)
-        return {"in_axis": tuple(in_axis), "out_axis": tuple(out_axis), "batch_axis": tuple(batch_axis)}
-    tensors_in = [einx.param.instantiate(tensor, expr.shape, backend, **get_fans(i), name="weight", init="dot") for i, (tensor, expr) in enumerate(zip(tensors_in, exprs_in))]
+        return {
+            "in_axis": tuple(in_axis),
+            "out_axis": tuple(out_axis),
+            "batch_axis": tuple(batch_axis),
+        }
+
+    tensors_in = [
+        einx.param.instantiate(
+            tensor, expr.shape, backend, **get_fans(i), name="weight", init="dot"
+        )
+        for i, (tensor, expr) in enumerate(zip(tensors_in, exprs_in))
+    ]
 
     # Flatten expressions
-    exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend)
+    exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend=backend)
     expr_out_flat = util.flatten([expr_out])[0]
     assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_in)
     assert einx.expr.stage3.is_flat(expr_out_flat)
 
     # Apply einsum
     einsum_variables = {}
+
     def get_einsum_variable(key):
         if key in einsum_variables:
             return einsum_variables[key]
         else:
             v = chr(ord("a") + len(einsum_variables))
             if ord(v) > ord("z"):
                 raise ValueError(f"Only supports up to {ord('z') - ord('a') + 1} unique input axes")
             einsum_variables[key] = v
             return v
+
     def to_einsum(axes):
         return "".join(get_einsum_variable(a.name) for a in axes)
 
-    input_axis_names = set(a.name for expr in exprs_in for a in einx.expr.stage3.get_axes(expr))
+    input_axis_names = {a.name for expr in exprs_in for a in einx.expr.stage3.get_axes(expr)}
 
-    einsum_str = ",".join(to_einsum(einx.expr.stage3.get_axes(expr)) for expr in exprs_in) \
-               + "->" + to_einsum([a for a in einx.expr.stage3.get_axes(expr_out_flat) if a.name in input_axis_names])
+    einsum_str = (
+        ",".join(to_einsum(einx.expr.stage3.get_axes(expr)) for expr in exprs_in)
+        + "->"
+        + to_einsum([
+            a for a in einx.expr.stage3.get_axes(expr_out_flat) if a.name in input_axis_names
+        ])
+    )
 
     tensor = backend.einsum(einsum_str, *tensors_in)
-    expr = einx.expr.stage3.List([a.__deepcopy__() for a in einx.expr.stage3.get_axes(expr_out_flat) if a.name in input_axis_names])
+    expr = einx.expr.stage3.List([
+        a.__deepcopy__()
+        for a in einx.expr.stage3.get_axes(expr_out_flat)
+        if a.name in input_axis_names
+    ])
 
     # Transpose and broadcast missing output dimensions
-    tensor = util.transpose_broadcast(expr, tensor, expr_out_flat)[0]
+    tensor = util.transpose_broadcast(expr, tensor, expr_out_flat, backend=backend)[0]
 
     # Unflatten output expression
-    assert not tensor.shape is None
+    assert tensor.shape is not None
     if tensor.shape != expr_out.shape:
         tensor = backend.reshape(tensor, expr_out.shape)
 
     return tensor, expr_out
 
+
 @einx.lru_cache
 def parse(description, *tensor_shapes, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
-
-    description = description.split("->")
-    if len(description) == 1:
-        # Description: "input -> output" using [|]-choice
-        expr = description[0]
-        if "," in expr:
-            raise ValueError("Only a single input expression is allowed when output expression is not given")
-        if len(tensor_shapes) != 2:
-            raise ValueError(f"Expected 2 input tensors, got {len(tensor_shapes)}")
-
-        expr = einx.expr.stage1.parse(expr)
-        expr_in1 = str(einx.expr.stage1.choose(expr, 0, num=2))
-        expr_out = str(einx.expr.stage1.choose(expr, 1, num=2))
-
-        exprs_in = [expr_in1]
-    else:
-        # Description: "inputs... -> output"
-        if len(description) > 2:
-            raise ValueError("Operation can contain at most one '->'")
-        exprs_in, expr_out = description
-        exprs_in = exprs_in.split(",")
-
-    if len(exprs_in) == 1 and len(tensor_shapes) == 2:
-        # Description: input1 -> output, determine input2 implicitly
-        expr_in1 = einx.expr.stage1.parse(exprs_in[0])
-        expr_out = einx.expr.stage1.parse(expr_out)
-
-        for root in [expr_in1, expr_out]:
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
+
+    op = einx.expr.stage1.parse_op(description)
+
+    # Implicitly determine second input expression
+    if len(op[0]) == 1 and len(tensor_shapes) == 2:
+        for root in [op[0][0], op[1][0]]:
             for expr in root.all():
-                if isinstance(expr, einx.expr.stage1.UnnamedAxis) and expr.value != 1 and einx.expr.stage1.is_marked(expr):
+                if (
+                    isinstance(expr, einx.expr.stage1.UnnamedAxis)
+                    and expr.value != 1
+                    and einx.expr.stage1.is_marked(expr)
+                ):
                     raise ValueError(f"Cannot mark unnamed non-trivial axes, but found {expr}")
 
-        # Get ordered list of axes for second input
-        names = []
-        for root in [expr_in1, expr_out]:
+        # Create second input expression from ordered list of marked axes
+        names = set()
+        expr_in2 = []
+        for root in [op[0][0], op[1][0]]:
             for expr in root.all():
-                if isinstance(expr, einx.expr.stage1.NamedAxis) and einx.expr.stage1.is_marked(expr):
-                    name = expr.name
-                    for _ in range(expr.depth):
-                        name = name + einx.expr.stage1._ellipsis
-                    if not name in names:
-                        names.append(name)
-        expr_in2 = " ".join(names)
-
-        expr_in1 = einx.expr.stage1.demark(expr_in1)
-        expr_out = einx.expr.stage1.demark(expr_out)
-        exprs_in = [expr_in1, expr_in2]
-
-    if len(exprs_in) != len(tensor_shapes):
-        raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensor_shapes)}")
+                if (
+                    isinstance(expr, einx.expr.stage1.NamedAxis)
+                    and einx.expr.stage1.is_marked(expr)
+                    and expr.name not in names
+                ):
+                    names.add(expr.name)
+
+                    # Copy axis
+                    expr2 = expr.__deepcopy__()
+
+                    # Apply the same ellipses
+                    parent = expr
+                    while parent.parent is not None:
+                        if isinstance(parent, einx.expr.stage1.Ellipsis):
+                            expr2 = einx.expr.stage1.Ellipsis(expr2, ellipsis_id=parent.ellipsis_id)
+                        parent = parent.parent
+
+                    # Append to second output expression
+                    expr_in2.append(expr2)
+        expr_in2 = einx.expr.stage1.List(expr_in2)
+
+        op = einx.expr.stage1.Op([
+            einx.expr.stage1.Args([
+                einx.expr.stage1.demark(op[0][0]),
+                expr_in2,
+            ]),
+            einx.expr.stage1.Args([
+                einx.expr.stage1.demark(op[1][0]),
+            ]),
+        ])
+
+    if len(op[0]) != len(tensor_shapes):
+        raise ValueError(f"Expected {len(op[0])} input tensor(s), got {len(tensor_shapes)}")
+    if len(op[1]) != 1:
+        raise ValueError(f"Expected 1 output expression, but got {len(op[1])}")
 
     exprs = einx.expr.solve(
-            [einx.expr.Equation(expr_in, tensor_shape) for expr_in, tensor_shape in zip(exprs_in, tensor_shapes)] \
-          + [einx.expr.Equation(expr_out)] \
-          + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+        [
+            einx.expr.Equation(expr_in, tensor_shape)
+            for expr_in, tensor_shape in zip(op[0], tensor_shapes)
+        ]
+        + [einx.expr.Equation(op[1][0])]
+        + [
+            einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+            for k, v in parameters.items()
+        ],
         cse=cse,
         cse_concat=False,
-    )[:len(exprs_in) + 1]
+    )[: len(op[0]) + 1]
     exprs_in, expr_out = exprs[:-1], exprs[-1]
 
     return exprs_in, expr_out
 
-@einx.lru_cache(trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(description, *[t(x) for x in tensors], **kwargs))
-def dot(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+@einx.lru_cache(
+    trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
+        description, *[t(x) for x in tensors], **kwargs
+    )
+)
+def dot(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Computes a general dot-product of the input tensors.
 
-    The function flattens all input tensors, applies the general dot-product yielding a single output tensor, and rearranges
-    the result to match the output expression (see :doc:`How does einx handle input and output tensors? </faq/flatten>`).
+    The function flattens all input tensors, applies the general dot-product yielding a single
+    output tensor, and rearranges the result to match the output expression (see
+    :doc:`How does einx handle input and output tensors? </faq/flatten>`).
 
-    The `description` argument specifies the input and output expressions. It must meet one of the following formats:
+    The `description` argument specifies the input and output expressions. It must meet
+    one of the following formats:
 
     1. ``input1, input2, ... -> output``
-        All input and output expressions are specified explicitly. Similar to `np.einsum <https://numpy.org/doc/stable/reference/generated/numpy.einsum.html>`_ notation.
-        
-    2. ``input1 -> output``
-        The function accepts two input tensors. ``[]``-brackets mark all axes in ``input1`` and ``output`` that should also appear in the second input.
-        The second input is then determined as an ordered list of all marked axes (without duplicates).
-        
-        Example: ``[b c1] -> [b c2]`` resolves to ``b c1, b c1 c2 -> b c2``
+        All input and output expressions are specified explicitly. Similar to
+        `np.einsum <https://numpy.org/doc/stable/reference/generated/numpy.einsum.html>`_
+        notation.
 
-    3. ``... [input1|output] ...``
-        The function accepts two input tensors. The left and right choices correspond to the first input tensor and the output tensor, respectively.
+    2. ``input1 -> output``
+        The function accepts two input tensors. ``[]``-brackets mark all axes in ``input1``
+        and ``output`` that should also appear in the second input. The second input is then
+        determined as an ordered list of all marked axes (without duplicates).
 
-        Example: ``b [c1|c2]`` resolves to ``b [c1] -> b [c2]``
+        Example: ``[b c1] -> [b c2]`` resolves to ``b c1, b c1 c2 -> b c2``
 
-    The function additionally passes the ``in_axes``, ``out_axes`` and ``batch_axes`` arguments to tensor factories that can be used to determine the fan-in
-    and fan-out of a neural network layer and initialize weights accordingly
-    (see e.g. `jax.nn.initializers.lecun_normal <https://jax.readthedocs.io/en/latest/_autosummary/jax.nn.initializers.lecun_normal.html#jax.nn.initializers.lecun_normal>`_)
+    The function additionally passes the ``in_axes``, ``out_axes`` and ``batch_axes`` arguments
+    to tensor factories that can be used to determine the fan-in and fan-out of a neural network
+    layer and initialize weights accordingly (see e.g. `jax.nn.initializers.lecun_normal
+    <https://jax.readthedocs.io/en/latest/_autosummary/jax.nn.initializers.lecun_normal.html#jax.nn.initializers.lecun_normal>`_)
 
     Args:
         description: Description string in Einstein notation (see above).
         tensors: Input tensors or tensor factories matching the description string.
-        backend: Backend to use for all operations. If None, determines the backend from the input tensors. Defaults to None.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to True.
-        graph: Whether to return the graph representation of the operation instead of computing the result. Defaults to False.
+        backend: Backend to use for all operations. If None, determines the backend from the
+            input tensors. Defaults to None.
+        cse: Whether to apply common subexpression elimination to the expressions. Defaults
+            to True.
+        graph: Whether to return the graph representation of the operation instead of computing
+            the result. Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
-        The result of the dot-product operation if `graph=False`, otherwise the graph representation of the operation.
+        The result of the dot-product operation if `graph=False`, otherwise the graph
+        representation of the operation.
 
     Examples:
         Compute an inner product between two vectors:
 
         >>> a, b = np.random.uniform(size=(10,)), np.random.uniform(size=(10,))
         >>> einx.dot("a, a ->", a, b).shape
         ()
@@ -189,30 +257,42 @@
         Compute a matrix-vector product:
 
         >>> a, b = np.random.uniform(size=(10, 10)), np.random.uniform(size=(10,))
         >>> einx.dot("a b, b -> a", a, b).shape
         (10,)
         >>> einx.dot("a [b] -> a", a, b).shape
         (10,)
-        >>> einx.dot("a [b|]", a, b).shape
+        >>> einx.dot("a [b->]", a, b).shape
         (10,)
 
         Compute a vector-matrix product:
 
         >>> a, b = np.random.uniform(size=(10,)), np.random.uniform(size=(10, 10))
         >>> einx.dot("a, a b -> b", a, b).shape
         (10,)
         >>> einx.dot("[a] -> [b]", a, b).shape
         (10,)
-        >>> einx.dot("[a|b]", a, b).shape
+        >>> einx.dot("[a->b]", a, b).shape
         (10,)
 
         Multiply a tensor with a weight matrix:
 
-        >>> x, w = np.random.uniform(size=(4, 16, 16, 64)), np.random.uniform(size=(64, 32,))
-        >>> einx.dot("b... [c1|c2]", x, w).shape
+        >>> x, w = (
+        ...     np.random.uniform(size=(4, 16, 16, 64)),
+        ...     np.random.uniform(
+        ...         size=(
+        ...             64,
+        ...             32,
+        ...         )
+        ...     ),
+        ... )
+        >>> einx.dot("b... [c1->c2]", x, w).shape
         (4, 16, 16, 32)
     """
-    exprs_in, expr_out = parse(description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters)
-    tensor, expr = dot_stage3(exprs_in, tensors, expr_out, backend=backend)
+    exprs_in, expr_out = parse(
+        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+    )
+    tensor, _expr = dot_stage3(exprs_in, tensors, expr_out, backend=backend)
     return tensor
-dot.parse = parse
+
+
+dot.parse = parse
```

### Comparing `einx-0.1.3/einx/op/elementwise.py` & `einx-0.2.0/einx/op/elementwise.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import einx
 from . import util
 from functools import partial
 import numpy as np
 from typing import Callable, Union
 import numpy.typing as npt
 
-@einx.lru_cache(trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, op, backend=None: c(exprs_in, [t(x) for x in tensors_in], expr_out, op))
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, op, backend=None: c(
+        exprs_in, [t(x) for x in tensors_in], expr_out, op
+    )
+)
 def elementwise_stage3(exprs_in, tensors_in, expr_out, op, backend=None):
     if backend is None:
         backend = einx.backend.get(tensors_in)
     elif isinstance(backend, str):
         backend = einx.backend.get(backend)
     for root in list(exprs_in) + [expr_out]:
         for expr in root.all():
@@ -23,266 +28,486 @@
     def get_name(s):
         if s == "add":
             return "bias"
         elif s == "multiply":
             return "scale"
         else:
             return s
-    tensors_in = [einx.param.instantiate(tensor, expr.shape, backend, name=get_name(util._op_to_str(op)), init=util._op_to_str(op)) for tensor, expr in zip(tensors_in, exprs_in)]
 
-    tensors_out, exprs_out = einx.vmap_with_axis_stage3(exprs_in, tensors_in, [expr_out], op, backend=backend)
+    tensors_in = [
+        einx.param.instantiate(
+            tensor,
+            expr.shape,
+            backend,
+            name=get_name(util._op_to_str(op)),
+            init=util._op_to_str(op),
+        )
+        for tensor, expr in zip(tensors_in, exprs_in)
+    ]
+
+    tensors_out, exprs_out = einx.vmap_with_axis_stage3(
+        exprs_in, tensors_in, [expr_out], op, backend=backend
+    )
     assert len(tensors_out) == 1 and len(exprs_out) == 1
     return tensors_out[0], exprs_out[0]
 
+
 @einx.lru_cache
 def parse(description, *tensor_shapes, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
-
-    if "->" in description:
-        # Description: Inputs and output
-        description = description.split("->")
-        if len(description) != 2:
-            raise ValueError("Operation cannot contain more than one '->'")
-        exprs_in, expr_out = description
-        exprs_in = exprs_in.split(",")
-        if len(exprs_in) != len(tensor_shapes):
-            raise ValueError(f"Expected {len(exprs_in)} input tensors, got {len(tensor_shapes)}")
-
-        exprs = einx.expr.solve(
-              [einx.expr.Equation(expr_in, tensor_shape) for expr_in, tensor_shape in zip(exprs_in, tensor_shapes)] \
-            + [einx.expr.Equation(expr_out,)] \
-            + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
-            cse=cse,
-            cse_concat=False,
-        )[:len(exprs_in) + 1]
-        exprs_in, expr_out = exprs[:-1], exprs[-1]
-    else:
-        # Description: Only inputs
-        exprs_in = description.split(",")
-
-        if len(exprs_in) == 1 and len(tensor_shapes) == 2:
-            # Expression contains markers -> add second input expression from marked subexpressions
-            expr_in1 = einx.expr.stage1.parse(exprs_in[0])
-            expr_in2 = einx.expr.stage1.get_marked(expr_in1)
-            expr_in1 = einx.expr.stage1.demark(expr_in1)
-            exprs_in = [expr_in1, expr_in2]
-
-        if len(exprs_in) != len(tensor_shapes):
-            raise ValueError(f"Expected {len(exprs_in)} input tensors, got {len(tensor_shapes)}")
-
-        exprs_in = einx.expr.solve(
-                [einx.expr.Equation(expr_in, tensor_shape) for expr_in, tensor_shape in zip(exprs_in, tensor_shapes)] \
-              + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
-            cse=cse,
-            cse_concat=False,
-        )[:len(exprs_in)]
-
-        # Implicitly determine output expression: Check if one input expression contains the axis names of all others, and this choice is unique
-        in_axis_names = [set(expr.name for expr in root.all() if isinstance(expr, einx.expr.stage3.Axis) and not expr.is_unnamed) for root in exprs_in]
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
+
+    op = einx.expr.stage1.parse_op(description)
+
+    # Add second input expression from marked subexpressions
+    if len(op[0]) == 1 and len(tensor_shapes) == 2:
+        op = einx.expr.stage1.Op(
+            [
+                einx.expr.stage1.Args([
+                    einx.expr.stage1.demark(op[0][0]),
+                    einx.expr.stage1.get_marked(op[0][0]),
+                ]),
+            ]
+            + list(op[1:])
+        )
+
+    # Implicitly determine output expression
+    if len(op) == 1:
+        # Use one of the input expression if contains the axis names of
+        # all others and if this choice is unique
+        input_args = op[0]
+        in_axis_names = [
+            {expr.name for expr in root.all() if isinstance(expr, einx.expr.stage1.NamedAxis)}
+            for root in input_args
+        ]
 
         valid_parents = set()
         for i, parent in enumerate(in_axis_names):
             for j, child in enumerate(in_axis_names):
                 if i != j and not child.issubset(parent):
                     break
             else:
                 # Found valid parent
-                valid_parents.add(exprs_in[i])
+                valid_parents.add(input_args[i])
 
         if len(valid_parents) != 1:
-            raise ValueError(f"Could not implicitly determine output expression for input expressions {[str(expr) for expr in exprs_in]}")
+            raise ValueError(f"Could not implicitly determine output expression for op '{op}'")
         expr_out = next(iter(valid_parents)).__deepcopy__()
+        op = einx.expr.stage1.Op([op[0], einx.expr.stage1.Args([expr_out])])
+
+    if len(op[0]) != len(tensor_shapes):
+        raise ValueError(f"Expected {len(op[0])} input tensors, but got {len(tensor_shapes)}")
+    if len(op[1]) != 1:
+        raise ValueError(f"Expected 1 output expression, but got {len(op[1])}")
+
+    exprs = einx.expr.solve(
+        [
+            einx.expr.Equation(expr_in, tensor_shape)
+            for expr_in, tensor_shape in zip(op[0], tensor_shapes)
+        ]
+        + [
+            einx.expr.Equation(
+                op[1][0],
+            )
+        ]
+        + [
+            einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+            for k, v in parameters.items()
+        ],
+        cse=cse,
+        cse_concat=False,
+    )[: len(op[0]) + 1]
+    exprs_in, expr_out = exprs[:-1], exprs[-1]
 
     return exprs_in, expr_out
 
-@einx.lru_cache(trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(description, *[t(x) for x in tensors], **kwargs))
-def elementwise(description: str, *tensors: einx.Tensor, op: Callable, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
-    """Applies an element-by-element operation over the given tensors. Specializes :func:`einx.vmap_with_axis`.
 
-    The function flattens all input tensors, applies the given element-by-element operation yielding a single output tensor, and rearranges
-    the result to match the output expression (see :doc:`How does einx handle input and output tensors? </faq/flatten>`).
+@einx.traceback_util.filter
+@einx.lru_cache(
+    trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
+        description, *[t(x) for x in tensors], **kwargs
+    )
+)
+def elementwise(
+    description: str,
+    *tensors: einx.Tensor,
+    op: Callable,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
+    """Applies an element-by-element operation over the given tensors. Specializes
+    :func:`einx.vmap_with_axis`.
+
+    The function flattens all input tensors, applies the given element-by-element operation
+    yielding a single output tensor, and rearranges the result to match the output expression
+    (see :doc:`How does einx handle input and output tensors? </faq/flatten>`).
 
-    The `description` argument specifies the input and output expressions. It must meet one of the following formats:
+    The `description` argument specifies the input and output expressions. It must meet one of
+    the following formats:
 
     1. ``input1, input2, ... -> output``
         All input and output expressions are specified explicitly.
 
     2. ``input1, input2, ...``
-        All input expressions are specified explicitly. If one of the input expressions is a parent of or equal to all other input expressions,
-        it is used as the output expression. Otherwise, an exception is raised.
-        
+        All input expressions are specified explicitly. If one of the input expressions is a
+        parent of or equal to all other input expressions, it is used as the output expression.
+        Otherwise, an exception is raised.
+
         Example: ``a b, a`` resolves to ``a b, a -> a b``.
 
     3. ``input1`` with ``[]``-brackets
         The function accepts two input tensors. `[]`-brackets mark all subexpressions in the
         first input that should also appear in the second input.
-        
+
         Example: ``a [b]`` resolves to ``a b, b``
 
     Args:
         description: Description string in Einstein notation (see above).
         tensors: Input tensors or tensor factories matching the description string.
-        op: Backend elemebt-by-element operation. Must accept the same number of tensors as specified in the description string and comply with numpy broadcasting rules. If `op` is a string, retrieves the attribute of `backend` with the same name.
-        backend: Backend to use for all operations. If None, determines the backend from the input tensors. Defaults to None.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to True.
-        graph: Whether to return the graph representation of the operation instead of computing the result. Defaults to False.
+        op: Backend elemebt-by-element operation. Must accept the same number of tensors
+            as specified in the description string and comply with numpy broadcasting rules.
+            If `op` is a string, retrieves the attribute of `backend` with the same name.
+        backend: Backend to use for all operations. If None, determines the backend from
+            the input tensors. Defaults to None.
+        cse: Whether to apply common subexpression elimination to the expressions. Defaults
+            to True.
+        graph: Whether to return the graph representation of the operation instead of
+            computing the result. Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
-        The result of the elementwise operation if `graph=False`, otherwise the graph representation of the operation.
+        The result of the elementwise operation if `graph=False`, otherwise the graph
+        representation of the operation.
 
     Examples:
         Compute a sum of two vectors:
 
         >>> a, b = np.random.uniform(size=(10,)), np.random.uniform(size=(10,))
         >>> einx.elementwise("a, a -> a", a, b, op=np.add).shape
         (10,)
 
-        Add a vector on all rows of a matrix:
+        Add a vector on all columns of a matrix:
 
         >>> a, b = np.random.uniform(size=(10, 10)), np.random.uniform(size=(10,))
         >>> einx.add("a b, a -> a b", a, b).shape
         (10, 10,)
 
-        Subtract a vector from all columns of a matrix:
+        Subtract a vector from all rows of a matrix:
 
         >>> a, b = np.random.uniform(size=(10, 10)), np.random.uniform(size=(10,))
         >>> einx.subtract("a b, b -> a b", a, b).shape
         (10, 10,)
 
         Select from one of two choices according to a boolean mask:
 
-        >>> x, mask = np.random.uniform(size=(10, 10)), np.random.uniform(size=(10,))
+        >>> x, mask = (
+        ...     np.random.uniform(size=(10, 10)),
+        ...     np.random.uniform(size=(10,)),
+        ... )
         >>> einx.where("a, a b, -> a b", mask, x, 0).shape
         (10, 10,)
 
         Add a bias onto all channels of a tensor:
 
-        >>> x, w = np.random.uniform(size=(4, 16, 16, 64)), np.random.uniform(size=(64,))
+        >>> x, w = (
+        ...     np.random.uniform(size=(4, 16, 16, 64)),
+        ...     np.random.uniform(size=(64,)),
+        ... )
         >>> einx.add("b... [c]", x, w).shape
         (4, 16, 16, 64)
     """
-    exprs_in, expr_out = parse(description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters)
+    exprs_in, expr_out = parse(
+        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+    )
     tensor, expr_out = elementwise_stage3(exprs_in, tensors, expr_out, op=op, backend=backend)
     return tensor
-elementwise.parse = parse
 
 
+elementwise.parse = parse
 
-def add(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def add(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="add"``"""
     return elementwise(description, *tensors, op="add", backend=backend, cse=cse, **parameters)
 
+
 def add_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="add", **kwargs)
 
-def subtract(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def subtract(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="subtract"``"""
     return elementwise(description, *tensors, op="subtract", backend=backend, cse=cse, **parameters)
 
+
 def subtract_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="subtract", **kwargs)
 
-def multiply(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def multiply(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="multiply"``"""
     return elementwise(description, *tensors, op="multiply", backend=backend, cse=cse, **parameters)
 
+
 def multiply_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="multiply", **kwargs)
 
-def true_divide(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def true_divide(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="true_divide"``"""
-    return elementwise(description, *tensors, op="true_divide", backend=backend, cse=cse, **parameters)
+    return elementwise(
+        description, *tensors, op="true_divide", backend=backend, cse=cse, **parameters
+    )
+
 
 def true_divide_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="true_divide", **kwargs)
 
-def floor_divide(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def floor_divide(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="floor_divide"``"""
-    return elementwise(description, *tensors, op="floor_divide", backend=backend, cse=cse, **parameters)
+    return elementwise(
+        description, *tensors, op="floor_divide", backend=backend, cse=cse, **parameters
+    )
+
 
 def floor_divide_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="floor_divide", **kwargs)
 
-def divide(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def divide(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="divide"``"""
     return elementwise(description, *tensors, op="divide", backend=backend, cse=cse, **parameters)
 
+
 def divide_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="divide", **kwargs)
 
-def logical_and(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def logical_and(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="logical_and"``"""
-    return elementwise(description, *tensors, op="logical_and", backend=backend, cse=cse, **parameters)
+    return elementwise(
+        description, *tensors, op="logical_and", backend=backend, cse=cse, **parameters
+    )
+
 
 def logical_and_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="logical_and", **kwargs)
 
-def logical_or(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def logical_or(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="logical_or"``"""
-    return elementwise(description, *tensors, op="logical_or", backend=backend, cse=cse, **parameters)
+    return elementwise(
+        description, *tensors, op="logical_or", backend=backend, cse=cse, **parameters
+    )
+
 
 def logical_or_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="logical_or", **kwargs)
 
-def where(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def where(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="where"``"""
     return elementwise(description, *tensors, op="where", backend=backend, cse=cse, **parameters)
 
+
 def where_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="where", **kwargs)
 
-def less(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def less(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="less"``"""
     return elementwise(description, *tensors, op="less", backend=backend, cse=cse, **parameters)
 
+
 def less_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="less", **kwargs)
 
-def less_equal(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def less_equal(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="less_equal"``"""
-    return elementwise(description, *tensors, op="less_equal", backend=backend, cse=cse, **parameters)
+    return elementwise(
+        description, *tensors, op="less_equal", backend=backend, cse=cse, **parameters
+    )
+
 
 def less_equal_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="less_equal", **kwargs)
 
-def greater(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def greater(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="greater"``"""
     return elementwise(description, *tensors, op="greater", backend=backend, cse=cse, **parameters)
 
+
 def greater_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="greater", **kwargs)
 
-def greater_equal(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def greater_equal(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="greater_equal"``"""
-    return elementwise(description, *tensors, op="greater_equal", backend=backend, cse=cse, **parameters)
+    return elementwise(
+        description, *tensors, op="greater_equal", backend=backend, cse=cse, **parameters
+    )
+
 
 def greater_equal_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="greater_equal", **kwargs)
 
-def equal(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def equal(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="equal"``"""
     return elementwise(description, *tensors, op="equal", backend=backend, cse=cse, **parameters)
 
+
 def equal_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="equal", **kwargs)
 
-def not_equal(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def not_equal(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="not_equal"``"""
-    return elementwise(description, *tensors, op="not_equal", backend=backend, cse=cse, **parameters)
+    return elementwise(
+        description, *tensors, op="not_equal", backend=backend, cse=cse, **parameters
+    )
+
 
 def not_equal_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="not_equal", **kwargs)
 
-def maximum(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def maximum(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="maximum"``"""
     return elementwise(description, *tensors, op="maximum", backend=backend, cse=cse, **parameters)
 
+
 def maximum_stage3(*args, **kwargs):
     return elementwise_stage3(*args, op="maximum", **kwargs)
 
-def minimum(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def minimum(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.elementwise` with ``op="minimum"``"""
     return elementwise(description, *tensors, op="minimum", backend=backend, cse=cse, **parameters)
 
+
 def minimum_stage3(*args, **kwargs):
-    return elementwise_stage3(*args, op="minimum", **kwargs)
+    return elementwise_stage3(*args, op="minimum", **kwargs)
```

### Comparing `einx-0.1.3/einx/op/index.py` & `einx-0.2.0/einx/op/index.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,52 +2,77 @@
 from functools import partial
 from . import util
 import numpy as np
 from typing import Callable, Union
 import numpy.typing as npt
 
 
-
-def _index(*tensors, update, layout, expr_update_inner, expr_common, op=None):
+def _index(*tensors, update, layout, expr_update_inner, expr_common, op=None, backend=None):
+    assert backend is not None
     if update:
         tensor_in = tensors[0]
         tensor_coordinates = tensors[1:-1]
         tensor_update = tensors[-1]
     else:
         tensor_in = tensors[0]
         tensor_coordinates = tensors[1:]
 
     # Split multi-dim coordinate tensors into single-dim coordinate tensors
-    layout = [(tensor, coordinate_axis_name, expr_coord, ndim) for tensor, (coordinate_axis_name, expr_coord, ndim) in zip(tensor_coordinates, layout)]
+    layout = [
+        (tensor, coordinate_axis_name, expr_coord, ndim)
+        for tensor, (coordinate_axis_name, expr_coord, ndim) in zip(tensor_coordinates, layout)
+    ]
     layout2 = []
     for tensor_coord, coordinate_axis_name, expr_coord, ndim in layout:
-        axis_names = [axis.name for axis in expr_coord.all() if isinstance(axis, einx.expr.stage3.Axis)]
-        axis = axis_names.index(coordinate_axis_name) if coordinate_axis_name in axis_names else None
+        axis_names = [
+            axis.name for axis in expr_coord.all() if isinstance(axis, einx.expr.stage3.Axis)
+        ]
+        axis = (
+            axis_names.index(coordinate_axis_name) if coordinate_axis_name in axis_names else None
+        )
         if axis is None:
             assert ndim == 1
             layout2.append((tensor_coord, coordinate_axis_name, expr_coord))
         else:
             axes = [axis for axis in expr_coord.all() if isinstance(axis, einx.expr.stage3.Axis)]
             del axes[axis]
             expr_coord = einx.expr.stage3.List.maybe(axes)
             for i in range(ndim):
-                layout2.append((tensor_coord[(slice(None),) * axis + (i,)], coordinate_axis_name, expr_coord))
+                layout2.append((
+                    tensor_coord[(slice(None),) * axis + (i,)],
+                    coordinate_axis_name,
+                    expr_coord,
+                ))
     assert len(layout2) == tensor_in.ndim
     layout = layout2
 
     # Transpose coordinate and update tensors to match common coordinate expression
     def transpose(tensor, expr):
-        return util.transpose_broadcast(expr, tensor, expr_common, broadcast=False)[0]
-    tensor_coordinates = tuple(transpose(tensor, expr) for tensor, coordinate_axis_name, expr in layout)
+        return util.transpose_broadcast(
+            expr, tensor, expr_common, broadcast=False, backend=backend
+        )[0]
+
+    tensor_coordinates = tuple(
+        transpose(tensor, expr) for tensor, coordinate_axis_name, expr in layout
+    )
     if update:
         tensor_update = transpose(tensor_update, expr_update_inner)
 
-    return op(tensor_in, tensor_coordinates) if not update else op(tensor_in, tensor_coordinates, tensor_update)
+    return (
+        op(tensor_in, tensor_coordinates)
+        if not update
+        else op(tensor_in, tensor_coordinates, tensor_update)
+    )
+
 
-@einx.lru_cache(trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, **kwargs: c(exprs_in, [t(x) for x in tensors_in], expr_out, **kwargs))
+@einx.lru_cache(
+    trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, **kwargs: c(
+        exprs_in, [t(x) for x in tensors_in], expr_out, **kwargs
+    )
+)
 def index_stage3(exprs_in, tensors_in, expr_out, *, update, op=None, backend=None):
     if backend is None:
         backend = einx.backend.get(tensors_in)
     elif isinstance(backend, str):
         backend = einx.backend.get(backend)
     op = backend.op(op, tracable=False)
     if len(exprs_in) != len(tensors_in):
@@ -61,242 +86,456 @@
                 raise ValueError("Concatenation not allowed")
     if not update:
         # Ensure that no brackets exist in output expression
         for expr in expr_out.all():
             if einx.expr.stage3.is_marked(expr):
                 raise ValueError("Brackets in the output expression are not allowed")
     if update:
-        axis_names = set(axis.name for root in exprs_in[:-1] for axis in root.all() if isinstance(axis, einx.expr.stage3.Axis))
+        axis_names = {
+            axis.name
+            for root in exprs_in[:-1]
+            for axis in root.all()
+            if isinstance(axis, einx.expr.stage3.Axis)
+        }
         for axis in exprs_in[-1].all():
-            if isinstance(axis, einx.expr.stage3.Axis) and not axis.name in axis_names:
-                raise ValueError(f"Update expression cannot contain axes that are not in the coordinate or tensor expressions: {axis.name}")
+            if isinstance(axis, einx.expr.stage3.Axis) and axis.name not in axis_names:
+                raise ValueError(
+                    f"Update expression cannot contain axes that are not in the "
+                    f"coordinate or tensor expressions: {axis.name}"
+                )
 
     # Call tensor factories
     def get_name(s):
         if s == "get_at":
             return "embedding"
         else:
             return s
-    tensors_in = [einx.param.instantiate(tensor, expr.shape, backend, name=get_name(util._op_to_str(op)), init=util._op_to_str(op)) for tensor, expr in zip(tensors_in, exprs_in)]
+
+    tensors_in = [
+        einx.param.instantiate(
+            tensor,
+            expr.shape,
+            backend,
+            name=get_name(util._op_to_str(op)),
+            init=util._op_to_str(op),
+        )
+        for tensor, expr in zip(tensors_in, exprs_in)
+    ]
 
     expr_tensor = exprs_in[0]
-    exprs_coordinates = (exprs_in[1:-1] if update else exprs_in[1:])
+    exprs_coordinates = exprs_in[1:-1] if update else exprs_in[1:]
     if update:
         expr_update = exprs_in[-1]
 
     layout = []
     total_ndim = 0
     for expr_coord in exprs_coordinates:
-        marked_coordinate_axes = [expr for expr in expr_coord.all() if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr)]
+        marked_coordinate_axes = [
+            expr
+            for expr in expr_coord.all()
+            if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr)
+        ]
         if len(marked_coordinate_axes) > 1:
-            raise ValueError(f"Expected at most one coordinate axis in coordinate expression, got {len(marked_coordinate_axes)} in '{expr_coord}'")
+            raise ValueError(
+                f"Expected at most one coordinate axis in coordinate expression, "
+                f"got {len(marked_coordinate_axes)} in '{expr_coord}'"
+            )
         ndim = marked_coordinate_axes[0].value if len(marked_coordinate_axes) == 1 else 1
-        coordinate_axis_name = marked_coordinate_axes[0].name if len(marked_coordinate_axes) == 1 and (not marked_coordinate_axes[0].is_unnamed or marked_coordinate_axes[0].value != 1) else None
+        coordinate_axis_name = (
+            marked_coordinate_axes[0].name
+            if len(marked_coordinate_axes) == 1
+            and (not marked_coordinate_axes[0].is_unnamed or marked_coordinate_axes[0].value != 1)
+            else None
+        )
         layout.append((coordinate_axis_name, ndim))
         total_ndim += ndim
 
-    marked_tensor_axis_names = set(expr.name for expr in expr_tensor.all() if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr))
+    marked_tensor_axis_names = {
+        expr.name
+        for expr in expr_tensor.all()
+        if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr)
+    }
     if len(marked_tensor_axis_names) != total_ndim:
-        raise ValueError(f"Expected {total_ndim} marked axes in tensor, got {len(marked_tensor_axis_names)}")
+        raise ValueError(
+            f"Expected {total_ndim} marked axes in tensor, got {len(marked_tensor_axis_names)}"
+        )
 
     if update:
-        marked_update_axis_names = set(expr.name for expr in expr_update.all() if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr))
+        marked_update_axis_names = {
+            expr.name
+            for expr in expr_update.all()
+            if isinstance(expr, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(expr)
+        }
         if len(marked_update_axis_names) != 0:
-            raise ValueError(f"Update expression cannot contain marked axes")
+            raise ValueError("Update expression cannot contain marked axes")
 
     # Add markers around axes in coordinates and update that are not in tensor
-    tensor_axis_names = set(expr.name for expr in expr_tensor.all() if isinstance(expr, einx.expr.stage3.Axis))
+    tensor_axis_names = {
+        expr.name for expr in expr_tensor.all() if isinstance(expr, einx.expr.stage3.Axis)
+    }
     new_marked_axis_names = set()
+
     def replace(expr):
-        if isinstance(expr, einx.expr.stage3.Axis) and not expr.name in tensor_axis_names and not einx.expr.stage3.is_marked(expr):
+        if (
+            isinstance(expr, einx.expr.stage3.Axis)
+            and expr.name not in tensor_axis_names
+            and not einx.expr.stage3.is_marked(expr)
+        ):
             new_marked_axis_names.add(expr.name)
             return einx.expr.stage3.Marker(expr.__deepcopy__())
+
     exprs_coordinates = [einx.expr.stage3.replace(expr, replace) for expr in exprs_coordinates]
     expr_update = einx.expr.stage3.replace(expr_update, replace) if update else None
 
     # Add markers around those same axes in output and update
     def replace(expr):
-        if isinstance(expr, einx.expr.stage3.Axis) and expr.name in new_marked_axis_names and not einx.expr.stage3.is_marked(expr):
+        if (
+            isinstance(expr, einx.expr.stage3.Axis)
+            and expr.name in new_marked_axis_names
+            and not einx.expr.stage3.is_marked(expr)
+        ):
             return einx.expr.stage3.Marker(expr.__deepcopy__())
+
     expr_out = einx.expr.stage3.replace(expr_out, replace)
     if update:
         expr_update = einx.expr.stage3.replace(expr_update, replace)
 
-    # If updating: Add markers around axes in output that are also marked in tensor (and are not broadcasted axes)
+    # If updating: Add markers around axes in output that are also marked
+    # in tensor (and are not broadcasted axes)
     if update:
+
         def replace(expr):
-            if isinstance(expr, einx.expr.stage3.Axis) and expr.name in marked_tensor_axis_names and not einx.expr.stage3.is_marked(expr):
+            if (
+                isinstance(expr, einx.expr.stage3.Axis)
+                and expr.name in marked_tensor_axis_names
+                and not einx.expr.stage3.is_marked(expr)
+            ):
                 return einx.expr.stage3.Marker(expr.__deepcopy__())
+
         expr_out = einx.expr.stage3.replace(expr_out, replace)
 
     def to_inner(expr):
         expr = einx.expr.stage3.get_marked(expr)
         return util.flatten([expr])[0]
+
     exprs_coordinates_inner = [to_inner(expr) for expr in exprs_coordinates]
     expr_update_inner = to_inner(expr_update) if update else None
 
     # Find common expression for coordinates and update in vmapped function
-    layout = [(coordinate_axis_name, expr_coord, ndim) for expr_coord, (coordinate_axis_name, ndim) in zip(exprs_coordinates_inner, layout)]
+    layout = [
+        (coordinate_axis_name, expr_coord, ndim)
+        for expr_coord, (coordinate_axis_name, ndim) in zip(exprs_coordinates_inner, layout)
+    ]
     if update:
         layout2 = layout + [(None, expr_update_inner, None)]
         longest = sorted(layout2, key=lambda x: len(x[1].shape))[-1]
-        all_axes = [axis for axis in longest[1].all() if isinstance(axis, einx.expr.stage3.Axis) and not axis.name == longest[0]]
-        axes_names = set(axis.name for axis in all_axes)
-        for coordinate_axis_name, expr_coord, ndim in layout2:
+        all_axes = [
+            axis
+            for axis in longest[1].all()
+            if isinstance(axis, einx.expr.stage3.Axis) and not axis.name == longest[0]
+        ]
+        axes_names = {axis.name for axis in all_axes}
+        for coordinate_axis_name, expr_coord, _ in layout2:
             for axis in expr_coord.all():
-                if isinstance(axis, einx.expr.stage3.Axis) and axis.name != coordinate_axis_name and not axis.name in axes_names:
+                if (
+                    isinstance(axis, einx.expr.stage3.Axis)
+                    and axis.name != coordinate_axis_name
+                    and axis.name not in axes_names
+                ):
                     axes_names.add(axis.name)
                     all_axes.append(axis)
         expr_common = einx.expr.stage3.List.maybe(all_axes)
     else:
         expr_common = einx.expr.stage3.get_marked(util.flatten([expr_out])[0])
 
     # Construct vmapped indexing function
-    op = partial(_index, op=op, update=update, layout=layout, expr_common=expr_common, expr_update_inner=expr_update_inner)
+    op = partial(
+        _index,
+        op=op,
+        update=update,
+        layout=layout,
+        expr_common=expr_common,
+        expr_update_inner=expr_update_inner,
+        backend=backend,
+    )
     op = backend.op(op, tracable=True)
 
     exprs_in = [expr_tensor] + exprs_coordinates + ([expr_update] if update else [])
-    tensors_out, exprs_out = einx.vmap_stage3(exprs_in, tensors_in, [expr_out], op=op, flat=True, backend=backend)
+    tensors_out, exprs_out = einx.vmap_stage3(
+        exprs_in, tensors_in, [expr_out], op=op, flat=True, backend=backend
+    )
     assert len(tensors_out) == 1 and len(exprs_out) == 1
     return tensors_out[0], exprs_out[0]
 
+
 @einx.lru_cache
-def parse(description, *tensors_shapes, update, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
+def parse(description, *tensor_shapes, update, cse=True, **parameters):
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
 
-    description = description.split("->")
-    if update:
-        if len(description) == 1:
-            exprs_in = description[0]
-            exprs_in = exprs_in.split(",")
-            expr_out = exprs_in[0]
-        elif len(description) == 2:
-            exprs_in, expr_out = description
-            exprs_in = exprs_in.split(",")
-        else:
-            raise ValueError("Operation string must contain at most one '->'")
-    else:
-        if len(description) != 2:
-            raise ValueError("Operation string must contain exactly one '->'")
+    op = einx.expr.stage1.parse_op(description)
+
+    # Implicitiy determine output expression
+    if len(op) == 1:
+        if update:
+            op = einx.expr.stage1.Op([
+                op[0],
+                einx.expr.stage1.Args([op[0][0]]),
+            ])
         else:
-            exprs_in, expr_out = description
-            exprs_in = exprs_in.split(",")
-    if "," in expr_out:
-        raise ValueError("Only a single output expression is allowed")
-    if len(tensors_shapes) != len(exprs_in):
-        raise ValueError(f"Expected {len(exprs_in)} input tensors, got {len(tensors_shapes)}")
+            raise ValueError("Operation string must contain an output expression")
+
+    if len(op[0]) != len(tensor_shapes):
+        raise ValueError(f"Expected {len(op[0])} input tensors, but got {len(tensor_shapes)}")
+    if len(op[1]) != 1:
+        raise ValueError(f"Expected 1 output expression, but got {len(op[1])}")
 
     def after_stage2(exprs1, exprs2):
         for expr in exprs1[0].all():
-            if isinstance(expr, einx.expr.stage2.UnnamedAxis) and expr.value == 1 and einx.expr.stage2.is_marked(expr):
+            if (
+                isinstance(expr, einx.expr.stage2.UnnamedAxis)
+                and expr.value == 1
+                and einx.expr.stage2.is_marked(expr)
+            ):
                 raise ValueError("First expression cannot contain unnamed axes with value 1")
-        tensor_marked_axes = [expr for expr in exprs1[0].all() if isinstance(expr, (einx.expr.stage2.NamedAxis, einx.expr.stage2.UnnamedAxis)) and einx.expr.stage2.is_marked(expr)]
+        tensor_marked_axes = [
+            expr
+            for expr in exprs1[0].all()
+            if isinstance(expr, (einx.expr.stage2.NamedAxis, einx.expr.stage2.UnnamedAxis))
+            and einx.expr.stage2.is_marked(expr)
+        ]
         ndim = len(tensor_marked_axes)
 
         concat_this = []
 
-        coord_exprs = exprs1[1:len(tensors_shapes)]
+        coord_exprs = exprs1[1 : len(tensor_shapes)]
         if update:
             coord_exprs = coord_exprs[:-1]
         for expr in coord_exprs:
-            marked_coordinate_axes = [expr for expr in exprs1[1].all() if isinstance(expr, (einx.expr.stage2.NamedAxis, einx.expr.stage2.UnnamedAxis)) and einx.expr.stage2.is_marked(expr)]
+            marked_coordinate_axes = [
+                expr
+                for expr in exprs1[1].all()
+                if isinstance(expr, (einx.expr.stage2.NamedAxis, einx.expr.stage2.UnnamedAxis))
+                and einx.expr.stage2.is_marked(expr)
+            ]
             if len(marked_coordinate_axes) > 1:
-                raise ValueError(f"Expected at most one marked axis per coordinate tensor, got {len(marked_coordinate_axes)}")
+                raise ValueError(
+                    f"Expected at most one marked axis per coordinate tensor"
+                    f", got {len(marked_coordinate_axes)}"
+                )
             elif len(marked_coordinate_axes) == 1:
                 if isinstance(marked_coordinate_axes[0], einx.expr.stage2.NamedAxis):
                     concat_this.append(einx.expr.stage1.NamedAxis(marked_coordinate_axes[0].name))
                 else:
-                    concat_this.append(einx.expr.stage1.UnnamedAxis(marked_coordinate_axes[0].value))
+                    concat_this.append(
+                        einx.expr.stage1.UnnamedAxis(marked_coordinate_axes[0].value)
+                    )
             else:
                 concat_this.append(einx.expr.stage1.UnnamedAxis(1))
 
-        return [einx.expr.Equation(einx.expr.stage1.Concatenation.maybe(concat_this), np.asarray([ndim]))]
+        return [
+            einx.expr.Equation(
+                einx.expr.stage1.Concatenation.maybe(concat_this), np.asarray([ndim])
+            )
+        ]
 
     exprs = einx.expr.solve(
-            [einx.expr.Equation(expr_in, tensor_shape) for expr_in, tensor_shape in zip(exprs_in, tensors_shapes)] \
-          + [einx.expr.Equation(expr_out)] \
-          + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+        [
+            einx.expr.Equation(expr_in, tensor_shape)
+            for expr_in, tensor_shape in zip(op[0], tensor_shapes)
+        ]
+        + [einx.expr.Equation(op[1][0])]
+        + [
+            einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+            for k, v in parameters.items()
+        ],
         cse=cse,
         after_stage2=after_stage2,
-    )[:len(exprs_in) + 1]
-    exprs_in, expr_out = exprs[:len(exprs_in)], exprs[len(exprs_in)]
+    )[: len(op[0]) + 1]
+    exprs_in, expr_out = exprs[: len(op[0])], exprs[len(op[0])]
+
+    if update:
+        # Check that all axes in first input expression also appear in output expression
+        axes_in = {
+            axis.name for axis in exprs_in[0].all() if isinstance(axis, einx.expr.stage3.Axis)
+        }
+        axes_out = {axis.name for axis in expr_out.all() if isinstance(axis, einx.expr.stage3.Axis)}
+        if not axes_in.issubset(axes_out):
+            raise ValueError(
+                f"Output expression does not contain all axes from first input expression: "
+                f"{axes_in - axes_out}"
+            )
 
     return exprs_in, expr_out
 
-@einx.lru_cache(trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(description, *[t(x) for x in tensors], **kwargs))
-def index(description: str, *tensors: einx.Tensor, op: Callable, update: bool, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+def _has_zero_shape(tensor):
+    shape = einx.param.get_shape(tensor)
+    return shape is not None and any(s == 0 for s in shape)
+
+
+@einx.traceback_util.filter
+@einx.lru_cache(
+    trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
+        description, *[t(x) for x in tensors], **kwargs
+    )
+)
+def index(
+    description: str,
+    *tensors: einx.Tensor,
+    op: Callable,
+    update: bool,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Updates and/ or returns values from an array at the given coordinates.
 
-    The `description` argument specifies the input and output expressions and must meet one of the following formats:
+    The `description` argument specifies the input and output expressions and must meet one of
+    the following formats:
 
     1. ``tensor, coordinates1, coordinates2, ..., update -> output``
        when modifying values in the tensor.
     2. ``tensor, coordinates1, coordinates2, ... -> output``
        when only returning values from the tensor.
 
-    Brackets in the ``tensor`` expression mark the axes that will be indexed. Brackets in the ``coordinates`` expression mark the single coordinate axis. All other
-    axes are considered batch axes. Using multiple coordinate expressions will yield the same output as concatenating the coordinate expressions along the coordinate axis first.
+    Brackets in the ``tensor`` expression mark the axes that will be indexed. Brackets in the
+    ``coordinates`` expression mark the single coordinate axis. All other axes are considered
+    batch axes. Using multiple coordinate expressions will yield the same output as concatenating
+    the coordinate expressions along the coordinate axis first.
 
     Args:
         description: Description string in Einstein notation (see above).
-        *tensors: Tensors that the operation will be applied to. The first tensor will receive updates, the last tensor contains the updates, and all other tensors represent the coordinates.
-        op: The update/gather function. If `op` is a string, retrieves the attribute of `backend` with the same name.
+        *tensors: Tensors that the operation will be applied to. The first tensor will receive
+            updates, the last tensor contains the updates, and all other tensors represent
+            the coordinates.
+        op: The update/gather function. If `op` is a string, retrieves the attribute of `backend`
+            with the same name.
         update: Whether to update the tensor or return values from the tensor.
-        backend: Backend to use for all operations. If None, determines the backend from the input tensors. Defaults to None.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to True.
-        graph: Whether to return the graph representation of the operation instead of computing the result. Defaults to False.
+        backend: Backend to use for all operations. If None, determines the backend from the
+            input tensors. Defaults to None.
+        cse: Whether to apply common subexpression elimination to the expressions. Defaults
+            to True.
+        graph: Whether to return the graph representation of the operation instead of computing
+            the result. Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
-        The result of the update/ gather operation if `graph=False`, otherwise the graph representation of the operation.
+        The result of the update/ gather operation if `graph=False`, otherwise the graph
+        representation of the operation.
 
     Examples:
         Get values from a batch of images (different indices per image):
 
         >>> tensor = np.random.uniform(size=(4, 128, 128, 3))
         >>> coordinates = np.ones((4, 100, 2))
         >>> einx.get_at("b [h w] c, b p [2] -> b p c", tensor, coordinates).shape
         (4, 100, 3)
 
         >>> tensor = np.random.uniform(size=(4, 128, 128, 3))
         >>> coordinates_x = np.ones((4, 100), "int32")
         >>> coordinates_y = np.ones((4, 100), "int32")
-        >>> einx.get_at("b [h w] c, b p, b p -> b p c", tensor, coordinates_x, coordinates_y).shape
+        >>> einx.get_at(
+        ...     "b [h w] c, b p, b p -> b p c",
+        ...     tensor,
+        ...     coordinates_x,
+        ...     coordinates_y,
+        ... ).shape
         (4, 100, 3)
 
         Set values in a batch of images (same indices per image):
 
         >>> tensor = np.random.uniform(size=(4, 128, 128, 3))
         >>> coordinates = np.ones((100, 2), "int32")
         >>> updates = np.random.uniform(size=(100, 3))
-        >>> einx.set_at("b [h w] c, p [2], p c -> b [h w] c", tensor, coordinates, updates).shape
+        >>> einx.set_at(
+        ...     "b [h w] c, p [2], p c -> b [h w] c", tensor, coordinates, updates
+        ... ).shape
         (4, 128, 128, 3)
 
         >>> tensor = np.random.uniform(size=(4, 128, 128, 3))
         >>> coordinates_x = np.ones((100,), "int32")
         >>> coordinates_y = np.ones((100,), "int32")
         >>> updates = np.random.uniform(size=(100, 3))
-        >>> einx.set_at("b [h w] c, p, p, p c -> b [h w] c", tensor, coordinates_x, coordinates_y, updates).shape
+        >>> einx.set_at(
+        ...     "b [h w] c, p, p, p c -> b [h w] c",
+        ...     tensor,
+        ...     coordinates_x,
+        ...     coordinates_y,
+        ...     updates,
+        ... ).shape
         (4, 128, 128, 3)
     """
-    exprs_in, expr_out = parse(description, *[einx.param.get_shape(tensor) for tensor in tensors], update=update, cse=cse, **parameters)
-    tensor, expr_out = index_stage3(exprs_in, tensors, expr_out, op=op, update=update, backend=backend)
+    if update and any(_has_zero_shape(tensor) for tensor in tensors[1:]):
+        # Skip update if no coordinates are given
+        return tensors[0]
+    exprs_in, expr_out = parse(
+        description,
+        *[einx.param.get_shape(tensor) for tensor in tensors],
+        update=update,
+        cse=cse,
+        **parameters,
+    )
+    tensor, expr_out = index_stage3(
+        exprs_in, tensors, expr_out, op=op, update=update, backend=backend
+    )
     return tensor
-index.parse = parse
 
 
+index.parse = parse
+
 
-def get_at(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+@einx.traceback_util.filter
+def get_at(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.index` with ``op="get_at"`` and ``update=False``"""
-    return index(description, *tensors, op="get_at", update=False, backend=backend, cse=cse, **parameters)
+    return index(
+        description, *tensors, op="get_at", update=False, backend=backend, cse=cse, **parameters
+    )
 
-def set_at(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def set_at(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.index` with ``op="set_at"`` and ``update=True``"""
-    return index(description, *tensors, op="set_at", update=True, backend=backend, cse=cse, **parameters)
+    return index(
+        description, *tensors, op="set_at", update=True, backend=backend, cse=cse, **parameters
+    )
+
 
-def add_at(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+@einx.traceback_util.filter
+def add_at(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.index` with ``op="add_at"`` and ``update=True``"""
-    return index(description, *tensors, op="add_at", update=True, backend=backend, cse=cse, **parameters)
+    return index(
+        description, *tensors, op="add_at", update=True, backend=backend, cse=cse, **parameters
+    )
+
 
-def subtract_at(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+@einx.traceback_util.filter
+def subtract_at(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.index` with ``op="subtract_at"`` and ``update=True``"""
-    return index(description, *tensors, op="subtract_at", update=True, backend=backend, cse=cse, **parameters)
+    return index(
+        description, *tensors, op="subtract_at", update=True, backend=backend, cse=cse, **parameters
+    )
```

### Comparing `einx-0.1.3/einx/op/rearrange.py` & `einx-0.2.0/einx/op/rearrange.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,91 +1,130 @@
 import einx
 from . import util
 import numpy as np
 from typing import Union, Tuple
 import numpy.typing as npt
 
-@einx.lru_cache(trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, backend=None: c(exprs_in, [t(x) for x in tensors_in], exprs_out))
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, backend=None: c(
+        exprs_in, [t(x) for x in tensors_in], exprs_out
+    )
+)
 def rearrange_stage3(exprs_in, tensors_in, exprs_out, backend=None):
     if backend is None:
         backend = einx.backend.get(tensors_in)
     elif isinstance(backend, str):
         backend = einx.backend.get(backend)
     if len(exprs_in) != len(tensors_in):
         raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensors_in)}")
-    if any(isinstance(expr, einx.expr.stage3.Marker) for root in list(exprs_in) + list(exprs_out) for expr in root.all()):
+    if any(
+        isinstance(expr, einx.expr.stage3.Marker)
+        for root in list(exprs_in) + list(exprs_out)
+        for expr in root.all()
+    ):
         raise ValueError(f"Marker '{expr}' is not allowed")
 
     # Call tensor factories
-    tensors_in = [einx.param.instantiate(tensor, expr.shape, backend, name="embedding", init="rearrange") for tensor, expr in zip(tensors_in, exprs_in)]
+    tensors_in = [
+        einx.param.instantiate(tensor, expr.shape, backend, name="embedding", init="rearrange")
+        for tensor, expr in zip(tensors_in, exprs_in)
+    ]
 
     # Flatten expressions
-    exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend)
+    exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend=backend)
     exprs_out_flat = util.flatten(exprs_out)
     assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_in)
     assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_out_flat)
     if len(exprs_in) != len(exprs_out_flat):
-        raise ValueError(f"Got different number of input ({len(exprs_in)}) and output expressions ({len(exprs_out_flat)}) (after flattening)") # TODO:
+        raise ValueError(
+            f"Got different number of input ({len(exprs_in)}) and output expressions "
+            f"({len(exprs_out_flat)}) (after flattening)"
+        )  # TODO:
 
     # Order inputs to align with output expressions
     indices = util.assignment(exprs_in, exprs_out_flat)
     exprs_in = [exprs_in[i] for i in indices]
     tensors_in = [tensors_in[i] for i in indices]
 
     # Transpose and broadcast missing output dimensions
-    tensors = [util.transpose_broadcast(expr_in, tensor, expr_out)[0] for expr_in, tensor, expr_out in zip(exprs_in, tensors_in, exprs_out_flat)]
+    tensors = [
+        util.transpose_broadcast(expr_in, tensor, expr_out, backend=backend)[0]
+        for expr_in, tensor, expr_out in zip(exprs_in, tensors_in, exprs_out_flat)
+    ]
 
     # Unflatten output expressions
-    tensors = util.unflatten(exprs_out_flat, tensors, exprs_out, backend)
+    tensors = util.unflatten(exprs_out_flat, tensors, exprs_out, backend=backend)
 
     return tensors, exprs_out
 
+
 @einx.lru_cache
 def parse(description, *tensor_shapes, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
+
+    op = einx.expr.stage1.parse_op(description)
 
-    description = description.split("->")
-    if len(description) != 2:
-        raise ValueError("Operation must contain exactly one '->'")
-    exprs_in, exprs_out = description
-    exprs_in = exprs_in.split(",")
-    exprs_out = exprs_out.split(",")
-    exprs = exprs_in + exprs_out
-    if len(exprs_in) != len(tensor_shapes):
-        raise ValueError(f"Expected {len(exprs_in)} input tensors, got {len(tensor_shapes)}")
+    if len(op[0]) != len(tensor_shapes):
+        raise ValueError(f"Expected {len(op[0])} input tensors, but got {len(tensor_shapes)}")
 
     exprs = einx.expr.solve(
-            [einx.expr.Equation(expr_in, tensor_shape) for expr_in, tensor_shape in zip(exprs_in, tensor_shapes)] \
-          + [einx.expr.Equation(expr_out) for expr_out in exprs_out] \
-          + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+        [
+            einx.expr.Equation(expr_in, tensor_shape)
+            for expr_in, tensor_shape in zip(op[0], tensor_shapes)
+        ]
+        + [einx.expr.Equation(expr_out) for expr_out in op[1]]
+        + [
+            einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+            for k, v in parameters.items()
+        ],
         cse=cse,
-    )[:len(exprs_in) + len(exprs_out)]
-    exprs_in, exprs_out = exprs[:len(exprs_in)], exprs[len(exprs_in):]
+    )[: len(op[0]) + len(op[1])]
+    exprs_in, exprs_out = exprs[: len(op[0])], exprs[len(op[0]) :]
 
     return exprs_in, exprs_out
 
-@einx.lru_cache(trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(description, *[t(x) for x in tensors], **kwargs))
-def rearrange(description: str, *tensors: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> Union[einx.Tensor, Tuple[einx.Tensor, ...]]:
+
+@einx.traceback_util.filter
+@einx.lru_cache(
+    trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
+        description, *[t(x) for x in tensors], **kwargs
+    )
+)
+def rearrange(
+    description: str,
+    *tensors: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> Union[einx.Tensor, Tuple[einx.Tensor, ...]]:
     """Rearranges the input tensors to match the output expressions.
 
     See :doc:`How does einx handle input and output tensors? </faq/flatten>`.
 
-    The `description` argument specifies the input and output expressions. It must meet the following format:
+    The `description` argument specifies the input and output expressions. It must
+    meet the following format:
     ``input1, input2, ... -> output1, output2, ...``
 
     Args:
         description: Description string in Einstein notation (see above).
         tensors: Input tensors or tensor factories matching the description string.
-        backend: Backend to use for all operations. If None, determines the backend from the input tensors. Defaults to None.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to True.
-        graph: Whether to return the graph representation of the operation instead of computing the result. Defaults to False.
+        backend: Backend to use for all operations. If None, determines the backend from
+            the input tensors. Defaults to None.
+        cse: Whether to apply common subexpression elimination to the expressions. Defaults
+            to True.
+        graph: Whether to return the graph representation of the operation instead of
+            computing the result. Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
-        The result of the elementwise operation if `graph=False`, otherwise the graph representation of the operation.
+        The result of the elementwise operation if `graph=False`, otherwise the graph
+        representation of the operation.
 
     Examples:
         Transpose the row and column axes of a batch of images:
 
         >>> x = np.random.uniform(size=(4, 64, 48, 3))
         >>> einx.rearrange("b h w c -> b w h c", x).shape
         (4, 48, 64, 3,)
@@ -94,15 +133,18 @@
 
         >>> x = np.random.uniform(size=(10, 10))
         >>> einx.rearrange("a b -> a c b", x, c=100).shape
         (10, 100, 10,)
 
         Concatenate two tensors along the first axis:
 
-        >>> a, b = np.random.uniform(size=(10, 10)), np.random.uniform(size=(20, 10))
+        >>> a, b = (
+        ...     np.random.uniform(size=(10, 10)),
+        ...     np.random.uniform(size=(20, 10)),
+        ... )
         >>> einx.rearrange("a b, c b -> (a + c) b", a, b).shape
         (30, 10,)
 
         Split a tensor:
 
         >>> x = np.random.uniform(size=(10, 2))
         >>> a, b = einx.rearrange("a (1 + 1) -> a, a", x)
@@ -111,11 +153,15 @@
 
         Swap the first and last third of a tensor along a given axis:
 
         >>> x = np.arange(6)
         >>> einx.rearrange("(b + c + d) -> (d + c + b)", x, b=2, c=2)
         array([4, 5, 2, 3, 0, 1])
     """
-    exprs_in, exprs_out = parse(description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters)
+    exprs_in, exprs_out = parse(
+        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+    )
     tensors, exprs_out = rearrange_stage3(exprs_in, tensors, exprs_out, backend=backend)
     return tensors[0] if len(exprs_out) == 1 else tensors
+
+
 rearrange.parse = parse
```

### Comparing `einx-0.1.3/einx/op/reduce.py` & `einx-0.2.0/einx/op/reduce.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,109 +1,154 @@
 import einx
 from . import util
 import numpy as np
 from functools import partial
 from typing import Callable, Union
 import numpy.typing as npt
 
-_any = any # Is overwritten below
+_any = any  # Is overwritten below
 
-@einx.lru_cache(trace=lambda t, c: lambda expr_in, tensor_in, expr_out, op, backend=None: c(expr_in, t(tensor_in), expr_out, op=op))
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda expr_in, tensor_in, expr_out, op, backend=None: c(
+        expr_in, t(tensor_in), expr_out, op=op
+    )
+)
 def reduce_stage3(expr_in, tensor_in, expr_out, op, backend=None):
     for root in [expr_in, expr_out]:
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Concatenation):
                 raise ValueError("Concatenation not allowed")
-    tensors_out, exprs_out = einx.vmap_with_axis_stage3([expr_in], [tensor_in], [expr_out], op, backend=backend)
+    tensors_out, exprs_out = einx.vmap_with_axis_stage3(
+        [expr_in], [tensor_in], [expr_out], op, backend=backend
+    )
     return tensors_out[0], exprs_out[0]
 
+
 @einx.lru_cache
 def parse(description, tensor_shape, keepdims=None, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
-
-    if "," in description:
-        raise ValueError("Only a single input and output expression is allowed")
-
-    if "->" in description:
-        if not keepdims is None:
-            raise ValueError("keepdims cannot be given when using '->'")
-        description = description.split("->")
-        if len(description) != 2:
-            raise ValueError("Operation cannot contain more than one '->'")
-
-        expr_in, expr_out = description
-
-        expr_in, expr_out = einx.expr.solve(
-                [einx.expr.Equation(expr_in, tensor_shape)] \
-              + [einx.expr.Equation(expr_out)] \
-              + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
-            cse=cse,
-            cse_in_markers=True,
-        )[:2]
-
-        # If no axes are marked for reduction in expr_in, mark all axes that don't appear in expr_out
-        if not _any(einx.expr.stage3.is_marked(expr) for expr in expr_in.all()):
-            axes_names_out = set(axis.name for axis in expr_out.all() if isinstance(axis, einx.expr.stage3.Axis))
-            expr_in = einx.expr.stage3.mark(expr_in, lambda expr: isinstance(expr, einx.expr.stage3.Axis) and expr.name not in axes_names_out)
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
 
-    else:
-        expr_in = description
+    op = einx.expr.stage1.parse_op(description)
 
+    if len(op) == 1:
         expr_in = einx.expr.solve(
-                [einx.expr.Equation(expr_in, tensor_shape)] \
-              + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+            [einx.expr.Equation(op[0][0], tensor_shape)]
+            + [
+                einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+                for k, v in parameters.items()
+            ],
             cse=cse,
             cse_in_markers=True,
         )[0]
 
         if not _any(isinstance(expr, einx.expr.stage3.Marker) for expr in expr_in.all()):
             raise ValueError("No axes are marked for reduction")
 
         # Determine output expressions by removing markers from input expressions
         def replace(expr):
             if isinstance(expr, einx.expr.stage3.Marker):
                 if keepdims:
                     return [einx.expr.stage3.Axis(None, 1)]
                 else:
                     return []
+
         expr_out = einx.expr.stage3.replace(expr_in, replace)
 
+    else:
+        if keepdims is not None:
+            raise ValueError("keepdims cannot be given when using '->'")
+
+        if len(op[0]) != 1:
+            raise ValueError(f"Expected 1 input expression, but got {len(op[0])}")
+        if len(op[1]) != 1:
+            raise ValueError(f"Expected 1 output expression, but got {len(op[1])}")
+
+        expr_in, expr_out = einx.expr.solve(
+            [einx.expr.Equation(op[0][0], tensor_shape)]
+            + [einx.expr.Equation(op[1][0])]
+            + [
+                einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+                for k, v in parameters.items()
+            ],
+            cse=cse,
+            cse_in_markers=True,
+        )[:2]
+
+        # If no axes are marked for reduction in expr_in, mark all axes that
+        # don't appear in expr_out
+        if not _any(einx.expr.stage3.is_marked(expr) for expr in expr_in.all()):
+            axes_names_out = {
+                axis.name for axis in expr_out.all() if isinstance(axis, einx.expr.stage3.Axis)
+            }
+            expr_in = einx.expr.stage3.mark(
+                expr_in,
+                lambda expr: isinstance(expr, einx.expr.stage3.Axis)
+                and expr.name not in axes_names_out,
+            )
+
     return expr_in, expr_out
 
-@einx.lru_cache(trace=lambda t, c: lambda description, tensor, backend=None, **kwargs: c(description, t(tensor), **kwargs))
-def reduce(description: str, tensor: einx.Tensor, op: Union[Callable, str], keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+@einx.lru_cache(
+    trace=lambda t, c: lambda description, tensor, backend=None, **kwargs: c(
+        description, t(tensor), **kwargs
+    )
+)
+def reduce(
+    description: str,
+    tensor: einx.Tensor,
+    op: Union[Callable, str],
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Applies a reduction operation on the given tensors.
 
     The function flattens all input tensors, applies the given reduction operation and rearranges
-    the result to match the output expression (see :doc:`How does einx handle input and output tensors? </faq/flatten>`).
+    the result to match the output expression (see :doc:`How does einx handle input and
+    output tensors? </faq/flatten>`).
 
-    The `description` argument specifies the input and output expressions, as well as reduced axes. It must meet one of the following formats:
+    The `description` argument specifies the input and output expressions, as well as
+    reduced axes. It must meet one of the following formats:
 
     1. ``input -> output``
-        Input and output expressions are specified explicitly. Reduced axes are marked with ``[]``-brackets in the input expression. If no axes are
+        Input and output expressions are specified explicitly. Reduced axes are marked
+        with ``[]``-brackets in the input expression. If no axes are
         marked, reduces all axes that do not appear in the output expression.
 
     2. ``input``
-        A single input expression is specified. Reduced axes are marked with ``[]``-brackets. The output expression is determined by removing all marked expressions
+        A single input expression is specified. Reduced axes are marked with ``[]``-brackets.
+        The output expression is determined by removing all marked expressions
         from the input expression.
 
         Example: ``a [b]`` resolves to ``a b -> a``.
 
     Args:
         description: Description string in Einstein notation (see above).
         tensor: Input tensor or tensor factory matching the description string.
-        op: Backend reduction operation. Is called with ``op(tensor, axis=...)``. If `op` is a string, retrieves the attribute of `backend` with the same name.
-        keepdims: Whether to replace marked expressions with 1s instead of dropping them. Must be None when `description` already contains an output expression. Defaults to None.
-        backend: Backend to use for all operations. If None, determines the backend from the input tensors. Defaults to None.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to True.
-        graph: Whether to return the graph representation of the operation instead of computing the result. Defaults to False.
+        op: Backend reduction operation. Is called with ``op(tensor, axis=...)``. If `op` is
+            a string, retrieves the attribute of `backend` with the same name.
+        keepdims: Whether to replace marked expressions with 1s instead of dropping them. Must
+            be None when `description` already contains an output expression. Defaults to None.
+        backend: Backend to use for all operations. If None, determines the backend from the
+            input tensors. Defaults to None.
+        cse: Whether to apply common subexpression elimination to the expressions. Defaults
+            to True.
+        graph: Whether to return the graph representation of the operation instead of
+            computing the result. Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
-        The result of the reduction operation if ``graph=False``, otherwise the graph representation of the operation.
+        The result of the reduction operation if ``graph=False``, otherwise the graph
+        representation of the operation.
 
     Examples:
         Compute mean along rows of a matrix:
 
         >>> x = np.random.uniform(size=(16, 20))
         >>> einx.mean("a b -> b", x).shape
         (20,)
@@ -126,90 +171,223 @@
 
         Compute variance per channel over an image:
 
         >>> x = np.random.uniform(size=(256, 256, 3))
         >>> einx.var("[...] c", x).shape
         (3,)
     """
-    expr_in, expr_out = parse(description, einx.param.get_shape(tensor), keepdims=keepdims, cse=cse, **parameters)
+    expr_in, expr_out = parse(
+        description, einx.param.get_shape(tensor), keepdims=keepdims, cse=cse, **parameters
+    )
     tensor, expr_out = reduce_stage3(expr_in, tensor, expr_out, op=op, backend=backend)
     return tensor
-reduce.parse = parse
 
 
+reduce.parse = parse
+
 
-def sum(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+@einx.traceback_util.filter
+def sum(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="sum"``"""
-    return reduce(description, tensor, op="sum", keepdims=keepdims, backend=backend, cse=cse, **parameters)
+    return reduce(
+        description, tensor, op="sum", keepdims=keepdims, backend=backend, cse=cse, **parameters
+    )
+
 
 def sum_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="sum", **kwargs)
 
-def mean(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def mean(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="mean"``"""
-    return reduce(description, tensor, op="mean", keepdims=keepdims, backend=backend, cse=cse, **parameters)
+    return reduce(
+        description, tensor, op="mean", keepdims=keepdims, backend=backend, cse=cse, **parameters
+    )
+
 
 def mean_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="mean", **kwargs)
 
-def var(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def var(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="var"``"""
-    return reduce(description, tensor, op="var", keepdims=keepdims, backend=backend, cse=cse, **parameters)
+    return reduce(
+        description, tensor, op="var", keepdims=keepdims, backend=backend, cse=cse, **parameters
+    )
+
 
 def var_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="var", **kwargs)
 
-def std(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def std(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="std"``"""
-    return reduce(description, tensor, op="std", keepdims=keepdims, backend=backend, cse=cse, **parameters)
+    return reduce(
+        description, tensor, op="std", keepdims=keepdims, backend=backend, cse=cse, **parameters
+    )
+
 
 def std_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="std", **kwargs)
 
-def prod(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def prod(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="prod"``"""
-    return reduce(description, tensor, op="prod", keepdims=keepdims, backend=backend, cse=cse, **parameters)
+    return reduce(
+        description, tensor, op="prod", keepdims=keepdims, backend=backend, cse=cse, **parameters
+    )
+
 
 def prod_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="prod", **kwargs)
 
-def count_nonzero(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def count_nonzero(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="count_nonzero"``"""
-    return reduce(description, tensor, op="count_nonzero", keepdims=keepdims, backend=backend, cse=cse, **parameters)
+    return reduce(
+        description,
+        tensor,
+        op="count_nonzero",
+        keepdims=keepdims,
+        backend=backend,
+        cse=cse,
+        **parameters,
+    )
+
 
 def count_nonzero_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="count_nonzero", **kwargs)
 
-def any(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def any(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="any"``"""
-    return reduce(description, tensor, op="any", keepdims=keepdims, backend=backend, cse=cse, **parameters)
+    return reduce(
+        description, tensor, op="any", keepdims=keepdims, backend=backend, cse=cse, **parameters
+    )
+
 
 def any_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="any", **kwargs)
 
-def all(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def all(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="all"``"""
-    return reduce(description, tensor, op="all", keepdims=keepdims, backend=backend, cse=cse, **parameters)
+    return reduce(
+        description, tensor, op="all", keepdims=keepdims, backend=backend, cse=cse, **parameters
+    )
+
 
 def all_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="all", **kwargs)
 
-def max(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def max(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="max"``"""
     return reduce(description, tensor, op="max", keepdims=keepdims, backend=backend, **parameters)
 
+
 def max_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="max", **kwargs)
 
-def min(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def min(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="min"``"""
     return reduce(description, tensor, op="min", keepdims=keepdims, backend=backend, **parameters)
 
+
 def min_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="min", **kwargs)
 
-def logsumexp(description: str, tensor: einx.Tensor, keepdims: Union[bool, None] = None, backend: Union[einx.Backend, str, None] = None, **parameters: npt.ArrayLike) -> einx.Tensor:
+
+@einx.traceback_util.filter
+def logsumexp(
+    description: str,
+    tensor: einx.Tensor,
+    keepdims: Union[bool, None] = None,
+    backend: Union[einx.Backend, str, None] = None,
+    **parameters: npt.ArrayLike,
+) -> einx.Tensor:
     """Specialization of :func:`einx.reduce` with ``op="logsumexp"``"""
-    return reduce(description, tensor, op="logsumexp", keepdims=keepdims, backend=backend, **parameters)
+    return reduce(
+        description, tensor, op="logsumexp", keepdims=keepdims, backend=backend, **parameters
+    )
+
 
 def logsumexp_stage3(*args, **kwargs):
     return reduce_stage3(*args, op="logsumexp", **kwargs)
```

### Comparing `einx-0.1.3/einx/op/solve.py` & `einx-0.2.0/einx/op/solve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,139 @@
 import einx
 import numpy as np
 from collections import defaultdict
 from typing import Mapping, Optional
 import numpy.typing as npt
 
+
 @einx.lru_cache
 def _solve(description, *tensor_shapes, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
 
-    exprs = description.split(",")
+    exprs = einx.expr.stage1.parse_args(description)
     if len(exprs) != len(tensor_shapes):
         raise ValueError(f"Expected {len(exprs)} tensors, got {len(tensor_shapes)}")
 
     try:
         exprs = einx.expr.solve(
-              [einx.expr.Equation(expr, tensor_shape) for expr, tensor_shape in zip(exprs, tensor_shapes)] \
-            + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+            [
+                einx.expr.Equation(expr, tensor_shape)
+                for expr, tensor_shape in zip(exprs, tensor_shapes)
+            ]
+            + [
+                einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+                for k, v in parameters.items()
+            ],
             cse=cse,
         )
-    except (einx.expr.stage2.SolveDepthException, einx.expr.stage2.SolveExpansionException, einx.expr.stage3.SolveValueException):
+    except (
+        einx.expr.stage2.SolveDepthException,
+        einx.expr.stage2.SolveExpansionException,
+        einx.expr.stage3.SolveValueException,
+    ):
         return None
 
     values = defaultdict(list)
     for root in exprs:
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Axis):
                 tokens = expr.name.split(".")
                 values[tokens[0]].append((tuple(int(t) for t in tokens[1:]), expr.value))
-    
+
     values2 = {}
     for name, xs in values.items():
         shape = np.amax([coord for coord, value in xs], axis=0) + 1
         value = np.zeros(shape, dtype="int32")
         for coord, v in xs:
             value[coord] = v
         if value.shape == ():
             value = int(value)
         values2[name] = value
 
     return values2
 
-def solve(description: str, *tensors: einx.Tensor, cse: bool = False, **parameters: npt.ArrayLike) -> Optional[Mapping[str, npt.ArrayLike]]:
+
+def solve(
+    description: str, *tensors: einx.Tensor, cse: bool = False, **parameters: npt.ArrayLike
+) -> Optional[Mapping[str, npt.ArrayLike]]:
     """Solve for the axis values of the given expressions and tensors.
 
     The `description` argument must meet the following format:
     ``input1, input2, ...``
 
     Args:
         description: Description string in Einstein notation.
         tensors: Input tensors or tensor factories matching the description string.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to False.
+        cse: Whether to apply common subexpression elimination to the expressions.
+            Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
         A mapping from axis name to axis value, or ``None`` if no solution was found.
 
     Examples:
         >>> x = np.zeros((10, 5))
         >>> einx.solve("a b", x)
         {'a': 10, 'b': 5}
     """
-    return _solve(description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters)
+    return _solve(
+        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+    )
 
-def matches(description: str, *tensors: einx.Tensor, cse: bool = True, **parameters: npt.ArrayLike) -> bool:
+
+def matches(
+    description: str, *tensors: einx.Tensor, cse: bool = True, **parameters: npt.ArrayLike
+) -> bool:
     """Check whether the given expressions and tensors match.
 
     The `description` argument must meet the following format:
     ``input1, input2, ...``
 
     Args:
         description: Description string in Einstein notation.
         tensors: Input tensors or tensor factories matching the description string.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to False.
+        cse: Whether to apply common subexpression elimination to the expressions.
+            Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
         True if the expressions and tensors match, False otherwise.
     """
-    return not solve(description, *tensors, cse=cse, **parameters) is None
+    return solve(description, *tensors, cse=cse, **parameters) is not None
+
 
-def check(description: str, *tensors: einx.Tensor, cse: bool = True, **parameters: npt.ArrayLike) -> None:
+@einx.traceback_util.filter
+def check(
+    description: str, *tensors: einx.Tensor, cse: bool = True, **parameters: npt.ArrayLike
+) -> None:
     """Check whether the given expressions and tensors match and raise an exception if they don't.
 
     The `description` argument must meet the following format:
     ``input1, input2, ...``
 
     Args:
         description: Description string in Einstein notation.
         tensors: Input tensors or tensor factories matching the description string.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to False.
+        cse: Whether to apply common subexpression elimination to the expressions.
+            Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
 
-    exprs = description.split(",")
+    exprs = einx.expr.stage1.parse_args(description)
     if len(exprs) != len(tensors):
         raise ValueError(f"Expected {len(exprs)} tensors, got {len(tensors)}")
 
     tensor_shapes = [einx.param.get_shape(tensor) for tensor in tensors]
     einx.expr.solve(
-          [einx.expr.Equation(expr, tensor_shape) for expr, tensor_shape in zip(exprs, tensor_shapes)] \
-        + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+        [einx.expr.Equation(expr, tensor_shape) for expr, tensor_shape in zip(exprs, tensor_shapes)]
+        + [
+            einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+            for k, v in parameters.items()
+        ],
         cse=cse,
-    ) # Raises an exception if no solution is found
+    )  # Raises an exception if no solution is found
```

### Comparing `einx-0.1.3/einx/op/util.py` & `einx-0.2.0/einx/op/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,120 @@
-import einx, sys
+import einx
+import sys
 import numpy as np
 
+
 def flatten(exprs, tensors=None, backend=None):
     """Flatten the given expressions and optionally the corresponding tensors.
 
-    Flattening removes all compositions and concatenations and returns a list of new expressions (and optinally a list of flattened tensors).
+    Flattening removes all compositions and concatenations and returns a list of new expressions
+    (and optinally a list of flattened tensors).
 
     Parameters:
         exprs: Expressions to flatten.
-        tensors: Tensors corresponding to ``exprs``. If None, flattens and returns only ``exprs``. Defaults to None.
-        backend: Backend to use for tensor operations. If None, determines backend from ``tensors``. Defaults to None.
+        tensors: Tensors corresponding to ``exprs``. If None, flattens and returns only
+            ``exprs``. Defaults to None.
+        backend: Backend to use for tensor operations. If None, determines backend from
+            ``tensors``. Defaults to None.
 
     Returns:
         exprs: The flattened expressions.
         tensors, optional: The flattened tensors. Only returned if ``tensors`` is not None.
     """
     if tensors is None:
         exprs_out = []
         for expr in exprs:
             expr = einx.expr.stage3.decompose(expr)
             expr = einx.expr.stage3.remove_unnamed_trivial_axes(expr)
 
             if any(isinstance(e, einx.expr.stage3.Concatenation) for e in expr):
-                concat_index, concat_expr = [(i, e) for i, e in enumerate(expr) if isinstance(e, einx.expr.stage3.Concatenation)][0]
+                concat_index, concat_expr = [
+                    (i, e)
+                    for i, e in enumerate(expr)
+                    if isinstance(e, einx.expr.stage3.Concatenation)
+                ][0]
                 for i in range(len(concat_expr.children)):
                     # Extract subexpression
-                    subexpr = einx.expr.stage3.replace(expr, lambda expr:
-                        expr.children[i].__deepcopy__() if id(expr) == id(concat_expr) else None
+                    subexpr = einx.expr.stage3.replace(
+                        expr,
+                        lambda expr: expr.children[i].__deepcopy__()
+                        if id(expr) == id(concat_expr)
+                        else None,
                     )
 
                     exprs_out.extend(flatten([subexpr]))
             else:
                 exprs_out.append(expr)
 
         return exprs_out
     else:
+        assert backend is not None
         if len(exprs) != len(tensors):
             raise ValueError("Got different number of expressions and tensors")
-        if backend is None:
-            backend = einx.backend.get(tensors)
         exprs_out = []
         tensors_out = []
         for expr, tensor in zip(exprs, tensors):
             expr = einx.expr.stage3.decompose(expr)
             expr = einx.expr.stage3.remove_unnamed_trivial_axes(expr)
-            assert not tensor.shape is None
+            assert tensor.shape is not None
             if tensor.shape != expr.shape:
                 tensor = backend.reshape(tensor, expr.shape)
 
             if any(isinstance(e, einx.expr.stage3.Concatenation) for e in expr):
-                concat_index, concat_expr = [(i, e) for i, e in enumerate(expr) if isinstance(e, einx.expr.stage3.Concatenation)][0]
+                concat_index, concat_expr = [
+                    (i, e)
+                    for i, e in enumerate(expr)
+                    if isinstance(e, einx.expr.stage3.Concatenation)
+                ][0]
                 splits = np.cumsum([0] + [c.shape[0] for c in concat_expr.children])
 
                 for i in range(len(concat_expr.children)):
                     # Extract subtensor
                     s = (slice(None),) * concat_index + (slice(splits[i], splits[i + 1]),)
-                    subtensor = tensor[s] # TODO: split using np.split?
+                    subtensor = tensor[s]  # TODO: split using np.split?
 
                     # Extract subexpression
-                    subexpr = einx.expr.stage3.replace(expr, lambda expr:
-                        expr.children[i].__deepcopy__() if id(expr) == id(concat_expr) else None
+                    subexpr = einx.expr.stage3.replace(
+                        expr,
+                        lambda expr: expr.children[i].__deepcopy__()
+                        if id(expr) == id(concat_expr)
+                        else None,
                     )
 
-                    flattened_subexprs, flattened_subtensors = flatten([subexpr], [subtensor], backend)
+                    flattened_subexprs, flattened_subtensors = flatten(
+                        [subexpr], [subtensor], backend
+                    )
                     exprs_out.extend(flattened_subexprs)
                     tensors_out.extend(flattened_subtensors)
             else:
                 exprs_out.append(expr)
                 tensors_out.append(tensor)
 
         return exprs_out, tensors_out
 
+
 def assignment(exprs_in, exprs_out):
     """Solve the assignment problem between input and output expressions.
 
-    If multiple solutions exist: For each output expression in order, choose the first input expression that matches.
+    If multiple solutions exist: For each output expression in order,
+    choose the first input expression that matches.
 
     Args:
         exprs_in: Input expressions.
         exprs_out: Output expressions.
 
     Returns:
         indices: Indices into ``exprs_in`` with the same ordering as ``exprs_out``.
     """
     if len(exprs_in) != len(exprs_out):
         raise ValueError("Got different number of input and output expressions")
-    axes_in = [set([a.name for a in einx.expr.stage3.get_named_axes(expr_in)]) for expr_in in exprs_in]
-    axes_out = [set([a.name for a in einx.expr.stage3.get_named_axes(expr_out)]) for expr_out in exprs_out]
+    axes_in = [{a.name for a in einx.expr.stage3.get_named_axes(expr_in)} for expr_in in exprs_in]
+    axes_out = [
+        {a.name for a in einx.expr.stage3.get_named_axes(expr_out)} for expr_out in exprs_out
+    ]
 
     cost_matrix = np.ones((len(exprs_out), len(exprs_in)), dtype=int)
     for i, a_out in enumerate(axes_out):
         for j, a_in in enumerate(axes_in):
             cost_matrix[i, j] = 0 if a_in.issubset(a_out) else 1
 
     # Simple brute-force assignment problem solver
@@ -101,85 +125,106 @@
         # For an expr_out (r), find the first expr_in (c) that matches
         for c in range(cost_matrix.shape[1]):
             if cost_matrix[r, c] == 0:
                 cost_matrix2 = cost_matrix.copy()
                 cost_matrix2[r, :] = 1
                 cost_matrix2[:, c] = 1
                 rows, cols = assignment_solver(cost_matrix2, r + 1)
-                if not rows is None:
+                if rows is not None:
                     return [r] + rows, [c] + cols
         return None, None
 
     row_ind, col_ind = assignment_solver(cost_matrix)
     if row_ind is None:
-        raise RuntimeError("Failed to find assignment between input and output expressions") # TODO:
+        raise RuntimeError(
+            "Failed to find assignment between input and output expressions"
+        )  # TODO:
     assert np.all(row_ind == np.arange(len(exprs_out)))
 
     return col_ind
 
-def transpose_broadcast(expr_in, tensor, expr_out, broadcast=True, backend=None):
-    if backend is None:
-        backend = einx.backend.get([tensor])
-    assert einx.expr.stage3.is_flat(expr_in) and einx.expr.stage3.is_flat(expr_out), f"'{expr_in}' and '{expr_out}' must be flat"
+
+def transpose_broadcast(expr_in, tensor, expr_out, *, backend, broadcast=True):
+    assert einx.expr.stage3.is_flat(expr_in) and einx.expr.stage3.is_flat(
+        expr_out
+    ), f"'{expr_in}' and '{expr_out}' must be flat"
 
     # Transpose axes if necessary
     in_axes = [a.name for a in einx.expr.stage3.get_axes(expr_in)]
     out_axes = [a.name for a in einx.expr.stage3.get_axes(expr_out)]
     out_axes_intersect = [a for a in out_axes if a in in_axes]
     out_axes_broadcast = [a for a in out_axes if a not in in_axes]
     if set(out_axes_intersect) != set(in_axes):
-        raise RuntimeError("Found input axes that are not in output expression") # TODO:
+        raise RuntimeError("Found input axes that are not in output expression")  # TODO:
 
     perm = [in_axes.index(out_axis) for out_axis in out_axes_intersect]
     if perm != list(range(len(perm))):
         tensor = backend.transpose(tensor, tuple(perm))
 
     # Expand and broadcast missing output dimensions if necessary
     if len(out_axes_broadcast) > 0:
-        pre_broadcast_shape = tuple(1 if a.name in out_axes_broadcast else a.value for a in einx.expr.stage3.get_axes(expr_out))
-        assert not tensor.shape is None
+        pre_broadcast_shape = tuple(
+            1 if a.name in out_axes_broadcast else a.value
+            for a in einx.expr.stage3.get_axes(expr_out)
+        )
+        assert tensor.shape is not None
         if tensor.shape != pre_broadcast_shape:
             tensor = backend.reshape(tensor, pre_broadcast_shape)
         if broadcast and tensor.shape != expr_out.shape:
             tensor = backend.broadcast_to(tensor, expr_out.shape)
 
     if not broadcast:
-        expr_out = einx.expr.stage3.List([(axis if axis.name in in_axes else einx.expr.stage3.Axis(None, 1)) for axis in expr_out])
+        expr_out = einx.expr.stage3.List([
+            (axis if axis.name in in_axes else einx.expr.stage3.Axis(None, 1)) for axis in expr_out
+        ])
     return tensor, expr_out
 
+
 def _unflatten(exprs_in, tensors_in, expr_out, backend):
     expr_out_flat = einx.expr.stage3.decompose(expr_out)
     expr_out_flat = einx.expr.stage3.remove_unnamed_trivial_axes(expr_out_flat)
 
     if any(isinstance(e, einx.expr.stage3.Concatenation) for e in expr_out_flat):
-        concat_index, concat_expr = [(i, e) for i, e in enumerate(expr_out_flat) if isinstance(e, einx.expr.stage3.Concatenation)][0]
+        concat_index, concat_expr = [
+            (i, e)
+            for i, e in enumerate(expr_out_flat)
+            if isinstance(e, einx.expr.stage3.Concatenation)
+        ][0]
 
         tensors_out = []
         for i in range(len(concat_expr.children)):
-            # Extract subexpression
-            subexpr = einx.expr.stage3.replace(expr_out_flat, lambda expr:
-                expr.children[i].__deepcopy__() if id(expr) == id(concat_expr) else None
+            # Extract subexpression of i-th child in concatenation
+            subexpr = einx.expr.stage3.replace(
+                expr_out_flat,
+                lambda expr: expr.children[i].__deepcopy__()
+                if id(expr) == id(concat_expr)
+                else None,
             )
-            assert einx.expr.stage3.remove_unnamed_trivial_axes(einx.expr.stage3.decompose(subexpr)) == next(exprs_in)
 
             # Get subtensor
             subtensor = _unflatten(exprs_in, tensors_in, subexpr, backend)
 
             tensors_out.append(subtensor)
 
         tensor_out = backend.concatenate(tensors_out, axis=concat_index)
     else:
+        next_expr_in = next(exprs_in)
+        assert einx.expr.stage3.remove_unnamed_trivial_axes(
+            einx.expr.stage3.decompose(expr_out)
+        ) == einx.expr.stage3.remove_unnamed_trivial_axes(einx.expr.stage3.decompose(next_expr_in))
         tensor_out = next(tensors_in)
 
-    assert not tensor_out.shape is None
+    assert tensor_out.shape is not None
     if tensor_out.shape != expr_out.shape:
         tensor_out = backend.reshape(tensor_out, expr_out.shape)
+
     return tensor_out
 
-def unflatten(exprs_in, tensors_in, exprs_out, backend=None):
+
+def unflatten(exprs_in, tensors_in, exprs_out, *, backend):
     if len(exprs_in) != len(tensors_in):
         raise ValueError("Got different number of input expressions and tensors")
     if backend is None:
         backend = einx.backend.get(tensors_in)
 
     iter_exprs_in = iter(exprs_in)
     iter_tensors_in = iter(tensors_in)
@@ -187,20 +232,35 @@
     for expr_out in exprs_out:
         t = _unflatten(iter_exprs_in, iter_tensors_in, expr_out, backend)
         assert t.shape == expr_out.shape
         tensors_out.append(t)
 
     return tensors_out
 
+
+def _clean_parameter(k, v):
+    try:
+        v = np.asarray(v)
+    except Exception as e:
+        raise ValueError(f"Got invalid parameter {k}={v}") from e
+    if not np.issubdtype(v.dtype, np.integer):
+        raise ValueError(f"Got invalid parameter {k}={v}")
+    return v
+
+
 def _clean_description_and_parameters(description, parameters):
     # Remove parameters that are not used in the description
-    exprs = [einx.expr.stage1.parse(d) for d in description.split("->") for d in d.split(",")]
-    axis_names = {axis.name for root in exprs for axis in root.all() if isinstance(axis, einx.expr.stage1.NamedAxis)}
-    parameters = {k: v for k, v in parameters.items() if k in axis_names}
+    axis_names = {
+        axis.name
+        for axis in einx.expr.stage1.parse_op(description).all()
+        if isinstance(axis, einx.expr.stage1.NamedAxis)
+    }
+    parameters = {k: _clean_parameter(k, v) for k, v in parameters.items() if k in axis_names}
 
     return description, parameters
 
+
 def _op_to_str(op):
     if "__name__" in dir(op):
         return op.__name__
     else:
-        return str(op)
+        return str(op)
```

### Comparing `einx-0.1.3/einx/op/vmap.py` & `einx-0.2.0/einx/op/vmap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,59 @@
-import einx, inspect, functools
+import einx
+import inspect
+import functools
 from . import util
 import numpy as np
 from typing import Callable, Union, Mapping
 import numpy.typing as npt
 
-@einx.lru_cache(trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, **kwargs:
-    c(exprs_in, [t(x) for x in tensors_in], exprs_out, **kwargs))
-def vmap_stage3(exprs_in, tensors_in, exprs_out, *, flat=False, backend=None, op=None, kwargs={}, verbose=False):
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, **kwargs: c(
+        exprs_in, [t(x) for x in tensors_in], exprs_out, **kwargs
+    )
+)
+def vmap_stage3(
+    exprs_in,
+    tensors_in,
+    exprs_out,
+    *,
+    flat=False,
+    backend=None,
+    op=None,
+    kwargs=None,
+    verbose=False,
+):
+    if kwargs is None:
+        kwargs = {}
     if backend is None:
         backend = einx.backend.get(tensors_in)
     elif isinstance(backend, str):
         backend = einx.backend.get(backend)
     op = backend.op(op, tracable=False)
     if len(exprs_in) != len(tensors_in):
         raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensors_in)}")
     for root in list(exprs_in) + list(exprs_out):
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Concatenation):
                 raise ValueError("Concatenation not allowed")
 
     # Call tensor factories
-    tensors_in = [einx.param.instantiate(tensor, expr.shape, backend) for tensor, expr in zip(tensors_in, exprs_in)]
+    tensors_in = [
+        einx.param.instantiate(tensor, expr.shape, backend=backend)
+        for tensor, expr in zip(tensors_in, exprs_in)
+    ]
 
     if verbose:
         print("Expressions:")
         print("    IN:", [str(e) for e in exprs_in])
         print("    OUT:", [str(e) for e in exprs_out])
 
     # Flatten expressions
-    exprs_in_flat, tensors_in = util.flatten(exprs_in, tensors_in, backend)
+    exprs_in_flat, tensors_in = util.flatten(exprs_in, tensors_in, backend=backend)
     exprs_out_flat = util.flatten(exprs_out)
     assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_in_flat)
     assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_out_flat)
 
     if verbose:
         print("Flat expressions:")
         print("    IN:", [str(e) for e in exprs_in_flat])
@@ -49,238 +70,324 @@
         if not flat:
             print("    IN:", [str(e) for e in exprs_in_funcargs])
             print("    OUT:", [str(e) for e in exprs_out_funcargs])
         print("    IN_FLAT:", [str(e) for e in exprs_in_funcargs_flat])
         print("    OUT_FLAT:", [str(e) for e in exprs_out_funcargs_flat])
 
     def op(*tensors_in_flat, op=op):
-        assert not backend is None
-
         if verbose:
             print("Flat input tensors that arrived in op:", [str(a.shape) for a in tensors_in_flat])
             print("Input types to vmapped function:", [type(t) for t in tensors_in_flat])
         assert len(tensors_in_flat) == len(exprs_in_funcargs_flat)
 
         if not flat:
-            tensors_in = util.unflatten(exprs_in_funcargs_flat, tensors_in_flat, exprs_in_funcargs, backend=backend)
+            tensors_in = util.unflatten(
+                exprs_in_funcargs_flat, tensors_in_flat, exprs_in_funcargs, backend=backend
+            )
             if verbose:
                 print("Unflattened input tensors in op:", [str(a.shape) for a in tensors_in])
             assert len(tensors_in) == len(exprs_in)
         else:
             tensors_in = tensors_in_flat
         exprs_out_expected = exprs_out_funcargs if not flat else exprs_out_funcargs_flat
 
         output_shapes = [expr.shape for expr in exprs_out_expected]
         if len(output_shapes) == 1:
             output_shapes = output_shapes[0]
         tensors_out = backend.apply(op, args=tensors_in, kwargs=kwargs, output_shapes=output_shapes)
         if not isinstance(tensors_out, (tuple, list)):
             tensors_out = (tensors_out,)
         if len(tensors_out) != len(exprs_out_expected):
-            raise ValueError(f"Expected {len(exprs_out_expected)} output tensor(s) from vmapped function, but got {len(tensors_out)}")
+            raise ValueError(
+                f"Expected {len(exprs_out_expected)} output tensor(s) from vmapped "
+                f"function, but got {len(tensors_out)}"
+            )
 
         if verbose:
             print("Unflattened output tensors in op:")
-            for i, (expr_out, tensor_out) in enumerate(zip(exprs_out_expected, tensors_out)):
+            for expr_out, tensor_out in zip(exprs_out_expected, tensors_out):
                 print("    ", expr_out, tensor_out.shape)
 
         for i, (expr_out, tensor_out) in enumerate(zip(exprs_out_expected, tensors_out)):
-            assert tensor_out.shape == expr_out.shape, f"Expected output shape {expr_out.shape} from {i}-th (zero-based) output of vmapped function, but got {tensor_out.shape}"
+            if tensor_out.shape != expr_out.shape:
+                raise ValueError(
+                    f"Expected output shape {expr_out.shape} from {i}-th (zero-based) "
+                    f"output of vmapped function, but got {tensor_out.shape}"
+                )
 
         if not flat:
-            exprs_out_funcargs_flat2, tensors_out = util.flatten(exprs_out_funcargs, tensors_out, backend=backend)
+            exprs_out_funcargs_flat2, tensors_out = util.flatten(
+                exprs_out_funcargs, tensors_out, backend=backend
+            )
 
             if verbose:
                 print("Flattened output tensors in op:", [str(a.shape) for a in tensors_out])
-            assert exprs_out_funcargs_flat2 == exprs_out_funcargs_flat, f"{[str(s) for s in exprs_out_funcargs_flat2]} != {[str(s) for s in exprs_out_funcargs_flat]}"
+            assert (
+                exprs_out_funcargs_flat2 == exprs_out_funcargs_flat
+            ), f"{[str(s) for s in exprs_out_funcargs_flat2]} != "
+            f"{[str(s) for s in exprs_out_funcargs_flat]}"
 
         if verbose:
             print("Returning types from vmapped function:", [type(t) for t in tensors_out])
         return tuple(tensors_out)
 
     op = backend.op(op, tracable=True)
 
     axes_names_in = [[a.name for a in root] for root in exprs_in_flat]
-    axes_names_in_set = set(a.name for root in exprs_in_flat for a in root)
-    is_broadcast_axis = lambda expr: isinstance(expr, einx.expr.stage3.Axis) and not expr.name in axes_names_in_set and not einx.expr.stage3.is_marked(expr)
+    axes_names_in_set = {a.name for root in exprs_in_flat for a in root}
+
+    def is_broadcast_axis(expr):
+        return (
+            isinstance(expr, einx.expr.stage3.Axis)
+            and expr.name not in axes_names_in_set
+            and not einx.expr.stage3.is_marked(expr)
+        )
 
     # Get ordered list of vmapped axes
     def is_vmapped(expr):
         return not einx.expr.stage3.is_marked(expr)
+
     vmapped_axes = []
     for root in list(exprs_in_flat):
         for v in root:
-            if is_vmapped(v) and not v.name in vmapped_axes:
+            if is_vmapped(v) and v.name not in vmapped_axes:
                 vmapped_axes.append(v.name)
     if verbose:
         print(f"Vmapping the following axes: {vmapped_axes}")
     for root in list(exprs_in_flat) + list(exprs_out_flat):
         for v in root:
             if (v.name in vmapped_axes or is_broadcast_axis(v)) != is_vmapped(v):
                 raise ValueError(f"Axis {v.name} appears both as vmapped and non-vmapped")
 
     # Apply vmap to op
-    exprs_out_flat_without_broadcast = [einx.expr.stage3.remove(expr, is_broadcast_axis) for expr in exprs_out_flat]
-    axes_names_out_without_broadcast = [[a.name for a in root] for root in exprs_out_flat_without_broadcast]
-
-    axisname_to_value = {a.name: a.value for root in exprs_out_flat_without_broadcast for a in root}
+    exprs_out_flat_without_broadcast = [
+        einx.expr.stage3.remove(expr, is_broadcast_axis) for expr in exprs_out_flat
+    ]
+    axes_names_out_without_broadcast = [
+        [a.name for a in root] for root in exprs_out_flat_without_broadcast
+    ]
 
     if verbose:
-        print("Flat output expressions without broadcast:", [str(e) for e in exprs_out_flat_without_broadcast])
+        print(
+            "Flat output expressions without broadcast:",
+            [str(e) for e in exprs_out_flat_without_broadcast],
+        )
         print("Got input axis names:", axes_names_in)
-        print("Got output axis names (excluding broadcasted output axes):", axes_names_out_without_broadcast)
+        print(
+            "Got output axis names (excluding broadcasted output axes):",
+            axes_names_out_without_broadcast,
+        )
 
     vmaps = []
     input_shapes = tuple(expr.shape for expr in exprs_in_flat)
     output_shapes = tuple(expr.shape for expr in exprs_out_flat_without_broadcast)
     for v in reversed(vmapped_axes):
-        in_axes = tuple(axes_names.index(v) if v in axes_names else None for axes_names in axes_names_in)
-        out_axes = tuple(axes_names.index(v) if v in axes_names else None for axes_names in axes_names_out_without_broadcast)
+        in_axes = tuple(
+            axes_names.index(v) if v in axes_names else None for axes_names in axes_names_in
+        )
+        out_axes = tuple(
+            axes_names.index(v) if v in axes_names else None
+            for axes_names in axes_names_out_without_broadcast
+        )
         if verbose:
-            print(f"Applying backend.vmap to axis {v}, with input axis indices {in_axes} and output axis indices {out_axes}")
+            print(
+                f"Applying backend.vmap to axis {v}, with input axis indices "
+                f"{in_axes} and output axis indices {out_axes}"
+            )
         for out_axis, expr_out in zip(out_axes, exprs_out_flat):
             if out_axis is None:
-                raise ValueError(f"All vmapped axes must appear in the output expression, but '{v}' does not appear in '{expr_out}'")
+                raise ValueError(
+                    f"All vmapped axes must appear in the output expression, "
+                    f"but '{v}' does not appear in '{expr_out}'"
+                )
 
         vmaps.append((in_axes, out_axes, input_shapes, output_shapes))
+
         def drop_axis(shape, axis):
             if axis is None:
                 return shape
             else:
-                return shape[:axis] + shape[axis + 1:]
+                return shape[:axis] + shape[axis + 1 :]
+
         input_shapes = tuple(drop_axis(shape, axis) for shape, axis in zip(input_shapes, in_axes))
-        output_shapes = tuple(drop_axis(shape, axis) for shape, axis in zip(output_shapes, out_axes))
+        output_shapes = tuple(
+            drop_axis(shape, axis) for shape, axis in zip(output_shapes, out_axes)
+        )
 
         for axes_names in axes_names_in + axes_names_out_without_broadcast:
             if v in axes_names:
                 axes_names.remove(v)
             if v in axes_names_out_without_broadcast:
                 axes_names_out_without_broadcast.remove(v)
         if verbose:
-            print(f"Now has remaining input axes {axes_names_in} and output axes {axes_names_out_without_broadcast}")
+            print(
+                f"Now has remaining input axes {axes_names_in} and "
+                f"output axes {axes_names_out_without_broadcast}"
+            )
 
     for in_axes, out_axes, input_shapes, output_shapes in reversed(vmaps):
-        op = backend.vmap(op, in_axes=in_axes, out_axes=out_axes, input_shapes=input_shapes, output_shapes=output_shapes)
+        op = backend.vmap(
+            op,
+            in_axes=in_axes,
+            out_axes=out_axes,
+            input_shapes=input_shapes,
+            output_shapes=output_shapes,
+        )
 
     # Apply op to tensors
     if verbose:
         print("\nSending shapes to backend.vmap:", [str(a.shape) for a in tensors_in])
-    tensors = backend.apply(op, args=tensors_in, kwargs={}, output_shapes=tuple(expr.shape for expr in exprs_out_flat_without_broadcast))
+    tensors = backend.apply(
+        op,
+        args=tensors_in,
+        kwargs={},
+        output_shapes=tuple(expr.shape for expr in exprs_out_flat_without_broadcast),
+    )
     if verbose:
         for tensor, expr in zip(tensors, exprs_out_flat_without_broadcast):
             print("Got overall flat tensor_out:", tensor.shape, expr)
 
     # Transpose and broadcast missing output dimensions
-    tensors = [util.transpose_broadcast(expr_out_wb, tensor, expr_out)[0] for expr_out_wb, tensor, expr_out in zip(exprs_out_flat_without_broadcast, tensors, exprs_out_flat)]
+    tensors = [
+        util.transpose_broadcast(expr_out_wb, tensor, expr_out, backend=backend)[0]
+        for expr_out_wb, tensor, expr_out in zip(
+            exprs_out_flat_without_broadcast, tensors, exprs_out_flat
+        )
+    ]
     if verbose:
         print("Got overall transposed+broadcasted tensors_out:")
         for tensor, expr in zip(tensors, exprs_out_flat):
             print("    ", tensor.shape, expr)
 
     # Unflatten output expressions
-    tensors = util.unflatten(exprs_out_flat, tensors, exprs_out, backend)
+    tensors = util.unflatten(exprs_out_flat, tensors, exprs_out, backend=backend)
     if verbose:
         print("Got overall unflattened tensors_out:", [str(a.shape) for a in tensors])
 
     return tensors, exprs_out
 
+
 @einx.lru_cache
 def parse(description, *tensor_shapes, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
-
-    if "->" in description:
-        # Description: Inputs and output
-        description = description.split("->")
-        if len(description) != 2:
-            raise ValueError("Operation string must contain exactly one '->'")
-        exprs_in, exprs_out = description
-        exprs_in = exprs_in.split(",")
-        exprs_out = exprs_out.split(",")
-
-        if len(exprs_in) != len(tensor_shapes):
-            raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensor_shapes)}")
-
-    else:
-        # Description: "input -> output" using [|]-choice
-        expr = description
-        if "," in expr:
-            raise ValueError("Only a single expression is allowed when using the choice operator [|]")
-        if len(tensor_shapes) != 1:
-            raise ValueError(f"Expected 1 input tensor, got {len(tensor_shapes)}")
-
-        expr = einx.expr.stage1.parse(expr)
-        expr_in = str(einx.expr.stage1.choose(expr, 0, num=2))
-        expr_out = str(einx.expr.stage1.choose(expr, 1, num=2))
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
+
+    op = einx.expr.stage1.parse_op(description)
+
+    # Implicitly determine output expression
+    if len(op) == 1:
+        op = einx.expr.stage1.Op([
+            op[0],
+            op[0].__deepcopy__(),
+        ])
 
-        exprs_in = [expr_in]
-        exprs_out = [expr_out]
+    if len(op[0]) != len(tensor_shapes):
+        raise ValueError(f"Expected {len(op[0])} input tensors, but got {len(tensor_shapes)}")
 
     exprs = einx.expr.solve(
-          [einx.expr.Equation(expr_in, tensor_shape) for expr_in, tensor_shape in zip(exprs_in, tensor_shapes)] \
-        + [einx.expr.Equation(expr_out) for expr_out in exprs_out] \
-        + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+        [
+            einx.expr.Equation(expr_in, tensor_shape)
+            for expr_in, tensor_shape in zip(op[0], tensor_shapes)
+        ]
+        + [einx.expr.Equation(expr_out) for expr_out in op[1]]
+        + [
+            einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+            for k, v in parameters.items()
+        ],
         cse=cse,
         cse_concat=False,
-    )[:len(exprs_in) + len(exprs_out)]
-    exprs_in, exprs_out = exprs[:len(exprs_in)], exprs[len(exprs_in):]
+    )[: len(op[0]) + len(op[1])]
+    exprs_in, exprs_out = exprs[: len(op[0])], exprs[len(op[0]) :]
 
     return exprs_in, exprs_out
 
-@einx.lru_cache(trace=lambda t, c: lambda description, *tensors, **kwargs: c(description, *[t(x) for x in tensors], **kwargs))
-def vmap(description: str, *tensors: einx.Tensor, op: Callable, flat: bool = False, backend: Union[einx.Backend, str, None] = None, cse: bool = True, kwargs: Mapping = {}, **parameters: npt.ArrayLike):
-    """Applies a function to the marked axes of the input tensors using vectorization.
-
-    The function flattens all input tensors, applies the vectorized operation on the tensors and rearranges
-    the result to match the output expressions (see :doc:`How does einx handle input and output tensors? </faq/flatten>`).
 
-    The `description` argument specifies the input and output expressions. It must meet one of the following formats:
-
-    1. ``input1, input2, ... -> output1, output2, ...``
-        All input and output expressions are specified explicitly. The operation is applied over all axes marked with ``[]``-brackets.
-        All other axes are considered batch axes.
-
-    2. ``... [input1|output] ...``
-        The function accepts one input and one output tensor. The left and right choices correspond to the input and output tensor, respectively.
+@einx.traceback_util.filter
+@einx.lru_cache(
+    trace=lambda t, c: lambda description, *tensors, **kwargs: c(
+        description, *[t(x) for x in tensors], **kwargs
+    )
+)
+def vmap(
+    description: str,
+    *tensors: einx.Tensor,
+    op: Callable,
+    flat: bool = False,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    kwargs: Mapping = {},
+    **parameters: npt.ArrayLike,
+):
+    """Applies a function to the marked axes of the input tensors using vectorization.
 
-        Example: ``b [c1|c2]`` resolves to ``b [c1] -> b [c2]``
+    The function flattens all input tensors, applies the vectorized operation on the
+    tensors and rearranges the result to match the output expressions (see :doc:`How does
+    einx handle input and output tensors? </faq/flatten>`).
+
+    The `description` argument specifies the input and output expressions. The operation is
+    applied over all axes marked with ``[]``-brackets. All other axes are considered batch
+    axes and vectorized over.
 
-    The function ``op`` should accept input tensors and yield output tensors as specified in ``description`` with shapes matching the subexpressions that
-    are marked with ``[]``-brackets.
+    The function ``op`` should accept input tensors and yield output tensors as specified in
+    ``description`` with shapes matching the subexpressions that are marked with ``[]``-brackets.
 
     Args:
         description: Description string in Einstein notation (see above).
         tensors: Input tensors or tensor factories matching the description string.
-        op: Function that will be vectorized. If ``op`` is a string, retrieves the attribute of `backend` with the same name.
-        flat: Whether to pass the tensors to ``op`` in flattened form or matching the nested layout in the input expressions. Defaults to False.
+        op: Function that will be vectorized. If ``op`` is a string, retrieves the attribute
+            of `backend` with the same name.
+        flat: Whether to pass the tensors to ``op`` in flattened form or matching the nested
+            layout in the input expressions. Defaults to False.
         kwargs: Additional keyword arguments that are passed to ``op``. Defaults to ``{}``.
-        backend: Backend to use for all operations. If None, determines the backend from the input tensors. Defaults to None.
-        cse: Whether to apply common subexpression elimination to the expressions. Defaults to True.
-        graph: Whether to return the graph representation of the operation instead of computing the result. Defaults to False.
-        **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
+        backend: Backend to use for all operations. If None, determines the backend from the
+            input tensors. Defaults to None.
+        cse: Whether to apply common subexpression elimination to the expressions. Defaults
+            to True.
+        graph: Whether to return the graph representation of the operation instead of
+            computing the result. Defaults to False.
+        **parameters: Additional parameters that specify values for single axes,
+            e.g. ``a=4``.
 
     Returns:
-        The result of the vectorized operation if `graph=False`, otherwise the graph representation of the operation.
+        The result of the vectorized operation if `graph=False`, otherwise the graph
+        representation of the operation.
 
     Examples:
         Compute the mean along rows of a matrix:
 
         >>> x = np.random.uniform(size=(10, 8))
         >>> einx.vmap("a [b] -> a", x, op=np.mean)
         (10,)
 
         Vectorize a custom function:
 
-        >>> x, y = np.random.uniform(size=(10, 13, 4)), np.random.uniform(size=(4, 9,))
+        >>> x, y = (
+        ...     np.random.uniform(size=(10, 13, 4)),
+        ...     np.random.uniform(
+        ...         size=(
+        ...             4,
+        ...             9,
+        ...         )
+        ...     ),
+        ... )
         >>> def op(x, y): # c, d -> 2
         >>>     return np.stack([np.mean(x), np.max(y)])
         >>> einx.vmap("b1 [c] b2, b2 [d] -> b2 [2] b1", x, y, op=op).shape
         (4, 2, 10)
 
         Compute a matrix-matrix multiplication
 
-        >>> x, y = np.random.uniform(size=(5, 10)), np.random.uniform(size=(10, 3))
+        >>> x, y = (
+        ...     np.random.uniform(size=(5, 10)),
+        ...     np.random.uniform(size=(10, 3)),
+        ... )
         >>> einx.vmap("a [b], [b] c -> a c", x, y, op=np.dot).shape
         (5, 3)
     """
-    exprs_in, exprs_out = parse(description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters)
-    tensors, exprs_out = vmap_stage3(exprs_in, tensors, exprs_out, flat=flat, backend=backend, op=op, kwargs=kwargs)
+    exprs_in, exprs_out = parse(
+        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+    )
+    tensors, exprs_out = vmap_stage3(
+        exprs_in, tensors, exprs_out, flat=flat, backend=backend, op=op, kwargs=kwargs
+    )
     return tensors[0] if len(exprs_out) == 1 else tensors
```

### Comparing `einx-0.1.3/einx/op/vmap_with_axis.py` & `einx-0.2.0/einx/op/vmap_with_axis.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,220 +3,354 @@
 import numpy as np
 from functools import partial
 from typing import Callable, Mapping, Union, Tuple
 import numpy.typing as npt
 
 _op_names = ["roll", "flip"]
 
-@einx.lru_cache(trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, op, kwargs={}, backend=None: c(exprs_in, [t(x) for x in tensors_in], exprs_out, op, kwargs))
-def vmap_with_axis_stage3(exprs_in, tensors_in, exprs_out, op, kwargs={}, backend=None):
+
+@einx.lru_cache(
+    trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, op, kwargs={}, backend=None: c(
+        exprs_in, [t(x) for x in tensors_in], exprs_out, op, kwargs
+    )
+)
+def vmap_with_axis_stage3(exprs_in, tensors_in, exprs_out, op, kwargs=None, backend=None):
+    if kwargs is None:
+        kwargs = {}
     if backend is None:
         backend = einx.backend.get(tensors_in)
     elif isinstance(backend, str):
         backend = einx.backend.get(backend)
     op = backend.op(op, tracable=False)
     if len(exprs_in) != len(tensors_in):
         raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensors_in)}")
     if len(set(exprs_out)) != 1:
         raise ValueError("All output expressions must be the same")
     for root in list(exprs_in) + list(exprs_out):
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Concatenation):
                 raise ValueError("Concatenation not allowed")
+    if len(exprs_out) > 1:
+        raise ValueError("Only one output tensor allowed")
     kwargs = {**kwargs}
 
     # Call tensor factories
-    tensors_in = [einx.param.instantiate(tensor, expr.shape, backend) for tensor, expr in zip(tensors_in, exprs_in)]
+    tensors_in = [
+        einx.param.instantiate(tensor, expr.shape, backend=backend)
+        for tensor, expr in zip(tensors_in, exprs_in)
+    ]
 
     # Flatten expressions
-    exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend)
+    exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend=backend)
+    in_axis_names = {axis.name for expr in exprs_in for axis in expr}
+
+    def is_broadcast_axis(expr):
+        return isinstance(expr, einx.expr.stage3.Axis) and expr.name not in in_axis_names
+
     exprs_out_flat = util.flatten(exprs_out)
-    assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_in)
-    assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_out_flat)
+    exprs_out_flat_without_broadcast = [
+        einx.expr.stage3.remove(expr, is_broadcast_axis) for expr in exprs_out_flat
+    ]
 
-    transpose_first = len(exprs_in) > 1 # TODO: and inputs dont have matching expressions
-    if not transpose_first and len(exprs_in) > 1:
-        raise ValueError("When multiple input expressions are given, they have to be transposed to the same layout before applying the operation (transpose_first has to be set to True)")
+    transpose_first = len(exprs_in) > 1
 
     # Ensure that axis markings are consistent
     def is_vmapped(expr):
         return not einx.expr.stage3.is_marked(expr)
-    vmapped_axis_names = set(v.name for root in list(exprs_in) + list(exprs_out_flat) for v in root if is_vmapped(v))
-    for root in list(exprs_in) + list(exprs_out_flat):
+
+    vmapped_axis_names = {
+        v.name
+        for root in list(exprs_in) + list(exprs_out_flat_without_broadcast)
+        for v in root
+        if is_vmapped(v)
+    }
+    for root in list(exprs_in) + list(exprs_out_flat_without_broadcast):
         for v in root:
             if (v.name in vmapped_axis_names) != is_vmapped(v):
                 raise ValueError(f"Axis {v.name} appears both as vmapped and non-vmapped")
 
-    marked_input_axes = set(axis.name for expr_in in exprs_in for axis in expr_in.all() if isinstance(axis, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(axis))
-    marked_output_axes = set(axis.name for expr_out in exprs_out_flat for axis in expr_out.all() if isinstance(axis, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(axis))
+    marked_input_axes = {
+        axis.name
+        for expr_in in exprs_in
+        for axis in expr_in.all()
+        if isinstance(axis, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(axis)
+    }
+    marked_output_axes = {
+        axis.name
+        for expr_out in exprs_out_flat_without_broadcast
+        for axis in expr_out.all()
+        if isinstance(axis, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(axis)
+    }
+    if marked_output_axes.difference(marked_input_axes):
+        raise ValueError("Marked output axes must be a subset of marked input axes")
 
     if transpose_first:
         # Transpose and insert trivial axes
         if marked_input_axes != marked_output_axes:
-            raise ValueError("transpose_first can only be used when axes are unchanged")
-        x = [util.transpose_broadcast(expr_in, tensor_in, exprs_out_flat[0], broadcast=False) for expr_in, tensor_in in zip(exprs_in, tensors_in)]
+            raise ValueError(
+                "When using multiple input tensors the same axes must be marked in all tensors"
+            )
+        x = [
+            util.transpose_broadcast(
+                expr_in,
+                tensor_in,
+                exprs_out_flat_without_broadcast[0],
+                broadcast=False,
+                backend=backend,
+            )
+            for expr_in, tensor_in in zip(exprs_in, tensors_in)
+        ]
         tensors_in = [x[0] for x in x]
         exprs_in = [x[1] for x in x]
-        assert len(set(len(expr) for expr in exprs_in)) == 1
-        marked_input_axes = set(axis.name for expr_in in exprs_in for axis in expr_in.all() if isinstance(axis, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(axis))
+        assert len({len(expr) for expr in exprs_in}) == 1
+        marked_input_axes = {
+            axis.name
+            for expr_in in exprs_in
+            for axis in expr_in.all()
+            if isinstance(axis, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(axis)
+        }
+        exprs_op_output = exprs_out_flat_without_broadcast
+    else:
+        assert len(exprs_in) == 1  # TODO: see above
+        expr_in = exprs_in[0]
+
+        def to_op_output(expr_out_flat_wb):
+            axis_names = {
+                axis.name
+                for axis in expr_out_flat_wb.all()
+                if isinstance(axis, einx.expr.stage3.Axis)
+            }
+            new_axes = []
+            for axis in expr_in.all():
+                if isinstance(axis, einx.expr.stage3.Axis) and axis.name in axis_names:
+                    if isinstance(axis.parent, einx.expr.stage3.Marker):
+                        axis = axis.parent
+                    new_axes.append(axis)
+            return einx.expr.stage3.List.maybe(new_axes)
+
+        exprs_op_output = [
+            to_op_output(expr_out_flat_wb) for expr_out_flat_wb in exprs_out_flat_without_broadcast
+        ]
 
     # Add axis argument
     if transpose_first:
-        axis_indices = tuple(i for i, axis in enumerate(exprs_out_flat[0]) if axis.name in marked_input_axes)
+        axis_indices = tuple(
+            i
+            for i, axis in enumerate(exprs_out_flat_without_broadcast[0])
+            if axis.name in marked_input_axes
+        )
     else:
         axes_in = [list(expr) for expr in exprs_in]
-        axis_indices = tuple(i for i in range(len(axes_in[0])) if any(axes_in[i].name in marked_input_axes for axes_in in axes_in))
+        axis_indices = tuple(
+            i
+            for i in range(len(axes_in[0]))
+            if any(axes_in[i].name in marked_input_axes for axes_in in axes_in)
+        )
     if len(axis_indices) > 0:
         kwargs["axis"] = axis_indices if len(axis_indices) > 1 else axis_indices[0]
 
     # Apply operation
-    in_axis_names = set(axis.name for expr in exprs_in for axis in expr)
-    output_shape = np.asarray([(axis.value if axis.name in in_axis_names else 1) for axis in exprs_out_flat[0]])
-    output_shapes = (output_shape,) * len(exprs_out_flat) if len(exprs_out_flat) > 1 else output_shape
-    tensors_out = backend.apply(op, args=tensors_in, kwargs=kwargs, output_shapes=output_shapes)
+    tensors_out = backend.apply(
+        op,
+        args=tensors_in,
+        kwargs=kwargs,
+        output_shapes=[expr.shape for expr in exprs_op_output]
+        if len(exprs_op_output) > 1
+        else exprs_op_output[0].shape,
+    )
     if not isinstance(tensors_out, (tuple, list)):
         tensors_out = (tensors_out,)
-    if len(tensors_out) != len(exprs_out_flat):
-        raise ValueError(f"Expected {len(exprs_out_flat)} output tensor(s), got {len(tensors_out)}")
-
-    if not transpose_first:
-        # Transpose and broadcast missing output dimensions
-        def replace(expr):
-            if isinstance(expr, einx.expr.stage3.Marker):
-                if len(marked_output_axes) == 0:
-                    return []
-                else:
-                    return expr.__deepcopy__()
-        exprs_in = [einx.expr.stage3.replace(expr_in, replace) for expr_in in exprs_in]
-        tensors_out = [util.transpose_broadcast(exprs_in[0], tensor_out, expr_out)[0] for tensor_out, expr_out in zip(tensors_out, exprs_out_flat)]
-    else:
-        # Already transposed, only broadcast to flat output shape
-        def broadcast(tensor, expr):
-            if tensor.shape != expr.shape:
-                tensor = backend.broadcast_to(tensor, expr.shape)
-            return tensor
-        tensors_out = [broadcast(tensor, expr) for tensor, expr in zip(tensors_out, exprs_out_flat)]
+    if len(tensors_out) != len(exprs_out_flat_without_broadcast):
+        raise ValueError(
+            f"Expected {len(exprs_out_flat_without_broadcast)} output tensor(s), "
+            f"got {len(tensors_out)}"
+        )
+
+    # Transpose and broadcast missing output dimensions
+    tensors_out = [
+        util.transpose_broadcast(expr_in, tensor_out, expr_out, backend=backend)[0]
+        for expr_in, tensor_out, expr_out in zip(exprs_op_output, tensors_out, exprs_out_flat)
+    ]
 
     # Unflatten output expressions
-    tensors_out = util.unflatten(exprs_out_flat, tensors_out, exprs_out, backend)
+    tensors_out = util.unflatten(exprs_out_flat, tensors_out, exprs_out, backend=backend)
 
     return tensors_out, exprs_out
 
+
 @einx.lru_cache
 def parse(description, *tensor_shapes, cse=True, **parameters):
-    description, parameters = einx.op.util._clean_description_and_parameters(description, parameters)
-
-    if "->" in description:
-        # Description: Inputs and output
-        description = description.split("->")
-        if len(description) != 2:
-            raise ValueError("Operation string must contain exactly one '->'")
-        exprs_in, exprs_out = description
-        exprs_in = exprs_in.split(",")
-        exprs_out = exprs_out.split(",")
-
-        if len(exprs_in) != len(tensor_shapes):
-            raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensor_shapes)}")
-
-    else:
-        # Description: Single expression
-        expr = description
-        if "," in expr:
-            raise ValueError("Only a single expression is allowed when using the choice operator [|]")
-        if len(tensor_shapes) != 1:
-            raise ValueError(f"Expected 1 input tensor, got {len(tensor_shapes)}")
-
-        expr = einx.expr.stage1.parse(expr)
-        if any(isinstance(expr, einx.expr.stage1.Choice) for expr in expr.all()):
-            # "input -> output" using [|]-choice
-            expr_in = str(einx.expr.stage1.choose(expr, 0, num=2))
-            expr_out = str(einx.expr.stage1.choose(expr, 1, num=2))
-        else:
-            # Same input and output
-            expr_in = expr_out = str(expr)
+    description, parameters = einx.op.util._clean_description_and_parameters(
+        description, parameters
+    )
+
+    op = einx.expr.stage1.parse_op(description)
+
+    # Implicitly determine output expression
+    if len(op) == 1:
+        op = einx.expr.stage1.Op([
+            op[0],
+            op[0].__deepcopy__(),
+        ])
 
-        exprs_in = [expr_in]
-        exprs_out = [expr_out]
+    if len(op[0]) != len(tensor_shapes):
+        raise ValueError(f"Expected {len(op[0])} input tensors, but got {len(tensor_shapes)}")
 
     exprs = einx.expr.solve(
-          [einx.expr.Equation(expr_in, tensor_shape) for expr_in, tensor_shape in zip(exprs_in, tensor_shapes)] \
-        + [einx.expr.Equation(expr_out) for expr_out in exprs_out] \
-        + [einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None) for k, v in parameters.items()],
+        [
+            einx.expr.Equation(expr_in, tensor_shape)
+            for expr_in, tensor_shape in zip(op[0], tensor_shapes)
+        ]
+        + [einx.expr.Equation(expr_out) for expr_out in op[1]]
+        + [
+            einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
+            for k, v in parameters.items()
+        ],
         cse=cse,
         cse_concat=False,
-    )[:len(exprs_in) + len(exprs_out)]
-    exprs_in, exprs_out = exprs[:len(exprs_in)], exprs[len(exprs_in):]
+    )[: len(op[0]) + len(op[1])]
+    exprs_in, exprs_out = exprs[: len(op[0])], exprs[len(op[0]) :]
 
     return exprs_in, exprs_out
 
-@einx.lru_cache(trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(description, *[t(x) for x in tensors], **kwargs))
-def vmap_with_axis(description: str, *tensors: einx.Tensor, op: Callable, backend: Union[einx.Backend, str, None] = None, cse: bool = True, kwargs: Mapping = {}, **parameters: npt.ArrayLike):
-    """Applies a function to the marked axes of the input tensors by passing the ``axis`` argument.
 
-    The function flattens all input tensors, applies the given operation and rearranges
-    the result to match the output expressions (see :doc:`How does einx handle input and output tensors? </faq/flatten>`).
-
-    The `description` argument specifies the input and output expressions, as well as axes along which the operation is applied. It must meet one of the following formats:
-
-    1. ``input1, input2, ... -> output1, output2, ...``
-        All input and output expressions are specified explicitly. Axes that the operation is applied along are marked with ``[]``-brackets.
+@einx.traceback_util.filter
+@einx.lru_cache(
+    trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
+        description, *[t(x) for x in tensors], **kwargs
+    )
+)
+def vmap_with_axis(
+    description: str,
+    *tensors: einx.Tensor,
+    op: Callable,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    kwargs: Mapping = {},
+    **parameters: npt.ArrayLike,
+):
+    """Applies a function to the marked axes of the input tensors by passing the ``axis``
+    argument.
 
-    2. ``... [input|output] ...``
-        The left and right choices correspond to the input and output tensors, respectively. Axes that the operation is applied along are marked with ``[]``-brackets.
+    The function flattens all input tensors, applies the given operation and rearranges
+    the result to match the output expressions (see :doc:`How does einx handle input and output
+    tensors? </faq/flatten>`).
 
-        Example: ``a [b1|b2]`` resolves to ``a [b1] -> a [b2]``. ``a [b]`` resolves to ``a [b] -> a [b]``.
+    The `description` argument specifies the input and output expressions. The operation is
+    applied over all axes marked with ``[]``-brackets. All other axes are considered batch axes.
 
-    When the function is applied on scalars, the ``axis`` argument is not passed. For multiple input tensors, the function must follow
+    When the function is applied on scalars, the ``axis`` argument is not passed. For multiple
+    input tensors, the function must follow
     `Numpy broadcasting rules <https://numpy.org/doc/stable/user/basics.broadcasting.html>`_.
 
     Args:
         description: Description string in Einstein notation (see above).
         tensors: Input tensors or tensor factories matching the description string.
-        op: Backend operation. Is called with ``op(tensor, axis=...)``. If `op` is a string, retrieves the attribute of `backend` with the same name. 
+        op: Backend operation. Is called with ``op(tensor, axis=...)``. If `op` is a string,
+            retrieves the attribute of `backend` with the same name.
         kwargs: Additional keyword arguments that are passed to ``op``.
-        backend: Backend to use for all operations. If None, determines the backend from the input tensors. Defaults to None.
+        backend: Backend to use for all operations. If None, determines the backend from the input
+            tensors. Defaults to None.
         cse: Whether to apply common subexpression elimination to the expressions. Defaults to True.
-        graph: Whether to return the graph representation of the operation instead of computing the result. Defaults to False.
+        graph: Whether to return the graph representation of the operation instead of computing the
+            result. Defaults to False.
         **parameters: Additional parameters that specify values for single axes, e.g. ``a=4``.
 
     Returns:
-        The result of the operation if ``graph=False``, otherwise the graph representation of the operation.
+        The result of the operation if ``graph=False``, otherwise the graph
+        representation of the operation.
 
     Examples:
         Reverse order of elements along an axis:
 
         >>> x = np.random.uniform(size=(16, 20))
         >>> einx.vmap_with_axis("a [b] -> a [b]", x, op=np.flip).shape
         (16, 20)
 
         Roll elements along two axes:
 
         >>> x = np.random.uniform(size=(16, 20))
-        >>> einx.vmap_with_axis("a ([b c]) -> a ([b c])", x, op=partial(np.roll, shift=(2, 2)), b=2).shape
+        >>> einx.vmap_with_axis(
+        ...     "a ([b c]) -> a ([b c])",
+        ...     x,
+        ...     op=partial(np.roll, shift=(2, 2)),
+        ...     b=2,
+        ... ).shape
         (16, 20)
 
         Compute sum along axis:
 
         >>> x = np.random.uniform(size=(16, 20))
         >>> einx.vmap_with_axis("a ([b] c) -> c a", x, op=np.sum, b=2).shape
         (16, 20)
     """
-    exprs_in, exprs_out = parse(description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters)
-    tensors, exprs_out = vmap_with_axis_stage3(exprs_in, tensors, exprs_out, op=op, kwargs=kwargs, backend=backend)
+    exprs_in, exprs_out = parse(
+        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+    )
+    tensors, exprs_out = vmap_with_axis_stage3(
+        exprs_in, tensors, exprs_out, op=op, kwargs=kwargs, backend=backend
+    )
     return tensors[0] if len(exprs_out) == 1 else tensors
+
+
 vmap_with_axis.parse = parse
 
-def flip(description: str, tensor: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike):
+
+@einx.traceback_util.filter
+def flip(
+    description: str,
+    tensor: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+):
     """Specialization of :func:`einx.vmap_with_axis` with ``op="flip"``."""
     return vmap_with_axis(description, tensor, op="flip", backend=backend, cse=cse, **parameters)
 
-def roll(description: str, tensor: einx.Tensor, shift: Union[int, Tuple[int]], backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike):
-    """Specialization of :func:`einx.vmap_with_axis` with ``op="roll"`` and ``kwargs={"shift": shift}``."""
-    return vmap_with_axis(description, tensor, op="roll", backend=backend, kwargs={"shift": shift}, cse=cse, **parameters)
 
-def softmax(description: str, tensor: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike):
+@einx.traceback_util.filter
+def roll(
+    description: str,
+    tensor: einx.Tensor,
+    shift: Union[int, Tuple[int]],
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+):
+    """Specialization of :func:`einx.vmap_with_axis` with ``op="roll"`` and
+    ``kwargs={"shift": shift}``.
+    """
+    return vmap_with_axis(
+        description,
+        tensor,
+        op="roll",
+        backend=backend,
+        kwargs={"shift": shift},
+        cse=cse,
+        **parameters,
+    )
+
+
+@einx.traceback_util.filter
+def softmax(
+    description: str,
+    tensor: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+):
     """Specialization of :func:`einx.vmap_with_axis` with ``op="softmax"``"""
     return vmap_with_axis(description, tensor, op="softmax", backend=backend, cse=cse, **parameters)
 
-def log_softmax(description: str, tensor: einx.Tensor, backend: Union[einx.Backend, str, None] = None, cse: bool = True, **parameters: npt.ArrayLike):
+
+@einx.traceback_util.filter
+def log_softmax(
+    description: str,
+    tensor: einx.Tensor,
+    backend: Union[einx.Backend, str, None] = None,
+    cse: bool = True,
+    **parameters: npt.ArrayLike,
+):
     """Specialization of :func:`einx.vmap_with_axis` with ``op="log_softmax"``"""
-    return vmap_with_axis(description, tensor, op="log_softmax", backend=backend, cse=cse, **parameters)
+    return vmap_with_axis(
+        description, tensor, op="log_softmax", backend=backend, cse=cse, **parameters
+    )
```

### Comparing `einx-0.1.3/einx/param.py` & `einx-0.2.0/einx/param.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 import numpy as np
-import einx, sys, inspect, importlib
+import einx
+import sys
+import inspect
+import importlib
+
 
 def get_shape(x):
     if isinstance(x, (tuple, list)):
-        subshapes = set(get_shape(y) for y in x)
+        subshapes = {get_shape(y) for y in x}
         if len(subshapes) != 1:
-            raise ValueError(f"Failed to determine shape in input tensor")
+            raise ValueError("Failed to determine shape of input tensor")
         subshape = subshapes.pop()
         if subshape is None:
-            raise ValueError(f"Failed to determine shape in input tensor")
+            raise ValueError("Failed to determine shape of input tensor")
         return (len(x),) + subshape
     elif isinstance(x, (float, int, np.floating, np.integer)):
         # Scalar
         return ()
 
     try:
         # Concrete tensor
         return tuple(int(i) for i in x.shape)
     except:
         # Cannot determine shape (e.g. tensor factory)
         return None
 
+
 def instantiate(x, shape, backend, **kwargs):
     if x is None:
         raise TypeError("instantiate cannot be called on None")
     if backend == einx.backend.tracer:
         if x.shape is None:
-            return einx.backend.tracer.apply(instantiate, args=[x], kwargs={**{"shape": shape}, **kwargs}, output_shapes=shape)
+            return backend.apply(
+                instantiate, args=[x], kwargs={**{"shape": shape}, **kwargs}, output_shapes=shape
+            )
         else:
             return backend.to_tensor(x)
     else:
         if isinstance(x, (int, float, np.integer, np.floating)):
             return backend.to_tensor(x)
 
         for einn in einx.nn.get_frameworks():
             x2 = einn.to_tensor_factory(x)
-            if not x2 is None:
+            if x2 is not None:
                 x = x2
                 break
 
         if callable(x):
-            # Try to find keyword parameters of the tensor factory and forward all kwargs that are accepted. Pass no keyword parameters if this fails.
+            # Try to find keyword parameters of the tensor factory and forward all kwargs
+            # that are accepted. Pass no keyword parameters if this fails.
             try:
                 params = inspect.signature(x).parameters
                 if any(p.kind == inspect.Parameter.VAR_KEYWORD for p in params.values()):
                     pass
                 else:
                     kwargs = {k: v for k, v in kwargs.items() if k in params}
             except:
@@ -52,12 +60,14 @@
 
             x = x(shape, **kwargs)
             if x is None:
                 raise ValueError("Tensor factory returned None")
             if not hasattr(x, "shape"):
                 raise ValueError("Tensor factory returned an object without a shape attribute")
             if x.shape != shape:
-                raise ValueError(f"Tensor factory returned a tensor of shape {x.shape}, but expected {shape}")
+                raise ValueError(
+                    f"Tensor factory returned a tensor of shape {x.shape}, but expected {shape}"
+                )
         x = backend.to_tensor(x)
 
         assert x.shape == shape, f"Shape mismatch: {x.shape} != {shape} for {type(x)}"
-        return x
+        return x
```

### Comparing `einx-0.1.3/einx/tree_util.py` & `einx-0.2.0/einx/tree_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,67 @@
 # Avoid a hard jax dependency
 
+
 def tree_map_with_key(func, *trees, key=(), is_leaf=None):
-    if not is_leaf is None and is_leaf(key, *trees):
+    if is_leaf is not None and is_leaf(key, *trees):
         return func(*trees, key=key)
-    elif all(isinstance(tree, list) for tree in trees) and all(len(trees[0]) == len(tree) for tree in trees[1:]):
-        return [tree_map_with_key(func, *elements, key=key + (i,), is_leaf=is_leaf) for i, elements in enumerate(zip(*trees))]
-    elif all(isinstance(tree, tuple) for tree in trees) and all(len(trees[0]) == len(tree) for tree in trees[1:]):
-        return tuple(tree_map_with_key(func, *elements, key=key + (i,), is_leaf=is_leaf) for i, elements in enumerate(zip(*trees)))
-    elif all(isinstance(tree, dict) for tree in trees) and all(trees[0].keys() == tree.keys() for tree in trees[1:]):
-        return {k: tree_map_with_key(func, *[tree[k] for tree in trees], key=key + (k,), is_leaf=is_leaf) for k in trees[0]}
+    elif all(isinstance(tree, list) for tree in trees) and all(
+        len(trees[0]) == len(tree) for tree in trees[1:]
+    ):
+        return [
+            tree_map_with_key(func, *elements, key=key + (i,), is_leaf=is_leaf)
+            for i, elements in enumerate(zip(*trees))
+        ]
+    elif all(isinstance(tree, tuple) for tree in trees) and all(
+        len(trees[0]) == len(tree) for tree in trees[1:]
+    ):
+        return tuple(
+            tree_map_with_key(func, *elements, key=key + (i,), is_leaf=is_leaf)
+            for i, elements in enumerate(zip(*trees))
+        )
+    elif all(isinstance(tree, dict) for tree in trees) and all(
+        trees[0].keys() == tree.keys() for tree in trees[1:]
+    ):
+        return {
+            k: tree_map_with_key(
+                func, *[tree[k] for tree in trees], key=key + (k,), is_leaf=is_leaf
+            )
+            for k in trees[0]
+        }
     else:
         return func(*trees, key=key)
 
+
 def tree_map(func, *trees, is_leaf=None):
-    if not is_leaf is None and is_leaf(*trees):
+    if is_leaf is not None and is_leaf(*trees):
         return func(*trees)
-    elif all(isinstance(tree, list) for tree in trees) and all(len(trees[0]) == len(tree) for tree in trees[1:]):
-        return [tree_map(func, *elements, is_leaf=is_leaf) for i, elements in enumerate(zip(*trees))]
-    elif all(isinstance(tree, tuple) for tree in trees) and all(len(trees[0]) == len(tree) for tree in trees[1:]):
-        return tuple(tree_map(func, *elements, is_leaf=is_leaf) for i, elements in enumerate(zip(*trees)))
-    elif all(isinstance(tree, dict) for tree in trees) and all(trees[0].keys() == tree.keys() for tree in trees[1:]):
+    elif all(isinstance(tree, list) for tree in trees) and all(
+        len(trees[0]) == len(tree) for tree in trees[1:]
+    ):
+        return [
+            tree_map(func, *elements, is_leaf=is_leaf) for i, elements in enumerate(zip(*trees))
+        ]
+    elif all(isinstance(tree, tuple) for tree in trees) and all(
+        len(trees[0]) == len(tree) for tree in trees[1:]
+    ):
+        return tuple(
+            tree_map(func, *elements, is_leaf=is_leaf) for i, elements in enumerate(zip(*trees))
+        )
+    elif all(isinstance(tree, dict) for tree in trees) and all(
+        trees[0].keys() == tree.keys() for tree in trees[1:]
+    ):
         return {k: tree_map(func, *[tree[k] for tree in trees], is_leaf=is_leaf) for k in trees[0]}
     else:
         return func(*trees)
 
+
 def tree_flatten(x, is_leaf=None):
-    if not is_leaf is None and is_leaf(x):
+    if is_leaf is not None and is_leaf(x):
         yield x
     elif isinstance(x, (list, tuple)):
         for x in x:
             yield from tree_flatten(x, is_leaf=is_leaf)
     elif isinstance(x, dict):
         for x in x.items():
             yield from tree_flatten(x, is_leaf=is_leaf)
     else:
-        yield x
+        yield x
```

### Comparing `einx-0.1.3/einx.egg-info/PKG-INFO` & `einx-0.2.0/einx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einx
-Version: 0.1.3
+Version: 0.2.0
 Summary: Tensor Operations Expressed in Einstein-Inspired Notation
 Home-page: https://github.com/fferflo/einx
 Author: Florian Fervers
 Author-email: florian.fervers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
 [![PyPI version](https://badge.fury.io/py/einx.svg)](https://badge.fury.io/py/einx)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 einx is a Python library that allows formulating many tensor operations as concise expressions using Einstein notation. It is inspired by [einops](https://github.com/arogozhnikov/einops), but follows a novel and unique design:
 
 - Fully composable and powerful Einstein expressions with `[]`-notation.
 - Support for many tensor operations (`einx.{sum|max|where|add|dot|flip|get_at|...}`) with Numpy-like naming.
-- Easy integration and mixing with existing code. Supports tensor frameworks Numpy, PyTorch, Tensorflow and Jax.
+- Easy integration and mixing with existing code. Supports tensor frameworks Numpy, PyTorch, Tensorflow, Jax and others.
 - Just-in-time compilation of all operations into regular Python functions using Python's [`exec()`](https://docs.python.org/3/library/functions.html#exec).
 
 *Optional:*
 
 - Generalized neural network layers in Einstein notation. Supports PyTorch, Flax, Haiku, Equinox and Keras.
 
 **Getting started:**
@@ -51,30 +51,30 @@
 
 ## What does einx look like?
 
 #### Tensor manipulation
 
 ```python
 import einx
-x = {np.asarray|torch.as_tensor|jnp.asarray|tf.convert_to_tensor}(...) # Create some tensor
+x = {np.asarray|torch.as_tensor|jnp.asarray|...}(...) # Create some tensor
 
-einx.sum("a [b]", x)                              # Sum-reduction along columns
+einx.sum("a [b]", x)                              # Sum-reduction along second axis
 einx.flip("... (g [c])", x, c=2)                  # Flip pairs of values along the last axis
-einx.mean("b [s...] c", x)                        # Global mean-pooling
+einx.mean("b [s...] c", x)                        # Spatial mean-pooling
 einx.sum("b (s [s2])... c", x, s2=2)              # Sum-pooling with kernel_size=stride=2
-einx.add("b... [c]", x, b)                        # Add bias
+einx.add("a, b -> a b", x, y)                     # Outer sum
 
 einx.get_at("b [h w] c, b i [2] -> b i c", x, y)  # Gather values at coordinates
 
 einx.rearrange("b (q + k) -> b q, b k", x, q=2)   # Split
 einx.rearrange("b c, 1 -> b (c + 1)", x, [42])    # Append number to each channel
 
-einx.dot("... [c1|c2]", x, y)                     # Matmul = linear map from c1 to c2 channels
+einx.dot("... [c1->c2]", x, y)                    # Matmul = linear map from c1 to c2 channels
 
-# Vectorizing map
+                                                  # Apply custom operations:
 einx.vmap("b [s...] c -> b c", x, op=np.mean)     # Global mean-pooling
 einx.vmap("a [b], [b] c -> a c", x, y, op=np.dot) # Matmul
 ```
 
 All einx functions simply forward computation to the respective backend, e.g. by internally calling `np.reshape`, `np.transpose`, `np.sum` with the appropriate arguments.
 
 #### Common neural network operations
@@ -90,18 +90,18 @@
 
 # Multi-head attention
 attn = einx.dot("b q (h c), b k (h c) -> b q k h", q, k, h=8)
 attn = einx.softmax("b q [k] h", attn)
 x = einx.dot("b q k h, b k (h c) -> b q (h c)", attn, v)
 
 # Matmul in linear layers
-einx.dot("b...      [c1|c2]",  x, w)              # - Regular
-einx.dot("b...   (g [c1|c2])", x, w)              # - Grouped: Same weights per group
-einx.dot("b... ([g c1|g c2])", x, w)              # - Grouped: Different weights per group
-einx.dot("b  [s...|s2]  c",    x, w)              # - Spatial mixing as in MLP-mixer
+einx.dot("b...      [c1->c2]",  x, w)              # - Regular
+einx.dot("b...   (g [c1->c2])", x, w)              # - Grouped: Same weights per group
+einx.dot("b... ([g c1->g c2])", x, w)              # - Grouped: Different weights per group
+einx.dot("b  [s...->s2]  c",    x, w)              # - Spatial mixing as in MLP-mixer
 ```
 
 See [Common neural network ops](https://einx.readthedocs.io/en/latest/gettingstarted/commonnnops.html) for more examples.
 
 #### Deep learning modules
 
 ```python
@@ -109,18 +109,18 @@
 
 batchnorm       = einn.Norm("[b...] c", decay_rate=0.9)
 layernorm       = einn.Norm("b... [c]") # as used in transformers
 instancenorm    = einn.Norm("b [s...] c")
 groupnorm       = einn.Norm("b [s...] (g [c])", g=8)
 rmsnorm         = einn.Norm("b... [c]", mean=False, bias=False)
 
-channel_mix     = einn.Linear("b... [c1|c2]", c2=64)
-spatial_mix1    = einn.Linear("b [s...|s2] c", s2=64)
-spatial_mix2    = einn.Linear("b [s2|s...] c", s=(64, 64))
-patch_embed     = einn.Linear("b (s [s2|])... [c1|c2]", s2=4, c2=64)
+channel_mix     = einn.Linear("b... [c1->c2]", c2=64)
+spatial_mix1    = einn.Linear("b [s...->s2] c", s2=64)
+spatial_mix2    = einn.Linear("b [s2->s...] c", s=(64, 64))
+patch_embed     = einn.Linear("b (s [s2->])... [c1->c2]", s2=4, c2=64)
 
 dropout         = einn.Dropout("[...]",       drop_rate=0.2)
 spatial_dropout = einn.Dropout("[b] ... [c]", drop_rate=0.2)
 droppath        = einn.Dropout("[b] ...",     drop_rate=0.2)
 ```
 
 See `examples/train_{torch|flax|haiku|equinox|keras}.py` for example trainings on CIFAR10, [GPT-2](https://einx.readthedocs.io/en/latest/gettingstarted/gpt2.html) and [Mamba](https://github.com/fferflo/weightbridge/blob/master/examples/mamba2flax.py) for working example implementations of language models using einx, and [Tutorial: Neural networks](https://einx.readthedocs.io/en/latest/gettingstarted/neuralnetworks.html) for more details.
```

### Comparing `einx-0.1.3/einx.egg-info/SOURCES.txt` & `einx-0.2.0/einx.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 einx/__init__.py
 einx/lru_cache.py
 einx/param.py
+einx/traceback_util.py
 einx/tree_util.py
 einx/types.py
 einx.egg-info/PKG-INFO
 einx.egg-info/SOURCES.txt
 einx.egg-info/dependency_links.txt
 einx.egg-info/requires.txt
 einx.egg-info/top_level.txt
 einx/backend/__init__.py
+einx/backend/_dask.py
 einx/backend/_jax.py
+einx/backend/_mlx.py
 einx/backend/_numpy.py
 einx/backend/_tensorflow.py
 einx/backend/_torch.py
 einx/backend/base.py
 einx/backend/tracer.py
 einx/expr/__init__.py
 einx/expr/solver.py
```

### Comparing `einx-0.1.3/setup.py` & `einx-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="einx",
-    version="0.1.3",
+    version="0.2.0",
     python_requires=">=3.8",
     description="Tensor Operations Expressed in Einstein-Inspired Notation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Florian Fervers",
     author_email="florian.fervers@gmail.com",
     url="https://github.com/fferflo/einx",
```

### Comparing `einx-0.1.3/test/test_compare_einops.py` & `einx-0.2.0/test/test_compare_einops.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,63 @@
 import importlib
+
 if importlib.util.find_spec("einops"):
-    import einops, einx
+    import einops
+    import einx
     import numpy as np
 
     def assert_equal(a, b):
         assert a.shape == b.shape
         if a.dtype.kind in "f":
             assert np.allclose(a, b)
         else:
             assert np.all(a == b)
 
     def test_compare():
         x = np.random.uniform(size=(4, 128, 128, 3))
 
-        assert_equal(einx.mean("b [s...] c", x), einops.reduce(x, "b ... c -> b c", reduction="mean"))
-        assert_equal(einx.mean("b ... c -> b c", x), einops.reduce(x, "b ... c -> b c", reduction="mean"))
-
-        assert_equal(einx.mean("b [s...] c", x, keepdims=True), einops.reduce(x, "b h w c -> b 1 c", reduction="mean"))
-        assert_equal(einx.mean("b [s]... c", x, keepdims=True), einops.reduce(x, "b h w c -> b 1 1 c", reduction="mean"))
-        assert_equal(einx.mean("b h w c -> b 1 1 c", x), einops.reduce(x, "b h w c -> b 1 1 c", reduction="mean"))
-
-        assert_equal(einx.sum("b (s [s2])... c", x, s2=2), einops.reduce(x, "b (h h2) (w w2) c -> b h w c", reduction="sum", h2=2, w2=2))
-        assert_equal(einx.sum("b (h h2) (w w2) c -> b h w c", x, h2=2, w2=2), einops.reduce(x, "b (h h2) (w w2) c -> b h w c", reduction="sum", h2=2, w2=2))
+        assert_equal(
+            einx.mean("b [s...] c", x), einops.reduce(x, "b ... c -> b c", reduction="mean")
+        )
+        assert_equal(
+            einx.mean("b ... c -> b c", x), einops.reduce(x, "b ... c -> b c", reduction="mean")
+        )
+
+        assert_equal(
+            einx.mean("b [s...] c", x, keepdims=True),
+            einops.reduce(x, "b h w c -> b 1 c", reduction="mean"),
+        )
+        assert_equal(
+            einx.mean("b [s]... c", x, keepdims=True),
+            einops.reduce(x, "b h w c -> b 1 1 c", reduction="mean"),
+        )
+        assert_equal(
+            einx.mean("b h w c -> b 1 1 c", x),
+            einops.reduce(x, "b h w c -> b 1 1 c", reduction="mean"),
+        )
+
+        assert_equal(
+            einx.sum("b (s [s2])... c", x, s2=2),
+            einops.reduce(x, "b (h h2) (w w2) c -> b h w c", reduction="sum", h2=2, w2=2),
+        )
+        assert_equal(
+            einx.sum("b (h h2) (w w2) c -> b h w c", x, h2=2, w2=2),
+            einops.reduce(x, "b (h h2) (w w2) c -> b h w c", reduction="sum", h2=2, w2=2),
+        )
 
         w = np.random.uniform(size=(3, 32))
-        assert_equal(einx.dot("b... [c1|c2]", x, w), einops.einsum(x, w, "... c1, c1 c2 -> ... c2"))
-        assert_equal(einx.dot("... c1, c1 c2 -> ... c2", x, w), einops.einsum(x, w, "... c1, c1 c2 -> ... c2"))
+        assert_equal(
+            einx.dot("b... [c1->c2]", x, w), einops.einsum(x, w, "... c1, c1 c2 -> ... c2")
+        )
+        assert_equal(
+            einx.dot("... c1, c1 c2 -> ... c2", x, w),
+            einops.einsum(x, w, "... c1, c1 c2 -> ... c2"),
+        )
 
         w = np.random.uniform(size=(128, 128, 64))
-        assert_equal(einx.dot("b [s...|s2] c", x, w), einops.einsum(x, w, "b h w c, h w s2 -> b s2 c"))
-        assert_equal(einx.dot("b h w c, h w s2 -> b s2 c", x, w), einops.einsum(x, w, "b h w c, h w s2 -> b s2 c"))
+        assert_equal(
+            einx.dot("b [s...->s2] c", x, w), einops.einsum(x, w, "b h w c, h w s2 -> b s2 c")
+        )
+        assert_equal(
+            einx.dot("b h w c, h w s2 -> b s2 c", x, w),
+            einops.einsum(x, w, "b h w c, h w s2 -> b s2 c"),
+        )
```

### Comparing `einx-0.1.3/test/test_shapes.py` & `einx-0.2.0/test/test_shapes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,81 @@
 import importlib
+
 if importlib.util.find_spec("jax"):
     import jax
 if importlib.util.find_spec("torch"):
     import torch
 if importlib.util.find_spec("tensorflow"):
     import os
+
     os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = "true"
     import tensorflow
     import tensorflow.experimental.numpy as tnp
+
     tnp.experimental_enable_numpy_behavior()
+if importlib.util.find_spec("mlx"):
+    import mlx
+if importlib.util.find_spec("dask"):
+    import dask.array
 
-import einx, pytest
+import einx
+import pytest
 from functools import partial
 import numpy as np
 
 backends = [b for b in einx.backend.backends if b != einx.backend.tracer]
 
+
 @pytest.mark.parametrize("backend", backends)
 def test_shape_rearrange(backend):
     x = backend.zeros((10, 20, 1), "float32")
     assert einx.rearrange("a b c -> (a b) c 1", x).shape == (200, 1, 1)
     assert einx.rearrange("a b c -> (a b) c 1", x).shape == (200, 1, 1)
     assert einx.rearrange("a b c -> (a b) c 1 1 1", x).shape == (200, 1, 1, 1, 1)
     with pytest.raises(Exception):
         einx.rearrange("a a b c -> (a b) c 1", x)
         einx.rearrange("a (a + b) c -> (a b) c 1", x)
 
     x = backend.zeros((10, 20, 20, 2), "float32")
     assert einx.rearrange("b s... c -> b (s...) c", x).shape == (10, 400, 2)
     assert einx.rearrange("b ... c -> b (...) c", x).shape == (10, 400, 2)
-    assert einx.rearrange("b (s...) (r...) c -> b (s...) r... c", x, r=(10, 2)).shape == (10, 20, 10, 2, 2)
+    assert einx.rearrange("b (s...) (r...) c -> b (s...) r... c", x, r=(10, 2)).shape == (
+        10,
+        20,
+        10,
+        2,
+        2,
+    )
 
     assert einx.rearrange("1 -> (x)", backend.to_tensor([1]), x=10).shape == (10,)
     assert einx.rearrange("1 -> (x y)", backend.to_tensor([1]), x=10, y=20).shape == (200,)
 
     x = backend.zeros((10, 20, 1), "float32")
     assert einx.rearrange("a b c d... -> a b c (d...)", x).shape == (10, 20, 1, 1)
 
     x = backend.zeros((10, 20, 1, 2), "float32")
     assert einx.rearrange("a (b...) c d -> a (b... c) d", x).shape == (10, 20, 2)
 
     x = backend.zeros((10, 20, 1, 2, 3), "float32")
-    assert einx.rearrange("a (b... c) d... e -> a (b...) (c d...) e", x, b=[2, 5]).shape == (10, 10, 4, 3)
+    assert einx.rearrange("a (b... c) d... e -> a (b...) (c d...) e", x, b=[2, 5]).shape == (
+        10,
+        10,
+        4,
+        3,
+    )
 
     x = backend.zeros((10, 20, 6, 24), "float32")
-    assert einx.rearrange("a b (c...) (d...) -> a c... b d...", x, c=[2, 3], d=[4, 6]).shape == (10, 2, 3, 20, 4, 6)
+    assert einx.rearrange("a b (c...) (d...) -> a c... b d...", x, c=[2, 3], d=[4, 6]).shape == (
+        10,
+        2,
+        3,
+        20,
+        4,
+        6,
+    )
 
     x = backend.zeros((10, 10), "float32")
     assert einx.rearrange("a... -> 1 (a...)", x).shape == (1, 100)
 
     x = backend.zeros((10, 20, 5), "float32")
     assert einx.rearrange("(s1...) (s2...) h -> 1 h (s1...) (s2...)", x).shape == (1, 5, 10, 20)
 
@@ -62,20 +89,34 @@
 
     x = backend.zeros((10, 20, 1), "float32")
     with pytest.raises(Exception):
         einx.rearrange("a b... c... -> a (b...) c...", x)
     with pytest.raises(Exception):
         einx.rearrange("a b... -> a b", x)
 
-
     x = backend.zeros((1, 10, 20, 6), "float32")
-    assert einx.rearrange("a (b...) (e f...) (d c) -> a d (b...) (e f...) c", x, d=2).shape == (1, 2, 10, 20, 3)
+    assert einx.rearrange("a (b...) (e f...) (d c) -> a d (b...) (e f...) c", x, d=2).shape == (
+        1,
+        2,
+        10,
+        20,
+        3,
+    )
 
     x = backend.zeros((1, 10, 20, 6, 7, 12), "float32")
-    assert einx.rearrange("a b c d... (e f...) -> a b c d... ((e 2 2) f...)", x, f=[2, 2]).shape == (1, 10, 20, 6, 7, 12 * 2 * 2)
+    assert einx.rearrange(
+        "a b c d... (e f...) -> a b c d... ((e 2 2) f...)", x, f=[2, 2]
+    ).shape == (
+        1,
+        10,
+        20,
+        6,
+        7,
+        12 * 2 * 2,
+    )
 
     x = backend.zeros((10, 20, 3), "float32")
     assert einx.rearrange("(s s2)... c -> s... s2... c", x, s2=(2, 2)).shape == (5, 10, 2, 2, 3)
     assert einx.rearrange("(s s2)... c -> s... s2... c", x, s2=2).shape == (5, 10, 2, 2, 3)
 
     x = backend.zeros((10, 10, 10), "float32")
     assert einx.rearrange("(a b) (c d) (e f) -> a (b c d e) f", x, a=2, f=2).shape == (2, 250, 2)
@@ -107,16 +148,28 @@
     assert einx.arange("c1 c2 -> ([l] c2) c1", c1=4, c2=3, backend=backend).shape == (2 * 3, 4)
 
     x = backend.zeros((10, 20), "bool")
     y = backend.zeros((4, 10, 20, 3), "float32")
     x, y = einx.rearrange("h w, b h w c -> 1 h w 1, b h w c", x, y)
     assert backend.where(x, y, 0.0).shape == (4, 10, 20, 3)
 
+    x = np.zeros((5, 4))
+    x = einx.rearrange("(a + b + c) d -> b d, (a + c) d", x, a=1, b=2)
+    assert x[0].shape == (2, 4)
+    assert x[1].shape == (3, 4)
+    x = np.zeros((5, 4))
+    x = einx.rearrange("(a + b + c) d -> (a + c) d, b d", x, a=1, b=2)
+    assert x[0].shape == (3, 4)
+    assert x[1].shape == (2, 4)
+
+
 @pytest.mark.parametrize("backend", backends)
 def test_shape_dot(backend):
+    if backend.name == "mlx":
+        pytest.xfail(reason="mlx does not support einsum yet")
     x = backend.zeros((10, 10), "float32")
     assert einx.dot("a..., a... -> 1", x, x).shape == (1,)
     with pytest.raises(Exception):
         einx.dot("a..., [a]... -> 1", x, x)
 
     x = backend.zeros((10, 20, 1), "float32")
     y = backend.zeros((10, 24), "float32")
@@ -129,49 +182,63 @@
     with pytest.raises(Exception):
         einx.dot("a b c, a -> a b c", x)
 
     x = backend.zeros((10, 20), "float32")
     y = backend.zeros((20, 30), "float32")
     assert einx.dot("a [b] -> a [c]", x, y).shape == (10, 30)
     assert einx.dot("a b, b c -> a c", x, y).shape == (10, 30)
-    assert einx.dot("a [b|c]", x, y).shape == (10, 30)
-    assert einx.dot("a [b...|c]", x, y).shape == (10, 30)
+    assert einx.dot("a [b->c]", x, y).shape == (10, 30)
+    assert einx.dot("a [b...->c]", x, y).shape == (10, 30)
 
     x = backend.zeros((10, 20), "float32")
     y = backend.zeros((10, 20, 30), "float32")
     assert einx.dot("a b, a b c -> a c", x, y).shape == (10, 30)
     assert einx.dot("[a b] -> [a c]", x, y).shape == (10, 30)
-    assert einx.dot("[a b|a c]", x, y).shape == (10, 30)
+    assert einx.dot("[a b->a c]", x, y).shape == (10, 30)
 
     x = backend.zeros((10,), "float32")
     y = backend.zeros((30,), "float32")
     assert einx.dot("a, a ->", x, x).shape == ()
-    assert einx.dot("[a|]", x, x).shape == ()
+    assert einx.dot("[a->]", x, x).shape == ()
     assert einx.dot("a, c -> a c", x, y).shape == (10, 30)
-    assert einx.dot("a [|c]", x, y).shape == (10, 30)
-    assert einx.dot("a [b...|c]", x, y).shape == (10, 30)
+    assert einx.dot("a [->c]", x, y).shape == (10, 30)
+    assert einx.dot("a [b...->c]", x, y).shape == (10, 30)
 
     x = backend.zeros((4, 128, 128, 16), "float32")
-    assert einx.dot("b s... [c1|c2]", x, backend.zeros, c2=32).shape == (4, 128, 128, 32)
-    assert einx.dot("b [s...|s2] c", x, backend.zeros, s2=32).shape == (4, 32, 16)
+    assert einx.dot("b s... [c1->c2]", x, backend.zeros, c2=32).shape == (4, 128, 128, 32)
+    assert einx.dot("b [s...->s2] c", x, backend.zeros, s2=32).shape == (4, 32, 16)
 
     w = backend.zeros((2, 2, 16, 32), "float32")
-    assert einx.dot("b (s [s2|])... [c1|c2]", x, w, s2=2, c2=32).shape == (4, 64, 64, 32)
+    assert einx.dot("b (s [s2->])... [c1->c2]", x, w, s2=2, c2=32).shape == (4, 64, 64, 32)
 
     x = backend.zeros((4, 16, 16, 16), "float32")
-    w = lambda shape: backend.zeros(shape, "float32")
-    assert einx.dot("b [(s s2)|s]... [c1|c2]", x, w, s2=4, c2=4).shape == (4, 4, 4, 4)
-    assert einx.dot("b (s [s2|])... [c1|c2]", x, w, s2=4, c2=4).shape == (4, 4, 4, 4)
+
+    def w(shape):
+        return backend.zeros(shape, "float32")
+
+    assert einx.dot("b [(s s2)->s]... [c1->c2]", x, w, s2=4, c2=4).shape == (4, 4, 4, 4)
+    assert einx.dot("b (s [s2->])... [c1->c2]", x, w, s2=4, c2=4).shape == (4, 4, 4, 4)
 
     x = backend.ones((10, 10), "float32")
     y = backend.ones((10,), "float32")
-    assert einx.dot("[|]", 1, 1).shape == ()
-    assert einx.dot("a [|]", y, 1).shape == (10,)
-    assert einx.dot("a [b|]", x, y).shape == (10,)
-    assert einx.dot("a [|b]", y, y).shape == (10, 10)
+    assert einx.dot("[->]", 1, 1).shape == ()
+    assert einx.dot("a [->]", y, 1).shape == (10,)
+    assert einx.dot("a [b->]", x, y).shape == (10,)
+    assert einx.dot("a [->b]", y, y).shape == (10, 10)
+
+    x = backend.ones((11, 10), "float32")
+    y = backend.ones((11,), "float32")
+    assert einx.dot("... b, ... -> b", x, y).shape == (10,)
+    assert einx.dot("[...] b -> b", x, y).shape == (10,)
+
+    x = backend.ones((10,), "float32")
+    y = backend.ones((), "float32")
+    assert einx.dot("... b, ... -> b", x, y).shape == (10,)
+    assert einx.dot("[...] b -> b", x, y).shape == (10,)
+
 
 @pytest.mark.parametrize("backend", backends)
 def test_shape_reduce(backend):
     x = backend.zeros((10, 10), "float32")
     assert einx.reduce("a b -> 1 a", x, op=backend.mean).shape == (1, 10)
     assert einx.mean("a b -> 1 a", x).shape == (1, 10)
     assert einx.mean("[a] b", x).shape == (10,)
@@ -200,22 +267,30 @@
 
     x = backend.ones((16, 16, 32))
     bias = backend.ones((4,))
     assert einx.add("b... (g [c])", x, bias).shape == (16, 16, 32)
 
     assert einx.logsumexp("a [...]", x).shape == (16,)
 
-    assert einx.logsumexp("[a]", [0.0, 1.0]).shape == ()
-    assert einx.logsumexp("[a]", [np.asarray(0.0), np.asarray(1.0)]).shape == ()
-    assert einx.mean("[a]", [backend.to_tensor(0.0), np.asarray(1.0)]).shape == ()
-    assert einx.sum("[a]", [backend.to_tensor(0.0), backend.to_tensor(1.0)]).shape == ()
-    assert einx.logsumexp("[a] 1", [[0.0], [1.0]]).shape == (1,)
-    assert einx.logsumexp("[a]", [0.0] * 10).shape == ()
+    assert einx.logsumexp("[a]", [0.0, 1.0], backend=backend).shape == ()
+    assert (
+        einx.sum("[a]", [backend.to_tensor(0.0), backend.to_tensor(1.0)], backend=backend).shape
+        == ()
+    )
+    assert einx.logsumexp("[a] 1", [[0.0], [1.0]], backend=backend).shape == (1,)
+    assert einx.logsumexp("[a]", [0.0] * 10, backend=backend).shape == ()
     with pytest.raises(ValueError):
-        einx.logsumexp("a", [0.0, [1.0]])
+        einx.logsumexp("a", [0.0, [1.0]], backend=backend)
+
+    x = backend.ones((16, 15))
+    assert einx.sum("[b] a []", x).shape == (15,)
+    assert einx.sum("[b] a [...]", x).shape == (15,)
+
+    assert einx.sum("b [p] -> b p2", x, p2=7).shape == (16, 7)
+
 
 @pytest.mark.parametrize("backend", backends)
 def test_shape_elementwise(backend):
     x = backend.zeros((10, 5, 1), "float32")
     y = backend.zeros((13,), "float32")
     assert einx.elementwise("a b 1, l -> b l a 1", x, y, op=backend.add).shape == (5, 13, 10, 1)
     assert einx.add("a b 1, l -> b l a 1", x, y).shape == (5, 13, 10, 1)
@@ -236,171 +311,259 @@
         einx.add("a a, a -> a a", x, y)
     assert einx.add("a b, a b", x, backend.zeros).shape == (10, 10)
     assert einx.add("a, a", y, y).shape == (10,)
     assert einx.add("[a]", y, y).shape == (10,)
     assert einx.add("b, -> b 3", y, 1).shape == (10, 3)
 
     x = backend.zeros((2, 3), "float32")
-    y = backend.zeros((10,), "float32")
+    y = backend.ones((10,), "float32")
     with pytest.raises(Exception):
         einx.add("a b, c", x, y)
 
-    x = backend.zeros((16, 128, 196, 64), "float32")
-    y = backend.zeros((16, 4, 16), "float32")
-    assert einx.add("b h w (g c), b (g) c -> b h w (g c)", x, y).shape == (16, 128, 196, 64)
+    x = backend.zeros((3, 128, 196, 64), "float32")
+    y = backend.zeros((3, 4, 16), "float32")
+    assert einx.add("b h w (g c), b (g) c -> b h w (g c)", x, y).shape == (3, 128, 196, 64)
 
     x = backend.zeros((10, 20), "float32")
     y = backend.zeros((10, 20, 30), "float32")
     assert einx.add("a b, a b c -> a b c", x, y).shape == (10, 20, 30)
     assert einx.add("(a [1])...", x, backend.ones).shape == (10, 20)
 
     x = backend.zeros((10, 20), "float32")
     y = backend.zeros((30, 20), "float32")
     with pytest.raises(Exception):
         einx.subtract("ba c, i c -> i ba", x, y)
 
+
 @pytest.mark.parametrize("backend", backends)
 def test_shape_vmap(backend):
+    if backend.name in {"mlx", "dask"}:
+        pytest.xfail(reason="mlx does not fully support vmap with all primites yet")
+
     x = backend.zeros((13,), "float32")
     assert einx.vmap("b -> b [3]", x, op=lambda x: x + backend.zeros((3,))).shape == (13, 3)
 
     with pytest.raises(ValueError):
         einx.vmap("b -> [b] 3", x, op=lambda x: x + backend.zeros((3,)))
-    with pytest.raises(AssertionError):
+    with pytest.raises(Exception):
         einx.vmap("b -> b 3", x, op=lambda x: x + backend.ones((3,)))
 
     x = backend.zeros((4, 13, 2), "float32")
     y = backend.zeros((13, 4, 5, 5), "float32")
+
     def f(x, y):
         assert x.shape == (4, 2)
         assert y.shape == (4, 5)
         x = x[:, 0] + y[:, 0]
         return einx.rearrange("a -> a 15", x)
-    assert einx.vmap("[a] b [e], b [a] c [d] -> [a] b [g] c", x, y, op=f, g=15).shape == (4, 13, 15, 5)
-    assert einx.vmap("[a] b [e], b [a] c [d] -> [a] b ([g] c)", x, y, op=f, g=15).shape == (4, 13, 15 * 5)
+
+    assert einx.vmap("[a] b [e], b [a] c [d] -> [a] b [g] c", x, y, op=f, g=15).shape == (
+        4,
+        13,
+        15,
+        5,
+    )
+    assert einx.vmap("[a] b [e], b [a] c [d] -> [a] b ([g] c)", x, y, op=f, g=15).shape == (
+        4,
+        13,
+        15 * 5,
+    )
     with pytest.raises(Exception):
         einx.vmap("[a] b [e], b [a] c [d] -> [g] b [a] c", x, y, op=f, g=15)
-    
+
     with pytest.raises(Exception):
+
         def f(x, y):
             assert x.shape == (4, 2)
             assert y.shape == (4, 5)
             x = x[:, 0] + y[:, 0]
             return einx.rearrange("a -> a 16", x)
+
         einx.vmap("[a] b [e], b [a] c [d] -> [a] b [g] c", x, y, op=f, g=15)
 
     x = backend.zeros((4, 16), "float32")
     y = backend.zeros((16, 32), "float32")
-    assert einx.vmap("b [c1], [c1] c2 -> b c2", x, y, op=backend.dot).shape == (4, 32)
+    assert einx.vmap("b [c1], [c1] c2 -> b c2", x, y, op=lambda x, y: backend.sum(x * y)).shape == (
+        4,
+        32,
+    )
 
     x = backend.zeros((4,), "float32")
     y = backend.zeros((16, 32), "float32")
     assert einx.vmap("a, b c -> a b c", x, y, op=backend.add).shape == (4, 16, 32)
 
-    def func(x): # c -> 2
+    def func(x):  # c -> 2
         return backend.stack([backend.mean(x), backend.max(x)])
-    x = backend.zeros((16, 64, 3,), "float32")
+
+    x = backend.zeros(
+        (
+            16,
+            64,
+            3,
+        ),
+        "float32",
+    )
     assert einx.vmap("b [c] a -> a b [2]", x, op=func).shape == (3, 16, 2)
 
-    def func(x, y): # c, d -> 2
+    def func(x, y):  # c, d -> 2
         return backend.stack([backend.mean(x), backend.max(y)])
-    x = backend.zeros((16, 64), "float32") # b c
-    y = backend.zeros((16, 72), "float32") # b d
+
+    x = backend.zeros((16, 64), "float32")  # b c
+    y = backend.zeros((16, 72), "float32")  # b d
     assert einx.vmap("b [c], b [d] -> b [2]", x, y, op=func).shape == (16, 2)
 
-    x = backend.zeros((16, 64, 3), "float32") # b1 c b2
-    y = backend.zeros((3, 72), "float32") # b2 d
+    x = backend.zeros((16, 64, 3), "float32")  # b1 c b2
+    y = backend.zeros((3, 72), "float32")  # b2 d
     assert einx.vmap("b1 [c] b2, b2 [d] -> b2 [2] b1", x, y, op=func).shape == (3, 2, 16)
 
-    def func(x): # (c d) -> 2
+    def func(x):  # (c d) -> 2
         x = einx.vmap("([c] d) -> d", x, op=backend.mean, c=16)
         x = backend.max(x)
         return backend.stack([x, x])
-    x = backend.zeros((16, 64), "float32") # b c
+
+    x = backend.zeros((16, 64), "float32")  # b c
     assert einx.vmap("b ([c d]) -> b [2]", x, op=func, c=16).shape == (16, 2)
     assert einx.vmap("b ([c d]) -> b [2] 1", x, op=func, c=16).shape == (16, 2, 1)
-    assert einx.vmap("b [(c d)|2]", x, op=func, c=16).shape == (16, 2)
-    assert einx.vmap("b ([c d|2])", x, op=func, c=16).shape == (16, 2)
+    assert einx.vmap("b [(c d)->2]", x, op=func, c=16).shape == (16, 2)
+    assert einx.vmap("b ([c d->2])", x, op=func, c=16).shape == (16, 2)
     with pytest.raises(Exception):
         einx.vmap("b ([c d]) -> [2]", x, op=func, c=16)
 
-    def func(x): # c d -> 2
+    def func(x):  # c d -> 2
         x = einx.vmap("[c] d -> d", x, op=backend.mean, c=16)
         x = backend.max(x)
         return backend.stack([x, x])
-    x = backend.zeros((16, 64), "float32") # b c
+
+    x = backend.zeros((16, 64), "float32")  # b c
     assert einx.vmap("b ([c d]) -> b [2]", x, op=func, c=16, flat=True).shape == (16, 2)
     assert einx.vmap("b ([c d]) -> b [2] 1", x, op=func, c=16, flat=True).shape == (16, 2, 1)
-    assert einx.vmap("b [(c d)|2]", x, op=func, c=16, flat=True).shape == (16, 2)
-    assert einx.vmap("b ([c d|2])", x, op=func, c=16, flat=True).shape == (16, 2)
+    assert einx.vmap("b [(c d)->2]", x, op=func, c=16, flat=True).shape == (16, 2)
+    assert einx.vmap("b ([c d->2])", x, op=func, c=16, flat=True).shape == (16, 2)
     with pytest.raises(Exception):
         einx.vmap("b ([c d]) -> [2]", x, op=func, c=16, flat=True)
 
     with pytest.raises(Exception):
         einx.vmap_with_axis("a ([b c]) -> a ([b c])", x, op=partial(backend.roll, shift=(2, 2)))
-    assert einx.vmap_with_axis("a ([b c]) -> a ([b c])", x, op=partial(backend.roll, shift=(2, 2)), b=2).shape == (16, 64)
+    assert einx.vmap_with_axis(
+        "a ([b c]) -> a ([b c])", x, op=partial(backend.roll, shift=(2, 2)), b=2
+    ).shape == (
+        16,
+        64,
+    )
+
 
 @pytest.mark.parametrize("backend", backends)
 def test_shape_index(backend):
+    if backend.name in {"mlx", "dask"}:
+        pytest.xfail(reason="mlx does not fully support vmap with all primites yet")
+
     coord_dtype = "int32" if backend.name != "torch" else "long"
     x = backend.ones((4, 16, 16, 3))
     y = backend.cast(backend.ones((4, 128, 2)), coord_dtype)
     y2 = backend.cast(backend.ones((128, 4, 2)), coord_dtype)
     z = backend.ones((4, 128, 3))
     assert einx.get_at("b [h w] c, b p [2] -> b p c", x, y).shape == (4, 128, 3)
     assert einx.get_at("b [h w] c, p b [2] -> b p c", x, y2).shape == (4, 128, 3)
     assert einx.get_at("b [h w] c, b p, b p -> b p c", x, y[..., 0], y[..., 1]).shape == (4, 128, 3)
-    assert einx.get_at("b [h w] c, b (p [1]), b p -> b p c", x, y[..., 0], y[..., 1]).shape == (4, 128, 3)
-    assert einx.get_at("b [h w] c, b p, p b -> b p c", x, y[..., 0], y2[..., 1]).shape == (4, 128, 3)
-    assert einx.get_at("b [h w] c, p, p b -> b p c", x, y[0, ..., 0], y2[..., 1]).shape == (4, 128, 3)
-    assert einx.get_at("b [h w] c, b (p [1]), p b -> b p c", x, y[..., 0], y2[..., 1]).shape == (4, 128, 3)
-    assert einx.get_at("b [h w] c, b p [2] -> b p c", x, lambda shape: backend.ones(shape, coord_dtype), p=128).shape == (4, 128, 3)
-    assert einx.get_at("b [h w] c, b p [l] -> b p c", x, lambda shape: backend.ones(shape, coord_dtype), p=128).shape == (4, 128, 3)
+    assert einx.get_at("b [h w] c, b (p [1]), b p -> b p c", x, y[..., 0], y[..., 1]).shape == (
+        4,
+        128,
+        3,
+    )
+    assert einx.get_at("b [h w] c, b p, p b -> b p c", x, y[..., 0], y2[..., 1]).shape == (
+        4,
+        128,
+        3,
+    )
+    assert einx.get_at("b [h w] c, p, p b -> b p c", x, y[0, ..., 0], y2[..., 1]).shape == (
+        4,
+        128,
+        3,
+    )
+    assert einx.get_at("b [h w] c, b (p [1]), p b -> b p c", x, y[..., 0], y2[..., 1]).shape == (
+        4,
+        128,
+        3,
+    )
+    assert einx.get_at(
+        "b [h w] c, b p [2] -> b p c", x, lambda shape: backend.ones(shape, coord_dtype), p=128
+    ).shape == (4, 128, 3)
+    assert einx.get_at(
+        "b [h w] c, b p [l] -> b p c", x, lambda shape: backend.ones(shape, coord_dtype), p=128
+    ).shape == (4, 128, 3)
     assert einx.get_at("b [16 w] c, b p [2] -> b p c", x, y).shape == (4, 128, 3)
     assert einx.get_at("b [16 16] c, b p [2] -> b p c", x, y).shape == (4, 128, 3)
     assert einx.get_at("b [h w] c, p [2] -> b p c", x, y[0]).shape == (4, 128, 3)
     for op in [einx.set_at, einx.add_at, einx.subtract_at]:
         assert op("b [h w] c, b p [2], b p c -> b [h w] c", x, y, z).shape == (4, 16, 16, 3)
         assert op("b [h w] c, b p [2], b p c", x, y, z).shape == (4, 16, 16, 3)
-        assert op("b [h w] c, b p, b p, b p c -> b [h w] c", x, y[..., 0], y[..., 1], z).shape == (4, 16, 16, 3)
-        assert op("b [h w] c, b p, p b, b p c -> b [h w] c", x, y[..., 0], y2[..., 1], z).shape == (4, 16, 16, 3)
-        assert op("b [h w] c, b p, p b, p c -> b [h w] c", x, y[..., 0], y2[..., 1], z[0]).shape == (4, 16, 16, 3)
-        assert op("b [h w] c, b p, p b, c -> b [h w] c", x, y[..., 0], y2[..., 1], z[0, 0]).shape == (4, 16, 16, 3)
+        assert op("b [h w] c, b p, b p, b p c -> b [h w] c", x, y[..., 0], y[..., 1], z).shape == (
+            4,
+            16,
+            16,
+            3,
+        )
+        assert op("b [h w] c, b p, p b, b p c -> b [h w] c", x, y[..., 0], y2[..., 1], z).shape == (
+            4,
+            16,
+            16,
+            3,
+        )
+        assert op(
+            "b [h w] c, b p, p b, p c -> b [h w] c", x, y[..., 0], y2[..., 1], z[0]
+        ).shape == (4, 16, 16, 3)
+        assert op(
+            "b [h w] c, b p, p b, c -> b [h w] c", x, y[..., 0], y2[..., 1], z[0, 0]
+        ).shape == (4, 16, 16, 3)
         assert op("b [h w] c, p [2], p c -> b [h w] c", x, y[0], z[0]).shape == (4, 16, 16, 3)
         assert op("b [h w] c, b p [2], b p c -> b h w c", x, y, z).shape == (4, 16, 16, 3)
         assert op("b [h w] c, b p [2], p c -> b h w c", x, y, z[0]).shape == (4, 16, 16, 3)
         assert op("b [h w] c, p [2], b p c -> b h w c", x, y[0], z).shape == (4, 16, 16, 3)
         assert op("b [h w] c, p [2], p c -> b h w c", x, y[0], z[0]).shape == (4, 16, 16, 3)
 
     x = backend.ones((16, 4, 3, 16))
     y = backend.cast(backend.ones((2, 4, 128)), coord_dtype)
     z = backend.ones((3, 4, 128))
     assert einx.get_at("[w] b c [h], [2] b p -> b p c", x, y).shape == (4, 128, 3)
     assert einx.get_at("[w] b c [h], [2] p -> b p c", x, y[:, 0]).shape == (4, 128, 3)
     for op in [einx.set_at, einx.add_at, einx.subtract_at]:
         assert op("[w] b c [h], [2] b p, c b p -> b [w h] c", x, y, z).shape == (4, 16, 16, 3)
-        assert op("[w] b c [h], [2] p, c p -> b [w h] c", x, y[:, 0], z[:, 0]).shape == (4, 16, 16, 3)
+        assert op("[w] b c [h], [2] p, c p -> b [w h] c", x, y[:, 0], z[:, 0]).shape == (
+            4,
+            16,
+            16,
+            3,
+        )
 
     x = backend.ones((16, 4, 3 * 16))
     y = backend.cast(backend.ones((2, 4, 128)), coord_dtype)
     z = backend.ones((3, 4, 128))
     assert einx.get_at("[w] b (c [h]), [2] b p -> b p c", x, y, c=3).shape == (4, 128, 3)
     assert einx.get_at("[w] b (c [h]), [2] p -> b p c", x, y[:, 0], c=3).shape == (4, 128, 3)
     for op in [einx.set_at, einx.add_at, einx.subtract_at]:
         assert op("[w] b (c [h]), [2] b p, c b p -> b ([w h]) c", x, y, z).shape == (4, 256, 3)
-        assert op("[w] b (c [h]), [2] p, c p -> b ([w h]) c", x, y[:, 0], z[:, 0]).shape == (4, 256, 3)
+        assert op("[w] b (c [h]), [2] p, c p -> b ([w h]) c", x, y[:, 0], z[:, 0]).shape == (
+            4,
+            256,
+            3,
+        )
 
     x = backend.ones((4, 16, 16, 3))
     y = backend.cast(backend.ones((4, 3, 4, 5, 2)), coord_dtype)
     z = backend.ones((4, 3, 4, 5, 3))
     assert einx.get_at("b [h w] c, b p q r [2] -> b p q r c", x, y).shape == (4, 3, 4, 5, 3)
     assert einx.get_at("b [h w] c, p q r [2] -> b p q r c", x, y[0]).shape == (4, 3, 4, 5, 3)
     for op in [einx.set_at, einx.add_at, einx.subtract_at]:
         assert op("b [h w] c, b p q r [2], b p q r c -> b [h w] c", x, y, z).shape == (4, 16, 16, 3)
-        assert op("b [h w] c, p q r [2], p q r c -> b [h w] c", x, y[0], z[0]).shape == (4, 16, 16, 3)
+        assert op("b [h w] c, p q r [2], p q r c -> b [h w] c", x, y[0], z[0]).shape == (
+            4,
+            16,
+            16,
+            3,
+        )
 
     x = backend.ones((4, 1, 1, 3))
     y = backend.cast(backend.zeros((4, 128, 2)), coord_dtype)
     z = backend.ones((4, 128, 3))
     with pytest.raises(Exception):
         einx.get_at("b ([1 1]) c, b p [2] -> b p c", x, y)
 
@@ -408,55 +571,134 @@
     y = backend.cast(backend.zeros((4, 5)), coord_dtype)
     assert einx.get_at("b t [d], b t -> b t", x, y).shape == (4, 5)
     assert einx.get_at("... [d], ... -> ...", x, y).shape == (4, 5)
     assert einx.get_at("b t [d], b (t [1]) -> b (t 1)", x, y).shape == (4, 5)
     with pytest.raises(ValueError):
         einx.get_at("b t [d], b (t [1]) -> b (t [1])", x, y)
 
+    x = backend.ones((4, 128, 128, 3))
+    y = backend.cast(backend.zeros((4, 0, 2)), coord_dtype)
+    y2 = backend.cast(backend.zeros((4, 2)), coord_dtype)
+    z = backend.ones((4, 0, 3))
+    z2 = backend.ones((4, 3))
+    assert einx.set_at("b [h w] c, b p [2], b p c -> b [h w] c", x, y, z).shape == (4, 128, 128, 3)
+    assert einx.set_at("b [h w] c, b p [2], b c -> b [h w] c", x, y, z2).shape == (4, 128, 128, 3)
+    assert einx.set_at("b [h w] c, b [2], b p c -> b [h w] c", x, y, z2).shape == (4, 128, 128, 3)
+
+    x = backend.ones((4, 128, 16))
+    y = backend.cast(backend.zeros((4, 128)), coord_dtype)
+    z = backend.ones((4, 128))
+    assert einx.get_at("b p [i,->]", x, y).shape == (4, 128)
+    assert einx.set_at("b p [i,,->i]", x, y, z).shape == (4, 128, 16)
+
     consts = {"b": 4, "h": 16, "w": 16, "c": 3, "p": 128}
-    make_coords = lambda shape: backend.cast(backend.zeros(shape), coord_dtype)
+
+    def make_coords(shape):
+        return backend.cast(backend.zeros(shape), coord_dtype)
+
     xs = ["([h] b) [w] c", "[h] c [w]", "[h w]"]
     ys = ["b (p [2])", "[2] p", "[2]"]
     ys2 = ["p b", "p", "[1]"]
     zs = ["b p c", "c (p b)"]
     for x in xs:
         for z in zs:
-            shape = einx.add(f"{z}, ", backend.zeros, 0, **consts).shape
+            shape = einx.add(f"{z}, ", backend.zeros, 0, **consts, backend=backend).shape
             for y in ys:
-                assert einx.get_at(f"{x}, {y} -> {z}", backend.zeros, make_coords, **consts, backend=backend).shape == shape
+                assert (
+                    einx.get_at(
+                        f"{x}, {y} -> {z}", backend.zeros, make_coords, **consts, backend=backend
+                    ).shape
+                    == shape
+                )
             for y1 in ys2:
                 for y2 in ys2:
-                    assert einx.get_at(f"{x}, {y1}, {y2} -> {z}", backend.zeros, make_coords, make_coords, **consts, backend=backend).shape == shape
+                    assert (
+                        einx.get_at(
+                            f"{x}, {y1}, {y2} -> {z}",
+                            backend.zeros,
+                            make_coords,
+                            make_coords,
+                            **consts,
+                            backend=backend,
+                        ).shape
+                        == shape
+                    )
 
     for x in xs:
-        shape = einx.add(f"{x.replace('[', '').replace(']', '')}, ", backend.zeros, 0, **consts).shape
+        shape = einx.add(
+            f"{x.replace('[', '').replace(']', '')}, ", backend.zeros, 0, **consts, backend=backend
+        ).shape
         for z in zs:
-            z_axes = set(a for a in z if a.isalpha())
+            z_axes = {a for a in z if a.isalpha()}
             for y in ys:
                 if all(a in (x + y) for a in z_axes):
-                    assert einx.set_at(f"{x}, {y}, {z} -> {x}", backend.ones, make_coords, backend.zeros, **consts, backend=backend).shape == shape
+                    assert (
+                        einx.set_at(
+                            f"{x}, {y}, {z} -> {x}",
+                            backend.ones,
+                            make_coords,
+                            backend.zeros,
+                            **consts,
+                            backend=backend,
+                        ).shape
+                        == shape
+                    )
             for y1 in ys2:
                 for y2 in ys2:
                     if all(a in (x + y1 + y2) for a in z_axes):
-                        assert einx.set_at(f"{x}, {y1}, {y2}, {z} -> {x}", backend.ones, make_coords, make_coords, backend.zeros, **consts, backend=backend).shape == shape
-                        assert einx.set_at(f"{x}, {y1}, {y2}, {z}", backend.ones, make_coords, make_coords, backend.zeros, **consts, backend=backend).shape == shape
+                        assert (
+                            einx.set_at(
+                                f"{x}, {y1}, {y2}, {z} -> {x}",
+                                backend.ones,
+                                make_coords,
+                                make_coords,
+                                backend.zeros,
+                                **consts,
+                                backend=backend,
+                            ).shape
+                            == shape
+                        )
+                        assert (
+                            einx.set_at(
+                                f"{x}, {y1}, {y2}, {z}",
+                                backend.ones,
+                                make_coords,
+                                make_coords,
+                                backend.zeros,
+                                **consts,
+                                backend=backend,
+                            ).shape
+                            == shape
+                        )
+
 
 @pytest.mark.parametrize("backend", backends)
 def test_shape_vmap_with_axis(backend):
     x = backend.ones((10, 10), "float32")
     assert einx.flip("a [b] -> a [b]", x).shape == (10, 10)
     assert einx.flip("a [b]", x).shape == (10, 10)
     assert einx.roll("a [b]", x, shift=5).shape == (10, 10)
     assert einx.roll("a [b]", x, shift=(5,)).shape == (10, 10)
     assert einx.softmax("a [b] -> a [b]", x).shape == (10, 10)
     assert einx.softmax("a [b]", x).shape == (10, 10)
+    assert einx.softmax("a [b] -> (a [b]) c", x, c=3).shape == (100, 3)
+    assert einx.softmax("a [b] -> a ([b] c)", x, c=3).shape == (10, 30)
     assert einx.log_softmax("(a [b]) c", x, b=2).shape == (10, 10)
 
     assert einx.flip("a ([b c])", x, b=2).shape == (10, 10)
-    assert einx.roll("a ([b c])", x, shift=(5, 5,), b=2).shape == (10, 10)
+    assert einx.roll(
+        "a ([b c])",
+        x,
+        shift=(
+            5,
+            5,
+        ),
+        b=2,
+    ).shape == (10, 10)
+
 
 @pytest.mark.parametrize("backend", backends)
 def test_shape_solve(backend):
     x = backend.ones((2, 3, 4))
     assert einx.matches("a b c", x)
     assert not einx.matches("a b", x)
     with pytest.raises(Exception):
@@ -468,8 +710,11 @@
 
     x = backend.ones((2, 3, 4))
     assert einx.matches("a b...", x)
 
     x = backend.ones((5, 4))
     assert einx.matches("(a + b) c", x)
     assert einx.matches("(a + b) c", x, a=2)
-    assert not einx.matches("(a + b) c", x, a=10)
+    assert not einx.matches("(a + b) c", x, a=10)
+
+    params = einx.solve("a b, c b", x, x)
+    assert params["a"] == 5 and params["b"] == 4 and params["c"] == 5
```

### Comparing `einx-0.1.3/test/test_values.py` & `einx-0.2.0/test/test_values.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,104 @@
 import importlib
+
 if importlib.util.find_spec("jax"):
     import jax
 if importlib.util.find_spec("torch"):
     import torch
 if importlib.util.find_spec("tensorflow"):
     import os
+
     os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = "true"
     import tensorflow
     import tensorflow.experimental.numpy as tnp
+
     tnp.experimental_enable_numpy_behavior()
+if importlib.util.find_spec("mlx"):
+    import mlx
+if importlib.util.find_spec("dask"):
+    import dask.array
 
-import einx, pytest
+import einx
+import pytest
 import numpy as np
 
 backends = [b for b in einx.backend.backends if b != einx.backend.tracer]
 
+
 @pytest.mark.parametrize("backend", backends)
 def test_values(backend):
     rng = np.random.default_rng(42)
 
-    x = backend.to_tensor(rng.uniform(size=(13,)).astype("float32"))
-    assert backend.allclose(
-        einx.vmap("b -> b [3]", x, op=lambda x: x + backend.ones((3,))),
-        einx.add("b, -> b 3", x, 1),
-    )
+    if backend.name != "mlx":
+        x = backend.to_tensor(rng.uniform(size=(13,)).astype("float32"))
+        assert backend.allclose(
+            einx.vmap("b -> b [3]", x, op=lambda x: x + backend.ones((3,))),
+            einx.add("b, -> b 3", x, 1),
+        )
 
     x = backend.to_tensor(rng.uniform(size=(10, 20, 3)).astype("float32"))
     y = backend.to_tensor(rng.uniform(size=(10, 24)).astype("float32"))
-    assert backend.allclose(
-        einx.dot("a b c, a d -> a b c d", x, y),
-        einx.vmap("a [b c], a [d] -> a [b c d]", x, y, op=lambda x, y: einx.dot("b c, d -> b c d", x, y)),
-    )
+    if backend.name != "mlx":
+        assert backend.allclose(
+            einx.dot("a b c, a d -> a b c d", x, y),
+            einx.vmap(
+                "a [b c], a [d] -> a [b c d]",
+                x,
+                y,
+                op=lambda x, y: einx.dot("b c, d -> b c d", x, y),
+            ),
+        )
 
     assert backend.allclose(
         einx.multiply("a b c, a b c, a b c", x, x, x),
         x * x * x,
     )
 
-    assert backend.allclose(
-        einx.mean("a b [c]", x),
-        einx.vmap("a b [c] -> a b", x, op=backend.mean),
-    )
-
-    assert einx.dot("[|]", 1, 1) == 1
-
-    x = backend.ones((10, 10), "float32")
-    y = backend.ones((10,), "float32")
-    assert backend.allclose(
-        einx.dot("a [|]", y, 1),
-        y,
-    )
-    assert backend.allclose(
-        einx.dot("a [b|]", x, y),
-        y * 10,
-    )
-    assert backend.allclose(
-        einx.dot("a [|b]", y, y),
-        x,
-    )
-    assert backend.allclose(
-        einx.dot("a [b|b]", x, y),
-        einx.multiply("a b, b -> a b", x, y),
-    )
+    if backend.name != "mlx":
+        assert backend.allclose(
+            einx.mean("a b [c]", x),
+            einx.vmap("a b [c] -> a b", x, op=backend.mean),
+        )
+
+        assert einx.dot("[->]", 1, 1) == 1
+
+        x = backend.ones((10, 10), "float32")
+        y = backend.ones((10,), "float32")
+        assert backend.allclose(
+            einx.dot("a [->]", y, 1),
+            y,
+        )
+        assert backend.allclose(
+            einx.dot("a [b->]", x, y),
+            y * 10,
+        )
+        assert backend.allclose(
+            einx.dot("a [->b]", y, y),
+            x,
+        )
+        assert backend.allclose(
+            einx.dot("a [b->b]", x, y),
+            einx.multiply("a b, b -> a b", x, y),
+        )
 
     x = backend.to_tensor(np.arange(6)[np.newaxis])
     q, k, v = einx.rearrange("b (q+k+v) -> b q, b k, b v", x, q=2, k=2, v=2)
     assert backend.allclose(q, backend.to_tensor([[0, 1]]))
     assert backend.allclose(k, backend.to_tensor([[2, 3]]))
     assert backend.allclose(v, backend.to_tensor([[4, 5]]))
 
     x = backend.to_tensor(np.arange(4)[np.newaxis])
     q, k = einx.rearrange("b (q+k) -> b q, b k", x, q=2)
     assert backend.allclose(q, backend.to_tensor([[0, 1]]))
     assert backend.allclose(k, backend.to_tensor([[2, 3]]))
 
     x = backend.to_tensor(np.arange(4).reshape((2, 2)))
-    a, b, c, d = einx.rearrange("(a + b) (c + d) -> (a c), (a d), (b c), (b d)", x, a=1, b=1, c=1, d=1)
+    a, b, c, d = einx.rearrange(
+        "(a + b) (c + d) -> (a c), (a d), (b c), (b d)", x, a=1, b=1, c=1, d=1
+    )
     assert backend.allclose(a, backend.to_tensor([0]))
     assert backend.allclose(b, backend.to_tensor([1]))
     assert backend.allclose(c, backend.to_tensor([2]))
     assert backend.allclose(d, backend.to_tensor([3]))
 
     x = backend.to_tensor(np.arange(4)[np.newaxis])
     assert backend.allclose(
@@ -94,35 +113,46 @@
     x = backend.to_tensor(np.arange(10))
     y = backend.to_tensor(np.arange(10)[::-1].copy())
     z = backend.to_tensor(np.arange(10))
     assert backend.allclose(
         einx.get_at("[h], h2 -> h2", x, y),
         y,
     )
-    assert backend.allclose(
-        einx.set_at("[h], h2, h2 -> [h]", x, y, z),
-        y,
-    )
+    if backend.name != "mlx":
+        assert backend.allclose(
+            einx.set_at("[h], h2, h2 -> [h]", x, y, z),
+            y,
+        )
 
     assert backend.allclose(
         backend.cast(einx.arange("a b [2]", a=5, b=6, backend=backend), "int32"),
-        backend.to_tensor(np.stack(np.meshgrid(np.arange(5), np.arange(6), indexing="ij"), axis=-1).astype("int32")),
+        backend.to_tensor(
+            np.stack(np.meshgrid(np.arange(5), np.arange(6), indexing="ij"), axis=-1).astype(
+                "int32"
+            )
+        ),
     )
     assert backend.allclose(
         backend.cast(einx.arange("b a -> a b [2]", a=5, b=6, backend=backend), "int32"),
-        backend.to_tensor(np.stack(np.meshgrid(np.arange(6), np.arange(5), indexing="xy"), axis=-1).astype("int32")),
+        backend.to_tensor(
+            np.stack(np.meshgrid(np.arange(6), np.arange(5), indexing="xy"), axis=-1).astype(
+                "int32"
+            )
+        ),
     )
 
-    coord_dtype = "int32" if backend.name != "torch" else "long"
-    x = backend.to_tensor(rng.uniform(size=(4, 5, 6)).astype("float32"))
-    y = backend.cast(backend.ones((4, 5)) * 3, coord_dtype)
-    assert backend.allclose(
-        einx.get_at("... [d], ... -> ...", x, y),
-        x[:, :, 3],
-    )
+    if backend.name != "mlx":
+        coord_dtype = "int32" if backend.name != "torch" else "long"
+        x = backend.to_tensor(rng.uniform(size=(4, 5, 6)).astype("float32"))
+        y = backend.cast(backend.ones((4, 5)) * 3, coord_dtype)
+        assert backend.allclose(
+            einx.get_at("... [d], ... -> ...", x, y),
+            x[:, :, 3],
+        )
+
 
 @pytest.mark.parametrize("backend", backends)
 def test_compare_backends(backend):
     x = np.random.uniform(size=(10, 3, 10)).astype("float32")
 
     assert backend.allclose(
         backend.to_tensor(einx.sum("a [b] c", x)),
@@ -135,8 +165,8 @@
     assert backend.allclose(
         backend.to_tensor(einx.log_softmax("a [b] c", x)),
         einx.log_softmax("a [b] c", backend.to_tensor(x)),
     )
     assert backend.allclose(
         backend.to_tensor(einx.logsumexp("a [b] c", x)),
         einx.logsumexp("a [b] c", backend.to_tensor(x)),
-    )
+    )
```

