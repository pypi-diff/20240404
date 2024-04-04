# Comparing `tmp/sherpa_ai-0.1.1.tar.gz` & `tmp/sherpa_ai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa_ai-0.1.1.tar", max compression
+gzip compressed data, was "sherpa_ai-0.2.0.tar", max compression
```

## Comparing `sherpa_ai-0.1.1.tar` & `sherpa_ai-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,68 @@
--rw-r--r--   0        0        0     1086 2023-11-01 19:00:26.437685 sherpa_ai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-09-07 18:58:13.889346 sherpa_ai-0.1.1/README.md
--rw-r--r--   0        0        0       23 2023-09-07 18:58:13.896351 sherpa_ai-0.1.1/sherpa_ai/__init__.py
--rw-r--r--   0        0        0      203 2023-10-22 21:42:20.082581 sherpa_ai-0.1.1/sherpa_ai/action_planner/__init__.py
--rw-r--r--   0        0        0     3716 2023-10-26 19:09:34.163051 sherpa_ai-0.1.1/sherpa_ai/action_planner/action_planner.py
--rw-r--r--   0        0        0      310 2023-10-22 21:42:20.089584 sherpa_ai-0.1.1/sherpa_ai/action_planner/base.py
--rw-r--r--   0        0        0     1427 2023-10-27 03:52:01.976676 sherpa_ai-0.1.1/sherpa_ai/action_planner/selective_planner.py
--rw-r--r--   0        0        0       66 2023-10-22 21:42:20.092581 sherpa_ai-0.1.1/sherpa_ai/action_planner/simple_planner.py
--rw-r--r--   0        0        0      333 2023-10-22 21:42:20.094581 sherpa_ai-0.1.1/sherpa_ai/actions/__init__.py
--rw-r--r--   0        0        0     1644 2023-10-26 19:09:34.164052 sherpa_ai-0.1.1/sherpa_ai/actions/arxiv_search.py
--rw-r--r--   0        0        0      482 2023-10-26 19:09:34.165053 sherpa_ai-0.1.1/sherpa_ai/actions/base.py
--rw-r--r--   0        0        0     1789 2023-10-26 19:09:34.165053 sherpa_ai-0.1.1/sherpa_ai/actions/context_search.py
--rw-r--r--   0        0        0     1331 2023-10-26 19:09:34.166053 sherpa_ai-0.1.1/sherpa_ai/actions/deliberation.py
--rw-r--r--   0        0        0     1667 2023-11-01 19:00:23.403699 sherpa_ai-0.1.1/sherpa_ai/actions/google_search.py
--rw-r--r--   0        0        0     5630 2023-10-26 19:09:34.168053 sherpa_ai-0.1.1/sherpa_ai/actions/planning.py
--rw-r--r--   0        0        0     1339 2023-10-26 19:09:34.169053 sherpa_ai-0.1.1/sherpa_ai/actions/synthesize.py
--rw-r--r--   0        0        0      493 2023-10-26 19:09:34.169053 sherpa_ai-0.1.1/sherpa_ai/agents/__init__.py
--rw-r--r--   0        0        0     1177 2023-10-22 21:42:20.110091 sherpa_ai-0.1.1/sherpa_ai/agents/agent_pool.py
--rw-r--r--   0        0        0     3163 2023-10-26 19:09:34.170053 sherpa_ai-0.1.1/sherpa_ai/agents/base.py
--rw-r--r--   0        0        0     5148 2023-10-26 19:09:34.171055 sherpa_ai-0.1.1/sherpa_ai/agents/critic.py
--rw-r--r--   0        0        0     2871 2023-10-26 19:09:34.172052 sherpa_ai-0.1.1/sherpa_ai/agents/ml_engineer.py
--rw-r--r--   0        0        0     2557 2023-10-26 19:09:34.172052 sherpa_ai-0.1.1/sherpa_ai/agents/physicist.py
--rw-r--r--   0        0        0     2849 2023-10-26 19:09:34.173052 sherpa_ai-0.1.1/sherpa_ai/agents/planner.py
--rw-r--r--   0        0        0     3376 2023-10-26 19:09:34.173052 sherpa_ai-0.1.1/sherpa_ai/agents/qa_agent.py
--rw-r--r--   0        0        0     1665 2023-10-22 21:42:20.116222 sherpa_ai-0.1.1/sherpa_ai/agents/user.py
--rw-r--r--   0        0        0     3810 2023-11-01 19:00:26.438687 sherpa_ai-0.1.1/sherpa_ai/config.py
--rw-r--r--   0        0        0     1424 2023-09-14 14:00:23.450118 sherpa_ai-0.1.1/sherpa_ai/connectors/scripts/load_dump_to_chroma.py
--rw-r--r--   0        0        0     1249 2023-09-14 14:00:23.451116 sherpa_ai-0.1.1/sherpa_ai/connectors/scripts/query_chroma.py
--rw-r--r--   0        0        0     6672 2023-09-21 15:47:56.888677 sherpa_ai-0.1.1/sherpa_ai/connectors/vectorstores.py
--rw-r--r--   0        0        0      102 2023-09-07 18:58:13.900426 sherpa_ai-0.1.1/sherpa_ai/database/__init__.py
--rw-r--r--   0        0        0     7703 2023-11-01 19:00:26.438687 sherpa_ai-0.1.1/sherpa_ai/database/user_usage_tracker.py
--rw-r--r--   0        0        0      111 2023-09-07 18:58:13.901553 sherpa_ai-0.1.1/sherpa_ai/error_handling/__init__.py
--rw-r--r--   0        0        0     1762 2023-09-07 18:58:13.901553 sherpa_ai-0.1.1/sherpa_ai/error_handling/agent_error_handler.py
--rw-r--r--   0        0        0      841 2023-10-22 21:42:20.117097 sherpa_ai-0.1.1/sherpa_ai/events.py
--rw-r--r--   0        0        0      141 2023-10-22 21:42:20.118096 sherpa_ai-0.1.1/sherpa_ai/memory/__init__.py
--rw-r--r--   0        0        0     3692 2023-10-22 21:42:20.119096 sherpa_ai-0.1.1/sherpa_ai/memory/belief.py
--rw-r--r--   0        0        0     2093 2023-10-22 21:42:20.120096 sherpa_ai-0.1.1/sherpa_ai/memory/shared_memory.py
--rw-r--r--   0        0        0      181 2023-09-07 18:58:13.902558 sherpa_ai-0.1.1/sherpa_ai/models/__init__.py
--rw-r--r--   0        0        0     3002 2023-09-07 18:58:13.903331 sherpa_ai-0.1.1/sherpa_ai/models/sherpa_base_chat_model.py
--rw-r--r--   0        0        0     1522 2023-09-07 18:58:13.903331 sherpa_ai-0.1.1/sherpa_ai/models/sherpa_base_model.py
--rw-r--r--   0        0        0     4402 2023-10-22 21:42:20.122097 sherpa_ai-0.1.1/sherpa_ai/orchestrator.py
--rw-r--r--   0        0        0     1616 2023-09-07 18:58:13.904341 sherpa_ai-0.1.1/sherpa_ai/output_parser.py
--rw-r--r--   0        0        0      257 2023-09-07 18:58:13.904341 sherpa_ai-0.1.1/sherpa_ai/output_parsers/__init__.py
--rw-r--r--   0        0        0      153 2023-09-07 18:58:13.904341 sherpa_ai-0.1.1/sherpa_ai/output_parsers/base.py
--rw-r--r--   0        0        0     1917 2023-09-07 18:58:13.905751 sherpa_ai-0.1.1/sherpa_ai/output_parsers/link_parse.py
--rw-r--r--   0        0        0      391 2023-09-07 18:58:13.905751 sherpa_ai-0.1.1/sherpa_ai/output_parsers/md_to_slack_parse.py
--rw-r--r--   0        0        0      274 2023-09-07 18:58:13.905751 sherpa_ai-0.1.1/sherpa_ai/post_processors.py
--rw-r--r--   0        0        0     2845 2023-09-07 18:58:13.906764 sherpa_ai-0.1.1/sherpa_ai/prompt.py
--rw-r--r--   0        0        0     6810 2023-09-07 18:58:13.906764 sherpa_ai-0.1.1/sherpa_ai/prompt_generator.py
--rw-r--r--   0        0        0     2700 2023-09-07 18:58:13.906764 sherpa_ai-0.1.1/sherpa_ai/reflection.py
--rw-r--r--   0        0        0     2421 2023-09-07 18:58:13.908181 sherpa_ai-0.1.1/sherpa_ai/scrape/extract_github_readme.py
--rw-r--r--   0        0        0     3766 2023-11-01 19:00:26.440686 sherpa_ai-0.1.1/sherpa_ai/scrape/file_scraper.py
--rw-r--r--   0        0        0     2795 2023-11-01 19:00:26.440686 sherpa_ai-0.1.1/sherpa_ai/scrape/prompt_reconstructor.py
--rw-r--r--   0        0        0    11021 2023-11-01 19:00:23.405626 sherpa_ai-0.1.1/sherpa_ai/task_agent.py
--rw-r--r--   0        0        0     7243 2023-10-26 19:09:34.174052 sherpa_ai-0.1.1/sherpa_ai/tools.py
--rw-r--r--   0        0        0     8470 2023-11-01 19:00:26.441686 sherpa_ai-0.1.1/sherpa_ai/utils.py
--rw-r--r--   0        0        0      238 2023-09-07 18:58:13.910518 sherpa_ai-0.1.1/sherpa_ai/verbose_loggers/__init__.py
--rw-r--r--   0        0        0      141 2023-09-07 18:58:13.910518 sherpa_ai-0.1.1/sherpa_ai/verbose_loggers/base.py
--rw-r--r--   0        0        0     1012 2023-09-07 18:58:13.911517 sherpa_ai-0.1.1/sherpa_ai/verbose_loggers/verbose_loggers.py
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 sherpa_ai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1281 2024-04-04 20:47:37.185107 sherpa_ai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-09-07 18:58:13.889346 sherpa_ai-0.2.0/README.md
+-rw-r--r--   0        0        0       23 2023-09-07 18:58:13.896351 sherpa_ai-0.2.0/sherpa_ai/__init__.py
+-rw-r--r--   0        0        0      203 2023-10-22 21:42:20.082581 sherpa_ai-0.2.0/sherpa_ai/action_planner/__init__.py
+-rw-r--r--   0        0        0     3888 2023-12-19 19:27:04.507940 sherpa_ai-0.2.0/sherpa_ai/action_planner/action_planner.py
+-rw-r--r--   0        0        0      285 2023-12-19 19:27:04.507940 sherpa_ai-0.2.0/sherpa_ai/action_planner/base.py
+-rw-r--r--   0        0        0     1427 2023-11-22 04:28:04.077007 sherpa_ai-0.2.0/sherpa_ai/action_planner/selective_planner.py
+-rw-r--r--   0        0        0       66 2023-10-22 21:42:20.092581 sherpa_ai-0.2.0/sherpa_ai/action_planner/simple_planner.py
+-rw-r--r--   0        0        0      409 2024-04-04 20:46:01.175058 sherpa_ai-0.2.0/sherpa_ai/actions/__init__.py
+-rw-r--r--   0        0        0     1684 2024-02-28 14:01:30.482499 sherpa_ai-0.2.0/sherpa_ai/actions/arxiv_search.py
+-rw-r--r--   0        0        0      482 2023-12-19 19:27:04.509940 sherpa_ai-0.2.0/sherpa_ai/actions/base.py
+-rw-r--r--   0        0        0     1787 2023-12-19 19:27:04.510941 sherpa_ai-0.2.0/sherpa_ai/actions/context_search.py
+-rw-r--r--   0        0        0     1331 2023-12-19 19:27:04.510941 sherpa_ai-0.2.0/sherpa_ai/actions/deliberation.py
+-rw-r--r--   0        0        0     2918 2024-02-28 14:01:30.482499 sherpa_ai-0.2.0/sherpa_ai/actions/google_search.py
+-rw-r--r--   0        0        0     5641 2023-12-19 19:27:04.512941 sherpa_ai-0.2.0/sherpa_ai/actions/planning.py
+-rw-r--r--   0        0        0     1918 2024-03-01 16:22:17.952293 sherpa_ai-0.2.0/sherpa_ai/actions/synthesize.py
+-rw-r--r--   0        0        0      493 2024-02-20 04:55:11.807341 sherpa_ai-0.2.0/sherpa_ai/agents/__init__.py
+-rw-r--r--   0        0        0     1177 2023-11-22 02:47:37.184142 sherpa_ai-0.2.0/sherpa_ai/agents/agent_pool.py
+-rw-r--r--   0        0        0     4886 2024-03-01 16:17:05.632211 sherpa_ai-0.2.0/sherpa_ai/agents/base.py
+-rw-r--r--   0        0        0     5146 2023-12-19 19:27:04.514940 sherpa_ai-0.2.0/sherpa_ai/agents/critic.py
+-rw-r--r--   0        0        0     2895 2024-02-28 14:01:30.483423 sherpa_ai-0.2.0/sherpa_ai/agents/ml_engineer.py
+-rw-r--r--   0        0        0     2581 2024-02-28 14:01:30.483423 sherpa_ai-0.2.0/sherpa_ai/agents/physicist.py
+-rw-r--r--   0        0        0     2849 2023-12-19 19:27:04.515940 sherpa_ai-0.2.0/sherpa_ai/agents/planner.py
+-rw-r--r--   0        0        0     4838 2024-02-28 14:01:30.483423 sherpa_ai-0.2.0/sherpa_ai/agents/qa_agent.py
+-rw-r--r--   0        0        0     1665 2023-10-22 21:42:20.116222 sherpa_ai-0.2.0/sherpa_ai/agents/user.py
+-rw-r--r--   0        0        0     3905 2024-04-04 20:44:04.473809 sherpa_ai-0.2.0/sherpa_ai/config/__init__.py
+-rw-r--r--   0        0        0     3025 2024-01-17 05:47:33.698412 sherpa_ai-0.2.0/sherpa_ai/config/task_config.py
+-rw-r--r--   0        0        0     1424 2023-09-14 14:00:23.450118 sherpa_ai-0.2.0/sherpa_ai/connectors/scripts/load_dump_to_chroma.py
+-rw-r--r--   0        0        0     1249 2023-09-14 14:00:23.451116 sherpa_ai-0.2.0/sherpa_ai/connectors/scripts/query_chroma.py
+-rw-r--r--   0        0        0     6843 2024-02-07 04:00:13.352018 sherpa_ai-0.2.0/sherpa_ai/connectors/vectorstores.py
+-rw-r--r--   0        0        0      102 2023-09-07 18:58:13.900426 sherpa_ai-0.2.0/sherpa_ai/database/__init__.py
+-rw-r--r--   0        0        0    15220 2024-03-07 04:24:18.868368 sherpa_ai-0.2.0/sherpa_ai/database/user_usage_tracker.py
+-rw-r--r--   0        0        0      111 2023-09-07 18:58:13.901553 sherpa_ai-0.2.0/sherpa_ai/error_handling/__init__.py
+-rw-r--r--   0        0        0     1762 2023-09-07 18:58:13.901553 sherpa_ai-0.2.0/sherpa_ai/error_handling/agent_error_handler.py
+-rw-r--r--   0        0        0      841 2024-04-04 20:44:04.474845 sherpa_ai-0.2.0/sherpa_ai/events.py
+-rw-r--r--   0        0        0      141 2023-10-22 21:42:20.118096 sherpa_ai-0.2.0/sherpa_ai/memory/__init__.py
+-rw-r--r--   0        0        0     5423 2024-04-04 20:44:04.475878 sherpa_ai-0.2.0/sherpa_ai/memory/belief.py
+-rw-r--r--   0        0        0     2171 2024-02-28 14:01:30.484418 sherpa_ai-0.2.0/sherpa_ai/memory/shared_memory.py
+-rw-r--r--   0        0        0      181 2023-09-07 18:58:13.902558 sherpa_ai-0.2.0/sherpa_ai/models/__init__.py
+-rw-r--r--   0        0        0     2066 2024-02-15 02:06:06.152905 sherpa_ai-0.2.0/sherpa_ai/models/chat_model_with_logging.py
+-rw-r--r--   0        0        0     3224 2024-02-20 04:55:11.812339 sherpa_ai-0.2.0/sherpa_ai/models/sherpa_base_chat_model.py
+-rw-r--r--   0        0        0     1510 2024-04-03 04:17:33.589955 sherpa_ai-0.2.0/sherpa_ai/models/sherpa_base_model.py
+-rw-r--r--   0        0        0     4402 2023-10-22 21:42:20.122097 sherpa_ai-0.2.0/sherpa_ai/orchestrator.py
+-rw-r--r--   0        0        0     1616 2023-09-07 18:58:13.904341 sherpa_ai-0.2.0/sherpa_ai/output_parser.py
+-rw-r--r--   0        0        0      474 2024-02-28 14:01:30.485416 sherpa_ai-0.2.0/sherpa_ai/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1953 2024-02-28 14:01:30.485416 sherpa_ai-0.2.0/sherpa_ai/output_parsers/base.py
+-rw-r--r--   0        0        0    11349 2024-04-03 04:17:33.589955 sherpa_ai-0.2.0/sherpa_ai/output_parsers/citation_validation.py
+-rw-r--r--   0        0        0     4165 2024-02-15 02:06:06.155286 sherpa_ai-0.2.0/sherpa_ai/output_parsers/link_parse.py
+-rw-r--r--   0        0        0     1485 2024-02-15 02:06:06.155286 sherpa_ai-0.2.0/sherpa_ai/output_parsers/md_to_slack_parse.py
+-rw-r--r--   0        0        0     2062 2024-04-04 20:47:25.540942 sherpa_ai-0.2.0/sherpa_ai/output_parsers/number_validation.py
+-rw-r--r--   0        0        0      715 2024-04-03 04:17:33.590956 sherpa_ai-0.2.0/sherpa_ai/output_parsers/validation_result.py
+-rw-r--r--   0        0        0      274 2023-09-07 18:58:13.905751 sherpa_ai-0.2.0/sherpa_ai/post_processors.py
+-rw-r--r--   0        0        0     2834 2024-02-15 02:06:06.156687 sherpa_ai-0.2.0/sherpa_ai/prompt.py
+-rw-r--r--   0        0        0     6810 2023-09-07 18:58:13.906764 sherpa_ai-0.2.0/sherpa_ai/prompt_generator.py
+-rw-r--r--   0        0        0     2700 2023-09-07 18:58:13.906764 sherpa_ai-0.2.0/sherpa_ai/reflection.py
+-rw-r--r--   0        0        0     3226 2024-03-07 04:24:18.869369 sherpa_ai-0.2.0/sherpa_ai/scrape/extract_github_readme.py
+-rw-r--r--   0        0        0     5252 2024-04-03 04:17:33.591954 sherpa_ai-0.2.0/sherpa_ai/scrape/file_scraper.py
+-rw-r--r--   0        0        0     3588 2024-04-03 04:17:33.591954 sherpa_ai-0.2.0/sherpa_ai/scrape/prompt_reconstructor.py
+-rw-r--r--   0        0        0    10509 2024-02-15 02:06:06.156687 sherpa_ai-0.2.0/sherpa_ai/task_agent.py
+-rw-r--r--   0        0        0      327 2024-02-28 14:01:30.486415 sherpa_ai-0.2.0/sherpa_ai/test_utils/data.py
+-rw-r--r--   0        0        0     1752 2024-03-07 05:54:44.991058 sherpa_ai-0.2.0/sherpa_ai/test_utils/llms.py
+-rw-r--r--   0        0        0      755 2023-12-19 20:27:38.204282 sherpa_ai-0.2.0/sherpa_ai/test_utils/loggers.py
+-rw-r--r--   0        0        0    10071 2024-02-07 04:00:13.356017 sherpa_ai-0.2.0/sherpa_ai/tools.py
+-rw-r--r--   0        0        0    13170 2024-04-04 20:47:25.541939 sherpa_ai-0.2.0/sherpa_ai/utils.py
+-rw-r--r--   0        0        0      238 2024-02-15 02:06:06.158160 sherpa_ai-0.2.0/sherpa_ai/verbose_loggers/__init__.py
+-rw-r--r--   0        0        0      141 2023-09-07 18:58:13.910518 sherpa_ai-0.2.0/sherpa_ai/verbose_loggers/base.py
+-rw-r--r--   0        0        0     1012 2023-11-20 05:23:41.530778 sherpa_ai-0.2.0/sherpa_ai/verbose_loggers/verbose_loggers.py
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 sherpa_ai-0.2.0/PKG-INFO
```

### Comparing `sherpa_ai-0.1.1/pyproject.toml` & `sherpa_ai-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 [tool.poetry]
 name = "sherpa-ai"
