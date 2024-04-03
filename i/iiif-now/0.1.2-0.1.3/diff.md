# Comparing `tmp/iiif_now-0.1.2.tar.gz` & `tmp/iiif_now-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iiif_now-0.1.2.tar", max compression
+gzip compressed data, was "iiif_now-0.1.3.tar", max compression
```

## Comparing `iiif_now-0.1.2.tar` & `iiif_now-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1034 2024-04-02 23:08:15.145289 iiif_now-0.1.2/README.md
--rw-r--r--   0        0        0      132 2024-04-02 22:30:01.698940 iiif_now-0.1.2/iiif_now/__init__.py
--rw-r--r--   0        0        0       33 2024-03-31 14:34:26.835751 iiif_now-0.1.2/iiif_now/csvreader/__init__.py
--rw-r--r--   0        0        0     3750 2024-04-02 17:08:11.973748 iiif_now-0.1.2/iiif_now/csvreader/csvreader.py
--rw-r--r--   0        0        0       34 2024-03-31 14:35:09.074716 iiif_now-0.1.2/iiif_now/datacanvas/__init__.py
--rw-r--r--   0        0        0     2033 2024-04-02 17:02:15.140123 iiif_now-0.1.2/iiif_now/datacanvas/datacanvas.py
--rw-r--r--   0        0        0      975 2024-04-02 23:02:06.414380 iiif_now-0.1.2/iiif_now/iiifnow.py
--rw-r--r--   0        0        0       32 2024-03-31 23:06:07.096746 iiif_now-0.1.2/iiif_now/manifest/__init__.py
--rw-r--r--   0        0        0     5796 2024-04-02 23:00:34.337219 iiif_now-0.1.2/iiif_now/manifest/manifest.py
--rw-r--r--   0        0        0       30 2024-04-02 22:30:01.682517 iiif_now-0.1.2/iiif_now/navplace/__init__.py
--rw-r--r--   0        0        0     2173 2024-04-02 22:33:08.662831 iiif_now-0.1.2/iiif_now/navplace/navplace.py
--rw-r--r--   0        0        0      483 2024-04-02 23:08:27.225706 iiif_now-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 iiif_now-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      280 2024-04-03 22:39:47.822765 iiif_now-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1096 2024-04-03 23:26:07.781593 iiif_now-0.1.3/README.md
+-rw-r--r--   0        0        0      165 2024-04-03 22:15:54.969000 iiif_now-0.1.3/iiif_now/__init__.py
+-rw-r--r--   0        0        0       33 2024-03-31 14:34:26.835751 iiif_now-0.1.3/iiif_now/csvreader/__init__.py
+-rw-r--r--   0        0        0     4520 2024-04-03 14:47:09.996938 iiif_now-0.1.3/iiif_now/csvreader/csvreader.py
+-rw-r--r--   0        0        0       34 2024-03-31 14:35:09.074716 iiif_now-0.1.3/iiif_now/datacanvas/__init__.py
+-rw-r--r--   0        0        0     2033 2024-04-03 15:22:16.528962 iiif_now-0.1.3/iiif_now/datacanvas/datacanvas.py
+-rw-r--r--   0        0        0      975 2024-04-02 23:02:06.414380 iiif_now-0.1.3/iiif_now/iiifnow.py
+-rw-r--r--   0        0        0       32 2024-03-31 23:06:07.096746 iiif_now-0.1.3/iiif_now/manifest/__init__.py
+-rw-r--r--   0        0        0     6038 2024-04-03 22:57:04.940434 iiif_now-0.1.3/iiif_now/manifest/manifest.py
+-rw-r--r--   0        0        0       30 2024-04-02 22:30:01.682517 iiif_now-0.1.3/iiif_now/navplace/__init__.py
+-rw-r--r--   0        0        0     2173 2024-04-02 22:33:08.662831 iiif_now-0.1.3/iiif_now/navplace/navplace.py
+-rw-r--r--   0        0        0       32 2024-04-03 22:15:54.948804 iiif_now-0.1.3/iiif_now/thumbnail/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-03 22:38:50.485206 iiif_now-0.1.3/iiif_now/thumbnail/thumbnail.py
+-rw-r--r--   0        0        0      593 2024-04-03 23:28:07.016844 iiif_now-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 iiif_now-0.1.3/PKG-INFO
```

### Comparing `iiif_now-0.1.2/README.md` & `iiif_now-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # IIIF Now
 
 ## About
 
 IIIF Manifest generation tools for the Abolition Now project.
 
+![Example Manifest](manifest_example.png "Example Manifest")
+
 ## Installation
 
 ```bash
 pip install iiif-now
 ```
 
 ## Configuration
```

### Comparing `iiif_now-0.1.2/iiif_now/csvreader/csvreader.py` & `iiif_now-0.1.3/iiif_now/csvreader/csvreader.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,23 +67,36 @@
                 }
                 hierarchy.append(canvas_dict)
 
             canvas = DataCanvas(row, self.artists, self.metadata)
             if canvas.parent_title != '':
                 canvas_dict['manifest_title'] = canvas.parent_title
             canvas_dict['canvases'].append(canvas.as_dict)
+            # @Todo: Does this need to be here with below?
             for artist in canvas.artists:
                 if artist not in canvas_dict['artists']:
                     canvas_dict['artists'].append(artist)
+            # @Todo: Break this into separate method
             if canvas.metadata:
                 for k, v in canvas.metadata.items():
                     if k not in canvas_dict['metadata']:
                         canvas_dict['metadata'][k] = v
                     else:
-                        canvas_dict['metadata'][k].extend(v)
+                        for value in v:
+                            if value not in canvas_dict['metadata'][k]:
+                                canvas_dict['metadata'][k].append(value)
+            # @Todo: Break this into separate method
+            # Add artists to metadata if not already present
+            if len(canvas_dict['artists']) > 0:
+                if 'Artist' not in canvas_dict['metadata']:
+                    canvas_dict['metadata']['Artist'] = canvas_dict['artists']
+                else:
+                    for artist in canvas_dict['artists']:
+                        if artist not in canvas_dict['metadata']['Artist']:
+                            canvas_dict['metadata']['Artist'].append(artist)
         for canvas_dict in hierarchy:
             canvas_dict['canvases'] = sorted(canvas_dict['canvases'], key=lambda x: int(x['sequence']))
         return hierarchy
 
 
     @staticmethod
     def __read(csv_file):
```

### Comparing `iiif_now-0.1.2/iiif_now/datacanvas/datacanvas.py` & `iiif_now-0.1.3/iiif_now/datacanvas/datacanvas.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.2/iiif_now/iiifnow.py` & `iiif_now-0.1.3/iiif_now/iiifnow.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.2/iiif_now/manifest/manifest.py` & `iiif_now-0.1.3/iiif_now/manifest/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from iiif_prezi3 import Manifest, config, KeyValueString, load_bundled_extensions, AnnotationPage, Annotation, ResourceItem
 import requests
 import json
 from iiif_now.navplace import NavPlace
+from iiif_now.thumbnail import Thumbnail
 
 
 class ANManifest:
-    # @Todo: Add navPlace
+    # @Todo: Reduce requests by adding thumbnails to manifest.
     def __init__(
             self,
             manifest_data,
             image_server_path="https://strob6zro3bzklrulaqu2545sy0odbvz.lambda-url.us-east-2.on.aws/iiif/3/",
             video_location="https://digital.lib.utk.edu/static/",
             manifest_bucket="https://aboltion-now-manifests.s3.us-east-2.amazonaws.com/",
             extensions=[]
@@ -43,28 +44,30 @@
             manifest = Manifest(
                 id=f"https://raw.githubusercontent.com/markpbaggett/static_iiif/main/manifests/abolition_now/{self.manifest_data['id']}.json",
                 label=self.manifest_data['manifest_title'] if self.manifest_data[
                                                                   'manifest_title'] != "" else "Untitled",
                 metadata=self.metadata
             )
         for canvas in self.manifest_data['canvases']:
+            # @Todo: Add canvas metadata to canvas.
             if canvas['type'] == 'Image':
                 try:
                     # @Todo: Protect anno page and annotation
+                    thumbnail = Thumbnail(f"{self.image_server_path}{canvas['key']}").get()
                     manifest.make_canvas_from_iiif(
                         url=f"{self.image_server_path}{canvas['key']}",
                         label=canvas['label'] if canvas['label'] != "" else "Untitled",
                         id=f"{self.manifest_bucket}{canvas['key']}/canvas/{canvas['sequence']}",
                         anno_id=f"{self.manifest_bucket}{canvas['key']}/canvas/{canvas['sequence']}/annotation/1",
                         anno_page_id=f"{self.manifest_bucket}{canvas['key']}/canvas/{canvas['sequence']}/annotation/1/page/1",
+                        thumbnail=thumbnail
                     )
                 except requests.HTTPError as e:
                     print(f'{e}. Missing file in bucket or other image server problem.')
             elif canvas['type'] == 'Video':
-                # try:
                 vid_canvas = manifest.make_canvas(
                     id=f"{self.manifest_bucket}{canvas['key']}/canvas/{canvas['sequence']}",
                     label=canvas['label'] if canvas['label'] != "" else "Untitled",
                 )
                 details = self.__create_video_canvas(
                     canvas=vid_canvas,
                     canvas_data= canvas
@@ -72,15 +75,14 @@
                 vid_canvas.set_hwd(**details[1])
                 vid_canvas.add_item(details[0])
         x = manifest.json(indent=2)
         manifest_as_json = json.loads(x)
         manifest_as_json['@context'] = ["http://iiif.io/api/extension/navplace/context.json", "http://iiif.io/api/presentation/3/context.json"]
         return manifest_as_json
 
-
     def __find_features(self):
         all_features = []
         for k, v in self.manifest_data['metadata'].items():
             if k == 'Geography':
                 for feature in v:
                     all_features.append(feature)
         return all_features
```

### Comparing `iiif_now-0.1.2/iiif_now/navplace/navplace.py` & `iiif_now-0.1.3/iiif_now/navplace/navplace.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.2/PKG-INFO` & `iiif_now-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: iiif-now
-Version: 0.1.2
+Version: 0.1.3
 Summary: IIIF Manifest Generator for Abolition Now project
+Home-page: https://github.com/abolition-now/iiif_now/
 License: WTFPL
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: iiif-prezi3 (>=1.2.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Project-URL: Repository, https://github.com/abolition-now/iiif_now/
 Description-Content-Type: text/markdown
 
 # IIIF Now
 
 ## About
 
 IIIF Manifest generation tools for the Abolition Now project.
 
+![Example Manifest](manifest_example.png "Example Manifest")
+
 ## Installation
 
 ```bash
 pip install iiif-now
 ```
 
 ## Configuration
@@ -44,7 +52,25 @@
 ```
 
 ## Usage
 
 ```bash
 iiifnow use config.yml
 ```
+# Changes
+
+## [0.1.3] - 2024-04-03
+
+### Features
+
+* Added artists to metadata.
+* Added thumbnails to image canvases.
+
+### Bug Fixes
+
+* Made sure codes are not repeated in parent manifests.
+
+## [0.1.2] - 2024-04-02
+
+* Implemented change log.
+* Added progress bar.
+* Added navPlace.
```

