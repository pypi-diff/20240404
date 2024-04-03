# Comparing `tmp/prrr-0.1.0.tar.gz` & `tmp/prrr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prrr-0.1.0.tar", max compression
+gzip compressed data, was "prrr-0.1.1.tar", max compression
```

## Comparing `prrr-0.1.0.tar` & `prrr-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3302 2024-04-03 22:18:15.591583 prrr-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-03 22:26:11.976855 prrr-0.1.0/prrr/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-03 22:23:53.115949 prrr-0.1.0/prrr/commands/__pycache__/init.cpython-312.pyc
--rw-r--r--   0        0        0     3726 2024-04-03 22:23:53.125721 prrr-0.1.0/prrr/commands/__pycache__/pr.cpython-312.pyc
--rw-r--r--   0        0        0     1918 2024-04-03 22:26:11.977057 prrr-0.1.0/prrr/commands/init.py
--rw-r--r--   0        0        0     2899 2024-04-03 22:26:11.977404 prrr-0.1.0/prrr/commands/pr.py
--rw-r--r--   0        0        0      397 2024-04-03 22:26:11.977618 prrr-0.1.0/prrr/main.py
--rw-r--r--   0        0        0     1547 2024-04-03 22:23:53.328354 prrr-0.1.0/prrr/utils/__pycache__/git.cpython-312.pyc
--rw-r--r--   0        0        0      172 2024-04-03 22:26:11.977740 prrr-0.1.0/prrr/utils/config_reader.py
--rw-r--r--   0        0        0      756 2024-04-03 22:26:11.977861 prrr-0.1.0/prrr/utils/git.py
--rw-r--r--   0        0        0      421 2024-04-03 22:26:11.978145 prrr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 prrr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3302 2024-04-03 22:18:15.591583 prrr-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 22:26:11.976855 prrr-0.1.1/prrr/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-03 22:40:19.220062 prrr-0.1.1/prrr/commands/__pycache__/init.cpython-312.pyc
+-rw-r--r--   0        0        0     3726 2024-04-03 22:40:19.229550 prrr-0.1.1/prrr/commands/__pycache__/pr.cpython-312.pyc
+-rw-r--r--   0        0        0     1918 2024-04-03 22:26:11.977057 prrr-0.1.1/prrr/commands/init.py
+-rw-r--r--   0        0        0     2899 2024-04-03 22:26:11.977404 prrr-0.1.1/prrr/commands/pr.py
+-rw-r--r--   0        0        0      397 2024-04-03 22:26:11.977618 prrr-0.1.1/prrr/main.py
+-rw-r--r--   0        0        0     1547 2024-04-03 22:40:19.439471 prrr-0.1.1/prrr/utils/__pycache__/git.cpython-312.pyc
+-rw-r--r--   0        0        0      172 2024-04-03 22:26:11.977740 prrr-0.1.1/prrr/utils/config_reader.py
+-rw-r--r--   0        0        0      756 2024-04-03 22:26:11.977861 prrr-0.1.1/prrr/utils/git.py
+-rw-r--r--   0        0        0      469 2024-04-03 22:41:50.304330 prrr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3908 1970-01-01 00:00:00.000000 prrr-0.1.1/PKG-INFO
```

### Comparing `prrr-0.1.0/README.md` & `prrr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prrr-0.1.0/prrr/commands/__pycache__/init.cpython-312.pyc` & `prrr-0.1.1/prrr/commands/__pycache__/init.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Wed Apr  3 22:18:15 2024 UTC, .py size: 1918 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 a7d5 0d66 7e07 0000  ...........f~...
+00000000: cb0d 0d0a 0000 0000 83d7 0d66 7e07 0000  ...........f~...
 00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
 00000020: 0000 0000 00f3 1200 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6402 8400 5a01 7901 2903 e900  l.Z.d...Z.y.)...
 00000040: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000050: 0008 0000 0003 0000 00f3 ae00 0000 9700  ................
 00000060: 6401 7d00 6402 6403 6404 6405 6406 6407  d.}.d.d.d.d.d.d.
 00000070: 6700 6408 a201 6409 9c07 7d01 7401 0000  g.d...d...}.t...
```

### Comparing `prrr-0.1.0/prrr/commands/__pycache__/pr.cpython-312.pyc` & `prrr-0.1.1/prrr/commands/__pycache__/pr.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Wed Apr  3 22:22:42 2024 UTC, .py size: 2899 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 b2d6 0d66 530b 0000  ...........fS...
+00000000: cb0d 0d0a 0000 0000 83d7 0d66 530b 0000  ...........fS...
 00000010: e300 0000 0000 0000 0000 0000 0011 0000  ................
 00000020: 0000 0000 00f3 fe01 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 0100  l.Z.d.d.l.m.Z...
 00000040: 6400 6401 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6400 6404 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
 00000060: 6400 6405 6c08 6d09 5a09 0100 6400 6406  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6400 6407 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `prrr-0.1.0/prrr/commands/init.py` & `prrr-0.1.1/prrr/commands/init.py`

 * *Files identical despite different names*

### Comparing `prrr-0.1.0/prrr/commands/pr.py` & `prrr-0.1.1/prrr/commands/pr.py`

 * *Files identical despite different names*

### Comparing `prrr-0.1.0/prrr/utils/__pycache__/git.cpython-312.pyc` & `prrr-0.1.1/prrr/utils/__pycache__/git.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Wed Apr  3 22:18:15 2024 UTC, .py size: 756 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 a7d5 0d66 f402 0000  ...........f....
+00000000: cb0d 0d0a 0000 0000 83d7 0d66 f402 0000  ...........f....
 00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
 00000020: 0000 0000 00f3 2400 0000 9700 6400 6401  ......$.....d.d.
 00000030: 6c00 5a00 6402 8400 5a01 6403 8400 5a02  l.Z.d...Z.d...Z.
 00000040: 6404 8400 5a03 6405 8400 5a04 7901 2906  d...Z.d...Z.y.).
 00000050: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
 00000060: 0000 0003 0000 0003 0000 00f3 6400 0000  ............d...
 00000070: 9700 7401 0000 0000 0000 0000 6a02 0000  ..t.........j...
```

### Comparing `prrr-0.1.0/prrr/utils/git.py` & `prrr-0.1.1/prrr/utils/git.py`

 * *Files identical despite different names*

### Comparing `prrr-0.1.0/PKG-INFO` & `prrr-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: prrr
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: A simple CLI tool to help you write better PRs.
 Author: Oscar Nevarez
 Author-email: fu.wire@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.9.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gitpython (>=3.1.24,<4.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: typer-config[yaml] (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
```

