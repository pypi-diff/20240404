# Comparing `tmp/pytest-sentry-0.1.9.tar.gz` & `tmp/pytest_sentry-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sentry-0.1.9.tar", last modified: Wed Apr 21 14:30:09 2021, max compression
+gzip compressed data, was "pytest_sentry-0.2.0.tar", last modified: Thu Apr  4 14:30:11 2024, max compression
```

## Comparing `pytest-sentry-0.1.9.tar` & `pytest_sentry-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 untitaker   (501) staff       (20)        0 2021-04-21 14:30:09.073586 pytest-sentry-0.1.9/
--rw-r--r--   0 untitaker   (501) staff       (20)     1324 2018-12-29 16:33:31.000000 pytest-sentry-0.1.9/LICENSE
--rw-r--r--   0 untitaker   (501) staff       (20)     7149 2021-04-21 14:30:09.073138 pytest-sentry-0.1.9/PKG-INFO
--rw-r--r--   0 untitaker   (501) staff       (20)     5659 2021-04-21 14:28:39.000000 pytest-sentry-0.1.9/README.rst
-drwxr-xr-x   0 untitaker   (501) staff       (20)        0 2021-04-21 14:30:09.072486 pytest-sentry-0.1.9/pytest_sentry.egg-info/
--rw-r--r--   0 untitaker   (501) staff       (20)     7149 2021-04-21 14:30:08.000000 pytest-sentry-0.1.9/pytest_sentry.egg-info/PKG-INFO
--rw-r--r--   0 untitaker   (501) staff       (20)      268 2021-04-21 14:30:08.000000 pytest-sentry-0.1.9/pytest_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 untitaker   (501) staff       (20)        1 2021-04-21 14:30:08.000000 pytest-sentry-0.1.9/pytest_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 untitaker   (501) staff       (20)       35 2021-04-21 14:30:08.000000 pytest-sentry-0.1.9/pytest_sentry.egg-info/entry_points.txt
--rw-r--r--   0 untitaker   (501) staff       (20)       24 2021-04-21 14:30:08.000000 pytest-sentry-0.1.9/pytest_sentry.egg-info/requires.txt
--rw-r--r--   0 untitaker   (501) staff       (20)       14 2021-04-21 14:30:08.000000 pytest-sentry-0.1.9/pytest_sentry.egg-info/top_level.txt
--rw-r--r--   0 untitaker   (501) staff       (20)     9554 2021-04-21 14:28:26.000000 pytest-sentry-0.1.9/pytest_sentry.py
--rw-r--r--   0 untitaker   (501) staff       (20)       38 2021-04-21 14:30:09.073709 pytest-sentry-0.1.9/setup.cfg
--rw-r--r--   0 untitaker   (501) staff       (20)      512 2021-04-21 14:29:33.000000 pytest-sentry-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:30:11.672431 pytest_sentry-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-04 14:30:11.672431 pytest_sentry-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:30:11.668431 pytest_sentry-0.2.0/pytest_sentry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/pytest_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 14:30:11.672431 pytest_sentry-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:30:11.668431 pytest_sentry-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_tracing.py
```

### Comparing `pytest-sentry-0.1.9/LICENSE` & `pytest_sentry-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sentry-0.1.9/PKG-INFO` & `pytest_sentry-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,160 +1,169 @@
-Metadata-Version: 1.0
-Name: pytest-sentry
-Version: 0.1.9
+Metadata-Version: 2.1
+Name: pytest_sentry
+Version: 0.2.0
 Summary: A pytest plugin to send testrun information to Sentry.io
 Home-page: https://github.com/untitaker/pytest-sentry
 Author: Markus Unterwaditzer
 Author-email: markus@unterwaditzer.net
