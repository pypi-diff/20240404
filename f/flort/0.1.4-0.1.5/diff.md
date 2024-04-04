# Comparing `tmp/flort-0.1.4.tar.gz` & `tmp/flort-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flort-0.1.4.tar", last modified: Thu Apr  4 14:42:44 2024, max compression
+gzip compressed data, was "flort-0.1.5.tar", last modified: Thu Apr  4 14:44:07 2024, max compression
```

## Comparing `flort-0.1.4.tar` & `flort-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:42:44.110195 flort-0.1.4/
--rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.4/LICENSE
--rw-r--r--   0 nd        (1000) nd        (1000)     1711 2024-04-04 14:42:44.110195 flort-0.1.4/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)     1259 2024-04-04 14:42:30.000000 flort-0.1.4/README.md
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:42:44.110195 flort-0.1.4/flort/
--rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.4/flort/__init__.py
--rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1.4/flort/__main__.py
--rw-r--r--   0 nd        (1000) nd        (1000)     4136 2024-04-04 14:41:31.000000 flort-0.1.4/flort/cli.py
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:42:44.110195 flort-0.1.4/flort.egg-info/
--rw-r--r--   0 nd        (1000) nd        (1000)     1711 2024-04-04 14:42:43.000000 flort-0.1.4/flort.egg-info/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)      223 2024-04-04 14:42:44.000000 flort-0.1.4/flort.egg-info/SOURCES.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-04-04 14:42:43.000000 flort-0.1.4/flort.egg-info/dependency_links.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-04-04 14:42:43.000000 flort-0.1.4/flort.egg-info/entry_points.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-04-04 14:42:44.000000 flort-0.1.4/flort.egg-info/top_level.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-04-04 14:42:44.110195 flort-0.1.4/setup.cfg
--rw-r--r--   0 nd        (1000) nd        (1000)      778 2024-04-04 14:42:41.000000 flort-0.1.4/setup.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:44:07.093076 flort-0.1.5/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.5/LICENSE
+-rw-r--r--   0 nd        (1000) nd        (1000)     1716 2024-04-04 14:44:07.092076 flort-0.1.5/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)     1264 2024-04-04 14:43:55.000000 flort-0.1.5/README.md
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:44:07.092076 flort-0.1.5/flort/
+-rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.5/flort/__init__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1.5/flort/__main__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)     4136 2024-04-04 14:41:31.000000 flort-0.1.5/flort/cli.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:44:07.092076 flort-0.1.5/flort.egg-info/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1716 2024-04-04 14:44:06.000000 flort-0.1.5/flort.egg-info/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)      223 2024-04-04 14:44:07.000000 flort-0.1.5/flort.egg-info/SOURCES.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-04-04 14:44:06.000000 flort-0.1.5/flort.egg-info/dependency_links.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-04-04 14:44:06.000000 flort-0.1.5/flort.egg-info/entry_points.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-04-04 14:44:07.000000 flort-0.1.5/flort.egg-info/top_level.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-04-04 14:44:07.093076 flort-0.1.5/setup.cfg
+-rw-r--r--   0 nd        (1000) nd        (1000)      778 2024-04-04 14:44:04.000000 flort-0.1.5/setup.py
```

### Comparing `flort-0.1.4/LICENSE` & `flort-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flort-0.1.4/PKG-INFO` & `flort-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1.4
+Version: 0.1.5
 Summary: A utilty to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -24,41 +24,41 @@
 ```
 
 ## Usage
 
 flort provides various options for listing and cleaning up files in a directory.
 
 ```bash
-flort <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--tree]
+flort <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--no-tree]
 ```
 
 ### Options
 
 - `--compress`: Clean up files by removing unnecessary whitespace (optional).
 - `--output`: Specify the output file path (default: stdout).
 - `--php`, `--js`, `--py`, `--c`, `--cpp`: Include specific file types in the listing (optional).
-- `--tree`: Print the directory tree at the beginning of the output (optional).
+- `--no-tree`: Do not print the directory tree at the beginning of the output (optional).
 
 ## Examples
 
 List files in a directory and include PHP files:
 
 ```
