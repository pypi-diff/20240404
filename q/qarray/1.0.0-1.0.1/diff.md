# Comparing `tmp/qarray-1.0.0.tar.gz` & `tmp/qarray-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qarray-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qarray-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qarray-1.0.0.tar` & `qarray-1.0.1.tar`

### file list

```diff
@@ -1,68 +1,71 @@
--rw-r--r--   0        0        0      862 2024-04-04 11:27:56.018243 qarray-1.0.0/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0     1302 2024-04-04 11:27:56.018243 qarray-1.0.0/.github/workflows/run_tests.yaml
--rw-r--r--   0        0        0     3079 2024-04-04 11:27:56.018243 qarray-1.0.0/.gitignore
--rw-r--r--   0        0        0     1087 2024-04-04 11:27:56.018243 qarray-1.0.0/LICENSE
--rw-r--r--   0        0        0     2856 2024-04-04 11:27:56.018243 qarray-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-04 11:27:56.018243 qarray-1.0.0/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-04 11:27:56.018243 qarray-1.0.0/docs/installation.rst
--rw-r--r--   0        0        0     1652 2024-04-04 11:27:56.018243 qarray-1.0.0/docs/simulating_double_dot.rst
--rw-r--r--   0        0        0     2507 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/charge_sensing.py
--rw-r--r--   0        0        0     2632 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/double_dot.py
--rw-r--r--   0        0        0      589 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/gate_voltage_composer_tricks.py
--rw-r--r--   0        0        0     1933 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/gradient.py
--rw-r--r--   0        0        0     2747 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/linear_quadruple_dot.py
--rw-r--r--   0        0        0     2520 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/linear_triple_dot.py
--rw-r--r--   0        0        0      694 2024-04-04 11:27:56.018243 qarray-1.0.0/examples/paper_examples.py
--rw-r--r--   0        0        0     2650 2024-04-04 11:27:56.022243 qarray-1.0.0/examples/quadruple_dot_all_gates.py
--rw-r--r--   0        0        0     3229 2024-04-04 11:27:56.022243 qarray-1.0.0/examples/simulating_closed_5_.py
--rw-r--r--   0        0        0     1597 2024-04-04 11:27:56.022243 qarray-1.0.0/examples/simulating_linear_open_quadruple_dot.py
--rw-r--r--   0        0        0     2888 2024-04-04 11:27:56.022243 qarray-1.0.0/examples/triple_dot.py
--rw-r--r--   0        0        0      669 2024-04-04 11:27:56.022243 qarray-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      506 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/__init__.py
--rw-r--r--   0        0        0      108 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/__init__.py
--rw-r--r--   0        0        0       80 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      640 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2649 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/closed.py
--rw-r--r--   0        0        0     2429 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_jax/open.py
--rw-r--r--   0        0        0      114 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/__init__.py
--rw-r--r--   0        0        0       83 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      634 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     2372 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/closed.py
--rw-r--r--   0        0        0     2094 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/brute_force_python/open.py
--rw-r--r--   0        0        0     6570 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/BaseDataClass.py
--rw-r--r--   0        0        0     5629 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/ChargeSensedDotArray.py
--rw-r--r--   0        0        0     7092 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/DotArray.py
--rw-r--r--   0        0        0    10321 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/GateVoltageComposer.py
--rw-r--r--   0        0        0      139 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/__init__.py
--rw-r--r--   0        0        0     7884 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/classes/_helper_functions.py
--rw-r--r--   0        0        0     5334 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/functions.py
--rw-r--r--   0        0        0       84 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/__init__.py
--rw-r--r--   0        0        0       68 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0      726 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     6227 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/closed.py
--rw-r--r--   0        0        0      275 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/helper_functions.py
--rw-r--r--   0        0        0     4819 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/jax_core/open.py
--rw-r--r--   0        0        0       80 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/__init__.py
--rw-r--r--   0        0        0      132 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/charge_configuration_generators/__init__.py
--rw-r--r--   0        0        0     1486 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
--rw-r--r--   0        0        0      947 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
--rw-r--r--   0        0        0     7025 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/python_core/core_python.py
--rw-r--r--   0        0        0      258 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/qarray_types/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/qarray_types/typing_classes.py
--rw-r--r--   0        0        0      109 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/rust_core/__init__.py
--rw-r--r--   0        0        0     3750 2024-04-04 11:27:56.022243 qarray-1.0.0/qarray/rust_core/core_rust.py
--rw-r--r--   0        0        0      338 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/GLOBAL_OPTIONS.py
--rw-r--r--   0        0        0        0 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3357 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/helper_functions.py
--rw-r--r--   0        0        0      939 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/pydantic_validation_tests.py
--rw-r--r--   0        0        0     6195 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/test_against_brute_force.py
--rw-r--r--   0        0        0    17563 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/test_charge_combinations.py
--rw-r--r--   0        0        0     6115 2024-04-04 11:27:56.022243 qarray-1.0.0/tests/test_double_dot.py
--rw-r--r--   0        0        0     3978 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_gate_voltage_composer.py
--rw-r--r--   0        0        0     5944 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_quadruple_dot.py
--rw-r--r--   0        0        0     4579 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_solver.py
--rw-r--r--   0        0        0     9900 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_threshold.py
--rw-r--r--   0        0        0     5938 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_triple_dot.py
--rw-r--r--   0        0        0     1729 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/test_user_interaction.py
--rw-r--r--   0        0        0      109 2024-04-04 11:27:56.026243 qarray-1.0.0/tests/tests.py
--rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 qarray-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      850 2024-04-04 18:54:29.129871 qarray-1.0.1/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0     1317 2024-04-04 18:54:29.129871 qarray-1.0.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3079 2024-04-04 18:54:29.129871 qarray-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1087 2024-04-04 18:54:29.129871 qarray-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2958 2024-04-04 18:54:29.129871 qarray-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 18:54:29.129871 qarray-1.0.1/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-04 18:54:29.129871 qarray-1.0.1/docs/installation.rst
+-rw-r--r--   0        0        0     1652 2024-04-04 18:54:29.129871 qarray-1.0.1/docs/simulating_double_dot.rst
+-rw-r--r--   0        0        0     2507 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/charge_sensing.py
+-rw-r--r--   0        0        0     2632 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/double_dot.py
+-rw-r--r--   0        0        0      589 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/gate_voltage_composer_tricks.py
+-rw-r--r--   0        0        0     1933 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/gradient.py
+-rw-r--r--   0        0        0     2747 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/linear_quadruple_dot.py
+-rw-r--r--   0        0        0     2520 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/linear_triple_dot.py
+-rw-r--r--   0        0        0      694 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/paper_examples.py
+-rw-r--r--   0        0        0     2650 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/quadruple_dot_all_gates.py
+-rw-r--r--   0        0        0     3229 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/simulating_closed_five_dot_array_.py
+-rw-r--r--   0        0        0     1597 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/simulating_open_four_dot_array.py
+-rw-r--r--   0        0        0     2888 2024-04-04 18:54:29.129871 qarray-1.0.1/examples/triple_dot.py
+-rw-r--r--   0        0        0    27960 2024-04-04 18:54:29.133871 qarray-1.0.1/misc/recreations.jpg
+-rw-r--r--   0        0        0    17300 2024-04-04 18:54:29.133871 qarray-1.0.1/misc/structure.jpg
+-rw-r--r--   0        0        0      669 2024-04-04 18:54:29.133871 qarray-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      506 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      640 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2649 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/closed.py
+-rw-r--r--   0        0        0     2429 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_jax/open.py
+-rw-r--r--   0        0        0      114 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      634 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     2372 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/closed.py
+-rw-r--r--   0        0        0     2094 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/brute_force_python/open.py
+-rw-r--r--   0        0        0     6570 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/BaseDataClass.py
+-rw-r--r--   0        0        0     5629 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/ChargeSensedDotArray.py
+-rw-r--r--   0        0        0     7092 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/DotArray.py
+-rw-r--r--   0        0        0    10321 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/GateVoltageComposer.py
+-rw-r--r--   0        0        0      139 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/__init__.py
+-rw-r--r--   0        0        0     7884 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/classes/_helper_functions.py
+-rw-r--r--   0        0        0     5334 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/functions.py
+-rw-r--r--   0        0        0       84 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0      726 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     6227 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/closed.py
+-rw-r--r--   0        0        0      275 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/helper_functions.py
+-rw-r--r--   0        0        0     4819 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/jax_core/open.py
+-rw-r--r--   0        0        0       80 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/charge_configuration_generators/__init__.py
+-rw-r--r--   0        0        0     1486 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py
+-rw-r--r--   0        0        0      947 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/charge_configuration_generators/open_dot_configurations.py
+-rw-r--r--   0        0        0     7025 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/python_core/core_python.py
+-rw-r--r--   0        0        0      258 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/qarray_types/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/qarray_types/typing_classes.py
+-rw-r--r--   0        0        0      109 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/rust_core/__init__.py
+-rw-r--r--   0        0        0     3750 2024-04-04 18:54:29.133871 qarray-1.0.1/qarray/rust_core/core_rust.py
+-rw-r--r--   0        0        0      133 2024-04-04 18:54:29.133871 qarray-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      338 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/GLOBAL_OPTIONS.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     3357 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/helper_functions.py
+-rw-r--r--   0        0        0      939 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/pydantic_validation_tests.py
+-rw-r--r--   0        0        0     6190 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/test_against_brute_force.py
+-rw-r--r--   0        0        0    17563 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/test_charge_combinations.py
+-rw-r--r--   0        0        0     6110 2024-04-04 18:54:29.133871 qarray-1.0.1/tests/test_double_dot.py
+-rw-r--r--   0        0        0     3978 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_gate_voltage_composer.py
+-rw-r--r--   0        0        0     5939 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_quadruple_dot.py
+-rw-r--r--   0        0        0     4579 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_solver.py
+-rw-r--r--   0        0        0     9900 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_threshold.py
+-rw-r--r--   0        0        0     5938 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_triple_dot.py
+-rw-r--r--   0        0        0     1724 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/test_user_interaction.py
+-rw-r--r--   0        0        0      109 2024-04-04 18:54:29.137871 qarray-1.0.1/tests/tests.py
+-rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 qarray-1.0.1/PKG-INFO
```

