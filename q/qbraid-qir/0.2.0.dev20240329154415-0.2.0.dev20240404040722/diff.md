# Comparing `tmp/qbraid-qir-0.2.0.dev20240329154415.tar.gz` & `tmp/qbraid-qir-0.2.0.dev20240404040722.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-qir-0.2.0.dev20240329154415.tar", last modified: Fri Mar 29 15:44:17 2024, max compression
+gzip compressed data, was "qbraid-qir-0.2.0.dev20240404040722.tar", last modified: Thu Apr  4 04:07:24 2024, max compression
```

## Comparing `qbraid-qir-0.2.0.dev20240329154415.tar` & `qbraid-qir-0.2.0.dev20240404040722.tar`

### file list

```diff
@@ -1,56 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.651749 qbraid-qir-0.2.0.dev20240329154415/
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49005 2024-03-29 15:44:17.651749 qbraid-qir-0.2.0.dev20240329154415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.643749 qbraid-qir-0.2.0.dev20240329154415/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.643749 qbraid-qir-0.2.0.dev20240329154415/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.647749 qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    32358 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/qbraid.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/qosf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.647749 qbraid-qir-0.2.0.dev20240329154415/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/api/qbraid_qir.cirq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/api/qbraid_qir.qasm3.rst
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/api/qbraid_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.647749 qbraid-qir-0.2.0.dev20240329154415/docs/userguide/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/userguide/cirq_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/userguide/qasm3_qir.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/docs/userguide/qasm3_supported.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.647749 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-29 15:44:15.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.651749 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/opsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.651749 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/oq3_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    30899 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.651749 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49005 2024-03-29 15:44:17.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-29 15:44:17.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:44:17.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-29 15:44:17.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 15:44:17.000000 qbraid-qir-0.2.0.dev20240329154415/qbraid_qir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 15:44:17.651749 qbraid-qir-0.2.0.dev20240329154415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:44:17.651749 qbraid-qir-0.2.0.dev20240329154415/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5074 2024-03-29 15:44:11.000000 qbraid-qir-0.2.0.dev20240329154415/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49026 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.709945 qbraid-qir-0.2.0.dev20240404040722/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.709945 qbraid-qir-0.2.0.dev20240404040722/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.709945 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32358 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qbraid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qosf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.709945 qbraid-qir-0.2.0.dev20240404040722/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/api/qbraid_qir.cirq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/api/qbraid_qir.qasm3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/api/qbraid_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/api/qbraid_qir.runner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.713945 qbraid-qir-0.2.0.dev20240404040722/docs/userguide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/userguide/cirq_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/userguide/qasm3_qir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/docs/userguide/qasm3_supported.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.713945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 04:07:22.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.713945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/opsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.713945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/oq3_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30831 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/runner/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49026 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 04:07:24.000000 qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:07:24.717945 qbraid-qir-0.2.0.dev20240404040722/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5254 2024-04-04 04:07:19.000000 qbraid-qir-0.2.0.dev20240404040722/tools/verify_headers.py
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/CODE_OF_CONDUCT.md` & `qbraid-qir-0.2.0.dev20240404040722/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/CONTRIBUTING.md` & `qbraid-qir-0.2.0.dev20240404040722/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/LICENSE` & `qbraid-qir-0.2.0.dev20240404040722/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/PKG-INFO` & `qbraid-qir-0.2.0.dev20240404040722/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-qir
-Version: 0.2.0.dev20240329154415
+Version: 0.2.0.dev20240404040722
 Summary: qBraid-SDK extension providing support for QIR conversions.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,14 +696,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyqir~=0.10.0
