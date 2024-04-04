# Comparing `tmp/frameutils-0.1.8.tar.gz` & `tmp/frameutils-0.1.9.tar.gz`

## Comparing `frameutils-0.1.8.tar` & `frameutils-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 frameutils-0.1.8/.DS_Store
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 frameutils-0.1.8/README.md
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 frameutils-0.1.8/license.md
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 frameutils-0.1.8/.vscode/tasks.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 frameutils-0.1.8/src/frameutils/__init__.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 frameutils-0.1.8/src/frameutils/bluetooth.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 frameutils-0.1.8/src/frameutils/cli.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 frameutils-0.1.8/src/frameutils/create_sprites.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 frameutils-0.1.8/tests/test_bluetooth.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 frameutils-0.1.8/.gitignore
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 frameutils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 frameutils-0.1.8/readme.md
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 frameutils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 frameutils-0.1.9/.DS_Store
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 frameutils-0.1.9/README.md
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 frameutils-0.1.9/license.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 frameutils-0.1.9/.vscode/tasks.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 frameutils-0.1.9/src/frameutils/__init__.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 frameutils-0.1.9/src/frameutils/bluetooth.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 frameutils-0.1.9/src/frameutils/cli.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 frameutils-0.1.9/src/frameutils/create_sprites.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 frameutils-0.1.9/tests/test_bluetooth.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 frameutils-0.1.9/.gitignore
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 frameutils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 frameutils-0.1.9/readme.md
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 frameutils-0.1.9/PKG-INFO
```

### Comparing `frameutils-0.1.8/.DS_Store` & `frameutils-0.1.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `frameutils-0.1.8/README.md` & `frameutils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `frameutils-0.1.8/license.md` & `frameutils-0.1.9/license.md`

 * *Files identical despite different names*

### Comparing `frameutils-0.1.8/.vscode/tasks.json` & `frameutils-0.1.9/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `frameutils-0.1.8/src/frameutils/bluetooth.py` & `frameutils-0.1.9/src/frameutils/bluetooth.py`

 * *Files identical despite different names*

### Comparing `frameutils-0.1.8/src/frameutils/cli.py` & `frameutils-0.1.9/src/frameutils/cli.py`

 * *Files identical despite different names*

### Comparing `frameutils-0.1.8/src/frameutils/create_sprites.py` & `frameutils-0.1.9/src/frameutils/create_sprites.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,57 +75,60 @@
     img = np.array(Image.open(image_path))
 
     # img[:,:,:3] is img without alpha channel
     shape = img.shape
     flat_image = img[:, :, :3].reshape((shape[0] * shape[1], 3))
 
     # If space character, skip clustering, return all zeros
-    if (utf8_codepoint == 0x20):
+    if utf8_codepoint == 0x20:
         byte_list = [0] * (shape[0] * shape[1])
 
         color_mode = "SPRITE_" + str(colors) + "_COLORS"
 
         return (
             FontMetadata(
                 utf8_codepoint,
                 shape[1],
                 shape[0],
                 color_mode,
                 len(byte_list),
             ),
             byte_list,
         )
-        
+
     kmeans = KMeans(n_clusters=colors, random_state=0, n_init="auto").fit(flat_image)
 
     palleted_img = kmeans.predict(flat_image).astype(np.uint8)
 
     # if black is not at index 0, swap it
-    black_code = kmeans.predict(np.array([255, 255, 255]).reshape(1, -1))
+    black_code = kmeans.predict(np.array([0, 0, 0]).reshape(1, -1))[0]
+
     if black_code != 0:
-        np.put(palleted_img, [0, 1], [1, 0])
+        masked_black_code = palleted_img == black_code
+        masked_0 = palleted_img == 0
+        palleted_img[masked_black_code] = 0
+        palleted_img[masked_0] = black_code
 
     # debug = palleted_img.reshape((shape[0], shape[1]))
-    # print('\n'.join([''.join(['{:2}'.format(item) for item in row])
-    #     for row in debug]))
+    # print("\n".join(["".join(["{:2}".format(item) for item in row]) for row in debug]))
 
     bits_per_pixel = int(math.sqrt(colors))
 
     byte_list = []
     pixels_per_byte = int(8 / bits_per_pixel)
     current_byte = 0
     pixels_left_in_byte = pixels_per_byte
     mask = colors - 1
 
     for idx, pixel in enumerate(palleted_img):
         masked_value = pixel & mask
         if pixels_left_in_byte > 0:
             current_byte += masked_value << ((pixels_left_in_byte - 1) * bits_per_pixel)
             pixels_left_in_byte -= 1
-            if (idx == len(palleted_img)-1):
+            if idx == len(palleted_img) - 1:
                 byte_list.append(current_byte)
         else:
             pixels_left_in_byte = pixels_per_byte - 1
             byte_list.append(current_byte)
             current_byte = masked_value << ((pixels_left_in_byte - 1) * bits_per_pixel)
 
     # write last byte if necessary
```

### Comparing `frameutils-0.1.8/tests/test_bluetooth.py` & `frameutils-0.1.9/tests/test_bluetooth.py`

 * *Files identical despite different names*

### Comparing `frameutils-0.1.8/pyproject.toml` & `frameutils-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "frameutils"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{ name = "Brilliant Labs", email = "info@brilliant.xyz" }]
 description = "Useful utilities for your Brilliant Frame AR glasses"
 readme = "readme.md"
 requires-python = ">=3.7"
 license = { file = "license.md" }
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `frameutils-0.1.8/readme.md` & `frameutils-0.1.9/readme.md`

 * *Files identical despite different names*

### Comparing `frameutils-0.1.8/PKG-INFO` & `frameutils-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frameutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Useful utilities for your Brilliant Frame AR glasses
 Project-URL: Homepage, https://github.com/brilliantlabsAR/frame-utilities-for-python
 Project-URL: Bug Tracker, https://github.com/brilliantlabsAR/frame-utilities-for-python/issues
 Author-email: Brilliant Labs <info@brilliant.xyz>
 License: ISC License
         
         Copyright © 2023 Brilliant Labs Ltd.
```

