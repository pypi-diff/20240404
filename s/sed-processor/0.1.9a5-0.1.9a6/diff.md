# Comparing `tmp/sed_processor-0.1.9a5.tar.gz` & `tmp/sed_processor-0.1.9a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sed_processor-0.1.9a5.tar", max compression
+gzip compressed data, was "sed_processor-0.1.9a6.tar", max compression
```

## Comparing `sed_processor-0.1.9a5.tar` & `sed_processor-0.1.9a6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1072 2024-03-22 13:22:45.110681 sed_processor-0.1.9a5/LICENSE
--rw-r--r--   0        0        0     2881 2024-03-22 13:22:45.110681 sed_processor-0.1.9a5/README.md
--rw-r--r--   0        0        0     2751 2024-03-22 13:22:55.978732 sed_processor-0.1.9a5/pyproject.toml
--rw-r--r--   0        0        0      127 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/__init__.py
--rw-r--r--   0        0        0      160 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/binning/__init__.py
--rw-r--r--   0        0        0    21273 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/binning/binning.py
--rw-r--r--   0        0        0     8570 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/binning/numba_bin.py
--rw-r--r--   0        0        0     6073 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/binning/utils.py
--rw-r--r--   0        0        0      231 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/calibrator/__init__.py
--rw-r--r--   0        0        0    17235 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/calibrator/delay.py
--rw-r--r--   0        0        0    88904 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/calibrator/energy.py
--rw-r--r--   0        0        0    83115 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/calibrator/momentum.py
--rwxr-xr-x   0        0        0    17175 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/config/NXmpes_config.json
--rw-r--r--   0        0        0     4692 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/config/default.yaml
--rw-r--r--   0        0        0     6359 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/config/flash_example_config.yaml
--rw-r--r--   0        0        0    11357 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/config/mpes_example_config.yaml
--rw-r--r--   0        0        0      105 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/core/__init__.py
--rw-r--r--   0        0        0     9017 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/core/config.py
--rw-r--r--   0        0        0    17134 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/core/dfops.py
--rw-r--r--   0        0        0     4182 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/core/metadata.py
--rw-r--r--   0        0        0   101134 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/core/processor.py
--rw-r--r--   0        0        0     4903 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/diagnostics.py
--rw-r--r--   0        0        0      262 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/io/__init__.py
--rw-r--r--   0        0        0     5939 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/io/hdf5.py
--rw-r--r--   0        0        0     1381 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/io/nexus.py
--rw-r--r--   0        0        0     7865 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/io/tiff.py
--rw-r--r--   0        0        0      166 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/__init__.py
--rw-r--r--   0        0        0       14 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/base/README.md
--rw-r--r--   0        0        0        0 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/base/__init__.py
--rw-r--r--   0        0        0     6110 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/base/loader.py
--rw-r--r--   0        0        0        0 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/flash/__init__.py
--rw-r--r--   0        0        0    35827 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/flash/loader.py
--rw-r--r--   0        0        0     4300 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/flash/metadata.py
--rw-r--r--   0        0        0        0 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/generic/__init__.py
--rw-r--r--   0        0        0     5693 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/generic/loader.py
--rw-r--r--   0        0        0     2015 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/loader_interface.py
--rw-r--r--   0        0        0    11180 2024-03-22 13:22:45.114681 sed_processor-0.1.9a5/sed/loader/mirrorutil.py
--rw-r--r--   0        0        0        0 2024-03-22 13:22:45.118681 sed_processor-0.1.9a5/sed/loader/mpes/__init__.py
--rw-r--r--   0        0        0    35405 2024-03-22 13:22:45.118681 sed_processor-0.1.9a5/sed/loader/mpes/loader.py
--rw-r--r--   0        0        0        0 2024-03-22 13:22:45.118681 sed_processor-0.1.9a5/sed/loader/sxp/__init__.py
--rw-r--r--   0        0        0    38041 2024-03-22 13:22:45.118681 sed_processor-0.1.9a5/sed/loader/sxp/loader.py
--rw-r--r--   0        0        0     7507 2024-03-22 13:22:45.118681 sed_processor-0.1.9a5/sed/loader/utils.py
--rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 sed_processor-0.1.9a5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-04 07:13:45.495365 sed_processor-0.1.9a6/LICENSE
+-rw-r--r--   0        0        0     2881 2024-04-04 07:13:45.495365 sed_processor-0.1.9a6/README.md
+-rw-r--r--   0        0        0     2840 2024-04-04 07:14:27.231338 sed_processor-0.1.9a6/pyproject.toml
+-rw-r--r--   0        0        0      127 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/binning/__init__.py
+-rw-r--r--   0        0        0    21273 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/binning/binning.py
+-rw-r--r--   0        0        0     8570 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/binning/numba_bin.py
+-rw-r--r--   0        0        0     6073 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/binning/utils.py
+-rw-r--r--   0        0        0      231 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/calibrator/__init__.py
+-rw-r--r--   0        0        0    17235 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/calibrator/delay.py
+-rw-r--r--   0        0        0    88866 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/calibrator/energy.py
+-rw-r--r--   0        0        0    83020 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/calibrator/momentum.py
+-rwxr-xr-x   0        0        0    17175 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/config/NXmpes_config.json
+-rw-r--r--   0        0        0     4692 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/config/default.yaml
+-rw-r--r--   0        0        0     6359 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/config/flash_example_config.yaml
+-rw-r--r--   0        0        0    11357 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/config/mpes_example_config.yaml
+-rw-r--r--   0        0        0      105 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/__init__.py
+-rw-r--r--   0        0        0     9017 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/config.py
+-rw-r--r--   0        0        0    17134 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/dfops.py
+-rw-r--r--   0        0        0     4182 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/metadata.py
+-rw-r--r--   0        0        0   101134 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/core/processor.py
+-rw-r--r--   0        0        0     4903 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/diagnostics.py
+-rw-r--r--   0        0        0      262 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/io/__init__.py
+-rw-r--r--   0        0        0     5939 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/io/hdf5.py
+-rw-r--r--   0        0        0     1381 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/io/nexus.py
+-rw-r--r--   0        0        0     7865 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/io/tiff.py
+-rw-r--r--   0        0        0      166 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/loader/__init__.py
+-rw-r--r--   0        0        0       14 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/loader/base/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 07:13:45.499365 sed_processor-0.1.9a6/sed/loader/base/__init__.py
+-rw-r--r--   0        0        0     6110 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/base/loader.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/flash/__init__.py
+-rw-r--r--   0        0        0    35851 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/flash/loader.py
+-rw-r--r--   0        0        0     4300 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/flash/metadata.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/generic/__init__.py
+-rw-r--r--   0        0        0     5749 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/generic/loader.py
+-rw-r--r--   0        0        0     2015 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/loader_interface.py
+-rw-r--r--   0        0        0    11180 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/mirrorutil.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/mpes/__init__.py
+-rw-r--r--   0        0        0    35421 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/mpes/loader.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/sxp/__init__.py
+-rw-r--r--   0        0        0    38089 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/sxp/loader.py
+-rw-r--r--   0        0        0     7507 2024-04-04 07:13:45.503365 sed_processor-0.1.9a6/sed/loader/utils.py
+-rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 sed_processor-0.1.9a6/PKG-INFO
```

### Comparing `sed_processor-0.1.9a5/LICENSE` & `sed_processor-0.1.9a6/LICENSE`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/README.md` & `sed_processor-0.1.9a6/README.md`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/pyproject.toml` & `sed_processor-0.1.9a6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "sed-processor"
 packages = [
     {include = "sed"}
 ]
