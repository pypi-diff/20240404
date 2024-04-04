# Comparing `tmp/qianfan-0.3.7.tar.gz` & `tmp/qianfan-0.3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianfan-0.3.7.tar", max compression
+gzip compressed data, was "qianfan-0.3.7.1.tar", max compression
```

## Comparing `qianfan-0.3.7.tar` & `qianfan-0.3.7.1.tar`

### file list

```diff
@@ -1,160 +1,160 @@
--rw-r--r--   0        0        0     6443 2024-03-29 18:51:59.055189 qianfan-0.3.7/README.pypi.md
--rw-r--r--   0        0        0     3414 2024-03-29 18:51:59.055189 qianfan-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1578 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/__init__.py
--rw-r--r--   0        0        0      659 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/__init__.py
--rw-r--r--   0        0        0     2451 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/context.py
--rw-r--r--   0        0        0     4502 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/launcher.py
--rw-r--r--   0        0        0      847 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/runner/__init__.py
--rw-r--r--   0        0        0     1688 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/runner/base.py
--rw-r--r--   0        0        0     6028 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/runner/infer_runner.py
--rw-r--r--   0        0        0     6568 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/runner/qianfan_runner.py
--rw-r--r--   0        0        0     1460 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/space.py
--rw-r--r--   0        0        0      784 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/suggestor/__init__.py
--rw-r--r--   0        0        0     3370 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/suggestor/base.py
--rw-r--r--   0        0        0     3356 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/suggestor/random_suggestor.py
--rw-r--r--   0        0        0     3973 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/tune.py
--rw-r--r--   0        0        0     1357 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/autotuner/utils.py
--rw-r--r--   0        0        0      699 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/__init__.py
--rw-r--r--   0        0        0    15290 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/chat.py
--rw-r--r--   0        0        0     7120 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/completion.py
--rw-r--r--   0        0        0    14564 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/dataset.py
--rw-r--r--   0        0        0      790 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/embedding.py
--rw-r--r--   0        0        0     9595 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/evaluation.py
--rw-r--r--   0        0        0     6437 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/main.py
--rw-r--r--   0        0        0     4107 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/openai_adapter.py
--rw-r--r--   0        0        0    17018 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/plugin.py
--rw-r--r--   0        0        0    23840 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/trainer.py
--rw-r--r--   0        0        0     3265 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/txt2img.py
--rw-r--r--   0        0        0     9991 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/client/utils.py
--rw-r--r--   0        0        0        1 2024-03-29 18:51:59.055189 qianfan-0.3.7/qianfan/common/hub/__init__.py
--rw-r--r--   0        0        0     5823 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/hub/hub.py
--rw-r--r--   0        0        0     3512 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/hub/interface.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/persister/__init__.py
--rw-r--r--   0        0        0      963 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/persister/base.py
--rw-r--r--   0        0        0     2965 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/persister/persist.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/prompt/__init__.py
--rw-r--r--   0        0        0    23850 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/runnable/__init__.py
--rw-r--r--   0        0        0     6386 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/runnable/base.py
--rw-r--r--   0        0        0     3698 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/tool/baidu_search_tool.py
--rw-r--r--   0        0        0     7561 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/tool/base_tool.py
--rw-r--r--   0        0        0     2962 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/tool/duckduckgo_search_tool.py
--rw-r--r--   0        0        0     3312 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/common/tool/wikipedia_tool.py
--rw-r--r--   0        0        0     9582 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/config.py
--rw-r--r--   0        0        0    12267 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/consts.py
--rw-r--r--   0        0        0     1367 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/__init__.py
--rw-r--r--   0        0        0     2786 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/consts.py
--rw-r--r--   0        0        0     4363 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/data_operator.py
--rw-r--r--   0        0        0     1013 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/data_source/__init__.py
--rw-r--r--   0        0        0    27521 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/data_source/baidu_qianfan.py
--rw-r--r--   0        0        0     2701 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/data_source/base.py
--rw-r--r--   0        0        0    13584 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/data_source/bos.py
--rw-r--r--   0        0        0     9424 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/data_source/chunk_reader.py
--rw-r--r--   0        0        0     9532 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/data_source/file.py
--rw-r--r--   0        0        0    23618 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/data_source/utils.py
--rw-r--r--   0        0        0    58873 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/dataset.py
--rw-r--r--   0        0        0    14197 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/dataset_utils.py
--rw-r--r--   0        0        0     1139 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/__init__.py
--rw-r--r--   0        0        0     2237 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/base.py
--rw-r--r--   0        0        0     3942 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/check_character_repetition_filter.py
--rw-r--r--   0        0        0     4482 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/check_flagged_words.py
--rw-r--r--   0        0        0     2443 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/check_sentence_length_filter.py
--rw-r--r--   0        0        0     2504 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/check_special_characters.py
--rw-r--r--   0        0        0     4313 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/check_stopwords.py
--rw-r--r--   0        0        0     3085 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/check_word_number.py
--rw-r--r--   0        0        0     3910 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/check_word_repetition_filter.py
--rw-r--r--   0        0        0     4483 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/consts.py
--rw-r--r--   0        0        0     4693 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/utils.py
--rw-r--r--   0        0        0   136258 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/local_data_operators/word_list.py
--rw-r--r--   0        0        0     2832 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/process_interface.py
--rw-r--r--   0        0        0     4363 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/qianfan_data_operators.py
--rw-r--r--   0        0        0    10622 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/schema.py
--rw-r--r--   0        0        0    40452 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/table.py
--rw-r--r--   0        0        0     1302 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/dataset/table_utils.py
--rw-r--r--   0        0        0     2254 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/errors.py
--rw-r--r--   0        0        0      878 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/evaluation/__init__.py
--rw-r--r--   0        0        0     2748 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/evaluation/consts.py
--rw-r--r--   0        0        0    24029 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/evaluation/evaluation_manager.py
--rw-r--r--   0        0        0     1325 2024-03-29 18:51:59.059189 qianfan-0.3.7/qianfan/evaluation/evaluation_result.py
--rw-r--r--   0        0        0     3927 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/evaluation/evaluator.py
--rw-r--r--   0        0        0     4379 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/evaluation/local_evaluator.py
--rw-r--r--   0        0        0     2468 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/evaluation/opencompass_evaluator.py
--rw-r--r--   0        0        0       66 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/README.md
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/__init__.py
--rw-r--r--   0        0        0      200 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/langchain/__init__.py
--rw-r--r--   0        0        0      212 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/langchain/agents/__init__.py
--rw-r--r--   0        0        0    13025 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/openai/__init__.py
--rw-r--r--   0        0        0    18554 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/openai/adapter.py
--rw-r--r--   0        0        0     1602 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/semantic_kernel/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0     7804 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py
--rw-r--r--   0        0        0     1627 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py
--rw-r--r--   0        0        0     5365 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py
--rw-r--r--   0        0        0     4056 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py
--rw-r--r--   0        0        0     2577 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/fake_pyarrow_replacer.py
--rw-r--r--   0        0        0      742 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/model/__init__.py
--rw-r--r--   0        0        0      923 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/model/configs.py
--rw-r--r--   0        0        0      938 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/model/consts.py
--rw-r--r--   0        0        0    22871 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/model/model.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/py.typed
--rw-r--r--   0        0        0     1648 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/auth/__init__.py
--rw-r--r--   0        0        0     1656 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/auth/iam.py
--rw-r--r--   0        0        0    14286 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/auth/oauth.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/__init__.py
--rw-r--r--   0        0        0     4183 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/charge.py
--rw-r--r--   0        0        0     7503 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/consts.py
--rw-r--r--   0        0        0    30894 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/data.py
--rw-r--r--   0        0        0    16279 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/finetune.py
--rw-r--r--   0        0        0    23076 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/model.py
--rw-r--r--   0        0        0    19491 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/prompt.py
--rw-r--r--   0        0        0     5607 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/service.py
--rw-r--r--   0        0        0     4941 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/console/utils.py
--rw-r--r--   0        0        0     3779 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/http_client.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/images/__init__.py
--rw-r--r--   0        0        0    11411 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/images/image2text.py
--rw-r--r--   0        0        0    11777 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/images/text2image.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/llm/__init__.py
--rw-r--r--   0        0        0    27287 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/llm/base.py
--rw-r--r--   0        0        0    42166 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/llm/chat_completion.py
--rw-r--r--   0        0        0    11545 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/llm/completion.py
--rw-r--r--   0        0        0    10678 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/llm/embedding.py
--rw-r--r--   0        0        0    13139 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/llm/plugin.py
--rw-r--r--   0        0        0    14096 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/requestor/__init__.py
--rw-r--r--   0        0        0    12834 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/requestor/base.py
--rw-r--r--   0        0        0     3189 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/requestor/console_requestor.py
--rw-r--r--   0        0        0    21478 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/requestor/openapi_requestor.py
--rw-r--r--   0        0        0     9899 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/token_limiter.py
--rw-r--r--   0        0        0        0 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/tools/__init__.py
--rw-r--r--   0        0        0     4909 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/tools/tokenizer.py
--rw-r--r--   0        0        0     3580 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/tools/utils.py
--rw-r--r--   0        0        0     9199 2024-03-29 18:51:59.063189 qianfan-0.3.7/qianfan/resources/typing.py
--rw-r--r--   0        0        0     1141 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/__init__.py
--rw-r--r--   0        0        0    44551 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/actions.py
--rw-r--r--   0        0        0     6000 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/base.py
--rw-r--r--   0        0        0    38156 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/configs.py
--rw-r--r--   0        0        0     3600 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/consts.py
--rw-r--r--   0        0        0     3403 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/event.py
--rw-r--r--   0        0        0    11390 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/finetune.py
--rw-r--r--   0        0        0     9561 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/pipeline.py
--rw-r--r--   0        0        0     7772 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/post_pretrain.py
--rw-r--r--   0        0        0     1680 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/ppl.yaml
--rw-r--r--   0        0        0     4709 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/trainer/trainer.py
--rw-r--r--   0        0        0     1244 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/__init__.py
--rw-r--r--   0        0        0     4647 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/bos_uploader.py
--rw-r--r--   0        0        0      696 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/cache/__init__.py
--rw-r--r--   0        0        0      787 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/cache/base.py
--rw-r--r--   0        0        0      827 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/fake_pyarrow/__init__.py
--rw-r--r--   0        0        0      730 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/fake_pyarrow/compute.py
--rw-r--r--   0        0        0      812 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/fake_pyarrow/functions.py
--rw-r--r--   0        0        0      869 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/fake_pyarrow/ipc.py
--rw-r--r--   0        0        0      984 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/fake_pyarrow/table.py
--rw-r--r--   0        0        0     1084 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/helper.py
--rw-r--r--   0        0        0     5670 2024-03-29 18:51:59.067189 qianfan-0.3.7/qianfan/utils/logging.py
--rw-r--r--   0        0        0      734 2024-03-29 18:51:59.071189 qianfan-0.3.7/qianfan/utils/pydantic/__init__.py
--rw-r--r--   0        0        0     7230 2024-03-29 18:51:59.071189 qianfan-0.3.7/qianfan/utils/utils.py
--rw-r--r--   0        0        0      900 2024-03-29 18:51:59.071189 qianfan-0.3.7/qianfan/version.py
--rw-r--r--   0        0        0    10340 1970-01-01 00:00:00.000000 qianfan-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     6443 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/README.pypi.md
+-rw-r--r--   0        0        0     3668 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1578 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/__init__.py
+-rw-r--r--   0        0        0     2451 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/context.py
+-rw-r--r--   0        0        0     4502 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/launcher.py
+-rw-r--r--   0        0        0      847 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/runner/__init__.py
+-rw-r--r--   0        0        0     1688 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/runner/base.py
+-rw-r--r--   0        0        0     6028 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/runner/infer_runner.py
+-rw-r--r--   0        0        0     6571 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/runner/qianfan_runner.py
+-rw-r--r--   0        0        0     1460 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/space.py
+-rw-r--r--   0        0        0      784 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/suggestor/__init__.py
+-rw-r--r--   0        0        0     3370 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/suggestor/base.py
+-rw-r--r--   0        0        0     3356 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/suggestor/random_suggestor.py
+-rw-r--r--   0        0        0     3973 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/tune.py
+-rw-r--r--   0        0        0     1357 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/utils.py
+-rw-r--r--   0        0        0      699 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/__init__.py
+-rw-r--r--   0        0        0    15290 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/chat.py
+-rw-r--r--   0        0        0     7120 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/completion.py
+-rw-r--r--   0        0        0    14564 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/dataset.py
+-rw-r--r--   0        0        0      790 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/embedding.py
+-rw-r--r--   0        0        0     9595 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/evaluation.py
+-rw-r--r--   0        0        0     6437 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/main.py
+-rw-r--r--   0        0        0     4107 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/openai_adapter.py
+-rw-r--r--   0        0        0    17018 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/plugin.py
+-rw-r--r--   0        0        0    23840 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/trainer.py
+-rw-r--r--   0        0        0     3265 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/txt2img.py
+-rw-r--r--   0        0        0     9991 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/utils.py
+-rw-r--r--   0        0        0        1 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/hub/__init__.py
+-rw-r--r--   0        0        0     5823 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/hub/hub.py
+-rw-r--r--   0        0        0     3512 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/hub/interface.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/persister/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/persister/base.py
+-rw-r--r--   0        0        0     2965 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/persister/persist.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/prompt/__init__.py
+-rw-r--r--   0        0        0    23878 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/runnable/__init__.py
+-rw-r--r--   0        0        0     6386 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/runnable/base.py
+-rw-r--r--   0        0        0     3698 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/tool/baidu_search_tool.py
+-rw-r--r--   0        0        0     7561 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/tool/base_tool.py
+-rw-r--r--   0        0        0     2962 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/tool/duckduckgo_search_tool.py
+-rw-r--r--   0        0        0     3312 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/tool/wikipedia_tool.py
+-rw-r--r--   0        0        0     9582 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/config.py
+-rw-r--r--   0        0        0    12267 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/consts.py
+-rw-r--r--   0        0        0     1367 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/__init__.py
+-rw-r--r--   0        0        0     2786 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/consts.py
+-rw-r--r--   0        0        0     4363 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_operator.py
+-rw-r--r--   0        0        0     1013 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/__init__.py
+-rw-r--r--   0        0        0    27521 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/baidu_qianfan.py
+-rw-r--r--   0        0        0     2701 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/base.py
+-rw-r--r--   0        0        0    13584 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/bos.py
+-rw-r--r--   0        0        0     9420 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/chunk_reader.py
+-rw-r--r--   0        0        0     9532 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/file.py
+-rw-r--r--   0        0        0    23618 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/utils.py
+-rw-r--r--   0        0        0    58798 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/dataset.py
+-rw-r--r--   0        0        0    14197 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/dataset_utils.py
+-rw-r--r--   0        0        0     1139 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/__init__.py
+-rw-r--r--   0        0        0     2237 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/base.py
+-rw-r--r--   0        0        0     3942 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_character_repetition_filter.py
+-rw-r--r--   0        0        0     4482 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_flagged_words.py
+-rw-r--r--   0        0        0     2443 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_sentence_length_filter.py
+-rw-r--r--   0        0        0     2504 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_special_characters.py
+-rw-r--r--   0        0        0     4313 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_stopwords.py
+-rw-r--r--   0        0        0     3085 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_word_number.py
+-rw-r--r--   0        0        0     3910 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_word_repetition_filter.py
+-rw-r--r--   0        0        0     4483 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/consts.py
+-rw-r--r--   0        0        0     4693 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/utils.py
+-rw-r--r--   0        0        0   136258 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/word_list.py
+-rw-r--r--   0        0        0     2832 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/process_interface.py
+-rw-r--r--   0        0        0     4363 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/qianfan_data_operators.py
+-rw-r--r--   0        0        0    10622 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/dataset/schema.py
+-rw-r--r--   0        0        0    40452 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/dataset/table.py
+-rw-r--r--   0        0        0     1302 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/dataset/table_utils.py
+-rw-r--r--   0        0        0     2334 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/errors.py
+-rw-r--r--   0        0        0      878 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/__init__.py
+-rw-r--r--   0        0        0     2748 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/consts.py
+-rw-r--r--   0        0        0    26228 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/evaluation_manager.py
+-rw-r--r--   0        0        0     1325 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/evaluation_result.py
+-rw-r--r--   0        0        0     4484 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/evaluator.py
+-rw-r--r--   0        0        0     4379 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/local_evaluator.py
+-rw-r--r--   0        0        0     2468 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/opencompass_evaluator.py
+-rw-r--r--   0        0        0       66 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/langchain/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/langchain/agents/__init__.py
+-rw-r--r--   0        0        0    13709 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/openai/__init__.py
+-rw-r--r--   0        0        0    18554 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/openai/adapter.py
+-rw-r--r--   0        0        0     1602 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0     7804 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py
+-rw-r--r--   0        0        0     1627 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py
+-rw-r--r--   0        0        0     5365 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py
+-rw-r--r--   0        0        0     4056 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py
+-rw-r--r--   0        0        0     2577 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/fake_pyarrow_replacer.py
+-rw-r--r--   0        0        0      742 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/model/__init__.py
+-rw-r--r--   0        0        0      923 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/model/configs.py
+-rw-r--r--   0        0        0      938 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/model/consts.py
+-rw-r--r--   0        0        0    22871 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/py.typed
+-rw-r--r--   0        0        0     1648 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/auth/__init__.py
+-rw-r--r--   0        0        0     1656 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/auth/iam.py
+-rw-r--r--   0        0        0    15255 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/auth/oauth.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/__init__.py
+-rw-r--r--   0        0        0     4183 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/charge.py
+-rw-r--r--   0        0        0     7503 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/consts.py
+-rw-r--r--   0        0        0    30894 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/data.py
+-rw-r--r--   0        0        0    16279 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/finetune.py
+-rw-r--r--   0        0        0    23076 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/model.py
+-rw-r--r--   0        0        0    19491 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/prompt.py
+-rw-r--r--   0        0        0     5607 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/service.py
+-rw-r--r--   0        0        0     4941 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/utils.py
+-rw-r--r--   0        0        0     3779 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/http_client.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/images/__init__.py
+-rw-r--r--   0        0        0    11411 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/images/image2text.py
+-rw-r--r--   0        0        0    11777 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/images/text2image.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/__init__.py
+-rw-r--r--   0        0        0    27287 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/base.py
+-rw-r--r--   0        0        0    42166 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/chat_completion.py
+-rw-r--r--   0        0        0    11545 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/completion.py
+-rw-r--r--   0        0        0    10678 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/embedding.py
+-rw-r--r--   0        0        0    13139 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/plugin.py
+-rw-r--r--   0        0        0    14096 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/requestor/__init__.py
+-rw-r--r--   0        0        0    12834 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/requestor/base.py
+-rw-r--r--   0        0        0     3189 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/requestor/console_requestor.py
+-rw-r--r--   0        0        0    21478 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/requestor/openapi_requestor.py
+-rw-r--r--   0        0        0     9899 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/token_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/tools/__init__.py
+-rw-r--r--   0        0        0     4909 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/tools/tokenizer.py
+-rw-r--r--   0        0        0     3580 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/tools/utils.py
+-rw-r--r--   0        0        0     9199 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/typing.py
+-rw-r--r--   0        0        0     1141 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/__init__.py
+-rw-r--r--   0        0        0    44551 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/actions.py
+-rw-r--r--   0        0        0     6000 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/base.py
+-rw-r--r--   0        0        0    38156 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/configs.py
+-rw-r--r--   0        0        0     3600 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/consts.py
+-rw-r--r--   0        0        0     3403 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/event.py
+-rw-r--r--   0        0        0    11390 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/finetune.py
+-rw-r--r--   0        0        0     9561 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/pipeline.py
+-rw-r--r--   0        0        0     7772 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/post_pretrain.py
+-rw-r--r--   0        0        0     1680 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/ppl.yaml
+-rw-r--r--   0        0        0     4709 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/trainer.py
+-rw-r--r--   0        0        0     1244 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/utils/__init__.py
+-rw-r--r--   0        0        0     4647 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/utils/bos_uploader.py
+-rw-r--r--   0        0        0      696 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/cache/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/cache/base.py
+-rw-r--r--   0        0        0      827 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/__init__.py
+-rw-r--r--   0        0        0      730 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/compute.py
+-rw-r--r--   0        0        0      812 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/functions.py
+-rw-r--r--   0        0        0      869 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/ipc.py
+-rw-r--r--   0        0        0      984 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/table.py
+-rw-r--r--   0        0        0     1084 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/helper.py
+-rw-r--r--   0        0        0     5670 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/logging.py
+-rw-r--r--   0        0        0      734 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0     7230 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/utils.py
+-rw-r--r--   0        0        0      900 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/version.py
+-rw-r--r--   0        0        0    10341 1970-01-01 00:00:00.000000 qianfan-0.3.7.1/PKG-INFO
```

### Comparing `qianfan-0.3.7/README.pypi.md` & `qianfan-0.3.7.1/README.pypi.md`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/pyproject.toml` & `qianfan-0.3.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qianfan"
-version = "0.3.7"
+version = "0.3.7.1"
 description = "文心千帆大模型平台 Python SDK"
 authors = []
 license = "Apache-2.0"
 readme = "README.pypi.md"
 exclude = [
     "qianfan/tests",
     "qianfan/docs",
@@ -25,15 +25,15 @@
 pydantic = "*"
 python-dotenv = [
     { version = "<=0.21.1", python = "<3.8" },
     { version = ">=1.0", python = ">=3.8" }
 ]
 tenacity = "^8.2.3"
 multiprocess = "*"
-langchain = { version = ">=0.0.321", python = ">=3.8.1", optional = true }
+langchain = { version = ">=0.1.10", python = ">=3.8.1", optional = true }
 numpy = [
     { version = "<1.22.0", python = ">=3.7 <3.8", optional = true },
     { version = ">=1.22.0", python = ">=3.8", optional = true }
 ]
 pyarrow = [
     { version = ">=14.0.1", python = ">=3.8", optional = true },
     { version = "<=12.0.1", python = ">=3.7 <3.8", optional = true }
@@ -75,14 +75,20 @@
 sphinx-rtd-theme = ">=1.2.0"
 mypy = ">=1.4.0"
 myst-parser = ">=0.19.2"
 pytest-mock = "3.11.1"
 types-protobuf = "4.24.0.4"
 setuptools = "*"
 
+[tool.poetry.group.cookbook.dependencies]
+nbformat = {version = "^5.10.3", python = ">=3.8 <4"}
+aiohttp = {version = "^3.9.3", python = ">=3.8 <4"}
+papermill = {version = "*", python = ">=3.8 <4"}
+ipykernel = {version = "^6.29.4", python = ">=3.8 <4"}
+
 [tool.poetry.extras]
 dataset_base = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson"]
 langchain = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson", "langchain"]
 local_data_clean = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson", "ltp", "emoji", "sentencepiece", "torch"]
 openai = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson", "fastapi", "uvicorn"]
 extension = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson", "langchain", "ltp", "emoji", "sentencepiece", "torch", "fastapi", "uvicorn"]
```

