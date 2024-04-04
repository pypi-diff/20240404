# Comparing `tmp/openedx-events-9.6.0.tar.gz` & `tmp/openedx-events-9.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-9.6.0.tar", last modified: Mon Apr  1 12:59:12 2024, max compression
+gzip compressed data, was "openedx-events-9.7.0.tar", last modified: Thu Apr  4 17:57:41 2024, max compression
```

## Comparing `openedx-events-9.6.0.tar` & `openedx-events-9.7.0.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-04-01 12:59:09.000000 openedx-events-9.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 12:59:09.000000 openedx-events-9.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 12:59:09.000000 openedx-events-9.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17505 2024-04-01 12:59:12.792969 openedx-events-9.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-01 12:59:09.000000 openedx-events-9.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/analytics/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/analytics/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/management/commands/generate_avro_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_generate_avro_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_producer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17505 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 12:59:09.000000 openedx-events-9.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-01 12:59:09.000000 openedx-events-9.6.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-01 12:59:12.796969 openedx-events-9.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-01 12:59:09.000000 openedx-events-9.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-01 12:59:09.000000 openedx-events-9.6.0/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.064874 openedx-events-9.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-04 17:57:34.000000 openedx-events-9.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 17:57:34.000000 openedx-events-9.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-04 17:57:34.000000 openedx-events-9.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17697 2024-04-04 17:57:41.064874 openedx-events-9.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-04 17:57:34.000000 openedx-events-9.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/analytics/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/analytics/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/enterprise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/enterprise/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/enterprise/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/management/commands/generate_avro_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_generate_avro_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_producer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17697 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 17:57:34.000000 openedx-events-9.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-04 17:57:34.000000 openedx-events-9.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-04 17:57:41.064874 openedx-events-9.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-04 17:57:34.000000 openedx-events-9.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 17:57:34.000000 openedx-events-9.7.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-9.6.0/CHANGELOG.rst` & `openedx-events-9.7.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,24 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[9.7.0] - 2024-04-04
+--------------------
+Added
+~~~~~~~
+* Added new ``SUBSIDY_REDEEMED`` and ``SUBSIDY_REDEMPTION_REVERSED`` events in enterprise.
+
+[9.6.0] - 2024-04-01
+--------------------
 Added
-~~~~~
+~~~~~~~
 * Added new ``CONTENT_OBJECT_TAGGED`` events in content_authoring.
 
 [9.5.2] - 2024-02-13
 --------------------
 Removed
 ~~~~~~~
 * Remove unused ``MANAGE_STUDENTS_PERMISSION_ADDED`` and ``MANAGE_STUDENTS_PERMISSION_REMOVED`` events in learning
```

### Comparing `openedx-events-9.6.0/LICENSE.txt` & `openedx-events-9.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/PKG-INFO` & `openedx-events-9.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 9.6.0
+Version: 9.7.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -163,16 +163,24 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[9.7.0] - 2024-04-04
+--------------------
+Added
+~~~~~~~
+* Added new ``SUBSIDY_REDEEMED`` and ``SUBSIDY_REDEMPTION_REVERSED`` events in enterprise.
+
+[9.6.0] - 2024-04-01
+--------------------
 Added
-~~~~~
+~~~~~~~
 * Added new ``CONTENT_OBJECT_TAGGED`` events in content_authoring.
 
 [9.5.2] - 2024-02-13
 --------------------
 Removed
 ~~~~~~~
 * Remove unused ``MANAGE_STUDENTS_PERMISSION_ADDED`` and ``MANAGE_STUDENTS_PERMISSION_REMOVED`` events in learning
```

### Comparing `openedx-events-9.6.0/README.rst` & `openedx-events-9.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/analytics/data.py` & `openedx-events-9.7.0/openedx_events/analytics/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/analytics/signals.py` & `openedx-events-9.7.0/openedx_events/analytics/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/apps.py` & `openedx-events-9.7.0/openedx_events/apps.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/content_authoring/data.py` & `openedx-events-9.7.0/openedx_events/content_authoring/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/content_authoring/signals.py` & `openedx-events-9.7.0/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/data.py` & `openedx-events-9.7.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/__init__.py` & `openedx-events-9.7.0/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/schema.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/serializer.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-9.7.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/exceptions.py` & `openedx-events-9.7.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/learning/data.py` & `openedx-events-9.7.0/openedx_events/learning/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/learning/signals.py` & `openedx-events-9.7.0/openedx_events/learning/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/management/commands/consume_events.py` & `openedx-events-9.7.0/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/management/commands/generate_avro_schemas.py` & `openedx-events-9.7.0/openedx_events/management/commands/generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/tests/test_consume_events_command.py` & `openedx-events-9.7.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/tests/test_data.py` & `openedx-events-9.7.0/openedx_events/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/tests/test_generate_avro_schemas.py` & `openedx-events-9.7.0/openedx_events/tests/test_generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/tests/test_producer_config.py` & `openedx-events-9.7.0/openedx_events/tests/test_producer_config.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/tests/test_tooling.py` & `openedx-events-9.7.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/tests/utils.py` & `openedx-events-9.7.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/tooling.py` & `openedx-events-9.7.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events/utils.py` & `openedx-events-9.7.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/openedx_events.egg-info/PKG-INFO` & `openedx-events-9.7.0/openedx_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 9.6.0
+Version: 9.7.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -163,16 +163,24 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[9.7.0] - 2024-04-04
+--------------------
+Added
+~~~~~~~
+* Added new ``SUBSIDY_REDEEMED`` and ``SUBSIDY_REDEMPTION_REVERSED`` events in enterprise.
+
+[9.6.0] - 2024-04-01
+--------------------
 Added
-~~~~~
+~~~~~~~
 * Added new ``CONTENT_OBJECT_TAGGED`` events in content_authoring.
 
 [9.5.2] - 2024-02-13
 --------------------
 Removed
 ~~~~~~~
 * Remove unused ``MANAGE_STUDENTS_PERMISSION_ADDED`` and ``MANAGE_STUDENTS_PERMISSION_REMOVED`` events in learning
```

### Comparing `openedx-events-9.6.0/openedx_events.egg-info/SOURCES.txt` & `openedx-events-9.7.0/openedx_events.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 openedx_events.egg-info/top_level.txt
 openedx_events/analytics/__init__.py
 openedx_events/analytics/data.py
 openedx_events/analytics/signals.py
 openedx_events/content_authoring/__init__.py
 openedx_events/content_authoring/data.py
 openedx_events/content_authoring/signals.py
+openedx_events/enterprise/__init__.py
+openedx_events/enterprise/data.py
+openedx_events/enterprise/signals.py
 openedx_events/event_bus/__init__.py
 openedx_events/event_bus/avro/__init__.py
 openedx_events/event_bus/avro/custom_serializers.py
 openedx_events/event_bus/avro/deserializer.py
 openedx_events/event_bus/avro/schema.py
 openedx_events/event_bus/avro/serializer.py
 openedx_events/event_bus/avro/types.py
```

### Comparing `openedx-events-9.6.0/requirements/constraints.txt` & `openedx-events-9.7.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-9.6.0/setup.py` & `openedx-events-9.7.0/setup.py`

 * *Files identical despite different names*

