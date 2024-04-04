# Comparing `tmp/r2r-0.1.28.tar.gz` & `tmp/r2r-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.1.28.tar", max compression
+gzip compressed data, was "r2r-0.1.29.tar", max compression
```

## Comparing `r2r-0.1.28.tar` & `r2r-0.1.29.tar`

### file list

```diff
@@ -1,88 +1,85 @@
--rw-r--r--   0        0        0     1082 2024-03-29 05:10:44.004187 r2r-0.1.28/LICENSE.md
--rw-r--r--   0        0        0     6938 2024-03-29 05:10:44.004187 r2r-0.1.28/README.md
--rw-r--r--   0        0        0      683 2024-03-29 05:10:44.004187 r2r-0.1.28/config.json
--rw-r--r--   0        0        0     2118 2024-03-29 05:10:44.024187 r2r-0.1.28/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/__init__.py
--rw-r--r--   0        0        0       53 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/client/__init__.py
--rw-r--r--   0        0        0     5430 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/client/base.py
--rw-r--r--   0        0        0     1123 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/__init__.py
--rw-r--r--   0        0        0      110 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      773 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/abstractions/output.py
--rw-r--r--   0        0        0      249 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/adapters/__init__.py
--rw-r--r--   0        0        0     2928 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/adapters/advanced/reducto.py
--rw-r--r--   0        0        0     2797 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/adapters/base.py
--rw-r--r--   0        0        0     2406 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/pipelines/embedding.py
--rw-r--r--   0        0        0     1334 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/pipelines/eval.py
--rw-r--r--   0        0        0     2175 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/pipelines/ingestion.py
--rw-r--r--   0        0        0     1515 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/pipelines/pipeline.py
--rw-r--r--   0        0        0     6226 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/pipelines/rag.py
--rw-r--r--   0        0        0      935 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/providers/embedding.py
--rw-r--r--   0        0        0      603 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/providers/eval.py
--rw-r--r--   0        0        0     1772 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/providers/llm.py
--rw-r--r--   0        0        0    11873 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/providers/logging.py
--rw-r--r--   0        0        0     1249 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/providers/prompt.py
--rw-r--r--   0        0        0     3833 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/providers/vector_db.py
--rw-r--r--   0        0        0      256 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      176 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/utils/base.py
--rw-r--r--   0        0        0       95 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66611 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      203 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     1676 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/embeddings/modal/base.py
--rw-r--r--   0        0        0     3309 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/embeddings/openai/base.py
--rw-r--r--   0        0        0     1923 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/embeddings/setence_transformer/base.py
--rw-r--r--   0        0        0       76 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2067 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/eval/deepeval/base.py
--rw-r--r--   0        0        0     2659 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/eval/parea/base.py
--rw-r--r--   0        0        0        0 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/examples/academy/__init__.py
--rw-r--r--   0        0        0     5638 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/examples/academy/app.py
--rw-r--r--   0        0        0     1504 2024-03-29 05:10:44.024187 r2r-0.1.28/r2r/examples/academy/client.py
--rw-r--r--   0        0        0   802904 2024-03-29 05:10:44.028187 r2r-0.1.28/r2r/examples/academy/meditations.pdf
--rw-r--r--   0        0        0     1574 2024-03-29 05:10:44.028187 r2r-0.1.28/r2r/examples/academy/run_client.py
--rw-r--r--   0        0        0  1307590 2024-03-29 05:10:44.036187 r2r-0.1.28/r2r/examples/academy/the_republic.pdf
--rw-r--r--   0        0        0        0 2024-03-29 05:10:44.036187 r2r-0.1.28/r2r/examples/basic/__init__.py
--rw-r--r--   0        0        0      277 2024-03-29 05:10:44.036187 r2r-0.1.28/r2r/examples/basic/app.py
--rw-r--r--   0        0        0     3978 2024-03-29 05:10:44.036187 r2r-0.1.28/r2r/examples/basic/run_client.py
--rw-r--r--   0        0        0    14812 2024-03-29 05:10:44.036187 r2r-0.1.28/r2r/examples/basic/test.pdf
--rw-r--r--   0        0        0        0 2024-03-29 05:10:44.036187 r2r-0.1.28/r2r/examples/pdf_chat/__init__.py
--rw-r--r--   0        0        0   802904 2024-03-29 05:10:44.040187 r2r-0.1.28/r2r/examples/pdf_chat/meditations.pdf
--rw-r--r--   0        0        0     2658 2024-03-29 05:10:44.040187 r2r-0.1.28/r2r/examples/pdf_chat/run_client.py
--rw-r--r--   0        0        0  1307590 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/examples/pdf_chat/the_republic.pdf
--rw-r--r--   0        0        0        0 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/examples/reducto/__init__.py
--rw-r--r--   0        0        0      284 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/examples/reducto/app.py
--rw-r--r--   0        0        0        0 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/examples/web_search/__init__.py
--rw-r--r--   0        0        0      362 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/examples/web_search/app.py
--rw-r--r--   0        0        0       61 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1184 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3893 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/integrations/serper.py
--rw-r--r--   0        0        0      167 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3602 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/llms/litellm/base.py
--rw-r--r--   0        0        0     3793 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/llms/openai/base.py
--rw-r--r--   0        0        0      217 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/main/__init__.py
--rw-r--r--   0        0        0    16146 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/main/app.py
--rw-r--r--   0        0        0     4659 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/main/factory.py
--rw-r--r--   0        0        0     3280 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/main/models.py
--rw-r--r--   0        0        0    10757 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/main/utils.py
--rw-r--r--   0        0        0      541 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/pipelines/__init__.py
--rw-r--r--   0        0        0     5959 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/pipelines/basic/embedding.py
--rw-r--r--   0        0        0     1235 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/pipelines/basic/eval.py
--rw-r--r--   0        0        0     2977 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/pipelines/basic/ingestion.py
--rw-r--r--   0        0        0     1002 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/pipelines/basic/prompt_provider.py
--rw-r--r--   0        0        0     3078 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/pipelines/basic/rag.py
--rw-r--r--   0        0        0     2391 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/pipelines/web_search/rag.py
--rw-r--r--   0        0        0     6035 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/tests/end_to_end.py
--rw-r--r--   0        0        0    14812 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/tests/test.pdf
--rw-r--r--   0        0        0      539 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-03-29 05:10:44.044187 r2r-0.1.28/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3269 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5298 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     7510 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vecs/client.py
--rw-r--r--   0        0        0    35440 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vecs/exc.py
--rw-r--r--   0        0        0      166 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     5881 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vector_dbs/local/base.py
--rw-r--r--   0        0        0     5607 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vector_dbs/pg_vector/base.py
--rw-r--r--   0        0        0     7125 2024-03-29 05:10:44.048187 r2r-0.1.28/r2r/vector_dbs/qdrant/base.py
--rw-r--r--   0        0        0     9264 1970-01-01 00:00:00.000000 r2r-0.1.28/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-04 17:32:45.964493 r2r-0.1.29/LICENSE.md
+-rw-r--r--   0        0        0     6625 2024-04-04 17:32:45.964493 r2r-0.1.29/README.md
+-rw-r--r--   0        0        0      680 2024-04-04 17:32:45.964493 r2r-0.1.29/config.json
+-rw-r--r--   0        0        0     2252 2024-04-04 17:32:45.980493 r2r-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/client/__init__.py
+-rw-r--r--   0        0        0     5956 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/client/base.py
+-rw-r--r--   0        0        0     1123 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      781 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/abstractions/output.py
+-rw-r--r--   0        0        0      249 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2928 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/adapters/advanced/reducto.py
+-rw-r--r--   0        0        0     2797 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/adapters/base.py
+-rw-r--r--   0        0        0     2407 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/embedding.py
+-rw-r--r--   0        0        0     1334 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/eval.py
+-rw-r--r--   0        0        0     2175 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/ingestion.py
+-rw-r--r--   0        0        0     1515 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/pipeline.py
+-rw-r--r--   0        0        0     6227 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/pipelines/rag.py
+-rw-r--r--   0        0        0      935 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/embedding.py
+-rw-r--r--   0        0        0      789 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/eval.py
+-rw-r--r--   0        0        0     1773 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/llm.py
+-rw-r--r--   0        0        0    11873 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/logging.py
+-rw-r--r--   0        0        0     1249 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/prompt.py
+-rw-r--r--   0        0        0     3833 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/providers/vector_db.py
+-rw-r--r--   0        0        0      256 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/utils/base.py
+-rw-r--r--   0        0        0       95 2024-04-04 17:32:45.980493 r2r-0.1.29/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66651 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      203 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     1676 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/embeddings/modal/base.py
+-rw-r--r--   0        0        0     3311 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/embeddings/openai/base.py
+-rw-r--r--   0        0        0     1923 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/embeddings/setence_transformer/base.py
+-rw-r--r--   0        0        0      139 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2169 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/eval/deepeval/base.py
+-rw-r--r--   0        0        0     2676 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/eval/parea/base.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/clients/__init__.py
+-rw-r--r--   0        0        0     3135 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/clients/run_basic_client.py
+-rw-r--r--   0        0        0     4063 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/clients/run_basic_client_old.py
+-rw-r--r--   0        0        0     1625 2024-04-04 17:32:45.984493 r2r-0.1.29/r2r/examples/clients/run_synthetic_query_client.py
+-rw-r--r--   0        0        0   802904 2024-04-04 17:32:45.988493 r2r-0.1.29/r2r/examples/data/meditations.pdf
+-rw-r--r--   0        0        0    14812 2024-04-04 17:32:45.988493 r2r-0.1.29/r2r/examples/data/test.pdf
+-rw-r--r--   0        0        0  1307590 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/data/the_republic.pdf
+-rw-r--r--   0        0        0        0 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0      526 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/basic_pipeline.py
+-rw-r--r--   0        0        0      533 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/reducto_pipeline.py
+-rw-r--r--   0        0        0     6746 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/synthetic_query_pipeline.py
+-rw-r--r--   0        0        0      504 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/examples/servers/web_search_pipeline.py
+-rw-r--r--   0        0        0      101 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1184 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3905 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      276 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3602 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/litellm/base.py
+-rw-r--r--   0        0        0     4419 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/llamacpp/base.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/llamacpp/model/__init__.py
+-rw-r--r--   0        0        0     3794 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/llms/openai/base.py
+-rw-r--r--   0        0        0      217 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/__init__.py
+-rw-r--r--   0        0        0    16236 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/app.py
+-rw-r--r--   0        0        0     4966 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/factory.py
+-rw-r--r--   0        0        0     3280 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/models.py
+-rw-r--r--   0        0        0    10797 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/main/utils.py
+-rw-r--r--   0        0        0      541 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/__init__.py
+-rw-r--r--   0        0        0     5948 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/embedding.py
+-rw-r--r--   0        0        0     1767 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/eval.py
+-rw-r--r--   0        0        0     2978 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/ingestion.py
+-rw-r--r--   0        0        0     1002 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/prompt_provider.py
+-rw-r--r--   0        0        0     3079 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/basic/rag.py
+-rw-r--r--   0        0        0     2392 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/pipelines/web_search/rag.py
+-rw-r--r--   0        0        0     6035 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/tests/end_to_end.py
+-rw-r--r--   0        0        0    14812 2024-04-04 17:32:45.992493 r2r-0.1.29/r2r/tests/test.pdf
+-rw-r--r--   0        0        0      539 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3269 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5299 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9298 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/client.py
+-rw-r--r--   0        0        0    35441 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      166 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     5881 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vector_dbs/local/base.py
+-rw-r--r--   0        0        0     5607 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vector_dbs/pg_vector/base.py
+-rw-r--r--   0        0        0     7125 2024-04-04 17:32:45.996493 r2r-0.1.29/r2r/vector_dbs/qdrant/base.py
+-rw-r--r--   0        0        0     9094 1970-01-01 00:00:00.000000 r2r-0.1.29/PKG-INFO
```

### Comparing `r2r-0.1.28/LICENSE.md` & `r2r-0.1.29/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/README.md` & `r2r-0.1.29/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,131 @@
-# R2R: Production-ready RAG systems.
-
 <p align="left">
   <a href="https://r2r-docs.sciphi.ai"><img src="https://img.shields.io/badge/docs.sciphi.ai-3F16E4" alt="Docs"></a>
   <a href="https://discord.gg/p6KqD2kjtB"><img src="https://img.shields.io/discord/1120774652915105934?style=social&logo=discord" alt="Discord"></a>
   <a href="https://github.com/SciPhi-AI"><img src="https://img.shields.io/github/stars/SciPhi-AI/R2R" alt="Github Stars"></a>
   <a href="https://github.com/SciPhi-AI/R2R/pulse"><img src="https://img.shields.io/github/commit-activity/w/SciPhi-AI/R2R" alt="Commits-per-week"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-purple.svg" alt="License: MIT"></a>
 </p>
 
