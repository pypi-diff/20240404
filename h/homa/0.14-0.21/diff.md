# Comparing `tmp/homa-0.14.tar.gz` & `tmp/homa-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homa-0.14.tar", last modified: Wed Apr  3 21:44:42 2024, max compression
+gzip compressed data, was "homa-0.21.tar", last modified: Wed Apr  3 22:01:46 2024, max compression
```

## Comparing `homa-0.14.tar` & `homa-0.21.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-03 21:44:42.822756 homa-0.14/
--rw-r--r--   0 taha       (501) staff       (20)     1072 2024-03-27 20:05:25.000000 homa-0.14/LICENSE
--rw-r--r--   0 taha       (501) staff       (20)      315 2024-04-03 21:44:42.822583 homa-0.14/PKG-INFO
--rw-r--r--   0 taha       (501) staff       (20)      134 2024-04-03 21:17:30.000000 homa-0.14/README.md
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-03 21:44:42.820098 homa-0.14/homa/
--rw-r--r--   0 taha       (501) staff       (20)       20 2024-04-03 20:43:26.000000 homa-0.14/homa/__init__.py
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-03 21:44:42.822338 homa-0.14/homa/classes/
--rw-r--r--   0 taha       (501) staff       (20)      222 2024-04-03 16:22:17.000000 homa-0.14/homa/classes/Collection.py
--rw-r--r--   0 taha       (501) staff       (20)       93 2024-04-03 16:33:06.000000 homa-0.14/homa/classes/Logger.py
--rw-r--r--   0 taha       (501) staff       (20)      603 2024-04-03 21:36:30.000000 homa-0.14/homa/classes/Repository.py
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 21:21:15.000000 homa-0.14/homa/classes/__init__.py
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 15:09:00.000000 homa-0.14/homa/constants.py
--rw-r--r--   0 taha       (501) staff       (20)      308 2024-04-03 16:34:11.000000 homa-0.14/homa/helpers.py
--rw-r--r--   0 taha       (501) staff       (20)     2708 2024-04-03 21:44:13.000000 homa-0.14/homa/main.py
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-03 21:44:42.821226 homa-0.14/homa.egg-info/
--rw-r--r--   0 taha       (501) staff       (20)      315 2024-04-03 21:44:42.000000 homa-0.14/homa.egg-info/PKG-INFO
--rw-r--r--   0 taha       (501) staff       (20)      331 2024-04-03 21:44:42.000000 homa-0.14/homa.egg-info/SOURCES.txt
--rw-r--r--   0 taha       (501) staff       (20)        1 2024-04-03 21:44:42.000000 homa-0.14/homa.egg-info/dependency_links.txt
--rw-r--r--   0 taha       (501) staff       (20)       20 2024-04-03 21:44:42.000000 homa-0.14/homa.egg-info/requires.txt
--rw-r--r--   0 taha       (501) staff       (20)        5 2024-04-03 21:44:42.000000 homa-0.14/homa.egg-info/top_level.txt
--rw-r--r--   0 taha       (501) staff       (20)       38 2024-04-03 21:44:42.822827 homa-0.14/setup.cfg
--rw-r--r--   0 taha       (501) staff       (20)      671 2024-04-03 21:41:33.000000 homa-0.14/setup.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-03 22:01:46.187515 homa-0.21/
+-rw-r--r--   0 taha       (501) staff       (20)     1072 2024-03-27 20:05:25.000000 homa-0.21/LICENSE
+-rw-r--r--   0 taha       (501) staff       (20)      315 2024-04-03 22:01:46.187342 homa-0.21/PKG-INFO
+-rw-r--r--   0 taha       (501) staff       (20)      134 2024-04-03 21:17:30.000000 homa-0.21/README.md
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-03 22:01:46.185296 homa-0.21/homa/
+-rw-r--r--   0 taha       (501) staff       (20)       20 2024-04-03 20:43:26.000000 homa-0.21/homa/__init__.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-03 22:01:46.187061 homa-0.21/homa/classes/
+-rw-r--r--   0 taha       (501) staff       (20)      222 2024-04-03 16:22:17.000000 homa-0.21/homa/classes/Collection.py
+-rw-r--r--   0 taha       (501) staff       (20)       93 2024-04-03 16:33:06.000000 homa-0.21/homa/classes/Logger.py
+-rw-r--r--   0 taha       (501) staff       (20)      705 2024-04-03 21:57:58.000000 homa-0.21/homa/classes/Repository.py
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 21:21:15.000000 homa-0.21/homa/classes/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 15:09:00.000000 homa-0.21/homa/constants.py
+-rw-r--r--   0 taha       (501) staff       (20)      308 2024-04-03 16:34:11.000000 homa-0.21/homa/helpers.py
+-rw-r--r--   0 taha       (501) staff       (20)     2618 2024-04-03 21:56:17.000000 homa-0.21/homa/main.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-03 22:01:46.186231 homa-0.21/homa.egg-info/
+-rw-r--r--   0 taha       (501) staff       (20)      315 2024-04-03 22:01:46.000000 homa-0.21/homa.egg-info/PKG-INFO
+-rw-r--r--   0 taha       (501) staff       (20)      331 2024-04-03 22:01:46.000000 homa-0.21/homa.egg-info/SOURCES.txt
+-rw-r--r--   0 taha       (501) staff       (20)        1 2024-04-03 22:01:46.000000 homa-0.21/homa.egg-info/dependency_links.txt
+-rw-r--r--   0 taha       (501) staff       (20)       20 2024-04-03 22:01:46.000000 homa-0.21/homa.egg-info/requires.txt
+-rw-r--r--   0 taha       (501) staff       (20)        5 2024-04-03 22:01:46.000000 homa-0.21/homa.egg-info/top_level.txt
+-rw-r--r--   0 taha       (501) staff       (20)       38 2024-04-03 22:01:46.187593 homa-0.21/setup.cfg
+-rw-r--r--   0 taha       (501) staff       (20)      671 2024-04-03 21:59:07.000000 homa-0.21/setup.py
```

### Comparing `homa-0.14/LICENSE` & `homa-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `homa-0.14/homa/classes/Repository.py` & `homa-0.21/homa/classes/Repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,21 @@
         self.window_counter = 0
 
         if is_colab():
             from google.colab.patches import cv2_imshow as imshow
         else:
             from cv2 import imshow
 
-        self.imshow = imshow
+        def final_imshow(window, image):
+            if is_colab():
+                imshow(image)
+            else:
+                imshow(window, image)
+
+        self.imshow = final_imshow
 
     def get_counter(self):
         self.window_counter += 1
         return self.window_counter
 
-    def __getattr__(self, name: str) -> any:
-        pass
-
 
 Repository = RepositoryWrapper()
```

