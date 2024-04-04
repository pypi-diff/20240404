# Comparing `tmp/gink-0.20240404.1712197692.tar.gz` & `tmp/gink-0.20240404.1712204855.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240404.1712197692.tar", last modified: Thu Apr  4 02:28:20 2024, max compression
+gzip compressed data, was "gink-0.20240404.1712204855.tar", last modified: Thu Apr  4 04:27:38 2024, max compression
```

## Comparing `gink-0.20240404.1712197692.tar` & `gink-0.20240404.1712204855.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:20.261213 gink-0.20240404.1712197692/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-04 02:28:20.261213 gink-0.20240404.1712197692/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:20.249213 gink-0.20240404.1712197692/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:20.249213 gink-0.20240404.1712197692/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:20.257213 gink-0.20240404.1712197692/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17862 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    53266 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/impl/websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:20.261213 gink-0.20240404.1712197692/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10202 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-04 02:28:05.000000 gink-0.20240404.1712197692/gink/tests/test_websocket_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:28:20.261213 gink-0.20240404.1712197692/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-04 02:28:20.000000 gink-0.20240404.1712197692/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-04 02:28:20.000000 gink-0.20240404.1712197692/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 02:28:20.000000 gink-0.20240404.1712197692/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 02:28:20.000000 gink-0.20240404.1712197692/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 02:28:20.000000 gink-0.20240404.1712197692/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 02:28:20.261213 gink-0.20240404.1712197692/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-04 02:28:12.000000 gink-0.20240404.1712197692/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.538324 gink-0.20240404.1712204855/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.538324 gink-0.20240404.1712204855/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.546325 gink-0.20240404.1712204855/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20537 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17862 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11803 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53281 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/impl/websocket_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10202 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-04 04:27:31.000000 gink-0.20240404.1712204855/gink/tests/test_websocket_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 04:27:38.000000 gink-0.20240404.1712204855/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:27:38.550325 gink-0.20240404.1712204855/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-04 04:27:35.000000 gink-0.20240404.1712204855/setup.py
```

### Comparing `gink-0.20240404.1712197692/LICENSE` & `gink-0.20240404.1712204855/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/PKG-INFO` & `gink-0.20240404.1712204855/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240404.1712197692
+Version: 0.20240404.1712204855
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240404.1712197692/README.md` & `gink-0.20240404.1712204855/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/__init__.py` & `gink-0.20240404.1712204855/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/__main__.py` & `gink-0.20240404.1712204855/gink/__main__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/behavior_pb2.py` & `gink-0.20240404.1712204855/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/bundle_pb2.py` & `gink-0.20240404.1712204855/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/change_pb2.py` & `gink-0.20240404.1712204855/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/claim_pb2.py` & `gink-0.20240404.1712204855/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/clearance_pb2.py` & `gink-0.20240404.1712204855/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/container_pb2.py` & `gink-0.20240404.1712204855/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/entry_pb2.py` & `gink-0.20240404.1712204855/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/key_pb2.py` & `gink-0.20240404.1712204855/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/log_file_pb2.py` & `gink-0.20240404.1712204855/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/movement_pb2.py` & `gink-0.20240404.1712204855/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/muid_pb2.py` & `gink-0.20240404.1712204855/gink/builders/muid_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='proto/muid.proto',
   package='gink',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x10proto/muid.proto\x12\x04gink\"<\n\x04Muid\x12\x11\n\ttimestamp\x18\x01 \x01(\x12\x12\x11\n\tmedallion\x18\x02 \x01(\x12\x12\x0e\n\x06offset\x18\x03 \x01(\rb\x06proto3'
