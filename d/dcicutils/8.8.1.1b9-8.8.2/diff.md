# Comparing `tmp/dcicutils-8.8.1.1b9.tar.gz` & `tmp/dcicutils-8.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.1.1b9.tar", max compression
+gzip compressed data, was "dcicutils-8.8.2.tar", max compression
```

## Comparing `dcicutils-8.8.1.1b9.tar` & `dcicutils-8.8.2.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1102 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/README.rst
--rw-r--r--   0        0        0        0 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     2522 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7414 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/data_utils.py
--rw-r--r--   0        0        0     4666 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    68891 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    72972 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     2663 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/log_utils.py
--rw-r--r--   0        0        0   102210 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15408 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30260 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/portal_utils.py
--rw-r--r--   0        0        0     1475 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/progress_constants.py
--rw-r--r--   0        0        0    31250 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    58559 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/structured_data.py
--rw-r--r--   0        0        0     8082 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2027 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4714 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.1.1b9/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-04 18:38:58.343886 dcicutils-8.8.2/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-04 18:38:58.343886 dcicutils-8.8.2/README.rst
+-rw-r--r--   0        0        0        0 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     2522 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7414 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/data_utils.py
+-rw-r--r--   0        0        0     4666 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    68891 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-04 18:38:58.343886 dcicutils-8.8.2/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   102210 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30260 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    31250 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-04 18:38:58.347886 dcicutils-8.8.2/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    58451 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-04-04 18:38:58.351886 dcicutils-8.8.2/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4685 2024-04-04 18:38:58.351886 dcicutils-8.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 dcicutils-8.8.2/PKG-INFO
```

### Comparing `dcicutils-8.8.1.1b9/LICENSE.txt` & `dcicutils-8.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/README.rst` & `dcicutils-8.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/base.py` & `dcicutils-8.8.2/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.2/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/bundle_utils.py` & `dcicutils-8.8.2/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/captured_output.py` & `dcicutils-8.8.2/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.2/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/codebuild_utils.py` & `dcicutils-8.8.2/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/command_utils.py` & `dcicutils-8.8.2/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/common.py` & `dcicutils-8.8.2/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/contribution_scripts.py` & `dcicutils-8.8.2/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/contribution_utils.py` & `dcicutils-8.8.2/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/creds_utils.py` & `dcicutils-8.8.2/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/data_readers.py` & `dcicutils-8.8.2/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/data_utils.py` & `dcicutils-8.8.2/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/datetime_utils.py` & `dcicutils-8.8.2/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/deployment_utils.py` & `dcicutils-8.8.2/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/diff_utils.py` & `dcicutils-8.8.2/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/docker_utils.py` & `dcicutils-8.8.2/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/ecr_scripts.py` & `dcicutils-8.8.2/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/ecr_utils.py` & `dcicutils-8.8.2/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/ecs_utils.py` & `dcicutils-8.8.2/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/env_base.py` & `dcicutils-8.8.2/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/env_manager.py` & `dcicutils-8.8.2/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/env_scripts.py` & `dcicutils-8.8.2/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/env_utils.py` & `dcicutils-8.8.2/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.2/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/es_utils.py` & `dcicutils-8.8.2/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/exceptions.py` & `dcicutils-8.8.2/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/ff_mocks.py` & `dcicutils-8.8.2/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/ff_utils.py` & `dcicutils-8.8.2/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/file_utils.py` & `dcicutils-8.8.2/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.2/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/glacier_utils.py` & `dcicutils-8.8.2/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/jh_utils.py` & `dcicutils-8.8.2/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.2/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/kibana/readme.md` & `dcicutils-8.8.2/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/lang_utils.py` & `dcicutils-8.8.2/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.2/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.2/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/license_utils.py` & `dcicutils-8.8.2/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/log_utils.py` & `dcicutils-8.8.2/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/misc_utils.py` & `dcicutils-8.8.2/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.2/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/opensearch_utils.py` & `dcicutils-8.8.2/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/portal_object_utils.py` & `dcicutils-8.8.2/dcicutils/portal_object_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                     # TODO: Import from somewhere ...
                     lookup_options = 0
                     if schema := self.schema:
                         # TODO: Hook into the ref_lookup_strategy thing in structured_data to make
                         # sure we check accession format (since it does not have a pattern).
                         if callable(ref_lookup_strategy):
                             lookup_options, ref_validator = ref_lookup_strategy(
-                                self.type, schema, identifying_value)
+                                self._portal, self.type, schema, identifying_value)
                             if callable(ref_validator):
                                 if ref_validator(schema, identifying_property, identifying_value) is False:
                                     continue
                         if pattern := schema.get("properties", {}).get(identifying_property, {}).get("pattern"):
                             if not re.match(pattern, identifying_value):
                                 # If this identifying value is for a (identifying) property which has a
                                 # pattern, and the value does NOT match the pattern, then do NOT include
