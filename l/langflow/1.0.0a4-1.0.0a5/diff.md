# Comparing `tmp/langflow-1.0.0a4.tar.gz` & `tmp/langflow-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-1.0.0a4.tar", max compression
+gzip compressed data, was "langflow-1.0.0a5.tar", max compression
```

## Comparing `langflow-1.0.0a4.tar` & `langflow-1.0.0a5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-29 17:29:02.212613 langflow-1.0.0a4/LICENSE
--rw-r--r--   0        0        0     9324 2024-04-02 14:24:00.552315 langflow-1.0.0a4/README.md
--rw-r--r--   0        0        0     3771 2024-04-03 21:26:23.198331 langflow-1.0.0a4/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-02 04:17:58.852217 langflow-1.0.0a4/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      244 2024-04-02 21:46:53.099735 langflow-1.0.0a4/src/backend/langflow/version/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      449 2024-04-02 21:46:53.114509 langflow-1.0.0a4/src/backend/langflow/version/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0      156 2024-04-02 04:17:58.852448 langflow-1.0.0a4/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0    12577 1970-01-01 00:00:00.000000 langflow-1.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-04 05:47:11.670544 langflow-1.0.0a5/LICENSE
+-rw-r--r--   0        0        0     6934 2024-04-04 05:47:11.671417 langflow-1.0.0a5/README.md
+-rw-r--r--   0        0        0     3669 2024-04-04 06:24:20.522524 langflow-1.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-04 05:47:12.068790 langflow-1.0.0a5/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-04 05:52:19.875396 langflow-1.0.0a5/src/backend/langflow/version/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      449 2024-04-04 05:52:19.880207 langflow-1.0.0a5/src/backend/langflow/version/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0      156 2024-04-04 05:47:12.068865 langflow-1.0.0a5/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0    10097 1970-01-01 00:00:00.000000 langflow-1.0.0a5/PKG-INFO
```

### Comparing `langflow-1.0.0a4/LICENSE` & `langflow-1.0.0a5/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Logspace
+Copyright (c) 2024 Logspace
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `langflow-1.0.0a4/pyproject.toml` & `langflow-1.0.0a5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "1.0.0a4"
+version = "1.0.0a5"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Igor Carvalho <igorr.ackerman@gmail.com>",
@@ -19,16 +19,14 @@
 packages = [{ include = "langflow", from = "src/backend" }]
 include = ["src/backend/langflow/*", "src/backend/langflow/**/*"]
 documentation = "https://docs.langflow.org"
 
 [tool.poetry.scripts]
 langflow = "langflow.__main__:main"
 
-[tool.poetry-monorepo-dependency-plugin]
-enable = true
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 langflow-base = "^0.0.18"
 beautifulsoup4 = "^4.12.2"
 google-search-results = "^2.4.1"
 google-api-python-client = "^2.118.0"
@@ -70,18 +68,16 @@
 pgvector = "^0.2.3"
 pyautogen = "^0.2.0"
 langchain-google-genai = "^1.0.1"
 langchain-cohere = "^0.1.0rc1"
 elasticsearch = "^8.12.0"
 pytube = "^15.0.0"
 llama-index = "^0.10.13"
-langchain-openai = "^0.0.5"
 unstructured = { extras = ["md"], version = "^0.12.4" }
 dspy-ai = "^2.4.0"
-crewai = "^0.22.5"
 html2text = "^2024.2.26"
 assemblyai = "^0.23.1"
 litellm = "^1.34.22"
 
 [tool.poetry.group.dev.dependencies]
 types-redis = "^4.6.0.5"
 ipykernel = "^6.29.0"
```

