# Comparing `tmp/fundus-0.2.1.tar.gz` & `tmp/fundus-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundus-0.2.1.tar", last modified: Tue Mar 26 16:58:23 2024, max compression
+gzip compressed data, was "fundus-0.2.2.tar", last modified: Thu Apr  4 11:44:46 2024, max compression
```

## Comparing `fundus-0.2.1.tar` & `fundus-0.2.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.040480 fundus-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-26 16:58:18.000000 fundus-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 16:58:18.000000 fundus-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-03-26 16:58:23.040480 fundus-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-03-26 16:58:18.000000 fundus-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-26 16:58:18.000000 fundus-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 16:58:23.040480 fundus-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.024479 fundus-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.028480 fundus-0.2.1/src/fundus/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.028480 fundus-0.2.1/src/fundus/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.028480 fundus-0.2.1/src/fundus/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/parser/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/parser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.028480 fundus-0.2.1/src/fundus/publishers/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.028480 fundus-0.2.1/src/fundus/publishers/at/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/at/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/at/orf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/base_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.032480 fundus-0.2.1/src/fundus/publishers/de/
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/berliner_zeitung.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/bild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/braunschweiger_zeitung.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/business_insider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/die_welt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/die_zeit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/dw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/faz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/focus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/mdr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/merkur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/ndr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/ntv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/spon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/stern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/sz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/tagesschau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/taz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/de/waz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.032480 fundus-0.2.1/src/fundus/publishers/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/fr/le_monde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.032480 fundus-0.2.1/src/fundus/publishers/na/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/na/the_namibian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.032480 fundus-0.2.1/src/fundus/publishers/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/uk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/uk/i_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/uk/the_guardian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/uk/the_independent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/uk/the_telegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.036480 fundus-0.2.1/src/fundus/publishers/us/
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/ap_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/cnbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/fox_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/free_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/la_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/occupy_democrats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/reuters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/the_gateway_pundit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/the_intercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/the_nation_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/the_new_yorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/washington_times_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/publishers/us/world_truth.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.036480 fundus-0.2.1/src/fundus/scraping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/article.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.036480 fundus-0.2.1/src/fundus/scraping/common_crawl/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/common_crawl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/common_crawl/html.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/common_crawl/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/common_crawl/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/html.py
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/scraping/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.040480 fundus-0.2.1/src/fundus/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/utils/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-26 16:58:18.000000 fundus-0.2.1/src/fundus/utils/more_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.040480 fundus-0.2.1/src/fundus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-03-26 16:58:23.000000 fundus-0.2.1/src/fundus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-26 16:58:23.000000 fundus-0.2.1/src/fundus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:58:23.000000 fundus-0.2.1/src/fundus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-26 16:58:23.000000 fundus-0.2.1/src/fundus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 16:58:23.000000 fundus-0.2.1/src/fundus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:58:23.040480 fundus-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-26 16:58:18.000000 fundus-0.2.1/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-03-26 16:58:18.000000 fundus-0.2.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-26 16:58:18.000000 fundus-0.2.1/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.888215 fundus-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-04 11:44:40.000000 fundus-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 11:44:40.000000 fundus-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-04 11:44:46.888215 fundus-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-04 11:44:40.000000 fundus-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-04 11:44:40.000000 fundus-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 11:44:46.888215 fundus-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.872215 fundus-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.872215 fundus-0.2.2/src/fundus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.876215 fundus-0.2.2/src/fundus/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.876215 fundus-0.2.2/src/fundus/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/parser/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/parser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.876215 fundus-0.2.2/src/fundus/publishers/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.876215 fundus-0.2.2/src/fundus/publishers/at/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/at/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/at/orf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/base_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.880215 fundus-0.2.2/src/fundus/publishers/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/berliner_zeitung.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/bild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/braunschweiger_zeitung.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/business_insider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/die_welt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/die_zeit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/dw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/faz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/mdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/merkur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/ndr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/ntv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/spon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/stern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/sz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/tagesschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/taz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/de/waz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.880215 fundus-0.2.2/src/fundus/publishers/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/fr/le_monde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.880215 fundus-0.2.2/src/fundus/publishers/na/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/na/the_namibian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.880215 fundus-0.2.2/src/fundus/publishers/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/i_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/the_guardian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/the_independent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/uk/the_telegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus/publishers/us/
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/ap_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/cnbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/fox_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/free_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/la_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/occupy_democrats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/the_gateway_pundit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/the_intercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/the_nation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/the_new_yorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/washington_times_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/publishers/us/world_truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus/scraping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/article.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus/scraping/common_crawl/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/common_crawl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/common_crawl/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/common_crawl/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/common_crawl/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/scraping/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/utils/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-04 11:44:40.000000 fundus-0.2.2/src/fundus/utils/more_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/src/fundus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 11:44:46.000000 fundus-0.2.2/src/fundus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:46.884215 fundus-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-04 11:44:40.000000 fundus-0.2.2/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-04 11:44:40.000000 fundus-0.2.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-04 11:44:40.000000 fundus-0.2.2/tests/test_pipeline.py
```

### Comparing `fundus-0.2.1/LICENSE` & `fundus-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/PKG-INFO` & `fundus-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundus
-Version: 0.2.1
+Version: 0.2.2
 Summary: A very simple news crawler
 Author-email: Max Dallabetta <max.dallabetta@googlemail.com>
 License: MIT
 Project-URL: Repository, https://github.com/flairNLP/fundus
 Keywords: web scraping, web crawling
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fundus Version: 0.2.1 Summary: A very simple news
+Metadata-Version: 2.1 Name: fundus Version: 0.2.2 Summary: A very simple news
 crawler Author-email: Max Dallabetta
 googlemail.com> License: MIT Project-URL: Repository, https://github.com/
 flairNLP/fundus Keywords: web scraping, web crawling Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `fundus-0.2.1/README.md` & `fundus-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/pyproject.toml` & `fundus-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fundus"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name = "Max Dallabetta", email = "max.dallabetta@googlemail.com" },
 ]
 description = "A very simple news crawler"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fundus-0.2.1/src/fundus/__init__.py` & `fundus-0.2.2/src/fundus/__init__.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/parser/base_parser.py` & `fundus-0.2.2/src/fundus/parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/parser/data.py` & `fundus-0.2.2/src/fundus/parser/data.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/parser/utility.py` & `fundus-0.2.2/src/fundus/parser/utility.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/at/orf.py` & `fundus-0.2.2/src/fundus/publishers/at/orf.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/base_objects.py` & `fundus-0.2.2/src/fundus/publishers/base_objects.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/__init__.py` & `fundus-0.2.2/src/fundus/publishers/de/__init__.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/berliner_zeitung.py` & `fundus-0.2.2/src/fundus/publishers/de/berliner_zeitung.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/bild.py` & `fundus-0.2.2/src/fundus/publishers/de/bild.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/braunschweiger_zeitung.py` & `fundus-0.2.2/src/fundus/publishers/de/braunschweiger_zeitung.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/business_insider.py` & `fundus-0.2.2/src/fundus/publishers/de/business_insider.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/die_welt.py` & `fundus-0.2.2/src/fundus/publishers/de/die_welt.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/die_zeit.py` & `fundus-0.2.2/src/fundus/publishers/de/die_zeit.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/dw.py` & `fundus-0.2.2/src/fundus/publishers/de/dw.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/faz.py` & `fundus-0.2.2/src/fundus/publishers/de/faz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/focus.py` & `fundus-0.2.2/src/fundus/publishers/de/focus.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/mdr.py` & `fundus-0.2.2/src/fundus/publishers/de/mdr.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/merkur.py` & `fundus-0.2.2/src/fundus/publishers/de/merkur.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/ndr.py` & `fundus-0.2.2/src/fundus/publishers/de/ndr.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/ntv.py` & `fundus-0.2.2/src/fundus/publishers/de/ntv.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/spon.py` & `fundus-0.2.2/src/fundus/publishers/de/spon.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/stern.py` & `fundus-0.2.2/src/fundus/publishers/de/stern.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/sz.py` & `fundus-0.2.2/src/fundus/publishers/de/sz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/tagesschau.py` & `fundus-0.2.2/src/fundus/publishers/de/tagesschau.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/taz.py` & `fundus-0.2.2/src/fundus/publishers/de/taz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/de/waz.py` & `fundus-0.2.2/src/fundus/publishers/de/waz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/fr/__init__.py` & `fundus-0.2.2/src/fundus/publishers/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/fr/le_monde.py` & `fundus-0.2.2/src/fundus/publishers/fr/le_monde.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/na/__init__.py` & `fundus-0.2.2/src/fundus/publishers/na/__init__.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/na/the_namibian.py` & `fundus-0.2.2/src/fundus/publishers/na/the_namibian.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/uk/__init__.py` & `fundus-0.2.2/src/fundus/publishers/uk/__init__.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/uk/i_news.py` & `fundus-0.2.2/src/fundus/publishers/uk/i_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/uk/the_guardian.py` & `fundus-0.2.2/src/fundus/publishers/uk/the_guardian.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/uk/the_independent.py` & `fundus-0.2.2/src/fundus/publishers/uk/the_independent.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/uk/the_telegraph.py` & `fundus-0.2.2/src/fundus/publishers/uk/the_telegraph.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/__init__.py` & `fundus-0.2.2/src/fundus/publishers/us/__init__.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/ap_news.py` & `fundus-0.2.2/src/fundus/publishers/us/ap_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/cnbc.py` & `fundus-0.2.2/src/fundus/publishers/us/cnbc.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/fox_news.py` & `fundus-0.2.2/src/fundus/publishers/us/fox_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/free_beacon.py` & `fundus-0.2.2/src/fundus/publishers/us/free_beacon.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/la_times.py` & `fundus-0.2.2/src/fundus/publishers/us/la_times.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/occupy_democrats.py` & `fundus-0.2.2/src/fundus/publishers/us/occupy_democrats.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/reuters.py` & `fundus-0.2.2/src/fundus/publishers/us/reuters.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/the_gateway_pundit.py` & `fundus-0.2.2/src/fundus/publishers/us/the_gateway_pundit.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/the_intercept.py` & `fundus-0.2.2/src/fundus/publishers/us/the_intercept.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/the_nation_parser.py` & `fundus-0.2.2/src/fundus/publishers/us/the_nation_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,14 @@
         def _fix_malformed_html(self) -> None:
             if self.precomputed.doc.xpath("//div[contains(@id, 'cta-block')]"):
                 fixed_html = re.sub(
                     self._html_fix_pattern,
                     'name="sft_double_opt_sail"value="yes"/></div></form>',
                     self.precomputed.html,
                 )
-                with open("test_nation.html", "w", encoding="utf-8") as file:
-                    file.write(self.precomputed.html)
                 self.precomputed.doc = lxml.html.document_fromstring(fixed_html)
 
         # We remove aside tags here because the provided HTML does not enclose <p> tags
         # within .article-header-content. As a result, <aside> tags following <p> tags get attached
         # to the paragraph. This is valid HTML5 behaviour.
         # see https://stackoverflow.com/questions/8460993/p-end-tag-p-is-not-needed-in-html
         @function(priority=2)
```

