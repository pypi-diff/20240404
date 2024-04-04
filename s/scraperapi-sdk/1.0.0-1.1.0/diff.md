# Comparing `tmp/scraperapi_sdk-1.0.0.tar.gz` & `tmp/scraperapi_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraperapi_sdk-1.0.0.tar", max compression
+gzip compressed data, was "scraperapi_sdk-1.1.0.tar", max compression
```

## Comparing `scraperapi_sdk-1.0.0.tar` & `scraperapi_sdk-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1572 2024-04-03 07:49:15.926495 scraperapi_sdk-1.0.0/README.md
--rw-r--r--   0        0        0      713 2024-04-03 07:46:42.401487 scraperapi_sdk-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-12-20 08:41:35.662682 scraperapi_sdk-1.0.0/scraperapi_sdk/__init__.py
--rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.0.0/scraperapi_sdk/__version__.py
--rw-r--r--   0        0        0     2632 2024-04-03 07:46:57.405216 scraperapi_sdk-1.0.0/scraperapi_sdk/_client.py
--rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.0.0/scraperapi_sdk/exceptions.py
--rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 scraperapi_sdk-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3670 2024-04-04 06:44:07.242371 scraperapi_sdk-1.1.0/README.md
+-rw-r--r--   0        0        0      713 2024-04-03 11:43:14.100373 scraperapi_sdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-12-20 08:41:35.662682 scraperapi_sdk-1.1.0/scraperapi_sdk/__init__.py
+-rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.1.0/scraperapi_sdk/__version__.py
+-rw-r--r--   0        0        0     4346 2024-04-03 14:03:58.665538 scraperapi_sdk-1.1.0/scraperapi_sdk/_client.py
+-rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.1.0/scraperapi_sdk/exceptions.py
+-rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 scraperapi_sdk-1.1.0/PKG-INFO
```

### Comparing `scraperapi_sdk-1.0.0/pyproject.toml` & `scraperapi_sdk-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scraperapi-sdk"
-version = "1.0.0"
+version = "1.1.0"
 description = "ScraperAPI Python SDK"
 authors = ["ScraperAPI"]
 readme = "README.md"
 
 [project]
 requires-python = ">= 3.8"
```

