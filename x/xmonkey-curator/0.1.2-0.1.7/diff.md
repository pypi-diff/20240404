# Comparing `tmp/xmonkey-curator-0.1.2.tar.gz` & `tmp/xmonkey-curator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey-curator-0.1.2.tar", last modified: Wed Mar 27 23:16:03 2024, max compression
+gzip compressed data, was "xmonkey-curator-0.1.7.tar", last modified: Thu Apr  4 07:09:24 2024, max compression
```

## Comparing `xmonkey-curator-0.1.2.tar` & `xmonkey-curator-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:16:03.864452 xmonkey-curator-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-27 23:16:03.864452 xmonkey-curator-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 23:16:03.864452 xmonkey-curator-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:16:03.856452 xmonkey-curator-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:16:03.856452 xmonkey-curator-0.1.2/src/xmonkey_curator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handler_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:16:03.860452 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/archive_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/cplus_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/elf_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/java_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/jvm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/objectivec_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/octetstream_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/perl_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/python_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/ruby_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/rust_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/text_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/lexer_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/report_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/src/xmonkey_curator/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:16:03.860452 xmonkey-curator-0.1.2/src/xmonkey_curator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-27 23:16:03.000000 xmonkey-curator-0.1.2/src/xmonkey_curator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-27 23:16:03.000000 xmonkey-curator-0.1.2/src/xmonkey_curator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 23:16:03.000000 xmonkey-curator-0.1.2/src/xmonkey_curator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 23:16:03.000000 xmonkey-curator-0.1.2/src/xmonkey_curator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-27 23:16:03.000000 xmonkey-curator-0.1.2/src/xmonkey_curator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 23:16:03.000000 xmonkey-curator-0.1.2/src/xmonkey_curator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:16:03.860452 xmonkey-curator-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/tests/test_base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-27 23:16:00.000000 xmonkey-curator-0.1.2/tests/test_text_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.790192 xmonkey-curator-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.790192 xmonkey-curator-0.1.7/src/xmonkey_curator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handler_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.794191 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/archive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/archivelib_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/cplus_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/elf_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/java_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/jvm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/machos_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/objectivec_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/octetstream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/perl_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/python_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/ruby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/rust_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/sharedlib_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/text_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/lexer_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/apache_2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/gpl_2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/gpl_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/licenses/lgpl_2_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/report_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/src/xmonkey_curator/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/rules/license_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/rules_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/src/xmonkey_curator/signatures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/signatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   214075 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/signatures/ffmpeg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/src/xmonkey_curator/symbols_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 07:09:24.000000 xmonkey-curator-0.1.7/src/xmonkey_curator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:09:24.798192 xmonkey-curator-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/tests/test_base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-04 07:09:21.000000 xmonkey-curator-0.1.7/tests/test_text_handler.py
```

### Comparing `xmonkey-curator-0.1.2/LICENSE` & `xmonkey-curator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/setup.py` & `xmonkey-curator-0.1.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+import os
+import re        
 from setuptools import setup, find_packages
 
+here = os.path.abspath(os.path.dirname(__file__))
+
+def read_version():
+    version_file_path = os.path.join(here, 'src', 'xmonkey_curator', '__version__.py')
+    with open(version_file_path, encoding='utf-8') as f:
+        version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", f.read(), re.M)
+        if version_match:
+            return version_match.group(1)
+        raise RuntimeError("Unable to find version string.")
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='xmonkey-curator',
-    version='0.1.2',
+    version=read_version(),
     description="Automated OSS curation scanner",
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author="Oscar Valenzuela",
     author_email="oscar.valenzuela.b@gmail.com",
     url='https://github.com/Xpertians/xmonkey-curator',
     license='Apache 2.0',
@@ -32,14 +44,15 @@
     entry_points={
         'console_scripts': [
             'xmonkey-curator=xmonkey_curator.scanner:scan',
         ],
     },
     include_package_data=True,
     package_data={
+        'xmonkey_curator': ['signatures/*.json', 'licenses/*.json', 'rules/*.json'],
     },
     test_suite="tests",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handler_registry.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handler_registry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 from .base_handler import BaseFileHandler
 from .handlers import TextFileHandler, ElfFileHandler, PythonFileHandler
 from .handlers import PerlFileHandler, CplusFileHandler, JavaFileHandler
 from .handlers import RustFileHandler, RubyFileHandler, ObjectivecFileHandler
 from .handlers import JvmFileHandler, OctetStreamFileHandler
