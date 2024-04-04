# Comparing `tmp/kernel_tuner-1.0.0b5.tar.gz` & `tmp/kernel_tuner-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernel_tuner-1.0.0b5.tar", max compression
+gzip compressed data, was "kernel_tuner-1.0.0b6.tar", max compression
```

## Comparing `kernel_tuner-1.0.0b5.tar` & `kernel_tuner-1.0.0b6.tar`

### file list

```diff
@@ -1,67 +1,92 @@
--rw-r--r--   0        0        0    11358 2023-11-01 14:12:00.669399 kernel_tuner-1.0.0b5/LICENSE
--rw-r--r--   0        0        0     9485 2023-11-01 14:12:00.669399 kernel_tuner-1.0.0b5/README.rst
--rw-r--r--   0        0        0    21072 2023-11-01 14:12:00.681399 kernel_tuner-1.0.0b5/doc/source/convolution.ipynb
--rw-r--r--   0        0        0   248632 2023-11-01 14:12:00.681399 kernel_tuner-1.0.0b5/doc/source/diffusion.ipynb
--rw-r--r--   0        0        0   137909 2023-11-01 14:12:00.681399 kernel_tuner-1.0.0b5/doc/source/diffusion_opencl.ipynb
--rw-r--r--   0        0        0   128093 2023-11-01 14:12:00.681399 kernel_tuner-1.0.0b5/doc/source/diffusion_use_optparam.ipynb
--rw-r--r--   0        0        0    21342 2023-11-01 14:12:00.681399 kernel_tuner-1.0.0b5/doc/source/grid3d.ipynb
--rw-r--r--   0        0        0    22883 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/doc/source/matrix_multiplication.ipynb
--rw-r--r--   0        0        0      209 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/__init__.py
--rw-r--r--   0        0        0    10468 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/accuracy.py
--rw-r--r--   0        0        0        0 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/backends/__init__.py
--rw-r--r--   0        0        0     2704 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/backends/backend.py
--rw-r--r--   0        0        0    13049 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/backends/compiler.py
--rw-r--r--   0        0        0     9316 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/backends/cupy.py
--rw-r--r--   0        0        0    12200 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/backends/hip.py
--rw-r--r--   0        0        0    13391 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/backends/nvcuda.py
--rw-r--r--   0        0        0     7865 2023-11-01 14:12:00.685399 kernel_tuner-1.0.0b5/kernel_tuner/backends/opencl.py
--rw-r--r--   0        0        0    15313 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/backends/pycuda.py
--rw-r--r--   0        0        0    39796 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/core.py
--rw-r--r--   0        0        0        0 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/energy/__init__.py
--rw-r--r--   0        0        0     8115 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/energy/energy.py
--rw-r--r--   0        0        0     9962 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/file_utils.py
--rw-r--r--   0        0        0     3245 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/hyper.py
--rw-r--r--   0        0        0    17441 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/integration.py
--rw-r--r--   0        0        0    31990 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/interface.py
--rw-r--r--   0        0        0     4637 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/kernelbuilder.py
--rw-r--r--   0        0        0       95 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/__init__.py
--rw-r--r--   0        0        0      622 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/compiler.py
--rw-r--r--   0        0        0      756 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/cupy.py
--rw-r--r--   0        0        0     1026 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/hip.py
--rw-r--r--   0        0        0      849 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/nvcuda.py
--rw-r--r--   0        0        0    23257 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/nvml.py
--rw-r--r--   0        0        0     1878 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/observer.py
--rw-r--r--   0        0        0      612 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/opencl.py
--rw-r--r--   0        0        0     3173 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/pmt.py
--rw-r--r--   0        0        0     2193 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/powersensor.py
--rw-r--r--   0        0        0      661 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/observers/pycuda.py
--rw-r--r--   0        0        0        0 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/runners/__init__.py
--rw-r--r--   0        0        0      489 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/runners/runner.py
--rw-r--r--   0        0        0     5277 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/runners/sequential.py
--rw-r--r--   0        0        0     5535 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/runners/simulation.py
--rw-r--r--   0        0        0     1494 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/schema/T4/1.0.0/metadata-schema.json
--rw-r--r--   0        0        0     2780 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/schema/T4/1.0.0/results-schema.json
--rw-r--r--   0        0        0    35649 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/searchspace.py
--rw-r--r--   0        0        0        0 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/__init__.py
--rw-r--r--   0        0        0     1697 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/basinhopping.py
--rw-r--r--   0        0        0    47842 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/bayes_opt.py
--rw-r--r--   0        0        0      405 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/brute_force.py
--rw-r--r--   0        0        0     9025 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/common.py
--rw-r--r--   0        0        0     1725 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/diff_evo.py
--rw-r--r--   0        0        0     1511 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/dual_annealing.py
--rw-r--r--   0        0        0     4536 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/firefly_algorithm.py
--rw-r--r--   0        0        0     6665 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/genetic_algorithm.py
--rw-r--r--   0        0        0     2792 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/greedy_ils.py
--rw-r--r--   0        0        0     1805 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/greedy_mls.py
--rw-r--r--   0        0        0     3622 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/hillclimbers.py
--rw-r--r--   0        0        0     1419 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/minimize.py
--rw-r--r--   0        0        0     1270 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/mls.py
--rw-r--r--   0        0        0     1271 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/ordered_greedy_mls.py
--rw-r--r--   0        0        0     3765 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/pso.py
--rw-r--r--   0        0        0     1201 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/random_sample.py
--rw-r--r--   0        0        0     4310 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/strategies/simulated_annealing.py
--rw-r--r--   0        0        0    51563 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/util.py
--rw-r--r--   0        0        0        0 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/utils/__init__.py
--rw-r--r--   0        0        0    10310 2023-11-01 14:12:00.689399 kernel_tuner-1.0.0b5/kernel_tuner/utils/directives.py
--rw-r--r--   0        0        0     5846 2023-11-01 14:12:00.693399 kernel_tuner-1.0.0b5/pyproject.toml
--rw-r--r--   0        0        0    11807 1970-01-01 00:00:00.000000 kernel_tuner-1.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-11-08 13:52:46.127085 kernel_tuner-1.0.0b6/LICENSE
+-rw-r--r--   0        0        0     9485 2023-11-08 13:52:46.127085 kernel_tuner-1.0.0b6/README.rst
+-rw-r--r--   0        0        0      209 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/__init__.py
+-rw-r--r--   0        0        0    10468 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/accuracy.py
+-rw-r--r--   0        0        0        0 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/backends/__init__.py
+-rw-r--r--   0        0        0     2704 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/backends/backend.py
+-rw-r--r--   0        0        0    13049 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/backends/compiler.py
+-rw-r--r--   0        0        0     9316 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/backends/cupy.py
+-rw-r--r--   0        0        0    12200 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/backends/hip.py
+-rw-r--r--   0        0        0    13391 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/backends/nvcuda.py
+-rw-r--r--   0        0        0     7865 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/backends/opencl.py
+-rw-r--r--   0        0        0    15313 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/backends/pycuda.py
+-rw-r--r--   0        0        0    39796 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/core.py
+-rw-r--r--   0        0        0        0 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/energy/__init__.py
+-rw-r--r--   0        0        0     8115 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/energy/energy.py
+-rw-r--r--   0        0        0     9962 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/file_utils.py
+-rw-r--r--   0        0        0     3245 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/hyper.py
+-rw-r--r--   0        0        0    17441 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/integration.py
+-rw-r--r--   0        0        0    32036 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/interface.py
+-rw-r--r--   0        0        0     4637 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/kernelbuilder.py
+-rw-r--r--   0        0        0       95 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/__init__.py
+-rw-r--r--   0        0        0      622 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/compiler.py
+-rw-r--r--   0        0        0      756 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/cupy.py
+-rw-r--r--   0        0        0     1026 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/hip.py
+-rw-r--r--   0        0        0      849 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/nvcuda.py
+-rw-r--r--   0        0        0    23257 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/nvml.py
+-rw-r--r--   0        0        0     1878 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/observer.py
+-rw-r--r--   0        0        0      612 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/opencl.py
+-rw-r--r--   0        0        0     3173 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/pmt.py
+-rw-r--r--   0        0        0     2193 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/powersensor.py
+-rw-r--r--   0        0        0      661 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/observers/pycuda.py
+-rw-r--r--   0        0        0        0 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/runners/__init__.py
+-rw-r--r--   0        0        0      489 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/runners/runner.py
+-rw-r--r--   0        0        0     5277 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/runners/sequential.py
+-rw-r--r--   0        0        0     5535 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/runners/simulation.py
+-rw-r--r--   0        0        0     1494 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/schema/T4/1.0.0/metadata-schema.json
+-rw-r--r--   0        0        0     2780 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/schema/T4/1.0.0/results-schema.json
+-rw-r--r--   0        0        0    35649 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/searchspace.py
+-rw-r--r--   0        0        0        0 2023-11-08 13:52:46.143086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/__init__.py
+-rw-r--r--   0        0        0     1697 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/basinhopping.py
+-rw-r--r--   0        0        0    47842 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/bayes_opt.py
+-rw-r--r--   0        0        0      405 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/brute_force.py
+-rw-r--r--   0        0        0     9025 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/common.py
+-rw-r--r--   0        0        0     1725 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/diff_evo.py
+-rw-r--r--   0        0        0     1511 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/dual_annealing.py
+-rw-r--r--   0        0        0     4536 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/firefly_algorithm.py
+-rw-r--r--   0        0        0     6665 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/genetic_algorithm.py
+-rw-r--r--   0        0        0     2792 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/greedy_ils.py
+-rw-r--r--   0        0        0     1805 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/greedy_mls.py
+-rw-r--r--   0        0        0     3622 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/hillclimbers.py
+-rw-r--r--   0        0        0     1419 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/minimize.py
+-rw-r--r--   0        0        0     1270 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/mls.py
+-rw-r--r--   0        0        0     1271 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/ordered_greedy_mls.py
+-rw-r--r--   0        0        0     3765 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/pso.py
+-rw-r--r--   0        0        0     1201 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/random_sample.py
+-rw-r--r--   0        0        0     4310 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/strategies/simulated_annealing.py
+-rw-r--r--   0        0        0    51563 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/util.py
+-rw-r--r--   0        0        0        0 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/utils/__init__.py
+-rw-r--r--   0        0        0    10310 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/kernel_tuner/utils/directives.py
+-rw-r--r--   0        0        0     5832 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/__init__.py
+-rw-r--r--   0        0        0     3157 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/context.py
+-rw-r--r--   0        0        0     5859 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/strategies/test_bayesian_optimization.py
+-rw-r--r--   0        0        0     2130 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/strategies/test_common.py
+-rw-r--r--   0        0        0     2189 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/strategies/test_genetic_algorithm.py
+-rw-r--r--   0        0        0     2736 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/strategies/test_strategies.py
+-rw-r--r--   0        0        0     6088 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/synthetic_fp32_cache_NVIDIA_RTX_A4000.json
+-rw-r--r--   0        0        0     2826 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_accuracy.py
+-rw-r--r--   0        0        0      832 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_backend.py
+-rw-r--r--   0        0        0     8630 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_cache_file.json
+-rw-r--r--   0        0        0     2343 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_common.py
+-rw-r--r--   0        0        0     9118 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_compiler_functions.py
+-rw-r--r--   0        0        0    11050 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_core.py
+-rw-r--r--   0        0        0     1530 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_cuda_functions.py
+-rw-r--r--   0        0        0      251 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_cupy_functions.py
+-rw-r--r--   0        0        0      581 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_energy.py
+-rw-r--r--   0        0        0     1492 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_file_utils.py
+-rw-r--r--   0        0        0     4332 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_hip_functions.py
+-rw-r--r--   0        0        0      492 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_hyper.py
+-rw-r--r--   0        0        0     7645 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_integration.py
+-rw-r--r--   0        0        0     1988 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_kernelbuilder.py
+-rw-r--r--   0        0        0     1733 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_nvml_mocked.py
+-rw-r--r--   0        0        0      949 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_observers.py
+-rw-r--r--   0        0        0     2701 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_opencl_functions.py
+-rw-r--r--   0        0        0     1517 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_pycuda_functions.py
+-rw-r--r--   0        0        0     4288 2023-11-08 13:52:46.147086 kernel_tuner-1.0.0b6/test/test_pycuda_mocked.py
+-rw-r--r--   0        0        0     9940 2023-11-08 13:52:46.151085 kernel_tuner-1.0.0b6/test/test_runners.py
+-rw-r--r--   0        0        0    18073 2023-11-08 13:52:46.151085 kernel_tuner-1.0.0b6/test/test_searchspace.py
+-rw-r--r--   0        0        0     2151 2023-11-08 13:52:46.151085 kernel_tuner-1.0.0b6/test/test_toml_file.py
+-rw-r--r--   0        0        0    24922 2023-11-08 13:52:46.151085 kernel_tuner-1.0.0b6/test/test_util_functions.py
+-rw-r--r--   0        0        0     5915 2023-11-08 13:52:46.151085 kernel_tuner-1.0.0b6/test/test_utils_directives.py
+-rw-r--r--   0        0        0    11807 1970-01-01 00:00:00.000000 kernel_tuner-1.0.0b6/PKG-INFO
```

### Comparing `kernel_tuner-1.0.0b5/LICENSE` & `kernel_tuner-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/README.rst` & `kernel_tuner-1.0.0b6/README.rst`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/accuracy.py` & `kernel_tuner-1.0.0b6/kernel_tuner/accuracy.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/backends/backend.py` & `kernel_tuner-1.0.0b6/kernel_tuner/backends/backend.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/backends/compiler.py` & `kernel_tuner-1.0.0b6/kernel_tuner/backends/compiler.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/backends/cupy.py` & `kernel_tuner-1.0.0b6/kernel_tuner/backends/cupy.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/backends/hip.py` & `kernel_tuner-1.0.0b6/kernel_tuner/backends/hip.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/backends/nvcuda.py` & `kernel_tuner-1.0.0b6/kernel_tuner/backends/nvcuda.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/backends/opencl.py` & `kernel_tuner-1.0.0b6/kernel_tuner/backends/opencl.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/backends/pycuda.py` & `kernel_tuner-1.0.0b6/kernel_tuner/backends/pycuda.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/core.py` & `kernel_tuner-1.0.0b6/kernel_tuner/core.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/energy/energy.py` & `kernel_tuner-1.0.0b6/kernel_tuner/energy/energy.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/file_utils.py` & `kernel_tuner-1.0.0b6/kernel_tuner/file_utils.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/hyper.py` & `kernel_tuner-1.0.0b6/kernel_tuner/hyper.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/integration.py` & `kernel_tuner-1.0.0b6/kernel_tuner/integration.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/interface.py` & `kernel_tuner-1.0.0b6/kernel_tuner/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,15 +617,15 @@
     logging.debug("tuning_options: %s", util.get_config_string(tuning_options))
     logging.debug("device_options: %s", util.get_config_string(device_options))
 
     if strategy:
         if strategy in strategy_map:
             strategy = strategy_map[strategy]
         else:
-            raise ValueError("Strategy %s not recognized" % strategy)
+            raise ValueError(f"Unkown strategy {strategy}, must be one of: {', '.join(list(strategy_map.keys()))}")
 
         # make strategy_options into an Options object
         if tuning_options.strategy_options:
             if not isinstance(strategy_options, Options):
                 tuning_options.strategy_options = Options(strategy_options)
 
             # select strategy based on user options
```

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/kernelbuilder.py` & `kernel_tuner-1.0.0b6/kernel_tuner/kernelbuilder.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/compiler.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/compiler.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/cupy.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/cupy.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/hip.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/hip.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/nvcuda.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/nvcuda.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/nvml.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/nvml.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/observer.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/observer.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/opencl.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/opencl.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/pmt.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/pmt.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/powersensor.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/powersensor.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/observers/pycuda.py` & `kernel_tuner-1.0.0b6/kernel_tuner/observers/pycuda.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/runners/sequential.py` & `kernel_tuner-1.0.0b6/kernel_tuner/runners/sequential.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/runners/simulation.py` & `kernel_tuner-1.0.0b6/kernel_tuner/runners/simulation.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/schema/T4/1.0.0/metadata-schema.json` & `kernel_tuner-1.0.0b6/kernel_tuner/schema/T4/1.0.0/metadata-schema.json`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/schema/T4/1.0.0/results-schema.json` & `kernel_tuner-1.0.0b6/kernel_tuner/schema/T4/1.0.0/results-schema.json`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/searchspace.py` & `kernel_tuner-1.0.0b6/kernel_tuner/searchspace.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/basinhopping.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/basinhopping.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/bayes_opt.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/bayes_opt.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/common.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/common.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/diff_evo.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/diff_evo.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/dual_annealing.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/dual_annealing.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/firefly_algorithm.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/firefly_algorithm.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/genetic_algorithm.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/greedy_ils.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/greedy_ils.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/greedy_mls.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/greedy_mls.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/hillclimbers.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/hillclimbers.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/minimize.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/minimize.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/mls.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/mls.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/ordered_greedy_mls.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/ordered_greedy_mls.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/pso.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/pso.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/random_sample.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/random_sample.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/strategies/simulated_annealing.py` & `kernel_tuner-1.0.0b6/kernel_tuner/strategies/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/util.py` & `kernel_tuner-1.0.0b6/kernel_tuner/util.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/kernel_tuner/utils/directives.py` & `kernel_tuner-1.0.0b6/kernel_tuner/utils/directives.py`

 * *Files identical despite different names*

### Comparing `kernel_tuner-1.0.0b5/pyproject.toml` & `kernel_tuner-1.0.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.7.0", "setuptools>=67.7.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kernel_tuner"
 packages = [{ include = "kernel_tuner", from = "." }]
 description = "An easy to use CUDA/OpenCL kernel tuner in Python"
