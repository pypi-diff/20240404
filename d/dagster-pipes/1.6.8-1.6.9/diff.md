# Comparing `tmp/dagster-pipes-1.6.8.tar.gz` & `tmp/dagster-pipes-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pipes-1.6.8.tar", last modified: Fri Mar  1 19:13:24 2024, max compression
+gzip compressed data, was "dagster-pipes-1.6.9.tar", last modified: Fri Mar  8 00:18:54 2024, max compression
```

## Comparing `dagster-pipes-1.6.8.tar` & `dagster-pipes-1.6.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:13:24.272558 dagster-pipes-1.6.8/
--rw-r--r--   0 root         (0) root         (0)    11348 2024-03-01 19:11:21.000000 dagster-pipes-1.6.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-01 19:11:21.000000 dagster-pipes-1.6.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      794 2024-03-01 19:13:24.272558 dagster-pipes-1.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2024-03-01 19:11:21.000000 dagster-pipes-1.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:13:24.272558 dagster-pipes-1.6.8/dagster_pipes/
--rw-r--r--   0 root         (0) root         (0)    48179 2024-03-01 19:11:21.000000 dagster-pipes-1.6.8/dagster_pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-01 19:11:21.000000 dagster-pipes-1.6.8/dagster_pipes/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-01 19:11:21.000000 dagster-pipes-1.6.8/dagster_pipes/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:13:24.272558 dagster-pipes-1.6.8/dagster_pipes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      794 2024-03-01 19:13:23.000000 dagster-pipes-1.6.8/dagster_pipes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-03-01 19:13:23.000000 dagster-pipes-1.6.8/dagster_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 19:13:23.000000 dagster-pipes-1.6.8/dagster_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 19:13:23.000000 dagster-pipes-1.6.8/dagster_pipes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-01 19:13:23.000000 dagster-pipes-1.6.8/dagster_pipes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2024-03-01 19:13:24.276558 dagster-pipes-1.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1313 2024-03-01 19:11:21.000000 dagster-pipes-1.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:54.034186 dagster-pipes-1.6.9/
+-rw-r--r--   0 root         (0) root         (0)    11348 2024-03-08 00:17:46.000000 dagster-pipes-1.6.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-03-08 00:17:46.000000 dagster-pipes-1.6.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      794 2024-03-08 00:18:54.034186 dagster-pipes-1.6.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2024-03-08 00:17:46.000000 dagster-pipes-1.6.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:54.030186 dagster-pipes-1.6.9/dagster_pipes/
+-rw-r--r--   0 root         (0) root         (0)    48163 2024-03-08 00:17:46.000000 dagster-pipes-1.6.9/dagster_pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-03-08 00:17:46.000000 dagster-pipes-1.6.9/dagster_pipes/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-08 00:17:46.000000 dagster-pipes-1.6.9/dagster_pipes/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:54.034186 dagster-pipes-1.6.9/dagster_pipes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      794 2024-03-08 00:18:53.000000 dagster-pipes-1.6.9/dagster_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-03-08 00:18:53.000000 dagster-pipes-1.6.9/dagster_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:18:53.000000 dagster-pipes-1.6.9/dagster_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:18:53.000000 dagster-pipes-1.6.9/dagster_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2024-03-08 00:18:53.000000 dagster-pipes-1.6.9/dagster_pipes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2024-03-08 00:18:54.034186 dagster-pipes-1.6.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-03-08 00:17:46.000000 dagster-pipes-1.6.9/setup.py
```

### Comparing `dagster-pipes-1.6.8/LICENSE` & `dagster-pipes-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pipes-1.6.8/PKG-INFO` & `dagster-pipes-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.6.8
+Version: 1.6.9
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.6.8/dagster_pipes/__init__.py` & `dagster-pipes-1.6.9/dagster_pipes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,16 +558,15 @@
             a blob store.
         """
         channel = self.make_channel(params)
         with channel.buffered_upload_loop():
             yield channel
 
     @abstractmethod
-    def make_channel(self, params: PipesParams) -> T_BlobStoreMessageWriterChannel:
-        ...
+    def make_channel(self, params: PipesParams) -> T_BlobStoreMessageWriterChannel: ...
 
 
 class PipesBlobStoreMessageWriterChannel(PipesMessageWriterChannel):
     """Message writer channel that periodically uploads message chunks to some blob store endpoint."""
 
     def __init__(self, *, interval: float = 10):
         self._interval = interval
@@ -580,16 +579,15 @@
     def flush_messages(self) -> Sequence[PipesMessage]:
         items = []
         while not self._buffer.empty():
             items.append(self._buffer.get())
         return items
 
     @abstractmethod
-    def upload_messages_chunk(self, payload: StringIO, index: int) -> None:
-        ...
+    def upload_messages_chunk(self, payload: StringIO, index: int) -> None: ...
 
     @contextmanager
     def buffered_upload_loop(self) -> Iterator[None]:
         thread = None
         is_session_closed = Event()
         try:
             thread = Thread(target=self._upload_loop, args=(is_session_closed,), daemon=True)
```

### Comparing `dagster-pipes-1.6.8/dagster_pipes.egg-info/PKG-INFO` & `dagster-pipes-1.6.9/dagster_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.6.8
+Version: 1.6.9
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.6.8/setup.py` & `dagster-pipes-1.6.9/setup.py`

 * *Files identical despite different names*

