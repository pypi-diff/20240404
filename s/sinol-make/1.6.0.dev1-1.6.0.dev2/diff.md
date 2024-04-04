# Comparing `tmp/sinol_make-1.6.0.dev1.tar.gz` & `tmp/sinol_make-1.6.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol_make-1.6.0.dev1.tar", last modified: Thu Apr  4 20:42:56 2024, max compression
+gzip compressed data, was "sinol_make-1.6.0.dev2.tar", last modified: Thu Apr  4 21:08:04 2024, max compression
```

## Comparing `sinol_make-1.6.0.dev1.tar` & `sinol_make-1.6.0.dev2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.149683 sinol_make-1.6.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.149683 sinol_make-1.6.0.dev1/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/export/
--rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/gen/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/ingen/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/ingen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/ingen/ingen_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.153683 sinol_make-1.6.0.dev1/src/sinol_make/commands/init/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/inwer_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/outgen_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (127)    57981 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/commands/verify/
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/commands/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/icpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/contest_types/oi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/package_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/helpers/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.157683 sinol_make-1.6.0.dev1/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/src/sinol_make/oiejq/
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/oiejq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/oiejq/perf_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/src/sinol_make/structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/cache_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/compiler_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/gen_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/inwer_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/run_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/structs/status_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 20:42:56.000000 sinol_make-1.6.0.dev1/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:42:56.161683 sinol_make-1.6.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/tests/test_multiple_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/tests/test_oiejq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-04 20:42:51.000000 sinol_make-1.6.0.dev1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.564036 sinol_make-1.6.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.564036 sinol_make-1.6.0.dev2/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/export/
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/ingen_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/inwer_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.568036 sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/outgen_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (127)    57981 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/commands/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/commands/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/icpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/contest_types/oi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/helpers/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/oiejq/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/oiejq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/oiejq/perf_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.572036 sinol_make-1.6.0.dev2/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/cache_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/gen_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/inwer_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/run_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/structs/status_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 21:08:04.000000 sinol_make-1.6.0.dev2/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:08:04.576036 sinol_make-1.6.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/tests/test_multiple_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/tests/test_oiejq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-04 21:08:00.000000 sinol_make-1.6.0.dev2/tests/test_util.py
```

### Comparing `sinol_make-1.6.0.dev1/LICENSE` & `sinol_make-1.6.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/PKG-INFO` & `sinol_make-1.6.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol_make
-Version: 1.6.0.dev1
+Version: 1.6.0.dev2
 Summary: CLI tool for creating sio2 task packages
 Author: Mateusz Masiarz
 Author-email: m.masiarz@fri.edu.pl
 Maintainer: Tomasz Nowak, Mateusz Masiarz
 Maintainer-email: tomasz.nowak@tonowak.com, m.masiarz@fri.edu.pl
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
```

### Comparing `sinol_make-1.6.0.dev1/README.md` & `sinol_make-1.6.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/setup.cfg` & `sinol_make-1.6.0.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import argparse
 import traceback
 import argcomplete
 
 from sinol_make import util, oiejq
 
