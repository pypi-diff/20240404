# Comparing `tmp/sagemaker-jupyterlab-extension-0.3.0.tar.gz` & `tmp/sagemaker-jupyterlab-extension-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-jupyterlab-extension-0.3.0.tar", last modified: Tue Apr  2 23:22:26 2024, max compression
+gzip compressed data, was "sagemaker-jupyterlab-extension-0.3.1.tar", last modified: Thu Apr  4 00:01:35 2024, max compression
```

## Comparing `sagemaker-jupyterlab-extension-0.3.0.tar` & `sagemaker-jupyterlab-extension-0.3.1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.279719 sagemaker-jupyterlab-extension-0.3.0/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4755 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/LICENSE
--rw-r--r--   0 p4admin  (12569) amazon     (100)      612 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/MANIFEST.in
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-02 23:22:26.275719 sagemaker-jupyterlab-extension-0.3.0/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1322 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/README.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8139 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/THIRD-PARTY-LICENSES
--rw-r--r--   0 p4admin  (12569) amazon     (100)      221 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/install.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.223719 sagemaker-jupyterlab-extension-0.3.0/jupyter-config/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.231719 sagemaker-jupyterlab-extension-0.3.0/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      105 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3949 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.231719 sagemaker-jupyterlab-extension-0.3.0/public_dist/
--rw-r--r--   0 p4admin  (12569) amazon     (100)  2341780 2024-04-02 23:20:25.000000 sagemaker-jupyterlab-extension-0.3.0/public_dist/sagemaker_jupyterlab_extension-0.3.0-py3-none-any.whl
--rw-r--r--   0 p4admin  (12569) amazon     (100)      156 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/pyproject.toml
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.235719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1133 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      683 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/_version.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    11587 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/handlers.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.235719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4091 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.251719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3280 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    92715 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1874 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)  4112866 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8620 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2309 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    28094 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   205663 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    36761 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      249 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4283 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12933 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   292756 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)       50 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)   103503 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      487 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4474 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   237708 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   266482 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    58332 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7725 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   139405 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12105 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      185 2024-04-02 23:21:34.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    91011 2024-04-02 23:22:14.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.251719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       60 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/helper.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1647 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5332 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5041 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7701 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_request_logger.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.255719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       64 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      555 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2552 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/git_clone_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      507 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/metric_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7250 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/request_logger.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.275719 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5749 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-02 23:19:17.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/not-zip-safe
--rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/requires.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       31 2024-04-02 23:22:26.000000 sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/top_level.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2024-04-02 23:22:26.279719 sagemaker-jupyterlab-extension-0.3.0/setup.cfg
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2953 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/setup.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.255719 sagemaker-jupyterlab-extension-0.3.0/src/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.255719 sagemaker-jupyterlab-extension-0.3.0/src/__mocks__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/__mocks__/fileMock.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.255719 sagemaker-jupyterlab-extension-0.3.0/src/components/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3246 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/GitCloneComponent.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6489 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/ResourceUsageComponent.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      970 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/SpaceMenu.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.259719 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1797 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/AutoComplete.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      799 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/CheckboxComponent.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1917 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/GitCloneComponent.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      881 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/InputField.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1068 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/LinearProgressWithLabel.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3156 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/ResourceUsageComponent.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2343 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/SpaceMenu.spec.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.259719 sagemaker-jupyterlab-extension-0.3.0/src/components/common/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1394 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/common/AutoComplete.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      988 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/common/CheckboxComponent.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/common/InputField.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      980 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/common/LinearProgressWithLabel.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.259719 sagemaker-jupyterlab-extension-0.3.0/src/components/styles/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      575 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/styles/InputFieldStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      469 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/styles/SpaceMenuStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      475 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/components/styles/autoCompleteStyles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.263719 sagemaker-jupyterlab-extension-0.3.0/src/constants/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1201 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/errorMessages.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      191 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/gitCloneConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3228 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/il18Strings.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      174 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      632 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/resourceUsageConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1480 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/sessionManagementConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/constants/spaceMenuConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      425 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.263719 sagemaker-jupyterlab-extension-0.3.0/src/plugins/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6451 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/GitClonePlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      767 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/HideShutDownPlugin.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.267719 sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      785 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       45 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4320 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/utils.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      814 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/ResourceUsagePlugin.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6247 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/SessionManagementPlugin.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1167 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/SpaceMenuPlugin.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.267719 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3662 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/GitClonePlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      787 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/HideShutDownPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      741 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/ResourceUsagePlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4826 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/SessionManagementPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1365 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/SpaceMenuPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      226 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/plugins/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.267719 sagemaker-jupyterlab-extension-0.3.0/src/service/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.267719 sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2425 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/index.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1193 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/mock.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      526 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/service/constants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/service/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.271719 sagemaker-jupyterlab-extension-0.3.0/src/style/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/style/common.css
--rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/style/index.css
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.271719 sagemaker-jupyterlab-extension-0.3.0/src/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      531 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/ReactWidgetWrapper.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.271719 sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8036 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/gitCloneUtils.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    16809 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/sessionManagerUtils.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5331 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/gitCloneUtils.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      547 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/logger.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    10835 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/utils/sessionManagerUtils.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.271719 sagemaker-jupyterlab-extension-0.3.0/src/widgets/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1971 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/GitCloneWidget.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2161 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/ResourceUsageWidget.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      809 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/SpaceMenuWidget.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.275719 sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1597 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/GitCloneWidget.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1638 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/ResourceUsageWidget.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/SpaceMenuWidget.spec.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-02 23:22:26.275719 sagemaker-jupyterlab-extension-0.3.0/src/widgets/styles/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/styles/gitCloneStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2092 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/src/widgets/styles/resourceUsageStyle.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9490 2024-04-02 23:09:48.000000 sagemaker-jupyterlab-extension-0.3.0/tsconfig.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4755 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/LICENSE
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      612 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/MANIFEST.in
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1322 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/README.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8139 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/THIRD-PARTY-LICENSES
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      221 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/install.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.652631 sagemaker-jupyterlab-extension-0.3.1/jupyter-config/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.656631 sagemaker-jupyterlab-extension-0.3.1/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      105 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3949 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.656631 sagemaker-jupyterlab-extension-0.3.1/public_dist/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  2341809 2024-04-03 23:59:53.000000 sagemaker-jupyterlab-extension-0.3.1/public_dist/sagemaker_jupyterlab_extension-0.3.1-py3-none-any.whl
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      156 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/pyproject.toml
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.660631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1133 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      683 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/_version.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    11587 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/handlers.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.660631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4091 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3280 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    92715 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1874 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  4112866 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8620 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2309 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    28123 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   205663 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    36761 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      249 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4283 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12933 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   292756 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       50 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   103503 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      487 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4474 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   237708 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   266482 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    58332 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7725 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   139405 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12105 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      185 2024-04-04 00:00:40.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    91011 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       60 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/helper.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1647 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5332 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5041 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7701 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_request_logger.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       64 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      555 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2552 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/git_clone_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      507 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/metric_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7250 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/request_logger.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5749 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-03 23:58:45.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/not-zip-safe
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/requires.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       31 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/top_level.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/setup.cfg
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2953 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/setup.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/src/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/src/__mocks__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/__mocks__/fileMock.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/src/components/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3246 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/GitCloneComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6489 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/ResourceUsageComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1019 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/SpaceMenu.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.676631 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1797 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/AutoComplete.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      799 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/CheckboxComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1917 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/GitCloneComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      881 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/InputField.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1068 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/LinearProgressWithLabel.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3156 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/ResourceUsageComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2389 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/SpaceMenu.spec.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.676631 sagemaker-jupyterlab-extension-0.3.1/src/components/common/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1394 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/common/AutoComplete.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      988 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/common/CheckboxComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/common/InputField.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      980 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/common/LinearProgressWithLabel.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.676631 sagemaker-jupyterlab-extension-0.3.1/src/components/styles/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      575 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/styles/InputFieldStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      469 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/styles/SpaceMenuStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      475 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/styles/autoCompleteStyles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.676631 sagemaker-jupyterlab-extension-0.3.1/src/constants/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1201 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/errorMessages.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      191 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/gitCloneConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3263 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/il18Strings.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      174 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      632 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/resourceUsageConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1480 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/sessionManagementConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/spaceMenuConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      425 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/plugins/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6451 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/GitClonePlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      767 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/HideShutDownPlugin.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      785 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       45 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4320 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/utils.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      814 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/ResourceUsagePlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6247 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/SessionManagementPlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1167 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/SpaceMenuPlugin.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3662 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/GitClonePlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      787 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/HideShutDownPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      741 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/ResourceUsagePlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4826 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/SessionManagementPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1365 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/SpaceMenuPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      226 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/service/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2425 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/index.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1193 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/mock.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      526 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/service/constants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/service/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/style/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/style/common.css
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/style/index.css
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      531 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/ReactWidgetWrapper.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8036 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/gitCloneUtils.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    16809 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/sessionManagerUtils.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5331 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/gitCloneUtils.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      547 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/logger.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    10835 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/sessionManagerUtils.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/src/widgets/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1971 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/GitCloneWidget.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2161 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/ResourceUsageWidget.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      809 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/SpaceMenuWidget.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1597 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/GitCloneWidget.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1638 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/ResourceUsageWidget.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/SpaceMenuWidget.spec.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/src/widgets/styles/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/styles/gitCloneStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2092 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/styles/resourceUsageStyle.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9490 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/tsconfig.json
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/LICENSE` & `sagemaker-jupyterlab-extension-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/MANIFEST.in` & `sagemaker-jupyterlab-extension-0.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/PKG-INFO` & `sagemaker-jupyterlab-extension-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.3.0
+Version: 0.3.1
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/README.md` & `sagemaker-jupyterlab-extension-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/THIRD-PARTY-LICENSES` & `sagemaker-jupyterlab-extension-0.3.1/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/package.json` & `sagemaker-jupyterlab-extension-0.3.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -100,9 +100,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/public_dist/sagemaker_jupyterlab_extension-0.3.0-py3-none-any.whl` & `sagemaker-jupyterlab-extension-0.3.1/public_dist/sagemaker_jupyterlab_extension-0.3.1-py3-none-any.whl`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,78 +1,78 @@
-Zip file size: 2341780 bytes, number of entries: 76
+Zip file size: 2341809 bytes, number of entries: 76
 -rw-r--r--  2.0 unx     1133 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/__init__.py
 -rw-r--r--  2.0 unx      683 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/_version.py
 -rw-r--r--  2.0 unx    11587 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/handlers.py
 -rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/package.json
 -rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
--rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js
+-rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
 -rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
 -rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
 -rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 -rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
--rw-r--r--  2.0 unx    28094 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js
+-rw-r--r--  2.0 unx    28123 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js
 -rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 -rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 -rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
 -rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
 -rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
 -rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
 -rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 -rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
 -rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 -rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
--rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js
--rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js
+-rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
+-rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js
 -rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 -rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
 -rw-r--r--  2.0 unx   139405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
 -rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
--rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js
+-rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js
 -rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/style.js
 -rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 -rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/__init__.py
 -rw-r--r--  2.0 unx      405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/helper.py
 -rw-r--r--  2.0 unx     1647 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_error_util.py
 -rw-r--r--  2.0 unx     5332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
 -rw-r--r--  2.0 unx     5041 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_handlers.py
 -rw-r--r--  2.0 unx     7701 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_request_logger.py
 -rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/__init__.py
 -rw-r--r--  2.0 unx      555 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/error_util.py
 -rw-r--r--  2.0 unx     2552 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/git_clone_util.py
 -rw-r--r--  2.0 unx      507 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/metric_util.py
 -rw-r--r--  2.0 unx     7250 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/request_logger.py
--rw-r--r--  2.0 unx     8139 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/THIRD-PARTY-LICENSES
--rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
--rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
--rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
--rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
--rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.2135a6297693b09662d9.js
--rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
--rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
--rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
--rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
--rw-r--r--  2.0 unx    28094 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.5350b743f9a235d9e265.js
--rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
--rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
--rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
--rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
--rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
--rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
--rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
--rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
--rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
--rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.c508feab9dfdf7494214.js
--rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.7f061638d47075ac76be.js
--rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
--rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
--rw-r--r--  2.0 unx   139405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js
--rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt
--rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.27a0e3dfb32431afe940.js
--rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
--rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
--rw-r--r--  2.0 unx     4755 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2281 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       31 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    11677 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.0.dist-info/RECORD
-76 files, 11528004 bytes uncompressed, 2321222 bytes compressed:  79.9%
+-rw-r--r--  2.0 unx     8139 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/THIRD-PARTY-LICENSES
+-rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+-rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
+-rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
+-rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
+-rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js
+-rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
+-rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
+-rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
+-rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
+-rw-r--r--  2.0 unx    28123 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.a6ac1d0d39311897c48d.js
+-rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
+-rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
+-rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
+-rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
+-rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
+-rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
+-rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+-rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
+-rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+-rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
+-rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js
+-rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.26c15aab8d5d7301c11a.js
+-rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
+-rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
+-rw-r--r--  2.0 unx   139405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js
+-rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt
+-rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.7282f69f1fc0d8e37b1c.js
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
+-rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
+-rw-r--r--  2.0 unx     4755 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2281 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       31 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11677 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/RECORD
+76 files, 11528062 bytes uncompressed, 2321251 bytes compressed:  79.9%
```

#### zipnote «TEMP»/diffoscope_7e6msv9b_/tmpmrkzn9op_.zip

```diff
@@ -9,30 +9,30 @@
 
 Filename: sagemaker_jupyterlab_extension/labextension/package.json
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 Comment: 
@@ -57,33 +57,33 @@
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/style.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 Comment: 
@@ -117,113 +117,113 @@
 
 Filename: sagemaker_jupyterlab_extension/utils/metric_util.py
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/utils/request_logger.py
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/THIRD-PARTY-LICENSES
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/THIRD-PARTY-LICENSES
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.2135a6297693b09662d9.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.5350b743f9a235d9e265.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.a6ac1d0d39311897c48d.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.c508feab9dfdf7494214.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.7f061638d47075ac76be.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.26c15aab8d5d7301c11a.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.27a0e3dfb32431afe940.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.7282f69f1fc0d8e37b1c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
+Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/LICENSE
+Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/METADATA
+Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/WHEEL
+Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/top_level.txt
+Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.0.dist-info/RECORD
+Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### sagemaker_jupyterlab_extension/labextension/package.json

##### Pretty-printed

 * *Similarity: 0.9661111111111111%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7282f69f1fc0d8e37b1c.js'}}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -60,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.27a0e3dfb32431afe940.js",
+            "load": "static/remoteEntry.7282f69f1fc0d8e37b1c.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -105,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

#### sagemaker_jupyterlab_extension/tests/test_request_logger.py

```diff
@@ -211,15 +211,15 @@
     assert (
         data["UriPath"] == "/jupyterlab/default/aws/sagemaker/api/git/list-repositories"
     )
     assert data["ResponseLatencyMS"] == 0.1
     assert (
         data["Context"]["ExtensionName"] == "SagemakerStudioJuypterLabExtensionCommon"
     )
