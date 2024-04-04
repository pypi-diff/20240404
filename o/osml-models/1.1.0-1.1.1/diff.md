# Comparing `tmp/osml-models-1.1.0.tar.gz` & `tmp/osml-models-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osml-models-1.1.0.tar", last modified: Tue Nov 14 18:35:19 2023, max compression
+gzip compressed data, was "osml-models-1.1.1.tar", last modified: Thu Apr  4 19:18:51 2024, max compression
```

## Comparing `osml-models-1.1.0.tar` & `osml-models-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.006334 osml-models-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-11-14 18:35:09.000000 osml-models-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2023-11-14 18:35:19.006334 osml-models-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2023-11-14 18:35:09.000000 osml-models-1.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      600 2023-11-14 18:35:09.000000 osml-models-1.1.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1956 2023-11-14 18:35:19.006334 osml-models-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2023-11-14 18:35:09.000000 osml-models-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.002334 osml-models-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.002334 osml-models-1.1.0/src/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.002334 osml-models-1.1.0/src/aws/osml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.002334 osml-models-1.1.0/src/aws/osml/models/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-11-14 18:35:09.000000 osml-models-1.1.0/src/aws/osml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.006334 osml-models-1.1.0/src/aws/osml/models/aircraft/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-14 18:35:09.000000 osml-models-1.1.0/src/aws/osml/models/aircraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2023-11-14 18:35:09.000000 osml-models-1.1.0/src/aws/osml/models/aircraft/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.006334 osml-models-1.1.0/src/aws/osml/models/centerpoint/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-14 18:35:09.000000 osml-models-1.1.0/src/aws/osml/models/centerpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2023-11-14 18:35:09.000000 osml-models-1.1.0/src/aws/osml/models/centerpoint/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.006334 osml-models-1.1.0/src/aws/osml/models/flood/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-14 18:35:09.000000 osml-models-1.1.0/src/aws/osml/models/flood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-11-14 18:35:09.000000 osml-models-1.1.0/src/aws/osml/models/flood/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-11-14 18:35:09.000000 osml-models-1.1.0/src/aws/osml/models/server_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:35:19.006334 osml-models-1.1.0/src/osml_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2023-11-14 18:35:18.000000 osml-models-1.1.0/src/osml_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-11-14 18:35:19.000000 osml-models-1.1.0/src/osml_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 18:35:18.000000 osml-models-1.1.0/src/osml_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 18:35:18.000000 osml-models-1.1.0/src/osml_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-14 18:35:18.000000 osml-models-1.1.0/src/osml_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-14 18:35:18.000000 osml-models-1.1.0/src/osml_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.441103 osml-models-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 19:18:46.000000 osml-models-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-04 19:18:51.441103 osml-models-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-04 19:18:46.000000 osml-models-1.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      600 2024-04-04 19:18:46.000000 osml-models-1.1.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1956 2024-04-04 19:18:51.441103 osml-models-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-04 19:18:46.000000 osml-models-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.437103 osml-models-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.433103 osml-models-1.1.1/src/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.433103 osml-models-1.1.1/src/aws/osml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.437103 osml-models-1.1.1/src/aws/osml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 19:18:46.000000 osml-models-1.1.1/src/aws/osml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.437103 osml-models-1.1.1/src/aws/osml/models/aircraft/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 19:18:46.000000 osml-models-1.1.1/src/aws/osml/models/aircraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-04-04 19:18:46.000000 osml-models-1.1.1/src/aws/osml/models/aircraft/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.437103 osml-models-1.1.1/src/aws/osml/models/centerpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 19:18:46.000000 osml-models-1.1.1/src/aws/osml/models/centerpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-04 19:18:46.000000 osml-models-1.1.1/src/aws/osml/models/centerpoint/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.437103 osml-models-1.1.1/src/aws/osml/models/flood/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 19:18:46.000000 osml-models-1.1.1/src/aws/osml/models/flood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-04 19:18:46.000000 osml-models-1.1.1/src/aws/osml/models/flood/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-04 19:18:46.000000 osml-models-1.1.1/src/aws/osml/models/server_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:51.441103 osml-models-1.1.1/src/osml_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-04 19:18:51.000000 osml-models-1.1.1/src/osml_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-04 19:18:51.000000 osml-models-1.1.1/src/osml_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:18:51.000000 osml-models-1.1.1/src/osml_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:18:51.000000 osml-models-1.1.1/src/osml_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-04 19:18:51.000000 osml-models-1.1.1/src/osml_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 19:18:51.000000 osml-models-1.1.1/src/osml_models.egg-info/top_level.txt
```

### Comparing `osml-models-1.1.0/LICENSE` & `osml-models-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osml-models-1.1.0/PKG-INFO` & `osml-models-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-models
-Version: 1.1.0
+Version: 1.1.1
 Summary: A set of demonstration models to test OSML with.
 Author: Amazon Web Services
 Author-email: todo-public-library-poc@amazon.com
 License: 
         MIT No Attribution
         
         Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
