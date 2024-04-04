# Comparing `tmp/qarray-0.0.1.tar.gz` & `tmp/qarray-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qarray-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qarray-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qarray-0.0.1.tar` & `qarray-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,68 @@
--rw-r--r--   0        0        0     1003 2023-10-11 18:18:28.045800 qarray-0.0.1/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0     3079 2023-10-11 18:18:28.045800 qarray-0.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2023-10-11 18:18:28.045800 qarray-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-10-11 18:18:28.045800 qarray-0.0.1/README.md
--rw-r--r--   0        0        0       15 2023-10-11 18:18:28.045800 qarray-0.0.1/__init__.py
--rw-r--r--   0        0        0      418 2023-10-11 18:18:28.045800 qarray-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       90 2023-10-11 18:18:28.045800 qarray-0.0.1/qarray/__init__.py
--rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 qarray-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      862 2024-04-04 11:27:56.018243 qarray-1.0.0/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0     1302 2024-04-04 11:27:56.018243 qarray-1.0.0/.github/workflows/run_tests.yaml
+-rw-r--r--   0        0        0     3079 2024-04-04 11:27:56.018243 qarray-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1087 2024-04-04 11:27:56.018243 qarray-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2856 2024-04-04 11:27:56.018243 qarray-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 11:27:56.018243 qarray-1.0.0/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-04 11:27:56.018243 qarray-1.0.0/docs/installation.rst
+-rw-r--r--   0        0        0     1652 2024-04-04 11:27:56.018243 qarray-1.0.0/docs/simulating_double_dot.rst
+-rw-r--r--   0        0        0     2507 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/charge_sensing.py
+-rw-r--r--   0        0        0     2632 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/double_dot.py
+-rw-r--r--   0        0        0      589 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/gate_voltage_composer_tricks.py
+-rw-r--r--   0        0        0     1933 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/gradient.py
+-rw-r--r--   0        0        0     2747 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/linear_quadruple_dot.py
+-rw-r--r--   0        0        0     2520 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/linear_triple_dot.py
+-rw-r--r--   0        0        0      694 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/paper_examples.py
+-rw-r--r--   0        0        0     2650 2024-04-04 11:27:56.022243 qarray-1.0.0/examples/quadruple_dot_all_gates.py
+-rw-r--r--   0        0        0     3229 2024-04-04 11:27:56.022243 qarray-1.0.0/examples/simulating_closed_5_.py
+-rw-r--r--   0        0        0     1597 2024-04-04 11:27:56.022243 qarray-1.0.0/examples/simulating_linear_open_quadruple_dot.py
+-rw-r--r--   0        0        0     2888 2024-04-04 11:27:56.022243 qarray-1.0.0/examples/triple_dot.py
+-rw-r--r--   0        0        0      669 2024-04-04 11:27:56.022243 qarray-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      506 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      640 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2649 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/closed.py
+-rw-r--r--   0        0        0     2429 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/open.py
+-rw-r--r--   0        0        0      114 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      634 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2372 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/closed.py
+-rw-r--r--   0        0        0     2094 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/open.py
+-rw-r--r--   0        0        0     6570 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/BaseDataClass.py
+-rw-r--r--   0        0        0     5629 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/ChargeSensedDotArray.py
+-rw-r--r--   0        0        0     7092 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/DotArray.py
+-rw-r--r--   0        0        0    10321 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/GateVoltageComposer.py
+-rw-r--r--   0        0        0      139 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/__init__.py
+-rw-r--r--   0        0        0     7884 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/_helper_functions.py
+-rw-r--r--   0        0        0     5334 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/functions.py
+-rw-r--r--   0        0        0       84 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      726 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     6227 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/closed.py
+-rw-r--r--   0        0        0      275 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/helper_functions.py
+-rw-r--r--   0        0        0     4819 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/open.py
+-rw-r--r--   0        0        0       80 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0     1486 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
+-rw-r--r--   0        0        0      947 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     7025 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/core_python.py
+-rw-r--r--   0        0        0      258 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/qarray_types/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/qarray_types/typing_classes.py
+-rw-r--r--   0        0        0      109 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/rust_core/__init__.py
+-rw-r--r--   0        0        0     3750 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/rust_core/core_rust.py
+-rw-r--r--   0        0        0      338 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/GLOBAL_OPTIONS.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     3357 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/helper_functions.py
+-rw-r--r--   0        0        0      939 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/pydantic_validation_tests.py
+-rw-r--r--   0        0        0     6195 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/test_against_brute_force.py
+-rw-r--r--   0        0        0    17563 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/test_charge_combinations.py
+-rw-r--r--   0        0        0     6115 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/test_double_dot.py
+-rw-r--r--   0        0        0     3978 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_gate_voltage_composer.py
+-rw-r--r--   0        0        0     5944 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_quadruple_dot.py
+-rw-r--r--   0        0        0     4579 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_solver.py
+-rw-r--r--   0        0        0     9900 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_threshold.py
+-rw-r--r--   0        0        0     5938 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_triple_dot.py
+-rw-r--r--   0        0        0     1729 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_user_interaction.py
+-rw-r--r--   0        0        0      109 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/tests.py
+-rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 qarray-1.0.0/PKG-INFO
```

### Comparing `qarray-0.0.1/.github/workflows/pypi.yaml` & `qarray-1.0.0/.github/workflows/pypi.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 name: pypi
 
 # Controls when the workflow will run
 on:
     push:
         branches:
             - main
-    pull_request:
-    workflow_dispatch:
-
-
-# A workflow run is made up of one or more jobs that can run sequentially or in parallel
+        tags:
+            - 'publish'
+            
 jobs:
-
-    # This workflow contains a single job called "publish"
     publish:
 
         # The type of runner that the job will run on
         runs-on: ubuntu-latest
 
         # Steps represent a sequence of tasks that will be executed as part of the job
         steps:
```

### Comparing `qarray-0.0.1/.gitignore` & `qarray-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qarray-0.0.1/LICENSE` & `qarray-1.0.0/LICENSE`

 * *Files identical despite different names*

