# Comparing `tmp/FlipperNested-2.3.2.tar.gz` & `tmp/FlipperNested-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-2.3.2.tar", last modified: Thu Oct  5 08:52:33 2023, max compression
+gzip compressed data, was "FlipperNested-2.3.4.tar", last modified: Thu Apr  4 13:24:46 2024, max compression
```

## Comparing `FlipperNested-2.3.2.tar` & `FlipperNested-2.3.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.975574 FlipperNested-2.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.951574 FlipperNested-2.3.2/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14135 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.955574 FlipperNested-2.3.2/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.955574 FlipperNested-2.3.2/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-10-05 08:52:33.000000 FlipperNested-2.3.2/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2023-10-05 08:52:33.000000 FlipperNested-2.3.2/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 08:52:33.000000 FlipperNested-2.3.2/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-05 08:52:33.000000 FlipperNested-2.3.2/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-05 08:52:33.000000 FlipperNested-2.3.2/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-05 08:52:33.000000 FlipperNested-2.3.2/FlipperNested.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.959574 FlipperNested-2.3.2/HardNestedSolver/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2504 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/bucketsort.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/bucketsort.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    85428 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/cmdhfmfhard.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/cmdhfmfhard.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    18805 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/crapto1.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2951 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/crapto1.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     6561 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/crypto1.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.967574 FlipperNested-2.3.2/HardNestedSolver/hardnested/
--rwxr-xr-x   0 runner    (1001) docker     (127)   494104 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_benchmark_data.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    33334 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bf_core.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     4073 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bf_core.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    31568 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bitarray_core.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     3347 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bitarray_core.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    19427 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bruteforce.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2249 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bruteforce.h
--rwxr-xr-x   0 runner    (1001) docker     (127)  5060431 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/tables.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      941 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/hardnested/tables.h
--rwxr-xr-x   0 runner    (1001) docker     (127)      432 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/library.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      159 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/library.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     3340 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/parity.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.971574 FlipperNested-2.3.2/HardNestedSolver/pm3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/ansi.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     3405 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/common.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/commonutil.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1591 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/commonutil.h
--rwxr-xr-x   0 runner    (1001) docker     (127)   110555 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/emojis.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/emojis_alt.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    13770 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/ui.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/ui.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     1534 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/util.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1236 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/util.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     4044 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/util_posix.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/pm3/util_posix.h
--rwxr-xr-x   0 runner    (1001) docker     (127)      773 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/HardNestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.971574 FlipperNested-2.3.2/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-10-05 08:52:33.975574 FlipperNested-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 08:52:33.975574 FlipperNested-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:52:33.975574 FlipperNested-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-10-05 08:52:21.000000 FlipperNested-2.3.2/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.087797 FlipperNested-2.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.067797 FlipperNested-2.3.4/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.071797 FlipperNested-2.3.4/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.087797 FlipperNested-2.3.4/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 13:24:46.000000 FlipperNested-2.3.4/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-04 13:24:46.000000 FlipperNested-2.3.4/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:24:46.000000 FlipperNested-2.3.4/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 13:24:46.000000 FlipperNested-2.3.4/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 13:24:46.000000 FlipperNested-2.3.4/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 13:24:46.000000 FlipperNested-2.3.4/FlipperNested.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.071797 FlipperNested-2.3.4/HardNestedSolver/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2504 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/bucketsort.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/bucketsort.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    85428 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/cmdhfmfhard.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/cmdhfmfhard.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18805 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/crapto1.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2951 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/crapto1.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6561 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/crypto1.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.079798 FlipperNested-2.3.4/HardNestedSolver/hardnested/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   494104 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_benchmark_data.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33334 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bf_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4073 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bf_core.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31568 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bitarray_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3347 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bitarray_core.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19427 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bruteforce.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2249 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bruteforce.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)  5060431 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/tables.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      941 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/hardnested/tables.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/library.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/library.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3340 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/parity.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.083798 FlipperNested-2.3.4/HardNestedSolver/pm3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/ansi.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3405 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/common.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/commonutil.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1591 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/commonutil.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   110555 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/emojis.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/emojis_alt.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13770 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/ui.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/ui.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1534 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/util.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1236 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/util.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4044 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/util_posix.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/pm3/util_posix.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)      773 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/HardNestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.083798 FlipperNested-2.3.4/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 13:24:46.087797 FlipperNested-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:24:46.087797 FlipperNested-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:24:46.087797 FlipperNested-2.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-04 13:24:40.000000 FlipperNested-2.3.4/tests/test_parse.py
```

### Comparing `FlipperNested-2.3.2/FlipperNested/bridge.py` & `FlipperNested-2.3.4/FlipperNested/bridge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import serial
 import serial.tools.list_ports
 from google.protobuf.internal.encoder import _VarintBytes
 from google.protobuf.json_format import MessageToDict
 
 import FlipperNested.proto.flipper_pb2 as flipper_pb2
 import FlipperNested.proto.storage_pb2 as storage_pb2
