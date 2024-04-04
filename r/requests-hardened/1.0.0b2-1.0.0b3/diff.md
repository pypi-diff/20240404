# Comparing `tmp/requests-hardened-1.0.0b2.tar.gz` & `tmp/requests-hardened-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests-hardened-1.0.0b2.tar", last modified: Fri Sep 29 13:10:32 2023, max compression
+gzip compressed data, was "requests-hardened-1.0.0b3.tar", last modified: Thu Apr  4 14:06:54 2024, max compression
```

## Comparing `requests-hardened-1.0.0b2.tar` & `requests-hardened-1.0.0b3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 13:10:32.505266 requests-hardened-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-09-29 13:10:32.505266 requests-hardened-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 13:10:32.501266 requests-hardened-1.0.0b2/requests_hardened/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/requests_hardened/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/requests_hardened/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/requests_hardened/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/requests_hardened/host_header_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/requests_hardened/ip_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/requests_hardened/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/requests_hardened/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 13:10:32.501266 requests-hardened-1.0.0b2/requests_hardened.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-09-29 13:10:32.000000 requests-hardened-1.0.0b2/requests_hardened.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-09-29 13:10:32.000000 requests-hardened-1.0.0b2/requests_hardened.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 13:10:32.000000 requests-hardened-1.0.0b2/requests_hardened.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 13:10:32.000000 requests-hardened-1.0.0b2/requests_hardened.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-09-29 13:10:32.000000 requests-hardened-1.0.0b2/requests_hardened.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-29 13:10:32.000000 requests-hardened-1.0.0b2/requests_hardened.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-29 13:10:32.505266 requests-hardened-1.0.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 13:10:32.505266 requests-hardened-1.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/tests/test_default_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/tests/test_dummy_sni_tls_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/tests/test_dummy_tls_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/tests/test_never_allow_redirects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/tests/test_override_user_agent_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    10810 2023-09-29 13:10:16.000000 requests-hardened-1.0.0b2/tests/test_ssrf_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:06:54.838660 requests-hardened-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-04 14:06:54.838660 requests-hardened-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:06:54.834660 requests-hardened-1.0.0b3/requests_hardened/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/requests_hardened/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/requests_hardened/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/requests_hardened/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/requests_hardened/host_header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/requests_hardened/ip_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/requests_hardened/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/requests_hardened/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:06:54.838660 requests-hardened-1.0.0b3/requests_hardened.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-04 14:06:54.000000 requests-hardened-1.0.0b3/requests_hardened.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-04 14:06:54.000000 requests-hardened-1.0.0b3/requests_hardened.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:06:54.000000 requests-hardened-1.0.0b3/requests_hardened.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:06:54.000000 requests-hardened-1.0.0b3/requests_hardened.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 14:06:54.000000 requests-hardened-1.0.0b3/requests_hardened.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 14:06:54.000000 requests-hardened-1.0.0b3/requests_hardened.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:06:54.838660 requests-hardened-1.0.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:06:54.838660 requests-hardened-1.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/tests/test_default_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/tests/test_dummy_sni_tls_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/tests/test_dummy_tls_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/tests/test_never_allow_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/tests/test_override_user_agent_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-04 14:06:47.000000 requests-hardened-1.0.0b3/tests/test_ssrf_filter.py
```

### Comparing `requests-hardened-1.0.0b2/LICENSE` & `requests-hardened-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/PKG-INFO` & `requests-hardened-1.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-hardened
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A library that overrides the default behaviors of the requests library, and adds new security features.
 Author-email: Saleor Commerce <hello@saleor.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/saleor/requests-hardened/
 Project-URL: Source, https://github.com/saleor/requests-hardened/
 Project-URL: Issues, https://github.com/saleor/requests-hardened/issues
 Project-URL: Changelog, https://github.com/saleor/requests-hardened/releases/
```

### Comparing `requests-hardened-1.0.0b2/README.rst` & `requests-hardened-1.0.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/pyproject.toml` & `requests-hardened-1.0.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 readme = "README.rst"
 description = "A library that overrides the default behaviors of the requests library, and adds new security features."
 authors = [
     { name = "Saleor Commerce", email = "hello@saleor.io" }
 ]
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.8"
-version = "1.0.0b2"
+version = "1.0.0b3"
 dependencies = [
     'requests>=2.0.1,<3.0.0'
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
@@ -67,8 +67,8 @@
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 show_traceback = true
 
 exclude = [
     "tests/"
-]
+]
```

### Comparing `requests-hardened-1.0.0b2/requests_hardened/client.py` & `requests-hardened-1.0.0b3/requests_hardened/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,18 +27,21 @@
         if not timeout:
             kwargs["timeout"] = self._config.default_timeout
         return super().send(request, **kwargs)
 
     def prepare_request(self, request: Request) -> PreparedRequest:
         url = request.url
         if self._config.ip_filter_enable is True:
-            headers = request.headers or {}
-            # Cast potentially immutable header list to `dict`
-            if not isinstance(headers, dict):
-                headers = cast(dict, dict(**headers))
+            # IP filter will change headers, ensure copying because headers might be a global variable used by other requests
+            # ex. https://github.com/lepture/authlib/blob/a7d68b4c3b8a3a7fe0b62943b5228669f2f3dfec/authlib/oauth2/client.py#L205-L206
+            if request.headers:
+                headers = dict(**request.headers)
+            else:
+                headers = {}
+
             # Cast `bytes` to `str`
             if isinstance(url, bytes):
                 url = url.decode()
 
             url = filter_request(
                 url,
                 headers=headers,
```

### Comparing `requests-hardened-1.0.0b2/requests_hardened/config.py` & `requests-hardened-1.0.0b3/requests_hardened/config.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/requests_hardened/host_header_adapter.py` & `requests-hardened-1.0.0b3/requests_hardened/host_header_adapter.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/requests_hardened/ip_filter.py` & `requests-hardened-1.0.0b3/requests_hardened/ip_filter.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/requests_hardened/manager.py` & `requests-hardened-1.0.0b3/requests_hardened/manager.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/requests_hardened.egg-info/PKG-INFO` & `requests-hardened-1.0.0b3/requests_hardened.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-hardened
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A library that overrides the default behaviors of the requests library, and adds new security features.
 Author-email: Saleor Commerce <hello@saleor.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/saleor/requests-hardened/
 Project-URL: Source, https://github.com/saleor/requests-hardened/
 Project-URL: Issues, https://github.com/saleor/requests-hardened/issues
 Project-URL: Changelog, https://github.com/saleor/requests-hardened/releases/
```

### Comparing `requests-hardened-1.0.0b2/requests_hardened.egg-info/SOURCES.txt` & `requests-hardened-1.0.0b3/requests_hardened.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/tests/test_default_timeout.py` & `requests-hardened-1.0.0b3/tests/test_default_timeout.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/tests/test_dummy_sni_tls_server.py` & `requests-hardened-1.0.0b3/tests/test_dummy_sni_tls_server.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/tests/test_dummy_tls_server.py` & `requests-hardened-1.0.0b3/tests/test_dummy_tls_server.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/tests/test_never_allow_redirects.py` & `requests-hardened-1.0.0b3/tests/test_never_allow_redirects.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/tests/test_override_user_agent_header.py` & `requests-hardened-1.0.0b3/tests/test_override_user_agent_header.py`

 * *Files identical despite different names*

### Comparing `requests-hardened-1.0.0b2/tests/test_ssrf_filter.py` & `requests-hardened-1.0.0b3/tests/test_ssrf_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -317,7 +317,28 @@
     exc = exc_info.value.args[0]
     assert isinstance(exc, MaxRetryError)
     original_exception = exc.reason.args[0]
     assert isinstance(original_exception, CertificateError)
     assert (
         original_exception.args[0] == "hostname 'sni.local' doesn't match 'localhost'"
     )
+
+
+@pytest.mark.fake_resolver(enabled=False)
+@mock.patch("requests.sessions.Session.send")
+def test_pass_headers_reference(mocked_send: mock.MagicMock):
+    """
+    Ensure headers passed to IP filter are not modified in place but rather copied.
+    """
+    input_headers = {"foo": "bar"}
+
+    with mock_getaddrinfo("128.99.0.0"):
+        SSRFFilter.send_request("GET", "https://test.local", headers=input_headers)
+        mocked_send.assert_called_once()
+
+        [prepared_request], kwargs = mocked_send.call_args
+        assert isinstance(prepared_request, PreparedRequest)
+        assert prepared_request.method == "GET"
+        assert prepared_request.url == "https://128.99.0.0:443/"
+        assert "Host" not in input_headers
+        assert "Host" in prepared_request.headers
+        assert prepared_request.headers.get("Host") == "test.local"
```

