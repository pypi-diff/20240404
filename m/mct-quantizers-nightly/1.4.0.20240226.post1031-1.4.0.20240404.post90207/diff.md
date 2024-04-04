# Comparing `tmp/mct-quantizers-nightly-1.4.0.20240226.post1031.tar.gz` & `tmp/mct-quantizers-nightly-1.4.0.20240404.post90207.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.4.0.20240226.post1031.tar", last modified: Mon Feb 26 00:10:32 2024, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.4.0.20240404.post90207.tar", last modified: Thu Apr  4 09:02:08 2024, max compression
```

## Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031.tar` & `mct-quantizers-nightly-1.4.0.20240404.post90207.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.473144 mct-quantizers-nightly-1.4.0.20240226.post1031/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-02-26 00:10:32.473144 mct-quantizers-nightly-1.4.0.20240226.post1031/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.465144 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.465144 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.469143 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.469143 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.469143 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.469143 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.469143 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/onnxruntime_session_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/onnxruntime_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.473144 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.473144 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.473144 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-02-26 00:10:20.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 00:10:32.473144 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-02-26 00:10:32.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-02-26 00:10:32.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 00:10:32.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-26 00:10:32.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-26 00:10:32.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-26 00:10:32.473144 mct-quantizers-nightly-1.4.0.20240226.post1031/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-26 00:10:31.000000 mct-quantizers-nightly-1.4.0.20240226.post1031/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.949995 mct-quantizers-nightly-1.4.0.20240404.post90207/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-04 09:02:08.949995 mct-quantizers-nightly-1.4.0.20240404.post90207/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.941995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.945995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.945995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.945995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.945995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.945995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.949995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/onnxruntime_session_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/onnxruntime_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.949995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.949995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.949995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-04-04 09:01:53.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:02:08.949995 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-04 09:02:08.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-04 09:02:08.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:02:08.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 09:02:08.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 09:02:08.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 09:02:08.953995 mct-quantizers-nightly-1.4.0.20240404.post90207/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-04 09:02:07.000000 mct-quantizers-nightly-1.4.0.20240404.post90207/setup.py
```

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/LICENSE.md` & `mct-quantizers-nightly-1.4.0.20240404.post90207/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/PKG-INFO` & `mct-quantizers-nightly-1.4.0.20240404.post90207/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.4.0.20240226.post1031
+Version: 1.4.0.20240404.post90207
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/README.md` & `mct-quantizers-nightly-1.4.0.20240404.post90207/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 FOUND_ONNXRUNTIME_EXTENSIONS = importlib.util.find_spec(ONNXRUNTIME_EXTENSIONS) is not None
 
 
 ## Quantization properties
 IS_WEIGHTS = "is_weights"
 IS_ACTIVATIONS = "is_activations"
 WEIGHTS_QUANTIZERS = "weights_quantizer"
+WEIGHTS_VALUES = "weights_value"
+OP_CALL_ARGS = 'op_call_args'
+OP_CALL_KWARGS = 'op_call_kwargs'
+IS_INPUT_AS_LIST = 'is_inputs_as_list'
 WEIGHTS_QUANTIZATION_METHOD = 'weights_quantization_method'
 WEIGHTS_N_BITS = 'weights_n_bits'
 WEIGHTS_QUANTIZATION_PARAMS = 'weights_quantization_params'
 ENABLE_WEIGHTS_QUANTIZATION = 'enable_weights_quantization'
 WEIGHTS_CHANNELS_AXIS = 'weights_channels_axis'
 WEIGHTS_PER_CHANNEL_THRESHOLD = 'weights_per_channel_threshold'
 MIN_THRESHOLD = 'min_threshold'
@@ -76,9 +80,12 @@
 LAYER = "layer"
 STEPS = "optimizer_step"
 TRAINING = "training"
 EPS = 1e-8
 LUT_VALUES_BITWIDTH = 8
 MCTQ_VERSION = "mctq_version"
 
+POSITIONAL_WEIGHT = 'positional_weight'
+QUANTIZED_POSITIONAL_WEIGHT = f'quantized_{POSITIONAL_WEIGHT}'
+
 # ONNX ops domain
 ONNX_CUSTOM_OP_DOMAIN = f"mct_quantizers"