-License: BSD
-Description: =============
-        pytest-sentry
-        =============
-        
-        .. image:: https://img.shields.io/pypi/v/pytest-sentry
-            :target: https://pypi.org/project/pytest-sentry/
-        
-        .. image:: https://img.shields.io/pypi/l/pytest-sentry
-            :target: https://pypi.org/project/pytest-sentry/
-        
-        ``pytest-sentry`` is a `pytest <https://pytest.org>`_ plugin that uses `Sentry
-        <https://sentry.io/>`_ to store and aggregate information about your testruns.
-        
-        **This is not an official Sentry product.**
-        
-        Tracking flaky tests as errors
-        ==============================
-        
-        Let's say you have a testsuite with some flaky tests that randomly break your
-        CI build due to network issues, race conditions or other stuff that you don't
-        want to fix immediately. The known workaround is to retry those tests
-        automatically, for example using `pytest-rerunfailures
-        <https://github.com/pytest-dev/pytest-rerunfailures>`_.
-        
-        One concern against plugins like this is that they just hide the bugs in your
-        testsuite or even other code. After all your CI build is green and your code
-        probably works most of the time.
-        
-        ``pytest-sentry`` tries to make that choice a bit easier by tracking flaky test
-        failures in a place separate from your build status. Sentry is already a
-        good choice for keeping tabs on all kinds of errors, important or not, in
-        production, so let's try to use it in testsuites too.
-        
-        The prerequisite is that you already make use of ``pytest`` and
-        ``pytest-rerunfailures`` in CI. Now install ``pytest-sentry`` and set the
-        ``PYTEST_SENTRY_DSN`` environment variable to the DSN of a new Sentry project.
-        
-        Now every test failure that is "fixed" by retrying the test is reported to
-        Sentry, but still does not break CI. Tests that consistently fail will not be
-        reported.
-        
-        Tracking the performance of your testsuite
-        ==========================================
-        
-        By default ``pytest-sentry`` will send `Performance
-        <https://sentry.io/for/performance/>`_ data to Sentry:
-        
-        * Fixture setup is reported as "transaction" to Sentry, such that you can
-          answer questions like "what is my slowest test fixture" and "what is my most
-          used test fixture".
-        
-        * Calls to the test function itself are reported as separate transaction such
-          that you can find large, slow tests as well.
-        
-        * Fixture setup related to a particular test item will be in the same trace,
-          i.e. will have same trace ID. There is no common parent transaction though.
-          It is purposefully dropped to spare quota as it does not contain interesting
-          information::
-        
-              pytest.runtest.protocol  [one time, not sent]
-                pytest.fixture.setup [multiple times, sent]
-                pytest.runtest.call [one time, sent]
-        
-          The trace is per-test-item. For correlating transactions across an entire
-          test run, use the automatically attached CI tags or attach some tag on your
-          own.
-        
-        To measure performance data, install ``pytest-sentry`` and set
-        ``PYTEST_SENTRY_DSN``, like with errors.
-        
-        Transactions can have noticeable runtime overhead over just reporting errors.
-        To disable, use a marker::
-        
-            import pytest
-            import pytest_sentry
-        
-            pytestmarker = pytest.mark.sentry_client({"traces_sample_rate": 0.0})
-        
-        Advanced Options
-        ================
-        
-        ``pytest-sentry`` supports marking your tests to use a different DSN, client or
-        hub per-test. You can use this to provide custom options to the ``Client``
-        object from the `Sentry SDK for Python
-        <https://github.com/getsentry/sentry-python>`_::
-        
-            import random
-            import pytest
-        
-            from sentry_sdk import Hub
-            from pytest_sentry import Client
-        
-            @pytest.mark.sentry_client(None)
-            def test_no_sentry():
-                # Even though flaky, this test never gets reported to sentry
-                assert random.random() > 0.5
-        
-            @pytest.mark.sentry_client("MY NEW DSN")
-            def test_custom_dsn():
-                # Use a different DSN to report errors for this one
-                assert random.random() > 0.5
-        
-            # Other invocations:
-        
-            @pytest.mark.sentry_client(Client("CUSTOM DSN"))
-            @pytest.mark.sentry_client(lambda: Client("CUSTOM DSN"))
-            @pytest.mark.sentry_client(Hub(Client("CUSTOM DSN")))
-            @pytest.mark.sentry_client({"dsn": ..., "debug": True})
-        
-        
-        The ``Client`` class exposed by ``pytest-sentry`` only has different default
-        integrations. It disables some of the error-capturing integrations to avoid
-        sending random expected errors into your project.
-        
-        Accessing the used Sentry client
-        ================================
-        
-        You will notice that the global functions such as
-        ``sentry_sdk.capture_message`` will not actually send events into the same DSN
-        you configured this plugin with. That's because ``pytest-sentry`` goes to
-        extreme lenghts to keep its own SDK setup separate from the SDK setup of the
-        tested code.
-        
-        ``pytest-sentry`` exposes the ``sentry_test_hub`` fixture whose return value is
-        the ``Hub`` being used to send events to Sentry. Use ``with sentry_test_hub:``
-        to temporarily switch context. You can use this to set custom tags like so::
-        
-            def test_foo(sentry_test_hub):
-                with sentry_test_hub:
-                    sentry_sdk.set_tag("pull_request", os.environ['EXAMPLE_CI_PULL_REQUEST'])
-        
-        
-        Why all the hassle with the context manager? Just imagine if your tested
-        application would start to log some (expected) errors on its own. You would
-        immediately exceed your quota!
-        
-        Always reporting test failures
-        ==============================
-        
-        You can always report all test failures to Sentry by setting the environment
-        variable ``PYTEST_SENTRY_ALWAYS_REPORT=1``.
-        
-        This can be enabled for builds on the ``master`` or release branch, to catch
-        certain kinds of tests that are flaky across builds, but consistently fail or
-        pass within one testrun.
-        
-        License
-        =======
-        
-        Licensed under 2-clause BSD, see ``LICENSE``.
-        
-Platform: UNKNOWN
+License: BSD-2-Clause
+Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: pytest
+Requires-Dist: sentry-sdk==2.0.0rc4
+Requires-Dist: wrapt
+
+=============
+pytest-sentry
+=============
+
+.. image:: https://img.shields.io/pypi/v/pytest-sentry
+    :target: https://pypi.org/project/pytest-sentry/
+
+.. image:: https://img.shields.io/pypi/l/pytest-sentry
+    :target: https://pypi.org/project/pytest-sentry/
+
+``pytest-sentry`` is a `pytest <https://pytest.org>`_ plugin that uses `Sentry
+<https://sentry.io/>`_ to store and aggregate information about your testruns.
+
+**This is not an official Sentry product.**
+
+Tracking flaky tests as errors
+==============================
+
+Let's say you have a testsuite with some flaky tests that randomly break your
+CI build due to network issues, race conditions or other stuff that you don't
+want to fix immediately. The known workaround is to retry those tests
+automatically, for example using `pytest-rerunfailures
+<https://github.com/pytest-dev/pytest-rerunfailures>`_.
+
+One concern against plugins like this is that they just hide the bugs in your
+testsuite or even other code. After all your CI build is green and your code
+probably works most of the time.
+
+``pytest-sentry`` tries to make that choice a bit easier by tracking flaky test
+failures in a place separate from your build status. Sentry is already a
+good choice for keeping tabs on all kinds of errors, important or not, in
+production, so let's try to use it in testsuites too.
+
+The prerequisite is that you already make use of ``pytest`` and
+``pytest-rerunfailures`` in CI. Now install ``pytest-sentry`` and set the
+``PYTEST_SENTRY_DSN`` environment variable to the DSN of a new Sentry project.
+
+Now every test failure that is "fixed" by retrying the test is reported to
+Sentry, but still does not break CI. Tests that consistently fail will not be
+reported.
+
+Tracking the performance of your testsuite
+==========================================
+
+By default ``pytest-sentry`` will send `Performance
+<https://sentry.io/for/performance/>`_ data to Sentry:
+
+* Fixture setup is reported as "transaction" to Sentry, such that you can
+  answer questions like "what is my slowest test fixture" and "what is my most
+  used test fixture".
+
+* Calls to the test function itself are reported as separate transaction such
+  that you can find large, slow tests as well.
+
+* Fixture setup related to a particular test item will be in the same trace,
+  i.e. will have same trace ID. There is no common parent transaction though.
+  It is purposefully dropped to spare quota as it does not contain interesting
+  information::
+
+      pytest.runtest.protocol  [one time, not sent]
+        pytest.fixture.setup [multiple times, sent]
+        pytest.runtest.call [one time, sent]
+
+  The trace is per-test-item. For correlating transactions across an entire
+  test run, use the automatically attached CI tags or attach some tag on your
+  own.
+
+To measure performance data, install ``pytest-sentry`` and set
+``PYTEST_SENTRY_DSN``, like with errors. By default, the extension will send all
+performance data to Sentry. If you want to limit the amount of data sent, you
+can set the ``PYTEST_SENTRY_TRACES_SAMPLE_RATE`` environment variable to a float
+between ``0`` and ``1``. This will cause only a random sample of transactions to
+be sent to Sentry.
+
+Transactions can have noticeable runtime overhead over just reporting errors.
+To disable, use a marker::
+
+    import pytest
+    import pytest_sentry
+
+    pytestmarker = pytest.mark.sentry_client({"traces_sample_rate": 0.0})
+
+Advanced Options
+================
+
+``pytest-sentry`` supports marking your tests to use a different DSN, client or
+scope per-test. You can use this to provide custom options to the ``Client``
+object from the `Sentry SDK for Python
+<https://github.com/getsentry/sentry-python>`_::
+
+    import random
+    import pytest
+
+    from sentry_sdk import Scope
+    from pytest_sentry import Client
+
+    @pytest.mark.sentry_client(None)
+    def test_no_sentry():
+        # Even though flaky, this test never gets reported to sentry
+        assert random.random() > 0.5
+
+    @pytest.mark.sentry_client("MY NEW DSN")
+    def test_custom_dsn():
+        # Use a different DSN to report errors for this one
+        assert random.random() > 0.5
+
+    # Other invocations:
+
+    @pytest.mark.sentry_client(Client("CUSTOM DSN"))
+    @pytest.mark.sentry_client(lambda: Client("CUSTOM DSN"))
+    @pytest.mark.sentry_client(Scope(Client("CUSTOM DSN")))
+    @pytest.mark.sentry_client({"dsn": ..., "debug": True})
+
+
+The ``Client`` class exposed by ``pytest-sentry`` only has different default
+integrations. It disables some of the error-capturing integrations to avoid
+sending random expected errors into your project.
+
+Accessing the used Sentry client
+================================
+
+You will notice that the global functions such as
+``sentry_sdk.capture_message`` will not actually send events into the same DSN
+you configured this plugin with. That's because ``pytest-sentry`` goes to
+extreme lenghts to keep its own SDK setup separate from the SDK setup of the
+tested code.
+
+``pytest-sentry`` exposes the ``sentry_test_scope`` fixture whose return value is
+the ``Scope`` being used to send events to Sentry. Use ``with use_scope(entry_test_scope):``
+to temporarily switch context. You can use this to set custom tags like so::
+
+    def test_foo(sentry_test_scope):
+        with use_scope(sentry_test_scope):
+            sentry_sdk.set_tag("pull_request", os.environ['EXAMPLE_CI_PULL_REQUEST'])
+
+
+Why all the hassle with the context manager? Just imagine if your tested
+application would start to log some (expected) errors on its own. You would
+immediately exceed your quota!
+
+Always reporting test failures
+==============================
+
+You can always report all test failures to Sentry by setting the environment
+variable ``PYTEST_SENTRY_ALWAYS_REPORT=1``.
+
+This can be enabled for builds on the ``main`` or release branch, to catch
+certain kinds of tests that are flaky across builds, but consistently fail or
+pass within one testrun.
+
+License
+=======
+
+Licensed under 2-clause BSD, see ``LICENSE``.
```

### Comparing `pytest-sentry-0.1.9/README.rst` & `pytest_sentry-0.2.0/pytest_sentry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pytest_sentry
+Version: 0.2.0
+Summary: A pytest plugin to send testrun information to Sentry.io
+Home-page: https://github.com/untitaker/pytest-sentry
+Author: Markus Unterwaditzer
+Author-email: markus@unterwaditzer.net
+License: BSD-2-Clause
+Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: pytest
+Requires-Dist: sentry-sdk==2.0.0rc4
+Requires-Dist: wrapt
+
 =============
 pytest-sentry
 =============
 
 .. image:: https://img.shields.io/pypi/v/pytest-sentry
     :target: https://pypi.org/project/pytest-sentry/
 
