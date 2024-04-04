# Comparing `tmp/oteltest-0.0.1.tar.gz` & `tmp/oteltest-0.0.2.tar.gz`

## Comparing `oteltest-0.0.1.tar` & `oteltest-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.0.1/example_scripts/simple_loop.json
--rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 oteltest-0.0.1/example_scripts/simple_loop.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.0.1/src/oteltest/__about__.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.1/src/oteltest/__init__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 oteltest-0.0.1/src/oteltest/common.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 oteltest-0.0.1/src/oteltest/main.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 oteltest-0.0.1/src/oteltest/sink.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.0.1/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 oteltest-0.0.1/README.md
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 oteltest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 oteltest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.0.2/example_scripts/simple_loop.json
+-rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 oteltest-0.0.2/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/common.py
+-rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/main.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/sink.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.0.2/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.0.2/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.0.2/PKG-INFO
```

### Comparing `oteltest-0.0.1/example_scripts/simple_loop.json` & `oteltest-0.0.2/example_scripts/simple_loop.json`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.1/example_scripts/simple_loop.py` & `oteltest-0.0.2/example_scripts/simple_loop.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.1/src/oteltest/__about__.py` & `oteltest-0.0.2/src/oteltest/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

### Comparing `oteltest-0.0.1/src/oteltest/__init__.py` & `oteltest-0.0.2/src/oteltest/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.1/src/oteltest/common.py` & `oteltest-0.0.2/src/oteltest/common.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.1/src/oteltest/main.py` & `oteltest-0.0.2/src/oteltest/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,33 +21,47 @@
 import sys
 import tempfile
 import venv
 from pathlib import Path
 
 from google.protobuf.json_format import MessageToDict
 
-from opentelemetry.proto.collector.logs.v1.logs_service_pb2 import ExportLogsServiceRequest
-from opentelemetry.proto.collector.metrics.v1.metrics_service_pb2 import ExportMetricsServiceRequest
-from opentelemetry.proto.collector.trace.v1.trace_service_pb2 import ExportTraceServiceRequest
+from opentelemetry.proto.collector.logs.v1.logs_service_pb2 import (
+    ExportLogsServiceRequest,
+)
+from opentelemetry.proto.collector.metrics.v1.metrics_service_pb2 import (
+    ExportMetricsServiceRequest,
+)
+from opentelemetry.proto.collector.trace.v1.trace_service_pb2 import (
+    ExportTraceServiceRequest,
+)
 from oteltest.common import OtelTest, Telemetry
 from oteltest.sink import GrpcSink, RequestHandler
 
 import argparse
 
 
 def main():
     parser = argparse.ArgumentParser(description="OpenTelemetry Python Tester")
 
     w_help = "Path to a wheel (.whl) file to be used instead of `pip install oteltest`"
-    parser.add_argument("-w", "--wheel-file", type=str, required=False, help=w_help)
+    parser.add_argument(
+        "-w", "--wheel-file", type=str, required=False, help=w_help
+    )
 
     d_help = "A directory to hold per-script venv directories"
-    parser.add_argument("-d", "--venv-parent-dir", type=str, required=False, help=d_help)
+    parser.add_argument(
+        "-d", "--venv-parent-dir", type=str, required=False, help=d_help
+    )
 
-    parser.add_argument("script_dir", type=str, help="The directory containing your oteltest scripts")
+    parser.add_argument(
+        "script_dir",
+        type=str,
+        help="The directory containing your oteltest scripts",
+    )
 
     args = parser.parse_args()
     run(args.script_dir, args.wheel_file, args.venv_parent_dir)
 
 
 def run(script_dir: str, wheel_file: str, venv_parent_dir: str):
     venv_dir = venv_parent_dir or tempfile.mkdtemp()
@@ -96,15 +110,18 @@
         file.write(handler.telemetry_to_json())
 
     test_instance.validate(handler.telemetry)
     print(f"- {script} PASSED")
 
 
 def run_python_script(script, script_dir, test_instance, v):
