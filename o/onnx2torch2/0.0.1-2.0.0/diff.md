# Comparing `tmp/onnx2torch2-0.0.1.tar.gz` & `tmp/onnx2torch2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2torch2-0.0.1.tar", last modified: Tue Apr  2 09:38:27 2024, max compression
+gzip compressed data, was "onnx2torch2-2.0.0.tar", last modified: Thu Apr  4 15:24:02 2024, max compression
```

## Comparing `onnx2torch2-0.0.1.tar` & `onnx2torch2-2.0.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 c         (1000) c         (1000)        0 2024-04-02 09:38:27.678471 onnx2torch2-0.0.1/
--rw-r--r--   0 c         (1000) c         (1000)    11338 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/LICENSE
--rw-r--r--   0 c         (1000) c         (1000)       26 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/MANIFEST.in
--rw-r--r--   0 c         (1000) c         (1000)    23441 2024-04-02 09:38:27.678471 onnx2torch2-0.0.1/PKG-INFO
--rw-r--r--   0 c         (1000) c         (1000)     8879 2024-03-31 07:37:28.000000 onnx2torch2-0.0.1/README.md
-drwxr-xr-x   0 c         (1000) c         (1000)        0 2024-04-02 09:38:27.668471 onnx2torch2-0.0.1/onnx2torch2/
--rw-r--r--   0 c         (1000) c         (1000)       42 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/__init__.py
--rw-r--r--   0 c         (1000) c         (1000)     7001 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/converter.py
-drwxr-xr-x   0 c         (1000) c         (1000)        0 2024-04-02 09:38:27.675138 onnx2torch2-0.0.1/onnx2torch2/node_converters/
--rw-r--r--   0 c         (1000) c         (1000)     2967 2024-03-31 06:54:06.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/__init__.py
--rw-r--r--   0 c         (1000) c         (1000)     9229 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/activations.py
--rw-r--r--   0 c         (1000) c         (1000)     2168 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/average_pool.py
--rw-r--r--   0 c         (1000) c         (1000)     1316 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/base_element_wise.py
--rw-r--r--   0 c         (1000) c         (1000)     3736 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/batch_norm.py
--rw-r--r--   0 c         (1000) c         (1000)     3003 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/binary_math_operations.py
--rw-r--r--   0 c         (1000) c         (1000)     1986 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/cast.py
--rw-r--r--   0 c         (1000) c         (1000)     3011 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/clip.py
--rw-r--r--   0 c         (1000) c         (1000)     1843 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/comparisons.py
--rw-r--r--   0 c         (1000) c         (1000)     1217 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/concat.py
--rw-r--r--   0 c         (1000) c         (1000)     2025 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/constant.py
--rw-r--r--   0 c         (1000) c         (1000)     1741 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/constant_of_shape.py
--rw-r--r--   0 c         (1000) c         (1000)     3438 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/conv.py
--rw-r--r--   0 c         (1000) c         (1000)     2827 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/cumsum.py
--rw-r--r--   0 c         (1000) c         (1000)     1387 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/depth_to_space.py
--rw-r--r--   0 c         (1000) c         (1000)     1901 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/dropout.py
--rw-r--r--   0 c         (1000) c         (1000)     1060 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/einsum.py
--rw-r--r--   0 c         (1000) c         (1000)     1512 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/expand.py
--rw-r--r--   0 c         (1000) c         (1000)     2499 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/eye_like.py
--rw-r--r--   0 c         (1000) c         (1000)     1477 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/flatten.py
--rw-r--r--   0 c         (1000) c         (1000)     2209 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/functions.py
--rw-r--r--   0 c         (1000) c         (1000)     6362 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/gather.py
--rw-r--r--   0 c         (1000) c         (1000)     3289 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/gemm.py
--rw-r--r--   0 c         (1000) c         (1000)     2452 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/global_average_pool.py
--rw-r--r--   0 c         (1000) c         (1000)     2475 2024-03-31 07:14:58.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/gridsample.py
--rw-r--r--   0 c         (1000) c         (1000)     1339 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/identity.py
--rw-r--r--   0 c         (1000) c         (1000)     3137 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/instance_norm.py
--rw-r--r--   0 c         (1000) c         (1000)     2810 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/layer_norm.py
--rw-r--r--   0 c         (1000) c         (1000)     2935 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/logical.py
--rw-r--r--   0 c         (1000) c         (1000)      899 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/lrn.py
--rw-r--r--   0 c         (1000) c         (1000)     1433 2024-03-31 07:16:28.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/matmul.py
--rw-r--r--   0 c         (1000) c         (1000)     2403 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/max_pool.py
--rw-r--r--   0 c         (1000) c         (1000)     1300 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/mean.py
--rw-r--r--   0 c         (1000) c         (1000)     1627 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/min_max.py
--rw-r--r--   0 c         (1000) c         (1000)     1304 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/mod.py
--rw-r--r--   0 c         (1000) c         (1000)      991 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/neg.py
--rw-r--r--   0 c         (1000) c         (1000)     4914 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/nms.py
--rw-r--r--   0 c         (1000) c         (1000)     4882 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/pad.py
--rw-r--r--   0 c         (1000) c         (1000)     2345 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/pow.py
--rw-r--r--   0 c         (1000) c         (1000)     2107 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/range.py
--rw-r--r--   0 c         (1000) c         (1000)     1014 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/reciprocal.py
--rw-r--r--   0 c         (1000) c         (1000)     9576 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/reduce.py
--rw-r--r--   0 c         (1000) c         (1000)     1850 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/registry.py
--rw-r--r--   0 c         (1000) c         (1000)     1853 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/reshape.py
--rw-r--r--   0 c         (1000) c         (1000)     6488 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/resize.py
--rw-r--r--   0 c         (1000) c         (1000)     5565 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/roialign.py
--rw-r--r--   0 c         (1000) c         (1000)     1392 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/roundings.py
--rw-r--r--   0 c         (1000) c         (1000)     3689 2024-03-31 07:07:26.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/scatter_nd.py
--rw-r--r--   0 c         (1000) c         (1000)     2468 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/shape.py
--rw-r--r--   0 c         (1000) c         (1000)     4346 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/slice.py
--rw-r--r--   0 c         (1000) c         (1000)     2809 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/split.py
--rw-r--r--   0 c         (1000) c         (1000)     3473 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/squeeze.py
--rw-r--r--   0 c         (1000) c         (1000)     1217 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/sum.py
--rw-r--r--   0 c         (1000) c         (1000)     1748 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/tile.py
--rw-r--r--   0 c         (1000) c         (1000)     1819 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/topk.py
--rw-r--r--   0 c         (1000) c         (1000)     1718 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/transpose.py
--rw-r--r--   0 c         (1000) c         (1000)     2950 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/unsqueeze.py
--rw-r--r--   0 c         (1000) c         (1000)     1054 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/node_converters/where.py
--rw-r--r--   0 c         (1000) c         (1000)     4375 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/onnx_graph.py
--rw-r--r--   0 c         (1000) c         (1000)     2621 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/onnx_node.py
--rw-r--r--   0 c         (1000) c         (1000)     1241 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/onnx_tensor.py
-drwxr-xr-x   0 c         (1000) c         (1000)        0 2024-04-02 09:38:27.678471 onnx2torch2-0.0.1/onnx2torch2/utils/
--rw-r--r--   0 c         (1000) c         (1000)        0 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/utils/__init__.py
--rw-r--r--   0 c         (1000) c         (1000)     2544 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/utils/common.py
--rw-r--r--   0 c         (1000) c         (1000)     3194 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/utils/custom_export_to_onnx.py
--rw-r--r--   0 c         (1000) c         (1000)     2247 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/utils/dtype.py
--rw-r--r--   0 c         (1000) c         (1000)      633 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/utils/indices.py
--rw-r--r--   0 c         (1000) c         (1000)     1125 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/utils/padding.py
--rw-r--r--   0 c         (1000) c         (1000)     1620 2024-03-28 11:33:17.000000 onnx2torch2-0.0.1/onnx2torch2/utils/safe_shape_inference.py
-drwxr-xr-x   0 c         (1000) c         (1000)        0 2024-04-02 09:38:27.678471 onnx2torch2-0.0.1/onnx2torch2.egg-info/
--rw-r--r--   0 c         (1000) c         (1000)    23441 2024-04-02 09:38:27.000000 onnx2torch2-0.0.1/onnx2torch2.egg-info/PKG-INFO
--rw-r--r--   0 c         (1000) c         (1000)     2871 2024-04-02 09:38:27.000000 onnx2torch2-0.0.1/onnx2torch2.egg-info/SOURCES.txt
--rw-r--r--   0 c         (1000) c         (1000)        1 2024-04-02 09:38:27.000000 onnx2torch2-0.0.1/onnx2torch2.egg-info/dependency_links.txt
--rw-r--r--   0 c         (1000) c         (1000)      163 2024-04-02 09:38:27.000000 onnx2torch2-0.0.1/onnx2torch2.egg-info/requires.txt
--rw-r--r--   0 c         (1000) c         (1000)       12 2024-04-02 09:38:27.000000 onnx2torch2-0.0.1/onnx2torch2.egg-info/top_level.txt
--rw-r--r--   0 c         (1000) c         (1000)     1775 2024-04-02 09:37:49.000000 onnx2torch2-0.0.1/pyproject.toml
--rw-r--r--   0 c         (1000) c         (1000)       38 2024-04-02 09:38:27.678471 onnx2torch2-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:24:02.889019 onnx2torch2-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-04-04 15:24:02.889019 onnx2torch2-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:24:02.877019 onnx2torch2-2.0.0/onnx2torch2/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:24:02.885019 onnx2torch2-2.0.0/onnx2torch2/node_converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/base_element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/binary_math_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/constant_of_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/depth_to_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/einsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/eye_like.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/gemm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/global_average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/gridsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/instance_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/lrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/max_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/neg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/pow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/roialign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/roundings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/scatter_nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/topk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/node_converters/where.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/onnx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/onnx_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/onnx_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:24:02.889019 onnx2torch2-2.0.0/onnx2torch2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/utils/custom_export_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/utils/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/utils/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/utils/padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/onnx2torch2/utils/safe_shape_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:24:02.889019 onnx2torch2-2.0.0/onnx2torch2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-04-04 15:24:02.000000 onnx2torch2-2.0.0/onnx2torch2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-04 15:24:02.000000 onnx2torch2-2.0.0/onnx2torch2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:24:02.000000 onnx2torch2-2.0.0/onnx2torch2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-04 15:24:02.000000 onnx2torch2-2.0.0/onnx2torch2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 15:24:02.000000 onnx2torch2-2.0.0/onnx2torch2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-04 15:23:52.000000 onnx2torch2-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:24:02.889019 onnx2torch2-2.0.0/setup.cfg
```

### Comparing `onnx2torch2-0.0.1/LICENSE` & `onnx2torch2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/PKG-INFO` & `onnx2torch2-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2torch2
-Version: 0.0.1
+Version: 2.0.0
 Summary: ONNX to PyTorch converter
 Author-email: untetherai <info@untether.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -362,15 +362,15 @@
 
 #### :page_facing_up: List of currently supported operations can be founded [here](operators.md).
 
 ## How to add new operations to converter
 
 Here we show how to extend onnx2torch2 with new ONNX operation, that supported by both PyTorch and ONNX
 <details>