@@ -62,36 +77,40 @@
         pytest.runtest.call [one time, sent]
 
   The trace is per-test-item. For correlating transactions across an entire
   test run, use the automatically attached CI tags or attach some tag on your
   own.
 
 To measure performance data, install ``pytest-sentry`` and set
-``PYTEST_SENTRY_DSN``, like with errors.
+``PYTEST_SENTRY_DSN``, like with errors. By default, the extension will send all
+performance data to Sentry. If you want to limit the amount of data sent, you
+can set the ``PYTEST_SENTRY_TRACES_SAMPLE_RATE`` environment variable to a float
+between ``0`` and ``1``. This will cause only a random sample of transactions to
+be sent to Sentry.
 
 Transactions can have noticeable runtime overhead over just reporting errors.
 To disable, use a marker::
 
     import pytest
     import pytest_sentry
 
     pytestmarker = pytest.mark.sentry_client({"traces_sample_rate": 0.0})
 
 Advanced Options
 ================
 
 ``pytest-sentry`` supports marking your tests to use a different DSN, client or
-hub per-test. You can use this to provide custom options to the ``Client``
+scope per-test. You can use this to provide custom options to the ``Client``
 object from the `Sentry SDK for Python
 <https://github.com/getsentry/sentry-python>`_::
 
     import random
     import pytest
 