```

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/quant_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,24 +18,21 @@
 
 class QuantizationMethod(Enum):
     """
     Method for quantization function selection:
 
     POWER_OF_TWO - Symmetric, uniform, threshold is power of two quantization.
 
-    KMEANS - k-means quantization.
-
     LUT_POT_QUANTIZER - quantization using a lookup table and power of 2 threshold.
 
     SYMMETRIC - Symmetric, uniform, quantization.
 
     UNIFORM - uniform quantization,
 
     LUT_SYM_QUANTIZER - quantization using a lookup table and symmetric threshold.
 
     """
     POWER_OF_TWO = 0
-    KMEANS = 1
-    LUT_POT_QUANTIZER = 2
-    SYMMETRIC = 3
-    UNIFORM = 4
-    LUT_SYM_QUANTIZER = 5
+    LUT_POT_QUANTIZER = 1
+    SYMMETRIC = 2
+    UNIFORM = 3
+    LUT_SYM_QUANTIZER = 4
```

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,281 +7,288 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
-from typing import Dict, List, Any, Tuple
+# ==============================================================================f
+from typing import List, Union, Any, Dict, Tuple, Callable
+
+import inspect
 
 from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer
-from mct_quantizers.common.constants import FOUND_TF, WEIGHTS_QUANTIZERS, STEPS, LAYER, TRAINING, MCTQ_VERSION
+from mct_quantizers.common.constants import FOUND_TORCH, LAYER, TRAINING, POSITIONAL_WEIGHT, \
+    QUANTIZED_POSITIONAL_WEIGHT
 from mct_quantizers.logger import Logger
-from mct_quantizers.common.get_all_subclasses import get_all_subclasses
-from mct_quantizers import __version__ as mctq_version
-
-if FOUND_TF:
-    import tensorflow as tf
-    from tensorflow.python.util import tf_inspect
-    from tensorflow.python.keras.utils.control_flow_util import smart_cond
 
-    from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
+if FOUND_TORCH:
+    import torch
+    import torch.nn as nn
 
-    keras = tf.keras
 
-    def _make_quantizer_fn(quantizer, x, training):
-        """Use currying to return True/False specialized fns to the cond."""
+    class PytorchQuantizationWrapper(nn.Module):
+        def __init__(self,
+                     module: Union[nn.Module, Callable],
+                     weights_quantizers: Dict[Union[int, str], BaseInferableQuantizer],
+                     weight_values: Dict[int, torch.Tensor] = None,
+                     op_call_args: List = None,
+                     op_call_kwargs: Dict[str, Any] = None,
+                     is_inputs_as_list: bool = False):
+            """
+            The PytorchQuantizationWrapper takes a Pytorch layer and quantization information and creates
+            a quantized layer. The quantization information includes a quantizer per layer attribute for
+            a Torch layer that contains weight attributes (e.g. Conv2d, BatchNorm2d, etc.). For
+            layers that get constants (e.g. torch.add(Tensor, constant), the quantization information
+            also includes a weight values per attribute, the function call args & kwargs and a boolean for
+            whether the layer\function accepts the inputs as a list (e.g. torch.cat). Note that for a layer
+            with constants, the constants are referred to as "positional weights" whose attributes are integers
+            representing the input index in the function\layer's inputs.
 
-        def quantizer_fn():
-            return quantizer(x, training)
+            Args:
+                module: A pytorch module or as function.
+                weights_quantizers: A dictionary between a weight's name or position to its quantizer.
+                weight_values: A dictionary between a weight's position to its value.
+                op_call_args: A list containing the layer's call arguments.
+                op_call_kwargs: A dictionary containing the layer's call keyword arguments.
+                is_inputs_as_list: A boolean indicating the layer accepts the input tensors as a list.
 
-        return quantizer_fn
+            Examples:
 
+                Creating a quantized Conv2d (weight only):
 
-    def _weight_name(name: str) -> str:
-        """Extracts the weight name from the full TensorFlow variable name.
+                >>> import mct_quantizers as mctq
+                >>> import torch
 
-        For example, returns 'kernel' for 'dense_2/kernel:0'.
+                >>> attr_quant_dict = {'weight': mctq.pytorch.quantizers.WeightsPOTInferableQuantizer(4, [2.0], False)}
+                >>> QuantizedConv2D = mctq.PytorchQuantizationWrapper(torch.nn.Conv2d(3, 3, 3), attr_quant_dict)
 
