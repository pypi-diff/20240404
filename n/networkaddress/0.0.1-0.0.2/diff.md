# Comparing `tmp/networkaddress-0.0.1.tar.gz` & `tmp/networkaddress-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkaddress-0.0.1.tar", last modified: Sat Sep 30 12:00:59 2023, max compression
+gzip compressed data, was "networkaddress-0.0.2.tar", last modified: Fri Jan 26 02:37:49 2024, max compression
```

## Comparing `networkaddress-0.0.1.tar` & `networkaddress-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,92 @@
-drwxr-xr-x   0 duynha    (1000) duynha    (1000)        0 2023-09-30 12:00:59.297510 networkaddress-0.0.1/
--rw-r--r--   0 duynha    (1000) duynha    (1000)     1078 2023-09-30 05:26:14.000000 networkaddress-0.0.1/LICENSE
--rw-r--r--   0 duynha    (1000) duynha    (1000)     3733 2023-09-30 12:00:59.297510 networkaddress-0.0.1/PKG-INFO
--rw-r--r--   0 duynha    (1000) duynha    (1000)      103 2023-09-30 08:47:45.000000 networkaddress-0.0.1/README.md
--rw-r--r--   0 duynha    (1000) duynha    (1000)     2708 2023-09-30 11:50:55.000000 networkaddress-0.0.1/pyproject.toml
--rw-r--r--   0 duynha    (1000) duynha    (1000)       38 2023-09-30 12:00:59.301510 networkaddress-0.0.1/setup.cfg
-drwxr-xr-x   0 duynha    (1000) duynha    (1000)        0 2023-09-30 12:00:59.293511 networkaddress-0.0.1/src/
-drwxr-xr-x   0 duynha    (1000) duynha    (1000)        0 2023-09-30 12:00:59.297510 networkaddress-0.0.1/src/networkaddress/
--rw-r--r--   0 duynha    (1000) duynha    (1000)        0 2023-09-30 09:09:53.000000 networkaddress-0.0.1/src/networkaddress/__init__.py
-drwxr-xr-x   0 duynha    (1000) duynha    (1000)        0 2023-09-30 12:00:59.297510 networkaddress-0.0.1/src/networkaddress/ip/
--rw-r--r--   0 duynha    (1000) duynha    (1000)       55 2023-09-30 05:26:14.000000 networkaddress-0.0.1/src/networkaddress/ip/__init__.py
--rw-r--r--   0 duynha    (1000) duynha    (1000)     1736 2023-09-30 05:26:14.000000 networkaddress-0.0.1/src/networkaddress/ip/port.py
--rw-r--r--   0 duynha    (1000) duynha    (1000)     3713 2023-09-30 05:26:14.000000 networkaddress-0.0.1/src/networkaddress/mac.py
-drwxr-xr-x   0 duynha    (1000) duynha    (1000)        0 2023-09-30 12:00:59.297510 networkaddress-0.0.1/src/networkaddress.egg-info/
--rw-r--r--   0 duynha    (1000) duynha    (1000)     3733 2023-09-30 12:00:59.000000 networkaddress-0.0.1/src/networkaddress.egg-info/PKG-INFO
--rw-r--r--   0 duynha    (1000) duynha    (1000)      397 2023-09-30 12:00:59.000000 networkaddress-0.0.1/src/networkaddress.egg-info/SOURCES.txt
--rw-r--r--   0 duynha    (1000) duynha    (1000)        1 2023-09-30 12:00:59.000000 networkaddress-0.0.1/src/networkaddress.egg-info/dependency_links.txt
--rw-r--r--   0 duynha    (1000) duynha    (1000)      213 2023-09-30 12:00:59.000000 networkaddress-0.0.1/src/networkaddress.egg-info/requires.txt
--rw-r--r--   0 duynha    (1000) duynha    (1000)       15 2023-09-30 12:00:59.000000 networkaddress-0.0.1/src/networkaddress.egg-info/top_level.txt
-drwxr-xr-x   0 duynha    (1000) duynha    (1000)        0 2023-09-30 12:00:59.297510 networkaddress-0.0.1/test/
--rw-r--r--   0 duynha    (1000) duynha    (1000)     6898 2023-09-30 09:13:42.000000 networkaddress-0.0.1/test/test_mac.py
--rw-r--r--   0 duynha    (1000) duynha    (1000)      266 2023-09-30 09:13:42.000000 networkaddress-0.0.1/test/test_port.py
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.745196 networkaddress-0.0.2/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)     1078 2024-01-26 02:23:08.000000 networkaddress-0.0.2/LICENSE
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       23 2024-01-26 02:33:45.000000 networkaddress-0.0.2/MANIFEST.in
+-rw-r--r--   0 duynguyen  (1001) duynguyen  (1001)     3726 2024-01-26 02:37:49.745196 networkaddress-0.0.2/PKG-INFO
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)      103 2023-10-05 08:32:57.000000 networkaddress-0.0.2/README.md
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)     2318 2024-01-26 02:33:45.000000 networkaddress-0.0.2/pyproject.toml
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       38 2024-01-26 02:37:49.745196 networkaddress-0.0.2/setup.cfg
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.733197 networkaddress-0.0.2/src/
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.737197 networkaddress-0.0.2/src/networkaddress/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:23:08.000000 networkaddress-0.0.2/src/networkaddress/__init__.py
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)     3994 2024-01-26 02:33:45.000000 networkaddress-0.0.2/src/networkaddress/macaddress.py
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)     1665 2024-01-26 02:33:45.000000 networkaddress-0.0.2/src/networkaddress/portnumber.py
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:33:45.000000 networkaddress-0.0.2/src/networkaddress/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/src/networkaddress.egg-info/
+-rw-r--r--   0 duynguyen  (1001) duynguyen  (1001)     3726 2024-01-26 02:37:49.000000 networkaddress-0.0.2/src/networkaddress.egg-info/PKG-INFO
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)     2129 2024-01-26 02:37:49.000000 networkaddress-0.0.2/src/networkaddress.egg-info/SOURCES.txt
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        1 2024-01-26 02:37:49.000000 networkaddress-0.0.2/src/networkaddress.egg-info/dependency_links.txt
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)      219 2024-01-26 02:37:49.000000 networkaddress-0.0.2/src/networkaddress.egg-info/requires.txt
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       15 2024-01-26 02:37:49.000000 networkaddress-0.0.2/src/networkaddress.egg-info/top_level.txt
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.733197 networkaddress-0.0.2/venv/
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.733197 networkaddress-0.0.2/venv/lib/
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.733197 networkaddress-0.0.2/venv/lib/python3.9/
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.737197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/_pytest/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/_pytest/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/black/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:19.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/black/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/build/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:59.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/build/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/certifi/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/certifi/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/charset_normalizer/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/click/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/click/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/coverage/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       72 2024-01-25 07:20:00.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/coverage/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/cryptography/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/cryptography/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/exceptiongroup/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/idna/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/idna/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/importlib_metadata/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/iniconfig/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/iniconfig/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/isort/
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.737197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/isort/_vendored/
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/isort/_vendored/tomli/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       26 2023-09-26 03:05:53.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-26 03:05:53.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/isort/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/keyring/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:59.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/keyring/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/markdown_it/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       26 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/markdown_it/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/mdurl/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       26 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/mdurl/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/more_itertools/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:57.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/more_itertools/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/mypy/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       64 2023-09-27 07:47:18.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/mypy/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/nh3/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:57.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/nh3/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/packaging/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/packaging/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pathspec/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       68 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pathspec/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pip/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)      286 2023-09-26 02:54:26.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pip/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pkginfo/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:57.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pkginfo/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/platformdirs/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/platformdirs/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pluggy/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pluggy/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pytest/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/pytest/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/readme_renderer/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/readme_renderer/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/rich/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:58.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/rich/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/secretstorage/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:59.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/secretstorage/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/tomli/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       26 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/tomli/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/tomlkit/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-27 07:47:17.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/tomlkit/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/twine/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)        0 2023-09-28 02:47:59.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/twine/py.typed
+drwxrwxr-x   0 duynguyen  (1001) duynguyen  (1001)        0 2024-01-26 02:37:49.741197 networkaddress-0.0.2/venv/lib/python3.9/site-packages/urllib3/
+-rw-rw-r--   0 duynguyen  (1001) duynguyen  (1001)       93 2023-09-28 02:47:57.000000 networkaddress-0.0.2/venv/lib/python3.9/site-packages/urllib3/py.typed
```

### Comparing `networkaddress-0.0.1/LICENSE` & `networkaddress-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `networkaddress-0.0.1/PKG-INFO` & `networkaddress-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkaddress
-Version: 0.0.1
+Version: 0.0.2
 Summary: A network address manipulation library
 Author-email: "Duy N. H. A." <me@duynha.dev>
 License: MIT License
         
         Copyright (c) 2023, Nguyen Hoang Anh Duy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/duynhaaa/networkaddress
 Project-URL: repository, https://github.com/duynhaaa/networkaddress
-Keywords: Networking,IP,IPv4,IPv6
+Keywords: Networking
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
@@ -55,20 +55,20 @@
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Requires-Dist: flake8-pyproject; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: mypy; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
+Requires-Dist: pycodestyle; extra == "lint"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Provides-Extra: publish
 Requires-Dist: twine; extra == "publish"
```

