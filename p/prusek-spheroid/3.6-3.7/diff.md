# Comparing `tmp/prusek_spheroid-3.6.tar.gz` & `tmp/prusek_spheroid-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-3.6.tar", last modified: Thu Apr  4 17:20:11 2024, max compression
+gzip compressed data, was "prusek_spheroid-3.7.tar", last modified: Thu Apr  4 17:37:03 2024, max compression
```

## Comparing `prusek_spheroid-3.6.tar` & `prusek_spheroid-3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:20:11.062619 prusek_spheroid-3.6/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-04 17:20:11.062224 prusek_spheroid-3.6/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.6/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:20:11.060922 prusek_spheroid-3.6/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    17715 2024-04-04 06:15:38.000000 prusek_spheroid-3.6/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    44718 2024-04-04 17:15:00.000000 prusek_spheroid-3.6/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.6/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.6/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-3.6/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-3.6/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     6737 2024-04-04 14:40:14.000000 prusek_spheroid-3.6/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3641 2024-04-03 14:52:18.000000 prusek_spheroid-3.6/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-3.6/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.6/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:20:11.062013 prusek_spheroid-3.6/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      544 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-04 17:20:11.062661 prusek_spheroid-3.6/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-04 17:19:48.000000 prusek_spheroid-3.6/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:37:03.764314 prusek_spheroid-3.7/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-04 17:37:03.764070 prusek_spheroid-3.7/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.7/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:37:03.763062 prusek_spheroid-3.7/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    17332 2024-04-04 17:31:23.000000 prusek_spheroid-3.7/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    44627 2024-04-04 17:30:32.000000 prusek_spheroid-3.7/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.7/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.7/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-3.7/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-3.7/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     6737 2024-04-04 14:40:14.000000 prusek_spheroid-3.7/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3641 2024-04-03 14:52:18.000000 prusek_spheroid-3.7/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-3.7/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-3.7/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:37:03.763872 prusek_spheroid-3.7/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-04 17:37:03.000000 prusek_spheroid-3.7/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      544 2024-04-04 17:37:03.000000 prusek_spheroid-3.7/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-04 17:37:03.000000 prusek_spheroid-3.7/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-04 17:37:03.000000 prusek_spheroid-3.7/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-04 17:37:03.000000 prusek_spheroid-3.7/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-04 17:37:03.764363 prusek_spheroid-3.7/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-04 17:36:56.000000 prusek_spheroid-3.7/setup.py
```

### Comparing `prusek_spheroid-3.6/PKG-INFO` & `prusek_spheroid-3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.6
+Version: 3.7
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.6/README.md` & `prusek_spheroid-3.7/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-3.7/prusek_spheroid/ContoursClassGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,19 +126,14 @@
                                 grandparent_index = hierarchy[0][parent_index][3]
 
                                 if grandparent_index == -1:
                                     # Kontura s jedním předkem - vnitřní kontura
                                     cv.drawContours(img_with, [contour], -1, (255, 0, 0),
                                                     2)  # Modře pro vnitřní kontury
                                     inner_contours.append(contour)
-                                else:
-                                    # Kontura s dvěma předky - potomek vnitřní kontury
-                                    cv.drawContours(img_with, [contour], -1, (0, 0, 255),
-                                                    2)  # Zeleně pro potomky vnitřních kontur
-                                    outer_contours.append(contour)
 
                     if len(outer_contours) == 0:
                         outer_contours = contours
 
                     for index, contour in enumerate(outer_contours):
                         if not self.contours_state == "all":
                             cv.drawContours(img_without, [contour], -1, [0, 0, 255], 2)
```

### Comparing `prusek_spheroid-3.6/prusek_spheroid/GUI.py` & `prusek_spheroid-3.7/prusek_spheroid/GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from prusek_spheroid import characteristic_functions as cf
 from prusek_spheroid import file_management as fm
 from prusek_spheroid import conversion as c
 import pandas as pd
 import cv2 as cv
 from tkinter import Toplevel, Label
 from tkinter import ttk
-import sys
 
 
 
 class SelectionDialog:
     def __init__(self, root):
         self.root = root
         self.dialog = tk.Toplevel(root)
@@ -716,17 +715,15 @@
         self.stop_event = threading.Event()
 
     def go_back(self):
         self.dialog.destroy()
         self.selection_dialog.show()
 
     def on_close(self):
-        # Signal all threads to stop by setting the event
-        self.stop_event.set()
-        sys.exit()
+        self.dialog.quit()
 
     def get_contours_state(self):
         if self.detect_outer_var.get() == 1:
             return "no"
         elif self.detect_all_var.get() == 1:
             return "all"
         else:
```

### Comparing `prusek_spheroid-3.6/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-3.7/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-3.7/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/prusek_spheroid/conversion.py` & `prusek_spheroid-3.7/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/prusek_spheroid/file_management.py` & `prusek_spheroid-3.7/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/prusek_spheroid/image_processing.py` & `prusek_spheroid-3.7/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/prusek_spheroid/methods.py` & `prusek_spheroid-3.7/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/prusek_spheroid/metrics.py` & `prusek_spheroid-3.7/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-3.7/prusek_spheroid/selection_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,18 @@
         self.photo1 = None
         self.photo2 = None
         self.image_label1 = None
         self.image_label2 = None
 
         self.create_selection_dialog()
 
+        self.master.protocol("WM_DELETE_WINDOW", self.on_close)
+
+    def on_close(self):
+        self.master.quit()  # Toto ukončí celý program
     def create_selection_dialog(self):
         if self.selection_dialog:
             self.selection_dialog.destroy()
 
         initial_width = 1040
         initial_height = 520
         self.selection_dialog = Toplevel(self.master)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prusek_spheroid-3.6/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-3.7/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.6
+Version: 3.7
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.6/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-3.7/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.6/setup.py` & `prusek_spheroid-3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="3.6",
+    version="3.7",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