### Comparing `langflow-1.0.0a4/PKG-INFO` & `langflow-1.0.0a5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
@@ -19,30 +19,28 @@
 Provides-Extra: local
 Requires-Dist: assemblyai (>=0.23.1,<0.24.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: boto3 (>=1.34.0,<2.0.0)
 Requires-Dist: celery[redis] (>=5.3.6,<6.0.0) ; extra == "deploy"
 Requires-Dist: certifi (>=2023.11.17,<2024.0.0)
 Requires-Dist: cohere (>=5.1.7,<6.0.0)
-Requires-Dist: crewai (>=0.22.5,<0.23.0)
 Requires-Dist: ctransformers (>=0.2.10,<0.3.0) ; extra == "local"
 Requires-Dist: dspy-ai (>=2.4.0,<3.0.0)
 Requires-Dist: elasticsearch (>=8.12.0,<9.0.0)
 Requires-Dist: extract-msg (>=0.47.0,<0.48.0)
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fake-useragent (>=1.4.0,<2.0.0)
 Requires-Dist: fastavro (>=1.8.0,<2.0.0)
 Requires-Dist: flower (>=2.0.0,<3.0.0) ; extra == "deploy"
 Requires-Dist: google-api-python-client (>=2.118.0,<3.0.0)
 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: huggingface-hub[inference] (>=0.20.0,<0.21.0)
 Requires-Dist: langchain-cohere (>=0.1.0rc1,<0.2.0)
 Requires-Dist: langchain-google-genai (>=1.0.1,<2.0.0)
-Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
 Requires-Dist: langflow-base (>=0.0.18,<0.0.19)
 Requires-Dist: langfuse (>=2.9.0,<3.0.0)
 Requires-Dist: litellm (>=1.34.22,<2.0.0)
 Requires-Dist: llama-cpp-python (>=0.2.0,<0.3.0) ; extra == "local"
 Requires-Dist: llama-index (>=0.10.13,<0.11.0)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
 Requires-Dist: metal-sdk (>=2.5.0,<3.0.0)
@@ -73,75 +71,55 @@
 Project-URL: Repository, https://github.com/logspace-ai/langflow
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD030 -->
 
 # ⛓️ Langflow
 
-<h3>Discover a simpler & smarter way to build around Foundation Models</h3>
+### Discover a simpler & smarter way to build around Foundation Models</h3>
 
-[![Release Notes](https://img.shields.io/github/release/logspace-ai/langflow)](https://github.com/logspace-ai/langflow/releases)
-[![Contributors](https://img.shields.io/github/contributors/logspace-ai/langflow)](https://github.com/logspace-ai/langflow/contributors)
-[![Last Commit](https://img.shields.io/github/last-commit/logspace-ai/langflow)](https://github.com/logspace-ai/langflow/last-commit)
-[![Open Issues](https://img.shields.io/github/issues-raw/logspace-ai/langflow)](https://github.com/logspace-ai/langflow/issues)
-[![LRepo-size](https://img.shields.io/github/repo-size/logspace-ai/langflow)](https://github.com/logspace-ai/langflow/repo-size)
-[![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/logspace-ai/langflow)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![GitHub star chart](https://img.shields.io/github/stars/logspace-ai/langflow?style=social)](https://star-history.com/#logspace-ai/langflow)
-[![GitHub fork](https://img.shields.io/github/forks/logspace-ai/langflow?style=social)](https://github.com/logspace-ai/langflow/fork)
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/langflow_ai.svg?style=social&label=Follow%20%40langflow_ai)](https://twitter.com/langflow_ai)
-[![](https://dcbadge.vercel.app/api/server/EqksyE2EX9?compact=true&style=flat)](https://discord.com/invite/EqksyE2EX9)
-[![HuggingFace Spaces](https://huggingface.co/datasets/huggingface/badges/raw/main/duplicate-this-space-md.svg)](https://huggingface.co/spaces/Logspace/Langflow-Preview?duplicate=true)
-[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/logspace-ai/langflow)
-
-<a href="https://github.com/logspace-ai/langflow">
-<img width="100%" src="https://github.com/logspace-ai/langflow/blob/dev/docs/static/img/new_langflow_demo.gif"></a>
+# [![Langflow](https://github.com/logspace-ai/langflow/blob/dev/docs/static/img/new_langflow_demo.gif)](https://www.langflow.org)
 
 # 📦 Installation
 
-### <b>Locally</b>
-
-Make sure you have Python 3.10 installed on your system.
-
-You can install Langflow from pip:
+You can install Langflow with pip:
 
 ```shell
-# This installs the package without dependencies for local models
-pip install langflow
+# Install the pre-release version
+pip install langflow --pre --force-reinstall
+
+# or stable version
+pip install langflow -U
 ```
 
-To use local models (e.g llama-cpp-python) run:
+Then, run Langflow with:
 
 ```shell
-pip install langflow[local]
+python -m langflow run
+# or
+langflow run
 ```
 
-This will install the following dependencies:
-
-- [CTransformers](https://github.com/marella/ctransformers)
-- [llama-cpp-python](https://github.com/abetlen/llama-cpp-python)
-- [sentence-transformers](https://github.com/UKPLab/sentence-transformers)
+You can also preview Langflow in [HuggingFace Spaces](https://huggingface.co/spaces/Logspace/Langflow-Preview). [Clone the space using this link](https://huggingface.co/spaces/Logspace/Langflow-Preview?duplicate=true), to create your own Langflow workspace in minutes.
 
-You can still use models from projects like LocalAI, Ollama, LM Studio, Jan and others.
+# 🎨 Creating Flows
 
-Next, run:
+Creating flows with Langflow is easy. Simply drag components from the sidebar onto the canvas and connect them to start building your application.
 
-```shell
-python -m langflow run
-```
+Explore by editing prompt parameters, grouping components into a single high-level component, and building your own Custom Components.
 
-or
+Once you’re done, you can export your flow as a JSON file.
 
-```shell
-langflow run # or langflow --help
-```
+Load the flow with:
 
-### HuggingFace Spaces
+```python
+from langflow.load import run_flow_from_json
 
-You can also check it out on HuggingFace Spaces and run it in your browser for free! [Click here to duplicate the Space](https://huggingface.co/spaces/Logspace/Langflow-Preview?duplicate=true)
+results = run_flow_from_json("path/to/flow.json", input_value="Hello, World!")
+```
 
 # 🖥️ Command Line Interface (CLI)
 
 Langflow provides a command-line interface (CLI) for easy management and configuration.
 
 ## Usage
 
@@ -197,32 +175,14 @@
 
 ## Deploy on Render
 
 <a href="https://render.com/deploy?repo=https://github.com/logspace-ai/langflow/tree/main">
 <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render" />
 </a>
 
-# 🎨 Creating Flows
-
-Creating flows with Langflow is easy. Simply drag components from the sidebar onto the canvas and connect them to start building your application.
-
-Explore by editing prompt parameters, grouping components into a single high-level component, and building your own Custom Components.
-
-Once you’re done, you can export your flow as a JSON file.
-
-Load the flow with:
-
-```python
-from langflow import load_flow_from_json
-
-flow = load_flow_from_json("path/to/flow.json")
-# Now you can use it
-flow("Hey, have you heard of Langflow?")
-```
-
 # 👋 Contributing
 
 We welcome contributions from developers of all levels to our open-source project on GitHub. If you'd like to contribute, please check our [contributing guidelines](./CONTRIBUTING.md) and help make Langflow more accessible.
 
 Join our [Discord](https://discord.com/invite/EqksyE2EX9) server to ask questions, make suggestions, and showcase your projects! 🦾
 
 ---
```