-        Args:
-          name: TensorFlow variable name.
+                creating a quantized function with a constant: torch.sub(constant, Tensor)
 
-        Returns:
-          Extracted weight name.
-        """
-        return name.split(':')[0].split('/')[-1]
+                >>> attr_quant_dict = {0: mctq.pytorch.quantizers.WeightsPOTInferableQuantizer(4, [2.0], False)}
+                >>> attr_values = {0: torch.Tensor([1, 2, 3], dtype=torch.float32)}
+                >>> QuantizedSub = mctq.PytorchQuantizationWrapper(torch.sub), attr_quant_dict, attr_values)
 
+                creating a quantized function with constants and arguments: tf.cat([constant#1, Tensor, constant#2], dim=1)
+                >>> attr_quant_dict = {0: mctq.pytorch.quantizers.WeightsPOTInferableQuantizer(4, [2.0], False),
+                >>>                    2: mctq.pytorch.quantizers.WeightsPOTInferableQuantizer(4, [1.0], False)}
+                >>> attr_values = {0: torch.Tensor([[1,2,3], [4, 5, 6]], dtype=torch.float32),
+                >>>                2: torch.Tensor([[4,5,6], [4, 5, 6]], dtype=torch.float32)}
+                >>> QuantizedConcat = mctq.PytorchQuantizationWrapper(torch.cat, attr_quant_dict, attr_values,
+                >>>                                                   op_call_kwargs={'dim', 1})
 
-    class KerasQuantizationWrapper(tf.keras.layers.Wrapper):
-        def __init__(self,
-                     layer,
-                     weights_quantizers: Dict[str, BaseInferableQuantizer] = None,
-                     **kwargs):
-            """
-            Keras Quantization Wrapper takes a keras layer and quantizers and infer a quantized layer.
-
-            Args:
-                layer: A keras layer.
-                weights_quantizers: A dictionary between a weight's name to its quantizer.
             """
-            super(KerasQuantizationWrapper, self).__init__(layer, **kwargs)
-            self._track_trackable(layer, name='layer')
-
-            # making sure the attribute name is converted to the actual attribute field name in the layer.
-            self.weights_quantizers = {_weight_name(k): v for k, v in weights_quantizers.items()} \
-                if weights_quantizers is not None else dict()
-
-            self._mctq_version = mctq_version
-
-        def add_weights_quantizer(self, param_name: str, quantizer: BaseInferableQuantizer):
-            """
-            This function adds a weights quantizer to existing wrapper
-
-            Args:
-                param_name: The name of the parameter to quantize
-                quantizer: A quantizer.
+            super().__init__()
+            if isinstance(module, nn.Module):
+                self.add_module(LAYER, module)
+            else:
+                # Functional layers
+                setattr(self, LAYER, module)
 
-            Returns: None
+            self.weights_quantizers = weights_quantizers
+            # Initialize positional weights:
+            self.weight_values = weight_values if weight_values is not None else dict()
+            for pos, weight_val in self.weight_values.items():
+                if not isinstance(weight_val, torch.Tensor):
+                    Logger.error(f'Positional weight at position {pos} should be either an ndarray or a tf.Tensor,'
+                                 f'but type is {type(weight_val)}')
+
+            # Initialize functional module arguments. For examples, see the class description.
+            self.op_call_args = [] if op_call_args is None else op_call_args
+            self.op_call_kwargs = {} if op_call_kwargs is None else op_call_kwargs
+            self.is_inputs_as_list = is_inputs_as_list
+
+            # Sanity checks:
+            # 1. If there are no weight_values: verify all weight_quantizers are strings
+            # 2. If there are weight_values: verify all weight_quantizers and weight_values keys
+            #    are integers, and that they match.
+            # 3. A module with both weights as attributes and positional weights is not supported.
+            if len(self.weight_values) == 0:
+                # expecting weights_quantizers keys to be all strings.
+                if not all([isinstance(w, str) for w in self.weights_quantizers]):
+                    Logger.error('"weights_quantizers" keys should be all strings')
+                self.is_str_attr = True
+            else:
+                # expecting both weights_quantizers and weight_values keys to be all integers.
+                if not all([isinstance(w, int) for w in self.weight_values]):
+                    Logger.error('All "weight_values" keys should be integers')
+                if not all([a == b for a, b in zip(weights_quantizers, weight_values)]):
+                    Logger.error('Mismatch between "weights_quantizers" and "weight_values" keys')
+                self.is_str_attr = False
 
