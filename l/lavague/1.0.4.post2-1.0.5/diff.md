# Comparing `tmp/lavague-1.0.4.post2.tar.gz` & `tmp/lavague-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague-1.0.4.post2.tar", last modified: Wed Mar 20 00:09:43 2024, max compression
+gzip compressed data, was "lavague-1.0.5.tar", last modified: Thu Apr  4 18:08:05 2024, max compression
```

## Comparing `lavague-1.0.4.post2.tar` & `lavague-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-03-20 00:09:43.287812 lavague-1.0.4.post2/
--rw-rw-r--   0 vscode    (1003) vscode    (1003)    11357 2024-03-13 17:11:17.000000 lavague-1.0.4.post2/LICENSE
--rw-r--r--   0 vscode    (1003) vscode    (1003)    21068 2024-03-20 00:09:43.287812 lavague-1.0.4.post2/PKG-INFO
--rw-rw-r--   0 vscode    (1003) vscode    (1003)     5743 2024-03-19 21:37:36.000000 lavague-1.0.4.post2/README.md
--rw-rw-r--   0 vscode    (1003) vscode    (1003)     2272 2024-03-20 00:09:04.000000 lavague-1.0.4.post2/pyproject.toml
--rw-r--r--   0 vscode    (1003) vscode    (1003)       38 2024-03-20 00:09:43.287812 lavague-1.0.4.post2/setup.cfg
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-03-20 00:09:43.287812 lavague-1.0.4.post2/src/
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-03-20 00:09:43.287812 lavague-1.0.4.post2/src/lavague/
--rw-rw-r--   0 vscode    (1003) vscode    (1003)       82 2024-03-19 21:37:36.000000 lavague-1.0.4.post2/src/lavague/__init__.py
--rw-rw-r--   0 vscode    (1003) vscode    (1003)     4669 2024-03-19 21:37:36.000000 lavague-1.0.4.post2/src/lavague/action_engine.py
--rw-rw-r--   0 vscode    (1003) vscode    (1003)     7481 2024-03-19 21:37:36.000000 lavague-1.0.4.post2/src/lavague/command_center.py
--rw-rw-r--   0 vscode    (1003) vscode    (1003)     3056 2024-03-19 21:37:36.000000 lavague-1.0.4.post2/src/lavague/defaults.py
--rw-rw-r--   0 vscode    (1003) vscode    (1003)    10997 2024-03-19 21:37:36.000000 lavague-1.0.4.post2/src/lavague/prompts.py
-drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-03-20 00:09:43.287812 lavague-1.0.4.post2/src/lavague.egg-info/
--rw-r--r--   0 vscode    (1003) vscode    (1003)    21068 2024-03-20 00:09:43.000000 lavague-1.0.4.post2/src/lavague.egg-info/PKG-INFO
--rw-rw-r--   0 vscode    (1003) vscode    (1003)      336 2024-03-20 00:09:43.000000 lavague-1.0.4.post2/src/lavague.egg-info/SOURCES.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)        1 2024-03-20 00:09:43.000000 lavague-1.0.4.post2/src/lavague.egg-info/dependency_links.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)      850 2024-03-20 00:09:43.000000 lavague-1.0.4.post2/src/lavague.egg-info/requires.txt
--rw-rw-r--   0 vscode    (1003) vscode    (1003)        8 2024-03-20 00:09:43.000000 lavague-1.0.4.post2/src/lavague.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-04 18:08:05.650190 lavague-1.0.5/
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)    11357 2024-03-13 17:11:17.000000 lavague-1.0.5/LICENSE
+-rw-r--r--   0 vscode    (1003) vscode    (1003)    20848 2024-04-04 18:08:05.650190 lavague-1.0.5/PKG-INFO
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     5425 2024-04-04 14:09:01.000000 lavague-1.0.5/README.md
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     2383 2024-04-04 18:07:13.000000 lavague-1.0.5/pyproject.toml
+-rw-r--r--   0 vscode    (1003) vscode    (1003)       38 2024-04-04 18:08:05.650190 lavague-1.0.5/setup.cfg
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-04 18:08:05.650190 lavague-1.0.5/src/
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-04 18:08:05.650190 lavague-1.0.5/src/lavague/
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     4272 2024-04-04 17:28:18.000000 lavague-1.0.5/src/lavague/__init__.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     5555 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/action_engine.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     7157 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/command_center.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     1565 2024-04-04 17:50:35.000000 lavague-1.0.5/src/lavague/defaults.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)      964 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/driver.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)    11308 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/prompts.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)      494 2024-04-04 14:09:01.000000 lavague-1.0.5/src/lavague/telemetry.py
+-rw-r--r--   0 vscode    (1003) vscode    (1003)     1547 2024-04-04 15:30:32.000000 lavague-1.0.5/src/lavague/utils.py
+drwxr-xr-x   0 vscode    (1003) vscode    (1003)        0 2024-04-04 18:08:05.650190 lavague-1.0.5/src/lavague.egg-info/
+-rw-r--r--   0 vscode    (1003) vscode    (1003)    20848 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/PKG-INFO
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)      442 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/SOURCES.txt
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)        1 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1003) vscode    (1003)       80 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/entry_points.txt
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)      893 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/requires.txt
+-rw-rw-r--   0 vscode    (1003) vscode    (1003)        8 2024-04-04 18:08:05.000000 lavague-1.0.5/src/lavague.egg-info/top_level.txt
```

### Comparing `lavague-1.0.4.post2/LICENSE` & `lavague-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague-1.0.4.post2/PKG-INFO` & `lavague-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.4.post2
+Version: 1.0.5
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,49 +216,50 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llama-index==0.10.19
 Requires-Dist: llama-index-agent-openai==0.1.5
 Requires-Dist: llama-index-cli==0.1.9
 Requires-Dist: llama-index-core==0.10.19
 Requires-Dist: llama-index-embeddings-azure-openai==0.1.5
-Requires-Dist: llama-index-embeddings-huggingface==0.1.4
 Requires-Dist: llama-index-embeddings-openai==0.1.6
 Requires-Dist: llama-index-indices-managed-llama-cloud==0.1.4
 Requires-Dist: llama-index-legacy==0.9.48
 Requires-Dist: llama-index-llms-azure-openai==0.1.5
