# Comparing `tmp/sagemaker-jupyterlab-extension-common-0.1.8.tar.gz` & `tmp/sagemaker-jupyterlab-extension-common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-jupyterlab-extension-common-0.1.8.tar", last modified: Wed Nov  8 02:48:49 2023, max compression
+gzip compressed data, was "sagemaker-jupyterlab-extension-common-0.1.9.tar", last modified: Wed Nov  8 08:02:19 2023, max compression
```

## Comparing `sagemaker-jupyterlab-extension-common-0.1.8.tar` & `sagemaker-jupyterlab-extension-common-0.1.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.016822 sagemaker-jupyterlab-extension-common-0.1.8/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4755 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/LICENSE
--rw-r--r--   0 p4admin  (12569) amazon     (100)      749 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/MANIFEST.in
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2182 2023-11-08 02:48:49.016822 sagemaker-jupyterlab-extension-common-0.1.8/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1232 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/README.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)    14623 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/THIRD-PARTY-LICENSES
--rw-r--r--   0 p4admin  (12569) amazon     (100)      240 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/install.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:48.992822 sagemaker-jupyterlab-extension-common-0.1.8/jupyter-config/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.000822 sagemaker-jupyterlab-extension-common-0.1.8/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2336 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.000822 sagemaker-jupyterlab-extension-common-0.1.8/public_dist/
--rw-r--r--   0 p4admin  (12569) amazon     (100)   272443 2023-11-08 02:47:57.000000 sagemaker-jupyterlab-extension-common-0.1.8/public_dist/sagemaker_jupyterlab_extension_common-0.1.8-py3-none-any.whl
--rw-r--r--   0 p4admin  (12569) amazon     (100)      155 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/pyproject.toml
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.000822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      812 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      683 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/_version.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:48.996822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/botocore_model/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:48.996822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.004822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/
--rw-r--r--   0 p4admin  (12569) amazon     (100)  1378776 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/service-2.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5942 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      978 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/constants.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3674 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/handlers.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.004822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2452 2023-11-08 02:48:45.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.008822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5073 2023-11-08 02:48:45.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/117.e01e1fff3ce2e26893fe.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1949 2023-11-08 02:48:45.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/38.15ae4750d35a3729c290.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1949 2023-11-08 02:48:45.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/512.769ffeae9d7cc23f13a4.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8229 2023-11-08 02:48:45.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/687.d1a4669887f7c4f5716c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3758 2023-11-08 02:48:45.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/936.c7888f92b7d8a8d28b6a.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7751 2023-11-08 02:48:45.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.c75f0e99e1799c6fa7c3.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-11-08 02:48:44.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/style.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6761 2023-11-08 02:48:45.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.008822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    10666 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/logging_utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.008822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2292 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/handler_metrics_schema.yml
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3664 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_client_performance_metrics_schema.yml
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1950 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_operation_log_schema.yml
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1781 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/log_schema.yml
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2527 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/request_metrics_schema.yml
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/py.typed
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.012822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       67 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2354 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/test_app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9281 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/test_clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4050 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/test_handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    11038 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/test_logging_utils.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      527 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.012822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/util/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/util/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1679 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/util/app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2327 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/util/file_watcher.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.004822 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2182 2023-11-08 02:48:48.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3508 2023-11-08 02:48:48.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/SOURCES.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-11-08 02:48:48.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/dependency_links.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-11-08 02:47:42.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/not-zip-safe
--rw-r--r--   0 p4admin  (12569) amazon     (100)      140 2023-11-08 02:48:48.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/requires.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-11-08 02:48:48.000000 sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/top_level.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-11-08 02:48:49.020823 sagemaker-jupyterlab-extension-common-0.1.8/setup.cfg
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2955 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/setup.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.012822 sagemaker-jupyterlab-extension-common-0.1.8/src/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.012822 sagemaker-jupyterlab-extension-common-0.1.8/src/constants/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      228 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/constants/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      175 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/constants/fetchapi.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       80 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/constants/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      814 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/constants/logger.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      223 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.012822 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.012822 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1212 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/LoggerPlugin.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.016822 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2556 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/__tests__/LoggerPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1941 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/__tests__/logger.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2710 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/handlers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       32 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2473 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/logger.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      503 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/utils.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.016822 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1005 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/PanoramaPlugin.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.016822 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      733 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/__tests__/utils.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       34 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      536 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/utils.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.016822 sagemaker-jupyterlab-extension-common-0.1.8/src/services/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1143 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/services/fetchapi.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       28 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/services/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 02:48:49.016822 sagemaker-jupyterlab-extension-common-0.1.8/src/types/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       26 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/types/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2146 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/src/types/logger.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9748 2023-11-08 02:35:29.000000 sagemaker-jupyterlab-extension-common-0.1.8/tsconfig.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.469063 sagemaker-jupyterlab-extension-common-0.1.9/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4755 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/LICENSE
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      749 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/MANIFEST.in
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2182 2023-11-08 08:02:19.469063 sagemaker-jupyterlab-extension-common-0.1.9/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1232 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/README.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    14623 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/THIRD-PARTY-LICENSES
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      240 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/install.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.449063 sagemaker-jupyterlab-extension-common-0.1.9/jupyter-config/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.453063 sagemaker-jupyterlab-extension-common-0.1.9/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2336 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.453063 sagemaker-jupyterlab-extension-common-0.1.9/public_dist/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   272497 2023-11-08 08:01:25.000000 sagemaker-jupyterlab-extension-common-0.1.9/public_dist/sagemaker_jupyterlab_extension_common-0.1.9-py3-none-any.whl
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      155 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/pyproject.toml
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.457063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      812 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      683 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/_version.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.449063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/botocore_model/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.449063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.457063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  1378776 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/service-2.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5942 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      978 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/constants.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3766 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/handlers.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.457063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2452 2023-11-08 08:02:16.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.461063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5073 2023-11-08 08:02:16.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/117.e01e1fff3ce2e26893fe.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1949 2023-11-08 08:02:16.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/38.15ae4750d35a3729c290.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1949 2023-11-08 08:02:16.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/512.769ffeae9d7cc23f13a4.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8229 2023-11-08 08:02:16.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/687.d1a4669887f7c4f5716c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3758 2023-11-08 08:02:16.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/936.e849b05e674b2ed3d783.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7751 2023-11-08 08:02:16.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.b855f9574044219a399a.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-11-08 08:02:14.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/style.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6761 2023-11-08 08:02:16.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.461063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    10823 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/logging_utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.461063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2292 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/handler_metrics_schema.yml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3664 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_client_performance_metrics_schema.yml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1950 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_operation_log_schema.yml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1781 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/log_schema.yml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2527 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/request_metrics_schema.yml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/py.typed
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.465063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       67 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2354 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/test_app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9281 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/test_clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4050 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/test_handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    11038 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/test_logging_utils.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      527 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.465063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/util/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/util/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1679 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/util/app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2327 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/util/file_watcher.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.457063 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2182 2023-11-08 08:02:19.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3508 2023-11-08 08:02:19.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/SOURCES.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-11-08 08:02:19.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/dependency_links.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-11-08 08:01:10.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/not-zip-safe
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      140 2023-11-08 08:02:19.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/requires.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-11-08 08:02:19.000000 sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/top_level.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-11-08 08:02:19.469063 sagemaker-jupyterlab-extension-common-0.1.9/setup.cfg
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2955 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/setup.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.465063 sagemaker-jupyterlab-extension-common-0.1.9/src/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.465063 sagemaker-jupyterlab-extension-common-0.1.9/src/constants/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      228 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/constants/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      175 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/constants/fetchapi.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       80 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/constants/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      814 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/constants/logger.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      223 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.465063 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.465063 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1212 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/LoggerPlugin.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.465063 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2556 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/__tests__/LoggerPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1941 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/__tests__/logger.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2710 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/handlers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       32 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2473 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/logger.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      503 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/utils.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.469063 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1005 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/PanoramaPlugin.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.469063 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      733 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/__tests__/utils.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       34 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      536 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/utils.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.469063 sagemaker-jupyterlab-extension-common-0.1.9/src/services/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1143 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/services/fetchapi.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       28 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/services/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-11-08 08:02:19.469063 sagemaker-jupyterlab-extension-common-0.1.9/src/types/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       26 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/types/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2146 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/src/types/logger.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9748 2023-11-08 07:48:40.000000 sagemaker-jupyterlab-extension-common-0.1.9/tsconfig.json
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/LICENSE` & `sagemaker-jupyterlab-extension-common-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/MANIFEST.in` & `sagemaker-jupyterlab-extension-common-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/PKG-INFO` & `sagemaker-jupyterlab-extension-common-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension-common
-Version: 0.1.8
+Version: 0.1.9
 Summary: SageMaker JupyterLab workspace common module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/README.md` & `sagemaker-jupyterlab-extension-common-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/THIRD-PARTY-LICENSES` & `sagemaker-jupyterlab-extension-common-0.1.9/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/package.json` & `sagemaker-jupyterlab-extension-common-0.1.9/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.9'"}*