-            """
-            fixed_name = _weight_name(param_name)
-            self.weights_quantizers.update({fixed_name: quantizer})
+            self._set_weights_vars(True)
 
         @property
         def is_weights_quantization(self) -> bool:
             """
             This function check weights quantizer exists in wrapper.
 
-            Returns: a boolean if weights quantizer exists
+            Returns: a boolean if weights quantizer exists.
 
             """
             return self.num_weights_quantizers > 0
 
         @property
         def num_weights_quantizers(self) -> int:
             """
-            Returns: number of weights quantizers
+            Returns: number of weights quantizers.
             """
             return len(self.weights_quantizers)
 
-        def get_config(self):
+        def convert_to_inferable_quantizers(self):
             """
-            Returns: Configuration of KerasQuantizationWrapper.
+            Convert the wrapper quantizers with inferable quantizers.
 
             """
-            base_config = super(KerasQuantizationWrapper, self).get_config()
-            config = {WEIGHTS_QUANTIZERS: {k: keras.utils.serialize_keras_object(v) for k, v in self.weights_quantizers.items()}}
-
-            return_config = dict(list(base_config.items()) + list(config.items()))
-            return_config[MCTQ_VERSION] = self._mctq_version
-
-            return return_config
-
-        @property
-        def mctq_version(self):
-            return self._mctq_version
+            # Weight quantizers
+            if self.is_weights_quantization:
+                inferable_weight_quantizers = {}
+                for name, quantizer in self.weights_quantizers.items():
+                    if hasattr(quantizer, 'convert2inferable') and callable(quantizer.convert2inferable):
+                        inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
+                self.weights_quantizers = inferable_weight_quantizers
+                self._set_weights_vars(False)
 
         def _set_weights_vars(self, is_training: bool = True):
             """
-            This function sets weights quantizers vars to the layer
+            Initialize learnable weights as parameters in the wrapper, and their quantizers.
 
             Args:
-                is_training: Flag to indicate whether training or not
+                is_training: Whether working with InferableQuantizers or not. If so, do not register weight as parameter.
 
-            Returns: None
             """
             self._weights_vars = []
-            for name, quantizer in self.weights_quantizers.items():
-                weight = getattr(self.layer, name)
-                quantizer.initialize_quantization(weight.shape, _weight_name(weight.name) if is_training else None,
-                                                  self)
-                # Add weight to wrapper weight lists (rather than the layer weight lists), because it will be deleted
-                # from the layer's lists after the first call
-                self._weights_vars.append((name, weight, quantizer))
-                if is_training and not any([weight is w for w in self._trainable_weights]):
-                    self._trainable_weights.append(weight)
-                elif not is_training and any([weight is w for w in self._non_trainable_weights]):
-                    self._non_trainable_weights.append(weight)
 
-        @classmethod
-        def from_config(cls, config):
-            """
-
-            Args:
-                config(dict): dictionary  of  KerasQuantizationWrapper Configuration
+            # Init weights quantizers
+            for name, quantizer in self.weights_quantizers.items():
+                if self.is_str_attr:
+                    if is_training:
+                        weight = getattr(self.layer, name).detach()
+                        delattr(self.layer, name)
+                        setattr(self.layer, name, weight)
+                        self.register_parameter(name, torch.nn.Parameter(weight, requires_grad=True))
+                    else:
+                        weight = getattr(self, name).detach()
+                        delattr(self.layer, name)
+                        setattr(self.layer, name, weight)
+                    weight_var = getattr(self, name)
+                else:
+                    weight = self.weight_values[name]
+                    self.register_parameter(f'{POSITIONAL_WEIGHT}_{name}',
+                                            torch.nn.Parameter(weight, requires_grad=False))
+                    setattr(self, f'{QUANTIZED_POSITIONAL_WEIGHT}_{name}', weight)
+                    weight_var = getattr(self, f'{POSITIONAL_WEIGHT}_{name}')
 
-            Returns: A KerasQuantizationWrapper
+                quantizer.initialize_quantization(weight.shape, name, self)
+                self._weights_vars.append((name, weight_var, quantizer))
 
