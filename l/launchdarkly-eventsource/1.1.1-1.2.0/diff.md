# Comparing `tmp/launchdarkly_eventsource-1.1.1.tar.gz` & `tmp/launchdarkly_eventsource-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchdarkly_eventsource-1.1.1.tar", max compression
+gzip compressed data, was "launchdarkly_eventsource-1.2.0.tar", max compression
```

## Comparing `launchdarkly_eventsource-1.1.1.tar` & `launchdarkly_eventsource-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      557 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/LICENSE
--rw-r--r--   0        0        0     3976 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/README.md
--rw-r--r--   0        0        0       40 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/__init__.py
--rw-r--r--   0        0        0     3936 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/actions.py
--rw-r--r--   0        0        0      177 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/config/__init__.py
--rw-r--r--   0        0        0     4724 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/config/connect_strategy.py
--rw-r--r--   0        0        0     5908 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/config/error_strategy.py
--rw-r--r--   0        0        0     5924 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/config/retry_delay_strategy.py
--rw-r--r--   0        0        0      800 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/errors.py
--rw-r--r--   0        0        0     2850 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/http.py
--rw-r--r--   0        0        0     4557 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/reader.py
--rw-r--r--   0        0        0    14324 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/sse_client.py
--rw-r--r--   0        0        0       46 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/ld_eventsource/version.py
--rw-r--r--   0        0        0     1921 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/__init__.py
--rw-r--r--   0        0        0     2321 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/helpers.py
--rw-r--r--   0        0        0     6076 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/http_util.py
--rw-r--r--   0        0        0     1206 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/test_error_strategy.py
--rw-r--r--   0        0        0     5184 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/test_http_connect_strategy.py
--rw-r--r--   0        0        0     3315 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/test_http_connect_strategy_with_sse_client.py
--rw-r--r--   0        0        0     4606 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/test_reader.py
--rw-r--r--   0        0        0     2876 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/test_retry_delay_strategy.py
--rw-r--r--   0        0        0     2819 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/test_sse_client_basic.py
--rw-r--r--   0        0        0     3930 2024-03-01 18:48:37.827573 launchdarkly_eventsource-1.1.1/testing/test_sse_client_retry.py
--rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 launchdarkly_eventsource-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      557 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3976 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/README.md
+-rw-r--r--   0        0        0       40 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/__init__.py
+-rw-r--r--   0        0        0     3936 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/actions.py
+-rw-r--r--   0        0        0      177 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/config/__init__.py
+-rw-r--r--   0        0        0     4708 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/config/connect_strategy.py
+-rw-r--r--   0        0        0     5908 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/config/error_strategy.py
+-rw-r--r--   0        0        0     5884 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/config/retry_delay_strategy.py
+-rw-r--r--   0        0        0      800 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/errors.py
+-rw-r--r--   0        0        0     2850 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/http.py
+-rw-r--r--   0        0        0     4557 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/reader.py
+-rw-r--r--   0        0        0    14324 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/sse_client.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/helpers.py
+-rw-r--r--   0        0        0     6098 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/http_util.py
+-rw-r--r--   0        0        0     1206 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_error_strategy.py
+-rw-r--r--   0        0        0     5210 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_http_connect_strategy.py
+-rw-r--r--   0        0        0     3345 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_http_connect_strategy_with_sse_client.py
+-rw-r--r--   0        0        0     4606 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_reader.py
+-rw-r--r--   0        0        0     2876 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_retry_delay_strategy.py
+-rw-r--r--   0        0        0     2834 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_sse_client_basic.py
+-rw-r--r--   0        0        0     3921 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_sse_client_retry.py
+-rw-r--r--   0        0        0       46 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/ld_eventsource/version.py
+-rw-r--r--   0        0        0     1891 2024-04-04 17:25:19.024253 launchdarkly_eventsource-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 launchdarkly_eventsource-1.2.0/PKG-INFO
```

### Comparing `launchdarkly_eventsource-1.1.1/LICENSE` & `launchdarkly_eventsource-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/README.md` & `launchdarkly_eventsource-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 * Setting read timeouts, custom headers, and other HTTP request properties.
 * Specifying that connections should be retried under circumstances where the standard EventSource behavior would not retry them, such as if the server returns an HTTP error status.
 
 This is a synchronous implementation which blocks the caller's thread when reading events or reconnecting. By default, it uses `urllib3` to make HTTP requests, but it can be configured to read any input stream.
 
 ## Supported Python versions
 
