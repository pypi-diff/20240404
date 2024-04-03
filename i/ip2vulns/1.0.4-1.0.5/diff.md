# Comparing `tmp/ip2vulns-1.0.4.tar.gz` & `tmp/ip2vulns-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip2vulns-1.0.4.tar", last modified: Tue Apr  2 23:24:47 2024, max compression
+gzip compressed data, was "ip2vulns-1.0.5.tar", last modified: Wed Apr  3 23:37:54 2024, max compression
```

## Comparing `ip2vulns-1.0.4.tar` & `ip2vulns-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,35 @@
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.102776 ip2vulns-1.0.4/
--rw-r--r--   0 boxhezi    (501) staff       (20)     1064 2024-03-28 00:46:45.000000 ip2vulns-1.0.4/LICENSE
--rw-r--r--   0 boxhezi    (501) staff       (20)     2939 2024-04-02 23:24:47.101947 ip2vulns-1.0.4/PKG-INFO
--rw-r--r--   0 boxhezi    (501) staff       (20)     2611 2024-04-02 23:22:09.000000 ip2vulns-1.0.4/README.md
--rw-r--r--   0 boxhezi    (501) staff       (20)       38 2024-04-02 23:24:47.103114 ip2vulns-1.0.4/setup.cfg
--rw-r--r--   0 boxhezi    (501) staff       (20)     1076 2024-04-02 22:34:53.000000 ip2vulns-1.0.4/setup.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.086252 ip2vulns-1.0.4/src/
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.091334 ip2vulns-1.0.4/src/ip2vulns/
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.098741 ip2vulns-1.0.4/src/ip2vulns/Module/
--rw-r--r--   0 boxhezi    (501) staff       (20)     1175 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Module/CVE.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     1238 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Module/InternetDB.py
--rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Module/__init__.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.100297 ip2vulns-1.0.4/src/ip2vulns/Services/
--rw-r--r--   0 boxhezi    (501) staff       (20)     1245 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Services/CveService.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     5485 2024-04-02 23:18:36.000000 ip2vulns-1.0.4/src/ip2vulns/Services/InternetDBService.py
--rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Services/__init__.py
--rw-r--r--   0 boxhezi    (501) staff       (20)       62 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/__init__.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     2103 2024-04-02 23:20:37.000000 ip2vulns-1.0.4/src/ip2vulns/ip2vulns.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     3512 2024-04-02 23:23:47.000000 ip2vulns-1.0.4/src/ip2vulns/utils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)       22 2024-04-02 22:35:28.000000 ip2vulns-1.0.4/src/ip2vulns/version.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.100856 ip2vulns-1.0.4/src/ip2vulns.egg-info/
--rw-r--r--   0 boxhezi    (501) staff       (20)     2939 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/PKG-INFO
--rw-r--r--   0 boxhezi    (501) staff       (20)      546 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/SOURCES.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)        1 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/dependency_links.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)       52 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/entry_points.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)       14 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/requires.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)        9 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/top_level.txt
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.021999 ip2vulns-1.0.5/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1064 2024-03-28 00:46:45.000000 ip2vulns-1.0.5/LICENSE
+-rw-r--r--   0 boxhezi    (501) staff       (20)     3136 2024-04-03 23:37:54.021487 ip2vulns-1.0.5/PKG-INFO
+-rw-r--r--   0 boxhezi    (501) staff       (20)     2808 2024-04-03 23:35:50.000000 ip2vulns-1.0.5/README.md
+-rw-r--r--   0 boxhezi    (501) staff       (20)       38 2024-04-03 23:37:54.022101 ip2vulns-1.0.5/setup.cfg
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1076 2024-04-02 22:34:53.000000 ip2vulns-1.0.5/setup.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:53.997446 ip2vulns-1.0.5/src/
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.002416 ip2vulns-1.0.5/src/ip2vulns/
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.007042 ip2vulns-1.0.5/src/ip2vulns/Module/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1175 2024-04-03 03:15:15.000000 ip2vulns-1.0.5/src/ip2vulns/Module/CVE.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1297 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Module/InternetDB.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.5/src/ip2vulns/Module/__init__.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.008763 ip2vulns-1.0.5/src/ip2vulns/Services/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1249 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Services/CveService.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     5833 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Services/InternetDBService.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.5/src/ip2vulns/Services/__init__.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.020087 ip2vulns-1.0.5/src/ip2vulns/Utils/
+-rw-r--r--   0 boxhezi    (501) staff       (20)      470 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/DatetimeUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1031 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/IpUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      286 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/ListUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      675 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/OutputUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      203 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/PathUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      173 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/PipeUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)      303 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/QueryUtils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/Utils/__init__.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)       63 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/__init__.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     2555 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/ip2vulns.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)       22 2024-04-03 23:33:16.000000 ip2vulns-1.0.5/src/ip2vulns/version.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-03 23:37:54.020884 ip2vulns-1.0.5/src/ip2vulns.egg-info/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     3136 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/PKG-INFO
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1044 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/SOURCES.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)        1 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/dependency_links.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)       52 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/entry_points.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)       14 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/requires.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)        9 2024-04-03 23:37:53.000000 ip2vulns-1.0.5/src/ip2vulns.egg-info/top_level.txt
```

### Comparing `ip2vulns-1.0.4/LICENSE` & `ip2vulns-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.4/PKG-INFO` & `ip2vulns-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip2vulns
-Version: 1.0.4
+Version: 1.0.5
 Summary: An IP to vulnerability utility
 Home-page: https://github.com/BoxHezi/ip2vulns
 Author: Box Hezi
 Author-email: hezipypi.yixdpu@bumpmail.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -66,14 +66,18 @@
 
 ## Example
 
 - `ip2vulns -i <ip address> <cidr>`
 - `ip2vulns -i <ip address> <cidr> -s 7`
 - `echo "<ip address>" | ip2vulns`
 - `echo "<ip address>" | ip2vulns -s 7`
