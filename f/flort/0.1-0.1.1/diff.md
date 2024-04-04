# Comparing `tmp/flort-0.1.tar.gz` & `tmp/flort-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flort-0.1.tar", last modified: Thu Apr  4 13:58:11 2024, max compression
+gzip compressed data, was "flort-0.1.1.tar", last modified: Thu Apr  4 13:59:57 2024, max compression
```

## Comparing `flort-0.1.tar` & `flort-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:58:11.244187 flort-0.1/
--rw-r--r--   0 nd        (1000) nd        (1000)     1968 2024-04-04 13:58:11.244187 flort-0.1/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)     1539 2024-04-04 13:31:21.000000 flort-0.1/README.md
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:58:11.243187 flort-0.1/flort/
--rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1/flort/__init__.py
--rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1/flort/__main__.py
--rw-r--r--   0 nd        (1000) nd        (1000)     3960 2024-04-04 13:54:00.000000 flort-0.1/flort/cli.py
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:58:11.244187 flort-0.1/flort.egg-info/
--rw-r--r--   0 nd        (1000) nd        (1000)     1968 2024-04-04 13:58:10.000000 flort-0.1/flort.egg-info/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)      215 2024-04-04 13:58:11.000000 flort-0.1/flort.egg-info/SOURCES.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-04-04 13:58:10.000000 flort-0.1/flort.egg-info/dependency_links.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-04-04 13:58:11.000000 flort-0.1/flort.egg-info/entry_points.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-04-04 13:58:11.000000 flort-0.1/flort.egg-info/top_level.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-04-04 13:58:11.244187 flort-0.1/setup.cfg
--rw-r--r--   0 nd        (1000) nd        (1000)      776 2024-04-04 13:58:07.000000 flort-0.1/setup.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:59:57.867179 flort-0.1.1/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1755 2024-04-04 13:59:57.867179 flort-0.1.1/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)     1325 2024-04-04 13:59:38.000000 flort-0.1.1/README.md
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:59:57.867179 flort-0.1.1/flort/
+-rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.1/flort/__init__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1.1/flort/__main__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)     3960 2024-04-04 13:54:00.000000 flort-0.1.1/flort/cli.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:59:57.867179 flort-0.1.1/flort.egg-info/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1755 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)      215 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/SOURCES.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/dependency_links.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/entry_points.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/top_level.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-04-04 13:59:57.867179 flort-0.1.1/setup.cfg
+-rw-r--r--   0 nd        (1000) nd        (1000)      778 2024-04-04 13:59:54.000000 flort-0.1.1/setup.py
```

### Comparing `flort-0.1/PKG-INFO` & `flort-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1
+Version: 0.1.1
 Summary: A utilty to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-Here's a README for your project:
+# flort
 
----
-
-# Pancake
-
-Pancake is a command-line tool for listing and optionally cleaning up files in a directory.
+flort is a command-line tool for generating a single file with the contents of your code directories.. for use in LLMs.
 
 ## Installation
 
-You can install Pancake via pip:
+You can install flort via pip:
 
 ```
-pip install pancake
+pip install flort
 ```
 
 ## Usage
 
-Pancake provides various options for listing and cleaning up files in a directory.
+flort provides various options for listing and cleaning up files in a directory.
 
 ```
-pancake --dir <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--tree]
+flort --dir <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--tree]
 ```
 
 ### Options
 
 - `--dir`: Specify the directory to list files from (required).
 - `--compress`: Clean up files by removing unnecessary whitespace (optional).
 - `--output`: Specify the output file path (default: stdout).
@@ -43,29 +39,26 @@
 - `--tree`: Print the directory tree at the beginning of the output (optional).
 
 ## Examples
 
 List files in a directory and include PHP files:
 
 ```
-pancake --dir /path/to/directory --php
+flort --dir /path/to/directory --php
 ```
 
 Clean up files in a directory and save the output to a file:
 
 ```
-pancake --dir /path/to/directory --compress --output output.txt
+flort --dir /path/to/directory --compress --output output.txt
 ```
 
 List files in a directory, include JavaScript and Python files, and print the directory tree:
 
 ```
-pancake --dir /path/to/directory --js --py --tree
+flort --dir /path/to/directory --js --py --tree
 ```
 
 ## License
 
 This project is licensed under the BSD 3-Clause License - see the [LICENSE](LICENSE) file for details.
 
---- 
-
-You might need to provide additional information about the project's dependencies, how to contribute, or any other relevant details depending on your specific project requirements.
```

### Comparing `flort-0.1/flort/cli.py` & `flort-0.1.1/flort/cli.py`

 * *Files identical despite different names*

### Comparing `flort-0.1/flort.egg-info/PKG-INFO` & `flort-0.1.1/flort.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1
+Version: 0.1.1
 Summary: A utilty to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-Here's a README for your project:
+# flort
 
----
-
-# Pancake
-
-Pancake is a command-line tool for listing and optionally cleaning up files in a directory.
+flort is a command-line tool for generating a single file with the contents of your code directories.. for use in LLMs.
 
 ## Installation
 
-You can install Pancake via pip:
+You can install flort via pip:
 
 ```
-pip install pancake
+pip install flort
 ```
 
 ## Usage
 
-Pancake provides various options for listing and cleaning up files in a directory.
+flort provides various options for listing and cleaning up files in a directory.
 
 ```
-pancake --dir <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--tree]
+flort --dir <directory_path> [--compress] [--output <output_file>] [--php] [--js] [--py] [--c] [--cpp] [--tree]
 ```
 
 ### Options
 
 - `--dir`: Specify the directory to list files from (required).
 - `--compress`: Clean up files by removing unnecessary whitespace (optional).
 - `--output`: Specify the output file path (default: stdout).
@@ -43,29 +39,26 @@
 - `--tree`: Print the directory tree at the beginning of the output (optional).
 
 ## Examples
 
 List files in a directory and include PHP files:
 
 ```
-pancake --dir /path/to/directory --php
+flort --dir /path/to/directory --php
 ```
 
 Clean up files in a directory and save the output to a file:
 
 ```
-pancake --dir /path/to/directory --compress --output output.txt
+flort --dir /path/to/directory --compress --output output.txt
 ```
 
 List files in a directory, include JavaScript and Python files, and print the directory tree:
 
 ```
-pancake --dir /path/to/directory --js --py --tree
+flort --dir /path/to/directory --js --py --tree
 ```
 
 ## License
 
 This project is licensed under the BSD 3-Clause License - see the [LICENSE](LICENSE) file for details.
 
---- 
-
-You might need to provide additional information about the project's dependencies, how to contribute, or any other relevant details depending on your specific project requirements.
```

### Comparing `flort-0.1/setup.py` & `flort-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flort',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'flort = flort.__main__:main'
         ]
     },
     install_requires=[
```