+        def set_quantize_weights(self, quantized_weights: dict):
             """
-            config = config.copy()
-            qi_inferable_custom_objects = {subclass.__name__: subclass for subclass in
-                                           get_all_subclasses(BaseKerasInferableQuantizer)}
-            weights_quantizers = {k: keras.utils.deserialize_keras_object(v,
-                                                                          module_objects=globals(),
-                                                                          custom_objects=qi_inferable_custom_objects) for k, v in config.pop(WEIGHTS_QUANTIZERS).items()}
-            layer = tf.keras.layers.deserialize(config.pop(LAYER))
-
-            v = config.pop(MCTQ_VERSION, None)
-
-            obj = cls(layer=layer, weights_quantizers=weights_quantizers, **config)
-            obj._mctq_version = mctq_version if v is None else v
+            This function updates layer weights after quantization.
 
-            return obj
-
-        def build(self, input_shape):
-            """
-            KerasQuantization Wrapper build function.
             Args:
-                input_shape: the layer input shape
+                quantized_weights: a dict of weight to update.
 
             Returns: None
 
             """
-            super(KerasQuantizationWrapper, self).build(input_shape)
-
-            self.optimizer_step = self.add_weight(
-                STEPS,
-                initializer=tf.keras.initializers.Constant(-1),
-                dtype=tf.dtypes.int32,
-                trainable=False)
-
-            self._set_weights_vars()
+            for weight_attr in self.weights_quantizers:
+                weight = quantized_weights.get(weight_attr)
+                if self.is_str_attr:
+                    setattr(self.layer, weight_attr, weight)
+                else:
+                    setattr(self, f'{QUANTIZED_POSITIONAL_WEIGHT}_{weight_attr}', weight)
 
-        def set_quantize_weights(self, quantized_weights: dict):
+        def get_weights_vars(self) -> List[Tuple[str, Any, BaseInferableQuantizer]]:
             """
-            This function update layer weights after quantization.
-
-            Args:
-                quantized_weights: a dict of weight to update
+            A getter of the layer's weights variables.
 
-            Returns: None
+            Returns:
+                List pf tuples of the wrapped layer's weights variables with weight name, values and assigned quantizer.
 
             """
-            for weight_attr in self.weights_quantizers.keys():
-                weight = quantized_weights.get(weight_attr)
-                current_weight = getattr(self.layer, weight_attr)
-                if current_weight.shape != weight.shape:
-                    Logger.error(
-                        f"Existing layer weight shape {current_weight.shape} is incompatible with provided weight "
-                        f"shape {weight.shape}")  # pragma: no cover
 
-                setattr(self.layer, weight_attr, weight)
+            return self._weights_vars
 
-        def call(self, inputs, training=None, **kwargs):
+        def forward(self,
+                    *args: List[Any],
+                    **kwargs: Dict[str, Any]) -> Union[torch.Tensor, List[torch.Tensor]]:
             """
-            KerasQuantizationWrapper call functions
+            PytorchQuantizationWrapper forward functions.
             Args:
-                inputs: Input tensors to specified layer
-                training: a boolean stating if layer is in training mode.
-                **kwargs:
+                args: arguments to pass to internal layer.
+                kwargs: key-word dictionary to pass to the internal layer.
 