@@ -118,24 +119,29 @@
     def get_files(self, path="/ext") -> list:
         storage_response = []
         cmd_data = storage_pb2.ListRequest()
 
         cmd_data.path = path
         rep_data = self._rpc_send_and_read_answer(cmd_data, "storage_list_request")
 
-        storage_response.extend(
-            MessageToDict(message=rep_data.storage_list_response, including_default_value_fields=True, )["file"])
+        storage_response.extend(self._message_to_dict(rep_data.storage_list_response)["file"])
 
         while rep_data.has_next:
             rep_data = self._rpc_read_answer()
-            storage_response.extend(
-                MessageToDict(message=rep_data.storage_list_response, including_default_value_fields=True, )["file"])
+            storage_response.extend(self._message_to_dict(rep_data.storage_list_response)["file"])
 
         return storage_response
 
+    @staticmethod
+    def _message_to_dict(message):
+        if 'including_default_value_fields' in inspect.signature(MessageToDict).parameters:
+            return MessageToDict(message=message, including_default_value_fields=True)
+        else:
+            return MessageToDict(message=message, always_print_fields_with_no_presence=True)
+
     def file_read(self, path=None):
         storage_response = []
         cmd_data = storage_pb2.ReadRequest()
         cmd_data.path = path
 
         rep_data = self._rpc_send_and_read_answer(cmd_data, "storage_read_request")
 
@@ -178,15 +184,15 @@
 
         self._rpc_send_and_read_answer(cmd_data, "storage_delete_request")
 
     def mkdir(self, path="/ext"):
         cmd_data = storage_pb2.MkdirRequest()
         cmd_data.path = path
 
-        rep_data = self._rpc_send_and_read_answer(cmd_data, "storage_mkdir_request")
+        self._rpc_send_and_read_answer(cmd_data, "storage_mkdir_request")
 
     def file_rename(self, old, new):
         cmd_data = storage_pb2.RenameRequest()
         cmd_data.old_path = old
         cmd_data.new_path = new
 
         self._rpc_send_and_read_answer(cmd_data, "storage_rename_request")