```

### Comparing `osml-models-1.1.0/README.md` & `osml-models-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `osml-models-1.1.0/pyproject.toml` & `osml-models-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osml-models-1.1.0/setup.cfg` & `osml-models-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osml-models
-version = 1.1.0
+version = 1.1.1
 description = A set of demonstration models to test OSML with.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Amazon Web Services
 author_email = todo-public-library-poc@amazon.com
 license = 
 	MIT No Attribution
```

### Comparing `osml-models-1.1.0/src/aws/osml/models/aircraft/app.py` & `osml-models-1.1.1/src/aws/osml/models/aircraft/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import json
 import logging
 import os
 import uuid
 import warnings
 from typing import Dict, List, Optional, Union
 
@@ -89,42 +90,46 @@
     score, and type identifier as feature properties.
 
     :param instances: Detectron2 result instances
     :param image_id: Identifier for the processed image (optional)
     :return: FeatureCollection object containing detections
     """
     geojson_feature_collection_dict = {"type": "FeatureCollection", "features": []}
-
-    # Get the bounding boxes for this image
-    bboxes = instances.pred_boxes.tensor.cpu().numpy().tolist()
-
-    # Get the scores for this image
-    scores = instances.scores.cpu().numpy().tolist()
-
-    masks = None
-    if ENABLE_SEGMENTATION:
-        # Get the polygons for this image
-        masks = instances.pred_masks.cpu()
-
-    for i in range(0, len(bboxes)):
-        feature = {
-            "type": "Feature",
-            "geometry": {"type": "Point", "coordinates": [0.0, 0.0]},
-            "id": str(uuid.uuid4()),
-            "properties": {
-                "bounds_imcoords": bboxes[i],
-                "detection_score": float(scores[i]),
-                "feature_types": {"aircraft": float(scores[i])},
-                "image_id": image_id,
-            },
-        }
-        if masks is not None:
-            feature["properties"]["geom_imcoords"] = mask_to_polygon(masks[i])
-        app.logger.debug(feature)
-        geojson_feature_collection_dict["features"].append(feature)
+    if instances:
+        # Get the bounding boxes for this image
+        bboxes = instances.pred_boxes.tensor.cpu().numpy().tolist()
+
+        # Get the scores for this image
+        scores = instances.scores.cpu().numpy().tolist()
+
+        # Default masks to None
+        masks = None
+
+        # Get the polygon masks for this image if segmentation is enabled
+        if ENABLE_SEGMENTATION:
+            masks = instances.pred_masks.cpu()
+
+        for i in range(0, len(bboxes)):
+            feature = {
+                "type": "Feature",
+                "geometry": {"type": "Point", "coordinates": [0.0, 0.0]},
+                "id": str(uuid.uuid4()),
+                "properties": {
+                    "bounds_imcoords": bboxes[i],
+                    "detection_score": float(scores[i]),
+                    "feature_types": {"aircraft": float(scores[i])},
+                    "image_id": image_id,
+                },
+            }
+            if masks is not None:
+                feature["properties"]["geom_imcoords"] = mask_to_polygon(masks[i])
+            app.logger.debug(feature)
+            geojson_feature_collection_dict["features"].append(feature)
+    else:
+        app.logger.debug("No features found!")
 
     return geojson_feature_collection_dict
 
 
 def request_to_instances(req: Request) -> Union[Instances, None]:
     """
     Use GDAL to open the image. The binary payload from the HTTP request is used to
