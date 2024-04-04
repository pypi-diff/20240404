# Comparing `tmp/sinol_make-1.5.9.tar.gz` & `tmp/sinol_make-1.6.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol_make-1.5.9.tar", last modified: Sun Sep 24 10:44:02 2023, max compression
+gzip compressed data, was "sinol_make-1.6.0.dev1.tar", last modified: Thu Apr  4 20:42:56 2024, max compression
```

## Comparing `sinol_make-1.5.9.tar` & `sinol_make-1.6.0.dev1.tar`

### file list

```diff
@@ -1,62 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.816016 sinol_make-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-09-24 10:43:47.000000 sinol_make-1.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-09-24 10:44:02.816016 sinol_make-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-09-24 10:43:47.000000 sinol_make-1.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-24 10:43:47.000000 sinol_make-1.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-09-24 10:44:02.816016 sinol_make-1.5.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.808016 sinol_make-1.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.812016 sinol_make-1.5.9/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.808016 sinol_make-1.5.9/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.812016 sinol_make-1.5.9/src/sinol_make/commands/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/commands/doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.812016 sinol_make-1.5.9/src/sinol_make/commands/export/
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/commands/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.812016 sinol_make-1.5.9/src/sinol_make/commands/gen/
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/commands/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/commands/gen/gen_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.812016 sinol_make-1.5.9/src/sinol_make/commands/inwer/
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/commands/inwer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/commands/inwer/inwer_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.812016 sinol_make-1.5.9/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (127)    53492 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/commands/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.812016 sinol_make-1.5.9/src/sinol_make/contest_types/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/contest_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/contest_types/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/contest_types/icpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/contest_types/oi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.816016 sinol_make-1.5.9/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/helpers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/helpers/package_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/helpers/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/helpers/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/helpers/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.816016 sinol_make-1.5.9/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.816016 sinol_make-1.5.9/src/sinol_make/oiejq/
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/oiejq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/oiejq/perf_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.816016 sinol_make-1.5.9/src/sinol_make/structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/structs/cache_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/structs/compiler_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/structs/gen_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/structs/inwer_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/structs/run_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/structs/status_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2023-09-24 10:43:47.000000 sinol_make-1.5.9/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.812016 sinol_make-1.5.9/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-09-24 10:44:02.000000 sinol_make-1.5.9/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-09-24 10:44:02.000000 sinol_make-1.5.9/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-24 10:44:02.000000 sinol_make-1.5.9/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-24 10:44:02.000000 sinol_make-1.5.9/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-09-24 10:44:02.000000 sinol_make-1.5.9/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-24 10:44:02.000000 sinol_make-1.5.9/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 10:44:02.816016 sinol_make-1.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2023-09-24 10:43:47.000000 sinol_make-1.5.9/tests/test_oiejq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-09-24 10:43:47.000000 sinol_make-1.5.9/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.149683 sinol_make-1.6.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.149683 sinol_make-1.6.0.dev1/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/export/
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/ingen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/ingen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/ingen/ingen_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/inwer_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/outgen_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (127)    57981 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/commands/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/icpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/oi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/src/sinol_make/oiejq/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/oiejq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/oiejq/perf_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/cache_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/gen_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/inwer_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/run_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/status_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/tests/test_multiple_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/tests/test_oiejq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/tests/test_util.py
```

### Comparing `sinol_make-1.5.9/LICENSE` & `sinol_make-1.6.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol_make-1.5.9/PKG-INFO` & `sinol_make-1.6.0.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 Metadata-Version: 2.1
 Name: sinol_make
-Version: 1.5.9
+Version: 1.6.0.dev1
 Summary: CLI tool for creating sio2 task packages
 Author: Mateusz Masiarz
 Author-email: m.masiarz@fri.edu.pl
 Maintainer: Tomasz Nowak, Mateusz Masiarz
 Maintainer-email: tomasz.nowak@tonowak.com, m.masiarz@fri.edu.pl
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: argcomplete
 Requires-Dist: requests
 Requires-Dist: PyYAML
 Requires-Dist: dictdiffer
 Requires-Dist: importlib-resources
 Requires-Dist: psutil
+Requires-Dist: packaging
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
 
