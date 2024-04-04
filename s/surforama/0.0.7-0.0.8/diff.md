# Comparing `tmp/surforama-0.0.7.tar.gz` & `tmp/surforama-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surforama-0.0.7.tar", last modified: Wed Apr  3 05:57:14 2024, max compression
+gzip compressed data, was "surforama-0.0.8.tar", last modified: Thu Apr  4 13:27:12 2024, max compression
```

## Comparing `surforama-0.0.7.tar` & `surforama-0.0.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.406288 surforama-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.394288 surforama-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.398288 surforama-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-03 05:57:03.000000 surforama-0.0.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-03 05:57:03.000000 surforama-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 05:57:03.000000 surforama-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 05:57:03.000000 surforama-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 05:57:03.000000 surforama-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-03 05:57:14.406288 surforama-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 05:57:03.000000 surforama-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.398288 surforama-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   112422 2024-04-03 05:57:03.000000 surforama-0.0.7/examples/example_usecase_stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-03 05:57:03.000000 surforama-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-03 05:57:14.406288 surforama-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.394288 surforama-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.398288 surforama-0.0.7/src/surforama/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/_tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/data/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/data/_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/gui/qt_mesh_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/gui/qt_point_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/gui/qt_surface_picker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/io/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/_reader_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/io/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/_tests/test_star.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/star.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/utils/napari.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2606156 2024-04-03 05:57:03.000000 surforama-0.0.7/surforama_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 05:57:03.000000 surforama-0.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.211330 surforama-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.199330 surforama-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.207330 surforama-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-04 13:27:01.000000 surforama-0.0.8/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-04 13:27:01.000000 surforama-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 13:27:01.000000 surforama-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-04 13:27:01.000000 surforama-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 13:27:01.000000 surforama-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-04 13:27:12.211330 surforama-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 13:27:01.000000 surforama-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.207330 surforama-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   112422 2024-04-04 13:27:01.000000 surforama-0.0.8/examples/example_usecase_stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-04 13:27:01.000000 surforama-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-04 13:27:12.211330 surforama-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.199330 surforama-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.207330 surforama-0.0.8/src/surforama/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.207330 surforama-0.0.8/src/surforama/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/_tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 13:27:12.000000 surforama-0.0.8/src/surforama/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12113 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.207330 surforama-0.0.8/src/surforama/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/data/_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.211330 surforama-0.0.8/src/surforama/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/gui/qt_mesh_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/gui/qt_point_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/gui/qt_surface_picker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.211330 surforama-0.0.8/src/surforama/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/io/_reader_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.211330 surforama-0.0.8/src/surforama/io/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/io/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/io/_tests/test_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/io/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/io/star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.211330 surforama-0.0.8/src/surforama/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/utils/napari.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-04 13:27:01.000000 surforama-0.0.8/src/surforama/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:12.211330 surforama-0.0.8/src/surforama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-04 13:27:12.000000 surforama-0.0.8/src/surforama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 13:27:12.000000 surforama-0.0.8/src/surforama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:27:12.000000 surforama-0.0.8/src/surforama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 13:27:12.000000 surforama-0.0.8/src/surforama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 13:27:12.000000 surforama-0.0.8/src/surforama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 13:27:12.000000 surforama-0.0.8/src/surforama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2606156 2024-04-04 13:27:01.000000 surforama-0.0.8/surforama_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 13:27:01.000000 surforama-0.0.8/tox.ini
```

### Comparing `surforama-0.0.7/.github/workflows/test_and_deploy.yml` & `surforama-0.0.8/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/.gitignore` & `surforama-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/.pre-commit-config.yaml` & `surforama-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/LICENSE` & `surforama-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/PKG-INFO` & `surforama-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surforama
-Version: 0.0.7
+Version: 0.0.8
 Summary: a tool for using surfaces to explore volumetric data in napari
 Home-page: https://github.com/cellcanvas/surforama
 Author: Kyle Harrington
 Author-email: surforama@kyleharrington.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cellcanvas/surforama/issues
 Project-URL: Documentation, https://github.com/cellcanvas/surforama#README.md
