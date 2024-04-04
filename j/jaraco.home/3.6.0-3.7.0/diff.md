# Comparing `tmp/jaraco.home-3.6.0.tar.gz` & `tmp/jaraco.home-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.home-3.6.0.tar", last modified: Mon Apr  1 16:18:02 2024, max compression
+gzip compressed data, was "jaraco.home-3.7.0.tar", last modified: Thu Apr  4 17:10:46 2024, max compression
```

## Comparing `jaraco.home-3.6.0.tar` & `jaraco.home-3.7.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.127748 jaraco.home-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.123748 jaraco.home-3.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.123748 jaraco.home-3.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-01 16:18:02.127748 jaraco.home-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.123748 jaraco.home-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.119748 jaraco.home-3.6.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.127748 jaraco.home-3.6.0/jaraco/home/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/Gather HDHomeRun Stats.plist
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/mock hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/report-spam-call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.127748 jaraco.home-3.6.0/jaraco.home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-01 16:18:02.131748 jaraco.home-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.526130 jaraco.home-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.522130 jaraco.home-3.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.522130 jaraco.home-3.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-04 17:10:46.526130 jaraco.home-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.522130 jaraco.home-3.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.518129 jaraco.home-3.7.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.526130 jaraco.home-3.7.0/jaraco/home/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/Gather HDHomeRun Stats.plist
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/mock hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/report-spam-call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/jaraco/home/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:10:46.526130 jaraco.home-3.7.0/jaraco.home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 17:10:46.000000 jaraco.home-3.7.0/jaraco.home.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 17:10:46.530130 jaraco.home-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 17:10:31.000000 jaraco.home-3.7.0/tox.ini
```

### Comparing `jaraco.home-3.6.0/.github/workflows/main.yml` & `jaraco.home-3.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.6.0/LICENSE` & `jaraco.home-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.6.0/NEWS.rst` & `jaraco.home-3.7.0/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.7.0
+======
+
+Features
+--------
+
+- Allow time and browser to be specified in spam call reporter.
+
+
 v3.6.0
 ======
 
 Features
 --------
 
 - Add routine to quickly report spam calls to FTC.
```

### Comparing `jaraco.home-3.6.0/PKG-INFO` & `jaraco.home-3.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.6.0
+Version: 3.7.0
 Summary: Some functions supporting the devices in jaraco's home
 Home-page: https://github.com/jaraco/jaraco.home
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,23 +18,25 @@
 Requires-Dist: jaraco.functools
 Requires-Dist: jaraco.mongodb
 Requires-Dist: dnspython
 Requires-Dist: keyring
 Requires-Dist: jaraco.collections
 Requires-Dist: splinter[selenium]
 Requires-Dist: autocommand
+Requires-Dist: python-dateutil
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
 Requires-Dist: mockproc; extra == "testing"
+Requires-Dist: types-python-dateutil; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 
@@ -52,7 +54,21 @@
     :alt: Ruff
 
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
+
+
+Report spam calls
+=================
+
+Jason uses this routine to report spam calls to the FTC:
+
+```
+py -m jaraco.develop.report-spam-call 202-555-1212
+```
+
+It uses `Splinter <https://splinter.readthedocs.io/en/stable/index.html>`_ to automate the process of reporting a spam call through the donotcall.gov website.
+
+It might be overly tuned to a specific class of calls, so feel free to propose extensions to the process to suit more needs.
```

### Comparing `jaraco.home-3.6.0/conftest.py` & `jaraco.home-3.7.0/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import platform
 from importlib.resources import files
 
 import pytest
 from mockproc import mockprocess
 
-
 win_ignore = [
     'jaraco/home/hdhomerun.py',
 ] * (platform.system() == 'Windows')
 
 collect_ignore = [
     'jaraco/home/relay.py',
 ] + win_ignore
```

### Comparing `jaraco.home-3.6.0/docs/conf.py` & `jaraco.home-3.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.6.0/jaraco/home/Gather HDHomeRun Stats.plist` & `jaraco.home-3.7.0/jaraco/home/Gather HDHomeRun Stats.plist`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.6.0/jaraco/home/hdhomerun.py` & `jaraco.home-3.7.0/jaraco/home/hdhomerun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import functools
 import contextlib
-import time
-import subprocess
-import sys
+import functools
 import pathlib
 import random
 import re
+import subprocess
+import sys
+import time
 from importlib.resources import files
 
 import keyring
+
+from jaraco.collections import DictStack
 from jaraco.functools import retry
 from jaraco.mongodb.helper import connect_db
-from jaraco.collections import DictStack
 
 
 def parse_field(item):
     key, value = item.split('=')
     with contextlib.suppress(ValueError):
         value = int(value)
     if value == 'none':
@@ -76,15 +77,15 @@
     return ordered
 
 
 def find_idle_tuner():
     try:
         return next(id for id in shuffled(range(4)) if not get_status(id)['ch'])
     except StopIteration:
-        raise RuntimeError("Could not find idle tuner")
+        raise RuntimeError("Could not find idle tuner") from None
 
 
 def _combine(*dicts):
     return dict(DictStack(dicts))
 
 
 def gather_status():
```