### Comparing `networkaddress-0.0.1/pyproject.toml` & `networkaddress-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "networkaddress"
-version = "0.0.1"
+version = "0.0.2"
 description = "A network address manipulation library"
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 authors = [{ name = "Duy N. H. A.", email = "me@duynha.dev" }]
-keywords = ["Networking", "IP", "IPv4", "IPv6"]
+keywords = ["Networking"]
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Manufacturing",
     "Intended Audience :: System Administrators",
@@ -41,30 +41,26 @@
     "Typing :: Typed",
 ]
 
 [project.urls]
 homepage = "https://github.com/duynhaaa/networkaddress"
 repository = "https://github.com/duynhaaa/networkaddress"
 
-
 [project.optional-dependencies]
-lint = ["black", "flake8", "flake8-pyproject", "isort", "mypy", "pylint"]
+lint = ["flake8", "flake8-pyproject", "isort", "mypy", "pylint", "pycodestyle"]
 test = ["pytest", "pytest-cov"]
 build = ["build"]
 publish = ["twine"]
 develop = [
     "networkaddress[lint]",
     "networkaddress[test]",
     "networkaddress[build]",
     "networkaddress[publish]"
 ]
 
-[tool.black]
-line-length = 79
-
 [tool.isort]
 atomic = true
 case_sensitive = true
 dedup_headings = true
 balanced_wrapping = true
 combine_as_imports = true
 include_trailing_comma = true
