# Comparing `tmp/tfprovider-0.1.1.tar.gz` & `tmp/tfprovider-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfprovider-0.1.1.tar", max compression
+gzip compressed data, was "tfprovider-0.1.1.post1.tar", max compression
```

## Comparing `tfprovider-0.1.1.tar` & `tfprovider-0.1.1.post1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    16764 2023-12-27 02:31:40.231475 tfprovider-0.1.1/LICENSE
--rw-r--r--   0        0        0     1450 2023-12-24 00:39:41.255049 tfprovider-0.1.1/README.md
--rw-r--r--   0        0        0      986 2023-12-27 20:38:12.031468 tfprovider-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      458 2023-12-05 20:44:50.022576 tfprovider-0.1.1/tfprovider/__init__.py
--rw-r--r--   0        0        0      373 2023-12-19 00:04:06.101163 tfprovider-0.1.1/tfprovider/level1/__init__.py
--rw-r--r--   0        0        0        0 2023-12-19 00:07:52.583671 tfprovider-0.1.1/tfprovider/level1/_async/__init__.py
--rw-r--r--   0        0        0      246 2023-12-19 00:16:52.876331 tfprovider-0.1.1/tfprovider/level1/_async/rpc_plugin_server.py
--rw-r--r--   0        0        0        0 2023-12-19 00:08:23.424013 tfprovider-0.1.1/tfprovider/level1/_common/__init__.py
--rw-r--r--   0        0        0      510 2023-12-27 20:37:11.658648 tfprovider-0.1.1/tfprovider/level1/_common/rpc_plugin_server.py
--rw-r--r--   0        0        0        0 2023-12-24 00:26:28.675700 tfprovider-0.1.1/tfprovider/level1/_sync/__init__.py
--rw-r--r--   0        0        0      244 2023-12-24 00:26:28.675700 tfprovider-0.1.1/tfprovider/level1/_sync/rpc_plugin_server.py
--rw-r--r--   0        0        0      305 2023-11-05 00:40:05.943675 tfprovider-0.1.1/tfprovider/level1/proto/grpc_controller.proto
--rw-r--r--   0        0        0    14045 2023-10-22 16:13:49.250288 tfprovider-0.1.1/tfprovider/level1/proto/tfplugin64.proto
--rw-r--r--   0        0        0      245 2023-12-19 00:16:10.175668 tfprovider-0.1.1/tfprovider/level1/rpc_plugin.py
--rw-r--r--   0        0        0      372 2023-12-05 20:36:29.465044 tfprovider-0.1.1/tfprovider/level2/__init__.py
--rw-r--r--   0        0        0     1884 2023-12-17 00:18:55.229017 tfprovider-0.1.1/tfprovider/level2/attribute_path.py
--rw-r--r--   0        0        0     1845 2023-12-17 00:15:27.738079 tfprovider-0.1.1/tfprovider/level2/diagnostics.py
--rw-r--r--   0        0        0     2985 2023-12-20 01:30:37.689430 tfprovider-0.1.1/tfprovider/level2/dynamic_value.py
--rw-r--r--   0        0        0     3170 2023-12-17 15:42:46.152919 tfprovider-0.1.1/tfprovider/level2/usable_schema.py
--rw-r--r--   0        0        0     4098 2023-12-23 23:44:58.763979 tfprovider-0.1.1/tfprovider/level2/wire_format.py
--rw-r--r--   0        0        0    17151 2023-12-23 23:38:44.319275 tfprovider-0.1.1/tfprovider/level2/wire_marshaling.py
--rw-r--r--   0        0        0     5321 2023-12-23 14:02:13.408042 tfprovider-0.1.1/tfprovider/level2/wire_representation.py
--rw-r--r--   0        0        0      186 2023-12-10 14:46:35.908279 tfprovider-0.1.1/tfprovider/level3/__init__.py
--rw-r--r--   0        0        0    11181 2023-12-23 23:44:13.719416 tfprovider-0.1.1/tfprovider/level3/statically_typed_schema.py
--rw-r--r--   0        0        0      203 2023-12-15 00:18:21.473233 tfprovider-0.1.1/tfprovider/level4/__init__.py
--rw-r--r--   0        0        0        0 2023-12-13 01:01:19.378306 tfprovider-0.1.1/tfprovider/level4/_async/__init__.py
--rw-r--r--   0        0        0    15828 2023-12-23 17:20:24.769094 tfprovider-0.1.1/tfprovider/level4/_async/provider_servicer.py
--rw-r--r--   0        0        0        0 2023-12-24 00:26:28.691700 tfprovider-0.1.1/tfprovider/level4/_sync/__init__.py
--rw-r--r--   0        0        0    15646 2023-12-24 00:26:28.691700 tfprovider-0.1.1/tfprovider/level4/_sync/provider_servicer.py
--rw-r--r--   0        0        0      168 2023-12-15 00:18:59.657813 tfprovider-0.1.1/tfprovider/level4/async_provider_servicer.py
--rw-r--r--   0        0        0      167 2023-12-15 00:19:14.742041 tfprovider-0.1.1/tfprovider/level4/provider_servicer.py
--rw-r--r--   0        0        0      521 2023-12-23 17:18:39.407775 tfprovider-0.1.1/tfprovider/level4/utils.py
--rw-r--r--   0        0        0        0 2023-12-21 01:30:55.795144 tfprovider-0.1.1/tfprovider/py.typed
--rw-r--r--   0        0        0   323052 2023-12-04 23:52:47.317804 tfprovider-0.1.1/tfprovider/tfprovider.png
--rw-r--r--   0        0        0      114 2023-12-04 23:52:14.841393 tfprovider-0.1.1/tfprovider/tfprovider_level3.png
--rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 tfprovider-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    16764 2023-12-27 02:31:40.231475 tfprovider-0.1.1.post1/LICENSE
+-rw-r--r--   0        0        0     2042 2024-04-03 23:42:32.238842 tfprovider-0.1.1.post1/README.md
+-rw-r--r--   0        0        0      992 2024-04-03 23:43:47.947965 tfprovider-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0      458 2023-12-05 20:44:50.022576 tfprovider-0.1.1.post1/tfprovider/__init__.py
+-rw-r--r--   0        0        0      373 2023-12-19 00:04:06.101163 tfprovider-0.1.1.post1/tfprovider/level1/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:07:52.583671 tfprovider-0.1.1.post1/tfprovider/level1/_async/__init__.py
+-rw-r--r--   0        0        0      246 2023-12-19 00:16:52.876331 tfprovider-0.1.1.post1/tfprovider/level1/_async/rpc_plugin_server.py
+-rw-r--r--   0        0        0        0 2023-12-19 00:08:23.424013 tfprovider-0.1.1.post1/tfprovider/level1/_common/__init__.py
+-rw-r--r--   0        0        0      510 2023-12-27 20:37:11.658648 tfprovider-0.1.1.post1/tfprovider/level1/_common/rpc_plugin_server.py
+-rw-r--r--   0        0        0        0 2023-12-24 00:26:28.675700 tfprovider-0.1.1.post1/tfprovider/level1/_sync/__init__.py
+-rw-r--r--   0        0        0      244 2023-12-24 00:26:28.675700 tfprovider-0.1.1.post1/tfprovider/level1/_sync/rpc_plugin_server.py
+-rw-r--r--   0        0        0      305 2023-11-05 00:40:05.943675 tfprovider-0.1.1.post1/tfprovider/level1/proto/grpc_controller.proto
+-rw-r--r--   0        0        0    14045 2023-10-22 16:13:49.250288 tfprovider-0.1.1.post1/tfprovider/level1/proto/tfplugin64.proto
+-rw-r--r--   0        0        0      245 2023-12-19 00:16:10.175668 tfprovider-0.1.1.post1/tfprovider/level1/rpc_plugin.py
+-rw-r--r--   0        0        0      372 2023-12-05 20:36:29.465044 tfprovider-0.1.1.post1/tfprovider/level2/__init__.py
+-rw-r--r--   0        0        0     1884 2023-12-17 00:18:55.229017 tfprovider-0.1.1.post1/tfprovider/level2/attribute_path.py
+-rw-r--r--   0        0        0     1845 2023-12-17 00:15:27.738079 tfprovider-0.1.1.post1/tfprovider/level2/diagnostics.py
+-rw-r--r--   0        0        0     2985 2023-12-20 01:30:37.689430 tfprovider-0.1.1.post1/tfprovider/level2/dynamic_value.py
+-rw-r--r--   0        0        0     3170 2023-12-17 15:42:46.152919 tfprovider-0.1.1.post1/tfprovider/level2/usable_schema.py
+-rw-r--r--   0        0        0     4098 2023-12-23 23:44:58.763979 tfprovider-0.1.1.post1/tfprovider/level2/wire_format.py
+-rw-r--r--   0        0        0    17151 2023-12-23 23:38:44.319275 tfprovider-0.1.1.post1/tfprovider/level2/wire_marshaling.py
+-rw-r--r--   0        0        0     5321 2023-12-23 14:02:13.408042 tfprovider-0.1.1.post1/tfprovider/level2/wire_representation.py
+-rw-r--r--   0        0        0      186 2023-12-10 14:46:35.908279 tfprovider-0.1.1.post1/tfprovider/level3/__init__.py
+-rw-r--r--   0        0        0    11181 2023-12-23 23:44:13.719416 tfprovider-0.1.1.post1/tfprovider/level3/statically_typed_schema.py
+-rw-r--r--   0        0        0      203 2023-12-15 00:18:21.473233 tfprovider-0.1.1.post1/tfprovider/level4/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-13 01:01:19.378306 tfprovider-0.1.1.post1/tfprovider/level4/_async/__init__.py
+-rw-r--r--   0        0        0    15828 2023-12-23 17:20:24.769094 tfprovider-0.1.1.post1/tfprovider/level4/_async/provider_servicer.py
+-rw-r--r--   0        0        0        0 2023-12-24 00:26:28.691700 tfprovider-0.1.1.post1/tfprovider/level4/_sync/__init__.py
+-rw-r--r--   0        0        0    15646 2023-12-24 00:26:28.691700 tfprovider-0.1.1.post1/tfprovider/level4/_sync/provider_servicer.py
+-rw-r--r--   0        0        0      168 2023-12-15 00:18:59.657813 tfprovider-0.1.1.post1/tfprovider/level4/async_provider_servicer.py
+-rw-r--r--   0        0        0      167 2023-12-15 00:19:14.742041 tfprovider-0.1.1.post1/tfprovider/level4/provider_servicer.py
+-rw-r--r--   0        0        0      521 2023-12-23 17:18:39.407775 tfprovider-0.1.1.post1/tfprovider/level4/utils.py
+-rw-r--r--   0        0        0        0 2023-12-21 01:30:55.795144 tfprovider-0.1.1.post1/tfprovider/py.typed
+-rw-r--r--   0        0        0   323052 2023-12-04 23:52:47.317804 tfprovider-0.1.1.post1/tfprovider/tfprovider.png
+-rw-r--r--   0        0        0      114 2023-12-04 23:52:14.841393 tfprovider-0.1.1.post1/tfprovider/tfprovider_level3.png
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 tfprovider-0.1.1.post1/PKG-INFO
```

### Comparing `tfprovider-0.1.1/LICENSE` & `tfprovider-0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/README.md` & `tfprovider-0.1.1.post1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,53 @@
+Metadata-Version: 2.1
+Name: tfprovider
+Version: 0.1.1.post1
+Summary: Implement Terraform providers in Python
+Home-page: https://smheidrich.gitlab.io/tfprovider-python/
+License: MPL-2.0
+Author: smheidrich
+Author-email: smheidrich@weltenfunktion.de
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: cryptography (>=41.0.4,<42.0.0)
+Requires-Dist: grpcio (>=1.59.0,<2.0.0)
+Requires-Dist: grpcio-health-checking (>=1.59.0,<2.0.0)
+Requires-Dist: hc-go-plugin-server (>=0.1.0,<0.2.0)
+Requires-Dist: msgpack (>=1.0.7,<2.0.0)
+Requires-Dist: tfplugin-proto-all (>=0.1.0,<0.2.0)
+Project-URL: Documentation, https://smheidrich.gitlab.io/tfprovider-python/
+Project-URL: Repository, https://gitlab.com/smheidrich/tfprovider-python
+Description-Content-Type: text/markdown
+
 # tfprovider(-python)
 
 This is a library to allow you to write Terraform providers in Python.
 