### Comparing `qianfan-0.3.7/qianfan/__init__.py` & `qianfan-0.3.7.1/qianfan/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/__init__.py` & `qianfan-0.3.7.1/qianfan/autotuner/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/context.py` & `qianfan-0.3.7.1/qianfan/autotuner/context.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/launcher.py` & `qianfan-0.3.7.1/qianfan/autotuner/launcher.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/runner/__init__.py` & `qianfan-0.3.7.1/qianfan/autotuner/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/runner/base.py` & `qianfan-0.3.7.1/qianfan/autotuner/runner/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/runner/infer_runner.py` & `qianfan-0.3.7.1/qianfan/autotuner/runner/infer_runner.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/runner/qianfan_runner.py` & `qianfan-0.3.7.1/qianfan/autotuner/runner/qianfan_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     ) -> List[List[Dict[str, Any]]]:
         """
         Format the input using the prompt.
         """
         if self.prompt is not None:
             for i in range(len(input_list)):
                 content = input_list[i][-1]["content"]
-                new_content = self.prompt.render(content=content)
+                new_content, _ = self.prompt.render(content=content)
                 input_list[i][-1]["content"] = new_content
         return input_list
 
     async def _infer(self, config: Config, content: Context) -> List[Dict[str, Any]]:
         """
         Infer the whole dataset.
         """
