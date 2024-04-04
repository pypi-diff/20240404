# Comparing `tmp/tuneapi-0.2.1.tar.gz` & `tmp/tuneapi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.2.1.tar", max compression
+gzip compressed data, was "tuneapi-0.2.2.tar", max compression
```

## Comparing `tuneapi-0.2.1.tar` & `tuneapi-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.1/README.md
--rw-r--r--   0        0        0      754 2024-03-30 14:01:20.531636 tuneapi-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       78 2024-03-30 14:01:16.957309 tuneapi-0.2.1/tuneapi/__init__.py
--rw-r--r--   0        0        0    19841 2024-03-30 12:55:22.405282 tuneapi-0.2.1/tuneapi/apis.py
--rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.1/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    14513 2024-03-30 06:43:42.005369 tuneapi-0.2.1/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1423 2024-03-11 17:27:02.931939 tuneapi-0.2.1/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.1/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.1/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.1/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.1/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3537 2024-03-11 17:26:50.020305 tuneapi-0.2.1/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.1/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4591 2024-03-25 09:31:00.226006 tuneapi-0.2.1/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.1/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     5547 2024-03-15 08:31:20.357021 tuneapi-0.2.1/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.1/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.1/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.2/README.md
+-rw-r--r--   0        0        0      754 2024-04-04 13:48:41.808466 tuneapi-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-04 13:48:41.818332 tuneapi-0.2.2/tuneapi/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.2/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6602 2024-03-31 13:35:11.551633 tuneapi-0.2.2/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.2/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.2/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0      309 2024-03-30 16:59:19.448589 tuneapi-0.2.2/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.2/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.2/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1423 2024-03-11 17:27:02.931939 tuneapi-0.2.2/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.2/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.2/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.2/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.2/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3537 2024-03-11 17:26:50.020305 tuneapi-0.2.2/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.2/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.2/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.2/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     5547 2024-03-15 08:31:20.357021 tuneapi-0.2.2/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.2/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.2/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.2/PKG-INFO
```

### Comparing `tuneapi-0.2.1/pyproject.toml` & `tuneapi-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.2.1"
+version = "0.2.2"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
```

### Comparing `tuneapi-0.2.1/tuneapi/types/chats.py` & `tuneapi-0.2.2/tuneapi/types/chats.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,19 @@
 
     def __add__(self, other):
         return Message(self.value + other, self.role)
 
     def __repr__(self) -> str:
         return str(self.value)
 
+    def __getitem__(self, x):
+        if x == "content":
+            return self.value
+        return getattr(self, x)
+
     def to_dict(self, ft: bool = False):
         """
         if `ft` then export to following format: `{"from": "system/human/gpt", "value": "..."}`
         else export to following format: `{"role": "system/user/assistant", "content": "..."}`
         """
         role = self.role
         if not ft:
@@ -173,21 +178,22 @@
             }
         return {
             "chats": [x.to_dict() for x in self.chats],
         }
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "Thread":
-        chats = data.get("chats", None) or data.get("conversations", None)
+        chats = data.get("chats", []) or data.get("conversations", [])
         if not chats:
             raise ValueError("No chats found")
         return cls(
-            chats=[Message.from_dict(x) for x in chats],
-            jl=data.get("jl"),
-            model=data.get("model"),
+            *[Message.from_dict(x) for x in chats],
+            i=data.get("id", ""),
+            jl=data.get("jl", ""),
+            model=data.get("model", ""),
             **data.get("meta", {}),
         )
 
     def to_ft(
         self, id: Any = None, drop_last: bool = False
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         chats = self.chats if not drop_last else self.chats[:-1]
```

### Comparing `tuneapi-0.2.1/tuneapi/utils/__init__.py` & `tuneapi-0.2.2/tuneapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/tuneapi/utils/fs.py` & `tuneapi-0.2.2/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/tuneapi/utils/logger.py` & `tuneapi-0.2.2/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/tuneapi/utils/mime.py` & `tuneapi-0.2.2/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/tuneapi/utils/misc.py` & `tuneapi-0.2.2/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/tuneapi/utils/networking.py` & `tuneapi-0.2.2/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/tuneapi/utils/parallel.py` & `tuneapi-0.2.2/tuneapi/utils/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         max_threads (int, optional): The maximum number of threads to use. Defaults to 20.
         post_fn (function, optional): A function to call with the result. Defaults to None.
         _name (str, optional): The name of the thread pool. Defaults to "".
         safe (bool, optional): If true, all caughts exceptions are in the results. Defaults to False.
     """
     _name = _name or str(uuid4())
     results = [None for _ in range(len(inputs))]
+    errors = []
     _pbar = trange(len(inputs), desc="Processing", unit="input") if pbar else None
     with ThreadPoolExecutor(max_workers=max_threads, thread_name_prefix=_name) as exe:
         _fn = lambda i, x: [i, fn(*x)]
         futures = {exe.submit(_fn, i, x): i for i, x in enumerate(inputs)}
         if not wait:
             return futures
         for future in as_completed(futures):
@@ -48,17 +49,19 @@
                     _pbar.update(1)
                 i, res = future.result()
                 if post_fn:
                     res = post_fn(res)
                 results[i] = res
             except Exception as e:
                 if safe:
-                    results[i] = e
+                    errors.append(e)
                 else:
                     raise e
+    if safe:
+        return results, errors
     return results
 
 
 def batched(iterable, n, ol=0, expand: bool = False, last: bool = True):
     """Convert any ``iterable`` to a generator of batches of size ``n``, last one may be smaller.
     Python 3.12 has ``itertools.batched`` which does the same thing.
```

### Comparing `tuneapi-0.2.1/tuneapi/utils/serdeser.py` & `tuneapi-0.2.2/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/tuneapi/utils/subway.py` & `tuneapi-0.2.2/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/tuneapi/utils/terminal.py` & `tuneapi-0.2.2/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.1/PKG-INFO` & `tuneapi-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: Apache 2.0
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

