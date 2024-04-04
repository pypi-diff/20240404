# Comparing `tmp/zinolib-1.0.2.tar.gz` & `tmp/zinolib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zinolib-1.0.2.tar", last modified: Fri Jan 26 14:02:35 2024, max compression
+gzip compressed data, was "zinolib-1.0.3.tar", last modified: Thu Apr  4 12:57:16 2024, max compression
```

## Comparing `zinolib-1.0.2.tar` & `zinolib-1.0.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/
--rw-rw-r--   0 hm        (1000) hm        (1000)      114 2023-08-23 12:45:06.000000 zinolib-1.0.2/.git-blame-ignore-revs
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/.github/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/.github/workflows/
--rw-rw-r--   0 hm        (1000) hm        (1000)     1654 2024-01-26 08:36:22.000000 zinolib-1.0.2/.github/workflows/linter.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)     1049 2023-10-17 13:10:05.000000 zinolib-1.0.2/.github/workflows/publish-test-results.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)     1406 2023-10-18 08:33:08.000000 zinolib-1.0.2/.github/workflows/test.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)      192 2023-10-20 08:50:16.000000 zinolib-1.0.2/.gitignore
--rw-rw-r--   0 hm        (1000) hm        (1000)      417 2023-08-23 12:43:58.000000 zinolib-1.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 hm        (1000) hm        (1000)    11358 2023-08-23 12:43:58.000000 zinolib-1.0.2/LICENSE
--rw-rw-r--   0 hm        (1000) hm        (1000)      484 2023-10-20 08:51:23.000000 zinolib-1.0.2/Makefile
--rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-01-26 14:02:35.991078 zinolib-1.0.2/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)      955 2023-08-23 12:45:06.000000 zinolib-1.0.2/README.rst
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/examples/
--rw-rw-r--   0 hm        (1000) hm        (1000)      771 2023-08-23 12:43:58.000000 zinolib-1.0.2/examples/auth.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2993 2023-08-15 12:56:17.000000 zinolib-1.0.2/examples/host_up_cleanup.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2598 2023-08-23 12:43:58.000000 zinolib-1.0.2/examples/monitor.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2261 2023-08-23 12:43:58.000000 zinolib-1.0.2/examples/pm-add.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1932 2023-08-23 12:43:58.000000 zinolib-1.0.2/examples/pm-test.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1930 2023-08-23 12:43:58.000000 zinolib-1.0.2/examples/pm-test2.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2199 2023-08-17 12:47:05.000000 zinolib-1.0.2/examples/reboot.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1902 2023-08-17 12:47:05.000000 zinolib-1.0.2/examples/schedule_reboot_host.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2465 2023-08-23 12:43:58.000000 zinolib-1.0.2/examples/test-with.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2576 2023-08-23 12:43:58.000000 zinolib-1.0.2/examples/test.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1172 2023-11-28 14:11:44.000000 zinolib-1.0.2/pyproject.toml
--rw-rw-r--   0 hm        (1000) hm        (1000)       38 2024-01-26 14:02:35.991078 zinolib-1.0.2/setup.cfg
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/src/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/src/zinolib/
--rw-rw-r--   0 hm        (1000) hm        (1000)     1146 2023-08-24 07:39:23.000000 zinolib-1.0.2/src/zinolib/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      689 2023-10-18 09:02:30.000000 zinolib-1.0.2/src/zinolib/compat.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/src/zinolib/config/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-10-18 09:02:30.000000 zinolib-1.0.2/src/zinolib/config/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      373 2023-11-28 14:11:44.000000 zinolib-1.0.2/src/zinolib/config/models.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3906 2023-10-27 11:56:57.000000 zinolib-1.0.2/src/zinolib/config/tcl.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      917 2023-10-27 11:56:57.000000 zinolib-1.0.2/src/zinolib/config/toml.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1346 2023-10-27 11:56:57.000000 zinolib-1.0.2/src/zinolib/config/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2545 2023-11-28 14:11:44.000000 zinolib-1.0.2/src/zinolib/config/zino1.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/src/zinolib/controllers/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-10-16 07:43:38.000000 zinolib-1.0.2/src/zinolib/controllers/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2009 2023-10-20 13:44:36.000000 zinolib-1.0.2/src/zinolib/controllers/base.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    16820 2024-01-26 11:57:32.000000 zinolib-1.0.2/src/zinolib/controllers/zino1.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     7072 2024-01-11 12:27:27.000000 zinolib-1.0.2/src/zinolib/event_types.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    38213 2024-01-26 11:57:32.000000 zinolib-1.0.2/src/zinolib/ritz.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2723 2024-01-26 08:36:22.000000 zinolib-1.0.2/src/zinolib/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      411 2024-01-26 14:02:35.000000 zinolib-1.0.2/src/zinolib/version.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4549 2023-08-23 12:45:06.000000 zinolib-1.0.2/src/zinolib/zino_emu.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/src/zinolib.egg-info/
--rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-01-26 14:02:35.000000 zinolib-1.0.2/src/zinolib.egg-info/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)     1401 2024-01-26 14:02:35.000000 zinolib-1.0.2/src/zinolib.egg-info/SOURCES.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-01-26 14:02:35.000000 zinolib-1.0.2/src/zinolib.egg-info/dependency_links.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2023-11-27 12:05:48.000000 zinolib-1.0.2/src/zinolib.egg-info/not-zip-safe
--rw-rw-r--   0 hm        (1000) hm        (1000)       48 2024-01-26 14:02:35.000000 zinolib-1.0.2/src/zinolib.egg-info/requires.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        8 2024-01-26 14:02:35.000000 zinolib-1.0.2/src/zinolib.egg-info/top_level.txt
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/tests/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-08-24 07:39:23.000000 zinolib-1.0.2/tests/__init__.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/tests/config/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-10-20 09:01:07.000000 zinolib-1.0.2/tests/config/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2840 2023-10-20 08:59:41.000000 zinolib-1.0.2/tests/config/test_tcl.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1664 2023-10-20 08:59:34.000000 zinolib-1.0.2/tests/config/test_toml.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1155 2023-10-20 09:00:43.000000 zinolib-1.0.2/tests/config/test_utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2280 2023-10-20 08:42:09.000000 zinolib-1.0.2/tests/config/test_zino1.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-01-26 14:02:35.991078 zinolib-1.0.2/tests/ritz/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-10-20 08:54:05.000000 zinolib-1.0.2/tests/ritz/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     7530 2023-10-20 08:55:32.000000 zinolib-1.0.2/tests/ritz/test_default.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1322 2023-10-20 08:55:42.000000 zinolib-1.0.2/tests/ritz/test_slow.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9275 2023-12-06 14:10:47.000000 zinolib-1.0.2/tests/test_zinolib_controllers_zino1.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9189 2023-10-20 13:44:36.000000 zinolib-1.0.2/tests/test_zinolib_event_types.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      390 2023-10-12 09:04:56.000000 zinolib-1.0.2/tests/test_zinolib_utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4082 2023-10-20 08:42:09.000000 zinolib-1.0.2/tests/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1573 2024-01-26 11:57:26.000000 zinolib-1.0.2/tox.ini
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.296699 zinolib-1.0.3/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      114 2023-08-23 12:45:06.000000 zinolib-1.0.3/.git-blame-ignore-revs
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.288699 zinolib-1.0.3/.github/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/.github/workflows/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1654 2024-03-18 06:51:15.000000 zinolib-1.0.3/.github/workflows/linter.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1049 2023-10-17 13:10:05.000000 zinolib-1.0.3/.github/workflows/publish-test-results.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1406 2024-03-18 06:51:15.000000 zinolib-1.0.3/.github/workflows/test.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)      192 2024-03-18 06:51:15.000000 zinolib-1.0.3/.gitignore
+-rw-rw-r--   0 hm        (1000) hm        (1000)      417 2023-08-23 12:43:58.000000 zinolib-1.0.3/.pre-commit-config.yaml
+-rw-rw-r--   0 hm        (1000) hm        (1000)    11358 2023-08-23 12:43:58.000000 zinolib-1.0.3/LICENSE
+-rw-rw-r--   0 hm        (1000) hm        (1000)      484 2024-03-18 06:51:15.000000 zinolib-1.0.3/Makefile
+-rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-04-04 12:57:16.292698 zinolib-1.0.3/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)      955 2023-08-23 12:45:06.000000 zinolib-1.0.3/README.rst
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/examples/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      771 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/auth.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2993 2023-08-15 12:56:17.000000 zinolib-1.0.3/examples/host_up_cleanup.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2598 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/monitor.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2261 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/pm-add.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1932 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/pm-test.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1930 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/pm-test2.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2199 2023-08-17 12:47:05.000000 zinolib-1.0.3/examples/reboot.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1902 2023-08-17 12:47:05.000000 zinolib-1.0.3/examples/schedule_reboot_host.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2465 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/test-with.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2576 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/test.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1172 2024-03-18 06:51:15.000000 zinolib-1.0.3/pyproject.toml
+-rw-rw-r--   0 hm        (1000) hm        (1000)       38 2024-04-04 12:57:16.296699 zinolib-1.0.3/setup.cfg
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.288699 zinolib-1.0.3/src/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/src/zinolib/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1146 2023-08-24 07:39:23.000000 zinolib-1.0.3/src/zinolib/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      689 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/compat.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/src/zinolib/config/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      373 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/models.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3906 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/tcl.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      917 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/toml.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1346 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2545 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/zino1.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/src/zinolib/controllers/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/controllers/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2015 2024-04-04 12:53:35.000000 zinolib-1.0.3/src/zinolib/controllers/base.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    19002 2024-04-04 12:53:52.000000 zinolib-1.0.3/src/zinolib/controllers/zino1.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7072 2024-03-20 09:16:53.000000 zinolib-1.0.3/src/zinolib/event_types.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    38357 2024-03-20 09:16:58.000000 zinolib-1.0.3/src/zinolib/ritz.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2723 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      411 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib/version.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4549 2023-08-23 12:45:06.000000 zinolib-1.0.3/src/zinolib/zino_emu.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/src/zinolib.egg-info/
+-rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1401 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/SOURCES.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/dependency_links.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2023-11-27 12:05:48.000000 zinolib-1.0.3/src/zinolib.egg-info/not-zip-safe
+-rw-rw-r--   0 hm        (1000) hm        (1000)       48 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/requires.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        8 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/top_level.txt
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/tests/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-08-24 07:39:23.000000 zinolib-1.0.3/tests/__init__.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/tests/config/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2840 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/test_tcl.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1664 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/test_toml.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1155 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/test_utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2280 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/test_zino1.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/tests/ritz/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/ritz/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7530 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/ritz/test_default.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1322 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/ritz/test_slow.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9314 2024-04-04 12:53:35.000000 zinolib-1.0.3/tests/test_zinolib_controllers_zino1.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9189 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/test_zinolib_event_types.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      390 2023-10-12 09:04:56.000000 zinolib-1.0.3/tests/test_zinolib_utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4082 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1573 2024-03-18 06:51:15.000000 zinolib-1.0.3/tox.ini
```

### Comparing `zinolib-1.0.2/.github/workflows/linter.yml` & `zinolib-1.0.3/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/.github/workflows/publish-test-results.yml` & `zinolib-1.0.3/.github/workflows/publish-test-results.yml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/.github/workflows/test.yml` & `zinolib-1.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/LICENSE` & `zinolib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/PKG-INFO` & `zinolib-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zinolib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python interface to Zino
 Author-email: Runar Borge <runar.borge@sikt.no>
 Maintainer-email: Uninett Opensource <opensource@uninett.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `zinolib-1.0.2/README.rst` & `zinolib-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/auth.py` & `zinolib-1.0.3/examples/auth.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/host_up_cleanup.py` & `zinolib-1.0.3/examples/host_up_cleanup.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/monitor.py` & `zinolib-1.0.3/examples/monitor.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/pm-add.py` & `zinolib-1.0.3/examples/pm-add.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/pm-test.py` & `zinolib-1.0.3/examples/pm-test.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/pm-test2.py` & `zinolib-1.0.3/examples/pm-test2.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/reboot.py` & `zinolib-1.0.3/examples/reboot.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/schedule_reboot_host.py` & `zinolib-1.0.3/examples/schedule_reboot_host.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/test-with.py` & `zinolib-1.0.3/examples/test-with.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/examples/test.py` & `zinolib-1.0.3/examples/test.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/pyproject.toml` & `zinolib-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/__init__.py` & `zinolib-1.0.3/src/zinolib/__init__.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/compat.py` & `zinolib-1.0.3/src/zinolib/compat.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/config/tcl.py` & `zinolib-1.0.3/src/zinolib/config/tcl.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/config/toml.py` & `zinolib-1.0.3/src/zinolib/config/toml.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/config/utils.py` & `zinolib-1.0.3/src/zinolib/config/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/config/zino1.py` & `zinolib-1.0.3/src/zinolib/config/zino1.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/controllers/base.py` & `zinolib-1.0.3/src/zinolib/controllers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         raise ValueError("Unknown type")
 
     def _set_event(self, event: Event):
         self.events[event.id] = event
 
     def remove_event(self, event_or_id: EventOrId):
         event_id = self._get_event_id(event_or_id)
-        self.events.pop(event_id)
+        self.events.pop(event_id, None)
         self.removed_ids.add(event_id)
 
     def _verify_session(self, quiet=False):
         if not self.session:
             if quiet:
                 return False
             raise ValueError  # raise correct error
```