```

### Comparing `qianfan-0.3.7/qianfan/autotuner/space.py` & `qianfan-0.3.7.1/qianfan/autotuner/space.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/suggestor/__init__.py` & `qianfan-0.3.7.1/qianfan/autotuner/suggestor/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/suggestor/base.py` & `qianfan-0.3.7.1/qianfan/autotuner/suggestor/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/suggestor/random_suggestor.py` & `qianfan-0.3.7.1/qianfan/autotuner/suggestor/random_suggestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/tune.py` & `qianfan-0.3.7.1/qianfan/autotuner/tune.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/autotuner/utils.py` & `qianfan-0.3.7.1/qianfan/autotuner/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/__init__.py` & `qianfan-0.3.7.1/qianfan/common/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/chat.py` & `qianfan-0.3.7.1/qianfan/common/client/chat.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/completion.py` & `qianfan-0.3.7.1/qianfan/common/client/completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/dataset.py` & `qianfan-0.3.7.1/qianfan/common/client/dataset.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/embedding.py` & `qianfan-0.3.7.1/qianfan/common/client/embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/evaluation.py` & `qianfan-0.3.7.1/qianfan/common/client/evaluation.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/main.py` & `qianfan-0.3.7.1/qianfan/common/client/main.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/openai_adapter.py` & `qianfan-0.3.7.1/qianfan/common/client/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/plugin.py` & `qianfan-0.3.7.1/qianfan/common/client/plugin.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/trainer.py` & `qianfan-0.3.7.1/qianfan/common/client/trainer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/txt2img.py` & `qianfan-0.3.7.1/qianfan/common/client/txt2img.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/client/utils.py` & `qianfan-0.3.7.1/qianfan/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/hub/hub.py` & `qianfan-0.3.7.1/qianfan/common/hub/hub.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/hub/interface.py` & `qianfan-0.3.7.1/qianfan/common/hub/interface.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/persister/base.py` & `qianfan-0.3.7.1/qianfan/common/persister/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/persister/persist.py` & `qianfan-0.3.7.1/qianfan/common/persister/persist.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/prompt/prompt.py` & `qianfan-0.3.7.1/qianfan/common/prompt/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
             if status == 2:  # fininished
                 break
             elif status == 3:  # failed
                 raise RequestError("Prompt optimization task failed.")
             time.sleep(1)
         optimized_prompt = resp["result"]["optimizeContent"]
 
