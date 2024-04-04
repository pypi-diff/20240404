# Comparing `tmp/alcedo-0.1.5.tar.gz` & `tmp/alcedo-0.1.6.tar.gz`

## Comparing `alcedo-0.1.5.tar` & `alcedo-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,51 @@
--rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 alcedo-0.1.5/Cargo.toml
--rw-r--r--   0      501       20      392 2024-03-22 18:34:20.000000 alcedo-0.1.5/.gitignore
--rw-r--r--   0      501       20     1072 2024-03-22 05:37:01.000000 alcedo-0.1.5/LICENSE
--rw-r--r--   0      501       20     6711 2024-03-25 08:48:02.000000 alcedo-0.1.5/README.md
--rw-r--r--   0      501       20     1065 2024-03-27 14:18:42.000000 alcedo-0.1.5/alcedo.pyi
--rw-r--r--   0      501       20   115533 2024-03-21 16:49:27.000000 alcedo-0.1.5/poetry.lock
--rw-r--r--   0      501       20     2282 2024-03-27 14:07:20.000000 alcedo-0.1.5/pyproject.toml
--rw-r--r--   0      501       20     3074 2024-03-27 11:27:41.000000 alcedo-0.1.5/src/client.rs
--rw-r--r--   0      501       20     3181 2024-03-27 09:16:22.000000 alcedo-0.1.5/src/dictionary.rs
--rw-r--r--   0      501       20     2352 2024-03-23 17:24:27.000000 alcedo-0.1.5/src/json_value.rs
--rw-r--r--   0      501       20     1288 2024-03-27 09:05:43.000000 alcedo-0.1.5/src/lib.rs
--rw-r--r--   0      501       20     1977 2024-03-27 09:09:09.000000 alcedo-0.1.5/src/response.rs
--rw-r--r--   0      501       20   565477 2024-03-22 18:14:20.000000 alcedo-0.1.5/static/alcedo-banner.svg
--rw-r--r--   0      501       20   147962 2024-03-25 08:22:46.000000 alcedo-0.1.5/static/alcedo-preview.png
--rw-r--r--   0      501       20   567105 2024-03-25 06:59:07.000000 alcedo-0.1.5/static/alcedo-preview.svg
--rw-r--r--   0      501       20   363124 2024-03-20 16:54:52.000000 alcedo-0.1.5/static/alcedo.base64
--rw-r--r--   0      501       20   272342 2024-03-20 16:54:36.000000 alcedo-0.1.5/static/alcedo.svg
--rw-r--r--   0      501       20     1970 2024-03-27 14:15:12.000000 alcedo-0.1.5/tests/__init__.py
--rw-r--r--   0      501       20     1948 2024-03-27 14:15:42.000000 alcedo-0.1.5/tests/conftest.py
--rw-r--r--   0      501       20      479 2024-03-27 14:14:33.000000 alcedo-0.1.5/tests/get/__init__.py
--rw-r--r--   0      501       20      956 2024-03-27 14:14:09.000000 alcedo-0.1.5/tests/get/bench.py
--rw-r--r--   0      501       20     1046 2024-03-27 14:13:43.000000 alcedo-0.1.5/tests/get/bench_httpx.py
--rw-r--r--   0      501       20     1070 2024-03-27 14:13:02.000000 alcedo-0.1.5/tests/get/bench_requests.py
--rw-r--r--   0      501       20      495 2024-03-27 14:10:10.000000 alcedo-0.1.5/tests/session/get/__init__.py
--rw-r--r--   0      501       20     1093 2024-03-27 14:09:30.000000 alcedo-0.1.5/tests/session/get/bench.py
--rw-r--r--   0      501       20     1382 2024-03-27 14:10:49.000000 alcedo-0.1.5/tests/session/get/bench_aiohttp.py
--rw-r--r--   0      501       20     1183 2024-03-27 14:08:53.000000 alcedo-0.1.5/tests/session/get/bench_httpx.py
--rw-r--r--   0      501       20     1223 2024-03-27 14:08:12.000000 alcedo-0.1.5/tests/session/get/bench_requests.py
--rw-r--r--   0      501       20      497 2024-03-27 14:12:01.000000 alcedo-0.1.5/tests/session/post/__init__.py
--rw-r--r--   0      501       20      693 2024-03-27 14:11:30.000000 alcedo-0.1.5/tests/session/post/bench.py
--rw-r--r--   0      501       20      895 2024-03-27 14:12:36.000000 alcedo-0.1.5/tests/session/post/bench_aiohttp.py
--rw-r--r--   0      501       20      822 2024-03-27 14:11:21.000000 alcedo-0.1.5/tests/session/post/bench_httpx.py
--rw-r--r--   0      501       20      840 2024-03-27 14:11:09.000000 alcedo-0.1.5/tests/session/post/bench_requests.py
--rw-r--r--   0      501       20    35157 2024-03-27 14:18:58.000000 alcedo-0.1.5/Cargo.lock
--rw-r--r--   0        0        0     7925 1970-01-01 00:00:00.000000 alcedo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 alcedo-0.1.6/Cargo.toml
+-rw-r--r--   0      501       20      392 2024-03-22 18:34:20.000000 alcedo-0.1.6/.gitignore
+-rw-r--r--   0      501       20     1072 2024-03-22 05:37:01.000000 alcedo-0.1.6/LICENSE
+-rw-r--r--   0      501       20     6769 2024-03-28 09:16:55.000000 alcedo-0.1.6/README.md
+-rw-r--r--   0      501       20     1316 2024-04-04 08:08:19.000000 alcedo-0.1.6/alcedo.pyi
+-rw-r--r--   0      501       20     2067 2024-03-28 09:17:30.000000 alcedo-0.1.6/benchmarks.md
+-rw-r--r--   0      501       20   115533 2024-03-21 16:49:27.000000 alcedo-0.1.6/poetry.lock
+-rw-r--r--   0      501       20     2271 2024-04-04 08:08:03.000000 alcedo-0.1.6/pyproject.toml
+-rw-r--r--   0      501       20     4023 2024-04-04 08:03:13.000000 alcedo-0.1.6/src/client.rs
+-rw-r--r--   0      501       20     3172 2024-04-01 00:41:10.000000 alcedo-0.1.6/src/dictionary.rs
+-rw-r--r--   0      501       20     2352 2024-03-23 17:24:27.000000 alcedo-0.1.6/src/json_value.rs
+-rw-r--r--   0      501       20     1310 2024-04-01 00:47:44.000000 alcedo-0.1.6/src/lib.rs
+-rw-r--r--   0      501       20     1977 2024-03-27 09:09:09.000000 alcedo-0.1.6/src/response.rs
+-rw-r--r--   0      501       20   565477 2024-03-22 18:14:20.000000 alcedo-0.1.6/static/alcedo-banner.svg
+-rw-r--r--   0      501       20   147962 2024-03-25 08:22:46.000000 alcedo-0.1.6/static/alcedo-preview.png
+-rw-r--r--   0      501       20   567105 2024-03-25 06:59:07.000000 alcedo-0.1.6/static/alcedo-preview.svg
+-rw-r--r--   0      501       20   363124 2024-03-20 16:54:52.000000 alcedo-0.1.6/static/alcedo.base64
+-rw-r--r--   0      501       20   272342 2024-03-20 16:54:36.000000 alcedo-0.1.6/static/alcedo.svg
+-rw-r--r--   0      501       20     2721 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/__init__.py
+-rw-r--r--   0      501       20     1948 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/conftest.py
+-rw-r--r--   0      501       20      479 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/get/__init__.py
+-rw-r--r--   0      501       20     1015 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/get/bench.py
+-rw-r--r--   0      501       20     1105 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/get/bench_httpx.py
+-rw-r--r--   0      501       20     1129 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/get/bench_requests.py
+-rw-r--r--   0      501       20      501 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/__init__.py
+-rw-r--r--   0      501       20      654 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/bench.py
+-rw-r--r--   0      501       20      847 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/bench_aiohttp.py
+-rw-r--r--   0      501       20      779 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/bench_httpx.py
+-rw-r--r--   0      501       20      804 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/delete/bench_requests.py
+-rw-r--r--   0      501       20      495 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/__init__.py
+-rw-r--r--   0      501       20     1152 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/bench.py
+-rw-r--r--   0      501       20     1543 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/bench_aiohttp.py
+-rw-r--r--   0      501       20     1242 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/bench_httpx.py
+-rw-r--r--   0      501       20     1282 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/get/bench_requests.py
+-rw-r--r--   0      501       20      497 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/__init__.py
+-rw-r--r--   0      501       20      691 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/bench.py
+-rw-r--r--   0      501       20      893 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/bench_aiohttp.py
+-rw-r--r--   0      501       20      820 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/bench_httpx.py
+-rw-r--r--   0      501       20      838 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/post/bench_requests.py
+-rw-r--r--   0      501       20      495 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/__init__.py
+-rw-r--r--   0      501       20      697 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/bench.py
+-rw-r--r--   0      501       20      890 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/bench_aiohttp.py
+-rw-r--r--   0      501       20      817 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/bench_httpx.py
+-rw-r--r--   0      501       20      842 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/put/bench_requests.py
+-rw-r--r--   0      501       20      513 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/__init__.py
+-rw-r--r--   0      501       20     1398 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/bench.py
+-rw-r--r--   0      501       20     1769 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/bench_aiohttp.py
+-rw-r--r--   0      501       20     1490 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/bench_httpx.py
+-rw-r--r--   0      501       20     1530 2024-04-04 08:08:19.000000 alcedo-0.1.6/tests/session/queried_get/bench_requests.py
+-rw-r--r--   0      501       20    35157 2024-04-04 08:08:08.000000 alcedo-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0     7983 1970-01-01 00:00:00.000000 alcedo-0.1.6/PKG-INFO
```

### Comparing `alcedo-0.1.5/LICENSE` & `alcedo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/README.md` & `alcedo-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,18 @@
 
 ## Example usage
 
 ```py
 print("Hello, World!")
 ```
 