-Requires-Dist: llama-index-llms-huggingface==0.1.4
+Requires-Dist: llama-index-llms-litellm==0.1.4
 Requires-Dist: llama-index-llms-openai==0.1.9
 Requires-Dist: llama-index-multi-modal-llms-openai==0.1.4
 Requires-Dist: llama-index-program-openai==0.1.4
 Requires-Dist: llama-index-question-gen-openai==0.1.3
 Requires-Dist: llama-index-readers-file==0.1.9
 Requires-Dist: llama-index-readers-llama-parse==0.1.3
 Requires-Dist: llama-index-retrievers-bm25==0.1.3
 Requires-Dist: tree-sitter==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: nest_asyncio==1.6.0
 Requires-Dist: selenium==4.18.1
 Requires-Dist: google-search-results==2.4.2
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: accelerate==0.28.0
-Requires-Dist: bitsandbytes==0.42.0
 Requires-Dist: gradio==4.21.0
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Provides-Extra: cuda
+Requires-Dist: accelerate==0.28.0; extra == "cuda"
+Requires-Dist: bitsandbytes==0.42.0; extra == "cuda"
+Provides-Extra: huggingface
+Requires-Dist: llama-index-embeddings-huggingface==0.1.4; extra == "huggingface"
+Requires-Dist: llama-index-llms-huggingface==0.1.4; extra == "huggingface"
 
 <p align="center">
   <a href="https://github.com/lavague-ai/LaVague/stargazers"><img src="https://img.shields.io/github/stars/lavague-ai/LaVague.svg?style=for-the-badge" alt="Stargazers"></a>
   <a href="https://github.com/lavague-ai/LaVague/issues"><img src="https://img.shields.io/github/issues/lavague-ai/LaVague.svg?style=for-the-badge" alt="Issues"></a>
   <a href="https://github.com/lavague-ai/LaVague/network/members"><img src="https://img.shields.io/github/forks/lavague-ai/LaVague.svg?style=for-the-badge" alt="Forks"></a>
   <a href="https://github.com/lavague-ai/LaVague/graphs/contributors"><img src="https://img.shields.io/github/contributors/lavague-ai/LaVague.svg?style=for-the-badge" alt="Contributors"></a>
   <a href="https://github.com/lavague-ai/LaVague/blob/master/LICENSE.md"><img src="https://img.shields.io/github/license/lavague-ai/LaVague.svg?style=for-the-badge" alt="Apache License"></a>
@@ -267,84 +268,83 @@
 
 <div align="center">
   <img src="static/logo.png" width=140px: alt="LaVague Logo">
   <h1>Welcome to LaVague</h1>
 
 <h4 align="center">
  <a href="https://discord.gg/SDxn9KpqX9" target="_blank">
-    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" alt="Join our Discord server!">
+    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" height='35px' alt="Join our Discord server!">
   </a>
-  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" alt="Docs"></a>
+  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" height='35px' alt="Docs"></a>
 </h4>
-  <p>Redefining internet surfing by transforming natural language instructions into seamless browser interactions.</p>
+  <p>Copilot for devs to automate automation</p>
 <h1></h1>
 </div>
 
-## 🏄‍♀️ See LaVague in Action
+## 🏄‍♀️  What is LaVague?
 
-Here are examples to show how LaVague can execute natural instructions on a browser to automate interactions with a website:
+LaVague is an open-source project designed to automate automation for devs! By turning natural language queries into Python code leveraging Selenium, LaVague is designed to make it easy for users to automate express web workflows and execute them on a browser.
+
+### LaVague in Action
+
+Here's an examples to show how LaVague can execute natural lanaguge instructions on a browser to automate interactions with a website:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
 </div>
 
+## 🚀 Getting Started
 
-<div>
-  <figure>
-    <img src="static/irs_lavague.gif" alt="LaVague Workflow Example">
-    <figcaption><b>LaVague interacting with the IRS's website.</b></figcaption>
-  </figure>
-  <br>
-</div>
-
-## 🎯 Motivations
-
-LaVague is designed to automate menial tasks on behalf of its users. Many of these tasks are repetitive, time-consuming, and require little to no cognitive effort. By automating these tasks, LaVague aims to free up time for more meaningful endeavors, allowing users to focus on what truly matters to them.
-
-By providing an engine turning natural language queries into Selenium code, LaVague is designed to make it easy for users or other AIs to automate easily express web workflows and execute them on a browser.
+### Running LaVague in your local env
 
-One of the key usages we see is to automate tasks that are personal to users and require them to be logged in, for instance automating the process of paying bills, filling out forms or pulling data from specific websites. 
+You can get started with `LaVague` in 2 steps:
 
-LaVague is built on open-source projects and leverages open-sources models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
+1. Install LaVague & dependencies
+```
+wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
+sudo bash setup.sh
+```
+
+2. Run your LaVague command!
+```
+lavague-build --file_path tests/hf.txt --config_file examples/api/openai.py
+```
 
-## ✨ Features
+For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
 
-- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
-- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
-- **Open-Source**: Built on open-source projects such as transformers and llama-index, and leverages open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
-- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
-- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query, as directly dropping the full HTML code would not fit in context. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM (``Nous-Hermes-2-Mixtral-8x7B-DPO``) for code generation.
-
-## 🚀 Getting Started
-
-You can try LaVague in the following Colab notebook:
+## 🙋 Contributing
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lavague-ai/LaVague/blob/main/docs/docs/get-started/quick-tour.ipynb)
+We would love your help in making La Vague a reality. 
 
-## 🗺️ Roadmap
+To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
-This is an early project but could grow to democratize transparent and aligned AI models to undertake actions for the sake of users on the internet.
+1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
+2) 🙋‍♀️ If you are interested in working on one of these tasks, comment on the issue! 
+3) 🤝 We will discuss with you and assign you the task with a [`community assigned`](https://github.com/lavague-ai/LaVague/labels/community-assigned) label 
+4) 💬 We will then be available to discuss this task with you
+5) ⬆️ You should submit your work as a PR
+6) ✅ We will review & merge your code or request changes/give feedback
 
-We see the following key areas to explore:
-- Fine-tune local models like a ``gemma-7b-it`` to be expert in Text2Action 
-- Improve retrieval to make sure only relevant pieces of code are used for code generation
-- Support other browser engines (playwright) or even other automation frameworks
+Please check out our [`contributing guide`](./contributing.md) for a more detailed guide.
 
-Keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
+If you want to ask questions, contribute, or have proposals, please come on our [`Discord`](https://discord.gg/SDxn9KpqX9) to chat!
 
-## 🙋 Contributing
 
-We would love your help in making La Vague a reality. 
+## ✨ Features
 
-Please check out our [contributing guide](./contributing.md) to see how you can get involved!
+- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
+- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
+- **Open-Source**: Built on open-source projects such as transformers and llama-index, and compatible with open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
+- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
+- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM for code generation.
 
-If you are interested by this project, want to ask questions, contribute, or have proposals, please come on our [Discord](https://discord.gg/SDxn9KpqX9) to chat!
+## 🗺️ Roadmap
 
-### Set up your dev environment
+TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
-Install the chrome browser and driver on linux with ```bash install-dependencies.sh```. You will need admin privileges if you're missing system dependencies.
+### 🚨 Disclaimer
 
-Set up a development environment by running the following command in a virtual environment: ```pip install -e .[dev]```
+This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

### Comparing `lavague-1.0.4.post2/README.md` & `lavague-1.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,84 +9,83 @@
 
 <div align="center">
   <img src="static/logo.png" width=140px: alt="LaVague Logo">
   <h1>Welcome to LaVague</h1>
 
 <h4 align="center">
  <a href="https://discord.gg/SDxn9KpqX9" target="_blank">
-    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" alt="Join our Discord server!">
+    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" height='35px' alt="Join our Discord server!">
   </a>
-  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" alt="Docs"></a>
+  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" height='35px' alt="Docs"></a>
 </h4>
-  <p>Redefining internet surfing by transforming natural language instructions into seamless browser interactions.</p>
+  <p>Copilot for devs to automate automation</p>
 <h1></h1>
 </div>
 
-## 🏄‍♀️ See LaVague in Action
+## 🏄‍♀️  What is LaVague?
 
-Here are examples to show how LaVague can execute natural instructions on a browser to automate interactions with a website:
+LaVague is an open-source project designed to automate automation for devs! By turning natural language queries into Python code leveraging Selenium, LaVague is designed to make it easy for users to automate express web workflows and execute them on a browser.
+
+### LaVague in Action
+
+Here's an examples to show how LaVague can execute natural lanaguge instructions on a browser to automate interactions with a website:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
 </div>
 
+## 🚀 Getting Started
 
-<div>
-  <figure>
-    <img src="static/irs_lavague.gif" alt="LaVague Workflow Example">
-    <figcaption><b>LaVague interacting with the IRS's website.</b></figcaption>
-  </figure>
-  <br>
-</div>
-
-## 🎯 Motivations
-
-LaVague is designed to automate menial tasks on behalf of its users. Many of these tasks are repetitive, time-consuming, and require little to no cognitive effort. By automating these tasks, LaVague aims to free up time for more meaningful endeavors, allowing users to focus on what truly matters to them.
-
-By providing an engine turning natural language queries into Selenium code, LaVague is designed to make it easy for users or other AIs to automate easily express web workflows and execute them on a browser.
+### Running LaVague in your local env
 
-One of the key usages we see is to automate tasks that are personal to users and require them to be logged in, for instance automating the process of paying bills, filling out forms or pulling data from specific websites. 
+You can get started with `LaVague` in 2 steps:
 
-LaVague is built on open-source projects and leverages open-sources models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
+1. Install LaVague & dependencies
+```
+wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
+sudo bash setup.sh
+```
+
+2. Run your LaVague command!
+```
+lavague-build --file_path tests/hf.txt --config_file examples/api/openai.py
+```
 
-## ✨ Features
+For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
 
-- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
-- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
-- **Open-Source**: Built on open-source projects such as transformers and llama-index, and leverages open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
-- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
-- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query, as directly dropping the full HTML code would not fit in context. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM (``Nous-Hermes-2-Mixtral-8x7B-DPO``) for code generation.
-
-## 🚀 Getting Started
-
-You can try LaVague in the following Colab notebook:
+## 🙋 Contributing
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lavague-ai/LaVague/blob/main/docs/docs/get-started/quick-tour.ipynb)
+We would love your help in making La Vague a reality. 
 
-## 🗺️ Roadmap
+To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
-This is an early project but could grow to democratize transparent and aligned AI models to undertake actions for the sake of users on the internet.
+1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
+2) 🙋‍♀️ If you are interested in working on one of these tasks, comment on the issue! 
+3) 🤝 We will discuss with you and assign you the task with a [`community assigned`](https://github.com/lavague-ai/LaVague/labels/community-assigned) label 
+4) 💬 We will then be available to discuss this task with you
+5) ⬆️ You should submit your work as a PR
+6) ✅ We will review & merge your code or request changes/give feedback
 
-We see the following key areas to explore:
-- Fine-tune local models like a ``gemma-7b-it`` to be expert in Text2Action 
-- Improve retrieval to make sure only relevant pieces of code are used for code generation
-- Support other browser engines (playwright) or even other automation frameworks
+Please check out our [`contributing guide`](./contributing.md) for a more detailed guide.
 
-Keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
+If you want to ask questions, contribute, or have proposals, please come on our [`Discord`](https://discord.gg/SDxn9KpqX9) to chat!
 
-## 🙋 Contributing
 
-We would love your help in making La Vague a reality. 
+## ✨ Features
 
-Please check out our [contributing guide](./contributing.md) to see how you can get involved!
+- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
+- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
+- **Open-Source**: Built on open-source projects such as transformers and llama-index, and compatible with open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
+- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
+- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM for code generation.
 
-If you are interested by this project, want to ask questions, contribute, or have proposals, please come on our [Discord](https://discord.gg/SDxn9KpqX9) to chat!
+## 🗺️ Roadmap
 
-### Set up your dev environment
+TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
-Install the chrome browser and driver on linux with ```bash install-dependencies.sh```. You will need admin privileges if you're missing system dependencies.
+### 🚨 Disclaimer
 
-Set up a development environment by running the following command in a virtual environment: ```pip install -e .[dev]```
+This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

#### html2text {}

```diff
@@ -1,58 +1,54 @@
            _[_S_t_a_r_g_a_z_e_r_s_]_[_I_s_s_u_e_s_]_[_F_o_r_k_s_]_[_C_o_n_t_r_i_b_u_t_o_r_s_]_[_A_p_a_c_h_e_ _L_i_c_e_n_s_e_]
                                 [LaVague Logo]
                        ************ WWeellccoommee ttoo LLaaVVaagguuee ************
                    ****** _[[_JJ_oo_ii_nn_ _oo_uu_rr_ _DD_ii_ss_cc_oo_rr_dd_ _ss_ee_rr_vv_ee_rr_!!_]]_[[_DD_oo_cc_ss_]] ******
-Redefining internet surfing by transforming natural language instructions into
-                        seamless browser interactions.
-## ðââï¸ See LaVague in Action Here are examples to show how LaVague
-can execute natural instructions on a browser to automate interactions with a
-website:
+                    Copilot for devs to automate automation
+## ðââï¸ What is LaVague? LaVague is an open-source project designed to
+automate automation for devs! By turning natural language queries into Python
+code leveraging Selenium, LaVague is designed to make it easy for users to
+automate express web workflows and execute them on a browser. ### LaVague in
+Action Here's an examples to show how LaVague can execute natural lanaguge
+instructions on a browser to automate interactions with a website:
 [LaVague Interaction Example]LLaaVVaagguuee iinntteerraaccttiinngg wwiitthh HHuuggggiinngg FFaaccee''ss wweebbssiittee..
 
-[LaVague Workflow Example]LLaaVVaagguuee iinntteerraaccttiinngg wwiitthh tthhee IIRRSS''ss wweebbssiittee..
-## ð¯ Motivations LaVague is designed to automate menial tasks on behalf of
-its users. Many of these tasks are repetitive, time-consuming, and require
-little to no cognitive effort. By automating these tasks, LaVague aims to free
-up time for more meaningful endeavors, allowing users to focus on what truly
-matters to them. By providing an engine turning natural language queries into
-Selenium code, LaVague is designed to make it easy for users or other AIs to
-automate easily express web workflows and execute them on a browser. One of the
-key usages we see is to automate tasks that are personal to users and require
-them to be logged in, for instance automating the process of paying bills,
-filling out forms or pulling data from specific websites. LaVague is built on
-open-source projects and leverages open-sources models, either locally or
-remote, to ensure the transparency of the agent and ensures that it is aligned
-with users' interests. ## â¨ Features - **Natural Language Processing**:
-Understands instructions in natural language to perform browser interactions. -
-**Selenium Integration**: Seamlessly integrates with Selenium for automating
-web browsers. - **Open-Source**: Built on open-source projects such as
-transformers and llama-index, and leverages open-source models, either locally
-or remote, to ensure the transparency of the agent and ensures that it is
-aligned with users' interests. - **Local models for privacy and control**:
-Supports local models like ``Gemma-7b`` so that users can fully control their
-AI assistant and have privacy guarantees. - **Advanced AI techniques**: Uses a
-local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the
-most relevant HTML pieces to feed the LLM answering the query, as directly
-dropping the full HTML code would not fit in context. Then leverages Few-shot
-learning and Chain of Thought to elicit the most relevant Selenium code to
-perform the action without having to finetune the LLM (``Nous-Hermes-2-Mixtral-
-8x7B-DPO``) for code generation. ## ð Getting Started You can try LaVague in
-the following Colab notebook: [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/lavague-ai/LaVague/blob/main/docs/docs/get-
-started/quick-tour.ipynb) ## ðºï¸ Roadmap This is an early project but could
-grow to democratize transparent and aligned AI models to undertake actions for
-the sake of users on the internet. We see the following key areas to explore: -
-Fine-tune local models like a ``gemma-7b-it`` to be expert in Text2Action -
-Improve retrieval to make sure only relevant pieces of code are used for code
-generation - Support other browser engines (playwright) or even other
-automation frameworks Keep up to date with our project backlog [here](https://
-github.com/orgs/lavague-ai/projects/1/views/2). ## ð Contributing We would
-love your help in making La Vague a reality. Please check out our [contributing
-guide](./contributing.md) to see how you can get involved! If you are
-interested by this project, want to ask questions, contribute, or have
-proposals, please come on our [Discord](https://discord.gg/SDxn9KpqX9) to chat!
-### Set up your dev environment Install the chrome browser and driver on linux
-with ```bash install-dependencies.sh```. You will need admin privileges if
-you're missing system dependencies. Set up a development environment by running
-the following command in a virtual environment: ```pip install -e .[dev]```
+## ð Getting Started ### Running LaVague in your local env You can get
+started with `LaVague` in 2 steps: 1. Install LaVague & dependencies ``` wget
+https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh && sudo bash
+setup.sh ``` 2. Run your LaVague command! ``` lavague-build --file_path tests/
+hf.txt --config_file examples/api/openai.py ``` For a step-by-step guide or to
+run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/
+latest/docs/get-started/quick-tour/) which will walk you through how to get
+set-up and launch LaVague with our CLI tool. ## ð Contributing We would love
+your help in making La Vague a reality. To avoid having multiple people working
+on the same things & being unable to merge your work, we have outlined the
+following contribution process: 1) ð¢ We outline tasks on our [`backlog`]
+(https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check
+out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/
+labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-
+ai/LaVague/labels/good%20first%20issue) labels 2) ðââï¸ If you are
+interested in working on one of these tasks, comment on the issue! 3) ð¤ We
+will discuss with you and assign you the task with a [`community assigned`]
+(https://github.com/lavague-ai/LaVague/labels/community-assigned) label 4) ð¬
+We will then be available to discuss this task with you 5) â¬ï¸ You should
+submit your work as a PR 6) â We will review & merge your code or request
+changes/give feedback Please check out our [`contributing guide`](./
+contributing.md) for a more detailed guide. If you want to ask questions,
+contribute, or have proposals, please come on our [`Discord`](https://
+discord.gg/SDxn9KpqX9) to chat! ## â¨ Features - **Natural Language
+Processing**: Understands instructions in natural language to perform browser
+interactions. - **Selenium Integration**: Seamlessly integrates with Selenium
+for automating web browsers. - **Open-Source**: Built on open-source projects
+such as transformers and llama-index, and compatible with open-source models,
+either locally or remote, to ensure the transparency of the agent and ensures
+that it is aligned with users' interests. - **Local models for privacy and
+control**: Supports local models like ``Gemma-7b`` so that users can fully
+control their AI assistant and have privacy guarantees. - **Advanced AI
+techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform
+RAG to extract the most relevant HTML pieces to feed the LLM answering the
+query. Then leverages Few-shot learning and Chain of Thought to elicit the most
+relevant Selenium code to perform the action without having to finetune the LLM
+for code generation. ## ðºï¸ Roadmap TO keep up to date with our project
+backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2). ### ð¨
+Disclaimer This project executes LLM-generated code using `exec`. This is not
+considered a safe practice. We therefore recommend taking extra care when using
+LaVague (such as running LaVague in a sandboxed environment)!
```

### Comparing `lavague-1.0.4.post2/pyproject.toml` & `lavague-1.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["pip>=24", "setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lavague"
-version = "1.0.4.post2"
+version = "1.0.5"
 description = "Selenium code generation from text instructions"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["IA", "AI", "selenium", "generation"]
 authors = [
   {name = "Mithril Security", email = "contact@mithrilsecurity.io" }
 ]
 maintainers = [
   {name = "Mithril Security", email = "contact@mithrilsecurity.io" }
@@ -32,38 +32,41 @@
 # hard-fixing all of llama-index subdependencies because they can break at any time
 dependencies = [
   "llama-index==0.10.19",
   "llama-index-agent-openai==0.1.5",
   "llama-index-cli==0.1.9",
   "llama-index-core==0.10.19",
   "llama-index-embeddings-azure-openai==0.1.5",
-  "llama-index-embeddings-huggingface==0.1.4",
   "llama-index-embeddings-openai==0.1.6",
   "llama-index-indices-managed-llama-cloud==0.1.4",
   "llama-index-legacy==0.9.48",
   "llama-index-llms-azure-openai==0.1.5",
-  "llama-index-llms-huggingface==0.1.4",
+  "llama-index-llms-litellm==0.1.4",
   "llama-index-llms-openai==0.1.9",
   "llama-index-multi-modal-llms-openai==0.1.4",
   "llama-index-program-openai==0.1.4",
   "llama-index-question-gen-openai==0.1.3",
   "llama-index-readers-file==0.1.9",
   "llama-index-readers-llama-parse==0.1.3",
   "llama-index-retrievers-bm25==0.1.3",
   "tree-sitter==0.21.0",
   "tree-sitter-languages==1.10.2",
   "nest_asyncio==1.6.0",
   "selenium==4.18.1",
   "google-search-results==2.4.2",
   "python-dotenv==1.0.1",
-  "accelerate==0.28.0",
-  "bitsandbytes==0.42.0",
   "gradio==4.21.0",
 ]
 
 [project.optional-dependencies]
-dev = ["ruff", "ipykernel", "build", "twine"]
+dev = ["ruff", "ipykernel"]
+cuda = ["accelerate==0.28.0", "bitsandbytes==0.42.0"]
+huggingface = ["llama-index-embeddings-huggingface==0.1.4", "llama-index-llms-huggingface==0.1.4"]
 
 [project.urls]
 "Homepage" = "https://mithrilsecurity.io"
 "Bug Reports" = "https://github.com/lavague-ai/LaVague/issues"
 "Source" = "https://github.com/lavague-ai/LaVague/"
+
+[project.scripts]
+lavague-build = "lavague:build"
+lavague-launch = "lavague:launch"
```

### Comparing `lavague-1.0.4.post2/src/lavague/action_engine.py` & `lavague-1.0.5/src/lavague/action_engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,166 @@
-from typing import Callable, Optional
+from typing import Callable, Optional, Generator, Tuple
+from abc import ABC, abstractmethod
 from llama_index.core import Document
 from llama_index.core.node_parser import CodeSplitter
 from llama_index.retrievers.bm25 import BM25Retriever
 from llama_index.core import VectorStoreIndex
 from llama_index.core.query_engine import RetrieverQueryEngine
 from llama_index.core import get_response_synthesizer
 from llama_index.core import PromptTemplate
-from llama_index.core.service_context_elements.llm_predictor import LLMPredictorType
-from llama_index.core.embeddings.utils import EmbedType
+from llama_index.core.base.llms.base import BaseLLM
+from llama_index.core.base.embeddings.base import BaseEmbedding
+from .prompts import DEFAULT_PROMPT
+import requests
 import re
 
 
+class BaseActionEngine(ABC):
+    """
+    Abstract class for ActionEngine
+    """
+
+    @abstractmethod
+    def get_action(self, query: str, html: str) -> str:
+        """
+        Generate the code from a query and an html page, and clean it to extract the code
+
+        Args:
+            query (`str`): Instructions given at the end of the prompt to tell the model what to do on the html page
+            html (`str`): The html page
+
+        Return:
+            `str`: The generated code
+        """
+        pass
+
+    @abstractmethod
+    def get_action_streaming(self, query: str, html: str) -> Generator[str, None, None]:
+        """
+        Generate the code with streaming from a query and an html page (without cleaning)
+
+        Args:
+            query (`str`): Instructions given at the end of the prompt to tell the model what to do on the html page
+            html (`str`): The html page
+
+        Return:
+            `str`: The generated code
+        """
+        pass
+
+
 def extract_first_python_code(markdown_text: str):
     # Pattern to match the first ```python ``` code block
     pattern = r"```python(.*?)```"
 
     # Using re.DOTALL to make '.' match also newlines
     match = re.search(pattern, markdown_text, re.DOTALL)
     if match:
         # Return the first matched group, which is the code inside the ```python ```
         return match.group(1).strip()
     else:
         # Return None if no match is found
         return None
 
 
-class ActionEngine:
+class ActionEngine(BaseActionEngine):
     """
-    ActionEngine levergaes the llm model and the embedding model to output code from the prompt and the html page.
+    ActionEngine leverages the llm model and the embedding model to output code from the prompt and the html page.
 
     Args:
         llm (`LLMPredictorType`):
             The llm that will be used the generate the python code
         embedding (`EmbedType`):
             The embedding model to encode the html page and the prompt
-        prompt (`str`):
-            The initial prompt given to the llm, later completed by chunks of the html page and the query
+        prompt_template (`str`):
+            The prompt_template given to the llm, later completed by chunks of the html page and the query
         cleaning_function (`Callable[[str], Optional[str]]`):
             Function to extract the python code from the llm output
         top_k (`int`):
             The top K relevant chunks from the html page will be used in the final query
         max_chars_pc (`int`):
             A chunk can't be larger than max_chars_pc
-        streaming (`bool`)
     """
 
     def __init__(
         self,
-        llm: LLMPredictorType,
-        embedding: EmbedType,
-        prompt: str,
+        llm: BaseLLM,
+        embedder: BaseEmbedding,
+        prompt_template: str = DEFAULT_PROMPT,
         cleaning_function: Callable[[str], Optional[str]] = extract_first_python_code,
         top_k: int = 3,
         max_chars_pc: int = 1500,
-        streaming: bool = True,
     ):
         self.llm = llm
-        self.embedding = embedding
-        self.prompt = prompt
+        self.embedder = embedder
+        self.prompt_template = prompt_template
         self.cleaning_function = cleaning_function
         self.top_k = top_k
         self.max_chars_pc = max_chars_pc
-        self.streaming = streaming
 
     def _get_index(self, html):
         text_list = [html]
         documents = [Document(text=t) for t in text_list]
 
         splitter = CodeSplitter(
             language="html",
             chunk_lines=40,  # lines per chunk
             chunk_lines_overlap=200,  # lines overlap between chunks
             max_chars=self.max_chars_pc,  # max chars per chunk
         )
         nodes = splitter.get_nodes_from_documents(documents)
         nodes = [node for node in nodes if node.text]
 
-        index = VectorStoreIndex(nodes, embed_model=self.embedding)
+        index = VectorStoreIndex(nodes, embed_model=self.embedder)
 
         return index
 
-    def get_query_engine(self, state):
+    def get_query_engine(
+        self, state: str, streaming: bool = True
+    ) -> RetrieverQueryEngine:
         """
         Get the llama-index query engine
 
         Args:
             state (`str`): The initial html page
+            streaming (`bool`)
 
         Return:
             `RetrieverQueryEngine`
         """
         html = state
         index = self._get_index(html)
 
         retriever = BM25Retriever.from_defaults(
             index=index, similarity_top_k=self.top_k
         )
 
         response_synthesizer = get_response_synthesizer(
-            streaming=self.streaming, llm=self.llm
+            streaming=streaming, llm=self.llm
         )
 
         # assemble query engine
         query_engine = RetrieverQueryEngine(
             retriever=retriever,
             response_synthesizer=response_synthesizer,
         )
 
-        prompt_template = PromptTemplate(self.prompt)
+        prompt_template = PromptTemplate(self.prompt_template)
 
         query_engine.update_prompts(
             {"response_synthesizer:text_qa_template": prompt_template}
         )
 
         return query_engine
 
-    def get_action(self, query: str, html: str):
-        """
-        Generate the code from a query and an html page, only works if streaming=False
-
-        Args:
-            query (`str`): Instructions given at the end of the prompt to tell the model what to do on the html page
-            html (`str`): The html page
-
-        Return:
-            (`str`, `str`): The generated code, and the sources which were used
-        """
+    def get_action(self, query: str, html: str) -> str:
         query_engine = self.get_query_engine(html, streaming=False)
         response = query_engine.query(query)
-        source_nodes = response.get_formatted_sources(
-            self.max_chars_pc
-        )  # HTML sources with which the code was generated
         code = response.response
         code = self.cleaning_function(code)
-        return code, source_nodes
+        return code
+
+    def get_action_streaming(self, query: str, html: str) -> Generator[str, None, None]:
+        query_engine = self.get_query_engine(html, streaming=True)
+        streaming_response = query_engine.query(query)
+        for text in streaming_response.response_gen:
+            yield text
```

### Comparing `lavague-1.0.4.post2/src/lavague/command_center.py` & `lavague-1.0.5/src/lavague/command_center.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,122 @@
 from typing import Optional, List
+from abc import ABC, abstractmethod
 import gradio as gr
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
-from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By  # import used by generated selenium code
 from selenium.webdriver.common.keys import (
     Keys,
-)  # import used by generated selenium code
-from .action_engine import ActionEngine
+)
 
+from .telemetry import send_telemetry
+from .action_engine import BaseActionEngine
+from .driver import AbstractDriver
+import base64
 
-class CommandCenter:
+
+class CommandCenter(ABC):
+    @abstractmethod
+    def init_driver():
+        pass
+
+    @abstractmethod
+    def process_instructions():
+        pass
+
+
+class GradioDemo(CommandCenter):
     """
     CommandCenter allows you to launch a gradio demo powered by selenium and the ActionEngine
 
     Args:
-        chromedriverPath(`str`):
-            The path of the chromedriver executable
-        chromePath (`Optional[str]`):
-            The path of the chrome executable, if not specified, PATH will be used
-        actionEngine (`ActionEngine`):
+        actionEngine (`BaseActionEngine`):
             The action engine, with streaming enabled
+        driver (`AbstractDriver`):
+            The driver
     """
 
     title = """
     <div align="center">
     <h1>🌊 Welcome to LaVague</h1>
     <p>Redefining internet surfing by transforming natural language instructions into seamless browser interactions.</p>
     </div>
     """
 
-    def __init__(
-        self,
-        actionEngine: ActionEngine,
-        chromedriverPath: str,
-        chromePath: Optional[str] = None,
-    ):
+    def __init__(self, actionEngine: BaseActionEngine, driver: AbstractDriver):
         self.actionEngine = actionEngine
-
-        ## Setup chrome options
-        chrome_options = Options()
-        chrome_options.add_argument("--headless")  # Ensure GUI is off
-        chrome_options.add_argument("--no-sandbox")
-        chrome_options.add_argument("--window-size=1600,900")  # Size of screenshots
-        if chromePath is not None:
-            chrome_options.binary_location = chromePath
-        webdriver_service = Service(chromedriverPath)
-        self.driver = webdriver.Chrome(
-            service=webdriver_service, options=chrome_options
-        )
-
-    def __process_url(self):
-        def process_url(url):
-            self.driver.get(url)
-            self.driver.save_screenshot("screenshot.png")
+        self.driver = driver
+        self.base_url = ""
+        self.success = False
+
+    def init_driver(self):
+        def init_driver_impl(url):
+            self.driver.goTo(url)
+            self.driver.getScreenshot("screenshot.png")
             # This function is supposed to fetch and return the image from the URL.
             # Placeholder function: replace with actual image fetching logic.
             return "screenshot.png"
 
-        return process_url
-
-    def __process_instruction(self):
-        def process_instructions(query, url_input):
-            if url_input != self.driver.current_url:
-                self.driver.get(url_input)
-            state = self.driver.page_source
-            query_engine = self.actionEngine.get_query_engine(state)
-            streaming_response = query_engine.query(query)
-
-            source_nodes = streaming_response.get_formatted_sources(
-                self.actionEngine.max_chars_pc
-            )
+        return init_driver_impl
 
+    def process_instructions(self):
+        def process_instructions_impl(query, url_input):
+            if url_input != self.driver.getUrl():
+                self.driver.goTo(url_input)
+            state = self.driver.getHtml()
             response = ""
-
-            for text in streaming_response.response_gen:
+            for text in self.actionEngine.get_action_streaming(query, state):
                 # do something with text as they arrive.
                 response += text
-                yield response, source_nodes
+                yield response
 
-        return process_instructions
+        return process_instructions_impl
+
+    def __telemetry(self):
+        def telemetry(query, code, html):
+            screenshot = b""
+            try:
+                scr = open("screenshot.png", "rb")
+                screenshot = base64.b64encode(scr.read())
+            except:
+                pass
+            send_telemetry(
+                self.actionEngine.llm.metadata.model_name,
+                code,
+                screenshot,
+                html,
+                query,
+                self.driver.getUrl(),
+                "Lavague-Launch",
+                self.success,
+            )
+
+        return telemetry
 
     def __exec_code(self):
         def exec_code(code, full_code):
             code = self.actionEngine.cleaning_function(code)
-            html = self.driver.page_source
-            driver = self.driver  # define driver for exec
+            html = self.driver.getHtml()
+            driver = self.driver.getDriver()  # define driver for exec
             try:
                 exec(code)
                 output = "Successful code execution"
                 status = """<p style="color: green; font-size: 20px; font-weight: bold;">Success!</p>"""
+                self.success = True
                 full_code += code
             except Exception as e:
                 output = f"Error in code execution: {str(e)}"
                 status = """<p style="color: red; font-size: 20px; font-weight: bold;">Failure! Open the Debug tab for more information</p>"""
+                self.success = False
             return output, code, html, status, full_code
 
         return exec_code
 
     def __update_image_display(self):
         def update_image_display():
-            self.driver.save_screenshot("screenshot.png")
-            url = self.driver.current_url
+            self.driver.getScreenshot("screenshot.png")
+            url = self.driver.getUrl()
             return "screenshot.png", url
 
         return update_image_display
 
     def __show_processing_message(self):
         return lambda: "Processing..."
 
@@ -151,45 +162,41 @@
                             label="Enter instructions and press 'Enter' to generate code."
                         )
                         gr.Examples(examples=instructions, inputs=text_area)
             with gr.Tab("Debug"):
                 with gr.Row():
                     with gr.Column():
                         log_display = gr.Textbox(interactive=False, lines=20)
-                    with gr.Column():
-                        source_display = gr.Code(
-                            language="html",
-                            label="Retrieved nodes",
-                            interactive=False,
-                            lines=20,
-                        )
                 with gr.Row():
                     with gr.Accordion(label="Full HTML", open=False):
                         full_html = gr.Code(
                             language="html",
                             label="Full HTML",
                             interactive=False,
                             lines=20,
                         )
 
             # Linking components
             url_input.submit(
-                self.__process_url(),
+                self.init_driver(),
                 inputs=[url_input],
                 outputs=[image_display],
             )
             text_area.submit(
                 self.__show_processing_message(), outputs=[status_html]
             ).then(
-                self.__process_instruction(),
+                self.process_instructions(),
                 inputs=[text_area, url_input],
-                outputs=[code_display, source_display],
+                outputs=[code_display],
             ).then(
                 self.__exec_code(),
                 inputs=[code_display, full_code],
                 outputs=[log_display, code_display, full_html, status_html, full_code],
             ).then(
                 self.__update_image_display(),
                 inputs=[],
                 outputs=[image_display, url_input],
+            ).then(
+                self.__telemetry(),
+                inputs=[text_area, code_display, full_html],
             )
         demo.launch(server_port=server_port, share=True, debug=True)
```

### Comparing `lavague-1.0.4.post2/src/lavague/prompts.py` & `lavague-1.0.5/src/lavague/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 DEFAULT_PROMPT = '''
 Your goal is to write Selenium code to answer queries.
 
 Your answer must be a Python markdown only.
 You can have access to external websites and libraries.
 
+Don't assume attribute values are unique, try use the combination of text content and class or ID if available to more precisely target the element.
+Even if there is mutliple elements doing the same action, choose the most relevant and target it precisely.
+Don’t forget to use contains@class if multi-class.
+
 You can assume the following code has been executed:
 ```python
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 driver = webdriver.Firefox()
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,12 +1,17 @@
 DEFAULT_PROMPT = ''' Your goal is to write Selenium code to answer queries.
 Your answer must be a Python markdown only. You can have access to external
-websites and libraries. You can assume the following code has been executed:
-```python from selenium import webdriver from selenium.webdriver.common.by
-import By driver = webdriver.Firefox() ``` --- HTML:
+websites and libraries. Don't assume attribute values are unique, try use the
+combination of text content and class or ID if available to more precisely
+target the element. Even if there is mutliple elements doing the same action,
+choose the most relevant and target it precisely. Donât forget to use
+contains@class if multi-class. You can assume the following code has been
+executed: ```python from selenium import webdriver from
+selenium.webdriver.common.by import By driver = webdriver.Firefox() ``` --
+- HTML:
 ************ SSeeaarrcchh PPaaggee EExxaammppllee ************
 [                    ]Search
 Query: Click on the search bar 'Type here to search...', type 'selenium', and
 press the 'Enter' key Completion: ```python # Let's proceed step by step. #
 First we need to identify the component first, then we can click on it. # Based
 on the HTML, the link can be uniquely identified using the ID "searchBar" #
 Let's use this ID with Selenium to identify the link search_bar =
```

### Comparing `lavague-1.0.4.post2/src/lavague.egg-info/PKG-INFO` & `lavague-1.0.5/src/lavague.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.4.post2
+Version: 1.0.5
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,49 +216,50 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llama-index==0.10.19
 Requires-Dist: llama-index-agent-openai==0.1.5
 Requires-Dist: llama-index-cli==0.1.9
 Requires-Dist: llama-index-core==0.10.19
 Requires-Dist: llama-index-embeddings-azure-openai==0.1.5
-Requires-Dist: llama-index-embeddings-huggingface==0.1.4
 Requires-Dist: llama-index-embeddings-openai==0.1.6
 Requires-Dist: llama-index-indices-managed-llama-cloud==0.1.4
 Requires-Dist: llama-index-legacy==0.9.48
 Requires-Dist: llama-index-llms-azure-openai==0.1.5
-Requires-Dist: llama-index-llms-huggingface==0.1.4
+Requires-Dist: llama-index-llms-litellm==0.1.4
 Requires-Dist: llama-index-llms-openai==0.1.9
 Requires-Dist: llama-index-multi-modal-llms-openai==0.1.4
 Requires-Dist: llama-index-program-openai==0.1.4
 Requires-Dist: llama-index-question-gen-openai==0.1.3
 Requires-Dist: llama-index-readers-file==0.1.9
 Requires-Dist: llama-index-readers-llama-parse==0.1.3
 Requires-Dist: llama-index-retrievers-bm25==0.1.3
 Requires-Dist: tree-sitter==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: nest_asyncio==1.6.0
 Requires-Dist: selenium==4.18.1
 Requires-Dist: google-search-results==2.4.2
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: accelerate==0.28.0
-Requires-Dist: bitsandbytes==0.42.0
 Requires-Dist: gradio==4.21.0
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Provides-Extra: cuda
+Requires-Dist: accelerate==0.28.0; extra == "cuda"
+Requires-Dist: bitsandbytes==0.42.0; extra == "cuda"
+Provides-Extra: huggingface
+Requires-Dist: llama-index-embeddings-huggingface==0.1.4; extra == "huggingface"
+Requires-Dist: llama-index-llms-huggingface==0.1.4; extra == "huggingface"
 
 <p align="center">
   <a href="https://github.com/lavague-ai/LaVague/stargazers"><img src="https://img.shields.io/github/stars/lavague-ai/LaVague.svg?style=for-the-badge" alt="Stargazers"></a>
   <a href="https://github.com/lavague-ai/LaVague/issues"><img src="https://img.shields.io/github/issues/lavague-ai/LaVague.svg?style=for-the-badge" alt="Issues"></a>
   <a href="https://github.com/lavague-ai/LaVague/network/members"><img src="https://img.shields.io/github/forks/lavague-ai/LaVague.svg?style=for-the-badge" alt="Forks"></a>
   <a href="https://github.com/lavague-ai/LaVague/graphs/contributors"><img src="https://img.shields.io/github/contributors/lavague-ai/LaVague.svg?style=for-the-badge" alt="Contributors"></a>
   <a href="https://github.com/lavague-ai/LaVague/blob/master/LICENSE.md"><img src="https://img.shields.io/github/license/lavague-ai/LaVague.svg?style=for-the-badge" alt="Apache License"></a>
@@ -267,84 +268,83 @@
 
 <div align="center">
   <img src="static/logo.png" width=140px: alt="LaVague Logo">
   <h1>Welcome to LaVague</h1>
 
 <h4 align="center">
  <a href="https://discord.gg/SDxn9KpqX9" target="_blank">
-    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" alt="Join our Discord server!">
+    <img src="https://img.shields.io/badge/discord-000000?style=for-the-badge&colorB=555" height='35px' alt="Join our Discord server!">
   </a>
-  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" alt="Docs"></a>
+  <a href="https://docs.lavague.ai/en/latest/"><img src="https://img.shields.io/badge/docs-000000?style=for-the-badge&colorB=07f" height='35px' alt="Docs"></a>
 </h4>
-  <p>Redefining internet surfing by transforming natural language instructions into seamless browser interactions.</p>
+  <p>Copilot for devs to automate automation</p>
 <h1></h1>
 </div>
 
-## 🏄‍♀️ See LaVague in Action
+## 🏄‍♀️  What is LaVague?
 
-Here are examples to show how LaVague can execute natural instructions on a browser to automate interactions with a website:
+LaVague is an open-source project designed to automate automation for devs! By turning natural language queries into Python code leveraging Selenium, LaVague is designed to make it easy for users to automate express web workflows and execute them on a browser.
+
+### LaVague in Action
+
+Here's an examples to show how LaVague can execute natural lanaguge instructions on a browser to automate interactions with a website:
 
 <div>
   <figure>
     <img src="static/hf_lavague.gif" alt="LaVague Interaction Example" style="margin-right: 20px;">
     <figcaption><b>LaVague interacting with Hugging Face's website.</b></figcaption>
   </figure>
   <br><br>
 </div>
 
+## 🚀 Getting Started
 
-<div>
-  <figure>
-    <img src="static/irs_lavague.gif" alt="LaVague Workflow Example">
-    <figcaption><b>LaVague interacting with the IRS's website.</b></figcaption>
-  </figure>
-  <br>
-</div>
-
-## 🎯 Motivations
-
-LaVague is designed to automate menial tasks on behalf of its users. Many of these tasks are repetitive, time-consuming, and require little to no cognitive effort. By automating these tasks, LaVague aims to free up time for more meaningful endeavors, allowing users to focus on what truly matters to them.
-
-By providing an engine turning natural language queries into Selenium code, LaVague is designed to make it easy for users or other AIs to automate easily express web workflows and execute them on a browser.
+### Running LaVague in your local env
 
-One of the key usages we see is to automate tasks that are personal to users and require them to be logged in, for instance automating the process of paying bills, filling out forms or pulling data from specific websites. 
+You can get started with `LaVague` in 2 steps:
 
-LaVague is built on open-source projects and leverages open-sources models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
+1. Install LaVague & dependencies
+```
+wget https://raw.githubusercontent.com/lavague-ai/LaVague/main/setup.sh &&
+sudo bash setup.sh
+```
+
+2. Run your LaVague command!
+```
+lavague-build --file_path tests/hf.txt --config_file examples/api/openai.py
+```
 
-## ✨ Features
+For a step-by-step guide or to run LaVague in a Google Colab, see our [quick-tour](https://docs.lavague.ai/en/latest/docs/get-started/quick-tour/) which will walk you through how to get set-up and launch LaVague with our CLI tool.
 
-- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
-- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
-- **Open-Source**: Built on open-source projects such as transformers and llama-index, and leverages open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
-- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
-- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query, as directly dropping the full HTML code would not fit in context. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM (``Nous-Hermes-2-Mixtral-8x7B-DPO``) for code generation.
-
-## 🚀 Getting Started
-
-You can try LaVague in the following Colab notebook:
+## 🙋 Contributing
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lavague-ai/LaVague/blob/main/docs/docs/get-started/quick-tour.ipynb)
+We would love your help in making La Vague a reality. 
 
-## 🗺️ Roadmap
+To avoid having multiple people working on the same things & being unable to merge your work, we have outlined the following contribution process:
 
-This is an early project but could grow to democratize transparent and aligned AI models to undertake actions for the sake of users on the internet.
+1) 📢 We outline tasks on our [`backlog`](https://github.com/orgs/lavague-ai/projects/1/views/3): we recommend you check out issues with the [`help-wanted`](https://github.com/lavague-ai/LaVague/labels/help%20wanted) labels & [`good first issue`](https://github.com/lavague-ai/LaVague/labels/good%20first%20issue) labels
+2) 🙋‍♀️ If you are interested in working on one of these tasks, comment on the issue! 
+3) 🤝 We will discuss with you and assign you the task with a [`community assigned`](https://github.com/lavague-ai/LaVague/labels/community-assigned) label 
+4) 💬 We will then be available to discuss this task with you
+5) ⬆️ You should submit your work as a PR
+6) ✅ We will review & merge your code or request changes/give feedback
 