-version = "0.1.1"
+version = "0.2.0"
 description = "Sherpa: AI-augmented thinking companion"
 authors = []
 readme = "README.md"
 repository = "https://github.com/Aggregate-Intellect/sherpa"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-langchain = "0.0.205"
+langchain = "0.0.332"
 python-dotenv = "^1.0.0"
 unstructured = "^0.10.11"
 openai = "^0.28.0"
 chromadb = "^0.4.8"
 tiktoken = "^0.4.0"
 pinecone-client = "^2.2.2"
 beautifulsoup4 = "4.12.2"
 markdown = ">=3.4.4,<3.5.0"
 loguru = ">=0.7.0,<0.8.0"
-pypdf2 = "^3.0.1"
-
+boto3 = "^1.28.77"
+pypdf = "^3.17.0"
+transformers = "^4.35.2"
+pydantic = "^2.5.3"
+hydra-core = "^1.3.2"
+word2number = "^1.1"
+spacy = "^3.7.4"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.4.0"
 pytest-cov = "^4.1.0"
 
 
@@ -37,14 +42,17 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "."
 ]
+markers = [
+  "external_api:  this test calls 3rd party APIs"
+]
 
 [tool.black]
 line-length = 88
 
 [tool.flake8]
 max-line-length = 88
 ignore  = ['F401', 'W503']
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/action_planner/action_planner.py` & `sherpa_ai-0.2.0/sherpa_ai/action_planner/action_planner.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,15 +65,19 @@
         Args:
             output_str: Output string
 
         Returns:
             str: Action to be taken
             dict: Arguments for the action
         """
-        output = json.loads(output_str)
+        try:
+            output = json.loads(output_str)
+        except json.decoder.JSONDecodeError:
+            logger.error("Output is not a proper json format {}", output_str)
+            return "Finished", None
         command = output["command"]
         name = command["name"]
         args = command.get("args", {})
         return name, args
 
     def select_action(
         self,
@@ -106,21 +110,20 @@
             task_description=task_description,
             possible_actions=possible_actions,
             history_of_previous_actions=history_of_previous_actions,
             task_context=task_context,
             output_instruction=self.output_instruction,
             response_format=response_format,
         )
-
         logger.debug(f"Prompt: {prompt}")
         result = self.llm.predict(prompt)
         logger.debug(f"Result: {result}")
 
         if result == "Finished":
             return None
 
         name, args = self.transform_output(result)
 
         if name == "Finished":
             return None
-        
-        return name, args
+
+        return name, args
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/action_planner/selective_planner.py` & `sherpa_ai-0.2.0/sherpa_ai/action_planner/selective_planner.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/actions/arxiv_search.py` & `sherpa_ai-0.2.0/sherpa_ai/actions/arxiv_search.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 class ArxivSearch(BaseAction):
     def __init__(
         self,
         role_description: str,
         task: str,
         llm: BaseLanguageModel,
         description: str = SEARCH_SUMMARY_DESCRIPTION,
-        n: int = 5,
+        max_results: int = 5,
     ):
         self.role_description = role_description
         self.task = task
 
         self.description = description
         self.llm = llm
-        self.n = n
+        self.max_results = max_results
 
         self.search_tool = SearchArxivTool()
 
     def execute(self, query) -> str:
         result = self.search_tool._run(query)
 
         prompt = self.description.format(
             task=self.task,
             paper_title_summary=result,
-            n=self.n,
+            n=self.max_results,
             role_description=self.role_description,
         )
 
         result = self.llm.predict(prompt)
 
         return result
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/actions/context_search.py` & `sherpa_ai-0.2.0/sherpa_ai/actions/context_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.role_description = role_description
         self.task = task
 
         self.description = description
         self.llm = llm
         self.n = n
 
-        self.context = ContextTool(memory = get_vectordb())
+        self.context = ContextTool(memory=get_vectordb())
 
     def execute(self, query) -> str:
         result = self.context._run(query)
         # result = "Context Search"
         logger.debug("Context Search Result: {}", result)
 
         prompt = self.description.format(
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/actions/deliberation.py` & `sherpa_ai-0.2.0/sherpa_ai/actions/deliberation.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/actions/planning.py` & `sherpa_ai-0.2.0/sherpa_ai/actions/planning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from langchain.llms.base import LLM
 from loguru import logger
 
 from sherpa_ai.actions.base import BaseAction
 
-PLANNING_PROMPT = """You are a **task decomposition assisstant** who simplifies complex tasks into sequential steps, assigning roles or agents to each.
+PLANNING_PROMPT = """You are a **task decomposition assistant** who simplifies complex tasks into sequential steps, assigning roles or agents to each.
 By analyzing user-defined tasks and agent capabilities, you provides structured plans, enhancing project clarity and efficiency.
 Your adaptability ensures customized solutions for diverse needs.
 
 A good plan is concise, detailed, feasible and efficient.
 
 Task: **{task}**
 
@@ -25,16 +25,16 @@
     Agent: <AgentName>
     Task: <detailed task description>
 
 Do not answer anything else, and do not add any other information in your answer. Only select agents from the the list and only select one agent at a time.
 """  # noqa: E501
 
 
