# Comparing `tmp/kdp-python-connector-0.60.0.tar.gz` & `tmp/kdp-python-connector-0.62.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-python-connector-0.60.0.tar", last modified: Mon Apr  1 23:02:11 2024, max compression
+gzip compressed data, was "kdp-python-connector-0.62.0.tar", last modified: Thu Apr  4 05:44:41 2024, max compression
```

## Comparing `kdp-python-connector-0.60.0.tar` & `kdp-python-connector-0.62.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.255176 kdp-python-connector-0.60.0/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.247176 kdp-python-connector-0.60.0/.github/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      234 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/.github/pull_request_template.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.247176 kdp-python-connector-0.60.0/.github/workflows/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7347 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/.github/workflows/build-internal.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6899 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/.github/workflows/build-public.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5028 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/.github/workflows/release-internal.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4044 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/.github/workflows/release-public.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3956 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/.github/workflows/release.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1869 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/.gitignore
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/.nojekyll
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-01 23:02:11.255176 kdp-python-connector-0.60.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.247176 kdp-python-connector-0.60.0/datafiles/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13666 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/datafiles/actorfilms.csv
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.247176 kdp-python-connector-0.60.0/docs/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/.nojekyll
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      634 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/Makefile
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/conf.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/index.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/kdp_connector.configuration.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1581 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/kdp_connector.connectors.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      447 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/kdp_connector.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      765 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/make.bat
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/docs/modules.rst
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.247176 kdp-python-connector-0.60.0/kdp_connector/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.251176 kdp-python-connector-0.60.0/kdp_connector/configuration/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/configuration/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/configuration/authenticationUtil.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/configuration/configurationUtil.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/configuration/keycloak_authentication.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/configuration/proxy_authentication.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.251176 kdp-python-connector-0.60.0/kdp_connector/connectors/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      669 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/Storage.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1585 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/audit_log.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3620 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/audit_log_configs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7467 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/batch_write.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2205 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/index_management.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/ingest_job_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8754 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/kdp_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2302 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4760 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/read.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1892 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/connectors/upload.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25205 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/kdp_connector/main.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.255176 kdp-python-connector-0.60.0/kdp_python_connector.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-01 23:02:11.000000 kdp-python-connector-0.60.0/kdp_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1496 2024-04-01 23:02:11.000000 kdp-python-connector-0.60.0/kdp_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-01 23:02:11.000000 kdp-python-connector-0.60.0/kdp_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-01 23:02:11.000000 kdp-python-connector-0.60.0/kdp_python_connector.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-01 23:02:11.000000 kdp-python-connector-0.60.0/kdp_python_connector.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-01 23:02:11.255176 kdp-python-connector-0.60.0/setup.cfg
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 23:02:11.255176 kdp-python-connector-0.60.0/test/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/test/README.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4014 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/test/test_ingest.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/test/test_keycloak.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2024-04-01 23:02:00.000000 kdp-python-connector-0.60.0/test/test_read.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.881898 kdp-python-connector-0.62.0/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.869898 kdp-python-connector-0.62.0/.github/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      234 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/.github/pull_request_template.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.869898 kdp-python-connector-0.62.0/.github/workflows/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7347 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/.github/workflows/build-internal.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6903 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/.github/workflows/build-public.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5028 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/.github/workflows/release-internal.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4044 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/.github/workflows/release-public.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3956 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/.github/workflows/release.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1869 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/.gitignore
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/.nojekyll
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-04 05:44:41.881898 kdp-python-connector-0.62.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.869898 kdp-python-connector-0.62.0/datafiles/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13666 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/datafiles/actorfilms.csv
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.873898 kdp-python-connector-0.62.0/docs/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/.nojekyll
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      634 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/Makefile
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/conf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/index.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/kdp_connector.configuration.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1581 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/kdp_connector.connectors.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      447 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/kdp_connector.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      765 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/make.bat
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/docs/modules.rst
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.873898 kdp-python-connector-0.62.0/kdp_connector/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.873898 kdp-python-connector-0.62.0/kdp_connector/configuration/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/configuration/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/configuration/authenticationUtil.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/configuration/configurationUtil.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/configuration/keycloak_authentication.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/configuration/proxy_authentication.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.877899 kdp-python-connector-0.62.0/kdp_connector/connectors/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      669 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/Storage.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1624 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/audit_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3620 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/audit_log_configs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7528 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/batch_write.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2276 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/index_management.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2388 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/ingest_job_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8921 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/kdp_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2311 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4782 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/read.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1892 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/connectors/upload.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25522 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/kdp_connector/main.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.877899 kdp-python-connector-0.62.0/kdp_python_connector.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-04 05:44:41.000000 kdp-python-connector-0.62.0/kdp_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1496 2024-04-04 05:44:41.000000 kdp-python-connector-0.62.0/kdp_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-04 05:44:41.000000 kdp-python-connector-0.62.0/kdp_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-04 05:44:41.000000 kdp-python-connector-0.62.0/kdp_python_connector.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-04 05:44:41.000000 kdp-python-connector-0.62.0/kdp_python_connector.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-04 05:44:41.881898 kdp-python-connector-0.62.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 05:44:41.877899 kdp-python-connector-0.62.0/test/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/test/README.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4263 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/test/test_ingest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/test/test_keycloak.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4857 2024-04-04 05:44:31.000000 kdp-python-connector-0.62.0/test/test_read.py
```

### Comparing `kdp-python-connector-0.60.0/.github/workflows/build-internal.yaml` & `kdp-python-connector-0.62.0/.github/workflows/build-internal.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/.github/workflows/build-public.yaml` & `kdp-python-connector-0.62.0/.github/workflows/build-public.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on:
   push:
   repository_dispatch:
     types: [ build-connector, build-public-connector ]
 
 
 env:
-  VERSION: ${{ github.event.client_payload.version || '0.0.1' }}
+  VERSION: ${{ github.event.client_payload.version || '0.56.dev5' }}
   PACKAGE_NAME: kdp-python-connector
   CODE_ARTIFACT_DOMAIN: kdp
   CODE_ARTIFACT_REPO: kdp-python-connector
   CODE_ARTIFACT_URL: https://us-west-2.console.aws.amazon.com/codesuite/codeartifact/d/365668498277/kdp/r/kdp-python-connector/p/pypi/kdp-python-connector/versions?region=us-west-2&package-versions-meta=eyJmIjp7fSwicyI6e30sIm4iOjIwLCJpIjowfQ
   BRANCH_REF: ${{ github.event.client_payload.pythonConnectorRef || 'main' }}
   PYTHON_CLIENT_VERSION: ${{ github.event.client_payload.pythonClientVersion }}
   PYTHON_CLIENT_CODE_ARTIFACT_REPO: kdp-api-python-client
```

### Comparing `kdp-python-connector-0.60.0/.github/workflows/release-internal.yaml` & `kdp-python-connector-0.62.0/.github/workflows/release-internal.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/.github/workflows/release-public.yaml` & `kdp-python-connector-0.62.0/.github/workflows/release-public.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/.github/workflows/release.yaml` & `kdp-python-connector-0.62.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/.gitignore` & `kdp-python-connector-0.62.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/PKG-INFO` & `kdp-python-connector-0.62.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kdp-python-connector
-Version: 0.60.0
+Version: 0.62.0
 Summary: Python Connector for KDP Platform
 Author-email: Koverse development team <developer@koverse.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: kdp-api-python-client~=4.125.0
+Requires-Dist: kdp-api-python-client~=4.126.0
 Requires-Dist: pandas~=1.4.2
 Requires-Dist: numpy~=1.22.4
 
 # kdp-python-connector
 
 ## Prequisites
 * Python version 3.8.5
```

### Comparing `kdp-python-connector-0.60.0/datafiles/actorfilms.csv` & `kdp-python-connector-0.62.0/datafiles/actorfilms.csv`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/docs/Makefile` & `kdp-python-connector-0.62.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/docs/conf.py` & `kdp-python-connector-0.62.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/docs/kdp_connector.configuration.rst` & `kdp-python-connector-0.62.0/docs/kdp_connector.configuration.rst`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/docs/kdp_connector.connectors.rst` & `kdp-python-connector-0.62.0/docs/kdp_connector.connectors.rst`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/docs/make.bat` & `kdp-python-connector-0.62.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/kdp_connector/configuration/authenticationUtil.py` & `kdp-python-connector-0.62.0/kdp_connector/configuration/authenticationUtil.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/kdp_connector/configuration/configurationUtil.py` & `kdp-python-connector-0.62.0/kdp_connector/configuration/configurationUtil.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/kdp_connector/configuration/keycloak_authentication.py` & `kdp-python-connector-0.62.0/kdp_connector/configuration/keycloak_authentication.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/Storage.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/Storage.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/audit_log.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/audit_log.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import kdp_api
 import logging
+
+from kdp_api import LuceneQueryRequest
 from kdp_api.api import workspaces_api
 from kdp_api.models.audit_log_paginator import AuditLogPaginator
 from kdp_api.configuration import Configuration
 
 
 class AuditLogApi(object):
     def __init__(self, configuration: Configuration=None):
@@ -21,15 +23,17 @@
             :returns: AuditLogPaginator object which contains audit log records matching query expression
 
             :rtype: AuditLogPaginator
         """
         logging.info(f'function parameters - dataset_id: %s, expression: %s, limit: %s, offset: %s' % (dataset_id, expression, limit, offset))
         with kdp_api.ApiClient(config) as api_client:
             api_instance = workspaces_api.WorkspacesApi(api_client)
-            query = {}
-            query['datasetId'] = dataset_id
-            query['expression'] = expression
-            query['limit'] = limit
-            query['offset'] = offset
+
+            query = LuceneQueryRequest(
+              datasetId=dataset_id,
+              expression=expression,
+              limit=limit,
+              offset=offset
+            )
 
             return api_instance.post_audit_log_query(lucene_query_request=query)
```

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/audit_log_configs.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/audit_log_configs.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/batch_write.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/batch_write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,61 @@
+from typing import List, Dict, Any
+
 import kdp_api
 import logging
 import gzip
 import json
 import urllib3
