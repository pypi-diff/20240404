# Comparing `tmp/frogress-0.9.0.tar.gz` & `tmp/frogress-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/frogress-0.9.0.tar", last modified: Tue Jun  4 23:50:13 2013, max compression
+gzip compressed data, was "dist/frogress-0.9.1.tar", last modified: Sun Jun 23 17:36:44 2013, max compression
```

## Comparing `frogress-0.9.0.tar` & `frogress-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-04 23:50:13.000000 frogress-0.9.0/
-drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-04 23:50:13.000000 frogress-0.9.0/frogress/
--rw-r--r--   0 lukasz     (501) staff       (20)     1023 2013-06-04 21:25:49.000000 frogress-0.9.0/frogress/__init__.py
--rw-r--r--   0 lukasz     (501) staff       (20)      538 2013-06-02 22:10:09.000000 frogress-0.9.0/frogress/api.py
--rw-r--r--   0 lukasz     (501) staff       (20)     4145 2013-06-04 23:26:21.000000 frogress-0.9.0/frogress/bars.py
--rw-r--r--   0 lukasz     (501) staff       (20)     1092 2013-06-04 22:13:28.000000 frogress-0.9.0/frogress/humanize.py
-drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-04 23:50:13.000000 frogress-0.9.0/frogress/tests/
--rw-r--r--   0 lukasz     (501) staff       (20)      216 2013-06-02 22:28:43.000000 frogress-0.9.0/frogress/tests/__init__.py
--rw-r--r--   0 lukasz     (501) staff       (20)      126 2013-06-02 22:28:15.000000 frogress-0.9.0/frogress/tests/compat.py
--rw-r--r--   0 lukasz     (501) staff       (20)      745 2013-06-04 22:05:24.000000 frogress-0.9.0/frogress/tests/test_api.py
--rw-r--r--   0 lukasz     (501) staff       (20)     5391 2013-06-04 23:26:21.000000 frogress-0.9.0/frogress/tests/test_bars.py
--rw-r--r--   0 lukasz     (501) staff       (20)     1107 2013-06-03 22:50:08.000000 frogress-0.9.0/frogress/tests/test_humanize.py
--rw-r--r--   0 lukasz     (501) staff       (20)      663 2013-06-04 21:26:10.000000 frogress-0.9.0/frogress/tests/test_main.py
--rw-r--r--   0 lukasz     (501) staff       (20)     2857 2013-06-04 22:12:12.000000 frogress-0.9.0/frogress/tests/test_utils.py
--rw-r--r--   0 lukasz     (501) staff       (20)     6885 2013-06-04 21:19:36.000000 frogress-0.9.0/frogress/tests/test_widgets.py
--rw-r--r--   0 lukasz     (501) staff       (20)     1027 2013-06-02 21:56:44.000000 frogress-0.9.0/frogress/utils.py
--rw-r--r--   0 lukasz     (501) staff       (20)     3274 2013-06-04 11:34:41.000000 frogress-0.9.0/frogress/widgets.py
-drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-04 23:50:13.000000 frogress-0.9.0/frogress.egg-info/
--rw-r--r--   0 lukasz     (501) staff       (20)        1 2013-06-04 23:50:13.000000 frogress-0.9.0/frogress.egg-info/dependency_links.txt
--rw-r--r--   0 lukasz     (501) staff       (20)        1 2013-05-26 21:50:11.000000 frogress-0.9.0/frogress.egg-info/not-zip-safe
--rw-r--r--   0 lukasz     (501) staff       (20)     8114 2013-06-04 23:50:13.000000 frogress-0.9.0/frogress.egg-info/PKG-INFO
--rw-r--r--   0 lukasz     (501) staff       (20)      518 2013-06-04 23:50:13.000000 frogress-0.9.0/frogress.egg-info/SOURCES.txt
--rw-r--r--   0 lukasz     (501) staff       (20)        9 2013-06-04 23:50:13.000000 frogress-0.9.0/frogress.egg-info/top_level.txt
--rw-r--r--   0 lukasz     (501) staff       (20)     8114 2013-06-04 23:50:13.000000 frogress-0.9.0/PKG-INFO
--rw-r--r--   0 lukasz     (501) staff       (20)     6041 2013-06-04 22:32:31.000000 frogress-0.9.0/README.rst
--rw-r--r--   0 lukasz     (501) staff       (20)       59 2013-06-04 23:50:13.000000 frogress-0.9.0/setup.cfg
--rw-r--r--   0 lukasz     (501) staff       (20)     1330 2013-06-03 22:19:46.000000 frogress-0.9.0/setup.py
+drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-23 17:36:44.000000 frogress-0.9.1/
+-rwxr-xr-x   0 lukasz     (501) staff       (20)     2467 2013-06-04 23:26:18.000000 frogress-0.9.1/examples.py
+drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-23 17:36:44.000000 frogress-0.9.1/frogress/
+-rw-r--r--   0 lukasz     (501) staff       (20)     1023 2013-06-23 17:36:13.000000 frogress-0.9.1/frogress/__init__.py
+-rw-r--r--   0 lukasz     (501) staff       (20)      538 2013-06-02 22:10:09.000000 frogress-0.9.1/frogress/api.py
+-rw-r--r--   0 lukasz     (501) staff       (20)     4145 2013-06-06 09:42:22.000000 frogress-0.9.1/frogress/bars.py
+-rw-r--r--   0 lukasz     (501) staff       (20)     1092 2013-06-04 22:13:28.000000 frogress-0.9.1/frogress/humanize.py
+drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-23 17:36:44.000000 frogress-0.9.1/frogress/tests/
+-rw-r--r--   0 lukasz     (501) staff       (20)      216 2013-06-02 22:28:43.000000 frogress-0.9.1/frogress/tests/__init__.py
+-rw-r--r--   0 lukasz     (501) staff       (20)      126 2013-06-02 22:28:15.000000 frogress-0.9.1/frogress/tests/compat.py
+-rw-r--r--   0 lukasz     (501) staff       (20)      745 2013-06-04 22:05:24.000000 frogress-0.9.1/frogress/tests/test_api.py
+-rw-r--r--   0 lukasz     (501) staff       (20)     5391 2013-06-04 23:26:21.000000 frogress-0.9.1/frogress/tests/test_bars.py
+-rw-r--r--   0 lukasz     (501) staff       (20)     1107 2013-06-03 22:50:08.000000 frogress-0.9.1/frogress/tests/test_humanize.py
+-rw-r--r--   0 lukasz     (501) staff       (20)      663 2013-06-04 21:26:10.000000 frogress-0.9.1/frogress/tests/test_main.py
+-rw-r--r--   0 lukasz     (501) staff       (20)     2857 2013-06-04 22:12:12.000000 frogress-0.9.1/frogress/tests/test_utils.py
+-rw-r--r--   0 lukasz     (501) staff       (20)     6885 2013-06-04 21:19:36.000000 frogress-0.9.1/frogress/tests/test_widgets.py
+-rw-r--r--   0 lukasz     (501) staff       (20)     1027 2013-06-02 21:56:44.000000 frogress-0.9.1/frogress/utils.py
+-rw-r--r--   0 lukasz     (501) staff       (20)     3274 2013-06-04 11:34:41.000000 frogress-0.9.1/frogress/widgets.py
+drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-23 17:36:44.000000 frogress-0.9.1/frogress.egg-info/
+-rw-r--r--   0 lukasz     (501) staff       (20)        1 2013-06-23 17:36:44.000000 frogress-0.9.1/frogress.egg-info/dependency_links.txt
+-rw-r--r--   0 lukasz     (501) staff       (20)        1 2013-05-26 21:50:11.000000 frogress-0.9.1/frogress.egg-info/not-zip-safe
+-rw-r--r--   0 lukasz     (501) staff       (20)     8846 2013-06-23 17:36:44.000000 frogress-0.9.1/frogress.egg-info/PKG-INFO
+-rw-r--r--   0 lukasz     (501) staff       (20)      595 2013-06-23 17:36:44.000000 frogress-0.9.1/frogress.egg-info/SOURCES.txt
+-rw-r--r--   0 lukasz     (501) staff       (20)        9 2013-06-23 17:36:44.000000 frogress-0.9.1/frogress.egg-info/top_level.txt
+-rw-r--r--   0 lukasz     (501) staff       (20)     1082 2013-06-03 22:19:00.000000 frogress-0.9.1/LICENSE
+-rw-r--r--   0 lukasz     (501) staff       (20)      168 2013-06-23 17:36:36.000000 frogress-0.9.1/MANIFEST.in
+-rw-r--r--   0 lukasz     (501) staff       (20)     8846 2013-06-23 17:36:44.000000 frogress-0.9.1/PKG-INFO
+-rw-r--r--   0 lukasz     (501) staff       (20)     6621 2013-06-23 17:30:14.000000 frogress-0.9.1/README.rst
+drwxr-xr-x   0 lukasz     (501) staff       (20)        0 2013-06-23 17:36:44.000000 frogress-0.9.1/sampledata/
+-rw-r--r--   0 lukasz     (501) staff       (20)     4430 2013-05-29 11:41:42.000000 frogress-0.9.1/sampledata/books.xml
+-rw-r--r--   0 lukasz     (501) staff       (20)     1380 2013-05-29 11:41:12.000000 frogress-0.9.1/sampledata/books.xml.gz
+-rw-r--r--   0 lukasz     (501) staff       (20)       59 2013-06-23 17:36:44.000000 frogress-0.9.1/setup.cfg
+-rw-r--r--   0 lukasz     (501) staff       (20)     1265 2013-06-06 10:28:32.000000 frogress-0.9.1/setup.py
```

### Comparing `frogress-0.9.0/frogress/__init__.py` & `frogress-0.9.1/frogress/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'TimerWidget',
     'WhirlWidget',
     'get_file_info',
     'get_iterable_size',
     'bar',
 ]
 