```

### Comparing `FlipperNested-2.3.2/FlipperNested/cli.py` & `FlipperNested-2.3.4/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/FlipperNested/main.py` & `FlipperNested-2.3.4/FlipperNested/main.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-2.3.4/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/FlipperNested/proto/storage_pb2.py` & `FlipperNested-2.3.4/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-2.3.4/FlipperNested.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 2.3.2
+Version: 2.3.4
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-2.3.2/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-2.3.4/FlipperNested.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/bucketsort.c` & `FlipperNested-2.3.4/HardNestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/bucketsort.h` & `FlipperNested-2.3.4/HardNestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/cmdhfmfhard.c` & `FlipperNested-2.3.4/HardNestedSolver/cmdhfmfhard.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/cmdhfmfhard.h` & `FlipperNested-2.3.4/HardNestedSolver/cmdhfmfhard.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/crapto1.c` & `FlipperNested-2.3.4/HardNestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/crapto1.h` & `FlipperNested-2.3.4/HardNestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/crypto1.c` & `FlipperNested-2.3.4/HardNestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_benchmark_data.h` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_benchmark_data.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bf_core.c` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bf_core.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bf_core.h` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bf_core.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bitarray_core.c` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bitarray_core.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bitarray_core.h` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bitarray_core.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bruteforce.c` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bruteforce.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/hardnested_bruteforce.h` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/hardnested_bruteforce.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/tables.c` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/tables.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/hardnested/tables.h` & `FlipperNested-2.3.4/HardNestedSolver/hardnested/tables.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/parity.h` & `FlipperNested-2.3.4/HardNestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/ansi.h` & `FlipperNested-2.3.4/HardNestedSolver/pm3/ansi.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/common.h` & `FlipperNested-2.3.4/HardNestedSolver/pm3/common.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/commonutil.c` & `FlipperNested-2.3.4/HardNestedSolver/pm3/commonutil.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/commonutil.h` & `FlipperNested-2.3.4/HardNestedSolver/pm3/commonutil.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/emojis.h` & `FlipperNested-2.3.4/HardNestedSolver/pm3/emojis.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/emojis_alt.h` & `FlipperNested-2.3.4/HardNestedSolver/pm3/emojis_alt.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/ui.c` & `FlipperNested-2.3.4/HardNestedSolver/pm3/ui.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/ui.h` & `FlipperNested-2.3.4/HardNestedSolver/pm3/ui.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/util.c` & `FlipperNested-2.3.4/HardNestedSolver/pm3/util.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/util.h` & `FlipperNested-2.3.4/HardNestedSolver/pm3/util.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/util_posix.c` & `FlipperNested-2.3.4/HardNestedSolver/pm3/util_posix.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/pm3/util_posix.h` & `FlipperNested-2.3.4/HardNestedSolver/pm3/util_posix.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/HardNestedSolver/python.c` & `FlipperNested-2.3.4/HardNestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/LICENSE.md` & `FlipperNested-2.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/bucketsort.c` & `FlipperNested-2.3.4/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/bucketsort.h` & `FlipperNested-2.3.4/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/crapto1.c` & `FlipperNested-2.3.4/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/crapto1.h` & `FlipperNested-2.3.4/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/crypto1.c` & `FlipperNested-2.3.4/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/library.c` & `FlipperNested-2.3.4/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/library.h` & `FlipperNested-2.3.4/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/parity.h` & `FlipperNested-2.3.4/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/progress.c` & `FlipperNested-2.3.4/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/NestedSolver/python.c` & `FlipperNested-2.3.4/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/PKG-INFO` & `FlipperNested-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 2.3.2
+Version: 2.3.4
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-2.3.2/README.md` & `FlipperNested-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.3.2/setup.py` & `FlipperNested-2.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                                                      "HardNestedSolver/pm3/util_posix.c",
                                                      "HardNestedSolver/python.c"], include_dirs=include_dirs,
                               library_dirs=include_dirs, extra_compile_args=extra_compile_args, libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-setuptools.setup(name="FlipperNested", version="2.3.2", author="AloneLiberty",
+setuptools.setup(name="FlipperNested", version="2.3.4", author="AloneLiberty",
                  description="Recover keys from collected nonces", long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AloneLiberty/FlipperNestedRecovery",
                  entry_points={"console_scripts": ["FlipperNested = FlipperNested.cli:main"]},
                  install_requires=["protobuf>4", "pyserial"], ext_modules=[nested_solver, hardnested_solver],
                  packages=["FlipperNested", "FlipperNested.proto"], python_requires=">=3.8",
                  classifiers=["Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9",
```

### Comparing `FlipperNested-2.3.2/tests/test_calculate.py` & `FlipperNested-2.3.4/tests/test_calculate.py`

 * *Files identical despite different names*