+## Do you even bench bro?
+
+[Benchmarks](./benchmarks.md)
+
 ## Roadmap
 
 - Write (actual) asynchronous tests for `aiohttp` benchmarks.
 - Create asynchronous implementation for `alcedo.Client`.
 - Write asynchronous tests.
 - Write malformed-json test servers.
 - Create implementation where POST body can be attached.
```

### Comparing `alcedo-0.1.5/alcedo.pyi` & `alcedo-0.1.6/alcedo.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/alcedo.pyi
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-21 00:20
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
 ### Standard packages ###
 from typing import Any, Optional
 
 class Client:
   def __init__(self, headers: Optional[dict] = None, **kwargs: Any) -> None: ...
+  def delete(
+    self, url: str, headers: Optional[dict] = None, payload: dict = {}, **kwargs: Any
+  ) -> Response: ...
   def get(self, url: str, headers: Optional[dict] = None, **kwargs: Any) -> Response: ...
-  def post(self, url: str, headers: Optional[dict] = None, payload: dict = {}, **kwargs: Any) -> Response:
+  def post(
+    self, url: str, headers: Optional[dict] = None, payload: dict = {}, **kwargs: Any
+  ) -> Response: ...
+  def put(
+    self, url: str, headers: Optional[dict] = None, payload: dict = {}, **kwargs: Any
+  ) -> Response: ...
   def request(
     self, method: str, url: str, headers: Optional[dict] = None, **kwargs: Any
   ) -> Response: ...
 
 class Response:
   def __init__(self, **kwargs: Any) -> None: ...
   def json(self) -> dict: ...
