# Comparing `tmp/pytracekit-0.1.0.tar.gz` & `tmp/pytracekit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytracekit-0.1.0.tar", last modified: Tue Apr  2 17:02:06 2024, max compression
+gzip compressed data, was "pytracekit-0.1.1.tar", last modified: Thu Apr  4 09:46:05 2024, max compression
```

## Comparing `pytracekit-0.1.0.tar` & `pytracekit-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     3352 2024-04-02 16:47:31.938032 pytracekit-0.1.0/README.md
--rw-r--r--   0        0        0      942 2024-04-02 17:02:06.852159 pytracekit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      312 2024-04-01 05:25:45.255239 pytracekit-0.1.0/pytracekit/__init__.py
--rw-r--r--   0        0        0      459 2024-04-01 06:00:40.180442 pytracekit-0.1.0/pytracekit/config/TraceConfig.py
--rw-r--r--   0        0        0      167 2024-04-01 04:53:41.940492 pytracekit-0.1.0/pytracekit/constants/common.py
--rw-r--r--   0        0        0       84 2024-04-02 16:39:27.447306 pytracekit-0.1.0/pytracekit/decorators/__init__.py
--rw-r--r--   0        0        0     1992 2024-04-02 16:39:21.618740 pytracekit-0.1.0/pytracekit/decorators/tracing.py
--rw-r--r--   0        0        0      200 2024-04-01 05:05:02.864835 pytracekit-0.1.0/pytracekit/instrumentors/__init__.py
--rw-r--r--   0        0        0      296 2024-04-01 05:18:24.903039 pytracekit-0.1.0/pytracekit/instrumentors/base.py
--rw-r--r--   0        0        0      276 2024-04-01 05:21:10.791657 pytracekit-0.1.0/pytracekit/instrumentors/falcon.py
--rw-r--r--   0        0        0      286 2024-04-01 05:21:03.096263 pytracekit-0.1.0/pytracekit/instrumentors/fastapi.py
--rw-r--r--   0        0        0      299 2024-04-01 05:20:49.529353 pytracekit-0.1.0/pytracekit/instrumentors/flask.py
--rw-r--r--   0        0        0      612 2024-04-01 06:00:40.184442 pytracekit-0.1.0/pytracekit/instrumentors/utils.py
--rw-r--r--   0        0        0     1830 2024-04-02 04:31:34.147620 pytracekit-0.1.0/pytracekit/main.py
--rw-r--r--   0        0        0        0 2024-04-01 05:06:09.738056 pytracekit-0.1.0/pytracekit/utils/__init__.py
--rw-r--r--   0        0        0      711 2024-04-01 06:00:40.180442 pytracekit-0.1.0/pytracekit/utils/detect_framework.py
--rw-r--r--   0        0        0     1554 2024-04-02 04:43:38.509669 pytracekit-0.1.0/pytracekit/utils/trace_logger.py
--rw-r--r--   0        0        0        0 2024-03-27 17:32:03.457619 pytracekit-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 pytracekit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3368 2024-04-02 17:05:31.309426 pytracekit-0.1.1/README.md
+-rw-r--r--   0        0        0      886 2024-04-04 09:46:05.761747 pytracekit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      312 2024-04-01 05:25:45.255239 pytracekit-0.1.1/pytracekit/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-04 05:48:58.843716 pytracekit-0.1.1/pytracekit/config/TraceConfig.py
+-rw-r--r--   0        0        0      167 2024-04-01 04:53:41.940492 pytracekit-0.1.1/pytracekit/constants/common.py
+-rw-r--r--   0        0        0       84 2024-04-02 16:39:27.447306 pytracekit-0.1.1/pytracekit/decorators/__init__.py
+-rw-r--r--   0        0        0     1992 2024-04-02 16:39:21.618740 pytracekit-0.1.1/pytracekit/decorators/tracing.py
+-rw-r--r--   0        0        0      200 2024-04-01 05:05:02.864835 pytracekit-0.1.1/pytracekit/instrumentors/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-01 05:18:24.903039 pytracekit-0.1.1/pytracekit/instrumentors/base.py
+-rw-r--r--   0        0        0      276 2024-04-01 05:21:10.791657 pytracekit-0.1.1/pytracekit/instrumentors/falcon.py
+-rw-r--r--   0        0        0      286 2024-04-01 05:21:03.096263 pytracekit-0.1.1/pytracekit/instrumentors/fastapi.py
+-rw-r--r--   0        0        0      299 2024-04-01 05:20:49.529353 pytracekit-0.1.1/pytracekit/instrumentors/flask.py
+-rw-r--r--   0        0        0      612 2024-04-01 06:00:40.184442 pytracekit-0.1.1/pytracekit/instrumentors/utils.py
+-rw-r--r--   0        0        0     1829 2024-04-04 09:45:54.793686 pytracekit-0.1.1/pytracekit/main.py
+-rw-r--r--   0        0        0        0 2024-04-01 05:06:09.738056 pytracekit-0.1.1/pytracekit/utils/__init__.py
+-rw-r--r--   0        0        0      711 2024-04-01 06:00:40.180442 pytracekit-0.1.1/pytracekit/utils/detect_framework.py
+-rw-r--r--   0        0        0     1554 2024-04-02 04:43:38.509669 pytracekit-0.1.1/pytracekit/utils/trace_logger.py
+-rw-r--r--   0        0        0        0 2024-03-27 17:32:03.457619 pytracekit-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3679 2024-04-04 08:46:57.401523 pytracekit-0.1.1/tests/test_instrument.py
+-rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 pytracekit-0.1.1/PKG-INFO
```

### Comparing `pytracekit-0.1.0/README.md` & `pytracekit-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyTraceKit
 
  **PyTraceKit**, is a low code solution designed to simplify the integration of distributed tracing into Python microservices through the power of OpenTelemetry. This package provides straightforward approach to enrich your logging with trace IDs and allowing detailed tracing with minimal setup.
 