### Comparing `jaraco.home-3.6.0/jaraco/home/relay.py` & `jaraco.home-3.7.0/jaraco/home/relay.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.6.0/jaraco/home/report-spam-call.py` & `jaraco.home-3.7.0/jaraco/home/report-spam-call.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
 import json
 import os
 import re
 import types
 
 import autocommand
-import jaraco.collections
+import dateutil.parser
 from splinter import Browser
 
+import jaraco.collections
 
 DROPPED_CALL = '2'
 
 
 class IdentifierDict(jaraco.collections.KeyTransformingDict):
     @staticmethod
     def transform_key(key):
@@ -29,27 +30,32 @@
     >>> clean_phone("+1 202 555 1212")
     '2025551212'
     """
     return re.sub(r'[-. ]', '', number.removeprefix('+1'))
 
 
 @autocommand.autocommand(__name__)
-def report_spam_call(number, comment='', close=False):
+def report_spam_call(
+    number,
+    comment='',
+    close=False,
+    browser='firefox',
+    when: dateutil.parser.parse = datetime.datetime.now(),  # type: ignore
+):
     """
     Report the common spam calls.
     """
     contact = read_contact_info()
-    browser = Browser('firefox')
+    browser = Browser(browser)
     browser.visit('https://www.donotcall.gov/report.html')
     browser.find_by_value('Continue').click()
     browser.fill('PhoneTextBox', clean_phone(contact.phone))
-    now = datetime.datetime.now()
-    browser.fill('DateOfCallTextBox', now.strftime('%m/%d/%Y'))
-    browser.select('TimeOfCallDropDownList', now.strftime('%H'))
-    browser.select('ddlMinutes', now.strftime('%M'))
+    browser.fill('DateOfCallTextBox', when.strftime('%m/%d/%Y'))  # type: ignore
+    browser.select('TimeOfCallDropDownList', when.strftime('%H'))  # type: ignore
+    browser.select('ddlMinutes', when.strftime('%M'))  # type: ignore
     browser.choose('PrerecMsg', 'PrerecordMessageYESRadioButton')
     browser.choose('TextMsg', 'PhoneCallRadioButton')
     browser.select(
         'ddlSubjectMatter',
         DROPPED_CALL,
     )
     browser.find_by_value('Continue').click()
```

### Comparing `jaraco.home-3.6.0/jaraco/home/thermostat.py` & `jaraco.home-3.7.0/jaraco/home/thermostat.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 True
 """
 
 import argparse
 import urllib.parse
 from pprint import pprint
 
-import requests
 import lxml.html
+import requests
 
 """
 API wiki: http://central.isaroach.com/wiki/index.php/Main_Page
 """
 
 thermostat = 'http://192.168.14.20'
```

### Comparing `jaraco.home-3.6.0/jaraco.home.egg-info/PKG-INFO` & `jaraco.home-3.7.0/jaraco.home.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.6.0
+Version: 3.7.0
 Summary: Some functions supporting the devices in jaraco's home
 Home-page: https://github.com/jaraco/jaraco.home
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,23 +18,25 @@
 Requires-Dist: jaraco.functools
 Requires-Dist: jaraco.mongodb
 Requires-Dist: dnspython
 Requires-Dist: keyring
 Requires-Dist: jaraco.collections
 Requires-Dist: splinter[selenium]
 Requires-Dist: autocommand
+Requires-Dist: python-dateutil
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
 Requires-Dist: mockproc; extra == "testing"
+Requires-Dist: types-python-dateutil; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 
@@ -52,7 +54,21 @@
     :alt: Ruff
 
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
+
+
+Report spam calls
+=================
+
+Jason uses this routine to report spam calls to the FTC:
+
+```
+py -m jaraco.develop.report-spam-call 202-555-1212
+```
+
+It uses `Splinter <https://splinter.readthedocs.io/en/stable/index.html>`_ to automate the process of reporting a spam call through the donotcall.gov website.
+
+It might be overly tuned to a specific class of calls, so feel free to propose extensions to the process to suit more needs.
```

### Comparing `jaraco.home-3.6.0/jaraco.home.egg-info/SOURCES.txt` & `jaraco.home-3.7.0/jaraco.home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.6.0/pytest.ini` & `jaraco.home-3.7.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.6.0/setup.cfg` & `jaraco.home-3.7.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 	jaraco.functools
 	jaraco.mongodb
 	dnspython
 	keyring
 	jaraco.collections
 	splinter[selenium]
 	autocommand
+	python-dateutil
 
 [options.extras_require]
 testing = 
 	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
 	pytest-cov
 	pytest-mypy
 	pytest-enabler >= 2.2
 	pytest-ruff >= 0.2.1
 	
 	types-requests
 	mockproc
+	types-python-dateutil
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
```

### Comparing `jaraco.home-3.6.0/tox.ini` & `jaraco.home-3.7.0/tox.ini`

 * *Files identical despite different names*