@@ -143,25 +148,29 @@
         # Load the binary memory buffer sent to the model
         gdal.FileFromMemBuffer(temp_ds_name, req.get_data())
         gdal_dataset = gdal.Open(temp_ds_name)
 
         # Read GDAL dataset and convert to a numpy array
         image_array = gdal_dataset.ReadAsArray()
 
-        # Check if the image has an alpha channel (4 channels) and remove it if so
-        if image_array.shape[0] == 4:
+        # Handling of different image shapes
+        if image_array.ndim == 2:  # For grayscale images without a channel dimension
+            # Reshape to add a channel dimension and replicate across 3 channels for RGB
+            image_array = np.stack([image_array] * 3, axis=0)
+        elif image_array.shape[0] == 1:  # For grayscale images with a channel dimension
+            # Replicate the single channel across 3 channels for RGB
+            image_array = np.repeat(image_array, 3, axis=0)
+        elif image_array.shape[0] == 4:  # For images with an alpha channel
             # Remove the alpha channel
             image_array = image_array[:3, :, :]
 
-        # Ensure the image has 3 channels (e.g., RGB)
-        if image_array.shape[0] == 1:
-            image_array = np.repeat(image_array, 3, axis=0)
-
-        # Convert numpy array to uint8 format (required for Detectron2)
+        # Conversion to uint8 (ensure this is done after ensuring 3 channels)
         image_array = (image_array * 255).astype(np.uint8)
+
+        # Transpose the array from (channels, height, width) to (height, width, channels)
         image = np.transpose(image_array, (1, 2, 0))
 
         # grab detections from Detectron2
         app.logger.debug(f"Running D2 on image array: {image}")
 
         # PyTorch can often give warnings about upcoming changes
         with warnings.catch_warnings():
```

### Comparing `osml-models-1.1.0/src/aws/osml/models/centerpoint/app.py` & `osml-models-1.1.1/src/aws/osml/models/centerpoint/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import json
 import logging
 import os
 from secrets import token_hex
 from typing import Dict, List
 
 from flask import Flask, Response, request
@@ -50,18 +51,18 @@
     circle = CirclePolygon(center, radius, resolution=number_of_vertices)
     poly_path = circle.get_path().vertices.tolist()
     # This is part of CV model requirements, to have (only) closed polygons
     poly_path.append(poly_path[0])
     # This moves poly to nonzero 0-1 coords
     nonzero_circle = [((x + 1) / 2, (y + 1) / 2) for (x, y) in poly_path]
     # Project to the correct percentage of our image coordinates