+  serialized_pb=b'\n\x10proto/muid.proto\x12\x04gink\"<\n\x04Muid\x12\x11\n\ttimestamp\x18\x01 \x01(\x12\x12\x11\n\tmedallion\x18\x02 \x01(\x12\x12\x0e\n\x06offset\x18\x03 \x01(\x11\x62\x06proto3'
 )
 
 
 
 
 _MUID = _descriptor.Descriptor(
   name='Muid',
@@ -45,15 +45,15 @@
       number=2, type=18, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='offset', full_name='gink.Muid.offset', index=2,
-      number=3, type=13, cpp_type=3, label=1,
+      number=3, type=17, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
```

### Comparing `gink-0.20240404.1712197692/gink/builders/pair_pb2.py` & `gink-0.20240404.1712204855/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/sync_message_pb2.py` & `gink-0.20240404.1712204855/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/builders/value_pb2.py` & `gink-0.20240404.1712204855/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/abstract_store.py` & `gink-0.20240404.1712204855/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/addressable.py` & `gink-0.20240404.1712204855/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/attribution.py` & `gink-0.20240404.1712204855/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/box.py` & `gink-0.20240404.1712204855/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/builders.py` & `gink-0.20240404.1712204855/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/bundle_info.py` & `gink-0.20240404.1712204855/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/bundle_wrapper.py` & `gink-0.20240404.1712204855/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/bundler.py` & `gink-0.20240404.1712204855/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/chain_tracker.py` & `gink-0.20240404.1712204855/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/coding.py` & `gink-0.20240404.1712204855/gink/impl/coding.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,21 @@
 INT_INF = 0xffffffffffffffff
 ZERO_64: bytes = b"\x00" * 8
 KEY_MAX: int = 2**53 - 1
 deletion = Deletion()
 inclusion = Inclusion()
 
 
-def ensure_entry_is_valid(builder: EntryBuilder, context: Any = object()):
+def ensure_entry_is_valid(builder: EntryBuilder, context: Any = object(), offset: Optional[int]=None):
     if getattr(builder, "behavior") == UNSPECIFIED:
         raise ValueError("entry lacks a behavior")
     if not builder.HasField("container"):
         raise ValueError("no container specified in entry")
-    container_muid = Muid.create(context, builder=getattr(builder, "container"))
+    entry_muid = Muid.create(context, offset=offset)
+    container_muid = Muid.create(context=entry_muid, builder=getattr(builder, "container"))
     if container_muid.timestamp == -1 and container_muid.medallion > 0:
         if getattr(context, "medallion") != container_muid.medallion:
             raise ValueError("attempt to modify instance container from other instance")
 
 
 def serialize(thing) -> bytes:
     """ Converts a protobuf builder or a timestamp into binary data. """
@@ -124,16 +125,16 @@
         assert not isinstance(self.middle, QueueMiddleKey)
         return self.middle
 
 
     @staticmethod
     def from_builder(builder: EntryBuilder, new_info: BundleInfo, offset: int):
         """ Create an EntryStorageKey from an Entry itself, plus address information. """
-        container = Muid.create(builder=getattr(builder, "container"), context=new_info)
         entry_muid = Muid.create(context=new_info, offset=offset)
+        container = Muid.create(builder=getattr(builder, "container"), context=entry_muid)
         behavior = getattr(builder, "behavior")
         position = getattr(builder, "effective")
         middle_key: Union[QueueMiddleKey, Muid, UserKey, None, Tuple[Muid, Muid]]
         if behavior in [DIRECTORY, KEY_SET]:
             middle_key = decode_key(builder)
         elif behavior in (BOX, VERTEX):
             middle_key = None
```

### Comparing `gink-0.20240404.1712197692/gink/impl/connection.py` & `gink-0.20240404.1712204855/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/container.py` & `gink-0.20240404.1712204855/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/database.py` & `gink-0.20240404.1712204855/gink/impl/database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/deferred.py` & `gink-0.20240404.1712204855/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/directory.py` & `gink-0.20240404.1712204855/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/graph.py` & `gink-0.20240404.1712204855/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/key_set.py` & `gink-0.20240404.1712204855/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/listener.py` & `gink-0.20240404.1712204855/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/lmdb_store.py` & `gink-0.20240404.1712204855/gink/impl/lmdb_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,15 +829,15 @@
     def _add_entry(
             self,
             new_info: BundleInfo,
             txn: Trxn,
             offset: int,
             builder: EntryBuilder):
         retaining = bool(decode_muts(bytes(txn.get(b"entries", db=self._retentions))))
-        ensure_entry_is_valid(builder=builder, context=new_info)
+        ensure_entry_is_valid(builder=builder, context=new_info, offset=offset)
         placement_key = Placement.from_builder(builder, new_info, offset)
         placer_muid = placement_key.placer
         container_muid = placement_key.container
         serialized_placement_key = bytes(placement_key)
         if builder.behavior in (Behavior.DIRECTORY, Behavior.BOX, Behavior.PROPERTY, Behavior.ROLE):
             found_entry = self.get_entry_by_key(container_muid, placement_key.middle)
             if found_entry:
```

### Comparing `gink-0.20240404.1712197692/gink/impl/lmdb_utilities.py` & `gink-0.20240404.1712204855/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/log_backed_store.py` & `gink-0.20240404.1712204855/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/memory_store.py` & `gink-0.20240404.1712204855/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/muid.py` & `gink-0.20240404.1712204855/gink/impl/muid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ contains the Muid class (basically a way to represent global addresses) """
-from typing import NamedTuple, Union
+from __future__ import annotations
+from typing import NamedTuple, Union, Optional
 from uuid import UUID
 
 from .builders import MuidBuilder
 from .dummy import Dummy
 from .typedefs import MuTimestamp, Medallion
 
 
@@ -45,21 +46,33 @@
     def put_into(self, builder: MuidBuilder):
         """ Puts the data from this muid into the builder. """
         builder.offset = self.offset  # type: ignore
         builder.timestamp = self.timestamp if self.timestamp else 0  # type: ignore
         builder.medallion = self.medallion if self.medallion else 0  # type: ignore
 
     @classmethod
-    def create(cls, context, builder: Union[MuidBuilder, Dummy] = Dummy(), offset=None):
-        """ Creates a muid from a builder and optionally a bundle_info context object. """
+    def create(
+            cls,
+            context,
+            builder: Union[MuidBuilder, Dummy] = Dummy(),
+            offset: Optional[int]=None):
+        """ Creates a muid.
+
+            The context argument should either be a BundleInfo
+
+        """
         timestamp = builder.timestamp or context.timestamp  # type: ignore
         medallion = builder.medallion or context.medallion  # type: ignore
         offset = offset or builder.offset  # type: ignore
         if not offset:
             raise ValueError("no offset specified")
+        if offset < 0:
+            if not isinstance(context, Muid):
+                raise ValueError("invalid context for negative offset")
+            offset = context.offset + offset
         assert medallion, "no medallion"
         assert timestamp, "no timestamp"
         return cls(timestamp, medallion, offset)
 
     @staticmethod
     def from_str(hexed: str):
         """ the inverse of str(muid) """
```

### Comparing `gink-0.20240404.1712197692/gink/impl/pair_map.py` & `gink-0.20240404.1712204855/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/pair_set.py` & `gink-0.20240404.1712204855/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/property.py` & `gink-0.20240404.1712204855/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/role.py` & `gink-0.20240404.1712204855/gink/impl/role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/selectable_console.py` & `gink-0.20240404.1712204855/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/sequence.py` & `gink-0.20240404.1712204855/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/tuples.py` & `gink-0.20240404.1712204855/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/typedefs.py` & `gink-0.20240404.1712204855/gink/impl/typedefs.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/utilities.py` & `gink-0.20240404.1712204855/gink/impl/utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/watcher.py` & `gink-0.20240404.1712204855/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/impl/websocket_connection.py` & `gink-0.20240404.1712204855/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_box.py` & `gink-0.20240404.1712204855/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_chain_tracker.py` & `gink-0.20240404.1712204855/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_change_set_info.py` & `gink-0.20240404.1712204855/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_code_values.py` & `gink-0.20240404.1712204855/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_container.py` & `gink-0.20240404.1712204855/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_database.py` & `gink-0.20240404.1712204855/gink/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_demo.py` & `gink-0.20240404.1712204855/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_directory.py` & `gink-0.20240404.1712204855/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_graph.py` & `gink-0.20240404.1712204855/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_key_set.py` & `gink-0.20240404.1712204855/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_lmdb_store.py` & `gink-0.20240404.1712204855/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_logbackedstore.py` & `gink-0.20240404.1712204855/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_muid.py` & `gink-0.20240404.1712204855/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_names.py` & `gink-0.20240404.1712204855/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_pair_map.py` & `gink-0.20240404.1712204855/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_pair_set.py` & `gink-0.20240404.1712204855/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_property.py` & `gink-0.20240404.1712204855/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_role.py` & `gink-0.20240404.1712204855/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_sequence.py` & `gink-0.20240404.1712204855/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink/tests/test_store.py` & `gink-0.20240404.1712204855/gink/tests/test_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -303,7 +303,69 @@
         assert found[1].entry_muid == Muid(123, 789, 3)
         assert found[0].entry_muid == Muid(123, 789, 4)
 
         found = [_ for _ in store.get_ordered_entries(container=sequence, as_of=235, desc=True)]
         assert len(found) == 2
         assert found[0].entry_muid == Muid(123, 789, 3)
         assert found[1].entry_muid == Muid(123, 789, 4)
+
+
+
+def generic_test_negative_offsets(store_maker: StoreMaker):
+    """ makes sure that the get_ordered_entries works """
+    textproto1 = """
+        medallion: 789
+        chain_start: 123
+        timestamp: 123
+        changes {
+            key: 1
+            value {
+                container {
+                    behavior: SEQUENCE
+                }
+            }
+        }
+        changes {
+            key: 2
+            value {
+                entry {
+                    behavior: SEQUENCE
+                    container { offset: -1 }
+                    pointee {
+                        timestamp: -1
+                        medallion: -1
+                        offset: 1 }
+                }
+            }
+        }
+        changes {
+            key: 3
+            value {
+                entry {
+                    behavior: SEQUENCE
+                    container { offset: -2 }
+                    value { characters: "Hello, World!" }
+                }
+            }
+        }
+        changes {
+            key: 4
+            value {
+                entry {
+                    behavior: SEQUENCE
+                    container { offset: -3 }
+                    value { integer: 32 }
+                }
+            }
+        }
+    """
+    with closing(store_maker()) as store:
+        bundle_builder = BundleBuilder()
+        Parse(textproto1, bundle_builder)  # type: ignore
+        serialized = bundle_builder.SerializeToString()  # type: ignore
+        store.apply_bundle(serialized)
+        sequence = Muid(123, 789, 1)
+        found = [_ for _ in store.get_ordered_entries(container=sequence, as_of=124)]
+        assert len(found) == 3, found
+        assert found[0].entry_muid == Muid(123, 789, 2)
+        assert found[1].entry_muid == Muid(123, 789, 3)
+        assert found[2].entry_muid == Muid(123, 789, 4)
```

### Comparing `gink-0.20240404.1712197692/gink/tests/test_websocket_connection.py` & `gink-0.20240404.1712204855/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/gink.egg-info/PKG-INFO` & `gink-0.20240404.1712204855/gink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240404.1712197692
+Version: 0.20240404.1712204855
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240404.1712197692/gink.egg-info/SOURCES.txt` & `gink-0.20240404.1712204855/gink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gink-0.20240404.1712197692/setup.py` & `gink-0.20240404.1712204855/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240404.1712197692',
+    version='0.20240404.1712204855',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