-VERSION = (0, 9, 0)
+VERSION = (0, 9, 1)
 
 __version__ = '.'.join((str(each) for each in VERSION[:4]))
 
 def get_version():
     """
     Returns shorter version (digit parts only) as string.
     """
```

### Comparing `frogress-0.9.0/frogress/api.py` & `frogress-0.9.1/frogress/api.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/bars.py` & `frogress-0.9.1/frogress/bars.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/humanize.py` & `frogress-0.9.1/frogress/humanize.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/tests/test_api.py` & `frogress-0.9.1/frogress/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/tests/test_bars.py` & `frogress-0.9.1/frogress/tests/test_bars.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/tests/test_humanize.py` & `frogress-0.9.1/frogress/tests/test_humanize.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/tests/test_main.py` & `frogress-0.9.1/frogress/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/tests/test_utils.py` & `frogress-0.9.1/frogress/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/tests/test_widgets.py` & `frogress-0.9.1/frogress/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/utils.py` & `frogress-0.9.1/frogress/utils.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress/widgets.py` & `frogress-0.9.1/frogress/widgets.py`

 * *Files identical despite different names*

### Comparing `frogress-0.9.0/frogress.egg-info/PKG-INFO` & `frogress-0.9.1/frogress.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 1.1
 Name: frogress
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 frogress is simple progress tool
 
 Home-page: https://github.com/lukaszb/frogress
 Author: Lukasz Balcerzak
 Author-email: lukaszbalcerzak@gmail.com
 License: MIT
 Description: =====================================
         frogress - a progress tool for humans
         =====================================
         
         .. image:: https://secure.travis-ci.org/lukaszb/frogress.png?branch=master