```diff
@@ -65,9 +65,9 @@
         "lint:fix": "eslint --fix . --ext .js,.ts,.tsx",
         "release": "run-s build",
         "test": "jest",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/public_dist/sagemaker_jupyterlab_extension_common-0.1.8-py3-none-any.whl` & `sagemaker-jupyterlab-extension-common-0.1.9/public_dist/sagemaker_jupyterlab_extension_common-0.1.9-py3-none-any.whl`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,51 +1,51 @@
-Zip file size: 272443 bytes, number of entries: 49
+Zip file size: 272497 bytes, number of entries: 49
 -rw-r--r--  2.0 unx      812 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/__init__.py
 -rw-r--r--  2.0 unx      683 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/_version.py
 -rw-r--r--  2.0 unx     5942 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/clients.py
 -rw-r--r--  2.0 unx      978 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/constants.py
--rw-r--r--  2.0 unx     3674 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/handlers.py
+-rw-r--r--  2.0 unx     3766 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/handlers.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/py.typed
 -rw-r--r--  2.0 unx  1378776 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/service-2.json
 -rw-r--r--  2.0 unx     2452 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/package.json
 -rw-r--r--  2.0 unx     5073 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/117.e01e1fff3ce2e26893fe.js
 -rw-r--r--  2.0 unx     1949 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/38.15ae4750d35a3729c290.js
 -rw-r--r--  2.0 unx     1949 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/512.769ffeae9d7cc23f13a4.js
 -rw-r--r--  2.0 unx     8229 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/687.d1a4669887f7c4f5716c.js
--rw-r--r--  2.0 unx     3758 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/936.c7888f92b7d8a8d28b6a.js
--rw-r--r--  2.0 unx     7751 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.c75f0e99e1799c6fa7c3.js
+-rw-r--r--  2.0 unx     3758 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/936.e849b05e674b2ed3d783.js
+-rw-r--r--  2.0 unx     7751 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.b855f9574044219a399a.js
 -rw-r--r--  2.0 unx      118 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/style.js
 -rw-r--r--  2.0 unx     6761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/labextension/static/third-party-licenses.json
 -rw-r--r--  2.0 unx       66 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/logging/__init__.py
--rw-r--r--  2.0 unx    10666 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/logging/logging_utils.py
+-rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/logging/logging_utils.py
 -rw-r--r--  2.0 unx     2292 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/logging/schemas/handler_metrics_schema.yml
 -rw-r--r--  2.0 unx     3664 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_client_performance_metrics_schema.yml
 -rw-r--r--  2.0 unx     1950 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_operation_log_schema.yml
 -rw-r--r--  2.0 unx     1781 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/logging/schemas/log_schema.yml
 -rw-r--r--  2.0 unx     2527 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/logging/schemas/request_metrics_schema.yml
 -rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/tests/__init__.py
 -rw-r--r--  2.0 unx     2354 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/tests/test_app_metadata.py
 -rw-r--r--  2.0 unx     9281 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/tests/test_clients.py
 -rw-r--r--  2.0 unx     4050 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/tests/test_handlers.py
 -rw-r--r--  2.0 unx    11038 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/tests/test_logging_utils.py
 -rw-r--r--  2.0 unx      527 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/tests/utils.py
 -rw-r--r--  2.0 unx       66 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/util/__init__.py
 -rw-r--r--  2.0 unx     1679 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/util/app_metadata.py
 -rw-r--r--  2.0 unx     2327 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common/util/file_watcher.py
--rw-r--r--  2.0 unx    14623 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/THIRD-PARTY-LICENSES
--rw-r--r--  2.0 unx      123 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json
--rw-r--r--  2.0 unx      240 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/install.json
--rw-r--r--  2.0 unx     2452 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/package.json
--rw-r--r--  2.0 unx     5073 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/117.e01e1fff3ce2e26893fe.js
--rw-r--r--  2.0 unx     1949 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/38.15ae4750d35a3729c290.js
--rw-r--r--  2.0 unx     1949 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/512.769ffeae9d7cc23f13a4.js
--rw-r--r--  2.0 unx     8229 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/687.d1a4669887f7c4f5716c.js
--rw-r--r--  2.0 unx     3758 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/936.c7888f92b7d8a8d28b6a.js
--rw-r--r--  2.0 unx     7751 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/remoteEntry.c75f0e99e1799c6fa7c3.js
--rw-r--r--  2.0 unx      118 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/style.js
--rw-r--r--  2.0 unx     6761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/third-party-licenses.json
--rw-r--r--  2.0 unx     4755 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2191 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6952 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.8.dist-info/RECORD
-49 files, 1550294 bytes uncompressed, 260241 bytes compressed:  83.2%
+-rw-r--r--  2.0 unx    14623 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/THIRD-PARTY-LICENSES
+-rw-r--r--  2.0 unx      123 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json
+-rw-r--r--  2.0 unx      240 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/install.json
+-rw-r--r--  2.0 unx     2452 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/package.json
+-rw-r--r--  2.0 unx     5073 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/117.e01e1fff3ce2e26893fe.js
+-rw-r--r--  2.0 unx     1949 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/38.15ae4750d35a3729c290.js
+-rw-r--r--  2.0 unx     1949 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/512.769ffeae9d7cc23f13a4.js
+-rw-r--r--  2.0 unx     8229 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/687.d1a4669887f7c4f5716c.js
+-rw-r--r--  2.0 unx     3758 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/936.e849b05e674b2ed3d783.js
+-rw-r--r--  2.0 unx     7751 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/remoteEntry.b855f9574044219a399a.js
+-rw-r--r--  2.0 unx      118 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/style.js
+-rw-r--r--  2.0 unx     6761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/third-party-licenses.json
+-rw-r--r--  2.0 unx     4755 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2191 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6952 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension_common-0.1.9.dist-info/RECORD
+49 files, 1550543 bytes uncompressed, 260295 bytes compressed:  83.2%
```

#### zipnote «TEMP»/diffoscope_kok8i350_/tmp0m0ozocy_.zip

```diff
@@ -30,18 +30,18 @@
 
 Filename: sagemaker_jupyterlab_extension_common/labextension/static/512.769ffeae9d7cc23f13a4.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension_common/labextension/static/687.d1a4669887f7c4f5716c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common/labextension/static/936.c7888f92b7d8a8d28b6a.js