-    python_script_cmd = [v.path_to_executable("python"), str(Path(script_dir) / script)]
+    python_script_cmd = [
+        v.path_to_executable("python"),
+        str(Path(script_dir) / script),
+    ]
     ws = test_instance.wrapper_script()
     if ws is not None:
         python_script_cmd.insert(0, v.path_to_executable(ws))
     run_subprocess(python_script_cmd, test_instance.environment_variables())
 
 
 def run_subprocess(args, env_vars=None):
@@ -114,32 +131,36 @@
         args,
         capture_output=True,
         env=env_vars,
     )
     print(f"- Return Code: {result.returncode}")
     print("- Standard Output:")
     if result.stdout:
-        print(result.stdout.decode('utf-8').strip())
+        print(result.stdout.decode("utf-8").strip())
     print("- Standard Error:")
     if result.stderr:
-        print(result.stderr.decode('utf-8').strip())
+        print(result.stderr.decode("utf-8").strip())
     print("- End Subprocess -\n")
 
 
 def load_test_class_for_script(module_name):
     module = importlib.import_module(module_name)
     for attr_name in dir(module):
         value = getattr(module, attr_name)
         if is_test_class(value):
             return value
     return None
 
 
 def is_test_class(value):
-    return inspect.isclass(value) and issubclass(value, OtelTest) and value is not OtelTest
+    return (
+        inspect.isclass(value)
+        and issubclass(value, OtelTest)
+        and value is not OtelTest
+    )
 
 
 class Venv:
     def __init__(self, venv_dir):
         self.venv_dir = venv_dir
 
     def create(self):
@@ -152,22 +173,34 @@
         shutil.rmtree(self.venv_dir)
 
 
 class AccumulatingHandler(RequestHandler):
     def __init__(self):
         self.telemetry = Telemetry()
 
-    def handle_logs(self, request: ExportLogsServiceRequest, context):  # noqa: ARG002
-        self.telemetry.add_log(MessageToDict(request), get_context_headers(context))
-
-    def handle_metrics(self, request: ExportMetricsServiceRequest, context):  # noqa: ARG002
-        self.telemetry.add_metric(MessageToDict(request), get_context_headers(context))
-
-    def handle_trace(self, request: ExportTraceServiceRequest, context):  # noqa: ARG002
-        self.telemetry.add_trace(MessageToDict(request), get_context_headers(context))
+    def handle_logs(
+        self, request: ExportLogsServiceRequest, context
+    ):  # noqa: ARG002
+        self.telemetry.add_log(
+            MessageToDict(request), get_context_headers(context)
+        )
+
+    def handle_metrics(
+        self, request: ExportMetricsServiceRequest, context
+    ):  # noqa: ARG002
+        self.telemetry.add_metric(
+            MessageToDict(request), get_context_headers(context)
+        )
+
+    def handle_trace(
+        self, request: ExportTraceServiceRequest, context
+    ):  # noqa: ARG002
+        self.telemetry.add_trace(
+            MessageToDict(request), get_context_headers(context)
+        )
 
     def telemetry_to_json(self):
         return self.telemetry.to_json()
 
 
 def get_context_headers(context):
     return pbmetadata_to_dict(context.invocation_metadata())
@@ -176,9 +209,9 @@
 def pbmetadata_to_dict(pbmetadata):
     out = {}
     for k, v in pbmetadata:
         out[k] = v
     return out
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `oteltest-0.0.1/src/oteltest/sink.py` & `oteltest-0.0.2/src/oteltest/sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     def Export(self, request, context):  # noqa: N802
         self.handle_request(request, context)
         return metrics_service_pb2.ExportMetricsServiceResponse()
 
 
 class RequestHandler(abc.ABC):
     """
-    This interface is meant to be implemented by users of the otelsink API. If you use the API, you'll want to create
-    an implementation, instantiate it, and pass the instance to the GrpcSink constructor. As messages arrive, the
-    callbacks defined by this interface will be invoked.
+    The RequestHandler interface is meant to be implemented by users of the otelsink API. If you use the API,
+    you'll want to create a RequestHandler implementation, instantiate it, and pass the instance to the GrpcSink
+    constructor. As messages arrive, the callbacks defined by this interface will be invoked.
 
     grpc_sink = GrpcSink(MyRequestHandler())
     """
 
     @abc.abstractmethod
     def handle_logs(self, request: ExportLogsServiceRequest, context):
         pass
@@ -104,15 +104,17 @@
 
     def handle_logs(self, request, context):  # noqa: ARG002
         print(f"log request: {request}")  # noqa: T201
 
     def handle_metrics(self, request, context):  # noqa: ARG002
         print(f"metrics request: {request}")  # noqa: T201
 
-    def handle_trace(self, request: ExportTraceServiceRequest, context):  # noqa: ARG002
+    def handle_trace(
+        self, request: ExportTraceServiceRequest, context
+    ):  # noqa: ARG002
         print(f"trace request: {request}")  # noqa: T201
 
 
 def run_with_print_handler():
     """
     Runs otelsink with a PrintHandler.
     """
```