```

### Comparing `dcicutils-8.8.1.1b9/dcicutils/portal_utils.py` & `dcicutils-8.8.2/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/project_utils.py` & `dcicutils-8.8.2/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/qa_checkers.py` & `dcicutils-8.8.2/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/qa_utils.py` & `dcicutils-8.8.2/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/redis_tools.py` & `dcicutils-8.8.2/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/redis_utils.py` & `dcicutils-8.8.2/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/s3_utils.py` & `dcicutils-8.8.2/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/schema_utils.py` & `dcicutils-8.8.2/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.2/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.2/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.2/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/secrets_utils.py` & `dcicutils-8.8.2/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/sheet_utils.py` & `dcicutils-8.8.2/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/snapshot_utils.py` & `dcicutils-8.8.2/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.2/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/structured_data.py` & `dcicutils-8.8.2/dcicutils/structured_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dcicutils.datetime_utils import normalize_date_string, normalize_datetime_string
 from dcicutils.file_utils import search_for_file
 from dcicutils.misc_utils import (create_dict, create_readonly_object, is_uuid, load_json_if,
                                   merge_objects, remove_empty_properties, right_trim, split_string,
                                   to_boolean, to_enum, to_float, to_integer, VirtualApp)
 from dcicutils.portal_object_utils import PortalObject
 from dcicutils.portal_utils import Portal as PortalBase
-from dcicutils.progress_constants import PROGRESS_PARSE as PROGRESS
+from dcicutils.submitr.progress_constants import PROGRESS_PARSE as PROGRESS
 from dcicutils.schema_utils import Schema as SchemaBase
 from dcicutils.zip_utils import unpack_gz_file_to_temporary_file, unpack_files
 
 
 # Classes/functions to parse a CSV or Excel Spreadsheet into structured data, using a specialized
 # syntax to allow structured object properties to be referenced by column specifiers. This syntax
 # uses an (intuitive) dot notation to reference nested objects, and a (less intuitive) notation
@@ -188,15 +188,15 @@
                 ntypes = len(self.data)
                 for type_name in self.data:
                     nobjects += len(self.data[type_name])
             return ntypes, nobjects
         diffs = {}
         if callable(progress):
             ntypes, nobjects = get_counts()
-            progress({PROGRESS.ANALYZE_START: True,
+            progress({PROGRESS.ANALYZE_START: PROGRESS.NOW(),
                       PROGRESS.ANALYZE_COUNT_TYPES: ntypes, PROGRESS.ANALYZE_COUNT_ITEMS: nobjects})
         if self.data or self.portal:  # TODO: what is this OR biz?
             refs = self.resolved_refs_with_uuids
             # TODO: Need feedback/progress tracking mechanism here.
             # TODO: Check validity of reference; actually check that earlier on even maybe.
             for type_name in self.data:
                 if not diffs.get(type_name):
@@ -209,26 +209,27 @@
                         object_diffs, nlookups_compare = portal_object.compare(
                             existing_object, consider_refs=True, resolved_refs=refs)
                         diffs[type_name].append(create_readonly_object(path=identifying_path,
                                                                        uuid=existing_object.uuid,
                                                                        diffs=object_diffs or None))
                         if callable(progress):
                             progress({PROGRESS.ANALYZE_UPDATE: True,
-                                      PROGRESS.ANALYZE_COUNT_LOOKUP: nlookups + nlookups_compare})
+                                      PROGRESS.ANALYZE_LOOKUPS: nlookups + nlookups_compare})
                     elif identifying_path:
                         # If there is no existing object we still create a record for this object
                         # but with no uuid which will be the indication that it does not exist.
                         diffs[type_name].append(create_readonly_object(path=identifying_path, uuid=None, diffs=None))
                         if callable(progress):
-                            progress({PROGRESS.ANALYZE_CREATE: True, PROGRESS.ANALYZE_COUNT_LOOKUP: nlookups})
+                            progress({PROGRESS.ANALYZE_CREATE: True,
+                                      PROGRESS.ANALYZE_LOOKUPS: nlookups})
                     else:
                         if callable(progress):
-                            progress({PROGRESS.ANALYZE_COUNT_LOOKUP: nlookups})
+                            progress({PROGRESS.ANALYZE_LOOKUPS: nlookups})
         if callable(progress):
-            progress({PROGRESS.ANALYZE_DONE: True})
+            progress({PROGRESS.ANALYZE_DONE: PROGRESS.NOW()})
         return diffs
 
     def load_file(self, file: str) -> None:
         # Returns a dictionary where each property is the name (i.e. the type) of the data,
         # and the value is array of dictionaries for the data itself. Handle these kinds of files:
         # 1.  Single CSV, TSV, or JSON file, where the (base) name of the file is the data type name.
         # 2.  Single Excel file containing one or more sheets, where each sheet
