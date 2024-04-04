# Comparing `tmp/systembridgemodels-4.0.4.dev0.tar.gz` & `tmp/systembridgemodels-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgemodels-4.0.4.dev0.tar", last modified: Sat Mar  9 13:42:51 2024, max compression
+gzip compressed data, was "systembridgemodels-4.1.0.tar", last modified: Thu Apr  4 00:59:19 2024, max compression
```

## Comparing `systembridgemodels-4.0.4.dev0.tar` & `systembridgemodels-4.1.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 13:42:51.990260 systembridgemodels-4.0.4.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-09 13:42:51.990260 systembridgemodels-4.0.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 13:42:51.990260 systembridgemodels-4.0.4.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 13:42:51.978260 systembridgemodels-4.0.4.dev0/systembridgemodels/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 13:42:51.978260 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/media_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 13:42:51.982260 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/media_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/media_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/media_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/media_play.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 13:42:51.982260 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/modules/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/open_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/open_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/systembridgemodels/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 13:42:51.990260 systembridgemodels-4.0.4.dev0/systembridgemodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-09 13:42:51.000000 systembridgemodels-4.0.4.dev0/systembridgemodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-03-09 13:42:51.000000 systembridgemodels-4.0.4.dev0/systembridgemodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 13:42:51.000000 systembridgemodels-4.0.4.dev0/systembridgemodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-09 13:42:51.000000 systembridgemodels-4.0.4.dev0/systembridgemodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-09 13:42:51.000000 systembridgemodels-4.0.4.dev0/systembridgemodels.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 13:42:51.986260 systembridgemodels-4.0.4.dev0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 13:42:51.986260 systembridgemodels-4.0.4.dev0/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_displays.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/modules/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_media_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_media_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_media_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_media_play.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_open_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_open_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-09 13:42:35.000000 systembridgemodels-4.0.4.dev0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.886464 systembridgemodels-4.1.0/systembridgemodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 00:59:17.000000 systembridgemodels-4.1.0/systembridgemodels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.886464 systembridgemodels-4.1.0/systembridgemodels/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/media_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.886464 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_play.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.890464 systembridgemodels-4.1.0/systembridgemodels/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/systembridgemodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_open_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_open_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_version.py
```

### Comparing `systembridgemodels-4.0.4.dev0/LICENSE` & `systembridgemodels-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/pyproject.toml` & `systembridgemodels-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/setup.py` & `systembridgemodels-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/const.py` & `systembridgemodels-4.1.0/systembridgemodels/const.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Model constants."""
-# Model
+
+from enum import StrEnum
+
 from .keyboard_key import KeyboardKey
 from .keyboard_text import KeyboardText
 from .media_directories import MediaDirectory
 from .media_files import MediaFile, MediaFiles
-from .modules import ModulesData
+from .modules import Module, ModulesData
 from .modules.battery import Battery
 from .modules.cpu import CPU
 from .modules.disks import Disks
 from .modules.displays import Display
 from .modules.gpus import GPU
 from .modules.media import Media
 from .modules.memory import Memory
@@ -17,55 +19,59 @@
 from .modules.sensors import Sensors
 from .modules.system import System
 from .notification import Notification
 from .open_path import OpenPath
 from .open_url import OpenUrl
 from .response import Response
 
-MODEL_BATTERY = "battery"
-MODEL_CPU = "cpu"
-MODEL_DATA = "data"
-MODEL_DISKS = "disks"
-MODEL_DISPLAYS = "displays"
-MODEL_GENERIC = "generic"
-MODEL_GPUS = "gpus"
-MODEL_KEYBOARD_KEY = "keyboard_key"
-MODEL_KEYBOARD_TEXT = "keyboard_text"
-MODEL_MEDIA = "media"
-MODEL_MEDIA_DIRECTORIES = "media_directories"
-MODEL_MEDIA_FILE = "media_file"
-MODEL_MEDIA_FILES = "media_files"
-MODEL_MEMORY = "memory"
-MODEL_NETWORKS = "networks"
-MODEL_NOTIFICATION = "notification"
-MODEL_OPEN_PATH = "open_path"
-MODEL_OPEN_URL = "open_url"
-MODEL_PROCESSES = "processes"
-MODEL_RESPONSE = "response"
-MODEL_SECRETS = "secrets"
-MODEL_SENSORS = "sensors"
-MODEL_SETTINGS = "settings"
-MODEL_SYSTEM = "system"
+
+class Model(StrEnum):
+    """Model Enums."""
+
+    BATTERY = Module.BATTERY
+    CPU = Module.CPU
+    DATA = "data"
+    DISKS = Module.DISKS
+    DISPLAYS = Module.DISPLAYS
+    GPUS = Module.GPUS
+    KEYBOARD_KEY = "keyboard_key"
+    KEYBOARD_TEXT = "keyboard_text"
+    MEDIA = Module.MEDIA
+    MEDIA_DIRECTORIES = "media_directories"
+    MEDIA_FILE = "media_file"
+    MEDIA_FILES = "media_files"
+    MEMORY = Module.MEMORY
+    NETWORKS = Module.NETWORKS
+    NOTIFICATION = "notification"
+    OPEN_PATH = "open_path"
+    OPEN_URL = "open_url"
+    PROCESSES = Module.PROCESSES
+    RESPONSE = "response"
+    SECRETS = "secrets"
+    SENSORS = Module.SENSORS
+    SETTINGS = "settings"
+    SYSTEM = Module.SYSTEM
+
 
 MODEL_MAP = {
-    MODEL_BATTERY: Battery,
-    MODEL_CPU: CPU,
-    MODEL_DATA: ModulesData,
-    MODEL_DISKS: Disks,
-    MODEL_DISPLAYS: Display, # Map to Display not list[Display] so it can be mapped
-    MODEL_GPUS: GPU, # Map to GPU not list[GPU] so it can be mapped
-    MODEL_KEYBOARD_KEY: KeyboardKey,
-    MODEL_KEYBOARD_TEXT: KeyboardText,
-    MODEL_MEDIA_DIRECTORIES: MediaDirectory, # Map to MediaDirectory not list[MediaDirectory] so it can be mapped
-    MODEL_MEDIA_FILE: MediaFile,
-    MODEL_MEDIA_FILES: MediaFiles,
-    MODEL_MEDIA: Media,
-    MODEL_MEMORY: Memory,
-    MODEL_NETWORKS: Networks,
-    MODEL_NOTIFICATION: Notification,
-    MODEL_OPEN_PATH: OpenPath,
-    MODEL_OPEN_URL: OpenUrl,
-    MODEL_PROCESSES: Process, # Map to Process not list[Process] so it can be mapped
-    MODEL_RESPONSE: Response,
-    MODEL_SENSORS: Sensors,
-    MODEL_SYSTEM: System,
+    Model.BATTERY: Battery,
+    Model.CPU: CPU,
+    Model.DATA: ModulesData,
+    Model.DISKS: Disks,
+    Model.DISPLAYS: Display,  # Map to Display not list[Display] so it can be mapped
+    Model.GPUS: GPU,  # Map to GPU not list[GPU] so it can be mapped
+    Model.KEYBOARD_KEY: KeyboardKey,
+    Model.KEYBOARD_TEXT: KeyboardText,
+    Model.MEDIA_DIRECTORIES: MediaDirectory,  # Map to MediaDirectory not list[MediaDirectory] so it can be mapped
+    Model.MEDIA_FILE: MediaFile,
+    Model.MEDIA_FILES: MediaFiles,
+    Model.MEDIA: Media,
+    Model.MEMORY: Memory,
+    Model.NETWORKS: Networks,
+    Model.NOTIFICATION: Notification,
+    Model.OPEN_PATH: OpenPath,
+    Model.OPEN_URL: OpenUrl,
+    Model.PROCESSES: Process,  # Map to Process not list[Process] so it can be mapped
+    Model.RESPONSE: Response,
+    Model.SENSORS: Sensors,
+    Model.SYSTEM: System,
 }
```

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/media_files.py` & `systembridgemodels-4.1.0/systembridgemodels/fixtures/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/cpu.py` & `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/disks.py` & `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/media.py` & `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/memory.py` & `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/networks.py` & `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/sensors.py` & `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/fixtures/modules/system.py` & `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/system.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/media_control.py` & `systembridgemodels-4.1.0/systembridgemodels/media_control.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/media_files.py` & `systembridgemodels-4.1.0/systembridgemodels/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/__init__.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 """Modules."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
-from enum import Enum
+from enum import StrEnum
 
 from .battery import Battery
 from .cpu import CPU
 from .disks import Disks
 from .displays import Display
 from .gpus import GPU
 from .media import Media
 from .memory import Memory
 from .networks import Networks
 from .processes import Process
 from .sensors import Sensors
 from .system import System
 
 
