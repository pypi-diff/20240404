# Comparing `tmp/antibot-2.1.5.tar.gz` & `tmp/antibot-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antibot-2.1.5.tar", last modified: Tue Nov 30 15:57:44 2021, max compression
+gzip compressed data, was "antibot-2.1.6.tar", last modified: Thu Apr  4 14:57:15 2024, max compression
```

## Comparing `antibot-2.1.5.tar` & `antibot-2.1.6.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)    26461 2021-11-30 15:57:35.000000 antibot-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-11-30 15:57:44.539794 antibot-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2021-11-30 15:57:35.000000 antibot-2.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-30 15:57:44.543794 antibot-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      989 2021-11-30 15:57:35.000000 antibot-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.535794 antibot-2.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/src/antibot/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/src/antibot/internal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/src/antibot/internal/backend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/src/antibot/internal/backend/actions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/actions/action_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3722 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/actions/block_action_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/actions/view_closed_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/actions/view_submit_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/debugger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/endpoint_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/installer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/request_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/backend/ws_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/module.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/src/antibot/internal/slack/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/slack/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/slack/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/internal/slack/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/main.py
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/provided.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/src/antibot/repository/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/repository/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/repository/users.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/src/antibot/slack/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5296 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/slack/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/slack/callback.py
--rw-r--r--   0 runner    (1001) docker     (121)     7174 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/slack/message.py
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-11-30 15:57:35.000000 antibot-2.1.5/src/antibot/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 15:57:44.539794 antibot-2.1.5/src/antibot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-11-30 15:57:44.000000 antibot-2.1.5/src/antibot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2021-11-30 15:57:44.000000 antibot-2.1.5/src/antibot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-30 15:57:44.000000 antibot-2.1.5/src/antibot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-11-30 15:57:44.000000 antibot-2.1.5/src/antibot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-11-30 15:57:44.000000 antibot-2.1.5/src/antibot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-11-30 15:57:44.000000 antibot-2.1.5/src/antibot.egg-info/top_level.txt
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.518943 antibot-2.1.6/
+-rw-r--r--   0 jean       (501) staff       (20)    26461 2020-09-11 12:25:00.000000 antibot-2.1.6/LICENSE
+-rw-r--r--   0 jean       (501) staff       (20)      314 2024-04-04 14:57:15.518414 antibot-2.1.6/PKG-INFO
+-rw-r--r--   0 jean       (501) staff       (20)     1712 2020-09-11 12:24:58.000000 antibot-2.1.6/README.md
+-rw-r--r--   0 jean       (501) staff       (20)       38 2024-04-04 14:57:15.519055 antibot-2.1.6/setup.cfg
+-rw-r--r--   0 jean       (501) staff       (20)     1007 2024-04-04 14:42:45.000000 antibot-2.1.6/setup.py
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.468275 antibot-2.1.6/src/
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.477131 antibot-2.1.6/src/antibot/
+-rw-r--r--   0 jean       (501) staff       (20)       22 2024-04-04 14:43:20.000000 antibot-2.1.6/src/antibot/__init__.py
+-rw-r--r--   0 jean       (501) staff       (20)     1502 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/decorators.py
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.483663 antibot-2.1.6/src/antibot/internal/
+-rw-r--r--   0 jean       (501) staff       (20)        0 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/__init__.py
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.489515 antibot-2.1.6/src/antibot/internal/backend/
+-rw-r--r--   0 jean       (501) staff       (20)        0 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/__init__.py
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.493089 antibot-2.1.6/src/antibot/internal/backend/actions/
+-rw-r--r--   0 jean       (501) staff       (20)        0 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/actions/__init__.py
+-rw-r--r--   0 jean       (501) staff       (20)     1470 2021-07-06 13:29:03.000000 antibot-2.1.6/src/antibot/internal/backend/actions/action_runner.py
+-rw-r--r--   0 jean       (501) staff       (20)     3722 2021-07-06 14:13:35.000000 antibot-2.1.6/src/antibot/internal/backend/actions/block_action_runner.py
+-rw-r--r--   0 jean       (501) staff       (20)     1786 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/actions/view_closed_runner.py
+-rw-r--r--   0 jean       (501) staff       (20)     2331 2021-01-06 14:28:30.000000 antibot-2.1.6/src/antibot/internal/backend/actions/view_submit_runner.py
+-rw-r--r--   0 jean       (501) staff       (20)     1562 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/command_runner.py
+-rw-r--r--   0 jean       (501) staff       (20)      361 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/constants.py
+-rw-r--r--   0 jean       (501) staff       (20)     2107 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/debugger.py
+-rw-r--r--   0 jean       (501) staff       (20)     1010 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/descriptor.py
+-rw-r--r--   0 jean       (501) staff       (20)     1237 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/internal/backend/endpoint_runner.py
+-rw-r--r--   0 jean       (501) staff       (20)     2130 2021-07-06 13:28:26.000000 antibot-2.1.6/src/antibot/internal/backend/installer.py
+-rw-r--r--   0 jean       (501) staff       (20)     1269 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/request_checker.py
+-rw-r--r--   0 jean       (501) staff       (20)     1288 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/backend/ws_runner.py
+-rw-r--r--   0 jean       (501) staff       (20)      172 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/configuration.py
+-rw-r--r--   0 jean       (501) staff       (20)     1603 2021-11-30 14:01:29.000000 antibot-2.1.6/src/antibot/internal/module.py
+-rw-r--r--   0 jean       (501) staff       (20)      720 2020-09-11 12:25:00.000000 antibot-2.1.6/src/antibot/internal/plugins.py
+-rw-r--r--   0 jean       (501) staff       (20)     1549 2024-04-04 14:42:45.000000 antibot-2.1.6/src/antibot/internal/scheduler.py
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.495697 antibot-2.1.6/src/antibot/internal/slack/
+-rw-r--r--   0 jean       (501) staff       (20)        0 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/internal/slack/__init__.py
+-rw-r--r--   0 jean       (501) staff       (20)       88 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/internal/slack/channel.py
+-rw-r--r--   0 jean       (501) staff       (20)      702 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/internal/slack/upload.py
+-rw-r--r--   0 jean       (501) staff       (20)      358 2020-12-07 10:25:31.000000 antibot-2.1.6/src/antibot/internal/slack/user.py
+-rw-r--r--   0 jean       (501) staff       (20)     1258 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/main.py
+-rw-r--r--   0 jean       (501) staff       (20)       76 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/plugin.py
+-rw-r--r--   0 jean       (501) staff       (20)     1569 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/provided.py
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.497712 antibot-2.1.6/src/antibot/repository/
+-rw-r--r--   0 jean       (501) staff       (20)        0 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/repository/__init__.py
+-rw-r--r--   0 jean       (501) staff       (20)     1636 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/repository/messages.py
+-rw-r--r--   0 jean       (501) staff       (20)     1167 2021-10-12 12:53:33.000000 antibot-2.1.6/src/antibot/repository/users.py
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.516617 antibot-2.1.6/src/antibot/slack/
+-rw-r--r--   0 jean       (501) staff       (20)        0 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/slack/__init__.py
+-rw-r--r--   0 jean       (501) staff       (20)     5296 2021-10-19 09:53:58.000000 antibot-2.1.6/src/antibot/slack/api.py
+-rw-r--r--   0 jean       (501) staff       (20)     1622 2020-10-09 12:36:23.000000 antibot-2.1.6/src/antibot/slack/callback.py
+-rw-r--r--   0 jean       (501) staff       (20)     7174 2022-05-25 13:50:25.000000 antibot-2.1.6/src/antibot/slack/message.py
+-rw-r--r--   0 jean       (501) staff       (20)      402 2020-09-11 12:25:01.000000 antibot-2.1.6/src/antibot/tools.py
+-rw-r--r--   0 jean       (501) staff       (20)      214 2020-12-07 10:24:14.000000 antibot-2.1.6/src/antibot/user.py
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.480475 antibot-2.1.6/src/antibot.egg-info/
+-rw-r--r--   0 jean       (501) staff       (20)      314 2024-04-04 14:57:15.000000 antibot-2.1.6/src/antibot.egg-info/PKG-INFO
+-rw-r--r--   0 jean       (501) staff       (20)     1623 2024-04-04 14:57:15.000000 antibot-2.1.6/src/antibot.egg-info/SOURCES.txt
+-rw-r--r--   0 jean       (501) staff       (20)        1 2024-04-04 14:57:15.000000 antibot-2.1.6/src/antibot.egg-info/dependency_links.txt
+-rw-r--r--   0 jean       (501) staff       (20)      181 2024-04-04 14:57:15.000000 antibot-2.1.6/src/antibot.egg-info/entry_points.txt
+-rw-r--r--   0 jean       (501) staff       (20)       73 2024-04-04 14:57:15.000000 antibot-2.1.6/src/antibot.egg-info/requires.txt
+-rw-r--r--   0 jean       (501) staff       (20)        8 2024-04-04 14:57:15.000000 antibot-2.1.6/src/antibot.egg-info/top_level.txt
+drwxr-xr-x   0 jean       (501) staff       (20)        0 2024-04-04 14:57:15.517466 antibot-2.1.6/tests/
+-rw-r--r--   0 jean       (501) staff       (20)       67 2020-09-11 12:24:58.000000 antibot-2.1.6/tests/test_basic.py
```

### Comparing `antibot-2.1.5/LICENSE` & `antibot-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/README.md` & `antibot-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/setup.py` & `antibot-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,13 +24,14 @@
       packages=find_packages(where='src'),
       package_dir={'': 'src'},
       install_requires=[
           'pymongo',
           'requests',
           'injector',
           'pyckson',
+          'pytz',
           'schedule',
           'slackclient',
           'arrow',
           'bottle'
       ],
       )