-REVISION_PROMPT = """You are a **task decomposition assisstant** who simplifies complex tasks into sequential steps, assigning roles or agents to each.
-By analyzing user-defined tasks and agent capabilities, you provides structured plans, enhancing project clarity and efficiency.
+REVISION_PROMPT = """You are a **task decomposition assistant** who simplifies complex tasks into sequential steps, assigning roles or agents to each.
+By analyzing user-defined tasks and agent capabilities, you provide structured plans, enhancing project clarity and efficiency.
 Your adaptability ensures customized solutions for diverse needs.
 
 A good plan is concise, detailed, feasible and efficient. It should be broken down into individual steps, with each step assigned to an appropriate agent.
 
 Task: **{task}**
 
 Agents:
@@ -112,16 +112,16 @@
         self.prompt = PLANNING_PROMPT
         self.revision_prompt = REVISION_PROMPT
 
     def execute(
         self,
         task: str,
         agent_pool_description: str,
-        last_plan: Optional[str],
-        feedback: Optional[str],
+        last_plan: Optional[str] = None,
+        feedback: Optional[str] = None,
     ) -> Plan:
         """
         Execute the action
         """
 
         if last_plan is None or feedback is None:
             prompt = self.prompt.format(
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/agents/agent_pool.py` & `sherpa_ai-0.2.0/sherpa_ai/agents/agent_pool.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/agents/critic.py` & `sherpa_ai-0.2.0/sherpa_ai/agents/critic.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,13 +115,13 @@
 
             self.shared_memory.add(EventType.feedback, self.name, feedback)
             logger.info(f"feedback: {feedback}")
 
             return self.post_process(feedback)
         else:
             return ""
-    
+
     def create_actions(self):
         pass
 
     def synthesize_output(self) -> str:
-        pass
+        pass
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/agents/ml_engineer.py` & `sherpa_ai-0.2.0/sherpa_ai/agents/ml_engineer.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,22 +30,24 @@
         llm: BaseLanguageModel,
         name="ML Engineer",
         description=ML_ENGINEER_DESCRIPTION,
         shared_memory: SharedMemory = None,
         num_runs=3,
         verbose_logger=DummyVerboseLogger(),
     ):
