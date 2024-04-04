# Comparing `tmp/kkpyutil-1.8.0.tar.gz` & `tmp/kkpyutil-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyutil-1.8.0.tar", max compression
+gzip compressed data, was "kkpyutil-1.9.0.tar", max compression
```

## Comparing `kkpyutil-1.8.0.tar` & `kkpyutil-1.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2021-11-28 23:18:46.338722 kkpyutil-1.8.0/LICENSE
--rw-r--r--   0        0        0      302 2023-09-30 22:36:57.878309 kkpyutil-1.8.0/README.md
--rwxr-xr-x   0        0        0    92572 2023-10-13 19:22:49.196032 kkpyutil-1.8.0/kkpyutil.py
--rw-r--r--   0        0        0      446 2023-09-23 22:00:57.688828 kkpyutil-1.8.0/kkpyutil_helper/windows/kkttssave.ps1
--rw-r--r--   0        0        0      305 2023-09-23 22:00:57.689100 kkpyutil-1.8.0/kkpyutil_helper/windows/kkttsspeak.ps1
--rw-r--r--   0        0        0      780 2023-10-13 19:24:25.278874 kkpyutil-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 kkpyutil-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-11-28 23:18:46.338722 kkpyutil-1.9.0/LICENSE
+-rw-r--r--   0        0        0      302 2023-09-30 22:36:57.878309 kkpyutil-1.9.0/README.md
+-rwxr-xr-x   0        0        0    92704 2023-10-14 00:30:55.141965 kkpyutil-1.9.0/kkpyutil.py
+-rw-r--r--   0        0        0      446 2023-09-23 22:00:57.688828 kkpyutil-1.9.0/kkpyutil_helper/windows/kkttssave.ps1
+-rw-r--r--   0        0        0      305 2023-09-23 22:00:57.689100 kkpyutil-1.9.0/kkpyutil_helper/windows/kkttsspeak.ps1
+-rw-r--r--   0        0        0      780 2023-10-14 01:04:24.031953 kkpyutil-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 kkpyutil-1.9.0/PKG-INFO
```

### Comparing `kkpyutil-1.8.0/LICENSE` & `kkpyutil-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyutil-1.8.0/kkpyutil.py` & `kkpyutil-1.9.0/kkpyutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -5774,13 +5774,21 @@
 000168d0: 6179 732c 207b 686f 7572 737d 2068 6f75  ays, {hours} hou
 000168e0: 7273 2c20 7b6d 696e 7574 6573 7d20 6d69  rs, {minutes} mi
 000168f0: 6e75 7465 732c 207b 7365 6373 7d20 7365  nutes, {secs} se
 00016900: 636f 6e64 732c 2061 6e64 207b 6475 7261  conds, and {dura
 00016910: 7469 6f6e 2e6d 6963 726f 7365 636f 6e64  tion.microsecond
 00016920: 732f 2f31 3030 307d 206d 696c 6c69 7365  s//1000} millise
 00016930: 636f 6e64 7322 0a20 2020 2072 6574 7572  conds".    retur
-00016940: 6e20 6475 7261 7469 6f6e 0a0a 0a0a 6465  n duration....de
-00016950: 6620 5f74 6573 7428 293a 0a20 2020 2070  f _test():.    p
-00016960: 7269 6e74 2873 6179 2827 6865 6c6c 6f27  rint(say('hello'
-00016970: 2929 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  ))...if __name__
-00016980: 203d 3d20 275f 5f6d 6169 6e5f 5f27 3a0a   == '__main__':.
-00016990: 2020 2020 5f74 6573 7428 290a                _test().
+00016940: 6e20 6475 7261 7469 6f6e 0a0a 0a64 6566  n duration...def
+00016950: 2073 6166 655f 6765 745f 656c 656d 656e   safe_get_elemen
+00016960: 7428 6d79 6c69 7374 2c20 6964 782c 2064  t(mylist, idx, d
+00016970: 6566 6175 6c74 3d4e 6f6e 6529 3a0a 2020  efault=None):.  
+00016980: 2020 7472 793a 0a20 2020 2020 2020 2072    try:.        r
+00016990: 6574 7572 6e20 6d79 6c69 7374 5b69 6478  eturn mylist[idx
+000169a0: 5d0a 2020 2020 6578 6365 7074 2049 6e64  ].    except Ind
+000169b0: 6578 4572 726f 723a 0a20 2020 2020 2020  exError:.       
+000169c0: 2072 6574 7572 6e20 6465 6661 756c 740a   return default.
+000169d0: 0a0a 6465 6620 5f74 6573 7428 293a 0a20  ..def _test():. 
+000169e0: 2020 2070 7269 6e74 2873 6179 2827 6865     print(say('he
+000169f0: 6c6c 6f27 2929 0a0a 0a69 6620 5f5f 6e61  llo'))...if __na
+00016a00: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+00016a10: 5f27 3a0a 2020 2020 5f74 6573 7428 290a  _':.    _test().
```

### Comparing `kkpyutil-1.8.0/pyproject.toml` & `kkpyutil-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kkpyutil"
-version = "1.8.0"
+version = "1.9.0"
 description = "Building blocks for sysadmin and DevOps"
 authors = ["Beinan Li <li.beinan@gmail.com>"]
 maintainers = ["Beinan Li <li.beinan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/kakyoism/kkpyutil/"
```

### Comparing `kkpyutil-1.8.0/PKG-INFO` & `kkpyutil-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkpyutil
-Version: 1.8.0
+Version: 1.9.0
 Summary: Building blocks for sysadmin and DevOps
 Home-page: https://github.com/kakyoism/kkpyutil/
 License: MIT
 Keywords: utility,logging,systems
 Author: Beinan Li
 Author-email: li.beinan@gmail.com
 Maintainer: Beinan Li
```