```

### Comparing `alcedo-0.1.5/poetry.lock` & `alcedo-0.1.6/poetry.lock`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/pyproject.toml` & `alcedo-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 [tool.poetry]
 authors = [ 'Sitt Guruvanich <aekazitt+github@gmail.com>' ]
 description = 'Oxidized and Optimistic HTTP Client for Python'
 license = 'MIT'
 name = 'alcedo'
-version = '0.1.5'
+version = '0.1.6'
 packages = [{include='alcedo.pyi'}]
 
 
 [tool.poetry.dependencies]
 python = '^3.8'
 
 
@@ -68,15 +68,15 @@
 requests = '^2.31.0'
 ruff = '^0.3.3'
 uvicorn = '^0.29.0'
 types-requests = "^2.31.0.20240311"
 
 
 [tool.pytest.ini_options]
-addopts = '--durations=0 --tb=short'
+addopts = '--durations=0'
 markers = [
   'aiohttp: aiohttp benchmarks optional when running tests',
   'httpx: httpx benchmarks optional when running tests',
   'requests: requests benchmarks optional when running tests',
 ]
 python_files = '*.py'
 pythonpath = [ 'alcedo.pyi' ]
```

### Comparing `alcedo-0.1.5/src/client.rs` & `alcedo-0.1.6/src/client.rs`

 * *Files 23% similar despite different names*