### Comparing `qarray-1.0.0/.github/workflows/pypi.yaml` & `qarray-1.0.1/.github/workflows/pypi.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Controls when the workflow will run
 on:
     push:
         branches:
             - main
         tags:
             - 'publish'
-            
+
 jobs:
     publish:
 
         # The type of runner that the job will run on
         runs-on: ubuntu-latest
 
         # Steps represent a sequence of tasks that will be executed as part of the job
```

### Comparing `qarray-1.0.0/.github/workflows/run_tests.yaml` & `qarray-1.0.1/.github/workflows/test.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 with:
                     python-version: ${{ matrix.python-version }}
 
             -   name: Install dependencies
                 run: pip install -r requirements.txt
 
             -   name: Run unit tests
-                run: python -m unittest discover -s tests
+                run: python -m unittest discover -s ./tests -t ./
 
 
     windows:
         runs-on: windows-latest
         strategy:
             matrix:
                 python-version: [ '3.10', '3.11' ]
@@ -41,8 +41,8 @@
                 with:
                     python-version: ${{ matrix.python-version }}
 
             -   name: Install dependencies
                 run: pip install -r requirements.txt
 
             -   name: Run unit tests
-                run: python -m unittest discover -s tests
+                run: python -m unittest discover -s ./tests -t .
```

### Comparing `qarray-1.0.0/.gitignore` & `qarray-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/LICENSE` & `qarray-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/README.md` & `qarray-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # Qarray
 
