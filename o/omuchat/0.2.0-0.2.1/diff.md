# Comparing `tmp/omuchat-0.2.0.tar.gz` & `tmp/omuchat-0.2.1.tar.gz`

## Comparing `omuchat-0.2.0.tar` & `omuchat-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchat-0.2.0/.python-version
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchat-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 omuchat-0.2.0/example/chatlogger.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/__init__.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/chat.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/client.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/event/__init__.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/event/event.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/event/event_types.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/__init__.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/author.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/channel.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/content.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/gift.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/message.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/paid.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/provider.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/role.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 omuchat-0.2.0/src/omuchat/model/room.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchat-0.2.0/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.2.0/README.md
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchat-0.2.1/.python-version
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchat-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 omuchat-0.2.1/example/chatlogger.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/__init__.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/chat.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/client.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/event/__init__.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/event/event.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/event/event_types.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/__init__.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/author.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/channel.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/content.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/gift.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/message.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/paid.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/provider.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/role.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 omuchat-0.2.1/src/omuchat/model/room.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchat-0.2.1/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.2.1/README.md
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.2.1/PKG-INFO
```

### Comparing `omuchat-0.2.0/src/omuchat/chat.py` & `omuchat-0.2.1/src/omuchat/chat.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/client.py` & `omuchat-0.2.1/src/omuchat/client.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/event/event.py` & `omuchat-0.2.1/src/omuchat/event/event.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/event/event_types.py` & `omuchat-0.2.1/src/omuchat/event/event_types.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/author.py` & `omuchat-0.2.1/src/omuchat/model/author.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/channel.py` & `omuchat-0.2.1/src/omuchat/model/channel.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/content.py` & `omuchat-0.2.1/src/omuchat/model/content.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/gift.py` & `omuchat-0.2.1/src/omuchat/model/gift.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/message.py` & `omuchat-0.2.1/src/omuchat/model/message.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/paid.py` & `omuchat-0.2.1/src/omuchat/model/paid.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/provider.py` & `omuchat-0.2.1/src/omuchat/model/provider.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/role.py` & `omuchat-0.2.1/src/omuchat/model/role.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.0/src/omuchat/model/room.py` & `omuchat-0.2.1/src/omuchat/model/room.py`

 * *Files identical despite different names*