@@ -267,15 +268,15 @@
             nrows = 0
             for sheet_name in excel.sheet_names:
                 for row in excel.sheet_reader(sheet_name):
                     nrows += 1
             return nrows, len(excel.sheet_names)
         if self._progress:  # TODO: Move to _load_reader
             nrows, nsheets = get_counts()
-            self._progress({PROGRESS.LOAD_START: True,
+            self._progress({PROGRESS.LOAD_START: PROGRESS.NOW(),
                             PROGRESS.LOAD_COUNT_SHEETS: nsheets, PROGRESS.LOAD_COUNT_ROWS: nrows})
         excel = Excel(file)  # Order the sheet names by any specified ordering (e.g. ala snovault.loadxl).
         order = {Schema.type_name(key): index for index, key in enumerate(self._order)} if self._order else {}
         for sheet_name in sorted(excel.sheet_names, key=lambda key: order.get(Schema.type_name(key), sys.maxsize)):
             self._load_reader(excel.sheet_reader(sheet_name), type_name=Schema.type_name(sheet_name))
         # TODO: Do we really need progress reporting for the below?
         # Check for unresolved reference errors which really are not because of ordering.
@@ -293,15 +294,15 @@
                     self._resolved_refs.add((ref, resolved.get("uuid")))
             if ref_errors_actual:
                 self._errors["ref"] = ref_errors_actual
             else:
                 del self._errors["ref"]
         if self._progress:
             self._progress({   # TODO: Refactor with same thing below in _load_reader.
-                PROGRESS.LOAD_DONE: True,
+                PROGRESS.LOAD_DONE: PROGRESS.NOW(),
                 PROGRESS.LOAD_COUNT_REFS: self.ref_total_count,
                 PROGRESS.LOAD_COUNT_REFS_FOUND: self.ref_total_found_count,
                 PROGRESS.LOAD_COUNT_REFS_NOT_FOUND: self.ref_total_notfound_count,
                 PROGRESS.LOAD_COUNT_REFS_LOOKUP: self.ref_lookup_count,
                 PROGRESS.LOAD_COUNT_REFS_LOOKUP_CACHE_HIT: self.ref_lookup_cache_hit_count,
                 PROGRESS.LOAD_COUNT_REFS_EXISTS_CACHE_HIT: self.ref_exists_cache_hit_count,
                 PROGRESS.LOAD_COUNT_REFS_INVALID: self.ref_invalid_identifying_property_count
@@ -649,14 +650,15 @@
             return value if value is not None else ""
         return map_datetime
 
     def _map_function_ref(self, typeinfo: dict) -> Callable:
         def map_ref(value: str, link_to: str, portal: Optional[Portal], src: Optional[str]) -> Any:
             nonlocal self, typeinfo
             if self._norefs:
+                self._resolved_refs.add((f"/{link_to}/{value}", None))
                 return value
             if not value:
                 if (column := typeinfo.get("column")) and column in self.data.get("required", []):
                     self._unresolved_refs.append({"src": src, "error": f"/{link_to}/<null>"})
             elif portal:
                 if not (resolved := portal.ref_exists(link_to, value, True)):
                     self._unresolved_refs.append({"src": src, "error": f"/{link_to}/{value}"})
@@ -816,15 +818,15 @@
             self._data = data if data is not None else arg._data  # Data set being loaded; e.g. by StructuredDataSet.
         else:
             self._schemas = schemas
             self._data = data
         if callable(ref_lookup_strategy):
             self._ref_lookup_strategy = ref_lookup_strategy
         else:
-            self._ref_lookup_strategy = lambda type_name, schema, value: (Portal.LOOKUP_DEFAULT, None)
+            self._ref_lookup_strategy = lambda portal, type_name, schema, value: (Portal.LOOKUP_DEFAULT, None)
         if ref_lookup_nocache is True:
             self.ref_lookup = self.ref_lookup_uncached
             self._ref_cache = None
         else:
             self.ref_lookup = self.ref_lookup_cached
             self._ref_cache = {}
         self._ref_lookup_found_count = 0
@@ -854,18 +856,14 @@
             else:
                 self._ref_lookup_error_count += 1
             return None
 
     @lru_cache(maxsize=100)
     def get_schema(self, schema_name: str) -> Optional[dict]:
         return schemas.get(Schema.type_name(schema_name), None) if (schemas := self.get_schemas()) else None
-#       if schema_name == schema_name.upper() and (schema := schemas.get(schema_name.lower().title())):
-#           return schema
-#       if schema_name == schema_name.lower() and (schema := schemas.get(schema_name.title())):
-#           return schema
 
     @lru_cache(maxsize=1)
     def get_schemas(self) -> Optional[dict]:
         if not (schemas := super().get_schemas()) or (schemas.get("status") == "error"):
             return None
         if self._schemas:
             schemas = copy.deepcopy(schemas)
@@ -886,15 +884,15 @@
             type_name, value = Portal._get_type_name_and_value_from_path(type_name)
             if not type_name or not value:
                 return None
         if called_from_map_ref:
             self._ref_total_count += 1
         # First make sure the given value can possibly be a reference to the given type.
         schema = self.get_schema(type_name)
-        ref_lookup_strategy, ref_validator = self._ref_lookup_strategy(type_name, schema, value)
+        ref_lookup_flags, ref_validator = self._ref_lookup_strategy(self, type_name, schema, value)
         if not self._is_valid_ref(type_name, value, ref_validator):
             if called_from_map_ref:
                 self._ref_invalid_identifying_property_count += 1
                 self._ref_total_notfound_count += 1
             return None
         # Check our reference cache.
         if (resolved := self._ref_exists_from_cache(type_name, value)) is not None:
@@ -916,19 +914,19 @@
             if called_from_map_ref:
                 self._ref_total_found_count += 1
             return resolved
         # Reference is NOT cached and was NOT resolved internally; lookup in PORTAL.
         # Get the lookup strategy; i.e. should do we lookup by root path, and if so, should
         # we do this first, and do we lookup by subtypes; by default we lookup by root path
         # but not first, and we also lookup by subtypes by default.
-        ref_lookup_strategy, _ = self._ref_lookup_strategy(type_name, self.get_schema(type_name), value)
-        is_ref_lookup_specified_type = StructuredDataSet._is_ref_lookup_specified_type(ref_lookup_strategy)
-        is_ref_lookup_root = StructuredDataSet._is_ref_lookup_root(ref_lookup_strategy)
-        is_ref_lookup_root_first = StructuredDataSet._is_ref_lookup_root_first(ref_lookup_strategy)
-        is_ref_lookup_subtypes = StructuredDataSet._is_ref_lookup_subtypes(ref_lookup_strategy)
+        ref_lookup_flags, _ = self._ref_lookup_strategy(self, type_name, self.get_schema(type_name), value)
+        is_ref_lookup_specified_type = StructuredDataSet._is_ref_lookup_specified_type(ref_lookup_flags)
+        is_ref_lookup_root = StructuredDataSet._is_ref_lookup_root(ref_lookup_flags)
+        is_ref_lookup_root_first = StructuredDataSet._is_ref_lookup_root_first(ref_lookup_flags)
+        is_ref_lookup_subtypes = StructuredDataSet._is_ref_lookup_subtypes(ref_lookup_flags)
         # First construct the list of lookup paths at which to look for the referenced item.
         lookup_paths = []
         if is_ref_lookup_root_first:
             lookup_paths.append(f"/{value}")
         if is_ref_lookup_specified_type:
             lookup_paths.append(f"/{type_name}/{value}")
         if is_ref_lookup_root and not is_ref_lookup_root_first:
@@ -965,17 +963,17 @@
         of the resolved item.
         """
         if not value:
             type_name, value = Portal._get_type_name_and_value_from_path(type_name)
             if not type_name or not value:
                 return None  # Should not happen.
         # Note that root lookup not applicable here.
-        ref_lookup_strategy, ref_validator = (
-            self._ref_lookup_strategy(type_name, self.get_schema(type_name), value))
-        is_ref_lookup_subtypes = StructuredDataSet._is_ref_lookup_subtypes(ref_lookup_strategy)
+        ref_lookup_flags, ref_validator = (
+            self._ref_lookup_strategy(self, type_name, self.get_schema(type_name), value))
+        is_ref_lookup_subtypes = StructuredDataSet._is_ref_lookup_subtypes(ref_lookup_flags)
         subtype_names = self.get_schema_subtype_names(type_name) if is_ref_lookup_subtypes else []
         for type_name in [type_name] + subtype_names:
             is_resolved, resolved_item = self._ref_exists_single_internally(type_name, value)
             if is_resolved:
                 if update_counts:
                     self._ref_exists_internal_count += 1
                     self._ref_total_found_count += 1
```

### Comparing `dcicutils-8.8.1.1b9/dcicutils/task_utils.py` & `dcicutils-8.8.2/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.2/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/trace_utils.py` & `dcicutils-8.8.2/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/validation_utils.py` & `dcicutils-8.8.2/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/variant_utils.py` & `dcicutils-8.8.2/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/dcicutils/zip_utils.py` & `dcicutils-8.8.2/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b9/pyproject.toml` & `dcicutils-8.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.1.1b9"  # TODO: To become 8.8.2
+version = "8.8.2"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.1.1b9/PKG-INFO` & `dcicutils-8.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.1.1b9
+Version: 8.8.2
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