-A semi-opinionated RAG framework.
-
 <img src="./docs/pages/r2r.png" alt="Sciphi Framework">
-R2R was conceived to bridge the gap between experimental RAG models and robust, production-ready systems. Our semi-opinionated framework cuts through the complexity, offering a straightforward path to deploy, adapt, and maintain RAG pipelines in production. We prioritize simplicity and practicality, aiming to set a new industry benchmark for ease of use and effectiveness.
+<h3 align="center">
+Build, deploy, and optimize your RAG system.
+</h3>
+
+## About
+
+R2R, short for RAG to Riches, provides the fastest and most efficient way to provide high quality RAG to end users. The framework is built around customizable pipelines and a feature-rich FastAPI implementation.
+
+## Why?
+
+R2R was conceived to bridge the gap between local LLM experimentation and scalable production solutions. **R2R is to LangChain/LlamaIndex what NextJS is to React**. A JavaScript client for R2R deployments can be [found here](https://github.com/SciPhi-AI/r2r-js).
+
+### Key Features
+
+- **🚀 Deploy**: Instantly launch production-ready RAG pipelines with streaming capabilities.
+- **🧩 Customize**: Tailor your pipeline with intuitive configuration files.
+- **🔌 Extend**: Enhance your pipeline with custom code integrations.
+- **⚖️ Autoscale**: Scale your pipeline effortlessly in the cloud using [SciPhi](https://app.sciphi.ai/).
+- **🤖 OSS**: Benefit from a framework developed by the open-source community, designed to simplify RAG deployment.
 
 ## Demo(s)
 
-Using cloud application to deploy the pre-built basic pipeline:
+Using the cloud application to deploy the pre-built basic pipeline:
+
 https://www.loom.com/share/e3b934b554484787b005702ced650ac9
 
-!! Note - The server has been removed from this repo - instead we now recommend using [SciPhi Cloud](https://app.sciphi.ai) to pair with the R2R framework for observability and optimization.
+Note - the example above uses [SciPhi Cloud](https://app.sciphi.ai) to pair with the R2R framework for deployment and observability. SciPhi is working to launch a self-hosted version of their cloud platform as R2R matures.
 
-### Quick Install:
+## Links
+
+[Join the Discord server](https://discord.gg/p6KqD2kjtB)
+
+[R2R Docs Quickstart](https://r2r-docs.sciphi.ai/getting-started/quick-install)
+
+[SciPhi Cloud](https://docs.sciphi.ai/)
 
-**Install R2R directly using `pip`:**
+## Quick Install:
 
 ```bash
 # use the `'r2r[all]'` to download all required deps
 pip install 'r2r[parsing,eval]'
 
 # setup env 
 export OPENAI_API_KEY=sk-...
+# Set `LOCAL_DB_PATH` for local testing
 export LOCAL_DB_PATH=local.sqlite
 
 # OR do `vim .env.example && cp .env.example .env`
 # INCLUDE secrets and modify config.json
-# if using cloud providers (e.g. pgvector, supabase, ...)
+# if using cloud providers (e.g. pgvector, qdrant, ...)
 ```
 
-### Run the server with Docker:
+## Docker:
 
 ```bash
 docker pull emrgntcmplxty/r2r:latest
 
-# Place your secrets in `.env` before deploying
+# Place your secrets in `.env`
 docker run -d --name r2r_container -p 8000:8000 --env-file .env r2r
 ```
 
-## Links
-
-[Join the Discord server](https://discord.gg/p6KqD2kjtB)
-
-[Read the R2R Docs](https://r2r-docs.sciphi.ai/)
+## Basic Example
 
-## Basic Examples
-
-The project includes several basic examples that demonstrate application deployment and interaction:
-
-1. [`basic app`](r2r/examples/basic/app.py): This example runs the backend server, which includes the ingestion, embedding, and RAG pipelines served via FastAPI.
+[`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the default **backend server**. It establishes a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes, all accessible via FastAPI.
 
    ```bash
-   # If using a venv, replace `uvicorn` with `venv_path/bin/uvicorn`
-   uvicorn r2r.examples.basic.app:app
+   # launch the server
+   python -m r2r.examples.servers.basic_pipeline
    ```
 
-2. [`basic client`](r2r/examples/basic/run_client.py): This example should be run after starting the server. It demonstrates uploading text entries as well as a PDF to the local server with the python client. Further, it shows document and user-level vector management with built-in features.
+[`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This **client script** should be executed subsequent to the server startup above. It facilitates the upload of text entries and PDFs to the server using the Python client and demonstrates the management of document and user-level vectors through its built-in features.
 
    ```bash
-   python -m r2r.examples.basic.run_client
+   # run the client
+   python -m r2r.examples.clients.run_basic_client
    ```
 
-3. [`academy`](r2r/examples/academy): A more sophisticated demo demonstrating how to build a more novel pipeline which involves synthetic queries
+## Synthetic Queries Example
 
-   ```bash
-   # Launch the `academy` example application
-   # If using a venv, replace `uvicorn` with `venv_path/bin/uvicorn`
-   uvicorn r2r.examples.academy.app:app
+[`synthetic_query_pipeline.py`](r2r/examples/servers/synthetic_query_pipeline.py): Execute this script to start a backend server equipped with an advanced pipeline. This pipeline is designed to create synthetic queries, enhancing the RAG system's learning and performance.
 
-   # Ask a question
-   python -m r2r.examples.academy.run_client search "What are the key themes of Meditations?"
+   ```bash
+   # launch the server
+   python -m r2r.examples.servers.synthetic_query_pipeline
    ```
-4. [`end-to-end`](docs/pages/examples/end-to-end.mdx): An example showing how to combine a complete web application with the basic RAG pipeline above.
-
-5. [`intelligence`](app.sciphi.ai): A cloud platform which can be used to deploy R2R pipelines powered by SciPhi
-
-
-
-### Full Install:
-
-Follow these steps to ensure a smooth setup:
 
-1. **Install Poetry:**
+[`run_synthetic_query_client.py`](r2r/examples/clients/run_synthetic_query_client.py): Use this client script after the synthetic query pipeline is running. It's tailored for use with the synthetic query pipeline, demonstrating the improved features of the RAG system.
 
-   - Before installing the project, make sure you have Poetry on your system. If not, visit the [official Poetry website](https://python-poetry.org/docs/#installation) for installation instructions.
-
-2. **Clone and Install Dependencies:**
-
-  - Clone the project repository and navigate to the project directory:
-     
-     ```bash
-     git clone git@github.com:SciPhi-AI/r2r.git
-     cd r2r
-     ```
-     
-  - Copy the `.env.example` file to `.env`. This file is in the main project folder:
+   ```bash
+   # run the client
+   python -m r2r.examples.clients.run_synthetic_query_client
+   ```
 
-     ```bash
-     cp .env.example .env
+## Extras Examples
 
-     # Add secrets, `OPENAI_API_KEY` at a minimum
-     vim .env
-     ```
-     
-  - Install the project dependencies with Poetry:
-  
-     ```bash
-     # See pyproject.toml for available extras
-     # use "all" to include every optional dependency
-     poetry install -E parsing -E eval
-     ```
-     
-  - Execute with poetry run:
-     
-     ```bash
-     python -m r2r.examples.pdf_chat.run_client ingest
-     ```
+[`reducto_pipeline.py`](r2r/examples/servers/reducto_pipeline.py): Launch this script to activate a backend server that integrates a Reducto adapter for enhanced PDF ingestion.
 
-3. **Configure Environment Variables:**
-   - You need to set up cloud provider secrets in your `.env`. At a minimum, you will need an OpenAI key.
-   - The framework currently supports PostgreSQL (locally), pgvector and Qdrant with plans to extend coverage.
+   ```bash
+   # launch the server
+   python -m r2r.examples.servers.reducto_pipeline
+   ```
 
-## Key Features
+[`web_search_pipeline.py`](r2r/examples/servers/web_search_pipeline.py): This script sets up a backend server that includes a `WebSearchRAGPipeline`, adding web search functionality to your RAG setup.
 
-- **🚀 Rapid Deployment**: Facilitates a smooth setup and development of production-ready RAG systems.
-- **⚖️ Flexible Standardization**: `Ingestion`, `Embedding`, and `RAG` with proper `Observability`.
-- **🧩 Easy to modify**: Provides a structure that can be extended to deploy your own custom pipelines.
-- **📦 Versioning**: Ensures your work remains reproducible and traceable through version control.
-- **🔌 Extensibility**: Enables a quick and robust integration with various VectorDBs, LLMs and Embeddings Models.
-- **🤖 OSS Driven**: Built for and by the OSS community, to help startups and enterprises to quickly build with RAG.
-- **📝 Deployment Support**: Available to help you build and deploy your RAG systems end-to-end.
+   ```bash
+   # launch the server
+   python -m r2r.examples.servers.web_search_pipeline
+   ```
 
 ## Core Abstractions
 
 The framework primarily revolves around three core abstractions:
 
-- The **Ingestion Pipeline**: Facilitates the preparation of embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.). The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/ingestion.py).
+- The **Ingestion Pipeline**: Facilitates the preparation of embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.). The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/ingestion).
 
-- The **Embedding Pipeline**: Manages the transformation of text into stored vector embeddings, interacting with embedding and vector database providers through a series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks, etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/embedding.py).
+- The **Embedding Pipeline**: Manages the transformation of text into stored vector embeddings, interacting with embedding and vector database providers through a series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks, etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/embedding.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/embedding).
 
-- The **RAG Pipeline**: Works similarly to the embedding pipeline but incorporates an LLM provider to produce text completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/rag.py).
+- The **RAG Pipeline**: Works similarly to the embedding pipeline but incorporates an LLM provider to produce text completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/rag.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/rag).
 
-- The **Eval Pipeline**: Samples some subset of rag_completion calls for evaluation. Currently [DeepEval](https://github.com/confident-ai/deepeval) is supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/eval.py).
+- The **Eval Pipeline**: Samples some subset of rag_completion calls for evaluation. Currently [DeepEval](https://github.com/confident-ai/deepeval) is supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/eval).
 
 Each pipeline incorporates a logging database for operation tracking and observability.
```

#### html2text {}

```diff
@@ -1,82 +1,79 @@
-# R2R: Production-ready RAG systems.
 _[_D_o_c_s_]_[_D_i_s_c_o_r_d_]_[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
-A semi-opinionated RAG framework. [Sciphi Framework]R2R was conceived to bridge
-the gap between experimental RAG models and robust, production-ready systems.
-Our semi-opinionated framework cuts through the complexity, offering a
-straightforward path to deploy, adapt, and maintain RAG pipelines in
-production. We prioritize simplicity and practicality, aiming to set a new
-industry benchmark for ease of use and effectiveness. ## Demo(s) Using cloud
-application to deploy the pre-built basic pipeline: https://www.loom.com/share/
-e3b934b554484787b005702ced650ac9 !! Note - The server has been removed from
-this repo - instead we now recommend using [SciPhi Cloud](https://
-app.sciphi.ai) to pair with the R2R framework for observability and
-optimization. ### Quick Install: **Install R2R directly using `pip`:** ```bash
-# use the `'r2r[all]'` to download all required deps pip install 'r2r
-[parsing,eval]' # setup env export OPENAI_API_KEY=sk-... export
+[Sciphi Framework]
+            ******** BBuuiilldd,, ddeeppllooyy,, aanndd ooppttiimmiizzee yyoouurr RRAAGG ssyysstteemm.. ********
+## About R2R, short for RAG to Riches, provides the fastest and most efficient
+way to provide high quality RAG to end users. The framework is built around
+customizable pipelines and a feature-rich FastAPI implementation. ## Why? R2R
+was conceived to bridge the gap between local LLM experimentation and scalable
+production solutions. **R2R is to LangChain/LlamaIndex what NextJS is to
+React**. A JavaScript client for R2R deployments can be [found here](https://
+github.com/SciPhi-AI/r2r-js). ### Key Features - **ð Deploy**: Instantly
+launch production-ready RAG pipelines with streaming capabilities. - **ð§©
+Customize**: Tailor your pipeline with intuitive configuration files. - **ð
+Extend**: Enhance your pipeline with custom code integrations. - **âï¸
+Autoscale**: Scale your pipeline effortlessly in the cloud using [SciPhi]
+(https://app.sciphi.ai/). - **ð¤ OSS**: Benefit from a framework developed by
+the open-source community, designed to simplify RAG deployment. ## Demo(s)
+Using the cloud application to deploy the pre-built basic pipeline: https://
+www.loom.com/share/e3b934b554484787b005702ced650ac9 Note - the example above
+uses [SciPhi Cloud](https://app.sciphi.ai) to pair with the R2R framework for
+deployment and observability. SciPhi is working to launch a self-hosted version
+of their cloud platform as R2R matures. ## Links [Join the Discord server]
+(https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart](https://r2r-
+docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud](https://
+docs.sciphi.ai/) ## Quick Install: ```bash # use the `'r2r[all]'` to download
+all required deps pip install 'r2r[parsing,eval]' # setup env export
+OPENAI_API_KEY=sk-... # Set `LOCAL_DB_PATH` for local testing export
 LOCAL_DB_PATH=local.sqlite # OR do `vim .env.example && cp .env.example .env` #
 INCLUDE secrets and modify config.json # if using cloud providers (e.g.
-pgvector, supabase, ...) ``` ### Run the server with Docker: ```bash docker
-pull emrgntcmplxty/r2r:latest # Place your secrets in `.env` before deploying
-docker run -d --name r2r_container -p 8000:8000 --env-file .env r2r ``` ##
-Links [Join the Discord server](https://discord.gg/p6KqD2kjtB) [Read the R2R
-Docs](https://r2r-docs.sciphi.ai/) ## Basic Examples The project includes
-several basic examples that demonstrate application deployment and interaction:
-1. [`basic app`](r2r/examples/basic/app.py): This example runs the backend
-server, which includes the ingestion, embedding, and RAG pipelines served via
-FastAPI. ```bash # If using a venv, replace `uvicorn` with `venv_path/bin/
-uvicorn` uvicorn r2r.examples.basic.app:app ``` 2. [`basic client`](r2r/
-examples/basic/run_client.py): This example should be run after starting the
-server. It demonstrates uploading text entries as well as a PDF to the local
-server with the python client. Further, it shows document and user-level vector
-management with built-in features. ```bash python -
-m r2r.examples.basic.run_client ``` 3. [`academy`](r2r/examples/academy): A
-more sophisticated demo demonstrating how to build a more novel pipeline which
-involves synthetic queries ```bash # Launch the `academy` example application #
-If using a venv, replace `uvicorn` with `venv_path/bin/uvicorn` uvicorn
-r2r.examples.academy.app:app # Ask a question python -
-m r2r.examples.academy.run_client search "What are the key themes of
-Meditations?" ``` 4. [`end-to-end`](docs/pages/examples/end-to-end.mdx): An
-example showing how to combine a complete web application with the basic RAG
-pipeline above. 5. [`intelligence`](app.sciphi.ai): A cloud platform which can
-be used to deploy R2R pipelines powered by SciPhi ### Full Install: Follow
-these steps to ensure a smooth setup: 1. **Install Poetry:** - Before
-installing the project, make sure you have Poetry on your system. If not, visit
-the [official Poetry website](https://python-poetry.org/docs/#installation) for
-installation instructions. 2. **Clone and Install Dependencies:** - Clone the
-project repository and navigate to the project directory: ```bash git clone
-git@github.com:SciPhi-AI/r2r.git cd r2r ``` - Copy the `.env.example` file to
-`.env`. This file is in the main project folder: ```bash cp .env.example .env #
-Add secrets, `OPENAI_API_KEY` at a minimum vim .env ``` - Install the project
-dependencies with Poetry: ```bash # See pyproject.toml for available extras #
-use "all" to include every optional dependency poetry install -E parsing -
-E eval ``` - Execute with poetry run: ```bash python -
-m r2r.examples.pdf_chat.run_client ingest ``` 3. **Configure Environment
-Variables:** - You need to set up cloud provider secrets in your `.env`. At a
-minimum, you will need an OpenAI key. - The framework currently supports
-PostgreSQL (locally), pgvector and Qdrant with plans to extend coverage. ## Key
-Features - **ð Rapid Deployment**: Facilitates a smooth setup and
-development of production-ready RAG systems. - **âï¸ Flexible
-Standardization**: `Ingestion`, `Embedding`, and `RAG` with proper
-`Observability`. - **ð§© Easy to modify**: Provides a structure that can be
-extended to deploy your own custom pipelines. - **ð¦ Versioning**: Ensures
-your work remains reproducible and traceable through version control. - **ð
-Extensibility**: Enables a quick and robust integration with various VectorDBs,
-LLMs and Embeddings Models. - **ð¤ OSS Driven**: Built for and by the OSS
-community, to help startups and enterprises to quickly build with RAG. - **ð
-Deployment Support**: Available to help you build and deploy your RAG systems
-end-to-end. ## Core Abstractions The framework primarily revolves around three
-core abstractions: - The **Ingestion Pipeline**: Facilitates the preparation of
-embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.).
-The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/
-ingestion.py). - The **Embedding Pipeline**: Manages the transformation of text
-into stored vector embeddings, interacting with embedding and vector database
-providers through a series of steps (e.g., extract_text, transform_text,
-chunk_text, embed_chunks, etc.). The abstraction can be found in
-[`embedding.py`](r2r/core/pipelines/embedding.py). - The **RAG Pipeline**:
-Works similarly to the embedding pipeline but incorporates an LLM provider to
-produce text completions. The abstraction can be found in [`rag.py`](r2r/core/
-pipelines/rag.py). - The **Eval Pipeline**: Samples some subset of
-rag_completion calls for evaluation. Currently [DeepEval](https://github.com/
-confident-ai/deepeval) is supported. The abstraction can be found in
-[`eval.py`](r2r/core/pipelines/eval.py). Each pipeline incorporates a logging
-database for operation tracking and observability.
+pgvector, qdrant, ...) ``` ## Docker: ```bash docker pull emrgntcmplxty/r2r:
+latest # Place your secrets in `.env` docker run -d --name r2r_container -
+p 8000:8000 --env-file .env r2r ``` ## Basic Example [`basic_pipeline.py`](r2r/
+examples/servers/basic_pipeline.py): Execute this script to initiate the
+default **backend server**. It establishes a basic RAG pipeline that
+encompasses ingestion, embedding, and RAG processes, all accessible via
+FastAPI. ```bash # launch the server python -
+m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
+clients/run_basic_client.py): This **client script** should be executed
+subsequent to the server startup above. It facilitates the upload of text
+entries and PDFs to the server using the Python client and demonstrates the
+management of document and user-level vectors through its built-in features.
+```bash # run the client python -m r2r.examples.clients.run_basic_client ``` ##
+Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/examples/servers/
+synthetic_query_pipeline.py): Execute this script to start a backend server
+equipped with an advanced pipeline. This pipeline is designed to create
+synthetic queries, enhancing the RAG system's learning and performance. ```bash
+# launch the server python -m r2r.examples.servers.synthetic_query_pipeline ```
+[`run_synthetic_query_client.py`](r2r/examples/clients/
+run_synthetic_query_client.py): Use this client script after the synthetic
+query pipeline is running. It's tailored for use with the synthetic query
+pipeline, demonstrating the improved features of the RAG system. ```bash # run
+the client python -m r2r.examples.clients.run_synthetic_query_client ``` ##
+Extras Examples [`reducto_pipeline.py`](r2r/examples/servers/
+reducto_pipeline.py): Launch this script to activate a backend server that
+integrates a Reducto adapter for enhanced PDF ingestion. ```bash # launch the
+server python -m r2r.examples.servers.reducto_pipeline ```
+[`web_search_pipeline.py`](r2r/examples/servers/web_search_pipeline.py): This
+script sets up a backend server that includes a `WebSearchRAGPipeline`, adding
+web search functionality to your RAG setup. ```bash # launch the server python
+-m r2r.examples.servers.web_search_pipeline ``` ## Core Abstractions The
+framework primarily revolves around three core abstractions: - The **Ingestion
+Pipeline**: Facilitates the preparation of embeddable 'Documents' from various
+data formats (json, txt, pdf, html, etc.). The abstraction can be found in
+[`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is
+available [here](https://r2r-docs.sciphi.ai/core-features/ingestion). - The
+**Embedding Pipeline**: Manages the transformation of text into stored vector
+embeddings, interacting with embedding and vector database providers through a
+series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks,
+etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/
+embedding.py) and relevant documentation is available [here](https://r2r-
+docs.sciphi.ai/core-features/embedding). - The **RAG Pipeline**: Works
+similarly to the embedding pipeline but incorporates an LLM provider to produce
+text completions. The abstraction can be found in [`rag.py`](r2r/core/
+pipelines/rag.py) and relevant documentation is available [here](https://r2r-
+docs.sciphi.ai/core-features/rag). - The **Eval Pipeline**: Samples some subset
+of rag_completion calls for evaluation. Currently [DeepEval](https://
+github.com/confident-ai/deepeval) is supported. The abstraction can be found in
+[`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available
+[here](https://r2r-docs.sciphi.ai/core-features/eval). Each pipeline
+incorporates a logging database for operation tracking and observability.
```

### Comparing `r2r-0.1.28/config.json` & `r2r-0.1.29/config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428571%*

 * *Differences: {"'evals'": "{'provider': 'parea'}"}*

```diff
@@ -7,15 +7,15 @@
         "batch_size": 32,
         "dimension": 1536,
         "model": "text-embedding-3-small",
         "provider": "openai"
     },
     "evals": {
         "frequency": 1.0,
-        "provider": "deepeval"
+        "provider": "parea"
     },
     "ingestion": {
         "provider": "local",
         "text_splitter": {
             "chunk_overlap": 20,
             "chunk_size": 512,
             "type": "recursive_character"
```

### Comparing `r2r-0.1.28/pyproject.toml` & `r2r-0.1.29/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 [build-system]
 requires = ["poetry-core", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "r2r"
-version = "0.1.28"
+version = "0.1.29"
 description = "SciPhi R2R"
 authors = ["Owen Colegrove <owen@sciphi.ai>"]
 license = "MIT"
 readme = "README.md"
 include = ["config.json"]
 
 [tool.poetry.dependencies]
 # Python Versions
 python = ">=3.9,<3.13"
 
 # Required dependencies
 fastapi = "^0.109.2"
 fire = "^0.5.0"
 gunicorn = "^21.2.0"
-litellm = "^1.28.0"
+litellm = "^1.34.0"
 openai = "^1.11.1"
 pydantic = "^2.6.3"
 python-dotenv = "^1.0.1"
 python-multipart = "^0.0.9"
 requests = "^2.31.0"
 types-requests = "^2.31.0"
 uvicorn = "^0.27.0.post1"
 vecs = "^0.4.0"
 
+
 # Optional dependencies
 bs4 = {version = "^0.0.2", optional = true}
 pypdf = {version = "^4.0.2", optional = true}
 tiktoken = {version = "^0.5.2", optional = true}
 datasets = {version = "^2.16.1", optional = true}
 qdrant_client = {version = "^1.7.0", optional = true}
 psycopg2-binary = {version = "^2.9.9", optional = true}
 numpy = {version = "^1.26.4", optional = true}
-scikit-learn = {version = "^1.4.1.post1", optional = true}
 sentry-sdk = {version = "^1.40.4", optional = true}
 deepeval = {version ="^0.20.88", optional = true}
 parea-ai = {version = "^0.2.86", optional = true}
 ionic-api-sdk = {version = "0.9.3", optional = true}
 boto3 = {version = "^1.34.71", optional = true}
+exa-py = {version = "^1.0.9", optional = true}
+llama-cpp-python = {version = "^0.2.57", optional = true}
+sentence-transformers = {version = "^2.6.1", optional = true}
 
 [tool.poetry.extras]
 parsing = ["bs4", "pypdf"]
 embedding = ["tiktoken"]
 streaming = ["datasets"]
 qdrant = ["qdrant_client"]
 postgres = ["psycopg2-binary"]
-local_vectordb = ["numpy", "scikit-learn"]
 monitoring = ["sentry-sdk"]
-eval = ["deepeval", "parea-ai"]
+deepeval = ["deepeval"]
+eval = ["parea-ai"]
 ionic = ["ionic-api-sdk"]
 reducto = ["boto3"]
-all = ["bs4", "pypdf", "tiktoken", "datasets", "qdrant_client", "psycopg2-binary", "numpy", "scikit-learn", "sentry-sdk", "protobuf", "deepeval", "parea-ai", "ionic"]
+exa = ["exa-py"]
+local_llm = ["llama-cpp-python", "sentence-transformers"]
+all = ["bs4", "pypdf", "tiktoken", "datasets", "qdrant_client", "psycopg2-binary", "sentry-sdk", "parea-ai", "boto3", "exa-py", "llama-cpp-python"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 flake8 = "6.1.0"
 isort = "5.12.0"
 mypy = "^1.5.1"
```

### Comparing `r2r-0.1.28/r2r/client/base.py` & `r2r-0.1.29/r2r/client/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         url = f"{self.base_url}/upload_and_process_file/"
         with open(file_path, "rb") as file:
             files = {
                 "file": (file_path.split("/")[-1], file, "application/pdf")
             }
             data = {
                 "document_id": document_id,
-                "metadata": json.dumps(metadata)
-                if metadata
-                else json.dumps({}),
-                "settings": json.dumps(settings)
-                if settings
-                else json.dumps({}),
+                "metadata": (
+                    json.dumps(metadata) if metadata else json.dumps({})
+                ),
+                "settings": (
+                    json.dumps(settings) if settings else json.dumps({})
+                ),
             }
             response = requests.post(
                 url,
                 files=files,
                 data=data,
             )
         return response.json()
@@ -117,14 +117,33 @@
             "limit": limit,
             "settings": settings or {},
             "generation_config": generation_config or {},
         }
         response = requests.post(url, json=json_data)
         return response.json()
 
+    def eval(
+        self,
+        query: str,
+        context: str,
+        completion_text: str,
+        run_id: str,
+        settings: Optional[Dict[str, Any]] = None,
+    ):
+        url = f"{self.base_url}/eval/"
+        payload = {
+            "query": query,
+            "context": context,
+            "completion_text": completion_text,
+            "run_id": run_id,
+            "settings": settings or {},
+        }
+        response = requests.post(url, json=payload)
+        return response.json()
+
     async def stream_rag_completion(
         self,
         query: str,
         limit: Optional[int] = 10,
         filters: Optional[Dict[str, Any]] = None,
         settings: Optional[Dict[str, Any]] = None,
         generation_config: Optional[Dict[str, Any]] = None,
```

### Comparing `r2r-0.1.28/r2r/core/__init__.py` & `r2r-0.1.29/r2r/core/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/adapters/advanced/reducto.py` & `r2r-0.1.29/r2r/core/adapters/advanced/reducto.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/adapters/base.py` & `r2r-0.1.29/r2r/core/adapters/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/pipelines/embedding.py` & `r2r-0.1.29/r2r/core/pipelines/embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Abstract base class for embedding pipelines.
 """
+
 import logging
 from abc import abstractmethod
 from typing import Any, Optional
 
 from ..providers.embedding import EmbeddingProvider
 from ..providers.logging import LoggingDatabaseConnection
 from ..providers.vector_db import VectorDBProvider, VectorEntry
```

### Comparing `r2r-0.1.28/r2r/core/pipelines/eval.py` & `r2r-0.1.29/r2r/core/pipelines/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/pipelines/ingestion.py` & `r2r-0.1.29/r2r/core/pipelines/ingestion.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/pipelines/pipeline.py` & `r2r-0.1.29/r2r/core/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/pipelines/rag.py` & `r2r-0.1.29/r2r/core/pipelines/rag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Abstract base class for completion pipelines.
 """
+
 import json
 import logging
 import uuid
 from abc import abstractmethod
 from typing import Any, Generator, Optional, Union
 
 from openai.types.chat import ChatCompletion
```

### Comparing `r2r-0.1.28/r2r/core/providers/embedding.py` & `r2r-0.1.29/r2r/core/providers/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/providers/llm.py` & `r2r-0.1.29/r2r/core/providers/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base classes for language model providers."""
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field, fields
 from typing import Optional
 
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
```

### Comparing `r2r-0.1.28/r2r/core/providers/logging.py` & `r2r-0.1.29/r2r/core/providers/logging.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/providers/prompt.py` & `r2r-0.1.29/r2r/core/providers/prompt.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/providers/vector_db.py` & `r2r-0.1.29/r2r/core/providers/vector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/core/utils/splitter/text.py` & `r2r-0.1.29/r2r/core/utils/splitter/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,17 +222,19 @@
             if secret_value is not None:
                 lc_kwargs.update({key: secret_value})
 
         return {
             "lc": 1,
             "type": "constructor",
             "id": self.lc_id(),
-            "kwargs": lc_kwargs
-            if not secrets
-            else _replace_secrets(lc_kwargs, secrets),
+            "kwargs": (
+                lc_kwargs
+                if not secrets
+                else _replace_secrets(lc_kwargs, secrets)
+            ),
         }
 
     def to_json_not_implemented(self) -> SerializedNotImplemented:
         return to_json_not_implemented(self)
 
 
 def _replace_secrets(
```

### Comparing `r2r-0.1.28/r2r/embeddings/modal/base.py` & `r2r-0.1.29/r2r/embeddings/modal/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/embeddings/openai/base.py` & `r2r-0.1.29/r2r/embeddings/openai/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         super().__init__(provider)
         if provider != "openai":
             raise ValueError(
                 "OpenAIEmbeddingProvider must be initialized with provider `openai`."
             )
         if not os.getenv("OPENAI_API_KEY"):
             raise ValueError(
-                "Must set OPEN_API_KEY in order to initialize OpenAIEmbeddingProvider."
+                "Must set OPENAI_API_KEY in order to initialize OpenAIEmbeddingProvider."
             )
         self.client = OpenAI()
 
     def _check_inputs(self, model: str, dimensions: Optional[int]) -> None:
         if model not in OpenAIEmbeddingProvider.MODEL_TO_TOKENIZER:
             raise ValueError(f"OpenAI embedding model {model} not supported.")
         if (
```

### Comparing `r2r-0.1.28/r2r/embeddings/setence_transformer/base.py` & `r2r-0.1.29/r2r/embeddings/setence_transformer/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/eval/deepeval/base.py` & `r2r-0.1.29/r2r/eval/deepeval/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 from r2r.core import EvalProvider
 
 
 class DeepEvalProvider(EvalProvider):
-    def __init__(self):
+    def __init__(self, provider: str, sampling_fraction: float = 1.0):
+        super().__init__(provider, sampling_fraction)
         try:
             from deepeval import evaluate
             from deepeval.metrics import (
                 AnswerRelevancyMetric,
                 HallucinationMetric,
             )
             from deepeval.test_case import LLMTestCase
@@ -22,15 +23,15 @@
                 "DeepEval is not installed. Please install it using `pip install deepeval`."
             )
         if not os.getenv("OPENAI_API_KEY"):
             raise ValueError(
                 "Please set the `OPENAI_API_KEY` environment variable to run with DeepEval."
             )
 
-    def evaluate(
+    def _evaluate(
         self, query: str, context: str, completion: str
     ) -> dict[str, dict[str, str]]:
         test_case = self.LLMTestCase(
             input=query,
             actual_output=completion,
             context=[context],
             retrieval_context=[context],
```

### Comparing `r2r-0.1.28/r2r/eval/parea/base.py` & `r2r-0.1.29/r2r/eval/parea/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from r2r.core.providers.eval import EvalProvider
 
 
 class PareaEvalProvider(EvalProvider):
-    def __init__(self, sampling_fraction: float = 1.0):
-        super().__init__("parea", sampling_fraction)
+    def __init__(self, provider: str, sampling_fraction: float = 1.0):
+        super().__init__(provider, sampling_fraction)
         try:
             from parea.evals.general import answer_relevancy_factory
             from parea.evals.rag import (
                 answer_context_faithfulness_statement_level_factory,
                 context_query_relevancy_factory,
                 context_ranking_pointwise_factory,
             )
@@ -39,15 +39,15 @@
                 "Parea is not installed. Please install it using `pip install parea`."
             )
         if not os.getenv("OPENAI_API_KEY"):
             raise ValueError(
                 "Please set the `OPENAI_API_KEY` environment variable to run with Parea."
             )
 
-    def evaluate(
+    def _evaluate(
         self, query: str, context: str, completion: str
     ) -> dict[str, dict[str, str | float]]:
         log = self._create_log(query, context, completion)
 
         answer_relevancy_score = self.answer_relevancy(log)
         context_query_relevancy_score = self.context_query_relevancy(log)
         context_ranking_pointwise_score = self.context_ranking_pointwise(log)
```

### Comparing `r2r-0.1.28/r2r/examples/academy/client.py` & `r2r-0.1.29/r2r/examples/clients/run_synthetic_query_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 from r2r.core.utils import generate_id_from_label
 
 # Initialize the client with the base URL of your API
 base_url = "http://localhost:8000"  # Change this to your actual API base URL
 client = R2RClient(base_url)
 
 titles = {
-    "examples/academy/meditations.pdf": "Title: Meditations - Marcus Aurelius",
-    "examples/academy/the_republic.pdf": "Title: The Republic - Plato",
+    "meditations.pdf": "Title: Meditations - Marcus Aurelius",
+    "the_republic.pdf": "Title: The Republic - Plato",
+    "test.pdf": "Title: A Test Document",
 }
 
 user_id_0 = generate_id_from_label("user_0")
 
-# Get the directory of the current file
-current_dir = os.path.dirname(os.path.abspath(__file__))
-
+current_file_directory = os.path.dirname(os.path.abspath(__file__))
+data_path = os.path.join(current_file_directory, "..", "data")
+print("data_path = ", data_path)
 # Use this directory in the glob pattern
-for file_path in glob.glob(os.path.join(current_dir, "*.pdf")):
+for file_path in glob.glob(os.path.join(data_path, "*.pdf")):
+    file_name = file_path.split(os.path.sep)[-1]
     print(f"Uploading and processing file: {file_path}")
     # # Upload and process a file
     document_id = str(generate_id_from_label(file_path))
-    metadata = {"user_id": user_id_0, "chunk_prefix": titles[file_path]}
+    metadata = {"user_id": user_id_0, "chunk_prefix": titles[file_name]}
     settings: dict = {}
     upload_response = client.upload_and_process_file(
         document_id, file_path, metadata, settings
     )
 
 prompt = """You are given a user query {query} and a user context {context}. Use the context to answer the given query. """
 formatted_prompt = prompt.format(
```

### Comparing `r2r-0.1.28/r2r/examples/academy/meditations.pdf` & `r2r-0.1.29/r2r/examples/data/meditations.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/examples/academy/the_republic.pdf` & `r2r-0.1.29/r2r/examples/data/the_republic.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/examples/basic/run_client.py` & `r2r-0.1.29/r2r/examples/clients/run_basic_client_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from r2r.client import R2RClient
 from r2r.core.utils import generate_id_from_label
 
 # Initialize the client with the base URL of your API
 base_url = "http://localhost:8000"
 client = R2RClient(base_url)
 
+from r2r.client import R2RClient
+
+# print('eval_result:', eval_result)
 print("Upserting entry to remote db...")
 # Upsert a single entry
 
 entry_response = client.add_entry(
     generate_id_from_label("doc 1"),
     {"txt": "This is a test entry"},
     {"tags": ["example", "test"]},
@@ -72,15 +75,15 @@
     f"Search response w/ filter+deletion:\n{post_deletion_filtered_search_response}\n\n"
 )
 
 # Example file path for upload
 # get file directory
 current_file_directory = os.path.dirname(os.path.realpath(__file__))
 
-file_path = os.path.join(current_file_directory, "test.pdf")
+file_path = os.path.join(current_file_directory, "..", "data", "test.pdf")
 
 print(f"Uploading and processing file: {file_path}...")
 # # Upload and process a file
 metadata = {"tags": ["example", "test"]}
 upload_pdf_response = client.upload_and_process_file(
     generate_id_from_label("pdf 1"), file_path, metadata, None
 )
```

### Comparing `r2r-0.1.28/r2r/examples/basic/test.pdf` & `r2r-0.1.29/r2r/examples/data/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/examples/pdf_chat/run_client.py` & `r2r-0.1.29/r2r/examples/clients/run_basic_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,18 @@
         self.titles = {
             "meditations.pdf": "Title: Meditations - Marcus Aurelius",
             # uncomment the following line to add more documents
             # "the_republic.pdf": "Title: The Republic - Plato",
         }
 
     def ingest(self):
-        current_dir = os.path.dirname(os.path.abspath(__file__))
-        for file_path in glob.glob(os.path.join(current_dir, "*.pdf")):
+        current_file_directory = os.path.dirname(os.path.abspath(__file__))
+        data_path = os.path.join(current_file_directory, "..", "data")
+
+        for file_path in glob.glob(os.path.join(data_path, "*.pdf")):
             file_name = file_path.split(os.path.sep)[-1]
             if file_name in self.titles:
                 document_id = generate_id_from_label(file_path)
                 metadata = {
                     "user_id": self.user_id,
                     "chunk_prefix": self.titles[file_name],
                 }
@@ -70,10 +72,20 @@
         asyncio.run(stream_rag_completion())
 
     def delete_document(self, document_path: str):
         document_id = generate_id_from_label(document_path)
         response = self.client.filtered_deletion("document_id", document_id)
         print("Deletion response = ", response)
 
+    def get_logs(self):
+        print("Fetching logs after all steps...")
+        logs_response = self.client.get_logs()
+        print(f"Logs response:\n{logs_response}\n")
+
+    def get_logs_summary(self):
+        print("Fetching logs summary after all steps...")
+        logs_summary_response = self.client.get_logs_summary()
+        print(f"Logs summary response:\n{logs_summary_response}\n")
+
 
 if __name__ == "__main__":
     fire.Fire(PDFChat)
```

### Comparing `r2r-0.1.28/r2r/integrations/ionic.py` & `r2r-0.1.29/r2r/integrations/ionic.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/integrations/serper.py` & `r2r-0.1.29/r2r/integrations/serper.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,16 @@
         payload = json.dumps({"q": query, "num": limit})
         connection.request("POST", "/search", payload, self.headers)
         response = connection.getresponse()
         data = response.read()
         json_data = json.loads(data.decode("utf-8"))
         return SerperClient._extract_results(json_data)
 
-    def construct_context(self, results: list) -> str:
+    @staticmethod
+    def construct_context(results: list) -> str:
         # Organize results by type
         organized_results = {}
         for result in results:
             result_type = result.pop(
                 "type", "Unknown"
             )  # Pop the type and use as key
             if result_type not in organized_results:
```

### Comparing `r2r-0.1.28/r2r/llms/litellm/base.py` & `r2r-0.1.29/r2r/llms/litellm/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/llms/openai/base.py` & `r2r-0.1.29/r2r/llms/openai/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A module for creating OpenAI model abstractions."""
+
 import logging
 import os
 from dataclasses import dataclass
 from typing import Union
 
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
```

### Comparing `r2r-0.1.28/r2r/main/app.py` & `r2r-0.1.29/r2r/main/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,17 @@
     EvalPipeline,
     GenerationConfig,
     IngestionPipeline,
     LoggingDatabaseConnection,
     RAGPipeline,
     RAGPipelineOutput,
 )
-from r2r.main.utils import (
+from r2r.main.utils import (  # configure_logging,
     R2RConfig,
     apply_cors,
-    configure_logging,
     find_project_root,
     process_logs,
 )
 
 from .models import (
     AddEntriesRequest,
     AddEntryRequest,
@@ -56,14 +55,16 @@
     eval_pipeline: EvalPipeline,
     rag_pipeline: RAGPipeline,
     config: R2RConfig,
     upload_path: Optional[Path] = None,
     logging_connection: Optional[LoggingDatabaseConnection] = None,
 ):
     app = FastAPI()
+    # TODO - Consider impact of logging in remote environments
+    # e.g. such as Google Cloud Run
     # configure_logging()
     apply_cors(app)
 
     upload_path = upload_path or find_project_root(CURRENT_DIR) / "uploads"
 
     if not upload_path.exists():
         upload_path.mkdir()
@@ -79,19 +80,19 @@
     ):
         metadata_json = json.loads(metadata)
         settings_model = SettingsModel.parse_raw(settings)
 
         if (
             file is not None
             and file.size
-            > config.app.get("max_file_size_in_mb", 10) * MB_CONVERSION_FACTOR
+            > config.app.get("max_file_size_in_mb", 100) * MB_CONVERSION_FACTOR
         ):
             raise HTTPException(
                 status_code=413,
-                detail="File size exceeds maximum allowed size of 10 MB.",
+                detail="File size exceeds maximum allowed size.",
             )
 
         if not file.filename:
             raise HTTPException(
                 status_code=400, detail="No file was uploaded."
             )
         # Extract file extension and check if it's an allowed type
```

### Comparing `r2r-0.1.28/r2r/main/factory.py` & `r2r-0.1.29/r2r/main/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import logging
 from typing import Any
 
 import dotenv
 
 from r2r.core import LoggingDatabaseConnection
 from r2r.core.utils import RecursiveCharacterTextSplitter
-from r2r.llms import LiteLLM, LiteLLMConfig, OpenAIConfig, OpenAILLM
+from r2r.llms import (
+    LiteLLM,
+    LiteLLMConfig,
+    LlamaCPP,
+    LlamaCppConfig,
+    OpenAIConfig,
+    OpenAILLM,
+)
 from r2r.pipelines import (
     BasicEmbeddingPipeline,
     BasicEvalPipeline,
     BasicIngestionPipeline,
     BasicRAGPipeline,
 )
 
@@ -50,14 +57,21 @@
 
     @staticmethod
     def get_llm(llm_config: dict[str, Any]):
         if llm_config["provider"] == "openai":
             return OpenAILLM(OpenAIConfig())
         elif llm_config["provider"] == "litellm":
             return LiteLLM(LiteLLMConfig())
+        elif llm_config["provider"] == "llamacpp":
+            return LlamaCPP(
+                LlamaCppConfig(
+                    llm_config.get("model_path", ""),
+                    llm_config.get("model_name", ""),
+                )
+            )
 
     @staticmethod
     def get_text_splitter(text_splitter_config: dict[str, Any]):
         if text_splitter_config["type"] != "recursive_character":
             raise ValueError(
                 "Only recursive character text splitter is supported"
             )
```

### Comparing `r2r-0.1.28/r2r/main/models.py` & `r2r-0.1.29/r2r/main/models.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/main/utils.py` & `r2r-0.1.29/r2r/main/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,17 +264,19 @@
             "method": "",
             "search_query": "",
             "search_results": [],
             "eval_results": None,
             "embedding_chunks": None,
             "document": None,
             "completion_result": "N/A",
-            "outcome": "success"
-            if aggregation["events"][-1].get("log_level") == "INFO"
-            else "fail",
+            "outcome": (
+                "success"
+                if aggregation["events"][-1].get("log_level") == "INFO"
+                else "fail"
+            ),
         }
 
         for event in aggregation["events"]:
             new_event = process_event(event, pipeline_type)
             if summary_entry["embedding_chunks"]:
                 new_event["embedding_chunks"] = summary_entry[
                     "embedding_chunks"
```

### Comparing `r2r-0.1.28/r2r/pipelines/__init__.py` & `r2r-0.1.29/r2r/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/pipelines/basic/embedding.py` & `r2r-0.1.29/r2r/pipelines/basic/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A simple example to demonstrate the usage of `BasicEmbeddingPipeline`.
 """
+
 import copy
 import logging
-import uuid
 from typing import Any, Optional, Tuple
 
 from r2r.core import (
     BasicDocument,
     EmbeddingPipeline,
     LoggingDatabaseConnection,
     VectorDBProvider,
```

### Comparing `r2r-0.1.28/r2r/pipelines/basic/eval.py` & `r2r-0.1.29/r2r/pipelines/basic/eval.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,12 +28,27 @@
         if provider == "deepeval":
             try:
                 from r2r.eval import DeepEvalProvider
             except ImportError:
                 raise ImportError(
                     "DeepEval is not installed. Please install it using `pip install deepeval`."
                 )
-            self.eval_provider = DeepEvalProvider()
+            self.eval_provider = DeepEvalProvider(
+                provider,
+                eval_config.get("sampling_fraction", 1.0),
+            )
+
+        elif provider == "parea":
+            try:
+                from r2r.eval import PareaEvalProvider
+            except ImportError:
+                raise ImportError(
+                    "Parea is not installed. Please install it using `pip install parea`."
+                )
+            self.eval_provider = PareaEvalProvider(
+                provider,
+                eval_config.get("sampling_fraction", 1.0),
+            )
 
     @log_execution_to_db
     def evaluate(self, query: str, context: str, completion: str) -> Any:
         return self.eval_provider.evaluate(query, context, completion)
```

### Comparing `r2r-0.1.28/r2r/pipelines/basic/ingestion.py` & `r2r-0.1.29/r2r/pipelines/basic/ingestion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A simple example to demonstrate the usage of `BasicIngestionPipeline`.
 """
+
 import logging
 from enum import Enum
 from typing import Any, Iterator, Optional, Union
 
 from r2r.core import (
     BasicDocument,
     IngestionPipeline,
```

### Comparing `r2r-0.1.28/r2r/pipelines/basic/prompt_provider.py` & `r2r-0.1.29/r2r/pipelines/basic/prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/pipelines/basic/rag.py` & `r2r-0.1.29/r2r/pipelines/basic/rag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A simple example to demonstrate the usage of `BasicRAGPipeline`.
 """
+
 import logging
 from typing import Optional
 
 from r2r.core import (
     LLMProvider,
     LoggingDatabaseConnection,
     PromptProvider,
```

### Comparing `r2r-0.1.28/r2r/pipelines/web_search/rag.py` & `r2r-0.1.29/r2r/pipelines/web_search/rag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A simple example to demonstrate the usage of `WebSearchRAGPipeline`.
 """
+
 import logging
 from typing import Optional
 
 from r2r.core import (
     LLMProvider,
     LoggingDatabaseConnection,
     PromptProvider,
```

### Comparing `r2r-0.1.28/r2r/tests/end_to_end.py` & `r2r-0.1.29/r2r/tests/end_to_end.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/tests/test.pdf` & `r2r-0.1.29/r2r/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/vecs/__init__.py` & `r2r-0.1.29/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/vecs/adapter/base.py` & `r2r-0.1.29/r2r/vecs/adapter/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/vecs/adapter/markdown.py` & `r2r-0.1.29/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/vecs/adapter/noop.py` & `r2r-0.1.29/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/vecs/adapter/text.py` & `r2r-0.1.29/r2r/vecs/adapter/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The `vecs.experimental.adapter.text` module provides adapter steps specifically designed for
 handling text data. It provides two main classes, `TextEmbedding` and `ParagraphChunker`.
 
 All public classes, enums, and functions are re-exported by `vecs.adapters` module.
 """
+
 from typing import Any, Dict, Generator, Iterable, Literal, Optional, Tuple
 
 from flupy import flu
 from vecs.exc import MissingDependency
 
 from .base import AdapterContext, AdapterStep
```

### Comparing `r2r-0.1.28/r2r/vecs/client.py` & `r2r-0.1.29/r2r/vecs/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 
 Importing from the `vecs.client` directly is not supported.
 All public classes, enums, and functions are re-exported by the top level `vecs` module.
 """
 
 from __future__ import annotations
 
+import logging
+import time
 from typing import TYPE_CHECKING, List, Optional
 
 from deprecated import deprecated
 from sqlalchemy import MetaData, create_engine, text
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.pool import QueuePool
 
 from r2r.vecs.adapter import Adapter
 from r2r.vecs.exc import CollectionNotFound
 
 if TYPE_CHECKING:
     from r2r.vecs.collection import Collection
 
+logger = logging.getLogger(__name__)
+
 
 class Client:
     """
     The `vecs.Client` class serves as an interface to a PostgreSQL database with pgvector support. It facilitates
     the creation, retrieval, listing and deletion of vector collections, while managing connections to the
     database.
 
@@ -44,42 +48,88 @@
         # OR
 
         vx = vecs.create_client(DB_CONNECTION)
         # do some work
         vx.disconnect()
     """
 
-    def __init__(self, connection_string: str, pool_size=1, *args, **kwargs):
-        """
-        Initialize a Client instance.
-
-        Args:
-            connection_string (str): A string representing the database connection information.
-
-        Returns:
-            None
-        """
+    def __init__(
+        self,
+        connection_string: str,
+        pool_size: int = 1,
+        max_retries: int = 3,
+        retry_delay: int = 1,
+    ):
         self.engine = create_engine(
             connection_string,
             pool_size=pool_size,
             poolclass=QueuePool,
             pool_recycle=300,  # Recycle connections after 5 min
         )
         self.meta = MetaData(schema="vecs")
         self.Session = sessionmaker(self.engine)
+        self.max_retries = max_retries
+        self.retry_delay = retry_delay
+        self.vector_version: Optional[str] = None
+        self._initialize_database()
+
+    def _initialize_database(self):
+        retries = 0
+        while retries < self.max_retries:
+            try:
+                with self.Session() as sess:
+                    with sess.begin():
+                        self._create_schema(sess)
+                        self._create_extension(sess)
+                        self._get_vector_version(sess)
+                return
+            except Exception as e:
+                logger.warning(
+                    f"Database connection error: {str(e)}. Retrying in {self.retry_delay} seconds..."
+                )
+                retries += 1
+                time.sleep(self.retry_delay)
 
-        with self.Session() as sess:
-            with sess.begin():
-                sess.execute(text("create schema if not exists vecs;"))
-                sess.execute(text("create extension if not exists vector;"))
-                self.vector_version: str = sess.execute(
+        logger.error(
+            f"Failed to initialize database after {self.max_retries} retries."
+        )
+        raise RuntimeError("Failed to initialize database.")
+
+    def _create_schema(self, sess):
+        try:
+            sess.execute(text("CREATE SCHEMA IF NOT EXISTS vecs;"))
+        except Exception as e:
+            logger.warning(f"Failed to create schema: {str(e)}")
+
+    def _create_extension(self, sess):
+        try:
+            sess.execute(text("CREATE EXTENSION IF NOT EXISTS vector;"))
+        except Exception as e:
+            logger.warning(f"Failed to create extension: {str(e)}")
+
+    def _get_vector_version(self, sess):
+        try:
+            self.vector_version = sess.execute(
+                text(
+                    "SELECT installed_version FROM pg_available_extensions WHERE name = 'vector' LIMIT 1;"
+                )
+            ).scalar_one()
+        except sqlalchemy.exc.InternalError as e:
+            if isinstance(e.orig, psycopg2.errors.InFailedSqlTransaction):
+                sess.rollback()
+                self.vector_version = sess.execute(
                     text(
-                        "select installed_version from pg_available_extensions where name = 'vector' limit 1;"
+                        "SELECT installed_version FROM pg_available_extensions WHERE name = 'vector' LIMIT 1;"
                     )
                 ).scalar_one()
+            else:
+                raise e
+        except Exception as e:
+            logger.error(f"Failed to retrieve vector version: {str(e)}")
+            raise e
 
     def _supports_hnsw(self):
         return (
             not self.vector_version.startswith("0.4")
             and not self.vector_version.startswith("0.3")
             and not self.vector_version.startswith("0.2")
             and not self.vector_version.startswith("0.1")
@@ -222,14 +272,15 @@
         """
         Disconnect the client from the database.
 
         Returns:
             None
         """
         self.engine.dispose()
+        logger.info("Disconnected from the database.")
         return
 
     def __enter__(self) -> "Client":
         """
         Enable use of the 'with' statement.
 
         Returns:
```

### Comparing `r2r-0.1.28/r2r/vecs/collection.py` & `r2r-0.1.29/r2r/vecs/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Defines the 'Collection' class
 
 Importing from the `vecs.collection` directly is not supported.
 All public classes, enums, and functions are re-exported by the top level `vecs` module.
 """
+
 from __future__ import annotations
 
 import math
 import uuid
 import warnings
 from dataclasses import dataclass
 from enum import Enum
```

### Comparing `r2r-0.1.28/r2r/vecs/exc.py` & `r2r-0.1.29/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/vector_dbs/local/base.py` & `r2r-0.1.29/r2r/vector_dbs/local/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/vector_dbs/pg_vector/base.py` & `r2r-0.1.29/r2r/vector_dbs/pg_vector/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/r2r/vector_dbs/qdrant/base.py` & `r2r-0.1.29/r2r/vector_dbs/qdrant/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.28/PKG-INFO` & `r2r-0.1.29/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,207 +1,188 @@
 Metadata-Version: 2.1
 Name: r2r
-Version: 0.1.28
+Version: 0.1.29
 Summary: SciPhi R2R
 License: MIT
 Author: Owen Colegrove
 Author-email: owen@sciphi.ai
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
+Provides-Extra: deepeval
 Provides-Extra: embedding
 Provides-Extra: eval
+Provides-Extra: exa
 Provides-Extra: ionic
-Provides-Extra: local-vectordb
+Provides-Extra: local-llm
 Provides-Extra: monitoring
 Provides-Extra: parsing
 Provides-Extra: postgres
 Provides-Extra: qdrant
 Provides-Extra: reducto
 Provides-Extra: streaming
-Requires-Dist: boto3 (>=1.34.71,<2.0.0) ; extra == "reducto"
+Requires-Dist: boto3 (>=1.34.71,<2.0.0) ; extra == "reducto" or extra == "all"
 Requires-Dist: bs4 (>=0.0.2,<0.0.3) ; extra == "parsing" or extra == "all"
 Requires-Dist: datasets (>=2.16.1,<3.0.0) ; extra == "streaming" or extra == "all"
-Requires-Dist: deepeval (>=0.20.88,<0.21.0) ; extra == "eval" or extra == "all"
+Requires-Dist: deepeval (>=0.20.88,<0.21.0) ; extra == "deepeval"
+Requires-Dist: exa-py (>=1.0.9,<2.0.0) ; extra == "exa" or extra == "all"
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gunicorn (>=21.2.0,<22.0.0)
 Requires-Dist: ionic-api-sdk (==0.9.3) ; extra == "ionic"
-Requires-Dist: litellm (>=1.28.0,<2.0.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0) ; extra == "local-vectordb" or extra == "all"
+Requires-Dist: litellm (>=1.34.0,<2.0.0)
+Requires-Dist: llama-cpp-python (>=0.2.57,<0.3.0) ; extra == "local-llm" or extra == "all"
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: openai (>=1.11.1,<2.0.0)
 Requires-Dist: parea-ai (>=0.2.86,<0.3.0) ; extra == "eval" or extra == "all"
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ; extra == "postgres" or extra == "all"
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pypdf (>=4.0.2,<5.0.0) ; extra == "parsing" or extra == "all"
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: qdrant_client (>=1.7.0,<2.0.0) ; extra == "qdrant" or extra == "all"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0) ; extra == "local-vectordb" or extra == "all"
+Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0) ; extra == "local-llm"
 Requires-Dist: sentry-sdk (>=1.40.4,<2.0.0) ; extra == "monitoring" or extra == "all"
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra == "embedding" or extra == "all"
 Requires-Dist: types-requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.27.0.post1,<0.28.0)
 Requires-Dist: vecs (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
-# R2R: Production-ready RAG systems.
-
 <p align="left">
   <a href="https://r2r-docs.sciphi.ai"><img src="https://img.shields.io/badge/docs.sciphi.ai-3F16E4" alt="Docs"></a>
   <a href="https://discord.gg/p6KqD2kjtB"><img src="https://img.shields.io/discord/1120774652915105934?style=social&logo=discord" alt="Discord"></a>
   <a href="https://github.com/SciPhi-AI"><img src="https://img.shields.io/github/stars/SciPhi-AI/R2R" alt="Github Stars"></a>
   <a href="https://github.com/SciPhi-AI/R2R/pulse"><img src="https://img.shields.io/github/commit-activity/w/SciPhi-AI/R2R" alt="Commits-per-week"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-purple.svg" alt="License: MIT"></a>
 </p>
 
-A semi-opinionated RAG framework.
-
 <img src="./docs/pages/r2r.png" alt="Sciphi Framework">
-R2R was conceived to bridge the gap between experimental RAG models and robust, production-ready systems. Our semi-opinionated framework cuts through the complexity, offering a straightforward path to deploy, adapt, and maintain RAG pipelines in production. We prioritize simplicity and practicality, aiming to set a new industry benchmark for ease of use and effectiveness.
+<h3 align="center">
+Build, deploy, and optimize your RAG system.
+</h3>
+
+## About
+
+R2R, short for RAG to Riches, provides the fastest and most efficient way to provide high quality RAG to end users. The framework is built around customizable pipelines and a feature-rich FastAPI implementation.
+
+## Why?
+
+R2R was conceived to bridge the gap between local LLM experimentation and scalable production solutions. **R2R is to LangChain/LlamaIndex what NextJS is to React**. A JavaScript client for R2R deployments can be [found here](https://github.com/SciPhi-AI/r2r-js).
+
+### Key Features
+
+- **🚀 Deploy**: Instantly launch production-ready RAG pipelines with streaming capabilities.
+- **🧩 Customize**: Tailor your pipeline with intuitive configuration files.
+- **🔌 Extend**: Enhance your pipeline with custom code integrations.
+- **⚖️ Autoscale**: Scale your pipeline effortlessly in the cloud using [SciPhi](https://app.sciphi.ai/).
+- **🤖 OSS**: Benefit from a framework developed by the open-source community, designed to simplify RAG deployment.
 
 ## Demo(s)
 
-Using cloud application to deploy the pre-built basic pipeline:
+Using the cloud application to deploy the pre-built basic pipeline:
+
 https://www.loom.com/share/e3b934b554484787b005702ced650ac9
 
-!! Note - The server has been removed from this repo - instead we now recommend using [SciPhi Cloud](https://app.sciphi.ai) to pair with the R2R framework for observability and optimization.
+Note - the example above uses [SciPhi Cloud](https://app.sciphi.ai) to pair with the R2R framework for deployment and observability. SciPhi is working to launch a self-hosted version of their cloud platform as R2R matures.
 
-### Quick Install:
+## Links
+
+[Join the Discord server](https://discord.gg/p6KqD2kjtB)
+
+[R2R Docs Quickstart](https://r2r-docs.sciphi.ai/getting-started/quick-install)
+
+[SciPhi Cloud](https://docs.sciphi.ai/)
 
-**Install R2R directly using `pip`:**
+## Quick Install:
 
 ```bash
 # use the `'r2r[all]'` to download all required deps
 pip install 'r2r[parsing,eval]'
 
 # setup env 
 export OPENAI_API_KEY=sk-...
+# Set `LOCAL_DB_PATH` for local testing
 export LOCAL_DB_PATH=local.sqlite
 
 # OR do `vim .env.example && cp .env.example .env`
 # INCLUDE secrets and modify config.json
-# if using cloud providers (e.g. pgvector, supabase, ...)
+# if using cloud providers (e.g. pgvector, qdrant, ...)
 ```
 
-### Run the server with Docker:
+## Docker:
 
 ```bash
 docker pull emrgntcmplxty/r2r:latest
 
-# Place your secrets in `.env` before deploying
+# Place your secrets in `.env`
 docker run -d --name r2r_container -p 8000:8000 --env-file .env r2r
 ```
 
-## Links
-
-[Join the Discord server](https://discord.gg/p6KqD2kjtB)
-
-[Read the R2R Docs](https://r2r-docs.sciphi.ai/)
+## Basic Example
 
-## Basic Examples
-
-The project includes several basic examples that demonstrate application deployment and interaction:
-
-1. [`basic app`](r2r/examples/basic/app.py): This example runs the backend server, which includes the ingestion, embedding, and RAG pipelines served via FastAPI.
+[`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the default **backend server**. It establishes a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes, all accessible via FastAPI.
 
    ```bash
-   # If using a venv, replace `uvicorn` with `venv_path/bin/uvicorn`
-   uvicorn r2r.examples.basic.app:app
+   # launch the server
+   python -m r2r.examples.servers.basic_pipeline
    ```
 
-2. [`basic client`](r2r/examples/basic/run_client.py): This example should be run after starting the server. It demonstrates uploading text entries as well as a PDF to the local server with the python client. Further, it shows document and user-level vector management with built-in features.
+[`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This **client script** should be executed subsequent to the server startup above. It facilitates the upload of text entries and PDFs to the server using the Python client and demonstrates the management of document and user-level vectors through its built-in features.
 
    ```bash
-   python -m r2r.examples.basic.run_client
+   # run the client
+   python -m r2r.examples.clients.run_basic_client
    ```
 
-3. [`academy`](r2r/examples/academy): A more sophisticated demo demonstrating how to build a more novel pipeline which involves synthetic queries
+## Synthetic Queries Example
 
-   ```bash
-   # Launch the `academy` example application
-   # If using a venv, replace `uvicorn` with `venv_path/bin/uvicorn`
-   uvicorn r2r.examples.academy.app:app
+[`synthetic_query_pipeline.py`](r2r/examples/servers/synthetic_query_pipeline.py): Execute this script to start a backend server equipped with an advanced pipeline. This pipeline is designed to create synthetic queries, enhancing the RAG system's learning and performance.
 
-   # Ask a question
-   python -m r2r.examples.academy.run_client search "What are the key themes of Meditations?"
+   ```bash
+   # launch the server
+   python -m r2r.examples.servers.synthetic_query_pipeline
    ```
-4. [`end-to-end`](docs/pages/examples/end-to-end.mdx): An example showing how to combine a complete web application with the basic RAG pipeline above.
-
-5. [`intelligence`](app.sciphi.ai): A cloud platform which can be used to deploy R2R pipelines powered by SciPhi
-
-
-
-### Full Install:
-
-Follow these steps to ensure a smooth setup:
 
-1. **Install Poetry:**
+[`run_synthetic_query_client.py`](r2r/examples/clients/run_synthetic_query_client.py): Use this client script after the synthetic query pipeline is running. It's tailored for use with the synthetic query pipeline, demonstrating the improved features of the RAG system.
 
-   - Before installing the project, make sure you have Poetry on your system. If not, visit the [official Poetry website](https://python-poetry.org/docs/#installation) for installation instructions.
-
-2. **Clone and Install Dependencies:**
-
-  - Clone the project repository and navigate to the project directory:
-     
-     ```bash
-     git clone git@github.com:SciPhi-AI/r2r.git
-     cd r2r
-     ```
-     
-  - Copy the `.env.example` file to `.env`. This file is in the main project folder:
+   ```bash
+   # run the client
+   python -m r2r.examples.clients.run_synthetic_query_client
+   ```
 
-     ```bash
-     cp .env.example .env
+## Extras Examples
 
-     # Add secrets, `OPENAI_API_KEY` at a minimum
-     vim .env
-     ```
-     
-  - Install the project dependencies with Poetry:
-  
-     ```bash
-     # See pyproject.toml for available extras
-     # use "all" to include every optional dependency
-     poetry install -E parsing -E eval
-     ```
-     
-  - Execute with poetry run:
-     
-     ```bash
-     python -m r2r.examples.pdf_chat.run_client ingest
-     ```
+[`reducto_pipeline.py`](r2r/examples/servers/reducto_pipeline.py): Launch this script to activate a backend server that integrates a Reducto adapter for enhanced PDF ingestion.
 
-3. **Configure Environment Variables:**
-   - You need to set up cloud provider secrets in your `.env`. At a minimum, you will need an OpenAI key.
-   - The framework currently supports PostgreSQL (locally), pgvector and Qdrant with plans to extend coverage.
+   ```bash
+   # launch the server
+   python -m r2r.examples.servers.reducto_pipeline
+   ```
 
-## Key Features
+[`web_search_pipeline.py`](r2r/examples/servers/web_search_pipeline.py): This script sets up a backend server that includes a `WebSearchRAGPipeline`, adding web search functionality to your RAG setup.
 
-- **🚀 Rapid Deployment**: Facilitates a smooth setup and development of production-ready RAG systems.
-- **⚖️ Flexible Standardization**: `Ingestion`, `Embedding`, and `RAG` with proper `Observability`.
-- **🧩 Easy to modify**: Provides a structure that can be extended to deploy your own custom pipelines.
-- **📦 Versioning**: Ensures your work remains reproducible and traceable through version control.
-- **🔌 Extensibility**: Enables a quick and robust integration with various VectorDBs, LLMs and Embeddings Models.
-- **🤖 OSS Driven**: Built for and by the OSS community, to help startups and enterprises to quickly build with RAG.
-- **📝 Deployment Support**: Available to help you build and deploy your RAG systems end-to-end.
+   ```bash
+   # launch the server
+   python -m r2r.examples.servers.web_search_pipeline
+   ```
 
 ## Core Abstractions
 
 The framework primarily revolves around three core abstractions:
 
-- The **Ingestion Pipeline**: Facilitates the preparation of embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.). The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/ingestion.py).
+- The **Ingestion Pipeline**: Facilitates the preparation of embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.). The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/ingestion).
 
-- The **Embedding Pipeline**: Manages the transformation of text into stored vector embeddings, interacting with embedding and vector database providers through a series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks, etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/embedding.py).
+- The **Embedding Pipeline**: Manages the transformation of text into stored vector embeddings, interacting with embedding and vector database providers through a series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks, etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/embedding.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/embedding).
 
-- The **RAG Pipeline**: Works similarly to the embedding pipeline but incorporates an LLM provider to produce text completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/rag.py).
+- The **RAG Pipeline**: Works similarly to the embedding pipeline but incorporates an LLM provider to produce text completions. The abstraction can be found in [`rag.py`](r2r/core/pipelines/rag.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/rag).
 
-- The **Eval Pipeline**: Samples some subset of rag_completion calls for evaluation. Currently [DeepEval](https://github.com/confident-ai/deepeval) is supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/eval.py).
+- The **Eval Pipeline**: Samples some subset of rag_completion calls for evaluation. Currently [DeepEval](https://github.com/confident-ai/deepeval) is supported. The abstraction can be found in [`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available [here](https://r2r-docs.sciphi.ai/core-features/eval).
 
 Each pipeline incorporates a logging database for operation tracking and observability.
```

#### html2text {}

```diff
@@ -1,112 +1,112 @@
-Metadata-Version: 2.1 Name: r2r Version: 0.1.28 Summary: SciPhi R2R License:
+Metadata-Version: 2.1 Name: r2r Version: 0.1.29 Summary: SciPhi R2R License:
 MIT Author: Owen Colegrove Author-email: owen@sciphi.ai Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Provides-Extra: all Provides-Extra: embedding Provides-Extra:
-eval Provides-Extra: ionic Provides-Extra: local-vectordb Provides-Extra:
-monitoring Provides-Extra: parsing Provides-Extra: postgres Provides-Extra:
-qdrant Provides-Extra: reducto Provides-Extra: streaming Requires-Dist: boto3
-(>=1.34.71,<2.0.0) ; extra == "reducto" Requires-Dist: bs4 (>=0.0.2,<0.0.3) ;
-extra == "parsing" or extra == "all" Requires-Dist: datasets (>=2.16.1,<3.0.0)
-; extra == "streaming" or extra == "all" Requires-Dist: deepeval
-(>=0.20.88,<0.21.0) ; extra == "eval" or extra == "all" Requires-Dist: fastapi
-(>=0.109.2,<0.110.0) Requires-Dist: fire (>=0.5.0,<0.6.0) Requires-Dist:
-gunicorn (>=21.2.0,<22.0.0) Requires-Dist: ionic-api-sdk (==0.9.3) ; extra ==
-"ionic" Requires-Dist: litellm (>=1.28.0,<2.0.0) Requires-Dist: numpy
-(>=1.26.4,<2.0.0) ; extra == "local-vectordb" or extra == "all" Requires-Dist:
-openai (>=1.11.1,<2.0.0) Requires-Dist: parea-ai (>=0.2.86,<0.3.0) ; extra ==
-"eval" or extra == "all" Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ;
-extra == "postgres" or extra == "all" Requires-Dist: pydantic (>=2.6.3,<3.0.0)
-Requires-Dist: pypdf (>=4.0.2,<5.0.0) ; extra == "parsing" or extra == "all"
-Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-multipart
-(>=0.0.9,<0.0.10) Requires-Dist: qdrant_client (>=1.7.0,<2.0.0) ; extra ==
-"qdrant" or extra == "all" Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
-Dist: scikit-learn (>=1.4.1.post1,<2.0.0) ; extra == "local-vectordb" or extra
-== "all" Requires-Dist: sentry-sdk (>=1.40.4,<2.0.0) ; extra == "monitoring" or
-extra == "all" Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra == "embedding"
-or extra == "all" Requires-Dist: types-requests (>=2.31.0,<3.0.0) Requires-
-Dist: uvicorn (>=0.27.0.post1,<0.28.0) Requires-Dist: vecs (>=0.4.0,<0.5.0)
-Description-Content-Type: text/markdown # R2R: Production-ready RAG systems.
+Python :: 3.12 Provides-Extra: all Provides-Extra: deepeval Provides-Extra:
+embedding Provides-Extra: eval Provides-Extra: exa Provides-Extra: ionic
+Provides-Extra: local-llm Provides-Extra: monitoring Provides-Extra: parsing
+Provides-Extra: postgres Provides-Extra: qdrant Provides-Extra: reducto
+Provides-Extra: streaming Requires-Dist: boto3 (>=1.34.71,<2.0.0) ; extra ==
+"reducto" or extra == "all" Requires-Dist: bs4 (>=0.0.2,<0.0.3) ; extra ==
+"parsing" or extra == "all" Requires-Dist: datasets (>=2.16.1,<3.0.0) ; extra
+== "streaming" or extra == "all" Requires-Dist: deepeval (>=0.20.88,<0.21.0) ;
+extra == "deepeval" Requires-Dist: exa-py (>=1.0.9,<2.0.0) ; extra == "exa" or
+extra == "all" Requires-Dist: fastapi (>=0.109.2,<0.110.0) Requires-Dist: fire
+(>=0.5.0,<0.6.0) Requires-Dist: gunicorn (>=21.2.0,<22.0.0) Requires-Dist:
+ionic-api-sdk (==0.9.3) ; extra == "ionic" Requires-Dist: litellm
+(>=1.34.0,<2.0.0) Requires-Dist: llama-cpp-python (>=0.2.57,<0.3.0) ; extra ==
+"local-llm" or extra == "all" Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-
+Dist: openai (>=1.11.1,<2.0.0) Requires-Dist: parea-ai (>=0.2.86,<0.3.0) ;
+extra == "eval" or extra == "all" Requires-Dist: psycopg2-binary
+(>=2.9.9,<3.0.0) ; extra == "postgres" or extra == "all" Requires-Dist:
+pydantic (>=2.6.3,<3.0.0) Requires-Dist: pypdf (>=4.0.2,<5.0.0) ; extra ==
+"parsing" or extra == "all" Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: python-multipart (>=0.0.9,<0.0.10) Requires-Dist: qdrant_client
+(>=1.7.0,<2.0.0) ; extra == "qdrant" or extra == "all" Requires-Dist: requests
+(>=2.31.0,<3.0.0) Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0) ; extra
+== "local-llm" Requires-Dist: sentry-sdk (>=1.40.4,<2.0.0) ; extra ==
+"monitoring" or extra == "all" Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra
+== "embedding" or extra == "all" Requires-Dist: types-requests
+(>=2.31.0,<3.0.0) Requires-Dist: uvicorn (>=0.27.0.post1,<0.28.0) Requires-
+Dist: vecs (>=0.4.0,<0.5.0) Description-Content-Type: text/markdown
 _[_D_o_c_s_]_[_D_i_s_c_o_r_d_]_[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
-A semi-opinionated RAG framework. [Sciphi Framework]R2R was conceived to bridge
-the gap between experimental RAG models and robust, production-ready systems.
-Our semi-opinionated framework cuts through the complexity, offering a
-straightforward path to deploy, adapt, and maintain RAG pipelines in
-production. We prioritize simplicity and practicality, aiming to set a new
-industry benchmark for ease of use and effectiveness. ## Demo(s) Using cloud
-application to deploy the pre-built basic pipeline: https://www.loom.com/share/
-e3b934b554484787b005702ced650ac9 !! Note - The server has been removed from
-this repo - instead we now recommend using [SciPhi Cloud](https://
-app.sciphi.ai) to pair with the R2R framework for observability and
-optimization. ### Quick Install: **Install R2R directly using `pip`:** ```bash
-# use the `'r2r[all]'` to download all required deps pip install 'r2r
-[parsing,eval]' # setup env export OPENAI_API_KEY=sk-... export
+[Sciphi Framework]
+            ******** BBuuiilldd,, ddeeppllooyy,, aanndd ooppttiimmiizzee yyoouurr RRAAGG ssyysstteemm.. ********
+## About R2R, short for RAG to Riches, provides the fastest and most efficient
+way to provide high quality RAG to end users. The framework is built around
+customizable pipelines and a feature-rich FastAPI implementation. ## Why? R2R
+was conceived to bridge the gap between local LLM experimentation and scalable
+production solutions. **R2R is to LangChain/LlamaIndex what NextJS is to
+React**. A JavaScript client for R2R deployments can be [found here](https://
+github.com/SciPhi-AI/r2r-js). ### Key Features - **ð Deploy**: Instantly
+launch production-ready RAG pipelines with streaming capabilities. - **ð§©
+Customize**: Tailor your pipeline with intuitive configuration files. - **ð
+Extend**: Enhance your pipeline with custom code integrations. - **âï¸
+Autoscale**: Scale your pipeline effortlessly in the cloud using [SciPhi]
+(https://app.sciphi.ai/). - **ð¤ OSS**: Benefit from a framework developed by
+the open-source community, designed to simplify RAG deployment. ## Demo(s)
+Using the cloud application to deploy the pre-built basic pipeline: https://
+www.loom.com/share/e3b934b554484787b005702ced650ac9 Note - the example above
+uses [SciPhi Cloud](https://app.sciphi.ai) to pair with the R2R framework for
+deployment and observability. SciPhi is working to launch a self-hosted version
+of their cloud platform as R2R matures. ## Links [Join the Discord server]
+(https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart](https://r2r-
+docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud](https://
+docs.sciphi.ai/) ## Quick Install: ```bash # use the `'r2r[all]'` to download
+all required deps pip install 'r2r[parsing,eval]' # setup env export
+OPENAI_API_KEY=sk-... # Set `LOCAL_DB_PATH` for local testing export
 LOCAL_DB_PATH=local.sqlite # OR do `vim .env.example && cp .env.example .env` #
 INCLUDE secrets and modify config.json # if using cloud providers (e.g.
-pgvector, supabase, ...) ``` ### Run the server with Docker: ```bash docker
-pull emrgntcmplxty/r2r:latest # Place your secrets in `.env` before deploying
-docker run -d --name r2r_container -p 8000:8000 --env-file .env r2r ``` ##
-Links [Join the Discord server](https://discord.gg/p6KqD2kjtB) [Read the R2R
-Docs](https://r2r-docs.sciphi.ai/) ## Basic Examples The project includes
-several basic examples that demonstrate application deployment and interaction:
-1. [`basic app`](r2r/examples/basic/app.py): This example runs the backend
-server, which includes the ingestion, embedding, and RAG pipelines served via
-FastAPI. ```bash # If using a venv, replace `uvicorn` with `venv_path/bin/
-uvicorn` uvicorn r2r.examples.basic.app:app ``` 2. [`basic client`](r2r/
-examples/basic/run_client.py): This example should be run after starting the
-server. It demonstrates uploading text entries as well as a PDF to the local
-server with the python client. Further, it shows document and user-level vector
-management with built-in features. ```bash python -
-m r2r.examples.basic.run_client ``` 3. [`academy`](r2r/examples/academy): A
-more sophisticated demo demonstrating how to build a more novel pipeline which
-involves synthetic queries ```bash # Launch the `academy` example application #
-If using a venv, replace `uvicorn` with `venv_path/bin/uvicorn` uvicorn
-r2r.examples.academy.app:app # Ask a question python -
-m r2r.examples.academy.run_client search "What are the key themes of
-Meditations?" ``` 4. [`end-to-end`](docs/pages/examples/end-to-end.mdx): An
-example showing how to combine a complete web application with the basic RAG
-pipeline above. 5. [`intelligence`](app.sciphi.ai): A cloud platform which can
-be used to deploy R2R pipelines powered by SciPhi ### Full Install: Follow
-these steps to ensure a smooth setup: 1. **Install Poetry:** - Before
-installing the project, make sure you have Poetry on your system. If not, visit
-the [official Poetry website](https://python-poetry.org/docs/#installation) for
-installation instructions. 2. **Clone and Install Dependencies:** - Clone the
-project repository and navigate to the project directory: ```bash git clone
-git@github.com:SciPhi-AI/r2r.git cd r2r ``` - Copy the `.env.example` file to
-`.env`. This file is in the main project folder: ```bash cp .env.example .env #
-Add secrets, `OPENAI_API_KEY` at a minimum vim .env ``` - Install the project
-dependencies with Poetry: ```bash # See pyproject.toml for available extras #
-use "all" to include every optional dependency poetry install -E parsing -
-E eval ``` - Execute with poetry run: ```bash python -
-m r2r.examples.pdf_chat.run_client ingest ``` 3. **Configure Environment
-Variables:** - You need to set up cloud provider secrets in your `.env`. At a
-minimum, you will need an OpenAI key. - The framework currently supports
-PostgreSQL (locally), pgvector and Qdrant with plans to extend coverage. ## Key
-Features - **ð Rapid Deployment**: Facilitates a smooth setup and
-development of production-ready RAG systems. - **âï¸ Flexible
-Standardization**: `Ingestion`, `Embedding`, and `RAG` with proper
-`Observability`. - **ð§© Easy to modify**: Provides a structure that can be
-extended to deploy your own custom pipelines. - **ð¦ Versioning**: Ensures
-your work remains reproducible and traceable through version control. - **ð
-Extensibility**: Enables a quick and robust integration with various VectorDBs,
-LLMs and Embeddings Models. - **ð¤ OSS Driven**: Built for and by the OSS
-community, to help startups and enterprises to quickly build with RAG. - **ð
-Deployment Support**: Available to help you build and deploy your RAG systems
-end-to-end. ## Core Abstractions The framework primarily revolves around three
-core abstractions: - The **Ingestion Pipeline**: Facilitates the preparation of
-embeddable 'Documents' from various data formats (json, txt, pdf, html, etc.).
-The abstraction can be found in [`ingestion.py`](r2r/core/pipelines/
-ingestion.py). - The **Embedding Pipeline**: Manages the transformation of text
-into stored vector embeddings, interacting with embedding and vector database
-providers through a series of steps (e.g., extract_text, transform_text,
-chunk_text, embed_chunks, etc.). The abstraction can be found in
-[`embedding.py`](r2r/core/pipelines/embedding.py). - The **RAG Pipeline**:
-Works similarly to the embedding pipeline but incorporates an LLM provider to
-produce text completions. The abstraction can be found in [`rag.py`](r2r/core/
-pipelines/rag.py). - The **Eval Pipeline**: Samples some subset of
-rag_completion calls for evaluation. Currently [DeepEval](https://github.com/
-confident-ai/deepeval) is supported. The abstraction can be found in
-[`eval.py`](r2r/core/pipelines/eval.py). Each pipeline incorporates a logging
-database for operation tracking and observability.
+pgvector, qdrant, ...) ``` ## Docker: ```bash docker pull emrgntcmplxty/r2r:
+latest # Place your secrets in `.env` docker run -d --name r2r_container -
+p 8000:8000 --env-file .env r2r ``` ## Basic Example [`basic_pipeline.py`](r2r/
+examples/servers/basic_pipeline.py): Execute this script to initiate the
+default **backend server**. It establishes a basic RAG pipeline that
+encompasses ingestion, embedding, and RAG processes, all accessible via
+FastAPI. ```bash # launch the server python -
+m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
+clients/run_basic_client.py): This **client script** should be executed
+subsequent to the server startup above. It facilitates the upload of text
+entries and PDFs to the server using the Python client and demonstrates the
+management of document and user-level vectors through its built-in features.
+```bash # run the client python -m r2r.examples.clients.run_basic_client ``` ##
+Synthetic Queries Example [`synthetic_query_pipeline.py`](r2r/examples/servers/
+synthetic_query_pipeline.py): Execute this script to start a backend server
+equipped with an advanced pipeline. This pipeline is designed to create
+synthetic queries, enhancing the RAG system's learning and performance. ```bash
+# launch the server python -m r2r.examples.servers.synthetic_query_pipeline ```
+[`run_synthetic_query_client.py`](r2r/examples/clients/
+run_synthetic_query_client.py): Use this client script after the synthetic
+query pipeline is running. It's tailored for use with the synthetic query
+pipeline, demonstrating the improved features of the RAG system. ```bash # run
+the client python -m r2r.examples.clients.run_synthetic_query_client ``` ##
+Extras Examples [`reducto_pipeline.py`](r2r/examples/servers/
+reducto_pipeline.py): Launch this script to activate a backend server that
+integrates a Reducto adapter for enhanced PDF ingestion. ```bash # launch the
+server python -m r2r.examples.servers.reducto_pipeline ```
+[`web_search_pipeline.py`](r2r/examples/servers/web_search_pipeline.py): This
+script sets up a backend server that includes a `WebSearchRAGPipeline`, adding
+web search functionality to your RAG setup. ```bash # launch the server python
+-m r2r.examples.servers.web_search_pipeline ``` ## Core Abstractions The
+framework primarily revolves around three core abstractions: - The **Ingestion
+Pipeline**: Facilitates the preparation of embeddable 'Documents' from various
+data formats (json, txt, pdf, html, etc.). The abstraction can be found in
+[`ingestion.py`](r2r/core/pipelines/ingestion.py) and relevant documentation is
+available [here](https://r2r-docs.sciphi.ai/core-features/ingestion). - The
+**Embedding Pipeline**: Manages the transformation of text into stored vector
+embeddings, interacting with embedding and vector database providers through a
+series of steps (e.g., extract_text, transform_text, chunk_text, embed_chunks,
+etc.). The abstraction can be found in [`embedding.py`](r2r/core/pipelines/
+embedding.py) and relevant documentation is available [here](https://r2r-
+docs.sciphi.ai/core-features/embedding). - The **RAG Pipeline**: Works
+similarly to the embedding pipeline but incorporates an LLM provider to produce
+text completions. The abstraction can be found in [`rag.py`](r2r/core/
+pipelines/rag.py) and relevant documentation is available [here](https://r2r-
+docs.sciphi.ai/core-features/rag). - The **Eval Pipeline**: Samples some subset
+of rag_completion calls for evaluation. Currently [DeepEval](https://
+github.com/confident-ai/deepeval) is supported. The abstraction can be found in
+[`eval.py`](r2r/core/pipelines/eval.py) and relevant documentation is available
+[here](https://r2r-docs.sciphi.ai/core-features/eval). Each pipeline
+incorporates a logging database for operation tracking and observability.
```