-version = "0.1.9a5"
+version = "0.1.9a6"
 description = "Single Event Data Frame Processor: Backend to handle photoelectron resolved datastreams"
 authors = ["OpenCOMPES team <sed-processor@mpes.science>"]
 readme = "README.md"
 repository = "https://github.com/OpenCOMPES/sed"
 documentation = "https://opencompes.github.io/sed/"
 keywords = ["sed", "mpes", "flash", "arpes"]
 license = "MIT"
@@ -84,14 +84,17 @@
 
 [tool.ruff]
 include = ["sed/*.py", "tests/*.py"]
 lint.select = [
     "E", # pycodestyle
     "W", # pycodestyle
     "PL", # pylint
+    "F841", # unused variable
+    "F401", # unused imports
+    "ARG", # unused arguments
 ]
 lint.ignore = [
     "E701", # Multiple statements on one line (colon)
     "PLR0911", # Too many return statements
     "PLR0912", # Too many branches
     "PLR0913", # Too many arguments in function definition
     "PLR0915", # Too many statements
```

### Comparing `sed_processor-0.1.9a5/sed/binning/binning.py` & `sed_processor-0.1.9a6/sed/binning/binning.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/binning/numba_bin.py` & `sed_processor-0.1.9a6/sed/binning/numba_bin.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/binning/utils.py` & `sed_processor-0.1.9a6/sed/binning/utils.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/calibrator/delay.py` & `sed_processor-0.1.9a6/sed/calibrator/delay.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/calibrator/energy.py` & `sed_processor-0.1.9a6/sed/calibrator/energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
         ipw.interact(
             update,
             refid=refid_slider,
             ranges=ranges_slider,
         )
 
-        def apply_func(apply: bool):  # pylint: disable=unused-argument
+        def apply_func(apply: bool):  # noqa: ARG001
             self.add_ranges(
                 ranges_slider.value,
                 refid_slider.value,
                 traces=self.traces_normed,
             )
             self.feature_extract(peak_window=7)
             ranges_slider.close()
@@ -1137,15 +1137,15 @@
             trace1.set_ydata(correction_x)
             line1.set_xdata(x=x_center)
             trace2.set_ydata(correction_y)
             line2.set_xdata(x=y_center)
 
             fig.canvas.draw_idle()
 
-        def common_apply_func(apply: bool):  # pylint: disable=unused-argument
+        def common_apply_func(apply: bool):  # noqa: ARG001
             self.correction = {}
             self.correction["amplitude"] = correction["amplitude"]
             self.correction["center"] = correction["center"]
             self.correction["correction_type"] = correction["correction_type"]
             self.correction["creation_date"] = datetime.now().timestamp()
             amplitude_slider.close()
             x_center_slider.close()
```

### Comparing `sed_processor-0.1.9a5/sed/calibrator/momentum.py` & `sed_processor-0.1.9a6/sed/calibrator/momentum.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 
         ipw.interact(
             update,
             plane=plane_slider,
             width=width_slider,
         )
 
-        def apply_fun(apply: bool):  # pylint: disable=unused-argument
+        def apply_fun(apply: bool):  # noqa: ARG001
             start = plane_slider.value
             stop = plane_slider.value + width_slider.value
 
             selector = slice(
                 start,
                 stop,
             )
@@ -537,15 +537,15 @@
         def onclick(event):
             point_input_x.value = event.xdata
             point_input_y.value = event.ydata
             point_no_input.value = (point_no_input.value + 1) % features.shape[0]
 
         cid = fig.canvas.mpl_connect("button_press_event", onclick)
 
-        def apply_func(apply: bool):  # pylint: disable=unused-argument
+        def apply_func(apply: bool):  # noqa: ARG001
             fig.canvas.mpl_disconnect(cid)
 
             point_no_input.close()
             point_input_x.close()
             point_input_y.close()
             apply_button.close()
 
@@ -1140,15 +1140,15 @@
             update,
             scale=scale_slider,
             xtrans=xtrans_slider,
             ytrans=ytrans_slider,
             angle=angle_slider,
         )
 