+Filename: sagemaker_jupyterlab_extension_common/labextension/static/936.e849b05e674b2ed3d783.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.c75f0e99e1799c6fa7c3.js
+Filename: sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.b855f9574044219a399a.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension_common/labextension/static/style.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension_common/labextension/static/third-party-licenses.json
 Comment: 
@@ -90,59 +90,59 @@
 
 Filename: sagemaker_jupyterlab_extension_common/util/app_metadata.py
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension_common/util/file_watcher.py
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/THIRD-PARTY-LICENSES
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/THIRD-PARTY-LICENSES
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/install.json
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/install.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/package.json
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/package.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/117.e01e1fff3ce2e26893fe.js
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/117.e01e1fff3ce2e26893fe.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/38.15ae4750d35a3729c290.js
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/38.15ae4750d35a3729c290.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/512.769ffeae9d7cc23f13a4.js
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/512.769ffeae9d7cc23f13a4.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/687.d1a4669887f7c4f5716c.js
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/687.d1a4669887f7c4f5716c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/936.c7888f92b7d8a8d28b6a.js
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/936.e849b05e674b2ed3d783.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/remoteEntry.c75f0e99e1799c6fa7c3.js
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/remoteEntry.b855f9574044219a399a.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/style.js
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/style.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/third-party-licenses.json
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/third-party-licenses.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.dist-info/LICENSE
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.dist-info/METADATA
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.dist-info/WHEEL
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.dist-info/top_level.txt
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension_common-0.1.8.dist-info/RECORD
+Filename: sagemaker_jupyterlab_extension_common-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### sagemaker_jupyterlab_extension_common/handlers.py

```diff
@@ -19,15 +19,18 @@
     """Handle event log requests emitted by Studio JupyterLab UI"""
 
     eventlog_instance = None
 
     def get_eventlog(self):
         if not JupterLabUILogHandler.eventlog_instance:
             """ "Create a StudioEventLog with the correct schemas"""
-            schema_documents = [SchemaDocument.JupyterLabOperation]
+            schema_documents = [
+                SchemaDocument.JupyterLabOperation,
+                SchemaDocument.JupyterLabPerformanceMetrics,
+            ]
             JupterLabUILogHandler.eventlog_instance = create_ui_eventlogger(
                 schema_documents
             )
         return JupterLabUILogHandler.eventlog_instance
 
     def inject_log_context(self, event_record):
         if event_record and "Context" in event_record:
```

#### sagemaker_jupyterlab_extension_common/labextension/package.json

##### Pretty-printed

 * *Similarity: 0.962797619047619%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b855f9574044219a399a.js'}}",*

 * * "'version'": "'0.1.9'"}*

```diff
@@ -42,15 +42,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c75f0e99e1799c6fa7c3.js"
+            "load": "static/remoteEntry.b855f9574044219a399a.js"
         },
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension_common/labextension"
     },
     "license": "Amazon Software License",
     "licenses": [
         {
@@ -69,9 +69,9 @@
         "lint:fix": "eslint --fix . --ext .js,.ts,.tsx",
         "release": "run-s build",
         "test": "jest",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

#### sagemaker_jupyterlab_extension_common/logging/logging_utils.py

```diff
@@ -3,14 +3,15 @@
 import os
 import os.path
 from enum import Enum
 from pathlib import Path
 
 from traitlets import log
 from jupyter_events.logger import EventLogger
+from jupyter_events.schema_registry import SchemaRegistryException
 from aws_embedded_metrics.logger.metrics_context import MetricsContext
 from aws_embedded_metrics.serializers.log_serializer import LogSerializer
 
 from sagemaker_jupyterlab_extension_common.util.app_metadata import (
     get_domain_id,
     get_aws_account_id,
     get_space_name,
@@ -277,19 +278,22 @@
             self, self.jl_extension_name, self.jl_extension_version
         )
 
 
 def create_ui_eventlogger(schema_documents):
     eventlog = _default_eventlog
     for schema_document in schema_documents:
-        handler = get_handler(schema_document)
-        # Add filter for handler
-        handler.addFilter(schema_document.get_log_event_filter())
-        eventlog.register_handler(handler)
-        eventlog.register_event_schema(schema_document.get_schema_file_path())
+        try:
+            handler = get_handler(schema_document)
+            # Add filter for handler
+            handler.addFilter(schema_document.get_log_event_filter())
+            eventlog.register_handler(handler)
+            eventlog.register_event_schema(schema_document.get_schema_file_path())
+        except SchemaRegistryException:
+            pass
     return eventlog
 
 
 class SchemaDocumentLogFilter:
     def __init__(self, schema_document):
         self.schema_document = schema_document
         self.schema_filter = list(
```

#### Comparing `sagemaker_jupyterlab_extension_common/labextension/static/936.c7888f92b7d8a8d28b6a.js` & `sagemaker_jupyterlab_extension_common/labextension/static/936.e849b05e674b2ed3d783.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -103,15 +103,15 @@
                     return this.eventLog.recordEvent({
                         version: this.schema.schemaVersion,
                         schema: this.schema.schemaId,
                         body: this.format(e, t)
                     })
                 }
             }