```diff
@@ -23,65 +23,101 @@
 #[pyclass]
 pub struct Client {
     blocking_client: BlockingClient,
 }
 
 #[pymethods]
 impl Client {
+    fn delete(
+        &self,
+        url: &str,
+        headers: Option<HashMap<String, String>>,
+        query: Option<PyObject>,
+    ) -> PyResult<Response> {
+        Ok(self.request("DELETE", url, headers, query, None))
+    }
+
+    fn get(
+        &self,
+        url: &str,
+        headers: Option<HashMap<String, String>>,
+        query: Option<PyObject>,
+    ) -> PyResult<Response> {
+        Ok(self.request("GET", url, headers, query, None))
+    }
+
     #[new]
     fn new(h: Option<HashMap<String, String>>) -> Self {
         let headers = h.unwrap_or(HashMap::new());
         let hmap = dict_to_headers(headers);
         Self {
             blocking_client: BlockingClient::builder()
                 .default_headers(hmap)
                 .user_agent(APP_USER_AGENT)
                 .build()
                 .unwrap(),
         }
     }
 
-    fn get(&self, url: &str, headers: Option<HashMap<String, String>>) -> PyResult<Response> {
-        Ok(self.request("GET", url, headers, None))
+    fn post(
+        &self,
+        url: &str,
+        headers: Option<HashMap<String, String>>,
+        query: Option<PyObject>,
+        payload: Option<PyObject>,
+    ) -> PyResult<Response> {
+        Ok(self.request("POST", url, headers, query, payload))
     }
 
-    fn post(
+    fn put(
         &self,
         url: &str,
         headers: Option<HashMap<String, String>>,
+        query: Option<PyObject>,
         payload: Option<PyObject>,
     ) -> PyResult<Response> {
-        Ok(self.request("POST", url, headers, payload))
+        Ok(self.request("PUT", url, headers, query, payload))
     }
 
     fn request(
         &self,
         method: &str,
         url: &str,
         headers: Option<HashMap<String, String>>,
+        query: Option<PyObject>,
         payload: Option<PyObject>,
     ) -> Response {
         let builder = self
             .blocking_client
             .request(Method::from_bytes(method.as_bytes()).unwrap(), url)
             .headers(dict_to_headers(headers.unwrap_or(HashMap::new())));
-        let req: Result<RequestBuilder, RequestBuilder> = match payload {
+        let mut req: Result<RequestBuilder, RequestBuilder> = match payload {
             None => Ok(builder),
             Some(value) => Python::with_gil(|py| {
                 let d = Dictionary {
                     py,
                     obj: value.extract(py).unwrap(),
                 };
                 // let body = to_string(&d).map_err(ser::Error::custom);
                 let body = to_string(&d).unwrap();
                 Ok(builder
                     .header("Content-Type", "application/json")
                     .json(&json!(body)))
             }),
         };
+        req = match query {
+            None => req,
+            Some(value) => Python::with_gil(|py| {
+                let d = Dictionary {
+                    py,
+                    obj: value.extract(py).unwrap(),
+                };
+                Ok(req.unwrap().query(&d))
+            }),
+        };
         let response = req.unwrap().send().unwrap();
         let mut h: HashMap<String, String> = HashMap::with_capacity(response.headers().len());
         for (key, value) in response.headers().iter() {
             h.insert(key.to_string(), value.to_str().unwrap().to_string());
         }
         let status = response.status();
         Response {
```

### Comparing `alcedo-0.1.5/src/dictionary.rs` & `alcedo-0.1.6/src/dictionary.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // SPDX-License-Identifier: MIT
 
 use pyo3::types::{PyAny, PyDict, PyFloat, PyList, PyTuple};
-use pyo3::{FromPyObject, PyTryFrom, Python};
+use pyo3::{FromPyObject, Python};
 use serde::ser::{self, Serialize, SerializeMap, SerializeSeq, Serializer};
 use std::string::String;
 
 pub struct Dictionary<'p, 'a> {
     pub py: Python<'p>,
     pub obj: &'a PyAny,
 }
