# Comparing `tmp/rpcclient-4.5.1.tar.gz` & `tmp/rpcclient-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-4.5.1.tar", last modified: Mon Apr  1 08:18:24 2024, max compression
+gzip compressed data, was "rpcclient-4.6.0.tar", last modified: Thu Apr  4 06:08:05 2024, max compression
```

## Comparing `rpcclient-4.5.1.tar` & `rpcclient-4.6.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.765927 rpcclient-4.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-01 08:18:10.000000 rpcclient-4.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-01 08:18:10.000000 rpcclient-4.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-01 08:18:10.000000 rpcclient-4.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-01 08:18:24.761927 rpcclient-4.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 08:18:10.000000 rpcclient-4.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-01 08:18:10.000000 rpcclient-4.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-01 08:18:10.000000 rpcclient-4.5.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.749927 rpcclient-4.5.1/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 08:18:24.000000 rpcclient-4.5.1/rpcclient/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.757927 rpcclient-4.5.1/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    42645 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    44292 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    30236 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.757927 rpcclient-4.5.1/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/amfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.757927 rpcclient-4.5.1/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.757927 rpcclient-4.5.1/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/processes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.757927 rpcclient-4.5.1/rpcclient/protos/
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-01 08:18:15.000000 rpcclient-4.5.1/rpcclient/protos/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-04-01 08:18:15.000000 rpcclient-4.5.1/rpcclient/protos/rpc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/protosocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.761927 rpcclient-4.5.1/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (127)    25827 2024-04-01 08:18:10.000000 rpcclient-4.5.1/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.761927 rpcclient-4.5.1/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-01 08:18:24.000000 rpcclient-4.5.1/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-01 08:18:24.000000 rpcclient-4.5.1/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 08:18:24.000000 rpcclient-4.5.1/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 08:18:24.000000 rpcclient-4.5.1/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-01 08:18:24.000000 rpcclient-4.5.1/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 08:18:24.000000 rpcclient-4.5.1/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 08:18:24.765927 rpcclient-4.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:18:24.761927 rpcclient-4.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_allocation_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_core_foundation_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_darwin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_objc_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_spawn.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_thread_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_worker_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-01 08:18:10.000000 rpcclient-4.5.1/tests/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.354661 rpcclient-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-04 06:07:41.000000 rpcclient-4.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-04 06:07:41.000000 rpcclient-4.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 06:07:41.000000 rpcclient-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-04 06:08:05.350661 rpcclient-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 06:07:41.000000 rpcclient-4.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-04 06:07:41.000000 rpcclient-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 06:07:41.000000 rpcclient-4.6.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.338661 rpcclient-4.6.0/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42645 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44670 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30236 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/processes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.346661 rpcclient-4.6.0/rpcclient/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-04 06:07:52.000000 rpcclient-4.6.0/rpcclient/protos/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30372 2024-04-04 06:07:52.000000 rpcclient-4.6.0/rpcclient/protos/rpc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/protosocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.350661 rpcclient-4.6.0/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25827 2024-04-04 06:07:41.000000 rpcclient-4.6.0/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.350661 rpcclient-4.6.0/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 06:08:05.000000 rpcclient-4.6.0/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 06:08:05.354661 rpcclient-4.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:08:05.350661 rpcclient-4.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_allocation_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_core_foundation_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_darwin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_objc_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_thread_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_worker_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 06:07:41.000000 rpcclient-4.6.0/tests/test_xpc.py
```

### Comparing `rpcclient-4.5.1/CODE_OF_CONDUCT.md` & `rpcclient-4.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/LICENSE` & `rpcclient-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/PKG-INFO` & `rpcclient-4.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 4.5.1
+Version: 4.6.0
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 License: GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
 Project-URL: Homepage, https://github.com/doronz88/rpc-project
 Project-URL: Bug Reports, https://github.com/doronz88/rpc-project/issues
 Keywords: ios,macos,linux,automation,remote-shell,remote-control,ipython
