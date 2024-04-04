# Comparing `tmp/pyfdmss-0.0.3.tar.gz` & `tmp/pyfdmss-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, from Unix
+gzip compressed data, was "pyfdmss-0.0.5.tar", last modified: Thu Apr  4 17:10:00 2024, max compression
```

## Comparing `pyfdmss-0.0.3.tar` & `pyfdmss-0.0.5.tar`

### file list

```diff
@@ -1,73 +1,69 @@
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-02 21:04:20.000000 pyfdmss-0.0.3/
--rw-r--r--   0 ananev    (1000) ananev    (1000)       73 2024-04-02 19:18:56.000000 pyfdmss-0.0.3/README.md
--rw-r--r--   0 ananev    (1000) ananev    (1000)      744 2024-04-02 21:03:37.000000 pyfdmss-0.0.3/CMakeLists.txt
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-02 21:04:28.000000 pyfdmss-0.0.3/src/
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/pyfdmss/
--rw-r--r--   0 ananev    (1000) ananev    (1000)        0 2024-03-30 12:03:27.000000 pyfdmss-0.0.3/src/pyfdmss/__init__.py
--rw-r--r--   0 ananev    (1000) ananev    (1000)     4510 2024-04-02 20:00:57.000000 pyfdmss-0.0.3/src/pyfdmss/pyfdmss.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)       35 2024-04-02 20:34:40.000000 pyfdmss-0.0.3/src/CMakeLists.txt
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/fdmss_lib/
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/fdmss_lib/include/
--rw-r--r--   0 ananev    (1000) ananev    (1000)      269 2024-03-30 11:56:35.000000 pyfdmss-0.0.3/src/fdmss_lib/include/stdafx.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    64834 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/tinyxml.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      592 2024-03-30 10:20:01.000000 pyfdmss-0.0.3/src/fdmss_lib/include/Polynom.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      814 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/HorseBCOverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      447 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/Slau.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/MouseFuncY.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      478 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/BoundaryArea3d.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/MouseFuncX.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/MouseFuncZ.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     3918 2024-03-30 12:41:37.000000 pyfdmss-0.0.3/src/fdmss_lib/include/OverdozenPermsolver.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1081 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/PbcOverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/CrtFuncZ.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1119 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/CmdLineParameters.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      732 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/FbcOverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      460 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/StuffedVoxel.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     3097 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/Area3d.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/CrtFuncX.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2221 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/EnvCaseGenerator.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1032 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/Codegen.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/CrtFuncY.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1264 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/NfbcOverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      103 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/AccuracyOrder.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1086 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/InputParameters.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1278 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/PeriodicArea3d.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     8198 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/tinystr.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1685 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/OverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1214 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/include/FreeArea3d.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      816 2024-04-02 19:57:29.000000 pyfdmss-0.0.3/src/fdmss_lib/CMakeLists.txt
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/fdmss_lib/src/
--rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/MouseFuncY.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      298 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/stdafx.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/MouseFuncX.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/CrtFuncY.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     8258 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/PbcOverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2809 2024-03-30 10:24:05.000000 pyfdmss-0.0.3/src/fdmss_lib/src/Polynom.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     5592 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/FbcOverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      756 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/EnvCaseGenerator.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    63641 2024-03-30 12:41:45.000000 pyfdmss-0.0.3/src/fdmss_lib/src/OverdozenPermsolver.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      786 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/StuffedVoxel.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     8407 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/HorseBCOverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    37621 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/tinyxml.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     4168 2024-03-30 12:02:00.000000 pyfdmss-0.0.3/src/fdmss_lib/src/Slau.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    37242 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/tinyxmlparser.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    10371 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/OverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/CrtFuncX.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2507 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/tinystr.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     3823 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/InputParameters.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    10470 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/NfbcOverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    25995 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/Codegen.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/MouseFuncZ.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/CrtFuncZ.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1791 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/tinyxmlerror.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      329 2024-03-30 09:57:44.000000 pyfdmss-0.0.3/src/fdmss_lib/src/AntiMain.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)        0 2024-03-30 12:03:27.000000 pyfdmss-0.0.3/src/fdmss_lib/__init__.py
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/pyfdmss.egg-info/
--rw-r--r--   0 ananev    (1000) ananev    (1000)       18 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/pyfdmss.egg-info/top_level.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)        1 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/pyfdmss.egg-info/dependency_links.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)      645 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/pyfdmss.egg-info/PKG-INFO
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2129 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/src/pyfdmss.egg-info/SOURCES.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2241 2024-04-02 21:03:32.000000 pyfdmss-0.0.3/setup.py
--rw-r--r--   0 ananev    (1000) ananev    (1000)       38 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/setup.cfg
--rw-r--r--   0 ananev    (1000) ananev    (1000)      645 2024-04-02 21:03:54.000000 pyfdmss-0.0.3/PKG-INFO
--rw-r--r--   0 ananev    (1000) ananev    (1000)    35821 2023-10-30 16:40:18.000000 pyfdmss-0.0.3/LICENSE.txt
+drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    35821 2023-10-30 16:40:18.000000 pyfdmss-0.0.5/LICENSE.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      611 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/PKG-INFO
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       73 2024-03-30 10:52:38.000000 pyfdmss-0.0.5/README.md
+drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/pyfdmss.egg-info/
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      611 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/PKG-INFO
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1424 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/SOURCES.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)        1 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/dependency_links.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       34 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/entry_points.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)        9 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/requires.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       17 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/top_level.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       38 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/setup.cfg
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     2273 2024-04-04 17:08:39.000000 pyfdmss-0.0.5/setup.py
+drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/src/
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      103 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/AccuracyOrder.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     3097 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/Area3d.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      478 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/BoundaryArea3d.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1119 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CmdLineParameters.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    25995 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/Codegen.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1032 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/Codegen.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncX.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncX.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncY.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncY.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncZ.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncZ.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      756 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/EnvCaseGenerator.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     2221 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/EnvCaseGenerator.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     5592 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/FbcOverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      732 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/FbcOverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1214 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/FreeArea3d.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     8407 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/HorseBCOverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      814 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/HorseBCOverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     3823 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/InputParameters.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1086 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/InputParameters.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncX.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncX.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncY.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncY.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncZ.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncZ.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    10470 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/NfbcOverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1264 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/NfbcOverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    10371 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/OverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1685 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/OverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    63641 2024-03-30 12:41:45.000000 pyfdmss-0.0.5/src/OverdozenPermsolver.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     3918 2024-03-30 12:41:37.000000 pyfdmss-0.0.5/src/OverdozenPermsolver.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     8258 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/PbcOverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1081 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/PbcOverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1278 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/PeriodicArea3d.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     2809 2024-03-30 10:24:05.000000 pyfdmss-0.0.5/src/Polynom.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      592 2024-03-30 10:20:01.000000 pyfdmss-0.0.5/src/Polynom.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     4168 2024-03-30 12:02:00.000000 pyfdmss-0.0.5/src/Slau.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      447 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/Slau.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      786 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/StuffedVoxel.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      460 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/StuffedVoxel.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)        0 2024-04-04 16:41:42.000000 pyfdmss-0.0.5/src/__init__.py
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      342 2024-04-04 17:04:10.000000 pyfdmss-0.0.5/src/main.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      298 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/stdafx.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      269 2024-03-30 11:56:35.000000 pyfdmss-0.0.5/src/stdafx.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      178 2024-04-04 15:13:08.000000 pyfdmss-0.0.5/src/testmodule.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       45 2024-04-04 15:10:11.000000 pyfdmss-0.0.5/src/testmodule.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     2507 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinystr.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     8198 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinystr.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    37621 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinyxml.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    64834 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinyxml.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1791 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinyxmlerror.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    37242 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinyxmlparser.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     3306 2024-04-04 16:00:54.000000 pyfdmss-0.0.5/src/wrapper.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/tinyxml.h` & `pyfdmss-0.0.5/src/tinyxml.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/Polynom.h` & `pyfdmss-0.0.5/src/Polynom.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/HorseBCOverdozenMicroperm.h` & `pyfdmss-0.0.5/src/HorseBCOverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/MouseFuncY.h` & `pyfdmss-0.0.5/src/MouseFuncY.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/MouseFuncX.h` & `pyfdmss-0.0.5/src/MouseFuncX.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/MouseFuncZ.h` & `pyfdmss-0.0.5/src/MouseFuncZ.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/OverdozenPermsolver.h` & `pyfdmss-0.0.5/src/OverdozenPermsolver.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/PbcOverdozenMicroperm.h` & `pyfdmss-0.0.5/src/PbcOverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/CrtFuncZ.h` & `pyfdmss-0.0.5/src/CrtFuncZ.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/CmdLineParameters.h` & `pyfdmss-0.0.5/src/CmdLineParameters.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/FbcOverdozenMicroperm.h` & `pyfdmss-0.0.5/src/FbcOverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/Area3d.h` & `pyfdmss-0.0.5/src/Area3d.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/CrtFuncX.h` & `pyfdmss-0.0.5/src/CrtFuncX.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/EnvCaseGenerator.h` & `pyfdmss-0.0.5/src/EnvCaseGenerator.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/Codegen.h` & `pyfdmss-0.0.5/src/Codegen.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/CrtFuncY.h` & `pyfdmss-0.0.5/src/CrtFuncY.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/NfbcOverdozenMicroperm.h` & `pyfdmss-0.0.5/src/NfbcOverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/InputParameters.h` & `pyfdmss-0.0.5/src/InputParameters.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/PeriodicArea3d.h` & `pyfdmss-0.0.5/src/PeriodicArea3d.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/tinystr.h` & `pyfdmss-0.0.5/src/tinystr.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/OverdozenMicroperm.h` & `pyfdmss-0.0.5/src/OverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/include/FreeArea3d.h` & `pyfdmss-0.0.5/src/FreeArea3d.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/MouseFuncY.cpp` & `pyfdmss-0.0.5/src/MouseFuncY.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/MouseFuncX.cpp` & `pyfdmss-0.0.5/src/MouseFuncX.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/CrtFuncY.cpp` & `pyfdmss-0.0.5/src/CrtFuncY.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/PbcOverdozenMicroperm.cpp` & `pyfdmss-0.0.5/src/PbcOverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/Polynom.cpp` & `pyfdmss-0.0.5/src/Polynom.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/FbcOverdozenMicroperm.cpp` & `pyfdmss-0.0.5/src/FbcOverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/EnvCaseGenerator.cpp` & `pyfdmss-0.0.5/src/EnvCaseGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/OverdozenPermsolver.cpp` & `pyfdmss-0.0.5/src/OverdozenPermsolver.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/StuffedVoxel.cpp` & `pyfdmss-0.0.5/src/StuffedVoxel.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/HorseBCOverdozenMicroperm.cpp` & `pyfdmss-0.0.5/src/HorseBCOverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/tinyxml.cpp` & `pyfdmss-0.0.5/src/tinyxml.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/Slau.cpp` & `pyfdmss-0.0.5/src/Slau.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/tinyxmlparser.cpp` & `pyfdmss-0.0.5/src/tinyxmlparser.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/OverdozenMicroperm.cpp` & `pyfdmss-0.0.5/src/OverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/CrtFuncX.cpp` & `pyfdmss-0.0.5/src/CrtFuncX.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/tinystr.cpp` & `pyfdmss-0.0.5/src/tinystr.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/InputParameters.cpp` & `pyfdmss-0.0.5/src/InputParameters.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/NfbcOverdozenMicroperm.cpp` & `pyfdmss-0.0.5/src/NfbcOverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/Codegen.cpp` & `pyfdmss-0.0.5/src/Codegen.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/MouseFuncZ.cpp` & `pyfdmss-0.0.5/src/MouseFuncZ.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/CrtFuncZ.cpp` & `pyfdmss-0.0.5/src/CrtFuncZ.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/fdmss_lib/src/tinyxmlerror.cpp` & `pyfdmss-0.0.5/src/tinyxmlerror.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.3/src/pyfdmss.egg-info/PKG-INFO` & `pyfdmss-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 Metadata-Version: 2.1
 Name: pyfdmss
-Version: 0.0.3
-Summary: todo
+Version: 0.0.5
+Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev, Andrey Zubov
 Author-email: andrey.ananev@phystech.edu
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
+Requires: pybind11
 License-File: LICENSE.txt
 
-# PyFDMSS
-TODO
-....
-
-Authors:
-Moscow, 2024
-
-## Prerequisites
-
-
-
+UNKNOWN
```

### Comparing `pyfdmss-0.0.3/PKG-INFO` & `pyfdmss-0.0.5/pyfdmss.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 Metadata-Version: 2.1
 Name: pyfdmss
-Version: 0.0.3
-Summary: todo
+Version: 0.0.5
+Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev, Andrey Zubov
 Author-email: andrey.ananev@phystech.edu
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
+Requires: pybind11
 License-File: LICENSE.txt
 
-# PyFDMSS
-TODO
-....
-
-Authors:
-Moscow, 2024
-
-## Prerequisites
-
-
-
+UNKNOWN
```

### Comparing `pyfdmss-0.0.3/LICENSE.txt` & `pyfdmss-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

