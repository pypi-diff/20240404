# Comparing `tmp/whyhow-0.0.1.tar.gz` & `tmp/whyhow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyhow-0.0.1.tar", last modified: Thu Apr  4 07:21:21 2024, max compression
+gzip compressed data, was "whyhow-0.0.2.tar", last modified: Thu Apr  4 07:55:43 2024, max compression
```

## Comparing `whyhow-0.0.1.tar` & `whyhow-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:21:21.237704 whyhow-0.0.1/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6018 2024-04-04 07:21:21.237484 whyhow-0.0.1/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)     4899 2024-04-04 05:49:16.000000 whyhow-0.0.1/README.md
--rw-r--r--   0 tomsmoker   (501) staff       (20)     2051 2024-04-04 07:21:18.000000 whyhow-0.0.1/pyproject.toml
--rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-04-04 07:21:21.237751 whyhow-0.0.1/setup.cfg
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:21:21.231955 whyhow-0.0.1/src/
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:21:21.233173 whyhow-0.0.1/src/whyhow/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-04-04 07:18:35.000000 whyhow-0.0.1/src/whyhow/__init__.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:21:21.235085 whyhow-0.0.1/src/whyhow/apis/
--rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.1/src/whyhow/apis/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.1/src/whyhow/apis/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     3866 2024-04-04 07:11:07.000000 whyhow-0.0.1/src/whyhow/apis/graph.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-04 07:04:26.000000 whyhow-0.0.1/src/whyhow/client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.1/src/whyhow/exceptions.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.1/src/whyhow/py.typed
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:21:21.235882 whyhow-0.0.1/src/whyhow/schemas/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.1/src/whyhow/schemas/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.1/src/whyhow/schemas/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     3755 2024-04-04 06:49:03.000000 whyhow-0.0.1/src/whyhow/schemas/common.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1289 2024-04-04 07:02:16.000000 whyhow-0.0.1/src/whyhow/schemas/graph.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:21:21.236450 whyhow-0.0.1/src/whyhow.egg-info/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6018 2024-04-04 07:21:21.000000 whyhow-0.0.1/src/whyhow.egg-info/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-04-04 07:21:21.000000 whyhow-0.0.1/src/whyhow.egg-info/SOURCES.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-04-04 07:21:21.000000 whyhow-0.0.1/src/whyhow.egg-info/dependency_links.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.1/src/whyhow.egg-info/not-zip-safe
--rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-04-04 07:21:21.000000 whyhow-0.0.1/src/whyhow.egg-info/requires.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-04-04 07:21:21.000000 whyhow-0.0.1/src/whyhow.egg-info/top_level.txt
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:21:21.236277 whyhow-0.0.1/tests/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1395 2024-04-04 07:15:22.000000 whyhow-0.0.1/tests/test_client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.1/tests/test_dummy.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.759480 whyhow-0.0.2/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5447 2024-04-04 07:55:43.759234 whyhow-0.0.2/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     4318 2024-04-04 07:54:08.000000 whyhow-0.0.2/README.md
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-04-04 07:43:46.000000 whyhow-0.0.2/pyproject.toml
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-04-04 07:55:43.759559 whyhow-0.0.2/setup.cfg
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.754414 whyhow-0.0.2/src/
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.755426 whyhow-0.0.2/src/whyhow/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-04-04 07:55:05.000000 whyhow-0.0.2/src/whyhow/__init__.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.756852 whyhow-0.0.2/src/whyhow/apis/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/apis/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.2/src/whyhow/apis/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     3866 2024-04-04 07:11:07.000000 whyhow-0.0.2/src/whyhow/apis/graph.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-04 07:04:26.000000 whyhow-0.0.2/src/whyhow/client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/exceptions.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/py.typed
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.757432 whyhow-0.0.2/src/whyhow/schemas/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/schemas/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.2/src/whyhow/schemas/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     3755 2024-04-04 06:49:03.000000 whyhow-0.0.2/src/whyhow/schemas/common.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1289 2024-04-04 07:02:16.000000 whyhow-0.0.2/src/whyhow/schemas/graph.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.758074 whyhow-0.0.2/src/whyhow.egg-info/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5447 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/SOURCES.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/dependency_links.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.2/src/whyhow.egg-info/not-zip-safe
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/requires.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-04-04 07:55:43.000000 whyhow-0.0.2/src/whyhow.egg-info/top_level.txt
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-04-04 07:55:43.757778 whyhow-0.0.2/tests/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1395 2024-04-04 07:15:22.000000 whyhow-0.0.2/tests/test_client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.2/tests/test_dummy.py
```

### Comparing `whyhow-0.0.1/PKG-INFO` & `whyhow-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.1
-Summary: Whyhow KG SDK
+Version: 0.0.2
+Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -30,15 +30,15 @@
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pymdown-extensions; extra == "docs"
 
 # WhyHow Knowledge Graph Creation SDK
 
 [![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
-[![PyPI Version](https://img.shields.io/pypi/v/whyhow-knowledge-graph)](https://pypi.org/project/whyhow-knowledge-graph/)
+[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/why/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](https://mypy-lang.org/)
 [![Whyhow Discord](https://dcbadge.vercel.app/api/server/9bWqrsxgHr?compact=true&style=flat)](https://discord.gg/9bWqrsxgHr)
 
 The WhyHow Knowledge Graph Creation SDK enables you to quickly and easily build automated knowledge graphs tailored to your unique worldview. Instantly build, extend, and query well-scoped KGs using a raw PDF and simple seed concepts in natural language. This version leverages OpenAI for embeddings and NLP, Pinecone serverless for scalable vector search and storage, and Neo4j for graph data storage and management.
 
 # Installation
@@ -136,26 +136,10 @@
 
 query_response = client.graph.query_graph(namespace, query)
 print(query_response)
 # {answer: "Harry wears a cloak, glasses, robe, and Dudley's old clothes.", cypher_query: "MATCH (:Entity {name: "Harry"})-[:WEARS]->(clothing:Entity)\nRETURN clothing;"}
 
 ```
 
-# Contributing
-
-We welcome contributions to improve the Rule-based Retrieval package! If you have any ideas, bug reports, or feature requests, please open an issue on the GitHub repository.
-
-If you'd like to contribute code, please follow these steps:
-
-1. Fork the repository
-2. Create a new branch for your feature or bug fix
-3. Make your changes and commit them with descriptive messages
-4. Push your changes to your forked repository
-5. Open a pull request to the main repository
-
-### License
-
-This project is licensed under the MIT License.
-
 ### Support
 
 WhyHow.AI is building tools to help developers bring more determinism and control to their RAG pipelines using graph structures. If you're thinking about, in the process of, or have already incorporated knowledge graphs in RAG, we’d love to chat at team@whyhow.ai, or follow our newsletter at [WhyHow.AI](https://www.whyhow.ai/). Join our discussions about rules, determinism and knowledge graphs in RAG on our [Discord](https://discord.com/invite/9bWqrsxgHr).
```

### Comparing `whyhow-0.0.1/README.md` & `whyhow-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # WhyHow Knowledge Graph Creation SDK
 
 [![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
-[![PyPI Version](https://img.shields.io/pypi/v/whyhow-knowledge-graph)](https://pypi.org/project/whyhow-knowledge-graph/)
+[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/why/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](https://mypy-lang.org/)
 [![Whyhow Discord](https://dcbadge.vercel.app/api/server/9bWqrsxgHr?compact=true&style=flat)](https://discord.gg/9bWqrsxgHr)
 
 The WhyHow Knowledge Graph Creation SDK enables you to quickly and easily build automated knowledge graphs tailored to your unique worldview. Instantly build, extend, and query well-scoped KGs using a raw PDF and simple seed concepts in natural language. This version leverages OpenAI for embeddings and NLP, Pinecone serverless for scalable vector search and storage, and Neo4j for graph data storage and management.
 
 # Installation
@@ -104,26 +104,10 @@
 
 query_response = client.graph.query_graph(namespace, query)
 print(query_response)
 # {answer: "Harry wears a cloak, glasses, robe, and Dudley's old clothes.", cypher_query: "MATCH (:Entity {name: "Harry"})-[:WEARS]->(clothing:Entity)\nRETURN clothing;"}
 
 ```
 
-# Contributing
-
-We welcome contributions to improve the Rule-based Retrieval package! If you have any ideas, bug reports, or feature requests, please open an issue on the GitHub repository.
-
-If you'd like to contribute code, please follow these steps:
-
-1. Fork the repository
-2. Create a new branch for your feature or bug fix
-3. Make your changes and commit them with descriptive messages
-4. Push your changes to your forked repository
-5. Open a pull request to the main repository
-
-### License
-
-This project is licensed under the MIT License.
-
 ### Support
 
 WhyHow.AI is building tools to help developers bring more determinism and control to their RAG pipelines using graph structures. If you're thinking about, in the process of, or have already incorporated knowledge graphs in RAG, we’d love to chat at team@whyhow.ai, or follow our newsletter at [WhyHow.AI](https://www.whyhow.ai/). Join our discussions about rules, determinism and knowledge graphs in RAG on our [Discord](https://discord.com/invite/9bWqrsxgHr).
```

### Comparing `whyhow-0.0.1/pyproject.toml` & `whyhow-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "whyhow"
 authors = [
     {name = "Tom Smoker", email = "tom@whyhow.ai"},
     {name = "Chris Rec", email = "chris@whyhow.ai"}
 ]
-description = "Whyhow KG SDK"
+description = "Whyhow automated KG SDK"
 keywords = ["SDK", "KG"]
 classifiers = ["Programming Language :: Python :: 3"]
 requires-python = ">=3.10"
 dependencies = [
     "httpx",
     "pydantic>1",
 ]
```

### Comparing `whyhow-0.0.1/src/whyhow/apis/graph.py` & `whyhow-0.0.2/src/whyhow/apis/graph.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.1/src/whyhow/client.py` & `whyhow-0.0.2/src/whyhow/client.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.1/src/whyhow/schemas/base.py` & `whyhow-0.0.2/src/whyhow/schemas/base.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.1/src/whyhow/schemas/common.py` & `whyhow-0.0.2/src/whyhow/schemas/common.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.1/src/whyhow/schemas/graph.py` & `whyhow-0.0.2/src/whyhow/schemas/graph.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.1/src/whyhow.egg-info/PKG-INFO` & `whyhow-0.0.2/src/whyhow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.1
-Summary: Whyhow KG SDK
+Version: 0.0.2
+Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -30,15 +30,15 @@
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pymdown-extensions; extra == "docs"
 
 # WhyHow Knowledge Graph Creation SDK
 
 [![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
-[![PyPI Version](https://img.shields.io/pypi/v/whyhow-knowledge-graph)](https://pypi.org/project/whyhow-knowledge-graph/)
+[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/why/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](https://mypy-lang.org/)
 [![Whyhow Discord](https://dcbadge.vercel.app/api/server/9bWqrsxgHr?compact=true&style=flat)](https://discord.gg/9bWqrsxgHr)
 
 The WhyHow Knowledge Graph Creation SDK enables you to quickly and easily build automated knowledge graphs tailored to your unique worldview. Instantly build, extend, and query well-scoped KGs using a raw PDF and simple seed concepts in natural language. This version leverages OpenAI for embeddings and NLP, Pinecone serverless for scalable vector search and storage, and Neo4j for graph data storage and management.
 
 # Installation
@@ -136,26 +136,10 @@
 
 query_response = client.graph.query_graph(namespace, query)
 print(query_response)
 # {answer: "Harry wears a cloak, glasses, robe, and Dudley's old clothes.", cypher_query: "MATCH (:Entity {name: "Harry"})-[:WEARS]->(clothing:Entity)\nRETURN clothing;"}
 
 ```
 
-# Contributing
-
-We welcome contributions to improve the Rule-based Retrieval package! If you have any ideas, bug reports, or feature requests, please open an issue on the GitHub repository.
-
-If you'd like to contribute code, please follow these steps:
-
-1. Fork the repository
-2. Create a new branch for your feature or bug fix
-3. Make your changes and commit them with descriptive messages
-4. Push your changes to your forked repository
-5. Open a pull request to the main repository
-
-### License
-
-This project is licensed under the MIT License.
-
 ### Support
 
 WhyHow.AI is building tools to help developers bring more determinism and control to their RAG pipelines using graph structures. If you're thinking about, in the process of, or have already incorporated knowledge graphs in RAG, we’d love to chat at team@whyhow.ai, or follow our newsletter at [WhyHow.AI](https://www.whyhow.ai/). Join our discussions about rules, determinism and knowledge graphs in RAG on our [Discord](https://discord.com/invite/9bWqrsxgHr).
```

### Comparing `whyhow-0.0.1/src/whyhow.egg-info/SOURCES.txt` & `whyhow-0.0.2/src/whyhow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.1/tests/test_client.py` & `whyhow-0.0.2/tests/test_client.py`

 * *Files identical despite different names*

