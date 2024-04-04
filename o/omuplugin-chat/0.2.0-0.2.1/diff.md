# Comparing `tmp/omuplugin_chat-0.2.0.tar.gz` & `tmp/omuplugin_chat-0.2.1.tar.gz`

## Comparing `omuplugin_chat-0.2.0.tar` & `omuplugin_chat-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.0/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.0/src/omuplugin_chat/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.0/src/omuplugin_chat/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.0/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.0/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/.python-version
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/src/omuplugin_chat/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/src/omuplugin_chat/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.1/PKG-INFO
```

### Comparing `omuplugin_chat-0.2.0/src/omuplugin_chat/plugin.py` & `omuplugin_chat-0.2.1/src/omuplugin_chat/plugin.py`

 * *Files identical despite different names*

### Comparing `omuplugin_chat-0.2.0/pyproject.toml` & `omuplugin_chat-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_chat"
-version = "0.2.0"
+version = "0.2.1"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