-            var f = r(768);
+            var f = r(495);
             const y = [d, {
                 id: s,
                 autoStart: !0,
                 provides: u,
                 activate: e => {
                     const t = {
                             SessionId: (e => {
```

#### Comparing `sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.c75f0e99e1799c6fa7c3.js` & `sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.b855f9574044219a399a.js`

 * *Files 6% similar despite different names*

##### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, d, c, p, h, m, b, v, g, y = {
-            222: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, f, s, d, c, p, h, m, b, v, g, y = {
+            801: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(713), t.e(936)]).then((() => () => t(936))),
                         "./extension": () => Promise.all([t.e(713), t.e(936)]).then((() => () => t(936)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         w = {};
 
     function j(e) {
         var r = w[e];
@@ -47,47 +47,47 @@
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         38: "15ae4750d35a3729c290",
         117: "e01e1fff3ce2e26893fe",
         512: "769ffeae9d7cc23f13a4",
         687: "d1a4669887f7c4f5716c",
         713: "6ec4e1111ab220edbbdf",
         901: "8f38b8390513a01e8ffb",
-        936: "c7888f92b7d8a8d28b6a"
+        936: "e849b05e674b2ed3d783"
     } [e] + ".js?v=" + {
         38: "15ae4750d35a3729c290",
         117: "e01e1fff3ce2e26893fe",
         512: "769ffeae9d7cc23f13a4",
         687: "d1a4669887f7c4f5716c",
         713: "6ec4e1111ab220edbbdf",
         901: "8f38b8390513a01e8ffb",
-        936: "c7888f92b7d8a8d28b6a"
+        936: "e849b05e674b2ed3d783"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amzn/sagemaker-jupyterlab-extension-common:", j.l = (t, n, a, o) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amzn/sagemaker-jupyterlab-extension-common:", j.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
-                        i = f;
+            if (void 0 !== o)
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
@@ -99,31 +99,31 @@
         })
     }, (() => {
         j.S = {};
         var e = {},
             r = {};
         j.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 j.o(j.S, t) || (j.S[t] = {});
-                var o = j.S[t],
+                var a = j.S[t],
                     i = "@amzn/sagemaker-jupyterlab-extension-common",
                     u = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            u = a[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
+                        var o = a[e] = a[e] || {},
+                            u = o[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("@amzn/sagemaker-jupyterlab-extension-common", "0.1.8", (() => Promise.all([j.e(713), j.e(936)]).then((() => () => j(936))))), u("@jupyterlab/jupyterlab-telemetry", "1.0.3", (() => Promise.all([j.e(713), j.e(901), j.e(512)]).then((() => () => j(512))))), u("p-retry", "6.1.0", (() => j.e(117).then((() => () => j(117))))), u("uuid", "9.0.1", (() => j.e(687).then((() => () => j(687)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@amzn/sagemaker-jupyterlab-extension-common", "0.1.9", (() => Promise.all([j.e(713), j.e(936)]).then((() => () => j(936))))), u("@jupyterlab/jupyterlab-telemetry", "1.0.3", (() => Promise.all([j.e(713), j.e(901), j.e(512)]).then((() => () => j(512))))), u("p-retry", "6.1.0", (() => j.e(117).then((() => () => j(117))))), u("uuid", "9.0.1", (() => j.e(687).then((() => () => j(687)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -138,161 +138,161 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 u = (typeof i)[0];
-            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
-                if ("u" == f) {
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
                     if (!l || "u" != d) return !1
                 } else if (l)
-                    if (d == f)
+                    if (d == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (a ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
-                    if (a || u <= n) return !1;
+                    if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != a) return !1;
+                    if (u <= n || s < d != o) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
-        var a = u(e, t);
-        return o(n, a) || d(l(e, t, a, n)), c(e[t][a])
-    }, f = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+        var o = u(e, t);
+        return a(n, o) || d(l(e, t, o, n)), c(e[t][o])
+    }, s = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, a) {
-        var o = j.I(r);
-        return o && o.then ? o.then(e.bind(e, r, j.S[r], t, n, a)) : e(r, j.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), m = p(((e, r, t, n, a) => {
-        var o = r && j.o(r, t) && f(r, t, n);
-        return o ? c(o) : a()
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+        var a = j.I(r);
+        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = p(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && s(r, t, n);
+        return a ? c(a) : o()
     })), b = {}, v = {
         858: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 8]),
         976: () => h("default", "@jupyterlab/services", [1, 7, 0, 8]),
         13: () => m("default", "uuid", [1, 9, 0, 1], (() => j.e(687).then((() => () => j(687))))),
         321: () => m("default", "p-retry", [1, 6, 1, 0], (() => j.e(117).then((() => () => j(117))))),
-        768: () => m("default", "@jupyterlab/jupyterlab-telemetry", [1, 1, 0, 3], (() => Promise.all([j.e(901), j.e(38)]).then((() => () => j(512))))),
+        495: () => m("default", "@jupyterlab/jupyterlab-telemetry", [1, 1, 0, 3], (() => Promise.all([j.e(901), j.e(38)]).then((() => () => j(512))))),
         930: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         901: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
     }, g = {
         713: [858, 976],
         901: [901],
-        936: [13, 321, 768, 930]
+        936: [13, 321, 495, 930]
     }, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete b[e], j.m[e] = t => {
                         throw delete j.c[e], r
                     }
                 };
             try {
-                var a = v[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var o = v[e]();
+                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             61: 0
         };
         j.f.j = (r, t) => {
             var n = j.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (/^(713|901)$/.test(r)) e[r] = 0;
             else {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
-                var o = j.p + j.u(r),
+                var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                t.push(n[2] = o);
+                var a = j.p + j.u(r),
                     i = new Error;
-                j.l(o, (t => {
+                j.l(a, (t => {
                     if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                        var o = t && ("load" === t.type ? "missing" : t.type),
+                            a = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var n, a, [o, i, u] = t,
+                var n, o, [a, i, u] = t,
                     l = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) j.o(i, n) && (j.m[n] = i[n]);
                     u && u(j)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], j.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extension_common = self.webpackChunk_amzn_sagemaker_jupyterlab_extension_common || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var k = j(222);
+    var k = j(801);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extension-common"] = k
 })();
```

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/THIRD-PARTY-LICENSES` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/package.json` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/package.json`

 * *Files 2% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.962797619047619%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b855f9574044219a399a.js'}}",*

 * * "'version'": "'0.1.9'"}*

```diff
@@ -42,15 +42,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c75f0e99e1799c6fa7c3.js"
+            "load": "static/remoteEntry.b855f9574044219a399a.js"
         },
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension_common/labextension"
     },
     "license": "Amazon Software License",
     "licenses": [
         {
@@ -69,9 +69,9 @@
         "lint:fix": "eslint --fix . --ext .js,.ts,.tsx",
         "release": "run-s build",
         "test": "jest",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/117.e01e1fff3ce2e26893fe.js` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/117.e01e1fff3ce2e26893fe.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/38.15ae4750d35a3729c290.js` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/38.15ae4750d35a3729c290.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/512.769ffeae9d7cc23f13a4.js` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/512.769ffeae9d7cc23f13a4.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/687.d1a4669887f7c4f5716c.js` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/687.d1a4669887f7c4f5716c.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/936.c7888f92b7d8a8d28b6a.js` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/936.e849b05e674b2ed3d783.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -103,15 +103,15 @@
                     return this.eventLog.recordEvent({
                         version: this.schema.schemaVersion,
                         schema: this.schema.schemaId,
                         body: this.format(e, t)
                     })
                 }
             }
-            var f = r(768);
+            var f = r(495);
             const y = [d, {
                 id: s,
                 autoStart: !0,
                 provides: u,
                 activate: e => {
                     const t = {
                             SessionId: (e => {
```

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/remoteEntry.c75f0e99e1799c6fa7c3.js` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/remoteEntry.b855f9574044219a399a.js`

 * *Files 6% similar despite different names*

##### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, d, c, p, h, m, b, v, g, y = {
-            222: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, f, s, d, c, p, h, m, b, v, g, y = {
+            801: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(713), t.e(936)]).then((() => () => t(936))),
                         "./extension": () => Promise.all([t.e(713), t.e(936)]).then((() => () => t(936)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         w = {};
 
     function j(e) {
         var r = w[e];
@@ -47,47 +47,47 @@
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         38: "15ae4750d35a3729c290",
         117: "e01e1fff3ce2e26893fe",
         512: "769ffeae9d7cc23f13a4",
         687: "d1a4669887f7c4f5716c",
         713: "6ec4e1111ab220edbbdf",
         901: "8f38b8390513a01e8ffb",
-        936: "c7888f92b7d8a8d28b6a"
+        936: "e849b05e674b2ed3d783"
     } [e] + ".js?v=" + {
         38: "15ae4750d35a3729c290",
         117: "e01e1fff3ce2e26893fe",
         512: "769ffeae9d7cc23f13a4",
         687: "d1a4669887f7c4f5716c",
         713: "6ec4e1111ab220edbbdf",
         901: "8f38b8390513a01e8ffb",
-        936: "c7888f92b7d8a8d28b6a"
+        936: "e849b05e674b2ed3d783"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amzn/sagemaker-jupyterlab-extension-common:", j.l = (t, n, a, o) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amzn/sagemaker-jupyterlab-extension-common:", j.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
-                        i = f;
+            if (void 0 !== o)
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
@@ -99,31 +99,31 @@
         })
     }, (() => {
         j.S = {};
         var e = {},
             r = {};
         j.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 j.o(j.S, t) || (j.S[t] = {});
-                var o = j.S[t],
+                var a = j.S[t],
                     i = "@amzn/sagemaker-jupyterlab-extension-common",
                     u = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            u = a[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
+                        var o = a[e] = a[e] || {},
+                            u = o[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("@amzn/sagemaker-jupyterlab-extension-common", "0.1.8", (() => Promise.all([j.e(713), j.e(936)]).then((() => () => j(936))))), u("@jupyterlab/jupyterlab-telemetry", "1.0.3", (() => Promise.all([j.e(713), j.e(901), j.e(512)]).then((() => () => j(512))))), u("p-retry", "6.1.0", (() => j.e(117).then((() => () => j(117))))), u("uuid", "9.0.1", (() => j.e(687).then((() => () => j(687)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@amzn/sagemaker-jupyterlab-extension-common", "0.1.9", (() => Promise.all([j.e(713), j.e(936)]).then((() => () => j(936))))), u("@jupyterlab/jupyterlab-telemetry", "1.0.3", (() => Promise.all([j.e(713), j.e(901), j.e(512)]).then((() => () => j(512))))), u("p-retry", "6.1.0", (() => j.e(117).then((() => () => j(117))))), u("uuid", "9.0.1", (() => j.e(687).then((() => () => j(687)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -138,161 +138,161 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 u = (typeof i)[0];
-            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
-                if ("u" == f) {
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
                     if (!l || "u" != d) return !1
                 } else if (l)
-                    if (d == f)
+                    if (d == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (a ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
-                    if (a || u <= n) return !1;
+                    if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != a) return !1;
+                    if (u <= n || s < d != o) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
-        var a = u(e, t);
-        return o(n, a) || d(l(e, t, a, n)), c(e[t][a])
-    }, f = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+        var o = u(e, t);
+        return a(n, o) || d(l(e, t, o, n)), c(e[t][o])
+    }, s = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, a) {
-        var o = j.I(r);
-        return o && o.then ? o.then(e.bind(e, r, j.S[r], t, n, a)) : e(r, j.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), m = p(((e, r, t, n, a) => {
-        var o = r && j.o(r, t) && f(r, t, n);
-        return o ? c(o) : a()
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+        var a = j.I(r);
+        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = p(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && s(r, t, n);
+        return a ? c(a) : o()
     })), b = {}, v = {
         858: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 8]),
         976: () => h("default", "@jupyterlab/services", [1, 7, 0, 8]),
         13: () => m("default", "uuid", [1, 9, 0, 1], (() => j.e(687).then((() => () => j(687))))),
         321: () => m("default", "p-retry", [1, 6, 1, 0], (() => j.e(117).then((() => () => j(117))))),
-        768: () => m("default", "@jupyterlab/jupyterlab-telemetry", [1, 1, 0, 3], (() => Promise.all([j.e(901), j.e(38)]).then((() => () => j(512))))),
+        495: () => m("default", "@jupyterlab/jupyterlab-telemetry", [1, 1, 0, 3], (() => Promise.all([j.e(901), j.e(38)]).then((() => () => j(512))))),
         930: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         901: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
     }, g = {
         713: [858, 976],
         901: [901],
-        936: [13, 321, 768, 930]
+        936: [13, 321, 495, 930]
     }, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete b[e], j.m[e] = t => {
                         throw delete j.c[e], r
                     }
                 };
             try {
-                var a = v[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var o = v[e]();
+                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             61: 0
         };
         j.f.j = (r, t) => {
             var n = j.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (/^(713|901)$/.test(r)) e[r] = 0;
             else {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
-                var o = j.p + j.u(r),
+                var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                t.push(n[2] = o);
+                var a = j.p + j.u(r),
                     i = new Error;
-                j.l(o, (t => {
+                j.l(a, (t => {
                     if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                        var o = t && ("load" === t.type ? "missing" : t.type),
+                            a = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var n, a, [o, i, u] = t,
+                var n, o, [a, i, u] = t,
                     l = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) j.o(i, n) && (j.m[n] = i[n]);
                     u && u(j)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], j.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extension_common = self.webpackChunk_amzn_sagemaker_jupyterlab_extension_common || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var k = j(222);
+    var k = j(801);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extension-common"] = k
 })();
```

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/third-party-licenses.json` & `sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/third-party-licenses.json`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.dist-info/LICENSE` & `sagemaker_jupyterlab_extension_common-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.dist-info/METADATA` & `sagemaker_jupyterlab_extension_common-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension-common
-Version: 0.1.8
+Version: 0.1.9
 Summary: SageMaker JupyterLab workspace common module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

#### Comparing `sagemaker_jupyterlab_extension_common-0.1.8.dist-info/RECORD` & `sagemaker_jupyterlab_extension_common-0.1.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 sagemaker_jupyterlab_extension_common/__init__.py,sha256=P8ACHznRh5jjH9QJXVYBo8vFD5mX1U3tw4RGROKcjkc,812
 sagemaker_jupyterlab_extension_common/_version.py,sha256=H8LOQyA3X6Xj3pixozSSsatne-Jd9sIhfgCIwlM6AGg,683
 sagemaker_jupyterlab_extension_common/clients.py,sha256=Th-D6fycpDm9_rcYfJoGev7ENZ3qtjN4ArAO4Wg0Ue4,5942
 sagemaker_jupyterlab_extension_common/constants.py,sha256=7_-OlFmhltaL2R_clbzcqZcofWaRU_9ZkojiZ3472qo,978
-sagemaker_jupyterlab_extension_common/handlers.py,sha256=yNFSgjVXTsKlGcHVZKauxswyT8OzyzA7bWxFetHfTFg,3674
+sagemaker_jupyterlab_extension_common/handlers.py,sha256=jF93BBKAPa5yfjlhEc8FGoOvfsrwdTnho1UT0Dd2hmU,3766
 sagemaker_jupyterlab_extension_common/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/service-2.json,sha256=MR052fuTjylbk2Kg5s-nxosFLAkVk81RVSKeoRrDmow,1378776
-sagemaker_jupyterlab_extension_common/labextension/package.json,sha256=Z6Iig0n_bEIfviiUWEh8u6IKVhfsYdJ3s_UztoGJ-94,2452
+sagemaker_jupyterlab_extension_common/labextension/package.json,sha256=2O8XW2zrgS36p6u51DLiU_VKsxzI-cngL3ThFAH7ehU,2452
 sagemaker_jupyterlab_extension_common/labextension/static/117.e01e1fff3ce2e26893fe.js,sha256=4B4f_zzi4miT_jcBqmiRlEFy63ipNz2x19KOlNAuPIE,5073
 sagemaker_jupyterlab_extension_common/labextension/static/38.15ae4750d35a3729c290.js,sha256=Fa5HUNNaNynCkF3SZ7iwkT8Ya71A4MAX4J8v_0gm3EQ,1949
 sagemaker_jupyterlab_extension_common/labextension/static/512.769ffeae9d7cc23f13a4.js,sha256=dp_-rp18wj8TpKy6tt7xgpVy-ibXJxnb3OptkDdzHJA,1949
 sagemaker_jupyterlab_extension_common/labextension/static/687.d1a4669887f7c4f5716c.js,sha256=0aRmmIf3xPVxbDtH-8EaOJEyOGx4GQX2Y99zH-qfaRA,8229
-sagemaker_jupyterlab_extension_common/labextension/static/936.c7888f92b7d8a8d28b6a.js,sha256=x4iPkrfYqNKLanFPpLowLrNAz5NOfORlbj9p0TtYTSs,3758
-sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.c75f0e99e1799c6fa7c3.js,sha256=x18OmeF5nG-nw4eFq9U_pPeAdnHv9Qd85_qunbvZh44,7751
+sagemaker_jupyterlab_extension_common/labextension/static/936.e849b05e674b2ed3d783.js,sha256=6EmwXmdLLtPXg5z105Go_OtPRmm_MRe8j6X6Cjl8bNE,3758
+sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.b855f9574044219a399a.js,sha256=uFX5V0BEIZo5mm5mzdDACHIgqNM5qWOXWYOf2uRs6E0,7751
 sagemaker_jupyterlab_extension_common/labextension/static/style.js,sha256=-CQt0ZTPaCTvrRiLcznxflAbfvIKlOVzjOos-muaXQ8,118
 sagemaker_jupyterlab_extension_common/labextension/static/third-party-licenses.json,sha256=i8yhqwusdJETkbUBnGQKWEr2kpNwQJlDI0nCvZ8ng9o,6761
 sagemaker_jupyterlab_extension_common/logging/__init__.py,sha256=1I6YYNelr5hBJrNcxtFOJEHc-OzD95tsvUTFD1iUAx0,66
-sagemaker_jupyterlab_extension_common/logging/logging_utils.py,sha256=giXsocEKUstQoR35r3t_KqCZUj897as9HYdcyYWyzxw,10666
+sagemaker_jupyterlab_extension_common/logging/logging_utils.py,sha256=9bjnQSIxiqy4WT7WeokxXPW0BDG8AX6fIzyIYT9dVBk,10823
 sagemaker_jupyterlab_extension_common/logging/schemas/handler_metrics_schema.yml,sha256=fu-_hiYHy9Yq5VRnMf1vMVw03TVPgKTIyEbxYSk3gYI,2292
 sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_client_performance_metrics_schema.yml,sha256=JtkL_W1wbCoInCGqQ2bwezQ_9nJVOR59LZ4D1rHBjH0,3664
 sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_operation_log_schema.yml,sha256=CszkYo1C9zLqe_HwHazuTPhgeYClsQ0fu8d_gIP8-FA,1950
 sagemaker_jupyterlab_extension_common/logging/schemas/log_schema.yml,sha256=qpx-Dbi1kjpAmpOerm2yigmuSaNX5-1EbCJqXTmfN8M,1781
 sagemaker_jupyterlab_extension_common/logging/schemas/request_metrics_schema.yml,sha256=xuqDHjapJh2Ud1s47gEMfDSoNhD7mUvMQ9t2ZloCOMw,2527
 sagemaker_jupyterlab_extension_common/tests/__init__.py,sha256=4nLK1s0wHxpcnaDbf981H_Pa3FkFf8-t1Tw8A4yXqWo,67
 sagemaker_jupyterlab_extension_common/tests/test_app_metadata.py,sha256=Aa_TUnKYwgEBlIJnlK3ds1TcmyZPy7eRkiIcXUKMPvk,2354
 sagemaker_jupyterlab_extension_common/tests/test_clients.py,sha256=Mb8r6Yv9IV2BjUk1KOBfxt1lVHpwHqFDyzysl4qh_Tg,9281
 sagemaker_jupyterlab_extension_common/tests/test_handlers.py,sha256=QCFdiYEi1MNNNLGA75_RZckDhMXOUlqnoR5kqh9akBg,4050
 sagemaker_jupyterlab_extension_common/tests/test_logging_utils.py,sha256=t2MEnOFn77lcQlAnU2xYyWhe9DSlydmlRkpe0UKEWao,11038
 sagemaker_jupyterlab_extension_common/tests/utils.py,sha256=RgbSmvdmwNo0GDY7GG489WXIh-v3WBKqsQmPimNTcIM,527
 sagemaker_jupyterlab_extension_common/util/__init__.py,sha256=1I6YYNelr5hBJrNcxtFOJEHc-OzD95tsvUTFD1iUAx0,66
 sagemaker_jupyterlab_extension_common/util/app_metadata.py,sha256=HzMKwYytytFiOKc_1OE90BU2xkQPNWOo4t6L0-_ei9Q,1679
 sagemaker_jupyterlab_extension_common/util/file_watcher.py,sha256=FDpI-E78vuNw9GukH3y4V32x559WgFqXlEV1soOi178,2327
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/THIRD-PARTY-LICENSES,sha256=Xf_WPb1hL9MPcZb08ULM_aFKGpNjMQwt0_VzUFGKd5E,14623
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json,sha256=do8kNpot610HiXHT2F3GjIZSqKId0ZsrzgALuVQHli0,123
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/install.json,sha256=SYyYWifHnqcJRmquYcPhU-gfdr32gIWHQ8v5wKLCito,240
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/package.json,sha256=Z6Iig0n_bEIfviiUWEh8u6IKVhfsYdJ3s_UztoGJ-94,2452
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/117.e01e1fff3ce2e26893fe.js,sha256=4B4f_zzi4miT_jcBqmiRlEFy63ipNz2x19KOlNAuPIE,5073
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/38.15ae4750d35a3729c290.js,sha256=Fa5HUNNaNynCkF3SZ7iwkT8Ya71A4MAX4J8v_0gm3EQ,1949
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/512.769ffeae9d7cc23f13a4.js,sha256=dp_-rp18wj8TpKy6tt7xgpVy-ibXJxnb3OptkDdzHJA,1949
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/687.d1a4669887f7c4f5716c.js,sha256=0aRmmIf3xPVxbDtH-8EaOJEyOGx4GQX2Y99zH-qfaRA,8229
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/936.c7888f92b7d8a8d28b6a.js,sha256=x4iPkrfYqNKLanFPpLowLrNAz5NOfORlbj9p0TtYTSs,3758
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/remoteEntry.c75f0e99e1799c6fa7c3.js,sha256=x18OmeF5nG-nw4eFq9U_pPeAdnHv9Qd85_qunbvZh44,7751
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/style.js,sha256=-CQt0ZTPaCTvrRiLcznxflAbfvIKlOVzjOos-muaXQ8,118
-sagemaker_jupyterlab_extension_common-0.1.8.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/third-party-licenses.json,sha256=i8yhqwusdJETkbUBnGQKWEr2kpNwQJlDI0nCvZ8ng9o,6761
-sagemaker_jupyterlab_extension_common-0.1.8.dist-info/LICENSE,sha256=ZWQ-fVLy0k5hdDLaputxwZyEfnfpvEx3ZImaRiZyuTA,4755
-sagemaker_jupyterlab_extension_common-0.1.8.dist-info/METADATA,sha256=_igwps7NNaFvrqBIB_WA4GIFNrSCEcBPX_xPLsbL2uk,2191
-sagemaker_jupyterlab_extension_common-0.1.8.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-sagemaker_jupyterlab_extension_common-0.1.8.dist-info/top_level.txt,sha256=CShh661ZekKnAVxZHhdch0xRYNgkvgSIwFdhWQxQX28,38
-sagemaker_jupyterlab_extension_common-0.1.8.dist-info/RECORD,,
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/THIRD-PARTY-LICENSES,sha256=Xf_WPb1hL9MPcZb08ULM_aFKGpNjMQwt0_VzUFGKd5E,14623
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json,sha256=do8kNpot610HiXHT2F3GjIZSqKId0ZsrzgALuVQHli0,123
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/install.json,sha256=SYyYWifHnqcJRmquYcPhU-gfdr32gIWHQ8v5wKLCito,240
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/package.json,sha256=2O8XW2zrgS36p6u51DLiU_VKsxzI-cngL3ThFAH7ehU,2452
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/117.e01e1fff3ce2e26893fe.js,sha256=4B4f_zzi4miT_jcBqmiRlEFy63ipNz2x19KOlNAuPIE,5073
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/38.15ae4750d35a3729c290.js,sha256=Fa5HUNNaNynCkF3SZ7iwkT8Ya71A4MAX4J8v_0gm3EQ,1949
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/512.769ffeae9d7cc23f13a4.js,sha256=dp_-rp18wj8TpKy6tt7xgpVy-ibXJxnb3OptkDdzHJA,1949
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/687.d1a4669887f7c4f5716c.js,sha256=0aRmmIf3xPVxbDtH-8EaOJEyOGx4GQX2Y99zH-qfaRA,8229
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/936.e849b05e674b2ed3d783.js,sha256=6EmwXmdLLtPXg5z105Go_OtPRmm_MRe8j6X6Cjl8bNE,3758
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/remoteEntry.b855f9574044219a399a.js,sha256=uFX5V0BEIZo5mm5mzdDACHIgqNM5qWOXWYOf2uRs6E0,7751
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/style.js,sha256=-CQt0ZTPaCTvrRiLcznxflAbfvIKlOVzjOos-muaXQ8,118
+sagemaker_jupyterlab_extension_common-0.1.9.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extension-common/static/third-party-licenses.json,sha256=i8yhqwusdJETkbUBnGQKWEr2kpNwQJlDI0nCvZ8ng9o,6761
+sagemaker_jupyterlab_extension_common-0.1.9.dist-info/LICENSE,sha256=ZWQ-fVLy0k5hdDLaputxwZyEfnfpvEx3ZImaRiZyuTA,4755
+sagemaker_jupyterlab_extension_common-0.1.9.dist-info/METADATA,sha256=_mNkO6UPk_j5SRKYuj8oa77I3GVzLP7SUd9BxjZE_NI,2191
+sagemaker_jupyterlab_extension_common-0.1.9.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+sagemaker_jupyterlab_extension_common-0.1.9.dist-info/top_level.txt,sha256=CShh661ZekKnAVxZHhdch0xRYNgkvgSIwFdhWQxQX28,38
+sagemaker_jupyterlab_extension_common-0.1.9.dist-info/RECORD,,
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/__init__.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/_version.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/_version.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/service-2.json` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/service-2.json`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/clients.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/clients.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/constants.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/constants.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/handlers.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     """Handle event log requests emitted by Studio JupyterLab UI"""
 
     eventlog_instance = None
 
     def get_eventlog(self):
         if not JupterLabUILogHandler.eventlog_instance:
             """ "Create a StudioEventLog with the correct schemas"""
-            schema_documents = [SchemaDocument.JupyterLabOperation]
+            schema_documents = [
+                SchemaDocument.JupyterLabOperation,
+                SchemaDocument.JupyterLabPerformanceMetrics,
+            ]
             JupterLabUILogHandler.eventlog_instance = create_ui_eventlogger(
                 schema_documents
             )
         return JupterLabUILogHandler.eventlog_instance
 
     def inject_log_context(self, event_record):
         if event_record and "Context" in event_record:
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/package.json` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.962797619047619%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b855f9574044219a399a.js'}}",*

 * * "'version'": "'0.1.9'"}*

```diff
@@ -42,15 +42,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c75f0e99e1799c6fa7c3.js"
+            "load": "static/remoteEntry.b855f9574044219a399a.js"
         },
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension_common/labextension"
     },
     "license": "Amazon Software License",
     "licenses": [
         {
@@ -69,9 +69,9 @@
         "lint:fix": "eslint --fix . --ext .js,.ts,.tsx",
         "release": "run-s build",
         "test": "jest",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/117.e01e1fff3ce2e26893fe.js` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/117.e01e1fff3ce2e26893fe.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/38.15ae4750d35a3729c290.js` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/38.15ae4750d35a3729c290.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/512.769ffeae9d7cc23f13a4.js` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/512.769ffeae9d7cc23f13a4.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/687.d1a4669887f7c4f5716c.js` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/687.d1a4669887f7c4f5716c.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/936.c7888f92b7d8a8d28b6a.js` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/936.e849b05e674b2ed3d783.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -103,15 +103,15 @@
                     return this.eventLog.recordEvent({
                         version: this.schema.schemaVersion,
                         schema: this.schema.schemaId,
                         body: this.format(e, t)
                     })
                 }
             }
-            var f = r(768);
+            var f = r(495);
             const y = [d, {
                 id: s,
                 autoStart: !0,
                 provides: u,
                 activate: e => {
                     const t = {
                             SessionId: (e => {
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.c75f0e99e1799c6fa7c3.js` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.b855f9574044219a399a.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, d, c, p, h, m, b, v, g, y = {
-            222: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, f, s, d, c, p, h, m, b, v, g, y = {
+            801: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(713), t.e(936)]).then((() => () => t(936))),
                         "./extension": () => Promise.all([t.e(713), t.e(936)]).then((() => () => t(936)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         w = {};
 
     function j(e) {
         var r = w[e];
@@ -47,47 +47,47 @@
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         38: "15ae4750d35a3729c290",
         117: "e01e1fff3ce2e26893fe",
         512: "769ffeae9d7cc23f13a4",
         687: "d1a4669887f7c4f5716c",
         713: "6ec4e1111ab220edbbdf",
         901: "8f38b8390513a01e8ffb",
-        936: "c7888f92b7d8a8d28b6a"
+        936: "e849b05e674b2ed3d783"
     } [e] + ".js?v=" + {
         38: "15ae4750d35a3729c290",
         117: "e01e1fff3ce2e26893fe",
         512: "769ffeae9d7cc23f13a4",
         687: "d1a4669887f7c4f5716c",
         713: "6ec4e1111ab220edbbdf",
         901: "8f38b8390513a01e8ffb",
-        936: "c7888f92b7d8a8d28b6a"
+        936: "e849b05e674b2ed3d783"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amzn/sagemaker-jupyterlab-extension-common:", j.l = (t, n, a, o) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amzn/sagemaker-jupyterlab-extension-common:", j.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
-                        i = f;
+            if (void 0 !== o)
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
@@ -99,31 +99,31 @@
         })
     }, (() => {
         j.S = {};
         var e = {},
             r = {};
         j.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 j.o(j.S, t) || (j.S[t] = {});
-                var o = j.S[t],
+                var a = j.S[t],
                     i = "@amzn/sagemaker-jupyterlab-extension-common",
                     u = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            u = a[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
+                        var o = a[e] = a[e] || {},
+                            u = o[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("@amzn/sagemaker-jupyterlab-extension-common", "0.1.8", (() => Promise.all([j.e(713), j.e(936)]).then((() => () => j(936))))), u("@jupyterlab/jupyterlab-telemetry", "1.0.3", (() => Promise.all([j.e(713), j.e(901), j.e(512)]).then((() => () => j(512))))), u("p-retry", "6.1.0", (() => j.e(117).then((() => () => j(117))))), u("uuid", "9.0.1", (() => j.e(687).then((() => () => j(687)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@amzn/sagemaker-jupyterlab-extension-common", "0.1.9", (() => Promise.all([j.e(713), j.e(936)]).then((() => () => j(936))))), u("@jupyterlab/jupyterlab-telemetry", "1.0.3", (() => Promise.all([j.e(713), j.e(901), j.e(512)]).then((() => () => j(512))))), u("p-retry", "6.1.0", (() => j.e(117).then((() => () => j(117))))), u("uuid", "9.0.1", (() => j.e(687).then((() => () => j(687)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -138,161 +138,161 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 u = (typeof i)[0];
-            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
-                if ("u" == f) {
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
                     if (!l || "u" != d) return !1
                 } else if (l)
-                    if (d == f)
+                    if (d == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (a ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
-                    if (a || u <= n) return !1;
+                    if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != a) return !1;
+                    if (u <= n || s < d != o) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
-        var a = u(e, t);
-        return o(n, a) || d(l(e, t, a, n)), c(e[t][a])
-    }, f = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+        var o = u(e, t);
+        return a(n, o) || d(l(e, t, o, n)), c(e[t][o])
+    }, s = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, a) {
-        var o = j.I(r);
-        return o && o.then ? o.then(e.bind(e, r, j.S[r], t, n, a)) : e(r, j.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), m = p(((e, r, t, n, a) => {
-        var o = r && j.o(r, t) && f(r, t, n);
-        return o ? c(o) : a()
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+        var a = j.I(r);
+        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = p(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && s(r, t, n);
+        return a ? c(a) : o()
     })), b = {}, v = {
         858: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 8]),
         976: () => h("default", "@jupyterlab/services", [1, 7, 0, 8]),
         13: () => m("default", "uuid", [1, 9, 0, 1], (() => j.e(687).then((() => () => j(687))))),
         321: () => m("default", "p-retry", [1, 6, 1, 0], (() => j.e(117).then((() => () => j(117))))),
-        768: () => m("default", "@jupyterlab/jupyterlab-telemetry", [1, 1, 0, 3], (() => Promise.all([j.e(901), j.e(38)]).then((() => () => j(512))))),
+        495: () => m("default", "@jupyterlab/jupyterlab-telemetry", [1, 1, 0, 3], (() => Promise.all([j.e(901), j.e(38)]).then((() => () => j(512))))),
         930: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         901: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
     }, g = {
         713: [858, 976],
         901: [901],
-        936: [13, 321, 768, 930]
+        936: [13, 321, 495, 930]
     }, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete b[e], j.m[e] = t => {
                         throw delete j.c[e], r
                     }
                 };
             try {
-                var a = v[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var o = v[e]();
+                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             61: 0
         };
         j.f.j = (r, t) => {
             var n = j.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (/^(713|901)$/.test(r)) e[r] = 0;
             else {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
-                var o = j.p + j.u(r),
+                var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                t.push(n[2] = o);
+                var a = j.p + j.u(r),
                     i = new Error;
-                j.l(o, (t => {
+                j.l(a, (t => {
                     if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                        var o = t && ("load" === t.type ? "missing" : t.type),
+                            a = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var n, a, [o, i, u] = t,
+                var n, o, [a, i, u] = t,
                     l = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) j.o(i, n) && (j.m[n] = i[n]);
                     u && u(j)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], j.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extension_common = self.webpackChunk_amzn_sagemaker_jupyterlab_extension_common || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var k = j(222);
+    var k = j(801);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extension-common"] = k
 })();
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/labextension/static/third-party-licenses.json` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/logging_utils.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/logging_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import os.path
 from enum import Enum
 from pathlib import Path
 
 from traitlets import log
 from jupyter_events.logger import EventLogger
+from jupyter_events.schema_registry import SchemaRegistryException
 from aws_embedded_metrics.logger.metrics_context import MetricsContext
 from aws_embedded_metrics.serializers.log_serializer import LogSerializer
 
 from sagemaker_jupyterlab_extension_common.util.app_metadata import (
     get_domain_id,
     get_aws_account_id,
     get_space_name,
@@ -277,19 +278,22 @@
             self, self.jl_extension_name, self.jl_extension_version
         )
 
 
 def create_ui_eventlogger(schema_documents):
     eventlog = _default_eventlog
     for schema_document in schema_documents:
-        handler = get_handler(schema_document)
-        # Add filter for handler
-        handler.addFilter(schema_document.get_log_event_filter())
-        eventlog.register_handler(handler)
-        eventlog.register_event_schema(schema_document.get_schema_file_path())
+        try:
+            handler = get_handler(schema_document)
+            # Add filter for handler
+            handler.addFilter(schema_document.get_log_event_filter())
+            eventlog.register_handler(handler)
+            eventlog.register_event_schema(schema_document.get_schema_file_path())
+        except SchemaRegistryException:
+            pass
     return eventlog
 
 
 class SchemaDocumentLogFilter:
     def __init__(self, schema_document):
         self.schema_document = schema_document
         self.schema_filter = list(
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/handler_metrics_schema.yml` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/handler_metrics_schema.yml`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_client_performance_metrics_schema.yml` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_client_performance_metrics_schema.yml`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_operation_log_schema.yml` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_operation_log_schema.yml`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/log_schema.yml` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/log_schema.yml`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/logging/schemas/request_metrics_schema.yml` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/logging/schemas/request_metrics_schema.yml`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/test_app_metadata.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/test_app_metadata.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/test_clients.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/test_handlers.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/test_logging_utils.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/tests/utils.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/util/app_metadata.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/util/app_metadata.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common/util/file_watcher.py` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common/util/file_watcher.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/PKG-INFO` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension-common
-Version: 0.1.8
+Version: 0.1.9
 Summary: SageMaker JupyterLab workspace common module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/sagemaker_jupyterlab_extension_common.egg-info/SOURCES.txt` & `sagemaker-jupyterlab-extension-common-0.1.9/sagemaker_jupyterlab_extension_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 THIRD-PARTY-LICENSES
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
 jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension_common.json
-public_dist/sagemaker_jupyterlab_extension_common-0.1.8-py3-none-any.whl
+public_dist/sagemaker_jupyterlab_extension_common-0.1.9-py3-none-any.whl
 sagemaker_jupyterlab_extension_common/__init__.py
 sagemaker_jupyterlab_extension_common/_version.py
 sagemaker_jupyterlab_extension_common/clients.py
 sagemaker_jupyterlab_extension_common/constants.py
 sagemaker_jupyterlab_extension_common/handlers.py
 sagemaker_jupyterlab_extension_common/py.typed
 sagemaker_jupyterlab_extension_common.egg-info/PKG-INFO
@@ -23,16 +23,16 @@
 sagemaker_jupyterlab_extension_common.egg-info/top_level.txt
 sagemaker_jupyterlab_extension_common/botocore_model/sagemaker/2017-07-24/service-2.json
 sagemaker_jupyterlab_extension_common/labextension/package.json
 sagemaker_jupyterlab_extension_common/labextension/static/117.e01e1fff3ce2e26893fe.js
 sagemaker_jupyterlab_extension_common/labextension/static/38.15ae4750d35a3729c290.js
 sagemaker_jupyterlab_extension_common/labextension/static/512.769ffeae9d7cc23f13a4.js
 sagemaker_jupyterlab_extension_common/labextension/static/687.d1a4669887f7c4f5716c.js
-sagemaker_jupyterlab_extension_common/labextension/static/936.c7888f92b7d8a8d28b6a.js
-sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.c75f0e99e1799c6fa7c3.js
+sagemaker_jupyterlab_extension_common/labextension/static/936.e849b05e674b2ed3d783.js
+sagemaker_jupyterlab_extension_common/labextension/static/remoteEntry.b855f9574044219a399a.js
 sagemaker_jupyterlab_extension_common/labextension/static/style.js
 sagemaker_jupyterlab_extension_common/labextension/static/third-party-licenses.json
 sagemaker_jupyterlab_extension_common/logging/__init__.py
 sagemaker_jupyterlab_extension_common/logging/logging_utils.py
 sagemaker_jupyterlab_extension_common/logging/schemas/handler_metrics_schema.yml
 sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_client_performance_metrics_schema.yml
 sagemaker_jupyterlab_extension_common/logging/schemas/jupyterlab_operation_log_schema.yml
```

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/setup.py` & `sagemaker-jupyterlab-extension-common-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/constants/logger.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/constants/logger.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/LoggerPlugin.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/LoggerPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/__tests__/LoggerPlugin.spec.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/__tests__/LoggerPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/__tests__/logger.spec.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/__tests__/logger.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/handlers.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/handlers.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/LoggerPlugin/logger.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/LoggerPlugin/logger.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/PanoramaPlugin.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/PanoramaPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/__tests__/utils.spec.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/__tests__/utils.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/plugins/PanoramaPlugin/utils.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/plugins/PanoramaPlugin/utils.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/services/fetchapi.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/services/fetchapi.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/src/types/logger.ts` & `sagemaker-jupyterlab-extension-common-0.1.9/src/types/logger.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-common-0.1.8/tsconfig.json` & `sagemaker-jupyterlab-extension-common-0.1.9/tsconfig.json`

 * *Files identical despite different names*