-from urllib3.util import Timeout
+from urllib3 import Timeout
 from pprint import pprint
 from kdp_api.api import write_api
 from kdp_api.models import WriteBatchResponse
 from kdp_api.models import BatchWriteRequest
 from kdp_api.models import SecurityLabelInfoParams
 from kdp_api.configuration import Configuration
 from pandas import DataFrame
 
+
 class WriteApi(object):
-    def __init__(self, configuration: Configuration=None):
+    def __init__(self, configuration: Configuration = None):
         self.configuration = configuration
-        host=self.configuration.host.replace('https://', '')
-
-        self.http = urllib3.HTTPSConnectionPool(host, port=443, cert_reqs='CERT_NONE', assert_hostname=False,
-        timeout=Timeout(connect=2.0, read=60.0))
+        host = self.configuration.host.replace('https://', '')
 
+        self.http = urllib3.HTTPSConnectionPool(host, port=443, cert_reqs='CERT_NONE', assert_hostname=False, timeout=Timeout(connect=2.0, read=60.0))
 
-    def batch_write(self, config, dataset_id: str, dataframe: DataFrame, batch_size: int, is_async: bool = True):
+    def batch_write(self, config, dataset_id: str, dataframe: DataFrame, batch_size: int, is_async: bool = False):
         """This method will be used to write batches of data to KDP
 
             :param Configuration config: Connection configuration
             :param str dataset_id: ID of the KDP dataset where the data will be written
             :param DataFrame dataframe: Data to write to KDP
             :param int batch_size: Defaults to 100
-            :param bool is_async: Defaults to True
+            :param bool is_async: Defaults to False
 
             :returns: Set of partitions data was written to
 
             :rtype: set
         """
         with kdp_api.ApiClient(config) as api_client:
 
             # Create an instance of the API class
             api_instance = write_api.WriteApi(api_client)
 
             partitions_set = set()
 
             try:
                 # Convert dataframe into dict. The result is an array of json.
-                json_record_array = dataframe.to_dict(orient='records')
+                json_record_array: List[Dict[str, Dict[str, Any]]] = dataframe.to_dict(orient='records')
 
                 for i in range(0, len(json_record_array), batch_size):
-
                     batch = json_record_array[i:i + batch_size]
 
                     write_batch_response: WriteBatchResponse = api_instance.post_write_id(
                         dataset_id=dataset_id,
-                        json_record=batch,
+                        request_body=batch,
                         is_async=is_async
                     )
 
                     partitions_set.update(write_batch_response.partitions)
 
                 return partitions_set
 