+Requires-Dist: numpy
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: qasm3
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0; extra == "qasm3"
 Provides-Extra: test
 Requires-Dist: qbraid~=0.5.3; extra == "test"
 Requires-Dist: pytest; extra == "test"
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/README.md` & `qbraid-qir-0.2.0.dev20240404040722/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/_static/favicon.ico` & `qbraid-qir-0.2.0.dev20240404040722/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/_static/logo.png` & `qbraid-qir-0.2.0.dev20240404040722/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/cirq.png` & `qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/qbraid.png` & `qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qbraid.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/qir.png` & `qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/_static/pkg-logos/qosf.png` & `qbraid-qir-0.2.0.dev20240404040722/docs/_static/pkg-logos/qosf.png`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/conf.py` & `qbraid-qir-0.2.0.dev20240404040722/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/index.rst` & `qbraid-qir-0.2.0.dev20240404040722/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,15 @@
    :maxdepth: 1
    :caption: API Reference
    :hidden:
 
    api/qbraid_qir
    api/qbraid_qir.cirq
    api/qbraid_qir.qasm3
+   api/qbraid_qir.runner
 
 
 Indices and Tables
 ------------------
 
 * :ref:`genindex`
 * :ref:`modindex`
```

#### html2text {}

```diff
@@ -33,9 +33,10 @@
 align: middle :width: 100px :target: qBraid_ .. |cirq| image:: _static/pkg-
 logos/cirq.png :align: middle :width: 100px :target: Cirq_ .. |qosf| image::
 _static/pkg-logos/qosf.png :align: middle :width: 100px :target: QOSF_ .. _QIR:
 https://www.qir-alliance.org/ .. _qBraid: https://docs.qbraid.com/en/latest/ ..
 _Cirq: https://quantumai.google/cirq .. _QOSF: https://qosf.org/ | .. toctree::
 :maxdepth: 1 :caption: User Guide :hidden: userguide/cirq_qir userguide/
 qasm3_qir userguide/qasm3_supported .. toctree:: :maxdepth: 1 :caption: API
-Reference :hidden: api/qbraid_qir api/qbraid_qir.cirq api/qbraid_qir.qasm3
-Indices and Tables ------------------ * :ref:`genindex` * :ref:`modindex`
+Reference :hidden: api/qbraid_qir api/qbraid_qir.cirq api/qbraid_qir.qasm3 api/
+qbraid_qir.runner Indices and Tables ------------------ * :ref:`genindex` * :
+ref:`modindex`
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/userguide/cirq_qir.rst` & `qbraid-qir-0.2.0.dev20240404040722/docs/userguide/cirq_qir.rst`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/userguide/qasm3_qir.rst` & `qbraid-qir-0.2.0.dev20240404040722/docs/userguide/qasm3_qir.rst`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/docs/userguide/qasm3_supported.rst` & `qbraid-qir-0.2.0.dev20240404040722/docs/userguide/qasm3_supported.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 QASM support
 ==================
 
 Currently Supported Constructs
 ------------------------------
 
-The qasm3 to QIR converter supports the following openqasm constructrs - 
+The ``qbraid_qir.qasm3.qasm3_to_qir()`` converter supports the following OpenQASM 3 constructs:
 
-1. **Register Declarations** : Openqasm declarations of all forms ``qreg``, ``qubit``, ``bit`` and ``creg`` are supported. 
+1. **Register Declarations** : OpenQASM declarations of all forms ``qreg``, ``qubit``, ``bit`` and ``creg`` are supported. 
 
 2. **QuantumMeasurements** : Openqasm measurements are supported which involve single qubit measurement and full register measurements. Range based measurements are not supported currently.
 
 .. code-block:: c
 
     OPENQASM 3;
 
@@ -33,15 +33,15 @@
 
 3. **QuantumReset** : Resets are supported on declared quantum registers in all forms.
 
 
 4. **QuantumGates** : **pyqir._native** gates are supported alongwith support for ``U3`` and ``U2`` gates. The U[x] gates are defined in the terms of existing ``rx`` and ``rz`` gates according to the decomposition present on the qiskit website - https://docs.quantum.ibm.com/api/qiskit/qiskit.circuit.library.UGate, https://docs.quantum.ibm.com/api/qiskit/qiskit.circuit.library.PhaseGate
 
 
-5. **QuantumBarriers** : Barriers are supported only if they are placed on ALL the qubits in the circuit. Eg. - 
+5. **QuantumBarriers** : Barriers are supported only if they are placed on ALL the qubits in the circuit. For example: 
 
 .. code-block:: c
 
     qubit q[2];
 
     U(0.1, 0.2, 0.3) q[0];
 
@@ -79,15 +79,15 @@
     }
 
     qubit[2] q;
     custom(2 + 3 - 1/5, 0.1, 0.3) q[0], q[1];
 
 
 
-7. **Simple Branching Statements** (controlled on 1 bit) : Since QIR supports branching on a measurement result, single bit branching statements are supported at the moment. General boolean expressions and support for branching on full registers will be added in future. Example - 
+7. **Simple Branching Statements** (controlled on 1 bit) : Since QIR supports branching on a measurement result, single bit branching statements are supported at the moment. General boolean expressions and support for branching on full registers will be added in future. For example: 
 
 .. code-block:: c
 
     OPENQASM 3;
     include "stdgates.inc";
     qubit[4] q;
     bit[4] c;
@@ -114,15 +114,15 @@
     // ERROR : not supported
     int[4] element;
     if(element > 5){
         y q[1];
     }
 
 
-8.  **Expressions** : General expression evaluation involving literals and constants is supported. Example - 
+8.  **Expressions** : General expression evaluation involving literals and constants is supported. For example: 
 
 .. code-block:: c 
 
     OPENQASM 3;
     qubit q;
 
     // supported
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/pyproject.toml` & `qbraid-qir-0.2.0.dev20240404040722/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics"
 ]
-dependencies = ["pyqir~=0.10.0"]
+dependencies = ["pyqir~=0.10.0", "numpy"]
 requires-python = ">= 3.8"
 
 [project.urls]
 Homepage = "https://github.com/qBraid/qbraid-qir"
 Documentation = "https://docs.qbraid.com/projects/qir/en/stable/"
 "Bug Tracker" = "https://github.com/qBraid/qbraid-qir/issues"
 Discord = "https://discord.gg/TPBU2sa8Et"
@@ -64,8 +64,16 @@
   "pass",
   "raise NotImplementedError",
   "return NotImplemented",
   "def __repr__",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "logger.debug"
+]
+
+[tool.coverage.run]
+parallel = true
+source = ["qbraid_qir"]
+omit = [
+  "**/qbraid_qir/runner/simulator.py",
+  "**/qbraid_qir/__init__.py"
 ]
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/__init__.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    dumps
 
+
 Exceptions
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    QbraidQirError
@@ -38,15 +39,15 @@
 __all__ = [
     "__version__",
     "QbraidQirError",
     "QirConversionError",
     "dumps",
 ]
 
-_lazy_mods = ["cirq", "qasm3"]
+_lazy_mods = ["cirq", "qasm3", "runner"]
 
 
 def __getattr__(name):
     if name in _lazy_mods:
         import importlib  # pylint: disable=import-outside-toplevel
 
         module = importlib.import_module(f".{name}", __name__)
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/__init__.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 Classes
 ---------
 
 .. autosummary::
    :toctree: ../stubs/
 
    CirqModule
-   BasicQisVisitor
+   BasicCirqVisitor
 
 Exceptions
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    CirqConversionError
 
 """
 from .convert import cirq_to_qir
 from .elements import CirqModule
 from .exceptions import CirqConversionError
-from .visitor import BasicQisVisitor
+from .visitor import BasicCirqVisitor
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/convert.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import cirq
 from pyqir import Context, Module, qir_module
 
 from .elements import CirqModule, generate_module_id
 from .exceptions import CirqConversionError
 from .passes import preprocess_circuit
-from .visitor import BasicQisVisitor
+from .visitor import BasicCirqVisitor
 
 
 def cirq_to_qir(circuit: cirq.Circuit, name: Optional[str] = None, **kwargs) -> Module:
     """
     Converts a Cirq circuit to a PyQIR module.
 
     Args:
@@ -57,14 +57,14 @@
         circuit = preprocess_circuit(circuit)
     except Exception as err:  # pylint: disable=broad-exception-caught
         raise CirqConversionError("Failed to preprocess circuit.") from err
 
     llvm_module = qir_module(Context(), name)
     module = CirqModule.from_circuit(circuit, llvm_module)
 
-    visitor = BasicQisVisitor(**kwargs)
+    visitor = BasicCirqVisitor(**kwargs)
     module.accept(visitor)
 
     err = llvm_module.verify()
     if err is not None:
         raise CirqConversionError(err)
     return llvm_module
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/elements.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/elements.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/exceptions.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/opsets.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/opsets.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/passes.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/passes.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/cirq/visitor.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/cirq/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         pass
 
     @abstractmethod
     def visit_operation(self, operation):
         pass
 
 
-class BasicQisVisitor(CircuitElementVisitor):
-    """A visitor for QIS (Quantum Instruction Set) basic elements.
+class BasicCirqVisitor(CircuitElementVisitor):
+    """A visitor for basic cirq.Circuit elements.
 
     This class is designed to traverse and interact with elements in a quantum circuit.
 
     Args:
         initialize_runtime (bool): If True, quantum runtime will be initialized. Defaults to True.
         record_output (bool): If True, output of the circuit will be recorded. Defaults to True.
     """
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/exceptions.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/__init__.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 Classes
 ---------
 
 .. autosummary::
    :toctree: ../stubs/
 
    Qasm3Module
-   BasicQisVisitor
+   BasicQasmVisitor
 
 
 Exceptions
 -----------
 
 .. autosummary::
    :toctree: ../stubs/
 
    Qasm3ConversionError
 
 """
 from .convert import qasm3_to_qir
 from .elements import Qasm3Module
 from .exceptions import Qasm3ConversionError
-from .visitor import BasicQisVisitor
+from .visitor import BasicQasmVisitor
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/convert.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Optional, Union
 
 import openqasm3
 from pyqir import Context, Module, qir_module
 
 from .elements import Qasm3Module, generate_module_id
 from .exceptions import Qasm3ConversionError
-from .visitor import BasicQisVisitor
+from .visitor import BasicQasmVisitor
 
 
 def qasm3_to_qir(
     program: Union[openqasm3.ast.Program, str], name: Optional[str] = None, **kwargs
 ) -> Module:
     """Converts an OpenQASM 3 program to a PyQIR module.
 
@@ -51,14 +51,14 @@
 
     if name is None:
         name = generate_module_id()
 
     llvm_module = qir_module(Context(), name)
     module = Qasm3Module.from_program(program, llvm_module)
 
-    visitor = BasicQisVisitor(**kwargs)
+    visitor = BasicQasmVisitor(**kwargs)
     module.accept(visitor)
 
     err = llvm_module.verify()
     if err is not None:
         raise Qasm3ConversionError(err)
     return llvm_module
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/elements.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,44 +12,46 @@
 Module defining Qasm3 Converter elements.
 
 """
 
 import uuid
 from abc import ABCMeta, abstractmethod
 from enum import Enum
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from openqasm3.ast import BitType, ClassicalDeclaration, Program, QubitDeclaration, Statement
 from pyqir import Context as qirContext
 from pyqir import Module
 
 
 def generate_module_id() -> str:
     """
     Generates a QIR module ID from a given openqasm3 program.
-    """
 
+    """
     # TODO: Consider a better approach of generating a unique identifier.
     generated_id = uuid.uuid1()
-    return f"circuit-{generated_id}"
+    return f"program-{generated_id}"
 
 
 class Scope(Enum):
     """
     Enum for the different scopes in QIR.
+
     """
 
     GLOBAL = "global"
     GATE = "gate"
     FUNCTION = "function"
 
 
 class Context(Enum):
     """
     Enum for the different contexts in QIR.
+
     """
 
     GLOBAL = "global"
     IF = "if"
     LOOP = "loop"
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/exceptions.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/oq3_maps.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/oq3_maps.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/qasm3/visitor.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/qasm3/visitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,68 +19,65 @@
 from abc import ABCMeta, abstractmethod
 from typing import Any, List, Optional, Tuple, Union
 
 import pyqir
 import pyqir._native
 import pyqir.rt
 from openqasm3.ast import (
+    AliasStatement,
     BinaryExpression,
     BooleanLiteral,
     BranchingStatement,
     ClassicalDeclaration,
     DurationLiteral,
     FloatLiteral,
-    FloatType,
     Identifier,
     ImaginaryLiteral,
     Include,
     IndexedIdentifier,
     IndexExpression,
     IntegerLiteral,
-)
-from openqasm3.ast import IntType as qasm3IntType
-from openqasm3.ast import (
+    IODeclaration,
     QuantumBarrier,
     QuantumGate,
     QuantumGateDefinition,
     QuantumMeasurementStatement,
     QuantumReset,
     QubitDeclaration,
     RangeDefinition,
     Span,
     Statement,
     SubroutineDefinition,
-    UintType,
     UnaryExpression,
 )
 from pyqir import BasicBlock, Builder, Constant
 from pyqir import IntType as qirIntType
 from pyqir import PointerType
 
 from .elements import Context, Qasm3Module, Scope
 from .exceptions import Qasm3ConversionError
 from .oq3_maps import map_qasm_op_to_pyqir_callable, qasm3_constants_map, qasm3_expression_op_map
 
 _log = logging.getLogger(name=__name__)
 
 
-class CircuitElementVisitor(metaclass=ABCMeta):
+class ProgramElementVisitor(metaclass=ABCMeta):
     @abstractmethod
-    def visit_register(self, register, is_qubit):
+    def visit_register(self, register):
         pass
 
     @abstractmethod
     def visit_statement(self, statement):
         pass
 
 
-class BasicQisVisitor(CircuitElementVisitor):
-    """A visitor for QIS (Quantum Instruction Set) basic elements.
+class BasicQasmVisitor(ProgramElementVisitor):
+    """A visitor for basic OpenQASM program elements.
 
-    This class is designed to traverse and interact with elements in a quantum circuit.
+    This class is designed to traverse and interact with elements in an OpenQASM program.
 
     Args:
         initialize_runtime (bool): If True, quantum runtime will be initialized. Defaults to True.
         record_output (bool): If True, output of the circuit will be recorded. Defaults to True.
     """
 
     def __init__(self, initialize_runtime: bool = True, record_output: bool = True):
@@ -551,20 +548,14 @@
             # necessary to avoid modifying the original gate definition
             # in case the gate is reapplied
             gate_op_copy = copy.deepcopy(gate_op)
             if isinstance(gate_op, QuantumGate):
                 self._transform_gate_params(gate_op_copy, param_map)
                 self._transform_gate_qubits(gate_op_copy, qubit_map)
                 self._visit_generic_gate_operation(gate_op_copy)
-            elif isinstance(gate_op, QuantumMeasurementStatement):
-                self._print_err_location(gate_op.span)
-                raise Qasm3ConversionError("Unsupported measurement statement in gate definition")
-            elif isinstance(gate_op, QuantumReset):
-                self._print_err_location(gate_op.span)
-                raise Qasm3ConversionError("Unsupported reset statement in gate definition")
             else:
                 # TODO: add control flow support
                 self._print_err_location(gate_op.span)
                 raise Qasm3ConversionError(f"Unsupported gate definition statement {gate_op}")
 
     def _visit_generic_gate_operation(self, operation: QuantumGate) -> None:
         """Visit a gate operation element.
@@ -587,14 +578,15 @@
             statement (ClassicalType): The classical operation to visit.
 
         Returns:
             None
         """
         raise NotImplementedError("Classical declarations not yet supported")
 
+    # pylint: disable-next=too-many-return-statements
     def _evaluate_expression(self, expression: Any) -> bool:
         """Evaluate an expression.
 
         Args:
             expression (Any): The expression to evaluate.
 
         Returns:
@@ -618,38 +610,41 @@
                 self._print_err_location(expression.span)
                 raise Qasm3ConversionError(
                     f"Undefined identifier {expression.name} in {expression}"
                 ) from err
 
         if isinstance(expression, BooleanLiteral):
             return expression.value
-        elif isinstance(expression, (IntegerLiteral, FloatLiteral)):
+        if isinstance(expression, (IntegerLiteral, FloatLiteral)):
             return expression.value
-        elif isinstance(expression, UnaryExpression):
+        if isinstance(expression, UnaryExpression):
             op = expression.op.name
             if op == "!":
                 return not self._evaluate_expression(expression.expression)
-            elif op == "-":
+            if op == "-":
                 return -1 * self._evaluate_expression(expression.expression)
-            elif op == "~":
+            if op == "~":
                 value = self._evaluate_expression(expression.expression)
                 if not isinstance(value, int):
                     self._print_err_location(expression.span)
                     raise Qasm3ConversionError(
                         f"Unsupported expression type {type(value)} in ~ operation"
                     )
                 return ~value
-        elif isinstance(expression, BinaryExpression):
+            raise Qasm3ConversionError(
+                f"Unsupported UnaryExpression operation: {op}. Expected one of ['!', '-', '~']"
+            )
+        if isinstance(expression, BinaryExpression):
             lhs = self._evaluate_expression(expression.lhs)
             op = expression.op.name
             rhs = self._evaluate_expression(expression.rhs)
             return qasm3_expression_op_map(op, lhs, rhs)
-        else:
-            self._print_err_location(expression.span)
-            raise Qasm3ConversionError(f"Unsupported expression type {type(expression)}")
+
+        self._print_err_location(expression.span)
+        raise Qasm3ConversionError(f"Unsupported expression type {type(expression)}")
 
     def _analyse_branch_condition(self, condition) -> bool:
         """
         Analyse the branching condition to determine the branch to take
 
         Args:
             condition (Any): The condition to analyse
@@ -773,17 +768,21 @@
             self._visit_generic_gate_operation(statement)
         elif isinstance(statement, ClassicalDeclaration):
             self._visit_classical_operation(statement)
         elif isinstance(statement, BranchingStatement):
             self._visit_branching_statement(statement)
         elif isinstance(statement, SubroutineDefinition):
             raise NotImplementedError("OpenQASM 3 subroutines not yet supported")
+        elif isinstance(statement, AliasStatement):
+            raise NotImplementedError("OpenQASM 3 aliases not yet supported")
+        elif isinstance(statement, IODeclaration):
+            raise NotImplementedError("OpenQASM 3 IO declarations not yet supported")
         else:
             # TODO : extend this
             self._print_err_location(statement.span)
-            raise Qasm3ConversionError(f"Unsupported statement type {type(statement)}")
+            raise Qasm3ConversionError(f"Unsupported statement of type {type(statement)}")
 
     def ir(self) -> str:
         return str(self._module)
 
     def bitcode(self) -> bytes:
         return self._module.bitcode()
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir/serialization.py` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir/serialization.py`

 * *Files identical despite different names*

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir.egg-info/PKG-INFO` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-qir
-Version: 0.2.0.dev20240329154415
+Version: 0.2.0.dev20240404040722
 Summary: qBraid-SDK extension providing support for QIR conversions.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,14 +696,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyqir~=0.10.0
