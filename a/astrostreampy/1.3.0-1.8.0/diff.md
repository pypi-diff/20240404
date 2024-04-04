# Comparing `tmp/astrostreampy-1.3.0.tar.gz` & `tmp/astrostreampy-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrostreampy-1.3.0.tar", last modified: Tue Jan  2 15:48:56 2024, max compression
+gzip compressed data, was "astrostreampy-1.8.0.tar", last modified: Thu Feb  8 09:06:11 2024, max compression
```

## Comparing `astrostreampy-1.3.0.tar` & `astrostreampy-1.8.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-01-02 15:48:56.070282 astrostreampy-1.3.0/
--rw-rw-rw-   0        0        0     1087 2023-08-15 10:36:54.000000 astrostreampy-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     3608 2024-01-02 15:48:56.067282 astrostreampy-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3062 2023-09-10 12:22:50.000000 astrostreampy-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-02 15:48:56.007285 astrostreampy-1.3.0/astrostreampy/
-drwxrwxrwx   0        0        0        0 2024-01-02 15:48:56.049284 astrostreampy-1.3.0/astrostreampy/BuildModel/
--rw-rw-rw-   0        0        0        0 2023-03-06 09:50:55.000000 astrostreampy-1.3.0/astrostreampy/BuildModel/__init__.py
--rw-rw-rw-   0        0        0     2739 2023-08-21 12:32:17.000000 astrostreampy-1.3.0/astrostreampy/BuildModel/aperture.py
--rw-rw-rw-   0        0        0    23497 2024-01-02 12:35:03.000000 astrostreampy-1.3.0/astrostreampy/BuildModel/autobuild.py
--rw-rw-rw-   0        0        0     8872 2023-12-14 15:39:08.000000 astrostreampy-1.3.0/astrostreampy/BuildModel/box.py
--rw-rw-rw-   0        0        0     1374 2023-08-19 07:34:39.000000 astrostreampy-1.3.0/astrostreampy/BuildModel/constants.py
--rw-rw-rw-   0        0        0     2350 2023-08-19 07:35:02.000000 astrostreampy-1.3.0/astrostreampy/BuildModel/liveplot.py
--rw-rw-rw-   0        0        0     4236 2024-01-02 12:47:36.000000 astrostreampy-1.3.0/astrostreampy/BuildModel/modify.py
--rw-rw-rw-   0        0        0    11994 2023-09-24 12:33:37.000000 astrostreampy-1.3.0/astrostreampy/BuildModel/utilities.py
-drwxrwxrwx   0        0        0        0 2024-01-02 15:48:56.064283 astrostreampy-1.3.0/astrostreampy/Image/
--rw-rw-rw-   0        0        0        0 2023-05-02 09:43:41.000000 astrostreampy-1.3.0/astrostreampy/Image/__init__.py
--rw-rw-rw-   0        0        0    16119 2023-12-20 08:28:58.000000 astrostreampy-1.3.0/astrostreampy/Image/inspect.py
--rw-rw-rw-   0        0        0    11686 2024-01-02 14:20:06.000000 astrostreampy-1.3.0/astrostreampy/Image/measure.py
--rw-rw-rw-   0        0        0     7788 2024-01-02 12:30:12.000000 astrostreampy-1.3.0/astrostreampy/Image/point.py
--rw-rw-rw-   0        0        0     4686 2023-12-20 08:07:18.000000 astrostreampy-1.3.0/astrostreampy/Image/stream.py
--rw-rw-rw-   0        0        0      881 2023-08-24 17:44:14.000000 astrostreampy-1.3.0/astrostreampy/Image/utilities.py
--rw-rw-rw-   0        0        0        0 2023-02-20 14:38:47.000000 astrostreampy-1.3.0/astrostreampy/__init__.py
--rw-rw-rw-   0        0        0      825 2023-08-19 07:41:30.000000 astrostreampy-1.3.0/astrostreampy/argutils.py
--rw-rw-rw-   0        0        0     1746 2023-08-21 12:33:48.000000 astrostreampy-1.3.0/astrostreampy/utilities.py
-drwxrwxrwx   0        0        0        0 2024-01-02 15:48:56.066289 astrostreampy-1.3.0/astrostreampy.egg-info/
--rw-rw-rw-   0        0        0     3608 2024-01-02 15:48:55.000000 astrostreampy-1.3.0/astrostreampy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-01-02 15:48:55.000000 astrostreampy-1.3.0/astrostreampy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-02 15:48:55.000000 astrostreampy-1.3.0/astrostreampy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-01-02 15:48:55.000000 astrostreampy-1.3.0/astrostreampy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      876 2024-01-02 15:46:59.000000 astrostreampy-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-02 15:48:56.070282 astrostreampy-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-08 09:06:11.254869 astrostreampy-1.8.0/
+-rw-rw-rw-   0        0        0     1087 2023-08-15 10:36:54.000000 astrostreampy-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0     3602 2024-02-08 09:06:11.251881 astrostreampy-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3062 2023-09-10 12:22:50.000000 astrostreampy-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-02-08 09:06:11.182007 astrostreampy-1.8.0/astrostreampy/
+drwxrwxrwx   0        0        0        0 2024-02-08 09:06:11.219005 astrostreampy-1.8.0/astrostreampy/BuildModel/
+-rw-rw-rw-   0        0        0        0 2023-03-06 09:50:55.000000 astrostreampy-1.8.0/astrostreampy/BuildModel/__init__.py
+-rw-rw-rw-   0        0        0     4628 2024-02-07 11:06:56.000000 astrostreampy-1.8.0/astrostreampy/BuildModel/aperture.py
+-rw-rw-rw-   0        0        0    23779 2024-01-30 14:29:19.000000 astrostreampy-1.8.0/astrostreampy/BuildModel/autobuild.py
+-rw-rw-rw-   0        0        0     8872 2023-12-14 15:39:08.000000 astrostreampy-1.8.0/astrostreampy/BuildModel/box.py
+-rw-rw-rw-   0        0        0     1374 2023-08-19 07:34:39.000000 astrostreampy-1.8.0/astrostreampy/BuildModel/constants.py
+-rw-rw-rw-   0        0        0     2350 2023-08-19 07:35:02.000000 astrostreampy-1.8.0/astrostreampy/BuildModel/liveplot.py
+-rw-rw-rw-   0        0        0     4236 2024-01-02 12:47:36.000000 astrostreampy-1.8.0/astrostreampy/BuildModel/modify.py
+-rw-rw-rw-   0        0        0    14179 2024-02-07 12:48:13.000000 astrostreampy-1.8.0/astrostreampy/BuildModel/utilities.py
+drwxrwxrwx   0        0        0        0 2024-02-08 09:06:11.244875 astrostreampy-1.8.0/astrostreampy/Image/
+-rw-rw-rw-   0        0        0        0 2023-05-02 09:43:41.000000 astrostreampy-1.8.0/astrostreampy/Image/__init__.py
+-rw-rw-rw-   0        0        0    16119 2023-12-20 08:28:58.000000 astrostreampy-1.8.0/astrostreampy/Image/inspect.py
+-rw-rw-rw-   0        0        0    20229 2024-02-07 12:58:42.000000 astrostreampy-1.8.0/astrostreampy/Image/measure.py
+-rw-rw-rw-   0        0        0     7836 2024-01-30 14:02:18.000000 astrostreampy-1.8.0/astrostreampy/Image/point.py
+-rw-rw-rw-   0        0        0     4686 2023-12-20 08:07:18.000000 astrostreampy-1.8.0/astrostreampy/Image/stream.py
+-rw-rw-rw-   0        0        0     6669 2024-02-07 12:48:37.000000 astrostreampy-1.8.0/astrostreampy/Image/track.py
+-rw-rw-rw-   0        0        0     2101 2024-02-05 10:07:44.000000 astrostreampy-1.8.0/astrostreampy/Image/utilities.py
+-rw-rw-rw-   0        0        0        0 2023-02-20 14:38:47.000000 astrostreampy-1.8.0/astrostreampy/__init__.py
+-rw-rw-rw-   0        0        0      825 2023-08-19 07:41:30.000000 astrostreampy-1.8.0/astrostreampy/argutils.py
+-rw-rw-rw-   0        0        0     2349 2024-01-30 13:12:26.000000 astrostreampy-1.8.0/astrostreampy/utilities.py
+drwxrwxrwx   0        0        0        0 2024-02-08 09:06:11.248863 astrostreampy-1.8.0/astrostreampy.egg-info/
+-rw-rw-rw-   0        0        0     3602 2024-02-08 09:06:11.000000 astrostreampy-1.8.0/astrostreampy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2024-02-08 09:06:11.000000 astrostreampy-1.8.0/astrostreampy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-08 09:06:11.000000 astrostreampy-1.8.0/astrostreampy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-02-08 09:06:11.000000 astrostreampy-1.8.0/astrostreampy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      870 2024-02-08 09:01:09.000000 astrostreampy-1.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-08 09:06:11.255864 astrostreampy-1.8.0/setup.cfg
```

### Comparing `astrostreampy-1.3.0/LICENSE` & `astrostreampy-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/PKG-INFO` & `astrostreampy-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: astrostreampy
-Version: 1.3.0
+Version: 1.8.0
 Summary: Package to model stellar tidal streams.