- The package comes with inbuilt support for Falcon, FastAPI , Flask 
+ The package comes with inbuilt support for Falcon, FastAPI , Flask ,redis , MongoDB
 
 ## Key Features
 
 - **Simplified Tracing**: Easily integrate distributed tracing into FastAPI, Flask, or Falcon applications with just one line of code.
 - **Function-Level Tracing with Customization**: Add detailed tracing to any function, specifying custom operation names and span attributes for in-depth observability.
 - **Advanced Logging**: Each log message includes a trace ID for easy correlation, with customizable logging settings such as file paths, sizes, and rotation.
 - **Framework Agnostic**: Automatically detects and integrates with your Python web framework, offering out-of-the-box support for FastAPI, Flask, and Falcon.
```

### Comparing `pytracekit-0.1.0/pyproject.toml` & `pytracekit-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytracekit"
-version = "0.1.0"
+version = "0.1.1"
 description = "Distributed tracing made easy for python"
 authors = [
     { name = "Himanshu Barak", email = "himanshu.barak12@gmail.com" },
 ]
 dependencies = [
     "opentelemetry-api>=1.23.0",
     "opentelemetry-sdk>=1.23.0",
@@ -13,16 +13,15 @@
     "opentelemetry-instrumentation-redis>=0.44b0",
     "opentelemetry-exporter-otlp>=1.23.0",
     "opentelemetry-instrumentation-requests>=0.44b0",
     "redis>=5.0.3",
     "pymongo>=4.6.3",
     "opentelemetry-instrumentation-flask>=0.44b0",
     "opentelemetry-instrumentation-falcon>=0.44b0",
-    "opentelemetry-instrumentation-psycopg2>=0.44b0",
-    "psycopg2>=2.9.9",
+    "pytest>=8.1.1",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `pytracekit-0.1.0/pytracekit/decorators/tracing.py` & `pytracekit-0.1.1/pytracekit/decorators/tracing.py`

 * *Files identical despite different names*

### Comparing `pytracekit-0.1.0/pytracekit/instrumentors/utils.py` & `pytracekit-0.1.1/pytracekit/instrumentors/utils.py`

 * *Files identical despite different names*

### Comparing `pytracekit-0.1.0/pytracekit/main.py` & `pytracekit-0.1.1/pytracekit/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
        app : the instance of the fastapi, flask ,falcon application
        framework: the name of the framework which needs to be instrumented 
     """
     config = TraceConfig()
     if not config.enable_tracing:
         print("Tracing is disabled.")
         return
-
     if not config.tracing_endpoint:
         raise Exception("Tracing endpoint not provided.")
 
     if not config.trace_service_name:
         raise Exception("Trace service name not provided.")
```

### Comparing `pytracekit-0.1.0/pytracekit/utils/detect_framework.py` & `pytracekit-0.1.1/pytracekit/utils/detect_framework.py`

 * *Files identical despite different names*

### Comparing `pytracekit-0.1.0/pytracekit/utils/trace_logger.py` & `pytracekit-0.1.1/pytracekit/utils/trace_logger.py`

 * *Files identical despite different names*

### Comparing `pytracekit-0.1.0/PKG-INFO` & `pytracekit-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytracekit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Distributed tracing made easy for python
 Author-Email: Himanshu Barak <himanshu.barak12@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: opentelemetry-api>=1.23.0
 Requires-Dist: opentelemetry-sdk>=1.23.0
 Requires-Dist: opentelemetry-instrumentation-fastapi>=0.44b0
@@ -12,23 +12,22 @@
 Requires-Dist: opentelemetry-instrumentation-redis>=0.44b0
 Requires-Dist: opentelemetry-exporter-otlp>=1.23.0
 Requires-Dist: opentelemetry-instrumentation-requests>=0.44b0
 Requires-Dist: redis>=5.0.3
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: opentelemetry-instrumentation-flask>=0.44b0
 Requires-Dist: opentelemetry-instrumentation-falcon>=0.44b0
-Requires-Dist: opentelemetry-instrumentation-psycopg2>=0.44b0
-Requires-Dist: psycopg2>=2.9.9
+Requires-Dist: pytest>=8.1.1
 Description-Content-Type: text/markdown
 
 # PyTraceKit
 
  **PyTraceKit**, is a low code solution designed to simplify the integration of distributed tracing into Python microservices through the power of OpenTelemetry. This package provides straightforward approach to enrich your logging with trace IDs and allowing detailed tracing with minimal setup.
 
- The package comes with inbuilt support for Falcon, FastAPI , Flask 
+ The package comes with inbuilt support for Falcon, FastAPI , Flask ,redis , MongoDB
 
 ## Key Features
 
 - **Simplified Tracing**: Easily integrate distributed tracing into FastAPI, Flask, or Falcon applications with just one line of code.
 - **Function-Level Tracing with Customization**: Add detailed tracing to any function, specifying custom operation names and span attributes for in-depth observability.
 - **Advanced Logging**: Each log message includes a trace ID for easy correlation, with customizable logging settings such as file paths, sizes, and rotation.
 - **Framework Agnostic**: Automatically detects and integrates with your Python web framework, offering out-of-the-box support for FastAPI, Flask, and Falcon.
```