+        super().__init__(
+            name=name,
+            description=description,
+            shared_memory=shared_memory,
+            belief=Belief(),
+            action_planner=ActionPlanner(description, ACTION_PLAN_DESCRIPTION, llm),
+            num_runs=num_runs,
+            verbose_logger=verbose_logger,
+        )
         self.llm = llm
-        self.name = name
-        self.description = description
-        self.shared_memory = shared_memory
-        self.action_planner = ActionPlanner(description, ACTION_PLAN_DESCRIPTION, llm)
-        self.num_runs = num_runs
-        self.belief = Belief()
-        self.verbose_logger = verbose_logger
 
     def create_actions(self) -> List[BaseAction]:
         return [
             Deliberation(self.description, self.llm),
             GoogleSearch(self.description, self.belief.current_task, self.llm),
             ArxivSearch(self.description, self.belief.current_task, self.llm),
         ]
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/agents/physicist.py` & `sherpa_ai-0.2.0/sherpa_ai/agents/physicist.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,22 +25,24 @@
         llm: BaseLanguageModel,
         name="Physicist",
         description=PHYSICIST_DESCRIPTION,
         shared_memory: SharedMemory = None,
         num_runs=3,
         verbose_logger=DummyVerboseLogger(),
     ):
+        super().__init__(
+            name=name,
+            description=description,
+            shared_memory=shared_memory,
+            belief=Belief(),
+            action_planner=ActionPlanner(description, ACTION_PLAN_DESCRIPTION, llm),
+            num_runs=num_runs,
+            verbose_logger=verbose_logger,
+        )
         self.llm = llm
-        self.name = name
-        self.description = description
-        self.shared_memory = shared_memory
-        self.action_planner = ActionPlanner(description, ACTION_PLAN_DESCRIPTION, llm)
-        self.num_runs = num_runs
-        self.belief = Belief()
-        self.verbose_logger = verbose_logger
 
     def create_actions(self) -> List[BaseAction]:
         return [
             Deliberation(self.description, self.llm),
             GoogleSearch(self.description, self.belief.current_task, self.llm),
         ]
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/agents/planner.py` & `sherpa_ai-0.2.0/sherpa_ai/agents/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from sherpa_ai.actions.planning import TaskPlanning
 from sherpa_ai.agents.agent_pool import AgentPool
 from sherpa_ai.agents.base import BaseAgent
 from sherpa_ai.events import Event, EventType
 from sherpa_ai.memory import Belief, SharedMemory
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
-PLANNER_DESCRIPTION = """You are a **task decomposition assisstant** who simplifies complex tasks into sequential steps, assigning roles or agents to each.
-By analyzing user-defined tasks and agent capabilities, you provides structured plans, enhancing project clarity and efficiency.
+PLANNER_DESCRIPTION = """You are a **task decomposition assistant** who simplifies complex tasks into sequential steps, assigning roles or agents to each.
+By analyzing user-defined tasks and agent capabilities, you provide structured plans, enhancing project clarity and efficiency.
 Your adaptability ensures customized solutions for diverse needs. 
 """  # noqa: E501
 
 
 class Planner(BaseAgent):
     def __init__(
         self,
@@ -78,8 +78,8 @@
 
         return plan
 
     def create_actions(self):
         pass
 
     def synthesize_output(self) -> str:
-        pass
+        pass
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/agents/qa_agent.py` & `sherpa_ai-0.2.0/sherpa_ai/agents/qa_agent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,106 @@
-from typing import List
+from typing import List, Optional
 
 from langchain.base_language import BaseLanguageModel
 
 from sherpa_ai.action_planner import ActionPlanner
-from sherpa_ai.actions import Deliberation, GoogleSearch, SynthesizeOutput
+from sherpa_ai.actions import GoogleSearch, SynthesizeOutput
 from sherpa_ai.actions.base import BaseAction
 from sherpa_ai.agents.base import BaseAgent
+from sherpa_ai.config import AgentConfig
 from sherpa_ai.memory import Belief
 from sherpa_ai.memory.shared_memory import SharedMemory
+from sherpa_ai.output_parsers.base import BaseOutputProcessor
+from sherpa_ai.output_parsers.citation_validation import CitationValidation
+from sherpa_ai.verbose_loggers.base import BaseVerboseLogger
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
 # TODO: QA Agent only contains partial implementation from the original
 # task agent, more investigation is needed to add more content to it.
 # Some of the feature may be added to the agent base class, such as
 # the verbose logger.
 
 ACTION_PLAN_DESCRIPTION = "Given your specialized expertise, historical context, and your mission to facilitate Machine-Learning-based solutions, determine which action and its corresponding arguments would be the most scientifically sound and efficient approach to achieve the described task."  # noqa: E501
 
-TASK_AGENT_DESRIPTION = "You are a **question answering assistant** who solves user questions and offers a detailed solution."  # noqa: E501
+TASK_AGENT_DESCRIPTION = "You are a **question answering assistant** who solves user questions and offers a detailed solution."  # noqa: E501
 
 
 class QAAgent(BaseAgent):
     """
     The task agent is the agent handles a single task.
     """
 
     def __init__(
         self,
         llm: BaseLanguageModel,
         name: str = "QA Agent",
-        description: str = TASK_AGENT_DESRIPTION,
+        description: str = TASK_AGENT_DESCRIPTION,
         shared_memory: SharedMemory = None,
-        belief: Belief = Belief(),
+        belief: Optional[Belief] = None,
+        agent_config: AgentConfig = AgentConfig(),
         num_runs: int = 3,
-        verbose_logger=DummyVerboseLogger(),
+        verbose_logger: BaseVerboseLogger = DummyVerboseLogger(),
+        actions: List[BaseAction] = [],
+        validation_steps: int = 1,
+        validations: List[BaseOutputProcessor] = [],
     ):
         """
-        The QA agent is the agent handles a single task.
+        The QA agent handles a single question-answering task.
 
         Args:
             llm (BaseLanguageModel): The language model used to generate text
             name (str, optional): The name of the agent. Defaults to "QA Agent".