-    from sentry_sdk import Hub
+    from sentry_sdk import Scope
     from pytest_sentry import Client
 
     @pytest.mark.sentry_client(None)
     def test_no_sentry():
         # Even though flaky, this test never gets reported to sentry
         assert random.random() > 0.5
 
@@ -100,15 +119,15 @@
         # Use a different DSN to report errors for this one
         assert random.random() > 0.5
 
     # Other invocations:
 
     @pytest.mark.sentry_client(Client("CUSTOM DSN"))
     @pytest.mark.sentry_client(lambda: Client("CUSTOM DSN"))
-    @pytest.mark.sentry_client(Hub(Client("CUSTOM DSN")))
+    @pytest.mark.sentry_client(Scope(Client("CUSTOM DSN")))
     @pytest.mark.sentry_client({"dsn": ..., "debug": True})
 
 
 The ``Client`` class exposed by ``pytest-sentry`` only has different default
 integrations. It disables some of the error-capturing integrations to avoid
 sending random expected errors into your project.
 
@@ -117,34 +136,34 @@
 
 You will notice that the global functions such as
 ``sentry_sdk.capture_message`` will not actually send events into the same DSN
 you configured this plugin with. That's because ``pytest-sentry`` goes to
 extreme lenghts to keep its own SDK setup separate from the SDK setup of the
 tested code.
 