-        def apply_func(apply: bool):  # pylint: disable=unused-argument
+        def apply_func(apply: bool):  # noqa: ARG001
             if transformations.get("scale", 1) != 1:
                 self.coordinate_transform(
                     transform_type="scaling",
                     xscale=transformations["scale"],
                     yscale=transformations["scale"],
                     keep=True,
                 )
@@ -1453,15 +1453,15 @@
         (marker_b,) = ax.plot(point_b[0], point_b[1], "ro")
 
         def update(
             point_a_x: int,
             point_a_y: int,
             point_b_x: int,
             point_b_y: int,
-            k_distance: float,  # pylint: disable=unused-argument
+            k_distance: float,  # noqa: ARG001
         ):
             fig.canvas.draw_idle()
             marker_a.set_xdata(point_a_x)
             marker_a.set_ydata(point_a_y)
             marker_b.set_xdata(point_b_x)
             marker_b.set_ydata(point_b_y)
 
@@ -1489,15 +1489,15 @@
             else:
                 point_b_input_x.value = event.xdata
                 point_b_input_y.value = event.ydata
                 self._state = 0
 
         cid = fig.canvas.mpl_connect("button_press_event", onclick)
 
-        def apply_func(apply: bool):  # pylint: disable=unused-argument
+        def apply_func(apply: bool):  # noqa: ARG001
             point_a = [point_a_input_x.value, point_a_input_y.value]
             point_b = [point_b_input_x.value, point_b_input_y.value]
             calibration = self.calibrate(
                 point_a=point_a,
                 point_b=point_b,
                 k_distance=k_distance,
                 equiscale=equiscale,
```

### Comparing `sed_processor-0.1.9a5/sed/config/NXmpes_config.json` & `sed_processor-0.1.9a6/sed/config/NXmpes_config.json`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/config/default.yaml` & `sed_processor-0.1.9a6/sed/config/default.yaml`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/config/flash_example_config.yaml` & `sed_processor-0.1.9a6/sed/config/flash_example_config.yaml`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/config/mpes_example_config.yaml` & `sed_processor-0.1.9a6/sed/config/mpes_example_config.yaml`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/core/config.py` & `sed_processor-0.1.9a6/sed/core/config.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/core/dfops.py` & `sed_processor-0.1.9a6/sed/core/dfops.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/core/metadata.py` & `sed_processor-0.1.9a6/sed/core/metadata.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/core/processor.py` & `sed_processor-0.1.9a6/sed/core/processor.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/diagnostics.py` & `sed_processor-0.1.9a6/sed/diagnostics.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/io/hdf5.py` & `sed_processor-0.1.9a6/sed/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/io/nexus.py` & `sed_processor-0.1.9a6/sed/io/nexus.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/io/tiff.py` & `sed_processor-0.1.9a6/sed/io/tiff.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/loader/base/loader.py` & `sed_processor-0.1.9a6/sed/loader/base/loader.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/loader/flash/loader.py` & `sed_processor-0.1.9a6/sed/loader/flash/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -746,15 +746,14 @@
         data_parquet_dir: Path,
         detector: str = "",
         parquet_path: Path = None,
         converted: bool = False,
         load_parquet: bool = False,
         save_parquet: bool = False,
         force_recreate: bool = False,
-        **kwds,
     ) -> Tuple[dd.DataFrame, dd.DataFrame]:
         """
         Handles loading and saving of parquet files based on the provided parameters.
 
         Args:
             data_parquet_dir (Path): Directory where the parquet files are located.
             detector (str, optional): Adds a identifier for parquets to distinguish multidetector
@@ -832,15 +831,15 @@
         # Save the dataframe as parquet if requested
         if save_parquet:
             dataframe_electron.compute().reset_index(drop=True).to_parquet(parquet_path)
             print("Combined parquet file saved.")
 
         return dataframe_electron, dataframe_pulse
 
-    def parse_metadata(self, scicat_token: str = None, **kwds) -> dict:
+    def parse_metadata(self, scicat_token: str = None) -> dict:
         """Uses the MetadataRetriever class to fetch metadata from scicat for each run.
 
         Returns:
             dict: Metadata dictionary
             scicat_token (str, optional):: The scicat token to use for fetching metadata
         """
         metadata_retriever = MetadataRetriever(self._config["metadata"], scicat_token)
@@ -850,20 +849,20 @@
             metadata=self.metadata,
         )
 
         return metadata
 
     def get_count_rate(
         self,
-        fids: Sequence[int] = None,
-        **kwds,
+        fids: Sequence[int] = None,  # noqa: ARG002
+        **kwds,  # noqa: ARG002
     ):
         return None, None
 
-    def get_elapsed_time(self, fids=None, **kwds):
+    def get_elapsed_time(self, fids=None, **kwds):  # noqa: ARG002
         return None
 
     def read_dataframe(
         self,
         files: Union[str, Sequence[str]] = None,
         folders: Union[str, Sequence[str]] = None,
         runs: Union[str, Sequence[str]] = None,
```

### Comparing `sed_processor-0.1.9a5/sed/loader/flash/metadata.py` & `sed_processor-0.1.9a6/sed/loader/flash/metadata.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/loader/generic/loader.py` & `sed_processor-0.1.9a6/sed/loader/generic/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,18 +97,18 @@
         except (TypeError, ValueError, NotImplementedError) as exc:
             raise ValueError(
                 "The file format cannot be understood!",
             ) from exc
 
     def get_files_from_run_id(
         self,
-        run_id: str,
-        folders: Union[str, Sequence[str]] = None,
-        extension: str = None,
-        **kwds,
+        run_id: str,  # noqa: ARG002
+        folders: Union[str, Sequence[str]] = None,  # noqa: ARG002
+        extension: str = None,  # noqa: ARG002
+        **kwds,  # noqa: ARG002
     ) -> List[str]:
         """Locate the files for a given run identifier.
 
         Args:
             run_id (str): The run identifier to locate.
             folders (Union[str, Sequence[str]], optional): The directory(ies) where the raw
                 data is located. Defaults to None.