-We see the following key areas to explore:
-- Fine-tune local models like a ``gemma-7b-it`` to be expert in Text2Action 
-- Improve retrieval to make sure only relevant pieces of code are used for code generation
-- Support other browser engines (playwright) or even other automation frameworks
+Please check out our [`contributing guide`](./contributing.md) for a more detailed guide.
 
-Keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
+If you want to ask questions, contribute, or have proposals, please come on our [`Discord`](https://discord.gg/SDxn9KpqX9) to chat!
 
-## 🙋 Contributing
 
-We would love your help in making La Vague a reality. 
+## ✨ Features
 
-Please check out our [contributing guide](./contributing.md) to see how you can get involved!
+- **Natural Language Processing**: Understands instructions in natural language to perform browser interactions.
+- **Selenium Integration**: Seamlessly integrates with Selenium for automating web browsers.
+- **Open-Source**: Built on open-source projects such as transformers and llama-index, and compatible with open-source models, either locally or remote, to ensure the transparency of the agent and ensures that it is aligned with users' interests.
+- **Local models for privacy and control**: Supports local models like ``Gemma-7b`` so that users can fully control their AI assistant and have privacy guarantees.
+- **Advanced AI techniques**: Uses a local embedding (``bge-small-en-v1.5``) first to perform RAG to extract the most relevant HTML pieces to feed the LLM answering the query. Then leverages Few-shot learning and Chain of Thought to elicit the most relevant Selenium code to perform the action without having to finetune the LLM for code generation.
 
-If you are interested by this project, want to ask questions, contribute, or have proposals, please come on our [Discord](https://discord.gg/SDxn9KpqX9) to chat!
+## 🗺️ Roadmap
 
-### Set up your dev environment
+TO keep up to date with our project backlog [here](https://github.com/orgs/lavague-ai/projects/1/views/2).
 
-Install the chrome browser and driver on linux with ```bash install-dependencies.sh```. You will need admin privileges if you're missing system dependencies.
+### 🚨 Disclaimer
 
-Set up a development environment by running the following command in a virtual environment: ```pip install -e .[dev]```
+This project executes LLM-generated code using `exec`. This is not considered a safe practice. We therefore recommend taking extra care when using LaVague (such as running LaVague in a sandboxed environment)!
```

### Comparing `lavague-1.0.4.post2/src/lavague.egg-info/requires.txt` & `lavague-1.0.5/src/lavague.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 llama-index==0.10.19
 llama-index-agent-openai==0.1.5
 llama-index-cli==0.1.9
 llama-index-core==0.10.19
 llama-index-embeddings-azure-openai==0.1.5
-llama-index-embeddings-huggingface==0.1.4
 llama-index-embeddings-openai==0.1.6
 llama-index-indices-managed-llama-cloud==0.1.4
 llama-index-legacy==0.9.48
 llama-index-llms-azure-openai==0.1.5
-llama-index-llms-huggingface==0.1.4
+llama-index-llms-litellm==0.1.4
 llama-index-llms-openai==0.1.9
 llama-index-multi-modal-llms-openai==0.1.4
 llama-index-program-openai==0.1.4
 llama-index-question-gen-openai==0.1.3
 llama-index-readers-file==0.1.9
 llama-index-readers-llama-parse==0.1.3
 llama-index-retrievers-bm25==0.1.3
 tree-sitter==0.21.0
 tree-sitter-languages==1.10.2
 nest_asyncio==1.6.0
 selenium==4.18.1
 google-search-results==2.4.2
 python-dotenv==1.0.1
+gradio==4.21.0
+
+[cuda]
 accelerate==0.28.0
 bitsandbytes==0.42.0
-gradio==4.21.0
 
 [dev]
 ruff
 ipykernel
-build
-twine
+
+[huggingface]
+llama-index-embeddings-huggingface==0.1.4
+llama-index-llms-huggingface==0.1.4
```