@@ -73,21 +69,9 @@
 [tool.mypy]
 strict = true
 python_version = "3.9"
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
 disallow_any_unimported = true
 check_untyped_defs = true
 
-[tool.flake8]
-extend_ignore = [
-    # Ignore "Whitespace before ':'" error because it conflicts with 'black'
-    # formatter.
-    "E203",
-]
-
 [tool.pylint]
-disable = [
-    # Ignore "consider-using-f-string" error because we uses different string
-    # formatting ways to achieve better code readability and consistent code
-    # formatting using 'black'.
-    "C0209",
-]
+disable = []
```

### Comparing `networkaddress-0.0.1/src/networkaddress/ip/port.py` & `networkaddress-0.0.2/src/networkaddress/portnumber.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,63 @@
-__all__ = ["PortNumber"]
+__all__ = [
+    "MIN_VALUE",
+    "MAX_VALUE",
+    "PortNumber",
+    "InvalidPortNumber",
+]
 
-from typing import Any
+import typing
 
-MIN_VALUE = 0
-MAX_VALUE = 65535
+MIN_VALUE: typing.Final[int] = 0
+MAX_VALUE: typing.Final[int] = 65535
 
 
 class PortNumber:
     __slots__ = ("_value",)
 
     def __init__(self, value: int, /) -> None:
         if value < MIN_VALUE:
-            raise ValueError(
-                "%s (< %s) is not permitted as a port number"
-                % (value, MIN_VALUE)
-            )
+            raise InvalidPortNumber(f"{value} < {MIN_VALUE}")
         if value > MAX_VALUE:
-            raise ValueError(
-                "%s (> %s) is not permitted as a port number"
-                % (value, MAX_VALUE)
-            )
+            raise InvalidPortNumber(f"{value} > {MAX_VALUE}")
         self._value = value
 
     def __str__(self) -> str:
         return str(self._value)
 
     def __repr__(self) -> str:
-        return "%s.%s(%s)" % (
-            self.__class__.__module__,
-            self.__class__.__name__,
-            self._value,
-        )
+        return f"{type(self).__name__}({self._value})"
 
     def __index__(self) -> int:
         return self._value
 
     def __hash__(self) -> int:
         return hash((type(self), self._value))
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: typing.Any) -> bool:
         if isinstance(other, PortNumber):
             return self._value == other._value
         return NotImplemented
 
-    def __lt__(self, other: Any) -> bool:
+    def __lt__(self, other: typing.Any) -> bool:
         if isinstance(other, PortNumber):
             return self._value < other._value
         return NotImplemented
 
-    def __le__(self, other: Any) -> bool:
+    def __le__(self, other: typing.Any) -> bool:
         if isinstance(other, PortNumber):
             return self._value <= other._value
         return NotImplemented
 
-    def __gt__(self, other: Any) -> bool:
+    def __gt__(self, other: typing.Any) -> bool:
         if isinstance(other, PortNumber):
             return self._value > other._value
         return NotImplemented
 
-    def __ge__(self, other: Any) -> bool:
+    def __ge__(self, other: typing.Any) -> bool:
         if isinstance(other, PortNumber):
             return self._value >= other._value
         return NotImplemented
+
+
+class InvalidPortNumber(ValueError):
+    pass
```

### Comparing `networkaddress-0.0.1/src/networkaddress.egg-info/PKG-INFO` & `networkaddress-0.0.2/src/networkaddress.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkaddress
-Version: 0.0.1
+Version: 0.0.2
 Summary: A network address manipulation library
 Author-email: "Duy N. H. A." <me@duynha.dev>
 License: MIT License
         
         Copyright (c) 2023, Nguyen Hoang Anh Duy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/duynhaaa/networkaddress
 Project-URL: repository, https://github.com/duynhaaa/networkaddress
-Keywords: Networking,IP,IPv4,IPv6
+Keywords: Networking
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
@@ -55,20 +55,20 @@
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Requires-Dist: flake8-pyproject; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: mypy; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
+Requires-Dist: pycodestyle; extra == "lint"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Provides-Extra: publish
 Requires-Dist: twine; extra == "publish"
```