```

### Comparing `surforama-0.0.7/README.md` & `surforama-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/examples/example_usecase_stats.ipynb` & `surforama-0.0.8/examples/example_usecase_stats.ipynb`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/pyproject.toml` & `surforama-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/setup.cfg` & `surforama-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/_cli.py` & `surforama-0.0.8/src/surforama/_cli.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/_tests/test_geometry.py` & `surforama-0.0.8/src/surforama/_tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/_tests/test_widget.py` & `surforama-0.0.8/src/surforama/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/app.py` & `surforama-0.0.8/src/surforama/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         viewer: napari.Viewer,
         surface_layer: Optional[Surface] = None,
         volume_layer: Optional[Image] = None,
         parent: Optional[QWidget] = None,
     ):
         super().__init__(parent=parent)
         self.viewer = viewer
+        self._enabled = False
 
         # make the layer selection widget
         self._layer_selection_widget = magicgui(
             self._set_layers,
             surface_layer={"choices": self._get_valid_surface_layers},
             image_layer={"choices": self._get_valid_image_layers},
             call_button="start surfing",
@@ -107,14 +108,47 @@
         self.layout().addWidget(self.picking_widget)
         self.layout().addWidget(self.point_writer_widget)
         self.layout().addStretch()
 
         # set the layers
         self._set_layers(surface_layer=surface_layer, image_layer=volume_layer)
 
+    @property
+    def enabled(self) -> bool:
+        return self._enabled
+
+    @enabled.setter
+    def enabled(self, enabled: bool):
+        if enabled == self.enabled:
+            # no change
+            return
+
+        if enabled:
+            # make the widgets visible
+            self.slider.setVisible(True)
+            self.sampling_depth_slider.setVisible(True)
+            self.picking_widget.setVisible(True)
+            self.point_writer_widget.setVisible(True)
+            self.slider_title.setVisible(True)
+            self.slider_value.setVisible(True)
+            self.sampling_depth_title.setVisible(True)
+            self.sampling_depth_value.setVisible(True)
+        else:
+            # make the widgets visible
+            self.slider.setVisible(False)
+            self.sampling_depth_slider.setVisible(False)
+            self.picking_widget.setVisible(False)
+            self.point_writer_widget.setVisible(False)
+            self.slider_title.setVisible(False)
+            self.slider_value.setVisible(False)
+            self.sampling_depth_title.setVisible(False)
+            self.sampling_depth_value.setVisible(False)
+
+        self._enabled = enabled
+
     def _set_layers(
         self,
         surface_layer: Surface,
         image_layer: Image,
     ):
         self.surface_layer = surface_layer
         self.image_layer = image_layer
@@ -134,40 +168,52 @@
         self.color_values = np.ones((self.mesh.vertices.shape[0],))
 
         self.surface_layer.data = (
             self.vertices,
             self.faces,
             self.color_values,
         )
+        self.surface_layer.shading = "none"
         self.surface_layer.refresh()
 
         self.normals = self.mesh.vertex_normals
         self.volume = image_layer.data.astype(np.float32)
 
-        # make the widgets visible
-        self.slider.setVisible(True)
-        self.sampling_depth_slider.setVisible(True)
-        self.picking_widget.setVisible(True)
-        self.point_writer_widget.setVisible(True)
-        self.slider_title.setVisible(True)
-        self.slider_value.setVisible(True)
-        self.sampling_depth_title.setVisible(True)
-        self.sampling_depth_value.setVisible(True)
+        self.enabled = True
 
     def _get_valid_surface_layers(self, combo_box) -> List[Surface]:
         return [
             layer
             for layer in self._viewer.layers
             if isinstance(layer, napari.layers.Surface)
         ]
 
     def _on_layer_update(self, event=None):
         """When the model updates the selected layer, update widgets."""
         self._layer_selection_widget.reset_choices()
 
+        # check if the stored layers are still around
+        layer_deleted = False
+        if (
+            self.surface_layer is not None
+        ) and self.surface_layer not in self.viewer.layers:
+            # remove the surface layer if it has been deleted.
+            self.surface_layer = None
+            layer_deleted = True
+
+        if (self.image_layer is not None) and (
+            self.image_layer not in self.viewer.layers
+        ):
+            # remove the surface layer if it has been deleted.
+            self.image_layer = None
+            layer_deleted = True
+
+        if layer_deleted:
+            self.enabled = False
+
     def _get_valid_image_layers(self, combo_box) -> List[Image]:
         return [
             layer
             for layer in self._viewer.layers
             if isinstance(layer, napari.layers.Image)
         ]
```

### Comparing `surforama-0.0.7/src/surforama/data/_datasets.py` & `surforama-0.0.8/src/surforama/data/_datasets.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/gui/qt_mesh_generator.py` & `surforama-0.0.8/src/surforama/gui/qt_mesh_generator.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/gui/qt_point_io.py` & `surforama-0.0.8/src/surforama/gui/qt_point_io.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/gui/qt_surface_picker.py` & `surforama-0.0.8/src/surforama/gui/qt_surface_picker.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import napari
 import numpy as np
 from qtpy.QtCore import Qt
 from qtpy.QtWidgets import (
     QGroupBox,
     QPushButton,
-    QSlider,
     QVBoxLayout,
     QWidget,
 )
