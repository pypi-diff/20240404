# Comparing `tmp/invideoquiz-xblock-1.5.0.tar.gz` & `tmp/invideoquiz-xblock-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invideoquiz-xblock-1.5.0.tar", last modified: Thu Feb 29 15:42:43 2024, max compression
+gzip compressed data, was "invideoquiz-xblock-1.6.0.tar", last modified: Thu Apr  4 04:47:42 2024, max compression
```

## Comparing `invideoquiz-xblock-1.5.0.tar` & `invideoquiz-xblock-1.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.004420 invideoquiz-xblock-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/LICENSE-BSD-3c
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-29 15:42:43.004420 invideoquiz-xblock-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.000420 invideoquiz-xblock-1.5.0/invideoquiz/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/invideoquiz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.000420 invideoquiz-xblock-1.5.0/invideoquiz/public/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/public/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.000420 invideoquiz-xblock-1.5.0/invideoquiz/public/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/public/css/invideoquiz.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.000420 invideoquiz-xblock-1.5.0/invideoquiz/public/html/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/public/html/invideoquiz.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.000420 invideoquiz-xblock-1.5.0/invideoquiz/public/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.004420 invideoquiz-xblock-1.5.0/invideoquiz/public/js/src/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/public/js/src/config.js
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/public/js/src/invideoquiz.js
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/invideoquiz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.004420 invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-29 15:42:42.000000 invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-29 15:42:42.000000 invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-29 15:42:42.000000 invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-29 15:42:42.000000 invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-29 15:42:42.000000 invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 15:42:42.000000 invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:42:43.004420 invideoquiz-xblock-1.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-29 15:42:43.004420 invideoquiz-xblock-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-02-29 15:42:39.000000 invideoquiz-xblock-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/LICENSE-BSD-3c
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/invideoquiz/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/invideoquiz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/invideoquiz/public/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/public/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/invideoquiz/public/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/public/css/invideoquiz.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/invideoquiz/public/html/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/public/html/invideoquiz.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.942823 invideoquiz-xblock-1.6.0/invideoquiz/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/invideoquiz/public/js/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/public/js/src/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/public/js/src/invideoquiz.js
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/invideoquiz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-04 04:47:42.000000 invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-04 04:47:42.000000 invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 04:47:42.000000 invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 04:47:42.000000 invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 04:47:42.000000 invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 04:47:42.000000 invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 04:47:42.946823 invideoquiz-xblock-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-04 04:47:39.000000 invideoquiz-xblock-1.6.0/setup.py
```

### Comparing `invideoquiz-xblock-1.5.0/LICENSE` & `invideoquiz-xblock-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.5.0/LICENSE-BSD-3c` & `invideoquiz-xblock-1.6.0/LICENSE-BSD-3c`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.5.0/PKG-INFO` & `invideoquiz-xblock-1.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: invideoquiz-xblock
-Version: 1.5.0
+Version: 1.6.0
 Summary: Helper XBlock to locate CAPA problems within videos.
 License: AGPL v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 License-File: LICENSE-BSD-3c
 Requires-Dist: Django
 Requires-Dist: XBlock
 Requires-Dist: six
```

### Comparing `invideoquiz-xblock-1.5.0/README.rst` & `invideoquiz-xblock-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.5.0/invideoquiz/invideoquiz.py` & `invideoquiz-xblock-1.6.0/invideoquiz/invideoquiz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
 This XBlock allows for edX components to be displayed to users inside of
 videos at specific time points.
 """
 
-import os
 import json
+import os
+
 import pkg_resources
 
 from xblock.core import XBlock
 from xblock.fields import Scope
 from xblock.fields import String
-from xblock.fragment import Fragment
+
+try:
+    from web_fragments.fragment import Fragment
+except ImportError:
+    # For backward compatibility with quince and earlier.
+    from xblock.fragment import Fragment
 from xblock.validation import ValidationMessage
 try:
     from xblock.utils.studio_editable import StudioEditableXBlockMixin
 except ModuleNotFoundError:
     # For backward compatibility with releases older than Quince.
     from xblockutils.studio_editable import StudioEditableXBlockMixin
```

### Comparing `invideoquiz-xblock-1.5.0/invideoquiz/public/README.txt` & `invideoquiz-xblock-1.6.0/invideoquiz/public/README.txt`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.5.0/invideoquiz/public/css/invideoquiz.css` & `invideoquiz-xblock-1.6.0/invideoquiz/public/css/invideoquiz.css`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.5.0/invideoquiz/public/js/src/config.js` & `invideoquiz-xblock-1.6.0/invideoquiz/public/js/src/config.js`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.5.0/invideoquiz/public/js/src/invideoquiz.js` & `invideoquiz-xblock-1.6.0/invideoquiz/public/js/src/invideoquiz.js`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/PKG-INFO` & `invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: invideoquiz-xblock
-Version: 1.5.0
+Version: 1.6.0
 Summary: Helper XBlock to locate CAPA problems within videos.
 License: AGPL v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 License-File: LICENSE-BSD-3c
 Requires-Dist: Django
 Requires-Dist: XBlock
 Requires-Dist: six
```

### Comparing `invideoquiz-xblock-1.5.0/invideoquiz_xblock.egg-info/SOURCES.txt` & `invideoquiz-xblock-1.6.0/invideoquiz_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invideoquiz-xblock-1.5.0/requirements/constraints.txt` & `invideoquiz-xblock-1.6.0/requirements/constraints.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
 # TODO: Many pinned dependencies should be unpinned and/or moved to this constraints file.
 
 # This file contains all common constraints for edx-repos
 -c common_constraints.txt
+backports.zoneinfo;python_version<"3.9"
```

### Comparing `invideoquiz-xblock-1.5.0/setup.py` & `invideoquiz-xblock-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,10 +152,11 @@
         'Framework :: Django',
         'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
 )
```

