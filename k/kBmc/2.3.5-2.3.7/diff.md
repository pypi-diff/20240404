# Comparing `tmp/kBmc-2.3.5.tar.gz` & `tmp/kBmc-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kBmc-2.3.5.tar", last modified: Tue Mar 26 05:18:50 2024, max compression
+gzip compressed data, was "kBmc-2.3.7.tar", last modified: Thu Apr  4 05:47:18 2024, max compression
```

## Comparing `kBmc-2.3.5.tar` & `kBmc-2.3.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-03-26 05:18:50.608601 kBmc-2.3.5/
--rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-17 05:54:12.000000 kBmc-2.3.5/LICENSE
--rw-r--r--   0 kage      (1000) kage      (1000)     2875 2024-03-26 05:18:50.608601 kBmc-2.3.5/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)     2457 2021-12-19 02:10:48.000000 kBmc-2.3.5/README.md
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-03-26 05:18:50.607601 kBmc-2.3.5/kBmc/
--rw-r--r--   0 kage      (1000) kage      (1000)   208052 2024-03-26 05:18:10.000000 kBmc-2.3.5/kBmc/__init__.py
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-03-26 05:18:50.607601 kBmc-2.3.5/kBmc.egg-info/
--rw-rw-r--   0 kage      (1000) kage      (1000)     2875 2024-03-26 05:18:50.000000 kBmc-2.3.5/kBmc.egg-info/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)      155 2024-03-26 05:18:50.000000 kBmc-2.3.5/kBmc.egg-info/SOURCES.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        1 2024-03-26 05:18:50.000000 kBmc-2.3.5/kBmc.egg-info/dependency_links.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        5 2024-03-26 05:18:50.000000 kBmc-2.3.5/kBmc.egg-info/top_level.txt
--rw-r--r--   0 kage      (1000) kage      (1000)       38 2024-03-26 05:18:50.608601 kBmc-2.3.5/setup.cfg
--rw-rw-r--   0 kage      (1000) kage      (1000)     1975 2021-12-17 05:56:02.000000 kBmc-2.3.5/setup.py
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-04 05:47:18.223357 kBmc-2.3.7/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-17 05:54:12.000000 kBmc-2.3.7/LICENSE
+-rw-r--r--   0 kage      (1000) kage      (1000)     2875 2024-04-04 05:47:18.223357 kBmc-2.3.7/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2457 2021-12-19 02:10:48.000000 kBmc-2.3.7/README.md
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-04 05:47:18.222357 kBmc-2.3.7/kBmc/
+-rw-r--r--   0 kage      (1000) kage      (1000)   208397 2024-04-04 05:46:06.000000 kBmc-2.3.7/kBmc/__init__.py
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-04 05:47:18.222357 kBmc-2.3.7/kBmc.egg-info/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2875 2024-04-04 05:47:18.000000 kBmc-2.3.7/kBmc.egg-info/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)      155 2024-04-04 05:47:18.000000 kBmc-2.3.7/kBmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        1 2024-04-04 05:47:18.000000 kBmc-2.3.7/kBmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        5 2024-04-04 05:47:18.000000 kBmc-2.3.7/kBmc.egg-info/top_level.txt
+-rw-r--r--   0 kage      (1000) kage      (1000)       38 2024-04-04 05:47:18.223357 kBmc-2.3.7/setup.cfg
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1975 2021-12-17 05:56:02.000000 kBmc-2.3.7/setup.py
```

### Comparing `kBmc-2.3.5/LICENSE` & `kBmc-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kBmc-2.3.5/PKG-INFO` & `kBmc-2.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kBmc
-Version: 2.3.5
+Version: 2.3.7
 Summary: Kage's Intelgent BMC handler
 Home-page: https://github.com/kagepark/kBmc
 Author: Kage Park
 License: MIT
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kBmc-2.3.5/README.md` & `kBmc-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `kBmc-2.3.5/kBmc/__init__.py` & `kBmc-2.3.7/kBmc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2845,17 +2845,23 @@
                                 persistent=True
                             elif 'Network:IBA' in Get(rf_boot_info.get('bios',{}).get('order',[]),0,default={}).get('name'):
                                 status='pxe'
                                 efi=False
                                 persistent=True
                         else:
                             efi=True if rf_boot_info.get('bios',{}).get('mode','') == 'UEFI' else False
-                            if 'Network:' in Get(rf_boot_info.get('bios',{}).get('order',[]),0,default={}).get('name'):
-                                status='pxe'
-                                persistent=True
+                            order_info=Get(rf_boot_info.get('bios',{}).get('order',[]),0,default={})
+                            if isinstance(order_info,dict):
+                                if 'Network:' in order_info.get('name'):
+                                    status='pxe'
+                                    persistent=True
+                            elif isinstance(order_info,str):
+                                if 'Network:' in order_info:
+                                    status='pxe'
+                                    persistent=True
                     else: # Follow instant overwriten Boot-Order
                         efi=True if rf_boot_info.get('order',{}).get('mode','') == 'UEFI' else False
                         status=rf_boot_info.get('order',{}).get('1','').lower()
                         persistent=True if rf_boot_info.get('order',{}).get('enable','') == 'Continuous' else False
                     return [status,efi,persistent]
                 #If received bios_cfg file
                 if bios_cfg:
```

### Comparing `kBmc-2.3.5/kBmc.egg-info/PKG-INFO` & `kBmc-2.3.7/kBmc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kBmc
-Version: 2.3.5
+Version: 2.3.7
 Summary: Kage's Intelgent BMC handler
 Home-page: https://github.com/kagepark/kBmc
 Author: Kage Park
 License: MIT
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kBmc-2.3.5/setup.py` & `kBmc-2.3.7/setup.py`

 * *Files identical despite different names*

