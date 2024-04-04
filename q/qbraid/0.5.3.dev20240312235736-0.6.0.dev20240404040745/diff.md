# Comparing `tmp/qbraid-0.5.3.dev20240312235736.tar.gz` & `tmp/qbraid-0.6.0.dev20240404040745.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.5.3.dev20240312235736.tar", last modified: Tue Mar 12 23:57:38 2024, max compression
+gzip compressed data, was "qbraid-0.6.0.dev20240404040745.tar", last modified: Thu Apr  4 04:07:47 2024, max compression
```

## Comparing `qbraid-0.5.3.dev20240312235736.tar` & `qbraid-0.6.0.dev20240404040745.tar`

### file list

```diff
@@ -1,253 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.585875 qbraid-0.5.3.dev20240312235736/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-03-12 23:57:38.585875 qbraid-0.5.3.dev20240312235736/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.549875 qbraid-0.5.3.dev20240312235736/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.549875 qbraid-0.5.3.dev20240312235736/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.549875 qbraid-0.5.3.dev20240312235736/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.553875 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/pennylane.png
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/qasm.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/quantinuum.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.553875 qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/batch_counts.png
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/conversion_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/hub_spokes.png
--rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/lab_jobs.png
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.557875 qbraid-0.5.3.dev20240312235736/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/api/qbraid.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/api/qbraid.compiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/api/qbraid.programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/api/qbraid.providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/api/qbraid.transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/api/qbraid.visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.557875 qbraid-0.5.3.dev20240312235736/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/sdk/programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/sdk/providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/docs/sdk/transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.557875 qbraid-0.5.3.dev20240312235736/qbraid/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/_qdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/_qprogram.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-12 23:57:36.000000 qbraid-0.5.3.dev20240312235736/qbraid/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.561875 qbraid-0.5.3.dev20240312235736/qbraid/api/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/api/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/api/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.561875 qbraid-0.5.3.dev20240312235736/qbraid/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.561875 qbraid-0.5.3.dev20240312235736/qbraid/compiler/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/compiler/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/compiler/braket/ionq.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/compiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/get_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.561875 qbraid-0.5.3.dev20240312235736/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/interface/circuit_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.561875 qbraid-0.5.3.dev20240312235736/qbraid/interface/random/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/interface/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/interface/random/cirq_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/interface/random/qasm3_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/interface/random/qiskit_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/interface/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/load_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/load_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.565875 qbraid-0.5.3.dev20240312235736/qbraid/programs/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/abc_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/pennylane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/qasm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15440 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/programs/qiskit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.565875 qbraid-0.5.3.dev20240312235736/qbraid/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.565875 qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.565875 qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/providers/status_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.569875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.569875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.569875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/cirq_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    13331 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/cirq_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/custom_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.569875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/cirq_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.569875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/openqasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/openqasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/openqasm3/convert_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.569875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pennylane/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pennylane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.569875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/quil_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    21875 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/quil_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.569875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pytket/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/qasm_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/qasm_qelib1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.573875 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/transpiler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.573875 qbraid-0.5.3.dev20240312235736/qbraid/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/visualization/draw_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/visualization/draw_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/visualization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/visualization/plot_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/qbraid/visualization/plot_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.581875 qbraid-0.5.3.dev20240312235736/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-03-12 23:57:38.000000 qbraid-0.5.3.dev20240312235736/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-03-12 23:57:38.000000 qbraid-0.5.3.dev20240312235736/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 23:57:38.000000 qbraid-0.5.3.dev20240312235736/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-12 23:57:38.000000 qbraid-0.5.3.dev20240312235736/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-12 23:57:38.000000 qbraid-0.5.3.dev20240312235736/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-12 23:57:38.000000 qbraid-0.5.3.dev20240312235736/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-12 23:57:38.589875 qbraid-0.5.3.dev20240312235736/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.573875 qbraid-0.5.3.dev20240312235736/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.573875 qbraid-0.5.3.dev20240312235736/tests/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/benchmarking/qaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/benchmarking/qiskit_to_braket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.573875 qbraid-0.5.3.dev20240312235736/tests/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/compiler/test_braket_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.573875 qbraid-0.5.3.dev20240312235736/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.573875 qbraid-0.5.3.dev20240312235736/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/interface/test_conversion_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/interface/test_conversion_grah.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/interface/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/interface/test_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.577875 qbraid-0.5.3.dev20240312235736/tests/programs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_abc_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_braket_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_circuit_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_cirq_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_pennylane_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_pytket_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_qasm2_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_qasm3_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/programs/test_qiskit_program.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.577875 qbraid-0.5.3.dev20240312235736/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/test_braket_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/test_braket_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/test_braket_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/test_datetime_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/test_qiskit_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/test_qiskit_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/test_quantum_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/providers/test_quantum_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.577875 qbraid-0.5.3.dev20240312235736/tests/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/cirq_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.577875 qbraid-0.5.3.dev20240312235736/tests/transpiler/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/coverage/test_coverage_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/coverage/test_coverage_from_cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/coverage/test_coverage_from_pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/coverage/test_coverage_from_pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/coverage/test_coverage_from_qiskit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.581875 qbraid-0.5.3.dev20240312235736/tests/transpiler/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/pytket/test_conversions_pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/pytket/test_from_pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/pytket/test_to_pytket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.581875 qbraid-0.5.3.dev20240312235736/tests/transpiler/qasm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/qasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/qasm/test_conversions_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/qasm/test_qasm2_to_qasm3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.581875 qbraid-0.5.3.dev20240312235736/tests/transpiler/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/qiskit/test_conversions_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/qiskit/test_from_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/qiskit/test_qiskit_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/qiskit/test_to_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/test_idle_qubits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/test_qasm2_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    20027 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/transpiler/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.581875 qbraid-0.5.3.dev20240312235736/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/visualization/test_circuit_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/visualization/test_plot_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tests/visualization/test_qasm3_circuit_drawer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:57:38.581875 qbraid-0.5.3.dev20240312235736/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tools/verify_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-12 23:57:32.000000 qbraid-0.5.3.dev20240312235736/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.776929 qbraid-0.6.0.dev20240404040745/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55239 2024-04-04 04:07:47.776929 qbraid-0.6.0.dev20240404040745/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.748930 qbraid-0.6.0.dev20240404040745/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.748930 qbraid-0.6.0.dev20240404040745/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.748930 qbraid-0.6.0.dev20240404040745/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.752930 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/pennylane.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/quantinuum.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.752930 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/batch_counts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/conversion_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/hub_spokes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/lab_jobs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.756929 qbraid-0.6.0.dev20240404040745/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.compiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/api/qbraid.visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.756929 qbraid-0.6.0.dev20240404040745/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/docs/sdk/transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.756929 qbraid-0.6.0.dev20240404040745/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 04:07:45.000000 qbraid-0.6.0.dev20240404040745/qbraid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/ionq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/compiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/get_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/circuit_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/cirq_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/qasm3_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/qiskit_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/interface/random/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.760929 qbraid-0.6.0.dev20240404040745/qbraid/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/abc_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/programs/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/providers/status_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.764929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/cirq_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/cirq_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/custom_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/cirq_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/convert_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/conversions_qasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10806 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/quil_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21875 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/quil_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qasm_passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qasm_qelib1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.768929 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/conversions_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/transpiler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.772929 qbraid-0.6.0.dev20240404040745/qbraid/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/draw_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/draw_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/plot_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/qbraid/visualization/plot_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.772929 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55239 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 04:07:47.000000 qbraid-0.6.0.dev20240404040745/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:07:47.776929 qbraid-0.6.0.dev20240404040745/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:47.772929 qbraid-0.6.0.dev20240404040745/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/tools/set_provider_configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4480 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/tools/verify_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-04 04:07:39.000000 qbraid-0.6.0.dev20240404040745/tox.ini
```

### Comparing `qbraid-0.5.3.dev20240312235736/CODE_OF_CONDUCT.md` & `qbraid-0.6.0.dev20240404040745/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/CONTRIBUTING.md` & `qbraid-0.6.0.dev20240404040745/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/LICENSE` & `qbraid-0.6.0.dev20240404040745/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/PKG-INFO` & `qbraid-0.6.0.dev20240404040745/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,7 @@
-Metadata-Version: 2.1
-Name: qbraid
-Version: 0.5.3.dev20240312235736
-Summary: A Python toolkit for cross-framework abstraction of quantum programs.
-Home-page: https://www.qbraid.com/
-Author: qBraid Development Team
-Author-email: contact@qbraid.com
-License: GPL v3.0
-Project-URL: Documentation, https://docs.qbraid.com/en/latest/
-Project-URL: Bug Tracker, https://github.com/qBraid/qBraid/issues
-Project-URL: Source Code, https://github.com/qBraid/qBraid
-Project-URL: Discord, https://discord.gg/TPBU2sa8Et
-Project-URL: Launch on Lab, https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid.git
-Keywords: qbraid,quantum
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: networkx<4.0,>=2.5
-Requires-Dist: numpy<1.27,>=1.17
-Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
-Requires-Dist: ply>=3.6
-Requires-Dist: requests>=2.28.0
-Provides-Extra: braket
-Requires-Dist: amazon-braket-sdk<1.74.0,>=1.42.1; extra == "braket"
-Provides-Extra: cirq
-Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
-Provides-Extra: pennylane
-Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane"
-Provides-Extra: pytket
-Requires-Dist: pytket<1.26.0,>=1.16.0; extra == "pytket"
-Provides-Extra: pyquil
-Requires-Dist: pyquil<4.4.0,>=3.5.4; extra == "pyquil"
-Provides-Extra: qiskit
-Requires-Dist: qiskit<1.1.0,>=0.44.0; extra == "qiskit"
-Requires-Dist: qiskit-ibm-provider<0.11.0,>=0.5.3; extra == "qiskit"
-Requires-Dist: qiskit-ibm-runtime<0.21.0,>=0.18.0; extra == "qiskit"
-Provides-Extra: qasm3
-Requires-Dist: qiskit-qasm3-import<0.5.0,>=0.2.0; extra == "qasm3"
-Provides-Extra: ionq
-Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "ionq"
-Requires-Dist: cirq-ionq<1.4.0,>=1.3.0; extra == "ionq"
-Requires-Dist: pytket-braket<0.35.0,>=0.30.0; extra == "ionq"
-Provides-Extra: all
-Requires-Dist: amazon-braket-sdk<1.74.0,>=1.42.1; extra == "all"
-Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "all"
-Requires-Dist: cirq-ionq<1.4.0,>=1.3.0; extra == "all"
-Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "all"
-Requires-Dist: pytket<1.26.0,>=1.16.0; extra == "all"
-Requires-Dist: pytket-braket<0.35.0,>=0.30.0; extra == "all"
-Requires-Dist: pyquil<4.5.0,>=3.5.4; extra == "all"
-Requires-Dist: qiskit<1.1.0,>=0.44.0; extra == "all"
-Requires-Dist: qiskit-ibm-provider<0.11.0,>=0.5.3; extra == "all"
-Requires-Dist: qiskit-ibm-runtime<0.21.0,>=0.18.0; extra == "all"
-Requires-Dist: qiskit-qasm3-import<0.5.0,>=0.2.0; extra == "all"
-Provides-Extra: visualization
-Requires-Dist: ipython; extra == "visualization"
-Requires-Dist: matplotlib; extra == "visualization"
-Requires-Dist: pylatexenc; extra == "visualization"
-Requires-Dist: qiskit[visualization]; extra == "visualization"
-Provides-Extra: docs
-Requires-Dist: sphinx~=7.2.6; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints<2.1,>=1.24; extra == "docs"
-Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
-
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
 <p align="center">
   <a href="https://github.com/qBraid/qBraid/actions/workflows/main.yml">
     <img src="https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg?branch=main" alt="CI"/>
   </a>
   <a href="https://codecov.io/gh/qBraid/qBraid">
@@ -138,15 +64,15 @@
 ```
 
 You can also [install from source](CONTRIBUTING.md#installing-from-source) by cloning this repository and running a pip install command in the root directory of the repository:
 
 ```bash
 git clone https://github.com/qBraid/qBraid.git
 cd qBraid
-pip install -e '.[all]'
+pip install .
 ```
 
 *Note*: The qBraid-SDK requires Python 3.9 or greater.
 
 If using locally, follow linked instructions to configure your
 [qBraid](#local-account-setup),
 [AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-credentials),
@@ -181,51 +107,51 @@
 Construct a quantum program of any supported program type.
 
 Below, `SUPPORTED_QPROGRAMS` maps shorthand identifiers for supported quantum programs, each corresponding to a type in the typed `QPROGRAM` Union.
 For example, 'qiskit' maps to `qiskit.QuantumCircuit` in `QPROGRAM`. Notably, 'qasm2' and 'qasm3' both represent raw OpenQASM strings.
 This arrangement simplifies targeting and transpiling between different quantum programming frameworks.
 
 ```python
->>> from qbraid import SUPPORTED_QPROGRAMS
+>>> from qbraid.programs import SUPPORTED_QPROGRAMS
 >>> SUPPORTED_QPROGRAMS
 {'cirq': 'cirq.circuits.circuit.Circuit',
  'qiskit': 'qiskit.circuit.quantumcircuit.QuantumCircuit',
  'pyquil': 'pyquil.quil.Program',
  'pytket': 'pytket._tket.circuit.Circuit',
  'braket': 'braket.circuits.circuit.Circuit',
  'openqasm3': 'openqasm3.ast.Program',
  'qasm2': 'str',
  'qasm3': 'str'}
 ```
 
-Pass any quantum program of type `qbraid.QPROGRAM` to the `circuit_wrapper()` and specify a target package
+Pass any quantum program of type `qbraid.programs.QPROGRAM` to the `load_program()` and specify a target package
 from `SUPPORTED_QPROGRAMS` to "transpile" your circuit to a new program type:
 
 ```python
->>> from qbraid import circuit_wrapper
 >>> from qbraid.interface import random_circuit
+>>> from qbraid.transpiler import transpile
 >>> qiskit_circuit = random_circuit("qiskit")
->>> cirq_circuit = circuit_wrapper(qiskit_circuit).transpile("cirq")
+>>> cirq_circuit = transpile(qiskit_circuit, "cirq")
 >>> print(qiskit_circuit)
           ┌────────────┐
 q_0: ──■──┤ Rx(3.0353) ├
      ┌─┴─┐└───┬────┬───┘
 q_1: ┤ H ├────┤ √X ├────
      └───┘    └────┘
 >>> print(cirq_circuit)
 0: ───@───Rx(0.966π)───
       │
 1: ───H───X^0.5────────
 ```
 
-The same functionality can be achieved using the underlying `convert_to_package()` function directly:
+The same functionality can be achieved using the underlying `transpile()` function directly:
 
 ```python
->>> from qbraid import convert_to_package
->>> cirq_circuit = convert_to_package(qiskit_circuit, "cirq")
+>>> from qbraid.transpiler import transpile
+>>> cirq_circuit = transpile(qiskit_circuit, "cirq")
 ```
 
 Behind the scenes, the qBraid-SDK uses ``networkx`` to create a directional graph that maps all possible conversions between supported program types:
 
 ```python
 from qbraid.transpiler import ConversionGraph
 from qbraid.visualization import plot_conversion_graph
@@ -253,21 +179,32 @@
 aws_ionq_aria2                      OFFLINE
 aws_rigetti_aspen_m3                ONLINE
 ibm_q_brisbane                      ONLINE
 ...
 
 ```
 
-Apply the `device_wrapper()`, and send quantum jobs to any supported backend,
-from any supported program type:
+You can get a Python list of device objects using:
 
 ```python
->>> from qbraid import device_wrapper, get_jobs
->>> aws_device = device_wrapper("aws_oqc_lucy")
->>> ibm_device = device_wrapper("ibm_q_brisbane")
+from qbraid.providers import QbraidProvider
+
+provider = QbraidProvider()
+qdevices = provider.get_devices()
+```
+
+Or, instantiate a known device by ID via the `QbraidProvider.get_device()` method,
+and submit quantum jobs from any supported program type:
+
+```python
+>>> from qbraid import get_jobs
+>>> from qbraid.providers import QbraidProvider
+>>> provider = QbraidProvider()
+>>> aws_device = provider.get_device("aws_oqc_lucy")
+>>> ibm_device = provider.get_device("ibm_q_brisbane")
 >>> aws_job = aws_device.run(qiskit_circuit, shots=1000)
 >>> ibm_job = ibm_device.run(cirq_circuit, shots=1000)
 >>> get_jobs()
 Displaying 2 most recent jobs:
 
 Job ID                                              Submitted                  Status
 ------                                              ---------                  ------