```

### Comparing `antibot-2.1.5/src/antibot/decorators.py` & `antibot-2.1.6/src/antibot/decorators.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/actions/action_runner.py` & `antibot-2.1.6/src/antibot/internal/backend/actions/action_runner.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/actions/block_action_runner.py` & `antibot-2.1.6/src/antibot/internal/backend/actions/block_action_runner.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/actions/view_closed_runner.py` & `antibot-2.1.6/src/antibot/internal/backend/actions/view_closed_runner.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/actions/view_submit_runner.py` & `antibot-2.1.6/src/antibot/internal/backend/actions/view_submit_runner.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/command_runner.py` & `antibot-2.1.6/src/antibot/internal/backend/command_runner.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/debugger.py` & `antibot-2.1.6/src/antibot/internal/backend/debugger.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/descriptor.py` & `antibot-2.1.6/src/antibot/internal/backend/descriptor.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/endpoint_runner.py` & `antibot-2.1.6/src/antibot/internal/backend/endpoint_runner.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/installer.py` & `antibot-2.1.6/src/antibot/internal/backend/installer.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/request_checker.py` & `antibot-2.1.6/src/antibot/internal/backend/request_checker.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/backend/ws_runner.py` & `antibot-2.1.6/src/antibot/internal/backend/ws_runner.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/module.py` & `antibot-2.1.6/src/antibot/internal/module.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/plugins.py` & `antibot-2.1.6/src/antibot/internal/plugins.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/internal/scheduler.py` & `antibot-2.1.6/src/antibot/internal/scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import atexit
+import os
 import traceback
 from inspect import getmembers
 from threading import Thread
 from time import sleep
 
 import schedule
 from injector import inject, Injector
