# Comparing `tmp/sagemaker-schema-inference-artifacts-0.0.2.tar.gz` & `tmp/sagemaker-schema-inference-artifacts-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-schema-inference-artifacts-0.0.2.tar", last modified: Mon Apr  1 20:59:39 2024, max compression
+gzip compressed data, was "sagemaker-schema-inference-artifacts-0.0.4.tar", last modified: Thu Apr  4 17:57:23 2024, max compression
```

## Comparing `sagemaker-schema-inference-artifacts-0.0.2.tar` & `sagemaker-schema-inference-artifacts-0.0.4.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.925779 sagemaker-schema-inference-artifacts-0.0.2/
--rw-r--r--   0 samruds  (4963930) amazon     (100)    10142 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/LICENSE
--rw-r--r--   0 samruds  (4963930) amazon     (100)      298 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/MANIFEST.in
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2265 2024-04-01 20:59:39.925779 sagemaker-schema-inference-artifacts-0.0.2/PKG-INFO
--rw-r--r--   0 samruds  (4963930) amazon     (100)      862 2024-03-28 00:46:06.000000 sagemaker-schema-inference-artifacts-0.0.2/README.rst
--rw-r--r--   0 samruds  (4963930) amazon     (100)        6 2024-04-01 20:58:31.000000 sagemaker-schema-inference-artifacts-0.0.2/VERSION
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/requirements/
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/requirements/extras/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      210 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/extras/test_requirements.txt
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/
--rw-r--r--   0 samruds  (4963930) amazon     (100)       30 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/doc8_requirements.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)       18 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/docstyle_requirements.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)       42 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/flake8_requirements.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)       12 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/mypy_requirements.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)       18 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/pydocstyle_requirements.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)       29 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/pylint_requirements.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)       31 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/spelling_requirements.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)       13 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/requirements/tox/twine_requirements.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)      108 2024-04-01 20:59:39.925779 sagemaker-schema-inference-artifacts-0.0.2/setup.cfg
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3636 2024-03-28 22:05:48.000000 sagemaker-schema-inference-artifacts-0.0.2/setup.py
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/src/
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      599 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/__init__.py
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      599 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/__init__.py
--rw-r--r--   0 samruds  (4963930) amazon     (100)      290 2024-04-01 20:58:31.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/config.py
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1068 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/LICENSE
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2828 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/README.md
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/
--rw-r--r--   0 samruds  (4963930) amazon     (100)   223572 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.cjs
--rw-r--r--   0 samruds  (4963930) amazon     (100)   101724 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.d.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)   221943 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.js
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3071 2024-03-28 22:17:24.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/package.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/
--rw-r--r--   0 samruds  (4963930) amazon     (100)    43778 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/default-widget-inputs.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1603 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/index.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2152 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/library-to-tasks.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3253 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)      602 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries-downloads.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)    17447 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries-snippets.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)    11601 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)    13594 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/pipelines.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2565 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/curl.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)      170 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/index.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     5429 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/inputs.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4611 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/js.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     5339 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/python.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)      238 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/types.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3807 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1467 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1222 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1019 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      345 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2376 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1680 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/data.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     6533 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1900 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4851 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1080 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1052 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3713 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1955 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1776 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/output.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1460 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/output_stream.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4781 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/common-definitions.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1999 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1426 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)      651 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      663 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      412 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3537 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2522 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3012 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2897 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1071 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1350 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1377 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)      439 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      707 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      263 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3536 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1851 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1456 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1164 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      781 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2659 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1852 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1234 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1019 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      357 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2991 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3006 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1550 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1439 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      680 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3891 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3040 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1469 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1595 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      309 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3654 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2204 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4332 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      947 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      371 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/spec/output.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)    12509 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/index.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3354 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1473 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/data.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1512 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2273 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1349 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      785 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1045 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      453 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)      434 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/data.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      927 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      441 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3334 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2111 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2635 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2507 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      797 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     8922 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2573 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/data.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.905779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4235 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3109 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)      793 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1187 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      406 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3297 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2653 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1264 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      262 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      371 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1172 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1684 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1404 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1201 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1080 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3754 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1475 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/data.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4899 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1330 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/data.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     7247 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2012 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1224 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1032 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      354 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/
--rw-r--r--   0 samruds  (4963930) amazon     (100)    12087 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3321 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     5627 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3067 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4056 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/output.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1318 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/output_stream.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4338 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      848 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      477 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3427 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3206 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1591 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1775 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      333 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2910 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1659 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     4425 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      256 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      260 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2781 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3094 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/data.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1269 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1423 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      393 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3237 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2082 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2100 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2008 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      887 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3228 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1950 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1260 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)      256 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      373 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3233 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2423 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/data.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1617 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1767 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1432 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1290 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      357 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1945 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2297 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1489 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1263 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      546 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2804 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1473 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1773 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1696 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      368 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3892 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1729 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1521 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1377 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      385 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/output.json
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1709 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/about.md
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1692 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1464 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/inference.ts
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1136 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/input.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     1101 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/output.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)      713 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tokenizer-data.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)     3814 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/widget-example.ts
--rw-r--r--   0 samruds  (4963930) amazon     (100)      415 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/tsconfig.json
--rw-r--r--   0 samruds  (4963930) amazon     (100)     7265 2024-04-01 20:58:31.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/remote_schema_retriever.py
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.895779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/audio/
--rw-r--r--   0 samruds  (4963930) amazon     (100)       72 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/audio/mp3.mp3
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/image/
--rw-r--r--   0 samruds  (4963930) amazon     (100)       51 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/image/png-truncated.png
-drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-01 20:59:39.915779 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts.egg-info/
--rw-r--r--   0 samruds  (4963930) amazon     (100)     2265 2024-04-01 20:59:39.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts.egg-info/PKG-INFO
--rw-r--r--   0 samruds  (4963930) amazon     (100)    24002 2024-04-01 20:59:39.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts.egg-info/SOURCES.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)        1 2024-04-01 20:59:39.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts.egg-info/dependency_links.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)      230 2024-04-01 20:59:39.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts.egg-info/requires.txt
--rw-r--r--   0 samruds  (4963930) amazon     (100)       37 2024-04-01 20:59:39.000000 sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts.egg-info/top_level.txt
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)    10142 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/LICENSE
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      298 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/MANIFEST.in
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1664 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/PKG-INFO
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      862 2024-03-28 00:46:06.000000 sagemaker-schema-inference-artifacts-0.0.4/README.rst
+-rw-r--r--   0 samruds  (4963930) amazon     (100)        6 2024-04-04 17:56:42.000000 sagemaker-schema-inference-artifacts-0.0.4/VERSION
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/requirements/
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/requirements/extras/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      210 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/extras/test_requirements.txt
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       30 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/doc8_requirements.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       18 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/docstyle_requirements.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       42 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/flake8_requirements.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       12 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/mypy_requirements.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       18 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/pydocstyle_requirements.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       29 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/pylint_requirements.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       31 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/spelling_requirements.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       13 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/requirements/tox/twine_requirements.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      108 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/setup.cfg
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3636 2024-03-28 22:05:48.000000 sagemaker-schema-inference-artifacts-0.0.4/setup.py
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/src/
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      599 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/__init__.py
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      599 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/__init__.py
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      567 2024-04-04 17:56:42.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/config.py
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1068 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/LICENSE
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2828 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/README.md
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)   223954 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.cjs
+-rw-r--r--   0 samruds  (4963930) amazon     (100)   101590 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.d.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)   222371 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.js
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3069 2024-04-04 17:57:22.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/package.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)    43778 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/default-widget-inputs.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1580 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/index.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2471 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/library-to-tasks.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3253 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      602 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries-downloads.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)    17447 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries-snippets.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)    11601 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)    13594 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/pipelines.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2565 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/curl.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      170 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/index.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     5429 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/inputs.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4611 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/js.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     5339 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/python.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      238 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/types.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3807 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1467 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1222 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1019 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      345 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2376 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1680 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/data.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     6533 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1900 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4851 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1080 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1052 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3713 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1955 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1776 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/output.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1460 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/output_stream.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4781 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/common-definitions.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1999 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1426 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      651 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      663 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      412 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3537 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2522 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3012 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2897 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1071 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1350 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1377 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      439 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      707 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      263 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3536 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1851 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1456 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1164 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      781 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2659 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1852 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1234 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1019 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      357 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2991 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3006 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1550 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1439 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      680 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3891 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3040 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1469 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1595 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      309 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3654 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2204 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4332 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      947 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      371 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/spec/output.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)    12520 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/index.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3354 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1473 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/data.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1512 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2273 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1349 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      785 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1045 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      453 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      434 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/data.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      927 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      441 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3334 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2111 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2635 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2507 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      797 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     8922 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2573 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/data.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4235 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3109 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      793 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1187 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      406 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3297 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2653 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1264 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      262 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      371 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.084424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1172 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1684 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1404 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1201 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1080 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3754 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1475 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/data.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4899 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1330 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/data.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     7247 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2012 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1224 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1032 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      354 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)    12087 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3321 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     5627 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3067 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4056 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/output.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1318 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/output_stream.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4338 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      848 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      477 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3427 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3206 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1591 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1775 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      333 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2910 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1659 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     4425 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      256 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      260 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2781 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3094 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/data.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1269 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1423 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      393 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3237 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2082 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2100 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2008 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      887 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3228 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1950 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1260 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      256 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      373 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3233 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2423 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/data.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1617 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1767 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1432 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1290 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      357 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1945 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2297 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1489 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1263 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      546 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     2804 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1473 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1773 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1696 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      368 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3892 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1729 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1521 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1377 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      385 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/output.json
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1709 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/about.md
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1692 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1464 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/inference.ts
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1136 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/input.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1101 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/output.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      713 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tokenizer-data.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     3814 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/widget-example.ts
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      415 1985-10-26 08:15:00.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/tsconfig.json
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     9100 2024-04-04 17:56:42.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/remote_schema_retriever.py
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/audio/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)   278018 2024-04-04 17:56:42.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/audio/sample.flac
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.094424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/image/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       51 2024-03-27 23:13:32.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/sample_data/image/png-truncated.png
+drwxr-xr-x   0 samruds  (4963930) amazon     (100)        0 2024-04-04 17:57:23.074424 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts.egg-info/
+-rw-r--r--   0 samruds  (4963930) amazon     (100)     1664 2024-04-04 17:57:22.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts.egg-info/PKG-INFO
+-rw-r--r--   0 samruds  (4963930) amazon     (100)    24006 2024-04-04 17:57:23.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts.egg-info/SOURCES.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)        1 2024-04-04 17:57:22.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts.egg-info/dependency_links.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)      230 2024-04-04 17:57:22.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts.egg-info/requires.txt
+-rw-r--r--   0 samruds  (4963930) amazon     (100)       37 2024-04-04 17:57:22.000000 sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts.egg-info/top_level.txt
```

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/LICENSE` & `sagemaker-schema-inference-artifacts-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/README.rst` & `sagemaker-schema-inference-artifacts-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/setup.py` & `sagemaker-schema-inference-artifacts-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/__init__.py` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/__init__.py` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/LICENSE` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/README.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.cjs` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.cjs`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 // src/index.ts
 var src_exports = {};
 __export(src_exports, {
   ALL_DISPLAY_MODEL_LIBRARY_KEYS: () => ALL_DISPLAY_MODEL_LIBRARY_KEYS,
   ALL_MODEL_LIBRARY_KEYS: () => ALL_MODEL_LIBRARY_KEYS,
   InferenceDisplayability: () => InferenceDisplayability,
-  LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS: () => LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS,
+  LIBRARY_TASK_MAPPING: () => LIBRARY_TASK_MAPPING,
   MAPPING_DEFAULT_WIDGET: () => MAPPING_DEFAULT_WIDGET,
   MODALITIES: () => MODALITIES,
   MODALITY_LABELS: () => MODALITY_LABELS,
   MODEL_LIBRARIES_UI_ELEMENTS: () => MODEL_LIBRARIES_UI_ELEMENTS,
   PIPELINE_DATA: () => PIPELINE_DATA,
   PIPELINE_TYPES: () => PIPELINE_TYPES,
   PIPELINE_TYPES_SET: () => PIPELINE_TYPES_SET,
@@ -36,15 +36,15 @@
   TASKS_DATA: () => TASKS_DATA,
   TASKS_MODEL_LIBRARIES: () => TASKS_MODEL_LIBRARIES,
   snippets: () => snippets_exports
 });
 module.exports = __toCommonJS(src_exports);
 
 // src/library-to-tasks.ts
