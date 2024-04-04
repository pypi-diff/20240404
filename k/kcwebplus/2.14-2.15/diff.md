# Comparing `tmp/kcwebplus-2.14.tar.gz` & `tmp/kcwebplus-2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-2.14.tar", last modified: Wed Jan 17 12:49:52 2024, max compression
+gzip compressed data, was "dist\kcwebplus-2.15.tar", last modified: Thu Apr  4 03:20:17 2024, max compression
```

## Comparing `kcwebplus-2.14.tar` & `kcwebplus-2.15.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/common/
--rw-rw-rw-   0        0        0       41 2024-01-16 11:07:08.000000 kcwebplus-2.14/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-01-16 10:20:35.000000 kcwebplus-2.14/kcwebplus/common/model.py
--rw-rw-rw-   0        0        0    18682 2024-01-16 11:00:52.000000 kcwebplus-2.14/kcwebplus/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/config/
--rw-rw-rw-   0        0        0      645 2024-01-17 12:48:41.000000 kcwebplus-2.14/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/index/
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       30 2024-01-16 10:33:28.000000 kcwebplus-2.14/kcwebplus/index/common/autoload.py
--rw-rw-rw-   0        0        0       48 2022-03-31 12:40:32.000000 kcwebplus-2.14/kcwebplus/index/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/index/controller/
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/index/controller/index/
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       36 2024-01-16 10:34:46.000000 kcwebplus-2.14/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2022-03-31 12:40:32.000000 kcwebplus-2.14/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0       45 2022-03-31 12:40:32.000000 kcwebplus-2.14/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-01-16 10:29:29.000000 kcwebplus-2.14/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-01-14 06:19:18.000000 kcwebplus-2.14/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-01-14 06:19:21.000000 kcwebplus-2.14/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0       19 2022-03-31 12:40:32.000000 kcwebplus-2.14/kcwebplus/index/controller/index/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-08 13:32:00.000000 kcwebplus-2.14/kcwebplus/index/controller/__init__.py
--rw-rw-rw-   0        0        0       24 2022-03-31 12:40:32.000000 kcwebplus-2.14/kcwebplus/index/__init__.py
--rw-rw-rw-   0        0        0    12401 2024-01-17 11:54:05.000000 kcwebplus-2.14/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1048 2024-01-16 15:35:08.000000 kcwebplus-2.14/kcwebplus/server
--rw-rw-rw-   0        0        0      334 2024-01-16 15:36:01.000000 kcwebplus-2.14/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0        1 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      312 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0      883 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      450 2024-01-17 12:49:52.000000 kcwebplus-2.14/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-03-31 12:40:32.000000 kcwebplus-2.14/LICENSE
--rw-rw-rw-   0        0        0      312 2024-01-17 12:49:52.000000 kcwebplus-2.14/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2024-01-16 14:23:04.000000 kcwebplus-2.14/README.md
--rw-rw-rw-   0        0        0       42 2024-01-17 12:49:52.000000 kcwebplus-2.14/setup.cfg
--rw-rw-rw-   0        0        0     2439 2024-01-17 12:48:57.000000 kcwebplus-2.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/common/
+-rw-rw-rw-   0        0        0       41 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/common/model.py
+-rw-rw-rw-   0        0        0    18682 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/config/
+-rw-rw-rw-   0        0        0      645 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       30 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/common/autoload.py
+-rw-rw-rw-   0        0        0       48 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/index/
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       36 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0       45 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0       19 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/__init__.py
+-rw-rw-rw-   0        0        0       24 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/__init__.py
+-rw-rw-rw-   0        0        0    12401 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1014 2024-04-04 03:15:45.000000 kcwebplus-2.15/kcwebplus/server
+-rw-rw-rw-   0        0        0      334 2024-04-04 03:14:17.000000 kcwebplus-2.15/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      312 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      883 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      450 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-04 02:31:55.000000 kcwebplus-2.15/LICENSE
+-rw-rw-rw-   0        0        0      312 2024-04-04 03:20:17.000000 kcwebplus-2.15/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2024-04-04 02:31:55.000000 kcwebplus-2.15/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 03:20:17.000000 kcwebplus-2.15/setup.cfg
+-rw-rw-rw-   0        0        0     2439 2024-04-04 03:20:09.000000 kcwebplus-2.15/setup.py
```

### Comparing `kcwebplus-2.14/kcwebplus/common/model.py` & `kcwebplus-2.15/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/kcwebplus/common/__init__.py` & `kcwebplus-2.15/kcwebplus/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/kcwebplus/config/__init__.py` & `kcwebplus-2.15/kcwebplus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/kcwebplus/index/controller/index/index.py` & `kcwebplus-2.15/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/kcwebplus/kcwebplus.py` & `kcwebplus-2.15/kcwebplus/kcwebplus.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-2.15/kcwebplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/LICENSE` & `kcwebplus-2.15/LICENSE`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/README.md` & `kcwebplus-2.15/README.md`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.14/setup.py` & `kcwebplus-2.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 00000240: 726e 2063 6f6e 0d0a 636f 6e66 6b63 773d  rn con..confkcw=
 00000250: 7b7d 0d0a 636f 6e66 6b63 775b 276e 616d  {}..confkcw['nam
 00000260: 6527 5d3d 276b 6377 6562 706c 7573 2720  e']='kcwebplus' 
 00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000280: 2020 2020 2020 2020 2020 2020 23e9 a1b9              #...
 00000290: e79b aee7 9a84 e590 8de7 a7b0 200d 0a63  ............ ..c
 000002a0: 6f6e 666b 6377 5b27 7665 7273 696f 6e27  onfkcw['version'
-000002b0: 5d3d 2732 2e31 3427 0909 0909 0909 0923  ]='2.14'.......#
+000002b0: 5d3d 2732 2e31 3527 0909 0909 0909 0923  ]='2.15'.......#
 000002c0: e9a1 b9e7 9bae e789 88e6 9cac 0d0a 636f  ..............co
 000002d0: 6e66 6b63 775b 2764 6573 6372 6970 7469  nfkcw['descripti
 000002e0: 6f6e 275d 3d27 2720 2020 2020 2020 23e9  on']=''       #.
 000002f0: a1b9 e79b aee7 9a84 e7ae 80e5 8d95 e68f  ................
 00000300: 8fe8 bfb0 0d0a 636f 6e66 6b63 775b 276c  ......confkcw['l
 00000310: 6f6e 675f 6465 7363 7269 7074 696f 6e27  ong_description'
 00000320: 5d3d 2222 2020 2020 2023 e9a1 b9e7 9bae  ]=""     #......
@@ -129,15 +129,15 @@
 00000800: 6377 5b27 7572 6c27 5d2c 0d0a 2020 2020  cw['url'],..    
 00000810: 7061 636b 6167 6573 203d 2020 622c 0d0a  packages =  b,..
 00000820: 2020 2020 2320 6461 7461 5f66 696c 6573      # data_files
 00000830: 3d5b 2827 5363 7269 7074 7327 2c20 5b27  =[('Scripts', ['
 00000840: 6b63 7765 6270 6c75 732f 6269 6e2f 6b63  kcwebplus/bin/kc
 00000850: 772e 6578 6527 5d29 5d2c 0d0a 2020 2020  w.exe'])],..    
 00000860: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000870: 203d 205b 276b 6377 6562 3e3d 352e 3234   = ['kcweb>=5.24
+00000870: 203d 205b 276b 6377 6562 3e3d 352e 3236   = ['kcweb>=5.26
 00000880: 275d 2c20 23e7 acac e4b8 89e6 96b9 e58c  '], #...........
 00000890: 850d 0a20 2020 2070 6163 6b61 6765 5f64  ...    package_d
 000008a0: 6174 6120 3d20 7b0d 0a20 2020 2020 2020  ata = {..       
 000008b0: 2027 273a 205b 272a 2e68 746d 6c27 2c20   '': ['*.html', 
 000008c0: 272a 2e6a 7327 2c27 2a2e 6373 7327 2c27  '*.js','*.css','
 000008d0: 2a2e 6a70 6727 2c27 2a2e 706e 6727 2c27  *.jpg','*.png','
 000008e0: 2a2e 6769 6627 2c27 7365 7276 6572 272c  *.gif','server',
```