+- `ip2vulns -i <input file>`
+- `cat <input file> | ip2vulns`
+
+**When input is file, only the first element will be considered**<br>_TODO: add support for multiple files and with valid IPs or CIDR_
 
 ## Use `ip2vulns` in Python script
 
 ```python
 from ip2vulns import ip2vulns_scan
 
 # s => success list
```

### Comparing `ip2vulns-1.0.4/README.md` & `ip2vulns-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,18 @@
 
 ## Example
 
 - `ip2vulns -i <ip address> <cidr>`
 - `ip2vulns -i <ip address> <cidr> -s 7`
 - `echo "<ip address>" | ip2vulns`
 - `echo "<ip address>" | ip2vulns -s 7`
+- `ip2vulns -i <input file>`
+- `cat <input file> | ip2vulns`
+
+**When input is file, only the first element will be considered**<br>_TODO: add support for multiple files and with valid IPs or CIDR_
 
 ## Use `ip2vulns` in Python script
 
 ```python
 from ip2vulns import ip2vulns_scan
 
 # s => success list
```

### Comparing `ip2vulns-1.0.4/setup.py` & `ip2vulns-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.4/src/ip2vulns/Module/CVE.py` & `ip2vulns-1.0.5/src/ip2vulns/Module/CVE.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.4/src/ip2vulns/Module/InternetDB.py` & `ip2vulns-1.0.5/src/ip2vulns/Module/InternetDB.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from .. import utils
+from ..Utils import IpUtils
+from ..Utils import DatetimeUtils
 
 
 class InternetDB:
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
-        self.ip_int = utils.ip_int(self.ip)
-        self.last_updated = utils.get_now_datetime()
+        self.ip_int = IpUtils.ip_int(self.ip)
+        self.last_updated = DatetimeUtils.get_now_datetime()
 
     def __repr__(self):
         out = [f"\nIP: {self.ip}"]
         if self.hostnames:
             out.extend(["\nHostnames:", *(f"\t{name}" for name in self.hostnames)])
         if self.ports:
             out.extend(["\nPorts:", *(f"\t{port}" for port in self.ports)])
@@ -18,15 +19,15 @@
             out.extend(["\nVulns:", *(f"\t{vuln}" for vuln in self.vulns)])
         return '\n'.join(out) + "\n"
 
     def __str__(self):
         # re-order keys of attribute
         attribute_order = ["ip_int", "ip", "hostnames", "ports", "cpes", "vulns", "tags", "last_updated"]
         out_dict = {k: getattr(self, k) for k in attribute_order}
-        out_dict.update({"last_updated": utils.datetime_2_str(out_dict.get("last_updated"))})
+        out_dict.update({"last_updated": DatetimeUtils.datetime_2_str(out_dict.get("last_updated"))})
 
         out = []
         for k, v in out_dict.items():
             if not k.startswith("_"):
                 if isinstance(v, list):
                     v = "|".join([str(i) for i in v])
                 out.append(str(v))
```

### Comparing `ip2vulns-1.0.4/src/ip2vulns/Services/CveService.py` & `ip2vulns-1.0.5/src/ip2vulns/Services/CveService.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-import requests
-
 from typing import Optional
 
-from .. import utils
 from ..Module.CVE import CVE
 