### Comparing `fundus-0.2.1/src/fundus/publishers/us/the_new_yorker.py` & `fundus-0.2.2/src/fundus/publishers/us/the_new_yorker.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/washington_times_parser.py` & `fundus-0.2.2/src/fundus/publishers/us/washington_times_parser.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/publishers/us/world_truth.py` & `fundus-0.2.2/src/fundus/publishers/us/world_truth.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/scraping/article.py` & `fundus-0.2.2/src/fundus/scraping/article.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/scraping/common_crawl/html.py` & `fundus-0.2.2/src/fundus/scraping/common_crawl/html.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/scraping/common_crawl/pipeline.py` & `fundus-0.2.2/src/fundus/scraping/common_crawl/pipeline.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/scraping/common_crawl/scraper.py` & `fundus-0.2.2/src/fundus/scraping/common_crawl/scraper.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/scraping/filter.py` & `fundus-0.2.2/src/fundus/scraping/filter.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/scraping/html.py` & `fundus-0.2.2/src/fundus/scraping/html.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/scraping/pipeline.py` & `fundus-0.2.2/src/fundus/scraping/pipeline.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/scraping/scraper.py` & `fundus-0.2.2/src/fundus/scraping/scraper.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus/utils/more_async.py` & `fundus-0.2.2/src/fundus/utils/more_async.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/src/fundus.egg-info/PKG-INFO` & `fundus-0.2.2/src/fundus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundus
-Version: 0.2.1
+Version: 0.2.2
 Summary: A very simple news crawler
 Author-email: Max Dallabetta <max.dallabetta@googlemail.com>
 License: MIT
 Project-URL: Repository, https://github.com/flairNLP/fundus
 Keywords: web scraping, web crawling
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fundus Version: 0.2.1 Summary: A very simple news
+Metadata-Version: 2.1 Name: fundus Version: 0.2.2 Summary: A very simple news
 crawler Author-email: Max Dallabetta
 googlemail.com> License: MIT Project-URL: Repository, https://github.com/
 flairNLP/fundus Keywords: web scraping, web crawling Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `fundus-0.2.1/src/fundus.egg-info/SOURCES.txt` & `fundus-0.2.2/src/fundus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/tests/test_collection.py` & `fundus-0.2.2/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/tests/test_parser.py` & `fundus-0.2.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `fundus-0.2.1/tests/test_pipeline.py` & `fundus-0.2.2/tests/test_pipeline.py`

 * *Files identical despite different names*