@@ -79,15 +79,14 @@
             :rtype: set
         """
 
         request = {
             'records': data
         }
 
-
         params = security_label_info_params.to_dict()
 
         if security_label_info_params is not None:
             # required attributes
             request['securityLabelInfo'] = {
                 'parserClassName': security_label_info_params.parser_class_name,
                 'fields': security_label_info_params.fields
@@ -95,16 +94,14 @@
 
             if 'label_handling_policy' in params:
                 request['securityLabelInfo']['labelHandlingPolicy'] = params['label_handling_policy']
 
             if 'replacementString' in params:
                 request['securityLabelInfo']['replacementString'] = params['replacementString']
 
-
-
         json_bytes = json.dumps(request).encode('utf-8')
         compressed = gzip.compress(json_bytes)
 
         url = self.configuration.host + "/v2/write/" + dataset_id + '?isAsync=' + str(is_async)
 
         logging.debug(f'request url = {url}')
         logging.debug('request payload (before compression): %s' % json_bytes)
@@ -113,25 +110,24 @@
             'POST',
             url,
             body=compressed,
             headers={
                 'Content-Encoding': 'gzip',
                 'Content-Type': 'application/json',
                 'Authorization': 'Bearer ' + self.configuration.access_token
-                }
-            )
+            }
+        )
 
         if result.status == 200:
             return json.loads(result.data)
         else:
             logging.error('unexpected response code returned. status: %s, reason: %s, message: %s' %
-                (result.status, result.reason, result.msg))
+                          (result.status, result.reason, result.msg))
             raise Exception('Failed to post to batch-write')
 
-
     def batch_write_v2(self, config,
             dataset_id: str,
             dataframe: DataFrame,
             security_label_info_params: SecurityLabelInfoParams = None,
             batch_size: int = 100,
             is_async: bool = True,
             is_compressed: bool = False):
@@ -170,15 +166,15 @@
                             dataset_id=dataset_id,
                             data=batch,
                             security_label_info_params=security_label_info_params,
                             is_async=is_async)
 
                         partitions_set.update(write_batch_response['partitions'])
                     else:
-                        request:BatchWriteRequest = BatchWriteRequest(records=batch, security_label_info=security_label_info_params)
+                        request: BatchWriteRequest = BatchWriteRequest(records=batch, security_label_info=security_label_info_params)
 
                         write_batch_response: WriteBatchResponse = api_instance.post_v2_write_id(
                             dataset_id=dataset_id,
                             batch_write_request=request,
                             is_async=is_async
                         )
```

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/index_management.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/index_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,59 +2,58 @@
 import urllib3
 import logging
 
 from urllib3.util import Timeout
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
+
 class IndexManagementApi(object):
     def __init__(self, configuration=None):
         self.configuration = configuration
-        host=self.configuration.host.replace('https://', '')
+        host = self.configuration.host.replace('https://', '')
 
         self.http = urllib3.HTTPSConnectionPool(host, port=443, cert_reqs='CERT_NONE', assert_hostname=False,
-        timeout=Timeout(connect=2.0, read=10.0))
-
+                                                timeout=Timeout(connect=2.0, read=10.0))
 
     def modify_indexes(self, dataset_id: str, create: list, remove: list,
-        autoCreateIndexes: bool = False, searchAnyField: bool = False) -> object :
+                       autoCreateIndexes: bool = False, searchAnyField: bool = False) -> object:
         """This method will modify existing indexes on a dataset
 
             :param str dataset_id: ID of dataset
             :param list create: List of indexes to create
             :param list remove: List of indexes to delete
             :param bool autoCreateIndexes: Whether to automatically create indexes when data is written
             :param bool searchAnyField: Whether to automatically search any field
 
             :returns: Job ID
 
             :rtype: str
        """
-        request={}
-        request['action']='modifyIndexes'
-        request['datasetId']=dataset_id
-        request['remove']=remove
-        request['create']=create
-        request['autoCreateIndexes']=autoCreateIndexes
-        request['searchAnyField']=searchAnyField
+        request = {}
+        request['action'] = 'modifyIndexes'
+        request['datasetId'] = dataset_id
+        request['remove'] = remove
+        request['create'] = create
+        request['autoCreateIndexes'] = autoCreateIndexes
+        request['searchAnyField'] = searchAnyField
 
         encoded_data = json.dumps(request).encode('utf-8')
 
         logging.info('modify_indexes payload: %s' % json.dumps(request))
 
         result: urllib3.response.HTTPResponse = self.http.request(
             'POST',
             self.configuration.host + "/index-management",
             body=encoded_data,
             headers={
                 'Content-Type': 'application/json',
                 'Authorization': 'Bearer ' + self.configuration.access_token
-                }
-            )
+            }
+        )
 
         if result.status == 201:
             return json.loads(result.data)
         else:
             logging.error('unexpected response code returned. status: %s, reason: %s, message: %s' %
-                (result.status, result.reason, result.msg))
+                          (result.status, result.reason, result.msg))
             raise Exception('Failed to modify indexes')
-
```

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/ingest_job_api.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/ingest_job_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 import json
 import urllib3
 import logging
 from urllib3.util import Timeout
 
+
 class IngestJobApi(object):
     def __init__(self, configuration=None):
         self.configuration = configuration
-        host=self.configuration.host.replace('https://', '')
+        host = self.configuration.host.replace('https://', '')
 
         self.http = urllib3.HTTPSConnectionPool(host, port=443, cert_reqs='CERT_NONE',
-            assert_hostname=False, timeout=Timeout(connect=2.0, read=10.0))
-
+                                                assert_hostname=False, timeout=Timeout(connect=2.0, read=10.0))
 
-    def create_url_ingest_job(self, workspace_id: str, dataset_id: str, url_list) -> str :
+    def create_url_ingest_job(self, workspace_id: str, dataset_id: str, url_list) -> str:
 
         """This method will be used to start a job that ingests files to KDP
 
             :param str workspace_id: ID of KDP workspace data will be written to
             :param str dataset_id: ID of the KDP dataset where the data will be written
             :param list url_list: List of urls for each file to be ingested
 
             :returns: Job ID
 
             :rtype: str
         """
 
-        ingest_request={}
-        ingest_request['workspaceId']=workspace_id
-        ingest_request['datasetId']=dataset_id
-        ingest_request['securityLabeled']=False
-        ingest_request['dataSourceParams']={}
-        ingest_request['dataSourceParams']['type']='URL'
-        ingest_request['dataSourceParams']['connectionInfo']={}
-        ingest_request['dataSourceParams']['connectionInfo']['urls']=[]
+        ingest_request = {}
+        ingest_request['workspaceId'] = workspace_id
+        ingest_request['datasetId'] = dataset_id
+        ingest_request['securityLabeled'] = False
+        ingest_request['dataSourceParams'] = {}
+        ingest_request['dataSourceParams']['type'] = 'URL'
+        ingest_request['dataSourceParams']['connectionInfo'] = {}
+        ingest_request['dataSourceParams']['connectionInfo']['urls'] = []
 
         for url_str in url_list:
-            url={}
-            url['url']=url_str
+            url = {}
+            url['url'] = url_str
             ingest_request['dataSourceParams']['connectionInfo']['urls'].append(url)
 
         return self.create_ingest_job(ingest_request)
 
-
-    def create_ingest_job(self, ingest_request: object) -> str :
+    def create_ingest_job(self, ingest_request: object) -> str:
         encoded_data = json.dumps(ingest_request).encode('utf-8')
 
         result: urllib3.response.HTTPResponse = self.http.request(
             'POST',
             self.configuration.host + "/ingest",
             body=encoded_data,
             headers={
                 'Content-Type': 'application/json',
                 'Authorization': 'Bearer ' + self.configuration.access_token
-                }
-            )
+            }
+        )
 
         if result.status == 202:
             return json.loads(result.data)
         else:
             logging.error('unexpected response code returned. status: %s, reason: %s, message: %s' %
-                (result.status, result.reason, result.msg))
+                          (result.status, result.reason, result.msg))
             raise Exception('Failed to create ingest job')
-
```

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/kdp_api.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/kdp_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,95 +1,97 @@
 import kdp_api as kdp_api_client
+from kdp_api import DatasetCreateRequest, WorkspaceCreateRequest, DatasetPatchRequest
 from kdp_api.api.datasets_api import DatasetsApi
 from kdp_api.api.workspaces_api import WorkspacesApi
 from kdp_api.api.indexing_api import IndexingApi
 from kdp_api.api.users_and_groups_api import UsersAndGroupsApi
 
+
 class KdpApi(object):
 
     @staticmethod
     def create_dataset(config, name: str, workspace_id: str, description: str = '', auto_create_indexes: bool = True,
-                       schema: dict = '{}', search_any_field: bool = True, record_count: int = 0):
+                       schema: any = None, search_any_field: bool = True, record_count: int = 0):
         """This method will create a new KDP dataset
 
             :param str name: Name of dataset to create
             :param str workspace_id: Workspace that dataset will be created in
             :param str description: Description of dataset
             :param bool auto_create_indexes: Whether to automatically index new data
             :param dict schema: Schema of dataset
             :param bool search_any_field: Whether to search any field
             :param int record_count: Whether to search any field
 
             :returns: New dataset
 
             :rtype: Dataset
         """
+        if schema is None:
+            schema: dict = {}
         with kdp_api_client.ApiClient(config) as api_client:
-            request_body = {
-                    'name': name,
-                    'record_count': record_count,
-                    'description': description,
-                    'auto_create_indexes': auto_create_indexes,
-                    'schema': schema,
-                    'search_any_field': search_any_field,
-                    'workspace_id': workspace_id
-                }
+
+            dataset_create_request = DatasetCreateRequest(
+              name=name,
+              record_count=record_count,
+              description=description,
+              auto_create_indexes=auto_create_indexes,
+              schema=schema,
+              search_any_field=search_any_field,
+              workspace_id=workspace_id
+            )
 
             datasets_api = DatasetsApi(api_client)
-            return datasets_api.post_datasets(dataset_create_request=request_body)
+            return datasets_api.post_datasets(dataset_create_request=dataset_create_request)
 
     @staticmethod
     def create_workspace(config, name: str, workspace_id: str = None):
         """This method will create a new KDP workspace
 
             :param str name: Name of workspace to create
             :param str workspace_id: ID of workspace if specified (defaults to name)
 
             :returns: New workspace
 
             :rtype: Workspace
         """
         with kdp_api_client.ApiClient(config) as api_client:
 
-            request_body = {
-                'name': name,
-                'id': workspace_id if workspace_id is not None else name
-            }
+            workspace_create_request = WorkspaceCreateRequest(
+              name=name,
+              id=workspace_id if workspace_id is not None else name
+            )
             workspaces_api = WorkspacesApi(api_client)
-            return workspaces_api.post_workspaces(workspace_create_request=request_body)
+            return workspaces_api.post_workspaces(workspace_create_request=workspace_create_request)
 
     @staticmethod
     def delete_workspace(config, workspace_id: str):
         """This method will delete a workspace by id
 
             :param Configuration config: Connection configuration
             :param str workspace_id: ID of workspace
 
             :returns: Deleted workspace
 
             :rtype: Workspace
         """
         with kdp_api_client.ApiClient(config) as api_client:
-
             workspaces_api = WorkspacesApi(api_client)
             return workspaces_api.delete_workspaces_id(workspace_id)
 
-
     @staticmethod
     def get_workspace(config, workspace_id: str):
         """This method will get a workspace by id
             :param Configuration config: Connection configuration
             :param str workspace_id: ID of workspace
 
             :returns: Workspace
 
             :rtype: Workspace
         """
         with kdp_api_client.ApiClient(config) as api_client:
-
             workspaces_api = WorkspacesApi(api_client)
             return workspaces_api.get_workspaces_id(workspace_id)
 
     @staticmethod
     def get_dataset(config, dataset_id: str):
         """This method will get a dataset by id
 
