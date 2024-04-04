# Comparing `tmp/langfun-0.0.2.dev20240403.tar.gz` & `tmp/langfun-0.0.2.dev20240404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240403.tar", last modified: Wed Apr  3 08:03:47 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240404.tar", last modified: Thu Apr  4 08:04:19 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240403.tar` & `langfun-0.0.2.dev20240404.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.417411 langfun-0.0.2.dev20240403/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-03 08:03:47.417411 langfun-0.0.2.dev20240403/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.401411 langfun-0.0.2.dev20240403/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.405411 langfun-0.0.2.dev20240403/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.405411 langfun-0.0.2.dev20240403/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.409412 langfun-0.0.2.dev20240403/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.409412 langfun-0.0.2.dev20240403/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54730 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21083 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.409412 langfun-0.0.2.dev20240403/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.409412 langfun-0.0.2.dev20240403/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.409412 langfun-0.0.2.dev20240403/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.413411 langfun-0.0.2.dev20240403/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.413411 langfun-0.0.2.dev20240403/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19249 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19129 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25020 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.417411 langfun-0.0.2.dev20240403/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:03:47.417411 langfun-0.0.2.dev20240403/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-03 08:03:47.000000 langfun-0.0.2.dev20240403/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-03 08:03:47.000000 langfun-0.0.2.dev20240403/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:03:47.000000 langfun-0.0.2.dev20240403/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 08:03:47.000000 langfun-0.0.2.dev20240403/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 08:03:47.000000 langfun-0.0.2.dev20240403/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:03:47.417411 langfun-0.0.2.dev20240403/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 08:03:21.000000 langfun-0.0.2.dev20240403/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.041835 langfun-0.0.2.dev20240404/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-04 08:04:19.041835 langfun-0.0.2.dev20240404/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.021836 langfun-0.0.2.dev20240404/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.029836 langfun-0.0.2.dev20240404/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.029836 langfun-0.0.2.dev20240404/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.033836 langfun-0.0.2.dev20240404/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.033836 langfun-0.0.2.dev20240404/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54730 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21083 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.033836 langfun-0.0.2.dev20240404/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.033836 langfun-0.0.2.dev20240404/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.037835 langfun-0.0.2.dev20240404/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.037835 langfun-0.0.2.dev20240404/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.041835 langfun-0.0.2.dev20240404/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19249 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19610 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25020 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.041835 langfun-0.0.2.dev20240404/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:04:19.041835 langfun-0.0.2.dev20240404/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-04 08:04:18.000000 langfun-0.0.2.dev20240404/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-04 08:04:18.000000 langfun-0.0.2.dev20240404/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:04:18.000000 langfun-0.0.2.dev20240404/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 08:04:18.000000 langfun-0.0.2.dev20240404/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 08:04:18.000000 langfun-0.0.2.dev20240404/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 08:04:19.041835 langfun-0.0.2.dev20240404/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-04 08:04:02.000000 langfun-0.0.2.dev20240404/setup.py
```

### Comparing `langfun-0.0.2.dev20240403/LICENSE` & `langfun-0.0.2.dev20240404/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/PKG-INFO` & `langfun-0.0.2.dev20240404/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240403
+Version: 0.0.2.dev20240404
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240403/README.md` & `langfun-0.0.2.dev20240404/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/__init__.py` & `langfun-0.0.2.dev20240404/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/correction.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Python code error correction."""
-import re
 from typing import Any
 import langfun.core as lf
 from langfun.core.coding.python import errors
 from langfun.core.coding.python import execution
 import pyglove as pg
 
 
@@ -27,19 +26,14 @@
   error: str
 
 
 class CorrectedCode(pg.Object):
   corrected_code: str
 
 
-def remove_docstrings(code):
-  pattern = re.compile(r"(def .+?:\s*?)('''|\"\"\")((.|\s)*?)(\2)", re.DOTALL)
-  return pattern.sub(r"\1", code)
-
-
 def run_with_correction(
     code: str,
     error: str | None = None,
     *,
     global_vars: dict[str, Any] | None = None,
     lm: lf.LanguageModel | None = None,
     max_attempts: int = 5,
@@ -82,15 +76,14 @@
   # Delay import at runtime to avoid circular depenency.
   # pylint: disable=g-import-not-at-top
   # pytype: disable=import-error
   from langfun.core.structured import prompting
   # pytype: enable=import-error
   # pylint: enable=g-import-not-at-top
 
-  code = remove_docstrings(code)
   if max_attempts == 0:
     result = execution.run(
         code,
         global_vars=global_vars,
         sandbox=sandbox,
         timeout=timeout,
         outputs_intermediate=outputs_intermediate,
```

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240404/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/component.py` & `langfun-0.0.2.dev20240404/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/component_test.py` & `langfun-0.0.2.dev20240404/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240404/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240404/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/console.py` & `langfun-0.0.2.dev20240404/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/console_test.py` & `langfun-0.0.2.dev20240404/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240404/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240404/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240404/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240404/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240404/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240404/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240404/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240404/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/language_model.py` & `langfun-0.0.2.dev20240404/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240404/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240404/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240404/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240404/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/memory.py` & `langfun-0.0.2.dev20240404/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/message.py` & `langfun-0.0.2.dev20240404/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/message_test.py` & `langfun-0.0.2.dev20240404/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240404/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240404/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240404/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240404/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240404/langfun/core/modalities/video.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Video modality."""
 
 import base64
 from typing import cast