+Requires-Dist: numpy
 Provides-Extra: cirq
 Requires-Dist: cirq-core<1.4.0,>=1.3.0; extra == "cirq"
 Provides-Extra: qasm3
 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0; extra == "qasm3"
 Provides-Extra: test
 Requires-Dist: qbraid~=0.5.3; extra == "test"
 Requires-Dist: pytest; extra == "test"
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/qbraid_qir.egg-info/SOURCES.txt` & `qbraid-qir-0.2.0.dev20240404040722/qbraid_qir.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 docs/_static/pkg-logos/cirq.png
 docs/_static/pkg-logos/qbraid.png
 docs/_static/pkg-logos/qir.png
 docs/_static/pkg-logos/qosf.png
 docs/api/qbraid_qir.cirq.rst
 docs/api/qbraid_qir.qasm3.rst
 docs/api/qbraid_qir.rst
+docs/api/qbraid_qir.runner.rst
 docs/userguide/cirq_qir.rst
 docs/userguide/qasm3_qir.rst
 docs/userguide/qasm3_supported.rst
 qbraid_qir/__init__.py
 qbraid_qir/_version.py
 qbraid_qir/exceptions.py
 qbraid_qir/serialization.py
@@ -36,8 +37,12 @@
 qbraid_qir/cirq/visitor.py
 qbraid_qir/qasm3/__init__.py
 qbraid_qir/qasm3/convert.py
 qbraid_qir/qasm3/elements.py
 qbraid_qir/qasm3/exceptions.py
 qbraid_qir/qasm3/oq3_maps.py
 qbraid_qir/qasm3/visitor.py
