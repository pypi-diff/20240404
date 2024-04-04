# Comparing `tmp/MetaDefender_api-1.0.4.tar.gz` & `tmp/MetaDefender_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetaDefender_api-1.0.4.tar", last modified: Thu Apr  4 17:22:48 2024, max compression
+gzip compressed data, was "MetaDefender_api-1.0.5.tar", last modified: Thu Apr  4 18:10:46 2024, max compression
```

## Comparing `MetaDefender_api-1.0.4.tar` & `MetaDefender_api-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 17:22:48.468187 MetaDefender_api-1.0.4/
--rw-rw-rw-   0        0        0    35108 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       28 2024-04-04 17:20:46.000000 MetaDefender_api-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      988 2024-04-04 17:22:48.467688 MetaDefender_api-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-04-04 17:21:42.000000 MetaDefender_api-1.0.4/README.md
--rw-rw-rw-   0        0        0      101 2024-04-04 17:11:54.000000 MetaDefender_api-1.0.4/__init__.py
--rw-rw-rw-   0        0        0      108 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      581 2024-04-04 17:22:48.469187 MetaDefender_api-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 17:22:48.460688 MetaDefender_api-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 17:22:48.466687 MetaDefender_api-1.0.4/src/MetaDefender_api.egg-info/
--rw-rw-rw-   0        0        0      988 2024-04-04 17:22:48.000000 MetaDefender_api-1.0.4/src/MetaDefender_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-04 17:22:48.000000 MetaDefender_api-1.0.4/src/MetaDefender_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 17:22:48.000000 MetaDefender_api-1.0.4/src/MetaDefender_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 17:22:48.000000 MetaDefender_api-1.0.4/src/MetaDefender_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-04-04 17:01:57.000000 MetaDefender_api-1.0.4/src/__init__.py
--rw-rw-rw-   0        0        0     5038 2024-04-04 15:56:32.000000 MetaDefender_api-1.0.4/src/main.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:10:46.571944 MetaDefender_api-1.0.5/
+-rw-rw-rw-   0        0        0    35108 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       28 2024-04-04 17:20:46.000000 MetaDefender_api-1.0.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-04-04 18:10:46.562742 MetaDefender_api-1.0.5/MetaDefender/
+-rw-rw-rw-   0        0        0        0 2024-04-04 17:01:57.000000 MetaDefender_api-1.0.5/MetaDefender/__init__.py
+-rw-rw-rw-   0        0        0     5038 2024-04-04 15:56:32.000000 MetaDefender_api-1.0.5/MetaDefender/api.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:10:46.571438 MetaDefender_api-1.0.5/MetaDefender_api.egg-info/
+-rw-rw-rw-   0        0        0      988 2024-04-04 18:10:46.000000 MetaDefender_api-1.0.5/MetaDefender_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-04 18:10:46.000000 MetaDefender_api-1.0.5/MetaDefender_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 18:10:46.000000 MetaDefender_api-1.0.5/MetaDefender_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 18:10:46.000000 MetaDefender_api-1.0.5/MetaDefender_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      988 2024-04-04 18:10:46.571944 MetaDefender_api-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-04-04 18:03:55.000000 MetaDefender_api-1.0.5/README.md
+-rw-rw-rw-   0        0        0      101 2024-04-04 17:11:54.000000 MetaDefender_api-1.0.5/__init__.py
+-rw-rw-rw-   0        0        0      108 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      542 2024-04-04 18:10:46.573955 MetaDefender_api-1.0.5/setup.cfg
```

### Comparing `MetaDefender_api-1.0.4/LICENSE` & `MetaDefender_api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MetaDefender_api-1.0.4/PKG-INFO` & `MetaDefender_api-1.0.5/MetaDefender_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: MetaDefender_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple MetaDefender Api wrapper
 Home-page: https://github.com/cookie0o
 Author: cookie0_o
 Author-email: raphael.contact@zohomail.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align=center>
   
-  # MetaDefender_api v1.0.4
+  # MetaDefender_api v1.0.5
   
   **A simple MetaDefender Api wrapper**
 </div>
 
 ## +Info and usage:
 go to the wiki on the Github Page [here](https://github.com/sch-raphael/MetaDefender-api/wiki).
```

### Comparing `MetaDefender_api-1.0.4/README.md` & `MetaDefender_api-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align=center>
   
-  # MetaDefender_api v1.0.4
+  # MetaDefender_api v1.0.5
   
   **A simple MetaDefender Api wrapper**
 </div>
 
 ## +Info and usage:
 go to the wiki on the Github Page [here](https://github.com/sch-raphael/MetaDefender-api/wiki).
```

### Comparing `MetaDefender_api-1.0.4/setup.cfg` & `MetaDefender_api-1.0.5/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204d 6574 6144 6566 656e 6465 725f   = MetaDefender_
 00000020: 6170 690d 0a76 6572 7369 6f6e 203d 2031  api..version = 1
-00000030: 2e30 2e34 0d0a 6175 7468 6f72 203d 2063  .0.4..author = c
+00000030: 2e30 2e35 0d0a 6175 7468 6f72 203d 2063  .0.5..author = c
 00000040: 6f6f 6b69 6530 5f6f 0d0a 6175 7468 6f72  ookie0_o..author
 00000050: 5f65 6d61 696c 203d 2072 6170 6861 656c  _email = raphael
 00000060: 2e63 6f6e 7461 6374 407a 6f68 6f6d 6169  .contact@zohomai
 00000070: 6c2e 6575 0d0a 7572 6c20 3d20 6874 7470  l.eu..url = http
 00000080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
 00000090: 6f6f 6b69 6530 6f0d 0a64 6573 6372 6970  ookie0o..descrip
 000000a0: 7469 6f6e 203d 2041 2073 696d 706c 6520  tion = A simple 
@@ -22,16 +22,13 @@
 00000150: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
 00000160: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
 00000170: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
 00000180: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 00000190: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
 000001a0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
 000001b0: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-000001c0: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-000001d0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-000001e0: 6571 7569 7265 7320 3d20 3e3d 332e 370d  equires = >=3.7.
-000001f0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000200: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-00000210: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
-00000220: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000230: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000240: 300d 0a0d 0a                             0....
+000001c0: 202e 0d0a 7061 636b 6167 6573 203d 200d   ...packages = .
+000001d0: 0a09 6669 6e64 3a0d 0a70 7974 686f 6e5f  ..find:..python_
+000001e0: 7265 7175 6972 6573 203d 203e 3d33 2e37  requires = >=3.7
+000001f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000200: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000210: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `MetaDefender_api-1.0.4/src/MetaDefender_api.egg-info/PKG-INFO` & `MetaDefender_api-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: MetaDefender_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple MetaDefender Api wrapper
 Home-page: https://github.com/cookie0o
 Author: cookie0_o
 Author-email: raphael.contact@zohomail.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align=center>
   
-  # MetaDefender_api v1.0.4
+  # MetaDefender_api v1.0.5
   
   **A simple MetaDefender Api wrapper**
 </div>
 
 ## +Info and usage:
 go to the wiki on the Github Page [here](https://github.com/sch-raphael/MetaDefender-api/wiki).
```

### Comparing `MetaDefender_api-1.0.4/src/main.py` & `MetaDefender_api-1.0.5/MetaDefender/api.py`

 * *Files identical despite different names*