```

### Comparing `rpcclient-4.5.1/pyproject.toml` & `rpcclient-4.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/__main__.py` & `rpcclient-4.6.0/rpcclient/__main__.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/client.py` & `rpcclient-4.6.0/rpcclient/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/client_factory.py` & `rpcclient-4.6.0/rpcclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/bluetooth.py` & `rpcclient-4.6.0/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/cfpreferences.py` & `rpcclient-4.6.0/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/client.py` & `rpcclient-4.6.0/rpcclient/darwin/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/consts.py` & `rpcclient-4.6.0/rpcclient/darwin/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/core_graphics.py` & `rpcclient-4.6.0/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/crash_reports.py` & `rpcclient-4.6.0/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/darwin_lief.py` & `rpcclient-4.6.0/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/fs.py` & `rpcclient-4.6.0/rpcclient/darwin/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/hid.py` & `rpcclient-4.6.0/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/ioregistry.py` & `rpcclient-4.6.0/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/keychain.py` & `rpcclient-4.6.0/rpcclient/darwin/keychain.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/location.py` & `rpcclient-4.6.0/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/media.py` & `rpcclient-4.6.0/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/network.py` & `rpcclient-4.6.0/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/objc.py` & `rpcclient-4.6.0/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/objective_c_class.py` & `rpcclient-4.6.0/rpcclient/darwin/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-4.6.0/rpcclient/darwin/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/power.py` & `rpcclient-4.6.0/rpcclient/darwin/power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/processes.py` & `rpcclient-4.6.0/rpcclient/darwin/processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 _CF_STRING_ARRAY_SUFFIX_LEN = len('",')
 _BACKTRACE_FRAME_REGEX = re.compile(r'\[\s*(\d+)\] (0x[0-9a-f]+)\s+\{(.+?) \+ (.+?)\} (.*)')
 
 FdStruct = namedtuple('FdStruct', 'fd struct')
 
 logger = logging.getLogger(__name__)
 
+CDHASH_SIZE = 20
 CHUNK_SIZE = 1024 * 64
 APP_SUFFIX = '.app/'
 
 
 @dataclasses.dataclass()
 class Fd:
     fd: int
@@ -728,14 +729,22 @@
                 region_detail = line[i]
 
             result.append(Region(region_type=region_type, start=self.get_process_symbol(start), end=end, vsize=vsize,
                                  protection=protection[0], protection_max=protection[1], region_detail=region_detail))
 
         return result
 
+    @property
+    def cdhash(self) -> bytes:
+        with self._client.safe_malloc(CDHASH_SIZE) as cdhash:
+            # by reversing online-auth-agent
+            if 0 != self._client.symbols.csops(self.pid, 5, cdhash, CDHASH_SIZE):
+                raise BadReturnValueError(f'failed to get cdhash for {self.pid}')
+            return cdhash.peek(CDHASH_SIZE)
+
     def get_process_symbol(self, address: int) -> ProcessSymbol:
         return ProcessSymbol.create(address, self._client, self)
 
     def vm_allocate(self, size: int) -> ProcessSymbol:
         with self._client.safe_malloc(8) as out_address:
             if self._client.symbols.vm_allocate(self.task, out_address, size, VM_FLAGS_ANYWHERE):
                 raise BadReturnValueError('vm_allocate() failed')
```

### Comparing `rpcclient-4.5.1/rpcclient/darwin/reports.py` & `rpcclient-4.6.0/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/scpreferences.py` & `rpcclient-4.6.0/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/structs.py` & `rpcclient-4.6.0/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/symbol.py` & `rpcclient-4.6.0/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/syslog.py` & `rpcclient-4.6.0/rpcclient/darwin/syslog.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/time.py` & `rpcclient-4.6.0/rpcclient/darwin/time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/darwin/xpc.py` & `rpcclient-4.6.0/rpcclient/darwin/xpc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/exceptions.py` & `rpcclient-4.6.0/rpcclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/fs.py` & `rpcclient-4.6.0/rpcclient/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/accessibility.py` & `rpcclient-4.6.0/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/amfi.py` & `rpcclient-4.6.0/rpcclient/ios/amfi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/backlight.py` & `rpcclient-4.6.0/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/client.py` & `rpcclient-4.6.0/rpcclient/ios/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/lockdown.py` & `rpcclient-4.6.0/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/mobile_gestalt.py` & `rpcclient-4.6.0/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/processes.py` & `rpcclient-4.6.0/rpcclient/ios/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/screen_capture.py` & `rpcclient-4.6.0/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/sprinboard.py` & `rpcclient-4.6.0/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/telephony.py` & `rpcclient-4.6.0/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/ios/wifi.py` & `rpcclient-4.6.0/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/lief.py` & `rpcclient-4.6.0/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/linux/client.py` & `rpcclient-4.6.0/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/linux/structs.py` & `rpcclient-4.6.0/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/macos/apple_script.py` & `rpcclient-4.6.0/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/macos/client.py` & `rpcclient-4.6.0/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/network.py` & `rpcclient-4.6.0/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/processes.py` & `rpcclient-4.6.0/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/protos/rpc_pb2.py` & `rpcclient-4.6.0/rpcclient/protos/rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/protos/rpc_pb2.pyi` & `rpcclient-4.6.0/rpcclient/protos/rpc_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import sys
@@ -29,15 +30,15 @@
 
 class Arch(_Arch, metaclass=_ArchEnumTypeWrapper): ...
 
 ARCH_UNKNOWN: Arch.ValueType  # 0
 ARCH_ARM64: Arch.ValueType  # 1
 global___Arch = Arch
 