### Comparing `zinolib-1.0.2/src/zinolib/controllers/zino1.py` & `zinolib-1.0.3/src/zinolib/controllers/zino1.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,22 @@
 To get a set of removed event ids::
 
     > event_manager.removed_ids
 
 For updates, either regularly use ``get_events()`` or utilize the UpdateHandler::
 
     > updater = UpdateHandler(event_manager)
-    > updated = updater.poll()
+    > updated = updater.get_event_update()
 
-``updater.poll()`` updates ``event_manager.events`` and
-``event_manager.removed_ids`` and returns ``True`` on any change, falsey
-otherwise.
+The updater is unique per authenticated user and is only available after login.
+
+``updater.get_event_update()`` updates ``event_manager.events`` and
+``event_manager.removed_ids`` and returns the id of a changed event on any
+change, falsey otherwise. Check the id against the removed_id's set to see if
+it has been removed from the server.
 
 To get history for a specific event::
 
     > history_list = event_manager.get_history_for_id(INT)
 
 To get the log for a specific event::
 
@@ -65,18 +68,17 @@
 The adapters are not meant to be used directly.
 """
 
 from datetime import datetime, timezone
 from typing import Dict, Iterable, List, TypedDict, Optional, Set
 import logging
 
-from .base import EventManager
+from .base import EventManager, EventOrId
 from ..compat import StrEnum
 from ..event_types import EventType, Event, HistoryEntry, LogEntry, AdmState
-from ..event_types import PortStateEvent
 from ..ritz import ZinoError, ProtocolError, ritz, notifier
 from ..utils import log_exception_with_params
 
 
 __all__ = [
     'Zino1EventManager',
 ]
@@ -131,59 +133,97 @@
             raise self.UpdateError(msg)
         self.manager = manager
         if not self.manager.session.push:
             self.manager.connect_push_channel()
         self.events = manager.events
         self.autoremove = autoremove
 
-    def poll(self):
+    def get_event_update(self):
+        """
+        Fetches one update for a single event and runs the appropriate handler
+
+        Attributes on the update object:
+
+        id: event id
+        type: update type, triggers the correct handler
+        info: a type-specific string with the actual change
+
+        Run in a loop/every N seconds for a lightweight way to update the event
+        list
+        """
         update = self.manager.session.push.poll()
         if not update:
             return False
-        return self.handle(update)
+        return self.handle_event_update(update)
 
     def update(self, event_id: int):
+        "Refresh an event from the server, refreshing everything"
         event = self.manager.get_updated_event_for_id(event_id)
         self.manager._set_event(event)
         LOG.debug("Updated event #%i", event_id)
 
     def remove(self, event_id: int):
+        "Remove an event from our local copy of the events list"
         self.manager.remove_event(event_id)
         LOG.debug("Removed event #%i", event_id)
 
-    def handle(self, update):
+    def handle_event_update(self, update):
+        """Call the right handle on the update object depending on type
+
+        If the update is about a locally unknown id and the update type is not
+        UpdateType.STATE it is a new, incomplete event so we return nothing.
+
+        Otherwise call the right handler on the update data.
+        """
         if update.id not in self.events and update.type != self.UpdateType.STATE:
-            # new event that still don't have a state
+            # unknown event that don't have a state (yet), wait for new update
             return None
         if update.type in tuple(self.UpdateType):
             method = getattr(self, f"cmd_{update.type}")
             return method(update)
         return self.fallback(update)
 
     def cmd_state(self, update):
+        """State has been changed
+
+        Removes a now closed state if the setting "autoremove" is True,
+        otherwise refreshes the event from the server.
+        """
         states = update.info.split(" ")
         if states[1] == "closed" and self.autoremove:
             LOG.debug('Autoremoving "%s"', update.id)
             self.remove(update.id)
         else:
             self.update(update.id)
-        return True
+        return update.id
 
     def cmd_attr(self, update):
+        """Attributes has been changed
+
+        Refresh the event from the server.
+        """
         self.update(update.id)
-        return True
+        return update.id
 
     cmd_history = cmd_attr
     cmd_log = cmd_attr
 
     def cmd_scavenged(self, update):
+        """The event has been removed from the server
+
+        Remove it from our local copy of the events list.
+        """
         self.remove(update.id)
-        return True
+        return update.id
 
     def fallback(self, update):
+        """There's an unknown update type
+
+        Log it and do nothing.
+        """
         LOG.warning('Unknown update type: "%s" for id %s' % (update.type, update.id))
         return False
 
 
 class SessionAdapter:
 
     class _Session:
@@ -298,14 +338,21 @@
     @staticmethod
     def get_event_ids(request):
         try:
             return request.get_caseids()
         except ProtocolError as e:
             raise RetryError('Zino 1 failed to send a correct response header, retry') from e
 
+    @staticmethod
+    def poll(request, event: EventType) -> bool:
+        if event.type == Event.Type.PORTSTATE:
+            return request.poll_interface(event.router, event.if_index)
+        else:
+            return request.poll_router(event.router)
+
 
 class HistoryAdapter:
     SYSTEM_USER = "monitor"
 
     @staticmethod
     def get_history(request, event_id: int):
         return request.get_raw_history(event_id).data
@@ -428,15 +475,15 @@
         return self.session.request.connected if session_ok else False
 
     def rename_exception(self, function, *args):
         "Replace the original exception with our own"
         try:
             return function(*args)
         except ZinoError as e:
-            raise self.ManagerException(e)
+            raise self.ManagerException(e) from e
 
     def _verify_session(self, quiet=False):
         if not getattr(self.session, 'request', None):
             if quiet:
                 return False
             raise ValueError
         return True
@@ -459,32 +506,42 @@
         except (ZinoError, ValueError) as e:
             raise self.ManagerException(e)
 
     def disconnect(self):
         self._verify_session()
         self.session = self._session_adapter.close_session(self.session)
 
-    def clear_flapping(self, event: PortStateEvent):
+    def clear_flapping(self, event_or_id: EventOrId):
         """Clear flapping state of a PortStateEvent
 
         Usage:
             c = ritz_session.case(123)
             c.clear_flapping()
         """
-        if event.type == Event.Type.PortState:
+        event = self._get_event(event_or_id)
+        if event.type == Event.Type.PORTSTATE:
             return self.session.request.clear_flapping(event.router, event.if_index)
         return None
 
+    def poll(self, event_or_id: EventOrId):
+        """Ask the server to refresh data for the event
+
+        If there are any changes they will be available through the update
+        handler in a bit
+        """
+        event = self._get_event(event_or_id)
+        return self._event_adapter.poll(self.session.request, event)
+
     def get_events(self):
         self._verify_session()
         for event_id in self._event_adapter.get_event_ids(self.session.request):
             try:
                 event = self.create_event_from_id(event_id)
             except self.ManagerException:
-                self.removed_ids.add(event_id)
+                self.remove_event(event_id)
                 continue
             self.events[event_id] = event
 
     def create_event_from_id(self, event_id: int):
         self._verify_session()
         attrlist = self.rename_exception(self._event_adapter.get_attrlist, self.session.request, event_id)
         if not self._event_adapter.validate_raw_attrlist(attrlist):
```

### Comparing `zinolib-1.0.2/src/zinolib/event_types.py` & `zinolib-1.0.3/src/zinolib/event_types.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/ritz.py` & `zinolib-1.0.3/src/zinolib/ritz.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,18 @@
         header: DataResponseHeader = ()
         r: List[str] = []
         logger.debug("send: %s" % command.__repr__())
         if command:
             delimiter = bytes(self.DELIMITER, 'ascii')
             if not command.endswith(delimiter):
                 command += delimiter
-            self._sock.send(command)
+            try:
+                self._sock.send(command)
+            except BrokenPipeError as e:
+                raise NotConnectedError(f'Lost connection to server: {e}') from e
         while data:
             try:
                 data = self._sock.recv(recv_buffer)
             except socket.timeout:
                 raise TimeoutError(
                     "Timed out waiting for data. command: %s buffer: %s"
                     % (repr(command), repr(buffer))
```

### Comparing `zinolib-1.0.2/src/zinolib/utils.py` & `zinolib-1.0.3/src/zinolib/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib/zino_emu.py` & `zinolib-1.0.3/src/zinolib/zino_emu.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/src/zinolib.egg-info/PKG-INFO` & `zinolib-1.0.3/src/zinolib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zinolib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python interface to Zino
 Author-email: Runar Borge <runar.borge@sikt.no>
 Maintainer-email: Uninett Opensource <opensource@uninett.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `zinolib-1.0.2/src/zinolib.egg-info/SOURCES.txt` & `zinolib-1.0.3/src/zinolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tests/config/test_tcl.py` & `zinolib-1.0.3/tests/config/test_tcl.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tests/config/test_toml.py` & `zinolib-1.0.3/tests/config/test_toml.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tests/config/test_utils.py` & `zinolib-1.0.3/tests/config/test_utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tests/config/test_zino1.py` & `zinolib-1.0.3/tests/config/test_zino1.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tests/ritz/test_default.py` & `zinolib-1.0.3/tests/ritz/test_default.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tests/ritz/test_slow.py` & `zinolib-1.0.3/tests/ritz/test_slow.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tests/test_zinolib_controllers_zino1.py` & `zinolib-1.0.3/tests/test_zinolib_controllers_zino1.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,29 +236,29 @@
         with self.assertLogs('zinolib.controllers.zino1', level='WARNING') as cm:
             self.assertFalse(updates.fallback(update))
 
     def test_handle_new_stateless_event_is_very_special(self):
         zino1 = self.init_manager()
         updates = UpdateHandler(zino1)
         update = NotifierResponse(1337, "", "")
-        result = updates.handle(update)
+        result = updates.handle_event_update(update)
         self.assertEqual(result, None)
 
     def test_handle_known_type(self):
         zino1 = self.init_manager()
         zino1.get_events()
         old_events = zino1.events.copy()
         old_events[raw_event_id].priority = 500
         updates = UpdateHandler(zino1)
         update = NotifierResponse(raw_event_id, updates.UpdateType.LOG, "")
-        ok = updates.handle(update)  # will refetch events
+        ok = updates.handle_event_update(update)  # will refetch events
         self.assertTrue(ok)
         self.assertNotEqual(zino1.events[raw_event_id].priority, old_events[raw_event_id].priority)
 
     def test_handle_unknown_type(self):
         zino1 = self.init_manager()
         zino1.get_events()
         updates = UpdateHandler(zino1)
         update = NotifierResponse(raw_event_id, "trout", "")
         with self.assertLogs('zinolib.controllers.zino1', level='WARNING'):
-            ok = updates.handle(update)  # will run fallback
+            ok = updates.handle_event_update(update)  # will run fallback
             self.assertFalse(ok)
```

### Comparing `zinolib-1.0.2/tests/test_zinolib_event_types.py` & `zinolib-1.0.3/tests/test_zinolib_event_types.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tests/utils.py` & `zinolib-1.0.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.2/tox.ini` & `zinolib-1.0.3/tox.ini`

 * *Files identical despite different names*