-NOT USABLE YET for anyone but myself, trust me.
+To actually deploy providers that use this library, you'll probably want to use
+a packaging system like
+[terradep-python](https://pypi.org/project/terradep-python/).
+
+## Project status
+
+**NOT USABLE YET** for anyone but myself, trust me.
+
+**If this would be useful for you once completed, just let me know in an
+issue** and I'll see what I can do to finish it. There is just no point working
+on this if nobody needs it, and my own use case isn't as important to me
+anymore, so I've put it on hold for now.
 
 ## Implemented/missing features
 
 If you need any of these, please either open an issue (on GitLab or GitHub,
 doesn't matter to me) or comment on an existing one and I'll see what I can do.
-In contrast to larger projects, I prefer +1 comments over thumbs ups *for now*
-(!) because they are easier for me to get notified of.
+In contrast to larger projects, I actually prefer +1 comments over thumbs ups
+*for now* (!) because they are easier for me to get notified of.
 
 Most of them aren't difficult or time-consuming for me to implement, there is
 just no point doing it if nobody needs it.
 
 - General:
   - [ ] Not being completely horrible to use and full of bugs
 - Kinds of Terraform objects:
@@ -27,16 +61,20 @@
   - [ ] Anything else, including more complex types
 - Miscellaneous features:
   - [ ] Private state
   - [ ] Upgrading state from earlier versions
     - Currently has an API for this that can't possibly work => needs overhaul
 - Utilities:
   - [ ] Automatic comparison for `requires_replace`
+- Infrastructure:
+  - [ ] Possibly tighter integration with
+    [terradep-python](https://pypi.org/project/terradep-python/)
 
 ## Development
 
 ### Sync/Async variants
 
 The sync variant of the API is automatically generated from the async one
 using [unasync](https://pypi.org/project/unasync/). With dev dependencies
 installed, you can regenerate them by running `run_unasync.py` as a Python
 script (e.g. via `poetry run run_unasync.py`).
+
```

### Comparing `tfprovider-0.1.1/pyproject.toml` & `tfprovider-0.1.1.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tfprovider"
-version = "0.1.1"
+version = "0.1.1.post1"
 description = "Implement Terraform providers in Python"
 authors = ["smheidrich <smheidrich@weltenfunktion.de>"]
 readme = "README.md"
 homepage = "https://smheidrich.gitlab.io/tfprovider-python/"
 repository = "https://gitlab.com/smheidrich/tfprovider-python"
 documentation = "https://smheidrich.gitlab.io/tfprovider-python/"
 license = "MPL-2.0"
```

### Comparing `tfprovider-0.1.1/tfprovider/level1/proto/tfplugin64.proto` & `tfprovider-0.1.1.post1/tfprovider/level1/proto/tfplugin64.proto`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level2/attribute_path.py` & `tfprovider-0.1.1.post1/tfprovider/level2/attribute_path.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level2/diagnostics.py` & `tfprovider-0.1.1.post1/tfprovider/level2/diagnostics.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level2/dynamic_value.py` & `tfprovider-0.1.1.post1/tfprovider/level2/dynamic_value.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level2/usable_schema.py` & `tfprovider-0.1.1.post1/tfprovider/level2/usable_schema.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level2/wire_format.py` & `tfprovider-0.1.1.post1/tfprovider/level2/wire_format.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level2/wire_marshaling.py` & `tfprovider-0.1.1.post1/tfprovider/level2/wire_marshaling.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level2/wire_representation.py` & `tfprovider-0.1.1.post1/tfprovider/level2/wire_representation.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level3/statically_typed_schema.py` & `tfprovider-0.1.1.post1/tfprovider/level3/statically_typed_schema.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level4/_async/provider_servicer.py` & `tfprovider-0.1.1.post1/tfprovider/level4/_async/provider_servicer.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level4/_sync/provider_servicer.py` & `tfprovider-0.1.1.post1/tfprovider/level4/_sync/provider_servicer.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/level4/utils.py` & `tfprovider-0.1.1.post1/tfprovider/level4/utils.py`

 * *Files identical despite different names*

### Comparing `tfprovider-0.1.1/tfprovider/tfprovider.png` & `tfprovider-0.1.1.post1/tfprovider/tfprovider.png`

 * *Files identical despite different names*

