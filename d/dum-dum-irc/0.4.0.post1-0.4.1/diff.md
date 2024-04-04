# Comparing `tmp/dum-dum-irc-0.4.0.post1.tar.gz` & `tmp/dum-dum-irc-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dum-dum-irc-0.4.0.post1.tar", last modified: Sat Mar 30 22:32:11 2024, max compression
+gzip compressed data, was "dum-dum-irc-0.4.1.tar", last modified: Thu Apr  4 21:13:31 2024, max compression
```

## Comparing `dum-dum-irc-0.4.0.post1.tar` & `dum-dum-irc-0.4.1.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:11.025509 dum-dum-irc-0.4.0.post1/
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.944751 dum-dum-irc-0.4.0.post1/.github/
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.958455 dum-dum-irc-0.4.0.post1/.github/workflows/
--rw-rw-rw-   0        0        0      424 2024-03-09 16:40:11.000000 dum-dum-irc-0.4.0.post1/.github/workflows/pyright-lint.yml
--rw-rw-rw-   0        0        0      384 2024-03-09 16:40:03.000000 dum-dum-irc-0.4.0.post1/.github/workflows/python-test.yml
--rw-rw-rw-   0        0        0     3024 2024-03-24 05:03:08.000000 dum-dum-irc-0.4.0.post1/.gitignore
--rw-rw-rw-   0        0        0     6592 2024-03-30 22:31:44.000000 dum-dum-irc-0.4.0.post1/CHANGELOG.md
--rw-rw-rw-   0        0        0     2504 2024-03-19 19:36:13.000000 dum-dum-irc-0.4.0.post1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1091 2024-01-13 19:00:47.000000 dum-dum-irc-0.4.0.post1/LICENSE
--rw-rw-rw-   0        0        0       80 2024-03-11 15:28:00.000000 dum-dum-irc-0.4.0.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     5040 2024-03-30 22:32:11.024313 dum-dum-irc-0.4.0.post1/PKG-INFO
--rw-rw-rw-   0        0        0     4444 2024-03-30 22:29:35.000000 dum-dum-irc-0.4.0.post1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.946081 dum-dum-irc-0.4.0.post1/docs/
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.959462 dum-dum-irc-0.4.0.post1/docs/images/
--rw-rw-rw-   0        0        0    58505 2024-03-21 20:02:00.000000 dum-dum-irc-0.4.0.post1/docs/images/demo.png
--rw-rw-rw-   0        0        0     1174 2024-03-30 21:56:24.000000 dum-dum-irc-0.4.0.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 22:32:11.025509 dum-dum-irc-0.4.0.post1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.947093 dum-dum-irc-0.4.0.post1/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:11.023314 dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/
--rw-rw-rw-   0        0        0     5040 2024-03-30 22:32:10.000000 dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1813 2024-03-30 22:32:10.000000 dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 22:32:10.000000 dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2024-03-30 22:32:10.000000 dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       86 2024-03-30 22:32:10.000000 dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-30 22:32:10.000000 dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.985640 dum-dum-irc-0.4.0.post1/src/dumdum/
--rw-rw-rw-   0        0        0        0 2024-03-08 15:19:16.000000 dum-dum-irc-0.4.0.post1/src/dumdum/__init__.py
--rw-rw-rw-   0        0        0      164 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/appdirs.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.996236 dum-dum-irc-0.4.0.post1/src/dumdum/client/
--rw-rw-rw-   0        0        0        0 2024-03-09 06:31:44.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/__init__.py
--rw-rw-rw-   0        0        0     2264 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/__main__.py
--rw-rw-rw-   0        0        0     9027 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/app.py
--rw-rw-rw-   0        0        0     6020 2024-03-24 07:35:15.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/async_client.py
--rw-rw-rw-   0        0        0     8403 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/chat_frame.py
--rw-rw-rw-   0        0        0     6073 2024-03-24 06:00:44.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/connect_frame.py
--rw-rw-rw-   0        0        0      372 2024-03-24 05:47:55.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/errors.py
--rw-rw-rw-   0        0        0     1182 2024-03-09 06:32:40.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/event_thread.py
--rw-rw-rw-   0        0        0     1867 2024-03-24 06:00:44.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/file_entry.py
--rw-rw-rw-   0        0        0     5270 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/scrollable_frame.py
--rw-rw-rw-   0        0        0     1960 2024-03-11 20:45:20.000000 dum-dum-irc-0.4.0.post1/src/dumdum/client/store.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.999242 dum-dum-irc-0.4.0.post1/src/dumdum/db/
--rw-rw-rw-   0        0        0      107 2024-03-11 15:24:20.000000 dum-dum-irc-0.4.0.post1/src/dumdum/db/__init__.py
--rw-rw-rw-   0        0        0     2431 2024-03-03 20:02:04.000000 dum-dum-irc-0.4.0.post1/src/dumdum/db/connection.py
--rw-rw-rw-   0        0        0     1435 2024-03-11 20:09:28.000000 dum-dum-irc-0.4.0.post1/src/dumdum/db/migrations.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:10.947093 dum-dum-irc-0.4.0.post1/src/dumdum/db/scripts/
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:11.000249 dum-dum-irc-0.4.0.post1/src/dumdum/db/scripts/client/
--rw-rw-rw-   0        0        0      160 2024-03-11 19:50:30.000000 dum-dum-irc-0.4.0.post1/src/dumdum/db/scripts/client/0001-base.sql
--rw-rw-rw-   0        0        0     3389 2024-03-30 21:59:55.000000 dum-dum-irc-0.4.0.post1/src/dumdum/logging.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:11.008902 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/
--rw-rw-rw-   0        0        0     1077 2024-03-13 14:46:58.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/README.md
--rw-rw-rw-   0        0        0     1301 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/__init__.py
--rw-rw-rw-   0        0        0      522 2024-03-09 04:17:41.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/channel.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:11.013320 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/client/
--rw-rw-rw-   0        0        0      449 2024-03-24 05:23:48.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/client/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-24 05:23:48.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/client/events.py
--rw-rw-rw-   0        0        0     1877 2024-03-24 05:48:25.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/client/messages.py
--rw-rw-rw-   0        0        0     6939 2024-03-24 05:48:25.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/client/protocol.py
--rw-rw-rw-   0        0        0      149 2024-03-13 15:01:06.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/constants.py
--rw-rw-rw-   0        0        0      349 2024-03-24 05:23:48.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/enums.py
--rw-rw-rw-   0        0        0     1282 2024-03-24 04:41:26.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/errors.py
--rw-rw-rw-   0        0        0      236 2024-03-09 16:41:53.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/interfaces.py
--rw-rw-rw-   0        0        0     1096 2024-03-13 14:35:47.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/message.py
--rw-rw-rw-   0        0        0     1669 2024-03-13 14:35:47.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/reader.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:11.016321 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/server/
--rw-rw-rw-   0        0        0      501 2024-03-24 05:23:48.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/server/__init__.py
--rw-rw-rw-   0        0        0      961 2024-03-24 05:23:48.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/server/events.py
--rw-rw-rw-   0        0        0     2343 2024-03-24 05:23:48.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/server/messages.py
--rw-rw-rw-   0        0        0     5728 2024-03-24 05:48:25.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/server/protocol.py
--rw-rw-rw-   0        0        0     1163 2024-03-13 14:48:09.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/snowflake.py
--rw-rw-rw-   0        0        0     1267 2024-03-12 16:39:29.000000 dum-dum-irc-0.4.0.post1/src/dumdum/protocol/varchar.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:11.020314 dum-dum-irc-0.4.0.post1/src/dumdum/server/
--rw-rw-rw-   0        0        0      111 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/server/__init__.py
--rw-rw-rw-   0        0        0     2428 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/server/__main__.py
--rw-rw-rw-   0        0        0     1078 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/server/connection.py
--rw-rw-rw-   0        0        0     5139 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/server/manager.py
--rw-rw-rw-   0        0        0     2723 2024-03-30 21:53:59.000000 dum-dum-irc-0.4.0.post1/src/dumdum/server/state.py
-drwxrwxrwx   0        0        0        0 2024-03-30 22:32:11.022317 dum-dum-irc-0.4.0.post1/tests/
--rw-rw-rw-   0        0        0     8077 2024-03-24 05:48:25.000000 dum-dum-irc-0.4.0.post1/tests/test_protocol.py
--rw-rw-rw-   0        0        0     1265 2024-03-12 14:57:55.000000 dum-dum-irc-0.4.0.post1/tests/test_reader.py
--rw-rw-rw-   0        0        0     2234 2024-03-12 16:36:44.000000 dum-dum-irc-0.4.0.post1/tests/test_varchar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.403914 dum-dum-irc-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.391914 dum-dum-irc-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.395913 dum-dum-irc-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/.github/workflows/pyright-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-04 21:13:31.403914 dum-dum-irc-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.391914 dum-dum-irc-0.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.395913 dum-dum-irc-0.4.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    58505 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/docs/images/demo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:13:31.403914 dum-dum-irc-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.391914 dum-dum-irc-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.403914 dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-04 21:13:31.000000 dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-04 21:13:31.000000 dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:13:31.000000 dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 21:13:31.000000 dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 21:13:31.000000 dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 21:13:31.000000 dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.395913 dum-dum-irc-0.4.1/src/dumdum/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/appdirs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.395913 dum-dum-irc-0.4.1/src/dumdum/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/chat_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/connect_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/event_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/file_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/scrollable_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/client/store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.399913 dum-dum-irc-0.4.1/src/dumdum/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/db/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.391914 dum-dum-irc-0.4.1/src/dumdum/db/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.399913 dum-dum-irc-0.4.1/src/dumdum/db/scripts/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/db/scripts/client/0001-base.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.399913 dum-dum-irc-0.4.1/src/dumdum/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.399913 dum-dum-irc-0.4.1/src/dumdum/protocol/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/client/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.399913 dum-dum-irc-0.4.1/src/dumdum/protocol/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/server/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/server/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/protocol/varchar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.403914 dum-dum-irc-0.4.1/src/dumdum/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/server/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/server/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/src/dumdum/server/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:13:31.403914 dum-dum-irc-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-04 21:13:24.000000 dum-dum-irc-0.4.1/tests/test_varchar.py
```

### Comparing `dum-dum-irc-0.4.0.post1/PKG-INFO` & `dum-dum-irc-0.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,109 @@
-Metadata-Version: 2.1
-Name: dum-dum-irc
-Version: 0.4.0.post1
-Summary: A non-standard internet relay chat program.
-Author: thegamecracks
-License: MIT
-Project-URL: Homepage, https://github.com/thegamecracks/dum-dum-irc
-Project-URL: Issue Tracker, https://github.com/thegamecracks/dum-dum-irc/issues
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: importlib-resources>=6.1.3
-Requires-Dist: platformdirs>=4.2.0
-Provides-Extra: tests
-Requires-Dist: coverage>=7.4.3; extra == "tests"
-Requires-Dist: pytest>=8.0.2; extra == "tests"
-
-# dum-dum-irc
-
-[![](https://img.shields.io/pypi/v/dum-dum-irc?style=flat-square)](https://pypi.org/project/dum-dum-irc/)
-[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/pyright-lint.yml?style=flat-square&label=pyright)](https://microsoft.github.io/pyright/#/)
-[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/python-test.yml?style=flat-square&logo=pytest&label=tests)](https://docs.pytest.org/en/stable/)
-
-A handcrafted implementation of an internet relay chat without following
-any conventions or RFC standards.
-
-![Two client windows side-by-side](https://raw.githubusercontent.com/thegamecracks/dum-dum-irc/main/docs/images/demo.png)
-
-### [Changelog] | [Contributing Guide]
-
-[Changelog]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CHANGELOG.md
-[Contributing Guide]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CONTRIBUTING.md
-
-## Usage
-
-With Python 3.11+ installed, you can get the currently stable version on PyPI:
-
-```sh
-pip install dum-dum-irc
-```
-
-Or if you have Git, you can install the latest in-development version:
-
-```sh
-pip install git+https://github.com/thegamecracks/dum-dum-irc
-```
-
-Once installed, the `dumdum` and `dumdum-server` entry points should be
-provided. Run `dumdum-server --help` for options.
-
-## Implementation
-
-Dumdum consists of two parts:
-
-1. The Sans-IO protocol, defined in [dumdum.protocol]
-2. The asyncio wrapper, defined in [dumdum.client] and [dumdum.server]
-
-The [Sans-IO] protocol is responsible for handling the generation and
-consumption of byte streams, along with producing events from received
-messages, while the asyncio wrapper is responsible for the actual network
-communication between the server and its clients.
-
-[Sans-IO]: https://sans-io.readthedocs.io/
-
-[dumdum.protocol]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/protocol
-[dumdum.client]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/client
-[dumdum.server]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/server
-
-## Protocol
-
-Clients are able to send the following messages:
-
-1. HELLO: `0x00 | 1-byte version`
-2. AUTHENTICATE: `0x02 | varchar nickname (32)`
-3. SEND_MESSAGE: `0x03 | varchar channel name (32) | varchar content (1024)`
-4. LIST_CHANNELS: `0x04`
-5. LIST_MESSAGES: `0x05 | 8-byte before snowflake or 0 | 8-byte after snowflake or 0`
-
-Servers are able to send the following messages:
-
-1. HELLO: `0x00 | 0 or 1 using SSL`
-2. INCOMPATIBLE_VERSION: `0x01 | 1-byte version`
-3. ACKNOWLEDGE_AUTHENTICATION: `0x02 | 0 or 1 success`
-4. SEND_MESSAGE: `0x03 | 8-byte snowflake | varchar channel name (32) | varchar nickname (32) | varchar content (1024)`
-5. LIST_CHANNELS: `0x04 | 2-byte length | varchar channel name (32) | ...`
-6. LIST_MESSAGES: `0x05 | 3-byte length | same fields after SEND_MESSAGE | ...`
-
-Clients must send a HELLO command and wait for the server to respond with HELLO.
-Afterwards the client must send an AUTHENTICATE command and wait for a successful
-ACKNOWLEDGE_AUTHENTICATION before they can begin chat communications.
-
-When the client disconnects and reconnects, they MUST re-send hello
-and re-authenticate with the server.
-
-If the server supports SSL, they can set `using SSL` in HELLO to indicate
-that the client should upgrade the connection to SSL.
-At this point, the protocol should not receive any data until after the
-SSL handshake is complete.
-
-As this protocol has been intentionally designed to be simple (no timeouts
-or keep alives), I/O wrappers do not need a significant amount of work to
-implement it.
-
-## TLS Encryption
-
-`dumdum-server` can use SSL certificates to encrypt connections.
-For example, if you want to use a self-signed certificate and private key,
-you can install OpenSSL and run the following command:
-
-```sh
-openssl req -new -x509 -days 365 -nodes -out dumdum.crt -keyout dumdum.key
-```
-
-After filling out (or skipping) the certificate signing request prompts,
-you can then run the server with the resulting `dumdum.crt` and `dumdum.key`
-files:
-
-```sh
-dumdum-server --cert dumdum.crt:dumdum.key
-```
-
-As for the `dumdum` client, SSL can be enabled by the user before connecting
-to a server. If the server uses a self-signed certificate, the user will need
-to download the server's certificate (.crt) and select it.
+# dum-dum-irc
+
+[![](https://img.shields.io/pypi/v/dum-dum-irc?style=flat-square)](https://pypi.org/project/dum-dum-irc/)
+[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/pyright-lint.yml?style=flat-square&label=pyright)](https://microsoft.github.io/pyright/#/)
+[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/python-test.yml?style=flat-square&logo=pytest&label=tests)](https://docs.pytest.org/en/stable/)
+
+A handcrafted implementation of an internet relay chat without following
+any conventions or RFC standards.
+
+![Two client windows side-by-side](https://raw.githubusercontent.com/thegamecracks/dum-dum-irc/main/docs/images/demo.png)
+
+### [Changelog] | [Contributing Guide]
+
+[Changelog]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CHANGELOG.md
+[Contributing Guide]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CONTRIBUTING.md
+
+## Usage
+
+With Python 3.11+ installed, you can get the current stable version on PyPI:
+
+```sh
+pip install dum-dum-irc
+```
+
+Or if you have Git, you can install the latest in-development version:
+
+```sh
+pip install git+https://github.com/thegamecracks/dum-dum-irc
+```
+
+Once installed, you can use the `dumdum` and `dumdum-server` commands.
+Running `dumdum` starts a graphical client which you can use to join
+Dumdum servers, while `dumdum-server` is used to host servers of your own.
+Both support the `-h/--help` option if you want to see more details on their usage.
+
+## Implementation
+
+Dumdum consists of two parts:
+
+1. The Sans-IO protocol, defined in [dumdum.protocol]
+2. The asyncio wrapper, defined in [dumdum.client] and [dumdum.server]
+
+The [Sans-IO] protocol is responsible for handling the generation and
+consumption of byte streams, along with producing events from received
+messages, while the asyncio wrapper is responsible for the actual network
+communication between the server and its clients.
+
+[Sans-IO]: https://sans-io.readthedocs.io/
+
+[dumdum.protocol]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/protocol
+[dumdum.client]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/client
+[dumdum.server]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/server
+
+## Protocol
+
+Clients are able to send the following messages:
+
+1. HELLO: `0x00 | 1-byte version`
+2. AUTHENTICATE: `0x02 | varchar nickname (32)`
+3. SEND_MESSAGE: `0x03 | varchar channel name (32) | varchar content (1024)`
+4. LIST_CHANNELS: `0x04`
+5. LIST_MESSAGES: `0x05 | 8-byte before snowflake or 0 | 8-byte after snowflake or 0`
+
+Servers are able to send the following messages:
+
+1. HELLO: `0x00 | 0 or 1 using SSL`
+2. INCOMPATIBLE_VERSION: `0x01 | 1-byte version`
+3. ACKNOWLEDGE_AUTHENTICATION: `0x02 | 0 or 1 success`
+4. SEND_MESSAGE: `0x03 | 8-byte snowflake | varchar channel name (32) | varchar nickname (32) | varchar content (1024)`
+5. LIST_CHANNELS: `0x04 | 2-byte length | varchar channel name (32) | ...`
+6. LIST_MESSAGES: `0x05 | 3-byte length | same fields after SEND_MESSAGE | ...`
+
+Clients must send a HELLO command and wait for the server to respond with HELLO.
+Afterwards the client must send an AUTHENTICATE command and wait for a successful
+ACKNOWLEDGE_AUTHENTICATION before they can begin chat communications.
+
+When the client disconnects and reconnects, they MUST re-send hello
+and re-authenticate with the server.
+
+If the server supports SSL, they can set `using SSL` in HELLO to indicate
+that the client should upgrade the connection to SSL.
+At this point, the protocol should not receive any data until after the
+SSL handshake is complete.
+
+As this protocol has been intentionally designed to be simple (no timeouts
+or keep alives), I/O wrappers do not need a significant amount of work to
+implement it.
+
+## TLS Encryption
+
+`dumdum-server` can use SSL certificates to encrypt connections.
+For example, if you want to use a self-signed certificate and private key,
+you can install OpenSSL and run the following command:
+
+```sh
+openssl req -new -x509 -days 365 -noenc -out dumdum.crt -keyout dumdum.key
+```
+
+After filling out (or skipping) the certificate signing request prompts,
+you can then run the server with the resulting `dumdum.crt` and `dumdum.key`
+files:
+
+```sh
+dumdum-server --cert dumdum.crt:dumdum.key
+```
+
+As for the `dumdum` client, SSL can be enabled by the user before connecting
+to a server. If the server uses a self-signed certificate, the user will need
+to download the server's certificate (.crt) and select it.
```

### Comparing `dum-dum-irc-0.4.0.post1/README.md` & `dum-dum-irc-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,126 @@
-# dum-dum-irc
-
-[![](https://img.shields.io/pypi/v/dum-dum-irc?style=flat-square)](https://pypi.org/project/dum-dum-irc/)
-[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/pyright-lint.yml?style=flat-square&label=pyright)](https://microsoft.github.io/pyright/#/)
-[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/python-test.yml?style=flat-square&logo=pytest&label=tests)](https://docs.pytest.org/en/stable/)
-
-A handcrafted implementation of an internet relay chat without following
-any conventions or RFC standards.
-
-![Two client windows side-by-side](https://raw.githubusercontent.com/thegamecracks/dum-dum-irc/main/docs/images/demo.png)
-
-### [Changelog] | [Contributing Guide]
-
-[Changelog]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CHANGELOG.md
-[Contributing Guide]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CONTRIBUTING.md
-
-## Usage
-
-With Python 3.11+ installed, you can get the currently stable version on PyPI:
-
-```sh
-pip install dum-dum-irc
-```
-
-Or if you have Git, you can install the latest in-development version:
-
-```sh
-pip install git+https://github.com/thegamecracks/dum-dum-irc
-```
-
-Once installed, the `dumdum` and `dumdum-server` entry points should be
-provided. Run `dumdum-server --help` for options.
-
-## Implementation
-
-Dumdum consists of two parts:
-
-1. The Sans-IO protocol, defined in [dumdum.protocol]
-2. The asyncio wrapper, defined in [dumdum.client] and [dumdum.server]
-
-The [Sans-IO] protocol is responsible for handling the generation and
-consumption of byte streams, along with producing events from received
-messages, while the asyncio wrapper is responsible for the actual network
-communication between the server and its clients.
-
-[Sans-IO]: https://sans-io.readthedocs.io/
-
-[dumdum.protocol]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/protocol
-[dumdum.client]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/client
-[dumdum.server]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/server
-
-## Protocol
-
-Clients are able to send the following messages:
-
-1. HELLO: `0x00 | 1-byte version`
-2. AUTHENTICATE: `0x02 | varchar nickname (32)`
-3. SEND_MESSAGE: `0x03 | varchar channel name (32) | varchar content (1024)`
-4. LIST_CHANNELS: `0x04`
-5. LIST_MESSAGES: `0x05 | 8-byte before snowflake or 0 | 8-byte after snowflake or 0`
-
-Servers are able to send the following messages:
-
-1. HELLO: `0x00 | 0 or 1 using SSL`
-2. INCOMPATIBLE_VERSION: `0x01 | 1-byte version`
-3. ACKNOWLEDGE_AUTHENTICATION: `0x02 | 0 or 1 success`
-4. SEND_MESSAGE: `0x03 | 8-byte snowflake | varchar channel name (32) | varchar nickname (32) | varchar content (1024)`
-5. LIST_CHANNELS: `0x04 | 2-byte length | varchar channel name (32) | ...`
-6. LIST_MESSAGES: `0x05 | 3-byte length | same fields after SEND_MESSAGE | ...`
-
-Clients must send a HELLO command and wait for the server to respond with HELLO.
-Afterwards the client must send an AUTHENTICATE command and wait for a successful
-ACKNOWLEDGE_AUTHENTICATION before they can begin chat communications.
-
-When the client disconnects and reconnects, they MUST re-send hello
-and re-authenticate with the server.
-
-If the server supports SSL, they can set `using SSL` in HELLO to indicate
-that the client should upgrade the connection to SSL.
-At this point, the protocol should not receive any data until after the
-SSL handshake is complete.
-
-As this protocol has been intentionally designed to be simple (no timeouts
-or keep alives), I/O wrappers do not need a significant amount of work to
-implement it.
-
-## TLS Encryption
-
-`dumdum-server` can use SSL certificates to encrypt connections.
-For example, if you want to use a self-signed certificate and private key,
-you can install OpenSSL and run the following command:
-
-```sh
-openssl req -new -x509 -days 365 -nodes -out dumdum.crt -keyout dumdum.key
-```
-
-After filling out (or skipping) the certificate signing request prompts,
-you can then run the server with the resulting `dumdum.crt` and `dumdum.key`
-files:
-
-```sh
-dumdum-server --cert dumdum.crt:dumdum.key
-```
-
-As for the `dumdum` client, SSL can be enabled by the user before connecting
-to a server. If the server uses a self-signed certificate, the user will need
-to download the server's certificate (.crt) and select it.
+Metadata-Version: 2.1
+Name: dum-dum-irc
+Version: 0.4.1
+Summary: A non-standard internet relay chat program.
+Author: thegamecracks
+License: MIT
+Project-URL: Homepage, https://github.com/thegamecracks/dum-dum-irc
+Project-URL: Issue Tracker, https://github.com/thegamecracks/dum-dum-irc/issues
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: importlib-resources>=6.1.3
+Requires-Dist: platformdirs>=4.2.0
+Provides-Extra: tests
+Requires-Dist: coverage>=7.4.3; extra == "tests"
+Requires-Dist: pytest>=8.0.2; extra == "tests"
+
+# dum-dum-irc
+
+[![](https://img.shields.io/pypi/v/dum-dum-irc?style=flat-square)](https://pypi.org/project/dum-dum-irc/)
+[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/pyright-lint.yml?style=flat-square&label=pyright)](https://microsoft.github.io/pyright/#/)
+[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/python-test.yml?style=flat-square&logo=pytest&label=tests)](https://docs.pytest.org/en/stable/)
+
+A handcrafted implementation of an internet relay chat without following
+any conventions or RFC standards.
+
+![Two client windows side-by-side](https://raw.githubusercontent.com/thegamecracks/dum-dum-irc/main/docs/images/demo.png)
+
+### [Changelog] | [Contributing Guide]
+
+[Changelog]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CHANGELOG.md
+[Contributing Guide]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CONTRIBUTING.md
+
+## Usage
+
+With Python 3.11+ installed, you can get the current stable version on PyPI:
+
+```sh
+pip install dum-dum-irc
+```
+
+Or if you have Git, you can install the latest in-development version:
+
+```sh
+pip install git+https://github.com/thegamecracks/dum-dum-irc
+```
+
+Once installed, you can use the `dumdum` and `dumdum-server` commands.
+Running `dumdum` starts a graphical client which you can use to join
+Dumdum servers, while `dumdum-server` is used to host servers of your own.
+Both support the `-h/--help` option if you want to see more details on their usage.
+
+## Implementation
+
+Dumdum consists of two parts:
+
+1. The Sans-IO protocol, defined in [dumdum.protocol]
+2. The asyncio wrapper, defined in [dumdum.client] and [dumdum.server]
+
+The [Sans-IO] protocol is responsible for handling the generation and
+consumption of byte streams, along with producing events from received
+messages, while the asyncio wrapper is responsible for the actual network
+communication between the server and its clients.
+
+[Sans-IO]: https://sans-io.readthedocs.io/
+
+[dumdum.protocol]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/protocol
+[dumdum.client]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/client
+[dumdum.server]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/server
+
+## Protocol
+
+Clients are able to send the following messages:
+
+1. HELLO: `0x00 | 1-byte version`
+2. AUTHENTICATE: `0x02 | varchar nickname (32)`
+3. SEND_MESSAGE: `0x03 | varchar channel name (32) | varchar content (1024)`
+4. LIST_CHANNELS: `0x04`
+5. LIST_MESSAGES: `0x05 | 8-byte before snowflake or 0 | 8-byte after snowflake or 0`
+
+Servers are able to send the following messages:
+
+1. HELLO: `0x00 | 0 or 1 using SSL`
+2. INCOMPATIBLE_VERSION: `0x01 | 1-byte version`
+3. ACKNOWLEDGE_AUTHENTICATION: `0x02 | 0 or 1 success`
+4. SEND_MESSAGE: `0x03 | 8-byte snowflake | varchar channel name (32) | varchar nickname (32) | varchar content (1024)`
+5. LIST_CHANNELS: `0x04 | 2-byte length | varchar channel name (32) | ...`
+6. LIST_MESSAGES: `0x05 | 3-byte length | same fields after SEND_MESSAGE | ...`
+
+Clients must send a HELLO command and wait for the server to respond with HELLO.
+Afterwards the client must send an AUTHENTICATE command and wait for a successful
+ACKNOWLEDGE_AUTHENTICATION before they can begin chat communications.
+
+When the client disconnects and reconnects, they MUST re-send hello
+and re-authenticate with the server.
+
+If the server supports SSL, they can set `using SSL` in HELLO to indicate
+that the client should upgrade the connection to SSL.
+At this point, the protocol should not receive any data until after the
+SSL handshake is complete.
+
+As this protocol has been intentionally designed to be simple (no timeouts
+or keep alives), I/O wrappers do not need a significant amount of work to
+implement it.
+
+## TLS Encryption
+
+`dumdum-server` can use SSL certificates to encrypt connections.
+For example, if you want to use a self-signed certificate and private key,
+you can install OpenSSL and run the following command:
+
+```sh
+openssl req -new -x509 -days 365 -noenc -out dumdum.crt -keyout dumdum.key
+```
+
+After filling out (or skipping) the certificate signing request prompts,
+you can then run the server with the resulting `dumdum.crt` and `dumdum.key`
+files:
+
+```sh
+dumdum-server --cert dumdum.crt:dumdum.key
+```
+
+As for the `dumdum` client, SSL can be enabled by the user before connecting
+to a server. If the server uses a self-signed certificate, the user will need
+to download the server's certificate (.crt) and select it.
```

### Comparing `dum-dum-irc-0.4.0.post1/docs/images/demo.png` & `dum-dum-irc-0.4.1/docs/images/demo.png`

 * *Files identical despite different names*

### Comparing `dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/PKG-INFO` & `dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,126 @@
-Metadata-Version: 2.1
-Name: dum-dum-irc
-Version: 0.4.0.post1
-Summary: A non-standard internet relay chat program.
-Author: thegamecracks
-License: MIT
-Project-URL: Homepage, https://github.com/thegamecracks/dum-dum-irc
-Project-URL: Issue Tracker, https://github.com/thegamecracks/dum-dum-irc/issues
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: importlib-resources>=6.1.3
-Requires-Dist: platformdirs>=4.2.0
-Provides-Extra: tests
-Requires-Dist: coverage>=7.4.3; extra == "tests"
-Requires-Dist: pytest>=8.0.2; extra == "tests"
-
-# dum-dum-irc
-
-[![](https://img.shields.io/pypi/v/dum-dum-irc?style=flat-square)](https://pypi.org/project/dum-dum-irc/)
-[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/pyright-lint.yml?style=flat-square&label=pyright)](https://microsoft.github.io/pyright/#/)
-[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/python-test.yml?style=flat-square&logo=pytest&label=tests)](https://docs.pytest.org/en/stable/)
-
-A handcrafted implementation of an internet relay chat without following
-any conventions or RFC standards.
-
-![Two client windows side-by-side](https://raw.githubusercontent.com/thegamecracks/dum-dum-irc/main/docs/images/demo.png)
-
-### [Changelog] | [Contributing Guide]
-
-[Changelog]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CHANGELOG.md
-[Contributing Guide]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CONTRIBUTING.md
-
-## Usage
-
-With Python 3.11+ installed, you can get the currently stable version on PyPI:
-
-```sh
-pip install dum-dum-irc
-```
-
-Or if you have Git, you can install the latest in-development version:
-
-```sh
-pip install git+https://github.com/thegamecracks/dum-dum-irc
-```
-
-Once installed, the `dumdum` and `dumdum-server` entry points should be
-provided. Run `dumdum-server --help` for options.
-
-## Implementation
-
-Dumdum consists of two parts:
-
-1. The Sans-IO protocol, defined in [dumdum.protocol]
-2. The asyncio wrapper, defined in [dumdum.client] and [dumdum.server]
-
-The [Sans-IO] protocol is responsible for handling the generation and
-consumption of byte streams, along with producing events from received
-messages, while the asyncio wrapper is responsible for the actual network
-communication between the server and its clients.
-
-[Sans-IO]: https://sans-io.readthedocs.io/
-
-[dumdum.protocol]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/protocol
-[dumdum.client]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/client
-[dumdum.server]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/server
-
-## Protocol
-
-Clients are able to send the following messages:
-
-1. HELLO: `0x00 | 1-byte version`
-2. AUTHENTICATE: `0x02 | varchar nickname (32)`
-3. SEND_MESSAGE: `0x03 | varchar channel name (32) | varchar content (1024)`
-4. LIST_CHANNELS: `0x04`
-5. LIST_MESSAGES: `0x05 | 8-byte before snowflake or 0 | 8-byte after snowflake or 0`
-
-Servers are able to send the following messages:
-
-1. HELLO: `0x00 | 0 or 1 using SSL`
-2. INCOMPATIBLE_VERSION: `0x01 | 1-byte version`
-3. ACKNOWLEDGE_AUTHENTICATION: `0x02 | 0 or 1 success`
-4. SEND_MESSAGE: `0x03 | 8-byte snowflake | varchar channel name (32) | varchar nickname (32) | varchar content (1024)`
-5. LIST_CHANNELS: `0x04 | 2-byte length | varchar channel name (32) | ...`
-6. LIST_MESSAGES: `0x05 | 3-byte length | same fields after SEND_MESSAGE | ...`
-
-Clients must send a HELLO command and wait for the server to respond with HELLO.
-Afterwards the client must send an AUTHENTICATE command and wait for a successful
-ACKNOWLEDGE_AUTHENTICATION before they can begin chat communications.
-
-When the client disconnects and reconnects, they MUST re-send hello
-and re-authenticate with the server.
-
-If the server supports SSL, they can set `using SSL` in HELLO to indicate
-that the client should upgrade the connection to SSL.
-At this point, the protocol should not receive any data until after the
-SSL handshake is complete.
-
-As this protocol has been intentionally designed to be simple (no timeouts
-or keep alives), I/O wrappers do not need a significant amount of work to
-implement it.
-
-## TLS Encryption
-
-`dumdum-server` can use SSL certificates to encrypt connections.
-For example, if you want to use a self-signed certificate and private key,
-you can install OpenSSL and run the following command:
-
-```sh
-openssl req -new -x509 -days 365 -nodes -out dumdum.crt -keyout dumdum.key
-```
-
-After filling out (or skipping) the certificate signing request prompts,
-you can then run the server with the resulting `dumdum.crt` and `dumdum.key`
-files:
-
-```sh
-dumdum-server --cert dumdum.crt:dumdum.key
-```
-
-As for the `dumdum` client, SSL can be enabled by the user before connecting
-to a server. If the server uses a self-signed certificate, the user will need
-to download the server's certificate (.crt) and select it.
+Metadata-Version: 2.1
+Name: dum-dum-irc
+Version: 0.4.1
+Summary: A non-standard internet relay chat program.
+Author: thegamecracks
+License: MIT
+Project-URL: Homepage, https://github.com/thegamecracks/dum-dum-irc
+Project-URL: Issue Tracker, https://github.com/thegamecracks/dum-dum-irc/issues
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: importlib-resources>=6.1.3
+Requires-Dist: platformdirs>=4.2.0
+Provides-Extra: tests
+Requires-Dist: coverage>=7.4.3; extra == "tests"
+Requires-Dist: pytest>=8.0.2; extra == "tests"
+
+# dum-dum-irc
+
+[![](https://img.shields.io/pypi/v/dum-dum-irc?style=flat-square)](https://pypi.org/project/dum-dum-irc/)
+[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/pyright-lint.yml?style=flat-square&label=pyright)](https://microsoft.github.io/pyright/#/)
+[![](https://img.shields.io/github/actions/workflow/status/thegamecracks/dum-dum-irc/python-test.yml?style=flat-square&logo=pytest&label=tests)](https://docs.pytest.org/en/stable/)
+
+A handcrafted implementation of an internet relay chat without following
+any conventions or RFC standards.
+
+![Two client windows side-by-side](https://raw.githubusercontent.com/thegamecracks/dum-dum-irc/main/docs/images/demo.png)
+
+### [Changelog] | [Contributing Guide]
+
+[Changelog]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CHANGELOG.md
+[Contributing Guide]: https://github.com/thegamecracks/dum-dum-irc/blob/main/CONTRIBUTING.md
+
+## Usage
+
+With Python 3.11+ installed, you can get the current stable version on PyPI:
+
+```sh
+pip install dum-dum-irc
+```
+
+Or if you have Git, you can install the latest in-development version:
+
+```sh
+pip install git+https://github.com/thegamecracks/dum-dum-irc
+```
+
+Once installed, you can use the `dumdum` and `dumdum-server` commands.
+Running `dumdum` starts a graphical client which you can use to join
+Dumdum servers, while `dumdum-server` is used to host servers of your own.
+Both support the `-h/--help` option if you want to see more details on their usage.
+
+## Implementation
+
+Dumdum consists of two parts:
+
+1. The Sans-IO protocol, defined in [dumdum.protocol]
+2. The asyncio wrapper, defined in [dumdum.client] and [dumdum.server]
+
+The [Sans-IO] protocol is responsible for handling the generation and
+consumption of byte streams, along with producing events from received
+messages, while the asyncio wrapper is responsible for the actual network
+communication between the server and its clients.
+
+[Sans-IO]: https://sans-io.readthedocs.io/
+
+[dumdum.protocol]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/protocol
+[dumdum.client]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/client
+[dumdum.server]: https://github.com/thegamecracks/dum-dum-irc/tree/main/src/dumdum/server
+
+## Protocol
+
+Clients are able to send the following messages:
+
+1. HELLO: `0x00 | 1-byte version`
+2. AUTHENTICATE: `0x02 | varchar nickname (32)`
+3. SEND_MESSAGE: `0x03 | varchar channel name (32) | varchar content (1024)`
+4. LIST_CHANNELS: `0x04`
+5. LIST_MESSAGES: `0x05 | 8-byte before snowflake or 0 | 8-byte after snowflake or 0`
+
+Servers are able to send the following messages:
+
+1. HELLO: `0x00 | 0 or 1 using SSL`
+2. INCOMPATIBLE_VERSION: `0x01 | 1-byte version`
+3. ACKNOWLEDGE_AUTHENTICATION: `0x02 | 0 or 1 success`
+4. SEND_MESSAGE: `0x03 | 8-byte snowflake | varchar channel name (32) | varchar nickname (32) | varchar content (1024)`
+5. LIST_CHANNELS: `0x04 | 2-byte length | varchar channel name (32) | ...`
+6. LIST_MESSAGES: `0x05 | 3-byte length | same fields after SEND_MESSAGE | ...`
+
+Clients must send a HELLO command and wait for the server to respond with HELLO.
+Afterwards the client must send an AUTHENTICATE command and wait for a successful
+ACKNOWLEDGE_AUTHENTICATION before they can begin chat communications.
+
+When the client disconnects and reconnects, they MUST re-send hello
+and re-authenticate with the server.
+
+If the server supports SSL, they can set `using SSL` in HELLO to indicate
+that the client should upgrade the connection to SSL.
+At this point, the protocol should not receive any data until after the
+SSL handshake is complete.
+
+As this protocol has been intentionally designed to be simple (no timeouts
+or keep alives), I/O wrappers do not need a significant amount of work to
+implement it.
+
+## TLS Encryption
+
+`dumdum-server` can use SSL certificates to encrypt connections.
+For example, if you want to use a self-signed certificate and private key,
+you can install OpenSSL and run the following command:
+
+```sh
+openssl req -new -x509 -days 365 -noenc -out dumdum.crt -keyout dumdum.key
+```
+
+After filling out (or skipping) the certificate signing request prompts,
+you can then run the server with the resulting `dumdum.crt` and `dumdum.key`
+files:
+
+```sh
+dumdum-server --cert dumdum.crt:dumdum.key
+```
+
+As for the `dumdum` client, SSL can be enabled by the user before connecting
+to a server. If the server uses a self-signed certificate, the user will need
+to download the server's certificate (.crt) and select it.
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dum_dum_irc.egg-info/SOURCES.txt` & `dum-dum-irc-0.4.1/src/dum_dum_irc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 .github/workflows/pyright-lint.yml
+.github/workflows/python-publish.yml
 .github/workflows/python-test.yml
 docs/images/demo.png
 src/dum_dum_irc.egg-info/PKG-INFO
 src/dum_dum_irc.egg-info/SOURCES.txt
 src/dum_dum_irc.egg-info/dependency_links.txt
 src/dum_dum_irc.egg-info/entry_points.txt
 src/dum_dum_irc.egg-info/requires.txt
@@ -30,14 +31,15 @@
 src/dumdum/client/store.py
 src/dumdum/db/__init__.py
 src/dumdum/db/connection.py
 src/dumdum/db/migrations.py
 src/dumdum/db/scripts/client/0001-base.sql
 src/dumdum/protocol/README.md
 src/dumdum/protocol/__init__.py
+src/dumdum/protocol/buffer.py
 src/dumdum/protocol/channel.py
 src/dumdum/protocol/constants.py
 src/dumdum/protocol/enums.py
 src/dumdum/protocol/errors.py
 src/dumdum/protocol/interfaces.py
 src/dumdum/protocol/message.py
 src/dumdum/protocol/reader.py
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/client/__main__.py` & `dum-dum-irc-0.4.1/src/dumdum/client/__main__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""Start the client interface for connecting to dumdum servers."""
-
-from __future__ import annotations
-
-import argparse
-import contextlib
-import sys
-from typing import Iterator
-
-from dumdum.logging import configure_logging
-
-from .app import TkApp
-from .connect_frame import ConnectFrame
-from .event_thread import EventThread
-from .store import ClientStore
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description=__doc__,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="count",
-        default=0,
-        help="Increase logging verbosity",
-    )
-    parser.set_defaults(mode="gui")
-
-    commands = parser.add_subparsers()
-
-    appdirs = commands.add_parser(
-        "appdirs",
-        description="Show data directories used by dumdum.",
-    )
-    appdirs.set_defaults(mode="appdirs")
-
-    args = parser.parse_args()
-    verbose: int = args.verbose
-    mode: str = args.mode
-
-    configure_logging("client", verbose)
-    enable_windows_dpi_awareness()
-
-    if mode == "gui":
-        with contextlib.suppress(KeyboardInterrupt):
-            run_gui()
-    elif mode == "appdirs":
-        show_appdirs()
-    else:
-        raise RuntimeError(f"Unknown mode {mode!r}")
-
-
-def run_gui() -> None:
-    with EventThread() as event_thread:
-        app = TkApp(
-            event_thread=event_thread,
-            store_factory=store_factory,
-        )
-        app.switch_frame(ConnectFrame(app))
-
-        try:
-            app.mainloop()
-        except BaseException:
-            app.destroy()
-            app.mainloop()
-            raise
-
-
-def enable_windows_dpi_awareness():
-    if sys.platform == "win32":
-        from ctypes import windll
-
-        windll.shcore.SetProcessDpiAwareness(2)
-
-
-def show_appdirs() -> None:
-    from dumdum.appdirs import APP_DIRS
-
-    print("user_data_path =", APP_DIRS.user_data_path)
-    print("user_log_path =", APP_DIRS.user_log_path)
-
-
-@contextlib.contextmanager
-def store_factory() -> Iterator[ClientStore]:
-    with ClientStore.from_appdirs() as store, store.transaction():
-        yield store
-
-
-if __name__ == "__main__":
-    main()
+"""Start the client interface for connecting to dumdum servers."""
+
+from __future__ import annotations
+
+import argparse
+import contextlib
+import sys
+from typing import Iterator
+
+from dumdum.logging import configure_logging
+
+from .app import TkApp
+from .connect_frame import ConnectFrame
+from .event_thread import EventThread
+from .store import ClientStore
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description=__doc__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="count",
+        default=0,
+        help="Increase logging verbosity",
+    )
+    parser.set_defaults(mode="gui")
+
+    commands = parser.add_subparsers()
+
+    appdirs = commands.add_parser(
+        "appdirs",
+        description="Show data directories used by dumdum.",
+    )
+    appdirs.set_defaults(mode="appdirs")
+
+    args = parser.parse_args()
+    verbose: int = args.verbose
+    mode: str = args.mode
+
+    configure_logging("client", verbose)
+    enable_windows_dpi_awareness()
+
+    if mode == "gui":
+        with contextlib.suppress(KeyboardInterrupt):
+            run_gui()
+    elif mode == "appdirs":
+        show_appdirs()
+    else:
+        raise RuntimeError(f"Unknown mode {mode!r}")
+
+
+def run_gui() -> None:
+    with EventThread() as event_thread:
+        app = TkApp(
+            event_thread=event_thread,
+            store_factory=store_factory,
+        )
+        app.switch_frame(ConnectFrame(app))
+
+        try:
+            app.mainloop()
+        except BaseException:
+            app.destroy()
+            app.mainloop()
+            raise
+
+
+def enable_windows_dpi_awareness():
+    if sys.platform == "win32":
+        from ctypes import windll
+
+        windll.shcore.SetProcessDpiAwareness(2)
+
+
+def show_appdirs() -> None:
+    from dumdum.appdirs import APP_DIRS
+
+    print("user_data_path =", APP_DIRS.user_data_path)
+    print("user_log_path =", APP_DIRS.user_log_path)
+
+
+@contextlib.contextmanager
+def store_factory() -> Iterator[ClientStore]:
+    with ClientStore.from_appdirs() as store, store.transaction():
+        yield store
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/client/async_client.py` & `dum-dum-irc-0.4.1/src/dumdum/client/async_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,188 +1,201 @@
-import asyncio
-import contextlib
-import ssl
-from typing import Any, AsyncIterator, Callable, Iterator, Self
-
-from dumdum.protocol import (
-    Client,
-    ClientEvent,
-    ClientEventAuthentication,
-    ClientEventHello,
-    ClientEventIncompatibleVersion,
-)
-
-from .errors import (
-    AuthenticationFailedError,
-    ClientCannotUpgradeSSLError,
-    ServerCannotUpgradeSSLError,
-)
-
-
-def maybe_create_fut(last: asyncio.Future | None) -> asyncio.Future:
-    if last is None:
-        return asyncio.get_running_loop().create_future()
-    return last
-
-
-class AsyncClient:
-    _reader: asyncio.StreamReader | None
-    _writer: asyncio.StreamWriter | None
-    _read_task: asyncio.Task | None
-    _addr: str | None
-    _auth_fut: asyncio.Future[bool | None] | None
-    _ssl_context: ssl.SSLContext | None
-
-    def __init__(
-        self,
-        nick: str,
-        *,
-        event_callback: Callable[[ClientEvent], Any],
-    ) -> None:
-        self.nick = nick
-        self.event_callback = event_callback
-
-        self._protocol = Client(nick)
-        self._reader = None
-        self._writer = None
-        self._read_task = None
-        self._addr = None
-
-        self._auth_fut = None
-        self._ssl_context = None
-
-    @property
-    def addr(self) -> str:
-        if self._addr is None:
-            raise RuntimeError("addr is not yet defined")
-        return self._addr
-
-    @contextlib.asynccontextmanager
-    async def connect(
-        self,
-        host: str,
-        port: int,
-        *,
-        ssl: ssl.SSLContext | None,
-    ) -> AsyncIterator[Self]:
-        self._addr = f"{host}:{port}"  # FIXME: must be canonicalized
-        self._ssl_context = ssl
-
-        with self._prepare_auth_fut():
-            self._reader, self._writer = await asyncio.open_connection(host, port)
-            async with asyncio.TaskGroup() as tg:
-                _read_coro = self._read_loop(self._reader, self._writer)
-                self._read_task = tg.create_task(_read_coro)
-
-                try:
-                    success = await self._handshake()
-                    if not success:
-                        raise AuthenticationFailedError()
-
-                    yield self
-                finally:
-                    await self.close()
-
-    async def run_forever(self) -> None:
-        assert self._read_task is not None
-        await self._read_task
-
-    async def close(self) -> None:
-        if self._writer is None:
-            return
-
-        # Any exceptions here will be repeated in _read_loop()
-        self._writer.close()
-        with contextlib.suppress(Exception):
-            await self._writer.wait_closed()
-
-    async def send_message(self, channel_name: str, content: str) -> None:
-        data = self._protocol.send_message(channel_name, content)
-        await self._send_and_drain(data)
-
-    async def list_channels(self) -> None:
-        data = self._protocol.list_channels()
-        await self._send_and_drain(data)
-
-    async def list_messages(
-        self,
-        channel_name: str,
-        *,
-        before: int | None = None,
-        after: int | None = None,
-    ) -> None:
-        data = self._protocol.list_messages(channel_name, before=before, after=after)
-        await self._send_and_drain(data)
-
-    @contextlib.contextmanager
-    def _prepare_auth_fut(self) -> Iterator[None]:
-        self._auth_fut = maybe_create_fut(self._auth_fut)
-        try:
-            yield
-        finally:
-            self._set_authentication(None)
-
-    async def _read_loop(
-        self,
-        reader: asyncio.StreamReader,
-        writer: asyncio.StreamWriter,
-    ) -> None:
-        while True:
-            data = await reader.read(1024)
-            if len(data) == 0:
-                break
-
-            events, outgoing = self._protocol.receive_bytes(data)
-            writer.write(outgoing)
-            await self._handle_events(events)
-            await writer.drain()  # exert backpressure
-
-    async def _handshake(self) -> bool | None:
-        assert self._writer is not None
-        data = self._protocol.hello()
-        self._writer.write(data)
-        return await self._wait_for_authentication()
-
-    async def _wait_for_authentication(self) -> bool | None:
-        self._auth_fut = maybe_create_fut(self._auth_fut)
-        return await asyncio.shield(self._auth_fut)
-
-    async def _handle_events(self, events: list[ClientEvent]) -> None:
-        for event in events:
-            await self._handle_event(event)
-
-    async def _handle_event(self, event: ClientEvent) -> None:
-        if isinstance(event, ClientEventHello):
-            if event.using_ssl:
-                await self._upgrade_to_ssl()
-            elif self._ssl_context is not None:
-                raise ServerCannotUpgradeSSLError()
-
-            assert self._writer is not None
-            data = self._protocol.authenticate()
-            self._writer.write(data)
-        elif isinstance(event, ClientEventIncompatibleVersion):
-            assert self._writer is not None
-            self._writer.close()
-        elif isinstance(event, ClientEventAuthentication):
-            self._set_authentication(event.success)
-        self._dispatch_event(event)
-
-    async def _upgrade_to_ssl(self) -> None:
-        if self._ssl_context is None:
-            raise ClientCannotUpgradeSSLError()
-
-        assert self._writer is not None
-        await self._writer.start_tls(self._ssl_context)
-
-    def _set_authentication(self, result: bool | None) -> None:
-        assert self._auth_fut is not None
-        if not self._auth_fut.done():
-            self._auth_fut.set_result(result)
-
-    def _dispatch_event(self, event: ClientEvent) -> None:
-        self.event_callback(event)
-
-    async def _send_and_drain(self, data: bytes) -> None:
-        assert self._writer is not None
-        self._writer.write(data)
-        await self._writer.drain()
+import asyncio
+import contextlib
+import ssl
+from typing import Any, AsyncIterator, Callable, Iterator, Self
+
+from dumdum.protocol import (
+    Client,
+    ClientEvent,
+    ClientEventAuthentication,
+    ClientEventHello,
+    ClientEventIncompatibleVersion,
+)
+
+from .errors import (
+    AuthenticationFailedError,
+    ClientCannotUpgradeSSLError,
+    ServerCannotUpgradeSSLError,
+)
+
+
+def maybe_create_fut(last: asyncio.Future | None) -> asyncio.Future:
+    if last is None:
+        return asyncio.get_running_loop().create_future()
+    return last
+
+
+class AsyncClient:
+    _reader: asyncio.StreamReader | None
+    _writer: asyncio.StreamWriter | None
+    _read_task: asyncio.Task | None
+    _addr: str | None
+    _auth_fut: asyncio.Future[bool | None] | None
+    _ssl_context: ssl.SSLContext | None
+
+    def __init__(
+        self,
+        nick: str,
+        *,
+        event_callback: Callable[[ClientEvent], Any],
+        drain_timeout: float = 30,
+        close_timeout: float = 5,
+    ) -> None:
+        self.nick = nick
+        self.event_callback = event_callback
+        self.drain_timeout = drain_timeout
+        self.close_timeout = close_timeout
+
+        self._protocol = Client(nick)
+        self._reader = None
+        self._writer = None
+        self._read_task = None
+        self._addr = None
+
+        self._auth_fut = None
+        self._ssl_context = None
+
+    @property
+    def addr(self) -> str:
+        if self._addr is None:
+            raise RuntimeError("addr is not yet defined")
+        return self._addr
+
+    @contextlib.asynccontextmanager
+    async def connect(
+        self,
+        host: str,
+        port: int,
+        *,
+        ssl: ssl.SSLContext | None,
+    ) -> AsyncIterator[Self]:
+        self._addr = f"{host}:{port}"  # FIXME: must be canonicalized
+        self._ssl_context = ssl
+
+        with self._prepare_auth_fut():
+            self._reader, self._writer = await asyncio.open_connection(host, port)
+            async with asyncio.TaskGroup() as tg:
+                _read_coro = self._read_loop(self._reader, self._writer)
+                self._read_task = tg.create_task(_read_coro)
+
+                try:
+                    success = await self._handshake()
+                    if not success:
+                        raise AuthenticationFailedError()
+
+                    yield self
+                finally:
+                    await self.close()
+
+    async def run_forever(self) -> None:
+        assert self._read_task is not None
+        await self._read_task
+
+    async def close(self) -> None:
+        if self._writer is None:
+            return
+
+        # Any exceptions here will be repeated in _read_loop()
+        self._writer.close()
+        await self._wait_closed()
+
+    async def send_message(self, channel_name: str, content: str) -> None:
+        data = self._protocol.send_message(channel_name, content)
+        await self._send_and_drain(data)
+
+    async def list_channels(self) -> None:
+        data = self._protocol.list_channels()
+        await self._send_and_drain(data)
+
+    async def list_messages(
+        self,
+        channel_name: str,
+        *,
+        before: int | None = None,
+        after: int | None = None,
+    ) -> None:
+        data = self._protocol.list_messages(channel_name, before=before, after=after)
+        await self._send_and_drain(data)
+
+    @contextlib.contextmanager
+    def _prepare_auth_fut(self) -> Iterator[None]:
+        self._auth_fut = maybe_create_fut(self._auth_fut)
+        try:
+            yield
+        finally:
+            self._set_authentication(None)
+
+    async def _read_loop(
+        self,
+        reader: asyncio.StreamReader,
+        writer: asyncio.StreamWriter,
+    ) -> None:
+        while True:
+            data = await reader.read(1024)
+            if len(data) == 0:
+                break
+
+            events, outgoing = self._protocol.receive_bytes(data)
+            writer.write(outgoing)
+            await self._handle_events(events)
+            await self._drain()  # exert backpressure
+
+    async def _handshake(self) -> bool | None:
+        assert self._writer is not None
+        data = self._protocol.hello()
+        self._writer.write(data)
+        return await self._wait_for_authentication()
+
+    async def _wait_for_authentication(self) -> bool | None:
+        self._auth_fut = maybe_create_fut(self._auth_fut)
+        return await asyncio.shield(self._auth_fut)
+
+    async def _handle_events(self, events: list[ClientEvent]) -> None:
+        for event in events:
+            await self._handle_event(event)
+
+    async def _handle_event(self, event: ClientEvent) -> None:
+        if isinstance(event, ClientEventHello):
+            if event.using_ssl:
+                await self._upgrade_to_ssl()
+            elif self._ssl_context is not None:
+                raise ServerCannotUpgradeSSLError()
+
+            assert self._writer is not None
+            data = self._protocol.authenticate()
+            self._writer.write(data)
+        elif isinstance(event, ClientEventIncompatibleVersion):
+            assert self._writer is not None
+            self._writer.close()
+        elif isinstance(event, ClientEventAuthentication):
+            self._set_authentication(event.success)
+        self._dispatch_event(event)
+
+    async def _upgrade_to_ssl(self) -> None:
+        if self._ssl_context is None:
+            raise ClientCannotUpgradeSSLError()
+
+        assert self._writer is not None
+        await self._writer.start_tls(self._ssl_context)
+
+    def _set_authentication(self, result: bool | None) -> None:
+        assert self._auth_fut is not None
+        if not self._auth_fut.done():
+            self._auth_fut.set_result(result)
+
+    def _dispatch_event(self, event: ClientEvent) -> None:
+        self.event_callback(event)
+
+    async def _send_and_drain(self, data: bytes) -> None:
+        assert self._writer is not None
+        self._writer.write(data)
+        await self._drain()
+
+    async def _drain(self) -> None:
+        assert self._writer is not None
+        await asyncio.wait_for(self._writer.drain(), timeout=self.drain_timeout)
+
+    async def _wait_closed(self) -> None:
+        assert self._writer is not None
+        timeout = self.close_timeout
+        with contextlib.suppress(Exception):
+            await asyncio.wait_for(self._writer.wait_closed(), timeout=timeout)
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/client/connect_frame.py` & `dum-dum-irc-0.4.1/src/dumdum/client/connect_frame.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-import concurrent.futures
-import logging
-import ssl
-from pathlib import Path
-from tkinter import BooleanVar, StringVar, messagebox
-from tkinter.ttk import Button, Checkbutton, Entry, Frame, Label
-
-from .app import TkApp
-from .file_entry import ALL_FILETYPE, SSL_CERTIFICATE_FILETYPE, FileEntry
-
-log = logging.getLogger(__name__)
-
-
-class ConnectFrame(Frame):
-    _connection_attempt: concurrent.futures.Future[None] | None
-
-    def __init__(self, app: TkApp):
-        super().__init__(padding=10)
-
-        self.app = app
-
-        self.grid_columnconfigure(1, weight=1)
-
-        self.host_label = Label(self, text="Host:")
-        self.host_label.grid(row=0, column=0, sticky="w")
-        self.host_entry_var = StringVar(self)
-        self.host_entry = Entry(self, textvariable=self.host_entry_var)
-        self.host_entry.grid(row=0, column=1, sticky="ew")
-
-        self.port_label = Label(self, text="Port:")
-        self.port_label.grid(row=1, column=0, sticky="w")
-        self.port_entry_var = StringVar(self)
-        self.port_entry = Entry(self, textvariable=self.port_entry_var)
-        self.port_entry.grid(row=1, column=1, sticky="ew")
-
-        self.ssl_enabled_var = BooleanVar(self, value=False)
-        self.ssl_enabled = Checkbutton(
-            self,
-            text="Use SSL?",
-            variable=self.ssl_enabled_var,
-        )
-        self.ssl_enabled.grid(row=2, column=0, sticky="w")
-        self.ssl_enabled_var.trace_add("write", self._on_cert_check_var_write)
-
-        self.ssl_cert = FileEntry(
-            self,
-            text="Certificate (Optional):",
-            browse_kwargs={
-                "title": "Use Certificate File",
-                "filetypes": [SSL_CERTIFICATE_FILETYPE, ALL_FILETYPE],
-            },
-        )
-        self.ssl_cert.grid(row=2, column=1, padx=(15, 0), sticky="ew")
-
-        self.nick_label = Label(self, text="Nickname:")
-        self.nick_label.grid(row=3, column=0, sticky="w")
-        self.nick_entry_var = StringVar(self)
-        self.nick_entry = Entry(self, textvariable=self.nick_entry_var)
-        self.nick_entry.grid(row=3, column=1, sticky="ew")
-
-        self.connect = Button(self, text="Connect", command=self.do_connect)
-        self.connect.grid(row=3, column=1, sticky="e")
-
-        self.apply_last_connect_entries()
-
-        self._connect_bind = app.bind("<Return>", lambda event: self.do_connect())
-
-        self._connection_attempt = None
-        self._destroying = False
-
-    def apply_last_connect_entries(self) -> None:
-        with self.app.store_factory() as store:
-            host = store.get_setting("last-connect-host", "127.0.0.1")
-            port = store.get_setting("last-connect-port", 6667)
-            nick = store.get_setting("last-connect-nick", "Somebody")
-            ssl_enabled = store.get_setting("last-connect-ssl-enabled", False)
-            ssl_cert = store.get_setting("last-connect-ssl-cert", "")
-
-        self.host_entry_var.set(host)
-        self.port_entry_var.set(port)
-        self.nick_entry_var.set(nick)
-        self.ssl_enabled_var.set(ssl_enabled)
-        self.ssl_cert.var.set(ssl_cert)
-
-    def do_connect(self) -> None:
-        fut = self._connection_attempt
-        if fut is not None and not fut.done():
-            return
-
-        host = self.host_entry_var.get()
-        port = int(self.port_entry_var.get())
-        nick = self.nick_entry_var.get()
-        ssl_enabled = self.ssl_enabled_var.get()
-        ssl_cert = self.ssl_cert.get()
-
-        if ssl_enabled:
-            path = self.ssl_cert.get_path()
-            if path is not None and not path.is_file():
-                messagebox.showerror(
-                    "Certificate Not Found",
-                    "The SSL certificate path does not exist.",
-                )
-                return
-
-            try:
-                ssl_context = self._create_ssl_context(path)
-            except ssl.SSLError as e:
-                log.error("Could not create SSL context", exc_info=e)
-                messagebox.showerror(
-                    "Invalid Certificate",
-                    "The SSL certificate could not be loaded.",
-                )
-                return
-
-        else:
-            ssl_context = None
-
-        self.set_last_connect_entries(host, port, nick, ssl_enabled, ssl_cert)
-
-        coro = self.app.attempt_connection(host, port, nick, ssl=ssl_context)
-        self._connection_attempt = self.app.submit(coro)
-
-        self.connect.state(["disabled"])
-        self._connection_attempt.add_done_callback(self._on_connection_attempt)
-
-    def set_last_connect_entries(
-        self,
-        host: str,
-        port: int,
-        nick: str,
-        ssl_enabled: bool,
-        ssl_cert: str,
-    ) -> None:
-        with self.app.store_factory() as store:
-            store.set_setting("last-connect-host", host)
-            store.set_setting("last-connect-port", port)
-            store.set_setting("last-connect-nick", nick)
-            store.set_setting("last-connect-ssl-enabled", ssl_enabled)
-            store.set_setting("last-connect-ssl-cert", ssl_cert)
-
-    def destroy(self) -> None:
-        self._destroying = True
-        self.app.unbind("<Return>", self._connect_bind)
-        super().destroy()
-
-    def _on_cert_check_var_write(self, *args) -> None:
-        enabled = self.ssl_enabled_var.get()
-        self.ssl_cert.enable(enabled)
-
-    def _create_ssl_context(self, cafile: str | Path | None) -> ssl.SSLContext:
-        if cafile is not None:
-            cafile = str(cafile)
-
-        context = ssl.create_default_context(cafile=cafile)
-
-        # WARNING: for ease of server setup, skip hostname checks for self-signed certs
-        if cafile is not None:
-            context.check_hostname = False
-
-        return context
-
-    def _on_connection_attempt(self, fut: concurrent.futures.Future) -> None:
-        if self._destroying:
-            return
-
-        self.connect.state(["!disabled"])
+import concurrent.futures
+import logging
+import ssl
+from pathlib import Path
+from tkinter import BooleanVar, StringVar, messagebox
+from tkinter.ttk import Button, Checkbutton, Entry, Frame, Label
+
+from .app import TkApp
+from .file_entry import ALL_FILETYPE, SSL_CERTIFICATE_FILETYPE, FileEntry
+
+log = logging.getLogger(__name__)
+
+
+class ConnectFrame(Frame):
+    _connection_attempt: concurrent.futures.Future[None] | None
+
+    def __init__(self, app: TkApp):
+        super().__init__(padding=10)
+
+        self.app = app
+
+        self.grid_columnconfigure(1, weight=1)
+
+        self.host_label = Label(self, text="Host:")
+        self.host_label.grid(row=0, column=0, sticky="w")
+        self.host_entry_var = StringVar(self)
+        self.host_entry = Entry(self, textvariable=self.host_entry_var)
+        self.host_entry.grid(row=0, column=1, sticky="ew")
+
+        self.port_label = Label(self, text="Port:")
+        self.port_label.grid(row=1, column=0, sticky="w")
+        self.port_entry_var = StringVar(self)
+        self.port_entry = Entry(self, textvariable=self.port_entry_var)
+        self.port_entry.grid(row=1, column=1, sticky="ew")
+
+        self.ssl_enabled_var = BooleanVar(self, value=False)
+        self.ssl_enabled = Checkbutton(
+            self,
+            text="Use SSL?",
+            variable=self.ssl_enabled_var,
+        )
+        self.ssl_enabled.grid(row=2, column=0, sticky="w")
+        self.ssl_enabled_var.trace_add("write", self._on_cert_check_var_write)
+
+        self.ssl_cert = FileEntry(
+            self,
+            text="Certificate (Optional):",
+            browse_kwargs={
+                "title": "Use Certificate File",
+                "filetypes": [SSL_CERTIFICATE_FILETYPE, ALL_FILETYPE],
+            },
+        )
+        self.ssl_cert.grid(row=2, column=1, padx=(15, 0), sticky="ew")
+
+        self.nick_label = Label(self, text="Nickname:")
+        self.nick_label.grid(row=3, column=0, sticky="w")
+        self.nick_entry_var = StringVar(self)
+        self.nick_entry = Entry(self, textvariable=self.nick_entry_var)
+        self.nick_entry.grid(row=3, column=1, sticky="ew")
+
+        self.connect = Button(self, text="Connect", command=self.do_connect)
+        self.connect.grid(row=3, column=1, sticky="e")
+
+        self.apply_last_connect_entries()
+
+        self._connect_bind = app.bind("<Return>", lambda event: self.do_connect())
+
+        self._connection_attempt = None
+        self._destroying = False
+
+    def apply_last_connect_entries(self) -> None:
+        with self.app.store_factory() as store:
+            host = store.get_setting("last-connect-host", "127.0.0.1")
+            port = store.get_setting("last-connect-port", 6667)
+            nick = store.get_setting("last-connect-nick", "Somebody")
+            ssl_enabled = store.get_setting("last-connect-ssl-enabled", False)
+            ssl_cert = store.get_setting("last-connect-ssl-cert", "")
+
+        self.host_entry_var.set(host)
+        self.port_entry_var.set(port)
+        self.nick_entry_var.set(nick)
+        self.ssl_enabled_var.set(ssl_enabled)
+        self.ssl_cert.var.set(ssl_cert)
+
+    def do_connect(self) -> None:
+        fut = self._connection_attempt
+        if fut is not None and not fut.done():
+            return
+
+        host = self.host_entry_var.get()
+        port = int(self.port_entry_var.get())
+        nick = self.nick_entry_var.get()
+        ssl_enabled = self.ssl_enabled_var.get()
+        ssl_cert = self.ssl_cert.get()
+
+        if ssl_enabled:
+            path = self.ssl_cert.get_path()
+            if path is not None and not path.is_file():
+                messagebox.showerror(
+                    "Certificate Not Found",
+                    "The SSL certificate path does not exist.",
+                )
+                return
+
+            try:
+                ssl_context = self._create_ssl_context(path)
+            except ssl.SSLError as e:
+                log.error("Could not create SSL context", exc_info=e)
+                messagebox.showerror(
+                    "Invalid Certificate",
+                    "The SSL certificate could not be loaded.",
+                )
+                return
+
+        else:
+            ssl_context = None
+
+        self.set_last_connect_entries(host, port, nick, ssl_enabled, ssl_cert)
+
+        coro = self.app.attempt_connection(host, port, nick, ssl=ssl_context)
+        self._connection_attempt = self.app.submit(coro)
+
+        self.connect.state(["disabled"])
+        self._connection_attempt.add_done_callback(self._on_connection_attempt)
+
+    def set_last_connect_entries(
+        self,
+        host: str,
+        port: int,
+        nick: str,
+        ssl_enabled: bool,
+        ssl_cert: str,
+    ) -> None:
+        with self.app.store_factory() as store:
+            store.set_setting("last-connect-host", host)
+            store.set_setting("last-connect-port", port)
+            store.set_setting("last-connect-nick", nick)
+            store.set_setting("last-connect-ssl-enabled", ssl_enabled)
+            store.set_setting("last-connect-ssl-cert", ssl_cert)
+
+    def destroy(self) -> None:
+        self._destroying = True
+        self.app.unbind("<Return>", self._connect_bind)
+        super().destroy()
+
+    def _on_cert_check_var_write(self, *args) -> None:
+        enabled = self.ssl_enabled_var.get()
+        self.ssl_cert.enable(enabled)
+
+    def _create_ssl_context(self, cafile: str | Path | None) -> ssl.SSLContext:
+        if cafile is not None:
+            cafile = str(cafile)
+
+        context = ssl.create_default_context(cafile=cafile)
+
+        # WARNING: for ease of server setup, skip hostname checks for self-signed certs
+        if cafile is not None:
+            context.check_hostname = False
+
+        return context
+
+    def _on_connection_attempt(self, fut: concurrent.futures.Future) -> None:
+        if self._destroying:
+            return
+
+        self.connect.state(["!disabled"])
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/client/event_thread.py` & `dum-dum-irc-0.4.1/src/dumdum/client/event_thread.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import asyncio
-import concurrent.futures
-import threading
-from typing import Self
-
-
-class EventThread(threading.Thread):
-    """Handles starting and stopping an asyncio event loop in a separate thread."""
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-        self.loop_fut = concurrent.futures.Future()
-        self.stop_fut = concurrent.futures.Future()
-        self.finished_fut = concurrent.futures.Future()
-
-    def __enter__(self) -> Self:
-        self.start()
-        return self
-
-    def __exit__(self, exc_type, exc_val, tb) -> None:
-        self.stop()
-        self.join()
-
-    @property
-    def loop(self) -> asyncio.AbstractEventLoop:
-        return self.loop_fut.result()
-
-    def run(self) -> None:
-        try:
-            asyncio.run(self._run_forever())
-        finally:
-            self.finished_fut.set_result(None)
-
-    def stop(self) -> None:
-        if not self.stop_fut.done():
-            self.stop_fut.set_result(None)
-
-    async def _run_forever(self) -> None:
-        self.loop_fut.set_result(asyncio.get_running_loop())
-        await asyncio.wrap_future(self.stop_fut)
+import asyncio
+import concurrent.futures
+import threading
+from typing import Self
+
+
+class EventThread(threading.Thread):
+    """Handles starting and stopping an asyncio event loop in a separate thread."""
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.loop_fut = concurrent.futures.Future()
+        self.stop_fut = concurrent.futures.Future()
+        self.finished_fut = concurrent.futures.Future()
+
+    def __enter__(self) -> Self:
+        self.start()
+        return self
+
+    def __exit__(self, exc_type, exc_val, tb) -> None:
+        self.stop()
+        self.join()
+
+    @property
+    def loop(self) -> asyncio.AbstractEventLoop:
+        return self.loop_fut.result()
+
+    def run(self) -> None:
+        try:
+            asyncio.run(self._run_forever())
+        finally:
+            self.finished_fut.set_result(None)
+
+    def stop(self) -> None:
+        if not self.stop_fut.done():
+            self.stop_fut.set_result(None)
+
+    async def _run_forever(self) -> None:
+        self.loop_fut.set_result(asyncio.get_running_loop())
+        await asyncio.wrap_future(self.stop_fut)
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/client/file_entry.py` & `dum-dum-irc-0.4.1/src/dumdum/client/file_entry.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from pathlib import Path
-from tkinter import StringVar, filedialog
-from tkinter.ttk import Button, Entry, Frame, Label
-from typing import Any
-
-ALL_FILETYPE = ("All files", ("*",))
-SSL_CERTIFICATE_FILETYPE = (
-    "SSL Certificate",
-    ("*.pem", "*.crt", "*.ca-bundle", "*.cer"),
-)
-
-
-class FileEntry(Frame):
-    def __init__(
-        self,
-        parent: Frame,
-        *,
-        browse_kwargs: dict[str, Any] | None = None,
-        text: str = "",
-    ) -> None:
-        super().__init__(parent)
-
-        if browse_kwargs is None:
-            browse_kwargs = {}
-        self.browse_kwargs = browse_kwargs
-
-        self.grid_columnconfigure(1, weight=1)
-
-        self._validatecommand = (self.register(self._validate), "%P")
-
-        self.label = Label(self, text=text)
-        self.label.grid(row=0, column=0)
-
-        self.var = StringVar(self)
-        self.entry = Entry(
-            self,
-            textvariable=self.var,
-            validate="focusout",
-            validatecommand=self._validatecommand,
-        )
-        self.entry.grid(row=0, column=1, sticky="ew")
-
-        self.browse = Button(self, text="Browse", command=self.do_browse)
-        self.browse.grid(row=0, column=2)
-
-    def enable(self, enabled: bool) -> None:
-        state = ["!disabled" if enabled else "disabled"]
-        self.entry.state(state)
-        self.browse.state(state)
-
-    def get(self) -> str:
-        return self.var.get().strip()
-
-    def get_path(self) -> Path | None:
-        filename = self.get()
-        if filename != "":
-            return Path(filename)
-
-    def do_browse(self) -> None:
-        filename = filedialog.askopenfilename(**self.browse_kwargs)
-        if filename != "":
-            self.var.set(filename)
-
-    def _validate(self, val: str) -> bool:
-        return Path(val).is_file()
+from pathlib import Path
+from tkinter import StringVar, filedialog
+from tkinter.ttk import Button, Entry, Frame, Label
+from typing import Any
+
+ALL_FILETYPE = ("All files", ("*",))
+SSL_CERTIFICATE_FILETYPE = (
+    "SSL Certificate",
+    ("*.pem", "*.crt", "*.ca-bundle", "*.cer"),
+)
+
+
+class FileEntry(Frame):
+    def __init__(
+        self,
+        parent: Frame,
+        *,
+        browse_kwargs: dict[str, Any] | None = None,
+        text: str = "",
+    ) -> None:
+        super().__init__(parent)
+
+        if browse_kwargs is None:
+            browse_kwargs = {}
+        self.browse_kwargs = browse_kwargs
+
+        self.grid_columnconfigure(1, weight=1)
+
+        self._validatecommand = (self.register(self._validate), "%P")
+
+        self.label = Label(self, text=text)
+        self.label.grid(row=0, column=0)
+
+        self.var = StringVar(self)
+        self.entry = Entry(
+            self,
+            textvariable=self.var,
+            validate="focusout",
+            validatecommand=self._validatecommand,
+        )
+        self.entry.grid(row=0, column=1, sticky="ew")
+
+        self.browse = Button(self, text="Browse", command=self.do_browse)
+        self.browse.grid(row=0, column=2)
+
+    def enable(self, enabled: bool) -> None:
+        state = ["!disabled" if enabled else "disabled"]
+        self.entry.state(state)
+        self.browse.state(state)
+
+    def get(self) -> str:
+        return self.var.get().strip()
+
+    def get_path(self) -> Path | None:
+        filename = self.get()
+        if filename != "":
+            return Path(filename)
+
+    def do_browse(self) -> None:
+        filename = filedialog.askopenfilename(**self.browse_kwargs)
+        if filename != "":
+            self.var.set(filename)
+
+    def _validate(self, val: str) -> bool:
+        return Path(val).is_file()
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/client/scrollable_frame.py` & `dum-dum-irc-0.4.1/src/dumdum/client/scrollable_frame.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from tkinter import Canvas, Event, Widget
-from tkinter.ttk import Frame, Scrollbar, Style
-from weakref import WeakSet
-
-
-class ScrollableFrame(Frame):
-    __last_scrollregion: tuple[int, int, int, int] | None
-
-    def __init__(
-        self,
-        *args,
-        autoscroll: bool = False,
-        xscroll: bool = False,
-        yscroll: bool = False,
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
-
-        self.autoscroll = autoscroll
-        self.xscroll = xscroll
-        self.yscroll = yscroll
-
-        self.grid_columnconfigure(0, weight=1)
-        self.grid_rowconfigure(0, weight=1)
-
-        self.__canvas = Canvas(self, highlightthickness=0)
-        self.__canvas.grid(row=0, column=0, sticky="nesw")
-
-        self.__xscrollbar = Scrollbar(self, orient="horizontal")
-        self.__yscrollbar = Scrollbar(self, orient="vertical")
-
-        # Use rowspan=2 or columnspan=2 appropriately if filling the
-        # bottom-right corner of the frame is desired.
-        self.__xscrollbar.grid(row=1, column=0, sticky="ew")
-        self.__yscrollbar.grid(row=0, column=1, sticky="ns")
-
-        self.__xscrollbar["command"] = self.__canvas.xview
-        self.__yscrollbar["command"] = self.__canvas.yview
-        self.__canvas["xscrollcommand"] = self.__wrap_scrollbar_set(self.__xscrollbar)
-        self.__canvas["yscrollcommand"] = self.__wrap_scrollbar_set(self.__yscrollbar)
-
-        self.inner = Frame(self.__canvas)
-        self.__inner_id = self.__canvas.create_window(
-            (0, 0), window=self.inner, anchor="nw"
-        )
-
-        self.__canvas.bind("<Configure>", lambda event: self.__update())
-        self.inner.bind("<Configure>", self.__on_inner_configure)
-
-        self.__last_scrollregion = None
-        self.__scrolled_widgets = WeakSet()
-        self.__style = Style(self)
-        self.__update_rate = 125
-        self.__update_loop()
-
-    def __on_inner_configure(self, event: Event):
-        background = self.__style.lookup(self.inner.winfo_class(), "background")
-        self.__canvas.configure(background=background)
-        self.__update()
-
-    def __update_loop(self):
-        # Without this, any changes to the inner frame won't affect
-        # the scroll bar/region until the window is resized.
-        self.__update()
-        self.after(self.__update_rate, self.__update_loop)
-
-    def __update(self):
-        scroll_edges = self.__get_scroll_edges()
-
-        # self._canvas.bbox("all") doesn't update until window resize
-        # so we're relying on the inner frame's requested height instead.
-        new_width = self.__canvas.winfo_width()
-        new_height = self.__canvas.winfo_height()
-        if self.xscroll:
-            new_width = max(new_width, self.inner.winfo_reqwidth())
-        if self.yscroll:
-            new_height = max(new_height, self.inner.winfo_reqheight())
-
-        bbox = (0, 0, new_width, new_height)
-        self.__canvas.configure(scrollregion=bbox)
-        self.__canvas.itemconfigure(self.__inner_id, width=new_width, height=new_height)
-
-        self.__update_scrollbar_visibility(self.__xscrollbar)
-        self.__update_scrollbar_visibility(self.__yscrollbar)
-        self.__propagate_scroll_binds(self.inner)
-        self.__update_scroll_edges(bbox, *scroll_edges)
-
-    def __get_scroll_edges(self) -> tuple[bool, bool]:
-        xview = self.__canvas.xview()
-        yview = self.__canvas.yview()
-        scrolled_to_right = xview[1] == 1 and xview[0] != 0
-        scrolled_to_bottom = yview[1] == 1 and yview[0] != 0
-        return scrolled_to_right, scrolled_to_bottom
-
-    def __propagate_scroll_binds(self, parent: Widget):
-        if parent not in self.__scrolled_widgets:
-            parent.bind("<MouseWheel>", self.__on_mouse_yscroll)
-            parent.bind("<Shift-MouseWheel>", self.__on_mouse_xscroll)
-            self.__scrolled_widgets.add(parent)
-
-        for child in parent.winfo_children():
-            self.__propagate_scroll_binds(child)
-
-    def __update_scroll_edges(
-        self,
-        bbox: tuple[int, int, int, int],
-        scrolled_to_right: bool,
-        scrolled_to_bottom: bool,
-    ) -> None:
-        self.__last_scrollregion, last_bbox = bbox, self.__last_scrollregion
-        if not self.autoscroll:
-            return
-        elif bbox == last_bbox:
-            return
-
-        if scrolled_to_right:
-            self.__canvas.xview_moveto(1)
-        if scrolled_to_bottom:
-            self.__canvas.yview_moveto(1)
-
-    def __on_mouse_xscroll(self, event: Event):
-        delta = int(-event.delta / 100)
-        self.__canvas.xview_scroll(delta, "units")
-
-    def __on_mouse_yscroll(self, event: Event):
-        delta = int(-event.delta / 100)
-        self.__canvas.yview_scroll(delta, "units")
-
-    def __update_scrollbar_visibility(self, scrollbar: Scrollbar):
-        if scrollbar.get() == (0, 1):
-            scrollbar.grid_remove()
-        else:
-            scrollbar.grid()
-
-    def __wrap_scrollbar_set(self, scrollbar: Scrollbar):
-        def wrapper(*args, **kwargs):
-            scrollbar.set(*args, **kwargs)
-            self.__update_scrollbar_visibility(scrollbar)
-
-        return wrapper
+from tkinter import Canvas, Event, Widget
+from tkinter.ttk import Frame, Scrollbar, Style
+from weakref import WeakSet
+
+
+class ScrollableFrame(Frame):
+    __last_scrollregion: tuple[int, int, int, int] | None
+
+    def __init__(
+        self,
+        *args,
+        autoscroll: bool = False,
+        xscroll: bool = False,
+        yscroll: bool = False,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+
+        self.autoscroll = autoscroll
+        self.xscroll = xscroll
+        self.yscroll = yscroll
+
+        self.grid_columnconfigure(0, weight=1)
+        self.grid_rowconfigure(0, weight=1)
+
+        self.__canvas = Canvas(self, highlightthickness=0)
+        self.__canvas.grid(row=0, column=0, sticky="nesw")
+
+        self.__xscrollbar = Scrollbar(self, orient="horizontal")
+        self.__yscrollbar = Scrollbar(self, orient="vertical")
+
+        # Use rowspan=2 or columnspan=2 appropriately if filling the
+        # bottom-right corner of the frame is desired.
+        self.__xscrollbar.grid(row=1, column=0, sticky="ew")
+        self.__yscrollbar.grid(row=0, column=1, sticky="ns")
+
+        self.__xscrollbar["command"] = self.__canvas.xview
+        self.__yscrollbar["command"] = self.__canvas.yview
+        self.__canvas["xscrollcommand"] = self.__wrap_scrollbar_set(self.__xscrollbar)
+        self.__canvas["yscrollcommand"] = self.__wrap_scrollbar_set(self.__yscrollbar)
+
+        self.inner = Frame(self.__canvas)
+        self.__inner_id = self.__canvas.create_window(
+            (0, 0), window=self.inner, anchor="nw"
+        )
+
+        self.__canvas.bind("<Configure>", lambda event: self.__update())
+        self.inner.bind("<Configure>", self.__on_inner_configure)
+
+        self.__last_scrollregion = None
+        self.__scrolled_widgets = WeakSet()
+        self.__style = Style(self)
+        self.__update_rate = 125
+        self.__update_loop()
+
+    def __on_inner_configure(self, event: Event):
+        background = self.__style.lookup(self.inner.winfo_class(), "background")
+        self.__canvas.configure(background=background)
+        self.__update()
+
+    def __update_loop(self):
+        # Without this, any changes to the inner frame won't affect
+        # the scroll bar/region until the window is resized.
+        self.__update()
+        self.after(self.__update_rate, self.__update_loop)
+
+    def __update(self):
+        scroll_edges = self.__get_scroll_edges()
+
+        # self._canvas.bbox("all") doesn't update until window resize
+        # so we're relying on the inner frame's requested height instead.
+        new_width = self.__canvas.winfo_width()
+        new_height = self.__canvas.winfo_height()
+        if self.xscroll:
+            new_width = max(new_width, self.inner.winfo_reqwidth())
+        if self.yscroll:
+            new_height = max(new_height, self.inner.winfo_reqheight())
+
+        bbox = (0, 0, new_width, new_height)
+        self.__canvas.configure(scrollregion=bbox)
+        self.__canvas.itemconfigure(self.__inner_id, width=new_width, height=new_height)
+
+        self.__update_scrollbar_visibility(self.__xscrollbar)
+        self.__update_scrollbar_visibility(self.__yscrollbar)
+        self.__propagate_scroll_binds(self.inner)
+        self.__update_scroll_edges(bbox, *scroll_edges)
+
+    def __get_scroll_edges(self) -> tuple[bool, bool]:
+        xview = self.__canvas.xview()
+        yview = self.__canvas.yview()
+        scrolled_to_right = xview[1] == 1 and xview[0] != 0
+        scrolled_to_bottom = yview[1] == 1 and yview[0] != 0
+        return scrolled_to_right, scrolled_to_bottom
+
+    def __propagate_scroll_binds(self, parent: Widget):
+        if parent not in self.__scrolled_widgets:
+            parent.bind("<MouseWheel>", self.__on_mouse_yscroll)
+            parent.bind("<Shift-MouseWheel>", self.__on_mouse_xscroll)
+            self.__scrolled_widgets.add(parent)
+
+        for child in parent.winfo_children():
+            self.__propagate_scroll_binds(child)
+
+    def __update_scroll_edges(
+        self,
+        bbox: tuple[int, int, int, int],
+        scrolled_to_right: bool,
+        scrolled_to_bottom: bool,
+    ) -> None:
+        self.__last_scrollregion, last_bbox = bbox, self.__last_scrollregion
+        if not self.autoscroll:
+            return
+        elif bbox == last_bbox:
+            return
+
+        if scrolled_to_right:
+            self.__canvas.xview_moveto(1)
+        if scrolled_to_bottom:
+            self.__canvas.yview_moveto(1)
+
+    def __on_mouse_xscroll(self, event: Event):
+        delta = int(-event.delta / 100)
+        self.__canvas.xview_scroll(delta, "units")
+
+    def __on_mouse_yscroll(self, event: Event):
+        delta = int(-event.delta / 100)
+        self.__canvas.yview_scroll(delta, "units")
+
+    def __update_scrollbar_visibility(self, scrollbar: Scrollbar):
+        if scrollbar.get() == (0, 1):
+            scrollbar.grid_remove()
+        else:
+            scrollbar.grid()
+
+    def __wrap_scrollbar_set(self, scrollbar: Scrollbar):
+        def wrapper(*args, **kwargs):
+            scrollbar.set(*args, **kwargs)
+            self.__update_scrollbar_visibility(scrollbar)
+
+        return wrapper
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/db/connection.py` & `dum-dum-irc-0.4.1/src/dumdum/db/connection.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import contextlib
-import sqlite3
-from abc import ABC, abstractmethod
-from typing import Any, ContextManager, Iterator, Protocol, Self, Sequence
-
-Row = Sequence[Any]
-
-
-class Cursor(Protocol):
-    def fetchone(self) -> Row: ...
-    def fetchall(self) -> Sequence[Row]: ...
-
-
-class Connection(ABC):
-    @abstractmethod
-    def execute(self, query: str, /, *parameters: Any) -> Cursor:
-        """Execute query and return a cursor."""
-
-    @abstractmethod
-    def executescript(self, query: str, /) -> None:
-        """Execute one or more SQL statements."""
-
-    @abstractmethod
-    def transaction(self) -> ContextManager[Self]:
-        """Returns a context manager to begin a transaction."""
-
-    def fetchone(self, query: str, /, *parameters: Any) -> Row | None:
-        """Execute query and return the first row.
-
-        If the results are empty, None is returned.
-
-        """
-        c = self.execute(query, *parameters)
-        return c.fetchone()
-
-    def fetchall(self, query: str, /, *parameters: Any) -> Sequence[Row]:
-        """Execute query and return all rows.
-
-        If the results are empty, None is returned.
-
-        """
-        c = self.execute(query, *parameters)
-        return c.fetchall()
-
-    def fetchval(self, query: str, /, *parameters: Any) -> Any:
-        """Execute query and return the first value of the first row.
-
-        If the results are empty, None is returned.
-
-        """
-        row = self.fetchone(query, *parameters)
-        if row is not None:
-            return row[0]
-
-
-class SQLiteConnection(Connection):
-    def __init__(self, conn: sqlite3.Connection) -> None:
-        self._conn = conn
-
-    def execute(self, query: str, *parameters: Any) -> sqlite3.Cursor:
-        if len(parameters) == 1 and isinstance(parameters[0], (tuple, list, dict)):
-            _params = parameters[0]
-        else:
-            _params = parameters
-
-        return self._conn.execute(query, _params)
-
-    def executescript(self, query: str) -> None:
-        self._conn.executescript(query)
-
-    @contextlib.contextmanager
-    def transaction(self) -> Iterator[Self]:
-        with self._conn:
-            yield self
-
-    @classmethod
-    @contextlib.contextmanager
-    def connect(cls, *args, **kwargs) -> Iterator[Self]:
-        with contextlib.closing(sqlite3.connect(*args, **kwargs)) as conn:
-            yield cls(conn)
+import contextlib
+import sqlite3
+from abc import ABC, abstractmethod
+from typing import Any, ContextManager, Iterator, Protocol, Self, Sequence
+
+Row = Sequence[Any]
+
+
+class Cursor(Protocol):
+    def fetchone(self) -> Row: ...
+    def fetchall(self) -> Sequence[Row]: ...
+
+
+class Connection(ABC):
+    @abstractmethod
+    def execute(self, query: str, /, *parameters: Any) -> Cursor:
+        """Execute query and return a cursor."""
+
+    @abstractmethod
+    def executescript(self, query: str, /) -> None:
+        """Execute one or more SQL statements."""
+
+    @abstractmethod
+    def transaction(self) -> ContextManager[Self]:
+        """Returns a context manager to begin a transaction."""
+
+    def fetchone(self, query: str, /, *parameters: Any) -> Row | None:
+        """Execute query and return the first row.
+
+        If the results are empty, None is returned.
+
+        """
+        c = self.execute(query, *parameters)
+        return c.fetchone()
+
+    def fetchall(self, query: str, /, *parameters: Any) -> Sequence[Row]:
+        """Execute query and return all rows.
+
+        If the results are empty, None is returned.
+
+        """
+        c = self.execute(query, *parameters)
+        return c.fetchall()
+
+    def fetchval(self, query: str, /, *parameters: Any) -> Any:
+        """Execute query and return the first value of the first row.
+
+        If the results are empty, None is returned.
+
+        """
+        row = self.fetchone(query, *parameters)
+        if row is not None:
+            return row[0]
+
+
+class SQLiteConnection(Connection):
+    def __init__(self, conn: sqlite3.Connection) -> None:
+        self._conn = conn
+
+    def execute(self, query: str, *parameters: Any) -> sqlite3.Cursor:
+        if len(parameters) == 1 and isinstance(parameters[0], (tuple, list, dict)):
+            _params = parameters[0]
+        else:
+            _params = parameters
+
+        return self._conn.execute(query, _params)
+
+    def executescript(self, query: str) -> None:
+        self._conn.executescript(query)
+
+    @contextlib.contextmanager
+    def transaction(self) -> Iterator[Self]:
+        with self._conn:
+            yield self
+
+    @classmethod
+    @contextlib.contextmanager
+    def connect(cls, *args, **kwargs) -> Iterator[Self]:
+        with contextlib.closing(sqlite3.connect(*args, **kwargs)) as conn:
+            yield cls(conn)
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/db/migrations.py` & `dum-dum-irc-0.4.1/src/dumdum/db/migrations.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import logging
-import re
-from typing import Literal
-
-import importlib_resources
-
-from .connection import SQLiteConnection
-
-log = logging.getLogger(__name__)
-
-MigrationPath = Literal["client"]
-
-
-def run_migrations(conn: SQLiteConnection, path: MigrationPath):
-    version: int = conn.fetchval("PRAGMA user_version")
-    script_version = version
-
-    for script_version, script in _get_migrations(path, version).items():
-        conn.executescript(script)
-
-    if script_version > version:
-        conn.execute(f"PRAGMA user_version = {script_version}")
-        log.debug("Migrated database v%d to v%d", version, script_version)
-
-
-def _get_migrations(path: MigrationPath, version: int) -> dict[int, str]:
-    migrations: dict[int, str] = {}
-
-    resource = importlib_resources.files(__package__) / "scripts" / path
-    with importlib_resources.as_file(resource) as root:
-        for file in root.glob("*.sql"):
-            m = re.match(r"\d+", file.stem)
-            if m is None:
-                continue
-
-            file_version = int(m[0])
-            if file_version in migrations:
-                raise ValueError(
-                    f"Duplicate migration found for version {file_version}"
-                )
-
-            if file_version <= version:
-                continue
-
-            migrations[file_version] = file.read_text("utf-8")
-
-    return dict(sorted(migrations.items()))
+import logging
+import re
+from typing import Literal
+
+import importlib_resources
+
+from .connection import SQLiteConnection
+
+log = logging.getLogger(__name__)
+
+MigrationPath = Literal["client"]
+
+
+def run_migrations(conn: SQLiteConnection, path: MigrationPath):
+    version: int = conn.fetchval("PRAGMA user_version")
+    script_version = version
+
+    for script_version, script in _get_migrations(path, version).items():
+        conn.executescript(script)
+
+    if script_version > version:
+        conn.execute(f"PRAGMA user_version = {script_version}")
+        log.debug("Migrated database v%d to v%d", version, script_version)
+
+
+def _get_migrations(path: MigrationPath, version: int) -> dict[int, str]:
+    migrations: dict[int, str] = {}
+
+    resource = importlib_resources.files(__package__) / "scripts" / path
+    with importlib_resources.as_file(resource) as root:
+        for file in root.glob("*.sql"):
+            m = re.match(r"\d+", file.stem)
+            if m is None:
+                continue
+
+            file_version = int(m[0])
+            if file_version in migrations:
+                raise ValueError(
+                    f"Duplicate migration found for version {file_version}"
+                )
+
+            if file_version <= version:
+                continue
+
+            migrations[file_version] = file.read_text("utf-8")
+
+    return dict(sorted(migrations.items()))
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/logging.py` & `dum-dum-irc-0.4.1/src/dumdum/logging.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import datetime
-import json
-import logging
-import logging.config
-from typing import Any, Literal
-
-from .appdirs import APP_DIRS
-
-BASE_CONFIG = {
-    "version": 1,
-    "disable_existing_loggers": False,
-    "root": {
-        "level": "DEBUG",
-        "handlers": ["stdout", "file"],
-    },
-    "handlers": {
-        "stdout": {
-            "class": "logging.StreamHandler",
-            "formatter": "text",
-            "stream": "ext://sys.stdout",
-        },
-        "file": {
-            "class": "logging.handlers.RotatingFileHandler",
-            "formatter": "json",
-            "filename": "",  # Filled in by configure_logging()
-            "maxBytes": 5_000_000,
-            "backupCount": 3,
-        },
-    },
-    "formatters": {
-        "text": {
-            "format": "%(message)s",  # Filled in by configure_logging()
-            "datefmt": "%Y-%m-%dT%H:%M:%S%z",
-        },
-        "json": {
-            "()": "dumdum.logging.JSONFormatter",
-        },
-    },
-}
-
-LOG_RECORD_ATTRIBUTES = {
-    "args",
-    "asctime",
-    "created",
-    "exc_info",
-    "exc_text",  # cached by formatException()
-    "filename",
-    "funcName",
-    "levelname",
-    "levelno",
-    "lineno",
-    "message",
-    "module",
-    "msecs",
-    "msg",
-    "name",
-    "pathname",
-    "process",
-    "processName",
-    "relativeCreated",
-    "stack_info",
-    "thread",
-    "threadName",
-    "taskName",
-}
-
-
-def configure_logging(mode: Literal["client", "server"], verbose: int) -> None:
-    config = BASE_CONFIG.copy()
-
-    if verbose == 0:
-        text_format = "%(levelname)s: %(message)s"
-        stdout_level = logging.WARNING
-        file_level = logging.INFO
-    elif verbose == 1:
-        text_format = "%(levelname)s: %(message)s"
-        stdout_level = logging.INFO
-        file_level = logging.INFO
-    else:
-        text_format = "%(levelname)s: %(message)-50s (%(name)s#L%(lineno)d)"
-        stdout_level = logging.DEBUG
-        file_level = logging.DEBUG
-
-    config["formatters"]["text"]["format"] = text_format
-    config["handlers"]["stdout"]["level"] = stdout_level
-    config["handlers"]["file"]["level"] = file_level
-
-    if mode == "server":
-        file_filename = str(APP_DIRS.user_log_path / "dumdum-server.jsonl")
-    else:
-        file_filename = str(APP_DIRS.user_log_path / "dumdum.jsonl")
-
-    config["handlers"]["file"]["filename"] = file_filename
-
-    logging.config.dictConfig(config)
-
-
-class JSONFormatter(logging.Formatter):
-    def format(self, record: logging.LogRecord) -> str:
-        data = self._prepare_record(record)
-        return json.dumps(data, default=str)
-
-    def _prepare_record(self, record: logging.LogRecord) -> dict[str, Any]:
-        data = {}
-
-        for k, v in vars(record).items():
-            if k not in LOG_RECORD_ATTRIBUTES:
-                data[k] = v
-
-        created = datetime.datetime.fromtimestamp(
-            record.created,
-            tz=datetime.timezone.utc,
-        )
-
-        data["created"] = created.isoformat()
-        data["message"] = record.getMessage()
-
-        if record.exc_info is not None:
-            data["exc_info"] = self.formatException(record.exc_info)
-
-        if record.stack_info is not None:
-            data["stack_info"] = self.formatStack(record.stack_info)
-
-        return data
+import datetime
+import json
+import logging
+import logging.config
+from typing import Any, Literal
+
+from .appdirs import APP_DIRS
+
+BASE_CONFIG = {
+    "version": 1,
+    "disable_existing_loggers": False,
+    "root": {
+        "level": "DEBUG",
+        "handlers": ["stdout", "file"],
+    },
+    "handlers": {
+        "stdout": {
+            "class": "logging.StreamHandler",
+            "formatter": "text",
+            "stream": "ext://sys.stdout",
+        },
+        "file": {
+            "class": "logging.handlers.RotatingFileHandler",
+            "formatter": "json",
+            "filename": "",  # Filled in by configure_logging()
+            "maxBytes": 5_000_000,
+            "backupCount": 3,
+        },
+    },
+    "formatters": {
+        "text": {
+            "format": "%(message)s",  # Filled in by configure_logging()
+            "datefmt": "%Y-%m-%dT%H:%M:%S%z",
+        },
+        "json": {
+            "()": "dumdum.logging.JSONFormatter",
+        },
+    },
+}
+
+LOG_RECORD_ATTRIBUTES = {
+    "args",
+    "asctime",
+    "created",
+    "exc_info",
+    "exc_text",  # cached by formatException()
+    "filename",
+    "funcName",
+    "levelname",
+    "levelno",
+    "lineno",
+    "message",
+    "module",
+    "msecs",
+    "msg",
+    "name",
+    "pathname",
+    "process",
+    "processName",
+    "relativeCreated",
+    "stack_info",
+    "thread",
+    "threadName",
+    "taskName",
+}
+
+
+def configure_logging(mode: Literal["client", "server"], verbose: int) -> None:
+    config = BASE_CONFIG.copy()
+
+    if verbose == 0:
+        text_format = "%(levelname)s: %(message)s"
+        stdout_level = logging.WARNING
+        file_level = logging.INFO
+    elif verbose == 1:
+        text_format = "%(levelname)s: %(message)s"
+        stdout_level = logging.INFO
+        file_level = logging.INFO
+    else:
+        text_format = "%(levelname)s: %(message)-50s (%(name)s#L%(lineno)d)"
+        stdout_level = logging.DEBUG
+        file_level = logging.DEBUG
+
+    config["formatters"]["text"]["format"] = text_format
+    config["handlers"]["stdout"]["level"] = stdout_level
+    config["handlers"]["file"]["level"] = file_level
+
+    if mode == "server":
+        file_filename = str(APP_DIRS.user_log_path / "dumdum-server.jsonl")
+    else:
+        file_filename = str(APP_DIRS.user_log_path / "dumdum.jsonl")
+
+    config["handlers"]["file"]["filename"] = file_filename
+
+    logging.config.dictConfig(config)
+
+
+class JSONFormatter(logging.Formatter):
+    def format(self, record: logging.LogRecord) -> str:
+        data = self._prepare_record(record)
+        return json.dumps(data, default=str)
+
+    def _prepare_record(self, record: logging.LogRecord) -> dict[str, Any]:
+        data = {}
+
+        for k, v in vars(record).items():
+            if k not in LOG_RECORD_ATTRIBUTES:
+                data[k] = v
+
+        created = datetime.datetime.fromtimestamp(
+            record.created,
+            tz=datetime.timezone.utc,
+        )
+
+        data["created"] = created.isoformat()
+        data["message"] = record.getMessage()
+
+        if record.exc_info is not None:
+            data["exc_info"] = self.formatException(record.exc_info)
+
+        if record.stack_info is not None:
+            data["stack_info"] = self.formatStack(record.stack_info)
+
+        return data
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/README.md` & `dum-dum-irc-0.4.1/src/dumdum/protocol/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-This contains the [Sans-IO] implementation of the Dumdum protocol.
-
-- [`client/`](client/): Implements the client side of the protocol.
-- [`server/`](server/): Implements the server side of the protocol.
-- [`channel.py`](channel.py): A basic channel dataclass shared between the client and server.
-- [`constants.py`](constants.py): Defines a few constants used by the protocol.
-- [`enums.py`](enums.py): Defines the message types that will be sent between the client and server.
-- [`errors.py`](errors.py): Defines exceptions that the protocol can raise.
-- [`highcommand.py`](highcommand.py): A server-side, in-memory datastore for channels and users.
-- [`interfaces.py`](interfaces.py): Defines a common interface between the client and server.
-- [`reader.py`](reader.py): Provides functions to read through bytes/bytearrays like streams.
-- [`snowflake.py`](snowflake.py): Provides functions to generate snowflake identifiers.
-- [`varchar.py`](varchar.py): Provides functions to de/serialize variable-length strings.
-
-[Sans-IO]: https://sans-io.readthedocs.io/
+This contains the [Sans-IO] implementation of the Dumdum protocol.
+
+- [`client/`](client/): Implements the client side of the protocol.
+- [`server/`](server/): Implements the server side of the protocol.
+- [`channel.py`](channel.py): A basic channel dataclass shared between the client and server.
+- [`constants.py`](constants.py): Defines a few constants used by the protocol.
+- [`enums.py`](enums.py): Defines the message types that will be sent between the client and server.
+- [`errors.py`](errors.py): Defines exceptions that the protocol can raise.
+- [`highcommand.py`](highcommand.py): A server-side, in-memory datastore for channels and users.
+- [`interfaces.py`](interfaces.py): Defines a common interface between the client and server.
+- [`reader.py`](reader.py): Provides functions to read through bytes/bytearrays like streams.
+- [`snowflake.py`](snowflake.py): Provides functions to generate snowflake identifiers.
+- [`varchar.py`](varchar.py): Provides functions to de/serialize variable-length strings.
+
+[Sans-IO]: https://sans-io.readthedocs.io/
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/__init__.py` & `dum-dum-irc-0.4.1/src/dumdum/protocol/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-from .client import (
-    Client,
-    ClientEvent,
-    ClientEventAuthentication,
-    ClientEventChannelsListed,
-    ClientEventHello,
-    ClientEventIncompatibleVersion,
-    ClientEventMessageReceived,
-    ClientEventMessagesListed,
-    ClientMessageAuthenticate,
-    ClientMessageHello,
-    ClientMessageListChannels,
-    ClientMessageListMessages,
-    ClientMessagePost,
-    ClientState,
-)
-from .server import (
-    Server,
-    ServerEvent,
-    ServerEventAuthentication,
-    ServerEventHello,
-    ServerEventIncompatibleVersion,
-    ServerEventListChannels,
-    ServerEventListMessages,
-    ServerEventMessageReceived,
-    ServerMessageAcknowledgeAuthentication,
-    ServerMessageHello,
-    ServerMessageListChannels,
-    ServerMessageListMessages,
-    ServerMessagePost,
-    ServerMessageSendIncompatibleVersion,
-    ServerState,
-)
-from .channel import Channel
-from .constants import MAX_MESSAGE_LENGTH, MAX_NICK_LENGTH
-from .enums import ClientMessageType, ServerMessageType
-from .errors import (
-    InvalidLengthError,
-    InvalidStateError,
-    MalformedDataError,
-    ProtocolError,
-)
-from .interfaces import Protocol
-from .message import Message
-from .reader import Reader, bytearray_reader, byte_reader
-from .snowflake import create_snowflake
+from .client import (
+    Client,
+    ClientEvent,
+    ClientEventAuthentication,
+    ClientEventChannelsListed,
+    ClientEventHello,
+    ClientEventIncompatibleVersion,
+    ClientEventMessageReceived,
+    ClientEventMessagesListed,
+    ClientMessageAuthenticate,
+    ClientMessageHello,
+    ClientMessageListChannels,
+    ClientMessageListMessages,
+    ClientMessagePost,
+    ClientState,
+)
+from .server import (
+    Server,
+    ServerEvent,
+    ServerEventAuthentication,
+    ServerEventHello,
+    ServerEventIncompatibleVersion,
+    ServerEventListChannels,
+    ServerEventListMessages,
+    ServerEventMessageReceived,
+    ServerMessageAcknowledgeAuthentication,
+    ServerMessageHello,
+    ServerMessageListChannels,
+    ServerMessageListMessages,
+    ServerMessagePost,
+    ServerMessageSendIncompatibleVersion,
+    ServerState,
+)
+from .buffer import extend_limited_buffer
+from .channel import Channel
+from .constants import MAX_MESSAGE_LENGTH, MAX_NICK_LENGTH
+from .enums import ClientMessageType, ServerMessageType
+from .errors import (
+    BufferOverflowError,
+    InvalidLengthError,
+    InvalidStateError,
+    MalformedDataError,
+    ProtocolError,
+)
+from .interfaces import Protocol
+from .message import Message
+from .reader import Reader, bytearray_reader, byte_reader
+from .snowflake import create_snowflake
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/client/messages.py` & `dum-dum-irc-0.4.1/src/dumdum/protocol/client/messages.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from dataclasses import dataclass
-
-from dumdum.protocol import varchar
-from dumdum.protocol.constants import (
-    MAX_CHANNEL_NAME_LENGTH,
-    MAX_MESSAGE_LENGTH,
-    MAX_NICK_LENGTH,
-)
-from dumdum.protocol.enums import ClientMessageType
-
-
-@dataclass
-class ClientMessageHello:
-    version: int
-
-    def __bytes__(self) -> bytes:
-        return bytes(
-            [
-                ClientMessageType.HELLO.value,
-                self.version,
-            ]
-        )
-
-
-@dataclass
-class ClientMessageAuthenticate:
-    nick: str
-
-    def __bytes__(self) -> bytes:
-        return bytes(
-            [
-                ClientMessageType.AUTHENTICATE.value,
-                *varchar.dumps(self.nick, max_length=MAX_NICK_LENGTH),
-            ]
-        )
-
-
-@dataclass
-class ClientMessagePost:
-    channel_name: str
-    content: str
-
-    def __bytes__(self) -> bytes:
-        return bytes(
-            [
-                ClientMessageType.SEND_MESSAGE.value,
-                *varchar.dumps(self.channel_name, max_length=MAX_CHANNEL_NAME_LENGTH),
-                *varchar.dumps(self.content, max_length=MAX_MESSAGE_LENGTH),
-            ]
-        )
-
-
-@dataclass
-class ClientMessageListChannels:
-    def __bytes__(self) -> bytes:
-        return bytes([ClientMessageType.LIST_CHANNELS.value])
-
-
-@dataclass
-class ClientMessageListMessages:
-    channel_name: str
-    before: int | None
-    after: int | None
-
-    def __bytes__(self) -> bytes:
-        before = self.before or 0
-        after = self.after or 0
-        return bytes(
-            [
-                ClientMessageType.LIST_MESSAGES.value,
-                *varchar.dumps(self.channel_name, max_length=MAX_CHANNEL_NAME_LENGTH),
-                *before.to_bytes(8, byteorder="big"),
-                *after.to_bytes(8, byteorder="big"),
-            ]
-        )
+from dataclasses import dataclass
+
+from dumdum.protocol import varchar
+from dumdum.protocol.constants import (
+    MAX_CHANNEL_NAME_LENGTH,
+    MAX_MESSAGE_LENGTH,
+    MAX_NICK_LENGTH,
+)
+from dumdum.protocol.enums import ClientMessageType
+
+
+@dataclass
+class ClientMessageHello:
+    version: int
+
+    def __bytes__(self) -> bytes:
+        return bytes(
+            [
+                ClientMessageType.HELLO.value,
+                self.version,
+            ]
+        )
+
+
+@dataclass
+class ClientMessageAuthenticate:
+    nick: str
+
+    def __bytes__(self) -> bytes:
+        return bytes(
+            [
+                ClientMessageType.AUTHENTICATE.value,
+                *varchar.dumps(self.nick, max_length=MAX_NICK_LENGTH),
+            ]
+        )
+
+
+@dataclass
+class ClientMessagePost:
+    channel_name: str
+    content: str
+
+    def __bytes__(self) -> bytes:
+        return bytes(
+            [
+                ClientMessageType.SEND_MESSAGE.value,
+                *varchar.dumps(self.channel_name, max_length=MAX_CHANNEL_NAME_LENGTH),
+                *varchar.dumps(self.content, max_length=MAX_MESSAGE_LENGTH),
+            ]
+        )
+
+
+@dataclass
+class ClientMessageListChannels:
+    def __bytes__(self) -> bytes:
+        return bytes([ClientMessageType.LIST_CHANNELS.value])
+
+
+@dataclass
+class ClientMessageListMessages:
+    channel_name: str
+    before: int | None
+    after: int | None
+
+    def __bytes__(self) -> bytes:
+        before = self.before or 0
+        after = self.after or 0
+        return bytes(
+            [
+                ClientMessageType.LIST_MESSAGES.value,
+                *varchar.dumps(self.channel_name, max_length=MAX_CHANNEL_NAME_LENGTH),
+                *before.to_bytes(8, byteorder="big"),
+                *after.to_bytes(8, byteorder="big"),
+            ]
+        )
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/message.py` & `dum-dum-irc-0.4.1/src/dumdum/protocol/message.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from dataclasses import dataclass
-from typing import Self
-
-from . import varchar
-from .constants import MAX_CHANNEL_NAME_LENGTH, MAX_MESSAGE_LENGTH, MAX_NICK_LENGTH
-from .reader import Reader
-
-
-@dataclass
-class Message:
-    id: int
-    channel_name: str
-    nick: str
-    content: str
-
-    def __bytes__(self) -> bytes:
-        return bytes(
-            [
-                *self.id.to_bytes(8, byteorder="big"),
-                *varchar.dumps(self.channel_name, max_length=MAX_CHANNEL_NAME_LENGTH),
-                *varchar.dumps(self.nick, max_length=MAX_NICK_LENGTH),
-                *varchar.dumps(self.content, max_length=MAX_MESSAGE_LENGTH),
-            ]
-        )
-
-    @classmethod
-    def from_reader(cls, reader: Reader) -> Self:
-        id = reader.read_bigint()
-        channel_name = reader.read_varchar(max_length=MAX_CHANNEL_NAME_LENGTH)
-        nick = reader.read_varchar(max_length=MAX_NICK_LENGTH)
-        content = reader.read_varchar(max_length=MAX_MESSAGE_LENGTH)
-        return cls(id=id, channel_name=channel_name, nick=nick, content=content)
+from dataclasses import dataclass
+from typing import Self
+
+from . import varchar
+from .constants import MAX_CHANNEL_NAME_LENGTH, MAX_MESSAGE_LENGTH, MAX_NICK_LENGTH
+from .reader import Reader
+
+
+@dataclass
+class Message:
+    id: int
+    channel_name: str
+    nick: str
+    content: str
+
+    def __bytes__(self) -> bytes:
+        return bytes(
+            [
+                *self.id.to_bytes(8, byteorder="big"),
+                *varchar.dumps(self.channel_name, max_length=MAX_CHANNEL_NAME_LENGTH),
+                *varchar.dumps(self.nick, max_length=MAX_NICK_LENGTH),
+                *varchar.dumps(self.content, max_length=MAX_MESSAGE_LENGTH),
+            ]
+        )
+
+    @classmethod
+    def from_reader(cls, reader: Reader) -> Self:
+        id = reader.read_bigint()
+        channel_name = reader.read_varchar(max_length=MAX_CHANNEL_NAME_LENGTH)
+        nick = reader.read_varchar(max_length=MAX_NICK_LENGTH)
+        content = reader.read_varchar(max_length=MAX_MESSAGE_LENGTH)
+        return cls(id=id, channel_name=channel_name, nick=nick, content=content)
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/reader.py` & `dum-dum-irc-0.4.1/src/dumdum/protocol/reader.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import contextlib
-from typing import Iterator
-
-from dumdum.protocol import varchar
-
-
-class Reader:
-    def __init__(self, buffer: bytearray | bytes) -> None:
-        self.buffer = buffer
-        self._index = 0
-        self._closed = False
-
-    def read(self, n: int = -1) -> bytes:
-        if self._closed:
-            raise RuntimeError("Cannot read from closed reader")
-
-        if n < 0:
-            n = len(self.buffer)
-        else:
-            n = min(n, len(self.buffer))
-
-        start, self._index = self._index, self._index + n
-        return self.buffer[start : self._index]
-
-    def readexactly(self, n: int) -> bytes:
-        if n < 0:
-            raise ValueError(f"n must be 0 or greater, not {n}")
-
-        data = self.read(n)
-        if len(data) != n:
-            raise IndexError(
-                f"Insufficent data to read (expected {n}, got {len(data)})"
-            )
-
-        return data
-
-    def read_bigint(self) -> int:
-        data = self.readexactly(8)
-        return int.from_bytes(data, byteorder="big")
-
-    def read_varchar(self, *, max_length: int) -> str:
-        return varchar.load(self, max_length=max_length)
-
-    def close(self) -> None:
-        self._closed = True
-
-
-@contextlib.contextmanager
-def bytearray_reader(buffer: bytearray) -> Iterator[Reader]:
-    reader = Reader(buffer)
-
-    try:
-        yield reader
-    finally:
-        reader.close()
-
-    buffer[: reader._index] = b""
-
-
-@contextlib.contextmanager
-def byte_reader(buffer: bytes) -> Iterator[Reader]:
-    reader = Reader(buffer)
-
-    try:
-        yield reader
-    finally:
-        reader.close()
+import contextlib
+from typing import Iterator
+
+from dumdum.protocol import varchar
+
+
+class Reader:
+    def __init__(self, buffer: bytearray | bytes) -> None:
+        self.buffer = buffer
+        self._index = 0
+        self._closed = False
+
+    def read(self, n: int = -1) -> bytes:
+        if self._closed:
+            raise RuntimeError("Cannot read from closed reader")
+
+        if n < 0:
+            n = len(self.buffer)
+        else:
+            n = min(n, len(self.buffer))
+
+        start, self._index = self._index, self._index + n
+        return self.buffer[start : self._index]
+
+    def readexactly(self, n: int) -> bytes:
+        if n < 0:
+            raise ValueError(f"n must be 0 or greater, not {n}")
+
+        data = self.read(n)
+        if len(data) != n:
+            raise IndexError(
+                f"Insufficent data to read (expected {n}, got {len(data)})"
+            )
+
+        return data
+
+    def read_bigint(self) -> int:
+        data = self.readexactly(8)
+        return int.from_bytes(data, byteorder="big")
+
+    def read_varchar(self, *, max_length: int) -> str:
+        return varchar.load(self, max_length=max_length)
+
+    def close(self) -> None:
+        self._closed = True
+
+
+@contextlib.contextmanager
+def bytearray_reader(buffer: bytearray) -> Iterator[Reader]:
+    reader = Reader(buffer)
+
+    try:
+        yield reader
+    finally:
+        reader.close()
+
+    buffer[: reader._index] = b""
+
+
+@contextlib.contextmanager
+def byte_reader(buffer: bytes) -> Iterator[Reader]:
+    reader = Reader(buffer)
+
+    try:
+        yield reader
+    finally:
+        reader.close()
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/server/messages.py` & `dum-dum-irc-0.4.1/src/dumdum/protocol/server/messages.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-from dataclasses import dataclass
-from typing import Sequence
-
-from dumdum.protocol.channel import Channel
-from dumdum.protocol.constants import (
-    MAX_LIST_CHANNEL_LENGTH_BYTES,
-    MAX_LIST_MESSAGE_LENGTH_BYTES,
-)
-from dumdum.protocol.enums import ServerMessageType
-from dumdum.protocol.message import Message
-
-
-@dataclass
-class ServerMessageHello:
-    using_ssl: bool
-
-    def __bytes__(self) -> bytes:
-        return bytes([ServerMessageType.HELLO.value, self.using_ssl])
-
-
-@dataclass
-class ServerMessageSendIncompatibleVersion:
-    required: int
-
-    def __bytes__(self) -> bytes:
-        return bytes(
-            [
-                ServerMessageType.INCOMPATIBLE_VERSION.value,
-                self.required,
-            ]
-        )
-
-
-@dataclass
-class ServerMessageAcknowledgeAuthentication:
-    success: bool
-
-    def __bytes__(self) -> bytes:
-        return bytes(
-            [
-                ServerMessageType.ACKNOWLEDGE_AUTHENTICATION.value,
-                self.success,
-            ]
-        )
-
-
-@dataclass
-class ServerMessagePost:
-    message: Message
-
-    def __bytes__(self) -> bytes:
-        return bytes(
-            [
-                ServerMessageType.SEND_MESSAGE.value,
-                *bytes(self.message),
-            ]
-        )
-
-
-@dataclass
-class ServerMessageListChannels:
-    channels: Sequence[Channel]
-
-    def __bytes__(self) -> bytes:
-        channel_bytes = b"".join(bytes(c) for c in self.channels)
-        channel_length = len(channel_bytes).to_bytes(
-            MAX_LIST_CHANNEL_LENGTH_BYTES,
-            byteorder="big",
-        )
-        return bytes(
-            [
-                ServerMessageType.LIST_CHANNELS.value,
-                *channel_length,
-                *channel_bytes,
-            ]
-        )
-
-
-@dataclass
-class ServerMessageListMessages:
-    messages: Sequence[Message]
-
-    def __bytes__(self) -> bytes:
-        message_bytes = b"".join(bytes(c) for c in self.messages)
-        message_length = len(message_bytes).to_bytes(
-            MAX_LIST_MESSAGE_LENGTH_BYTES,
-            byteorder="big",
-        )
-        return bytes(
-            [
-                ServerMessageType.LIST_MESSAGES.value,
-                *message_length,
-                *message_bytes,
-            ]
-        )
+from dataclasses import dataclass
+from typing import Sequence
+
+from dumdum.protocol.channel import Channel
+from dumdum.protocol.constants import (
+    MAX_LIST_CHANNEL_LENGTH_BYTES,
+    MAX_LIST_MESSAGE_LENGTH_BYTES,
+)
+from dumdum.protocol.enums import ServerMessageType
+from dumdum.protocol.message import Message
+
+
+@dataclass
+class ServerMessageHello:
+    using_ssl: bool
+
+    def __bytes__(self) -> bytes:
+        return bytes([ServerMessageType.HELLO.value, self.using_ssl])
+
+
+@dataclass
+class ServerMessageSendIncompatibleVersion:
+    required: int
+
+    def __bytes__(self) -> bytes:
+        return bytes(
+            [
+                ServerMessageType.INCOMPATIBLE_VERSION.value,
+                self.required,
+            ]
+        )
+
+
+@dataclass
+class ServerMessageAcknowledgeAuthentication:
+    success: bool
+
+    def __bytes__(self) -> bytes:
+        return bytes(
+            [
+                ServerMessageType.ACKNOWLEDGE_AUTHENTICATION.value,
+                self.success,
+            ]
+        )
+
+
+@dataclass
+class ServerMessagePost:
+    message: Message
+
+    def __bytes__(self) -> bytes:
+        return bytes(
+            [
+                ServerMessageType.SEND_MESSAGE.value,
+                *bytes(self.message),
+            ]
+        )
+
+
+@dataclass
+class ServerMessageListChannels:
+    channels: Sequence[Channel]
+
+    def __bytes__(self) -> bytes:
+        channel_bytes = b"".join(bytes(c) for c in self.channels)
+        channel_length = len(channel_bytes).to_bytes(
+            MAX_LIST_CHANNEL_LENGTH_BYTES,
+            byteorder="big",
+        )
+        return bytes(
+            [
+                ServerMessageType.LIST_CHANNELS.value,
+                *channel_length,
+                *channel_bytes,
+            ]
+        )
+
+
+@dataclass
+class ServerMessageListMessages:
+    messages: Sequence[Message]
+
+    def __bytes__(self) -> bytes:
+        message_bytes = b"".join(bytes(c) for c in self.messages)
+        message_length = len(message_bytes).to_bytes(
+            MAX_LIST_MESSAGE_LENGTH_BYTES,
+            byteorder="big",
+        )
+        return bytes(
+            [
+                ServerMessageType.LIST_MESSAGES.value,
+                *message_length,
+                *message_bytes,
+            ]
+        )
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/server/protocol.py` & `dum-dum-irc-0.4.1/src/dumdum/protocol/server/protocol.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,162 @@
-from enum import Enum
-from typing import Sequence
-
-from dumdum.protocol.channel import Channel
-from dumdum.protocol.constants import (
-    MAX_CHANNEL_NAME_LENGTH,
-    MAX_MESSAGE_LENGTH,
-    MAX_NICK_LENGTH,
-)
-from dumdum.protocol.enums import ClientMessageType
-from dumdum.protocol.errors import InvalidStateError, MalformedDataError
-from dumdum.protocol.interfaces import Protocol
-from dumdum.protocol.message import Message
-from dumdum.protocol.reader import Reader, bytearray_reader
-
-from .events import (
-    ServerEvent,
-    ServerEventAuthentication,
-    ServerEventHello,
-    ServerEventIncompatibleVersion,
-    ServerEventListChannels,
-    ServerEventListMessages,
-    ServerEventMessageReceived,
-)
-from .messages import (
-    ServerMessageAcknowledgeAuthentication,
-    ServerMessageHello,
-    ServerMessageListChannels,
-    ServerMessageListMessages,
-    ServerMessagePost,
-    ServerMessageSendIncompatibleVersion,
-)
-
-ParsedData = tuple[list[ServerEvent], bytes]
-
-
-class ServerState(Enum):
-    AWAITING_HELLO = 0
-    AWAITING_AUTHENTICATION = 1
-    READY = 2
-
-
-class Server(Protocol):
-    """The server for a single client."""
-
-    PROTOCOL_VERSION = 2
-
-    def __init__(self) -> None:
-        self._buffer = bytearray()
-        self._state = ServerState.AWAITING_HELLO
-
-    def receive_bytes(self, data: bytes) -> ParsedData:
-        self._buffer.extend(data)
-        return self._maybe_parse_buffer()
-
-    def hello(self, *, using_ssl: bool) -> bytes:
-        self._assert_state(ServerState.AWAITING_AUTHENTICATION)
-        return bytes(ServerMessageHello(using_ssl))
-
-    def authenticate(self, *, success: bool) -> bytes:
-        self._assert_state(ServerState.AWAITING_AUTHENTICATION)
-
-        if success:
-            self._state = ServerState.READY
-
-        return bytes(ServerMessageAcknowledgeAuthentication(success))
-
-    def send_message(self, message: Message) -> bytes:
-        self._assert_state(ServerState.READY)
-        return bytes(ServerMessagePost(message))
-
-    def list_channels(self, channels: Sequence[Channel]) -> bytes:
-        return bytes(ServerMessageListChannels(channels))
-
-    def list_messages(self, messages: Sequence[Message]) -> bytes:
-        return bytes(ServerMessageListMessages(messages))
-
-    def _assert_state(self, *states: ServerState) -> None:
-        if self._state not in states:
-            raise InvalidStateError(self._state, states)
-
-    def _maybe_parse_buffer(self) -> ParsedData:
-        full_events: list[ServerEvent] = []
-        full_outgoing = bytearray()
-
-        try:
-            while True:
-                with bytearray_reader(self._buffer) as reader:
-                    events, outgoing = self._read_message(reader)
-
-                full_events.extend(events)
-                full_outgoing.extend(outgoing)
-        except (IndexError, ValueError) as e:
-            # FIXME: this is making stuff hard to debug...
-            if isinstance(e, UnicodeDecodeError):
-                raise MalformedDataError(str(e)) from e
-
-        return full_events, bytes(full_outgoing)
-
-    def _read_message(self, reader: Reader) -> ParsedData:
-        n = reader.readexactly(1)[0]
-        try:
-            t = ClientMessageType(n)
-        except ValueError:
-            raise MalformedDataError(f"Unknown message type {n}") from None
-
-        if t == ClientMessageType.HELLO:
-            return self._parse_hello(reader)
-        elif t == ClientMessageType.AUTHENTICATE:
-            return self._authenticate(reader)
-        elif t == ClientMessageType.SEND_MESSAGE:
-            return self._send_message(reader)
-        elif t == ClientMessageType.LIST_CHANNELS:
-            return self._list_channels(reader)
-        elif t == ClientMessageType.LIST_MESSAGES:
-            return self._list_messages(reader)
-
-        raise RuntimeError(f"No handler for {t}")  # pragma: no cover
-
-    def _parse_hello(self, reader: Reader) -> ParsedData:
-        self._assert_state(ServerState.AWAITING_HELLO)
-
-        version = reader.readexactly(1)[0]
-        if version != self.PROTOCOL_VERSION:
-            event = ServerEventIncompatibleVersion(version)
-            response = ServerMessageSendIncompatibleVersion(self.PROTOCOL_VERSION)
-            return [event], bytes(response)
-
-        event = ServerEventHello()
-        self._state = ServerState.AWAITING_AUTHENTICATION
-        return [event], b""
-
-    def _authenticate(self, reader: Reader) -> ParsedData:
-        self._assert_state(ServerState.AWAITING_AUTHENTICATION)
-        nick = reader.read_varchar(max_length=MAX_NICK_LENGTH)
-        event = ServerEventAuthentication(nick=nick)
-        return [event], b""
-
-    def _send_message(self, reader: Reader) -> ParsedData:
-        self._assert_state(ServerState.READY)
-        channel_name = reader.read_varchar(max_length=MAX_CHANNEL_NAME_LENGTH)
-        content = reader.read_varchar(max_length=MAX_MESSAGE_LENGTH)
-
-        event = ServerEventMessageReceived(channel_name, content)
-        # TODO: broadcast message to all users
-        return [event], b""
-
-    def _list_channels(self, reader: Reader) -> ParsedData:
-        self._assert_state(ServerState.READY)
-        event = ServerEventListChannels()
-        return [event], b""
-
-    def _list_messages(self, reader: Reader) -> ParsedData:
-        self._assert_state(ServerState.READY)
-        channel_name = reader.read_varchar(max_length=MAX_CHANNEL_NAME_LENGTH)
-        before = reader.read_bigint() or None
-        after = reader.read_bigint() or None
-        event = ServerEventListMessages(channel_name, before, after)
-        return [event], b""
+from enum import Enum
+from typing import Sequence
+
+from dumdum.protocol.buffer import extend_limited_buffer
+from dumdum.protocol.channel import Channel
+from dumdum.protocol.constants import (
+    MAX_CHANNEL_NAME_LENGTH,
+    MAX_MESSAGE_LENGTH,
+    MAX_NICK_LENGTH,
+)
+from dumdum.protocol.enums import ClientMessageType
+from dumdum.protocol.errors import InvalidStateError, MalformedDataError
+from dumdum.protocol.interfaces import Protocol
+from dumdum.protocol.message import Message
+from dumdum.protocol.reader import Reader, bytearray_reader
+
+from .events import (
+    ServerEvent,
+    ServerEventAuthentication,
+    ServerEventHello,
+    ServerEventIncompatibleVersion,
+    ServerEventListChannels,
+    ServerEventListMessages,
+    ServerEventMessageReceived,
+)
+from .messages import (
+    ServerMessageAcknowledgeAuthentication,
+    ServerMessageHello,
+    ServerMessageListChannels,
+    ServerMessageListMessages,
+    ServerMessagePost,
+    ServerMessageSendIncompatibleVersion,
+)
+
+ParsedData = tuple[list[ServerEvent], bytes]
+
+
+class ServerState(Enum):
+    AWAITING_HELLO = 0
+    AWAITING_AUTHENTICATION = 1
+    READY = 2
+
+
+class Server(Protocol):
+    """The server for a single client."""
+
+    PROTOCOL_VERSION = 2
+
+    def __init__(self, *, buffer_size: int | None = 2**20) -> None:
+        self.buffer_size = buffer_size
+
+        self._buffer = bytearray()
+        self._state = ServerState.AWAITING_HELLO
+
+    def receive_bytes(self, data: bytes) -> ParsedData:
+        extend_limited_buffer(self._buffer, data, limit=self.buffer_size)
+        return self._maybe_parse_buffer()
+
+    def hello(self, *, using_ssl: bool) -> bytes:
+        self._assert_state(ServerState.AWAITING_AUTHENTICATION)
+        return bytes(ServerMessageHello(using_ssl))
+
+    def authenticate(self, *, success: bool) -> bytes:
+        self._assert_state(ServerState.AWAITING_AUTHENTICATION)
+
+        if success:
+            self._state = ServerState.READY
+
+        return bytes(ServerMessageAcknowledgeAuthentication(success))
+
+    def send_message(self, message: Message) -> bytes:
+        self._assert_state(ServerState.READY)
+        return bytes(ServerMessagePost(message))
+
+    def list_channels(self, channels: Sequence[Channel]) -> bytes:
+        return bytes(ServerMessageListChannels(channels))
+
+    def list_messages(self, messages: Sequence[Message]) -> bytes:
+        return bytes(ServerMessageListMessages(messages))
+
+    def _assert_state(self, *states: ServerState) -> None:
+        if self._state not in states:
+            raise InvalidStateError(self._state, states)
+
+    def _maybe_parse_buffer(self) -> ParsedData:
+        full_events: list[ServerEvent] = []
+        full_outgoing = bytearray()
+
+        try:
+            while True:
+                with bytearray_reader(self._buffer) as reader:
+                    events, outgoing = self._read_message(reader)
+
+                full_events.extend(events)
+                full_outgoing.extend(outgoing)
+        except (IndexError, ValueError) as e:
+            # FIXME: this is making stuff hard to debug...
+            if isinstance(e, UnicodeDecodeError):
+                raise MalformedDataError(str(e)) from e
+
+        return full_events, bytes(full_outgoing)
+
+    def _read_message(self, reader: Reader) -> ParsedData:
+        n = reader.readexactly(1)[0]
+        try:
+            t = ClientMessageType(n)
+        except ValueError:
+            raise MalformedDataError(f"Unknown message type {n}") from None
+
+        if t == ClientMessageType.HELLO:
+            return self._parse_hello(reader)
+        elif t == ClientMessageType.AUTHENTICATE:
+            return self._authenticate(reader)
+        elif t == ClientMessageType.SEND_MESSAGE:
+            return self._send_message(reader)
+        elif t == ClientMessageType.LIST_CHANNELS:
+            return self._list_channels(reader)
+        elif t == ClientMessageType.LIST_MESSAGES:
+            return self._list_messages(reader)
+
+        raise RuntimeError(f"No handler for {t}")  # pragma: no cover
+
+    def _parse_hello(self, reader: Reader) -> ParsedData:
+        self._assert_state(ServerState.AWAITING_HELLO)
+
+        version = reader.readexactly(1)[0]
+        if version != self.PROTOCOL_VERSION:
+            event = ServerEventIncompatibleVersion(version)
+            response = ServerMessageSendIncompatibleVersion(self.PROTOCOL_VERSION)
+            return [event], bytes(response)
+
+        event = ServerEventHello()
+        self._state = ServerState.AWAITING_AUTHENTICATION
+        return [event], b""
+
+    def _authenticate(self, reader: Reader) -> ParsedData:
+        self._assert_state(ServerState.AWAITING_AUTHENTICATION)
+        nick = reader.read_varchar(max_length=MAX_NICK_LENGTH)
+        event = ServerEventAuthentication(nick=nick)
+        return [event], b""
+
+    def _send_message(self, reader: Reader) -> ParsedData:
+        self._assert_state(ServerState.READY)
+        channel_name = reader.read_varchar(max_length=MAX_CHANNEL_NAME_LENGTH)
+        content = reader.read_varchar(max_length=MAX_MESSAGE_LENGTH)
+
+        event = ServerEventMessageReceived(channel_name, content)
+        # TODO: broadcast message to all users
+        return [event], b""
+
+    def _list_channels(self, reader: Reader) -> ParsedData:
+        self._assert_state(ServerState.READY)
+        event = ServerEventListChannels()
+        return [event], b""
+
+    def _list_messages(self, reader: Reader) -> ParsedData:
+        self._assert_state(ServerState.READY)
+        channel_name = reader.read_varchar(max_length=MAX_CHANNEL_NAME_LENGTH)
+        before = reader.read_bigint() or None
+        after = reader.read_bigint() or None
+        event = ServerEventListMessages(channel_name, before, after)
+        return [event], b""
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/snowflake.py` & `dum-dum-irc-0.4.1/src/dumdum/protocol/snowflake.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""
-64 63                                           19     12           0
- 0  00011000111000111000000101110101101101000100 1110101 000000000111
-
-64-63: Always 0
-63-19: Unix timestamp in milliseconds
-19-12: Process ID
-12-00: Incrementing per-process ID
-"""
-
-import datetime
-import os
-import time
-
-_incrementing_id = 0
-
-
-def create_snowflake(
-    t: float | int | datetime.datetime | None = None,
-    pid: int | None = None,
-    increment: int | None = None,
-) -> int:
-    if t is None:
-        # WARNING: this may roll back or forwards depending on system time
-        t = time.time_ns() // 1000000
-    elif isinstance(t, datetime.datetime):
-        t = int(t.timestamp() * 1000)
-    elif isinstance(t, float):
-        t = int(t * 1000)
-
-    if t.bit_length() > 44:
-        raise OverflowError(f"Timestamp {t} out of bounds (are we in 2527?)")
-
-    if pid is None:
-        pid = os.getpid()
-
-    if increment is None:
-        global _incrementing_id
-        increment = _incrementing_id
-        _incrementing_id += 1
-
-    pid = pid % 128
-    increment = increment % 4096
-
-    return (t << 19) + (pid << 12) + increment
+"""
+64 63                                           19     12           0
+ 0  00011000111000111000000101110101101101000100 1110101 000000000111
+
+64-63: Always 0
+63-19: Unix timestamp in milliseconds
+19-12: Process ID
+12-00: Incrementing per-process ID
+"""
+
+import datetime
+import os
+import time
+
+_incrementing_id = 0
+
+
+def create_snowflake(
+    t: float | int | datetime.datetime | None = None,
+    pid: int | None = None,
+    increment: int | None = None,
+) -> int:
+    if t is None:
+        # WARNING: this may roll back or forwards depending on system time
+        t = time.time_ns() // 1000000
+    elif isinstance(t, datetime.datetime):
+        t = int(t.timestamp() * 1000)
+    elif isinstance(t, float):
+        t = int(t * 1000)
+
+    if t.bit_length() > 44:
+        raise OverflowError(f"Timestamp {t} out of bounds (are we in 2527?)")
+
+    if pid is None:
+        pid = os.getpid()
+
+    if increment is None:
+        global _incrementing_id
+        increment = _incrementing_id
+        _incrementing_id += 1
+
+    pid = pid % 128
+    increment = increment % 4096
+
+    return (t << 19) + (pid << 12) + increment
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/protocol/varchar.py` & `dum-dum-irc-0.4.1/src/dumdum/protocol/varchar.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import math
-from io import BytesIO
-from typing import Protocol
-
-from .errors import InvalidLengthError
-
-
-class _Readable(Protocol):
-    def read(self, n: int, /) -> bytes: ...
-
-
-def load(f: _Readable, *, max_length: int) -> str:
-    byte_count = math.ceil(max_length.bit_length() / 8)
-    length_bytes = f.read(byte_count)
-    if len(length_bytes) != byte_count:
-        raise IndexError(f"Insufficient bytes for {max_length = }")
-
-    length = int.from_bytes(length_bytes, byteorder="big")
-    if length > max_length:
-        raise InvalidLengthError(length, max_length)
-
-    message = f.read(length)
-    if length != len(message):
-        raise IndexError(f"Insufficient bytes for {max_length = }")
-
-    return message.decode()
-
-
-def loads(message: bytes, *, max_length: int) -> str:
-    return load(BytesIO(message), max_length=max_length)
-
-
-def dumps(message: str, *, max_length: int) -> bytes:
-    message_bytes = message.encode()
-
-    length = len(message_bytes)
-    if length > max_length:
-        raise InvalidLengthError(length, max_length)
-
-    byte_count = math.ceil(max_length.bit_length() / 8)
-    length_bytes = len(message_bytes).to_bytes(byte_count, byteorder="big")
-
-    return length_bytes + message_bytes
+import math
+from io import BytesIO
+from typing import Protocol
+
+from .errors import InvalidLengthError
+
+
+class _Readable(Protocol):
+    def read(self, n: int, /) -> bytes: ...
+
+
+def load(f: _Readable, *, max_length: int) -> str:
+    byte_count = math.ceil(max_length.bit_length() / 8)
+    length_bytes = f.read(byte_count)
+    if len(length_bytes) != byte_count:
+        raise IndexError(f"Insufficient bytes for {max_length = }")
+
+    length = int.from_bytes(length_bytes, byteorder="big")
+    if length > max_length:
+        raise InvalidLengthError(length, max_length)
+
+    message = f.read(length)
+    if length != len(message):
+        raise IndexError(f"Insufficient bytes for {max_length = }")
+
+    return message.decode()
+
+
+def loads(message: bytes, *, max_length: int) -> str:
+    return load(BytesIO(message), max_length=max_length)
+
+
+def dumps(message: str, *, max_length: int) -> bytes:
+    message_bytes = message.encode()
+
+    length = len(message_bytes)
+    if length > max_length:
+        raise InvalidLengthError(length, max_length)
+
+    byte_count = math.ceil(max_length.bit_length() / 8)
+    length_bytes = len(message_bytes).to_bytes(byte_count, byteorder="big")
+
+    return length_bytes + message_bytes
```

### Comparing `dum-dum-irc-0.4.0.post1/src/dumdum/server/__main__.py` & `dum-dum-irc-0.4.1/src/dumdum/server/__main__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-"""Host a dumdum server.
-
-To use TLS encryption, you must provide a certificate and private key.
-This can be specified as either:
-1. A single file containing both the private key and certificate:
-     --cert hello.pem
-2. A pair of certificate and private key files, separated with a colon:
-     --cert hello.crt:hello.key
-
-"""
-
-import argparse
-import asyncio
-import ssl
-
-from dumdum.protocol import Channel
-from dumdum.logging import configure_logging
-
-from .manager import host_server
-from .state import ServerState
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description=__doc__,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="count",
-        default=0,
-        help="Increase logging verbosity",
-    )
-    parser.add_argument(
-        "-c",
-        "--channels",
-        action="extend",
-        nargs="+",
-        help="A list of channels",
-        type=parse_channel,
-    )
-    parser.add_argument(
-        "--host",
-        default=None,
-        help="The address to host on",
-    )
-    parser.add_argument(
-        "--port",
-        default=6667,
-        help="The port number to host on",
-    )
-    parser.add_argument(
-        "--cert",
-        default="",
-        help="The SSL certificate and private key to use",
-        type=parse_cert,
-    )
-
-    args = parser.parse_args()
-    verbose: int = args.verbose
-    channels: list[Channel] = args.channels or get_default_channels()
-    host: str | None = args.host
-    port: int = args.port
-    ssl_context: ssl.SSLContext | None = args.cert
-
-    configure_logging("server", verbose)
-
-    state = ServerState()
-    for channel in channels:
-        state.add_channel(channel)
-
-    try:
-        asyncio.run(host_server(state, host, port, ssl=ssl_context))
-    except KeyboardInterrupt:
-        pass
-
-
-def parse_channel(s: str) -> Channel:
-    return Channel(name=s)
-
-
-def get_default_channels() -> list[Channel]:
-    return [Channel("general")]
-
-
-def parse_cert(s: str) -> ssl.SSLContext | None:
-    if s == "":
-        return
-
-    cafile, _, keyfile = s.partition(":")
-    keyfile = keyfile or None
-
-    context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
-    context.load_cert_chain(cafile, keyfile)
-    return context
-
-
-if __name__ == "__main__":
-    main()
+"""Host a dumdum server.
+
+To use TLS encryption, you must provide a certificate and private key.
+This can be specified as either:
+1. A single file containing both the private key and certificate:
+     --cert hello.pem
+2. A pair of certificate and private key files, separated with a colon:
+     --cert hello.crt:hello.key
+
+"""
+
+import argparse
+import asyncio
+import ssl
+
+from dumdum.protocol import Channel
+from dumdum.logging import configure_logging
+
+from .manager import host_server
+from .state import ServerState
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description=__doc__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="count",
+        default=0,
+        help="Increase logging verbosity",
+    )
+    parser.add_argument(
+        "-c",
+        "--channels",
+        action="extend",
+        nargs="+",
+        help="A list of channels",
+        type=parse_channel,
+    )
+    parser.add_argument(
+        "--host",
+        default=None,
+        help="The address to host on",
+    )
+    parser.add_argument(
+        "--port",
+        default=6667,
+        help="The port number to host on",
+    )
+    parser.add_argument(
+        "--cert",
+        default="",
+        help="The SSL certificate and private key to use",
+        type=parse_cert,
+    )
+
+    args = parser.parse_args()
+    verbose: int = args.verbose
+    channels: list[Channel] = args.channels or get_default_channels()
+    host: str | None = args.host
+    port: int = args.port
+    ssl_context: ssl.SSLContext | None = args.cert
+
+    configure_logging("server", verbose)
+
+    state = ServerState()
+    for channel in channels:
+        state.add_channel(channel)
+
+    try:
+        asyncio.run(host_server(state, host, port, ssl=ssl_context))
+    except KeyboardInterrupt:
+        pass
+
+
+def parse_channel(s: str) -> Channel:
+    return Channel(name=s)
+
+
+def get_default_channels() -> list[Channel]:
+    return [Channel("general")]
+
+
+def parse_cert(s: str) -> ssl.SSLContext | None:
+    if s == "":
+        return
+
+    cafile, _, keyfile = s.partition(":")
+    keyfile = keyfile or None
+
+    context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+    context.load_cert_chain(cafile, keyfile)
+    return context
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `dum-dum-irc-0.4.0.post1/tests/test_protocol.py` & `dum-dum-irc-0.4.1/tests/test_protocol.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,258 +1,273 @@
-from typing import Sequence, Type, TypeVar
-
-import pytest
-
-from dumdum.protocol import (
-    Channel,
-    Client,
-    ClientEventAuthentication,
-    ClientEventChannelsListed,
-    ClientEventHello,
-    ClientEventIncompatibleVersion,
-    ClientEventMessagesListed,
-    ClientState,
-    InvalidStateError,
-    MalformedDataError,
-    Message,
-    Protocol,
-    Server,
-    ServerEventAuthentication,
-    ServerEventHello,
-    ServerEventIncompatibleVersion,
-    ServerEventListChannels,
-    ServerEventListMessages,
-    ServerEventMessageReceived,
-    ServerState,
-)
-
-T = TypeVar("T")
-
-
-def communicate(
-    sender: Protocol,
-    data: bytes,
-    receiver: Protocol,
-) -> tuple[list[object], list[object]]:
-    def send_loop():
-        i, outgoing = 0, data
-        while len(outgoing) > 0:
-            receiver, receiver_events = order[i % len(order)]
-            print(f"{type(receiver).__name__} << {outgoing}")
-            events, outgoing = receiver.receive_bytes(outgoing)
-            receiver_events.extend(events)
-            i += 1
-
-    sender_events: list[object] = []
-    receiver_events: list[object] = []
-    order = [(receiver, receiver_events), (sender, sender_events)]
-    send_loop()
-    return sender_events, receiver_events
-
-
-def assert_event_order(events: Sequence[object], *expected_events: Type[object]):
-    # fmt: off
-    assert len(events) == len(expected_events), \
-        "Expected exactly {} event(s), got {} instead".format(
-        len(expected_events),
-        len(events),
-    )
-
-    for i, (event, type_) in enumerate(zip(events, expected_events)):
-        assert isinstance(event, type_), \
-            "Expected {} at index {}, got {} instead".format(
-            type_.__name__,
-            i,
-            type(event).__name__,
-        )
-    # fmt: on
-
-
-def test_authenticate():
-    nick = "thegamecracks"
-    client = Client(nick=nick)
-    server = Server()
-
-    client_events, server_events = communicate(client, client.hello(), server)
-    assert client_events == []
-    assert server_events == [ServerEventHello()]
-
-    data = server.hello(using_ssl=False)
-    server_events, client_events = communicate(server, data, client)
-    assert client_events == [ClientEventHello(using_ssl=False)]
-    assert server_events == []
-
-    client_events, server_events = communicate(client, client.authenticate(), server)
-    assert client_events == []
-    assert server_events == [ServerEventAuthentication(nick=nick)]
-
-    data = server.authenticate(success=True)
-    server_events, client_events = communicate(server, data, client)
-    assert client_events == [ClientEventAuthentication(success=True)]
-    assert server_events == []
-
-
-def test_authenticate_incompatible_version():
-    nick = "thegamecracks"
-    client = Client(nick=nick)
-    server = Server()
-
-    client.PROTOCOL_VERSION = server.PROTOCOL_VERSION + 1  # type: ignore
-    if client.PROTOCOL_VERSION > 255:
-        client.PROTOCOL_VERSION = server.PROTOCOL_VERSION - 1  # type: ignore
-
-    assert client.PROTOCOL_VERSION != server.PROTOCOL_VERSION
-
-    client_events, server_events = communicate(client, client.hello(), server)
-    assert client_events == [
-        ClientEventIncompatibleVersion(
-            client_version=client.PROTOCOL_VERSION,
-            server_version=server.PROTOCOL_VERSION,
-        )
-    ]
-    assert server_events == [
-        ServerEventIncompatibleVersion(
-            version=client.PROTOCOL_VERSION,
-        )
-    ]
-
-
-def test_send_message():
-    nick = "thegamecracks"
-    content = "Hello world!"
-    channel_name = "general"
-
-    client = Client(nick=nick)
-    server = Server()
-
-    communicate(client, client.hello(), server)
-    communicate(server, server.hello(using_ssl=False), client)
-    communicate(client, client.authenticate(), server)
-    communicate(server, server.authenticate(success=True), client)
-
-    client_events, server_events = communicate(
-        client,
-        client.send_message(channel_name, content),
-        server,
-    )
-    assert client_events == []
-    assert server_events == [ServerEventMessageReceived(channel_name, content)]
-
-
-def test_list_channels():
-    channels = [
-        Channel("announcements"),
-        Channel("general"),
-        Channel("memes"),
-        Channel("coding-lounge"),
-        Channel("fishing-trips"),
-    ]
-
-    client = Client(nick="thegamecracks")
-    server = Server()
-
-    communicate(client, client.hello(), server)
-    communicate(server, server.hello(using_ssl=False), client)
-    communicate(client, client.authenticate(), server)
-    communicate(server, server.authenticate(success=True), client)
-
-    client_events, server_events = communicate(client, client.list_channels(), server)
-    assert client_events == []
-    assert server_events == [ServerEventListChannels()]
-
-    data = server.list_channels(channels)
-    server_events, client_events = communicate(server, data, client)
-    assert client_events == [ClientEventChannelsListed(channels)]
-    assert server_events == []
-
-
-def test_unauthenticated_send_message():
-    nick = "thegamecracks"
-    content = "Hello world!"
-    channel = Channel("general")
-
-    client = Client(nick=nick)
-    server = Server()
-
-    with pytest.raises(InvalidStateError):
-        client.send_message(channel.name, content)
-
-    client._state = ClientState.READY
-    data = client.send_message(channel.name, content)
-
-    with pytest.raises(InvalidStateError):
-        communicate(client, data, server)
-
-
-def test_unauthenticated_server_send_message():
-    nick = "thegamecracks"
-    content = "Hello world!"
-    message = Message(0, "general", nick, content)
-
-    client = Client(nick=nick)
-    server = Server()
-
-    with pytest.raises(InvalidStateError):
-        server.send_message(message)
-
-    server._state = ServerState.READY
-    data = server.send_message(message)
-
-    with pytest.raises(InvalidStateError):
-        communicate(server, data, client)
-
-
-def test_list_messages():
-    nick = "thegamecracks"
-    channel = Channel("general")
-
-    client = Client(nick=nick)
-    server = Server()
-
-    communicate(client, client.hello(), server)
-    communicate(server, server.hello(using_ssl=False), client)
-    communicate(client, client.authenticate(), server)
-    communicate(server, server.authenticate(success=True), client)
-
-    before = 1
-    after = 2
-    data = client.list_messages(channel.name, before=before, after=after)
-    client_events, server_events = communicate(client, data, server)
-    assert client_events == []
-    assert server_events == [ServerEventListMessages(channel.name, before, after)]
-
-    messages = [Message(i, channel.name, nick, "Hello world!") for i in range(100)]
-    data = server.list_messages(messages)
-    server_events, client_events = communicate(server, data, client)
-    assert server_events == []
-    assert client_events == [ClientEventMessagesListed(messages)]
-
-
-def test_invalid_message_type():
-    client = Client("thegamecracks")
-    server = Server()
-
-    with pytest.raises(MalformedDataError):
-        client.receive_bytes(b"\xff")
-
-    with pytest.raises(MalformedDataError):
-        server.receive_bytes(b"\xff")
-
-
-def test_unicode_decode_error():
-    client = Client("thegamecracks")
-    server = Server()
-
-    communicate(client, client.hello(), server)
-    communicate(server, server.hello(using_ssl=False), client)
-    communicate(client, client.authenticate(), server)
-    communicate(server, server.authenticate(success=True), client)
-
-    with pytest.raises(MalformedDataError):
-        # LIST_CHANNELS, Channel name \N{EYES} but missing last 3 bytes
-        data = b"\x04\x00\x02\x01\xf0"
-        client.receive_bytes(data)
-
-    with pytest.raises(MalformedDataError):
-        # SEND_MESSAGE, Channel name \N{EYES} but missing last 3 bytes
-        data = b"\x03\x01\xf0"
-        server.receive_bytes(data)
+from typing import Sequence, Type, TypeVar
+
+import pytest
+
+from dumdum.protocol import (
+    BufferOverflowError,
+    Channel,
+    Client,
+    ClientEventAuthentication,
+    ClientEventChannelsListed,
+    ClientEventHello,
+    ClientEventIncompatibleVersion,
+    ClientEventMessagesListed,
+    ClientState,
+    InvalidStateError,
+    MalformedDataError,
+    Message,
+    Protocol,
+    Server,
+    ServerEventAuthentication,
+    ServerEventHello,
+    ServerEventIncompatibleVersion,
+    ServerEventListChannels,
+    ServerEventListMessages,
+    ServerEventMessageReceived,
+    ServerState,
+)
+
+T = TypeVar("T")
+
+
+def communicate(
+    sender: Protocol,
+    data: bytes,
+    receiver: Protocol,
+) -> tuple[list[object], list[object]]:
+    def send_loop():
+        i, outgoing = 0, data
+        while len(outgoing) > 0:
+            receiver, receiver_events = order[i % len(order)]
+            print(f"{type(receiver).__name__} << {outgoing}")
+            events, outgoing = receiver.receive_bytes(outgoing)
+            receiver_events.extend(events)
+            i += 1
+
+    sender_events: list[object] = []
+    receiver_events: list[object] = []
+    order = [(receiver, receiver_events), (sender, sender_events)]
+    send_loop()
+    return sender_events, receiver_events
+
+
+def assert_event_order(events: Sequence[object], *expected_events: Type[object]):
+    # fmt: off
+    assert len(events) == len(expected_events), \
+        "Expected exactly {} event(s), got {} instead".format(
+        len(expected_events),
+        len(events),
+    )
+
+    for i, (event, type_) in enumerate(zip(events, expected_events)):
+        assert isinstance(event, type_), \
+            "Expected {} at index {}, got {} instead".format(
+            type_.__name__,
+            i,
+            type(event).__name__,
+        )
+    # fmt: on
+
+
+def test_authenticate():
+    nick = "thegamecracks"
+    client = Client(nick=nick)
+    server = Server()
+
+    client_events, server_events = communicate(client, client.hello(), server)
+    assert client_events == []
+    assert server_events == [ServerEventHello()]
+
+    data = server.hello(using_ssl=False)
+    server_events, client_events = communicate(server, data, client)
+    assert client_events == [ClientEventHello(using_ssl=False)]
+    assert server_events == []
+
+    client_events, server_events = communicate(client, client.authenticate(), server)
+    assert client_events == []
+    assert server_events == [ServerEventAuthentication(nick=nick)]
+
+    data = server.authenticate(success=True)
+    server_events, client_events = communicate(server, data, client)
+    assert client_events == [ClientEventAuthentication(success=True)]
+    assert server_events == []
+
+
+def test_authenticate_incompatible_version():
+    nick = "thegamecracks"
+    client = Client(nick=nick)
+    server = Server()
+
+    client.PROTOCOL_VERSION = server.PROTOCOL_VERSION + 1  # type: ignore
+    if client.PROTOCOL_VERSION > 255:
+        client.PROTOCOL_VERSION = server.PROTOCOL_VERSION - 1  # type: ignore
+
+    assert client.PROTOCOL_VERSION != server.PROTOCOL_VERSION
+
+    client_events, server_events = communicate(client, client.hello(), server)
+    assert client_events == [
+        ClientEventIncompatibleVersion(
+            client_version=client.PROTOCOL_VERSION,
+            server_version=server.PROTOCOL_VERSION,
+        )
+    ]
+    assert server_events == [
+        ServerEventIncompatibleVersion(
+            version=client.PROTOCOL_VERSION,
+        )
+    ]
+
+
+def test_send_message():
+    nick = "thegamecracks"
+    content = "Hello world!"
+    channel_name = "general"
+
+    client = Client(nick=nick)
+    server = Server()
+
+    communicate(client, client.hello(), server)
+    communicate(server, server.hello(using_ssl=False), client)
+    communicate(client, client.authenticate(), server)
+    communicate(server, server.authenticate(success=True), client)
+
+    client_events, server_events = communicate(
+        client,
+        client.send_message(channel_name, content),
+        server,
+    )
+    assert client_events == []
+    assert server_events == [ServerEventMessageReceived(channel_name, content)]
+
+
+def test_list_channels():
+    channels = [
+        Channel("announcements"),
+        Channel("general"),
+        Channel("memes"),
+        Channel("coding-lounge"),
+        Channel("fishing-trips"),
+    ]
+
+    client = Client(nick="thegamecracks")
+    server = Server()
+
+    communicate(client, client.hello(), server)
+    communicate(server, server.hello(using_ssl=False), client)
+    communicate(client, client.authenticate(), server)
+    communicate(server, server.authenticate(success=True), client)
+
+    client_events, server_events = communicate(client, client.list_channels(), server)
+    assert client_events == []
+    assert server_events == [ServerEventListChannels()]
+
+    data = server.list_channels(channels)
+    server_events, client_events = communicate(server, data, client)
+    assert client_events == [ClientEventChannelsListed(channels)]
+    assert server_events == []
+
+
+def test_unauthenticated_send_message():
+    nick = "thegamecracks"
+    content = "Hello world!"
+    channel = Channel("general")
+
+    client = Client(nick=nick)
+    server = Server()
+
+    with pytest.raises(InvalidStateError):
+        client.send_message(channel.name, content)
+
+    client._state = ClientState.READY
+    data = client.send_message(channel.name, content)
+
+    with pytest.raises(InvalidStateError):
+        communicate(client, data, server)
+
+
+def test_unauthenticated_server_send_message():
+    nick = "thegamecracks"
+    content = "Hello world!"
+    message = Message(0, "general", nick, content)
+
+    client = Client(nick=nick)
+    server = Server()
+
+    with pytest.raises(InvalidStateError):
+        server.send_message(message)
+
+    server._state = ServerState.READY
+    data = server.send_message(message)
+
+    with pytest.raises(InvalidStateError):
+        communicate(server, data, client)
+
+
+def test_list_messages():
+    nick = "thegamecracks"
+    channel = Channel("general")
+
+    client = Client(nick=nick)
+    server = Server()
+
+    communicate(client, client.hello(), server)
+    communicate(server, server.hello(using_ssl=False), client)
+    communicate(client, client.authenticate(), server)
+    communicate(server, server.authenticate(success=True), client)
+
+    before = 1
+    after = 2
+    data = client.list_messages(channel.name, before=before, after=after)
+    client_events, server_events = communicate(client, data, server)
+    assert client_events == []
+    assert server_events == [ServerEventListMessages(channel.name, before, after)]
+
+    messages = [Message(i, channel.name, nick, "Hello world!") for i in range(100)]
+    data = server.list_messages(messages)
+    server_events, client_events = communicate(server, data, client)
+    assert server_events == []
+    assert client_events == [ClientEventMessagesListed(messages)]
+
+
+def test_invalid_message_type():
+    client = Client("thegamecracks")
+    server = Server()
+
+    with pytest.raises(MalformedDataError):
+        client.receive_bytes(b"\xff")
+
+    with pytest.raises(MalformedDataError):
+        server.receive_bytes(b"\xff")
+
+
+def test_unicode_decode_error():
+    client = Client("thegamecracks")
+    server = Server()
+
+    communicate(client, client.hello(), server)
+    communicate(server, server.hello(using_ssl=False), client)
+    communicate(client, client.authenticate(), server)
+    communicate(server, server.authenticate(success=True), client)
+
+    with pytest.raises(MalformedDataError):
+        # LIST_CHANNELS, Channel name \N{EYES} but missing last 3 bytes
+        data = b"\x04\x00\x02\x01\xf0"
+        client.receive_bytes(data)
+
+    with pytest.raises(MalformedDataError):
+        # SEND_MESSAGE, Channel name \N{EYES} but missing last 3 bytes
+        data = b"\x03\x01\xf0"
+        server.receive_bytes(data)
+
+
+def test_buffer_overflow_prevention():
+    data = b"Hello world!\n"
+    size = len(data) - 1
+
+    client = Client("thegamecracks", buffer_size=size)
+    server = Server(buffer_size=size)
+
+    with pytest.raises(BufferOverflowError):
+        client.receive_bytes(data)
+
+    with pytest.raises(BufferOverflowError):
+        server.receive_bytes(data)
```

### Comparing `dum-dum-irc-0.4.0.post1/tests/test_reader.py` & `dum-dum-irc-0.4.1/tests/test_reader.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import pytest
-
-from dumdum.protocol import bytearray_reader, byte_reader
-
-
-def test_bytearray_reader_commit_and_rollback():
-    data = bytearray(b"Hello world!\n")
-
-    with bytearray_reader(data) as reader:
-        assert reader.read(5) == b"Hello"
-
-    assert data == b" world!\n"
-
-    with pytest.raises(RuntimeError), bytearray_reader(data) as reader:
-        assert reader.read() == b" world!\n"
-        raise RuntimeError
-
-    assert data == b" world!\n"
-
-
-def test_reader_out_of_bounds():
-    with byte_reader(b"Hello world!\n") as reader:
-        with pytest.raises(ValueError):
-            reader.readexactly(-1)
-
-        assert reader.read(1000) == b"Hello world!\n"
-
-        reader.readexactly(0)
-
-        with pytest.raises(IndexError):
-            reader.readexactly(1)
-
-
-def test_reader_varchar():
-    with byte_reader(b"\x05Hello\x08 world!\n") as reader:
-        assert reader.read_varchar(max_length=5) == "Hello"
-        assert reader.read_varchar(max_length=8) == " world!\n"
-
-
-def test_reader_closed():
-    with byte_reader(b"Hello world!\n") as reader:
-        pass
-
-    with pytest.raises(RuntimeError):
-        reader.read()
-
-    with pytest.raises(RuntimeError):
-        reader.readexactly(1)
+import pytest
+
+from dumdum.protocol import bytearray_reader, byte_reader
+
+
+def test_bytearray_reader_commit_and_rollback():
+    data = bytearray(b"Hello world!\n")
+
+    with bytearray_reader(data) as reader:
+        assert reader.read(5) == b"Hello"
+
+    assert data == b" world!\n"
+
+    with pytest.raises(RuntimeError), bytearray_reader(data) as reader:
+        assert reader.read() == b" world!\n"
+        raise RuntimeError
+
+    assert data == b" world!\n"
+
+
+def test_reader_out_of_bounds():
+    with byte_reader(b"Hello world!\n") as reader:
+        with pytest.raises(ValueError):
+            reader.readexactly(-1)
+
+        assert reader.read(1000) == b"Hello world!\n"
+
+        reader.readexactly(0)
+
+        with pytest.raises(IndexError):
+            reader.readexactly(1)
+
+
+def test_reader_varchar():
+    with byte_reader(b"\x05Hello\x08 world!\n") as reader:
+        assert reader.read_varchar(max_length=5) == "Hello"
+        assert reader.read_varchar(max_length=8) == " world!\n"
+
+
+def test_reader_closed():
+    with byte_reader(b"Hello world!\n") as reader:
+        pass
+
+    with pytest.raises(RuntimeError):
+        reader.read()
+
+    with pytest.raises(RuntimeError):
+        reader.readexactly(1)
```