-This version of the package is compatible with Python 3.7 and higher.
+This version of the package is compatible with Python 3.8 and higher.
 
 ## Contributing
 
 We encourage pull requests and other contributions from the community. Check out our [contributing guidelines](CONTRIBUTING.md) for instructions on how to contribute to this SDK.
 
 ## About LaunchDarkly
```

### Comparing `launchdarkly_eventsource-1.1.1/ld_eventsource/actions.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/actions.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/ld_eventsource/config/connect_strategy.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/config/connect_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ld_eventsource.http import _HttpClientImpl, _HttpConnectParams
 
 
 class ConnectStrategy:
     """
     An abstraction for how :class:`.SSEClient` should obtain an input stream.
-    
+
     The default implementation is :meth:`http()`, which makes HTTP requests with ``urllib3``.
     Or, if you want to consume an input stream from some other source, you can create your own
     subclass of :class:`ConnectStrategy`.
 
     Instances of this class should be immutable and should not contain any state that is specific
     to one active stream. The :class:`ConnectionClient` that they produce is stateful and belongs
     to a single :class:`.SSEClient`.
@@ -25,15 +25,15 @@
 
         This is called once when an :class:`.SSEClient` is created. The SSEClient returns the
         returned :class:`ConnectionClient` and uses it to perform all subsequent connection attempts.
 
         :param logger: the logger being used by the SSEClient
         """
         raise NotImplementedError("ConnectStrategy base class cannot be used by itself")
-    
+
     @staticmethod
     def http(
         url: str,
         headers: Optional[dict]=None,
         pool: Optional[PoolManager]=None,
         urllib3_request_options: Optional[dict]=None
     ) -> ConnectStrategy:
@@ -58,19 +58,19 @@
     """
 
     def connect(self, last_event_id: Optional[str]) -> ConnectionResult:
         """
         Attempts to connect to a stream. Raises an exception if unsuccessful.
 
         :param last_event_id: the current value of :attr:`SSEClient.last_event_id`
-        (should be sent to the server to support resuming an interrupted stream)
+            (should be sent to the server to support resuming an interrupted stream)
         :return: a :class:`ConnectionResult` representing the stream
         """
         raise NotImplementedError("ConnectionClient base class cannot be used by itself")
-    
+
     def close(self):
         """
         Does whatever is necessary to release resources when the SSEClient is closed.
         """
         pass
 
     def __enter__(self):
@@ -88,15 +88,15 @@
     def __init__(
         self,
         stream: Iterator[bytes],
         closer: Optional[Callable]
     ):
         self.__stream = stream
         self.__closer = closer
-    
+
     @property
     def stream(self) -> Iterator[bytes]:
         """
         An iterator that returns chunks of data.
         """
         return self.__stream
 
@@ -117,15 +117,15 @@
 
 # _HttpConnectStrategy and _HttpConnectionClient are defined here rather than in http.py to avoid
 # a circular module reference.
 
 class _HttpConnectStrategy(ConnectStrategy):
     def __init__(self, params: _HttpConnectParams):
         self.__params = params
-    
+
     def create_client(self, logger: Logger) -> ConnectionClient:
         return _HttpConnectionClient(self.__params, logger)
 
 
 class _HttpConnectionClient(ConnectionClient):
     def __init__(self, params: _HttpConnectParams, logger: Logger):
         self.__impl = _HttpClientImpl(params, logger)
```

### Comparing `launchdarkly_eventsource-1.1.1/ld_eventsource/config/error_strategy.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/config/error_strategy.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/ld_eventsource/config/retry_delay_strategy.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/config/retry_delay_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from random import Random
 import time
 from typing import Callable, Optional, Tuple
 
 
 class RetryDelayStrategy:
     """Base class of strategies for computing how long to wait before retrying a connection.
