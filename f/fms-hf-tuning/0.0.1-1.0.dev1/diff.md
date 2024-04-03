# Comparing `tmp/fms-hf-tuning-0.0.1.tar.gz` & `tmp/fms-hf-tuning-1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms-hf-tuning-0.0.1.tar", last modified: Wed Apr  3 18:45:07 2024, max compression
+gzip compressed data, was "fms-hf-tuning-1.0.dev1.tar", last modified: Wed Apr  3 23:02:31 2024, max compression
```

## Comparing `fms-hf-tuning-0.0.1.tar` & `fms-hf-tuning-1.0.dev1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.422865 fms-hf-tuning-0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.409865 fms-hf-tuning-0.0.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.410865 fms-hf-tuning-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      675 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 root         (0) root         (0)      443 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0 root         (0) root         (0)      106 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      448 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.411865 fms-hf-tuning-0.0.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-03 18:27:57.000000 fms-hf-tuning-0.0.1/.github/workflows/build-and-publish.yaml
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.github/workflows/format.yml
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.isort.cfg
--rw-r--r--   0 root         (0) root         (0)      255 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    21494 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      299 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/CODEOWNERS
--rw-r--r--   0 root         (0) root         (0)     8344 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      167 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/Makefile
--rw-r--r--   0 root         (0) root         (0)    14238 2024-04-03 18:45:07.421865 fms-hf-tuning-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13064 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.411865 fms-hf-tuning-0.0.1/architecture_records/
--rw-r--r--   0 root         (0) root         (0)     2243 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/architecture_records/template.md
--rw-r--r--   0 root         (0) root         (0)     3362 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/code-of-conduct.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.402865 fms-hf-tuning-0.0.1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.411865 fms-hf-tuning-0.0.1/examples/prompt_tuning_twitter_complaints/
--rw-r--r--   0 root         (0) root         (0)     2351 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/examples/prompt_tuning_twitter_complaints/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.412865 fms-hf-tuning-0.0.1/fixtures/
--rw-r--r--   0 root         (0) root         (0)     2849 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/fixtures/accelerate_fsdp_defaults.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.419865 fms-hf-tuning-0.0.1/fms_hf_tuning.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14238 2024-04-03 18:45:07.000000 fms-hf-tuning-0.0.1/fms_hf_tuning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1449 2024-04-03 18:45:07.000000 fms-hf-tuning-0.0.1/fms_hf_tuning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 18:45:07.000000 fms-hf-tuning-0.0.1/fms_hf_tuning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      193 2024-04-03 18:45:07.000000 fms-hf-tuning-0.0.1/fms_hf_tuning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 18:45:07.000000 fms-hf-tuning-0.0.1/fms_hf_tuning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      963 2024-04-03 18:43:54.000000 fms-hf-tuning-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      247 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/pytest.ini
--rw-r--r--   0 root         (0) root         (0)      120 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.413865 fms-hf-tuning-0.0.1/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      720 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/scripts/fmt.sh
--rw-r--r--   0 root         (0) root         (0)    10833 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/scripts/run_inference.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 18:45:07.422865 fms-hf-tuning-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      715 2024-04-03 18:41:11.000000 fms-hf-tuning-0.0.1/setup.py
--rw-r--r--   0 root         (0) root         (0)       95 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/setup_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.414865 fms-hf-tuning-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.415865 fms-hf-tuning-0.0.1/tests/build/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/build/dummy_job_config.json
--rw-r--r--   0 root         (0) root         (0)     2780 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/build/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.415865 fms-hf-tuning-0.0.1/tests/data/
--rw-r--r--   0 root         (0) root         (0)      831 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3198 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/data/twitter_complaints_small.json
--rw-r--r--   0 root         (0) root         (0)     1432 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/helpers.py
--rw-r--r--   0 root         (0) root         (0)    11750 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/test_sft_trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.416865 fms-hf-tuning-0.0.1/tests/utils/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tests/utils/test_data_type_utils.py
--rw-r--r--   0 root         (0) root         (0)      695 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.416865 fms-hf-tuning-0.0.1/tuning/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1384 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/aim_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.417865 fms-hf-tuning-0.0.1/tuning/config/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3077 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/config/configs.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/config/peft_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.418865 fms-hf-tuning-0.0.1/tuning/data/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1593 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/data/tokenizer_data_utils.py
--rw-r--r--   0 root         (0) root         (0)    11268 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/sft_trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 18:45:07.419865 fms-hf-tuning-0.0.1/tuning/utils/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3135 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/utils/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     2006 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/utils/data_type_utils.py
--rw-r--r--   0 root         (0) root         (0)      770 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/utils/import_utils.py
--rw-r--r--   0 root         (0) root         (0)     4136 2024-04-02 22:14:14.000000 fms-hf-tuning-0.0.1/tuning/utils/merge_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.205817 fms-hf-tuning-1.0.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.197817 fms-hf-tuning-1.0.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.github/workflows/build-and-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-04-03 23:02:31.205817 fms-hf-tuning-1.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/architecture_records/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/architecture_records/template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/code-of-conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.193817 fms-hf-tuning-1.0.dev1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/examples/prompt_tuning_twitter_complaints/
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/examples/prompt_tuning_twitter_complaints/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/fixtures/accelerate_fsdp_defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.205817 fms-hf-tuning-1.0.dev1/fms_hf_tuning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-04-03 23:02:31.000000 fms-hf-tuning-1.0.dev1/fms_hf_tuning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 23:02:31.000000 fms-hf-tuning-1.0.dev1/fms_hf_tuning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:02:31.000000 fms-hf-tuning-1.0.dev1/fms_hf_tuning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-03 23:02:31.000000 fms-hf-tuning-1.0.dev1/fms_hf_tuning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 23:02:31.000000 fms-hf-tuning-1.0.dev1/fms_hf_tuning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 22:58:20.000000 fms-hf-tuning-1.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/scripts/fmt.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/scripts/run_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:02:31.205817 fms-hf-tuning-1.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/setup_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/tests/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/build/dummy_job_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/build/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/data/twitter_complaints_small.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/test_sft_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.201817 fms-hf-tuning-1.0.dev1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tests/utils/test_data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.205817 fms-hf-tuning-1.0.dev1/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/aim_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.205817 fms-hf-tuning-1.0.dev1/tuning/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/config/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/config/peft_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.205817 fms-hf-tuning-1.0.dev1/tuning/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/data/tokenizer_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/sft_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:02:31.205817 fms-hf-tuning-1.0.dev1/tuning/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/utils/data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-03 22:58:10.000000 fms-hf-tuning-1.0.dev1/tuning/utils/merge_model_utils.py
```

### Comparing `fms-hf-tuning-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `fms-hf-tuning-1.0.dev1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `fms-hf-tuning-1.0.dev1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/.github/workflows/build-and-publish.yaml` & `fms-hf-tuning-1.0.dev1/.github/workflows/build-and-publish.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -20,15 +20,20 @@
             release-version:
               type: string
               required: true
               description: 'Version number (for example: 0.0.1)'
 
 jobs:
   build:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
