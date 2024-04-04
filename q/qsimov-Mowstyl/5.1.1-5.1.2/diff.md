# Comparing `tmp/qsimov-Mowstyl-5.1.1.tar.gz` & `tmp/qsimov-Mowstyl-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsimov-Mowstyl-5.1.1.tar", last modified: Wed May 10 20:45:09 2023, max compression
+gzip compressed data, was "qsimov-Mowstyl-5.1.2.tar", last modified: Thu Apr  4 20:56:43 2024, max compression
```

## Comparing `qsimov-Mowstyl-5.1.1.tar` & `qsimov-Mowstyl-5.1.2.tar`

### file list

```diff
@@ -1,44 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 20:45:09.323584 qsimov-Mowstyl-5.1.1/
--rw-rw-rw-   0        0        0     1111 2020-08-24 08:47:52.000000 qsimov-Mowstyl-5.1.1/LICENSE
--rw-rw-rw-   0        0        0      855 2023-05-10 20:45:09.323584 qsimov-Mowstyl-5.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3786 2023-02-17 14:46:14.000000 qsimov-Mowstyl-5.1.1/README.md
--rw-rw-rw-   0        0        0      110 2021-07-23 13:21:51.000000 qsimov-Mowstyl-5.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-10 20:45:08.985003 qsimov-Mowstyl-5.1.1/qsimov/
--rw-rw-rw-   0        0        0      455 2023-04-22 14:30:17.000000 qsimov-Mowstyl-5.1.1/qsimov/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:45:08.989004 qsimov-Mowstyl-5.1.1/qsimov/connectors/
--rw-rw-rw-   0        0        0        0 2021-11-07 14:13:55.000000 qsimov-Mowstyl-5.1.1/qsimov/connectors/__init__.py
--rw-rw-rw-   0        0        0      897 2022-05-24 09:37:52.000000 qsimov-Mowstyl-5.1.1/qsimov/connectors/drewom.py
--rw-rw-rw-   0        0        0      226 2021-02-27 01:28:39.000000 qsimov-Mowstyl-5.1.1/qsimov/connectors/forestapi.py
--rw-rw-rw-   0        0        0    11118 2023-05-10 20:39:58.000000 qsimov-Mowstyl-5.1.1/qsimov/connectors/parser.py
--rw-rw-rw-   0        0        0     8107 2022-05-21 19:50:42.000000 qsimov-Mowstyl-5.1.1/qsimov/connectors/qsimovapi.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:45:08.990004 qsimov-Mowstyl-5.1.1/qsimov/cores/
--rw-rw-rw-   0        0        0        0 2021-11-07 14:13:55.000000 qsimov-Mowstyl-5.1.1/qsimov/cores/__init__.py
--rw-rw-rw-   0        0        0     5852 2023-04-22 14:33:19.000000 qsimov-Mowstyl-5.1.1/qsimov/cores/bdoki.py
--rw-rw-rw-   0        0        0     3616 2022-04-19 11:09:36.000000 qsimov-Mowstyl-5.1.1/qsimov/qsimov.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:45:08.992003 qsimov-Mowstyl-5.1.1/qsimov/samples/
--rw-rw-rw-   0        0        0        0 2021-11-07 14:14:03.000000 qsimov-Mowstyl-5.1.1/qsimov/samples/__init__.py
--rw-rw-rw-   0        0        0     2631 2022-05-21 18:59:40.000000 qsimov-Mowstyl-5.1.1/qsimov/samples/djcircuit.py
--rw-rw-rw-   0        0        0      736 2022-05-24 22:21:45.000000 qsimov-Mowstyl-5.1.1/qsimov/samples/fourier.py
--rw-rw-rw-   0        0        0     3986 2021-11-05 11:42:46.000000 qsimov-Mowstyl-5.1.1/qsimov/samples/state_gate.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:45:09.000003 qsimov-Mowstyl-5.1.1/qsimov/structures/
--rw-rw-rw-   0        0        0        0 2021-11-07 14:14:09.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/__init__.py
--rw-rw-rw-   0        0        0    12917 2021-11-08 00:37:00.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/funmatrix.py
--rw-rw-rw-   0        0        0      126 2022-02-10 11:19:15.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/qbase.py
--rw-rw-rw-   0        0        0     7264 2023-05-10 19:59:59.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/qcircuit.py
--rw-rw-rw-   0        0        0      527 2022-05-22 18:40:22.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/qdesign.py
--rw-rw-rw-   0        0        0     6420 2023-05-10 20:01:20.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/qgate.py
--rw-rw-rw-   0        0        0    15880 2023-05-10 19:57:04.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/qregistry.py
--rw-rw-rw-   0        0        0     6829 2023-05-10 19:24:28.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/qstructure.py
--rw-rw-rw-   0        0        0    18742 2023-05-10 20:08:40.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/qsystem.py
--rw-rw-rw-   0        0        0     5160 2023-05-10 20:27:49.000000 qsimov-Mowstyl-5.1.1/qsimov/structures/simple_gate.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:45:09.002005 qsimov-Mowstyl-5.1.1/qsimov/utils/
--rw-rw-rw-   0        0        0        0 2022-02-10 11:50:33.000000 qsimov-Mowstyl-5.1.1/qsimov/utils/__init__.py
--rw-rw-rw-   0        0        0     5577 2022-02-10 15:44:35.000000 qsimov-Mowstyl-5.1.1/qsimov/utils/bloch.py
-drwxrwxrwx   0        0        0        0 2023-05-10 20:45:09.238351 qsimov-Mowstyl-5.1.1/qsimov_Mowstyl.egg-info/
--rw-rw-rw-   0        0        0      855 2023-05-10 20:45:08.000000 qsimov-Mowstyl-5.1.1/qsimov_Mowstyl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      917 2023-05-10 20:45:08.000000 qsimov-Mowstyl-5.1.1/qsimov_Mowstyl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 20:45:08.000000 qsimov-Mowstyl-5.1.1/qsimov_Mowstyl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-10 20:45:08.000000 qsimov-Mowstyl-5.1.1/qsimov_Mowstyl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 20:45:08.000000 qsimov-Mowstyl-5.1.1/qsimov_Mowstyl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 20:45:09.323584 qsimov-Mowstyl-5.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-05-10 20:41:37.000000 qsimov-Mowstyl-5.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:56:43.093264 qsimov-Mowstyl-5.1.2/
+-rw-rw-rw-   0        0        0     1195 2024-04-04 20:56:43.092266 qsimov-Mowstyl-5.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      898 2024-04-03 23:20:48.000000 qsimov-Mowstyl-5.1.2/README.md
+-rw-rw-rw-   0        0        0      288 2024-04-04 20:55:49.000000 qsimov-Mowstyl-5.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-04 20:56:43.092266 qsimov-Mowstyl-5.1.2/qsimov_Mowstyl.egg-info/
+-rw-rw-rw-   0        0        0     1195 2024-04-04 20:56:43.000000 qsimov-Mowstyl-5.1.2/qsimov_Mowstyl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-04-04 20:56:43.000000 qsimov-Mowstyl-5.1.2/qsimov_Mowstyl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 20:56:43.000000 qsimov-Mowstyl-5.1.2/qsimov_Mowstyl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-04 20:56:43.000000 qsimov-Mowstyl-5.1.2/qsimov_Mowstyl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 20:56:43.000000 qsimov-Mowstyl-5.1.2/qsimov_Mowstyl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 20:56:43.093264 qsimov-Mowstyl-5.1.2/setup.cfg
```

