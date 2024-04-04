# Comparing `tmp/train_route-0.6.1.tar.gz` & `tmp/train_route-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "train_route-0.6.1.tar", max compression
+gzip compressed data, was "train_route-0.6.2.tar", max compression
```

## Comparing `train_route-0.6.1.tar` & `train_route-0.6.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2024-03-24 14:11:14.824841 train_route-0.6.1/LICENSE
--rw-r--r--   0        0        0      228 2024-03-28 11:56:12.497719 train_route-0.6.1/README.md
--rw-r--r--   0        0        0      407 2024-04-04 14:39:53.447507 train_route-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-24 12:22:27.136302 train_route-0.6.1/train_route/__init__.py
--rw-r--r--   0        0        0      496 2024-03-28 00:12:18.072432 train_route-0.6.1/train_route/rotation.py
--rw-r--r--   0        0        0     3808 2024-03-24 16:54:39.986473 train_route-0.6.1/train_route/route.py
--rw-r--r--   0        0        0     5445 2024-04-04 14:39:36.447509 train_route-0.6.1/train_route/traveler.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 train_route-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-24 14:11:14.824841 train_route-0.6.2/LICENSE
+-rw-r--r--   0        0        0      228 2024-03-28 11:56:12.497719 train_route-0.6.2/README.md
+-rw-r--r--   0        0        0      407 2024-04-04 14:46:41.407430 train_route-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-24 12:22:27.136302 train_route-0.6.2/train_route/__init__.py
+-rw-r--r--   0        0        0      496 2024-03-28 00:12:18.072432 train_route-0.6.2/train_route/rotation.py
+-rw-r--r--   0        0        0     3808 2024-03-24 16:54:39.986473 train_route-0.6.2/train_route/route.py
+-rw-r--r--   0        0        0     5447 2024-04-04 14:46:34.207431 train_route-0.6.2/train_route/traveler.py
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 train_route-0.6.2/PKG-INFO
```

### Comparing `train_route-0.6.1/LICENSE` & `train_route-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `train_route-0.6.1/train_route/route.py` & `train_route-0.6.2/train_route/route.py`

 * *Files identical despite different names*

### Comparing `train_route-0.6.1/train_route/traveler.py` & `train_route-0.6.2/train_route/traveler.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             return center_position
         d0 = max(0, distance - car_length / 2)
         d1 = min(self.distance, distance + car_length / 2)
         start_position = self.state(d0)
         end_position = self.state(d1)
         x0, y0 = start_position['x'], start_position['y']
         x1, y1 = end_position['x'], end_position['y']
-        print(x0, y0, x1, y1)
+        # print(x0, y0, x1, y1)
         rotation = spheric_rotation(x0, y0, x1, y1)
         center_position['rotation'] = rotation
         center_position['x'] = (x0 + x1) / 2
         center_position['y'] = (y0 + y1) / 2
         return center_position
     
     def to_dict(self):
```

### Comparing `train_route-0.6.1/PKG-INFO` & `train_route-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: train-route
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Author: Samarin Aleksei
 Author-email: liotbiu1@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