-![GitHub Workflow Status](https://github.com/b-vanstraaten/rusty_capacitance_model/workflows/tests/badge.svg)
-![PyPI](https://img.shields.io/pypi/v/rusty-capacitance-model)
+![GitHub Workflow Status](https://github.com/b-vanstraaten/qarray/actions/workflows/test.yaml//badge.svg)
+![PyPI](https://img.shields.io/pypi/v/qarray)
+
+![structure.jpg](./misc/structure.jpg)
 
 **Qarray** is a high-performance Python package that leverages the power of Rust and Jax to provide a fully parallelised
 and optimised simulation environment for quantum dots with constant capacitance. It can run on both CPUs and GPUs,
 and is designed to be easy to use and integrate into your existing workflow.
 
-## Features
+Harnesses the speed of Rust or the compute power of GPUs using Jax to deliver charge stability diagrams in seconds or
+millisecond
 
-- **Ultra-fast Simulation:** Harnesses the speed of Rust or the compute power of GPUs using Jax to deliver
-  lightning-fast simulations.
-- **Constant Capacitance:** Specialized for simulating quantum dots with constant capacitance, allowing precise
-  modelling of charge stability diagrams.
-- **User-Friendly:** Designed with ease of use in mind, making it accessible to both experts and newcomers in quantum dot simulations.
-- **Extensive Documentation:** Comprehensive documentation and examples to help you get started quickly.
+![recreations.jpg](./misc/recreations.jpg)
 
 ## Installation
 
 Install Quantum Dot Constant Capacitance Simulator using pip:
 
 ```bash
 pip install qarray
@@ -54,24 +52,23 @@
 # defining the gate voltage sweep we wish to perform
 vg = voltage_composer.do2d(
     x_gate=0, x_min=-0.5, x_max=0.5, x_res=100,
     y_gate=1, y_min=-0.5, y_max=0.5, y_res=100
 )
 
 # run the simulation with the quantum dot array open such that the number of charge carriers is not fixed
-n_open = model.get_n(
-    vg)  # n_open is a (100, 100, 2) array encoding the number of charge carriers in each dot for each gate voltage
+n_open = model.ground_state_open(vg)  # n_open is a (100, 100, 2) array encoding the 
+# number of charge carriers in each dot for each gate voltage
 # run the simulation with the quantum dot array closed such that the number of charge carriers is fixed to 2
-n_closed = model.get_n(vg, n_charge=2)
-
+n_closed = model.ground_state_closed(vg, n_charge_carriers=2)  # n_closed is a (100, 100, 2) array encoding the 
+# number of charge carriers in each dot for each gate voltage
 ```
-
 ## Examples
 
 The examples folder contains a number of examples that demonstrate how to use the package to simulate different quantum
 dot systems.
 
-1. [Double Quantum Dot]()
-2. [Linear Triple Quantum Dot]()
-3. [Linear Quadruple Quantum Dot]()
-4. [Charge sensed double quantum dot]()
+1. [Double Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/double_dot.py)
+2. [Linear Triple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_triple_dot.py)
+3. [Linear Quadruple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_quadruple_dot.py)
+4. [Charge sensed double quantum dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/charge_sensing.py)
```

### Comparing `qarray-1.0.0/docs/installation.rst` & `qarray-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/docs/simulating_double_dot.rst` & `qarray-1.0.1/docs/simulating_double_dot.rst`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/charge_sensing.py` & `qarray-1.0.1/examples/charge_sensing.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/double_dot.py` & `qarray-1.0.1/examples/double_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/gate_voltage_composer_tricks.py` & `qarray-1.0.1/examples/gate_voltage_composer_tricks.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/gradient.py` & `qarray-1.0.1/examples/gradient.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/linear_quadruple_dot.py` & `qarray-1.0.1/examples/linear_quadruple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/linear_triple_dot.py` & `qarray-1.0.1/examples/linear_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/paper_examples.py` & `qarray-1.0.1/examples/paper_examples.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/quadruple_dot_all_gates.py` & `qarray-1.0.1/examples/quadruple_dot_all_gates.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/simulating_closed_5_.py` & `qarray-1.0.1/examples/simulating_closed_five_dot_array_.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/simulating_linear_open_quadruple_dot.py` & `qarray-1.0.1/examples/simulating_open_four_dot_array.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/examples/triple_dot.py` & `qarray-1.0.1/examples/triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/pyproject.toml` & `qarray-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.1/qarray/brute_force_jax/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/brute_force_jax/closed.py` & `qarray-1.0.1/qarray/brute_force_jax/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/brute_force_jax/open.py` & `qarray-1.0.1/qarray/brute_force_jax/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.1/qarray/brute_force_python/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/brute_force_python/closed.py` & `qarray-1.0.1/qarray/brute_force_python/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/brute_force_python/open.py` & `qarray-1.0.1/qarray/brute_force_python/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/classes/BaseDataClass.py` & `qarray-1.0.1/qarray/classes/BaseDataClass.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/classes/ChargeSensedDotArray.py` & `qarray-1.0.1/qarray/classes/ChargeSensedDotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/classes/DotArray.py` & `qarray-1.0.1/qarray/classes/DotArray.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/classes/GateVoltageComposer.py` & `qarray-1.0.1/qarray/classes/GateVoltageComposer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/classes/_helper_functions.py` & `qarray-1.0.1/qarray/classes/_helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/functions.py` & `qarray-1.0.1/qarray/functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.1/qarray/jax_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/jax_core/closed.py` & `qarray-1.0.1/qarray/jax_core/closed.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/jax_core/open.py` & `qarray-1.0.1/qarray/jax_core/open.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py` & `qarray-1.0.1/qarray/python_core/charge_configuration_generators/closed_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/python_core/charge_configuration_generators/open_dot_configurations.py` & `qarray-1.0.1/qarray/python_core/charge_configuration_generators/open_dot_configurations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/python_core/core_python.py` & `qarray-1.0.1/qarray/python_core/core_python.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/qarray_types/typing_classes.py` & `qarray-1.0.1/qarray/qarray_types/typing_classes.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/qarray/rust_core/core_rust.py` & `qarray-1.0.1/qarray/rust_core/core_rust.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/tests/helper_functions.py` & `qarray-1.0.1/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/tests/pydantic_validation_tests.py` & `qarray-1.0.1/tests/pydantic_validation_tests.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/tests/test_against_brute_force.py` & `qarray-1.0.1/tests/test_against_brute_force.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 from tqdm import tqdm
 
 from qarray import (ground_state_open_rust, ground_state_closed_rust, dot_occupation_changes)
 from qarray.brute_force_jax import ground_state_open_brute_force_jax, ground_state_closed_brute_force_jax
-from tests.helper_functions import randomly_generate_matrices, too_different
 from .GLOBAL_OPTIONS import disable_tqdm, N_ITERATIONS, N_VOLTAGES
+from .helper_functions import randomly_generate_matrices, too_different
 
 
 class BruteForceTests(unittest.TestCase):
     def test_double_dot_open(self):
         """
         Test that the python and rust open double dot ground state functions return the same result.
```

### Comparing `qarray-1.0.0/tests/test_charge_combinations.py` & `qarray-1.0.1/tests/test_charge_combinations.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/tests/test_double_dot.py` & `qarray-1.0.1/tests/test_double_dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from tqdm import tqdm
 
 from qarray import (ground_state_open_rust, ground_state_closed_rust, ground_state_open_python,
                     ground_state_closed_python, optimal_Vg, compute_threshold)
 from qarray.jax_core import ground_state_open_jax, ground_state_closed_jax
-from tests.helper_functions import randomly_generate_matrices, too_different
 from .GLOBAL_OPTIONS import disable_tqdm, N_ITERATIONS, N_VOLTAGES
+from .helper_functions import randomly_generate_matrices, too_different
 
 
 class DoubleDotTests(unittest.TestCase):
     def test_python_vs_rust_open(self):
         """
         Test that the python and rust open double dot ground state functions return the same result.
```

### Comparing `qarray-1.0.0/tests/test_gate_voltage_composer.py` & `qarray-1.0.1/tests/test_gate_voltage_composer.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/tests/test_quadruple_dot.py` & `qarray-1.0.1/tests/test_quadruple_dot.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from qarray import (ground_state_open_rust, ground_state_closed_rust, ground_state_open_python,
                     ground_state_closed_python, optimal_Vg, compute_threshold)
 from qarray.jax_core import ground_state_open_jax, ground_state_closed_jax
-from tests.helper_functions import randomly_generate_matrices, too_different
 from .GLOBAL_OPTIONS import N_ITERATIONS, N_VOLTAGES
+from .helper_functions import randomly_generate_matrices, too_different
 
 
 class DoubleDotTests(unittest.TestCase):
     def test_python_vs_rust_open(self):
         """
         Test that the python and rust open double dot ground state functions return the same result.
```

### Comparing `qarray-1.0.0/tests/test_solver.py` & `qarray-1.0.1/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/tests/test_threshold.py` & `qarray-1.0.1/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/tests/test_triple_dot.py` & `qarray-1.0.1/tests/test_triple_dot.py`

 * *Files identical despite different names*

### Comparing `qarray-1.0.0/tests/test_user_interaction.py` & `qarray-1.0.1/tests/test_user_interaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
 from qarray import (DotArray, GateVoltageComposer)
-from tests.helper_functions import if_errors
+from .helper_functions import if_errors
 
 # setting up the constant capacitance model_threshold_1
 model = DotArray(
     Cdd=[
         [0., 0.1],
         [0.1, 0.]
     ],
```

### Comparing `qarray-1.0.0/PKG-INFO` & `qarray-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qarray
-Version: 1.0.0
+Version: 1.0.1
 Summary: Qarray is a Python package for simulating quantum dot arrays.
 Author-email: Barnaby van Straaten <barnaby.vanstraaten@kellogg.ox.ac.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: qarray-rust-core==1.2.0
 Requires-Dist: osqp==0.6.3
@@ -16,29 +16,27 @@
 Requires-Dist: jax>=0.2
 Requires-Dist: jaxopt>=0.4
 Requires-Dist: tqdm>=4.62
 Project-URL: Home, https://github.com/b-vanstraaten/qarray
 
 # Qarray
 
-![GitHub Workflow Status](https://github.com/b-vanstraaten/rusty_capacitance_model/workflows/tests/badge.svg)
-![PyPI](https://img.shields.io/pypi/v/rusty-capacitance-model)
+![GitHub Workflow Status](https://github.com/b-vanstraaten/qarray/actions/workflows/test.yaml//badge.svg)
+![PyPI](https://img.shields.io/pypi/v/qarray)
+
+![structure.jpg](./misc/structure.jpg)
 
 **Qarray** is a high-performance Python package that leverages the power of Rust and Jax to provide a fully parallelised
 and optimised simulation environment for quantum dots with constant capacitance. It can run on both CPUs and GPUs,
 and is designed to be easy to use and integrate into your existing workflow.
 
-## Features
+Harnesses the speed of Rust or the compute power of GPUs using Jax to deliver charge stability diagrams in seconds or
+millisecond
 
-- **Ultra-fast Simulation:** Harnesses the speed of Rust or the compute power of GPUs using Jax to deliver
-  lightning-fast simulations.
-- **Constant Capacitance:** Specialized for simulating quantum dots with constant capacitance, allowing precise
-  modelling of charge stability diagrams.
-- **User-Friendly:** Designed with ease of use in mind, making it accessible to both experts and newcomers in quantum dot simulations.
-- **Extensive Documentation:** Comprehensive documentation and examples to help you get started quickly.
+![recreations.jpg](./misc/recreations.jpg)
 
 ## Installation
 
 Install Quantum Dot Constant Capacitance Simulator using pip:
 
 ```bash
 pip install qarray
@@ -74,25 +72,24 @@
 # defining the gate voltage sweep we wish to perform
 vg = voltage_composer.do2d(
     x_gate=0, x_min=-0.5, x_max=0.5, x_res=100,
     y_gate=1, y_min=-0.5, y_max=0.5, y_res=100
 )
 
 # run the simulation with the quantum dot array open such that the number of charge carriers is not fixed
-n_open = model.get_n(
-    vg)  # n_open is a (100, 100, 2) array encoding the number of charge carriers in each dot for each gate voltage
+n_open = model.ground_state_open(vg)  # n_open is a (100, 100, 2) array encoding the 
+# number of charge carriers in each dot for each gate voltage
 # run the simulation with the quantum dot array closed such that the number of charge carriers is fixed to 2
-n_closed = model.get_n(vg, n_charge=2)
-
+n_closed = model.ground_state_closed(vg, n_charge_carriers=2)  # n_closed is a (100, 100, 2) array encoding the 
+# number of charge carriers in each dot for each gate voltage
 ```
-
 ## Examples
 
 The examples folder contains a number of examples that demonstrate how to use the package to simulate different quantum
 dot systems.
 
-1. [Double Quantum Dot]()
-2. [Linear Triple Quantum Dot]()
-3. [Linear Quadruple Quantum Dot]()
-4. [Charge sensed double quantum dot]()
+1. [Double Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/double_dot.py)
+2. [Linear Triple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_triple_dot.py)
+3. [Linear Quadruple Quantum Dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/linear_quadruple_dot.py)
+4. [Charge sensed double quantum dot](https://github.com/b-vanstraaten/qarray/blob/main/examples/charge_sensing.py)
```