-``pytest-sentry`` exposes the ``sentry_test_hub`` fixture whose return value is
-the ``Hub`` being used to send events to Sentry. Use ``with sentry_test_hub:``
+``pytest-sentry`` exposes the ``sentry_test_scope`` fixture whose return value is
+the ``Scope`` being used to send events to Sentry. Use ``with use_scope(entry_test_scope):``
 to temporarily switch context. You can use this to set custom tags like so::
 
-    def test_foo(sentry_test_hub):
-        with sentry_test_hub:
+    def test_foo(sentry_test_scope):
+        with use_scope(sentry_test_scope):
             sentry_sdk.set_tag("pull_request", os.environ['EXAMPLE_CI_PULL_REQUEST'])
 
 
 Why all the hassle with the context manager? Just imagine if your tested
 application would start to log some (expected) errors on its own. You would
 immediately exceed your quota!
 
 Always reporting test failures
 ==============================
 
 You can always report all test failures to Sentry by setting the environment
 variable ``PYTEST_SENTRY_ALWAYS_REPORT=1``.
 
-This can be enabled for builds on the ``master`` or release branch, to catch
+This can be enabled for builds on the ``main`` or release branch, to catch
 certain kinds of tests that are flaky across builds, but consistently fail or
 pass within one testrun.
 
 License
 =======
 
 Licensed under 2-clause BSD, see ``LICENSE``.
```

### Comparing `pytest-sentry-0.1.9/pytest_sentry.py` & `pytest_sentry-0.2.0/pytest_sentry.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 import pytest
 
 import wrapt
 import sentry_sdk
 from sentry_sdk.integrations import Integration
 
-from sentry_sdk import Hub, capture_exception
+from sentry_sdk import Scope, capture_exception
 from sentry_sdk.tracing import Transaction
