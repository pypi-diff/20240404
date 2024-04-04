# Comparing `tmp/ciliaseg-0.0.4.dev20231206.tar.gz` & `tmp/ciliaseg-0.0.5.dev20240404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciliaseg-0.0.4.dev20231206.tar", last modified: Wed Dec  6 17:18:03 2023, max compression
+gzip compressed data, was "ciliaseg-0.0.5.dev20240404.tar", last modified: Thu Apr  4 19:14:30 2024, max compression
```

## Comparing `ciliaseg-0.0.4.dev20231206.tar` & `ciliaseg-0.0.5.dev20240404.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.212416 ciliaseg-0.0.4.dev20231206/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-21 17:12:23.000000 ciliaseg-0.0.4.dev20231206/MANIFEST.in
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       64 2023-12-06 17:18:03.212230 ciliaseg-0.0.4.dev20231206/PKG-INFO
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.208373 ciliaseg-0.0.4.dev20231206/ciliaseg/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:26.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      961 2023-11-21 17:12:23.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/__main__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     7482 2023-12-06 17:14:38.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/app.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.209774 ciliaseg-0.0.4.dev20231206/ciliaseg/eval/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:19.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/eval/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1205 2023-11-29 16:16:40.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/eval/model.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1130 2023-11-13 18:32:23.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/eval/polygon.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.210112 ciliaseg-0.0.4.dev20231206/ciliaseg/gui/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:41.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/gui/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    17457 2023-12-01 15:28:57.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/gui/canvas.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.210820 ciliaseg-0.0.4.dev20231206/ciliaseg/state/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:31.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/state/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5949 2023-11-22 16:49:44.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/state/image.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     7367 2023-12-01 15:28:57.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/state/stereocilia.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.211065 ciliaseg-0.0.4.dev20231206/ciliaseg/train/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:09.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/train/__init__.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.211269 ciliaseg-0.0.4.dev20231206/ciliaseg/utils/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:52.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/utils/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1091 2023-12-01 18:10:18.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/utils/io.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.211862 ciliaseg-0.0.4.dev20231206/ciliaseg/widgets/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:33.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/widgets/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    12223 2023-12-01 15:32:21.000000 ciliaseg-0.0.4.dev20231206/ciliaseg/widgets/control.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2023-12-06 17:18:03.209270 ciliaseg-0.0.4.dev20231206/ciliaseg.egg-info/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       64 2023-12-06 17:18:03.000000 ciliaseg-0.0.4.dev20231206/ciliaseg.egg-info/PKG-INFO
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      607 2023-12-06 17:18:03.000000 ciliaseg-0.0.4.dev20231206/ciliaseg.egg-info/SOURCES.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2023-12-06 17:18:03.000000 ciliaseg-0.0.4.dev20231206/ciliaseg.egg-info/dependency_links.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       54 2023-12-06 17:18:03.000000 ciliaseg-0.0.4.dev20231206/ciliaseg.egg-info/entry_points.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      118 2023-12-06 17:18:03.000000 ciliaseg-0.0.4.dev20231206/ciliaseg.egg-info/requires.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        9 2023-12-06 17:18:03.000000 ciliaseg-0.0.4.dev20231206/ciliaseg.egg-info/top_level.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       38 2023-12-06 17:18:03.212472 ciliaseg-0.0.4.dev20231206/setup.cfg
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      446 2023-12-06 17:17:53.000000 ciliaseg-0.0.4.dev20231206/setup.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.077943 ciliaseg-0.0.5.dev20240404/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-21 17:12:23.000000 ciliaseg-0.0.5.dev20240404/MANIFEST.in
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       64 2024-04-04 19:14:30.077763 ciliaseg-0.0.5.dev20240404/PKG-INFO
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.074915 ciliaseg-0.0.5.dev20240404/ciliaseg/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:26.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      961 2023-11-21 17:12:23.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/__main__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     9878 2024-04-04 19:13:28.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/app.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.076053 ciliaseg-0.0.5.dev20240404/ciliaseg/eval/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:19.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/eval/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1205 2024-04-04 19:05:36.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/eval/model.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1130 2023-11-13 18:32:23.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/eval/polygon.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.076398 ciliaseg-0.0.5.dev20240404/ciliaseg/gui/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:41.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/gui/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    18613 2024-04-04 18:37:17.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/gui/canvas.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.076818 ciliaseg-0.0.5.dev20240404/ciliaseg/state/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:31.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/state/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     6120 2024-04-04 19:10:50.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/state/image.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    10063 2024-04-04 18:36:21.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/state/stereocilia.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.076949 ciliaseg-0.0.5.dev20240404/ciliaseg/train/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:33:09.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/train/__init__.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.077148 ciliaseg-0.0.5.dev20240404/ciliaseg/utils/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:52.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/utils/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1091 2023-12-01 18:10:18.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/utils/io.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.077524 ciliaseg-0.0.5.dev20240404/ciliaseg/widgets/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        0 2023-11-08 20:32:33.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/widgets/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    12356 2024-04-04 16:05:51.000000 ciliaseg-0.0.5.dev20240404/ciliaseg/widgets/control.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-04 19:14:30.075701 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       64 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/PKG-INFO
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      607 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       54 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/entry_points.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      118 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/requires.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        9 2024-04-04 19:14:30.000000 ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/top_level.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       38 2024-04-04 19:14:30.077992 ciliaseg-0.0.5.dev20240404/setup.cfg
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      446 2024-04-04 19:13:47.000000 ciliaseg-0.0.5.dev20240404/setup.py
```

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg/__main__.py` & `ciliaseg-0.0.5.dev20240404/ciliaseg/__main__.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg/app.py` & `ciliaseg-0.0.5.dev20240404/ciliaseg/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from ciliaseg.gui.canvas import ImageCanvasWidget
 from ciliaseg.widgets.control import ControlWidget
 from ciliaseg.state.image import SEMImage
 from ciliaseg.state.stereocilia import Stereocilia
 from ciliaseg.eval.model import get_model, load_model
 import ciliaseg.utils.io
 
-__MODEL_LINK__ = 'https://www.dropbox.com/scl/fi/2y91fany1nr5aebuluvs3/Dec02_22-56-46_CHRISUBUNTU.trch?rlkey=rfa4lebpcg7jtlzasz16eicbz&dl=1'
-__MODEL_PATH__ = 'Dec02_22-56-46_CHRISUBUNTU.trch'
+__MODEL_LINK__ = 'https://www.dropbox.com/s/okp29b7v54gadg5/Jul27_SEM_Segmentaiton_model.trch?dl=1'
+__MODEL_PATH__ = 'Jul27_SEM_Segmentaiton_model.trch'
 
 class MainApplication(QMainWindow):
     def __init__(self):
         super(MainApplication, self).__init__()
 
         self.model = None
 
@@ -53,24 +53,26 @@
 
         self.resize(1200, 800)
 
         self.link_slots_and_signals()
 
         self.active_image = None
 
-        # self.active_image = SEMImage().load_image(filepath='/Users/chrisbuswinka/Dropbox (Partners HealthCare)/Annotations/Stereocilia/16k 2 16k_14w cre+ 2020-02-21 230-11.TIF')
+        # self.active_image = SEMImage().load_image(filepath='/Users/chrisbuswinka/Dropbox (Partners HealthCare)/Annotations/Stereocilia/16k 3 16k_14w cre+ 2020-02-21 230-11.TIF')
         # self.canvas.setActiveImage(self.active_image)
         # self.load_model('/Users/chrisbuswinka/Dropbox (Partners HealthCare)/public_models/Nov22_17-08-29_CHRISUBUNTU.trch')
         # self.eval_model()
 
         # assert os.path.exists('/Users/chrisbuswinka/Dropbox (Partners HealthCare)/Annotations/Stereocilia/16k 2 16k_14w cre+ 2020-02-21 230-11.csv')
         #
 
         self.canvas.zoomToScreen()
 
+        # self.load_csv(path='/Users/chrisbuswinka/Dropbox (Partners HealthCare)/Annotations/Stereocilia/16k 3 16k_14w cre+ 2020-02-21 230-11.csv')
+
     def link_slots_and_signals(self):
 
         self.control_widget.enable_move_mode_button.clicked.connect(self.canvas.enableMoveMode)
         self.control_widget.enable_draw_mode_button.clicked.connect(self.canvas.enableDrawStereociliaMode)
         self.control_widget.enable_edit_mode_button.clicked.connect(self.canvas.enableEditStereociliaMode)
         self.control_widget.delete_stereocilia_button.clicked.connect(self.canvas.deleteSelected)
         self.control_widget.selected_class_selector.currentTextChanged.connect(self.canvas.setDefaultClassLabel)
@@ -85,14 +87,15 @@
         self.control_widget.model_selector.modelFileSelected.connect(self.load_model)
         self.control_widget.default_model_button.clicked.connect(self.load_default_model)
 
         self.control_widget.open_button.clicked.connect(self.open_image)
         self.control_widget.next_file_button.clicked.connect(self.next_image)
         self.control_widget.previous_file_button.clicked.connect(self.previous_image)
         self.control_widget.save_csv_button.clicked.connect(self.save_csv)
+        self.control_widget.load_csv_button.clicked.connect(self.load_csv)
 
 
 
     def update_model_from_polygon_slider(self):
         if self.active_image is None:
             return
 
@@ -112,33 +115,45 @@
 
         self.canvas.update()
 
     def load_default_model(self):
         # path = os.path.split(__MODEL_LINK__)[-1].replace('?dl=1', '')
         path = __MODEL_PATH__
         if not os.path.exists(path):
+            print('downloading!')
             wget.download(__MODEL_LINK__)
         else:
             print('LOADED', os.path.exists(__MODEL_PATH__), __MODEL_PATH__)
         # path = '/Users/chrisbuswinka/Dropbox (Partners HealthCare)/public_models/Nov22_17-08-29_CHRISUBUNTU.trch'
+        self.model = load_model(
+            get_model(),
+            path
+        )
+        self.model.eval()
+        self.control_widget.model_selector.blockSignals(True)
         self.control_widget.model_selector.set_file(path)
-        self.load_model(path)
+        self.control_widget.model_selector.blockSignals(False)
+        print('done')
 
     def load_model(self, path):
         self.model = load_model(
             get_model(),
             path
         )
         self.model.eval()
 
     def eval_model(self):
+        print('trying to eval the model')
         if self.model is None or self.active_image is None:
             return
-        self.active_image.eval_model(self.model).update_polygons(
-            self.control_widget.polygon_approx_slider.value()).populate_stereocilia_from_model_out()  # adds stereocilia internally
+        (self.active_image
+         .eval_model(self.model, 0, 1)
+         .update_polygons(self.control_widget.polygon_approx_slider.value())
+         .populate_stereocilia_from_model_out()
+         )  # adds stereocilia internally
         self.canvas.update()
 
     def set_active_image(self, image: SEMImage):
         self.active_image = image
         self.canvas.setActiveImage(image)
         self.update()
 
@@ -172,10 +187,57 @@
     def save_csv(self):
         """ save the segmentation masks as a csv for the image, suitable for training """
         if self.active_image is not None:
             filepath, ext = os.path.splitext(self.active_image.filepath)
             print(filepath + '.csv')
             ciliaseg.utils.io.save_image_as_csv(self.active_image, filepath + '.csv')
 
+    def load_csv(self, path = None):
+        if self.active_image is not None:
+            if not path:
+                file_path, _ = QFileDialog.getOpenFileName(self, 'Select Saved CSV File')
+            else:
+                file_path = path
+
+            stereocilia_list = []
+            assert os.path.exists(file_path), 'shit doesnt exist!'
+            if file_path:
+                with open(file_path, 'r') as file:
+                    keys = file.readline().split(',')
+                    print(keys)
+
+                    line = file.readline()
+                    while line:
+                        line = line.split(',')
+                        stereocilia_list.append({k: v for k, v in zip(keys, line)})
+                        line = file.readline()
+
+            self.active_image.clear_stereocilia()
+
+            for _s in stereocilia_list:
+                """
+                            poly = polygons[i]
+                poly: List[QPointF] = ciliaseg.eval.polygon.polygon_to_qt(poly)
+
+                s = Stereocilia() \
+                    .set_score(scores[i]) \
+                    .set_label(int(labels[i]) - 1) \
+                    .set_vertices(poly)
+                """
+                print('verts')
+                print( _s['x_vertices'].replace('[', '').replace(']','').split(' '))
+                x = [float(x) for x in _s['x_vertices'].replace('[', '').replace(']','').split(' ') if x]
+                y = [float(y) for y in _s['y_vertices'].replace('[', '').replace(']','').split(' ') if y]
+                poly = [QPointF(_x, _y) for _x, _y in zip(x, y)]
+
+                s = (Stereocilia()
+                     .set_score(float(_s['score']))
+                     .set_label(_s['type'])
+                     .set_vertices(poly)
+                     .set_gt()
+                     )
+                self.active_image.add_stereocilia(s)
+
+
     def save_overlay(self):
         """ save the segmentation masks as an overlay, for publicaiton """
         print('notimplemented')
```

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg/eval/model.py` & `ciliaseg-0.0.5.dev20240404/ciliaseg/eval/model.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg/eval/polygon.py` & `ciliaseg-0.0.5.dev20240404/ciliaseg/eval/polygon.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg/gui/canvas.py` & `ciliaseg-0.0.5.dev20240404/ciliaseg/gui/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         self._default_stereocilia_label = 'short'  # short middle tall
         self.polygon_buffer = []
 
         # polygon for stereocila region drawing
         self._draw_mouse_position = None
         self._mouse_position = None
         self._editable_vertex = None