@@ -298,38 +235,37 @@
 2. Copy your API Key token from the left side of
     your [account page](https://account.qbraid.com/):
 
 3. Save your API key from step 2 by calling
    `QbraidSession.save_config()`:
 
 ```python
-from qbraid.api import QbraidSession
+from qbraid_core import QbraidSession
 
 session = QbraidSession(api_key='API_KEY')
 session.save_config()
 ```
 
 The command above stores your credentials locally in a configuration file `~/.qbraid/qbraidrc`,
 where `~` corresponds to your home (`$HOME`) directory. Once saved, you can then connect to the
 qBraid API and leverage functions such as `get_devices()` and `get_jobs()`.
 
 ### Load Account from Environment Variables
 
 Alternatively, the qBraid-SDK can discover credentials from environment
 variables:
 
-```bash
-export JUPYTERHUB_USER='USER_EMAIL'
+```shell
 export QBRAID_API_KEY='QBRAID_API_KEY'
 ```
 
 Then instantiate the session without any arguments
 
 ```python
-from qbraid.api import QbraidSession
+from qbraid_core import QbraidSession
 
 session = QbraidSession()
 ```
 
 ## Launch on qBraid
 
 The "Launch on qBraid" button (below) can be added to any public GitHub
```

#### html2text {}

```diff
@@ -1,52 +1,7 @@
-Metadata-Version: 2.1 Name: qbraid Version: 0.5.3.dev20240312235736 Summary: A
-Python toolkit for cross-framework abstraction of quantum programs. Home-page:
-https://www.qbraid.com/ Author: qBraid Development Team Author-email:
-contact@qbraid.com License: GPL v3.0 Project-URL: Documentation, https://
-docs.qbraid.com/en/latest/ Project-URL: Bug Tracker, https://github.com/qBraid/
-qBraid/issues Project-URL: Source Code, https://github.com/qBraid/qBraid
-Project-URL: Discord, https://discord.gg/TPBU2sa8Et Project-URL: Launch on Lab,
-https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid.git
-Keywords: qbraid,quantum Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: Natural Language
-:: English Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: networkx<4.0,>=2.5 Requires-Dist: numpy<1.27,>=1.17
-Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0 Requires-Dist: ply>=3.6
-Requires-Dist: requests>=2.28.0 Provides-Extra: braket Requires-Dist: amazon-
-braket-sdk<1.74.0,>=1.42.1; extra == "braket" Provides-Extra: cirq Requires-
-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq" Provides-Extra: pennylane
-Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "pennylane" Provides-Extra:
-pytket Requires-Dist: pytket<1.26.0,>=1.16.0; extra == "pytket" Provides-Extra:
-pyquil Requires-Dist: pyquil<4.4.0,>=3.5.4; extra == "pyquil" Provides-Extra:
-qiskit Requires-Dist: qiskit<1.1.0,>=0.44.0; extra == "qiskit" Requires-Dist:
-qiskit-ibm-provider<0.11.0,>=0.5.3; extra == "qiskit" Requires-Dist: qiskit-
-ibm-runtime<0.21.0,>=0.18.0; extra == "qiskit" Provides-Extra: qasm3 Requires-
-Dist: qiskit-qasm3-import<0.5.0,>=0.2.0; extra == "qasm3" Provides-Extra: ionq
-Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "ionq" Requires-Dist: cirq-
-ionq<1.4.0,>=1.3.0; extra == "ionq" Requires-Dist: pytket-
-braket<0.35.0,>=0.30.0; extra == "ionq" Provides-Extra: all Requires-Dist:
-amazon-braket-sdk<1.74.0,>=1.42.1; extra == "all" Requires-Dist: cirq-
-core<1.4.0,>=1.3.0; extra == "all" Requires-Dist: cirq-ionq<1.4.0,>=1.3.0;
-extra == "all" Requires-Dist: pennylane<0.36.0,>=0.33.1; extra == "all"
-Requires-Dist: pytket<1.26.0,>=1.16.0; extra == "all" Requires-Dist: pytket-
-braket<0.35.0,>=0.30.0; extra == "all" Requires-Dist: pyquil<4.5.0,>=3.5.4;
-extra == "all" Requires-Dist: qiskit<1.1.0,>=0.44.0; extra == "all" Requires-
-Dist: qiskit-ibm-provider<0.11.0,>=0.5.3; extra == "all" Requires-Dist: qiskit-
-ibm-runtime<0.21.0,>=0.18.0; extra == "all" Requires-Dist: qiskit-qasm3-
-import<0.5.0,>=0.2.0; extra == "all" Provides-Extra: visualization Requires-
-Dist: ipython; extra == "visualization" Requires-Dist: matplotlib; extra ==
-"visualization" Requires-Dist: pylatexenc; extra == "visualization" Requires-
-Dist: qiskit[visualization]; extra == "visualization" Provides-Extra: docs
-Requires-Dist: sphinx~=7.2.6; extra == "docs" Requires-Dist: sphinx-autodoc-
-typehints<2.1,>=1.24; extra == "docs" Requires-Dist: sphinx-rtd-
-theme<2.1,>=1.3; extra == "docs" Requires-Dist: docutils<0.21; extra == "docs"
 [qbraid-sdk-header]
 _[_C_I_]_[_c_o_d_e_c_o_v_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]_[_D_i_s_c_o_r_d_]
 The qBraid-SDK is a Python toolkit for cross-framework abstraction,
 transpilation, and execution of quantum programs. [[https://qbraid-
 static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png]](https://
 account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git) ## Features
 - Unified quantum frontend interface. **Transpile** quantum circuits between
@@ -65,92 +20,95 @@
 latest/developerguide/braket-devices.html) with no additional access keys or
 API tokens required. See [qBraid Quantum Jobs](https://docs.qbraid.com/
 projects/lab/en/latest/lab/quantum_jobs.html) for more. ### Local install The
 qBraid-SDK, and all of its dependencies, can also be installed using pip:
 ```bash pip install qbraid ``` You can also [install from source]
 (CONTRIBUTING.md#installing-from-source) by cloning this repository and running
 a pip install command in the root directory of the repository: ```bash git
-clone https://github.com/qBraid/qBraid.git cd qBraid pip install -e '.[all]'
-``` *Note*: The qBraid-SDK requires Python 3.9 or greater. If using locally,
-follow linked instructions to configure your [qBraid](#local-account-setup),
-[AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-
-credentials), and [IBMQ](https://github.com/Qiskit/qiskit-ibm-
-provider#provider-setup) credentials. ### Check version You can view the
-version of the qBraid-SDK you have installed within Python using the following:
-```python In [1]: import qbraid In [2]: qbraid.__version__ ``` ## Documentation
-& Tutorials qBraid documentation is available at [docs.qbraid.com](https://
-docs.qbraid.com/en/stable/). See also: - [API Reference](https://
-docs.qbraid.com/en/stable/api/qbraid.html) - [User Guide](https://
-docs.qbraid.com/en/stable/sdk/overview.html) - [Example Notebooks](https://
-github.com/qBraid/qbraid-lab-demo) ## Quickstart ### Transpiler Construct a
-quantum program of any supported program type. Below, `SUPPORTED_QPROGRAMS`
-maps shorthand identifiers for supported quantum programs, each corresponding
-to a type in the typed `QPROGRAM` Union. For example, 'qiskit' maps to
-`qiskit.QuantumCircuit` in `QPROGRAM`. Notably, 'qasm2' and 'qasm3' both
-represent raw OpenQASM strings. This arrangement simplifies targeting and
-transpiling between different quantum programming frameworks. ```python >>>
-from qbraid import SUPPORTED_QPROGRAMS >>> SUPPORTED_QPROGRAMS {'cirq':
+clone https://github.com/qBraid/qBraid.git cd qBraid pip install . ``` *Note*:
+The qBraid-SDK requires Python 3.9 or greater. If using locally, follow linked
+instructions to configure your [qBraid](#local-account-setup), [AWS](https://
+github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-credentials),
+and [IBMQ](https://github.com/Qiskit/qiskit-ibm-provider#provider-setup)
+credentials. ### Check version You can view the version of the qBraid-SDK you
+have installed within Python using the following: ```python In [1]: import
+qbraid In [2]: qbraid.__version__ ``` ## Documentation & Tutorials qBraid
+documentation is available at [docs.qbraid.com](https://docs.qbraid.com/en/
+stable/). See also: - [API Reference](https://docs.qbraid.com/en/stable/api/
+qbraid.html) - [User Guide](https://docs.qbraid.com/en/stable/sdk/
+overview.html) - [Example Notebooks](https://github.com/qBraid/qbraid-lab-demo)
+## Quickstart ### Transpiler Construct a quantum program of any supported
+program type. Below, `SUPPORTED_QPROGRAMS` maps shorthand identifiers for
+supported quantum programs, each corresponding to a type in the typed
+`QPROGRAM` Union. For example, 'qiskit' maps to `qiskit.QuantumCircuit` in
+`QPROGRAM`. Notably, 'qasm2' and 'qasm3' both represent raw OpenQASM strings.
+This arrangement simplifies targeting and transpiling between different quantum
+programming frameworks. ```python >>> from qbraid.programs import
+SUPPORTED_QPROGRAMS >>> SUPPORTED_QPROGRAMS {'cirq':
 'cirq.circuits.circuit.Circuit', 'qiskit':
 'qiskit.circuit.quantumcircuit.QuantumCircuit', 'pyquil':
 'pyquil.quil.Program', 'pytket': 'pytket._tket.circuit.Circuit', 'braket':
 'braket.circuits.circuit.Circuit', 'openqasm3': 'openqasm3.ast.Program',
 'qasm2': 'str', 'qasm3': 'str'} ``` Pass any quantum program of type
-`qbraid.QPROGRAM` to the `circuit_wrapper()` and specify a target package from
-`SUPPORTED_QPROGRAMS` to "transpile" your circuit to a new program type:
-```python >>> from qbraid import circuit_wrapper >>> from qbraid.interface
-import random_circuit >>> qiskit_circuit = random_circuit("qiskit") >>>
-cirq_circuit = circuit_wrapper(qiskit_circuit).transpile("cirq") >>> print
+`qbraid.programs.QPROGRAM` to the `load_program()` and specify a target package
+from `SUPPORTED_QPROGRAMS` to "transpile" your circuit to a new program type:
+```python >>> from qbraid.interface import random_circuit >>> from
+qbraid.transpiler import transpile >>> qiskit_circuit = random_circuit
+("qiskit") >>> cirq_circuit = transpile(qiskit_circuit, "cirq") >>> print
 (qiskit_circuit) ââââââââââââââ q_0:
 âââ âââ¤ Rx(3.0353) â
 âââ´âââââââ¬âââââ¬ââââ q_1: â¤ H
 ââââââ¤ âX âââââ âââââ ââââââ >>>
 print(cirq_circuit) 0: âââ@âââRx(0.966Ï)âââ â 1:
 âââHâââX^0.5ââââââââ ``` The same functionality can
-be achieved using the underlying `convert_to_package()` function directly:
-```python >>> from qbraid import convert_to_package >>> cirq_circuit =
-convert_to_package(qiskit_circuit, "cirq") ``` Behind the scenes, the qBraid-
-SDK uses ``networkx`` to create a directional graph that maps all possible
-conversions between supported program types: ```python from qbraid.transpiler
-import ConversionGraph from qbraid.visualization import plot_conversion_graph
-graph = ConversionGraph() plot_conversion_graph(graph) ```
-[conversion_graph]You can use the native conversions supported by qBraid, or
-define your own custom nodes and/or edges. See [example](https://github.com/
-qBraid/qbraid-lab-demo/blob/main/qbraid_sdk/
-qbraid_sdk_transpiler_braket_qiskit.ipynb). ### Devices & Jobs Search for
-quantum backend(s) on which to execute your program. ```python >>> from qbraid
-import get_devices >>> get_devices() Device status updated 0 minutes ago Device
-ID Status --------- ------ aws_oqc_lucy ONLINE aws_ionq_aria2 OFFLINE
-aws_rigetti_aspen_m3 ONLINE ibm_q_brisbane ONLINE ... ``` Apply the
-`device_wrapper()`, and send quantum jobs to any supported backend, from any
-supported program type: ```python >>> from qbraid import device_wrapper,
-get_jobs >>> aws_device = device_wrapper("aws_oqc_lucy") >>> ibm_device =
-device_wrapper("ibm_q_brisbane") >>> aws_job = aws_device.run(qiskit_circuit,
-shots=1000) >>> ibm_job = ibm_device.run(cirq_circuit, shots=1000) >>> get_jobs
-() Displaying 2 most recent jobs: Job ID Submitted Status ------ --------- ----
--- aws_oqc_lucy-exampleuser-qjob-zzzzzzz... 2023-05-21T21:13:47.220Z QUEUED
-ibm_q_brisbane-exampleuser-qjob-xxxxxxx... 2023-05-21T21:13:48.220Z RUNNING ...
-``` Compare results in a consistent, unified format: ```python >>> aws_result =
-aws_job.result() >>> ibm_result = ibm_job.result() >>>
-aws_result.measurement_counts() {'00': 483, '01': 14, '10': 486, '11': 17} >>>
-ibm_result.measurement_counts() {'00': 496, '01': 12, '10': 479, '11': 13} ```
-## Local account setup [api_key]To use the qBraid-SDK locally (outside of
-qBraid Lab), you must add your account credentials: 1. Create a qBraid account
-or log in to your existing account by visiting [account.qbraid.com](https://
-account.qbraid.com/) 2. Copy your API Key token from the left side of your
-[account page](https://account.qbraid.com/): 3. Save your API key from step 2
-by calling `QbraidSession.save_config()`: ```python from qbraid.api import
-QbraidSession session = QbraidSession(api_key='API_KEY') session.save_config()
-``` The command above stores your credentials locally in a configuration file
-`~/.qbraid/qbraidrc`, where `~` corresponds to your home (`$HOME`) directory.
-Once saved, you can then connect to the qBraid API and leverage functions such
-as `get_devices()` and `get_jobs()`. ### Load Account from Environment
-Variables Alternatively, the qBraid-SDK can discover credentials from
-environment variables: ```bash export JUPYTERHUB_USER='USER_EMAIL' export
+be achieved using the underlying `transpile()` function directly: ```python >>>
+from qbraid.transpiler import transpile >>> cirq_circuit = transpile
+(qiskit_circuit, "cirq") ``` Behind the scenes, the qBraid-SDK uses
+``networkx`` to create a directional graph that maps all possible conversions
+between supported program types: ```python from qbraid.transpiler import
+ConversionGraph from qbraid.visualization import plot_conversion_graph graph =
+ConversionGraph() plot_conversion_graph(graph) ``` [conversion_graph]You can
+use the native conversions supported by qBraid, or define your own custom nodes
+and/or edges. See [example](https://github.com/qBraid/qbraid-lab-demo/blob/
+main/qbraid_sdk/qbraid_sdk_transpiler_braket_qiskit.ipynb). ### Devices & Jobs
+Search for quantum backend(s) on which to execute your program. ```python >>>
+from qbraid import get_devices >>> get_devices() Device status updated 0
+minutes ago Device ID Status --------- ------ aws_oqc_lucy ONLINE
+aws_ionq_aria2 OFFLINE aws_rigetti_aspen_m3 ONLINE ibm_q_brisbane ONLINE ...
+``` You can get a Python list of device objects using: ```python from
+qbraid.providers import QbraidProvider provider = QbraidProvider() qdevices =
+provider.get_devices() ``` Or, instantiate a known device by ID via the
+`QbraidProvider.get_device()` method, and submit quantum jobs from any
+supported program type: ```python >>> from qbraid import get_jobs >>> from
+qbraid.providers import QbraidProvider >>> provider = QbraidProvider() >>>
+aws_device = provider.get_device("aws_oqc_lucy") >>> ibm_device =
+provider.get_device("ibm_q_brisbane") >>> aws_job = aws_device.run
+(qiskit_circuit, shots=1000) >>> ibm_job = ibm_device.run(cirq_circuit,
+shots=1000) >>> get_jobs() Displaying 2 most recent jobs: Job ID Submitted
+Status ------ --------- ------ aws_oqc_lucy-exampleuser-qjob-zzzzzzz... 2023-
+05-21T21:13:47.220Z QUEUED ibm_q_brisbane-exampleuser-qjob-xxxxxxx... 2023-05-
+21T21:13:48.220Z RUNNING ... ``` Compare results in a consistent, unified
+format: ```python >>> aws_result = aws_job.result() >>> ibm_result =
+ibm_job.result() >>> aws_result.measurement_counts() {'00': 483, '01': 14,
+'10': 486, '11': 17} >>> ibm_result.measurement_counts() {'00': 496, '01': 12,
+'10': 479, '11': 13} ``` ## Local account setup [api_key]To use the qBraid-SDK
+locally (outside of qBraid Lab), you must add your account credentials: 1.
+Create a qBraid account or log in to your existing account by visiting
+[account.qbraid.com](https://account.qbraid.com/) 2. Copy your API Key token
+from the left side of your [account page](https://account.qbraid.com/): 3. Save
+your API key from step 2 by calling `QbraidSession.save_config()`: ```python
+from qbraid_core import QbraidSession session = QbraidSession
+(api_key='API_KEY') session.save_config() ``` The command above stores your
+credentials locally in a configuration file `~/.qbraid/qbraidrc`, where `~`
+corresponds to your home (`$HOME`) directory. Once saved, you can then connect
+to the qBraid API and leverage functions such as `get_devices()` and `get_jobs
+()`. ### Load Account from Environment Variables Alternatively, the qBraid-SDK
+can discover credentials from environment variables: ```shell export
 QBRAID_API_KEY='QBRAID_API_KEY' ``` Then instantiate the session without any
-arguments ```python from qbraid.api import QbraidSession session =
+arguments ```python from qbraid_core import QbraidSession session =
 QbraidSession() ``` ## Launch on qBraid The "Launch on qBraid" button (below)
 can be added to any public GitHub repository. Clicking on it automaically opens
 qBraid Lab, and performs a `git clone` of the project repo into your account's
 home directory. Copy the code below, and replace `YOUR-USERNAME` and `YOUR-
 REPOSITORY` with your GitHub info. [[https://qbraid-static.s3.amazonaws.com/
 logos/Launch_on_qBraid_white.png]](https://account.qbraid.com?gitHubUrl=https:/
 /github.com/qBraid/qBraid.git) Use the badge in your project's `README.md`:
```

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/cards/jupyter.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/cards/python.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/cards/terminal.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/favicon.ico` & `qbraid-0.6.0.dev20240404040745/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/logo.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/braket.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/cirq.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/pennylane.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/pennylane.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/qasm.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qasm.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/qir.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/pkg-logos/quantinuum.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/pkg-logos/quantinuum.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/batch_counts.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/batch_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/conversion_graph.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/conversion_graph.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/get_devices.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/hub_spokes.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/hub_spokes.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/lab_jobs.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/lab_jobs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.6.0.dev20240404040745/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/docs/conf.py` & `qbraid-0.6.0.dev20240404040745/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
 import qbraid
 
+# Set an environment variable to detect whether we are building the docs
+# so that we know to use raw imports instead of lazy loading.
+# os.environ['SPHINX_BUILD'] = '1'
+
+
 sys.path.insert(0, os.path.abspath(".."))
 sys.path.insert(0, os.path.abspath("../../qbraid"))
 
 # -- Project information -----------------------------------------------------
 
 project = "qBraid"
-copyright = "2023, qBraid Development Team"
+copyright = "2024, qBraid Development Team"
 author = "qBraid Development Team"
 
 # The full version, including alpha/beta/rc tags
 release = qbraid.__version__
 
 # -- General configuration ---------------------------------------------------
 
@@ -42,15 +47,15 @@
     "sphinx.ext.coverage",
     "sphinx.ext.viewcode",
 ]
 
 # set_type_checking_flag = True
 autodoc_member_order = "bysource"
 autoclass_content = "both"
-autodoc_mock_imports = ["cirq", "qiskit", "braket", "numpy", "requests", "requests.Session", "matplotlib", "matplotlib.pyplot"]
+autodoc_mock_imports = ["cirq", "braket", "qiskit", "pennylane", "pyquil", "pytket", "openqasm3", "numpy", "matplotlib", "matplotlib.pyplot"]
 napoleon_numpy_docstring = False
 todo_include_todos = True
 mathjax_path = "https://cdn.jsdelivr.net/npm/mathjax@2/MathJax.js?config=TeX-AMS-MML_HTMLorMML"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
```

### Comparing `qbraid-0.5.3.dev20240312235736/docs/index.rst` & `qbraid-0.6.0.dev20240404040745/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 
 .. toctree::
    :maxdepth: 1
    :caption: SDK API Reference
    :hidden:
 
    api/qbraid
-   api/qbraid.api
    api/qbraid.programs
    api/qbraid.interface
    api/qbraid.transpiler
    api/qbraid.compiler
    api/qbraid.providers
    api/qbraid.visualization
```

#### html2text {}

```diff
@@ -6,11 +6,10 @@
 _**_**_**_**_ _CC_LL_II_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 _**_**_**_**_ _SS_DD_KK_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 | .. toctree:: :maxdepth: 1 :caption: SDK User Guide :hidden: sdk/overview sdk/
 programs sdk/transpiler sdk/providers sdk/devices sdk/jobs sdk/results ..
 toctree:: :maxdepth: 1 :caption: SDK API Reference :hidden: api/qbraid api/
-qbraid.api api/qbraid.programs api/qbraid.interface api/qbraid.transpiler api/
-qbraid.compiler api/qbraid.providers api/qbraid.visualization .. Indices and
-Tables .. ------------------ .. * :ref:`genindex` .. * :ref:`modindex` .. * :
-ref:`search`
+qbraid.programs api/qbraid.interface api/qbraid.transpiler api/qbraid.compiler
+api/qbraid.providers api/qbraid.visualization .. Indices and Tables .. --------
+---------- .. * :ref:`genindex` .. * :ref:`modindex` .. * :ref:`search`
```

### Comparing `qbraid-0.5.3.dev20240312235736/docs/sdk/devices.rst` & `qbraid-0.6.0.dev20240404040745/docs/sdk/devices.rst`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,20 @@
 ----------------
 
 Given a ``qbraid_id`` retrieved from ``get_devices``, a ``qbraid.providers.QuantumDevice``
 object can be created as follows:
 
 .. code-block:: python
 
-    from qbraid import device_wrapper
+    from qbraid.providers import QbraidProvider
 
+    provider = QbraidProvider()
     qbraid_id = 'aws_oqc_lucy'  # as an example
 
-    qdevice = device_wrapper(qbraid_id)
+    qdevice = provider.get_device(qbraid_id)
 
 
 From here, class methods are available to get information about the device,
 execute quantum programs (to be covered in the next section), access the
 wrapped device object directly, and more.
 
 .. code-block:: python
@@ -186,15 +187,15 @@
 ``ibm_least_busy_qpu`` function to get the ``qbraid_id`` of the IBMQ QPU with the
 least number of queued quantum jobs.
 
 .. code-block:: python
 
     >>> from qbraid.providers.ibm import ibm_least_busy_qpu
     >>> qbraid_id = ibm_least_busy_qpu()
-    >>> qdevice = device_wrapper(qbraid_id)
+    >>> qdevice = provider.get_device(qbraid_id)
     >>> qdevice.name
     'Nairobi'
     >>> qdevice.status()
     <DeviceStatus.ONLINE: 0>
 
 After applying the device wrapper and verifying the device is online, we're ready
 to submit a job. This time, we'll use a Cirq circuit as the ``run`` method input.
@@ -215,14 +216,14 @@
 qubits supported by the backend. We then checked the backend's number of pending jobs,
 and saw the number increase by one after submitting our job.
 
 Summary
 --------
 
 The device layer of the qBraid SDK enables users to execute quantum circuits of
-any ``qbraid.QPROGRAM_TYPES`` on any simulator or QPU returned by
+any ``qbraid.programs.QPROGRAM_TYPES`` on any simulator or QPU returned by
 ``qbraid.get_devices``. Filter your search to the specifications of your task,
 identify a device, and execute your program through a consistent three-step protocol:
 
 1. Get qbraid device ID
 2. Apply device wrapper
 3. Execute program via ``run`` method
```

### Comparing `qbraid-0.5.3.dev20240312235736/docs/sdk/jobs.rst` & `qbraid-0.6.0.dev20240404040745/docs/sdk/jobs.rst`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 The `device module <./devices.html>`_ illustrated how qBraid device wrappers can
 be used execute circuits on quantum backends. Using the OQC Lucy QPU as our example
 target backend, the procedure was as follows:
 
 .. code-block:: python
 
-    >>> from qbraid import device_wrapper
+    >>> from qbraid.providers import QbraidProvider
     >>> qbraid_id = 'aws_oqc_lucy'
-    >>> qdevice = device_wrapper(qbraid_id)
+    >>> provider = QbraidProvider()
+    >>> qdevice = provider.get_device(qbraid_id)
     >>> qjob = qdevice.run(circuit)
     >>> type(qjob)
     qbraid.providers.aws.job.BraketQuantumTaskWrapper
 
 Invoking the ``run`` method of a qBraid ``QuantumDevice`` returns a qBraid
 ``QuantumJob``. Through a unified set of methods and attributes, this class
 provides access to data about the quantum jobs executed across any qBraid supported
@@ -52,24 +53,24 @@
 Batch Jobs
 ------------
 
 For AWS devices, ``run_batch`` will create a list of quantum job objects:
 
 .. code-block:: python
 
-    >>> aws_device = device_wrapper('aws_ionq_harmony')
+    >>> aws_device = provider.get_device('aws_ionq_harmony')
     >>> batch_jobs = aws_device.run_batch([circuit1, circuit2, circuit3], shots=1000)
     >>> batch_results = [job.result() for job in batch_jobs]
 
 
 For IBM devices, ``run_batch`` will create a single object that contains all batch jobs:
 
 .. code-block:: python
 
-    >>> ibm_device = device_wrapper('ibm_q_kyoto')
+    >>> ibm_device = provider.get_device('ibm_q_kyoto')
     >>> batch_job = ibm_device.run_batch([circuit1, circuit2, circuit3], shots=1000)
     >>> batch_result = batch_job.result()
 
 
 Retrieve Jobs
 --------------
 
@@ -94,17 +95,17 @@
 
 
 This job ID can be used to reinstantiate a qBraid ``QuantumJob`` object at any
 time, and even in a seperate program, with no loss of information.
 
 .. code-block:: python
 
-    >>> from qbraid import job_wrapper
+    >>> from qbraid.providers import QuantumJob
     >>> saved_job_id = 'aws_oqc_lucy-exampleuser-qjob-xxxxxxxxxxxxxxxxxxxx'
-    >>> qjob = job_wrapper(saved_job_id)
+    >>> qjob = QuantumJob.retrieve(saved_job_id)
 
 
 You can also load a previously submitted jobs directly through the corresponding provider class:
 
 .. code-block:: python
 
     >>> from qbraid.providers.aws import BraketQuantumTask
```

### Comparing `qbraid-0.5.3.dev20240312235736/docs/sdk/overview.rst` & `qbraid-0.6.0.dev20240404040745/docs/sdk/overview.rst`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Usage
 ------
 
 Construct a quantum program of any supported program type:
 
 .. code-block:: python
    
-   >>> from qbraid import QPROGRAM_LIBS
+   >>> from qbraid.programs import QPROGRAM_LIBS
    >>> from qbraid.interface import random_circuit
    >>> QPROGRAM_LIBS
    ['cirq', 'qiskit', 'pyquil', 'pytket', 'braket', 'openqasm3', 'qasm2', 'qasm3']
    >>> circuit = random_circuit("qiskit", num_qubits=1, measure=True)
 
 Search for quantum backend(s) on which to execute your program:
 
@@ -80,23 +80,24 @@
    aws_oqc_lucy                        ONLINE        
    aws_ionq_aria2                      OFFLINE
    aws_rigetti_aspen_m3                ONLINE
    
    >>> ibm_least_busy_qpu()
    ibm_q_oslo
 
-Apply the device wrapper and send your quantum jobs:
+Select a device using the ``QbraidProvider`` and send your quantum jobs:
 
 .. code-block:: python
 
-   >>> from qbraid import device_wrapper
+   >>> from qbraid.providers import QbraidProvider
+   >>> provider = QbraidProvider()
    >>> jobs  = []
    >>> qbraid_ids = ['aws_oqc_lucy', 'ibm_q_oslo']
    >>> for device in qbraid_ids:
-   ... qdevice = device_wrapper(device)
+   ... qdevice = provider.get_device(device)
    ... qjob = qdevice.run(circuit, shots=1000)
    ... jobs.append(qjob)
 
 List your submitted jobs and view their status:
 
 .. code-block:: python
```

### Comparing `qbraid-0.5.3.dev20240312235736/docs/sdk/programs.rst` & `qbraid-0.6.0.dev20240404040745/docs/sdk/programs.rst`

 * *Files 4% similar despite different names*

```diff
@@ -66,17 +66,17 @@
               └───┘
 
 
 Next, we'll apply the qbraid circuit wrapper.
 
 .. code-block:: python
 
-    from qbraid import circuit_wrapper
+    from qbraid.programs import load_program
 
-    qprogram = circuit_wrapper(qiskit_circuit)
+    qprogram = load_program(qiskit_circuit)
 
 
 Each circuit wrapper object has ``num_qubits`` and ``depth`` attributes, regardless of the input circuit type.
 The underlying "wrapped" circuit can be accessed using the circuit wrapper's ``program`` attribute.
 
 .. code-block:: python
 
@@ -88,15 +88,15 @@
     qiskit.circuit.quantumcircuit.QuantumCircuit
 
 
 Transpiler
 -----------
 
 Now, we can use the ``qbraid.programs.QuantumProgram.transpile`` method to convert to wrapped circuit into
-any other supported program type. Simply pass in the name of the target package from one of ``qbraid.QPROGRAM_LIBS``.
+any other supported program type. Simply pass in the name of the target package from one of ``qbraid.programs.QPROGRAM_LIBS``.
 For example, use input "braket" to return a ``braket.circuits.Circuit``:
 
 .. code-block:: python
 
     >>> braket_circuit = qprogram.transpile("braket")
     >>> print(braket_circuit)
     T  : |0|1|
@@ -122,24 +122,24 @@
 ----------------------
 
 The ``unitary`` method will calculate the matrix representation of an input circuit of any
 supported program type.
 
 .. code-block:: python
 
-    >>> from qbraid import circuit_wrapper
-    >>> cirq_unitary = circuit_wrapper(cirq_circuit).unitary()
+    >>> from qbraid.programs import load_program
+    >>> cirq_unitary = load_program(cirq_circuit).unitary()
     >>> cirq_unitary.shape
     (16, 16)
 
 We can now apply the circuit wrapper to the random Cirq circuit above, and use the transpiler to return the equivalent ``pyquil.Program``:
 
 .. code-block:: python
     
-    >>> pyquil_circuit = circuit_wrapper(cirq_circuit).transpile("pyquil")
+    >>> pyquil_circuit = load_program(cirq_circuit).transpile("pyquil")
     >>> print(pyquil_circuit)
     ISWAP 0 3
     Z 1
     CNOT 0 2
     CZ 3 1
     CZ 2 3
     H 0
@@ -203,28 +203,28 @@
 From here, we can use ``remove_idle_qubits`` to map the circuit to the ``[0,1,2]`` convention.
 If the use-case requires using the dimensionality of the maximally indexed qubit, you
 can use ``populate_idle_qubits`` to append identity gates to "vacant" registers instead of
 performing the qubit mapping.
 
 .. code-block:: python
 
-    >>> from qbraid import circuit_wrapper
-    >>> qprogram = circuit_wrapper(braket_circuit)
+    >>> from qbraid.programs import load_program
+    >>> qprogram = load_program(braket_circuit)
     >>> qprogram.remove_idle_qubits()
     >>> print(qprogram.program)
     T  : |0|1|2|
             
     q0 : -H-C---
             |   
     q1 : ---X-C-
               | 
     q2 : -----X-
 
     T  : |0|1|2|
-    >>> qprogram1 = circuit_wrapper(braket_circuit)
+    >>> qprogram1 = load_program(braket_circuit)
     >>> qprogram1.populate_idle_qubits()
     >>> print(qprogram1.program)
     T  : |0|1|2|
             
     q0 : -H-C---
             |   
     q1 : -I-|---
```

### Comparing `qbraid-0.5.3.dev20240312235736/docs/sdk/results.rst` & `qbraid-0.6.0.dev20240404040745/docs/sdk/results.rst`

 * *Files 14% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 
 This time, we'll run our quantum program on the IBMQ Nairobi QPU. After the
 job has completed, we'll gather the result, print the measurement counts,
 and plot a histogram of the probabilities.
 
 .. code-block:: python
 
-    from qbraid import device_wrapper
+    from qbraid.providers import QbraidProvider
     from qbraid.visualization import plot_histogram
 
     shots = 2**10
     
-    qdevice = device_wrapper('ibm_q_nairobi')
+    provider = QbraidProvider()
+    qdevice = provider.get_device('ibm_q_nairobi')
     qjob = ibmq_device.run(circuit, shots=shots)
     qjob.wait_for_final_state()
     
     qresult_ibmq = qjob.result()
     qresult_ibmq.measurement_counts()
     # {'0': 136, '1': 864}
 
@@ -57,15 +58,15 @@
 
 
 Now, let's run a batch job using two copies of the one-qubit qiskit circuit
 on a density-matrix simulator provided AWS:
 
 .. code-block:: python
 
-    aws_device = device_wrapper('aws_dm_sim')
+    aws_device = provider.get_device('aws_dm_sim')
 
     batch_jobs = aws_device.run_batch([circuit, circuit], shots=shots)
 
     batch_results = [job.result() for job in batch_jobs]
 
     batch_counts = [result.measurement_counts() for result in batch_results]
```

### Comparing `qbraid-0.5.3.dev20240312235736/docs/sdk/transpiler.rst` & `qbraid-0.6.0.dev20240404040745/docs/sdk/transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/_about.py` & `qbraid-0.6.0.dev20240404040745/qbraid/_about.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,48 +5,51 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """Information about qBraid and dependencies."""
-import platform
-
-from networkx import __version__ as networkx_version
-from numpy import __version__ as numpy_version
-from openqasm3 import __version__ as openqasm3_version
-from ply import __version__ as ply_version
-from requests import __version__ as requests_version
-
-from ._version import __version__ as qbraid_version
 
 
 def about() -> None:
     """Displays information about qBraid, core/optional packages, and Python
     version/platform information.
     """
+    # pylint: disable=import-outside-toplevel
+    import platform
+
+    from networkx import __version__ as networkx_version
+    from numpy import __version__ as numpy_version
+    from openqasm3 import __version__ as openqasm3_version
+    from ply import __version__ as ply_version
+    from qbraid_core._version import __version__ as qbraid_core_version
+
+    from ._version import __version__ as qbraid_version
+
     # Core dependencies
     core_dependencies = {
+        "qbraid_core": qbraid_core_version,
         "networkx": networkx_version,
         "openqasm3": openqasm3_version,
         "numpy": numpy_version,
-        "requests": requests_version,
         "ply": ply_version,
     }
 
     # Optional dependencies
     optional_packages = {
         "pyquil": "pyquil",
         "qiskit": "qiskit",
         "braket": "braket._sdk",
         "pennylane": "pennylane",
         "cirq": "cirq",
         "pytket": "pytket",
         "qiskit_ibm_provider": "qiskit_ibm_provider",
         "qiskit_ibm_runtime": "qiskit_ibm_runtime",
+        "qbraid_qir": "qbraid_qir",
     }
 
     optional_dependencies = {}
     for package_name, import_path in optional_packages.items():
         try:
             package = __import__(import_path, fromlist=[""])
             optional_dependencies[package_name] = package.__version__
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/_display.py` & `qbraid-0.6.0.dev20240404040745/qbraid/_display.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/_qdevice.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/_qprogram.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/api/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/compiler/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,39 +4,22 @@
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
-# pylint: skip-file
-
 """
-Module for interfacing with the qBraid API.
+Module for device-specific quantum program conversions
 
-.. currentmodule:: qbraid.api
+.. currentmodule:: qbraid.compiler
 
 Exceptions
-------------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-   ApiError
-   AuthError
-   ConfigError
-   RequestsApiError
-
-
-Classes
---------
+-----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   QbraidSession
-   PostForcelistRetry
+   CompilerError
 
 """
-from .exceptions import ApiError, AuthError, ConfigError, RequestsApiError
-from .retry import PostForcelistRetry
-from .session import QbraidSession
+from .exceptions import CompilerError
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/api/exceptions.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,27 +5,37 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for exceptions raised while interacting with the qbraid API.
+Module defining exceptions for errors raised by qBraid.
 
 """
+
 from qbraid.exceptions import QbraidError
 
+from ._import import QPROGRAM_LIBS
+
 
-class ApiError(QbraidError):
-    """Base class for errors raised in the :mod:`qbraid.api` module"""
+class PackageValueError(QbraidError):
+    """Class for errors raised due to unsupported quantum frontend package"""
 
+    def __init__(self, package):
+        msg = (
+            f"Quantum frontend module '{package}' is not supported.\n"
+            f"Frontends supported by qBraid are: {QPROGRAM_LIBS}"
+        )
+        super().__init__(msg)
 
-class AuthError(ApiError):
-    """Base class for errors raised authorizing user"""
 
+class ProgramTypeError(QbraidError):
+    """Class for errors raised when processing unsupported quantum programs"""
 
-class ConfigError(ApiError):
-    """Base class for errors raised while setting a user configuartion"""
+    def __init__(self, program):
+        msg = f"Quantum program of type '{type(program)}' is not supported."
+        super().__init__(msg)
 
 
-class RequestsApiError(ApiError):
-    """Exception re-raising a RequestException."""
+class QasmError(QbraidError):
+    """For errors raised while processing OpenQASM programs."""
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/compiler/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/compiler/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,16 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for device-specific quantum program conversions
+Module defining exceptions for errors raised by the qBraid compiler.
 
-.. currentmodule:: qbraid.compiler
-
-Exceptions
------------
+"""
 
-.. autosummary::
-   :toctree: ../stubs/
+from qbraid.exceptions import QbraidError
 
-   CompilerError
 
-"""
-from .exceptions import CompilerError
+class CompilerError(QbraidError):
+    """Base class for errors raised by the qBraid compiler."""
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/compiler/braket/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/compiler/braket/ionq.py` & `qbraid-0.6.0.dev20240404040745/qbraid/compiler/braket/ionq.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,27 +25,27 @@
     try:
         # pytket >1.18,<1.22
         from pytket.circuit_library import _TK1_to_RzRx as TK1_to_RzRx  # type: ignore
     except (ModuleNotFoundError, ImportError):
         # pytket <= 1.18
         from pytket._tket.circuit._library import _TK1_to_RzRx as TK1_to_RzRx  # type: ignore
 
-
 from pytket.passes import RebaseCustom
 from pytket.predicates import (
     CompilationUnit,
     GateSetPredicate,
     MaxNQubitsPredicate,
     NoClassicalControlPredicate,
     NoFastFeedforwardPredicate,
     NoMidMeasurePredicate,
     NoSymbolsPredicate,
 )
 
 from qbraid.compiler.exceptions import CompilerError
+from qbraid.transpiler import transpile
 
 HARMONY_MAX_QUBITS = 11
 
 ionq_gates = {
     pytket.circuit.OpType.X,
     pytket.circuit.OpType.Y,
     pytket.circuit.OpType.Z,
@@ -117,17 +117,15 @@
         - Otherwise, the circuit is transpiled using ``pytket-braket``'s ``braket_to_tk``.
 
     """
     if isinstance(circuit, Circuit):
         try:
             tk_circuit = pytket.extensions.braket.braket_convert.braket_to_tk(circuit)
         except NotImplementedError:
-            from qbraid import circuit_wrapper  # pylint: disable=import-outside-toplevel
-
-            tk_circuit = circuit_wrapper(circuit).transpile("pytket")
+            tk_circuit = transpile(circuit, "pytket")
     else:
         tk_circuit = circuit
 
     cu = CompilationUnit(tk_circuit, preds)
     ionq_rebase_pass.apply(cu)
     if not cu.check_all_predicates():
         raise CompilerError("Circuit cannot be compiled to IonQ Harmony.")
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/compiler/exceptions.py` & `qbraid-0.6.0.dev20240404040745/qbraid/visualization/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
-
 """
-Module defining exceptions for errors raised by the qBraid compiler.
+Module for exceptions raised by visualization tools.
 
 """
-
 from qbraid.exceptions import QbraidError
 
 
-class CompilerError(QbraidError):
-    """Base class for errors raised by the qBraid compiler."""
+class VisualizationError(QbraidError):
+    """Class for errors raised when using visualization features."""
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/exceptions.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,39 +5,54 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module defining exceptions for errors raised by qBraid.
+Module containing quantum circuit wrapper classes providing uniform
+suite of methods and functionality for supported program types.
 
-"""
+.. currentmodule:: qbraid.programs
+
+.. _programs_data_type:
 
-from ._qprogram import QPROGRAM_LIBS
+Data Types
+-----------
 
+.. autodata:: QPROGRAM
+   :annotation: = Type alias defining all supported quantum circuit / program types
 
-class QbraidError(Exception):
-    """Base class for errors raised by qBraid."""
+Functions
+----------
 
+.. autosummary::
+   :toctree: ../stubs/
 
-class PackageValueError(QbraidError):
-    """Class for errors raised due to unsupported quantum frontend package"""
+   get_qasm_version
+   get_program_type
+   load_program
 
-    def __init__(self, package):
-        msg = (
-            f"Quantum frontend module '{package}' is not supported.\n"
-            f"Frontends supported by qBraid are: {QPROGRAM_LIBS}"
-        )
-        super().__init__(msg)
+Classes
+--------
 
+.. autosummary::
+   :toctree: ../stubs/
 
-class ProgramTypeError(QbraidError):
-    """Class for errors raised when processing unsupported quantum programs"""
+   QuantumProgram
 
-    def __init__(self, program):
-        msg = f"Quantum program of type '{type(program)}' is not supported."
-        super().__init__(msg)
+Exceptions
+-----------
 
+.. autosummary::
+   :toctree: ../stubs/
 
-class QasmError(QbraidError):
-    """For errors raised while processing OpenQASM programs."""
+   PackageValueError
+   ProgramTypeError
+   QasmError
+
+"""
+from ._import import QPROGRAM, QPROGRAM_LIBS, QPROGRAM_TYPES, SUPPORTED_QPROGRAMS
+from .abc_program import QuantumProgram
+from .exceptions import PackageValueError, ProgramTypeError, QasmError
+from .inspector import get_program_type, get_qasm_version
+from .loader import load_program
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/get_devices.py` & `qbraid-0.6.0.dev20240404040745/qbraid/get_devices.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,47 +11,49 @@
 # pylint: disable=consider-using-f-string
 
 """
 Module to retrieve, update, and display information about devices
 supported by the qBraid SDK.
 
 """
-
-from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+from qbraid_core import QbraidSession
+from qbraid_core.services.quantum import QuantumClient, process_device_data
+
 try:
     from IPython.display import HTML, clear_output, display
 except ImportError:
     pass
 
 from ._display import running_in_jupyter, update_progress_bar
-from .api import QbraidSession
-from .load_provider import device_wrapper
 
 if TYPE_CHECKING:
     from IPython.display import DisplayHandle
 
 
 def refresh_devices() -> None:
     """Refreshes status for all qbraid supported devices. Requires credential for each vendor."""
+    # pylint: disable-next=import-outside-toplevel
+    from qbraid.providers import QbraidProvider
 
-    session = QbraidSession()
-    devices = session.get("/public/lab/get-devices", params={}).json()
+    client = QuantumClient()
+    provider = QbraidProvider(client=client)
+    devices = client.search_devices()
     count = 0
     num_devices = len(devices)  # i.e. number of iterations
     for document in devices:
         progress = count / num_devices
         update_progress_bar(progress)
         if document["statusRefresh"] is not None:  # None => internally not available at moment
             qbraid_id = document["qbraid_id"]
             try:
-                device = device_wrapper(qbraid_id)
+                device = provider.get_device(qbraid_id)
                 status = device.status().name
-                session.put("/lab/update-device", data={"qbraid_id": qbraid_id, "status": status})
+                client.update_device(data={"qbraid_id": qbraid_id, "status": status})
             except Exception:  # pylint: disable=broad-except
                 pass
 
         count += 1
     update_progress_bar(1)
     print()
 
@@ -67,40 +69,15 @@
     if query.get("type") == "SIMULATOR":
         query["type"] = "Simulator"
 
     # get-devices must be a POST request with kwarg `json` (not `data`) to
     # encode the query. This is because certain queries contain regular
     # expressions which cannot be encoded in GET request `params`.
     devices = session.post("/public/lab/get-devices", json=query).json()
-
-    device_data = []
-    tot_dev = 0
-    min_lag = 1e7
-    for document in devices:
-        qbraid_id = document["qbraid_id"]
-        name = document["name"]
-        provider = document["provider"]
-        status_refresh = document["statusRefresh"]
-        timestamp = datetime.utcnow()
-        if status_refresh is not None:
-            format_datetime = str(status_refresh)[:10].split("-") + str(status_refresh)[
-                11:19
-            ].split(":")
-            format_datetime_int = [int(x) for x in format_datetime]
-            mk_datime = datetime(*format_datetime_int)
-            lag = (timestamp - mk_datime).seconds
-            min_lag = min(lag, min_lag)
-        status = document["status"]
-        tot_dev += 1
-        device_data.append([provider, name, qbraid_id, status])
-    if len(device_data) == 0:
-        return [], 0  # No results matching given criteria
-    device_data.sort()
-    lag_minutes, _ = divmod(min_lag, 60)
-    return device_data, int(lag_minutes)
+    return process_device_data(devices)
 
 
 def _display_basic(data: List[str], message: str) -> None:
     if len(data) == 0:
         print(message)
     else:
         print(f"{message}\n")
@@ -222,31 +199,13 @@
         filters: A dictionary containing any filters to be applied.
         refresh: If True, calls :func:`~qbraid.refresh_devices` before execution.
 
     """
     if refresh:
         refresh_devices()
     query = {} if filters is None else filters
-    device_data, lag = _get_device_data(query)
-
-    if len(device_data) == 0:
-        align = "center"
-        msg = "No results matching given criteria"
-    else:
-        align = "right"
-        hours, minutes = divmod(lag, 60)
-        min_10, _ = divmod(minutes, 10)
-        min_display = min_10 * 10
-        if hours > 0:
-            if minutes > 30:
-                msg = f"Device status updated {hours}.5 hours ago"
-            else:
-                hour_s = "hour" if hours == 1 else "hours"
-                msg = f"Device status updated {hours} {hour_s} ago"
-        else:
-            if minutes < 10:
-                min_display = minutes
-            msg = f"Device status updated {min_display} minutes ago"
+    device_data, msg = _get_device_data(query)
+    align = "center" if len(device_data) == 0 else "right"
 
     if running_in_jupyter():
         return _display_jupyter(device_data, msg, align=align)
     return _display_basic(device_data, msg)
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/get_jobs.py` & `qbraid-0.6.0.dev20240404040745/qbraid/get_jobs.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 try:
     from IPython.display import HTML, clear_output, display
 except ImportError:
     pass
 
-from ._display import running_in_jupyter, update_progress_bar
-from .api import QbraidSession
-from .load_provider import job_wrapper
+from qbraid_core import QbraidSession
+from qbraid_core.services.quantum.adapter import _job_status_msg
+
+from qbraid._display import running_in_jupyter, update_progress_bar
 
 
 def _display_jobs_basic(data, msg):
     if len(data) == 0:
         print(msg)
     else:
         headers = ["Job ID", "Submitted", "Status"]
@@ -98,15 +99,14 @@
     refresh: bool = False,
     session: Optional[QbraidSession] = None,
 ) -> Tuple[List[List[str]], str]:
     from qbraid.providers import QuantumJob  # pylint: disable=import-outside-toplevel
 
     session = QbraidSession() if not session else session
     jobs = session.post("/get-user-jobs", json=query).json()
-    max_results = query.pop("numResults", 10)
     count = 0
     num_jobs = len(jobs)
     job_data = []
     for document in jobs:
         count += 1
         progress = count / num_jobs
         if refresh:
@@ -121,35 +121,25 @@
         status = document.get("qbraidStatus", document.get("status", "UNKNOWN"))
         try:
             status_final = QuantumJob.status_final(status)
         except Exception:  # pylint: disable=broad-except
             status_final = True
         if refresh and not status_final:
             try:
-                qbraid_job = job_wrapper(job_id)
+                qbraid_job = QuantumJob.retrieve(job_id)
                 with warnings.catch_warnings():
                     warnings.simplefilter("ignore")
                     status_obj = qbraid_job.status()
                 status = status_obj.name
             except Exception:  # pylint: disable=broad-except
                 pass
         job_data.append([job_id, created_at, status])
 
-    if num_jobs == 0:  # Design choice whether to display anything here or not
-        if len(query) == 0:
-            msg = f"No jobs found for user {session.user_email}"
-        else:
-            msg = "No jobs found matching given criteria"
-    elif num_jobs < max_results:
-        msg = f"Displaying {num_jobs}/{num_jobs} jobs matching query"
-    elif len(query) > 0:
-        s = "s" if num_jobs > 1 else ""
-        msg = f"Displaying {num_jobs} most recent job{s} matching query"
-    else:
-        msg = f"Displaying {num_jobs} most recent jobs"
+    msg = _job_status_msg(num_jobs, query)
+
     return job_data, msg
 
 
 def get_jobs(
     filters: Optional[dict] = None,
     refresh: bool = False,
     raw: bool = False,
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/inspector.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/inspector.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,71 +8,78 @@
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module for performing QASM program checks before conversion
 
 """
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from openqasm3.parser import QASM3ParsingError, parse
 
-from qbraid._qprogram import QPROGRAM_LIBS
-from qbraid.exceptions import PackageValueError, ProgramTypeError, QasmError
+from ._import import QPROGRAM_LIBS
+from .exceptions import PackageValueError, ProgramTypeError, QasmError
 
 if TYPE_CHECKING:
-    import qbraid
+    import qbraid.programs
 
 
 def get_qasm_version(qasm_str: str) -> str:
     """Gets OpenQASM program version, either qasm2 or qasm3.
 
     Args:
         qasm_str: An OpenQASM program string
 
     Returns:
-        QASM version from list :obj:`~qbraid.QPROGRAM_LIBS`
+        QASM version from list :obj:`~qbraid.programs.QPROGRAM_LIBS`
 
     Raises:
-        :class:`~qbraid.QasmError`: If string does not represent a valid OpenQASAM program.
+        :class:`~qbraid.programs.QasmError`: If string does not represent a valid OpenQASAM program.
 
     """
     qasm_str = qasm_str.replace("opaque", "// opaque")
 
     try:
         program = parse(qasm_str)
         verion = int(float(program.version))
         return f"qasm{verion}"
     except QASM3ParsingError as err:
         raise QasmError("Failed to parse OpenQASM program.") from err
 
 
-def get_program_type(program: "qbraid.QPROGRAM", require_supported: bool = True) -> str:
+def get_program_type(
+    program: "qbraid.programs.QPROGRAM", require_supported: bool = True
+) -> Optional[str]:
     """
     Get the type of a quantum program.
 
     Args:
-        program (qbraid.QPROGRAM): The quantum program to get the type of.
+        program (qbraid.programs.QPROGRAM): The quantum program to get the type of.
         require_supported (bool): If True, raise an error if the program type is not supported.
 
     Returns:
-        str: The type of the quantum program.
+        str: The type of the quantum program, or None if the type cannot be determined and
+             require_supported is False.
     """
     if isinstance(program, str):
         try:
             package = get_qasm_version(program)
         except QasmError as err:
-            raise ProgramTypeError(
-                "Input of type string must represent a valid OpenQASM program."
-            ) from err
+            if require_supported:
+                raise ProgramTypeError(
+                    "Input of type string must represent a valid OpenQASM program."
+                ) from err
+            package = None
 
     else:
         try:
             program_module = program.__module__
             package = program_module.split(".")[0].lower()
         except AttributeError as err:
-            raise ProgramTypeError(program) from err
+            if require_supported:
+                raise ProgramTypeError(program) from err
+            package = None
 
     if package not in QPROGRAM_LIBS and require_supported:
         raise PackageValueError(package)
 
     return package
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/interface/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/interface/circuit_equality.py` & `qbraid-0.6.0.dev20240404040745/qbraid/interface/circuit_equality.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 Module for calculating unitary of quantum circuit/program
 
 """
 from typing import TYPE_CHECKING, Tuple
 
 import numpy as np
 
+from qbraid.programs import load_program
+
 if TYPE_CHECKING:
     import qbraid
 
 
 def match_global_phase(a: np.ndarray, b: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     """
     Matches the global phase of two numpy arrays.
@@ -73,38 +75,37 @@
 
     """
     a, b = match_global_phase(a, b)
     np.testing.assert_allclose(actual=a, desired=b, atol=atol, **kwargs)
 
 
 def circuits_allclose(  # pylint: disable=too-many-arguments
-    circuit0: "qbraid.QPROGRAM",
-    circuit1: "qbraid.QPROGRAM",
+    circuit0: "qbraid.programs.QPROGRAM",
+    circuit1: "qbraid.programs.QPROGRAM",
     index_contig: bool = False,
     allow_rev_qubits: bool = False,
     strict_gphase: bool = False,
     atol: float = 1e-7,
 ) -> bool:
     """Check if quantum program unitaries are equivalent.
 
     Args:
-        circuit0 (:data:`~qbraid.QPROGRAM`): First quantum program to compare
-        circuit1 (:data:`~qbraid.QPROGRAM`): Second quantum program to compare
+        circuit0 (:data:`~qbraid.programs.QPROGRAM`): First quantum program to compare
+        circuit1 (:data:`~qbraid.programs.QPROGRAM`): Second quantum program to compare
         index_contig: If True, calculates circuit unitaries using contiguous qubit indexing.
         allow_rev_qubits: Whether to count identical circuits with reversed qubit ordering
             as equivalent.
         strict_gphase: If False, disregards global phase when verifying
             equivalence of the input circuit's unitaries.
         atol: Absolute tolerance parameter for np.allclose function.
 
     Returns:
         True if the input circuits pass unitary equality check
 
     """
-    from qbraid import circuit_wrapper  # pylint: disable=import-outside-toplevel
 
     def unitary_equivalence_check(unitary0, unitary1, unitary_rev=None):
         if strict_gphase:
             return np.allclose(unitary0, unitary1) or (
                 allow_rev_qubits and np.allclose(unitary0, unitary_rev)
             )
         try:
@@ -115,16 +116,16 @@
                     assert_allclose_up_to_global_phase(unitary0, unitary_rev, atol=atol)
                 except AssertionError:
                     return False
             else:
                 return False
         return True
 
-    program0 = circuit_wrapper(circuit0)
-    program1 = circuit_wrapper(circuit1)
+    program0 = load_program(circuit0)
+    program1 = load_program(circuit1)
 
     if index_contig:
         program0.remove_idle_qubits()
         program1.remove_idle_qubits()
 
     unitary0 = program0.unitary()
     unitary1 = program1.unitary()
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/interface/random/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/interface/random/cirq_random.py` & `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/cirq_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/interface/random/qasm3_random.py` & `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/qasm3_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/interface/random/qiskit_random.py` & `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/qiskit_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/interface/random/random.py` & `qbraid-0.6.0.dev20240404040745/qbraid/interface/random/random.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,41 +12,41 @@
 Module for generate random quantum circuits used for testing
 
 """
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple
 
 import numpy as np
 
-from qbraid._qprogram import QPROGRAM, QPROGRAM_LIBS
-from qbraid.exceptions import PackageValueError
-from qbraid.transpiler.converter import convert_to_package
+from qbraid.programs._import import QPROGRAM, QPROGRAM_LIBS
+from qbraid.programs.exceptions import PackageValueError
+from qbraid.transpiler.converter import transpile
 
 QROGRAM_TEST_TYPE = Tuple[Dict[str, Callable[[Any], QPROGRAM]], np.ndarray]
 
 if TYPE_CHECKING:
-    import qbraid
+    import qbraid.programs
 
 
 def random_circuit(
     package: str, num_qubits: Optional[int] = None, depth: Optional[int] = None, **kwargs
-) -> "qbraid.QPROGRAM":
+) -> "qbraid.programs.QPROGRAM":
     """Generate random circuit of arbitrary size and form.
 
     Args:
         package: qBraid supported software package
         num_qubits: Number of quantum wires. If not provided, set randomly in range [2,4].
         depth: Layers of operations (i.e. critical path length)
             If not provided, set randomly in range [2,4].
 
     Raises:
         PackageValueError: if ``package`` is not supported
         QbraidError: when invalid random circuit options given
 
     Returns:
-        :data:`~qbraid.QPROGRAM`: randomly generated quantum circuit/program
+        :data:`~qbraid.programs.QPROGRAM`: randomly generated quantum circuit/program
 
     """
     if package not in QPROGRAM_LIBS:
         raise PackageValueError(package)
 
     num_qubits = np.random.randint(1, 4) if num_qubits is None else num_qubits
     depth = np.random.randint(1, 4) if depth is None else depth
@@ -62,15 +62,15 @@
         rand_circuit = _qiskit_random(num_qubits, depth, **kwargs)
     else:
         from qbraid.interface.random.cirq_random import _cirq_random
 
         rand_circuit = _cirq_random(num_qubits, depth, **kwargs)
 
         if package != "cirq":
-            rand_circuit = convert_to_package(rand_circuit, package)
+            rand_circuit = transpile(rand_circuit, package)
 
     return rand_circuit
 
 
 def random_unitary_matrix(dim: int) -> np.ndarray:
     """Create a random (complex) unitary matrix of order `dim`
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,22 +5,44 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module containing quantum circuit wrapper classes providing uniform
-suite of methods and functionality for supported program types.
+Module providing unified conversions interface between supported
+quantum program types.
 
-.. currentmodule:: qbraid.programs
+.. currentmodule:: qbraid.transpiler
 
 Classes
 --------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   QuantumProgram
+   ConversionGraph
+   Conversion
+
+Functions
+-----------
+
+.. autosummary::
+   :toctree: ../stubs/
+
+   transpile
+
+Exceptions
+-----------
+
+.. autosummary::
+   :toctree: ../stubs/
+
+   CircuitConversionError
+   NodeNotFoundError
+   ConversionPathNotFoundError
 
 """
-from qbraid.programs.abc_program import QuantumProgram
+from .converter import transpile
+from .edge import Conversion
+from .exceptions import CircuitConversionError, ConversionPathNotFoundError, NodeNotFoundError
+from .graph import ConversionGraph
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/abc_program.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/abc_program.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,36 +13,35 @@
 
 """
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Any, List, Optional
 
 import numpy as np
 
-from qbraid.inspector import get_program_type
-from qbraid.transpiler.converter import convert_to_package
+from .inspector import get_program_type
 
 if TYPE_CHECKING:
     import qbraid
 
 
 class QuantumProgram:
     """Abstract class for qbraid program wrapper objects."""
 
-    def __init__(self, program: "qbraid.QPROGRAM"):
+    def __init__(self, program: "qbraid.programs.QPROGRAM"):
         self.program = program
         self._program = program
         self._package = get_program_type(program)
 
     @property
     def package(self) -> str:
         """Return the original package of the wrapped circuit."""
         return self._package
 
     @property
-    def program(self) -> "qbraid.QPROGRAM":
+    def program(self) -> "qbraid.programs.QPROGRAM":
         """Return the wrapped quantum program object."""
         return self._program
 
     @property
     @abstractmethod
     def qubits(self) -> List[Any]:
         """Return the qubits acted upon by the operations in this circuit"""
@@ -141,26 +140,7 @@
     @abstractmethod
     def remove_idle_qubits(self) -> None:
         """Remove empty registers of circuit."""
 
     @abstractmethod
     def reverse_qubit_order(self) -> None:
         """Rerverse qubit ordering of circuit."""
-
-    def transpile(self, conversion_type: str) -> "qbraid.QPROGRAM":
-        """Transpile a qbraid quantum program wrapper object to quantum
-        program object of type specified by ``conversion_type``.
-
-        Args:
-            conversion_type: a supported quantum frontend package.
-                Must be one of :data:`~qbraid.QPROGRAM_LIBS`.
-
-        Raises:
-            PackageValueError: If ``conversion_type`` is not one of
-                :data:`~qbraid.QPROGRAM_LIBS`.
-            CircuitConversionError: If the input quantum program could not be
-                converted to a program of type ``conversion_type``.
-
-        Returns:
-            :data:`~qbraid.QPROGRAM`: supported quantum program object
-        """
-        return convert_to_package(self.program, conversion_type)
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/braket.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/cirq.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/pennylane.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pennylane.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/pyquil.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pyquil.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 """
 
 from typing import List
 
 import numpy as np
 import pyquil
+from pyquil import Program
+from pyquil.quilbase import Declare, Measurement
 from pyquil.simulation.tools import program_unitary
 
 from qbraid.programs.abc_program import QuantumProgram
 
 
 class PyQuilProgram(QuantumProgram):
     """Wrapper class for ``pyQuil.Program`` objects."""
@@ -54,17 +56,27 @@
         return 0
 
     @property
     def depth(self) -> int:
         """Return the circuit depth (i.e., length of critical path)."""
         return len(self.program)
 
+    @staticmethod
+    def remove_measurements(original_program):
+        """Remove MEASURE and DECLARE instructions from a pyQuil program."""
+        program = Program()
+        for instruction in original_program:
+            if not isinstance(instruction, Measurement) and not isinstance(instruction, Declare):
+                program += instruction
+        return program
+
     def _unitary(self) -> "np.ndarray":
         """Return the unitary of a pyQuil program."""
-        return program_unitary(self.program, n_qubits=self.num_qubits)
+        program_copy = self.remove_measurements(self.program)
+        return program_unitary(program_copy, n_qubits=self.num_qubits)
 
     def remove_idle_qubits(self) -> None:
         """Checks whether the circuit uses contiguous qubits/indices,
         and if not, reduces dimension accordingly."""
         raise NotImplementedError
 
     def reverse_qubit_order(self) -> None:
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/pytket.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/pytket.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Module defining PytketCircuit Class
 
 """
 
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import numpy as np
-from pytket.circuit import Circuit, Command
+from pytket.circuit import Circuit, Command, OpType
 from pytket.unit_id import Qubit
 
 from qbraid.programs.abc_program import QuantumProgram
 
 if TYPE_CHECKING:
     import pytket
 
@@ -57,17 +57,46 @@
         return self.program.n_bits
 
     @property
     def depth(self) -> int:
         """Return the circuit depth (i.e., length of critical path)."""
         return self.program.depth()
 
+    @staticmethod
+    def remove_measurements(original_circuit):
+        """
+        Return a new circuit with all non-measurement operations from the original circuit.
+
+        Args:
+            original_circuit: The pytket Circuit to process.
+
+        Returns:
+            A new pytket Circuit without measurement operations.
+        """
+        new_circuit = Circuit()
+        for qreg in original_circuit.qubits:
+            new_circuit.add_qubit(qreg)
+        for creg in original_circuit.bits:
+            new_circuit.add_bit(creg)
+
+        for command in original_circuit.get_commands():
+            if command.op.type != OpType.Measure:
+                new_circuit.add_gate(
+                    command.op.type, command.op.params, [q.index[0] for q in command.qubits]
+                )
+
+        return new_circuit
+
     def _unitary(self) -> "np.ndarray":
         """Return the unitary of a pytket circuit."""
-        return self.program.get_unitary()
+        try:
+            return self.program.get_unitary()
+        except RuntimeError:
+            program_copy = self.remove_measurements(self.program)
+            return program_copy.get_unitary()
 
     def remove_idle_qubits(self) -> None:
         """Checks whether the circuit uses contiguous qubits/indices,
         and if not, reduces dimension accordingly."""
         circuit = self.program.copy()
         circuit.remove_blank_wires()
         self._program = circuit
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/qasm2.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/qasm3.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qasm3.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,26 +87,19 @@
     def num_clbits(self) -> int:
         """Return the number of classical bits in the circuit."""
         return self._num_clbits
 
     @property
     def depth(self) -> int:
         """Return the circuit depth (i.e., length of critical path)."""
-        # pylint: disable=import-outside-toplevel
-        from qiskit.qasm3 import loads
-
-        return loads(self.program).depth()
+        raise NotImplementedError
 
     def _unitary(self) -> "np.ndarray":
         """Calculate unitary of circuit."""
-        # pylint: disable=import-outside-toplevel
-        from qiskit.qasm3 import loads
-        from qiskit.quantum_info import Operator
-
-        return Operator(loads(self.program)).data
+        raise NotImplementedError
 
     @staticmethod
     def _remove_gate_definitions(qasm_str: str) -> str:
         """This is required to account for the case when the gate
         definition has an argument which is having same name as a
         quantum register
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/programs/qiskit.py` & `qbraid-0.6.0.dev20240404040745/qbraid/programs/libs/qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,17 +10,22 @@
 
 """
 Module providing unified interface for interacting with
 various quantum provider APIs.
 
 .. currentmodule:: qbraid.providers
 
+.. _devices_data_type:
+
 Data Types
 ------------
 
+.. autodata:: QDEVICE
+   :annotation: = Type alias defining all supported quantum device / backend types
+
 .. autosummary::
    :toctree: ../stubs/
 
    DeviceStatus
    DeviceType
 
 Classes
@@ -40,17 +45,24 @@
 
 .. autosummary::
    :toctree: ../stubs/
 
    JobError
    JobStateError
    ProgramValidationError
-   QbraidDeviceNotFoundError
    QbraidRuntimeError
+   ResourceNotFoundError
 
 """
+from ._import import QDEVICE, QDEVICE_LIBS, QDEVICE_TYPES, SUPPORTED_QDEVICES
 from .device import QuantumDevice
 from .enums import DeviceStatus, DeviceType, JobStatus
-from .exceptions import JobError, JobStateError, ProgramValidationError, QbraidRuntimeError
+from .exceptions import (
+    JobError,
+    JobStateError,
+    ProgramValidationError,
+    QbraidRuntimeError,
+    ResourceNotFoundError,
+)
 from .job import QuantumJob
-from .provider import QbraidDeviceNotFoundError, QbraidProvider
+from .provider import QbraidProvider
 from .result import QuantumJobResult
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/device.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,31 @@
 
 """
 Module defining BraketDeviceWrapper Class
 
 """
 import json
 from datetime import datetime, timedelta
-from typing import TYPE_CHECKING, List, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Tuple
 
 from braket.device_schema import ExecutionDay
 
-from qbraid._qprogram import QPROGRAM_LIBS
+from qbraid.programs._import import QPROGRAM_LIBS
+from qbraid.programs.libs.braket import BraketCircuit
 from qbraid.providers.device import QuantumDevice
 from qbraid.providers.enums import DeviceStatus, DeviceType
 
 from .job import BraketQuantumTask
 
 if TYPE_CHECKING:
     import braket.aws
+    import braket.circuits
 
-    import qbraid
+    import qbraid.providers.aws
+    import qbraid.transpiler
 
 
 def _future_utc_datetime(hours: int, minutes: int, seconds: int) -> str:
     """Return a UTC datetime that is hours, minutes, and seconds from now
     as an ISO string without fractional seconds."""
     current_utc = datetime.utcnow()
     future_time = current_utc + timedelta(hours=hours, minutes=minutes, seconds=seconds)
@@ -50,15 +53,15 @@
 
     def _populate_metadata(self, device: "braket.aws.AwsDevice") -> None:
         """Populate device metadata using BraketSchemaBase"""
         # pylint: disable=attribute-defined-outside-init
         metadata = device.aws_session.get_device(device.arn)
         capabilities = json.loads(metadata.get("deviceCapabilities"))
 
-        self._id = metadata.get("deviceArn")
+        self._vendor_id = metadata.get("deviceArn")
         self._name = metadata.get("deviceName")
         self._provider = metadata.get("providerName")
         self._device_type = DeviceType(metadata.get("deviceType"))
 
         try:
             self._num_qubits = capabilities["paradigm"]["qubitCount"]
         except KeyError:
@@ -195,17 +198,14 @@
                 num_queued = num_queued[1:]
             total_queued += int(num_queued)
         return total_queued
 
     def _transpile(self, run_input):
         """Transpile a circuit for the device."""
         if self._device_type.name == "SIMULATOR":
-            # pylint: disable=import-outside-toplevel
-            from qbraid.programs.braket import BraketCircuit
-
             program = BraketCircuit(run_input)
             program.remove_idle_qubits()
             run_input = program.program
 
         return run_input
 
     def _compile(self, run_input):
@@ -213,79 +213,60 @@
         if self.provider.lower() == "ionq" and "pytket" in QPROGRAM_LIBS:
             # pylint: disable=import-outside-toplevel
             from qbraid.compiler.braket.ionq import braket_ionq_compile
 
             run_input = braket_ionq_compile(run_input)
         return run_input
 
-    def run(
-        self, run_input, *args, auto_compile: bool = False, **kwargs
-    ) -> "qbraid.device.aws.BraketQuantumTaskWrapper":
+    def _run(self, run_input: "braket.circuits.Circuit", *args, **kwargs) -> Dict[str, Any]:
         """Run a quantum task specification on this quantum device. Task must represent a
         quantum circuit, annealing problems not supported.
 
         Args:
             run_input: Specification of a task to run on device.
 
         Keyword Args:
-            auto_compile (bool): Whether to compile the circuit for the device before running.
             shots (int): The number of times to run the task on the device.
 
         Returns:
             The job like object for the run.
 
         """
-        qbraid_circuit = self.process_run_input(run_input, auto_compile=auto_compile)
-        run_input = qbraid_circuit._program
         aws_quantum_task = self._device.run(run_input, *args, **kwargs)
         metadata = aws_quantum_task.metadata()
-        shots = metadata.get("shots", 0)
-        tags = metadata.get("tags", {})
-        vendor_job_id = metadata["quantumTaskArn"]
-        job_id = self._init_job(vendor_job_id, [qbraid_circuit], shots, tags)
-        return BraketQuantumTask(
-            job_id, vendor_job_id=vendor_job_id, device=self, vendor_job_obj=aws_quantum_task
-        )
-
-    def run_batch(
-        self, run_input, *args, auto_compile: bool = False, **kwargs
-    ) -> List["qbraid.device.aws.BraketQuantumTaskWrapper"]:
+        return {
+            "vendor_job_id": metadata["quantumTaskArn"],
+            "tags": metadata.get("tags", {}),
+            "shots": metadata.get("shots", 0),
+            "vendor_job_obj": aws_quantum_task,
+            "qbraid_job_obj": BraketQuantumTask,
+        }
+
+    def _run_batch(self, run_input, *args, **kwargs) -> List[Dict[str, Any]]:
         """Run batch of quantum tasks on this quantum device.
 
         Args:
             run_input: A circuit object list to run on the wrapped device.
 
         Keyword Args:
             auto_compile (bool): Whether to compile the circuits for the device before running.
             shots (int): The number of times to run the task on the device. Default is 1024.
 
         Returns:
             List of BraketQuantumTask objects for the run.
 
         """
         device = self._device
-        qbraid_circuit_batch = []
-        run_input_batch = []
-        for circuit in run_input:
-            qbraid_circuit = self.process_run_input(circuit, auto_compile=auto_compile)
-            run_input = qbraid_circuit._program
-            run_input_batch.append(run_input)
-            qbraid_circuit_batch.append(qbraid_circuit)
-        aws_quantum_task_batch = device.run_batch(run_input_batch, *args, **kwargs)
+        aws_quantum_task_batch = device.run_batch(run_input, *args, **kwargs)
         aws_quantum_tasks = aws_quantum_task_batch.tasks
-        aws_quantum_task_wrapper_list = []
-        for index, aws_quantum_task in enumerate(aws_quantum_tasks):
-            qbraid_circuit = qbraid_circuit_batch[index]
+        aws_quantum_task_data = []
+        for _, aws_quantum_task in enumerate(aws_quantum_tasks):
             metadata = aws_quantum_task.metadata()
-            shots = metadata.get("shots", 0)
-            tags = metadata.get("tags", {})
-            vendor_job_id = metadata["quantumTaskArn"]
-            job_id = self._init_job(vendor_job_id, [qbraid_circuit], shots, tags)
-            aws_quantum_task_wrapper_list.append(
-                BraketQuantumTask(
-                    job_id,
-                    vendor_job_id=vendor_job_id,
-                    device=self,
-                    vendor_job_obj=aws_quantum_task,
-                )
-            )
-        return aws_quantum_task_wrapper_list
+            job_data = {
+                "vendor_job_id": metadata["quantumTaskArn"],
+                "tags": metadata.get("tags", {}),
+                "shots": metadata.get("shots", 0),
+                "vendor_job_obj": aws_quantum_task,
+                "qbraid_job_obj": BraketQuantumTask,
+            }
+            aws_quantum_task_data.append(job_data)
+        return aws_quantum_task_data
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/job.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/provider.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 import os
 from typing import TYPE_CHECKING, List, Optional
 
 import boto3
 from boto3.session import Session
 from braket.aws import AwsDevice, AwsSession
+from qbraid_core.services.quantum import quantum_lib_proxy_state
 
-from qbraid.api import QbraidSession
 from qbraid.exceptions import QbraidError
+from qbraid.providers.provider import QuantumProvider
 
 if TYPE_CHECKING:
     import braket.aws
 
 
-class BraketProvider:
+class BraketProvider(QuantumProvider):
     """
     This class is responsible for managing the interactions and
     authentications with the AWS services.
 
     Attributes:
         aws_access_key_id (str): AWS access key ID for authenticating with AWS services.
         aws_secret_access_key (str): AWS secret access key for authenticating with AWS services.
@@ -105,19 +106,19 @@
     ) -> List["braket.aws.AwsDevice"]:
         """Return a list of backends matching the specified filtering."""
         aws_session = self._get_aws_session() if aws_session is None else aws_session
         statuses = ["ONLINE", "OFFLINE"] if statuses is None else statuses
 
         return AwsDevice.get_devices(aws_session=aws_session, statuses=statuses, **kwargs)
 
-    def get_device(self, device_arn: str) -> "braket.aws.AwsDevice":
+    def get_device(self, device_id: str) -> "braket.aws.AwsDevice":
         """Returns the AWS device."""
-        region_name = self._get_region_name(device_arn)
+        region_name = self._get_region_name(device_id)  # deviceArn
         aws_session = self._get_aws_session(region_name=region_name)
-        return AwsDevice(arn=device_arn, aws_session=aws_session)
+        return AwsDevice(arn=device_id, aws_session=aws_session)
 
     def get_tasks_by_tag(
         self, key: str, values: Optional[List[str]] = None, region_names: Optional[List[str]] = None
     ) -> List[str]:
         """
         Retrieves a list of quantum task ARNs that match the specified tag keys or key/value pairs.
 
@@ -132,15 +133,21 @@
         Returns:
             List[str]: A list of ARNs for quantum tasks that match the given tag criteria.
 
         Raises:
             QbraidError: If the function is called within a qBraid quantum job environment
                          where AWS S3 requests are not supported.
         """
-        if QbraidSession._qbraid_jobs_enabled():
+        try:
+            jobs_state = quantum_lib_proxy_state("braket")
+            jobs_enabled = jobs_state.get("enabled", False)
+        except ValueError:
+            jobs_enabled = False
+
+        if jobs_enabled:
             raise QbraidError("AWS S3 requests not supported by qBraid quantum jobs.")
 
         region_names = (
             region_names
             if region_names is not None and len(region_names) > 0
             else list(self.REGIONS)
         )
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/result.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/aws/tracker.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/aws/tracker.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/enums.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/exceptions.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,13 +19,17 @@
     """Base class for errors raised while validating a quantum program."""
 
 
 class QbraidRuntimeError(QbraidError):
     """Base class for errors raised while submitting a quantum job."""
 
 
+class ResourceNotFoundError(QbraidError):
+    """Exception raised when the desired resource could not be found."""
+
+
 class JobError(QbraidError):
     """Base class for errors raised by Jobs."""
 
 
 class JobStateError(JobError):
     """Class for errors raised due to the state of a quantum job"""
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/device.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Module defining QiskitBackend Class
 
 """
 import re
-from typing import TYPE_CHECKING, Union  # pylint: disable=unused-import
+from typing import TYPE_CHECKING, List, Union
 
 from qiskit import transpile
 from qiskit.transpiler import TranspilerError
 
+from qbraid.programs.libs.qiskit import QiskitCircuit
 from qbraid.providers.device import QuantumDevice
 from qbraid.providers.enums import DeviceStatus, DeviceType
 
 from .job import QiskitJob
 
 if TYPE_CHECKING:
+    import qiskit
     import qiskit_ibm_provider
     import qiskit_ibm_runtime
 
 
 class QiskitBackend(QuantumDevice):
     """Wrapper class for IBM Qiskit ``Backend`` objects."""
 
@@ -54,15 +56,15 @@
 
     def _populate_metadata(
         self, device: Union["qiskit_ibm_provider.IBMBackend", "qiskit_ibm_runtime.IBMBackend"]
     ) -> None:
         """Populate device metadata using IBMBackend object."""
         # pylint: disable=attribute-defined-outside-init
         device_name = self._get_device_name()
-        self._id = device_name
+        self._vendor_id = device_name
         self._name = device_name
         self._provider = "IBM"
         lower_device_name = device_name.lower()
         if lower_device_name.startswith("fake"):
             self._device_type = DeviceType.FAKE
         elif "simulator" in lower_device_name or "aer" in lower_device_name:
             self._device_type = DeviceType.SIMULATOR
@@ -81,17 +83,14 @@
                 5000
                 if device.name == "simulator_stabilizer"
                 else 63 if device.name == "simulator_extended_stabilizer" else None
             )
 
     def _transpile(self, run_input):
         if self._device_type.name != "FAKE" and self._device.local:
-            # pylint: disable=import-outside-toplevel
-            from qbraid.programs.qiskit import QiskitCircuit
-
             program = QiskitCircuit(run_input)
             program.remove_idle_qubits()
             run_input = program.program
 
         return transpile(run_input, backend=self._device)
 
     def _compile(self, run_input):
@@ -113,90 +112,63 @@
 
     def queue_depth(self) -> int:
         """Return the number of jobs in the queue for the ibm backend"""
         if self._device_type == DeviceType("FAKE"):
             return 0
         return self._device.status().pending_jobs
 
-    def run(self, run_input, *args, **kwargs):
+    def _run(
+        self,
+        run_input: "Union[qiskit.QuantumCircuit, List[qiskit.QuantumCircuit]]",
+        *args,
+        **kwargs,
+    ):
         """Runs circuit(s) on qiskit backend via :meth:`~qiskit.execute`
 
-        Uses the :meth:`~qiskit.execute` method to create a :class:`~qiskit.providers.Job` object,
-        applies a :class:`~qbraid.providers.ibm.QiskitJob`, and return the result.
+        Uses the :meth:`~qiskit.execute` method to create a :class:`~qiskit.providers.QuantumJob`
+        object, applies a :class:`~qbraid.providers.ibm.QiskitJob`, and return the result.
 
         Args:
-            run_input: A circuit object to run on the wrapped device.
+            run_input: A circuit object to run on the IBM device.
 
         Keyword Args:
             shots (int): The number of times to run the task on the device. Default is 1024.
 
         Returns:
             qbraid.providers.ibm.QiskitJob: The job like object for the run.
 
         """
         backend = self._device
-        qbraid_circuit = self.process_run_input(run_input)
-        run_input = qbraid_circuit._program
         shots = kwargs.pop("shots", backend.options.get("shots"))
         memory = kwargs.pop("memory", True)  # Needed to get measurements
-        qiskit_job = backend.run(run_input, shots=shots, memory=memory, **kwargs)
+        qiskit_job = backend.run(run_input, shots=shots, memory=memory)
         try:
             tags_lst = qiskit_job.update_tags(kwargs.get("tags", []))
         except AttributeError:  # BasicAerJob does not have update_tags
             tags_lst = []
         tags = {tag: "*" for tag in tags_lst}
         qiskit_job_id = qiskit_job.job_id()
-        qbraid_job_id = (
-            self._init_job(qiskit_job_id, [qbraid_circuit], shots, tags)
-            if self._device_type != DeviceType("FAKE")
-            else "qbraid_test_id"
-        )
-        qbraid_job = QiskitJob(
-            qbraid_job_id, vendor_job_id=qiskit_job_id, device=self, vendor_job_obj=qiskit_job
-        )
-        return qbraid_job
+        return {
+            "vendor_job_id": qiskit_job_id,
+            "tags": tags,
+            "shots": shots,
+            "vendor_job_obj": qiskit_job,
+            "qbraid_job_obj": QiskitJob,
+        }
 
-    def run_batch(self, run_input, **kwargs):
+    def _run_batch(self, run_input: "List[qiskit.QuantumCircuit]", *args, **kwargs):
         """Runs circuit(s) on qiskit backend via :meth:`~qiskit.execute`
 
-        Uses the :meth:`~qiskit.execute` method to create a :class:`~qiskit.providers.Job` object,
-        applies a :class:`~qbraid.providers.ibm.QiskitJob`, and return the result.
+        Uses the :meth:`~qiskit.execute` method to create a :class:`~qiskit.providers.QuantumJob`
+        object, applies a :class:`~qbraid.providers.ibm.QiskitJob`, and return the result.
 
         Args:
             run_input: A circuit object list to run on the wrapped device.
 
         Keyword Args:
             shots (int): The number of times to run the task on the device. Default is 1024.
 
         Returns:
             qbraid.providers.ibm.QiskitJob: The job like object for the run.
 
         """
-        backend = self._device
-        qbraid_circuit_batch = []
-        run_input_batch = []
-        for circuit in run_input:
-            qbraid_circuit = self.process_run_input(circuit)
-            run_input = qbraid_circuit._program
-            run_input_batch.append(run_input)
-            qbraid_circuit_batch.append(qbraid_circuit)
-
-        shots = kwargs.pop("shots", backend.options.get("shots"))
-        memory = kwargs.pop("memory", True)  # Needed to get measurements
-        qiskit_job = backend.run(run_input_batch, shots=shots, memory=memory, **kwargs)
-        try:
-            tags_lst = qiskit_job.update_tags(kwargs.get("tags", []))
-        except AttributeError:  # BasicAerJob does not have update_tags
-            tags_lst = []
-        tags = {tag: "*" for tag in tags_lst}
-        qiskit_job_id = qiskit_job.job_id()
-
-        # to change to batch
-        qbraid_job_id = (
-            self._init_job(qiskit_job_id, qbraid_circuit_batch, shots, tags)
-            if self._device_type != DeviceType("FAKE")
-            else "qbraid_test_id"
-        )
-        qbraid_job = QiskitJob(
-            qbraid_job_id, vendor_job_id=qiskit_job_id, device=self, vendor_job_obj=qiskit_job
-        )
-        return qbraid_job
+        return self._run(run_input, **kwargs)
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/job.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/provider.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 """
 
 import os
 import re
 from abc import abstractmethod
 from typing import TYPE_CHECKING, List, Union
 
+from qbraid.providers.provider import QuantumProvider
+
 if TYPE_CHECKING:
     import qiskit_ibm_provider
     import qiskit_ibm_runtime
 
 
-class QiskitRemoteService:
+class QiskitRemoteService(QuantumProvider):
     """
     This class is responsible for managing the interactions and
     authentications with the IBM Quantum services.
 
     Attributes:
         qiskit_ibm_token (str): IBM Quantum token for authenticating with IBM Quantum services.
     """
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/ibm/result.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/ibm/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/job.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/job.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,56 +12,93 @@
 Module defining abstract QuantumJob Class
 
 """
 import logging
 from abc import ABC, abstractmethod
 from enum import Enum
 from time import sleep, time
-from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
-from qbraid.api import QbraidSession
+from qbraid_core.services.quantum import QuantumClient, QuantumServiceRequestError
+
+from qbraid._import import _load_entrypoint
 
 from .enums import JOB_FINAL, JobStatus
-from .exceptions import JobError
+from .exceptions import JobError, ResourceNotFoundError
+from .provider import QbraidProvider
 from .status_maps import STATUS_MAP
 
 if TYPE_CHECKING:
     import qbraid
 
 
 class QuantumJob(ABC):
     """Abstract interface for job-like classes."""
 
+    @classmethod
+    def retrieve(cls, job_id: str, **kwargs) -> "qbraid.providers.QuantumJob":
+        """Create a QuantumJob object from a job_id."""
+        try:
+            vendor = job_id.split("_")[0]
+            job_class = _load_entrypoint("providers", f"{vendor}.job")
+        except (ValueError, IndexError) as err:
+            raise ResourceNotFoundError(f"Invalid Job Id {job_id}.") from err
+        return job_class(job_id, **kwargs)
+
     def __init__(  # pylint: disable=too-many-arguments
         self,
         job_id: str,
-        vendor_job_id: Optional[str] = None,
+        job_obj: Optional[Any] = None,
+        job_json: Optional[Dict[str, Any]] = None,
         device: "Optional[qbraid.providers.QuantumDevice]" = None,
-        vendor_job_obj: Optional[Any] = None,
-        status: Optional[Union[str, JobStatus]] = None,
+        circuits: "Optional[List[qbraid.programs.QuantumProgram]]" = None,
+        provider: Optional[QbraidProvider] = None,
     ):
-        self._vendor = None
-        self._cache_metadata = None
-        self._cache_status = self._map_status(status)
+        if type(self) is QuantumJob:  # pylint: disable=unidiomatic-typecheck
+            raise NotImplementedError(
+                "QuantumJob is an abstract class and cannot be instantiated directly."
+            )
         self._job_id = job_id
-        self._vendor_job_id = vendor_job_id
-        self._device = device
-        self._job = vendor_job_obj or self._get_job()
+        self._provider = provider
+        self._client = None
+
+        job_data = job_json or self._fetch_metadata()
+        self._cache_metadata = job_data
+        self._cache_status = job_data.get("qbraidStatus", job_data.get("status"))
+        self._vendor = job_data.get("vendor")
+        self._vendor_job_id = job_data.get("vendorJobId")
+        self._device = device or self.provider.get_device(job_data["qbraidDeviceId"])
+        self._job = job_obj or self._get_job()
         self._status_map = STATUS_MAP[self.vendor]
+        self._circuits = circuits
 
     @property
     def id(self) -> str:  # pylint: disable=invalid-name
         """Return a unique id identifying the job."""
         return self._job_id
 
     @property
+    def provider(self) -> QbraidProvider:
+        """Return the quantum client object."""
+        if self._provider is None:
+            self._provider = QbraidProvider()
+        return self._provider
+
+    @property
+    def client(self) -> QuantumClient:
+        """Return the quantum client object."""
+        if self._client is None:
+            self._client = self.provider.client
+        return self._client
+
+    @property
     def vendor(self) -> str:
         """Get job vendor."""
         if self._vendor is not None:
-            return self._vendor
+            return self._vendor.upper()
 
         try:
             vendor = self._cache_metadata["vendor"]
         except (KeyError, TypeError):
             vendor = self.device.vendor
 
         self._vendor = vendor.upper()
@@ -75,39 +112,34 @@
             self._vendor_job_id = self._cache_metadata["vendorJobId"]
         return self._vendor_job_id
 
     @property
     def device(self) -> "qbraid.providers.QuantumDevice":
         """Returns the qbraid QuantumDevice object associated with this job."""
         if self._device is None:
-            self._fetch_and_set_device()
+            qbraid_device_id = self._cache_metadata["qbraidDeviceId"]
+            self._device = self.client.get_device(qbraid_device_id)
         return self._device
 
-    def _fetch_and_set_device(self) -> None:
-        """Fetches device id from the server and sets the device object."""
-        session = QbraidSession()
-        job_lst = session.post(
-            "/get-user-jobs", json={"qbraidJobId": self.id, "numResults": 1}
-        ).json()
+    def _fetch_metadata(self) -> Dict[str, Any]:
+        first_error = None
 
-        if len(job_lst) == 0:
-            job_lst = session.post("/get-user-jobs", json={"_id": self.id, "numResults": 1}).json()
+        # Attempt to get the device data first with the qbraid_id and then with the vendor_id
+        get_job_functions = [
+            lambda: self.client.get_job(qbraid_id=self.id),
+            lambda: self.client.get_job(object_id=self.id),
+        ]
+
+        for get_job_function in get_job_functions:
+            try:
+                return get_job_function()
+            except (ValueError, QuantumServiceRequestError) as err:
+                first_error = first_error or err
 
-            if len(job_lst) == 0:
-                raise JobError(f"Could not find device associated with job {self.id}.")
-
-        job_data = job_lst[0]
-
-        try:
-            import qbraid  # pylint: disable=import-outside-toplevel
-
-            vendor_device_id = job_data["vendorDeviceId"]
-            self._device = qbraid.device_wrapper(vendor_device_id)
-        except Exception as err:  # pylint: disable=broad-except
-            raise JobError(f"Could not find device associated with job {self.id}.") from err
+        raise ResourceNotFoundError(f"Quantum Job {self.id} not found.") from first_error
 
     @staticmethod
     def _map_status(status: Optional[Union[str, JobStatus]] = None) -> JobStatus:
         """Returns `JobStatus` object mapped from raw status value. If no value
         provided or conversion from string fails, returns `JobStatus.UNKNOWN`."""
         if status is None:
             return JobStatus.UNKNOWN
@@ -154,50 +186,53 @@
         qbraid_status, vendor_status = self._status()
         if qbraid_status != self._cache_status:
             self._post_job_data(
                 update={"status": vendor_status, "qbraidStatus": qbraid_status.name}
             )
         return qbraid_status
 
-    def _post_job_data(self, update: Optional[dict] = None) -> dict:
+    def _post_job_data(self, update: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
         """Retreives job metadata and optionally updates document.
 
         Args:
             update: Dictionary containing fields to update in job document.
 
         Returns:
             The metadata associated with this job
 
         """
-        session = QbraidSession()
-        body = {"_id": self.id, "qbraidJobId": self.id}
+        if self._device and self._device._device_type.name == "FAKE":
+            return self._cache_metadata
+
+        client = QuantumClient()
+        body = {"_id": self.id} if client._is_valid_object_id(self.id) else {"qbraidJobId": self.id}
         # Two status variables so we can track both qBraid and vendor status.
         if update is not None and "status" in update and "qbraidStatus" in update:
             body["status"] = update["status"]
             body["qbraidStatus"] = update["qbraidStatus"]
-        metadata = session.put("/update-job", data=body).json()
+        metadata = client.update_job(data=body)
         if "qbraidJobId" not in metadata:
             metadata["qbraidJobId"] = metadata.get("_id")
         return metadata
 
     def metadata(self) -> Dict[str, Any]:
         """Return the metadata regarding the job."""
         qbraid_status, vendor_status = self._status()
         if not self._cache_metadata or qbraid_status != self._cache_status:
             update = {"status": vendor_status, "qbraidStatus": qbraid_status.name}
             self._cache_metadata = self._post_job_data(update=update)
             self._cache_status = self._map_status(self._cache_metadata["qbraidStatus"])
         return self._cache_metadata
 
-    def wait_for_final_state(self, timeout=None, poll_interval=5) -> None:
+    def wait_for_final_state(self, timeout: Optional[int] = None, poll_interval: int = 5) -> None:
         """Poll the job status until it progresses to a final state.
 
         Args:
             timeout: Seconds to wait for the job. If ``None``, wait indefinitely.
-            poll_interval: Seconds between queries.
+            poll_interval: Seconds between queries. Defaults to 5 seconds.
 
         Raises:
             JobError: If the job does not reach a final state before the specified timeout.
 
         """
         start_time = time()
         status = self.status()
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/result.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/providers/status_maps.py` & `qbraid-0.6.0.dev20240404040745/qbraid/providers/status_maps.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,44 +5,21 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module providing unified conversions interface between supported
-quantum program types.
+Pennylane conversions
 
-.. currentmodule:: qbraid.transpiler
-
-Classes
---------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-   ConversionGraph
-   Conversion
+.. currentmodule:: qbraid.transpiler.conversions.pennylane
 
 Functions
------------
-
-.. autosummary::
-   :toctree: ../stubs/
-
-   convert_to_package
-
-Exceptions
------------
+----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   CircuitConversionError
-   NodeNotFoundError
-   ConversionPathNotFoundError
+   pennylane_to_qasm2
 
 """
-from .converter import convert_to_package
-from .edge import Conversion
-from .exceptions import CircuitConversionError, ConversionPathNotFoundError, NodeNotFoundError
-from .graph import ConversionGraph
+from qbraid.transpiler.conversions.pennylane.conversions_qasm import pennylane_to_qasm2
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import importlib
 import inspect
 
 from .qasm_passes import flatten_qasm_program, remove_qasm_barriers, unfold_qasm_gate_defs
 from .qasm_qelib1 import decompose_qasm_qelib1
 
 # Dynamically import QPROGRAM_LIBS when needed
-_qbraid = importlib.import_module("qbraid._qprogram")
+_qbraid = importlib.import_module("qbraid.programs._import")
 _PROGRAM_LIBS = getattr(_qbraid, "_PROGRAM_LIBS", [])
 
 # List to store the names of the imported functions
 conversion_functions = []
 
 # Base path for the sub-modules
 base_path = "qbraid.transpiler.conversions."
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/cirq_from_braket.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/cirq_from_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/cirq_to_braket.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/cirq_to_braket.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from braket.circuits import gates as braket_gates
 from braket.circuits import noises as braket_noise_gate
 from cirq import Circuit
 from cirq import ops as cirq_ops
 from cirq import protocols
 from cirq.linalg.decompositions import kak_decomposition
 
+import qbraid.programs.libs.cirq
+
 try:
     import cirq_ionq.ionq_native_gates as cirq_ionq_ops
 except ImportError:
     cirq_ionq_ops = None
 
 from qbraid.transpiler.conversions.braket.custom_gates import C as BKControl
 from qbraid.transpiler.exceptions import CircuitConversionError
@@ -44,19 +46,18 @@
 
     Args:
         circuit: Cirq circuit to convert to a Braket circuit.
 
     Returns:
         Braket circuit equivalent to the input Cirq circuit.
     """
-    # pylint: disable=import-outside-toplevel
-    import qbraid.programs.cirq
-
     cirq_qubits = list(circuit.all_qubits())
-    cirq_int_qubits = [qbraid.programs.cirq.CirqCircuit._int_from_qubit(q) for q in cirq_qubits]
+    cirq_int_qubits = [
+        qbraid.programs.libs.cirq.CirqCircuit._int_from_qubit(q) for q in cirq_qubits
+    ]
     braket_int_qubits = deepcopy(cirq_int_qubits)
     qubit_mapping = {q: braket_int_qubits[i] for i, q in enumerate(cirq_int_qubits)}
     return BKCircuit(
         _to_braket_instruction(operation, qubit_mapping) for operation in circuit.all_operations()
     )
 
 
@@ -69,25 +70,24 @@
     Args:
         operation: Cirq operation to convert.
         qubit_mapping: Mappings of input / output qubit indicies
 
     Raises:
         CircuitConversionError: If the operation cannot be converted to Braket.
     """
-    # pylint: disable=import-outside-toplevel
-    import qbraid.programs.cirq
-
     if isinstance(
         operation, (cirq_ops.MeasurementGate, cirq_ops.Operation)
-    ) and qbraid.programs.cirq.CirqCircuit.is_measurement_gate(operation):
+    ) and qbraid.programs.libs.cirq.CirqCircuit.is_measurement_gate(operation):
         return []
 
     nqubits = protocols.num_qubits(operation)
     cirq_qubits = operation.qubits
-    cirq_qubits = [qbraid.programs.cirq.CirqCircuit._int_from_qubit(q) for q in operation.qubits]
+    cirq_qubits = [
+        qbraid.programs.libs.cirq.CirqCircuit._int_from_qubit(q) for q in operation.qubits
+    ]
     qubits = [qubit_mapping[x] for x in cirq_qubits]
 
     if nqubits == 1:
         target = qubits[0]
         return _to_one_qubit_braket_instruction(operation, target)
 
     if nqubits == 2:
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/conversions_qasm.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/conversions_qasm.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import math
 import re
 
 from braket.circuits import Circuit
 from braket.circuits.serialization import IRType
 from braket.ir.openqasm import Program as OpenQasmProgram
 
-from qbraid.exceptions import QasmError
+from qbraid.programs.exceptions import QasmError
 
 QASMType = str
 
 
 def _convert_pi_to_decimal(qasm_str: str) -> str:
     """Convert all instances of 'pi' in the QASM string to their decimal value."""
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/braket/custom_gates.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/braket/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/cirq_gates.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/cirq_gates.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/cirq_qasm_parser.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/cirq/conversions_qasm.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/cirq/conversions_qasm.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Optional
 
 import cirq
 from cirq import ops
 from cirq.contrib.qasm_import.exception import QasmException as CirqQasmException
 
 import qbraid
-from qbraid.exceptions import QasmError as QbraidQasmError
+from qbraid.programs.exceptions import QasmError as QbraidQasmError
 from qbraid.transpiler.conversions.cirq.cirq_gates import _map_zpow_and_unroll
 from qbraid.transpiler.conversions.cirq.cirq_qasm_parser import QasmParser
 from qbraid.transpiler.conversions.qasm_passes import flatten_qasm_program
 
 QASMType = str
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/openqasm3/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/openqasm3/convert_qasm.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/openqasm3/convert_qasm.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Module containing OpenQASM conversion function
 
 """
 import os
 
 import openqasm3
 
-from qbraid.inspector import get_qasm_version
+from qbraid.programs.inspector import get_qasm_version
 from qbraid.transpiler.conversions.qasm_qelib1 import _decompose_rxx_instr
 
 QASMType = str
 
 
 def _get_qasm3_gate_defs() -> str:
     """Helper function to get openqasm 3 gate defs from .qasm file"""
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pennylane/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Pennylane conversions
+PyTKET conversions
 
-.. currentmodule:: qbraid.transpiler.conversions.pennylane
+.. currentmodule:: qbraid.transpiler.conversions.pytket
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   pennylane_to_qasm2
+   pytket_to_qasm2
+   qasm2_to_pytket
 
 """
-from qbraid.transpiler.conversions.pennylane.conversions_qasm import pennylane_to_qasm2
+from qbraid.transpiler.conversions.pytket.conversions_qasm import pytket_to_qasm2, qasm2_to_pytket
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pennylane/conversions_qasm.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pennylane/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/conversions.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/quil_input.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/quil_input.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pyquil/quil_output.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pyquil/quil_output.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pytket/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,22 +5,29 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-PyTKET conversions
+Qiskit conversions
 
-.. currentmodule:: qbraid.transpiler.conversions.pytket
+.. currentmodule:: qbraid.transpiler.conversions.qiskit
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   pytket_to_qasm2
-   qasm2_to_pytket
+   qasm3_to_qiskit
+   qiskit_to_qasm3
+   qasm2_to_qiskit
+   qiskit_to_qasm2
 
 """
-from qbraid.transpiler.conversions.pytket.conversions_qasm import pytket_to_qasm2, qasm2_to_pytket
+from qbraid.transpiler.conversions.qiskit.conversions_qasm import (
+    qasm2_to_qiskit,
+    qasm3_to_qiskit,
+    qiskit_to_qasm2,
+    qiskit_to_qasm3,
+)
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/pytket/conversions_qasm.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/pytket/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/qasm_passes.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qasm_passes.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/qasm_qelib1.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qasm_qelib1.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 Module that implements qelib1.inc qasm gate definitions as python functions
 
 """
 import re
 from typing import Optional
 
-from qbraid.exceptions import QasmError
+from qbraid.programs.exceptions import QasmError
 
 
 def _get_param(instr: str) -> Optional[str]:
     try:
         return instr[instr.index("(") + 1 : instr.index(")")]
     except ValueError:
         return None
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/conversions/qiskit/conversions_qasm.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/conversions/qiskit/conversions_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/converter.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,26 @@
 
 """
 import logging
 import warnings
 from copy import deepcopy
 from typing import TYPE_CHECKING, Callable, List, Optional
 
-from qbraid._qprogram import QPROGRAM_LIBS
-from qbraid.inspector import get_program_type
+from qbraid.programs import QPROGRAM_LIBS, get_program_type
 from qbraid.transpiler.exceptions import (
     CircuitConversionError,
     ConversionPathNotFoundError,
     NodeNotFoundError,
 )
 from qbraid.transpiler.graph import ConversionGraph
 
 if TYPE_CHECKING:
     import cirq
 
-    import qbraid
+    import qbraid.programs
 
 
 def _warn_if_unsupported(program_type, program_direction):
     if program_type not in QPROGRAM_LIBS:
         warnings.warn(
             f"Converting {program_direction} unsupported program type '{program_type}'.",
             UserWarning,
@@ -91,42 +90,42 @@
 
     # Add the target of the last method's instance to complete the path
     path.append(bound_methods[-1].__self__.target)
 
     return " -> ".join(path)
 
 
-def convert_to_package(
-    program: "qbraid.QPROGRAM",
+def transpile(
+    program: "qbraid.programs.QPROGRAM",
     target: str,
     conversion_graph: Optional[ConversionGraph] = None,
     max_path_attempts: int = 3,
     max_path_depth: Optional[int] = None,
-) -> "qbraid.QPROGRAM":
+) -> "qbraid.programs.QPROGRAM":
     """
     Transpile a quantum program to a target language using a conversion graph.
     This function attempts to find a conversion path from the program's current
     format to the target format. It can limit the search to a certain number of
     attempts and path depths.
 
     Args:
-        program (qbraid.QPROGRAM): The quantum program to transpile.
+        program (qbraid.programs.QPROGRAM): The quantum program to transpile.
         target (str): The target language to transpile to.
         conversion_graph (Optional[ConversionGraph]): The graph representing available conversions.
             If None, a default graph is used. Defaults to None.
         max_path_attempts (int): The maximum number of conversion paths to attempt before raising an
             exception. This is useful to avoid excessive computations when multiple paths are
             available. Defaults to 3.
         max_path_depth (Optional[int]): The maximum depth of conversions within a given path to
             allow. For example, a path with a depth of 2 would be ['cirq' -> 'qasm2' -> 'qiskit'],
             whereas a depth  of 1 would be a direct conversion ['cirq' -> 'braket']. Defaults
             to None, i.e. no limit set on the path depth.
 
     Returns:
-        qbraid.QPROGRAM: The transpiled quantum program.
+        qbraid.programs.QPROGRAM: The transpiled quantum program.
 
     Raises:
         NodeNotFoundError: If the target or source package is not in the ConversionGraph.
         ConversionPathNotFoundError: If no path is available to conversion between the
             source and target packages.
         CircuitConversionError: If the conversion fails through all attempted paths.
     """
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/edge.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/edge.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 """
 Module for defining custom conversions
 
 """
 import inspect
 from typing import TYPE_CHECKING, Any, Callable, Union
 
-from qbraid._qprogram import SUPPORTED_QPROGRAMS
-from qbraid.inspector import get_program_type
+from qbraid.programs import SUPPORTED_QPROGRAMS, get_program_type
 
 if TYPE_CHECKING:
     import qbraid
 
 
 class Conversion:
     """
@@ -86,23 +85,25 @@
 
         if module is None:
             return False
 
         package = module.__name__.split(".")[0]
         return package == "qbraid"
 
-    def convert(self, program: "qbraid.QPROGRAM") -> Union["qbraid.QPROGRAM", Any]:
+    def convert(
+        self, program: "qbraid.programs.QPROGRAM"
+    ) -> Union["qbraid.programs.QPROGRAM", Any]:
         """
         Convert a quantum program from the source package to the target package.
 
         Args:
-            program (qbraid.QPROGRAM): The quantum program to be converted.
+            program (qbraid.programs.QPROGRAM): The quantum program to be converted.
 
         Returns:
-            Union[qbraid.QPROGRAM, Any]: The converted quantum program,
+            Union[qbraid.programs.QPROGRAM, Any]: The converted quantum program,
                                          typically of a supported program type.
 
         Raises:
             ValueError: If the provided program's type does not match the source package type.
         """
         package = get_program_type(program)
         if package != self._source:
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/exceptions.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/transpiler/graph.py` & `qbraid-0.6.0.dev20240404040745/qbraid/transpiler/graph.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/visualization/__init__.py` & `qbraid-0.6.0.dev20240404040745/qbraid/visualization/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,13 +29,14 @@
 Exceptions
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    VisualizationError
+
 """
 from .draw_circuit import circuit_drawer
 from .draw_qasm3 import qasm3_drawer
 from .exceptions import VisualizationError
 from .plot_conversions import plot_conversion_graph
 from .plot_counts import plot_distribution, plot_histogram
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/visualization/draw_circuit.py` & `qbraid-0.6.0.dev20240404040745/qbraid/visualization/draw_circuit.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,43 +10,42 @@
 
 """
 Module for drawing quantum circuit diagrams
 
 """
 from typing import TYPE_CHECKING, Optional
 
-from qbraid._qprogram import QPROGRAM_LIBS
-from qbraid.exceptions import ProgramTypeError
-from qbraid.inspector import get_program_type
-from qbraid.transpiler.converter import convert_to_package
-from qbraid.visualization.draw_qasm3 import qasm3_drawer
-from qbraid.visualization.exceptions import VisualizationError
+from qbraid.programs import QPROGRAM_LIBS, ProgramTypeError, get_program_type
+from qbraid.transpiler.converter import transpile
+
+from .draw_qasm3 import qasm3_drawer
+from .exceptions import VisualizationError
 
 if TYPE_CHECKING:
-    import qbraid
+    import qbraid.programs
 
 
 def circuit_drawer(
-    program: "qbraid.QPROGRAM",
+    program: "qbraid.programs.QPROGRAM",
     as_package: Optional[str] = None,
     output: Optional[str] = None,
     **kwargs,
 ) -> None:
     """Draws circuit diagram.
 
     Args:
-        :data:`~.qbraid.QPROGRAM`: Supported quantum program
+        :data:`~.qbraid.programs.QPROGRAM`: Supported quantum program
 
     Raises:
         ProgramTypeError: If quantum program is not of a supported type
     """
     package = get_program_type(program)
 
     if as_package and as_package != package and as_package in QPROGRAM_LIBS:
-        program = convert_to_package(program, as_package)
+        program = transpile(program, as_package)
         package = as_package
 
     # pylint: disable=import-outside-toplevel
 
     if package == "qiskit":
         from qiskit.visualization import circuit_drawer as qiskit_drawer
 
@@ -105,21 +104,21 @@
 
     if package == "qasm3":
         return qasm3_drawer(program)
 
     if package == "qasm2":
         # coverage: ignore
         if "cirq" in QPROGRAM_LIBS:
-            program = convert_to_package(program, "cirq")
+            program = transpile(program, "cirq")
         elif "qiskit" in QPROGRAM_LIBS:
-            program = convert_to_package(program, "qiskit")
+            program = transpile(program, "qiskit")
         else:
-            program = convert_to_package(program, "qasm3")
+            program = transpile(program, "qasm3")
 
         return circuit_drawer(program, output=output, **kwargs)
 
     if package == "pennylane":
-        program = convert_to_package(program, "qasm2")
+        program = transpile(program, "qasm2")
 
         return circuit_drawer(program, output=output, **kwargs)
 
     raise ProgramTypeError(package)
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/visualization/draw_qasm3.py` & `qbraid-0.6.0.dev20240404040745/qbraid/visualization/draw_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/visualization/exceptions.py` & `qbraid-0.6.0.dev20240404040745/qbraid/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
+
 """
-Module for exceptions raised by visualization tools.
+Module defining exceptions for errors raised by qBraid.
 
 """
-from qbraid.exceptions import QbraidError
 
 
-class VisualizationError(QbraidError):
-    """Class for errors raised when using visualization features."""
+class QbraidError(Exception):
+    """Base class for errors raised by qBraid."""
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/visualization/plot_conversions.py` & `qbraid-0.6.0.dev20240404040745/qbraid/visualization/plot_conversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 """
 from typing import TYPE_CHECKING, Dict, Optional
 
 import matplotlib.pyplot as plt
 import networkx as nx
 
-from qbraid._qprogram import QPROGRAM_LIBS
+from qbraid.programs._import import QPROGRAM_LIBS
 
 if TYPE_CHECKING:
     import qbraid.transpiler
 
 
 def plot_conversion_graph(  # pylint: disable=too-many-arguments
     graph: "qbraid.transpiler.ConversionGraph",
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid/visualization/plot_counts.py` & `qbraid-0.6.0.dev20240404040745/qbraid/visualization/plot_counts.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid.egg-info/SOURCES.txt` & `qbraid-0.6.0.dev20240404040745/qbraid.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
-setup.cfg
-setup.py
 tox.ini
 docs/conf.py
 docs/index.rst
 docs/_static/favicon.ico
 docs/_static/logo.png
 docs/_static/cards/jupyter.png
 docs/_static/cards/python.png
@@ -26,15 +24,14 @@
 docs/_static/pkg-logos/quantinuum.png
 docs/_static/sdk-files/batch_counts.png
 docs/_static/sdk-files/conversion_graph.png
 docs/_static/sdk-files/get_devices.png
 docs/_static/sdk-files/hub_spokes.png
 docs/_static/sdk-files/lab_jobs.png
 docs/_static/sdk-files/plot_counts.png
-docs/api/qbraid.api.rst
 docs/api/qbraid.compiler.rst
 docs/api/qbraid.interface.rst
 docs/api/qbraid.programs.rst
 docs/api/qbraid.providers.rst
 docs/api/qbraid.rst
 docs/api/qbraid.transpiler.rst
 docs/api/qbraid.visualization.rst
@@ -45,57 +42,53 @@
 docs/sdk/providers.rst
 docs/sdk/results.rst
 docs/sdk/transpiler.rst
 qbraid/__init__.py
 qbraid/_about.py
 qbraid/_display.py
 qbraid/_import.py
-qbraid/_qdevice.py
-qbraid/_qprogram.py
 qbraid/_version.py
 qbraid/_warnings.py
 qbraid/exceptions.py
 qbraid/get_devices.py
 qbraid/get_jobs.py
-qbraid/inspector.py
-qbraid/load_program.py
-qbraid/load_provider.py
 qbraid.egg-info/PKG-INFO
 qbraid.egg-info/SOURCES.txt
 qbraid.egg-info/dependency_links.txt
 qbraid.egg-info/entry_points.txt
 qbraid.egg-info/requires.txt
 qbraid.egg-info/top_level.txt
-qbraid/api/__init__.py
-qbraid/api/exceptions.py
-qbraid/api/retry.py
-qbraid/api/session.py
-qbraid/api/system.py
 qbraid/compiler/__init__.py
 qbraid/compiler/exceptions.py
 qbraid/compiler/braket/__init__.py
 qbraid/compiler/braket/ionq.py
 qbraid/interface/__init__.py
 qbraid/interface/circuit_equality.py
 qbraid/interface/random/__init__.py
 qbraid/interface/random/cirq_random.py
 qbraid/interface/random/qasm3_random.py
 qbraid/interface/random/qiskit_random.py
 qbraid/interface/random/random.py
 qbraid/programs/__init__.py
+qbraid/programs/_import.py
 qbraid/programs/abc_program.py
-qbraid/programs/braket.py
-qbraid/programs/cirq.py
-qbraid/programs/pennylane.py
-qbraid/programs/pyquil.py
-qbraid/programs/pytket.py
-qbraid/programs/qasm2.py
-qbraid/programs/qasm3.py
-qbraid/programs/qiskit.py
+qbraid/programs/exceptions.py
+qbraid/programs/inspector.py
+qbraid/programs/loader.py
+qbraid/programs/libs/__init__.py
+qbraid/programs/libs/braket.py
+qbraid/programs/libs/cirq.py
+qbraid/programs/libs/pennylane.py
+qbraid/programs/libs/pyquil.py
+qbraid/programs/libs/pytket.py
+qbraid/programs/libs/qasm2.py
+qbraid/programs/libs/qasm3.py
+qbraid/programs/libs/qiskit.py
 qbraid/providers/__init__.py
+qbraid/providers/_import.py
 qbraid/providers/device.py
 qbraid/providers/enums.py
 qbraid/providers/exceptions.py
 qbraid/providers/job.py
 qbraid/providers/provider.py
 qbraid/providers/result.py
 qbraid/providers/status_maps.py
@@ -141,69 +134,9 @@
 qbraid/transpiler/conversions/qiskit/conversions_qasm.py
 qbraid/visualization/__init__.py
 qbraid/visualization/draw_circuit.py
 qbraid/visualization/draw_qasm3.py
 qbraid/visualization/exceptions.py
 qbraid/visualization/plot_conversions.py
 qbraid/visualization/plot_counts.py
-tests/__init__.py
-tests/conftest.py
-tests/benchmarking/__init__.py
-tests/benchmarking/qaps.py
-tests/benchmarking/qiskit_to_braket.py
-tests/compiler/__init__.py
-tests/compiler/test_braket_compiler.py
-tests/fixtures/__init__.py
-tests/interface/__init__.py
-tests/interface/test_conversion_edge.py
-tests/interface/test_conversion_grah.py
-tests/interface/test_converter.py
-tests/interface/test_inspector.py
-tests/programs/__init__.py
-tests/programs/test_abc_program.py
-tests/programs/test_braket_program.py
-tests/programs/test_circuit_equality.py
-tests/programs/test_cirq_program.py
-tests/programs/test_pennylane_program.py
-tests/programs/test_pytket_program.py
-tests/programs/test_qasm2_program.py
-tests/programs/test_qasm3_program.py
-tests/programs/test_qiskit_program.py
-tests/providers/__init__.py
-tests/providers/conftest.py
-tests/providers/fixtures.py
-tests/providers/test_braket_device.py
-tests/providers/test_braket_provider.py
-tests/providers/test_braket_tracker.py
-tests/providers/test_datetime_helpers.py
-tests/providers/test_qiskit_backend.py
-tests/providers/test_qiskit_provider.py
-tests/providers/test_quantum_jobs.py
-tests/providers/test_quantum_results.py
-tests/transpiler/__init__.py
-tests/transpiler/cirq_utils.py
-tests/transpiler/test_idle_qubits.py
-tests/transpiler/test_qasm2_preprocess.py
-tests/transpiler/test_transpiler.py
-tests/transpiler/coverage/__init__.py
-tests/transpiler/coverage/test_coverage_from_braket.py
-tests/transpiler/coverage/test_coverage_from_cirq.py
-tests/transpiler/coverage/test_coverage_from_pyquil.py
-tests/transpiler/coverage/test_coverage_from_pytket.py
-tests/transpiler/coverage/test_coverage_from_qiskit.py
-tests/transpiler/pytket/__init__.py
-tests/transpiler/pytket/test_conversions_pytket.py
-tests/transpiler/pytket/test_from_pytket.py
-tests/transpiler/pytket/test_to_pytket.py
-tests/transpiler/qasm/__init__.py
-tests/transpiler/qasm/test_conversions_qasm3.py
-tests/transpiler/qasm/test_qasm2_to_qasm3.py
-tests/transpiler/qiskit/__init__.py
-tests/transpiler/qiskit/test_conversions_qiskit.py
-tests/transpiler/qiskit/test_from_qiskit.py
-tests/transpiler/qiskit/test_qiskit_qasm.py
-tests/transpiler/qiskit/test_to_qiskit.py
-tests/visualization/__init__.py
-tests/visualization/test_circuit_drawer.py
-tests/visualization/test_plot_counts.py
-tests/visualization/test_qasm3_circuit_drawer.py
+tools/set_provider_configs.py
 tools/verify_headers.py
```

### Comparing `qbraid-0.5.3.dev20240312235736/qbraid.egg-info/requires.txt` & `qbraid-0.6.0.dev20240404040745/qbraid.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 networkx<4.0,>=2.5
 numpy<1.27,>=1.17
 openqasm3[parser]<0.6.0,>=0.4.0
 ply>=3.6
-requests>=2.28.0
-
-[all]
-amazon-braket-sdk<1.74.0,>=1.42.1
-cirq-core<1.4.0,>=1.3.0
-cirq-ionq<1.4.0,>=1.3.0
-pennylane<0.36.0,>=0.33.1
-pytket<1.26.0,>=1.16.0
-pytket-braket<0.35.0,>=0.30.0
-pyquil<4.5.0,>=3.5.4
-qiskit<1.1.0,>=0.44.0
-qiskit-ibm-provider<0.11.0,>=0.5.3
-qiskit-ibm-runtime<0.21.0,>=0.18.0
-qiskit-qasm3-import<0.5.0,>=0.2.0
+qbraid-core==0.1.0.dev3
 
 [braket]
-amazon-braket-sdk<1.74.0,>=1.42.1
+amazon-braket-sdk<1.77.0,>=1.42.1
 
 [cirq]
 cirq-core<1.4.0,>=1.3.0
 
 [docs]
 sphinx~=7.2.6
 sphinx-autodoc-typehints<2.1,>=1.24
 sphinx-rtd-theme<2.1,>=1.3
 docutils<0.21
 
 [ionq]
 cirq-core<1.4.0,>=1.3.0
 cirq-ionq<1.4.0,>=1.3.0
-pytket-braket<0.35.0,>=0.30.0
+pytket-braket<0.36.0,>=0.30.0
+
+[lint]
+black
+isort
+pylint
 
 [pennylane]
 pennylane<0.36.0,>=0.33.1
 
 [pyquil]
 pyquil<4.4.0,>=3.5.4
 
 [pytket]
-pytket<1.26.0,>=1.16.0
+pytket<1.27.0,>=1.16.0
 
-[qasm3]
-qiskit-qasm3-import<0.5.0,>=0.2.0
+[qir]
+qbraid-qir<0.2.0,>=0.1.1
 
 [qiskit]
 qiskit<1.1.0,>=0.44.0
 qiskit-ibm-provider<0.11.0,>=0.5.3
 qiskit-ibm-runtime<0.21.0,>=0.18.0
+qiskit[visualization]
+
+[test]
+qbraid~=0.5.3
+pytest
+pytest-cov
 
 [visualization]
 ipython
 matplotlib
 pylatexenc
-qiskit[visualization]
```

### Comparing `qbraid-0.5.3.dev20240312235736/tools/verify_headers.py` & `qbraid-0.6.0.dev20240404040745/tools/verify_headers.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.5.3.dev20240312235736/tox.ini` & `qbraid-0.6.0.dev20240404040745/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -11,38 +11,36 @@
 [testenv]
 package = editable-legacy
 basepython = python3
 deps =
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/requirements-dev.txt
 pass_env =
-    JUPYTERHUB_USER
-    REFRESH
     QBRAID_API_KEY
     AWS_ACCESS_KEY_ID
     AWS_SECRET_ACCESS_KEY
     QISKIT_IBM_TOKEN
     QBRAID_RUN_REMOTE_TESTS
 
 [testenv:unit-tests]
 description = Run pytests and generate coverage report.
 commands =
-    coverage run -m pytest -x tests/api \
-                              tests/programs \
+    python3 tools/set_provider_configs.py
+    coverage run -m pytest -x tests/programs \
                               tests/transpiler \
                               tests/providers \
                               tests/compiler \
                               tests/visualization \
                               tests/top_level \
                            -W ignore::DeprecationWarning \
                            -W ignore::PendingDeprecationWarning \
                            -W ignore::urllib3.exceptions.InsecureRequestWarning \
                            -W ignore::RuntimeWarning
     coverage combine
-    coverage report --omit=qbraid/transpiler/conversions/cirq/cirq_gates.py,qbraid/visualization/draw_circuit.py,qbraid/visualization/plot_conversions.py,qbraid/api/retry.py,qbraid/api/system.py
+    coverage report --omit=qbraid/transpiler/conversions/cirq/cirq_gates.py,qbraid/visualization/draw_circuit.py,qbraid/visualization/plot_conversions.py
     coverage html
     coverage xml
 
 [testenv:docs]
 description = Use sphinx to build the HTML docs.
 extras =
     docs
```

