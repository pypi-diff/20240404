# Comparing `tmp/train_route-0.5.0.tar.gz` & `tmp/train_route-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "train_route-0.5.0.tar", max compression
+gzip compressed data, was "train_route-0.6.0.tar", max compression
```

## Comparing `train_route-0.5.0.tar` & `train_route-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2024-03-24 14:11:14.824841 train_route-0.5.0/LICENSE
--rw-r--r--   0        0        0      228 2024-03-28 11:56:12.497719 train_route-0.5.0/README.md
--rw-r--r--   0        0        0      407 2024-04-03 16:25:12.785652 train_route-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-24 12:22:27.136302 train_route-0.5.0/train_route/__init__.py
--rw-r--r--   0        0        0      496 2024-03-28 00:12:18.072432 train_route-0.5.0/train_route/rotation.py
--rw-r--r--   0        0        0     3808 2024-03-24 16:54:39.986473 train_route-0.5.0/train_route/route.py
--rw-r--r--   0        0        0     4758 2024-04-03 15:42:56.856101 train_route-0.5.0/train_route/traveler.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 train_route-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-24 14:11:14.824841 train_route-0.6.0/LICENSE
+-rw-r--r--   0        0        0      228 2024-03-28 11:56:12.497719 train_route-0.6.0/README.md
+-rw-r--r--   0        0        0      407 2024-04-04 14:32:48.867588 train_route-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-24 12:22:27.136302 train_route-0.6.0/train_route/__init__.py
+-rw-r--r--   0        0        0      496 2024-03-28 00:12:18.072432 train_route-0.6.0/train_route/rotation.py
+-rw-r--r--   0        0        0     3808 2024-03-24 16:54:39.986473 train_route-0.6.0/train_route/route.py
+-rw-r--r--   0        0        0     5353 2024-04-04 14:30:35.947609 train_route-0.6.0/train_route/traveler.py
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 train_route-0.6.0/PKG-INFO
```

### Comparing `train_route-0.5.0/LICENSE` & `train_route-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `train_route-0.5.0/train_route/route.py` & `train_route-0.6.0/train_route/route.py`

 * *Files identical despite different names*

### Comparing `train_route-0.5.0/train_route/traveler.py` & `train_route-0.6.0/train_route/traveler.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,22 +98,34 @@
         if position is None:
             return None
         idx, delta = position
         d0 = self.distances[idx]
         d1 = self.distances[idx + 1]
         return d0 + (d1 - d0) * delta
 
-    def state(self, distance):
+    def state(self, distance, car_length = None):
         position = index_delta(self.distances, distance)
         if position is None:
             return None
         idx, delta = position
         segment = self.segments[idx]
         segment_distance = segment.distance * delta
-        return segment.state(segment_distance)
+        center_position = segment.state(segment_distance)
+        if car_length is None:
+            return center_position
+        d0 = max(0, distance - car_length / 2)
+        d1 = min(self.distance, distance + car_length / 2)
+        start_position = self.state(d0)
+        end_position = self.state(d1)
+        x0, y0 = start_position['x'], start_position['y']
+        x1, y1 = end_position['x'], end_position['y']
+        print(x0, y0, x1, y1)
+        rotation = spheric_rotation(x0, y0, x1, y1)
+        center_position['rotation'] = rotation
+        return center_position
     
     def to_dict(self):
         return {
             'relative_path_id': self.relative_path_id,
             'segments': [s.to_ref() for s in self.segments],
             'ts': self.ts[1:]
         }
@@ -131,24 +143,24 @@
         "State of traveler at t"
         state = self.chain_state(t, distance_lags=[0])
         if state:
             return state[0]
         else:
             return None
         
-    def chain_state(self, t, distance_lags = [0]):
+    def chain_state(self, t, distance_lags = [0], car_length = None):
         if isinstance(self.start, datetime):
             relative_t = (t - self.start).total_seconds()
         else:
             relative_t = t - self.start
         distance = self.path.covered_distance(relative_t)
         if distance is None:
             return None
         
-        return [self.path.state(distance - l) for l in distance_lags if distance - l >= 0]
+        return [self.path.state(distance - l, car_length) for l in distance_lags if distance - l >= 0]
 
     def to_dict(self):
         return {
             'path_id': self.path_id,
             'path': self.path.to_ref(),
             'start': self.start if isinstance(self.start, int) else str(self.start),
         }
```

### Comparing `train_route-0.5.0/PKG-INFO` & `train_route-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: train-route
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Samarin Aleksei
 Author-email: liotbiu1@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

