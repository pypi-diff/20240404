# Comparing `tmp/brom_drake-0.0.2.tar.gz` & `tmp/brom_drake-0.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brom_drake-0.0.2.tar", last modified: Thu Apr  4 16:31:43 2024, max compression
+gzip compressed data, was "brom_drake-0.0.2.post2.tar", last modified: Thu Apr  4 20:39:57 2024, max compression
```

## Comparing `brom_drake-0.0.2.tar` & `brom_drake-0.0.2.post2.tar`

### file list

```diff
@@ -1,12 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:31:43.690851 brom_drake-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 16:31:36.000000 brom_drake-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-04 16:31:43.690851 brom_drake-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-04 16:31:36.000000 brom_drake-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:31:43.690851 brom_drake-0.0.2/brom_drake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-04 16:31:43.000000 brom_drake-0.0.2/brom_drake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-04 16:31:43.000000 brom_drake-0.0.2/brom_drake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:31:43.000000 brom_drake-0.0.2/brom_drake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 16:31:43.000000 brom_drake-0.0.2/brom_drake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:31:43.000000 brom_drake-0.0.2/brom_drake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:31:43.690851 brom_drake-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-04 16:31:41.000000 brom_drake-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 20:39:55.000000 brom_drake-0.0.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.287056 brom_drake-0.0.2.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake/DiagramTarget/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramTarget/DiagramTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramTarget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/DiagramWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake/all/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/all/add_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/top_level.txt
```

### Comparing `brom_drake-0.0.2/LICENSE` & `brom_drake-0.0.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `brom_drake-0.0.2/PKG-INFO` & `brom_drake-0.0.2.post2/src/brom_drake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: brom_drake
-Version: 0.0.2
+Name: brom-drake
+Version: 0.0.2.post2
 Summary: A set of convenient logging and testing tools for the Drake robotics toolbox.
 Author: Kwesi Rutledge
 Author-email: thesolitaryecrivain@gmail.com
 Keywords: drake,robotics,testing,logging
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `brom_drake-0.0.2/README.md` & `brom_drake-0.0.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `brom_drake-0.0.2/brom_drake.egg-info/PKG-INFO` & `brom_drake-0.0.2.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: brom-drake
-Version: 0.0.2
+Name: brom_drake
+Version: 0.0.2.post2
 Summary: A set of convenient logging and testing tools for the Drake robotics toolbox.
 Author: Kwesi Rutledge
 Author-email: thesolitaryecrivain@gmail.com
 Keywords: drake,robotics,testing,logging
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `brom_drake-0.0.2/setup.py` & `brom_drake-0.0.2.post2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     with codecs.open(
         os.path.join(here, "README.md"), encoding="utf-8"
     ) as f:
         long_description = "\n" + f.read()
 
     setup(
         name="brom_drake",
-        version='0.0.2',
+        version='0.0.2-2',
         author="Kwesi Rutledge",
         author_email="thesolitaryecrivain@gmail.com",
         description="A set of convenient logging and testing tools for the Drake robotics toolbox.",
         long_description_content_type="text/markdown",
         long_description=long_description,
-        packages=find_packages(),
+        # packages=find_packages(where='src/brom_drake'),
         install_requires=['drake', 'meshcat', 'manipulation', 'loguru', 'matplotlib'],
         keywords=["drake", "robotics", "testing", "logging"],
         classifiers=[
             "Programming Language :: Python :: 3",
         ]
     )
```

