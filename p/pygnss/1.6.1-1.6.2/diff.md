# Comparing `tmp/pygnss-1.6.1.tar.gz` & `tmp/pygnss-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygnss-1.6.1.tar", last modified: Tue Sep 22 08:37:21 2020, max compression
+gzip compressed data, was "dist/pygnss-1.6.2.tar", last modified: Tue Sep 22 08:40:02 2020, max compression
```

## Comparing `pygnss-1.6.1.tar` & `pygnss-1.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-22 08:37:21.373487 pygnss-1.6.1/
--rw-r--r--   0 root         (0) root         (0)     2248 2020-09-22 08:37:21.373487 pygnss-1.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1425 2020-09-22 08:36:48.000000 pygnss-1.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-22 08:37:21.373487 pygnss-1.6.1/pygnss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2248 2020-09-22 08:37:21.000000 pygnss-1.6.1/pygnss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2020-09-22 08:37:21.000000 pygnss-1.6.1/pygnss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-22 08:37:21.000000 pygnss-1.6.1/pygnss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2020-09-22 08:37:21.000000 pygnss-1.6.1/pygnss.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2020-09-22 08:37:21.000000 pygnss-1.6.1/pygnss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2020-09-22 08:37:21.000000 pygnss-1.6.1/pygnss.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-22 08:37:21.373487 pygnss-1.6.1/roktools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-14 12:33:20.000000 pygnss-1.6.1/roktools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2020-09-14 12:33:20.000000 pygnss-1.6.1/roktools/cl.py
--rw-rw-rw-   0 root         (0) root         (0)    21349 2020-09-14 12:33:20.000000 pygnss-1.6.1/roktools/geodetic.py
--rw-rw-rw-   0 root         (0) root         (0)     1479 2020-09-14 12:33:20.000000 pygnss-1.6.1/roktools/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3328 2020-09-14 12:33:20.000000 pygnss-1.6.1/roktools/rinex.py
--rwxrwxrwx   0 root         (0) root         (0)     1580 2020-09-14 12:33:20.000000 pygnss-1.6.1/roktools/tensorial.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2020-09-14 12:33:20.000000 pygnss-1.6.1/roktools/time.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2020-09-22 08:37:21.373487 pygnss-1.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1107 2020-09-22 08:36:48.000000 pygnss-1.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-22 08:40:02.164059 pygnss-1.6.2/
+-rw-r--r--   0 root         (0) root         (0)     2243 2020-09-22 08:40:02.164059 pygnss-1.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2020-09-22 08:39:52.000000 pygnss-1.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-22 08:40:02.164059 pygnss-1.6.2/pygnss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2243 2020-09-22 08:40:02.000000 pygnss-1.6.2/pygnss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2020-09-22 08:40:02.000000 pygnss-1.6.2/pygnss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-22 08:40:02.000000 pygnss-1.6.2/pygnss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2020-09-22 08:40:02.000000 pygnss-1.6.2/pygnss.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2020-09-22 08:40:02.000000 pygnss-1.6.2/pygnss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2020-09-22 08:40:02.000000 pygnss-1.6.2/pygnss.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-22 08:40:02.164059 pygnss-1.6.2/roktools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-14 12:29:41.000000 pygnss-1.6.2/roktools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2020-09-14 12:29:41.000000 pygnss-1.6.2/roktools/cl.py
+-rw-rw-rw-   0 root         (0) root         (0)    21349 2020-09-14 12:29:41.000000 pygnss-1.6.2/roktools/geodetic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2020-09-14 12:29:41.000000 pygnss-1.6.2/roktools/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3328 2020-09-14 12:29:41.000000 pygnss-1.6.2/roktools/rinex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1580 2020-09-14 12:29:41.000000 pygnss-1.6.2/roktools/tensorial.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2020-09-14 12:29:41.000000 pygnss-1.6.2/roktools/time.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2020-09-22 08:40:02.168058 pygnss-1.6.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2020-09-22 08:30:40.000000 pygnss-1.6.2/setup.py
```

### Comparing `pygnss-1.6.1/PKG-INFO` & `pygnss-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pygnss
-Version: 1.6.1
+Version: 1.6.2
 Summary: Set of tools used in internal GNSS Rokubun projects
 Home-page: https://www.rokubun.cat
 Author: Rokubun
 Author-email: info@rokubun.cat
 License: http://opensource.org/licenses/MIT
-Description: # pyrok-tools
+Description: # pygnss
         
         Python tools used in internal GNSS Rokubun projects. This repository contains the following modules:
         
         - `logger`, a module that extends basic Python logging
         - `geodetic`, to perform basic geodetic transformation (Cartesian to Geodetic,
           Cartesian to Local Tangential Plane, ...)
```

### Comparing `pygnss-1.6.1/README.md` & `pygnss-1.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pyrok-tools
+# pygnss
 
 Python tools used in internal GNSS Rokubun projects. This repository contains the following modules:
 
 - `logger`, a module that extends basic Python logging
 - `geodetic`, to perform basic geodetic transformation (Cartesian to Geodetic,
   Cartesian to Local Tangential Plane, ...)
```

### Comparing `pygnss-1.6.1/pygnss.egg-info/PKG-INFO` & `pygnss-1.6.2/pygnss.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pygnss
-Version: 1.6.1
+Version: 1.6.2
 Summary: Set of tools used in internal GNSS Rokubun projects
 Home-page: https://www.rokubun.cat
 Author: Rokubun
 Author-email: info@rokubun.cat
 License: http://opensource.org/licenses/MIT
-Description: # pyrok-tools
+Description: # pygnss
         
         Python tools used in internal GNSS Rokubun projects. This repository contains the following modules:
         
         - `logger`, a module that extends basic Python logging
         - `geodetic`, to perform basic geodetic transformation (Cartesian to Geodetic,
           Cartesian to Local Tangential Plane, ...)
```

### Comparing `pygnss-1.6.1/roktools/cl.py` & `pygnss-1.6.2/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `pygnss-1.6.1/roktools/geodetic.py` & `pygnss-1.6.2/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `pygnss-1.6.1/roktools/logger.py` & `pygnss-1.6.2/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `pygnss-1.6.1/roktools/rinex.py` & `pygnss-1.6.2/roktools/rinex.py`

 * *Files identical despite different names*

### Comparing `pygnss-1.6.1/roktools/tensorial.py` & `pygnss-1.6.2/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `pygnss-1.6.1/setup.py` & `pygnss-1.6.2/setup.py`

 * *Files identical despite different names*