+    environment:
+      name: pypi
+      url: https://pypi.org/p/fms-hf-tuning
+    permissions:
+      id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
           python-version: 3.9
       - name: Install dependencies
@@ -40,13 +45,15 @@
           export RELEASE_VERSION=${{ github.event.inputs.release-version }}
           sed -i "s/^version = \"[0-9.]*\"$/version = \"${RELEASE_VERSION}\"/g" pyproject.toml
       - name: Build and test with tox
         run: tox -e py39
       - name: Build and check wheel package
         run:
           tox -e build,twinecheck
+      - name: Publish package distributions to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
 # Work in progress... need to get a PYPI_TOKEN in the repo
 #      - name: Publish wheel package on PyPI
 #        if: github.event_name == 'release'
 #        uses: pypa/gh-action-pypi-publish@release/v1
 #        with:
 #          password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `fms-hf-tuning-0.0.1/.github/workflows/format.yml` & `fms-hf-tuning-1.0.dev1/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/.pylintrc` & `fms-hf-tuning-1.0.dev1/.pylintrc`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/CONTRIBUTING.md` & `fms-hf-tuning-1.0.dev1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/LICENSE` & `fms-hf-tuning-1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/PKG-INFO` & `fms-hf-tuning-1.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fms-hf-tuning
-Version: 0.0.1
+Version: 1.0.dev1
 Summary: FMS HF Tuning
 Author-email: Sukriti Sharma <sukriti.sharma4@ibm.com>, Anh Uong <anh.uong@ibm.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/foundation-model-stack/fms-hf-tuning
 Project-URL: Repository, https://github.com/foundation-model-stack/fms-hf-tuning
 Project-URL: Issues, https://github.com/foundation-model-stack/fms-hf-tuning/issues
 Keywords: fms-hf-tuning,python,tuning
