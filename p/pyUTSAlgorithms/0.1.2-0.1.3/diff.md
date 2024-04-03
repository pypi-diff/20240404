# Comparing `tmp/pyUTSAlgorithms-0.1.2.tar.gz` & `tmp/pyUTSAlgorithms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUTSAlgorithms-0.1.2.tar", last modified: Wed Aug 30 18:30:28 2023, max compression
+gzip compressed data, was "pyUTSAlgorithms-0.1.3.tar", last modified: Wed Apr  3 23:06:47 2024, max compression
```

## Comparing `pyUTSAlgorithms-0.1.2.tar` & `pyUTSAlgorithms-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 18:30:28.008337 pyUTSAlgorithms-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (999)     1092 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     3010 2023-08-30 18:30:28.008337 pyUTSAlgorithms-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1447 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       84 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      699 2023-08-30 18:30:28.008337 pyUTSAlgorithms-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 18:30:28.004337 pyUTSAlgorithms-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 18:30:28.004337 pyUTSAlgorithms-0.1.2/src/pyUTSAlgorithms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3010 2023-08-30 18:30:27.000000 pyUTSAlgorithms-0.1.2/src/pyUTSAlgorithms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      508 2023-08-30 18:30:28.000000 pyUTSAlgorithms-0.1.2/src/pyUTSAlgorithms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 18:30:27.000000 pyUTSAlgorithms-0.1.2/src/pyUTSAlgorithms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-08-30 18:30:27.000000 pyUTSAlgorithms-0.1.2/src/pyUTSAlgorithms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-30 18:30:27.000000 pyUTSAlgorithms-0.1.2/src/pyUTSAlgorithms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 18:30:28.004337 pyUTSAlgorithms-0.1.2/src/uts/
--rw-r--r--   0 runner    (1001) docker     (999)      116 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/src/uts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2725 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/src/uts/ema.py
--rw-r--r--   0 runner    (1001) docker     (999)     3475 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/src/uts/gradient.py
--rw-r--r--   0 runner    (1001) docker     (999)     7316 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/src/uts/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (999)      134 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/src/uts/rolling.py
--rw-r--r--   0 runner    (1001) docker     (999)     7505 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/src/uts/sma.py
--rw-r--r--   0 runner    (1001) docker     (999)      707 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/src/uts/thresholding.py
--rw-r--r--   0 runner    (1001) docker     (999)     4135 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/src/uts/zscore.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 18:30:28.008337 pyUTSAlgorithms-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (999)     1224 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/test/test_ema.py
--rw-r--r--   0 runner    (1001) docker     (999)     1635 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/test/test_gradient.py
--rw-r--r--   0 runner    (1001) docker     (999)     6992 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/test/test_peaks.py
--rw-r--r--   0 runner    (1001) docker     (999)     1254 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/test/test_sma.py
--rw-r--r--   0 runner    (1001) docker     (999)     1236 2023-08-30 18:30:18.000000 pyUTSAlgorithms-0.1.2/test/test_zscore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:06:47.324855 pyUTSAlgorithms-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-03 23:06:47.324855 pyUTSAlgorithms-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:06:47.324855 pyUTSAlgorithms-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:06:47.320855 pyUTSAlgorithms-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:06:47.320855 pyUTSAlgorithms-0.1.3/src/pyUTSAlgorithms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-03 23:06:47.000000 pyUTSAlgorithms-0.1.3/src/pyUTSAlgorithms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 23:06:47.000000 pyUTSAlgorithms-0.1.3/src/pyUTSAlgorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:06:47.000000 pyUTSAlgorithms-0.1.3/src/pyUTSAlgorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 23:06:47.000000 pyUTSAlgorithms-0.1.3/src/pyUTSAlgorithms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 23:06:47.000000 pyUTSAlgorithms-0.1.3/src/pyUTSAlgorithms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:06:47.320855 pyUTSAlgorithms-0.1.3/src/uts/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/src/uts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/src/uts/ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/src/uts/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/src/uts/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/src/uts/rolling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/src/uts/sma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/src/uts/thresholding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/src/uts/zscore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:06:47.320855 pyUTSAlgorithms-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/test/test_ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/test/test_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/test/test_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/test/test_rolling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/test/test_sma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 23:06:41.000000 pyUTSAlgorithms-0.1.3/test/test_zscore.py
```

### Comparing `pyUTSAlgorithms-0.1.2/LICENSE` & `pyUTSAlgorithms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/PKG-INFO` & `pyUTSAlgorithms-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyUTSAlgorithms
-Version: 0.1.2
+Version: 0.1.3
 Summary: pyUTSAlgorithms (Unevenly Spaced Time Series Algorithms) Python package computes rolling statistics for uneven time series data.
