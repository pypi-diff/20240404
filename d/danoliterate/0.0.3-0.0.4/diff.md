# Comparing `tmp/danoliterate-0.0.3.tar.gz` & `tmp/danoliterate-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danoliterate-0.0.3.tar", last modified: Mon Jan 15 19:44:09 2024, max compression
+gzip compressed data, was "danoliterate-0.0.4.tar", last modified: Thu Apr  4 20:52:34 2024, max compression
```

## Comparing `danoliterate-0.0.3.tar` & `danoliterate-0.0.4.tar`

### file list

```diff
@@ -1,364 +1,529 @@
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.955270 danoliterate-0.0.3/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/.github/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.911937 danoliterate-0.0.3/.github/workflows/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1113 2024-01-11 21:05:30.000000 danoliterate-0.0.3/.github/workflows/is_it_tidy.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       77 2024-01-11 21:05:31.000000 danoliterate-0.0.3/MANIFEST.in
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2507 2024-01-15 19:44:09.955270 danoliterate-0.0.3/PKG-INFO
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      567 2024-01-11 21:05:31.000000 danoliterate-0.0.3/README.md
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.911937 danoliterate-0.0.3/danoliterate/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3022 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/__main__.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.911937 danoliterate-0.0.3/danoliterate/configs/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.911937 danoliterate-0.0.3/danoliterate/configs/databuild/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      253 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/databuild/citizenship_test.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      294 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/databuild/da_cloze_self_test.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       90 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/databuild/da_gym_2000.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      178 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/databuild/hashtag_twitterhjerne.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      220 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/databuild/hyggeswag.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      158 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/databuild/nordjylland_news.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       96 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/databuild/prompt_answer.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1349 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/master.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.918604 danoliterate-0.0.3/danoliterate/configs/model/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       56 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/baseline.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      146 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/danoliterate-baseline.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      152 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/danoliterate-llama.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      154 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/danoliterate-mistral.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       67 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/danskgpt-api.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       87 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/danskgpt-tiny.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       58 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/danskgpt.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       77 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/google-gemini-pro.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       92 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/gpt-neo-da.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       81 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/gpt-neox-da.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      106 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/gpt-sw3-20b-instruct.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/gpt-sw3-20b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      118 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/gpt-sw3-6b-instruct.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      100 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/gpt-sw3-6b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/hestenet-lm.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       89 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/kanelsnegl.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       95 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/llama2-13b-chat.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       85 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/llama2-13b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      133 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/llama2-70b-chat.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      123 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/llama2-70b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       93 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/llama2-7b-chat.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       83 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/llama2-7b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       76 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/mgpt-13b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       68 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/mgpt.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      109 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/mistral-7b-instruct-v0.2.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      102 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/mistral-7b-instruct.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       84 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/mistral-7b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      144 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/mixtral-8-7b-instruct.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      126 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/mixtral-8-7b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       92 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/nb-gpt-j-norpaca.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       76 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/nb-gpt-j.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       43 2024-01-15 19:42:53.000000 danoliterate-0.0.3/danoliterate/configs/model/new.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       76 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/openai-ada-001.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       79 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/openai-babbage-002.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       79 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/openai-davinci-002.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       84 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/openai-davinci-003.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      101 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/openai-gpt-3.5-turbo-instruct.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       86 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/openai-gpt-4-turbo.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       67 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/openai-gpt-4.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       83 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/openai-gpt-turbo.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      102 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/solar-11b-instruct.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       84 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/solar-11b.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       99 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/model/test.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.918604 danoliterate-0.0.3/danoliterate/configs/scenarios/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      391 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/angry-tweets.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      332 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/citizenship-test-free.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      294 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/citizenship-test-simple.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      369 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/citizenship-test.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      365 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/da-cloze-self-test-free.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      375 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/da-cloze-self-test.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      405 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/da-gym-2000-english.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      299 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/da-gym-2000-free.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      377 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/da-gym-2000.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      569 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/dane-1.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      569 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/dane-5.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      517 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/dane.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      412 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/hashtag-twitterhjerne.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      266 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/hyggeswag-free.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      361 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/hyggeswag.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      765 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/nordjylland-news-detailed-prompt.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      393 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/nordjylland-news.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      123 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/scenarios/prompt-answer.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.918604 danoliterate-0.0.3/danoliterate/configs/train/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      780 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/train/default.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      803 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/configs/train/test.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.918604 danoliterate-0.0.3/danoliterate/data/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/__init__.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.921937 danoliterate-0.0.3/danoliterate/data/building/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)    11349 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/citizenship_test_da.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3640 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/da_cloze_self_test.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5094 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/da_gym_2000.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      560 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/hashtag_twitterhjerne.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      641 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/hub.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3407 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/hyggeswag.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1273 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/nordjylland_news.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5114 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/building/prompt_answer_da.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     7513 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/pretraining.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1562 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/data/statistics.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.921937 danoliterate-0.0.3/danoliterate/evaluation/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/__init__.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.921937 danoliterate-0.0.3/danoliterate/evaluation/analysis/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/analysis/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2639 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/analysis/analyser.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)    32146 2024-01-15 19:26:16.000000 danoliterate-0.0.3/danoliterate/evaluation/analysis/analysis_notebook.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      221 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/analysis/dimensions.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1560 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/analysis/inspection.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     6987 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/analysis/meta_scorings.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)    18800 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/analysis/metrics.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4910 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/analysis/scorer.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4947 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/artifact_integration.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.921937 danoliterate-0.0.3/danoliterate/evaluation/execution/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/execution/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     9470 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/execution/api_inference.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4063 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/execution/augmentation.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      192 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/execution/eval_types.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5208 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/execution/evaluator.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     8105 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/execution/huggingface_inference.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5650 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/execution/model_inference.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)    14445 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/execution/task_runner.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.925271 danoliterate-0.0.3/danoliterate/evaluation/leaderboard/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/leaderboard/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2994 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/leaderboard/metric_parsing.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4624 2024-01-15 00:12:11.000000 danoliterate-0.0.3/danoliterate/evaluation/leaderboard/table.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1570 2024-01-15 19:19:23.000000 danoliterate-0.0.3/danoliterate/evaluation/leaderboard/🇩🇰_Hello.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.925271 danoliterate-0.0.3/danoliterate/evaluation/registries/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/registries/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/registries/get.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2922 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/registries/inferences.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4307 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/registries/metrics.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     7462 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/registries/tasks.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     8788 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/results.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4354 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/evaluation/serialization.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.925271 danoliterate-0.0.3/danoliterate/infrastructure/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       69 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/infrastructure/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      277 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/infrastructure/constants.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      783 2024-01-15 19:24:56.000000 danoliterate-0.0.3/danoliterate/infrastructure/logging.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.925271 danoliterate-0.0.3/danoliterate/infrastructure/management/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/infrastructure/management/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     9491 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/infrastructure/management/artifacto.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      229 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/infrastructure/runs.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      228 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/infrastructure/timing.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.925271 danoliterate-0.0.3/danoliterate/modeling/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/modeling/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3113 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/modeling/gpt_ner_alignment.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      757 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/modeling/language_identification.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4231 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/modeling/load_model.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1101 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/modeling/ngram_language_modeling.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1563 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/modeling/text_classification.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5337 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/modeling/text_comparison.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1517 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/modeling/uncertainty_estimation.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.925271 danoliterate-0.0.3/danoliterate/training/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       34 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/training/__init__.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1214 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/training/efficiency.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     6247 2024-01-11 21:05:31.000000 danoliterate-0.0.3/danoliterate/training/lm_training.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.955270 danoliterate-0.0.3/danoliterate.egg-info/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2507 2024-01-15 19:44:09.000000 danoliterate-0.0.3/danoliterate.egg-info/PKG-INFO
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)    12236 2024-01-15 19:44:09.000000 danoliterate-0.0.3/danoliterate.egg-info/SOURCES.txt
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        1 2024-01-15 19:44:09.000000 danoliterate-0.0.3/danoliterate.egg-info/dependency_links.txt
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      754 2024-01-15 19:44:09.000000 danoliterate-0.0.3/danoliterate.egg-info/requires.txt
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       13 2024-01-15 19:44:09.000000 danoliterate-0.0.3/danoliterate.egg-info/top_level.txt
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/job-outputs/job-20240102-075208/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.925271 danoliterate-0.0.3/job-outputs/job-20240102-075208/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2050 2024-01-02 06:52:08.000000 danoliterate-0.0.3/job-outputs/job-20240102-075208/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3829 2024-01-02 06:52:08.000000 danoliterate-0.0.3/job-outputs/job-20240102-075208/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-02 06:52:08.000000 danoliterate-0.0.3/job-outputs/job-20240102-075208/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/job-outputs/job-20240102-080050/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.928604 danoliterate-0.0.3/job-outputs/job-20240102-080050/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2050 2024-01-02 07:00:51.000000 danoliterate-0.0.3/job-outputs/job-20240102-080050/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3829 2024-01-02 07:00:51.000000 danoliterate-0.0.3/job-outputs/job-20240102-080050/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-02 07:00:51.000000 danoliterate-0.0.3/job-outputs/job-20240102-080050/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/job-outputs/job-20240102-133515/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.928604 danoliterate-0.0.3/job-outputs/job-20240102-133515/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2050 2024-01-02 12:35:15.000000 danoliterate-0.0.3/job-outputs/job-20240102-133515/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3829 2024-01-02 12:35:15.000000 danoliterate-0.0.3/job-outputs/job-20240102-133515/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-02 12:35:15.000000 danoliterate-0.0.3/job-outputs/job-20240102-133515/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/job-outputs/job-20240102-193039/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.928604 danoliterate-0.0.3/job-outputs/job-20240102-193039/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2050 2024-01-02 18:30:39.000000 danoliterate-0.0.3/job-outputs/job-20240102-193039/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3829 2024-01-02 18:30:39.000000 danoliterate-0.0.3/job-outputs/job-20240102-193039/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-02 18:30:39.000000 danoliterate-0.0.3/job-outputs/job-20240102-193039/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/job-outputs/job-20240102-232500/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.928604 danoliterate-0.0.3/job-outputs/job-20240102-232500/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2050 2024-01-02 22:25:00.000000 danoliterate-0.0.3/job-outputs/job-20240102-232500/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3829 2024-01-02 22:25:00.000000 danoliterate-0.0.3/job-outputs/job-20240102-232500/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-02 22:25:00.000000 danoliterate-0.0.3/job-outputs/job-20240102-232500/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/job-outputs/job-20240103-084437/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.931937 danoliterate-0.0.3/job-outputs/job-20240103-084437/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2050 2024-01-03 07:44:37.000000 danoliterate-0.0.3/job-outputs/job-20240103-084437/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3829 2024-01-03 07:44:37.000000 danoliterate-0.0.3/job-outputs/job-20240103-084437/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-03 07:44:37.000000 danoliterate-0.0.3/job-outputs/job-20240103-084437/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/job-outputs/job-20240103-164458/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.931937 danoliterate-0.0.3/job-outputs/job-20240103-164458/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2050 2024-01-03 15:44:58.000000 danoliterate-0.0.3/job-outputs/job-20240103-164458/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3842 2024-01-03 15:44:58.000000 danoliterate-0.0.3/job-outputs/job-20240103-164458/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-03 15:44:58.000000 danoliterate-0.0.3/job-outputs/job-20240103-164458/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.905271 danoliterate-0.0.3/job-outputs/job-20240103-164511/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.931937 danoliterate-0.0.3/job-outputs/job-20240103-164511/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2055 2024-01-03 15:45:11.000000 danoliterate-0.0.3/job-outputs/job-20240103-164511/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3866 2024-01-03 15:45:11.000000 danoliterate-0.0.3/job-outputs/job-20240103-164511/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       14 2024-01-03 15:45:11.000000 danoliterate-0.0.3/job-outputs/job-20240103-164511/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-164531/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.931937 danoliterate-0.0.3/job-outputs/job-20240103-164531/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2055 2024-01-03 15:45:31.000000 danoliterate-0.0.3/job-outputs/job-20240103-164531/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3866 2024-01-03 15:45:31.000000 danoliterate-0.0.3/job-outputs/job-20240103-164531/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       14 2024-01-03 15:45:31.000000 danoliterate-0.0.3/job-outputs/job-20240103-164531/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-185156/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.935270 danoliterate-0.0.3/job-outputs/job-20240103-185156/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2055 2024-01-03 17:51:56.000000 danoliterate-0.0.3/job-outputs/job-20240103-185156/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3894 2024-01-03 17:51:56.000000 danoliterate-0.0.3/job-outputs/job-20240103-185156/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       27 2024-01-03 17:51:56.000000 danoliterate-0.0.3/job-outputs/job-20240103-185156/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-185500/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.935270 danoliterate-0.0.3/job-outputs/job-20240103-185500/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2056 2024-01-03 17:55:00.000000 danoliterate-0.0.3/job-outputs/job-20240103-185500/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3940 2024-01-03 17:55:00.000000 danoliterate-0.0.3/job-outputs/job-20240103-185500/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       49 2024-01-03 17:55:00.000000 danoliterate-0.0.3/job-outputs/job-20240103-185500/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-185540/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.935270 danoliterate-0.0.3/job-outputs/job-20240103-185540/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2056 2024-01-03 17:55:40.000000 danoliterate-0.0.3/job-outputs/job-20240103-185540/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3940 2024-01-03 17:55:40.000000 danoliterate-0.0.3/job-outputs/job-20240103-185540/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       49 2024-01-03 17:55:40.000000 danoliterate-0.0.3/job-outputs/job-20240103-185540/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-185737/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.935270 danoliterate-0.0.3/job-outputs/job-20240103-185737/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4767 2024-01-03 17:57:37.000000 danoliterate-0.0.3/job-outputs/job-20240103-185737/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4012 2024-01-03 17:57:37.000000 danoliterate-0.0.3/job-outputs/job-20240103-185737/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       84 2024-01-03 17:57:37.000000 danoliterate-0.0.3/job-outputs/job-20240103-185737/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-190426/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.938604 danoliterate-0.0.3/job-outputs/job-20240103-190426/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4769 2024-01-03 18:04:26.000000 danoliterate-0.0.3/job-outputs/job-20240103-190426/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4118 2024-01-03 18:04:26.000000 danoliterate-0.0.3/job-outputs/job-20240103-190426/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      131 2024-01-03 18:04:26.000000 danoliterate-0.0.3/job-outputs/job-20240103-190426/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-204714/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.938604 danoliterate-0.0.3/job-outputs/job-20240103-204714/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5226 2024-01-03 19:47:14.000000 danoliterate-0.0.3/job-outputs/job-20240103-204714/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3964 2024-01-03 19:47:14.000000 danoliterate-0.0.3/job-outputs/job-20240103-204714/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       57 2024-01-03 19:47:14.000000 danoliterate-0.0.3/job-outputs/job-20240103-204714/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-204731/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.938604 danoliterate-0.0.3/job-outputs/job-20240103-204731/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5226 2024-01-03 19:47:32.000000 danoliterate-0.0.3/job-outputs/job-20240103-204731/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4000 2024-01-03 19:47:32.000000 danoliterate-0.0.3/job-outputs/job-20240103-204731/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       74 2024-01-03 19:47:32.000000 danoliterate-0.0.3/job-outputs/job-20240103-204731/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240103-204744/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.938604 danoliterate-0.0.3/job-outputs/job-20240103-204744/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5231 2024-01-03 19:47:44.000000 danoliterate-0.0.3/job-outputs/job-20240103-204744/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4010 2024-01-03 19:47:44.000000 danoliterate-0.0.3/job-outputs/job-20240103-204744/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       79 2024-01-03 19:47:44.000000 danoliterate-0.0.3/job-outputs/job-20240103-204744/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240104-071348/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.938604 danoliterate-0.0.3/job-outputs/job-20240104-071348/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5235 2024-01-04 06:13:48.000000 danoliterate-0.0.3/job-outputs/job-20240104-071348/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3842 2024-01-04 06:13:48.000000 danoliterate-0.0.3/job-outputs/job-20240104-071348/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-04 06:13:48.000000 danoliterate-0.0.3/job-outputs/job-20240104-071348/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240104-142624/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.941937 danoliterate-0.0.3/job-outputs/job-20240104-142624/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5235 2024-01-04 13:26:24.000000 danoliterate-0.0.3/job-outputs/job-20240104-142624/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3842 2024-01-04 13:26:24.000000 danoliterate-0.0.3/job-outputs/job-20240104-142624/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-04 13:26:24.000000 danoliterate-0.0.3/job-outputs/job-20240104-142624/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-093656/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.941937 danoliterate-0.0.3/job-outputs/job-20240106-093656/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5235 2024-01-06 08:36:56.000000 danoliterate-0.0.3/job-outputs/job-20240106-093656/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3842 2024-01-06 08:36:56.000000 danoliterate-0.0.3/job-outputs/job-20240106-093656/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-06 08:36:56.000000 danoliterate-0.0.3/job-outputs/job-20240106-093656/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-220155/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.941937 danoliterate-0.0.3/job-outputs/job-20240106-220155/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:01:55.000000 danoliterate-0.0.3/job-outputs/job-20240106-220155/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:01:55.000000 danoliterate-0.0.3/job-outputs/job-20240106-220155/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:01:55.000000 danoliterate-0.0.3/job-outputs/job-20240106-220155/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-220249/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.941937 danoliterate-0.0.3/job-outputs/job-20240106-220249/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:02:49.000000 danoliterate-0.0.3/job-outputs/job-20240106-220249/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:02:49.000000 danoliterate-0.0.3/job-outputs/job-20240106-220249/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:02:49.000000 danoliterate-0.0.3/job-outputs/job-20240106-220249/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-220441/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.941937 danoliterate-0.0.3/job-outputs/job-20240106-220441/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:04:41.000000 danoliterate-0.0.3/job-outputs/job-20240106-220441/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:04:41.000000 danoliterate-0.0.3/job-outputs/job-20240106-220441/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:04:41.000000 danoliterate-0.0.3/job-outputs/job-20240106-220441/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-220632/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.945270 danoliterate-0.0.3/job-outputs/job-20240106-220632/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:06:32.000000 danoliterate-0.0.3/job-outputs/job-20240106-220632/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:06:32.000000 danoliterate-0.0.3/job-outputs/job-20240106-220632/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:06:32.000000 danoliterate-0.0.3/job-outputs/job-20240106-220632/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-220737/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.945270 danoliterate-0.0.3/job-outputs/job-20240106-220737/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:07:37.000000 danoliterate-0.0.3/job-outputs/job-20240106-220737/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:07:37.000000 danoliterate-0.0.3/job-outputs/job-20240106-220737/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:07:37.000000 danoliterate-0.0.3/job-outputs/job-20240106-220737/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-220842/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.945270 danoliterate-0.0.3/job-outputs/job-20240106-220842/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:08:42.000000 danoliterate-0.0.3/job-outputs/job-20240106-220842/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:08:42.000000 danoliterate-0.0.3/job-outputs/job-20240106-220842/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:08:42.000000 danoliterate-0.0.3/job-outputs/job-20240106-220842/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-220951/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.945270 danoliterate-0.0.3/job-outputs/job-20240106-220951/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:09:51.000000 danoliterate-0.0.3/job-outputs/job-20240106-220951/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:09:51.000000 danoliterate-0.0.3/job-outputs/job-20240106-220951/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:09:51.000000 danoliterate-0.0.3/job-outputs/job-20240106-220951/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-221029/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.948604 danoliterate-0.0.3/job-outputs/job-20240106-221029/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:10:29.000000 danoliterate-0.0.3/job-outputs/job-20240106-221029/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4028 2024-01-06 21:10:29.000000 danoliterate-0.0.3/job-outputs/job-20240106-221029/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       90 2024-01-06 21:10:29.000000 danoliterate-0.0.3/job-outputs/job-20240106-221029/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-221253/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.948604 danoliterate-0.0.3/job-outputs/job-20240106-221253/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:12:53.000000 danoliterate-0.0.3/job-outputs/job-20240106-221253/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:12:53.000000 danoliterate-0.0.3/job-outputs/job-20240106-221253/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:12:53.000000 danoliterate-0.0.3/job-outputs/job-20240106-221253/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-221330/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.948604 danoliterate-0.0.3/job-outputs/job-20240106-221330/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:13:30.000000 danoliterate-0.0.3/job-outputs/job-20240106-221330/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:13:30.000000 danoliterate-0.0.3/job-outputs/job-20240106-221330/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:13:30.000000 danoliterate-0.0.3/job-outputs/job-20240106-221330/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-221504/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.948604 danoliterate-0.0.3/job-outputs/job-20240106-221504/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:15:04.000000 danoliterate-0.0.3/job-outputs/job-20240106-221504/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:15:04.000000 danoliterate-0.0.3/job-outputs/job-20240106-221504/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:15:04.000000 danoliterate-0.0.3/job-outputs/job-20240106-221504/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-221552/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.951937 danoliterate-0.0.3/job-outputs/job-20240106-221552/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:15:52.000000 danoliterate-0.0.3/job-outputs/job-20240106-221552/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:15:52.000000 danoliterate-0.0.3/job-outputs/job-20240106-221552/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:15:52.000000 danoliterate-0.0.3/job-outputs/job-20240106-221552/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240106-221615/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.951937 danoliterate-0.0.3/job-outputs/job-20240106-221615/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5238 2024-01-06 21:16:15.000000 danoliterate-0.0.3/job-outputs/job-20240106-221615/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4024 2024-01-06 21:16:15.000000 danoliterate-0.0.3/job-outputs/job-20240106-221615/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       88 2024-01-06 21:16:15.000000 danoliterate-0.0.3/job-outputs/job-20240106-221615/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240107-124826/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.951937 danoliterate-0.0.3/job-outputs/job-20240107-124826/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5273 2024-01-07 11:48:26.000000 danoliterate-0.0.3/job-outputs/job-20240107-124826/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     3842 2024-01-07 11:48:26.000000 danoliterate-0.0.3/job-outputs/job-20240107-124826/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)        3 2024-01-07 11:48:26.000000 danoliterate-0.0.3/job-outputs/job-20240107-124826/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240115-204316/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.951937 danoliterate-0.0.3/job-outputs/job-20240115-204316/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     5277 2024-01-15 19:43:16.000000 danoliterate-0.0.3/job-outputs/job-20240115-204316/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4087 2024-01-15 19:43:16.000000 danoliterate-0.0.3/job-outputs/job-20240115-204316/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      121 2024-01-15 19:43:16.000000 danoliterate-0.0.3/job-outputs/job-20240115-204316/.hydra/overrides.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/job-outputs/job-20240115-204343/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.951937 danoliterate-0.0.3/job-outputs/job-20240115-204343/.hydra/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     2512 2024-01-15 19:43:43.000000 danoliterate-0.0.3/job-outputs/job-20240115-204343/.hydra/config.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     4007 2024-01-15 19:43:43.000000 danoliterate-0.0.3/job-outputs/job-20240115-204343/.hydra/hydra.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       78 2024-01-15 19:43:43.000000 danoliterate-0.0.3/job-outputs/job-20240115-204343/.hydra/overrides.yaml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1341 2024-01-11 21:05:31.000000 danoliterate-0.0.3/pyproject.toml
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      287 2024-01-11 21:05:31.000000 danoliterate-0.0.3/requirements-full.txt
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      538 2024-01-11 21:05:31.000000 danoliterate-0.0.3/requirements.txt
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)       38 2024-01-15 19:44:09.955270 danoliterate-0.0.3/setup.cfg
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1068 2024-01-15 19:44:00.000000 danoliterate-0.0.3/setup.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.951937 danoliterate-0.0.3/tests/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1590 2024-01-11 21:05:31.000000 danoliterate-0.0.3/tests/test_from_pretrained_no_disk.py
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)     1472 2024-01-11 21:05:31.000000 danoliterate-0.0.3/tests/test_likelihood_computation.py
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/wandb/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/wandb/latest-run/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.951937 danoliterate-0.0.3/wandb/latest-run/files/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      590 2024-01-03 17:52:08.000000 danoliterate-0.0.3/wandb/latest-run/files/config.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/wandb/run-20240102_144118-yu960l4r/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.955270 danoliterate-0.0.3/wandb/run-20240102_144118-yu960l4r/files/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      700 2024-01-02 13:41:45.000000 danoliterate-0.0.3/wandb/run-20240102_144118-yu960l4r/files/config.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/wandb/run-20240102_144223-8dnifqy5/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.955270 danoliterate-0.0.3/wandb/run-20240102_144223-8dnifqy5/files/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      700 2024-01-02 13:42:39.000000 danoliterate-0.0.3/wandb/run-20240102_144223-8dnifqy5/files/config.yaml
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.908604 danoliterate-0.0.3/wandb/run-20240102_144307-cc949b1q/
-drwxr-xr-x   0 sorenmulli  (1001) sorenmulli  (1001)        0 2024-01-15 19:44:09.955270 danoliterate-0.0.3/wandb/run-20240102_144307-cc949b1q/files/
--rw-r--r--   0 sorenmulli  (1001) sorenmulli  (1001)      700 2024-01-02 13:43:23.000000 danoliterate-0.0.3/wandb/run-20240102_144307-cc949b1q/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/.github/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/.github/workflows/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1113 2024-01-11 21:05:30.000000 danoliterate-0.0.4/.github/workflows/is_it_tidy.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       77 2024-01-11 21:05:31.000000 danoliterate-0.0.4/MANIFEST.in
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4075 2024-04-04 20:52:34.870272 danoliterate-0.0.4/PKG-INFO
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2072 2024-04-04 20:21:29.000000 danoliterate-0.0.4/README.md
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/danoliterate/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3083 2024-04-04 19:58:25.000000 danoliterate-0.0.4/danoliterate/__main__.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/danoliterate/configs/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/danoliterate/configs/databuild/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      253 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/databuild/citizenship_test.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      294 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/databuild/da_cloze_self_test.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       90 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/databuild/da_gym_2000.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      178 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/databuild/hashtag_twitterhjerne.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      220 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/databuild/hyggeswag.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      158 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/databuild/nordjylland_news.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       96 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/databuild/prompt_answer.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1274 2024-04-04 20:12:58.000000 danoliterate-0.0.4/danoliterate/configs/master.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/configs/model/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       56 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/baseline.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-04-02 19:44:55.000000 danoliterate-0.0.4/danoliterate/configs/model/claude-haiku.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       86 2024-04-02 19:44:07.000000 danoliterate-0.0.4/danoliterate/configs/model/claude-opus.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       90 2024-04-02 19:44:36.000000 danoliterate-0.0.4/danoliterate/configs/model/claude-sonnet.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      146 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/danoliterate-baseline.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      152 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/danoliterate-llama.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      154 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/danoliterate-mistral.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       67 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/danskgpt-api.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       97 2024-01-31 07:44:55.000000 danoliterate-0.0.4/danoliterate/configs/model/danskgpt-tiny-chat.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       87 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/danskgpt-tiny.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       58 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/danskgpt.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       84 2024-03-05 14:03:23.000000 danoliterate-0.0.4/danoliterate/configs/model/gemma-7b-it.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       72 2024-03-05 14:02:18.000000 danoliterate-0.0.4/danoliterate/configs/model/gemma-7b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       77 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/google-gemini-pro.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       96 2024-03-05 14:01:12.000000 danoliterate-0.0.4/danoliterate/configs/model/gpt-7b-nordic-prerelease.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       92 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/gpt-neo-da.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       81 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/gpt-neox-da.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      106 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/gpt-sw3-20b-instruct.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/gpt-sw3-20b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      118 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/gpt-sw3-6b-instruct.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      100 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/gpt-sw3-6b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      102 2024-03-05 13:58:23.000000 danoliterate-0.0.4/danoliterate/configs/model/heidrun-mistral-7b-base.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      102 2024-03-05 13:57:52.000000 danoliterate-0.0.4/danoliterate/configs/model/heidrun-mistral-7b-chat.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/hestenet-lm.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       89 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/kanelsnegl.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       95 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/llama2-13b-chat.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       85 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/llama2-13b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      133 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/llama2-70b-chat.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      123 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/llama2-70b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       93 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/llama2-7b-chat.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       83 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/llama2-7b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       76 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/mgpt-13b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       68 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/mgpt.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      109 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/mistral-7b-instruct-v0.2.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      102 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/mistral-7b-instruct.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       84 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/mistral-7b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      144 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/mixtral-8-7b-instruct.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      126 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/mixtral-8-7b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       82 2024-04-02 20:44:21.000000 danoliterate-0.0.4/danoliterate/configs/model/mixtral-groq.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      102 2024-01-31 07:44:55.000000 danoliterate-0.0.4/danoliterate/configs/model/munin-7b-alpha.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       99 2024-03-05 13:59:59.000000 danoliterate-0.0.4/danoliterate/configs/model/munin-mistral-7b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       97 2024-01-31 07:44:55.000000 danoliterate-0.0.4/danoliterate/configs/model/munin-neuralbeagle-7b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       92 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/nb-gpt-j-norpaca.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       76 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/nb-gpt-j.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       51 2024-04-04 20:13:21.000000 danoliterate-0.0.4/danoliterate/configs/model/new-hf.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       89 2024-03-05 14:04:38.000000 danoliterate-0.0.4/danoliterate/configs/model/olmo-7b-instruct.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       76 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/openai-ada-001.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       79 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/openai-babbage-002.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       79 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/openai-davinci-002.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       84 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/openai-davinci-003.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      101 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/openai-gpt-3.5-turbo-instruct.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       86 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/openai-gpt-4-turbo.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       67 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/openai-gpt-4.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       83 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/openai-gpt-turbo.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       69 2024-03-05 14:05:28.000000 danoliterate-0.0.4/danoliterate/configs/model/phi-2.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       84 2024-03-05 14:04:05.000000 danoliterate-0.0.4/danoliterate/configs/model/qwen1.5-7b-chat.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      102 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/solar-11b-instruct.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       84 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/solar-11b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       99 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/model/test.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       78 2024-04-04 12:58:20.000000 danoliterate-0.0.4/danoliterate/configs/model/viking-13b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       78 2024-04-04 12:58:41.000000 danoliterate-0.0.4/danoliterate/configs/model/viking-33b.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       76 2024-04-04 12:58:03.000000 danoliterate-0.0.4/danoliterate/configs/model/viking-7b.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/configs/scenarios/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      399 2024-04-04 12:45:17.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/angry-tweets.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      332 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/citizenship-test-free.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      294 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/citizenship-test-simple.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      369 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/citizenship-test.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      365 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/da-cloze-self-test-free.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      375 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/da-cloze-self-test.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      405 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/da-gym-2000-english.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      299 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/da-gym-2000-free.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      377 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/da-gym-2000.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      577 2024-04-04 12:39:37.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/dane-1.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      577 2024-04-04 12:39:49.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/dane-5.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      525 2024-04-04 12:39:25.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/dane.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      412 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/hashtag-twitterhjerne.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      266 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/hyggeswag-free.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      361 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/hyggeswag.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      765 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/nordjylland-news-detailed-prompt.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      393 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/nordjylland-news.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      123 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/scenarios/prompt-answer.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/configs/train/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      780 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/train/default.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      803 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/configs/train/test.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/data/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/data/__init__.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/data/building/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/data/building/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)    11349 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/data/building/citizenship_test_da.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3640 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/data/building/da_cloze_self_test.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5094 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/data/building/da_gym_2000.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      560 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/data/building/hashtag_twitterhjerne.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      641 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/data/building/hub.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3407 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/data/building/hyggeswag.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1273 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/data/building/nordjylland_news.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5114 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/data/building/prompt_answer_da.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     7513 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/data/pretraining.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1562 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/data/statistics.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/evaluation/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/evaluation/__init__.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/evaluation/analysis/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/evaluation/analysis/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      221 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/evaluation/analysis/dimensions.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     6929 2024-04-04 10:27:17.000000 danoliterate-0.0.4/danoliterate/evaluation/analysis/meta_scorings.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)    18800 2024-04-02 20:45:03.000000 danoliterate-0.0.4/danoliterate/evaluation/analysis/metrics.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4781 2024-04-04 19:35:39.000000 danoliterate-0.0.4/danoliterate/evaluation/analysis/scorer.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1152 2024-04-04 20:12:00.000000 danoliterate-0.0.4/danoliterate/evaluation/analysis/scores_report.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/evaluation/execution/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/evaluation/execution/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)    14951 2024-04-04 12:36:23.000000 danoliterate-0.0.4/danoliterate/evaluation/execution/api_inference.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4402 2024-04-04 12:36:23.000000 danoliterate-0.0.4/danoliterate/evaluation/execution/augmentation.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      192 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/evaluation/execution/eval_types.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4999 2024-04-04 12:36:23.000000 danoliterate-0.0.4/danoliterate/evaluation/execution/evaluator.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     8147 2024-04-04 20:48:10.000000 danoliterate-0.0.4/danoliterate/evaluation/execution/huggingface_inference.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5650 2024-04-02 20:45:03.000000 danoliterate-0.0.4/danoliterate/evaluation/execution/model_inference.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)    14445 2024-04-02 20:45:03.000000 danoliterate-0.0.4/danoliterate/evaluation/execution/task_runner.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/evaluation/registries/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/evaluation/registries/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3202 2024-04-04 12:36:23.000000 danoliterate-0.0.4/danoliterate/evaluation/registries/inferences.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4307 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/evaluation/registries/metrics.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     7462 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/evaluation/registries/tasks.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     9511 2024-04-04 19:45:06.000000 danoliterate-0.0.4/danoliterate/evaluation/results.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4693 2024-04-04 19:31:43.000000 danoliterate-0.0.4/danoliterate/evaluation/serialization.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/infrastructure/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       69 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/infrastructure/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      259 2024-04-04 12:36:23.000000 danoliterate-0.0.4/danoliterate/infrastructure/constants.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1291 2024-04-04 12:54:21.000000 danoliterate-0.0.4/danoliterate/infrastructure/logging.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.858272 danoliterate-0.0.4/danoliterate/infrastructure/management/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/infrastructure/management/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      229 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/infrastructure/runs.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      228 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/infrastructure/timing.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/danoliterate/modeling/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        0 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/modeling/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3113 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/modeling/gpt_ner_alignment.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      757 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/modeling/language_identification.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4231 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/modeling/load_model.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1101 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/modeling/ngram_language_modeling.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1563 2024-04-04 12:04:25.000000 danoliterate-0.0.4/danoliterate/modeling/text_classification.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5337 2024-04-02 20:45:03.000000 danoliterate-0.0.4/danoliterate/modeling/text_comparison.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1517 2024-03-04 11:59:47.000000 danoliterate-0.0.4/danoliterate/modeling/uncertainty_estimation.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/danoliterate/training/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       34 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/training/__init__.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1214 2024-01-11 21:05:31.000000 danoliterate-0.0.4/danoliterate/training/efficiency.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     6247 2024-04-02 20:45:03.000000 danoliterate-0.0.4/danoliterate/training/lm_training.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/danoliterate.egg-info/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4075 2024-04-04 20:52:34.000000 danoliterate-0.0.4/danoliterate.egg-info/PKG-INFO
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)    17272 2024-04-04 20:52:34.000000 danoliterate-0.0.4/danoliterate.egg-info/SOURCES.txt
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        1 2024-04-04 20:52:34.000000 danoliterate-0.0.4/danoliterate.egg-info/dependency_links.txt
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      768 2024-04-04 20:52:34.000000 danoliterate-0.0.4/danoliterate.egg-info/requires.txt
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       13 2024-04-04 20:52:34.000000 danoliterate-0.0.4/danoliterate.egg-info/top_level.txt
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240102-075208/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240102-075208/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2050 2024-01-02 06:52:08.000000 danoliterate-0.0.4/job-outputs/job-20240102-075208/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3829 2024-01-02 06:52:08.000000 danoliterate-0.0.4/job-outputs/job-20240102-075208/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-02 06:52:08.000000 danoliterate-0.0.4/job-outputs/job-20240102-075208/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240102-080050/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240102-080050/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2050 2024-01-02 07:00:51.000000 danoliterate-0.0.4/job-outputs/job-20240102-080050/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3829 2024-01-02 07:00:51.000000 danoliterate-0.0.4/job-outputs/job-20240102-080050/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-02 07:00:51.000000 danoliterate-0.0.4/job-outputs/job-20240102-080050/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240102-133515/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240102-133515/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2050 2024-01-02 12:35:15.000000 danoliterate-0.0.4/job-outputs/job-20240102-133515/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3829 2024-01-02 12:35:15.000000 danoliterate-0.0.4/job-outputs/job-20240102-133515/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-02 12:35:15.000000 danoliterate-0.0.4/job-outputs/job-20240102-133515/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240102-193039/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240102-193039/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2050 2024-01-02 18:30:39.000000 danoliterate-0.0.4/job-outputs/job-20240102-193039/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3829 2024-01-02 18:30:39.000000 danoliterate-0.0.4/job-outputs/job-20240102-193039/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-02 18:30:39.000000 danoliterate-0.0.4/job-outputs/job-20240102-193039/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240102-232500/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240102-232500/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2050 2024-01-02 22:25:00.000000 danoliterate-0.0.4/job-outputs/job-20240102-232500/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3829 2024-01-02 22:25:00.000000 danoliterate-0.0.4/job-outputs/job-20240102-232500/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-02 22:25:00.000000 danoliterate-0.0.4/job-outputs/job-20240102-232500/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-084437/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-084437/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2050 2024-01-03 07:44:37.000000 danoliterate-0.0.4/job-outputs/job-20240103-084437/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3829 2024-01-03 07:44:37.000000 danoliterate-0.0.4/job-outputs/job-20240103-084437/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-03 07:44:37.000000 danoliterate-0.0.4/job-outputs/job-20240103-084437/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-164458/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-164458/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2050 2024-01-03 15:44:58.000000 danoliterate-0.0.4/job-outputs/job-20240103-164458/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3842 2024-01-03 15:44:58.000000 danoliterate-0.0.4/job-outputs/job-20240103-164458/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-03 15:44:58.000000 danoliterate-0.0.4/job-outputs/job-20240103-164458/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-164511/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-164511/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2055 2024-01-03 15:45:11.000000 danoliterate-0.0.4/job-outputs/job-20240103-164511/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3866 2024-01-03 15:45:11.000000 danoliterate-0.0.4/job-outputs/job-20240103-164511/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       14 2024-01-03 15:45:11.000000 danoliterate-0.0.4/job-outputs/job-20240103-164511/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-164531/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-164531/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2055 2024-01-03 15:45:31.000000 danoliterate-0.0.4/job-outputs/job-20240103-164531/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3866 2024-01-03 15:45:31.000000 danoliterate-0.0.4/job-outputs/job-20240103-164531/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       14 2024-01-03 15:45:31.000000 danoliterate-0.0.4/job-outputs/job-20240103-164531/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-185156/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-185156/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2055 2024-01-03 17:51:56.000000 danoliterate-0.0.4/job-outputs/job-20240103-185156/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3894 2024-01-03 17:51:56.000000 danoliterate-0.0.4/job-outputs/job-20240103-185156/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       27 2024-01-03 17:51:56.000000 danoliterate-0.0.4/job-outputs/job-20240103-185156/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-185500/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-185500/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2056 2024-01-03 17:55:00.000000 danoliterate-0.0.4/job-outputs/job-20240103-185500/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3940 2024-01-03 17:55:00.000000 danoliterate-0.0.4/job-outputs/job-20240103-185500/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       49 2024-01-03 17:55:00.000000 danoliterate-0.0.4/job-outputs/job-20240103-185500/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-185540/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-185540/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2056 2024-01-03 17:55:40.000000 danoliterate-0.0.4/job-outputs/job-20240103-185540/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3940 2024-01-03 17:55:40.000000 danoliterate-0.0.4/job-outputs/job-20240103-185540/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       49 2024-01-03 17:55:40.000000 danoliterate-0.0.4/job-outputs/job-20240103-185540/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-185737/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-185737/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4767 2024-01-03 17:57:37.000000 danoliterate-0.0.4/job-outputs/job-20240103-185737/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4012 2024-01-03 17:57:37.000000 danoliterate-0.0.4/job-outputs/job-20240103-185737/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       84 2024-01-03 17:57:37.000000 danoliterate-0.0.4/job-outputs/job-20240103-185737/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-190426/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-190426/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4769 2024-01-03 18:04:26.000000 danoliterate-0.0.4/job-outputs/job-20240103-190426/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4118 2024-01-03 18:04:26.000000 danoliterate-0.0.4/job-outputs/job-20240103-190426/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      131 2024-01-03 18:04:26.000000 danoliterate-0.0.4/job-outputs/job-20240103-190426/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-204714/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-204714/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5226 2024-01-03 19:47:14.000000 danoliterate-0.0.4/job-outputs/job-20240103-204714/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3964 2024-01-03 19:47:14.000000 danoliterate-0.0.4/job-outputs/job-20240103-204714/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       57 2024-01-03 19:47:14.000000 danoliterate-0.0.4/job-outputs/job-20240103-204714/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-204731/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-204731/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5226 2024-01-03 19:47:32.000000 danoliterate-0.0.4/job-outputs/job-20240103-204731/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4000 2024-01-03 19:47:32.000000 danoliterate-0.0.4/job-outputs/job-20240103-204731/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       74 2024-01-03 19:47:32.000000 danoliterate-0.0.4/job-outputs/job-20240103-204731/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240103-204744/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240103-204744/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5231 2024-01-03 19:47:44.000000 danoliterate-0.0.4/job-outputs/job-20240103-204744/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4010 2024-01-03 19:47:44.000000 danoliterate-0.0.4/job-outputs/job-20240103-204744/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       79 2024-01-03 19:47:44.000000 danoliterate-0.0.4/job-outputs/job-20240103-204744/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240104-071348/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240104-071348/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5235 2024-01-04 06:13:48.000000 danoliterate-0.0.4/job-outputs/job-20240104-071348/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3842 2024-01-04 06:13:48.000000 danoliterate-0.0.4/job-outputs/job-20240104-071348/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-04 06:13:48.000000 danoliterate-0.0.4/job-outputs/job-20240104-071348/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240104-142624/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240104-142624/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5235 2024-01-04 13:26:24.000000 danoliterate-0.0.4/job-outputs/job-20240104-142624/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3842 2024-01-04 13:26:24.000000 danoliterate-0.0.4/job-outputs/job-20240104-142624/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-04 13:26:24.000000 danoliterate-0.0.4/job-outputs/job-20240104-142624/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-093656/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240106-093656/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5235 2024-01-06 08:36:56.000000 danoliterate-0.0.4/job-outputs/job-20240106-093656/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3842 2024-01-06 08:36:56.000000 danoliterate-0.0.4/job-outputs/job-20240106-093656/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-06 08:36:56.000000 danoliterate-0.0.4/job-outputs/job-20240106-093656/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-220155/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240106-220155/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:01:55.000000 danoliterate-0.0.4/job-outputs/job-20240106-220155/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:01:55.000000 danoliterate-0.0.4/job-outputs/job-20240106-220155/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:01:55.000000 danoliterate-0.0.4/job-outputs/job-20240106-220155/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-220249/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240106-220249/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:02:49.000000 danoliterate-0.0.4/job-outputs/job-20240106-220249/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:02:49.000000 danoliterate-0.0.4/job-outputs/job-20240106-220249/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:02:49.000000 danoliterate-0.0.4/job-outputs/job-20240106-220249/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-220441/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240106-220441/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:04:41.000000 danoliterate-0.0.4/job-outputs/job-20240106-220441/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:04:41.000000 danoliterate-0.0.4/job-outputs/job-20240106-220441/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:04:41.000000 danoliterate-0.0.4/job-outputs/job-20240106-220441/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-220632/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240106-220632/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:06:32.000000 danoliterate-0.0.4/job-outputs/job-20240106-220632/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:06:32.000000 danoliterate-0.0.4/job-outputs/job-20240106-220632/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:06:32.000000 danoliterate-0.0.4/job-outputs/job-20240106-220632/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-220737/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240106-220737/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:07:37.000000 danoliterate-0.0.4/job-outputs/job-20240106-220737/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:07:37.000000 danoliterate-0.0.4/job-outputs/job-20240106-220737/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:07:37.000000 danoliterate-0.0.4/job-outputs/job-20240106-220737/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-220842/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.862272 danoliterate-0.0.4/job-outputs/job-20240106-220842/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:08:42.000000 danoliterate-0.0.4/job-outputs/job-20240106-220842/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:08:42.000000 danoliterate-0.0.4/job-outputs/job-20240106-220842/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:08:42.000000 danoliterate-0.0.4/job-outputs/job-20240106-220842/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-220951/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240106-220951/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:09:51.000000 danoliterate-0.0.4/job-outputs/job-20240106-220951/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:09:51.000000 danoliterate-0.0.4/job-outputs/job-20240106-220951/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:09:51.000000 danoliterate-0.0.4/job-outputs/job-20240106-220951/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-221029/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240106-221029/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:10:29.000000 danoliterate-0.0.4/job-outputs/job-20240106-221029/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4028 2024-01-06 21:10:29.000000 danoliterate-0.0.4/job-outputs/job-20240106-221029/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       90 2024-01-06 21:10:29.000000 danoliterate-0.0.4/job-outputs/job-20240106-221029/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-221253/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240106-221253/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:12:53.000000 danoliterate-0.0.4/job-outputs/job-20240106-221253/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:12:53.000000 danoliterate-0.0.4/job-outputs/job-20240106-221253/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:12:53.000000 danoliterate-0.0.4/job-outputs/job-20240106-221253/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-221330/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240106-221330/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:13:30.000000 danoliterate-0.0.4/job-outputs/job-20240106-221330/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:13:30.000000 danoliterate-0.0.4/job-outputs/job-20240106-221330/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:13:30.000000 danoliterate-0.0.4/job-outputs/job-20240106-221330/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-221504/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240106-221504/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:15:04.000000 danoliterate-0.0.4/job-outputs/job-20240106-221504/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:15:04.000000 danoliterate-0.0.4/job-outputs/job-20240106-221504/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:15:04.000000 danoliterate-0.0.4/job-outputs/job-20240106-221504/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-221552/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240106-221552/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:15:52.000000 danoliterate-0.0.4/job-outputs/job-20240106-221552/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:15:52.000000 danoliterate-0.0.4/job-outputs/job-20240106-221552/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:15:52.000000 danoliterate-0.0.4/job-outputs/job-20240106-221552/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240106-221615/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240106-221615/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5238 2024-01-06 21:16:15.000000 danoliterate-0.0.4/job-outputs/job-20240106-221615/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4024 2024-01-06 21:16:15.000000 danoliterate-0.0.4/job-outputs/job-20240106-221615/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       88 2024-01-06 21:16:15.000000 danoliterate-0.0.4/job-outputs/job-20240106-221615/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240107-124826/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240107-124826/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5273 2024-01-07 11:48:26.000000 danoliterate-0.0.4/job-outputs/job-20240107-124826/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3842 2024-01-07 11:48:26.000000 danoliterate-0.0.4/job-outputs/job-20240107-124826/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)        3 2024-01-07 11:48:26.000000 danoliterate-0.0.4/job-outputs/job-20240107-124826/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240115-204316/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240115-204316/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5277 2024-01-15 19:43:16.000000 danoliterate-0.0.4/job-outputs/job-20240115-204316/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4087 2024-01-15 19:43:16.000000 danoliterate-0.0.4/job-outputs/job-20240115-204316/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      121 2024-01-15 19:43:16.000000 danoliterate-0.0.4/job-outputs/job-20240115-204316/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240115-204343/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240115-204343/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2512 2024-01-15 19:43:43.000000 danoliterate-0.0.4/job-outputs/job-20240115-204343/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4007 2024-01-15 19:43:43.000000 danoliterate-0.0.4/job-outputs/job-20240115-204343/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       78 2024-01-15 19:43:43.000000 danoliterate-0.0.4/job-outputs/job-20240115-204343/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240305-094247/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240305-094247/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5275 2024-03-05 08:42:47.000000 danoliterate-0.0.4/job-outputs/job-20240305-094247/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3860 2024-03-05 08:42:47.000000 danoliterate-0.0.4/job-outputs/job-20240305-094247/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-03-05 08:42:47.000000 danoliterate-0.0.4/job-outputs/job-20240305-094247/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240305-105817/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240305-105817/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5275 2024-03-05 09:58:17.000000 danoliterate-0.0.4/job-outputs/job-20240305-105817/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3860 2024-03-05 09:58:17.000000 danoliterate-0.0.4/job-outputs/job-20240305-105817/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-03-05 09:58:17.000000 danoliterate-0.0.4/job-outputs/job-20240305-105817/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240305-134743/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240305-134743/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5275 2024-03-05 12:47:44.000000 danoliterate-0.0.4/job-outputs/job-20240305-134743/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3860 2024-03-05 12:47:44.000000 danoliterate-0.0.4/job-outputs/job-20240305-134743/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-03-05 12:47:44.000000 danoliterate-0.0.4/job-outputs/job-20240305-134743/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240305-134823/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240305-134823/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5275 2024-03-05 12:48:23.000000 danoliterate-0.0.4/job-outputs/job-20240305-134823/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3860 2024-03-05 12:48:23.000000 danoliterate-0.0.4/job-outputs/job-20240305-134823/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-03-05 12:48:23.000000 danoliterate-0.0.4/job-outputs/job-20240305-134823/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240305-135336/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240305-135336/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5275 2024-03-05 12:53:36.000000 danoliterate-0.0.4/job-outputs/job-20240305-135336/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3860 2024-03-05 12:53:36.000000 danoliterate-0.0.4/job-outputs/job-20240305-135336/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-03-05 12:53:36.000000 danoliterate-0.0.4/job-outputs/job-20240305-135336/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240305-135854/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240305-135854/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5275 2024-03-05 12:58:54.000000 danoliterate-0.0.4/job-outputs/job-20240305-135854/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3860 2024-03-05 12:58:54.000000 danoliterate-0.0.4/job-outputs/job-20240305-135854/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-03-05 12:58:54.000000 danoliterate-0.0.4/job-outputs/job-20240305-135854/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240305-135908/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240305-135908/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5275 2024-03-05 12:59:08.000000 danoliterate-0.0.4/job-outputs/job-20240305-135908/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3860 2024-03-05 12:59:08.000000 danoliterate-0.0.4/job-outputs/job-20240305-135908/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-03-05 12:59:08.000000 danoliterate-0.0.4/job-outputs/job-20240305-135908/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240305-135950/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240305-135950/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5275 2024-03-05 12:59:50.000000 danoliterate-0.0.4/job-outputs/job-20240305-135950/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3860 2024-03-05 12:59:50.000000 danoliterate-0.0.4/job-outputs/job-20240305-135950/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-03-05 12:59:50.000000 danoliterate-0.0.4/job-outputs/job-20240305-135950/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240404-145007/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-145007/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5219 2024-04-04 12:50:07.000000 danoliterate-0.0.4/job-outputs/job-20240404-145007/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3879 2024-04-04 12:50:07.000000 danoliterate-0.0.4/job-outputs/job-20240404-145007/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       27 2024-04-04 12:50:07.000000 danoliterate-0.0.4/job-outputs/job-20240404-145007/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.850272 danoliterate-0.0.4/job-outputs/job-20240404-145426/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-145426/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5219 2024-04-04 12:54:26.000000 danoliterate-0.0.4/job-outputs/job-20240404-145426/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3879 2024-04-04 12:54:26.000000 danoliterate-0.0.4/job-outputs/job-20240404-145426/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       27 2024-04-04 12:54:26.000000 danoliterate-0.0.4/job-outputs/job-20240404-145426/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-150131/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-150131/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5216 2024-04-04 13:01:31.000000 danoliterate-0.0.4/job-outputs/job-20240404-150131/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3845 2024-04-04 13:01:31.000000 danoliterate-0.0.4/job-outputs/job-20240404-150131/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-04-04 13:01:31.000000 danoliterate-0.0.4/job-outputs/job-20240404-150131/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-150158/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-150158/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5216 2024-04-04 13:01:58.000000 danoliterate-0.0.4/job-outputs/job-20240404-150158/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3845 2024-04-04 13:01:58.000000 danoliterate-0.0.4/job-outputs/job-20240404-150158/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-04-04 13:01:58.000000 danoliterate-0.0.4/job-outputs/job-20240404-150158/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-213153/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-213153/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5216 2024-04-04 19:31:53.000000 danoliterate-0.0.4/job-outputs/job-20240404-213153/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3845 2024-04-04 19:31:53.000000 danoliterate-0.0.4/job-outputs/job-20240404-213153/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       11 2024-04-04 19:31:53.000000 danoliterate-0.0.4/job-outputs/job-20240404-213153/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-215256/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-215256/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5217 2024-04-04 19:52:56.000000 danoliterate-0.0.4/job-outputs/job-20240404-215256/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3847 2024-04-04 19:52:56.000000 danoliterate-0.0.4/job-outputs/job-20240404-215256/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       12 2024-04-04 19:52:56.000000 danoliterate-0.0.4/job-outputs/job-20240404-215256/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-215335/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-215335/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5217 2024-04-04 19:53:35.000000 danoliterate-0.0.4/job-outputs/job-20240404-215335/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3847 2024-04-04 19:53:35.000000 danoliterate-0.0.4/job-outputs/job-20240404-215335/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       12 2024-04-04 19:53:35.000000 danoliterate-0.0.4/job-outputs/job-20240404-215335/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-215350/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-215350/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5217 2024-04-04 19:53:50.000000 danoliterate-0.0.4/job-outputs/job-20240404-215350/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3847 2024-04-04 19:53:50.000000 danoliterate-0.0.4/job-outputs/job-20240404-215350/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       12 2024-04-04 19:53:50.000000 danoliterate-0.0.4/job-outputs/job-20240404-215350/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-215353/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-215353/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5217 2024-04-04 19:53:53.000000 danoliterate-0.0.4/job-outputs/job-20240404-215353/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3847 2024-04-04 19:53:53.000000 danoliterate-0.0.4/job-outputs/job-20240404-215353/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       12 2024-04-04 19:53:53.000000 danoliterate-0.0.4/job-outputs/job-20240404-215353/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-215511/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-215511/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5217 2024-04-04 19:55:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-215511/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3847 2024-04-04 19:55:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-215511/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       12 2024-04-04 19:55:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-215511/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-215525/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.866272 danoliterate-0.0.4/job-outputs/job-20240404-215525/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5217 2024-04-04 19:55:25.000000 danoliterate-0.0.4/job-outputs/job-20240404-215525/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3847 2024-04-04 19:55:25.000000 danoliterate-0.0.4/job-outputs/job-20240404-215525/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       12 2024-04-04 19:55:25.000000 danoliterate-0.0.4/job-outputs/job-20240404-215525/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-215609/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/job-outputs/job-20240404-215609/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5217 2024-04-04 19:56:09.000000 danoliterate-0.0.4/job-outputs/job-20240404-215609/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3847 2024-04-04 19:56:09.000000 danoliterate-0.0.4/job-outputs/job-20240404-215609/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       12 2024-04-04 19:56:09.000000 danoliterate-0.0.4/job-outputs/job-20240404-215609/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-220513/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/job-outputs/job-20240404-220513/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5231 2024-04-04 20:05:13.000000 danoliterate-0.0.4/job-outputs/job-20240404-220513/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4098 2024-04-04 20:05:13.000000 danoliterate-0.0.4/job-outputs/job-20240404-220513/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      134 2024-04-04 20:05:13.000000 danoliterate-0.0.4/job-outputs/job-20240404-220513/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-220659/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/job-outputs/job-20240404-220659/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2016 2024-04-04 20:06:59.000000 danoliterate-0.0.4/job-outputs/job-20240404-220659/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4278 2024-04-04 20:06:59.000000 danoliterate-0.0.4/job-outputs/job-20240404-220659/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      205 2024-04-04 20:06:59.000000 danoliterate-0.0.4/job-outputs/job-20240404-220659/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-221031/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/job-outputs/job-20240404-221031/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5202 2024-04-04 20:10:31.000000 danoliterate-0.0.4/job-outputs/job-20240404-221031/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3931 2024-04-04 20:10:31.000000 danoliterate-0.0.4/job-outputs/job-20240404-221031/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       53 2024-04-04 20:10:31.000000 danoliterate-0.0.4/job-outputs/job-20240404-221031/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-221111/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/job-outputs/job-20240404-221111/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5203 2024-04-04 20:11:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-221111/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3933 2024-04-04 20:11:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-221111/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       54 2024-04-04 20:11:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-221111/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-221511/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/job-outputs/job-20240404-221511/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     2016 2024-04-04 20:15:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-221511/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     4187 2024-04-04 20:15:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-221511/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      160 2024-04-04 20:15:11.000000 danoliterate-0.0.4/job-outputs/job-20240404-221511/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-221624/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/job-outputs/job-20240404-221624/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5173 2024-04-04 20:16:24.000000 danoliterate-0.0.4/job-outputs/job-20240404-221624/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3933 2024-04-04 20:16:24.000000 danoliterate-0.0.4/job-outputs/job-20240404-221624/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       53 2024-04-04 20:16:24.000000 danoliterate-0.0.4/job-outputs/job-20240404-221624/.hydra/overrides.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/job-outputs/job-20240404-221627/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/job-outputs/job-20240404-221627/.hydra/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     5174 2024-04-04 20:16:27.000000 danoliterate-0.0.4/job-outputs/job-20240404-221627/.hydra/config.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     3935 2024-04-04 20:16:28.000000 danoliterate-0.0.4/job-outputs/job-20240404-221627/.hydra/hydra.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       54 2024-04-04 20:16:28.000000 danoliterate-0.0.4/job-outputs/job-20240404-221627/.hydra/overrides.yaml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1341 2024-03-05 08:14:36.000000 danoliterate-0.0.4/pyproject.toml
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      318 2024-04-04 20:52:30.000000 danoliterate-0.0.4/requirements-full.txt
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      504 2024-04-04 20:46:48.000000 danoliterate-0.0.4/requirements.txt
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)       38 2024-04-04 20:52:34.870272 danoliterate-0.0.4/setup.cfg
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1068 2024-04-04 20:40:16.000000 danoliterate-0.0.4/setup.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/tests/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1590 2024-03-04 12:08:02.000000 danoliterate-0.0.4/tests/test_from_pretrained_no_disk.py
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)     1472 2024-03-04 12:08:02.000000 danoliterate-0.0.4/tests/test_likelihood_computation.py
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240102_144118-yu960l4r/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240102_144118-yu960l4r/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      700 2024-01-02 13:41:45.000000 danoliterate-0.0.4/wandb/run-20240102_144118-yu960l4r/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240102_144223-8dnifqy5/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240102_144223-8dnifqy5/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      700 2024-01-02 13:42:39.000000 danoliterate-0.0.4/wandb/run-20240102_144223-8dnifqy5/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240102_144307-cc949b1q/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240102_144307-cc949b1q/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      700 2024-01-02 13:43:23.000000 danoliterate-0.0.4/wandb/run-20240102_144307-cc949b1q/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240103_185207-2gwbcbde/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240103_185207-2gwbcbde/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      590 2024-01-03 17:52:08.000000 danoliterate-0.0.4/wandb/run-20240103_185207-2gwbcbde/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240305_094252-df29fahs/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240305_094252-df29fahs/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      656 2024-03-05 08:43:24.000000 danoliterate-0.0.4/wandb/run-20240305_094252-df29fahs/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240305_105822-c8kqo92t/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240305_105822-c8kqo92t/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      656 2024-03-05 09:58:53.000000 danoliterate-0.0.4/wandb/run-20240305_105822-c8kqo92t/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240305_134750-oo297j8y/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240305_134750-oo297j8y/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      656 2024-03-05 12:48:11.000000 danoliterate-0.0.4/wandb/run-20240305_134750-oo297j8y/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240305_134828-x0uracs9/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240305_134828-x0uracs9/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      656 2024-03-05 12:49:01.000000 danoliterate-0.0.4/wandb/run-20240305_134828-x0uracs9/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240305_135341-5hv9bvag/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240305_135341-5hv9bvag/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      656 2024-03-05 12:54:00.000000 danoliterate-0.0.4/wandb/run-20240305_135341-5hv9bvag/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240305_135914-1eueet3m/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240305_135914-1eueet3m/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      656 2024-03-05 12:59:38.000000 danoliterate-0.0.4/wandb/run-20240305_135914-1eueet3m/files/config.yaml
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.854272 danoliterate-0.0.4/wandb/run-20240305_135956-qujwpo8u/
+drwxr-xr-x   0 swiho    (237651) unixusers  (1040)        0 2024-04-04 20:52:34.870272 danoliterate-0.0.4/wandb/run-20240305_135956-qujwpo8u/files/
+-rw-r--r--   0 swiho    (237651) unixusers  (1040)      656 2024-03-05 13:00:28.000000 danoliterate-0.0.4/wandb/run-20240305_135956-qujwpo8u/files/config.yaml
```

### Comparing `danoliterate-0.0.3/.github/workflows/is_it_tidy.yaml` & `danoliterate-0.0.4/.github/workflows/is_it_tidy.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/PKG-INFO` & `danoliterate-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6461 6e6f  : 2.1.Name: dano
 00000020: 6c69 7465 7261 7465 0a56 6572 7369 6f6e  literate.Version