-__version__ = "1.6.0.dev1"
+__version__ = "1.6.0.dev2"
 
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
```

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/doc/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/export/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/export/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,32 +94,46 @@
         return [package_util.extract_test_id(test, self.task_id) for test in tests]
 
     def create_ocen(self, target_dir: str):
         """
         Creates ocen archive for sio2.
         :param target_dir: Path to exported package.
         """
+        print('Generating ocen archive...')
         attachments_dir = os.path.join(target_dir, 'attachments')
         if not os.path.exists(attachments_dir):
             os.makedirs(attachments_dir)
         tests_dir = paths.get_cache_path('export', 'tests')
 
         with tempfile.TemporaryDirectory() as tmpdir:
             ocen_dir = os.path.join(tmpdir, self.task_id)
             os.makedirs(ocen_dir)
             in_dir = os.path.join(ocen_dir, 'in')
             os.makedirs(in_dir)
             out_dir = os.path.join(ocen_dir, 'out')
             os.makedirs(out_dir)
+            num_tests = 0
             for ext in ['in', 'out']:
                 for test in glob.glob(os.path.join(tests_dir, ext, f'{self.task_id}0*.{ext}')) + \
                             glob.glob(os.path.join(tests_dir, ext, f'{self.task_id}*ocen.{ext}')):
                     shutil.copy(test, os.path.join(ocen_dir, ext, os.path.basename(test)))
+                    num_tests += 1
 
-            shutil.make_archive(os.path.join(attachments_dir, f'{self.task_id}ocen'), 'zip', tmpdir)
+            if num_tests == 0:
+                print(util.warning('No ocen tests found.'))
+            else:
+                shutil.make_archive(os.path.join(attachments_dir, f'{self.task_id}ocen'), 'zip', tmpdir)
+
+            dlazaw_dir = os.path.join(os.getcwd(), 'dlazaw')
+            if os.path.exists(dlazaw_dir):
+                print('Archiving dlazaw directory and adding to attachments.')
+                os.makedirs(os.path.join(tmpdir, 'dlazaw'), exist_ok=True)
+                shutil.copytree(dlazaw_dir, os.path.join(tmpdir, 'dlazaw', 'dlazaw'))
+                shutil.make_archive(os.path.join(attachments_dir, 'dlazaw'), 'zip',
+                                    os.path.join(tmpdir, 'dlazaw'))
 
     def compile_statement(self):
         command = DocCommand()
         doc_args = argparse.Namespace()
         doc_args.files = [f'./doc/{self.task_id}zad.tex']
         command.run(doc_args)
         if not os.path.isfile(f'./doc/{self.task_id}zad.pdf') and not self.args.no_statement:
@@ -165,15 +179,14 @@
             for test in tests_to_copy:
                 print(util.warning(f'Copying {os.path.basename(test[1])}...'))
                 shutil.copy(test[1], os.path.join(target_dir, test[0], os.path.basename(test[1])))
                 shutil.copy(test[1], os.path.join(cache_test_dir, test[0], os.path.basename(test[1])))
 
         self.generate_output_files()
         if self.args.export_ocen:
-            print('Generating ocen archive...')
             self.create_ocen(target_dir)
 
     def clear_files(self, target_dir: str):
         """
         Clears unnecessary files from target directory.
         :param target_dir: Directory to clear files from.
         """
```

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/gen/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/ingen/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/ingen/ingen_util.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/ingen/ingen_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/init/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/init/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/inwer/inwer_util.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/inwer/inwer_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/outgen/outgen_util.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/outgen/outgen_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/run/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/commands/verify/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/commands/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/contest_types/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/contest_types/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/contest_types/default.py` & `sinol_make-1.6.0.dev2/src/sinol_make/contest_types/default.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/contest_types/icpc.py` & `sinol_make-1.6.0.dev2/src/sinol_make/contest_types/icpc.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/contest_types/oi.py` & `sinol_make-1.6.0.dev2/src/sinol_make/contest_types/oi.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/helpers/cache.py` & `sinol_make-1.6.0.dev2/src/sinol_make/helpers/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,45 +31,44 @@
         return CacheFile()
     except (yaml.YAMLError, TypeError):
         print(util.warning(f"Cache file for program {os.path.basename(solution_path)} is corrupted."))
         os.unlink(cache_file_path)
         return CacheFile()
 
 
-def check_compiled(file_path: str) -> Union[str, None]:
+def check_compiled(file_path: str, compilation_flags: str, sanitizers: bool) -> Union[str, None]:
     """
     Check if a file is compiled
     :param file_path: Path to the file
     :return: executable path if compiled, None otherwise
     """
     md5sum = util.get_file_md5(file_path)
     try:
         info = get_cache_file(file_path)
-        if info.md5sum == md5sum:
+        if info.md5sum == md5sum and info.compilation_flags == compilation_flags and info.sanitizers == sanitizers:
             exe_path = info.executable_path
             if os.path.exists(exe_path):
                 return exe_path
         return None
     except FileNotFoundError:
         return None
 
 
-def save_compiled(file_path: str, exe_path: str, is_checker: bool = False):
+def save_compiled(file_path: str, exe_path: str, compilation_flags: str, sanitizers: bool, is_checker: bool = False):
     """
     Save the compiled executable path to cache in `.cache/md5sums/<basename of file_path>`,
     which contains the md5sum of the file and the path to the executable.
     :param file_path: Path to the file
     :param exe_path: Path to the compiled executable
+    :param compilation_flags: Compilation flags used
+    :param sanitizers: Whether -fsanitize=undefined,address was used
     :param is_checker: Whether the compiled file is a checker. If True, all cached tests are removed.
     """
-    info = CacheFile()
-    info.executable_path = exe_path
-    info.md5sum = util.get_file_md5(file_path)
+    info = CacheFile(util.get_file_md5(file_path), exe_path, compilation_flags, sanitizers)
     info.save(file_path)
-
     if is_checker:
         remove_results_cache()
 
 
 def _check_file_changed(file_path, lang, task_id):
     solutions_re = package_util.get_solutions_re(task_id)
     md5sum = util.get_file_md5(file_path)