### Comparing `oteltest-0.0.1/tests/__init__.py` & `oteltest-0.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.1/.gitignore` & `oteltest-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.1/LICENSE.txt` & `oteltest-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.1/README.md` & `oteltest-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -82,26 +82,26 @@
 
     def validate(self, telemetry: Telemetry):
         assert telemetry.num_spans() == NUM_ADDS
 ```
 
 #### Usage with OTel Examples
 
-Runnable examples are a great way for new users to get up to speed, but it would be nice to give them an opportunity
-to see the telemetry they just generated. Adding an `OtelTest` implementation (e.g. `MyTest` above) to existing
-example scripts lets users run examples without having to set up Python environments with dependencies. It also lets
-them potentially see the output of their instrumented script.
+Runnable examples are a great way to get up to speed on OpenTelemetry but running them can be tedious.
+oteltest lets you run example scripts and potentially see the telemetry you just generated without starting Docker or
+setting up Python enviornments. Adding an `OtelTest` implementation (e.g. `MyTest` above) to an existing example script
+lets you run it without having to set up a Python environment with dependencies.
 
 ### otelsink
 
 `otelsink` is a gRPC server that listens for OTel metrics, traces, and logs.
 
 #### Operation
 
-You can run it either from the command line by using the `otelsink` command (installed when you
+You can run otelink either from the command line by using the `otelsink` command (installed when you
 `pip install oteltest`), or programatically.
 
 Either way, `otelsink` runs a gRPC server listening on 0.0.0.0:4317.
 
 #### Command Line
 
 ```
```

### Comparing `oteltest-0.0.1/PKG-INFO` & `oteltest-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.0.1
+Version: 0.0.2
+Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Requires-Dist: grpcio
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-proto
 Requires-Dist: protobuf
 Description-Content-Type: text/markdown
 
 # oteltest
@@ -107,26 +109,26 @@
 
     def validate(self, telemetry: Telemetry):
         assert telemetry.num_spans() == NUM_ADDS
 ```
 
 #### Usage with OTel Examples
 
-Runnable examples are a great way for new users to get up to speed, but it would be nice to give them an opportunity
-to see the telemetry they just generated. Adding an `OtelTest` implementation (e.g. `MyTest` above) to existing
-example scripts lets users run examples without having to set up Python environments with dependencies. It also lets
-them potentially see the output of their instrumented script.
+Runnable examples are a great way to get up to speed on OpenTelemetry but running them can be tedious.
+oteltest lets you run example scripts and potentially see the telemetry you just generated without starting Docker or
+setting up Python enviornments. Adding an `OtelTest` implementation (e.g. `MyTest` above) to an existing example script
+lets you run it without having to set up a Python environment with dependencies.
 
 ### otelsink
 
 `otelsink` is a gRPC server that listens for OTel metrics, traces, and logs.
 
 #### Operation
 
-You can run it either from the command line by using the `otelsink` command (installed when you
+You can run otelink either from the command line by using the `otelsink` command (installed when you
 `pip install oteltest`), or programatically.
 
 Either way, `otelsink` runs a gRPC server listening on 0.0.0.0:4317.
 
 #### Command Line
 
 ```
```