+        self._potential_new_vert = None
 
         # image viewer state
         self.scale = 1.0
         self._temp_ratio = (0.0, 0.0)
 
         # where is the mouse?
         self.mouse_position = QPointF()
@@ -257,14 +258,20 @@
             press = QPointF(_x, _y)
 
             if any(s.is_selected() for s in self.active_image.get_stereocilia()):
                 for s in self.active_image.get_stereocilia():
                     if s.is_selected():
                         self._editable_vertex: QPointF = s.return_clicked_vertex(press, self.VERTEX_CLICK_TRH)
 
+                        if self._editable_vertex is None:
+                            self._potential_new_vert = s.closest_point_on_polygon(press, self.VERTEX_CLICK_TRH*2500)
+                            s.insert_vertex(self._potential_new_vert)
+                            self._editable_vertex = self._potential_new_vert
+                            self._potential_new_vert = None
+
             if not self._editable_vertex:
                 self.selected_stereocilia.emit('')
                 for s in self.active_image.get_stereocilia():
                     s.deselect()
                 for s in self.active_image.get_stereocilia():
                     if s.is_inside(press):
                         s.select()
@@ -296,14 +303,19 @@
         if self.draw_stereocilia_mode and self.polygon_buffer:
             self._draw_mouse_position = QPointF(_x, _y)
 
         if self.edit_stereocilia_mode and self._editable_vertex:
             self._editable_vertex.setX(_x)
             self._editable_vertex.setY(_y)
 