-class DataEnum(Enum):
-    """Data Enum."""
+class Module(StrEnum):
+    """Module Enum."""
 
     BATTERY = "battery"
     CPU = "cpu"
     DISKS = "disks"
     DISPLAYS = "displays"
     GPUS = "gpus"
     MEDIA = "media"
     MEMORY = "memory"
     NETWORKS = "networks"
     PROCESSES = "processes"
-    SENSORS = "sensor"
+    SENSORS = "sensors"
     SYSTEM = "system"
 
 
 @dataclass
 class GetData:
     """Get Data."""
 
-    modules: list[str]
+    modules: list[Module]
 
 
 @dataclass
 class RegisterDataListener(GetData):
     """Register Data Listener."""
```

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/cpu.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/disks.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/gpus.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/gpus.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/media.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/memory.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/networks.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/sensors.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/modules/system.py` & `systembridgemodels-4.1.0/systembridgemodels/modules/system.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/notification.py` & `systembridgemodels-4.1.0/systembridgemodels/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels/settings.py` & `systembridgemodels-4.1.0/systembridgemodels/settings.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/systembridgemodels.egg-info/SOURCES.txt` & `systembridgemodels-4.1.0/systembridgemodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_cpu.py` & `systembridgemodels-4.1.0/tests/modules/test_cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_disks.py` & `systembridgemodels-4.1.0/tests/modules/test_disks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_displays.py` & `systembridgemodels-4.1.0/tests/modules/test_displays.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_gpus.py` & `systembridgemodels-4.1.0/tests/modules/test_gpus.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_media.py` & `systembridgemodels-4.1.0/tests/modules/test_media.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_memory.py` & `systembridgemodels-4.1.0/tests/modules/test_memory.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_networks.py` & `systembridgemodels-4.1.0/tests/modules/test_networks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_processes.py` & `systembridgemodels-4.1.0/tests/modules/test_processes.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_sensors.py` & `systembridgemodels-4.1.0/tests/modules/test_sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/modules/test_system.py` & `systembridgemodels-4.1.0/tests/modules/test_system.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/test_media_files.py` & `systembridgemodels-4.1.0/tests/test_media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/test_media_play.py` & `systembridgemodels-4.1.0/tests/test_media_play.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/test_notification.py` & `systembridgemodels-4.1.0/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/test_response.py` & `systembridgemodels-4.1.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.0.4.dev0/tests/test_settings.py` & `systembridgemodels-4.1.0/tests/test_settings.py`

 * *Files identical despite different names*

