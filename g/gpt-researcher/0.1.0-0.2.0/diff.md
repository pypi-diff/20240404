# Comparing `tmp/gpt-researcher-0.1.0.tar.gz` & `tmp/gpt-researcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.1.0.tar", last modified: Wed Mar 20 15:56:09 2024, max compression
+gzip compressed data, was "gpt-researcher-0.2.0.tar", last modified: Thu Apr  4 09:18:12 2024, max compression
```

## Comparing `gpt-researcher-0.1.0.tar` & `gpt-researcher-0.2.0.tar`

### file list

```diff
@@ -1,75 +1,96 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.835390 gpt-researcher-0.1.0/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2023-08-18 12:11:22.000000 gpt-researcher-0.1.0/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    12243 2024-03-20 15:56:09.833709 gpt-researcher-0.1.0/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    11530 2024-03-20 15:51:50.000000 gpt-researcher-0.1.0/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.767928 gpt-researcher-0.1.0/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.1.0/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.775616 gpt-researcher-0.1.0/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.1.0/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2046 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.780054 gpt-researcher-0.1.0/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.1.0/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1706 2023-11-19 07:06:28.000000 gpt-researcher-0.1.0/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.1.0/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.784655 gpt-researcher-0.1.0/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.1.0/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     5501 2024-03-05 16:41:59.000000 gpt-researcher-0.1.0/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)     7600 2024-03-17 08:29:46.000000 gpt-researcher-0.1.0/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)     7763 2023-12-18 08:18:37.000000 gpt-researcher-0.1.0/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.787191 gpt-researcher-0.1.0/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.1.0/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      827 2024-03-17 08:29:46.000000 gpt-researcher-0.1.0/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.788867 gpt-researcher-0.1.0/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.790712 gpt-researcher-0.1.0/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.792294 gpt-researcher-0.1.0/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2023-11-13 18:29:19.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.794416 gpt-researcher-0.1.0/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.796554 gpt-researcher-0.1.0/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1284 2023-11-19 07:01:11.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.799743 gpt-researcher-0.1.0/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.801810 gpt-researcher-0.1.0/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.803841 gpt-researcher-0.1.0/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1473 2024-01-03 12:37:34.000000 gpt-researcher-0.1.0/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.810593 gpt-researcher-0.1.0/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.813981 gpt-researcher-0.1.0/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.817864 gpt-researcher-0.1.0/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.819931 gpt-researcher-0.1.0/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.821937 gpt-researcher-0.1.0/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.826945 gpt-researcher-0.1.0/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.1.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.831791 gpt-researcher-0.1.0/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.1.0/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     4597 2023-11-13 18:29:19.000000 gpt-researcher-0.1.0/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)     2462 2023-12-18 08:18:37.000000 gpt-researcher-0.1.0/gpt_researcher/utils/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-03-20 15:56:09.773778 gpt-researcher-0.1.0/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    12243 2024-03-20 15:56:09.000000 gpt-researcher-0.1.0/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     1970 2024-03-20 15:56:09.000000 gpt-researcher-0.1.0/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-03-20 15:56:09.000000 gpt-researcher-0.1.0/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      253 2024-03-20 15:56:09.000000 gpt-researcher-0.1.0/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       15 2024-03-20 15:56:09.000000 gpt-researcher-0.1.0/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)      892 2024-03-05 16:41:59.000000 gpt-researcher-0.1.0/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-03-20 15:56:09.835702 gpt-researcher-0.1.0/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1166 2024-03-20 15:54:07.000000 gpt-researcher-0.1.0/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.253180 gpt-researcher-0.2.0/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    12547 2024-04-04 09:18:12.252490 gpt-researcher-0.2.0/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    11824 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.205573 gpt-researcher-0.2.0/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.0/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.210380 gpt-researcher-0.2.0/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.0/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2101 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.212787 gpt-researcher-0.2.0/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.0/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.0/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.213781 gpt-researcher-0.2.0/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.215222 gpt-researcher-0.2.0/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2526 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.216696 gpt-researcher-0.2.0/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.218234 gpt-researcher-0.2.0/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.222356 gpt-researcher-0.2.0/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.0/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     8604 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12120 2024-04-01 16:02:57.000000 gpt-researcher-0.2.0/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12175 2024-04-01 16:15:31.000000 gpt-researcher-0.2.0/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.224475 gpt-researcher-0.2.0/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.0/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.225284 gpt-researcher-0.2.0/gpt_researcher/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.226657 gpt-researcher-0.2.0/gpt_researcher/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.227955 gpt-researcher-0.2.0/gpt_researcher/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6033 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/detailed_report/detailed_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.228973 gpt-researcher-0.2.0/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.230415 gpt-researcher-0.2.0/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.231881 gpt-researcher-0.2.0/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2023-11-13 18:29:19.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.233419 gpt-researcher-0.2.0/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.234848 gpt-researcher-0.2.0/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.236022 gpt-researcher-0.2.0/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.237553 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.239021 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.240840 gpt-researcher-0.2.0/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.242324 gpt-researcher-0.2.0/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.243746 gpt-researcher-0.2.0/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.245148 gpt-researcher-0.2.0/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.246366 gpt-researcher-0.2.0/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.247619 gpt-researcher-0.2.0/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.251357 gpt-researcher-0.2.0/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     4851 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/utils/validators.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2872 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/utils/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.208930 gpt-researcher-0.2.0/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    12547 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2629 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      322 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       15 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1150 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-04 09:18:12.253338 gpt-researcher-0.2.0/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-04 09:17:55.000000 gpt-researcher-0.2.0/setup.py
```

### Comparing `gpt-researcher-0.1.0/LICENSE` & `gpt-researcher-0.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Assaf Elovic
+Copyright (c) 2024 Assaf Elovic
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gpt-researcher-0.1.0/PKG-INFO` & `gpt-researcher-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.1.0
+Version: 0.2.0
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
-Author: Tavily
-Author-email: support@tavily.com
+Author: Assaf Elovic
+Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -66,19 +66,20 @@
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
 - 📝 Generate research, outlines, resources and lessons reports