-Author-email: Jan-Niklas Pippert <pippertjanniklas@gmail.com>
+Author-email: Jan-Niklas Pippert <jnpippert@usm.lmu.de>
 Project-URL: Homepage, https://github.com/jnpippert/streamPy
 Project-URL: Bug Tracker, https://github.com/jnpippert/streamPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `astrostreampy-1.3.0/README.md` & `astrostreampy-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/astrostreampy/BuildModel/autobuild.py` & `astrostreampy-1.8.0/astrostreampy/BuildModel/autobuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from astropy.io import fits
 from astropy.wcs import WCS
 
 from ..Image.point import Point
 from . import utilities as util
 from .box import Box
 from .constants import direction_dict, sectors, slope_dict
-
+from ..utilities import timeit
 warnings.filterwarnings("ignore")
 
 
 class SegmentModel:
     def __init__(self, shape: tuple) -> None:
         self.model = np.full(shape=shape, fill_value=np.nan)
 
@@ -93,17 +93,16 @@
             ``False`` if repetion limit reached. Otherwise ``True``.
         """
 
         if not np.isclose(self._tmp, self._value, atol=1e-10):
             self._rep_count = 1
             return True
         self._rep_count += 1
-        if self._rep_count == 3:
-            return False
-        return True
+        return not (self._rep_count == 3)
+            
 
 
 class Model:
 
     """
     Creates a model object for a stream
 