@@ -97,36 +99,33 @@
             :param str dataset_id: ID of dataset
 
             :returns: Dataset
 
             :rtype: Dataset
         """
         with kdp_api_client.ApiClient(config) as api_client:
-
             datasets_api = DatasetsApi(api_client)
             return datasets_api.get_datasets_id(dataset_id)
 
-
     @staticmethod
-    def patch_dataset(config, dataset_id: str, payload):
+    def patch_dataset(config, dataset_id: str, payload: DatasetPatchRequest):
         """This method will update fields in a dataset
 
            :param Configuration config: Connection configuration
            :param str dataset_id: ID of dataset
            :param PatchDataset payload: Payload with the fields to update
 
            :returns: Dataset
 
            :rtype: Dataset
        """
         with kdp_api_client.ApiClient(config) as api_client:
             datasets_api = DatasetsApi(api_client)
             return datasets_api.patch_datasets_id(id=dataset_id, dataset_patch_request=payload)
 
-
     @staticmethod
     def get_indexes(config, dataset_id: str, limit: int = 10):
         """This method will get indexes for a dataset
 
             :param Configuration config: Connection configuration
             :param str dataset_id: ID of dataset
             :param int limit: Limit number of results returned (default 10)
@@ -198,15 +197,14 @@
 
             :rtype: JobPaginator
         """
         with kdp_api_client.ApiClient(config) as api_client:
             datasets_api = DatasetsApi(api_client)
             return datasets_api.get_jobs(dataset_id=dataset_id, **kwargs)
 
-
     @staticmethod
     def delete_user(config, user_id: str):
         """This method will delete a user by id
 
             :param Configuration config: Connection configuration
             :param str user_id: ID of user