-00000030: 3a20 302e 302e 330a 5375 6d6d 6172 793a  : 0.0.3.Summary:
+00000030: 3a20 302e 302e 340a 5375 6d6d 6172 793a  : 0.0.4.Summary:
 00000040: 2042 656e 6368 6d61 726b 206f 6620 4765   Benchmark of Ge
 00000050: 6e65 7261 7469 7665 204c 6172 6765 204c  nerative Large L
 00000060: 616e 6775 6167 6520 4d6f 6465 6c73 2069  anguage Models i
 00000070: 6e20 4461 6e69 7368 0a48 6f6d 652d 7061  n Danish.Home-pa
 00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000090: 7562 2e63 6f6d 2f73 6f72 656e 6d75 6c6c  ub.com/sorenmull
 000000a0: 692f 6461 6e6f 6c69 7465 7261 7465 0a41  i/danoliterate.A
@@ -21,137 +21,235 @@
 00000140: 2070 616e 6461 737e 3d31 2e35 2e33 0a52   pandas~=1.5.3.R
 00000150: 6571 7569 7265 732d 4469 7374 3a20 6461  equires-Dist: da
 00000160: 7461 7365 7473 7e3d 322e 3134 2e35 0a52  tasets~=2.14.5.R
 00000170: 6571 7569 7265 732d 4469 7374 3a20 7472  equires-Dist: tr
 00000180: 616e 7366 6f72 6d65 7273 7e3d 342e 3336  ansformers~=4.36
 00000190: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
 000001a0: 3a20 746f 7263 687e 3d32 2e31 2e31 0a52  : torch~=2.1.1.R
