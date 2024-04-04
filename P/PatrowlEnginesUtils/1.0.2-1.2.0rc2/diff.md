# Comparing `tmp/PatrowlEnginesUtils-1.0.2.tar.gz` & `tmp/PatrowlEnginesUtils-1.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PatrowlEnginesUtils-1.0.2.tar", last modified: Mon Jul 12 14:28:25 2021, max compression
+gzip compressed data, was "PatrowlEnginesUtils-1.2.0rc2.tar", last modified: Thu Apr  4 07:46:41 2024, max compression
```

## Comparing `PatrowlEnginesUtils-1.0.2.tar` & `PatrowlEnginesUtils-1.2.0rc2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2021-07-12 14:28:25.000000 PatrowlEnginesUtils-1.0.2/
--rw-r--r--   0 nicolas    (501) staff       (20)      376 2021-07-12 14:28:25.000000 PatrowlEnginesUtils-1.0.2/PKG-INFO
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2021-07-12 14:28:25.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)      376 2021-07-12 14:28:24.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      357 2021-07-12 14:28:24.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)       20 2021-07-12 14:28:24.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils.egg-info/top_level.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2021-07-12 14:28:24.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils.egg-info/dependency_links.txt
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2021-07-12 14:28:25.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils/
--rw-r--r--   0 nicolas    (501) staff       (20)     5984 2021-01-20 13:03:59.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils/PatrowlEngineTest.py
--rw-r--r--   0 nicolas    (501) staff       (20)      248 2021-07-12 14:28:13.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)    17510 2021-07-12 14:28:13.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils/PatrowlEngine.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1120 2019-06-14 07:45:00.000000 PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils/PatrowlEngineExceptions.py
--rw-r--r--   0 nicolas    (501) staff       (20)      159 2021-07-12 14:28:13.000000 PatrowlEnginesUtils-1.0.2/README.md
--rw-r--r--   0 nicolas    (501) staff       (20)      506 2021-07-12 14:28:13.000000 PatrowlEnginesUtils-1.0.2/setup.py
--rw-r--r--   0 nicolas    (501) staff       (20)       67 2021-07-12 14:28:25.000000 PatrowlEnginesUtils-1.0.2/setup.cfg
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    34523 2024-04-02 14:20:35.000000 PatrowlEnginesUtils-1.2.0rc2/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/PKG-INFO
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    23779 2024-04-03 15:51:44.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngine.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1074 2024-04-03 12:48:12.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngineExceptions.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5949 2024-04-03 12:48:12.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngineTest.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      252 2024-04-03 15:51:44.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/__init__.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2024-04-04 07:46:41.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      365 2024-04-04 07:46:41.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2024-04-04 07:46:41.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       20 2024-04-04 07:46:41.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      159 2024-04-02 14:20:35.000000 PatrowlEnginesUtils-1.2.0rc2/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       67 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      510 2024-04-03 15:51:44.000000 PatrowlEnginesUtils-1.2.0rc2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils/PatrowlEngineTest.py` & `PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngineTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,77 +93,79 @@
             assert r.json()["status"] == "SUCCESS"
         except AssertionError:
             print(r.json())
             assert False
         finally:
             return r.json()
 
-    def custom_test(self, test_name, assets, scan_policy=None, is_valid=True,
-                    max_timeout=1200, scan_id=random.randint(1000000, 1999999)):
+    def custom_test(
+        self,
+        test_name,
+        assets,
+        scan_policy=None,
+        is_valid=True,
+        max_timeout=1200,
+        scan_id=random.randint(1000000, 1999999),
+    ):
         """Start a custom test."""
         print("test-{}-custom: {}".format(self.engine_name, test_name))
         if scan_policy is None:
             scan_policy = {}
-        post_data = {
-            "assets":  assets,
-            "options": scan_policy,
-            "scan_id": str(scan_id)
-        }
+        post_data = {"assets": assets, "options": scan_policy, "scan_id": str(scan_id)}
 
         r = requests.post(
             url="{}/startscan".format(self.base_url),
             data=json.dumps(post_data),
-            headers={
-                'Content-type': 'application/json',
-                'Accept': 'application/json'
-                })
+            headers={"Content-type": "application/json", "Accept": "application/json"},
+        )
         try:
             assert r.status_code == 200
-            assert r.json()['status'] == "accepted"
+            assert r.json()["status"] == "accepted"
         except AssertionError:
             print(r.json())
             assert False
 
         # Wait until scan is finished
         timeout_start = time.time()
         # Mitigate PID error
         retries = 0
         has_error = False
         while time.time() < timeout_start + max_timeout:
-            r = requests.get(
-                url="{}/status/{}".format(self.base_url, scan_id))
+            r = requests.get(url="{}/status/{}".format(self.base_url, scan_id))
             if r.json()["status"] in ("SCANNING", "STARTED"):
                 time.sleep(3)
-            elif (r.json()["status"] == "ERROR" and "reason" in r.json() and
-                  r.json()["reason"] == "No PID found" and retries < 3):
+            elif (
+                r.json()["status"] == "ERROR"
+                and "reason" in r.json()
+                and r.json()["reason"] == "No PID found"
+                and retries < 3
+            ):
                 retries += 1
                 time.sleep(3)
             else:
                 if r.json()["status"] == "FINISHED":
                     assert True
                 else:
                     has_error = True
                     assert False
                 break
 
         # Get findings
         if not has_error:
             findings = {}
-            r = requests.get(
-                url="{}/getfindings/{}".format(self.base_url, scan_id))
+            r = requests.get(url="{}/getfindings/{}".format(self.base_url, scan_id))
             try:
-                assert r.json()['status'] == "success"
+                assert r.json()["status"] == "success"
                 findings = r.json()
             except AssertionError:
                 print(r.json())
                 assert False
 
             # Get report
-            r = requests.get(
-                url="{}/getreport/{}".format(self.base_url, scan_id))
+            r = requests.get(url="{}/getreport/{}".format(self.base_url, scan_id))
             try:
                 # check the file name & siza !!
                 assert True
                 # assert r.json()['scan']['status'] == "FINISHED"
             except AssertionError:
                 print(r.json())
                 assert False
```

### Comparing `PatrowlEnginesUtils-1.0.2/PatrowlEnginesUtils/PatrowlEngineExceptions.py` & `PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngineExceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     This class is all about exceptions based directly on PatrowlEnginese.
 
     It will consist of a **code** and a **message** describing the reason of
     the exception shortly.
     """
 
     _error_codes = {
-        1000: 'Configuration file not found.',
-        1001: 'Report file not found.',
-        1002: 'Scan_id not found in current scans.',
-        1003: 'Scan not finished.',
+        1000: "Configuration file not found.",
+        1001: "Report file not found.",
+        1002: "Scan_id not found in current scans.",
+        1003: "Scan not finished.",
     }
 
     def __init__(self, code, msg=None):
         """Initialise a new PatrowlEngineExceptions."""
         Exception.__init__(self)
         self.code = code
         if msg:
@@ -28,12 +28,8 @@
 
     def __str__(self):
         """Return a string-formated object."""
         return "Error %i: %s" % (self.code, self.message)
 
     def to_dict(self):
         """Return a dict-formated object."""
-        return {
-            "code": self.code,
-            "message": self.message,
-            "status": "ERROR"
-        }
+        return {"code": self.code, "message": self.message, "status": "ERROR"}
```