```

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/read.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pandas as pd
 import kdp_api
+from kdp_api import ReadRangeRequest
 from kdp_api.api import read_and_query_api
 from kdp_api.models import SequenceReadRequest
 from kdp_api.models import RecordBatch
 
 
 class ReadApi(object):
 
@@ -30,15 +31,15 @@
                     api_instance=api_instance,
                     dataset_id=dataset_id,
                     starting_record_id=starting_record_id,
                     batch_size=batch_size)
                 has_more_records = record_batch.more
                 starting_record_id = record_batch.last_record_id
                 for json_record in record_batch.records:
-                    dictionary_list.append(json_record['_data_store'])
+                    dictionary_list.append(json_record)
 
             return dictionary_list
 
     @staticmethod
     def read_batch_in_sequence(api_instance, dataset_id: str, starting_record_id: str,
                                batch_size: int):
         sequence_read_request = SequenceReadRequest(dataset_id=dataset_id,
@@ -94,15 +95,16 @@
             :returns: List of records
 
             :rtype: RecordBatch
         """
         with kdp_api.ApiClient(config) as api_client:
             api_instance = read_and_query_api.ReadAndQueryApi(api_client)
 
-            request = {}
-            request['datasetId'] = dataset_id
-            request['excludeStartingRecordId'] = exclude_starting_record_id
-            request['startingRecordId'] = starting_record_id
-            request['endingRecordId'] = ending_record_id
-            request['batchSize'] = batch_size
+            read_range_request = ReadRangeRequest(
+              datasetId=dataset_id,
+              excludeStartingRecordId=exclude_starting_record_id,
+              startingRecordId=starting_record_id,
+              endingRecordId=ending_record_id,
+              batchSize=batch_size
+            )
 
-            return api_instance.post_read(request)
+            return api_instance.post_read(read_range_request)
```