+qbraid_qir/runner/__init__.py
+qbraid_qir/runner/exceptions.py
+qbraid_qir/runner/result.py
+qbraid_qir/runner/simulator.py
 tools/verify_headers.py
```

### Comparing `qbraid-qir-0.2.0.dev20240329154415/tools/verify_headers.py` & `qbraid-qir-0.2.0.dev20240404040722/tools/verify_headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,34 @@
 import sys
 
 # ANSI escape codes
 BLUE = "\033[94m"
 BOLD = "\033[1m"
 RESET = "\033[0m"
 
-header = """# Copyright (C) 2023 qBraid
+header = """# Copyright (C) 2024 qBraid
 #
 # This file is part of the qBraid-SDK
 #
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 """
 
+header_2023 = header.replace("2024", "2023")
+
 skip_files = []
 
 failed_headers = []
 fixed_headers = []
 
 
-def should_skip(file_path, content):
+def should_skip(file_path: str, content: str) -> bool:
     if file_path in skip_files:
         return True
 
     if os.path.basename(file_path) == "__init__.py":
         return not content.strip()
 
     skip_header_tag = "# qbraid: skip-header"
@@ -55,19 +57,23 @@
             return True
         if line_number > 30:
             break
 
     return False
 
 
-def replace_or_add_header(file_path, fix=False):
+def replace_or_add_header(file_path: str, fix: bool = False) -> None:
     with open(file_path, "r", encoding="ISO-8859-1") as f:
         content = f.read()
 
-    if content.startswith(header) or should_skip(file_path, content):
+    if (
+        content.startswith(header)
+        or content.startswith(header_2023)
+        or should_skip(file_path, content)
+    ):
         return
 
     if not fix:
         failed_headers.append(file_path)
         return
 
     lines = content.splitlines()
@@ -86,26 +92,26 @@
 
     with open(file_path, "w", encoding="ISO-8859-1") as f:
         f.write(new_content)
 
     fixed_headers.append(file_path)
 
 
-def process_files_in_directory(directory, fix=False):
+def process_files_in_directory(directory: str, fix: bool = False) -> int:
     count = 0
     for root, _, files in os.walk(directory):
         for file in files:
             if file.endswith(".py"):
                 file_path = os.path.join(root, file)
                 replace_or_add_header(file_path, fix)
                 count += 1
     return count
 
 
-def display_help():
+def display_help() -> None:
     help_message = """
     Usage: python verify_headers.py SRC [OPTIONS] ...
 
     This script checks for copyright headers at the specified path.
     If no flags are passed, it will indicate which files would be
     modified without actually making any changes.
```