-    assert data["Context"]["ExtensionVersion"] == "0.3.0"
+    assert data["Context"]["ExtensionVersion"] == "0.3.1"
     assert data["Context"]["AccountId"] == "1234567890"
     assert data["Context"]["DomainId"] == "d-jk12345678"
     assert data["Context"]["SpaceName"] == "default-space"
     data["_aws"]["Timestamp"] = 123456
 
     assert data["_aws"] == {
         "CloudWatchMetrics": [
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js` & `sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -2749,15 +2749,15 @@
                 l = o(4780),
                 s = o(917),
                 d = o(1796),
                 c = o(8216),
                 p = o(2734),
                 u = o(948),
                 m = o(1657),
-                f = o(7651),
+                f = o(8962),
                 h = o(5893);
             const b = ["className", "color", "value", "valueBuffer", "variant"];
             let v, g, Z, x, y, S, C = e => e;
             const P = (0, s.F4)(v || (v = C`
   0% {
     left: -35%;
     right: 100%;
@@ -3002,15 +3002,15 @@
                             className: x.bar2,
                             ownerState: Z,
                             style: C.bar2
                         })]
                     }))
                 }))
         },
-        7651: (e, t, o) => {
+        8962: (e, t, o) => {
             o.d(t, {
                 E: () => a,
                 Z: () => i
             });
             var r = o(1588),
                 n = o(4867);
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js` & `sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js`

 * *Files 4% similar despite different names*

##### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [548], {
-        4548: (e, t, a) => {
-            a.r(t), a.d(t, {
+        4548: (e, t, n) => {
+            n.r(t), n.d(t, {
                 default: () => Xe
             });
-            var n = a(9557);
+            var a = n(9557);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
                 i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
                 o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
                 r = {
                     shutdown: "filemenu:shutdown"
                 },
                 l = "Sso",
@@ -75,34 +75,35 @@
                             failedOptionsBody: "Something went wrong when trying to open README file within the repo.",
                             invalidCloneUrlTitle: "Invalid URL provided",
                             invalidCloneUrlBody: "The URL provided is not valid. Please input a valid URL to clone."
                         }
                     },
                     Space: {
                         privateSpaceHeader: "Personal Studio",
-                        unknownUser: "Unknown User"
+                        unknownUser: "Unknown User",
+                        unknownSpace: "Unknown Space"
                     }
                 },
                 g = "GitCloneDialogError",
                 h = "ValidRepoPathError",
                 y = "spaceMenuHeader",
                 v = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:hideshutdown",
-                    requires: [n.IMainMenu],
+                    requires: [a.IMainMenu],
                     autoStart: !0,
                     activate: (e, t) => {
                         e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
-            var w = a(9801),
-                b = a.n(w),
-                E = a(6029),
-                f = a.n(E),
-                x = a(8368),
-                S = a(9510);
+            var w = n(9801),
+                b = n.n(w),
+                E = n(6029),
+                f = n.n(E),
+                x = n(8368),
+                S = n(9510);
             class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
@@ -117,162 +118,162 @@
                 R = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
                 T = () => {
                     const e = R("expiryTime"),
                         t = R("ssoExpiryTimestamp");
                     return M() && t ? Number(t[1]) : e ? Number(e[1]) : null
                 },
                 j = (e, t) => {
-                    var a, n;
-                    t ? null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.disconnect(x.ConnectionLost) : null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.connect(x.ConnectionLost)
+                    var n, a;
+                    t ? null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.disconnect(x.ConnectionLost) : null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.connect(x.ConnectionLost)
                 },
                 k = () => {
                     const e = R("redirectURL");
                     let t;
                     try {
                         if (t = new URL(e ? e[1] : void 0), "http:" === t.protocol || "https:" === t.protocol) return t.toString()
                     } catch (e) {
                         return
                     }
                 },
                 D = (e, t) => {
-                    const a = T(),
-                        n = window.open(e, "signin window", "width=800, height=600");
+                    const n = T(),
+                        a = window.open(e, "signin window", "width=800, height=600");
                     let s = !1;
                     const i = window.setInterval((() => {
-                        if (n && n.closed && !s) return void window.clearInterval(i);
+                        if (a && a.closed && !s) return void window.clearInterval(i);
                         const e = T();
-                        if (null !== e && null !== a && (e > a || isNaN(e))) {
-                            window.clearInterval(i), n && n.close(), s = !0;
+                        if (null !== e && null !== n && (e > n || isNaN(e))) {
+                            window.clearInterval(i), a && a.close(), s = !0;
                             for (const e of t) e.kernel.reconnect();
                             S.Dialog.tracker.forEach((e => e.reject()))
                         }
                     }), u)
                 },
                 _ = async () => {
                     const {
                         SignInSession: e
                     } = m, {
                         signinDialog: t
-                    } = e, a = k(), n = a ? [S.Dialog.okButton({
+                    } = e, n = k(), a = n ? [S.Dialog.okButton({
                         label: e.signInButton
                     })] : [S.Dialog.cancelButton({
                         label: e.closeButton
-                    })], s = a ? f().createElement("div", {
+                    })], s = n ? f().createElement("div", {
                         "data-testid": "session-signin-log-out"
                     }, t.loggedOutBody) : f().createElement("div", {
                         "data-testid": "session-signin-restart"
                     }, t.restartSessionBody), i = new S.Dialog({
                         title: t.title,
                         body: s,
-                        buttons: n,
+                        buttons: a,
                         hasClose: !1
                     });
                     return {
                         sigInDialogResult: await i.launch(),
                         confirmDialog: i
                     }
                 };
-            var N = a(6797),
-                B = a(6697),
-                I = a(1638),
-                z = a(7217),
-                A = a(5326);
-            const U = (e, t, a, n, s, i, o) => {
+            var N = n(6797),
+                B = n(6697),
+                I = n(1638),
+                z = n(7217),
+                A = n(5326);
+            const U = (e, t, n, a, s, i, o) => {
                     const r = T(),
                         l = o(),
                         d = l && l + c;
                     if (null === r) j(e, !1);
                     else {
                         const o = b().unix(r / 1e3).diff(b()()),
                             u = Date.now();
-                        ((e, t, a) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(a, e))(M(), r, o) ? (n(), (async (e, t, a) => {
+                        ((e, t, n) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(n, e))(M(), r, o) ? (a(), (async (e, t, n) => {
                             const {
-                                SignInSession: n
+                                SignInSession: a
                             } = m, s = k();
                             S.Dialog.tracker.forEach((e => e.reject())), j(e, !0);
                             const {
                                 sigInDialogResult: i,
                                 confirmDialog: o
                             } = await _();
                             if (i && i.button)
-                                if (a(), s) D(k(), t);
-                                else if (i && i.button.label === n.closeButton) {
+                                if (n(), s) D(k(), t);
+                                else if (i && i.button.label === a.closeButton) {
                                 const e = T(),
                                     t = e && e / 1e3,
-                                    a = t && b().unix(t).diff(b()());
-                                null !== a && a && a > c && (o.dispose(), setTimeout((async () => {
+                                    n = t && b().unix(t).diff(b()());
+                                null !== n && n && n > c && (o.dispose(), setTimeout((async () => {
                                     await _()
                                 }), c))
                             } else o.dispose(), D(k(), t)
-                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (n(), (async (e, t, a, n, s) => {
+                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (a(), (async (e, t, n, a, s) => {
                             const {
                                 SignInSession: i
                             } = m, {
                                 renewSessionDialog: o
                             } = m.SignInSession, {
                                 renewSessionDialogResult: r,
                                 confirmDialog: l
                             } = await (async () => {
                                 const {
                                     SignInSession: e
                                 } = m, {
                                     renewSessionDialog: t
-                                } = m.SignInSession, a = k(), n = T(), s = n && b().unix(n / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
+                                } = m.SignInSession, n = k(), a = T(), s = a && b().unix(a / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
                                     "data-testid": "session-renew-lose-unsaved-changes"
                                 }, o, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), f().createElement("div", null, r)) : f().createElement("div", {
                                     "data-testid": "session-renew-now"
                                 }, f().createElement("p", null, o), f().createElement("p", null, t.renewSessionNow)), c = [S.Dialog.okButton({
                                     label: t.remindText
-                                }), a && S.Dialog.okButton({
+                                }), n && S.Dialog.okButton({
                                     label: e.saveAndRenewButton
                                 })], d = new S.Dialog({
                                     title: t.title,
                                     body: l,
                                     buttons: c,
                                     hasClose: !1
                                 });
                                 return {
                                     renewSessionDialogResult: await d.launch(),
                                     confirmDialog: d
                                 }
                             })();
                             if (r && r.button.label === o.remindText) {
                                 const e = new C;
-                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), n()
-                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), a(), n(), M() || D(k(), t))
-                        })(0, t._sessions, a, s, i), j(e, !1)) : j(e, !1)
+                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), a()
+                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), n(), a(), M() || D(k(), t))
+                        })(0, t._sessions, n, s, i), j(e, !1)) : j(e, !1)
                     }
                 },
                 L = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:sessionmanagement",
                     requires: [],
                     autoStart: !0,
                     activate: async e => {
                         let t;
-                        const a = e.serviceManager.sessions,
-                            n = () => {
+                        const n = e.serviceManager.sessions,
+                            a = () => {
                                 s.start()
                             },
-                            s = ((e, t, a, n, s, i, o) => new N.Poll({
+                            s = ((e, t, n, a, s, i, o) => new N.Poll({
                                 auto: !0,
-                                factory: async () => U(e, t, a, n, s, i, o),
+                                factory: async () => U(e, t, n, a, s, i, o),
                                 frequency: {
                                     interval: d,
                                     backoff: !0,
                                     max: p
                                 }
-                            }))(e, a, (() => {
+                            }))(e, n, (() => {
                                 const t = new I.TextModelFactory,
-                                    a = new I.DocumentRegistry({
+                                    n = new I.DocumentRegistry({
                                         textModelFactory: t
                                     }),
-                                    n = new z.ServiceManager({}),
+                                    a = new z.ServiceManager({}),
                                     s = new A.DocumentManager({
-                                        registry: a,
-                                        manager: n,
+                                        registry: n,
+                                        manager: a,
                                         opener: {
                                             open: e => {},
                                             get opened() {
                                                 return {
                                                     connect: () => !1,
                                                     disconnect: () => !1
                                                 }
@@ -283,40 +284,40 @@
                                     const t = s.contextForWidget(e);
                                     void 0 !== t && t.save().then((() => t.createCheckpoint())).catch((e => {
                                         if ("Cancel" !== e.message) throw e
                                     }))
                                 }))
                             }), (() => {
                                 s.stop()
-                            }), n, (e => {
+                            }), a, (e => {
                                 t = e
                             }), (() => t));
-                        n()
+                        a()
                     }
                 };
-            var P = a(4613);
+            var P = n(4613);
             const G = [200, 201];
-            var $, O = a(6311);
+            var $, O = n(6311);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
             }($ || ($ = {}));
             const F = async (e, t) => {
-                const a = z.ServerConnection.makeSettings(),
-                    n = O.URLExt.join(a.baseUrl, e);
+                const n = z.ServerConnection.makeSettings(),
+                    a = O.URLExt.join(n.baseUrl, e);
                 try {
-                    const e = await z.ServerConnection.makeRequest(n, {
+                    const e = await z.ServerConnection.makeRequest(a, {
                         method: t
-                    }, a);
+                    }, n);
                     if (!G.includes(e.status)) throw new Error("Unable to fetch data");
                     return e
                 } catch (e) {
                     throw Error(e)
                 }
             };
-            var V = a(5933);
+            var V = n(5933);
             const Z = "8px",
                 W = "12px",
                 H = V.css`
   border-bottom: solid 1px var(--sm-border-color2);
 `,
                 q = V.css`
   background-color: var(--jp-layout-color2);
@@ -363,59 +364,59 @@
 `,
                 te = V.css`
   border-radius: 10px;
   width: 40px;
   margin: 0 0 2px 4px;
   height: 6px !important;
 `,
-                ae = (V.css`
+                ne = (V.css`
   border-radius: 10px;
   display: inline-block;
   width: 40px;
   height: 8px;
 `, V.css`
   display: flex;
   align-items: center;
 `);
-            var ne = a(8441);
+            var ae = n(8441);
             const se = ({
                     value: e,
                     singleProgressBarStyle: t,
-                    displayValue: a,
-                    label: n,
+                    displayValue: n,
+                    label: a,
                     labelClassName: s,
                     conatinerClassName: i
                 }) => f().createElement("div", {
                     role: "container",
                     "data-testid": "linear-progress-bar-container"
                 }, f().createElement("div", {
                     className: i
-                }, n && f().createElement("span", {
+                }, a && f().createElement("span", {
                     className: s
-                }, n, " ", a, "%"), f().createElement(ne.Z, {
+                }, a, " ", n, "%"), f().createElement(ae.Z, {
                     "data-testid": "linear-progress-bar",
                     className: t,
                     variant: "determinate",
                     value: e
                 }))),
                 ie = "jlStudio-",
                 oe = `${ie}ResourceUsageWidgetContainer`,
                 re = `${ie}MetricsWidgetContainer`,
                 le = ({
                     onClickHandler: e,
                     instanceMetricsResponse: t,
-                    instanceMetricsDisplayValue: a
+                    instanceMetricsDisplayValue: n
                 }) => {
-                    const [n, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
+                    const [a, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
                     (0, E.useEffect)((() => {
                         if (void 0 !== t && (null == t ? void 0 : t.metrics)) {
                             const {
                                 metrics: e
-                            } = t, a = e.cpu.cpu_percentage, n = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
-                            o(a), l(n), d(r)
+                            } = t, n = e.cpu.cpu_percentage, a = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
+                            o(n), l(a), d(r)
                         }
                     }), [t]), (0, E.useEffect)((() => {
                         if (c && c > 95 && !1 === u) {
                             const {
                                 stoargeSpaceLimitDialog: e
                             } = m.ResourceUsage;
                             S.Notification.info(e.title), p(!0)
@@ -430,32 +431,32 @@
                     } = m.ResourceUsage;
                     return f().createElement("div", {
                         "data-testid": "resource-usage-widget",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab",
                         className: `${oe} ${K}`
                     }, f().createElement("div", {
-                        className: ae,
+                        className: ne,
                         onClick: () => (t => {
                             s(!t), e()
-                        })(n),
+                        })(a),
                         "data-testid": "resource-usage-widget-click-handler",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "ResourceUsage-Widget-Click"
-                    }, y, " ", void 0 === a ? f().createElement(ne.Z, {
+                    }, y, " ", void 0 === n ? f().createElement(ae.Z, {
                         "data-testid": "resource-usage-linear-progress-spinner",
                         className: te
                     }) : f().createElement("div", {
-                        className: ae,
+                        className: ne,
                         "data-testid": "resource-usage-status-bar-container"
-                    }, f().createElement(ne.Z, {
+                    }, f().createElement(ae.Z, {
                         className: te,
                         variant: "determinate",
-                        value: 0 | a
-                    }), a ? Math.round(a) : 0, "%")), n && f().createElement("div", {
+                        value: 0 | n
+                    }), n ? Math.round(n) : 0, "%")), a && f().createElement("div", {
                         className: `${re} ${q}`,
                         "data-testid": "resource-usage-data-container"
                     }, f().createElement("div", {
                         className: H
                     }, f().createElement("div", {
                         className: Y
                     }, v), f().createElement("div", {
@@ -489,16 +490,16 @@
             class ce extends S.ReactWidget {
                 constructor() {
                     super(), this.clickHandler = () => {
                         this.update()
                     }, this.getInstanceMetrics = async () => {
                         await F("aws/sagemaker/api/instance/metrics", $.GET).then((e => {
                             e && e.json().then((e => {
-                                var t, a;
-                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (a = this._instanceMetricsResponse) || void 0 === a ? void 0 : a.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
+                                var t, n;
+                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (n = this._instanceMetricsResponse) || void 0 === n ? void 0 : n.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
                             }))
                         })), this.update()
                     }, this._getInstanceMetricsLoop = setInterval(this.getInstanceMetrics, 5e3), this._instanceMetricsResponse = null, this._instanceMetricsDisplayValue = void 0
                 }
                 render() {
                     return f().createElement(le, {
                         onClickHandler: this.clickHandler,
@@ -508,49 +509,49 @@
                 }
             }
             const de = {
                 id: "@amzn/sagemaker-jupyterlab-extensions:resourceusage",
                 requires: [P.IStatusBar],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const a = new ce;
+                    const n = new ce;
                     t.registerStatusItem("@amzn/sagemaker-jupyterlab-extensions:resourceusage:resource-usage-widget", {
-                        item: a,
+                        item: n,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ue = a(8031),
-                pe = a(2715);
+            var ue = n(8031),
+                pe = n(2715);
             const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
                 ge = ({
                     label: e,
                     id: t,
-                    helperText: a,
-                    error: n,
+                    helperText: n,
+                    error: a,
                     handleChange: s,
                     regEx: i,
                     ...o
                 }) => {
                     const [r, l] = (0, E.useState)(""), [c, d] = (0, E.useState)(!0);
                     return f().createElement(pe.Z, {
                         variant: "standard",
                         className: me,
                         "data-testid": "text-field-container",
                         error: !c,
                         id: t,
                         label: e,
-                        helperText: a,
+                        helperText: n,
                         value: r,
                         onChange: e => (e => {
                             l(e.target.value);
                             const t = new RegExp(i);
                             d(t.test(e.target.value)), s(e.target.value)
                         })(e),
                         ...o
@@ -567,84 +568,84 @@
   .MuiFormControl-root.MuiTextField-root {
     margin-bottom: 20px;
   }
 `;
             V.css`
   margin-bottom: 20px;
 `;
-            var ve = a(3776);
+            var ve = n(3776);
             const we = (e = !1) => V.css`
   color: var(--jp-color-root-light-800);
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
   margin-bottom: var(--jp-ui-font-size1);
   ${e&&"\n    &:after {\n      content: '*';\n      color: var(--jp-error-color1);\n    }\n  "}
 `,
                 be = V.css`
   margin-top: 20px;
 `,
                 Ee = ({
                     options: e,
                     handleChange: t,
-                    label: a,
-                    freeSolo: n
+                    label: n,
+                    freeSolo: a
                 }) => {
-                    const s = (e, a) => {
-                        t(a)
+                    const s = (e, n) => {
+                        t(n)
                     };
                     return E.createElement("div", {
                         className: be
                     }, E.createElement("label", {
                         className: we(!0)
-                    }, a), E.createElement(ve.Z, {
+                    }, n), E.createElement(ve.Z, {
                         id: "autocomplete",
-                        freeSolo: n,
+                        freeSolo: a,
                         autoSelect: !0,
                         onChange: (e, t) => s(0, t),
                         onInputChange: (e, t) => s(0, t),
                         options: e.map((e => e.label)),
                         renderInput: e => E.createElement(pe.Z, {
                             ...e,
                             variant: "outlined",
                             size: "small",
                             margin: "dense"
                         })
                     }))
                 };
-            var fe = a(2671),
-                xe = a(847);
+            var fe = n(2671),
+                xe = n(847);
             const Se = ({
                     label: e,
                     id: t,
-                    handleChange: a,
-                    ...n
+                    handleChange: n,
+                    ...a
                 }) => {
                     const [s, i] = (0, E.useState)(!0);
                     return f().createElement(f().Fragment, null, f().createElement(xe.Z, {
                         control: f().createElement(fe.Z, {
                             "data-testid": "checkbox-field",
                             inputProps: {
                                 "aria-label": "controlled"
                             },
                             checked: s,
                             onChange: e => {
-                                i(e.target.checked), a(e.target.checked)
+                                i(e.target.checked), n(e.target.checked)
                             },
                             id: t,
-                            ...n
+                            ...a
                         }),
                         label: e
                     }))
                 },
                 Ce = ({
                     gitRepositories: e,
                     setGitURL: t,
-                    setPath: a,
-                    setOpenREADME: n
+                    setPath: n,
+                    setOpenREADME: a
                 }) => {
                     const [s, i] = (0, E.useState)(""), [o, r] = (0, E.useState)(""), [l, c] = (0, E.useState)(!0), [d, u] = (0, E.useState)([]), {
                         repoTitle: p,
                         pathTitle: g,
                         openReadMeFilesLabel: h
                     } = m.GitClone;
                     return (0, E.useEffect)((() => {
@@ -677,25 +678,25 @@
                         "data-analytics": "GitClone-Path-TextField",
                         error: !1,
                         id: "path",
                         label: g,
                         helperText: "",
                         valuePassed: s,
                         handleChange: e => {
-                            i(e), a(e)
+                            i(e), n(e)
                         },
                         regEx: "^([A-Za-z]*|[0-9]*|[/]*|[.]*|[A-Za-z0-9/.]*)$"
                     }), f().createElement(Se, {
                         "data-testid": "read-me-field",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-OpenReadMeCheckbox",
                         label: h,
                         id: "openReadMe",
                         handleChange: e => {
-                            c(e), n(e)
+                            c(e), a(e)
                         },
                         checked: l
                     }))
                 };
             class Me extends S.ReactWidget {
                 constructor() {
                     super(), this.setGitURL = e => {
@@ -724,85 +725,85 @@
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Re = a(5962),
-                Te = a(2190);
+            var Re = n(5962),
+                Te = n(2190);
             const {
                 name: je,
                 version: ke
-            } = a(4147), De = (e, t, a) => e.child({
+            } = n(4147), De = (e, t, n) => e.child({
                 ExtensionName: je,
                 ExtensionVersion: ke,
                 PluginId: t
-            }, a);
+            }, n);
             var _e;
             ! function(e) {
                 e[e.CanClone = 0] = "CanClone", e[e.NotExist = 1] = "NotExist", e[e.AlreadyCloned = 2] = "AlreadyCloned"
             }(_e || (_e = {}));
             const Ne = [{
                     name: "README.ipynb",
                     factory: "Notebook"
                 }, {
                     name: "README.md",
                     factory: "Markdown Preview"
                 }],
-                Be = async (e, t, a) => {
+                Be = async (e, t, n) => {
                     const {
-                        repoPath: n,
+                        repoPath: a,
                         openREADME: s
-                    } = a;
+                    } = n;
                     if (await e.execute("filebrowser:go-to-path", {
-                            path: n
+                            path: a
                         }), !0 === s) try {
-                        await (async (e, t, a) => {
-                            const n = await t.get(e);
-                            if ("directory" === n.type) {
-                                const t = Ne.find((e => n.content.some((t => t.name === e.name))));
-                                t && await a.execute("docmanager:open", {
+                        await (async (e, t, n) => {
+                            const a = await t.get(e);
+                            if ("directory" === a.type) {
+                                const t = Ne.find((e => a.content.some((t => t.name === e.name))));
+                                t && await n.execute("docmanager:open", {
                                     path: O.PathExt.join(e, t.name),
                                     factory: t.factory
                                 })
                             }
-                        })(n, t, e)
+                        })(a, t, e)
                     } catch (e) {}
                 }, Ie = async (e, t) => {
-                    let a;
+                    let n;
                     try {
-                        a = await t.get(e)
+                        n = await t.get(e)
                     } catch (e) {
                         return !1
                     }
-                    return "directory" === a.type
+                    return "directory" === n.type
                 };
-            var ze = a(1775),
-                Ae = a(248),
-                Ue = a(4337),
-                Le = a(8625);
+            var ze = n(1775),
+                Ae = n(248),
+                Ue = n(4337),
+                Le = n(8625);
             const {
                 dialogTitle: Pe,
                 cancelButton: Ge,
                 cloneButton: $e,
                 errors: Oe
             } = m.GitClone, Fe = {
                 id: s,
                 requires: [ue.IFileBrowserFactory, ue.IDefaultFileBrowser, Te.IGitExtension, S.IToolbarWidgetRegistry, Ae.ILogger, Re.ITranslator],
                 autoStart: !0,
-                activate: async (e, t, a, n, i, o, r) => {
+                activate: async (e, t, n, a, i, o, r) => {
                     const {
                         commands: l,
                         serviceManager: c
                     } = e, d = c.contents, u = De(o, s), p = (r = r || Re.nullTranslator).load("sagemaker_studio");
                     l.addCommand(Ue.TQ.gitClone, {
                         label: "Git Clone Repo",
                         caption: "",
-                        execute: () => (async (e, t, a, n, s) => {
+                        execute: () => (async (e, t, n, a, s) => {
                             var i, o;
                             const r = t.model;
                             let l = "";
                             const c = null === (o = null === (i = null == e ? void 0 : e.tracker) || void 0 === i ? void 0 : i.currentWidget) || void 0 === o ? void 0 : o.model.path;
                             let d, u = null != c ? c : "",
                                 p = !0,
                                 y = !0;
@@ -839,139 +840,139 @@
                             const b = (e => {
                                     const t = O.URLExt.parse(e);
                                     return O.PathExt.basename(t.pathname, ".git")
                                 })(l),
                                 E = O.PathExt.join(u, b);
                             let f;
                             try {
-                                f = await (async (e, t, a, n) => {
+                                f = await (async (e, t, n, a) => {
                                     const {
                                         errors: s
                                     } = m.GitClone;
-                                    return await Ie(t, e) ? await Ie(n, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
-                                        message: s.localGitCloneExistBody + a
+                                    return await Ie(t, e) ? await Ie(a, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
+                                        message: s.localGitCloneExistBody + n
                                     }), _e.AlreadyCloned) : _e.CanClone : (await (0, S.showErrorMessage)(s.directoryNotExistTitle, {
                                         message: s.directoryNotExistBody + t
                                     }), _e.NotExist)
-                                })(a, u, l, E)
+                                })(n, u, l, E)
                             } catch (e) {
                                 s.error({
                                     Message: h,
                                     Error: new Error(JSON.stringify(e))
                                 })
                             }
                             const x = {
                                 repoPath: E,
                                 openREADME: p,
                                 findEnvironment: y
                             };
-                            f === _e.CanClone ? (async (e, t, a, n, s, i) => {
+                            f === _e.CanClone ? (async (e, t, n, a, s, i) => {
                                 const {
                                     errors: o
                                 } = m.GitClone, r = await e.execute("terminal:create-new");
                                 let l = "";
                                 s && (l += `cd ${s} && `), l += `git clone ${i} && exit\r`;
                                 try {
                                     const s = r.content;
                                     s.session.send({
                                         type: "stdin",
                                         content: [l]
-                                    }), s.session.connectionStatusChanged.connect((async n => {
-                                        if ("disconnected" === n.connectionStatus) try {
-                                            await Be(e, t, a)
+                                    }), s.session.connectionStatusChanged.connect((async a => {
+                                        if ("disconnected" === a.connectionStatus) try {
+                                            await Be(e, t, n)
                                         } catch (e) {
                                             await (0, S.showErrorMessage)(o.failedOptions, o.failedOptionsBody, [S.Dialog.warnButton({
                                                 label: "DISMISS"
                                             })])
                                         }
-                                    })), await n.refresh()
+                                    })), await a.refresh()
                                 } catch (e) {
                                     r.dispose(), await (0, S.showErrorMessage)(o.generalCloneErrorTitle, {
                                         message: o.generalCloneErrorBody + e
                                     })
                                 }
-                            })(n, a, x, r, u, l) : f === _e.AlreadyCloned && Be(n, a, x)
-                        })(t, a, d, l, u),
+                            })(a, n, x, r, u, l) : f === _e.AlreadyCloned && Be(a, n, x)
+                        })(t, n, d, l, u),
                         isEnabled: () => e.serviceManager.terminals.isAvailable()
                     }), i.addFactory("FileBrowser", "gitClone", (() => S.ReactWidget.create(f().createElement(S.UseSignal, {
-                        signal: n.repositoryChanged,
+                        signal: a.repositoryChanged,
                         initialArgs: {
                             name: "pathRepository",
                             oldValue: null,
-                            newValue: n.pathRepository
+                            newValue: a.pathRepository
                         }
-                    }, ((t, a) => f().createElement(S.ToolbarButtonComponent, {
-                        enabled: null === (null == a ? void 0 : a.newValue),
+                    }, ((t, n) => f().createElement(S.ToolbarButtonComponent, {
+                        enabled: null === (null == n ? void 0 : n.newValue),
                         icon: Le.W6,
                         onClick: () => {
                             e.commands.execute(Ue.TQ.gitClone)
                         },
                         tooltip: p.__("Git Clone")
-                    })))))), (0, ze.ZM)(n, a, e.serviceManager.contents, e.contextMenu, p), u.info({
+                    })))))), (0, ze.ZM)(a, n, e.serviceManager.contents, e.contextMenu, p), u.info({
                         Message: "Successfully loaded Git extension"
                     })
                 }
             }, Ve = e => {
-                var t, a;
-                const n = `${e}.AWSSageMakerUI`;
-                return performance.mark(n), performance.measure(n, void 0, n), null !== (a = null === (t = performance.getEntriesByName(n, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== a ? a : 0
+                var t, n;
+                const a = `${e}.AWSSageMakerUI`;
+                return performance.mark(a), performance.measure(a, void 0, a), null !== (n = null === (t = performance.getEntriesByName(a, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== n ? n : 0
             }, Ze = {
                 id: i,
                 requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: (e, t) => {
                     ((e, t) => {
-                        const a = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
-                        let n = {};
-                        Array.isArray(a) && a.length > 0 && a.forEach((e => {
+                        const n = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
+                        let a = {};
+                        Array.isArray(n) && n.length > 0 && n.forEach((e => {
                             const {
                                 duration: t,
-                                requestStart: a,
+                                requestStart: n,
                                 responseStart: s,
                                 startTime: i
                             } = e;
-                            a && t && (n = {
-                                ...n,
+                            n && t && (a = {
+                                ...a,
                                 TimeToFirstByteMS: Math.round(s - i)
                             })
                         }));
                         let s = null,
                             i = null,
                             o = null,
                             r = null,
                             l = null;
                         const c = performance.getEntriesByType("navigation")[0];
                         if (c) s = c.redirectCount, i = c.redirectEnd - c.redirectStart, o = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
                         else {
                             const e = performance.timing;
                             s = performance.navigation.redirectCount, i = e.redirectEnd - e.redirectStart, o = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
                         }
-                        n = {
-                            ...n,
+                        a = {
+                            ...a,
                             RedirectCount: s,
                             RedirectTimeMS: i,
                             TimeToDOMContentLoadedMS: o,
                             TimeToFirstByteMS: r,
                             TimeToOnLoadMS: l
-                        }, e.info(n), t.started.then((() => {
+                        }, e.info(a), t.started.then((() => {
                             e.info({
                                 TimeToAppStartedMS: Math.round(Ve("timeToAppStarted"))
                             })
                         })), t.restored.then((() => {
-                            const t = (a = Math.round(Ve("timeToAppRestored"))) > 0 ? a : null;
-                            var a;
+                            const t = (n = Math.round(Ve("timeToAppRestored"))) > 0 ? n : null;
+                            var n;
                             e.info({
                                 TimeToAppRestoredMS: t || void 0
                             })
                         }))
                     })(De(t, i, Ae.logSchemas.performance), e)
                 }
             };
-            var We = a(87),
-                He = a(8201);
+            var We = n(87),
+                He = n(8201);
             const qe = {
                     SpaceMenuHeader: V.css`
   margin: -6px 0;
   padding: 0 var(--jp-size-2);
   height: 10;
   border-radius: var(--jp-radius-small);
   font-size: var(--jp-size-3);
@@ -987,30 +988,30 @@
 
   & > svg {
     padding: 0 var(--jp-size-2);
   }
 `
                 },
                 {
-                    privateSpaceHeader: Je,
+                    unknownSpace: Je,
                     unknownUser: Ye
                 } = m.Space,
                 Qe = ({
                     spaceName: e
                 }) => {
                     const t = !!e,
-                        a = R("studioUserProfileName");
+                        n = R("studioUserProfileName");
                     return f().createElement("div", {
                         className: qe.SpaceMenuHeader,
                         "data-testid": y
                     }, t ? f().createElement(We.Z, {
                         fontSize: "small"
                     }) : f().createElement(He.Z, {
                         fontSize: "small"
-                    }), f().createElement("p", null, `${a||Ye} / ${t?e:Je}`))
+                    }), f().createElement("p", null, `${n&&n[1]||Ye} / ${t?e:Je}`))
                 };
             class Ke extends S.ReactWidget {
                 constructor() {
                     super(), this.getSpaceName = async () => {
                         await F("aws/sagemaker/api/context", $.GET).then((e => {
                             e && e.json().then((e => {
                                 this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
@@ -1025,48 +1026,48 @@
                 }
             }
             const Xe = [v, L, de, Fe, Ze, {
                 id: o,
                 requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const a = new Ke;
-                    a.id = S.DOMUtils.createDomID();
-                    const n = De(t, o);
-                    e.shell.add(a, "top", {
+                    const n = new Ke;
+                    n.id = S.DOMUtils.createDomID();
+                    const a = De(t, o);
+                    e.shell.add(n, "top", {
                         rank: 1e3
                     }), window && window.panorama && window.panorama("trackCustomEvent", {
                         eventType: "render",
                         eventDetail: "Space-Plugin",
                         eventContext: "JupyterLab",
                         timestamp: Date.now()
-                    }), n.info({
+                    }), a.info({
                         Message: "Successfully loaded Space plugin"
                     })
                 }
             }]
         },
-        8201: (e, t, a) => {
-            var n = a(5318);
+        8201: (e, t, n) => {
+            var a = n(5318);
             t.Z = void 0;
-            var s = n(a(4938)),
-                i = a(5893),
+            var s = a(n(4938)),
+                i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 4c1.93 0 3.5 1.57 3.5 3.5S13.93 13 12 13s-3.5-1.57-3.5-3.5S10.07 6 12 6zm0 14c-2.03 0-4.43-.82-6.14-2.88C7.55 15.8 9.68 15 12 15s4.45.8 6.14 2.12C16.43 19.18 14.03 20 12 20z"
                 }), "AccountCircle");
             t.Z = o
         },
-        87: (e, t, a) => {
-            var n = a(5318);
+        87: (e, t, n) => {
+            var a = n(5318);
             t.Z = void 0;
-            var s = n(a(4938)),
-                i = a(5893),
+            var s = a(n(4938)),
+                i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
                 }), "Language");
             t.Z = o
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.1","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js` & `sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -6188,15 +6188,15 @@
                     })
                 }));
             var Ns = o(8543),
                 Bs = o(5827),
                 js = o(76),
                 zs = o(6727),
                 Os = o(8441),
-                Ds = o(7651),
+                Ds = o(8962),
                 Es = o(9674);
 
             function Fs(e) {
                 return (0, Je.Z)("MuiLink", e)
             }
             const Ws = (0, Ke.Z)("MuiLink", ["root", "underlineNone", "underlineHover", "underlineAlways", "button", "focusVisible"]);
             var Us = o(4844);
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js` & `sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -5740,15 +5740,15 @@
                             return l(arguments, "callee").get
                         } catch (e) {
                             return c
                         }
                     }
                 }() : c,
                 d = i(1405)(),
-                u = i(8185)(),
+                u = i(3276)(),
                 f = Object.getPrototypeOf || (u ? function(e) {
                     return e.__proto__
                 } : null),
                 p = {},
                 g = "undefined" != typeof Uint8Array && f ? f(Uint8Array) : n,
                 m = {
                     "%AggregateError%": "undefined" == typeof AggregateError ? n : AggregateError,
@@ -5985,15 +5985,15 @@
                         value: 1
                     }).length
                 } catch (e) {
                     return !0
                 }
             }, e.exports = s
         },
-        8185: e => {
+        3276: e => {
             "use strict";
             var t = {
                     foo: {}
                 },
                 i = Object;
             e.exports = function() {
                 return {
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js` & `sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js`

 * *Files 4% similar despite different names*

##### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
-            1514: (e, r, t) => {
+            3570: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -48,58 +48,58 @@
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "2135a6297693b09662d9",
+        181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "5350b743f9a235d9e265",
+        548: "a6ac1d0d39311897c48d",
         571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "c508feab9dfdf7494214",
+        799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "7f061638d47075ac76be",
+        823: "26c15aab8d5d7301c11a",
         853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
         891: "4794a088a65e99550778"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "2135a6297693b09662d9",
+        181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "5350b743f9a235d9e265",
+        548: "a6ac1d0d39311897c48d",
         571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "c508feab9dfdf7494214",
+        799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "7f061638d47075ac76be",
+        823: "26c15aab8d5d7301c11a",
         853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
         891: "4794a088a65e99550778"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.1", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(1514);
+    var E = S(3570);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/THIRD-PARTY-LICENSES` & `sagemaker_jupyterlab_extension-0.3.1.data/data/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json`

 * *Files 1% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.9661111111111111%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7282f69f1fc0d8e37b1c.js'}}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -60,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.27a0e3dfb32431afe940.js",
+            "load": "static/remoteEntry.7282f69f1fc0d8e37b1c.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -105,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.2135a6297693b09662d9.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -2749,15 +2749,15 @@
                 l = o(4780),
                 s = o(917),
                 d = o(1796),
                 c = o(8216),
                 p = o(2734),
                 u = o(948),
                 m = o(1657),
-                f = o(7651),
+                f = o(8962),
                 h = o(5893);
             const b = ["className", "color", "value", "valueBuffer", "variant"];
             let v, g, Z, x, y, S, C = e => e;
             const P = (0, s.F4)(v || (v = C`
   0% {
     left: -35%;
     right: 100%;
@@ -3002,15 +3002,15 @@
                             className: x.bar2,
                             ownerState: Z,
                             style: C.bar2
                         })]
                     }))
                 }))
         },
-        7651: (e, t, o) => {
+        8962: (e, t, o) => {
             o.d(t, {
                 E: () => a,
                 Z: () => i
             });
             var r = o(1588),
                 n = o(4867);
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.5350b743f9a235d9e265.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.a6ac1d0d39311897c48d.js`

 * *Files 4% similar despite different names*

##### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [548], {
-        4548: (e, t, a) => {
-            a.r(t), a.d(t, {
+        4548: (e, t, n) => {
+            n.r(t), n.d(t, {
                 default: () => Xe
             });
-            var n = a(9557);
+            var a = n(9557);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
                 i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
                 o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
                 r = {
                     shutdown: "filemenu:shutdown"
                 },
                 l = "Sso",
@@ -75,34 +75,35 @@
                             failedOptionsBody: "Something went wrong when trying to open README file within the repo.",
                             invalidCloneUrlTitle: "Invalid URL provided",
                             invalidCloneUrlBody: "The URL provided is not valid. Please input a valid URL to clone."
                         }
                     },
                     Space: {
                         privateSpaceHeader: "Personal Studio",
-                        unknownUser: "Unknown User"
+                        unknownUser: "Unknown User",
+                        unknownSpace: "Unknown Space"
                     }
                 },
                 g = "GitCloneDialogError",
                 h = "ValidRepoPathError",
                 y = "spaceMenuHeader",
                 v = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:hideshutdown",
-                    requires: [n.IMainMenu],
+                    requires: [a.IMainMenu],
                     autoStart: !0,
                     activate: (e, t) => {
                         e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
-            var w = a(9801),
-                b = a.n(w),
-                E = a(6029),
-                f = a.n(E),
-                x = a(8368),
-                S = a(9510);
+            var w = n(9801),
+                b = n.n(w),
+                E = n(6029),
+                f = n.n(E),
+                x = n(8368),
+                S = n(9510);
             class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
@@ -117,162 +118,162 @@
                 R = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
                 T = () => {
                     const e = R("expiryTime"),
                         t = R("ssoExpiryTimestamp");
                     return M() && t ? Number(t[1]) : e ? Number(e[1]) : null
                 },
                 j = (e, t) => {
-                    var a, n;
-                    t ? null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.disconnect(x.ConnectionLost) : null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.connect(x.ConnectionLost)
+                    var n, a;
+                    t ? null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.disconnect(x.ConnectionLost) : null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.connect(x.ConnectionLost)
                 },
                 k = () => {
                     const e = R("redirectURL");
                     let t;
                     try {
                         if (t = new URL(e ? e[1] : void 0), "http:" === t.protocol || "https:" === t.protocol) return t.toString()
                     } catch (e) {
                         return
                     }
                 },
                 D = (e, t) => {
-                    const a = T(),
-                        n = window.open(e, "signin window", "width=800, height=600");
+                    const n = T(),
+                        a = window.open(e, "signin window", "width=800, height=600");
                     let s = !1;
                     const i = window.setInterval((() => {
-                        if (n && n.closed && !s) return void window.clearInterval(i);
+                        if (a && a.closed && !s) return void window.clearInterval(i);
                         const e = T();
-                        if (null !== e && null !== a && (e > a || isNaN(e))) {
-                            window.clearInterval(i), n && n.close(), s = !0;
+                        if (null !== e && null !== n && (e > n || isNaN(e))) {
+                            window.clearInterval(i), a && a.close(), s = !0;
                             for (const e of t) e.kernel.reconnect();
                             S.Dialog.tracker.forEach((e => e.reject()))
                         }
                     }), u)
                 },
                 _ = async () => {
                     const {
                         SignInSession: e
                     } = m, {
                         signinDialog: t
-                    } = e, a = k(), n = a ? [S.Dialog.okButton({
+                    } = e, n = k(), a = n ? [S.Dialog.okButton({
                         label: e.signInButton
                     })] : [S.Dialog.cancelButton({
                         label: e.closeButton
-                    })], s = a ? f().createElement("div", {
+                    })], s = n ? f().createElement("div", {
                         "data-testid": "session-signin-log-out"
                     }, t.loggedOutBody) : f().createElement("div", {
                         "data-testid": "session-signin-restart"
                     }, t.restartSessionBody), i = new S.Dialog({
                         title: t.title,
                         body: s,
-                        buttons: n,
+                        buttons: a,
                         hasClose: !1
                     });
                     return {
                         sigInDialogResult: await i.launch(),
                         confirmDialog: i
                     }
                 };
-            var N = a(6797),
-                B = a(6697),
-                I = a(1638),
-                z = a(7217),
-                A = a(5326);
-            const U = (e, t, a, n, s, i, o) => {
+            var N = n(6797),
+                B = n(6697),
+                I = n(1638),
+                z = n(7217),
+                A = n(5326);
+            const U = (e, t, n, a, s, i, o) => {
                     const r = T(),
                         l = o(),
                         d = l && l + c;
                     if (null === r) j(e, !1);
                     else {
                         const o = b().unix(r / 1e3).diff(b()()),
                             u = Date.now();
-                        ((e, t, a) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(a, e))(M(), r, o) ? (n(), (async (e, t, a) => {
+                        ((e, t, n) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(n, e))(M(), r, o) ? (a(), (async (e, t, n) => {
                             const {
-                                SignInSession: n
+                                SignInSession: a
                             } = m, s = k();
                             S.Dialog.tracker.forEach((e => e.reject())), j(e, !0);
                             const {
                                 sigInDialogResult: i,
                                 confirmDialog: o
                             } = await _();
                             if (i && i.button)
-                                if (a(), s) D(k(), t);
-                                else if (i && i.button.label === n.closeButton) {
+                                if (n(), s) D(k(), t);
+                                else if (i && i.button.label === a.closeButton) {
                                 const e = T(),
                                     t = e && e / 1e3,
-                                    a = t && b().unix(t).diff(b()());
-                                null !== a && a && a > c && (o.dispose(), setTimeout((async () => {
+                                    n = t && b().unix(t).diff(b()());
+                                null !== n && n && n > c && (o.dispose(), setTimeout((async () => {
                                     await _()
                                 }), c))
                             } else o.dispose(), D(k(), t)
-                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (n(), (async (e, t, a, n, s) => {
+                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (a(), (async (e, t, n, a, s) => {
                             const {
                                 SignInSession: i
                             } = m, {
                                 renewSessionDialog: o
                             } = m.SignInSession, {
                                 renewSessionDialogResult: r,
                                 confirmDialog: l
                             } = await (async () => {
                                 const {
                                     SignInSession: e
                                 } = m, {
                                     renewSessionDialog: t
-                                } = m.SignInSession, a = k(), n = T(), s = n && b().unix(n / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
+                                } = m.SignInSession, n = k(), a = T(), s = a && b().unix(a / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
                                     "data-testid": "session-renew-lose-unsaved-changes"
                                 }, o, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), f().createElement("div", null, r)) : f().createElement("div", {
                                     "data-testid": "session-renew-now"
                                 }, f().createElement("p", null, o), f().createElement("p", null, t.renewSessionNow)), c = [S.Dialog.okButton({
                                     label: t.remindText
-                                }), a && S.Dialog.okButton({
+                                }), n && S.Dialog.okButton({
                                     label: e.saveAndRenewButton
                                 })], d = new S.Dialog({
                                     title: t.title,
                                     body: l,
                                     buttons: c,
                                     hasClose: !1
                                 });
                                 return {
                                     renewSessionDialogResult: await d.launch(),
                                     confirmDialog: d
                                 }
                             })();
                             if (r && r.button.label === o.remindText) {
                                 const e = new C;
-                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), n()
-                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), a(), n(), M() || D(k(), t))
-                        })(0, t._sessions, a, s, i), j(e, !1)) : j(e, !1)
+                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), a()
+                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), n(), a(), M() || D(k(), t))
+                        })(0, t._sessions, n, s, i), j(e, !1)) : j(e, !1)
                     }
                 },
                 L = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:sessionmanagement",
                     requires: [],
                     autoStart: !0,
                     activate: async e => {
                         let t;
-                        const a = e.serviceManager.sessions,
-                            n = () => {
+                        const n = e.serviceManager.sessions,
+                            a = () => {
                                 s.start()
                             },
-                            s = ((e, t, a, n, s, i, o) => new N.Poll({
+                            s = ((e, t, n, a, s, i, o) => new N.Poll({
                                 auto: !0,
-                                factory: async () => U(e, t, a, n, s, i, o),
+                                factory: async () => U(e, t, n, a, s, i, o),
                                 frequency: {
                                     interval: d,
                                     backoff: !0,
                                     max: p
                                 }
-                            }))(e, a, (() => {
+                            }))(e, n, (() => {
                                 const t = new I.TextModelFactory,
-                                    a = new I.DocumentRegistry({
+                                    n = new I.DocumentRegistry({
                                         textModelFactory: t
                                     }),
-                                    n = new z.ServiceManager({}),
+                                    a = new z.ServiceManager({}),
                                     s = new A.DocumentManager({
-                                        registry: a,
-                                        manager: n,
+                                        registry: n,
+                                        manager: a,
                                         opener: {
                                             open: e => {},
                                             get opened() {
                                                 return {
                                                     connect: () => !1,
                                                     disconnect: () => !1
                                                 }
@@ -283,40 +284,40 @@
                                     const t = s.contextForWidget(e);
                                     void 0 !== t && t.save().then((() => t.createCheckpoint())).catch((e => {
                                         if ("Cancel" !== e.message) throw e
                                     }))
                                 }))
                             }), (() => {
                                 s.stop()
-                            }), n, (e => {
+                            }), a, (e => {
                                 t = e
                             }), (() => t));
-                        n()
+                        a()
                     }
                 };
-            var P = a(4613);
+            var P = n(4613);
             const G = [200, 201];
-            var $, O = a(6311);
+            var $, O = n(6311);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
             }($ || ($ = {}));
             const F = async (e, t) => {
-                const a = z.ServerConnection.makeSettings(),
-                    n = O.URLExt.join(a.baseUrl, e);
+                const n = z.ServerConnection.makeSettings(),
+                    a = O.URLExt.join(n.baseUrl, e);
                 try {
-                    const e = await z.ServerConnection.makeRequest(n, {
+                    const e = await z.ServerConnection.makeRequest(a, {
                         method: t
-                    }, a);
+                    }, n);
                     if (!G.includes(e.status)) throw new Error("Unable to fetch data");
                     return e
                 } catch (e) {
                     throw Error(e)
                 }
             };
-            var V = a(5933);
+            var V = n(5933);
             const Z = "8px",
                 W = "12px",
                 H = V.css`
   border-bottom: solid 1px var(--sm-border-color2);
 `,
                 q = V.css`
   background-color: var(--jp-layout-color2);
@@ -363,59 +364,59 @@
 `,
                 te = V.css`
   border-radius: 10px;
   width: 40px;
   margin: 0 0 2px 4px;
   height: 6px !important;
 `,
-                ae = (V.css`
+                ne = (V.css`
   border-radius: 10px;
   display: inline-block;
   width: 40px;
   height: 8px;
 `, V.css`
   display: flex;
   align-items: center;
 `);
-            var ne = a(8441);
+            var ae = n(8441);
             const se = ({
                     value: e,
                     singleProgressBarStyle: t,
-                    displayValue: a,
-                    label: n,
+                    displayValue: n,
+                    label: a,
                     labelClassName: s,
                     conatinerClassName: i
                 }) => f().createElement("div", {
                     role: "container",
                     "data-testid": "linear-progress-bar-container"
                 }, f().createElement("div", {
                     className: i
-                }, n && f().createElement("span", {
+                }, a && f().createElement("span", {
                     className: s
-                }, n, " ", a, "%"), f().createElement(ne.Z, {
+                }, a, " ", n, "%"), f().createElement(ae.Z, {
                     "data-testid": "linear-progress-bar",
                     className: t,
                     variant: "determinate",
                     value: e
                 }))),
                 ie = "jlStudio-",
                 oe = `${ie}ResourceUsageWidgetContainer`,
                 re = `${ie}MetricsWidgetContainer`,
                 le = ({
                     onClickHandler: e,
                     instanceMetricsResponse: t,
-                    instanceMetricsDisplayValue: a
+                    instanceMetricsDisplayValue: n
                 }) => {
-                    const [n, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
+                    const [a, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
                     (0, E.useEffect)((() => {
                         if (void 0 !== t && (null == t ? void 0 : t.metrics)) {
                             const {
                                 metrics: e
-                            } = t, a = e.cpu.cpu_percentage, n = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
-                            o(a), l(n), d(r)
+                            } = t, n = e.cpu.cpu_percentage, a = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
+                            o(n), l(a), d(r)
                         }
                     }), [t]), (0, E.useEffect)((() => {
                         if (c && c > 95 && !1 === u) {
                             const {
                                 stoargeSpaceLimitDialog: e
                             } = m.ResourceUsage;
                             S.Notification.info(e.title), p(!0)
@@ -430,32 +431,32 @@
                     } = m.ResourceUsage;
                     return f().createElement("div", {
                         "data-testid": "resource-usage-widget",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab",
                         className: `${oe} ${K}`
                     }, f().createElement("div", {
-                        className: ae,
+                        className: ne,
                         onClick: () => (t => {
                             s(!t), e()
-                        })(n),
+                        })(a),
                         "data-testid": "resource-usage-widget-click-handler",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "ResourceUsage-Widget-Click"
-                    }, y, " ", void 0 === a ? f().createElement(ne.Z, {
+                    }, y, " ", void 0 === n ? f().createElement(ae.Z, {
                         "data-testid": "resource-usage-linear-progress-spinner",
                         className: te
                     }) : f().createElement("div", {
-                        className: ae,
+                        className: ne,
                         "data-testid": "resource-usage-status-bar-container"
-                    }, f().createElement(ne.Z, {
+                    }, f().createElement(ae.Z, {
                         className: te,
                         variant: "determinate",
-                        value: 0 | a
-                    }), a ? Math.round(a) : 0, "%")), n && f().createElement("div", {
+                        value: 0 | n
+                    }), n ? Math.round(n) : 0, "%")), a && f().createElement("div", {
                         className: `${re} ${q}`,
                         "data-testid": "resource-usage-data-container"
                     }, f().createElement("div", {
                         className: H
                     }, f().createElement("div", {
                         className: Y
                     }, v), f().createElement("div", {
@@ -489,16 +490,16 @@
             class ce extends S.ReactWidget {
                 constructor() {
                     super(), this.clickHandler = () => {
                         this.update()
                     }, this.getInstanceMetrics = async () => {
                         await F("aws/sagemaker/api/instance/metrics", $.GET).then((e => {
                             e && e.json().then((e => {
-                                var t, a;
-                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (a = this._instanceMetricsResponse) || void 0 === a ? void 0 : a.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
+                                var t, n;
+                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (n = this._instanceMetricsResponse) || void 0 === n ? void 0 : n.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
                             }))
                         })), this.update()
                     }, this._getInstanceMetricsLoop = setInterval(this.getInstanceMetrics, 5e3), this._instanceMetricsResponse = null, this._instanceMetricsDisplayValue = void 0
                 }
                 render() {
                     return f().createElement(le, {
                         onClickHandler: this.clickHandler,
@@ -508,49 +509,49 @@
                 }
             }
             const de = {
                 id: "@amzn/sagemaker-jupyterlab-extensions:resourceusage",
                 requires: [P.IStatusBar],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const a = new ce;
+                    const n = new ce;
                     t.registerStatusItem("@amzn/sagemaker-jupyterlab-extensions:resourceusage:resource-usage-widget", {
-                        item: a,
+                        item: n,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ue = a(8031),
-                pe = a(2715);
+            var ue = n(8031),
+                pe = n(2715);
             const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
                 ge = ({
                     label: e,
                     id: t,
-                    helperText: a,
-                    error: n,
+                    helperText: n,
+                    error: a,
                     handleChange: s,
                     regEx: i,
                     ...o
                 }) => {
                     const [r, l] = (0, E.useState)(""), [c, d] = (0, E.useState)(!0);
                     return f().createElement(pe.Z, {
                         variant: "standard",
                         className: me,
                         "data-testid": "text-field-container",
                         error: !c,
                         id: t,
                         label: e,
-                        helperText: a,
+                        helperText: n,
                         value: r,
                         onChange: e => (e => {
                             l(e.target.value);
                             const t = new RegExp(i);
                             d(t.test(e.target.value)), s(e.target.value)
                         })(e),
                         ...o
@@ -567,84 +568,84 @@
   .MuiFormControl-root.MuiTextField-root {
     margin-bottom: 20px;
   }
 `;
             V.css`
   margin-bottom: 20px;
 `;
-            var ve = a(3776);
+            var ve = n(3776);
             const we = (e = !1) => V.css`
   color: var(--jp-color-root-light-800);
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
   margin-bottom: var(--jp-ui-font-size1);
   ${e&&"\n    &:after {\n      content: '*';\n      color: var(--jp-error-color1);\n    }\n  "}
 `,
                 be = V.css`
   margin-top: 20px;
 `,
                 Ee = ({
                     options: e,
                     handleChange: t,
-                    label: a,
-                    freeSolo: n
+                    label: n,
+                    freeSolo: a
                 }) => {
-                    const s = (e, a) => {
-                        t(a)
+                    const s = (e, n) => {
+                        t(n)
                     };
                     return E.createElement("div", {
                         className: be
                     }, E.createElement("label", {
                         className: we(!0)
-                    }, a), E.createElement(ve.Z, {
+                    }, n), E.createElement(ve.Z, {
                         id: "autocomplete",
-                        freeSolo: n,
+                        freeSolo: a,
                         autoSelect: !0,
                         onChange: (e, t) => s(0, t),
                         onInputChange: (e, t) => s(0, t),
                         options: e.map((e => e.label)),
                         renderInput: e => E.createElement(pe.Z, {
                             ...e,
                             variant: "outlined",
                             size: "small",
                             margin: "dense"
                         })
                     }))
                 };
-            var fe = a(2671),
-                xe = a(847);
+            var fe = n(2671),
+                xe = n(847);
             const Se = ({
                     label: e,
                     id: t,
-                    handleChange: a,
-                    ...n
+                    handleChange: n,
+                    ...a
                 }) => {
                     const [s, i] = (0, E.useState)(!0);
                     return f().createElement(f().Fragment, null, f().createElement(xe.Z, {
                         control: f().createElement(fe.Z, {
                             "data-testid": "checkbox-field",
                             inputProps: {
                                 "aria-label": "controlled"
                             },
                             checked: s,
                             onChange: e => {
-                                i(e.target.checked), a(e.target.checked)
+                                i(e.target.checked), n(e.target.checked)
                             },
                             id: t,
-                            ...n
+                            ...a
                         }),
                         label: e
                     }))
                 },
                 Ce = ({
                     gitRepositories: e,
                     setGitURL: t,
-                    setPath: a,
-                    setOpenREADME: n
+                    setPath: n,
+                    setOpenREADME: a
                 }) => {
                     const [s, i] = (0, E.useState)(""), [o, r] = (0, E.useState)(""), [l, c] = (0, E.useState)(!0), [d, u] = (0, E.useState)([]), {
                         repoTitle: p,
                         pathTitle: g,
                         openReadMeFilesLabel: h
                     } = m.GitClone;
                     return (0, E.useEffect)((() => {
@@ -677,25 +678,25 @@
                         "data-analytics": "GitClone-Path-TextField",
                         error: !1,
                         id: "path",
                         label: g,
                         helperText: "",
                         valuePassed: s,
                         handleChange: e => {
-                            i(e), a(e)
+                            i(e), n(e)
                         },
                         regEx: "^([A-Za-z]*|[0-9]*|[/]*|[.]*|[A-Za-z0-9/.]*)$"
                     }), f().createElement(Se, {
                         "data-testid": "read-me-field",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-OpenReadMeCheckbox",
                         label: h,
                         id: "openReadMe",
                         handleChange: e => {
-                            c(e), n(e)
+                            c(e), a(e)
                         },
                         checked: l
                     }))
                 };
             class Me extends S.ReactWidget {
                 constructor() {
                     super(), this.setGitURL = e => {
@@ -724,85 +725,85 @@
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Re = a(5962),
-                Te = a(2190);
+            var Re = n(5962),
+                Te = n(2190);
             const {
                 name: je,
                 version: ke
-            } = a(4147), De = (e, t, a) => e.child({
+            } = n(4147), De = (e, t, n) => e.child({
                 ExtensionName: je,
                 ExtensionVersion: ke,
                 PluginId: t
-            }, a);
+            }, n);
             var _e;
             ! function(e) {
                 e[e.CanClone = 0] = "CanClone", e[e.NotExist = 1] = "NotExist", e[e.AlreadyCloned = 2] = "AlreadyCloned"
             }(_e || (_e = {}));
             const Ne = [{
                     name: "README.ipynb",
                     factory: "Notebook"
                 }, {
                     name: "README.md",
                     factory: "Markdown Preview"
                 }],
-                Be = async (e, t, a) => {
+                Be = async (e, t, n) => {
                     const {
-                        repoPath: n,
+                        repoPath: a,
                         openREADME: s
-                    } = a;
+                    } = n;
                     if (await e.execute("filebrowser:go-to-path", {
-                            path: n
+                            path: a
                         }), !0 === s) try {
-                        await (async (e, t, a) => {
-                            const n = await t.get(e);
-                            if ("directory" === n.type) {
-                                const t = Ne.find((e => n.content.some((t => t.name === e.name))));
-                                t && await a.execute("docmanager:open", {
+                        await (async (e, t, n) => {
+                            const a = await t.get(e);
+                            if ("directory" === a.type) {
+                                const t = Ne.find((e => a.content.some((t => t.name === e.name))));
+                                t && await n.execute("docmanager:open", {
                                     path: O.PathExt.join(e, t.name),
                                     factory: t.factory
                                 })
                             }
-                        })(n, t, e)
+                        })(a, t, e)
                     } catch (e) {}
                 }, Ie = async (e, t) => {
-                    let a;
+                    let n;
                     try {
-                        a = await t.get(e)
+                        n = await t.get(e)
                     } catch (e) {
                         return !1
                     }
-                    return "directory" === a.type
+                    return "directory" === n.type
                 };
-            var ze = a(1775),
-                Ae = a(248),
-                Ue = a(4337),
-                Le = a(8625);
+            var ze = n(1775),
+                Ae = n(248),
+                Ue = n(4337),
+                Le = n(8625);
             const {
                 dialogTitle: Pe,
                 cancelButton: Ge,
                 cloneButton: $e,
                 errors: Oe
             } = m.GitClone, Fe = {
                 id: s,
                 requires: [ue.IFileBrowserFactory, ue.IDefaultFileBrowser, Te.IGitExtension, S.IToolbarWidgetRegistry, Ae.ILogger, Re.ITranslator],
                 autoStart: !0,
-                activate: async (e, t, a, n, i, o, r) => {
+                activate: async (e, t, n, a, i, o, r) => {
                     const {
                         commands: l,
                         serviceManager: c
                     } = e, d = c.contents, u = De(o, s), p = (r = r || Re.nullTranslator).load("sagemaker_studio");
                     l.addCommand(Ue.TQ.gitClone, {
                         label: "Git Clone Repo",
                         caption: "",
-                        execute: () => (async (e, t, a, n, s) => {
+                        execute: () => (async (e, t, n, a, s) => {
                             var i, o;
                             const r = t.model;
                             let l = "";
                             const c = null === (o = null === (i = null == e ? void 0 : e.tracker) || void 0 === i ? void 0 : i.currentWidget) || void 0 === o ? void 0 : o.model.path;
                             let d, u = null != c ? c : "",
                                 p = !0,
                                 y = !0;
@@ -839,139 +840,139 @@
                             const b = (e => {
                                     const t = O.URLExt.parse(e);
                                     return O.PathExt.basename(t.pathname, ".git")
                                 })(l),
                                 E = O.PathExt.join(u, b);
                             let f;
                             try {
-                                f = await (async (e, t, a, n) => {
+                                f = await (async (e, t, n, a) => {
                                     const {
                                         errors: s
                                     } = m.GitClone;
-                                    return await Ie(t, e) ? await Ie(n, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
-                                        message: s.localGitCloneExistBody + a
+                                    return await Ie(t, e) ? await Ie(a, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
+                                        message: s.localGitCloneExistBody + n
                                     }), _e.AlreadyCloned) : _e.CanClone : (await (0, S.showErrorMessage)(s.directoryNotExistTitle, {
                                         message: s.directoryNotExistBody + t
                                     }), _e.NotExist)
-                                })(a, u, l, E)
+                                })(n, u, l, E)
                             } catch (e) {
                                 s.error({
                                     Message: h,
                                     Error: new Error(JSON.stringify(e))
                                 })
                             }
                             const x = {
                                 repoPath: E,
                                 openREADME: p,
                                 findEnvironment: y
                             };
-                            f === _e.CanClone ? (async (e, t, a, n, s, i) => {
+                            f === _e.CanClone ? (async (e, t, n, a, s, i) => {
                                 const {
                                     errors: o
                                 } = m.GitClone, r = await e.execute("terminal:create-new");
                                 let l = "";
                                 s && (l += `cd ${s} && `), l += `git clone ${i} && exit\r`;
                                 try {
                                     const s = r.content;
                                     s.session.send({
                                         type: "stdin",
                                         content: [l]
-                                    }), s.session.connectionStatusChanged.connect((async n => {
-                                        if ("disconnected" === n.connectionStatus) try {
-                                            await Be(e, t, a)
+                                    }), s.session.connectionStatusChanged.connect((async a => {
+                                        if ("disconnected" === a.connectionStatus) try {
+                                            await Be(e, t, n)
                                         } catch (e) {
                                             await (0, S.showErrorMessage)(o.failedOptions, o.failedOptionsBody, [S.Dialog.warnButton({
                                                 label: "DISMISS"
                                             })])
                                         }
-                                    })), await n.refresh()
+                                    })), await a.refresh()
                                 } catch (e) {
                                     r.dispose(), await (0, S.showErrorMessage)(o.generalCloneErrorTitle, {
                                         message: o.generalCloneErrorBody + e
                                     })
                                 }
-                            })(n, a, x, r, u, l) : f === _e.AlreadyCloned && Be(n, a, x)
-                        })(t, a, d, l, u),
+                            })(a, n, x, r, u, l) : f === _e.AlreadyCloned && Be(a, n, x)
+                        })(t, n, d, l, u),
                         isEnabled: () => e.serviceManager.terminals.isAvailable()
                     }), i.addFactory("FileBrowser", "gitClone", (() => S.ReactWidget.create(f().createElement(S.UseSignal, {
-                        signal: n.repositoryChanged,
+                        signal: a.repositoryChanged,
                         initialArgs: {
                             name: "pathRepository",
                             oldValue: null,
-                            newValue: n.pathRepository
+                            newValue: a.pathRepository
                         }
-                    }, ((t, a) => f().createElement(S.ToolbarButtonComponent, {
-                        enabled: null === (null == a ? void 0 : a.newValue),
+                    }, ((t, n) => f().createElement(S.ToolbarButtonComponent, {
+                        enabled: null === (null == n ? void 0 : n.newValue),
                         icon: Le.W6,
                         onClick: () => {
                             e.commands.execute(Ue.TQ.gitClone)
                         },
                         tooltip: p.__("Git Clone")
-                    })))))), (0, ze.ZM)(n, a, e.serviceManager.contents, e.contextMenu, p), u.info({
+                    })))))), (0, ze.ZM)(a, n, e.serviceManager.contents, e.contextMenu, p), u.info({
                         Message: "Successfully loaded Git extension"
                     })
                 }
             }, Ve = e => {
-                var t, a;
-                const n = `${e}.AWSSageMakerUI`;
-                return performance.mark(n), performance.measure(n, void 0, n), null !== (a = null === (t = performance.getEntriesByName(n, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== a ? a : 0
+                var t, n;
+                const a = `${e}.AWSSageMakerUI`;
+                return performance.mark(a), performance.measure(a, void 0, a), null !== (n = null === (t = performance.getEntriesByName(a, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== n ? n : 0
             }, Ze = {
                 id: i,
                 requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: (e, t) => {
                     ((e, t) => {
-                        const a = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
-                        let n = {};
-                        Array.isArray(a) && a.length > 0 && a.forEach((e => {
+                        const n = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
+                        let a = {};
+                        Array.isArray(n) && n.length > 0 && n.forEach((e => {
                             const {
                                 duration: t,
-                                requestStart: a,
+                                requestStart: n,
                                 responseStart: s,
                                 startTime: i
                             } = e;
-                            a && t && (n = {
-                                ...n,
+                            n && t && (a = {
+                                ...a,
                                 TimeToFirstByteMS: Math.round(s - i)
                             })
                         }));
                         let s = null,
                             i = null,
                             o = null,
                             r = null,
                             l = null;
                         const c = performance.getEntriesByType("navigation")[0];
                         if (c) s = c.redirectCount, i = c.redirectEnd - c.redirectStart, o = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
                         else {
                             const e = performance.timing;
                             s = performance.navigation.redirectCount, i = e.redirectEnd - e.redirectStart, o = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
                         }
-                        n = {
-                            ...n,
+                        a = {
+                            ...a,
                             RedirectCount: s,
                             RedirectTimeMS: i,
                             TimeToDOMContentLoadedMS: o,
                             TimeToFirstByteMS: r,
                             TimeToOnLoadMS: l
-                        }, e.info(n), t.started.then((() => {
+                        }, e.info(a), t.started.then((() => {
                             e.info({
                                 TimeToAppStartedMS: Math.round(Ve("timeToAppStarted"))
                             })
                         })), t.restored.then((() => {
-                            const t = (a = Math.round(Ve("timeToAppRestored"))) > 0 ? a : null;
-                            var a;
+                            const t = (n = Math.round(Ve("timeToAppRestored"))) > 0 ? n : null;
+                            var n;
                             e.info({
                                 TimeToAppRestoredMS: t || void 0
                             })
                         }))
                     })(De(t, i, Ae.logSchemas.performance), e)
                 }
             };
-            var We = a(87),
-                He = a(8201);
+            var We = n(87),
+                He = n(8201);
             const qe = {
                     SpaceMenuHeader: V.css`
   margin: -6px 0;
   padding: 0 var(--jp-size-2);
   height: 10;
   border-radius: var(--jp-radius-small);
   font-size: var(--jp-size-3);
@@ -987,30 +988,30 @@
 
   & > svg {
     padding: 0 var(--jp-size-2);
   }
 `
                 },
                 {
-                    privateSpaceHeader: Je,
+                    unknownSpace: Je,
                     unknownUser: Ye
                 } = m.Space,
                 Qe = ({
                     spaceName: e
                 }) => {
                     const t = !!e,
-                        a = R("studioUserProfileName");
+                        n = R("studioUserProfileName");
                     return f().createElement("div", {
                         className: qe.SpaceMenuHeader,
                         "data-testid": y
                     }, t ? f().createElement(We.Z, {
                         fontSize: "small"
                     }) : f().createElement(He.Z, {
                         fontSize: "small"
-                    }), f().createElement("p", null, `${a||Ye} / ${t?e:Je}`))
+                    }), f().createElement("p", null, `${n&&n[1]||Ye} / ${t?e:Je}`))
                 };
             class Ke extends S.ReactWidget {
                 constructor() {
                     super(), this.getSpaceName = async () => {
                         await F("aws/sagemaker/api/context", $.GET).then((e => {
                             e && e.json().then((e => {
                                 this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
@@ -1025,48 +1026,48 @@
                 }
             }
             const Xe = [v, L, de, Fe, Ze, {
                 id: o,
                 requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const a = new Ke;
-                    a.id = S.DOMUtils.createDomID();
-                    const n = De(t, o);
-                    e.shell.add(a, "top", {
+                    const n = new Ke;
+                    n.id = S.DOMUtils.createDomID();
+                    const a = De(t, o);
+                    e.shell.add(n, "top", {
                         rank: 1e3
                     }), window && window.panorama && window.panorama("trackCustomEvent", {
                         eventType: "render",
                         eventDetail: "Space-Plugin",
                         eventContext: "JupyterLab",
                         timestamp: Date.now()
-                    }), n.info({
+                    }), a.info({
                         Message: "Successfully loaded Space plugin"
                     })
                 }
             }]
         },
-        8201: (e, t, a) => {
-            var n = a(5318);
+        8201: (e, t, n) => {
+            var a = n(5318);
             t.Z = void 0;
-            var s = n(a(4938)),
-                i = a(5893),
+            var s = a(n(4938)),
+                i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 4c1.93 0 3.5 1.57 3.5 3.5S13.93 13 12 13s-3.5-1.57-3.5-3.5S10.07 6 12 6zm0 14c-2.03 0-4.43-.82-6.14-2.88C7.55 15.8 9.68 15 12 15s4.45.8 6.14 2.12C16.43 19.18 14.03 20 12 20z"
                 }), "AccountCircle");
             t.Z = o
         },
-        87: (e, t, a) => {
-            var n = a(5318);
+        87: (e, t, n) => {
+            var a = n(5318);
             t.Z = void 0;
-            var s = n(a(4938)),
-                i = a(5893),
+            var s = a(n(4938)),
+                i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
                 }), "Language");
             t.Z = o
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.1","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.c508feab9dfdf7494214.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -6188,15 +6188,15 @@
                     })
                 }));
             var Ns = o(8543),
                 Bs = o(5827),
                 js = o(76),
                 zs = o(6727),
                 Os = o(8441),
-                Ds = o(7651),
+                Ds = o(8962),
                 Es = o(9674);
 
             function Fs(e) {
                 return (0, Je.Z)("MuiLink", e)
             }
             const Ws = (0, Ke.Z)("MuiLink", ["root", "underlineNone", "underlineHover", "underlineAlways", "button", "focusVisible"]);
             var Us = o(4844);
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.7f061638d47075ac76be.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.26c15aab8d5d7301c11a.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -5740,15 +5740,15 @@
                             return l(arguments, "callee").get
                         } catch (e) {
                             return c
                         }
                     }
                 }() : c,
                 d = i(1405)(),
-                u = i(8185)(),
+                u = i(3276)(),
                 f = Object.getPrototypeOf || (u ? function(e) {
                     return e.__proto__
                 } : null),
                 p = {},
                 g = "undefined" != typeof Uint8Array && f ? f(Uint8Array) : n,
                 m = {
                     "%AggregateError%": "undefined" == typeof AggregateError ? n : AggregateError,
@@ -5985,15 +5985,15 @@
                         value: 1
                     }).length
                 } catch (e) {
                     return !0
                 }
             }, e.exports = s
         },
-        8185: e => {
+        3276: e => {
             "use strict";
             var t = {
                     foo: {}
                 },
                 i = Object;
             e.exports = function() {
                 return {
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.27a0e3dfb32431afe940.js` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.7282f69f1fc0d8e37b1c.js`

 * *Files 4% similar despite different names*

##### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
-            1514: (e, r, t) => {
+            3570: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -48,58 +48,58 @@
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "2135a6297693b09662d9",
+        181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "5350b743f9a235d9e265",
+        548: "a6ac1d0d39311897c48d",
         571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "c508feab9dfdf7494214",
+        799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "7f061638d47075ac76be",
+        823: "26c15aab8d5d7301c11a",
         853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
         891: "4794a088a65e99550778"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "2135a6297693b09662d9",
+        181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "5350b743f9a235d9e265",
+        548: "a6ac1d0d39311897c48d",
         571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "c508feab9dfdf7494214",
+        799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "7f061638d47075ac76be",
+        823: "26c15aab8d5d7301c11a",
         853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
         891: "4794a088a65e99550778"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.1", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(1514);
+    var E = S(3570);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json` & `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.dist-info/LICENSE` & `sagemaker_jupyterlab_extension-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.dist-info/METADATA` & `sagemaker_jupyterlab_extension-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.3.0
+Version: 0.3.1
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.0.dist-info/RECORD` & `sagemaker_jupyterlab_extension-0.3.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 sagemaker_jupyterlab_extension/__init__.py,sha256=hxDcPQ4HLDyOST0TL-Lu5fvzhEwrIgSkZLybVPPEkgk,1133
 sagemaker_jupyterlab_extension/_version.py,sha256=H8LOQyA3X6Xj3pixozSSsatne-Jd9sIhfgCIwlM6AGg,683
 sagemaker_jupyterlab_extension/handlers.py,sha256=j2uNNvU6Vu2guPRev4OEuyKtc_YkOJfAql3exvdn1nw,11587
-sagemaker_jupyterlab_extension/labextension/package.json,sha256=vNBJJjg0D1EZFYUpr5nhKC-qF876ZBk3JTiFLal9Q2Q,4091
+sagemaker_jupyterlab_extension/labextension/package.json,sha256=MJlCTqCdvftbBuXD6FnQG7gwbiFt7MxiShrRbgGUhl8,4091
 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
-sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js,sha256=ITWmKXaTsJZi2RNSG_PhVswJsCWBUWbBG0NIspc16uY,92715
+sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js,sha256=mgzfpBTly6OUfBmlVxrxcB1y7VZM780VsUDayhCRzJU,92715
 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
-sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js,sha256=U1C3Q_miNdniZQpaU-SBDzhd4-P6ZkDu9G0foZd9rbU,28094
+sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js,sha256=pqwdDTkxGJfEjX8rz1Mva5X-RXr5FGeFs98FHE2UxHg,28123
 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
-sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js,sha256=xQj-q53990lCFADTVbj3XegiS7kmYg8nAZtBnh79AG4,237708
-sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js,sha256=fwYWONRwdax2vgvW-p1L_6Sxs96H0fuY5f-tv22OsFs,266482
+sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js,sha256=6T0wmiNHtya0yRj7fFMvBT3z5B7M8kUQoFSgnIyQAJc,237708
+sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js,sha256=JsFaq41dcwHBGlJbsMA6G_eWnb33uUncDPP8e8qUf5I,266482
 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js,sha256=5iQSQgHaR-F5tI50GUTo-KOV1q9-eYprmtQw962uIOg,139405
 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
-sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js,sha256=J6Dj37MkMa_pQGmyuP4D6AwYwfeTQf73i5AJieQzCl4,12105
+sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js,sha256=coL2nx_A2ON7HHT_xMFMCti2yk2w5G6rylX5P6EipG4,12105
 sagemaker_jupyterlab_extension/labextension/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
 sagemaker_jupyterlab_extension/tests/__init__.py,sha256=LJe9lg48SCXTjTOe_oc0_Zj9blApYphXi-12E_3fh2s,60
 sagemaker_jupyterlab_extension/tests/helper.py,sha256=bH3LEHznHOzkfOfBmRn-S8hh5sUuRHj_EmjvjUdQ4uc,405
 sagemaker_jupyterlab_extension/tests/test_error_util.py,sha256=QBhspnhVQzw_a8yUVlfhxalT8ywS3sntb_diFK4nvDw,1647
 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py,sha256=O-QWKCetqSPCpzhBlFqS4zO1dp9_nJdGGpE_mqor2BU,5332
 sagemaker_jupyterlab_extension/tests/test_handlers.py,sha256=6BOEKL3v87psZtcqVbqlHjfRzyiBFZfFcUbig-ELCB8,5041
-sagemaker_jupyterlab_extension/tests/test_request_logger.py,sha256=y9sHb49HgUQDBLLQLwmSa-Cz1CwXnW2mu7qHvZUR4qE,7701
+sagemaker_jupyterlab_extension/tests/test_request_logger.py,sha256=MLvH7Ncrj34HdS9wkNZNAd_UDBDWKpBzpnNRPxNQqzc,7701
 sagemaker_jupyterlab_extension/utils/__init__.py,sha256=r4W_GQMVXe3D90bLPU9hZUehj0U1AhbN1qDE9M5vI6Y,64
 sagemaker_jupyterlab_extension/utils/error_util.py,sha256=fT6BDMGeHK9J70A8vyGkl_ygL662XQ5incmoq8X_R1Y,555
 sagemaker_jupyterlab_extension/utils/git_clone_util.py,sha256=pHExYjlSniCLZ-Q78OjrfIvsPPz2Cd13jB7F9Jiiu-s,2552
 sagemaker_jupyterlab_extension/utils/metric_util.py,sha256=h2w-vEFVpJkSSOA97gr5hpG6ROe6xgfYbK_VaaBItvg,507
 sagemaker_jupyterlab_extension/utils/request_logger.py,sha256=SNq6_gng-ElaUDl_akXmcFRYy9gFlydcRwWRZphNFs4,7250
-sagemaker_jupyterlab_extension-0.3.0.data/data/THIRD-PARTY-LICENSES,sha256=lL9OuaJ1ullVxluRJKKFT6xqWiCV3COZsSBBQHmFD6U,8139
-sagemaker_jupyterlab_extension-0.3.0.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json,sha256=U-i2pBYj1meFIyYC2auwNjK24HQIzgGCAcZZPtqjJZQ,105
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json,sha256=Y5TsP4lidrq-9l8YzVJvdwPbOXcVvHbehOFJov8eM_A,221
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json,sha256=vNBJJjg0D1EZFYUpr5nhKC-qF876ZBk3JTiFLal9Q2Q,4091
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.2135a6297693b09662d9.js,sha256=ITWmKXaTsJZi2RNSG_PhVswJsCWBUWbBG0NIspc16uY,92715
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.5350b743f9a235d9e265.js,sha256=U1C3Q_miNdniZQpaU-SBDzhd4-P6ZkDu9G0foZd9rbU,28094
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.c508feab9dfdf7494214.js,sha256=xQj-q53990lCFADTVbj3XegiS7kmYg8nAZtBnh79AG4,237708
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.7f061638d47075ac76be.js,sha256=fwYWONRwdax2vgvW-p1L_6Sxs96H0fuY5f-tv22OsFs,266482
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js,sha256=5iQSQgHaR-F5tI50GUTo-KOV1q9-eYprmtQw962uIOg,139405
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.27a0e3dfb32431afe940.js,sha256=J6Dj37MkMa_pQGmyuP4D6AwYwfeTQf73i5AJieQzCl4,12105
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
-sagemaker_jupyterlab_extension-0.3.0.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
-sagemaker_jupyterlab_extension-0.3.0.dist-info/LICENSE,sha256=ZWQ-fVLy0k5hdDLaputxwZyEfnfpvEx3ZImaRiZyuTA,4755
-sagemaker_jupyterlab_extension-0.3.0.dist-info/METADATA,sha256=bhG-_zyCuCnM3Bevz3uvAefQ3kyqYXCiyZLjLZE-jZc,2281
-sagemaker_jupyterlab_extension-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-sagemaker_jupyterlab_extension-0.3.0.dist-info/top_level.txt,sha256=96mz5zVRnlKUFu46rV4QFpibtf4h9CD5HVkLxPBcah8,31
-sagemaker_jupyterlab_extension-0.3.0.dist-info/RECORD,,
+sagemaker_jupyterlab_extension-0.3.1.data/data/THIRD-PARTY-LICENSES,sha256=lL9OuaJ1ullVxluRJKKFT6xqWiCV3COZsSBBQHmFD6U,8139
+sagemaker_jupyterlab_extension-0.3.1.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json,sha256=U-i2pBYj1meFIyYC2auwNjK24HQIzgGCAcZZPtqjJZQ,105
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json,sha256=Y5TsP4lidrq-9l8YzVJvdwPbOXcVvHbehOFJov8eM_A,221
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json,sha256=MJlCTqCdvftbBuXD6FnQG7gwbiFt7MxiShrRbgGUhl8,4091
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js,sha256=mgzfpBTly6OUfBmlVxrxcB1y7VZM780VsUDayhCRzJU,92715
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.a6ac1d0d39311897c48d.js,sha256=pqwdDTkxGJfEjX8rz1Mva5X-RXr5FGeFs98FHE2UxHg,28123
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js,sha256=6T0wmiNHtya0yRj7fFMvBT3z5B7M8kUQoFSgnIyQAJc,237708
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.26c15aab8d5d7301c11a.js,sha256=JsFaq41dcwHBGlJbsMA6G_eWnb33uUncDPP8e8qUf5I,266482
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js,sha256=5iQSQgHaR-F5tI50GUTo-KOV1q9-eYprmtQw962uIOg,139405
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.7282f69f1fc0d8e37b1c.js,sha256=coL2nx_A2ON7HHT_xMFMCti2yk2w5G6rylX5P6EipG4,12105
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
+sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
+sagemaker_jupyterlab_extension-0.3.1.dist-info/LICENSE,sha256=ZWQ-fVLy0k5hdDLaputxwZyEfnfpvEx3ZImaRiZyuTA,4755
+sagemaker_jupyterlab_extension-0.3.1.dist-info/METADATA,sha256=wMFygsrQaYHwrrG8vq2NB_IUVAieHGuS0NV7gqQ4oBc,2281
+sagemaker_jupyterlab_extension-0.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+sagemaker_jupyterlab_extension-0.3.1.dist-info/top_level.txt,sha256=96mz5zVRnlKUFu46rV4QFpibtf4h9CD5HVkLxPBcah8,31
+sagemaker_jupyterlab_extension-0.3.1.dist-info/RECORD,,
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/__init__.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/_version.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/_version.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/handlers.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/package.json` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9661111111111111%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7282f69f1fc0d8e37b1c.js'}}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -60,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.27a0e3dfb32431afe940.js",
+            "load": "static/remoteEntry.7282f69f1fc0d8e37b1c.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -105,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2749,15 +2749,15 @@
                 l = o(4780),
                 s = o(917),
                 d = o(1796),
                 c = o(8216),
                 p = o(2734),
                 u = o(948),
                 m = o(1657),
-                f = o(7651),
+                f = o(8962),
                 h = o(5893);
             const b = ["className", "color", "value", "valueBuffer", "variant"];
             let v, g, Z, x, y, S, C = e => e;
             const P = (0, s.F4)(v || (v = C`
   0% {
     left: -35%;
     right: 100%;
@@ -3002,15 +3002,15 @@
                             className: x.bar2,
                             ownerState: Z,
                             style: C.bar2
                         })]
                     }))
                 }))
         },
-        7651: (e, t, o) => {
+        8962: (e, t, o) => {
             o.d(t, {
                 E: () => a,
                 Z: () => i
             });
             var r = o(1588),
                 n = o(4867);
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [548], {
-        4548: (e, t, a) => {
-            a.r(t), a.d(t, {
+        4548: (e, t, n) => {
+            n.r(t), n.d(t, {
                 default: () => Xe
             });
-            var n = a(9557);
+            var a = n(9557);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
                 i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
                 o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
                 r = {
                     shutdown: "filemenu:shutdown"
                 },
                 l = "Sso",
@@ -75,34 +75,35 @@
                             failedOptionsBody: "Something went wrong when trying to open README file within the repo.",
                             invalidCloneUrlTitle: "Invalid URL provided",
                             invalidCloneUrlBody: "The URL provided is not valid. Please input a valid URL to clone."
                         }
                     },
                     Space: {
                         privateSpaceHeader: "Personal Studio",
-                        unknownUser: "Unknown User"
+                        unknownUser: "Unknown User",
+                        unknownSpace: "Unknown Space"
                     }
                 },
                 g = "GitCloneDialogError",
                 h = "ValidRepoPathError",
                 y = "spaceMenuHeader",
                 v = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:hideshutdown",
-                    requires: [n.IMainMenu],
+                    requires: [a.IMainMenu],
                     autoStart: !0,
                     activate: (e, t) => {
                         e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
-            var w = a(9801),
-                b = a.n(w),
-                E = a(6029),
-                f = a.n(E),
-                x = a(8368),
-                S = a(9510);
+            var w = n(9801),
+                b = n.n(w),
+                E = n(6029),
+                f = n.n(E),
+                x = n(8368),
+                S = n(9510);
             class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
@@ -117,162 +118,162 @@
                 R = e => document.cookie.match("\\b" + e + '="?([^;]*)"?\\b'),
                 T = () => {
                     const e = R("expiryTime"),
                         t = R("ssoExpiryTimestamp");
                     return M() && t ? Number(t[1]) : e ? Number(e[1]) : null
                 },
                 j = (e, t) => {
-                    var a, n;
-                    t ? null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.disconnect(x.ConnectionLost) : null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.connect(x.ConnectionLost)
+                    var n, a;
+                    t ? null === (n = e.serviceManager) || void 0 === n || n.connectionFailure.disconnect(x.ConnectionLost) : null === (a = e.serviceManager) || void 0 === a || a.connectionFailure.connect(x.ConnectionLost)
                 },
                 k = () => {
                     const e = R("redirectURL");
                     let t;
                     try {
                         if (t = new URL(e ? e[1] : void 0), "http:" === t.protocol || "https:" === t.protocol) return t.toString()
                     } catch (e) {
                         return
                     }
                 },
                 D = (e, t) => {
-                    const a = T(),
-                        n = window.open(e, "signin window", "width=800, height=600");
+                    const n = T(),
+                        a = window.open(e, "signin window", "width=800, height=600");
                     let s = !1;
                     const i = window.setInterval((() => {
-                        if (n && n.closed && !s) return void window.clearInterval(i);
+                        if (a && a.closed && !s) return void window.clearInterval(i);
                         const e = T();
-                        if (null !== e && null !== a && (e > a || isNaN(e))) {
-                            window.clearInterval(i), n && n.close(), s = !0;
+                        if (null !== e && null !== n && (e > n || isNaN(e))) {
+                            window.clearInterval(i), a && a.close(), s = !0;
                             for (const e of t) e.kernel.reconnect();
                             S.Dialog.tracker.forEach((e => e.reject()))
                         }
                     }), u)
                 },
                 _ = async () => {
                     const {
                         SignInSession: e
                     } = m, {
                         signinDialog: t
-                    } = e, a = k(), n = a ? [S.Dialog.okButton({
+                    } = e, n = k(), a = n ? [S.Dialog.okButton({
                         label: e.signInButton
                     })] : [S.Dialog.cancelButton({
                         label: e.closeButton
-                    })], s = a ? f().createElement("div", {
+                    })], s = n ? f().createElement("div", {
                         "data-testid": "session-signin-log-out"
                     }, t.loggedOutBody) : f().createElement("div", {
                         "data-testid": "session-signin-restart"
                     }, t.restartSessionBody), i = new S.Dialog({
                         title: t.title,
                         body: s,
-                        buttons: n,
+                        buttons: a,
                         hasClose: !1
                     });
                     return {
                         sigInDialogResult: await i.launch(),
                         confirmDialog: i
                     }
                 };
-            var N = a(6797),
-                B = a(6697),
-                I = a(1638),
-                z = a(7217),
-                A = a(5326);
-            const U = (e, t, a, n, s, i, o) => {
+            var N = n(6797),
+                B = n(6697),
+                I = n(1638),
+                z = n(7217),
+                A = n(5326);
+            const U = (e, t, n, a, s, i, o) => {
                     const r = T(),
                         l = o(),
                         d = l && l + c;
                     if (null === r) j(e, !1);
                     else {
                         const o = b().unix(r / 1e3).diff(b()()),
                             u = Date.now();
-                        ((e, t, a) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(a, e))(M(), r, o) ? (n(), (async (e, t, a) => {
+                        ((e, t, n) => ((e, t) => -1 === e && t)(t, e) || ((e, t) => e <= 0 && !t)(n, e))(M(), r, o) ? (a(), (async (e, t, n) => {
                             const {
-                                SignInSession: n
+                                SignInSession: a
                             } = m, s = k();
                             S.Dialog.tracker.forEach((e => e.reject())), j(e, !0);
                             const {
                                 sigInDialogResult: i,
                                 confirmDialog: o
                             } = await _();
                             if (i && i.button)
-                                if (a(), s) D(k(), t);
-                                else if (i && i.button.label === n.closeButton) {
+                                if (n(), s) D(k(), t);
+                                else if (i && i.button.label === a.closeButton) {
                                 const e = T(),
                                     t = e && e / 1e3,
-                                    a = t && b().unix(t).diff(b()());
-                                null !== a && a && a > c && (o.dispose(), setTimeout((async () => {
+                                    n = t && b().unix(t).diff(b()());
+                                null !== n && n && n > c && (o.dispose(), setTimeout((async () => {
                                     await _()
                                 }), c))
                             } else o.dispose(), D(k(), t)
-                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (n(), (async (e, t, a, n, s) => {
+                        })(e, t, s)) : o <= 9e5 && (void 0 === l || d && u > d) ? (a(), (async (e, t, n, a, s) => {
                             const {
                                 SignInSession: i
                             } = m, {
                                 renewSessionDialog: o
                             } = m.SignInSession, {
                                 renewSessionDialogResult: r,
                                 confirmDialog: l
                             } = await (async () => {
                                 const {
                                     SignInSession: e
                                 } = m, {
                                     renewSessionDialog: t
-                                } = m.SignInSession, a = k(), n = T(), s = n && b().unix(n / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
+                                } = m.SignInSession, n = k(), a = T(), s = a && b().unix(a / 1e3).fromNow(), i = `${t.contDownTimerMessage}${s}.`, o = `${M()?t.soonExpiringSessionBody:i}`, r = t.renewSessionBody, l = M() ? f().createElement(f().Fragment, null, f().createElement("div", {
                                     "data-testid": "session-renew-lose-unsaved-changes"
                                 }, o, " ", t.loseUnsavedChanges, " ", t.saveAllChanges), f().createElement("div", null, r)) : f().createElement("div", {
                                     "data-testid": "session-renew-now"
                                 }, f().createElement("p", null, o), f().createElement("p", null, t.renewSessionNow)), c = [S.Dialog.okButton({
                                     label: t.remindText
-                                }), a && S.Dialog.okButton({
+                                }), n && S.Dialog.okButton({
                                     label: e.saveAndRenewButton
                                 })], d = new S.Dialog({
                                     title: t.title,
                                     body: l,
                                     buttons: c,
                                     hasClose: !1
                                 });
                                 return {
                                     renewSessionDialogResult: await d.launch(),
                                     confirmDialog: d
                                 }
                             })();
                             if (r && r.button.label === o.remindText) {
                                 const e = new C;
-                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), n()
-                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), a(), n(), M() || D(k(), t))
-                        })(0, t._sessions, a, s, i), j(e, !1)) : j(e, !1)
+                                0 === e._count ? (e.setDismissTime(Date.now()), s(e._dismissTime)) : e.getDismissTime(), l.dispose(), a()
+                            } else r && r.button.label === i.saveAndRenewButton && (l.dispose(), n(), a(), M() || D(k(), t))
+                        })(0, t._sessions, n, s, i), j(e, !1)) : j(e, !1)
                     }
                 },
                 L = {
                     id: "@amzn/sagemaker-jupyterlab-extensions:sessionmanagement",
                     requires: [],
                     autoStart: !0,
                     activate: async e => {
                         let t;
-                        const a = e.serviceManager.sessions,
-                            n = () => {
+                        const n = e.serviceManager.sessions,
+                            a = () => {
                                 s.start()
                             },
-                            s = ((e, t, a, n, s, i, o) => new N.Poll({
+                            s = ((e, t, n, a, s, i, o) => new N.Poll({
                                 auto: !0,
-                                factory: async () => U(e, t, a, n, s, i, o),
+                                factory: async () => U(e, t, n, a, s, i, o),
                                 frequency: {
                                     interval: d,
                                     backoff: !0,
                                     max: p
                                 }
-                            }))(e, a, (() => {
+                            }))(e, n, (() => {
                                 const t = new I.TextModelFactory,
-                                    a = new I.DocumentRegistry({
+                                    n = new I.DocumentRegistry({
                                         textModelFactory: t
                                     }),
-                                    n = new z.ServiceManager({}),
+                                    a = new z.ServiceManager({}),
                                     s = new A.DocumentManager({
-                                        registry: a,
-                                        manager: n,
+                                        registry: n,
+                                        manager: a,
                                         opener: {
                                             open: e => {},
                                             get opened() {
                                                 return {
                                                     connect: () => !1,
                                                     disconnect: () => !1
                                                 }
@@ -283,40 +284,40 @@
                                     const t = s.contextForWidget(e);
                                     void 0 !== t && t.save().then((() => t.createCheckpoint())).catch((e => {
                                         if ("Cancel" !== e.message) throw e
                                     }))
                                 }))
                             }), (() => {
                                 s.stop()
-                            }), n, (e => {
+                            }), a, (e => {
                                 t = e
                             }), (() => t));
-                        n()
+                        a()
                     }
                 };
-            var P = a(4613);
+            var P = n(4613);
             const G = [200, 201];
-            var $, O = a(6311);
+            var $, O = n(6311);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
             }($ || ($ = {}));
             const F = async (e, t) => {
-                const a = z.ServerConnection.makeSettings(),
-                    n = O.URLExt.join(a.baseUrl, e);
+                const n = z.ServerConnection.makeSettings(),
+                    a = O.URLExt.join(n.baseUrl, e);
                 try {
-                    const e = await z.ServerConnection.makeRequest(n, {
+                    const e = await z.ServerConnection.makeRequest(a, {
                         method: t
-                    }, a);
+                    }, n);
                     if (!G.includes(e.status)) throw new Error("Unable to fetch data");
                     return e
                 } catch (e) {
                     throw Error(e)
                 }
             };
-            var V = a(5933);
+            var V = n(5933);
             const Z = "8px",
                 W = "12px",
                 H = V.css`
   border-bottom: solid 1px var(--sm-border-color2);
 `,
                 q = V.css`
   background-color: var(--jp-layout-color2);
@@ -363,59 +364,59 @@
 `,
                 te = V.css`
   border-radius: 10px;
   width: 40px;
   margin: 0 0 2px 4px;
   height: 6px !important;
 `,
-                ae = (V.css`
+                ne = (V.css`
   border-radius: 10px;
   display: inline-block;
   width: 40px;
   height: 8px;
 `, V.css`
   display: flex;
   align-items: center;
 `);
-            var ne = a(8441);
+            var ae = n(8441);
             const se = ({
                     value: e,
                     singleProgressBarStyle: t,
-                    displayValue: a,
-                    label: n,
+                    displayValue: n,
+                    label: a,
                     labelClassName: s,
                     conatinerClassName: i
                 }) => f().createElement("div", {
                     role: "container",
                     "data-testid": "linear-progress-bar-container"
                 }, f().createElement("div", {
                     className: i
-                }, n && f().createElement("span", {
+                }, a && f().createElement("span", {
                     className: s
-                }, n, " ", a, "%"), f().createElement(ne.Z, {
+                }, a, " ", n, "%"), f().createElement(ae.Z, {
                     "data-testid": "linear-progress-bar",
                     className: t,
                     variant: "determinate",
                     value: e
                 }))),
                 ie = "jlStudio-",
                 oe = `${ie}ResourceUsageWidgetContainer`,
                 re = `${ie}MetricsWidgetContainer`,
                 le = ({
                     onClickHandler: e,
                     instanceMetricsResponse: t,
-                    instanceMetricsDisplayValue: a
+                    instanceMetricsDisplayValue: n
                 }) => {
-                    const [n, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
+                    const [a, s] = (0, E.useState)(!1), [i, o] = (0, E.useState)(0), [r, l] = (0, E.useState)(0), [c, d] = (0, E.useState)(0), [u, p] = (0, E.useState)(!1), g = e => e && void 0 !== e ? Math.round(e) : 0, h = e => 0 === e ? "0.0" : e && void 0 !== e ? e.toFixed(2).toString() : "--";
                     (0, E.useEffect)((() => {
                         if (void 0 !== t && (null == t ? void 0 : t.metrics)) {
                             const {
                                 metrics: e
-                            } = t, a = e.cpu.cpu_percentage, n = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
-                            o(a), l(n), d(r)
+                            } = t, n = e.cpu.cpu_percentage, a = e.memory.memory_percentage, s = e.storage.used_space_in_bytes, i = e.storage.total_space_in_bytes, r = s && i && s / i * 100;
+                            o(n), l(a), d(r)
                         }
                     }), [t]), (0, E.useEffect)((() => {
                         if (c && c > 95 && !1 === u) {
                             const {
                                 stoargeSpaceLimitDialog: e
                             } = m.ResourceUsage;
                             S.Notification.info(e.title), p(!0)
@@ -430,32 +431,32 @@
                     } = m.ResourceUsage;
                     return f().createElement("div", {
                         "data-testid": "resource-usage-widget",
                         "data-analytics-type": "eventContext",
                         "data-analytics": "JupyterLab",
                         className: `${oe} ${K}`
                     }, f().createElement("div", {
-                        className: ae,
+                        className: ne,
                         onClick: () => (t => {
                             s(!t), e()
-                        })(n),
+                        })(a),
                         "data-testid": "resource-usage-widget-click-handler",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "ResourceUsage-Widget-Click"
-                    }, y, " ", void 0 === a ? f().createElement(ne.Z, {
+                    }, y, " ", void 0 === n ? f().createElement(ae.Z, {
                         "data-testid": "resource-usage-linear-progress-spinner",
                         className: te
                     }) : f().createElement("div", {
-                        className: ae,
+                        className: ne,
                         "data-testid": "resource-usage-status-bar-container"
-                    }, f().createElement(ne.Z, {
+                    }, f().createElement(ae.Z, {
                         className: te,
                         variant: "determinate",
-                        value: 0 | a
-                    }), a ? Math.round(a) : 0, "%")), n && f().createElement("div", {
+                        value: 0 | n
+                    }), n ? Math.round(n) : 0, "%")), a && f().createElement("div", {
                         className: `${re} ${q}`,
                         "data-testid": "resource-usage-data-container"
                     }, f().createElement("div", {
                         className: H
                     }, f().createElement("div", {
                         className: Y
                     }, v), f().createElement("div", {
@@ -489,16 +490,16 @@
             class ce extends S.ReactWidget {
                 constructor() {
                     super(), this.clickHandler = () => {
                         this.update()
                     }, this.getInstanceMetrics = async () => {
                         await F("aws/sagemaker/api/instance/metrics", $.GET).then((e => {
                             e && e.json().then((e => {
-                                var t, a;
-                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (a = this._instanceMetricsResponse) || void 0 === a ? void 0 : a.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
+                                var t, n;
+                                this._instanceMetricsResponse = e || null, (null === (t = this._instanceMetricsResponse) || void 0 === t ? void 0 : t.metrics.memory) ? this._instanceMetricsDisplayValue = null === (n = this._instanceMetricsResponse) || void 0 === n ? void 0 : n.metrics.memory.memory_percentage : this._instanceMetricsDisplayValue = void 0
                             }))
                         })), this.update()
                     }, this._getInstanceMetricsLoop = setInterval(this.getInstanceMetrics, 5e3), this._instanceMetricsResponse = null, this._instanceMetricsDisplayValue = void 0
                 }
                 render() {
                     return f().createElement(le, {
                         onClickHandler: this.clickHandler,
@@ -508,49 +509,49 @@
                 }
             }
             const de = {
                 id: "@amzn/sagemaker-jupyterlab-extensions:resourceusage",
                 requires: [P.IStatusBar],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const a = new ce;
+                    const n = new ce;
                     t.registerStatusItem("@amzn/sagemaker-jupyterlab-extensions:resourceusage:resource-usage-widget", {
-                        item: a,
+                        item: n,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ue = a(8031),
-                pe = a(2715);
+            var ue = n(8031),
+                pe = n(2715);
             const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
                 ge = ({
                     label: e,
                     id: t,
-                    helperText: a,
-                    error: n,
+                    helperText: n,
+                    error: a,
                     handleChange: s,
                     regEx: i,
                     ...o
                 }) => {
                     const [r, l] = (0, E.useState)(""), [c, d] = (0, E.useState)(!0);
                     return f().createElement(pe.Z, {
                         variant: "standard",
                         className: me,
                         "data-testid": "text-field-container",
                         error: !c,
                         id: t,
                         label: e,
-                        helperText: a,
+                        helperText: n,
                         value: r,
                         onChange: e => (e => {
                             l(e.target.value);
                             const t = new RegExp(i);
                             d(t.test(e.target.value)), s(e.target.value)
                         })(e),
                         ...o
@@ -567,84 +568,84 @@
   .MuiFormControl-root.MuiTextField-root {
     margin-bottom: 20px;
   }
 `;
             V.css`
   margin-bottom: 20px;
 `;
-            var ve = a(3776);
+            var ve = n(3776);
             const we = (e = !1) => V.css`
   color: var(--jp-color-root-light-800);
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
   margin-bottom: var(--jp-ui-font-size1);
   ${e&&"\n    &:after {\n      content: '*';\n      color: var(--jp-error-color1);\n    }\n  "}
 `,
                 be = V.css`
   margin-top: 20px;
 `,
                 Ee = ({
                     options: e,
                     handleChange: t,
-                    label: a,
-                    freeSolo: n
+                    label: n,
+                    freeSolo: a
                 }) => {
-                    const s = (e, a) => {
-                        t(a)
+                    const s = (e, n) => {
+                        t(n)
                     };
                     return E.createElement("div", {
                         className: be
                     }, E.createElement("label", {
                         className: we(!0)
-                    }, a), E.createElement(ve.Z, {
+                    }, n), E.createElement(ve.Z, {
                         id: "autocomplete",
-                        freeSolo: n,
+                        freeSolo: a,
                         autoSelect: !0,
                         onChange: (e, t) => s(0, t),
                         onInputChange: (e, t) => s(0, t),
                         options: e.map((e => e.label)),
                         renderInput: e => E.createElement(pe.Z, {
                             ...e,
                             variant: "outlined",
                             size: "small",
                             margin: "dense"
                         })
                     }))
                 };
-            var fe = a(2671),
-                xe = a(847);
+            var fe = n(2671),
+                xe = n(847);
             const Se = ({
                     label: e,
                     id: t,
-                    handleChange: a,
-                    ...n
+                    handleChange: n,
+                    ...a
                 }) => {
                     const [s, i] = (0, E.useState)(!0);
                     return f().createElement(f().Fragment, null, f().createElement(xe.Z, {
                         control: f().createElement(fe.Z, {
                             "data-testid": "checkbox-field",
                             inputProps: {
                                 "aria-label": "controlled"
                             },
                             checked: s,
                             onChange: e => {
-                                i(e.target.checked), a(e.target.checked)
+                                i(e.target.checked), n(e.target.checked)
                             },
                             id: t,
-                            ...n
+                            ...a
                         }),
                         label: e
                     }))
                 },
                 Ce = ({
                     gitRepositories: e,
                     setGitURL: t,
-                    setPath: a,
-                    setOpenREADME: n
+                    setPath: n,
+                    setOpenREADME: a
                 }) => {
                     const [s, i] = (0, E.useState)(""), [o, r] = (0, E.useState)(""), [l, c] = (0, E.useState)(!0), [d, u] = (0, E.useState)([]), {
                         repoTitle: p,
                         pathTitle: g,
                         openReadMeFilesLabel: h
                     } = m.GitClone;
                     return (0, E.useEffect)((() => {
@@ -677,25 +678,25 @@
                         "data-analytics": "GitClone-Path-TextField",
                         error: !1,
                         id: "path",
                         label: g,
                         helperText: "",
                         valuePassed: s,
                         handleChange: e => {
-                            i(e), a(e)
+                            i(e), n(e)
                         },
                         regEx: "^([A-Za-z]*|[0-9]*|[/]*|[.]*|[A-Za-z0-9/.]*)$"
                     }), f().createElement(Se, {
                         "data-testid": "read-me-field",
                         "data-analytics-type": "eventDetail",
                         "data-analytics": "GitClone-OpenReadMeCheckbox",
                         label: h,
                         id: "openReadMe",
                         handleChange: e => {
-                            c(e), n(e)
+                            c(e), a(e)
                         },
                         checked: l
                     }))
                 };
             class Me extends S.ReactWidget {
                 constructor() {
                     super(), this.setGitURL = e => {
@@ -724,85 +725,85 @@
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Re = a(5962),
-                Te = a(2190);
+            var Re = n(5962),
+                Te = n(2190);
             const {
                 name: je,
                 version: ke
-            } = a(4147), De = (e, t, a) => e.child({
+            } = n(4147), De = (e, t, n) => e.child({
                 ExtensionName: je,
                 ExtensionVersion: ke,
                 PluginId: t
-            }, a);
+            }, n);
             var _e;
             ! function(e) {
                 e[e.CanClone = 0] = "CanClone", e[e.NotExist = 1] = "NotExist", e[e.AlreadyCloned = 2] = "AlreadyCloned"
             }(_e || (_e = {}));
             const Ne = [{
                     name: "README.ipynb",
                     factory: "Notebook"
                 }, {
                     name: "README.md",
                     factory: "Markdown Preview"
                 }],
-                Be = async (e, t, a) => {
+                Be = async (e, t, n) => {
                     const {
-                        repoPath: n,
+                        repoPath: a,
                         openREADME: s
-                    } = a;
+                    } = n;
                     if (await e.execute("filebrowser:go-to-path", {
-                            path: n
+                            path: a
                         }), !0 === s) try {
-                        await (async (e, t, a) => {
-                            const n = await t.get(e);
-                            if ("directory" === n.type) {
-                                const t = Ne.find((e => n.content.some((t => t.name === e.name))));
-                                t && await a.execute("docmanager:open", {
+                        await (async (e, t, n) => {
+                            const a = await t.get(e);
+                            if ("directory" === a.type) {
+                                const t = Ne.find((e => a.content.some((t => t.name === e.name))));
+                                t && await n.execute("docmanager:open", {
                                     path: O.PathExt.join(e, t.name),
                                     factory: t.factory
                                 })
                             }
-                        })(n, t, e)
+                        })(a, t, e)
                     } catch (e) {}
                 }, Ie = async (e, t) => {
-                    let a;
+                    let n;
                     try {
-                        a = await t.get(e)
+                        n = await t.get(e)
                     } catch (e) {
                         return !1
                     }
-                    return "directory" === a.type
+                    return "directory" === n.type
                 };
-            var ze = a(1775),
-                Ae = a(248),
-                Ue = a(4337),
-                Le = a(8625);
+            var ze = n(1775),
+                Ae = n(248),
+                Ue = n(4337),
+                Le = n(8625);
             const {
                 dialogTitle: Pe,
                 cancelButton: Ge,
                 cloneButton: $e,
                 errors: Oe
             } = m.GitClone, Fe = {
                 id: s,
                 requires: [ue.IFileBrowserFactory, ue.IDefaultFileBrowser, Te.IGitExtension, S.IToolbarWidgetRegistry, Ae.ILogger, Re.ITranslator],
                 autoStart: !0,
-                activate: async (e, t, a, n, i, o, r) => {
+                activate: async (e, t, n, a, i, o, r) => {
                     const {
                         commands: l,
                         serviceManager: c
                     } = e, d = c.contents, u = De(o, s), p = (r = r || Re.nullTranslator).load("sagemaker_studio");
                     l.addCommand(Ue.TQ.gitClone, {
                         label: "Git Clone Repo",
                         caption: "",
-                        execute: () => (async (e, t, a, n, s) => {
+                        execute: () => (async (e, t, n, a, s) => {
                             var i, o;
                             const r = t.model;
                             let l = "";
                             const c = null === (o = null === (i = null == e ? void 0 : e.tracker) || void 0 === i ? void 0 : i.currentWidget) || void 0 === o ? void 0 : o.model.path;
                             let d, u = null != c ? c : "",
                                 p = !0,
                                 y = !0;
@@ -839,139 +840,139 @@
                             const b = (e => {
                                     const t = O.URLExt.parse(e);
                                     return O.PathExt.basename(t.pathname, ".git")
                                 })(l),
                                 E = O.PathExt.join(u, b);
                             let f;
                             try {
-                                f = await (async (e, t, a, n) => {
+                                f = await (async (e, t, n, a) => {
                                     const {
                                         errors: s
                                     } = m.GitClone;
-                                    return await Ie(t, e) ? await Ie(n, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
-                                        message: s.localGitCloneExistBody + a
+                                    return await Ie(t, e) ? await Ie(a, e) ? (await (0, S.showErrorMessage)(s.localGitCloneExistTitle, {
+                                        message: s.localGitCloneExistBody + n
                                     }), _e.AlreadyCloned) : _e.CanClone : (await (0, S.showErrorMessage)(s.directoryNotExistTitle, {
                                         message: s.directoryNotExistBody + t
                                     }), _e.NotExist)
-                                })(a, u, l, E)
+                                })(n, u, l, E)
                             } catch (e) {
                                 s.error({
                                     Message: h,
                                     Error: new Error(JSON.stringify(e))
                                 })
                             }
                             const x = {
                                 repoPath: E,
                                 openREADME: p,
                                 findEnvironment: y
                             };
-                            f === _e.CanClone ? (async (e, t, a, n, s, i) => {
+                            f === _e.CanClone ? (async (e, t, n, a, s, i) => {
                                 const {
                                     errors: o
                                 } = m.GitClone, r = await e.execute("terminal:create-new");
                                 let l = "";
                                 s && (l += `cd ${s} && `), l += `git clone ${i} && exit\r`;
                                 try {
                                     const s = r.content;
                                     s.session.send({
                                         type: "stdin",
                                         content: [l]
-                                    }), s.session.connectionStatusChanged.connect((async n => {
-                                        if ("disconnected" === n.connectionStatus) try {
-                                            await Be(e, t, a)
+                                    }), s.session.connectionStatusChanged.connect((async a => {
+                                        if ("disconnected" === a.connectionStatus) try {
+                                            await Be(e, t, n)
                                         } catch (e) {
                                             await (0, S.showErrorMessage)(o.failedOptions, o.failedOptionsBody, [S.Dialog.warnButton({
                                                 label: "DISMISS"
                                             })])
                                         }
-                                    })), await n.refresh()
+                                    })), await a.refresh()
                                 } catch (e) {
                                     r.dispose(), await (0, S.showErrorMessage)(o.generalCloneErrorTitle, {
                                         message: o.generalCloneErrorBody + e
                                     })
                                 }
-                            })(n, a, x, r, u, l) : f === _e.AlreadyCloned && Be(n, a, x)
-                        })(t, a, d, l, u),
+                            })(a, n, x, r, u, l) : f === _e.AlreadyCloned && Be(a, n, x)
+                        })(t, n, d, l, u),
                         isEnabled: () => e.serviceManager.terminals.isAvailable()
                     }), i.addFactory("FileBrowser", "gitClone", (() => S.ReactWidget.create(f().createElement(S.UseSignal, {
-                        signal: n.repositoryChanged,
+                        signal: a.repositoryChanged,
                         initialArgs: {
                             name: "pathRepository",
                             oldValue: null,
-                            newValue: n.pathRepository
+                            newValue: a.pathRepository
                         }
-                    }, ((t, a) => f().createElement(S.ToolbarButtonComponent, {
-                        enabled: null === (null == a ? void 0 : a.newValue),
+                    }, ((t, n) => f().createElement(S.ToolbarButtonComponent, {
+                        enabled: null === (null == n ? void 0 : n.newValue),
                         icon: Le.W6,
                         onClick: () => {
                             e.commands.execute(Ue.TQ.gitClone)
                         },
                         tooltip: p.__("Git Clone")
-                    })))))), (0, ze.ZM)(n, a, e.serviceManager.contents, e.contextMenu, p), u.info({
+                    })))))), (0, ze.ZM)(a, n, e.serviceManager.contents, e.contextMenu, p), u.info({
                         Message: "Successfully loaded Git extension"
                     })
                 }
             }, Ve = e => {
-                var t, a;
-                const n = `${e}.AWSSageMakerUI`;
-                return performance.mark(n), performance.measure(n, void 0, n), null !== (a = null === (t = performance.getEntriesByName(n, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== a ? a : 0
+                var t, n;
+                const a = `${e}.AWSSageMakerUI`;
+                return performance.mark(a), performance.measure(a, void 0, a), null !== (n = null === (t = performance.getEntriesByName(a, "measure")[0]) || void 0 === t ? void 0 : t.duration) && void 0 !== n ? n : 0
             }, Ze = {
                 id: i,
                 requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: (e, t) => {
                     ((e, t) => {
-                        const a = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
-                        let n = {};
-                        Array.isArray(a) && a.length > 0 && a.forEach((e => {
+                        const n = null === window || void 0 === window ? void 0 : window.performance.getEntriesByType("resource");
+                        let a = {};
+                        Array.isArray(n) && n.length > 0 && n.forEach((e => {
                             const {
                                 duration: t,
-                                requestStart: a,
+                                requestStart: n,
                                 responseStart: s,
                                 startTime: i
                             } = e;
-                            a && t && (n = {
-                                ...n,
+                            n && t && (a = {
+                                ...a,
                                 TimeToFirstByteMS: Math.round(s - i)
                             })
                         }));
                         let s = null,
                             i = null,
                             o = null,
                             r = null,
                             l = null;
                         const c = performance.getEntriesByType("navigation")[0];
                         if (c) s = c.redirectCount, i = c.redirectEnd - c.redirectStart, o = Math.round(c.domContentLoadedEventEnd), r = Math.round(c.responseStart), l = Math.round(c.loadEventEnd);
                         else {
                             const e = performance.timing;
                             s = performance.navigation.redirectCount, i = e.redirectEnd - e.redirectStart, o = e.domContentLoadedEventEnd - e.navigationStart, r = e.responseStart - e.navigationStart, l = e.loadEventEnd - e.navigationStart
                         }
-                        n = {
-                            ...n,
+                        a = {
+                            ...a,
                             RedirectCount: s,
                             RedirectTimeMS: i,
                             TimeToDOMContentLoadedMS: o,
                             TimeToFirstByteMS: r,
                             TimeToOnLoadMS: l
-                        }, e.info(n), t.started.then((() => {
+                        }, e.info(a), t.started.then((() => {
                             e.info({
                                 TimeToAppStartedMS: Math.round(Ve("timeToAppStarted"))
                             })
                         })), t.restored.then((() => {
-                            const t = (a = Math.round(Ve("timeToAppRestored"))) > 0 ? a : null;
-                            var a;
+                            const t = (n = Math.round(Ve("timeToAppRestored"))) > 0 ? n : null;
+                            var n;
                             e.info({
                                 TimeToAppRestoredMS: t || void 0
                             })
                         }))
                     })(De(t, i, Ae.logSchemas.performance), e)
                 }
             };
-            var We = a(87),
-                He = a(8201);
+            var We = n(87),
+                He = n(8201);
             const qe = {
                     SpaceMenuHeader: V.css`
   margin: -6px 0;
   padding: 0 var(--jp-size-2);
   height: 10;
   border-radius: var(--jp-radius-small);
   font-size: var(--jp-size-3);
@@ -987,30 +988,30 @@
 
   & > svg {
     padding: 0 var(--jp-size-2);
   }
 `
                 },
                 {
-                    privateSpaceHeader: Je,
+                    unknownSpace: Je,
                     unknownUser: Ye
                 } = m.Space,
                 Qe = ({
                     spaceName: e
                 }) => {
                     const t = !!e,
-                        a = R("studioUserProfileName");
+                        n = R("studioUserProfileName");
                     return f().createElement("div", {
                         className: qe.SpaceMenuHeader,
                         "data-testid": y
                     }, t ? f().createElement(We.Z, {
                         fontSize: "small"
                     }) : f().createElement(He.Z, {
                         fontSize: "small"
-                    }), f().createElement("p", null, `${a||Ye} / ${t?e:Je}`))
+                    }), f().createElement("p", null, `${n&&n[1]||Ye} / ${t?e:Je}`))
                 };
             class Ke extends S.ReactWidget {
                 constructor() {
                     super(), this.getSpaceName = async () => {
                         await F("aws/sagemaker/api/context", $.GET).then((e => {
                             e && e.json().then((e => {
                                 this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
@@ -1025,48 +1026,48 @@
                 }
             }
             const Xe = [v, L, de, Fe, Ze, {
                 id: o,
                 requires: [Ae.ILogger],
                 autoStart: !0,
                 activate: async (e, t) => {
-                    const a = new Ke;
-                    a.id = S.DOMUtils.createDomID();
-                    const n = De(t, o);
-                    e.shell.add(a, "top", {
+                    const n = new Ke;
+                    n.id = S.DOMUtils.createDomID();
+                    const a = De(t, o);
+                    e.shell.add(n, "top", {
                         rank: 1e3
                     }), window && window.panorama && window.panorama("trackCustomEvent", {
                         eventType: "render",
                         eventDetail: "Space-Plugin",
                         eventContext: "JupyterLab",
                         timestamp: Date.now()
-                    }), n.info({
+                    }), a.info({
                         Message: "Successfully loaded Space plugin"
                     })
                 }
             }]
         },
-        8201: (e, t, a) => {
-            var n = a(5318);
+        8201: (e, t, n) => {
+            var a = n(5318);
             t.Z = void 0;
-            var s = n(a(4938)),
-                i = a(5893),
+            var s = a(n(4938)),
+                i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 4c1.93 0 3.5 1.57 3.5 3.5S13.93 13 12 13s-3.5-1.57-3.5-3.5S10.07 6 12 6zm0 14c-2.03 0-4.43-.82-6.14-2.88C7.55 15.8 9.68 15 12 15s4.45.8 6.14 2.12C16.43 19.18 14.03 20 12 20z"
                 }), "AccountCircle");
             t.Z = o
         },
-        87: (e, t, a) => {
-            var n = a(5318);
+        87: (e, t, n) => {
+            var a = n(5318);
             t.Z = void 0;
-            var s = n(a(4938)),
-                i = a(5893),
+            var s = a(n(4938)),
+                i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
                 }), "Language");
             t.Z = o
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.0","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.1","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6188,15 +6188,15 @@
                     })
                 }));
             var Ns = o(8543),
                 Bs = o(5827),
                 js = o(76),
                 zs = o(6727),
                 Os = o(8441),
-                Ds = o(7651),
+                Ds = o(8962),
                 Es = o(9674);
 
             function Fs(e) {
                 return (0, Je.Z)("MuiLink", e)
             }
             const Ws = (0, Ke.Z)("MuiLink", ["root", "underlineNone", "underlineHover", "underlineAlways", "button", "focusVisible"]);
             var Us = o(4844);
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5740,15 +5740,15 @@
                             return l(arguments, "callee").get
                         } catch (e) {
                             return c
                         }
                     }
                 }() : c,
                 d = i(1405)(),
-                u = i(8185)(),
+                u = i(3276)(),
                 f = Object.getPrototypeOf || (u ? function(e) {
                     return e.__proto__
                 } : null),
                 p = {},
                 g = "undefined" != typeof Uint8Array && f ? f(Uint8Array) : n,
                 m = {
                     "%AggregateError%": "undefined" == typeof AggregateError ? n : AggregateError,
@@ -5985,15 +5985,15 @@
                         value: 1
                     }).length
                 } catch (e) {
                     return !0
                 }
             }, e.exports = s
         },
-        8185: e => {
+        3276: e => {
             "use strict";
             var t = {
                     foo: {}
                 },
                 i = Object;
             e.exports = function() {
                 return {
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
-            1514: (e, r, t) => {
+            3570: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -48,58 +48,58 @@
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "2135a6297693b09662d9",
+        181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "5350b743f9a235d9e265",
+        548: "a6ac1d0d39311897c48d",
         571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "c508feab9dfdf7494214",
+        799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "7f061638d47075ac76be",
+        823: "26c15aab8d5d7301c11a",
         853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
         891: "4794a088a65e99550778"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
-        181: "2135a6297693b09662d9",
+        181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "5350b743f9a235d9e265",
+        548: "a6ac1d0d39311897c48d",
         571: "8dccdf5de15d462291c1",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
-        799: "c508feab9dfdf7494214",
+        799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "7f061638d47075ac76be",
+        823: "26c15aab8d5d7301c11a",
         853: "ced0d3671ec7406522f7",
         860: "d9b9c7e6da98c3818e92",
         891: "4794a088a65e99550778"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.1", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(1514);
+    var E = S(3570);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_error_util.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_error_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_handlers.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/tests/test_request_logger.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_request_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     assert (
         data["UriPath"] == "/jupyterlab/default/aws/sagemaker/api/git/list-repositories"
     )
     assert data["ResponseLatencyMS"] == 0.1
     assert (
         data["Context"]["ExtensionName"] == "SagemakerStudioJuypterLabExtensionCommon"
     )
-    assert data["Context"]["ExtensionVersion"] == "0.3.0"
+    assert data["Context"]["ExtensionVersion"] == "0.3.1"
     assert data["Context"]["AccountId"] == "1234567890"
     assert data["Context"]["DomainId"] == "d-jk12345678"
     assert data["Context"]["SpaceName"] == "default-space"
     data["_aws"]["Timestamp"] = 123456
 
     assert data["_aws"] == {
         "CloudWatchMetrics": [
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/error_util.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/error_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/git_clone_util.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/git_clone_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension/utils/request_logger.py` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/request_logger.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/PKG-INFO` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.3.0
+Version: 0.3.1
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt` & `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 THIRD-PARTY-LICENSES
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
 jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
-public_dist/sagemaker_jupyterlab_extension-0.3.0-py3-none-any.whl
+public_dist/sagemaker_jupyterlab_extension-0.3.1-py3-none-any.whl
 sagemaker_jupyterlab_extension/__init__.py
 sagemaker_jupyterlab_extension/_version.py
 sagemaker_jupyterlab_extension/handlers.py
 sagemaker_jupyterlab_extension.egg-info/PKG-INFO
 sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
 sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
 sagemaker_jupyterlab_extension.egg-info/not-zip-safe
 sagemaker_jupyterlab_extension.egg-info/requires.txt
 sagemaker_jupyterlab_extension.egg-info/top_level.txt
 sagemaker_jupyterlab_extension/labextension/package.json
 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
-sagemaker_jupyterlab_extension/labextension/static/181.2135a6297693b09662d9.js
+sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
-sagemaker_jupyterlab_extension/labextension/static/548.5350b743f9a235d9e265.js
+sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js
 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
-sagemaker_jupyterlab_extension/labextension/static/799.c508feab9dfdf7494214.js
-sagemaker_jupyterlab_extension/labextension/static/823.7f061638d47075ac76be.js
+sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
+sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js
 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
-sagemaker_jupyterlab_extension/labextension/static/remoteEntry.27a0e3dfb32431afe940.js
+sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js
 sagemaker_jupyterlab_extension/labextension/static/style.js
 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 sagemaker_jupyterlab_extension/tests/__init__.py
 sagemaker_jupyterlab_extension/tests/helper.py
 sagemaker_jupyterlab_extension/tests/test_error_util.py
 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
 sagemaker_jupyterlab_extension/tests/test_handlers.py
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/setup.py` & `sagemaker-jupyterlab-extension-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/GitCloneComponent.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/GitCloneComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/ResourceUsageComponent.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/ResourceUsageComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/AutoComplete.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/AutoComplete.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/CheckboxComponent.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/CheckboxComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/GitCloneComponent.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/GitCloneComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/InputField.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/InputField.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/LinearProgressWithLabel.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/LinearProgressWithLabel.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/ResourceUsageComponent.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/ResourceUsageComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/__tests__/SpaceMenu.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/SpaceMenu.spec.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -6,38 +6,40 @@
 import { il18Strings } from '../../constants/il18Strings';
 
 // Mocking the getCookie function
 jest.mock('../../utils/sessionManagerUtils', () => ({
   getCookie: jest.fn(),
 }));
 
-const { privateSpaceHeader, unknownUser } = il18Strings.Space;
+const { unknownSpace, unknownUser } = il18Strings.Space;
 
 describe('SpaceMenu Component', () => {
   beforeEach(() => {
     jest.clearAllMocks(); // Reset mock calls before each test
   });
 
+  const cookie = ['studioUserProfileName:John Doe', 'John Doe'];
+
   test('renders private space header when spaceName is not provided', () => {
     // Mocking the getCookie function to return a user profile name
-    getCookie.mockReturnValue('John Doe');
+    getCookie.mockReturnValue(cookie);
 
     const { getByTestId, getByText } = render(<SpaceMenu spaceName="" />);
 
     // Assert that the header element is rendered
     const headerElement = getByTestId(spaceTestIds.menu.header);
     expect(headerElement).toBeTruthy();
 
     // Assert that the user profile name is displayed correctly
-    expect(getByText('John Doe / ' + privateSpaceHeader)).toBeTruthy();
+    expect(getByText('John Doe / ' + unknownSpace)).toBeTruthy();
   });
 
   test('renders shared space header when spaceName is provided', () => {
     // Mocking the getCookie function to return a user profile name
-    getCookie.mockReturnValue('John Doe');
+    getCookie.mockReturnValue(cookie);
 
     const { getByTestId, getByText } = render(<SpaceMenu spaceName="Shared Space" />);
 
     // Assert that the header element is rendered
     const headerElement = getByTestId(spaceTestIds.menu.header);
     expect(headerElement).toBeTruthy();
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/common/AutoComplete.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/common/AutoComplete.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/common/CheckboxComponent.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/common/CheckboxComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/common/InputField.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/common/InputField.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/common/LinearProgressWithLabel.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/components/common/LinearProgressWithLabel.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/components/styles/InputFieldStyles.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/components/styles/InputFieldStyles.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/constants/common.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/constants/common.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/constants/il18Strings.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/constants/il18Strings.ts`

 * *Files 1% similar despite different names*

```diff
@@ -62,9 +62,10 @@
       invalidCloneUrlTitle: 'Invalid URL provided',
       invalidCloneUrlBody: 'The URL provided is not valid. Please input a valid URL to clone.',
     },
   },
   Space: {
     privateSpaceHeader: 'Personal Studio',
     unknownUser: 'Unknown User',
+    unknownSpace: 'Unknown Space',
   },
 };
```

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/constants/resourceUsageConstants.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/constants/resourceUsageConstants.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/constants/sessionManagementConstants.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/constants/sessionManagementConstants.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/GitClonePlugin.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/GitClonePlugin.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/HideShutDownPlugin.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/HideShutDownPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/PerformancePlugin/utils.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/utils.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/ResourceUsagePlugin.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/ResourceUsagePlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/SessionManagementPlugin.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/SessionManagementPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/SpaceMenuPlugin.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/SpaceMenuPlugin.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/GitClonePlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/GitClonePlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/HideShutDownPlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/HideShutDownPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/ResourceUsagePlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/ResourceUsagePlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/SessionManagementPlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/SessionManagementPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/plugins/__tests__/SpaceMenuPlugin.spec.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/SpaceMenuPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/index.spec.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/service/__tests__/mock.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/mock.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/service/constants.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/service/constants.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/service/index.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/service/index.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/utils/ReactWidgetWrapper.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/utils/ReactWidgetWrapper.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/gitCloneUtils.spec.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/gitCloneUtils.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/utils/__tests__/sessionManagerUtils.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/sessionManagerUtils.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/utils/gitCloneUtils.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/utils/gitCloneUtils.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/utils/logger.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/utils/logger.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/utils/sessionManagerUtils.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/utils/sessionManagerUtils.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/widgets/GitCloneWidget.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/widgets/GitCloneWidget.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/widgets/ResourceUsageWidget.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/widgets/ResourceUsageWidget.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/widgets/SpaceMenuWidget.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/widgets/SpaceMenuWidget.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/GitCloneWidget.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/GitCloneWidget.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/widgets/__tests__/ResourceUsageWidget.spec.tsx` & `sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/ResourceUsageWidget.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/src/widgets/styles/resourceUsageStyle.ts` & `sagemaker-jupyterlab-extension-0.3.1/src/widgets/styles/resourceUsageStyle.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.0/tsconfig.json` & `sagemaker-jupyterlab-extension-0.3.1/tsconfig.json`

 * *Files identical despite different names*