-<summary>and has the same behavior</summary>
+<summary>and has the same behaviour</summary>
 
 An example of such a module is [Relu](./onnx2torch2/node_converters/activations.py)
 
 ```python
 @add_converter(operation_type='Relu', version=6)
 @add_converter(operation_type='Relu', version=13)
 @add_converter(operation_type='Relu', version=14)
@@ -379,19 +379,19 @@
         torch_module=nn.ReLU(),
         onnx_mapping=onnx_mapping_from_node(node=node),
     )
 ```
 
 Here we have registered an operation named ``Relu`` for opset versions 6, 13, 14.
 Note that the ``torch_module`` argument in ``OperationConverterResult`` must be a torch.nn.Module, not just a callable object!
-If Operation's behavior differs from one opset version to another, you should implement it separately.
+If Operation's behaviour differs from one opset version to another, you should implement it separately.
 </details>
 
 <details>
-<summary>but has different behavior</summary>
+<summary>but has different behaviour</summary>
 
 An example of such a module is [ScatterND](./onnx2torch2/node_converters/scatter_nd.py)
 
 ```python
 # It is recommended to use Enum for string ONNX attributes.
 class ReductionOnnxAttr(Enum):
     NONE = 'none'
```

### Comparing `onnx2torch2-0.0.1/README.md` & `onnx2torch2-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
 #### :page_facing_up: List of currently supported operations can be founded [here](operators.md).
 
 ## How to add new operations to converter
 
 Here we show how to extend onnx2torch2 with new ONNX operation, that supported by both PyTorch and ONNX
 <details>