-version = "1.0.0b5" # adhere to PEP440 versioning: https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#id55
+version = "1.0.0b6" # adhere to PEP440 versioning: https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#id55
 license = "Apache-2.0"
 authors = [
     "Ben van Werkhoven <b.vanwerkhoven@esciencecenter.nl>",
     "Alessio Sclocco <a.sclocco@esciencecenter.nl>",
     "Stijn Heldens <s.heldens@esciencecenter.nl>",
     "Floris-Jan Willemsen <f.j.Willemsen@esciencecenter.nl>",
     "Willem-Jan Palenstijn <w.j.palenstijn@liacs.leidenuniv.nl>",
@@ -40,15 +40,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
     "Topic :: System :: Distributed Computing",
 ]
 include = [
-    { path = "doc/source/*.ipynb" },
+    { path = "test" },
 ] # this ensures that people won't have to clone the whole repo to include notebooks, they can just do `pip install kernel_tuner[tutorial,cuda]`
 homepage = "https://KernelTuner.github.io/kernel_tuner/"
 documentation = "https://KernelTuner.github.io/kernel_tuner/"
 repository = "https://github.com/KernelTuner/kernel_tuner"
 [tool.poetry.urls]
 "Tracker" = "https://github.com/KernelTuner/kernel_tuner/issues"
 [tool.poetry.build]
```

### Comparing `kernel_tuner-1.0.0b5/PKG-INFO` & `kernel_tuner-1.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kernel_tuner
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: An easy to use CUDA/OpenCL kernel tuner in Python
 Home-page: https://KernelTuner.github.io/kernel_tuner/
 License: Apache-2.0
 Keywords: auto-tuning,gpu,computing,pycuda,cuda,pyopencl,opencl
 Author: Ben van Werkhoven
 Author-email: b.vanwerkhoven@esciencecenter.nl
 Requires-Python: >=3.8,<3.12
```