-        return Prompt(optimized_prompt)
+        return Prompt(optimized_prompt, identifier=self.identifier)
 
     @dataclass
     class PromptEvaluateResult(object):
         """
         Evaluation result of a prompt
         """
```

### Comparing `qianfan-0.3.7/qianfan/common/runnable/base.py` & `qianfan-0.3.7.1/qianfan/common/runnable/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/tool/baidu_search_tool.py` & `qianfan-0.3.7.1/qianfan/common/tool/baidu_search_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/tool/base_tool.py` & `qianfan-0.3.7.1/qianfan/common/tool/base_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/tool/duckduckgo_search_tool.py` & `qianfan-0.3.7.1/qianfan/common/tool/duckduckgo_search_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/common/tool/wikipedia_tool.py` & `qianfan-0.3.7.1/qianfan/common/tool/wikipedia_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/config.py` & `qianfan-0.3.7.1/qianfan/config.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/consts.py` & `qianfan-0.3.7.1/qianfan/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/__init__.py` & `qianfan-0.3.7.1/qianfan/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/consts.py` & `qianfan-0.3.7.1/qianfan/dataset/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/data_operator.py` & `qianfan-0.3.7.1/qianfan/dataset/data_operator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/data_source/__init__.py` & `qianfan-0.3.7.1/qianfan/dataset/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/data_source/baidu_qianfan.py` & `qianfan-0.3.7.1/qianfan/dataset/data_source/baidu_qianfan.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/data_source/base.py` & `qianfan-0.3.7.1/qianfan/dataset/data_source/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/data_source/bos.py` & `qianfan-0.3.7.1/qianfan/dataset/data_source/bos.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/data_source/chunk_reader.py` & `qianfan-0.3.7.1/qianfan/dataset/data_source/chunk_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         data_list: List[Any] = []
         for i in range(chunk_size):
             try:
                 data_list.append(self._get_an_element(i))
             except StopIteration:
                 break
             except Exception as e:
-                err_msg = f"exception occurred during read csv file streamly: {e}"
+                err_msg = f"exception occurred during read file streamly: {e}"
                 log_error(err_msg)
                 raise e
 
         return data_list
 
     @abstractmethod
     def _get_an_element(self, index: int) -> Any:
```

### Comparing `qianfan-0.3.7/qianfan/dataset/data_source/file.py` & `qianfan-0.3.7.1/qianfan/dataset/data_source/file.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/data_source/utils.py` & `qianfan-0.3.7.1/qianfan/dataset/data_source/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/dataset.py` & `qianfan-0.3.7.1/qianfan/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1294,34 +1294,29 @@
             is_download_to_local=output_prettified,
             **kwargs,
         )
 
         if not output_prettified and result_dataset.is_dataset_located_in_qianfan():
             return result_dataset
 
-        result_dataset.unpack()
+        def _map_func(entry: Dict[str, Any]) -> Dict[str, Any]:
+            return {
+                "prompt": entry["prompt"],
+                NewInputPromptColumnName: entry["prompt"],
+                LLMOutputColumnName: entry["completion"],
+                OldReferenceColumnName: _extract_string(entry["response"]),
+            }
 
-        new_list: List[Dict[str, Any]] = []
-        for entry in result_dataset.list():
-            new_list.append(
-                {
-                    "prompt": entry["prompt"],
-                    NewInputPromptColumnName: entry["prompt"],
-                    LLMOutputColumnName: entry["model_response"][0]["content"],
-                    OldReferenceColumnName: _extract_string(entry["response"]),
-                }
-            )
+        result_dataset = result_dataset.map(_map_func)
+        result_dataset.input_columns = ["prompt"]
+        result_dataset.reference_column = OldReferenceColumnName
+        result_dataset.eval_input_column = NewInputPromptColumnName
+        result_dataset.eval_llm_output_column = LLMOutputColumnName
 
-        return Dataset.create_from_pyobj(
-            new_list,
-            input_columns=["prompt"],
-            reference_column=OldReferenceColumnName,
-            eval_input_column=NewInputPromptColumnName,
-            eval_llm_output_column=LLMOutputColumnName,
-        )
+        return result_dataset
 
     def _get_completion_return_dataset(
         self,
         input_str_list: List[str],
         output_list: List[str],
         request_latency_list: List[float],
         first_token_latency_list: List[float],
```

### Comparing `qianfan-0.3.7/qianfan/dataset/dataset_utils.py` & `qianfan-0.3.7.1/qianfan/dataset/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/__init__.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/base.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/check_character_repetition_filter.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_character_repetition_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/check_flagged_words.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_flagged_words.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/check_sentence_length_filter.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_sentence_length_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/check_special_characters.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_special_characters.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/check_stopwords.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_stopwords.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/check_word_number.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_word_number.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/check_word_repetition_filter.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_word_repetition_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/consts.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/utils.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/local_data_operators/word_list.py` & `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/word_list.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/process_interface.py` & `qianfan-0.3.7.1/qianfan/dataset/process_interface.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/qianfan_data_operators.py` & `qianfan-0.3.7.1/qianfan/dataset/qianfan_data_operators.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/schema.py` & `qianfan-0.3.7.1/qianfan/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/table.py` & `qianfan-0.3.7.1/qianfan/dataset/table.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/dataset/table_utils.py` & `qianfan-0.3.7.1/qianfan/dataset/table_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/errors.py` & `qianfan-0.3.7.1/qianfan/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 
 class InternalError(QianfanError):
     """Exception when internal error occurs"""
 
     pass
 
 
+class AuthError(QianfanError):
+    """Exception when auth failed"""
+
+    pass
+
+
 class ValidationError(Exception):
     """Exception when validating failed"""
 
     ...
 
 
 class QianfanRequestError(Exception):
```

### Comparing `qianfan-0.3.7/qianfan/evaluation/__init__.py` & `qianfan-0.3.7.1/qianfan/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/evaluation/consts.py` & `qianfan-0.3.7.1/qianfan/evaluation/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/evaluation/evaluation_manager.py` & `qianfan-0.3.7.1/qianfan/evaluation/evaluation_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,34 +12,37 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """
 manager which manage whole procedure of evaluation
 """
+import json
 import math
 import multiprocessing
 import os.path
 import shutil
 import time
 import zipfile
 from concurrent.futures import ALL_COMPLETED, Future, ThreadPoolExecutor, wait
 from copy import copy
 from typing import Any, Dict, List, Optional, Sequence, Set, Union
 
 import pyarrow
 
 from qianfan import get_config
+from qianfan.config import encoding
 from qianfan.dataset import Dataset
 from qianfan.dataset.consts import (
     LLMOutputColumnName,
     LLMTagColumnName,
     OldReferenceColumnName,
 )
 from qianfan.dataset.data_source import FileDataSource, QianfanDataSource
+from qianfan.dataset.data_source.chunk_reader import JsonLineReader
 from qianfan.dataset.data_source.utils import (
     _download_file_from_url_streamly,
 )
 from qianfan.dataset.schema import EvaluationSchema
 from qianfan.errors import QianfanError
 from qianfan.evaluation.consts import QianfanRefereeEvaluatorPromptTemplate
 from qianfan.evaluation.evaluation_result import EvaluationResult
@@ -57,14 +60,52 @@
     EvaluationTaskStatus,
 )
 from qianfan.utils import log_debug, log_error, log_info, log_warn
 from qianfan.utils.pydantic import BaseModel, Field, root_validator
 from qianfan.utils.utils import generate_letter_num_random_id
 
 
