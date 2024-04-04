# Comparing `tmp/omuplugin_emoji-0.2.1.tar.gz` & `tmp/omuplugin_emoji-0.2.2.tar.gz`

## Comparing `omuplugin_emoji-0.2.1.tar` & `omuplugin_emoji-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.1/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.1/src/omuplugin_emoji/__init__.py
--rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.1/src/omuplugin_emoji/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.1/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.1/README.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.2/.python-version
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.2/src/omuplugin_emoji/__init__.py
+-rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.2/src/omuplugin_emoji/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.2/README.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.2/PKG-INFO
```

### Comparing `omuplugin_emoji-0.2.1/src/omuplugin_emoji/plugin.py` & `omuplugin_emoji-0.2.2/src/omuplugin_emoji/plugin.py`

 * *Files identical despite different names*

### Comparing `omuplugin_emoji-0.2.1/pyproject.toml` & `omuplugin_emoji-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_emoji"
-version = "0.2.1"
+version = "0.2.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