@@ -238,19 +237,19 @@
         self._skew = skew
         self._h4 = h4
         self._sn_threshold = sn_threshold
         self._init_params = [self.init_angle, 1, 1, 0, 0, 0, 0, 0, 0]
 
         # like that, higher order fitting is more robust
         if h2:
-            self._init_params[6] = 0.1
+            self._init_params[6] = 0.01
         if skew:
-            self._init_params[7] = 0.1
+            self._init_params[7] = 0.01
         if h4:
-            self._init_params[8] = 0.1
+            self._init_params[8] = 0.01
 
         # error monitoring
         self.param_errors = []
 
         # parameters
         self.params = []
         self.box_properties = []
@@ -298,25 +297,26 @@
         int
             -1 if any condition is met, otherwise 0.
         """
         if self._head is not None:
             if box_center.isclose(self._head, tol=self._tol):
                 self._head_dist -= 1
 
-        if self._head_dist == 0:
-            print("head reached. segment terminated.")
-            return -1
-
+            if self._head_dist == 0:
+                print("head reached. segment terminated.")
+                return -1
+            return 0
+        
         if self._tail is not None:
             if box_center.isclose(self._tail, tol=self._tol):
                 self._tail_dist -= 1
-
-        if self._tail_dist == 0:
-            print("tail reached. segment terminated.")
-            return -1
+            if self._tail_dist == 0:
+                print("tail reached. segment terminated.")
+                return -1
+            return 0
 
         if peak_pos is None:
             print("no peak for a gaussian fit found. segment terminated.")
             return -1
 
         if isinstance(norm_err, float):
             if self._sn_threshold == 0:
@@ -331,14 +331,16 @@
         if norm_tracker.add_val(value=norm) == -1:
             print("repeating parameters detected. segment terminated.")
             return -1
         return 0
 
     def _segment(self, args):
         angle, x, y, w, h, direction, step_number, guess_parameter = args
+        init_w  = w
+        inti_h = h
         best_fit_parameter: list = []
         box_properties: list = []
         seg_model = SegmentModel(shape=(self._dimy, self._dimx))
         norm_tracker = ParamTracker()
         box_center = Point()
         for _ in range(step_number):
             x, y = util.calculate_next_boxcenter(
@@ -392,17 +394,20 @@
                 == -1
             ):
                 break
 
             x, y = util.correct_box_center_from_peak(
                 x=x, y=y, w=w, h=h, peak_pos=tmp_box.peak_pos
             )
+            if self._vary_box_dim:
+                w,h = util.calculate_new_box_dimensions(tmp_box.angle,init_height=inti_h,init_width=init_w)
 
         return [best_fit_parameter, seg_model.model, box_properties]
 
+    @timeit
     def build(self, steps: tuple[int, int] = (9999, 9999)):
         """
         Does the model building.
 
         First, the initial box is fitted. From there the two possible
         directions in which the box could be shifted is determined.
         From there two loops shift the box and make a model in every step.