-@typing_extensions.final
+@typing.final
 class Command(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAGIC_FIELD_NUMBER: builtins.int
     EXEC_FIELD_NUMBER: builtins.int
     DLOPEN_FIELD_NUMBER: builtins.int
     DLCLOSE_FIELD_NUMBER: builtins.int
@@ -100,21 +101,21 @@
         show_class: global___CmdShowClass | None = ...,
         dummy_block: global___CmdDummyBlock | None = ...,
         close: global___CmdClose | None = ...,
         class_list: global___CmdGetClassList | None = ...,
         exec_chunk: global___CmdExecChunk | None = ...,
         custom: global___CmdCustom | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["call", b"call", "class_list", b"class_list", "close", b"close", "custom", b"custom", "dlclose", b"dlclose", "dlopen", b"dlopen", "dlsym", b"dlsym", "dummy_block", b"dummy_block", "exec", b"exec", "exec_chunk", b"exec_chunk", "list_dir", b"list_dir", "peek", b"peek", "poke", b"poke", "show_class", b"show_class", "show_object", b"show_object", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["call", b"call", "class_list", b"class_list", "close", b"close", "custom", b"custom", "dlclose", b"dlclose", "dlopen", b"dlopen", "dlsym", b"dlsym", "dummy_block", b"dummy_block", "exec", b"exec", "exec_chunk", b"exec_chunk", "list_dir", b"list_dir", "magic", b"magic", "peek", b"peek", "poke", b"poke", "show_class", b"show_class", "show_object", b"show_object", "type", b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["exec", "dlopen", "dlclose", "dlsym", "call", "peek", "poke", "list_dir", "show_object", "show_class", "dummy_block", "close", "class_list", "exec_chunk", "custom"] | None: ...
+    def HasField(self, field_name: typing.Literal["call", b"call", "class_list", b"class_list", "close", b"close", "custom", b"custom", "dlclose", b"dlclose", "dlopen", b"dlopen", "dlsym", b"dlsym", "dummy_block", b"dummy_block", "exec", b"exec", "exec_chunk", b"exec_chunk", "list_dir", b"list_dir", "peek", b"peek", "poke", b"poke", "show_class", b"show_class", "show_object", b"show_object", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["call", b"call", "class_list", b"class_list", "close", b"close", "custom", b"custom", "dlclose", b"dlclose", "dlopen", b"dlopen", "dlsym", b"dlsym", "dummy_block", b"dummy_block", "exec", b"exec", "exec_chunk", b"exec_chunk", "list_dir", b"list_dir", "magic", b"magic", "peek", b"peek", "poke", b"poke", "show_class", b"show_class", "show_object", b"show_object", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["type", b"type"]) -> typing.Literal["exec", "dlopen", "dlclose", "dlsym", "call", "peek", "poke", "list_dir", "show_object", "show_class", "dummy_block", "close", "class_list", "exec_chunk", "custom"] | None: ...
 
 global___Command = Command
 
-@typing_extensions.final
+@typing.final
 class Response(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXEC_FIELD_NUMBER: builtins.int
     EXEC_CHUNK_FIELD_NUMBER: builtins.int
     DLOPEN_FIELD_NUMBER: builtins.int
     DLCLOSE_FIELD_NUMBER: builtins.int
@@ -174,21 +175,21 @@
         dummy_block: global___ResponseDummyBlock | None = ...,
         show_object: global___ResponseShowObject | None = ...,
         class_list: global___ResponseGetClassList | None = ...,
         show_class: global___ResponseShowClass | None = ...,
         list_dir: global___ResponseListdir | None = ...,
         custom: global___ResponseCustom | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["call", b"call", "class_list", b"class_list", "custom", b"custom", "dlclose", b"dlclose", "dlopen", b"dlopen", "dlsym", b"dlsym", "dummy_block", b"dummy_block", "error", b"error", "exec", b"exec", "exec_chunk", b"exec_chunk", "list_dir", b"list_dir", "peek", b"peek", "poke", b"poke", "show_class", b"show_class", "show_object", b"show_object", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["call", b"call", "class_list", b"class_list", "custom", b"custom", "dlclose", b"dlclose", "dlopen", b"dlopen", "dlsym", b"dlsym", "dummy_block", b"dummy_block", "error", b"error", "exec", b"exec", "exec_chunk", b"exec_chunk", "list_dir", b"list_dir", "peek", b"peek", "poke", b"poke", "show_class", b"show_class", "show_object", b"show_object", "type", b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["exec", "exec_chunk", "dlopen", "dlclose", "dlsym", "peek", "poke", "call", "error", "dummy_block", "show_object", "class_list", "show_class", "list_dir", "custom"] | None: ...
+    def HasField(self, field_name: typing.Literal["call", b"call", "class_list", b"class_list", "custom", b"custom", "dlclose", b"dlclose", "dlopen", b"dlopen", "dlsym", b"dlsym", "dummy_block", b"dummy_block", "error", b"error", "exec", b"exec", "exec_chunk", b"exec_chunk", "list_dir", b"list_dir", "peek", b"peek", "poke", b"poke", "show_class", b"show_class", "show_object", b"show_object", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["call", b"call", "class_list", b"class_list", "custom", b"custom", "dlclose", b"dlclose", "dlopen", b"dlopen", "dlsym", b"dlsym", "dummy_block", b"dummy_block", "error", b"error", "exec", b"exec", "exec_chunk", b"exec_chunk", "list_dir", b"list_dir", "peek", b"peek", "poke", b"poke", "show_class", b"show_class", "show_object", b"show_object", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["type", b"type"]) -> typing.Literal["exec", "exec_chunk", "dlopen", "dlclose", "dlsym", "peek", "poke", "call", "error", "dummy_block", "show_object", "class_list", "show_class", "list_dir", "custom"] | None: ...
 
 global___Response = Response
 
-@typing_extensions.final
+@typing.final
 class ReturnRegistersArm(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     X0_FIELD_NUMBER: builtins.int
     X1_FIELD_NUMBER: builtins.int
     X2_FIELD_NUMBER: builtins.int
     X3_FIELD_NUMBER: builtins.int
@@ -236,19 +237,19 @@
         d2: builtins.float = ...,
         d3: builtins.float = ...,
         d4: builtins.float = ...,
         d5: builtins.float = ...,
         d6: builtins.float = ...,
         d7: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["d0", b"d0", "d1", b"d1", "d2", b"d2", "d3", b"d3", "d4", b"d4", "d5", b"d5", "d6", b"d6", "d7", b"d7", "x0", b"x0", "x1", b"x1", "x2", b"x2", "x3", b"x3", "x4", b"x4", "x5", b"x5", "x6", b"x6", "x7", b"x7"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["d0", b"d0", "d1", b"d1", "d2", b"d2", "d3", b"d3", "d4", b"d4", "d5", b"d5", "d6", b"d6", "d7", b"d7", "x0", b"x0", "x1", b"x1", "x2", b"x2", "x3", b"x3", "x4", b"x4", "x5", b"x5", "x6", b"x6", "x7", b"x7"]) -> None: ...
 
 global___ReturnRegistersArm = ReturnRegistersArm
 
-@typing_extensions.final
+@typing.final
 class Argument(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     V_INT_FIELD_NUMBER: builtins.int
     V_DOUBLE_FIELD_NUMBER: builtins.int
     V_STR_FIELD_NUMBER: builtins.int
     V_BYTES_FIELD_NUMBER: builtins.int
@@ -260,21 +261,21 @@
         self,
         *,
         v_int: builtins.int = ...,
         v_double: builtins.float = ...,
         v_str: builtins.str = ...,
         v_bytes: builtins.bytes = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["type", b"type", "v_bytes", b"v_bytes", "v_double", b"v_double", "v_int", b"v_int", "v_str", b"v_str"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["type", b"type", "v_bytes", b"v_bytes", "v_double", b"v_double", "v_int", b"v_int", "v_str", b"v_str"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["v_int", "v_double", "v_str", "v_bytes"] | None: ...
+    def HasField(self, field_name: typing.Literal["type", b"type", "v_bytes", b"v_bytes", "v_double", b"v_double", "v_int", b"v_int", "v_str", b"v_str"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["type", b"type", "v_bytes", b"v_bytes", "v_double", b"v_double", "v_int", b"v_int", "v_str", b"v_str"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["type", b"type"]) -> typing.Literal["v_int", "v_double", "v_str", "v_bytes"] | None: ...
 
 global___Argument = Argument
 
-@typing_extensions.final
+@typing.final
 class Handshake(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAGIC_FIELD_NUMBER: builtins.int
     ARCH_FIELD_NUMBER: builtins.int
     SYSNAME_FIELD_NUMBER: builtins.int
     MACHINE_FIELD_NUMBER: builtins.int
@@ -286,228 +287,228 @@
         self,
         *,
         magic: builtins.int = ...,
         arch: global___Arch.ValueType = ...,
         sysname: builtins.str = ...,
         machine: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["arch", b"arch", "machine", b"machine", "magic", b"magic", "sysname", b"sysname"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["arch", b"arch", "machine", b"machine", "magic", b"magic", "sysname", b"sysname"]) -> None: ...
 
 global___Handshake = Handshake
 
-@typing_extensions.final
+@typing.final
 class ObjcClass(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     address: builtins.int
     name: builtins.str
     def __init__(
         self,
         *,
         address: builtins.int = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["address", b"address", "name", b"name"]) -> None: ...
 
 global___ObjcClass = ObjcClass
 
-@typing_extensions.final
+@typing.final
 class CmdShowObject(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     address: builtins.int
     def __init__(
         self,
         *,
         address: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["address", b"address"]) -> None: ...
 
 global___CmdShowObject = CmdShowObject
 
-@typing_extensions.final
+@typing.final
 class ResponseShowObject(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DESCRIPTION_FIELD_NUMBER: builtins.int
     description: builtins.str
     def __init__(
         self,
         *,
         description: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description", b"description"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["description", b"description"]) -> None: ...
 
 global___ResponseShowObject = ResponseShowObject
 
-@typing_extensions.final
+@typing.final
 class CmdShowClass(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     address: builtins.int
     def __init__(
         self,
         *,
         address: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["address", b"address"]) -> None: ...
 
 global___CmdShowClass = CmdShowClass
 
-@typing_extensions.final
+@typing.final
 class ResponseShowClass(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DESCRIPTION_FIELD_NUMBER: builtins.int
     description: builtins.str
     def __init__(
         self,
         *,
         description: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description", b"description"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["description", b"description"]) -> None: ...
 
 global___ResponseShowClass = ResponseShowClass
 
-@typing_extensions.final
+@typing.final
 class CmdExecChunk(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BUFFER_FIELD_NUMBER: builtins.int
     buffer: builtins.bytes
     def __init__(
         self,
         *,
         buffer: builtins.bytes = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["buffer", b"buffer"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["buffer", b"buffer"]) -> None: ...
 
 global___CmdExecChunk = CmdExecChunk
 
-@typing_extensions.final
+@typing.final
 class ResponseCmdExecChunk(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BUFFER_FIELD_NUMBER: builtins.int
     EXIT_CODE_FIELD_NUMBER: builtins.int
     buffer: builtins.bytes
     exit_code: builtins.int
     def __init__(
         self,
         *,
         buffer: builtins.bytes = ...,
         exit_code: builtins.int = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["buffer", b"buffer", "exit_code", b"exit_code", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["buffer", b"buffer", "exit_code", b"exit_code", "type", b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["buffer", "exit_code"] | None: ...
+    def HasField(self, field_name: typing.Literal["buffer", b"buffer", "exit_code", b"exit_code", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["buffer", b"buffer", "exit_code", b"exit_code", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["type", b"type"]) -> typing.Literal["buffer", "exit_code"] | None: ...
 
 global___ResponseCmdExecChunk = ResponseCmdExecChunk
 
-@typing_extensions.final
+@typing.final
 class CmdDlopen(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FILENAME_FIELD_NUMBER: builtins.int
     MODE_FIELD_NUMBER: builtins.int
     filename: builtins.str
     mode: builtins.int
     def __init__(
         self,
         *,
         filename: builtins.str = ...,
         mode: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["filename", b"filename", "mode", b"mode"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["filename", b"filename", "mode", b"mode"]) -> None: ...
 
 global___CmdDlopen = CmdDlopen
 
-@typing_extensions.final
+@typing.final
 class ResponseDlopen(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HANDLE_FIELD_NUMBER: builtins.int
     handle: builtins.int
     def __init__(
         self,
         *,
         handle: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["handle", b"handle"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["handle", b"handle"]) -> None: ...
 
 global___ResponseDlopen = ResponseDlopen
 
-@typing_extensions.final
+@typing.final
 class CmdDlclose(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HANDLE_FIELD_NUMBER: builtins.int
     handle: builtins.int
     def __init__(
         self,
         *,
         handle: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["handle", b"handle"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["handle", b"handle"]) -> None: ...
 
 global___CmdDlclose = CmdDlclose
 
-@typing_extensions.final
+@typing.final
 class ResponseDlclose(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RES_FIELD_NUMBER: builtins.int
     res: builtins.int
     def __init__(
         self,
         *,
         res: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["res", b"res"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["res", b"res"]) -> None: ...
 
 global___ResponseDlclose = ResponseDlclose
 
-@typing_extensions.final
+@typing.final
 class CmdDlsym(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HANDLE_FIELD_NUMBER: builtins.int
     SYMBOL_NAME_FIELD_NUMBER: builtins.int
     handle: builtins.int
     symbol_name: builtins.str
     def __init__(
         self,
         *,
         handle: builtins.int = ...,
         symbol_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["handle", b"handle", "symbol_name", b"symbol_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["handle", b"handle", "symbol_name", b"symbol_name"]) -> None: ...
 
 global___CmdDlsym = CmdDlsym
 
-@typing_extensions.final
+@typing.final
 class ResponseDlsym(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PTR_FIELD_NUMBER: builtins.int
     ptr: builtins.int
     def __init__(
         self,
         *,
         ptr: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ptr", b"ptr"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["ptr", b"ptr"]) -> None: ...
 
 global___ResponseDlsym = ResponseDlsym
 
-@typing_extensions.final
+@typing.final
 class CmdExec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BACKGROUND_FIELD_NUMBER: builtins.int
     ARGV_FIELD_NUMBER: builtins.int
     ENVP_FIELD_NUMBER: builtins.int
     background: builtins.bool
@@ -518,34 +519,34 @@
     def __init__(
         self,
         *,
         background: builtins.bool = ...,
         argv: collections.abc.Iterable[builtins.str] | None = ...,
         envp: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["argv", b"argv", "background", b"background", "envp", b"envp"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["argv", b"argv", "background", b"background", "envp", b"envp"]) -> None: ...
 
 global___CmdExec = CmdExec
 
-@typing_extensions.final
+@typing.final
 class ResponseCmdExec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PID_FIELD_NUMBER: builtins.int
     pid: builtins.int
     def __init__(
         self,
         *,
         pid: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pid", b"pid"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pid", b"pid"]) -> None: ...
 
 global___ResponseCmdExec = ResponseCmdExec
 
-@typing_extensions.final
+@typing.final
 class CmdCall(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     VA_LIST_INDEX_FIELD_NUMBER: builtins.int
     ARGV_FIELD_NUMBER: builtins.int
     address: builtins.int
@@ -555,180 +556,180 @@
     def __init__(
         self,
         *,
         address: builtins.int = ...,
         va_list_index: builtins.int = ...,
         argv: collections.abc.Iterable[global___Argument] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "argv", b"argv", "va_list_index", b"va_list_index"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["address", b"address", "argv", b"argv", "va_list_index", b"va_list_index"]) -> None: ...
 
 global___CmdCall = CmdCall
 
-@typing_extensions.final
+@typing.final
 class ResponseCall(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ARM_REGISTERS_FIELD_NUMBER: builtins.int
     RETURN_VALUE_FIELD_NUMBER: builtins.int
+    return_value: builtins.int
     @property
     def arm_registers(self) -> global___ReturnRegistersArm: ...
-    return_value: builtins.int
     def __init__(
         self,
         *,
         arm_registers: global___ReturnRegistersArm | None = ...,
         return_value: builtins.int = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["arm_registers", b"arm_registers", "return_value", b"return_value", "return_values", b"return_values"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["arm_registers", b"arm_registers", "return_value", b"return_value", "return_values", b"return_values"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["return_values", b"return_values"]) -> typing_extensions.Literal["arm_registers", "return_value"] | None: ...
+    def HasField(self, field_name: typing.Literal["arm_registers", b"arm_registers", "return_value", b"return_value", "return_values", b"return_values"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["arm_registers", b"arm_registers", "return_value", b"return_value", "return_values", b"return_values"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["return_values", b"return_values"]) -> typing.Literal["arm_registers", "return_value"] | None: ...
 
 global___ResponseCall = ResponseCall
 
-@typing_extensions.final
+@typing.final
 class CmdPeek(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     address: builtins.int
     size: builtins.int
     def __init__(
         self,
         *,
         address: builtins.int = ...,
         size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "size", b"size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["address", b"address", "size", b"size"]) -> None: ...
 
 global___CmdPeek = CmdPeek
 
-@typing_extensions.final
+@typing.final
 class ResponsePeek(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     data: builtins.bytes
     def __init__(
         self,
         *,
         data: builtins.bytes = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["data", b"data"]) -> None: ...
 
 global___ResponsePeek = ResponsePeek
 
-@typing_extensions.final
+@typing.final
 class CmdPoke(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     address: builtins.int
     data: builtins.bytes
     def __init__(
         self,
         *,
         address: builtins.int = ...,
         data: builtins.bytes = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "data", b"data"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["address", b"address", "data", b"data"]) -> None: ...
 
 global___CmdPoke = CmdPoke
 
-@typing_extensions.final
+@typing.final
 class ResponsePoke(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ResponsePoke = ResponsePoke
 
-@typing_extensions.final
+@typing.final
 class CmdListDir(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PATH_FIELD_NUMBER: builtins.int
     path: builtins.str
     def __init__(
         self,
         *,
         path: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["path", b"path"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["path", b"path"]) -> None: ...
 
 global___CmdListDir = CmdListDir
 
-@typing_extensions.final
+@typing.final
 class CmdDummyBlock(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___CmdDummyBlock = CmdDummyBlock
 
-@typing_extensions.final
+@typing.final
 class ResponseDummyBlock(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     address: builtins.int
     size: builtins.int
     def __init__(
         self,
         *,
         address: builtins.int = ...,
         size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "size", b"size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["address", b"address", "size", b"size"]) -> None: ...
 
 global___ResponseDummyBlock = ResponseDummyBlock
 
-@typing_extensions.final
+@typing.final
 class CmdGetClassList(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___CmdGetClassList = CmdGetClassList
 
-@typing_extensions.final
+@typing.final
 class ResponseGetClassList(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CLASSES_FIELD_NUMBER: builtins.int
     @property
     def classes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ObjcClass]: ...
     def __init__(
         self,
         *,
         classes: collections.abc.Iterable[global___ObjcClass] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["classes", b"classes"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["classes", b"classes"]) -> None: ...
 
 global___ResponseGetClassList = ResponseGetClassList
 
-@typing_extensions.final
+@typing.final
 class ResponseError(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ResponseError = ResponseError
 
-@typing_extensions.final
+@typing.final
 class ResponseListdir(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAGIC_FIELD_NUMBER: builtins.int
     DIRP_FIELD_NUMBER: builtins.int
     DIR_ENTRIES_FIELD_NUMBER: builtins.int
     magic: builtins.int
@@ -738,19 +739,19 @@
     def __init__(
         self,
         *,
         magic: builtins.int = ...,
         dirp: builtins.int = ...,
         dir_entries: collections.abc.Iterable[global___DirEntry] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dir_entries", b"dir_entries", "dirp", b"dirp", "magic", b"magic"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dir_entries", b"dir_entries", "dirp", b"dirp", "magic", b"magic"]) -> None: ...
 
 global___ResponseListdir = ResponseListdir
 
-@typing_extensions.final
+@typing.final
 class DirEntry(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     D_TYPE_FIELD_NUMBER: builtins.int
     D_NAME_FIELD_NUMBER: builtins.int
     LSTAT_FIELD_NUMBER: builtins.int
     STAT_FIELD_NUMBER: builtins.int
@@ -764,20 +765,20 @@
         self,
         *,
         d_type: builtins.int = ...,
         d_name: builtins.str = ...,
         lstat: global___DirEntryStat | None = ...,
         stat: global___DirEntryStat | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["lstat", b"lstat", "stat", b"stat"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["d_name", b"d_name", "d_type", b"d_type", "lstat", b"lstat", "stat", b"stat"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["lstat", b"lstat", "stat", b"stat"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["d_name", b"d_name", "d_type", b"d_type", "lstat", b"lstat", "stat", b"stat"]) -> None: ...
 
 global___DirEntry = DirEntry
 
-@typing_extensions.final
+@typing.final
 class DirEntryStat(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ERRNO1_FIELD_NUMBER: builtins.int
     ST_DEV_FIELD_NUMBER: builtins.int
     ST_MODE_FIELD_NUMBER: builtins.int
     ST_NLINK_FIELD_NUMBER: builtins.int
@@ -819,50 +820,50 @@
         st_size: builtins.int = ...,
         st_blocks: builtins.int = ...,
         st_blksize: builtins.int = ...,
         st_atime1: builtins.int = ...,
         st_mtime1: builtins.int = ...,
         st_ctime1: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["errno1", b"errno1", "st_atime1", b"st_atime1", "st_blksize", b"st_blksize", "st_blocks", b"st_blocks", "st_ctime1", b"st_ctime1", "st_dev", b"st_dev", "st_gid", b"st_gid", "st_ino", b"st_ino", "st_mode", b"st_mode", "st_mtime1", b"st_mtime1", "st_nlink", b"st_nlink", "st_rdev", b"st_rdev", "st_size", b"st_size", "st_uid", b"st_uid"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["errno1", b"errno1", "st_atime1", b"st_atime1", "st_blksize", b"st_blksize", "st_blocks", b"st_blocks", "st_ctime1", b"st_ctime1", "st_dev", b"st_dev", "st_gid", b"st_gid", "st_ino", b"st_ino", "st_mode", b"st_mode", "st_mtime1", b"st_mtime1", "st_nlink", b"st_nlink", "st_rdev", b"st_rdev", "st_size", b"st_size", "st_uid", b"st_uid"]) -> None: ...
 
 global___DirEntryStat = DirEntryStat
 
-@typing_extensions.final
+@typing.final
 class CmdClose(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___CmdClose = CmdClose
 
-@typing_extensions.final
+@typing.final
 class CmdCustom(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONTENT_FIELD_NUMBER: builtins.int
     content: builtins.bytes
     def __init__(
         self,
         *,
         content: builtins.bytes = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["content", b"content"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["content", b"content"]) -> None: ...
 
 global___CmdCustom = CmdCustom
 
-@typing_extensions.final
+@typing.final
 class ResponseCustom(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONTENT_FIELD_NUMBER: builtins.int
     content: builtins.bytes
     def __init__(
         self,
         *,
         content: builtins.bytes = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["content", b"content"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["content", b"content"]) -> None: ...
 
 global___ResponseCustom = ResponseCustom
```

### Comparing `rpcclient-4.5.1/rpcclient/protosocket.py` & `rpcclient-4.6.0/rpcclient/protosocket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/structs/consts.py` & `rpcclient-4.6.0/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/structs/generic.py` & `rpcclient-4.6.0/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/symbol.py` & `rpcclient-4.6.0/rpcclient/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/symbols_jar.py` & `rpcclient-4.6.0/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/sysctl.py` & `rpcclient-4.6.0/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient/xonshrc.py` & `rpcclient-4.6.0/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/rpcclient.egg-info/PKG-INFO` & `rpcclient-4.6.0/rpcclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 4.5.1
+Version: 4.6.0
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanelc305 <netanelc305@pm.me>
 License: GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007
 Project-URL: Homepage, https://github.com/doronz88/rpc-project
 Project-URL: Bug Reports, https://github.com/doronz88/rpc-project/issues
 Keywords: ios,macos,linux,automation,remote-shell,remote-control,ipython
```

### Comparing `rpcclient-4.5.1/rpcclient.egg-info/SOURCES.txt` & `rpcclient-4.6.0/rpcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/conftest.py` & `rpcclient-4.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_allocation_cleanup.py` & `rpcclient-4.6.0/tests/test_allocation_cleanup.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_client.py` & `rpcclient-4.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_darwin_client.py` & `rpcclient-4.6.0/tests/test_darwin_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_fs.py` & `rpcclient-4.6.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_objc_symbol.py` & `rpcclient-4.6.0/tests/test_objc_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_power.py` & `rpcclient-4.6.0/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_preferences.py` & `rpcclient-4.6.0/tests/test_preferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_processes.py` & `rpcclient-4.6.0/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_socket.py` & `rpcclient-4.6.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_spawn.py` & `rpcclient-4.6.0/tests/test_spawn.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_thread_safe.py` & `rpcclient-4.6.0/tests/test_thread_safe.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_time.py` & `rpcclient-4.6.0/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-4.5.1/tests/test_xpc.py` & `rpcclient-4.6.0/tests/test_xpc.py`

 * *Files identical despite different names*