+        if self.edit_stereocilia_mode and not self._editable_vertex:
+            selected = self.active_image.get_selected()
+            s = selected[0] if selected else None
+            if s is not None:
+                self._potential_new_vert = self.active_image.get_selected()[0].closest_point_on_polygon(QPointF(_x, _y), self.VERTEX_CLICK_TRH * 2500)
 
         self.update()
 
     def mouseReleaseEvent(self, event: QMouseEvent) -> None:
         self.mouse_position = event.position()
         pos = event.position()
         _x = (pos.x() / self.scale) - self._pixmap_offset.x()
@@ -391,14 +403,15 @@
         self.painter.scale(self.scale, self.scale)
 
         self._paint_pixmap()  # draws the image
 
         if self.edit_stereocilia_mode or self.draw_stereocilia_mode:
             self._paint_center_cross()
             self._paint_polygon_buffer()
+            self._paint_potential_vert()
         self._paint_current_mode()
         self._paint_stereocilia()
         self.painter.end()
 
     def _paint_center_cross(self):
         p = self.painter
         _x, _y = (
@@ -449,14 +462,28 @@
             raise RuntimeError("UNKOWN MODE")
 
         p.drawText(QPointF(x, y), text)
 
         p.setPen(_pen)
         p.setFont(_font)
 
+    def _paint_potential_vert(self):
+        if not self._potential_new_vert:
+            return
+
+        p = self.painter
+        pen = QPen()
+        pen.setWidthF(6 / self.scale)
+        color = QColor('yellow')
+        pen.setColor(color)
+
+        p.setPen(pen)
+
+        p.drawPoint(self._potential_new_vert + self._pixmap_offset)
+
     def _paint_polygon_buffer(self):
         if not self.polygon_buffer:
             return
 
         p = self.painter
         pen = QPen()
         pen.setWidthF(2 / self.scale)
```

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg/state/image.py` & `ciliaseg-0.0.5.dev20240404/ciliaseg/state/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,36 +48,40 @@
         self._candidate_stereocilia = []
 
         self.nms_thr = 0.5
         self.stereocilia_thr = 0.5
 
         self._display_image_buffer = None
 
-    def eval_model(self, model: nn.Module):
+    def eval_model(self, model: nn.Module, mean: float = .3717, std: float = .1897):
         image: Tensor = torch.from_numpy(self.image)  # [X, Y ,3]
-        image = image.permute(2, 0, 1).div(255).float()
+        image = image.permute(2, 0, 1).div(255).sub(mean).div(std).float()
 
         with torch.no_grad():
             out = model([image])[0]
 
         self.model_out = out
+        print(out)
         self.model_out['polygons'] = [
             ciliaseg.eval.polygon.find_contours(out['masks'][i, 0, ...].permute(1,0).numpy()) for i in range(out['scores'].shape[0])]
         return self
 
     def update_polygons(self, polygon_threshold: float = 0.25):
         if self.model_out is None:
             return
 
         self.model_out['polygons-downsampled'] = [
             ciliaseg.eval.polygon.approximate_polygon(c, tolerance=polygon_threshold) for c in self.model_out['polygons']]
 
         return self
 
     def populate_stereocilia_from_model_out(self):
+        if not self.model_out:
+            return
+
 
         to_delete = [s for s in self.get_stereocilia() if not s.is_ground_truth()]
         self.set_stereocilia([s for s in self.get_stereocilia() if s.is_ground_truth()])
         del to_delete
 
         scores = self.model_out['scores']
         masks = self.model_out['masks']  # [N, 1, X, Y]
@@ -192,8 +196,9 @@
     def populate_from_network_output(self, data_dict: Dict[str, Tensor]):
         raise NotImplemented
         return self
 
     def clear_stereocilia(self):
         self.seleted = None
         self.stereocilia = []
+        self._candidate_stereocilia = []
         return self
```

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg/utils/io.py` & `ciliaseg-0.0.5.dev20240404/ciliaseg/utils/io.py`

 * *Files identical despite different names*

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg/widgets/control.py` & `ciliaseg-0.0.5.dev20240404/ciliaseg/widgets/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,17 +205,17 @@
         self.label.setAlignment(Qt.AlignLeft)
         self.label.setStyleSheet("""
         QTextEdit {
             background-color: rgba(0,0,0,0);
             font: 12px;
         }
         """)
+        self.modelFileSelected.emit(str(self.file_path))
         self.file_path = _justfile
         self.label.update()
-        self.modelFileSelected.emit(str(self.file_path))
 
     def remove_file(self):
         self.label.setText('NOT SET')
         self.label.text_set = False
         self.label.setReadOnly(True)
         self.label.setAlignment(Qt.AlignCenter)
         self.label.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
@@ -228,15 +228,15 @@
             border: 1px solid black;
         }
         """)
 
     def select_file(self):
         # Open a file dialog to choose a file
         file_path, _ = QFileDialog.getOpenFileName(self, 'Select File')
-
+        print(file_path)
         if file_path:
             # Update the label with the selected file path
             if not self.validate_model_file(self.file_path):
                 self.file_path = None
                 return
 
             self.file_path = file_path
@@ -265,14 +265,16 @@
 class ControlWidget(QWidget):
     def __init__(self):
         super(ControlWidget, self).__init__()
 
 
         self.open_button = QPushButton('Open')
         self.save_csv_button = QPushButton('Save CSV')
+        self.load_csv_button = QPushButton('Load from CSV')
+
         self.save_overlay_button = QPushButton('Save Overlay')
         self.next_file_button = QPushButton('-->')
         self.previous_file_button = QPushButton('<--')
         self.enable_move_mode_button = QPushButton('Move')
         self.enable_draw_mode_button = QPushButton('Draw')
         self.enable_edit_mode_button = QPushButton('Edit')
         self.run_model_button = QPushButton('Eval Model')
@@ -294,14 +296,15 @@
 
         self.model_selector = ModelFileSelector()
 
         file_group = QGroupBox('File')
         _layout = QVBoxLayout()
         _layout.addWidget(self.open_button)
         _layout.addWidget(self.save_csv_button)
+        _layout.addWidget(self.load_csv_button)
         # _layout.addWidget(self.save_overlay_button)
         _lr_layout = QHBoxLayout()
         _lr_layout.addWidget(self.previous_file_button)
         _lr_layout.addWidget(self.next_file_button)
         _lr_layout.setContentsMargins(0,0,0,0)
         _layout.addLayout(_lr_layout)
         file_group.setLayout(_layout)
```

### Comparing `ciliaseg-0.0.4.dev20231206/ciliaseg.egg-info/SOURCES.txt` & `ciliaseg-0.0.5.dev20240404/ciliaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