-<summary>and has the same behavior</summary>
+<summary>and has the same behaviour</summary>
 
 An example of such a module is [Relu](./onnx2torch2/node_converters/activations.py)
 
 ```python
 @add_converter(operation_type='Relu', version=6)
 @add_converter(operation_type='Relu', version=13)
 @add_converter(operation_type='Relu', version=14)
@@ -137,19 +137,19 @@
         torch_module=nn.ReLU(),
         onnx_mapping=onnx_mapping_from_node(node=node),
     )
 ```
 
 Here we have registered an operation named ``Relu`` for opset versions 6, 13, 14.
 Note that the ``torch_module`` argument in ``OperationConverterResult`` must be a torch.nn.Module, not just a callable object!
-If Operation's behavior differs from one opset version to another, you should implement it separately.
+If Operation's behaviour differs from one opset version to another, you should implement it separately.
 </details>
 
 <details>
-<summary>but has different behavior</summary>
+<summary>but has different behaviour</summary>
 
 An example of such a module is [ScatterND](./onnx2torch2/node_converters/scatter_nd.py)
 
 ```python
 # It is recommended to use Enum for string ONNX attributes.
 class ReductionOnnxAttr(Enum):
     NONE = 'none'
```

### Comparing `onnx2torch2-0.0.1/onnx2torch2/converter.py` & `onnx2torch2-2.0.0/onnx2torch2/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/__init__.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/activations.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/activations.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/average_pool.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/average_pool.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/base_element_wise.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/base_element_wise.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/batch_norm.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/binary_math_operations.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/binary_math_operations.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/cast.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/cast.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/clip.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/clip.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/comparisons.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/comparisons.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/concat.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/concat.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/constant.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/constant.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/constant_of_shape.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/conv.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/conv.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/cumsum.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/cumsum.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/depth_to_space.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/depth_to_space.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/dropout.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/einsum.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/einsum.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/expand.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/expand.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/eye_like.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/eye_like.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/flatten.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/flatten.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/functions.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/functions.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/gather.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/gather.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/gemm.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/gemm.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/global_average_pool.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/global_average_pool.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/gridsample.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/gridsample.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/identity.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/identity.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/instance_norm.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/instance_norm.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/layer_norm.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/layer_norm.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/logical.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/logical.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/lrn.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/lrn.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/matmul.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/matmul.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/max_pool.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/max_pool.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/mean.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/mean.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/min_max.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/min_max.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/mod.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/mod.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/neg.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/neg.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/nms.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/nms.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/pad.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/pad.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/pow.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/pow.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/range.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/range.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/reciprocal.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/reciprocal.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/reduce.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/reduce.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/registry.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/registry.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/reshape.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/reshape.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/resize.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/resize.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/roialign.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/roialign.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/roundings.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/roundings.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/scatter_nd.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/scatter_nd.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/shape.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/shape.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/slice.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/split.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/split.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/squeeze.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/squeeze.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/sum.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/sum.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/tile.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/tile.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/topk.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/topk.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/transpose.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/transpose.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/unsqueeze.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/unsqueeze.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/node_converters/where.py` & `onnx2torch2-2.0.0/onnx2torch2/node_converters/where.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/onnx_graph.py` & `onnx2torch2-2.0.0/onnx2torch2/onnx_graph.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/onnx_node.py` & `onnx2torch2-2.0.0/onnx2torch2/onnx_node.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/onnx_tensor.py` & `onnx2torch2-2.0.0/onnx2torch2/onnx_tensor.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/utils/common.py` & `onnx2torch2-2.0.0/onnx2torch2/utils/common.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/utils/custom_export_to_onnx.py` & `onnx2torch2-2.0.0/onnx2torch2/utils/custom_export_to_onnx.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/utils/dtype.py` & `onnx2torch2-2.0.0/onnx2torch2/utils/dtype.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/utils/indices.py` & `onnx2torch2-2.0.0/onnx2torch2/utils/indices.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/utils/padding.py` & `onnx2torch2-2.0.0/onnx2torch2/utils/padding.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2/utils/safe_shape_inference.py` & `onnx2torch2-2.0.0/onnx2torch2/utils/safe_shape_inference.py`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/onnx2torch2.egg-info/PKG-INFO` & `onnx2torch2-2.0.0/onnx2torch2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2torch2
-Version: 0.0.1
+Version: 2.0.0
 Summary: ONNX to PyTorch converter
 Author-email: untetherai <info@untether.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -362,15 +362,15 @@
 
 #### :page_facing_up: List of currently supported operations can be founded [here](operators.md).
 
 ## How to add new operations to converter
 
 Here we show how to extend onnx2torch2 with new ONNX operation, that supported by both PyTorch and ONNX
 <details>