+def _convert_the_value_in_evaluation_into_str(json_line_path: str) -> str:
+    reader = JsonLineReader(json_line_path)
+    new_file_path = os.path.join(
+        os.path.split(json_line_path)[0], "tmp_eval_modify.jsonl"
+    )
+
+    is_judge_reason_existed_checked: bool = False
+
+    with open(new_file_path, mode="w", encoding=encoding()) as f:
+        for entry in reader:
+            for inner_list in entry:
+                for single_entry in inner_list:
+                    # 判断是否包含 judge_reason，如果包含则退出
+                    if "evaluation" not in single_entry or (
+                        not is_judge_reason_existed_checked
+                        and not any(
+                            [
+                                v == "judge_reason"
+                                for item in single_entry["evaluation"]
+                                for _, v in item.items()
+                            ]
+                        )
+                    ):
+                        return json_line_path
+
+                    is_judge_reason_existed_checked = True
+
+                    single_entry["evaluation"] = [
+                        {k: str(v) for k, v in item.items()}
+                        for item in single_entry["evaluation"]
+                    ]
+
+                json.dump(inner_list, f, ensure_ascii=False)
+                f.write("\n")
+
+    return new_file_path
+
+
 class EvaluationManager(BaseModel):
     """logic control center of evaluation"""
 
     local_evaluators: Optional[List[LocalEvaluator]] = Field(default=None)
     qianfan_evaluators: Optional[List[QianfanEvaluator]] = Field(default=None)
     task_id: Optional[str] = Field(default=None)
 
@@ -178,14 +219,15 @@
         for llm in llms:
             if isinstance(llm, Service):
                 if llm.model:
                     llm_key_str = f"{llm.id}_{llm.endpoint}_{llm.model.name}"
                 else:
                     llm_key_str = f"{llm.id}_{llm.endpoint}"
             elif isinstance(llm, Model):
+                llm.auto_complete_info()
                 llm_key_str = f"{llm.id}_{llm.version_id}_{llm.name}"
             else:
                 llm_key_str = ""
             llm_tags.append(llm_key_str)
 
         return llm_tags
 
@@ -476,35 +518,49 @@
                         f" evaluation: {e}"
                     )
                     log_warn(err_msg)
 
             # 整合数据，将得到的数据集整合成网页人工评估的数据集格式
             log_info("start to merge evaluation result dataset")
             table_list: List[pyarrow.Table] = []
+            metrics_dict: Dict[str, Dict[str, Any]] = {}
+
             for index, response_list in llm_response_list.items():
                 index_tag_column = [llm_tags[index] for _ in range(len(response_list))]
                 ds = dataset.create_from_pyobj(
                     {
                         LLMTagColumnName: index_tag_column,
                         input_column_name: llm_input_list,
                         OldReferenceColumnName: expected_output_list,
                         LLMOutputColumnName: response_list,
                     }
                 )
 
                 metrics_ds = dataset.create_from_pyobj(
                     llm_evaluation_result_dict[index]
                 )
+
                 ds.col_append(metrics_ds.col_list())
                 table_list.append(ds.inner_table)
 
+                summarization_dict: Dict[str, Any] = {}
+
+                for evaluator in self.local_evaluators:
+                    summarization = evaluator.summarize(metrics_ds)
+                    if summarization:
+                        summarization_dict.update(summarization)
+
+                if summarization_dict:
+                    metrics_dict[llm_tags[index]] = summarization_dict
+
             return EvaluationResult(
                 result_dataset=Dataset.create_from_pyarrow_table(
                     pyarrow.concat_tables(table_list)
-                )
+                ),
+                metrics=metrics_dict,
             )
 
         if self.qianfan_evaluators:
             # 检查是否有不支持的实例
             if any([not isinstance(inst, Model) for inst in llms]):
                 err_msg = "only Model instance can use QianfanEvaluator"
                 log_error(err_msg)
@@ -589,14 +645,18 @@
             unfold_zip_file_path = "tmp_folder"
             data_jsonl_file_path = os.path.join(unfold_zip_file_path, "data.jsonl")
             try:
                 _download_file_from_url_streamly(download_url, local_cache_file_path)
                 with zipfile.ZipFile(local_cache_file_path) as zip_f:
                     zip_f.extractall(unfold_zip_file_path)
 
+                data_jsonl_file_path = _convert_the_value_in_evaluation_into_str(
+                    data_jsonl_file_path
+                )
+
                 # 返回指标信息
                 return EvaluationResult(
                     result_dataset=Dataset.load(
                         FileDataSource(path=data_jsonl_file_path)
                     ),
                     metrics=metric_list,
                 )
```

### Comparing `qianfan-0.3.7/qianfan/evaluation/evaluation_result.py` & `qianfan-0.3.7.1/qianfan/evaluation/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/evaluation/evaluator.py` & `qianfan-0.3.7.1/qianfan/evaluation/evaluator.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 """
 collection of evaluator
 """
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Union
 
+from qianfan.dataset import Dataset
 from qianfan.evaluation.consts import (
     QianfanRefereeEvaluatorDefaultMaxScore,
     QianfanRefereeEvaluatorDefaultMetrics,
     QianfanRefereeEvaluatorDefaultSteps,
 )
 from qianfan.utils import log_error
 from qianfan.utils.pydantic import BaseModel, Field, root_validator
@@ -33,14 +34,29 @@
 
     @abstractmethod
     def evaluate(
         self, input: Union[str, List[Dict[str, Any]]], reference: str, output: str
     ) -> Dict[str, Any]:
         """evaluate one entry"""
 
