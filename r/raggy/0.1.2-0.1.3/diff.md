# Comparing `tmp/raggy-0.1.2.tar.gz` & `tmp/raggy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raggy-0.1.2.tar", last modified: Thu Mar 28 14:33:18 2024, max compression
+gzip compressed data, was "raggy-0.1.3.tar", last modified: Thu Apr  4 18:08:10 2024, max compression
```

## Comparing `raggy-0.1.2.tar` & `raggy-0.1.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.125238 raggy-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.109238 raggy-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.113237 raggy-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-28 14:33:08.000000 raggy-0.1.2/.github/workflows/publish-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-28 14:33:08.000000 raggy-0.1.2/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-28 14:33:08.000000 raggy-0.1.2/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-03-28 14:33:08.000000 raggy-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-28 14:33:08.000000 raggy-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-28 14:33:08.000000 raggy-0.1.2/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-28 14:33:18.125238 raggy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-28 14:33:08.000000 raggy-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.113237 raggy-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.113237 raggy-0.1.2/docs/api_reference/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.113237 raggy-0.1.2/docs/api_reference/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/loaders/base.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/loaders/github.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/loaders/pdf.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/loaders/web.md
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/settings.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/docs/api_reference/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/utilities/asyncutils.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/utilities/collections.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/utilities/embeddings.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/utilities/filesystem.md
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/utilities/ids.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/utilities/logging.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/utilities/text.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/docs/api_reference/vectorstores/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/vectorstores/base.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/vectorstores/chroma.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/api_reference/vectorstores/tpuf.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.109238 raggy-0.1.2/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/docs/assets/logos/
--rw-r--r--   0 runner    (1001) docker     (127)   506712 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/assets/logos/raggy.png
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/ingest_strategy.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/docs/welcome/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/welcome/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-28 14:33:08.000000 raggy-0.1.2/docs/welcome/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/examples/chat_with_X/
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-28 14:33:08.000000 raggy-0.1.2/examples/chat_with_X/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 14:33:08.000000 raggy-0.1.2/examples/chat_with_X/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-28 14:33:08.000000 raggy-0.1.2/examples/reddit_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/examples/refresh_chroma/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-28 14:33:08.000000 raggy-0.1.2/examples/refresh_chroma/refresh_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 14:33:08.000000 raggy-0.1.2/examples/refresh_chroma/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/examples/refresh_tpuf/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-28 14:33:08.000000 raggy-0.1.2/examples/refresh_tpuf/refresh_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-28 14:33:08.000000 raggy-0.1.2/examples/refresh_tpuf/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-03-28 14:33:08.000000 raggy-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-28 14:33:08.000000 raggy-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:33:18.125238 raggy-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.109238 raggy-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.117237 raggy-0.1.2/src/raggy/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 14:33:18.000000 raggy-0.1.2/src/raggy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.121238 raggy-0.1.2/src/raggy/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.121238 raggy-0.1.2/src/raggy/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/loaders/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/loaders/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/loaders/web.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.121238 raggy-0.1.2/src/raggy/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/utilities/asyncutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/utilities/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/utilities/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/utilities/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/utilities/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.121238 raggy-0.1.2/src/raggy/vectorstores/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/vectorstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/vectorstores/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/vectorstores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-03-28 14:33:08.000000 raggy-0.1.2/src/raggy/vectorstores/tpuf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.125238 raggy-0.1.2/src/raggy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-28 14:33:18.000000 raggy-0.1.2/src/raggy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-28 14:33:18.000000 raggy-0.1.2/src/raggy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:33:18.000000 raggy-0.1.2/src/raggy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-28 14:33:18.000000 raggy-0.1.2/src/raggy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-28 14:33:18.000000 raggy-0.1.2/src/raggy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 14:33:18.000000 raggy-0.1.2/src/raggy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.121238 raggy-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:08.000000 raggy-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:18.125238 raggy-0.1.2/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:08.000000 raggy-0.1.2/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:08.000000 raggy-0.1.2/tests/loaders/test_github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.827490 raggy-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.811490 raggy-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.815490 raggy-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 18:08:02.000000 raggy-0.1.3/.github/workflows/publish-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-04 18:08:02.000000 raggy-0.1.3/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-04 18:08:02.000000 raggy-0.1.3/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-04 18:08:02.000000 raggy-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-04 18:08:02.000000 raggy-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-04 18:08:02.000000 raggy-0.1.3/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-04 18:08:10.827490 raggy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-04 18:08:02.000000 raggy-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.815490 raggy-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.815490 raggy-0.1.3/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.815490 raggy-0.1.3/docs/api_reference/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/loaders/base.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/loaders/github.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/loaders/pdf.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/loaders/web.md
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/settings.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.815490 raggy-0.1.3/docs/api_reference/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/utilities/asyncutils.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/utilities/collections.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/utilities/embeddings.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/utilities/filesystem.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/utilities/ids.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/utilities/logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/utilities/text.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.815490 raggy-0.1.3/docs/api_reference/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/vectorstores/base.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/vectorstores/chroma.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/api_reference/vectorstores/tpuf.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.811490 raggy-0.1.3/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.815490 raggy-0.1.3/docs/assets/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)   506712 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/assets/logos/raggy.png
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/ingest_strategy.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.819490 raggy-0.1.3/docs/welcome/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/welcome/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-04 18:08:02.000000 raggy-0.1.3/docs/welcome/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.819490 raggy-0.1.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.819490 raggy-0.1.3/examples/chat_with_X/
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-04 18:08:02.000000 raggy-0.1.3/examples/chat_with_X/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 18:08:02.000000 raggy-0.1.3/examples/chat_with_X/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-04 18:08:02.000000 raggy-0.1.3/examples/reddit_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.819490 raggy-0.1.3/examples/refresh_chroma/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-04 18:08:02.000000 raggy-0.1.3/examples/refresh_chroma/refresh_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 18:08:02.000000 raggy-0.1.3/examples/refresh_chroma/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.819490 raggy-0.1.3/examples/refresh_tpuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-04 18:08:02.000000 raggy-0.1.3/examples/refresh_tpuf/refresh_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 18:08:02.000000 raggy-0.1.3/examples/refresh_tpuf/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-04 18:08:02.000000 raggy-0.1.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-04 18:08:02.000000 raggy-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:08:10.827490 raggy-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.811490 raggy-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.819490 raggy-0.1.3/src/raggy/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 18:08:10.000000 raggy-0.1.3/src/raggy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.819490 raggy-0.1.3/src/raggy/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.823490 raggy-0.1.3/src/raggy/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/loaders/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/loaders/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/loaders/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.823490 raggy-0.1.3/src/raggy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/utilities/asyncutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/utilities/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/utilities/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/utilities/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/utilities/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.823490 raggy-0.1.3/src/raggy/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/vectorstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/vectorstores/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/vectorstores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-04 18:08:02.000000 raggy-0.1.3/src/raggy/vectorstores/tpuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.823490 raggy-0.1.3/src/raggy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-04 18:08:10.000000 raggy-0.1.3/src/raggy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-04 18:08:10.000000 raggy-0.1.3/src/raggy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:08:10.000000 raggy-0.1.3/src/raggy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 18:08:10.000000 raggy-0.1.3/src/raggy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-04 18:08:10.000000 raggy-0.1.3/src/raggy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 18:08:10.000000 raggy-0.1.3/src/raggy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.823490 raggy-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:02.000000 raggy-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:10.823490 raggy-0.1.3/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:02.000000 raggy-0.1.3/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:08:02.000000 raggy-0.1.3/tests/loaders/test_github.py
```

### Comparing `raggy-0.1.2/.github/workflows/publish-docs.yml` & `raggy-0.1.3/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/.github/workflows/static-analysis.yml` & `raggy-0.1.3/.github/workflows/static-analysis.yml`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/.gitignore` & `raggy-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/PKG-INFO` & `raggy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raggy
-Version: 0.1.2
+Version: 0.1.3
 Summary: scraping stuff
 Project-URL: Code, https://github.com/zzstoatzz/raggy
 Keywords: scraping,nlp,ai,document-processing
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `raggy-0.1.2/docs/assets/logos/raggy.png` & `raggy-0.1.3/docs/assets/logos/raggy.png`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/docs/hooks.py` & `raggy-0.1.3/docs/hooks.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/docs/index.md` & `raggy-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/docs/welcome/installation.md` & `raggy-0.1.3/docs/welcome/installation.md`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/docs/welcome/tutorial.md` & `raggy-0.1.3/docs/welcome/tutorial.md`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/examples/chat_with_X/repo.py` & `raggy-0.1.3/examples/chat_with_X/repo.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/examples/reddit_thread.py` & `raggy-0.1.3/examples/reddit_thread.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/examples/refresh_chroma/refresh_collection.py` & `raggy-0.1.3/examples/refresh_chroma/refresh_collection.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/examples/refresh_tpuf/refresh_namespace.py` & `raggy-0.1.3/examples/refresh_tpuf/refresh_namespace.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/mkdocs.yml` & `raggy-0.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/pyproject.toml` & `raggy-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/cli/__init__.py` & `raggy-0.1.3/src/raggy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/documents.py` & `raggy-0.1.3/src/raggy/documents.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/loaders/base.py` & `raggy-0.1.3/src/raggy/loaders/base.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/loaders/github.py` & `raggy-0.1.3/src/raggy/loaders/github.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/loaders/pdf.py` & `raggy-0.1.3/src/raggy/loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/loaders/web.py` & `raggy-0.1.3/src/raggy/loaders/web.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/settings.py` & `raggy-0.1.3/src/raggy/settings.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/utilities/asyncutils.py` & `raggy-0.1.3/src/raggy/utilities/asyncutils.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/utilities/collections.py` & `raggy-0.1.3/src/raggy/utilities/collections.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/utilities/embeddings.py` & `raggy-0.1.3/src/raggy/utilities/embeddings.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/utilities/filesystem.py` & `raggy-0.1.3/src/raggy/utilities/filesystem.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/utilities/ids.py` & `raggy-0.1.3/src/raggy/utilities/ids.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/utilities/logging.py` & `raggy-0.1.3/src/raggy/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/utilities/text.py` & `raggy-0.1.3/src/raggy/utilities/text.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/vectorstores/base.py` & `raggy-0.1.3/src/raggy/vectorstores/base.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/vectorstores/chroma.py` & `raggy-0.1.3/src/raggy/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy/vectorstores/tpuf.py` & `raggy-0.1.3/src/raggy/vectorstores/tpuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,28 @@
 from raggy.vectorstores.base import Vectorstore
 
 
 class TurboPufferSettings(BaseSettings):
     """Settings for the TurboPuffer vectorstore."""
 
     model_config = SettingsConfigDict(
-        env_prefix="RAGGY_TURBOPUFFER_",
+        env_prefix="TURBOPUFFER_",
         env_file=("~/.raggy/.env", ".env"),
         arbitrary_types_allowed=True,
         extra="ignore",
     )
 
     api_key: SecretStr
     default_namespace: str = "raggy"
 
     @model_validator(mode="after")
     def set_api_key(self):
         if not tpuf.api_key and self.api_key:
             tpuf.api_key = self.api_key.get_secret_value()
+        return self
 
 
 tpuf_settings = TurboPufferSettings()
 
 
 class TurboPuffer(Vectorstore):
     """Wrapper for turbopuffer.Namespace as an async context manager.
```

### Comparing `raggy-0.1.2/src/raggy.egg-info/PKG-INFO` & `raggy-0.1.3/src/raggy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raggy
-Version: 0.1.2
+Version: 0.1.3
 Summary: scraping stuff
 Project-URL: Code, https://github.com/zzstoatzz/raggy
 Keywords: scraping,nlp,ai,document-processing
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `raggy-0.1.2/src/raggy.egg-info/SOURCES.txt` & `raggy-0.1.3/src/raggy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raggy-0.1.2/src/raggy.egg-info/requires.txt` & `raggy-0.1.3/src/raggy.egg-info/requires.txt`

 * *Files identical despite different names*

