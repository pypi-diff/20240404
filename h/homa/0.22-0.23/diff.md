# Comparing `tmp/homa-0.22.tar.gz` & `tmp/homa-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homa-0.22.tar", last modified: Thu Apr  4 12:24:10 2024, max compression
+gzip compressed data, was "homa-0.23.tar", last modified: Thu Apr  4 15:53:23 2024, max compression
```

## Comparing `homa-0.22.tar` & `homa-0.23.tar`

### file list

```diff
@@ -1,25 +1,36 @@
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 12:24:10.499815 homa-0.22/
--rw-r--r--   0 taha       (501) staff       (20)     1072 2024-03-27 20:05:25.000000 homa-0.22/LICENSE
--rw-r--r--   0 taha       (501) staff       (20)     2011 2024-04-04 12:24:10.499641 homa-0.22/PKG-INFO
--rw-r--r--   0 taha       (501) staff       (20)     1830 2024-04-04 12:21:43.000000 homa-0.22/README.md
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 12:24:10.496970 homa-0.22/homa/
--rw-r--r--   0 taha       (501) staff       (20)       92 2024-04-04 10:37:31.000000 homa-0.22/homa/__init__.py
--rw-r--r--   0 taha       (501) staff       (20)      391 2024-04-04 11:00:35.000000 homa-0.22/homa/camera.py
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 12:24:10.499431 homa-0.22/homa/classes/
--rw-r--r--   0 taha       (501) staff       (20)      222 2024-04-03 16:22:17.000000 homa-0.22/homa/classes/Collection.py
--rw-r--r--   0 taha       (501) staff       (20)       93 2024-04-03 16:33:06.000000 homa-0.22/homa/classes/Logger.py
--rw-r--r--   0 taha       (501) staff       (20)      705 2024-04-03 21:57:58.000000 homa-0.22/homa/classes/Repository.py
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 21:21:15.000000 homa-0.22/homa/classes/__init__.py
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 15:09:00.000000 homa-0.22/homa/constants.py
--rw-r--r--   0 taha       (501) staff       (20)      821 2024-04-04 11:15:16.000000 homa-0.22/homa/filters.py
--rw-r--r--   0 taha       (501) staff       (20)      593 2024-04-04 11:14:46.000000 homa-0.22/homa/helpers.py
--rw-r--r--   0 taha       (501) staff       (20)     1346 2024-04-04 12:07:54.000000 homa-0.22/homa/main.py
--rw-r--r--   0 taha       (501) staff       (20)      749 2024-04-04 12:08:41.000000 homa-0.22/homa/orientation.py
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 12:24:10.498124 homa-0.22/homa.egg-info/
--rw-r--r--   0 taha       (501) staff       (20)     2011 2024-04-04 12:24:10.000000 homa-0.22/homa.egg-info/PKG-INFO
--rw-r--r--   0 taha       (501) staff       (20)      382 2024-04-04 12:24:10.000000 homa-0.22/homa.egg-info/SOURCES.txt
--rw-r--r--   0 taha       (501) staff       (20)        1 2024-04-04 12:24:10.000000 homa-0.22/homa.egg-info/dependency_links.txt
--rw-r--r--   0 taha       (501) staff       (20)       20 2024-04-04 12:24:10.000000 homa-0.22/homa.egg-info/requires.txt
--rw-r--r--   0 taha       (501) staff       (20)        5 2024-04-04 12:24:10.000000 homa-0.22/homa.egg-info/top_level.txt
--rw-r--r--   0 taha       (501) staff       (20)       38 2024-04-04 12:24:10.499882 homa-0.22/setup.cfg
--rw-r--r--   0 taha       (501) staff       (20)      671 2024-04-03 21:59:07.000000 homa-0.22/setup.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 15:53:23.008153 homa-0.23/
+-rw-r--r--   0 taha       (501) staff       (20)     1072 2024-03-27 20:05:25.000000 homa-0.23/LICENSE
+-rw-r--r--   0 taha       (501) staff       (20)     2021 2024-04-04 15:53:23.007931 homa-0.23/PKG-INFO
+-rw-r--r--   0 taha       (501) staff       (20)     1840 2024-04-04 12:25:51.000000 homa-0.23/README.md
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 15:53:23.002451 homa-0.23/homa/
+-rw-r--r--   0 taha       (501) staff       (20)      182 2024-04-04 15:42:04.000000 homa-0.23/homa/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)      464 2024-04-04 13:08:57.000000 homa-0.23/homa/camera.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 15:53:23.005083 homa-0.23/homa/classes/
+-rw-r--r--   0 taha       (501) staff       (20)      222 2024-04-03 16:22:17.000000 homa-0.23/homa/classes/Collection.py
+-rw-r--r--   0 taha       (501) staff       (20)       93 2024-04-03 16:33:06.000000 homa-0.23/homa/classes/Logger.py
+-rw-r--r--   0 taha       (501) staff       (20)      589 2024-04-04 15:46:34.000000 homa-0.23/homa/classes/Repository.py
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 21:21:15.000000 homa-0.23/homa/classes/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 15:09:00.000000 homa-0.23/homa/constants.py
+-rw-r--r--   0 taha       (501) staff       (20)     1946 2024-04-04 15:39:07.000000 homa-0.23/homa/events.py
+-rw-r--r--   0 taha       (501) staff       (20)     1058 2024-04-04 14:28:59.000000 homa-0.23/homa/filters.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 15:53:23.006686 homa-0.23/homa/helpers/
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-04 13:55:31.000000 homa-0.23/homa/helpers/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)      288 2024-04-04 14:12:22.000000 homa-0.23/homa/helpers/alias.py
+-rw-r--r--   0 taha       (501) staff       (20)       78 2024-04-04 13:53:19.000000 homa-0.23/homa/helpers/environment.py
+-rw-r--r--   0 taha       (501) staff       (20)      330 2024-04-04 13:56:06.000000 homa-0.23/homa/helpers/kernel.py
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-04 13:56:03.000000 homa-0.23/homa/helpers.py
+-rw-r--r--   0 taha       (501) staff       (20)     1774 2024-04-04 15:52:39.000000 homa-0.23/homa/main.py
+-rw-r--r--   0 taha       (501) staff       (20)      804 2024-04-04 13:57:15.000000 homa-0.23/homa/orientation.py
+-rw-r--r--   0 taha       (501) staff       (20)      283 2024-04-04 15:52:49.000000 homa-0.23/homa/shapes.py
+-rw-r--r--   0 taha       (501) staff       (20)      460 2024-04-04 13:55:28.000000 homa-0.23/homa/spaces.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 15:53:23.003548 homa-0.23/homa.egg-info/
+-rw-r--r--   0 taha       (501) staff       (20)     2021 2024-04-04 15:53:22.000000 homa-0.23/homa.egg-info/PKG-INFO
+-rw-r--r--   0 taha       (501) staff       (20)      564 2024-04-04 15:53:22.000000 homa-0.23/homa.egg-info/SOURCES.txt
+-rw-r--r--   0 taha       (501) staff       (20)        1 2024-04-04 15:53:22.000000 homa-0.23/homa.egg-info/dependency_links.txt
+-rw-r--r--   0 taha       (501) staff       (20)       20 2024-04-04 15:53:22.000000 homa-0.23/homa.egg-info/requires.txt
+-rw-r--r--   0 taha       (501) staff       (20)       11 2024-04-04 15:53:22.000000 homa-0.23/homa.egg-info/top_level.txt
+-rw-r--r--   0 taha       (501) staff       (20)       38 2024-04-04 15:53:23.008229 homa-0.23/setup.cfg
+-rw-r--r--   0 taha       (501) staff       (20)      671 2024-04-03 21:59:07.000000 homa-0.23/setup.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 15:53:23.007477 homa-0.23/tests/
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-04 14:06:35.000000 homa-0.23/tests/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)      772 2024-04-04 14:23:48.000000 homa-0.23/tests/test_images.py
```

### Comparing `homa-0.22/LICENSE` & `homa-0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `homa-0.22/PKG-INFO` & `homa-0.23/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homa
-Version: 0.22
+Version: 0.23
 Maintainer: Taha Shieenavaz
 Maintainer-email: tahashieenavaz@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 	<img
@@ -43,28 +43,30 @@
 from homa import *
 
 image("horse.jpg")
 
 blur("horse", 7)                    # rewrites "horse" key
 blur("horse", (7, 19))              # rewrites "horse" key
 blur("horse", 9, "blurred horse")   # as a new key in the repository
-show("blurred horse")
+
+showWait("blurred horse")
 ```
 
 ### Gaussian Blur
 
 ```python
 from homa import *
 
 image("horse.jpg")
 
 gaussian("horse", 7)                             # rewrites "horse" key
 gaussian("horse", (7, 19))                       # rewrites "horse" key
 gaussian("horse", 9, "gaussian blurred horse")   # as a new key in the repository
-show("gaussian blurred horse")
+
+showWait("gaussian blurred horse")
 ```
 
 ## Stacking
 
 ```python
 from homa import *
```

