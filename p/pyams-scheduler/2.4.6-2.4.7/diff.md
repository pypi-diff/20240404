# Comparing `tmp/pyams_scheduler-2.4.6.tar.gz` & `tmp/pyams_scheduler-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_scheduler-2.4.6.tar", last modified: Wed Feb 14 16:52:16 2024, max compression
+gzip compressed data, was "dist/pyams_scheduler-2.4.7.tar", last modified: Thu Apr  4 08:19:09 2024, max compression
```

## Comparing `pyams_scheduler-2.4.6.tar` & `pyams_scheduler-2.4.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6203 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/docs/
--rwxrwxrwx   0 root         (0) root         (0)     4235 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1428 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2953 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3024 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/folder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1967 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7653 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     7233 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/
--rw-rw-rw-   0 root         (0) root         (0)    12685 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8166 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     3507 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/ssh.py
--rw-rw-rw-   0 root         (0) root         (0)     8391 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    29885 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.mo
--rw-rw-rw-   0 root         (0) root         (0)    46701 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.po
--rw-rw-rw-   0 root         (0) root         (0)    30452 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/locales/pyams_scheduler.pot
--rw-rw-rw-   0 root         (0) root         (0)    11296 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/process.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/
--rw-rw-rw-   0 root         (0) root         (0)    23220 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5777 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/ftp.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/local.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     5539 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    10599 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     6355 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/ssh.py
--rw-rw-rw-   0 root         (0) root         (0)    12058 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     9023 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10917 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     9930 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     4625 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/ssh.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/tests/
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     7580 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    11156 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8871 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     9937 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4056 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     3851 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/templates/directory-host-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      725 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/templates/directory-host-input.pt
--rw-rw-rw-   0 root         (0) root         (0)    10200 2024-02-14 16:51:18.000000 pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6203 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2118 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      404 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-02-14 16:52:16.000000 pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6258 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     4310 2024-04-04 08:10:32.000000 pyams_scheduler-2.4.7/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2953 2024-04-04 08:10:32.000000 pyams_scheduler-2.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3024 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/folder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2024-02-01 13:14:38.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     7233 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/
+-rw-rw-rw-   0 root         (0) root         (0)    12685 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8166 2023-12-20 09:03:43.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3507 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/ssh.py
+-rw-rw-rw-   0 root         (0) root         (0)     8391 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    29885 2024-02-03 00:13:32.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.mo
+-rw-rw-rw-   0 root         (0) root         (0)    46701 2024-02-03 00:13:32.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.po
+-rw-rw-rw-   0 root         (0) root         (0)    30452 2024-01-05 13:03:39.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/locales/pyams_scheduler.pot
+-rw-rw-rw-   0 root         (0) root         (0)    11296 2024-01-04 11:48:06.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-02-01 13:14:38.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/
+-rw-rw-rw-   0 root         (0) root         (0)    23335 2024-04-04 08:10:32.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5777 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/ftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5539 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    10599 2024-02-02 15:57:16.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6355 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/ssh.py
+-rw-rw-rw-   0 root         (0) root         (0)    12058 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     9023 2024-02-03 00:13:32.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10917 2024-02-03 00:13:32.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     9930 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4625 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/ssh.py
+-rw-rw-rw-   0 root         (0) root         (0)     6309 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     7580 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    11156 2024-02-03 00:13:32.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8871 2024-02-01 13:14:38.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9937 2024-02-02 15:57:16.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2024-02-02 15:57:16.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/templates/directory-host-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-12-16 10:16:55.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/templates/directory-host-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)    10200 2024-01-03 14:55:13.000000 pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6258 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2118 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 08:19:00.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-04 08:19:09.000000 pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/top_level.txt
```

### Comparing `pyams_scheduler-2.4.6/LICENSE` & `pyams_scheduler-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/PKG-INFO` & `pyams_scheduler-2.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyams_scheduler
-Version: 2.4.6
+Version: 2.4.7
 Summary: PyAMS tasks scheduler
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
 License-File: LICENSE
@@ -51,14 +50,18 @@
 
 The package relies on ZeroMQ for process synchronisation, and APScheduler for tasks scheduling.
 
 
 Changelog
 =========
 
+2.4.7
+-----
+ - avoid exception after task execution when chat is disabled
+
 2.4.6
 -----
  - added source task as chat message user attribute to correctly get message targets
 
 2.4.5
 -----
  - updated ZMI menus and views permissions for guests better access