-# <img src="https://avatars.githubusercontent.com/u/2264918?s=200&v=4" height=60em> sinol-make
+# ![Logo](https://avatars.githubusercontent.com/u/2264918?s=60&v=4) sinol-make
 
 `sinol-make` is a CLI tool for creating and verifying problem packages
 for [sio2](https://github.com/sio2project/oioioi)
 with features such as:
+
 - measuring time and memory in the same deterministic way as sio2,
 - running the solutions in parallel,
 - keeping a git-friendly report of solutions' scores,
 - catching mistakes in the problem packages as early as possible,
 - and more.
 
-# Contents
+## Contents
 
 - [Why?](#why)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Configuarion](#configuration)
 - [Reporting bugs and contributing code](#reporting-bugs-and-contributing-code)
 
 ### Why?
 
 The purpose of the tool is to make it easier to create good problem packages
 for official competitions, which requires collaboration with other people
 and using a multitude of "good practices" recommendations.
@@ -58,49 +60,68 @@
 solutions' runtime, called `oiejq`.
 
 ### Installation
 
 It's possible to directly install [sinol-make](https://pypi.org/project/sinol-make/)
 through Python's package manager pip, which usually is installed alongside Python:
 
-```
+```bash
 pip3 install sinol-make
 ```
 
+`pip` installs the `sinol-make` executable in `~/.local/bin/` directory,
+so make sure this directory is in your `PATH`.
+[Here's](https://gist.github.com/nex3/c395b2f8fd4b02068be37c961301caa7) how to add a directory to `PATH`.
+
 As `oiejq` works only on Linux-based operating systems,
 *we do not recommend* using operating systems such as Windows or macOS.
 Nevertheless `sinol-make` supports those operating systems,
 though there are additional installation steps required to use
 other tools for measuring time (which are non-deterministic and produce reports different from sio2):
+
 - Debian-based systems (Ubuntu, usually Windows WSL): `apt install time`
 - Arch-based systems: `pacman -S time`
 - macOS: `brew install gnu-time coreutils`
 
-### Autocompletion (optional)
+#### Autocompletion (optional)
 
 If you would like to have autocompletion for `sinol-make` commands,
 run the following command and refresh the shell (e.g. by opening a new terminal):
 
 ```shell
 activate-global-python-argcomplete
 ```
 
 ### Usage
 
 The availabe commands (see `sinol-make --help`) are:
 
 - `sinol-make run` -- Runs selected solutions (by default all solutions) on selected tests (by default all tests) with a given number
 of CPUs. Measures the solutions' time with oiejq, unless specified otherwise. After running the solutions, it
-compares the solutions' scores with the ones saved in config.yml.
+compares the solutions' scores with the ones saved in config.yml. If you're using oiejq, make sure you are not running on efficiency
+cpu cores. You can check if you have them [like this](https://stackoverflow.com/a/71282744). To run on normal cpu cores, use
+`taskset -c 8-15 sinol-make ...`, assuming that cpu cores 8-15 are not efficiency cores.
 Run `sinol-make run --help` to see available flags.
 - `sinol-make gen` -- Generate input files using ingen program (for example prog/abcingen.cpp for abc task). 
-Whenever the new input differs from the previous one, the model solution will be used to generate the new output file. 
-You can also specify your ingen source file which will be used. Run `sinol-make gen --help` to see available flags.
+Whenever the new input differs from the previous one, the model solution will be used to generate the new output file.
+You can also specify your ingen source file which will be used.
+Run `sinol-make gen --help` to see available flags.
+- `sinol-make ingen` -- Generate input files using ingen program (for example prog/abcingen.cpp for abc task).
+You can also specify your ingen source file which will be used.
+Run `sinol-make ingen --help` to see available flags.
+- `sinol-make outgen` -- Generate output files using the model solutions. Run `sinol-make outgen --help` to see available flags.
 - `sinol-make inwer` -- Verifies whether input files are correct using your "inwer.cpp" program. You can specify what inwer
 program to use, what tests to check and how many CPUs to use. Run `sinol-make inwer --help` to see available flags.
 - `sinol-make export` -- Creates archive ready to upload to sio2 or szkopul. Run `sinol-make export --help` to see all available flags.
 - `sinol-make doc` -- Compiles all LaTeX files in doc/ directory to PDF. Run `sinol-make doc --help` to see all available flags.
+- `sinol-make init [id]` -- Creates package from template [on github](https://github.com/sio2project/sinol-make/tree/main/example_package) and sets task id to provided `[id]`. Requires an internet connection to run.
+
+You can also run multiple commands at once, for example:
+
+```shell
+sinol-make gen prog/abcingen2.cpp inwer --cpus 4 run --tests abc1*.in doc export --no-statement
+```
 
 ### Reporting bugs and contributing code
 
 - Want to report a bug or request a feature? [Open an issue](https://github.com/sio2project/sinol-make/issues).
 - Want to help us build `sinol-make`? Create a Pull Request and we will gladly review it.
```

### Comparing `sinol_make-1.5.9/setup.cfg` & `sinol_make-1.6.0.dev1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Bug Tracker = https://github.com/sio2project/sinol-make/issues
 	Homepage = https://github.com/sio2project/sinol-make
 classifiers = 
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: MIT License
+	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 
 [options]
 packages = find_namespace:
 packages_dir = src
 include_package_data = True
 python_requires = >=3.7
@@ -25,22 +25,24 @@
 	argparse
 	argcomplete
 	requests
 	PyYAML
 	dictdiffer
 	importlib-resources
 	psutil
+	packaging
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-cov
+	pytest-xdist
 	requests-mock
 
 [options.entry_points]
 console_scripts = 
 	sinol-make = sinol_make:main
 
 [tool:pytest]
```

### Comparing `sinol_make-1.5.9/src/sinol_make/__init__.py` & `sinol_make-1.6.0.dev1/src/sinol_make/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # PYTHON_ARGCOMPLETE_OK
-
-import argcomplete
-import traceback
-import argparse
 import sys
-import os
+import argparse
+import traceback
+import argcomplete
 
 from sinol_make import util, oiejq
 
-
-__version__ = "1.5.9"
+__version__ = "1.6.0.dev1"
 
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
@@ -30,52 +27,80 @@
     for command in commands:
         command.configure_subparser(subparsers)
 
     argcomplete.autocomplete(parser)
     return parser
 
 
+def check_oiejq():
+    if util.is_linux() and not oiejq.check_oiejq():
+        print(util.warning('`oiejq` in `~/.local/bin/` not found, installing now...'))
+        try:
+            if oiejq.install_oiejq():
+                print(util.info('`oiejq` was successfully installed.'))
+            else:
+                util.exit_with_error('`oiejq` could not be installed.\n'
+                                     'You can download it from https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz, '
+                                     'unpack it to `~/.local/bin/` and rename oiejq.sh to oiejq.\n'
+                                     'You can also use --oiejq-path to specify path to your oiejq.')
+        except Exception as err:
+            util.exit_with_error('`oiejq` could not be installed.\n' + str(err))
+
+
 def main_exn():
     parser = configure_parsers()
-    args = parser.parse_args()
+    arguments = []
+    curr_args = []
+    for arg in sys.argv[1:]:
+        if arg in util.get_command_names() and not (len(curr_args) > 0 and curr_args[0] == 'init'):
+            if curr_args:
+                arguments.append(curr_args)
+            curr_args = [arg]
+        else:
+            curr_args.append(arg)
+    if curr_args:
+        arguments.append(curr_args)
     commands = util.get_commands()
+    check_oiejq()
 
-    for command in commands:
-        if command.get_name() == args.command:
-            new_version = util.check_for_updates(__version__)
-            if new_version is not None:
-                print(util.warning(
-                    f'New version of sinol-make is available (your version: {__version__}, available version: {new_version}).\n'
-                    f' You can update it by running `pip3 install sinol-make --upgrade`.'))
-
-            if util.is_linux() and not oiejq.check_oiejq():
-                print(util.warning('`oiejq` in `~/.local/bin/` not found, installing now...'))
-
-                try:
-                    if oiejq.install_oiejq():
-                        print(util.info('`oiejq` was successfully installed.'))
-                    else:
-                        util.exit_with_error('`oiejq` could not be installed.\n'
-                                             'You can download it from https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz'
-                                             ', unpack it to `~/.local/bin/` and rename oiejq.sh to oiejq.\n'
-                                             'You can also use --oiejq-path to specify path to your oiejq.')
-                except Exception as err:
-                    util.exit_with_error('`oiejq` could not be installed.\n' + err)
-
-            util.make_version_changes()
-            command.run(args)
-            exit(0)
-
-    parser.print_help()
+    for curr_args in arguments:
+        args = parser.parse_args(curr_args)
+        command_found = False
+        for command in commands:
+            if command.get_name() == args.command:
+                command_found = True
+                if len(arguments) > 1:
+                    print(f' {command.get_name()} command '.center(util.get_terminal_size()[1], '='))
+                command.run(args)
+        if not command_found:
+            parser.print_help()
+            exit(1)
 
 
 def main():
+    new_version = None
     try:
+        if util.is_dev(__version__):
+            print(util.warning('You are using a development version of sinol-make. '
+                               'It may be unstable and contain bugs.'))
+        new_version = util.check_for_updates(__version__)
         main_exn()
     except argparse.ArgumentError as err:
         util.exit_with_error(err)
     except SystemExit as err:
         exit(err.code)
-    except:
+    except Exception:
         print(traceback.format_exc())
         util.exit_with_error('An error occurred while running the command.\n'
-                             'If that is a bug, please report it or submit a bugfix: https://github.com/sio2project/sinol-make/#reporting-bugs-and-contributing-code')
+                             'If that is a bug, please report it or submit a bugfix: '
+                             'https://github.com/sio2project/sinol-make/#reporting-bugs-and-contributing-code')
+    finally:
+        if new_version is not None:
+            if not util.is_dev(new_version):
+                print(util.warning(
+                    f'New version of sinol-make is available (your version: {__version__}, available version: '
+                    f'{new_version}).\nYou can update it by running `pip3 install sinol-make --upgrade`.'))
+            elif util.is_dev(new_version):
+                print(util.warning(
+                    f'New development version of sinol-make is available (your version: {__version__}, available '
+                    f'version: {new_version}).\nYou can update it by running `pip3 install sinol-make --pre --upgrade`.'
+                ))
```

### Comparing `sinol_make-1.5.9/src/sinol_make/commands/export/__init__.py` & `sinol_make-1.6.0.dev1/src/sinol_make/commands/export/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import os
 import glob
+import stat
 import shutil
 import tarfile
+import tempfile
 import argparse
-import yaml
 
-from sinol_make import util
+from sinol_make import util, contest_types
+from sinol_make.commands.ingen.ingen_util import get_ingen, compile_ingen, run_ingen, ingen_exists
 from sinol_make.helpers import package_util, parsers, paths
-from sinol_make.commands.gen import gen_util
 from sinol_make.interfaces.BaseCommand import BaseCommand
+from sinol_make.commands.outgen import Command as OutgenCommand, compile_correct_solution, get_correct_solution
+from sinol_make.commands.doc import Command as DocCommand
+from sinol_make.interfaces.Errors import UnknownContestType
 
 
 class Command(BaseCommand):
     """
     Class for "export" command.
     """
 
@@ -20,37 +24,112 @@
         return "export"
 
     def configure_subparser(self, subparser: argparse.ArgumentParser):
         parser = subparser.add_parser(
             self.get_name(),
             help='Create archive for oioioi upload',
             description='Creates archive in the current directory ready to upload to sio2 or szkopul.')
+        parser.add_argument('-c', '--cpus', type=int,
+                            help=f'number of cpus to use to generate output files '
+                                 f'(default: {util.default_cpu_count()})',
+                            default=util.default_cpu_count())
+        parser.add_argument('--no-statement', dest='no_statement', action='store_true',
+                            help='allow export without statement')
+        parser.add_argument('--export-ocen', dest='export_ocen', action='store_true',
+                            help='Create ocen archive')
         parsers.add_compilation_arguments(parser)
+        return parser
+
+    def generate_input_tests(self):
+        print('Generating tests...')
+        temp_package = paths.get_cache_path('export', 'tests')
+        if os.path.exists(temp_package):
+            shutil.rmtree(temp_package)
+        os.makedirs(temp_package)
+        in_dir = os.path.join(temp_package, 'in')
+        os.makedirs(in_dir)
+        out_dir = os.path.join(temp_package, 'out')
+        os.makedirs(out_dir)
+        prog_dir = os.path.join(temp_package, 'prog')
+        if os.path.exists(os.path.join(os.getcwd(), 'prog')):
+            shutil.copytree(os.path.join(os.getcwd(), 'prog'), prog_dir)
+
+        if ingen_exists(self.task_id):
+            ingen_path = get_ingen(self.task_id)
+            ingen_path = os.path.join(prog_dir, os.path.basename(ingen_path))
+            ingen_exe = compile_ingen(ingen_path, self.args, self.args.compile_mode)
+            if not run_ingen(ingen_exe, in_dir):
+                util.exit_with_error('Failed to run ingen.')
+
+    def generate_output_files(self):
+        tests = paths.get_cache_path('export', 'tests')
+        in_dir = os.path.join(tests, 'in')
+        os.makedirs(in_dir, exist_ok=True)
+        out_dir = os.path.join(tests, 'out')
+        os.makedirs(out_dir, exist_ok=True)
+
+        # Only example output tests are required for export.
+        ocen_tests = glob.glob(os.path.join(in_dir, f'{self.task_id}0*.in')) + \
+                     glob.glob(os.path.join(in_dir, f'{self.task_id}*ocen.in'))
+        outputs = []
+        for test in ocen_tests:
+            outputs.append(os.path.join(out_dir, os.path.basename(test).replace('.in', '.out')))
+        if len(outputs) > 0:
+            outgen = OutgenCommand()
+            correct_solution_exe = compile_correct_solution(get_correct_solution(self.task_id), self.args,
+                                                            self.args.compile_mode)
+            outgen.args = self.args
+            outgen.correct_solution_exe = correct_solution_exe
+            outgen.generate_outputs(outputs)
 
     def get_generated_tests(self):
         """
         Returns list of generated tests.
         Executes ingen to check what tests are generated.
         """
-        if not gen_util.ingen_exists(self.task_id):
+        if not ingen_exists(self.task_id):
             return []
 
-        working_dir = paths.get_cache_path('export', 'tests')
-        if os.path.exists(working_dir):
-            shutil.rmtree(working_dir)
-        os.makedirs(working_dir)
-
-        ingen_path = gen_util.get_ingen(self.task_id)
-        ingen_exe = gen_util.compile_ingen(ingen_path, self.args, self.args.weak_compilation_flags)
-        if not gen_util.run_ingen(ingen_exe, working_dir):
-            util.exit_with_error('Failed to run ingen.')
-
-        tests = glob.glob(os.path.join(working_dir, f'{self.task_id}*.in'))
+        in_dir = paths.get_cache_path('export', 'tests', 'in')
+        tests = glob.glob(os.path.join(in_dir, f'{self.task_id}*.in'))
         return [package_util.extract_test_id(test, self.task_id) for test in tests]
 
+    def create_ocen(self, target_dir: str):
+        """
+        Creates ocen archive for sio2.
+        :param target_dir: Path to exported package.
+        """
+        attachments_dir = os.path.join(target_dir, 'attachments')
+        if not os.path.exists(attachments_dir):
+            os.makedirs(attachments_dir)
+        tests_dir = paths.get_cache_path('export', 'tests')
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            ocen_dir = os.path.join(tmpdir, self.task_id)
+            os.makedirs(ocen_dir)
+            in_dir = os.path.join(ocen_dir, 'in')
+            os.makedirs(in_dir)
+            out_dir = os.path.join(ocen_dir, 'out')
+            os.makedirs(out_dir)
+            for ext in ['in', 'out']:
+                for test in glob.glob(os.path.join(tests_dir, ext, f'{self.task_id}0*.{ext}')) + \
+                            glob.glob(os.path.join(tests_dir, ext, f'{self.task_id}*ocen.{ext}')):
+                    shutil.copy(test, os.path.join(ocen_dir, ext, os.path.basename(test)))
+
+            shutil.make_archive(os.path.join(attachments_dir, f'{self.task_id}ocen'), 'zip', tmpdir)
+
+    def compile_statement(self):
+        command = DocCommand()
+        doc_args = argparse.Namespace()
+        doc_args.files = [f'./doc/{self.task_id}zad.tex']
+        command.run(doc_args)
+        if not os.path.isfile(f'./doc/{self.task_id}zad.pdf') and not self.args.no_statement:
+            util.exit_with_error('There is no pdf statements. If this intentional, export with flag "--no-statement". '
+                                 'Otherwise create pdf before continuing.')
+
     def copy_package_required_files(self, target_dir: str):
         """
         Copies package files and directories from
         current directory to target directory.
         :param target_dir: Directory to copy files to.
         """
         files = ['config.yml', 'makefile.in', 'Makefile.in',
@@ -58,34 +137,44 @@
         for file in files:
             file_path = os.path.join(os.getcwd(), file)
             if os.path.exists(file_path):
                 if os.path.isdir(file_path):
                     shutil.copytree(file_path, os.path.join(target_dir, file))
                 else:
                     shutil.copy(file_path, target_dir)
+        shell_ingen = os.path.join(target_dir, 'prog', f'{self.task_id}ingen.sh')
+        if os.path.exists(shell_ingen):
+            st = os.stat(shell_ingen)
+            os.chmod(shell_ingen, st.st_mode | stat.S_IEXEC)
 
         print('Copying example tests...')
         for ext in ['in', 'out']:
             os.mkdir(os.path.join(target_dir, ext))
             for test in glob.glob(os.path.join(os.getcwd(), ext, f'{self.task_id}0*.{ext}')):
                 shutil.copy(test, os.path.join(target_dir, ext))
 
-        print('Generating tests...')
         generated_tests = self.get_generated_tests()
         tests_to_copy = []
         for ext in ['in', 'out']:
             for test in glob.glob(os.path.join(os.getcwd(), ext, f'{self.task_id}*.{ext}')):
                 if package_util.extract_test_id(test, self.task_id) not in generated_tests:
-                    tests_to_copy.append(test)
+                    tests_to_copy.append((ext, test))
 
+        cache_test_dir = paths.get_cache_path('export', 'tests')
         if len(tests_to_copy) > 0:
             print(util.warning(f'Found {len(tests_to_copy)} tests that are not generated by ingen.'))
             for test in tests_to_copy:
-                print(util.warning(f'Coping {os.path.basename(test)}...'))
-                shutil.copy(test, os.path.join(target_dir, os.path.splitext(os.path.basename(test))[1]))
+                print(util.warning(f'Copying {os.path.basename(test[1])}...'))
+                shutil.copy(test[1], os.path.join(target_dir, test[0], os.path.basename(test[1])))
+                shutil.copy(test[1], os.path.join(cache_test_dir, test[0], os.path.basename(test[1])))
+
+        self.generate_output_files()
+        if self.args.export_ocen:
+            print('Generating ocen archive...')
+            self.create_ocen(target_dir)
 
     def clear_files(self, target_dir: str):
         """
         Clears unnecessary files from target directory.
         :param target_dir: Directory to clear files from.
         """
         files_to_remove = ['doc/*~', 'doc/*.aux', 'doc/*.log', 'doc/*.dvi', 'doc/*.err', 'doc/*.inf']
@@ -98,14 +187,15 @@
         Creates required `makefile.in` file.
         :param target_dir: Directory to create files in.
         :param config: Config dictionary.
         """
         with open(os.path.join(target_dir, 'makefile.in'), 'w') as f:
             cxx_flags = '-std=c++20'
             c_flags = '-std=gnu99'
+
             def format_multiple_arguments(obj):
                 if isinstance(obj, str):
                     return obj
                 return ' '.join(obj)
 
             if 'extra_compilation_args' in config:
                 if 'cpp' in config['extra_compilation_args']:
@@ -128,34 +218,43 @@
 
     def compress(self, target_dir):
         """
         Compresses target directory to archive.
         :param target_dir: Target directory path.
         :return: Path to archive.
         """
-        archive = os.path.join(os.getcwd(), f'{self.task_id}.tgz')
+        archive = os.path.join(os.getcwd(), f'{self.export_name}.tgz')
         with tarfile.open(archive, "w:gz") as tar:
             tar.add(target_dir, arcname=os.path.basename(target_dir))
         return archive
 
     def run(self, args: argparse.Namespace):
-        util.exit_if_not_package()
+        args = util.init_package_command(args)
 
         self.args = args
         self.task_id = package_util.get_task_id()
+        self.export_name = self.task_id
         package_util.validate_test_names(self.task_id)
+        try:
+            self.contest = contest_types.get_contest_type()
+        except UnknownContestType as e:
+            util.exit_with_error(str(e))
 
-        with open(os.path.join(os.getcwd(), 'config.yml'), 'r') as config_file:
-            config = yaml.load(config_file, Loader=yaml.FullLoader)
+        config = package_util.get_config()
 
         export_package_path = paths.get_cache_path('export', self.task_id)
         if os.path.exists(export_package_path):
             shutil.rmtree(export_package_path)
         os.makedirs(export_package_path)
 
         util.change_stack_size_to_unlimited()
+        self.generate_input_tests()
+        self.compile_statement()
         self.copy_package_required_files(export_package_path)
         self.clear_files(export_package_path)
         self.create_makefile_in(export_package_path, config)
+        export_name = self.contest.additional_export_job()
+        if export_name is not None:
+            self.export_name = export_name
         archive = self.compress(export_package_path)
 
-        print(util.info(f'Exported to {self.task_id}.tgz'))
+        print(util.info(f'Exported to {self.export_name}.tgz'))
```

### Comparing `sinol_make-1.5.9/src/sinol_make/commands/gen/__init__.py` & `sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,115 +2,135 @@
 import glob
 import os
 import yaml
 
 import multiprocessing as mp
 
 from sinol_make import util
-from sinol_make.commands.gen import gen_util
+from sinol_make.commands.outgen.outgen_util import get_correct_solution, compile_correct_solution, generate_output
 from sinol_make.structs.gen_structs import OutputGenerationArguments
-from sinol_make.helpers import parsers, package_util
+from sinol_make.helpers import parsers, package_util, cache, paths
 from sinol_make.interfaces.BaseCommand import BaseCommand
 
 
 class Command(BaseCommand):
     """
     Class for `gen` command.
     """
 
     def get_name(self):
-        return "gen"
+        return "outgen"
 
     def configure_subparser(self, subparser):
         parser = subparser.add_parser(
             self.get_name(),
-            help='Generate input and output files',
-            description='Generate input files using ingen program '
-                        '(for example prog/abcingen.cpp for abc task). Whenever '
-                        'the new input differs from the previous one, '
-                        'the model solution will be used to generate the new output '
-                        'file. You can also specify your ingen source '
-                        'file which will be used.'
+            help='Generate output files',
+            description='Generate output files using the correct solution.'
         )
 
-        parser.add_argument('ingen_path', type=str, nargs='?',
-                            help='path to ingen source file, for example prog/abcingen.cpp')
         parser.add_argument('-c', '--cpus', type=int,
-                            help=f'number of cpus to use to generate output files (default: {mp.cpu_count()} - all available)',
-                            default=mp.cpu_count())
+                            help=f'number of cpus to use to generate output files '
+                                 f'(default: {util.default_cpu_count()})',
+                            default=util.default_cpu_count())
+        parser.add_argument('-n', '--no-validate', default=False, action='store_true',
+                            help='do not validate test contents')
         parsers.add_compilation_arguments(parser)
+        return parser
 
     def generate_outputs(self, outputs_to_generate):
         print(f'Generating output files for {len(outputs_to_generate)} tests on {self.args.cpus} cpus.')
         arguments = []
         for output in outputs_to_generate:
             output_basename = os.path.basename(output)
-            input = os.path.join(os.getcwd(), 'in', os.path.splitext(output_basename)[0] + '.in')
+            in_dir = os.path.join("/", *(os.path.abspath(output).split(os.sep)[:-2]), 'in')
+            input = os.path.join(in_dir, os.path.splitext(output_basename)[0] + '.in')
             arguments.append(OutputGenerationArguments(self.correct_solution_exe, input, output))
 
         with mp.Pool(self.args.cpus) as pool:
             results = []
-            for i, result in enumerate(pool.imap(gen_util.generate_output, arguments)):
+            for i, result in enumerate(pool.imap(generate_output, arguments)):
                 results.append(result)
                 if result:
                     print(util.info(f'Successfully generated output file {os.path.basename(arguments[i].output_test)}'))
                 else:
                     print(util.error(f'Failed to generate output file {os.path.basename(arguments[i].output_test)}'))
 
             if not all(results):
                 util.exit_with_error('Failed to generate some output files.')
             else:
                 print(util.info('Successfully generated all output files.'))
 
-    def calculate_md5_sums(self):
+    def calculate_md5_sums(self, tests=None):
         """
         Calculates md5 sums for each test.
-        :return: Tuple (dictionary of md5 sums, list of outputs tests that need to be generated)
+        :return: Tuple (dictionary of md5 sums, list of outputs tests that need to be generated,
+                 list of input tests based on which the output tests will be generated)
         """
+        if tests is None:
+            tests = glob.glob(os.path.join(os.getcwd(), 'in', '*.in'))
+
         old_md5_sums = None
         try:
             with open(os.path.join(os.getcwd(), 'in', '.md5sums'), 'r') as f:
                 file_content = yaml.load(f, Loader=yaml.FullLoader)
                 if isinstance(file_content, dict):
                     old_md5_sums = file_content
         except (yaml.YAMLError, OSError):
             pass
 
         md5_sums = {}
         outputs_to_generate = []
-        for file in glob.glob(os.path.join(os.getcwd(), 'in', '*.in')):
+        from_inputs = []
+        for file in tests:
             basename = os.path.basename(file)
+            output_basename = os.path.splitext(os.path.basename(basename))[0] + '.out'
+            output_path = os.path.join(os.getcwd(), 'out', output_basename)
             md5_sums[basename] = util.get_file_md5(file)
 
             if old_md5_sums is None or old_md5_sums.get(basename, '') != md5_sums[basename]:
-                output_basename = os.path.splitext(os.path.basename(basename))[0] + '.out'
-                outputs_to_generate.append(os.path.join(os.getcwd(), "out", output_basename))
+                outputs_to_generate.append(output_path)
+                from_inputs.append(file)
+            elif not os.path.exists(output_path):
+                # If output file does not exist, generate it.
+                outputs_to_generate.append(output_path)
+                from_inputs.append(file)
+
+        return md5_sums, outputs_to_generate, from_inputs
 
-        return md5_sums, outputs_to_generate
+    def clean_cache(self, inputs):
+        """
+        Cleans cache for the given input files.
+        """
+        md5_sums = [util.get_file_md5(file) for file in inputs]
+        for solution in glob.glob(paths.get_cache_path("md5sums", "*")):
+            sol_cache = cache.get_cache_file(solution)
+            for input in md5_sums:
+                if input in sol_cache.tests:
+                    del sol_cache.tests[input]
+            sol_cache.save(solution)
 
     def run(self, args: argparse.Namespace):
-        util.exit_if_not_package()
+        args = util.init_package_command(args)
 
         self.args = args
         self.task_id = package_util.get_task_id()
         package_util.validate_test_names(self.task_id)
-        self.ingen = gen_util.get_ingen(self.task_id, args.ingen_path)
-        print(util.info(f'Using ingen file {os.path.basename(self.ingen)}'))
-
-        self.correct_solution = gen_util.get_correct_solution(self.task_id)
-        self.ingen_exe = gen_util.compile_ingen(self.ingen, self.args, self.args.weak_compilation_flags)
-
         util.change_stack_size_to_unlimited()
-        if gen_util.run_ingen(self.ingen_exe):
-            print(util.info('Successfully generated input files.'))
-        else:
-            util.exit_with_error('Failed to generate input files.')
-        md5_sums, outputs_to_generate = self.calculate_md5_sums()
+        cache.check_correct_solution(self.task_id)
+        self.correct_solution = get_correct_solution(self.task_id)
+
+        md5_sums, outputs_to_generate, from_inputs = self.calculate_md5_sums()
         if len(outputs_to_generate) == 0:
             print(util.info('All output files are up to date.'))
         else:
-            self.correct_solution_exe = gen_util.compile_correct_solution(self.correct_solution, self.args,
-                                                                          self.args.weak_compilation_flags)
+            self.clean_cache(from_inputs)
+            self.correct_solution_exe = compile_correct_solution(self.correct_solution, self.args,
+                                                                 self.args.compile_mode)
             self.generate_outputs(outputs_to_generate)
+            with open(os.path.join(os.getcwd(), 'in', '.md5sums'), 'w') as f:
+                yaml.dump(md5_sums, f)
 
-        with open(os.path.join(os.getcwd(), 'in', '.md5sums'), 'w') as f:
-            yaml.dump(md5_sums, f)
+        if not self.args.no_validate:
+            print(util.info('Validating output test contents.'))
+            for test in sorted(outputs_to_generate):
+                package_util.validate_test(test)
+            print(util.info('Output test contents are valid!'))
```

### Comparing `sinol_make-1.5.9/src/sinol_make/commands/inwer/__init__.py` & `sinol_make-1.6.0.dev1/src/sinol_make/commands/verify/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,158 +1,160 @@
-import subprocess
-import sys
-import signal
-import threading
-import argparse
 import os
-import multiprocessing as mp
-from typing import Dict, List
+import stat
+import shutil
+import argparse
+import subprocess
 
-from sinol_make import util
-from sinol_make.structs.inwer_structs import TestResult, InwerExecution, VerificationResult, TableData
-from sinol_make.helpers import package_util, compile, printer, paths
-from sinol_make.helpers.parsers import add_compilation_arguments
+from sinol_make import util, contest_types
+from sinol_make.helpers import parsers, package_util, paths
 from sinol_make.interfaces.BaseCommand import BaseCommand
-from sinol_make.commands.inwer import inwer_util
+from sinol_make.commands.gen import Command as GenCommand
+from sinol_make.commands.doc import Command as DocCommand
+from sinol_make.commands.inwer import Command as InwerCommand, inwer_util
+from sinol_make.commands.run import Command as RunCommand
 
 
 class Command(BaseCommand):
     """
-    Class for "inwer" command.
+    Class for `verify` command.
     """
 
     def get_name(self):
-        return "inwer"
+        return "verify"
 
-    def configure_subparser(self, subparser: argparse.ArgumentParser):
+    def configure_subparser(self, subparser):
         parser = subparser.add_parser(
             self.get_name(),
-            help='Verify if input files are correct',
-            description='Verify if input files are correct using inwer program '
-                        '(for example prog/abcinwer.cpp for abc task). You can also '
-                        'specify your inwer source file which will be used.'
+            help='Verify the package',
+            description='Verify the whole package. This command will first '
+                        'run stress tests (if the file `prog/{task_id}stresstest.sh` exists), '
+                        'verify the config, generate tests, generate problem '
+                        'statements, run inwer and run all solutions. '
+                        'Ingen and inwer are compiled with sanitizers (-fsanitize=address,undefined), '
+                        'which may fail on some systems. To fix this, run `sudo sysctl vm.mmap_rnd_bits = 28` '
+                        'or disable sanitizers with --no-fsanitize.'
         )
 
-        parser.add_argument('inwer_path', type=str, nargs='?',
-                            help='path to inwer source file, for example prog/abcinwer.cpp')
-        parser.add_argument('-t', '--tests', type=str, nargs='+',
-                            help='test to verify, for example in/abc{0,1}*')
+        parser.add_argument('-f', '--no-fsanitize', action='store_true', default=False,
+                             help='do not use sanitizers for ingen and inwer programs')
         parser.add_argument('-c', '--cpus', type=int,
-                            help=f'number of cpus to use (default: {mp.cpu_count()} -all available)')
-        add_compilation_arguments(parser)
+                            help=f'number of cpus that sinol-make will use '
+                                 f'(default: {util.default_cpu_count()})',
+                            default=util.default_cpu_count())
+        parsers.add_compilation_arguments(parser)
 
-    def compile_inwer(self, args: argparse.Namespace):
-        self.inwer_executable, compile_log_path = inwer_util.compile_inwer(self.inwer, args, args.weak_compilation_flags)
-        if self.inwer_executable is None:
-            util.exit_with_error('Compilation failed.', lambda: compile.print_compile_log(compile_log_path))
-        else:
-            print(util.info('Compilation successful.'))
-
-    @staticmethod
-    def verify_test(execution: InwerExecution) -> VerificationResult:
+    def remove_cache(self):
         """
-        Verifies a test and returns the result of inwer on this test.
+        Remove whole cache dir
         """
-        output_dir = paths.get_executables_path(execution.test_name)
-        os.makedirs(output_dir, exist_ok=True)
-
-        command = [execution.inwer_exe_path]
-        with open(execution.test_path, 'r') as test:
-            process = subprocess.Popen(command, stdin=test, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-                                       preexec_fn=os.setsid)
-
-            def sigint_handler(signum, frame):
-                try:
-                    os.killpg(os.getpgid(process.pid), signal.SIGTERM)
-                except ProcessLookupError:
-                    pass
-                sys.exit(1)
-            signal.signal(signal.SIGINT, sigint_handler)
-
-            process.wait()
-        exit_code = process.returncode
-        out, _ = process.communicate()
-
-        return VerificationResult(
-            execution.test_path,
-            exit_code == 0,
-            out.decode('utf-8')
-        )
+        cache_dir = paths.get_cache_path()
+        if os.path.exists(cache_dir):
+            shutil.rmtree(cache_dir)
 
-    def verify_and_print_table(self) -> Dict[str, TestResult]:
+    def check_extra_files(self):
         """
-        Verifies all tests and prints the results in a table.
-        :return: dictionary of TestResult objects
+        Checks if extra_compilation_files and extra_execution_files exist.
         """
-        results = {}
-        sorted_tests = sorted(self.tests, key=lambda test: package_util.get_group(test, self.task_id))
-        executions: List[InwerExecution] = []
-        for test in sorted_tests:
-            results[test] = TestResult(test, self.task_id)
-            executions.append(InwerExecution(test, results[test].test_name, self.inwer_executable))
-
-        has_terminal, terminal_width, terminal_height = util.get_terminal_size()
-
-        table_data = TableData(results, 0)
-        if has_terminal:
-            run_event = threading.Event()
-            run_event.set()
-            thr = threading.Thread(target=printer.printer_thread, args=(run_event, inwer_util.print_view, table_data))
-            thr.start()
-
-        keyboard_interrupt = False
-        try:
-            with mp.Pool(self.cpus) as pool:
-                for i, result in enumerate(pool.imap(self.verify_test, executions)):
-                    table_data.results[result.test_path].set_results(result.valid, result.output)
-                    table_data.i = i
-        except KeyboardInterrupt:
-            keyboard_interrupt = True
-
-        if has_terminal:
-            run_event.clear()
-            thr.join()
-
-        print("\n".join(inwer_util.print_view(terminal_width, terminal_height, table_data)[0]))
-
-        if keyboard_interrupt:
-            util.exit_with_error('Keyboard interrupt.')
-
-        return results
+        extra_compilation_files = self.config.get('extra_compilation_files', [])
+        for file in extra_compilation_files:
+            if not os.path.exists(os.path.join(os.getcwd(), "prog", file)):
+                util.exit_with_error(f"Extra compilation file `{file}` does not exist. "
+                                     f"It should be in `prog` directory.")
+        if extra_compilation_files:
+            print(util.info("All extra compilation files exist."))
+
+        extra_execution_files = self.config.get('extra_execution_files', {})
+        for lang, files in extra_execution_files.items():
+            for file in files:
+                if not os.path.exists(os.path.join(os.getcwd(), "prog", file)):
+                    util.exit_with_error(f"Extra execution file `{file}` for language `{lang}` does not exist. "
+                                         f"It should be in `prog` directory.")
+        if extra_execution_files:
+            print(util.info("All extra execution files exist."))
+
+    def verify_scores(self, scored_groups):
+        config_scores = self.config.get('scores', {})
+        if not config_scores:
+            return
+        if '0' in scored_groups:
+            scored_groups.remove('0')
+        if 0 in scored_groups:
+            scored_groups.remove(0)
+
+        for group in scored_groups:
+            if int(group) not in config_scores:
+                util.exit_with_error(f"Score for group '{group}' not found. "
+                                     f"You must either provide scores for all groups "
+                                     f"or not provide them at all (to have them assigned automatically).")
+
+        for group in config_scores:
+            if int(group) not in scored_groups:
+                util.exit_with_error(f"Score for group '{group}' found in config, "
+                                     f"but no such test group exists in scored groups. "
+                                     f"You must either provide scores for all groups "
+                                     f"or not provide them at all (to have them assigned automatically).")
+
+        print(util.info("All scores are provided for all groups."))
+
+    def prepare_args(self, command):
+        parser = argparse.ArgumentParser()
+        subparser = parser.add_subparsers(dest='command')
+        command_parser = command.configure_subparser(subparser)
+        command_args = command_parser.parse_args([])
+        for key, value in vars(self.args).items():
+            setattr(command_args, key, value)
+        setattr(command_args, 'fsanitize', not self.args.no_fsanitize)
+        return command_args
+
+    def run_stresstests(self):
+        stresstests_path = os.path.join(os.getcwd(), 'prog', self.task_id + 'stresstest.sh')
+        if not os.path.exists(stresstests_path):
+            return
+
+        print(util.bold(' Running stress tests '.center(util.get_terminal_size()[1], '=')))
+        print(f"See the comments in `prog/{self.task_id}stresstest.sh` for details.".center(
+            util.get_terminal_size()[1], ' '))
+        st = os.stat(stresstests_path)
+        os.chmod(stresstests_path, st.st_mode | stat.S_IEXEC)
+        p = subprocess.Popen([stresstests_path], shell=True)
+        p.wait()
+        if p.returncode != 0:
+            util.exit_with_error("Stress tests failed.")
 
     def run(self, args: argparse.Namespace):
-        util.exit_if_not_package()
-
+        self.args = util.init_package_command(args)
+        self.config = package_util.get_config()
         self.task_id = package_util.get_task_id()
-        package_util.validate_test_names(self.task_id)
-        self.inwer = inwer_util.get_inwer_path(self.task_id, args.inwer_path)
-        if self.inwer is None:
-            if args.inwer_path is None:
-                util.exit_with_error('No inwer found in `prog/` directory.')
-            else:
-                util.exit_with_error(f'Inwer "{args.inwer_path}" not found.')
-        relative_path = os.path.relpath(self.inwer, os.getcwd())
-        print(f'Verifying with inwer {util.bold(relative_path)}')
+        self.contest = contest_types.get_contest_type()
 
-        self.cpus = args.cpus or mp.cpu_count()
-        self.tests = package_util.get_tests(self.task_id, args.tests)
-
-        if len(self.tests) == 0:
-            util.exit_with_error('No tests found.')
+        self.remove_cache()
+        self.check_extra_files()
+        self.contest.verify_pre_gen()
+
+        # Run stresstests (if present)
+        self.run_stresstests()
+
+        # Generate tests
+        print(util.bold(' Generating tests '.center(util.get_terminal_size()[1], '=')))
+        gen = GenCommand()
+        gen.run(self.prepare_args(gen))
+        self.verify_scores(package_util.get_groups(package_util.get_all_inputs(self.task_id), self.task_id))
+
+        # Generate problem statements
+        print(util.bold(' Generating problem statements '.center(util.get_terminal_size()[1], '=')))
+        doc = DocCommand()
+        doc.run(self.prepare_args(doc))
+
+        # Run inwer
+        if inwer_util.get_inwer_path(self.task_id) is None:
+            print(util.warning("Package doesn't have inwer."))
         else:
-            print('Verifying tests: ' + util.bold(', '.join(self.tests)))
-
-        util.change_stack_size_to_unlimited()
-        self.compile_inwer(args)
-        results: Dict[str, TestResult] = self.verify_and_print_table()
-        print('')
-
-        failed_tests = []
-        for result in results.values():
-            if not result.valid:
-                failed_tests.append(result.test_name)
+            print(util.bold(' Running inwer '.center(util.get_terminal_size()[1], '=')))
+            inwer = InwerCommand()
+            inwer.run(self.prepare_args(inwer))
+
+        # Run solutions
+        print(util.bold(' Running solutions '.center(util.get_terminal_size()[1], '=')))
+        run = RunCommand()
+        run.run(self.prepare_args(run))
 
-        if len(failed_tests) > 0:
-            util.exit_with_error(f'Verification failed for tests: {", ".join(failed_tests)}')
-        else:
-            print(util.info('Verification successful.'))
-            exit(0)
+        print(util.info('Package verification successful.'))
```

### Comparing `sinol_make-1.5.9/src/sinol_make/commands/inwer/inwer_util.py` & `sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/inwer_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sinol_make import util
 from sinol_make.commands.inwer import TestResult, TableData
 from sinol_make.helpers import compile, package_util
 from sinol_make.helpers import compiler
 from sinol_make.interfaces.Errors import CompilationError
 
 
-def get_inwer_path(task_id: str, path = None) -> Union[str, None]:
+def get_inwer_path(task_id: str, path=None) -> Union[str, None]:
     """
     Returns path to inwer executable for given task or None if no inwer was found.
     """
     if path is None:
         inwers = package_util.get_files_matching_pattern(task_id, f'{task_id}inwer.*')
         if len(inwers) == 0:
             return None
@@ -25,55 +25,72 @@
     else:
         inwer = os.path.join(os.getcwd(), path)
         if os.path.exists(inwer):
             return inwer
         return None
 
 
-def compile_inwer(inwer_path: str, args: argparse.Namespace, weak_compilation_flags=False):
+def compile_inwer(inwer_path: str, args: argparse.Namespace, compilation_flags='default', use_fsanitize=False):
     """
     Compiles inwer and returns path to compiled executable and path to compile log.
     """
     compilers = compiler.verify_compilers(args, [inwer_path])
-    return compile.compile_file(inwer_path, package_util.get_executable(inwer_path), compilers, weak_compilation_flags)
+    inwer_exe, compile_log_path = compile.compile_file(inwer_path, package_util.get_executable(inwer_path), compilers,
+                                                       compilation_flags, use_fsanitize=use_fsanitize,
+                                                       additional_flags='-D_INWER')
+
+    if inwer_exe is None:
+        compile.print_compile_log(compile_log_path)
+        util.exit_with_error('Failed inwer compilation.')
+    else:
+        print(util.info('Compilation successful.'))
+    return inwer_exe
+
+
+def sort_tests(tests, task_id):
+    # First sort by group, then by test name.
+    tests.sort(key=lambda test: [package_util.get_group(test, task_id), test])
+    return tests
 
 
 def print_view(term_width, term_height, table_data: TableData):
     """
     Prints current results of test verification.
     """
 
     previous_stdout = sys.stdout
     new_stdout = StringIO()
     sys.stdout = new_stdout
 
     results = table_data.results
     column_lengths = [0, len('Group') + 1, len('Status') + 1, 0]
-    sorted_test_paths = []
+    tests = []
     for result in results.values():
         column_lengths[0] = max(column_lengths[0], len(result.test_name))
         column_lengths[1] = max(column_lengths[1], len(result.test_group))
-        sorted_test_paths.append(result.test_path)
-    sorted_test_paths.sort()
+        tests.append(result.test_path)
+    tests = sort_tests(tests, table_data.task_id)
 
-    column_lengths[3] = max(10, term_width - column_lengths[0] - column_lengths[1] - column_lengths[2] - 9 - 3) # 9 is for " | " between columns, 3 for margin.
+    column_lengths[3] = max(10, term_width - column_lengths[0] - column_lengths[1] - column_lengths[
+        2] - 9 - 3)  # 9 is for " | " between columns, 3 for margin.
     margin = "  "
 
     def print_line_separator():
-        res = "-" * (column_lengths[0] + 3) + "+" + "-" * (column_lengths[1] + 1) + "+" + "-" * (column_lengths[2] + 1) + "+"
+        res = "-" * (column_lengths[0] + 3) + "+" + "-" * (column_lengths[1] + 1) + "+" + "-" * (
+                    column_lengths[2] + 1) + "+"
         res += "-" * (term_width - len(res) - 1)
         print(res)
 
     print_line_separator()
 
     print(margin + "Test".ljust(column_lengths[0]) + " | " + "Group".ljust(column_lengths[1] - 1) + " | " + "Status" +
           " | " + "Output")
     print_line_separator()
 
-    for test_path in sorted_test_paths:
+    for test_path in tests:
         result = results[test_path]
         print(margin + result.test_name.ljust(column_lengths[0]) + " | ", end='')
         print(result.test_group.ljust(column_lengths[1] - 1) + " | ", end='')
 
         if result.verified:
             if result.valid:
                 print(util.info("OK".ljust(column_lengths[2] - 1)), end='')
```

### Comparing `sinol_make-1.5.9/src/sinol_make/commands/run/__init__.py` & `sinol_make-1.6.0.dev1/src/sinol_make/commands/run/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 # Version 0.6 (2021-08-29)
 import subprocess
 import signal
 import threading
 import time
 import psutil
 import glob
+import shutil
 from io import StringIO
 from typing import Dict
 
 from sinol_make import contest_types, oiejq
 from sinol_make.structs.run_structs import ExecutionData, PrintData
 from sinol_make.structs.cache_structs import CacheTest, CacheFile
 from sinol_make.helpers.parsers import add_compilation_arguments
 from sinol_make.interfaces.BaseCommand import BaseCommand
 from sinol_make.interfaces.Errors import CompilationError, CheckerOutputException, UnknownContestType
 from sinol_make.helpers import compile, compiler, package_util, printer, paths, cache
-from sinol_make.structs.status_structs import Status, ResultChange, PointsChange, ValidationResult, ExecutionResult
+from sinol_make.structs.status_structs import Status, ResultChange, PointsChange, ValidationResult, ExecutionResult, \
+    TotalPointsChange
 import sinol_make.util as util
 import yaml, os, collections, sys, re, math, dictdiffer
 import multiprocessing as mp
 
 
 def color_memory(memory, limit):
     if memory == -1: return util.color_yellow("")
@@ -47,25 +49,37 @@
 
 def colorize_status(status):
     if status == Status.OK: return util.bold(util.color_green(status))
     if status == Status.PENDING: return util.warning(status)
     return util.error(status)
 
 
+def colorize_points(points, min_points, max_points):
+    if points == max_points:
+        return util.color_green(str(points))
+    elif points == min_points:
+        return util.color_red(str(points))
+    else:
+        return util.color_yellow(str(points))
+
+
 def update_group_status(group_status, new_status):
-    order = [Status.CE, Status.TL, Status.ML, Status.RE, Status.WA, Status.OK]
+    order = [Status.CE, Status.TL, Status.ML, Status.RE, Status.WA, Status.OK, Status.PENDING]
     if order.index(new_status) < order.index(group_status):
         return new_status
     return group_status
 
 
 def print_view(term_width, term_height, task_id, program_groups_scores, all_results, print_data: PrintData, names, executions,
                groups, scores, tests, possible_score, cpus, hide_memory, config, contest, args):
-    width = term_width - 13  # First column has 6 characters, the " | " separator has 3 characters and 4 for margin
-    programs_in_row = width // 13  # Each program has 10 characters and the " | " separator has 3 characters
+    width = term_width - 11  # First column has 6 characters, the " | " separator has 3 characters and 2 for margin
+    # First column has 11 characters and each solution has 13 characters and the " | " separator has 3 characters
+    programs_in_row = width // 16
+    if programs_in_row == 0:
+        return ["Terminal window is too small to display the results."], None, None
 
     previous_stdout = sys.stdout
     output = StringIO()
     sys.stdout = output
 
     program_scores = collections.defaultdict(int)
     # program_times and program_memory are dictionaries of tuples (max, limit),
@@ -89,28 +103,46 @@
     for program_ix in range(0, len(names), programs_in_row):
         program_group = names[program_ix:program_ix + programs_in_row]
 
         def print_table_end():
             print("-" * 8, end="-+-")
             for i in range(len(program_group)):
                 if i != len(program_group) - 1:
-                    print("-" * 10, end="-+-")
+                    print("-" * 13, end="-+-")
                 else:
-                    print("-" * 10, end="-+")
+                    print("-" * 13, end="-+")
             print()
 
         print_table_end()
 
         print(margin + "groups", end=" | ")
-        for program in program_group:
-            print("%10s" % program, end=" | ")
-        print()
+        next_row = {solution: solution for solution in program_group}
+        first = True
+        while next_row != {}:
+            if first:
+                first = False
+            else:
+                print(margin + " " * 6, end=" | ")
+
+            for solution in program_group:
+                if solution in next_row:
+                    to_print = next_row[solution]
+                    if len(to_print) > 13:
+                        print(to_print[:13], end=" | ")
+                        next_row[solution] = to_print[13:]
+                    else:
+                        print(to_print.ljust(13), end=" | ")
+                        del next_row[solution]
+                else:
+                    print(" " * 13, end=" | ")
+            print()
+
         print(8 * "-", end=" | ")
         for program in program_group:
-            print(10 * "-", end=" | ")
+            print(13 * "-", end=" | ")
         print()
         for group in groups:
             print(margin + "%6s" % group, end=" | ")
             for program in program_group:
                 lang = package_util.get_file_lang(program)
                 results = all_results[program][group]
                 group_status = Status.OK
@@ -136,57 +168,58 @@
                     if status == Status.PENDING:
                         group_status = Status.PENDING
                     else:
                         group_status = update_group_status(group_status, status)
 
                 points = contest.get_group_score(test_scores, scores[group])
                 if any([results[test].Status == Status.PENDING for test in results]):
-                    print(" " * 3 + ("?" * len(str(scores[group]))).rjust(3) +
+                    print(" " * 6 + ("?" * len(str(scores[group]))).rjust(3) +
                           f'/{str(scores[group]).rjust(3)}', end=' | ')
                 else:
-                    print("%3s" % util.bold(util.color_green(group_status)) if group_status == Status.OK else util.bold(
-                        util.color_red(group_status)),
-                          "%3s/%3s" % (points, scores[group]),
-                          end=" | ")
+                    if group_status == Status.OK:
+                        status_text = util.bold(util.color_green(group_status.ljust(6)))
+                    else:
+                        status_text = util.bold(util.color_red(group_status.ljust(6)))
+                    print(f"{status_text}{str(points).rjust(3)}/{str(scores[group]).rjust(3)}", end=' | ')
                 program_groups_scores[program][group] = {"status": group_status, "points": points}
             print()
         for program in program_group:
             program_scores[program] = contest.get_global_score(program_groups_scores[program], possible_score)
 
         print(8 * " ", end=" | ")
         for program in program_group:
-            print(10 * " ", end=" | ")
+            print(13 * " ", end=" | ")
         print()
         print(margin + "points", end=" | ")
         for program in program_group:
-            print(util.bold("   %3s/%3s" % (program_scores[program], possible_score)), end=" | ")
+            print(util.bold("      %3s/%3s" % (program_scores[program], possible_score)), end=" | ")
         print()
         print(margin + "  time", end=" | ")
         for program in program_group:
             program_time = program_times[program]
-            print(util.bold(("%20s" % color_time(program_time[0], program_time[1]))
+            print(util.bold(("%23s" % color_time(program_time[0], program_time[1]))
                             if program_time[0] < 2 * program_time[1] and program_time[0] >= 0
-                            else "   " + 7 * '-'), end=" | ")
+                            else "      " + 7 * '-'), end=" | ")
         print()
         print(margin + "memory", end=" | ")
         for program in program_group:
             program_mem = program_memory[program]
-            print(util.bold(("%20s" % color_memory(program_mem[0], program_mem[1]))
+            print(util.bold(("%23s" % color_memory(program_mem[0], program_mem[1]))
                             if program_mem[0] < 2 * program_mem[1] and program_mem[0] >= 0
-                            else "   " + 7 * '-'), end=" | ")
+                            else "      " + 7 * '-'), end=" | ")
         print()
         print(8*" ", end=" | ")
         for program in program_group:
-            print(10*" ", end=" | ")
+            print(13*" ", end=" | ")
         print()
 
         def print_group_seperator():
             print(8 * "-", end=" | ")
             for program in program_group:
-                print(10 * "-", end=" | ")
+                print(13 * "-", end=" | ")
             print()
 
         print_group_seperator()
 
         last_group = None
         for test in tests:
             group = package_util.get_group(test, task_id)
@@ -196,25 +229,30 @@
                 last_group = group
 
             print(margin + "%6s" % package_util.extract_test_id(test, task_id), end=" | ")
             for program in program_group:
                 lang = package_util.get_file_lang(program)
                 result = all_results[program][package_util.get_group(test, task_id)][test]
                 status = result.Status
-                if status == Status.PENDING: print(10 * ' ', end=" | ")
+                if status == Status.PENDING: print(13 * ' ', end=" | ")
                 else:
                     print("%3s" % colorize_status(status),
-                         ("%17s" % color_time(result.Time, package_util.get_time_limit(test, config, lang, task_id, args)))
-                         if result.Time is not None else 7*" ", end=" | ")
+                         ("%20s" % color_time(result.Time, package_util.get_time_limit(test, config, lang, task_id, args)))
+                         if result.Time is not None else 10*" ", end=" | ")
             print()
             if not hide_memory:
                 print(8*" ", end=" | ")
                 for program in program_group:
                     lang = package_util.get_file_lang(program)
                     result = all_results[program][package_util.get_group(test, task_id)][test]
+                    if result.Points:
+                        print(colorize_points(result.Points, contest.min_score_per_test(),
+                                              contest.max_score_per_test()).ljust(13), end="")
+                    else:
+                        print(3*" ", end="")
                     print(("%20s" % color_memory(result.Memory, package_util.get_memory_limit(test, config, lang, task_id, args)))
                           if result.Memory is not None else 10*" ", end=" | ")
                 print()
 
         print_table_end()
         print()
 
@@ -247,26 +285,27 @@
         default_timetool = 'oiejq' if util.is_linux() else 'time'
 
         parser.add_argument('-s', '--solutions', type=str, nargs='+',
                             help='solutions to be run, for example prog/abc{b,s}*.{cpp,py}')
         parser.add_argument('-t', '--tests', type=str, nargs='+',
                             help='tests to be run, for example in/abc{0,1}*')
         parser.add_argument('-c', '--cpus', type=int,
-                            help='number of cpus to use, you have %d avaliable' % mp.cpu_count())
+                            help=f'number of cpus to use (default: {util.default_cpu_count()}')
         parser.add_argument('--tl', type=float, help='time limit for all tests (in s)')
         parser.add_argument('--ml', type=float, help='memory limit for all tests (in MB)')
         parser.add_argument('--hide-memory', dest='hide_memory', action='store_true',
                             help='hide memory usage in report')
         parser.add_argument('-T', '--time-tool', dest='time_tool', choices=['oiejq', 'time'],
                             help=f'tool to measure time and memory usage (default: {default_timetool})')
         parser.add_argument('--oiejq-path', dest='oiejq_path', type=str,
                             help='path to oiejq executable (default: `~/.local/bin/oiejq`)')
         parser.add_argument('-a', '--apply-suggestions', dest='apply_suggestions', action='store_true',
                             help='apply suggestions from expected scores report')
         add_compilation_arguments(parser)
+        return parser
 
     def parse_time(self, time_str):
         if len(time_str) < 3: return -1
         return int(time_str[:-2])
 
 
     def parse_memory(self, memory_str):
@@ -275,17 +314,15 @@
 
 
     def extract_file_name(self, file_path):
         return os.path.split(file_path)[1]
 
 
     def get_group(self, test_path):
-        if package_util.extract_test_id(test_path, self.ID).endswith("ocen"):
-            return 0
-        return int("".join(filter(str.isdigit, package_util.extract_test_id(test_path, self.ID))))
+        return package_util.get_group(test_path, self.ID)
 
 
     def get_solution_from_exe(self, executable):
         file = os.path.splitext(executable)[0]
         for ext in self.SOURCE_EXTENSIONS:
             if os.path.isfile(os.path.join(os.getcwd(), "prog", file + ext)):
                 return file + ext
@@ -336,15 +373,15 @@
                 extra_compilation_args.append(os.path.join(os.getcwd(), "prog", file))
 
             for file in self.config.get("extra_compilation_files", []):
                 extra_compilation_files.append(os.path.join(os.getcwd(), "prog", file))
 
         try:
             with open(compile_log_file, "w") as compile_log:
-                compile.compile(source_file, output, self.compilers, compile_log, self.args.weak_compilation_flags,
+                compile.compile(source_file, output, self.compilers, compile_log, self.args.compile_mode,
                                 extra_compilation_args, extra_compilation_files, is_checker=is_checker)
             print(util.info("Compilation of file %s was successful."
                             % package_util.get_file_name(solution)))
             return True
         except CompilationError as e:
             print(util.error("Compilation of file %s was unsuccessful."
                              % package_util.get_file_name(solution)))
@@ -398,48 +435,55 @@
                 correct = util.lines_diff(output, answer_file.readlines())
             return correct, 100 if correct else 0
         else:
             with open(output_file_path, "w") as output_file:
                 output_file.write("\n".join(output) + "\n")
             return self.check_output_checker(name, input_file, output_file_path, answer_file_path)
 
-    def execute_oiejq(self, command, name, result_file_path, input_file_path, output_file_path, answer_file_path,
-                      time_limit, memory_limit, hard_time_limit):
+    def execute_oiejq(self, name, timetool_path, executable, result_file_path, input_file_path, output_file_path, answer_file_path,
+                      time_limit, memory_limit, hard_time_limit, execution_dir):
+        command = f'"{timetool_path}" "{executable}"'
         env = os.environ.copy()
         env["MEM_LIMIT"] = f'{memory_limit}K'
         env["MEASURE_MEM"] = "1"
+        env["UNDER_OIEJQ"] = "1"
 
         timeout = False
-        with open(input_file_path, "r") as input_file:
-            process = subprocess.Popen(command, shell=True, stdin=input_file, stdout=subprocess.PIPE,
-                                       stderr=subprocess.PIPE, env=env, preexec_fn=os.setsid)
+        with open(input_file_path, "r") as input_file, open(output_file_path, "w") as output_file, \
+                open(result_file_path, "w") as result_file:
+            process = subprocess.Popen(command, shell=True, stdin=input_file, stdout=output_file,
+                                       stderr=result_file, env=env, preexec_fn=os.setsid, cwd=execution_dir)
 
             def sigint_handler(signum, frame):
                 try:
                     os.killpg(os.getpgid(process.pid), signal.SIGTERM)
                 except ProcessLookupError:
                     pass
                 sys.exit(1)
             signal.signal(signal.SIGINT, sigint_handler)
 
             try:
-                output, lines = process.communicate(timeout=hard_time_limit)
+                process.wait(timeout=hard_time_limit)
             except subprocess.TimeoutExpired:
                 timeout = True
                 try:
                     os.killpg(os.getpgid(process.pid), signal.SIGTERM)
                 except ProcessLookupError:
                     pass
                 process.communicate()
 
+        with open(result_file_path, "r") as result_file:
+            lines = result_file.read()
+        with open(output_file_path, "r") as output_file:
+            output = output_file.read()
         result = ExecutionResult()
 
         if not timeout:
-            lines = lines.decode('utf-8').splitlines()
-            output = output.decode('utf-8').splitlines()
+            lines = lines.splitlines()
+            output = output.splitlines()
 
             for line in lines:
                 line = line.strip()
                 if ": " in line:
                     (key, value) = line.split(": ")[:2]
                     if key == "Time":
                         result.Time = self.parse_time(value)
@@ -471,23 +515,29 @@
                     result.Error = e.message
         else:
             result.Status = result.Status[:2]
 
         return result
 
 
-    def execute_time(self, command, name, result_file_path, input_file_path, output_file_path, answer_file_path,
-                      time_limit, memory_limit, hard_time_limit):
+    def execute_time(self, name, executable, result_file_path, input_file_path, output_file_path, answer_file_path,
+                      time_limit, memory_limit, hard_time_limit, execution_dir):
+        if sys.platform == 'darwin':
+            time_name = 'gtime'
+        elif sys.platform == 'linux':
+            time_name = 'time'
+        elif sys.platform == 'win32' or sys.platform == 'cygwin':
+            raise Exception("Measuring time with GNU time on Windows is not supported.")
 
-        executable = package_util.get_executable(name)
+        command = [f'{time_name}', '-f', '%U\\n%M\\n%x', '-o', result_file_path, executable]
         timeout = False
         mem_limit_exceeded = False
-        with open(input_file_path, "r") as input_file:
-            process = subprocess.Popen(command, stdin=input_file, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL,
-                                       preexec_fn=os.setsid)
+        with open(input_file_path, "r") as input_file, open(output_file_path, "w") as output_file:
+            process = subprocess.Popen(command, stdin=input_file, stdout=output_file, stderr=subprocess.DEVNULL,
+                                       preexec_fn=os.setsid, cwd=execution_dir)
 
             def sigint_handler(signum, frame):
                 try:
                     os.killpg(os.getpgid(process.pid), signal.SIGTERM)
                 except ProcessLookupError:
                     pass
                 sys.exit(1)
@@ -515,20 +565,21 @@
                 if time.time() - start_time > hard_time_limit:
                     try:
                         os.killpg(os.getpgid(process.pid), signal.SIGTERM)
                     except ProcessLookupError:
                         pass
                     timeout = True
                     break
-            output, _ = process.communicate()
 
+        with open(output_file_path, "r") as output_file:
+            output = output_file.read()
         result = ExecutionResult()
         program_exit_code = None
         if not timeout:
-            output = output.decode("utf-8").splitlines()
+            output = output.splitlines()
             with open(result_file_path, "r") as result_file:
                 lines = result_file.readlines()
             if len(lines) == 3:
                 """
                 If programs runs successfully, the output looks like this:
                  - first line is CPU time in seconds
                  - second line is memory in KB
@@ -543,15 +594,15 @@
                 If there was a runtime error, the first line is the error message with signal number.
                 For example:
                     Command terminated by signal 11
                 """
                 program_exit_code = int(lines[0].strip().split(" ")[-1])
             elif not mem_limit_exceeded:
                 result.Status = Status.RE
-                result.Error = "Unexpected output from time command: " + "\n".join(lines)
+                result.Error = "Unexpected output from time command: " + "".join(lines)
                 return result
 
         if program_exit_code is not None and program_exit_code != 0:
             result.Status = Status.RE
         elif timeout:
             result.Status = Status.TL
         elif mem_limit_exceeded:
@@ -577,49 +628,44 @@
 
 
     def run_solution(self, data_for_execution: ExecutionData):
         """
         Run an execution and return the result as ExecutionResult object.
         """
 
-        (name, executable, test, time_limit, memory_limit, timetool_path) = data_for_execution
+        (name, executable, test, time_limit, memory_limit, timetool_path, execution_dir) = data_for_execution
         file_no_ext = paths.get_executions_path(name, package_util.extract_test_id(test, self.ID))
         output_file = file_no_ext + ".out"
         result_file = file_no_ext + ".res"
         hard_time_limit_in_s = math.ceil(2 * time_limit / 1000.0)
 
         if self.timetool_name == 'oiejq':
-            command = f'"{timetool_path}" "{executable}"'
-
-            return self.execute_oiejq(command, name, result_file, test, output_file, self.get_output_file(test),
-                                      time_limit, memory_limit, hard_time_limit_in_s)
+            return self.execute_oiejq(name, timetool_path, executable, result_file, test, output_file, self.get_output_file(test),
+                                      time_limit, memory_limit, hard_time_limit_in_s, execution_dir)
         elif self.timetool_name == 'time':
-            if sys.platform == 'darwin':
-                timeout_name = 'gtimeout'
-                time_name = 'gtime'
-            elif sys.platform == 'linux':
-                timeout_name = 'timeout'
-                time_name = 'time'
-            elif sys.platform == 'win32' or sys.platform == 'cygwin':
-                raise Exception("Measuring time with GNU time on Windows is not supported.")
-
-            command = [f'{time_name}', '-f', '%U\\n%M\\n%x', '-o', result_file, executable]
-            return self.execute_time(command, name, result_file, test, output_file, self.get_output_file(test),
-                                     time_limit, memory_limit, hard_time_limit_in_s)
+            return self.execute_time(name, executable, result_file, test, output_file, self.get_output_file(test),
+                                     time_limit, memory_limit, hard_time_limit_in_s, execution_dir)
 
-    def run_solutions(self, compiled_commands, names, solutions):
+    def run_solutions(self, compiled_commands, names, solutions, executables_dir):
         """
         Run solutions on tests and print the results as a table to stdout.
         """
 
         executions = []
         all_cache_files: Dict[str, CacheFile] = {}
         all_results = collections.defaultdict(
             lambda: collections.defaultdict(lambda: collections.defaultdict(map)))
 
+        for lang, files in self.config.get('extra_execution_files', {}).items():
+            for file in files:
+                shutil.copy(os.path.join(os.getcwd(), "prog", file), executables_dir)
+        # Copy swig generated .so files
+        for file in glob.glob(os.path.join(os.getcwd(), "prog", f"_{self.ID}lib.so")):
+            shutil.copy(file, executables_dir)
+
         for (name, executable, result) in compiled_commands:
             lang = package_util.get_file_lang(name)
             solution_cache = cache.get_cache_file(os.path.join(os.getcwd(), "prog", name))
             all_cache_files[name] = solution_cache
 
             if result:
                 for test in self.tests:
@@ -629,15 +675,15 @@
                     test_result: CacheTest = solution_cache.tests.get(self.test_md5sums[os.path.basename(test)], None)
                     if test_result is not None and test_result.time_limit == test_time_limit and \
                             test_result.memory_limit == test_memory_limit and \
                             test_result.time_tool == self.timetool_name:
                         all_results[name][self.get_group(test)][test] = test_result.result
                     else:
                         executions.append((name, executable, test, test_time_limit, test_memory_limit,
-                                           self.timetool_path))
+                                           self.timetool_path, os.path.dirname(executable)))
                         all_results[name][self.get_group(test)][test] = ExecutionResult(Status.PENDING)
                 os.makedirs(paths.get_executions_path(name), exist_ok=True)
             else:
                 for test in self.tests:
                     all_results[name][self.get_group(test)][test] = ExecutionResult(Status.CE)
         print()
         executions.sort(key = lambda x: (package_util.get_executable_key(x[1], self.ID), x[2]))
@@ -702,15 +748,15 @@
         for i in range(len(solutions)):
             if not compilation_results[i]:
                 self.failed_compilations.append(solutions[i])
         os.makedirs(paths.get_executions_path(), exist_ok=True)
         executables = [paths.get_executables_path(package_util.get_executable(solution)) for solution in solutions]
         compiled_commands = zip(solutions, executables, compilation_results)
         names = solutions
-        return self.run_solutions(compiled_commands, names, solutions)
+        return self.run_solutions(compiled_commands, names, solutions, paths.get_executables_path())
 
     def convert_status_to_string(self, dictionary):
         """
         Converts all `Status` enums in dict to strings.
         """
         def _convert(obj):
             if isinstance(obj, dict):
@@ -823,14 +869,15 @@
 
         expected_scores_diff = dictdiffer.diff(expected_scores, new_expected_scores)
         added_solutions = set()
         removed_solutions = set()
         added_groups = set()
         removed_groups = set()
         changes = []
+        unknown_change = False
 
         for type, field, change in list(expected_scores_diff):
             if type == "add":
                 if field == '': # Solutions were added
                     for solution in change:
                         added_solutions.add(solution[0])
                 elif field[1] == "expected": # Groups were added
@@ -873,30 +920,45 @@
                     else:
                         changes.append(ResultChange(
                             solution=solution,
                             group=group,
                             old_result=change[0],
                             result=change[1]
                         ))
+                elif field[1] == "points": # Points for at least one solution has changed
+                    solution = field[0]
+                    changes.append(TotalPointsChange(
+                        solution=solution,
+                        old_points=change[0],
+                        new_points=change[1]
+                    ))
+                else:
+                    unknown_change = True
+
 
         return ValidationResult(
             added_solutions,
             removed_solutions,
             added_groups,
             removed_groups,
             changes,
             expected_scores,
-            new_expected_scores
+            new_expected_scores,
+            unknown_change,
         )
 
 
     def print_expected_scores_diff(self, validation_results: ValidationResult):
         diff = validation_results
         config_expected_scores = self.config.get("sinol_expected_scores", {})
 
+        if diff.unknown_change:
+            print(util.error("There was an unknown change in expected scores. "
+                             "You should apply the suggested changes to avoid errors."))
+
         def warn_if_not_empty(set, message):
             if len(set) > 0:
                 print(util.warning(message + ": "), end='')
                 print(util.warning(", ".join([str(x) for x in set])))
 
         warn_if_not_empty(diff.added_solutions, "Solutions were added")
         warn_if_not_empty(diff.removed_solutions, "Solutions were removed")
@@ -912,16 +974,19 @@
                 if isinstance(change.result, str):
                     print(util.warning("Solution %s passed group %d with status %s while it should pass with status %s." %
                                        (change.solution, change.group, change.result, change.old_result)))
                 elif isinstance(change.result, int):
                     print_points_change(change.solution, change.group, change.result, change.old_result)
             elif isinstance(change, PointsChange):
                 print_points_change(change.solution, change.group, change.new_points, change.old_points)
+            elif isinstance(change, TotalPointsChange):
+                print(util.warning("Solution %s passed all groups with %d points while it should pass with %d points." %
+                                   (change.solution, change.new_points, change.old_points)))
 
-        if diff.expected_scores == diff.new_expected_scores:
+        if diff.expected_scores == diff.new_expected_scores and not diff.unknown_change:
             print(util.info("Expected scores are correct!"))
         else:
             def delete_group(solution, group):
                 if group in config_expected_scores[solution]["expected"]:
                     del config_expected_scores[solution]["expected"][group]
                     config_expected_scores[solution]["points"] = self.contest.get_global_score(
                         config_expected_scores[solution]["expected"],
@@ -931,15 +996,14 @@
             def set_group_result(solution, group, result):
                 config_expected_scores[solution]["expected"][group] = result
                 config_expected_scores[solution]["points"] = self.contest.get_global_score(
                     config_expected_scores[solution]["expected"],
                     self.possible_score
                 )
 
-
             if self.args.apply_suggestions:
                 for solution in diff.removed_solutions:
                     del config_expected_scores[solution]
 
                 for solution in config_expected_scores:
                     for group in diff.removed_groups:
                         delete_group(solution, group)
@@ -947,15 +1011,14 @@
                 for solution in diff.new_expected_scores.keys():
                     if solution in config_expected_scores:
                         for group, result in diff.new_expected_scores[solution]["expected"].items():
                             set_group_result(solution, group, result)
                     else:
                         config_expected_scores[solution] = diff.new_expected_scores[solution]
 
-
                 self.config["sinol_expected_scores"] = self.convert_status_to_string(config_expected_scores)
                 util.save_config(self.config)
                 print(util.info("Saved suggested expected scores description."))
             else:
                 util.exit_with_error("Use flag --apply-suggestions to apply suggestions.")
 
 
@@ -1099,48 +1162,65 @@
         checker_basename = os.path.basename(self.checker)
         self.checker_executable = paths.get_executables_path(checker_basename + ".e")
 
         checker_compilation = self.compile_solutions([self.checker], is_checker=True)
         if not checker_compilation[0]:
             util.exit_with_error('Checker compilation failed.')
 
+    def check_had_checker(self, has_checker):
+        """
+        Checks if there was a checker and if it is now removed (or the other way around) and if so, removes tests cache.
+        In theory, removing cache after adding a checker is redundant, because during its compilation, the cache is
+        removed.
+        """
+        had_checker = os.path.exists(paths.get_cache_path("checker"))
+        if (had_checker and not has_checker) or (not had_checker and has_checker):
+            cache.remove_results_cache()
+        if has_checker:
+            with open(paths.get_cache_path("checker"), "w") as f:
+                f.write("")
+        else:
+            try:
+                os.remove(paths.get_cache_path("checker"))
+            except FileNotFoundError:
+                pass
+
+
     def run(self, args):
-        util.exit_if_not_package()
+        args = util.init_package_command(args)
 
         self.set_constants()
         package_util.validate_test_names(self.ID)
         self.args = args
-        with open(os.path.join(os.getcwd(), "config.yml"), 'r') as config:
-            try:
-                self.config = yaml.load(config, Loader=yaml.FullLoader)
-            except AttributeError:
-                self.config = yaml.load(config)
-
+        self.config = package_util.get_config()
         try:
             self.contest = contest_types.get_contest_type()
         except UnknownContestType as e:
             util.exit_with_error(str(e))
 
         if not 'title' in self.config.keys():
             util.exit_with_error('Title was not defined in config.yml.')
 
         self.compilers, self.timetool_path, self.timetool_name = self.validate_arguments(args)
 
         title = self.config["title"]
         print("Task: %s (tag: %s)" % (title, self.ID))
-        self.cpus = args.cpus or mp.cpu_count()
-        cache.save_to_cache_extra_compilation_files(self.config.get("extra_compilation_files", []), self.ID)
+        self.cpus = args.cpus or util.default_cpu_count()
+        cache.process_extra_compilation_files(self.config.get("extra_compilation_files", []), self.ID)
+        cache.process_extra_execution_files(self.config.get("extra_execution_files", {}), self.ID)
+        cache.remove_results_if_contest_type_changed(self.config.get("sinol_contest_type", "default"))
 
         checker = package_util.get_files_matching_pattern(self.ID, f'{self.ID}chk.*')
         if len(checker) != 0:
             print(util.info("Checker found: %s" % os.path.basename(checker[0])))
             self.checker = checker[0]
             self.compile_checker()
         else:
             self.checker = None
+        self.check_had_checker(self.checker is not None)
 
         lib = package_util.get_files_matching_pattern(self.ID, f'{self.ID}lib.*')
         self.has_lib = len(lib) != 0
 
         self.tests = package_util.get_tests(self.ID, self.args.tests)
         self.test_md5sums = {os.path.basename(test): util.get_file_md5(test) for test in self.tests}
         self.check_are_any_tests_to_run()
@@ -1154,10 +1234,19 @@
             for test in self.tests:
                 # The functions will exit if the limits are not set
                 _ = package_util.get_time_limit(test, self.config, lang, self.ID, self.args)
                 _ = package_util.get_memory_limit(test, self.config, lang, self.ID, self.args)
 
         results, all_results = self.compile_and_run(solutions)
         self.check_errors(all_results)
-        validation_results = self.validate_expected_scores(results)
+        try:
+            validation_results = self.validate_expected_scores(results)
+        except Exception:
+            self.config = util.try_fix_config(self.config)
+            try:
+                validation_results = self.validate_expected_scores(results)
+            except Exception:
+                util.exit_with_error("Validating expected scores failed. "
+                                     "This probably means that `sinol_expected_scores` is broken. "
+                                     "Delete it and run `sinol-make run --apply-suggestions` again.")
         self.print_expected_scores_diff(validation_results)
         self.exit()
```

### Comparing `sinol_make-1.5.9/src/sinol_make/contest_types/icpc.py` & `sinol_make-1.6.0.dev1/src/sinol_make/contest_types/icpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,7 +25,13 @@
             return 0
 
     def get_group_score(self, test_scores, group_max_score):
         return min(test_scores)
 
     def get_global_score(self, groups_scores: Dict[int, Dict], global_max_score):
         return min(group["points"] for group in groups_scores.values())
+
+    def min_score_per_test(self):
+        return 0
+
+    def max_score_per_test(self):
+        return 1
```

### Comparing `sinol_make-1.5.9/src/sinol_make/helpers/cache.py` & `sinol_make-1.6.0.dev1/src/sinol_make/helpers/cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -57,46 +57,124 @@
     """
     Save the compiled executable path to cache in `.cache/md5sums/<basename of file_path>`,
     which contains the md5sum of the file and the path to the executable.
     :param file_path: Path to the file
     :param exe_path: Path to the compiled executable
     :param is_checker: Whether the compiled file is a checker. If True, all cached tests are removed.
     """
-    info = get_cache_file(file_path)
+    info = CacheFile()
     info.executable_path = exe_path
     info.md5sum = util.get_file_md5(file_path)
     info.save(file_path)
 
     if is_checker:
+        remove_results_cache()
+
+
+def _check_file_changed(file_path, lang, task_id):
+    solutions_re = package_util.get_solutions_re(task_id)
+    md5sum = util.get_file_md5(file_path)
+    info = get_cache_file(file_path)
+
+    if info.md5sum != md5sum:
         for solution in os.listdir(paths.get_cache_path('md5sums')):
-            info = get_cache_file(solution)
-            info.tests = {}
-            info.save(solution)
+            # Remove only files in the same language and matching the solution regex
+            if package_util.get_file_lang(solution) == lang and \
+                    solutions_re.match(solution) is not None:
+                os.unlink(paths.get_cache_path('md5sums', solution))
+
+    info.md5sum = md5sum
+    info.save(file_path)
 
 
-def save_to_cache_extra_compilation_files(extra_compilation_files, task_id):
+def process_extra_compilation_files(extra_compilation_files, task_id):
     """
     Checks if extra compilation files have changed and saves them to cache.
     If they have, removes all cached solutions that use them.
     :param extra_compilation_files: List of extra compilation files
     :param task_id: Task id
     """
-    solutions_re = package_util.get_solutions_re(task_id)
     for file in extra_compilation_files:
         file_path = os.path.join(os.getcwd(), "prog", file)
         if not os.path.exists(file_path):
             continue
         md5sum = util.get_file_md5(file_path)
         lang = package_util.get_file_lang(file)
         if lang == 'h':
             lang = 'cpp'
+        _check_file_changed(file_path, lang, task_id)
+
+
+def process_extra_execution_files(extra_execution_files, task_id):
+    """
+    Checks if extra execution files have changed and saves them to cache.
+    If they have, removes all cached solutions that use them.
+    :param extra_execution_files: List of extra execution files
+    :param task_id: Task id
+    """
+    for lang, files in extra_execution_files.items():
+        for file in files:
+            file_path = os.path.join(os.getcwd(), "prog", file)
+            if not os.path.exists(file_path):
+                continue
+            _check_file_changed(file_path, lang, task_id)
+
+
+def remove_results_cache():
+    """
+    Removes all cached test results
+    """
+    for solution in os.listdir(paths.get_cache_path('md5sums')):
+        info = get_cache_file(solution)
+        info.tests = {}
+        info.save(solution)
+
+
+def remove_results_if_contest_type_changed(contest_type):
+    """
+    Checks if contest type has changed and removes all cached test results if it has.
+    :param contest_type: Contest type
+    """
+    if package_util.check_if_contest_type_changed(contest_type):
+        remove_results_cache()
+    package_util.save_contest_type_to_cache(contest_type)
+
+
+def check_can_access_cache():
+    """
+    Checks if user can access cache.
+    """
+    try:
+        os.makedirs(paths.get_cache_path(), exist_ok=True)
+        with open(paths.get_cache_path("test"), "w") as f:
+            f.write("test")
+        os.unlink(paths.get_cache_path("test"))
+    except PermissionError:
+        util.exit_with_error("You don't have permission to access the `.cache/` directory. "
+                             "`sinol-make` needs to be able to write to this directory.")
+
+
+def has_file_changed(file_path: str) -> bool:
+    """
+    Checks if file has changed since last compilation.
+    :param file_path: Path to the file
+    :return: True if file has changed, False otherwise
+    """
+    try:
         info = get_cache_file(file_path)
+        return info.md5sum != util.get_file_md5(file_path)
+    except FileNotFoundError:
+        return True
 
-        if info.md5sum != md5sum:
-            for solution in os.listdir(paths.get_cache_path('md5sums')):
-                # Remove only files in the same language and matching the solution regex
-                if package_util.get_file_lang(solution) == lang and \
-                        solutions_re.match(solution) is not None:
-                    os.unlink(paths.get_cache_path('md5sums', solution))
 
-        info.md5sum = md5sum
-        info.save(file_path)
+def check_correct_solution(task_id: str):
+    """
+    Checks if correct solution has changed. If it did, removes cache for input files.
+    :param task_id: Task id
+    """
+    try:
+        solution = package_util.get_correct_solution(task_id)
+    except FileNotFoundError:
+        return
+
+    if has_file_changed(solution) and os.path.exists(os.path.join(os.getcwd(), 'in', '.md5sums')):
+        os.unlink(os.path.join(os.getcwd(), 'in', '.md5sums'))
```

### Comparing `sinol_make-1.5.9/src/sinol_make/helpers/compile.py` & `sinol_make-1.6.0.dev1/src/sinol_make/helpers/compile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from typing import Tuple, Union
 import os
 import sys
 import shutil
 import stat
 import subprocess
-import yaml
 
 import sinol_make.helpers.compiler as compiler
+from sinol_make import util
 from sinol_make.helpers import paths
-from sinol_make.helpers.cache import check_compiled, save_compiled
+from sinol_make.helpers.cache import check_compiled, save_compiled, package_util
 from sinol_make.interfaces.Errors import CompilationError
 from sinol_make.structs.compiler_structs import Compilers
 
 
-def compile(program, output, compilers: Compilers = None, compile_log = None, weak_compilation_flags = False,
-            extra_compilation_args = None, extra_compilation_files = None, is_checker = False):
+def compile(program, output, compilers: Compilers = None, compile_log=None, compilation_flags='default',
+            extra_compilation_args=None, extra_compilation_files=None, is_checker=False, use_fsanitize=False):
     """
     Compile a program.
     :param program: Path to the program to compile
     :param output: Path to the output file
     :param compilers: Compilers object
     :param compile_log: File to write the compilation log to
-    :param weak_compilation_flags: If True, disable all warnings
+    :param compilation_flags: Group of compilation flags to use
     :param extra_compilation_args: Extra compilation arguments
     :param extra_compilation_files: Extra compilation files
     :param is_checker: Set to True if compiling a checker. This will remove all cached test results.
+    :param use_fsanitize: Whether to use fsanitize when compiling C/C++ programs. Sanitizes address and undefined behavior.
     """
     if extra_compilation_args is None:
         extra_compilation_args = []
     if isinstance(extra_compilation_args, str):
         extra_compilation_args = [extra_compilation_args]
     assert isinstance(extra_compilation_args, list) and all(isinstance(arg, str) for arg in extra_compilation_args)
 
+    # Address and undefined sanitizer is not yet supported on Apple Silicon.
+    if use_fsanitize and util.is_macos_arm():
+        use_fsanitize = False
+
     if extra_compilation_files is None:
         extra_compilation_files = []
 
     compiled_exe = check_compiled(program)
     if compiled_exe is not None:
         if compile_log is not None:
             compile_log.write(f'Using cached executable {compiled_exe}\n')
@@ -43,34 +48,45 @@
         if os.path.abspath(compiled_exe) != os.path.abspath(output):
             shutil.copy(compiled_exe, output)
         return True
 
     for file in extra_compilation_files:
         shutil.copy(file, os.path.join(os.path.dirname(output), os.path.basename(file)))
 
-    gcc_compilation_flags = '-Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'
-    if weak_compilation_flags:
-        gcc_compilation_flags = '-w'  # Disable all warnings
+    gcc_compilation_flags = ''
+    if compilation_flags == 'weak' or compilation_flags == 'w':
+        compilation_flags = 'weak'
+        gcc_compilation_flags = ''  # Disable all warnings
+    elif compilation_flags == 'oioioi' or compilation_flags == 'o':
+        gcc_compilation_flags = ' -Wall -Wno-unused-result -Werror'  # Same flags as oioioi
+    elif compilation_flags == 'default' or compilation_flags == 'd':
+        gcc_compilation_flags = ' -Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'
+    else:
+        util.exit_with_error(f'Unknown compilation flags group: {compilation_flags}')
 
     if compilers is None:
         compilers = Compilers()
 
     ext = os.path.splitext(program)[1]
-    arguments = []
     if ext == '.cpp':
         arguments = [compilers.cpp_compiler_path or compiler.get_cpp_compiler_path(), program] + \
                     extra_compilation_args + ['-o', output] + \
-                    f'--std=c++20 -O3 -lm {gcc_compilation_flags} -fdiagnostics-color'.split(' ')
+                    f'--std=c++20 -O3 -lm{gcc_compilation_flags} -fdiagnostics-color'.split(' ')
+        if use_fsanitize and compilation_flags != 'weak':
+            arguments += ['-fsanitize=address,undefined', '-fno-sanitize-recover']
     elif ext == '.c':
         arguments = [compilers.c_compiler_path or compiler.get_c_compiler_path(), program] + \
                     extra_compilation_args + ['-o', output] + \
-                    f'--std=gnu99 -O3 -lm {gcc_compilation_flags} -fdiagnostics-color'.split(' ')
+                    f'--std=gnu99 -O3 -lm{gcc_compilation_flags} -fdiagnostics-color'.split(' ')
+        if use_fsanitize and compilation_flags != 'weak':
+            arguments += ['-fsanitize=address,undefined', '-fno-sanitize-recover']
     elif ext == '.py':
         if sys.platform == 'win32' or sys.platform == 'cygwin':
             # TODO: Make this work on Windows
+            print(util.error('Python is not supported on Windows'))
             pass
         else:
             with open(output, 'w') as output_file, open(program, 'r') as program_file:
                 output_file.write('#!/usr/bin/python3\n')
                 output_file.write(program_file.read())
 
             st = os.stat(output)
@@ -78,68 +94,74 @@
         arguments = [compilers.python_interpreter_path, '-m', 'py_compile', program]
     elif ext == '.java':
         raise NotImplementedError('Java compilation is not implemented')
     else:
         raise CompilationError('Unknown file extension: ' + ext)
 
     process = subprocess.Popen(arguments, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-    process.wait()
     out, _ = process.communicate()
     if compile_log is not None:
         compile_log.write(out.decode('utf-8'))
         compile_log.close()
     else:
         print(out.decode('utf-8'))
 
     if process.returncode != 0:
         raise CompilationError('Compilation failed')
     else:
         save_compiled(program, output, is_checker)
         return True
 
 
-def compile_file(file_path: str, name: str, compilers: Compilers, weak_compilation_flags = False) \
+def compile_file(file_path: str, name: str, compilers: Compilers, compilation_flags='default',
+                 use_fsanitize=False, additional_flags=None) \
         -> Tuple[Union[str, None], str]:
     """
     Compile a file
     :param file_path: Path to the file to compile
     :param name: Name of the executable
     :param compilers: Compilers object
-    :param weak_compilation_flags: Use weaker compilation flags
+    :param compilation_flags: Group of compilation flags to use
+    :param use_fsanitize: Whether to use fsanitize when compiling C/C++ programs. Sanitizes address and undefined behavior.
+    :param additional_flags: Additional flags for c / c++ compiler.
     :return: Tuple of (executable path or None if compilation failed, log path)
     """
     os.makedirs(paths.get_executables_path(), exist_ok=True)
     os.makedirs(paths.get_compilation_log_path(), exist_ok=True)
 
-    with open(os.path.join(os.getcwd(), "config.yml"), "r") as config_file:
-        config = yaml.load(config_file, Loader=yaml.FullLoader)
+    config = package_util.get_config()
 
     extra_compilation_files = [os.path.join(os.getcwd(), "prog", file)
                                for file in config.get("extra_compilation_files", [])]
     lang = os.path.splitext(file_path)[1][1:]
     args = config.get('extra_compilation_args', {}).get(lang, [])
     if isinstance(args, str):
         args = [args]
     extra_compilation_args = [os.path.join(os.getcwd(), "prog", file) for file in args]
+    if additional_flags is not None:
+        extra_compilation_args.append(additional_flags)
 
     output = paths.get_executables_path(name)
     compile_log_path = paths.get_compilation_log_path(os.path.splitext(name)[0] + '.compile_log')
     with open(compile_log_path, 'w') as compile_log:
         try:
-            if compile(file_path, output, compilers, compile_log, weak_compilation_flags, extra_compilation_args,
-                       extra_compilation_files):
+            if compile(file_path, output, compilers, compile_log, compilation_flags, extra_compilation_args,
+                       extra_compilation_files, use_fsanitize=use_fsanitize):
                 return output, compile_log_path
         except CompilationError:
             pass
         return None, compile_log_path
 
 
 def print_compile_log(compile_log_path: str):
     """
     Print the first 500 lines of compilation log
     :param compile_log_path: path to the compilation log
     """
+    lines_to_print = 500
 
     with open(compile_log_path, 'r') as compile_log:
         lines = compile_log.readlines()
-        for line in lines[:500]:
+        for line in lines[:lines_to_print]:
             print(line, end='')
+        if len(lines) > lines_to_print:
+            print(util.error(f"Compilation log too long. Whole log file at: {compile_log_path}"))
```

### Comparing `sinol_make-1.5.9/src/sinol_make/helpers/compiler.py` & `sinol_make-1.6.0.dev1/src/sinol_make/helpers/compiler.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.5.9/src/sinol_make/helpers/paths.py` & `sinol_make-1.6.0.dev1/src/sinol_make/helpers/paths.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.5.9/src/sinol_make/helpers/printer.py` & `sinol_make-1.6.0.dev1/src/sinol_make/helpers/printer.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.5.9/src/sinol_make/oiejq/__init__.py` & `sinol_make-1.6.0.dev1/src/sinol_make/oiejq/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     # that the package creator might want to look into.
     with tempfile.TemporaryDirectory() as tmpdir:
         oiejq_path = os.path.join(tmpdir, 'oiejq.tar.gz')
         with open(oiejq_path, 'wb') as oiejq_file:
             oiejq_file.write(request.content)
 
         with tarfile.open(oiejq_path) as tar:
-            tar.extractall(path=tmpdir)
+            util.extract_tar(tar, tmpdir)
         shutil.copy(os.path.join(tmpdir, 'oiejq', 'oiejq.sh'), os.path.expanduser('~/.local/bin/oiejq'))
         shutil.copy(os.path.join(tmpdir, 'oiejq', 'sio2jail'), os.path.expanduser('~/.local/bin/'))
 
     return check_oiejq()
 
 
 def get_oiejq_path():
```

### Comparing `sinol_make-1.5.9/src/sinol_make/structs/cache_structs.py` & `sinol_make-1.6.0.dev1/src/sinol_make/structs/cache_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.5.9/src/sinol_make/structs/compiler_structs.py` & `sinol_make-1.6.0.dev1/src/sinol_make/structs/compiler_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.5.9/src/sinol_make/structs/inwer_structs.py` & `sinol_make-1.6.0.dev1/src/sinol_make/structs/inwer_structs.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 
     # Dictionary with test path as key and verification result as value.
     results: Dict[str, TestResult]
 
     # Number of executions finished
     i: int
 
+    # Task id
+    task_id: str
+
 @dataclass
 class InwerExecution:
     test_path: str
     test_name: str
     inwer_exe_path: str
 
 @dataclass
```

### Comparing `sinol_make-1.5.9/src/sinol_make/structs/run_structs.py` & `sinol_make-1.6.0.dev1/src/sinol_make/structs/run_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.5.9/src/sinol_make/structs/status_structs.py` & `sinol_make-1.6.0.dev1/src/sinol_make/structs/status_structs.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,24 +33,34 @@
         elif status == "OK":
             return Status.OK
         elif status == "  ":
             return Status.PENDING
         else:
             raise ValueError(f"Unknown status: '{status}'")
 
+    @staticmethod
+    def possible_statuses():
+        return [Status.PENDING, Status.CE, Status.TL, Status.ML, Status.RE, Status.WA, Status.OK]
+
 
 @dataclass
 class ResultChange:
     solution: str
     group: int
     old_result: Status
     result: Status
 
 
 @dataclass
+class TotalPointsChange:
+    solution: str
+    old_points: int
+    new_points: int
+
+@dataclass
 class PointsChange:
     solution: str
     group: int
     old_points: int
     new_points: int
 
 
@@ -59,14 +69,15 @@
     added_solutions: set
     removed_solutions: set
     added_groups: set
     removed_groups: set
     changes: List[ResultChange]
     expected_scores: dict
     new_expected_scores: dict
+    unknown_change: bool
 
 
 @dataclass
 class ExecutionResult:
     # Result status of execution. Possible values
     #  can be found in `Status` enum definition.
     Status: Status
```

### Comparing `sinol_make-1.5.9/src/sinol_make/util.py` & `sinol_make-1.6.0.dev1/src/sinol_make/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 import glob, importlib, os, sys, requests, yaml
+import math
+import multiprocessing
 import platform
-import tempfile
-import shutil
+import tarfile
 import hashlib
-import subprocess
-import threading
+import multiprocessing
 import resource
 from typing import Union
+from packaging.version import parse as parse_version
 
-import sinol_make
 from sinol_make.contest_types import get_contest_type
+from sinol_make.helpers import paths, cache
+from sinol_make.structs.status_structs import Status
+
+
+__cache = {}
 
 
 def get_commands():
     """
     Function to get an array of all available commands.
     """
+    global __cache
+    if 'commands' in __cache:
+        return __cache['commands']
     commands_path = glob.glob(
         os.path.join(
             os.path.dirname(os.path.realpath(__file__)),
             'commands/*'
         )
     )
     commands = []
     for path in commands_path:
         temp = importlib.import_module('sinol_make.commands.' + os.path.basename(path), 'Command')
         commands.append(temp.Command())
 
+    __cache['commands'] = commands
     return commands
 
 
+def get_command_names():
+    """
+    Function to get an array of all available command names.
+    """
+    return [command.get_name() for command in get_commands()]
+
+
 def find_and_chdir_package():
     """
     Checks if current directory or parent directory is a package directory.
     If it is, it changes the current working directory to it and returns True.
     If it isn't, it returns False.
     """
     if os.path.exists(os.path.join(os.getcwd(), 'config.yml')):
@@ -41,22 +57,34 @@
     elif os.path.exists(os.path.join(os.getcwd(), '..', 'config.yml')):
         os.chdir('..')
         return True
     else:
         return False
 
 
+def init_package_command(args):
+    """
+    Updates arguments with contest specific overrides for commands
+    that require being in package directory
+    """
+    exit_if_not_package()
+    contest = get_contest_type()
+    contest.verify_config()
+    return contest.argument_overrides(args)
+
+
 def exit_if_not_package():
     """
     Checks if current directory or parent directory is a package directory.
     If it is, current working directory is changed to it.
     If it isn't, it exits with an error.
     """
     if not find_and_chdir_package():
         exit_with_error('You are not in a package directory (couldn\'t find config.yml in current directory).')
+    cache.check_can_access_cache()
 
 
 def save_config(config):
     """
     Function to save nicely formated config.yml.
     """
 
@@ -83,34 +111,34 @@
         {
             "key": "extra_compilation_args",
             "default_flow_style": None
         },
         {
             "key": "sinol_expected_scores",
             "default_flow_style": None
-        }
+        },
     ]
 
     config = config.copy()
     with open("config.yml", "w") as config_file:
         for field in order:
             if isinstance(field, dict): # If the field is a dict, it means that it has a custom property (for example default_flow_style).
                 if field["key"] in config:
-                    yaml.dump({field["key"]: config[field["key"]]}, config_file, default_flow_style=field["default_flow_style"])
+                    yaml.dump({field["key"]: config[field["key"]]}, config_file, default_flow_style=field["default_flow_style"], allow_unicode=True)
                     # The considered fields are deleted, thus `config` at the end will contain only custom fields written by the user.
                     del config[field["key"]]
             else: # When the field is a string, it doesn't have any custom properties, so it's just a dict key.
                 if field in config:
-                    yaml.dump({field: config[field]}, config_file)
+                    yaml.dump({field: config[field]}, config_file, allow_unicode=True)
                     del config[field] # Same reason for deleting as above.
 
         if config != {}:
             print(warning("Found unknown fields in config.yml: " + ", ".join([str(x) for x in config])))
             # All remaining non-considered fields are appended to the end of the file.
-            yaml.dump(config, config_file)
+            yaml.dump(config, config_file, allow_unicode=True)
 
 
 def import_importlib_resources():
     """
     Function to import importlib_resources.
     For Python 3.8 and below, we use importlib_resources.
     For Python 3.9 and above, we use importlib.resources.
@@ -119,41 +147,58 @@
     if python_version.minor <= 8:
         import importlib_resources as importlib
     else:
         import importlib.resources as importlib
     return importlib
 
 
-def check_for_updates(current_version) -> Union[str, None]:
+def is_dev(version):
+    """
+    Function to check if the version is a development version.
+    """
+    return parse_version(version).is_devrelease
+
+
+def check_for_updates(current_version, check=True) -> Union[str, None]:
     """
     Function to check if there is a new version of sinol-make.
     :param current_version: current version of sinol-make
+    :param check: whether to check for new version
     :return: returns new version if there is one, None otherwise
     """
     importlib = import_importlib_resources()
 
     data_dir = importlib.files("sinol_make").joinpath("data")
     if not data_dir.is_dir():
         os.mkdir(data_dir)
 
     # We check for new version asynchronously, so that it doesn't slow down the program.
-    thread = threading.Thread(target=check_version)
-    thread.start()
+    # If the main process exits, the check_version process will also exit.
+    if check:
+        process = multiprocessing.Process(target=check_version, daemon=True)
+        process.start()
     version_file = data_dir.joinpath("version")
 
-    if version_file.is_file():
+    try:
         version = version_file.read_text()
+    except (PermissionError, FileNotFoundError):
         try:
-            if compare_versions(current_version, version) == -1:
-                return version
-            else:
-                return None
-        except ValueError:  # If the version file is corrupted, we just ignore it.
+            with open(paths.get_cache_path("sinol_make_version"), "r") as f:
+                version = f.read()
+        except (FileNotFoundError, PermissionError):
             return None
-    else:
+
+    try:
+        if not is_dev(version) and parse_version(version) > parse_version(current_version):
+            return version
+        if is_dev(current_version) and is_dev(version) and parse_version(version) > parse_version(current_version):
+            return version
+        else:
+            return None
+    except ValueError:  # If the version file is corrupted, we just ignore it.
         return None
 
 
 def check_version():
     """
     Function that asynchronously checks for new version of sinol-make.
     Writes the newest version to data/version file.
@@ -168,35 +213,24 @@
     if request.status_code != 200:
         return
 
     data = request.json()
     latest_version = data["info"]["version"]
 
     version_file = importlib.files("sinol_make").joinpath("data/version")
-    version_file.write_text(latest_version)
-
-
-def compare_versions(version_a, version_b):
-    """
-    Function to compare two versions.
-    Returns 1 if version_a > version_b, 0 if version_a == version_b, -1 if version_a < version_b.
-    """
-
-    def convert(version):
-        return tuple(map(int, version.split(".")))
-
-    version_a = convert(version_a)
-    version_b = convert(version_b)
-
-    if version_a > version_b:
-        return 1
-    elif version_a == version_b:
-        return 0
-    else:
-        return -1
+    try:
+        version_file.write_text(latest_version)
+    except PermissionError:
+        if find_and_chdir_package():
+            try:
+                os.makedirs(paths.get_cache_path(), exist_ok=True)
+                with open(paths.get_cache_path("sinol_make_version"), "w") as f:
+                    f.write(latest_version)
+            except PermissionError:
+                pass
 
 
 def lines_diff(lines1, lines2):
     """
     Function to compare two lists of lines.
     Returns True if they are the same, False otherwise.
     """
@@ -262,14 +296,16 @@
         return d
 
 
 def change_stack_size_to_unlimited():
     """
     Function to change the stack size to unlimited.
     """
+    if is_macos():
+        return
     try:
         resource.setrlimit(resource.RLIMIT_STACK, (resource.RLIM_INFINITY, resource.RLIM_INFINITY))
     except (resource.error, ValueError):
         # We can't run `ulimit -s unlimited` in the code, because since it failed, it probably requires root.
         print(error(f'Failed to change stack size to unlimited. Please run `ulimit -s unlimited` '
                     f'to make sure that solutions with large stack size will work.'))
 
@@ -284,54 +320,100 @@
 def is_linux():
     """
     Function to check if the program is running on Linux and not WSL.
     """
     return sys.platform == "linux" and not is_wsl()
 
 
+def is_macos():
+    """
+    Function to check if the program is running on macOS.
+    """
+    return sys.platform == "darwin"
+
+
+def is_macos_arm():
+    """
+    Function to check if the program is running on macOS on ARM.
+    """
+    return is_macos() and platform.machine().lower() == "arm64"
+
+
 def get_file_md5(path):
     with open(path, "rb") as f:
         return hashlib.md5(f.read()).hexdigest()
 
 
-def make_version_changes():
-    if compare_versions(sinol_make.__version__, "1.5.8") == 1:
-        # In version 1.5.9 we changed the format of sinol_expected_scores.
-        # Now all groups have specified points and status.
+def try_fix_config(config):
+    """
+    Function to try to fix the config.yml file.
+    Tries to:
+    - reformat `sinol_expected_scores` field
+    :param config: config.yml file as a dict
+    :return: config.yml file as a dict
+    """
+    # The old format was:
+    # sinol_expected_scores:
+    #   solution1:
+    #     expected: {1: OK, 2: OK, ...}
+    #     points: 100
+    #
+    # We change it to:
+    # sinol_expected_scores:
+    #   solution1:
+    #     expected: {1: {status: OK, points: 100}, 2: {status: OK, points: 100}, ...}
+    #     points: 100
+    try:
+        new_expected_scores = {}
+        expected_scores = config["sinol_expected_scores"]
+        contest = get_contest_type()
+        groups = []
+        for solution, results in expected_scores.items():
+            for group in results["expected"].keys():
+                if group not in groups:
+                    groups.append(int(group))
+
+        scores = contest.assign_scores(groups)
+        for solution, results in expected_scores.items():
+            new_expected_scores[solution] = {"expected": {}, "points": results["points"]}
+            for group, result in results["expected"].items():
+                if result in Status.possible_statuses():
+                    new_expected_scores[solution]["expected"][group] = {"status": result}
+                    if result == "OK":
+                        new_expected_scores[solution]["expected"][group]["points"] = scores[group]
+                    else:
+                        new_expected_scores[solution]["expected"][group]["points"] = 0
+                else:
+                    # This means that the result is probably valid.
+                    new_expected_scores[solution]["expected"][group] = result
+        config["sinol_expected_scores"] = new_expected_scores
+        save_config(config)
+    except:
+        # If there is an error, we just delete the field.
+        if "sinol_expected_scores" in config:
+            del config["sinol_expected_scores"]
+            save_config(config)
+    return config
+
+
+def extract_tar(tar: tarfile.TarFile, destination: str):
+    if sys.version_info.major == 3 and sys.version_info.minor >= 12:
+        tar.extractall(destination, filter='tar')
+    else:
+        tar.extractall(destination)
 
-        if find_and_chdir_package():
-            with open("config.yml", "r") as config_file:
-                config = yaml.load(config_file, Loader=yaml.FullLoader)
 
-            try:
-                new_expected_scores = {}
-                expected_scores = config["sinol_expected_scores"]
-                contest = get_contest_type()
-                groups = []
-                for solution, results in expected_scores.items():
-                    for group in results["expected"].keys():
-                        if group not in groups:
-                            groups.append(int(group))
-
-                scores = contest.assign_scores(groups)
-                for solution, results in expected_scores.items():
-                    new_expected_scores[solution] = {"expected": {}, "points": results["points"]}
-                    for group, result in results["expected"].items():
-                        new_expected_scores[solution]["expected"][group] = {"status": result}
-                        if result == "OK":
-                            new_expected_scores[solution]["expected"][group]["points"] = scores[group]
-                        else:
-                            new_expected_scores[solution]["expected"][group]["points"] = 0
-                config["sinol_expected_scores"] = new_expected_scores
-                save_config(config)
-            except:
-                # If there is an error, we just delete the field.
-                if "sinol_expected_scores" in config:
-                    del config["sinol_expected_scores"]
-                    save_config(config)
+def default_cpu_count():
+    """
+    Function to get default number of cpus to use for multiprocessing.
+    """
+    cpu_count = multiprocessing.cpu_count()
+    if cpu_count == 1:
+        return 1
+    return cpu_count - max(1, int(math.log2(cpu_count)) - 1)
 
 
 def color_red(text): return "\033[91m{}\033[00m".format(text)
 def color_green(text): return "\033[92m{}\033[00m".format(text)
 def color_yellow(text): return "\033[93m{}\033[00m".format(text)
 def color_gray(text): return "\033[90m{}\033[00m".format(text)
 def bold(text): return "\033[01m{}\033[00m".format(text)
@@ -347,7 +429,11 @@
 def exit_with_error(text, func=None):
     print(error(text))
     try:
         func()
     except TypeError:
         pass
     exit(1)
+
+
+def has_sanitizer_error(output, exit_code):
+    return ('ELF_ET_DYN_BASE' in output or 'ASan' in output) and exit_code != 0
```

### Comparing `sinol_make-1.5.9/src/sinol_make.egg-info/PKG-INFO` & `sinol_make-1.6.0.dev1/src/sinol_make.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 Metadata-Version: 2.1
-Name: sinol-make
-Version: 1.5.9
+Name: sinol_make
+Version: 1.6.0.dev1
 Summary: CLI tool for creating sio2 task packages
 Author: Mateusz Masiarz
 Author-email: m.masiarz@fri.edu.pl
 Maintainer: Tomasz Nowak, Mateusz Masiarz
 Maintainer-email: tomasz.nowak@tonowak.com, m.masiarz@fri.edu.pl
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: argcomplete
 Requires-Dist: requests
 Requires-Dist: PyYAML
 Requires-Dist: dictdiffer
 Requires-Dist: importlib-resources
 Requires-Dist: psutil
+Requires-Dist: packaging
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
 
-# <img src="https://avatars.githubusercontent.com/u/2264918?s=200&v=4" height=60em> sinol-make
+# ![Logo](https://avatars.githubusercontent.com/u/2264918?s=60&v=4) sinol-make
 
 `sinol-make` is a CLI tool for creating and verifying problem packages
 for [sio2](https://github.com/sio2project/oioioi)
 with features such as:
+
 - measuring time and memory in the same deterministic way as sio2,
 - running the solutions in parallel,
 - keeping a git-friendly report of solutions' scores,
 - catching mistakes in the problem packages as early as possible,
 - and more.
 
-# Contents
+## Contents
 
 - [Why?](#why)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Configuarion](#configuration)
 - [Reporting bugs and contributing code](#reporting-bugs-and-contributing-code)
 
 ### Why?
 
 The purpose of the tool is to make it easier to create good problem packages
 for official competitions, which requires collaboration with other people
 and using a multitude of "good practices" recommendations.
@@ -58,49 +60,68 @@
 solutions' runtime, called `oiejq`.
 
 ### Installation
 
 It's possible to directly install [sinol-make](https://pypi.org/project/sinol-make/)
 through Python's package manager pip, which usually is installed alongside Python:
 
-```
+```bash
 pip3 install sinol-make
 ```
 
+`pip` installs the `sinol-make` executable in `~/.local/bin/` directory,
+so make sure this directory is in your `PATH`.
+[Here's](https://gist.github.com/nex3/c395b2f8fd4b02068be37c961301caa7) how to add a directory to `PATH`.
+
 As `oiejq` works only on Linux-based operating systems,
 *we do not recommend* using operating systems such as Windows or macOS.
 Nevertheless `sinol-make` supports those operating systems,
 though there are additional installation steps required to use
 other tools for measuring time (which are non-deterministic and produce reports different from sio2):
+
 - Debian-based systems (Ubuntu, usually Windows WSL): `apt install time`
 - Arch-based systems: `pacman -S time`
 - macOS: `brew install gnu-time coreutils`
 
-### Autocompletion (optional)
+#### Autocompletion (optional)
 
 If you would like to have autocompletion for `sinol-make` commands,
 run the following command and refresh the shell (e.g. by opening a new terminal):
 
 ```shell
 activate-global-python-argcomplete
 ```
 
 ### Usage
 
 The availabe commands (see `sinol-make --help`) are:
 
 - `sinol-make run` -- Runs selected solutions (by default all solutions) on selected tests (by default all tests) with a given number
 of CPUs. Measures the solutions' time with oiejq, unless specified otherwise. After running the solutions, it
-compares the solutions' scores with the ones saved in config.yml.
+compares the solutions' scores with the ones saved in config.yml. If you're using oiejq, make sure you are not running on efficiency
+cpu cores. You can check if you have them [like this](https://stackoverflow.com/a/71282744). To run on normal cpu cores, use
+`taskset -c 8-15 sinol-make ...`, assuming that cpu cores 8-15 are not efficiency cores.
 Run `sinol-make run --help` to see available flags.
 - `sinol-make gen` -- Generate input files using ingen program (for example prog/abcingen.cpp for abc task). 
-Whenever the new input differs from the previous one, the model solution will be used to generate the new output file. 
-You can also specify your ingen source file which will be used. Run `sinol-make gen --help` to see available flags.
+Whenever the new input differs from the previous one, the model solution will be used to generate the new output file.
+You can also specify your ingen source file which will be used.
+Run `sinol-make gen --help` to see available flags.
+- `sinol-make ingen` -- Generate input files using ingen program (for example prog/abcingen.cpp for abc task).
+You can also specify your ingen source file which will be used.
+Run `sinol-make ingen --help` to see available flags.
+- `sinol-make outgen` -- Generate output files using the model solutions. Run `sinol-make outgen --help` to see available flags.
 - `sinol-make inwer` -- Verifies whether input files are correct using your "inwer.cpp" program. You can specify what inwer
 program to use, what tests to check and how many CPUs to use. Run `sinol-make inwer --help` to see available flags.
 - `sinol-make export` -- Creates archive ready to upload to sio2 or szkopul. Run `sinol-make export --help` to see all available flags.
 - `sinol-make doc` -- Compiles all LaTeX files in doc/ directory to PDF. Run `sinol-make doc --help` to see all available flags.
+- `sinol-make init [id]` -- Creates package from template [on github](https://github.com/sio2project/sinol-make/tree/main/example_package) and sets task id to provided `[id]`. Requires an internet connection to run.
+
+You can also run multiple commands at once, for example:
+
+```shell
+sinol-make gen prog/abcingen2.cpp inwer --cpus 4 run --tests abc1*.in doc export --no-statement
+```
 
 ### Reporting bugs and contributing code
 
 - Want to report a bug or request a feature? [Open an issue](https://github.com/sio2project/sinol-make/issues).
 - Want to help us build `sinol-make`? Create a Pull Request and we will gladly review it.
```

### Comparing `sinol_make-1.5.9/src/sinol_make.egg-info/SOURCES.txt` & `sinol_make-1.6.0.dev1/src/sinol_make.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,23 @@
 src/sinol_make.egg-info/dependency_links.txt
 src/sinol_make.egg-info/entry_points.txt
 src/sinol_make.egg-info/requires.txt
 src/sinol_make.egg-info/top_level.txt
 src/sinol_make/commands/doc/__init__.py
 src/sinol_make/commands/export/__init__.py
 src/sinol_make/commands/gen/__init__.py
-src/sinol_make/commands/gen/gen_util.py
+src/sinol_make/commands/ingen/__init__.py
+src/sinol_make/commands/ingen/ingen_util.py
+src/sinol_make/commands/init/__init__.py
 src/sinol_make/commands/inwer/__init__.py
 src/sinol_make/commands/inwer/inwer_util.py
+src/sinol_make/commands/outgen/__init__.py
+src/sinol_make/commands/outgen/outgen_util.py
 src/sinol_make/commands/run/__init__.py
+src/sinol_make/commands/verify/__init__.py
 src/sinol_make/contest_types/__init__.py
 src/sinol_make/contest_types/default.py
 src/sinol_make/contest_types/icpc.py
 src/sinol_make/contest_types/oi.py
 src/sinol_make/helpers/__init__.py
 src/sinol_make/helpers/cache.py
 src/sinol_make/helpers/compile.py
@@ -37,9 +42,10 @@
 src/sinol_make/structs/__init__.py
 src/sinol_make/structs/cache_structs.py
 src/sinol_make/structs/compiler_structs.py
 src/sinol_make/structs/gen_structs.py
 src/sinol_make/structs/inwer_structs.py
 src/sinol_make/structs/run_structs.py
 src/sinol_make/structs/status_structs.py
+tests/test_multiple_arguments.py
 tests/test_oiejq.py
 tests/test_util.py
```

### Comparing `sinol_make-1.5.9/tests/test_oiejq.py` & `sinol_make-1.6.0.dev1/tests/test_oiejq.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,32 +7,50 @@
 
 
 @pytest.mark.github_runner
 def test_install_oiejq():
     if sys.platform != 'linux':
         return
 
-    shutil.rmtree(os.path.expanduser('~/.local/bin/'), ignore_errors=True)
+    try:
+        os.remove(os.path.expanduser('~/.local/bin/oiejq'))
+        os.remove(os.path.expanduser('~/.local/bin/sio2jail'))
+    except IsADirectoryError:
+        shutil.rmtree(os.path.expanduser('~/.local/bin/oiejq'), ignore_errors=True)    
+    except FileNotFoundError:
+        pass
     assert not oiejq.check_oiejq()
     assert oiejq.install_oiejq()
     assert oiejq.get_oiejq_path() == os.path.expanduser('~/.local/bin/oiejq')
 
-    shutil.rmtree(os.path.expanduser('~/.local/bin/'), ignore_errors=True)
+    try:
+        os.remove(os.path.expanduser('~/.local/bin/oiejq'))
+        os.remove(os.path.expanduser('~/.local/bin/sio2jail'))
+    except FileNotFoundError:
+        pass
+    
     assert not oiejq.check_oiejq()
     os.makedirs(os.path.expanduser('~/.local/bin/oiejq'))
     with pytest.raises(SystemExit):
         oiejq.install_oiejq()
 
 
 @pytest.mark.github_runner
 def test_check_oiejq():
     if sys.platform != 'linux':
         return
 
-    shutil.rmtree(os.path.expanduser('~/.local/bin/'), ignore_errors=True)
+    try:
+        os.remove(os.path.expanduser('~/.local/bin/oiejq'))
+        os.remove(os.path.expanduser('~/.local/bin/sio2jail'))
+    except IsADirectoryError:
+        shutil.rmtree(os.path.expanduser('~/.local/bin/oiejq'), ignore_errors=True)    
+    except FileNotFoundError:
+        pass
+
     assert not oiejq.check_oiejq()
     os.makedirs(os.path.expanduser('~/.local/bin/oiejq'), exist_ok=True)
     assert not oiejq.check_oiejq()
     os.rmdir(os.path.expanduser('~/.local/bin/oiejq'))
     with open(os.path.expanduser('~/.local/bin/oiejq'), 'w') as f:
         f.write('abcdef')
     assert not oiejq.check_oiejq()
```