### Comparing `homa-0.22/README.md` & `homa-0.23/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,28 +35,30 @@
 from homa import *
 
 image("horse.jpg")
 
 blur("horse", 7)                    # rewrites "horse" key
 blur("horse", (7, 19))              # rewrites "horse" key
 blur("horse", 9, "blurred horse")   # as a new key in the repository
-show("blurred horse")
+
+showWait("blurred horse")
 ```
 
 ### Gaussian Blur
 
 ```python
 from homa import *
 
 image("horse.jpg")
 
 gaussian("horse", 7)                             # rewrites "horse" key
 gaussian("horse", (7, 19))                       # rewrites "horse" key
 gaussian("horse", 9, "gaussian blurred horse")   # as a new key in the repository
-show("gaussian blurred horse")
+
+showWait("gaussian blurred horse")
 ```
 
 ## Stacking
 
 ```python
 from homa import *
```

### Comparing `homa-0.22/homa/classes/Repository.py` & `homa-0.23/homa/classes/Repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-from ..helpers import is_colab
+from ..helpers.environment import is_colab
 
 
 class RepositoryWrapper:
     def __init__(self):
         self.sigmaX = 0
         self.sigmaY = 0
 
         self.directory = "./"
         self.images = {}
-        self.cameras = {}
-        self.window_counter = 0
+        self.windows = {}
 
         if is_colab():
             from google.colab.patches import cv2_imshow as imshow
         else:
             from cv2 import imshow
 
         def final_imshow(window, image):
             if is_colab():
                 imshow(image)
             else:
                 imshow(window, image)
 
         self.imshow = final_imshow
 