-    poly_scale = [bbox_percentage * width, bbox_percentage * height]
+    scale = [bbox_percentage * width, bbox_percentage * height]
     # Do final scaling of coordinates, and w/h translation to ensure within bounds of the bbox
     center_polygon = [
-        [round(x * poly_scale[0] + center_xy[0], 4), round(y * poly_scale[1] + center_xy[1], 4)] for (x, y) in nonzero_circle
+        [round(x * scale[0] + center_xy[0], 4), round(y * scale[1] + center_xy[1], 4)] for (x, y) in nonzero_circle
     ]
     return center_polygon
 
 
 def gen_center_detect(width: int, height: int, bbox_percentage: float) -> Dict:
     """
     Create  circular polygon that is at the center of and sized proportionally to the bbox
```

### Comparing `osml-models-1.1.0/src/aws/osml/models/flood/app.py` & `osml-models-1.1.1/src/aws/osml/models/flood/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import json
 import logging
 import math
 import os
+import random
 from random import randrange
 from secrets import token_hex
 from typing import Dict, Union
 
 from flask import Flask, Response, request
 from osgeo import gdal
 
@@ -15,14 +17,15 @@
 
 app = Flask(__name__)
 app.logger.setLevel(logging.ERROR)
 
 # Optional ENV configurations
 BBOX_PERCENTAGE = float(os.environ.get("BBOX_PERCENTAGE", 0.1))
 FLOOD_VOLUME = int(os.environ.get("FLOOD_VOLUME", 100))
+ENABLE_SEGMENTATION = os.environ.get("ENABLE_SEGMENTATION", "False").lower() == "true"
 
 
 def gen_flood_detects(height: int, width: int, bbox_percentage: float) -> Dict[str, Union[str, list]]:
     """
     Generate a random detection within the input image given a buffer percentage that
     limits the bounding boxes we generate to always fall within the image bounds.
 
@@ -38,21 +41,25 @@
         gen_y = randrange(fixed_object_size_xy[1], height - fixed_object_size_xy[1])
         fixed_object_bbox = [
             gen_x - fixed_object_size_xy[0],
             gen_y - fixed_object_size_xy[1],
             gen_x + fixed_object_size_xy[0],
             gen_y + fixed_object_size_xy[1],
         ]
-        fixed_object_mask = [
-            [gen_x - fixed_object_size_xy[0], gen_y + fixed_object_size_xy[1]],
-            [gen_y - fixed_object_size_xy[0], gen_x + fixed_object_size_xy[0]],
-            [gen_x + fixed_object_size_xy[0], gen_y + fixed_object_size_xy[1]],
-            [gen_y + fixed_object_size_xy[1], gen_x + fixed_object_size_xy[0]],
-        ]
-        feature = detect_to_feature(fixed_object_bbox, fixed_object_mask)
+        fixed_object_mask = None
+        if ENABLE_SEGMENTATION:
+            fixed_object_mask = [
+                [gen_x - fixed_object_size_xy[0], gen_y + fixed_object_size_xy[1]],
+                [gen_y - fixed_object_size_xy[0], gen_x + fixed_object_size_xy[0]],
+                [gen_x + fixed_object_size_xy[0], gen_y + fixed_object_size_xy[1]],
+                [gen_y + fixed_object_size_xy[1], gen_x + fixed_object_size_xy[0]],
+                [gen_x - fixed_object_size_xy[0], gen_y + fixed_object_size_xy[1]],
+            ]
+        # Create a feature with a random confidence score for each random detect
+        feature = detect_to_feature(fixed_object_bbox, fixed_object_mask, random.uniform(0, 1))
         geojson_features.append(feature)
 
     geojson_feature_collection_dict = {"type": "FeatureCollection", "features": geojson_features}
 
     return geojson_feature_collection_dict
```

### Comparing `osml-models-1.1.0/src/aws/osml/models/server_utils.py` & `osml-models-1.1.1/src/aws/osml/models/server_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import argparse
 import logging
 from secrets import token_hex
 from typing import Dict, List, Optional, Union
 
 from flask import Flask
```

### Comparing `osml-models-1.1.0/src/osml_models.egg-info/PKG-INFO` & `osml-models-1.1.1/src/osml_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-models
-Version: 1.1.0
+Version: 1.1.1
 Summary: A set of demonstration models to test OSML with.
 Author: Amazon Web Services
 Author-email: todo-public-library-poc@amazon.com
 License: 
         MIT No Attribution
         
         Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
```

### Comparing `osml-models-1.1.0/src/osml_models.egg-info/SOURCES.txt` & `osml-models-1.1.1/src/osml_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