```

### Comparing `astrostreampy-1.3.0/astrostreampy/BuildModel/box.py` & `astrostreampy-1.8.0/astrostreampy/BuildModel/box.py`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/astrostreampy/BuildModel/constants.py` & `astrostreampy-1.8.0/astrostreampy/BuildModel/constants.py`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/astrostreampy/BuildModel/liveplot.py` & `astrostreampy-1.8.0/astrostreampy/BuildModel/liveplot.py`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/astrostreampy/BuildModel/modify.py` & `astrostreampy-1.8.0/astrostreampy/BuildModel/modify.py`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/astrostreampy/BuildModel/utilities.py` & `astrostreampy-1.8.0/astrostreampy/BuildModel/utilities.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from astropy.io import fits
 from scipy.signal import find_peaks
+from .constants import *
+from scipy.stats import norm as scn
+from astropy.convolution import Gaussian1DKernel, convolve
 
 
 def intro():
     """
     Prints the intro of the stream modelling.
     """
     print(
@@ -361,7 +364,80 @@
         left = np.argmin(np.abs(model_slice[left_ids] - half_max))
         right = np.argmin(np.abs(model_slice[right_ids] - half_max)) + center_id + 1
 
         left_dists.append(center_id - left)
         right_dists.append(right - center_id)
         center_ids.append(center_id)
     return center_ids, left_dists, right_dists
+
+
+def fit_func(
+    size: int,
+    sigma: float,
+    norm: float,
+    offset: float,
+    h2: float,
+    skew: float,
+    h4: float,
+    psf: float = None,
+) -> np.ndarray:
+    """
+    The fit function parsed into ``lmfit.Model``. All parameters are varied by LMfit-py.
+    Every call a new set of parameters is used to create a model image with the size of the box.
+    Before returning the model array it gets convovled by the seeing, this ensure that the intrinsic
+    Gaussian parameters are fitted. This is a private method and should not be used outside this class.
+
+    """
+
+    vals = np.arange(-size, size + 1, 1) / sigma
+    h4_comp = h4 * (c4_1 * vals**4 - c4_2 * vals**2 + c4_3)
+    h2_comp = h2 * (c2_1 * vals**2 - c2_2)
+    model = (
+        norm * np.exp(-0.5 * vals**2) * (1 + h2_comp + h4_comp + scn.cdf(skew * vals))
+    ) + offset
+
+    if isinstance(psf, float):
+        return convolve(
+            model,
+            kernel=Gaussian1DKernel(stddev=psf),
+            boundary="extend",
+            nan_treatment="fill",
+        )
+    return model
+
+
+def get_effective_distances(parameter_file, multifits_file):
+    dists: list = []
+    center_ids: list = []
+    table = fits.getdata(parameter_file, ext=1)
+    model = fits.getdata(multifits_file, ext=4)
+
+    for row in table:
+        (
+            x,
+            y,
+            w,
+            h,
+        ) = np.array(row)[
+            np.array([0, 1, 2, 3])
+        ].astype(int)
+
+        if w > h:
+            model_slice = model.copy()[y, x - w : x + w + 1]
+        else:
+            model_slice = model.copy()[y - h : y + h + 1, x]
+        total_flux = np.sum(model_slice)
+        center_id = np.argmax(model_slice)
+        dist = 0
+
+        while True:
+            region = model_slice[center_id - dist : center_id + dist + 1]
+
+            if np.sum(region) > total_flux / 2:
+
+                break
+            dist += 1
+
+        dists.append(dist)
+        center_ids.append(center_id)
+
+    return center_ids, dists
```

### Comparing `astrostreampy-1.3.0/astrostreampy/Image/inspect.py` & `astrostreampy-1.8.0/astrostreampy/Image/inspect.py`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/astrostreampy/Image/point.py` & `astrostreampy-1.8.0/astrostreampy/Image/point.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,28 +52,28 @@
         img = ax.imshow(data, vmin=vmin, vmax=vmax, origin="lower", cmap=cmap)
 
         # initialize vmin slider
         ax_vmin = fig.add_axes([0.2, 0.07, 0.7, 0.03])
         vmin_slider = Slider(
             ax=ax_vmin,
             label="shadows",
-            valmin=np.percentile(data, 1),
-            valmax=np.percentile(data, 99),
+            valmin=np.min(data),
+            valmax=np.max(data),
             valinit=vmin,
             valstep=vmin / 10,
         )
         vmin_slider.on_changed(self._update)
 
         # initialize vmax slider
         ax_vmax = fig.add_axes([0.2, 0.03, 0.7, 0.03])
         vmax_slider = Slider(
             ax=ax_vmax,
             label="highlights",
-            valmin=np.percentile(data, 1),
-            valmax=np.percentile(data, 99),
+            valmin=np.min(data),
+            valmax=np.max(data),
             valinit=vmax,
             valstep=vmax / 10,
         )
         vmax_slider.on_changed(self._update)
 
         rect = ax.add_patch(
             Rectangle(
@@ -146,23 +146,26 @@
         self._p1 = p1
         self._p2 = p2
         self.tail = Point()
         self.head = Point()
         self._pointmode = True
         self._p1mode = False
         self._p2mode = False
+        
         self._cid = point.figure.canvas.mpl_connect(
             "button_press_event", self._mouse_click
         )
         self._fig.suptitle(r"set init point and box", color="k")
-        fig.canvas.mpl_connect("key_press_event", self._key_press)
+        
+        self._fig.canvas.mpl_connect('key_press_event', self._key_press_event)
 
         plt.show()
 
-    def _key_press(self, event):
+    def _key_press_event(self,event):
+        print(f"key pressed {event.key}")
         sys.stdout.flush()
         if event.key == "a":
             self._p1mode = True
             self._p2mode = False
             self._pointmode = False
             self._fig.suptitle(r"set first end point", color="k")
             self._fig.figure.canvas.draw()
@@ -180,14 +183,15 @@
             self._fig.figure.canvas.draw()
 
     def _mouse_click(self, event):
         """
         Handles mouse clicking events in the matplotlib API.
         This is a private method and should not be used outside this class.
         """
+        
         if event.inaxes != self._point.axes:
             return
         x = int(np.round(event.xdata, 0))
         y = int(np.round(event.ydata, 0))
         if self._p1mode:
             self.tail.x = x
             self.tail.y = y
```

### Comparing `astrostreampy-1.3.0/astrostreampy/Image/stream.py` & `astrostreampy-1.8.0/astrostreampy/Image/stream.py`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/astrostreampy/argutils.py` & `astrostreampy-1.8.0/astrostreampy/argutils.py`

 * *Files identical despite different names*

### Comparing `astrostreampy-1.3.0/astrostreampy/utilities.py` & `astrostreampy-1.8.0/astrostreampy/utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 from astropy.convolution import Gaussian1DKernel, convolve
 from scipy.stats import norm as scn
 
 from .BuildModel.constants import c2_1, c2_2, c4_1, c4_2, c4_3
 from .BuildModel.utilities import create_grid_arrays
+from functools import wraps
+import time
 
 
 def fit_func_2D(
     _: None,
     angle: float,
     sigma: float,
     norm: float,
@@ -53,7 +55,28 @@
     h2_comp = h2 * (c2_1 * vals**2 - c2_2)
     model = (
         norm * np.exp(-0.5 * vals**2) * (1 + h2_comp + h4_comp + scn.cdf(skew * vals))
     ) + offset
     if seeing is None:
         return model
     return convolve(model, kernel=kernel, boundary="extend", nan_treatment="fill")
+
+def timeit(
+    func=None
+):
+    def decorator_timeit(func):
+        @wraps(func)
+        def wrapper_timeit(*args, **kwargs):
+            start_time = time.perf_counter()
+            result = func(*args, **kwargs)
+            end_time = time.perf_counter()
+            print(
+                f"\tfinished after {np.round(end_time - start_time,2)} seconds"
+            )
+            return result
+
+        return wrapper_timeit
+
+    if func is None:  # @timeit() -> @timeit
+        return decorator_timeit
+
+    return decorator_timeit(func)
```

### Comparing `astrostreampy-1.3.0/astrostreampy.egg-info/PKG-INFO` & `astrostreampy-1.8.0/astrostreampy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: astrostreampy
-Version: 1.3.0
+Version: 1.8.0
 Summary: Package to model stellar tidal streams.
-Author-email: Jan-Niklas Pippert <pippertjanniklas@gmail.com>
+Author-email: Jan-Niklas Pippert <jnpippert@usm.lmu.de>
 Project-URL: Homepage, https://github.com/jnpippert/streamPy
 Project-URL: Bug Tracker, https://github.com/jnpippert/streamPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `astrostreampy-1.3.0/astrostreampy.egg-info/SOURCES.txt` & `astrostreampy-1.8.0/astrostreampy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 astrostreampy/BuildModel/modify.py
 astrostreampy/BuildModel/utilities.py
 astrostreampy/Image/__init__.py
 astrostreampy/Image/inspect.py
 astrostreampy/Image/measure.py
 astrostreampy/Image/point.py
 astrostreampy/Image/stream.py
+astrostreampy/Image/track.py
 astrostreampy/Image/utilities.py
```

### Comparing `astrostreampy-1.3.0/pyproject.toml` & `astrostreampy-1.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,17 @@
             "lmfit>=1.2.2"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "astrostreampy"
-version = "1.3.0"
+version = "1.8.0"
 authors = [
-  { name="Jan-Niklas Pippert", email="pippertjanniklas@gmail.com" },
+  { name="Jan-Niklas Pippert", email="jnpippert@usm.lmu.de" },
 ]
 description = "Package to model stellar tidal streams."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