@@ -13,15 +13,15 @@
 impl<'p, 'a> Serialize for Dictionary<'p, 'a> {
     fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         macro_rules! cast {
             ($f:expr) => {
-                if let Ok(val) = PyTryFrom::try_from(self.obj) {
+                if let Ok(val) = FromPyObject::extract(self.obj) {
                     return $f(val);
                 }
             };
         }
 
         macro_rules! extract {
             ($t:ty) => {
```

### Comparing `alcedo-0.1.5/src/json_value.rs` & `alcedo-0.1.6/src/json_value.rs`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/src/lib.rs` & `alcedo-0.1.6/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // SPDX-License-Identifier: MIT
 
 use pyo3::exceptions::PyException;
 use pyo3::types::PyModule;
-use pyo3::{create_exception, pyfunction, pymodule, wrap_pyfunction, PyResult, Python};
+use pyo3::{create_exception, pyfunction, pymodule, wrap_pyfunction, Bound, PyResult};
 use reqwest::blocking::get as r_get;
 use std::collections::HashMap;
 use std::str::FromStr;
 static APP_USER_AGENT: &str = concat!(env!("CARGO_PKG_NAME"), "/", env!("CARGO_PKG_VERSION"),);
 
 mod client;
 mod dictionary;
@@ -33,13 +33,13 @@
             .collect::<HashMap<String, String>>(),
         body: response.text().unwrap(),
         reason: "lol".to_string(), // TODO: give me a reason
     })
 }
 
 #[pymodule]
-fn alcedo(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(get, m)?)?;
-    m.add_class::<client::Client>()?;
-    m.add_class::<Response>()?;
+fn alcedo(module: &Bound<'_, PyModule>) -> PyResult<()> {
+    module.add_function(wrap_pyfunction!(get, module)?)?;
+    module.add_class::<client::Client>()?;
+    module.add_class::<Response>()?;
     Ok(())
 }
```

### Comparing `alcedo-0.1.5/src/response.rs` & `alcedo-0.1.6/src/response.rs`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/static/alcedo-banner.svg` & `alcedo-0.1.6/static/alcedo-banner.svg`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/static/alcedo-preview.png` & `alcedo-0.1.6/static/alcedo-preview.png`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/static/alcedo-preview.svg` & `alcedo-0.1.6/static/alcedo-preview.svg`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/static/alcedo.base64` & `alcedo-0.1.6/static/alcedo.base64`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/static/alcedo.svg` & `alcedo-0.1.6/static/alcedo.svg`

 * *Files identical despite different names*

### Comparing `alcedo-0.1.5/tests/__init__.py` & `alcedo-0.1.6/tests/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,81 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/__init__.py
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-21 13:31
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION: https://www.w3docs.com/snippets/python/what-is-init-py-for.html
 #
 # HISTORY:
 # *************************************************************
 """Module indicating that `~~/tests` directory is present in is a Python package."""
 
 ### Standard packages ###
 from json import loads
 from multiprocessing import Process
+from urllib.parse import parse_qs
 from time import sleep
 from typing import Generator
 
 ### Third-party packages ###
 from fastapi import FastAPI
 from fastapi.requests import Request
 from fastapi.responses import JSONResponse, PlainTextResponse, ORJSONResponse
 from pytest import fixture
 from uvicorn import run
 
+RUNS: int = 1_000
 TEST_HOST: str = "localhost"
 TEST_PORT: int = 6969
 TEST_ENDPOINT: str = f"http://{ TEST_HOST }:{ TEST_PORT }"
 
 
 def run_test_server() -> None:
   app: FastAPI = FastAPI()
 
   @app.get("/plaintext", response_class=PlainTextResponse)
   async def plaintext_endpoint() -> str:
     return "OK"
 
   @app.get("/json", response_class=JSONResponse)
-  async def json_endpoint() -> dict:
-    return {"detail": "OK", "status": 200}
+  async def json_endpoint(request: Request) -> dict:
+    response = {
+      "detail": "OK",
+      "float": 1.234,
+      "integer": 200,
+      "null": None,
+    }
+    if len(request.query_params) > 0:
+      response["query"] = parse_qs(str(request.query_params))
+    return response
 
   @app.get("/orjson", response_class=ORJSONResponse)
-  async def orjson_endpoint() -> dict:
-    return {"detail": "OK", "status": 200}
+  async def orjson_endpoint(request: Request) -> dict:
+    response = {
+      "detail": "OK",
+      "float": 1.234,
+      "integer": 200,
+      "null": None,
+    }
+    if len(request.query_params) > 0:
+      response["query"] = parse_qs(str(request.query_params))
+    return response
 
-  @app.post("/create", response_class=JSONResponse)
+  @app.post("/create", response_class=JSONResponse, status_code=201)
   async def create_post(request: Request) -> dict:
-    return {"received": loads(await request.json())}
+    return {"created": loads(await request.json())}
+
+  @app.put("/update", response_class=JSONResponse)
+  async def update_post(request: Request) -> dict:
+    return {"updated": loads(await request.json())}
+
+  @app.delete("/delete", response_class=PlainTextResponse, status_code=204)
+  async def delete_post() -> None: ...
 
   run(app, host="localhost", port=6969)
 
 
 @fixture(scope="session", autouse=True)
 def setup_teardown_api_server() -> Generator:
   """
@@ -62,8 +87,8 @@
   process: Process = Process(daemon=True, target=run_test_server)
   process.start()
   sleep(0.5)  # setup-delay
   yield
   process.terminate()
 
 
-__all__ = ("TEST_ENDPOINT", "setup_teardown_api_server")
+__all__ = ("RUNS", "TEST_ENDPOINT", "setup_teardown_api_server")
```

### Comparing `alcedo-0.1.5/tests/conftest.py` & `alcedo-0.1.6/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/conftest.py
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-21 16:42
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
@@ -59,8 +59,8 @@
       item.add_marker(
         mark.skip(
           reason="Test excluded without flag; Add --bench-against-requests flag to run test."
         )
       )
 
 
-__all__ = ["pytest_addoption", "pytest_collection_modifyitems"]
+__all__ = ("pytest_addoption", "pytest_collection_modifyitems")
```

### Comparing `alcedo-0.1.5/tests/get/bench.py` & `alcedo-0.1.6/tests/get/bench_httpx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
-# FILENAME:    ~~/tests/get/bench.py
-# VERSION:     0.1.5
+# FILENAME:    ~~/tests/get/bench_httpx.py
+# VERSION:     0.1.6
 # CREATED:     2024-03-21 13:31
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
+### Third-party packages ###
+from httpx import Response, get
+from pytest import mark
+
 ### Local modules ###
-from alcedo import Response, get
 from tests import *
 
 
-def test_alcedo_get_json_endpoint() -> None:
-  for _ in range(1_000):
+@mark.httpx
+def test_httpx_get_json_endpoint() -> None:
+  for _ in range(RUNS):
     response: Response = get(f"{ TEST_ENDPOINT }/json")
-    assert response.json() == {"detail": "OK", "status": 200}
+    assert response.json() == {"detail": "OK", "float": 1.234, "integer": 200, "null": None}
 
 
-def test_alcedo_get_orjson_endpoint() -> None:
-  for _ in range(1_000):
+@mark.httpx
+def test_httpx_get_orjson_endpoint() -> None:
+  for _ in range(RUNS):
     response: Response = get(f"{ TEST_ENDPOINT }/orjson")
-    assert response.json() == {"detail": "OK", "status": 200}
+    assert response.json() == {"detail": "OK", "float": 1.234, "integer": 200, "null": None}
 
 
-def test_alcedo_get_plaintext_endpoint() -> None:
-  for _ in range(1_000):
+@mark.httpx
+def test_httpx_get_plaintext_endpoint() -> None:
+  for _ in range(RUNS):
     response: Response = get(f"{ TEST_ENDPOINT }/plaintext")
-    assert response.text() == "OK"
+    assert response.text == "OK"
```

### Comparing `alcedo-0.1.5/tests/get/bench_httpx.py` & `alcedo-0.1.6/tests/session/put/bench_aiohttp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
-# FILENAME:    ~~/tests/get/bench_httpx.py
-# VERSION:     0.1.5
-# CREATED:     2024-03-21 13:31
+# FILENAME:    ~~/tests/session/put/bench_aiohttp.py
+# VERSION:     0.1.6
+# CREATED:     2024-03-28 14:18
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
+### Standard packages ###
+from json import dumps
+
 ### Third-party packages ###
-from httpx import Response, get
+from aiohttp.client import ClientSession
 from pytest import mark
 
 ### Local modules ###
 from tests import *
 
 
-@mark.httpx
-def test_httpx_get_json_endpoint() -> None:
-  for _ in range(1_000):
-    response: Response = get(f"{ TEST_ENDPOINT }/json")
-    assert response.json() == {"detail": "OK", "status": 200}
-
-
-@mark.httpx
-def test_httpx_get_orjson_endpoint() -> None:
-  for _ in range(1_000):
-    response: Response = get(f"{ TEST_ENDPOINT }/orjson")
-    assert response.json() == {"detail": "OK", "status": 200}
-
-
-@mark.httpx
-def test_httpx_get_plaintext_endpoint() -> None:
-  for _ in range(1_000):
-    response: Response = get(f"{ TEST_ENDPOINT }/plaintext")
-    assert response.text == "OK"
+@mark.aiohttp
+@mark.asyncio
+async def test_aiohttp_client_session_put_update_endpoint() -> None:
+  async with ClientSession() as session:
+    for i in range(RUNS):
+      body: dict = {"hello": "world", "count": i}
+      async with session.put(f"{ TEST_ENDPOINT }/update", json=dumps(body)) as response:
+        assert await response.json() == {"updated": body}
```

### Comparing `alcedo-0.1.5/tests/session/get/bench.py` & `alcedo-0.1.6/tests/session/get/bench.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/get/bench.py
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
 ### Local modules ###
 from alcedo import Client, Response
 from tests import *
 
 
 def test_alcedo_client_get_json_endpoint() -> None:
   client: Client = Client()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = client.get(f"{ TEST_ENDPOINT }/json")
-    assert response.json() == {"detail": "OK", "status": 200}
+    assert response.json() == {"detail": "OK", "float": 1.234, "integer": 200, "null": None}
 
 
 def test_alcedo_client_get_orjson_endpoint() -> None:
   client: Client = Client()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = client.get(f"{ TEST_ENDPOINT }/orjson")
-    assert response.json() == {"detail": "OK", "status": 200}
+    assert response.json() == {"detail": "OK", "float": 1.234, "integer": 200, "null": None}
 
 
 def test_alcedo_client_get_plaintext_endpoint() -> None:
   client: Client = Client()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = client.get(f"{ TEST_ENDPOINT }/plaintext")
     assert response.text() == "OK"
```

### Comparing `alcedo-0.1.5/tests/session/get/bench_aiohttp.py` & `alcedo-0.1.6/tests/session/queried_get/bench_aiohttp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
-# FILENAME:    ~~/tests/session/get/bench_aiohttp.py
-# VERSION:     0.1.5
-# CREATED:     2024-03-25 02:00
+# FILENAME:    ~~/tests/session/queried_get/bench_aiohttp.py
+# VERSION:     0.1.6
+# CREATED:     2024-04-01 08:07
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
 ### Third-party packages ###
@@ -18,28 +18,44 @@
 from tests import *
 
 
 @mark.aiohttp
 @mark.asyncio
 async def test_aiohttp_client_session_get_json_endpoint() -> None:
   async with ClientSession() as session:
-    for _ in range(1_000):
-      async with session.get(f"{ TEST_ENDPOINT }/json") as response:
-        assert await response.json() == {"detail": "OK", "status": 200}
+    for i in range(RUNS):
+      async with session.get(
+        f"{ TEST_ENDPOINT }/json", params={"foo": "bar", "index": i}
+      ) as response:
+        assert await response.json() == {
+          "detail": "OK",
+          "float": 1.234,
+          "integer": 200,
+          "null": None,
+          "query": {"foo": ["bar"], "index": [f"{ i }"]},
+        }
 
 
 @mark.aiohttp
 @mark.asyncio
 async def test_aiohttp_client_session_get_orjson_endpoint() -> None:
   async with ClientSession() as session:
-    for _ in range(1_000):
-      async with session.get(f"{ TEST_ENDPOINT }/orjson") as response:
-        assert await response.json() == {"detail": "OK", "status": 200}
+    for i in range(RUNS):
+      async with session.get(
+        f"{ TEST_ENDPOINT }/orjson", params={"foo": "bar", "index": i}
+      ) as response:
+        assert await response.json() == {
+          "detail": "OK",
+          "float": 1.234,
+          "integer": 200,
+          "null": None,
+          "query": {"foo": ["bar"], "index": [f"{ i }"]},
+        }
 
 
 @mark.aiohttp
 @mark.asyncio
 async def test_aiohttp_client_session_get_plaintext_endpoint() -> None:
   async with ClientSession() as session:
-    for _ in range(1_000):
+    for _ in range(RUNS):
       async with session.get(f"{ TEST_ENDPOINT }/plaintext") as response:
         assert await response.text() == "OK"
```

### Comparing `alcedo-0.1.5/tests/session/get/bench_httpx.py` & `alcedo-0.1.6/tests/session/get/bench_httpx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/get/bench_httpx.py
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
@@ -17,26 +17,26 @@
 ### Local modules ###
 from tests import *
 
 
 @mark.httpx
 def test_httpx_client_get_json_endpoint() -> None:
   client: Client = Client()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = client.get(f"{ TEST_ENDPOINT }/json")
-    assert response.json() == {"detail": "OK", "status": 200}
+    assert response.json() == {"detail": "OK", "float": 1.234, "integer": 200, "null": None}
 
 
 @mark.httpx
 def test_httpx_client_get_orjson_endpoint() -> None:
   client: Client = Client()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = client.get(f"{ TEST_ENDPOINT }/orjson")
-    assert response.json() == {"detail": "OK", "status": 200}
+    assert response.json() == {"detail": "OK", "float": 1.234, "integer": 200, "null": None}
 
 
 @mark.httpx
 def test_httpx_client_get_plaintext_endpoint() -> None:
   client: Client = Client()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = client.get(f"{ TEST_ENDPOINT }/plaintext")
     assert response.text == "OK"
```

### Comparing `alcedo-0.1.5/tests/session/get/bench_requests.py` & `alcedo-0.1.6/tests/session/get/bench_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/get/bench_requests.py
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
@@ -17,26 +17,26 @@
 ### Local modules ###
 from tests import *
 
 
 @mark.requests
 def test_requests_session_get_json_endpoint() -> None:
   session: Session = Session()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = session.get(f"{ TEST_ENDPOINT }/json")
-    assert response.json() == {"detail": "OK", "status": 200}
+    assert response.json() == {"detail": "OK", "float": 1.234, "integer": 200, "null": None}
 
 
 @mark.requests
 def test_requests_session_get_orjson_endpoint() -> None:
   session: Session = Session()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = session.get(f"{ TEST_ENDPOINT }/orjson")
-    assert response.json() == {"detail": "OK", "status": 200}
+    assert response.json() == {"detail": "OK", "float": 1.234, "integer": 200, "null": None}
 
 
 @mark.requests
 def test_requests_session_get_plaintext_endpoint() -> None:
   session: Session = Session()
-  for _ in range(1_000):
+  for _ in range(RUNS):
     response: Response = session.get(f"{ TEST_ENDPOINT }/plaintext")
     assert response.text == "OK"
```

### Comparing `alcedo-0.1.5/tests/session/post/bench.py` & `alcedo-0.1.6/tests/session/delete/bench_httpx.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
-# FILENAME:    ~~/tests/session/post/bench.py
-# VERSION:     0.1.5
-# CREATED:     2024-03-27 16:29
+# FILENAME:    ~~/tests/session/delete/bench_httpx.py
+# VERSION:     0.1.6
+# CREATED:     2024-03-28 14:24
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
+### Standard packages ###
+from json import dumps
+
+### Third-party packages ###
+from httpx import Client, Response
+from pytest import mark
+
 ### Local modules ###
-from alcedo import Client, Response
 from tests import *
 
 
-def test_alcedo_client_post_create() -> None:
+@mark.httpx
+def test_httpx_client_delete_endpoint() -> None:
   client: Client = Client()
-  for i in range(1_000):
-    body: dict = {"hello": "world", "count": i + 1}
-    response: Response = client.post(f"{ TEST_ENDPOINT }/create", payload=body)
-    assert response.json() == {"received": body}
+  for _ in range(RUNS):
+    response: Response = client.delete(f"{ TEST_ENDPOINT }/delete")
+    assert response.status_code == 204
+    assert response.content == b""
```

### Comparing `alcedo-0.1.5/tests/session/post/bench_aiohttp.py` & `alcedo-0.1.6/tests/session/post/bench_aiohttp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/post/bench_aiohttp.py
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-25 02:00
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
@@ -21,11 +21,11 @@
 from tests import *
 
 
 @mark.aiohttp
 @mark.asyncio
 async def test_aiohttp_client_session_post_create_endpoint() -> None:
   async with ClientSession() as session:
-    for i in range(1_000):
+    for i in range(RUNS):
       body: dict = {"hello": "world", "count": i}
       async with session.post(f"{ TEST_ENDPOINT }/create", json=dumps(body)) as response:
-        assert await response.json() == {"received": body}
+        assert await response.json() == {"created": body}
```

### Comparing `alcedo-0.1.5/tests/session/post/bench_httpx.py` & `alcedo-0.1.6/tests/session/post/bench_httpx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/post/bench_httpx.py
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-27 20:58
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
@@ -20,11 +20,11 @@
 ### Local modules ###
 from tests import *
 
 
 @mark.httpx
 def test_httpx_client_post_create_endpoint() -> None:
   client: Client = Client()
-  for i in range(1_000):
+  for i in range(RUNS):
     body: dict = {"hello": "world", "count": i}
     response: Response = client.post(f"{ TEST_ENDPOINT }/create", json=dumps(body))
-    assert response.json() == {"received": body}
+    assert response.json() == {"created": body}
```

### Comparing `alcedo-0.1.5/tests/session/post/bench_requests.py` & `alcedo-0.1.6/tests/session/post/bench_requests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2024 All rights reserved.
 # FILENAME:    ~~/tests/session/post/bench_requests.py
-# VERSION:     0.1.5
+# VERSION:     0.1.6
 # CREATED:     2024-03-27 19:25
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 
@@ -20,11 +20,11 @@
 ### Local modules ###
 from tests import *
 
 
 @mark.requests
 def test_requests_session_client_post_endpoint() -> None:
   session: Session = Session()
-  for i in range(1_000):
+  for i in range(RUNS):
     body: dict = {"hello": "world", "count": i}
     response: Response = session.post(f"{ TEST_ENDPOINT }/create", json=dumps(body))
-    assert response.json() == {"received": body}
+    assert response.json() == {"created": body}
```

### Comparing `alcedo-0.1.5/Cargo.lock` & `alcedo-0.1.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "alcedo"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "pyo3",
  "reqwest",
  "serde",
  "serde_derive",
  "serde_json",
 ]
```

### Comparing `alcedo-0.1.5/PKG-INFO` & `alcedo-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcedo
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Rust
@@ -81,14 +81,18 @@
 
 ## Example usage
 
 ```py
 print("Hello, World!")
 ```
 
+## Do you even bench bro?
+
+[Benchmarks](./benchmarks.md)
+
 ## Roadmap
 
 - Write (actual) asynchronous tests for `aiohttp` benchmarks.
 - Create asynchronous implementation for `alcedo.Client`.
 - Write asynchronous tests.
 - Write malformed-json test servers.
 - Create implementation where POST body can be attached.
```

