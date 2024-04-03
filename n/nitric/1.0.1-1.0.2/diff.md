# Comparing `tmp/nitric-1.0.1.tar.gz` & `tmp/nitric-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitric-1.0.1.tar", last modified: Tue Mar 26 22:09:45 2024, max compression
+gzip compressed data, was "nitric-1.0.2.tar", last modified: Wed Apr  3 23:01:30 2024, max compression
```

## Comparing `nitric-1.0.1.tar` & `nitric-1.0.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.417105 nitric-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-03-26 22:09:45.417105 nitric-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-26 22:09:03.000000 nitric-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.409105 nitric-1.0.1/nitric/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/bidi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.409105 nitric-1.0.1/nitric/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.409105 nitric-1.0.1/nitric/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.409105 nitric-1.0.1/nitric/proto/KeyValue/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/KeyValue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.409105 nitric-1.0.1/nitric/proto/KeyValue/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/KeyValue/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.409105 nitric-1.0.1/nitric/proto/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/apis/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/apis/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/deployments/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/deployments/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/http/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/http/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/http/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/kvstore/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/kvstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/kvstore/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/kvstore/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/queues/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/queues/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/queues/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/resources/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/resources/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/schedules/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/schedules/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/secrets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/secrets/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/storage/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/storage/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/topics/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/topics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/topics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/topics/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/websockets/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/websockets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.413105 nitric-1.0.1/nitric/proto/websockets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/proto/websockets/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:03.000000 nitric-1.0.1/nitric/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.417105 nitric-1.0.1/nitric/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20208 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/kv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/resources/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-26 22:09:39.000000 nitric-1.0.1/nitric/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:09:45.409105 nitric-1.0.1/nitric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-03-26 22:09:45.000000 nitric-1.0.1/nitric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-26 22:09:45.000000 nitric-1.0.1/nitric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:09:45.000000 nitric-1.0.1/nitric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-26 22:09:45.000000 nitric-1.0.1/nitric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 22:09:45.000000 nitric-1.0.1/nitric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-26 22:09:03.000000 nitric-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 22:09:45.417105 nitric-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-26 22:09:03.000000 nitric-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.455870 nitric-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-03 23:01:30.455870 nitric-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 23:00:51.000000 nitric-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.447870 nitric-1.0.2/nitric/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/bidi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.447870 nitric-1.0.2/nitric/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/KeyValue/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/KeyValue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/KeyValue/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/KeyValue/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/apis/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/apis/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/deployments/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/deployments/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/http/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/http/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/kvstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/kvstore/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/kvstore/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/queues/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/queues/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/queues/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/resources/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/resources/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/schedules/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/schedules/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/secrets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/secrets/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/storage/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/storage/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/topics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/topics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/topics/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/websockets/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/websockets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/websockets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/websockets/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:00:51.000000 nitric-1.0.2/nitric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.455870 nitric-1.0.2/nitric/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/kv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.447870 nitric-1.0.2/nitric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 23:00:51.000000 nitric-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:01:30.455870 nitric-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-03 23:00:51.000000 nitric-1.0.2/setup.py
```

### Comparing `nitric-1.0.1/PKG-INFO` & `nitric-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 1.0.1 Summary: The Nitric SDK for
+Metadata-Version: 2.1 Name: nitric Version: 1.0.2 Summary: The Nitric SDK for
 Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
 Description-Content-Type: text/markdown Provides-Extra: dev
                                  _[_N_i_t_r_i_c_ _L_o_g_o_]
                ********** BBuuiilldd _nn_ii_tt_rr_ii_cc aapppplliiccaattiioonnss wwiitthh PPyytthhoonn **********
            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_/_w_e_e_k_]_[_D_i_s_c_o_r_d_]
```

### Comparing `nitric-1.0.1/README.md` & `nitric-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/__init__.py` & `nitric-1.0.2/nitric/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/application.py` & `nitric-1.0.2/nitric/application.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/bidi.py` & `nitric-1.0.2/nitric/bidi.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/config/__init__.py` & `nitric-1.0.2/nitric/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/context.py` & `nitric-1.0.2/nitric/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,17 +435,17 @@
                 output_context = await cur(result, acc_next)  # type: ignore
                 if not output_context:
                     return result  # type: ignore
                 return output_context  # type: ignore
 
             return chained_middleware
 
-        middleware_chain = functools.reduce(reduce_chain, reversed(middlewares))  # type: ignore
+        middleware_chain = functools.reduce(reduce_chain, reversed(middlewares), last_middleware)  # type: ignore
         # type ignored because mypy appears to misidentify the correct return type
-        return await middleware_chain(ctx, last_middleware)  # type: ignore
+        return await middleware_chain(ctx)  # type: ignore
 
     return composed
 
 
 class FunctionServer(ABC):
     """Represents a worker that should be started at runtime."""