-            description (str, optional): The description of the agent. Defaults
-                to TASK_AGENT_DESRIPTION.
-            shared_memory (SharedMemory, optional): The shared memory used to
-                store the context shared with all other agents. Defaults to None.
-            belief (Belief, optional): The belief of the agent. Defaults to Belief().
-            num_runs (int, optional): The number of runs the agent will run. Defaults
-                to 3.
-            verbose_logger (BaseVerboseLogger, optional): The verbose logger used to
-                log the agent's internal state. Defaults to DummyVerboseLogger().
+            description (str, optional): The description of the agent. Defaults to TASK_AGENT_DESCRIPTION.
+            shared_memory (SharedMemory, optional): The shared memory used to store information and shared with other agents. Defaults to None.
+            belief (Optional[Belief], optional): The belief of the agent. Defaults to None.
+            agent_config (AgentConfig, optional): The agent configuration. Defaults to AgentConfig.
+            num_runs (int, optional): The number of runs the agent will perform. Defaults to 3.
+            verbose_logger (BaseVerboseLogger, optional): The verbose logger used to log information. Defaults to DummyVerboseLogger().
+            actions (List[BaseAction], optional): The list of actions the agent can perform. Defaults to [].
+            validation_steps (int, optional): The number of validation steps the agent will perform. Defaults to 1.
+            validations (List[BaseOutputProcessor], optional): The list of validations the agent will perform. Defaults to [].
         """
-        self.name = name
-        self.description = description
-        self.shared_memory = shared_memory
-        self.belief = belief
-        self.num_runs = num_runs
+        super().__init__(
+            name,
+            description + "\n\n" + f"Your name is {name}.",
+            shared_memory,
+            belief,
+            ActionPlanner(description, ACTION_PLAN_DESCRIPTION, llm),
+            num_runs,
+            verbose_logger,
+            actions,
+            validation_steps,
+            validations,
+        )
         self.llm = llm
-        self.action_planner = ActionPlanner(description, ACTION_PLAN_DESCRIPTION, llm)
-        self.verbose_logger = verbose_logger
+        self.config = agent_config
+
+        if belief is None:
+            belief = Belief()
+        self.belief = belief
+        self.citation_enabled = False
+        for validation in self.validations:
+            if isinstance(validation, CitationValidation):
+                self.citation_enabled = True
+                break
 
     def create_actions(self) -> List[BaseAction]:
         return [
-            GoogleSearch(self.description, self.belief.current_task, self.llm),
+            GoogleSearch(
+                self.description,
+                self.belief.current_task,
+                self.llm,
+                config=self.config,
+                include_metadata=self.citation_enabled,
+            ),
         ]
 
     def synthesize_output(self) -> str:
-        synthesize_action = SynthesizeOutput(self.description, self.llm)
+        synthesize_action = SynthesizeOutput(
+            self.description, self.llm, add_citation=self.citation_enabled
+        )
         result = synthesize_action.execute(
             self.belief.current_task.content,
             self.belief.get_context(self.llm.get_num_tokens),
             self.belief.get_internal_history(self.llm.get_num_tokens),
         )
-
         return result
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/agents/user.py` & `sherpa_ai-0.2.0/sherpa_ai/agents/user.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/config.py` & `sherpa_ai-0.2.0/sherpa_ai/config/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 
 import sys
 from os import environ
 
 from dotenv import find_dotenv, load_dotenv
 from loguru import logger
 
+from sherpa_ai.config.task_config import AgentConfig
+
 env_path = find_dotenv(usecwd=True)
 load_dotenv(env_path)
 
 
 AWS_ACCESS_KEY = environ.get("AWS_ACCESS_KEY")
 AWS_SECRET_KEY = environ.get("AWS_SECRET_KEY")
 FLASK_DEBUG = environ.get("FLASK_DEBUG", False) == "True"
 GITHUB_AUTH_TOKEN = environ.get("GITHUB_AUTH_TOKEN")
 SLACK_SIGNING_SECRET = environ.get("SLACK_SIGNING_SECRET")
 SLACK_OAUTH_TOKEN = environ.get("SLACK_OAUTH_TOKEN")
 SLACK_VERIFICATION_TOKEN = environ.get("SLACK_VERIFICATION_TOKEN")
 SLACK_PORT = environ.get("SLACK_PORT", 3000)
 OPENAI_API_KEY = environ.get("OPENAI_API_KEY")
-TEMPRATURE = environ.get("TEMPRATURE") or 0
+TEMPERATURE = environ.get("TEMPERATURE") or 0
 
 # Pinecone settings
 PINECONE_API_KEY = environ.get("PINECONE_API_KEY")
 PINECONE_NAMESPACE = environ.get("PINECONE_NAMESPACE", "ReadTheDocs")
 PINECONE_ENV = environ.get("PINECONE_ENV")
 PINECONE_INDEX = environ.get("PINECONE_INDEX")
 
@@ -42,23 +44,24 @@
 CHROMA_HOST = environ.get("CHROMA_HOST")
 CHROMA_PORT = environ.get("CHROMA_PORT")
 CHROMA_INDEX = environ.get("CHROMA_INDEX")
 
 SERPER_API_KEY = environ.get("SERPER_API_KEY")
 LOG_LEVEL = environ.get("LOG_LEVEL", "INFO").upper()
 
-#Usage setting 
-DAILY_TOKEN_LIMIT = environ.get("DAILY_TOKEN_LIMIT") or 20000
+# Usage setting
+DAILY_TOKEN_LIMIT = float(environ.get("DAILY_TOKEN_LIMIT") or 20000)
 DAILY_LIMIT_REACHED_MESSAGE = (
     environ.get("DAILY_LIMIT_REACHED_MESSAGE")
     or "Sorry for the inconvenience, but it seems that you have exceeded your daily token limit. As a result, you will need to try again after 24 hours. Thank you for your understanding."
 )
 LIMIT_TIME_SIZE_IN_HOURS = environ.get("LIMIT_TIME_SIZE_IN_HOURS") or "24"
 FILE_SIZE_LIMIT = environ.get("FILE_SIZE_LIMIT") or 2097152
 FILE_TOKEN_LIMIT = environ.get("FILE_TOKEN_LIMIT") or 20000
+DB_NAME = environ.get("DB_NAME") or "sqlite:///token_counter.db"
 
 # Configure logger. To get JSON serialization, set serialize=True.
 # See https://loguru.readthedocs.io/en/stable/ for info on Loguru features.
 logger.remove(0)  # remove the default handler configuration
 logger.add(sys.stderr, level=LOG_LEVEL, serialize=False)
 
 
@@ -93,19 +96,21 @@
 # Ensure all mandatory environment variables are set, otherwise exit
 if None in [
     this.SLACK_VERIFICATION_TOKEN,
     this.SLACK_SIGNING_SECRET,
     this.SLACK_OAUTH_TOKEN,
     this.SLACK_PORT,
 ]:
-    logger.info("Config: Slack environment variables not set, unable to run")
-    raise SystemExit(1)
+    logger.warning("Config: Slack environment variables not set")
 else:
     logger.info("Config: Slack environment variables are set")
 
 if this.OPENAI_API_KEY is None:
-    logger.info("Config: OpenAI environment variables not set, unable to run")
-    raise SystemExit(1)
+    logger.warning("Config: OpenAI environment variables not set")
 else:
     logger.info("Config: OpenAI environment variables are set")
 
 check_vectordb_setting()
+
+__all__ = [
+    "AgentConfig",
+]
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/connectors/scripts/load_dump_to_chroma.py` & `sherpa_ai-0.2.0/sherpa_ai/connectors/scripts/load_dump_to_chroma.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/connectors/scripts/query_chroma.py` & `sherpa_ai-0.2.0/sherpa_ai/connectors/scripts/query_chroma.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/connectors/vectorstores.py` & `sherpa_ai-0.2.0/sherpa_ai/connectors/vectorstores.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,39 @@
 from sherpa_ai.utils import load_files
 
 
 class ConversationStore(VectorStore):
     def __init__(self, namespace, db, embeddings, text_key):
         self.db = db
         self.namespace = namespace
-        self.embeddings = embeddings
+        self.embeddings_func = embeddings
         self.text_key = text_key
 
     @classmethod
     def from_index(cls, namespace, openai_api_key, index_name, text_key="text"):
         pinecone.init(api_key=cfg.PINECONE_API_KEY, environment=cfg.PINECONE_ENV)
         logger.info(f"Loading index {index_name} from Pinecone")
         index = pinecone.Index(index_name)
-        embeddings = OpenAIEmbeddings(openai_api_key=openai_api_key)
-        return cls(namespace, index, embeddings, text_key)
+        embedding = OpenAIEmbeddings(openai_api_key=openai_api_key)
+        return cls(namespace, index, embedding, text_key)
 
     def add_text(self, text: str, metadata={}) -> str:
         metadata[self.text_key] = text
         id = str(uuid.uuid4())
         embedding = self.embeddings.embed_query(text)
         doc = {"id": id, "values": embedding, "metadata": metadata}
         self.db.upsert(vectors=[doc], namespace=self.namespace)
 
         return id
 
+    @property
+    def embeddings(self) -> Optional[Embeddings]:
+        """Access the query embedding object if available."""
+        return self.embeddings_func
+
     def add_texts(self, texts: Iterable[str], metadatas: List[dict]) -> List[str]:
         for text, metadata in zip(texts, metadatas):
             self.add_text(text, metadata)
 
     def similarity_search(
         self,
         text: str,
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/error_handling/agent_error_handler.py` & `sherpa_ai-0.2.0/sherpa_ai/error_handling/agent_error_handler.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/events.py` & `sherpa_ai-0.2.0/sherpa_ai/events.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/memory/belief.py` & `sherpa_ai-0.2.0/sherpa_ai/memory/belief.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from typing import Callable, List
+from typing import Callable, List, Optional
 
 from sherpa_ai.actions.base import BaseAction
 from sherpa_ai.events import Event, EventType
 
 
 class Belief:
-    def __init__(self):
-        # TODO: Handle long belief history, if it's longer than the context size
-        # maybe use summarization or a vector db
+    """
+    The belief of the agent. it contains
+        1. events: the events observed by the agent, synchronized with the shared memory
+        2. internal_events: the internal events generated by the agent through its reasoning process (actions)
+    """
 
+    def __init__(self):
         self.events: List[Event] = []
         self.internal_events: List[Event] = []
         self.current_task: Event = None
 
     def update(self, observation: Event):
         if observation in self.events:
             return
@@ -25,15 +28,17 @@
         agent: str,
         content: str,
     ):
         event = Event(event_type=event_type, agent=agent, content=content)
         self.internal_events.append(event)
 
     def get_by_type(self, event_type):
-        return [event for event in self.internal_events if event.event_type == event_type]
+        return [
+            event for event in self.internal_events if event.event_type == event_type
+        ]
 
     def set_current_task(self, task: Event):
         self.current_task = task
 
     def get_context(self, token_counter: Callable[[str], int], max_tokens=4000):
         """
         Get the context of the agent