-000001b0: 6571 7569 7265 732d 4469 7374 3a20 6163  equires-Dist: ac
-000001c0: 6365 6c65 7261 7465 7e3d 302e 3233 2e30  celerate~=0.23.0
+000001b0: 6571 7569 7265 732d 4469 7374 3a20 7361  equires-Dist: sa
+000001c0: 6665 7465 6e73 6f72 737e 3d30 2e33 2e33  fetensors~=0.3.3
 000001d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000001e0: 7361 6665 7465 6e73 6f72 737e 3d30 2e33  safetensors~=0.3
-000001f0: 2e33 0a52 6571 7569 7265 732d 4469 7374  .3.Requires-Dist
-00000200: 3a20 6d61 7470 6c6f 746c 6962 7e3d 332e  : matplotlib~=3.
-00000210: 382e 300a 5265 7175 6972 6573 2d44 6973  8.0.Requires-Dis
-00000220: 743a 2073 696d 706c 652d 7465 726d 2d6d  t: simple-term-m
-00000230: 656e 757e 3d31 2e36 2e31 0a52 6571 7569  enu~=1.6.1.Requi
-00000240: 7265 732d 4469 7374 3a20 6461 6e6c 707e  res-Dist: danlp~
-00000250: 3d30 2e31 2e32 0a52 6571 7569 7265 732d  =0.1.2.Requires-
-00000260: 4469 7374 3a20 6765 6e73 696d 7e3d 342e  Dist: gensim~=4.
-00000270: 332e 320a 5265 7175 6972 6573 2d44 6973  3.2.Requires-Dis
-00000280: 743a 2064 6565 7073 7065 6564 7e3d 302e  t: deepspeed~=0.
-00000290: 3132 2e34 0a52 6571 7569 7265 732d 4469  12.4.Requires-Di
-000002a0: 7374 3a20 7365 6e74 656e 6365 7069 6563  st: sentencepiec
-000002b0: 657e 3d30 2e31 2e39 390a 5265 7175 6972  e~=0.1.99.Requir
-000002c0: 6573 2d44 6973 743a 2061 7567 6d65 6e74  es-Dist: augment
-000002d0: 797e 3d31 2e34 2e33 0a52 6571 7569 7265  y~=1.4.3.Require
-000002e0: 732d 4469 7374 3a20 6461 6379 7e3d 322e  s-Dist: dacy~=2.
-000002f0: 372e 360a 5265 7175 6972 6573 2d44 6973  7.6.Requires-Dis
-00000300: 743a 2067 6f6f 676c 652d 636c 6f75 642d  t: google-cloud-
-00000310: 6169 706c 6174 666f 726d 7e3d 312e 3338  aiplatform~=1.38
-00000320: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
-00000330: 3a20 6f70 656e 6169 7e3d 302e 3238 2e31  : openai~=0.28.1
-00000340: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000350: 7374 7265 616d 6c69 747e 3d31 2e32 372e  streamlit~=1.27.
-00000360: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-00000370: 2068 7567 6769 6e67 6661 6365 5f68 7562   huggingface_hub
-00000380: 7e3d 302e 3139 2e34 0a52 6571 7569 7265  ~=0.19.4.Require
-00000390: 732d 4469 7374 3a20 6879 6472 612d 636f  s-Dist: hydra-co
-000003a0: 7265 7e3d 312e 332e 320a 5265 7175 6972  re~=1.3.2.Requir
-000003b0: 6573 2d44 6973 743a 2068 7964 7261 2d63  es-Dist: hydra-c
-000003c0: 6f6c 6f72 6c6f 677e 3d31 2e32 2e30 0a52  olorlog~=1.2.0.R
-000003d0: 6571 7569 7265 732d 4469 7374 3a20 6f6d  equires-Dist: om
-000003e0: 6567 6163 6f6e 667e 3d32 2e33 2e30 0a52  egaconf~=2.3.0.R
-000003f0: 6571 7569 7265 732d 4469 7374 3a20 7761  equires-Dist: wa
-00000400: 6e64 627e 3d30 2e31 352e 3131 0a52 6571  ndb~=0.15.11.Req
-00000410: 7569 7265 732d 4469 7374 3a20 6769 7470  uires-Dist: gitp
-00000420: 7974 686f 6e7e 3d33 2e31 2e33 370a 5265  ython~=3.1.37.Re
-00000430: 7175 6972 6573 2d44 6973 743a 2062 6c61  quires-Dist: bla
-00000440: 636b 7e3d 3233 2e37 2e30 0a52 6571 7569  ck~=23.7.0.Requi
-00000450: 7265 732d 4469 7374 3a20 6973 6f72 747e  res-Dist: isort~
-00000460: 3d35 2e31 322e 300a 5265 7175 6972 6573  =5.12.0.Requires
-00000470: 2d44 6973 743a 206d 7970 797e 3d31 2e35  -Dist: mypy~=1.5
-00000480: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
-00000490: 3a20 7079 6c69 6e74 7e3d 322e 3137 2e35  : pylint~=2.17.5
-000004a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004b0: 7061 6e64 6173 2d73 7475 6273 7e3d 322e  pandas-stubs~=2.
-000004c0: 302e 330a 5265 7175 6972 6573 2d44 6973  0.3.Requires-Dis
-000004d0: 743a 2074 7970 6573 2d74 7164 6d7e 3d34  t: types-tqdm~=4
-000004e0: 2e36 362e 300a 5265 7175 6972 6573 2d44  .66.0.Requires-D
-000004f0: 6973 743a 2074 7970 6573 2d72 6571 7565  ist: types-reque
-00000500: 7374 737e 3d32 2e33 312e 300a 5072 6f76  sts~=2.31.0.Prov
-00000510: 6964 6573 2d45 7874 7261 3a20 6675 6c6c  ides-Extra: full
-00000520: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000530: 7079 7064 667e 3d33 2e31 362e 313b 2065  pypdf~=3.16.1; e
-00000540: 7874 7261 203d 3d20 2266 756c 6c22 0a52  xtra == "full".R
-00000550: 6571 7569 7265 732d 4469 7374 3a20 6661  equires-Dist: fa
-00000560: 7374 7465 7874 2d77 6865 656c 7e3d 302e  sttext-wheel~=0.
-00000570: 392e 323b 2065 7874 7261 203d 3d20 2266  9.2; extra == "f
-00000580: 756c 6c22 0a52 6571 7569 7265 732d 4469  ull".Requires-Di
-00000590: 7374 3a20 7065 6674 7e3d 302e 352e 303b  st: peft~=0.5.0;
-000005a0: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
-000005b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000005c0: 7363 6970 797e 3d31 2e31 312e 333b 2065  scipy~=1.11.3; e
-000005d0: 7874 7261 203d 3d20 2266 756c 6c22 0a52  xtra == "full".R
-000005e0: 6571 7569 7265 732d 4469 7374 3a20 6e6c  equires-Dist: nl
-000005f0: 746b 7e3d 332e 382e 313b 2065 7874 7261  tk~=3.8.1; extra
-00000600: 203d 3d20 2266 756c 6c22 0a52 6571 7569   == "full".Requi
-00000610: 7265 732d 4469 7374 3a20 726f 7567 655f  res-Dist: rouge_
-00000620: 7363 6f72 657e 3d30 2e31 2e32 3b20 6578  score~=0.1.2; ex
-00000630: 7472 6120 3d3d 2022 6675 6c6c 220a 5265  tra == "full".Re
-00000640: 7175 6972 6573 2d44 6973 743a 2065 7661  quires-Dist: eva
-00000650: 6c75 6174 657e 3d30 2e34 2e30 3b20 6578  luate~=0.4.0; ex
-00000660: 7472 6120 3d3d 2022 6675 6c6c 220a 5265  tra == "full".Re
-00000670: 7175 6972 6573 2d44 6973 743a 2062 6572  quires-Dist: ber
-00000680: 745f 7363 6f72 657e 3d30 2e33 2e31 333b  t_score~=0.3.13;
-00000690: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
-000006a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000006b0: 7370 6163 797e 3d33 2e35 2e34 3b20 6578  spacy~=3.5.4; ex
-000006c0: 7472 6120 3d3d 2022 6675 6c6c 220a 5265  tra == "full".Re
-000006d0: 7175 6972 6573 2d44 6973 743a 206c 6576  quires-Dist: lev
-000006e0: 656e 7368 7465 696e 7e3d 302e 3233 2e30  enshtein~=0.23.0
-000006f0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
-00000700: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000710: 2073 6571 6576 616c 7e3d 312e 322e 323b   seqeval~=1.2.2;
-00000720: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
-00000730: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000740: 6265 6175 7469 6675 6c73 6f75 7034 7e3d  beautifulsoup4~=
-00000750: 342e 3132 2e32 3b20 6578 7472 6120 3d3d  4.12.2; extra ==
-00000760: 2022 6675 6c6c 220a 5265 7175 6972 6573   "full".Requires
-00000770: 2d44 6973 743a 2074 726c 7e3d 302e 372e  -Dist: trl~=0.7.
-00000780: 343b 2065 7874 7261 203d 3d20 2266 756c  4; extra == "ful
-00000790: 6c22 0a0a 2320 4172 6520 4c4c 4d73 2044  l"..# Are LLMs D
-000007a0: 616e 6f6c 6974 6572 6174 653f 0a0a 0a41  anoliterate?...A
-000007b0: 2062 656e 6368 6d61 726b 2074 6f6f 6c20   benchmark tool 
-000007c0: 666f 7220 4765 6e65 7261 7469 7665 204c  for Generative L
-000007d0: 6172 6765 204c 616e 6775 6167 6520 4d6f  arge Language Mo
-000007e0: 6465 6c73 2069 6e20 4461 6e69 7368 2e0a  dels in Danish..
-000007f0: 0a4e 6f74 653a 2054 6869 7320 7265 706f  .Note: This repo
-00000800: 7369 746f 7279 2069 7320 6375 7272 656e  sitory is curren
-00000810: 746c 7920 776f 726b 2d69 6e2d 7072 6f67  tly work-in-prog
-00000820: 7265 7373 2077 6869 6c65 2074 6865 206d  ress while the m
-00000830: 6173 7465 7227 7320 7468 6573 6973 2069  aster's thesis i
-00000840: 7320 6669 6e69 7368 6564 2e0a 496d 706c  s finished..Impl
-00000850: 656d 656e 7461 7469 6f6e 7320 6172 6520  ementations are 
-00000860: 7375 626a 6563 7420 746f 2063 6861 6e67  subject to chang
-00000870: 652e 0a0a 2323 2049 6e73 7461 6c6c 6174  e...## Installat
-00000880: 696f 6e0a 0a54 6865 2070 6163 6b61 6765  ion..The package
-00000890: 2068 6173 2062 6565 6e20 6465 7665 6c6f   has been develo
-000008a0: 7065 6420 616e 6420 7573 6564 2077 6974  ped and used wit
-000008b0: 6820 5079 7468 6f6e 2033 2e31 312e 0a54  h Python 3.11..T
-000008c0: 6f20 696e 7374 616c 6c20 7468 6520 7061  o install the pa
-000008d0: 636b 6167 6520 696e 2061 2062 6173 6520  ckage in a base 
-000008e0: 7665 7273 696f 6e2c 2065 6e61 626c 696e  version, enablin
-000008f0: 6720 6d6f 6465 6c20 6578 6563 7574 696f  g model executio
-00000900: 6e2c 2069 6e73 7461 6c6c 0a60 6060 0a70  n, install.```.p
-00000910: 6970 2069 6e73 7461 6c6c 2064 616e 6f6c  ip install danol
-00000920: 6974 6572 6174 650a 6060 600a 0a54 6f20  iterate.```..To 
-00000930: 696e 7374 616c 6c20 6974 2077 6974 6820  install it with 
-00000940: 7468 6520 656e 7469 7265 2073 7569 7465  the entire suite
-00000950: 206f 6620 6465 7065 6e64 656e 6369 6573   of dependencies
-00000960: 2074 6861 7420 7765 7265 2075 7365 6420   that were used 
-00000970: 696e 2074 6865 7369 732c 2072 756e 200a  in thesis, run .
-00000980: 6060 600a 6d61 6b65 2069 6e73 7461 6c6c  ```.make install
-00000990: 0a60 6060 0a0a 2323 2055 7361 6765 0a0a  .```..## Usage..
-000009a0: 6060 600a 7079 7468 6f6e 202d 6d20 6461  ```.python -m da
-000009b0: 6e6f 6c69 7465 7261 7465 2064 6f3d 6576  noliterate do=ev
-000009c0: 616c 7561 7465 0a60 6060 0a              aluate.```.
+000001e0: 6d61 7470 6c6f 746c 6962 7e3d 332e 382e  matplotlib~=3.8.
+000001f0: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
+00000200: 2073 696d 706c 652d 7465 726d 2d6d 656e   simple-term-men
+00000210: 757e 3d31 2e36 2e31 0a52 6571 7569 7265  u~=1.6.1.Require
+00000220: 732d 4469 7374 3a20 6175 676d 656e 7479  s-Dist: augmenty
+00000230: 7e3d 312e 342e 340a 5265 7175 6972 6573  ~=1.4.4.Requires
+00000240: 2d44 6973 743a 2073 6571 6576 616c 7e3d  -Dist: seqeval~=
+00000250: 312e 322e 320a 5265 7175 6972 6573 2d44  1.2.2.Requires-D
+00000260: 6973 743a 206c 6576 656e 7368 7465 696e  ist: levenshtein
+00000270: 7e3d 302e 3233 2e30 0a52 6571 7569 7265  ~=0.23.0.Require
+00000280: 732d 4469 7374 3a20 6e6c 746b 7e3d 332e  s-Dist: nltk~=3.
+00000290: 382e 310a 5265 7175 6972 6573 2d44 6973  8.1.Requires-Dis
+000002a0: 743a 2061 6273 6c2d 7079 7e3d 322e 312e  t: absl-py~=2.1.
+000002b0: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
+000002c0: 2065 7661 6c75 6174 657e 3d30 2e34 2e30   evaluate~=0.4.0
+000002d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000002e0: 726f 7567 655f 7363 6f72 657e 3d30 2e31  rouge_score~=0.1
+000002f0: 2e32 0a52 6571 7569 7265 732d 4469 7374  .2.Requires-Dist
+00000300: 3a20 6265 7274 5f73 636f 7265 7e3d 302e  : bert_score~=0.
+00000310: 332e 3133 0a52 6571 7569 7265 732d 4469  3.13.Requires-Di
+00000320: 7374 3a20 6765 6e73 696d 7e3d 342e 332e  st: gensim~=4.3.
+00000330: 320a 5265 7175 6972 6573 2d44 6973 743a  2.Requires-Dist:
+00000340: 2064 616e 6c70 7e3d 302e 312e 320a 5265   danlp~=0.1.2.Re
+00000350: 7175 6972 6573 2d44 6973 743a 2068 7567  quires-Dist: hug
+00000360: 6769 6e67 6661 6365 5f68 7562 7e3d 302e  gingface_hub~=0.
+00000370: 3139 2e34 0a52 6571 7569 7265 732d 4469  19.4.Requires-Di
+00000380: 7374 3a20 6879 6472 612d 636f 7265 7e3d  st: hydra-core~=
+00000390: 312e 332e 320a 5265 7175 6972 6573 2d44  1.3.2.Requires-D
+000003a0: 6973 743a 2068 7964 7261 2d63 6f6c 6f72  ist: hydra-color
+000003b0: 6c6f 677e 3d31 2e32 2e30 0a52 6571 7569  log~=1.2.0.Requi
+000003c0: 7265 732d 4469 7374 3a20 6f6d 6567 6163  res-Dist: omegac
+000003d0: 6f6e 667e 3d32 2e33 2e30 0a52 6571 7569  onf~=2.3.0.Requi
+000003e0: 7265 732d 4469 7374 3a20 6769 7470 7974  res-Dist: gitpyt
+000003f0: 686f 6e7e 3d33 2e31 2e33 370a 5265 7175  hon~=3.1.37.Requ
+00000400: 6972 6573 2d44 6973 743a 2062 6c61 636b  ires-Dist: black
+00000410: 7e3d 3233 2e37 2e30 0a52 6571 7569 7265  ~=23.7.0.Require
+00000420: 732d 4469 7374 3a20 6973 6f72 747e 3d35  s-Dist: isort~=5
+00000430: 2e31 322e 300a 5265 7175 6972 6573 2d44  .12.0.Requires-D
+00000440: 6973 743a 206d 7970 797e 3d31 2e35 2e31  ist: mypy~=1.5.1
+00000450: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000460: 7079 6c69 6e74 7e3d 322e 3137 2e35 0a52  pylint~=2.17.5.R
+00000470: 6571 7569 7265 732d 4469 7374 3a20 7061  equires-Dist: pa
+00000480: 6e64 6173 2d73 7475 6273 7e3d 322e 302e  ndas-stubs~=2.0.
+00000490: 330a 5265 7175 6972 6573 2d44 6973 743a  3.Requires-Dist:
+000004a0: 2074 7970 6573 2d74 7164 6d7e 3d34 2e36   types-tqdm~=4.6
+000004b0: 362e 300a 5265 7175 6972 6573 2d44 6973  6.0.Requires-Dis
+000004c0: 743a 2074 7970 6573 2d72 6571 7565 7374  t: types-request
+000004d0: 737e 3d32 2e33 312e 300a 5072 6f76 6964  s~=2.31.0.Provid
+000004e0: 6573 2d45 7874 7261 3a20 6675 6c6c 0a52  es-Extra: full.R
+000004f0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000500: 7064 667e 3d33 2e31 362e 313b 2065 7874  pdf~=3.16.1; ext
+00000510: 7261 203d 3d20 2266 756c 6c22 0a52 6571  ra == "full".Req
+00000520: 7569 7265 732d 4469 7374 3a20 6661 7374  uires-Dist: fast
+00000530: 7465 7874 2d77 6865 656c 7e3d 302e 392e  text-wheel~=0.9.
+00000540: 323b 2065 7874 7261 203d 3d20 2266 756c  2; extra == "ful
+00000550: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
+00000560: 3a20 7065 6674 7e3d 302e 352e 303b 2065  : peft~=0.5.0; e
+00000570: 7874 7261 203d 3d20 2266 756c 6c22 0a52  xtra == "full".R
+00000580: 6571 7569 7265 732d 4469 7374 3a20 7363  equires-Dist: sc
+00000590: 6970 797e 3d31 2e31 312e 333b 2065 7874  ipy~=1.11.3; ext
+000005a0: 7261 203d 3d20 2266 756c 6c22 0a52 6571  ra == "full".Req
+000005b0: 7569 7265 732d 4469 7374 3a20 7370 6163  uires-Dist: spac
+000005c0: 797e 3d33 2e35 2e34 3b20 6578 7472 6120  y~=3.5.4; extra 
+000005d0: 3d3d 2022 6675 6c6c 220a 5265 7175 6972  == "full".Requir
+000005e0: 6573 2d44 6973 743a 2062 6561 7574 6966  es-Dist: beautif
+000005f0: 756c 736f 7570 347e 3d34 2e31 322e 323b  ulsoup4~=4.12.2;
+00000600: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
+00000610: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000620: 7472 6c7e 3d30 2e37 2e34 3b20 6578 7472  trl~=0.7.4; extr
+00000630: 6120 3d3d 2022 6675 6c6c 220a 5265 7175  a == "full".Requ
+00000640: 6972 6573 2d44 6973 743a 2077 616e 6462  ires-Dist: wandb
+00000650: 7e3d 302e 3136 2e36 3b20 6578 7472 6120  ~=0.16.6; extra 
+00000660: 3d3d 2022 6675 6c6c 220a 5265 7175 6972  == "full".Requir
+00000670: 6573 2d44 6973 743a 2064 6565 7073 7065  es-Dist: deepspe
+00000680: 6564 7e3d 302e 3132 2e34 3b20 6578 7472  ed~=0.12.4; extr
+00000690: 6120 3d3d 2022 6675 6c6c 220a 5265 7175  a == "full".Requ
+000006a0: 6972 6573 2d44 6973 743a 2073 656e 7465  ires-Dist: sente
+000006b0: 6e63 6570 6965 6365 7e3d 302e 312e 3939  ncepiece~=0.1.99
+000006c0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
+000006d0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000006e0: 2061 6363 656c 6572 6174 657e 3d30 2e32   accelerate~=0.2
+000006f0: 332e 303b 2065 7874 7261 203d 3d20 2266  3.0; extra == "f
+00000700: 756c 6c22 0a52 6571 7569 7265 732d 4469  ull".Requires-Di
+00000710: 7374 3a20 676f 6f67 6c65 2d63 6c6f 7564  st: google-cloud
+00000720: 2d61 6970 6c61 7466 6f72 6d7e 3d31 2e33  -aiplatform~=1.3
+00000730: 382e 313b 2065 7874 7261 203d 3d20 2266  8.1; extra == "f
+00000740: 756c 6c22 0a52 6571 7569 7265 732d 4469  ull".Requires-Di
+00000750: 7374 3a20 6f70 656e 6169 7e3d 302e 3238  st: openai~=0.28
+00000760: 2e31 3b20 6578 7472 6120 3d3d 2022 6675  .1; extra == "fu
+00000770: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000780: 743a 2061 6e74 6872 6f70 6963 7e3d 302e  t: anthropic~=0.
+00000790: 3231 2e33 3b20 6578 7472 6120 3d3d 2022  21.3; extra == "
+000007a0: 6675 6c6c 220a 5265 7175 6972 6573 2d44  full".Requires-D
+000007b0: 6973 743a 2067 726f 713d 3d30 2e34 2e32  ist: groq==0.4.2
+000007c0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
+000007d0: 220a 0a23 2041 7265 204c 4c4d 7320 4461  "..# Are LLMs Da
+000007e0: 6e6f 6c69 7465 7261 7465 3f0a 0a41 2062  noliterate?..A b
+000007f0: 656e 6368 6d61 726b 2066 6f72 2047 656e  enchmark for Gen
+00000800: 6572 6174 6976 6520 4c61 7267 6520 4c61  erative Large La
+00000810: 6e67 7561 6765 204d 6f64 656c 7320 696e  nguage Models in
+00000820: 2044 616e 6973 682e 200a 546f 2073 6565   Danish. .To see
+00000830: 2072 6573 756c 7473 2061 6e64 2061 6e64   results and and
+00000840: 2067 6574 206d 6f72 6520 6465 7461 696c   get more detail
+00000850: 732c 2063 6865 636b 206f 7574 2074 6865  s, check out the
+00000860: 206c 6561 6465 7262 6f61 7264 2073 6974   leaderboard sit
+00000870: 653a 0a0a 3c70 2061 6c69 676e 3d22 6365  e:..<p align="ce
+00000880: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
+00000890: 6874 7470 733a 2f2f 6461 6e6f 6c69 7465  https://danolite
+000008a0: 7261 7465 2e63 6f6d 7075 7465 2e64 7475  rate.compute.dtu
+000008b0: 2e64 6b2f 223e 6461 6e6f 6c69 7465 7261  .dk/">danolitera
+000008c0: 7465 2e63 6f6d 7075 7465 2e64 7475 2e64  te.compute.dtu.d
+000008d0: 6b3c 2f61 3e0a 3c2f 703e 0a0a 5468 6520  k</a>.</p>..The 
+000008e0: 7072 6f6a 6563 7420 6973 206d 6169 6e74  project is maint
+000008f0: 6169 6e65 6420 6279 2053 c3b8 7265 6e20  ained by S..ren 
+00000900: 5665 6a6c 6761 6172 6420 486f 6c6d 2061  Vejlgaard Holm a
+00000910: 7420 4454 5520 436f 6d70 7574 652c 2073  t DTU Compute, s
+00000920: 7570 706f 7274 6564 2062 7920 7468 6520  upported by the 
+00000930: 4461 6e69 7368 2050 696f 6e65 6572 2043  Danish Pioneer C
+00000940: 656e 7472 6520 666f 7220 4149 2061 6e64  entre for AI and
+00000950: 2077 6974 6820 6d6f 7374 206f 6620 7468   with most of th
+00000960: 6520 776f 726b 2064 6f6e 6520 6173 2070  e work done as p
+00000970: 6172 7420 6f66 2074 6865 204d 6173 7465  art of the Maste
+00000980: 7227 7320 7468 6573 6973 205b 2727 4172  r's thesis [''Ar
+00000990: 6520 474c 4c4d 7320 4461 6e6f 6c69 7465  e GLLMs Danolite
+000009a0: 7261 7465 3f20 4265 6e63 686d 6172 6b69  rate? Benchmarki
+000009b0: 6e67 2047 656e 6572 6174 6976 6520 4e4c  ng Generative NL
+000009c0: 5020 696e 2044 616e 6973 6827 275d 2868  P in Danish''](h
+000009d0: 7474 7073 3a2f 2f73 6f72 656e 6d75 6c6c  ttps://sorenmull
+000009e0: 692e 6769 7468 7562 2e69 6f2f 7468 6573  i.github.io/thes
+000009f0: 6973 2f74 6865 7369 732e 7064 6629 2073  is/thesis.pdf) s
+00000a00: 7570 6572 7669 7365 6420 6279 204c 6172  upervised by Lar
+00000a10: 7320 4b61 6920 4861 6e73 656e 2066 726f  s Kai Hansen fro
+00000a20: 6d20 4454 5520 436f 6d70 7574 6520 616e  m DTU Compute an
+00000a30: 6420 4d61 7274 696e 2043 6172 7374 656e  d Martin Carsten
+00000a40: 204e 6965 6c73 656e 2066 726f 6d20 416c   Nielsen from Al
+00000a50: 7665 6e69 722e 0a0a 2323 2049 6e73 7461  venir...## Insta
+00000a60: 6c6c 6174 696f 6e0a 0a54 6865 2070 6163  llation..The pac
+00000a70: 6b61 6765 2068 6173 2062 6565 6e20 6465  kage has been de
+00000a80: 7665 6c6f 7065 6420 616e 6420 7573 6564  veloped and used
+00000a90: 2077 6974 6820 5079 7468 6f6e 2033 2e31   with Python 3.1
+00000aa0: 312e 0a54 6f20 696e 7374 616c 6c20 7468  1..To install th
+00000ab0: 6520 7061 636b 6167 6520 696e 2061 2062  e package in a b
+00000ac0: 6173 6520 7665 7273 696f 6e2c 2065 6e61  ase version, ena
+00000ad0: 626c 696e 6720 6d6f 6465 6c20 6578 6563  bling model exec
+00000ae0: 7574 696f 6e2c 2069 6e73 7461 6c6c 0a60  ution, install.`
+00000af0: 6060 0a70 6970 2069 6e73 7461 6c6c 2064  ``.pip install d
+00000b00: 616e 6f6c 6974 6572 6174 650a 6060 600a  anoliterate.```.
+00000b10: 2a4e 6f74 653a 2a20 536f 6d65 2066 6561  *Note:* Some fea
+00000b20: 7475 7265 7320 6e65 6564 2061 2066 756c  tures need a ful
+00000b30: 6c20 696e 7374 616c 6c20 746f 2072 756e  l install to run
+00000b40: 3a0a 6060 600a 7069 7020 696e 7374 616c  :.```.pip instal
+00000b50: 6c20 6461 6e6f 6c69 7465 7261 7465 5b66  l danoliterate[f
+00000b60: 756c 6c5d 0a60 6060 0a0a 2323 2055 7361  ull].```..## Usa
+00000b70: 6765 0a0a 5365 6520 6f70 7469 6f6e 7320  ge..See options 
+00000b80: 7769 7468 0a60 6060 6261 7368 0a70 7974  with.```bash.pyt
+00000b90: 686f 6e20 2d6d 2064 616e 6f6c 6974 6572  hon -m danoliter
+00000ba0: 6174 6520 646f 3d65 7661 6c75 6174 650a  ate do=evaluate.
+00000bb0: 6060 600a 0a41 2074 7970 6963 616c 2075  ```..A typical u
+00000bc0: 7365 2077 6f75 6c64 2062 6520 746f 2072  se would be to r
+00000bd0: 756e 2079 6f75 7220 6f77 6e20 6d6f 6465  un your own mode
+00000be0: 6c20 686f 7374 6564 206f 6e20 7468 6520  l hosted on the 
+00000bf0: 4875 6767 696e 6766 6163 6520 4875 6220  Huggingface Hub 
+00000c00: 6f6e 2061 2073 6365 6e61 7269 6f2c 2066  on a scenario, f
+00000c10: 6f72 2065 7861 6d70 6c65 2074 6865 2043  or example the C
+00000c20: 6974 697a 656e 7368 6970 2054 6573 7420  itizenship Test 
+00000c30: 5363 656e 6172 696f 2028 7365 6520 5b74  Scenario (see [t
+00000c40: 6865 2066 726f 6e74 656e 645d 2868 7474  he frontend](htt
+00000c50: 7073 3a2f 2f64 616e 6f6c 6974 6572 6174  ps://danoliterat
+00000c60: 652e 636f 6d70 7574 652e 6474 752e 646b  e.compute.dtu.dk
+00000c70: 2f53 6365 6e61 7269 6f73 2920 666f 7220  /Scenarios) for 
+00000c80: 7363 656e 6172 696f 2064 6573 6372 6970  scenario descrip
+00000c90: 7469 6f6e 7329 2e0a 536b 6970 2074 6865  tions)..Skip the
+00000ca0: 206c 696e 6520 6073 6365 6e61 7269 6f73   line `scenarios
+00000cb0: 3d60 2074 6f20 6d61 6b65 2069 7420 7275  =` to make it ru
+00000cc0: 6e20 6f6e 2061 6c6c 2073 6365 6e61 7269  n on all scenari
+00000cd0: 6f73 2069 6e73 7465 6164 2e0a 6060 6062  os instead..```b
+00000ce0: 6173 680a 7079 7468 6f6e 202d 6d20 6461  ash.python -m da
+00000cf0: 6e6f 6c69 7465 7261 7465 2064 6f3d 6576  noliterate do=ev
+00000d00: 616c 7561 7465 5c0a 2020 2020 7363 656e  aluate\.    scen
+00000d10: 6172 696f 733d 2263 6974 697a 656e 7368  arios="citizensh
+00000d20: 6970 2d74 6573 7422 5c0a 2020 2020 6d6f  ip-test"\.    mo
+00000d30: 6465 6c2e 6e61 6d65 3d22 4d79 4c69 7474  del.name="MyLitt
+00000d40: 6c65 4750 5422 5c0a 2020 2020 6d6f 6465  leGPT"\.    mode
+00000d50: 6c2e 7061 7468 3d22 6866 2d69 6e74 6572  l.path="hf-inter
+00000d60: 6e61 6c2d 7465 7374 696e 672f 7469 6e79  nal-testing/tiny
+00000d70: 2d72 616e 646f 6d2d 6770 7432 225c 0a20  -random-gpt2"\. 
+00000d80: 2020 2065 7661 6c75 6174 696f 6e2e 6c6f     evaluation.lo
+00000d90: 6361 6c5f 7265 7375 6c74 733d 222e 2f6d  cal_results="./m
+00000da0: 792d 7265 7375 6c74 2d64 6222 0a60 6060  y-result-db".```
+00000db0: 0a0a 4e6f 772c 2079 6f75 2063 6f75 6c64  ..Now, you could
+00000dc0: 2073 6861 7265 2074 6865 2072 6573 756c   share the resul
+00000dd0: 7469 6e67 204a 534f 4e20 706c 6163 6564  ting JSON placed
+00000de0: 2069 6e20 606d 792d 7265 7375 6c74 2d64   in `my-result-d
+00000df0: 6260 2074 6f20 6765 7420 6974 2069 6e63  b` to get it inc
+00000e00: 6c75 6465 6420 696e 2074 6865 2044 616e  luded in the Dan
+00000e10: 6f6c 6974 6572 6174 6520 6265 6e63 686d  oliterate benchm
+00000e20: 6172 6b2c 206f 7220 796f 7520 6361 6e20  ark, or you can 
+00000e30: 7361 7469 7366 7920 796f 7572 2063 7572  satisfy your cur
+00000e40: 696f 7369 7479 2061 6e64 2073 636f 7265  iosity and score
+00000e50: 2069 7420 796f 7572 7365 6c66 0a60 6060   it yourself.```
+00000e60: 6261 7368 0a23 2043 616c 6375 6c61 7465  bash.# Calculate
+00000e70: 7320 7363 6f72 696e 6720 6d65 7472 6963  s scoring metric
+00000e80: 730a 7079 7468 6f6e 202d 6d20 6461 6e6f  s.python -m dano
+00000e90: 6c69 7465 7261 7465 2064 6f3d 7363 6f72  literate do=scor
+00000ea0: 655c 0a20 2020 2065 7661 6c75 6174 696f  e\.    evaluatio
+00000eb0: 6e2e 6c6f 6361 6c5f 7265 7375 6c74 733d  n.local_results=
+00000ec0: 222e 2f6d 792d 7265 7375 6c74 2d64 6222  "./my-result-db"
+00000ed0: 0a23 2050 7269 6e74 7320 7468 656d 2066  .# Prints them f
+00000ee0: 6f72 2079 6f75 0a70 7974 686f 6e20 2d6d  or you.python -m
+00000ef0: 2064 616e 6f6c 6974 6572 6174 6520 646f   danoliterate do
+00000f00: 3d72 6570 6f72 745c 0a20 2020 2065 7661  =report\.    eva
+00000f10: 6c75 6174 696f 6e2e 6c6f 6361 6c5f 7265  luation.local_re
+00000f20: 7375 6c74 733d 222e 2f6d 792d 7265 7375  sults="./my-resu
+00000f30: 6c74 2d64 6222 0a60 6060 0a0a 2323 2043  lt-db".```..## C
+00000f40: 6f6e 7461 6374 0a50 6c65 6173 6520 7265  ontact.Please re
+00000f50: 6163 6820 6865 7265 2075 7369 6e67 2047  ach here using G
+00000f60: 6974 4875 6220 6973 7375 6573 206f 7220  itHub issues or 
+00000f70: 6f6e 206d 6169 6c20 746f 2053 c3b8 7265  on mail to S..re
+00000f80: 6e20 5665 6a6c 6761 6172 6420 486f 6c6d  n Vejlgaard Holm
+00000f90: 2065 6974 6865 7220 6174 205b 7377 6968   either at [swih
+00000fa0: 6f40 6474 752e 646b 5d28 6d61 696c 746f  o@dtu.dk](mailto
+00000fb0: 3a73 7769 686f 4064 7475 2e64 6b29 206f  :swiho@dtu.dk) o
+00000fc0: 7220 5b73 7768 4061 6c76 656e 6972 2e61  r [swh@alvenir.a
+00000fd0: 695d 286d 6169 6c74 6f3a 7377 6840 616c  i](mailto:swh@al
+00000fe0: 7665 6e69 722e 6169 292e 0a              venir.ai)..
```

### Comparing `danoliterate-0.0.3/danoliterate/__main__.py` & `danoliterate-0.0.4/danoliterate/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,21 +54,24 @@
             from danoliterate.training import train_lm
 
             train_lm(cfg)
         case "score":
             from danoliterate.evaluation.analysis.scorer import score
 
             score(cfg)