-<summary>and has the same behavior</summary>
+<summary>and has the same behaviour</summary>
 
 An example of such a module is [Relu](./onnx2torch2/node_converters/activations.py)
 
 ```python
 @add_converter(operation_type='Relu', version=6)
 @add_converter(operation_type='Relu', version=13)
 @add_converter(operation_type='Relu', version=14)
@@ -379,19 +379,19 @@
         torch_module=nn.ReLU(),
         onnx_mapping=onnx_mapping_from_node(node=node),
     )
 ```
 
 Here we have registered an operation named ``Relu`` for opset versions 6, 13, 14.
 Note that the ``torch_module`` argument in ``OperationConverterResult`` must be a torch.nn.Module, not just a callable object!
-If Operation's behavior differs from one opset version to another, you should implement it separately.
+If Operation's behaviour differs from one opset version to another, you should implement it separately.
 </details>
 
 <details>
-<summary>but has different behavior</summary>
+<summary>but has different behaviour</summary>
 
 An example of such a module is [ScatterND](./onnx2torch2/node_converters/scatter_nd.py)
 
 ```python
 # It is recommended to use Enum for string ONNX attributes.
 class ReductionOnnxAttr(Enum):
     NONE = 'none'
```

### Comparing `onnx2torch2-0.0.1/onnx2torch2.egg-info/SOURCES.txt` & `onnx2torch2-2.0.0/onnx2torch2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnx2torch2-0.0.1/pyproject.toml` & `onnx2torch2-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'onnx2torch2'
-version = '0.0.1'
+version = '2.0.0'
 license = {file = 'LICENSE'}
 description = 'ONNX to PyTorch converter'
 readme = {file = 'README.md', content-type = 'text/markdown'}
 keywords = ['AI', 'onnx', 'torch', 'onnx2torch2', 'converters']
 authors = [{name = 'untetherai', email = 'info@untether.ai'}]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
```