### Comparing `homa-0.14/homa/main.py` & `homa-0.21/homa/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,15 @@
     # TODO: add functionality to distinguish between camera and images
 
     if key is not None and not isinstance(key, str):
         Repository.imshow(f"Window #{Repository.get_counter()}", key)
 
     elif key is None:
         for key, image in Repository.images.items():
-            if is_colab():
-                Repository.imshow(image)
-            else:
-                Repository.imshow(key, image)
+            Repository.imshow(key, image)
 
     elif key is not None:
         if key in Repository.images:
             Repository.imshow(key, Repository.images[key])
         else:
             danger(f"No image found with key {key}")
```

### Comparing `homa-0.14/setup.py` & `homa-0.21/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 with open("README.md") as fh:
     description = fh.read()
 
 with open("version.txt", "r") as fh:
     current_version = float(fh.readline())
 
 with open("version.txt", "w") as fh:
-    next_version = current_version + 0.01
+    next_version = round(current_version + 0.01, 2)
     fh.write(str(next_version))
 
 setup(
     name="homa",
     maintainer="Taha Shieenavaz",
     maintainer_email="tahashieenavaz@gmail.com",
-    version=round(next_version, 2),
+    version=next_version,
     packages=find_packages(),
     install_requires=[
         "opencv-python",
         "numpy"
     ],
     long_description=description,
     long_description_content_type="text/markdown",
```