-
 from langfun.core.modalities import mime
-import magic
 
 
 class Video(mime.MimeType):
   """Base class for Video."""
 
   @property
   def video_format(self) -> str:
     return cast(str, self.mime_type.lstrip('video/'))
 
   @property
   def mime_type(self) -> str:
+    # TODO(daiyip): after cl/619658455, LaunchPad binaries cannot import `magic`
+    # correctly. This is to mitigate the issue for major Langfun users who do
+    # not use Video. We shall move this import out once the issue is fixed.
+    import magic  # pylint: disable=g-import-not-at-top
+
     video_mime_type = magic.from_buffer(self.to_bytes(), mime=True)
     if 'video/' not in video_mime_type:
       raise ValueError(f'Not a video: {video_mime_type!r}.')
     return video_mime_type
 
   def _repr_html_(self) -> str:
     if self.uri and self.uri.lower().startswith(('http:', 'https:', 'ftp:')):
```

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240404/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modality.py` & `langfun-0.0.2.dev20240404/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240404/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240404/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240404/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/sampling.py` & `langfun-0.0.2.dev20240404/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240404/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """The base of symbolic mapping methods."""
 
 import io
-from typing import Annotated, Any
+from typing import Annotated, Any, Callable
 import langfun.core as lf
 from langfun.core.structured import schema as schema_lib
 import pyglove as pg
 
 
 @pg.use_init_args(['input', 'output', 'schema', 'context'])
 class MappingExample(lf.NaturalLanguageFormattable, lf.Component):
@@ -274,14 +274,22 @@
       (
           'The default value to use if the LM response is not a valid code '
           'based on the schema (after autofix). '
           'If unspecified, error will be raisen.'
       ),
   ] = lf.RAISE_IF_HAS_ERROR
 
+  response_postprocess: Annotated[
+      Callable[[str], str] | None,
+      (
+          'A callable object that post process the raw LLM response before '
+          'parsing it into the output Python object.'
+      )
+  ] = None
+
   #
   # Key methods for implementing specific mappings.
   #
 
   def transform_input(self, lm_input: lf.Message) -> lf.Message:
     # Find modalities to fill the input message.
     lm_input.metadata.update(
@@ -292,14 +300,15 @@
     if isinstance(self.input, lf.Message):
       lm_input.source = self.input
     return lm_input
 
   def transform_output(self, lm_output: lf.Message) -> lf.Message:
     """Transforms LM response into structure if schema is present."""
     try:
+      lm_output = self.postprocess_response(lm_output)
       lm_output.result = self.postprocess_result(self.parse_result(lm_output))
     except Exception as e:  # pylint: disable=broad-exception-caught
       if self.default == lf.RAISE_IF_HAS_ERROR:
         raise e
       lm_output.result = self.default
     return lm_output
 
@@ -312,14 +321,22 @@
         lm_output.text,
         protocol=self.protocol,
         additional_context=self.globals(),
         autofix=self.autofix,
         autofix_lm=self.autofix_lm or self.lm,
     )
 
+  def postprocess_response(self, response: lf.Message) -> lf.Message:
+    """Post process LLM response."""
+    if self.response_postprocess is not None:
+      postprocessed_text = self.response_postprocess(response.text)
+      if postprocessed_text != response.text:
+        return lf.AIMessage(postprocessed_text, source=response)
+    return response
+
   def postprocess_result(self, result: Any) -> Any:
     """Post process structured output."""
     return result
 
   def globals(self) -> dict[str, Any]:
     """Gets additional symbol definitions besides schema as globals."""
     return {'ModalityRef': lf.modality.ModalityRef}
```

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/prompting.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Symbolic query."""
 
-from typing import Any, Type, Union
+from typing import Any, Callable, Type, Union
 
 import langfun.core as lf
 from langfun.core.structured import mapping
 from langfun.core.structured import schema as schema_lib
 import pyglove as pg
 
 
@@ -103,14 +103,15 @@
         schema_lib.Schema, Type[Any], list[Type[Any]], dict[str, Any], None
     ] = None,
     default: Any = lf.RAISE_IF_HAS_ERROR,
     *,
     lm: lf.LanguageModel | None = None,
     examples: list[mapping.MappingExample] | None = None,
     cache_seed: int | None = 0,
+    response_postprocess: Callable[[str], str] | None = None,
     autofix: int = 0,
     autofix_lm: lf.LanguageModel | None = None,
     protocol: schema_lib.SchemaProtocol = 'python',
     returns_message: bool = False,
     skip_lm: bool = False,
     **kwargs,
 ) -> Any:
@@ -155,14 +156,17 @@
     lm: The language model to use. If not specified, the language model from
       `lf.context` context manager will be used.
     examples: An optional list of fewshot examples for helping parsing. If None,
       the default one-shot example will be added.
     cache_seed: Seed for computing cache key. The cache key is determined by a
       tuple of (lm, prompt, cache seed). If None, cache will be disabled for
       the query even cache is configured by the LM.
+    response_postprocess: An optional callable object to process the raw LM
+      response before parsing it into the final output object. If None, the
+      raw LM response will not be processed.
     autofix: Number of attempts to auto fix the generated code. If 0, autofix is
       disabled. Auto-fix is not supported for 'json' protocol.
     autofix_lm: The language model to use for autofix. If not specified, the
       `autofix_lm` from `lf.context` context manager will be used. Otherwise it
       will use `lm`.
     protocol: The protocol for schema/value representation. Applicable values
       are 'json' and 'python'. By default `python` will be used.
@@ -184,14 +188,18 @@
     schema = prompt.__class__
 
   if schema in (None, str):
     # Query with natural language output.
     output = lf.LangFunc.from_value(prompt, **kwargs)(
         lm=lm, cache_seed=cache_seed, skip_lm=skip_lm
     )
+    if response_postprocess:
+      processed_text = response_postprocess(output.text)
+      if processed_text != output.text:
+        output = lf.AIMessage(processed_text, source=output)
     return output if returns_message else output.text
 
   # Query with structured output.
   if isinstance(prompt, str):
     prompt = lf.Template(prompt, **kwargs)
   elif isinstance(prompt, lf.Template):
     prompt = prompt.rebind(**kwargs)
@@ -202,14 +210,15 @@
     prompt = schema_lib.mark_missing(prompt)
 
   output = _query_structure_cls(protocol)(
       input=prompt,
       schema=schema,
       default=default,
       examples=examples,
+      response_postprocess=response_postprocess,
       autofix=autofix if protocol == 'python' else 0,
       **kwargs,
   )(
       lm=lm,
       autofix_lm=autofix_lm or lm,
       cache_seed=cache_seed,
       skip_lm=skip_lm,
```

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/prompting_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -432,14 +432,31 @@
             CorrectedCode(
                 corrected_code='1',
             )
             """),
     ])
     self.assertEqual(prompting.query('what is 1 + 0', int, lm=lm, autofix=3), 1)
 
+  def test_response_postprocess(self):
+    with lf.context(
+        lm=fake.StaticResponse('<!-- some comment-->\n3'),
+        override_attrs=True,
+    ):
+      self.assertEqual(
+          prompting.query(
+              'Compute 1 + 2', response_postprocess=lambda x: x.split('\n')[1]),
+          '3'
+      )
+      self.assertEqual(
+          prompting.query(
+              'Compute 1 + 2', int,
+              response_postprocess=lambda x: x.split('\n')[1]),
+          3
+      )
+
 
 class QueryStructureJsonTest(unittest.TestCase):
 
   def test_render_no_examples(self):
     l = prompting.QueryStructureJson(
         input=lf.AIMessage('Compute 12 / 6 + 2.'), schema=int
     )
```

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240404/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/subscription.py` & `langfun-0.0.2.dev20240404/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240404/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/template.py` & `langfun-0.0.2.dev20240404/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/template_test.py` & `langfun-0.0.2.dev20240404/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240404/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240404/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240404/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240404/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240403
+Version: 0.0.2.dev20240404
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240403/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240404/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240403/setup.py` & `langfun-0.0.2.dev20240404/setup.py`

 * *Files identical despite different names*