### Comparing `kdp-python-connector-0.60.0/kdp_connector/connectors/upload.py` & `kdp-python-connector-0.62.0/kdp_connector/connectors/upload.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/kdp_connector/main.py` & `kdp-python-connector-0.62.0/kdp_connector/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from kdp_api import DatasetPatchRequest
+
 from kdp_connector.configuration.configurationUtil import ConfigurationUtil
 from kdp_connector.configuration.authenticationUtil import AuthenticationUtil
 from kdp_connector.configuration.keycloak_authentication import KeycloakAuthentication
 from kdp_connector.connectors.batch_write import WriteApi
 from kdp_connector.connectors.ingest_job_api import IngestJobApi
 from kdp_connector.connectors.read import ReadApi
 from kdp_connector.connectors.kdp_api import KdpApi
@@ -102,22 +104,22 @@
 
         print('Calling to get koverse token from keycloak login')
 
         return auth_util.get_koverse_token_from_keycloak_login(config=config, keycloak=keycloak_auth, workspace_id=workspace_id)
 
     # , kc_username: str, kc_password: str,
     # WRITE
-    def batch_write(self, dataframe, dataset_id: str, jwt: str, batch_size: int = 100, is_async: bool = True):
+    def batch_write(self, dataframe, dataset_id: str, jwt: str, batch_size: int = 100, is_async: bool = False):
         """This method will be used to write batches of data to KDP
 
             :param DataFrame dataframe: Data to write to KDP
             :param str dataset_id: ID of the KDP dataset where the data will be written
             :param str jwt: JWT token
             :param int batch_size: Defaults to 100
-            :param bool is_async: Defaults to True
+            :param bool is_async: Defaults to False
 
             :returns: Set of partitions data was written to
 
             :rtype: set
         """
         config = self.create_configuration(jwt)
         write_api = WriteApi(configuration=config)
@@ -274,15 +276,15 @@
         return read_api.read_batch(config=config, dataset_id=dataset_id, starting_record_id=starting_record_id,
                                    ending_record_id=ending_record_id,
                                    exclude_starting_record_id=exclude_starting_record_id,
                                    batch_size=batch_size)
 
     # dataset
     def create_dataset(self, name: str, workspace_id: str, jwt: str, description: str = '',
-                       auto_create_indexes: bool = True, schema: dict = '{}', search_any_field: bool = True,
+                       auto_create_indexes: bool = True, schema: any = None, search_any_field: bool = True,
                        record_count: int = 0):
         """This method will create a new KDP dataset
 
             :param str name: Name of dataset to create
             :param str workspace_id: Workspace that dataset will be created in
             :param str jwt: JWT token
             :param str description: Description of dataset
@@ -293,16 +295,22 @@
 
             :returns: New dataset
 
             :rtype: Dataset
         """
         kdp_api = KdpApi()
         config = self.create_configuration(jwt)
-        return kdp_api.create_dataset(config, name, workspace_id, description, auto_create_indexes, schema,
-                                      search_any_field, record_count)
+        return kdp_api.create_dataset(config,
+                                      name,
+                                      workspace_id,
+                                      description,
+                                      auto_create_indexes,
+                                      {} if schema is None else schema,
+                                      search_any_field,
+                                      record_count)
 
     def get_dataset(self, dataset_id, jwt):
         """This method will get a dataset by id
 
             :param str dataset_id: ID of dataset
             :param str jwt: JWT token
 
@@ -310,15 +318,15 @@
 
             :rtype: Dataset
         """
         kdp_api = KdpApi()
         config = self.create_configuration(jwt)
         return kdp_api.get_dataset(config, dataset_id)
 