+from .handlers import SharedLibFileHandler, ArchiveLibFileHandler
+from .handlers import MachOSFileHandler
 
 
 HANDLER_REGISTRY = {
-    'application/x-executable': ElfFileHandler,
     # Plan Text and String
     'text/plain': TextFileHandler,
     'text/x-makefile': TextFileHandler,
     'text/markdown': TextFileHandler,
     'text/css': TextFileHandler,
     'text/html': TextFileHandler,
     'text/xml': TextFileHandler,
     'text/csv': TextFileHandler,
+    'application/pls+xml': TextFileHandler,
+    'application/x-mpegurl': TextFileHandler,
+    'application/json': TextFileHandler,
     'text/x-tex': TextFileHandler,
     'text/vtt': TextFileHandler,
     'text/x-asm': TextFileHandler,
+    'text/x-m4': TextFileHandler,
     'text/x-shellscript': TextFileHandler,
     'text/cache-manifest': TextFileHandler,
+    'text/javascript': TextFileHandler,
+    'application/javascript': TextFileHandler,
     'application/json': TextFileHandler,
     'application/x-sh': TextFileHandler,
     'application/x-tex': TextFileHandler,
     'application/x-texinfo': TextFileHandler,
     'application/xml': TextFileHandler,
     'application/postscript': TextFileHandler,
     'application/cu-seeme': TextFileHandler,
     'application/x-msdownload': TextFileHandler,
     # Pygments based extraction
     'text/x-c': CplusFileHandler,
     'text/x-c++': CplusFileHandler,
     'text/x-python': PythonFileHandler,
     'application/x-python-code': PythonFileHandler,
+    'text/x-script.python': PythonFileHandler,
     'text/x-perl': PerlFileHandler,
     'text/x-java-source': JavaFileHandler,
     'application/java-vm': JvmFileHandler,
     'text/rust': RustFileHandler,
     'text/x-rust': RustFileHandler,
     'application/rls-services+xml': RustFileHandler,
     'text/ruby': RubyFileHandler,
     'text/x-ruby': RubyFileHandler,
     'text/x-objective-c': ObjectivecFileHandler,
     # Library Specific
     'application/octet-stream': OctetStreamFileHandler,
+    'application/x-executable': ElfFileHandler,
+    'application/x-sharedlib': SharedLibFileHandler,
+    'application/x-archive': ArchiveLibFileHandler,
+    'application/x-mach-binary': MachOSFileHandler,
 }
 
 
 def register_handler(mime_type, handler_class):
     """Registers a new handler for a given MIME type."""
     HANDLER_REGISTRY[mime_type] = handler_class
```

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/archive_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/archive_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/cplus_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/cplus_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/elf_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/machos_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,38 @@
-import lief
 import os
-from ..base_handler import BaseFileHandler
+import re
+import lief
 import logging
+from ..base_handler import BaseFileHandler
+from ..lexer_utilities import LexerUtilities
 
 
-class ElfFileHandler(BaseFileHandler):
+class MachOSFileHandler(BaseFileHandler):
     def __init__(self, file_path):
         super().__init__(file_path)
         self.logger = logging.getLogger(__name__)
 
     def extract_words(self):
-        """Extract strings from an ELF file using LIEF."""
         if not self.is_eligible():
             return []
         try:
-            elf = lief.parse(self.file_path)
-            strings = []
-            for section in elf.sections:
-                if section.name == ".rodata":
-                    data = section.content
-                    strings.extend(self._extract_strings_from_data(data))
-            if not strings:
+            libSO = lief.parse(self.file_path)
+            words = []
+            for i in libSO.symbols:
+                words.append(i.name)
+                print('sym:', i.name)
+            words = list(set(words))
+            if not words:
                 self.logger.warning(
                      f"No strings extracted from {self.file_path}."
                      )
-            return strings
-        except lief.exception as e:
+                # Using file data
+                strings = LexerUtilities.get_strings(self.file_path)
+                if strings:
+                    words = strings+words
+                    words = LexerUtilities.clean_strings(words)
+            return words
+        except Exception as e:
             self.logger.error(
-                 f"Error processing ELF file {self.file_path}: {e}"
+                 f"Error processing Shared Lib file {self.file_path}: {e}"
                  )
             return []
-
-    def _extract_strings_from_data(self, data):
-        """A utility method to extract strings from binary data."""
-        strings = []
-        current_str = []
-        for byte in data:
-            if 32 <= byte <= 127:  # Printable ASCII range
-                current_str.append(chr(byte))
-            elif current_str:
-                strings.append(''.join(current_str))
-                current_str = []
-        if current_str:  # Add the last string if any
-            strings.append(''.join(current_str))
-        return strings
```

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/java_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/java_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/objectivec_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/objectivec_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/octetstream_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/octetstream_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import logging
 from os import path
 from ..base_handler import BaseFileHandler