-# Get CVE Info from: https://github.com/fkie-cad/nvd-json-data-feeds/tree/main
+from ..Utils import QueryUtils
 
+# Get CVE Info from: https://github.com/fkie-cad/nvd-json-data-feeds/tree/main
 # get raw content: https://raw.githubusercontent.com/fkie-cad/nvd-json-data-feeds/main/<CVE years>/<CVE-id-prefix>/<CVE-id>.json
 
 
-END_POINT_PREFIX = "https://raw.githubusercontent.com/fkie-cad/nvd-json-data-feeds/main/"
+ENDPOINT_PREFIX = "https://raw.githubusercontent.com/fkie-cad/nvd-json-data-feeds/main/"
 
 
 def construct_url(cve_id: str) -> str:
     """
     Constructs a URL based on the given CVE ID.
 
     :param cve_id: The CVE ID used to construct the URL.
     :return: The constructed URL.
     """
     year = cve_id[0:8]
     branch = cve_id[:-2] + "xx"
     ending = cve_id + ".json"
 
-    return END_POINT_PREFIX + year + "/" + branch + "/" + ending
+    return ENDPOINT_PREFIX + year + "/" + branch + "/" + ending
 
 
 def get_cve_info(cve_id: str) -> Optional[CVE]:
     """
     Retrieves information about a CVE using the provided CVE ID.
 
     :param cve_id: The ID of the CVE.
     :return: An CVE instance, or None if an exception occurs.
     """
     cve_data_endpoint = construct_url(cve_id)
     try:
-        resp = requests.get(cve_data_endpoint)
-        resp_json = utils.resp_2_json(resp)
+        resp = QueryUtils.get_query(cve_data_endpoint)
+        resp_json = QueryUtils.resp_2_json(resp)
         return CVE(**resp_json)
     except:
         print(f"Exception while querying CVE {cve_id}")
         return None
```

### Comparing `ip2vulns-1.0.4/src/ip2vulns/Services/InternetDBService.py` & `ip2vulns-1.0.5/src/ip2vulns/Services/InternetDBService.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 from tqdm import tqdm
 from typing import Optional
 
 from ..Module.InternetDB import InternetDB
 from ..Module.CVE import CVE
-from .. import utils
+
+# from ..Utils import QueryUtils
+# from ..Utils import IpUtils
+# from ..Utils import ListUtils
+# from ..Utils import OutputUtils
+from ..Utils import QueryUtils
+from ..Utils import IpUtils
+from ..Utils import ListUtils
+from ..Utils import OutputUtils
 
 from . import CveService
 
 # ref: https://internetdb.shodan.io/
 
 # local CVE cache to avoid searching duplicate CVEs
 # structure { "CVE-YYYY-XXXX" : CVE instance }
 CVE_CACHE: dict[str, CVE] = {}
 
 
-def list_to_ips(ls: list, ipv6: bool = False) -> list:
+def input_list_to_ips(ls: list, ipv6: bool = False) -> list:
     """
     convert input list (either IPs or cidr, or both) to list of ip
     :param ls: list to convert
     :param ipv6: use IPv6 if True. Default set to False
     :return: a list contains IP addresses
     """
     temp = []
     for i in ls:
-        if utils.is_cidr(i):
-            temp += utils.cidr2ip(i, ipv6)
+        if IpUtils.is_cidr(i):
+            temp += IpUtils.cidr2ip(i, ipv6)
         else:
             temp.append(i)
     return list(dict.fromkeys(temp))  # deduplicate
 
 
 def query_idb(ip: str) -> Optional[InternetDB]:
     """
     query internetdb api for ip
     :param ip: target ip address
     :return: InternetDB instance, None if no information is available
     """
-    resp = utils.internet_db_query(ip, 50)
-    resp_json = utils.resp_2_json(resp)
+    idb_prefix = "https://internetdb.shodan.io/"
+    idb_endpoint = idb_prefix + ip
+    resp = QueryUtils.get_query(idb_endpoint)
+    resp_json = QueryUtils.resp_2_json(resp)
     if "ip" not in resp_json:
         return None
     return InternetDB(**resp_json)
 
 
 def filter_cvss(idb: InternetDB, cvss_threshold: float) -> bool:
     """
@@ -78,15 +88,15 @@
     :param failure_list: A list of IP addresses where exceptions occurred during querying from the Shodan InternetDB API.
     :param out_dest: The output option, which can be 'stdout' (default), 'csv', or 'json'.
     """
     if len(success_list) != 0:
         if not disable_stdout:
             for item in success_list:
                 print(item)