+- 📜 Can generate long and detailed research reports (over 2K words)
 - 🌐 Aggregates over 20 web sources per research to form objective and factual conclusions
 - 🖥️ Includes an easy-to-use web interface (HTML/CSS/JS)
 - 🔍 Scrapes web sources with javascript support
 - 📂 Keeps track and context of visited and used web sources
-- 📄 Export research reports to PDF and more...
+- 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - How-To examples (demos, integrations, docker support)
@@ -163,17 +164,16 @@
 For a more permanent setup, create a `.env` file in the current `gpt-researcher` folder and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. Follow [this guide](https://python.langchain.com/docs/integrations/llms/) to learn how to integrate LLMs with Langchain. 
-- **For search engine, we recommend [Tavily Search API](https://app.tavily.com) (optimized for LLMs)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
-- **We highly recommend using [OpenAI GPT](https://platform.openai.com/docs/guides/gpt) models and [Tavily Search API](https://app.tavily.com) for optimal performance.**
+- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
+- **For search engine, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
 
 <br />
 
 > **Step 5** - Launch the FastAPI application agent on a *Virtual Environment or Poetry* setup by executing the following command:
 ```bash
 python -m uvicorn main:app --reload
 ```
@@ -187,21 +187,33 @@
 To learn how to get started with Docker or to learn more about the features and services check out the [documentation](https://docs.tavily.com) page.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
+## ✉️ Support / Contact us
+- [Community Discord](https://discord.gg/spBgZmm3Xe)
+- Our email: assafelovic@gmail.com
+
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
 1. The whole point of our scraping system is to reduce incorrect fact. How? The more sites we scrape the less chances of incorrect data. We are scraping 20 per research, the chances that they are all wrong is extremely low.
 2. We do not aim to eliminate biases; we aim to reduce it as much as possible. **We are here as a community to figure out the most effective human/llm interactions.**
 3. In research, people also tend towards biases as most have already opinions on the topics they research about. This tool scrapes many opinions and will evenly explain diverse views that a biased person would never have read.
 
 **Please note that the use of the GPT-4 language model can be expensive due to its token usage.** By utilizing this project, you acknowledge that you are responsible for monitoring and managing your own token usage and the associated costs. It is highly recommended to check your OpenAI API usage regularly and set up any necessary limits or alerts to prevent unexpected charges.
 
-## ✉️ Support / Contact us
-- [Community Discord](https://discord.gg/spBgZmm3Xe)
-- Our email: assafelovic@gmail.com
+---
+
+<p align="center">
+<a href="https://star-history.com/#assafelovic/gpt-researcher">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date&theme=dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date" />
+    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date" />
+  </picture>
+</a>
+</p>
```

### Comparing `gpt-researcher-0.1.0/README.md` & `gpt-researcher-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,20 @@
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
 - 📝 Generate research, outlines, resources and lessons reports
+- 📜 Can generate long and detailed research reports (over 2K words)
 - 🌐 Aggregates over 20 web sources per research to form objective and factual conclusions
 - 🖥️ Includes an easy-to-use web interface (HTML/CSS/JS)
 - 🔍 Scrapes web sources with javascript support
 - 📂 Keeps track and context of visited and used web sources
-- 📄 Export research reports to PDF and more...
+- 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - How-To examples (demos, integrations, docker support)
@@ -145,17 +146,16 @@
 For a more permanent setup, create a `.env` file in the current `gpt-researcher` folder and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. Follow [this guide](https://python.langchain.com/docs/integrations/llms/) to learn how to integrate LLMs with Langchain. 
-- **For search engine, we recommend [Tavily Search API](https://app.tavily.com) (optimized for LLMs)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
-- **We highly recommend using [OpenAI GPT](https://platform.openai.com/docs/guides/gpt) models and [Tavily Search API](https://app.tavily.com) for optimal performance.**
+- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
+- **For search engine, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
 
 <br />
 
 > **Step 5** - Launch the FastAPI application agent on a *Virtual Environment or Poetry* setup by executing the following command:
 ```bash
 python -m uvicorn main:app --reload
 ```
@@ -169,21 +169,33 @@
 To learn how to get started with Docker or to learn more about the features and services check out the [documentation](https://docs.tavily.com) page.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
+## ✉️ Support / Contact us
+- [Community Discord](https://discord.gg/spBgZmm3Xe)
+- Our email: assafelovic@gmail.com
+
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
 1. The whole point of our scraping system is to reduce incorrect fact. How? The more sites we scrape the less chances of incorrect data. We are scraping 20 per research, the chances that they are all wrong is extremely low.
 2. We do not aim to eliminate biases; we aim to reduce it as much as possible. **We are here as a community to figure out the most effective human/llm interactions.**
 3. In research, people also tend towards biases as most have already opinions on the topics they research about. This tool scrapes many opinions and will evenly explain diverse views that a biased person would never have read.
 
 **Please note that the use of the GPT-4 language model can be expensive due to its token usage.** By utilizing this project, you acknowledge that you are responsible for monitoring and managing your own token usage and the associated costs. It is highly recommended to check your OpenAI API usage regularly and set up any necessary limits or alerts to prevent unexpected charges.
 
-## ✉️ Support / Contact us
-- [Community Discord](https://discord.gg/spBgZmm3Xe)
-- Our email: assafelovic@gmail.com
+---
+
+<p align="center">
+<a href="https://star-history.com/#assafelovic/gpt-researcher">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date&theme=dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date" />
+    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date" />
+  </picture>
+</a>
+</p>
```

### Comparing `gpt-researcher-0.1.0/gpt_researcher/config/config.py` & `gpt-researcher-0.2.0/gpt_researcher/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """Config class for GPT Researcher."""
 
     def __init__(self, config_file: str = None):
         """Initialize the config class."""
         self.config_file = config_file if config_file else os.getenv('CONFIG_FILE')
         self.retriever = os.getenv('SEARCH_RETRIEVER', "tavily")
         self.embedding_provider = os.getenv('EMBEDDING_PROVIDER', 'openai')
-        self.llm_provider = os.getenv('LLM_PROVIDER', "ChatOpenAI")
+        self.llm_provider = os.getenv('LLM_PROVIDER', "openai")
         self.fast_llm_model = os.getenv('FAST_LLM_MODEL', "gpt-3.5-turbo-16k")
         self.smart_llm_model = os.getenv('SMART_LLM_MODEL', "gpt-4-1106-preview")
         self.fast_token_limit = int(os.getenv('FAST_TOKEN_LIMIT', 2000))
         self.smart_token_limit = int(os.getenv('SMART_TOKEN_LIMIT', 4000))
         self.browse_chunk_max_length = int(os.getenv('BROWSE_CHUNK_MAX_LENGTH', 8192))
         self.summary_token_limit = int(os.getenv('SUMMARY_TOKEN_LIMIT', 700))
         self.temperature = float(os.getenv('TEMPERATURE', 0.55))
@@ -24,14 +24,15 @@
         self.max_search_results_per_query = int(os.getenv('MAX_SEARCH_RESULTS_PER_QUERY', 5))
         self.memory_backend = os.getenv('MEMORY_BACKEND', "local")
         self.total_words = int(os.getenv('TOTAL_WORDS', 1000))
         self.report_format = os.getenv('REPORT_FORMAT', "APA")
         self.max_iterations = int(os.getenv('MAX_ITERATIONS', 3))
         self.agent_role = os.getenv('AGENT_ROLE', None)
         self.scraper = os.getenv("SCRAPER", "bs")
+        self.max_subtopics = os.getenv("MAX_SUBTOPICS", 3)
 
         self.load_config_file()
 
     def load_config_file(self) -> None:
         """Load the config file."""
         if self.config_file is None:
             return None
```

### Comparing `gpt-researcher-0.1.0/gpt_researcher/context/compression.py` & `gpt-researcher-0.2.0/gpt_researcher/context/compression.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 
 class ContextCompressor:
     def __init__(self, documents, embeddings, max_results=5, **kwargs):
         self.max_results = max_results
         self.documents = documents
         self.kwargs = kwargs
         self.embeddings = embeddings
+        self.similarity_threshold = 0.38
 
     def _get_contextual_retriever(self):
         splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=100)
-        relevance_filter = EmbeddingsFilter(embeddings=self.embeddings, similarity_threshold=0.78)
+        relevance_filter = EmbeddingsFilter(embeddings=self.embeddings,
+                                            similarity_threshold=self.similarity_threshold)
         pipeline_compressor = DocumentCompressorPipeline(
             transformers=[splitter, relevance_filter]
         )
         base_retriever = SearchAPIRetriever(
             pages=self.documents
         )
         contextual_retriever = ContextualCompressionRetriever(
```

### Comparing `gpt-researcher-0.1.0/gpt_researcher/context/retriever.py` & `gpt-researcher-0.2.0/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/master/prompts.py` & `gpt-researcher-0.2.0/gpt_researcher/master/prompts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from datetime import datetime
+from datetime import datetime, timezone
+
+from gpt_researcher.utils.enum import ReportType
 
 
 def generate_search_queries_prompt(question, max_iterations=3):
     """ Generates the search queries prompt for the given question.
     Args: question (str): The question to generate the search queries prompt for
     Returns: str: The search queries prompt for the given question
     """
 
-    return f'Write {max_iterations} google search queries to search online that form an objective opinion from the following: "{question}"' \
+    return f'Write {max_iterations} google search queries to search online that form an objective opinion from the following task: "{question}"' \
            f'Use the current date if needed: {datetime.now().strftime("%B %d, %Y")}.\n' \
+           f'Also include in the queries specified task details such as locations, names, etc.\n' \
            f'You must respond with a list of strings in the following format: ["query 1", "query 2", "query 3"].'
 
 
 def generate_report_prompt(question, context, report_format="apa", total_words=1000):
     """ Generates the report prompt for the given question and research summary.
     Args: question (str): The question to generate the report prompt for
             research_summary (str): The research summary to generate the report prompt for
@@ -25,15 +28,24 @@
            " The report should focus on the answer to the query, should be well structured, informative," \
            f" in depth and comprehensive, with facts and numbers if available and a minimum of {total_words} words.\n" \
            "You should strive to write the report as long as you can using all relevant and necessary information provided.\n" \
            "You must write the report with markdown syntax.\n " \
            f"Use an unbiased and journalistic tone. \n" \
            "You MUST determine your own concrete and valid opinion based on the given information. Do NOT deter to general and meaningless conclusions.\n" \
            f"You MUST write all used source urls at the end of the report as references, and make sure to not add duplicated sources, but only one reference for each.\n" \
-           f"You MUST write the report in {report_format} format.\n " \
+           "Every url should be hyperlinked: [url website](url)"\
+           """
+            Additionally, you MUST include hyperlinks to the relevant URLs wherever they are referenced in the report : 
+        
+            eg:    
+                # Report Header
+                
+                This is a sample text. ([url website](url))
+            """\
+            f"You MUST write the report in {report_format} format.\n " \
             f"Cite search results using inline notations. Only cite the most \
             relevant results that answer the query accurately. Place these citations at the end \
             of the sentence or paragraph that reference them.\n"\
             f"Please do your best, this is very important to my career. " \
             f"Assume that the current date is {datetime.now().strftime('%B %d, %Y')}"
 
 
@@ -50,15 +62,17 @@
     return f'"""{context}"""\n\nBased on the above information, generate a bibliography recommendation report for the following' \
            f' question or topic: "{question}". The report should provide a detailed analysis of each recommended resource,' \
            ' explaining how each source can contribute to finding answers to the research question.\n' \
            'Focus on the relevance, reliability, and significance of each source.\n' \
            'Ensure that the report is well-structured, informative, in-depth, and follows Markdown syntax.\n' \
            'Include relevant facts, figures, and numbers whenever available.\n' \
            'The report should have a minimum length of 700 words.\n' \
-            'You MUST include all relevant source urls.'
+        'You MUST include all relevant source urls.'\
+        'Every url should be hyperlinked: [url website](url)'
+
 
 def generate_custom_report_prompt(query_prompt, context, report_format="apa", total_words=1000):
     return f'"{context}"\n\n{query_prompt}'
 
 
 def generate_outline_report_prompt(question, context, report_format="apa", total_words=1000):
     """ Generates the outline report prompt for the given question and research summary.
@@ -72,18 +86,19 @@
            ' for the research report, including the main sections, subsections, and key points to be covered.' \
            ' The research report should be detailed, informative, in-depth, and a minimum of 1,200 words.' \
            ' Use appropriate Markdown syntax to format the outline and ensure readability.'
 
 
 def get_report_by_type(report_type):
     report_type_mapping = {
-        'research_report': generate_report_prompt,
-        'resource_report': generate_resource_report_prompt,
-        'outline_report': generate_outline_report_prompt,
-        'custom_report': generate_custom_report_prompt
+        ReportType.ResearchReport.value: generate_report_prompt,
+        ReportType.ResourceReport.value: generate_resource_report_prompt,
+        ReportType.OutlineReport.value: generate_outline_report_prompt,
+        ReportType.CustomReport.value: generate_custom_report_prompt,
+        ReportType.SubtopicReport.value: generate_subtopic_report_prompt
     }
     return report_type_mapping[report_type]
 
 
 def auto_agent_instructions():
     return """
         This task involves researching a given topic, regardless of its complexity or the availability of a definitive answer. The research is conducted by a specific server, defined by its type and role, with each server requiring distinct instructions.
@@ -107,18 +122,102 @@
         response:
         {
             "server:  "🌍 Travel Agent",
             "agent_role_prompt": "You are a world-travelled AI tour guide assistant. Your main purpose is to draft engaging, insightful, unbiased, and well-structured travel reports on given locations, including history, attractions, and cultural insights."
         }
     """
 
+
 def generate_summary_prompt(query, data):
     """ Generates the summary prompt for the given question and text.
     Args: question (str): The question to generate the summary prompt for
             text (str): The text to generate the summary prompt for
     Returns: str: The summary prompt for the given question and text
     """
 
     return f'{data}\n Using the above text, summarize it based on the following task or query: "{query}".\n If the ' \
            f'query cannot be answered using the text, YOU MUST summarize the text in short.\n Include all factual ' \
            f'information such as numbers, stats, quotes, etc if available. '
 
+
+################################################################################################
+
+# DETAILED REPORT PROMPTS
+
+def generate_subtopics_prompt() -> str:
+    return """
+                Provided the main topic:
+                
+                {task}
+                
+                and research data:
+                
+                {data}
+                
+                - Construct a list of subtopics which indicate the headers of a report document to be generated on the task. 
+                - These are a possible list of subtopics : {subtopics}.
+                - There should NOT be any duplicate subtopics.
+                - Limit the number of subtopics to a maximum of {max_subtopics}
+                - Finally order the subtopics by their tasks, in a relevant and meaningful order which is presentable in a detailed report
+                
+                "IMPORTANT!":
+                - Every subtopic MUST be relevant to the main topic and provided research data ONLY!
+                
+                {format_instructions}
+            """
+
+
+def generate_subtopic_report_prompt(
+    current_subtopic,
+    existing_headers,
+    main_topic,
+    context,
+    report_format="apa",
+    total_words=1000,
+) -> str:
+
+    return f"""
+    "Context":
+    "{context}"
+    
+    "Main Topic and Subtopic":
+    Using the latest information available, construct a detailed report on the subtopic: {current_subtopic} under the main topic: {main_topic}.
+    You must limit the number of subsections to a maximum of 5.
+    
+    "Content Focus":
+    - The report should focus on answering the question, be well-structured, informative, in-depth, and include facts and numbers if available.
+    - Use markdown syntax and follow the {report_format.upper()} format.
+    
+    "Structure and Formatting":
+    - As this sub-report will be part of a larger report, include only the main body divided into suitable subtopics without any introduction, conclusion, or reference section.
+    
+    - Include hyperlinks to relevant URLs wherever referenced in the report, for example:
+    
+        # Report Header
+        
+        This is a sample text. ([url website](url))
+    
+    "Existing Subtopic Reports":
+    - This is a list of existing subtopic reports and their section headers:
+    
+        {existing_headers}.
+    
+    - Do not use any of the above headers or related details to avoid duplicates. Use smaller Markdown headers (e.g., H2 or H3) for content structure, avoiding the largest header (H1) as it will be used for the larger report's heading.
+    
+    "Date":
+    Assume the current date is {datetime.now(timezone.utc).strftime('%B %d, %Y')} if required.
+    
+    "IMPORTANT!":
+    - The focus MUST be on the main topic! You MUST Leave out any information un-related to it!
+    - Must NOT have any introduction, conclusion, summary or reference section.
+    """
+
+
+def generate_report_introduction(question: str, research_summary: str = "") -> str:
+    return f"""{research_summary}\n 
+        Using the above latest information, Prepare a detailed report introduction on the topic -- {question}.
+        - The introduction should be succinct, well-structured, informative with markdown syntax.
+        - As this introduction will be part of a larger report, do NOT include any other sections, which are generally present in a report.
+        - The introduction should be preceded by an H1 heading with a suitable topic for the entire report.
+        - You must include hyperlinks with markdown syntax ([url website](url)) related to the sentences wherever necessary.
+        Assume that the current date is {datetime.now(timezone.utc).strftime('%B %d, %Y')} if required.
+    """
```

### Comparing `gpt-researcher-0.1.0/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.2.0/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.2.0/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.2.0/gpt_researcher/retrievers/searx/searx.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tavily API Retriever
 
 # libraries
 import os
 from tavily import TavilyClient
-from langchain.utilities import SearxSearchWrapper
+from langchain_community.utilities import SearxSearchWrapper
 
 
 class SearxSearch():
     """
     Tavily API Retriever
     """
     def __init__(self, query):
```

### Comparing `gpt-researcher-0.1.0/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.2.0/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,10 +42,11 @@
         """
         try:
             # Search the query
             results = self.client.search(self.query, search_depth="advanced", max_results=max_results)
             # Return the results
             search_response = [{"href": obj["url"], "body": obj["content"]} for obj in results.get("results", [])]
         except Exception as e: # Fallback in case overload on Tavily Search API
+            print(f"Error: {e}")
             ddg = DDGS()
             search_response = ddg.text(self.query, region='wt-wt', max_results=max_results)
         return search_response
```

### Comparing `gpt-researcher-0.1.0/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.2.0/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.2.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.2.0/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.2.0/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.2.0/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.2.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.1.0/gpt_researcher/utils/websocket_manager.py` & `gpt-researcher-0.2.0/gpt_researcher/utils/websocket_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # connect any client to gpt-researcher using websocket
 import asyncio
 import datetime
-from typing import List, Dict
+from typing import Dict, List
+
 from fastapi import WebSocket
-from gpt_researcher.master.agent import GPTResearcher
+
+from gpt_researcher.report_type import BasicReport, DetailedReport
+
+from .enum import ReportType
 
 
 class WebSocketManager:
     """Manage websockets"""
+
     def __init__(self):
         """Initialize the WebSocketManager class."""
         self.active_connections: List[WebSocket] = []
         self.sender_tasks: Dict[WebSocket, asyncio.Task] = {}
         self.message_queues: Dict[WebSocket, asyncio.Queue] = {}
 
     async def start_sender(self, websocket: WebSocket):
@@ -31,15 +36,16 @@
                 break
 
     async def connect(self, websocket: WebSocket):
         """Connect a websocket."""
         await websocket.accept()
         self.active_connections.append(websocket)
         self.message_queues[websocket] = asyncio.Queue()
-        self.sender_tasks[websocket] = asyncio.create_task(self.start_sender(websocket))
+        self.sender_tasks[websocket] = asyncio.create_task(
+            self.start_sender(websocket))
 
     async def disconnect(self, websocket: WebSocket):
         """Disconnect a websocket."""
         if websocket in self.active_connections:
             self.active_connections.remove(websocket)
             self.sender_tasks[websocket].cancel()
             await self.message_queues[websocket].put(None)
@@ -54,15 +60,21 @@
 
 async def run_agent(task, report_type, websocket):
     """Run the agent."""
     # measure time
     start_time = datetime.datetime.now()
     # add customized JSON config file path here
     config_path = None
-    # run agent
-    researcher = GPTResearcher(query=task, report_type=report_type, source_urls=None, config_path=config_path, websocket=websocket)
+    # Instead of running the agent directly run it through the different report type classes
+    if report_type == ReportType.DetailedReport.value:
+        researcher = DetailedReport(query=task, report_type=report_type,
+                                    source_urls=None, config_path=config_path, websocket=websocket)
+    else:
+        researcher = BasicReport(query=task, report_type=report_type,
+                                 source_urls=None, config_path=config_path, websocket=websocket)
+
     report = await researcher.run()
     # measure time
     end_time = datetime.datetime.now()
     await websocket.send_json({"type": "logs", "output": f"\nTotal run time: {end_time - start_time}\n"})
 
     return report
```

### Comparing `gpt-researcher-0.1.0/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.2.0/gpt_researcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.1.0
+Version: 0.2.0
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
-Author: Tavily
-Author-email: support@tavily.com
+Author: Assaf Elovic
+Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -66,19 +66,20 @@
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
 - 📝 Generate research, outlines, resources and lessons reports
+- 📜 Can generate long and detailed research reports (over 2K words)
 - 🌐 Aggregates over 20 web sources per research to form objective and factual conclusions
 - 🖥️ Includes an easy-to-use web interface (HTML/CSS/JS)
 - 🔍 Scrapes web sources with javascript support
 - 📂 Keeps track and context of visited and used web sources
-- 📄 Export research reports to PDF and more...
+- 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - How-To examples (demos, integrations, docker support)
@@ -163,17 +164,16 @@
 For a more permanent setup, create a `.env` file in the current `gpt-researcher` folder and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. Follow [this guide](https://python.langchain.com/docs/integrations/llms/) to learn how to integrate LLMs with Langchain. 
-- **For search engine, we recommend [Tavily Search API](https://app.tavily.com) (optimized for LLMs)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
-- **We highly recommend using [OpenAI GPT](https://platform.openai.com/docs/guides/gpt) models and [Tavily Search API](https://app.tavily.com) for optimal performance.**
+- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
+- **For search engine, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search engines of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"googleSerp"`, or `"searx"`. Then add the corresponding env API key as seen in the config.py file.
 
 <br />
 
 > **Step 5** - Launch the FastAPI application agent on a *Virtual Environment or Poetry* setup by executing the following command:
 ```bash
 python -m uvicorn main:app --reload
 ```
@@ -187,21 +187,33 @@
 To learn how to get started with Docker or to learn more about the features and services check out the [documentation](https://docs.tavily.com) page.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
+## ✉️ Support / Contact us
+- [Community Discord](https://discord.gg/spBgZmm3Xe)
+- Our email: assafelovic@gmail.com
+
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
 1. The whole point of our scraping system is to reduce incorrect fact. How? The more sites we scrape the less chances of incorrect data. We are scraping 20 per research, the chances that they are all wrong is extremely low.
 2. We do not aim to eliminate biases; we aim to reduce it as much as possible. **We are here as a community to figure out the most effective human/llm interactions.**
 3. In research, people also tend towards biases as most have already opinions on the topics they research about. This tool scrapes many opinions and will evenly explain diverse views that a biased person would never have read.
 
 **Please note that the use of the GPT-4 language model can be expensive due to its token usage.** By utilizing this project, you acknowledge that you are responsible for monitoring and managing your own token usage and the associated costs. It is highly recommended to check your OpenAI API usage regularly and set up any necessary limits or alerts to prevent unexpected charges.
 
-## ✉️ Support / Contact us
-- [Community Discord](https://discord.gg/spBgZmm3Xe)
-- Our email: assafelovic@gmail.com
+---
+
+<p align="center">
+<a href="https://star-history.com/#assafelovic/gpt-researcher">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date&theme=dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date" />
+    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=assafelovic/gpt-researcher&type=Date" />
+  </picture>
+</a>
+</p>
```

### Comparing `gpt-researcher-0.1.0/setup.py` & `gpt-researcher-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,23 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.1.0",
+    version="0.2.0",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
-    author="Tavily",
-    author_email="support@tavily.com",
+    author="Assaf Elovic",
+    author_email="assaf.elovic@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3.11",
```

