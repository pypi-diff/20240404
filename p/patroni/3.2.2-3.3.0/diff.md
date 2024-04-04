# Comparing `tmp/patroni-3.2.2.tar.gz` & `tmp/patroni-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patroni-3.2.2.tar", last modified: Wed Jan 17 09:00:23 2024, max compression
+gzip compressed data, was "patroni-3.3.0.tar", last modified: Thu Apr  4 16:58:18 2024, max compression
```

## Comparing `patroni-3.2.2.tar` & `patroni-3.3.0.tar`

### file list

```diff
@@ -1,103 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.478954 patroni-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-17 08:59:36.000000 patroni-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-17 08:59:36.000000 patroni-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-01-17 09:00:23.478954 patroni-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-01-17 08:59:36.000000 patroni-3.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.462954 patroni-3.2.2/patroni/
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84202 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/async_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    45581 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)   103299 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/ctl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.466954 patroni-3.2.2/patroni/dcs/
--rw-r--r--   0 runner    (1001) docker     (127)    85649 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/dcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29383 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/dcs/consul.py
--rw-r--r--   0 runner    (1001) docker     (127)    37958 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/dcs/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    40449 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/dcs/etcd3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/dcs/exhibitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    66106 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/dcs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19196 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/dcs/raft.py
--rw-r--r--   0 runner    (1001) docker     (127)    20322 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/dcs/zookeeper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/file_perm.py
--rw-r--r--   0 runner    (1001) docker     (127)   111319 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/ha.py
--rw-r--r--   0 runner    (1001) docker     (127)    15962 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.470954 patroni-3.2.2/patroni/postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)    63112 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.470954 patroni-3.2.2/patroni/postgresql/available_parameters/
--rw-r--r--   0 runner    (1001) docker     (127)    35206 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/available_parameters/0_postgres.yml
--rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/callback_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/cancellable.py
--rw-r--r--   0 runner    (1001) docker     (127)    19255 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/citus.py
--rw-r--r--   0 runner    (1001) docker     (127)    64769 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/postmaster.py
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/rewind.py
--rw-r--r--   0 runner    (1001) docker     (127)    37776 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/slots.py
--rw-r--r--   0 runner    (1001) docker     (127)    15621 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/postgresql/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/psycopg.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/raft_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.470954 patroni-3.2.2/patroni/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3234 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/scripts/aws.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14799 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/scripts/wale_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    40780 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51020 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.470954 patroni-3.2.2/patroni/watchdog/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/watchdog/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-01-17 08:59:36.000000 patroni-3.2.2/patroni/watchdog/linux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.478954 patroni-3.2.2/patroni.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-01-17 09:00:23.000000 patroni-3.2.2/patroni.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-01-17 09:00:23.000000 patroni-3.2.2/patroni.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 09:00:23.000000 patroni-3.2.2/patroni.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-17 09:00:23.000000 patroni-3.2.2/patroni.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-17 09:00:23.000000 patroni-3.2.2/patroni.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-17 09:00:23.000000 patroni-3.2.2/patroni.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-17 08:59:36.000000 patroni-3.2.2/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-17 08:59:36.000000 patroni-3.2.2/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-17 08:59:36.000000 patroni-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 09:00:23.478954 patroni-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-01-17 08:59:36.000000 patroni-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:00:23.478954 patroni-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    36951 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_async_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_callback_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_cancellable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_citus.py
--rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_consul.py
--rw-r--r--   0 runner    (1001) docker     (127)    41761 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_ctl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_etcd3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_exhibitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_file_perm.py
--rw-r--r--   0 runner    (1001) docker     (127)    91727 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_ha.py
--rw-r--r--   0 runner    (1001) docker     (127)    27086 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_patroni.py
--rw-r--r--   0 runner    (1001) docker     (127)    53560 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_postmaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_raft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_raft_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    16767 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_rewind.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_slots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_wale_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_watchdog.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-01-17 08:59:36.000000 patroni-3.2.2/tests/test_zookeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.591266 patroni-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-04 16:57:32.000000 patroni-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 16:57:32.000000 patroni-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-04 16:58:18.591266 patroni-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-04 16:57:32.000000 patroni-3.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.575266 patroni-3.3.0/patroni/
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84582 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/async_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39541 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23779 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102632 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/ctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.579266 patroni-3.3.0/patroni/dcs/
+-rw-r--r--   0 runner    (1001) docker     (127)    81875 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dcs/consul.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38558 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dcs/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40653 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dcs/etcd3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dcs/exhibitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67274 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dcs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19767 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dcs/raft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dcs/zookeeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/dynamic_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/file_perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111272 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/ha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21988 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.579266 patroni-3.3.0/patroni/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)    63049 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.579266 patroni-3.3.0/patroni/postgresql/available_parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)    35206 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/available_parameters/0_postgres.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/available_parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23880 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/callback_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/cancellable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67448 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.583266 patroni-3.3.0/patroni/postgresql/mpp/
+-rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/mpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20880 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/mpp/citus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/postmaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28231 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37285 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15495 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21026 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/postgresql/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/psycopg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/raft_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.583266 patroni-3.3.0/patroni/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3234 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/scripts/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.583266 patroni-3.3.0/patroni/scripts/barman/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/scripts/barman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/scripts/barman/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/scripts/barman/config_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/scripts/barman/recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/scripts/barman/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14799 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/scripts/wale_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46064 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53380 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.583266 patroni-3.3.0/patroni/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/watchdog/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-04 16:57:32.000000 patroni-3.3.0/patroni/watchdog/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.591266 patroni-3.3.0/patroni.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-04 16:58:18.000000 patroni-3.3.0/patroni.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-04 16:58:18.000000 patroni-3.3.0/patroni.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:58:18.000000 patroni-3.3.0/patroni.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 16:58:18.000000 patroni-3.3.0/patroni.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-04 16:58:18.000000 patroni-3.3.0/patroni.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 16:58:18.000000 patroni-3.3.0/patroni.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 16:57:32.000000 patroni-3.3.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 16:57:32.000000 patroni-3.3.0/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-04 16:57:32.000000 patroni-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:58:18.591266 patroni-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-04 16:57:32.000000 patroni-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:18.591266 patroni-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    37444 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_async_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30499 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_barman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14558 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_callback_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_cancellable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_citus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16479 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_consul.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40305 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_ctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17058 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_etcd3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_exhibitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_file_perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91433 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_ha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28604 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_mpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_patroni.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57649 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_postmaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_raft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_raft_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_rewind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_wale_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_watchdog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-04 16:57:32.000000 patroni-3.3.0/tests/test_zookeeper.py
```

### Comparing `patroni-3.2.2/LICENSE` & `patroni-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/PKG-INFO` & `patroni-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patroni
-Version: 3.2.2
+Version: 3.3.0
 Summary: PostgreSQL High-Available orchestrator and CLI
 Home-page: https://github.com/zalando/patroni
 Author: Alexander Kukushkin, Polina Bungina
 Author-email: akukushkin@microsoft.com, polina.bungina@zalando.de
 License: The MIT License
 Keywords: etcd governor patroni postgresql postgres ha haproxy confd zookeeper exhibitor consul streaming replication kubernetes k8s
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,21 +45,24 @@
 Requires-Dist: kazoo>=1.3.1; extra == "exhibitor"
 Provides-Extra: zookeeper
 Requires-Dist: kazoo>=1.3.1; extra == "zookeeper"
 Provides-Extra: kubernetes
 Provides-Extra: raft
 Requires-Dist: pysyncobj>=0.3.8; extra == "raft"
 Requires-Dist: cryptography>=1.4; extra == "raft"
+Provides-Extra: jsonlogger
+Requires-Dist: python-json-logger>=2.0.2; extra == "jsonlogger"
 Provides-Extra: all
 Requires-Dist: python-etcd<0.5,>=0.4.3; extra == "all"
-Requires-Dist: kazoo>=1.3.1; extra == "all"
-Requires-Dist: boto3; extra == "all"
 Requires-Dist: pysyncobj>=0.3.8; extra == "all"
-Requires-Dist: cryptography>=1.4; extra == "all"
 Requires-Dist: python-consul>=0.7.1; extra == "all"
+Requires-Dist: cryptography>=1.4; extra == "all"
+Requires-Dist: boto3; extra == "all"
+Requires-Dist: kazoo>=1.3.1; extra == "all"
+Requires-Dist: python-json-logger>=2.0.2; extra == "all"
 Provides-Extra: psycopg2
 Requires-Dist: psycopg2>=2.5.4; extra == "psycopg2"
 Provides-Extra: psycopg2-binary
 Requires-Dist: psycopg2-binary; extra == "psycopg2-binary"
 Provides-Extra: psycopg3
 Requires-Dist: psycopg[binary]>=3.0.0; extra == "psycopg3"
 
@@ -212,15 +215,15 @@
 
     > psql --host 127.0.0.1 --port 5000 postgres
 
 ==================
 YAML Configuration
 ==================
 
-Go `here <https://github.com/zalando/patroni/blob/master/docs/SETTINGS.rst>`__ for comprehensive information about settings for etcd, consul, and ZooKeeper. And for an example, see `postgres0.yml <https://github.com/zalando/patroni/blob/master/postgres0.yml>`__.
+Go `here <https://github.com/zalando/patroni/blob/master/docs/dynamic_configuration.rst>`__ for comprehensive information about settings for etcd, consul, and ZooKeeper. And for an example, see `postgres0.yml <https://github.com/zalando/patroni/blob/master/postgres0.yml>`__.
 
 =========================
 Environment Configuration
 =========================
 
 Go `here <https://github.com/zalando/patroni/blob/master/docs/ENVIRONMENT.rst>`__ for comprehensive information about configuring(overriding) settings via environment variables.
```

### Comparing `patroni-3.2.2/README.rst` & `patroni-3.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
     > psql --host 127.0.0.1 --port 5000 postgres
 
 ==================
 YAML Configuration
 ==================
 
-Go `here <https://github.com/zalando/patroni/blob/master/docs/SETTINGS.rst>`__ for comprehensive information about settings for etcd, consul, and ZooKeeper. And for an example, see `postgres0.yml <https://github.com/zalando/patroni/blob/master/postgres0.yml>`__.
+Go `here <https://github.com/zalando/patroni/blob/master/docs/dynamic_configuration.rst>`__ for comprehensive information about settings for etcd, consul, and ZooKeeper. And for an example, see `postgres0.yml <https://github.com/zalando/patroni/blob/master/postgres0.yml>`__.
 
 =========================
 Environment Configuration
 =========================
 
 Go `here <https://github.com/zalando/patroni/blob/master/docs/ENVIRONMENT.rst>`__ for comprehensive information about configuring(overriding) settings via environment variables.
```

### Comparing `patroni-3.2.2/patroni/__init__.py` & `patroni-3.3.0/patroni/__init__.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/__main__.py` & `patroni-3.3.0/patroni/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self.request = PatroniRequest(self.config, True)
 
         self.ensure_unique_name()
 
         self.watchdog = Watchdog(self.config)
         self.load_dynamic_configuration()
 
-        self.postgresql = Postgresql(self.config['postgresql'])
+        self.postgresql = Postgresql(self.config['postgresql'], self.dcs.mpp)
         self.api = RestApiServer(self, self.config['restapi'])
         self.ha = Ha(self)
 
         self._tags = self._get_tags()
         self.next_run = time.time()
         self.scheduled_restart: Dict[str, Any] = {}
```

### Comparing `patroni-3.2.2/patroni/api.py` & `patroni-3.3.0/patroni/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from ipaddress import ip_address, ip_network, IPv4Network, IPv6Network
 from socketserver import ThreadingMixIn
 from threading import Thread
 from urllib.parse import urlparse, parse_qs
 
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, TYPE_CHECKING, Union
 
-from . import psycopg
+from . import global_config, psycopg
 from .__main__ import Patroni
 from .dcs import Cluster
 from .exceptions import PostgresConnectionException, PostgresException
 from .postgresql.misc import postgres_version_to_int
 from .utils import deep_compare, enable_keepalive, parse_bool, patch_config, Retry, \
     RetryFailedError, parse_int, split_host_port, tzutc, uri, cluster_as_json
 
@@ -176,14 +176,16 @@
             * ``scope``: value of ``scope`` setting from Patroni configuration.
 
         May also add the following optional keys, depending on the status of this Patroni/PostgreSQL node:
 
             * ``tags``: tags that were set through Patroni configuration merged with dynamically applied tags;
             * ``database_system_identifier``: ``Database system identifier`` from ``pg_controldata`` output;
             * ``pending_restart``: ``True`` if PostgreSQL is pending to be restarted;
+            * ``pending_restart_reason``: dictionary where each key is the parameter that caused "pending restart" flag
+                to be set and the value is a dictionary with the old and the new value.
             * ``scheduled_restart``: a dictionary with a single key ``schedule``, which is the timestamp for the
                 scheduled restart;
             * ``watchdog_failed``: ``True`` if watchdog device is unhealthy;
             * ``logger_queue_size``: log queue length if it is longer than expected;
             * ``logger_records_lost``: number of log records that have been lost while the log queue was full.
 
         :param status_code: response HTTP status code.
@@ -192,16 +194,17 @@
         """
         patroni = self.server.patroni
         tags = patroni.ha.get_effective_tags()
         if tags:
             response['tags'] = tags
         if patroni.postgresql.sysid:
             response['database_system_identifier'] = patroni.postgresql.sysid
-        if patroni.postgresql.pending_restart:
+        if patroni.postgresql.pending_restart_reason:
             response['pending_restart'] = True
+            response['pending_restart_reason'] = dict(patroni.postgresql.pending_restart_reason)
         response['patroni'] = {
             'version': patroni.version,
             'scope': patroni.postgresql.scope,
             'name': patroni.postgresql.name
         }
         if patroni.scheduled_restart:
             response['scheduled_restart'] = patroni.scheduled_restart.copy()
@@ -286,15 +289,15 @@
                                        Useful when health-checks are executed by HAProxy.
         """
         path = '/primary' if self.path == '/' else self.path
         response = self.get_postgresql_status()
 
         patroni = self.server.patroni
         cluster = patroni.dcs.cluster
-        global_config = patroni.config.get_global_config(cluster)
+        config = global_config.from_cluster(cluster)
 
         leader_optime = cluster and cluster.last_lsn or 0
         replayed_location = response.get('xlog', {}).get('replayed_location', 0)
         max_replica_lag = parse_int(self.path_query.get('lag', [sys.maxsize])[0], 'B')
         if max_replica_lag is None:
             max_replica_lag = sys.maxsize
         is_lagging = leader_optime and leader_optime > replayed_location + max_replica_lag
@@ -304,15 +307,15 @@
 
         if not cluster and response.get('pause'):
             leader_status_code = 200 if response.get('role') in ('master', 'primary', 'standby_leader') else 503
             primary_status_code = 200 if response.get('role') in ('master', 'primary') else 503
             standby_leader_status_code = 200 if response.get('role') == 'standby_leader' else 503
         elif patroni.ha.is_leader():
             leader_status_code = 200
-            if global_config.is_standby_cluster:
+            if config.is_standby_cluster:
                 primary_status_code = replica_status_code = 503
                 standby_leader_status_code = 200 if response.get('role') in ('replica', 'standby_leader') else 503
             else:
                 primary_status_code = 200
                 standby_leader_status_code = 503
         else:
             leader_status_code = primary_status_code = standby_leader_status_code = 503
@@ -448,17 +451,16 @@
     def do_GET_cluster(self) -> None:
         """Handle a ``GET`` request to ``/cluster`` path.
 
         Write an HTTP response with JSON content based on the output of :func:`~patroni.utils.cluster_as_json`, with
         HTTP status ``200`` and the JSON representation of the cluster topology.
         """
         cluster = self.server.patroni.dcs.get_cluster()
-        global_config = self.server.patroni.config.get_global_config(cluster)
 
-        response = cluster_as_json(cluster, global_config)
+        response = cluster_as_json(cluster)
         response['scope'] = self.server.patroni.postgresql.scope
         self._write_json_response(200, response)
 
     def do_GET_history(self) -> None:
         """Handle a ``GET`` request to ``/history`` path.
 
         Write an HTTP response with a JSON content representing the history of events in the cluster, with HTTP status
@@ -631,15 +633,15 @@
                        " by Patroni.")
         metrics.append("# TYPE patroni_dcs_last_seen gauge")
         metrics.append("patroni_dcs_last_seen{0} {1}".format(labels, postgres.get('dcs_last_seen', 0)))
 
         metrics.append("# HELP patroni_pending_restart Value is 1 if the node needs a restart, 0 otherwise.")
         metrics.append("# TYPE patroni_pending_restart gauge")
         metrics.append("patroni_pending_restart{0} {1}"
-                       .format(labels, int(patroni.postgresql.pending_restart)))
+                       .format(labels, int(bool(patroni.postgresql.pending_restart_reason))))
 
         metrics.append("# HELP patroni_is_paused Value is 1 if auto failover is disabled, 0 otherwise.")
         metrics.append("# TYPE patroni_is_paused gauge")
         metrics.append("patroni_is_paused{0} {1}".format(labels, int(postgres.get('pause', 0))))
 
         self.write_response(200, '\n'.join(metrics) + '\n', content_type='text/plain')
 
@@ -860,15 +862,15 @@
         cluster = self.server.patroni.dcs.get_cluster()
         if request is None:
             # failed to parse the json
             return
         if request:
             logger.debug("received restart request: {0}".format(request))
 
-        if self.server.patroni.config.get_global_config(cluster).is_paused and 'schedule' in request:
+        if global_config.from_cluster(cluster).is_paused and 'schedule' in request:
             self.write_response(status_code, "Can't schedule restart in the paused state")
             return
 
         for k in request:
             if k == 'schedule':
                 (_, data, request[k]) = self.parse_schedule(request[k], "restart")
                 if _:
@@ -1029,15 +1031,15 @@
         :param cluster: the Patroni cluster.
         :param leader: name of the current Patroni leader.
         :param candidate: name of the Patroni node to be promoted.
         :param action: the action to be performed (``switchover`` or ``failover``).
 
         :returns: a string with the error message or ``None`` if good nodes are found.
         """
-        is_synchronous_mode = self.server.patroni.config.get_global_config(cluster).is_synchronous_mode
+        is_synchronous_mode = global_config.from_cluster(cluster).is_synchronous_mode
         if leader and (not cluster.leader or cluster.leader.name != leader):
             return 'leader name does not match'
         if candidate:
             if action == 'switchover' and is_synchronous_mode and not cluster.sync.matches(candidate):
                 return 'candidate name does not match with sync_standby'
             members = [m for m in cluster.members if m.name == candidate]
             if not members:
@@ -1087,33 +1089,33 @@
         if not request:
             return
 
         leader = request.get('leader')
         candidate = request.get('candidate') or request.get('member')
         scheduled_at = request.get('scheduled_at')
         cluster = self.server.patroni.dcs.get_cluster()
-        global_config = self.server.patroni.config.get_global_config(cluster)
+        config = global_config.from_cluster(cluster)
 
         logger.info("received %s request with leader=%s candidate=%s scheduled_at=%s",
                     action, leader, candidate, scheduled_at)
 
         if action == 'failover' and not candidate:
             data = 'Failover could be performed only to a specific candidate'
         elif action == 'switchover' and not leader:
             data = 'Switchover could be performed only from a specific leader'
 
         if not data and scheduled_at:
             if action == 'failover':
                 data = "Failover can't be scheduled"
-            elif global_config.is_paused:
+            elif config.is_paused:
                 data = "Can't schedule switchover in the paused state"
             else:
                 (status_code, data, scheduled_at) = self.parse_schedule(scheduled_at, action)
 
-        if not data and global_config.is_paused and not candidate:
+        if not data and config.is_paused and not candidate:
             data = 'Switchover is possible only to a specific candidate in a paused state'
 
         if action == 'failover' and leader:
             logger.warning('received failover request with leader specifed - performing switchover instead')
             action = 'switchover'
 
         if not data and leader == candidate:
@@ -1150,28 +1152,36 @@
         """
         self.do_POST_failover(action='switchover')
 
     @check_access
     def do_POST_citus(self) -> None:
         """Handle a ``POST`` request to ``/citus`` path.
 
-        Call :func:`~patroni.postgresql.CitusHandler.handle_event` to handle the request, then write a response with
-        HTTP status code ``200``.
+        .. note::
+            We keep this entrypoint for backward compatibility and simply dispatch the request to :meth:`do_POST_mpp`.
+        """
+        self.do_POST_mpp()
+
+    def do_POST_mpp(self) -> None:
+        """Handle a ``POST`` request to ``/mpp`` path.
+
+        Call :func:`~patroni.postgresql.mpp.AbstractMPPHandler.handle_event` to handle the request,
+        then write a response with HTTP status code ``200``.
 
         .. note::
             If unable to parse the request body, then the request is silently discarded.
         """
         request = self._read_json_content()
         if not request:
             return
 
         patroni = self.server.patroni
-        if patroni.postgresql.citus_handler.is_coordinator() and patroni.ha.is_leader():
+        if patroni.postgresql.mpp_handler.is_coordinator() and patroni.ha.is_leader():
             cluster = patroni.dcs.get_cluster()
-            patroni.postgresql.citus_handler.handle_event(cluster, request)
+            patroni.postgresql.mpp_handler.handle_event(cluster, request)
         self.write_response(200, 'OK')
 
     def parse_request(self) -> bool:
         """Override :func:`parse_request` to enrich basic functionality of :class:`~http.server.BaseHTTPRequestHandler`.
 
         Original class can only invoke :func:`do_GET`, :func:`do_POST`, :func:`do_PUT`, etc method implementations if
         they are defined.
@@ -1256,15 +1266,15 @@
             * ``cluster_unlocked``: ``True`` if cluster has no node holding the leader lock;
             * ``failsafe_mode_is_active``: ``True`` if DCS failsafe mode is currently active;
             * ``dcs_last_seen``: epoch timestamp DCS was last reached by Patroni.
 
         """
         postgresql = self.server.patroni.postgresql
         cluster = self.server.patroni.dcs.cluster
-        global_config = self.server.patroni.config.get_global_config(cluster)
+        config = global_config.from_cluster(cluster)
         try:
 
             if postgresql.state not in ('running', 'restarting', 'starting'):
                 raise RetryFailedError('')
             replication_state = ('(pg_catalog.pg_stat_get_wal_receiver()).status'
                                  if postgresql.major_version >= 90600 else 'NULL') + ", " +\
                 ("pg_catalog.current_setting('restore_command')" if postgresql.major_version >= 120000 else "NULL")
@@ -1287,18 +1297,18 @@
                     'replayed_location': row[3],
                     'replayed_timestamp': row[6],
                     'paused': row[5]} if row[1] == 0 else {
                     'location': row[2]
                 })
             }
 
-            if result['role'] == 'replica' and global_config.is_standby_cluster:
+            if result['role'] == 'replica' and config.is_standby_cluster:
                 result['role'] = postgresql.role
 
-            if result['role'] == 'replica' and global_config.is_synchronous_mode\
+            if result['role'] == 'replica' and config.is_synchronous_mode\
                     and cluster and cluster.sync.matches(postgresql.name):
                 result['sync_standby'] = True
 
             if row[1] > 0:
                 result['timeline'] = row[1]
             else:
                 leader_timeline = None\
@@ -1315,15 +1325,15 @@
         except (psycopg.Error, RetryFailedError, PostgresConnectionException):
             state = postgresql.state
             if state == 'running':
                 logger.exception('get_postgresql_status')
                 state = 'unknown'
             result: Dict[str, Any] = {'state': state, 'role': postgresql.role}
 
-        if global_config.is_paused:
+        if config.is_paused:
             result['pause'] = True
         if not cluster or cluster.is_unlocked():
             result['cluster_unlocked'] = True
         if self.server.patroni.ha.failsafe_is_active():
             result['failsafe_mode_is_active'] = True
         result['dcs_last_seen'] = self.server.patroni.dcs.last_seen
         return result
```

### Comparing `patroni-3.2.2/patroni/async_executor.py` & `patroni-3.3.0/patroni/async_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/collections.py` & `patroni-3.3.0/patroni/collections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Patroni custom object types somewhat like :mod:`collections` module.
 
-Provides a case insensitive :class:`dict` and :class:`set` object types.
+Provides a case insensitive :class:`dict` and :class:`set` object types, and `EMPTY_DICT` frozen dictionary object.
 """
 from collections import OrderedDict
-from typing import Any, Collection, Dict, Iterator, KeysView, MutableMapping, MutableSet, Optional
+from copy import deepcopy
+from typing import Any, Collection, Dict, Iterator, KeysView, Mapping, MutableMapping, MutableSet, Optional
 
 
 class CaseInsensitiveSet(MutableSet[str]):
     """A case-insensitive :class:`set`-like object.
 
     Implements all methods and operations of :class:`~typing.MutableSet`. All values are expected to be strings.
     The structure remembers the case of the last value set, however, contains testing is case insensitive.
@@ -44,24 +45,24 @@
         :Example:
 
             >>> str(CaseInsensitiveSet(('1', 'test', 'Test', 'TESt', 'test2')))  # doctest: +SKIP
             "{'TESt', 'test2', '1'}"
         """
         return str(set(self._values.values()))
 
-    def __contains__(self, value: str) -> bool:
+    def __contains__(self, value: object) -> bool:
         """Check if set contains *value*.
 
         The check is performed case-insensitively.
 
         :param value: value to be checked.
 
         :returns: ``True`` if *value* is already in the set, ``False`` otherwise.
         """
-        return value.lower() in self._values
+        return isinstance(value, str) and value.lower() in self._values
 
     def __iter__(self) -> Iterator[str]:
         """Iterate over the values in this set.
 
         :yields: values from set.
         """
         return iter(self._values.values())
@@ -203,7 +204,51 @@
 
         :Example:
 
             >>> repr(CaseInsensitiveDict({'a': 'b', 'A': 'B', 'c': 'd'}))  # doctest: +ELLIPSIS
             "<CaseInsensitiveDict{'A': 'B', 'c': 'd'} at ..."
         """
         return '<{0}{1} at {2:x}>'.format(type(self).__name__, dict(self.items()), id(self))
+
+
+class _FrozenDict(Mapping[str, Any]):
+    """Frozen dictionary object."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        """Create a new instance of :class:`_FrozenDict` with given data."""
+        self.__values: Dict[str, Any] = dict(*args, **kwargs)
+
+    def __iter__(self) -> Iterator[str]:
+        """Iterate over keys of this dict.
+
+        :yields: each key present in the dict. Yields each key with its last case that has been stored.
+        """
+        return iter(self.__values)
+
+    def __len__(self) -> int:
+        """Get the length of this dict.
+
+        :returns: number of keys in the dict.
+
+        :Example:
+
+        >>> len(_FrozenDict())
+        0
+        """
+        return len(self.__values)
+
+    def __getitem__(self, key: str) -> Any:
+        """Get the value corresponding to *key*.
+
+        :returns: value corresponding to *key*.
+        """
+        return self.__values[key]
+
+    def copy(self) -> Dict[str, Any]:
+        """Create a copy of this dict.
+
+        :return: a new dict object with the same keys and values of this dict.
+        """
+        return deepcopy(self.__values)
+
+
+EMPTY_DICT = _FrozenDict()
```

### Comparing `patroni-3.2.2/patroni/config.py` & `patroni-3.3.0/patroni/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Facilities related to Patroni configuration."""
+import re
 import json
 import logging
 import os
 import shutil
 import tempfile
 import yaml
 
 from collections import defaultdict
 from copy import deepcopy
 from typing import Any, Callable, Collection, Dict, List, Optional, Union, TYPE_CHECKING
 
 from . import PATRONI_ENV_PREFIX
-from .collections import CaseInsensitiveDict
-from .dcs import ClusterConfig, Cluster
+from .collections import CaseInsensitiveDict, EMPTY_DICT
+from .dcs import ClusterConfig
 from .exceptions import ConfigParseError
 from .file_perm import pg_perm
 from .postgresql.config import ConfigHandler
 from .validator import IntValidator
 from .utils import deep_compare, parse_bool, parse_int, patch_config
 
 logger = logging.getLogger(__name__)
@@ -50,162 +51,14 @@
         :class:`ConfigParseError`: if *conf* is empty.
     """
     if not conf:
         raise ConfigParseError("Config is empty.")
     return []
 
 
-class GlobalConfig(object):
-    """A class that wraps global configuration and provides convenient methods to access/check values.
-
-    It is instantiated either by calling :func:`get_global_config` or :meth:`Config.get_global_config`, which picks
-    either a configuration from provided :class:`Cluster` object (the most up-to-date) or from the
-    local cache if :class:`ClusterConfig` is not initialized or doesn't have a valid config.
-    """
-
-    def __init__(self, config: Dict[str, Any]) -> None:
-        """Initialize :class:`GlobalConfig` object with given *config*.
-
-        :param config: current configuration either from
-                       :class:`ClusterConfig` or from :func:`Config.dynamic_configuration`.
-        """
-        self.__config = config
-
-    def get(self, name: str) -> Any:
-        """Gets global configuration value by *name*.
-
-        :param name: parameter name.
-
-        :returns: configuration value or ``None`` if it is missing.
-        """
-        return self.__config.get(name)
-
-    def check_mode(self, mode: str) -> bool:
-        """Checks whether the certain parameter is enabled.
-
-        :param mode: parameter name, e.g. ``synchronous_mode``, ``failsafe_mode``, ``pause``, ``check_timeline``, and
-            so on.
-
-        :returns: ``True`` if parameter *mode* is enabled in the global configuration.
-        """
-        return bool(parse_bool(self.__config.get(mode)))
-
-    @property
-    def is_paused(self) -> bool:
-        """``True`` if cluster is in maintenance mode."""
-        return self.check_mode('pause')
-
-    @property
-    def is_synchronous_mode(self) -> bool:
-        """``True`` if synchronous replication is requested and it is not a standby cluster config."""
-        return self.check_mode('synchronous_mode') and not self.is_standby_cluster
-
-    @property
-    def is_synchronous_mode_strict(self) -> bool:
-        """``True`` if at least one synchronous node is required."""
-        return self.check_mode('synchronous_mode_strict')
-
-    def get_standby_cluster_config(self) -> Union[Dict[str, Any], Any]:
-        """Get ``standby_cluster`` configuration.
-
-        :returns: a copy of ``standby_cluster`` configuration.
-        """
-        return deepcopy(self.get('standby_cluster'))
-
-    @property
-    def is_standby_cluster(self) -> bool:
-        """``True`` if global configuration has a valid ``standby_cluster`` section."""
-        config = self.get_standby_cluster_config()
-        return isinstance(config, dict) and\
-            bool(config.get('host') or config.get('port') or config.get('restore_command'))
-
-    def get_int(self, name: str, default: int = 0) -> int:
-        """Gets current value of *name* from the global configuration and try to return it as :class:`int`.
-
-        :param name: name of the parameter.
-        :param default: default value if *name* is not in the configuration or invalid.
-
-        :returns: currently configured value of *name* from the global configuration or *default* if it is not set or
-            invalid.
-        """
-        ret = parse_int(self.get(name))
-        return default if ret is None else ret
-
-    @property
-    def min_synchronous_nodes(self) -> int:
-        """The minimal number of synchronous nodes based on whether ``synchronous_mode_strict`` is enabled or not."""
-        return 1 if self.is_synchronous_mode_strict else 0
-
-    @property
-    def synchronous_node_count(self) -> int:
-        """Currently configured value of ``synchronous_node_count`` from the global configuration.
-
-        Assume ``1`` if it is not set or invalid.
-        """
-        return max(self.get_int('synchronous_node_count', 1), self.min_synchronous_nodes)
-
-    @property
-    def maximum_lag_on_failover(self) -> int:
-        """Currently configured value of ``maximum_lag_on_failover`` from the global configuration.
-
-        Assume ``1048576`` if it is not set or invalid.
-        """
-        return self.get_int('maximum_lag_on_failover', 1048576)
-
-    @property
-    def maximum_lag_on_syncnode(self) -> int:
-        """Currently configured value of ``maximum_lag_on_syncnode`` from the global configuration.
-
-        Assume ``-1`` if it is not set or invalid.
-        """
-        return self.get_int('maximum_lag_on_syncnode', -1)
-
-    @property
-    def primary_start_timeout(self) -> int:
-        """Currently configured value of ``primary_start_timeout`` from the global configuration.
-
-        Assume ``300`` if it is not set or invalid.
-
-        .. note::
-            ``master_start_timeout`` is still supported to keep backward compatibility.
-        """
-        default = 300
-        return self.get_int('primary_start_timeout', default)\
-            if 'primary_start_timeout' in self.__config else self.get_int('master_start_timeout', default)
-
-    @property
-    def primary_stop_timeout(self) -> int:
-        """Currently configured value of ``primary_stop_timeout`` from the global configuration.
-
-        Assume ``0`` if it is not set or invalid.
-
-        .. note::
-            ``master_stop_timeout`` is still supported to keep backward compatibility.
-        """
-        default = 0
-        return self.get_int('primary_stop_timeout', default)\
-            if 'primary_stop_timeout' in self.__config else self.get_int('master_stop_timeout', default)
-
-
-def get_global_config(cluster: Optional[Cluster], default: Optional[Dict[str, Any]] = None) -> GlobalConfig:
-    """Instantiates :class:`GlobalConfig` based on the input.
-
-    :param cluster: the currently known cluster state from DCS.
-    :param default: default configuration, which will be used if there is no valid *cluster.config*.
-
-    :returns: :class:`GlobalConfig` object.
-    """
-    # Try to protect from the case when DCS was wiped out
-    if cluster and cluster.config and cluster.config.modify_version:
-        config = cluster.config.data
-    else:
-        config = default or {}
-    return GlobalConfig(deepcopy(config))
-
-
 class Config(object):
     """Handle Patroni configuration.
 
     This class is responsible for:
 
       1) Building and giving access to ``effective_configuration`` from:
 
@@ -588,22 +441,22 @@
         :returns: copy of *dynamic_configuration*, merged with default dynamic configuration and with some sanity checks
             performed over it.
         """
         config = self.get_default_config()
 
         for name, value in dynamic_configuration.items():
             if name == 'postgresql':
-                for name, value in (value or {}).items():
+                for name, value in (value or EMPTY_DICT).items():
                     if name == 'parameters':
                         config['postgresql'][name].update(self._process_postgresql_parameters(value))
                     elif name not in ('connect_address', 'proxy_address', 'listen',
                                       'config_dir', 'data_dir', 'pgpass', 'authentication'):
                         config['postgresql'][name] = deepcopy(value)
             elif name == 'standby_cluster':
-                for name, value in (value or {}).items():
+                for name, value in (value or EMPTY_DICT).items():
                     if name in self.__DEFAULT_CONFIG['standby_cluster']:
                         config['standby_cluster'][name] = deepcopy(value)
             elif name in config:  # only variables present in __DEFAULT_CONFIG allowed to be overridden from DCS
                 config[name] = int(value)
         return config
 
     @staticmethod
@@ -678,16 +531,16 @@
         _set_section_values('restapi', ['listen', 'connect_address', 'certfile', 'keyfile', 'keyfile_password',
                                         'cafile', 'ciphers', 'verify_client', 'http_extra_headers',
                                         'https_extra_headers', 'allowlist', 'allowlist_include_members',
                                         'request_queue_size'])
         _set_section_values('ctl', ['insecure', 'cacert', 'certfile', 'keyfile', 'keyfile_password'])
         _set_section_values('postgresql', ['listen', 'connect_address', 'proxy_address',
                                            'config_dir', 'data_dir', 'pgpass', 'bin_dir'])
-        _set_section_values('log', ['level', 'traceback_level', 'format', 'dateformat', 'max_queue_size',
-                                    'dir', 'file_size', 'file_num', 'loggers'])
+        _set_section_values('log', ['type', 'level', 'traceback_level', 'format', 'dateformat', 'static_fields',
+                                    'max_queue_size', 'dir', 'file_size', 'file_num', 'loggers'])
         _set_section_values('raft', ['data_dir', 'self_addr', 'partner_addrs', 'password', 'bind_addr'])
 
         for binary in ('pg_ctl', 'initdb', 'pg_controldata', 'pg_basebackup', 'postgres', 'pg_isready', 'pg_rewind'):
             value = _popenv('POSTGRESQL_BIN_' + binary)
             if value:
                 ret['postgresql'].setdefault('bin_name', {})[binary] = value
 
@@ -726,14 +579,20 @@
         for first, second in (('raft', 'partner_addrs'), ('restapi', 'allowlist')):
             value = ret.get(first, {}).pop(second, None)
             if value:
                 value = _parse_list(value)
                 if value:
                     ret[first][second] = value
 
+        logformat = ret.get('log', {}).get('format')
+        if logformat and not re.search(r'%\(\w+\)', logformat):
+            logformat = _parse_list(logformat)
+            if logformat:
+                ret['log']['format'] = logformat
+
         def _parse_dict(value: str) -> Optional[Dict[str, Any]]:
             """Parse an YAML dictionary *value* as a :class:`dict`.
 
             :param value: YAML dictionary as a string.
 
             :returns: *value* as :class:`dict`.
             """
@@ -741,15 +600,20 @@
                 value = '{{{0}}}'.format(value)
             try:
                 return yaml.safe_load(value)
             except Exception:
                 logger.exception('Exception when parsing dict %s', value)
                 return None
 
-        for first, params in (('restapi', ('http_extra_headers', 'https_extra_headers')), ('log', ('loggers',))):
+        dict_configs = (
+            ('restapi', ('http_extra_headers', 'https_extra_headers')),
+            ('log', ('static_fields', 'loggers'))
+        )
+
+        for first, params in dict_configs:
             for second in params:
                 value = ret.get(first, {}).pop(second, None)
                 if value:
                     value = _parse_dict(value)
                     if value:
                         ret[first][second] = value
 
@@ -788,26 +652,26 @@
                 name, suffix = (param[len(PATRONI_ENV_PREFIX):].split('_', 1) + [''])[:2]
                 if suffix in ('HOST', 'HOSTS', 'PORT', 'USE_PROXIES', 'PROTOCOL', 'SRV', 'SRV_SUFFIX', 'URL', 'PROXY',
                               'CACERT', 'CERT', 'KEY', 'VERIFY', 'TOKEN', 'CHECKS', 'DC', 'CONSISTENCY',
                               'REGISTER_SERVICE', 'SERVICE_CHECK_INTERVAL', 'SERVICE_CHECK_TLS_SERVER_NAME',
                               'SERVICE_TAGS', 'NAMESPACE', 'CONTEXT', 'USE_ENDPOINTS', 'SCOPE_LABEL', 'ROLE_LABEL',
                               'POD_IP', 'PORTS', 'LABELS', 'BYPASS_API_SERVICE', 'RETRIABLE_HTTP_CODES', 'KEY_PASSWORD',
                               'USE_SSL', 'SET_ACLS', 'GROUP', 'DATABASE', 'LEADER_LABEL_VALUE', 'FOLLOWER_LABEL_VALUE',
-                              'STANDBY_LEADER_LABEL_VALUE', 'TMP_ROLE_LABEL') and name:
+                              'STANDBY_LEADER_LABEL_VALUE', 'TMP_ROLE_LABEL', 'AUTH_DATA') and name:
                     value = os.environ.pop(param)
                     if name == 'CITUS':
                         if suffix == 'GROUP':
                             value = parse_int(value)
                         elif suffix != 'DATABASE':
                             continue
                     elif suffix == 'PORT':
                         value = value and parse_int(value)
                     elif suffix in ('HOSTS', 'PORTS', 'CHECKS', 'SERVICE_TAGS', 'RETRIABLE_HTTP_CODES'):
                         value = value and _parse_list(value)
-                    elif suffix in ('LABELS', 'SET_ACLS'):
+                    elif suffix in ('LABELS', 'SET_ACLS', 'AUTH_DATA'):
                         value = _parse_dict(value)
                     elif suffix in ('USE_PROXIES', 'REGISTER_SERVICE', 'USE_ENDPOINTS', 'BYPASS_API_SERVICE', 'VERIFY'):
                         value = parse_bool(value)
                     if value is not None:
                         ret[name.lower()][suffix.lower()] = value
         for dcs in ('etcd', 'etcd3'):
             if dcs in ret:
@@ -946,26 +810,14 @@
     def copy(self) -> Dict[str, Any]:
         """Get a deep copy of effective Patroni configuration.
 
         :returns: a deep copy of the Patroni configuration.
         """
         return deepcopy(self.__effective_configuration)
 
-    def get_global_config(self, cluster: Optional[Cluster]) -> GlobalConfig:
-        """Instantiate :class:`GlobalConfig` based on input.
-
-        Use the configuration from provided *cluster* (the most up-to-date) or from the
-        local cache if *cluster.config* is not initialized or doesn't have a valid config.
-
-        :param cluster: the currently known cluster state from DCS.
-
-        :returns: :class:`GlobalConfig` object.
-        """
-        return get_global_config(cluster, self._dynamic_configuration)
-
     def _validate_failover_tags(self) -> None:
         """Check ``nofailover``/``failover_priority`` config and warn user if it's contradictory.
 
         .. note::
           To preserve sanity (and backwards compatibility) the ``nofailover`` tag will still exist. A contradictory
           configuration is one where ``nofailover`` is ``True`` but ``failover_priority > 0``, or where
           ``nofailover`` is ``False``, but ``failover_priority <= 0``. Essentially, ``nofailover`` and
```

### Comparing `patroni-3.2.2/patroni/config_generator.py` & `patroni-3.3.0/patroni/config_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from contextlib import contextmanager
 from typing import Any, Dict, Iterator, List, Optional, TextIO, Tuple, TYPE_CHECKING, Union
 if TYPE_CHECKING:  # pragma: no cover
     from psycopg import Cursor
     from psycopg2 import cursor
 
 from . import psycopg
+from .collections import EMPTY_DICT
 from .config import Config
 from .exceptions import PatroniException
 from .log import PatroniLogger
 from .postgresql.config import ConfigHandler, parse_dsn
 from .postgresql.misc import postgres_major_version_to_int
 from .utils import get_major_version, parse_bool, patch_config, read_stripped
 
@@ -95,14 +96,15 @@
             'scope': NO_VALUE_MSG,
             'name': cls._HOSTNAME,
             'restapi': {
                 'connect_address': cls._IP + ':8008',
                 'listen': cls._IP + ':8008'
             },
             'log': {
+                'type': PatroniLogger.DEFAULT_TYPE,
                 'level': PatroniLogger.DEFAULT_LEVEL,
                 'traceback_level': PatroniLogger.DEFAULT_TRACEBACK_LEVEL,
                 'format': PatroniLogger.DEFAULT_FORMAT,
                 'max_queue_size': PatroniLogger.DEFAULT_MAX_QUEUE_SIZE
             },
             'postgresql': {
                 'data_dir': NO_VALUE_MSG,
@@ -121,14 +123,15 @@
                 }
             },
             'tags': {
                 'failover_priority': 1,
                 'noloadbalance': False,
                 'clonefrom': True,
                 'nosync': False,
+                'nostream': False,
             }
         }
 
         dynamic_config = Config.get_default_config()
         # to properly dump CaseInsensitiveDict as YAML later
         dynamic_config['postgresql']['parameters'] = dict(dynamic_config['postgresql']['parameters'])
         config = Config('', None).local_configuration  # Get values from env
@@ -238,15 +241,16 @@
     def _get_int_major_version(self) -> int:
         """Get major PostgreSQL version from the binary as an integer.
 
         :returns: an integer PostgreSQL major version representation gathered from the PostgreSQL binary.
                   See :func:`~patroni.postgresql.misc.postgres_major_version_to_int` and
                   :func:`~patroni.utils.get_major_version`.
         """
-        postgres_bin = ((self.config.get('postgresql') or {}).get('bin_name') or {}).get('postgres', 'postgres')
+        postgres_bin = ((self.config.get('postgresql')
+                         or EMPTY_DICT).get('bin_name') or EMPTY_DICT).get('postgres', 'postgres')
         return postgres_major_version_to_int(get_major_version(self.config['postgresql'].get('bin_dir'), postgres_bin))
 
     def generate(self) -> None:
         """Generate sample config using some sane defaults and update :attr:`~AbstractConfigGenerator.config`."""
         self.pg_major = self._get_int_major_version()
 
         self.config['postgresql']['parameters'] = {'password_encryption': self.get_auth_method}
@@ -405,16 +409,18 @@
         Information set is based on the options used for connection.
         """
         su_params: Dict[str, str] = {}
         for conn_param, env_var in _AUTH_ALLOWED_PARAMETERS_MAPPING.items():
             val = self.parsed_dsn.get(conn_param, os.getenv(env_var))
             if val:
                 su_params[conn_param] = val
-        patroni_env_su_username = ((self.config.get('authentication') or {}).get('superuser') or {}).get('username')
-        patroni_env_su_pwd = ((self.config.get('authentication') or {}).get('superuser') or {}).get('password')
+        patroni_env_su_username = ((self.config.get('authentication')
+                                    or EMPTY_DICT).get('superuser') or EMPTY_DICT).get('username')
+        patroni_env_su_pwd = ((self.config.get('authentication')
+                               or EMPTY_DICT).get('superuser') or EMPTY_DICT).get('password')
         # because we use "username" in the config for some reason
         su_params['username'] = su_params.pop('user', patroni_env_su_username) or getuser()
         su_params['password'] = su_params.get('password', patroni_env_su_pwd) or \
             getpass('Please enter the user password:')
         self.config['postgresql']['authentication'] = {
             'superuser': su_params,
             'replication': {'username': NO_VALUE_MSG, 'password': NO_VALUE_MSG}
```

### Comparing `patroni-3.2.2/patroni/ctl.py` & `patroni-3.3.0/patroni/ctl.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,29 @@
 from prettytable import ALL, FRAME, PrettyTable
 from urllib.parse import urlparse
 from typing import Any, Dict, Iterator, List, Optional, Union, Tuple, TYPE_CHECKING
 if TYPE_CHECKING:  # pragma: no cover
     from psycopg import Cursor
     from psycopg2 import cursor
 
-try:
-    from ydiff import markup_to_pager, PatchStream  # pyright: ignore [reportMissingModuleSource]
+try:  # pragma: no cover
+    from ydiff import markup_to_pager  # pyright: ignore [reportMissingModuleSource]
+    try:
+        from ydiff import PatchStream  # pyright: ignore [reportMissingModuleSource]
+    except ImportError:
+        PatchStream = iter
 except ImportError:  # pragma: no cover
     from cdiff import markup_to_pager, PatchStream  # pyright: ignore [reportMissingModuleSource]
 
-from .config import Config, get_global_config
+from . import global_config
+from .config import Config
 from .dcs import get_dcs as _get_dcs, AbstractDCS, Cluster, Member
 from .exceptions import PatroniException
 from .postgresql.misc import postgres_version_to_int
+from .postgresql.mpp import get_mpp
 from .utils import cluster_as_json, patch_config, polling_loop
 from .request import PatroniRequest
 from .version import __version__
 
 CONFIG_DIR_PATH = click.get_app_dir('patroni')
 CONFIG_FILE_PATH = os.path.join(CONFIG_DIR_PATH, 'patronictl.yaml')
 DCS_DEFAULTS: Dict[str, Dict[str, Any]] = {
@@ -251,23 +257,31 @@
     if dcs_kwargs:
         for d in DCS_DEFAULTS:
             config.pop(d, None)
         config.update(dcs_kwargs)
     return config
 
 
+def _get_configuration() -> Dict[str, Any]:
+    """Get configuration object.
+
+    :returns: configuration object from the current context.
+    """
+    return click.get_current_context().obj['__config']
+
+
 option_format = click.option('--format', '-f', 'fmt', help='Output format', default='pretty',
                              type=click.Choice(['pretty', 'tsv', 'json', 'yaml', 'yml']))
 option_watchrefresh = click.option('-w', '--watch', type=float, help='Auto update the screen every X seconds')
 option_watch = click.option('-W', is_flag=True, help='Auto update the screen every 2 seconds')
 option_force = click.option('--force', is_flag=True, help='Do not ask for confirmation at any point')
 arg_cluster_name = click.argument('cluster_name', required=False,
-                                  default=lambda: click.get_current_context().obj.get('scope'))
+                                  default=lambda: _get_configuration().get('scope'))
 option_default_citus_group = click.option('--group', required=False, type=int, help='Citus group',
-                                          default=lambda: click.get_current_context().obj.get('citus', {}).get('group'))
+                                          default=lambda: _get_configuration().get('citus', {}).get('group'))
 option_citus_group = click.option('--group', required=False, type=int, help='Citus group')
 role_choice = click.Choice(['leader', 'primary', 'standby-leader', 'replica', 'standby', 'any', 'master'])
 
 
 @click.group(cls=click.Group)
 @click.option('--config-file', '-c', help='Configuration file',
               envvar='PATRONICTL_CONFIG_FILE', default=CONFIG_FILE_PATH)
@@ -297,41 +311,51 @@
         ``ctl.insecure` in the configuration file.
     """
     level = 'WARNING'
     for name in ('LOGLEVEL', 'PATRONI_LOGLEVEL', 'PATRONI_LOG_LEVEL'):
         level = os.environ.get(name, level)
     logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s', level=level)
     logging.captureWarnings(True)  # Capture eventual SSL warning
-    ctx.obj = load_config(config_file, dcs_url)
+    config = load_config(config_file, dcs_url)
     # backward compatibility for configuration file where ctl section is not defined
-    ctx.obj.setdefault('ctl', {})['insecure'] = ctx.obj.get('ctl', {}).get('insecure') or insecure
+    config.setdefault('ctl', {})['insecure'] = config.get('ctl', {}).get('insecure') or insecure
+    ctx.obj = {'__config': config, '__mpp': get_mpp(config)}
+
 
+def is_citus_cluster() -> bool:
+    """Check if we are working with Citus cluster.
 
-def get_dcs(config: Dict[str, Any], scope: str, group: Optional[int]) -> AbstractDCS:
+    :returns: ``True`` if configuration has ``citus`` section, otherwise ``False``.
+    """
+    return click.get_current_context().obj['__mpp'].is_enabled()
+
+
+def get_dcs(scope: str, group: Optional[int]) -> AbstractDCS:
     """Get the DCS object.
 
-    :param config: Patroni configuration.
     :param scope: cluster name.
     :param group: if *group* is defined, use it to select which alternative Citus group this DCS refers to. If *group*
         is ``None`` and a Citus configuration exists, assume this is the coordinator. Coordinator has the group ``0``.
         Refer to the module note for more details.
 
     :returns: a subclass of :class:`~patroni.dcs.AbstractDCS`, according to the DCS technology that is configured.
 
     :raises:
         :class:`PatroniCtlException`: if not suitable DCS configuration could be found.
     """
+    config = _get_configuration()
     config.update({'scope': scope, 'patronictl': True})
     if group is not None:
-        config['citus'] = {'group': group}
+        config['citus'] = {'group': group, 'database': 'postgres'}
     config.setdefault('name', scope)
     try:
         dcs = _get_dcs(config)
-        if config.get('citus') and group is None:
-            dcs.is_citus_coordinator = lambda: True
+        if is_citus_cluster() and group is None:
+            dcs.is_mpp_coordinator = lambda: True
+        click.get_current_context().obj['__mpp'] = dcs.mpp
         return dcs
     except PatroniException as e:
         raise PatroniCtlException(str(e))
 
 
 def request_patroni(member: Member, method: str = 'GET',
                     endpoint: Optional[str] = None, data: Optional[Any] = None) -> urllib3.response.HTTPResponse:
@@ -343,15 +367,15 @@
     :param data: anything to be used as the request body.
 
     :returns: the response for the request.
     """
     ctx = click.get_current_context()  # the current click context
     request_executor = ctx.obj.get('__request_patroni')
     if not request_executor:
-        request_executor = ctx.obj['__request_patroni'] = PatroniRequest(ctx.obj)
+        request_executor = ctx.obj['__request_patroni'] = PatroniRequest(_get_configuration())
     return request_executor(member, method, endpoint, data)
 
 
 def print_output(columns: Optional[List[str]], rows: List[List[Any]], alignment: Optional[Dict[str, str]] = None,
                  fmt: str = 'pretty', header: str = '', delimiter: str = '\t') -> None:
     """Print tabular information.
 
@@ -410,17 +434,17 @@
                 table.align[k] = v
             for r in rows:
                 table.add_row(r)
             click.echo(table)
 
 
 def watching(w: bool, watch: Optional[int], max_count: Optional[int] = None, clear: bool = True) -> Iterator[int]:
-    """Yield a value every ``x`` seconds.
+    """Yield a value every ``watch`` seconds.
 
-    Used to run a command with a watch-based aproach.
+    Used to run a command with a watch-based approach.
 
     :param w: if ``True`` and *watch* is ``None``, then *watch* assumes the value ``2``.
     :param watch: amount of seconds to wait before yielding another value.
     :param max_count: maximum number of yielded values. If ``None`` keep yielding values indefinitely.
     :param clear: if the screen should be cleared out at each iteration.
 
     :yields: ``0`` each time *watch* seconds have passed.
@@ -448,33 +472,31 @@
         time.sleep(watch)
         counter += 1
         if clear:
             click.clear()
         yield 0
 
 
-def get_all_members(obj: Dict[str, Any], cluster: Cluster,
-                    group: Optional[int], role: str = 'leader') -> Iterator[Member]:
+def get_all_members(cluster: Cluster, group: Optional[int], role: str = 'leader') -> Iterator[Member]:
     """Get all cluster members that have the given *role*.
 
-    :param obj: the Patroni configuration.
     :param cluster: the Patroni cluster.
     :param group: filter which Citus group we should get members from. If ``None`` get from all groups.
     :param role: role to filter members. Can be one among:
 
         * ``primary`` or ``master``: the primary PostgreSQL instance;
         * ``replica`` or ``standby``: a standby PostgreSQL instance;
         * ``leader``: the leader of a Patroni cluster. Can also be used to get the leader of a Patroni standby cluster;
         * ``standby-leader``: the leader of a Patroni standby cluster;
         * ``any``: matches any node independent of its role.
 
     :yields: members that have the given *role*.
     """
     clusters = {0: cluster}
-    if obj.get('citus') and group is None:
+    if is_citus_cluster() and group is None:
         clusters.update(cluster.workers)
     if role in ('leader', 'master', 'primary', 'standby-leader'):
         # In the DCS the members' role can be one among: ``primary``, ``master``, ``replica`` or ``standby_leader``.
         # ``primary`` and ``master`` are the same thing, so we map both to ``master`` to have a simpler ``if``.
         # In a future release we might remove ``master`` from the available roles for the DCS members.
         role = {'primary': 'master', 'standby-leader': 'standby_leader'}.get(role, role)
         for cluster in clusters.values():
@@ -488,19 +510,18 @@
     for cluster in clusters.values():
         leader_name = (cluster.leader.member.name if cluster.leader else None)
         for m in cluster.members:
             if role == 'any' or role in ('replica', 'standby') and m.name != leader_name:
                 yield m
 
 
-def get_any_member(obj: Dict[str, Any], cluster: Cluster, group: Optional[int],
+def get_any_member(cluster: Cluster, group: Optional[int],
                    role: Optional[str] = None, member: Optional[str] = None) -> Optional[Member]:
     """Get the first found cluster member that has the given *role*.
 
-    :param obj: the Patroni configuration.
     :param cluster: the Patroni cluster.
     :param group: filter which Citus group we should get members from. If ``None`` get from all groups.
     :param role: role to filter members. See :func:`get_all_members` for available options.
     :param member: if specified, then besides having the given *role*, the cluster member's name should be *member*.
 
     :returns: the first found cluster member that has the given *role*.
 
@@ -510,15 +531,15 @@
     if member is not None:
         if role is not None:
             raise PatroniCtlException('--role and --member are mutually exclusive options')
         role = 'any'
     elif role is None:
         role = 'leader'
 
-    for m in get_all_members(obj, cluster, group, role):
+    for m in get_all_members(cluster, group, role):
         if member is None or m.name == member:
             return m
 
 
 def get_all_members_leader_first(cluster: Cluster) -> Iterator[Member]:
     """Get all cluster members, with the cluster leader being yielded first.
 
@@ -531,39 +552,38 @@
     if leader_name and cluster.leader:
         yield cluster.leader.member
     for member in cluster.members:
         if member.api_url and member.name != leader_name:
             yield member
 
 
-def get_cursor(obj: Dict[str, Any], cluster: Cluster, group: Optional[int], connect_parameters: Dict[str, Any],
+def get_cursor(cluster: Cluster, group: Optional[int], connect_parameters: Dict[str, Any],
                role: Optional[str] = None, member_name: Optional[str] = None) -> Union['cursor', 'Cursor[Any]', None]:
     """Get a cursor object to execute queries against a member that has the given *role* or *member_name*.
 
     .. note::
         Besides what is passed through *connect_parameters*, this function also sets the following parameters:
             * ``fallback_application_name``: as ``Patroni ctl``;
             * ``connect_timeout``: as ``5``.
 
-    :param obj: the Patroni configuration.
     :param cluster: the Patroni cluster.
     :param group: filter which Citus group we should get members to create a cursor against. If ``None`` consider
         members from all groups.
     :param connect_parameters: database connection parameters.
     :param role: role to filter members. See :func:`get_all_members` for available options.
     :param member_name: if specified, then besides having the given *role*, the cluster member's name should be
         *member_name*.
 
     :returns: a cursor object to execute queries against the database. Can be either:
 
         * A :class:`psycopg.Cursor` if using :mod:`psycopg`; or
         * A :class:`psycopg2.extensions.cursor` if using :mod:`psycopg2`;
         * ``None`` if not able to get a cursor that attendees *role* and *member_name*.
     """
-    member = get_any_member(obj, cluster, group, role=role, member=member_name)
+    member = get_any_member(cluster, group, role=role, member=member_name)
     if member is None:
         return None
 
     params = member.conn_kwargs(connect_parameters)
     params.update({'fallback_application_name': 'Patroni ctl', 'connect_timeout': '5'})
     if 'dbname' in connect_parameters:
         params['dbname'] = connect_parameters['dbname']
@@ -590,15 +610,15 @@
         return cursor
 
     conn.close()
 
     return None
 
 
-def get_members(obj: Dict[str, Any], cluster: Cluster, cluster_name: str, member_names: List[str], role: str,
+def get_members(cluster: Cluster, cluster_name: str, member_names: List[str], role: str,
                 force: bool, action: str, ask_confirmation: bool = True, group: Optional[int] = None) -> List[Member]:
     """Get the list of members based on the given filters.
 
     .. note::
         Contain some filtering and checks processing that are common to several actions that are exposed
         by `patronictl`, like:
 
@@ -614,15 +634,14 @@
         over the retrieved members. That won't actually perform the action, but it works as the "last confirmation"
         before the *action* is processed by the caller method.
 
         Additional checks can also be implemented in the caller method, in which case you might want to pass
         ``ask_confirmation=False``, and later call :func:`confirm_members_action` manually in the caller method. That
         way the workflow won't look broken to the user that is interacting with ``patronictl``.
 
-    :param obj: Patroni configuration.
     :param cluster: Patroni cluster.
     :param cluster_name: name of the Patroni cluster.
     :param member_names: used to filter which members should take the *action* based on their names. Each item is the
         name of a Patroni member, as per ``name`` configuration. If *member_names* is an empty :class:`tuple` no filters
         are applied based on names.
     :param role: used to filter which members should take the *action* based on their role. See :func:`get_all_members`
         for available options.
@@ -643,21 +662,21 @@
 
     :raises:
         :class:`PatroniCtlException`: if
             * Cluster does not have members that match the given *role*; or
             * Cluster does not have members that match the given *member_names*; or
             * No member with given *role* is found among the specified *member_names*.
     """
-    members = list(get_all_members(obj, cluster, group, role))
+    members = list(get_all_members(cluster, group, role))
 
     candidates = {m.name for m in members}
     if not force or role:
         if not member_names and not candidates:
             raise PatroniCtlException('{0} cluster doesn\'t have any members'.format(cluster_name))
-        output_members(obj, cluster, cluster_name, group=group)
+        output_members(cluster, cluster_name, group=group)
 
     if member_names:
         member_names = list(set(member_names) & candidates)
         if not member_names:
             raise PatroniCtlException('No {0} among provided members'.format(role))
     elif action != 'reinitialize':
         member_names = list(candidates)
@@ -709,39 +728,36 @@
 
 
 @ctl.command('dsn', help='Generate a dsn for the provided member, defaults to a dsn of the leader')
 @click.option('--role', '-r', help='Give a dsn of any member with this role', type=role_choice, default=None)
 @click.option('--member', '-m', help='Generate a dsn for this member', type=str)
 @arg_cluster_name
 @option_citus_group
-@click.pass_obj
-def dsn(obj: Dict[str, Any], cluster_name: str, group: Optional[int],
-        role: Optional[str], member: Optional[str]) -> None:
+def dsn(cluster_name: str, group: Optional[int], role: Optional[str], member: Optional[str]) -> None:
     """Process ``dsn`` command of ``patronictl`` utility.
 
     Get DSN to connect to *member*.
 
     .. note::
         If no *role* nor *member* is given assume *role* as ``leader``.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should get members to get DSN from. Refer to the module note for more
         details.
     :param role: filter which members to get DSN from based on their role. See :func:`get_all_members` for available
         options.
     :param member: filter which member to get DSN from based on its name.
 
     :raises:
         :class:`PatroniCtlException`: if
             * both *role* and *member* are provided; or
             * No member matches requested *member* or *role*.
     """
-    cluster = get_dcs(obj, cluster_name, group).get_cluster()
-    m = get_any_member(obj, cluster, group, role=role, member=member)
+    cluster = get_dcs(cluster_name, group).get_cluster()
+    m = get_any_member(cluster, group, role=role, member=member)
     if m is None:
         raise PatroniCtlException('Can not find a suitable member')
 
     params = m.conn_kwargs()
     click.echo('host={host} port={port}'.format(**params))
 
 
@@ -755,17 +771,15 @@
 @option_watch
 @option_watchrefresh
 @click.option('--role', '-r', help='The role of the query', type=role_choice, default=None)
 @click.option('--member', '-m', help='Query a specific member', type=str)
 @click.option('--delimiter', help='The column delimiter', default='\t')
 @click.option('--command', '-c', help='The SQL commands to execute')
 @click.option('-d', '--dbname', help='database name to connect to', type=str)
-@click.pass_obj
 def query(
-    obj: Dict[str, Any],
     cluster_name: str,
     group: Optional[int],
     role: Optional[str],
     member: Optional[str],
     w: bool,
     watch: Optional[int],
     delimiter: str,
@@ -776,15 +790,14 @@
     dbname: Optional[str],
     fmt: str = 'tsv'
 ) -> None:
     """Process ``query`` command of ``patronictl`` utility.
 
     Perform a Postgres query in a Patroni node.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should get members from to perform the query. Refer to the module note for
         more details.
     :param role: filter which members to perform the query against based on their role. See :func:`get_all_members` for
         available options.
     :param member: filter which member to perform the query against based on its name.
     :param w: perform query with watch-based approach every 2 seconds.
@@ -816,32 +829,30 @@
     if username:
         connect_parameters['username'] = username
     if password:
         connect_parameters['password'] = click.prompt('Password', hide_input=True, type=str)
     if dbname:
         connect_parameters['dbname'] = dbname
 
-    dcs = get_dcs(obj, cluster_name, group)
+    dcs = get_dcs(cluster_name, group)
 
     cluster = cursor = None
     for _ in watching(w, watch, clear=False):
         if cluster is None:
             cluster = dcs.get_cluster()
-#            cursor = get_cursor(obj, cluster, group, connect_parameters, role=role, member=member)
 
-        output, header = query_member(obj, cluster, group, cursor, member, role, sql, connect_parameters)
+        output, header = query_member(cluster, group, cursor, member, role, sql, connect_parameters)
         print_output(header, output, fmt=fmt, delimiter=delimiter)
 
 
-def query_member(obj: Dict[str, Any], cluster: Cluster, group: Optional[int],
-                 cursor: Union['cursor', 'Cursor[Any]', None], member: Optional[str], role: Optional[str],
-                 command: str, connect_parameters: Dict[str, Any]) -> Tuple[List[List[Any]], Optional[List[Any]]]:
+def query_member(cluster: Cluster, group: Optional[int], cursor: Union['cursor', 'Cursor[Any]', None],
+                 member: Optional[str], role: Optional[str], command: str,
+                 connect_parameters: Dict[str, Any]) -> Tuple[List[List[Any]], Optional[List[Any]]]:
     """Execute SQL *command* against a member.
 
-    :param obj: Patroni configuration.
     :param cluster: the Patroni cluster.
     :param group: filter which Citus group we should get members from to perform the query. Refer to the module note for
         more details.
     :param cursor: cursor through which *command* is executed. If ``None`` a new cursor is instantiated through
         :func:`get_cursor`.
     :param member: filter which member to create a cursor against based on its name, if *cursor* is ``None``.
     :param role: filter which member to create a cursor against based on their role, if *cursor* is ``None``. See
@@ -862,15 +873,15 @@
           * Error message.
 
         * ``None``.
     """
     from . import psycopg
     try:
         if cursor is None:
-            cursor = get_cursor(obj, cluster, group, connect_parameters, role=role, member_name=member)
+            cursor = get_cursor(cluster, group, connect_parameters, role=role, member_name=member)
 
         if cursor is None:
             if member is not None:
                 message = f'No connection to member {member} is available'
             elif role is not None:
                 message = f'No connection to role {role} is available'
             else:
@@ -889,40 +900,38 @@
         return [[timestamp(0), 'ERROR, SQLSTATE: {0}'.format(message)]], None
 
 
 @ctl.command('remove', help='Remove cluster from DCS')
 @click.argument('cluster_name')
 @option_citus_group
 @option_format
-@click.pass_obj
-def remove(obj: Dict[str, Any], cluster_name: str, group: Optional[int], fmt: str) -> None:
+def remove(cluster_name: str, group: Optional[int], fmt: str) -> None:
     """Process ``remove`` command of ``patronictl`` utility.
 
     Remove cluster *cluster_name* from the DCS.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the cluster which information will be wiped out of the DCS.
     :param group: which Citus group should have its information wiped out of the DCS. Refer to the module note for more
         details.
     :param fmt: the output table printing format. See :func:`print_output` for available options.
 
     :raises:
         :class:`PatroniCtlException`: if:
             * Patroni is running on a Citus cluster, but no *group* was specified; or
             * *cluster_name* does not exist; or
             * user did not type the expected confirmation message when prompted for confirmation; or
             * use did not type the correct leader name when requesting removal of a healthy cluster.
 
     """
-    dcs = get_dcs(obj, cluster_name, group)
+    dcs = get_dcs(cluster_name, group)
     cluster = dcs.get_cluster()
 
-    if obj.get('citus') and group is None:
+    if is_citus_cluster() and group is None:
         raise PatroniCtlException('For Citus clusters the --group must me specified')
-    output_members(obj, cluster, cluster_name, fmt=fmt)
+    output_members(cluster, cluster_name, fmt=fmt)
 
     confirm = click.prompt('Please confirm the cluster name to remove', type=str)
     if confirm != cluster_name:
         raise PatroniCtlException('Cluster names specified do not match')
 
     message = 'Yes I am aware'
     confirm = \
@@ -999,39 +1008,36 @@
 
 @ctl.command('reload', help='Reload cluster member configuration')
 @click.argument('cluster_name')
 @click.argument('member_names', nargs=-1)
 @option_citus_group
 @click.option('--role', '-r', help='Reload only members with this role', type=role_choice, default='any')
 @option_force
-@click.pass_obj
-def reload(obj: Dict[str, Any], cluster_name: str, member_names: List[str],
-           group: Optional[int], force: bool, role: str) -> None:
+def reload(cluster_name: str, member_names: List[str], group: Optional[int], force: bool, role: str) -> None:
     """Process ``reload`` command of ``patronictl`` utility.
 
     Reload configuration of cluster members based on given filters.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param member_names: name of the members which configuration should be reloaded.
     :param group: filter which Citus group we should reload members. Refer to the module note for more details.
     :param force: perform the reload without asking for confirmations.
     :param role: role to filter members. See :func:`get_all_members` for available options.
     """
-    dcs = get_dcs(obj, cluster_name, group)
+    dcs = get_dcs(cluster_name, group)
     cluster = dcs.get_cluster()
 
-    members = get_members(obj, cluster, cluster_name, member_names, role, force, 'reload', group=group)
+    members = get_members(cluster, cluster_name, member_names, role, force, 'reload', group=group)
 
     for member in members:
         r = request_patroni(member, 'post', 'reload')
         if r.status == 200:
             click.echo('No changes to apply on member {0}'.format(member.name))
         elif r.status == 202:
-            config = get_global_config(cluster)
+            config = global_config.from_cluster(cluster)
             click.echo('Reload request received for member {0} and will be processed within {1} seconds'.format(
                 member.name, config.get('loop_wait') or dcs.loop_wait)
             )
         else:
             click.echo('Failed: reload for member {0}, status code={1}, ({2})'.format(
                 member.name, r.status, r.data.decode('utf-8'))
             )
@@ -1046,23 +1052,21 @@
 @click.option('--scheduled', help='Timestamp of a scheduled restart in unambiguous format (e.g. ISO 8601)',
               default=None)
 @click.option('--pg-version', 'version', help='Restart if the PostgreSQL version is less than provided (e.g. 9.5.2)',
               default=None)
 @click.option('--pending', help='Restart if pending', is_flag=True)
 @click.option('--timeout', help='Return error and fail over if necessary when restarting takes longer than this.')
 @option_force
-@click.pass_obj
-def restart(obj: Dict[str, Any], cluster_name: str, group: Optional[int], member_names: List[str],
+def restart(cluster_name: str, group: Optional[int], member_names: List[str],
             force: bool, role: str, p_any: bool, scheduled: Optional[str], version: Optional[str],
             pending: bool, timeout: Optional[str]) -> None:
     """Process ``restart`` command of ``patronictl`` utility.
 
     Restart Postgres on cluster members based on given filters.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should restart members. Refer to the module note for more details.
     :param member_names: name of the members that should be restarted.
     :param force: perform the restart without asking for confirmations.
     :param role: role to filter members. See :func:`get_all_members` for available options.
     :param p_any: restart a single and random member among the ones that match the given filters.
     :param scheduled: timestamp when the restart should be scheduled to occur. If ``now`` restart immediately.
@@ -1072,17 +1076,17 @@
 
     :raises:
         :class:`PatroniCtlException`: if:
             * *scheduled* could not be parsed; or
             * *version* could not be parsed; or
             * a restart is attempted against a cluster that is in maintenance mode.
     """
-    cluster = get_dcs(obj, cluster_name, group).get_cluster()
+    cluster = get_dcs(cluster_name, group).get_cluster()
 
-    members = get_members(obj, cluster, cluster_name, member_names, role, force, 'restart', False, group=group)
+    members = get_members(cluster, cluster_name, member_names, role, force, 'restart', False, group=group)
     if scheduled is None and not force:
         next_hour = (datetime.datetime.now() + datetime.timedelta(hours=1)).strftime('%Y-%m-%dT%H:%M')
         scheduled = click.prompt('When should the restart take place (e.g. ' + next_hour + ') ',
                                  type=str, default='now')
 
     scheduled_at = parse_scheduled(scheduled)
     confirm_members_action(members, force, 'restart', scheduled_at)
@@ -1104,15 +1108,15 @@
             postgres_version_to_int(version)
         except PatroniException as e:
             raise PatroniCtlException(e.value)
 
         content['postgres_version'] = version
 
     if scheduled_at:
-        if get_global_config(cluster).is_paused:
+        if global_config.from_cluster(cluster).is_paused:
             raise PatroniCtlException("Can't schedule restart in the paused state")
         content['schedule'] = scheduled_at.isoformat()
 
     if timeout is not None:
         content['timeout'] = timeout
 
     for member in members:
@@ -1136,33 +1140,30 @@
 
 @ctl.command('reinit', help='Reinitialize cluster member')
 @click.argument('cluster_name')
 @option_citus_group
 @click.argument('member_names', nargs=-1)
 @option_force
 @click.option('--wait', help='Wait until reinitialization completes', is_flag=True)
-@click.pass_obj
-def reinit(obj: Dict[str, Any], cluster_name: str, group: Optional[int],
-           member_names: List[str], force: bool, wait: bool) -> None:
+def reinit(cluster_name: str, group: Optional[int], member_names: List[str], force: bool, wait: bool) -> None:
     """Process ``reinit`` command of ``patronictl`` utility.
 
     Reinitialize cluster members based on given filters.
 
     .. note::
         Only reinitialize replica members, not a leader.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should reinit members. Refer to the module note for more details.
     :param member_names: name of the members that should be reinitialized.
     :param force: perform the restart without asking for confirmations.
     :param wait: wait for the operation to complete.
     """
-    cluster = get_dcs(obj, cluster_name, group).get_cluster()
-    members = get_members(obj, cluster, cluster_name, member_names, 'replica', force, 'reinitialize', group=group)
+    cluster = get_dcs(cluster_name, group).get_cluster()
+    members = get_members(cluster, cluster_name, member_names, 'replica', force, 'reinitialize', group=group)
 
     wait_on_members: List[Member] = []
     for member in members:
         body: Dict[str, bool] = {'force': force}
         while True:
             r = request_patroni(member, 'post', 'reinitialize', body)
             started = check_response(r, member.name, 'reinitialize')
@@ -1185,26 +1186,25 @@
         for member in wait_on_members:
             data = json.loads(request_patroni(member, 'get', 'patroni').data.decode('utf-8'))
             if data.get('state') != 'creating replica':
                 click.echo('Reinitialize is completed on: {0}'.format(member.name))
                 wait_on_members.remove(member)
 
 
-def _do_failover_or_switchover(obj: Dict[str, Any], action: str, cluster_name: str,
-                               group: Optional[int], switchover_leader: Optional[str], candidate: Optional[str],
+def _do_failover_or_switchover(action: str, cluster_name: str, group: Optional[int],
+                               switchover_leader: Optional[str], candidate: Optional[str],
                                force: bool, scheduled: Optional[str] = None) -> None:
     """Perform a failover or a switchover operation in the cluster.
 
     Informational messages are printed in the console during the operation, as well as the list of members before and
     after the operation, so the user can follow the operation status.
 
     .. note::
         If not able to perform the operation through the REST API, write directly to the DCS as a fall back.
 
-    :param obj: Patroni configuration.
     :param action: action to be taken -- ``failover`` or ``switchover``.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter Citus group within we should perform a failover or switchover. If ``None``, user will be
         prompted for filling it -- unless *force* is ``True``, in which case an exception is raised.
     :param switchover_leader: name of the leader member passed as switchover option.
     :param candidate: name of a standby member to be promoted. Nodes that are tagged with ``nofailover`` cannot be used.
     :param force: perform the failover or switchover without asking for confirmations.
@@ -1219,40 +1219,40 @@
             * no *candidate* is given for a failover operation; or
             * current leader and *candidate* are the same; or
             * *candidate* is tagged as nofailover; or
             * *candidate* is not a member of the cluster; or
             * trying to schedule a switchover in a cluster that is in maintenance mode; or
             * user aborts the operation.
     """
-    dcs = get_dcs(obj, cluster_name, group)
+    dcs = get_dcs(cluster_name, group)
     cluster = dcs.get_cluster()
     click.echo('Current cluster topology')
-    output_members(obj, cluster, cluster_name, group=group)
+    output_members(cluster, cluster_name, group=group)
 
-    if obj.get('citus') and group is None:
+    if is_citus_cluster() and group is None:
         if force:
             raise PatroniCtlException('For Citus clusters the --group must me specified')
         else:
             group = click.prompt('Citus group', type=int)
-            dcs = get_dcs(obj, cluster_name, group)
+            dcs = get_dcs(cluster_name, group)
             cluster = dcs.get_cluster()
 
-    global_config = get_global_config(cluster)
+    config = global_config.from_cluster(cluster)
 
     cluster_leader = cluster.leader and cluster.leader.name
     # leader has to be be defined for switchover only
     if action == 'switchover':
         if not cluster_leader:
             raise PatroniCtlException('This cluster has no leader')
 
         if switchover_leader is None:
             if force:
                 switchover_leader = cluster_leader
             else:
-                prompt = 'Standby Leader' if global_config.is_standby_cluster else 'Primary'
+                prompt = 'Standby Leader' if config.is_standby_cluster else 'Primary'
                 switchover_leader = click.prompt(prompt, type=str, default=cluster_leader)
 
         if cluster_leader != switchover_leader:
             raise PatroniCtlException(f'Member {switchover_leader} is not the leader of cluster {cluster_name}')
 
     # excluding members with nofailover tag
     candidate_names = [str(m.name) for m in cluster.members if m.name != cluster_leader and not m.nofailover]
@@ -1273,15 +1273,15 @@
             raise PatroniCtlException(
                 f'Member {candidate} is already the leader of cluster {cluster_name}')
         raise PatroniCtlException(
             f'Member {candidate} does not exist in cluster {cluster_name} or is tagged as nofailover')
 
     if all((not force,
             action == 'failover',
-            global_config.is_synchronous_mode,
+            config.is_synchronous_mode,
             not cluster.sync.is_empty,
             not cluster.sync.matches(candidate, True))):
         if not click.confirm(f'Are you sure you want to failover to the asynchronous node {candidate}?'):
             raise PatroniCtlException('Aborting ' + action)
 
     scheduled_at_str = None
     scheduled_at = None
@@ -1290,15 +1290,15 @@
         if scheduled is None and not force:
             next_hour = (datetime.datetime.now() + datetime.timedelta(hours=1)).strftime('%Y-%m-%dT%H:%M')
             scheduled = click.prompt('When should the switchover take place (e.g. ' + next_hour + ' ) ',
                                      type=str, default='now')
 
         scheduled_at = parse_scheduled(scheduled)
         if scheduled_at:
-            if global_config.is_paused:
+            if config.is_paused:
                 raise PatroniCtlException("Can't schedule switchover in the paused state")
             scheduled_at_str = scheduled_at.isoformat()
 
     failover_value = {'candidate': candidate}
     if action == 'switchover':
         failover_value['leader'] = switchover_leader
     if scheduled_at_str:
@@ -1340,85 +1340,81 @@
             return
     except Exception:
         logging.exception(r)
         logging.warning('Failing over to DCS')
         click.echo('{0} Could not {1} using Patroni api, falling back to DCS'.format(timestamp(), action))
         dcs.manual_failover(switchover_leader, candidate, scheduled_at=scheduled_at)
 
-    output_members(obj, cluster, cluster_name, group=group)
+    output_members(cluster, cluster_name, group=group)
 
 
 @ctl.command('failover', help='Failover to a replica')
 @arg_cluster_name
 @option_citus_group
 @click.option('--leader', '--primary', '--master', 'leader', help='The name of the current leader', default=None)
 @click.option('--candidate', help='The name of the candidate', default=None)
 @option_force
-@click.pass_obj
-def failover(obj: Dict[str, Any], cluster_name: str, group: Optional[int],
+def failover(cluster_name: str, group: Optional[int],
              leader: Optional[str], candidate: Optional[str], force: bool) -> None:
     """Process ``failover`` command of ``patronictl`` utility.
 
     Perform a failover operation immediately in the cluster.
 
     .. note::
         If *leader* is given perform a switchover instead of a failover.
         This behavior is deprecated. ``--leader`` option support will be
         removed in the next major release.
 
     .. seealso::
         Refer to :func:`_do_failover_or_switchover` for details.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter Citus group within we should perform a failover or switchover. If ``None``, user will be
         prompted for filling it -- unless *force* is ``True``, in which case an exception is raised by
         :func:`_do_failover_or_switchover`.
     :param leader: name of the current leader member.
     :param candidate: name of a standby member to be promoted. Nodes that are tagged with ``nofailover`` cannot be used.
     :param force: perform the failover or switchover without asking for confirmations.
     """
     action = 'failover'
     if leader:
         action = 'switchover'
         click.echo(click.style(
             'Supplying a leader name using this command is deprecated and will be removed in a future version of'
             ' Patroni, change your scripts to use `switchover` instead.\nExecuting switchover!', fg='red'))
-    _do_failover_or_switchover(obj, action, cluster_name, group, leader, candidate, force)
+    _do_failover_or_switchover(action, cluster_name, group, leader, candidate, force)
 
 
 @ctl.command('switchover', help='Switchover to a replica')
 @arg_cluster_name
 @option_citus_group
 @click.option('--leader', '--primary', '--master', 'leader', help='The name of the current leader', default=None)
 @click.option('--candidate', help='The name of the candidate', default=None)
 @click.option('--scheduled', help='Timestamp of a scheduled switchover in unambiguous format (e.g. ISO 8601)',
               default=None)
 @option_force
-@click.pass_obj
-def switchover(obj: Dict[str, Any], cluster_name: str, group: Optional[int],
-               leader: Optional[str], candidate: Optional[str], force: bool, scheduled: Optional[str]) -> None:
+def switchover(cluster_name: str, group: Optional[int], leader: Optional[str],
+               candidate: Optional[str], force: bool, scheduled: Optional[str]) -> None:
     """Process ``switchover`` command of ``patronictl`` utility.
 
     Perform a switchover operation in the cluster.
 
     .. seealso::
         Refer to :func:`_do_failover_or_switchover` for details.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter Citus group within we should perform a switchover. If ``None``, user will be prompted for
         filling it -- unless *force* is ``True``, in which case an exception is raised by
         :func:`_do_failover_or_switchover`.
     :param leader: name of the current leader member.
     :param candidate: name of a standby member to be promoted. Nodes that are tagged with ``nofailover`` cannot be used.
     :param force: perform the switchover without asking for confirmations.
     :param scheduled: timestamp when the switchover should be scheduled to occur. If ``now`` perform immediately.
     """
-    _do_failover_or_switchover(obj, 'switchover', cluster_name, group, leader, candidate, force, scheduled)
+    _do_failover_or_switchover('switchover', cluster_name, group, leader, candidate, force, scheduled)
 
 
 def generate_topology(level: int, member: Dict[str, Any],
                       topology: Dict[Optional[str], List[Dict[str, Any]]]) -> Iterator[Dict[str, Any]]:
     """Recursively yield members with their names adjusted according to their *level* in the cluster topology.
 
     .. note::
@@ -1512,16 +1508,16 @@
         for name in ('from', 'to'):
             if name in cluster['scheduled_switchover']:
                 info += '\n{0:>24}: {1}'.format(name, cluster['scheduled_switchover'][name])
         service_info.append(info)
     return service_info
 
 
-def output_members(obj: Dict[str, Any], cluster: Cluster, name: str,
-                   extended: bool = False, fmt: str = 'pretty', group: Optional[int] = None) -> None:
+def output_members(cluster: Cluster, name: str, extended: bool = False,
+                   fmt: str = 'pretty', group: Optional[int] = None) -> None:
     """Print information about the Patroni cluster and its members.
 
     Information is printed to console through :func:`print_output`, and contains:
 
         * ``Cluster``: name of the Patroni cluster, as per ``scope`` configuration;
         * ``Member``: name of the Patroni node, as per ``name`` configuration;
         * ``Host``: hostname (or IP) and port, as per ``postgresql.listen`` configuration;
@@ -1538,15 +1534,14 @@
         * ``Pending restart``: if the node is pending a restart -- showed only if *extended*;
         * ``Scheduled restart``: timestamp for scheduled restart, if any -- showed only if *extended*;
         * ``Tags``: node tags, if any -- showed only if *extended*.
 
     The 3 extended columns are always included if *extended*, even if the member has no value for a given column.
     If not *extended*, these columns may still be shown if any of the members has any information for them.
 
-    :param obj: Patroni configuration.
     :param cluster: Patroni cluster.
     :param name: name of the Patroni cluster.
     :param extended: if extended information (pending restarts, scheduled restarts, node tags) should be printed, if
         available.
     :param fmt: the output table printing format. See :func:`print_output` for available options. If *fmt* is neither
         ``topology`` nor ``pretty``, then complementary information gathered through :func:`get_cluster_service_info` is
         not printed.
@@ -1556,113 +1551,121 @@
     logging.debug(cluster)
 
     initialize = {None: 'uninitialized', '': 'initializing'}.get(cluster.initialize, cluster.initialize)
     columns = ['Cluster', 'Member', 'Host', 'Role', 'State', 'TL', 'Lag in MB']
 
     clusters = {group or 0: cluster_as_json(cluster)}
 
-    is_citus_cluster = obj.get('citus')
-    if is_citus_cluster:
+    if is_citus_cluster():
         columns.insert(1, 'Group')
         if group is None:
             clusters.update({g: cluster_as_json(c) for g, c in cluster.workers.items()})
 
     all_members = [m for c in clusters.values() for m in c['members'] if 'host' in m]
 
-    for c in ('Pending restart', 'Scheduled restart', 'Tags'):
+    for c in ('Pending restart', 'Pending restart reason', 'Scheduled restart', 'Tags'):
         if extended or any(m.get(c.lower().replace(' ', '_')) for m in all_members):
             columns.append(c)
 
     # Show Host as 'host:port' if somebody is running on non-standard port or two nodes are running on the same host
     append_port = any('port' in m and m['port'] != 5432 for m in all_members) or\
         len(set(m['host'] for m in all_members)) < len(all_members)
 
     sort = topology_sort if fmt == 'topology' else iter
     for g, c in sorted(clusters.items()):
         for member in sort(c['members']):
             logging.debug(member)
 
             lag = member.get('lag', '')
+
+            def format_diff(param: str, values: Dict[str, str], hide_long: bool):
+                full_diff = param + ': ' + values['old_value'] + '->' + values['new_value']
+                return full_diff if not hide_long or len(full_diff) <= 50 else param + ': [hidden - too long]'
+            restart_reason = '\n'.join([format_diff(k, v, fmt in ('pretty', 'topology'))
+                                        for k, v in member.get('pending_restart_reason', {}).items()]) or ''
+
             member.update(cluster=name, member=member['name'], group=g,
                           host=member.get('host', ''), tl=member.get('timeline', ''),
                           role=member['role'].replace('_', ' ').title(),
                           lag_in_mb=round(lag / 1024 / 1024) if isinstance(lag, int) else lag,
-                          pending_restart='*' if member.get('pending_restart') else '')
+                          pending_restart='*' if member.get('pending_restart') else '',
+                          pending_restart_reason=restart_reason)
 
             if append_port and member['host'] and member.get('port'):
                 member['host'] = ':'.join([member['host'], str(member['port'])])
 
             if 'scheduled_restart' in member:
                 value = member['scheduled_restart']['schedule']
                 if 'postgres_version' in member['scheduled_restart']:
                     value += ' if version < {0}'.format(member['scheduled_restart']['postgres_version'])
                 member['scheduled_restart'] = value
 
             rows.append([member.get(n.lower().replace(' ', '_'), '') for n in columns])
 
-    title = 'Citus cluster' if is_citus_cluster else 'Cluster'
-    title_details = f' ({initialize})'
-    if is_citus_cluster:
+    if is_citus_cluster():
+        title = 'Citus cluster'
         title_details = '' if group is None else f' (group: {group}, {initialize})'
+    else:
+        title = 'Cluster'
+        title_details = f' ({initialize})'
 
     title = f' {title}: {name}{title_details} '
     print_output(columns, rows, {'Group': 'r', 'Lag in MB': 'r', 'TL': 'r'}, fmt, title)
 
     if fmt not in ('pretty', 'topology'):  # Omit service info when using machine-readable formats
         return
 
     for g, c in sorted(clusters.items()):
         service_info = get_cluster_service_info(c)
         if service_info:
-            if is_citus_cluster and group is None:
+            if is_citus_cluster() and group is None:
                 click.echo('Citus group: {0}'.format(g))
             click.echo(' ' + '\n '.join(service_info))
 
 
 @ctl.command('list', help='List the Patroni members for a given Patroni')
 @click.argument('cluster_names', nargs=-1)
 @option_citus_group
 @click.option('--extended', '-e', help='Show some extra information', is_flag=True)
 @click.option('--timestamp', '-t', 'ts', help='Print timestamp', is_flag=True)
 @option_format
 @option_watch
 @option_watchrefresh
-@click.pass_obj
-def members(obj: Dict[str, Any], cluster_names: List[str], group: Optional[int],
-            fmt: str, watch: Optional[int], w: bool, extended: bool, ts: bool) -> None:
+def members(cluster_names: List[str], group: Optional[int], fmt: str,
+            watch: Optional[int], w: bool, extended: bool, ts: bool) -> None:
     """Process ``list`` command of ``patronictl`` utility.
 
     Print information about the Patroni cluster through :func:`output_members`.
 
-    :param obj: Patroni configuration.
     :param cluster_names: name of clusters that should be printed. If ``None`` consider only the cluster present in
-        ``scope`` key of *obj*.
+        ``scope`` key of the configuration.
     :param group: filter which Citus group we should get members from. Refer to the module note for more details.
     :param fmt: the output table printing format. See :func:`print_output` for available options.
     :param watch: if given print output every *watch* seconds.
     :param w: if ``True`` print output every 2 seconds.
     :param extended: if extended information should be printed. See ``extended`` argument of :func:`output_members` for
         more details.
     :param ts: if timestamp should be included in the output.
     """
+    config = _get_configuration()
     if not cluster_names:
-        if 'scope' in obj:
-            cluster_names = [obj['scope']]
+        if 'scope' in config:
+            cluster_names = [config['scope']]
         if not cluster_names:
             return logging.warning('Listing members: No cluster names were provided')
 
     for _ in watching(w, watch):
         if ts:
             click.echo(timestamp(0))
 
         for cluster_name in cluster_names:
-            dcs = get_dcs(obj, cluster_name, group)
+            dcs = get_dcs(cluster_name, group)
 
             cluster = dcs.get_cluster()
-            output_members(obj, cluster, cluster_name, extended, fmt, group)
+            output_members(cluster, cluster_name, extended, fmt, group)
 
 
 @ctl.command('topology', help='Prints ASCII topology for given cluster')
 @click.argument('cluster_names', nargs=-1)
 @option_citus_group
 @option_watch
 @option_watchrefresh
@@ -1696,34 +1699,32 @@
 @ctl.command('flush', help='Discard scheduled events')
 @click.argument('cluster_name')
 @option_citus_group
 @click.argument('member_names', nargs=-1)
 @click.argument('target', type=click.Choice(['restart', 'switchover']))
 @click.option('--role', '-r', help='Flush only members with this role', type=role_choice, default='any')
 @option_force
-@click.pass_obj
-def flush(obj: Dict[str, Any], cluster_name: str, group: Optional[int],
+def flush(cluster_name: str, group: Optional[int],
           member_names: List[str], force: bool, role: str, target: str) -> None:
     """Process ``flush`` command of ``patronictl`` utility.
 
     Discard scheduled restart or switchover events.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should flush an event. Refer to the module note for more details.
     :param member_names: name of the members which events should be flushed.
     :param force: perform the operation without asking for confirmations.
     :param role: role to filter members. See :func:`get_all_members` for available options.
     :param target: the event that should be flushed -- ``restart`` or ``switchover``.
     """
-    dcs = get_dcs(obj, cluster_name, group)
+    dcs = get_dcs(cluster_name, group)
     cluster = dcs.get_cluster()
 
     if target == 'restart':
-        for member in get_members(obj, cluster, cluster_name, member_names, role, force, 'flush', group=group):
+        for member in get_members(cluster, cluster_name, member_names, role, force, 'flush', group=group):
             if member.data.get('scheduled_restart'):
                 r = request_patroni(member, 'delete', 'restart')
                 check_response(r, member.name, 'flush scheduled restart')
             else:
                 click.echo('No scheduled restart for member {0}'.format(member.name))
     elif target == 'switchover':
         failover = cluster.failover
@@ -1751,15 +1752,15 @@
     """Wait for all members in the cluster to have ``pause`` state set to *paused*.
 
     :param dcs: DCS object from where to get fresh cluster information.
     :param paused: the desired state for ``pause`` in all nodes.
     :param old_cluster: original cluster information before pause or unpause has been requested. Used to report which
         nodes are still pending to have ``pause`` equal *paused* at a given point in time.
     """
-    config = get_global_config(old_cluster)
+    config = global_config.from_cluster(old_cluster)
 
     click.echo("'{0}' request sent, waiting until it is recognized by all nodes".format(paused and 'pause' or 'resume'))
     old = {m.name: m.version for m in old_cluster.members if m.api_url}
     loop_wait = config.get('loop_wait') or dcs.loop_wait
 
     cluster = None
     for _ in polling_loop(loop_wait + 1):
@@ -1773,32 +1774,31 @@
                      and m.name in old and old[m.name] != m.version]
         if remaining:
             return click.echo("{0} members didn't recognized pause state after {1} seconds"
                               .format(', '.join(remaining), loop_wait))
     return click.echo('Success: cluster management is {0}'.format(paused and 'paused' or 'resumed'))
 
 
-def toggle_pause(config: Dict[str, Any], cluster_name: str, group: Optional[int], paused: bool, wait: bool) -> None:
+def toggle_pause(cluster_name: str, group: Optional[int], paused: bool, wait: bool) -> None:
     """Toggle the ``pause`` state in the cluster members.
 
-    :param config: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should toggle the pause state of. Refer to the module note for more
         details.
     :param paused: the desired state for ``pause`` in all nodes.
     :param wait: ``True`` if it should block until the operation is finished or ``false`` for returning immediately.
 
     :raises:
         PatroniCtlException: if
             * ``pause`` state is already *paused*; or
             * cluster contains no accessible members.
     """
-    dcs = get_dcs(config, cluster_name, group)
+    dcs = get_dcs(cluster_name, group)
     cluster = dcs.get_cluster()
-    if get_global_config(cluster).is_paused == paused:
+    if global_config.from_cluster(cluster).is_paused == paused:
         raise PatroniCtlException('Cluster is {0} paused'.format(paused and 'already' or 'not'))
 
     for member in get_all_members_leader_first(cluster):
         try:
             r = request_patroni(member, 'patch', 'config', {'pause': paused or None})
         except Exception as err:
             logging.warning(str(err))
@@ -1817,45 +1817,41 @@
     else:
         raise PatroniCtlException('Can not find accessible cluster member')
 
 
 @ctl.command('pause', help='Disable auto failover')
 @arg_cluster_name
 @option_default_citus_group
-@click.pass_obj
 @click.option('--wait', help='Wait until pause is applied on all nodes', is_flag=True)
-def pause(obj: Dict[str, Any], cluster_name: str, group: Optional[int], wait: bool) -> None:
+def pause(cluster_name: str, group: Optional[int], wait: bool) -> None:
     """Process ``pause`` command of ``patronictl`` utility.
 
     Put the cluster in maintenance mode.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should pause. Refer to the module note for more details.
     :param wait: ``True`` if it should block until the operation is finished or ``false`` for returning immediately.
     """
-    return toggle_pause(obj, cluster_name, group, True, wait)
+    return toggle_pause(cluster_name, group, True, wait)
 
 
 @ctl.command('resume', help='Resume auto failover')
 @arg_cluster_name
 @option_default_citus_group
 @click.option('--wait', help='Wait until pause is cleared on all nodes', is_flag=True)
-@click.pass_obj
-def resume(obj: Dict[str, Any], cluster_name: str, group: Optional[int], wait: bool) -> None:
+def resume(cluster_name: str, group: Optional[int], wait: bool) -> None:
     """Process ``unpause`` command of ``patronictl`` utility.
 
     Put the cluster out of maintenance mode.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should unpause. Refer to the module note for more details.
     :param wait: ``True`` if it should block until the operation is finished or ``false`` for returning immediately.
     """
-    return toggle_pause(obj, cluster_name, group, False, wait)
+    return toggle_pause(cluster_name, group, False, wait)
 
 
 @contextmanager
 def temporary_file(contents: bytes, suffix: str = '', prefix: str = 'tmp') -> Iterator[str]:
     """Create a temporary file with specified contents that persists for the context.
 
     :param contents: binary string that will be written to the file.
@@ -2079,23 +2075,20 @@
 @click.option('--pg', '-p', 'pgkvpairs', multiple=True,
               help='Set specific PostgreSQL parameter value. Shorthand for -s postgresql.parameters. '
                    'Can be specified multiple times')
 @click.option('--apply', 'apply_filename', help='Apply configuration from file. Use - for stdin.')
 @click.option('--replace', 'replace_filename', help='Apply configuration from file, replacing existing configuration.'
               ' Use - for stdin.')
 @option_force
-@click.pass_obj
-def edit_config(obj: Dict[str, Any], cluster_name: str, group: Optional[int],
-                force: bool, quiet: bool, kvpairs: List[str], pgkvpairs: List[str],
-                apply_filename: Optional[str], replace_filename: Optional[str]) -> None:
+def edit_config(cluster_name: str, group: Optional[int], force: bool, quiet: bool, kvpairs: List[str],
+                pgkvpairs: List[str], apply_filename: Optional[str], replace_filename: Optional[str]) -> None:
     """Process ``edit-config`` command of ``patronictl`` utility.
 
     Update or replace Patroni configuration in the DCS.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group configuration we should edit. Refer to the module note for more details.
     :param force: if ``True`` apply config changes without asking for confirmations.
     :param quiet: if ``True`` skip showing config diff in the console.
     :param kvpairs: list of key value general parameters to be changed.
     :param pgkvpairs: list of key value Postgres parameters to be changed.
     :param apply_filename: name of the file which contains with new configuration parameters to be applied. Pass ``-``
@@ -2104,15 +2097,15 @@
         configuration. Pass ``-`` for using stdin instead.
 
     :raises:
         :class:`PatroniCtlException`: if
             * Configuration is absent from DCS; or
             * Detected a concurrent modification of the configuration in the DCS.
     """
-    dcs = get_dcs(obj, cluster_name, group)
+    dcs = get_dcs(cluster_name, group)
     cluster = dcs.get_cluster()
 
     if not cluster.config:
         raise PatroniCtlException('The config key does not exist in the cluster {0}'.format(cluster_name))
 
     before_editing = format_config_for_editing(cluster.config.data)
 
@@ -2142,63 +2135,59 @@
         show_diff(before_editing, after_editing)
 
     if (apply_filename == '-' or replace_filename == '-') and not force:
         click.echo("Use --force option to apply changes")
         return
 
     if force or click.confirm('Apply these changes?'):
-        if not dcs.set_config_value(json.dumps(changed_data), cluster.config.version):
+        if not dcs.set_config_value(json.dumps(changed_data, separators=(',', ':')), cluster.config.version):
             raise PatroniCtlException("Config modification aborted due to concurrent changes")
         click.echo("Configuration changed")
 
 
 @ctl.command('show-config', help="Show cluster configuration")
 @arg_cluster_name
 @option_default_citus_group
-@click.pass_obj
-def show_config(obj: Dict[str, Any], cluster_name: str, group: Optional[int]) -> None:
+def show_config(cluster_name: str, group: Optional[int]) -> None:
     """Process ``show-config`` command of ``patronictl`` utility.
 
     Show Patroni configuration stored in the DCS.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group configuration we should show. Refer to the module note for more details.
     """
-    cluster = get_dcs(obj, cluster_name, group).get_cluster()
+    cluster = get_dcs(cluster_name, group).get_cluster()
     if cluster.config:
         click.echo(format_config_for_editing(cluster.config.data))
 
 
 @ctl.command('version', help='Output version of patronictl command or a running Patroni instance')
 @click.argument('cluster_name', required=False)
 @click.argument('member_names', nargs=-1)
 @option_citus_group
-@click.pass_obj
-def version(obj: Dict[str, Any], cluster_name: str, group: Optional[int], member_names: List[str]) -> None:
+def version(cluster_name: str, group: Optional[int], member_names: List[str]) -> None:
     """Process ``version`` command of ``patronictl`` utility.
 
     Show version of:
         * ``patronictl`` on invoker;
         * ``patroni`` on all members of the cluster;
         * ``PostgreSQL`` on all members of the cluster.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should get members from. Refer to the module note for more details.
     :param member_names: filter which members we should get version information from.
     """
     click.echo("patronictl version {0}".format(__version__))
 
     if not cluster_name:
         return
 
     click.echo("")
-    cluster = get_dcs(obj, cluster_name, group).get_cluster()
-    for m in get_all_members(obj, cluster, group, 'any'):
+    cluster = get_dcs(cluster_name, group).get_cluster()
+    for m in get_all_members(cluster, group, 'any'):
         if m.api_url:
             if not member_names or m.name in member_names:
                 try:
                     response = request_patroni(m)
                     data = json.loads(response.data.decode('utf-8'))
                     version = data.get('patroni', {}).get('version')
                     pg_version = data.get('server_version')
@@ -2208,33 +2197,31 @@
                     click.echo("{0}: failed to get version: {1}".format(m.name, e))
 
 
 @ctl.command('history', help="Show the history of failovers/switchovers")
 @arg_cluster_name
 @option_default_citus_group
 @option_format
-@click.pass_obj
-def history(obj: Dict[str, Any], cluster_name: str, group: Optional[int], fmt: str) -> None:
+def history(cluster_name: str, group: Optional[int], fmt: str) -> None:
     """Process ``history`` command of ``patronictl`` utility.
 
     Show the history of failover/switchover events in the cluster.
 
     Information is printed to console through :func:`print_output`, and contains:
         * ``TL``: Postgres timeline when the event occurred;
         * ``LSN``: Postgres LSN, in bytes, when the event occurred;
         * ``Reason``: the reason that motivated the event, if any;
         * ``Timestamp``: timestamp when the event occurred;
         * ``New Leader``: the Postgres node that was promoted during the event.
 
-    :param obj: Patroni configuration.
     :param cluster_name: name of the Patroni cluster.
     :param group: filter which Citus group we should get events from. Refer to the module note for more details.
     :param fmt: the output table printing format. See :func:`print_output` for available options.
     """
-    cluster = get_dcs(obj, cluster_name, group).get_cluster()
+    cluster = get_dcs(cluster_name, group).get_cluster()
     cluster_history = cluster.history.lines if cluster.history else []
     history: List[List[Any]] = list(map(list, cluster_history))
     table_header_row = ['TL', 'LSN', 'Reason', 'Timestamp', 'New Leader']
     for line in history:
         if len(line) < len(table_header_row):
             add_column_num = len(table_header_row) - len(line)
             for _ in range(add_column_num):
```

### Comparing `patroni-3.2.2/patroni/daemon.py` & `patroni-3.3.0/patroni/daemon.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/dcs/__init__.py` & `patroni-3.3.0/patroni/dcs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 """Abstract classes for Distributed Configuration Store."""
 import abc
 import datetime
-import importlib
-import inspect
 import json
 import logging
-import os
-import pkgutil
 import re
-import sys
 import time
 from collections import defaultdict
 from copy import deepcopy
 from random import randint
 from threading import Event, Lock
-from types import ModuleType
-from typing import Any, Callable, Collection, Dict, List, NamedTuple, Optional, Set, Tuple, Union, TYPE_CHECKING, \
-    Type, Iterator
+from typing import Any, Callable, Collection, Dict, Iterator, List, \
+    NamedTuple, Optional, Tuple, Type, TYPE_CHECKING, Union
 from urllib.parse import urlparse, urlunparse, parse_qsl
 
 import dateutil.parser
 
+from .. import global_config
+from ..dynamic_loader import iter_classes, iter_modules
 from ..exceptions import PatroniFatalException
 from ..utils import deep_compare, uri
 from ..tags import Tags
 from ..utils import parse_int
 
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
+    from ..postgresql import Postgresql
+    from ..postgresql.mpp import AbstractMPP
 
 SLOT_ADVANCE_AVAILABLE_VERSION = 110000
-CITUS_COORDINATOR_GROUP_ID = 0
-citus_group_re = re.compile('^(0|[1-9][0-9]*)$')
 slot_name_re = re.compile('^[a-z0-9_]{1,63}$')
 logger = logging.getLogger(__name__)
 
 
 def slot_name_from_member_name(member_name: str) -> str:
     """Translate member name to valid PostgreSQL slot name.
 
@@ -83,87 +79,44 @@
     api_url = ([v for n, v in parse_qsl(query) if n == 'application_name'] or [None])[0]
     return conn_url, api_url
 
 
 def dcs_modules() -> List[str]:
     """Get names of DCS modules, depending on execution environment.
 
-    .. note::
-        If being packaged with PyInstaller, modules aren't discoverable dynamically by scanning source directory because
-        :class:`importlib.machinery.FrozenImporter` doesn't implement :func:`iter_modules`. But it is still possible to
-        find all potential DCS modules by iterating through ``toc``, which contains list of all "frozen" resources.
-
     :returns: list of known module names with absolute python module path namespace, e.g. ``patroni.dcs.etcd``.
     """
-    dcs_dirname = os.path.dirname(__file__)
-    module_prefix = __package__ + '.'
-
-    if getattr(sys, 'frozen', False):
-        toc: Set[str] = set()
-        # dcs_dirname may contain a dot, which causes pkgutil.iter_importers()
-        # to misinterpret the path as a package name. This can be avoided
-        # altogether by not passing a path at all, because PyInstaller's
-        # FrozenImporter is a singleton and registered as top-level finder.
-        for importer in pkgutil.iter_importers():
-            if hasattr(importer, 'toc'):
-                toc |= getattr(importer, 'toc')
-        return [module for module in toc if module.startswith(module_prefix) and module.count('.') == 2]
-
-    return [module_prefix + name for _, name, is_pkg in pkgutil.iter_modules([dcs_dirname]) if not is_pkg]
+    if TYPE_CHECKING:  # pragma: no cover
+        assert isinstance(__package__, str)
+    return iter_modules(__package__)
 
 
 def iter_dcs_classes(
         config: Optional[Union['Config', Dict[str, Any]]] = None
 ) -> Iterator[Tuple[str, Type['AbstractDCS']]]:
     """Attempt to import DCS modules that are present in the given configuration.
 
     .. note::
             If a module successfully imports we can assume that all its requirements are installed.
 
     :param config: configuration information with possible DCS names as keys. If given, only attempt to import DCS
                    modules defined in the configuration. Else, if ``None``, attempt to import any supported DCS module.
 
-    :yields: a tuple containing the module ``name`` and the imported DCS class object.
+    :returns: an iterator of tuples, each containing the module ``name`` and the imported DCS class object.
     """
-    for mod_name in dcs_modules():
-        name = mod_name.rpartition('.')[2]
-        if config is None or name in config:
-
-            try:
-                module = importlib.import_module(mod_name)
-                dcs_module = find_dcs_class_in_module(module)
-                if dcs_module:
-                    yield name, dcs_module
-
-            except ImportError:
-                logger.log(logging.DEBUG if config is not None else logging.INFO,
-                           'Failed to import %s', mod_name)
-
-
-def find_dcs_class_in_module(module: ModuleType) -> Optional[Type['AbstractDCS']]:
-    """Try to find the implementation of :class:`AbstractDCS` interface in *module* matching the *module* name.
-
-    :param module: Imported DCS module.
-
-    :returns: class with a name matching the name of *module* that implements :class:`AbstractDCS` or ``None`` if not
-              found.
-    """
-    module_name = module.__name__.rpartition('.')[2]
-    return next(
-        (obj for obj_name, obj in module.__dict__.items()
-         if (obj_name.lower() == module_name
-             and inspect.isclass(obj) and issubclass(obj, AbstractDCS))),
-        None)
+    if TYPE_CHECKING:  # pragma: no cover
+        assert isinstance(__package__, str)
+    return iter_classes(__package__, AbstractDCS, config)
 
 
 def get_dcs(config: Union['Config', Dict[str, Any]]) -> 'AbstractDCS':
     """Attempt to load a Distributed Configuration Store from known available implementations.
 
     .. note::
-        Using the list of available DCS classes returned by :func:`iter_dcs_classes` attempt to dynamically
+        Using the list of available DCS classes returned by :func:`iter_classes` attempt to dynamically
         instantiate the class that implements a DCS using the abstract class :class:`AbstractDCS`.
 
         Basic top-level configuration parameters retrieved from *config* are propagated to the DCS specific config
         before being passed to the module DCS class.
 
         If no module is found to satisfy configuration then report and log an error. This will cause Patroni to exit.
 
@@ -176,22 +129,21 @@
     """
     for name, dcs_class in iter_dcs_classes(config):
         # Propagate some parameters from top level of config if defined to the DCS specific config section.
         config[name].update({
             p: config[p] for p in ('namespace', 'name', 'scope', 'loop_wait',
                                    'patronictl', 'ttl', 'retry_timeout')
             if p in config})
-        # From citus section we only need "group" parameter, but will propagate everything just in case.
-        if isinstance(config.get('citus'), dict):
-            config[name].update(config['citus'])
-        return dcs_class(config[name])
-
-    raise PatroniFatalException(
-        f"Can not find suitable configuration of distributed configuration store\n"
-        f"Available implementations: {', '.join(sorted([n for n, _ in iter_dcs_classes()]))}")
+
+        from patroni.postgresql.mpp import get_mpp
+        return dcs_class(config[name], get_mpp(config))
+
+    available_implementations = ', '.join(sorted([n for n, _ in iter_dcs_classes()]))
+    raise PatroniFatalException("Can not find suitable configuration of distributed configuration store\n"
+                                f"Available implementations: {available_implementations}")
 
 
 _Version = Union[int, str]
 _Session = Union[int, float, str, None]
 
 
 class Member(Tags, NamedTuple('Member',
@@ -586,32 +538,14 @@
             data = json.loads(value)
             assert isinstance(data, dict)
         except (AssertionError, TypeError, ValueError):
             data: Dict[str, Any] = {}
             modify_version = 0
         return ClusterConfig(version, data, version if modify_version is None else modify_version)
 
-    @property
-    def permanent_slots(self) -> Dict[str, Any]:
-        """Dictionary of permanent slots information looked up from :attr:`~ClusterConfig.data`."""
-        return (self.data.get('permanent_replication_slots')
-                or self.data.get('permanent_slots')
-                or self.data.get('slots')
-                or {})
-
-    @property
-    def ignore_slots_matchers(self) -> List[Dict[str, Any]]:
-        """The value for ``ignore_slots`` from :attr:`~ClusterConfig.data` if defined or an empty list."""
-        return self.data.get('ignore_slots') or []
-
-    @property
-    def max_timelines_history(self) -> int:
-        """The value for ``max_timelines_history`` from :attr:`~ClusterConfig.data` if defined or ``0``."""
-        return self.data.get('max_timelines_history', 0)
-
 
 class SyncState(NamedTuple):
     """Immutable object (namedtuple) which represents last observed synchronous replication state.
 
     :ivar version: modification version of a synchronization key in a Configuration Store.
     :ivar leader: reference to member that was leader.
     :ivar sync_standby: synchronous standby list (comma delimited) which are last synchronized to leader.
@@ -622,15 +556,15 @@
     sync_standby: Optional[str]
 
     @staticmethod
     def from_node(version: Optional[_Version], value: Union[str, Dict[str, Any], None]) -> 'SyncState':
         """Factory method to parse *value* as synchronisation state information.
 
         :param version: optional *version* number for the object.
-        :param value: (optionally JSON serialised) sychronisation state information
+        :param value: (optionally JSON serialised) synchronisation state information
 
         :returns: constructed :class:`SyncState` object.
 
         :Example:
 
             >>> SyncState.from_node(1, None).leader is None
             True
@@ -848,15 +782,15 @@
                           ('status', Status),
                           ('members', List[Member]),
                           ('failover', Optional[Failover]),
                           ('sync', SyncState),
                           ('history', Optional[TimelineHistory]),
                           ('failsafe', Optional[Dict[str, str]]),
                           ('workers', Dict[int, 'Cluster'])])):
-    """Immutable object (namedtuple) which represents PostgreSQL or Citus cluster.
+    """Immutable object (namedtuple) which represents PostgreSQL or MPP cluster.
 
     .. note::
         We are using an old-style attribute declaration here because otherwise it is not possible to override `__new__`
         method. Without it the *workers* by default gets always the same :class:`dict` object that could be mutated.
 
     Consists of the following fields:
 
@@ -865,16 +799,16 @@
     :ivar leader: :class:`Leader` object which represents current leader of the cluster.
     :ivar status: :class:`Status` object which represents the `/status` key.
     :ivar members: list of:class:` Member` objects, all PostgreSQL cluster members including leader
     :ivar failover: reference to :class:`Failover` object.
     :ivar sync: reference to :class:`SyncState` object, last observed synchronous replication state.
     :ivar history: reference to `TimelineHistory` object.
     :ivar failsafe: failsafe topology. Node is allowed to become the leader only if its name is found in this list.
-    :ivar workers: dictionary of workers of the Citus cluster, optional. Each key is an :class:`int` representing
-                   the group, and the corresponding value is a :class:`Cluster` instance.
+    :ivar workers: dictionary of workers of the MPP cluster, optional. Each key representing the group and the
+                   corresponding value is a :class:`Cluster` instance.
     """
 
     def __new__(cls, *args: Any, **kwargs: Any):
         """Make workers argument optional and set it to an empty dict object."""
         if len(args) < len(cls._fields) and 'workers' not in kwargs:
             kwargs['workers'] = {}
         return super(Cluster, cls).__new__(cls, *args, **kwargs)
@@ -992,15 +926,15 @@
         return isinstance(value, dict) \
             and value.get('type', 'logical') == 'logical' \
             and bool(value.get('database') and value.get('plugin'))
 
     @property
     def __permanent_slots(self) -> Dict[str, Union[Dict[str, Any], Any]]:
         """Dictionary of permanent replication slots with their known LSN."""
-        ret: Dict[str, Union[Dict[str, Any], Any]] = deepcopy(self.config.permanent_slots if self.config else {})
+        ret: Dict[str, Union[Dict[str, Any], Any]] = global_config.permanent_slots
 
         members: Dict[str, int] = {slot_name_from_member_name(m.name): m.lsn or 0 for m in self.members}
         slots: Dict[str, int] = {k: parse_int(v) or 0 for k, v in (self.slots or {}).items()}
         for name, value in list(ret.items()):
             if not value:
                 value = ret[name] = {}
             if isinstance(value, dict):
@@ -1021,266 +955,257 @@
         return {name: value for name, value in self.__permanent_slots.items() if self.is_physical_slot(value)}
 
     @property
     def __permanent_logical_slots(self) -> Dict[str, Any]:
         """Dictionary of permanent ``logical`` replication slots."""
         return {name: value for name, value in self.__permanent_slots.items() if self.is_logical_slot(value)}
 
-    @property
-    def use_slots(self) -> bool:
-        """``True`` if cluster is configured to use replication slots."""
-        return bool(self.config and (self.config.data.get('postgresql') or {}).get('use_slots', True))
-
-    def get_replication_slots(self, my_name: str, role: str, nofailover: bool, major_version: int, *,
-                              is_standby_cluster: bool = False, show_error: bool = False) -> Dict[str, Dict[str, Any]]:
+    def get_replication_slots(self, postgresql: 'Postgresql', member: Tags, *,
+                              role: Optional[str] = None, show_error: bool = False) -> Dict[str, Dict[str, Any]]:
         """Lookup configured slot names in the DCS, report issues found and merge with permanent slots.
 
         Will log an error if:
 
             * Any logical slots are disabled, due to version compatibility, and *show_error* is ``True``.
 
-        :param my_name: name of this node.
-        :param role: role of this node.
-        :param nofailover: ``True`` if this node is tagged to not be a failover candidate.
-        :param major_version: postgresql major version.
-        :param is_standby_cluster: ``True`` if it is known that this is a standby cluster. We pass the value from
-                                   the outside because we want to protect from the ``/config`` key removal.
+        :param postgresql: reference to :class:`Postgresql` object.
+        :param member: reference to an object implementing :class:`Tags` interface.
+        :param role: role of the node, if not set will be taken from *postgresql*.
         :param show_error: if ``True`` report error if any disabled logical slots or conflicting slot names are found.
 
         :returns: final dictionary of slot names, after merging with permanent slots and performing sanity checks.
         """
-        slots: Dict[str, Dict[str, str]] = self._get_members_slots(my_name, role)
-        permanent_slots: Dict[str, Any] = self._get_permanent_slots(is_standby_cluster=is_standby_cluster,
-                                                                    role=role, nofailover=nofailover,
-                                                                    major_version=major_version)
+        name = member.name if isinstance(member, Member) else postgresql.name
+        role = role or postgresql.role
+
+        slots: Dict[str, Dict[str, str]] = self._get_members_slots(name, role)
+        permanent_slots: Dict[str, Any] = self._get_permanent_slots(postgresql, member, role)
 
         disabled_permanent_logical_slots: List[str] = self._merge_permanent_slots(
-            slots, permanent_slots, my_name, major_version)
+            slots, permanent_slots, name, postgresql.major_version)
 
         if disabled_permanent_logical_slots and show_error:
             logger.error("Permanent logical replication slots supported by Patroni only starting from PostgreSQL 11. "
                          "Following slots will not be created: %s.", disabled_permanent_logical_slots)
 
         return slots
 
-    def _merge_permanent_slots(self, slots: Dict[str, Dict[str, str]], permanent_slots: Dict[str, Any], my_name: str,
+    def _merge_permanent_slots(self, slots: Dict[str, Dict[str, str]], permanent_slots: Dict[str, Any], name: str,
                                major_version: int) -> List[str]:
         """Merge replication *slots* for members with *permanent_slots*.
 
         Perform validation of configured permanent slot name, skipping invalid names.
 
         Will update *slots* in-line based on ``type`` of slot, ``physical`` or ``logical``, and name of node.
         Type is assumed to be ``physical`` if there are no attributes stored as the slot value.
 
         :param slots: Slot names with existing attributes if known.
-        :param my_name: name of this node.
+        :param name: name of this node.
         :param permanent_slots: dictionary containing slot name key and slot information values.
         :param major_version: postgresql major version.
 
         :returns: List of disabled permanent, logical slot names, if postgresql version < 11.
         """
         disabled_permanent_logical_slots: List[str] = []
 
-        for name, value in permanent_slots.items():
-            if not slot_name_re.match(name):
-                logger.error("Invalid permanent replication slot name '%s'", name)
+        for slot_name, value in permanent_slots.items():
+            if not slot_name_re.match(slot_name):
+                logger.error("Invalid permanent replication slot name '%s'", slot_name)
                 logger.error("Slot name may only contain lower case letters, numbers, and the underscore chars")
                 continue
 
             value = deepcopy(value) if value else {'type': 'physical'}
             if isinstance(value, dict):
                 if 'type' not in value:
                     value['type'] = 'logical' if value.get('database') and value.get('plugin') else 'physical'
 
                 if value['type'] == 'physical':
                     # Don't try to create permanent physical replication slot for yourself
-                    if name != slot_name_from_member_name(my_name):
-                        slots[name] = value
+                    if slot_name != slot_name_from_member_name(name):
+                        slots[slot_name] = value
                     continue
 
                 if self.is_logical_slot(value):
                     if major_version < SLOT_ADVANCE_AVAILABLE_VERSION:
-                        disabled_permanent_logical_slots.append(name)
-                    elif name in slots:
+                        disabled_permanent_logical_slots.append(slot_name)
+                    elif slot_name in slots:
                         logger.error("Permanent logical replication slot {'%s': %s} is conflicting with"
-                                     " physical replication slot for cluster member", name, value)
+                                     " physical replication slot for cluster member", slot_name, value)
                     else:
-                        slots[name] = value
+                        slots[slot_name] = value
                     continue
 
-            logger.error("Bad value for slot '%s' in permanent_slots: %s", name, permanent_slots[name])
+            logger.error("Bad value for slot '%s' in permanent_slots: %s", slot_name, permanent_slots[slot_name])
         return disabled_permanent_logical_slots
 
-    def _get_permanent_slots(self, *, is_standby_cluster: bool, role: str,
-                             nofailover: bool, major_version: int) -> Dict[str, Any]:
+    def _get_permanent_slots(self, postgresql: 'Postgresql', tags: Tags, role: str) -> Dict[str, Any]:
         """Get configured permanent replication slots.
 
         .. note::
             Permanent replication slots are only considered if ``use_slots`` configuration is enabled.
             A node that is not supposed to become a leader (*nofailover*) will not have permanent replication slots.
+            Also node with disabled streaming (*nostream*) and its cascading followers must not have permanent
+            logical slots due to lack of feedback from node to primary, which makes them unsafe to use.
 
             In a standby cluster we only support physical replication slots.
 
             The returned dictionary for a non-standby cluster always contains permanent logical replication slots in
             order to show a warning if they are not supported by PostgreSQL before v11.
 
-        :param is_standby_cluster: ``True`` if it is known that this is a standby cluster. We pass the value from
-                                   the outside because we want to protect from the ``/config`` key removal.
-        :param role: role of this node -- ``primary``, ``standby_leader`` or ``replica``.
-        :param nofailover: ``True`` if this node is tagged to not be a failover candidate.
-        :param major_version: postgresql major version.
+        :param postgresql: reference to :class:`Postgresql` object.
+        :param tags: reference to an object implementing :class:`Tags` interface.
+        :param role: role of the node -- ``primary``, ``standby_leader`` or ``replica``.
 
         :returns: dictionary of permanent slot names mapped to attributes.
         """
-        if not self.use_slots or nofailover:
+        if not global_config.use_slots or tags.nofailover:
             return {}
 
-        if is_standby_cluster:
+        if global_config.is_standby_cluster or self.get_slot_name_on_primary(postgresql.name, tags) is None:
             return self.__permanent_physical_slots \
-                if major_version >= SLOT_ADVANCE_AVAILABLE_VERSION or role == 'standby_leader' else {}
+                if postgresql.major_version >= SLOT_ADVANCE_AVAILABLE_VERSION or role == 'standby_leader' else {}
 
-        return self.__permanent_slots if major_version >= SLOT_ADVANCE_AVAILABLE_VERSION\
+        return self.__permanent_slots if postgresql.major_version >= SLOT_ADVANCE_AVAILABLE_VERSION\
             or role in ('master', 'primary') else self.__permanent_logical_slots
 
-    def _get_members_slots(self, my_name: str, role: str) -> Dict[str, Dict[str, str]]:
+    def _get_members_slots(self, name: str, role: str) -> Dict[str, Dict[str, str]]:
         """Get physical replication slots configuration for members that sourcing from this node.
 
         If the ``replicatefrom`` tag is set on the member - we should not create the replication slot for it on
         the current primary, because that member would replicate from elsewhere. We still create the slot if
         the ``replicatefrom`` destination member is currently not a member of the cluster (fallback to the
         primary), or if ``replicatefrom`` destination member happens to be the current primary.
 
+        If the ``nostream`` tag is set on the member - we should not create the replication slot for it on
+        the current primary or any other member even if ``replicatefrom`` is set, because ``nostream`` disables
+        WAL streaming.
+
         Will log an error if:
 
             * Conflicting slot names between members are found
 
-        :param my_name: name of this node.
+        :param name: name of this node.
         :param role: role of this node, if this is a ``primary`` or ``standby_leader`` return list of members
                      replicating from this node. If not then return a list of members replicating as cascaded
                      replicas from this node.
 
         :returns: dictionary of physical replication slots that should exist on a given node.
         """
-        if not self.use_slots:
+        if not global_config.use_slots:
             return {}
 
-        # we always want to exclude the member with our name from the list
-        members = filter(lambda m: m.name != my_name, self.members)
+        # we always want to exclude the member with our name from the list,
+        # also exlude members with disabled WAL streaming
+        members = filter(lambda m: m.name != name and not m.nostream, self.members)
 
         if role in ('master', 'primary', 'standby_leader'):
             members = [m for m in members if m.replicatefrom is None
-                       or m.replicatefrom == my_name or not self.has_member(m.replicatefrom)]
+                       or m.replicatefrom == name or not self.has_member(m.replicatefrom)]
         else:
             # only manage slots for replicas that replicate from this one, except for the leader among them
-            members = [m for m in members if m.replicatefrom == my_name and m.name != self.leader_name]
+            members = [m for m in members if m.replicatefrom == name and m.name != self.leader_name]
 
         slots = {slot_name_from_member_name(m.name): {'type': 'physical'} for m in members}
         if len(slots) < len(members):
             # Find which names are conflicting for a nicer error message
             slot_conflicts: Dict[str, List[str]] = defaultdict(list)
             for member in members:
                 slot_conflicts[slot_name_from_member_name(member.name)].append(member.name)
             logger.error("Following cluster members share a replication slot name: %s",
                          "; ".join(f"{', '.join(v)} map to {k}"
                                    for k, v in slot_conflicts.items() if len(v) > 1))
         return slots
 
-    def has_permanent_slots(self, my_name: str, *, is_standby_cluster: bool = False, nofailover: bool = False,
-                            major_version: int = SLOT_ADVANCE_AVAILABLE_VERSION) -> bool:
-        """Check if the given member node has permanent replication slots configured.
-
-        :param my_name: name of the member node to check.
-        :param is_standby_cluster: ``True`` if it is known that this is a standby cluster. We pass the value from
-                                   the outside because we want to protect from the ``/config`` key removal.
-        :param nofailover: ``True`` if this node is tagged to not be a failover candidate.
-        :param major_version: postgresql major version.
+    def has_permanent_slots(self, postgresql: 'Postgresql', member: Tags) -> bool:
+        """Check if our node has permanent replication slots configured.
+
+        :param postgresql: reference to :class:`Postgresql` object.
+        :param member: reference to an object implementing :class:`Tags` interface for
+                       the node that we are checking permanent logical replication slots for.
 
         :returns: ``True`` if there are permanent replication slots configured, otherwise ``False``.
         """
         role = 'replica'
-        members_slots: Dict[str, Dict[str, str]] = self._get_members_slots(my_name, role)
-        permanent_slots: Dict[str, Any] = self._get_permanent_slots(is_standby_cluster=is_standby_cluster,
-                                                                    role=role, nofailover=nofailover,
-                                                                    major_version=major_version)
+        members_slots: Dict[str, Dict[str, str]] = self._get_members_slots(postgresql.name, role)
+        permanent_slots: Dict[str, Any] = self._get_permanent_slots(postgresql, member, role)
         slots = deepcopy(members_slots)
-        self._merge_permanent_slots(slots, permanent_slots, my_name, major_version)
+        self._merge_permanent_slots(slots, permanent_slots, postgresql.name, postgresql.major_version)
         return len(slots) > len(members_slots) or any(self.is_physical_slot(v) for v in permanent_slots.values())
 
-    def filter_permanent_slots(self, slots: Dict[str, int], is_standby_cluster: bool,
-                               major_version: int) -> Dict[str, int]:
+    def filter_permanent_slots(self, postgresql: 'Postgresql', slots: Dict[str, int]) -> Dict[str, int]:
         """Filter out all non-permanent slots from provided *slots* dict.
 
-        :param slots: slot names with LSN values
-        :param is_standby_cluster: ``True`` if it is known that this is a standby cluster. We pass the value from
-                                   the outside because we want to protect from the ``/config`` key removal.
-        :param major_version: postgresql major version.
+        :param postgresql: reference to :class:`Postgresql` object.
+        :param slots: slot names with LSN values.
 
         :returns: a :class:`dict` object that contains only slots that are known to be permanent.
         """
-        if major_version < SLOT_ADVANCE_AVAILABLE_VERSION:
+        if postgresql.major_version < SLOT_ADVANCE_AVAILABLE_VERSION:
             return {}  # for legacy PostgreSQL we don't support permanent slots on standby nodes
 
-        permanent_slots: Dict[str, Any] = self._get_permanent_slots(is_standby_cluster=is_standby_cluster,
-                                                                    role='replica',
-                                                                    nofailover=False,
-                                                                    major_version=major_version)
+        permanent_slots: Dict[str, Any] = self._get_permanent_slots(postgresql, RemoteMember('', {}), 'replica')
         members_slots = {slot_name_from_member_name(m.name) for m in self.members}
 
         return {name: value for name, value in slots.items() if name in permanent_slots
                 and (self.is_physical_slot(permanent_slots[name])
                      or self.is_logical_slot(permanent_slots[name]) and name not in members_slots)}
 
-    def _has_permanent_logical_slots(self, my_name: str, nofailover: bool) -> bool:
+    def _has_permanent_logical_slots(self, postgresql: 'Postgresql', member: Tags) -> bool:
         """Check if the given member node has permanent ``logical`` replication slots configured.
 
-        :param my_name: name of the member node to check.
-        :param nofailover: ``True`` if this node is tagged to not be a failover candidate.
+        :param postgresql: reference to a :class:`Postgresql` object.
+        :param member: reference to an object implementing :class:`Tags` interface for
+                       the node that we are checking permanent logical replication slots for.
 
         :returns: ``True`` if any detected replications slots are ``logical``, otherwise ``False``.
         """
-        slots = self.get_replication_slots(my_name, 'replica', nofailover, SLOT_ADVANCE_AVAILABLE_VERSION).values()
+        slots = self.get_replication_slots(postgresql, member, role='replica').values()
         return any(v for v in slots if v.get("type") == "logical")
 
-    def should_enforce_hot_standby_feedback(self, my_name: str, nofailover: bool) -> bool:
+    def should_enforce_hot_standby_feedback(self, postgresql: 'Postgresql', member: Tags) -> bool:
         """Determine whether ``hot_standby_feedback`` should be enabled for the given member.
 
         The ``hot_standby_feedback`` must be enabled if the current replica has ``logical`` slots,
         or it is working as a cascading replica for the other node that has ``logical`` slots.
 
-        :param my_name: name of the member node to check.
-        :param nofailover: ``True`` if this node is tagged to not be a failover candidate.
+        :param postgresql: reference to a :class:`Postgresql` object.
+        :param member: reference to an object implementing :class:`Tags` interface for
+                       the node that we are checking permanent logical replication slots for.
 
         :returns: ``True`` if this node or any member replicating from this node has
                   permanent logical slots, otherwise ``False``.
         """
-        if self._has_permanent_logical_slots(my_name, nofailover):
+        if self._has_permanent_logical_slots(postgresql, member):
             return True
 
-        if self.use_slots:
-            members = [m for m in self.members if m.replicatefrom == my_name and m.name != self.leader_name]
-            return any(self.should_enforce_hot_standby_feedback(m.name, m.nofailover) for m in members)
+        if global_config.use_slots:
+            name = member.name if isinstance(member, Member) else postgresql.name
+            members = [m for m in self.members if m.replicatefrom == name and m.name != self.leader_name]
+            return any(self.should_enforce_hot_standby_feedback(postgresql, m) for m in members)
         return False
 
-    def get_my_slot_name_on_primary(self, my_name: str, replicatefrom: Optional[str]) -> str:
-        """Canonical slot name for physical replication.
+    def get_slot_name_on_primary(self, name: str, tags: Tags) -> Optional[str]:
+        """Get the name of physical replication slot for this node on the primary.
 
         .. note::
             P <-- I <-- L
 
             In case of cascading replication we have to check not our physical slot, but slot of the replica that
             connects us to the primary.
 
-        :param my_name: the member node name that is replicating.
-        :param replicatefrom: the Intermediate member name that is configured to replicate for cascading replication.
+        :param name: name of the member node to check.
+        :param tags: reference to an object implementing :class:`Tags` interface.
 
-        :returns: The slot name that is in use for physical replication on this no`de.
+        :returns: the slot name on the primary that is in use for physical replication on this node.
         """
-        m = self.get_member(replicatefrom, False) if replicatefrom else None
-        return self.get_my_slot_name_on_primary(m.name, m.replicatefrom) \
-            if isinstance(m, Member) else slot_name_from_member_name(my_name)
+        if tags.nostream:
+            return None
+        replicatefrom = self.get_member(tags.replicatefrom, False) if tags.replicatefrom else None
+        return self.get_slot_name_on_primary(replicatefrom.name, replicatefrom) \
+            if isinstance(replicatefrom, Member) else slot_name_from_member_name(name)
 
     @property
     def timeline(self) -> int:
         """Get the cluster history index from the :attr:`~Cluster.history`.
 
         :returns: If the recorded history is empty assume timeline is ``1``, if it is not defined or the stored history
                   is not formatted as expected ``0`` is returned and an error will be logged.
@@ -1347,19 +1272,19 @@
 
     Implementations of a concrete DCS class, using appropriate backend client interfaces, must include the following
     methods and properties.
 
     Functional methods that are critical in their timing, required to complete within ``retry_timeout`` period in order
     to prevent the DCS considered inaccessible, each perform construction of complex data objects:
 
-        * :meth:`~AbstractDCS._cluster_loader`:
+        * :meth:`~AbstractDCS._postgresql_cluster_loader`:
             method which processes the structure of data stored in the DCS used to build the :class:`Cluster` object
             with all relevant associated data.
-        * :meth:`~AbstractDCS._citus_cluster_loader`:
-            Similar to above but specifically representing Citus group and workers information.
+        * :meth:`~AbstractDCS._mpp_cluster_loader`:
+            Similar to above but specifically representing MPP group and workers information.
         * :meth:`~AbstractDCS._load_cluster`:
             main method for calling specific ``loader`` method to build the :class:`Cluster` object representing the
             state and topology of the cluster.
 
     Functional methods that are critical in their timing and must be written with ACID transaction properties in mind:
 
         * :meth:`~AbstractDCS.attempt_to_acquire_leader`:
@@ -1420,45 +1345,50 @@
     _MEMBERS = 'members/'
     _OPTIME = 'optime'
     _STATUS = 'status'  # JSON, contains "leader_lsn" and confirmed_flush_lsn of logical "slots" on the leader
     _LEADER_OPTIME = _OPTIME + '/' + _LEADER  # legacy
     _SYNC = 'sync'
     _FAILSAFE = 'failsafe'
 
-    def __init__(self, config: Dict[str, Any]) -> None:
-        """Prepare DCS paths, Citus group ID, initial values for state information and processing dependencies.
+    def __init__(self, config: Dict[str, Any], mpp: 'AbstractMPP') -> None:
+        """Prepare DCS paths, MPP object, initial values for state information and processing dependencies.
 
         :ivar config: :class:`dict`, reference to config section of selected DCS.
                       i.e.: ``zookeeper`` for zookeeper, ``etcd`` for etcd, etc...
         """
+        self._mpp = mpp
         self._name = config['name']
         self._base_path = re.sub('/+', '/', '/'.join(['', config.get('namespace', 'service'), config['scope']]))
-        self._citus_group = str(config['group']) if isinstance(config.get('group'), int) else None
         self._set_loop_wait(config.get('loop_wait', 10))
 
         self._ctl = bool(config.get('patronictl', False))
         self._cluster: Optional[Cluster] = None
         self._cluster_valid_till: float = 0
         self._cluster_thread_lock = Lock()
         self._last_lsn: int = 0
         self._last_seen: int = 0
         self._last_status: Dict[str, Any] = {}
         self._last_failsafe: Optional[Dict[str, str]] = {}
         self.event = Event()
 
+    @property
+    def mpp(self) -> 'AbstractMPP':
+        """Get the effective underlying MPP, if any has been configured."""
+        return self._mpp
+
     def client_path(self, path: str) -> str:
         """Construct the absolute key name from appropriate parts for the DCS type.
 
         :param path: The key name within the current Patroni cluster.
 
         :returns: absolute key name for the current Patroni cluster.
         """
         components = [self._base_path]
-        if self._citus_group:
-            components.append(self._citus_group)
+        if self._mpp.is_enabled():
+            components.append(str(self._mpp.group))
         components.append(path.lstrip('/'))
         return '/'.join(components)
 
     @property
     def initialize_path(self) -> str:
         """Get the client path for ``initialize``."""
         return self.client_path(self._INITIALIZE)
@@ -1551,111 +1481,112 @@
 
     @property
     def last_seen(self) -> int:
         """The time recorded when the DCS was last reachable."""
         return self._last_seen
 
     @abc.abstractmethod
-    def _cluster_loader(self, path: Any) -> Cluster:
-        """Load and build the :class:`Cluster` object from DCS, which represents a single Patroni or Citus cluster.
+    def _postgresql_cluster_loader(self, path: Any) -> Cluster:
+        """Load and build the :class:`Cluster` object from DCS, which represents a single PostgreSQL cluster.
 
-        :param path: the path in DCS where to load Cluster(s) from.
+        :param path: the path in DCS where to load :class:`Cluster` from.
 
         :returns: :class:`Cluster` instance.
         """
 
     @abc.abstractmethod
-    def _citus_cluster_loader(self, path: Any) -> Dict[int, Cluster]:
-        """Load and build all Patroni clusters from a single Citus cluster.
+    def _mpp_cluster_loader(self, path: Any) -> Dict[int, Cluster]:
+        """Load and build all PostgreSQL clusters from a single MPP cluster.
 
         :param path: the path in DCS where to load Cluster(s) from.
 
-        :returns: all Citus groups as :class:`dict`, with group IDs as keys and :class:`Cluster` objects as values or a
-                  :class:`Cluster` object representing the coordinator with filled `Cluster.workers` attribute.
+        :returns: all MPP groups as :class:`dict`, with group IDs as keys and :class:`Cluster` objects as values.
         """
 
     @abc.abstractmethod
     def _load_cluster(
             self, path: str, loader: Callable[[Any], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
         """Main abstract method that implements the loading of :class:`Cluster` instance.
 
         .. note::
             Internally this method should call the *loader* method that will build :class:`Cluster` object which
             represents current state and topology of the cluster in DCS. This method supposed to be called only by
             the :meth:`~AbstractDCS.get_cluster` method.
 
         :param path: the path in DCS where to load Cluster(s) from.
-        :param loader: one of :meth:`~AbstractDCS._cluster_loader` or :meth:`~AbstractDCS._citus_cluster_loader`.
+        :param loader: one of :meth:`~AbstractDCS._postgresql_cluster_loader` or
+                       :meth:`~AbstractDCS._mpp_cluster_loader`.
 
         :raise: :exc:`~DCSError` in case of communication problems with DCS. If the current node was running as a
                 primary and exception raised, instance would be demoted.
         """
 
-    def __get_patroni_cluster(self, path: Optional[str] = None) -> Cluster:
+    def __get_postgresql_cluster(self, path: Optional[str] = None) -> Cluster:
         """Low level method to load a :class:`Cluster` object from DCS.
 
         :param path: optional client path in DCS backend to load from.
 
         :returns: a loaded :class:`Cluster` instance.
         """
         if path is None:
             path = self.client_path('')
-        cluster = self._load_cluster(path, self._cluster_loader)
+        cluster = self._load_cluster(path, self._postgresql_cluster_loader)
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(cluster, Cluster)
         return cluster
 
-    def is_citus_coordinator(self) -> bool:
-        """:class:`Cluster` instance has a Citus Coordinator group ID.
+    def is_mpp_coordinator(self) -> bool:
+        """:class:`Cluster` instance has a Coordinator group ID.
 
-        :returns: ``True`` if the given node is running as Citus Coordinator (``group=0``).
+        :returns: ``True`` if the given node is running as the MPP Coordinator.
         """
-        return self._citus_group == str(CITUS_COORDINATOR_GROUP_ID)
+        return self._mpp.is_coordinator()
 
-    def get_citus_coordinator(self) -> Optional[Cluster]:
-        """Load the Patroni cluster for the Citus Coordinator.
+    def get_mpp_coordinator(self) -> Optional[Cluster]:
+        """Load the PostgreSQL cluster for the MPP Coordinator.
 
-          .. note::
-              This method is only executed on the worker nodes (``group!=0``) to find the coordinator.
+        .. note::
+            This method is only executed on the worker nodes to find the coordinator.
 
-        :returns: Select :class:`Cluster` instance associated with the Citus Coordinator group ID.
+        :returns: Select :class:`Cluster` instance associated with the MPP Coordinator group ID.
         """
         try:
-            return self.__get_patroni_cluster(f'{self._base_path}/{CITUS_COORDINATOR_GROUP_ID}/')
+            return self.__get_postgresql_cluster(f'{self._base_path}/{self._mpp.coordinator_group_id}/')
         except Exception as e:
-            logger.error('Failed to load Citus coordinator cluster from %s: %r', self.__class__.__name__, e)
+            logger.error('Failed to load %s coordinator cluster from %s: %r',
+                         self._mpp.type, self.__class__.__name__, e)
         return None
 
-    def _get_citus_cluster(self) -> Cluster:
-        """Load Citus cluster from DCS.
+    def _get_mpp_cluster(self) -> Cluster:
+        """Load MPP cluster from DCS.
 
-        :returns: A Citus :class:`Cluster` instance for the coordinator with workers clusters in the `Cluster.workers`
+        :returns: A MPP :class:`Cluster` instance for the coordinator with workers clusters in the `Cluster.workers`
                   dict.
         """
-        groups = self._load_cluster(self._base_path + '/', self._citus_cluster_loader)
+        groups = self._load_cluster(self._base_path + '/', self._mpp_cluster_loader)
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(groups, dict)
-        cluster = groups.pop(CITUS_COORDINATOR_GROUP_ID, Cluster.empty())
+        cluster = groups.pop(self._mpp.coordinator_group_id, Cluster.empty())
         cluster.workers.update(groups)
         return cluster
 
     def get_cluster(self) -> Cluster:
         """Retrieve a fresh view of DCS.
 
         .. note::
             Stores copy of time, status and failsafe values for comparison in DCS update decisions.
             Caching is required to avoid overhead placed upon the REST API.
 
-            Returns either a Citus or Patroni implementation of :class:`Cluster` depending on availability.
+            Returns either a PostgreSQL or MPP implementation of :class:`Cluster` depending on availability.
 
         :returns:
         """
         try:
-            cluster = self._get_citus_cluster() if self.is_citus_coordinator() else self.__get_patroni_cluster()
+            cluster = self._get_mpp_cluster() if self.is_mpp_coordinator() else self.__get_postgresql_cluster()
         except Exception:
             self.reset_cluster()
             raise
 
         self._last_seen = int(time.time())
         self._last_status = {self._OPTIME: cluster.last_lsn}
         if cluster.slots:
```

### Comparing `patroni-3.2.2/patroni/dcs/consul.py` & `patroni-3.3.0/patroni/dcs/consul.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 from consul import ConsulException, NotFound, base
 from http.client import HTTPException
 from urllib3.exceptions import HTTPError
 from urllib.parse import urlencode, urlparse, quote
 from typing import Any, Callable, Dict, List, Mapping, NamedTuple, Optional, Union, Tuple, TYPE_CHECKING
 
 from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, Status, SyncState, \
-    TimelineHistory, ReturnFalseException, catch_return_false_exception, citus_group_re
+    TimelineHistory, ReturnFalseException, catch_return_false_exception
 from ..exceptions import DCSError
+from ..postgresql.mpp import AbstractMPP
 from ..utils import deep_compare, parse_bool, Retry, RetryFailedError, split_host_port, uri, USER_AGENT
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
 
 logger = logging.getLogger(__name__)
 
 
@@ -228,16 +229,16 @@
 
     service_name = re.sub(r'[^a-z0-9\-]', replace_char, scope_name.lower())
     return service_name[0:230]
 
 
 class Consul(AbstractDCS):
 
-    def __init__(self, config: Dict[str, Any]) -> None:
-        super(Consul, self).__init__(config)
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP) -> None:
+        super(Consul, self).__init__(config, mpp)
         self._base_path = self._base_path[1:]
         self._scope = config['scope']
         self._session = None
         self.__do_not_watch = False
         self._retry = Retry(deadline=config['retry_timeout'], max_delay=1, max_tries=-1,
                             retry_exceptions=(ConsulInternalError, HTTPException,
                                               HTTPError, socket.error, socket.timeout))
@@ -415,31 +416,44 @@
 
         return Cluster(initialize, config, leader, status, members, failover, sync, history, failsafe)
 
     @property
     def _consistency(self) -> str:
         return 'consistent' if self._ctl else self._client.consistency
 
-    def _cluster_loader(self, path: str) -> Cluster:
+    def _postgresql_cluster_loader(self, path: str) -> Cluster:
+        """Load and build the :class:`Cluster` object from DCS, which represents a single PostgreSQL cluster.
+
+        :param path: the path in DCS where to load :class:`Cluster` from.
+
+        :returns: :class:`Cluster` instance.
+        """
         _, results = self.retry(self._client.kv.get, path, recurse=True, consistency=self._consistency)
         if results is None:
             return Cluster.empty()
         nodes: Dict[str, Dict[str, Any]] = {}
         for node in results:
             node['Value'] = (node['Value'] or b'').decode('utf-8')
             nodes[node['Key'][len(path):]] = node
 
         return self._cluster_from_nodes(nodes)
 
-    def _citus_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+    def _mpp_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+        """Load and build all PostgreSQL clusters from a single MPP cluster.
+
+        :param path: the path in DCS where to load Cluster(s) from.
+
+        :returns: all MPP groups as :class:`dict`, with group IDs as keys and :class:`Cluster` objects as values.
+        """
+        results: Optional[List[Dict[str, Any]]]
         _, results = self.retry(self._client.kv.get, path, recurse=True, consistency=self._consistency)
-        clusters: Dict[int, Dict[str, Cluster]] = defaultdict(dict)
+        clusters: Dict[int, Dict[str, Dict[str, Any]]] = defaultdict(dict)
         for node in results or []:
             key = node['Key'][len(path):].split('/', 1)
-            if len(key) == 2 and citus_group_re.match(key[0]):
+            if len(key) == 2 and self._mpp.group_re.match(key[0]):
                 node['Value'] = (node['Value'] or b'').decode('utf-8')
                 clusters[int(key[0])][key[1]] = node
         return {group: self._cluster_from_nodes(nodes) for group, nodes in clusters.items()}
 
     def _load_cluster(
             self, path: str, loader: Callable[[str], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
@@ -560,22 +574,25 @@
         ):
             return self._update_service(new_data)
 
     def _do_attempt_to_acquire_leader(self, retry: Retry) -> bool:
         try:
             return retry(self._client.kv.put, self.leader_path, self._name, acquire=self._session)
         except InvalidSession:
-            logger.error('Our session disappeared from Consul. Will try to get a new one and retry attempt')
             self._session = None
-            retry.ensure_deadline(0)
+
+            if not retry.ensure_deadline(0):
+                logger.error('Our session disappeared from Consul. Deadline exceeded, giving up')
+                return False
+
+            logger.error('Our session disappeared from Consul. Will try to get a new one and retry attempt')
 
             retry(self._do_refresh_session)
 
             retry.ensure_deadline(1, ConsulError('_do_attempt_to_acquire_leader timeout'))
-
             return retry(self._client.kv.put, self.leader_path, self._name, acquire=self._session)
 
     @catch_return_false_exception
     def attempt_to_acquire_leader(self) -> bool:
         retry = self._retry.copy()
         self._run_and_handle_exceptions(self._do_refresh_session, retry=retry)
```

### Comparing `patroni-3.2.2/patroni/dcs/etcd.py` & `patroni-3.3.0/patroni/dcs/etcd.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 from threading import Thread
 from typing import Any, Callable, Collection, Dict, List, Optional, Union, Tuple, Type, TYPE_CHECKING
 from urllib.parse import urlparse
 from urllib3 import Timeout
 from urllib3.exceptions import HTTPError, ReadTimeoutError, ProtocolError
 
 from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, Status, SyncState, \
-    TimelineHistory, ReturnFalseException, catch_return_false_exception, citus_group_re
+    TimelineHistory, ReturnFalseException, catch_return_false_exception
 from ..exceptions import DCSError
+from ..postgresql.mpp import AbstractMPP
 from ..request import get as requests_get
 from ..utils import Retry, RetryFailedError, split_host_port, uri, USER_AGENT
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
 
 logger = logging.getLogger(__name__)
 
@@ -466,17 +467,17 @@
         if method in (self._MPOST, self._MPUT):
             kwargs['encode_multipart'] = False
         return self.http.request
 
 
 class AbstractEtcd(AbstractDCS):
 
-    def __init__(self, config: Dict[str, Any], client_cls: Type[AbstractEtcdClientWithFailover],
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP, client_cls: Type[AbstractEtcdClientWithFailover],
                  retry_errors_cls: Union[Type[Exception], Tuple[Type[Exception], ...]]) -> None:
-        super(AbstractEtcd, self).__init__(config)
+        super(AbstractEtcd, self).__init__(config, mpp)
         self._retry = Retry(deadline=config['retry_timeout'], max_delay=1, max_tries=-1,
                             retry_exceptions=retry_errors_cls)
         self._ttl = int(config.get('ttl') or 30)
         self._abstract_client = self.get_etcd_client(config, client_cls)
         self.__do_not_watch = False
         self._has_failed = False
 
@@ -641,16 +642,16 @@
     def wrapper(self: AbstractEtcd, *args: Any, **kwargs: Any) -> Any:
         return self.handle_etcd_exceptions(func, *args, **kwargs)
     return wrapper
 
 
 class Etcd(AbstractEtcd):
 
-    def __init__(self, config: Dict[str, Any]) -> None:
-        super(Etcd, self).__init__(config, EtcdClient, (etcd.EtcdLeaderElectionInProgress, EtcdRaftInternal))
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP) -> None:
+        super(Etcd, self).__init__(config, mpp, EtcdClient, (etcd.EtcdLeaderElectionInProgress, EtcdRaftInternal))
         self.__do_not_watch = False
 
     @property
     def _client(self) -> EtcdClient:
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(self._abstract_client, EtcdClient)
         return self._abstract_client
@@ -705,32 +706,44 @@
         try:
             failsafe = json.loads(failsafe.value) if failsafe else None
         except Exception:
             failsafe = None
 
         return Cluster(initialize, config, leader, status, members, failover, sync, history, failsafe)
 
-    def _cluster_loader(self, path: str) -> Cluster:
+    def _postgresql_cluster_loader(self, path: str) -> Cluster:
+        """Load and build the :class:`Cluster` object from DCS, which represents a single PostgreSQL cluster.
+
+        :param path: the path in DCS where to load :class:`Cluster` from.
+
+        :returns: :class:`Cluster` instance.
+        """
         try:
             result = self.retry(self._client.read, path, recursive=True, quorum=self._ctl)
         except etcd.EtcdKeyNotFound:
             return Cluster.empty()
         nodes = {node.key[len(result.key):].lstrip('/'): node for node in result.leaves}
         return self._cluster_from_nodes(result.etcd_index, nodes)
 
-    def _citus_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+    def _mpp_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+        """Load and build all PostgreSQL clusters from a single MPP cluster.
+
+        :param path: the path in DCS where to load Cluster(s) from.
+
+        :returns: all MPP groups as :class:`dict`, with group IDs as keys and :class:`Cluster` objects as values.
+        """
         try:
             result = self.retry(self._client.read, path, recursive=True, quorum=self._ctl)
         except etcd.EtcdKeyNotFound:
             return {}
 
         clusters: Dict[int, Dict[str, etcd.EtcdResult]] = defaultdict(dict)
         for node in result.leaves:
             key = node.key[len(result.key):].lstrip('/').split('/', 1)
-            if len(key) == 2 and citus_group_re.match(key[0]):
+            if len(key) == 2 and self._mpp.group_re.match(key[0]):
                 clusters[int(key[0])][key[1]] = node
         return {group: self._cluster_from_nodes(result.etcd_index, nodes) for group, nodes in clusters.items()}
 
     def _load_cluster(
             self, path: str, loader: Callable[[str], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
         cluster = None
```

### Comparing `patroni-3.2.2/patroni/dcs/etcd3.py` & `patroni-3.3.0/patroni/dcs/etcd3.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 from collections import defaultdict
 from enum import IntEnum
 from urllib3.exceptions import ReadTimeoutError, ProtocolError
 from threading import Condition, Lock, Thread
 from typing import Any, Callable, Collection, Dict, Iterator, List, Optional, Tuple, Type, TYPE_CHECKING, Union
 
 from . import ClusterConfig, Cluster, Failover, Leader, Member, Status, SyncState, \
-    TimelineHistory, catch_return_false_exception, citus_group_re
+    TimelineHistory, catch_return_false_exception
 from .etcd import AbstractEtcdClientWithFailover, AbstractEtcd, catch_etcd_errors, DnsCachingResolver, Retry
 from ..exceptions import DCSError, PatroniException
+from ..postgresql.mpp import AbstractMPP
 from ..utils import deep_compare, enable_keepalive, iter_response_objects, RetryFailedError, USER_AGENT
 
 logger = logging.getLogger(__name__)
 
 
 class Etcd3Error(DCSError):
     pass
@@ -193,32 +194,26 @@
 def build_range_request(key: str, range_end: Union[bytes, str, None] = None) -> Dict[str, Any]:
     fields = {'key': base64_encode(key)}
     if range_end:
         fields['range_end'] = base64_encode(range_end)
     return fields
 
 
-class ReAuthenticateMode(IntEnum):
-    NOT_REQUIRED = 0
-    REQUIRED = 1
-    WITHOUT_WATCHER_RESTART = 2
-
-
 def _handle_auth_errors(func: Callable[..., Any]) -> Any:
     def wrapper(self: 'Etcd3Client', *args: Any, **kwargs: Any) -> Any:
         return self.handle_auth_errors(func, *args, **kwargs)
     return wrapper
 
 
 class Etcd3Client(AbstractEtcdClientWithFailover):
 
     ERROR_CLS = Etcd3Error
 
     def __init__(self, config: Dict[str, Any], dns_resolver: DnsCachingResolver, cache_ttl: int = 300) -> None:
-        self._reauthenticate_reason = ReAuthenticateMode.NOT_REQUIRED
+        self._reauthenticate = False
         self._token = None
         self._cluster_version: Tuple[int, ...] = tuple()
         super(Etcd3Client, self).__init__({**config, 'version_prefix': '/v3beta'}, dns_resolver, cache_ttl)
 
         try:
             self.authenticate()
         except AuthFailed as e:
@@ -289,15 +284,15 @@
         members = self._handle_server_response(resp)['members']
         return [url for member in members for url in member.get('clientURLs', [])]
 
     def call_rpc(self, method: str, fields: Dict[str, Any], retry: Optional[Retry] = None) -> Dict[str, Any]:
         fields['retry'] = retry
         return self.api_execute(self.version_prefix + method, self._MPOST, fields)
 
-    def authenticate(self, *, restart_watcher: bool = True, retry: Optional[Retry] = None) -> bool:
+    def authenticate(self, *, retry: Optional[Retry] = None) -> bool:
         if self._use_proxies and not self._cluster_version:
             kwargs = self._prepare_common_parameters(1)
             self._ensure_version_prefix(self._base_uri, **kwargs)
         if not (self._cluster_version >= (3, 3) and self.username and self.password):
             return False
         logger.info('Trying to authenticate on Etcd...')
         old_token, self._token = self._token, None
@@ -311,28 +306,26 @@
             raise
         else:
             self._token = response.get('token')
         return old_token != self._token
 
     def handle_auth_errors(self: 'Etcd3Client', func: Callable[..., Any], *args: Any,
                            retry: Optional[Retry] = None, **kwargs: Any) -> Any:
+        reauthenticated = False
         exc = None
         while True:
-            if self._reauthenticate_reason:
+            if self._reauthenticate:
                 if self.username and self.password:
-                    self.authenticate(
-                        restart_watcher=self._reauthenticate_reason != ReAuthenticateMode.WITHOUT_WATCHER_RESTART,
-                        retry=retry)
-                    self._reauthenticate_reason = ReAuthenticateMode.NOT_REQUIRED
-                    if retry:
-                        retry.ensure_deadline(0)
+                    self.authenticate(retry=retry)
+                    self._reauthenticate = False
                 else:
                     msg = 'Username or password not set, authentication is not possible'
                     logger.fatal(msg)
                     raise exc or Etcd3Exception(msg)
+                reauthenticated = True
 
             try:
                 return func(self, *args, retry=retry, **kwargs)
             except (UserEmpty, PermissionDenied) as e:  # no token provided
                 # PermissionDenied is raised on 3.0 and 3.1
                 if self._cluster_version < (3, 3) and (not isinstance(e, PermissionDenied)
                                                        or self._cluster_version < (3, 2)):
@@ -342,19 +335,20 @@
                 exc = e
             except InvalidAuthToken as e:
                 logger.error('Invalid auth token: %s', self._token)
                 exc = e
             except AuthOldRevision as e:
                 logger.error('Auth token is for old revision of auth store')
                 exc = e
-            self._reauthenticate_reason = ReAuthenticateMode.WITHOUT_WATCHER_RESTART \
-                if isinstance(exc, AuthOldRevision) else ReAuthenticateMode.REQUIRED
-            if not retry:
+            self._reauthenticate = True
+            if retry:
+                logger.error('retry = %s', retry)
+                retry.ensure_deadline(0.5, exc)
+            elif reauthenticated:
                 raise exc
-            retry.ensure_deadline(0.5, exc)
 
     @_handle_auth_errors
     def range(self, key: str, range_end: Union[bytes, str, None] = None, serializable: bool = True,
               *, retry: Optional[Retry] = None) -> Dict[str, Any]:
         params = build_range_request(key, range_end)
         params['serializable'] = serializable  # For better performance. We can tolerate stale reads
         return self.call_rpc('/kv/range', params, retry)
@@ -598,20 +592,14 @@
         if self._kv_cache:
             self._kv_cache.kill_stream()
 
     def set_base_uri(self, value: str) -> None:
         super(PatroniEtcd3Client, self).set_base_uri(value)
         self._restart_watcher()
 
-    def authenticate(self, *, restart_watcher: bool = True, retry: Optional[Retry] = None) -> bool:
-        ret = super(PatroniEtcd3Client, self).authenticate(restart_watcher=restart_watcher, retry=retry)
-        if ret and restart_watcher:
-            self._restart_watcher()
-        return ret
-
     def _wait_cache(self, timeout: float) -> None:
         stop_time = time.time() + timeout
         while self._kv_cache and not self._kv_cache.is_ready():
             timeout = stop_time - time.time()
             if timeout <= 0:
                 raise RetryFailedError('Exceeded retry deadline')
             self._kv_cache.condition.wait(timeout)
@@ -667,16 +655,17 @@
         if not failure and not ret:
             self._restart_watcher()
         return ret
 
 
 class Etcd3(AbstractEtcd):
 
-    def __init__(self, config: Dict[str, Any]) -> None:
-        super(Etcd3, self).__init__(config, PatroniEtcd3Client, (DeadlineExceeded, Unavailable, FailedPrecondition))
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP) -> None:
+        super(Etcd3, self).__init__(config, mpp, PatroniEtcd3Client,
+                                    (DeadlineExceeded, Unavailable, FailedPrecondition))
         self.__do_not_watch = False
         self._lease = None
         self._last_lease_refresh = 0
 
         self._client.configure(self)
         if not self._ctl:
             self._client.start_watcher()
@@ -727,15 +716,19 @@
                 self.refresh_lease()
             except Etcd3Error:
                 logger.info('waiting on etcd')
                 time.sleep(5)
 
     @property
     def cluster_prefix(self) -> str:
-        return self._base_path + '/' if self.is_citus_coordinator() else self.client_path('')
+        """Construct the cluster prefix for the cluster.
+
+        :returns: path in the DCS under which we store information about this Patroni cluster.
+        """
+        return self._base_path + '/' if self.is_mpp_coordinator() else self.client_path('')
 
     @staticmethod
     def member(node: Dict[str, str]) -> Member:
         return Member.from_node(node['mod_revision'], os.path.basename(node['key']), node['lease'], node['value'])
 
     def _cluster_from_nodes(self, nodes: Dict[str, Any]) -> Cluster:
         # get initialize flag
@@ -781,26 +774,38 @@
         try:
             failsafe = json.loads(failsafe['value']) if failsafe else None
         except Exception:
             failsafe = None
 
         return Cluster(initialize, config, leader, status, members, failover, sync, history, failsafe)
 
-    def _cluster_loader(self, path: str) -> Cluster:
+    def _postgresql_cluster_loader(self, path: str) -> Cluster:
+        """Load and build the :class:`Cluster` object from DCS, which represents a single PostgreSQL cluster.
+
+        :param path: the path in DCS where to load :class:`Cluster` from.
+
+        :returns: :class:`Cluster` instance.
+        """
         nodes = {node['key'][len(path):]: node
                  for node in self._client.get_cluster(path)
                  if node['key'].startswith(path)}
         return self._cluster_from_nodes(nodes)
 
-    def _citus_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+    def _mpp_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+        """Load and build all PostgreSQL clusters from a single MPP cluster.
+
+        :param path: the path in DCS where to load Cluster(s) from.
+
+        :returns: all MPP groups as :class:`dict`, with group IDs as keys and :class:`Cluster` objects as values.
+        """
         clusters: Dict[int, Dict[str, Dict[str, Any]]] = defaultdict(dict)
         path = self._base_path + '/'
         for node in self._client.get_cluster(path):
             key = node['key'][len(path):].split('/', 1)
-            if len(key) == 2 and citus_group_re.match(key[0]):
+            if len(key) == 2 and self._mpp.group_re.match(key[0]):
                 clusters[int(key[0])][key[1]] = node
         return {group: self._cluster_from_nodes(nodes) for group, nodes in clusters.items()}
 
     def _load_cluster(
             self, path: str, loader: Callable[[str], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
         cluster = None
@@ -844,22 +849,24 @@
         def _retry(*args: Any, **kwargs: Any) -> Any:
             kwargs['retry'] = retry
             return retry(*args, **kwargs)
 
         try:
             return _retry(self._client.put, self.leader_path, self._name, self._lease, create_revision='0')
         except LeaseNotFound:
-            logger.error('Our lease disappeared from Etcd. Will try to get a new one and retry attempt')
             self._lease = None
-            retry.ensure_deadline(0)
+            if not retry.ensure_deadline(0):
+                logger.error('Our lease disappeared from Etcd. Deadline exceeded, giving up')
+                return False
+
+            logger.error('Our lease disappeared from Etcd. Will try to get a new one and retry attempt')
 
             _retry(self._do_refresh_lease)
 
             retry.ensure_deadline(1, Etcd3Error('_do_attempt_to_acquire_leader timeout'))
-
             return _retry(self._client.put, self.leader_path, self._name, self._lease, create_revision='0')
 
     @catch_return_false_exception
     def attempt_to_acquire_leader(self) -> bool:
         retry = self._retry.copy()
 
         def _retry(*args: Any, **kwargs: Any) -> Any:
```

### Comparing `patroni-3.2.2/patroni/dcs/exhibitor.py` & `patroni-3.3.0/patroni/dcs/exhibitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import random
 import time
 
 from typing import Any, Callable, Dict, List, Union
 
 from . import Cluster
 from .zookeeper import ZooKeeper
+from ..postgresql.mpp import AbstractMPP
 from ..request import get as requests_get
 from ..utils import uri
 
 logger = logging.getLogger(__name__)
 
 
 class ExhibitorEnsembleProvider(object):
@@ -62,18 +63,18 @@
     @property
     def zookeeper_hosts(self) -> str:
         return self._zookeeper_hosts
 
 
 class Exhibitor(ZooKeeper):
 
-    def __init__(self, config: Dict[str, Any]) -> None:
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP) -> None:
         interval = config.get('poll_interval', 300)
         self._ensemble_provider = ExhibitorEnsembleProvider(config['hosts'], config['port'], poll_interval=interval)
-        super(Exhibitor, self).__init__({**config, 'hosts': self._ensemble_provider.zookeeper_hosts})
+        super(Exhibitor, self).__init__({**config, 'hosts': self._ensemble_provider.zookeeper_hosts}, mpp)
 
     def _load_cluster(
             self, path: str, loader: Callable[[str], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
         if self._ensemble_provider.poll():
             self._client.set_hosts(self._ensemble_provider.zookeeper_hosts)
         return super(Exhibitor, self)._load_cluster(path, loader)
```

### Comparing `patroni-3.2.2/patroni/dcs/kubernetes.py` & `patroni-3.3.0/patroni/dcs/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 from collections import defaultdict
 from copy import deepcopy
 from http.client import HTTPException
 from urllib3.exceptions import HTTPError
 from threading import Condition, Lock, Thread
 from typing import Any, Callable, Collection, Dict, List, Optional, Tuple, Type, Union, TYPE_CHECKING
 
-from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, Status, SyncState, \
-    TimelineHistory, CITUS_COORDINATOR_GROUP_ID, citus_group_re
+from . import AbstractDCS, Cluster, ClusterConfig, Failover, Leader, Member, Status, SyncState, TimelineHistory
+from ..collections import EMPTY_DICT
 from ..exceptions import DCSError
+from ..postgresql.mpp import AbstractMPP
 from ..utils import deep_compare, iter_response_objects, keepalive_socket_options, \
     Retry, RetryFailedError, tzutc, uri, USER_AGENT
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
 
 logger = logging.getLogger(__name__)
 
@@ -466,15 +467,15 @@
                     path = '/'.join([args[1], kind, args[0]])
 
                 headers = {'Content-Type': 'application/strategic-merge-patch+json'} if action == 'patch' else {}
 
                 if len(args) == 3:  # name, namespace, body
                     body = args[2]
                 elif action == 'create':  # namespace, body
-                    body = args[1]
+                    body = args[1]  # pyright: ignore [reportGeneralTypeIssues]
                 elif action == 'delete':  # name, namespace
                     body = kwargs.pop('body', None)
                 else:
                     body = None
 
                 return self._api_client.call_api(method, path, headers, body, **kwargs)
             return wrapper
@@ -505,15 +506,15 @@
         super(KubernetesRetriableException, self).__init__(orig.status, orig.reason)
         self.body = orig.body
         self.headers = orig.headers
 
     @property
     def sleeptime(self) -> Optional[int]:
         try:
-            return int((self.headers or {}).get('retry-after', ''))
+            return int((self.headers or EMPTY_DICT).get('retry-after', ''))
         except Exception:
             return None
 
 
 class CoreV1ApiProxy(object):
     """Proxy class to work with k8s_client.CoreV1Api() object"""
 
@@ -650,23 +651,23 @@
         name = obj['metadata']['name']
 
         new_value = None
         if ev_type in ('ADDED', 'MODIFIED'):
             obj = K8sObject(obj)
             success, old_value = self.set(name, obj)
             if success:
-                new_value = (obj.metadata.annotations or {}).get(self._annotations_map.get(name))
+                new_value = (obj.metadata.annotations or EMPTY_DICT).get(self._annotations_map.get(name, ''))
         elif ev_type == 'DELETED':
             success, old_value = self.delete(name, obj['metadata']['resourceVersion'])
         else:
             return logger.warning('Unexpected event type: %s', ev_type)
 
         if success and obj.get('kind') != 'Pod':
             if old_value:
-                old_value = (old_value.metadata.annotations or {}).get(self._annotations_map.get(name))
+                old_value = (old_value.metadata.annotations or EMPTY_DICT).get(self._annotations_map.get(name, ''))
 
             value_changed = old_value != new_value and \
                 (name != self._dcs.config_path or old_value is not None and new_value is not None)
 
             if value_changed:
                 logger.debug('%s changed from %s to %s', name, old_value, new_value)
 
@@ -742,30 +743,28 @@
     def is_ready(self) -> bool:
         """Must be called only when holding the lock on `_condition`"""
         return self._is_ready
 
 
 class Kubernetes(AbstractDCS):
 
-    _CITUS_LABEL = 'citus-group'
-
-    def __init__(self, config: Dict[str, Any]) -> None:
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP) -> None:
         self._labels = deepcopy(config['labels'])
         self._labels[config.get('scope_label', 'cluster-name')] = config['scope']
         self._label_selector = ','.join('{0}={1}'.format(k, v) for k, v in self._labels.items())
         self._namespace = config.get('namespace') or 'default'
         self._role_label = config.get('role_label', 'role')
         self._leader_label_value = config.get('leader_label_value', 'master')
         self._follower_label_value = config.get('follower_label_value', 'replica')
         self._standby_leader_label_value = config.get('standby_leader_label_value', 'master')
         self._tmp_role_label = config.get('tmp_role_label')
         self._ca_certs = os.environ.get('PATRONI_KUBERNETES_CACERT', config.get('cacert')) or SERVICE_CERT_FILENAME
-        super(Kubernetes, self).__init__({**config, 'namespace': ''})
-        if self._citus_group:
-            self._labels[self._CITUS_LABEL] = self._citus_group
+        super(Kubernetes, self).__init__({**config, 'namespace': ''}, mpp)
+        if self._mpp.is_enabled():
+            self._labels[self._mpp.k8s_group_label] = str(self._mpp.group)
 
         self._retry = Retry(deadline=config['retry_timeout'], max_delay=1, max_tries=-1,
                             retry_exceptions=KubernetesRetriableException)
         self._ttl = int(config.get('ttl') or 30)
         try:
             k8s_config.load_incluster_config(ca_certs=self._ca_certs)
         except k8s_config.ConfigException:
@@ -842,15 +841,15 @@
         try:
             self._api.configure_retriable_http_codes([int(c) for c in retriable_http_codes])
         except Exception as e:
             logger.warning('Invalid value of retriable_http_codes = %s: %r', config['retriable_http_codes'], e)
 
     @staticmethod
     def member(pod: K8sObject) -> Member:
-        annotations = pod.metadata.annotations or {}
+        annotations = pod.metadata.annotations or EMPTY_DICT
         member = Member.from_node(pod.metadata.resource_version, pod.metadata.name, None, annotations.get('status', ''))
         member.data['pod_labels'] = pod.metadata.labels
         return member
 
     def _wait_caches(self, stop_time: float) -> None:
         while not (self._pods.is_ready() and self._kinds.is_ready()):
             timeout = stop_time - time.time()
@@ -923,37 +922,49 @@
         else:
             leader = None
 
         # failover key
         failover = nodes.get(path + self._FAILOVER)
         metadata = failover and failover.metadata
         failover = metadata and Failover.from_node(metadata.resource_version,
-                                                   (metadata.annotations or {}).copy())
+                                                   (metadata.annotations or EMPTY_DICT).copy())
 
         # get synchronization state
         sync = nodes.get(path + self._SYNC)
         metadata = sync and sync.metadata
         sync = SyncState.from_node(metadata and metadata.resource_version, metadata and metadata.annotations)
 
         return Cluster(initialize, config, leader, status, members, failover, sync, history, failsafe)
 
-    def _cluster_loader(self, path: Dict[str, Any]) -> Cluster:
+    def _postgresql_cluster_loader(self, path: Dict[str, Any]) -> Cluster:
+        """Load and build the :class:`Cluster` object from DCS, which represents a single PostgreSQL cluster.
+
+        :param path: the path in DCS where to load :class:`Cluster` from.
+
+        :returns: :class:`Cluster` instance.
+        """
         return self._cluster_from_nodes(path['group'], path['nodes'], path['pods'].values())
 
-    def _citus_cluster_loader(self, path: Dict[str, Any]) -> Dict[int, Cluster]:
+    def _mpp_cluster_loader(self, path: Dict[str, Any]) -> Dict[int, Cluster]:
+        """Load and build all PostgreSQL clusters from a single MPP cluster.
+
+        :param path: the path in DCS where to load Cluster(s) from.
+
+        :returns: all MPP groups as :class:`dict`, with group IDs as keys and :class:`Cluster` objects as values.
+        """
         clusters: Dict[str, Dict[str, Dict[str, K8sObject]]] = defaultdict(lambda: defaultdict(dict))
 
         for name, pod in path['pods'].items():
-            group = pod.metadata.labels.get(self._CITUS_LABEL)
-            if group and citus_group_re.match(group):
+            group = pod.metadata.labels.get(self._mpp.k8s_group_label)
+            if group and self._mpp.group_re.match(group):
                 clusters[group]['pods'][name] = pod
 
         for name, kind in path['nodes'].items():
-            group = kind.metadata.labels.get(self._CITUS_LABEL)
-            if group and citus_group_re.match(group):
+            group = kind.metadata.labels.get(self._mpp.k8s_group_label)
+            if group and self._mpp.group_re.match(group):
                 clusters[group]['nodes'][name] = kind
         return {int(group): self._cluster_from_nodes(group, value['nodes'], value['pods'].values())
                 for group, value in clusters.items()}
 
     def __load_cluster(
             self, group: Optional[str], loader: Callable[[Dict[str, Any]], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
@@ -961,36 +972,43 @@
             assert self._retry.deadline is not None
         stop_time = time.time() + self._retry.deadline
         self._api.refresh_api_servers_cache()
         try:
             with self._condition:
                 self._wait_caches(stop_time)
                 pods = {name: pod for name, pod in self._pods.copy().items()
-                        if not group or pod.metadata.labels.get(self._CITUS_LABEL) == group}
+                        if not group or pod.metadata.labels.get(self._mpp.k8s_group_label) == group}
                 nodes = {name: kind for name, kind in self._kinds.copy().items()
-                         if not group or kind.metadata.labels.get(self._CITUS_LABEL) == group}
+                         if not group or kind.metadata.labels.get(self._mpp.k8s_group_label) == group}
             return loader({'group': group, 'pods': pods, 'nodes': nodes})
         except Exception:
             logger.exception('get_cluster')
             raise KubernetesError('Kubernetes API is not responding properly')
 
     def _load_cluster(
             self, path: str, loader: Callable[[Any], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
-        group = self._citus_group if path == self.client_path('') else None
+        group = str(self._mpp.group) if self._mpp.is_enabled() and path == self.client_path('') else None
         return self.__load_cluster(group, loader)
 
-    def get_citus_coordinator(self) -> Optional[Cluster]:
+    def get_mpp_coordinator(self) -> Optional[Cluster]:
+        """Load the PostgreSQL cluster for the MPP Coordinator.
+
+        .. note::
+            This method is only executed on the worker nodes to find the coordinator.
+
+        :returns: Select :class:`Cluster` instance associated with the MPP Coordinator group ID.
+        """
         try:
-            ret = self.__load_cluster(str(CITUS_COORDINATOR_GROUP_ID), self._cluster_loader)
+            ret = self.__load_cluster(str(self._mpp.coordinator_group_id), self._postgresql_cluster_loader)
             if TYPE_CHECKING:  # pragma: no cover
                 assert isinstance(ret, Cluster)
             return ret
         except Exception as e:
-            logger.error('Failed to load Citus coordinator cluster from Kubernetes: %r', e)
+            logger.error('Failed to load %s coordinator cluster from Kubernetes: %r', self._mpp.type, e)
 
     @staticmethod
     def compare_ports(p1: K8sObject, p2: K8sObject) -> bool:
         return p1.name == p2.name and p1.port == p2.port and (p1.protocol or 'TCP') == (p2.protocol or 'TCP')
 
     @staticmethod
     def subsets_changed(last_observed_subsets: List[K8sObject], ip: str, ports: List[K8sObject]) -> bool:
@@ -1026,24 +1044,26 @@
         for p in ports:
             if p.name not in observed_ports or not Kubernetes.compare_ports(p, observed_ports.pop(p.name)):
                 return True
         return False
 
     def __target_ref(self, leader_ip: str, latest_subsets: List[K8sObject], pod: K8sObject) -> K8sObject:
         # we want to re-use existing target_ref if possible
+        empty_addresses: List[K8sObject] = []
         for subset in latest_subsets:
-            for address in subset.addresses or []:
+            for address in subset.addresses or empty_addresses:
                 if address.ip == leader_ip and address.target_ref and address.target_ref.name == self._name:
                     return address.target_ref
         return k8s_client.V1ObjectReference(kind='Pod', uid=pod.metadata.uid, namespace=self._namespace,
                                             name=self._name, resource_version=pod.metadata.resource_version)
 
     def _map_subsets(self, endpoints: Dict[str, Any], ips: List[str]) -> None:
         leader = self._kinds.get(self.leader_path)
-        latest_subsets = leader and leader.subsets or []
+        empty_addresses: List[K8sObject] = []
+        latest_subsets = leader and leader.subsets or empty_addresses
         if not ips:
             # We want to have subsets empty
             if latest_subsets:
                 endpoints['subsets'] = []
             return
 
         pod = self._pods.get(self._name)
@@ -1191,28 +1211,28 @@
             return False
 
         self._kinds.set(self.leader_path, kind)
 
         if not retry.ensure_deadline(0.5):
             return False
 
-        kind_annotations = kind and kind.metadata.annotations or {}
+        kind_annotations = kind and kind.metadata.annotations or EMPTY_DICT
         kind_resource_version = kind and kind.metadata.resource_version
 
         # There is different leader or resource_version in cache didn't change
         if kind and (kind_annotations.get(self._LEADER) != self._name or kind_resource_version == resource_version):
             return False
 
         return bool(_run_and_handle_exceptions(self._patch_or_create, self.leader_path, annotations,
                                                kind_resource_version, ips=ips, retry=_retry))
 
     def update_leader(self, leader: Leader, last_lsn: Optional[int],
                       slots: Optional[Dict[str, int]] = None, failsafe: Optional[Dict[str, str]] = None) -> bool:
         kind = self._kinds.get(self.leader_path)
-        kind_annotations = kind and kind.metadata.annotations or {}
+        kind_annotations = kind and kind.metadata.annotations or EMPTY_DICT
 
         if kind and kind_annotations.get(self._LEADER) != self._name:
             return False
 
         now = datetime.datetime.now(tzutc).isoformat()
         leader_observed_record = kind_annotations or self._leader_observed_record
         annotations = {self._LEADER: self._name, 'ttl': str(self._ttl), 'renewTime': now,
@@ -1325,15 +1345,15 @@
     def _delete_leader(self, leader: Leader) -> bool:
         """Unused"""
         raise NotImplementedError  # pragma: no cover
 
     def delete_leader(self, leader: Optional[Leader], last_lsn: Optional[int] = None) -> bool:
         ret = False
         kind = self._kinds.get(self.leader_path)
-        if kind and (kind.metadata.annotations or {}).get(self._LEADER) == self._name:
+        if kind and (kind.metadata.annotations or EMPTY_DICT).get(self._LEADER) == self._name:
             annotations: Dict[str, Optional[str]] = {self._LEADER: None}
             if last_lsn:
                 annotations[self._OPTIME] = str(last_lsn)
             ret = self.patch_or_create(self.leader_path, annotations, kind.metadata.resource_version, True, False, [])
             self.reset_cluster()
         return ret
```

### Comparing `patroni-3.2.2/patroni/dcs/raft.py` & `patroni-3.3.0/patroni/dcs/raft.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from pysyncobj import SyncObj, SyncObjConf, replicated, FAIL_REASON
 from pysyncobj.dns_resolver import globalDnsResolver
 from pysyncobj.node import TCPNode
 from pysyncobj.transport import TCPTransport, CONNECTION_STATE
 from pysyncobj.utility import TcpUtility
 from typing import Any, Callable, Collection, Dict, List, Optional, Set, Union, TYPE_CHECKING
 
-from . import AbstractDCS, ClusterConfig, Cluster, Failover, Leader, Member, Status, SyncState, \
-    TimelineHistory, citus_group_re
+from . import AbstractDCS, ClusterConfig, Cluster, Failover, Leader, Member, Status, SyncState, TimelineHistory
 from ..exceptions import DCSError
+from ..postgresql.mpp import AbstractMPP
 from ..utils import validate_directory
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
 
 logger = logging.getLogger(__name__)
 
 
@@ -281,16 +281,16 @@
             self.__destroying = True
             self.__thread.join()
         super(KVStoreTTL, self).destroy()
 
 
 class Raft(AbstractDCS):
 
-    def __init__(self, config: Dict[str, Any]) -> None:
-        super(Raft, self).__init__(config)
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP) -> None:
+        super(Raft, self).__init__(config, mpp)
         self._ttl = int(config.get('ttl') or 30)
 
         ready_event = threading.Event()
         self._sync_obj = KVStoreTTL(ready_event.set, self._on_set, self._on_delete, commandsWaitLeader=False, **config)
         self._sync_obj.startAutoTick()
 
         while True:
@@ -371,27 +371,39 @@
         try:
             failsafe = json.loads(failsafe['value']) if failsafe else None
         except Exception:
             failsafe = None
 
         return Cluster(initialize, config, leader, status, members, failover, sync, history, failsafe)
 
-    def _cluster_loader(self, path: str) -> Cluster:
+    def _postgresql_cluster_loader(self, path: str) -> Cluster:
+        """Load and build the :class:`Cluster` object from DCS, which represents a single PostgreSQL cluster.
+
+        :param path: the path in DCS where to load :class:`Cluster` from.
+
+        :returns: :class:`Cluster` instance.
+        """
         response = self._sync_obj.get(path, recursive=True)
         if not response:
             return Cluster.empty()
         nodes = {key[len(path):]: value for key, value in response.items()}
         return self._cluster_from_nodes(nodes)
 
-    def _citus_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+    def _mpp_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+        """Load and build all PostgreSQL clusters from a single MPP cluster.
+
+        :param path: the path in DCS where to load Cluster(s) from.
+
+        :returns: all MPP groups as :class:`dict`, with group IDs as keys and :class:`Cluster` objects as values.
+        """
         clusters: Dict[int, Dict[str, Any]] = defaultdict(dict)
         response = self._sync_obj.get(path, recursive=True)
         for key, value in (response or {}).items():
             key = key[len(path):].split('/', 1)
-            if len(key) == 2 and citus_group_re.match(key[0]):
+            if len(key) == 2 and self._mpp.group_re.match(key[0]):
                 clusters[int(key[0])][key[1]] = value
         return {group: self._cluster_from_nodes(nodes) for group, nodes in clusters.items()}
 
     def _load_cluster(
             self, path: str, loader: Callable[[str], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
         return loader(path)
```

### Comparing `patroni-3.2.2/patroni/dcs/zookeeper.py` & `patroni-3.3.0/patroni/dcs/zookeeper.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from kazoo.exceptions import ConnectionClosedError, NoNodeError, NodeExistsError, SessionExpiredError
 from kazoo.handlers.threading import AsyncResult, SequentialThreadingHandler
 from kazoo.protocol.states import KeeperState, WatchedEvent, ZnodeStat
 from kazoo.retry import RetryFailedError
 from kazoo.security import ACL, make_acl
 from typing import Any, Callable, Dict, List, Optional, Union, Tuple, TYPE_CHECKING
 
-from . import AbstractDCS, ClusterConfig, Cluster, Failover, Leader, Member, Status, SyncState, \
-    TimelineHistory, citus_group_re
+from . import AbstractDCS, ClusterConfig, Cluster, Failover, Leader, Member, Status, SyncState, TimelineHistory
 from ..exceptions import DCSError
+from ..postgresql.mpp import AbstractMPP
 from ..utils import deep_compare
 if TYPE_CHECKING:  # pragma: no cover
     from ..config import Config
 
 logger = logging.getLogger(__name__)
 
 
@@ -83,16 +83,16 @@
             async_object.set_exception(SessionExpiredError())
             return False
         return super(PatroniKazooClient, self)._call(request, async_object)
 
 
 class ZooKeeper(AbstractDCS):
 
-    def __init__(self, config: Dict[str, Any]) -> None:
-        super(ZooKeeper, self).__init__(config)
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP) -> None:
+        super(ZooKeeper, self).__init__(config, mpp)
 
         hosts: Union[str, List[str]] = config.get('hosts', [])
         if isinstance(hosts, list):
             hosts = ','.join(hosts)
 
         mapping = {'use_ssl': 'use_ssl', 'verify': 'verify_certs', 'cacert': 'ca',
                    'cert': 'certfile', 'key': 'keyfile', 'key_password': 'keyfile_password'}
@@ -111,15 +111,16 @@
                                             admin='ADMIN' in normalizedPermissions,
                                             all='ALL' in normalizedPermissions))
             kwargs['default_acl'] = default_acl
 
         self._client = PatroniKazooClient(hosts, handler=PatroniSequentialThreadingHandler(config['retry_timeout']),
                                           timeout=config['ttl'], connection_retry=KazooRetry(max_delay=1, max_tries=-1,
                                           sleep_func=time.sleep), command_retry=KazooRetry(max_delay=1, max_tries=-1,
-                                          deadline=config['retry_timeout'], sleep_func=time.sleep), **kwargs)
+                                          deadline=config['retry_timeout'], sleep_func=time.sleep),
+                                          auth_data=list(config.get('auth_data', {}).items()), **kwargs)
 
         self.__last_member_data: Optional[Dict[str, Any]] = None
 
         self._orig_kazoo_connect = self._client._connection._connect
         self._client._connection._connect = self._kazoo_connect
 
         self._client.start()
@@ -209,15 +210,21 @@
         members: List[Member] = []
         for member in self.get_children(path + self._MEMBERS):
             data = self.get_node(path + self._MEMBERS + member)
             if data is not None:
                 members.append(self.member(member, *data))
         return members
 
-    def _cluster_loader(self, path: str) -> Cluster:
+    def _postgresql_cluster_loader(self, path: str) -> Cluster:
+        """Load and build the :class:`Cluster` object from DCS, which represents a single PostgreSQL cluster.
+
+        :param path: the path in DCS where to load :class:`Cluster` from.
+
+        :returns: :class:`Cluster` instance.
+        """
         nodes = set(self.get_children(path))
 
         # get initialize flag
         initialize = (self.get_node(path + self._INITIALIZE) or [None])[0] if self._INITIALIZE in nodes else None
 
         # get global dynamic configuration
         config = self.get_node(path + self._CONFIG, watch=self._watcher) if self._CONFIG in nodes else None
@@ -253,19 +260,25 @@
         try:
             failsafe = json.loads(failsafe[0]) if failsafe else None
         except Exception:
             failsafe = None
 
         return Cluster(initialize, config, leader, status, members, failover, sync, history, failsafe)
 
-    def _citus_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+    def _mpp_cluster_loader(self, path: str) -> Dict[int, Cluster]:
+        """Load and build all PostgreSQL clusters from a single MPP cluster.
+
+        :param path: the path in DCS where to load Cluster(s) from.
+
+        :returns: all MPP groups as :class:`dict`, with group IDs as keys and :class:`Cluster` objects as values.
+        """
         ret: Dict[int, Cluster] = {}
         for node in self.get_children(path):
-            if citus_group_re.match(node):
-                ret[int(node)] = self._cluster_loader(path + node + '/')
+            if self._mpp.group_re.match(node):
+                ret[int(node)] = self._postgresql_cluster_loader(path + node + '/')
         return ret
 
     def _load_cluster(
             self, path: str, loader: Callable[[str], Union[Cluster, Dict[int, Cluster]]]
     ) -> Union[Cluster, Dict[int, Cluster]]:
         try:
             return self._client.retry(loader, path)
```

### Comparing `patroni-3.2.2/patroni/exceptions.py` & `patroni-3.3.0/patroni/exceptions.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/file_perm.py` & `patroni-3.3.0/patroni/file_perm.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/ha.py` & `patroni-3.3.0/patroni/ha.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import uuid
 
 from multiprocessing.pool import ThreadPool
 from threading import RLock
 from typing import Any, Callable, Collection, Dict, List, NamedTuple, Optional, Union, Tuple, TYPE_CHECKING
 
-from . import psycopg
+from . import global_config, psycopg
 from .__main__ import Patroni
 from .async_executor import AsyncExecutor, CriticalTask
 from .collections import CaseInsensitiveSet
 from .dcs import AbstractDCS, Cluster, Leader, Member, RemoteMember, Status, slot_name_from_member_name
 from .exceptions import DCSError, PostgresConnectionException, PatroniFatalException
 from .postgresql.callback_executor import CallbackAction
 from .postgresql.misc import postgres_version_to_int
@@ -152,15 +152,14 @@
 
     def __init__(self, patroni: Patroni):
         self.patroni = patroni
         self.state_handler = patroni.postgresql
         self._rewind = Rewind(self.state_handler)
         self.dcs = patroni.dcs
         self.cluster = Cluster.empty()
-        self.global_config = self.patroni.config.get_global_config(None)
         self.old_cluster = Cluster.empty()
         self._leader_expiry = 0
         self._leader_expiry_lock = RLock()
         self._failsafe = Failsafe(patroni.dcs)
         self._was_paused = False
         self._leader_timeline = None
         self.recovering = False
@@ -172,40 +171,43 @@
 
         # Each member publishes various pieces of information to the DCS using touch_member. This lock protects
         # the state and publishing procedure to have consistent ordering and avoid publishing stale values.
         self._member_state_lock = RLock()
         # Count of concurrent sync disabling requests. Value above zero means that we don't want to be synchronous
         # standby. Changes protected by _member_state_lock.
         self._disable_sync = 0
-        # Remember the last known member role and state written to the DCS in order to notify Citus coordinator
+        # Remember the last known member role and state written to the DCS in order to notify MPP coordinator
         self._last_state = None
 
         # We need following property to avoid shutdown of postgres when join of Patroni to the postgres
         # already running as replica was aborted due to cluster not being initialized in DCS.
         self._join_aborted = False
 
         # used only in backoff after failing a pre_promote script
         self._released_leader_key_timestamp = 0
 
+        # Initialize global config
+        global_config.update(None, self.patroni.config.dynamic_configuration)
+
     def primary_stop_timeout(self) -> Union[int, None]:
         """:returns: "primary_stop_timeout" from the global configuration or `None` when not in synchronous mode."""
-        ret = self.global_config.primary_stop_timeout
+        ret = global_config.primary_stop_timeout
         return ret if ret > 0 and self.is_synchronous_mode() else None
 
     def is_paused(self) -> bool:
         """:returns: `True` if in maintenance mode."""
-        return self.global_config.is_paused
+        return global_config.is_paused
 
     def check_timeline(self) -> bool:
         """:returns: `True` if should check whether the timeline is latest during the leader race."""
-        return self.global_config.check_mode('check_timeline')
+        return global_config.check_mode('check_timeline')
 
     def is_standby_cluster(self) -> bool:
         """:returns: `True` if global configuration has a valid "standby_cluster" section."""
-        return self.global_config.is_standby_cluster
+        return global_config.is_standby_cluster
 
     def is_leader(self) -> bool:
         """:returns: `True` if the current node is the leader, based on expiration set when it last held the key."""
         with self._leader_expiry_lock:
             return self._leader_expiry > time.time()
 
     def set_is_leader(self, value: bool) -> None:
@@ -291,17 +293,16 @@
                   as a ``primary`` or as a ``standby_leader``, otherwise ``False``.
         """
         last_lsn = slots = None
         if update_status:
             try:
                 last_lsn = self.state_handler.last_operation()
                 slots = self.cluster.filter_permanent_slots(
-                    {**self.state_handler.slots(), slot_name_from_member_name(self.state_handler.name): last_lsn},
-                    self.is_standby_cluster(),
-                    self.state_handler.major_version)
+                    self.state_handler,
+                    {**self.state_handler.slots(), slot_name_from_member_name(self.state_handler.name): last_lsn})
             except Exception:
                 logger.exception('Exception when called state_handler.last_operation()')
         if TYPE_CHECKING:  # pragma: no cover
             assert self.cluster.leader is not None
         try:
             ret = self.dcs.update_leader(self.cluster.leader, last_lsn, slots, self._failsafe_config())
         except DCSError:
@@ -324,28 +325,34 @@
         """Return configuration tags merged with dynamically applied tags."""
         tags = self.patroni.tags.copy()
         # _disable_sync could be modified concurrently, but we don't care as attribute get and set are atomic.
         if self._disable_sync > 0:
             tags['nosync'] = True
         return tags
 
-    def notify_citus_coordinator(self, event: str) -> None:
-        if self.state_handler.citus_handler.is_worker():
-            coordinator = self.dcs.get_citus_coordinator()
+    def notify_mpp_coordinator(self, event: str) -> None:
+        """Send an event to the MPP coordinator.
+
+        :param event: the type of event for coordinator to parse.
+        """
+        mpp_handler = self.state_handler.mpp_handler
+        if mpp_handler.is_worker():
+            coordinator = self.dcs.get_mpp_coordinator()
             if coordinator and coordinator.leader and coordinator.leader.conn_url:
                 try:
                     data = {'type': event,
-                            'group': self.state_handler.citus_handler.group(),
+                            'group': mpp_handler.group,
                             'leader': self.state_handler.name,
                             'timeout': self.dcs.ttl,
                             'cooldown': self.patroni.config['retry_timeout']}
                     timeout = self.dcs.ttl if event == 'before_demote' else 2
-                    self.patroni.request(coordinator.leader.member, 'post', 'citus', data, timeout=timeout, retries=0)
+                    endpoint = 'citus' if mpp_handler.type == 'Citus' else 'mpp'
+                    self.patroni.request(coordinator.leader.member, 'post', endpoint, data, timeout=timeout, retries=0)
                 except Exception as e:
-                    logger.warning('Request to Citus coordinator leader %s %s failed: %r',
+                    logger.warning('Request to %s coordinator leader %s %s failed: %r', mpp_handler.type,
                                    coordinator.leader.name, coordinator.leader.member.api_url, e)
 
     def touch_member(self) -> bool:
         with self._member_state_lock:
             data: Dict[str, Any] = {
                 'conn_url': self.state_handler.connection_string,
                 'api_url': self.patroni.api.connection_string,
@@ -359,16 +366,17 @@
                 data['proxy_url'] = proxy_url
 
             if self.is_leader() and not self._rewind.checkpoint_after_promote():
                 data['checkpoint_after_promote'] = False
             tags = self.get_effective_tags()
             if tags:
                 data['tags'] = tags
-            if self.state_handler.pending_restart:
+            if self.state_handler.pending_restart_reason:
                 data['pending_restart'] = True
+                data['pending_restart_reason'] = dict(self.state_handler.pending_restart_reason)
             if self._async_executor.scheduled_action in (None, 'promote') \
                     and data['state'] in ['running', 'restarting', 'starting']:
                 try:
                     timeline, wal_position, pg_control_timeline = self.state_handler.timeline_wal_position()
                     data['xlog_location'] = wal_position
                     if not timeline:  # running as a standby
                         replication_state = self.state_handler.replication_state()
@@ -400,15 +408,15 @@
             if self.is_paused():
                 data['pause'] = True
 
             ret = self.dcs.touch_member(data)
             if ret:
                 new_state = (data['state'], {'master': 'primary'}.get(data['role'], data['role']))
                 if self._last_state != new_state and new_state == ('running', 'primary'):
-                    self.notify_citus_coordinator('after_promote')
+                    self.notify_mpp_coordinator('after_promote')
                 self._last_state = new_state
             return ret
 
     def clone(self, clone_member: Union[Leader, Member, None] = None, msg: str = '(without leader)') -> Optional[bool]:
         if self.is_standby_cluster() and not isinstance(clone_member, RemoteMember):
             clone_member = self.get_remote_member(clone_member)
 
@@ -446,15 +454,15 @@
         if not self.cluster.is_unlocked() and clone_member:
             member_role = 'leader' if clone_member == self.cluster.leader else 'replica'
             msg = "from {0} '{1}'".format(member_role, clone_member.name)
             ret = self._async_executor.try_run_async('bootstrap {0}'.format(msg), self.clone, args=(clone_member, msg))
             return ret or 'trying to bootstrap {0}'.format(msg)
 
         # no leader, but configuration may allowed replica creation using backup tools
-        create_replica_methods = self.global_config.get_standby_cluster_config().get('create_replica_methods', []) \
+        create_replica_methods = global_config.get_standby_cluster_config().get('create_replica_methods', []) \
             if self.is_standby_cluster() else None
         can_bootstrap = self.state_handler.can_create_replica_without_replication_connection(create_replica_methods)
         concurrent_bootstrap = self.cluster.initialize == ""
         if can_bootstrap and not concurrent_bootstrap:
             msg = 'bootstrap (without leader)'
             return self._async_executor.try_run_async(msg, self.clone) or 'trying to ' + msg
         return 'waiting for {0}leader to bootstrap'.format('standby_' if self.is_standby_cluster() else '')
@@ -521,15 +529,15 @@
              be removed if it is allowed by configuration.
 
           - after ``crash recovery`` and/or ``pg_rewind`` are executed, postgres is started in recovery.
 
         :returns: action message, describing what was performed.
         """
         if self.has_lock() and self.update_lock():
-            timeout = self.global_config.primary_start_timeout
+            timeout = global_config.primary_start_timeout
             if timeout == 0:
                 # We are requested to prefer failing over to restarting primary. But see first if there
                 # is anyone to fail over to.
                 if self.is_failover_possible():
                     self.watchdog.disable()
                     logger.info("Primary crashed. Failing over.")
                     self.demote('immediate')
@@ -598,17 +606,20 @@
     def _get_node_to_follow(self, cluster: Cluster) -> Union[Leader, Member, None]:
         """Determine the node to follow.
 
         :param cluster: the currently known cluster state from DCS.
 
         :returns: the node which we should be replicating from.
         """
+        # nostream is set, the node must not use WAL streaming
+        if self.patroni.nostream:
+            return None
         # The standby leader or when there is no standby leader we want to follow
         # the remote member, except when there is no standby leader in pause.
-        if self.is_standby_cluster() \
+        elif self.is_standby_cluster() \
                 and (cluster.leader and cluster.leader.name and cluster.leader.name == self.state_handler.name
                      or cluster.is_unlocked() and not self.is_paused()):
             node_to_follow = self.get_remote_member()
         # If replicatefrom tag is set, try to follow the node mentioned there, otherwise, follow the leader.
         elif self.patroni.replicatefrom and self.patroni.replicatefrom != self.state_handler.name:
             node_to_follow = cluster.get_member(self.patroni.replicatefrom)
         else:
@@ -618,15 +629,15 @@
 
         if node_to_follow and not isinstance(node_to_follow, RemoteMember):
             # we are going to abuse Member.data to pass following parameters
             params = ('restore_command', 'archive_cleanup_command')
             for param in params:  # It is highly unlikely to happen, but we want to protect from the case
                 node_to_follow.data.pop(param, None)  # when above-mentioned params came from outside.
             if self.is_standby_cluster():
-                standby_config = self.global_config.get_standby_cluster_config()
+                standby_config = global_config.get_standby_cluster_config()
                 node_to_follow.data.update({p: standby_config[p] for p in params if standby_config.get(p)})
 
         return node_to_follow
 
     def follow(self, demote_reason: str, follow_reason: str, refresh: bool = True) -> str:
         if refresh:
             self.load_cluster_from_dcs()
@@ -680,19 +691,19 @@
                 self.state_handler.set_role(role)
                 self.state_handler.call_nowait(CallbackAction.ON_ROLE_CHANGE)
 
         return follow_reason
 
     def is_synchronous_mode(self) -> bool:
         """:returns: `True` if synchronous replication is requested."""
-        return self.global_config.is_synchronous_mode
+        return global_config.is_synchronous_mode
 
     def is_failsafe_mode(self) -> bool:
         """:returns: `True` if failsafe_mode is enabled in global configuration."""
-        return self.global_config.check_mode('failsafe_mode')
+        return global_config.check_mode('failsafe_mode')
 
     def process_sync_replication(self) -> None:
         """Process synchronous standby beahvior.
 
         Synchronous standbys are registered in two places postgresql.conf and DCS. The order of updating them must
         be right. The invariant that should be kept is that if a node is primary and sync_standby is set in DCS,
         then that node must have synchronous_standby set to that value. Or more simple, first set in postgresql.conf
@@ -728,15 +739,15 @@
                     logger.info("Updating synchronous privilege temporarily from %s to %s",
                                 list(current), list(sync_common))
                     sync = self.dcs.write_sync_state(self.state_handler.name, sync_common, version=sync.version)
                     if not sync:
                         return logger.info('Synchronous replication key updated by someone else.')
 
                 # When strict mode and no suitable replication connections put "*" to synchronous_standby_names
-                if self.global_config.is_synchronous_mode_strict and not picked:
+                if global_config.is_synchronous_mode_strict and not picked:
                     picked = CaseInsensitiveSet('*')
                     logger.warning("No standbys available!")
 
                 # Update postgresql.conf and wait 2 secs for changes to become active
                 logger.info("Assigning synchronous standby status to %s", list(picked))
                 self.state_handler.sync_handler.set_synchronous_standby_names(picked)
 
@@ -801,15 +812,15 @@
         if primary_timeline == 1:
             if cluster_history:
                 self.dcs.set_history_value('[]')
         elif not cluster_history or cluster_history[-1][0] != primary_timeline - 1 or len(cluster_history[-1]) != 5:
             cluster_history_dict: Dict[int, List[Any]] = {line[0]: list(line) for line in cluster_history}
             history: List[List[Any]] = list(map(list, self.state_handler.get_history(primary_timeline)))
             if self.cluster.config:
-                history = history[-self.cluster.config.max_timelines_history:]
+                history = history[-global_config.max_timelines_history:]
             for line in history:
                 # enrich current history with promotion timestamps stored in DCS
                 cluster_history_line = cluster_history_dict.get(line[0], [])
                 if len(line) == 3 and len(cluster_history_line) >= 4 and cluster_history_line[1] == line[1]:
                     line.append(cluster_history_line[3])
                     if len(cluster_history_line) == 5:
                         line.append(cluster_history_line[4])
@@ -845,35 +856,35 @@
 
         if self.state_handler.is_primary():
             # Inform the state handler about its primary role.
             # It may be unaware of it if postgres is promoted manually.
             self.state_handler.set_role('master')
             self.process_sync_replication()
             self.update_cluster_history()
-            self.state_handler.citus_handler.sync_pg_dist_node(self.cluster)
+            self.state_handler.mpp_handler.sync_meta_data(self.cluster)
             return message
         elif self.state_handler.role in ('master', 'promoted', 'primary'):
             self.process_sync_replication()
             return message
         else:
             if self.is_synchronous_mode():
                 # Just set ourselves as the authoritative source of truth for now. We don't want to wait for standbys
                 # to connect. We will try finding a synchronous standby in the next cycle.
                 if not self.dcs.write_sync_state(self.state_handler.name, None, version=self.cluster.sync.version):
                     # Somebody else updated sync state, it may be due to us losing the lock. To be safe, postpone
                     # promotion until next cycle. TODO: trigger immediate retry of run_cycle
                     return 'Postponing promotion because synchronous replication state was updated by somebody else'
                 self.state_handler.sync_handler.set_synchronous_standby_names(
-                    CaseInsensitiveSet('*') if self.global_config.is_synchronous_mode_strict else CaseInsensitiveSet())
+                    CaseInsensitiveSet('*') if global_config.is_synchronous_mode_strict else CaseInsensitiveSet())
             if self.state_handler.role not in ('master', 'promoted', 'primary'):
                 # reset failsafe state when promote
                 self._failsafe.set_is_active(0)
 
                 def before_promote():
-                    self.notify_citus_coordinator('before_promote')
+                    self.notify_mpp_coordinator('before_promote')
 
                 with self._async_response:
                     self._async_response.reset()
 
                 self._async_executor.try_run_async('promote', self.state_handler.promote,
                                                    args=(self.dcs.loop_wait, self._async_response, before_promote))
             return promote_message
@@ -970,15 +981,15 @@
         """Returns if instance with an wal should consider itself unhealthy to be promoted due to replication lag.
 
         :param wal_position: Current wal position.
 
         :returns True when node is lagging
         """
         lag = (self.cluster.last_lsn or 0) - wal_position
-        return lag > self.global_config.maximum_lag_on_failover
+        return lag > global_config.maximum_lag_on_failover
 
     def _is_healthiest_node(self, members: Collection[Member], check_replication_lag: bool = True) -> bool:
         """This method tries to determine whether I am healthy enough to became a new leader candidate or not."""
 
         my_wal_position = self.state_handler.last_operation()
         if check_replication_lag and self.is_lagging(my_wal_position):
             logger.info('My wal position exceeds maximum replication lag')
@@ -1236,18 +1247,18 @@
             if self.is_failover_possible(cluster_lsn=checkpoint_location):
                 self.state_handler.set_role('demoted')
                 with self._async_executor:
                     self.release_leader_key_voluntarily(prev_location)
                     status['released'] = True
 
         def before_shutdown() -> None:
-            if self.state_handler.citus_handler.is_coordinator():
-                self.state_handler.citus_handler.on_demote()
+            if self.state_handler.mpp_handler.is_coordinator():
+                self.state_handler.mpp_handler.on_demote()
             else:
-                self.notify_citus_coordinator('before_demote')
+                self.notify_mpp_coordinator('before_demote')
 
         self.state_handler.stop(str(mode_control['stop']), checkpoint=bool(mode_control['checkpoint']),
                                 on_safepoint=self.watchdog.disable if self.watchdog.is_running else None,
                                 on_shutdown=on_shutdown if mode_control['release'] else None,
                                 before_shutdown=before_shutdown if mode == 'graceful' else None,
                                 stop_timeout=self.primary_stop_timeout())
         self.state_handler.set_role('demoted')
@@ -1483,15 +1494,15 @@
         # run_scheduled_action.
         if role and role != self.state_handler.role:
             reason_to_cancel = "host role mismatch"
 
         if postgres_version and postgres_version_to_int(postgres_version) <= int(self.state_handler.server_version):
             reason_to_cancel = "postgres version mismatch"
 
-        if pending_restart and not self.state_handler.pending_restart:
+        if pending_restart and not self.state_handler.pending_restart_reason:
             reason_to_cancel = "pending restart flag is not set"
 
         if not reason_to_cancel:
             return True
         else:
             logger.info("not proceeding with the restart: %s", reason_to_cancel)
         return False
@@ -1537,22 +1548,22 @@
             # Make the main loop to think that we were recovering dead postgres. If we fail
             # to start postgres after a specified timeout (see below), we need to remove
             # leader key (if it belong to us) rather than trying to start postgres once again.
             self.recovering = True
 
         # Now that restart is scheduled we can set timeout for startup, it will get reset
         # once async executor runs and main loop notices PostgreSQL as up.
-        timeout = restart_data.get('timeout', self.global_config.primary_start_timeout)
+        timeout = restart_data.get('timeout', global_config.primary_start_timeout)
         self.set_start_timeout(timeout)
 
         def before_shutdown() -> None:
-            self.notify_citus_coordinator('before_demote')
+            self.notify_mpp_coordinator('before_demote')
 
         def after_start() -> None:
-            self.notify_citus_coordinator('after_promote')
+            self.notify_mpp_coordinator('after_promote')
 
         # For non async cases we want to wait for restart to complete or timeout before returning.
         do_restart = functools.partial(self.state_handler.restart, timeout, self._async_executor.critical_task,
                                        before_shutdown=before_shutdown if self.has_lock() else None,
                                        after_start=after_start if self.has_lock() else None)
         if self.is_synchronous_mode() and not self.has_lock():
             do_restart = functools.partial(self.while_not_sync_standby, do_restart)
@@ -1601,15 +1612,15 @@
 
         self._async_executor.run_async(self._do_reinitialize, args=(cluster, ))
 
     def handle_long_action_in_progress(self) -> str:
         """Figure out what to do with the task AsyncExecutor is performing."""
         if self.has_lock() and self.update_lock():
             if self._async_executor.scheduled_action == 'doing crash recovery in a single user mode':
-                time_left = self.global_config.primary_start_timeout - (time.time() - self._crash_recovery_started)
+                time_left = global_config.primary_start_timeout - (time.time() - self._crash_recovery_started)
                 if time_left <= 0 and self.is_failover_possible():
                     logger.info("Demoting self because crash recovery is taking too long")
                     self.state_handler.cancellable.cancel(True)
                     self.demote('immediate')
                     return 'terminated crash recovery because of startup timeout'
 
             return 'updated leader lock during {0}'.format(self._async_executor.scheduled_action)
@@ -1686,15 +1697,15 @@
         self._rewind.ensure_checkpoint_after_promote(self.wakeup)
         self.dcs.initialize(create_new=(self.cluster.initialize is None), sysid=self.state_handler.sysid)
         self.dcs.set_config_value(json.dumps(self.patroni.config.dynamic_configuration, separators=(',', ':')))
         self.dcs.take_leader()
         self.set_is_leader(True)
         if self.is_synchronous_mode():
             self.state_handler.sync_handler.set_synchronous_standby_names(
-                CaseInsensitiveSet('*') if self.global_config.is_synchronous_mode_strict else CaseInsensitiveSet())
+                CaseInsensitiveSet('*') if global_config.is_synchronous_mode_strict else CaseInsensitiveSet())
         self.state_handler.call_nowait(CallbackAction.ON_START)
         self.load_cluster_from_dcs()
 
         return 'initialized a new cluster'
 
     def handle_starting_instance(self) -> Optional[str]:
         """Starting up PostgreSQL may take a long time. In case we are the leader we may want to fail over to."""
@@ -1709,15 +1720,15 @@
         # state_handler.state == 'starting' here
         if self.has_lock():
             if not self.update_lock():
                 logger.info("Lost lock while starting up. Demoting self.")
                 self.demote('immediate-nolock')
                 return 'stopped PostgreSQL while starting up because leader key was lost'
 
-            timeout = self._start_timeout or self.global_config.primary_start_timeout
+            timeout = self._start_timeout or global_config.primary_start_timeout
             time_left = timeout - self.state_handler.time_in_state()
 
             if time_left <= 0:
                 if self.is_failover_possible():
                     logger.info("Demoting self because primary startup is taking too long")
                     self.demote('immediate')
                     return 'stopped PostgreSQL because of startup timeout'
@@ -1742,16 +1753,16 @@
         self._start_timeout = value
 
     def _run_cycle(self) -> str:
         dcs_failed = False
         try:
             try:
                 self.load_cluster_from_dcs()
-                self.global_config = self.patroni.config.get_global_config(self.cluster)
-                self.state_handler.reset_cluster_info_state(self.cluster, self.patroni.nofailover, self.global_config)
+                global_config.update(self.cluster)
+                self.state_handler.reset_cluster_info_state(self.cluster, self.patroni)
             except Exception:
                 self.state_handler.reset_cluster_info_state(None)
                 raise
 
             if self.is_paused():
                 self.watchdog.disable()
                 self._was_paused = True
@@ -1763,18 +1774,18 @@
                     self._rewind.reset_state()
                 self._was_paused = False
 
             if not self.cluster.has_member(self.state_handler.name):
                 self.touch_member()
 
             # cluster has leader key but not initialize key
-            if not (self.cluster.is_unlocked() or self.sysid_valid(self.cluster.initialize)) and self.has_lock():
+            if self.has_lock(False) and not self.sysid_valid(self.cluster.initialize):
                 self.dcs.initialize(create_new=(self.cluster.initialize is None), sysid=self.state_handler.sysid)
 
-            if not (self.cluster.is_unlocked() or self.cluster.config and self.cluster.config.data) and self.has_lock():
+            if self.has_lock(False) and not (self.cluster.config and self.cluster.config.data):
                 self.dcs.set_config_value(json.dumps(self.patroni.config.dynamic_configuration, separators=(',', ':')))
                 self.cluster = self.dcs.get_cluster()
 
             if self._async_executor.busy:
                 return self.handle_long_action_in_progress()
 
             msg = self.handle_starting_instance()
@@ -1899,15 +1910,15 @@
                     if not is_promoting and not self.state_handler.is_primary():
                         self._rewind.trigger_check_diverged_lsn()
                     self.state_handler.call_nowait(CallbackAction.ON_START)
 
                 if not is_promoting and create_slots and self.cluster.leader:
                     err = self._async_executor.try_run_async('copy_logical_slots',
                                                              self.state_handler.slots_handler.copy_logical_slots,
-                                                             args=(self.cluster, create_slots))
+                                                             args=(self.cluster, self.patroni, create_slots))
                     if not err:
                         ret = 'Copying logical slots {0} from the primary'.format(create_slots)
             return ret
         except DCSError:
             dcs_failed = True
             logger.error('Error communicating with DCS')
             return self._handle_dcs_error()
@@ -1955,18 +1966,15 @@
         # It could be that DCS is read-only, or only the leader can't access it.
         # Only the second one could be handled by `load_cluster_from_dcs()`.
         # The first one affects advancing logical replication slots on replicas, therefore we rely on
         # Failsafe.update_cluster(), that will return "modified" Cluster if failsafe mode is active.
         cluster = self._failsafe.update_cluster(self.cluster)\
             if self.is_failsafe_mode() and not self.is_leader() else self.cluster
         if cluster:
-            slots = self.state_handler.slots_handler.sync_replication_slots(cluster,
-                                                                            self.patroni.nofailover,
-                                                                            self.patroni.replicatefrom,
-                                                                            self.is_paused())
+            slots = self.state_handler.slots_handler.sync_replication_slots(cluster, self.patroni)
         # Don't copy replication slots if failsafe_mode is active
         return [] if self.failsafe_is_active() else slots
 
     def run_cycle(self) -> str:
         with self._async_executor:
             try:
                 info = self._run_cycle()
@@ -2000,15 +2008,15 @@
                     if self.is_failover_possible(cluster_lsn=checkpoint_location):
                         self.dcs.delete_leader(self.cluster.leader, prev_location)
                         status['deleted'] = True
                     else:
                         self.dcs.write_leader_optime(prev_location)
 
             def _before_shutdown() -> None:
-                self.notify_citus_coordinator('before_demote')
+                self.notify_mpp_coordinator('before_demote')
 
             on_shutdown = _on_shutdown if self.is_leader() else None
             before_shutdown = _before_shutdown if self.is_leader() else None
             self.while_not_sync_standby(lambda: self.state_handler.stop(checkpoint=False, on_safepoint=disable_wd,
                                                                         on_shutdown=on_shutdown,
                                                                         before_shutdown=before_shutdown,
                                                                         stop_timeout=self.primary_stop_timeout()))
@@ -2042,15 +2050,15 @@
     def get_remote_member(self, member: Union[Leader, Member, None] = None) -> RemoteMember:
         """Get remote member node to stream from.
 
         In case of standby cluster this will tell us from which remote member to stream. Config can be both patroni
         config or cluster.config.data.
         """
         data: Dict[str, Any] = {}
-        cluster_params = self.global_config.get_standby_cluster_config()
+        cluster_params = global_config.get_standby_cluster_config()
 
         if cluster_params:
             data.update({k: v for k, v in cluster_params.items() if k in RemoteMember.ALLOWED_KEYS})
             data['no_replication_slot'] = 'primary_slot_name' not in cluster_params
             conn_kwargs = member.conn_kwargs() if member else \
                 {k: cluster_params[k] for k in ('host', 'port') if k in cluster_params}
             if conn_kwargs:
```

### Comparing `patroni-3.2.2/patroni/postgresql/__init__.py` & `patroni-3.3.0/patroni/postgresql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 from typing import Any, Callable, Dict, Iterator, List, Optional, Union, Tuple, TYPE_CHECKING
 
 from .bootstrap import Bootstrap
 from .callback_executor import CallbackAction, CallbackExecutor
 from .cancellable import CancellableSubprocess
 from .config import ConfigHandler, mtime
 from .connection import ConnectionPool, get_connection_cursor
-from .citus import CitusHandler
 from .misc import parse_history, parse_lsn, postgres_major_version_to_int
+from .mpp import AbstractMPP
 from .postmaster import PostmasterProcess
 from .slots import SlotsHandler
 from .sync import SyncHandler
-from .. import psycopg
+from .. import global_config, psycopg
 from ..async_executor import CriticalTask
-from ..collections import CaseInsensitiveSet
+from ..collections import CaseInsensitiveSet, CaseInsensitiveDict, EMPTY_DICT
 from ..dcs import Cluster, Leader, Member, SLOT_ADVANCE_AVAILABLE_VERSION
 from ..exceptions import PostgresConnectionException
 from ..utils import Retry, RetryFailedError, polling_loop, data_directory_is_empty, parse_int
+from ..tags import Tags
 
 if TYPE_CHECKING:  # pragma: no cover
     from psycopg import Connection as Connection3, Cursor
     from psycopg2 import connection as connection3, cursor
-    from ..config import GlobalConfig
 
 logger = logging.getLogger(__name__)
 
 STATE_RUNNING = 'running'
 STATE_REJECT = 'rejecting connections'
 STATE_NO_RESPONSE = 'not responding'
 STATE_UNKNOWN = 'unknown'
@@ -59,33 +59,32 @@
               "pg_catalog.pg_current_{0}_{1}()), 1, 8))::bit(32)::int END, "  # primary timeline
               "CASE WHEN pg_catalog.pg_is_in_recovery() THEN 0 ELSE "
               "pg_catalog.pg_{0}_{1}_diff(pg_catalog.pg_current_{0}{2}_{1}(), '0/0')::bigint END, "  # wal(_flush)?_lsn
               "pg_catalog.pg_{0}_{1}_diff(pg_catalog.pg_last_{0}_replay_{1}(), '0/0')::bigint, "
               "pg_catalog.pg_{0}_{1}_diff(COALESCE(pg_catalog.pg_last_{0}_receive_{1}(), '0/0'), '0/0')::bigint, "
               "pg_catalog.pg_is_in_recovery() AND pg_catalog.pg_is_{0}_replay_paused()")
 
-    def __init__(self, config: Dict[str, Any]) -> None:
+    def __init__(self, config: Dict[str, Any], mpp: AbstractMPP) -> None:
         self.name: str = config['name']
         self.scope: str = config['scope']
         self._data_dir: str = config['data_dir']
         self._database = config.get('database', 'postgres')
         self._version_file = os.path.join(self._data_dir, 'PG_VERSION')
         self._pg_control = os.path.join(self._data_dir, 'global', 'pg_control')
         self.connection_string: str
         self.proxy_url: Optional[str]
         self._major_version = self.get_major_version()
-        self._global_config = None
 
         self._state_lock = Lock()
         self.set_state('stopped')
 
-        self._pending_restart = False
+        self._pending_restart_reason = CaseInsensitiveDict()
         self.connection_pool = ConnectionPool()
         self._connection = self.connection_pool.get('heartbeat')
-        self.citus_handler = CitusHandler(self, config.get('citus'))
+        self.mpp_handler = mpp.get_handler_impl(self)
         self.config = ConfigHandler(self, config)
         self.config.check_directories()
 
         self._bin_dir = config.get('bin_dir') or ''
         self.bootstrap = Bootstrap(self)
         self.bootstrapping = False
         self.__thread_ident = current_thread().ident
@@ -215,15 +214,15 @@
                          "(SELECT pg_catalog.json_agg(r.*) FROM (SELECT w.pid as pid, application_name, sync_state,"
                          " pg_catalog.pg_{0}_{1}_diff(write_{1}, '0/0')::bigint AS write_lsn,"
                          " pg_catalog.pg_{0}_{1}_diff(flush_{1}, '0/0')::bigint AS flush_lsn,"
                          " pg_catalog.pg_{0}_{1}_diff(replay_{1}, '0/0')::bigint AS replay_lsn "
                          "FROM pg_catalog.pg_stat_get_wal_senders() w,"
                          " pg_catalog.pg_stat_get_activity(w.pid)"
                          " WHERE w.state = 'streaming') r)").format(self.wal_name, self.lsn_name)
-                        if (not self.global_config or self.global_config.is_synchronous_mode)
+                        if global_config.is_synchronous_mode
                         and self.role in ('master', 'primary', 'promoted') else "'on', '', NULL")
 
         if self._major_version >= 90600:
             extra = ("pg_catalog.current_setting('restore_command')" if self._major_version >= 120000 else "NULL") +\
                 ", " + ("(SELECT pg_catalog.json_agg(s.*) FROM (SELECT slot_name, slot_type as type, datoid::bigint, "
                         "plugin, catalog_xmin, pg_catalog.pg_wal_lsn_diff(confirmed_flush_lsn, '0/0')::bigint"
                         " AS confirmed_flush_lsn, pg_catalog.pg_wal_lsn_diff(restart_lsn, '0/0')::bigint"
@@ -269,15 +268,15 @@
             If ``postgresql.bin_name.*cmd*`` was configured by the user then that binary name is used, otherwise the
             default binary name *cmd* is used.
 
         :param cmd: the Postgres binary name to get path to.
 
         :returns: path to Postgres binary named *cmd*.
         """
-        return os.path.join(self._bin_dir, (self.config.get('bin_name', {}) or {}).get(cmd, cmd))
+        return os.path.join(self._bin_dir, (self.config.get('bin_name', {}) or EMPTY_DICT).get(cmd, cmd))
 
     def pg_ctl(self, cmd: str, *args: str, **kwargs: Any) -> bool:
         """Builds and executes pg_ctl command
 
         :returns: `!True` when return_code == 0, otherwise `!False`"""
 
         pg_ctl = [self.pgcommand('pg_ctl'), cmd]
@@ -318,19 +317,30 @@
         return return_codes.get(ret, STATE_UNKNOWN)
 
     def reload_config(self, config: Dict[str, Any], sighup: bool = False) -> None:
         self.config.reload_config(config, sighup)
         self._is_leader_retry.deadline = self.retry.deadline = config['retry_timeout'] / 2.0
 
     @property
-    def pending_restart(self) -> bool:
-        return self._pending_restart
+    def pending_restart_reason(self) -> CaseInsensitiveDict:
+        """Get :attr:`_pending_restart_reason` value.
 
-    def set_pending_restart(self, value: bool) -> None:
-        self._pending_restart = value
+        :attr:`_pending_restart_reason` is a :class:`CaseInsensitiveDict` object of the PG parameters that are
+        causing pending restart state. Every key is a parameter name, value - a dictionary containing the old
+        and the new value (see :func:`~patroni.postgresql.config.get_param_diff`).
+        """
+        return self._pending_restart_reason
+
+    def set_pending_restart_reason(self, diff_dict: CaseInsensitiveDict) -> None:
+        """Set new or update current :attr:`_pending_restart_reason`.
+
+        :param diff_dict: :class:``CaseInsensitiveDict`` object with the parameters that are causing pending restart
+            state with the diff of their values. Used to reset/update the :attr:`_pending_restart_reason`.
+        """
+        self._pending_restart_reason = diff_dict
 
     @property
     def sysid(self) -> str:
         if not self._sysid and not self.bootstrapping:
             data = self.controldata()
             self._sysid = data.get('Database system identifier', '')
         return self._sysid
@@ -400,15 +410,15 @@
 
     def data_directory_empty(self) -> bool:
         if self.pg_control_exists():
             return False
         return data_directory_is_empty(self._data_dir)
 
     def replica_method_options(self, method: str) -> Dict[str, Any]:
-        return deepcopy(self.config.get(method, {}) or {})
+        return deepcopy(self.config.get(method, {}) or EMPTY_DICT.copy())
 
     def replica_method_can_work_without_replication_connection(self, method: str) -> bool:
         return method != 'basebackup' and bool(self.replica_method_options(method).get('no_master')
                                                or self.replica_method_options(method).get('no_leader'))
 
     def can_create_replica_without_replication_connection(self, replica_methods: Optional[List[str]]) -> bool:
         """ go through the replication methods to see if there are ones
@@ -426,54 +436,38 @@
         # If we enable or disable the hot_standby_feedback we need to update postgresql.conf and reload
         if self._enforce_hot_standby_feedback != value:
             self._enforce_hot_standby_feedback = value
             if self.is_running():
                 self.config.write_postgresql_conf()
                 self.reload()
 
-    @property
-    def global_config(self) -> Optional['GlobalConfig']:
-        return self._global_config
-
-    def reset_cluster_info_state(self, cluster: Union[Cluster, None], nofailover: bool = False,
-                                 global_config: Optional['GlobalConfig'] = None) -> None:
+    def reset_cluster_info_state(self, cluster: Optional[Cluster], tags: Optional[Tags] = None) -> None:
         """Reset monitoring query cache.
 
-        It happens in the beginning of heart-beat loop and on change of `synchronous_standby_names`.
+        .. note::
+            It happens in the beginning of heart-beat loop and on change of `synchronous_standby_names`.
 
         :param cluster: currently known cluster state from DCS
-        :param nofailover: whether this node could become a new primary.
-                           Important when there are logical permanent replication slots because "nofailover"
-                           node could do cascading replication and should enable `hot_standby_feedback`
-        :param global_config: last known :class:`GlobalConfig` object
+        :param tags: reference to an object implementing :class:`Tags` interface.
         """
         self._cluster_info_state = {}
 
-        if global_config:
-            self._global_config = global_config
-
-        if not self._global_config:
+        if not tags:
             return
 
-        if self._global_config.is_standby_cluster:
+        if global_config.is_standby_cluster:
             # Standby cluster can't have logical replication slots, and we don't need to enforce hot_standby_feedback
             self.set_enforce_hot_standby_feedback(False)
 
         if cluster and cluster.config and cluster.config.modify_version:
             # We want to enable hot_standby_feedback if the replica is supposed
             # to have a logical slot or in case if it is the cascading replica.
-            self.set_enforce_hot_standby_feedback(not self._global_config.is_standby_cluster and self.can_advance_slots
-                                                  and cluster.should_enforce_hot_standby_feedback(self.name,
-                                                                                                  nofailover))
-
-            self._has_permanent_slots = cluster.has_permanent_slots(
-                my_name=self.name,
-                is_standby_cluster=self._global_config.is_standby_cluster,
-                nofailover=nofailover,
-                major_version=self.major_version)
+            self.set_enforce_hot_standby_feedback(not global_config.is_standby_cluster and self.can_advance_slots
+                                                  and cluster.should_enforce_hot_standby_feedback(self, tags))
+            self._has_permanent_slots = cluster.has_permanent_slots(self, tags)
 
     def _cluster_info_state_get(self, name: str) -> Optional[Any]:
         if not self._cluster_info_state:
             try:
                 result = self._is_leader_retry(self._query, self.cluster_info_query)[0]
                 cluster_info_state = dict(zip(['timeline', 'wal_position', 'replayed_location',
                                                'received_location', 'replay_paused', 'pg_control_timeline',
@@ -740,15 +734,15 @@
 
         if not block_callbacks:
             self.__cb_pending = CallbackAction.ON_START
 
         self.set_role(role or self.get_postgres_role_from_data_directory())
 
         self.set_state('starting')
-        self._pending_restart = False
+        self.set_pending_restart_reason(CaseInsensitiveDict())
 
         try:
             if not self.ensure_major_version_is_known():
                 return None
             configuration = self.config.effective_configuration
         except Exception:
             return None
@@ -1210,15 +1204,15 @@
             logger.info("PostgreSQL promote cancelled.")
             return False
 
         if before_promote is not None:
             before_promote()
 
         self.slots_handler.on_promote()
-        self.citus_handler.schedule_cache_rebuild()
+        self.mpp_handler.schedule_cache_rebuild()
 
         ret = self.pg_ctl('promote', '-W')
         if ret:
             self.set_role('promoted')
             self.call_nowait(CallbackAction.ON_ROLE_CHANGE)
             ret = self._wait_promote(wait_seconds)
         return ret
@@ -1357,15 +1351,15 @@
             After coming out of pause we have to:
             1. configure server parameters if necessary
             2. sync replication slots, because it might happen that slots were removed
             3. get new 'Database system identifier' to make sure that it wasn't changed
         """
         self.ensure_major_version_is_known()
         self.slots_handler.schedule()
-        self.citus_handler.schedule_cache_rebuild()
+        self.mpp_handler.schedule_cache_rebuild()
         self._sysid = ''
 
     def _get_gucs(self) -> CaseInsensitiveSet:
         """Get all available GUCs based on ``postgres --describe-config`` output.
 
         :returns: all available GUCs in the local Postgres server.
         """
```

### Comparing `patroni-3.2.2/patroni/postgresql/available_parameters/0_postgres.yml` & `patroni-3.3.0/patroni/postgresql/available_parameters/0_postgres.yml`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/postgresql/bootstrap.py` & `patroni-3.3.0/patroni/postgresql/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import shlex
 import tempfile
 import time
 
 from typing import Any, Callable, Dict, List, Optional, Union, Tuple, TYPE_CHECKING
 
 from ..async_executor import CriticalTask
+from ..collections import EMPTY_DICT
 from ..dcs import Leader, Member, RemoteMember
 from ..psycopg import quote_ident, quote_literal
 from ..utils import deep_compare, unquote
 
 if TYPE_CHECKING:  # pragma: no cover
     from . import Postgresql
 
@@ -96,18 +97,19 @@
                     user_options.append('--{0}={1}'.format(key, unquote(val)))
         elif isinstance(options, list):
             for opt in options:
                 if isinstance(opt, str) and option_is_allowed(opt):
                     user_options.append('--{0}'.format(opt))
                 elif isinstance(opt, dict):
                     keys = list(opt.keys())
-                    if len(keys) != 1 or not isinstance(opt[keys[0]], str) or not option_is_allowed(keys[0]):
+                    if len(keys) == 1 and isinstance(opt[keys[0]], str) and option_is_allowed(keys[0]):
+                        user_options.append('--{0}={1}'.format(keys[0], unquote(opt[keys[0]])))
+                    else:
                         error_handler('Error when parsing {0} key-value option {1}: only one key-value is allowed'
                                       ' and value should be a string'.format(tool, opt[keys[0]]))
-                    user_options.append('--{0}={1}'.format(keys[0], unquote(opt[keys[0]])))
                 else:
                     error_handler('Error when parsing {0} option {1}: value should be string value'
                                   ' or a single key-value pair'.format(tool, opt))
         else:
             error_handler('{0} options must be list or dict'.format(tool))
         return user_options
 
@@ -141,15 +143,15 @@
 
     def _post_restore(self) -> None:
         self._postgresql.config.restore_configuration_files()
         self._postgresql.configure_server_parameters()
 
         # make sure there is no trigger file or postgres will be automatically promoted
         trigger_file = self._postgresql.config.triggerfile_good_name
-        trigger_file = (self._postgresql.config.get('recovery_conf') or {}).get(trigger_file) or 'promote'
+        trigger_file = (self._postgresql.config.get('recovery_conf') or EMPTY_DICT).get(trigger_file) or 'promote'
         trigger_file = os.path.abspath(os.path.join(self._postgresql.data_dir, trigger_file))
         if os.path.exists(trigger_file):
             os.unlink(trigger_file)
 
     def _custom_bootstrap(self, config: Any) -> bool:
         """Bootstrap a fresh Patroni cluster using a custom method provided by the user.
 
@@ -436,15 +438,15 @@
     GRANT EXECUTE ON function pg_catalog.{0} TO {1};
 END;$$""".format(f, quote_ident(rewind['username'], postgresql.connection()))
                         postgresql.query(sql)
 
                 if config.get('users'):
                     logger.warning('User creation via "bootstrap.users" will be removed in v4.0.0')
 
-                for name, value in (config.get('users') or {}).items():
+                for name, value in (config.get('users') or EMPTY_DICT).items():
                     if all(name != a.get('username') for a in (superuser, replication, rewind)):
                         self.create_or_update_role(name, value.get('password'), value.get('options', []))
 
                 # We were doing a custom bootstrap instead of running initdb, therefore we opened trust
                 # access from certain addresses to be able to reach cluster and change password
                 if self._running_custom_bootstrap:
                     self._running_custom_bootstrap = False
@@ -459,20 +461,20 @@
                     # at this point there should be no recovery.conf
                     postgresql.config.remove_recovery_conf()
 
                     if postgresql.config.hba_file:
                         postgresql.restart()
                     else:
                         postgresql.config.replace_pg_hba()
-                        if postgresql.pending_restart:
+                        if postgresql.pending_restart_reason:
                             postgresql.restart()
                         else:
                             postgresql.reload()
                             time.sleep(1)  # give a time to postgres to "reload" configuration files
                             postgresql.connection().close()  # close connection to reconnect with a new password
                 else:  # initdb
-                    # We may want create database and extension for citus
-                    self._postgresql.citus_handler.bootstrap()
+                    # We may want create database and extension for some MPP clusters
+                    self._postgresql.mpp_handler.bootstrap()
         except Exception:
             logger.exception('post_bootstrap')
             task.complete(False)
         return task.result
```

### Comparing `patroni-3.2.2/patroni/postgresql/callback_executor.py` & `patroni-3.3.0/patroni/postgresql/callback_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/postgresql/cancellable.py` & `patroni-3.3.0/patroni/postgresql/cancellable.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,16 @@
                     raise PostgresException('cancelled')
 
                 self._is_cancelled = False
                 started = self._start_process(*args, **kwargs)
 
             if started and self._process is not None:
                 if isinstance(communicate, dict):
-                    communicate['stdout'], communicate['stderr'] = self._process.communicate(input_data)
+                    communicate['stdout'], communicate['stderr'] = \
+                        self._process.communicate(input_data)  # pyright: ignore [reportGeneralTypeIssues]
                 return self._process.wait()
         finally:
             with self._lock:
                 self._process = None
             self._kill_children()
 
     def reset_is_cancelled(self) -> None:
```

### Comparing `patroni-3.2.2/patroni/postgresql/citus.py` & `patroni-3.3.0/patroni/postgresql/mpp/citus.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 import re
 import time
 
 from threading import Condition, Event, Thread
 from urllib.parse import urlparse
 from typing import Any, Dict, List, Optional, Union, Tuple, TYPE_CHECKING
 
-from ..dcs import CITUS_COORDINATOR_GROUP_ID, Cluster
-from ..psycopg import connect, quote_ident, ProgrammingError
+from . import AbstractMPP, AbstractMPPHandler
+from ...dcs import Cluster
+from ...psycopg import connect, quote_ident, ProgrammingError
+from ...utils import parse_int
 
 if TYPE_CHECKING:  # pragma: no cover
-    from . import Postgresql
+    from .. import Postgresql
 
+CITUS_COORDINATOR_GROUP_ID = 0
 CITUS_SLOT_NAME_RE = re.compile(r'^citus_shard_(move|split)_slot(_[1-9][0-9]*){2,3}$')
 logger = logging.getLogger(__name__)
 
 
 class PgDistNode(object):
     """Represents a single row in the `pg_dist_node` table"""
 
@@ -59,45 +62,69 @@
         return ('PgDistNode(nodeid={0},group={1},host={2},port={3},event={4})'
                 .format(self.nodeid, self.group, self.host, self.port, self.event))
 
     def __repr__(self) -> str:
         return str(self)
 
 
-class CitusHandler(Thread):
+class Citus(AbstractMPP):
 
-    def __init__(self, postgresql: 'Postgresql', config: Optional[Dict[str, Union[str, int]]]) -> None:
-        super(CitusHandler, self).__init__()
+    group_re = re.compile('^(0|[1-9][0-9]*)$')
+
+    @staticmethod
+    def validate_config(config: Union[Any, Dict[str, Union[str, int]]]) -> bool:
+        """Check whether provided config is good for a given MPP.
+
+        :param config: configuration of ``citus`` MPP section.
+
+        :returns: ``True`` is config passes validation, otherwise ``False``.
+        """
+        return isinstance(config, dict) \
+            and isinstance(config.get('database'), str) \
+            and parse_int(config.get('group')) is not None
+
+    @property
+    def group(self) -> int:
+        """The group of this Citus node."""
+        return int(self._config['group'])
+
+    @property
+    def coordinator_group_id(self) -> int:
+        """The group id of the Citus coordinator PostgreSQL cluster."""
+        return CITUS_COORDINATOR_GROUP_ID
+
+
+class CitusHandler(Citus, AbstractMPPHandler, Thread):
+    """Define the interfaces for handling an underlying Citus cluster."""
+
+    def __init__(self, postgresql: 'Postgresql', config: Dict[str, Union[str, int]]) -> None:
+        """"Initialize a new instance of :class:`CitusHandler`.
+
+        :param postgresql: the Postgres node.
+        :param config: the ``citus`` MPP config section.
+        """
+        Thread.__init__(self)
+        AbstractMPPHandler.__init__(self, postgresql, config)
         self.daemon = True
-        self._postgresql = postgresql
-        self._config = config
         if config:
             self._connection = postgresql.connection_pool.get(
                 'citus', {'dbname': config['database'],
                           'options': '-c statement_timeout=0 -c idle_in_transaction_session_timeout=0'})
         self._pg_dist_node: Dict[int, PgDistNode] = {}  # Cache of pg_dist_node: {groupid: PgDistNode()}
         self._tasks: List[PgDistNode] = []  # Requests to change pg_dist_node, every task is a `PgDistNode`
         self._in_flight: Optional[PgDistNode] = None  # Reference to the `PgDistNode` being changed in a transaction
         self._schedule_load_pg_dist_node = True  # Flag that "pg_dist_node" should be queried from the database
         self._condition = Condition()  # protects _pg_dist_node, _tasks, _in_flight, and _schedule_load_pg_dist_node
         self.schedule_cache_rebuild()
 
-    def is_enabled(self) -> bool:
-        return isinstance(self._config, dict)
-
-    def group(self) -> Optional[int]:
-        return int(self._config['group']) if isinstance(self._config, dict) else None
-
-    def is_coordinator(self) -> bool:
-        return self.is_enabled() and self.group() == CITUS_COORDINATOR_GROUP_ID
-
-    def is_worker(self) -> bool:
-        return self.is_enabled() and not self.is_coordinator()
-
     def schedule_cache_rebuild(self) -> None:
+        """Cache rebuild handler.
+
+        Is called to notify handler that it has to refresh its metadata cache from the database.
+        """
         with self._condition:
             self._schedule_load_pg_dist_node = True
 
     def on_demote(self) -> None:
         with self._condition:
             self._pg_dist_node.clear()
             empty_tasks: List[PgDistNode] = []
@@ -130,16 +157,16 @@
         except Exception:
             return False
 
         with self._condition:
             self._pg_dist_node = {r[1]: PgDistNode(r[1], r[2], r[3], 'after_promote', r[0]) for r in rows}
         return True
 
-    def sync_pg_dist_node(self, cluster: Cluster) -> None:
-        """Maintain the `pg_dist_node` from the coordinator leader every heartbeat loop.
+    def sync_meta_data(self, cluster: Cluster) -> None:
+        """Maintain the ``pg_dist_node`` from the coordinator leader every heartbeat loop.
 
         We can't always rely on REST API calls from worker nodes in order
         to maintain `pg_dist_node`, therefore at least once per heartbeat
         loop we make sure that workes registered in `self._pg_dist_node`
         cache are matching the cluster view from DCS by creating tasks
         the same way as it is done from the REST API."""
 
@@ -292,24 +319,24 @@
             except Exception:
                 logger.exception('run')
 
     def _add_task(self, task: PgDistNode) -> bool:
         with self._condition:
             i = self.find_task_by_group(task.group)
 
-            # The `PgDistNode.timeout` == None is an indicator that it was scheduled from the sync_pg_dist_node().
+            # The `PgDistNode.timeout` == None is an indicator that it was scheduled from the sync_meta_data().
             if task.timeout is None:
                 # We don't want to override the already existing task created from REST API.
                 if i is not None and self._tasks[i].timeout is not None:
                     return False
 
                 # There is a little race condition with tasks created from REST API - the call made "before" the member
-                # key is updated in DCS. Therefore it is possible that :func:`sync_pg_dist_node` will try to create a
-                # task based on the outdated values of "state"/"role". To solve it we introduce an artificial timeout.
-                # Only when the timeout is reached new tasks could be scheduled from sync_pg_dist_node()
+                # key is updated in DCS. Therefore it is possible that :func:`sync_meta_data` will try to create a task
+                # based on the outdated values of "state"/"role". To solve it we introduce an artificial timeout.
+                # Only when the timeout is reached new tasks could be scheduled from sync_meta_data()
                 if self._in_flight and self._in_flight.group == task.group and self._in_flight.timeout is not None\
                         and self._in_flight.deadline > time.time():
                     return False
 
             # Override already existing task for the same worker group
             if i is not None:
                 if task != self._tasks[i]:
@@ -349,17 +376,18 @@
         task = self.add_task(event['type'], event['group'],
                              worker.leader.conn_url,
                              event['timeout'], event['cooldown'] * 1000)
         if task and event['type'] == 'before_demote':
             task.wait()
 
     def bootstrap(self) -> None:
-        if not isinstance(self._config, dict):  # self.is_enabled()
-            return
+        """Bootstrap handler.
 
+        Is called when the new cluster is initialized (through ``initdb`` or a custom bootstrap method).
+        """
         conn_kwargs = {**self._postgresql.connection_pool.conn_kwargs,
                        'options': '-c synchronous_commit=local -c statement_timeout=0'}
         if self._config['database'] != self._postgresql.database:
             conn = connect(**conn_kwargs)
             try:
                 with conn.cursor() as cur:
                     cur.execute('CREATE DATABASE {0}'.format(
@@ -389,17 +417,18 @@
                     r = urlparse(self._postgresql.connection_string)
                     cur.execute("SELECT pg_catalog.citus_set_coordinator_host(%s, %s, 'primary', 'default')",
                                 (r.hostname, r.port or 5432))
         finally:
             conn.close()
 
     def adjust_postgres_gucs(self, parameters: Dict[str, Any]) -> None:
-        if not self.is_enabled():
-            return
+        """Adjust GUCs in the current PostgreSQL configuration.
 
+        :param parameters: dictionary of GUCs, with key as GUC name and the corresponding value as current GUC value.
+        """
         # citus extension must be on the first place in shared_preload_libraries
         shared_preload_libraries = list(filter(
             lambda el: el and el != 'citus',
             [p.strip() for p in parameters.get('shared_preload_libraries', '').split(',')]))
         parameters['shared_preload_libraries'] = ','.join(['citus'] + shared_preload_libraries)
 
         # if not explicitly set Citus overrides max_prepared_transactions to max_connections*2
@@ -409,12 +438,22 @@
         # Resharding in Citus implemented using logical replication
         parameters['wal_level'] = 'logical'
 
         # Sometimes Citus needs to connect to the local postgres. We will do it the same way as Patroni does.
         parameters['citus.local_hostname'] = self._postgresql.connection_pool.conn_kwargs.get('host', 'localhost')
 
     def ignore_replication_slot(self, slot: Dict[str, str]) -> bool:
-        if isinstance(self._config, dict) and self._postgresql.is_primary() and\
-                slot['type'] == 'logical' and slot['database'] == self._config['database']:
+        """Check whether provided replication *slot* existing in the database should not be removed.
+
+        .. note::
+            MPP database may create replication slots for its own use, for example to migrate data between workers
+            using logical replication, and we don't want to suddenly drop them.
+
+        :param slot: dictionary containing the replication slot settings, like ``name``, ``database``, ``type``, and
+                     ``plugin``.
+
+        :returns: ``True`` if the replication slots should not be removed, otherwise ``False``.
+        """
+        if self._postgresql.is_primary() and slot['type'] == 'logical' and slot['database'] == self._config['database']:
             m = CITUS_SLOT_NAME_RE.match(slot['name'])
             return bool(m and {'move': 'pgoutput', 'split': 'citus'}.get(m.group(1)) == slot['plugin'])
         return False
```

### Comparing `patroni-3.2.2/patroni/postgresql/config.py` & `patroni-3.3.0/patroni/postgresql/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 import socket
 import stat
 import time
 
 from contextlib import contextmanager
 from urllib.parse import urlparse, parse_qsl, unquote
 from types import TracebackType
-from typing import Any, Collection, Dict, Iterator, List, Optional, Union, Tuple, Type, TYPE_CHECKING
+from typing import Any, Callable, Collection, Dict, Iterator, List, Optional, Union, Tuple, Type, TYPE_CHECKING
 
 from .validator import recovery_parameters, transform_postgresql_parameter_value, transform_recovery_parameter_value
-from ..collections import CaseInsensitiveDict, CaseInsensitiveSet
+from .. import global_config
+from ..collections import CaseInsensitiveDict, CaseInsensitiveSet, EMPTY_DICT
 from ..dcs import Leader, Member, RemoteMember, slot_name_from_member_name
 from ..exceptions import PatroniFatalException, PostgresConnectionException
 from ..file_perm import pg_perm
-from ..utils import compare_values, parse_bool, parse_int, split_host_port, uri, validate_directory, is_subpath
+from ..utils import (compare_values, maybe_convert_from_base_unit, parse_bool, parse_int,
+                     split_host_port, uri, validate_directory, is_subpath)
 from ..validator import IntValidator, EnumValidator
 
 if TYPE_CHECKING:  # pragma: no cover
     from . import Postgresql
 
 logger = logging.getLogger(__name__)
 
@@ -265,14 +267,37 @@
     return parse_bool(value) is not None
 
 
 def _bool_is_true_validator(value: Any) -> bool:
     return parse_bool(value) is True
 
 
+def get_param_diff(old_value: Any, new_value: Any,
+                   vartype: Optional[str] = None, unit: Optional[str] = None) -> Dict[str, str]:
+    """Get a dictionary representing a single PG parameter's value diff.
+
+    :param old_value: current :class:`str` parameter value.
+    :param new_value: :class:`str` value of the paramater after a restart.
+    :param vartype: the target type to parse old/new_value. See ``vartype`` argument of
+        :func:`~patroni.utils.maybe_convert_from_base_unit`.
+    :param unit: unit of *old/new_value*. See ``base_unit`` argument of
+        :func:`~patroni.utils.maybe_convert_from_base_unit`.
+
+    :returns: a :class:`dict` object that contains two keys: ``old_value`` and ``new_value``
+        with their values casted to :class:`str` and converted from base units (if possible).
+    """
+    str_value: Callable[[Any], str] = lambda x: '' if x is None else str(x)
+    return {
+        'old_value': (maybe_convert_from_base_unit(str_value(old_value), vartype, unit)
+                      if vartype else str_value(old_value)),
+        'new_value': (maybe_convert_from_base_unit(str_value(new_value), vartype, unit)
+                      if vartype else str_value(new_value))
+    }
+
+
 class ConfigHandler(object):
 
     # List of parameters which must be always passed to postmaster as command line options
     # to make it not possible to change them with 'ALTER SYSTEM'.
     # Some of these parameters have sane default value assigned and Patroni doesn't allow
     # to decrease this value. E.g. 'wal_level' can't be lower then 'hot_standby' and so on.
     # These parameters could be changed only globally, i.e. via DCS.
@@ -590,36 +615,36 @@
                 value = transform_recovery_parameter_value(self._postgresql.major_version, name, value,
                                                            self._postgresql.available_gucs)
                 if value is None:
                     continue
             fd.write_param(name, value)
 
     def build_recovery_params(self, member: Union[Leader, Member, None]) -> CaseInsensitiveDict:
-        recovery_params = CaseInsensitiveDict({p: v for p, v in (self.get('recovery_conf') or {}).items()
+        default: Dict[str, Any] = {}
+        recovery_params = CaseInsensitiveDict({p: v for p, v in (self.get('recovery_conf') or default).items()
                                                if not p.lower().startswith('recovery_target')
                                                and p.lower() not in ('primary_conninfo', 'primary_slot_name')})
         recovery_params.update({'standby_mode': 'on', 'recovery_target_timeline': 'latest'})
         if self._postgresql.major_version >= 120000:
             # on pg12 we want to protect from following params being set in one of included files
             # not doing so might result in a standby being paused, promoted or shutted down.
             recovery_params.update({'recovery_target': '', 'recovery_target_name': '', 'recovery_target_time': '',
                                     'recovery_target_xid': '', 'recovery_target_lsn': ''})
 
         is_remote_member = isinstance(member, RemoteMember)
         primary_conninfo = self.primary_conninfo_params(member)
         if primary_conninfo:
-            use_slots = self.get('use_slots', True) and self._postgresql.major_version >= 90400
+            use_slots = global_config.use_slots and self._postgresql.major_version >= 90400
             if use_slots and not (is_remote_member and member.no_replication_slot):
                 primary_slot_name = member.primary_slot_name if is_remote_member else self._postgresql.name
                 recovery_params['primary_slot_name'] = slot_name_from_member_name(primary_slot_name)
                 # We are a standby leader and are using a replication slot. Make sure we connect to
                 # the leader of the main cluster (in case more than one host is specified in the
                 # connstr) by adding 'target_session_attrs=read-write' to primary_conninfo.
-                if is_remote_member and 'target_sesions_attrs' not in primary_conninfo and\
-                        self._postgresql.major_version >= 100000:
+                if is_remote_member and ',' in primary_conninfo['host'] and self._postgresql.major_version >= 100000:
                     primary_conninfo['target_session_attrs'] = 'read-write'
             recovery_params['primary_conninfo'] = primary_conninfo
 
         # standby_cluster config might have different parameters, we want to override them
         standby_cluster_params = ['restore_command', 'archive_cleanup_command']\
             + (['recovery_min_apply_delay'] if is_remote_member else [])
         recovery_params.update({p: member.data.get(p) for p in standby_cluster_params if member and member.data.get(p)})
@@ -817,15 +842,15 @@
                                   and not self._postgresql.cb_called
                                   and not self._postgresql.is_starting())}
 
         def record_missmatch(mtype: bool) -> None:
             required['restart' if mtype else 'reload'] += 1
 
         wanted_recovery_params = self.build_recovery_params(member)
-        for param, value in (self._current_recovery_params or {}).items():
+        for param, value in (self._current_recovery_params or EMPTY_DICT).items():
             # Skip certain parameters defined in the included postgres config files
             # if we know that they are not specified in the patroni configuration.
             if len(value) > 2 and value[2] not in (self._postgresql_conf, self._auto_conf) and \
                     param in ('archive_cleanup_command', 'promote_trigger_file', 'recovery_end_command',
                               'recovery_min_apply_delay', 'restore_command') and param not in wanted_recovery_params:
                 continue
             if param == 'recovery_min_apply_delay':
@@ -938,18 +963,18 @@
             if self.triggerfile_good_name not in self._config['recovery_conf'] and value:
                 self._config['recovery_conf'][self.triggerfile_good_name] = value
 
     def get_server_parameters(self, config: Dict[str, Any]) -> CaseInsensitiveDict:
         parameters = config['parameters'].copy()
         listen_addresses, port = split_host_port(config['listen'], 5432)
         parameters.update(cluster_name=self._postgresql.scope, listen_addresses=listen_addresses, port=str(port))
-        if not self._postgresql.global_config or self._postgresql.global_config.is_synchronous_mode:
+        if global_config.is_synchronous_mode:
             synchronous_standby_names = self._server_parameters.get('synchronous_standby_names')
             if synchronous_standby_names is None:
-                if self._postgresql.global_config and self._postgresql.global_config.is_synchronous_mode_strict\
+                if global_config.is_synchronous_mode_strict\
                         and self._postgresql.role in ('master', 'primary', 'promoted'):
                     parameters['synchronous_standby_names'] = '*'
                 else:
                     parameters.pop('synchronous_standby_names', None)
             else:
                 parameters['synchronous_standby_names'] = synchronous_standby_names
 
@@ -963,15 +988,15 @@
         if self._postgresql.major_version >= 130000:
             wal_keep_segments = parameters.pop('wal_keep_segments', self.CMDLINE_OPTIONS['wal_keep_segments'][0])
             parameters.setdefault('wal_keep_size', str(int(wal_keep_segments) * 16) + 'MB')
         elif self._postgresql.major_version:
             wal_keep_size = parse_int(parameters.pop('wal_keep_size', self.CMDLINE_OPTIONS['wal_keep_size'][0]), 'MB')
             parameters.setdefault('wal_keep_segments', int(((wal_keep_size or 0) + 8) / 16))
 
-        self._postgresql.citus_handler.adjust_postgres_gucs(parameters)
+        self._postgresql.mpp_handler.adjust_postgres_gucs(parameters)
 
         ret = CaseInsensitiveDict({k: v for k, v in parameters.items() if not self._postgresql.major_version
                                    or self._postgresql.major_version >= self.CMDLINE_OPTIONS.get(k, (0, 1, 90100))[2]})
         ret.update({k: os.path.join(self._config_dir, ret[k]) for k in ('hba_file', 'ident_file') if k in ret})
         return ret
 
     @staticmethod
@@ -1074,15 +1099,16 @@
             del changes['wal_buffers']
 
     def reload_config(self, config: Dict[str, Any], sighup: bool = False) -> None:
         self._superuser = config['authentication'].get('superuser', {})
         server_parameters = self.get_server_parameters(config)
         params_skip_changes = CaseInsensitiveSet((*self._RECOVERY_PARAMETERS, 'hot_standby', 'wal_log_hints'))
 
-        conf_changed = hba_changed = ident_changed = local_connection_address_changed = pending_restart = False
+        conf_changed = hba_changed = ident_changed = local_connection_address_changed = False
+        param_diff = CaseInsensitiveDict()
         if self._postgresql.state == 'running':
             changes = CaseInsensitiveDict({p: v for p, v in server_parameters.items()
                                            if p not in params_skip_changes})
             changes.update({p: None for p in self._server_parameters.keys()
                             if not (p in changes or p in params_skip_changes)})
             if changes:
                 undef = []
@@ -1098,49 +1124,50 @@
 
                 for r in old_values.values():
                     if r[4] != 'internal' and r[0] in changes:
                         new_value = changes.pop(r[0])
                         if new_value is None or not compare_values(r[3], r[2], r[1], new_value):
                             conf_changed = True
                             if r[4] == 'postmaster':
-                                pending_restart = True
-                                logger.info('Changed %s from %s to %s (restart might be required)',
-                                            r[0], r[1], new_value)
+                                param_diff[r[0]] = get_param_diff(r[1], new_value, r[3], r[2])
+                                logger.info("Changed %s from '%s' to '%s' (restart might be required)",
+                                            r[0], param_diff[r[0]]['old_value'], new_value)
                                 if config.get('use_unix_socket') and r[0] == 'unix_socket_directories'\
                                         or r[0] in ('listen_addresses', 'port'):
                                     local_connection_address_changed = True
                             else:
-                                logger.info('Changed %s from %s to %s', r[0], r[1], new_value)
+                                logger.info("Changed %s from '%s' to '%s'",
+                                            r[0], maybe_convert_from_base_unit(r[1], r[3], r[2]), new_value)
                         elif r[0] in self._server_parameters \
                                 and not compare_values(r[3], r[2], r[1], self._server_parameters[r[0]]):
                             # Check if any parameter was set back to the current pg_settings value
                             # We can use pg_settings value here, as it is proved to be equal to new_value
-                            logger.info('Changed %s from %s to %s', r[0], self._server_parameters[r[0]], r[1])
+                            logger.info("Changed %s from '%s' to '%s'", r[0], self._server_parameters[r[0]], new_value)
                             conf_changed = True
                 for param, value in changes.items():
                     if '.' in param:
-                        # Check that user-defined-paramters have changed (parameters with period in name)
+                        # Check that user-defined-parameters have changed (parameters with period in name)
                         if value is None or param not in self._server_parameters \
                                 or str(value) != str(self._server_parameters[param]):
-                            logger.info('Changed %s from %s to %s', param, self._server_parameters.get(param), value)
+                            logger.info("Changed %s from '%s' to '%s'",
+                                        param, self._server_parameters.get(param), value)
                             conf_changed = True
                     elif param in server_parameters:
                         logger.warning('Removing invalid parameter `%s` from postgresql.parameters', param)
                         server_parameters.pop(param)
 
             if (not server_parameters.get('hba_file') or server_parameters['hba_file'] == self._pg_hba_conf) \
                     and config.get('pg_hba'):
                 hba_changed = self._config.get('pg_hba', []) != config['pg_hba']
 
             if (not server_parameters.get('ident_file') or server_parameters['ident_file'] == self._pg_hba_conf) \
                     and config.get('pg_ident'):
                 ident_changed = self._config.get('pg_ident', []) != config['pg_ident']
 
         self._config = config
-        self._postgresql.set_pending_restart(pending_restart)
         self._server_parameters = server_parameters
         self._adjust_recovery_parameters()
         self._krbsrvname = config.get('krbsrvname')
 
         # for not so obvious connection attempts that may happen outside of pyscopg2
         if self._krbsrvname:
             os.environ['PGKRBSRVNAME'] = self._krbsrvname
@@ -1162,24 +1189,36 @@
 
         if sighup or conf_changed or hba_changed or ident_changed:
             logger.info('Reloading PostgreSQL configuration.')
             self._postgresql.reload()
             if self._postgresql.major_version >= 90500:
                 time.sleep(1)
                 try:
-                    pending_restart = self._postgresql.query(
-                        'SELECT COUNT(*) FROM pg_catalog.pg_settings'
-                        ' WHERE pg_catalog.lower(name) != ALL(%s) AND pending_restart',
-                        [n.lower() for n in params_skip_changes])[0][0] > 0
-                    self._postgresql.set_pending_restart(pending_restart)
+                    settings_diff: CaseInsensitiveDict = CaseInsensitiveDict()
+                    for param, value, unit, vartype in self._postgresql.query(
+                            'SELECT name, pg_catalog.current_setting(name), unit, vartype FROM pg_catalog.pg_settings'
+                            ' WHERE pg_catalog.lower(name) != ALL(%s) AND pending_restart',
+                            [n.lower() for n in params_skip_changes]):
+                        new_value = self._postgresql.get_guc_value(param)
+                        new_value = '?' if new_value is None else new_value
+                        settings_diff[param] = get_param_diff(value, new_value, vartype, unit)
+                    external_change = {param: value for param, value in settings_diff.items()
+                                       if param not in param_diff or value != param_diff[param]}
+                    if external_change:
+                        logger.info("PostgreSQL configuration parameters requiring restart"
+                                    " (%s) seem to be changed bypassing Patroni config."
+                                    " Setting 'Pending restart' flag", ', '.join(external_change))
+                    param_diff = settings_diff
                 except Exception as e:
                     logger.warning('Exception %r when running query', e)
         else:
             logger.info('No PostgreSQL configuration items changed, nothing to reload.')
 
+        self._postgresql.set_pending_restart_reason(param_diff)
+
     def set_synchronous_standby_names(self, value: Optional[str]) -> Optional[bool]:
         """Updates synchronous_standby_names and reloads if necessary.
         :returns: True if value was updated."""
         if value != self._server_parameters.get('synchronous_standby_names'):
             if value is None:
                 self._server_parameters.pop('synchronous_standby_names', None)
             else:
@@ -1214,24 +1253,28 @@
 
         if self._postgresql.major_version >= 120000:
             options_mapping['max_wal_senders'] = 'max_wal_senders setting'
 
         data = self._postgresql.controldata()
         effective_configuration = self._server_parameters.copy()
 
+        param_diff = CaseInsensitiveDict()
         for name, cname in options_mapping.items():
             value = parse_int(effective_configuration[name])
             if cname not in data:
                 logger.warning('%s is missing from pg_controldata output', cname)
                 continue
 
             cvalue = parse_int(data[cname])
             if cvalue is not None and value is not None and cvalue > value:
                 effective_configuration[name] = cvalue
-                self._postgresql.set_pending_restart(True)
+                logger.info("%s value in pg_controldata: %d, in the global configuration: %d."
+                            " pg_controldata value will be used. Setting 'Pending restart' flag", name, cvalue, value)
+                param_diff[name] = get_param_diff(cvalue, value)
+        self._postgresql.set_pending_restart_reason(param_diff)
 
         # If we are using custom bootstrap with PITR it could fail when values like max_connections
         # are increased, therefore we disable hot_standby if recovery_target_action == 'promote'.
         if self._postgresql.bootstrap.running_custom_bootstrap:
             disable_hot_standby = False
             if self._postgresql.bootstrap.keep_existing_recovery_conf:
                 disable_hot_standby = True  # trust that pgBackRest does the right thing
@@ -1278,8 +1321,8 @@
     def postgresql_conf(self) -> str:
         return self._postgresql_conf
 
     def get(self, key: str, default: Optional[Any] = None) -> Optional[Any]:
         return self._config.get(key, default)
 
     def restore_command(self) -> Optional[str]:
-        return (self.get('recovery_conf') or {}).get('restore_command')
+        return (self.get('recovery_conf') or EMPTY_DICT).get('restore_command')
```

### Comparing `patroni-3.2.2/patroni/postgresql/connection.py` & `patroni-3.3.0/patroni/postgresql/connection.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/postgresql/misc.py` & `patroni-3.3.0/patroni/postgresql/misc.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/postgresql/postmaster.py` & `patroni-3.3.0/patroni/postgresql/postmaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             return False
         if status == 0:
             return None
         else:
             return not self.is_running()
 
     def wait_for_user_backends_to_close(self, stop_timeout: Optional[float]) -> None:
-        # These regexps are cross checked against versions PostgreSQL 9.1 .. 15
+        # These regexps are cross checked against versions PostgreSQL 9.1 .. 16
         aux_proc_re = re.compile("(?:postgres:)( .*:)? (?:(?:archiver|startup|autovacuum launcher|autovacuum worker|"
                                  "checkpointer|logger|stats collector|wal receiver|wal writer|writer)(?: process  )?|"
                                  "walreceiver|wal sender process|walsender|walwriter|background writer|"
                                  "logical replication launcher|logical replication worker for|bgworker:) ")
 
         try:
             children = self.children()
```

### Comparing `patroni-3.2.2/patroni/postgresql/rewind.py` & `patroni-3.3.0/patroni/postgresql/rewind.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from threading import Lock, Thread
 from typing import Any, Callable, Dict, List, Optional, Union, Tuple
 
 from . import Postgresql
 from .connection import get_connection_cursor
 from .misc import format_lsn, fsync_dir, parse_history, parse_lsn
 from ..async_executor import CriticalTask
+from ..collections import EMPTY_DICT
 from ..dcs import Leader, RemoteMember
 
 logger = logging.getLogger(__name__)
 
 
 class REWIND_STATUS(IntEnum):
     INITIAL = 0
@@ -205,17 +206,18 @@
 
         logger.info('primary: history=%s', '\n'.join(history_show))
 
     def _conn_kwargs(self, member: Union[Leader, RemoteMember], auth: Dict[str, Any]) -> Dict[str, Any]:
         ret = member.conn_kwargs(auth)
         if not ret.get('dbname'):
             ret['dbname'] = self._postgresql.database
-        # Add target_session_attrs in case more than one hostname is specified
-        # (libpq client-side failover) making sure we hit the primary
-        if 'target_session_attrs' not in ret and self._postgresql.major_version >= 100000:
+        # Add target_session_attrs to make sure we hit the primary.
+        # It is not strictly necessary for starting from PostgreSQL v14, which made it possible
+        # to rewind from standby, but doing it from the real primary is always safer.
+        if self._postgresql.major_version >= 100000:
             ret['target_session_attrs'] = 'read-write'
         return ret
 
     def _check_timeline_and_lsn(self, leader: Union[Leader, RemoteMember]) -> None:
         in_recovery, local_timeline, local_lsn = self._get_local_timeline_lsn()
         if local_timeline is None or local_lsn is None:
             return
@@ -413,15 +415,15 @@
     def pg_rewind(self, r: Dict[str, Any]) -> bool:
         # prepare pg_rewind connection
         env = self._postgresql.config.write_pgpass(r)
         env.update(LANG='C', LC_ALL='C', PGOPTIONS='-c statement_timeout=0')
         dsn = self._postgresql.config.format_dsn(r, True)
         logger.info('running pg_rewind from %s', dsn)
 
-        restore_command = (self._postgresql.config.get('recovery_conf') or {}).get('restore_command') \
+        restore_command = (self._postgresql.config.get('recovery_conf') or EMPTY_DICT).get('restore_command') \
             if self._postgresql.major_version < 120000 else self._postgresql.get_guc_value('restore_command')
 
         # Until v15 pg_rewind expected postgresql.conf to be inside $PGDATA, which is not the case on e.g. Debian
         pg_rewind_can_restore = restore_command and (self._postgresql.major_version >= 150000
                                                      or (self._postgresql.major_version >= 130000
                                                          and self._postgresql.config.config_dir
                                                          == self._postgresql.data_dir))
```

### Comparing `patroni-3.2.2/patroni/postgresql/slots.py` & `patroni-3.3.0/patroni/postgresql/slots.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 from collections import defaultdict
 from contextlib import contextmanager
 from threading import Condition, Thread
 from typing import Any, Dict, Iterator, List, Optional, Union, Tuple, TYPE_CHECKING, Collection
 
 from .connection import get_connection_cursor
 from .misc import format_lsn, fsync_dir
+from .. import global_config
 from ..dcs import Cluster, Leader
 from ..file_perm import pg_perm
 from ..psycopg import OperationalError
+from ..tags import Tags
 
 if TYPE_CHECKING:  # pragma: no cover
     from psycopg import Cursor
     from psycopg2 import cursor
     from . import Postgresql
 
 logger = logging.getLogger(__name__)
@@ -285,26 +287,26 @@
     def ignore_replication_slot(self, cluster: Cluster, name: str) -> bool:
         """Check if slot *name* should not be managed by Patroni.
 
         :param cluster: cluster state information object.
         :param name: name of the slot to ignore
 
         :returns: ``True`` if slot *name* matches any slot specified in ``ignore_slots`` configuration,
-                 otherwise will pass through and return result of :meth:`CitusHandler.ignore_replication_slot`.
+                 otherwise will pass through and return result of :meth:`AbstractMPPHandler.ignore_replication_slot`.
         """
         slot = self._replication_slots[name]
         if cluster.config:
-            for matcher in cluster.config.ignore_slots_matchers:
+            for matcher in global_config.ignore_slots_matchers:
                 if (
                         (matcher.get("name") is None or matcher["name"] == name)
                         and all(not matcher.get(a) or matcher[a] == slot.get(a)
                                 for a in ('database', 'plugin', 'type'))
                 ):
                     return True
-        return self._postgresql.citus_handler.ignore_replication_slot(slot)
+        return self._postgresql.mpp_handler.ignore_replication_slot(slot)
 
     def drop_replication_slot(self, name: str) -> Tuple[bool, bool]:
         """Drop a named slot from Postgres.
 
         :param name: name of the slot to be dropped.
 
         :returns: a tuple of ``active`` and ``dropped``. ``active`` is ``True`` if the slot is active,
@@ -315,30 +317,29 @@
                             ' FROM pg_catalog.pg_replication_slots WHERE slot_name = %s),'
                             ' dropped AS (SELECT pg_catalog.pg_drop_replication_slot(slot_name),'
                             ' true AS dropped FROM slots WHERE not active) '
                             'SELECT active, COALESCE(dropped, false) FROM slots'
                             ' FULL OUTER JOIN dropped ON true'), name)
         return (rows[0][0], rows[0][1]) if rows else (False, False)
 
-    def _drop_incorrect_slots(self, cluster: Cluster, slots: Dict[str, Any], paused: bool) -> None:
+    def _drop_incorrect_slots(self, cluster: Cluster, slots: Dict[str, Any]) -> None:
         """Compare required slots and configured as permanent slots with those found, dropping extraneous ones.
 
         .. note::
             Slots that are not contained in *slots* will be dropped.
             Slots can be filtered out with ``ignore_slots`` configuration.
 
             Slots that have matching names but do not match attributes in *slots* will also be dropped.
 
         :param cluster: cluster state information object.
         :param slots: dictionary of desired slot names as keys with slot attributes as a dictionary value, if known.
-        :param paused: ``True`` if the patroni cluster is currently in a paused state.
         """
         # drop old replication slots which are not presented in desired slots.
         for name in set(self._replication_slots) - set(slots):
-            if not paused and not self.ignore_replication_slot(cluster, name):
+            if not global_config.is_paused and not self.ignore_replication_slot(cluster, name):
                 active, dropped = self.drop_replication_slot(name)
                 if dropped:
                     logger.info("Dropped unknown replication slot '%s'", name)
                 else:
                     self._schedule_load_slots = True
                     if active:
                         logger.debug("Unable to drop unknown replication slot '%s', slot is still active", name)
@@ -488,49 +489,44 @@
             slots.pop(name)
 
         error, copy_slots = self.schedule_advance_slots(advance_slots)
         if error:
             self._schedule_load_slots = True
         return create_slots + copy_slots
 
-    def sync_replication_slots(self, cluster: Cluster, nofailover: bool,
-                               replicatefrom: Optional[str] = None, paused: bool = False) -> List[str]:
+    def sync_replication_slots(self, cluster: Cluster, tags: Tags) -> List[str]:
         """During the HA loop read, check and alter replication slots found in the cluster.
 
         Read physical and logical slots from ``pg_replication_slots``, then compare to those configured in the DCS.
         Drop any slots that do not match those required by configuration and are not configured as permanent.
         Create any missing physical slots, or advance their position according to feedback stored in DCS.
         If we are the primary then create logical slots, otherwise if logical slots are known and active create
         them on replica nodes by copying slot files from the primary.
 
         :param cluster: object containing stateful information for the cluster.
-        :param nofailover: ``True`` if this node has been tagged to not be a failover candidate.
-        :param replicatefrom: the tag containing the node to replicate from.
-        :param paused: ``True`` if the cluster is in maintenance mode.
+        :param tags: reference to an object implementing :class:`Tags` interface.
 
         :returns: list of logical replication slots names that should be copied from the primary.
         """
         ret = []
-        if self._postgresql.major_version >= 90400 and self._postgresql.global_config and cluster.config:
+        if self._postgresql.major_version >= 90400 and cluster.config:
             try:
                 self.load_replication_slots()
 
-                slots = cluster.get_replication_slots(
-                    self._postgresql.name, self._postgresql.role, nofailover, self._postgresql.major_version,
-                    is_standby_cluster=self._postgresql.global_config.is_standby_cluster, show_error=True)
+                slots = cluster.get_replication_slots(self._postgresql, tags, show_error=True)
 
-                self._drop_incorrect_slots(cluster, slots, paused)
+                self._drop_incorrect_slots(cluster, slots)
 
                 self._ensure_physical_slots(slots)
 
                 if self._postgresql.is_primary():
                     self._logical_slots_processing_queue.clear()
                     self._ensure_logical_slots_primary(slots)
                 else:
-                    self.check_logical_slots_readiness(cluster, replicatefrom)
+                    self.check_logical_slots_readiness(cluster, tags)
                     ret = self._ensure_logical_slots_replica(slots)
 
                 self._replication_slots = slots
             except Exception:
                 logger.exception('Exception when changing replication slots')
                 self._schedule_load_slots = True
         return ret
@@ -548,30 +544,30 @@
         :yields: connection cursor object, note implementation varies depending on version of ``psycopg``.
         """
         conn_kwargs = leader.conn_kwargs(self._postgresql.config.rewind_credentials)
         conn_kwargs['dbname'] = self._postgresql.database
         with get_connection_cursor(connect_timeout=3, options="-c statement_timeout=2000", **conn_kwargs) as cur:
             yield cur
 
-    def check_logical_slots_readiness(self, cluster: Cluster, replicatefrom: Optional[str]) -> bool:
+    def check_logical_slots_readiness(self, cluster: Cluster, tags: Tags) -> bool:
         """Determine whether all known logical slots are synchronised from the leader.
 
         1) Retrieve the current ``catalog_xmin`` value for the physical slot from the cluster leader, and
         2) using previously stored list of "unready" logical slots, those which have yet to be checked hence have no
            stored slot attributes,
         3) store logical slot ``catalog_xmin`` when the physical slot ``catalog_xmin`` becomes valid.
 
         :param cluster: object containing stateful information for the cluster.
-        :param replicatefrom: name of the member that should be used to replicate from.
+        :param tags: reference to an object implementing :class:`Tags` interface.
 
         :returns: ``False`` if any issue while checking logical slots readiness, ``True`` otherwise.
         """
         catalog_xmin = None
         if self._logical_slots_processing_queue and cluster.leader:
-            slot_name = cluster.get_my_slot_name_on_primary(self._postgresql.name, replicatefrom)
+            slot_name = cluster.get_slot_name_on_primary(self._postgresql.name, tags)
             try:
                 with self._get_leader_connection_cursor(cluster.leader) as cur:
                     cur.execute("SELECT slot_name, catalog_xmin FROM pg_catalog.pg_get_replication_slots()"
                                 " WHERE NOT pg_catalog.pg_is_in_recovery() AND slot_name = ANY(%s)",
                                 ([n for n, v in self._logical_slots_processing_queue.items()
                                   if v is None] + [slot_name],))
                     slots = {row[0]: row[1] for row in cur}
@@ -641,24 +637,25 @@
             ):
 
                 del self._logical_slots_processing_queue[name]
 
                 if standby_logical_slot:
                     logger.info('Logical slot %s is safe to be used after a failover', name)
 
-    def copy_logical_slots(self, cluster: Cluster, create_slots: List[str]) -> None:
+    def copy_logical_slots(self, cluster: Cluster, tags: Tags, create_slots: List[str]) -> None:
         """Create logical replication slots on standby nodes.
 
         :param cluster: object containing stateful information for the cluster.
+        :param tags: reference to an object implementing :class:`Tags` interface.
         :param create_slots: list of slot names to copy from the primary.
         """
         leader = cluster.leader
         if not leader:
             return
-        slots = cluster.get_replication_slots(self._postgresql.name, 'replica', False, self._postgresql.major_version)
+        slots = cluster.get_replication_slots(self._postgresql, tags, role='replica')
         copy_slots: Dict[str, Dict[str, Any]] = {}
         with self._get_leader_connection_cursor(leader) as cur:
             try:
                 cur.execute("SELECT slot_name, slot_type, datname, plugin, catalog_xmin, "
                             "pg_catalog.pg_wal_lsn_diff(confirmed_flush_lsn, '0/0')::bigint, "
                             "pg_catalog.pg_read_binary_file('pg_replslot/' || slot_name || '/state')"
                             " FROM pg_catalog.pg_get_replication_slots() JOIN pg_catalog.pg_database ON datoid = oid"
```

### Comparing `patroni-3.2.2/patroni/postgresql/sync.py` & `patroni-3.3.0/patroni/postgresql/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import re
 import time
 
 from copy import deepcopy
 from typing import Collection, List, NamedTuple, Tuple, TYPE_CHECKING
 
+from .. import global_config
 from ..collections import CaseInsensitiveDict, CaseInsensitiveSet
 from ..dcs import Cluster
 from ..psycopg import quote_ident as _quote_ident
 if TYPE_CHECKING:  # pragma: no cover
     from . import Postgresql
 
 logger = logging.getLogger(__name__)
@@ -299,19 +300,16 @@
         :returns: tuple of candidates :class:`CaseInsensitiveSet` and synchronous standbys :class:`CaseInsensitiveSet`.
         """
         self._handle_synchronous_standby_names_change()
 
         replica_list = _ReplicaList(self._postgresql, cluster)
         self._process_replica_readiness(cluster, replica_list)
 
-        if TYPE_CHECKING:  # pragma: no cover
-            assert self._postgresql.global_config is not None
-        sync_node_count = self._postgresql.global_config.synchronous_node_count\
-            if self._postgresql.supports_multiple_sync else 1
-        sync_node_maxlag = self._postgresql.global_config.maximum_lag_on_syncnode
+        sync_node_count = global_config.synchronous_node_count if self._postgresql.supports_multiple_sync else 1
+        sync_node_maxlag = global_config.maximum_lag_on_syncnode
 
         candidates = CaseInsensitiveSet()
         sync_nodes = CaseInsensitiveSet()
         # Prefer members without nofailover tag. We are relying on the fact that sorts are guaranteed to be stable.
         for replica in sorted(replica_list, key=lambda x: x.nofailover):
             if sync_node_maxlag <= 0 or replica_list.max_lsn - replica.lsn <= sync_node_maxlag:
                 candidates.add(replica.application_name)
```

### Comparing `patroni-3.2.2/patroni/postgresql/validator.py` & `patroni-3.3.0/patroni/postgresql/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 from copy import deepcopy
 import logging
-import os
 import yaml
 
 from typing import Any, Dict, Iterator, List, MutableMapping, Optional, Tuple, Type, Union
 
+from .available_parameters import get_validator_files, PathLikeObj
 from ..collections import CaseInsensitiveDict, CaseInsensitiveSet
 from ..exceptions import PatroniException
 from ..utils import parse_bool, parse_int, parse_real
 
 logger = logging.getLogger(__name__)
 
 
@@ -254,27 +254,27 @@
     return tuple(validators)
 
 
 class InvalidGucValidatorsFile(PatroniException):
     """Raised when reading or parsing of a YAML file faces an issue."""
 
 
-def _read_postgres_gucs_validators_file(file: str) -> Dict[str, Any]:
+def _read_postgres_gucs_validators_file(file: PathLikeObj) -> Dict[str, Any]:
     """Read an YAML file and return the corresponding Python object.
 
-    :param file: path to the file to be read. It is expected to be encoded with ``UTF-8``, and to be a YAML document.
+    :param file: path-like object to read from. It is expected to be encoded with ``UTF-8``, and to be a YAML document.
 
     :returns: the YAML content parsed into a Python object. If any issue is faced while reading/parsing the file, then
         return ``None``.
 
     :raises:
         :class:`InvalidGucValidatorsFile`: if faces an issue while reading or parsing *file*.
     """
     try:
-        with open(file, encoding='UTF-8') as stream:
+        with file.open(encoding='UTF-8') as stream:
             return yaml.safe_load(stream)
     except Exception as exc:
         raise InvalidGucValidatorsFile(
             f'Unexpected issue while reading parameters file `{file}`: `{str(exc)}`.') from exc
 
 
 def _load_postgres_gucs_validators() -> None:
@@ -381,29 +381,15 @@
                 recovery_parameters:
                   archive_cleanup_command:
                   - type: String
                     version_from: 90300
                     version_till: null
 
     """
-    conf_dir = os.path.join(
-        os.path.dirname(os.path.abspath(__file__)),
-        'available_parameters',
-    )
-    yaml_files: List[str] = []
-
-    for root, _, files in os.walk(conf_dir):
-        for file in sorted(files):
-            full_path = os.path.join(root, file)
-            if file.lower().endswith(('.yml', '.yaml')):
-                yaml_files.append(full_path)
-            else:
-                logger.info('Ignored a non-YAML file found under `available_parameters` directory: `%s`.', full_path)
-
-    for file in yaml_files:
+    for file in get_validator_files():
         try:
             config: Dict[str, Any] = _read_postgres_gucs_validators_file(file)
         except InvalidGucValidatorsFile as exc:
             logger.warning(str(exc))
             continue
 
         logger.debug(f'Parsing validators from file `{file}`.')
```

### Comparing `patroni-3.2.2/patroni/psycopg.py` & `patroni-3.3.0/patroni/psycopg.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,29 +38,30 @@
         :returns: *value* quoted as a SQL literal.
         """
         value = adapt(value)
         if conn:
             value.prepare(conn)
         return value.getquoted().decode('utf-8')
 except ImportError:
-    from psycopg import connect as __connect, sql, Error, DatabaseError, OperationalError, ProgrammingError
+    from psycopg import connect as __connect  # pyright: ignore [reportUnknownVariableType]
+    from psycopg import sql, Error, DatabaseError, OperationalError, ProgrammingError
 
     def _connect(dsn: Optional[str] = None, **kwargs: Any) -> 'Connection[Any]':
         """Call :func:`psycopg.connect` with *dsn* and ``**kwargs``.
 
         .. note::
             Will create ``server_version`` attribute in the returning connection, so it keeps compatibility with the
             object that would be returned by :func:`psycopg2.connect`.
 
         :param dsn: DSN to call :func:`psycopg.connect` with.
         :param kwargs: keyword arguments to call :func:`psycopg.connect` with.
 
         :returns: a connection to the database.
         """
-        ret = __connect(dsn or "", **kwargs)
+        ret: 'Connection[Any]' = __connect(dsn or "", **kwargs)
         setattr(ret, 'server_version', ret.pgconn.server_version)  # compatibility with psycopg2
         return ret
 
     def _quote_ident(value: Any, scope: Any) -> str:
         """Quote *value* as a SQL identifier.
 
         :param value: value to be quoted.
```

### Comparing `patroni-3.2.2/patroni/raft_controller.py` & `patroni-3.3.0/patroni/raft_controller.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/request.py` & `patroni-3.3.0/patroni/request.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/scripts/aws.py` & `patroni-3.3.0/patroni/scripts/aws.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/scripts/wale_restore.py` & `patroni-3.3.0/patroni/scripts/wale_restore.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/tags.py` & `patroni-3.3.0/patroni/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """Tags handling."""
 import abc
 
 from typing import Any, Dict, Optional
 
-from patroni.utils import parse_int
+from patroni.utils import parse_int, parse_bool
 
 
 class Tags(abc.ABC):
     """An abstract class that encapsulates all the ``tags`` logic.
 
     Child classes that want to use provided facilities must implement ``tags`` abstract property.
+
+    .. note::
+        Due to backward-compatibility reasons, old tags may have a less strict type conversion than new ones.
     """
 
     @staticmethod
     def _filter_tags(tags: Dict[str, Any]) -> Dict[str, Any]:
         """Get tags configured for this node, if any.
 
         Handle both predefined Patroni tags and custom defined tags.
 
         .. note::
             A custom tag is any tag added to the configuration ``tags`` section that is not one of ``clonefrom``,
-            ``nofailover``, ``noloadbalance`` or ``nosync``.
+            ``nofailover``, ``noloadbalance``,``nosync`` or ``nostream``.
 
             For most of the Patroni predefined tags, the returning object will only contain them if they are enabled as
             they all are boolean values that default to disabled.
             However ``nofailover`` tag is always returned if ``failover_priority`` tag is defined. In this case, we need
             both values to see if they are contradictory and the ``nofailover`` value should be used.
 
         :returns: a dictionary of tags set for this node. The key is the tag name, and the value is the corresponding
             tag value.
         """
         return {tag: value for tag, value in tags.items()
-                if any((tag not in ('clonefrom', 'nofailover', 'noloadbalance', 'nosync'),
+                if any((tag not in ('clonefrom', 'nofailover', 'noloadbalance', 'nosync', 'nostream'),
                         value,
                         tag == 'nofailover' and 'failover_priority' in tags))}
 
     @property
     @abc.abstractmethod
     def tags(self) -> Dict[str, Any]:
         """Configured tags.
@@ -85,7 +88,12 @@
         """``True`` if ``nosync`` is ``True``, else ``False``."""
         return bool(self.tags.get('nosync', False))
 
     @property
     def replicatefrom(self) -> Optional[str]:
         """Value of ``replicatefrom`` tag, if any."""
         return self.tags.get('replicatefrom')
+
+    @property
+    def nostream(self) -> bool:
+        """``True`` if ``nostream`` is ``True``, else ``False``."""
+        return parse_bool(self.tags.get('nostream')) or False
```

### Comparing `patroni-3.2.2/patroni/utils.py` & `patroni-3.3.0/patroni/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,51 +6,83 @@
 :var OCT_RE: regular expression to match octal numbers, signed or unsigned.
 :var DEC_RE: regular expression to match decimal numbers, signed or unsigned.
 :var HEX_RE: regular expression to match hex strings, signed or unsigned.
 :var DBL_RE: regular expression to match double precision numbers, signed or unsigned. Matches scientific notation too.
 :var WHITESPACE_RE: regular expression to match whitespace characters
 """
 import errno
+import itertools
 import logging
 import os
 import platform
 import random
 import re
 import socket
 import subprocess
 import sys
 import tempfile
 import time
 from shlex import split
 
 from typing import Any, Callable, Dict, Iterator, List, Optional, Union, Tuple, Type, TYPE_CHECKING
 
+from collections import OrderedDict
 from dateutil import tz
 from json import JSONDecoder
 from urllib3.response import HTTPResponse
 
 from .exceptions import PatroniException
 from .version import __version__
 
 if TYPE_CHECKING:  # pragma: no cover
     from .dcs import Cluster
-    from .config import GlobalConfig
 
 tzutc = tz.tzutc()
 
 logger = logging.getLogger(__name__)
 
 USER_AGENT = 'Patroni/{0} Python/{1} {2}'.format(__version__, platform.python_version(), platform.system())
 OCT_RE = re.compile(r'^[-+]?0[0-7]*')
 DEC_RE = re.compile(r'^[-+]?(0|[1-9][0-9]*)')
 HEX_RE = re.compile(r'^[-+]?0x[0-9a-fA-F]+')
 DBL_RE = re.compile(r'^[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?')
 WHITESPACE_RE = re.compile(r'[ \t\n\r]*', re.VERBOSE | re.MULTILINE | re.DOTALL)
 
 
+def get_conversion_table(base_unit: str) -> Dict[str, Dict[str, Union[int, float]]]:
+    """Get conversion table for the specified base unit.
+
+    If no conversion table exists for the passed unit, return an empty :class:`OrderedDict`.
+
+    :param base_unit: unit to choose the conversion table for.
+
+    :returns: :class:`OrderedDict` object.
+    """
+    memory_unit_conversion_table: Dict[str, Dict[str, Union[int, float]]] = OrderedDict([
+        ('TB', {'B': 1024**4, 'kB': 1024**3, 'MB': 1024**2}),
+        ('GB', {'B': 1024**3, 'kB': 1024**2, 'MB': 1024}),
+        ('MB', {'B': 1024**2, 'kB': 1024, 'MB': 1}),
+        ('kB', {'B': 1024, 'kB': 1, 'MB': 1024**-1}),
+        ('B', {'B': 1, 'kB': 1024**-1, 'MB': 1024**-2})
+    ])
+    time_unit_conversion_table: Dict[str, Dict[str, Union[int, float]]] = OrderedDict([
+        ('d', {'ms': 1000 * 60**2 * 24, 's': 60**2 * 24, 'min': 60 * 24}),
+        ('h', {'ms': 1000 * 60**2, 's': 60**2, 'min': 60}),
+        ('min', {'ms': 1000 * 60, 's': 60, 'min': 1}),
+        ('s', {'ms': 1000, 's': 1, 'min': 60**-1}),
+        ('ms', {'ms': 1, 's': 1000**-1, 'min': 1 / (1000 * 60)}),
+        ('us', {'ms': 1000**-1, 's': 1000**-2, 'min': 1 / (1000**2 * 60)})
+    ])
+    if base_unit in ('B', 'kB', 'MB'):
+        return memory_unit_conversion_table
+    elif base_unit in ('ms', 's', 'min'):
+        return time_unit_conversion_table
+    return OrderedDict()
+
+
 def deep_compare(obj1: Dict[Any, Union[Any, Dict[Any, Any]]], obj2: Dict[Any, Union[Any, Dict[Any, Any]]]) -> bool:
     """Recursively compare two dictionaries to check if they are equal in terms of keys and values.
 
     .. note::
         Values are compared based on their string representation.
 
     :param obj1: dictionary to be compared with *obj2*.
@@ -269,41 +301,160 @@
 
         >>> convert_to_base_unit(1, 'gB', '512MB') is None
         True
 
         >>> convert_to_base_unit(1, 'GB', '512 MB') is None
         True
     """
-    convert: Dict[str, Dict[str, Union[int, float]]] = {
-        'B': {'B': 1, 'kB': 1024, 'MB': 1024 * 1024, 'GB': 1024 * 1024 * 1024, 'TB': 1024 * 1024 * 1024 * 1024},
-        'kB': {'B': 1.0 / 1024, 'kB': 1, 'MB': 1024, 'GB': 1024 * 1024, 'TB': 1024 * 1024 * 1024},
-        'MB': {'B': 1.0 / (1024 * 1024), 'kB': 1.0 / 1024, 'MB': 1, 'GB': 1024, 'TB': 1024 * 1024},
-        'ms': {'us': 1.0 / 1000, 'ms': 1, 's': 1000, 'min': 1000 * 60, 'h': 1000 * 60 * 60, 'd': 1000 * 60 * 60 * 24},
-        's': {'us': 1.0 / (1000 * 1000), 'ms': 1.0 / 1000, 's': 1, 'min': 60, 'h': 60 * 60, 'd': 60 * 60 * 24},
-        'min': {'us': 1.0 / (1000 * 1000 * 60), 'ms': 1.0 / (1000 * 60), 's': 1.0 / 60, 'min': 1, 'h': 60, 'd': 60 * 24}
-    }
+    base_value, base_unit = strtol(base_unit, False)
+    if TYPE_CHECKING:  # pragma: no cover
+        assert isinstance(base_value, int)
+
+    convert_tbl = get_conversion_table(base_unit)
+    # {'TB': 'GB', 'GB': 'MB', ...}
+    round_order = dict(zip(convert_tbl, itertools.islice(convert_tbl, 1, None)))
+    if unit in convert_tbl and base_unit in convert_tbl[unit]:
+        value *= convert_tbl[unit][base_unit] / float(base_value)
+        if unit in round_order:
+            multiplier = convert_tbl[round_order[unit]][base_unit]
+            value = round(value / float(multiplier)) * multiplier
+        return value
 
-    round_order = {
-        'TB': 'GB', 'GB': 'MB', 'MB': 'kB', 'kB': 'B',
-        'd': 'h', 'h': 'min', 'min': 's', 's': 'ms', 'ms': 'us'
-    }
 
-    if base_unit and base_unit not in convert:
-        base_value, base_unit = strtol(base_unit, False)
-    else:
-        base_value = 1
+def convert_int_from_base_unit(base_value: int, base_unit: Optional[str]) -> Optional[str]:
+    """Convert an integer value in some base unit to a human-friendly unit.
 
-    if base_value is not None and base_unit in convert and unit in convert[base_unit]:
-        value *= convert[base_unit][unit] / float(base_value)
+    The output unit is chosen so that it's the greatest unit that can represent
+    the value without loss.
 
-        if unit in round_order:
-            multiplier = convert[base_unit][round_order[unit]]
-            value = round(value / float(multiplier)) * multiplier
+    :param base_value: value to be converted from a base unit
+    :param base_unit: unit of *value*. Should be one of the base units (case sensitive):
 
-        return value
+            * For space: ``B``, ``kB``, ``MB``;
+            * For time: ``ms``, ``s``, ``min``.
+
+    :returns: :class:`str` value representing *base_value* converted from *base_unit* to the greatest
+        possible human-friendly unit, or ``None`` if conversion failed.
+
+    :Example:
+
+        >>> convert_int_from_base_unit(1024, 'kB')
+        '1MB'
+
+        >>> convert_int_from_base_unit(1025, 'kB')
+        '1025kB'
+
+        >>> convert_int_from_base_unit(4, '256MB')
+        '1GB'
+
+        >>> convert_int_from_base_unit(4, '256 MB') is None
+        True
+
+        >>> convert_int_from_base_unit(1024, 'KB') is None
+        True
+    """
+    base_value_mult, base_unit = strtol(base_unit, False)
+    if TYPE_CHECKING:  # pragma: no cover
+        assert isinstance(base_value_mult, int)
+    base_value *= base_value_mult
+
+    convert_tbl = get_conversion_table(base_unit)
+    for unit in convert_tbl:
+        multiplier = convert_tbl[unit][base_unit]
+        if multiplier <= 1.0 or base_value % multiplier == 0:
+            return str(round(base_value / multiplier)) + unit
+
+
+def convert_real_from_base_unit(base_value: float, base_unit: Optional[str]) -> Optional[str]:
+    """Convert an floating-point value in some base unit to a human-friendly unit.
+
+    Same as :func:`convert_int_from_base_unit`, except we have to do the math a bit differently,
+    and there's a possibility that we don't find any exact divisor.
+
+    :param base_value: value to be converted from a base unit
+    :param base_unit: unit of *value*. Should be one of the base units (case sensitive):
+
+            * For space: ``B``, ``kB``, ``MB``;
+            * For time: ``ms``, ``s``, ``min``.
+
+    :returns: :class:`str` value representing *base_value* converted from *base_unit* to the greatest
+        possible human-friendly unit, or ``None`` if conversion failed.
+
+    :Example:
+
+        >>> convert_real_from_base_unit(5, 'ms')
+        '5ms'
+
+        >>> convert_real_from_base_unit(2.5, 'ms')
+        '2500us'
+
+        >>> convert_real_from_base_unit(4.0, '256MB')
+        '1GB'
+
+        >>> convert_real_from_base_unit(4.0, '256 MB') is None
+        True
+    """
+    base_value_mult, base_unit = strtol(base_unit, False)
+    if TYPE_CHECKING:  # pragma: no cover
+        assert isinstance(base_value_mult, int)
+    base_value *= base_value_mult
+
+    result = None
+    convert_tbl = get_conversion_table(base_unit)
+    for unit in convert_tbl:
+        value = base_value / convert_tbl[unit][base_unit]
+        result = f'{value:g}{unit}'
+        if value > 0 and abs((round(value) / value) - 1.0) <= 1e-8:
+            break
+    return result
+
+
+def maybe_convert_from_base_unit(base_value: str, vartype: str, base_unit: Optional[str]) -> str:
+    """Try to convert integer or real value in a base unit to a human-readable unit.
+
+    Value is passed as a string. If parsing or subsequent conversion fails, the original
+    value is returned.
+
+    :param base_value: value to be converted from a base unit.
+    :param vartype: the target type to parse *base_value* before converting (``integer``
+        or ``real`` is expected, any other type results in return value being equal to the
+        *base_value* string).
+    :param base_unit: unit of *value*. Should be one of the base units (case sensitive):
+
+            * For space: ``B``, ``kB``, ``MB``;
+            * For time: ``ms``, ``s``, ``min``.
+
+    :returns: :class:`str` value representing *base_value* converted from *base_unit* to the greatest
+        possible human-friendly unit, or *base_value* string if conversion failed.
+
+    :Example:
+
+        >>> maybe_convert_from_base_unit('5', 'integer', 'ms')
+        '5ms'
+
+        >>> maybe_convert_from_base_unit('4.2', 'real', 'ms')
+        '4200us'
+
+        >>> maybe_convert_from_base_unit('on', 'bool', None)
+        'on'
+
+        >>> maybe_convert_from_base_unit('', 'integer', '256MB')
+        ''
+    """
+    converters: Dict[str, Tuple[Callable[[str, Optional[str]], Union[int, float, str, None]],
+                                Callable[[Any, Optional[str]], Optional[str]]]] = {
+        'integer': (parse_int, convert_int_from_base_unit),
+        'real': (parse_real, convert_real_from_base_unit),
+        'default': (lambda v, _: v, lambda v, _: v)
+    }
+    parser, converter = converters.get(vartype, converters['default'])
+    parsed_value = parser(base_value, None)
+    if parsed_value:
+        return converter(parsed_value, base_unit) or base_value
+    return base_value
 
 
 def parse_int(value: Any, base_unit: Optional[str] = None) -> Optional[int]:
     """Parse *value* as an :class:`int`.
 
     :param value: any value that can be handled either by :func:`strtol` or :func:`strtod`. If *value* contains a
         unit, then *base_unit* must be given.
@@ -561,27 +712,26 @@
 
     @property
     def stoptime(self) -> float:
         """Get the current stop time."""
         return self._cur_stoptime or 0
 
     def ensure_deadline(self, timeout: float, raise_ex: Optional[Exception] = None) -> bool:
-        """Calculates, sets, and checks the remaining deadline time.
+        """Calculates and checks the remaining deadline time.
 
         :param timeout: if the *deadline* is smaller than the provided *timeout* value raise *raise_ex* exception.
         :param raise_ex: the exception object that will be raised if the *deadline* is smaller than provided *timeout*.
 
         :returns: ``False`` if *deadline* is smaller than a provided *timeout* and *raise_ex* isn't set. Otherwise
             ``True``.
 
         :raises:
             :class:`Exception`: *raise_ex* if calculated deadline is smaller than provided *timeout*.
         """
-        self.deadline = self.stoptime - time.time()
-        if self.deadline < timeout:
+        if self.stoptime - time.time() < timeout:
             if raise_ex:
                 raise raise_ex
             return False
         return True
 
     def __call__(self, func: Callable[..., Any], *args: Any, **kwargs: Any) -> Any:
         """Call a function *func* with arguments ``*args`` and ``*kwargs`` in a loop.
@@ -756,20 +906,18 @@
             else:
                 yield message
                 idx = WHITESPACE_RE.match(chunk, idx).end()  # pyright: ignore [reportOptionalMemberAccess]
         # It is not usual that a ``chunk`` would contain more than one JSON document, but we handle that just in case
         prev = chunk[idx:]
 
 
-def cluster_as_json(cluster: 'Cluster', global_config: Optional['GlobalConfig'] = None) -> Dict[str, Any]:
+def cluster_as_json(cluster: 'Cluster') -> Dict[str, Any]:
     """Get a JSON representation of *cluster*.
 
     :param cluster: the :class:`~patroni.dcs.Cluster` object to be parsed as JSON.
-    :param global_config: optional :class:`~patroni.config.GlobalConfig` object to check the cluster state.
-                          if not provided will be instantiated from the `Cluster.config`.
 
     :returns: JSON representation of *cluster*.
 
     These are the possible keys in the returning object depending on the available information in *cluster*:
 
         * ``members``: list of members in the cluster. Each value is a :class:`dict` that may have the following keys:
 
@@ -790,37 +938,37 @@
         * ``pause``: ``True`` if cluster is in maintenance mode;
         * ``scheduled_switchover``: if a switchover has been scheduled, then it contains this entry with these keys:
 
             * ``at``: timestamp when switchover was scheduled to occur;
             * ``from``: name of the member to be demoted;
             * ``to``: name of the member to be promoted.
     """
-    if not global_config:
-        from patroni.config import get_global_config
-        global_config = get_global_config(cluster)
+    from . import global_config
+
+    config = global_config.from_cluster(cluster)
     leader_name = cluster.leader.name if cluster.leader else None
     cluster_lsn = cluster.last_lsn or 0
 
     ret: Dict[str, Any] = {'members': []}
     for m in cluster.members:
         if m.name == leader_name:
-            role = 'standby_leader' if global_config.is_standby_cluster else 'leader'
+            role = 'standby_leader' if config.is_standby_cluster else 'leader'
         elif cluster.sync.matches(m.name):
             role = 'sync_standby'
         else:
             role = 'replica'
 
         state = (m.data.get('replication_state', '') if role != 'leader' else '') or m.data.get('state', '')
         member = {'name': m.name, 'role': role, 'state': state, 'api_url': m.api_url}
         conn_kwargs = m.conn_kwargs()
         if conn_kwargs.get('host'):
             member['host'] = conn_kwargs['host']
             if conn_kwargs.get('port'):
                 member['port'] = int(conn_kwargs['port'])
-        optional_attributes = ('timeline', 'pending_restart', 'scheduled_restart', 'tags')
+        optional_attributes = ('timeline', 'pending_restart', 'pending_restart_reason', 'scheduled_restart', 'tags')
         member.update({n: m.data[n] for n in optional_attributes if n in m.data})
 
         if m.name != leader_name:
             lsn = m.lsn
             if lsn is None:
                 member['lag'] = 'unknown'
             elif cluster_lsn >= lsn:
@@ -829,15 +977,15 @@
                 member['lag'] = 0
 
         ret['members'].append(member)
 
     # sort members by name for consistency
     cmp: Callable[[Dict[str, Any]], bool] = lambda m: m['name']
     ret['members'].sort(key=cmp)
-    if global_config.is_paused:
+    if config.is_paused:
         ret['pause'] = True
     if cluster.failover and cluster.failover.scheduled_at:
         ret['scheduled_switchover'] = {'at': cluster.failover.scheduled_at.isoformat()}
         if cluster.failover.leader:
             ret['scheduled_switchover']['from'] = cluster.failover.leader
         if cluster.failover.candidate:
             ret['scheduled_switchover']['to'] = cluster.failover.candidate
```

### Comparing `patroni-3.2.2/patroni/validator.py` & `patroni-3.3.0/patroni/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,61 @@
 """
 import os
 import shutil
 import socket
 
 from typing import Any, Dict, Union, Iterator, List, Optional as OptionalType, Tuple, TYPE_CHECKING
 
-from .collections import CaseInsensitiveSet
-
+from .collections import CaseInsensitiveSet, EMPTY_DICT
 from .dcs import dcs_modules
 from .exceptions import ConfigParseError
 from .utils import parse_int, split_host_port, data_directory_is_empty, get_major_version
+from .log import type_logformat
+
+
+def validate_log_field(field: Union[str, Dict[str, Any], Any]) -> bool:
+    """Checks if log field is valid.
+
+    :param field: A log field to be validated.
+
+    :returns: ``True`` if the field is either a string or a dictionary with exactly one key
+              that has string value, ``False`` otherwise.
+    """
+    if isinstance(field, str):
+        return True
+    elif isinstance(field, dict):
+        return len(field) == 1 and isinstance(next(iter(field.values())), str)
+    return False
+
+
+def validate_log_format(logformat: type_logformat) -> bool:
+    """Checks if log format is valid.
+
+    :param logformat: A log format to be validated.
+
+    :returns: ``True`` if the log format is either a string or a list of valid log fields.
+
+    :raises:
+        :exc:`~patroni.exceptions.ConfigParseError`:
+            * If the logformat is not a string or a list; or
+            * If the logformat is an empty list; or
+            * If the log format is a list and it with values that don't pass validation using
+              :func:`validate_log_field`.
+    """
+    if isinstance(logformat, str):
+        return True
+    elif isinstance(logformat, list):
+        if len(logformat) == 0:
+            raise ConfigParseError('should contain at least one item')
+        if not all(map(validate_log_field, logformat)):
+            raise ConfigParseError('each item should be a string or a dictionary with string values')
+
+        return True
+    else:
+        raise ConfigParseError('Should be a string or a list')
 
 
 def data_directory_empty(data_dir: str) -> bool:
     """Check if PostgreSQL data directory is empty.
 
     :param data_dir: path to the PostgreSQL data directory to be checked.
 
@@ -198,15 +240,15 @@
 
     :param bin_name: a key to be retrieved from ``postgresql.bin_name`` configuration.
 
     :returns: value of ``postgresql.bin_name[*bin_name*]``, if present, otherwise *bin_name*.
     """
     if TYPE_CHECKING:  # pragma: no cover
         assert isinstance(schema.data, dict)
-    return (schema.data.get('postgresql', {}).get('bin_name', {}) or {}).get(bin_name, bin_name)
+    return (schema.data.get('postgresql', {}).get('bin_name', {}) or EMPTY_DICT).get(bin_name, bin_name)
 
 
 def validate_data_dir(data_dir: str) -> bool:
     """Validate the value of ``postgresql.data_dir`` configuration option.
 
     It requires that ``postgresql.data_dir`` is set and match one of following conditions:
 
@@ -933,14 +975,28 @@
     Optional("cert"): str,
     Optional("key"): str
 }
 
 schema = Schema({
     "name": str,
     "scope": str,
+    Optional("log"): {
+        Optional("type"): EnumValidator(('plain', 'json'), case_sensitive=True, raise_assert=True),
+        Optional("level"): EnumValidator(('DEBUG', 'INFO', 'WARN', 'WARNING', 'ERROR', 'FATAL', 'CRITICAL'),
+                                         case_sensitive=True, raise_assert=True),
+        Optional("traceback_level"): EnumValidator(('DEBUG', 'ERROR'), raise_assert=True),
+        Optional("format"): validate_log_format,
+        Optional("dateformat"): str,
+        Optional("static_fields"): dict,
+        Optional("max_queue_size"): int,
+        Optional("dir"): str,
+        Optional("file_num"): int,
+        Optional("file_size"): int,
+        Optional("loggers"): dict
+    },
     Optional("ctl"): {
         Optional("insecure"): bool,
         Optional("cacert"): str,
         Optional("certfile"): str,
         Optional("keyfile"): str,
         Optional("keyfile_password"): str
     },
@@ -1046,15 +1102,16 @@
             "hosts": Or(comma_separated_host_port, [validate_host_port]),
             Optional("use_ssl"): bool,
             Optional("cacert"): str,
             Optional("cert"): str,
             Optional("key"): str,
             Optional("key_password"): str,
             Optional("verify"): bool,
-            Optional("set_acls"): dict
+            Optional("set_acls"): dict,
+            Optional("auth_data"): dict,
         },
         "kubernetes": {
             "labels": {},
             Optional("bypass_api_service"): bool,
             Optional("namespace"): str,
             Optional("scope_label"): str,
             Optional("role_label"): str,
@@ -1110,10 +1167,11 @@
         AtMostOne("nofailover", "failover_priority"): Case({
             "nofailover": bool,
             "failover_priority": IntValidator(min=0, expected_type=int, raise_assert=True),
         }),
         Optional("clonefrom"): bool,
         Optional("noloadbalance"): bool,
         Optional("replicatefrom"): str,
-        Optional("nosync"): bool
+        Optional("nosync"): bool,
+        Optional("nostream"): bool
     }
 })
```

### Comparing `patroni-3.2.2/patroni/watchdog/base.py` & `patroni-3.3.0/patroni/watchdog/base.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni/watchdog/linux.py` & `patroni-3.3.0/patroni/watchdog/linux.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/patroni.egg-info/PKG-INFO` & `patroni-3.3.0/patroni.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patroni
-Version: 3.2.2
+Version: 3.3.0
 Summary: PostgreSQL High-Available orchestrator and CLI
 Home-page: https://github.com/zalando/patroni
 Author: Alexander Kukushkin, Polina Bungina
 Author-email: akukushkin@microsoft.com, polina.bungina@zalando.de
 License: The MIT License
 Keywords: etcd governor patroni postgresql postgres ha haproxy confd zookeeper exhibitor consul streaming replication kubernetes k8s
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,21 +45,24 @@
 Requires-Dist: kazoo>=1.3.1; extra == "exhibitor"
 Provides-Extra: zookeeper
 Requires-Dist: kazoo>=1.3.1; extra == "zookeeper"
 Provides-Extra: kubernetes
 Provides-Extra: raft
 Requires-Dist: pysyncobj>=0.3.8; extra == "raft"
 Requires-Dist: cryptography>=1.4; extra == "raft"
+Provides-Extra: jsonlogger
+Requires-Dist: python-json-logger>=2.0.2; extra == "jsonlogger"
 Provides-Extra: all
 Requires-Dist: python-etcd<0.5,>=0.4.3; extra == "all"
-Requires-Dist: kazoo>=1.3.1; extra == "all"
-Requires-Dist: boto3; extra == "all"
 Requires-Dist: pysyncobj>=0.3.8; extra == "all"
-Requires-Dist: cryptography>=1.4; extra == "all"
 Requires-Dist: python-consul>=0.7.1; extra == "all"
+Requires-Dist: cryptography>=1.4; extra == "all"
+Requires-Dist: boto3; extra == "all"
+Requires-Dist: kazoo>=1.3.1; extra == "all"
+Requires-Dist: python-json-logger>=2.0.2; extra == "all"
 Provides-Extra: psycopg2
 Requires-Dist: psycopg2>=2.5.4; extra == "psycopg2"
 Provides-Extra: psycopg2-binary
 Requires-Dist: psycopg2-binary; extra == "psycopg2-binary"
 Provides-Extra: psycopg3
 Requires-Dist: psycopg[binary]>=3.0.0; extra == "psycopg3"
 
@@ -212,15 +215,15 @@
 
     > psql --host 127.0.0.1 --port 5000 postgres
 
 ==================
 YAML Configuration
 ==================
 
-Go `here <https://github.com/zalando/patroni/blob/master/docs/SETTINGS.rst>`__ for comprehensive information about settings for etcd, consul, and ZooKeeper. And for an example, see `postgres0.yml <https://github.com/zalando/patroni/blob/master/postgres0.yml>`__.
+Go `here <https://github.com/zalando/patroni/blob/master/docs/dynamic_configuration.rst>`__ for comprehensive information about settings for etcd, consul, and ZooKeeper. And for an example, see `postgres0.yml <https://github.com/zalando/patroni/blob/master/postgres0.yml>`__.
 
 =========================
 Environment Configuration
 =========================
 
 Go `here <https://github.com/zalando/patroni/blob/master/docs/ENVIRONMENT.rst>`__ for comprehensive information about configuring(overriding) settings via environment variables.
```

### Comparing `patroni-3.2.2/patroni.egg-info/SOURCES.txt` & `patroni-3.3.0/patroni.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 patroni/api.py
 patroni/async_executor.py
 patroni/collections.py
 patroni/config.py
 patroni/config_generator.py
 patroni/ctl.py
 patroni/daemon.py
+patroni/dynamic_loader.py
 patroni/exceptions.py
 patroni/file_perm.py
+patroni/global_config.py
 patroni/ha.py
 patroni/log.py
 patroni/psycopg.py
 patroni/raft_controller.py
 patroni/request.py
 patroni/tags.py
 patroni/utils.py
@@ -39,33 +41,41 @@
 patroni/dcs/kubernetes.py
 patroni/dcs/raft.py
 patroni/dcs/zookeeper.py
 patroni/postgresql/__init__.py
 patroni/postgresql/bootstrap.py
 patroni/postgresql/callback_executor.py
 patroni/postgresql/cancellable.py
-patroni/postgresql/citus.py
 patroni/postgresql/config.py
 patroni/postgresql/connection.py
 patroni/postgresql/misc.py
 patroni/postgresql/postmaster.py
 patroni/postgresql/rewind.py
 patroni/postgresql/slots.py
 patroni/postgresql/sync.py
 patroni/postgresql/validator.py
 patroni/postgresql/available_parameters/0_postgres.yml
+patroni/postgresql/available_parameters/__init__.py
+patroni/postgresql/mpp/__init__.py
+patroni/postgresql/mpp/citus.py
 patroni/scripts/__init__.py
 patroni/scripts/aws.py
 patroni/scripts/wale_restore.py
+patroni/scripts/barman/__init__.py
+patroni/scripts/barman/cli.py
+patroni/scripts/barman/config_switch.py
+patroni/scripts/barman/recover.py
+patroni/scripts/barman/utils.py
 patroni/watchdog/__init__.py
 patroni/watchdog/base.py
 patroni/watchdog/linux.py
 tests/test_api.py
 tests/test_async_executor.py
 tests/test_aws.py
+tests/test_barman.py
 tests/test_bootstrap.py
 tests/test_callback_executor.py
 tests/test_cancellable.py
 tests/test_citus.py
 tests/test_config.py
 tests/test_config_generator.py
 tests/test_consul.py
@@ -73,14 +83,15 @@
 tests/test_etcd.py
 tests/test_etcd3.py
 tests/test_exhibitor.py
 tests/test_file_perm.py
 tests/test_ha.py
 tests/test_kubernetes.py
 tests/test_log.py
+tests/test_mpp.py
 tests/test_patroni.py
 tests/test_postgresql.py
 tests/test_postmaster.py
 tests/test_raft.py
 tests/test_raft_controller.py
 tests/test_rewind.py
 tests/test_slots.py
```

### Comparing `patroni-3.2.2/patroni.egg-info/requires.txt` & `patroni-3.3.0/patroni.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 prettytable>=0.7
 python-dateutil
 psutil>=2.0.0
 ydiff>=1.2.0
 
 [all]
 python-etcd<0.5,>=0.4.3
-kazoo>=1.3.1
-boto3
 pysyncobj>=0.3.8
-cryptography>=1.4
 python-consul>=0.7.1
+cryptography>=1.4
+boto3
+kazoo>=1.3.1
+python-json-logger>=2.0.2
 
 [aws]
 boto3
 
 [consul]
 python-consul>=0.7.1
 
@@ -25,14 +26,17 @@
 
 [etcd3]
 python-etcd<0.5,>=0.4.3
 
 [exhibitor]
 kazoo>=1.3.1
 
+[jsonlogger]
+python-json-logger>=2.0.2
+
 [kubernetes]
 
 [psycopg2]
 psycopg2>=2.5.4
 
 [psycopg2-binary]
 psycopg2-binary
```

### Comparing `patroni-3.2.2/setup.py` & `patroni-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 AUTHOR = 'Alexander Kukushkin, Polina Bungina'
 AUTHOR_EMAIL = 'akukushkin@microsoft.com, polina.bungina@zalando.de'
 KEYWORDS = 'etcd governor patroni postgresql postgres ha haproxy confd' +\
     ' zookeeper exhibitor consul streaming replication kubernetes k8s'
 
 EXTRAS_REQUIRE = {'aws': ['boto3'], 'etcd': ['python-etcd'], 'etcd3': ['python-etcd'],
                   'consul': ['python-consul'], 'exhibitor': ['kazoo'], 'zookeeper': ['kazoo'],
-                  'kubernetes': [], 'raft': ['pysyncobj', 'cryptography']}
+                  'kubernetes': [], 'raft': ['pysyncobj', 'cryptography'], 'jsonlogger': ['python-json-logger']}
 
 # Add here all kinds of additional classifiers as defined under
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Developers',
@@ -50,15 +50,16 @@
     'Programming Language :: Python :: Implementation :: CPython',
 ]
 
 CONSOLE_SCRIPTS = ['patroni = patroni.__main__:main',
                    'patronictl = patroni.ctl:ctl',
                    'patroni_raft_controller = patroni.raft_controller:main',
                    "patroni_wale_restore = patroni.scripts.wale_restore:main",
-                   "patroni_aws = patroni.scripts.aws:main"]
+                   "patroni_aws = patroni.scripts.aws:main",
+                   "patroni_barman = patroni.scripts.barman.cli:main"]
 
 
 class _Command(Command):
     user_options = []
 
     def initialize_options(self):
         pass
```

### Comparing `patroni-3.2.2/tests/test_api.py` & `patroni-3.3.0/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import socket
 
 from http.server import HTTPServer
 from io import BytesIO as IO
 from mock import Mock, PropertyMock, patch
 from socketserver import ThreadingMixIn
 
+from patroni import global_config
 from patroni.api import RestApiHandler, RestApiServer
-from patroni.config import GlobalConfig
 from patroni.dcs import ClusterConfig, Member
 from patroni.exceptions import PostgresConnectionException
 from patroni.ha import _MemberStatus
+from patroni.postgresql.config import get_param_diff
 from patroni.psycopg import OperationalError
 from patroni.utils import RetryFailedError, tzutc
 
 from . import MockConnect, psycopg_connect
 from .test_ha import get_cluster_initialized_without_leader
 
 
@@ -50,21 +51,21 @@
     name = 'test'
     state = 'running'
     role = 'primary'
     server_version = 90625
     major_version = 90600
     sysid = 'dummysysid'
     scope = 'dummy'
-    pending_restart = True
+    pending_restart_reason = {}
     wal_name = 'wal'
     lsn_name = 'lsn'
     wal_flush = '_flush'
     POSTMASTER_START_TIME = 'pg_catalog.pg_postmaster_start_time()'
     TL_LSN = 'CASE WHEN pg_catalog.pg_is_in_recovery()'
-    citus_handler = Mock()
+    mpp_handler = Mock()
 
     @staticmethod
     def postmaster_start_time():
         return postmaster_start_time
 
     @staticmethod
     def replica_cached_timeline(_):
@@ -144,24 +145,17 @@
 class MockLogger(object):
 
     NORMAL_LOG_QUEUE_SIZE = 2
     queue_size = 3
     records_lost = 1
 
 
-class MockConfig(object):
-
-    def get_global_config(self, _):
-        return GlobalConfig({})
-
-
 class MockPatroni(object):
 
     ha = MockHa()
-    config = MockConfig()
     postgresql = ha.state_handler
     dcs = Mock()
     logger = MockLogger()
     tags = {"key1": True, "key2": False, "key3": 1, "key4": 1.4, "key5": "RandomTag"}
     version = '0.00'
     noloadbalance = PropertyMock(return_value=False)
     scheduled_restart = {'schedule': future_restart_time,
@@ -205,17 +199,18 @@
 @patch('ssl.SSLContext.wrap_socket', Mock(return_value=0))
 @patch.object(HTTPServer, '__init__', Mock())
 class TestRestApiHandler(unittest.TestCase):
 
     _authorization = '\nAuthorization: Basic dGVzdDp0ZXN0'
 
     def test_do_GET(self):
+        MockPostgresql.pending_restart_reason = {'max_connections': get_param_diff('200', '100')}
         MockPatroni.dcs.cluster.last_lsn = 20
         MockPatroni.dcs.cluster.sync.members = [MockPostgresql.name]
-        with patch.object(GlobalConfig, 'is_synchronous_mode', PropertyMock(return_value=True)):
+        with patch.object(global_config.__class__, 'is_synchronous_mode', PropertyMock(return_value=True)):
             MockRestApiServer(RestApiHandler, 'GET /replica')
         MockRestApiServer(RestApiHandler, 'GET /replica?lag=1M')
         MockRestApiServer(RestApiHandler, 'GET /replica?lag=10MB')
         MockRestApiServer(RestApiHandler, 'GET /replica?lag=10485760')
         MockRestApiServer(RestApiHandler, 'GET /read-only')
         with patch.object(RestApiHandler, 'get_postgresql_status', Mock(return_value={})):
             MockRestApiServer(RestApiHandler, 'GET /replica')
@@ -230,26 +225,26 @@
             MockRestApiServer(RestApiHandler, 'GET /read-only-sync')
         with patch.object(RestApiHandler, 'get_postgresql_status', Mock(return_value={'role': 'replica'})):
             MockPatroni.dcs.cluster.sync.members = []
             MockRestApiServer(RestApiHandler, 'GET /asynchronous')
         with patch.object(MockHa, 'is_leader', Mock(return_value=True)):
             MockRestApiServer(RestApiHandler, 'GET /replica')
             MockRestApiServer(RestApiHandler, 'GET /read-only-sync')
-            with patch.object(GlobalConfig, 'is_standby_cluster', Mock(return_value=True)):
+            with patch.object(global_config.__class__, 'is_standby_cluster', Mock(return_value=True)):
                 MockRestApiServer(RestApiHandler, 'GET /standby_leader')
         MockPatroni.dcs.cluster = None
         with patch.object(RestApiHandler, 'get_postgresql_status', Mock(return_value={'role': 'primary'})):
             MockRestApiServer(RestApiHandler, 'GET /primary')
         with patch.object(MockHa, 'restart_scheduled', Mock(return_value=True)):
             MockRestApiServer(RestApiHandler, 'GET /primary')
         self.assertIsNotNone(MockRestApiServer(RestApiHandler, 'GET /primary'))
         with patch.object(RestApiServer, 'query', Mock(return_value=[('', 1, '', '', '', '', False, None, None, '')])):
             self.assertIsNotNone(MockRestApiServer(RestApiHandler, 'GET /patroni'))
-        with patch.object(GlobalConfig, 'is_standby_cluster', Mock(return_value=True)), \
-                patch.object(GlobalConfig, 'is_paused', Mock(return_value=True)):
+        with patch.object(global_config.__class__, 'is_standby_cluster', Mock(return_value=True)), \
+                patch.object(global_config.__class__, 'is_paused', Mock(return_value=True)):
             MockRestApiServer(RestApiHandler, 'GET /standby_leader')
 
         # test tags
         #
         MockRestApiServer(RestApiHandler, 'GET /primary?lag=1M&'
                                           'tag_key1=true&tag_key2=false&'
                                           'tag_key3=1&tag_key4=1.4&tag_key5=RandomTag')
@@ -471,15 +466,15 @@
             with patch.object(MockHa, 'schedule_future_restart', Mock(return_value=retval)):
                 request = make_request(schedule=future_restart_time.isoformat())
                 MockRestApiServer(RestApiHandler, request)
             with patch.object(MockHa, 'restart', Mock(return_value=(retval, "foo"))):
                 request = make_request(role='primary', postgres_version='9.5.2')
                 MockRestApiServer(RestApiHandler, request)
 
-        with patch.object(GlobalConfig, 'is_paused', PropertyMock(return_value=True)):
+        with patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=True)):
             MockRestApiServer(RestApiHandler, make_request(schedule='2016-08-42 12:45TZ+1', role='primary'))
             # Valid timeout
             MockRestApiServer(RestApiHandler, make_request(timeout='60s'))
             # Invalid timeout
             MockRestApiServer(RestApiHandler, make_request(timeout='42towels'))
 
     def test_do_DELETE_restart(self):
@@ -533,24 +528,25 @@
             request = post + '25\n\n{"leader": "postgresql1"}'
             MockRestApiServer(RestApiHandler, request)
             response_mock.assert_called_with(
                 412, 'switchover is not possible: cluster does not have members except leader')
 
         # Switchover in pause mode
         with patch.object(RestApiHandler, 'write_response') as response_mock, \
-             patch.object(GlobalConfig, 'is_paused', PropertyMock(return_value=True)):
+             patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=True)):
             MockRestApiServer(RestApiHandler, request)
             response_mock.assert_called_with(
                 400, 'Switchover is possible only to a specific candidate in a paused state')
 
         # No healthy nodes to promote in both sync and async mode
         for is_synchronous_mode, response in (
                 (True, 'switchover is not possible: can not find sync_standby'),
                 (False, 'switchover is not possible: cluster does not have members except leader')):
-            with patch.object(GlobalConfig, 'is_synchronous_mode', PropertyMock(return_value=is_synchronous_mode)), \
+            with patch.object(global_config.__class__, 'is_synchronous_mode',
+                              PropertyMock(return_value=is_synchronous_mode)), \
                  patch.object(RestApiHandler, 'write_response') as response_mock:
                 MockRestApiServer(RestApiHandler, request)
                 response_mock.assert_called_with(412, response)
 
         # [Switchover to the candidate specified]
 
         # Candidate to promote is the same as the leader specified
@@ -567,15 +563,16 @@
             response_mock.assert_called_with(412, 'leader name does not match')
 
         # Candidate to promote is not a member of the cluster
         cluster.leader.name = 'postgresql1'
         cluster.sync.matches.return_value = False
         for is_synchronous_mode, response in (
                 (True, 'candidate name does not match with sync_standby'), (False, 'candidate does not exists')):
-            with patch.object(GlobalConfig, 'is_synchronous_mode', PropertyMock(return_value=is_synchronous_mode)), \
+            with patch.object(global_config.__class__, 'is_synchronous_mode',
+                              PropertyMock(return_value=is_synchronous_mode)), \
                  patch.object(RestApiHandler, 'write_response') as response_mock:
                 MockRestApiServer(RestApiHandler, request)
                 response_mock.assert_called_with(412, response)
 
         cluster.members = [Member(0, 'postgresql0', 30, {'api_url': 'http'}),
                            Member(0, 'postgresql2', 30, {'api_url': 'http'})]
 
@@ -628,15 +625,15 @@
             request = post + '103\n\n{"leader": "postgresql1", "member": "postgresql2",' + \
                              ' "scheduled_at": "6016-02-15T18:13:30.568224+01:00"}'
             MockRestApiServer(RestApiHandler, request)
             response_mock.assert_called_with(202, 'Switchover scheduled')
 
         # Schedule in paused mode
         with patch.object(RestApiHandler, 'write_response') as response_mock, \
-             patch.object(GlobalConfig, 'is_paused', PropertyMock(return_value=True)):
+             patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=True)):
             dcs.manual_failover.return_value = False
             MockRestApiServer(RestApiHandler, request)
             response_mock.assert_called_with(400, "Can't schedule switchover in the paused state")
 
         # No timezone specified
         with patch.object(RestApiHandler, 'write_response') as response_mock:
             request = post + '97\n\n{"leader": "postgresql1", "member": "postgresql2",' + \
@@ -674,14 +671,20 @@
 
     @patch.object(MockHa, 'is_leader', Mock(return_value=True))
     def test_do_POST_citus(self):
         post = 'POST /citus HTTP/1.0' + self._authorization + '\nContent-Length: '
         MockRestApiServer(RestApiHandler, post + '0\n\n')
         MockRestApiServer(RestApiHandler, post + '14\n\n{"leader":"1"}')
 
+    @patch.object(MockHa, 'is_leader', Mock(return_value=True))
+    def test_do_POST_mpp(self):
+        post = 'POST /mpp HTTP/1.0' + self._authorization + '\nContent-Length: '
+        MockRestApiServer(RestApiHandler, post + '0\n\n')
+        MockRestApiServer(RestApiHandler, post + '14\n\n{"leader":"1"}')
+
 
 class TestRestApiServer(unittest.TestCase):
 
     @patch('ssl.SSLContext.load_cert_chain', Mock())
     @patch('ssl.SSLContext.set_ciphers', Mock())
     @patch('ssl.SSLContext.wrap_socket', Mock(return_value=0))
     @patch.object(HTTPServer, '__init__', Mock())
```

### Comparing `patroni-3.2.2/tests/test_async_executor.py` & `patroni-3.3.0/tests/test_async_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_aws.py` & `patroni-3.3.0/tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_bootstrap.py` & `patroni-3.3.0/tests/test_bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import sys
 
 from mock import Mock, PropertyMock, patch
 
 from patroni.async_executor import CriticalTask
+from patroni.collections import CaseInsensitiveDict
 from patroni.postgresql import Postgresql
 from patroni.postgresql.bootstrap import Bootstrap
 from patroni.postgresql.cancellable import CancellableSubprocess
-from patroni.postgresql.config import ConfigHandler
+from patroni.postgresql.config import ConfigHandler, get_param_diff
 
 from . import psycopg_connect, BaseTestPostgresql, mock_available_gucs
 
 
 @patch('subprocess.call', Mock(return_value=0))
 @patch('patroni.psycopg.connect', psycopg_connect)
 @patch('os.rename', Mock())
@@ -138,14 +139,24 @@
             self.assertEqual(
                 self.b.process_user_options(
                     'initdb',
                     {'key': "'value with spaces'"},
                     (), error_handler
                 ),
                 ["--key=value with spaces"])
+            # not allowed options in list of dicts/strs are filtered out
+            self.assertEqual(
+                self.b.process_user_options(
+                    'pg_basebackup',
+                    [{'checkpoint': 'fast'}, {'dbname': 'dbname=postgres'}, 'gzip', {'label': 'standby'}, 'verbose'],
+                    ('dbname', 'verbose'),
+                    print
+                ),
+                ['--checkpoint=fast', '--gzip', '--label=standby'],
+            )
 
     @patch.object(CancellableSubprocess, 'call', Mock())
     @patch.object(Postgresql, 'is_running', Mock(return_value=True))
     @patch.object(Postgresql, 'data_directory_empty', Mock(return_value=False))
     @patch.object(Postgresql, 'controldata', Mock(return_value={'max_connections setting': 100,
                                                                 'max_prepared_xacts setting': 0,
                                                                 'max_locks_per_xact setting': 64}))
@@ -231,16 +242,17 @@
             self.assertFalse(task.result)
 
         self.p.config._config.pop('pg_hba')
         self.b.post_bootstrap({}, task)
         self.assertTrue(task.result)
 
         self.b.bootstrap(config)
-        with patch.object(Postgresql, 'pending_restart', PropertyMock(return_value=True)), \
-                patch.object(Postgresql, 'restart', Mock()) as mock_restart:
+        with patch.object(Postgresql, 'pending_restart_reason',
+                          PropertyMock(CaseInsensitiveDict({'max_connections': get_param_diff('200', '100')}))), \
+             patch.object(Postgresql, 'restart', Mock()) as mock_restart:
             self.b.post_bootstrap({}, task)
             mock_restart.assert_called_once()
 
         self.b.bootstrap(config)
         self.p.set_state('stopped')
         self.p.reload_config({'authentication': {'superuser': {'username': 'p', 'password': 'p'},
                                                  'replication': {'username': 'r', 'password': 'r'},
```

### Comparing `patroni-3.2.2/tests/test_callback_executor.py` & `patroni-3.3.0/tests/test_callback_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_cancellable.py` & `patroni-3.3.0/tests/test_cancellable.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_citus.py` & `patroni-3.3.0/tests/test_citus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import time
 from mock import Mock, patch, PropertyMock
-from patroni.postgresql.citus import CitusHandler
+from patroni.postgresql.mpp.citus import CitusHandler
 from patroni.psycopg import ProgrammingError
 
 from . import BaseTestPostgresql, MockCursor, psycopg_connect, SleepException
 from .test_ha import get_cluster_initialized_with_leader
 
 
-@patch('patroni.postgresql.citus.Thread', Mock())
+@patch('patroni.postgresql.mpp.citus.Thread', Mock())
 @patch('patroni.psycopg.connect', psycopg_connect)
 class TestCitus(BaseTestPostgresql):
 
     def setUp(self):
         super(TestCitus, self).setUp()
-        self.c = self.p.citus_handler
+        self.c = self.p.mpp_handler
         self.cluster = get_cluster_initialized_with_leader()
         self.cluster.workers[1] = self.cluster
 
     @patch('time.time', Mock(side_effect=[100, 130, 160, 190, 220, 250, 280, 310, 340, 370]))
-    @patch('patroni.postgresql.citus.logger.exception', Mock(side_effect=SleepException))
-    @patch('patroni.postgresql.citus.logger.warning')
-    @patch('patroni.postgresql.citus.PgDistNode.wait', Mock())
+    @patch('patroni.postgresql.mpp.citus.logger.exception', Mock(side_effect=SleepException))
+    @patch('patroni.postgresql.mpp.citus.logger.warning')
+    @patch('patroni.postgresql.mpp.citus.PgDistNode.wait', Mock())
     @patch.object(CitusHandler, 'is_alive', Mock(return_value=True))
     def test_run(self, mock_logger_warning):
         # `before_demote` or `before_promote` REST API calls starting a
         # transaction. We want to make sure that it finishes during
         # certain timeout. In case if it is not, we want to roll it back
         # in order to not block other workers that want to update
         # `pg_dist_node`.
@@ -36,42 +36,42 @@
         self.assertRaises(SleepException, self.c.run)
         mock_logger_warning.assert_called_once()
         self.assertTrue(mock_logger_warning.call_args[0][0].startswith('Rolling back transaction'))
         self.assertTrue(repr(mock_logger_warning.call_args[0][1]).startswith('PgDistNode'))
 
     @patch.object(CitusHandler, 'is_alive', Mock(return_value=False))
     @patch.object(CitusHandler, 'start', Mock())
-    def test_sync_pg_dist_node(self):
+    def test_sync_meta_data(self):
         with patch.object(CitusHandler, 'is_enabled', Mock(return_value=False)):
-            self.c.sync_pg_dist_node(self.cluster)
-        self.c.sync_pg_dist_node(self.cluster)
+            self.c.sync_meta_data(self.cluster)
+        self.c.sync_meta_data(self.cluster)
 
     def test_handle_event(self):
         self.c.handle_event(self.cluster, {})
         with patch.object(CitusHandler, 'is_alive', Mock(return_value=True)):
             self.c.handle_event(self.cluster, {'type': 'after_promote', 'group': 2,
                                                'leader': 'leader', 'timeout': 30, 'cooldown': 10})
 
     def test_add_task(self):
-        with patch('patroni.postgresql.citus.logger.error') as mock_logger, \
-                patch('patroni.postgresql.citus.urlparse', Mock(side_effect=Exception)):
+        with patch('patroni.postgresql.mpp.citus.logger.error') as mock_logger, \
+                patch('patroni.postgresql.mpp.citus.urlparse', Mock(side_effect=Exception)):
             self.c.add_task('', 1, None)
             mock_logger.assert_called_once()
 
-        with patch('patroni.postgresql.citus.logger.debug') as mock_logger:
+        with patch('patroni.postgresql.mpp.citus.logger.debug') as mock_logger:
             self.c.add_task('before_demote', 1, 'postgres://host:5432/postgres', 30)
             mock_logger.assert_called_once()
             self.assertTrue(mock_logger.call_args[0][0].startswith('Adding the new task:'))
 
-        with patch('patroni.postgresql.citus.logger.debug') as mock_logger:
+        with patch('patroni.postgresql.mpp.citus.logger.debug') as mock_logger:
             self.c.add_task('before_promote', 1, 'postgres://host:5432/postgres', 30)
             mock_logger.assert_called_once()
             self.assertTrue(mock_logger.call_args[0][0].startswith('Overriding existing task:'))
 
-        # add_task called from sync_pg_dist_node should not override already scheduled or in flight task until deadline
+        # add_task called from sync_meta_data should not override already scheduled or in flight task until deadline
         self.assertIsNotNone(self.c.add_task('after_promote', 1, 'postgres://host:5432/postgres', 30))
         self.assertIsNone(self.c.add_task('after_promote', 1, 'postgres://host:5432/postgres'))
         self.c._in_flight = self.c._tasks.pop()
         self.c._in_flight.deadline = self.c._in_flight.timeout + time.time()
         self.assertIsNone(self.c.add_task('after_promote', 1, 'postgres://host:5432/postgres'))
         self.c._in_flight.deadline = 0
         self.assertIsNotNone(self.c.add_task('after_promote', 1, 'postgres://host:5432/postgres'))
@@ -103,24 +103,24 @@
             self.assertEqual(mock_query.call_args[0][0], 'COMMIT')
 
     def test_process_tasks(self):
         self.c.add_task('after_promote', 0, 'postgres://host2:5432/postgres')
         self.c.process_tasks()
 
         self.c.add_task('after_promote', 0, 'postgres://host3:5432/postgres')
-        with patch('patroni.postgresql.citus.logger.error') as mock_logger, \
+        with patch('patroni.postgresql.mpp.citus.logger.error') as mock_logger, \
                 patch.object(CitusHandler, 'query', Mock(side_effect=Exception)):
             self.c.process_tasks()
             mock_logger.assert_called_once()
             self.assertTrue(mock_logger.call_args[0][0].startswith('Exception when working with pg_dist_node: '))
 
     def test_on_demote(self):
         self.c.on_demote()
 
-    @patch('patroni.postgresql.citus.logger.error')
+    @patch('patroni.postgresql.mpp.citus.logger.error')
     @patch.object(MockCursor, 'execute', Mock(side_effect=Exception))
     def test_load_pg_dist_node(self, mock_logger):
         # load_pg_dist_node() triggers, query fails and exception is property handled
         self.c.process_tasks()
         self.assertTrue(self.c._schedule_load_pg_dist_node)
         mock_logger.assert_called_once()
         self.assertTrue(mock_logger.call_args[0][0].startswith('Exception when executing query'))
@@ -137,18 +137,14 @@
                       'shared_preload_libraries': 'foo , citus, bar '}
         self.c.adjust_postgres_gucs(parameters)
         self.assertEqual(parameters['max_prepared_transactions'], 202)
         self.assertEqual(parameters['shared_preload_libraries'], 'citus,foo,bar')
         self.assertEqual(parameters['wal_level'], 'logical')
         self.assertEqual(parameters['citus.local_hostname'], '/tmp')
 
-    def test_bootstrap(self):
-        self.c._config = None
-        self.c.bootstrap()
-
     def test_ignore_replication_slot(self):
         self.assertFalse(self.c.ignore_replication_slot({'name': 'foo', 'type': 'physical',
                                                          'database': 'bar', 'plugin': 'wal2json'}))
         self.assertFalse(self.c.ignore_replication_slot({'name': 'foo', 'type': 'logical',
                                                          'database': 'bar', 'plugin': 'wal2json'}))
         self.assertFalse(self.c.ignore_replication_slot({'name': 'foo', 'type': 'logical',
                                                          'database': 'bar', 'plugin': 'pgoutput'}))
@@ -159,17 +155,17 @@
         self.assertFalse(self.c.ignore_replication_slot({'name': 'citus_shard_move_slot_1_2_3',
                                                          'type': 'logical', 'database': 'citus', 'plugin': 'citus'}))
         self.assertFalse(self.c.ignore_replication_slot({'name': 'citus_shard_split_slot_1_2_3',
                                                          'type': 'logical', 'database': 'citus', 'plugin': 'pgoutput'}))
         self.assertTrue(self.c.ignore_replication_slot({'name': 'citus_shard_split_slot_1_2_3',
                                                         'type': 'logical', 'database': 'citus', 'plugin': 'citus'}))
 
-    @patch('patroni.postgresql.citus.logger.debug')
-    @patch('patroni.postgresql.citus.connect', psycopg_connect)
-    @patch('patroni.postgresql.citus.quote_ident', Mock())
+    @patch('patroni.postgresql.mpp.citus.logger.debug')
+    @patch('patroni.postgresql.mpp.citus.connect', psycopg_connect)
+    @patch('patroni.postgresql.mpp.citus.quote_ident', Mock())
     def test_bootstrap_duplicate_database(self, mock_logger):
         with patch.object(MockCursor, 'execute', Mock(side_effect=ProgrammingError)):
             self.assertRaises(ProgrammingError, self.c.bootstrap)
         with patch.object(MockCursor, 'execute', Mock(side_effect=[ProgrammingError, None, None, None])), \
                 patch.object(ProgrammingError, 'diag') as mock_diag:
             type(mock_diag).sqlstate = PropertyMock(return_value='42P04')
             self.c.bootstrap()
```

### Comparing `patroni-3.2.2/tests/test_config.py` & `patroni-3.3.0/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import os
 import sys
 import unittest
 import io
 
 from copy import deepcopy
 from mock import MagicMock, Mock, patch
-from patroni.config import Config, ConfigParseError, GlobalConfig
+
+from patroni import global_config
+from patroni.config import ClusterConfig, Config, ConfigParseError
+
+from .test_ha import get_cluster_initialized_with_only_leader
 
 
 class TestConfig(unittest.TestCase):
 
     @patch('os.path.isfile', Mock(return_value=True))
     @patch('json.load', Mock(side_effect=Exception))
     @patch('builtins.open', MagicMock())
@@ -27,14 +31,15 @@
 
     def test_reload_local_configuration(self):
         os.environ.update({
             'PATRONI_NAME': 'postgres0',
             'PATRONI_NAMESPACE': '/patroni/',
             'PATRONI_SCOPE': 'batman2',
             'PATRONI_LOGLEVEL': 'ERROR',
+            'PATRONI_LOG_FORMAT': '["message", {"levelname": "level"}]',
             'PATRONI_LOG_LOGGERS': 'patroni.postmaster: WARNING, urllib3: DEBUG',
             'PATRONI_LOG_FILE_NUM': '5',
             'PATRONI_CITUS_DATABASE': 'citus',
             'PATRONI_CITUS_GROUP': '0',
             'PATRONI_CITUS_HOST': '0',
             'PATRONI_RESTAPI_USERNAME': 'username',
             'PATRONI_RESTAPI_PASSWORD': 'password',
@@ -151,41 +156,39 @@
     def test_invalid_path(self):
         self.assertRaises(ConfigParseError, Config, 'postgres0')
 
     @patch.object(Config, 'get')
     @patch('patroni.config.logger')
     def test__validate_failover_tags(self, mock_logger, mock_get):
         """Ensures that only one of `nofailover` or `failover_priority` can be provided"""
-        config = Config("postgres0.yml")
-
         # Providing one of `nofailover` or `failover_priority` is fine
         for single_param in ({"nofailover": True}, {"failover_priority": 1}, {"failover_priority": 0}):
             mock_get.side_effect = [single_param] * 2
-            self.assertIsNone(config._validate_failover_tags())
+            self.assertIsNone(self.config._validate_failover_tags())
             mock_logger.warning.assert_not_called()
 
         # Providing both `nofailover` and `failover_priority` is fine if consistent
         for consistent_state in (
             {"nofailover": False, "failover_priority": 1},
             {"nofailover": True, "failover_priority": 0},
             {"nofailover": "False", "failover_priority": 0}
         ):
             mock_get.side_effect = [consistent_state] * 2
-            self.assertIsNone(config._validate_failover_tags())
+            self.assertIsNone(self.config._validate_failover_tags())
             mock_logger.warning.assert_not_called()
 
         # Providing both inconsistently should log a warning
         for inconsistent_state in (
             {"nofailover": False, "failover_priority": 0},
             {"nofailover": True, "failover_priority": 1},
             {"nofailover": "False", "failover_priority": 1},
             {"nofailover": "", "failover_priority": 0}
         ):
             mock_get.side_effect = [inconsistent_state] * 2
-            self.assertIsNone(config._validate_failover_tags())
+            self.assertIsNone(self.config._validate_failover_tags())
             mock_logger.warning.assert_called_once_with(
                 'Conflicting configuration between nofailover: %s and failover_priority: %s.'
                 + ' Defaulting to nofailover: %s',
                 inconsistent_state['nofailover'],
                 inconsistent_state['failover_priority'],
                 inconsistent_state['nofailover'])
             mock_logger.warning.reset_mock()
@@ -236,8 +239,10 @@
             self.assertEqual(mock_logger.call_args_list[0][0],
                              ('Violated the rule "loop_wait + 2*retry_timeout <= ttl", where ttl=%d. Adjusting'
                               ' loop_wait from %d to %d and retry_timeout from %d to %d', 20, 10, 1, 10, 9))
 
     def test_global_config_is_synchronous_mode(self):
         # we should ignore synchronous_mode setting in a standby cluster
         config = {'standby_cluster': {'host': 'some_host'}, 'synchronous_mode': True}
-        self.assertFalse(GlobalConfig(config).is_synchronous_mode)
+        cluster = get_cluster_initialized_with_only_leader(cluster_config=ClusterConfig(1, config, 1))
+        test_config = global_config.from_cluster(cluster)
+        self.assertFalse(test_config.is_synchronous_mode)
```

### Comparing `patroni-3.2.2/tests/test_config_generator.py` & `patroni-3.3.0/tests/test_config_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,18 @@
         dynamic_config['postgresql']['parameters']['wal_keep_segments'] = 8
         dynamic_config['postgresql']['use_pg_rewind'] = True
 
         self.config = {
             'scope': self.environ['PATRONI_SCOPE'],
             'name': HOSTNAME,
             'log': {
+                'type': PatroniLogger.DEFAULT_TYPE,
+                'format': PatroniLogger.DEFAULT_FORMAT,
                 'level': PatroniLogger.DEFAULT_LEVEL,
                 'traceback_level': PatroniLogger.DEFAULT_TRACEBACK_LEVEL,
-                'format': PatroniLogger.DEFAULT_FORMAT,
                 'max_queue_size': PatroniLogger.DEFAULT_MAX_QUEUE_SIZE
             },
             'restapi': {
                 'connect_address': self.environ['PATRONI_RESTAPI_CONNECT_ADDRESS'],
                 'listen': self.environ['PATRONI_RESTAPI_LISTEN']
             },
             'bootstrap': {
@@ -137,14 +138,15 @@
                 },
             },
             'tags': {
                 'failover_priority': 1,
                 'noloadbalance': False,
                 'clonefrom': True,
                 'nosync': False,
+                'nostream': False
             }
         }
         patch_config(self.config, conf)
 
     def _get_running_instance_open_res(self):
         hba_content = '\n'.join(self.config['postgresql']['pg_hba'] + ['#host all all all md5',
                                                                        '  host all all all md5',
```

### Comparing `patroni-3.2.2/tests/test_consul.py` & `patroni-3.3.0/tests/test_consul.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import consul
 import unittest
 
 from consul import ConsulException, NotFound
 from mock import Mock, PropertyMock, patch
+from patroni.dcs import get_dcs
 from patroni.dcs.consul import AbstractDCS, Cluster, Consul, ConsulInternalError, \
     ConsulError, ConsulClient, HTTPClient, InvalidSessionTTL, InvalidSession, RetryFailedError
+from patroni.postgresql.mpp import get_mpp
 from . import SleepException
 
 
 def kv_get(self, key, **kwargs):
     if key == 'service/test/members/postgresql1':
         return '1', {'Session': 'fd4f44fe-2cac-bba5-a60b-304b51ff39b7'}
     if key == 'service/test/':
@@ -87,21 +89,25 @@
 class TestConsul(unittest.TestCase):
 
     @patch.object(consul.Consul.Session, 'create', Mock(return_value='fd4f44fe-2cac-bba5-a60b-304b51ff39b7'))
     @patch.object(consul.Consul.Session, 'renew', Mock(side_effect=NotFound))
     @patch.object(consul.Consul.KV, 'get', kv_get)
     @patch.object(consul.Consul.KV, 'delete', Mock())
     def setUp(self):
-        Consul({'ttl': 30, 'scope': 't', 'name': 'p', 'url': 'https://l:1', 'retry_timeout': 10,
-                'verify': 'on', 'key': 'foo', 'cert': 'bar', 'cacert': 'buz', 'token': 'asd', 'dc': 'dc1',
-                'register_service': True})
-        Consul({'ttl': 30, 'scope': 't_', 'name': 'p', 'url': 'https://l:1', 'retry_timeout': 10,
-                'verify': 'on', 'cert': 'bar', 'cacert': 'buz', 'register_service': True})
-        self.c = Consul({'ttl': 30, 'scope': 'test', 'name': 'postgresql1', 'host': 'localhost:1', 'retry_timeout': 10,
-                         'register_service': True, 'service_check_tls_server_name': True})
+        self.assertIsInstance(get_dcs({'ttl': 30, 'scope': 't', 'name': 'p', 'retry_timeout': 10,
+                                       'consul': {'url': 'https://l:1', 'verify': 'on',
+                                                  'key': 'foo', 'cert': 'bar', 'cacert': 'buz',
+                                                  'token': 'asd', 'dc': 'dc1', 'register_service': True}}), Consul)
+        self.assertIsInstance(get_dcs({'ttl': 30, 'scope': 't_', 'name': 'p', 'retry_timeout': 10,
+                                       'consul': {'url': 'https://l:1', 'verify': 'on',
+                                                  'cert': 'bar', 'cacert': 'buz', 'register_service': True}}), Consul)
+        self.c = get_dcs({'ttl': 30, 'scope': 'test', 'name': 'postgresql1', 'retry_timeout': 10,
+                          'consul': {'host': 'localhost:1', 'register_service': True,
+                                     'service_check_tls_server_name': True}})
+        self.assertIsInstance(self.c, Consul)
         self.c._base_path = 'service/good'
         self.c.get_cluster()
 
     @patch('time.sleep', Mock(side_effect=SleepException))
     @patch.object(consul.Consul.Session, 'create', Mock(side_effect=ConsulException))
     def test_create_session(self):
         self.c._session = None
@@ -126,15 +132,15 @@
         self.assertRaises(ConsulError, self.c.get_cluster)
         self.c._base_path = 'service/broken'
         self.assertIsInstance(self.c.get_cluster(), Cluster)
         self.c._base_path = 'service/legacy'
         self.assertIsInstance(self.c.get_cluster(), Cluster)
 
     def test__get_citus_cluster(self):
-        self.c._citus_group = '0'
+        self.c._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
         cluster = self.c.get_cluster()
         self.assertIsInstance(cluster, Cluster)
         self.assertIsInstance(cluster.workers[1], Cluster)
 
     @patch.object(consul.Consul.KV, 'delete', Mock(side_effect=[ConsulException, True, True, True]))
     @patch.object(consul.Consul.KV, 'put', Mock(side_effect=[True, ConsulException, InvalidSession]))
     def test_touch_member(self):
@@ -150,18 +156,16 @@
         self.assertFalse(self.c.touch_member({'balbla': 'blabla'}))
 
     @patch.object(consul.Consul.KV, 'put', Mock(side_effect=[InvalidSession, False, InvalidSession]))
     def test_take_leader(self):
         self.c.set_ttl(20)
         self.c._do_refresh_session = Mock()
         self.assertFalse(self.c.take_leader())
-        with patch('time.time', Mock(side_effect=[0, 100])):
-            self.assertRaises(ConsulError, self.c.take_leader)
-        with patch('time.time', Mock(side_effect=[0, 0, 0, 0, 0, 0, 100])):
-            self.assertRaises(ConsulError, self.c.take_leader)
+        with patch('time.time', Mock(side_effect=[0, 0, 0, 100, 100, 100])):
+            self.assertFalse(self.c.take_leader())
 
     @patch.object(consul.Consul.KV, 'put', Mock(return_value=True))
     def test_set_failover_value(self):
         self.c.set_failover_value('')
 
     @patch.object(consul.Consul.KV, 'put', Mock(return_value=True))
     def test_set_config_value(self):
```

### Comparing `patroni-3.2.2/tests/test_ctl.py` & `patroni-3.3.0/tests/test_ctl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,54 @@
+import click
 import etcd
 import mock
 import os
 import unittest
 
 from click.testing import CliRunner
 from datetime import datetime, timedelta
 from mock import patch, Mock, PropertyMock
+from patroni import global_config
 from patroni.ctl import ctl, load_config, output_members, get_dcs, parse_dcs, \
     get_all_members, get_any_member, get_cursor, query_member, PatroniCtlException, apply_config_changes, \
     format_config_for_editing, show_diff, invoke_editor, format_pg_version, CONFIG_FILE_PATH, PatronictlPrettyTable
-from patroni.dcs.etcd import AbstractEtcdClientWithFailover, Cluster, Failover
+from patroni.dcs import Cluster, Failover
+from patroni.postgresql.config import get_param_diff
+from patroni.postgresql.mpp import get_mpp
 from patroni.psycopg import OperationalError
 from patroni.utils import tzutc
 from prettytable import PrettyTable, ALL
 from urllib3 import PoolManager
 
 from . import MockConnect, MockCursor, MockResponse, psycopg_connect
 from .test_etcd import etcd_read, socket_getaddrinfo
 from .test_ha import get_cluster_initialized_without_leader, get_cluster_initialized_with_leader, \
     get_cluster_initialized_with_only_leader, get_cluster_not_initialized_without_leader, get_cluster, Member
 
 
-DEFAULT_CONFIG = {
-    'scope': 'alpha',
-    'restapi': {'listen': '::', 'certfile': 'a'},
-    'ctl': {'certfile': 'a'},
-    'etcd': {'host': 'localhost:2379'},
-    'citus': {'database': 'citus', 'group': 0},
-    'postgresql': {'data_dir': '.', 'pgpass': './pgpass', 'parameters': {}, 'retry_timeout': 5}
-}
+def get_default_config(*args):
+    return {
+        'scope': 'alpha',
+        'restapi': {'listen': '::', 'certfile': 'a'},
+        'ctl': {'certfile': 'a'},
+        'etcd': {'host': 'localhost:2379', 'retry_timeout': 10, 'ttl': 30},
+        'citus': {'database': 'citus', 'group': 0},
+        'postgresql': {'data_dir': '.', 'pgpass': './pgpass', 'parameters': {}, 'retry_timeout': 5}
+    }
 
 
-@patch('patroni.ctl.load_config', Mock(return_value=DEFAULT_CONFIG))
+@patch.object(PoolManager, 'request', Mock(return_value=MockResponse()))
+@patch('patroni.ctl.load_config', get_default_config)
+@patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=get_cluster_initialized_with_leader()))
 class TestCtl(unittest.TestCase):
     TEST_ROLES = ('master', 'primary', 'leader')
 
     @patch('socket.getaddrinfo', socket_getaddrinfo)
-    @patch.object(AbstractEtcdClientWithFailover, '_get_machines_list', Mock(return_value=['http://remotehost:2379']))
     def setUp(self):
         self.runner = CliRunner()
-        self.e = get_dcs({'etcd': {'ttl': 30, 'host': 'ok:2379', 'retry_timeout': 10},
-                          'citus': {'group': 0}}, 'foo', None)
 
     @patch('patroni.ctl.logging.debug')
     def test_load_config(self, mock_logger_debug):
         runner = CliRunner()
         with runner.isolated_filesystem():
             self.assertRaises(PatroniCtlException, load_config, './non-existing-config-file', None)
 
@@ -62,67 +66,66 @@
                 mock_logger_debug.assert_called_once()
                 self.assertEqual(('Loading configuration from file %s', CONFIG_FILE_PATH),
                                  mock_logger_debug.call_args[0])
                 mock_logger_debug.reset_mock()
 
     @patch('patroni.psycopg.connect', psycopg_connect)
     def test_get_cursor(self):
-        for role in self.TEST_ROLES:
-            self.assertIsNone(get_cursor({}, get_cluster_initialized_without_leader(), None, {}, role=role))
-            self.assertIsNotNone(get_cursor({}, get_cluster_initialized_with_leader(), None, {}, role=role))
+        with click.Context(click.Command('query')) as ctx:
+            ctx.obj = {'__config': {}, '__mpp': get_mpp({})}
+            for role in self.TEST_ROLES:
+                self.assertIsNone(get_cursor(get_cluster_initialized_without_leader(), None, {}, role=role))
+                self.assertIsNotNone(get_cursor(get_cluster_initialized_with_leader(), None, {}, role=role))
 
-        # MockCursor returns pg_is_in_recovery as false
-        self.assertIsNone(get_cursor({}, get_cluster_initialized_with_leader(), None, {}, role='replica'))
+            # MockCursor returns pg_is_in_recovery as false
+            self.assertIsNone(get_cursor(get_cluster_initialized_with_leader(), None, {}, role='replica'))
 
-        self.assertIsNotNone(get_cursor({}, get_cluster_initialized_with_leader(), None, {'dbname': 'foo'}, role='any'))
+            self.assertIsNotNone(get_cursor(get_cluster_initialized_with_leader(), None, {'dbname': 'foo'}, role='any'))
 
-        # Mutually exclusive options
-        with self.assertRaises(PatroniCtlException) as e:
-            get_cursor({}, get_cluster_initialized_with_leader(), None, {'dbname': 'foo'}, member_name='other',
-                       role='replica')
+            # Mutually exclusive options
+            with self.assertRaises(PatroniCtlException) as e:
+                get_cursor(get_cluster_initialized_with_leader(), None, {'dbname': 'foo'}, member_name='other',
+                           role='replica')
+
+            self.assertEqual(str(e.exception), '--role and --member are mutually exclusive options')
 
-        self.assertEqual(str(e.exception), '--role and --member are mutually exclusive options')
+            # Invalid member provided
+            self.assertIsNone(get_cursor(get_cluster_initialized_with_leader(), None, {'dbname': 'foo'},
+                                         member_name='invalid'))
 
-        # Invalid member provided
-        self.assertIsNone(get_cursor({}, get_cluster_initialized_with_leader(), None, {'dbname': 'foo'},
-                                     member_name='invalid'))
-
-        # Valid member provided
-        self.assertIsNotNone(get_cursor({}, get_cluster_initialized_with_leader(), None, {'dbname': 'foo'},
-                                        member_name='other'))
+            # Valid member provided
+            self.assertIsNotNone(get_cursor(get_cluster_initialized_with_leader(), None, {'dbname': 'foo'},
+                                            member_name='other'))
 
     def test_parse_dcs(self):
         assert parse_dcs(None) is None
         assert parse_dcs('localhost') == {'etcd': {'host': 'localhost:2379'}}
         assert parse_dcs('') == {'etcd': {'host': 'localhost:2379'}}
         assert parse_dcs('localhost:8500') == {'consul': {'host': 'localhost:8500'}}
         assert parse_dcs('zookeeper://localhost') == {'zookeeper': {'hosts': ['localhost:2181']}}
         assert parse_dcs('exhibitor://dummy') == {'exhibitor': {'hosts': ['dummy'], 'port': 8181}}
         assert parse_dcs('consul://localhost') == {'consul': {'host': 'localhost:8500'}}
         assert parse_dcs('etcd3://random.com:2399') == {'etcd3': {'host': 'random.com:2399'}}
         self.assertRaises(PatroniCtlException, parse_dcs, 'invalid://test')
 
     def test_output_members(self):
-        scheduled_at = datetime.now(tzutc) + timedelta(seconds=600)
-        cluster = get_cluster_initialized_with_leader(Failover(1, 'foo', 'bar', scheduled_at))
-        del cluster.members[1].data['conn_url']
-        for fmt in ('pretty', 'json', 'yaml', 'topology'):
-            self.assertIsNone(output_members({}, cluster, name='abc', fmt=fmt))
-
-        with patch('click.echo') as mock_echo:
-            self.assertIsNone(output_members({}, cluster, name='abc', fmt='tsv'))
-            self.assertEqual(mock_echo.call_args[0][0], 'abc\tother\t\tReplica\trunning\t\tunknown')
-
-    @patch('patroni.ctl.get_dcs')
-    @patch.object(PoolManager, 'request', Mock(return_value=MockResponse()))
-    def test_switchover(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
-        mock_get_dcs.return_value.set_failover_value = Mock()
+        with click.Context(click.Command('list')) as ctx:
+            ctx.obj = {'__config': {}, '__mpp': get_mpp({})}
+            scheduled_at = datetime.now(tzutc) + timedelta(seconds=600)
+            cluster = get_cluster_initialized_with_leader(Failover(1, 'foo', 'bar', scheduled_at))
+            del cluster.members[1].data['conn_url']
+            for fmt in ('pretty', 'json', 'yaml', 'topology'):
+                self.assertIsNone(output_members(cluster, name='abc', fmt=fmt))
+
+            with patch('click.echo') as mock_echo:
+                self.assertIsNone(output_members(cluster, name='abc', fmt='tsv'))
+                self.assertEqual(mock_echo.call_args[0][0], 'abc\tother\t\tReplica\trunning\t\tunknown')
 
+    @patch('patroni.dcs.AbstractDCS.set_failover_value', Mock())
+    def test_switchover(self):
         # Confirm
         result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\ny')
         self.assertEqual(result.exit_code, 0)
 
         # Abort
         result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\nN')
         self.assertEqual(result.exit_code, 1)
@@ -143,15 +146,15 @@
 
         # Scheduled with --force option
         result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0',
                                     '--force', '--scheduled', '2015-01-01T12:00:00+01:00'])
         self.assertEqual(result.exit_code, 0)
 
         # Scheduled in pause mode
-        with patch('patroni.config.GlobalConfig.is_paused', PropertyMock(return_value=True)):
+        with patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=True)):
             result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0',
                                               '--force', '--scheduled', '2015-01-01T12:00:00'])
             self.assertEqual(result.exit_code, 1)
             self.assertIn("Can't schedule switchover in the paused state", result.output)
 
         # Target and source are equal
         result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nleader\n\ny')
@@ -177,94 +180,89 @@
 
         # Specifying wrong leader
         result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='dummy')
         self.assertEqual(result.exit_code, 1)
         self.assertIn('Member dummy is not the leader of cluster dummy', result.output)
 
         # Errors while sending Patroni REST API request
-        with patch.object(PoolManager, 'request', Mock(side_effect=Exception)):
+        with patch('patroni.ctl.request_patroni', Mock(side_effect=Exception)):
             result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'],
                                         input='leader\nother\n2300-01-01T12:23:00\ny')
             self.assertIn('falling back to DCS', result.output)
 
-        with patch.object(PoolManager, 'request') as mock_api_request:
+        with patch('patroni.ctl.request_patroni') as mock_api_request:
             mock_api_request.return_value.status = 500
             result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\ny')
             self.assertIn('Switchover failed', result.output)
 
             mock_api_request.return_value.status = 501
             mock_api_request.return_value.data = b'Server does not support this operation'
             result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\ny')
             self.assertIn('Switchover failed', result.output)
 
         # No members available
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_only_leader
-        result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\ny')
-        self.assertEqual(result.exit_code, 1)
-        self.assertIn('No candidates found to switchover to', result.output)
+        with patch('patroni.dcs.AbstractDCS.get_cluster',
+                   Mock(return_value=get_cluster_initialized_with_only_leader())):
+            result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\ny')
+            self.assertEqual(result.exit_code, 1)
+            self.assertIn('No candidates found to switchover to', result.output)
 
         # No leader available
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_without_leader
-        result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\ny')
-        self.assertEqual(result.exit_code, 1)
-        self.assertIn('This cluster has no leader', result.output)
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=get_cluster_initialized_without_leader())):
+            result = self.runner.invoke(ctl, ['switchover', 'dummy', '--group', '0'], input='leader\nother\n\ny')
+            self.assertEqual(result.exit_code, 1)
+            self.assertIn('This cluster has no leader', result.output)
 
         # Citus cluster, no group number specified
         result = self.runner.invoke(ctl, ['switchover', 'dummy', '--force'], input='\n')
         self.assertEqual(result.exit_code, 1)
         self.assertIn('For Citus clusters the --group must me specified', result.output)
 
-    @patch('patroni.ctl.get_dcs')
-    @patch.object(PoolManager, 'request', Mock(return_value=MockResponse()))
-    @patch('patroni.ctl.request_patroni', Mock(return_value=MockResponse()))
-    def test_failover(self, mock_get_dcs):
-        mock_get_dcs.return_value.set_failover_value = Mock()
-
+    @patch('patroni.dcs.AbstractDCS.set_failover_value', Mock())
+    def test_failover(self):
         # No candidate specified
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
         result = self.runner.invoke(ctl, ['failover', 'dummy'], input='0\n')
         self.assertIn('Failover could be performed only to a specific candidate', result.output)
 
         # Candidate is the same as the leader
         result = self.runner.invoke(ctl, ['failover', 'dummy', '--group', '0'], input='leader\n')
         self.assertIn("Candidate ['other']", result.output)
         self.assertIn('Member leader is already the leader of cluster dummy', result.output)
 
         # Temp test to check a fallback to switchover if leader is specified
         with patch('patroni.ctl._do_failover_or_switchover') as failover_func_mock:
             result = self.runner.invoke(ctl, ['failover', '--leader', 'leader', 'dummy'], input='0\n')
             self.assertIn('Supplying a leader name using this command is deprecated', result.output)
-            failover_func_mock.assert_called_once_with(
-                DEFAULT_CONFIG, 'switchover', 'dummy', None, 'leader', None, False)
+            failover_func_mock.assert_called_once_with('switchover', 'dummy', None, 'leader', None, False)
 
         cluster = get_cluster_initialized_with_leader(sync=('leader', 'other'))
         cluster.members.append(Member(0, 'async', 28, {'api_url': 'http://127.0.0.1:8012/patroni'}))
         cluster.config.data['synchronous_mode'] = True
-        mock_get_dcs.return_value.get_cluster = Mock(return_value=cluster)
-        # Failover to an async member in sync mode (confirm)
-        result = self.runner.invoke(ctl,
-                                    ['failover', 'dummy', '--group', '0', '--candidate', 'async'], input='y\ny')
-        self.assertIn('Are you sure you want to failover to the asynchronous node async', result.output)
-        self.assertEqual(result.exit_code, 0)
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=cluster)):
+            # Failover to an async member in sync mode (confirm)
+            result = self.runner.invoke(ctl,
+                                        ['failover', 'dummy', '--group', '0', '--candidate', 'async'], input='y\ny')
+            self.assertIn('Are you sure you want to failover to the asynchronous node async', result.output)
+            self.assertEqual(result.exit_code, 0)
 
-        # Failover to an async member in sync mode (abort)
-        result = self.runner.invoke(ctl, ['failover', 'dummy', '--group', '0', '--candidate', 'async'], input='N')
-        self.assertEqual(result.exit_code, 1)
-        self.assertIn('Aborting failover', result.output)
+            # Failover to an async member in sync mode (abort)
+            result = self.runner.invoke(ctl, ['failover', 'dummy', '--group', '0', '--candidate', 'async'], input='N')
+            self.assertEqual(result.exit_code, 1)
+            self.assertIn('Aborting failover', result.output)
 
-    @patch('patroni.dcs.dcs_modules', Mock(return_value=['patroni.dcs.dummy', 'patroni.dcs.etcd']))
+    @patch('patroni.dynamic_loader.iter_modules', Mock(return_value=['patroni.dcs.dummy', 'patroni.dcs.etcd']))
     def test_get_dcs(self):
-        self.assertRaises(PatroniCtlException, get_dcs, {'dummy': {}}, 'dummy', 0)
+        with click.Context(click.Command('list')) as ctx:
+            ctx.obj = {'__config': {'dummy': {}}, '__mpp': get_mpp({})}
+            self.assertRaises(PatroniCtlException, get_dcs, 'dummy', 0)
 
     @patch('patroni.psycopg.connect', psycopg_connect)
     @patch('patroni.ctl.query_member', Mock(return_value=([['mock column']], None)))
-    @patch('patroni.ctl.get_dcs')
     @patch.object(etcd.Client, 'read', etcd_read)
-    def test_query(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
+    def test_query(self):
         # Mutually exclusive
         for role in self.TEST_ROLES:
             result = self.runner.invoke(ctl, ['query', 'alpha', '--member', 'abc', '--role', role])
             assert result.exit_code == 1
 
         with self.runner.isolated_filesystem():
             with open('dummy', 'w') as dummy_file:
@@ -289,71 +287,64 @@
         result = self.runner.invoke(ctl, ['query', 'alpha', '--command', 'SELECT 1', '--username', 'root',
                                           '--password', '--dbname', 'postgres'], input='ab\nab')
         assert 'mock column' in result.output
 
     def test_query_member(self):
         with patch('patroni.ctl.get_cursor', Mock(return_value=MockConnect().cursor())):
             for role in self.TEST_ROLES:
-                rows = query_member({}, None, None, None, None, role, 'SELECT pg_catalog.pg_is_in_recovery()', {})
+                rows = query_member(None, None, None, None, role, 'SELECT pg_catalog.pg_is_in_recovery()', {})
                 self.assertTrue('False' in str(rows))
 
             with patch.object(MockCursor, 'execute', Mock(side_effect=OperationalError('bla'))):
-                rows = query_member({}, None, None, None, None, 'replica', 'SELECT pg_catalog.pg_is_in_recovery()', {})
+                rows = query_member(None, None, None, None, 'replica', 'SELECT pg_catalog.pg_is_in_recovery()', {})
 
         with patch('patroni.ctl.get_cursor', Mock(return_value=None)):
             # No role nor member given -- generic message
-            rows = query_member({}, None, None, None, None, None, 'SELECT pg_catalog.pg_is_in_recovery()', {})
+            rows = query_member(None, None, None, None, None, 'SELECT pg_catalog.pg_is_in_recovery()', {})
             self.assertTrue('No connection is available' in str(rows))
 
             # Member given -- message pointing to member
-            rows = query_member({}, None, None, None, 'foo', None, 'SELECT pg_catalog.pg_is_in_recovery()', {})
+            rows = query_member(None, None, None, 'foo', None, 'SELECT pg_catalog.pg_is_in_recovery()', {})
             self.assertTrue('No connection to member foo' in str(rows))
 
             # Role given -- message pointing to role
-            rows = query_member({}, None, None, None, None, 'replica', 'SELECT pg_catalog.pg_is_in_recovery()', {})
+            rows = query_member(None, None, None, None, 'replica', 'SELECT pg_catalog.pg_is_in_recovery()', {})
             self.assertTrue('No connection to role replica' in str(rows))
 
         with patch('patroni.ctl.get_cursor', Mock(side_effect=OperationalError('bla'))):
-            rows = query_member({}, None, None, None, None, 'replica', 'SELECT pg_catalog.pg_is_in_recovery()', {})
+            rows = query_member(None, None, None, None, 'replica', 'SELECT pg_catalog.pg_is_in_recovery()', {})
 
-    @patch('patroni.ctl.get_dcs')
-    def test_dsn(self, mock_get_dcs):
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
+    def test_dsn(self):
         result = self.runner.invoke(ctl, ['dsn', 'alpha'])
         assert 'host=127.0.0.1 port=5435' in result.output
 
         # Mutually exclusive options
         for role in self.TEST_ROLES:
             result = self.runner.invoke(ctl, ['dsn', 'alpha', '--role', role, '--member', 'dummy'])
             assert result.exit_code == 1
 
         # Non-existing member
         result = self.runner.invoke(ctl, ['dsn', 'alpha', '--member', 'dummy'])
         assert result.exit_code == 1
 
-    @patch.object(PoolManager, 'request')
-    @patch('patroni.ctl.get_dcs')
-    def test_reload(self, mock_get_dcs, mock_post):
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
-
+    @patch('patroni.ctl.request_patroni')
+    def test_reload(self, mock_post):
         result = self.runner.invoke(ctl, ['reload', 'alpha'], input='y')
         assert 'Failed: reload for member' in result.output
 
         mock_post.return_value.status = 200
         result = self.runner.invoke(ctl, ['reload', 'alpha'], input='y')
         assert 'No changes to apply on member' in result.output
 
         mock_post.return_value.status = 202
         result = self.runner.invoke(ctl, ['reload', 'alpha'], input='y')
         assert 'Reload request received for member' in result.output
 
-    @patch.object(PoolManager, 'request')
-    @patch('patroni.ctl.get_dcs')
-    def test_restart_reinit(self, mock_get_dcs, mock_post):
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
+    @patch('patroni.ctl.request_patroni')
+    def test_restart_reinit(self, mock_post):
         mock_post.return_value.status = 503
         result = self.runner.invoke(ctl, ['restart', 'alpha'], input='now\ny\n')
         assert 'Failed: restart for' in result.output
         assert result.exit_code == 0
 
         result = self.runner.invoke(ctl, ['reinit', 'alpha'], input='y')
         assert result.exit_code == 1
@@ -385,15 +376,15 @@
         result = self.runner.invoke(ctl, ['restart', 'alpha', '--pending', '--force', '--timeout', '10min'])
         assert result.exit_code == 0
 
         # normal restart, the schedule is actually parsed, but not validated in patronictl
         result = self.runner.invoke(ctl, ['restart', 'alpha', 'other', '--force', '--scheduled', '2300-10-01T14:30'])
         assert 'Failed: flush scheduled restart' in result.output
 
-        with patch('patroni.config.GlobalConfig.is_paused', PropertyMock(return_value=True)):
+        with patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=True)):
             result = self.runner.invoke(ctl,
                                         ['restart', 'alpha', 'other', '--force', '--scheduled', '2300-10-01T14:30'])
             assert result.exit_code == 1
 
         # force restart with restart already present
         result = self.runner.invoke(ctl, ['restart', 'alpha', 'other', '--force', '--scheduled', '2300-10-01T14:30'])
         assert result.exit_code == 0
@@ -420,20 +411,18 @@
         # get restart with the non-200 return code
         # normal restart, the schedule is actually parsed, but not validated in patronictl
         mock_post.return_value.status = 409
         result = self.runner.invoke(ctl, ctl_args, input='y')
         assert 'Failed: another restart is already' in result.output
         assert result.exit_code == 0
 
-    @patch('patroni.ctl.get_dcs')
-    def test_remove(self, mock_get_dcs):
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
+    def test_remove(self):
         result = self.runner.invoke(ctl, ['remove', 'dummy'], input='\n')
         assert 'For Citus clusters the --group must me specified' in result.output
-        result = self.runner.invoke(ctl, ['-k', 'remove', 'alpha', '--group', '0'], input='alpha\nstandby')
+        result = self.runner.invoke(ctl, ['remove', 'alpha', '--group', '0'], input='alpha\nstandby')
         assert 'Please confirm' in result.output
         assert 'You are about to remove all' in result.output
         # Not typing an exact confirmation
         assert result.exit_code == 1
 
         # leader specified does not match leader of cluster
         result = self.runner.invoke(ctl, ['remove', 'alpha', '--group', '0'], input='alpha\nYes I am aware\nstandby')
@@ -443,174 +432,161 @@
         result = self.runner.invoke(ctl, ['remove', 'alpha', '--group', '0'], input='beta\nleader')
         assert result.exit_code == 1
 
         result = self.runner.invoke(ctl, ['remove', 'alpha', '--group', '0'], input='alpha\nYes I am aware\nleader')
         assert result.exit_code == 0
 
     def test_ctl(self):
-        self.runner.invoke(ctl, ['list'])
-
         result = self.runner.invoke(ctl, ['--help'])
         assert 'Usage:' in result.output
 
     def test_get_any_member(self):
-        for role in self.TEST_ROLES:
-            self.assertIsNone(get_any_member({}, get_cluster_initialized_without_leader(), None, role=role))
+        with click.Context(click.Command('list')) as ctx:
+            ctx.obj = {'__config': {}, '__mpp': get_mpp({})}
+            for role in self.TEST_ROLES:
+                self.assertIsNone(get_any_member(get_cluster_initialized_without_leader(), None, role=role))
 
-            m = get_any_member({}, get_cluster_initialized_with_leader(), None, role=role)
-            self.assertEqual(m.name, 'leader')
+                m = get_any_member(get_cluster_initialized_with_leader(), None, role=role)
+                self.assertEqual(m.name, 'leader')
 
     def test_get_all_members(self):
-        for role in self.TEST_ROLES:
-            self.assertEqual(list(get_all_members({}, get_cluster_initialized_without_leader(), None, role=role)), [])
+        with click.Context(click.Command('list')) as ctx:
+            ctx.obj = {'__config': {}, '__mpp': get_mpp({})}
+            for role in self.TEST_ROLES:
+                self.assertEqual(list(get_all_members(get_cluster_initialized_without_leader(), None, role=role)), [])
+
+                r = list(get_all_members(get_cluster_initialized_with_leader(), None, role=role))
+                self.assertEqual(len(r), 1)
+                self.assertEqual(r[0].name, 'leader')
 
-            r = list(get_all_members({}, get_cluster_initialized_with_leader(), None, role=role))
+            r = list(get_all_members(get_cluster_initialized_with_leader(), None, role='replica'))
             self.assertEqual(len(r), 1)
-            self.assertEqual(r[0].name, 'leader')
+            self.assertEqual(r[0].name, 'other')
 
-        r = list(get_all_members({}, get_cluster_initialized_with_leader(), None, role='replica'))
-        self.assertEqual(len(r), 1)
-        self.assertEqual(r[0].name, 'other')
-
-        self.assertEqual(len(list(get_all_members({}, get_cluster_initialized_without_leader(),
-                                                  None, role='replica'))), 2)
-
-    @patch('patroni.ctl.get_dcs')
-    def test_members(self, mock_get_dcs):
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
+            self.assertEqual(len(list(get_all_members(get_cluster_initialized_without_leader(),
+                                                      None, role='replica'))), 2)
 
+    def test_members(self):
         result = self.runner.invoke(ctl, ['list'])
         assert '127.0.0.1' in result.output
         assert result.exit_code == 0
         assert 'Citus cluster: alpha -' in result.output
 
         result = self.runner.invoke(ctl, ['list', '--group', '0'])
         assert 'Citus cluster: alpha (group: 0, 12345678901) -' in result.output
 
-        with patch('patroni.ctl.load_config', Mock(return_value={'scope': 'alpha'})):
+        config = get_default_config()
+        del config['citus']
+        with patch('patroni.ctl.load_config', Mock(return_value=config)):
             result = self.runner.invoke(ctl, ['list'])
             assert 'Cluster: alpha (12345678901) -' in result.output
 
         with patch('patroni.ctl.load_config', Mock(return_value={})):
             self.runner.invoke(ctl, ['list'])
 
-    @patch('patroni.ctl.get_dcs')
-    def test_list_extended(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
-        cluster = get_cluster_initialized_with_leader(sync=('leader', 'other'))
-        mock_get_dcs.return_value.get_cluster = Mock(return_value=cluster)
+        cluster = get_cluster_initialized_with_leader()
+        cluster.members[1].data['pending_restart'] = True
+        cluster.members[1].data['pending_restart_reason'] = {'param': get_param_diff('', 'very l' + 'o' * 34 + 'ng')}
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=cluster)):
+            for cmd in ('list', 'topology'):
+                result = self.runner.invoke(ctl, [cmd, 'dummy'])
+                self.assertIn('param: [hidden - too long]', result.output)
+
+            result = self.runner.invoke(ctl, ['list', 'dummy', '-f', 'tsv'])
+            self.assertIn('param: ->very l' + 'o' * 34 + 'ng', result.output)
+
+            cluster.members[1].data['pending_restart_reason'] = {'param': get_param_diff('', 'new')}
+            result = self.runner.invoke(ctl, ['list', 'dummy'])
+            self.assertIn('param: ->new', result.output)
 
+    def test_list_extended(self):
         result = self.runner.invoke(ctl, ['list', 'dummy', '--extended', '--timestamp'])
         assert '2100' in result.output
         assert 'Scheduled restart' in result.output
 
-    @patch('patroni.ctl.get_dcs')
-    def test_topology(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
+    def test_topology(self):
         cluster = get_cluster_initialized_with_leader()
-        cascade_member = Member(0, 'cascade', 28, {'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5437/postgres',
-                                                   'api_url': 'http://127.0.0.1:8012/patroni',
-                                                   'state': 'running',
-                                                   'tags': {'replicatefrom': 'other'},
-                                                   })
-        cascade_member_wrong_tags = Member(0, 'wrong_cascade', 28,
-                                           {'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5438/postgres',
-                                            'api_url': 'http://127.0.0.1:8013/patroni',
-                                            'state': 'running',
-                                            'tags': {'replicatefrom': 'nonexistinghost'},
-                                            })
-        cluster.members.append(cascade_member)
-        cluster.members.append(cascade_member_wrong_tags)
-        mock_get_dcs.return_value.get_cluster = Mock(return_value=cluster)
-        result = self.runner.invoke(ctl, ['topology', 'dummy'])
-        assert '+\n|     0 | leader          | 127.0.0.1:5435 | Leader  |' in result.output
-        assert '|\n|     0 | + other         | 127.0.0.1:5436 | Replica |' in result.output
-        assert '|\n|     0 |   + cascade     | 127.0.0.1:5437 | Replica |' in result.output
-        assert '|\n|     0 | + wrong_cascade | 127.0.0.1:5438 | Replica |' in result.output
-
-        cluster = get_cluster_initialized_without_leader()
-        mock_get_dcs.return_value.get_cluster = Mock(return_value=cluster)
-        result = self.runner.invoke(ctl, ['topology', 'dummy'])
-        assert '+\n|     0 | + leader | 127.0.0.1:5435 | Replica |' in result.output
-        assert '|\n|     0 | + other  | 127.0.0.1:5436 | Replica |' in result.output
-
-    @patch('patroni.ctl.get_dcs')
-    @patch.object(PoolManager, 'request', Mock(return_value=MockResponse()))
-    def test_flush_restart(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
+        cluster.members.append(Member(0, 'cascade', 28,
+                                      {'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5437/postgres',
+                                       'api_url': 'http://127.0.0.1:8012/patroni', 'state': 'running',
+                                       'tags': {'replicatefrom': 'other'}}))
+        cluster.members.append(Member(0, 'wrong_cascade', 28,
+                                      {'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5438/postgres',
+                                       'api_url': 'http://127.0.0.1:8013/patroni', 'state': 'running',
+                                       'tags': {'replicatefrom': 'nonexistinghost'}}))
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=cluster)):
+            result = self.runner.invoke(ctl, ['topology', 'dummy'])
+            assert '+\n|     0 | leader          | 127.0.0.1:5435 | Leader  |' in result.output
+            assert '|\n|     0 | + other         | 127.0.0.1:5436 | Replica |' in result.output
+            assert '|\n|     0 |   + cascade     | 127.0.0.1:5437 | Replica |' in result.output
+            assert '|\n|     0 | + wrong_cascade | 127.0.0.1:5438 | Replica |' in result.output
+
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=get_cluster_initialized_without_leader())):
+            result = self.runner.invoke(ctl, ['topology', 'dummy'])
+            assert '+\n|     0 | + leader | 127.0.0.1:5435 | Replica |' in result.output
+            assert '|\n|     0 | + other  | 127.0.0.1:5436 | Replica |' in result.output
 
+    @patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=get_cluster_initialized_with_leader()))
+    def test_flush_restart(self):
         for role in self.TEST_ROLES:
-            result = self.runner.invoke(ctl, ['-k', 'flush', 'dummy', 'restart', '-r', role], input='y')
+            result = self.runner.invoke(ctl, ['flush', 'dummy', 'restart', '-r', role], input='y')
             assert 'No scheduled restart' in result.output
 
         result = self.runner.invoke(ctl, ['flush', 'dummy', 'restart', '--force'])
         assert 'Success: flush scheduled restart' in result.output
-        with patch.object(PoolManager, 'request', return_value=MockResponse(404)):
+        with patch('patroni.ctl.request_patroni', Mock(return_value=MockResponse(404))):
             result = self.runner.invoke(ctl, ['flush', 'dummy', 'restart', '--force'])
             assert 'Failed: flush scheduled restart' in result.output
 
-    @patch('patroni.ctl.get_dcs')
-    @patch.object(PoolManager, 'request', Mock(return_value=MockResponse()))
-    def test_flush_switchover(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
-
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
-        result = self.runner.invoke(ctl, ['flush', 'dummy', 'switchover'])
-        assert 'No pending scheduled switchover' in result.output
+    def test_flush_switchover(self):
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=get_cluster_initialized_with_leader())):
+            result = self.runner.invoke(ctl, ['flush', 'dummy', 'switchover'])
+            assert 'No pending scheduled switchover' in result.output
 
         scheduled_at = datetime.now(tzutc) + timedelta(seconds=600)
-        mock_get_dcs.return_value.get_cluster = Mock(
-            return_value=get_cluster_initialized_with_leader(Failover(1, 'a', 'b', scheduled_at)))
-        result = self.runner.invoke(ctl, ['flush', 'dummy', 'switchover'])
-        assert result.output.startswith('Success: ')
+        with patch('patroni.dcs.AbstractDCS.get_cluster',
+                   Mock(return_value=get_cluster_initialized_with_leader(Failover(1, 'a', 'b', scheduled_at)))):
+            result = self.runner.invoke(ctl, ['-k', 'flush', 'dummy', 'switchover'])
+            assert result.output.startswith('Success: ')
+
+            with patch('patroni.ctl.request_patroni', side_effect=[MockResponse(409), Exception]), \
+                    patch('patroni.dcs.AbstractDCS.manual_failover', Mock()):
+                result = self.runner.invoke(ctl, ['flush', 'dummy', 'switchover'])
+                assert 'Could not find any accessible member of cluster' in result.output
 
-        mock_get_dcs.return_value.manual_failover = Mock()
-        with patch.object(PoolManager, 'request', side_effect=[MockResponse(409), Exception]):
-            result = self.runner.invoke(ctl, ['flush', 'dummy', 'switchover'])
-            assert 'Could not find any accessible member of cluster' in result.output
-
-    @patch.object(PoolManager, 'request')
-    @patch('patroni.ctl.get_dcs')
     @patch('patroni.ctl.polling_loop', Mock(return_value=[1]))
-    def test_pause_cluster(self, mock_get_dcs, mock_post):
-        mock_get_dcs.return_value = self.e
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
-
-        mock_post.return_value.status = 500
-        result = self.runner.invoke(ctl, ['pause', 'dummy'])
-        assert 'Failed' in result.output
+    def test_pause_cluster(self):
+        with patch('patroni.ctl.request_patroni', Mock(return_value=MockResponse(500))):
+            result = self.runner.invoke(ctl, ['pause', 'dummy'])
+            assert 'Failed' in result.output
 
-        mock_post.return_value.status = 200
-        with patch('patroni.config.GlobalConfig.is_paused', PropertyMock(return_value=True)):
+        with patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=True)):
             result = self.runner.invoke(ctl, ['pause', 'dummy'])
             assert 'Cluster is already paused' in result.output
 
         result = self.runner.invoke(ctl, ['pause', 'dummy', '--wait'])
         assert "'pause' request sent" in result.output
-        mock_get_dcs.return_value.get_cluster = Mock(side_effect=[get_cluster_initialized_with_leader(),
-                                                                  get_cluster(None, None, [], None, None)])
-        self.runner.invoke(ctl, ['pause', 'dummy', '--wait'])
-        member = Member(1, 'other', 28, {})
-        mock_get_dcs.return_value.get_cluster = Mock(side_effect=[get_cluster_initialized_with_leader(),
-                                                                  get_cluster(None, None, [member], None, None)])
-        self.runner.invoke(ctl, ['pause', 'dummy', '--wait'])
-
-    @patch.object(PoolManager, 'request')
-    @patch('patroni.ctl.get_dcs')
-    def test_resume_cluster(self, mock_get_dcs, mock_post):
-        mock_get_dcs.return_value = self.e
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
 
+        with patch('patroni.dcs.AbstractDCS.get_cluster',
+                   Mock(side_effect=[get_cluster_initialized_with_leader(), get_cluster(None, None, [], None, None)])):
+            self.runner.invoke(ctl, ['pause', 'dummy', '--wait'])
+        with patch('patroni.dcs.AbstractDCS.get_cluster',
+                   Mock(side_effect=[get_cluster_initialized_with_leader(),
+                                     get_cluster(None, None, [Member(1, 'other', 28, {})], None, None)])):
+            self.runner.invoke(ctl, ['pause', 'dummy', '--wait'])
+
+    @patch('patroni.ctl.request_patroni')
+    @patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=get_cluster_initialized_with_leader()))
+    def test_resume_cluster(self, mock_post):
         mock_post.return_value.status = 200
-        with patch('patroni.config.GlobalConfig.is_paused', PropertyMock(return_value=False)):
+        with patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=False)):
             result = self.runner.invoke(ctl, ['resume', 'dummy'])
             assert 'Cluster is not paused' in result.output
 
-        with patch('patroni.config.GlobalConfig.is_paused', PropertyMock(return_value=True)):
+        with patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=True)):
             result = self.runner.invoke(ctl, ['resume', 'dummy'])
             assert 'Success' in result.output
 
             mock_post.return_value.status = 500
             result = self.runner.invoke(ctl, ['resume', 'dummy'])
             assert 'Failed' in result.output
 
@@ -704,75 +680,61 @@
     @patch('subprocess.call', return_value=1)
     def test_invoke_editor(self, mock_subprocess_call):
         os.environ.pop('EDITOR', None)
         for e in ('', '/bin/vi'):
             with patch('shutil.which', Mock(return_value=e)):
                 self.assertRaises(PatroniCtlException, invoke_editor, 'foo: bar\n', 'test')
 
-    @patch('patroni.ctl.get_dcs')
-    def test_show_config(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
+    def test_show_config(self):
         self.runner.invoke(ctl, ['show-config', 'dummy'])
 
-    @patch('patroni.ctl.get_dcs')
     @patch('subprocess.call', Mock(return_value=0))
-    def test_edit_config(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
-        mock_get_dcs.return_value.set_config_value = Mock(return_value=False)
+    def test_edit_config(self):
         os.environ['EDITOR'] = 'true'
         self.runner.invoke(ctl, ['edit-config', 'dummy'])
         self.runner.invoke(ctl, ['edit-config', 'dummy', '-s', 'foo=bar'])
         self.runner.invoke(ctl, ['edit-config', 'dummy', '--replace', 'postgres0.yml'])
         self.runner.invoke(ctl, ['edit-config', 'dummy', '--apply', '-'], input='foo: bar')
         self.runner.invoke(ctl, ['edit-config', 'dummy', '--force', '--apply', '-'], input='foo: bar')
-        mock_get_dcs.return_value.set_config_value.return_value = True
-        self.runner.invoke(ctl, ['edit-config', 'dummy', '--force', '--apply', '-'], input='foo: bar')
-        mock_get_dcs.return_value.get_cluster = Mock(return_value=Cluster.empty())
-        result = self.runner.invoke(ctl, ['edit-config', 'dummy'])
-        assert result.exit_code == 1
-        assert 'The config key does not exist in the cluster dummy' in result.output
+        with patch('patroni.dcs.etcd.Etcd.set_config_value', Mock(return_value=True)):
+            self.runner.invoke(ctl, ['edit-config', 'dummy', '--force', '--apply', '-'], input='foo: bar')
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=Cluster.empty())):
+            result = self.runner.invoke(ctl, ['edit-config', 'dummy'])
+            assert result.exit_code == 1
+            assert 'The config key does not exist in the cluster dummy' in result.output
 
-    @patch('patroni.ctl.get_dcs')
-    def test_version(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
-        with patch.object(PoolManager, 'request') as mocked:
-            result = self.runner.invoke(ctl, ['version'])
-            assert 'patronictl version' in result.output
-            mocked.return_value.data = b'{"patroni":{"version":"1.2.3"},"server_version": 100001}'
-            result = self.runner.invoke(ctl, ['version', 'dummy'])
-            assert '1.2.3' in result.output
-        with patch.object(PoolManager, 'request', Mock(side_effect=Exception)):
-            result = self.runner.invoke(ctl, ['version', 'dummy'])
-            assert 'failed to get version' in result.output
-
-    @patch('patroni.ctl.get_dcs')
-    def test_history(self, mock_get_dcs):
-        mock_get_dcs.return_value.get_cluster = Mock()
-        mock_get_dcs.return_value.get_cluster.return_value.history.lines = [[1, 67176, 'no recovery target specified']]
-        result = self.runner.invoke(ctl, ['history'])
-        assert 'Reason' in result.output
+    @patch('patroni.ctl.request_patroni')
+    def test_version(self, mock_request):
+        result = self.runner.invoke(ctl, ['version'])
+        assert 'patronictl version' in result.output
+        mock_request.return_value.data = b'{"patroni":{"version":"1.2.3"},"server_version": 100001}'
+        result = self.runner.invoke(ctl, ['version', 'dummy'])
+        assert '1.2.3' in result.output
+        mock_request.side_effect = Exception
+        result = self.runner.invoke(ctl, ['version', 'dummy'])
+        assert 'failed to get version' in result.output
+
+    def test_history(self):
+        with patch('patroni.dcs.AbstractDCS.get_cluster') as mock_get_cluster:
+            mock_get_cluster.return_value.history.lines = [[1, 67176, 'no recovery target specified']]
+            result = self.runner.invoke(ctl, ['history'])
+            assert 'Reason' in result.output
 
     def test_format_pg_version(self):
         self.assertEqual(format_pg_version(100001), '10.1')
         self.assertEqual(format_pg_version(90605), '9.6.5')
 
-    @patch('patroni.ctl.get_dcs')
-    def test_get_members(self, mock_get_dcs):
-        mock_get_dcs.return_value = self.e
-        mock_get_dcs.return_value.get_cluster = get_cluster_not_initialized_without_leader
-        result = self.runner.invoke(ctl, ['reinit', 'dummy'])
-        assert "cluster doesn\'t have any members" in result.output
+    def test_get_members(self):
+        with patch('patroni.dcs.AbstractDCS.get_cluster',
+                   Mock(return_value=get_cluster_not_initialized_without_leader())):
+            result = self.runner.invoke(ctl, ['reinit', 'dummy'])
+            assert "cluster doesn\'t have any members" in result.output
 
     @patch('time.sleep', Mock())
-    @patch('patroni.ctl.get_dcs')
-    def test_reinit_wait(self, mock_get_dcs):
-        mock_get_dcs.return_value.get_cluster = get_cluster_initialized_with_leader
+    def test_reinit_wait(self):
         with patch.object(PoolManager, 'request') as mocked:
             mocked.side_effect = [Mock(data=s, status=200) for s in
                                   [b"reinitialize", b'{"state":"creating replica"}', b'{"state":"running"}']]
             result = self.runner.invoke(ctl, ['reinit', 'alpha', 'other', '--wait'], input='y\ny')
         self.assertIn("Waiting for reinitialize to complete on: other", result.output)
         self.assertIn("Reinitialize is completed on: other", result.output)
```

### Comparing `patroni-3.2.2/tests/test_etcd.py` & `patroni-3.3.0/tests/test_etcd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import etcd
 import urllib3.util.connection
 import socket
 import unittest
 
 from dns.exception import DNSException
 from mock import Mock, PropertyMock, patch
+from patroni.dcs import get_dcs
 from patroni.dcs.etcd import AbstractDCS, EtcdClient, Cluster, Etcd, EtcdError, DnsCachingResolver
 from patroni.exceptions import DCSError
+from patroni.postgresql.mpp import get_mpp
 from patroni.utils import Retry
 from urllib3.exceptions import ReadTimeoutError
 
 from . import SleepException, MockResponse, requests_get
 
 
 def etcd_watch(self, key, index=None, timeout=None, recursive=None):
@@ -134,16 +136,17 @@
 
     @patch('dns.resolver.query', dns_query)
     @patch('socket.getaddrinfo', socket_getaddrinfo)
     @patch('patroni.dcs.etcd.requests_get', requests_get)
     @patch.object(EtcdClient, '_get_machines_list',
                   Mock(return_value=['http://localhost:2379', 'http://localhost:4001']))
     def setUp(self):
-        self.etcd = Etcd({'namespace': '/patroni/', 'ttl': 30, 'retry_timeout': 3,
-                          'srv': 'test', 'scope': 'test', 'name': 'foo'})
+        self.etcd = get_dcs({'namespace': '/patroni/', 'ttl': 30, 'retry_timeout': 3,
+                             'etcd': {'srv': 'test'}, 'scope': 'test', 'name': 'foo'})
+        self.assertIsInstance(self.etcd, Etcd)
         self.client = self.etcd._client
         self.client.http.request = http_request
         self.client.http.request_encode_body = http_request
 
     def test_machines(self):
         self.client._base_uri = 'http://localhost:4002'
         self.client._machines_cache = ['http://localhost:4002', 'http://localhost:2379']
@@ -231,15 +234,15 @@
 class TestEtcd(unittest.TestCase):
 
     @patch('socket.getaddrinfo', socket_getaddrinfo)
     @patch.object(EtcdClient, '_get_machines_list',
                   Mock(return_value=['http://localhost:2379', 'http://localhost:4001']))
     def setUp(self):
         self.etcd = Etcd({'namespace': '/patroni/', 'ttl': 30, 'retry_timeout': 10,
-                          'host': 'localhost:2379', 'scope': 'test', 'name': 'foo'})
+                          'host': 'localhost:2379', 'scope': 'test', 'name': 'foo'}, get_mpp({}))
 
     def test_base_path(self):
         self.assertEqual(self.etcd._base_path, '/patroni/test')
 
     @patch('dns.resolver.query', dns_query)
     @patch('time.sleep', Mock(side_effect=SleepException))
     @patch.object(EtcdClient, '_get_machines_list', Mock(side_effect=etcd.EtcdConnectionFailed))
@@ -266,15 +269,15 @@
         cluster = self.etcd.get_cluster()
         self.assertIsInstance(cluster, Cluster)
         self.assertIsNone(cluster.leader)
         self.etcd._base_path = '/service/noleader'
         self.assertRaises(EtcdError, self.etcd.get_cluster)
 
     def test__get_citus_cluster(self):
-        self.etcd._citus_group = '0'
+        self.etcd._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
         cluster = self.etcd.get_cluster()
         self.assertIsInstance(cluster, Cluster)
         self.assertIsInstance(cluster.workers[1], Cluster)
         self.etcd._base_path = '/service/nocluster'
         self.assertTrue(self.etcd.get_cluster().is_empty())
 
     def test_touch_member(self):
```

### Comparing `patroni-3.2.2/tests/test_etcd3.py` & `patroni-3.3.0/tests/test_etcd3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import etcd
 import json
 import unittest
 import urllib3
 
 from mock import Mock, PropertyMock, patch
+from patroni.dcs import get_dcs
 from patroni.dcs.etcd import DnsCachingResolver
 from patroni.dcs.etcd3 import PatroniEtcd3Client, Cluster, Etcd3, Etcd3Client, \
-    Etcd3Error, Etcd3ClientError, ReAuthenticateMode, RetryFailedError, InvalidAuthToken, Unavailable, \
+    Etcd3Error, Etcd3ClientError, RetryFailedError, InvalidAuthToken, Unavailable, \
     Unknown, UnsupportedEtcdVersion, UserEmpty, AuthFailed, AuthOldRevision, base64_encode
+from patroni.postgresql.mpp import get_mpp
 from threading import Thread
 
 from . import SleepException, MockResponse
 
 
 def mock_urlopen(self, method, url, **kwargs):
     ret = MockResponse()
@@ -76,17 +78,17 @@
 
 
 class BaseTestEtcd3(unittest.TestCase):
 
     @patch.object(Thread, 'start', Mock())
     @patch.object(urllib3.PoolManager, 'urlopen', mock_urlopen)
     def setUp(self):
-        self.etcd3 = Etcd3({'namespace': '/patroni/', 'ttl': 30, 'retry_timeout': 10,
-                            'host': 'localhost:2378', 'scope': 'test', 'name': 'foo',
-                            'username': 'etcduser', 'password': 'etcdpassword'})
+        self.etcd3 = get_dcs({'namespace': '/patroni/', 'ttl': 30, 'retry_timeout': 10, 'name': 'foo', 'scope': 'test',
+                              'etcd3': {'host': 'localhost:2378', 'username': 'etcduser', 'password': 'etcdpassword'}})
+        self.assertIsInstance(self.etcd3, Etcd3)
         self.client = self.etcd3._client
         self.kv_cache = self.client._kv_cache
 
 
 class TestKVCache(BaseTestEtcd3):
 
     @patch.object(urllib3.PoolManager, 'urlopen', mock_urlopen)
@@ -160,20 +162,22 @@
         self.assertRaises(UserEmpty, self.client.deleteprefix, 'foo')
         mock_urlopen.return_value.content = '{"code":16,"error":"etcdserver: invalid auth token"}'
         self.assertRaises(InvalidAuthToken, self.client.deleteprefix, 'foo')
         with patch.object(PatroniEtcd3Client, 'authenticate', Mock(return_value=True)):
             retry = self.etcd3._retry.copy()
             with patch('time.time', Mock(side_effect=[0, 10, 20, 30, 40])):
                 self.assertRaises(InvalidAuthToken, retry, self.client.deleteprefix, 'foo', retry=retry)
+            with patch('time.time', Mock(side_effect=[0, 10])):
+                self.assertRaises(InvalidAuthToken, self.client.deleteprefix, 'foo')
             self.client.username = None
-            self.client._reauthenticate_reason = ReAuthenticateMode.NOT_REQUIRED
+            self.client._reauthenticate = False
             retry = self.etcd3._retry.copy()
             self.assertRaises(InvalidAuthToken, retry, self.client.deleteprefix, 'foo', retry=retry)
             mock_urlopen.return_value.content = '{"code":3,"error":"etcdserver: revision of auth store is old"}'
-            self.client._reauthenticate_reason = ReAuthenticateMode.NOT_REQUIRED
+            self.client._reauthenticate = False
             self.assertRaises(AuthOldRevision, retry, self.client.deleteprefix, 'foo', retry=retry)
 
     def test__handle_server_response(self):
         response = MockResponse()
         response.content = '{"code":0,"error":"'
         self.assertRaises(etcd.EtcdException, self.client._handle_server_response, response)
         response.status_code = 400
@@ -232,15 +236,15 @@
             self.assertIsInstance(self.etcd3.get_cluster(), Cluster)
             mock_urlopen.side_effect = UnsupportedEtcdVersion('')
             self.assertRaises(UnsupportedEtcdVersion, self.etcd3.get_cluster)
             mock_urlopen.side_effect = SleepException()
             self.assertRaises(Etcd3Error, self.etcd3.get_cluster)
 
     def test__get_citus_cluster(self):
-        self.etcd3._citus_group = '0'
+        self.etcd3._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
         cluster = self.etcd3.get_cluster()
         self.assertIsInstance(cluster, Cluster)
         self.assertIsInstance(cluster.workers[1], Cluster)
 
     def test_touch_member(self):
         self.etcd3.touch_member({})
         self.etcd3._lease = 'bla'
@@ -265,16 +269,16 @@
             self.assertFalse(self.etcd3.update_leader(leader, '125'))
 
     def test_take_leader(self):
         self.assertFalse(self.etcd3.take_leader())
 
     def test_attempt_to_acquire_leader(self):
         self.assertFalse(self.etcd3.attempt_to_acquire_leader())
-        with patch('time.time', Mock(side_effect=[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 100, 200])):
-            self.assertRaises(Etcd3Error, self.etcd3.attempt_to_acquire_leader)
+        with patch('time.time', Mock(side_effect=[0, 0, 0, 0, 0, 100, 200, 300])):
+            self.assertFalse(self.etcd3.attempt_to_acquire_leader())
         with patch('time.time', Mock(side_effect=[0, 100, 200, 300, 400])):
             self.assertRaises(Etcd3Error, self.etcd3.attempt_to_acquire_leader)
         with patch.object(PatroniEtcd3Client, 'put', Mock(return_value=False)):
             self.assertFalse(self.etcd3.attempt_to_acquire_leader())
 
     def test_set_ttl(self):
         self.etcd3.set_ttl(20)
```

### Comparing `patroni-3.2.2/tests/test_exhibitor.py` & `patroni-3.3.0/tests/test_exhibitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 import urllib3
 
 from mock import Mock, patch
+from patroni.dcs import get_dcs
 from patroni.dcs.exhibitor import ExhibitorEnsembleProvider, Exhibitor
 from patroni.dcs.zookeeper import ZooKeeperError
 
 from . import SleepException, requests_get
 from .test_zookeeper import MockKazooClient
 
 
@@ -22,14 +23,15 @@
 
 class TestExhibitor(unittest.TestCase):
 
     @patch('urllib3.PoolManager.request', Mock(return_value=urllib3.HTTPResponse(
         status=200, body=b'{"servers":["127.0.0.1","127.0.0.2","127.0.0.3"],"port":2181}')))
     @patch('patroni.dcs.zookeeper.PatroniKazooClient', MockKazooClient)
     def setUp(self):
-        self.e = Exhibitor({'hosts': ['localhost', 'exhibitor'], 'port': 8181, 'scope': 'test',
-                            'name': 'foo', 'ttl': 30, 'retry_timeout': 10})
+        self.e = get_dcs({'exhibitor': {'hosts': ['localhost', 'exhibitor'], 'port': 8181},
+                          'scope': 'test', 'name': 'foo', 'ttl': 30, 'retry_timeout': 10})
+        self.assertIsInstance(self.e, Exhibitor)
 
     @patch.object(ExhibitorEnsembleProvider, 'poll', Mock(return_value=True))
     @patch.object(MockKazooClient, 'get_children', Mock(side_effect=Exception))
     def test_get_cluster(self):
         self.assertRaises(ZooKeeperError, self.e.get_cluster)
```

### Comparing `patroni-3.2.2/tests/test_file_perm.py` & `patroni-3.3.0/tests/test_file_perm.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_ha.py` & `patroni-3.3.0/tests/test_ha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import etcd
 import os
 import sys
 
 from mock import Mock, MagicMock, PropertyMock, patch, mock_open
+from patroni import global_config
 from patroni.collections import CaseInsensitiveSet
 from patroni.config import Config
 from patroni.dcs import Cluster, ClusterConfig, Failover, Leader, Member, get_dcs, Status, SyncState, TimelineHistory
 from patroni.dcs.etcd import AbstractEtcdClientWithFailover
 from patroni.exceptions import DCSError, PostgresConnectionException, PatroniFatalException
 from patroni.ha import Ha, _MemberStatus
 from patroni.postgresql import Postgresql
@@ -146,14 +147,15 @@
         self.api = Mock()
         self.tags = {'foo': 'bar'}
         self.nofailover = None
         self.replicatefrom = None
         self.api.connection_string = 'http://127.0.0.1:8008'
         self.clonefrom = None
         self.nosync = False
+        self.nostream = False
         self.scheduled_restart = {'schedule': future_restart_time,
                                   'postmaster_start_time': str(postmaster_start_time)}
         self.watchdog = Watchdog(self.config)
         self.request = lambda *args, **kwargs: requests_get(args[0].api_url, *args[1:], **kwargs)
         self.failover_priority = 1
 
 
@@ -192,15 +194,15 @@
 @patch.object(etcd.Client, 'write', etcd_write)
 @patch.object(etcd.Client, 'read', etcd_read)
 @patch.object(etcd.Client, 'delete', Mock(side_effect=etcd.EtcdException))
 @patch('patroni.postgresql.polling_loop', Mock(return_value=range(1)))
 @patch('patroni.async_executor.AsyncExecutor.busy', PropertyMock(return_value=False))
 @patch('patroni.async_executor.AsyncExecutor.run_async', run_async)
 @patch('patroni.postgresql.rewind.Thread', Mock())
-@patch('patroni.postgresql.citus.CitusHandler.start', Mock())
+@patch('patroni.postgresql.mpp.citus.CitusHandler.start', Mock())
 @patch('subprocess.call', Mock(return_value=0))
 @patch('time.sleep', Mock())
 class TestHa(PostgresInit):
 
     @patch('socket.getaddrinfo', socket_getaddrinfo)
     @patch('patroni.dcs.dcs_modules', Mock(return_value=['patroni.dcs.etcd']))
     @patch.object(etcd.Client, 'read', etcd_read)
@@ -213,14 +215,15 @@
         self.p.can_create_replica_without_replication_connection = MagicMock(return_value=False)
         self.e = get_dcs({'etcd': {'ttl': 30, 'host': 'ok:2379', 'scope': 'test',
                                    'name': 'foo', 'retry_timeout': 10},
                           'citus': {'database': 'citus', 'group': None}})
         self.ha = Ha(MockPatroni(self.p, self.e))
         self.ha.old_cluster = self.e.get_cluster()
         self.ha.cluster = get_cluster_initialized_without_leader()
+        global_config.update(self.ha.cluster)
         self.ha.load_cluster_from_dcs = Mock()
 
     def test_update_lock(self):
         self.ha.is_failsafe_mode = true
         self.p.last_operation = Mock(side_effect=PostgresConnectionException(''))
         self.ha.dcs.update_leader = Mock(side_effect=[DCSError(''), Exception])
         self.assertRaises(DCSError, self.ha.update_lock)
@@ -247,16 +250,16 @@
     def test_start_as_replica(self):
         self.p.is_healthy = false
         self.assertEqual(self.ha.run_cycle(), 'starting as a secondary')
 
     @patch('patroni.dcs.etcd.Etcd.initialize', return_value=True)
     def test_bootstrap_as_standby_leader(self, initialize):
         self.p.data_directory_empty = true
-        self.ha.cluster = get_cluster_not_initialized_without_leader(cluster_config=ClusterConfig(0, {}, 0))
-        self.ha.patroni.config._dynamic_configuration = {"standby_cluster": {"port": 5432}}
+        self.ha.cluster = get_cluster_not_initialized_without_leader(
+            cluster_config=ClusterConfig(1, {"standby_cluster": {"port": 5432}}, 1))
         self.assertEqual(self.ha.run_cycle(), 'trying to bootstrap a new standby leader')
 
     def test_bootstrap_waiting_for_standby_leader(self):
         self.p.data_directory_empty = true
         self.ha.cluster = get_cluster_initialized_without_leader()
         self.ha.cluster.config.data.update({'standby_cluster': {'port': 5432}})
         self.assertEqual(self.ha.run_cycle(), 'waiting for standby_leader to bootstrap')
@@ -314,15 +317,14 @@
         self.assertEqual(self.ha.run_cycle(), 'doing crash recovery in a single user mode')
         with patch('patroni.async_executor.AsyncExecutor.busy', PropertyMock(return_value=True)), \
                 patch.object(Ha, 'check_timeline', Mock(return_value=False)):
             self.ha._async_executor.schedule('doing crash recovery in a single user mode')
             self.ha.state_handler.cancellable._process = Mock()
             self.ha._crash_recovery_started -= 600
             self.ha.cluster.config.data.update({'maximum_lag_on_failover': 10})
-            self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
             self.assertEqual(self.ha.run_cycle(), 'terminated crash recovery because of startup timeout')
 
     @patch.object(Rewind, 'ensure_clean_shutdown', Mock())
     @patch.object(Rewind, 'rewind_or_reinitialize_needed_and_possible', Mock(return_value=True))
     @patch.object(Rewind, 'can_rewind', PropertyMock(return_value=True))
     def test_crash_recovery_before_rewind(self):
         self.p.is_primary = false
@@ -466,14 +468,19 @@
         self.ha.update_lock = false
         self.assertEqual(self.ha.run_cycle(), 'demoted self because failed to update leader lock in DCS')
         with patch.object(Ha, '_get_node_to_follow', Mock(side_effect=DCSError('foo'))):
             self.assertEqual(self.ha.run_cycle(), 'demoted self because failed to update leader lock in DCS')
         self.p.is_primary = false
         self.assertEqual(self.ha.run_cycle(), 'not promoting because failed to update leader lock in DCS')
 
+    def test_get_node_to_follow_nostream(self):
+        self.ha.patroni.nostream = True
+        self.ha.cluster = get_cluster_initialized_with_leader()
+        self.assertEqual(self.ha._get_node_to_follow(self.ha.cluster), None)
+
     @patch.object(Cluster, 'is_unlocked', Mock(return_value=False))
     def test_follow(self):
         self.p.is_primary = false
         self.assertEqual(self.ha.run_cycle(), 'no action. I am (postgresql0), a secondary, and following a leader ()')
         self.ha.patroni.replicatefrom = "foo"
         self.p.config.check_recovery_conf = Mock(return_value=(True, False))
         self.ha.cluster.config.data.update({'slots': {'l': {'database': 'a', 'plugin': 'b'}}})
@@ -505,15 +512,15 @@
         self.assertEqual(self.ha.run_cycle(), 'demoting self because DCS is not accessible and I was a leader')
         self.ha._async_executor.schedule('dummy')
         self.assertEqual(self.ha.run_cycle(), 'demoted self because DCS is not accessible and I was a leader')
 
     def test_check_failsafe_topology(self):
         self.ha.load_cluster_from_dcs = Mock(side_effect=DCSError('Etcd is not responding properly'))
         self.ha.cluster = get_cluster_initialized_with_leader_and_failsafe()
-        self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
+        global_config.update(self.ha.cluster)
         self.ha.dcs._last_failsafe = self.ha.cluster.failsafe
         self.assertEqual(self.ha.run_cycle(), 'demoting self because DCS is not accessible and I was a leader')
         self.ha.state_handler.name = self.ha.cluster.leader.name
         self.assertFalse(self.ha.failsafe_is_active())
         self.assertEqual(self.ha.run_cycle(),
                          'continue to run as a leader because failsafe mode is enabled and all members are accessible')
         self.assertTrue(self.ha.failsafe_is_active())
@@ -525,15 +532,15 @@
         self.ha.dcs._last_failsafe[self.ha.cluster.leader.name] = self.ha.cluster.leader.member.api_url
         self.assertEqual(self.ha.run_cycle(),
                          'continue to run as a leader because failsafe mode is enabled and all members are accessible')
 
     def test_no_dcs_connection_primary_failsafe(self):
         self.ha.load_cluster_from_dcs = Mock(side_effect=DCSError('Etcd is not responding properly'))
         self.ha.cluster = get_cluster_initialized_with_leader_and_failsafe()
-        self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
+        global_config.update(self.ha.cluster)
         self.ha.dcs._last_failsafe = self.ha.cluster.failsafe
         self.ha.state_handler.name = self.ha.cluster.leader.name
         self.assertEqual(self.ha.run_cycle(),
                          'continue to run as a leader because failsafe mode is enabled and all members are accessible')
 
     def test_readonly_dcs_primary_failsafe(self):
         self.ha.cluster = get_cluster_initialized_with_leader_and_failsafe()
@@ -542,15 +549,15 @@
         self.ha.state_handler.name = self.ha.cluster.leader.name
         self.assertEqual(self.ha.run_cycle(),
                          'continue to run as a leader because failsafe mode is enabled and all members are accessible')
 
     def test_no_dcs_connection_replica_failsafe(self):
         self.ha.load_cluster_from_dcs = Mock(side_effect=DCSError('Etcd is not responding properly'))
         self.ha.cluster = get_cluster_initialized_with_leader_and_failsafe()
-        self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
+        global_config.update(self.ha.cluster)
         self.ha.update_failsafe({'name': 'leader', 'api_url': 'http://127.0.0.1:8008/patroni',
                                  'conn_url': 'postgres://127.0.0.1:5432/postgres', 'slots': {'foo': 1000}})
         self.p.is_primary = false
         self.assertEqual(self.ha.run_cycle(), 'DCS is not accessible')
 
     def test_no_dcs_connection_replica_failsafe_not_enabled_but_active(self):
         self.ha.load_cluster_from_dcs = Mock(side_effect=DCSError('Etcd is not responding properly'))
@@ -585,16 +592,16 @@
         self.assertEqual(self.ha.bootstrap(), 'waiting for leader to bootstrap')
 
     def test_bootstrap_initialize_lock_failed(self):
         self.ha.cluster = get_cluster_not_initialized_without_leader()
         self.assertEqual(self.ha.bootstrap(), 'failed to acquire initialize lock')
 
     @patch('patroni.psycopg.connect', psycopg_connect)
-    @patch('patroni.postgresql.citus.connect', psycopg_connect)
-    @patch('patroni.postgresql.citus.quote_ident', Mock())
+    @patch('patroni.postgresql.mpp.citus.connect', psycopg_connect)
+    @patch('patroni.postgresql.mpp.citus.quote_ident', Mock())
     @patch.object(Postgresql, 'connection', Mock(return_value=None))
     def test_bootstrap_initialized_new_cluster(self):
         self.ha.cluster = get_cluster_not_initialized_without_leader()
         self.e.initialize = true
         self.assertEqual(self.ha.bootstrap(), 'trying to bootstrap a new cluster')
         self.p.is_primary = false
         self.assertEqual(self.ha.run_cycle(), 'waiting for end of recovery after bootstrap')
@@ -607,16 +614,16 @@
         self.ha.cluster = get_cluster_not_initialized_without_leader()
         self.e.initialize = true
         self.ha.bootstrap()
         self.p.is_running = false
         self.assertRaises(PatroniFatalException, self.ha.post_bootstrap)
 
     @patch('patroni.psycopg.connect', psycopg_connect)
-    @patch('patroni.postgresql.citus.connect', psycopg_connect)
-    @patch('patroni.postgresql.citus.quote_ident', Mock())
+    @patch('patroni.postgresql.mpp.citus.connect', psycopg_connect)
+    @patch('patroni.postgresql.mpp.citus.quote_ident', Mock())
     @patch.object(Postgresql, 'connection', Mock(return_value=None))
     def test_bootstrap_release_initialize_key_on_watchdog_failure(self):
         self.ha.cluster = get_cluster_not_initialized_without_leader()
         self.e.initialize = true
         self.ha.bootstrap()
         self.p.is_primary = true
         with patch.object(Watchdog, 'activate', Mock(return_value=False)), \
@@ -651,15 +658,15 @@
         with patch.object(self.ha, "restart_matches", return_value=False):
             self.assertEqual(self.ha.restart({'foo': 'bar'}), (False, "restart conditions are not satisfied"))
 
     @patch('time.sleep', Mock())
     @patch.object(ConfigHandler, 'replace_pg_hba', Mock())
     @patch.object(ConfigHandler, 'replace_pg_ident', Mock())
     @patch.object(PostmasterProcess, 'start', Mock(return_value=MockPostmaster()))
-    @patch('patroni.postgresql.citus.CitusHandler.is_coordinator', Mock(return_value=False))
+    @patch('patroni.postgresql.mpp.AbstractMPPHandler.is_coordinator', Mock(return_value=False))
     def test_worker_restart(self):
         self.ha.has_lock = true
         self.ha.patroni.request = Mock()
         self.p.is_running = Mock(side_effect=[Mock(), False])
         self.assertEqual(self.ha.restart({}), (True, 'restarted successfully'))
         self.ha.patroni.request.assert_called()
         self.assertEqual(self.ha.patroni.request.call_args_list[0][0][3]['type'], 'before_demote')
@@ -686,15 +693,15 @@
                     patch('patroni.postgresql.Postgresql.terminate_starting_postmaster') as mock_terminate:
                 self.assertEqual(self.ha.run_cycle(), 'lost leader lock during restart')
                 mock_terminate.assert_called()
 
             self.ha.is_paused = true
             self.assertEqual(self.ha.run_cycle(), 'PAUSE: restart in progress')
 
-    @patch('patroni.postgresql.citus.CitusHandler.is_coordinator', Mock(return_value=False))
+    @patch('patroni.postgresql.mpp.AbstractMPPHandler.is_coordinator', Mock(return_value=False))
     def test_manual_failover_from_leader(self):
         self.ha.has_lock = true  # I am the leader
 
         # to me
         with patch('patroni.ha.logger.warning') as mock_warning:
             self.ha.cluster = get_cluster_initialized_with_leader(Failover(0, '', self.p.name, None))
             self.assertEqual(self.ha.run_cycle(), 'no action. I am (postgresql0), the leader with the lock')
@@ -725,15 +732,15 @@
             self.ha.fetch_node_status = get_node_status(wal_position=1)
             self.ha.cluster.config.data.update({'maximum_lag_on_failover': 5})
             self.assertEqual(self.ha.run_cycle(), 'no action. I am (postgresql0), the leader with the lock')
             self.assertEqual(mock_info.call_args_list[0][0],
                              ('Member %s exceeds maximum replication lag', 'b'))
             self.ha.cluster.members.pop()
 
-    @patch('patroni.postgresql.citus.CitusHandler.is_coordinator', Mock(return_value=False))
+    @patch('patroni.postgresql.mpp.AbstractMPPHandler.is_coordinator', Mock(return_value=False))
     def test_manual_switchover_from_leader(self):
         self.ha.has_lock = true  # I am the leader
 
         self.ha.fetch_node_status = get_node_status()
 
         # different leader specified in failover key, no candidate
         with patch('patroni.ha.logger.warning') as mock_warning:
@@ -762,19 +769,18 @@
             self.ha.fetch_node_status = get_node_status(timeline=1)
             self.assertEqual(self.ha.run_cycle(), 'no action. I am (postgresql0), the leader with the lock')
             self.assertEqual(mock_info.call_args_list[0][0],
                              ('Timeline %s of member %s is behind the cluster timeline %s', 1, 'leader', 2))
         with patch('patroni.ha.logger.info') as mock_info:
             self.ha.fetch_node_status = get_node_status(wal_position=1)
             self.ha.cluster.config.data.update({'maximum_lag_on_failover': 5})
-            self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
             self.assertEqual(self.ha.run_cycle(), 'no action. I am (postgresql0), the leader with the lock')
             self.assertEqual(mock_info.call_args_list[0][0], ('Member %s exceeds maximum replication lag', 'leader'))
 
-    @patch('patroni.postgresql.citus.CitusHandler.is_coordinator', Mock(return_value=False))
+    @patch('patroni.postgresql.mpp.AbstractMPPHandler.is_coordinator', Mock(return_value=False))
     def test_scheduled_switchover_from_leader(self):
         self.ha.has_lock = true  # I am the leader
 
         self.ha.fetch_node_status = get_node_status()
 
         # switchover scheduled time must include timezone
         with patch('patroni.ha.logger.warning') as mock_warning:
@@ -1028,15 +1034,15 @@
             self.assertFalse(self.ha.is_healthiest_node())
         self.ha.is_paused = true
         self.assertFalse(self.ha.is_healthiest_node())
 
     def test__is_healthiest_node(self):
         self.p.is_primary = false
         self.ha.cluster = get_cluster_initialized_without_leader(sync=('postgresql1', self.p.name))
-        self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
+        global_config.update(self.ha.cluster)
         self.assertTrue(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         self.ha.fetch_node_status = get_node_status()  # accessible, in_recovery
         self.assertTrue(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         self.ha.fetch_node_status = get_node_status(in_recovery=False)  # accessible, not in_recovery
         self.assertFalse(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         self.ha.fetch_node_status = get_node_status(failover_priority=2)  # accessible, in_recovery, higher priority
         self.assertFalse(self.ha._is_healthiest_node(self.ha.old_cluster.members))
@@ -1045,15 +1051,15 @@
         self.assertTrue(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         self.ha.fetch_node_status = get_node_status(wal_position=11)  # accessible, in_recovery, wal position ahead
         self.assertFalse(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         # in synchronous_mode consider itself healthy if the former leader is accessible in read-only and ahead of us
         with patch.object(Ha, 'is_synchronous_mode', Mock(return_value=True)):
             self.assertTrue(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         self.ha.cluster.config.data.update({'maximum_lag_on_failover': 5})
-        self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
+        global_config.update(self.ha.cluster)
         with patch('patroni.postgresql.Postgresql.last_operation', return_value=1):
             self.assertFalse(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         with patch('patroni.postgresql.Postgresql.replica_cached_timeline', return_value=None):
             self.assertFalse(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         with patch('patroni.postgresql.Postgresql.replica_cached_timeline', return_value=1):
             self.assertFalse(self.ha._is_healthiest_node(self.ha.old_cluster.members))
         self.ha.patroni.nofailover = True
@@ -1268,31 +1274,30 @@
         self.assertEqual(self.ha.run_cycle(), 'switchover: demoting myself')
 
     @patch('patroni.ha.Ha.demote')
     def test_failover_immediately_on_zero_primary_start_timeout(self, demote):
         self.p.is_running = false
         self.ha.cluster = get_cluster_initialized_with_leader(sync=(self.p.name, 'other'))
         self.ha.cluster.config.data.update({'synchronous_mode': True, 'primary_start_timeout': 0})
-        self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
         self.ha.has_lock = true
         self.ha.update_lock = true
         self.ha.fetch_node_status = get_node_status()  # accessible, in_recovery
         self.assertEqual(self.ha.run_cycle(), 'stopped PostgreSQL to fail over after a crash')
         demote.assert_called_once()
 
     def test_primary_stop_timeout(self):
         self.assertEqual(self.ha.primary_stop_timeout(), None)
         self.ha.cluster.config.data.update({'primary_stop_timeout': 30})
-        self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
+        global_config.update(self.ha.cluster)
         with patch.object(Ha, 'is_synchronous_mode', Mock(return_value=True)):
             self.assertEqual(self.ha.primary_stop_timeout(), 30)
         with patch.object(Ha, 'is_synchronous_mode', Mock(return_value=False)):
             self.assertEqual(self.ha.primary_stop_timeout(), None)
             self.ha.cluster.config.data['primary_stop_timeout'] = None
-            self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
+            global_config.update(self.ha.cluster)
             self.assertEqual(self.ha.primary_stop_timeout(), None)
 
     @patch('patroni.postgresql.Postgresql.follow')
     def test_demote_immediate(self, follow):
         self.ha.has_lock = true
         self.e.get_cluster = Mock(return_value=get_cluster_initialized_without_leader())
         self.ha.demote('immediate')
@@ -1376,16 +1381,16 @@
         self.ha.dcs.get_cluster = Mock(return_value=get_cluster_initialized_with_leader(sync=('somebodyelse', None)))
         self.ha.run_cycle()
         self.assertEqual(self.ha.dcs.write_sync_state.call_count, 2)
 
         # Test sync set to '*' when synchronous_mode_strict is enabled
         mock_set_sync.reset_mock()
         self.p.sync_handler.current_state = Mock(return_value=(CaseInsensitiveSet(), CaseInsensitiveSet()))
-        with patch('patroni.config.GlobalConfig.is_synchronous_mode_strict', PropertyMock(return_value=True)):
-            self.ha.run_cycle()
+        self.ha.cluster.config.data['synchronous_mode_strict'] = True
+        self.ha.run_cycle()
         mock_set_sync.assert_called_once_with(CaseInsensitiveSet('*'))
 
     def test_sync_replication_become_primary(self):
         self.ha.is_synchronous_mode = true
 
         mock_set_sync = self.p.sync_handler.set_synchronous_standby_names = Mock()
         self.p.is_primary = false
@@ -1510,15 +1515,14 @@
         self.ha._disable_sync = True
         self.assertEqual(self.ha.get_effective_tags(), {'foo': 'bar', 'nosync': True})
         self.ha._disable_sync = False
         self.assertEqual(self.ha.get_effective_tags(), {'foo': 'bar'})
 
     @patch('patroni.postgresql.mtime', Mock(return_value=1588316884))
     @patch('builtins.open', Mock(side_effect=Exception))
-    @patch.object(Cluster, 'is_unlocked', Mock(return_value=False))
     def test_restore_cluster_config(self):
         self.ha.cluster.config.data.clear()
         self.ha.has_lock = true
         self.assertEqual(self.ha.run_cycle(), 'no action. I am (postgresql0), the leader with the lock')
 
     def test_watch(self):
         self.ha.cluster = get_cluster_initialized_with_leader()
@@ -1536,15 +1540,15 @@
 
         self.p.stop = stop
         self.ha.shutdown()
 
         self.ha.is_failover_possible = true
         self.ha.shutdown()
 
-    @patch('patroni.postgresql.citus.CitusHandler.is_coordinator', Mock(return_value=False))
+    @patch('patroni.postgresql.mpp.AbstractMPPHandler.is_coordinator', Mock(return_value=False))
     def test_shutdown_citus_worker(self):
         self.ha.is_leader = true
         self.p.is_running = Mock(side_effect=[Mock(), False])
         self.ha.patroni.request = Mock()
         self.ha.shutdown()
         self.ha.patroni.request.assert_called()
         self.assertEqual(self.ha.patroni.request.call_args[0][2], 'citus')
@@ -1648,19 +1652,20 @@
         self.assertTrue(self.ha.run_cycle().startswith('Copying logical slots'))
 
     def test_acquire_lock(self):
         self.ha.dcs.attempt_to_acquire_leader = Mock(side_effect=[DCSError('foo'), Exception])
         self.assertRaises(DCSError, self.ha.acquire_lock)
         self.assertFalse(self.ha.acquire_lock())
 
-    @patch('patroni.postgresql.citus.CitusHandler.is_coordinator', Mock(return_value=False))
+    @patch('patroni.postgresql.mpp.AbstractMPPHandler.is_coordinator', Mock(return_value=False))
     def test_notify_citus_coordinator(self):
         self.ha.patroni.request = Mock()
-        self.ha.notify_citus_coordinator('before_demote')
+        self.ha.notify_mpp_coordinator('before_demote')
         self.ha.patroni.request.assert_called_once()
         self.assertEqual(self.ha.patroni.request.call_args[1]['timeout'], 30)
         self.ha.patroni.request = Mock(side_effect=Exception)
         with patch('patroni.ha.logger.warning') as mock_logger:
-            self.ha.notify_citus_coordinator('before_promote')
+            self.ha.notify_mpp_coordinator('before_promote')
             self.assertEqual(self.ha.patroni.request.call_args[1]['timeout'], 2)
             mock_logger.assert_called()
-            self.assertTrue(mock_logger.call_args[0][0].startswith('Request to Citus coordinator'))
+            self.assertTrue(mock_logger.call_args[0][0].startswith('Request to %s coordinator leader'))
+            self.assertEqual(mock_logger.call_args[0][1], 'Citus')
```

### Comparing `patroni-3.2.2/tests/test_kubernetes.py` & `patroni-3.3.0/tests/test_kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,45 @@
 import mock
 import socket
 import time
 import unittest
 import urllib3
 
 from mock import Mock, PropertyMock, mock_open, patch
+from patroni.dcs import get_dcs
 from patroni.dcs.kubernetes import Cluster, k8s_client, k8s_config, K8sConfig, K8sConnectionFailed, \
     K8sException, K8sObject, Kubernetes, KubernetesError, KubernetesRetriableException, \
     Retry, RetryFailedError, SERVICE_HOST_ENV_NAME, SERVICE_PORT_ENV_NAME
+from patroni.postgresql.mpp import get_mpp
 from threading import Thread
 from . import MockResponse, SleepException
 
 
 def mock_list_namespaced_config_map(*args, **kwargs):
+    k8s_group_label = get_mpp({'citus': {'group': 0, 'database': 'postgres'}}).k8s_group_label
     metadata = {'resource_version': '1', 'labels': {'f': 'b'}, 'name': 'test-config',
                 'annotations': {'initialize': '123', 'config': '{}'}}
     items = [k8s_client.V1ConfigMap(metadata=k8s_client.V1ObjectMeta(**metadata))]
     metadata.update({'name': 'test-leader',
                      'annotations': {'optime': '1234x', 'leader': 'p-0', 'ttl': '30s', 'slots': '{', 'failsafe': '{'}})
     items.append(k8s_client.V1ConfigMap(metadata=k8s_client.V1ObjectMeta(**metadata)))
     metadata.update({'name': 'test-failover', 'annotations': {'leader': 'p-0'}})
     items.append(k8s_client.V1ConfigMap(metadata=k8s_client.V1ObjectMeta(**metadata)))
     metadata.update({'name': 'test-sync', 'annotations': {'leader': 'p-0'}})
     items.append(k8s_client.V1ConfigMap(metadata=k8s_client.V1ObjectMeta(**metadata)))
-    metadata.update({'name': 'test-0-leader', 'labels': {Kubernetes._CITUS_LABEL: '0'},
+    metadata.update({'name': 'test-0-leader', 'labels': {k8s_group_label: '0'},
                      'annotations': {'optime': '1234x', 'leader': 'p-0', 'ttl': '30s', 'slots': '{', 'failsafe': '{'}})
     items.append(k8s_client.V1ConfigMap(metadata=k8s_client.V1ObjectMeta(**metadata)))
-    metadata.update({'name': 'test-0-config', 'labels': {Kubernetes._CITUS_LABEL: '0'},
+    metadata.update({'name': 'test-0-config', 'labels': {k8s_group_label: '0'},
                      'annotations': {'initialize': '123', 'config': '{}'}})
     items.append(k8s_client.V1ConfigMap(metadata=k8s_client.V1ObjectMeta(**metadata)))
-    metadata.update({'name': 'test-1-leader', 'labels': {Kubernetes._CITUS_LABEL: '1'},
+    metadata.update({'name': 'test-1-leader', 'labels': {k8s_group_label: '1'},
                      'annotations': {'leader': 'p-3', 'ttl': '30s'}})
     items.append(k8s_client.V1ConfigMap(metadata=k8s_client.V1ObjectMeta(**metadata)))
-    metadata.update({'name': 'test-2-config', 'labels': {Kubernetes._CITUS_LABEL: '2'}, 'annotations': {}})
+    metadata.update({'name': 'test-2-config', 'labels': {k8s_group_label: '2'}, 'annotations': {}})
     items.append(k8s_client.V1ConfigMap(metadata=k8s_client.V1ObjectMeta(**metadata)))
 
     metadata = k8s_client.V1ObjectMeta(resource_version='1')
     return k8s_client.V1ConfigMapList(metadata=metadata, items=items, kind='ConfigMapList')
 
 
 def mock_read_namespaced_endpoints(*args, **kwargs):
@@ -56,15 +59,16 @@
 
 def mock_list_namespaced_endpoints(*args, **kwargs):
     return k8s_client.V1EndpointsList(metadata=k8s_client.V1ObjectMeta(resource_version='1'),
                                       items=[mock_read_namespaced_endpoints()], kind='V1EndpointsList')
 
 
 def mock_list_namespaced_pod(*args, **kwargs):
-    metadata = k8s_client.V1ObjectMeta(resource_version='1', labels={'f': 'b', Kubernetes._CITUS_LABEL: '1'},
+    k8s_group_label = get_mpp({'citus': {'group': 0, 'database': 'postgres'}}).k8s_group_label
+    metadata = k8s_client.V1ObjectMeta(resource_version='1', labels={'f': 'b', k8s_group_label: '1'},
                                        name='p-0', annotations={'status': '{}'},
                                        uid='964dfeae-e79b-4476-8a5a-1920b5c2a69d')
     status = k8s_client.V1PodStatus(pod_ip='10.0.0.1')
     spec = k8s_client.V1PodSpec(hostname='p-0', node_name='kind-control-plane', containers=[])
     items = [k8s_client.V1Pod(metadata=metadata, status=status, spec=spec)]
     return k8s_client.V1PodList(items=items, kind='PodList')
 
@@ -72,15 +76,15 @@
 def mock_namespaced_kind(*args, **kwargs):
     mock = Mock()
     mock.metadata.resource_version = '2'
     return mock
 
 
 def mock_load_k8s_config(self, *args, **kwargs):
-    self._server = ''
+    self._server = 'http://localhost'
 
 
 class TestK8sConfig(unittest.TestCase):
 
     def test_load_incluster_config(self):
         for env in ({}, {SERVICE_HOST_ENV_NAME: '', SERVICE_PORT_ENV_NAME: ''}):
             with patch('os.environ', env):
@@ -221,26 +225,28 @@
     @patch('socket.TCP_KEEPCNT', 6, create=True)
     @patch.object(Thread, 'start', Mock())
     @patch.object(K8sConfig, 'load_kube_config', mock_load_k8s_config)
     @patch.object(K8sConfig, 'load_incluster_config', Mock(side_effect=k8s_config.ConfigException))
     @patch.object(k8s_client.CoreV1Api, 'list_namespaced_pod', mock_list_namespaced_pod, create=True)
     @patch.object(k8s_client.CoreV1Api, 'list_namespaced_config_map', mock_list_namespaced_config_map, create=True)
     def setUp(self, config=None):
-        config = config or {}
-        config.update(ttl=30, scope='test', name='p-0', loop_wait=10, group=0,
-                      retry_timeout=10, labels={'f': 'b'}, bypass_api_service=True)
-        self.k = Kubernetes(config)
-        self.k._citus_group = None
+        config = {'ttl': 30, 'scope': 'test', 'name': 'p-0', 'loop_wait': 10, 'retry_timeout': 10,
+                  'kubernetes': {'labels': {'f': 'b'}, 'bypass_api_service': True, **(config or {})},
+                  'citus': {'group': 0, 'database': 'postgres'}}
+        self.k = get_dcs(config)
+        self.assertIsInstance(self.k, Kubernetes)
+        self.k._mpp = get_mpp({})
         self.assertRaises(AttributeError, self.k._pods._build_cache)
         self.k._pods._is_ready = True
         self.assertRaises(TypeError, self.k._kinds._build_cache)
         self.k._kinds._is_ready = True
         self.k.get_cluster()
 
 
+@patch('urllib3.PoolManager.request', Mock())
 @patch.object(k8s_client.CoreV1Api, 'patch_namespaced_config_map', mock_namespaced_kind, create=True)
 class TestKubernetesConfigMaps(BaseTestKubernetes):
 
     @patch('time.time', Mock(side_effect=[1, 10.9, 100]))
     def test__wait_caches(self):
         self.k._pods._is_ready = False
         with self.k._condition:
@@ -250,26 +256,39 @@
     def test_get_cluster(self):
         self.k.get_cluster()
 
         with patch.object(Kubernetes, '_wait_caches', Mock(side_effect=Exception)):
             self.assertRaises(KubernetesError, self.k.get_cluster)
 
     def test__get_citus_cluster(self):
-        self.k._citus_group = '0'
+        self.k._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
         cluster = self.k.get_cluster()
         self.assertIsInstance(cluster, Cluster)
         self.assertIsInstance(cluster.workers[1], Cluster)
 
     @patch('patroni.dcs.kubernetes.logger.error')
+    def test_get_mpp_coordinator(self, mock_logger):
+        self.assertIsInstance(self.k.get_mpp_coordinator(), Cluster)
+        with patch.object(Kubernetes, '_postgresql_cluster_loader', Mock(side_effect=Exception)):
+            self.assertIsNone(self.k.get_mpp_coordinator())
+            mock_logger.assert_called()
+            self.assertEqual(mock_logger.call_args[0][0], 'Failed to load %s coordinator cluster from Kubernetes: %r')
+            self.assertEqual(mock_logger.call_args[0][1], 'Null')
+            self.assertIsInstance(mock_logger.call_args[0][2], KubernetesError)
+
+    @patch('patroni.dcs.kubernetes.logger.error')
     def test_get_citus_coordinator(self, mock_logger):
-        self.assertIsInstance(self.k.get_citus_coordinator(), Cluster)
-        with patch.object(Kubernetes, '_cluster_loader', Mock(side_effect=Exception)):
-            self.assertIsNone(self.k.get_citus_coordinator())
+        self.k._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
+        self.assertIsInstance(self.k.get_mpp_coordinator(), Cluster)
+        with patch.object(Kubernetes, '_postgresql_cluster_loader', Mock(side_effect=Exception)):
+            self.assertIsNone(self.k.get_mpp_coordinator())
             mock_logger.assert_called()
-            self.assertTrue(mock_logger.call_args[0][0].startswith('Failed to load Citus coordinator'))
+            self.assertEqual(mock_logger.call_args[0][0], 'Failed to load %s coordinator cluster from Kubernetes: %r')
+            self.assertEqual(mock_logger.call_args[0][1], 'Citus')
+            self.assertIsInstance(mock_logger.call_args[0][2], KubernetesError)
 
     def test_attempt_to_acquire_leader(self):
         with patch.object(k8s_client.CoreV1Api, 'patch_namespaced_config_map', create=True) as mock_patch:
             mock_patch.side_effect = K8sException
             self.assertRaises(KubernetesError, self.k.attempt_to_acquire_leader)
             mock_patch.side_effect = k8s_client.rest.ApiException(409, '')
             self.assertFalse(self.k.attempt_to_acquire_leader())
@@ -352,28 +371,30 @@
         self.assertEqual(self.k._api._retriable_http_codes, self.k._api._DEFAULT_RETRIABLE_HTTP_CODES | set([402]))
         self.k.reload_config({'loop_wait': 10, 'ttl': 30, 'retry_timeout': 10, 'retriable_http_codes': [405, 406]})
         self.assertEqual(self.k._api._retriable_http_codes, self.k._api._DEFAULT_RETRIABLE_HTTP_CODES | set([405, 406]))
         self.k.reload_config({'loop_wait': 10, 'ttl': 30, 'retry_timeout': 10, 'retriable_http_codes': True})
         mock_warning.assert_called_once()
 
 
+@patch('urllib3.PoolManager.request', Mock())
 class TestKubernetesEndpointsNoPodIP(BaseTestKubernetes):
     @patch.object(k8s_client.CoreV1Api, 'list_namespaced_endpoints', mock_list_namespaced_endpoints, create=True)
     def setUp(self, config=None):
         super(TestKubernetesEndpointsNoPodIP, self).setUp({'use_endpoints': True})
 
     @patch.object(k8s_client.CoreV1Api, 'patch_namespaced_endpoints', create=True)
     def test_update_leader(self, mock_patch_namespaced_endpoints):
         leader = self.k.get_cluster().leader
         self.assertIsNotNone(self.k.update_leader(leader, '123', failsafe={'foo': 'bar'}))
         args = mock_patch_namespaced_endpoints.call_args[0]
         self.assertEqual(args[2].subsets[0].addresses[0].target_ref.resource_version, '1')
         self.assertEqual(args[2].subsets[0].addresses[0].ip, '10.0.0.1')
 
 
+@patch('urllib3.PoolManager.request', Mock())
 class TestKubernetesEndpoints(BaseTestKubernetes):
 
     @patch.object(k8s_client.CoreV1Api, 'list_namespaced_endpoints', mock_list_namespaced_endpoints, create=True)
     def setUp(self, config=None):
         super(TestKubernetesEndpoints, self).setUp({'use_endpoints': True, 'pod_ip': '10.0.0.0'})
 
     @patch.object(k8s_client.CoreV1Api, 'patch_namespaced_endpoints', create=True)
@@ -456,21 +477,22 @@
         self.k.write_leader_optime(12345)
 
 
 def mock_watch(*args):
     return urllib3.HTTPResponse()
 
 
+@patch('urllib3.PoolManager.request', Mock())
 class TestCacheBuilder(BaseTestKubernetes):
 
     @patch.object(k8s_client.CoreV1Api, 'list_namespaced_config_map', mock_list_namespaced_config_map, create=True)
     @patch('patroni.dcs.kubernetes.ObjectCache._watch', mock_watch)
     @patch.object(urllib3.HTTPResponse, 'read_chunked')
     def test__build_cache(self, mock_read_chunked):
-        self.k._citus_group = '0'
+        self.k._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
         mock_read_chunked.return_value = [json.dumps(
             {'type': 'MODIFIED', 'object': {'metadata': {
                 'name': self.k.config_path, 'resourceVersion': '2', 'annotations': {self.k._CONFIG: 'foo'}}}}
         ).encode('utf-8'), ('\n' + json.dumps(
             {'type': 'DELETED', 'object': {'metadata': {
                 'name': self.k.config_path, 'resourceVersion': '3'}}}
         ) + '\n' + json.dumps(
```

### Comparing `patroni-3.2.2/tests/test_patroni.py` & `patroni-3.3.0/tests/test_patroni.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,14 +150,15 @@
     def test_run(self):
         self.p.postgresql.set_role('replica')
         self.p.sighup_handler()
         self.p.ha.dcs.watch = Mock(side_effect=SleepException)
         self.p.api.start = Mock()
         self.p.logger.start = Mock()
         self.p.config._dynamic_configuration = {}
+        self.assertRaises(SleepException, self.p.run)
         with patch('patroni.dcs.Cluster.is_unlocked', Mock(return_value=True)):
             self.assertRaises(SleepException, self.p.run)
         with patch('patroni.config.Config.reload_local_configuration', Mock(return_value=False)):
             self.p.sighup_handler()
             self.assertRaises(SleepException, self.p.run)
         with patch('patroni.config.Config.set_dynamic_configuration', Mock(return_value=True)):
             self.assertRaises(SleepException, self.p.run)
@@ -244,14 +245,24 @@
 
     def test_nosync(self):
         self.p.tags['nosync'] = True
         self.assertTrue(self.p.nosync)
         self.p.tags['nosync'] = None
         self.assertFalse(self.p.nosync)
 
+    def test_nostream(self):
+        self.p.tags['nostream'] = 'True'
+        self.assertTrue(self.p.nostream)
+        self.p.tags['nostream'] = 'None'
+        self.assertFalse(self.p.nostream)
+        self.p.tags['nostream'] = 'foo'
+        self.assertFalse(self.p.nostream)
+        self.p.tags['nostream'] = ''
+        self.assertFalse(self.p.nostream)
+
     @patch.object(Thread, 'join', Mock())
     def test_shutdown(self):
         self.p.api.shutdown = Mock(side_effect=Exception)
         self.p.ha.shutdown = Mock(side_effect=Exception)
         self.p.shutdown()
 
     def test_check_psycopg(self):
```

### Comparing `patroni-3.2.2/tests/test_postgresql.py` & `patroni-3.3.0/tests/test_postgresql.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import psutil
 import re
 import subprocess
 import time
 
 from copy import deepcopy
 from mock import Mock, MagicMock, PropertyMock, patch, mock_open
+from pathlib import Path
 
 import patroni.psycopg as psycopg
 
+from patroni import global_config
 from patroni.async_executor import CriticalTask
-from patroni.collections import CaseInsensitiveSet
-from patroni.config import GlobalConfig
+from patroni.collections import CaseInsensitiveDict, CaseInsensitiveSet
 from patroni.dcs import RemoteMember
 from patroni.exceptions import PostgresConnectionException, PatroniException
 from patroni.postgresql import Postgresql, STATE_REJECT, STATE_NO_RESPONSE
 from patroni.postgresql.bootstrap import Bootstrap
 from patroni.postgresql.callback_executor import CallbackAction
-from patroni.postgresql.config import _false_validator
+from patroni.postgresql.config import get_param_diff, _false_validator
 from patroni.postgresql.postmaster import PostmasterProcess
 from patroni.postgresql.validator import (ValidatorFactoryNoType, ValidatorFactoryInvalidType,
                                           ValidatorFactoryInvalidSpec, ValidatorFactory, InvalidGucValidatorsFile,
                                           _get_postgres_guc_validators, _read_postgres_gucs_validators_file,
                                           _load_postgres_gucs_validators, Bool, Integer, Real, Enum, EnumBool, String)
 from patroni.utils import RetryFailedError
 from threading import Thread, current_thread
@@ -359,15 +360,15 @@
         self.p.config.write_recovery_conf({'foo': 'bar'})
         self.p.config.write_postgresql_conf()
 
     @patch.object(Postgresql, 'is_running', Mock(return_value=False))
     @patch.object(Postgresql, 'start', Mock())
     def test_follow(self):
         self.p.call_nowait(CallbackAction.ON_START)
-        m = RemoteMember('1', {'restore_command': '2', 'primary_slot_name': 'foo', 'conn_kwargs': {'host': 'bar'}})
+        m = RemoteMember('1', {'restore_command': '2', 'primary_slot_name': 'foo', 'conn_kwargs': {'host': 'foo,bar'}})
         self.p.follow(m)
         with patch.object(Postgresql, 'ensure_major_version_is_known', Mock(return_value=False)):
             self.assertIsNone(self.p.follow(m))
 
     @patch.object(MockCursor, 'execute', Mock(side_effect=psycopg.OperationalError))
     def test__query(self):
         self.assertRaises(PostgresConnectionException, self.p._query, 'blabla')
@@ -567,104 +568,135 @@
     def test_reload_config(self, mock_warning, mock_info):
         config = deepcopy(self.p.config._config)
 
         # Nothing changed
         self.p.reload_config(config)
         mock_info.assert_called_once_with('No PostgreSQL configuration items changed, nothing to reload.')
         mock_warning.assert_not_called()
-        self.assertEqual(self.p.pending_restart, False)
+        self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict())
 
         mock_info.reset_mock()
 
         # Ignored params changed
         config['parameters']['archive_cleanup_command'] = 'blabla'
         self.p.reload_config(config)
         mock_info.assert_called_once_with('No PostgreSQL configuration items changed, nothing to reload.')
-        self.assertEqual(self.p.pending_restart, False)
+        self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict())
 
         mock_info.reset_mock()
 
         # Handle wal_buffers
         self.p.config._config['parameters']['wal_buffers'] = '512'
         self.p.reload_config(config)
         mock_info.assert_called_once_with('No PostgreSQL configuration items changed, nothing to reload.')
-        self.assertEqual(self.p.pending_restart, False)
+        self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict())
 
         mock_info.reset_mock()
         config = deepcopy(self.p.config._config)
 
         # hba/ident_changed
         config['pg_hba'] = ['']
         config['pg_ident'] = ['']
         self.p.reload_config(config)
         mock_info.assert_called_once_with('Reloading PostgreSQL configuration.')
-        self.assertEqual(self.p.pending_restart, False)
+        self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict())
 
         mock_info.reset_mock()
 
         # Postmaster parameter change (pending_restart)
         init_max_worker_processes = config['parameters']['max_worker_processes']
         config['parameters']['max_worker_processes'] *= 2
-        with patch('patroni.postgresql.Postgresql._query', Mock(side_effect=[GET_PG_SETTINGS_RESULT, [(1,)]])):
+        new_max_worker_processes = config['parameters']['max_worker_processes']
+        # stale reason to be removed
+        self.p._pending_restart_reason = CaseInsensitiveDict({'max_connections': get_param_diff('200', '100')})
+
+        with patch.object(Postgresql, 'get_guc_value', Mock(return_value=str(new_max_worker_processes))), \
+             patch('patroni.postgresql.Postgresql._query', Mock(side_effect=[
+                 GET_PG_SETTINGS_RESULT, [('max_worker_processes', str(init_max_worker_processes), None, 'integer')]])):
             self.p.reload_config(config)
-            self.assertEqual(mock_info.call_args_list[0][0], ('Changed %s from %s to %s (restart might be required)',
-                                                              'max_worker_processes', str(init_max_worker_processes),
-                                                              config['parameters']['max_worker_processes']))
+            self.assertEqual(mock_info.call_args_list[0][0],
+                             ("Changed %s from '%s' to '%s' (restart might be required)", 'max_worker_processes',
+                              str(init_max_worker_processes), config['parameters']['max_worker_processes']))
             self.assertEqual(mock_info.call_args_list[1][0], ('Reloading PostgreSQL configuration.',))
-            self.assertEqual(self.p.pending_restart, True)
+            self.assertEqual(self.p.pending_restart_reason,
+                             CaseInsensitiveDict({'max_worker_processes': get_param_diff(init_max_worker_processes,
+                                                                                         new_max_worker_processes)}))
 
         mock_info.reset_mock()
 
         # Reset to the initial value without restart
         config['parameters']['max_worker_processes'] = init_max_worker_processes
         self.p.reload_config(config)
-        self.assertEqual(mock_info.call_args_list[0][0], ('Changed %s from %s to %s', 'max_worker_processes',
+        self.assertEqual(mock_info.call_args_list[0][0], ("Changed %s from '%s' to '%s'", 'max_worker_processes',
                                                           init_max_worker_processes * 2,
-                                                          str(config['parameters']['max_worker_processes'])))
+                                                          config['parameters']['max_worker_processes']))
         self.assertEqual(mock_info.call_args_list[1][0], ('Reloading PostgreSQL configuration.',))
-        self.assertEqual(self.p.pending_restart, False)
+        self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict())
 
         mock_info.reset_mock()
 
         # User-defined parameter changed (removed)
         config['parameters'].pop('f.oo')
         self.p.reload_config(config)
-        self.assertEqual(mock_info.call_args_list[0][0], ('Changed %s from %s to %s', 'f.oo', 'bar', None))
+        self.assertEqual(mock_info.call_args_list[0][0], ("Changed %s from '%s' to '%s'", 'f.oo', 'bar', None))
         self.assertEqual(mock_info.call_args_list[1][0], ('Reloading PostgreSQL configuration.',))
-        self.assertEqual(self.p.pending_restart, False)
+        self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict())
 
         mock_info.reset_mock()
 
         # Non-postmaster parameter change
-        config['parameters']['autovacuum'] = 'off'
+        config['parameters']['vacuum_cost_delay'] = 2.5
         self.p.reload_config(config)
-        self.assertEqual(mock_info.call_args_list[0][0], ("Changed %s from %s to %s", 'autovacuum', 'on', 'off'))
+        self.assertEqual(mock_info.call_args_list[0][0],
+                         ("Changed %s from '%s' to '%s'", 'vacuum_cost_delay', '200ms', 2.5))
         self.assertEqual(mock_info.call_args_list[1][0], ('Reloading PostgreSQL configuration.',))
-        self.assertEqual(self.p.pending_restart, False)
+        self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict())
 
-        config['parameters']['autovacuum'] = 'on'
+        config['parameters']['vacuum_cost_delay'] = 200
         mock_info.reset_mock()
 
         # Remove invalid parameter
         config['parameters']['invalid'] = 'value'
         self.p.reload_config(config)
         self.assertEqual(mock_warning.call_args_list[0][0],
                          ('Removing invalid parameter `%s` from postgresql.parameters', 'invalid'))
         config['parameters'].pop('invalid')
 
         mock_warning.reset_mock()
         mock_info.reset_mock()
 
-        # Non-empty result (outside changes) and exception while querying pending_restart parameters
-        with patch('patroni.postgresql.Postgresql._query',
-                   Mock(side_effect=[GET_PG_SETTINGS_RESULT, [(1,)], GET_PG_SETTINGS_RESULT, Exception])):
+        # Non-empty result (outside changes)
+        with patch.object(Postgresql, 'get_guc_value', Mock(side_effect=['73', None, ''])), \
+             patch('patroni.postgresql.Postgresql._query',
+                   Mock(side_effect=[GET_PG_SETTINGS_RESULT, [('shared_buffers', '128MB', '8kB', 'integer')]] * 3)):
+            # pg_settings shared_buffers (current value) == 128MB (16384)
+            # Patroni config shared_buffers == 42MB (should not end up in the restart reason diff)
+            # get_guc_value (will be used after restart) == 73 (584kB)
+            config['parameters']['shared_buffers'] = '42MB'
             self.p.reload_config(config, True)
-            self.assertEqual(mock_info.call_args_list[0][0], ('Reloading PostgreSQL configuration.',))
-            self.assertEqual(self.p.pending_restart, True)
+            self.assertEqual(mock_info.call_args_list[0][0],
+                             ("Changed %s from '%s' to '%s' (restart might be required)",
+                              'shared_buffers', '128MB', '42MB'))
+            self.assertEqual(mock_info.call_args_list[1][0], ('Reloading PostgreSQL configuration.',))
+            self.assertEqual(mock_info.call_args_list[2][0], ("PostgreSQL configuration parameters requiring restart"
+                                                              " (%s) seem to be changed bypassing Patroni config."
+                                                              " Setting 'Pending restart' flag", 'shared_buffers'))
+            self.assertEqual(self.p.pending_restart_reason,
+                             CaseInsensitiveDict({'shared_buffers': get_param_diff('128MB', '584kB')}))
+
+            self.p.reload_config(config, True)
+            self.assertEqual(self.p.pending_restart_reason,
+                             CaseInsensitiveDict({'shared_buffers': get_param_diff('128MB', '?')}))
+
+            self.p.reload_config(config, True)
+            self.assertEqual(self.p.pending_restart_reason,
+                             CaseInsensitiveDict({'shared_buffers': get_param_diff('128MB', '')}))
 
+        # Exception while querying pending_restart parameters
+        with patch('patroni.postgresql.Postgresql._query', Mock(side_effect=[GET_PG_SETTINGS_RESULT, Exception])):
             # Invalid values, just to increase silly coverage in postgresql.validator.
             # One day we will have proper tests there.
             config['parameters']['autovacuum'] = 'of'  # Bool.transform()
             config['parameters']['vacuum_cost_limit'] = 'smth'  # Number.transform()
             self.p.reload_config(config, True)
             self.assertEqual(mock_warning.call_args_list[-1][0][0], 'Exception %r when running query')
 
@@ -771,20 +803,20 @@
         with patch.object(Postgresql, 'check_startup_state_changed', Mock(return_value=False)):
             self.p.cancellable.cancel()
             self.p._state = 'starting'
             self.assertIsNone(self.p.wait_for_startup())
 
     def test_get_server_parameters(self):
         config = {'parameters': {'wal_level': 'hot_standby', 'max_prepared_transactions': 100}, 'listen': '0'}
-        self.p._global_config = GlobalConfig({'synchronous_mode': True})
-        self.p.config.get_server_parameters(config)
-        self.p._global_config = GlobalConfig({'synchronous_mode': True, 'synchronous_mode_strict': True})
-        self.p.config.get_server_parameters(config)
-        self.p.config.set_synchronous_standby_names('foo')
-        self.assertTrue(str(self.p.config.get_server_parameters(config)).startswith('<CaseInsensitiveDict'))
+        with patch.object(global_config.__class__, 'is_synchronous_mode', PropertyMock(return_value=True)):
+            self.p.config.get_server_parameters(config)
+            with patch.object(global_config.__class__, 'is_synchronous_mode_strict', PropertyMock(return_value=True)):
+                self.p.config.get_server_parameters(config)
+                self.p.config.set_synchronous_standby_names('foo')
+                self.assertTrue(str(self.p.config.get_server_parameters(config)).startswith('<CaseInsensitiveDict'))
 
     @patch('time.sleep', Mock())
     def test__wait_for_connection_close(self):
         mock_postmaster = MockPostmaster()
         with patch.object(Postgresql, 'is_running', Mock(return_value=mock_postmaster)):
             mock_postmaster.is_running.side_effect = [True, False, False]
             mock_callback = Mock()
@@ -814,28 +846,35 @@
         controldata = {'max_connections setting': '100', 'max_worker_processes setting': '8',
                        'max_locks_per_xact setting': '64', 'max_wal_senders setting': 5}
 
         with patch.object(Postgresql, 'controldata', Mock(return_value=controldata)), \
              patch.object(Bootstrap, 'keep_existing_recovery_conf', PropertyMock(return_value=True)):
             self.p.cancellable.cancel()
             self.assertFalse(self.p.start())
-            self.assertFalse(self.p.pending_restart)
+            self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict())
             mock_logger.warning.assert_called_once()
             self.assertEqual(mock_logger.warning.call_args[0],
                              ('%s is missing from pg_controldata output', 'max_prepared_xacts setting'))
 
         mock_logger.reset_mock()
         controldata['max_prepared_xacts setting'] = 0
         controldata['max_wal_senders setting'] *= 2
 
         with patch.object(Postgresql, 'controldata', Mock(return_value=controldata)):
             self.p.config.write_recovery_conf({'pause_at_recovery_target': 'false'})
             self.assertFalse(self.p.start())
             mock_logger.warning.assert_not_called()
-            self.assertTrue(self.p.pending_restart)
+            self.assertEqual(self.p.pending_restart_reason, CaseInsensitiveDict({
+                'max_wal_senders': get_param_diff('10', '5')
+            }))
+            mock_logger.info.assert_called_once()
+            self.assertEqual(mock_logger.info.call_args[0],
+                             ("%s value in pg_controldata: %d, in the global configuration: %d."
+                              " pg_controldata value will be used. Setting 'Pending restart' flag",
+                              'max_wal_senders', 10, 5))
 
     @patch('os.path.exists', Mock(return_value=True))
     @patch('os.path.isfile', Mock(return_value=False))
     def test_pgpass_is_dir(self):
         self.assertRaises(PatroniException, self.setUp)
 
     @patch.object(Postgresql, '_query', Mock(side_effect=RetryFailedError('')))
@@ -1022,34 +1061,49 @@
             self.assertEqual(mock_call[0], 'Faced an issue while parsing a validator for parameter `%s`: `%r`')
             self.assertEqual(mock_call[1], parameter)
             self.assertIsInstance(mock_call[2], ValidatorFactoryNoType)
 
     def test__read_postgres_gucs_validators_file(self):
         # raise exception
         with self.assertRaises(InvalidGucValidatorsFile) as exc:
-            _read_postgres_gucs_validators_file('random_file.yaml')
+            _read_postgres_gucs_validators_file(Path('random_file.yaml'))
         self.assertEqual(
             str(exc.exception),
             "Unexpected issue while reading parameters file `random_file.yaml`: `[Errno 2] No such file or directory: "
             "'random_file.yaml'`."
         )
 
     def test__load_postgres_gucs_validators(self):
         # log messages
-        with patch('os.walk', Mock(return_value=iter([('.', [], ['file.txt', 'random.yaml'])]))), \
-             patch('patroni.postgresql.validator.logger.info') as mock_info, \
+        file1_attrs = {'is_file.return_value': True, 'is_dir.return_value': False}
+        file1_mock = MagicMock(**file1_attrs)
+        file1_mock.name = '__init__.py'
+        file2_attrs = {'is_file.return_value': False, 'is_dir.return_value': True, 'iterdir.return_value': []}
+        file2_mock = MagicMock(**file2_attrs)
+        file2_mock.name = '__pycache__'
+        file3_attrs = {'is_file.return_value': True, 'is_dir.return_value': False}
+        file3_mock = MagicMock(**file3_attrs)
+        file3_mock.name = file3_mock.__str__.return_value = 'random.yaml'
+        file3_mock.open.side_effect = FileNotFoundError('[Errno 2] No such file or directory: random.yaml')
+        file4_attrs = {'is_file.return_value': True, 'is_dir.return_value': False}
+        file4_mock = MagicMock(**file4_attrs)
+        file4_mock.name = 'file.txt'
+        dir_attrs = {'name': 'available_parameters', 'is_file.return_value': False, 'is_dir.return_value': True}
+        dir_mock = MagicMock(**dir_attrs)
+        dir_mock.iterdir.return_value = [file1_mock, file2_mock, file3_mock, file4_mock]
+        with patch('patroni.postgresql.available_parameters.conf_dir', dir_mock), \
+             patch('patroni.postgresql.available_parameters.logger.info') as mock_info, \
              patch('patroni.postgresql.validator.logger.warning') as mock_warning:
             _load_postgres_gucs_validators()
-            mock_info.assert_called_once_with('Ignored a non-YAML file found under `available_parameters` directory: '
-                                              '`%s`.', os.path.join('.', 'file.txt'))
+            mock_info.assert_called_once_with('Ignored a non-YAML file found under `%s` '
+                                              'directory: `%s`.', 'available_parameters', file4_mock)
             mock_warning.assert_called_once()
             self.assertIn(
-                "Unexpected issue while reading parameters file `{0}`: `[Errno 2] No such file or "
-                "directory:".format(os.path.join('.', 'random.yaml')),
-                mock_warning.call_args[0][0]
+                "Unexpected issue while reading parameters file `random.yaml`: `[Errno 2] No such file or "
+                "directory:", mock_warning.call_args[0][0]
             )
 
 
 @patch('subprocess.call', Mock(return_value=0))
 @patch('patroni.psycopg.connect', psycopg_connect)
 class TestPostgresql2(BaseTestPostgresql):
```

### Comparing `patroni-3.2.2/tests/test_postmaster.py` & `patroni-3.3.0/tests/test_postmaster.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_raft.py` & `patroni-3.3.0/tests/test_raft.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import unittest
 import tempfile
 import time
 
 from mock import Mock, PropertyMock, patch
+from patroni.dcs import get_dcs
 from patroni.dcs.raft import Cluster, DynMemberSyncObj, KVStoreTTL, \
     Raft, RaftError, SyncObjUtility, TCPTransport, _TCPTransport
+from patroni.postgresql.mpp import get_mpp
 from pysyncobj import SyncObjConf, FAIL_REASON
 
 
 def remove_files(prefix):
     for f in ('journal', 'journal.meta', 'dump'):
         f = prefix + f
         if os.path.isfile(f):
@@ -124,46 +126,47 @@
 
 
 class TestRaft(unittest.TestCase):
 
     _TMP = tempfile.gettempdir()
 
     def test_raft(self):
-        raft = Raft({'ttl': 30, 'scope': 'test', 'name': 'pg', 'self_addr': '127.0.0.1:1234',
-                     'retry_timeout': 10, 'data_dir': self._TMP,
-                     'database': 'citus', 'group': 0})
+        raft = get_dcs({'ttl': 30, 'scope': 'test', 'name': 'pg', 'retry_timeout': 10,
+                        'raft': {'self_addr': '127.0.0.1:1234', 'data_dir': self._TMP},
+                        'citus': {'group': 0, 'database': 'postgres'}})
+        self.assertIsInstance(raft, Raft)
         raft.reload_config({'retry_timeout': 20, 'ttl': 60, 'loop_wait': 10})
         self.assertTrue(raft._sync_obj.set(raft.members_path + 'legacy', '{"version":"2.0.0"}'))
         self.assertTrue(raft.touch_member(''))
         self.assertTrue(raft.initialize())
         self.assertTrue(raft.cancel_initialization())
         self.assertTrue(raft.set_config_value('{}'))
         self.assertTrue(raft.write_sync_state('foo', 'bar'))
         self.assertFalse(raft.write_sync_state('foo', 'bar', 1))
-        raft._citus_group = '1'
+        raft._mpp = get_mpp({'citus': {'group': 1, 'database': 'postgres'}})
         self.assertTrue(raft.manual_failover('foo', 'bar'))
-        raft._citus_group = '0'
+        raft._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
         self.assertTrue(raft.take_leader())
         cluster = raft.get_cluster()
         self.assertIsInstance(cluster, Cluster)
         self.assertIsInstance(cluster.workers[1], Cluster)
         leader = cluster.leader
         self.assertTrue(raft.delete_leader(leader))
         self.assertTrue(raft._sync_obj.set(raft.status_path, '{"optime":1234567,"slots":{"ls":12345}}'))
         raft.get_cluster()
         self.assertTrue(raft.update_leader(leader, '1', failsafe={'foo': 'bat'}))
         self.assertTrue(raft._sync_obj.set(raft.failsafe_path, '{"foo"}'))
         self.assertTrue(raft._sync_obj.set(raft.status_path, '{'))
-        raft.get_citus_coordinator()
+        raft.get_mpp_coordinator()
         self.assertTrue(raft.delete_sync_state())
         self.assertTrue(raft.set_history_value(''))
         self.assertTrue(raft.delete_cluster())
-        raft._citus_group = '1'
+        raft._mpp = get_mpp({'citus': {'group': 1, 'database': 'postgres'}})
         self.assertTrue(raft.delete_cluster())
-        raft._citus_group = None
+        raft._mpp = get_mpp({})
         raft.get_cluster()
         raft.watch(None, 0.001)
         raft._sync_obj.destroy()
 
     def tearDown(self):
         remove_files(os.path.join(self._TMP, '127.0.0.1:1234.'))
 
@@ -171,9 +174,9 @@
         self.tearDown()
 
     @patch('patroni.dcs.raft.KVStoreTTL')
     @patch('threading.Event')
     def test_init(self, mock_event, mock_kvstore):
         mock_kvstore.return_value.applied_local_log = False
         mock_event.return_value.is_set.side_effect = [False, True]
-        self.assertIsNotNone(Raft({'ttl': 30, 'scope': 'test', 'name': 'pg', 'patronictl': True,
-                                   'self_addr': '1', 'data_dir': self._TMP}))
+        self.assertIsInstance(get_dcs({'ttl': 30, 'scope': 'test', 'name': 'pg', 'patronictl': True,
+                                       'raft': {'self_addr': '1', 'data_dir': self._TMP}}), Raft)
```

### Comparing `patroni-3.2.2/tests/test_raft_controller.py` & `patroni-3.3.0/tests/test_raft_controller.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_rewind.py` & `patroni-3.3.0/tests/test_rewind.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,16 @@
         with patch.object(Postgresql, 'is_running', Mock(return_value=True)), \
                 patch.object(MockCursor, 'fetchone', Mock(side_effect=Exception)), \
                 patch.object(MockCursor, 'fetchall',
                              Mock(return_value=[(0, 0, 1, 1, 0, 0, 0, 0, 0, None, None, None)])):
             self.r.rewind_or_reinitialize_needed_and_possible(self.leader)
 
     @patch.object(CancellableSubprocess, 'call', mock_cancellable_call)
-    @patch.object(Postgresql, 'checkpoint', side_effect=['', '1'],)
+    @patch.object(Postgresql, 'get_guc_value', Mock(return_value=''))
+    @patch.object(Postgresql, 'checkpoint', side_effect=['', '1'])
     @patch.object(Postgresql, 'stop', Mock(return_value=False))
     @patch.object(Postgresql, 'start', Mock())
     def test_execute(self, mock_checkpoint):
         self.r.execute(self.leader)
         with patch.object(Postgresql, 'major_version', PropertyMock(return_value=130000)):
             self.r.execute(self.leader)
             with patch.object(MockCursor, 'fetchone', Mock(side_effect=Exception)):
```

### Comparing `patroni-3.2.2/tests/test_slots.py` & `patroni-3.3.0/tests/test_slots.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,104 +2,115 @@
 import os
 import unittest
 
 
 from mock import Mock, PropertyMock, patch
 from threading import Thread
 
-from patroni import psycopg
-from patroni.config import GlobalConfig
+from patroni import global_config, psycopg
 from patroni.dcs import Cluster, ClusterConfig, Member, Status, SyncState
 from patroni.postgresql import Postgresql
 from patroni.postgresql.misc import fsync_dir
 from patroni.postgresql.slots import SlotsAdvanceThread, SlotsHandler
+from patroni.tags import Tags
 
 from . import BaseTestPostgresql, psycopg_connect, MockCursor
 
 
+class TestTags(Tags):
+
+    @property
+    def tags(self):
+        return {}
+
+
 @patch('subprocess.call', Mock(return_value=0))
 @patch('patroni.psycopg.connect', psycopg_connect)
 @patch.object(Thread, 'start', Mock())
 @patch.object(Postgresql, 'is_running', Mock(return_value=True))
 class TestSlotsHandler(BaseTestPostgresql):
 
     @patch('subprocess.call', Mock(return_value=0))
     @patch('os.rename', Mock())
     @patch('patroni.postgresql.CallbackExecutor', Mock())
     @patch.object(Postgresql, 'get_major_version', Mock(return_value=130000))
     @patch.object(Postgresql, 'is_running', Mock(return_value=True))
     def setUp(self):
         super(TestSlotsHandler, self).setUp()
-        self.p._global_config = GlobalConfig({})
         self.s = self.p.slots_handler
         self.p.start()
         config = ClusterConfig(1, {'slots': {'ls': {'database': 'a', 'plugin': 'b'}, 'ls2': None}}, 1)
         self.cluster = Cluster(True, config, self.leader, Status(0, {'ls': 12345, 'ls2': 12345}),
                                [self.me, self.other, self.leadermem], None, SyncState.empty(), None, None)
+        global_config.update(self.cluster)
+        self.tags = TestTags()
 
     def test_sync_replication_slots(self):
         config = ClusterConfig(1, {'slots': {'test_3': {'database': 'a', 'plugin': 'b'},
                                              'A': 0, 'ls': 0, 'b': {'type': 'logical', 'plugin': '1'}},
                                    'ignore_slots': [{'name': 'blabla'}]}, 1)
         cluster = Cluster(True, config, self.leader, Status(0, {'test_3': 10}),
                           [self.me, self.other, self.leadermem], None, SyncState.empty(), None, None)
+        global_config.update(cluster)
         with mock.patch('patroni.postgresql.Postgresql._query', Mock(side_effect=psycopg.OperationalError)):
-            self.s.sync_replication_slots(cluster, False)
+            self.s.sync_replication_slots(cluster, self.tags)
         self.p.set_role('standby_leader')
         with patch.object(SlotsHandler, 'drop_replication_slot', Mock(return_value=(True, False))), \
-                patch.object(GlobalConfig, 'is_standby_cluster', PropertyMock(return_value=True)), \
+                patch.object(global_config.__class__, 'is_standby_cluster', PropertyMock(return_value=True)), \
                 patch('patroni.postgresql.slots.logger.debug') as mock_debug:
-            self.s.sync_replication_slots(cluster, False)
+            self.s.sync_replication_slots(cluster, self.tags)
             mock_debug.assert_called_once()
         self.p.set_role('replica')
         with patch.object(Postgresql, 'is_primary', Mock(return_value=False)), \
+                patch.object(global_config.__class__, 'is_paused', PropertyMock(return_value=True)), \
                 patch.object(SlotsHandler, 'drop_replication_slot') as mock_drop:
             config.data['slots'].pop('ls')
-            self.s.sync_replication_slots(cluster, False, paused=True)
+            self.s.sync_replication_slots(cluster, self.tags)
             mock_drop.assert_not_called()
         self.p.set_role('primary')
         with mock.patch('patroni.postgresql.Postgresql.role', new_callable=PropertyMock(return_value='replica')):
-            self.s.sync_replication_slots(cluster, False)
+            self.s.sync_replication_slots(cluster, self.tags)
         with patch('patroni.dcs.logger.error', new_callable=Mock()) as errorlog_mock:
             alias1 = Member(0, 'test-3', 28, {'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5436/postgres'})
             alias2 = Member(0, 'test.3', 28, {'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5436/postgres'})
             cluster.members.extend([alias1, alias2])
-            self.s.sync_replication_slots(cluster, False)
+            self.s.sync_replication_slots(cluster, self.tags)
             self.assertEqual(errorlog_mock.call_count, 5)
             ca = errorlog_mock.call_args_list[0][0][1]
             self.assertTrue("test-3" in ca, "non matching {0}".format(ca))
             self.assertTrue("test.3" in ca, "non matching {0}".format(ca))
             with patch.object(Postgresql, 'major_version', PropertyMock(return_value=90618)):
-                self.s.sync_replication_slots(cluster, False)
+                self.s.sync_replication_slots(cluster, self.tags)
                 self.p.set_role('replica')
-                self.s.sync_replication_slots(cluster, False)
+                self.s.sync_replication_slots(cluster, self.tags)
 
     def test_cascading_replica_sync_replication_slots(self):
         """Test sync with a cascading replica so physical slots are present on a replica."""
         config = ClusterConfig(1, {'slots': {'ls': {'database': 'a', 'plugin': 'b'}}}, 1)
         cascading_replica = Member(0, 'test-2', 28, {
             'state': 'running', 'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5436/postgres',
             'tags': {'replicatefrom': 'postgresql0'}
         })
         cluster = Cluster(True, config, self.leader, Status(0, {'ls': 10}),
                           [self.me, self.other, self.leadermem, cascading_replica], None, SyncState.empty(), None, None)
         self.p.set_role('replica')
         with patch.object(Postgresql, '_query') as mock_query, \
                 patch.object(Postgresql, 'is_primary', Mock(return_value=False)):
             mock_query.return_value = [('ls', 'logical', 104, 'b', 'a', 5, 12345, 105)]
-            ret = self.s.sync_replication_slots(cluster, False)
+            ret = self.s.sync_replication_slots(cluster, self.tags)
         self.assertEqual(ret, [])
 
     def test_process_permanent_slots(self):
         config = ClusterConfig(1, {'slots': {'ls': {'database': 'a', 'plugin': 'b'}, 'blabla': {'type': 'physical'}},
                                    'ignore_slots': [{'name': 'blabla'}]}, 1)
         cluster = Cluster(True, config, self.leader, Status.empty(), [self.me, self.other, self.leadermem],
                           None, SyncState.empty(), None, None)
+        global_config.update(cluster)
 
-        self.s.sync_replication_slots(cluster, False)
+        self.s.sync_replication_slots(cluster, self.tags)
         with patch.object(Postgresql, '_query') as mock_query:
             self.p.reset_cluster_info_state(None)
             mock_query.return_value = [(
                 1, 0, 0, 0, 0, 0, 0, 0, 0, None, None,
                 [{"slot_name": "ls", "type": "logical", "datoid": 5, "plugin": "b",
                   "confirmed_flush_lsn": 12345, "catalog_xmin": 105, "restart_lsn": 12344},
                  {"slot_name": "blabla", "type": "physical", "datoid": None, "plugin": None,
@@ -109,61 +120,123 @@
             self.p.reset_cluster_info_state(None)
             mock_query.return_value = [(
                 1, 0, 0, 0, 0, 0, 0, 0, 0, None, None,
                 [{"slot_name": "ls", "type": "logical", "datoid": 6, "plugin": "b",
                   "confirmed_flush_lsn": 12345, "catalog_xmin": 105}])]
             self.assertEqual(self.p.slots(), {})
 
+    def test_nostream_slot_processing(self):
+        config = ClusterConfig(
+            1, {'slots': {'foo': {'type': 'logical', 'database': 'a', 'plugin': 'b'}, 'bar': {'type': 'physical'}}}, 1)
+        nostream_node = Member(0, 'test-2', 28, {
+            'state': 'running', 'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5436/postgres',
+            'tags': {'nostream': 'True'}
+        })
+        cascade_node = Member(0, 'test-3', 28, {
+            'state': 'running', 'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5436/postgres',
+            'tags': {'replicatefrom': 'test-2'}
+        })
+        stream_node = Member(0, 'test-4', 28, {
+            'state': 'running', 'conn_url': 'postgres://replicator:rep-pass@127.0.0.1:5436/postgres'})
+        cluster = Cluster(
+            True, config, self.leader, Status.empty(),
+            [self.leadermem, nostream_node, cascade_node, stream_node], None, SyncState.empty(), None, None)
+        global_config.update(cluster)
+
+        # sanity for primary
+        self.p.name = self.leadermem.name
+        self.assertEqual(
+            cluster._get_permanent_slots(self.p, self.leadermem, 'primary'),
+            {'foo': {'type': 'logical', 'database': 'a', 'plugin': 'b'}, 'bar': {'type': 'physical'}})
+        self.assertEqual(
+            cluster._get_members_slots(self.p.name, 'primary'),
+            {'test_4': {'type': 'physical'}})
+
+        # nostream node must not have slot on primary
+        self.p.name = nostream_node.name
+        # permanent logical slots are not allowed on nostream node
+        self.assertEqual(
+            cluster._get_permanent_slots(self.p, nostream_node, 'replica'),
+            {'bar': {'type': 'physical'}})
+        self.assertEqual(
+            cluster.get_slot_name_on_primary(self.p.name, nostream_node),
+            None)
+
+        # check cascade member-slot existence on nostream node
+        self.assertEqual(
+            cluster._get_members_slots(nostream_node.name, 'replica'),
+            {'test_3': {'type': 'physical'}})
+
+        # cascade also does not entitled to have logical slot on itself ...
+        self.p.name = cascade_node.name
+        self.assertEqual(
+            cluster._get_permanent_slots(self.p, cascade_node, 'replica'),
+            {'bar': {'type': 'physical'}})
+        # ... and member-slot on primary
+        self.assertEqual(
+            cluster.get_slot_name_on_primary(self.p.name, cascade_node),
+            None)
+
+        # simple replica must have every permanent slot ...
+        self.p.name = stream_node.name
+        self.assertEqual(
+            cluster._get_permanent_slots(self.p, stream_node, 'replica'),
+            {'foo': {'type': 'logical', 'database': 'a', 'plugin': 'b'}, 'bar': {'type': 'physical'}})
+        # ... and member-slot on primary
+        self.assertEqual(
+            cluster.get_slot_name_on_primary(self.p.name, stream_node),
+            'test_4')
+
     @patch.object(Postgresql, 'is_primary', Mock(return_value=False))
     def test__ensure_logical_slots_replica(self):
         self.p.set_role('replica')
         self.cluster.slots['ls'] = 12346
         with patch.object(SlotsHandler, 'check_logical_slots_readiness', Mock(return_value=False)):
-            self.assertEqual(self.s.sync_replication_slots(self.cluster, False), [])
+            self.assertEqual(self.s.sync_replication_slots(self.cluster, self.tags), [])
         with patch.object(SlotsHandler, '_query', Mock(return_value=[('ls', 'logical', 499, 'b', 'a', 5, 100, 500)])), \
                 patch.object(MockCursor, 'execute', Mock(side_effect=psycopg.OperationalError)), \
                 patch.object(SlotsAdvanceThread, 'schedule', Mock(return_value=(True, ['ls']))), \
                 patch.object(psycopg.OperationalError, 'diag') as mock_diag:
             type(mock_diag).sqlstate = PropertyMock(return_value='58P01')
-            self.assertEqual(self.s.sync_replication_slots(self.cluster, False), ['ls'])
+            self.assertEqual(self.s.sync_replication_slots(self.cluster, self.tags), ['ls'])
         self.cluster.slots['ls'] = 'a'
-        self.assertEqual(self.s.sync_replication_slots(self.cluster, False), [])
+        self.assertEqual(self.s.sync_replication_slots(self.cluster, self.tags), [])
         self.cluster.config.data['slots']['ls']['database'] = 'b'
         self.cluster.slots['ls'] = '500'
         with patch.object(MockCursor, 'rowcount', PropertyMock(return_value=1), create=True):
-            self.assertEqual(self.s.sync_replication_slots(self.cluster, False), ['ls'])
+            self.assertEqual(self.s.sync_replication_slots(self.cluster, self.tags), ['ls'])
 
     def test_copy_logical_slots(self):
         self.cluster.config.data['slots']['ls']['database'] = 'b'
-        self.s.copy_logical_slots(self.cluster, ['ls'])
+        self.s.copy_logical_slots(self.cluster, self.tags, ['ls'])
         with patch.object(MockCursor, 'execute', Mock(side_effect=psycopg.OperationalError)):
-            self.s.copy_logical_slots(self.cluster, ['foo'])
+            self.s.copy_logical_slots(self.cluster, self.tags, ['foo'])
         with patch.object(Cluster, 'leader', PropertyMock(return_value=None)):
-            self.s.copy_logical_slots(self.cluster, ['foo'])
+            self.s.copy_logical_slots(self.cluster, self.tags, ['foo'])
 
     @patch.object(Postgresql, 'stop', Mock(return_value=True))
     @patch.object(Postgresql, 'start', Mock(return_value=True))
     @patch.object(Postgresql, 'is_primary', Mock(return_value=False))
     def test_check_logical_slots_readiness(self):
-        self.s.copy_logical_slots(self.cluster, ['ls'])
+        self.s.copy_logical_slots(self.cluster, self.tags, ['ls'])
         with patch.object(MockCursor, '__iter__', Mock(return_value=iter([('postgresql0', None)]))), \
                 patch.object(MockCursor, 'fetchall', Mock(side_effect=Exception)):
-            self.assertFalse(self.s.check_logical_slots_readiness(self.cluster, None))
+            self.assertFalse(self.s.check_logical_slots_readiness(self.cluster, self.tags))
         with patch.object(MockCursor, '__iter__', Mock(return_value=iter([('postgresql0', None)]))), \
                 patch.object(MockCursor, 'fetchall', Mock(return_value=[(False,)])):
-            self.assertFalse(self.s.check_logical_slots_readiness(self.cluster, None))
+            self.assertFalse(self.s.check_logical_slots_readiness(self.cluster, self.tags))
         with patch.object(MockCursor, '__iter__', Mock(return_value=iter([('ls', 100)]))):
-            self.s.check_logical_slots_readiness(self.cluster, None)
+            self.s.check_logical_slots_readiness(self.cluster, self.tags)
 
     @patch.object(Postgresql, 'stop', Mock(return_value=True))
     @patch.object(Postgresql, 'start', Mock(return_value=True))
     @patch.object(Postgresql, 'is_primary', Mock(return_value=False))
     def test_on_promote(self):
         self.s.schedule_advance_slots({'foo': {'bar': 100}})
-        self.s.copy_logical_slots(self.cluster, ['ls'])
+        self.s.copy_logical_slots(self.cluster, self.tags, ['ls'])
         self.s.on_promote()
 
     @unittest.skipIf(os.name == 'nt', "Windows not supported")
     @patch('os.open', Mock())
     @patch('os.close', Mock())
     @patch('os.fsync', Mock(side_effect=OSError))
     def test_fsync_dir(self):
@@ -185,16 +258,17 @@
             self.s._advance.sync_slots()
 
     @patch.object(Postgresql, 'is_primary', Mock(return_value=False))
     def test_advance_physical_slots(self):
         config = ClusterConfig(1, {'slots': {'blabla': {'type': 'physical'}, 'leader': None}}, 1)
         cluster = Cluster(True, config, self.leader, Status(0, {'blabla': 12346}),
                           [self.me, self.other, self.leadermem], None, SyncState.empty(), None, None)
-        self.s.sync_replication_slots(cluster, False)
+        global_config.update(cluster)
+        self.s.sync_replication_slots(cluster, self.tags)
         with patch.object(SlotsHandler, '_query', Mock(side_effect=[[('blabla', 'physical', 12345, None, None, None,
                                                                       None, None)], Exception])) as mock_query, \
                 patch('patroni.postgresql.slots.logger.error') as mock_error:
-            self.s.sync_replication_slots(cluster, False)
+            self.s.sync_replication_slots(cluster, self.tags)
             self.assertEqual(mock_query.call_args[0],
                              ("SELECT pg_catalog.pg_replication_slot_advance(%s, %s)", "blabla", '0/303A'))
             self.assertEqual(mock_error.call_args[0][0],
                              "Error while advancing replication slot %s to position '%s': %r")
```

### Comparing `patroni-3.2.2/tests/test_sync.py` & `patroni-3.3.0/tests/test_sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import os
 
-from mock import Mock, patch
+from mock import Mock, patch, PropertyMock
 
+from patroni import global_config
 from patroni.collections import CaseInsensitiveSet
-from patroni.config import GlobalConfig
 from patroni.dcs import Cluster, SyncState
 from patroni.postgresql import Postgresql
 
 from . import BaseTestPostgresql, psycopg_connect, mock_available_gucs
 
 
 @patch('subprocess.call', Mock(return_value=0))
 @patch('patroni.psycopg.connect', psycopg_connect)
 @patch.object(Postgresql, 'available_gucs', mock_available_gucs)
+@patch.object(global_config.__class__, 'is_synchronous_mode', PropertyMock(return_value=True))
 class TestSync(BaseTestPostgresql):
 
     @patch('subprocess.call', Mock(return_value=0))
     @patch('os.rename', Mock())
     @patch('patroni.postgresql.CallbackExecutor', Mock())
     @patch.object(Postgresql, 'get_major_version', Mock(return_value=140000))
     @patch.object(Postgresql, 'is_running', Mock(return_value=True))
     @patch.object(Postgresql, 'available_gucs', mock_available_gucs)
     def setUp(self):
         super(TestSync, self).setUp()
         self.p.config.write_postgresql_conf()
-        self.p._global_config = GlobalConfig({'synchronous_mode': True})
         self.s = self.p.sync_handler
 
     @patch.object(Postgresql, 'last_operation', Mock(return_value=1))
     def test_pick_sync_standby(self):
         cluster = Cluster(True, None, self.leader, 0, [self.me, self.other, self.leadermem], None,
                           SyncState(0, self.me.name, self.leadermem.name), None, None, None)
 
@@ -92,11 +92,10 @@
 
         mock_reload.reset_mock()
         self.s.set_synchronous_standby_names(CaseInsensitiveSet([]))
         mock_reload.assert_called()
         self.assertEqual(value_in_conf(), None)
 
         mock_reload.reset_mock()
-        self.p._global_config = GlobalConfig({'synchronous_mode': True})
         self.s.set_synchronous_standby_names(CaseInsensitiveSet('*'))
         mock_reload.assert_called()
         self.assertEqual(value_in_conf(), "synchronous_standby_names = '*'")
```

### Comparing `patroni-3.2.2/tests/test_utils.py` & `patroni-3.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_validator.py` & `patroni-3.3.0/tests/test_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,29 @@
 from patroni.dcs import dcs_modules
 from patroni.validator import schema, Directory, Schema
 
 available_dcs = [m.split(".")[-1] for m in dcs_modules()]
 config = {
     "name": "string",
     "scope": "string",
+    "log": {
+        "type": "plain",
+        "level": "DEBUG",
+        "traceback_level": "DEBUG",
+        "format": "%(asctime)s %(levelname)s: %(message)s",
+        "dateformat": "%Y-%m-%d %H:%M:%S",
+        "max_queue_size": 100,
+        "dir": "/tmp",
+        "file_num": 10,
+        "file_size": 1000000,
+        "loggers": {
+            "patroni.postmaster": "WARNING",
+            "urllib3": "DEBUG"
+        }
+    },
     "restapi": {
         "listen": "127.0.0.2:800",
         "connect_address": "127.0.0.2:800",
         "verify_client": 'none'
     },
     "bootstrap": {
         "dcs": {
@@ -84,15 +99,16 @@
         "mode": "off",
         "device": "string"
     },
     "tags": {
         "nofailover": False,
         "clonefrom": False,
         "noloadbalance": False,
-        "nosync": False
+        "nosync": False,
+        "nostream": False
     }
 }
 
 config_2 = {
     "some_dir": "very_interesting_dir"
 }
 
@@ -353,7 +369,33 @@
         errors = schema(c)
         self.assertIn('tags.failover_priority a string is not an integer', errors)
         c = copy.deepcopy(config)
         del c["tags"]["nofailover"]
         c["tags"]["failover_priority"] = -6
         errors = schema(c)
         self.assertIn('tags.failover_priority -6 didn\'t pass validation: Wrong value', errors)
+
+    def test_json_log_format(self, *args):
+        c = copy.deepcopy(config)
+        c["log"]["type"] = "json"
+        c["log"]["format"] = {"levelname": "level"}
+        errors = schema(c)
+        self.assertIn("log.format {'levelname': 'level'} didn't pass validation: Should be a string or a list", errors)
+
+        c["log"]["format"] = []
+        errors = schema(c)
+        self.assertIn("log.format [] didn't pass validation: should contain at least one item", errors)
+
+        c["log"]["format"] = [{"levelname": []}]
+        errors = schema(c)
+        self.assertIn("log.format [{'levelname': []}] didn't pass validation: "
+                      "each item should be a string or a dictionary with string values", errors)
+
+        c["log"]["format"] = [[]]
+        errors = schema(c)
+        self.assertIn("log.format [[]] didn't pass validation: "
+                      "each item should be a string or a dictionary with string values", errors)
+
+        c["log"]["format"] = ['foo']
+        errors = schema(c)
+        output = "\n".join(errors)
+        self.assertEqual(['postgresql.bin_dir', 'raft.bind_addr', 'raft.self_addr'], parse_output(output))
```

### Comparing `patroni-3.2.2/tests/test_wale_restore.py` & `patroni-3.3.0/tests/test_wale_restore.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_watchdog.py` & `patroni-3.3.0/tests/test_watchdog.py`

 * *Files identical despite different names*

### Comparing `patroni-3.2.2/tests/test_zookeeper.py` & `patroni-3.3.0/tests/test_zookeeper.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 from kazoo.client import KazooClient
 from kazoo.exceptions import NoNodeError, NodeExistsError
 from kazoo.handlers.threading import SequentialThreadingHandler
 from kazoo.protocol.states import KeeperState, WatchedEvent, ZnodeStat
 from kazoo.retry import RetryFailedError
 from mock import Mock, PropertyMock, patch
+from patroni.dcs import get_dcs
 from patroni.dcs.zookeeper import Cluster, PatroniKazooClient, \
     PatroniSequentialThreadingHandler, ZooKeeper, ZooKeeperError
+from patroni.postgresql.mpp import get_mpp
 
 
 class MockKazooClient(Mock):
 
     handler = PatroniSequentialThreadingHandler(10)
     leader = False
     exists = True
@@ -144,54 +146,71 @@
         self.assertFalse(c._call(None, Mock()))
 
 
 class TestZooKeeper(unittest.TestCase):
 
     @patch('patroni.dcs.zookeeper.PatroniKazooClient', MockKazooClient)
     def setUp(self):
-        self.zk = ZooKeeper({'hosts': ['localhost:2181'], 'scope': 'test',
-                             'name': 'foo', 'ttl': 30, 'retry_timeout': 10, 'loop_wait': 10,
-                             'set_acls': {'CN=principal2': ['ALL']}})
+        self.zk = get_dcs({'scope': 'test', 'name': 'foo', 'ttl': 30, 'retry_timeout': 10, 'loop_wait': 10,
+                           'zookeeper': {'hosts': ['localhost:2181'], 'set_acls': {'CN=principal2': ['ALL']}}})
+        self.assertIsInstance(self.zk, ZooKeeper)
 
     def test_reload_config(self):
         self.zk.reload_config({'ttl': 20, 'retry_timeout': 10, 'loop_wait': 10})
         self.zk.reload_config({'ttl': 20, 'retry_timeout': 10, 'loop_wait': 5})
 
     def test_get_node(self):
         self.assertIsNone(self.zk.get_node('/no_node'))
 
     def test_get_children(self):
         self.assertListEqual(self.zk.get_children('/no_node'), [])
 
     def test__cluster_loader(self):
         self.zk._base_path = self.zk._base_path.replace('test', 'bla')
-        self.zk._cluster_loader(self.zk.client_path(''))
+        self.zk._postgresql_cluster_loader(self.zk.client_path(''))
         self.zk._base_path = self.zk._base_path = '/broken'
-        self.zk._cluster_loader(self.zk.client_path(''))
+        self.zk._postgresql_cluster_loader(self.zk.client_path(''))
         self.zk._base_path = self.zk._base_path = '/legacy'
-        self.zk._cluster_loader(self.zk.client_path(''))
+        self.zk._postgresql_cluster_loader(self.zk.client_path(''))
         self.zk._base_path = self.zk._base_path = '/no_node'
-        self.zk._cluster_loader(self.zk.client_path(''))
+        self.zk._postgresql_cluster_loader(self.zk.client_path(''))
 
     def test_get_cluster(self):
         cluster = self.zk.get_cluster()
         self.assertEqual(cluster.last_lsn, 500)
 
     def test__get_citus_cluster(self):
-        self.zk._citus_group = '0'
+        self.zk._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
         for _ in range(0, 2):
             cluster = self.zk.get_cluster()
             self.assertIsInstance(cluster, Cluster)
             self.assertIsInstance(cluster.workers[1], Cluster)
 
-    @patch('patroni.dcs.zookeeper.logger.error')
-    @patch.object(ZooKeeper, '_cluster_loader', Mock(side_effect=Exception))
+    @patch('patroni.dcs.logger.error')
+    def test_get_mpp_coordinator(self, mock_logger):
+        self.assertIsInstance(self.zk.get_mpp_coordinator(), Cluster)
+        with patch.object(ZooKeeper, '_postgresql_cluster_loader', Mock(side_effect=Exception)):
+            self.assertIsNone(self.zk.get_mpp_coordinator())
+            mock_logger.assert_called_once()
+            self.assertEqual(mock_logger.call_args[0][0], 'Failed to load %s coordinator cluster from %s: %r')
+            self.assertEqual(mock_logger.call_args[0][1], 'Null')
+            self.assertEqual(mock_logger.call_args[0][2], 'ZooKeeper')
+            self.assertIsInstance(mock_logger.call_args[0][3], ZooKeeperError)
+
+    @patch('patroni.dcs.logger.error')
     def test_get_citus_coordinator(self, mock_logger):
-        self.assertIsNone(self.zk.get_citus_coordinator())
-        mock_logger.assert_called_once()
+        self.zk._mpp = get_mpp({'citus': {'group': 0, 'database': 'postgres'}})
+        self.assertIsInstance(self.zk.get_mpp_coordinator(), Cluster)
+        with patch.object(ZooKeeper, '_postgresql_cluster_loader', Mock(side_effect=Exception)):
+            self.assertIsNone(self.zk.get_mpp_coordinator())
+            mock_logger.assert_called_once()
+            self.assertEqual(mock_logger.call_args[0][0], 'Failed to load %s coordinator cluster from %s: %r')
+            self.assertEqual(mock_logger.call_args[0][1], 'Citus')
+            self.assertEqual(mock_logger.call_args[0][2], 'ZooKeeper')
+            self.assertIsInstance(mock_logger.call_args[0][3], ZooKeeperError)
 
     def test_delete_leader(self):
         self.assertTrue(self.zk.delete_leader(self.zk.get_cluster().leader))
 
     def test_set_failover_value(self):
         self.zk.set_failover_value('')
         self.zk.set_failover_value('ok')
```