-        out_dest and utils.output_to_dest(success_list, out_dest)  # writing to destination
+        out_dest and OutputUtils.output_to_dest(success_list, out_dest)  # writing to destination
     if len(failure_list) != 0:
         print("\nException happened during following IP addresses: ")
         for ip in failure_list:
             print(ip)
 
 
 def start_scan(ips: list, cvss_threshold: float) -> tuple[list, list]:
@@ -113,15 +123,15 @@
 
 def start(targets: list, out_dest: str = None, cvss_threshold: float = 0, disable_stdout: bool = False, ipv6: bool = False) -> tuple[list, list]:
     if not isinstance(targets, list):
         raise ValueError("IP addresses or CIDR need to be passed in as a LIST")
 
     full_s_list = []  # store InternetDB instance for all ips has available information from internet.shodan.io
     full_f_list = []  # store ip addresses while exception happened during any stage of the scan progress
-    to_scan_list = utils.split_list(list_to_ips(targets, ipv6))
+    to_scan_list = ListUtils.split_list(input_list_to_ips(targets, ipv6))
     for i in range(len(to_scan_list)):
         s_list, f_list = start_scan(to_scan_list[i], cvss_threshold)
         full_s_list += s_list
         full_f_list += f_list
     if len(full_s_list) != 0 or len(full_f_list) != 0:
         write_result(full_s_list, full_f_list, out_dest, disable_stdout)
     else:
```

### Comparing `ip2vulns-1.0.4/src/ip2vulns/ip2vulns.py` & `ip2vulns-1.0.5/src/ip2vulns/ip2vulns.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import argparse
 
 from . import version
-from . import utils
 from .Services import InternetDBService
 
-
-# TODO: add file input support
+from .Utils import PipeUtils
 
 
 def init_argparse():
     arg = argparse.ArgumentParser(description="IP 2 vulnerability tools", formatter_class=argparse.RawTextHelpFormatter)
     arg.add_argument("-i", "--input", help="Query information from https://internetdb.shodan.io/\n"
                                                    "support multiple ip and cidr, separate using space, "
                                                    "e.g. -i 8.8.8.8 51.83.59.99 192.168.0.0/24\n",
@@ -22,23 +20,37 @@
                                          "For csv: please specify filename\n"
                                          "For json: a directory out_json will be created")
     arg.add_argument("--disable-stdout", help="Disable stdout", action="store_true")
     arg.add_argument("-v", "--version", help="Print current version", action="store_true")
     return arg
 
 
+def parse_args_input(input: list):
+    if len(input) == 1:  # when input is possibly a file
+        try:
+            with open(input[0]) as f:  # input is a file
+                # print("input is a file")
+                result = [line.strip() for line in f]
+                return result
+        except FileNotFoundError:  # input is ip or cidr
+            pass
+    # print("input is IP or CIDR")
+    return input
+
+
 def main():
     args = init_argparse().parse_args()  # init argparse
 
-    if utils.has_pipe_data():  # read from pipe, enable internetdb by default
-        args.input = utils.read_from_pipe()
+    if PipeUtils.has_pipe_data():  # read from pipe, enable internetdb by default
+        args.input = PipeUtils.read_from_pipe()
     elif not any(vars(args).values()):  # check if argument is provided, if not, print help
         args = init_argparse().parse_args(["-h"])
 
     if args.input:  # type(input) => list
-        InternetDBService.start(args.input, args.out, args.cvss, args.disable_stdout)
+        input_list = parse_args_input(args.input)
+        InternetDBService.start(input_list, args.out, args.cvss, args.disable_stdout)
     elif args.version:
         print(version.__version__)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ip2vulns-1.0.4/src/ip2vulns.egg-info/PKG-INFO` & `ip2vulns-1.0.5/src/ip2vulns.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip2vulns
-Version: 1.0.4
+Version: 1.0.5
 Summary: An IP to vulnerability utility
 Home-page: https://github.com/BoxHezi/ip2vulns
 Author: Box Hezi
 Author-email: hezipypi.yixdpu@bumpmail.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -66,14 +66,18 @@
 
 ## Example
 
 - `ip2vulns -i <ip address> <cidr>`
 - `ip2vulns -i <ip address> <cidr> -s 7`
 - `echo "<ip address>" | ip2vulns`
 - `echo "<ip address>" | ip2vulns -s 7`
+- `ip2vulns -i <input file>`
+- `cat <input file> | ip2vulns`
+
+**When input is file, only the first element will be considered**<br>_TODO: add support for multiple files and with valid IPs or CIDR_
 
 ## Use `ip2vulns` in Python script
 
 ```python
 from ip2vulns import ip2vulns_scan
 
 # s => success list
```