+    def summarize(self, metric_dataset: Dataset) -> Optional[Dict[str, Any]]:
+        """
+        The default implementation of summarize interface,
+        which is designed to get a summarization from custom metrics
+
+        Args:
+            metric_dataset (Dataset): a Dataset object containing all metrics
+            for one specific evaluated llm
+
+        Returns:
+            Optional[Dict[str, Any]]: A dict including summarization info, or None
+            for nothing happened
+        """
+        return None
+
 
 class LocalEvaluator(Evaluator, ABC):
     """
     Bass class for evaluator running locally
 
     For user who want to implement their own LocalEvaluator,
     they should overwrite function `evaluate`,
```

### Comparing `qianfan-0.3.7/qianfan/evaluation/local_evaluator.py` & `qianfan-0.3.7.1/qianfan/evaluation/local_evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/evaluation/opencompass_evaluator.py` & `qianfan-0.3.7.1/qianfan/evaluation/opencompass_evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py` & `qianfan-0.3.7.1/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     BaseMessage,
     BasePromptTemplate,
     FunctionMessage,
     SystemMessage,
 )
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.tools import BaseTool, format_tool_to_openai_function
+from langchain_core.runnables import RunnableConfig
 
 # langchain 新版本有部分逻辑迁移至 langchain_core
 # 为了兼容老版本而 try catch
 try:
     from langchain_core.callbacks.base import Callbacks
     from langchain_core.prompts import (
         ChatPromptTemplate,
@@ -155,16 +156,21 @@
         **kwargs: Any,
     ) -> Union[AgentAction, AgentFinish]:
         """plan an action"""
         tool_history = _convert_action_into_message(intermediate_steps)
         messages = self.prompt.format_prompt(
             history=tool_history, **kwargs
         ).to_messages()
-        result: BaseMessage = self.llm.predict_messages(
-            messages, callbacks=callbacks, functions=self._wrapper_function, **kwargs
+        if "input" in kwargs:
+            kwargs.pop("input")
+        result: BaseMessage = self.llm.invoke(  # type: ignore
+            messages,
+            RunnableConfig(callbacks=callbacks),
+            functions=self._wrapper_function,
+            **kwargs,
         )
         action = self._parse_message_to_action(result)
 
         assert isinstance(action, (AgentAction, AgentFinish))
         return action
 
     async def aplan(
@@ -174,16 +180,21 @@
         **kwargs: Any,
     ) -> Union[AgentAction, AgentFinish]:
         """plan an action asynchronously"""
         tool_history = _convert_action_into_message(intermediate_steps)
         messages = self.prompt.format_prompt(
             history=tool_history, **kwargs
         ).to_messages()
-        result: BaseMessage = await self.llm.apredict_messages(
-            messages, callbacks=callbacks, functions=self._wrapper_function, **kwargs
+        if "input" in kwargs:
+            kwargs.pop("input")
+        result: BaseMessage = await self.llm.ainvoke(
+            messages,
+            RunnableConfig(callbacks=callbacks),
+            functions=self._wrapper_function,
+            **kwargs,
         )
         action = self._parse_message_to_action(result)
 
         assert isinstance(action, (AgentAction, AgentFinish))
         return action
 
     @classmethod
@@ -267,16 +278,21 @@
         **kwargs: Any,
     ) -> Union[List[AgentAction], AgentFinish]:
         """plan an action"""
         tool_history = _convert_action_into_message(intermediate_steps)
         messages = self.prompt.format_prompt(
             history=tool_history, **kwargs
         ).to_messages()
-        result: BaseMessage = self.llm.predict_messages(
-            messages, callbacks=callbacks, functions=self._wrapper_function, **kwargs
+        if "input" in kwargs:
+            kwargs.pop("input")
+        result: BaseMessage = self.llm.invoke(  # type: ignore
+            messages,
+            RunnableConfig(callbacks=callbacks),
+            functions=self._wrapper_function,
+            **kwargs,
         )
         action = self._parse_message_to_action(result)
         assert isinstance(action, (list, AgentFinish))
         return action
 
     async def aplan(
         self,
@@ -285,16 +301,21 @@
         **kwargs: Any,
     ) -> Union[List[AgentAction], AgentFinish]:
         """plan an action asynchronously"""
         tool_history = _convert_action_into_message(intermediate_steps)
         messages = self.prompt.format_prompt(
             history=tool_history, **kwargs
         ).to_messages()
-        result: BaseMessage = await self.llm.apredict_messages(
-            messages, callbacks=callbacks, functions=self._wrapper_function, **kwargs
+        if "input" in kwargs:
+            kwargs.pop("input")
+        result: BaseMessage = await self.llm.ainvoke(
+            messages,
+            RunnableConfig(callbacks=callbacks),
+            functions=self._wrapper_function,
+            **kwargs,
         )
         action = self._parse_message_to_action(result)
         assert isinstance(action, (list, AgentFinish))
         return action
 
     @classmethod
     def _default_system_prompt(cls) -> SystemMessage:
@@ -352,15 +373,20 @@
         cls, result: BaseMessage
     ) -> Union[List[AgentAction], AgentFinish]:
         if result.content:
             return AgentFinish(
                 return_values={"output": result.content}, log=str(result)
             )
 
-        arg_str = result.additional_kwargs.get("function_call", {}).get("arguments", "")
+        if hasattr(result, "response_metadata"):
+            tool_json = result.response_metadata.get("function_call", {})  # noqa
+        else:
+            tool_json = result.additional_kwargs.get("function_call", {})
+
+        arg_str = tool_json.get("arguments", "")
         if not arg_str:
             raise ValueError("arguments retrieved from service is empty")
         action_list = json.loads(arg_str)["actions"]
         if not isinstance(action_list, list):
             raise TypeError("arguments isn't a list containing actions")
 
         actions = []
```

### Comparing `qianfan-0.3.7/qianfan/extensions/openai/adapter.py` & `qianfan-0.3.7.1/qianfan/extensions/openai/adapter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/extensions/semantic_kernel/__init__.py` & `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py` & `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py` & `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py` & `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py` & `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/fake_pyarrow_replacer.py` & `qianfan-0.3.7.1/qianfan/fake_pyarrow_replacer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/model/__init__.py` & `qianfan-0.3.7.1/qianfan/model/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/model/configs.py` & `qianfan-0.3.7.1/qianfan/model/configs.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/model/consts.py` & `qianfan-0.3.7.1/qianfan/model/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/model/model.py` & `qianfan-0.3.7.1/qianfan/model/model.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/__init__.py` & `qianfan-0.3.7.1/qianfan/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/auth/iam.py` & `qianfan-0.3.7.1/qianfan/resources/auth/iam.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/auth/oauth.py` & `qianfan-0.3.7.1/qianfan/resources/auth/oauth.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import threading
 import time
 from typing import Any, Dict, Optional, Tuple
 
 from qianfan.config import get_config
 from qianfan.consts import Consts
-from qianfan.errors import InternalError, InvalidArgumentError
+from qianfan.errors import AuthError, InternalError, InvalidArgumentError
 from qianfan.resources.http_client import HTTPClient
 from qianfan.resources.typing import QfRequest, RetryConfig
 from qianfan.utils import (
     AsyncLock,
     log_error,
     log_info,
     log_warn,
@@ -172,14 +172,29 @@
         self, obj: AccessToken, response: Dict[str, Any], ak: str = "", sk: str = ""
     ) -> None:
         """
         update access token from response of auth request
         this function is not thread safe and should be protected by lock from obj !!!
         """
         if "error" in response:
+            error = response["error"]
+            if error == "invalid_client":
+                exception_msg_tmpl = (
+                    "{}, please check! AK/SK should be obtained from"
+                    " https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application"
+                )
+                err_msg = response.get("error_description", "AK/SK is not correct")
+                if err_msg == "unknown client id":
+                    err_msg = f"AK({_masked_ak(ak)}) is not correct"
+                if err_msg == "Client authentication failed":
+                    err_msg = f"SK({_masked_ak(sk)}) is not correct"
+                err_msg = exception_msg_tmpl.format(err_msg)
+                log_error(err_msg)
+                raise AuthError(err_msg)
+            # unexpected error, maybe it can be recovered by retrying.
             log_error(
                 "refresh access_token for ak `{}` failed, error description={}".format(
                     _masked_ak(ak), response["error_description"]
                 )
             )
             return
         obj.token = response["access_token"]
@@ -209,14 +224,16 @@
             # the token should not be refreshed multiple times
             if self._refresh_access_token_too_often(obj):
                 return
             try:
                 resp = self._client.request(self._auth_request(ak, sk))
                 json_body = resp.json()
                 self._update_access_token(obj, json_body, ak, sk)
+            except AuthError:
+                raise
             except Exception as e:
                 log_error(f"refresh access token failed with exception {str(e)}")
                 return
 
         log_info("sucessfully refresh access_token")
 
     async def arefresh_access_token(self, ak: str, sk: str) -> None:
@@ -232,14 +249,16 @@
             if self._refresh_access_token_too_often(obj):
                 return
             try:
                 resp, session = await self._client.arequest(self._auth_request(ak, sk))
                 async with session:
                     json_body = await resp.json()
                 self._update_access_token(obj, json_body, ak, sk)
+            except AuthError:
+                raise
             except Exception as e:
                 log_error(f"refresh access token failed with exception {str(e)}")
                 return
 
         log_info(f"sucessfully refresh access_token for ak `{_masked_ak(ak)}`")
```

### Comparing `qianfan-0.3.7/qianfan/resources/console/charge.py` & `qianfan-0.3.7.1/qianfan/resources/console/charge.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/console/consts.py` & `qianfan-0.3.7.1/qianfan/resources/console/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/console/data.py` & `qianfan-0.3.7.1/qianfan/resources/console/data.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/console/finetune.py` & `qianfan-0.3.7.1/qianfan/resources/console/finetune.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/console/model.py` & `qianfan-0.3.7.1/qianfan/resources/console/model.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/console/prompt.py` & `qianfan-0.3.7.1/qianfan/resources/console/prompt.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/console/service.py` & `qianfan-0.3.7.1/qianfan/resources/console/service.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/console/utils.py` & `qianfan-0.3.7.1/qianfan/resources/console/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/http_client.py` & `qianfan-0.3.7.1/qianfan/resources/http_client.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/images/image2text.py` & `qianfan-0.3.7.1/qianfan/resources/images/image2text.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/images/text2image.py` & `qianfan-0.3.7.1/qianfan/resources/images/text2image.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/llm/base.py` & `qianfan-0.3.7.1/qianfan/resources/llm/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/llm/chat_completion.py` & `qianfan-0.3.7.1/qianfan/resources/llm/chat_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/llm/completion.py` & `qianfan-0.3.7.1/qianfan/resources/llm/completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/llm/embedding.py` & `qianfan-0.3.7.1/qianfan/resources/llm/embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/llm/plugin.py` & `qianfan-0.3.7.1/qianfan/resources/llm/plugin.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/rate_limiter.py` & `qianfan-0.3.7.1/qianfan/resources/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/requestor/base.py` & `qianfan-0.3.7.1/qianfan/resources/requestor/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/requestor/console_requestor.py` & `qianfan-0.3.7.1/qianfan/resources/requestor/console_requestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/requestor/openapi_requestor.py` & `qianfan-0.3.7.1/qianfan/resources/requestor/openapi_requestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/token_limiter.py` & `qianfan-0.3.7.1/qianfan/resources/token_limiter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/tools/tokenizer.py` & `qianfan-0.3.7.1/qianfan/resources/tools/tokenizer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/tools/utils.py` & `qianfan-0.3.7.1/qianfan/resources/tools/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/resources/typing.py` & `qianfan-0.3.7.1/qianfan/resources/typing.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/__init__.py` & `qianfan-0.3.7.1/qianfan/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/actions.py` & `qianfan-0.3.7.1/qianfan/trainer/actions.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/base.py` & `qianfan-0.3.7.1/qianfan/trainer/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/configs.py` & `qianfan-0.3.7.1/qianfan/trainer/configs.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/consts.py` & `qianfan-0.3.7.1/qianfan/trainer/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/event.py` & `qianfan-0.3.7.1/qianfan/trainer/event.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/finetune.py` & `qianfan-0.3.7.1/qianfan/trainer/finetune.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/pipeline.py` & `qianfan-0.3.7.1/qianfan/trainer/pipeline.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/post_pretrain.py` & `qianfan-0.3.7.1/qianfan/trainer/post_pretrain.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/ppl.yaml` & `qianfan-0.3.7.1/qianfan/trainer/ppl.yaml`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/trainer/trainer.py` & `qianfan-0.3.7.1/qianfan/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/__init__.py` & `qianfan-0.3.7.1/qianfan/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/bos_uploader.py` & `qianfan-0.3.7.1/qianfan/utils/bos_uploader.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/cache/__init__.py` & `qianfan-0.3.7.1/qianfan/utils/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/cache/base.py` & `qianfan-0.3.7.1/qianfan/utils/cache/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/fake_pyarrow/__init__.py` & `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/fake_pyarrow/compute.py` & `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/compute.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/fake_pyarrow/functions.py` & `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/functions.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/fake_pyarrow/ipc.py` & `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/ipc.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/fake_pyarrow/table.py` & `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/table.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/helper.py` & `qianfan-0.3.7.1/qianfan/utils/helper.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/logging.py` & `qianfan-0.3.7.1/qianfan/utils/logging.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/pydantic/__init__.py` & `qianfan-0.3.7.1/qianfan/utils/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/utils/utils.py` & `qianfan-0.3.7.1/qianfan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/qianfan/version.py` & `qianfan-0.3.7.1/qianfan/version.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7/PKG-INFO` & `qianfan-0.3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qianfan
-Version: 0.3.7
+Version: 0.3.7.1
 Summary: 文心千帆大模型平台 Python SDK
 Home-page: https://cloud.baidu.com/product/wenxinworkshop
 License: Apache-2.0
 Keywords: baidu,qianfan
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 Requires-Dist: clevercsv (<=0.8.0) ; (python_version < "3.8") and (extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension")
 Requires-Dist: clevercsv ; (python_version >= "3.8") and (extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension")
 Requires-Dist: diskcache (>=5.6.3,<6.0.0)
 Requires-Dist: emoji ; extra == "local-data-clean" or extra == "extension"
 Requires-Dist: fastapi ; extra == "openai" or extra == "extension"
 Requires-Dist: ijson ; extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension"
 Requires-Dist: importlib-metadata (>=1.4.0) ; python_full_version <= "3.7.0"
-Requires-Dist: langchain (>=0.0.321) ; (python_full_version >= "3.8.1") and (extra == "langchain" or extra == "extension")
+Requires-Dist: langchain (>=0.1.10) ; (python_full_version >= "3.8.1") and (extra == "langchain" or extra == "extension")
 Requires-Dist: ltp ; extra == "local-data-clean" or extra == "extension"
 Requires-Dist: multiprocess
 Requires-Dist: numpy (<1.22.0) ; (python_version >= "3.7" and python_version < "3.8") and (extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension")
 Requires-Dist: numpy (>=1.22.0) ; (python_version >= "3.8") and (extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension")
 Requires-Dist: prompt-toolkit (>=3.0.38)
 Requires-Dist: pyarrow (<=12.0.1) ; (python_version >= "3.7" and python_version < "3.8") and (extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension")
 Requires-Dist: pyarrow (>=14.0.1) ; (python_version >= "3.8") and (extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension")
```

