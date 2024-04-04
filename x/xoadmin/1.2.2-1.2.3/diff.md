# Comparing `tmp/xoadmin-1.2.2.tar.gz` & `tmp/xoadmin-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoadmin-1.2.2.tar", max compression
+gzip compressed data, was "xoadmin-1.2.3.tar", max compression
```

## Comparing `xoadmin-1.2.2.tar` & `xoadmin-1.2.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    11336 2024-04-04 20:56:51.381844 xoadmin-1.2.2/LICENSE
--rw-r--r--   0        0        0     5725 2024-04-04 20:56:51.381844 xoadmin-1.2.2/README.md
--rw-r--r--   0        0        0      787 2024-04-04 20:56:51.381844 xoadmin-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/__init__.py
--rw-r--r--   0        0        0     4643 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/api.py
--rw-r--r--   0        0        0      389 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/error.py
--rw-r--r--   0        0        0     2192 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/host.py
--rw-r--r--   0        0        0     6696 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/manager.py
--rw-r--r--   0        0        0     1418 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/storage.py
--rw-r--r--   0        0        0     3824 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/user.py
--rw-r--r--   0        0        0     1586 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/vm.py
--rw-r--r--   0        0        0     5724 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/websocket.py
--rw-r--r--   0        0        0        0 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/__init__.py
--rw-r--r--   0        0        0      750 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/apply.py
--rw-r--r--   0        0        0     2199 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/auth.py
--rw-r--r--   0        0        0     1433 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/cli.py
--rw-r--r--   0        0        0     4542 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/config.py
--rw-r--r--   0        0        0     2002 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/hosts.py
--rw-r--r--   0        0        0     1736 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/model.py
--rw-r--r--   0        0        0      784 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/options.py
--rw-r--r--   0        0        0     1937 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/storage.py
--rw-r--r--   0        0        0     2046 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/users.py
--rw-r--r--   0        0        0     6103 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/utils.py
--rw-r--r--   0        0        0     1940 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/vms.py
--rw-r--r--   0        0        0        0 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/configurator/__init__.py
--rw-r--r--   0        0        0      708 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/configurator/config.py
--rw-r--r--   0        0        0     1571 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/configurator/configurator.py
--rw-r--r--   0        0        0      283 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/configurator/loader.py
--rw-r--r--   0        0        0     1822 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/utils.py
--rw-r--r--   0        0        0     6589 1970-01-01 00:00:00.000000 xoadmin-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-04 21:20:56.820974 xoadmin-1.2.3/LICENSE
+-rw-r--r--   0        0        0     5725 2024-04-04 21:20:56.820974 xoadmin-1.2.3/README.md
+-rw-r--r--   0        0        0      787 2024-04-04 21:20:56.824974 xoadmin-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/__main__.py
+-rw-r--r--   0        0        0     4643 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/api/api.py
+-rw-r--r--   0        0        0      389 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/api/error.py
+-rw-r--r--   0        0        0     2192 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/api/host.py
+-rw-r--r--   0        0        0     6696 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/api/manager.py
+-rw-r--r--   0        0        0     1418 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/api/storage.py
+-rw-r--r--   0        0        0     3824 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/api/user.py
+-rw-r--r--   0        0        0     1586 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/api/vm.py
+-rw-r--r--   0        0        0     5724 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/api/websocket.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/apply.py
+-rw-r--r--   0        0        0     2199 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/auth.py
+-rw-r--r--   0        0        0     1433 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/cli.py
+-rw-r--r--   0        0        0     4542 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/config.py
+-rw-r--r--   0        0        0     2002 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/hosts.py
+-rw-r--r--   0        0        0     1736 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/model.py
+-rw-r--r--   0        0        0      784 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/options.py
+-rw-r--r--   0        0        0     1937 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/storage.py
+-rw-r--r--   0        0        0     2046 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/users.py
+-rw-r--r--   0        0        0     6103 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/utils.py
+-rw-r--r--   0        0        0     1940 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/cli/vms.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/configurator/__init__.py
+-rw-r--r--   0        0        0      708 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/configurator/config.py
+-rw-r--r--   0        0        0     1571 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/configurator/configurator.py
+-rw-r--r--   0        0        0      283 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/configurator/loader.py
+-rw-r--r--   0        0        0     1822 2024-04-04 21:20:56.824974 xoadmin-1.2.3/src/xoadmin/utils.py
+-rw-r--r--   0        0        0     6589 1970-01-01 00:00:00.000000 xoadmin-1.2.3/PKG-INFO
```

### Comparing `xoadmin-1.2.2/LICENSE` & `xoadmin-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/README.md` & `xoadmin-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/pyproject.toml` & `xoadmin-1.2.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xoadmin"
-version = "1.2.2"
+version = "1.2.3"
 description = "bindings and wrappers to manage an XOA instance"
 authors = ["dennis <it.admin@elnissi.co.id>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "xoadmin", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `xoadmin-1.2.2/src/xoadmin/api/api.py` & `xoadmin-1.2.3/src/xoadmin/api/api.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/api/host.py` & `xoadmin-1.2.3/src/xoadmin/api/host.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/api/manager.py` & `xoadmin-1.2.3/src/xoadmin/api/manager.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/api/storage.py` & `xoadmin-1.2.3/src/xoadmin/api/storage.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/api/user.py` & `xoadmin-1.2.3/src/xoadmin/api/user.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/api/vm.py` & `xoadmin-1.2.3/src/xoadmin/api/vm.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/api/websocket.py` & `xoadmin-1.2.3/src/xoadmin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/apply.py` & `xoadmin-1.2.3/src/xoadmin/cli/apply.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/auth.py` & `xoadmin-1.2.3/src/xoadmin/cli/auth.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/cli.py` & `xoadmin-1.2.3/src/xoadmin/cli/cli.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/config.py` & `xoadmin-1.2.3/src/xoadmin/cli/config.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/hosts.py` & `xoadmin-1.2.3/src/xoadmin/cli/hosts.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/model.py` & `xoadmin-1.2.3/src/xoadmin/cli/model.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/options.py` & `xoadmin-1.2.3/src/xoadmin/cli/options.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/storage.py` & `xoadmin-1.2.3/src/xoadmin/cli/storage.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/users.py` & `xoadmin-1.2.3/src/xoadmin/cli/users.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/utils.py` & `xoadmin-1.2.3/src/xoadmin/cli/utils.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/cli/vms.py` & `xoadmin-1.2.3/src/xoadmin/cli/vms.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/configurator/config.py` & `xoadmin-1.2.3/src/xoadmin/configurator/config.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/configurator/configurator.py` & `xoadmin-1.2.3/src/xoadmin/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/src/xoadmin/utils.py` & `xoadmin-1.2.3/src/xoadmin/utils.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.2/PKG-INFO` & `xoadmin-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoadmin
-Version: 1.2.2
+Version: 1.2.3
 Summary: bindings and wrappers to manage an XOA instance
 License: Apache 2.0
 Author: dennis
 Author-email: it.admin@elnissi.co.id
 Requires-Python: >=3.9.2
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