-    def get_counter(self):
-        self.window_counter += 1
-        return self.window_counter
-
 
 Repository = RepositoryWrapper()
```

### Comparing `homa-0.22/homa/filters.py` & `homa-0.23/homa/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from typing import List
 from .classes.Repository import Repository
-from .helpers import create_kernel
+from .helpers.kernel import create_kernel
 import cv2
 
 
-def blur(key: str, kernel: int | List[int] = (7, 7), new_key: str | None = None):
+def blur(key: str, kernel: int | List[int] = (7, 7), new_key: str | None = None) -> None:
     if new_key is None:
         new_key = key
 
     Repository.images[new_key] = cv2.blur(
         Repository.images[key],
         create_kernel(kernel)
     )
 
 
-def sigma(x: float = 0, y: float = 0):
+def median(key: str, kernel: int | List[int] = (7, 7), new_key: str | None = None) -> None:
+    if new_key is None:
+        new_key = key
+
+    Repository.images[new_key] = cv2.medianBlur(
+        Repository.images[key],
+        create_kernel(kernel)
+    )
+
+
+def sigma(x: float = 0, y: float = 0) -> None:
     Repository.sigmaX = x
     Repository.sigmaY = y
 
 
-def gaussian(key: str, kernel: None | List[int] = None, new_key: str | None = None):
+def gaussian(key: str, kernel: None | List[int] = None, new_key: str | None = None) -> None:
     if new_key is None:
         new_key = key
 
-    if isinstance(kernel, int):
-        kernel = (kernel, kernel)
-
     Repository.images[new_key] = cv2.GaussianBlur(
         Repository.images[key],
-        kernel,
+        create_kernel(kernel),
         sigmaX=Repository.sigmaX,
         sigmaY=Repository.sigmaY
     )
```

### Comparing `homa-0.22/homa/main.py` & `homa-0.23/homa/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 import cv2
-from .helpers import danger
+from .classes.Logger import Logger
 from .classes.Repository import Repository
 
 
+def destroy(key: str | None = None) -> None:
+    if key is not None:
+        cv2.destroyWindow(key)
+        return
+
+    cv2.destroyAllWindows()
+
+
+def win(key: str):
+    cv2.namedWindow(key)
+
+
 def path(directory: str) -> None:
     Repository.directory = directory
 
 
 def write(key: str, filename: str) -> None:
     cv2.imwrite(
         filename=filename,
@@ -37,20 +49,27 @@
 
 
 def show(key: any = None, wait: bool = False, window: str = "Homa Window") -> None:
     # TODO: add functionality to distinguish between camera and images
 
     if key is not None and not isinstance(key, str):
         Repository.imshow(window, key)
+        Repository.windows[key] = window
 
     elif key is None:
         for key, image in Repository.images.items():
             Repository.imshow(key, image)
+            Repository.windows[key] = key
 
     elif key is not None:
         if key in Repository.images:
             Repository.imshow(key, Repository.images[key])
+            Repository.windows[key] = key
         else:
-            danger(f"No image found with key {key}")
+            Logger.danger(f"No image found with key {key}")
 
     if wait:
         cv2.waitKey(0)
+
+
+def refresh(key: str) -> None:
+    cv2.imshow(Repository.windows[key], Repository.images[key])
```

### Comparing `homa-0.22/homa.egg-info/PKG-INFO` & `homa-0.23/homa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homa
-Version: 0.22
+Version: 0.23
 Maintainer: Taha Shieenavaz
 Maintainer-email: tahashieenavaz@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 	<img
@@ -43,28 +43,30 @@
 from homa import *
 
 image("horse.jpg")
 
 blur("horse", 7)                    # rewrites "horse" key
 blur("horse", (7, 19))              # rewrites "horse" key
 blur("horse", 9, "blurred horse")   # as a new key in the repository
-show("blurred horse")
+
+showWait("blurred horse")
 ```
 
 ### Gaussian Blur
 
 ```python
 from homa import *
 
 image("horse.jpg")
 
 gaussian("horse", 7)                             # rewrites "horse" key
 gaussian("horse", (7, 19))                       # rewrites "horse" key
 gaussian("horse", 9, "gaussian blurred horse")   # as a new key in the repository
-show("gaussian blurred horse")
+
+showWait("gaussian blurred horse")
 ```
 
 ## Stacking
 
 ```python
 from homa import *
```

### Comparing `homa-0.22/setup.py` & `homa-0.23/setup.py`

 * *Files identical despite different names*