+from ..lexer_utilities import LexerUtilities
 
 
 class OctetStreamFileHandler(BaseFileHandler):
     def __init__(self, file_path):
         super().__init__(file_path)
         self.logger = logging.getLogger(__name__)
 
@@ -23,16 +24,11 @@
                         text += char
                         continue
                 except UnicodeDecodeError:
                     pass
                 if len(text) >= min_length:
                     strings.append(text)
                 text = ''
-            words = list(set(strings))
-            regex = re.compile(r'[^a-zA-Z\s_-]+')
-            words = [
-                regex.sub('', word).strip() for word in words
-                if len(regex.sub('', word).strip()) >= 5
-            ]
+            words = LexerUtilities.clean_strings(strings)
             return words
         else:
             return []
```

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/perl_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/perl_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/python_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/python_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/ruby_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/ruby_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/handlers/rust_handler.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/handlers/rust_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/src/xmonkey_curator/scanner.py` & `xmonkey-curator-0.1.7/src/xmonkey_curator/scanner.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,35 +3,39 @@
 import logging
 import mimetypes
 from tqdm import tqdm
 from xmonkey_curator.handler_registry import get_handler
 from xmonkey_curator.report_generator import ReportGenerator
 from xmonkey_curator.handlers.archive_handler import ArchiveHandler
 from xmonkey_curator.file_utilities import FileUtilities
+from xmonkey_curator.symbols_handler import SymbolsHandler
+from xmonkey_curator.rules_handler import RulesHandler
 
 
 logging.basicConfig(
     filename='debug.log',
     level=logging.INFO,
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 )
 logger = logging.getLogger(__name__)
 
 EXCLUDED_MIME_TYPE_PREFIXES = [
     'image/',
     'video/',
     'audio/',
+    'inode/'
 ]
 
 EXCLUDED_MIME_TYPES = [
     'application/pgp-signature',
     'application/x-font-type1',
     'application/pdf',
     'application/x-git',
-    'inode/symlink',
+    'application/pkix-attr-cert',
+    'application/msword'
 ]
 
 ARCHIVE_MIME_TYPES = [
     'application/zip',
     'application/gzip',
     'application/x-tar',
     'application/x-rpm',
@@ -40,47 +44,78 @@
     'application/vnd.android.package-archive',
 ]
 
 
 @click.command()
 @click.argument('path', type=click.Path(exists=True))
 @click.option('--force-text', '-t', is_flag=True,
-              help="Force the use of StringExtract for all files.")
-@click.option('--skip-extraction', '-se', is_flag=True,
-              help="Skip extracting files from archives.")
+              help="Force using StringExtract for all files.")
+@click.option('--recursive-extraction', '-r', is_flag=True,
+              help="Extracting archives files.")
+@click.option('--export-symbols', '-s', is_flag=True,
+              help="Include words in the final report.")
+@click.option('--match-symbols', '-m', is_flag=True,
+              help="Match symbols against signatures.")
 @click.option('--print-report', '-p', is_flag=True,
-              help="Print the report instead of saving to JSON.")
-def scan(path, force_text, skip_extraction, print_report):
+              help="Print the report to screen.")
+def scan(path,
+         force_text,
+         recursive_extraction,
+         export_symbols,
+         match_symbols,
+         print_report):
+    if not recursive_extraction:
+        export_symbols = False
+    if not export_symbols:
+        match_symbols = False
     results = []
     if os.path.isdir(path):
         logger.info(f"Scanning directory: {path}")
         all_files = [
             os.path.join(root, file)
             for root, _, files in os.walk(path)
             for file in files
         ]
         for file_path in tqdm(all_files, desc="Scanning files"):
             result = process_file(file_path, results, '',
-                                  force_text, skip_extraction)
+                                  force_text, recursive_extraction,
+                                  export_symbols)
             if result:
                 results.append(result)
     else:
         logger.info(f"Scanning file: {path}")
-        result = process_file(path, results, '', force_text, skip_extraction)
+        result = process_file(
+            path,
+            results,
+            '',
+            force_text,
+            recursive_extraction,
+            export_symbols
+        )
         if result:
             results.append(result)
+    rules = RulesHandler()
+    results = rules.execute(results)
+    if match_symbols:
+        sym_matcher = SymbolsHandler()
+        matches = sym_matcher.search(results)
+        results = results + matches
     report_generator = ReportGenerator(results)
     if print_report:
         report_generator.print_report()
     else:
         report_generator.save_report('scan_report.json')
 
 
-def process_file(file_path, results, archive_checksum=None,
-                 force_text=False, skip_extraction=False):
+def process_file(file_path,
+                 results,
+                 archive_checksum=None,
+                 force_text=False,
+                 recursive_extraction=False,
+                 export_symbols=False):
     mime_type = FileUtilities.identify_mime_type(file_path)
     file_size = FileUtilities.get_file_size(file_path)
     hash_md5, hash_sha1, hash_sha256, hash_ssdeep = (
             FileUtilities.calculate_hashes(file_path)
         )
     if mime_type in EXCLUDED_MIME_TYPES:
         logger.info(
@@ -90,39 +125,41 @@
     elif any(mime_type.startswith(prefix)
              for prefix in EXCLUDED_MIME_TYPE_PREFIXES):
         logger.info(
                     f"Skipping {file_path} as CLASS: {mime_type} is excluded"
                 )
         return None
     elif mime_type in ARCHIVE_MIME_TYPES:
-        if not skip_extraction:
+        if recursive_extraction:
             handler = ArchiveHandler(file_path)
             archive_checksum = hash_md5
             handler.process(
                 lambda path: process_file(
                     path,
                     results,
                     archive_checksum,
                     force_text,
-                    skip_extraction
+                    recursive_extraction,
+                    export_symbols
                 )
             )
         result = {
             'file_path': file_path,
             'mime_type': mime_type,
             'size': file_size,
             'hashes': {
                 "md5": hash_md5,
                 "fuzzy": hash_ssdeep,
                 "sha1": hash_sha1,
                 "sha256": hash_sha256
             },
             'is_archive': True,
-            'words': '',
         }
+        if export_symbols:
+            result['words'] = ''
         results.append(result)
     elif force_text:
         handler_class = get_handler("text/plain")
         if handler_class:
             handler = handler_class(file_path)
             words = handler.extract_words()
             result = {
@@ -132,16 +169,17 @@
                 'hashes': {
                     "md5": hash_md5,
                     "fuzzy": hash_ssdeep,
                     "sha1": hash_sha1,
                     "sha256": hash_sha256
                 },
                 'is_archive': False,
-                'words': words,
             }
+            if export_symbols:
+                result['words'] = handler.extract_words()
             if archive_checksum:
                 result['parent_checksum'] = archive_checksum
             results.append(result)
     else:
         handler_class = get_handler(
             mime_type if mime_type else "application/octet-stream"
         )
@@ -155,52 +193,56 @@
                     'hashes': {
                         "md5": hash_md5,
                         "fuzzy": hash_ssdeep,
                         "sha1": hash_sha1,
                         "sha256": hash_sha256
                     },
                     'is_archive': True,
-                    'words': '',
                 }
+                if export_symbols:
+                    result['words'] = ''
                 results.append(result)
                 archive_checksum = checksum
                 handler.process(
                     lambda path: process_file(
                         path,
                         results,
                         archive_checksum,
                         force_text,
-                        skip_extraction
+                        recursive_extraction,
+                        export_symbols
                     )
                 )
             else:
-                words = handler.extract_words()
-                if len(words) == 0:
-                    logger.info(
-                        f"No words returned for MIME type: {mime_type} "
-                        f"for file {file_path}"
-                    )
                 result = {
                     'file_path': file_path,
                     'mime_type': mime_type,
                     'size': file_size,
                     'hashes': {
                         "md5": hash_md5,
                         "fuzzy": hash_ssdeep,
                         "sha1": hash_sha1,
                         "sha256": hash_sha256
                     },
                     'is_archive': False,
-                    'words': words,
                 }
+                if export_symbols:
+                    words = handler.extract_words()
+                    if len(words) == 0:
+                        logger.info(
+                            f"No words returned for MIME type: {mime_type} "
+                            f"for file {file_path}"
+                        )
+                    result['words'] = words
                 if archive_checksum:
                     result['parent_checksum'] = archive_checksum
                 results.append(result)
         else:
             logger.info(
                 f"No handler registered for MIME type: {mime_type} "
                 f"for file {file_path}"
             )
             return None
 
+
 if __name__ == '__main__':
     scan()
```

### Comparing `xmonkey-curator-0.1.2/tests/test_base_handler.py` & `xmonkey-curator-0.1.7/tests/test_base_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey-curator-0.1.2/tests/test_text_handler.py` & `xmonkey-curator-0.1.7/tests/test_text_handler.py`

 * *Files identical despite different names*