-        case "inspect":
-            from danoliterate.evaluation.analysis.inspection import inspect
 
-            inspect(cfg)
+        case "report":
+            from danoliterate.evaluation.analysis.scores_report import report_scores
+
+            report_scores(cfg)
         case _:
             logger.error(
-                "Unsupported do=%s. 'evaluate', 'databuild', 'train', 'score' are supported", cfg.do
+                "Unsupported do=%s. "
+                "'evaluate', 'databuild', 'train', 'score', 'report' are supported",
+                cfg.do,
             )
             raise ValueError("Unsupported do")
 
 
 if __name__ == "__main__":
     try:
         # pylint: disable=no-value-for-parameter
```

### Comparing `danoliterate-0.0.3/danoliterate/configs/master.yaml` & `danoliterate-0.0.4/danoliterate/configs/master.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     - dane
     - da-gym-2000
     - nordjylland-news
     - hashtag-twitterhjerne
     - citizenship-test
     - da-cloze-self-test
     - angry-tweets
-  - model: test
+  - model: new-hf
 # Used if running do=databuild
   - databuild: prompt_answer
 # Used if running do=train
   - train: default
   - override hydra/job_logging: colorlog
   - override hydra/hydra_logging: colorlog
 
@@ -39,19 +39,17 @@
 download_no_cache: false
 
 model_paths:
   fasttext: "local-models/lid.176.bin"
   dsl3gram: "local-models/dsl_3gram.klm"
 
 wandb:
-  enabled: true
+  enabled: false
   entity: "sorenmulli"
   project: "nlgenda"
-  artifact_cache: "local-computations/wandb-cache.json"
-  cache_update: false
 
 hydra:
   run:
     dir: ${outputs}/${hydra.job.name}
   sweep:
     dir: ${outputs}/${hydra.job.name}
     subdir: ${hydra.job.num}
```

### Comparing `danoliterate-0.0.3/danoliterate/configs/scenarios/dane-1.yaml` & `danoliterate-0.0.4/danoliterate/configs/scenarios/dane-1.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 dane:
   name: "DaNE"
-  path: "ScandEval/dane-mini"
+  path: "sorenmulli/dane-mini"
   pre_prompt: "Fuldfør annotering af sidste eksempel i opgaven.\nHer er en lingvists arbejde med at annotere entiteter af typen '{entity_str}'. {few_shot_str}\n\n# TEKST\n"
   post_prompt: "\n# ANNOTERING\n"
-  dataset_split: "val"
+  dataset_split: "validation"
   type: "few-shot-experiment-1"
   task:
     type: "gpt-ner"
     few_shot_format: "# TEKST\n{text}\n# ANNOTERING\n{annotated_text}"
     entity_types:
       - LOC: "lokation"
       - PER: "person"
```

### Comparing `danoliterate-0.0.3/danoliterate/configs/scenarios/dane-5.yaml` & `danoliterate-0.0.4/danoliterate/configs/scenarios/dane-5.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 dane:
   name: "DaNE"
-  path: "ScandEval/dane-mini"
+  path: "sorenmulli/dane-mini"
   pre_prompt: "Fuldfør annotering af sidste eksempel i opgaven.\nHer er en lingvists arbejde med at annotere entiteter af typen '{entity_str}'. {few_shot_str}\n\n# TEKST\n"
   post_prompt: "\n# ANNOTERING\n"
-  dataset_split: "val"
+  dataset_split: "validation"
   type: "few-shot-experiment-5"
   task:
     type: "gpt-ner"
     few_shot_format: "# TEKST\n{text}\n# ANNOTERING\n{annotated_text}"
     entity_types:
       - LOC: "lokation"
       - PER: "person"
```

### Comparing `danoliterate-0.0.3/danoliterate/configs/scenarios/dane.yaml` & `danoliterate-0.0.4/danoliterate/configs/scenarios/dane.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 dane:
   name: "DaNE"
-  path: "ScandEval/dane-mini"
+  path: "sorenmulli/dane-mini"
   pre_prompt: "Fuldfør annotering af sidste eksempel i opgaven.\nHer er en lingvists arbejde med at annotere entiteter af typen '{entity_str}'. {few_shot_str}\n\n# TEKST\n"
   post_prompt: "\n# ANNOTERING\n"
-  dataset_split: "val"
+  dataset_split: "validation"
   task:
     type: "gpt-ner"
     few_shot_format: "# TEKST\n{text}\n# ANNOTERING\n{annotated_text}"
     entity_types:
       - LOC: "lokation"
       - PER: "person"
       - ORG: "organisation"
```

### Comparing `danoliterate-0.0.3/danoliterate/configs/scenarios/nordjylland-news-detailed-prompt.yaml` & `danoliterate-0.0.4/danoliterate/configs/scenarios/nordjylland-news-detailed-prompt.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/configs/train/default.yaml` & `danoliterate-0.0.4/danoliterate/configs/train/default.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/configs/train/test.yaml` & `danoliterate-0.0.4/danoliterate/configs/train/test.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/building/citizenship_test_da.py` & `danoliterate-0.0.4/danoliterate/data/building/citizenship_test_da.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/building/da_cloze_self_test.py` & `danoliterate-0.0.4/danoliterate/data/building/da_cloze_self_test.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/building/da_gym_2000.py` & `danoliterate-0.0.4/danoliterate/data/building/da_gym_2000.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/building/hashtag_twitterhjerne.py` & `danoliterate-0.0.4/danoliterate/data/building/hashtag_twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/building/hub.py` & `danoliterate-0.0.4/danoliterate/data/building/hub.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/building/hyggeswag.py` & `danoliterate-0.0.4/danoliterate/data/building/hyggeswag.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/building/nordjylland_news.py` & `danoliterate-0.0.4/danoliterate/data/building/nordjylland_news.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/building/prompt_answer_da.py` & `danoliterate-0.0.4/danoliterate/data/building/prompt_answer_da.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/pretraining.py` & `danoliterate-0.0.4/danoliterate/data/pretraining.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/data/statistics.py` & `danoliterate-0.0.4/danoliterate/data/statistics.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/analysis/meta_scorings.py` & `danoliterate-0.0.4/danoliterate/evaluation/analysis/meta_scorings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import DefaultDict, Optional
 
 from danoliterate.evaluation.analysis.dimensions import Dimension
-from danoliterate.evaluation.results import MetricResult, Scores, Scoring
+from danoliterate.evaluation.results import ExecutionResultMetadata, MetricResult, Scores, Scoring
 from danoliterate.infrastructure.logging import logger
 
 
 class MetaScoring(ABC):
     @abstractmethod
-    def meta_score(self, scores: Scores) -> list[tuple[str, str, Dimension, list[MetricResult]]]:
+    def meta_score(
+        self, scores: Scores
+    ) -> list[tuple[ExecutionResultMetadata, list[MetricResult]]]:
         ...
 
 
 class TimingScore(MetaScoring):
-    def meta_score(self, scores: Scores) -> list[tuple[str, str, Dimension, list[MetricResult]]]:
+    def meta_score(
+        self, scores: Scores
+    ) -> list[tuple[ExecutionResultMetadata, list[MetricResult]]]:
         out = []
         for scoring in scores.scorings:
-            if scoring.execution_metadata.augmenter_key is not None:
+            if _should_skip_for_meta(scoring, (None,)):
                 continue
             if (total_time := scoring.execution_metadata.total_inference_seconds) is not None:
                 avg_time = total_time / len(scoring.metric_results[0].example_results)