+from superqt import QLabeledDoubleSlider
 
 if TYPE_CHECKING:
     from surforama import QtSurforama
 from surforama.constants import (
     NAPARI_NORMAL_0,
     NAPARI_NORMAL_1,
     NAPARI_NORMAL_2,
@@ -36,67 +36,117 @@
     def __init__(
         self, surforama: "QtSurforama", parent: Optional[QWidget] = None
     ):
         super().__init__("Pick on surface", parent=parent)
         self.surforama = surforama
         self.points_layer = None
         self.normal_vectors_layer = None
+        self.up_vectors_layer = None
+
+        self.surforama.viewer.layers.events.removed.connect(
+            self._on_layer_update
+        )
 
         # initialize orientation data
         # todo store elsewhere (e.g., layer features)
         self.normal_vectors = np.empty((0, 3))
         self.up_vectors = np.empty((0, 3))
         self.rotations = np.empty((0,))
 
         # enable state
-        self.enabled = False
+        self._enabled = False
 
         # make the activate button
         self.enable_button = QPushButton(self.ENABLE_BUTTON_TEXT)
         self.enable_button.clicked.connect(self._on_enable_button_pressed)
 
         # make the rotation slider
-        self.rotation_slider = QSlider()
-        self.rotation_slider.setOrientation(Qt.Horizontal)
+        self.rotation_slider = QLabeledDoubleSlider(Qt.Orientation.Horizontal)
         self.rotation_slider.setMinimum(-180)
         self.rotation_slider.setMaximum(180)
         self.rotation_slider.setValue(0)
         self.rotation_slider.valueChanged.connect(self._update_rotation)
 
         # make the layout
         self.setLayout(QVBoxLayout())
         self.layout().addWidget(self.enable_button)
         self.layout().addWidget(self.rotation_slider)
 
-    def _on_enable_button_pressed(self, event):
-        # toggle enabled
-        if self.enabled:
-            # if currently enabled, toggle to disabled
-            self.enabled = False
-            self.enable_button.setText(self.ENABLE_BUTTON_TEXT)
-
-        else:
-            # if disabled, toggle to enabled
-            self.enabled = True
+    @property
+    def enabled(self) -> bool:
+        return self._enabled
+
+    @enabled.setter
+    def enabled(self, enabled: bool):
+        if enabled == self.enabled:
+            # do nothing
+            return
+        if enabled:
             self.enable_button.setText(self.DISABLE_BUTTON_TEXT)
 
             if self.points_layer is None:
                 self._initialize_points_layer()
             if self.normal_vectors_layer is None:
-                self._initialize_vectors_layers()
+                self._initialize_normal_vectors_layers()
+            if self.up_vectors_layer is None:
+                self._initialize_up_vectors_layers()
             self.points_layer.visible = True
 
-        self._on_enable_change()
+            # update the vectors layer
+            self._on_points_update()
 
-    def _on_enable_change(self):
-        if self.enabled:
+            # add the mouse callbacks
             self._connect_mouse_callbacks()
+
         else:
+            self.enable_button.setText(self.ENABLE_BUTTON_TEXT)
+
+            # remove the mouse callbacks
             self._disconnect_mouse_callbacks()
 
+        self._enabled = enabled
+
+    def _on_layer_update(self):
+        # check if the stored layers are still around
+        viewer = self.surforama.viewer
+        layer_deleted = False
+        if (self.points_layer is not None) and (
+            self.points_layer not in viewer.layers
+        ):
+            # remove the surface layer if it has been deleted.
+            self.points_layer = None
+            layer_deleted = True
+
+        if (self.normal_vectors_layer is not None) and (
+            self.normal_vectors_layer not in viewer.layers
+        ):
+            # remove the surface layer if it has been deleted.
+            self.normal_vectors_layer = None
+            layer_deleted = True
+
+        if (self.up_vectors_layer is not None) and (
+            self.up_vectors_layer not in viewer.layers
+        ):
+            # remove the surface layer if it has been deleted.
+            self.up_vectors_layer = None
+            layer_deleted = True
+
+        if layer_deleted:
+            self.enabled = False
+
+    def _on_enable_button_pressed(self, event):
+        # toggle enabled
+        if self.enabled:
+            # if currently enabled, toggle to disabled
+            self.enabled = False
+
+        else:
+            # if disabled, toggle to enabled
+            self.enabled = True
+
     def _update_rotation(self, value):
         """Callback function to update the rotation of the selected points."""
         selected_points = list(self.points_layer.selected_data)
         self.rotations[selected_points] = value
 
         rotation_radians = value * (np.pi / 180)
         new_rotations = rotation_radians * np.ones(
@@ -123,23 +173,29 @@
 
     def _initialize_points_layer(self):
         self.points_layer = self.surforama.viewer.add_points(
             ndim=3, size=3, face_color="magenta"
         )
         self.points_layer.shading = "spherical"
         self.points_layer.events.data.connect(self._on_points_update)
+        self.points_layer.selected_data.events.items_changed.connect(
+            self._on_point_selection
+        )
         self.surforama.viewer.layers.selection = [self.surforama.surface_layer]
 
-    def _initialize_vectors_layers(self):
+    def _initialize_normal_vectors_layers(self):
         self.normal_vectors_layer = self.surforama.viewer.add_vectors(
             ndim=3,
             length=10,
             edge_color="cornflowerblue",
             name="surface normals",
         )
+        self.surforama.viewer.layers.selection = [self.surforama.surface_layer]
+
+    def _initialize_up_vectors_layers(self):
         self.up_vectors_layer = self.surforama.viewer.add_vectors(
             ndim=3, length=10, edge_color="orange", name="up vectors"
         )
         self.surforama.viewer.layers.selection = [self.surforama.surface_layer]
 
     def _on_points_update(self, event=None):
         """Update the vectors layers when the points data are updated."""
@@ -150,14 +206,29 @@
         self.normal_vectors_layer.data = normal_data
         self.up_vectors_layer.data = up_data
 
         # colors were being reset - this might not be necessary
         self.normal_vectors_layer.edge_color = "purple"
         self.up_vectors_layer.edge_color = "orange"
 
+    def _on_point_selection(self, event=None):
+        selected_points = list(self.points_layer.selected_data)
+        if len(selected_points) == 0:
+            # no points selected
+            return
+        rotation_column = self.points_layer.features.columns.get_loc(ROTATION)
+        rotations = self.points_layer.features.iloc[
+            selected_points, rotation_column
+        ].to_numpy()
+        rotation = rotations[0]
+
+        self.rotation_slider.blockSignals(True)
+        self.rotation_slider.setValue((180 / np.pi) * rotation)
+        self.rotation_slider.blockSignals(False)
+
     def _connect_mouse_callbacks(self):
         self.surforama.surface_layer.mouse_drag_callbacks.append(
             self._find_point_on_click
         )
 
     def _disconnect_mouse_callbacks(self):
         self.surforama.surface_layer.mouse_drag_callbacks.remove(
```

### Comparing `surforama-0.0.7/src/surforama/io/_reader_plugin.py` & `surforama-0.0.8/src/surforama/io/_reader_plugin.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/io/_tests/test_star.py` & `surforama-0.0.8/src/surforama/io/_tests/test_star.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/io/mesh.py` & `surforama-0.0.8/src/surforama/io/mesh.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/io/star.py` & `surforama-0.0.8/src/surforama/io/star.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/napari.yaml` & `surforama-0.0.8/src/surforama/napari.yaml`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/utils/geometry.py` & `surforama-0.0.8/src/surforama/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama/utils/napari.py` & `surforama-0.0.8/src/surforama/utils/napari.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,18 @@
     Returns
     -------
     normals_data : np.ndarray
         The Vectors layer data for the normal vectors
     up_data : np.ndarray
         The Vectors layer data for the up vectors
     """
+    # check in the points layer has any data
+    if len(point_coordinates) == 0:
+        # if there are no points, there are no vectors
+        return np.empty((0, 2, 3)), np.empty((0, 2, 3))
     # get the vectors
     normal_vectors = features_table[
         [NAPARI_NORMAL_0, NAPARI_NORMAL_1, NAPARI_NORMAL_2]
     ].to_numpy()
     up_vectors = features_table[
         [NAPARI_UP_0, NAPARI_UP_1, NAPARI_UP_2]
     ].to_numpy()
```

### Comparing `surforama-0.0.7/src/surforama/utils/stats.py` & `surforama-0.0.8/src/surforama/utils/stats.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/src/surforama.egg-info/PKG-INFO` & `surforama-0.0.8/src/surforama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surforama
-Version: 0.0.7
+Version: 0.0.8
 Summary: a tool for using surfaces to explore volumetric data in napari
 Home-page: https://github.com/cellcanvas/surforama
 Author: Kyle Harrington
 Author-email: surforama@kyleharrington.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cellcanvas/surforama/issues
 Project-URL: Documentation, https://github.com/cellcanvas/surforama#README.md
```

### Comparing `surforama-0.0.7/src/surforama.egg-info/SOURCES.txt` & `surforama-0.0.8/src/surforama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/surforama_screenshot.png` & `surforama-0.0.8/surforama_screenshot.png`

 * *Files identical despite different names*

### Comparing `surforama-0.0.7/tox.ini` & `surforama-0.0.8/tox.ini`

 * *Files identical despite different names*