@@ -68,28 +73,65 @@
         Get the internal history of the agent
 
         Args:
             token_counter: Token counter
             max_tokens: Maximum number of tokens
 
         Returns:
-            str: Internal history of the agent
+            str: Internal history of the agent with event content separated by newlines.
+            History is truncated if the number of tokens exceeds `max_tokens`.
         """
         results = []
         current_tokens = 0
 
         for event in reversed(self.internal_events):
             results.append(event.content)
             current_tokens += token_counter(event.content)
-
             if current_tokens > max_tokens:
                 break
 
         context = "\n".join(reversed(results))
+        return context
 
+    def get_histories_excluding_types(
+        self,
+        exclude_types: list[EventType],
+        token_counter: Optional[Callable[[str], int]] = None,
+        max_tokens=4000,
+    ):
+        """
+            Get the internal history of the agent without events of excluded_type
+
+        Args:
+            token_counter: Token counter
+            max_tokens: Maximum number of tokens
+            exclude_types: List of events to be excluded
+
+        Returns:
+            str: Internal history of the agent with event content separated by newlines.
+            History is truncated if the number of tokens exceeds `max_tokens`.
+        """
+        if token_counter is None:
+            # if no token counter is provided, use the default word counter
+            def token_counter(x):
+                return len(x.split())
+
+        results = []
+        feedback = []
+        current_tokens = 0
+        for event in reversed(self.internal_events):
+            if event.event_type not in exclude_types:
+                if event.event_type == EventType.feedback:
+                    feedback.append(event.content)
+                else:
+                    results.append(event.content)
+            current_tokens += token_counter(event.content)
+            if current_tokens > max_tokens:
+                break
+        context = "\n".join(set(reversed(results))) + "\n".join(set(feedback))
         return context
 
     def set_actions(self, actions: List[BaseAction]):
         self.actions = actions
 
     @property
     def action_description(self):
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/memory/shared_memory.py` & `sherpa_ai-0.2.0/sherpa_ai/memory/shared_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from typing import List, Optional
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, List, Optional
 
 from sherpa_ai.actions.planning import Plan
-from sherpa_ai.agents import AgentPool
 from sherpa_ai.events import Event, EventType
 from sherpa_ai.memory.belief import Belief
 
+if TYPE_CHECKING:
+    from sherpa_ai.agents import AgentPool
+
 
 class SharedMemory:
     def __init__(self, objective: str, agent_pool: AgentPool = None):
         self.objective = objective
         self.agent_pool = agent_pool
         self.events: List[Event] = []
         self.plan: Optional[Plan] = None
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/models/sherpa_base_chat_model.py` & `sherpa_ai-0.2.0/sherpa_ai/models/sherpa_base_chat_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,21 @@
     CallbackManagerForLLMRun,
 )
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import BaseMessage, ChatResult
 
 from sherpa_ai.database.user_usage_tracker import UserUsageTracker
+from sherpa_ai.verbose_loggers.base import BaseVerboseLogger
 
 
 class SherpaBaseChatModel(BaseChatModel):
     team_id: typing.Optional[str] = None
     user_id: typing.Optional[str] = None
+    verbose_logger: BaseVerboseLogger = None
 
     def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
@@ -40,24 +42,25 @@
         token_before = super().get_num_tokens_from_messages(messages)
         token_after = 0
         for result_message in response.generations:
             token_after += super().get_num_tokens(result_message.text)
         total_token = token_before + token_after
         if self.team_id and self.user_id:
             combined_id = self.user_id + "_" + self.team_id
-            user_db = UserUsageTracker()
+            user_db = UserUsageTracker(verbose_logger=self.verbose_logger)
             user_db.add_data(combined_id=combined_id, token=total_token)
             user_db.close_connection()
 
         return response
 
 
 class SherpaChatOpenAI(ChatOpenAI):
     team_id: typing.Optional[str] = None
     user_id: typing.Optional[str] = None
+    verbose_logger: BaseVerboseLogger = None
 
     def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
@@ -79,12 +82,12 @@
         token_before = super().get_num_tokens_from_messages(messages)
         token_after = 0
         for result_message in response.generations:
             token_after += super().get_num_tokens(result_message.text)
         total_token = token_before + token_after
         if self.team_id and self.user_id:
             combined_id = self.user_id + "_" + self.team_id
-            user_db = UserUsageTracker()
+            user_db = UserUsageTracker(verbose_logger=self.verbose_logger)
             user_db.add_data(combined_id=combined_id, token=total_token)
             user_db.close_connection()
 
         return response
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/models/sherpa_base_model.py` & `sherpa_ai-0.2.0/sherpa_ai/models/sherpa_base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import typing
 from typing import Any, List, Optional
 
-from langchain import OpenAI
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
+from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import BaseMessage, ChatResult
-from pydantic import BaseModel
 
 from sherpa_ai.database.user_usage_tracker import UserUsageTracker
 
 
-class SherpaOpenAI(OpenAI):
+class SherpaOpenAI(ChatOpenAI):
     team_id: typing.Optional[str] = None
     user_id: typing.Optional[str] = None
 
     def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/orchestrator.py` & `sherpa_ai-0.2.0/sherpa_ai/orchestrator.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/output_parser.py` & `sherpa_ai-0.2.0/sherpa_ai/output_parser.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/prompt.py` & `sherpa_ai-0.2.0/sherpa_ai/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from loguru import logger
 from pydantic import BaseModel
 
 from sherpa_ai.prompt_generator import get_prompt
 from sherpa_ai.tools import BaseTool
 
 
-class SlackBotPrompt(BaseChatPromptTemplate, BaseModel):
+class SlackBotPrompt(BaseChatPromptTemplate):
     ai_name: str
     ai_role: str
     tools: List[BaseTool]
     token_counter: Callable[[str], int]
     send_token_limit: int = 4196
 
     def construct_base_prompt(self):
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/prompt_generator.py` & `sherpa_ai-0.2.0/sherpa_ai/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/reflection.py` & `sherpa_ai-0.2.0/sherpa_ai/reflection.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/sherpa_ai/scrape/extract_github_readme.py` & `sherpa_ai-0.2.0/sherpa_ai/scrape/extract_github_readme.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,35 +8,56 @@
 from loguru import logger
 
 import sherpa_ai.config as cfg
 from sherpa_ai.connectors.vectorstores import ConversationStore
 
 
 def get_owner_and_repo(url):
+    """
+    Extracts the owner and repository name from a GitHub repository URL.
+
+    Parameters:
+    - url (str): The GitHub repository URL.
+
+    Returns:
+    Tuple[str, str]: A tuple containing the owner and repository name.
+    """
+
     url_content_list = url.split("/")
     return url_content_list[3], url_content_list[4].split("#")[0]
 
 
 def extract_github_readme(repo_url):
+    """
+    Extracts the content of the README file from a GitHub repository.
+
+    Parameters:
+    - repo_url (str): The GitHub repository URL.
+
+    Returns:
+    str or None: The content of the README file, or None if the file is not found.
+    """
+
     pattern = r"(?:https?://)?(?:www\.)?github\.com/.*"
     match = re.match(pattern, repo_url)
     if match:
         owner, repo = get_owner_and_repo(repo_url)
         path = "README.md"
         token = cfg.GITHUB_AUTH_TOKEN
-        logger.info(token)
         github_api_url = f"https://api.github.com/repos/{owner}/{repo}/contents"
         headers = {
             "Authorization": f"token {token}",
             "X-GitHub-Api-Version": "2022-11-28",
         }
 
         response = requests.get(github_api_url, headers=headers)
 
         files = response.json()
+        if type(files) is dict and files["message"].lower() == "bad credentials":
+            return None
         matching_files = [
             file["name"]
             for file in files
             if (
                 (
                     file["name"].lower().endswith(".md")
                     or file["name"].lower().endswith(".rst")
@@ -59,13 +80,21 @@
             save_to_pine_cone(content, metadata)
             return content
         else:
             logger.warning("README file not found.")
 
 
 def save_to_pine_cone(content, metadatas):
+    """
+    Saves the content and metadata to Pinecone vector store.
+
+    Parameters:
+    - content (str): The content to be saved.
+    - metadatas (list): List of metadata associated with the content.
+    """
+
     pinecone.init(api_key=cfg.PINECONE_API_KEY, environment=cfg.PINECONE_ENV)
     index = pinecone.Index("langchain")
     embeddings = OpenAIEmbeddings(openai_api_key=cfg.OPENAI_API_KEY)
 
     vectorstore = ConversationStore("Github_data", index, embeddings, "text")
     vectorstore.add_texts(content, metadatas)
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/task_agent.py` & `sherpa_ai-0.2.0/sherpa_ai/task_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from langchain.tools.human.tool import HumanInputRun
 from langchain.vectorstores.base import VectorStoreRetriever
 from loguru import logger
 from pydantic import ValidationError
 
 from sherpa_ai.action_planner import SelectiveActionPlanner
 from sherpa_ai.action_planner.base import BaseActionPlanner
+from sherpa_ai.config import AgentConfig
 from sherpa_ai.output_parser import BaseTaskOutputParser, TaskOutputParser
 from sherpa_ai.output_parsers import LinkParser, MDToSlackParse
 from sherpa_ai.post_processors import md_link_to_slack
 from sherpa_ai.reflection import Reflection
 from sherpa_ai.utils import show_commands_only
 from sherpa_ai.verbose_loggers import DummyVerboseLogger
 from sherpa_ai.verbose_loggers.base import BaseVerboseLogger
@@ -38,43 +39,42 @@
         ai_name: str,
         ai_id: str,
         memory: VectorStoreRetriever,
         llm: BaseLLM,
         action_planner: BaseActionPlanner,
         output_parser: BaseTaskOutputParser,
         tools: List[BaseTool],
-        previous_messages: List[dict],
+        previous_messages: List[BaseMessage],
         verbose_logger: BaseVerboseLogger,
         feedback_tool: Optional[HumanInputRun] = None,
+        agent_config: AgentConfig = AgentConfig(),
         max_iterations: int = 5,
     ):
         self.ai_name = ai_name
         self.memory = memory
-        # self.full_message_history: List[BaseMessage] = []
         self.next_action_count = 0
         self.llm = llm
         self.output_parser = output_parser
         self.tools = tools
         self.verbose_logger = verbose_logger
 
         self.action_planner = action_planner
         self.feedback_tool = feedback_tool
         self.max_iterations = max_iterations
         self.loop_count = 0
         self.ai_id = ai_id
-        self.previous_message = self.process_chat_history(previous_messages)
-        self.logger = []  # added by JF
+        self.agent_config = agent_config
+        self.previous_message = previous_messages
+        self.logger = []
 
         link_parser = LinkParser()
         slack_link_paerser = MDToSlackParse()
 
         self.tool_output_parsers = [link_parser]
         self.output_parsers = [link_parser, slack_link_paerser]
-        # print(self.full_message_history)
-        # print("message:", self.previous_message)
 
     @classmethod
     def from_llm_and_tools(
         cls,
         ai_name: str,
         ai_role: str,
         ai_id: str,
@@ -82,14 +82,15 @@
         tools: List[BaseTool],
         llm: BaseChatModel,
         previous_messages,
         action_planner: BaseActionPlanner = None,
         human_in_the_loop: bool = False,
         output_parser: Optional[BaseTaskOutputParser] = None,
         max_iterations: int = 1,
+        agent_config: AgentConfig = AgentConfig(),
         verbose_logger: BaseVerboseLogger = DummyVerboseLogger(),
     ):
         if action_planner is None:
             action_planner = SelectiveActionPlanner(
                 llm, tools, ai_name=ai_name, ai_role=ai_role
             )
         human_feedback_tool = HumanInputRun() if human_in_the_loop else None
@@ -101,14 +102,15 @@
             llm,
             action_planner,
             output_parser or TaskOutputParser(),
             tools,
             previous_messages,
             verbose_logger,
             feedback_tool=human_feedback_tool,
+            agent_config=agent_config,
             max_iterations=max_iterations,
         )
 
     def run(self, task: str) -> str:
         user_input = (
             "Determine which next command to use. Select the finish command if you "
             "and respond using the JSON format specified above without any extra text."
@@ -125,17 +127,17 @@
             loop_count = self.loop_count
             logger_step = {"Step": f"{loop_count + 1}/{self.max_iterations}"}
 
             if loop_count >= self.max_iterations:
                 user_input = (
                     "Use the above information to respond to the user's message:"
                     f"\n{task}\n\n"
-                    "If you use any resource, then create inline citation by adding "
-                    " of the reference document at the end of the sentence in the format "
-                    "of 'Sentence [DocID]'\n"
+                    "If you use any resource, then create inline citation by adding"
+                    "the DocID of the reference document at the end of the sentence in "
+                    "the format of 'Sentence [DocID]'\n"
                     "Example:\n"
                     "Sentence1 [1]. Sentence2. Sentence3 [2].\n"
                     "Only use the reference document. DO NOT use any links"
                     " DO NOT include citation if the resource is not"
                     "necessary. only write text but not the JSON format specified "
                     "above. \nResult:"
                 )
@@ -148,22 +150,28 @@
             logger.info(f"reply: {assistant_reply}")
             # added by JF
             try:
                 reply_json = json.loads(assistant_reply)
                 logger_step["reply"] = reply_json
             except json.JSONDecodeError:
                 logger_step["reply"] = assistant_reply  # last reply is a string
+            if self.agent_config.verbose:
+                self.verbose_logger.log(f"```{assistant_reply}```")
+
             self.logger.append(logger_step)
 
-            ########## Serial Verbose Feature #######
-            try:
-                formatted_logger_step = show_commands_only(logger_step)
-            except Exception as e:
-                logger.error(e)
+            # Serial Verbose Feature
+            if self.agent_config.verbose:
                 formatted_logger_step = logger_step
+            else:
+                try:
+                    formatted_logger_step = show_commands_only(logger_step)
+                except KeyError as e:
+                    logger.error(e)
+                    formatted_logger_step = logger_step
 
             logger.info(f"```{formatted_logger_step}```")
             self.verbose_logger.log(f"```{formatted_logger_step}```")
             #######################################
 
             # return assistant_reply
             # return if maximum itertation limit is reached
@@ -175,15 +183,15 @@
                     if (
                         "command" in result
                         and "args" in result["command"]
                         and "response" in result["command"]["args"]
                     ):
                         result = result["command"]["args"]["response"]
                 except json.JSONDecodeError:
-                    result = assistant_reply
+                    result = str(assistant_reply)
 
                 for output_parser in self.output_parsers:
                     result = output_parser.parse_output(result)
 
                 return result
 
             # Get command name and arguments
@@ -247,32 +255,14 @@
     def set_user_input(self, user_input: str):
         result = f"Command UserInput returned: {user_input}"
         assistant_reply = self.logger.get_full_messages()[-1].content
         memory_to_add = f"Assistant Reply: {assistant_reply} " f"\nResult: {result} "
 
         self.memory.add_documents([Document(page_content=memory_to_add)])
 
-    def process_chat_history(self, messages: List[dict]) -> List[BaseMessage]:
-        results = []
-
-        for message in messages:
-            logger.info(message)
-            if message["type"] != "message" and message["type"] != "text":
-                continue
-
-            message_cls = AIMessage if message["user"] == self.ai_id else HumanMessage
-            # replace the at in the message with the name of the bot
-            text = message["text"].replace(f"@{self.ai_id}", f"@{self.ai_name}")
-            # added by JF
-            text = text.split("#verbose", 1)[0]  # remove everything after #verbose
-            text = text.replace("-verbose", "")  # remove -verbose if it exists
-            results.append(message_cls(content=text))
-
-        return results
-
     def process_output(self, output: str) -> str:
         """
         Process the output of the AI to remove the bot's name and replace it with @bot
         """
         for processor in self.output_processors:
             output = processor(output)
         return output
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/tools.py` & `sherpa_ai-0.2.0/sherpa_ai/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 import os
 import re
 import urllib
 import urllib.parse
 import urllib.request
-from typing import Any
+from typing import Any, List, Tuple, Union
+from urllib.parse import urlparse
 
 import requests
 from bs4 import BeautifulSoup
-from langchain import LLMChain
+from langchain.chains import LLMChain
 from langchain.prompts import Prompt
 from langchain.tools import BaseTool
 from langchain.utilities import GoogleSerperAPIWrapper
 from langchain.vectorstores.base import VectorStoreRetriever
 from loguru import logger
 from typing_extensions import Literal
 
 import sherpa_ai.config as cfg
+from sherpa_ai.config.task_config import AgentConfig
+from sherpa_ai.output_parser import TaskAction
 
 
-def get_tools(memory):
+def get_tools(memory, config):
     tools = []
 
     # tools.append(ContextTool(memory=memory))
     tools.append(UserInputTool())
 
     if cfg.SERPER_API_KEY is not None:
-        search_tool = SearchTool()
+        search_tool = SearchTool(config=config)
         tools.append(search_tool)
     else:
         logger.warning(
             "No SERPER_API_KEY found in environment variables, skipping SearchTool"
         )
 
     return tools
 
 
 class SearchArxivTool(BaseTool):
     name = "Arxiv Search"
     description = (
-        "Access all the papers from Arxiv to search for domain-specific scientific publication."
+        "Access all the papers from Arxiv to search for domain-specific scientific publication."  # noqa: E501
         "Only use this tool when you need information in the scientific paper."
     )
 
     def _run(self, query: str) -> str:
         top_k = 10
 
         logger.debug(f"Search query: {query}")
@@ -64,29 +67,74 @@
         result_list = []
         for i in range(len(titles)):
             result_list.append(
                 "Title: " + titles[i] + "\n" + "Summary: " + summaries[i]
             )
 
         logger.debug(f"Arxiv Search Result: {result_list}")
-        
+
         return " ".join(result_list)
 
     def _arun(self, query: str) -> str:
         raise NotImplementedError("SearchArxivTool does not support async run")
 
 
 class SearchTool(BaseTool):
     name = "Search"
+    config = AgentConfig()
+    top_k: int = 10
     description = (
         "Access the internet to search for the information. Only use this tool when "
         "you cannot find the information using internal search."
     )
 
-    def _run(self, query: str) -> str:
+    def _run(
+        self, query: str, require_meta=False
+    ) -> Union[str, Tuple[str, List[dict]]]:
+        result = ""
+        if self.config.search_domains:
+            query_list = [
+                query + " Site: " + str(i) for i in self.config.search_domains
+            ]
+            if len(query_list) >= 5:
+                query_list = query_list[:5]
+                result = (
+                    result
+                    + "Warning: Only the first 5 URLs are taken into consideration.\n"
+                )  # noqa: E501
+        else:
+            query_list = [query]
+        if self.config.invalid_domains:
+            invalid_domain_string = ", ".join(self.config.invalid_domains)
+            result = (
+                result
+                + f"Warning: The doman {invalid_domain_string} is invalid and is not taken into consideration.\n"  # noqa: E501
+            )  # noqa: E501
+
+        top_k = int(self.top_k / len(query_list))
+        if require_meta:
+            meta = []
+
+        for query in query_list:
+            cur_result = self._run_single_query(query, top_k, require_meta)
+
+            if require_meta:
+                result += "\n" + cur_result[0]
+                meta.extend(cur_result[1])
+            else:
+                result += "\n" + cur_result
+
+        if require_meta:
+            result = (result, meta)
+
+        return result
+
+    def _run_single_query(
+        self, query: str, top_k: int, require_meta=False
+    ) -> Union[str, Tuple[str, List[dict]]]:
         logger.debug(f"Search query: {query}")
         google_serper = GoogleSerperAPIWrapper()
         search_results = google_serper._google_serper_api_results(query)
         logger.debug(f"Google Search Result: {search_results}")
 
         # case 1: answerBox in the result dictionary
         if search_results.get("answerBox", False):
@@ -96,54 +144,72 @@
             elif answer_box.get("snippet"):
                 answer = answer_box.get("snippet").replace("\n", " ")
             elif answer_box.get("snippetHighlighted"):
                 answer = answer_box.get("snippetHighlighted")
             title = search_results["organic"][0]["title"]
             link = search_results["organic"][0]["link"]
 
-            return "Answer: " + answer + "\nLink:" + link
+            response = "Answer: " + answer
+            meta = [{"Document": answer, "Source": link}]
+            if require_meta:
+                return response, meta
+            else:
+                return response + "\nLink:" + link
 
         # case 2: knowledgeGraph in the result dictionary
         snippets = []
         if search_results.get("knowledgeGraph", False):
             kg = search_results.get("knowledgeGraph", {})
             title = kg.get("title")
             entity_type = kg.get("type")
             if entity_type:
                 snippets.append(f"{title}: {entity_type}.")
             description = kg.get("description")
             if description:
                 snippets.append(description)
             for attribute, value in kg.get("attributes", {}).items():
                 snippets.append(f"{title} {attribute}: {value}.")
-        k = 10
+
         search_type: Literal["news", "search", "places", "images"] = "search"
         result_key_for_type = {
             "news": "news",
             "places": "places",
             "images": "images",
             "search": "organic",
         }
-        for result in search_results[result_key_for_type[search_type]][:k]:
+
+        # case 3: general search results
+        for result in search_results[result_key_for_type[search_type]][:top_k]:
             if "snippet" in result:
                 snippets.append(result["snippet"])
             for attribute, value in result.get("attributes", {}).items():
                 snippets.append(f"{attribute}: {value}.")
 
             if len(snippets) == 0:
                 return ["No good Google Search Result was found"]
 
         result = []
-        for i in range(len(search_results["organic"][:10])):
+
+        meta = []
+        for i in range(len(search_results["organic"][:top_k])):
             r = search_results["organic"][i]
-            single_result = (
-                "Description: " + r["title"] + r["snippet"] + "\nLink:" + r["link"]
-            )
+            single_result = r["title"] + r["snippet"]
+
+            # If the links are not considered explicitly, add it to the search result
+            # so that it can be considered by the LLM
+            if not require_meta:
+                single_result += "\nLink:" + r["link"]
 
             result.append(single_result)
+            meta.append(
+                {
+                    "Document": "Description: " + r["title"] + r["snippet"],
+                    "Source": r["link"],
+                }
+            )
         full_result = "\n".join(result)
 
         # answer = " ".join(snippets)
         if (
             "knowledgeGraph" in search_results
             and "description" in search_results["knowledgeGraph"]
             and "descriptionLink" in search_results["knowledgeGraph"]
@@ -151,54 +217,68 @@
             answer = (
                 "Description: "
                 + search_results["knowledgeGraph"]["title"]
                 + search_results["knowledgeGraph"]["description"]
                 + "\nLink:"
                 + search_results["knowledgeGraph"]["descriptionLink"]
             )
-            full_result = answer + "\n" + full_result
-        return full_result
+            full_result = answer + "\n\n" + full_result
+        if require_meta:
+            return full_result, meta
+        else:
+            return full_result
 
     def _arun(self, query: str) -> str:
         raise NotImplementedError("SearchTool does not support async run")
 
 
 class ContextTool(BaseTool):
     name = "Context Search"
     description = (
         "Access internal technical documentation for AI related projects, including"
-        + "Fixie, LangChain, GPT index, GPTCache, GPT4ALL, autoGPT, db-GPT, AgentGPT, sherpa."
+        + "Fixie, LangChain, GPT index, GPTCache, GPT4ALL, autoGPT, db-GPT, AgentGPT, sherpa."  # noqa: E501
         + "Only use this tool if you need information for these projects specifically."
     )
     memory: VectorStoreRetriever
 
-    def _run(self, query: str) -> str:
+    def _run(self, query: str, need_meta=False) -> str:
         docs = self.memory.get_relevant_documents(query)
         result = ""
+        metadata = []
         for doc in docs:
             result += (
                 "Document"
                 + doc.page_content
                 + "\nLink:"
                 + doc.metadata.get("source", "")
                 + "\n"
             )
-
-        return result
+            if need_meta:
+                metadata.append(
+                    {
+                        "Document": doc.page_content,
+                        "Source": doc.metadata.get("source", ""),
+                    }
+                )
+
+        if need_meta:
+            return result, metadata
+        else:
+            return result
 
     def _arun(self, query: str) -> str:
         raise NotImplementedError("ContextTool does not support async run")
 
 
 class UserInputTool(BaseTool):
-    # TODO: Make an action for the user input 
+    # TODO: Make an action for the user input
     name = "UserInput"
     description = (
         "Access the user input for the task."
-        "You use this tool if you need more context and would like to ask clarifying questions to solve the task"
+        "You use this tool if you need more context and would like to ask clarifying questions to solve the task"  # noqa: E501
     )
 
     def _run(self, query: str) -> str:
         return input(query)
 
     def _arun(self, query: str) -> str:
         raise NotImplementedError("UserInputTool does not support async run")
```

### Comparing `sherpa_ai-0.1.1/sherpa_ai/verbose_loggers/verbose_loggers.py` & `sherpa_ai-0.2.0/sherpa_ai/verbose_loggers/verbose_loggers.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.1.1/PKG-INFO` & `sherpa_ai-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: sherpa-ai
-Version: 0.1.1
+Version: 0.2.0
 Summary: Sherpa: AI-augmented thinking companion
 Home-page: https://github.com/Aggregate-Intellect/sherpa
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (==4.12.2)
+Requires-Dist: boto3 (>=1.28.77,<2.0.0)
 Requires-Dist: chromadb (>=0.4.8,<0.5.0)
-Requires-Dist: langchain (==0.0.205)
+Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
+Requires-Dist: langchain (==0.0.332)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: markdown (>=3.4.4,<3.5.0)
 Requires-Dist: openai (>=0.28.0,<0.29.0)
 Requires-Dist: pinecone-client (>=2.2.2,<3.0.0)
-Requires-Dist: pypdf2 (>=3.0.1,<4.0.0)
+Requires-Dist: pydantic (>=2.5.3,<3.0.0)
+Requires-Dist: pypdf (>=3.17.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: spacy (>=3.7.4,<4.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: transformers (>=4.35.2,<5.0.0)
 Requires-Dist: unstructured (>=0.10.11,<0.11.0)
+Requires-Dist: word2number (>=1.1,<2.0)
 Project-URL: Repository, https://github.com/Aggregate-Intellect/sherpa
 Description-Content-Type: text/markdown
 
 **To see the documentation, visit: https://sherpa-ai.readthedocs.io/**
```