-    
+
     The default behavior, provided by :meth:`default()`, provides customizable exponential backoff
     and jitter. Applications may also create their own subclasses of RetryDelayStrategy if they
     desire different behavior. It is generally a best practice to use backoff and jitter, to avoid
     a reconnect storm during a service interruption.
 
     Subclasses should be immutable. To implement strategies where the delay uses different parameters
     on each subsequent retry (such as exponential backoff), the strategy should return a new instance
@@ -47,30 +47,30 @@
           current base delay.
         * If ``max_delay`` is set and is greater than zero, the base delay is pinned to be no greater
           than that value.
         * If ``jitter_multiplier`` is set and is greater than zero, the actual delay for each attempt is
           equal to the current base delay minus a pseudo-random number equal to that ratio times itself.
           For instance, a jitter multiplier of 0.25 would mean that a base delay of 1000 is changed to a
           value in the range [750, 1000].
-        
-        
+
+
         :param max_delay: the maximum possible delay value, in seconds; default is 30 seconds
         :param backoff_multiplier: the exponential backoff factor
         :param jitter_multiplier: a fraction from 0.0 to 1.0 for how much of the delay may be
-        pseudo-randomly subtracted
+            pseudo-randomly subtracted
         """
         return _DefaultRetryDelayStrategy(max_delay or 0, backoff_multiplier, jitter_multiplier or 0,
             0, _ReusableRandom(time.time()))
 
     @staticmethod
     def from_lambda(fn: Callable[[float], Tuple[float, Optional[RetryDelayStrategy]]]) -> RetryDelayStrategy:
         """
         Convenience method for creating a RetryDelayStrategy whose ``apply`` method is equivalent to
         the given lambda.
