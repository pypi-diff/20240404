# Comparing `tmp/dreamai-0.9.0.tar.gz` & `tmp/dreamai-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-0.9.0.tar", last modified: Thu May  4 00:50:09 2023, max compression
+gzip compressed data, was "dreamai-2.0.tar", max compression
```

## Comparing `dreamai-0.9.0.tar` & `dreamai-2.0.tar`

### file list

```diff
@@ -1,22 +1,9 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:50:09.494943 dreamai-0.9.0/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.9.0/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.9.0/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-04 00:50:09.494943 dreamai-0.9.0/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-05-02 14:01:47.000000 dreamai-0.9.0/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:50:09.494943 dreamai-0.9.0/dreamai/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 00:50:04.000000 dreamai-0.9.0/dreamai/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     7897 2023-05-04 00:50:04.000000 dreamai-0.9.0/dreamai/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8873 2023-05-04 00:50:04.000000 dreamai-0.9.0/dreamai/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      858 2023-05-02 20:23:11.000000 dreamai-0.9.0/dreamai/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8258 2023-05-04 00:50:04.000000 dreamai-0.9.0/dreamai/vision.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:50:09.494943 dreamai-0.9.0/dreamai.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.9.0/dreamai.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2564 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-05-04 00:50:09.000000 dreamai-0.9.0/dreamai.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3224 2023-05-04 00:50:01.000000 dreamai-0.9.0/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 00:50:09.494943 dreamai-0.9.0/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-05-02 13:55:29.000000 dreamai-0.9.0/setup.py
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0/dreamai/__init__.py
+-rw-r--r--   0        0        0     3040 2024-04-03 18:36:32.193450 dreamai-2.0/dreamai/ai.py
+-rw-r--r--   0        0        0     4959 2024-04-04 15:15:49.821233 dreamai-2.0/dreamai/chroma.py
+-rw-r--r--   0        0        0     1902 2024-04-03 19:08:30.427986 dreamai-2.0/dreamai/pdf.py
+-rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0/dreamai/templates.py
+-rw-r--r--   0        0        0     5693 2024-04-03 18:34:42.550727 dreamai-2.0/dreamai/utils.py
+-rw-r--r--   0        0        0      676 2024-04-04 15:03:56.280560 dreamai-2.0/pyproject.toml
+-rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 dreamai-2.0/PKG-INFO
```

