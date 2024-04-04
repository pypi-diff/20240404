# Comparing `tmp/irtorch-0.0.2.tar.gz` & `tmp/irtorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irtorch-0.0.2.tar", last modified: Wed Apr  3 14:54:47 2024, max compression
+gzip compressed data, was "irtorch-0.0.3.tar", last modified: Thu Apr  4 11:56:24 2024, max compression
```

## Comparing `irtorch-0.0.2.tar` & `irtorch-0.0.3.tar`

### file list

```diff
@@ -1,93 +1,98 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.156587 irtorch-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-02-08 14:34:51.000000 irtorch-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2227 2024-04-03 14:54:47.156426 irtorch-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2024-03-08 15:11:37.000000 irtorch-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.111557 irtorch-0.0.2/irtorch/
--rw-rw-rw-   0        0        0      255 2024-04-03 14:54:41.000000 irtorch-0.0.2/irtorch/__init__.py
--rw-rw-rw-   0        0        0    14040 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/_internal_utils.py
--rw-rw-rw-   0        0        0     3279 2024-02-25 18:33:40.000000 irtorch-0.0.2/irtorch/activation_functions.py
--rw-rw-rw-   0        0        0     1000 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/config.py
--rw-rw-rw-   0        0        0     5326 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/cross_validation.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.096872 irtorch-0.0.2/irtorch/datasets/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.130662 irtorch-0.0.2/irtorch/datasets/big_five/
--rw-rw-rw-   0        0        0  3944929 2024-02-27 14:06:14.000000 irtorch-0.0.2/irtorch/datasets/big_five/big_five.pt
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.134908 irtorch-0.0.2/irtorch/datasets/national_mathematics/
--rw-rw-rw-   0        0        0   114121 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/datasets/national_mathematics/mathematics_1.pt
--rw-rw-rw-   0        0        0   158089 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/datasets/national_mathematics/mathematics_2.pt
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.139115 irtorch-0.0.2/irtorch/estimation_algorithms/
--rw-rw-rw-   0        0        0      104 2024-02-08 14:34:51.000000 irtorch-0.0.2/irtorch/estimation_algorithms/__init__.py
--rw-rw-rw-   0        0        0    15436 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/estimation_algorithms/aeirt.py
--rw-rw-rw-   0        0        0     2893 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/estimation_algorithms/base_irt_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.142570 irtorch-0.0.2/irtorch/estimation_algorithms/encoders/
--rw-rw-rw-   0        0        0      184 2024-02-08 14:34:51.000000 irtorch-0.0.2/irtorch/estimation_algorithms/encoders/__init__.py
--rw-rw-rw-   0        0        0      751 2024-02-20 20:30:27.000000 irtorch-0.0.2/irtorch/estimation_algorithms/encoders/base_encoder.py
--rw-rw-rw-   0        0        0     1427 2024-02-20 20:30:27.000000 irtorch-0.0.2/irtorch/estimation_algorithms/encoders/bounded_encoder.py
--rw-rw-rw-   0        0        0     1361 2024-02-20 20:30:27.000000 irtorch-0.0.2/irtorch/estimation_algorithms/encoders/standard_encoder.py
--rw-rw-rw-   0        0        0     1478 2024-02-20 20:30:27.000000 irtorch-0.0.2/irtorch/estimation_algorithms/encoders/variational_encoder.py
--rw-rw-rw-   0        0        0    14858 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/estimation_algorithms/vaeirt.py
--rw-rw-rw-   0        0        0     3526 2024-02-20 20:30:27.000000 irtorch-0.0.2/irtorch/gaussian_mixture_torch.py
--rw-rw-rw-   0        0        0    67273 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/irt.py
--rw-rw-rw-   0        0        0    34265 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/irt_evaluator.py
--rw-rw-rw-   0        0        0    55406 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/irt_plotter.py
--rw-rw-rw-   0        0        0    61121 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/irt_scorer.py
--rw-rw-rw-   0        0        0     2644 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/latent_variable_functions.py
--rw-rw-rw-   0        0        0     8310 2024-02-20 20:30:27.000000 irtorch-0.0.2/irtorch/layers.py
--rw-rw-rw-   0        0        0     5099 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/load_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.144835 irtorch-0.0.2/irtorch/models/
--rw-rw-rw-   0        0        0      115 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/models/__init__.py
--rw-rw-rw-   0        0        0     8057 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/models/base_irt_model.py
--rw-rw-rw-   0        0        0    13816 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/models/monotone_nn.py
--rw-rw-rw-   0        0        0    13397 2024-04-03 14:22:41.000000 irtorch-0.0.2/irtorch/models/parametric.py
--rw-rw-rw-   0        0        0     6868 2024-02-25 18:33:40.000000 irtorch-0.0.2/irtorch/outlier_detector.py
--rw-rw-rw-   0        0        0     3163 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/quantile_mv_normal.py
--rw-rw-rw-   0        0        0      767 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/timer.py
--rw-rw-rw-   0        0        0     6670 2024-03-08 13:28:02.000000 irtorch-0.0.2/irtorch/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:47.126828 irtorch-0.0.2/irtorch.egg-info/
--rw-rw-rw-   0        0        0     2227 2024-04-03 14:54:46.000000 irtorch-0.0.2/irtorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1874 2024-04-03 14:54:47.000000 irtorch-0.0.2/irtorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:54:46.000000 irtorch-0.0.2/irtorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-08 14:36:17.000000 irtorch-0.0.2/irtorch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      161 2024-04-03 14:54:46.000000 irtorch-0.0.2/irtorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 14:54:46.000000 irtorch-0.0.2/irtorch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 14:54:47.156587 irtorch-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1181 2024-04-03 14:54:29.000000 irtorch-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:50.946751 irtorch-0.0.2/tests/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:54:51.166528 irtorch-0.0.2/tests/__pycache__/
--rw-rw-rw-   0        0        0     5098 2024-04-03 14:54:50.947257 irtorch-0.0.2/tests/__pycache__/test_activation_functions.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    13774 2024-04-03 14:54:50.950631 irtorch-0.0.2/tests/__pycache__/test_aeirt.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    30081 2024-04-03 14:54:50.963541 irtorch-0.0.2/tests/__pycache__/test_base_irt_model.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     9527 2024-04-03 14:54:50.966545 irtorch-0.0.2/tests/__pycache__/test_config.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     5111 2024-04-03 14:54:50.970543 irtorch-0.0.2/tests/__pycache__/test_gaussian_mixture_torch.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0      175 2024-04-03 14:54:50.970543 irtorch-0.0.2/tests/__pycache__/test_integration.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    33306 2024-04-03 14:54:50.977472 irtorch-0.0.2/tests/__pycache__/test_internal_utils.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    86867 2024-04-03 14:54:51.064998 irtorch-0.0.2/tests/__pycache__/test_irt_evaluator.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     3508 2024-04-03 14:54:51.067507 irtorch-0.0.2/tests/__pycache__/test_irt_plotter.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    45494 2024-04-03 14:54:51.080524 irtorch-0.0.2/tests/__pycache__/test_irt_scorer.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    21348 2024-04-03 14:54:51.088029 irtorch-0.0.2/tests/__pycache__/test_latent_variable_functions.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    32202 2024-04-03 14:54:51.096536 irtorch-0.0.2/tests/__pycache__/test_layers.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    21163 2024-04-03 14:54:51.102688 irtorch-0.0.2/tests/__pycache__/test_load_dataset.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    44373 2024-04-03 14:54:51.116570 irtorch-0.0.2/tests/__pycache__/test_monotone_nn.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    12294 2024-04-03 14:54:51.123313 irtorch-0.0.2/tests/__pycache__/test_outlier_detector.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    48430 2024-04-03 14:54:51.141862 irtorch-0.0.2/tests/__pycache__/test_parametric.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    17322 2024-04-03 14:54:51.147775 irtorch-0.0.2/tests/__pycache__/test_quantile_mv_normal.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    19709 2024-04-03 14:54:51.158334 irtorch-0.0.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    20215 2024-04-03 14:54:51.166528 irtorch-0.0.2/tests/__pycache__/test_vaeirt.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     1132 2024-02-20 20:30:27.000000 irtorch-0.0.2/tests/test_activation_functions.py
--rw-rw-rw-   0        0        0     4099 2024-03-08 13:28:02.000000 irtorch-0.0.2/tests/test_aeirt.py
--rw-rw-rw-   0        0        0     5085 2024-04-03 14:22:41.000000 irtorch-0.0.2/tests/test_base_irt_model.py
--rw-rw-rw-   0        0        0      984 2024-02-21 12:30:49.000000 irtorch-0.0.2/tests/test_config.py
--rw-rw-rw-   0        0        0      924 2024-02-08 14:34:51.000000 irtorch-0.0.2/tests/test_gaussian_mixture_torch.py
--rw-rw-rw-   0        0        0     9673 2024-03-08 13:28:02.000000 irtorch-0.0.2/tests/test_integration.py
--rw-rw-rw-   0        0        0     7678 2024-04-03 14:22:41.000000 irtorch-0.0.2/tests/test_internal_utils.py
--rw-rw-rw-   0        0        0    17038 2024-04-03 14:22:41.000000 irtorch-0.0.2/tests/test_irt_evaluator.py
--rw-rw-rw-   0        0        0     3632 2024-02-25 18:33:40.000000 irtorch-0.0.2/tests/test_irt_plotter.py
--rw-rw-rw-   0        0        0    14108 2024-04-03 14:22:41.000000 irtorch-0.0.2/tests/test_irt_scorer.py
--rw-rw-rw-   0        0        0     3310 2024-03-08 13:28:02.000000 irtorch-0.0.2/tests/test_latent_variable_functions.py
--rw-rw-rw-   0        0        0     5111 2024-02-08 14:34:51.000000 irtorch-0.0.2/tests/test_layers.py
--rw-rw-rw-   0        0        0     1803 2024-04-03 14:22:41.000000 irtorch-0.0.2/tests/test_load_dataset.py
--rw-rw-rw-   0        0        0     9007 2024-03-08 13:28:02.000000 irtorch-0.0.2/tests/test_monotone_nn.py
--rw-rw-rw-   0        0        0     2850 2024-02-08 14:34:51.000000 irtorch-0.0.2/tests/test_outlier_detector.py
--rw-rw-rw-   0        0        0    10121 2024-04-03 14:22:41.000000 irtorch-0.0.2/tests/test_parametric.py
--rw-rw-rw-   0        0        0     3252 2024-02-08 14:34:51.000000 irtorch-0.0.2/tests/test_quantile_mv_normal.py
--rw-rw-rw-   0        0        0     4670 2024-03-08 13:28:02.000000 irtorch-0.0.2/tests/test_utils.py
--rw-rw-rw-   0        0        0     6369 2024-03-08 13:28:02.000000 irtorch-0.0.2/tests/test_vaeirt.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.319711 irtorch-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-02-08 14:34:51.000000 irtorch-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2227 2024-04-04 11:56:24.319711 irtorch-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2024-03-08 15:11:37.000000 irtorch-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.257140 irtorch-0.0.3/irtorch/
+-rw-rw-rw-   0        0        0      255 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/__init__.py
+-rw-rw-rw-   0        0        0    14040 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/_internal_utils.py
+-rw-rw-rw-   0        0        0     3279 2024-02-25 18:33:40.000000 irtorch-0.0.3/irtorch/activation_functions.py
+-rw-rw-rw-   0        0        0     1000 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/config.py
+-rw-rw-rw-   0        0        0     5326 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/cross_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.246655 irtorch-0.0.3/irtorch/datasets/
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.277765 irtorch-0.0.3/irtorch/datasets/big_five/
+-rw-rw-rw-   0        0        0  3944929 2024-02-27 14:06:14.000000 irtorch-0.0.3/irtorch/datasets/big_five/big_five.pt
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.281717 irtorch-0.0.3/irtorch/datasets/national_mathematics/
+-rw-rw-rw-   0        0        0   114121 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/datasets/national_mathematics/mathematics_1.pt
+-rw-rw-rw-   0        0        0   158089 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/datasets/national_mathematics/mathematics_2.pt
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.300421 irtorch-0.0.3/irtorch/datasets/swedish_sat/
+-rw-rw-rw-   0        0        0 12183084 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt
+-rw-rw-rw-   0        0        0 12183079 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt
+-rw-rw-rw-   0        0        0       80 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/datasets/swedish_sat/swesat22b_quant_correct.txt
+-rw-rw-rw-   0        0        0       82 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/datasets/swedish_sat/swesat22b_verb_correct.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.302421 irtorch-0.0.3/irtorch/estimation_algorithms/
+-rw-rw-rw-   0        0        0      104 2024-02-08 14:34:51.000000 irtorch-0.0.3/irtorch/estimation_algorithms/__init__.py
+-rw-rw-rw-   0        0        0    14839 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/estimation_algorithms/aeirt.py
+-rw-rw-rw-   0        0        0     2893 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/estimation_algorithms/base_irt_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.305967 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/
+-rw-rw-rw-   0        0        0      184 2024-02-08 14:34:51.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/__init__.py
+-rw-rw-rw-   0        0        0      751 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/base_encoder.py
+-rw-rw-rw-   0        0        0     1427 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/bounded_encoder.py
+-rw-rw-rw-   0        0        0     1361 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/standard_encoder.py
+-rw-rw-rw-   0        0        0     1478 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/variational_encoder.py
+-rw-rw-rw-   0        0        0    14716 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/estimation_algorithms/vaeirt.py
+-rw-rw-rw-   0        0        0     4002 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/gaussian_mixture_model.py
+-rw-rw-rw-   0        0        0    67068 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/irt.py
+-rw-rw-rw-   0        0        0    34307 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/irt_evaluator.py
+-rw-rw-rw-   0        0        0    55406 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/irt_plotter.py
+-rw-rw-rw-   0        0        0    62880 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/irt_scorer.py
+-rw-rw-rw-   0        0        0     2644 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/latent_variable_functions.py
+-rw-rw-rw-   0        0        0     8310 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/layers.py
+-rw-rw-rw-   0        0        0     5099 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/load_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.307967 irtorch-0.0.3/irtorch/models/
+-rw-rw-rw-   0        0        0      115 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/models/__init__.py
+-rw-rw-rw-   0        0        0     8057 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/models/base_irt_model.py
+-rw-rw-rw-   0        0        0    13816 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/models/monotone_nn.py
+-rw-rw-rw-   0        0        0    13397 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/models/parametric.py
+-rw-rw-rw-   0        0        0     6868 2024-02-25 18:33:40.000000 irtorch-0.0.3/irtorch/outlier_detector.py
+-rw-rw-rw-   0        0        0     3163 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/quantile_mv_normal.py
+-rw-rw-rw-   0        0        0      767 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/timer.py
+-rw-rw-rw-   0        0        0     6670 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.276945 irtorch-0.0.3/irtorch.egg-info/
+-rw-rw-rw-   0        0        0     2227 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2098 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-08 14:36:17.000000 irtorch-0.0.3/irtorch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 11:56:24.319711 irtorch-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1099 2024-04-04 11:55:33.000000 irtorch-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:28.045904 irtorch-0.0.3/tests/
+drwxrwxrwx   0        0        0        0 2024-04-04 11:56:28.499829 irtorch-0.0.3/tests/__pycache__/
+-rw-rw-rw-   0        0        0     5098 2024-04-04 11:56:28.047904 irtorch-0.0.3/tests/__pycache__/test_activation_functions.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    13774 2024-04-04 11:56:28.059825 irtorch-0.0.3/tests/__pycache__/test_aeirt.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    30081 2024-04-04 11:56:28.070861 irtorch-0.0.3/tests/__pycache__/test_base_irt_model.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     9527 2024-04-04 11:56:28.074860 irtorch-0.0.3/tests/__pycache__/test_config.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    15714 2024-04-04 11:56:28.080860 irtorch-0.0.3/tests/__pycache__/test_gaussian_mixture_torch.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0      175 2024-04-04 11:56:28.081861 irtorch-0.0.3/tests/__pycache__/test_integration.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    33306 2024-04-04 11:56:28.092861 irtorch-0.0.3/tests/__pycache__/test_internal_utils.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    86867 2024-04-04 11:56:28.117860 irtorch-0.0.3/tests/__pycache__/test_irt_evaluator.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     3508 2024-04-04 11:56:28.121860 irtorch-0.0.3/tests/__pycache__/test_irt_plotter.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    50778 2024-04-04 11:56:28.170475 irtorch-0.0.3/tests/__pycache__/test_irt_scorer.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    21348 2024-04-04 11:56:28.178475 irtorch-0.0.3/tests/__pycache__/test_latent_variable_functions.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    32202 2024-04-04 11:56:28.440395 irtorch-0.0.3/tests/__pycache__/test_layers.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    21163 2024-04-04 11:56:28.444405 irtorch-0.0.3/tests/__pycache__/test_load_dataset.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    44373 2024-04-04 11:56:28.452909 irtorch-0.0.3/tests/__pycache__/test_monotone_nn.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    12294 2024-04-04 11:56:28.452909 irtorch-0.0.3/tests/__pycache__/test_outlier_detector.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    48430 2024-04-04 11:56:28.468585 irtorch-0.0.3/tests/__pycache__/test_parametric.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    17322 2024-04-04 11:56:28.484207 irtorch-0.0.3/tests/__pycache__/test_quantile_mv_normal.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    19709 2024-04-04 11:56:28.484207 irtorch-0.0.3/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    20215 2024-04-04 11:56:28.499829 irtorch-0.0.3/tests/__pycache__/test_vaeirt.cpython-311-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     1132 2024-02-20 20:30:27.000000 irtorch-0.0.3/tests/test_activation_functions.py
+-rw-rw-rw-   0        0        0     4099 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_aeirt.py
+-rw-rw-rw-   0        0        0     5085 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_base_irt_model.py
+-rw-rw-rw-   0        0        0      984 2024-02-21 12:30:49.000000 irtorch-0.0.3/tests/test_config.py
+-rw-rw-rw-   0        0        0     2196 2024-04-04 11:55:33.000000 irtorch-0.0.3/tests/test_gaussian_mixture_torch.py
+-rw-rw-rw-   0        0        0     9673 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_integration.py
+-rw-rw-rw-   0        0        0     7678 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_internal_utils.py
+-rw-rw-rw-   0        0        0    17038 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_irt_evaluator.py
+-rw-rw-rw-   0        0        0     3632 2024-02-25 18:33:40.000000 irtorch-0.0.3/tests/test_irt_plotter.py
+-rw-rw-rw-   0        0        0    14999 2024-04-04 11:55:33.000000 irtorch-0.0.3/tests/test_irt_scorer.py
+-rw-rw-rw-   0        0        0     3310 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_latent_variable_functions.py
+-rw-rw-rw-   0        0        0     5111 2024-02-08 14:34:51.000000 irtorch-0.0.3/tests/test_layers.py
+-rw-rw-rw-   0        0        0     1803 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_load_dataset.py
+-rw-rw-rw-   0        0        0     9007 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_monotone_nn.py
+-rw-rw-rw-   0        0        0     2850 2024-02-08 14:34:51.000000 irtorch-0.0.3/tests/test_outlier_detector.py
+-rw-rw-rw-   0        0        0    10121 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_parametric.py
+-rw-rw-rw-   0        0        0     3252 2024-02-08 14:34:51.000000 irtorch-0.0.3/tests/test_quantile_mv_normal.py
+-rw-rw-rw-   0        0        0     4670 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_utils.py
+-rw-rw-rw-   0        0        0     6369 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_vaeirt.py
```

### Comparing `irtorch-0.0.2/LICENSE.txt` & `irtorch-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/PKG-INFO` & `irtorch-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irtorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: IRTorch: An item response theory package for python.
 Home-page: https://github.com/joakimwallmark/irtorch
 Author: Joakim Wallmark
 Author-email: wallmark.joakim@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `irtorch-0.0.2/README.md` & `irtorch-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/_internal_utils.py` & `irtorch-0.0.3/irtorch/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/activation_functions.py` & `irtorch-0.0.3/irtorch/activation_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/config.py` & `irtorch-0.0.3/irtorch/config.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/cross_validation.py` & `irtorch-0.0.3/irtorch/cross_validation.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/datasets/big_five/big_five.pt` & `irtorch-0.0.3/irtorch/datasets/big_five/big_five.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/datasets/national_mathematics/mathematics_1.pt` & `irtorch-0.0.3/irtorch/datasets/national_mathematics/mathematics_1.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/datasets/national_mathematics/mathematics_2.pt` & `irtorch-0.0.3/irtorch/datasets/national_mathematics/mathematics_2.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/estimation_algorithms/aeirt.py` & `irtorch-0.0.3/irtorch/estimation_algorithms/aeirt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import copy
 import torch
 from torch import nn
-from torch.utils.tensorboard import SummaryWriter
 from irtorch.models import BaseIRTModel
 from irtorch.estimation_algorithms import BaseIRTAlgorithm
 from irtorch.estimation_algorithms.encoders import BaseEncoder, StandardEncoder
 from irtorch._internal_utils import dynamic_print, PytorchIRTDataset
 from irtorch.utils import one_hot_encode_test_data, decode_one_hot_test_data
 
 logger = logging.getLogger('irtorch')
@@ -34,19 +33,17 @@
         self,
         model: BaseIRTModel,
         encoder: BaseEncoder = None,
         one_hot_encoded: bool = False,
         hidden_layers_encoder: list[int] = None,
         nonlinear_encoder = torch.nn.ELU(),
         batch_normalization_encoder: bool = True,
-        summary_writer: SummaryWriter = None,
     ):
         super().__init__(model = model, one_hot_encoded=one_hot_encoded)
         self.imputation_method = "zero"
-        self.summary_writer = summary_writer
         self.batch_normalization = batch_normalization_encoder
 
         if encoder is not None and self.model is not None:
             if encoder.latent_variables != self.model.latent_variables:
                 raise ValueError(
                     "Encoder and decoder must have the same number of latent variables"
                 )
@@ -230,17 +227,14 @@
 
         # Load the best model state
         if best_model_state is not None:
             self.load_state_dict(best_model_state['state_dict'])
             self.optimizer.load_state_dict(best_model_state['optimizer'])
             logger.info("Best model found at epoch %s with loss %.4f.", best_epoch, best_loss)
 
-        if self.summary_writer is not None:
-            self.summary_writer.close()
-
     def _train_step(self, epoch):
         """
         Perform a training step for the model.
 
         Returns
         -------
         float
@@ -254,20 +248,14 @@
             if batch.shape[0] < 4 and self.batch_normalization:
                 continue
             batch = self._impute_missing(batch, mask)
             self.optimizer.zero_grad()
             batch_loss = self._train_batch(batch)
             batch_loss.backward()
 
-            # After the backward pass, log the gradients and the parameters
-            if self.summary_writer is not None:
-                for name, param in self.model.named_parameters():
-                    self.summary_writer.add_histogram(f'{name}', param, epoch)
-                    self.summary_writer.add_histogram(f'{name}.grad', param.grad, epoch)
-
             self.optimizer.step()
             loss += batch_loss.item()
 
         # Calculate averge per batch loss and accuracy per epoch and print out what's happening
         loss /= len(self.data_loader)
         self.training_history["train_loss"].append(loss)
         return loss
```

### Comparing `irtorch-0.0.2/irtorch/estimation_algorithms/base_irt_algorithm.py` & `irtorch-0.0.3/irtorch/estimation_algorithms/base_irt_algorithm.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/estimation_algorithms/encoders/base_encoder.py` & `irtorch-0.0.3/irtorch/estimation_algorithms/encoders/base_encoder.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/estimation_algorithms/encoders/bounded_encoder.py` & `irtorch-0.0.3/irtorch/estimation_algorithms/encoders/bounded_encoder.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/estimation_algorithms/encoders/standard_encoder.py` & `irtorch-0.0.3/irtorch/estimation_algorithms/encoders/standard_encoder.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/estimation_algorithms/encoders/variational_encoder.py` & `irtorch-0.0.3/irtorch/estimation_algorithms/encoders/variational_encoder.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/estimation_algorithms/vaeirt.py` & `irtorch-0.0.3/irtorch/estimation_algorithms/vaeirt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import torch
 from torch.distributions import Normal
-from torch.utils.tensorboard import SummaryWriter
 from irtorch.models import BaseIRTModel
 from irtorch.estimation_algorithms.aeirt import AEIRT
 from irtorch.estimation_algorithms.encoders import BaseEncoder
 from irtorch.estimation_algorithms.encoders import VariationalEncoder
 from irtorch.utils import decode_one_hot_test_data
 
 logger = logging.getLogger('irtorch')
@@ -42,15 +41,14 @@
         one_hot_encoded: bool = False,
         hidden_layers_encoder: list[int] = None,
         nonlinear_encoder = torch.nn.ELU(),
         batch_normalization_encoder: bool = True,
         iw_samples: int = 1,
         anneal: bool = True,
         annealing_epochs: int = 5,
-        summary_writer: SummaryWriter = None,
     ):
         self.iw_samples = iw_samples
         self.annealing_epochs = annealing_epochs
         self.anneal = anneal
         self.annealing_factor = 1.0
 
         if encoder is not None:
@@ -73,15 +71,14 @@
                 if encoder is None
                 else encoder
             )
         super().__init__(
             model=model,
             encoder=encoder,
             one_hot_encoded=one_hot_encoded,
-            summary_writer=summary_writer,
         )
 
     def fit(
         self,
         train_data: torch.Tensor,
         validation_data: torch.Tensor = None,
         batch_size: int = 32,
```

### Comparing `irtorch-0.0.2/irtorch/irt.py` & `irtorch-0.0.3/irtorch/irt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import torch
 import pandas as pd
-from torch.utils.tensorboard import SummaryWriter
 from plotly import graph_objects as go
 from irtorch.models import BaseIRTModel
 from irtorch.models import Parametric
 from irtorch.models import MonotoneNN
 from irtorch.estimation_algorithms import AEIRT, VAEIRT
 from irtorch.irt_scorer import IRTScorer
 from irtorch.irt_plotter import IRTPlotter
@@ -79,15 +78,14 @@
         nominal_reference_category: bool = False,
         encoder: BaseEncoder = None,
         one_hot_encoded: bool = False,
         hidden_layers_decoder: list[int] = None,
         hidden_layers_encoder: list[int] = None,
         nonlinear_encoder = torch.nn.ELU(),
         batch_normalization_encoder: bool = True,
-        summary_writer: SummaryWriter = None,
     ):
         if isinstance(model, BaseIRTModel):
             self.latent_variables = model.latent_variables
             self.model = model
         else:
             if item_categories is None:
                 if data is None:
@@ -124,25 +122,23 @@
             self.algorithm = AEIRT(
                 model=self.model,
                 encoder=encoder,
                 one_hot_encoded=one_hot_encoded,
                 hidden_layers_encoder=hidden_layers_encoder,
                 nonlinear_encoder=nonlinear_encoder,
                 batch_normalization_encoder=batch_normalization_encoder,
-                summary_writer = summary_writer
             )
         elif estimation_algorithm == "VAE":
             self.algorithm = VAEIRT(
                 model=self.model,
                 encoder=encoder,
                 one_hot_encoded=one_hot_encoded,
                 hidden_layers_encoder=hidden_layers_encoder,
                 nonlinear_encoder=nonlinear_encoder,
                 batch_normalization_encoder=batch_normalization_encoder,
-                summary_writer = summary_writer
             )
 
         self.scorer = IRTScorer(self.model, self.algorithm)
         self.evaluator = IRTEvaluator(self.model, self.algorithm, self.scorer)
         self.plotter = IRTPlotter(self.model, self.algorithm, self.scorer, self.evaluator)
 
     def fit(
@@ -821,15 +817,15 @@
         ----------
         latent_density_method : str, optional
             Specifies the method used to approximate the latent space density.
             Possible options are
             - 'data' averages over the z scores from the population data.
             - 'encoder sampling' samples z scores from the encoder. Only available for VariationalAutoencoderIRT models
             - 'qmvn' for quantile multivariate normal approximation of a multivariate joint density function (QuantileMVNormal class).
-            - 'gmm' for an sklearn gaussian mixture model.
+            - 'gmm' for a gaussian mixture model.
 
         population_data : torch.Tensor, optional
             The population data used for approximating sum score probabilities. Default is None and uses the training data.
         trapezoidal_segments : int, optional
             The number of integration approximation intervals for each z dimension. (Default is 1000)
         sample_size : int, optional
             Sample size for the 'encoder sampling' method. (Default is 100000)
```

### Comparing `irtorch-0.0.2/irtorch/irt_evaluator.py` & `irtorch-0.0.3/irtorch/irt_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import torch
 from irtorch.models import BaseIRTModel
 from irtorch.estimation_algorithms import BaseIRTAlgorithm, VAEIRT
-from irtorch.irt_scorer import QuantileMVNormal, GaussianMixtureTorch
+from irtorch.quantile_mv_normal import QuantileMVNormal
+from irtorch.gaussian_mixture_model import GaussianMixtureModel
 from irtorch.irt_scorer import IRTScorer
 from irtorch._internal_utils import (
     impute_missing,
     conditional_score_distribution,
     sum_incorrect_probabilities,
 )
 
@@ -587,15 +588,15 @@
         ----------
         latent_density_method : str, optional
             Specifies the method used to approximate the latent space density.
             Possible options are
             - 'data' averages over the z scores from the population data.
             - 'encoder sampling' samples z scores from the encoder. Only available for VariationalAutoencoderIRT models
             - 'qmvn' for quantile multivariate normal approximation of a multivariate joint density function (QuantileMVNormal class).
-            - 'gmm' for an sklearn gaussian mixture model.
+            - 'gmm' for a gaussian mixture model.
         population_data : torch.Tensor, optional
             The population data used for approximating sum score probabilities. Default is None and uses the training data.
         trapezoidal_segments : int, optional
             The number of integration approximation intervals for each z dimension. (Default is 1000)
         sample_size : int, optional
             Sample size for the 'encoder sampling' method. (Default is 100000)
         Returns
@@ -689,15 +690,15 @@
         if population_data is not None or (
             (
                 latent_density_method != "qmvn"
                 or not isinstance(self.scorer.latent_density, QuantileMVNormal)
             )
             and (
                 latent_density_method != "gmm"
-                or not isinstance(self.scorer.latent_density, GaussianMixtureTorch)
+                or not isinstance(self.scorer.latent_density, GaussianMixtureModel)
             )
         ):
             self.scorer.approximate_latent_density(
                 z_scores=z_scores, approximation=latent_density_method
             )
 
         # get the min/max points for integration
```

### Comparing `irtorch-0.0.2/irtorch/irt_plotter.py` & `irtorch-0.0.3/irtorch/irt_plotter.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/irt_scorer.py` & `irtorch-0.0.3/irtorch/irt_scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import torch
 from torch.distributions import MultivariateNormal
 from irtorch.models.base_irt_model import BaseIRTModel
 from irtorch.estimation_algorithms.base_irt_algorithm import BaseIRTAlgorithm
 from irtorch.estimation_algorithms.aeirt import AEIRT
 from irtorch.quantile_mv_normal import QuantileMVNormal
-from irtorch.gaussian_mixture_torch import GaussianMixtureTorch
+from irtorch.gaussian_mixture_model import GaussianMixtureModel
 from irtorch._internal_utils import output_to_item_entropy, random_guessing_data, linear_regression, dynamic_print
 from irtorch.outlier_detector import OutlierDetector
 from irtorch.utils import one_hot_encode_test_data
 
 logger = logging.getLogger('irtorch')
 
 class IRTScorer:
@@ -30,46 +30,76 @@
 
 
     @torch.inference_mode()
     def approximate_latent_density(
         self,
         z_scores: torch.Tensor,
         approximation: str = "qmvn",
-        cv_n_components: list[int] = None,
-    ):
+        cv_n_components: list[int] = [2, 3, 4, 5, 10],
+    ) -> None:
         """
         Approximate the latent space density.
 
         Parameters
         ----------
         z_scores : torch.Tensor
             A 2D tensor with z scores. Each row represents one respondent, and each column an item.
         approximation : str, optional
             The approximation method to use. (default is 'qmvn')
             - 'qmvn' for quantile multivariate normal approximation of a multivariate joint density function (QuantileMVNormal class).
-            - 'gmm' for an sklearn gaussian mixture model.
+            - 'gmm' for a gaussian mixture model.
 
         cv_n_components: int, optional
-            The number of guassian components to use for 'gmm'. The best performing number . (default is 5)
+            The number of components to use for cross-validation in the Gaussian Mixture Model. (default is [2, 3, 4, 5, 10])
 
         Returns
         -------
         torch.Tensor
             A 2D tensor of latent scores, with latent variables as columns.
         """
         if approximation == "gmm":
             cv_n_components = [2, 3, 4, 5, 10] if cv_n_components is None else cv_n_components
-            self.latent_density = GaussianMixtureTorch()
-            self.latent_density.fit(z_scores, cv_n_components)
+            self.latent_density = self._cv_gaussian_mixture_model(z_scores, cv_n_components)
         elif approximation == "qmvn":
             self.latent_density = QuantileMVNormal()
             self.latent_density.fit(z_scores)
         else:
             raise ValueError("Invalid approximation method. Choose either 'qmvn' or 'gmm'.")
 
+    def _cv_gaussian_mixture_model(self, data: torch.Tensor, cv_n_components: list[int]) -> GaussianMixtureModel:
+        if len(cv_n_components) > 1:
+            logger.info("Performing cross-validation for Gaussian Mixture Model components...")
+            n_folds = 5
+            average_log_likelihood = torch.zeros(len(cv_n_components))
+            for comp_ind, components in enumerate(cv_n_components):
+                log_likelihoods = torch.zeros(n_folds)
+                data_chunks = data.chunk(n_folds)
+                for i, data_val in enumerate(data_chunks):
+                    train_chunks = [x for j, x in enumerate(data_chunks) if j != i]
+                    data_train = torch.cat(train_chunks, dim=0)
+
+                    gmm = GaussianMixtureModel(n_components=components, n_features=data.shape[1])
+                    gmm.fit(data_train)
+
+                    # Compute the log likelihood on the validation data
+                    log_likelihoods[i] = gmm(data_val)
+
+                # Compute the average log likelihood over the folds
+                average_log_likelihood[comp_ind] = log_likelihoods.mean()
+
+            # Select the number of components that maximizes the average log likelihood
+            optimal_n_components = cv_n_components[average_log_likelihood.argmax()]
+            logger.info("Fitting Gaussian Mixture Model for latent trait density.")
+            gmm = GaussianMixtureModel(n_components=optimal_n_components, n_features=data.shape[1])
+        else:
+            logger.info("Fitting Gaussian Mixture Model for latent trait density.")
+            gmm = GaussianMixtureModel(n_components=cv_n_components[0], n_features=data.shape[1])
+
+        gmm.fit(data)
+        return gmm
 
     @torch.inference_mode()
     def min_max_z_for_integration(
         self,
         z: torch.Tensor = None,
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """
```

### Comparing `irtorch-0.0.2/irtorch/latent_variable_functions.py` & `irtorch-0.0.3/irtorch/latent_variable_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/layers.py` & `irtorch-0.0.3/irtorch/layers.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/load_dataset.py` & `irtorch-0.0.3/irtorch/load_dataset.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/models/base_irt_model.py` & `irtorch-0.0.3/irtorch/models/base_irt_model.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/models/monotone_nn.py` & `irtorch-0.0.3/irtorch/models/monotone_nn.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/models/parametric.py` & `irtorch-0.0.3/irtorch/models/parametric.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/outlier_detector.py` & `irtorch-0.0.3/irtorch/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/quantile_mv_normal.py` & `irtorch-0.0.3/irtorch/quantile_mv_normal.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/timer.py` & `irtorch-0.0.3/irtorch/timer.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch/utils.py` & `irtorch-0.0.3/irtorch/utils.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/irtorch.egg-info/PKG-INFO` & `irtorch-0.0.3/irtorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irtorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: IRTorch: An item response theory package for python.
 Home-page: https://github.com/joakimwallmark/irtorch
 Author: Joakim Wallmark
 Author-email: wallmark.joakim@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `irtorch-0.0.2/irtorch.egg-info/SOURCES.txt` & `irtorch-0.0.3/irtorch.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 README.md
 setup.py
 irtorch/__init__.py
 irtorch/_internal_utils.py
 irtorch/activation_functions.py
 irtorch/config.py
 irtorch/cross_validation.py
-irtorch/gaussian_mixture_torch.py
+irtorch/gaussian_mixture_model.py
 irtorch/irt.py
 irtorch/irt_evaluator.py
 irtorch/irt_plotter.py
 irtorch/irt_scorer.py
 irtorch/latent_variable_functions.py
 irtorch/layers.py
 irtorch/load_dataset.py
@@ -23,14 +23,18 @@
 irtorch.egg-info/dependency_links.txt
 irtorch.egg-info/not-zip-safe
 irtorch.egg-info/requires.txt
 irtorch.egg-info/top_level.txt
 irtorch/datasets/big_five/big_five.pt
 irtorch/datasets/national_mathematics/mathematics_1.pt
 irtorch/datasets/national_mathematics/mathematics_2.pt
+irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt
+irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt
+irtorch/datasets/swedish_sat/swesat22b_quant_correct.txt
+irtorch/datasets/swedish_sat/swesat22b_verb_correct.txt
 irtorch/estimation_algorithms/__init__.py
 irtorch/estimation_algorithms/aeirt.py
 irtorch/estimation_algorithms/base_irt_algorithm.py
 irtorch/estimation_algorithms/vaeirt.py
 irtorch/estimation_algorithms/encoders/__init__.py
 irtorch/estimation_algorithms/encoders/base_encoder.py
 irtorch/estimation_algorithms/encoders/bounded_encoder.py
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_activation_functions.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_activation_functions.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -48,23 +48,23 @@
      4          60 LOAD_CONST               0 (0)
                 62 LOAD_CONST               3 (('BoundedELU',))
                 64 IMPORT_NAME             11 (irtorch.activation_functions)
                 66 IMPORT_FROM             12 (BoundedELU)
                 68 STORE_NAME              12 (BoundedELU)
                 70 POP_TOP
    
-     6          72 LOAD_CONST               4 (<code object test_BoundedELU_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_activation_functions.py", line 6>)
+     6          72 LOAD_CONST               4 (<code object test_BoundedELU_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_activation_functions.py", line 6>)
                 74 MAKE_FUNCTION            0
                 76 STORE_NAME              13 (test_BoundedELU_forward)
    
-    14          78 LOAD_CONST               5 (<code object test_BoundedELU_backward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_activation_functions.py", line 14>)
+    14          78 LOAD_CONST               5 (<code object test_BoundedELU_backward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_activation_functions.py", line 14>)
                 80 MAKE_FUNCTION            0
                 82 STORE_NAME              14 (test_BoundedELU_backward)
    
-    20          84 LOAD_CONST               6 (<code object test_BoundedELU_backward_double_backward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_activation_functions.py", line 20>)
+    20          84 LOAD_CONST               6 (<code object test_BoundedELU_backward_double_backward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_activation_functions.py", line 20>)
                 86 MAKE_FUNCTION            0
                 88 STORE_NAME              15 (test_BoundedELU_backward_double_backward)
                 90 LOAD_CONST               1 (None)
                 92 RETURN_VALUE
    consts
       0
       None
@@ -260,15 +260,15 @@
             'result'
             'expected'
             ('py0', 'py2', 'py3', 'py4', 'py6')
          names      ('torch', 'tensor', 'BoundedELU', 'apply', 'allclose', '@pytest_ar', '_format_assertmsg', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('input', 'alpha', 'result', 'expected', '@py_assert1', '@py_assert5', '@py_format7')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_activation_functions.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_activation_functions.py'
          name       'test_BoundedELU_forward'
          firstlineno 6
          lnotab 0x0202300104012a013001
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 8
@@ -423,15 +423,15 @@
             'gradcheck'
             'BoundedELU'
             ('py0', 'py1', 'py3', 'py5', 'py7')
          names      ('torch', 'randn', 'double', 'BoundedELU', 'apply', 'gradcheck', '@pytest_ar', '_format_assertmsg', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('input', 'alpha', '@py_assert2', '@py_assert4', '@py_assert6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_activation_functions.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_activation_functions.py'
          name       'test_BoundedELU_backward'
          firstlineno 14
          lnotab 0x020242010401
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 8
@@ -586,19 +586,19 @@
             'gradgradcheck'
             'BoundedELU'
             ('py0', 'py1', 'py3', 'py5', 'py7')
          names      ('torch', 'randn', 'double', 'BoundedELU', 'apply', 'gradgradcheck', '@pytest_ar', '_format_assertmsg', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('input', 'alpha', '@py_assert2', '@py_assert4', '@py_assert6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_activation_functions.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_activation_functions.py'
          name       'test_BoundedELU_backward_double_backward'
          firstlineno 20
          lnotab 0x020342010401
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'torch.autograd', 'gradcheck', 'gradgradcheck', 'irtorch.activation_functions', 'BoundedELU', 'test_BoundedELU_forward', 'test_BoundedELU_backward', 'test_BoundedELU_backward_double_backward')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_activation_functions.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_activation_functions.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02012201080110010c0206080606
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_aeirt.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_aeirt.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -63,15 +63,15 @@
                 84 IMPORT_NAME             14 (irtorch.models)
                 86 IMPORT_FROM             15 (MonotoneNN)
                 88 STORE_NAME              15 (MonotoneNN)
                 90 POP_TOP
    
     13          92 PUSH_NULL
                 94 LOAD_BUILD_CLASS
-                96 LOAD_CONST               6 (<code object TestAEIRT, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_aeirt.py", line 13>)
+                96 LOAD_CONST               6 (<code object TestAEIRT, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_aeirt.py", line 13>)
                 98 MAKE_FUNCTION            0
                100 LOAD_CONST               7 ('TestAEIRT')
                102 PRECALL                  2
                106 CALL                     2
                116 STORE_NAME              16 (TestAEIRT)
                118 LOAD_CONST               1 (None)
                120 RETURN_VALUE
@@ -101,61 +101,61 @@
          
           14          10 PUSH_NULL
                       12 LOAD_NAME                3 (pytest)
                       14 LOAD_ATTR                4 (fixture)
                       24 PRECALL                  0
                       28 CALL                     0
          
-          15          38 LOAD_CONST               1 (<code object algorithm, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_aeirt.py", line 14>)
+          15          38 LOAD_CONST               1 (<code object algorithm, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_aeirt.py", line 14>)
                       40 MAKE_FUNCTION            0
          
           14          42 PRECALL                  0
                       46 CALL                     0
          
           15          56 STORE_NAME               5 (algorithm)
          
           37          58 LOAD_CONST               2 ('algorithm')
                       60 LOAD_NAME                6 (AEIRT)
                       62 BUILD_TUPLE              2
-                      64 LOAD_CONST               3 (<code object test_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_aeirt.py", line 37>)
+                      64 LOAD_CONST               3 (<code object test_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_aeirt.py", line 37>)
                       66 MAKE_FUNCTION            4 (annotations)
                       68 STORE_NAME               7 (test_forward)
          
           41          70 LOAD_CONST               2 ('algorithm')
                       72 LOAD_NAME                6 (AEIRT)
                       74 BUILD_TUPLE              2
-                      76 LOAD_CONST               4 (<code object test_latent_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_aeirt.py", line 41>)
+                      76 LOAD_CONST               4 (<code object test_latent_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_aeirt.py", line 41>)
                       78 MAKE_FUNCTION            4 (annotations)
                       80 STORE_NAME               8 (test_latent_scores)
          
           45          82 LOAD_CONST               2 ('algorithm')
                       84 LOAD_NAME                6 (AEIRT)
                       86 BUILD_TUPLE              2
-                      88 LOAD_CONST               5 (<code object test__train_step, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_aeirt.py", line 45>)
+                      88 LOAD_CONST               5 (<code object test__train_step, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_aeirt.py", line 45>)
                       90 MAKE_FUNCTION            4 (annotations)
                       92 STORE_NAME               9 (test__train_step)
          
           52          94 LOAD_CONST               2 ('algorithm')
                       96 LOAD_NAME                6 (AEIRT)
                       98 BUILD_TUPLE              2
-                     100 LOAD_CONST               6 (<code object test__validation_step, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_aeirt.py", line 52>)
+                     100 LOAD_CONST               6 (<code object test__validation_step, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_aeirt.py", line 52>)
                      102 MAKE_FUNCTION            4 (annotations)
                      104 STORE_NAME              10 (test__validation_step)
          
           57         106 LOAD_CONST               2 ('algorithm')
                      108 LOAD_NAME                6 (AEIRT)
                      110 BUILD_TUPLE              2
-                     112 LOAD_CONST               7 (<code object test__impute_missing_zero, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_aeirt.py", line 57>)
+                     112 LOAD_CONST               7 (<code object test__impute_missing_zero, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_aeirt.py", line 57>)
                      114 MAKE_FUNCTION            4 (annotations)
                      116 STORE_NAME              11 (test__impute_missing_zero)
          
           89         118 LOAD_CONST               2 ('algorithm')
                      120 LOAD_NAME                6 (AEIRT)
                      122 BUILD_TUPLE              2
-                     124 LOAD_CONST               8 (<code object test_fit, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_aeirt.py", line 89>)
+                     124 LOAD_CONST               8 (<code object test_fit, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_aeirt.py", line 89>)
                      126 MAKE_FUNCTION            4 (annotations)
                      128 STORE_NAME              12 (test_fit)
                      130 LOAD_CONST               9 (None)
                      132 RETURN_VALUE
          consts
             'TestAEIRT'
             code
@@ -255,15 +255,15 @@
                   20
                   ('model', 'hidden_layers_encoder', 'nonlinear_encoder')
                   'zero'
                names      ('torch', 'cuda', 'is_available', 'pytest', 'skip', 'MonotoneNN', 'AEIRT', 'nn', 'ELU', 'imputation_method', 'data_loader', 'validation_data_loader', 'initialize_fit')
                varnames   ('self', 'device', 'latent_variables', 'item_categories', 'data_loaders', 'model', 'algorithm')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
                name       'algorithm'
                firstlineno 14
                lnotab
                   0x0202480128020c010201020104fd12050c01020104013afd12060e021e
                   021e01
             'algorithm'
             code
@@ -394,15 +394,15 @@
                   ('py0', 'py2', 'py5')
                   'assert %(py7)s'
                   'py7'
                names      ('forward', 'shape', 'model', 'max_item_responses', 'items', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
                varnames   ('self', 'algorithm', 'test_data', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
                name       'test_forward'
                firstlineno 37
                lnotab 0x02012a01
             code
                argcount  : 3
                nlocals   : 9
                stacksize : 8
@@ -539,15 +539,15 @@
                   ('py0', 'py2', 'py5')
                   'assert %(py7)s'
                   'py7'
                names      ('z_scores', 'to', 'next', 'parameters', 'device', 'shape', 'model', 'latent_variables', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
                varnames   ('self', 'algorithm', 'test_data', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
                name       'test_latent_scores'
                firstlineno 41
                lnotab 0x02019801
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 8
@@ -690,15 +690,15 @@
                   ('py0', 'py2')
                   'assert %(py4)s'
                   'py4'
                names      ('float', 'range', '_train_step', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
                varnames   ('self', 'algorithm', 'previous_loss', 'epoch', 'loss', '@py_assert1', '@py_format3', '@py_format5')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
                name       'test__train_step'
                firstlineno 45
                lnotab 0x02011e0122012a01ff00990106fd
             code
                argcount  : 2
                nlocals   : 9
                stacksize : 7
@@ -917,15 +917,15 @@
                   ('py0', 'py3')
                   'assert %(py5)s'
                   'py5'
                names      ('_validation_step', 'isinstance', 'float', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', '_call_reprcompare')
                varnames   ('self', 'algorithm', 'log_likelihood', '@py_assert3', '@py_format5', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
                name       'test__validation_step'
                firstlineno 52
                lnotab 0x02012801ff00ff004601
             code
                argcount  : 2
                nlocals   : 15
                stacksize : 11
@@ -1374,15 +1374,15 @@
                   'assert %(py6)s\n{%(py6)s = %(py2)s\n{%(py2)s = %(py0)s.equal\n}(%(py3)s, %(py4)s)\n}'
                   'data'
                   ('py0', 'py2', 'py3', 'py4', 'py6')
                names      ('torch', 'full', 'tensor', 'imputation_method', '_impute_missing', 'equal', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
                varnames   ('self', 'algorithm', 'a', 'b', 'data', 'no_missing_mask', 'missing_mask', 'imputed_data', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_format13', '@py_format7')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
                name       'test__impute_missing_zero'
                firstlineno 57
                lnotab
                   0x02010a012e012e011602060106010601060106fb02ff100a0e012c010c
                   0b0af50e0b0af5680b0af51e0b0af5280b0af52a0b0af51e0b0af51e0b0a
                   f51e0b0af5220b0af51e0b0af5280b0af52a0b0af51c0b0af51c0b0af51c
                   0b0af5320b0af5340c2c01
@@ -1713,31 +1713,31 @@
                   'assert %(py7)s'
                   'py7'
                   'mocked_validation_step'
                names      ('patch', 'object', 'torch', 'tensor', 'fit', 'call_count', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
                varnames   ('self', 'algorithm', 'test_data', 'mocked_train_step', 'mocked_validation_step', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
                name       'test_fit'
                firstlineno 89
                lnotab
                   0x020216012aff120218012aff10fe0204020218011201120102fd1207ff
                   008301ff0083f2
             None
          names      ('__name__', '__module__', '__qualname__', 'pytest', 'fixture', 'algorithm', 'AEIRT', 'test_forward', 'test_latent_scores', 'test__train_step', 'test__validation_step', 'test__impute_missing_zero', 'test_fit')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
          name       'TestAEIRT'
          firstlineno 13
          lnotab 0x0a011c0104ff0e0102160c040c040c070c050c20
       'TestAEIRT'
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'unittest.mock', 'patch', 'utils', 'initialize_fit', 'torch', 'irtorch.estimation_algorithms', 'AEIRT', 'irtorch.models', 'MonotoneNN', 'TestAEIRT')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_aeirt.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_aeirt.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020122010c010c0108010c010c07
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_base_irt_model.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_base_irt_model.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -60,51 +60,51 @@
                 76 STORE_NAME              13 (MagicMock)
                 78 IMPORT_FROM             14 (patch)
                 80 STORE_NAME              14 (patch)
                 82 POP_TOP
    
      7          84 PUSH_NULL
                 86 LOAD_BUILD_CLASS
-                88 LOAD_CONST               5 (<code object ConcreteIRTModel, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 7>)
+                88 LOAD_CONST               5 (<code object ConcreteIRTModel, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 7>)
                 90 MAKE_FUNCTION            0
                 92 LOAD_CONST               6 ('ConcreteIRTModel')
                 94 LOAD_NAME               11 (BaseIRTModel)
                 96 PRECALL                  3
                100 CALL                     3
                110 STORE_NAME              15 (ConcreteIRTModel)
    
     17         112 LOAD_NAME                6 (pytest)
                114 LOAD_ATTR               16 (fixture)
    
-    18         124 LOAD_CONST               7 (<code object base_irt_model, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 17>)
+    18         124 LOAD_CONST               7 (<code object base_irt_model, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 17>)
                126 MAKE_FUNCTION            0
    
     17         128 PRECALL                  0
                132 CALL                     0
    
     18         142 STORE_NAME              17 (base_irt_model)
    
     22         144 LOAD_CONST               8 ('base_irt_model')
                146 LOAD_NAME               11 (BaseIRTModel)
                148 BUILD_TUPLE              2
-               150 LOAD_CONST               9 (<code object test_expected_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 22>)
+               150 LOAD_CONST               9 (<code object test_expected_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 22>)
                152 MAKE_FUNCTION            4 (annotations)
                154 STORE_NAME              18 (test_expected_scores)
    
     74         156 LOAD_CONST               8 ('base_irt_model')
                158 LOAD_NAME               11 (BaseIRTModel)
                160 BUILD_TUPLE              2
-               162 LOAD_CONST              10 (<code object test_probability_gradients, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 74>)
+               162 LOAD_CONST              10 (<code object test_probability_gradients, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 74>)
                164 MAKE_FUNCTION            4 (annotations)
                166 STORE_NAME              19 (test_probability_gradients)
    
     90         168 LOAD_CONST               8 ('base_irt_model')
                170 LOAD_NAME               11 (BaseIRTModel)
                172 BUILD_TUPLE              2
-               174 LOAD_CONST              11 (<code object test_sample_test_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 90>)
+               174 LOAD_CONST              11 (<code object test_sample_test_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 90>)
                176 MAKE_FUNCTION            4 (annotations)
                178 STORE_NAME              20 (test_sample_test_data)
                180 LOAD_CONST               1 (None)
                182 RETURN_VALUE
    consts
       0
       None
@@ -124,23 +124,23 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ConcreteIRTModel')
                        8 STORE_NAME               2 (__qualname__)
          
            8          10 LOAD_CONST               1 ('\n    Concrete implementation of BaseIRTModel for testing purposes.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          11          14 LOAD_CONST               2 (<code object forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 11>)
+          11          14 LOAD_CONST               2 (<code object forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 11>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (forward)
          
           14          20 LOAD_CONST               3 ('output')
                       22 LOAD_NAME                5 (torch)
                       24 LOAD_ATTR                6 (Tensor)
                       34 BUILD_TUPLE              2
-                      36 LOAD_CONST               4 (<code object probabilities_from_output, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 14>)
+                      36 LOAD_CONST               4 (<code object probabilities_from_output, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 14>)
                       38 MAKE_FUNCTION            4 (annotations)
                       40 STORE_NAME               7 (probabilities_from_output)
                       42 LOAD_CONST               5 (None)
                       44 RETURN_VALUE
          consts
             'ConcreteIRTModel'
             '\n    Concrete implementation of BaseIRTModel for testing purposes.\n    '
@@ -156,15 +156,15 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'z')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
                name       'forward'
                firstlineno 11
                lnotab 0x0201
             'output'
             code
                argcount  : 2
                nlocals   : 2
@@ -177,24 +177,24 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'output')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
                name       'probabilities_from_output'
                firstlineno 14
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'forward', 'torch', 'Tensor', 'probabilities_from_output')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
          name       'ConcreteIRTModel'
          firstlineno 7
          lnotab 0x0a0104030603
       'ConcreteIRTModel'
       code
          argcount  : 1
          nlocals   : 1
@@ -217,15 +217,15 @@
             None
             3
             4
          names      ('ConcreteIRTModel',)
          varnames   ('latent_variables',)
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
          name       'base_irt_model'
          firstlineno 17
          lnotab 0x0202
       'base_irt_model'
       code
          argcount  : 1
          nlocals   : 20
@@ -617,15 +617,15 @@
             0000007413000000000000000000006a0b00000000000000007c07a60100
             00ab010000000000000000640d9c087a0600007d08741900000000000000
             0000007413000000000000000000006a0d00000000000000007c08a60100
             00ab010000000000000000a6010000ab0100000000000000008201640078
             017d0378017d0478017d0578017d067d0764005300
           22            0 RESUME                   0
          
-          24            2 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 24>)
+          24            2 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 24>)
                         4 MAKE_FUNCTION            0
                         6 STORE_FAST               1 (item_probabilities_mock)
          
           29            8 LOAD_GLOBAL              1 (NULL + MagicMock)
          
           30           20 LOAD_FAST                1 (item_probabilities_mock)
          
@@ -2151,15 +2151,15 @@
                      8772 STORE_FAST              14 (@py_assert18)
                      8774 COPY                     1
                      8776 STORE_FAST              15 (@py_assert20)
                      8778 COPY                     1
                      8780 STORE_FAST              16 (@py_assert22)
                      8782 STORE_FAST              17 (@py_assert24)
          
-          55         8784 LOAD_CONST              28 (<code object item_probabilities_mock2, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 55>)
+          55         8784 LOAD_CONST              28 (<code object item_probabilities_mock2, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 55>)
                      8786 MAKE_FUNCTION            0
                      8788 STORE_FAST              19 (item_probabilities_mock2)
          
           58         8790 LOAD_GLOBAL              1 (NULL + MagicMock)
          
           59         8802 LOAD_FAST               19 (item_probabilities_mock2)
          
@@ -2688,15 +2688,15 @@
                   (0.1, 0.1, 0.1, 0.7)
                   (0.3, 0.3, 0.4, 0.0)
                   (0.3, 0.5, 0.1, 0.1)
                names      ('torch', 'tensor')
                varnames   ('args', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
                name       'item_probabilities_mock'
                firstlineno 24
                lnotab 0x020116010e010efe
             ('side_effect',)
             (2, 2)
             True
             ('return_item_scores',)
@@ -2749,27 +2749,27 @@
                   None
                   (0.1, 0.1, 0.8, 0.0)
                   (0.1, 0.1, 0.2, 0.7)
                names      ('torch', 'tensor')
                varnames   ('args', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
                name       'item_probabilities_mock2'
                firstlineno 55
                lnotab 0x0201
             (1, 2)
             2.6
             3
             1.6
          names      ('MagicMock', 'item_probabilities', 'expected_scores', 'torch', 'randn', 'allclose', 'tensor', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'sum', 'model_missing', 'mc_correct')
          varnames   ('base_irt_model', 'item_probabilities_mock', 'expected_item_scores', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_format13', '@py_assert4', '@py_assert6', '@py_assert8', '@py_assert14', '@py_assert16', '@py_assert18', '@py_assert20', '@py_assert22', '@py_assert24', '@py_format26', 'item_probabilities_mock2')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
          name       'test_expected_scores'
          firstlineno 22
          lnotab
             0x020206050c0102ff1c045201ff00ff00ff003301ff00ff00ff00ff00f6
             020e015201ff00ff00ff003301ff00ff00ff00ff00f6020e0112015201ff
             00ff00ff003301ff00ff00ff00ff00f6020e0112015201ff00ff00ff0033
             01ff00ff00ff00ff00f60306030c0102ff1c030e010e015201ff00ff00ff
@@ -2797,15 +2797,15 @@
             05a6010000ab010000000000000000640b9c037a0600007d07640c640d7c
             0769017a0600007d08741900000000000000000000740d00000000000000
             0000006a0d00000000000000007c08a6010000ab010000000000000000a6
             010000ab0100000000000000008201640078017d0478017d067d05640053
             00
           74           0 RESUME                   0
          
-          76           2 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 76>)
+          76           2 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 76>)
                        4 MAKE_FUNCTION            0
                        6 STORE_FAST               1 (item_probabilities_mock)
          
           81           8 LOAD_GLOBAL              1 (NULL + MagicMock)
          
           82          20 LOAD_FAST                1 (item_probabilities_mock)
          
@@ -2999,15 +2999,15 @@
                   -1
                   0
                   3
                names      ('torch', 'tensor', 'expand', 'sum', 'reshape', 'inf', 'softmax')
                varnames   ('z', 'logits')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
                name       'item_probabilities_mock'
                firstlineno 76
                lnotab 0x0201b8012a01
             ('side_effect',)
             -2.0
             -3.0
             1.0
@@ -3019,15 +3019,15 @@
             ('py0', 'py2', 'py5')
             'assert %(py7)s'
             'py7'
          names      ('MagicMock', 'item_probabilities', 'torch', 'tensor', 'probability_gradients', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('base_irt_model', 'item_probabilities_mock', 'input_z', 'prob_gradients', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
          name       'test_probability_gradients'
          firstlineno 74
          lnotab 0x020206050c0102ff1c043a012a02
       code
          argcount  : 1
          nlocals   : 16
          stacksize : 8
@@ -3101,15 +3101,15 @@
             007c0da6010000ab01000000000000000064169c057a0600007d0f741900
             000000000000000000740d000000000000000000006a0d00000000000000
             007c0fa6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d0478017d0978017d0578017d0b78017d0a78017d0c7d
             0d64005300
           90           0 RESUME                   0
          
-          92           2 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_base_irt_model.py", line 92>)
+          92           2 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_base_irt_model.py", line 92>)
                        4 MAKE_FUNCTION            0
                        6 STORE_FAST               1 (item_probabilities_mock)
          
           97           8 LOAD_GLOBAL              1 (NULL + MagicMock)
                       20 LOAD_FAST                1 (item_probabilities_mock)
                       22 KW_NAMES                 2
                       24 PRECALL                  1
@@ -3541,15 +3541,15 @@
                   (0.1, 0.1, 0.1, 0.7)
                   (0.3, 0.3, 0.4, 0.0)
                   (0.3, 0.5, 0.1, 0.1)
                names      ('torch', 'tensor')
                varnames   ('args', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
                name       'item_probabilities_mock'
                firstlineno 92
                lnotab 0x020116010e010efe
             ('side_effect',)
             (2, 2)
             ('==',)
             ('%(py2)s\n{%(py2)s = %(py0)s.shape\n} == %(py6)s\n{%(py6)s = %(py4)s.shape\n}',)
@@ -3570,19 +3570,19 @@
             ('py9', 'py12')
             'assert %(py17)s\n{%(py17)s = %(py2)s\n{%(py2)s = %(py0)s.all\n}((%(py8)s & %(py14)s))\n}'
             ('py0', 'py2', 'py8', 'py14', 'py17')
          names      ('MagicMock', 'item_probabilities', 'torch', 'randn', 'sample_test_data', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'dtype', 'float32', 'all')
          varnames   ('base_irt_model', 'item_probabilities_mock', 'z', 'sampled_data', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_assert11', '@py_assert10', '@py_assert15', '@py_assert16', '@py_format13', '@py_format18')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
          name       'test_sample_test_data'
          firstlineno 90
          lnotab 0x020206052a0328012a03ff00ff000a01ff00ff002803
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'torch.nn.functional', 'softmax', 'irtorch.models', 'BaseIRTModel', 'unittest.mock', 'MagicMock', 'patch', 'ConcreteIRTModel', 'fixture', 'base_irt_model', 'test_expected_scores', 'test_probability_gradients', 'test_sample_test_data')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_base_irt_model.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_base_irt_model.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201220108010c010c0110021c0a0c0104ff0e0102040c340c10
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_config.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_config.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -32,15 +32,15 @@
      2          36 LOAD_CONST               0 (0)
                 38 LOAD_CONST               2 (('set_verbosity',))
                 40 IMPORT_NAME              7 (irtorch.config)
                 42 IMPORT_FROM              8 (set_verbosity)
                 44 STORE_NAME               8 (set_verbosity)
                 46 POP_TOP
    
-     4          48 LOAD_CONST               3 (<code object test_set_verbosity, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_config.py", line 4>)
+     4          48 LOAD_CONST               3 (<code object test_set_verbosity, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_config.py", line 4>)
                 50 MAKE_FUNCTION            0
                 52 STORE_NAME               9 (test_set_verbosity)
                 54 LOAD_CONST               1 (None)
                 56 RETURN_VALUE
    consts
       0
       None
@@ -1127,22 +1127,22 @@
             ('py0', 'py1', 'py3', 'py6')
             'assert %(py8)s'
             'py8'
          names      ('set_verbosity', 'logging', 'getLogger', 'getEffectiveLevel', 'CRITICAL', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'ValueError', 'str')
          varnames   ('@py_assert1', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert13', '@py_assert11', '@py_format15', '@py_format17', 'e', '@py_assert2', '@py_assert4', '@py_format7', '@py_format9')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_config.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_config.py'
          name       'test_set_verbosity'
          firstlineno 4
          lnotab
             0x02021e01ff00ff00ff002d031e01ff00ff00ff002d031e01ff00ff00ff
             002d031e01ff00ff00ff002d031e01ff00ff00ff002d03020124011401ff
             00ff0038ff
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'logging', 'irtorch.config', 'set_verbosity', 'test_set_verbosity')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_config.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_config.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020122010c02
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_internal_utils.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_internal_utils.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -71,55 +71,55 @@
                 98 LOAD_NAME                6 (pytest)
                100 LOAD_ATTR               20 (fixture)
                110 LOAD_CONST               3 ('module')
                112 KW_NAMES                 4
                114 PRECALL                  1
                118 CALL                     1
    
-    17         128 LOAD_CONST               5 (<code object logits, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 16>)
+    17         128 LOAD_CONST               5 (<code object logits, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 16>)
                130 MAKE_FUNCTION            0
    
     16         132 PRECALL                  0
                136 CALL                     0
    
     17         146 STORE_NAME              21 (logits)
    
-    60         148 LOAD_CONST               6 (<code object test_is_jupyter, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 60>)
+    60         148 LOAD_CONST               6 (<code object test_is_jupyter, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 60>)
                150 MAKE_FUNCTION            0
                152 STORE_NAME              22 (test_is_jupyter)
    
-    63         154 LOAD_CONST               7 (<code object testdynamic_print, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 63>)
+    63         154 LOAD_CONST               7 (<code object testdynamic_print, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 63>)
                156 MAKE_FUNCTION            0
                158 STORE_NAME              23 (testdynamic_print)
    
-    75         160 LOAD_CONST               8 (<code object test_linear_regression, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 75>)
+    75         160 LOAD_CONST               8 (<code object test_linear_regression, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 75>)
                162 MAKE_FUNCTION            0
                164 STORE_NAME              24 (test_linear_regression)
    
-    86         166 LOAD_CONST               9 (<code object test_conditional_scores_distribution, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 86>)
+    86         166 LOAD_CONST               9 (<code object test_conditional_scores_distribution, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 86>)
                168 MAKE_FUNCTION            0
                170 STORE_NAME              25 (test_conditional_scores_distribution)
    
-   121         172 LOAD_CONST              10 (<code object test_sum_incorrect_probabilities, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 121>)
+   121         172 LOAD_CONST              10 (<code object test_sum_incorrect_probabilities, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 121>)
                174 MAKE_FUNCTION            0
                176 STORE_NAME              26 (test_sum_incorrect_probabilities)
    
-   162         178 LOAD_CONST              11 (<code object test_entropy, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 162>)
+   162         178 LOAD_CONST              11 (<code object test_entropy, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 162>)
                180 MAKE_FUNCTION            0
                182 STORE_NAME              27 (test_entropy)
    
-   184         184 LOAD_CONST              12 (<code object test_output_to_item_entropy, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 184>)
+   184         184 LOAD_CONST              12 (<code object test_output_to_item_entropy, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 184>)
                186 MAKE_FUNCTION            0
                188 STORE_NAME              28 (test_output_to_item_entropy)
    
-   195         190 LOAD_CONST              13 (<code object test_impute_missing, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 195>)
+   195         190 LOAD_CONST              13 (<code object test_impute_missing, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 195>)
                192 MAKE_FUNCTION            0
                194 STORE_NAME              29 (test_impute_missing)
    
-   212         196 LOAD_CONST              14 (<code object test_random_guessing_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 212>)
+   212         196 LOAD_CONST              14 (<code object test_random_guessing_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 212>)
                198 MAKE_FUNCTION            0
                200 STORE_NAME              30 (test_random_guessing_data)
                202 LOAD_CONST               1 (None)
                204 RETURN_VALUE
    consts
       0
       None
@@ -164,15 +164,15 @@
             None
             (-0.2168, 0.0781, -0.0588, 0.1306, 0.1659, 0.1068, -0.3093, 0.0875, -0.1423, -0.0832, 0.319, -0.0511, 0.1717, -0.1309, 0.3678, 0.3022)
             (-0.2116, 0.0789, -0.0464, 0.1117, 0.1522, 0.1322, -0.3207, 0.0925, -0.1325, -0.0844, 0.3234, -0.0261, 0.1774, -0.1098, 0.345, 0.3082)
          names      ('torch', 'tensor', 'to')
          varnames   ('device',)
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'logits'
          firstlineno 16
          lnotab 0x02021602061206ed02ff0e2726d9
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 7
@@ -284,15 +284,15 @@
             ('py0', 'py2', 'py5')
             'assert %(py7)s'
             'py7'
          names      ('is_jupyter', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'test_is_jupyter'
          firstlineno 60
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
@@ -524,15 +524,15 @@
             'py7'
             'Hello World!'
             '\rHello World! '
          names      ('dynamic_print', 'readouterr', 'out', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('capsys', 'captured_output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'testdynamic_print'
          firstlineno 63
          lnotab 0x02011e032801ff0083021e012802
       code
          argcount  : 0
          nlocals   : 13
          stacksize : 11
@@ -1107,15 +1107,15 @@
             ('py1', 'py3', 'py5', 'py7', 'py9', 'py11', 'py13', 'py15')
             'assert %(py17)s'
             'py17'
          names      ('torch', 'tensor', 'float32', 'reshape', 'linear_regression', 'item', 'pytest', 'approx', '@pytest_ar', '_call_reprcompare', '_saferepr', '@py_builtins', 'locals', '_should_repr_global_name', 'AssertionError', '_format_explanation')
          varnames   ('x', 'y', 'coefficients', '@py_assert0', '@py_assert2', '@py_assert4', '@py_assert8', '@py_assert10', '@py_assert12', '@py_assert14', '@py_assert6', '@py_format16', '@py_format18')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'test_linear_regression'
          firstlineno 75
          lnotab 0x020158016c032002ff00ff00c601ff00ff00c601
       code
          argcount  : 0
          nlocals   : 10
          stacksize : 9
@@ -1536,15 +1536,15 @@
             (0.28, 0.47, 0.22, 0.03)
             (0.336, 0.452, 0.188, 0.024)
             'expected_output_mc_correct'
          names      ('torch', 'tensor', 'conditional_score_distribution', 'allclose', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'sum_incorrect_probabilities', 'len')
          varnames   ('probabilities', 'item_categories', 'result', 'expected_output', '@py_assert1', '@py_assert5', '@py_assert7', '@py_format9', 'mc_correct', 'expected_output_mc_correct')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'test_conditional_scores_distribution'
          firstlineno 86
          lnotab
             0x02011601140114fe1204080320031602060106fe02ff1007ff00ff0094
             0308010c0108ff10032601200216010eff1004
       code
          argcount  : 0
@@ -1810,15 +1810,15 @@
          
          146         874 LOAD_GLOBAL              5 (NULL + sum_incorrect_probabilities)
          
          147         886 LOAD_FAST                0 (probabilities)
          
          148         888 LOAD_FAST                1 (item_categories)
          
-         149         890 LOAD_CONST              25 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_internal_utils.py", line 149>)
+         149         890 LOAD_CONST              25 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_internal_utils.py", line 149>)
                      892 MAKE_FUNCTION            0
                      894 LOAD_FAST                2 (mc_correct)
                      896 GET_ITER
                      898 PRECALL                  0
                      902 CALL                     0
          
          150         912 LOAD_CONST              26 (True)
@@ -2017,24 +2017,24 @@
                        >>   22 RETURN_VALUE
                consts
                   1
                names      ()
                varnames   ('.0', 'x')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
                name       '<listcomp>'
                firstlineno 149
                lnotab 0x
             True
          names      ('torch', 'tensor', 'sum_incorrect_probabilities', 'allclose', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('probabilities', 'item_categories', 'mc_correct', 'result', 'expected_output', '@py_assert1', '@py_assert5', '@py_assert7', '@py_format9')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'test_sum_incorrect_probabilities'
          firstlineno 121
          lnotab
             0x02011601140114fe1205080108020c0102010201020102fc1207160114
             0114fe1206ff00ff0094030c0102010201160102fc12071601140114fe12
             06
       code
@@ -2320,15 +2320,15 @@
             ('py0', 'py2', 'py3', 'py4', 'py6')
             0.6
             0.9
          names      ('torch', 'tensor', 'entropy', 'np', 'log2', 'float', 'allclose', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'pytest', 'raises', 'RuntimeError')
          varnames   ('probabilities', 'bit_score_values', 'expected_values', '@py_assert1', '@py_assert5', '@py_format7', 'invalid_probabilities')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'test_entropy'
          firstlineno 162
          lnotab
             0x020234021e0116025c015cfe020416fb1208ff00ff006202340116010e
             ff10031efc
       code
          argcount  : 0
@@ -2512,15 +2512,15 @@
             'assert %(py7)s'
             'py7'
             (2, 2, 3, 2, 2)
          names      ('torch', 'randn', 'output_to_item_entropy', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'pytest', 'raises', 'ValueError')
          varnames   ('output', 'item_categories', 'entropies', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'test_output_to_item_entropy'
          firstlineno 184
          lnotab 0x02022a0108012001ff008303340124ff
       code
          argcount  : 0
          nlocals   : 22
          stacksize : 8
@@ -3348,15 +3348,15 @@
             (1, 1)
             (2, 0)
             (2, 1)
          names      ('torch', 'tensor', 'float', 'impute_missing', 'clone', 'all', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'logical_or', 'isnan')
          varnames   ('data', 'mc_correct', 'imputed_data', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert1', '@py_assert11', '@py_assert13', '@py_format9', '@py_format15', 'missing_mask', '@py_assert0', '@py_assert2', '@py_assert8', '@py_assert10', '@py_format6', '@py_format12', '@py_assert9', '@py_format5', '@py_format11', '@py_format7')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'test_impute_missing'
          firstlineno 195
          lnotab
             0x0201760208014401ff00ff00e80228015601ff008901ff008f01ff0009
             01ff000901ff000901ff000901
       code
          argcount  : 0
@@ -4412,23 +4412,23 @@
             (2, 1, 3, 1, 2)
             2
             (0, 1, 2)
          names      ('random_guessing_data', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'min', 'max', 'unique', 'tolist')
          varnames   ('item_categories', 'guessing_probabilities', 'data', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert5', '@py_format10', '@py_assert0', '@py_assert2', '@py_assert7', '@py_format9', '@py_format11', '@py_assert10', '@py_assert9', '@py_format12', '@py_format14', 'mc_correct')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
          name       'test_random_guessing_data'
          firstlineno 212
          lnotab
             0x0202080108012201ff008301ff00c101ff00c101ff008701ff00ff003c
             030801080108012401ff008301ff00c101ff00c101
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'numpy', 'np', 'irtorch._internal_utils', 'linear_regression', 'is_jupyter', 'dynamic_print', 'conditional_score_distribution', 'sum_incorrect_probabilities', 'entropy', 'output_to_item_entropy', 'impute_missing', 'random_guessing_data', 'fixture', 'logits', 'test_is_jupyter', 'testdynamic_print', 'test_linear_regression', 'test_conditional_scores_distribution', 'test_sum_incorrect_probabilities', 'test_entropy', 'test_output_to_item_entropy', 'test_impute_missing', 'test_random_guessing_data')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_internal_utils.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_internal_utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02012201080108012c0c200104ff0e01022b0603060c060b062306
       290616060b0611
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_irt_evaluator.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_irt_evaluator.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -92,40 +92,40 @@
                118 IMPORT_FROM             21 (QuantileMVNormal)
                120 STORE_NAME              21 (QuantileMVNormal)
                122 POP_TOP
    
     11         124 LOAD_NAME               12 (pytest)
                126 LOAD_ATTR               22 (fixture)
    
-    12         136 LOAD_CONST               8 (<code object irt_evaluator, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 11>)
+    12         136 LOAD_CONST               8 (<code object irt_evaluator, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 11>)
                138 MAKE_FUNCTION            0
    
     11         140 PRECALL                  0
                144 CALL                     0
    
     12         154 STORE_NAME              23 (irt_evaluator)
    
     93         156 LOAD_CONST               9 ('irt_evaluator')
                158 LOAD_NAME               14 (IRTEvaluator)
                160 BUILD_TUPLE              2
-               162 LOAD_CONST              10 (<code object test_evaluate_data_z_input, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 93>)
+               162 LOAD_CONST              10 (<code object test_evaluate_data_z_input, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 93>)
                164 MAKE_FUNCTION            4 (annotations)
                166 STORE_NAME              24 (test_evaluate_data_z_input)
    
    117         168 LOAD_CONST               9 ('irt_evaluator')
                170 LOAD_NAME               14 (IRTEvaluator)
                172 BUILD_TUPLE              2
-               174 LOAD_CONST              11 (<code object test_probabilities_from_grouped_z, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 117>)
+               174 LOAD_CONST              11 (<code object test_probabilities_from_grouped_z, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 117>)
                176 MAKE_FUNCTION            4 (annotations)
                178 STORE_NAME              25 (test_probabilities_from_grouped_z)
    
    130         180 LOAD_CONST               9 ('irt_evaluator')
                182 LOAD_NAME               14 (IRTEvaluator)
                184 BUILD_TUPLE              2
-               186 LOAD_CONST              12 (<code object test_probabilities_from_grouped_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 130>)
+               186 LOAD_CONST              12 (<code object test_probabilities_from_grouped_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 130>)
                188 MAKE_FUNCTION            4 (annotations)
                190 STORE_NAME              26 (test_probabilities_from_grouped_data)
    
    162         192 LOAD_NAME               12 (pytest)
                194 LOAD_ATTR               27 (mark)
                204 LOAD_METHOD             28 (parametrize)
                226 LOAD_CONST              13 ('scale')
@@ -134,26 +134,26 @@
                232 BUILD_LIST               2
                234 PRECALL                  2
                238 CALL                     2
    
    163         248 LOAD_CONST               9 ('irt_evaluator')
                250 LOAD_NAME               14 (IRTEvaluator)
                252 BUILD_TUPLE              2
-               254 LOAD_CONST              16 (<code object test_latent_group_probabilities, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 162>)
+               254 LOAD_CONST              16 (<code object test_latent_group_probabilities, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 162>)
                256 MAKE_FUNCTION            4 (annotations)
    
    162         258 PRECALL                  0
                262 CALL                     0
    
    163         272 STORE_NAME              29 (test_latent_group_probabilities)
    
    193         274 LOAD_CONST               9 ('irt_evaluator')
                276 LOAD_NAME               14 (IRTEvaluator)
                278 BUILD_TUPLE              2
-               280 LOAD_CONST              17 (<code object test_group_fit_residuals, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 193>)
+               280 LOAD_CONST              17 (<code object test_group_fit_residuals, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 193>)
                282 MAKE_FUNCTION            4 (annotations)
                284 STORE_NAME              30 (test_group_fit_residuals)
    
    208         286 LOAD_NAME               12 (pytest)
                288 LOAD_ATTR               27 (mark)
                298 LOAD_METHOD             28 (parametrize)
    
@@ -164,47 +164,47 @@
    
    208         328 PRECALL                  2
                332 CALL                     2
    
    211         342 LOAD_CONST               9 ('irt_evaluator')
                344 LOAD_NAME               14 (IRTEvaluator)
                346 BUILD_TUPLE              2
-               348 LOAD_CONST              20 (<code object test_sum_score_probabilities, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 208>)
+               348 LOAD_CONST              20 (<code object test_sum_score_probabilities, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 208>)
                350 MAKE_FUNCTION            4 (annotations)
    
    208         352 PRECALL                  0
                356 CALL                     0
    
    211         366 STORE_NAME              31 (test_sum_score_probabilities)
    
    227         368 LOAD_CONST               9 ('irt_evaluator')
                370 LOAD_NAME               14 (IRTEvaluator)
                372 BUILD_TUPLE              2
-               374 LOAD_CONST              21 (<code object test_log_likelihood, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 227>)
+               374 LOAD_CONST              21 (<code object test_log_likelihood, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 227>)
                376 MAKE_FUNCTION            4 (annotations)
                378 STORE_NAME              32 (test_log_likelihood)
    
    277         380 LOAD_CONST               9 ('irt_evaluator')
                382 LOAD_NAME               14 (IRTEvaluator)
                384 BUILD_TUPLE              2
-               386 LOAD_CONST              22 (<code object test_accuracy, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 277>)
+               386 LOAD_CONST              22 (<code object test_accuracy, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 277>)
                388 MAKE_FUNCTION            4 (annotations)
                390 STORE_NAME              33 (test_accuracy)
    
    315         392 LOAD_CONST               9 ('irt_evaluator')
                394 LOAD_NAME               14 (IRTEvaluator)
                396 BUILD_TUPLE              2
-               398 LOAD_CONST              23 (<code object test_residuals, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 315>)
+               398 LOAD_CONST              23 (<code object test_residuals, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 315>)
                400 MAKE_FUNCTION            4 (annotations)
                402 STORE_NAME              34 (test_residuals)
    
    366         404 LOAD_CONST               9 ('irt_evaluator')
                406 LOAD_NAME               14 (IRTEvaluator)
                408 BUILD_TUPLE              2
-               410 LOAD_CONST              24 (<code object test_infit_outfit, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 366>)
+               410 LOAD_CONST              24 (<code object test_infit_outfit, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 366>)
                412 MAKE_FUNCTION            4 (annotations)
                414 STORE_NAME              35 (test_infit_outfit)
                416 LOAD_CONST               1 (None)
                418 RETURN_VALUE
    consts
       0
       None
@@ -268,15 +268,15 @@
           16          56 LOAD_CONST               4 (False)
                       58 LOAD_FAST                1 (mock_algorithm)
                       60 STORE_ATTR               2 (one_hot_encoded)
          
           17          70 LOAD_GLOBAL              7 (NULL + torch)
                       82 LOAD_ATTR                4 (cat)
          
-          18          92 LOAD_CONST               5 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 18>)
+          18          92 LOAD_CONST               5 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 18>)
                       94 MAKE_FUNCTION            0
          
           20          96 LOAD_DEREF              12 (item_categories)
          
           18          98 GET_ITER
                      100 PRECALL                  0
                      104 CALL                     0
@@ -294,15 +294,15 @@
                      166 LOAD_CONST               8 (30)
                      168 LOAD_DEREF               0 (latent_variables)
                      170 PRECALL                  2
                      174 CALL                     2
                      184 LOAD_FAST                1 (mock_algorithm)
                      186 STORE_ATTR               7 (training_z_scores)
          
-          27         196 LOAD_CONST               9 (<code object fix_missing_values_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 27>)
+          27         196 LOAD_CONST               9 (<code object fix_missing_values_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 27>)
                      198 MAKE_FUNCTION            0
                      200 STORE_FAST               2 (fix_missing_values_mock)
          
           30         202 LOAD_GLOBAL              1 (NULL + MagicMock)
                      214 LOAD_FAST                2 (fix_missing_values_mock)
                      216 KW_NAMES                10
                      218 PRECALL                  1
@@ -312,21 +312,21 @@
          
           32         244 LOAD_CONST              11 ('input_tensor')
                      246 LOAD_GLOBAL              6 (torch)
                      258 LOAD_ATTR                9 (Tensor)
                      268 BUILD_TUPLE              2
                      270 LOAD_CLOSURE            12 (item_categories)
                      272 BUILD_TUPLE              1
-                     274 LOAD_CONST              12 (<code object model_forward_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 32>)
+                     274 LOAD_CONST              12 (<code object model_forward_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 32>)
                      276 MAKE_FUNCTION           12 (annotations, closure)
                      278 STORE_FAST               3 (model_forward_mock)
          
           40         280 LOAD_CLOSURE            12 (item_categories)
                      282 BUILD_TUPLE              1
-                     284 LOAD_CONST              13 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 40>)
+                     284 LOAD_CONST              13 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 40>)
                      286 MAKE_FUNCTION            8 (closure)
                      288 STORE_FAST               4 (item_probabilities_mock)
          
           46         290 LOAD_GLOBAL              1 (NULL + MagicMock)
                      302 LOAD_GLOBAL             20 (BaseIRTModel)
                      314 LOAD_FAST                3 (model_forward_mock)
                      316 KW_NAMES                14
@@ -360,15 +360,15 @@
          
           52         432 LOAD_DEREF               0 (latent_variables)
                      434 LOAD_FAST                5 (mock_model)
                      436 STORE_ATTR              16 (latent_variables)
          
           55         446 LOAD_CLOSURE             0 (latent_variables)
                      448 BUILD_TUPLE              1
-                     450 LOAD_CONST              15 (<code object z_scores_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 55>)
+                     450 LOAD_CONST              15 (<code object z_scores_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 55>)
                      452 MAKE_FUNCTION            8 (closure)
                      454 STORE_FAST               6 (z_scores_mock)
          
           59         456 LOAD_GLOBAL              1 (NULL + MagicMock)
                      468 LOAD_FAST                6 (z_scores_mock)
                      470 KW_NAMES                10
                      472 PRECALL                  1
@@ -381,27 +381,27 @@
                      522 KW_NAMES                 3
                      524 PRECALL                  1
                      528 CALL                     1
                      538 STORE_FAST               7 (mock_scorer)
          
           64         540 LOAD_CLOSURE             0 (latent_variables)
                      542 BUILD_TUPLE              1
-                     544 LOAD_CONST              16 (<code object latent_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 64>)
+                     544 LOAD_CONST              16 (<code object latent_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 64>)
                      546 MAKE_FUNCTION            8 (closure)
                      548 STORE_FAST               8 (latent_scores)
          
-          69         550 LOAD_CONST              17 (<code object bit_scores_from_z_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 69>)
+          69         550 LOAD_CONST              17 (<code object bit_scores_from_z_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 69>)
                      552 MAKE_FUNCTION            0
                      554 STORE_FAST               9 (bit_scores_from_z_mock)
          
-          73         556 LOAD_CONST              18 (<code object min_max_z_for_integration_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 73>)
+          73         556 LOAD_CONST              18 (<code object min_max_z_for_integration_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 73>)
                      558 MAKE_FUNCTION            0
                      560 STORE_FAST              10 (min_max_z_for_integration_mock)
          
-          80         562 LOAD_CONST              19 (<code object pdf_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 80>)
+          80         562 LOAD_CONST              19 (<code object pdf_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 80>)
                      564 MAKE_FUNCTION            0
                      566 STORE_FAST              11 (pdf_mock)
          
           82         568 LOAD_GLOBAL              1 (NULL + MagicMock)
                      580 LOAD_FAST                8 (latent_scores)
                      582 KW_NAMES                10
                      584 PRECALL                  1
@@ -484,15 +484,15 @@
                consts
                   0
                   (30, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 18
                lnotab 0x080202ff2aff
             1
             ('dim',)
             30
             code
@@ -507,15 +507,15 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('input_tensor',)
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'fix_missing_values_mock'
                firstlineno 27
                lnotab 0x0201
             ('side_effect',)
             'input_tensor'
             code
                argcount  : 1
@@ -529,15 +529,15 @@
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (input_tensor)
                
                 32           4 RESUME                   0
                
                 33           6 LOAD_CLOSURE             0 (input_tensor)
                              8 BUILD_TUPLE              1
-                            10 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 33>)
+                            10 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 33>)
                             12 MAKE_FUNCTION            8 (closure)
                
                 35          14 LOAD_DEREF               2 (item_categories)
                
                 33          16 GET_ITER
                             18 PRECALL                  0
                             22 CALL                     0
@@ -586,25 +586,25 @@
                              >>   78 RETURN_VALUE
                      consts
                         0
                      names      ('torch', 'randn', 'shape')
                      varnames   ('.0', 'category')
                      freevars   ('input_tensor',)
                      cellvars   ()
-                     filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+                     filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                      name       '<listcomp>'
                      firstlineno 33
                      lnotab 0x0a0202ff3eff
                   1
                   ('dim',)
                names      ('torch', 'cat')
                varnames   ('input_tensor', 'logits')
                freevars   ('item_categories',)
                cellvars   ('input_tensor',)
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'model_forward_mock'
                firstlineno 32
                lnotab 0x0601080202fe1204
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 7
@@ -679,15 +679,15 @@
                   0
                   2
                   ('dim',)
                names      ('torch', 'randn', 'shape', 'len', 'max', 'enumerate', 'inf', 'softmax')
                varnames   ('input_tensor', 'logits', 'item_id', 'item_cats')
                freevars   ('item_categories',)
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'item_probabilities_mock'
                firstlineno 40
                lnotab 0x0401760128013001
             ('spec', 'side_effect')
             code
                argcount  : 1
                nlocals   : 2
@@ -717,15 +717,15 @@
                consts
                   None
                   0
                names      ('torch', 'randn', 'shape')
                varnames   ('input_tensor', 'z_scores')
                freevars   ('latent_variables',)
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'z_scores_mock'
                firstlineno 55
                lnotab 0x04014001
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
@@ -754,15 +754,15 @@
                consts
                   None
                   0
                names      ('torch', 'randn', 'shape')
                varnames   ('data', 'kwargs', 'z_scores')
                freevars   ('latent_variables',)
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'latent_scores'
                firstlineno 64
                lnotab 0x04014001
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
@@ -810,15 +810,15 @@
                   0
                   1
                   10
                names      ('torch', 'randn', 'shape', 'abs')
                varnames   ('z', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'bit_scores_from_z_mock'
                firstlineno 69
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 3
@@ -872,15 +872,15 @@
                   None
                   0
                   ('dim',)
                names      ('min', 'max', 'std')
                varnames   ('z', 'z_min', 'z_max', 'z_stds')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'min_max_z_for_integration_mock'
                firstlineno 73
                lnotab 0x0201380138012c01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -903,23 +903,23 @@
                consts
                   None
                   0
                names      ('torch', 'rand', 'shape')
                varnames   ('z',)
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'pdf_mock'
                firstlineno 80
                lnotab 0x0201
          names      ('MagicMock', 'BaseIRTAlgorithm', 'one_hot_encoded', 'torch', 'cat', 'train_data', 'randn', 'training_z_scores', 'fix_missing_values', 'Tensor', 'BaseIRTModel', 'item_probabilities', 'item_categories', 'modeled_item_responses', 'model_missing', 'mc_correct', 'latent_variables', 'z_scores', 'IRTScorer', 'latent_scores', 'bit_scores_from_z', 'min_max_z_for_integration', 'QuantileMVNormal', 'latent_density', 'pdf', 'IRTEvaluator')
          varnames   ('latent_variables', 'mock_algorithm', 'fix_missing_values_mock', 'model_forward_mock', 'item_probabilities_mock', 'mock_model', 'z_scores_mock', 'mock_scorer', 'latent_scores', 'bit_scores_from_z_mock', 'min_max_z_for_integration_mock', 'pdf_mock')
          freevars   ()
          cellvars   ('latent_variables', 'item_categories')
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'irt_evaluator'
          firstlineno 11
          lnotab
             0x060308012a010e011601040202fe100402fb1c07340306032a0224080a
             062c012a010e010e010e010e010e030a042a022a030a050604060706022a
             012a010c0102ff1c0326013401
       'irt_evaluator'
@@ -1018,15 +1018,15 @@
             00ab0100000000000000008201640078017d0478017d0678017d0578017d
             097d0a64005300
           93           0 RESUME                   0
          
           95           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (cat)
          
-          96          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 96>)
+          96          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 96>)
                       26 MAKE_FUNCTION            0
          
           98          28 LOAD_FAST                0 (irt_evaluator)
                       30 LOAD_ATTR                2 (model)
                       40 LOAD_ATTR                3 (item_categories)
          
           96          50 GET_ITER
@@ -1553,15 +1553,15 @@
                consts
                   0
                   (30, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 96
                lnotab 0x080202ff2aff
             1
             ('dim',)
             'NN'
             ('==',)
@@ -1578,15 +1578,15 @@
             'assert %(py12)s'
             'py12'
             ('%(py2)s\n{%(py2)s = %(py0)s.shape\n} == %(py10)s\n{%(py10)s = %(py8)s\n{%(py8)s = %(py6)s\n{%(py6)s = %(py4)s.algorithm\n}.train_data\n}.shape\n}',)
          names      ('torch', 'cat', 'model', 'item_categories', '_evaluate_data_z_input', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'algorithm', 'training_z_scores', 'train_data')
          varnames   ('irt_evaluator', 'data', 'result_data', 'result_z', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert7', '@py_assert9', '@py_format11', '@py_format13')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_evaluate_data_z_input'
          firstlineno 93
          lnotab
             0x02021601040216fe100402fb12093403ff00ff000a01ff00ff007c0334
             03ff00ff007c01
       code
          argcount  : 2
@@ -1975,15 +1975,15 @@
             'assert %(py22)s\n{%(py22)s = %(py2)s\n{%(py2)s = %(py0)s.allclose\n}(%(py9)s\n{%(py9)s = %(py5)s\n{%(py5)s = %(py3)s.sum\n}(dim=%(py7)s)\n}, %(py18)s\n{%(py18)s = %(py12)s\n{%(py12)s = %(py10)s.ones\n}(%(py14)s, %(py16)s)\n}, atol=%(py20)s)\n}'
             'torch'
             ('py0', 'py2', 'py3', 'py5', 'py7', 'py9', 'py10', 'py12', 'py14', 'py16', 'py18', 'py20', 'py22')
          names      ('torch', 'randn', '_grouped_z_probabilities', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'allclose', 'sum', 'ones')
          varnames   ('irt_evaluator', 'latent_variables', 'grouped_z', 'probabilities', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert8', '@py_assert11', '@py_assert13', '@py_assert15', '@py_assert17', '@py_assert19', '@py_assert21', '@py_format23')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_probabilities_from_grouped_z'
          firstlineno 117
          lnotab 0x02032801280128fd04072a01ff008301
       code
          argcount  : 1
          nlocals   : 19
          stacksize : 15
@@ -2058,15 +2058,15 @@
             017d0a78017d0b78017d0c78017d0d78017d0e78017d0f78017d107d1164
             005300
          130           0 RESUME                   0
          
          133           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (cat)
          
-         134          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 134>)
+         134          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 134>)
                       26 MAKE_FUNCTION            0
          
          136          28 LOAD_FAST                0 (irt_evaluator)
                       30 LOAD_ATTR                2 (model)
                       40 LOAD_ATTR                3 (item_categories)
          
          134          50 GET_ITER
@@ -2078,15 +2078,15 @@
          133          68 KW_NAMES                 3
                       70 PRECALL                  2
                       74 CALL                     2
          
          140          84 LOAD_GLOBAL              1 (NULL + torch)
                       96 LOAD_ATTR                1 (cat)
          
-         141         106 LOAD_CONST               4 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 141>)
+         141         106 LOAD_CONST               4 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 141>)
                      108 MAKE_FUNCTION            0
          
          143         110 LOAD_FAST                0 (irt_evaluator)
                      112 LOAD_ATTR                2 (model)
                      122 LOAD_ATTR                3 (item_categories)
          
          141         132 GET_ITER
@@ -2098,15 +2098,15 @@
          140         150 KW_NAMES                 3
                      152 PRECALL                  2
                      156 CALL                     2
          
          147         166 LOAD_GLOBAL              1 (NULL + torch)
                      178 LOAD_ATTR                1 (cat)
          
-         148         188 LOAD_CONST               5 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 148>)
+         148         188 LOAD_CONST               5 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 148>)
                      190 MAKE_FUNCTION            0
          
          150         192 LOAD_FAST                0 (irt_evaluator)
                      194 LOAD_ATTR                2 (model)
                      204 LOAD_ATTR                3 (item_categories)
          
          148         214 GET_ITER
@@ -2472,15 +2472,15 @@
                consts
                   0
                   (5, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 134
                lnotab 0x080202ff2aff
             1
             ('dim',)
             code
                argcount  : 1
@@ -2511,15 +2511,15 @@
                consts
                   0
                   (5, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 141
                lnotab 0x080202ff2aff
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
@@ -2548,15 +2548,15 @@
                consts
                   0
                   (5, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 148
                lnotab 0x080202ff2aff
             (3, 2, 3)
             ('==',)
             ('%(py2)s\n{%(py2)s = %(py0)s.shape\n} == %(py10)s\n{%(py10)s = %(py6)s\n{%(py6)s = %(py4)s.Size\n}(%(py8)s)\n}',)
             'probabilities'
@@ -2570,15 +2570,15 @@
             ('atol',)
             'assert %(py20)s\n{%(py20)s = %(py2)s\n{%(py2)s = %(py0)s.allclose\n}(%(py9)s\n{%(py9)s = %(py5)s\n{%(py5)s = %(py3)s.sum\n}(dim=%(py7)s)\n}, %(py16)s\n{%(py16)s = %(py12)s\n{%(py12)s = %(py10)s.ones_like\n}(%(py14)s)\n}, atol=%(py18)s)\n}'
             ('py0', 'py2', 'py3', 'py5', 'py7', 'py9', 'py10', 'py12', 'py14', 'py16', 'py18', 'py20')
          names      ('torch', 'cat', 'model', 'item_categories', '_grouped_data_probabilities', 'shape', 'Size', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'allclose', 'sum', 'ones_like')
          varnames   ('irt_evaluator', 'grouped_data', 'probabilities', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert3', '@py_format11', '@py_format13', '@py_assert4', '@py_assert6', '@py_assert8', '@py_assert11', '@py_assert13', '@py_assert15', '@py_assert17', '@py_assert19', '@py_format21')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_probabilities_from_grouped_data'
          firstlineno 130
          lnotab
             0x02031601040216fe100402fb10071601040216fe100402fb1007160104
             0216fe100402fb10f104192a02ff00ff009c01
       'scale'
       'bit'
@@ -2720,15 +2720,15 @@
             0000006a130000000000000000a014000000000000000000000000000000
             0000000000a6000000ab00000000000000000001006400530064005300
          162           0 RESUME                   0
          
          165           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (cat)
          
-         166          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 166>)
+         166          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 166>)
                       26 MAKE_FUNCTION            0
          
          168          28 LOAD_FAST                0 (irt_evaluator)
                       30 LOAD_ATTR                2 (model)
                       40 LOAD_ATTR                3 (item_categories)
          
          166          50 GET_ITER
@@ -3489,15 +3489,15 @@
                consts
                   0
                   (30, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 166
                lnotab 0x080202ff2aff
             1
             ('dim',)
             3
             ('groups', 'data', 'scale', 'latent_variable')
@@ -3526,15 +3526,15 @@
             'assert %(py7)s'
             'py7'
             'bit'
          names      ('torch', 'cat', 'model', 'item_categories', 'latent_group_probabilities', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'Size', 'allclose', 'sum', 'ones_like', 'scorer', 'bit_scores_from_z', 'assert_called_once')
          varnames   ('irt_evaluator', 'scale', 'data', 'groups', 'grouped_data_probabilities', 'grouped_model_probabilities', 'group_averages', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert7', '@py_assert9', '@py_format11', '@py_format13', '@py_assert4', '@py_assert6', '@py_assert8', '@py_assert11', '@py_assert13', '@py_assert15', '@py_assert17', '@py_assert19', '@py_format21', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_latent_group_probabilities'
          firstlineno 162
          lnotab
             0x02031601040216fe100402fb12080405180108ff10fc04010201020102
             06ff00ff000a01ff00ff009c01ff00ff00ff00ff001c01ff00ff00ff00ff
             001c01ff0085020c0240fe
       code
@@ -3592,15 +3592,15 @@
             0100000000000000008201640078017d0478017d0678017d0978017d0b7d
             0a64005300
          193           0 RESUME                   0
          
          194           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (cat)
          
-         195          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 195>)
+         195          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 195>)
                       26 MAKE_FUNCTION            0
          
          197          28 LOAD_FAST                0 (irt_evaluator)
                       30 LOAD_ATTR                2 (model)
                       40 LOAD_ATTR                3 (item_categories)
          
          195          50 GET_ITER
@@ -3912,15 +3912,15 @@
                consts
                   0
                   (30, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 195
                lnotab 0x080202ff2aff
             1
             ('dim',)
             3
             ('data', 'groups', 'latent_variable')
@@ -3938,15 +3938,15 @@
             ('py0', 'py2', 'py4', 'py6', 'py9')
             'assert %(py11)s'
             'py11'
          names      ('torch', 'cat', 'model', 'item_categories', 'group_fit_residuals', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'item_probabilities', 'call_count')
          varnames   ('irt_evaluator', 'data', 'residuals', 'mid_points', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert5', '@py_assert8', '@py_assert7', '@py_format10', '@py_format12')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_group_fit_residuals'
          firstlineno 193
          lnotab 0x02011601040216fe100402fb12083602ff008301ff008301
       'latent_density_method'
       ('data', 'encoder sampling', 'qmvn', 'gmm')
       code
          argcount  : 2
@@ -4334,15 +4334,15 @@
             'assert %(py18)s\n{%(py18)s = %(py2)s\n{%(py2)s = %(py0)s.isclose\n}(%(py7)s\n{%(py7)s = %(py5)s\n{%(py5)s = %(py3)s.sum\n}()\n}, %(py14)s\n{%(py14)s = %(py10)s\n{%(py10)s = %(py8)s.tensor\n}(%(py12)s)\n}, atol=%(py16)s)\n}'
             'torch'
             ('py0', 'py2', 'py3', 'py5', 'py7', 'py8', 'py10', 'py12', 'py14', 'py16', 'py18')
          names      ('pytest', 'raises', 'ValueError', 'sum_score_probabilities', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'torch', 'isclose', 'sum', 'tensor')
          varnames   ('irt_evaluator', 'latent_density_method', 'total_score_probs', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert9', '@py_assert11', '@py_assert13', '@py_assert15', '@py_assert17', '@py_format19')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_sum_score_probabilities'
          firstlineno 208
          lnotab 0x02040c013401180102ff12ff3405180104ff1205ff008302
       code
          argcount  : 1
          nlocals   : 23
          stacksize : 12
@@ -4722,15 +4722,15 @@
             00ab0100000000000000008201640078017d0478017d0678017d0c78017d
             0d78017d0e78017d157d1064005300
          227            0 RESUME                   0
          
          229            2 LOAD_GLOBAL              1 (NULL + torch)
                        14 LOAD_ATTR                1 (cat)
          
-         230           24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 230>)
+         230           24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 230>)
                        26 MAKE_FUNCTION            0
          
          232           28 LOAD_FAST                0 (irt_evaluator)
                        30 LOAD_ATTR                2 (model)
                        40 LOAD_ATTR                3 (item_categories)
          
          230           50 GET_ITER
@@ -4740,15 +4740,15 @@
          234           66 LOAD_CONST               2 (1)
          
          229           68 KW_NAMES                 3
                        70 PRECALL                  2
                        74 CALL                     2
                        84 STORE_FAST               1 (data)
          
-         238           86 LOAD_CONST               4 (<code object log_likelihood_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 238>)
+         238           86 LOAD_CONST               4 (<code object log_likelihood_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 238>)
                        88 MAKE_FUNCTION            0
                        90 STORE_FAST               2 (log_likelihood_mock)
          
          243           92 LOAD_GLOBAL              9 (NULL + MagicMock)
                       104 LOAD_FAST                2 (log_likelihood_mock)
                       106 KW_NAMES                 5
                       108 PRECALL                  1
@@ -6788,15 +6788,15 @@
                consts
                   0
                   (30, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 230
                lnotab 0x080202ff2aff
             1
             ('dim',)
             code
                argcount  : 3
@@ -6873,15 +6873,15 @@
                   2
                   -0.1
                   -0.2
                names      ('torch', 'tensor', 'repeat', 'shape', 'cat')
                varnames   ('data', 'output', 'loss_reduction', 't1', 't2')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'log_likelihood_mock'
                firstlineno 238
                lnotab 0x02016e018a01
             ('side_effect',)
             ('data',)
             (10,)
             ('==',)
@@ -6922,15 +6922,15 @@
             'assert %(py14)s\n{%(py14)s = %(py2)s\n{%(py2)s = %(py0)s.isclose\n}(%(py4)s, %(py12)s\n{%(py12)s = %(py7)s\n{%(py7)s = %(py5)s.tensor\n}(-%(py9)s)\n})\n}'
             ('py0', 'py2', 'py4', 'py5', 'py7', 'py9', 'py12', 'py14')
             0.6
          names      ('torch', 'cat', 'model', 'item_categories', 'MagicMock', 'log_likelihood', 'group_fit_log_likelihood', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'dtype', 'float32', 'allclose', 'full', 'isclose', 'tensor')
          varnames   ('irt_evaluator', 'data', 'log_likelihood_mock', 'group_mean_likelihoods', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert5', '@py_format7', '@py_format9', '@py_assert6', '@py_assert8', '@py_assert10', '@py_assert12', '@py_assert13', '@py_assert15', '@py_format17', 'person_likelihoods', 'item_likelihoods', '@py_assert11', '@py_format15')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_log_likelihood'
          firstlineno 227
          lnotab
             0x02021601040216fe100402fb1209060534042c01ff008301ff00ff0028
             01ff00ff00ff002301ff00ff00ff0023023201ff008301ff00ff002801ff
             00ff00ff002301ff00ff00ff001f01ff00ff00ff0023043001ff008301ff
             00ff002801ff00ff00ff002301ff00ff00ff0023043001ff008301ff00ff
@@ -7137,15 +7137,15 @@
             008201640078017d0478017d0578017d0978017d0d78017d0c78017d0e7d
             0f64005300
          277           0 RESUME                   0
          
          279           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (cat)
          
-         280          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 280>)
+         280          24 LOAD_CONST               1 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 280>)
                       26 MAKE_FUNCTION            0
          
          282          28 LOAD_FAST                0 (irt_evaluator)
                       30 LOAD_ATTR                2 (model)
                       40 LOAD_ATTR                3 (item_categories)
          
          280          50 GET_ITER
@@ -7155,15 +7155,15 @@
          284          66 LOAD_CONST               2 (1)
          
          279          68 KW_NAMES                 3
                       70 PRECALL                  2
                       74 CALL                     2
                       84 STORE_FAST               1 (data)
          
-         288          86 LOAD_CONST               4 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 288>)
+         288          86 LOAD_CONST               4 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 288>)
                       88 MAKE_FUNCTION            0
                       90 STORE_FAST               2 (item_probabilities_mock)
          
          294          92 LOAD_GLOBAL              9 (NULL + MagicMock)
                      104 LOAD_FAST                2 (item_probabilities_mock)
                      106 KW_NAMES                 5
                      108 PRECALL                  1
@@ -8287,15 +8287,15 @@
                consts
                   0
                   (30, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       '<listcomp>'
                firstlineno 280
                lnotab 0x080202ff2aff
             1
             ('dim',)
             code
                argcount  : 1
@@ -8397,15 +8397,15 @@
                   1
                   (0.15, 0.85, 0.0)
                   (0.6, 0.05, 0.35)
                names      ('torch', 'tensor', 'unsqueeze', 'repeat', 'shape', 'cat')
                varnames   ('z', 't1', 't2')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'item_probabilities_mock'
                firstlineno 288
                lnotab 0x0202a001bc01
             ('side_effect',)
             'all'
             ('data', 'level')
             ()
@@ -8435,15 +8435,15 @@
             'item'
             (2,)
             'item_likelihoods'
          names      ('torch', 'cat', 'model', 'item_categories', 'MagicMock', 'item_probabilities', 'accuracy', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'dtype', 'float32', 'all', '_format_assertmsg')
          varnames   ('irt_evaluator', 'data', 'item_probabilities_mock', 'accuracy', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert5', '@py_format7', '@py_format9', '@py_assert11', '@py_assert10', '@py_assert15', '@py_assert16', '@py_format13', '@py_format18', 'item_likelihoods')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_accuracy'
          firstlineno 277
          lnotab
             0x02021601040216fe100402fb1209060634032e01ff008301ff00ff0028
             01ff00ff00ff0091032e01ff008301ff00ff002801ff00ff00ff0091032e
             01ff008301ff00ff002801
       code
@@ -8663,15 +8663,15 @@
          
          325          70 LOAD_METHOD              2 (float)
                       92 PRECALL                  0
                       96 CALL                     0
          
          317         106 STORE_FAST               1 (data)
          
-         328         108 LOAD_CONST               4 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 328>)
+         328         108 LOAD_CONST               4 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 328>)
                      110 MAKE_FUNCTION            0
                      112 STORE_FAST               2 (item_probabilities_mock)
          
          334         114 LOAD_GLOBAL              7 (NULL + MagicMock)
                      126 LOAD_FAST                2 (item_probabilities_mock)
                      128 KW_NAMES                 5
                      130 PRECALL                  1
@@ -9755,15 +9755,15 @@
                   1
                   (0.15, 0.85, 0.0)
                   (0.6, 0.05, 0.35)
                names      ('torch', 'tensor', 'unsqueeze', 'repeat', 'shape', 'cat')
                varnames   ('z', 't1', 't2')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'item_probabilities_mock'
                firstlineno 328
                lnotab 0x0202a001bc01
             ('side_effect',)
             ('data',)
             (5, 2)
             ('==',)
@@ -9795,15 +9795,15 @@
             (2,)
             0.57
             0.64
          names      ('torch', 'tensor', 'float', 'MagicMock', 'model', 'item_probabilities', 'mc_correct', 'residuals', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'allclose', '_format_assertmsg', 'isclose')
          varnames   ('irt_evaluator', 'data', 'item_probabilities_mock', 'residuals', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_format13')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_residuals'
          firstlineno 315
          lnotab
             0x02021602060106010601060106fb02ff0e0824f8020b060634051c022c
             01ff0083010c060afa0e060afa64060afa24060afa1e060afa28060afa2a
             060afa1e060afa1e060afa1e060afa22060afa1e060afa28060afa2a060a
             fa1c060afa1c060afa1c060afa32060afa34092e01ff008301ff00ff00ff
@@ -10084,28 +10084,28 @@
                      114 LOAD_FAST                0 (irt_evaluator)
                      116 LOAD_ATTR                4 (model)
                      126 LOAD_ATTR                5 (latent_variables)
                      136 PRECALL                  2
                      140 CALL                     2
                      150 STORE_FAST               2 (z)
          
-         370         152 LOAD_CONST               4 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 370>)
+         370         152 LOAD_CONST               4 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 370>)
                      154 MAKE_FUNCTION            0
                      156 STORE_FAST               3 (item_probabilities_mock)
          
          374         158 LOAD_GLOBAL             13 (NULL + MagicMock)
                      170 LOAD_FAST                3 (item_probabilities_mock)
                      172 KW_NAMES                 5
                      174 PRECALL                  1
                      178 CALL                     1
                      188 LOAD_FAST                0 (irt_evaluator)
                      190 LOAD_ATTR                4 (model)
                      200 STORE_ATTR               7 (item_probabilities)
          
-         376         210 LOAD_CONST               6 (<code object expected_scores_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 376>)
+         376         210 LOAD_CONST               6 (<code object expected_scores_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 376>)
                      212 MAKE_FUNCTION            0
                      214 STORE_FAST               4 (expected_scores_mock)
          
          379         216 LOAD_GLOBAL             13 (NULL + MagicMock)
                      228 LOAD_FAST                4 (expected_scores_mock)
                      230 KW_NAMES                 5
                      232 PRECALL                  1
@@ -10702,15 +10702,15 @@
                     3764 STORE_FAST               8 (@py_assert5)
                     3766 COPY                     1
                     3768 STORE_FAST               9 (@py_assert7)
                     3770 COPY                     1
                     3772 STORE_FAST              10 (@py_assert9)
                     3774 STORE_FAST              11 (@py_assert11)
          
-         389        3776 LOAD_CONST              25 (<code object expected_scores_mock_mc, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_evaluator.py", line 389>)
+         389        3776 LOAD_CONST              25 (<code object expected_scores_mock_mc, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_evaluator.py", line 389>)
                     3778 MAKE_FUNCTION            0
                     3780 STORE_FAST              13 (expected_scores_mock_mc)
          
          392        3782 LOAD_GLOBAL             13 (NULL + MagicMock)
                     3794 LOAD_FAST               13 (expected_scores_mock_mc)
                     3796 KW_NAMES                 5
                     3798 PRECALL                  1
@@ -11361,15 +11361,15 @@
                   (0.2, 0.35, 0.45)
                   (0.15, 0.85, 0.0)
                   (0.6, 0.05, 0.35)
                names      ('torch', 'tensor')
                varnames   ('z',)
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'item_probabilities_mock'
                firstlineno 370
                lnotab 0x0201
             ('side_effect',)
             code
                argcount  : 1
                nlocals   : 2
@@ -11398,15 +11398,15 @@
                   1.25
                   0.85
                   0.75
                names      ('torch', 'tensor')
                varnames   ('z', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'expected_scores_mock'
                firstlineno 376
                lnotab 0x0201
             'item'
             ('level',)
             0.6
             0.4237288
@@ -11452,15 +11452,15 @@
                   0.45
                   0.15
                   0.35
                names      ('torch', 'tensor')
                varnames   ('z', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
                name       'expected_scores_mock_mc'
                firstlineno 389
                lnotab 0x0201
             3
             0.8947369
             0.4973262
             0.8803419
@@ -11468,25 +11468,25 @@
             0.4084507
             1.0202019
             0.357466
          names      ('torch', 'tensor', 'float', 'randn', 'model', 'latent_variables', 'MagicMock', 'item_probabilities', 'expected_scores', 'infit_outfit', 'allclose', '@pytest_ar', '_format_assertmsg', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'mc_correct')
          varnames   ('irt_evaluator', 'data', 'z', 'item_probabilities_mock', 'expected_scores_mock', 'infit', 'outfit', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_format13', 'expected_scores_mock_mc')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
          name       'test_infit_outfit'
          firstlineno 366
          lnotab
             0x020158013e0206043402060334023601ff00ff00ff005501ff00ff00ff
             0055023601ff00ff00ff005501ff00ff00ff005502060334021c013601ff
             00ff00ff005501ff00ff00ff0055023601ff00ff00ff005501
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'unittest.mock', 'MagicMock', 'patch', 'torch', 'torch.nn.functional', 'softmax', 'pytest', 'irtorch.irt_evaluator', 'IRTEvaluator', 'IRTScorer', 'irtorch.estimation_algorithms', 'BaseIRTAlgorithm', 'irtorch.models', 'BaseIRTModel', 'irtorch.quantile_mv_normal', 'QuantileMVNormal', 'fixture', 'irt_evaluator', 'test_evaluate_data_z_input', 'test_probabilities_from_grouped_z', 'test_probabilities_from_grouped_data', 'mark', 'parametrize', 'test_latent_group_probabilities', 'test_group_fit_residuals', 'test_sum_score_probabilities', 'test_log_likelihood', 'test_accuracy', 'test_residuals', 'test_infit_outfit')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_evaluator.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_evaluator.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02012a0108010c01080110010c010c010c030c0104ff0e0102510c
       180c0d0c2038010aff0e01021e0c0f220108ff0e030afd0e0302100c320c
       260c33
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_irt_plotter.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_irt_plotter.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -68,15 +68,15 @@
                 94 IMPORT_FROM             17 (BaseIRTModel)
                 96 STORE_NAME              17 (BaseIRTModel)
                 98 POP_TOP
    
      9         100 LOAD_NAME                9 (pytest)
                102 LOAD_ATTR               18 (fixture)
    
-    10         112 LOAD_CONST               6 (<code object irt_plotter, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_plotter.py", line 9>)
+    10         112 LOAD_CONST               6 (<code object irt_plotter, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_plotter.py", line 9>)
                114 MAKE_FUNCTION            0
    
      9         116 PRECALL                  0
                120 CALL                     0
    
     10         130 STORE_NAME              19 (irt_plotter)
                132 LOAD_CONST               1 (None)
@@ -126,15 +126,15 @@
                       40 PRECALL                  1
                       44 CALL                     1
                       54 STORE_FAST               1 (mock_algorithm)
          
           13          56 LOAD_GLOBAL              5 (NULL + torch)
                       68 LOAD_ATTR                3 (cat)
          
-          14          78 LOAD_CONST               4 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_plotter.py", line 14>)
+          14          78 LOAD_CONST               4 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_plotter.py", line 14>)
                       80 MAKE_FUNCTION            0
          
           16          82 LOAD_DEREF               8 (item_categories)
          
           14          84 GET_ITER
                       86 PRECALL                  0
                       90 CALL                     0
@@ -160,29 +160,29 @@
          
           23         186 LOAD_DEREF               8 (item_categories)
                      188 LOAD_FAST                2 (mock_model)
                      190 STORE_ATTR               7 (modeled_item_responses)
          
           26         200 LOAD_CLOSURE             8 (item_categories)
                      202 BUILD_TUPLE              1
-                     204 LOAD_CONST               7 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_plotter.py", line 26>)
+                     204 LOAD_CONST               7 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_plotter.py", line 26>)
                      206 MAKE_FUNCTION            8 (closure)
                      208 STORE_FAST               3 (item_probabilities_mock)
          
           33         210 LOAD_GLOBAL              1 (NULL + MagicMock)
                      222 LOAD_FAST                3 (item_probabilities_mock)
                      224 KW_NAMES                 8
                      226 PRECALL                  1
                      230 CALL                     1
                      240 LOAD_FAST                2 (mock_model)
                      242 STORE_ATTR               8 (item_probabilities)
          
           35         252 LOAD_CLOSURE             0 (latent_variables)
                      254 BUILD_TUPLE              1
-                     256 LOAD_CONST               9 (<code object z_scores_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_plotter.py", line 35>)
+                     256 LOAD_CONST               9 (<code object z_scores_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_plotter.py", line 35>)
                      258 MAKE_FUNCTION            8 (closure)
                      260 STORE_FAST               4 (z_scores_mock)
          
           39         262 LOAD_GLOBAL              1 (NULL + MagicMock)
                      274 LOAD_FAST                4 (z_scores_mock)
                      276 KW_NAMES                 8
                      278 PRECALL                  1
@@ -193,15 +193,15 @@
           41         304 LOAD_GLOBAL              1 (NULL + MagicMock)
                      316 LOAD_GLOBAL             20 (IRTScorer)
                      328 KW_NAMES                 3
                      330 PRECALL                  1
                      334 CALL                     1
                      344 STORE_FAST               5 (mock_scorer)
          
-          44         346 LOAD_CONST              10 (<code object bit_score_distance_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_plotter.py", line 44>)
+          44         346 LOAD_CONST              10 (<code object bit_score_distance_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_plotter.py", line 44>)
                      348 MAKE_FUNCTION            0
                      350 STORE_FAST               6 (bit_score_distance_mock)
          
           48         352 LOAD_GLOBAL              1 (NULL + MagicMock)
                      364 LOAD_FAST                6 (bit_score_distance_mock)
                      366 KW_NAMES                 8
                      368 PRECALL                  1
@@ -258,15 +258,15 @@
                consts
                   0
                   (30, 1)
                names      ('torch', 'randint')
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_plotter.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_plotter.py'
                name       '<listcomp>'
                firstlineno 14
                lnotab 0x080202ff2aff
             1
             ('dim',)
             code
                argcount  : 1
@@ -343,15 +343,15 @@
                   0
                   2
                   ('dim',)
                names      ('torch', 'randn', 'shape', 'len', 'max', 'enumerate', 'inf', 'softmax')
                varnames   ('input_tensor', 'logits', 'item_id', 'item_cats')
                freevars   ('item_categories',)
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_plotter.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_plotter.py'
                name       'item_probabilities_mock'
                firstlineno 26
                lnotab 0x0402760128013001
             ('side_effect',)
             code
                argcount  : 1
                nlocals   : 2
@@ -381,15 +381,15 @@
                consts
                   None
                   0
                names      ('torch', 'randn', 'shape')
                varnames   ('input_tensor', 'z_scores')
                freevars   ('latent_variables',)
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_plotter.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_plotter.py'
                name       'z_scores_mock'
                firstlineno 35
                lnotab 0x04014001
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 4
@@ -428,29 +428,29 @@
                   0
                   10
                   1
                names      ('torch', 'randn', 'shape', 'abs', 'unsqueeze')
                varnames   ('input_tensor', 'steps', 'bit_score_method', 'bit_score_distances')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_plotter.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_plotter.py'
                name       'bit_score_distance_mock'
                firstlineno 44
                lnotab 0x02016801
          names      ('MagicMock', 'BaseIRTAlgorithm', 'torch', 'cat', 'train_data', 'BaseIRTModel', 'item_categories', 'modeled_item_responses', 'item_probabilities', 'z_scores', 'IRTScorer', 'bit_score_distance', 'IRTEvaluator', 'IRTPlotter')
          varnames   ('latent_variables', 'mock_algorithm', 'mock_model', 'item_probabilities_mock', 'z_scores_mock', 'mock_scorer', 'bit_score_distance_mock', 'mock_evaluator')
          freevars   ()
          cellvars   ('latent_variables', 'item_categories')
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_plotter.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_plotter.py'
          name       'irt_plotter'
          firstlineno 9
          lnotab
             0x060208012a011601040202fe100402fb1c082a010e010e030a072a020a
             042a022a0306042a022a02
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'unittest.mock', 'MagicMock', 'torch', 'pytest', 'irtorch.estimation_algorithms', 'BaseIRTAlgorithm', 'irtorch.irt_plotter', 'IRTScorer', 'IRTPlotter', 'IRTEvaluator', 'irtorch.models', 'BaseIRTModel', 'fixture', 'irt_plotter')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_plotter.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_plotter.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02012601080108010c0114010c030c0104ff0e01
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_irt_scorer.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_irt_scorer.cpython-311-pytest-7.3.1.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,36 +1,39 @@
 magic:    0xa70d0d0a
-moddate:  0x31660d66 (Wed Apr  3 14:22:41 2024 UTC)
-files sz: 14108
+moddate:  0x35950e66 (Thu Apr  4 11:55:33 2024 UTC)
+files sz: 14999
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a01640064016c026d03630201006d045a05010064
       0064026c066d075a076d085a080100640064016c095a09640064036c0a6d
       0b5a0b0100640064016c0c5a0c640064046c0d6d0e5a0e0100640064056c
       0f6d105a100100640064066c116d125a1201000200470064078400640865
       12a6030000ab0300000000000000005a13650c6a14000000000000000064
       098400a6000000ab0000000000000000005a15650c6a1400000000000000
-      00640a8400a6000000ab0000000000000000005a16650c6a170000000000
-      000000a0180000000000000000000000000000000000000000640b640c64
-      0d6702a6020000ab020000000000000000650c6a170000000000000000a0
-      180000000000000000000000000000000000000000640e640f64106702a6
-      020000ab0200000000000000006411650e660264128404a6000000ab0000
-      00000000000000a6000000ab0000000000000000005a19650c6a17000000
-      0000000000a0180000000000000000000000000000000000000000641364
-      0f64146702a6020000ab0200000000000000006411650e660264158404a6
-      000000ab0000000000000000005a1a650c6a170000000000000000a01800
-      00000000000000000000000000000000000000641667006417a201a60200
-      00ab0200000000000000006411650e660264188404a6000000ab00000000
-      00000000005a1b6411650e6602641984045a1c6411650e6602641a84045a
-      1d6411650e641b65126604641c84045a1e6411650e6602641d84045a1f64
-      015300
+      00640a8400a6000000ab0000000000000000005a166400640b6c066d085a
+      0801006400640c6c0d6d175a170100650c6a180000000000000000a01900
+      00000000000000000000000000000000000000640d640e67016700640fa2
+      016702a6020000ab0200000000000000006410650e660264118404a60000
+      00ab0000000000000000005a1a650c6a180000000000000000a019000000
+      00000000000000000000000000000000006412641364146702a6020000ab
+      020000000000000000650c6a180000000000000000a01900000000000000
+      000000000000000000000000006415641664176702a6020000ab02000000
+      00000000006410650e660264188404a6000000ab000000000000000000a6
+      000000ab0000000000000000005a1b650c6a180000000000000000a01900
+      0000000000000000000000000000000000000064196416641a6702a60200
+      00ab0200000000000000006410650e6602641b8404a6000000ab00000000
+      00000000005a1c650c6a180000000000000000a019000000000000000000
+      0000000000000000000000641c6700641da201a6020000ab020000000000
+      0000006410650e6602641e8404a6000000ab0000000000000000005a1d64
+      10650e6602641f84045a1e6410650e6602642084045a1f6410650e642165
+      126604642284045a206410650e6602642384045a2164015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (builtins)
                  8 STORE_NAME               1 (@py_builtins)
                 10 LOAD_CONST               0 (0)
@@ -87,151 +90,189 @@
                100 IMPORT_NAME             17 (irtorch.models)
                102 IMPORT_FROM             18 (BaseIRTModel)
                104 STORE_NAME              18 (BaseIRTModel)
                106 POP_TOP
    
      9         108 PUSH_NULL
                110 LOAD_BUILD_CLASS
-               112 LOAD_CONST               7 (<code object ConcreteIRTModel, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 9>)
+               112 LOAD_CONST               7 (<code object ConcreteIRTModel, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 9>)
                114 MAKE_FUNCTION            0
                116 LOAD_CONST               8 ('ConcreteIRTModel')
                118 LOAD_NAME               18 (BaseIRTModel)
                120 PRECALL                  3
                124 CALL                     3
                134 STORE_NAME              19 (ConcreteIRTModel)
    
     19         136 LOAD_NAME               12 (pytest)
                138 LOAD_ATTR               20 (fixture)
    
-    20         148 LOAD_CONST               9 (<code object base_irt_model, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 19>)
+    20         148 LOAD_CONST               9 (<code object base_irt_model, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 19>)
                150 MAKE_FUNCTION            0
    
     19         152 PRECALL                  0
                156 CALL                     0
    
     20         166 STORE_NAME              21 (base_irt_model)
    
     23         168 LOAD_NAME               12 (pytest)
                170 LOAD_ATTR               20 (fixture)
    
-    24         180 LOAD_CONST              10 (<code object irt_scorer, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 23>)
+    24         180 LOAD_CONST              10 (<code object irt_scorer, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 23>)
                182 MAKE_FUNCTION            0
    
     23         184 PRECALL                  0
                188 CALL                     0
    
     24         198 STORE_NAME              22 (irt_scorer)
    
-    86         200 LOAD_NAME               12 (pytest)
-               202 LOAD_ATTR               23 (mark)
-               212 LOAD_METHOD             24 (parametrize)
-               234 LOAD_CONST              11 ('one_dimensional')
-               236 LOAD_CONST              12 (True)
-               238 LOAD_CONST              13 (False)
-               240 BUILD_LIST               2
-               242 PRECALL                  2
-               246 CALL                     2
+    85         200 LOAD_CONST               0 (0)
+               202 LOAD_CONST              11 (('patch',))
+               204 IMPORT_NAME              6 (unittest.mock)
+               206 IMPORT_FROM              8 (patch)
+               208 STORE_NAME               8 (patch)
+               210 POP_TOP
    
-    87         256 LOAD_NAME               12 (pytest)
-               258 LOAD_ATTR               23 (mark)
-               268 LOAD_METHOD             24 (parametrize)
-               290 LOAD_CONST              14 ('bit_score_z_grid_method')
-               292 LOAD_CONST              15 ('NN')
-               294 LOAD_CONST              16 ('ML')
-               296 BUILD_LIST               2
-               298 PRECALL                  2
-               302 CALL                     2
+    86         212 LOAD_CONST               0 (0)
+               214 LOAD_CONST              12 (('GaussianMixtureModel',))
+               216 IMPORT_NAME             13 (irtorch.irt_scorer)
+               218 IMPORT_FROM             23 (GaussianMixtureModel)
+               220 STORE_NAME              23 (GaussianMixtureModel)
+               222 POP_TOP
    
-    88         312 LOAD_CONST              17 ('irt_scorer')
-               314 LOAD_NAME               14 (IRTScorer)
-               316 BUILD_TUPLE              2
-               318 LOAD_CONST              18 (<code object test_bit_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 86>)
-               320 MAKE_FUNCTION            4 (annotations)
+    88         224 LOAD_NAME               12 (pytest)
+               226 LOAD_ATTR               24 (mark)
+               236 LOAD_METHOD             25 (parametrize)
+               258 LOAD_CONST              13 ('cv_n_components')
+               260 LOAD_CONST              14 (1)
+               262 BUILD_LIST               1
+               264 BUILD_LIST               0
+               266 LOAD_CONST              15 ((1, 2, 3))
+               268 LIST_EXTEND              1
+               270 BUILD_LIST               2
+               272 PRECALL                  2
+               276 CALL                     2
    
-    87         322 PRECALL                  0
-               326 CALL                     0
+    89         286 LOAD_CONST              16 ('irt_scorer')
+               288 LOAD_NAME               14 (IRTScorer)
+               290 BUILD_TUPLE              2
+               292 LOAD_CONST              17 (<code object test_cv_gaussian_mixture_model, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 88>)
+               294 MAKE_FUNCTION            4 (annotations)
    
-    86         336 PRECALL                  0
-               340 CALL                     0
+    88         296 PRECALL                  0
+               300 CALL                     0
    
-    88         350 STORE_NAME              25 (test_bit_scores)
+    89         310 STORE_NAME              26 (test_cv_gaussian_mixture_model)
    
-   118         352 LOAD_NAME               12 (pytest)
-               354 LOAD_ATTR               23 (mark)
-               364 LOAD_METHOD             24 (parametrize)
-               386 LOAD_CONST              19 ('z_estimation_method')
-               388 LOAD_CONST              15 ('NN')
-               390 LOAD_CONST              20 ('EAP')
-               392 BUILD_LIST               2
-               394 PRECALL                  2
-               398 CALL                     2
+   105         312 LOAD_NAME               12 (pytest)
+               314 LOAD_ATTR               24 (mark)
+               324 LOAD_METHOD             25 (parametrize)
+               346 LOAD_CONST              18 ('one_dimensional')
+               348 LOAD_CONST              19 (True)
+               350 LOAD_CONST              20 (False)
+               352 BUILD_LIST               2
+               354 PRECALL                  2
+               358 CALL                     2
    
-   119         408 LOAD_CONST              17 ('irt_scorer')
-               410 LOAD_NAME               14 (IRTScorer)
-               412 BUILD_TUPLE              2
-               414 LOAD_CONST              21 (<code object test_latent_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 118>)
-               416 MAKE_FUNCTION            4 (annotations)
+   106         368 LOAD_NAME               12 (pytest)
+               370 LOAD_ATTR               24 (mark)
+               380 LOAD_METHOD             25 (parametrize)
+               402 LOAD_CONST              21 ('bit_score_z_grid_method')
+               404 LOAD_CONST              22 ('NN')
+               406 LOAD_CONST              23 ('ML')
+               408 BUILD_LIST               2
+               410 PRECALL                  2
+               414 CALL                     2
    
-   118         418 PRECALL                  0
-               422 CALL                     0
+   107         424 LOAD_CONST              16 ('irt_scorer')
+               426 LOAD_NAME               14 (IRTScorer)
+               428 BUILD_TUPLE              2
+               430 LOAD_CONST              24 (<code object test_bit_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 105>)
+               432 MAKE_FUNCTION            4 (annotations)
    
-   119         432 STORE_NAME              26 (test_latent_scores)
+   106         434 PRECALL                  0
+               438 CALL                     0
    
-   138         434 LOAD_NAME               12 (pytest)
-               436 LOAD_ATTR               23 (mark)
-               446 LOAD_METHOD             24 (parametrize)
-               468 LOAD_CONST              22 ('grid_size')
-               470 BUILD_LIST               0
-               472 LOAD_CONST              23 ((3, 4, 5))
-               474 LIST_EXTEND              1
-               476 PRECALL                  2
-               480 CALL                     2
+   105         448 PRECALL                  0
+               452 CALL                     0
    
-   139         490 LOAD_CONST              17 ('irt_scorer')
-               492 LOAD_NAME               14 (IRTScorer)
-               494 BUILD_TUPLE              2
-               496 LOAD_CONST              24 (<code object test_z_grid, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 138>)
-               498 MAKE_FUNCTION            4 (annotations)
+   107         462 STORE_NAME              27 (test_bit_scores)
    
-   138         500 PRECALL                  0
-               504 CALL                     0
+   137         464 LOAD_NAME               12 (pytest)
+               466 LOAD_ATTR               24 (mark)
+               476 LOAD_METHOD             25 (parametrize)
+               498 LOAD_CONST              25 ('z_estimation_method')
+               500 LOAD_CONST              22 ('NN')
+               502 LOAD_CONST              26 ('EAP')
+               504 BUILD_LIST               2
+               506 PRECALL                  2
+               510 CALL                     2
    
-   139         514 STORE_NAME              27 (test_z_grid)
+   138         520 LOAD_CONST              16 ('irt_scorer')
+               522 LOAD_NAME               14 (IRTScorer)
+               524 BUILD_TUPLE              2
+               526 LOAD_CONST              27 (<code object test_latent_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 137>)
+               528 MAKE_FUNCTION            4 (annotations)
    
-   167         516 LOAD_CONST              17 ('irt_scorer')
-               518 LOAD_NAME               14 (IRTScorer)
-               520 BUILD_TUPLE              2
-               522 LOAD_CONST              25 (<code object test_compute_1d_bit_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 167>)
-               524 MAKE_FUNCTION            4 (annotations)
-               526 STORE_NAME              28 (test_compute_1d_bit_scores)
+   137         530 PRECALL                  0
+               534 CALL                     0
    
-   191         528 LOAD_CONST              17 ('irt_scorer')
-               530 LOAD_NAME               14 (IRTScorer)
-               532 BUILD_TUPLE              2
-               534 LOAD_CONST              26 (<code object test_compute_multi_dimensional_bit_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 191>)
-               536 MAKE_FUNCTION            4 (annotations)
-               538 STORE_NAME              29 (test_compute_multi_dimensional_bit_scores)
+   138         544 STORE_NAME              28 (test_latent_scores)
    
-   217         540 LOAD_CONST              17 ('irt_scorer')
-               542 LOAD_NAME               14 (IRTScorer)
-               544 LOAD_CONST              27 ('base_irt_model')
-               546 LOAD_NAME               18 (BaseIRTModel)
-               548 BUILD_TUPLE              4
-               550 LOAD_CONST              28 (<code object test_expected_item_score_slopes, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 217>)
-               552 MAKE_FUNCTION            4 (annotations)
-               554 STORE_NAME              30 (test_expected_item_score_slopes)
+   157         546 LOAD_NAME               12 (pytest)
+               548 LOAD_ATTR               24 (mark)
+               558 LOAD_METHOD             25 (parametrize)
+               580 LOAD_CONST              28 ('grid_size')
+               582 BUILD_LIST               0
+               584 LOAD_CONST              29 ((3, 4, 5))
+               586 LIST_EXTEND              1
+               588 PRECALL                  2
+               592 CALL                     2
    
-   234         556 LOAD_CONST              17 ('irt_scorer')
-               558 LOAD_NAME               14 (IRTScorer)
-               560 BUILD_TUPLE              2
-               562 LOAD_CONST              29 (<code object test_information, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 234>)
-               564 MAKE_FUNCTION            4 (annotations)
-               566 STORE_NAME              31 (test_information)
-               568 LOAD_CONST               1 (None)
-               570 RETURN_VALUE
+   158         602 LOAD_CONST              16 ('irt_scorer')
+               604 LOAD_NAME               14 (IRTScorer)
+               606 BUILD_TUPLE              2
+               608 LOAD_CONST              30 (<code object test_z_grid, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 157>)
+               610 MAKE_FUNCTION            4 (annotations)
+   
+   157         612 PRECALL                  0
+               616 CALL                     0
+   
+   158         626 STORE_NAME              29 (test_z_grid)
+   
+   186         628 LOAD_CONST              16 ('irt_scorer')
+               630 LOAD_NAME               14 (IRTScorer)
+               632 BUILD_TUPLE              2
+               634 LOAD_CONST              31 (<code object test_compute_1d_bit_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 186>)
+               636 MAKE_FUNCTION            4 (annotations)
+               638 STORE_NAME              30 (test_compute_1d_bit_scores)
+   
+   210         640 LOAD_CONST              16 ('irt_scorer')
+               642 LOAD_NAME               14 (IRTScorer)
+               644 BUILD_TUPLE              2
+               646 LOAD_CONST              32 (<code object test_compute_multi_dimensional_bit_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 210>)
+               648 MAKE_FUNCTION            4 (annotations)
+               650 STORE_NAME              31 (test_compute_multi_dimensional_bit_scores)
+   
+   236         652 LOAD_CONST              16 ('irt_scorer')
+               654 LOAD_NAME               14 (IRTScorer)
+               656 LOAD_CONST              33 ('base_irt_model')
+               658 LOAD_NAME               18 (BaseIRTModel)
+               660 BUILD_TUPLE              4
+               662 LOAD_CONST              34 (<code object test_expected_item_score_slopes, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 236>)
+               664 MAKE_FUNCTION            4 (annotations)
+               666 STORE_NAME              32 (test_expected_item_score_slopes)
+   
+   253         668 LOAD_CONST              16 ('irt_scorer')
+               670 LOAD_NAME               14 (IRTScorer)
+               672 BUILD_TUPLE              2
+               674 LOAD_CONST              35 (<code object test_information, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 253>)
+               676 MAKE_FUNCTION            4 (annotations)
+               678 STORE_NAME              33 (test_information)
+               680 LOAD_CONST               1 (None)
+               682 RETURN_VALUE
    consts
       0
       None
       ('MagicMock', 'patch')
       ('softmax',)
       ('IRTScorer',)
       ('AEIRT',)
@@ -249,23 +290,23 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ConcreteIRTModel')
                        8 STORE_NAME               2 (__qualname__)
          
           10          10 LOAD_CONST               1 ('\n    Concrete implementation of BaseIRTModel for testing purposes.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          13          14 LOAD_CONST               2 (<code object forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 13>)
+          13          14 LOAD_CONST               2 (<code object forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 13>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (forward)
          
           16          20 LOAD_CONST               3 ('output')
                       22 LOAD_NAME                5 (torch)
                       24 LOAD_ATTR                6 (Tensor)
                       34 BUILD_TUPLE              2
-                      36 LOAD_CONST               4 (<code object probabilities_from_output, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 16>)
+                      36 LOAD_CONST               4 (<code object probabilities_from_output, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 16>)
                       38 MAKE_FUNCTION            4 (annotations)
                       40 STORE_NAME               7 (probabilities_from_output)
                       42 LOAD_CONST               5 (None)
                       44 RETURN_VALUE
          consts
             'ConcreteIRTModel'
             '\n    Concrete implementation of BaseIRTModel for testing purposes.\n    '
@@ -281,15 +322,15 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'z')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'forward'
                firstlineno 13
                lnotab 0x0201
             'output'
             code
                argcount  : 2
                nlocals   : 2
@@ -302,24 +343,24 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'output')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'probabilities_from_output'
                firstlineno 16
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'forward', 'torch', 'Tensor', 'probabilities_from_output')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'ConcreteIRTModel'
          firstlineno 9
          lnotab 0x0a0104030603
       'ConcreteIRTModel'
       code
          argcount  : 1
          nlocals   : 1
@@ -342,15 +383,15 @@
             None
             2
             3
          names      ('ConcreteIRTModel',)
          varnames   ('latent_variables',)
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'base_irt_model'
          firstlineno 19
          lnotab 0x0202
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 7
@@ -428,32 +469,32 @@
                      240 PRECALL                  0
                      244 CALL                     0
                      254 LOAD_FAST                2 (mock_algorithm)
                      256 STORE_ATTR               9 (train_data)
          
           33         266 LOAD_CLOSURE             1 (latent_variables)
                      268 BUILD_TUPLE              1
-                     270 LOAD_CONST               7 (<code object z_scores_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 33>)
+                     270 LOAD_CONST               7 (<code object z_scores_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 33>)
                      272 MAKE_FUNCTION            8 (closure)
                      274 STORE_FAST               3 (z_scores_mock)
          
-          48         276 LOAD_CONST               8 (<code object fix_missing_values_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 48>)
+          48         276 LOAD_CONST               8 (<code object fix_missing_values_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 48>)
                      278 MAKE_FUNCTION            0
                      280 STORE_FAST               4 (fix_missing_values_mock)
          
           52         282 LOAD_CLOSURE             8 (item_categories)
                      284 BUILD_TUPLE              1
-                     286 LOAD_CONST               9 (<code object forward_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 52>)
+                     286 LOAD_CONST               9 (<code object forward_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 52>)
                      288 MAKE_FUNCTION            8 (closure)
                      290 STORE_FAST               5 (forward_mock)
          
           69         292 LOAD_CONST              13 (('none',))
                      294 LOAD_CLOSURE             8 (item_categories)
                      296 BUILD_TUPLE              1
-                     298 LOAD_CONST              11 (<code object log_likelihood_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 69>)
+                     298 LOAD_CONST              11 (<code object log_likelihood_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 69>)
                      300 MAKE_FUNCTION            9 (defaults, closure)
                      302 STORE_FAST               6 (log_likelihood_mock)
          
           72         304 LOAD_GLOBAL              1 (NULL + MagicMock)
                      316 LOAD_GLOBAL             20 (BaseIRTModel)
                      328 KW_NAMES                 3
                      330 PRECALL                  1
@@ -562,15 +603,15 @@
                             56 BUILD_LIST               1
                             58 PRECALL                  1
                             62 CALL                     1
                             72 PRECALL                  2
                             76 CALL                     2
                             86 POP_JUMP_FORWARD_IF_FALSE    82 (to 252)
                
-                37          88 LOAD_CONST               2 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 37>)
+                37          88 LOAD_CONST               2 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 37>)
                             90 MAKE_FUNCTION            0
                             92 LOAD_GLOBAL              7 (NULL + range)
                            104 LOAD_DEREF               2 (latent_variables)
                            106 PRECALL                  1
                            110 CALL                     1
                            120 GET_ITER
                            122 PRECALL                  0
@@ -602,15 +643,15 @@
                            304 BUILD_LIST               1
                            306 PRECALL                  1
                            310 CALL                     1
                            320 PRECALL                  2
                            324 CALL                     2
                            334 POP_JUMP_FORWARD_IF_FALSE    82 (to 500)
                
-                42         336 LOAD_CONST               6 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 42>)
+                42         336 LOAD_CONST               6 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 42>)
                            338 MAKE_FUNCTION            0
                            340 LOAD_GLOBAL              7 (NULL + range)
                            352 LOAD_DEREF               2 (latent_variables)
                            354 PRECALL                  1
                            358 CALL                     1
                            368 GET_ITER
                            370 PRECALL                  0
@@ -674,15 +715,15 @@
                         0
                         3
                         -3
                      names      ()
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
-                     filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+                     filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                      name       '<listcomp>'
                      firstlineno 37
                      lnotab 0x
                   0
                   1.0
                   2.0
                   code
@@ -715,23 +756,23 @@
                         0
                         -3
                         3
                      names      ()
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
-                     filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+                     filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                      name       '<listcomp>'
                      firstlineno 42
                      lnotab 0x
                names      ('torch', 'allclose', 'tensor', 'range', 'unsqueeze', 'float', 'randn', 'shape')
                varnames   ('input_tensor', 'values')
                freevars   ('latent_variables',)
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'z_scores_mock'
                firstlineno 33
                lnotab 0x0401540332017201540332017202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -743,15 +784,15 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('input_tensor',)
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'fix_missing_values_mock'
                firstlineno 48
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 7
                stacksize : 7
@@ -862,15 +903,15 @@
                   True
                   ('dim', 'return_inverse')
                   -1
                names      ('torch', 'unique', 'randn', 'shape', 'len', 'max', 'enumerate', 'inf', 'reshape')
                varnames   ('input_tensor', 'unique_rows', 'inverse_indices', 'logits_unique', 'item', 'category', 'logits_all_rows')
                freevars   ('item_categories',)
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'forward_mock'
                firstlineno 52
                lnotab 0x04023401160118011c011cfd10052801300266011002
             'none'
             code
                argcount  : 3
                nlocals   : 3
@@ -901,37 +942,676 @@
                consts
                   None
                   0
                names      ('torch', 'randn', 'shape', 'len')
                varnames   ('replicated_data', 'replicated_logits', 'loss_reduction')
                freevars   ('item_categories',)
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'log_likelihood_mock'
                firstlineno 69
                lnotab 0x0401
             ('side_effect',)
             ('none',)
          names      ('MagicMock', 'AEIRT', 'one_hot_encoded', 'clone', 'detach', 'training_z_scores', 'torch', 'tensor', 'float', 'train_data', 'BaseIRTModel', 'mc_correct', 'latent_variables', 'item_categories', 'modeled_item_responses', 'side_effect', 'model_missing', 'log_likelihood', 'z_scores', 'fix_missing_values', 'IRTScorer')
          varnames   ('z_scores', 'latent_variables', 'mock_algorithm', 'z_scores_mock', 'fix_missing_values_mock', 'forward_mock', 'log_likelihood_mock', 'mock_model')
          freevars   ()
          cellvars   ('latent_variables', 'item_categories')
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'irt_scorer'
          firstlineno 23
          lnotab
             0x060308012a010e0156016e030a0f06040a110c032a010e010e010e010e
             010e010e012a012a012a02
+      ('patch',)
+      ('GaussianMixtureModel',)
+      'cv_n_components'
+      1
+      (1, 2, 3)
+      'irt_scorer'
+      code
+         argcount  : 2
+         nlocals   : 17
+         stacksize : 9
+         flags     : 3
+         code
+            0x97007401000000000000000000006a01000000000000000064017c006a
+            0200000000000000006a030000000000000000a6020000ab020000000000
+            0000007d027409000000000000000000006a050000000000000000740c00
+            0000000000000000006402a6020000ab02000000000000000035007d0374
+            09000000000000000000006a050000000000000000740c00000000000000
+            0000006403a6020000ab02000000000000000035007d0464007c035f0700
+            000000000000007401000000000000000000006a08000000000000000064
+            04a6010000ab0100000000000000007c045f0700000000000000007c00a0
+            0900000000000000000000000000000000000000007c027c01a6020000ab
+            0200000000000000007d05640064006400a6020000ab0200000000000000
+            0001006e0b23003100730477027803590077010100590001000100640064
+            006400a6020000ab02000000000000000001006e0b230031007304770278
+            035900770101005900010001007415000000000000000000007c05740c00
+            000000000000000000a6020000ab0200000000000000007d067c06900173
+            08640564067417000000000000000000006a0c0000000000000000a60000
+            00ab00000000000000000076007319741b000000000000000000006a0e00
+            00000000000000741400000000000000000000a6010000ab010000000000
+            0000007219741b000000000000000000006a0f0000000000000000741400
+            000000000000000000a6010000ab0100000000000000006e016406640774
+            17000000000000000000006a0c0000000000000000a6000000ab00000000
+            000000000076007314741b000000000000000000006a0e00000000000000
+            007c05a6010000ab0100000000000000007214741b000000000000000000
+            006a0f00000000000000007c05a6010000ab0100000000000000006e0164
+            0764087417000000000000000000006a0c0000000000000000a6000000ab
+            00000000000000000076007319741b000000000000000000006a0e000000
+            0000000000740c00000000000000000000a6010000ab0100000000000000
+            007219741b000000000000000000006a0f0000000000000000740c000000
+            00000000000000a6010000ab0100000000000000006e016408741b000000
+            000000000000006a0f00000000000000007c06a6010000ab010000000000
+            00000064099c047a0600007d07742100000000000000000000741b000000
+            000000000000006a1100000000000000007c07a6010000ab010000000000
+            000000a6010000ab010000000000000000820164007d067c056a12000000
+            00000000007d087c01640a190000000000000000007d097c087c096b0200
+            0000007d067c0673aa741b000000000000000000006a1300000000000000
+            00640b7c066601640c7c087c096602a6040000ab04000000000000000064
+            077417000000000000000000006a0c0000000000000000a6000000ab0000
+            0000000000000076007314741b000000000000000000006a0e0000000000
+            0000007c05a6010000ab0100000000000000007214741b00000000000000
+            0000006a0f00000000000000007c05a6010000ab0100000000000000006e
+            016407741b000000000000000000006a0f00000000000000007c08a60100
+            00ab010000000000000000741b000000000000000000006a0f0000000000
+            0000007c09a6010000ab010000000000000000640d9c037a0600007d0a64
+            0e640f7c0a69017a0600007d0b742100000000000000000000741b000000
+            000000000000006a1100000000000000007c0ba6010000ab010000000000
+            000000a6010000ab0100000000000000008201640078017d0878017d067d
+            097c056a1400000000000000007d087c026a150000000000000000641019
+            0000000000000000007d097c087c096b02000000007d067c0673aa741b00
+            0000000000000000006a130000000000000000640b7c06660164117c087c
+            096602a6040000ab04000000000000000064077417000000000000000000
+            006a0c0000000000000000a6000000ab0000000000000000007600731474
+            1b000000000000000000006a0e00000000000000007c05a6010000ab0100
+            000000000000007214741b000000000000000000006a0f00000000000000
+            007c05a6010000ab0100000000000000006e016407741b00000000000000
+            0000006a0f00000000000000007c08a6010000ab01000000000000000074
+            1b000000000000000000006a0f00000000000000007c09a6010000ab0100
+            00000000000000640d9c037a0600007d0a640e640f7c0a69017a0600007d
+            0b742100000000000000000000741b000000000000000000006a11000000
+            00000000007c0ba6010000ab010000000000000000a6010000ab01000000
+            00000000008201640078017d0878017d067d097c03a01600000000000000
+            00000000000000000000000000a6000000ab000000000000000000010074
+            2f000000000000000000007c01a6010000ab01000000000000000064106b
+            0400000000900172757c046a1800000000000000007d08742f0000000000
+            00000000007c01a6010000ab0100000000000000007d0c64127d0d7c0c7c
+            0d7a0500007d0e7c087c0e6b02000000007d067c0690017343741b000000
+            000000000000006a130000000000000000640b7c06660164137c087c0e66
+            02a6040000ab04000000000000000064147417000000000000000000006a
+            0c0000000000000000a6000000ab00000000000000000076007314741b00
+            0000000000000000006a0e00000000000000007c04a6010000ab01000000
+            00000000007214741b000000000000000000006a0f00000000000000007c
+            04a6010000ab0100000000000000006e016414741b000000000000000000
+            006a0f00000000000000007c08a6010000ab010000000000000000641574
+            17000000000000000000006a0c0000000000000000a6000000ab00000000
+            000000000076007319741b000000000000000000006a0e00000000000000
+            00742e00000000000000000000a6010000ab010000000000000000721974
+            1b000000000000000000006a0f0000000000000000742e00000000000000
+            000000a6010000ab0100000000000000006e016415641674170000000000
+            00000000006a0c0000000000000000a6000000ab00000000000000000076
+            007314741b000000000000000000006a0e00000000000000007c01a60100
+            00ab0100000000000000007214741b000000000000000000006a0f000000
+            00000000007c01a6010000ab0100000000000000006e016416741b000000
+            000000000000006a0f00000000000000007c0ca6010000ab010000000000
+            000000741b000000000000000000006a0f00000000000000007c0da60100
+            00ab01000000000000000064179c067a0600007d0f641864197c0f69017a
+            0600007d10742100000000000000000000741b000000000000000000006a
+            1100000000000000007c10a6010000ab010000000000000000a6010000ab
+            0100000000000000008201640078017d0878017d0678017d0c78017d0d7d
+            0e6400530064005300
+          88           0 RESUME                   0
+         
+          90           2 LOAD_GLOBAL              1 (NULL + torch)
+                      14 LOAD_ATTR                1 (randn)
+                      24 LOAD_CONST               1 (100)
+                      26 LOAD_FAST                0 (irt_scorer)
+                      28 LOAD_ATTR                2 (model)
+                      38 LOAD_ATTR                3 (latent_variables)
+                      48 PRECALL                  2
+                      52 CALL                     2
+                      62 STORE_FAST               2 (data)
+         
+          92          64 LOAD_GLOBAL              9 (NULL + patch)
+                      76 LOAD_ATTR                5 (object)
+                      86 LOAD_GLOBAL             12 (GaussianMixtureModel)
+                      98 LOAD_CONST               2 ('fit')
+                     100 PRECALL                  2
+                     104 CALL                     2
+                     114 BEFORE_WITH
+                     116 STORE_FAST               3 (mock_fit)
+                     118 LOAD_GLOBAL              9 (NULL + patch)
+                     130 LOAD_ATTR                5 (object)
+                     140 LOAD_GLOBAL             12 (GaussianMixtureModel)
+                     152 LOAD_CONST               3 ('__call__')
+                     154 PRECALL                  2
+                     158 CALL                     2
+                     168 BEFORE_WITH
+                     170 STORE_FAST               4 (mock_call)
+         
+          93         172 LOAD_CONST               0 (None)
+                     174 LOAD_FAST                3 (mock_fit)
+                     176 STORE_ATTR               7 (return_value)
+         
+          94         186 LOAD_GLOBAL              1 (NULL + torch)
+                     198 LOAD_ATTR                8 (tensor)
+                     208 LOAD_CONST               4 (1.0)
+                     210 PRECALL                  1
+                     214 CALL                     1
+                     224 LOAD_FAST                4 (mock_call)
+                     226 STORE_ATTR               7 (return_value)
+         
+          96         236 LOAD_FAST                0 (irt_scorer)
+                     238 LOAD_METHOD              9 (_cv_gaussian_mixture_model)
+                     260 LOAD_FAST                2 (data)
+                     262 LOAD_FAST                1 (cv_n_components)
+                     264 PRECALL                  2
+                     268 CALL                     2
+                     278 STORE_FAST               5 (gmm)
+         
+          92         280 LOAD_CONST               0 (None)
+                     282 LOAD_CONST               0 (None)
+                     284 LOAD_CONST               0 (None)
+                     286 PRECALL                  2
+                     290 CALL                     2
+                     300 POP_TOP
+                     302 JUMP_FORWARD            11 (to 326)
+                 >>  304 PUSH_EXC_INFO
+                     306 WITH_EXCEPT_START
+                     308 POP_JUMP_FORWARD_IF_TRUE     4 (to 318)
+                     310 RERAISE                  2
+                 >>  312 COPY                     3
+                     314 POP_EXCEPT
+                     316 RERAISE                  1
+                 >>  318 POP_TOP
+                     320 POP_EXCEPT
+                     322 POP_TOP
+                     324 POP_TOP
+                 >>  326 LOAD_CONST               0 (None)
+                     328 LOAD_CONST               0 (None)
+                     330 LOAD_CONST               0 (None)
+                     332 PRECALL                  2
+                     336 CALL                     2
+                     346 POP_TOP
+                     348 JUMP_FORWARD            11 (to 372)
+                 >>  350 PUSH_EXC_INFO
+                     352 WITH_EXCEPT_START
+                     354 POP_JUMP_FORWARD_IF_TRUE     4 (to 364)
+                     356 RERAISE                  2
+                 >>  358 COPY                     3
+                     360 POP_EXCEPT
+                     362 RERAISE                  1
+                 >>  364 POP_TOP
+                     366 POP_EXCEPT
+                     368 POP_TOP
+                     370 POP_TOP
+         
+          98     >>  372 LOAD_GLOBAL             21 (NULL + isinstance)
+                     384 LOAD_FAST                5 (gmm)
+                     386 LOAD_GLOBAL             12 (GaussianMixtureModel)
+                     398 PRECALL                  2
+                     402 CALL                     2
+                     412 STORE_FAST               6 (@py_assert3)
+                     414 LOAD_FAST                6 (@py_assert3)
+                     416 EXTENDED_ARG             1
+                     418 POP_JUMP_FORWARD_IF_TRUE   264 (to 948)
+                     420 LOAD_CONST               5 ('assert %(py4)s\n{%(py4)s = %(py0)s(%(py1)s, %(py2)s)\n}')
+                     422 LOAD_CONST               6 ('isinstance')
+                     424 LOAD_GLOBAL             23 (NULL + @py_builtins)
+                     436 LOAD_ATTR               12 (locals)
+                     446 PRECALL                  0
+                     450 CALL                     0
+                     460 CONTAINS_OP              0
+                     462 POP_JUMP_FORWARD_IF_TRUE    25 (to 514)
+                     464 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                     476 LOAD_ATTR               14 (_should_repr_global_name)
+                     486 LOAD_GLOBAL             20 (isinstance)
+                     498 PRECALL                  1
+                     502 CALL                     1
+                     512 POP_JUMP_FORWARD_IF_FALSE    25 (to 564)
+                 >>  514 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                     526 LOAD_ATTR               15 (_saferepr)
+                     536 LOAD_GLOBAL             20 (isinstance)
+                     548 PRECALL                  1
+                     552 CALL                     1
+                     562 JUMP_FORWARD             1 (to 566)
+                 >>  564 LOAD_CONST               6 ('isinstance')
+                 >>  566 LOAD_CONST               7 ('gmm')
+                     568 LOAD_GLOBAL             23 (NULL + @py_builtins)
+                     580 LOAD_ATTR               12 (locals)
+                     590 PRECALL                  0
+                     594 CALL                     0
+                     604 CONTAINS_OP              0
+                     606 POP_JUMP_FORWARD_IF_TRUE    20 (to 648)
+                     608 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                     620 LOAD_ATTR               14 (_should_repr_global_name)
+                     630 LOAD_FAST                5 (gmm)
+                     632 PRECALL                  1
+                     636 CALL                     1
+                     646 POP_JUMP_FORWARD_IF_FALSE    20 (to 688)
+                 >>  648 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                     660 LOAD_ATTR               15 (_saferepr)
+                     670 LOAD_FAST                5 (gmm)
+                     672 PRECALL                  1
+                     676 CALL                     1
+                     686 JUMP_FORWARD             1 (to 690)
+                 >>  688 LOAD_CONST               7 ('gmm')
+                 >>  690 LOAD_CONST               8 ('GaussianMixtureModel')
+                     692 LOAD_GLOBAL             23 (NULL + @py_builtins)
+                     704 LOAD_ATTR               12 (locals)
+                     714 PRECALL                  0
+                     718 CALL                     0
+                     728 CONTAINS_OP              0
+                     730 POP_JUMP_FORWARD_IF_TRUE    25 (to 782)
+                     732 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                     744 LOAD_ATTR               14 (_should_repr_global_name)
+                     754 LOAD_GLOBAL             12 (GaussianMixtureModel)
+                     766 PRECALL                  1
+                     770 CALL                     1
+                     780 POP_JUMP_FORWARD_IF_FALSE    25 (to 832)
+                 >>  782 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                     794 LOAD_ATTR               15 (_saferepr)
+                     804 LOAD_GLOBAL             12 (GaussianMixtureModel)
+                     816 PRECALL                  1
+                     820 CALL                     1
+                     830 JUMP_FORWARD             1 (to 834)
+                 >>  832 LOAD_CONST               8 ('GaussianMixtureModel')
+                 >>  834 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                     846 LOAD_ATTR               15 (_saferepr)
+                     856 LOAD_FAST                6 (@py_assert3)
+                     858 PRECALL                  1
+                     862 CALL                     1
+                     872 LOAD_CONST               9 (('py0', 'py1', 'py2', 'py4'))
+                     874 BUILD_CONST_KEY_MAP      4
+                     876 BINARY_OP                6 (%)
+                     880 STORE_FAST               7 (@py_format5)
+                     882 LOAD_GLOBAL             33 (NULL + AssertionError)
+                     894 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                     906 LOAD_ATTR               17 (_format_explanation)
+                     916 LOAD_FAST                7 (@py_format5)
+                     918 PRECALL                  1
+                     922 CALL                     1
+                     932 PRECALL                  1
+                     936 CALL                     1
+                     946 RAISE_VARARGS            1
+                 >>  948 LOAD_CONST               0 (None)
+                     950 STORE_FAST               6 (@py_assert3)
+         
+          99         952 LOAD_FAST                5 (gmm)
+                     954 LOAD_ATTR               18 (n_components)
+                     964 STORE_FAST               8 (@py_assert1)
+                     966 LOAD_FAST                1 (cv_n_components)
+                     968 LOAD_CONST              10 (0)
+                     970 BINARY_SUBSCR
+                     980 STORE_FAST               9 (@py_assert4)
+                     982 LOAD_FAST                8 (@py_assert1)
+                     984 LOAD_FAST                9 (@py_assert4)
+                     986 COMPARE_OP               2 (==)
+                     992 STORE_FAST               6 (@py_assert3)
+                     994 LOAD_FAST                6 (@py_assert3)
+                     996 POP_JUMP_FORWARD_IF_TRUE   170 (to 1338)
+                     998 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1010 LOAD_ATTR               19 (_call_reprcompare)
+                    1020 LOAD_CONST              11 (('==',))
+                    1022 LOAD_FAST                6 (@py_assert3)
+                    1024 BUILD_TUPLE              1
+                    1026 LOAD_CONST              12 (('%(py2)s\n{%(py2)s = %(py0)s.n_components\n} == %(py5)s',))
+                    1028 LOAD_FAST                8 (@py_assert1)
+                    1030 LOAD_FAST                9 (@py_assert4)
+                    1032 BUILD_TUPLE              2
+                    1034 PRECALL                  4
+                    1038 CALL                     4
+                    1048 LOAD_CONST               7 ('gmm')
+                    1050 LOAD_GLOBAL             23 (NULL + @py_builtins)
+                    1062 LOAD_ATTR               12 (locals)
+                    1072 PRECALL                  0
+                    1076 CALL                     0
+                    1086 CONTAINS_OP              0
+                    1088 POP_JUMP_FORWARD_IF_TRUE    20 (to 1130)
+                    1090 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1102 LOAD_ATTR               14 (_should_repr_global_name)
+                    1112 LOAD_FAST                5 (gmm)
+                    1114 PRECALL                  1
+                    1118 CALL                     1
+                    1128 POP_JUMP_FORWARD_IF_FALSE    20 (to 1170)
+                 >> 1130 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1142 LOAD_ATTR               15 (_saferepr)
+                    1152 LOAD_FAST                5 (gmm)
+                    1154 PRECALL                  1
+                    1158 CALL                     1
+                    1168 JUMP_FORWARD             1 (to 1172)
+                 >> 1170 LOAD_CONST               7 ('gmm')
+                 >> 1172 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1184 LOAD_ATTR               15 (_saferepr)
+                    1194 LOAD_FAST                8 (@py_assert1)
+                    1196 PRECALL                  1
+                    1200 CALL                     1
+                    1210 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1222 LOAD_ATTR               15 (_saferepr)
+                    1232 LOAD_FAST                9 (@py_assert4)
+                    1234 PRECALL                  1
+                    1238 CALL                     1
+                    1248 LOAD_CONST              13 (('py0', 'py2', 'py5'))
+                    1250 BUILD_CONST_KEY_MAP      3
+                    1252 BINARY_OP                6 (%)
+                    1256 STORE_FAST              10 (@py_format6)
+                    1258 LOAD_CONST              14 ('assert %(py7)s')
+                    1260 LOAD_CONST              15 ('py7')
+                    1262 LOAD_FAST               10 (@py_format6)
+                    1264 BUILD_MAP                1
+                    1266 BINARY_OP                6 (%)
+                    1270 STORE_FAST              11 (@py_format8)
+                    1272 LOAD_GLOBAL             33 (NULL + AssertionError)
+                    1284 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1296 LOAD_ATTR               17 (_format_explanation)
+                    1306 LOAD_FAST               11 (@py_format8)
+                    1308 PRECALL                  1
+                    1312 CALL                     1
+                    1322 PRECALL                  1
+                    1326 CALL                     1
+                    1336 RAISE_VARARGS            1
+                 >> 1338 LOAD_CONST               0 (None)
+                    1340 COPY                     1
+                    1342 STORE_FAST               8 (@py_assert1)
+                    1344 COPY                     1
+                    1346 STORE_FAST               6 (@py_assert3)
+                    1348 STORE_FAST               9 (@py_assert4)
+         
+         100        1350 LOAD_FAST                5 (gmm)
+                    1352 LOAD_ATTR               20 (n_features)
+                    1362 STORE_FAST               8 (@py_assert1)
+                    1364 LOAD_FAST                2 (data)
+                    1366 LOAD_ATTR               21 (shape)
+                    1376 LOAD_CONST              16 (1)
+                    1378 BINARY_SUBSCR
+                    1388 STORE_FAST               9 (@py_assert4)
+                    1390 LOAD_FAST                8 (@py_assert1)
+                    1392 LOAD_FAST                9 (@py_assert4)
+                    1394 COMPARE_OP               2 (==)
+                    1400 STORE_FAST               6 (@py_assert3)
+                    1402 LOAD_FAST                6 (@py_assert3)
+                    1404 POP_JUMP_FORWARD_IF_TRUE   170 (to 1746)
+                    1406 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1418 LOAD_ATTR               19 (_call_reprcompare)
+                    1428 LOAD_CONST              11 (('==',))
+                    1430 LOAD_FAST                6 (@py_assert3)
+                    1432 BUILD_TUPLE              1
+                    1434 LOAD_CONST              17 (('%(py2)s\n{%(py2)s = %(py0)s.n_features\n} == %(py5)s',))
+                    1436 LOAD_FAST                8 (@py_assert1)
+                    1438 LOAD_FAST                9 (@py_assert4)
+                    1440 BUILD_TUPLE              2
+                    1442 PRECALL                  4
+                    1446 CALL                     4
+                    1456 LOAD_CONST               7 ('gmm')
+                    1458 LOAD_GLOBAL             23 (NULL + @py_builtins)
+                    1470 LOAD_ATTR               12 (locals)
+                    1480 PRECALL                  0
+                    1484 CALL                     0
+                    1494 CONTAINS_OP              0
+                    1496 POP_JUMP_FORWARD_IF_TRUE    20 (to 1538)
+                    1498 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1510 LOAD_ATTR               14 (_should_repr_global_name)
+                    1520 LOAD_FAST                5 (gmm)
+                    1522 PRECALL                  1
+                    1526 CALL                     1
+                    1536 POP_JUMP_FORWARD_IF_FALSE    20 (to 1578)
+                 >> 1538 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1550 LOAD_ATTR               15 (_saferepr)
+                    1560 LOAD_FAST                5 (gmm)
+                    1562 PRECALL                  1
+                    1566 CALL                     1
+                    1576 JUMP_FORWARD             1 (to 1580)
+                 >> 1578 LOAD_CONST               7 ('gmm')
+                 >> 1580 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1592 LOAD_ATTR               15 (_saferepr)
+                    1602 LOAD_FAST                8 (@py_assert1)
+                    1604 PRECALL                  1
+                    1608 CALL                     1
+                    1618 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1630 LOAD_ATTR               15 (_saferepr)
+                    1640 LOAD_FAST                9 (@py_assert4)
+                    1642 PRECALL                  1
+                    1646 CALL                     1
+                    1656 LOAD_CONST              13 (('py0', 'py2', 'py5'))
+                    1658 BUILD_CONST_KEY_MAP      3
+                    1660 BINARY_OP                6 (%)
+                    1664 STORE_FAST              10 (@py_format6)
+                    1666 LOAD_CONST              14 ('assert %(py7)s')
+                    1668 LOAD_CONST              15 ('py7')
+                    1670 LOAD_FAST               10 (@py_format6)
+                    1672 BUILD_MAP                1
+                    1674 BINARY_OP                6 (%)
+                    1678 STORE_FAST              11 (@py_format8)
+                    1680 LOAD_GLOBAL             33 (NULL + AssertionError)
+                    1692 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1704 LOAD_ATTR               17 (_format_explanation)
+                    1714 LOAD_FAST               11 (@py_format8)
+                    1716 PRECALL                  1
+                    1720 CALL                     1
+                    1730 PRECALL                  1
+                    1734 CALL                     1
+                    1744 RAISE_VARARGS            1
+                 >> 1746 LOAD_CONST               0 (None)
+                    1748 COPY                     1
+                    1750 STORE_FAST               8 (@py_assert1)
+                    1752 COPY                     1
+                    1754 STORE_FAST               6 (@py_assert3)
+                    1756 STORE_FAST               9 (@py_assert4)
+         
+         101        1758 LOAD_FAST                3 (mock_fit)
+                    1760 LOAD_METHOD             22 (assert_called)
+                    1782 PRECALL                  0
+                    1786 CALL                     0
+                    1796 POP_TOP
+         
+         102        1798 LOAD_GLOBAL             47 (NULL + len)
+                    1810 LOAD_FAST                1 (cv_n_components)
+                    1812 PRECALL                  1
+                    1816 CALL                     1
+                    1826 LOAD_CONST              16 (1)
+                    1828 COMPARE_OP               4 (>)
+                    1834 EXTENDED_ARG             1
+                    1836 POP_JUMP_FORWARD_IF_FALSE   373 (to 2584)
+         
+         103        1838 LOAD_FAST                4 (mock_call)
+                    1840 LOAD_ATTR               24 (call_count)
+                    1850 STORE_FAST               8 (@py_assert1)
+                    1852 LOAD_GLOBAL             47 (NULL + len)
+                    1864 LOAD_FAST                1 (cv_n_components)
+                    1866 PRECALL                  1
+                    1870 CALL                     1
+                    1880 STORE_FAST              12 (@py_assert6)
+                    1882 LOAD_CONST              18 (5)
+                    1884 STORE_FAST              13 (@py_assert8)
+                    1886 LOAD_FAST               12 (@py_assert6)
+                    1888 LOAD_FAST               13 (@py_assert8)
+                    1890 BINARY_OP                5 (*)
+                    1894 STORE_FAST              14 (@py_assert10)
+                    1896 LOAD_FAST                8 (@py_assert1)
+                    1898 LOAD_FAST               14 (@py_assert10)
+                    1900 COMPARE_OP               2 (==)
+                    1906 STORE_FAST               6 (@py_assert3)
+                    1908 LOAD_FAST                6 (@py_assert3)
+                    1910 EXTENDED_ARG             1
+                    1912 POP_JUMP_FORWARD_IF_TRUE   323 (to 2560)
+                    1914 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    1926 LOAD_ATTR               19 (_call_reprcompare)
+                    1936 LOAD_CONST              11 (('==',))
+                    1938 LOAD_FAST                6 (@py_assert3)
+                    1940 BUILD_TUPLE              1
+                    1942 LOAD_CONST              19 (('%(py2)s\n{%(py2)s = %(py0)s.call_count\n} == (%(py7)s\n{%(py7)s = %(py4)s(%(py5)s)\n} * %(py9)s)',))
+                    1944 LOAD_FAST                8 (@py_assert1)
+                    1946 LOAD_FAST               14 (@py_assert10)
+                    1948 BUILD_TUPLE              2
+                    1950 PRECALL                  4
+                    1954 CALL                     4
+                    1964 LOAD_CONST              20 ('mock_call')
+                    1966 LOAD_GLOBAL             23 (NULL + @py_builtins)
+                    1978 LOAD_ATTR               12 (locals)
+                    1988 PRECALL                  0
+                    1992 CALL                     0
+                    2002 CONTAINS_OP              0
+                    2004 POP_JUMP_FORWARD_IF_TRUE    20 (to 2046)
+                    2006 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2018 LOAD_ATTR               14 (_should_repr_global_name)
+                    2028 LOAD_FAST                4 (mock_call)
+                    2030 PRECALL                  1
+                    2034 CALL                     1
+                    2044 POP_JUMP_FORWARD_IF_FALSE    20 (to 2086)
+                 >> 2046 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2058 LOAD_ATTR               15 (_saferepr)
+                    2068 LOAD_FAST                4 (mock_call)
+                    2070 PRECALL                  1
+                    2074 CALL                     1
+                    2084 JUMP_FORWARD             1 (to 2088)
+                 >> 2086 LOAD_CONST              20 ('mock_call')
+                 >> 2088 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2100 LOAD_ATTR               15 (_saferepr)
+                    2110 LOAD_FAST                8 (@py_assert1)
+                    2112 PRECALL                  1
+                    2116 CALL                     1
+                    2126 LOAD_CONST              21 ('len')
+                    2128 LOAD_GLOBAL             23 (NULL + @py_builtins)
+                    2140 LOAD_ATTR               12 (locals)
+                    2150 PRECALL                  0
+                    2154 CALL                     0
+                    2164 CONTAINS_OP              0
+                    2166 POP_JUMP_FORWARD_IF_TRUE    25 (to 2218)
+                    2168 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2180 LOAD_ATTR               14 (_should_repr_global_name)
+                    2190 LOAD_GLOBAL             46 (len)
+                    2202 PRECALL                  1
+                    2206 CALL                     1
+                    2216 POP_JUMP_FORWARD_IF_FALSE    25 (to 2268)
+                 >> 2218 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2230 LOAD_ATTR               15 (_saferepr)
+                    2240 LOAD_GLOBAL             46 (len)
+                    2252 PRECALL                  1
+                    2256 CALL                     1
+                    2266 JUMP_FORWARD             1 (to 2270)
+                 >> 2268 LOAD_CONST              21 ('len')
+                 >> 2270 LOAD_CONST              22 ('cv_n_components')
+                    2272 LOAD_GLOBAL             23 (NULL + @py_builtins)
+                    2284 LOAD_ATTR               12 (locals)
+                    2294 PRECALL                  0
+                    2298 CALL                     0
+                    2308 CONTAINS_OP              0
+                    2310 POP_JUMP_FORWARD_IF_TRUE    20 (to 2352)
+                    2312 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2324 LOAD_ATTR               14 (_should_repr_global_name)
+                    2334 LOAD_FAST                1 (cv_n_components)
+                    2336 PRECALL                  1
+                    2340 CALL                     1
+                    2350 POP_JUMP_FORWARD_IF_FALSE    20 (to 2392)
+                 >> 2352 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2364 LOAD_ATTR               15 (_saferepr)
+                    2374 LOAD_FAST                1 (cv_n_components)
+                    2376 PRECALL                  1
+                    2380 CALL                     1
+                    2390 JUMP_FORWARD             1 (to 2394)
+                 >> 2392 LOAD_CONST              22 ('cv_n_components')
+                 >> 2394 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2406 LOAD_ATTR               15 (_saferepr)
+                    2416 LOAD_FAST               12 (@py_assert6)
+                    2418 PRECALL                  1
+                    2422 CALL                     1
+                    2432 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2444 LOAD_ATTR               15 (_saferepr)
+                    2454 LOAD_FAST               13 (@py_assert8)
+                    2456 PRECALL                  1
+                    2460 CALL                     1
+                    2470 LOAD_CONST              23 (('py0', 'py2', 'py4', 'py5', 'py7', 'py9'))
+                    2472 BUILD_CONST_KEY_MAP      6
+                    2474 BINARY_OP                6 (%)
+                    2478 STORE_FAST              15 (@py_format11)
+                    2480 LOAD_CONST              24 ('assert %(py12)s')
+                    2482 LOAD_CONST              25 ('py12')
+                    2484 LOAD_FAST               15 (@py_format11)
+                    2486 BUILD_MAP                1
+                    2488 BINARY_OP                6 (%)
+                    2492 STORE_FAST              16 (@py_format13)
+                    2494 LOAD_GLOBAL             33 (NULL + AssertionError)
+                    2506 LOAD_GLOBAL             27 (NULL + @pytest_ar)
+                    2518 LOAD_ATTR               17 (_format_explanation)
+                    2528 LOAD_FAST               16 (@py_format13)
+                    2530 PRECALL                  1
+                    2534 CALL                     1
+                    2544 PRECALL                  1
+                    2548 CALL                     1
+                    2558 RAISE_VARARGS            1
+                 >> 2560 LOAD_CONST               0 (None)
+                    2562 COPY                     1
+                    2564 STORE_FAST               8 (@py_assert1)
+                    2566 COPY                     1
+                    2568 STORE_FAST               6 (@py_assert3)
+                    2570 COPY                     1
+                    2572 STORE_FAST              12 (@py_assert6)
+                    2574 COPY                     1
+                    2576 STORE_FAST              13 (@py_assert8)
+                    2578 STORE_FAST              14 (@py_assert10)
+                    2580 LOAD_CONST               0 (None)
+                    2582 RETURN_VALUE
+         
+         102     >> 2584 LOAD_CONST               0 (None)
+                    2586 RETURN_VALUE
+         ExceptionTable:
+           116 to 168 -> 350 [1] lasti
+           170 to 278 -> 304 [2] lasti
+           280 to 302 -> 350 [1] lasti
+           304 to 310 -> 312 [4] lasti
+           312 to 316 -> 350 [1] lasti
+           318 to 318 -> 312 [4] lasti
+           320 to 324 -> 350 [1] lasti
+           350 to 356 -> 358 [3] lasti
+           364 to 364 -> 358 [3] lasti
+         consts
+            None
+            100
+            'fit'
+            '__call__'
+            1.0
+            'assert %(py4)s\n{%(py4)s = %(py0)s(%(py1)s, %(py2)s)\n}'
+            'isinstance'
+            'gmm'
+            'GaussianMixtureModel'
+            ('py0', 'py1', 'py2', 'py4')
+            0
+            ('==',)
+            ('%(py2)s\n{%(py2)s = %(py0)s.n_components\n} == %(py5)s',)
+            ('py0', 'py2', 'py5')
+            'assert %(py7)s'
+            'py7'
+            1
+            ('%(py2)s\n{%(py2)s = %(py0)s.n_features\n} == %(py5)s',)
+            5
+            ('%(py2)s\n{%(py2)s = %(py0)s.call_count\n} == (%(py7)s\n{%(py7)s = %(py4)s(%(py5)s)\n} * %(py9)s)',)
+            'mock_call'
+            'len'
+            'cv_n_components'
+            ('py0', 'py2', 'py4', 'py5', 'py7', 'py9')
+            'assert %(py12)s'
+            'py12'
+         names      ('torch', 'randn', 'model', 'latent_variables', 'patch', 'object', 'GaussianMixtureModel', 'return_value', 'tensor', '_cv_gaussian_mixture_model', 'isinstance', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'n_components', '_call_reprcompare', 'n_features', 'shape', 'assert_called', 'len', 'call_count')
+         varnames   ('irt_scorer', 'cv_n_components', 'data', 'mock_fit', 'mock_call', 'gmm', '@py_assert3', '@py_format5', '@py_assert1', '@py_assert4', '@py_format6', '@py_format8', '@py_assert6', '@py_assert8', '@py_assert10', '@py_format11', '@py_format13')
+         freevars   ()
+         cellvars   ()
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
+         name       'test_cv_gaussian_mixture_model'
+         firstlineno 88
+         lnotab
+            0x02023e026c010e0132022cfc5c06ff00ff004601ff008f01ff00990128
+            012801ff00ff00ecff
       'one_dimensional'
       True
       False
       'bit_score_z_grid_method'
       'NN'
       'ML'
-      'irt_scorer'
       code
          argcount  : 4
          nlocals   : 17
          stacksize : 13
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000006401670164
@@ -1004,17 +1684,17 @@
             010000000000000000a6010000ab0100000000000000008201640078017d
             0c78017d0e7d0d7c03641d6b020000000072467c06a01400000000000000
             000000000000000000000000007c006a1500000000000000006a16000000
             0000000000641e641d7400000000000000000000006a1700000000000000
             00a0180000000000000000000000000000000000000000a6000000ab0000
             000000000000007202641f6e0164206421ac22a6050000ab050000000000
             00000001006400530064005300
-          86           0 RESUME                   0
+         105           0 RESUME                   0
          
-          89           2 LOAD_GLOBAL              1 (NULL + torch)
+         108           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (tensor)
                       24 LOAD_CONST               1 (0.8)
                       26 BUILD_LIST               1
                       28 LOAD_CONST               2 (2.1)
                       30 BUILD_LIST               1
                       32 LOAD_CONST               3 (-0.7)
                       34 BUILD_LIST               1
@@ -1026,35 +1706,35 @@
                       56 LOAD_METHOD              2 (repeat)
                       78 LOAD_CONST               5 (1)
                       80 LOAD_FAST                2 (latent_variables)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 STORE_FAST               4 (z)
          
-          90          98 LOAD_FAST                4 (z)
+         109          98 LOAD_FAST                4 (z)
                      100 LOAD_CONST               5 (1)
                      102 LOAD_CONST               0 (None)
                      104 LOAD_CONST               6 (2)
                      106 BUILD_SLICE              3
                      108 BINARY_SUBSCR
                      118 LOAD_CONST               7 (-1)
                      120 BINARY_OP                5 (*)
                      124 STORE_FAST               4 (z)
          
-          91         126 LOAD_GLOBAL              1 (NULL + torch)
+         110         126 LOAD_GLOBAL              1 (NULL + torch)
                      138 LOAD_ATTR                3 (full)
                      148 LOAD_CONST               5 (1)
                      150 LOAD_FAST                2 (latent_variables)
                      152 BUILD_TUPLE              2
                      154 LOAD_CONST               8 (-0.2)
                      156 PRECALL                  2
                      160 CALL                     2
                      170 STORE_FAST               5 (start_z)
          
-          94         172 LOAD_GLOBAL              9 (NULL + patch)
+         113         172 LOAD_GLOBAL              9 (NULL + patch)
                      184 LOAD_ATTR                5 (object)
                      194 LOAD_GLOBAL             12 (IRTScorer)
                      206 LOAD_CONST               9 ('latent_scores')
                      208 LOAD_GLOBAL              1 (NULL + torch)
                      220 LOAD_ATTR                1 (tensor)
                      230 LOAD_CONST               1 (0.8)
                      232 BUILD_LIST               1
@@ -1072,63 +1752,63 @@
                      288 CALL                     2
                      298 KW_NAMES                10
                      300 PRECALL                  3
                      304 CALL                     3
                      314 BEFORE_WITH
                      316 STORE_FAST               6 (mock_latent_scores)
          
-          95         318 LOAD_GLOBAL              1 (NULL + torch)
+         114         318 LOAD_GLOBAL              1 (NULL + torch)
                      330 LOAD_ATTR                7 (ones)
                      340 LOAD_CONST               5 (1)
                      342 LOAD_FAST                2 (latent_variables)
                      344 BUILD_TUPLE              2
                      346 PRECALL                  1
                      350 CALL                     1
                      360 STORE_FAST               7 (inverted_scales)
          
-          96         362 LOAD_CONST               7 (-1)
+         115         362 LOAD_CONST               7 (-1)
                      364 LOAD_FAST                7 (inverted_scales)
                      366 LOAD_CONST              11 (0)
                      368 LOAD_CONST               5 (1)
                      370 LOAD_CONST               0 (None)
                      372 LOAD_CONST               6 (2)
                      374 BUILD_SLICE              3
                      376 BUILD_TUPLE              2
                      378 STORE_SUBSCR
          
-          97         382 LOAD_GLOBAL              9 (NULL + patch)
+         116         382 LOAD_GLOBAL              9 (NULL + patch)
                      394 LOAD_ATTR                5 (object)
                      404 LOAD_GLOBAL             12 (IRTScorer)
                      416 LOAD_CONST              12 ('_inverted_scales')
                      418 LOAD_FAST                7 (inverted_scales)
                      420 KW_NAMES                10
                      422 PRECALL                  3
                      426 CALL                     3
                      436 BEFORE_WITH
                      438 POP_TOP
          
-          99         440 LOAD_GLOBAL              1 (NULL + torch)
+         118         440 LOAD_GLOBAL              1 (NULL + torch)
                      452 LOAD_ATTR                3 (full)
                      462 LOAD_FAST                2 (latent_variables)
                      464 BUILD_TUPLE              1
                      466 LOAD_CONST              13 (-0.6)
                      468 PRECALL                  2
                      472 CALL                     2
                      482 STORE_FAST               8 (grid_start)
          
-         100         484 LOAD_GLOBAL              1 (NULL + torch)
+         119         484 LOAD_GLOBAL              1 (NULL + torch)
                      496 LOAD_ATTR                3 (full)
                      506 LOAD_FAST                2 (latent_variables)
                      508 BUILD_TUPLE              1
                      510 LOAD_CONST              14 (2.0)
                      512 PRECALL                  2
                      516 CALL                     2
                      526 STORE_FAST               9 (grid_end)
          
-         101         528 LOAD_GLOBAL              9 (NULL + patch)
+         120         528 LOAD_GLOBAL              9 (NULL + patch)
                      540 LOAD_ATTR                5 (object)
                      550 LOAD_GLOBAL             12 (IRTScorer)
                      562 LOAD_CONST              15 ('_get_grid_boundaries')
                      564 LOAD_FAST                8 (grid_start)
                      566 LOAD_FAST                9 (grid_end)
                      568 LOAD_GLOBAL              1 (NULL + torch)
                      580 LOAD_ATTR                8 (zeros)
@@ -1143,18 +1823,18 @@
                      634 BUILD_TUPLE              3
                      636 KW_NAMES                10
                      638 PRECALL                  3
                      642 CALL                     3
                      652 BEFORE_WITH
                      654 POP_TOP
          
-         102         656 LOAD_FAST                1 (one_dimensional)
+         121         656 LOAD_FAST                1 (one_dimensional)
                      658 POP_JUMP_FORWARD_IF_FALSE   107 (to 874)
          
-         103         660 LOAD_GLOBAL              9 (NULL + patch)
+         122         660 LOAD_GLOBAL              9 (NULL + patch)
                      672 LOAD_ATTR                5 (object)
                      682 LOAD_GLOBAL             12 (IRTScorer)
                      694 LOAD_CONST              17 ('_compute_1d_bit_scores')
                      696 LOAD_GLOBAL              1 (NULL + torch)
                      708 LOAD_ATTR                1 (tensor)
                      718 LOAD_CONST              18 (0.5)
                      720 BUILD_LIST               1
@@ -1169,28 +1849,28 @@
                      740 CALL                     1
                      750 KW_NAMES                10
                      752 PRECALL                  3
                      756 CALL                     3
                      766 BEFORE_WITH
                      768 POP_TOP
          
-         104         770 LOAD_FAST                0 (irt_scorer)
+         123         770 LOAD_FAST                0 (irt_scorer)
                      772 LOAD_METHOD             10 (bit_scores_from_z)
                      794 LOAD_FAST                4 (z)
                      796 LOAD_FAST                5 (start_z)
                      798 LOAD_FAST                1 (one_dimensional)
                      800 LOAD_FAST                3 (bit_score_z_grid_method)
                      802 KW_NAMES                19
                      804 PRECALL                  4
                      808 CALL                     4
                      818 UNPACK_SEQUENCE          2
                      822 STORE_FAST              10 (bit_scores)
                      824 STORE_FAST              11 (_)
          
-         103         826 LOAD_CONST               0 (None)
+         122         826 LOAD_CONST               0 (None)
                      828 LOAD_CONST               0 (None)
                      830 LOAD_CONST               0 (None)
                      832 PRECALL                  2
                      836 CALL                     2
                      846 POP_TOP
                      848 JUMP_FORWARD            11 (to 872)
                  >>  850 PUSH_EXC_INFO
@@ -1202,15 +1882,15 @@
                      862 RERAISE                  1
                  >>  864 POP_TOP
                      866 POP_EXCEPT
                      868 POP_TOP
                      870 POP_TOP
                  >>  872 JUMP_FORWARD           126 (to 1126)
          
-         106     >>  874 LOAD_GLOBAL              9 (NULL + patch)
+         125     >>  874 LOAD_GLOBAL              9 (NULL + patch)
                      886 LOAD_ATTR                5 (object)
                      896 LOAD_GLOBAL             12 (IRTScorer)
                      908 LOAD_CONST              20 ('_compute_multi_dimensional_bit_scores')
                      910 LOAD_GLOBAL              1 (NULL + torch)
                      922 LOAD_ATTR                1 (tensor)
                      932 LOAD_CONST              18 (0.5)
                      934 BUILD_LIST               1
@@ -1230,28 +1910,28 @@
                      994 CALL                     2
                     1004 KW_NAMES                10
                     1006 PRECALL                  3
                     1010 CALL                     3
                     1020 BEFORE_WITH
                     1022 POP_TOP
          
-         107        1024 LOAD_FAST                0 (irt_scorer)
+         126        1024 LOAD_FAST                0 (irt_scorer)
                     1026 LOAD_METHOD             10 (bit_scores_from_z)
                     1048 LOAD_FAST                4 (z)
                     1050 LOAD_FAST                5 (start_z)
                     1052 LOAD_FAST                1 (one_dimensional)
                     1054 LOAD_FAST                3 (bit_score_z_grid_method)
                     1056 KW_NAMES                19
                     1058 PRECALL                  4
                     1062 CALL                     4
                     1072 UNPACK_SEQUENCE          2
                     1076 STORE_FAST              10 (bit_scores)
                     1078 STORE_FAST              11 (_)
          
-         106        1080 LOAD_CONST               0 (None)
+         125        1080 LOAD_CONST               0 (None)
                     1082 LOAD_CONST               0 (None)
                     1084 LOAD_CONST               0 (None)
                     1086 PRECALL                  2
                     1090 CALL                     2
                     1100 POP_TOP
                     1102 JUMP_FORWARD            11 (to 1126)
                  >> 1104 PUSH_EXC_INFO
@@ -1262,15 +1942,15 @@
                     1114 POP_EXCEPT
                     1116 RERAISE                  1
                  >> 1118 POP_TOP
                     1120 POP_EXCEPT
                     1122 POP_TOP
                     1124 POP_TOP
          
-         101     >> 1126 LOAD_CONST               0 (None)
+         120     >> 1126 LOAD_CONST               0 (None)
                     1128 LOAD_CONST               0 (None)
                     1130 LOAD_CONST               0 (None)
                     1132 PRECALL                  2
                     1136 CALL                     2
                     1146 POP_TOP
                     1148 JUMP_FORWARD            11 (to 1172)
                  >> 1150 PUSH_EXC_INFO
@@ -1281,15 +1961,15 @@
                     1160 POP_EXCEPT
                     1162 RERAISE                  1
                  >> 1164 POP_TOP
                     1166 POP_EXCEPT
                     1168 POP_TOP
                     1170 POP_TOP
          
-          97     >> 1172 LOAD_CONST               0 (None)
+         116     >> 1172 LOAD_CONST               0 (None)
                     1174 LOAD_CONST               0 (None)
                     1176 LOAD_CONST               0 (None)
                     1178 PRECALL                  2
                     1182 CALL                     2
                     1192 POP_TOP
                     1194 JUMP_FORWARD            11 (to 1218)
                  >> 1196 PUSH_EXC_INFO
@@ -1300,15 +1980,15 @@
                     1206 POP_EXCEPT
                     1208 RERAISE                  1
                  >> 1210 POP_TOP
                     1212 POP_EXCEPT
                     1214 POP_TOP
                     1216 POP_TOP
          
-          94     >> 1218 LOAD_CONST               0 (None)
+         113     >> 1218 LOAD_CONST               0 (None)
                     1220 LOAD_CONST               0 (None)
                     1222 LOAD_CONST               0 (None)
                     1224 PRECALL                  2
                     1228 CALL                     2
                     1238 POP_TOP
                     1240 JUMP_FORWARD            11 (to 1264)
                  >> 1242 PUSH_EXC_INFO
@@ -1319,18 +1999,18 @@
                     1252 POP_EXCEPT
                     1254 RERAISE                  1
                  >> 1256 POP_TOP
                     1258 POP_EXCEPT
                     1260 POP_TOP
                     1262 POP_TOP
          
-         110     >> 1264 LOAD_FAST                1 (one_dimensional)
+         129     >> 1264 LOAD_FAST                1 (one_dimensional)
                     1266 POP_JUMP_FORWARD_IF_FALSE   194 (to 1656)
          
-         111        1268 LOAD_FAST               10 (bit_scores)
+         130        1268 LOAD_FAST               10 (bit_scores)
                     1270 LOAD_ATTR               11 (shape)
                     1280 STORE_FAST              12 (@py_assert1)
                     1282 LOAD_CONST              21 ((4, 1))
                     1284 STORE_FAST              13 (@py_assert4)
                     1286 LOAD_FAST               12 (@py_assert1)
                     1288 LOAD_FAST               13 (@py_assert4)
                     1290 COMPARE_OP               2 (==)
@@ -1401,15 +2081,15 @@
                     1644 COPY                     1
                     1646 STORE_FAST              12 (@py_assert1)
                     1648 COPY                     1
                     1650 STORE_FAST              14 (@py_assert3)
                     1652 STORE_FAST              13 (@py_assert4)
                     1654 JUMP_FORWARD           195 (to 2046)
          
-         113     >> 1656 LOAD_FAST               10 (bit_scores)
+         132     >> 1656 LOAD_FAST               10 (bit_scores)
                     1658 LOAD_ATTR               11 (shape)
                     1668 STORE_FAST              12 (@py_assert1)
                     1670 LOAD_CONST              28 (4)
                     1672 LOAD_FAST                2 (latent_variables)
                     1674 BUILD_TUPLE              2
                     1676 STORE_FAST              13 (@py_assert4)
                     1678 LOAD_FAST               12 (@py_assert1)
@@ -1481,20 +2161,20 @@
                  >> 2034 LOAD_CONST               0 (None)
                     2036 COPY                     1
                     2038 STORE_FAST              12 (@py_assert1)
                     2040 COPY                     1
                     2042 STORE_FAST              14 (@py_assert3)
                     2044 STORE_FAST              13 (@py_assert4)
          
-         115     >> 2046 LOAD_FAST                3 (bit_score_z_grid_method)
+         134     >> 2046 LOAD_FAST                3 (bit_score_z_grid_method)
                     2048 LOAD_CONST              29 ('ML')
                     2050 COMPARE_OP               2 (==)
                     2056 POP_JUMP_FORWARD_IF_FALSE    70 (to 2198)
          
-         116        2058 LOAD_FAST                6 (mock_latent_scores)
+         135        2058 LOAD_FAST                6 (mock_latent_scores)
                     2060 LOAD_METHOD             20 (assert_called_once_with)
                     2082 LOAD_FAST                0 (irt_scorer)
                     2084 LOAD_ATTR               21 (algorithm)
                     2094 LOAD_ATTR               22 (train_data)
                     2104 LOAD_CONST              30 ('z')
                     2106 LOAD_CONST              29 ('ML')
                     2108 LOAD_GLOBAL              0 (torch)
@@ -1510,15 +2190,15 @@
                     2176 KW_NAMES                34
                     2178 PRECALL                  5
                     2182 CALL                     5
                     2192 POP_TOP
                     2194 LOAD_CONST               0 (None)
                     2196 RETURN_VALUE
          
-         115     >> 2198 LOAD_CONST               0 (None)
+         134     >> 2198 LOAD_CONST               0 (None)
                     2200 RETURN_VALUE
          ExceptionTable:
            316 to 436 -> 1242 [1] lasti
            438 to 652 -> 1196 [2] lasti
            654 to 766 -> 1150 [3] lasti
            768 to 824 -> 850 [4] lasti
            826 to 848 -> 1150 [3] lasti
@@ -1580,17 +2260,17 @@
             'cpu'
             0.3
             ('scale', 'z_estimation_method', 'ml_map_device', 'lbfgs_learning_rate')
          names      ('torch', 'tensor', 'repeat', 'full', 'patch', 'object', 'IRTScorer', 'ones', 'zeros', 'bool', 'bit_scores_from_z', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'assert_called_once_with', 'algorithm', 'train_data', 'cuda', 'is_available')
          varnames   ('irt_scorer', 'one_dimensional', 'latent_variables', 'bit_score_z_grid_method', 'z', 'start_z', 'mock_latent_scores', 'inverted_scales', 'grid_start', 'grid_end', 'bit_scores', '_', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'test_bit_scores'
-         firstlineno 86
+         firstlineno 105
          lnotab
             0x020360011c012e0392012c0114013a022c012c01800104016e0138ff30
             03960138ff2efb2efc2efd2e100401ff008502ff0087020c018cff
       'z_estimation_method'
       'EAP'
       code
          argcount  : 2
@@ -1688,17 +2368,17 @@
             0000000000000000006a0f00000000000000007400000000000000000000
             00a6010000ab0100000000000000006e0164117415000000000000000000
             006a0f00000000000000007c0fa6010000ab010000000000000000641a9c
             047a0600007d10641b641c7c1069017a0600007d11742300000000000000
             0000007415000000000000000000006a1200000000000000007c11a60100
             00ab010000000000000000a6010000ab0100000000000000008201640078
             017d0778017d0a7d0f64005300
-         118           0 RESUME                   0
+         137           0 RESUME                   0
          
-         120           2 LOAD_GLOBAL              1 (NULL + torch)
+         139           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (tensor)
                       24 LOAD_CONST               1 (1.0)
                       26 LOAD_CONST               2 (0.0)
                       28 BUILD_LIST               2
                       30 LOAD_CONST               1 (1.0)
                       32 LOAD_CONST               3 (2.0)
                       34 BUILD_LIST               2
@@ -1706,50 +2386,50 @@
                       38 LOAD_CONST               3 (2.0)
                       40 BUILD_LIST               2
                       42 BUILD_LIST               3
                       44 PRECALL                  1
                       48 CALL                     1
                       58 STORE_FAST               2 (data)
          
-         121          60 LOAD_GLOBAL              1 (NULL + torch)
+         140          60 LOAD_GLOBAL              1 (NULL + torch)
                       72 LOAD_ATTR                2 (randn)
                       82 LOAD_FAST                2 (data)
                       84 LOAD_ATTR                3 (shape)
                       94 LOAD_CONST               4 (0)
                       96 BINARY_SUBSCR
                      106 LOAD_FAST                0 (irt_scorer)
                      108 LOAD_ATTR                4 (model)
                      118 LOAD_ATTR                5 (latent_variables)
                      128 PRECALL                  2
                      132 CALL                     2
                      142 STORE_FAST               3 (expected_output)
          
-         122         144 LOAD_FAST                0 (irt_scorer)
+         141         144 LOAD_FAST                0 (irt_scorer)
                      146 LOAD_METHOD              6 (latent_scores)
                      168 LOAD_FAST                2 (data)
                      170 LOAD_CONST               5 ('z')
                      172 LOAD_FAST                1 (z_estimation_method)
                      174 KW_NAMES                 6
                      176 PRECALL                  3
                      180 CALL                     3
                      190 STORE_FAST               4 (scores)
          
-         124         192 LOAD_FAST                1 (z_estimation_method)
+         143         192 LOAD_FAST                1 (z_estimation_method)
                      194 LOAD_CONST               7 ('NN')
                      196 COMPARE_OP               2 (==)
                      202 EXTENDED_ARG             2
                      204 POP_JUMP_FORWARD_IF_FALSE   559 (to 1324)
          
-         125         206 LOAD_FAST                0 (irt_scorer)
+         144         206 LOAD_FAST                0 (irt_scorer)
                      208 LOAD_ATTR                7 (algorithm)
                      218 LOAD_ATTR                8 (z_scores)
                      228 LOAD_ATTR                9 (call_args)
                      238 STORE_FAST               5 (call_args)
          
-         126         240 LOAD_CONST               0 (None)
+         145         240 LOAD_CONST               0 (None)
                      242 STORE_FAST               6 (@py_assert2)
                      244 LOAD_FAST                5 (call_args)
                      246 LOAD_FAST                6 (@py_assert2)
                      248 IS_OP                    1
                      250 STORE_FAST               7 (@py_assert1)
                      252 LOAD_FAST                7 (@py_assert1)
                      254 POP_JUMP_FORWARD_IF_TRUE   172 (to 600)
@@ -1815,30 +2495,30 @@
                      588 CALL                     1
                      598 RAISE_VARARGS            1
                  >>  600 LOAD_CONST               0 (None)
                      602 COPY                     1
                      604 STORE_FAST               7 (@py_assert1)
                      606 STORE_FAST               6 (@py_assert2)
          
-         127         608 LOAD_GLOBAL              0 (torch)
+         146         608 LOAD_GLOBAL              0 (torch)
          
-         129         620 LOAD_ATTR               19 (allclose)
+         148         620 LOAD_ATTR               19 (allclose)
          
-         127         630 STORE_FAST               7 (@py_assert1)
+         146         630 STORE_FAST               7 (@py_assert1)
                      632 LOAD_FAST                5 (call_args)
                      634 LOAD_CONST               4 (0)
                      636 BINARY_SUBSCR
                      646 LOAD_CONST               4 (0)
                      648 BINARY_SUBSCR
                      658 STORE_FAST              10 (@py_assert3)
                      660 LOAD_FAST                2 (data)
          
-         129         662 LOAD_ATTR               20 (contiguous)
+         148         662 LOAD_ATTR               20 (contiguous)
          
-         127         672 STORE_FAST              11 (@py_assert6)
+         146         672 STORE_FAST              11 (@py_assert6)
                      674 PUSH_NULL
                      676 LOAD_FAST               11 (@py_assert6)
                      678 PRECALL                  0
                      682 CALL                     0
                      692 STORE_FAST              12 (@py_assert8)
                      694 PUSH_NULL
                      696 LOAD_FAST                7 (@py_assert1)
@@ -1848,118 +2528,118 @@
                      706 CALL                     2
                      716 STORE_FAST              13 (@py_assert10)
                      718 LOAD_FAST               13 (@py_assert10)
                      720 EXTENDED_ARG             1
                      722 POP_JUMP_FORWARD_IF_TRUE   289 (to 1302)
                      724 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129         736 LOAD_ATTR               16 (_format_assertmsg)
+         148         736 LOAD_ATTR               16 (_format_assertmsg)
          
-         127         746 LOAD_CONST              15 ('z_scores method was called with incorrect arguments')
+         146         746 LOAD_CONST              15 ('z_scores method was called with incorrect arguments')
                      748 PRECALL                  1
                      752 CALL                     1
                      762 LOAD_CONST              16 ('\n>assert %(py11)s\n{%(py11)s = %(py2)s\n{%(py2)s = %(py0)s.allclose\n}(%(py4)s, %(py9)s\n{%(py9)s = %(py7)s\n{%(py7)s = %(py5)s.contiguous\n}()\n})\n}')
                      764 BINARY_OP                0 (+)
                      768 LOAD_CONST              17 ('torch')
                      770 LOAD_GLOBAL             25 (NULL + @py_builtins)
          
-         129         782 LOAD_ATTR               13 (locals)
+         148         782 LOAD_ATTR               13 (locals)
          
-         127         792 PRECALL                  0
+         146         792 PRECALL                  0
                      796 CALL                     0
                      806 CONTAINS_OP              0
                      808 POP_JUMP_FORWARD_IF_TRUE    25 (to 860)
                      810 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129         822 LOAD_ATTR               14 (_should_repr_global_name)
+         148         822 LOAD_ATTR               14 (_should_repr_global_name)
          
-         127         832 LOAD_GLOBAL              0 (torch)
+         146         832 LOAD_GLOBAL              0 (torch)
                      844 PRECALL                  1
                      848 CALL                     1
                      858 POP_JUMP_FORWARD_IF_FALSE    25 (to 910)
                  >>  860 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129         872 LOAD_ATTR               15 (_saferepr)
+         148         872 LOAD_ATTR               15 (_saferepr)
          
-         127         882 LOAD_GLOBAL              0 (torch)
+         146         882 LOAD_GLOBAL              0 (torch)
                      894 PRECALL                  1
                      898 CALL                     1
                      908 JUMP_FORWARD             1 (to 912)
                  >>  910 LOAD_CONST              17 ('torch')
                  >>  912 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129         924 LOAD_ATTR               15 (_saferepr)
+         148         924 LOAD_ATTR               15 (_saferepr)
          
-         127         934 LOAD_FAST                7 (@py_assert1)
+         146         934 LOAD_FAST                7 (@py_assert1)
                      936 PRECALL                  1
                      940 CALL                     1
                      950 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129         962 LOAD_ATTR               15 (_saferepr)
+         148         962 LOAD_ATTR               15 (_saferepr)
          
-         127         972 LOAD_FAST               10 (@py_assert3)
+         146         972 LOAD_FAST               10 (@py_assert3)
                      974 PRECALL                  1
                      978 CALL                     1
                      988 LOAD_CONST              18 ('data')
                      990 LOAD_GLOBAL             25 (NULL + @py_builtins)
          
-         129        1002 LOAD_ATTR               13 (locals)
+         148        1002 LOAD_ATTR               13 (locals)
          
-         127        1012 PRECALL                  0
+         146        1012 PRECALL                  0
                     1016 CALL                     0
                     1026 CONTAINS_OP              0
                     1028 POP_JUMP_FORWARD_IF_TRUE    20 (to 1070)
                     1030 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129        1042 LOAD_ATTR               14 (_should_repr_global_name)
+         148        1042 LOAD_ATTR               14 (_should_repr_global_name)
          
-         127        1052 LOAD_FAST                2 (data)
+         146        1052 LOAD_FAST                2 (data)
                     1054 PRECALL                  1
                     1058 CALL                     1
                     1068 POP_JUMP_FORWARD_IF_FALSE    20 (to 1110)
                  >> 1070 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129        1082 LOAD_ATTR               15 (_saferepr)
+         148        1082 LOAD_ATTR               15 (_saferepr)
          
-         127        1092 LOAD_FAST                2 (data)
+         146        1092 LOAD_FAST                2 (data)
                     1094 PRECALL                  1
                     1098 CALL                     1
                     1108 JUMP_FORWARD             1 (to 1112)
                  >> 1110 LOAD_CONST              18 ('data')
                  >> 1112 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129        1124 LOAD_ATTR               15 (_saferepr)
+         148        1124 LOAD_ATTR               15 (_saferepr)
          
-         127        1134 LOAD_FAST               11 (@py_assert6)
+         146        1134 LOAD_FAST               11 (@py_assert6)
                     1136 PRECALL                  1
                     1140 CALL                     1
                     1150 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129        1162 LOAD_ATTR               15 (_saferepr)
+         148        1162 LOAD_ATTR               15 (_saferepr)
          
-         127        1172 LOAD_FAST               12 (@py_assert8)
+         146        1172 LOAD_FAST               12 (@py_assert8)
                     1174 PRECALL                  1
                     1178 CALL                     1
                     1188 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129        1200 LOAD_ATTR               15 (_saferepr)
+         148        1200 LOAD_ATTR               15 (_saferepr)
          
-         127        1210 LOAD_FAST               13 (@py_assert10)
+         146        1210 LOAD_FAST               13 (@py_assert10)
                     1212 PRECALL                  1
                     1216 CALL                     1
                     1226 LOAD_CONST              19 (('py0', 'py2', 'py4', 'py5', 'py7', 'py9', 'py11'))
                     1228 BUILD_CONST_KEY_MAP      7
                     1230 BINARY_OP                6 (%)
                     1234 STORE_FAST              14 (@py_format12)
                     1236 LOAD_GLOBAL             35 (NULL + AssertionError)
                     1248 LOAD_GLOBAL             21 (NULL + @pytest_ar)
          
-         129        1260 LOAD_ATTR               18 (_format_explanation)
+         148        1260 LOAD_ATTR               18 (_format_explanation)
          
-         127        1270 LOAD_FAST               14 (@py_format12)
+         146        1270 LOAD_FAST               14 (@py_format12)
                     1272 PRECALL                  1
                     1276 CALL                     1
                     1286 PRECALL                  1
                     1290 CALL                     1
                     1300 RAISE_VARARGS            1
                  >> 1302 LOAD_CONST               0 (None)
                     1304 COPY                     1
@@ -1969,25 +2649,25 @@
                     1312 COPY                     1
                     1314 STORE_FAST              11 (@py_assert6)
                     1316 COPY                     1
                     1318 STORE_FAST              12 (@py_assert8)
                     1320 STORE_FAST              13 (@py_assert10)
                     1322 JUMP_FORWARD           202 (to 1728)
          
-         130     >> 1324 LOAD_FAST                1 (z_estimation_method)
+         149     >> 1324 LOAD_FAST                1 (z_estimation_method)
                     1326 LOAD_CONST              20 ('EAP')
                     1328 COMPARE_OP               2 (==)
                     1334 POP_JUMP_FORWARD_IF_FALSE   196 (to 1728)
          
-         131        1336 LOAD_FAST                0 (irt_scorer)
+         150        1336 LOAD_FAST                0 (irt_scorer)
                     1338 LOAD_ATTR                4 (model)
                     1348 LOAD_ATTR                9 (call_args)
                     1358 STORE_FAST               5 (call_args)
          
-         132        1360 LOAD_CONST               0 (None)
+         151        1360 LOAD_CONST               0 (None)
                     1362 STORE_FAST               6 (@py_assert2)
                     1364 LOAD_FAST                5 (call_args)
                     1366 LOAD_FAST                6 (@py_assert2)
                     1368 IS_OP                    1
                     1370 STORE_FAST               7 (@py_assert1)
                     1372 LOAD_FAST                7 (@py_assert1)
                     1374 POP_JUMP_FORWARD_IF_TRUE   172 (to 1720)
@@ -2053,15 +2733,15 @@
                     1708 CALL                     1
                     1718 RAISE_VARARGS            1
                  >> 1720 LOAD_CONST               0 (None)
                     1722 COPY                     1
                     1724 STORE_FAST               7 (@py_assert1)
                     1726 STORE_FAST               6 (@py_assert2)
          
-         134     >> 1728 LOAD_FAST                4 (scores)
+         153     >> 1728 LOAD_FAST                4 (scores)
                     1730 LOAD_ATTR                3 (shape)
                     1740 STORE_FAST               7 (@py_assert1)
                     1742 LOAD_FAST                3 (expected_output)
                     1744 LOAD_ATTR                3 (shape)
                     1754 STORE_FAST              15 (@py_assert5)
                     1756 LOAD_FAST                7 (@py_assert1)
                     1758 LOAD_FAST               15 (@py_assert5)
@@ -2152,15 +2832,15 @@
                  >> 2236 LOAD_CONST               0 (None)
                     2238 COPY                     1
                     2240 STORE_FAST               7 (@py_assert1)
                     2242 COPY                     1
                     2244 STORE_FAST              10 (@py_assert3)
                     2246 STORE_FAST              15 (@py_assert5)
          
-         135        2248 LOAD_FAST                4 (scores)
+         154        2248 LOAD_FAST                4 (scores)
                     2250 LOAD_ATTR               21 (dtype)
                     2260 STORE_FAST               7 (@py_assert1)
                     2262 LOAD_GLOBAL              0 (torch)
                     2274 LOAD_ATTR               22 (float32)
                     2284 STORE_FAST              15 (@py_assert5)
                     2286 LOAD_FAST                7 (@py_assert1)
                     2288 LOAD_FAST               15 (@py_assert5)
@@ -2287,17 +2967,17 @@
             'assert %(py8)s'
             'py8'
             ('%(py2)s\n{%(py2)s = %(py0)s.dtype\n} == %(py6)s\n{%(py6)s = %(py4)s.float32\n}',)
          names      ('torch', 'tensor', 'randn', 'shape', 'model', 'latent_variables', 'latent_scores', 'algorithm', 'z_scores', 'call_args', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'allclose', 'contiguous', 'dtype', 'float32')
          varnames   ('irt_scorer', 'z_estimation_method', 'data', 'expected_output', 'scores', 'call_args', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6', '@py_assert3', '@py_assert6', '@py_assert8', '@py_assert10', '@py_format12', '@py_assert5', '@py_format7', '@py_format9')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'test_latent_scores'
-         firstlineno 118
+         firstlineno 137
          lnotab
             0x02023a01540130020e012201ff0071010c020afe20020afe40020afe24
             020afe1e020afe28020afe2a020afe1c020afe1e020afe1e020afe1e020a
             fe20020afe1c020afe1c020afe32020afe36030c011801ff007102ff00ff
             000a01
       'grid_size'
       (3, 4, 5)
@@ -2401,17 +3081,17 @@
             000000000000007409000000000000000000006a0600000000000000007c
             09a6010000ab01000000000000000064119c027a0600007d0a7409000000
             000000000000006a0a00000000000000006423a6010000ab010000000000
             00000064137a00000064147c0a69017a0600007d0b741700000000000000
             0000007409000000000000000000006a0c00000000000000007c0ba60100
             00ab010000000000000000a6010000ab0100000000000000008201640078
             017d0578017d067d0964005300
-         138           0 RESUME                   0
+         157           0 RESUME                   0
          
-         140           2 LOAD_GLOBAL              1 (NULL + torch)
+         159           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (tensor)
                       24 BUILD_LIST               0
                       26 LOAD_CONST               1 ((1, -4, -1))
                       28 LIST_EXTEND              1
                       30 BUILD_LIST               0
                       32 LOAD_CONST               2 ((2, 5, -3))
                       34 LIST_EXTEND              1
@@ -2422,32 +3102,32 @@
                       44 LOAD_CONST               4 ((4, 6, -5))
                       46 LIST_EXTEND              1
                       48 BUILD_LIST               4
                       50 PRECALL                  1
                       54 CALL                     1
                       64 STORE_FAST               2 (test_tensor)
          
-         142          66 LOAD_FAST                0 (irt_scorer)
+         161          66 LOAD_FAST                0 (irt_scorer)
                       68 LOAD_METHOD              2 (_z_grid)
                       90 LOAD_FAST                2 (test_tensor)
                       92 LOAD_FAST                1 (grid_size)
                       94 KW_NAMES                 5
                       96 PRECALL                  2
                      100 CALL                     2
                      110 STORE_FAST               3 (grid_combinations)
          
-         145         112 LOAD_FAST                1 (grid_size)
+         164         112 LOAD_FAST                1 (grid_size)
                      114 LOAD_FAST                2 (test_tensor)
                      116 LOAD_ATTR                3 (shape)
                      126 LOAD_CONST               6 (1)
                      128 BINARY_SUBSCR
                      138 BINARY_OP                8 (**)
                      142 STORE_FAST               4 (expected_rows)
          
-         146         144 LOAD_FAST                3 (grid_combinations)
+         165         144 LOAD_FAST                3 (grid_combinations)
                      146 LOAD_ATTR                3 (shape)
                      156 LOAD_CONST               7 (0)
                      158 BINARY_SUBSCR
                      168 STORE_FAST               5 (@py_assert0)
                      170 LOAD_FAST                5 (@py_assert0)
                      172 LOAD_FAST                4 (expected_rows)
                      174 COMPARE_OP               2 (==)
@@ -2525,15 +3205,15 @@
                      552 CALL                     1
                      562 RAISE_VARARGS            1
                  >>  564 LOAD_CONST               0 (None)
                      566 COPY                     1
                      568 STORE_FAST               5 (@py_assert0)
                      570 STORE_FAST               6 (@py_assert2)
          
-         149         572 LOAD_FAST                3 (grid_combinations)
+         168         572 LOAD_FAST                3 (grid_combinations)
                      574 LOAD_ATTR                3 (shape)
                      584 LOAD_CONST               6 (1)
                      586 BINARY_SUBSCR
                      596 STORE_FAST               5 (@py_assert0)
                      598 LOAD_FAST                2 (test_tensor)
                      600 LOAD_ATTR                3 (shape)
                      610 LOAD_CONST               6 (1)
@@ -2606,75 +3286,75 @@
                  >>  954 LOAD_CONST               0 (None)
                      956 COPY                     1
                      958 STORE_FAST               5 (@py_assert0)
                      960 COPY                     1
                      962 STORE_FAST               6 (@py_assert2)
                      964 STORE_FAST               9 (@py_assert3)
          
-         152         966 LOAD_GLOBAL             27 (NULL + range)
+         171         966 LOAD_GLOBAL             27 (NULL + range)
                      978 LOAD_FAST                2 (test_tensor)
                      980 LOAD_ATTR                3 (shape)
                      990 LOAD_CONST               6 (1)
                      992 BINARY_SUBSCR
                     1002 PRECALL                  1
                     1006 CALL                     1
                     1016 GET_ITER
                  >> 1018 EXTENDED_ARG             2
                     1020 FOR_ITER               757 (to 2536)
                     1022 STORE_FAST              12 (col)
          
-         153        1024 LOAD_FAST                2 (test_tensor)
+         172        1024 LOAD_FAST                2 (test_tensor)
                     1026 LOAD_CONST               0 (None)
                     1028 LOAD_CONST               0 (None)
                     1030 BUILD_SLICE              2
                     1032 LOAD_FAST               12 (col)
                     1034 BUILD_TUPLE              2
                     1036 BINARY_SUBSCR
                     1046 LOAD_METHOD             14 (min)
                     1068 PRECALL                  0
                     1072 CALL                     0
                     1082 LOAD_METHOD             15 (item)
                     1104 PRECALL                  0
                     1108 CALL                     0
                     1118 STORE_FAST              13 (min_val)
          
-         154        1120 LOAD_FAST                2 (test_tensor)
+         173        1120 LOAD_FAST                2 (test_tensor)
                     1122 LOAD_CONST               0 (None)
                     1124 LOAD_CONST               0 (None)
                     1126 BUILD_SLICE              2
                     1128 LOAD_FAST               12 (col)
                     1130 BUILD_TUPLE              2
                     1132 BINARY_SUBSCR
                     1142 LOAD_METHOD             16 (max)
                     1164 PRECALL                  0
                     1168 CALL                     0
                     1178 LOAD_METHOD             15 (item)
                     1200 PRECALL                  0
                     1204 CALL                     0
                     1214 STORE_FAST              14 (max_val)
          
-         157        1216 LOAD_FAST               13 (min_val)
+         176        1216 LOAD_FAST               13 (min_val)
                     1218 LOAD_CONST              21 (0.25)
                     1220 LOAD_FAST               14 (max_val)
                     1222 LOAD_FAST               13 (min_val)
                     1224 BINARY_OP               10 (-)
                     1228 BINARY_OP                5 (*)
                     1232 BINARY_OP               10 (-)
                     1236 STORE_FAST              15 (adjusted_min)
          
-         158        1238 LOAD_FAST               14 (max_val)
+         177        1238 LOAD_FAST               14 (max_val)
                     1240 LOAD_CONST              21 (0.25)
                     1242 LOAD_FAST               14 (max_val)
                     1244 LOAD_FAST               13 (min_val)
                     1246 BINARY_OP               10 (-)
                     1250 BINARY_OP                5 (*)
                     1254 BINARY_OP                0 (+)
                     1258 STORE_FAST              16 (adjusted_max)
          
-         160        1260 LOAD_FAST                3 (grid_combinations)
+         179        1260 LOAD_FAST                3 (grid_combinations)
                     1262 LOAD_CONST               0 (None)
                     1264 LOAD_CONST               0 (None)
                     1266 BUILD_SLICE              2
                     1268 LOAD_FAST               12 (col)
                     1270 BUILD_TUPLE              2
                     1272 BINARY_SUBSCR
                     1282 STORE_FAST               5 (@py_assert0)
@@ -2794,15 +3474,15 @@
                     1884 STORE_FAST              17 (@py_assert4)
                     1886 COPY                     1
                     1888 STORE_FAST              18 (@py_assert6)
                     1890 COPY                     1
                     1892 STORE_FAST              19 (@py_assert8)
                     1894 STORE_FAST              20 (@py_assert10)
          
-         161        1896 LOAD_FAST                3 (grid_combinations)
+         180        1896 LOAD_FAST                3 (grid_combinations)
                     1898 LOAD_CONST               0 (None)
                     1900 LOAD_CONST               0 (None)
                     1902 BUILD_SLICE              2
                     1904 LOAD_FAST               12 (col)
                     1906 BUILD_TUPLE              2
                     1908 BINARY_SUBSCR
                     1918 STORE_FAST               5 (@py_assert0)
@@ -2924,24 +3604,24 @@
                     2524 STORE_FAST              18 (@py_assert6)
                     2526 COPY                     1
                     2528 STORE_FAST              19 (@py_assert8)
                     2530 STORE_FAST              20 (@py_assert10)
                     2532 EXTENDED_ARG             2
                     2534 JUMP_BACKWARD          759 (to 1018)
          
-         164     >> 2536 LOAD_GLOBAL              1 (NULL + torch)
+         183     >> 2536 LOAD_GLOBAL              1 (NULL + torch)
                     2548 LOAD_ATTR               17 (unique)
                     2558 LOAD_FAST                3 (grid_combinations)
                     2560 LOAD_CONST               7 (0)
                     2562 KW_NAMES                34
                     2564 PRECALL                  2
                     2568 CALL                     2
                     2578 STORE_FAST              23 (unique_rows)
          
-         165        2580 LOAD_FAST               23 (unique_rows)
+         184        2580 LOAD_FAST               23 (unique_rows)
                     2582 LOAD_ATTR                3 (shape)
                     2592 LOAD_CONST               7 (0)
                     2594 BINARY_SUBSCR
                     2604 STORE_FAST               5 (@py_assert0)
                     2606 LOAD_FAST                3 (grid_combinations)
                     2608 LOAD_ATTR                3 (shape)
                     2618 LOAD_CONST               7 (0)
@@ -3044,17 +3724,17 @@
             ' max value is more than expected'
             ('dim',)
             'Detected repeated combinations in the grid'
          names      ('torch', 'tensor', '_z_grid', 'shape', '@pytest_ar', '_call_reprcompare', '_saferepr', '@py_builtins', 'locals', '_should_repr_global_name', '_format_assertmsg', 'AssertionError', '_format_explanation', 'range', 'min', 'item', 'max', 'unique')
          varnames   ('irt_scorer', 'grid_size', 'test_tensor', 'grid_combinations', 'expected_rows', '@py_assert0', '@py_assert2', '@py_format4', '@py_format6', '@py_assert3', '@py_format5', '@py_format7', 'col', 'min_val', 'max_val', 'adjusted_min', 'adjusted_max', '@py_assert4', '@py_assert6', '@py_assert8', '@py_assert10', '@py_format12', '@py_format14', 'unique_rows')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'test_z_grid'
-         firstlineno 138
+         firstlineno 157
          lnotab
             0x020240022e032001ff00ad03ff008b033a016001600316011602ff00ff
             007e01ff00ff0082032c01
       code
          argcount  : 2
          nlocals   : 21
          stacksize : 8
@@ -3139,105 +3819,105 @@
             0000000000000000000000a6010000ab0100000000000000006e01641c74
             11000000000000000000006a0d00000000000000007c09a6010000ab0100
             000000000000007c0d7411000000000000000000006a0d00000000000000
             007c14a6010000ab010000000000000000641d9c047a0600007d12741f00
             0000000000000000007411000000000000000000006a1000000000000000
             007c12a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d0978017d0b78017d0e78017d137d1464005300
-         167           0 RESUME                   0
+         186           0 RESUME                   0
          
-         168           2 LOAD_GLOBAL              1 (NULL + torch)
+         187           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (manual_seed)
                       24 LOAD_CONST               1 (4)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 POP_TOP
          
-         169          42 LOAD_GLOBAL              1 (NULL + torch)
+         188          42 LOAD_GLOBAL              1 (NULL + torch)
                       54 LOAD_ATTR                2 (full)
                       64 LOAD_CONST               2 (1)
                       66 LOAD_FAST                1 (latent_variables)
                       68 BUILD_TUPLE              2
                       70 LOAD_CONST               3 (-1.5)
                       72 PRECALL                  2
                       76 CALL                     2
                       86 STORE_FAST               2 (start_z_adjusted)
          
-         170          88 LOAD_GLOBAL              1 (NULL + torch)
+         189          88 LOAD_GLOBAL              1 (NULL + torch)
                      100 LOAD_ATTR                3 (tensor)
                      110 LOAD_CONST               4 (-1.2)
                      112 BUILD_LIST               1
                      114 LOAD_FAST                1 (latent_variables)
                      116 BINARY_OP                5 (*)
                      120 BUILD_LIST               1
                      122 PRECALL                  1
                      126 CALL                     1
                      136 STORE_FAST               3 (grid_start)
          
-         171         138 LOAD_GLOBAL              1 (NULL + torch)
+         190         138 LOAD_GLOBAL              1 (NULL + torch)
                      150 LOAD_ATTR                3 (tensor)
                      160 LOAD_CONST               5 (1.0)
                      162 BUILD_LIST               1
                      164 LOAD_FAST                1 (latent_variables)
                      166 BINARY_OP                5 (*)
                      170 BUILD_LIST               1
                      172 PRECALL                  1
                      176 CALL                     1
                      186 STORE_FAST               4 (grid_end)
          
-         172         188 LOAD_GLOBAL              1 (NULL + torch)
+         191         188 LOAD_GLOBAL              1 (NULL + torch)
                      200 LOAD_ATTR                4 (randn)
                      210 LOAD_CONST               6 (5)
                      212 LOAD_FAST                1 (latent_variables)
                      214 PRECALL                  2
                      218 CALL                     2
                      228 STORE_FAST               5 (z_adjusted)
          
-         173         230 LOAD_GLOBAL              1 (NULL + torch)
+         192         230 LOAD_GLOBAL              1 (NULL + torch)
                      242 LOAD_ATTR                5 (ones)
                      252 LOAD_CONST               2 (1)
                      254 LOAD_FAST                1 (latent_variables)
                      256 BUILD_TUPLE              2
                      258 PRECALL                  1
                      262 CALL                     1
                      272 STORE_FAST               6 (inverted_scale)
          
-         174         274 LOAD_CONST               7 (-1)
+         193         274 LOAD_CONST               7 (-1)
                      276 LOAD_FAST                6 (inverted_scale)
                      278 LOAD_CONST               8 (0)
                      280 LOAD_CONST               2 (1)
                      282 LOAD_CONST               0 (None)
                      284 LOAD_CONST               9 (2)
                      286 BUILD_SLICE              3
                      288 BUILD_TUPLE              2
                      290 STORE_SUBSCR
          
-         175         294 LOAD_CONST              10 (10)
+         194         294 LOAD_CONST              10 (10)
                      296 STORE_FAST               7 (grid_points)
          
-         177         298 LOAD_FAST                0 (irt_scorer)
+         196         298 LOAD_FAST                0 (irt_scorer)
                      300 LOAD_METHOD              6 (_compute_1d_bit_scores)
          
-         178         322 LOAD_FAST                5 (z_adjusted)
+         197         322 LOAD_FAST                5 (z_adjusted)
          
-         179         324 LOAD_FAST                2 (start_z_adjusted)
+         198         324 LOAD_FAST                2 (start_z_adjusted)
          
-         180         326 LOAD_FAST                3 (grid_start)
+         199         326 LOAD_FAST                3 (grid_start)
          
-         181         328 LOAD_FAST                4 (grid_end)
+         200         328 LOAD_FAST                4 (grid_end)
          
-         182         330 LOAD_FAST                6 (inverted_scale)
+         201         330 LOAD_FAST                6 (inverted_scale)
          
-         183         332 LOAD_FAST                7 (grid_points)
+         202         332 LOAD_FAST                7 (grid_points)
          
-         177         334 PRECALL                  6
+         196         334 PRECALL                  6
                      338 CALL                     6
                      348 STORE_FAST               8 (bit_scores)
          
-         186         350 LOAD_FAST                8 (bit_scores)
+         205         350 LOAD_FAST                8 (bit_scores)
                      352 LOAD_ATTR                7 (ndim)
                      362 STORE_FAST               9 (@py_assert1)
                      364 LOAD_CONST               9 (2)
                      366 STORE_FAST              10 (@py_assert4)
                      368 LOAD_FAST                9 (@py_assert1)
                      370 LOAD_FAST               10 (@py_assert4)
                      372 COMPARE_OP               2 (==)
@@ -3313,15 +3993,15 @@
                  >>  766 LOAD_CONST               0 (None)
                      768 COPY                     1
                      770 STORE_FAST               9 (@py_assert1)
                      772 COPY                     1
                      774 STORE_FAST              11 (@py_assert3)
                      776 STORE_FAST              10 (@py_assert4)
          
-         187         778 LOAD_FAST                8 (bit_scores)
+         206         778 LOAD_FAST                8 (bit_scores)
                      780 LOAD_ATTR               17 (size)
                      790 STORE_FAST               9 (@py_assert1)
                      792 LOAD_CONST               2 (1)
                      794 STORE_FAST              11 (@py_assert3)
                      796 PUSH_NULL
                      798 LOAD_FAST                9 (@py_assert1)
                      800 LOAD_FAST               11 (@py_assert3)
@@ -3419,15 +4099,15 @@
                     1304 STORE_FAST              11 (@py_assert3)
                     1306 COPY                     1
                     1308 STORE_FAST              14 (@py_assert5)
                     1310 COPY                     1
                     1312 STORE_FAST              16 (@py_assert7)
                     1314 STORE_FAST              15 (@py_assert8)
          
-         188        1316 LOAD_FAST                8 (bit_scores)
+         207        1316 LOAD_FAST                8 (bit_scores)
                     1318 LOAD_ATTR               17 (size)
                     1328 STORE_FAST               9 (@py_assert1)
                     1330 LOAD_CONST               8 (0)
                     1332 STORE_FAST              11 (@py_assert3)
                     1334 PUSH_NULL
                     1336 LOAD_FAST                9 (@py_assert1)
                     1338 LOAD_FAST               11 (@py_assert3)
@@ -3525,15 +4205,15 @@
                     1842 STORE_FAST              11 (@py_assert3)
                     1844 COPY                     1
                     1846 STORE_FAST              14 (@py_assert5)
                     1848 COPY                     1
                     1850 STORE_FAST              16 (@py_assert7)
                     1852 STORE_FAST              15 (@py_assert8)
          
-         189        1854 LOAD_GLOBAL              0 (torch)
+         208        1854 LOAD_GLOBAL              0 (torch)
                     1866 LOAD_ATTR               18 (all)
                     1876 STORE_FAST               9 (@py_assert1)
                     1878 LOAD_FAST                8 (bit_scores)
                     1880 LOAD_FAST                5 (z_adjusted)
                     1882 LOAD_FAST                2 (start_z_adjusted)
                     1884 COMPARE_OP               0 (<)
                     1890 LOAD_METHOD             18 (all)
@@ -3676,17 +4356,17 @@
             '\n>assert %(py11)s\n{%(py11)s = %(py2)s\n{%(py2)s = %(py0)s.all\n}(%(py9)s)\n}'
             'torch'
             ('py0', 'py2', 'py9', 'py11')
          names      ('torch', 'manual_seed', 'full', 'tensor', 'randn', 'ones', '_compute_1d_bit_scores', 'ndim', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'size', 'all')
          varnames   ('irt_scorer', 'latent_variables', 'start_z_adjusted', 'grid_start', 'grid_end', 'z_adjusted', 'inverted_scale', 'grid_points', 'bit_scores', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert5', '@py_assert8', '@py_assert7', '@py_format10', '@py_format12', '@py_assert6', '@py_assert10')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'test_compute_1d_bit_scores'
-         firstlineno 167
+         firstlineno 186
          lnotab
             0x020128012e01320132012a012c01140104021801020102010201020102
             0102fa1009ff00ad01ff00ff001c01ff00ff001c01
       code
          argcount  : 2
          nlocals   : 24
          stacksize : 9
@@ -3774,115 +4454,115 @@
             0000000000a6010000ab0100000000000000006e01641f74110000000000
             00000000006a0d00000000000000007c0aa6010000ab0100000000000000
             007c0e7411000000000000000000006a0d00000000000000007c17a60100
             00ab01000000000000000064209c047a0600007d15741f00000000000000
             0000007411000000000000000000006a1000000000000000007c15a60100
             00ab010000000000000000a6010000ab0100000000000000008201640078
             017d0a78017d0c78017d0f78017d167d1764005300
-         191           0 RESUME                   0
+         210           0 RESUME                   0
          
-         192           2 LOAD_GLOBAL              1 (NULL + torch)
+         211           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (manual_seed)
                       24 LOAD_CONST               1 (51)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 POP_TOP
          
-         193          42 LOAD_GLOBAL              1 (NULL + torch)
+         212          42 LOAD_GLOBAL              1 (NULL + torch)
                       54 LOAD_ATTR                2 (full)
                       64 LOAD_CONST               2 (1)
                       66 LOAD_FAST                1 (latent_variables)
                       68 BUILD_TUPLE              2
                       70 LOAD_CONST               3 (-1.2)
                       72 PRECALL                  2
                       76 CALL                     2
                       86 STORE_FAST               2 (start_z_adjusted)
          
-         194          88 LOAD_GLOBAL              1 (NULL + torch)
+         213          88 LOAD_GLOBAL              1 (NULL + torch)
                      100 LOAD_ATTR                3 (randn)
                      110 LOAD_CONST               4 (5)
                      112 LOAD_FAST                1 (latent_variables)
                      114 PRECALL                  2
                      118 CALL                     2
                      128 STORE_FAST               3 (train_z_adjusted)
          
-         195         130 LOAD_GLOBAL              1 (NULL + torch)
+         214         130 LOAD_GLOBAL              1 (NULL + torch)
                      142 LOAD_ATTR                3 (randn)
                      152 LOAD_CONST               4 (5)
                      154 LOAD_FAST                1 (latent_variables)
                      156 PRECALL                  2
                      160 CALL                     2
                      170 STORE_FAST               4 (z_adjusted)
          
-         196         172 LOAD_GLOBAL              1 (NULL + torch)
+         215         172 LOAD_GLOBAL              1 (NULL + torch)
                      184 LOAD_ATTR                4 (tensor)
                      194 LOAD_CONST               5 (-1)
                      196 BUILD_LIST               1
                      198 LOAD_FAST                1 (latent_variables)
                      200 BINARY_OP                5 (*)
                      204 BUILD_LIST               1
                      206 PRECALL                  1
                      210 CALL                     1
                      220 STORE_FAST               5 (grid_start)
          
-         197         222 LOAD_GLOBAL              1 (NULL + torch)
+         216         222 LOAD_GLOBAL              1 (NULL + torch)
                      234 LOAD_ATTR                4 (tensor)
                      244 LOAD_CONST               6 (1.0)
                      246 BUILD_LIST               1
                      248 LOAD_FAST                1 (latent_variables)
                      250 BINARY_OP                5 (*)
                      254 BUILD_LIST               1
                      256 PRECALL                  1
                      260 CALL                     1
                      270 STORE_FAST               6 (grid_end)
          
-         198         272 LOAD_GLOBAL              1 (NULL + torch)
+         217         272 LOAD_GLOBAL              1 (NULL + torch)
                      284 LOAD_ATTR                5 (ones)
                      294 LOAD_CONST               2 (1)
                      296 LOAD_FAST                1 (latent_variables)
                      298 BUILD_TUPLE              2
                      300 PRECALL                  1
                      304 CALL                     1
                      314 STORE_FAST               7 (inverted_scale)
          
-         199         316 LOAD_CONST               5 (-1)
+         218         316 LOAD_CONST               5 (-1)
                      318 LOAD_FAST                7 (inverted_scale)
                      320 LOAD_CONST               7 (0)
                      322 LOAD_CONST               2 (1)
                      324 LOAD_CONST               0 (None)
                      326 LOAD_CONST               8 (2)
                      328 BUILD_SLICE              3
                      330 BUILD_TUPLE              2
                      332 STORE_SUBSCR
          
-         200         336 LOAD_CONST               9 (10)
+         219         336 LOAD_CONST               9 (10)
                      338 STORE_FAST               8 (grid_points)
          
-         202         340 LOAD_FAST                0 (irt_scorer)
+         221         340 LOAD_FAST                0 (irt_scorer)
                      342 LOAD_METHOD              6 (_compute_multi_dimensional_bit_scores)
          
-         203         364 LOAD_FAST                4 (z_adjusted)
+         222         364 LOAD_FAST                4 (z_adjusted)
          
-         204         366 LOAD_FAST                2 (start_z_adjusted)
+         223         366 LOAD_FAST                2 (start_z_adjusted)
          
-         205         368 LOAD_FAST                3 (train_z_adjusted)
+         224         368 LOAD_FAST                3 (train_z_adjusted)
          
-         206         370 LOAD_FAST                5 (grid_start)
+         225         370 LOAD_FAST                5 (grid_start)
          
-         207         372 LOAD_FAST                6 (grid_end)
+         226         372 LOAD_FAST                6 (grid_end)
          
-         208         374 LOAD_FAST                7 (inverted_scale)
+         227         374 LOAD_FAST                7 (inverted_scale)
          
-         209         376 LOAD_FAST                8 (grid_points)
+         228         376 LOAD_FAST                8 (grid_points)
          
-         202         378 PRECALL                  7
+         221         378 PRECALL                  7
                      382 CALL                     7
                      392 STORE_FAST               9 (bit_scores)
          
-         212         394 LOAD_FAST                9 (bit_scores)
+         231         394 LOAD_FAST                9 (bit_scores)
                      396 LOAD_ATTR                7 (ndim)
                      406 STORE_FAST              10 (@py_assert1)
                      408 LOAD_CONST               8 (2)
                      410 STORE_FAST              11 (@py_assert4)
                      412 LOAD_FAST               10 (@py_assert1)
                      414 LOAD_FAST               11 (@py_assert4)
                      416 COMPARE_OP               2 (==)
@@ -3958,15 +4638,15 @@
                  >>  810 LOAD_CONST               0 (None)
                      812 COPY                     1
                      814 STORE_FAST              10 (@py_assert1)
                      816 COPY                     1
                      818 STORE_FAST              12 (@py_assert3)
                      820 STORE_FAST              11 (@py_assert4)
          
-         213         822 LOAD_FAST                9 (bit_scores)
+         232         822 LOAD_FAST                9 (bit_scores)
                      824 LOAD_ATTR               17 (size)
                      834 STORE_FAST              10 (@py_assert1)
                      836 LOAD_CONST               2 (1)
                      838 STORE_FAST              12 (@py_assert3)
                      840 PUSH_NULL
                      842 LOAD_FAST               10 (@py_assert1)
                      844 LOAD_FAST               12 (@py_assert3)
@@ -4076,15 +4756,15 @@
                     1428 STORE_FAST              10 (@py_assert1)
                     1430 COPY                     1
                     1432 STORE_FAST              12 (@py_assert3)
                     1434 COPY                     1
                     1436 STORE_FAST              15 (@py_assert5)
                     1438 STORE_FAST              16 (@py_assert7)
          
-         214        1440 LOAD_FAST                9 (bit_scores)
+         233        1440 LOAD_FAST                9 (bit_scores)
                     1442 LOAD_ATTR               17 (size)
                     1452 STORE_FAST              10 (@py_assert1)
                     1454 LOAD_CONST               7 (0)
                     1456 STORE_FAST              12 (@py_assert3)
                     1458 PUSH_NULL
                     1460 LOAD_FAST               10 (@py_assert1)
                     1462 LOAD_FAST               12 (@py_assert3)
@@ -4182,15 +4862,15 @@
                     1966 STORE_FAST              12 (@py_assert3)
                     1968 COPY                     1
                     1970 STORE_FAST              15 (@py_assert5)
                     1972 COPY                     1
                     1974 STORE_FAST              16 (@py_assert7)
                     1976 STORE_FAST              19 (@py_assert8)
          
-         215        1978 LOAD_GLOBAL              0 (torch)
+         234        1978 LOAD_GLOBAL              0 (torch)
                     1990 LOAD_ATTR               18 (all)
                     2000 STORE_FAST              10 (@py_assert1)
                     2002 LOAD_FAST                9 (bit_scores)
                     2004 LOAD_FAST                4 (z_adjusted)
                     2006 LOAD_FAST                2 (start_z_adjusted)
                     2008 COMPARE_OP               0 (<)
                     2014 BINARY_SUBSCR
@@ -4331,17 +5011,17 @@
             '\n>assert %(py11)s\n{%(py11)s = %(py2)s\n{%(py2)s = %(py0)s.all\n}(%(py9)s)\n}'
             'torch'
             ('py0', 'py2', 'py9', 'py11')
          names      ('torch', 'manual_seed', 'full', 'randn', 'tensor', 'ones', '_compute_multi_dimensional_bit_scores', 'ndim', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'size', 'all')
          varnames   ('irt_scorer', 'latent_variables', 'start_z_adjusted', 'train_z_adjusted', 'z_adjusted', 'grid_start', 'grid_end', 'inverted_scale', 'grid_points', 'bit_scores', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert5', '@py_assert7', '@py_format9', '@py_format11', '@py_assert8', '@py_format10', '@py_format12', '@py_assert6', '@py_assert10')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'test_compute_multi_dimensional_bit_scores'
-         firstlineno 191
+         firstlineno 210
          lnotab
             0x020128012e012a012a01320132012c0114010402180102010201020102
             010201020102f9100aff00ad01ff00ff006c01ff00ff001c01
       'base_irt_model'
       code
          argcount  : 2
          nlocals   : 12
@@ -4379,36 +5059,36 @@
             0b00000000000000007c08a6010000ab0100000000000000007413000000
             000000000000006a0b00000000000000007c09a6010000ab010000000000
             0000007413000000000000000000006a0b00000000000000007c0aa60100
             00ab01000000000000000064109c097a0600007d0b741900000000000000
             0000007413000000000000000000006a0d00000000000000007c0ba60100
             00ab010000000000000000a6010000ab0100000000000000008201640078
             017d0578017d0678017d0778017d0878017d097d0a64005300
-         217           0 RESUME                   0
+         236           0 RESUME                   0
          
-         218           2 LOAD_FAST                1 (base_irt_model)
+         237           2 LOAD_FAST                1 (base_irt_model)
                        4 LOAD_FAST                0 (irt_scorer)
                        6 STORE_ATTR               0 (model)
          
-         220          16 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 220>)
+         239          16 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 239>)
                       18 MAKE_FUNCTION            0
                       20 STORE_FAST               2 (item_probabilities_mock)
          
-         225          22 LOAD_GLOBAL              3 (NULL + MagicMock)
+         244          22 LOAD_GLOBAL              3 (NULL + MagicMock)
          
-         226          34 LOAD_FAST                2 (item_probabilities_mock)
+         245          34 LOAD_FAST                2 (item_probabilities_mock)
          
-         225          36 KW_NAMES                 2
+         244          36 KW_NAMES                 2
                       38 PRECALL                  1
                       42 CALL                     1
                       52 LOAD_FAST                0 (irt_scorer)
                       54 LOAD_ATTR                0 (model)
                       64 STORE_ATTR               2 (item_probabilities)
          
-         229          74 LOAD_GLOBAL              7 (NULL + torch)
+         248          74 LOAD_GLOBAL              7 (NULL + torch)
                       86 LOAD_ATTR                4 (tensor)
                       96 LOAD_CONST               3 (-2.0)
                       98 LOAD_CONST               4 (-3.0)
                      100 BUILD_LIST               2
                      102 LOAD_CONST               5 (1.0)
                      104 LOAD_CONST               6 (2.0)
                      106 BUILD_LIST               2
@@ -4416,22 +5096,22 @@
                      110 LOAD_CONST               5 (1.0)
                      112 BUILD_LIST               2
                      114 BUILD_LIST               3
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               3 (input_z)
          
-         230         132 LOAD_FAST                0 (irt_scorer)
+         249         132 LOAD_FAST                0 (irt_scorer)
                      134 LOAD_METHOD              5 (expected_item_score_slopes)
                      156 LOAD_FAST                3 (input_z)
                      158 PRECALL                  1
                      162 CALL                     1
                      172 STORE_FAST               4 (expected_item_scores)
          
-         232         174 LOAD_GLOBAL              6 (torch)
+         251         174 LOAD_GLOBAL              6 (torch)
                      186 LOAD_ATTR                6 (allclose)
                      196 STORE_FAST               5 (@py_assert1)
                      198 LOAD_GLOBAL              6 (torch)
                      210 LOAD_ATTR                4 (tensor)
                      220 STORE_FAST               6 (@py_assert5)
                      222 LOAD_CONST               7 (0.2472)
                      224 LOAD_CONST               8 (0.1237)
@@ -4592,17 +5272,17 @@
                   0000000000000000000000000000000000640364046405a6030000ab0300
                   000000000000007c00a00300000000000000000000000000000000000000
                   006406ac07a6010000ab010000000000000000a004000000000000000000
                   0000000000000000000000640864066406a6030000ab0300000000000000
                   007a0500007d017400000000000000000000006a0500000000000000000b
                   007c016400640085026409640366033c000000740d000000000000000000
                   007c016404ac07a6020000ab0200000000000000005300
-               220           0 RESUME                   0
+               239           0 RESUME                   0
                
-               221           2 LOAD_GLOBAL              1 (NULL + torch)
+               240           2 LOAD_GLOBAL              1 (NULL + torch)
                             14 LOAD_ATTR                1 (tensor)
                             24 BUILD_LIST               0
                             26 LOAD_CONST               1 ((1, 2, 3, 0))
                             28 LIST_EXTEND              1
                             30 BUILD_LIST               0
                             32 LOAD_CONST               2 ((4, 3, 2, 1))
                             34 LIST_EXTEND              1
@@ -4627,27 +5307,27 @@
                            162 LOAD_CONST               6 (1)
                            164 LOAD_CONST               6 (1)
                            166 PRECALL                  3
                            170 CALL                     3
                            180 BINARY_OP                5 (*)
                            184 STORE_FAST               1 (logits)
                
-               222         186 LOAD_GLOBAL              0 (torch)
+               241         186 LOAD_GLOBAL              0 (torch)
                            198 LOAD_ATTR                5 (inf)
                            208 UNARY_NEGATIVE
                            210 LOAD_FAST                1 (logits)
                            212 LOAD_CONST               0 (None)
                            214 LOAD_CONST               0 (None)
                            216 BUILD_SLICE              2
                            218 LOAD_CONST               9 (0)
                            220 LOAD_CONST               3 (3)
                            222 BUILD_TUPLE              3
                            224 STORE_SUBSCR
                
-               223         228 LOAD_GLOBAL             13 (NULL + softmax)
+               242         228 LOAD_GLOBAL             13 (NULL + softmax)
                            240 LOAD_FAST                1 (logits)
                            242 LOAD_CONST               4 (2)
                            244 KW_NAMES                 7
                            246 PRECALL                  2
                            250 CALL                     2
                            260 RETURN_VALUE
                consts
@@ -4661,17 +5341,17 @@
                   ('dim',)
                   -1
                   0
                names      ('torch', 'tensor', 'expand', 'sum', 'reshape', 'inf', 'softmax')
                varnames   ('z', 'logits')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'item_probabilities_mock'
-               firstlineno 220
+               firstlineno 239
                lnotab 0x0201b8012a01
             ('side_effect',)
             -2.0
             -3.0
             1.0
             2.0
             0.2472
@@ -4684,17 +5364,17 @@
             'torch'
             'expected_item_scores'
             ('py0', 'py2', 'py3', 'py4', 'py6', 'py8', 'py10', 'py12', 'py14')
          names      ('model', 'MagicMock', 'item_probabilities', 'torch', 'tensor', 'expected_item_score_slopes', 'allclose', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('irt_scorer', 'base_irt_model', 'item_probabilities_mock', 'input_z', 'expected_item_scores', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_assert13', '@py_format15')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'test_expected_item_score_slopes'
-         firstlineno 217
+         firstlineno 236
          lnotab 0x02010e0206050c0102ff26043a012a02
       code
          argcount  : 1
          nlocals   : 13
          stacksize : 8
          flags     : 3
          code
@@ -4850,67 +5530,67 @@
             000000000000006a0c00000000000000007c0aa6010000ab010000000000
             00000072147411000000000000000000006a0d00000000000000007c0aa6
             010000ab0100000000000000006e01641d7411000000000000000000006a
             0d00000000000000007c0ba6010000ab010000000000000000641e9c057a
             0600007d0c741d000000000000000000007411000000000000000000006a
             0f00000000000000007c0ca6010000ab010000000000000000a6010000ab
             0100000000000000008201640078017d057d0b6400530064005300
-         234           0 RESUME                   0
+         253           0 RESUME                   0
          
-         235           2 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 235>)
+         254           2 LOAD_CONST               1 (<code object item_probabilities_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 254>)
                        4 MAKE_FUNCTION            0
                        6 STORE_FAST               1 (item_probabilities_mock)
          
-         239           8 LOAD_GLOBAL              1 (NULL + MagicMock)
+         258           8 LOAD_GLOBAL              1 (NULL + MagicMock)
          
-         240          20 LOAD_FAST                1 (item_probabilities_mock)
+         259          20 LOAD_FAST                1 (item_probabilities_mock)
          
-         239          22 KW_NAMES                 2
+         258          22 KW_NAMES                 2
                       24 PRECALL                  1
                       28 CALL                     1
                       38 LOAD_FAST                0 (irt_scorer)
                       40 LOAD_ATTR                1 (model)
                       50 STORE_ATTR               2 (item_probabilities)
          
-         243          60 LOAD_CONST               3 (<code object probability_gradients_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_irt_scorer.py", line 243>)
+         262          60 LOAD_CONST               3 (<code object probability_gradients_mock, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_irt_scorer.py", line 262>)
                       62 MAKE_FUNCTION            0
                       64 STORE_FAST               2 (probability_gradients_mock)
          
-         249          66 LOAD_GLOBAL              1 (NULL + MagicMock)
+         268          66 LOAD_GLOBAL              1 (NULL + MagicMock)
          
-         250          78 LOAD_FAST                2 (probability_gradients_mock)
+         269          78 LOAD_FAST                2 (probability_gradients_mock)
          
-         249          80 KW_NAMES                 2
+         268          80 KW_NAMES                 2
                       82 PRECALL                  1
                       86 CALL                     1
                       96 LOAD_FAST                0 (irt_scorer)
                       98 LOAD_ATTR                1 (model)
                      108 STORE_ATTR               3 (probability_gradients)
          
-         253         118 LOAD_GLOBAL              9 (NULL + torch)
+         272         118 LOAD_GLOBAL              9 (NULL + torch)
                      130 LOAD_ATTR                5 (tensor)
                      140 LOAD_CONST               4 (1.0)
                      142 LOAD_CONST               5 (2.0)
                      144 BUILD_LIST               2
                      146 LOAD_CONST               6 (3.0)
                      148 LOAD_CONST               7 (4.0)
                      150 BUILD_LIST               2
                      152 BUILD_LIST               2
                      154 PRECALL                  1
                      158 CALL                     1
                      168 STORE_FAST               3 (input_z)
          
-         254         170 LOAD_FAST                0 (irt_scorer)
+         273         170 LOAD_FAST                0 (irt_scorer)
                      172 LOAD_METHOD              6 (information)
                      194 LOAD_FAST                3 (input_z)
                      196 PRECALL                  1
                      200 CALL                     1
                      210 STORE_FAST               4 (information_matrices)
          
-         255         212 LOAD_FAST                4 (information_matrices)
+         274         212 LOAD_FAST                4 (information_matrices)
                      214 LOAD_ATTR                7 (shape)
                      224 STORE_FAST               5 (@py_assert1)
                      226 LOAD_CONST               8 ((2, 2, 2, 2))
                      228 STORE_FAST               6 (@py_assert4)
                      230 LOAD_FAST                5 (@py_assert1)
                      232 LOAD_FAST                6 (@py_assert4)
                      234 COMPARE_OP               2 (==)
@@ -4980,18 +5660,18 @@
                  >>  586 LOAD_CONST               0 (None)
                      588 COPY                     1
                      590 STORE_FAST               5 (@py_assert1)
                      592 COPY                     1
                      594 STORE_FAST               7 (@py_assert3)
                      596 STORE_FAST               6 (@py_assert4)
          
-         256         598 LOAD_GLOBAL              9 (NULL + torch)
+         275         598 LOAD_GLOBAL              9 (NULL + torch)
                      610 LOAD_ATTR                5 (tensor)
          
-         257         620 LOAD_CONST              15 (4184.934082)
+         276         620 LOAD_CONST              15 (4184.934082)
                      622 LOAD_CONST              16 (4786.79834)
                      624 BUILD_LIST               2
                      626 LOAD_CONST              16 (4786.79834)
                      628 LOAD_CONST              17 (5478.406738)
                      630 BUILD_LIST               2
                      632 BUILD_LIST               2
                      634 LOAD_CONST              18 (19931.039062)
@@ -4999,15 +5679,15 @@
                      638 BUILD_LIST               2
                      640 LOAD_CONST              19 (21267.791016)
                      642 LOAD_CONST              20 (22694.289062)
                      644 BUILD_LIST               2
                      646 BUILD_LIST               2
                      648 BUILD_LIST               2
          
-         258         650 LOAD_CONST              21 (646821568)
+         277         650 LOAD_CONST              21 (646821568)
                      652 LOAD_CONST              22 (739235008)
                      654 BUILD_LIST               2
                      656 LOAD_CONST              22 (739235008)
                      658 LOAD_CONST              23 (844860736)
                      660 BUILD_LIST               2
                      662 BUILD_LIST               2
                      664 LOAD_CONST              24 (2972079104)
@@ -5015,20 +5695,20 @@
                      668 BUILD_LIST               2
                      670 LOAD_CONST              25 (3170238464)
                      672 LOAD_CONST              26 (3381610496)
                      674 BUILD_LIST               2
                      676 BUILD_LIST               2
                      678 BUILD_LIST               2
          
-         256         680 BUILD_LIST               2
+         275         680 BUILD_LIST               2
                      682 PRECALL                  1
                      686 CALL                     1
                      696 STORE_FAST              10 (expected_output)
          
-         260         698 LOAD_GLOBAL              8 (torch)
+         279         698 LOAD_GLOBAL              8 (torch)
                      710 LOAD_ATTR               16 (allclose)
                      720 STORE_FAST               5 (@py_assert1)
                      722 PUSH_NULL
                      724 LOAD_FAST                5 (@py_assert1)
                      726 LOAD_FAST                4 (information_matrices)
                      728 LOAD_FAST               10 (expected_output)
                      730 PRECALL                  2
@@ -5122,34 +5802,34 @@
                     1286 CALL                     1
                     1296 RAISE_VARARGS            1
                  >> 1298 LOAD_CONST               0 (None)
                     1300 COPY                     1
                     1302 STORE_FAST               5 (@py_assert1)
                     1304 STORE_FAST              11 (@py_assert5)
          
-         263        1306 LOAD_FAST                0 (irt_scorer)
+         282        1306 LOAD_FAST                0 (irt_scorer)
                     1308 LOAD_ATTR                1 (model)
                     1318 LOAD_ATTR               17 (latent_variables)
                     1328 LOAD_CONST              31 (2)
                     1330 COMPARE_OP               2 (==)
                     1336 EXTENDED_ARG             2
                     1338 POP_JUMP_FORWARD_IF_FALSE   548 (to 2436)
          
-         264        1340 LOAD_FAST                0 (irt_scorer)
+         283        1340 LOAD_FAST                0 (irt_scorer)
                     1342 LOAD_METHOD              6 (information)
                     1364 LOAD_FAST                3 (input_z)
                     1366 LOAD_CONST              32 (45)
                     1368 LOAD_CONST              32 (45)
                     1370 BUILD_LIST               2
                     1372 KW_NAMES                33
                     1374 PRECALL                  2
                     1378 CALL                     2
                     1388 STORE_FAST               4 (information_matrices)
          
-         265        1390 LOAD_FAST                4 (information_matrices)
+         284        1390 LOAD_FAST                4 (information_matrices)
                     1392 LOAD_ATTR                7 (shape)
                     1402 STORE_FAST               5 (@py_assert1)
                     1404 LOAD_CONST              34 ((2, 2))
                     1406 STORE_FAST               6 (@py_assert4)
                     1408 LOAD_FAST                5 (@py_assert1)
                     1410 LOAD_FAST                6 (@py_assert4)
                     1412 COMPARE_OP               2 (==)
@@ -5219,31 +5899,31 @@
                  >> 1764 LOAD_CONST               0 (None)
                     1766 COPY                     1
                     1768 STORE_FAST               5 (@py_assert1)
                     1770 COPY                     1
                     1772 STORE_FAST               7 (@py_assert3)
                     1774 STORE_FAST               6 (@py_assert4)
          
-         266        1776 LOAD_GLOBAL              9 (NULL + torch)
+         285        1776 LOAD_GLOBAL              9 (NULL + torch)
                     1788 LOAD_ATTR                5 (tensor)
          
-         267        1798 LOAD_CONST              35 (9618.4677734)
+         286        1798 LOAD_CONST              35 (9618.4677734)
                     1800 LOAD_CONST              36 (42580.453125)
                     1802 BUILD_LIST               2
          
-         268        1804 LOAD_CONST              37 (1485075968.0)
+         287        1804 LOAD_CONST              37 (1485075968.0)
                     1806 LOAD_CONST              38 (6347082752.0)
                     1808 BUILD_LIST               2
          
-         266        1810 BUILD_LIST               2
+         285        1810 BUILD_LIST               2
                     1812 PRECALL                  1
                     1816 CALL                     1
                     1826 STORE_FAST              10 (expected_output)
          
-         270        1828 LOAD_GLOBAL              8 (torch)
+         289        1828 LOAD_GLOBAL              8 (torch)
                     1840 LOAD_ATTR               16 (allclose)
                     1850 STORE_FAST               5 (@py_assert1)
                     1852 PUSH_NULL
                     1854 LOAD_FAST                5 (@py_assert1)
                     1856 LOAD_FAST                4 (information_matrices)
                     1858 LOAD_FAST               10 (expected_output)
                     1860 PRECALL                  2
@@ -5337,24 +6017,24 @@
                     2416 CALL                     1
                     2426 RAISE_VARARGS            1
                  >> 2428 LOAD_CONST               0 (None)
                     2430 COPY                     1
                     2432 STORE_FAST               5 (@py_assert1)
                     2434 STORE_FAST              11 (@py_assert5)
          
-         273     >> 2436 LOAD_FAST                0 (irt_scorer)
+         292     >> 2436 LOAD_FAST                0 (irt_scorer)
                     2438 LOAD_METHOD              6 (information)
                     2460 LOAD_FAST                3 (input_z)
                     2462 LOAD_CONST              39 (False)
                     2464 KW_NAMES                40
                     2466 PRECALL                  2
                     2470 CALL                     2
                     2480 STORE_FAST               4 (information_matrices)
          
-         274        2482 LOAD_FAST                4 (information_matrices)
+         293        2482 LOAD_FAST                4 (information_matrices)
                     2484 LOAD_ATTR                7 (shape)
                     2494 STORE_FAST               5 (@py_assert1)
                     2496 LOAD_CONST              41 ((2, 2, 2))
                     2498 STORE_FAST               6 (@py_assert4)
                     2500 LOAD_FAST                5 (@py_assert1)
                     2502 LOAD_FAST                6 (@py_assert4)
                     2504 COMPARE_OP               2 (==)
@@ -5424,39 +6104,39 @@
                  >> 2856 LOAD_CONST               0 (None)
                     2858 COPY                     1
                     2860 STORE_FAST               5 (@py_assert1)
                     2862 COPY                     1
                     2864 STORE_FAST               7 (@py_assert3)
                     2866 STORE_FAST               6 (@py_assert4)
          
-         275        2868 LOAD_GLOBAL              9 (NULL + torch)
+         294        2868 LOAD_GLOBAL              9 (NULL + torch)
                     2880 LOAD_ATTR                5 (tensor)
          
-         276        2890 LOAD_CONST              42 (24115.972656)
+         295        2890 LOAD_CONST              42 (24115.972656)
                     2892 LOAD_CONST              43 (26054.589844)
                     2894 BUILD_LIST               2
                     2896 LOAD_CONST              43 (26054.589844)
                     2898 LOAD_CONST              44 (28172.695312)
                     2900 BUILD_LIST               2
                     2902 BUILD_LIST               2
          
-         277        2904 LOAD_CONST              45 (3618900480)
+         296        2904 LOAD_CONST              45 (3618900480)
                     2906 LOAD_CONST              46 (3909473536)
                     2908 BUILD_LIST               2
                     2910 LOAD_CONST              46 (3909473536)
                     2912 LOAD_CONST              47 (4226471168)
                     2914 BUILD_LIST               2
                     2916 BUILD_LIST               2
          
-         275        2918 BUILD_LIST               2
+         294        2918 BUILD_LIST               2
                     2920 PRECALL                  1
                     2924 CALL                     1
                     2934 STORE_FAST              10 (expected_output)
          
-         279        2936 LOAD_GLOBAL              8 (torch)
+         298        2936 LOAD_GLOBAL              8 (torch)
                     2948 LOAD_ATTR               16 (allclose)
                     2958 STORE_FAST               5 (@py_assert1)
                     2960 PUSH_NULL
                     2962 LOAD_FAST                5 (@py_assert1)
                     2964 LOAD_FAST                4 (information_matrices)
                     2966 LOAD_FAST               10 (expected_output)
                     2968 PRECALL                  2
@@ -5550,35 +6230,35 @@
                     3524 CALL                     1
                     3534 RAISE_VARARGS            1
                  >> 3536 LOAD_CONST               0 (None)
                     3538 COPY                     1
                     3540 STORE_FAST               5 (@py_assert1)
                     3542 STORE_FAST              11 (@py_assert5)
          
-         282        3544 LOAD_FAST                0 (irt_scorer)
+         301        3544 LOAD_FAST                0 (irt_scorer)
                     3546 LOAD_ATTR                1 (model)
                     3556 LOAD_ATTR               17 (latent_variables)
                     3566 LOAD_CONST              31 (2)
                     3568 COMPARE_OP               2 (==)
                     3574 EXTENDED_ARG             2
                     3576 POP_JUMP_FORWARD_IF_FALSE   547 (to 4672)
          
-         283        3578 LOAD_FAST                0 (irt_scorer)
+         302        3578 LOAD_FAST                0 (irt_scorer)
                     3580 LOAD_METHOD              6 (information)
                     3602 LOAD_FAST                3 (input_z)
                     3604 LOAD_CONST              39 (False)
                     3606 LOAD_CONST              48 (0)
                     3608 LOAD_CONST              49 (90)
                     3610 BUILD_LIST               2
                     3612 KW_NAMES                50
                     3614 PRECALL                  3
                     3618 CALL                     3
                     3628 STORE_FAST               4 (information_matrices)
          
-         284        3630 LOAD_FAST                4 (information_matrices)
+         303        3630 LOAD_FAST                4 (information_matrices)
                     3632 LOAD_ATTR                7 (shape)
                     3642 STORE_FAST               5 (@py_assert1)
                     3644 LOAD_CONST              51 ((2,))
                     3646 STORE_FAST               6 (@py_assert4)
                     3648 LOAD_FAST                5 (@py_assert1)
                     3650 LOAD_FAST                6 (@py_assert4)
                     3652 COMPARE_OP               2 (==)
@@ -5648,24 +6328,24 @@
                  >> 4004 LOAD_CONST               0 (None)
                     4006 COPY                     1
                     4008 STORE_FAST               5 (@py_assert1)
                     4010 COPY                     1
                     4012 STORE_FAST               7 (@py_assert3)
                     4014 STORE_FAST               6 (@py_assert4)
          
-         285        4016 LOAD_GLOBAL              9 (NULL + torch)
+         304        4016 LOAD_GLOBAL              9 (NULL + torch)
                     4028 LOAD_ATTR                5 (tensor)
                     4038 LOAD_CONST              42 (24115.972656)
                     4040 LOAD_CONST              52 (3618899968.0)
                     4042 BUILD_LIST               2
                     4044 PRECALL                  1
                     4048 CALL                     1
                     4058 STORE_FAST              10 (expected_output)
          
-         286        4060 LOAD_GLOBAL              8 (torch)
+         305        4060 LOAD_GLOBAL              8 (torch)
                     4072 LOAD_ATTR               16 (allclose)
                     4082 STORE_FAST               5 (@py_assert1)
                     4084 PUSH_NULL
                     4086 LOAD_FAST                5 (@py_assert1)
                     4088 LOAD_FAST                4 (information_matrices)
                     4090 LOAD_FAST               10 (expected_output)
                     4092 PRECALL                  2
@@ -5761,15 +6441,15 @@
                  >> 4660 LOAD_CONST               0 (None)
                     4662 COPY                     1
                     4664 STORE_FAST               5 (@py_assert1)
                     4666 STORE_FAST              11 (@py_assert5)
                     4668 LOAD_CONST               0 (None)
                     4670 RETURN_VALUE
          
-         282     >> 4672 LOAD_CONST               0 (None)
+         301     >> 4672 LOAD_CONST               0 (None)
                     4674 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
@@ -5779,17 +6459,17 @@
                   0167006402a20167026701a6010000ab010000000000000000a002000000
                   0000000000000000000000000000000000640364036404a6030000ab0300
                   000000000000007c00a00300000000000000000000000000000000000000
                   006405ac06a6010000ab010000000000000000a004000000000000000000
                   0000000000000000000000640764056405a6030000ab0300000000000000
                   007a0500007d01740b000000000000000000007c016403ac06a6020000ab
                   0200000000000000005300
-               235           0 RESUME                   0
+               254           0 RESUME                   0
                
-               236           2 LOAD_GLOBAL              1 (NULL + torch)
+               255           2 LOAD_GLOBAL              1 (NULL + torch)
                             14 LOAD_ATTR                1 (tensor)
                             24 BUILD_LIST               0
                             26 LOAD_CONST               1 ((1, 2, 3, 0))
                             28 LIST_EXTEND              1
                             30 BUILD_LIST               0
                             32 LOAD_CONST               2 ((4, 3, 2, 1))
                             34 LIST_EXTEND              1
@@ -5814,15 +6494,15 @@
                            162 LOAD_CONST               5 (1)
                            164 LOAD_CONST               5 (1)
                            166 PRECALL                  3
                            170 CALL                     3
                            180 BINARY_OP                5 (*)
                            184 STORE_FAST               1 (logits)
                
-               237         186 LOAD_GLOBAL             11 (NULL + softmax)
+               256         186 LOAD_GLOBAL             11 (NULL + softmax)
                            198 LOAD_FAST                1 (logits)
                            200 LOAD_CONST               3 (2)
                            202 KW_NAMES                 6
                            204 PRECALL                  2
                            208 CALL                     2
                            218 RETURN_VALUE
                consts
@@ -5834,37 +6514,37 @@
                   1
                   ('dim',)
                   -1
                names      ('torch', 'tensor', 'expand', 'sum', 'reshape', 'softmax')
                varnames   ('z', 'logits')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'item_probabilities_mock'
-               firstlineno 235
+               firstlineno 254
                lnotab 0x0201b801
             ('side_effect',)
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 9
                flags     : 19
                code
                   0x97007401000000000000000000006a0100000000000000006401640267
                   0264036404670264056406670264076408670267046409640a6702640b64
                   0c6702640d640e6702640f64106702670467026401640267026403640467
                   0264056406670264076408670267046409640a6702640b640c6702640d64
                   0e6702640f64106702670467026702a6010000ab01000000000000000053
                   00
-               243           0 RESUME                   0
+               262           0 RESUME                   0
                
-               244           2 LOAD_GLOBAL              1 (NULL + torch)
+               263           2 LOAD_GLOBAL              1 (NULL + torch)
                             14 LOAD_ATTR                1 (tensor)
                
-               245          24 LOAD_CONST               1 (0.1)
+               264          24 LOAD_CONST               1 (0.1)
                             26 LOAD_CONST               2 (0.2)
                             28 BUILD_LIST               2
                             30 LOAD_CONST               3 (0.3)
                             32 LOAD_CONST               4 (0.4)
                             34 BUILD_LIST               2
                             36 LOAD_CONST               5 (0.5)
                             38 LOAD_CONST               6 (0.6)
@@ -5884,15 +6564,15 @@
                             66 BUILD_LIST               2
                             68 LOAD_CONST              15 (1.5)
                             70 LOAD_CONST              16 (1.6)
                             72 BUILD_LIST               2
                             74 BUILD_LIST               4
                             76 BUILD_LIST               2
                
-               246          78 LOAD_CONST               1 (0.1)
+               265          78 LOAD_CONST               1 (0.1)
                             80 LOAD_CONST               2 (0.2)
                             82 BUILD_LIST               2
                             84 LOAD_CONST               3 (0.3)
                             86 LOAD_CONST               4 (0.4)
                             88 BUILD_LIST               2
                             90 LOAD_CONST               5 (0.5)
                             92 LOAD_CONST               6 (0.6)
@@ -5912,15 +6592,15 @@
                            120 BUILD_LIST               2
                            122 LOAD_CONST              15 (1.5)
                            124 LOAD_CONST              16 (1.6)
                            126 BUILD_LIST               2
                            128 BUILD_LIST               4
                            130 BUILD_LIST               2
                
-               244         132 BUILD_LIST               2
+               263         132 BUILD_LIST               2
                            134 PRECALL                  1
                            138 CALL                     1
                            148 RETURN_VALUE
                consts
                   None
                   0.1
                   0.2
@@ -5938,17 +6618,17 @@
                   1.4
                   1.5
                   1.6
                names      ('torch', 'tensor')
                varnames   ('z',)
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
                name       'probability_gradients_mock'
-               firstlineno 243
+               firstlineno 262
                lnotab 0x02011601360136fe
             1.0
             2.0
             3.0
             4.0
             (2, 2, 2, 2)
             ('==',)
@@ -5995,26 +6675,26 @@
             ('item', 'degrees')
             (2,)
             3618899968.0
          names      ('MagicMock', 'model', 'item_probabilities', 'probability_gradients', 'torch', 'tensor', 'information', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'allclose', 'latent_variables')
          varnames   ('irt_scorer', 'item_probabilities_mock', 'probability_gradients_mock', 'input_z', 'information_matrices', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'expected_output', '@py_assert5', '@py_format7')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
          name       'test_information'
-         firstlineno 234
+         firstlineno 253
          lnotab
             0x020106040c0102ff260406060c0102ff260434012a01ff00830116011e
             011efe1204ff00ff00620322013201ff0083011601060106fe1204ff00ff
             0062032e01ff00830116010e010efe1204ff00ff00620322013401ff0083
             012c01ff00ff0066fc
-   names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'unittest.mock', 'MagicMock', 'patch', 'torch', 'torch.nn.functional', 'softmax', 'pytest', 'irtorch.irt_scorer', 'IRTScorer', 'irtorch.estimation_algorithms', 'AEIRT', 'irtorch.models', 'BaseIRTModel', 'ConcreteIRTModel', 'fixture', 'base_irt_model', 'irt_scorer', 'mark', 'parametrize', 'test_bit_scores', 'test_latent_scores', 'test_z_grid', 'test_compute_1d_bit_scores', 'test_compute_multi_dimensional_bit_scores', 'test_expected_item_score_slopes', 'test_information')
+   names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'unittest.mock', 'MagicMock', 'patch', 'torch', 'torch.nn.functional', 'softmax', 'pytest', 'irtorch.irt_scorer', 'IRTScorer', 'irtorch.estimation_algorithms', 'AEIRT', 'irtorch.models', 'BaseIRTModel', 'ConcreteIRTModel', 'fixture', 'base_irt_model', 'irt_scorer', 'GaussianMixtureModel', 'mark', 'parametrize', 'test_cv_gaussian_mixture_model', 'test_bit_scores', 'test_latent_scores', 'test_z_grid', 'test_compute_1d_bit_scores', 'test_compute_multi_dimensional_bit_scores', 'test_expected_item_score_slopes', 'test_information')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_irt_scorer.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_irt_scorer.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02012a0108010c0108010c010c010c021c0a0c0104ff0e0102030c
-      0104ff0e01023e380138010aff0eff0e02021e38010aff0e01021338010a
-      ff0e01021c0c180c1a1011
+      0104ff0e01023d0c010c023e010aff0e010210380138010aff0eff0e0202
+      1e38010aff0e01021338010aff0e01021c0c180c1a1011
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_latent_variable_functions.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_latent_variable_functions.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -47,19 +47,19 @@
                 60 IMPORT_NAME             10 (irtorch.latent_variable_functions)
                 62 IMPORT_FROM             11 (interp)
                 64 STORE_NAME              11 (interp)
                 66 IMPORT_FROM             12 (quantile_transform)
                 68 STORE_NAME              12 (quantile_transform)
                 70 POP_TOP
    
-     6          72 LOAD_CONST               3 (<code object test_interp, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_latent_variable_functions.py", line 6>)
+     6          72 LOAD_CONST               3 (<code object test_interp, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_latent_variable_functions.py", line 6>)
                 74 MAKE_FUNCTION            0
                 76 STORE_NAME              13 (test_interp)
    
-    23          78 LOAD_CONST               4 (<code object test_quantile_transform, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_latent_variable_functions.py", line 23>)
+    23          78 LOAD_CONST               4 (<code object test_quantile_transform, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_latent_variable_functions.py", line 23>)
                 80 MAKE_FUNCTION            0
                 82 STORE_NAME              14 (test_quantile_transform)
                 84 LOAD_CONST               1 (None)
                 86 RETURN_VALUE
    consts
       0
       None
@@ -315,15 +315,15 @@
             'y_new'
             'y_new_expected'
             ('py0', 'py2', 'py3', 'py4', 'py6', 'py8')
          names      ('torch', 'tensor', 'interp', 'allclose', '@pytest_ar', '_format_assertmsg', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('x', 'y', 'x_new', 'y_new_expected', 'y_new', '@py_assert1', '@py_assert5', '@py_assert7', '@py_format9')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_latent_variable_functions.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_latent_variable_functions.py'
          name       'test_interp'
          firstlineno 6
          lnotab
             0x02012c012c01160106ff1003160106ff100422020c020afe34020afe24
             020afe1e020afe28020afe2a020afe1e020afe1e020afe1e020afe22020a
             fe1e020afe1e020afe20020afe1c020afe32020afe
       code
@@ -1375,15 +1375,15 @@
           54        3542 LOAD_GLOBAL              1 (NULL + torch)
                     3554 LOAD_ATTR               26 (stack)
          
           55        3564 LOAD_CLOSURE            34 (cat)
                     3566 LOAD_CLOSURE            35 (means)
                     3568 LOAD_CLOSURE            36 (std_devs)
                     3570 BUILD_TUPLE              3
-                    3572 LOAD_CONST              33 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_latent_variable_functions.py", line 55>)
+                    3572 LOAD_CONST              33 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_latent_variable_functions.py", line 55>)
                     3574 MAKE_FUNCTION            8 (closure)
          
           57        3576 LOAD_GLOBAL             11 (NULL + range)
                     3588 LOAD_CONST              34 (3000)
                     3590 PRECALL                  1
                     3594 CALL                     1
          
@@ -2635,15 +2635,15 @@
                            150 JUMP_BACKWARD           72 (to 8)
                        >>  152 RETURN_VALUE
                consts
                names      ('torch', 'normal', 'sample')
                varnames   ('.0', '_')
                freevars   ('cat', 'means', 'std_devs')
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_latent_variable_functions.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_latent_variable_functions.py'
                name       '<listcomp>'
                firstlineno 55
                lnotab 0x0a0202ff88ff
             3000
             1000
             (1, 2, 2, 3, 4)
             (-0.9674, -0.4307, 0.0, 0.4307, 0.9674)
@@ -2655,15 +2655,15 @@
             ('py18', 'py20', 'py21', 'py22', 'py24', 'py26', 'py28', 'py30', 'py32')
             'assert %(py35)s'
             'py35'
          names      ('torch', 'arange', 'repeat', 'T', 'float', 'range', 'shape', 'randperm', 'quantile_transform', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'allclose', 'mean', 'tensor', 'std', 'stats', 'shapiro', 'cpu', 'distributions', 'Categorical', 'stack', 'reshape', 'append', '_format_boolop')
          varnames   ('data_tensor', 'i', 'tensor_transformed', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_assert6', '@py_assert8', '@py_assert11', '@py_assert13', '@py_assert15', '@py_assert17', '@py_assert19', '@py_format21', 'shapiro_test_p', '@py_assert2', '@py_format4', '@py_format6', 'probs', '@py_assert7', '@py_assert9', '@py_assert0', '@py_assert23', '@py_assert25', '@py_assert27', '@py_assert29', '@py_assert31', '@py_format17', '@py_format33', '@py_format34', '@py_format36')
          freevars   ()
          cellvars   ('cat', 'means', 'std_devs')
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_latent_variable_functions.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_latent_variable_functions.py'
          name       'test_quantile_transform'
          firstlineno 23
          lnotab
             0x0802840238016e021e01ff00ff000a010c040afc04040afc2a040afc56
             040afc1e040afc28040afc2a040afc1e040afc1e040afc1e040afc20040a
             fc1c040afc1c040afc1e040afc1e040afc28040afc2a040afc1c040afc1c
             040afc1c040afc1c040afc32040afc44050c040afc04040afc2a040afc56
@@ -2683,11 +2683,11 @@
             f816080af81e080af828080af82a080af81e080af81e080af81e080af822
             080af81e080af828080af82a080af81c080af81c080af81c080af81c080a
             f81c0816f8020810f80c080af840080af8
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'scipy.stats', 'stats', 'irtorch.latent_variable_functions', 'interp', 'quantile_transform', 'test_interp', 'test_quantile_transform')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_latent_variable_functions.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_latent_variable_functions.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201220108010c0110020611
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_layers.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_layers.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -41,31 +41,31 @@
                 48 IMPORT_NAME              8 (irtorch.layers)
                 50 IMPORT_FROM              9 (NegationLayer)
                 52 STORE_NAME               9 (NegationLayer)
                 54 IMPORT_FROM             10 (SoftplusLinear)
                 56 STORE_NAME              10 (SoftplusLinear)
                 58 POP_TOP
    
-     5          60 LOAD_CONST               3 (<code object test_SoftplusLinear_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_layers.py", line 5>)
+     5          60 LOAD_CONST               3 (<code object test_SoftplusLinear_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_layers.py", line 5>)
                 62 MAKE_FUNCTION            0
                 64 STORE_NAME              11 (test_SoftplusLinear_forward)
    
-    35          66 LOAD_CONST               4 (<code object test_SoftplusLinear_forward_with_separate_groups, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_layers.py", line 35>)
+    35          66 LOAD_CONST               4 (<code object test_SoftplusLinear_forward_with_separate_groups, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_layers.py", line 35>)
                 68 MAKE_FUNCTION            0
                 70 STORE_NAME              12 (test_SoftplusLinear_forward_with_separate_groups)
    
-    72          72 LOAD_CONST               5 (<code object test_NegationLayer_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_layers.py", line 72>)
+    72          72 LOAD_CONST               5 (<code object test_NegationLayer_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_layers.py", line 72>)
                 74 MAKE_FUNCTION            0
                 76 STORE_NAME              13 (test_NegationLayer_forward)
    
-    96          78 LOAD_CONST               6 (<code object test_NegationLayer_all_item_weights, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_layers.py", line 96>)
+    96          78 LOAD_CONST               6 (<code object test_NegationLayer_all_item_weights, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_layers.py", line 96>)
                 80 MAKE_FUNCTION            0
                 82 STORE_NAME              14 (test_NegationLayer_all_item_weights)
    
-   109          84 LOAD_CONST               7 (<code object test_separate_weights, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_layers.py", line 109>)
+   109          84 LOAD_CONST               7 (<code object test_separate_weights, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_layers.py", line 109>)
                 86 MAKE_FUNCTION            0
                 88 STORE_NAME              15 (test_separate_weights)
                 90 LOAD_CONST               1 (None)
                 92 RETURN_VALUE
    consts
       0
       None
@@ -1283,15 +1283,15 @@
             'Free weights should have changed'
             ('%(py3)s != %(py7)s\n{%(py7)s = %(py5)s.bias_param\n}',)
             'original_bias'
          names      ('torch', 'tensor', 'SoftplusLinear', 'raw_weight_param', 'clone', 'bias_param', 'optim', 'Adam', 'parameters', 'range', 'zero_grad', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'all', 'free_bias', 'bool', 'sum', 'backward', 'grad', 'step')
          varnames   ('zero_outputs', 'sp_linear', 'original_weights', 'original_bias', 'optimizer', '_', 'result', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert5', '@py_assert10', '@py_format12', '@py_assert9', '@py_assert8', '@py_assert13', '@py_format11', '@py_format15')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_layers.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_layers.py'
          name       'test_SoftplusLinear_forward'
          firstlineno 5
          lnotab
             0x02012c010c010201020102fd1206320132032c0130ff1203240128014c
             01ff00ad01ff00ff00a201ff00ff0024024c01ff00ff00fa01ff00ff00fa
             012c02ff00ff00ff001101
       code
@@ -2544,15 +2544,15 @@
             'Free weights should have changed'
             ('%(py3)s != %(py7)s\n{%(py7)s = %(py5)s.bias_param\n}',)
             'original_bias'
          names      ('torch', 'tensor', 'SoftplusLinear', 'raw_weight_param', 'clone', 'bias_param', 'optim', 'Adam', 'parameters', 'range', 'zero_grad', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'all', 'free_bias', 'bool', 'sum', 'backward', 'grad', 'step')
          varnames   ('zero_inputs', 'zero_outputs', 'sp_linear', 'original_weights', 'original_bias', 'optimizer', '_', 'result', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert5', '@py_assert10', '@py_format12', '@py_assert9', '@py_assert8', '@py_assert13', '@py_format11', '@py_format15')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_layers.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_layers.py'
          name       'test_SoftplusLinear_forward_with_separate_groups'
          firstlineno 35
          lnotab
             0x02012c012c010c01020102012a012a01020102fa1209320132032c0130
             ff1203240128012001060106fe2003ff00ad01ff00ff00a201ff00ff0024
             024c01ff00ff00fa01ff00ff00fa012c02ff00ff00ff001101
       code
@@ -3116,15 +3116,15 @@
             'assert %(py12)s\n{%(py12)s = %(py2)s\n{%(py2)s = %(py0)s.equal\n}(%(py3)s, %(py10)s\n{%(py10)s = %(py6)s\n{%(py6)s = %(py4)s.tensor\n}(%(py8)s)\n})\n}'
             'result'
             ('py0', 'py2', 'py3', 'py4', 'py6', 'py8', 'py10', 'py12')
          names      ('NegationLayer', 'torch', 'tensor', 'bool', 'no_grad', 'weight_param', 'fill_', 'sum', 'backward', 'all', 'grad', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'equal')
          varnames   ('neg_layer', 'input', 'result', '@py_assert1', '@py_assert4', '@py_assert6', '@py_assert9', '@py_assert8', '@py_assert13', '@py_format11', '@py_format15', '@py_assert5', '@py_assert7', '@py_assert11', '@py_format13')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_layers.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_layers.py'
          name       'test_NegationLayer_forward'
          firstlineno 72
          lnotab
             0x02010c012a0102014efd12052801400140fe2e0546011201160116024c
             01ff00ff00fa010c040afc0e040afc5c040afc1e040afc28040afc2a040a
             fc1e040afc1e040afc1e040afc22040afc1e040afc28040afc2a040afc1c
             040afc1c040afc1c040afc32040afc
@@ -3406,15 +3406,15 @@
             'neg_layer'
             'torch'
             ('py0', 'py2', 'py4', 'py6', 'py7', 'py9', 'py11', 'py13', 'py15')
          names      ('NegationLayer', 'torch', 'tensor', 'bool', 'no_grad', 'weight_param', 'fill_', 'all_item_weights', 'equal', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('neg_layer', '@py_assert1', '@py_assert3', '@py_assert5', '@py_assert8', '@py_assert10', '@py_assert12', '@py_assert14', '@py_format16')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_layers.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_layers.py'
          name       'test_NegationLayer_all_item_weights'
          firstlineno 96
          lnotab 0x02010c012a0102014efd12052801400140fe2e04
       code
          argcount  : 0
          nlocals   : 13
          stacksize : 7
@@ -4087,21 +4087,21 @@
             'torch'
             ('py0', 'py2', 'py9', 'py11')
             False
          names      ('torch', 'tensor', 'SoftplusLinear', 'separate_weights', 'in_features', 'out_features', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'all')
          varnames   ('separate_inputs', 'separate_outputs', 'model', 'result', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert5', '@py_assert10', '@py_format12')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_layers.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_layers.py'
          name       'test_separate_weights'
          firstlineno 109
          lnotab
             0x02012c012c0120014401ff009b01ff00ff002801ff00ff002801ff00ff
             002801
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'irtorch.layers', 'NegationLayer', 'SoftplusLinear', 'test_SoftplusLinear_forward', 'test_SoftplusLinear_forward_with_separate_groups', 'test_NegationLayer_forward', 'test_NegationLayer_all_item_weights', 'test_separate_weights')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_layers.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_layers.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201220108011002061e06250618060d
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_load_dataset.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_load_dataset.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -52,39 +52,39 @@
                 68 STORE_NAME              13 (swedish_sat)
                 70 IMPORT_FROM             14 (swedish_sat_binary)
                 72 STORE_NAME              14 (swedish_sat_binary)
                 74 IMPORT_FROM             15 (big_five)
                 76 STORE_NAME              15 (big_five)
                 78 POP_TOP
    
-     5          80 LOAD_CONST               3 (<code object test_swedish_national_mathematics_2, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 5>)
+     5          80 LOAD_CONST               3 (<code object test_swedish_national_mathematics_2, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 5>)
                 82 MAKE_FUNCTION            0
                 84 STORE_NAME              16 (test_swedish_national_mathematics_2)
    
-    10          86 LOAD_CONST               4 (<code object test_swedish_national_mathematics_1, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 10>)
+    10          86 LOAD_CONST               4 (<code object test_swedish_national_mathematics_1, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 10>)
                 88 MAKE_FUNCTION            0
                 90 STORE_NAME              17 (test_swedish_national_mathematics_1)
    
-    15          92 LOAD_CONST               5 (<code object test_swedish_sat_verbal, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 15>)
+    15          92 LOAD_CONST               5 (<code object test_swedish_sat_verbal, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 15>)
                 94 MAKE_FUNCTION            0
                 96 STORE_NAME              18 (test_swedish_sat_verbal)
    
-    22          98 LOAD_CONST               6 (<code object test_swedish_sat_quantitative, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 22>)
+    22          98 LOAD_CONST               6 (<code object test_swedish_sat_quantitative, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 22>)
                100 MAKE_FUNCTION            0
                102 STORE_NAME              19 (test_swedish_sat_quantitative)
    
-    29         104 LOAD_CONST               7 (<code object test_swedish_sat, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 29>)
+    29         104 LOAD_CONST               7 (<code object test_swedish_sat, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 29>)
                106 MAKE_FUNCTION            0
                108 STORE_NAME              20 (test_swedish_sat)
    
-    36         110 LOAD_CONST               8 (<code object test_swedish_sat_binary, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 36>)
+    36         110 LOAD_CONST               8 (<code object test_swedish_sat_binary, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 36>)
                112 MAKE_FUNCTION            0
                114 STORE_NAME              21 (test_swedish_sat_binary)
    
-    43         116 LOAD_CONST               9 (<code object test_big_five, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 43>)
+    43         116 LOAD_CONST               9 (<code object test_big_five, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 43>)
                118 MAKE_FUNCTION            0
                120 STORE_NAME              22 (test_big_five)
                122 LOAD_CONST               1 (None)
                124 RETURN_VALUE
    consts
       0
       None
@@ -327,15 +327,15 @@
             ('py0', 'py2', 'py5')
             'assert %(py7)s'
             'py7'
          names      ('swedish_national_mathematics_2', 'dtype', 'torch', 'float32', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape')
          varnames   ('data', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
          name       'test_swedish_national_mathematics_2'
          firstlineno 5
          lnotab 0x02011c01ff00ff002801
       code
          argcount  : 0
          nlocals   : 9
          stacksize : 7
@@ -573,15 +573,15 @@
             ('py0', 'py2', 'py5')
             'assert %(py7)s'
             'py7'
          names      ('swedish_national_mathematics_1', 'dtype', 'torch', 'float32', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape')
          varnames   ('data', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
          name       'test_swedish_national_mathematics_1'
          firstlineno 10
          lnotab 0x02011c01ff00ff002801
       code
          argcount  : 0
          nlocals   : 12
          stacksize : 7
@@ -932,15 +932,15 @@
                  >> 1506 LOAD_CONST               0 (None)
                     1508 COPY                     1
                     1510 STORE_FAST              10 (@py_assert2)
                     1512 COPY                     1
                     1514 STORE_FAST               7 (@py_assert4)
                     1516 STORE_FAST               3 (@py_assert5)
          
-          20        1518 LOAD_CONST              18 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 20>)
+          20        1518 LOAD_CONST              18 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 20>)
                     1520 MAKE_FUNCTION            0
                     1522 LOAD_FAST                1 (correct_category)
                     1524 GET_ITER
                     1526 PRECALL                  0
                     1530 CALL                     0
                     1540 STORE_FAST               2 (@py_assert1)
                     1542 LOAD_GLOBAL             29 (NULL + all)
@@ -1041,26 +1041,26 @@
                             52 JUMP_BACKWARD           24 (to 6)
                        >>   54 RETURN_VALUE
                consts
                names      ('isinstance', 'int')
                varnames   ('.0', 'x')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
                name       '<listcomp>'
                firstlineno 20
                lnotab 0x
             'assert %(py4)s\n{%(py4)s = %(py0)s(%(py2)s)\n}'
             'all'
             ('py0', 'py2', 'py4')
          names      ('swedish_sat_verbal', 'dtype', 'torch', 'float32', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape', 'len', 'all')
          varnames   ('data', 'correct_category', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_format6', '@py_format8', '@py_assert2', '@py_format5')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
          name       'test_swedish_sat_verbal'
          firstlineno 15
          lnotab 0x02012201ff00ff002801ff008301ff00ff002401
       code
          argcount  : 0
          nlocals   : 12
          stacksize : 7
@@ -1411,15 +1411,15 @@
                  >> 1506 LOAD_CONST               0 (None)
                     1508 COPY                     1
                     1510 STORE_FAST              10 (@py_assert2)
                     1512 COPY                     1
                     1514 STORE_FAST               7 (@py_assert4)
                     1516 STORE_FAST               3 (@py_assert5)
          
-          27        1518 LOAD_CONST              18 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 27>)
+          27        1518 LOAD_CONST              18 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 27>)
                     1520 MAKE_FUNCTION            0
                     1522 LOAD_FAST                1 (correct_category)
                     1524 GET_ITER
                     1526 PRECALL                  0
                     1530 CALL                     0
                     1540 STORE_FAST               2 (@py_assert1)
                     1542 LOAD_GLOBAL             29 (NULL + all)
@@ -1520,26 +1520,26 @@
                             52 JUMP_BACKWARD           24 (to 6)
                        >>   54 RETURN_VALUE
                consts
                names      ('isinstance', 'int')
                varnames   ('.0', 'x')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
                name       '<listcomp>'
                firstlineno 27
                lnotab 0x
             'assert %(py4)s\n{%(py4)s = %(py0)s(%(py2)s)\n}'
             'all'
             ('py0', 'py2', 'py4')
          names      ('swedish_sat_quantitative', 'dtype', 'torch', 'float32', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape', 'len', 'all')
          varnames   ('data', 'correct_category', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_format6', '@py_format8', '@py_assert2', '@py_format5')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
          name       'test_swedish_sat_quantitative'
          firstlineno 22
          lnotab 0x02012201ff00ff002801ff008301ff00ff002401
       code
          argcount  : 0
          nlocals   : 12
          stacksize : 7
@@ -1890,15 +1890,15 @@
                  >> 1506 LOAD_CONST               0 (None)
                     1508 COPY                     1
                     1510 STORE_FAST              10 (@py_assert2)
                     1512 COPY                     1
                     1514 STORE_FAST               7 (@py_assert4)
                     1516 STORE_FAST               3 (@py_assert5)
          
-          34        1518 LOAD_CONST              18 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_load_dataset.py", line 34>)
+          34        1518 LOAD_CONST              18 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_load_dataset.py", line 34>)
                     1520 MAKE_FUNCTION            0
                     1522 LOAD_FAST                1 (correct_category)
                     1524 GET_ITER
                     1526 PRECALL                  0
                     1530 CALL                     0
                     1540 STORE_FAST               2 (@py_assert1)
                     1542 LOAD_GLOBAL             29 (NULL + all)
@@ -1999,26 +1999,26 @@
                             52 JUMP_BACKWARD           24 (to 6)
                        >>   54 RETURN_VALUE
                consts
                names      ('isinstance', 'int')
                varnames   ('.0', 'x')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
                name       '<listcomp>'
                firstlineno 34
                lnotab 0x
             'assert %(py4)s\n{%(py4)s = %(py0)s(%(py2)s)\n}'
             'all'
             ('py0', 'py2', 'py4')
          names      ('swedish_sat', 'dtype', 'torch', 'float32', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape', 'len', 'all')
          varnames   ('data', 'correct_category', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_format6', '@py_format8', '@py_assert2', '@py_format5')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
          name       'test_swedish_sat'
          firstlineno 29
          lnotab 0x02012201ff00ff002801ff008301ff00ff002401
       code
          argcount  : 0
          nlocals   : 14
          stacksize : 7
@@ -2461,15 +2461,15 @@
             'py10'
             0.0
             ('%(py5)s\n{%(py5)s = %(py3)s\n{%(py3)s = %(py1)s.min\n}()\n} == %(py8)s',)
          names      ('swedish_sat_binary', 'dtype', 'torch', 'float32', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape', 'isnan', 'max', 'min')
          varnames   ('data', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_format6', '@py_format8', '@py_assert0', '@py_assert2', '@py_assert7', '@py_assert6', '@py_format11')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
          name       'test_swedish_sat_binary'
          firstlineno 36
          lnotab 0x02011c01ff00ff002801ff008301ff00a501
       code
          argcount  : 0
          nlocals   : 14
          stacksize : 7
@@ -2912,19 +2912,19 @@
             'py10'
             0.0
             ('%(py5)s\n{%(py5)s = %(py3)s\n{%(py3)s = %(py1)s.min\n}()\n} == %(py8)s',)
          names      ('big_five', 'dtype', 'torch', 'float32', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape', 'isnan', 'max', 'min')
          varnames   ('data', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_format6', '@py_format8', '@py_assert0', '@py_assert2', '@py_assert7', '@py_assert6', '@py_format11')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
          name       'test_big_five'
          firstlineno 43
          lnotab 0x02011c01ff00ff002801ff008301ff00a501
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'irtorch.load_dataset', 'swedish_national_mathematics_2', 'swedish_national_mathematics_1', 'swedish_sat_verbal', 'swedish_sat_quantitative', 'swedish_sat', 'swedish_sat_binary', 'big_five', 'test_swedish_national_mathematics_2', 'test_swedish_national_mathematics_1', 'test_swedish_sat_verbal', 'test_swedish_sat_quantitative', 'test_swedish_sat', 'test_swedish_sat_binary', 'test_big_five')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_load_dataset.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_load_dataset.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201220108012402060506050607060706070607
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_monotone_nn.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_monotone_nn.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -44,37 +44,37 @@
      3          44 LOAD_CONST               0 (0)
                 46 LOAD_CONST               2 (('MonotoneNN',))
                 48 IMPORT_NAME              8 (irtorch.models)
                 50 IMPORT_FROM              9 (MonotoneNN)
                 52 STORE_NAME               9 (MonotoneNN)
                 54 POP_TOP
    
-     5          56 LOAD_CONST               3 (<code object test_mc_correct_output_idx, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 5>)
+     5          56 LOAD_CONST               3 (<code object test_mc_correct_output_idx, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 5>)
                 58 MAKE_FUNCTION            0
                 60 STORE_NAME              10 (test_mc_correct_output_idx)
    
-    29          62 LOAD_CONST               4 (<code object test_log_likelihood, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 29>)
+    29          62 LOAD_CONST               4 (<code object test_log_likelihood, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 29>)
                 64 MAKE_FUNCTION            0
                 66 STORE_NAME              11 (test_log_likelihood)
    
-    51          68 LOAD_CONST               5 (<code object test_split_activation, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 51>)
+    51          68 LOAD_CONST               5 (<code object test_split_activation, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 51>)
                 70 MAKE_FUNCTION            0
                 72 STORE_NAME              12 (test_split_activation)
    
     76          74 LOAD_NAME                6 (pytest)
                 76 LOAD_ATTR               13 (mark)
                 86 LOAD_METHOD             14 (parametrize)
                108 LOAD_CONST               6 ('separate')
                110 LOAD_CONST               7 ('items')
                112 LOAD_CONST               8 ('categories')
                114 BUILD_LIST               2
                116 PRECALL                  2
                120 CALL                     2
    
-    77         130 LOAD_CONST               9 (<code object test_forward_ordered, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 76>)
+    77         130 LOAD_CONST               9 (<code object test_forward_ordered, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 76>)
                132 MAKE_FUNCTION            0
    
     76         134 PRECALL                  0
                138 CALL                     0
    
     77         148 STORE_NAME              15 (test_forward_ordered)
    
@@ -84,27 +84,27 @@
                184 LOAD_CONST               6 ('separate')
                186 LOAD_CONST               7 ('items')
                188 LOAD_CONST               8 ('categories')
                190 BUILD_LIST               2
                192 PRECALL                  2
                196 CALL                     2
    
-   112         206 LOAD_CONST              10 (<code object test_forward_mc, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 111>)
+   112         206 LOAD_CONST              10 (<code object test_forward_mc, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 111>)
                208 MAKE_FUNCTION            0
    
    111         210 PRECALL                  0
                214 CALL                     0
    
    112         224 STORE_NAME              16 (test_forward_mc)
    
-   146         226 LOAD_CONST              11 (<code object test_probabilities_from_output, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 146>)
+   146         226 LOAD_CONST              11 (<code object test_probabilities_from_output, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 146>)
                228 MAKE_FUNCTION            0
                230 STORE_NAME              17 (test_probabilities_from_output)
    
-   175         232 LOAD_CONST              12 (<code object test_item_z_relationship_directions, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 175>)
+   175         232 LOAD_CONST              12 (<code object test_item_z_relationship_directions, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 175>)
                234 MAKE_FUNCTION            0
                236 STORE_NAME              18 (test_item_z_relationship_directions)
                238 LOAD_CONST               1 (None)
                240 RETURN_VALUE
    consts
       0
       None
@@ -536,15 +536,15 @@
             ('py0', 'py2', 'py3', 'py5', 'py6', 'py8', 'py10', 'py12', 'py14')
             False
             (False, True, False, False, True, False, False, False)
          names      ('MonotoneNN', 'torch', 'equal', 'mc_correct_output_idx', 'tensor', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('model', '@py_assert1', '@py_assert4', '@py_assert7', '@py_assert9', '@py_assert11', '@py_assert13', '@py_format15')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
          name       'test_mc_correct_output_idx'
          firstlineno 5
          lnotab
             0x02010c010201040106010201060102fa1209ff00ff00ff0063020c0102
             01040106010201060102fa1209
       code
          argcount  : 0
@@ -1507,15 +1507,15 @@
             'incorrect item likelihood'
             '\n>assert %(py14)s\n{%(py14)s = %(py2)s\n{%(py2)s = %(py0)s.isclose\n}(%(py4)s, %(py12)s\n{%(py12)s = %(py7)s\n{%(py7)s = %(py5)s.tensor\n}(-%(py9)s)\n})\n}'
             ('py0', 'py2', 'py4', 'py5', 'py7', 'py9', 'py12', 'py14')
          names      ('MonotoneNN', 'torch', 'tensor', 'float', 'inf', 'log_likelihood', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'isclose', 'sum', 'equal', 'append', '_format_boolop')
          varnames   ('model', 'data', 'output', 'result', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert9', '@py_assert11', '@py_assert13', '@py_assert14', '@py_assert16', '@py_format18', '@py_assert5', '@py_assert7', '@py_assert0', '@py_assert15', '@py_assert17', '@py_assert19', '@py_format11', '@py_format21', '@py_format22', '@py_format24', '@py_format9', '@py_assert8', '@py_assert10', '@py_format15')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
          name       'test_log_likelihood'
          firstlineno 29
          lnotab
             0x02010c0102010401060102fc12075e0116012801280128fd12053001ff
             00ad01ff00ff00ff00d101ff00ff00ff00ff004c01ff00ff000601
       code
          argcount  : 0
@@ -2576,15 +2576,15 @@
             'output_tensor_false'
             'Output shape is incorrect with use_bounded_activation=False'
             (1.0, 0.6321, 1.0, -1.0, -0.6321, -1.0)
          names      ('MonotoneNN', 'torch', 'cat', 'ones', 'requires_grad_', 'split_activation', 'sum', 'backward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'grad', 'allclose', 'tensor', 'use_bounded_activation')
          varnames   ('model', 'input_tensor', 'output_tensor_true', '@py_assert1', '@py_assert5', '@py_assert3', '@py_format7', '@py_format9', '@py_assert4', '@py_format6', '@py_format8', '@py_assert7', '@py_assert9', '@py_assert11', '@py_assert13', '@py_format15', 'output_tensor_false')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
          name       'test_split_activation'
          firstlineno 51
          lnotab
             0x02012c02a2012a014c01ff00ff003401ff00a9010c030afd0e030afd5a
             030afd24030afd1e030afd28030afd2a030afd1e030afd1e030afd1e030a
             fd22030afd1e030afd28030afd2a030afd1c030afd1c030afd1c030afd1c
             030afd32030afd3806a2010e012a014c01ff00ff003401ff00a9010c030a
@@ -2710,15 +2710,15 @@
           87         118 LOAD_CONST               8 (True)
          
           79         120 KW_NAMES                 9
                      122 PRECALL                  8
                      126 CALL                     8
                      136 STORE_FAST               2 (model)
          
-          90         138 LOAD_CONST              10 (<code object <dictcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 90>)
+          90         138 LOAD_CONST              10 (<code object <dictcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 90>)
                      140 MAKE_FUNCTION            0
                      142 LOAD_FAST                2 (model)
                      144 LOAD_METHOD              4 (named_parameters)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 GET_ITER
                      182 PRECALL                  0
@@ -3104,15 +3104,15 @@
                             58 JUMP_BACKWARD           27 (to 6)
                        >>   60 RETURN_VALUE
                consts
                names      ('clone',)
                varnames   ('.0', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
                name       '<dictcomp>'
                firstlineno 90
                lnotab 0x
             'params'
             0.02
             ('lr', 'amsgrad')
             0.1
@@ -3145,15 +3145,15 @@
             '\n>assert %(py9)s\n{%(py9)s = %(py2)s\n{%(py2)s = %(py0)s.all\n}(%(py7)s)\n}'
             'torch'
             ('py0', 'py2', 'py7', 'py9')
          names      ('MonotoneNN', 'torch', 'tensor', 'bool', 'named_parameters', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'log_likelihood', 'backward', 'step', 'all')
          varnames   ('separate', 'hidden_dim', 'model', 'original_parameter_dictionary', 'optimizer', 'z', 'data', '_', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'loss', 'name', 'param', 'original_parameters', '@py_assert8', '@py_format10')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
          name       'test_forward_ordered'
          firstlineno 76
          lnotab
             0x020208010c01020106010201020102015001020102f8120b3c022c0130
             ff120340016401240128012a01ff00ad02300128012c0334011001ff00ff
             00e4fe
       code
@@ -3272,15 +3272,15 @@
          121         120 LOAD_CONST               9 (True)
          
          114         122 KW_NAMES                10
                      124 PRECALL                  7
                      128 CALL                     7
                      138 STORE_FAST               2 (model)
          
-         124         140 LOAD_CONST              11 (<code object <dictcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_monotone_nn.py", line 124>)
+         124         140 LOAD_CONST              11 (<code object <dictcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_monotone_nn.py", line 124>)
                      142 MAKE_FUNCTION            0
                      144 LOAD_FAST                2 (model)
                      146 LOAD_METHOD              4 (named_parameters)
                      168 PRECALL                  0
                      172 CALL                     0
                      182 GET_ITER
                      184 PRECALL                  0
@@ -3667,15 +3667,15 @@
                             58 JUMP_BACKWARD           27 (to 6)
                        >>   60 RETURN_VALUE
                consts
                names      ('clone',)
                varnames   ('.0', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
                name       '<dictcomp>'
                firstlineno 124
                lnotab 0x
             'params'
             0.02
             ('lr', 'amsgrad')
             0.1
@@ -3708,15 +3708,15 @@
             '\n>assert %(py9)s\n{%(py9)s = %(py2)s\n{%(py2)s = %(py0)s.all\n}(%(py7)s)\n}'
             'torch'
             ('py0', 'py2', 'py7', 'py9')
          names      ('MonotoneNN', 'torch', 'tensor', 'bool', 'named_parameters', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'log_likelihood', 'backward', 'step', 'all')
          varnames   ('separate', 'hidden_dim', 'model', 'original_parameter_dictionary', 'optimizer', 'z', 'data', '_', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'loss', 'name', 'param', 'original_parameters', '@py_assert8', '@py_format10')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
          name       'test_forward_mc'
          firstlineno 111
          lnotab
             0x020208010c0102010601020106010201500102f9120a3c022c0130ff12
             0340016401240128012a01ff00ad02300128012c0334011001ff00ff00e4
             fe
       code
@@ -4645,15 +4645,15 @@
             ('dim',)
             '\n>assert %(py20)s\n{%(py20)s = %(py2)s\n{%(py2)s = %(py0)s.allclose\n}(%(py9)s\n{%(py9)s = %(py5)s\n{%(py5)s = %(py3)s.sum\n}(dim=%(py7)s)\n}, %(py18)s\n{%(py18)s = %(py12)s\n{%(py12)s = %(py10)s.ones\n}(%(py14)s, %(py16)s)\n})\n}'
             ('py0', 'py2', 'py3', 'py5', 'py7', 'py9', 'py10', 'py12', 'py14', 'py16', 'py18', 'py20')
          names      ('MonotoneNN', 'torch', 'tensor', 'bool', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'log_likelihood', 'backward', 'step', 'probabilities_from_output', 'all', 'allclose', 'sum', 'ones')
          varnames   ('model', 'optimizer', 'z', 'data', '_', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'loss', 'probabilities', '@py_assert6', '@py_assert5', '@py_assert10', '@py_format12', '@py_assert8', '@py_assert11', '@py_assert13', '@py_assert15', '@py_assert17', '@py_assert19', '@py_format21')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
          name       'test_probabilities_from_output'
          firstlineno 146
          lnotab
             0x02010c01020106010401500102fb12082c0130ff120340016401240128
             012a01ff00ad02300128012c023c01ff00ad01ff00ff005401ff00ff0054
             01
       code
@@ -5411,24 +5411,24 @@
             'py6'
             (2, 1)
             'item_z_relationship_directions should be 0 the third and second latent variable'
          names      ('torch', 'manual_seed', 'MonotoneNN', 'tensor', 'bool', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'log_likelihood', 'backward', 'step', 'item_z_relationship_directions', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'all')
          varnames   ('model', 'optimizer', 'z', 'data', '_', 'output', 'loss', 'item_z_relationship_directions', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert5', '@py_assert10', '@py_format12', '@py_assert8', '@py_assert11', '@py_format9', '@py_format13', '@py_assert0', '@py_assert2', '@py_format5', '@py_format7')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
          name       'test_item_z_relationship_directions'
          firstlineno 175
          lnotab
             0x020128010c01020106010401500102fb12082c0130ff12034001640122
             0128012a01300128012a022801ff00ad01ff00ff004e01ff00ff005801ff
             003301
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'irtorch.models', 'MonotoneNN', 'test_mc_correct_output_idx', 'test_log_likelihood', 'test_split_activation', 'mark', 'parametrize', 'test_forward_ordered', 'test_forward_mc', 'test_probabilities_from_output', 'test_item_z_relationship_directions')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_monotone_nn.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_monotone_nn.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201220108010c02061806160619380104ff0e010222380104ff0e
       010222061d
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_outlier_detector.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_outlier_detector.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -38,23 +38,23 @@
      3          44 LOAD_CONST               0 (0)
                 46 LOAD_CONST               2 (('OutlierDetector',))
                 48 IMPORT_NAME              8 (irtorch.outlier_detector)
                 50 IMPORT_FROM              9 (OutlierDetector)
                 52 STORE_NAME               9 (OutlierDetector)
                 54 POP_TOP
    
-     5          56 LOAD_CONST               3 (<code object test_identify_outliers, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_outlier_detector.py", line 5>)
+     5          56 LOAD_CONST               3 (<code object test_identify_outliers, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_outlier_detector.py", line 5>)
                 58 MAKE_FUNCTION            0
                 60 STORE_NAME              10 (test_identify_outliers)
    
-    30          62 LOAD_CONST               4 (<code object test_is_outlier, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_outlier_detector.py", line 30>)
+    30          62 LOAD_CONST               4 (<code object test_is_outlier, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_outlier_detector.py", line 30>)
                 64 MAKE_FUNCTION            0
                 66 STORE_NAME              11 (test_is_outlier)
    
-    51          68 LOAD_CONST               5 (<code object test_smallest_largest_non_outlier, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_outlier_detector.py", line 51>)
+    51          68 LOAD_CONST               5 (<code object test_smallest_largest_non_outlier, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_outlier_detector.py", line 51>)
                 70 MAKE_FUNCTION            0
                 72 STORE_NAME              12 (test_smallest_largest_non_outlier)
                 74 LOAD_CONST               1 (None)
                 76 RETURN_VALUE
    consts
       0
       None
@@ -698,15 +698,15 @@
             'outliers_lower'
             'expected_outliers_lower'
             5
          names      ('OutlierDetector', 'torch', 'tensor', 'identify_outliers', 'equal', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'pytest', 'raises', 'ValueError', 'rand')
          varnames   ('detector', 'data', 'expected_outliers_all', 'expected_outliers_upper', 'expected_outliers_lower', 'outliers_all', '@py_assert1', '@py_assert5', '@py_format7', 'outliers_upper', 'outliers_lower')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_outlier_detector.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_outlier_detector.py'
          name       'test_identify_outliers'
          firstlineno 5
          lnotab
             0x02011c014c034c014c014c022a01ff00ff0062023001ff00ff00620230
             01ff00ff00620234014eff2e03340130ff
       code
          argcount  : 0
@@ -1147,15 +1147,15 @@
             5
             (2.5, 1.0, 0.5)
             ('upper', 'lower')
          names      ('OutlierDetector', 'torch', 'tensor', 'is_outlier', 'equal', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'pytest', 'raises', 'ValueError', 'rand')
          varnames   ('detector', 'data', 'new_observation', 'result', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_format13')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_outlier_detector.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_outlier_detector.py'
          name       'test_is_outlier'
          firstlineno 30
          lnotab
             0x02011c0140012e022c01ff00ff00ff002d02340152ff2e03340150ff2e
             03340156ff2e03340132ff
       code
          argcount  : 0
@@ -1616,21 +1616,21 @@
             False
             ('smallest',)
             5
          names      ('OutlierDetector', 'torch', 'tensor', 'smallest_largest_non_outlier', 'equal', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'pytest', 'raises', 'ValueError', 'rand')
          varnames   ('detector', 'data', 'result', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_format13')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_outlier_detector.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_outlier_detector.py'
          name       'test_smallest_largest_non_outlier'
          firstlineno 51
          lnotab
             0x02011c0152022a01ff00ff00ff002d022e01ff00ff00ff002d0234014e
             ff
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'irtorch.outlier_detector', 'OutlierDetector', 'test_identify_outliers', 'test_is_outlier', 'test_smallest_largest_non_outlier')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_outlier_detector.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_outlier_detector.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201220108010c0206190615
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_parametric.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_parametric.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -44,39 +44,39 @@
      4          52 LOAD_CONST               0 (0)
                 54 LOAD_CONST               2 (('Parametric',))
                 56 IMPORT_NAME             10 (irtorch.models)
                 58 IMPORT_FROM             11 (Parametric)
                 60 STORE_NAME              11 (Parametric)
                 62 POP_TOP
    
-     6          64 LOAD_CONST               3 (<code object test_1pl_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_parametric.py", line 6>)
+     6          64 LOAD_CONST               3 (<code object test_1pl_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_parametric.py", line 6>)
                 66 MAKE_FUNCTION            0
                 68 STORE_NAME              12 (test_1pl_forward)
    
-    35          70 LOAD_CONST               4 (<code object test_2pl_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_parametric.py", line 35>)
+    35          70 LOAD_CONST               4 (<code object test_2pl_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_parametric.py", line 35>)
                 72 MAKE_FUNCTION            0
                 74 STORE_NAME              13 (test_2pl_forward)
    
-    63          76 LOAD_CONST               5 (<code object test_gpc_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_parametric.py", line 63>)
+    63          76 LOAD_CONST               5 (<code object test_gpc_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_parametric.py", line 63>)
                 78 MAKE_FUNCTION            0
                 80 STORE_NAME              14 (test_gpc_forward)
    
-    91          82 LOAD_CONST               6 (<code object test_nominal_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_parametric.py", line 91>)
+    91          82 LOAD_CONST               6 (<code object test_nominal_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_parametric.py", line 91>)
                 84 MAKE_FUNCTION            0
                 86 STORE_NAME              15 (test_nominal_forward)
    
-   154          88 LOAD_CONST               7 (<code object test_probabilities_from_output, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_parametric.py", line 154>)
+   154          88 LOAD_CONST               7 (<code object test_probabilities_from_output, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_parametric.py", line 154>)
                 90 MAKE_FUNCTION            0
                 92 STORE_NAME              16 (test_probabilities_from_output)
    
-   183          94 LOAD_CONST               8 (<code object test_item_parameters, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_parametric.py", line 183>)
+   183          94 LOAD_CONST               8 (<code object test_item_parameters, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_parametric.py", line 183>)
                 96 MAKE_FUNCTION            0
                 98 STORE_NAME              17 (test_item_parameters)
    
-   213         100 LOAD_CONST               9 (<code object test_item_z_relationship_directions, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_parametric.py", line 213>)
+   213         100 LOAD_CONST               9 (<code object test_item_z_relationship_directions, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_parametric.py", line 213>)
                102 MAKE_FUNCTION            0
                104 STORE_NAME              18 (test_item_z_relationship_directions)
                106 LOAD_CONST               1 (None)
                108 RETURN_VALUE
    consts
       0
       None
@@ -734,15 +734,15 @@
             ('%(py3)s != %(py7)s\n{%(py7)s = %(py5)s.bias_param\n}',)
             'original_bias'
             'Free bias should have changed'
          names      ('Parametric', 'torch', 'tensor', 'weight_param', 'clone', 'bias_param', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'log_likelihood', 'backward', 'step', 'all')
          varnames   ('model', 'original_weights', 'original_bias', 'optimizer', 'z', 'data', '_', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'loss', '@py_assert6', '@py_assert10', '@py_format12')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_parametric.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_parametric.py'
          name       'test_1pl_forward'
          firstlineno 6
          lnotab
             0x02010c0102010601020138fc1206320132022c0130ff12034001640124
             0128012a01ff00ad02300228012c02ff00ff00ff001101
       code
          argcount  : 0
@@ -1397,15 +1397,15 @@
             ('%(py3)s != %(py7)s\n{%(py7)s = %(py5)s.bias_param\n}',)
             'original_bias'
             'Free bias should have changed'
          names      ('Parametric', 'torch', 'tensor', 'weight_param', 'clone', 'bias_param', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'log_likelihood', 'backward', 'step', 'all')
          varnames   ('model', 'original_weights', 'original_bias', 'optimizer', 'z', 'data', '_', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'loss', '@py_assert6', '@py_assert10', '@py_format12')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_parametric.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_parametric.py'
          name       'test_2pl_forward'
          firstlineno 35
          lnotab
             0x02010c0102010201060138fc1206320132022c0130ff12034001640124
             0128012a01ff00ad02300228012c02ff00ff00ff001101
       code
          argcount  : 0
@@ -2062,15 +2062,15 @@
             ('%(py3)s != %(py7)s\n{%(py7)s = %(py5)s.bias_param\n}',)
             'original_bias'
             'Free bias should have changed'
          names      ('Parametric', 'torch', 'tensor', 'weight_param', 'clone', 'bias_param', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'log_likelihood', 'backward', 'step', 'all')
          varnames   ('model', 'original_weights', 'original_bias', 'optimizer', 'z', 'data', '_', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'loss', '@py_assert6', '@py_assert10', '@py_format12')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_parametric.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_parametric.py'
          name       'test_gpc_forward'
          firstlineno 63
          lnotab
             0x02010c0102010201060138fc1206320132022c0130ff12034001640124
             0128012a01ff00ad02300228012c02ff00ff00ff001101
       code
          argcount  : 0
@@ -4000,15 +4000,15 @@
             'original_bias'
             'Free bias should have changed'
             13
          names      ('Parametric', 'torch', 'tensor', 'weight_param', 'clone', 'bias_param', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'log_likelihood', 'backward', 'step', 'Size', 'all')
          varnames   ('model', 'original_weights', 'original_bias', 'optimizer', 'z', 'data', '_', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'loss', '@py_assert7', '@py_assert9', '@py_assert11', '@py_assert5', '@py_format13', '@py_format15', '@py_assert6', '@py_assert10', '@py_format12')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_parametric.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_parametric.py'
          name       'test_nominal_forward'
          firstlineno 91
          lnotab
             0x02020c01020102010601380102fb1207320132022c0130ff1203400164
             01240128012a01ff00ad02300228012c02ff00ff00fc01ff00ff00fc01ff
             00ff00ff001101ff00ff00ff0011030c01020102010601380102fb120732
             0132022c0130ff120340016401240128012a01ff00ad02300228012c02ff
@@ -4932,15 +4932,15 @@
             ('dim',)
             '\n>assert %(py20)s\n{%(py20)s = %(py2)s\n{%(py2)s = %(py0)s.allclose\n}(%(py9)s\n{%(py9)s = %(py5)s\n{%(py5)s = %(py3)s.sum\n}(dim=%(py7)s)\n}, %(py18)s\n{%(py18)s = %(py12)s\n{%(py12)s = %(py10)s.ones\n}(%(py14)s, %(py16)s)\n})\n}'
             ('py0', 'py2', 'py3', 'py5', 'py7', 'py9', 'py10', 'py12', 'py14', 'py16', 'py18', 'py20')
          names      ('Parametric', 'torch', 'tensor', 'optim', 'Adam', 'parameters', 'float', 'range', 'zero_grad', 'forward', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'log_likelihood', 'backward', 'step', 'probabilities_from_output', 'all', 'allclose', 'sum', 'ones')
          varnames   ('model', 'optimizer', 'z', 'data', '_', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', 'loss', 'probabilities', '@py_assert6', '@py_assert5', '@py_assert10', '@py_format12', '@py_assert8', '@py_assert11', '@py_assert13', '@py_assert15', '@py_assert17', '@py_assert19', '@py_format21')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_parametric.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_parametric.py'
          name       'test_probabilities_from_output'
          firstlineno 154
          lnotab
             0x02010c0102010201060138fc12072c0130ff120340016401240128012a
             01ff00ad02300228012c023c01ff00ad01ff00ff005401ff00ff005401
       code
          argcount  : 1
@@ -5909,15 +5909,15 @@
             '\n>assert %(py7)s'
             'py7'
             'parameters_irt'
          names      ('Parametric', 'torch', 'tensor', 'repeat', 'item_parameters', 'pd', 'DataFrame', 'isinstance', '@pytest_ar', '_format_assertmsg', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape', 'items', 'latent_variables', 'max_item_responses', '_call_reprcompare')
          varnames   ('latent_variables', 'model_type', 'item_categories', 'model', 'parameters', '@py_assert3', '@py_assert5', '@py_format7', '@py_assert1', '@py_assert4', '@py_format6', '@py_format8', 'parameters_irt')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_parametric.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_parametric.py'
          name       'test_item_parameters'
          firstlineno 183
          lnotab
             0x02010a0108010a0208010c010201020102015afc12062c02ff00ff00b0
             010c01ff00e502ff00dd022c02ff00ff00b0010c01ff00e7011601ff00e7
             02ff00e1e5
       code
@@ -6535,21 +6535,21 @@
             '\n>assert %(py6)s'
             'py6'
             (2, 1)
          names      ('Parametric', 'torch', 'tensor', 'weight_param', 'data', 'item_z_relationship_directions', 'shape', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', '_format_assertmsg', 'AssertionError', '_format_explanation', 'all')
          varnames   ('model', 'directions', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8', '@py_assert6', '@py_assert5', '@py_assert10', '@py_format12', '@py_assert8', '@py_assert11', '@py_format9', '@py_format13', '@py_assert0', '@py_assert2', '@py_format5', '@py_format7')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_parametric.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_parametric.py'
          name       'test_item_z_relationship_directions'
          firstlineno 213
          lnotab
             0x02010c0102010201060138fc120640022801ff00ad01ff00ff004e01ff
             00ff005801ff003301
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'pandas', 'pd', 'irtorch.models', 'Parametric', 'test_1pl_forward', 'test_2pl_forward', 'test_gpc_forward', 'test_nominal_forward', 'test_probabilities_from_output', 'test_item_parameters', 'test_item_z_relationship_directions')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_parametric.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_parametric.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02012201080108010c02061d061c061c063f061d061e
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_quantile_mv_normal.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_quantile_mv_normal.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -46,23 +46,23 @@
      4          56 LOAD_CONST               0 (0)
                 58 LOAD_CONST               3 (('QuantileMVNormal',))
                 60 IMPORT_NAME             10 (irtorch.quantile_mv_normal)
                 62 IMPORT_FROM             11 (QuantileMVNormal)
                 64 STORE_NAME              11 (QuantileMVNormal)
                 66 POP_TOP
    
-     7          68 LOAD_CONST               4 (<code object test_fit, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_quantile_mv_normal.py", line 7>)
+     7          68 LOAD_CONST               4 (<code object test_fit, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_quantile_mv_normal.py", line 7>)
                 70 MAKE_FUNCTION            0
                 72 STORE_NAME              12 (test_fit)
    
-    18          74 LOAD_CONST               5 (<code object test_fit_multivariate_normal, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_quantile_mv_normal.py", line 18>)
+    18          74 LOAD_CONST               5 (<code object test_fit_multivariate_normal, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_quantile_mv_normal.py", line 18>)
                 76 MAKE_FUNCTION            0
                 78 STORE_NAME              13 (test_fit_multivariate_normal)
    
-    41          80 LOAD_CONST               6 (<code object test_pdf, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_quantile_mv_normal.py", line 41>)
+    41          80 LOAD_CONST               6 (<code object test_pdf, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_quantile_mv_normal.py", line 41>)
                 82 MAKE_FUNCTION            0
                 84 STORE_NAME              14 (test_pdf)
                 86 LOAD_CONST               1 (None)
                 88 RETURN_VALUE
    consts
       0
       None
@@ -575,15 +575,15 @@
             'assert %(py14)s'
             'py14'
             ('%(py4)s\n{%(py4)s = %(py2)s\n{%(py2)s = %(py0)s.mvnormal\n}.event_shape\n} == %(py12)s\n{%(py12)s = %(py8)s\n{%(py8)s = %(py6)s.Size\n}(%(py10)s)\n}',)
          names      ('torch', 'randn', 'QuantileMVNormal', 'fit', 'mvnormal', 'distributions', 'MultivariateNormal', 'isinstance', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'batch_shape', 'Size', '_call_reprcompare', 'event_shape')
          varnames   ('data', 'qmvn', '@py_assert2', '@py_assert5', '@py_assert7', '@py_assert9', '@py_format11', '@py_assert1', '@py_assert3', '@py_assert11', '@py_format13', '@py_format15')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_quantile_mv_normal.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_quantile_mv_normal.py'
          name       'test_fit'
          firstlineno 7
          lnotab 0x02012a021c012a02ff00ff00ee01ff00ff00d001
       code
          argcount  : 0
          nlocals   : 14
          stacksize : 9
@@ -1103,15 +1103,15 @@
             ('py0', 'py2', 'py3', 'py5', 'py6', 'py8')
             'assert %(py8)s\n{%(py8)s = %(py2)s\n{%(py2)s = %(py0)s.allclose\n}(%(py5)s\n{%(py5)s = %(py3)s.covariance_matrix\n}, %(py6)s)\n}'
             'cov'
          names      ('torch', 'tensor', 'linalg', 'cholesky', 'mm', 't', 'MultivariateNormal', 'sample', 'QuantileMVNormal', 'fit_multivariate_normal', 'isinstance', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'mean', 'shape', 'allclose', 'covariance_matrix')
          varnames   ('symmetric_matrix', 'cho_dec', 'cov', 'data_dist', 'data_tensor', 'mv_norm', '@py_assert3', '@py_format5', 'mean', 'data_centered', '@py_assert1', '@py_assert4', '@py_assert7', '@py_format9')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_quantile_mv_normal.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_quantile_mv_normal.py'
          name       'test_fit_multivariate_normal'
          firstlineno 18
          lnotab
             0x02023a023e024e0148012a014202ff00ff0046032c010a017003ff00ff
             009a01
       code
          argcount  : 0
@@ -2085,15 +2085,15 @@
             'py26'
             2.9
             3.9
          names      ('torch', 'tensor', 'linalg', 'cholesky', 'mm', 't', 'MultivariateNormal', 'QuantileMVNormal', 'fit', 'mvnormal', 'pdf', 'shape', 'Size', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('symmetric_matrix', 'cho_dec', 'cov', 'data_dist', 'data', 'qmvn', 'pdf', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert3', '@py_format11', '@py_format13', '@py_assert4', '@py_assert6', '@py_assert8', '@py_assert10', '@py_assert14', '@py_assert17', '@py_assert19', '@py_assert21', '@py_assert23', '@py_assert12', '@py_format25', '@py_format27')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_quantile_mv_normal.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_quantile_mv_normal.py'
          name       'test_pdf'
          firstlineno 41
          lnotab
             0x020234023e024e01480240011c012a010e026001ff00ff009a0202020a
             fe0e020afe3a020afe0e020afe56020afe2a020afe1e020afe1e020afe20
             020afe1e020afe1e020afe28020afe2a020afe1c020afe1c020afe1c020a
             fe1e020afe1e020afe1e020afe20020afe1e020afe1e020afe28020afe2a
@@ -2102,11 +2102,11 @@
             fe1e020afe28020afe2a020afe1c020afe1c020afe1c020afe1e020afe1e
             020afe1e020afe20020afe1e020afe1e020afe28020afe2a020afe1c020a
             fe1c020afe1c020afe40020afe
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'torch.distributions.multivariate_normal', 'MultivariateNormal', 'irtorch.quantile_mv_normal', 'QuantileMVNormal', 'test_fit', 'test_fit_multivariate_normal', 'test_pdf')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_quantile_mv_normal.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_quantile_mv_normal.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201220108010c010c03060b0617
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -45,27 +45,27 @@
                 56 STORE_NAME              10 (one_hot_encode_test_data)
                 58 IMPORT_FROM             11 (decode_one_hot_test_data)
                 60 STORE_NAME              11 (decode_one_hot_test_data)
                 62 IMPORT_FROM             12 (split_data)
                 64 STORE_NAME              12 (split_data)
                 66 POP_TOP
    
-     5          68 LOAD_CONST               3 (<code object test_get_item_categories, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_utils.py", line 5>)
+     5          68 LOAD_CONST               3 (<code object test_get_item_categories, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_utils.py", line 5>)
                 70 MAKE_FUNCTION            0
                 72 STORE_NAME              13 (test_get_item_categories)
    
-     9          74 LOAD_CONST               4 (<code object test_one_hot_encode_test_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_utils.py", line 9>)
+     9          74 LOAD_CONST               4 (<code object test_one_hot_encode_test_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_utils.py", line 9>)
                 76 MAKE_FUNCTION            0
                 78 STORE_NAME              14 (test_one_hot_encode_test_data)
    
-    63          80 LOAD_CONST               5 (<code object test_decode_one_hot_test_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_utils.py", line 63>)
+    63          80 LOAD_CONST               5 (<code object test_decode_one_hot_test_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_utils.py", line 63>)
                 82 MAKE_FUNCTION            0
                 84 STORE_NAME              15 (test_decode_one_hot_test_data)
    
-   102          86 LOAD_CONST               6 (<code object test_split_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_utils.py", line 102>)
+   102          86 LOAD_CONST               6 (<code object test_split_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_utils.py", line 102>)
                 88 MAKE_FUNCTION            0
                 90 STORE_NAME              16 (test_split_data)
                 92 LOAD_CONST               1 (None)
                 94 RETURN_VALUE
    consts
       0
       None
@@ -188,15 +188,15 @@
             ('py0', 'py2')
             'assert %(py4)s'
             'py4'
          names      ('get_item_categories', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('test_data', 'item_categories', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_utils.py'
          name       'test_get_item_categories'
          firstlineno 5
          lnotab 0x02011e01
       code
          argcount  : 1
          nlocals   : 15
          stacksize : 9
@@ -989,15 +989,15 @@
             ('py0', 'py2', 'py4', 'py6')
             'assert %(py8)s'
             'py8'
          names      ('torch', 'tensor', 'float', 'to', 'one_hot_encode_test_data', 'all', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape', 'sum', 'dtype', 'float32', 'pytest', 'raises', 'ValueError')
          varnames   ('device', 'scores', 'item_categories', 'one_hot_scores', 'expected', '@py_assert1', '@py_assert4', '@py_assert8', '@py_format6', '@py_format10', '@py_assert3', '@py_format8', '@py_assert5', '@py_format7', '@py_format9')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_utils.py'
          name       'test_one_hot_encode_test_data'
          firstlineno 9
          lnotab
             0x02045a01240126fd020508030c0106ff1205160206010601060106fc02
             ff0e08240126f6020dff00ff00ae030c0106ff1204160206010601060106
             fc02ff0e0726f90209ff00ff00ae01ff00a101ff00ff00280134010c012e
             ff12ff2e04340128ff
@@ -1384,15 +1384,15 @@
                     1442 PRECALL                  3
                     1446 CALL                     3
                     1456 STORE_FAST               3 (one_hot_scores)
          
           95        1458 LOAD_GLOBAL             11 (NULL + decode_one_hot_test_data)
          
           96        1470 LOAD_FAST                3 (one_hot_scores)
-                    1472 LOAD_CONST              19 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_utils.py", line 96>)
+                    1472 LOAD_CONST              19 (<code object <listcomp>, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_utils.py", line 96>)
                     1474 MAKE_FUNCTION            0
                     1476 LOAD_FAST                2 (item_categories)
                     1478 GET_ITER
                     1480 PRECALL                  0
                     1484 CALL                     0
          
           95        1494 PRECALL                  2
@@ -1584,28 +1584,28 @@
                        >>   22 RETURN_VALUE
                consts
                   1
                names      ()
                varnames   ('.0', 'item_cat')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_utils.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_utils.py'
                name       '<listcomp>'
                firstlineno 96
                lnotab 0x
             1
             ('%(py3)s == (%(py5)s + %(py7)s)',)
             ('py3', 'py5', 'py7')
             'assert %(py12)s\n{%(py12)s = %(py2)s\n{%(py2)s = %(py0)s.all\n}(%(py10)s)\n}'
             ('py0', 'py2', 'py10', 'py12')
          names      ('torch', 'tensor', 'float', 'to', 'one_hot_encode_test_data', 'decode_one_hot_test_data', 'all', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'pytest', 'raises', 'ValueError')
          varnames   ('device', 'scores', 'item_categories', 'one_hot_scores', 'decoded_scores', '@py_assert1', '@py_assert4', '@py_assert8', '@py_format6', '@py_format10', '@py_assert6', '@py_assert11', '@py_format9', '@py_format13')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_utils.py'
          name       'test_decode_one_hot_test_data'
          firstlineno 63
          lnotab
             0x0202880124fe020308020c0106ff12042003ff00ff00ae02340148ff2e
             02340124ff2e05880124fe020308030c0106ff12050c0118ff1005
       code
          argcount  : 0
@@ -2644,22 +2644,22 @@
             40
             1.0
             0.0
          names      ('torch', 'manual_seed', 'rand', 'split_data', 'shape', '@pytest_ar', '_call_reprcompare', '_saferepr', 'AssertionError', '_format_explanation', 'equal', '@py_builtins', 'locals', '_should_repr_global_name')
          varnames   ('data', 'train_data', 'test_data', '@py_assert0', '@py_assert3', '@py_assert2', '@py_format5', '@py_format7', '@py_assert1', '@py_assert6', '@py_assert8', '@py_format9', '@py_format8')
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_utils.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_utils.py'
          name       'test_split_data'
          firstlineno 102
          lnotab
             0x020128012a032a01ff001301ff001301ff00ff002c032a01ff001301ff
             001301ff00ff0022032a01ff001301ff0013032a01ff001301ff0013032a
             01ff001301
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'irtorch.utils', 'get_item_categories', 'one_hot_encode_test_data', 'decode_one_hot_test_data', 'split_data', 'test_get_item_categories', 'test_one_hot_encode_test_data', 'test_decode_one_hot_test_data', 'test_split_data')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_utils.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_utils.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201220108011802060406360627
```

### Comparing `irtorch-0.0.2/tests/__pycache__/test_vaeirt.cpython-311-pytest-7.3.1.pyc` & `irtorch-0.0.3/tests/__pycache__/test_vaeirt.cpython-311-pytest-7.3.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -55,15 +55,15 @@
                 72 IMPORT_NAME             12 (irtorch.models)
                 74 IMPORT_FROM             13 (MonotoneNN)
                 76 STORE_NAME              13 (MonotoneNN)
                 78 POP_TOP
    
     12          80 PUSH_NULL
                 82 LOAD_BUILD_CLASS
-                84 LOAD_CONST               5 (<code object TestVAIRT, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_vaeirt.py", line 12>)
+                84 LOAD_CONST               5 (<code object TestVAIRT, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_vaeirt.py", line 12>)
                 86 MAKE_FUNCTION            0
                 88 LOAD_CONST               6 ('TestVAIRT')
                 90 PRECALL                  2
                 94 CALL                     2
                104 STORE_NAME              14 (TestVAIRT)
                106 LOAD_CONST               1 (None)
                108 RETURN_VALUE
@@ -96,61 +96,61 @@
          
           13          10 PUSH_NULL
                       12 LOAD_NAME                3 (pytest)
                       14 LOAD_ATTR                4 (fixture)
                       24 PRECALL                  0
                       28 CALL                     0
          
-          14          38 LOAD_CONST               1 (<code object algorithm, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_vaeirt.py", line 13>)
+          14          38 LOAD_CONST               1 (<code object algorithm, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_vaeirt.py", line 13>)
                       40 MAKE_FUNCTION            0
          
           13          42 PRECALL                  0
                       46 CALL                     0
          
           14          56 STORE_NAME               5 (algorithm)
          
           35          58 PUSH_NULL
                       60 LOAD_NAME                3 (pytest)
                       62 LOAD_ATTR                4 (fixture)
                       72 PRECALL                  0
                       76 CALL                     0
          
-          36          86 LOAD_CONST               2 (<code object algorithm_small_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_vaeirt.py", line 35>)
+          36          86 LOAD_CONST               2 (<code object algorithm_small_data, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_vaeirt.py", line 35>)
                       88 MAKE_FUNCTION            0
          
           35          90 PRECALL                  0
                       94 CALL                     0
          
           36         104 STORE_NAME               6 (algorithm_small_data)
          
           58         106 LOAD_CONST               3 ('algorithm')
                      108 LOAD_NAME                7 (VAEIRT)
                      110 BUILD_TUPLE              2
-                     112 LOAD_CONST               4 (<code object test_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_vaeirt.py", line 58>)
+                     112 LOAD_CONST               4 (<code object test_forward, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_vaeirt.py", line 58>)
                      114 MAKE_FUNCTION            4 (annotations)
                      116 STORE_NAME               8 (test_forward)
          
           98         118 LOAD_CONST               3 ('algorithm')
                      120 LOAD_NAME                7 (VAEIRT)
                      122 BUILD_TUPLE              2
-                     124 LOAD_CONST               5 (<code object test_latent_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_vaeirt.py", line 98>)
+                     124 LOAD_CONST               5 (<code object test_latent_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_vaeirt.py", line 98>)
                      126 MAKE_FUNCTION            4 (annotations)
                      128 STORE_NAME               9 (test_latent_scores)
          
          102         130 LOAD_CONST               3 ('algorithm')
                      132 LOAD_NAME                7 (VAEIRT)
                      134 BUILD_TUPLE              2
-                     136 LOAD_CONST               6 (<code object test__impute_missing_with_prior, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_vaeirt.py", line 102>)
+                     136 LOAD_CONST               6 (<code object test__impute_missing_with_prior, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_vaeirt.py", line 102>)
                      138 MAKE_FUNCTION            4 (annotations)
                      140 STORE_NAME              10 (test__impute_missing_with_prior)
          
          127         142 LOAD_CONST               3 ('algorithm')
                      144 LOAD_NAME                7 (VAEIRT)
                      146 BUILD_TUPLE              2
-                     148 LOAD_CONST               7 (<code object test__mean_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_vaeirt.py", line 127>)
+                     148 LOAD_CONST               7 (<code object test__mean_scores, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_vaeirt.py", line 127>)
                      150 MAKE_FUNCTION            4 (annotations)
                      152 STORE_NAME              11 (test__mean_scores)
          
          158         154 LOAD_NAME                3 (pytest)
                      156 LOAD_ATTR               12 (mark)
                      166 LOAD_METHOD             13 (parametrize)
                      188 LOAD_CONST               8 ('iw_samples')
@@ -161,15 +161,15 @@
                      200 CALL                     2
          
          159         210 LOAD_CONST              11 ('algorithm_small_data')
          
          161         212 LOAD_NAME                7 (VAEIRT)
          
          159         214 BUILD_TUPLE              2
-                     216 LOAD_CONST              12 (<code object test__loss_function, file "c:\Users\wallm\git\irtorch\irtorch-0.0.2\tests\test_vaeirt.py", line 158>)
+                     216 LOAD_CONST              12 (<code object test__loss_function, file "c:\Users\wallm\git\irtorch\irtorch-0.0.3\tests\test_vaeirt.py", line 158>)
                      218 MAKE_FUNCTION            4 (annotations)
          
          158         220 PRECALL                  0
                      224 CALL                     0
          
          159         234 STORE_NAME              14 (test__loss_function)
                      236 LOAD_CONST              13 (None)
@@ -268,15 +268,15 @@
                   ('latent_variables', 'item_categories', 'hidden_dim')
                   20
                   ('model', 'hidden_layers_encoder', 'nonlinear_encoder')
                names      ('torch', 'cuda', 'is_available', 'pytest', 'skip', 'MonotoneNN', 'VAEIRT', 'nn', 'ELU', 'data_loader', 'validation_data_loader', 'initialize_fit')
                varnames   ('self', 'device', 'latent_variables', 'item_categories', 'data_loaders', 'model', 'algorithm')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
                name       'algorithm'
                firstlineno 13
                lnotab
                   0x0202480128020c010201020104fd12050c01020104013afd12071e021e
                   01
             code
                argcount  : 4
@@ -355,15 +355,15 @@
                   ('latent_variables', 'item_categories', 'hidden_dim')
                   20
                   ('model', 'hidden_layers_encoder', 'nonlinear_encoder')
                names      ('torch', 'manual_seed', 'MonotoneNN', 'VAEIRT', 'nn', 'ELU', 'data_loader', 'validation_data_loader', 'initialize_fit')
                varnames   ('self', 'latent_variables', 'item_categories_small', 'data_loaders_small', 'model', 'algorithm')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
                name       'algorithm_small_data'
                firstlineno 35
                lnotab 0x020528010c010201020104fd12050c01020104013afd12071e021e01
             'algorithm'
             code
                argcount  : 3
                nlocals   : 10
@@ -1514,15 +1514,15 @@
                   2
                   3
                   10
                names      ('iw_samples', 'len', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'shape', 'max', 'model', 'modeled_item_responses', 'latent_variables')
                varnames   ('self', 'algorithm', 'test_data', 'output', '@py_assert2', '@py_assert5', '@py_assert4', '@py_format7', '@py_format9', '@py_assert0')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
                name       'test_forward'
                firstlineno 58
                lnotab
                   0x02010e011601ff00ff00240112030afd04030afd140314fd1c0314fd32
                   030afd28030afd1c030afd1c030afd40030afd300412030afd04030afd08
                   0314fd20030afd28030afd1c030afd1c030afd40030afd300412030afd04
                   030afd080314fd20030afd28030afd1c030afd1c030afd40030afd300412
@@ -1656,15 +1656,15 @@
                   ('py0', 'py2', 'py5')
                   'assert %(py7)s'
                   'py7'
                names      ('z_scores', 'shape', 'model', 'latent_variables', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
                varnames   ('self', 'algorithm', 'test_data', 'output', '@py_assert1', '@py_assert4', '@py_assert3', '@py_format6', '@py_format8')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
                name       'test_latent_scores'
                firstlineno 98
                lnotab 0x02012a01
             code
                argcount  : 2
                nlocals   : 19
                stacksize : 14
@@ -2070,15 +2070,15 @@
                   'assert %(py0)s'
                   'py0'
                   'replaced'
                names      ('torch', 'full', 'float', 'tensor', 'imputation_method', '_impute_missing_with_prior', 'equal', 'bool', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'not_equal')
                varnames   ('self', 'algorithm', 'a', 'b', 'data', 'missing_mask', 'imputed_data', '@py_assert1', '@py_assert4', '@py_assert6', '@py_assert8', '@py_assert10', '@py_assert12', '@py_assert14', '@py_assert16', '@py_assert18', '@py_format20', 'replaced', '@py_format1')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
                name       'test__impute_missing_with_prior'
                firstlineno 102
                lnotab
                   0x02010a0152011602060106010601060106fb02ff100a0e012c010c030a
                   fd0e030afd24030afd200324fd3a030afd1e030afd28030afd2a030afd1e
                   030afd1e030afd28030afd2a030afd1c030afd1c030afd1c030afd1c030a
                   fd1c030afd1c030afd1c030afd32030afd440416014c0132fe1404d0fc
@@ -2336,15 +2336,15 @@
                   'torch'
                   'means'
                   ('py0', 'py2', 'py3', 'py4', 'py6', 'py8', 'py10', 'py12', 'py14')
                names      ('torch', 'tensor', '_mean_scores', 'allclose', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
                varnames   ('self', 'algorithm', 'logits', 'means', '@py_assert1', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_assert13', '@py_format15')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
                name       'test__mean_scores'
                firstlineno 127
                lnotab
                   0x0201160206ff02ff10172a010c040afc0e040afc56040afc1e040afc28
                   040afc2a040afc1e040afc1e040afc1e040afc22040afc1e040afc28040a
                   fc2a040afc1c040afc1c040afc1c040afc1c040afc32040afc
             'iw_samples'
@@ -2596,33 +2596,33 @@
                   ('py0', 'py3')
                   'assert %(py5)s'
                   'py5'
                names      ('iw_samples', 'torch', 'tensor', 'inf', 'repeat', 'exp', 'randn_like', '_loss_function', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
                varnames   ('self', 'algorithm_small_data', 'test_data', 'iw_samples', 'latent_variables', 'logits', 'means', 'logvars', 'std', 'z_samples', 'loss', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
                freevars   ()
                cellvars   ()
-               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+               filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
                name       'test__loss_function'
                firstlineno 158
                lnotab
                   0x02080e011602240124fe02ff0e0528fb0206440104ff1003440104ff10
                   032e013401180122ff1003
             None
          names      ('__name__', '__module__', '__qualname__', 'pytest', 'fixture', 'algorithm', 'algorithm_small_data', 'VAEIRT', 'test_forward', 'test_latent_scores', 'test__impute_missing_with_prior', 'test__mean_scores', 'mark', 'parametrize', 'test__loss_function')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+         filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
          name       'TestVAIRT'
          firstlineno 12
          lnotab
             0x0a011c0104ff0e0102151c0104ff0e0102160c280c040c190c1f380102
             0202fe06ff0e01
       'TestVAIRT'
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'torch', 'utils', 'initialize_fit', 'irtorch.estimation_algorithms.vaeirt', 'VAEIRT', 'irtorch.models', 'MonotoneNN', 'TestVAIRT')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.2\\tests\\test_vaeirt.py'
+   filename   'c:\\Users\\wallm\\git\\irtorch\\irtorch-0.0.3\\tests\\test_vaeirt.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201220108010c010c010c07
```

### Comparing `irtorch-0.0.2/tests/test_activation_functions.py` & `irtorch-0.0.3/tests/test_activation_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_aeirt.py` & `irtorch-0.0.3/tests/test_aeirt.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_base_irt_model.py` & `irtorch-0.0.3/tests/test_base_irt_model.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_config.py` & `irtorch-0.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_integration.py` & `irtorch-0.0.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_internal_utils.py` & `irtorch-0.0.3/tests/test_internal_utils.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_irt_evaluator.py` & `irtorch-0.0.3/tests/test_irt_evaluator.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_irt_plotter.py` & `irtorch-0.0.3/tests/test_irt_plotter.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_irt_scorer.py` & `irtorch-0.0.3/tests/test_irt_scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,33 @@
     mock_model.model_missing = False
     mock_model.log_likelihood = MagicMock(side_effect=log_likelihood_mock)
     mock_algorithm.z_scores = MagicMock(side_effect=z_scores_mock)
     mock_algorithm.fix_missing_values = MagicMock(side_effect=fix_missing_values_mock)
 
     return IRTScorer(mock_model, mock_algorithm)
 
+from unittest.mock import patch
+from irtorch.irt_scorer import GaussianMixtureModel
+
+@pytest.mark.parametrize("cv_n_components", [[1], [1, 2, 3]])
+def test_cv_gaussian_mixture_model(irt_scorer: IRTScorer, cv_n_components):
+    data = torch.randn(100, irt_scorer.model.latent_variables)
+
+    with patch.object(GaussianMixtureModel, "fit") as mock_fit, patch.object(GaussianMixtureModel, "__call__") as mock_call:
+        mock_fit.return_value = None
+        mock_call.return_value = torch.tensor(1.0)
+
+        gmm = irt_scorer._cv_gaussian_mixture_model(data, cv_n_components)
+
+    assert isinstance(gmm, GaussianMixtureModel)
+    assert gmm.n_components == cv_n_components[0]
+    assert gmm.n_features == data.shape[1]
+    mock_fit.assert_called()
+    if len(cv_n_components) > 1:
+        assert mock_call.call_count == len(cv_n_components) * 5  # 5-fold cross-validation
 
 @pytest.mark.parametrize("one_dimensional", [True, False])
 @pytest.mark.parametrize("bit_score_z_grid_method", ["NN", "ML"])
 def test_bit_scores(irt_scorer: IRTScorer, one_dimensional, latent_variables, bit_score_z_grid_method):
     z = torch.tensor([[0.8], [2.1], [-0.7], [-0.5]]).repeat(1, latent_variables)
     z = z[1::2] * -1 # invert every other scale
     start_z = torch.full((1, latent_variables), -0.2)
```

### Comparing `irtorch-0.0.2/tests/test_latent_variable_functions.py` & `irtorch-0.0.3/tests/test_latent_variable_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_layers.py` & `irtorch-0.0.3/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_load_dataset.py` & `irtorch-0.0.3/tests/test_load_dataset.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_monotone_nn.py` & `irtorch-0.0.3/tests/test_monotone_nn.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_outlier_detector.py` & `irtorch-0.0.3/tests/test_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_parametric.py` & `irtorch-0.0.3/tests/test_parametric.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_quantile_mv_normal.py` & `irtorch-0.0.3/tests/test_quantile_mv_normal.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_utils.py` & `irtorch-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.2/tests/test_vaeirt.py` & `irtorch-0.0.3/tests/test_vaeirt.py`

 * *Files identical despite different names*