-        
+
         The one difference is that the second return value is an ``Optional[RetryDelayStrategy]`` which
         can be None to mean "no change", since the lambda cannot reference the strategy's ``self``.
         """
         return _LambdaRetryDelayStrategy(fn)
 
 
 class _DefaultRetryDelayStrategy(RetryDelayStrategy):
@@ -97,37 +97,37 @@
 
         random = self.__random
         if self.__jitter_multiplier > 0:
             # To avoid having this object contain mutable state, we create a new Random with the same
             # state as our previous Random before using it.
             random = random.clone()
             adjusted_delay -= (random.random() * self.__jitter_multiplier * adjusted_delay)
-        
+
         next_strategy = _DefaultRetryDelayStrategy(
             self.__max_delay,
             self.__backoff_multiplier,
             self.__jitter_multiplier,
             next_base_delay,
             random
         )
         return (adjusted_delay, next_strategy)
 
 class _LambdaRetryDelayStrategy(RetryDelayStrategy):
     def __init__(self, fn: Callable[[float], Tuple[float, Optional[RetryDelayStrategy]]]):
         self.__fn = fn
-    
+
     def apply(self, base_delay: float) -> Tuple[float, RetryDelayStrategy]:
         delay, maybe_next = self.__fn(base_delay)
         return (delay, maybe_next or self)
 
 class _ReusableRandom:
     def __init__(self, seed: float):
         self.__seed = seed
         self.__random = Random(seed)
-    
+
     def clone(self):
         state = self.__random.getstate()
         ret = _ReusableRandom(self.__seed)
         ret.__random.setstate(state)
         return ret
 
     def random(self) -> float:
```

### Comparing `launchdarkly_eventsource-1.1.1/ld_eventsource/errors.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/errors.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/ld_eventsource/http.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/http.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/ld_eventsource/reader.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/reader.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/ld_eventsource/sse_client.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/sse_client.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/pyproject.toml` & `launchdarkly_eventsource-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 [tool.poetry]
 name = "launchdarkly-eventsource"
-version = "1.1.1"
+version = "1.2.0"
 description = "LaunchDarkly SSE Client"
 authors = ["LaunchDarkly <dev@launchdarkly.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://docs.launchdarkly.com/sdk/server-side/python"
 repository = "https://github.com/launchdarkly/python-eventsource"
 documentation = "https://launchdarkly-python-sdk.readthedocs.io/en/latest/"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
 ]
-packages = [
-    { include = "ld_eventsource" },
-    { include = "testing" },
+packages = [ { include = "ld_eventsource" } ]
+exclude = [
+    { path = "ld_eventsource/testing", format = "wheel" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.8"
 urllib3 = ">=1.26.0,<3"
 
 
 [tool.poetry.group.dev.dependencies]
 mock = ">=2.0.0"
 pytest = ">=2.8"
-pytest-mypy = "0.8.1"
-mypy = ">=1.4.1"
+mypy = "^1.4.0"
 
 
 [tool.poetry.group.contract-tests]
 optional = true
 
 [tool.poetry.group.contract-tests.dependencies]
 Flask = "2.2.5"
@@ -59,15 +57,15 @@
 pyrfc3339 = ">=1.0"
 jsonpickle = ">1.4.1"
 semver = ">=2.7.9"
 urllib3 = ">=1.26.0"
 jinja2 = "3.0.0"
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
 
 
 [tool.pytest.ini_options]
 addopts = ["-ra"]
```

### Comparing `launchdarkly_eventsource-1.1.1/testing/helpers.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from ld_eventsource import *
 from ld_eventsource.config import *
 from ld_eventsource.errors import *
 
-from testing.http_util import *
+from ld_eventsource.testing.http_util import *
 
 from logging import Logger
 from typing import Iterable, Iterator, List, Optional
 
 
 def make_stream() -> ChunkedResponse:
     return ChunkedResponse({ 'Content-Type': 'text/event-stream' })
```

### Comparing `launchdarkly_eventsource-1.1.1/testing/http_util.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/http_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         Thread.__init__(self)
         self.port = port
         self.uri = '%s://localhost:%d' % ('https' if secure else 'http', port)
         self.server = HTTPServer(('localhost', port), MockServerRequestHandler)
         if secure:
             self.server.socket = ssl.wrap_socket(
                 self.server.socket,
-                certfile='./testing/selfsigned.pem', # this is a pre-generated self-signed cert that is valid for 100 years
-                keyfile='./testing/selfsigned.key',
+                certfile='./ld_eventsource/testing/selfsigned.pem', # this is a pre-generated self-signed cert that is valid for 100 years
+                keyfile='./ld_eventsource/testing/selfsigned.key',
                 server_side=True
             )
         self.server.server_wrapper = self
         self.matchers = {}
         self.requests = queue.Queue()
 
     def close(self):
@@ -72,15 +72,15 @@
 
     def require_request(self):
         return self.requests.get(block=False)
 
     def wait_until_request_received(self):
         req = self.requests.get()
         self.requests.put(req)
-        
+
     def should_have_requests(self, count):
         if self.requests.qsize() != count:
             rs = []
             while not self.requests.empty():
                 rs.append(str(self.requests.get(False)))
             assert False, "expected %d more requests but had %s" % (count, rs)
```

### Comparing `launchdarkly_eventsource-1.1.1/testing/test_error_strategy.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_error_strategy.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/testing/test_http_connect_strategy.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_http_connect_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ld_eventsource.config.connect_strategy import *
 
-from testing.helpers import *
-from testing.http_util import *
+from ld_eventsource.testing.helpers import *
+from ld_eventsource.testing.http_util import *
 
 import logging
 from urllib3.exceptions import ProtocolError
 
 # Tests of the basic client/request configuration methods and HTTP functionality in
 # ConnectStrategy.http(), using an embedded HTTP server as a target, but without using
 # SSEClient.
@@ -83,15 +83,15 @@
             server.for_path('/', CauseNetworkError())
             try:
                 with ConnectStrategy.http(server.uri).create_client(logger()) as client:
                     client.connect(None)
                 raise Exception("expected exception, did not get one")
             except ProtocolError as e:
                 pass
-    
+
 def test_auto_redirect_301():
     with start_server() as server:
         with make_stream() as stream:
             server.for_path('/', BasicResponse(301, None, {'Location': server.uri + '/real-stream'}))
             server.for_path('/real-stream', stream)
             with ConnectStrategy.http(server.uri).create_client(logger()) as client:
                 client.connect(None)
```

### Comparing `launchdarkly_eventsource-1.1.1/testing/test_http_connect_strategy_with_sse_client.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_http_connect_strategy_with_sse_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ld_eventsource import *
 from ld_eventsource.config import *
 
-from testing.helpers import *
-from testing.http_util import *
+from ld_eventsource.testing.helpers import *
+from ld_eventsource.testing.http_util import *
 
 # Tests of basic SSEClient behavior using real HTTP requests.
 
 def test_sse_client_reads_events():
     with start_server() as server:
         with make_stream() as stream:
             server.for_path('/', stream)
```

### Comparing `launchdarkly_eventsource-1.1.1/testing/test_reader.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_reader.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/testing/test_retry_delay_strategy.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_retry_delay_strategy.py`

 * *Files identical despite different names*

### Comparing `launchdarkly_eventsource-1.1.1/testing/test_sse_client_basic.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_sse_client_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ld_eventsource import *
 from ld_eventsource.actions import *
 from ld_eventsource.config import *
 
-from testing.helpers import *
+from ld_eventsource.testing.helpers import *
 
 import pytest
 
 # Tests for SSEClient's basic properties and parsing behavior. These tests do not use real HTTP
 # requests; instead, they use a ConnectStrategy that provides a preconfigured input stream. HTTP
 # functionality is tested separately in test_http_connect_strategy.py and
 # test_http_connect_strategy_with_sse_client.py.
```

### Comparing `launchdarkly_eventsource-1.1.1/testing/test_sse_client_retry.py` & `launchdarkly_eventsource-1.2.0/ld_eventsource/testing/test_sse_client_retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ld_eventsource import *
 from ld_eventsource.actions import *
 from ld_eventsource.config import *
 
-from testing.helpers import *
+from ld_eventsource.testing.helpers import *
 
 
 def test_retry_during_initial_connect_succeeds():
     mock = MockConnectStrategy(
         RejectConnection(HTTPStatusError(503)),
         RespondWithData("data: data1\n\n"),
         ExpectNoMoreRequests(),
@@ -84,15 +84,15 @@
         item3 = next(all)
         assert isinstance(item3, Fault)
         assert item3.error is None
         assert client.next_retry_delay == initial_delay
 
         item4 = next(all)
         assert isinstance(item4, Start)
-        
+
         item5 = next(all)
         assert isinstance(item5, Event)
         assert item5.data == 'data2'
 
         item6 = next(all)
         assert isinstance(item6, Fault)
         assert item6.error is None
@@ -121,14 +121,14 @@
         assert item2.data == 'data1'
 
         client.interrupt()
         assert client.next_retry_delay == initial_delay
 
         item3 = next(all)
         assert isinstance(item3, Fault)
-        
+
         item4 = next(all)
         assert isinstance(item4, Start)
-        
+
         item5 = next(all)
         assert isinstance(item5, Event)
         assert item5.data == 'data3'
```

### Comparing `launchdarkly_eventsource-1.1.1/PKG-INFO` & `launchdarkly_eventsource-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: launchdarkly-eventsource
-Version: 1.1.1
+Version: 1.2.0
 Summary: LaunchDarkly SSE Client
 Home-page: https://docs.launchdarkly.com/sdk/server-side/python
 License: Apache-2.0
 Author: LaunchDarkly
 Author-email: dev@launchdarkly.com
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
@@ -40,15 +39,15 @@
 * Setting read timeouts, custom headers, and other HTTP request properties.
 * Specifying that connections should be retried under circumstances where the standard EventSource behavior would not retry them, such as if the server returns an HTTP error status.
 
 This is a synchronous implementation which blocks the caller's thread when reading events or reconnecting. By default, it uses `urllib3` to make HTTP requests, but it can be configured to read any input stream.
 
 ## Supported Python versions
 
-This version of the package is compatible with Python 3.7 and higher.
+This version of the package is compatible with Python 3.8 and higher.
 
 ## Contributing
 
 We encourage pull requests and other contributions from the community. Check out our [contributing guidelines](CONTRIBUTING.md) for instructions on how to contribute to this SDK.
 
 ## About LaunchDarkly
```