-    def patch_dataset(self, dataset_id, payload, jwt):
+    def patch_dataset(self, dataset_id, payload: DatasetPatchRequest, jwt):
         """This method will update fields in a dataset
 
             :param str dataset_id: ID of dataset
             :param PatchDataset payload: Payload with the fields to update
             :param str jwt: JWT token
 
             :returns: Dataset
```

### Comparing `kdp-python-connector-0.60.0/kdp_python_connector.egg-info/PKG-INFO` & `kdp-python-connector-0.62.0/kdp_python_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kdp-python-connector
-Version: 0.60.0
+Version: 0.62.0
 Summary: Python Connector for KDP Platform
 Author-email: Koverse development team <developer@koverse.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: kdp-api-python-client~=4.125.0
+Requires-Dist: kdp-api-python-client~=4.126.0
 Requires-Dist: pandas~=1.4.2
 Requires-Dist: numpy~=1.22.4
 
 # kdp-python-connector
 
 ## Prequisites
 * Python version 3.8.5
```

### Comparing `kdp-python-connector-0.60.0/kdp_python_connector.egg-info/SOURCES.txt` & `kdp-python-connector-0.62.0/kdp_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/pyproject.toml` & `kdp-python-connector-0.62.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "0.60.0"
+version = "0.62.0"
 dependencies = [
-  'kdp-api-python-client ~= 4.125.0',
+  'kdp-api-python-client ~= 4.126.0',
   'pandas ~= 1.4.2',
   'numpy ~= 1.22.4'
 ]
 
 [tool.setuptools.packages.find]
 include = ["kdp_connector"]
```

### Comparing `kdp-python-connector-0.60.0/test/test_ingest.py` & `kdp-python-connector-0.62.0/test/test_ingest.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         self.host = 'https://api.koverse.localhost'
         self.input_file = '~/documents/Test documents/WithDates.csv'
         self.write_batch_response = WriteBatchResponse(workspace=self.workspace_id,
                                                        dataset_id=self.dataset_id,
                                                        partitions=[0, 1])
         self.api_instance = Mock()
         self.api_instance.post_write_id.return_value = self.write_batch_response
+        self.configuration = Mock()
+        self.configuration.host = self.host
 
     @staticmethod
     def getDataframe(size: int):
         data = []
         for x in range(size):
             data.append({'name': 'tom', 'age': 20 + x})
         return pd.DataFrame(data)
@@ -45,37 +47,39 @@
             TestCase(records=0, batch_size=10, expected_batches=0),
             TestCase(records=10, batch_size=1000, expected_batches=1),
             TestCase(records=11, batch_size=10, expected_batches=2),
         ]
         for case in test_cases:
             self.setup()
             mock_api_instance = self.api_instance
+            mock_configuration = self.configuration
 
             with(mock.patch('kdp_api.ApiClient')):
-                with(mock.patch('kdp_api.Configuration')):
+                with(mock.patch('kdp_api.Configuration', side_effect=[mock_configuration])):
                     with(mock.patch('kdp_api.api.write_api.WriteApi', side_effect=[mock_api_instance])):
                         kdp_conn = KdpConn()
                         partitions_set = kdp_conn.batch_write(self.getDataframe(case.records), self.dataset_id, self.JWT,
                                                               case.batch_size)
                         self.assertEqual(len(mock_api_instance.post_write_id.mock_calls), case.expected_batches,
                                          'FAILURE: for records=' + str(case.records) +
                                          ' and batch_size=' + str(case.batch_size) +
                                          ' expected_batches did not equal ' + str(case.expected_batches))
 
     def test_ingest_dataframe(self):
         self.setup()
         self.batch_size = 10
         mock_api_instance = self.api_instance
+        mock_configuration = self.configuration
         expected_write_calls = [call(dataset_id=self.dataset_id,
-                                     json_record=[{'name': 'tom', 'age': 20}, {'name': 'tom', 'age': 21},
+                                     request_body=[{'name': 'tom', 'age': 20}, {'name': 'tom', 'age': 21},
                                                   {'name': 'tom', 'age': 22}, {'name': 'tom', 'age': 23}],
                                      is_async=False)]
 
         with(mock.patch('kdp_api.ApiClient')):
-            with(mock.patch('kdp_api.Configuration')):
+            with(mock.patch('kdp_api.Configuration', side_effect=[mock_configuration])):
                 with(mock.patch('kdp_api.api.write_api.WriteApi', side_effect=[mock_api_instance])):
                     self.setup()
                     self.batch_size = 10
                     kdp_conn = KdpConn()
                     partitions_set = kdp_conn.batch_write(self.getDataframe(4), self.dataset_id, self.JWT,
                                                           self.batch_size)
                     mock_api_instance.post_write_id.assert_has_calls(expected_write_calls)
```

### Comparing `kdp-python-connector-0.60.0/test/test_keycloak.py` & `kdp-python-connector-0.62.0/test/test_keycloak.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.60.0/test/test_read.py` & `kdp-python-connector-0.62.0/test/test_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import unittest
 from unittest.mock import Mock, call, ANY
 
-from kdp_api.models.json_record import JsonRecord
 from pandas._testing import assert_frame_equal
 
 import pandas as pd
 
 from kdp_connector.connectors.read import ReadApi
 from kdp_api.models import RecordBatch
 from kdp_connector.main import KdpConn
@@ -72,23 +71,23 @@
         expected_dataframe = pd.DataFrame(expected_list)
 
         assert_frame_equal(expected_dataframe, dataframe)
 
     @staticmethod
     def getRecords():
         # Including data to test that the dataframe gets the correct data
-        first_json_record = JsonRecord(record={'a': 3})
-        second_json_record = JsonRecord(record={'b': 4})
+        first_json_record = {"record": {'a': 3}}
+        second_json_record = {"record": {'b': 4}}
         return [first_json_record, second_json_record]
 
     @staticmethod
     def getDataStoreList(json_record_list):
         result_list = []
         for json_record in json_record_list:
-            result_list.append(json_record['_data_store'])
+            result_list.append(json_record['record'])
 
         return result_list
 
 
     def getRecordBatch(self):
         record_batch = RecordBatch()
         record_batch.records = self.getRecords()
```