-                scenario_name: str = scoring.execution_metadata.scenario_cfg["name"]  # type: ignore
-                model_name: str = scoring.execution_metadata.model_cfg["name"]  # type: ignore
                 out.append(
                     (
-                        scenario_name,
-                        model_name,
-                        Dimension.EFFICIENCY,
+                        scoring.execution_metadata,
                         [
                             MetricResult(
                                 "Inference seconds",
                                 "Total dataset wall time in seconds "
                                 "divided by number of examples",
                                 {},  # TODO: Add examples so we can do micro avg
                                 aggregate=avg_time,
@@ -72,69 +72,66 @@
         first, other = self.relevant_augmenter_keys
         for result in scorings[first].metric_results:
             for other_result in scorings[other].metric_results:
                 if result.short_name == other_result.short_name:
                     diff = result.aggregate - other_result.aggregate
                     if diff:
                         if diff > 0 and self.cannot_be_positive:
-                            res = 0
+                            res = 0.0
                         elif result.aggregate:
                             res = diff / result.aggregate
                         else:
-                            res = 1
+                            res = 1.0
                     else:
-                        res = 0
+                        res = 0.0
                     out.append(
                         MetricResult(
-                            result.short_name,
+                            f"{self.name}: {result.short_name}",
                             f"{self.description}: {result.description}",
                             {},
                             aggregate=res,
                             error=None,
                             higher_is_better=result.higher_is_better,
                         )
                     )
                     break
             else:
                 raise ValueError("Disparity calculation not possible: Different metrics")
         return out
 
-    def meta_score(self, scores: Scores) -> list[tuple[str, str, Dimension, list[MetricResult]]]:
+    def meta_score(
+        self, scores: Scores
+    ) -> list[tuple[ExecutionResultMetadata, list[MetricResult]]]:
         out = []
-        scorings_to_keep = []
         to_calculate: DefaultDict[tuple[str, str], dict] = defaultdict(dict)
 
         for scoring in scores.scorings:
-            if scoring.execution_metadata.augmenter_key not in self.relevant_augmenter_keys:
-                scorings_to_keep.append(scoring)
+            if _should_skip_for_meta(scoring, self.relevant_augmenter_keys):
                 continue
             to_calculate[
                 scoring.execution_metadata.scenario_cfg["name"],  # type: ignore
                 scoring.execution_metadata.model_cfg["name"],
             ][scoring.execution_metadata.augmenter_key] = scoring
-            if scoring.execution_metadata.augmenter_key is None:
-                scorings_to_keep.append(scoring)
-        scores.scorings = scorings_to_keep
 
         for (scenario_name, model_name), scorings in to_calculate.items():
             if len(scorings) != 2:
                 if list(scorings.keys()) != [None]:
                     logger.warning(
                         "Unfinished disparity score %s for scoring %s "
                         "on %s did not have 2 augmenters",
                         self.name,
                         scenario_name,
                         model_name,
                     )
                 continue
             out.append(
                 (
-                    f"{self.name}: {scenario_name}",
-                    model_name,
-                    self.dimension,
+                    sorted(scorings.values(), key=lambda scoring: scoring.timestamp)[
+                        0
+                    ].execution_metadata,
                     self.calculate_disparities(scorings),
                 )
             )
         return out
 
 
 class KeyStrokeRobustness(DisparityScoring):
@@ -201,7 +198,17 @@
 
 META_SCORERS = [
     TimingScore(),
     KeyStrokeRobustness(),
     GenderNameScore(),
     NameOriginScore(),
 ]
+
+
+def _should_skip_for_meta(scoring: Scoring, keys: tuple[Optional[str], ...]) -> bool:
+    if scoring.execution_metadata.augmenter_key not in keys:
+        return True
+    if scoring.is_meta:
+        return True
+    if scoring.execution_metadata.scenario_cfg.get("type", "standard") != "standard":
+        return True
+    return False
```

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/analysis/metrics.py` & `danoliterate-0.0.4/danoliterate/evaluation/analysis/metrics.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/analysis/scorer.py` & `danoliterate-0.0.4/danoliterate/evaluation/analysis/scorer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,39 @@
+from pathlib import Path
 from typing import Sequence
 
 from omegaconf import DictConfig
 from tqdm import tqdm
 
+from danoliterate.evaluation.analysis.meta_scorings import META_SCORERS
 from danoliterate.evaluation.analysis.metrics import Metric
-from danoliterate.evaluation.artifact_integration import (
-    get_results_wandb,
-    get_scores_wandb,
-    send_scores_wandb,
-    setup_short_run,
-)
 from danoliterate.evaluation.registries.metrics import get_compatible_metrics
 from danoliterate.evaluation.results import ExecutionResult, Scores, Scoring
-from danoliterate.infrastructure.logging import format_config, logger
+from danoliterate.infrastructure.constants import EXECUTION_RESULT_NAME
+from danoliterate.infrastructure.logging import format_config, logger, maybe_setup_wandb_logging_run
 from danoliterate.infrastructure.timing import from_timestamp
 
 
 class Scorer:
     def __init__(self, cfg: DictConfig):
         self.wandb_cfg = cfg.wandb
         self.eval_cfg = cfg.evaluation
 
         self.result = Scores.from_config(cfg)
 
-        self.wandb = setup_short_run(self.result.name, "score", self.wandb_cfg)
-        self.previous_result = (
-            None
-            if cfg.evaluation.rescore
-            else get_scores_wandb(cfg.wandb.project, cfg.wandb.entity)
-        )
+        maybe_setup_wandb_logging_run(self.result.name, "score", self.wandb_cfg)
+        self.previous_result = None if cfg.evaluation.rescore else Scores.from_local_result_db(cfg)
         self.combinations_to_skip: dict[str, Scoring] = {}
 
     def run(self):
-        logger.info("Fetching executed results ...")
-        results = get_results_wandb(
-            self.wandb_cfg.project,
-            self.wandb_cfg.entity,
-            cache_file=self.wandb_cfg.artifact_cache,
-            cache_update=self.wandb_cfg.cache_update,
-        )
+        logger.info("Fetching executed results locally from %s ...", self.eval_cfg.local_results)
+        results = [
+            ExecutionResult.from_path(path)
+            for path in Path(self.eval_cfg.local_results).glob(f"{EXECUTION_RESULT_NAME}*.json")
+        ]
         if (min_time := self.eval_cfg.do_not_score_before) is not None:
             len_before = len(results)
             results = [
                 result
                 for result in results
                 if from_timestamp(result.metadata.timestamp) >= from_timestamp(min_time)
             ]
@@ -55,17 +46,24 @@
         if self.previous_result is not None and not self.eval_cfg.rescore:
             self.combinations_to_skip = {
                 self._get_scoring_comparison_key(old_scoring, []): old_scoring
                 for old_scoring in self.previous_result.scorings
             }
         logger.info("Acquired %i execution results. Scoring ...", len(results))
         for result in tqdm(results):
-            if _should_skip(result):
-                continue
             self.result.scorings.append(self.score_result(result))
+        logger.info("Running meta scores")
+        meta_scorings = []
+        for meta_scorer in tqdm(META_SCORERS):
+            for metadata, metric_results in meta_scorer.meta_score(self.result):
+                meta_scoring = Scoring.from_execution_metadata(metadata)
+                meta_scoring.metric_results = metric_results
+                meta_scoring.is_meta = True
+                meta_scorings.append(meta_scoring)
+        self.result.scorings.extend(meta_scorings)
 
     def score_result(self, result: ExecutionResult) -> Scoring:
         scoring = Scoring.from_execution_metadata(result.metadata)
         metrics = get_compatible_metrics(
             result.metadata.scenario_cfg["task"]["type"],  # type: ignore
             result.metadata.model_cfg["inference"]["type"],  # type: ignore
             result.metadata.scenario_cfg,
@@ -94,42 +92,25 @@
             ", ".join(metric.name for metric in metrics),
         )
         for metric in metrics:
             scoring.metric_results.append(metric(result.examples))
         return scoring
 
     def save_scores(self):
-        if self.wandb is not None:
-            send_scores_wandb(self.result, self.wandb)
-            logger.info("Sucessfully sent scores to W&B.")
-
         out = self.result.save_locally()
         logger.info("Scores were saved locally to %s.", out)
 
     def _get_scoring_comparison_key(self, scoring: Scoring, metrics: Sequence[Metric]):
         metric_names = (
             [metric.name for metric in metrics]
             if metrics
             else [metric_res.short_name for metric_res in scoring.metric_results]
         )
         return scoring.execution_metadata.id_ + "-" + "-".join(sorted(metric_names))
 
 
-def _should_skip(result: ExecutionResult):
-    # TODO: Remove these partial results
-    if (mname := result.metadata.model_cfg["name"]) in {
-        "mGPT 13B",
-        "Hestenettet LM",
-        "SOLAR 10.7B",
-        "OpenAI Davinci 003",
-    }:
-        logger.warning("Manually skipped scoring of result for model %s", mname)
-        return True
-    return False
-
-
 def score(cfg: DictConfig):
     logger.debug("Running scoring with arguments: %s", format_config(cfg))
 
     scorer = Scorer(cfg)
     scorer.run()
     scorer.save_scores()
```

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/execution/augmentation.py` & `danoliterate-0.0.4/danoliterate/evaluation/execution/augmentation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+# pylint: disable=import-outside-toplevel
 from abc import ABC, abstractmethod
 from typing import Callable, Iterator
 
 import augmenty
 import spacy
 from augmenty.character.replace import create_keystroke_error_augmenter_v1
 from augmenty.util import Example
-from dacy.datasets import danish_names, female_names, male_names, muslim_names
 from omegaconf import DictConfig
 from spacy.language import Language
 
 from danoliterate.infrastructure.logging import logger
 
+DACY_IMPORT_ERROR = None
+try:
+    from dacy.datasets import danish_names, female_names, male_names, muslim_names
+except ImportError as _error:
+    DACY_IMPORT_ERROR = _error
+
 
 class Augmenter(ABC):
     @abstractmethod
     def __call__(self, text: str) -> str:
         ...
 
     @property
@@ -36,15 +42,16 @@
         self.augmenter = self.create_augmenter()
 
     def __call__(self, text: str) -> str:
         try:
             return list(augmenty.texts([text], augmenter=self.augmenter, nlp=self.nlp))[0]
         except ValueError as error:
             logger.warning(
-                "%s\nCould not augment text due to above error. Using it in non-augmented form. Text was:\n%s.",
+                "%s\nCould not augment text due to above error."
+                " Using it in non-augmented form. Text was:\n%s.",
                 error,
                 text,
             )
             return text
 
     @abstractmethod
     def create_augmenter(self) -> Callable[[Language, Example], Iterator[Example]]:
@@ -64,14 +71,18 @@
     @property
     def key(self):
         return "keystroke-error"
 
 
 class NameInserter(AugmentyBasedAugmenter, ABC):
     def __init__(self):
+        if DACY_IMPORT_ERROR is not None:
+            raise ImportError(
+                "To run name-based augmentation, you must install Dacy"
+            ) from DACY_IMPORT_ERROR
         self.names = self.get_names()
         super().__init__()
 
     @abstractmethod
     def get_names(self) -> dict[str, list[str]]:
         ...
```

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/execution/evaluator.py` & `danoliterate-0.0.4/danoliterate/evaluation/execution/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from time import perf_counter
 from typing import Generator, Optional
 
 from datasets import Dataset, load_dataset
 from omegaconf import DictConfig
 
-from danoliterate.evaluation.artifact_integration import send_result_wandb, setup_short_run
 from danoliterate.evaluation.execution.augmentation import Augmenter, get_augmenters
 from danoliterate.evaluation.execution.eval_types import EVALUATION_TYPES
 from danoliterate.evaluation.execution.model_inference import ModelInference, set_deterministic
 from danoliterate.evaluation.registries.inferences import get_inference
 from danoliterate.evaluation.registries.tasks import get_task_runner
 from danoliterate.evaluation.results import ExecutionExample, ExecutionResult
 from danoliterate.infrastructure import format_config
-from danoliterate.infrastructure.logging import logger
+from danoliterate.infrastructure.logging import logger, maybe_setup_wandb_logging_run
 
 
 class Evaluator:
     def __init__(
         self,
         cfg: DictConfig,
         scenario_cfg: DictConfig,
@@ -50,15 +49,15 @@
             self.train_dataset = load_dataset(
                 scenario_cfg.path,
                 split="train",
             )
 
         self.model_inference = model_inference
 
-        self.wandb = setup_short_run(self.result.name, "eval", cfg.wandb)
+        maybe_setup_wandb_logging_run(self.result.name, "eval", cfg.wandb)
         self.scenario_cfg: DictConfig = scenario_cfg
         if (eval_type := self.scenario_cfg.get("type")) is not None:
             assert eval_type in EVALUATION_TYPES, f"scenario.type must be one of {EVALUATION_TYPES}"
 
     def run(self):
         logger.info("Initializing example generators ...")
         examples = self.generate_examples()
@@ -70,17 +69,14 @@
             self.result.examples.append(result)
         self.result.metadata.total_inference_seconds = total_time = perf_counter() - start_time
         logger.info("Finished result loop in %.0f seconds.", total_time)
 
     def save_results(self):
         out = self.result.save_locally()
         logger.info("Result was saved locally to %s.", out)
-        if self.wandb is not None:
-            send_result_wandb(self.result, self.wandb)
-            logger.info("Sucessfully sent result to W&B.")
 
     def generate_examples(self) -> Generator[ExecutionExample, None, None]:
         for i, data_example in enumerate(self.dataset):
             args = {
                 "row": data_example,
                 "pre_prompt": self.scenario_cfg.get("pre_prompt", ""),
                 "post_prompt": self.scenario_cfg.get("post_prompt", ""),
```

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/execution/huggingface_inference.py` & `danoliterate-0.0.4/danoliterate/evaluation/execution/huggingface_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Any, Optional
 
 import torch
 from tqdm import tqdm
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from transformers.tokenization_utils_base import VERY_LARGE_INTEGER
 
 from danoliterate.evaluation.execution.model_inference import ModelInference
@@ -25,15 +25,16 @@
     # TODO: Should be set at scenario level
     max_new_tokens = 256
     default_max_length = 1024
 
     def __init__(self, hf_key: str, batch_size=1, auto_device_map=False, download_no_cache=False):
         super().__init__()
 
-        init_kwargs = {}
+        # TODO: Should be in generation config
+        init_kwargs: dict[str, Any] = {"use_cache": True}
         if auto_device_map:
             init_kwargs["device_map"] = "auto"
         model_cls = AutoModelForCausalLM
         self.model = (
             from_pretrained_hf_hub_no_disk(hf_key, model_cls)
             if download_no_cache
             else model_cls.from_pretrained(hf_key, **init_kwargs)
@@ -86,15 +87,14 @@
                         return_token_type_ids=False,
                     ).to(DEVICE)
                     with torch.inference_mode():
                         outputs = self.model.generate(
                             **model_inputs,
                             max_new_tokens=self.max_new_tokens,
                             do_sample=False,
-                            temperature=0,
                             return_dict_in_generate=True,
                             output_scores=True,
                         )
                     input_id_len = model_inputs.input_ids.shape[1]
                     texts = self.tokenizer.batch_decode(
                         outputs.sequences[:, input_id_len:],
                         skip_special_tokens=True,
```

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/execution/model_inference.py` & `danoliterate-0.0.4/danoliterate/evaluation/execution/model_inference.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/execution/task_runner.py` & `danoliterate-0.0.4/danoliterate/evaluation/execution/task_runner.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/registries/metrics.py` & `danoliterate-0.0.4/danoliterate/evaluation/registries/metrics.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/registries/tasks.py` & `danoliterate-0.0.4/danoliterate/evaluation/registries/tasks.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/results.py` & `danoliterate-0.0.4/danoliterate/evaluation/results.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from danoliterate.evaluation.serialization import (
     OutDictType,
     apply_backcomp_fixes_execution_example,
     apply_backcomp_fixes_execution_result_metadata,
     apply_backcomp_reordering_metric_results,
     fix_args_for_dataclass,
 )
-from danoliterate.infrastructure.constants import SCORES_ARTIFACT_TYPE
+from danoliterate.infrastructure.constants import EXECUTION_RESULT_NAME, SCORES_NAME
 from danoliterate.infrastructure.logging import commit_hash, get_compute_unit_string, logger
 from danoliterate.infrastructure.timing import get_now_stamp
 
 
 # pylint: disable=too-many-instance-attributes
 @dataclass
 class ExecutionExample:
@@ -53,15 +53,14 @@
 
     scenario_cfg: OutDictType
     model_cfg: OutDictType
     evaluation_cfg: OutDictType
 
     augmenter_key: Optional[str] = None
     total_inference_seconds: Optional[float] = None
-    sent_to_wandb: bool = False
 
     def to_dict(self) -> OutDictType:
         return asdict(self)
 
     @classmethod
     def from_dict(cls, self_dict: OutDictType):
         fix_args_for_dataclass(cls, self_dict)
@@ -101,15 +100,15 @@
             name_part.replace(".", "").replace(" ", "-").lower() for name_part in name_parts
         )
 
         results_path = Path(cfg.evaluation.local_results)
         if not results_path.is_dir():
             logger.warning("Creating new local directory for results: %s", results_path)
             os.makedirs(results_path)
-        out_path = results_path / f"{autoname}.json"
+        out_path = results_path / f"{EXECUTION_RESULT_NAME}.{autoname}.json"
 
         return cls(
             name=autoname,
             local_path=out_path,
             metadata=ExecutionResultMetadata(
                 **metadata_fields,  # type: ignore
                 scenario_cfg=conf_to_dict(scenario_cfg),
@@ -128,14 +127,19 @@
             logger.warning("Fixing erroneuous extra list in examples field!")
             self_dict["examples"] = self_dict["examples"][0]
 
         example_dicts: list[OutDictType] = self_dict.pop("examples")  # type: ignore
         examples = [ExecutionExample.from_dict(example_dict) for example_dict in example_dicts]
         return cls(metadata=metadata, examples=examples, **self_dict)  # type: ignore
 
+    @classmethod
+    def from_path(cls, path: str | Path):
+        with open(path, "r", encoding="utf-8") as file:
+            return cls.from_dict(json.load(file))
+
 
 @dataclass
 class MetricResult:
     short_name: str
     description: str
 
     # Maps single example ID to either a float describing a score in [0, 1]
@@ -164,14 +168,16 @@
     commit: Optional[str]
     compute_unit: Optional[str]
 
     execution_metadata: ExecutionResultMetadata
 
     metric_results: list[MetricResult]
 
+    is_meta: bool = False
+
     @classmethod
     def from_execution_metadata(cls, metadata: ExecutionResultMetadata):
         return cls(
             **get_reproducability_metadata_fields(),  # type: ignore
             execution_metadata=metadata,
             metric_results=[],
         )
@@ -199,32 +205,42 @@
 @dataclass
 class Scores:
     scorings: list[Scoring]
     local_path: str | os.PathLike
 
     debug: bool
 
-    sent_to_wandb = False
-    name = SCORES_ARTIFACT_TYPE
+    name = SCORES_NAME
 
     @classmethod
-    def from_config(cls, cfg: DictConfig):
+    def from_config(cls, cfg: DictConfig) -> "Scores":
         autoname = f"{cls.name}-{get_now_stamp()}"
         results_path = Path(cfg.evaluation.local_results)
         if not results_path.is_dir():
             logger.warning("Creating new local directory for results: %s", results_path)
             results_path.mkdir()
             os.makedirs(results_path)
         out_path = results_path / f"{autoname}.json"
         return cls(
             local_path=out_path,
             scorings=[],
             debug=cfg.evaluation.debug,
         )
 
+    @classmethod
+    def from_local_result_db(cls, cfg: DictConfig) -> "None | Scores":
+        result_db_path = Path(cfg.evaluation.local_results)
+        all_possible_scores = list(result_db_path.glob(f"{SCORES_NAME}*.json"))
+        if not all_possible_scores:
+            logger.warning("Found no previous scores in %s", result_db_path)
+            return None
+        newest_scores_path = sorted(all_possible_scores)[-1]
+        with open(newest_scores_path, "r", encoding="utf-8") as file:
+            return cls.from_dict(json.load(file))
+
     def to_dict(self) -> OutDictType:
         self_dict = asdict(self)
         self_dict["scorings"] = [scoring.to_dict() for scoring in self.scorings]
         return self_dict
 
     @classmethod
     def from_dict(cls, self_dict: OutDictType):
```

### Comparing `danoliterate-0.0.3/danoliterate/evaluation/serialization.py` & `danoliterate-0.0.4/danoliterate/evaluation/serialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,30 +26,38 @@
     "gpt-4-1106-preview": "OpenAI GPT 4 Turbo",
 }
 
 
 def apply_backcomp_fixes_execution_result_metadata(input_args: OutDictType):
     warnings = []
     model_cfg: OutDictType = input_args["model_cfg"]  # type: ignore
-    if (new_name := MODEL_KEY_TO_NEW_NAME.get(model_cfg.get("path"))) is not None:
+    if (new_name := MODEL_KEY_TO_NEW_NAME.get(model_cfg.get("path"))) is not None:  # type: ignore
         model_cfg["name"] = new_name
     scenario_cfg: OutDictType = input_args["scenario_cfg"]  # type: ignore
     task_type: str = scenario_cfg["task"]["type"]  # type: ignore
     scenario_name: str = scenario_cfg["name"]  # type: ignore
     scenario_type: Optional[str] = scenario_cfg.get("type")  # type: ignore
+
     if (desired_task_type := SCENARIO_NAME_TO_TASK_TYPE.get(scenario_name)) is not None or (
         desired_task_type := SCENARIO_NAME_AND_TYPE_TO_TASK_TYPE.get((scenario_name, scenario_type))
     ) is not None:
         if task_type != desired_task_type:
             scenario_cfg["task"]["type"] = desired_task_type  # type: ignore
             warnings.append(f"Changed {scenario_cfg['name']} task type to {desired_task_type}")
-
     elif (new_name := TASK_TYPE_RENAMES.get(task_type)) is not None:
         scenario_cfg["task"]["type"] = new_name  # type: ignore
         warnings.append(f"Renamed {task_type} to {new_name}.")
+
+    if "ScandEval" in scenario_cfg["path"]:  # type: ignore
+        scenario_cfg["path"] = n_path = (old_path := scenario_cfg["path"]).replace(  # type: ignore
+            "ScandEval", "sorenmulli"
+        )
+        scenario_cfg["dataset_split"] = "validation"
+        warnings.append(f"Renamed {old_path} to {n_path}.")
+
     if warnings:
         logger.debug("Performed backwards compatability fixing:\n%s", ",".join(warnings))
 
 
 RENAME_OPTIONS = {
     "negative": "negativ",
     "positive": "positiv",
```

### Comparing `danoliterate-0.0.3/danoliterate/modeling/gpt_ner_alignment.py` & `danoliterate-0.0.4/danoliterate/modeling/gpt_ner_alignment.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/modeling/language_identification.py` & `danoliterate-0.0.4/danoliterate/modeling/language_identification.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/modeling/load_model.py` & `danoliterate-0.0.4/danoliterate/modeling/load_model.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/modeling/ngram_language_modeling.py` & `danoliterate-0.0.4/danoliterate/modeling/ngram_language_modeling.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/modeling/text_classification.py` & `danoliterate-0.0.4/danoliterate/modeling/text_classification.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/modeling/text_comparison.py` & `danoliterate-0.0.4/danoliterate/modeling/text_comparison.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/modeling/uncertainty_estimation.py` & `danoliterate-0.0.4/danoliterate/modeling/uncertainty_estimation.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/training/efficiency.py` & `danoliterate-0.0.4/danoliterate/training/efficiency.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate/training/lm_training.py` & `danoliterate-0.0.4/danoliterate/training/lm_training.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/danoliterate.egg-info/PKG-INFO` & `danoliterate-0.0.4/danoliterate.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6461 6e6f  : 2.1.Name: dano
 00000020: 6c69 7465 7261 7465 0a56 6572 7369 6f6e  literate.Version
-00000030: 3a20 302e 302e 330a 5375 6d6d 6172 793a  : 0.0.3.Summary:
+00000030: 3a20 302e 302e 340a 5375 6d6d 6172 793a  : 0.0.4.Summary:
 00000040: 2042 656e 6368 6d61 726b 206f 6620 4765   Benchmark of Ge
 00000050: 6e65 7261 7469 7665 204c 6172 6765 204c  nerative Large L
 00000060: 616e 6775 6167 6520 4d6f 6465 6c73 2069  anguage Models i
 00000070: 6e20 4461 6e69 7368 0a48 6f6d 652d 7061  n Danish.Home-pa
 00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000090: 7562 2e63 6f6d 2f73 6f72 656e 6d75 6c6c  ub.com/sorenmull
 000000a0: 692f 6461 6e6f 6c69 7465 7261 7465 0a41  i/danoliterate.A
@@ -21,137 +21,235 @@
 00000140: 2070 616e 6461 737e 3d31 2e35 2e33 0a52   pandas~=1.5.3.R
 00000150: 6571 7569 7265 732d 4469 7374 3a20 6461  equires-Dist: da
 00000160: 7461 7365 7473 7e3d 322e 3134 2e35 0a52  tasets~=2.14.5.R
 00000170: 6571 7569 7265 732d 4469 7374 3a20 7472  equires-Dist: tr
 00000180: 616e 7366 6f72 6d65 7273 7e3d 342e 3336  ansformers~=4.36
 00000190: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
 000001a0: 3a20 746f 7263 687e 3d32 2e31 2e31 0a52  : torch~=2.1.1.R
-000001b0: 6571 7569 7265 732d 4469 7374 3a20 6163  equires-Dist: ac
-000001c0: 6365 6c65 7261 7465 7e3d 302e 3233 2e30  celerate~=0.23.0
+000001b0: 6571 7569 7265 732d 4469 7374 3a20 7361  equires-Dist: sa
+000001c0: 6665 7465 6e73 6f72 737e 3d30 2e33 2e33  fetensors~=0.3.3
 000001d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000001e0: 7361 6665 7465 6e73 6f72 737e 3d30 2e33  safetensors~=0.3
-000001f0: 2e33 0a52 6571 7569 7265 732d 4469 7374  .3.Requires-Dist
-00000200: 3a20 6d61 7470 6c6f 746c 6962 7e3d 332e  : matplotlib~=3.
-00000210: 382e 300a 5265 7175 6972 6573 2d44 6973  8.0.Requires-Dis
-00000220: 743a 2073 696d 706c 652d 7465 726d 2d6d  t: simple-term-m
-00000230: 656e 757e 3d31 2e36 2e31 0a52 6571 7569  enu~=1.6.1.Requi
-00000240: 7265 732d 4469 7374 3a20 6461 6e6c 707e  res-Dist: danlp~
-00000250: 3d30 2e31 2e32 0a52 6571 7569 7265 732d  =0.1.2.Requires-
-00000260: 4469 7374 3a20 6765 6e73 696d 7e3d 342e  Dist: gensim~=4.
-00000270: 332e 320a 5265 7175 6972 6573 2d44 6973  3.2.Requires-Dis
-00000280: 743a 2064 6565 7073 7065 6564 7e3d 302e  t: deepspeed~=0.
-00000290: 3132 2e34 0a52 6571 7569 7265 732d 4469  12.4.Requires-Di
-000002a0: 7374 3a20 7365 6e74 656e 6365 7069 6563  st: sentencepiec
-000002b0: 657e 3d30 2e31 2e39 390a 5265 7175 6972  e~=0.1.99.Requir
-000002c0: 6573 2d44 6973 743a 2061 7567 6d65 6e74  es-Dist: augment
-000002d0: 797e 3d31 2e34 2e33 0a52 6571 7569 7265  y~=1.4.3.Require
-000002e0: 732d 4469 7374 3a20 6461 6379 7e3d 322e  s-Dist: dacy~=2.
-000002f0: 372e 360a 5265 7175 6972 6573 2d44 6973  7.6.Requires-Dis
-00000300: 743a 2067 6f6f 676c 652d 636c 6f75 642d  t: google-cloud-
-00000310: 6169 706c 6174 666f 726d 7e3d 312e 3338  aiplatform~=1.38
-00000320: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
-00000330: 3a20 6f70 656e 6169 7e3d 302e 3238 2e31  : openai~=0.28.1
-00000340: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000350: 7374 7265 616d 6c69 747e 3d31 2e32 372e  streamlit~=1.27.
-00000360: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-00000370: 2068 7567 6769 6e67 6661 6365 5f68 7562   huggingface_hub
-00000380: 7e3d 302e 3139 2e34 0a52 6571 7569 7265  ~=0.19.4.Require
-00000390: 732d 4469 7374 3a20 6879 6472 612d 636f  s-Dist: hydra-co
-000003a0: 7265 7e3d 312e 332e 320a 5265 7175 6972  re~=1.3.2.Requir
-000003b0: 6573 2d44 6973 743a 2068 7964 7261 2d63  es-Dist: hydra-c
-000003c0: 6f6c 6f72 6c6f 677e 3d31 2e32 2e30 0a52  olorlog~=1.2.0.R
-000003d0: 6571 7569 7265 732d 4469 7374 3a20 6f6d  equires-Dist: om
-000003e0: 6567 6163 6f6e 667e 3d32 2e33 2e30 0a52  egaconf~=2.3.0.R
-000003f0: 6571 7569 7265 732d 4469 7374 3a20 7761  equires-Dist: wa
-00000400: 6e64 627e 3d30 2e31 352e 3131 0a52 6571  ndb~=0.15.11.Req
-00000410: 7569 7265 732d 4469 7374 3a20 6769 7470  uires-Dist: gitp
-00000420: 7974 686f 6e7e 3d33 2e31 2e33 370a 5265  ython~=3.1.37.Re
-00000430: 7175 6972 6573 2d44 6973 743a 2062 6c61  quires-Dist: bla
-00000440: 636b 7e3d 3233 2e37 2e30 0a52 6571 7569  ck~=23.7.0.Requi
-00000450: 7265 732d 4469 7374 3a20 6973 6f72 747e  res-Dist: isort~
-00000460: 3d35 2e31 322e 300a 5265 7175 6972 6573  =5.12.0.Requires
-00000470: 2d44 6973 743a 206d 7970 797e 3d31 2e35  -Dist: mypy~=1.5
-00000480: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
-00000490: 3a20 7079 6c69 6e74 7e3d 322e 3137 2e35  : pylint~=2.17.5
-000004a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004b0: 7061 6e64 6173 2d73 7475 6273 7e3d 322e  pandas-stubs~=2.
-000004c0: 302e 330a 5265 7175 6972 6573 2d44 6973  0.3.Requires-Dis
-000004d0: 743a 2074 7970 6573 2d74 7164 6d7e 3d34  t: types-tqdm~=4
-000004e0: 2e36 362e 300a 5265 7175 6972 6573 2d44  .66.0.Requires-D
-000004f0: 6973 743a 2074 7970 6573 2d72 6571 7565  ist: types-reque
-00000500: 7374 737e 3d32 2e33 312e 300a 5072 6f76  sts~=2.31.0.Prov
-00000510: 6964 6573 2d45 7874 7261 3a20 6675 6c6c  ides-Extra: full
-00000520: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000530: 7079 7064 667e 3d33 2e31 362e 313b 2065  pypdf~=3.16.1; e
-00000540: 7874 7261 203d 3d20 2266 756c 6c22 0a52  xtra == "full".R
-00000550: 6571 7569 7265 732d 4469 7374 3a20 6661  equires-Dist: fa
-00000560: 7374 7465 7874 2d77 6865 656c 7e3d 302e  sttext-wheel~=0.
-00000570: 392e 323b 2065 7874 7261 203d 3d20 2266  9.2; extra == "f
-00000580: 756c 6c22 0a52 6571 7569 7265 732d 4469  ull".Requires-Di
-00000590: 7374 3a20 7065 6674 7e3d 302e 352e 303b  st: peft~=0.5.0;
-000005a0: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
-000005b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000005c0: 7363 6970 797e 3d31 2e31 312e 333b 2065  scipy~=1.11.3; e
-000005d0: 7874 7261 203d 3d20 2266 756c 6c22 0a52  xtra == "full".R
-000005e0: 6571 7569 7265 732d 4469 7374 3a20 6e6c  equires-Dist: nl
-000005f0: 746b 7e3d 332e 382e 313b 2065 7874 7261  tk~=3.8.1; extra
-00000600: 203d 3d20 2266 756c 6c22 0a52 6571 7569   == "full".Requi
-00000610: 7265 732d 4469 7374 3a20 726f 7567 655f  res-Dist: rouge_
-00000620: 7363 6f72 657e 3d30 2e31 2e32 3b20 6578  score~=0.1.2; ex
-00000630: 7472 6120 3d3d 2022 6675 6c6c 220a 5265  tra == "full".Re
-00000640: 7175 6972 6573 2d44 6973 743a 2065 7661  quires-Dist: eva
-00000650: 6c75 6174 657e 3d30 2e34 2e30 3b20 6578  luate~=0.4.0; ex
-00000660: 7472 6120 3d3d 2022 6675 6c6c 220a 5265  tra == "full".Re
-00000670: 7175 6972 6573 2d44 6973 743a 2062 6572  quires-Dist: ber
-00000680: 745f 7363 6f72 657e 3d30 2e33 2e31 333b  t_score~=0.3.13;
-00000690: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
-000006a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000006b0: 7370 6163 797e 3d33 2e35 2e34 3b20 6578  spacy~=3.5.4; ex
-000006c0: 7472 6120 3d3d 2022 6675 6c6c 220a 5265  tra == "full".Re
-000006d0: 7175 6972 6573 2d44 6973 743a 206c 6576  quires-Dist: lev
-000006e0: 656e 7368 7465 696e 7e3d 302e 3233 2e30  enshtein~=0.23.0
-000006f0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
-00000700: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000710: 2073 6571 6576 616c 7e3d 312e 322e 323b   seqeval~=1.2.2;
-00000720: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
-00000730: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000740: 6265 6175 7469 6675 6c73 6f75 7034 7e3d  beautifulsoup4~=
-00000750: 342e 3132 2e32 3b20 6578 7472 6120 3d3d  4.12.2; extra ==
-00000760: 2022 6675 6c6c 220a 5265 7175 6972 6573   "full".Requires
-00000770: 2d44 6973 743a 2074 726c 7e3d 302e 372e  -Dist: trl~=0.7.
-00000780: 343b 2065 7874 7261 203d 3d20 2266 756c  4; extra == "ful
-00000790: 6c22 0a0a 2320 4172 6520 4c4c 4d73 2044  l"..# Are LLMs D
-000007a0: 616e 6f6c 6974 6572 6174 653f 0a0a 0a41  anoliterate?...A
-000007b0: 2062 656e 6368 6d61 726b 2074 6f6f 6c20   benchmark tool 
-000007c0: 666f 7220 4765 6e65 7261 7469 7665 204c  for Generative L
-000007d0: 6172 6765 204c 616e 6775 6167 6520 4d6f  arge Language Mo
-000007e0: 6465 6c73 2069 6e20 4461 6e69 7368 2e0a  dels in Danish..
-000007f0: 0a4e 6f74 653a 2054 6869 7320 7265 706f  .Note: This repo
-00000800: 7369 746f 7279 2069 7320 6375 7272 656e  sitory is curren
-00000810: 746c 7920 776f 726b 2d69 6e2d 7072 6f67  tly work-in-prog
-00000820: 7265 7373 2077 6869 6c65 2074 6865 206d  ress while the m
-00000830: 6173 7465 7227 7320 7468 6573 6973 2069  aster's thesis i
-00000840: 7320 6669 6e69 7368 6564 2e0a 496d 706c  s finished..Impl
-00000850: 656d 656e 7461 7469 6f6e 7320 6172 6520  ementations are 
-00000860: 7375 626a 6563 7420 746f 2063 6861 6e67  subject to chang
-00000870: 652e 0a0a 2323 2049 6e73 7461 6c6c 6174  e...## Installat
-00000880: 696f 6e0a 0a54 6865 2070 6163 6b61 6765  ion..The package
-00000890: 2068 6173 2062 6565 6e20 6465 7665 6c6f   has been develo
-000008a0: 7065 6420 616e 6420 7573 6564 2077 6974  ped and used wit
-000008b0: 6820 5079 7468 6f6e 2033 2e31 312e 0a54  h Python 3.11..T
-000008c0: 6f20 696e 7374 616c 6c20 7468 6520 7061  o install the pa
-000008d0: 636b 6167 6520 696e 2061 2062 6173 6520  ckage in a base 
-000008e0: 7665 7273 696f 6e2c 2065 6e61 626c 696e  version, enablin
-000008f0: 6720 6d6f 6465 6c20 6578 6563 7574 696f  g model executio
-00000900: 6e2c 2069 6e73 7461 6c6c 0a60 6060 0a70  n, install.```.p
-00000910: 6970 2069 6e73 7461 6c6c 2064 616e 6f6c  ip install danol
-00000920: 6974 6572 6174 650a 6060 600a 0a54 6f20  iterate.```..To 
-00000930: 696e 7374 616c 6c20 6974 2077 6974 6820  install it with 
-00000940: 7468 6520 656e 7469 7265 2073 7569 7465  the entire suite
-00000950: 206f 6620 6465 7065 6e64 656e 6369 6573   of dependencies
-00000960: 2074 6861 7420 7765 7265 2075 7365 6420   that were used 
-00000970: 696e 2074 6865 7369 732c 2072 756e 200a  in thesis, run .
-00000980: 6060 600a 6d61 6b65 2069 6e73 7461 6c6c  ```.make install
-00000990: 0a60 6060 0a0a 2323 2055 7361 6765 0a0a  .```..## Usage..
-000009a0: 6060 600a 7079 7468 6f6e 202d 6d20 6461  ```.python -m da
-000009b0: 6e6f 6c69 7465 7261 7465 2064 6f3d 6576  noliterate do=ev
-000009c0: 616c 7561 7465 0a60 6060 0a              aluate.```.
+000001e0: 6d61 7470 6c6f 746c 6962 7e3d 332e 382e  matplotlib~=3.8.
+000001f0: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
+00000200: 2073 696d 706c 652d 7465 726d 2d6d 656e   simple-term-men
+00000210: 757e 3d31 2e36 2e31 0a52 6571 7569 7265  u~=1.6.1.Require
+00000220: 732d 4469 7374 3a20 6175 676d 656e 7479  s-Dist: augmenty
+00000230: 7e3d 312e 342e 340a 5265 7175 6972 6573  ~=1.4.4.Requires
+00000240: 2d44 6973 743a 2073 6571 6576 616c 7e3d  -Dist: seqeval~=
+00000250: 312e 322e 320a 5265 7175 6972 6573 2d44  1.2.2.Requires-D
+00000260: 6973 743a 206c 6576 656e 7368 7465 696e  ist: levenshtein
+00000270: 7e3d 302e 3233 2e30 0a52 6571 7569 7265  ~=0.23.0.Require
+00000280: 732d 4469 7374 3a20 6e6c 746b 7e3d 332e  s-Dist: nltk~=3.
+00000290: 382e 310a 5265 7175 6972 6573 2d44 6973  8.1.Requires-Dis
+000002a0: 743a 2061 6273 6c2d 7079 7e3d 322e 312e  t: absl-py~=2.1.
+000002b0: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
+000002c0: 2065 7661 6c75 6174 657e 3d30 2e34 2e30   evaluate~=0.4.0
+000002d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000002e0: 726f 7567 655f 7363 6f72 657e 3d30 2e31  rouge_score~=0.1
+000002f0: 2e32 0a52 6571 7569 7265 732d 4469 7374  .2.Requires-Dist
+00000300: 3a20 6265 7274 5f73 636f 7265 7e3d 302e  : bert_score~=0.
+00000310: 332e 3133 0a52 6571 7569 7265 732d 4469  3.13.Requires-Di
+00000320: 7374 3a20 6765 6e73 696d 7e3d 342e 332e  st: gensim~=4.3.
+00000330: 320a 5265 7175 6972 6573 2d44 6973 743a  2.Requires-Dist:
+00000340: 2064 616e 6c70 7e3d 302e 312e 320a 5265   danlp~=0.1.2.Re
+00000350: 7175 6972 6573 2d44 6973 743a 2068 7567  quires-Dist: hug
+00000360: 6769 6e67 6661 6365 5f68 7562 7e3d 302e  gingface_hub~=0.
+00000370: 3139 2e34 0a52 6571 7569 7265 732d 4469  19.4.Requires-Di
+00000380: 7374 3a20 6879 6472 612d 636f 7265 7e3d  st: hydra-core~=
+00000390: 312e 332e 320a 5265 7175 6972 6573 2d44  1.3.2.Requires-D
+000003a0: 6973 743a 2068 7964 7261 2d63 6f6c 6f72  ist: hydra-color
+000003b0: 6c6f 677e 3d31 2e32 2e30 0a52 6571 7569  log~=1.2.0.Requi
+000003c0: 7265 732d 4469 7374 3a20 6f6d 6567 6163  res-Dist: omegac
+000003d0: 6f6e 667e 3d32 2e33 2e30 0a52 6571 7569  onf~=2.3.0.Requi
+000003e0: 7265 732d 4469 7374 3a20 6769 7470 7974  res-Dist: gitpyt
+000003f0: 686f 6e7e 3d33 2e31 2e33 370a 5265 7175  hon~=3.1.37.Requ
+00000400: 6972 6573 2d44 6973 743a 2062 6c61 636b  ires-Dist: black
+00000410: 7e3d 3233 2e37 2e30 0a52 6571 7569 7265  ~=23.7.0.Require
+00000420: 732d 4469 7374 3a20 6973 6f72 747e 3d35  s-Dist: isort~=5
+00000430: 2e31 322e 300a 5265 7175 6972 6573 2d44  .12.0.Requires-D
+00000440: 6973 743a 206d 7970 797e 3d31 2e35 2e31  ist: mypy~=1.5.1
+00000450: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000460: 7079 6c69 6e74 7e3d 322e 3137 2e35 0a52  pylint~=2.17.5.R
+00000470: 6571 7569 7265 732d 4469 7374 3a20 7061  equires-Dist: pa
+00000480: 6e64 6173 2d73 7475 6273 7e3d 322e 302e  ndas-stubs~=2.0.
+00000490: 330a 5265 7175 6972 6573 2d44 6973 743a  3.Requires-Dist:
+000004a0: 2074 7970 6573 2d74 7164 6d7e 3d34 2e36   types-tqdm~=4.6
+000004b0: 362e 300a 5265 7175 6972 6573 2d44 6973  6.0.Requires-Dis
+000004c0: 743a 2074 7970 6573 2d72 6571 7565 7374  t: types-request
+000004d0: 737e 3d32 2e33 312e 300a 5072 6f76 6964  s~=2.31.0.Provid
+000004e0: 6573 2d45 7874 7261 3a20 6675 6c6c 0a52  es-Extra: full.R
+000004f0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000500: 7064 667e 3d33 2e31 362e 313b 2065 7874  pdf~=3.16.1; ext
+00000510: 7261 203d 3d20 2266 756c 6c22 0a52 6571  ra == "full".Req
+00000520: 7569 7265 732d 4469 7374 3a20 6661 7374  uires-Dist: fast
+00000530: 7465 7874 2d77 6865 656c 7e3d 302e 392e  text-wheel~=0.9.
+00000540: 323b 2065 7874 7261 203d 3d20 2266 756c  2; extra == "ful
+00000550: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
+00000560: 3a20 7065 6674 7e3d 302e 352e 303b 2065  : peft~=0.5.0; e
+00000570: 7874 7261 203d 3d20 2266 756c 6c22 0a52  xtra == "full".R
+00000580: 6571 7569 7265 732d 4469 7374 3a20 7363  equires-Dist: sc
+00000590: 6970 797e 3d31 2e31 312e 333b 2065 7874  ipy~=1.11.3; ext
+000005a0: 7261 203d 3d20 2266 756c 6c22 0a52 6571  ra == "full".Req
+000005b0: 7569 7265 732d 4469 7374 3a20 7370 6163  uires-Dist: spac
+000005c0: 797e 3d33 2e35 2e34 3b20 6578 7472 6120  y~=3.5.4; extra 
+000005d0: 3d3d 2022 6675 6c6c 220a 5265 7175 6972  == "full".Requir
+000005e0: 6573 2d44 6973 743a 2062 6561 7574 6966  es-Dist: beautif
+000005f0: 756c 736f 7570 347e 3d34 2e31 322e 323b  ulsoup4~=4.12.2;
+00000600: 2065 7874 7261 203d 3d20 2266 756c 6c22   extra == "full"
+00000610: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000620: 7472 6c7e 3d30 2e37 2e34 3b20 6578 7472  trl~=0.7.4; extr
+00000630: 6120 3d3d 2022 6675 6c6c 220a 5265 7175  a == "full".Requ
+00000640: 6972 6573 2d44 6973 743a 2077 616e 6462  ires-Dist: wandb
+00000650: 7e3d 302e 3136 2e36 3b20 6578 7472 6120  ~=0.16.6; extra 
+00000660: 3d3d 2022 6675 6c6c 220a 5265 7175 6972  == "full".Requir
+00000670: 6573 2d44 6973 743a 2064 6565 7073 7065  es-Dist: deepspe
+00000680: 6564 7e3d 302e 3132 2e34 3b20 6578 7472  ed~=0.12.4; extr
+00000690: 6120 3d3d 2022 6675 6c6c 220a 5265 7175  a == "full".Requ
+000006a0: 6972 6573 2d44 6973 743a 2073 656e 7465  ires-Dist: sente
+000006b0: 6e63 6570 6965 6365 7e3d 302e 312e 3939  ncepiece~=0.1.99
+000006c0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
+000006d0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000006e0: 2061 6363 656c 6572 6174 657e 3d30 2e32   accelerate~=0.2
+000006f0: 332e 303b 2065 7874 7261 203d 3d20 2266  3.0; extra == "f
+00000700: 756c 6c22 0a52 6571 7569 7265 732d 4469  ull".Requires-Di
+00000710: 7374 3a20 676f 6f67 6c65 2d63 6c6f 7564  st: google-cloud
+00000720: 2d61 6970 6c61 7466 6f72 6d7e 3d31 2e33  -aiplatform~=1.3
+00000730: 382e 313b 2065 7874 7261 203d 3d20 2266  8.1; extra == "f
+00000740: 756c 6c22 0a52 6571 7569 7265 732d 4469  ull".Requires-Di
+00000750: 7374 3a20 6f70 656e 6169 7e3d 302e 3238  st: openai~=0.28
+00000760: 2e31 3b20 6578 7472 6120 3d3d 2022 6675  .1; extra == "fu
+00000770: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000780: 743a 2061 6e74 6872 6f70 6963 7e3d 302e  t: anthropic~=0.
+00000790: 3231 2e33 3b20 6578 7472 6120 3d3d 2022  21.3; extra == "
+000007a0: 6675 6c6c 220a 5265 7175 6972 6573 2d44  full".Requires-D
+000007b0: 6973 743a 2067 726f 713d 3d30 2e34 2e32  ist: groq==0.4.2
+000007c0: 3b20 6578 7472 6120 3d3d 2022 6675 6c6c  ; extra == "full
+000007d0: 220a 0a23 2041 7265 204c 4c4d 7320 4461  "..# Are LLMs Da
+000007e0: 6e6f 6c69 7465 7261 7465 3f0a 0a41 2062  noliterate?..A b
+000007f0: 656e 6368 6d61 726b 2066 6f72 2047 656e  enchmark for Gen
+00000800: 6572 6174 6976 6520 4c61 7267 6520 4c61  erative Large La
+00000810: 6e67 7561 6765 204d 6f64 656c 7320 696e  nguage Models in
+00000820: 2044 616e 6973 682e 200a 546f 2073 6565   Danish. .To see
+00000830: 2072 6573 756c 7473 2061 6e64 2061 6e64   results and and
+00000840: 2067 6574 206d 6f72 6520 6465 7461 696c   get more detail
+00000850: 732c 2063 6865 636b 206f 7574 2074 6865  s, check out the
+00000860: 206c 6561 6465 7262 6f61 7264 2073 6974   leaderboard sit
+00000870: 653a 0a0a 3c70 2061 6c69 676e 3d22 6365  e:..<p align="ce
+00000880: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
+00000890: 6874 7470 733a 2f2f 6461 6e6f 6c69 7465  https://danolite
+000008a0: 7261 7465 2e63 6f6d 7075 7465 2e64 7475  rate.compute.dtu
+000008b0: 2e64 6b2f 223e 6461 6e6f 6c69 7465 7261  .dk/">danolitera
+000008c0: 7465 2e63 6f6d 7075 7465 2e64 7475 2e64  te.compute.dtu.d
+000008d0: 6b3c 2f61 3e0a 3c2f 703e 0a0a 5468 6520  k</a>.</p>..The 
+000008e0: 7072 6f6a 6563 7420 6973 206d 6169 6e74  project is maint
+000008f0: 6169 6e65 6420 6279 2053 c3b8 7265 6e20  ained by S..ren 
+00000900: 5665 6a6c 6761 6172 6420 486f 6c6d 2061  Vejlgaard Holm a
+00000910: 7420 4454 5520 436f 6d70 7574 652c 2073  t DTU Compute, s
+00000920: 7570 706f 7274 6564 2062 7920 7468 6520  upported by the 
+00000930: 4461 6e69 7368 2050 696f 6e65 6572 2043  Danish Pioneer C
+00000940: 656e 7472 6520 666f 7220 4149 2061 6e64  entre for AI and
+00000950: 2077 6974 6820 6d6f 7374 206f 6620 7468   with most of th
+00000960: 6520 776f 726b 2064 6f6e 6520 6173 2070  e work done as p
+00000970: 6172 7420 6f66 2074 6865 204d 6173 7465  art of the Maste
+00000980: 7227 7320 7468 6573 6973 205b 2727 4172  r's thesis [''Ar
+00000990: 6520 474c 4c4d 7320 4461 6e6f 6c69 7465  e GLLMs Danolite
+000009a0: 7261 7465 3f20 4265 6e63 686d 6172 6b69  rate? Benchmarki
+000009b0: 6e67 2047 656e 6572 6174 6976 6520 4e4c  ng Generative NL
+000009c0: 5020 696e 2044 616e 6973 6827 275d 2868  P in Danish''](h
+000009d0: 7474 7073 3a2f 2f73 6f72 656e 6d75 6c6c  ttps://sorenmull
+000009e0: 692e 6769 7468 7562 2e69 6f2f 7468 6573  i.github.io/thes
+000009f0: 6973 2f74 6865 7369 732e 7064 6629 2073  is/thesis.pdf) s
+00000a00: 7570 6572 7669 7365 6420 6279 204c 6172  upervised by Lar
+00000a10: 7320 4b61 6920 4861 6e73 656e 2066 726f  s Kai Hansen fro
+00000a20: 6d20 4454 5520 436f 6d70 7574 6520 616e  m DTU Compute an
+00000a30: 6420 4d61 7274 696e 2043 6172 7374 656e  d Martin Carsten
+00000a40: 204e 6965 6c73 656e 2066 726f 6d20 416c   Nielsen from Al
+00000a50: 7665 6e69 722e 0a0a 2323 2049 6e73 7461  venir...## Insta
+00000a60: 6c6c 6174 696f 6e0a 0a54 6865 2070 6163  llation..The pac
+00000a70: 6b61 6765 2068 6173 2062 6565 6e20 6465  kage has been de
+00000a80: 7665 6c6f 7065 6420 616e 6420 7573 6564  veloped and used
+00000a90: 2077 6974 6820 5079 7468 6f6e 2033 2e31   with Python 3.1
+00000aa0: 312e 0a54 6f20 696e 7374 616c 6c20 7468  1..To install th
+00000ab0: 6520 7061 636b 6167 6520 696e 2061 2062  e package in a b
+00000ac0: 6173 6520 7665 7273 696f 6e2c 2065 6e61  ase version, ena
+00000ad0: 626c 696e 6720 6d6f 6465 6c20 6578 6563  bling model exec
+00000ae0: 7574 696f 6e2c 2069 6e73 7461 6c6c 0a60  ution, install.`
+00000af0: 6060 0a70 6970 2069 6e73 7461 6c6c 2064  ``.pip install d
+00000b00: 616e 6f6c 6974 6572 6174 650a 6060 600a  anoliterate.```.
+00000b10: 2a4e 6f74 653a 2a20 536f 6d65 2066 6561  *Note:* Some fea
+00000b20: 7475 7265 7320 6e65 6564 2061 2066 756c  tures need a ful
+00000b30: 6c20 696e 7374 616c 6c20 746f 2072 756e  l install to run
+00000b40: 3a0a 6060 600a 7069 7020 696e 7374 616c  :.```.pip instal
+00000b50: 6c20 6461 6e6f 6c69 7465 7261 7465 5b66  l danoliterate[f
+00000b60: 756c 6c5d 0a60 6060 0a0a 2323 2055 7361  ull].```..## Usa
+00000b70: 6765 0a0a 5365 6520 6f70 7469 6f6e 7320  ge..See options 
+00000b80: 7769 7468 0a60 6060 6261 7368 0a70 7974  with.```bash.pyt
+00000b90: 686f 6e20 2d6d 2064 616e 6f6c 6974 6572  hon -m danoliter
+00000ba0: 6174 6520 646f 3d65 7661 6c75 6174 650a  ate do=evaluate.
+00000bb0: 6060 600a 0a41 2074 7970 6963 616c 2075  ```..A typical u
+00000bc0: 7365 2077 6f75 6c64 2062 6520 746f 2072  se would be to r
+00000bd0: 756e 2079 6f75 7220 6f77 6e20 6d6f 6465  un your own mode
+00000be0: 6c20 686f 7374 6564 206f 6e20 7468 6520  l hosted on the 
+00000bf0: 4875 6767 696e 6766 6163 6520 4875 6220  Huggingface Hub 
+00000c00: 6f6e 2061 2073 6365 6e61 7269 6f2c 2066  on a scenario, f
+00000c10: 6f72 2065 7861 6d70 6c65 2074 6865 2043  or example the C
+00000c20: 6974 697a 656e 7368 6970 2054 6573 7420  itizenship Test 
+00000c30: 5363 656e 6172 696f 2028 7365 6520 5b74  Scenario (see [t
+00000c40: 6865 2066 726f 6e74 656e 645d 2868 7474  he frontend](htt
+00000c50: 7073 3a2f 2f64 616e 6f6c 6974 6572 6174  ps://danoliterat
+00000c60: 652e 636f 6d70 7574 652e 6474 752e 646b  e.compute.dtu.dk
+00000c70: 2f53 6365 6e61 7269 6f73 2920 666f 7220  /Scenarios) for 
+00000c80: 7363 656e 6172 696f 2064 6573 6372 6970  scenario descrip
+00000c90: 7469 6f6e 7329 2e0a 536b 6970 2074 6865  tions)..Skip the
+00000ca0: 206c 696e 6520 6073 6365 6e61 7269 6f73   line `scenarios
+00000cb0: 3d60 2074 6f20 6d61 6b65 2069 7420 7275  =` to make it ru
+00000cc0: 6e20 6f6e 2061 6c6c 2073 6365 6e61 7269  n on all scenari
+00000cd0: 6f73 2069 6e73 7465 6164 2e0a 6060 6062  os instead..```b
+00000ce0: 6173 680a 7079 7468 6f6e 202d 6d20 6461  ash.python -m da
+00000cf0: 6e6f 6c69 7465 7261 7465 2064 6f3d 6576  noliterate do=ev
+00000d00: 616c 7561 7465 5c0a 2020 2020 7363 656e  aluate\.    scen
+00000d10: 6172 696f 733d 2263 6974 697a 656e 7368  arios="citizensh
+00000d20: 6970 2d74 6573 7422 5c0a 2020 2020 6d6f  ip-test"\.    mo
+00000d30: 6465 6c2e 6e61 6d65 3d22 4d79 4c69 7474  del.name="MyLitt
+00000d40: 6c65 4750 5422 5c0a 2020 2020 6d6f 6465  leGPT"\.    mode
+00000d50: 6c2e 7061 7468 3d22 6866 2d69 6e74 6572  l.path="hf-inter
+00000d60: 6e61 6c2d 7465 7374 696e 672f 7469 6e79  nal-testing/tiny
+00000d70: 2d72 616e 646f 6d2d 6770 7432 225c 0a20  -random-gpt2"\. 
+00000d80: 2020 2065 7661 6c75 6174 696f 6e2e 6c6f     evaluation.lo
+00000d90: 6361 6c5f 7265 7375 6c74 733d 222e 2f6d  cal_results="./m
+00000da0: 792d 7265 7375 6c74 2d64 6222 0a60 6060  y-result-db".```
+00000db0: 0a0a 4e6f 772c 2079 6f75 2063 6f75 6c64  ..Now, you could
+00000dc0: 2073 6861 7265 2074 6865 2072 6573 756c   share the resul
+00000dd0: 7469 6e67 204a 534f 4e20 706c 6163 6564  ting JSON placed
+00000de0: 2069 6e20 606d 792d 7265 7375 6c74 2d64   in `my-result-d
+00000df0: 6260 2074 6f20 6765 7420 6974 2069 6e63  b` to get it inc
+00000e00: 6c75 6465 6420 696e 2074 6865 2044 616e  luded in the Dan
+00000e10: 6f6c 6974 6572 6174 6520 6265 6e63 686d  oliterate benchm
+00000e20: 6172 6b2c 206f 7220 796f 7520 6361 6e20  ark, or you can 
+00000e30: 7361 7469 7366 7920 796f 7572 2063 7572  satisfy your cur
+00000e40: 696f 7369 7479 2061 6e64 2073 636f 7265  iosity and score
+00000e50: 2069 7420 796f 7572 7365 6c66 0a60 6060   it yourself.```
+00000e60: 6261 7368 0a23 2043 616c 6375 6c61 7465  bash.# Calculate
+00000e70: 7320 7363 6f72 696e 6720 6d65 7472 6963  s scoring metric
+00000e80: 730a 7079 7468 6f6e 202d 6d20 6461 6e6f  s.python -m dano
+00000e90: 6c69 7465 7261 7465 2064 6f3d 7363 6f72  literate do=scor
+00000ea0: 655c 0a20 2020 2065 7661 6c75 6174 696f  e\.    evaluatio
+00000eb0: 6e2e 6c6f 6361 6c5f 7265 7375 6c74 733d  n.local_results=
+00000ec0: 222e 2f6d 792d 7265 7375 6c74 2d64 6222  "./my-result-db"
+00000ed0: 0a23 2050 7269 6e74 7320 7468 656d 2066  .# Prints them f
+00000ee0: 6f72 2079 6f75 0a70 7974 686f 6e20 2d6d  or you.python -m
+00000ef0: 2064 616e 6f6c 6974 6572 6174 6520 646f   danoliterate do
+00000f00: 3d72 6570 6f72 745c 0a20 2020 2065 7661  =report\.    eva
+00000f10: 6c75 6174 696f 6e2e 6c6f 6361 6c5f 7265  luation.local_re
+00000f20: 7375 6c74 733d 222e 2f6d 792d 7265 7375  sults="./my-resu
+00000f30: 6c74 2d64 6222 0a60 6060 0a0a 2323 2043  lt-db".```..## C
+00000f40: 6f6e 7461 6374 0a50 6c65 6173 6520 7265  ontact.Please re
+00000f50: 6163 6820 6865 7265 2075 7369 6e67 2047  ach here using G
+00000f60: 6974 4875 6220 6973 7375 6573 206f 7220  itHub issues or 
+00000f70: 6f6e 206d 6169 6c20 746f 2053 c3b8 7265  on mail to S..re
+00000f80: 6e20 5665 6a6c 6761 6172 6420 486f 6c6d  n Vejlgaard Holm
+00000f90: 2065 6974 6865 7220 6174 205b 7377 6968   either at [swih
+00000fa0: 6f40 6474 752e 646b 5d28 6d61 696c 746f  o@dtu.dk](mailto
+00000fb0: 3a73 7769 686f 4064 7475 2e64 6b29 206f  :swiho@dtu.dk) o
+00000fc0: 7220 5b73 7768 4061 6c76 656e 6972 2e61  r [swh@alvenir.a
+00000fd0: 695d 286d 6169 6c74 6f3a 7377 6840 616c  i](mailto:swh@al
+00000fe0: 7665 6e69 722e 6169 292e 0a              venir.ai)..
```

### Comparing `danoliterate-0.0.3/danoliterate.egg-info/SOURCES.txt` & `danoliterate-0.0.4/danoliterate.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,27 +17,36 @@
 danoliterate/configs/databuild/da_cloze_self_test.yaml
 danoliterate/configs/databuild/da_gym_2000.yaml
 danoliterate/configs/databuild/hashtag_twitterhjerne.yaml
 danoliterate/configs/databuild/hyggeswag.yaml
 danoliterate/configs/databuild/nordjylland_news.yaml
 danoliterate/configs/databuild/prompt_answer.yaml
 danoliterate/configs/model/baseline.yaml
+danoliterate/configs/model/claude-haiku.yaml
+danoliterate/configs/model/claude-opus.yaml
+danoliterate/configs/model/claude-sonnet.yaml
 danoliterate/configs/model/danoliterate-baseline.yaml
 danoliterate/configs/model/danoliterate-llama.yaml
 danoliterate/configs/model/danoliterate-mistral.yaml
 danoliterate/configs/model/danskgpt-api.yaml
+danoliterate/configs/model/danskgpt-tiny-chat.yaml
 danoliterate/configs/model/danskgpt-tiny.yaml
 danoliterate/configs/model/danskgpt.yaml
+danoliterate/configs/model/gemma-7b-it.yaml
+danoliterate/configs/model/gemma-7b.yaml
 danoliterate/configs/model/google-gemini-pro.yaml
+danoliterate/configs/model/gpt-7b-nordic-prerelease.yaml
 danoliterate/configs/model/gpt-neo-da.yaml
 danoliterate/configs/model/gpt-neox-da.yaml
 danoliterate/configs/model/gpt-sw3-20b-instruct.yaml
 danoliterate/configs/model/gpt-sw3-20b.yaml
 danoliterate/configs/model/gpt-sw3-6b-instruct.yaml
 danoliterate/configs/model/gpt-sw3-6b.yaml
+danoliterate/configs/model/heidrun-mistral-7b-base.yaml
+danoliterate/configs/model/heidrun-mistral-7b-chat.yaml
 danoliterate/configs/model/hestenet-lm.yaml
 danoliterate/configs/model/kanelsnegl.yaml
 danoliterate/configs/model/llama2-13b-chat.yaml
 danoliterate/configs/model/llama2-13b.yaml
 danoliterate/configs/model/llama2-70b-chat.yaml
 danoliterate/configs/model/llama2-70b.yaml
 danoliterate/configs/model/llama2-7b-chat.yaml
@@ -45,28 +54,38 @@
 danoliterate/configs/model/mgpt-13b.yaml
 danoliterate/configs/model/mgpt.yaml
 danoliterate/configs/model/mistral-7b-instruct-v0.2.yaml
 danoliterate/configs/model/mistral-7b-instruct.yaml
 danoliterate/configs/model/mistral-7b.yaml
 danoliterate/configs/model/mixtral-8-7b-instruct.yaml
 danoliterate/configs/model/mixtral-8-7b.yaml
+danoliterate/configs/model/mixtral-groq.yaml
+danoliterate/configs/model/munin-7b-alpha.yaml
+danoliterate/configs/model/munin-mistral-7b.yaml
+danoliterate/configs/model/munin-neuralbeagle-7b.yaml
 danoliterate/configs/model/nb-gpt-j-norpaca.yaml
 danoliterate/configs/model/nb-gpt-j.yaml
-danoliterate/configs/model/new.yaml
+danoliterate/configs/model/new-hf.yaml
+danoliterate/configs/model/olmo-7b-instruct.yaml
 danoliterate/configs/model/openai-ada-001.yaml
 danoliterate/configs/model/openai-babbage-002.yaml
 danoliterate/configs/model/openai-davinci-002.yaml
 danoliterate/configs/model/openai-davinci-003.yaml
 danoliterate/configs/model/openai-gpt-3.5-turbo-instruct.yaml
 danoliterate/configs/model/openai-gpt-4-turbo.yaml
 danoliterate/configs/model/openai-gpt-4.yaml
 danoliterate/configs/model/openai-gpt-turbo.yaml
+danoliterate/configs/model/phi-2.yaml
+danoliterate/configs/model/qwen1.5-7b-chat.yaml
 danoliterate/configs/model/solar-11b-instruct.yaml
 danoliterate/configs/model/solar-11b.yaml
 danoliterate/configs/model/test.yaml
+danoliterate/configs/model/viking-13b.yaml
+danoliterate/configs/model/viking-33b.yaml
+danoliterate/configs/model/viking-7b.yaml
 danoliterate/configs/scenarios/angry-tweets.yaml
 danoliterate/configs/scenarios/citizenship-test-free.yaml
 danoliterate/configs/scenarios/citizenship-test-simple.yaml
 danoliterate/configs/scenarios/citizenship-test.yaml
 danoliterate/configs/scenarios/da-cloze-self-test-free.yaml
 danoliterate/configs/scenarios/da-cloze-self-test.yaml
 danoliterate/configs/scenarios/da-gym-2000-english.yaml
@@ -92,49 +111,40 @@
 danoliterate/data/building/da_gym_2000.py
 danoliterate/data/building/hashtag_twitterhjerne.py
 danoliterate/data/building/hub.py
 danoliterate/data/building/hyggeswag.py
 danoliterate/data/building/nordjylland_news.py
 danoliterate/data/building/prompt_answer_da.py
 danoliterate/evaluation/__init__.py
-danoliterate/evaluation/artifact_integration.py
 danoliterate/evaluation/results.py
 danoliterate/evaluation/serialization.py
 danoliterate/evaluation/analysis/__init__.py
-danoliterate/evaluation/analysis/analyser.py
-danoliterate/evaluation/analysis/analysis_notebook.py
 danoliterate/evaluation/analysis/dimensions.py
-danoliterate/evaluation/analysis/inspection.py
 danoliterate/evaluation/analysis/meta_scorings.py
 danoliterate/evaluation/analysis/metrics.py
 danoliterate/evaluation/analysis/scorer.py
+danoliterate/evaluation/analysis/scores_report.py
 danoliterate/evaluation/execution/__init__.py
 danoliterate/evaluation/execution/api_inference.py
 danoliterate/evaluation/execution/augmentation.py
 danoliterate/evaluation/execution/eval_types.py
 danoliterate/evaluation/execution/evaluator.py
 danoliterate/evaluation/execution/huggingface_inference.py
 danoliterate/evaluation/execution/model_inference.py
 danoliterate/evaluation/execution/task_runner.py
-danoliterate/evaluation/leaderboard/__init__.py
-danoliterate/evaluation/leaderboard/metric_parsing.py
-danoliterate/evaluation/leaderboard/table.py
-danoliterate/evaluation/leaderboard/🇩🇰_Hello.py
 danoliterate/evaluation/registries/__init__.py
-danoliterate/evaluation/registries/get.py
 danoliterate/evaluation/registries/inferences.py
 danoliterate/evaluation/registries/metrics.py
 danoliterate/evaluation/registries/tasks.py
 danoliterate/infrastructure/__init__.py
 danoliterate/infrastructure/constants.py
 danoliterate/infrastructure/logging.py
 danoliterate/infrastructure/runs.py
 danoliterate/infrastructure/timing.py
 danoliterate/infrastructure/management/__init__.py
-danoliterate/infrastructure/management/artifacto.py
 danoliterate/modeling/__init__.py
 danoliterate/modeling/gpt_ner_alignment.py
 danoliterate/modeling/language_identification.py
 danoliterate/modeling/load_model.py
 danoliterate/modeling/ngram_language_modeling.py
 danoliterate/modeling/text_classification.py
 danoliterate/modeling/text_comparison.py
@@ -246,13 +256,101 @@
 job-outputs/job-20240107-124826/.hydra/overrides.yaml
 job-outputs/job-20240115-204316/.hydra/config.yaml
 job-outputs/job-20240115-204316/.hydra/hydra.yaml
 job-outputs/job-20240115-204316/.hydra/overrides.yaml
 job-outputs/job-20240115-204343/.hydra/config.yaml
 job-outputs/job-20240115-204343/.hydra/hydra.yaml
 job-outputs/job-20240115-204343/.hydra/overrides.yaml
+job-outputs/job-20240305-094247/.hydra/config.yaml
+job-outputs/job-20240305-094247/.hydra/hydra.yaml
+job-outputs/job-20240305-094247/.hydra/overrides.yaml
+job-outputs/job-20240305-105817/.hydra/config.yaml
+job-outputs/job-20240305-105817/.hydra/hydra.yaml
+job-outputs/job-20240305-105817/.hydra/overrides.yaml
+job-outputs/job-20240305-134743/.hydra/config.yaml
+job-outputs/job-20240305-134743/.hydra/hydra.yaml
+job-outputs/job-20240305-134743/.hydra/overrides.yaml
+job-outputs/job-20240305-134823/.hydra/config.yaml
+job-outputs/job-20240305-134823/.hydra/hydra.yaml
+job-outputs/job-20240305-134823/.hydra/overrides.yaml
+job-outputs/job-20240305-135336/.hydra/config.yaml
+job-outputs/job-20240305-135336/.hydra/hydra.yaml
+job-outputs/job-20240305-135336/.hydra/overrides.yaml
+job-outputs/job-20240305-135854/.hydra/config.yaml
+job-outputs/job-20240305-135854/.hydra/hydra.yaml
+job-outputs/job-20240305-135854/.hydra/overrides.yaml
+job-outputs/job-20240305-135908/.hydra/config.yaml
+job-outputs/job-20240305-135908/.hydra/hydra.yaml
+job-outputs/job-20240305-135908/.hydra/overrides.yaml
+job-outputs/job-20240305-135950/.hydra/config.yaml
+job-outputs/job-20240305-135950/.hydra/hydra.yaml
+job-outputs/job-20240305-135950/.hydra/overrides.yaml
+job-outputs/job-20240404-145007/.hydra/config.yaml
+job-outputs/job-20240404-145007/.hydra/hydra.yaml
+job-outputs/job-20240404-145007/.hydra/overrides.yaml
+job-outputs/job-20240404-145426/.hydra/config.yaml
+job-outputs/job-20240404-145426/.hydra/hydra.yaml
+job-outputs/job-20240404-145426/.hydra/overrides.yaml
+job-outputs/job-20240404-150131/.hydra/config.yaml
+job-outputs/job-20240404-150131/.hydra/hydra.yaml
+job-outputs/job-20240404-150131/.hydra/overrides.yaml
+job-outputs/job-20240404-150158/.hydra/config.yaml
+job-outputs/job-20240404-150158/.hydra/hydra.yaml
+job-outputs/job-20240404-150158/.hydra/overrides.yaml
+job-outputs/job-20240404-213153/.hydra/config.yaml
+job-outputs/job-20240404-213153/.hydra/hydra.yaml
+job-outputs/job-20240404-213153/.hydra/overrides.yaml
+job-outputs/job-20240404-215256/.hydra/config.yaml
+job-outputs/job-20240404-215256/.hydra/hydra.yaml
+job-outputs/job-20240404-215256/.hydra/overrides.yaml
+job-outputs/job-20240404-215335/.hydra/config.yaml
+job-outputs/job-20240404-215335/.hydra/hydra.yaml
+job-outputs/job-20240404-215335/.hydra/overrides.yaml
+job-outputs/job-20240404-215350/.hydra/config.yaml
+job-outputs/job-20240404-215350/.hydra/hydra.yaml
+job-outputs/job-20240404-215350/.hydra/overrides.yaml
+job-outputs/job-20240404-215353/.hydra/config.yaml
+job-outputs/job-20240404-215353/.hydra/hydra.yaml
+job-outputs/job-20240404-215353/.hydra/overrides.yaml
+job-outputs/job-20240404-215511/.hydra/config.yaml
+job-outputs/job-20240404-215511/.hydra/hydra.yaml
+job-outputs/job-20240404-215511/.hydra/overrides.yaml
+job-outputs/job-20240404-215525/.hydra/config.yaml
+job-outputs/job-20240404-215525/.hydra/hydra.yaml
+job-outputs/job-20240404-215525/.hydra/overrides.yaml
+job-outputs/job-20240404-215609/.hydra/config.yaml
+job-outputs/job-20240404-215609/.hydra/hydra.yaml
+job-outputs/job-20240404-215609/.hydra/overrides.yaml
+job-outputs/job-20240404-220513/.hydra/config.yaml
+job-outputs/job-20240404-220513/.hydra/hydra.yaml
+job-outputs/job-20240404-220513/.hydra/overrides.yaml
+job-outputs/job-20240404-220659/.hydra/config.yaml
+job-outputs/job-20240404-220659/.hydra/hydra.yaml
+job-outputs/job-20240404-220659/.hydra/overrides.yaml
+job-outputs/job-20240404-221031/.hydra/config.yaml
+job-outputs/job-20240404-221031/.hydra/hydra.yaml
+job-outputs/job-20240404-221031/.hydra/overrides.yaml
+job-outputs/job-20240404-221111/.hydra/config.yaml
+job-outputs/job-20240404-221111/.hydra/hydra.yaml
+job-outputs/job-20240404-221111/.hydra/overrides.yaml
+job-outputs/job-20240404-221511/.hydra/config.yaml
+job-outputs/job-20240404-221511/.hydra/hydra.yaml
+job-outputs/job-20240404-221511/.hydra/overrides.yaml
+job-outputs/job-20240404-221624/.hydra/config.yaml
+job-outputs/job-20240404-221624/.hydra/hydra.yaml
+job-outputs/job-20240404-221624/.hydra/overrides.yaml
+job-outputs/job-20240404-221627/.hydra/config.yaml
+job-outputs/job-20240404-221627/.hydra/hydra.yaml
+job-outputs/job-20240404-221627/.hydra/overrides.yaml
 tests/test_from_pretrained_no_disk.py
 tests/test_likelihood_computation.py
-wandb/latest-run/files/config.yaml
 wandb/run-20240102_144118-yu960l4r/files/config.yaml
 wandb/run-20240102_144223-8dnifqy5/files/config.yaml
-wandb/run-20240102_144307-cc949b1q/files/config.yaml
+wandb/run-20240102_144307-cc949b1q/files/config.yaml
+wandb/run-20240103_185207-2gwbcbde/files/config.yaml
+wandb/run-20240305_094252-df29fahs/files/config.yaml
+wandb/run-20240305_105822-c8kqo92t/files/config.yaml
+wandb/run-20240305_134750-oo297j8y/files/config.yaml
+wandb/run-20240305_134828-x0uracs9/files/config.yaml
+wandb/run-20240305_135341-5hv9bvag/files/config.yaml
+wandb/run-20240305_135914-1eueet3m/files/config.yaml
+wandb/run-20240305_135956-qujwpo8u/files/config.yaml
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-075208/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-075208/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-075208/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-075208/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-080050/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-080050/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-080050/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-080050/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-133515/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-133515/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-133515/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-133515/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-193039/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-193039/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-193039/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-193039/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-232500/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-232500/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240102-232500/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240102-232500/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-084437/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-084437/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-084437/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-084437/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-164458/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-164458/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-164458/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-164458/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-164511/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-164511/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-164511/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-164511/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-164531/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-164531/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-164531/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-164531/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-185156/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-185156/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-185156/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-185156/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-185500/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-185500/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-185500/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-185500/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-185540/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-185540/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-185540/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-185540/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-185737/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-185737/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-185737/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-185737/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-190426/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-190426/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-190426/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-190426/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-204714/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-204714/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-204714/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-204714/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-204731/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-204731/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-204731/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-204731/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-204744/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-204744/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240103-204744/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240103-204744/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240104-071348/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240104-071348/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240104-071348/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240104-071348/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240104-142624/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240104-142624/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240104-142624/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240104-142624/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-093656/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-093656/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-093656/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-093656/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220155/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220155/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220155/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220155/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220249/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220249/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220249/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220249/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220441/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220441/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220441/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220441/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220632/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220632/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220632/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220632/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220737/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220737/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220737/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220737/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220842/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220842/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220842/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220842/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220951/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220951/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-220951/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-220951/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221029/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221029/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221029/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221029/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221253/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221253/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221253/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221253/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221330/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221330/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221330/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221330/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221504/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221504/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221504/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221504/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221552/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221552/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221552/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221552/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221615/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221615/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240106-221615/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240106-221615/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240107-124826/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240107-124826/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240107-124826/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240107-124826/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240115-204316/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240115-204316/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240115-204316/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240115-204316/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240115-204343/.hydra/config.yaml` & `danoliterate-0.0.4/job-outputs/job-20240115-204343/.hydra/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/job-outputs/job-20240115-204343/.hydra/hydra.yaml` & `danoliterate-0.0.4/job-outputs/job-20240115-204343/.hydra/hydra.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/pyproject.toml` & `danoliterate-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/setup.py` & `danoliterate-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             line.strip()
             for line in f.read().splitlines()
             if line.strip() and not line.strip().startswith("#")
         ]
 
 setup_args = dict(
     name="danoliterate",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     author="Søren Winkel Holm",
     author_email="swholm@protonmail.com",
     install_requires=requires["base"],
     extras_require={
         "full": requires["full"],
     },
```

### Comparing `danoliterate-0.0.3/tests/test_from_pretrained_no_disk.py` & `danoliterate-0.0.4/tests/test_from_pretrained_no_disk.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/tests/test_likelihood_computation.py` & `danoliterate-0.0.4/tests/test_likelihood_computation.py`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/wandb/latest-run/files/config.yaml` & `danoliterate-0.0.4/wandb/run-20240103_185207-2gwbcbde/files/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/wandb/run-20240102_144118-yu960l4r/files/config.yaml` & `danoliterate-0.0.4/wandb/run-20240102_144118-yu960l4r/files/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/wandb/run-20240102_144223-8dnifqy5/files/config.yaml` & `danoliterate-0.0.4/wandb/run-20240102_144223-8dnifqy5/files/config.yaml`

 * *Files identical despite different names*

### Comparing `danoliterate-0.0.3/wandb/run-20240102_144307-cc949b1q/files/config.yaml` & `danoliterate-0.0.4/wandb/run-20240102_144307-cc949b1q/files/config.yaml`

 * *Files identical despite different names*

