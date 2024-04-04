# Comparing `tmp/ip2vulns-1.0.5.tar.gz` & `tmp/ip2vulns-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip2vulns-1.0.5.tar", last modified: Wed Apr  3 23:37:54 2024, max compression
+gzip compressed data, was "ip2vulns-1.0.6.tar", last modified: Thu Apr  4 06:07:15 2024, max compression
```

## Comparing `ip2vulns-1.0.5.tar` & `ip2vulns-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.021999 ip2vulns-1.0.5/
--rw-r--r--   0 boxhezi    (501) staff       (20)     1064 2024-03-28 00:46:45.000000 ip2vulns-1.0.5/LICENSE
--rw-r--r--   0 boxhezi    (501) staff       (20)     3136 2024-04-03 23:37:54.021487 ip2vulns-1.0.5/PKG-INFO
--rw-r--r--   0 boxhezi    (501) staff       (20)     2808 2024-04-03 23:35:50.000000 ip2vulns-1.0.5/README.md
--rw-r--r--   0 boxhezi    (501) staff       (20)       38 2024-04-03 23:37:54.022101 ip2vulns-1.0.5/setup.cfg
--rw-r--r--   0 boxhezi    (501) staff       (20)     1076 2024-04-02 22:34:53.000000 ip2vulns-1.0.5/setup.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:53.997446 ip2vulns-1.0.5/src/
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.002416 ip2vulns-1.0.5/src/ip2vulns/
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.007042 ip2vulns-1.0.5/src/ip2vulns/Module/
--rw-r--r--   0 boxhezi    (501) staff       (20)     1175 2024-04-03 03:15:15.000000 ip2vulns-1.0.5/src/ip2vulns/Module/CVE.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     1297 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Module/InternetDB.py
--rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.5/src/ip2vulns/Module/__init__.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.008763 ip2vulns-1.0.5/src/ip2vulns/Services/
--rw-r--r--   0 boxhezi    (501) staff       (20)     1249 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Services/CveService.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     5833 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Services/InternetDBService.py
--rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.5/src/ip2vulns/Services/__init__.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.020087 ip2vulns-1.0.5/src/ip2vulns/Utils/
--rw-r--r--   0 boxhezi    (501) staff       (20)      470 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/DatetimeUtils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     1031 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/IpUtils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)      286 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/ListUtils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)      675 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/OutputUtils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)      203 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/PathUtils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)      173 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/PipeUtils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)      303 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/QueryUtils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/__init__.py
--rw-r--r--   0 boxhezi    (501) staff       (20)       63 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/__init__.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     2555 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/ip2vulns.py
--rw-r--r--   0 boxhezi    (501) staff       (20)       22 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/version.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.020884 ip2vulns-1.0.5/src/ip2vulns.egg-info/
--rw-r--r--   0 boxhezi    (501) staff       (20)     3136 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/PKG-INFO
--rw-r--r--   0 boxhezi    (501) staff       (20)     1044 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/SOURCES.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)        1 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/dependency_links.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)       52 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/entry_points.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)       14 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/requires.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)        9 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/top_level.txt
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-04 06:07:15.976637 ip2vulns-1.0.6/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1064 2024-03-28 00:46:45.000000 ip2vulns-1.0.6/LICENSE
+-rw-r--r--   0 boxhezi    (501) staff       (20)     3136 2024-04-04 06:07:15.975125 ip2vulns-1.0.6/PKG-INFO
+-rw-r--r--   0 boxhezi    (501) staff       (20)     2808 2024-04-03 23:35:50.000000 ip2vulns-1.0.6/README.md
+-rw-r--r--   0 boxhezi    (501) staff       (20)       38 2024-04-04 06:07:15.978120 ip2vulns-1.0.6/setup.cfg
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1076 2024-04-02 22:34:53.000000 ip2vulns-1.0.6/setup.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-04 06:07:15.758024 ip2vulns-1.0.6/src/
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-04 06:07:15.765605 ip2vulns-1.0.6/src/ip2vulns/
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-04 06:07:15.778501 ip2vulns-1.0.6/src/ip2vulns/Module/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1175 2024-04-03 03:15:15.000000 ip2vulns-1.0.6/src/ip2vulns/Module/CVE.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1297 2024-04-03 23:33:16.000000 ip2vulns-1.0.6/src/ip2vulns/Module/InternetDB.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.6/src/ip2vulns/Module/__init__.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-04 06:07:15.781466 ip2vulns-1.0.6/src/ip2vulns/Services/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1249 2024-04-03 23:33:16.000000 ip2vulns-1.0.6/src/ip2vulns/Services/CveService.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     6021 2024-04-04 06:01:59.000000 ip2vulns-1.0.6/src/ip2vulns/Services/InternetDBService.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.6/src/ip2vulns/Services/__init__.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-04 06:07:15.968173 ip2vulns-1.0.6/src/ip2vulns/Utils/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1424 2024-04-04 05:57:30.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/ArgUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      565 2024-04-04 05:12:20.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/DatetimeUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1031 2024-04-03 23:33:16.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/IpUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      302 2024-04-04 03:26:11.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/ListUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      675 2024-04-03 23:33:16.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/OutputUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      203 2024-04-03 23:33:16.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/PathUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      181 2024-04-04 03:28:59.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/PipeUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      707 2024-04-04 05:19:05.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/QueryUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:33:16.000000 ip2vulns-1.0.6/src/ip2vulns/Utils/__init__.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)       63 2024-04-03 23:33:16.000000 ip2vulns-1.0.6/src/ip2vulns/__init__.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      709 2024-04-04 05:59:45.000000 ip2vulns-1.0.6/src/ip2vulns/ip2vulns.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)       22 2024-04-04 06:03:53.000000 ip2vulns-1.0.6/src/ip2vulns/version.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-04 06:07:15.971150 ip2vulns-1.0.6/src/ip2vulns.egg-info/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     3136 2024-04-04 06:07:15.000000 ip2vulns-1.0.6/src/ip2vulns.egg-info/PKG-INFO
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1075 2024-04-04 06:07:15.000000 ip2vulns-1.0.6/src/ip2vulns.egg-info/SOURCES.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)        1 2024-04-04 06:07:15.000000 ip2vulns-1.0.6/src/ip2vulns.egg-info/dependency_links.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)       52 2024-04-04 06:07:15.000000 ip2vulns-1.0.6/src/ip2vulns.egg-info/entry_points.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)       14 2024-04-04 06:07:15.000000 ip2vulns-1.0.6/src/ip2vulns.egg-info/requires.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)        9 2024-04-04 06:07:15.000000 ip2vulns-1.0.6/src/ip2vulns.egg-info/top_level.txt
```

### Comparing `ip2vulns-1.0.5/LICENSE` & `ip2vulns-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.5/PKG-INFO` & `ip2vulns-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip2vulns
-Version: 1.0.5
+Version: 1.0.6
 Summary: An IP to vulnerability utility
 Home-page: https://github.com/BoxHezi/ip2vulns
 Author: Box Hezi
 Author-email: hezipypi.yixdpu@bumpmail.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ip2vulns-1.0.5/README.md` & `ip2vulns-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.5/setup.py` & `ip2vulns-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.5/src/ip2vulns/Module/CVE.py` & `ip2vulns-1.0.6/src/ip2vulns/Module/CVE.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.5/src/ip2vulns/Module/InternetDB.py` & `ip2vulns-1.0.6/src/ip2vulns/Module/InternetDB.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.5/src/ip2vulns/Services/CveService.py` & `ip2vulns-1.0.6/src/ip2vulns/Services/CveService.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.5/src/ip2vulns/Services/InternetDBService.py` & `ip2vulns-1.0.6/src/ip2vulns/Services/InternetDBService.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from tqdm import tqdm
 from typing import Optional
 
 from ..Module.InternetDB import InternetDB
 from ..Module.CVE import CVE
 