@@ -116,18 +116,18 @@
             kwds: Keyword arguments
 
         Return:
             str: Path to the location of run data.
         """
         raise NotImplementedError
 
-    def get_count_rate(  # Pylint: disable=unused_parameter
+    def get_count_rate(
         self,
-        fids: Sequence[int] = None,
-        **kwds,
+        fids: Sequence[int] = None,  # noqa: ARG002
+        **kwds,  # noqa: ARG002
     ) -> Tuple[np.ndarray, np.ndarray]:
         """Create count rate data for the files specified in ``fids``.
 
         Args:
             fids (Sequence[int], optional): fids (Sequence[int]): the file ids to
                 include. Defaults to list of all file ids.
             kwds: Keyword arguments
@@ -135,18 +135,18 @@
         Return:
             Tuple[np.ndarray, np.ndarray]: Arrays containing countrate and seconds
             into the scan.
         """
         # TODO
         return None, None
 
-    def get_elapsed_time(  # Pylint: disable=unused_parameter
+    def get_elapsed_time(
         self,
-        fids: Sequence[int] = None,
-        **kwds,
+        fids: Sequence[int] = None,  # noqa: ARG002
+        **kwds,  # noqa: ARG002
     ) -> float:
         """Return the elapsed time in the files specified in ``fids``.
 
         Args:
             fids (Sequence[int], optional): fids (Sequence[int]): the file ids to
                 include. Defaults to list of all file ids.
             kwds: Keyword arguments