-            Returns: tensors that simulate a quantized layer.
+            Returns: a tensor that simulates a quantized layer.
 
             """
-            if training is None:
-                training = tf.keras.backend.learning_phase()
 
+            # ----------------------------------
             # Quantize all weights, and replace them in the underlying layer.
-            quantized_weights = {}
-            for name, unquantized_weight, quantizer in self._weights_vars:
+            # ----------------------------------
+            if self.is_weights_quantization:
+
+                quantized_weights = {}
+                for name, unquantized_weight, quantizer in self._weights_vars:
+                    s = inspect.signature(quantizer.__call__)
+                    if TRAINING in s.parameters.keys():
+                        quantized_weight = quantizer(unquantized_weight, self.training)
+                    else:
+                        quantized_weight = quantizer(unquantized_weight)
 
-                weights_quantizer_args_spec = tf_inspect.getfullargspec(quantizer.__call__).args
-                if TRAINING in weights_quantizer_args_spec:
-                    quantized_weight = smart_cond(
-                        training,
-                        _make_quantizer_fn(quantizer, unquantized_weight, True),
-                        _make_quantizer_fn(quantizer, unquantized_weight, False))
-                    quantized_weights.update({name: quantized_weight})
-                else:
-                    # Keras weights inferable quantizer
-                    quantized_weight = quantizer(unquantized_weight)
                     quantized_weights.update({name: quantized_weight})
 
-            self.set_quantize_weights(quantized_weights)
+                self.set_quantize_weights(quantized_weights)
 
-            args_spec = tf_inspect.getfullargspec(self.layer.call).args
-            if TRAINING in args_spec:
-                outputs = self.layer.call(inputs, training=training, **kwargs)
+            if not self.is_str_attr:
+                # Positional weights need to be inserted in the wrapper input list according to their (key) position.
+                args = list(args)
+                weight_positions = [w[0] for w in self._weights_vars]
+                for pos in sorted(weight_positions):
+                    args.insert(pos, getattr(self, f'{QUANTIZED_POSITIONAL_WEIGHT}_{pos}'))
+
+            _kwargs = {**self.op_call_kwargs, **kwargs}
+            # ----------------------------------
+            # Layer operation
+            # ----------------------------------
+            if self.is_inputs_as_list:
+                outputs = self.layer(args, *self.op_call_args, **_kwargs)
             else:
-                outputs = self.layer.call(inputs, **kwargs)
+                outputs = self.layer(*args, *self.op_call_args, **_kwargs)
 
             return outputs
 
-        def get_weights_vars(self) -> List[Tuple[str, Any, BaseInferableQuantizer]]:
-            """
-            A getter of the layer's weights variables.
-
-            Returns:
-                List pf tuples of the wrapped layer's weights variables with weight name, values and assigned quantizer.
-
-            """
-
-            return self._weights_vars
-
-        def get_quantized_weights(self) -> Dict[str, tf.Tensor]:
+        def get_quantized_weights(self) -> Dict[str, torch.Tensor]:
             """
 
             Returns: A dictionary of weights attributes to quantized weights.
 
             """
             quantized_weights = {}
             weights_var = self.get_weights_vars()
             for name, w, quantizer in weights_var:
                 quantized_weights[name] = quantizer(w)
             return quantized_weights
 
 else:
-    class KerasQuantizationWrapper(object):
+    class PytorchQuantizationWrapper:
         def __init__(self,
                      layer,
-                     weights_quantizers: Dict[str, BaseInferableQuantizer] = None):
+                     weight_quantizers: Dict[str, BaseInferableQuantizer],
+                     weight_values: Dict = None,
+                     op_call_args: List = None,
+                     op_call_kwargs: Dict[str, Any] = None,
+                     is_inputs_as_list: bool = False):
             """
-            Keras Quantization Wrapper takes a keras layer and quantizers and infer a quantized layer.
+            Pytorch Quantization Wrapper takes a pytorch module and quantizers and infer a quantized layer.
 
             Args:
-                layer: A keras layer.
-                weights_quantizers: A dictionary between a weight's name to its quantizer.
-            """
-            Logger.critical('Installing tensorflow is mandatory '
-                            'when using KerasQuantizationWrapper. '
-                            'Could not find Tensorflow package.')  # pragma: no cover
+                layer: A pytorch module.
+                weight_quantizers: A dictionary between a weight's name to its quantizer.
+                weight_values: A dictionary between a weight's position to its value.
+                op_call_args: A list containing the layer's call arguments.
+                op_call_kwargs: A dictionary containing the layer's call keyword arguments.
+                is_inputs_as_list: A boolean indicating the layer accepts the input tensors as a list.
+            """
+            Logger.critical('Installing Pytorch is mandatory '
+                            'when using PytorchQuantizationWrapper. '
+                            'Could not find torch package.')  # pragma: no cover
```

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/onnxruntime_session_options.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/onnxruntime_session_options.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/onnxruntime_validations.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/onnxruntime_validations.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.4.0.20240226.post1031
+Version: 1.4.0.20240404.post90207
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.4.0.20240404.post90207/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240226.post1031/setup.py` & `mct-quantizers-nightly-1.4.0.20240404.post90207/setup.py`

 * *Files identical despite different names*