-flort --dir /path/to/directory --php
+flort /path/to/directory --php
 ```
 
 Clean up files in a directory and save the output to a file:
 
 ```
-flort --dir /path/to/directory --compress --output output.txt
+flort /path/to/directory --compress --output output.txt
 ```
 
-List files in a directory, include JavaScript and Python files, and print the directory tree:
+List files in a directory, include JavaScript and Python files, and do not print the directory tree:
 
 ```
-flort --dir /path/to/directory --js --py --tree
+flort /path/to/directory --js --py --no-tree
 ```
 
 ## License
 
 This project is licensed under the BSD 3-Clause License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `flort-0.1.4/README.md` & `flort-0.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 ```
 
 ## Usage
 
 flort provides various options for listing and cleaning up files in a directory.
 
 ```bash
-flort <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--tree]
+flort <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--no-tree]
 ```
 
 ### Options
 
 - `--compress`: Clean up files by removing unnecessary whitespace (optional).
 - `--output`: Specify the output file path (default: stdout).
 - `--php`, `--js`, `--py`, `--c`, `--cpp`: Include specific file types in the listing (optional).
-- `--tree`: Print the directory tree at the beginning of the output (optional).
+- `--no-tree`: Do not print the directory tree at the beginning of the output (optional).
 
 ## Examples
 
 List files in a directory and include PHP files:
 
 ```
-flort --dir /path/to/directory --php
+flort /path/to/directory --php
 ```
 
 Clean up files in a directory and save the output to a file:
 
 ```
-flort --dir /path/to/directory --compress --output output.txt
+flort /path/to/directory --compress --output output.txt
 ```
 
-List files in a directory, include JavaScript and Python files, and print the directory tree:
+List files in a directory, include JavaScript and Python files, and do not print the directory tree:
 
 ```
-flort --dir /path/to/directory --js --py --tree
+flort /path/to/directory --js --py --no-tree
 ```
 
 ## License
 
 This project is licensed under the BSD 3-Clause License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `flort-0.1.4/flort/cli.py` & `flort-0.1.5/flort/cli.py`

 * *Files identical despite different names*

### Comparing `flort-0.1.4/flort.egg-info/PKG-INFO` & `flort-0.1.5/flort.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1.4
+Version: 0.1.5
 Summary: A utilty to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -24,41 +24,41 @@
 ```
 
 ## Usage
 
 flort provides various options for listing and cleaning up files in a directory.
 
 ```bash
-flort <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--tree]
+flort <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--no-tree]
 ```
 
 ### Options
 
 - `--compress`: Clean up files by removing unnecessary whitespace (optional).
 - `--output`: Specify the output file path (default: stdout).
 - `--php`, `--js`, `--py`, `--c`, `--cpp`: Include specific file types in the listing (optional).
-- `--tree`: Print the directory tree at the beginning of the output (optional).
+- `--no-tree`: Do not print the directory tree at the beginning of the output (optional).
 
 ## Examples
 
 List files in a directory and include PHP files:
 
 ```
-flort --dir /path/to/directory --php
+flort /path/to/directory --php
 ```
 
 Clean up files in a directory and save the output to a file:
 
 ```
-flort --dir /path/to/directory --compress --output output.txt
+flort /path/to/directory --compress --output output.txt
 ```
 
-List files in a directory, include JavaScript and Python files, and print the directory tree:
+List files in a directory, include JavaScript and Python files, and do not print the directory tree:
 
 ```
-flort --dir /path/to/directory --js --py --tree
+flort /path/to/directory --js --py --no-tree
 ```
 
 ## License
 
 This project is licensed under the BSD 3-Clause License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `flort-0.1.4/setup.py` & `flort-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flort',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'flort = flort.__main__:main'
         ]
     },
     install_requires=[
```