```

### Comparing `sed_processor-0.1.9a5/sed/loader/loader_interface.py` & `sed_processor-0.1.9a6/sed/loader/loader_interface.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/loader/mirrorutil.py` & `sed_processor-0.1.9a6/sed/loader/mirrorutil.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/sed/loader/mpes/loader.py` & `sed_processor-0.1.9a6/sed/loader/mpes/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,15 @@
         return df, timed_df, metadata
 
     def get_files_from_run_id(
         self,
         run_id: str,
         folders: Union[str, Sequence[str]] = None,
         extension: str = "h5",
-        **kwds,
+        **kwds,  # noqa: ARG002
     ) -> List[str]:
         """Locate the files for a given run identifier.
 
         Args:
             run_id (str): The run identifier to locate.
             folders (Union[str, Sequence[str]], optional): The directory(ies) where the raw
                 data is located. Defaults to config["core"]["base_folder"]
```

### Comparing `sed_processor-0.1.9a5/sed/loader/sxp/loader.py` & `sed_processor-0.1.9a6/sed/loader/sxp/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,20 +894,20 @@
         if metadata is None:
             metadata = {}
 
         return metadata
 
     def get_count_rate(
         self,
-        fids: Sequence[int] = None,
-        **kwds,
+        fids: Sequence[int] = None,  # noqa: ARG002
+        **kwds,  # noqa: ARG002
     ):
         return None, None
 
-    def get_elapsed_time(self, fids=None, **kwds):
+    def get_elapsed_time(self, fids=None, **kwds):  # noqa: ARG002
         return None
 
     def read_dataframe(
         self,
         files: Union[str, Sequence[str]] = None,
         folders: Union[str, Sequence[str]] = None,
         runs: Union[str, Sequence[str]] = None,
```

### Comparing `sed_processor-0.1.9a5/sed/loader/utils.py` & `sed_processor-0.1.9a6/sed/loader/utils.py`

 * *Files identical despite different names*

### Comparing `sed_processor-0.1.9a5/PKG-INFO` & `sed_processor-0.1.9a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sed-processor
-Version: 0.1.9a5
+Version: 0.1.9a6
 Summary: Single Event Data Frame Processor: Backend to handle photoelectron resolved datastreams
 Home-page: https://github.com/OpenCOMPES/sed
 License: MIT
 Keywords: sed,mpes,flash,arpes
 Author: OpenCOMPES team
 Author-email: sed-processor@mpes.science
 Requires-Python: >=3.8,<3.12
```