-          :target: http://travis-ci.org/lukaszb/frogress
+           :target: http://travis-ci.org/lukaszb/frogress
+        
+        .. image:: https://coveralls.io/repos/lukaszb/frogress/badge.png?branch=master
+           :target: https://coveralls.io/r/lukaszb/frogress/
+        
+        .. image:: https://pypip.in/v/frogress/badge.png
+           :target: https://crate.io/packages/frogress/
         
         ::
         
                         /----------------------------------------------------------------------------------\
                         |                                                                                  |
               @..@     /| [###.......] Progress: 34.2MB / 125.8MB |  25.0% | Time: 14min3s | ETA: 19min52s |
              (----)   / |                                                                                  |
@@ -193,14 +199,27 @@
             <open file '<stderr>', mode 'w' at 0x103df61e0>
             >>> progressbar.started
             datetime.datetime(2013, 5, 12, 22, 2, 26, 752454)
             >>> progressbar.finished
             datetime.datetime(2013, 5, 12, 22, 2, 26, 792901)
         
         
+        Tips & Tricks
+        =============
+        
+        How to change label of the progress widget
+        ------------------------------------------
+        
+        ::
+        
+            >>> import frogress
+            >>> items = [1, 2, 3, 4, 5]
+            >>> widgets = [frogress.BarWidget, frogress.ProgressWidget('Items: '), frogress.TimerWidget]
+            >>> for item in frogress.bar(items, widgets=widgets):
+            >>>     pass
         
         
         .. _lxml: http://lxml.de/
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `frogress-0.9.0/frogress.egg-info/SOURCES.txt` & `frogress-0.9.1/frogress.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+LICENSE
+MANIFEST.in
 README.rst
+examples.py
 setup.py
 frogress/__init__.py
 frogress/api.py
 frogress/bars.py
 frogress/humanize.py
 frogress/utils.py
 frogress/widgets.py
@@ -14,8 +17,10 @@
 frogress/tests/__init__.py
 frogress/tests/compat.py
 frogress/tests/test_api.py
 frogress/tests/test_bars.py
 frogress/tests/test_humanize.py
 frogress/tests/test_main.py
 frogress/tests/test_utils.py
-frogress/tests/test_widgets.py
+frogress/tests/test_widgets.py
+sampledata/books.xml
+sampledata/books.xml.gz
```

### Comparing `frogress-0.9.0/PKG-INFO` & `frogress-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 1.1
 Name: frogress
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 frogress is simple progress tool
 
 Home-page: https://github.com/lukaszb/frogress
 Author: Lukasz Balcerzak
 Author-email: lukaszbalcerzak@gmail.com
 License: MIT
 Description: =====================================
         frogress - a progress tool for humans
         =====================================
         
         .. image:: https://secure.travis-ci.org/lukaszb/frogress.png?branch=master
-          :target: http://travis-ci.org/lukaszb/frogress
+           :target: http://travis-ci.org/lukaszb/frogress
+        
+        .. image:: https://coveralls.io/repos/lukaszb/frogress/badge.png?branch=master
+           :target: https://coveralls.io/r/lukaszb/frogress/
+        
+        .. image:: https://pypip.in/v/frogress/badge.png
+           :target: https://crate.io/packages/frogress/
         
         ::
         
                         /----------------------------------------------------------------------------------\
                         |                                                                                  |
               @..@     /| [###.......] Progress: 34.2MB / 125.8MB |  25.0% | Time: 14min3s | ETA: 19min52s |
              (----)   / |                                                                                  |
@@ -193,14 +199,27 @@
             <open file '<stderr>', mode 'w' at 0x103df61e0>
             >>> progressbar.started
             datetime.datetime(2013, 5, 12, 22, 2, 26, 752454)
             >>> progressbar.finished
             datetime.datetime(2013, 5, 12, 22, 2, 26, 792901)
         
         
+        Tips & Tricks
+        =============
+        
+        How to change label of the progress widget
+        ------------------------------------------
+        
+        ::
+        
+            >>> import frogress
+            >>> items = [1, 2, 3, 4, 5]
+            >>> widgets = [frogress.BarWidget, frogress.ProgressWidget('Items: '), frogress.TimerWidget]
+            >>> for item in frogress.bar(items, widgets=widgets):
+            >>>     pass
         
         
         .. _lxml: http://lxml.de/
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `frogress-0.9.0/README.rst` & `frogress-0.9.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 =====================================
 frogress - a progress tool for humans
 =====================================
 
 .. image:: https://secure.travis-ci.org/lukaszb/frogress.png?branch=master
-  :target: http://travis-ci.org/lukaszb/frogress
+   :target: http://travis-ci.org/lukaszb/frogress
+
+.. image:: https://coveralls.io/repos/lukaszb/frogress/badge.png?branch=master
+   :target: https://coveralls.io/r/lukaszb/frogress/
+
+.. image:: https://pypip.in/v/frogress/badge.png
+   :target: https://crate.io/packages/frogress/
 
 ::
 
                 /----------------------------------------------------------------------------------\
                 |                                                                                  |
       @..@     /| [###.......] Progress: 34.2MB / 125.8MB |  25.0% | Time: 14min3s | ETA: 19min52s |
      (----)   / |                                                                                  |
@@ -183,11 +189,24 @@
     <open file '<stderr>', mode 'w' at 0x103df61e0>
     >>> progressbar.started
     datetime.datetime(2013, 5, 12, 22, 2, 26, 752454)
     >>> progressbar.finished
     datetime.datetime(2013, 5, 12, 22, 2, 26, 792901)
 
 
+Tips & Tricks
+=============
+
+How to change label of the progress widget
+------------------------------------------
+
+::
+
+    >>> import frogress
+    >>> items = [1, 2, 3, 4, 5]
+    >>> widgets = [frogress.BarWidget, frogress.ProgressWidget('Items: '), frogress.TimerWidget]
+    >>> for item in frogress.bar(items, widgets=widgets):
+    >>>     pass
 
 
 .. _lxml: http://lxml.de/
```

### Comparing `frogress-0.9.0/setup.py` & `frogress-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     sys.stderr.write("[ERROR] Cannot find file specified as "
         "long_description (%s)\n" % readme_file)
     sys.exit(1)
 
 extra_kwargs = {'tests_require': ['mock>1.0']}
 if sys.version_info < (2, 7):
     extra_kwargs['tests_require'].append('unittest2')
-if sys.version_info >= (3,):
-    extra_kwargs['use_2to3'] = True
 
 frogress = __import__('frogress')
 
 setup(
     name='frogress',
     version=frogress.get_version(),
     url='https://github.com/lukaszb/frogress',
```