-var LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS = {
+var LIBRARY_TASK_MAPPING = {
   "adapter-transformers": ["question-answering", "text-classification", "token-classification"],
   allennlp: ["question-answering"],
   asteroid: [
     // "audio-source-separation",
     "audio-to-audio"
   ],
   bertopic: ["text-classification"],
@@ -72,14 +72,32 @@
     "audio-to-audio",
     "automatic-speech-recognition",
     "text-to-speech",
     "text2text-generation"
   ],
   stanza: ["token-classification"],
   timm: ["image-classification"],
+  transformers: [
+    "audio-classification",
+    "automatic-speech-recognition",
+    "depth-estimation",
+    "document-question-answering",
+    "fill-mask",
+    "image-classification",
+    "image-segmentation",
+    "image-to-text",
+    "image-to-image",
+    "object-detection",
+    "question-answering",
+    "text-generation",
+    "text2text-generation",
+    "visual-question-answering",
+    "zero-shot-classification",
+    "zero-shot-image-classification"
+  ],
   mindspore: ["image-classification"]
 };
 
 // src/default-widget-inputs.ts
 var MAPPING_EN = /* @__PURE__ */ new Map([
   ["text-classification", [`I like you. I love you`]],
   [
@@ -3843,15 +3861,15 @@
   youtubeId: ""
 };
 var data_default34 = taskData34;
 
 // src/tasks/index.ts
 var TASKS_MODEL_LIBRARIES = {
   "audio-classification": ["speechbrain", "transformers", "transformers.js"],
-  "audio-to-audio": ["asteroid", "speechbrain"],
+  "audio-to-audio": ["asteroid", "fairseq", "speechbrain"],
   "automatic-speech-recognition": ["espnet", "nemo", "speechbrain", "transformers", "transformers.js"],
   "depth-estimation": ["transformers", "transformers.js"],
   "document-question-answering": ["transformers", "transformers.js"],
   "feature-extraction": ["sentence-transformers", "transformers", "transformers.js"],
   "fill-mask": ["transformers", "transformers.js"],
   "graph-ml": ["transformers"],
   "image-classification": ["keras", "timm", "transformers", "transformers.js"],
@@ -5320,15 +5338,15 @@
   return !!model.pipeline_tag && model.pipeline_tag in jsSnippets;
 }
 // Annotate the CommonJS export names for ESM import in node:
 0 && (module.exports = {
   ALL_DISPLAY_MODEL_LIBRARY_KEYS,
   ALL_MODEL_LIBRARY_KEYS,
   InferenceDisplayability,
-  LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS,
+  LIBRARY_TASK_MAPPING,
   MAPPING_DEFAULT_WIDGET,
   MODALITIES,
   MODALITY_LABELS,
   MODEL_LIBRARIES_UI_ELEMENTS,
   PIPELINE_DATA,
   PIPELINE_TYPES,
   PIPELINE_TYPES_SET,
```

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.d.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.d.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1141,21 +1141,21 @@
     };
 };
 type ModelLibraryKey = keyof typeof MODEL_LIBRARIES_UI_ELEMENTS;
 declare const ALL_MODEL_LIBRARY_KEYS: ("sklearn" | "adapter-transformers" | "allennlp" | "asteroid" | "audiocraft" | "bertopic" | "diffusers" | "doctr" | "espnet" | "fairseq" | "fastai" | "fasttext" | "flair" | "gliner" | "grok" | "keras" | "k2" | "mindspore" | "ml-agents" | "mlx" | "mlx-image" | "nemo" | "open_clip" | "paddlenlp" | "peft" | "pyannote-audio" | "pythae" | "sample-factory" | "sentence-transformers" | "setfit" | "spacy" | "span-marker" | "speechbrain" | "stable-baselines3" | "stanza" | "tensorflowtts" | "timm" | "transformers" | "transformers.js" | "unity-sentis" | "whisperkit")[];
 declare const ALL_DISPLAY_MODEL_LIBRARY_KEYS: ("sklearn" | "adapter-transformers" | "allennlp" | "asteroid" | "audiocraft" | "bertopic" | "diffusers" | "doctr" | "espnet" | "fairseq" | "fastai" | "fasttext" | "flair" | "gliner" | "grok" | "keras" | "k2" | "mindspore" | "ml-agents" | "mlx" | "mlx-image" | "nemo" | "open_clip" | "paddlenlp" | "peft" | "pyannote-audio" | "pythae" | "sample-factory" | "sentence-transformers" | "setfit" | "spacy" | "span-marker" | "speechbrain" | "stable-baselines3" | "stanza" | "tensorflowtts" | "timm" | "transformers" | "transformers.js" | "unity-sentis" | "whisperkit")[];
 
 /**
- * Mapping from library name (excluding Transformers) to its supported tasks.
+ * Mapping from library name to its supported tasks.
  * Inference API (serverless) should be disabled for all other (library, task) pairs beyond this mapping.
- * As an exception, we assume Transformers supports all inference tasks.
- * This mapping is generated automatically by "python-api-export-tasks" action in huggingface/api-inference-community repo upon merge.
- * Ref: https://github.com/huggingface/api-inference-community/pull/158
+ * This mapping is partially generated automatically by "python-api-export-tasks" action in
+ * huggingface/api-inference-community repo upon merge. For transformers, the mapping is manually
+ * based on api-inference.
  */
-declare const LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS: Partial<Record<ModelLibraryKey, PipelineType[]>>;
+declare const LIBRARY_TASK_MAPPING: Partial<Record<ModelLibraryKey, PipelineType[]>>;
 
 type PerLanguageMapping = Map<WidgetType, string[] | WidgetExample[]>;
 declare const MAPPING_DEFAULT_WIDGET: Map<string, PerLanguageMapping>;
 
 /**
  * Inference code generated from the JSON schema spec in ./spec
  *
@@ -3467,8 +3467,8 @@
     index_curl as curl,
     index_inputs as inputs,
     index_js as js,
     index_python as python,
   };
 }
 
-export { ALL_DISPLAY_MODEL_LIBRARY_KEYS, ALL_MODEL_LIBRARY_KEYS, AddedToken, AudioClassificationInput, AudioClassificationOutput, AudioClassificationOutputElement, AudioClassificationParameters, AutomaticSpeechRecognitionInput, AutomaticSpeechRecognitionOutput, AutomaticSpeechRecognitionOutputChunk, AutomaticSpeechRecognitionParameters, BoundingBox, ChatCompletionFinishReason, ChatCompletionInput, ChatCompletionInputMessage, ChatCompletionOutput, ChatCompletionOutputChoice, ChatCompletionOutputChoiceMessage, ChatCompletionStreamOutput, ChatCompletionStreamOutputChoice, ChatCompletionStreamOutputDelta, ChatMessage, ClassificationOutputTransform$1 as ClassificationOutputTransform, DepthEstimationInput, DepthEstimationOutput, DocumentQuestionAnsweringInput, DocumentQuestionAnsweringInputData, DocumentQuestionAnsweringOutput, DocumentQuestionAnsweringOutputElement, DocumentQuestionAnsweringParameters, EarlyStoppingUnion$2 as EarlyStoppingUnion, ExampleRepo, FeatureExtractionInput, FeatureExtractionOutput, FillMaskInput, FillMaskOutput, FillMaskOutputElement, FillMaskParameters, GenerationParameters$2 as GenerationParameters, ImageClassificationInput, ImageClassificationOutput, ImageClassificationOutputElement, ImageClassificationParameters, ImageSegmentationInput, ImageSegmentationOutput, ImageSegmentationOutputElement, ImageSegmentationParameters, ImageSegmentationSubtask, ImageToImageInput, ImageToImageOutput, ImageToImageParameters, ImageToTextInput, ImageToTextOutput, ImageToTextParameters, InferenceDisplayability, LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS, LibraryUiElement, MAPPING_DEFAULT_WIDGET, MODALITIES, MODALITY_LABELS, MODEL_LIBRARIES_UI_ELEMENTS, Modality, ModelData, ModelLibraryKey, ObjectDetectionInput, ObjectDetectionOutput, ObjectDetectionOutputElement, ObjectDetectionParameters, PIPELINE_DATA, PIPELINE_TYPES, PIPELINE_TYPES_SET, PipelineData, PipelineType, QuestionAnsweringInput, QuestionAnsweringInputData, QuestionAnsweringOutput, QuestionAnsweringOutputElement, QuestionAnsweringParameters, SPECIAL_TOKENS_ATTRIBUTES, SUBTASK_TYPES, SentenceSimilarityInput, SentenceSimilarityInputData, SentenceSimilarityOutput, SpecialTokensMap, SummarizationInput, SummarizationOutput, TASKS_DATA, TASKS_MODEL_LIBRARIES, TableQuestionAnsweringInput, TableQuestionAnsweringInputData, TableQuestionAnsweringOutput, TableQuestionAnsweringOutputElement, TargetSize$1 as TargetSize, TaskData, TaskDataCustom, TaskDemo, TaskDemoEntry, Text2TextGenerationParameters, Text2TextGenerationTruncationStrategy, TextClassificationInput, TextClassificationOutput, TextClassificationOutputElement, TextClassificationParameters, TextGenerationFinishReason, TextGenerationInput, TextGenerationOutput, TextGenerationOutputDetails, TextGenerationOutputSequenceDetails, TextGenerationOutputToken, TextGenerationParameters, TextGenerationPrefillToken, TextToAudioParameters, TextToImageInput, TextToImageOutput, TextToImageParameters, TextToSpeechInput, TextToSpeechOutput, TokenClassificationAggregationStrategy, TokenClassificationInput, TokenClassificationOutput, TokenClassificationOutputElement, TokenClassificationParameters, TokenizerConfig, TransformersInfo, TranslationInput, TranslationOutput, VideoClassificationInput, VideoClassificationOutput, VideoClassificationOutputElement, VideoClassificationParameters, VisualQuestionAnsweringInput, VisualQuestionAnsweringInputData, VisualQuestionAnsweringOutput, VisualQuestionAnsweringOutputElement, VisualQuestionAnsweringParameters, WidgetExample, WidgetExampleAssetAndPromptInput, WidgetExampleAssetAndTextInput, WidgetExampleAssetAndZeroShotInput, WidgetExampleAssetInput, WidgetExampleAttribute, WidgetExampleChatInput, WidgetExampleOutput, WidgetExampleOutputAnswerScore, WidgetExampleOutputLabels, WidgetExampleOutputText, WidgetExampleOutputUrl, WidgetExampleSentenceSimilarityInput, WidgetExampleStructuredDataInput, WidgetExampleTableDataInput, WidgetExampleTextAndContextInput, WidgetExampleTextAndTableInput, WidgetExampleTextInput, WidgetExampleZeroShotTextInput, WidgetType, WordBox, ZeroShotClassificationInput, ZeroShotClassificationInputData, ZeroShotClassificationOutput, ZeroShotClassificationOutputElement, ZeroShotClassificationParameters, ZeroShotImageClassificationInput, ZeroShotImageClassificationInputData, ZeroShotImageClassificationOutput, ZeroShotImageClassificationOutputElement, ZeroShotImageClassificationParameters, ZeroShotObjectDetectionInput, ZeroShotObjectDetectionInputData, ZeroShotObjectDetectionOutput, ZeroShotObjectDetectionOutputElement, index as snippets };
+export { ALL_DISPLAY_MODEL_LIBRARY_KEYS, ALL_MODEL_LIBRARY_KEYS, AddedToken, AudioClassificationInput, AudioClassificationOutput, AudioClassificationOutputElement, AudioClassificationParameters, AutomaticSpeechRecognitionInput, AutomaticSpeechRecognitionOutput, AutomaticSpeechRecognitionOutputChunk, AutomaticSpeechRecognitionParameters, BoundingBox, ChatCompletionFinishReason, ChatCompletionInput, ChatCompletionInputMessage, ChatCompletionOutput, ChatCompletionOutputChoice, ChatCompletionOutputChoiceMessage, ChatCompletionStreamOutput, ChatCompletionStreamOutputChoice, ChatCompletionStreamOutputDelta, ChatMessage, ClassificationOutputTransform$1 as ClassificationOutputTransform, DepthEstimationInput, DepthEstimationOutput, DocumentQuestionAnsweringInput, DocumentQuestionAnsweringInputData, DocumentQuestionAnsweringOutput, DocumentQuestionAnsweringOutputElement, DocumentQuestionAnsweringParameters, EarlyStoppingUnion$2 as EarlyStoppingUnion, ExampleRepo, FeatureExtractionInput, FeatureExtractionOutput, FillMaskInput, FillMaskOutput, FillMaskOutputElement, FillMaskParameters, GenerationParameters$2 as GenerationParameters, ImageClassificationInput, ImageClassificationOutput, ImageClassificationOutputElement, ImageClassificationParameters, ImageSegmentationInput, ImageSegmentationOutput, ImageSegmentationOutputElement, ImageSegmentationParameters, ImageSegmentationSubtask, ImageToImageInput, ImageToImageOutput, ImageToImageParameters, ImageToTextInput, ImageToTextOutput, ImageToTextParameters, InferenceDisplayability, LIBRARY_TASK_MAPPING, LibraryUiElement, MAPPING_DEFAULT_WIDGET, MODALITIES, MODALITY_LABELS, MODEL_LIBRARIES_UI_ELEMENTS, Modality, ModelData, ModelLibraryKey, ObjectDetectionInput, ObjectDetectionOutput, ObjectDetectionOutputElement, ObjectDetectionParameters, PIPELINE_DATA, PIPELINE_TYPES, PIPELINE_TYPES_SET, PipelineData, PipelineType, QuestionAnsweringInput, QuestionAnsweringInputData, QuestionAnsweringOutput, QuestionAnsweringOutputElement, QuestionAnsweringParameters, SPECIAL_TOKENS_ATTRIBUTES, SUBTASK_TYPES, SentenceSimilarityInput, SentenceSimilarityInputData, SentenceSimilarityOutput, SpecialTokensMap, SummarizationInput, SummarizationOutput, TASKS_DATA, TASKS_MODEL_LIBRARIES, TableQuestionAnsweringInput, TableQuestionAnsweringInputData, TableQuestionAnsweringOutput, TableQuestionAnsweringOutputElement, TargetSize$1 as TargetSize, TaskData, TaskDataCustom, TaskDemo, TaskDemoEntry, Text2TextGenerationParameters, Text2TextGenerationTruncationStrategy, TextClassificationInput, TextClassificationOutput, TextClassificationOutputElement, TextClassificationParameters, TextGenerationFinishReason, TextGenerationInput, TextGenerationOutput, TextGenerationOutputDetails, TextGenerationOutputSequenceDetails, TextGenerationOutputToken, TextGenerationParameters, TextGenerationPrefillToken, TextToAudioParameters, TextToImageInput, TextToImageOutput, TextToImageParameters, TextToSpeechInput, TextToSpeechOutput, TokenClassificationAggregationStrategy, TokenClassificationInput, TokenClassificationOutput, TokenClassificationOutputElement, TokenClassificationParameters, TokenizerConfig, TransformersInfo, TranslationInput, TranslationOutput, VideoClassificationInput, VideoClassificationOutput, VideoClassificationOutputElement, VideoClassificationParameters, VisualQuestionAnsweringInput, VisualQuestionAnsweringInputData, VisualQuestionAnsweringOutput, VisualQuestionAnsweringOutputElement, VisualQuestionAnsweringParameters, WidgetExample, WidgetExampleAssetAndPromptInput, WidgetExampleAssetAndTextInput, WidgetExampleAssetAndZeroShotInput, WidgetExampleAssetInput, WidgetExampleAttribute, WidgetExampleChatInput, WidgetExampleOutput, WidgetExampleOutputAnswerScore, WidgetExampleOutputLabels, WidgetExampleOutputText, WidgetExampleOutputUrl, WidgetExampleSentenceSimilarityInput, WidgetExampleStructuredDataInput, WidgetExampleTableDataInput, WidgetExampleTextAndContextInput, WidgetExampleTextAndTableInput, WidgetExampleTextInput, WidgetExampleZeroShotTextInput, WidgetType, WordBox, ZeroShotClassificationInput, ZeroShotClassificationInputData, ZeroShotClassificationOutput, ZeroShotClassificationOutputElement, ZeroShotClassificationParameters, ZeroShotImageClassificationInput, ZeroShotImageClassificationInputData, ZeroShotImageClassificationOutput, ZeroShotImageClassificationOutputElement, ZeroShotImageClassificationParameters, ZeroShotObjectDetectionInput, ZeroShotObjectDetectionInputData, ZeroShotObjectDetectionOutput, ZeroShotObjectDetectionOutputElement, index as snippets };
```

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.js` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/dist/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         __defProp(target, name, {
             get: all[name],
             enumerable: true
         });
 };
 
 // src/library-to-tasks.ts
-var LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS = {
+var LIBRARY_TASK_MAPPING = {
     "adapter-transformers": ["question-answering", "text-classification", "token-classification"],
     allennlp: ["question-answering"],
     asteroid: [
         // "audio-source-separation",
         "audio-to-audio"
     ],
     bertopic: ["text-classification"],
@@ -40,14 +40,32 @@
         "audio-to-audio",
         "automatic-speech-recognition",
         "text-to-speech",
         "text2text-generation"
     ],
     stanza: ["token-classification"],
     timm: ["image-classification"],
+    transformers: [
+        "audio-classification",
+        "automatic-speech-recognition",
+        "depth-estimation",
+        "document-question-answering",
+        "fill-mask",
+        "image-classification",
+        "image-segmentation",
+        "image-to-text",
+        "image-to-image",
+        "object-detection",
+        "question-answering",
+        "text-generation",
+        "text2text-generation",
+        "visual-question-answering",
+        "zero-shot-classification",
+        "zero-shot-image-classification"
+    ],
     mindspore: ["image-classification"]
 };
 
 // src/default-widget-inputs.ts
 var MAPPING_EN = /* @__PURE__ */ new Map([
     ["text-classification", [`I like you. I love you`]],
     [
@@ -3045,15 +3063,15 @@
     youtubeId: ""
 };
 var data_default34 = taskData34;
 
 // src/tasks/index.ts
 var TASKS_MODEL_LIBRARIES = {
     "audio-classification": ["speechbrain", "transformers", "transformers.js"],
-    "audio-to-audio": ["asteroid", "speechbrain"],
+    "audio-to-audio": ["asteroid", "fairseq", "speechbrain"],
     "automatic-speech-recognition": ["espnet", "nemo", "speechbrain", "transformers", "transformers.js"],
     "depth-estimation": ["transformers", "transformers.js"],
     "document-question-answering": ["transformers", "transformers.js"],
     "feature-extraction": ["sentence-transformers", "transformers", "transformers.js"],
     "fill-mask": ["transformers", "transformers.js"],
     "graph-ml": ["transformers"],
     "image-classification": ["keras", "timm", "transformers", "transformers.js"],
@@ -4588,15 +4606,15 @@
 function hasJsInferenceSnippet(model) {
     return !!model.pipeline_tag && model.pipeline_tag in jsSnippets;
 }
 export {
     ALL_DISPLAY_MODEL_LIBRARY_KEYS,
     ALL_MODEL_LIBRARY_KEYS,
     InferenceDisplayability,
-    LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS,
+    LIBRARY_TASK_MAPPING,
     MAPPING_DEFAULT_WIDGET,
     MODALITIES,
     MODALITY_LABELS,
     MODEL_LIBRARIES_UI_ELEMENTS,
     PIPELINE_DATA,
     PIPELINE_TYPES,
     PIPELINE_TYPES_SET,
```

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/package.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9150883838383839%*

 * *Differences: {"'_id'": "'@huggingface/tasks@0.7.0'",*

 * * "'_integrity'": "'sha512-vOHd5hnbfPWlxmH2jW1FD55TckwuXb9VMAaNHYSvj5bjUn5O9uwez0XdPJBK9wkB0V46aWZs0jcqlEnvIvQwCw=='",*

 * * "'_npmOperationalInternal'": "{'tmp': 'tmp/tasks_0.7.0_1712042147160_0.3654645127547085'}",*

 * * "'_resolved'": "'https://registry.npmjs.org/@huggingface/tasks/-/tasks-0.7.0.tgz'",*

 * * "'_shasum'": "'304c38ef75ec1557bd91e96db9b0887b2d3a1579'",*

 * * "'dist'": "{'integrity': "*

 * *           "'sha512-vOHd5hnbfPWlxmH2jW1FD55TckwuXb9VMAaNHYSvj5bjUn5O9uwez0XdPJBK9wkB0V46 […]*

```diff
@@ -1,48 +1,48 @@
 {
     "_from": "@huggingface/tasks@>=0.3.0",
     "_hasShrinkwrap": false,
-    "_id": "@huggingface/tasks@0.6.1",
-    "_integrity": "sha512-tsT8O3xBzZke0ZbFTnCgrJWIDWe3hlt2IWp2cRiynXWZzJwE2NfULPMb4157rdp3xZ7gIgneMnYdesr8d3DzmA==",
+    "_id": "@huggingface/tasks@0.7.0",
+    "_integrity": "sha512-vOHd5hnbfPWlxmH2jW1FD55TckwuXb9VMAaNHYSvj5bjUn5O9uwez0XdPJBK9wkB0V46aWZs0jcqlEnvIvQwCw==",
     "_nodeVersion": "20.11.1",
     "_npmOperationalInternal": {
         "host": "s3://npm-registry-packages",
-        "tmp": "tmp/tasks_0.6.1_1711402682920_0.019089037073535486"
+        "tmp": "tmp/tasks_0.7.0_1712042147160_0.3654645127547085"
     },
     "_npmUser": {
         "email": "coyotte508@gmail.com",
         "name": "coyotte508"
     },
     "_npmVersion": "10.2.4",
-    "_resolved": "https://registry.npmjs.org/@huggingface/tasks/-/tasks-0.6.1.tgz",
-    "_shasum": "fcbd40e6fd9b13dfada9f5274c4ca044ffd2cbad",
+    "_resolved": "https://registry.npmjs.org/@huggingface/tasks/-/tasks-0.7.0.tgz",
+    "_shasum": "304c38ef75ec1557bd91e96db9b0887b2d3a1579",
     "author": {
         "name": "Hugging Face"
     },
     "bugs": {
         "url": "https://github.com/huggingface/huggingface.js/issues"
     },
     "description": "List of ML tasks for huggingface.co/tasks",
     "devDependencies": {
         "@types/node": "^20.11.5",
         "quicktype-core": "https://github.com/huggingface/quicktype/raw/pack-18.0.17/packages/quicktype-core/quicktype-core-18.0.17.tgz"
     },
     "directories": {},
     "dist": {
         "fileCount": 184,
-        "integrity": "sha512-tsT8O3xBzZke0ZbFTnCgrJWIDWe3hlt2IWp2cRiynXWZzJwE2NfULPMb4157rdp3xZ7gIgneMnYdesr8d3DzmA==",
-        "shasum": "fcbd40e6fd9b13dfada9f5274c4ca044ffd2cbad",
+        "integrity": "sha512-vOHd5hnbfPWlxmH2jW1FD55TckwuXb9VMAaNHYSvj5bjUn5O9uwez0XdPJBK9wkB0V46aWZs0jcqlEnvIvQwCw==",
+        "shasum": "304c38ef75ec1557bd91e96db9b0887b2d3a1579",
         "signatures": [
             {
                 "keyid": "SHA256:jl3bwswu80PjjokCgh0o2w5c2U4LhQAE57gj9cz1kzA",
-                "sig": "MEUCIQCOaxke8bcmZDhpMhZqVzVIk/nyo8lYsJBM20dtYohwrQIgBMsZV/ExKCw12pyzBsnc5Au/MUFjff21EsmifIPiGcY="
+                "sig": "MEYCIQC1uo6UObtO3CnmHhU8zV2akwnPolaqUenMv6hfkB2plgIhALn/L+aINqe2nE7B+BV1GbtnmIlMVYkY2TQO8hRJpy8D"
             }
         ],
-        "tarball": "https://registry.npmjs.org/@huggingface/tasks/-/tasks-0.6.1.tgz",
-        "unpackedSize": 1002509
+        "tarball": "https://registry.npmjs.org/@huggingface/tasks/-/tasks-0.7.0.tgz",
+        "unpackedSize": 1003492
     },
     "exports": {
         ".": {
             "import": "./dist/index.js",
             "require": "./dist/index.cjs",
             "types": "./dist/index.d.ts"
         }
@@ -92,9 +92,9 @@
         "inference-codegen": "tsx scripts/inference-codegen.ts && prettier --write src/tasks/*/inference.ts",
         "lint": "eslint --quiet --fix --ext .cjs,.ts .",
         "lint:check": "eslint --ext .cjs,.ts ."
     },
     "source": "src/index.ts",
     "type": "module",
     "types": "./dist/index.d.ts",
-    "version": "0.6.1"
+    "version": "0.7.0"
 }
```

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/default-widget-inputs.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/default-widget-inputs.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/index.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/index.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-export { LIBRARY_TASK_MAPPING_EXCLUDING_TRANSFORMERS } from "./library-to-tasks";
+export { LIBRARY_TASK_MAPPING } from "./library-to-tasks";
 export { MAPPING_DEFAULT_WIDGET } from "./default-widget-inputs";
 export type { TaskData, TaskDemo, TaskDemoEntry, ExampleRepo } from "./tasks";
 export * from "./tasks";
 export {
 	PIPELINE_DATA,
 	PIPELINE_TYPES,
 	type WidgetType,
```

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries-downloads.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries-downloads.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries-snippets.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries-snippets.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/model-libraries.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/pipelines.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/pipelines.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/curl.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/curl.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/inputs.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/inputs.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/js.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/js.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/python.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/snippets/python.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-classification/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/audio-to-audio/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/automatic-speech-recognition/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/output_stream.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/chat-completion/spec/output_stream.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/common-definitions.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/common-definitions.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/depth-estimation/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/document-question-answering/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/feature-extraction/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/fill-mask/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-classification/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-segmentation/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-image/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/image-to-text/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/index.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/index.ts`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 import type { ModelLibraryKey } from "../model-libraries";
 
 /**
  * Model libraries compatible with each ML task
  */
 export const TASKS_MODEL_LIBRARIES: Record<PipelineType, ModelLibraryKey[]> = {
 	"audio-classification": ["speechbrain", "transformers", "transformers.js"],
-	"audio-to-audio": ["asteroid", "speechbrain"],
+	"audio-to-audio": ["asteroid", "fairseq", "speechbrain"],
 	"automatic-speech-recognition": ["espnet", "nemo", "speechbrain", "transformers", "transformers.js"],
 	"depth-estimation": ["transformers", "transformers.js"],
 	"document-question-answering": ["transformers", "transformers.js"],
 	"feature-extraction": ["sentence-transformers", "transformers", "transformers.js"],
 	"fill-mask": ["transformers", "transformers.js"],
 	"graph-ml": ["transformers"],
 	"image-classification": ["keras", "timm", "transformers", "transformers.js"],
```

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/mask-generation/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/object-detection/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/placeholder/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/question-answering/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/reinforcement-learning/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/sentence-similarity/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/summarization/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/table-question-answering/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-classification/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/tabular-regression/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-classification/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/output_stream.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-generation/spec/output_stream.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-audio/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-image/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-speech/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text-to-video/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/text2text-generation/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/token-classification/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/translation/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/unconditional-image-generation/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/video-classification/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/visual-question-answering/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-classification/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/about.md` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/about.md`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/inference.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/inference.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/input.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/input.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/output.json` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/output.json`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tokenizer-data.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tokenizer-data.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/widget-example.ts` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/widget-example.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts/huggingface/remote_schema_retriever.py` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts/huggingface/remote_schema_retriever.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,42 +35,64 @@
             RuntimeError: If the sample data from huggingface failed to be loaded.
         """
         self.__validate_task_support(task)
         hugging_face_demo_data = self.__retrieve_hf_demo_data_for_task(task)
         sample_inputs, sample_outputs = dict(), [dict()]
         try:
             input_data, output_data = hugging_face_demo_data['inputs'], hugging_face_demo_data['outputs']
-            for item in input_data:
-                processed_item = dict(item)
-                self.__add_image_or_audio_sample(processed_item)
-                if 'label' in processed_item:
-                    label = processed_item['label'].lower()
-                    if label.lower() == 'input':
-                        label = 'inputs'
-                    sample_inputs[label] = processed_item['content']
-                elif 'filename' in processed_item:
-                    sample_inputs['inputs'] = processed_item['path']
-                    sample_inputs['type'] = processed_item['type']
-                else:
-                    raise KeyError(f"Sample input data for task {task} from huggingface contained invalid property: "
-                                   f"{processed_item}.")
-            for item in output_data:
-                processed_item = dict(item)
-                self.__add_image_or_audio_sample(processed_item)
-                if 'label' in processed_item:
-                    label = processed_item['label'].lower()
-                    if label.lower() == 'transcript':
-                        label = 'output'
-                    sample_outputs[0][label] = processed_item['content']
-                elif 'filename' in processed_item:
-                    sample_outputs[0]['output'] = processed_item['path']
-                    sample_outputs[0]['type'] = processed_item['type']
-                else:
-                    raise KeyError(f"Sample output data for task {task} from huggingface contained invalid property: "
-                                   f"{processed_item}.")
+            if task in ('question-answering', 'text-to-image', 'automatic-speech-recognition'):
+                for item in input_data:
+                    processed_item = dict(item)
+                    if 'type' in item.keys() and item['type'] in ('img', 'audio'):
+                        sample_inputs = self.__sanitize_image_or_audio_sample(processed_item)
+                    elif 'label' in processed_item:
+                        label = processed_item['label'].lower()
+                        if label.lower() == 'input':
+                            label = 'inputs'
+                        sample_inputs[label] = processed_item['content']
+                    else:
+                        raise KeyError(
+                            f"Sample input data for task {task} from huggingface contained invalid property: "
+                            f"{processed_item}.")
+                for item in output_data:
+                    processed_item = dict(item)
+                    if 'type' in item.keys() and item['type'] in ('img', 'audio'):
+                        sample_outputs[0] = self.__sanitize_image_or_audio_sample(processed_item)
+                    elif 'label' in processed_item:
+                        label = processed_item['label'].lower()
+                        if label.lower() == 'transcript':
+                            label = 'output'
+                        sample_outputs[0][label] = processed_item['content']
+                    else:
+                        raise KeyError(
+                            f"Sample output data for task {task} from huggingface contained invalid property: "
+                            f"{processed_item}.")
+            if task == "fill-mask":
+                for item in input_data:
+                    processed_item = dict(item)
+                    if 'label' in processed_item and processed_item['label'].lower() == 'input':
+                        sample_inputs['inputs'] = processed_item['content'].replace('<mask>', '[MASK]')
+                    else:
+                        raise RuntimeError(f"Sample input data for task {task} from huggingface contained invalid "
+                                           f"property: {processed_item}.")
+                for item in output_data:
+                    processed_item = dict(item)
+                    if 'type' in item and item['type'] == 'chart':
+                        try:
+                            if 'data' in item and isinstance(item['data'], list):
+                                options = list(item['data'])
+                                options.sort(key=lambda op: -float(op['score']))
+                                sample_outputs[0]['sequence'] = (
+                                    sample_inputs['inputs'].replace('[MASK]', options[0]['label']))
+                                sample_outputs[0]['score'] = options[0]['score']
+                        except KeyError as e:
+                            raise RuntimeError(f"Unable to infer output sample from {task} data for huggingface. {e}")
+                    else:
+                        raise RuntimeError(f"Sample output data for task {task} from huggingface contained invalid "
+                                           f"property: {processed_item}.")
             if not sample_inputs or not sample_outputs:
                 raise RuntimeError(f"Sample data for task {task} could not be loaded.")
             return sample_inputs, sample_outputs
         except KeyError as e:
             raise RuntimeError(f"Sample data for task {task} from huggingface was invalid. KeyError: {e}")
 
     def get_src_dir(self) -> str:
@@ -120,33 +142,35 @@
 
         Raises:
             ValueError: If the task is not supported.
         """
         if task not in SUPPORTED_TASKS:
             raise ValueError(f"Task {task} is not supported. Supported tasks are: {', '.join(SUPPORTED_TASKS)}")
 
-    def __add_image_or_audio_sample(self, item: dict[str, Any]) -> None:
-        """Adds an image or audio file and path if needed
+    def __sanitize_image_or_audio_sample(self, item: dict[str, Any]) -> dict[str, Any]:
+        """Constructs the image/audio sample dict for use with SchemaBuilder
 
         Args:
-            item (dict[str,Any]): Unaltered HuggingFace object
+            item (dict[str,Any]): Unaltered HuggingFace object with "data" (raw bytes)
+            and "content_type" (for interpretation)
 
         Raises:
             RuntimeError: If the sample image or audio files are not found.
         """
-        if 'type' in item.keys():
-            if item['type'] == 'img':
-                item['filename'] = SAMPLE_IMAGE
-                img = os.path.join(self.__src_dir, PATH_TO_SAMPLE_IMAGE, SAMPLE_IMAGE)
-                try:
-                    with open(img) as _:  # Validate file exists
-                        item['path'] = img
-                except FileNotFoundError as e:
-                    raise RuntimeError(f"File '{SAMPLE_IMAGE}' was not found. {e}")
-            elif item['type'] == 'audio':
-                item['filename'] = SAMPLE_AUDIO
-                audio = os.path.join(self.__src_dir, PATH_TO_SAMPLE_AUDIO, SAMPLE_AUDIO)
-                try:
-                    with open(audio) as _:  # Validate file exists
-                        item['path'] = audio
-                except FileNotFoundError as e:
-                    raise RuntimeError(f"File '{SAMPLE_AUDIO}' was not found. {e}")
+        processed_item = dict()
+        if item['type'] == 'img':
+            img = os.path.join(self.__src_dir, PATH_TO_SAMPLE_IMAGE, SAMPLE_IMAGE)
+            try:
+                with open(img, 'rb') as raw_image:  # Validate file exists
+                    processed_item['data'] = raw_image.read()
+                    processed_item['content_type'] = 'image/png'
+            except FileNotFoundError as e:
+                raise RuntimeError(f"File '{SAMPLE_IMAGE}' was not found. {e}")
+        elif item['type'] == 'audio':
+            audio = os.path.join(self.__src_dir, PATH_TO_SAMPLE_AUDIO, SAMPLE_AUDIO)
+            try:
+                with open(audio, 'rb') as raw_audio:  # Validate file exists
+                    processed_item['data'] = raw_audio.read()
+                    processed_item['content_type'] = 'audio/x-audio'
+            except FileNotFoundError as e:
+                raise RuntimeError(f"File '{SAMPLE_AUDIO}' was not found. {e}")
+        return processed_item
```

### Comparing `sagemaker-schema-inference-artifacts-0.0.2/src/sagemaker_schema_inference_artifacts.egg-info/SOURCES.txt` & `sagemaker-schema-inference-artifacts-0.0.4/src/sagemaker_schema_inference_artifacts.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -202,9 +202,9 @@
 src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/input.json
 src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-image-classification/spec/output.json
 src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/about.md
 src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/data.ts
 src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/inference.ts
 src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/input.json
 src/sagemaker_schema_inference_artifacts/huggingface/node_modules/@huggingface/tasks/src/tasks/zero-shot-object-detection/spec/output.json
-src/sagemaker_schema_inference_artifacts/huggingface/sample_data/audio/mp3.mp3
+src/sagemaker_schema_inference_artifacts/huggingface/sample_data/audio/sample.flac
 src/sagemaker_schema_inference_artifacts/huggingface/sample_data/image/png-truncated.png
```