```

### Comparing `fms-hf-tuning-0.0.1/README.md` & `fms-hf-tuning-1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/architecture_records/template.md` & `fms-hf-tuning-1.0.dev1/architecture_records/template.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/code-of-conduct.md` & `fms-hf-tuning-1.0.dev1/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/examples/prompt_tuning_twitter_complaints/README.md` & `fms-hf-tuning-1.0.dev1/examples/prompt_tuning_twitter_complaints/README.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/fixtures/accelerate_fsdp_defaults.yaml` & `fms-hf-tuning-1.0.dev1/fixtures/accelerate_fsdp_defaults.yaml`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/fms_hf_tuning.egg-info/PKG-INFO` & `fms-hf-tuning-1.0.dev1/fms_hf_tuning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fms-hf-tuning
-Version: 0.0.1
+Version: 1.0.dev1
 Summary: FMS HF Tuning
 Author-email: Sukriti Sharma <sukriti.sharma4@ibm.com>, Anh Uong <anh.uong@ibm.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/foundation-model-stack/fms-hf-tuning
 Project-URL: Repository, https://github.com/foundation-model-stack/fms-hf-tuning
 Project-URL: Issues, https://github.com/foundation-model-stack/fms-hf-tuning/issues
 Keywords: fms-hf-tuning,python,tuning
```

### Comparing `fms-hf-tuning-0.0.1/fms_hf_tuning.egg-info/SOURCES.txt` & `fms-hf-tuning-1.0.dev1/fms_hf_tuning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/pyproject.toml` & `fms-hf-tuning-1.0.dev1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [build-system]
 requires = [
     "setuptools>=61",
     "setuptools-scm>=8.0"]
 
 [project]
 name = "fms-hf-tuning"
-version = "0.0.1"
-#dynamic = ["version"]
+version = "1.0.dev1"
 description = "FMS HF Tuning"
 authors = [
   {name = "Sukriti Sharma", email = "sukriti.sharma4@ibm.com"},
   {name = "Anh Uong", email = "anh.uong@ibm.com"},
 ]
 license = {text = "Apache-2.0"}
 readme = "README.md"
```

### Comparing `fms-hf-tuning-0.0.1/scripts/fmt.sh` & `fms-hf-tuning-1.0.dev1/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/scripts/run_inference.py` & `fms-hf-tuning-1.0.dev1/scripts/run_inference.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/setup.py` & `fms-hf-tuning-1.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/__init__.py` & `fms-hf-tuning-1.0.dev1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/build/__init__.py` & `fms-hf-tuning-1.0.dev1/tests/build/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/build/dummy_job_config.json` & `fms-hf-tuning-1.0.dev1/tests/build/dummy_job_config.json`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/build/test_utils.py` & `fms-hf-tuning-1.0.dev1/tests/build/test_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/data/__init__.py` & `fms-hf-tuning-1.0.dev1/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/data/twitter_complaints_small.json` & `fms-hf-tuning-1.0.dev1/tests/data/twitter_complaints_small.json`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/helpers.py` & `fms-hf-tuning-1.0.dev1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/test_sft_trainer.py` & `fms-hf-tuning-1.0.dev1/tests/test_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/utils/__init__.py` & `fms-hf-tuning-1.0.dev1/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tests/utils/test_data_type_utils.py` & `fms-hf-tuning-1.0.dev1/tests/utils/test_data_type_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tox.ini` & `fms-hf-tuning-1.0.dev1/tox.ini`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/__init__.py` & `fms-hf-tuning-1.0.dev1/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/aim_loader.py` & `fms-hf-tuning-1.0.dev1/tuning/aim_loader.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/config/__init__.py` & `fms-hf-tuning-1.0.dev1/tuning/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/config/configs.py` & `fms-hf-tuning-1.0.dev1/tuning/config/configs.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/config/peft_config.py` & `fms-hf-tuning-1.0.dev1/tuning/config/peft_config.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/data/__init__.py` & `fms-hf-tuning-1.0.dev1/tuning/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/data/tokenizer_data_utils.py` & `fms-hf-tuning-1.0.dev1/tuning/data/tokenizer_data_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/sft_trainer.py` & `fms-hf-tuning-1.0.dev1/tuning/sft_trainer.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/utils/__init__.py` & `fms-hf-tuning-1.0.dev1/tuning/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/utils/config_utils.py` & `fms-hf-tuning-1.0.dev1/tuning/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/utils/data_type_utils.py` & `fms-hf-tuning-1.0.dev1/tuning/utils/data_type_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/utils/import_utils.py` & `fms-hf-tuning-1.0.dev1/tuning/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-0.0.1/tuning/utils/merge_model_utils.py` & `fms-hf-tuning-1.0.dev1/tuning/utils/merge_model_utils.py`

 * *Files identical despite different names*