-from sentry_sdk.scope import add_global_event_processor
+from sentry_sdk.scope import add_global_event_processor, use_scope
 
 _ENVVARS_AS_TAGS = frozenset(
     [
         "GITHUB_WORKFLOW",  # The name of the workflow.
         "GITHUB_RUN_ID",  # A unique number for each run within a repository. This number does not change if you re-run the workflow run.
         "GITHUB_RUN_NUMBER",  # A unique number for each run of a particular workflow in a repository. This number begins at 1 for the workflow's first run, and increments with each new run. This number does not change if you re-run the workflow run.
         "GITHUB_ACTION",  # The unique identifier (id) of the action.
@@ -55,15 +55,15 @@
 
         self.always_report = always_report
 
     @staticmethod
     def setup_once():
         @add_global_event_processor
         def procesor(event, hint):
-            if Hub.current.get_integration(PytestIntegration) is None:
+            if Scope.get_client().get_integration(PytestIntegration) is None:
                 return event
 
             for key in _ENVVARS_AS_TAGS:
                 value = os.environ.get(key)
                 if not value:
                     continue
                 event.setdefault("tags", {})["pytest_environ.{}".format(key)] = value
@@ -78,87 +78,90 @@
 
             return event
 
 
 class Client(sentry_sdk.Client):
     def __init__(self, *args, **kwargs):
         kwargs.setdefault("dsn", os.environ.get("PYTEST_SENTRY_DSN", None))
-        kwargs.setdefault("traces_sample_rate", 1.0)
+        kwargs.setdefault(
+            "traces_sample_rate",
+            float(os.environ.get("PYTEST_SENTRY_TRACES_SAMPLE_RATE", 1.0)),
+        )
         kwargs.setdefault("_experiments", {}).setdefault(
             "auto_enabling_integrations", True
         )
-        kwargs.setdefault("environment", "test")
+        kwargs.setdefault("environment", os.environ.get("SENTRY_ENVIRONMENT", "test"))
         kwargs.setdefault("integrations", []).append(PytestIntegration())
 
         sentry_sdk.Client.__init__(self, *args, **kwargs)
 
 
 def hookwrapper(itemgetter, **kwargs):
     """
-    A version of pytest.hookimpl that sets the current hub to the correct one
+    A version of pytest.hookimpl that sets the current scope to the correct one
     and skips the hook if the integration is disabled.
 
     Assumes the function is a hookwrapper, ie yields once
     """
 
     @wrapt.decorator
-    def _with_hub(wrapped, instance, args, kwargs):
+    def _with_scope(wrapped, instance, args, kwargs):
         item = itemgetter(*args, **kwargs)
-        hub = _resolve_hub_marker_value(item.get_closest_marker("sentry_client"))
+        scope = _resolve_scope_marker_value(item.get_closest_marker("sentry_client"))
 
-        if hub.get_integration(PytestIntegration) is None:
+        if scope.client.get_integration(PytestIntegration) is None:
             yield
         else:
-            with hub:
+            with use_scope(scope):
                 gen = wrapped(*args, **kwargs)
 
             while True:
                 try:
-                    with hub:
+                    with use_scope(scope):
                         chunk = next(gen)
 
                     y = yield chunk
 
-                    with hub:
+                    with use_scope(scope):
                         gen.send(y)
 
                 except StopIteration:
                     break
 
     def inner(f):
-        return pytest.hookimpl(hookwrapper=True, **kwargs)(_with_hub(f))
+        return pytest.hookimpl(hookwrapper=True, **kwargs)(_with_scope(f))
 
     return inner
 
 
 def pytest_load_initial_conftests(early_config, parser, args):
     early_config.addinivalue_line(
         "markers",
-        "sentry_client(client=None): Use this client instance for reporting tests. You can also pass a DSN string directly, or a `Hub` if you need it.",
+        "sentry_client(client=None): Use this client instance for reporting tests. You can also pass a DSN string directly, or a `Scope` if you need it.",
     )
 
 
 def _start_transaction(**kwargs):
     transaction = Transaction.continue_from_headers(
-        dict(Hub.current.iter_trace_propagation_headers()), **kwargs
+        dict(Scope.get_current_scope().iter_trace_propagation_headers()), **kwargs
     )
     transaction.same_process_as_parent = True
     return sentry_sdk.start_transaction(transaction)
 
 
 @hookwrapper(itemgetter=lambda item: item)
 def pytest_runtest_protocol(item):
     op = "pytest.runtest.protocol"
 
     name = item.nodeid
 
     # We use the full name including parameters because then we can identify
     # how often a single test has run as part of the same GITHUB_RUN_ID.
 
-    with _start_transaction(op=op, name=u"{} {}".format(op, name)) as tx:
+    with _start_transaction(op=op, name="{} {}".format(op, name)) as tx:
         yield
 
         # Purposefully drop transaction to spare quota. We only created it to
         # have a trace_id to correlate by.
         tx.sampled = False
 
 
@@ -167,102 +170,105 @@
     op = "pytest.runtest.call"
 
     name = item.nodeid
 
     # We use the full name including parameters because then we can identify
     # how often a single test has run as part of the same GITHUB_RUN_ID.
 
-    with _start_transaction(op=op, name=u"{} {}".format(op, name)):
+    with _start_transaction(op=op, name="{} {}".format(op, name)):
         yield
 
 
 @hookwrapper(itemgetter=lambda fixturedef, request: request._pyfuncitem)
 def pytest_fixture_setup(fixturedef, request):
     op = "pytest.fixture.setup"
-    with _start_transaction(op=op, name=u"{} {}".format(op, fixturedef.argname)) as transaction:
+    with _start_transaction(
+        op=op, name="{} {}".format(op, fixturedef.argname)
+    ) as transaction:
         transaction.set_tag("pytest.fixture.scope", fixturedef.scope)
         yield
 
 
 @hookwrapper(tryfirst=True, itemgetter=lambda item, call: item)
 def pytest_runtest_makereport(item, call):
     sentry_sdk.set_tag("pytest.result", "pending")
     report = yield
-    sentry_sdk.set_tag("pytest.result", report.get_result().outcome)
+    outcome = report.get_result().outcome
+    sentry_sdk.set_tag("pytest.result", outcome)
 
-    if call.when == "call":
+    if call.when == "call" and outcome != "skipped":
         cur_exc_chain = getattr(item, "pytest_sentry_exc_chain", [])
 
         if call.excinfo is not None:
             item.pytest_sentry_exc_chain = cur_exc_chain = cur_exc_chain + [
                 call.excinfo
             ]
 
-        integration = Hub.current.get_integration(PytestIntegration)
+        integration = Scope.get_client().get_integration(PytestIntegration)
 
         if (cur_exc_chain and call.excinfo is None) or integration.always_report:
             for exc_info in cur_exc_chain:
                 capture_exception((exc_info.type, exc_info.value, exc_info.tb))
 
 
-DEFAULT_HUB = Hub(Client())
+DEFAULT_SCOPE = Scope(client=Client())
 
-_hub_cache = {}
+_scope_cache = {}
 
 
-def _resolve_hub_marker_value(marker_value):
-    if id(marker_value) not in _hub_cache:
-        _hub_cache[id(marker_value)] = rv = _resolve_hub_marker_value_uncached(
+def _resolve_scope_marker_value(marker_value):
+    if id(marker_value) not in _scope_cache:
+        _scope_cache[id(marker_value)] = rv = _resolve_scope_marker_value_uncached(
             marker_value
         )
         return rv
 
-    return _hub_cache[id(marker_value)]
+    return _scope_cache[id(marker_value)]
 
 
-def _resolve_hub_marker_value_uncached(marker_value):
+def _resolve_scope_marker_value_uncached(marker_value):
     if marker_value is None:
-        marker_value = DEFAULT_HUB
+        marker_value = DEFAULT_SCOPE
     else:
         marker_value = marker_value.args[0]
 
     if callable(marker_value):
         marker_value = marker_value()
 
     if marker_value is None:
         # user explicitly disabled reporting
-        return Hub()
+        return Scope()
 
     if isinstance(marker_value, str):
-        return Hub(Client(marker_value))
+        return Scope(client=Client(marker_value))
 
     if isinstance(marker_value, dict):
-        return Hub(Client(**marker_value))
+        return Scope(client=Client(**marker_value))
 
     if isinstance(marker_value, Client):
-        return Hub(marker_value)
+        return Scope(client=marker_value)
 
-    if isinstance(marker_value, Hub):
+    if isinstance(marker_value, Scope):
         return marker_value
 
     raise RuntimeError(
-        "The `sentry_client` value must be a client, hub or string, not {}".format(
+        "The `sentry_client` value must be a client, scope or string, not {}".format(
             repr(type(marker_value))
         )
     )
 
 
 @pytest.fixture
-def sentry_test_hub(request):
+def sentry_test_scope(request):
     """
-    Gives back the current hub.
+    Gives back the current scope.
     """
 
     item = request.node
-    return _resolve_hub_marker_value(item.get_closest_marker("sentry_client"))
+    return _resolve_scope_marker_value(item.get_closest_marker("sentry_client"))
 
 
 def _process_stacktrace(stacktrace):
     for frame in stacktrace["frames"]:
         frame["in_app"] = not frame["module"].startswith(
             ("_pytest.", "pytest.", "pluggy.")
         )
```