-# from ..Utils import QueryUtils
-# from ..Utils import IpUtils
-# from ..Utils import ListUtils
-# from ..Utils import OutputUtils
 from ..Utils import QueryUtils
 from ..Utils import IpUtils
 from ..Utils import ListUtils
 from ..Utils import OutputUtils
 
 from . import CveService
 
@@ -121,17 +117,26 @@
     return success_list, failure_list
 
 
 def start(targets: list, out_dest: str = None, cvss_threshold: float = 0, disable_stdout: bool = False, ipv6: bool = False) -> tuple[list, list]:
     if not isinstance(targets, list):
         raise ValueError("IP addresses or CIDR need to be passed in as a LIST")
 
+    temp_target = []
+    for t in targets:
+        try:
+            with open(t, "r") as f:  # element is a file
+                temp_target += [line.strip() for line in f.readlines()]
+        except FileNotFoundError:  # element is a IP or a CIDR
+            temp_target.append(t)
+    temp_target = input_list_to_ips(temp_target, ipv6)
+
     full_s_list = []  # store InternetDB instance for all ips has available information from internet.shodan.io
     full_f_list = []  # store ip addresses while exception happened during any stage of the scan progress
-    to_scan_list = ListUtils.split_list(input_list_to_ips(targets, ipv6))
+    to_scan_list = ListUtils.split_list(temp_target)
     for i in range(len(to_scan_list)):
         s_list, f_list = start_scan(to_scan_list[i], cvss_threshold)
         full_s_list += s_list
         full_f_list += f_list
     if len(full_s_list) != 0 or len(full_f_list) != 0:
         write_result(full_s_list, full_f_list, out_dest, disable_stdout)
     else:
```

### Comparing `ip2vulns-1.0.5/src/ip2vulns/Utils/IpUtils.py` & `ip2vulns-1.0.6/src/ip2vulns/Utils/IpUtils.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.5/src/ip2vulns/Utils/OutputUtils.py` & `ip2vulns-1.0.6/src/ip2vulns/Utils/OutputUtils.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.5/src/ip2vulns.egg-info/PKG-INFO` & `ip2vulns-1.0.6/src/ip2vulns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip2vulns
-Version: 1.0.5
+Version: 1.0.6
 Summary: An IP to vulnerability utility
 Home-page: https://github.com/BoxHezi/ip2vulns
 Author: Box Hezi
 Author-email: hezipypi.yixdpu@bumpmail.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ip2vulns-1.0.5/src/ip2vulns.egg-info/SOURCES.txt` & `ip2vulns-1.0.6/src/ip2vulns.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/ip2vulns.egg-info/top_level.txt
 src/ip2vulns/Module/CVE.py
 src/ip2vulns/Module/InternetDB.py
 src/ip2vulns/Module/__init__.py
 src/ip2vulns/Services/CveService.py
 src/ip2vulns/Services/InternetDBService.py
 src/ip2vulns/Services/__init__.py
+src/ip2vulns/Utils/ArgUtils.py
 src/ip2vulns/Utils/DatetimeUtils.py
 src/ip2vulns/Utils/IpUtils.py
 src/ip2vulns/Utils/ListUtils.py
 src/ip2vulns/Utils/OutputUtils.py
 src/ip2vulns/Utils/PathUtils.py
 src/ip2vulns/Utils/PipeUtils.py
 src/ip2vulns/Utils/QueryUtils.py
```

