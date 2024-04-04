# Comparing `tmp/flort-0.1.1.tar.gz` & `tmp/flort-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flort-0.1.1.tar", last modified: Thu Apr  4 13:59:57 2024, max compression
+gzip compressed data, was "flort-0.1.2.tar", last modified: Thu Apr  4 14:39:30 2024, max compression
```

## Comparing `flort-0.1.1.tar` & `flort-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:59:57.867179 flort-0.1.1/
--rw-r--r--   0 nd        (1000) nd        (1000)     1755 2024-04-04 13:59:57.867179 flort-0.1.1/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)     1325 2024-04-04 13:59:38.000000 flort-0.1.1/README.md
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:59:57.867179 flort-0.1.1/flort/
--rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.1/flort/__init__.py
--rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1.1/flort/__main__.py
--rw-r--r--   0 nd        (1000) nd        (1000)     3960 2024-04-04 13:54:00.000000 flort-0.1.1/flort/cli.py
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 13:59:57.867179 flort-0.1.1/flort.egg-info/
--rw-r--r--   0 nd        (1000) nd        (1000)     1755 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)      215 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/SOURCES.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/dependency_links.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/entry_points.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-04-04 13:59:57.000000 flort-0.1.1/flort.egg-info/top_level.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-04-04 13:59:57.867179 flort-0.1.1/setup.cfg
--rw-r--r--   0 nd        (1000) nd        (1000)      778 2024-04-04 13:59:54.000000 flort-0.1.1/setup.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:39:30.712148 flort-0.1.2/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.2/LICENSE
+-rw-r--r--   0 nd        (1000) nd        (1000)     1777 2024-04-04 14:39:30.711148 flort-0.1.2/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)     1325 2024-04-04 13:59:38.000000 flort-0.1.2/README.md
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:39:30.711148 flort-0.1.2/flort/
+-rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.2/flort/__init__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1.2/flort/__main__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)     4126 2024-04-04 14:37:46.000000 flort-0.1.2/flort/cli.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:39:30.711148 flort-0.1.2/flort.egg-info/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1777 2024-04-04 14:39:30.000000 flort-0.1.2/flort.egg-info/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)      223 2024-04-04 14:39:30.000000 flort-0.1.2/flort.egg-info/SOURCES.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-04-04 14:39:30.000000 flort-0.1.2/flort.egg-info/dependency_links.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-04-04 14:39:30.000000 flort-0.1.2/flort.egg-info/entry_points.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-04-04 14:39:30.000000 flort-0.1.2/flort.egg-info/top_level.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-04-04 14:39:30.712148 flort-0.1.2/setup.cfg
+-rw-r--r--   0 nd        (1000) nd        (1000)      778 2024-04-04 14:39:28.000000 flort-0.1.2/setup.py
```

### Comparing `flort-0.1.1/PKG-INFO` & `flort-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utilty to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # flort
 
 flort is a command-line tool for generating a single file with the contents of your code directories.. for use in LLMs.
 
 ## Installation
```

### Comparing `flort-0.1.1/README.md` & `flort-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flort-0.1.1/flort/cli.py` & `flort-0.1.2/flort/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,28 @@
     """Cleans up the content of a file by removing unnecessary whitespace."""
     with open(file_path, 'r') as file:
         lines = file.readlines()
         cleaned_lines = [line.strip() for line in lines if line.strip()]
         return '\n'.join(cleaned_lines)
 
 def generate_tree(directory):
-    """Generates a tree structure of the given directory."""
+    """Generates a tree structure of the given directory, ignoring .git folders."""
     tree_structure = ''
     for root, dirs, files in os.walk(directory):
+        if '.git' in dirs:
+            dirs.remove('.git')  # Ignore .git folder
         level = root.replace(directory, '').count(os.sep)
         indent = '|   ' * level + '|-- '
         tree_structure += f"{indent}{os.path.basename(root)}/\n"
         sub_indent = '|   ' * (level + 1) + '|-- '
         for file in files:
             tree_structure += f"{sub_indent}{file}\n"
     return tree_structure
 
+
 def list_files(directory, compress=False, extensions=None):
     """Lists files in the given directory with optional compression."""
     directory_path = Path(directory)
     if not directory_path.is_dir():
         print(f"The path {directory} is not a valid directory.")
         return
     
@@ -67,30 +70,32 @@
     parser.add_argument('--compress', default=False, action='store_true', help='Compress the listed files by removing whitespace.')
     parser.add_argument('--output', type=str, default="stdio", help='Output file path. Defaults to stdout if not specified.')
     parser.add_argument('--php', action='store_true', help='Include PHP files.')
     parser.add_argument('--js', action='store_true', help='Include JavaScript files.')
     parser.add_argument('--py', action='store_true', help='Include Python files.')
     parser.add_argument('--c', action='store_true', help='Include C files.')
     parser.add_argument('--cpp', action='store_true', help='Include C++ files.')    
-    parser.add_argument('--tree', default=True, action='store_true', help='Print the tree at the beginning.')    
+    parser.add_argument('--no-tree', action='store_true', help='Dont print the tree at the beginning.')    
     args = parser.parse_args()
     
     extensions = []
     output = []
     if args.php:
         extensions.append('.php')
     if args.js:
         extensions.append('.js')
     if args.py:
         extensions.append('.py')
     if args.c:
         extensions.append('.c')
+        extensions.append('.h')
     if args.cpp:
         extensions.append('.cpp')
-    if args.tree == True:
+        extensions.append('.h')
+    if args.no_tree != True:
         output.append(generate_tree(args.dir))
     
     output.append(list_files(args.dir, compress=args.compress, extensions=extensions))
 
     if args.output != "stdio":    
         write_file(args.output, "\n".join(output))
     else:
```

### Comparing `flort-0.1.1/flort.egg-info/PKG-INFO` & `flort-0.1.2/flort.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1.1
+Version: 0.1.2
 Summary: A utilty to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # flort
 
 flort is a command-line tool for generating a single file with the contents of your code directories.. for use in LLMs.
 
 ## Installation
```

### Comparing `flort-0.1.1/setup.py` & `flort-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flort',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'flort = flort.__main__:main'
         ]
     },
     install_requires=[
```

