# Comparing `tmp/letsreadscraper-0.1.1.tar.gz` & `tmp/letsreadscraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsreadscraper-0.1.1.tar", max compression
+gzip compressed data, was "letsreadscraper-0.1.2.tar", max compression
```

## Comparing `letsreadscraper-0.1.1.tar` & `letsreadscraper-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-03 21:54:06.103141 letsreadscraper-0.1.1/letsreadscraper/__init__.py
--rw-r--r--   0        0        0       89 2024-04-03 22:56:08.138265 letsreadscraper-0.1.1/letsreadscraper/cli.py
--rw-r--r--   0        0        0      136 2024-04-03 22:58:48.675205 letsreadscraper-0.1.1/letsreadscraper/main.py
--rw-r--r--   0        0        0      573 2024-04-03 23:02:38.466572 letsreadscraper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 21:54:06.104143 letsreadscraper-0.1.1/README.md
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 letsreadscraper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-04-04 18:58:20.368834 letsreadscraper-0.1.2/letsreadscraper/__init__.py
+-rw-r--r--   0        0        0     1607 2024-04-04 19:19:54.425323 letsreadscraper-0.1.2/letsreadscraper/scraper.py
+-rw-r--r--   0        0        0      950 2024-04-04 18:22:12.550219 letsreadscraper-0.1.2/letsreadscraper/utilities.py
+-rw-r--r--   0        0        0      736 2024-04-04 19:15:32.376765 letsreadscraper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 18:15:34.197043 letsreadscraper-0.1.2/README.md
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 letsreadscraper-0.1.2/PKG-INFO
```