-Home-page: https://github.com/mariolpantunes/uts
+Home-page: https://github.com/mariolpantunes/pyUTSAlgorithms
 Author: Mário Antunes
 Author-email: mario.antunes@ua.pt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.23
 
 # pyUTSAlgorithms (Unevenly Spaced Time Series Algorithms)
 
 Unevenly Spaced Time Series: Moving Averages and Other Rolling Operators
 This repository started as a conversion of the code from this [one](https://github.com/andreas50/utsAlgorithms).
 Right now the library contains more algorithms that help while dealing with Unevenly Spaced Time Series, for more details check the [here](#documentation).
 
@@ -26,27 +27,36 @@
 
 ```bash
 python -m unittest
 ```
 
 ## Documentation
 
-This library was documented using the google style docstring, it can be accessed [here](https://mariolpantunes.github.io/uts/).
+This library was documented using the google style docstring, it can be accessed [here](https://mariolpantunes.github.io/pyUTSAlgorithms/).
 Run the following commands to produce the documentation for this library.
 
 ```bash
 pip install pdoc
 pdoc --math -d google -o docs src/uts
 ```
 
 ## Instalation
 
-The library can be used by adding this line to the requirement.txt file:
+To install the library locally, simple execute the following commands:
+
+```bash
+python3 -m venv venv
+source venv/bin/activate
+python -m pip install --upgrade pip
+pip install .
+```
+You can also use the PyPI repository for easy access to the library:
+
 ```txt
-git+https://github.com/mariolpantunes/uts@main#egg=knee
+pyUTSAlgorithms>=0.1.3
 ```
 
 ## Authors
 
 * **Mário Antunes** - [mariolpantunes](https://github.com/mariolpantunes)
 
 ## License
```

### Comparing `pyUTSAlgorithms-0.1.2/README.md` & `pyUTSAlgorithms-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,36 @@
 
 ```bash
 python -m unittest
 ```
 
 ## Documentation
 
-This library was documented using the google style docstring, it can be accessed [here](https://mariolpantunes.github.io/uts/).
+This library was documented using the google style docstring, it can be accessed [here](https://mariolpantunes.github.io/pyUTSAlgorithms/).
 Run the following commands to produce the documentation for this library.
 
 ```bash
 pip install pdoc
 pdoc --math -d google -o docs src/uts
 ```
 
 ## Instalation
 
-The library can be used by adding this line to the requirement.txt file:
+To install the library locally, simple execute the following commands:
+
+```bash
+python3 -m venv venv
+source venv/bin/activate
+python -m pip install --upgrade pip
+pip install .
+```
+You can also use the PyPI repository for easy access to the library:
+
 ```txt
-git+https://github.com/mariolpantunes/uts@main#egg=knee
+pyUTSAlgorithms>=0.1.3
 ```
 
 ## Authors
 
 * **Mário Antunes** - [mariolpantunes](https://github.com/mariolpantunes)
 
 ## License
```

### Comparing `pyUTSAlgorithms-0.1.2/src/pyUTSAlgorithms.egg-info/PKG-INFO` & `pyUTSAlgorithms-0.1.3/src/pyUTSAlgorithms.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyUTSAlgorithms
-Version: 0.1.2
+Version: 0.1.3
 Summary: pyUTSAlgorithms (Unevenly Spaced Time Series Algorithms) Python package computes rolling statistics for uneven time series data.
-Home-page: https://github.com/mariolpantunes/uts
+Home-page: https://github.com/mariolpantunes/pyUTSAlgorithms
 Author: Mário Antunes
 Author-email: mario.antunes@ua.pt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.23
 
 # pyUTSAlgorithms (Unevenly Spaced Time Series Algorithms)
 
 Unevenly Spaced Time Series: Moving Averages and Other Rolling Operators
 This repository started as a conversion of the code from this [one](https://github.com/andreas50/utsAlgorithms).
 Right now the library contains more algorithms that help while dealing with Unevenly Spaced Time Series, for more details check the [here](#documentation).
 
@@ -26,27 +27,36 @@
 
 ```bash
 python -m unittest
 ```
 
 ## Documentation
 
-This library was documented using the google style docstring, it can be accessed [here](https://mariolpantunes.github.io/uts/).
+This library was documented using the google style docstring, it can be accessed [here](https://mariolpantunes.github.io/pyUTSAlgorithms/).
 Run the following commands to produce the documentation for this library.
 
 ```bash
 pip install pdoc
 pdoc --math -d google -o docs src/uts
 ```
 
 ## Instalation
 
-The library can be used by adding this line to the requirement.txt file:
+To install the library locally, simple execute the following commands:
+
+```bash
+python3 -m venv venv
+source venv/bin/activate
+python -m pip install --upgrade pip
+pip install .
+```
+You can also use the PyPI repository for easy access to the library:
+
 ```txt
-git+https://github.com/mariolpantunes/uts@main#egg=knee
+pyUTSAlgorithms>=0.1.3
 ```
 
 ## Authors
 
 * **Mário Antunes** - [mariolpantunes](https://github.com/mariolpantunes)
 
 ## License
```

### Comparing `pyUTSAlgorithms-0.1.2/src/uts/ema.py` & `pyUTSAlgorithms-0.1.3/src/uts/ema.py`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/src/uts/gradient.py` & `pyUTSAlgorithms-0.1.3/src/uts/gradient.py`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/src/uts/peak_detection.py` & `pyUTSAlgorithms-0.1.3/src/uts/peak_detection.py`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/src/uts/sma.py` & `pyUTSAlgorithms-0.1.3/src/uts/sma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # coding: utf-8
 
 __author__ = 'Mário Antunes'
 __version__ = '0.1'
 __email__ = 'mariolpantunes@gmail.com'
 __status__ = 'Development'
 
+
 import numpy as np
 
 
-def trapezoid_left(x1:float, x2:float, x3:float, y1:float, y3:float) -> float:
+def _trapezoid_left(x1:float, x2:float, x3:float, y1:float, y3:float) -> float:
     """
+    Internal function used in SMA linear variant.
+    
     Calculate the area of the trapezoid with corner coordinates (x2, 0), (x2, y2), (x3, 0), (x3, y3),
     where y2 is obtained by linear interpolation of (x1, y1) and (x3, y3) evaluated at x2.
 
     Args:
         x1 (float): x coordinate
         x2 (float): x coordinate
         x3 (float): x coordinate
@@ -30,16 +33,18 @@
 
     # Find y2 using linear interpolation and calculate the trapezoid area
     w = (x3 - x2) / (x3 - x1)
     y2 = y1 * w + y3 * (1 - w)
     return (x3 - x2) * (y2 + y3) / 2
 
 
-def trapezoid_right(x1,  x2,  x3,  y1,  y3) -> float:
+def _trapezoid_right(x1,  x2,  x3,  y1,  y3) -> float:
     """
+    Internal function used in SMA linear variant.
+
     Calculate the area of the trapezoid with corner coordinates (x1, 0), (x1, y1), (x2, 0), (x2, y2),
     where y2 is obtained by linear interpolation of (x1, y1) and (x3, y3) evaluated at x2.
 
     Args:
         x1 (float): x coordinate
         x2 (float): x coordinate
         x3 (float): x coordinate
@@ -214,15 +219,15 @@
         # Shrink interval on left end
         t_left_new = values[i][0] - width_before
         while values[left][0] < t_left_new:
             roll_area -= (values[left][1]+values[left+1][1])/2.0 * (values[left+1][0] - values[left][0])
             left += 1
     
         # Add truncated area on left and right end
-        left_area = trapezoid_left(values[max(0,left-1)][0], t_left_new, values[left][0], values[max(0,left-1)][1], values[left][1])
-        right_area = trapezoid_right(values[right][0], t_right_new, values[min(right+1, n-1)][0], values[right][1], values[min(right+1, n-1)][1]) 
+        left_area = _trapezoid_left(values[max(0,left-1)][0], t_left_new, values[left][0], values[max(0,left-1)][1], values[left][1])
+        right_area = _trapezoid_right(values[right][0], t_right_new, values[min(right+1, n-1)][0], values[right][1], values[min(right+1, n-1)][1]) 
         roll_area += left_area + right_area
 
         # Save SMA value for current time window
         y = roll_area / (width_before + width_after)
         rv[i] = np.array([values[i][0], y])
     return rv
```

### Comparing `pyUTSAlgorithms-0.1.2/src/uts/thresholding.py` & `pyUTSAlgorithms-0.1.3/src/uts/thresholding.py`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/src/uts/zscore.py` & `pyUTSAlgorithms-0.1.3/src/uts/zscore.py`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/test/test_ema.py` & `pyUTSAlgorithms-0.1.3/test/test_ema.py`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/test/test_gradient.py` & `pyUTSAlgorithms-0.1.3/test/test_gradient.py`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/test/test_peaks.py` & `pyUTSAlgorithms-0.1.3/test/test_peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import numpy as np
 import numpy.testing as npt
 
 from uts import peak_detection
 
 
 class Test_Peaks(unittest.TestCase):
-
     def test_find_next_tau(self):
         points = np.array(
             [[1.0, 1.0], [3.0, 2.0], [6.0, 3.0], [12.0, 4.0], [24.0, 5.0]])
         result = peak_detection.find_next_tau(points, 1, 5.0)
         desired = 3
         self.assertEqual(result, desired)
```

### Comparing `pyUTSAlgorithms-0.1.2/test/test_sma.py` & `pyUTSAlgorithms-0.1.3/test/test_sma.py`

 * *Files identical despite different names*

### Comparing `pyUTSAlgorithms-0.1.2/test/test_zscore.py` & `pyUTSAlgorithms-0.1.3/test/test_zscore.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,12 +25,11 @@
         desired = -2.2453655975512468
         self.assertAlmostEqual(result, desired, places=6)
     
     def test_zscore_array(self):
         points = np.array([[1,1], [2,2], [3,3], [4,4], [5,5], [6,6]])
         result = zscore.zscore_array_points(points)
         desired = np.array([-1.76776695, -1.06066017, -0.35355339,  0.35355339,  1.06066017,  1.76776695])
-        #print(result)
         np.testing.assert_array_almost_equal(result, desired, decimal=6)
 
 if __name__ == '__main__':
     unittest.main()
```