@@ -31,19 +32,20 @@
 class Scheduler:
     @inject
     def __init__(self, injector: Injector, plugins: PluginsCollection, watch: SchedulerWatch):
         self.plugins = plugins
         self.injector = injector
         self.watch = watch
         self.watch_thread = Thread(target=watch.run)
+        self.tz = os.getenv("SCHEDULER_TIMEZONE")
 
     def bootstrap(self):
         for plugin in self.plugins.plugins:
             for method, hour in find_daily_jobs(plugin):
-                schedule.every().day.at(hour).do(self.run, plugin, method)
+                schedule.every().day.at(hour, self.tz).do(self.run, plugin, method)
         self.watch_thread.start()
 
         def stop():
             self.watch.running = False
             self.watch_thread.join(1)
 
         atexit.register(lambda: stop())
```

### Comparing `antibot-2.1.5/src/antibot/internal/slack/upload.py` & `antibot-2.1.6/src/antibot/internal/slack/upload.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/main.py` & `antibot-2.1.6/src/antibot/main.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/provided.py` & `antibot-2.1.6/src/antibot/provided.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/repository/messages.py` & `antibot-2.1.6/src/antibot/repository/messages.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/repository/users.py` & `antibot-2.1.6/src/antibot/repository/users.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/slack/api.py` & `antibot-2.1.6/src/antibot/slack/api.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/slack/callback.py` & `antibot-2.1.6/src/antibot/slack/callback.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot/slack/message.py` & `antibot-2.1.6/src/antibot/slack/message.py`

 * *Files identical despite different names*

### Comparing `antibot-2.1.5/src/antibot.egg-info/SOURCES.txt` & `antibot-2.1.6/src/antibot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,9 @@
 src/antibot/internal/slack/user.py
 src/antibot/repository/__init__.py
 src/antibot/repository/messages.py
 src/antibot/repository/users.py
 src/antibot/slack/__init__.py
 src/antibot/slack/api.py
 src/antibot/slack/callback.py
-src/antibot/slack/message.py
+src/antibot/slack/message.py
+tests/test_basic.py
```