```

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/helpers/compile.py` & `sinol_make-1.6.0.dev2/src/sinol_make/helpers/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,36 +33,42 @@
         extra_compilation_args = [extra_compilation_args]
     assert isinstance(extra_compilation_args, list) and all(isinstance(arg, str) for arg in extra_compilation_args)
 
     # Address and undefined sanitizer is not yet supported on Apple Silicon.
     if use_fsanitize and util.is_macos_arm():
         use_fsanitize = False
 
+    if compilation_flags == 'w':
+        compilation_flags = 'weak'
+    elif compilation_flags == 'o':
+        compilation_flags = 'oioioi'
+    elif compilation_flags == 'd':
+        compilation_flags = 'default'
+
     if extra_compilation_files is None:
         extra_compilation_files = []
 
-    compiled_exe = check_compiled(program)
+    compiled_exe = check_compiled(program, compilation_flags, use_fsanitize)
     if compiled_exe is not None:
         if compile_log is not None:
             compile_log.write(f'Using cached executable {compiled_exe}\n')
             compile_log.close()
         if os.path.abspath(compiled_exe) != os.path.abspath(output):
             shutil.copy(compiled_exe, output)
         return True
 
     for file in extra_compilation_files:
         shutil.copy(file, os.path.join(os.path.dirname(output), os.path.basename(file)))
 
     gcc_compilation_flags = ''
-    if compilation_flags == 'weak' or compilation_flags == 'w':
-        compilation_flags = 'weak'
+    if compilation_flags == 'weak':
         gcc_compilation_flags = ''  # Disable all warnings
-    elif compilation_flags == 'oioioi' or compilation_flags == 'o':
+    elif compilation_flags == 'oioioi':
         gcc_compilation_flags = ' -Wall -Wno-unused-result -Werror'  # Same flags as oioioi
-    elif compilation_flags == 'default' or compilation_flags == 'd':
+    elif compilation_flags == 'default':
         gcc_compilation_flags = ' -Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'
     else:
         util.exit_with_error(f'Unknown compilation flags group: {compilation_flags}')
 
     if compilers is None:
         compilers = Compilers()
 
@@ -104,15 +110,15 @@
         compile_log.close()
     else:
         print(out.decode('utf-8'))
 
     if process.returncode != 0:
         raise CompilationError('Compilation failed')
     else:
-        save_compiled(program, output, is_checker)
+        save_compiled(program, output, compilation_flags, use_fsanitize, is_checker)
         return True
 
 
 def compile_file(file_path: str, name: str, compilers: Compilers, compilation_flags='default',
                  use_fsanitize=False, additional_flags=None) \
         -> Tuple[Union[str, None], str]:
     """
```

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/helpers/compiler.py` & `sinol_make-1.6.0.dev2/src/sinol_make/helpers/compiler.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/helpers/package_util.py` & `sinol_make-1.6.0.dev2/src/sinol_make/helpers/package_util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/helpers/parsers.py` & `sinol_make-1.6.0.dev2/src/sinol_make/helpers/parsers.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/helpers/paths.py` & `sinol_make-1.6.0.dev2/src/sinol_make/helpers/paths.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/helpers/printer.py` & `sinol_make-1.6.0.dev2/src/sinol_make/helpers/printer.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/oiejq/__init__.py` & `sinol_make-1.6.0.dev2/src/sinol_make/oiejq/__init__.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/structs/compiler_structs.py` & `sinol_make-1.6.0.dev2/src/sinol_make/structs/compiler_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/structs/inwer_structs.py` & `sinol_make-1.6.0.dev2/src/sinol_make/structs/inwer_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/structs/run_structs.py` & `sinol_make-1.6.0.dev2/src/sinol_make/structs/run_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/structs/status_structs.py` & `sinol_make-1.6.0.dev2/src/sinol_make/structs/status_structs.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make/util.py` & `sinol_make-1.6.0.dev2/src/sinol_make/util.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make.egg-info/PKG-INFO` & `sinol_make-1.6.0.dev2/src/sinol_make.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol_make
-Version: 1.6.0.dev1
+Version: 1.6.0.dev2
 Summary: CLI tool for creating sio2 task packages
 Author: Mateusz Masiarz
 Author-email: m.masiarz@fri.edu.pl
 Maintainer: Tomasz Nowak, Mateusz Masiarz
 Maintainer-email: tomasz.nowak@tonowak.com, m.masiarz@fri.edu.pl
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
```

### Comparing `sinol_make-1.6.0.dev1/src/sinol_make.egg-info/SOURCES.txt` & `sinol_make-1.6.0.dev2/src/sinol_make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/tests/test_multiple_arguments.py` & `sinol_make-1.6.0.dev2/tests/test_multiple_arguments.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/tests/test_oiejq.py` & `sinol_make-1.6.0.dev2/tests/test_oiejq.py`

 * *Files identical despite different names*

### Comparing `sinol_make-1.6.0.dev1/tests/test_util.py` & `sinol_make-1.6.0.dev2/tests/test_util.py`

 * *Files identical despite different names*