```

### Comparing `nitric-1.0.1/nitric/exception.py` & `nitric-1.0.2/nitric/exception.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/KeyValue/__init__.py` & `nitric-1.0.2/nitric/proto/KeyValue/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/KeyValue/v1/__init__.py` & `nitric-1.0.2/nitric/proto/KeyValue/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/__init__.py` & `nitric-1.0.2/nitric/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/apis/__init__.py` & `nitric-1.0.2/nitric/proto/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/apis/v1/__init__.py` & `nitric-1.0.2/nitric/proto/apis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/deployments/__init__.py` & `nitric-1.0.2/nitric/proto/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/deployments/v1/__init__.py` & `nitric-1.0.2/nitric/proto/deployments/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/http/__init__.py` & `nitric-1.0.2/nitric/proto/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/http/v1/__init__.py` & `nitric-1.0.2/nitric/proto/http/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/kvstore/__init__.py` & `nitric-1.0.2/nitric/proto/kvstore/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/kvstore/v1/__init__.py` & `nitric-1.0.2/nitric/proto/kvstore/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/queues/__init__.py` & `nitric-1.0.2/nitric/proto/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/queues/v1/__init__.py` & `nitric-1.0.2/nitric/proto/queues/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/resources/__init__.py` & `nitric-1.0.2/nitric/proto/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/resources/v1/__init__.py` & `nitric-1.0.2/nitric/proto/resources/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/schedules/__init__.py` & `nitric-1.0.2/nitric/proto/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/schedules/v1/__init__.py` & `nitric-1.0.2/nitric/proto/schedules/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/secrets/__init__.py` & `nitric-1.0.2/nitric/proto/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/secrets/v1/__init__.py` & `nitric-1.0.2/nitric/proto/secrets/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/storage/__init__.py` & `nitric-1.0.2/nitric/proto/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/storage/v1/__init__.py` & `nitric-1.0.2/nitric/proto/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/topics/__init__.py` & `nitric-1.0.2/nitric/proto/topics/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/topics/v1/__init__.py` & `nitric-1.0.2/nitric/proto/topics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/websockets/__init__.py` & `nitric-1.0.2/nitric/proto/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/proto/websockets/v1/__init__.py` & `nitric-1.0.2/nitric/proto/websockets/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/__init__.py` & `nitric-1.0.2/nitric/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/apis.py` & `nitric-1.0.2/nitric/resources/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,17 @@
             raise exception_from_grpc_error(grpc_err) from grpc_err
 
     def _route(self, match: str, opts: Optional[RouteOptions] = None) -> Route:
         """Define an HTTP route to be handled by this API."""
         if opts is None:
             opts = RouteOptions()
 
+        if self.middleware is not None:
+            opts.middleware = self.middleware + opts.middleware
+
         r = Route(self, match, opts)
         self.routes.append(r)
         return r
 
     def all(self, match: str, opts: Optional[MethodOptions] = None) -> Callable[[HttpHandler], None]:
         """Define an HTTP route which will respond to HTTP GET requests."""
 
@@ -335,14 +338,21 @@
         self.path = (api.path + path).replace("//", "/")
         self.middleware = opts.middleware if opts.middleware is not None else []
 
     def method(
         self, methods: List[HttpMethod], *middleware: HttpMiddleware | HttpHandler, opts: Optional[MethodOptions] = None
     ) -> None:
         """Register middleware for multiple HTTP Methods."""
+
+        # ensure route/api middlewares are added
+        middleware = (
+            *self.middleware,
+            *middleware
+        )
+
         Method(self, methods, *middleware, opts=opts if opts else MethodOptions())
 
     def get(self, *middleware: HttpMiddleware | HttpHandler, opts: Optional[MethodOptions] = None) -> None:
         """Register middleware for HTTP GET requests."""
         return self.method([HttpMethod.GET], *middleware, opts=opts)
 
     def post(self, *middleware: HttpMiddleware | HttpHandler, opts: Optional[MethodOptions] = None) -> None:
```

### Comparing `nitric-1.0.1/nitric/resources/buckets.py` & `nitric-1.0.2/nitric/resources/buckets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/kv.py` & `nitric-1.0.2/nitric/resources/kv.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/queues.py` & `nitric-1.0.2/nitric/resources/queues.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/resource.py` & `nitric-1.0.2/nitric/resources/resource.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/schedules.py` & `nitric-1.0.2/nitric/resources/schedules.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/secrets.py` & `nitric-1.0.2/nitric/resources/secrets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/topics.py` & `nitric-1.0.2/nitric/resources/topics.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/resources/websockets.py` & `nitric-1.0.2/nitric/resources/websockets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric/utils.py` & `nitric-1.0.2/nitric/utils.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/nitric.egg-info/PKG-INFO` & `nitric-1.0.2/nitric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 1.0.1 Summary: The Nitric SDK for
+Metadata-Version: 2.1 Name: nitric Version: 1.0.2 Summary: The Nitric SDK for
 Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
 Description-Content-Type: text/markdown Provides-Extra: dev
                                  _[_N_i_t_r_i_c_ _L_o_g_o_]
                ********** BBuuiilldd _nn_ii_tt_rr_ii_cc aapppplliiccaattiioonnss wwiitthh PPyytthhoonn **********
            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_/_w_e_e_k_]_[_D_i_s_c_o_r_d_]
```

### Comparing `nitric-1.0.1/nitric.egg-info/SOURCES.txt` & `nitric-1.0.2/nitric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitric-1.0.1/setup.py` & `nitric-1.0.2/setup.py`

 * *Files identical despite different names*