@@ -256,9 +259,7 @@
 -----
  - updated Gitlab-CI configuration
  - removed Travis-CI configuration
 
 1.0.0
 -----
  - initial release
-
-
```

### Comparing `pyams_scheduler-2.4.6/docs/HISTORY.rst` & `pyams_scheduler-2.4.7/docs/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.4.7
+-----
+ - avoid exception after task execution when chat is disabled
+
 2.4.6
 -----
  - added source task as chat message user attribute to correctly get message targets
 
 2.4.5
 -----
  - updated ZMI menus and views permissions for guests better access
```

### Comparing `pyams_scheduler-2.4.6/docs/README.rst` & `pyams_scheduler-2.4.7/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/setup.py` & `pyams_scheduler-2.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.4.6'
+version = '2.4.7'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/doctests/README.rst` & `pyams_scheduler-2.4.7/src/pyams_scheduler/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/folder.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/generations/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/include.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/include.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/rest.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/ssh.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/ssh.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/interfaces/task/sync.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/interfaces/task/sync.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.mo` & `pyams_scheduler-2.4.7/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.mo`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.po` & `pyams_scheduler-2.4.7/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.po`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/locales/pyams_scheduler.pot` & `pyams_scheduler-2.4.7/src/pyams_scheduler/locales/pyams_scheduler.pot`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/process.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/process.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/scheduler.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,14 +293,15 @@
                                 LOGGER.debug("Skipping inactive task {0}".format(task.name))
                                 return status, result
                             translate = request.localizer.translate
                             tm = ITransactionManager(task)  # pylint: disable=invalid-name
                             for attempt in tm.attempts():
                                 with attempt as t:  # pylint: disable=invalid-name
                                     status = TASK_STATUS_NONE
+                                    message = None
                                     start_date = datetime.utcnow()
                                     duration = 0.
                                     try:
                                         registry.notify(BeforeRunJobEvent(task))
                                         (status, result) = task.run(report, **kwargs)
                                         if status == TASK_STATUS_FAIL:
                                             raise FailedTaskRunException
@@ -353,15 +354,16 @@
                                                                     "")).format(task.name),
                                                 url='/'.join(('', '++etc++site') +
                                                              tuple(self.get_path_elements()) +
                                                              ('++history++', history_item.__name__,
                                                               'history.html')),
                                                 modal=True,
                                                 task=task)
-                                    message.send()
+                                    if message is not None:
+                                        message.send()
                                     registry.notify(AfterRunJobEvent(task, status, result))
                                     task.send_report(report, status, registry)
                                 if t.status == COMMITTED_STATUS:
                                     break
                 finally:
                     set_local_registry(old_registry)
             except:  # pylint: disable=bare-except
```

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/ftp.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/ftp.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/local.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/local.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/handler/sftp.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/handler/sftp.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/notification.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/rest.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/ssh.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/ssh.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/sync.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/sync.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/notification.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/rest.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/ssh.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/ssh.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/task/zmi/sync.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/task/zmi/sync.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/tests/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/tests/test_utilsdocs.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/tests/test_utilsdocstrings.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/trigger.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/trigger.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/__init__.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/folder.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/history.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/history.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/interfaces.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/jobs.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/jobs.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/scheduler.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/templates/directory-host-display.pt` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/templates/directory-host-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/templates/directory-host-input.pt` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/templates/directory-host-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler/zmi/trigger.py` & `pyams_scheduler-2.4.7/src/pyams_scheduler/zmi/trigger.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/PKG-INFO` & `pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyams-scheduler
-Version: 2.4.6
+Version: 2.4.7
 Summary: PyAMS tasks scheduler
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
 License-File: LICENSE
@@ -51,14 +50,18 @@
 
 The package relies on ZeroMQ for process synchronisation, and APScheduler for tasks scheduling.
 
 
 Changelog
 =========
 
+2.4.7
+-----
+ - avoid exception after task execution when chat is disabled
+
 2.4.6
 -----
  - added source task as chat message user attribute to correctly get message targets
 
 2.4.5
 -----
  - updated ZMI menus and views permissions for guests better access
@@ -256,9 +259,7 @@
 -----
  - updated Gitlab-CI configuration
  - removed Travis-CI configuration
 
 1.0.0
 -----
  - initial release
-
-
```

### Comparing `pyams_scheduler-2.4.6/src/pyams_scheduler.egg-info/SOURCES.txt` & `pyams_scheduler-2.4.7/src/pyams_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

