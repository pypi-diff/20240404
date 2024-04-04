# Comparing `tmp/pytritech-1.0.1.tar.gz` & `tmp/pytritech-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytritech-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytritech-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytritech-1.0.1.tar` & `pytritech-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2049 2024-02-15 14:06:57.535656 pytritech-1.0.1/README.md
--rwxr-xr-x   0        0        0     1135 2024-02-15 16:14:35.278488 pytritech-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 14:06:57.535656 pytritech-1.0.1/src/pytritech/__init__.py
--rwxr-xr-x   0        0        0     2657 2024-02-15 16:12:05.398194 pytritech-1.0.1/src/pytritech/ciheader.py
--rwxr-xr-x   0        0        0     5265 2024-02-15 16:12:05.398194 pytritech-1.0.1/src/pytritech/glf.py
--rw-r--r--   0        0        0     3126 2024-02-15 16:12:06.164863 pytritech-1.0.1/src/pytritech/glftimes.py
--rwxr-xr-x   0        0        0     6530 2024-02-15 16:12:06.454863 pytritech-1.0.1/src/pytritech/image.py
--rwxr-xr-x   0        0        0     6492 2024-02-15 16:12:05.394861 pytritech-1.0.1/src/pytritech/status.py
--rw-r--r--   0        0        0      871 2024-02-15 16:13:52.418404 pytritech-1.0.1/src/pytritech/util/range.py
--rwxr-xr-x   0        0        0      420 2024-02-15 14:40:55.303174 pytritech-1.0.1/src/pytritech/util/time.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 pytritech-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2049 2024-02-13 10:55:34.510024 pytritech-1.0.2/README.md
+-rwxr-xr-x   0        0        0     1136 2024-04-04 15:03:01.336618 pytritech-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-12 15:54:16.736503 pytritech-1.0.2/src/pytritech/__init__.py
+-rwxr-xr-x   0        0        0     2657 2024-04-04 14:52:23.780214 pytritech-1.0.2/src/pytritech/ciheader.py
+-rwxr-xr-x   0        0        0     5572 2024-04-04 14:52:23.780214 pytritech-1.0.2/src/pytritech/glf.py
+-rw-r--r--   0        0        0     3126 2024-04-04 14:52:23.780214 pytritech-1.0.2/src/pytritech/glftimes.py
+-rwxr-xr-x   0        0        0     6530 2024-04-04 14:52:23.780214 pytritech-1.0.2/src/pytritech/image.py
+-rwxr-xr-x   0        0        0     6492 2024-04-04 14:52:23.780214 pytritech-1.0.2/src/pytritech/status.py
+-rw-r--r--   0        0        0      871 2024-04-04 14:52:23.780214 pytritech-1.0.2/src/pytritech/util/range.py
+-rwxr-xr-x   0        0        0      420 2024-04-04 14:52:23.780214 pytritech-1.0.2/src/pytritech/util/time.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 pytritech-1.0.2/PKG-INFO
```

### Comparing `pytritech-1.0.1/README.md` & `pytritech-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pytritech-1.0.1/pyproject.toml` & `pytritech-1.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pytritech"
 description = "A Python interface to Tritech Gemini Sonar files."
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "Benjamin James Blundell", email = "me@benjamin.computer" }
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -46,8 +46,8 @@
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project.urls]
 "Homepage" = "https://github.com/onidaito/pytritech"
-"Bug Tracker" = "https://github.com/onidaito/pytritech/issues"
+"Bug Tracker" = "https://github.com/onidaito/pytritech/issues"
```

### Comparing `pytritech-1.0.1/src/pytritech/ciheader.py` & `pytritech-1.0.2/src/pytritech/ciheader.py`

 * *Files identical despite different names*

### Comparing `pytritech-1.0.1/src/pytritech/glf.py` & `pytritech-1.0.2/src/pytritech/glf.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,18 +61,19 @@
                     cfg = cfg.replace("</1>", "</one>")
 
                     root = ET.fromstring(cfg)
                     self.config = root
 
         # Set some useful parameters on the GLF class such as sonar_id and range
         # TODO - it turns out that the range text doesn't always exist and there may be multiple ones
-        self.sonar_ids = []
+        #self.sonar_ids = []
 
-        for sonar_node in root.find("GuiCurrentSettings/devices"):
-            self.sonar_ids.append(int(sonar_node.find("id").text))
+        # This method appears not to work
+        #for sonar_node in root.find("GuiCurrentSettings/devices"):
+        #    self.sonar_ids.append(int(sonar_node.find("id").text))
 
     
     def __enter__(self):
         self._zobject = ZipFile(self.filepath, "r")
         
         for zname in self._zobject.namelist():
             if ".dat" in zname:
@@ -114,28 +115,36 @@
             assert False
 
         return image_data, image_rec.image_dim
 
     def _parse_dat(self):
         """Read the dat file stored inside the glf which uses Zip."""
         self.images = []
+        self.sonar_ids = []
         self.dat = self._f.read()
         file_offset = 0
 
         # We should get towards the last bytes, both of which
         # should be DEDE
         while file_offset < len(self.dat) - 2:
             header = CIHeader(self.dat, file_offset)
             file_offset += len(header)
 
             if header.type == 0:
                 # image record
                 image_rec = ImageRecord(header, self.dat, file_offset)
                 self.images.append(image_rec)
                 file_offset += len(image_rec)
+
+                # Add sonar IDs here as we find them. Seems the best way.
+                sonar_id = image_rec.header.device_id
+
+                if sonar_id not in self.sonar_ids:
+                    self.sonar_ids.append(sonar_id)
+
             elif header.type == 1:
                 # V4 protocol
                 assert False
                 break
             elif header.type == 2:
                 # analog video
                 assert False
```

### Comparing `pytritech-1.0.1/src/pytritech/glftimes.py` & `pytritech-1.0.2/src/pytritech/glftimes.py`

 * *Files identical despite different names*

### Comparing `pytritech-1.0.1/src/pytritech/image.py` & `pytritech-1.0.2/src/pytritech/image.py`

 * *Files identical despite different names*

### Comparing `pytritech-1.0.1/src/pytritech/status.py` & `pytritech-1.0.2/src/pytritech/status.py`

 * *Files identical despite different names*

### Comparing `pytritech-1.0.1/src/pytritech/util/range.py` & `pytritech-1.0.2/src/pytritech/util/range.py`

 * *Files identical despite different names*

### Comparing `pytritech-1.0.1/PKG-INFO` & `pytritech-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytritech
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python interface to Tritech Gemini Sonar files.
 Author-email: Benjamin James Blundell <me@benjamin.computer>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
```

