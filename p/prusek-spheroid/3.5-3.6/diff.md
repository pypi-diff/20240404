# Comparing `tmp/prusek_spheroid-3.5.tar.gz` & `tmp/prusek_spheroid-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-3.5.tar", last modified: Tue Apr  2 12:35:38 2024, max compression
+gzip compressed data, was "prusek_spheroid-3.6.tar", last modified: Thu Apr  4 17:20:11 2024, max compression
```

## Comparing `prusek_spheroid-3.5.tar` & `prusek_spheroid-3.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:35:38.168375 prusek_spheroid-3.5/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:35:38.168142 prusek_spheroid-3.5/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.5/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:35:38.166933 prusek_spheroid-3.5/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    16517 2024-04-02 12:34:56.000000 prusek_spheroid-3.5/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    35159 2024-04-02 11:58:27.000000 prusek_spheroid-3.5/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.5/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.5/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7200 2024-04-02 12:11:35.000000 prusek_spheroid-3.5/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3466 2024-04-02 09:37:18.000000 prusek_spheroid-3.5/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3705 2024-04-02 09:37:18.000000 prusek_spheroid-3.5/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-3.5/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.5/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:35:38.167916 prusek_spheroid-3.5/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:35:38.000000 prusek_spheroid-3.5/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      514 2024-04-02 12:35:38.000000 prusek_spheroid-3.5/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-02 12:35:38.000000 prusek_spheroid-3.5/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-02 12:35:38.000000 prusek_spheroid-3.5/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-02 12:35:38.000000 prusek_spheroid-3.5/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-02 12:35:38.168421 prusek_spheroid-3.5/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-02 12:35:33.000000 prusek_spheroid-3.5/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:20:11.062619 prusek_spheroid-3.6/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-04 17:20:11.062224 prusek_spheroid-3.6/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.6/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:20:11.060922 prusek_spheroid-3.6/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    17715 2024-04-04 06:15:38.000000 prusek_spheroid-3.6/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    44718 2024-04-04 17:15:00.000000 prusek_spheroid-3.6/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.6/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.6/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-3.6/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-3.6/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     6737 2024-04-04 14:40:14.000000 prusek_spheroid-3.6/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3641 2024-04-03 14:52:18.000000 prusek_spheroid-3.6/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-3.6/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.6/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-04 17:20:11.062013 prusek_spheroid-3.6/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      544 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-04 17:20:11.000000 prusek_spheroid-3.6/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-04 17:20:11.062661 prusek_spheroid-3.6/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-04 17:19:48.000000 prusek_spheroid-3.6/setup.py
```

### Comparing `prusek_spheroid-3.5/PKG-INFO` & `prusek_spheroid-3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.5
+Version: 3.6
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.5/README.md` & `prusek_spheroid-3.6/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.5/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-3.6/prusek_spheroid/ContoursClassGUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import json
 import pandas as pd
 from prusek_spheroid import file_management as fm
 from prusek_spheroid import selection_dialog as sd
 from prusek_spheroid import metrics as metric
 from prusek_spheroid.methods import BaseImageProcessing
 from prusek_spheroid import characteristic_functions as cf
+from prusek_spheroid import image_processing as ip
 
 
 class Contours(BaseImageProcessing):
 
     def __init__(self, master, adresaDatasetu, adresa_output, projekt, algorithm, parameters, show_img, function,
                  contours_state, detect_corrupted, create_json, calculate_properties,
                  progress_window=None):
@@ -33,35 +34,43 @@
         self.parameters = parameters
         self.contours_state = contours_state
         self.detect_corrupted = detect_corrupted
         self.create_json = create_json
         self.calculate_properties = calculate_properties
         self.f = function
         self.progress_window = progress_window
+        self.min_area = self.parameters["min_area"]
 
         fm.create_directory(os.path.dirname(self.output_json_path), delete=True)
         fm.create_directory(self.output_images_path, delete=True)
         fm.create_directory(f"{self.output_segmented_path}/masks", delete=True)
         fm.create_directory(f"{self.output_segmented_path}/results", delete=True)
 
     def run(self):
+        dialog = None
         all_contour_data = []
         filenames = os.listdir(self.adresaDatasetu)
         total_files = len(filenames)
         print(f"loaded {total_files} dataset images")
         self.counter = 1
 
         if self.contours_state == "select":
             dialog = sd.SelectionDialog(self.master, self.counter, total_files, self.user_decision_lock)
 
         for filename in os.listdir(self.adresaDatasetu):
             if filename.lower().endswith(('.png', '.jpg', '.jpeg', '.bmp', '.tiff', '.tif')):
-                self.user_decision_lock.acquire()
+                if self.contours_state == "select":
+                    self.user_decision_lock.acquire()
+
+                img_path = os.path.join(self.adresaDatasetu, filename)
+                img = cv.imread(img_path)
 
-                img = cv.imread(os.path.join(self.adresaDatasetu, filename))
+                if img is None:
+                    print(f"FAILED to load image: {img_path}")
+                    continue  # Skip to the next image
 
                 img_gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
 
                 img_binary, inner_contours_mask = self.apply_segmentation_algorithm(self.algorithm, self.parameters,
                                                                                     img_gray,
                                                                                     self.contours_state,
                                                                                     self.detect_corrupted)
@@ -77,48 +86,59 @@
                 else:
                     mask_with = None
 
                 contours, hierarchy = cv.findContours(img_binary, cv.RETR_TREE, cv.CHAIN_APPROX_SIMPLE)
 
                 height, width = np.shape(img_binary)
 
+                contours, hierarchy = ip.filter_contours_on_frame(contours, hierarchy, (height, width), self.min_area, self.detect_corrupted)
+
                 if self.create_json:
                     if not cv.imwrite(f"{self.output_images_path}/{filename}", img):
                         print(f"FAILED to save image: {self.output_images_path}/{filename}")
 
+                img_with = img.copy()
                 if not contours:
                     if self.create_json:
                         self.coco_data = fm.convert_contours_to_coco([], [], height, width,
                                                                      filename,
                                                                      self.counter,
                                                                      self.coco_data)
-                    cv.line(img, (0, 0), (width - 1, height - 1), (0, 0, 255), 5)
-                    cv.line(img, (0, height - 1), (width - 1, 0), (0, 0, 255), 5)
+                    cv.line(img_with, (0, 0), (width - 1, height - 1), (0, 0, 255), 5)
+                    cv.line(img_with, (0, height - 1), (width - 1, 0), (0, 0, 255), 5)
+                    cv.line(img_without, (0, 0), (width - 1, height - 1), (0, 0, 255), 5)
+                    cv.line(img_without, (0, height - 1), (width - 1, 0), (0, 0, 255), 5)
                 else:
 
                     inner_contours = []
                     outer_contours = []
                     img_without = img.copy()
                     if self.contours_state == "all" or self.contours_state == "select":
-                        img_with = img.copy()
 
                         for i, contour in enumerate(contours):
                             # Získání indexu rodiče pro aktuální konturu
-                            parent_index = hierarchy[0][i][3]
-
-                            if parent_index != -1:
+                            parent_index = hierarchy[0, i, 3]  # Correctly access the parent index
+                            if parent_index == -1:
+                                # Kontura bez rodiče - vnější kontura
+                                cv.drawContours(img_with, [contour], -1, (0, 0, 255), 2)  # Červeně pro vnější kontury
+                                outer_contours.append(contour)
+                            else:
                                 # Kontrola, zda má rodič této kontury také rodiče (kontury druhého řádu)
                                 grandparent_index = hierarchy[0][parent_index][3]
+
                                 if grandparent_index == -1:
-                                    # Kontura je prvního řádu (má rodiče, ale nemá dědečka)
-                                    cv.drawContours(img_with, [contour], -1, [255, 0, 0], 2)
+                                    # Kontura s jedním předkem - vnitřní kontura
+                                    cv.drawContours(img_with, [contour], -1, (255, 0, 0),
+                                                    2)  # Modře pro vnitřní kontury
                                     inner_contours.append(contour)
-                            else:
-                                cv.drawContours(img_with, [contour], -1, [0, 0, 255], 2)
-                                outer_contours.append(contour)
+                                else:
+                                    # Kontura s dvěma předky - potomek vnitřní kontury
+                                    cv.drawContours(img_with, [contour], -1, (0, 0, 255),
+                                                    2)  # Zeleně pro potomky vnitřních kontur
+                                    outer_contours.append(contour)
 
                     if len(outer_contours) == 0:
                         outer_contours = contours
 
                     for index, contour in enumerate(outer_contours):
                         if not self.contours_state == "all":
                             cv.drawContours(img_without, [contour], -1, [0, 0, 255], 2)
@@ -205,17 +225,14 @@
         self.algorithm = algorithm
         self.contours_state = contours_state
         self.detect_corrupted = detect_corrupted
         self.adresa_output = f"{adresa_output}/{project}/IoU"
         self.adresa_plots = f"{adresa_output}/{project}/IoU/plots/{self.algorithm}"
 
         fm.create_directory(self.adresa_output)
-        fm.create_directory(self.adresa_plots, delete=True)
-
-        self.plot_lock = Lock()
 
         # for mask, name in zip(self.masks, self.img_names):
         #    cv.imwrite(f"img_print/{name}",mask)
 
     def process_and_compute_iou(self, ref_mask, img, img_name, parameters, save, lock):
         # Convert the mask tensor and image tensor to numpy arrays
         ref_mask = ref_mask.numpy()
```

### Comparing `prusek_spheroid-3.5/prusek_spheroid/GUI.py` & `prusek_spheroid-3.6/prusek_spheroid/GUI.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,55 +2,234 @@
 from tkinter import filedialog
 from tkinter import messagebox
 from prusek_spheroid import GradientDescentGUI as g
 from prusek_spheroid import ContoursClassGUI as F
 import threading
 import time
 import json
-import zipfile
 import os
 from prusek_spheroid import characteristic_functions as cf
 from prusek_spheroid import file_management as fm
+from prusek_spheroid import conversion as c
 import pandas as pd
 import cv2 as cv
 from tkinter import Toplevel, Label
 from tkinter import ttk
+import sys
 
 
-def show_selection_dialog(root):
-    # Skryje hlavní Tkinter okno
-    root.withdraw()
 
-    dialog = tk.Toplevel(root)
-    dialog.title("Software Selection")
-    dialog.geometry("400x150")  # Nastaví velikost dialogového okna
+class SelectionDialog:
+    def __init__(self, root):
+        self.root = root
+        self.dialog = tk.Toplevel(root)
+        self.dialog.title("Software Selection")
+        self.dialog.geometry("400x150")
 
-    seg_button = tk.Button(dialog, text="Spheroids Segmentation", command=lambda: open_segmentation_gui(dialog, root))
-    seg_button.pack(pady=20)
+        seg_button = tk.Button(self.dialog, text="Spheroids Segmentation", command=self.open_segmentation_gui)
+        seg_button.pack(pady=10)
 
-    quant_button = tk.Button(dialog, text="Spheroids Quantification",
-                             command=lambda: open_quantification_gui(dialog, root))
-    quant_button.pack(pady=20)
+        quant_button = tk.Button(self.dialog, text="Spheroids Quantification", command=self.open_quantification_gui)
+        quant_button.pack(pady=10)
 
-    def on_close():
-        root.quit()  # Ukončí celý program, když je zavřeno toto dialogové okno
+        convert_button = tk.Button(self.dialog, text="Convert between COCO 1.0 and Masks",
+                                   command=self.open_conversion_gui)
+        convert_button.pack(pady=10)
 
-    dialog.protocol("WM_DELETE_WINDOW", on_close)
+        self.dialog.protocol("WM_DELETE_WINDOW", self.on_close)
 
+    def show(self):
+        self.dialog.deiconify()
 
-def open_segmentation_gui(dialog, root):
-    dialog.destroy()
-    root.deiconify()
-    app = SpheroidSegmentationGUI(root)
+    def hide(self):
+        self.dialog.withdraw()
 
+    def open_segmentation_gui(self):
+        self.hide()
+        SpheroidSegmentationGUI(self)
+
+    def open_quantification_gui(self):
+        self.hide()
+        SpheroidQuantificationGUI(self)
+
+    def open_conversion_gui(self):
+        self.hide()
+        ConversionDialog(self)
+
+    def on_close(self):
+        self.root.quit()
+
+
+class ConversionDialog:
+    def __init__(self, selection_dialog):
+        self.output_folder_label_masks = None
+        self.images_folder_label = None
+        self.coco_address_label = None
+        self.output_folder_label_coco = None
+        self.masks_folder_label = None
+        self.selection_dialog = selection_dialog
+        # Define the StringVar attributes here before calling setup_dialog
+        self.coco_annotation_path = tk.StringVar()
+        self.output_folder_path_coco = tk.StringVar()
+        self.masks_folder_path = tk.StringVar()
+        self.images_folder_path = tk.StringVar()
+        self.output_folder_path_masks = tk.StringVar()
+
+        self.dialog = tk.Toplevel(selection_dialog.root)
+        self.dialog.title("Conversion dialog")
+        self.setup_dialog()  # Now all necessary attributes are defined before setup_dialog is called
+
+    def setup_dialog(self):
+        back_button = tk.Button(self.dialog, text="Back", command=self.go_back)
+        back_button.pack(anchor='nw', padx=10, pady=5)
+
+        notebook = ttk.Notebook(self.dialog)
+        coco_to_masks_tab = ttk.Frame(notebook)
+        masks_to_coco_tab = ttk.Frame(notebook)
+        notebook.add(coco_to_masks_tab, text='COCO 1.0 to Masks')
+        notebook.add(masks_to_coco_tab, text='Masks to COCO 1.0')
+        notebook.pack(expand=True, fill='both')
+
+        # COCO to Masks tab components
+        coco_annotation_button = tk.Button(coco_to_masks_tab, text="Load COCO 1.0 Annotations ZIP",
+                                           command=lambda: browse_file(self.coco_annotation_path,
+                                                                       "COCO Annotations ZIP", self.coco_address_label))
+        self.coco_address_label = tk.Label(coco_to_masks_tab, textvariable=self.coco_annotation_path)
+        coco_annotation_button.pack(pady=10)
+        self.coco_address_label.pack()
+
+        output_folder_button_coco = tk.Button(coco_to_masks_tab, text="Select Output Folder",
+                                              command=lambda: browse_directory(self.output_folder_path_coco,
+                                                                               "Output Folder for COCO to Masks",
+                                                                               self.output_folder_label_coco))
+        self.output_folder_label_coco = tk.Label(coco_to_masks_tab, textvariable=self.output_folder_path_coco)
+        output_folder_button_coco.pack(pady=10)
+        self.output_folder_label_coco.pack()
+
+        # Masks to COCO tab components
+        masks_folder_button = tk.Button(masks_to_coco_tab, text="Load Masks Folder",
+                                        command=lambda: browse_directory(self.masks_folder_path, "Masks Folder",
+                                                                         self.masks_folder_label))
+        self.masks_folder_label = tk.Label(masks_to_coco_tab, textvariable=self.masks_folder_path)
+        masks_folder_button.pack(pady=10)
+        self.masks_folder_label.pack()
+
+
+        images_folder_button = tk.Button(masks_to_coco_tab, text="Load Images Folder",
+                                         command=lambda: browse_directory(self.images_folder_path, "Images Folder",
+                                                                          self.images_folder_label))
+        self.images_folder_label = tk.Label(masks_to_coco_tab, textvariable=self.images_folder_path)
+        images_folder_button.pack(pady=10)
+        self.images_folder_label.pack()
+
+        output_folder_button_masks = tk.Button(masks_to_coco_tab, text="Select Output Folder",
+                                               command=lambda: browse_directory(self.output_folder_path_masks,
+                                                                                "Output Folder for Masks to COCO",
+                                                                                self.output_folder_label_masks))
+        self.output_folder_label_masks = tk.Label(masks_to_coco_tab, textvariable=self.output_folder_path_masks)
+        output_folder_button_masks.pack(pady=10)
+        self.output_folder_label_masks.pack()
+
+        # Inside the setup_dialog method of ConversionDialog class
+
+        run_button = tk.Button(self.dialog, text="Run Conversion",
+                               command=lambda: self.run_conversion(notebook.index(notebook.select())))
+        run_button.pack(pady=20)
+
+        self.dialog.protocol("WM_DELETE_WINDOW", self.on_close)
+
+    def show_done_dialog(self, message):
+        # Create a top-level window
+        done_dialog = tk.Toplevel()
+        done_dialog.title("Conversion Completed")
+
+        # Set the window size and make it non-resizable
+        done_dialog.geometry("300x100")
+        done_dialog.resizable(False, False)
+
+        # Message Label
+        tk.Label(done_dialog, text=message, pady=10).pack()
+
+        # OK Button
+        ok_button = tk.Button(done_dialog, text="OK", command=done_dialog.destroy, width=10)
+        ok_button.pack(pady=10)
+
+    def show_wait_dialog(self):
+        self.wait_dialog = tk.Toplevel()  # Create a new top-level window
+        self.wait_dialog.title("Processing")
+
+        # Set the window size and make it non-resizable
+        self.wait_dialog.geometry("200x100")
+        self.wait_dialog.resizable(False, False)
+
+        # Message Label
+        tk.Label(self.wait_dialog, text="Wait...", pady=20).pack()
+
+
+        self.wait_dialog.grab_set()  # Make it modal
+        self.wait_dialog.lift()  # Bring it to front
+        self.wait_dialog.focus_set()  # Set focus to this window
+
+        # This window should not be closed manually; it will be closed programmatically
+        self.wait_dialog.protocol("WM_DELETE_WINDOW", lambda: None)  # Disable the close button
+
+    def go_back(self):
+        self.dialog.destroy()
+        self.selection_dialog.show()
+
+    def run_conversion(self, active_tab_index):
+        self.show_wait_dialog()
+        if active_tab_index == 0:  # COCO 1.0 to Masks
+            coco_zip_path = self.coco_annotation_path.get()
+            output_folder_path = self.output_folder_path_coco.get()
+
+            if not coco_zip_path or not output_folder_path:
+                messagebox.showerror("Error", "Both COCO ZIP file and output folder addresses must be filled.")
+                return
+
+            try:
+                annotation_address = fm.unzip(
+                    coco_zip_path)
+                annotations_address, images_address = update_addresses(annotation_address)
+                c.load_annotations_and_save(annotations_address, images_address,
+                                            os.path.join(output_folder_path, "masks"),
+                                            os.path.join(output_folder_path, "images"))
+                self.wait_dialog.destroy()  # Close the wait dialog on success
+                self.show_done_dialog("Conversion to masks completed successfully.")
+            except Exception as e:
+                self.wait_dialog.destroy()
+                messagebox.showerror("Error", f"Failed to process COCO annotations. Error: {str(e)}")
+
+        elif active_tab_index == 1:  # Masks to COCO 1.0
+            masks_folder_path = self.masks_folder_path.get()
+            images_folder_path = self.images_folder_path.get()
+            output_folder_path = self.output_folder_path_masks.get()
+
+            if not masks_folder_path or not images_folder_path or not output_folder_path:
+                messagebox.showerror("Error",
+                                     "Masks folder, images folder, and output folder addresses must be filled.")
+                return
+
+            try:
+                c.process_masks_to_coco(masks_folder_path, images_folder_path, output_folder_path)
+                self.wait_dialog.destroy()
+                self.show_done_dialog("Conversion to COCO completed successfully.")
+            except Exception as e:
+                self.wait_dialog.destroy()
+                messagebox.showerror("Error", f"Failed to process masks. Error: {str(e)}")
+
+    def on_close(self):
+        self.dialog.quit()
+
+    @staticmethod
+    def shorten_path(path, max_length=40):
+        if len(path) > max_length:
+            return '...' + path[-max_length + 3:]
+        return path
 
-def open_quantification_gui(dialog, root):
-    dialog.destroy()
-    root.deiconify()
-    app = SpheroidQuantificationGUI(root)
 
 def update_addresses(annotationsAddress):
     annotation_address = os.path.join(annotationsAddress, "annotations")
     images_address = os.path.join(annotationsAddress, "images")
 
     return annotation_address, images_address
 
@@ -186,68 +365,76 @@
     directory_path = filedialog.askdirectory()
     var.set(directory_path)
     shortened_path = shorten_path(directory_path)
     label.config(text=f"{title}: {shortened_path}")
 
 
 class SpheroidQuantificationGUI:
-    def __init__(self, master):
-        self.master = master
-        self.master.title("Spheroid Quantification")
+    def __init__(self, selection_dialog):
+        self.selection_dialog = selection_dialog
+        self.dialog = tk.Toplevel(selection_dialog.root)
+        self.dialog.title("Spheroid Quantification")
+
+        back_button = tk.Button(self.dialog, text="Back", command=self.go_back)
+        back_button.pack(anchor='nw', padx=10, pady=5)
 
         # Sekce pro kvantifikaci sféroidů
         # Implementace funkcí a GUI prvků pro kvantifikaci sféroidů
 
         # Button to retrieve the folder address of masks of annotated spheroids
-        self.retrieve_masks_button_quantification = tk.Button(master,
+        self.retrieve_masks_button_quantification = tk.Button(self.dialog,
                                                               text="Retrieve the folder address of masks of annotated spheroids",
                                                               command=lambda: browse_directory(
                                                                   self.masks_annotation_path_quantification,
                                                                   "Selected masks folder",
                                                                   self.masks_address_label_quantification))
         self.retrieve_masks_button_quantification.pack()
 
         self.masks_annotation_path_quantification = tk.StringVar()
-        self.masks_address_label_quantification = tk.Label(master, text="")
+        self.masks_address_label_quantification = tk.Label(self.dialog, text="")
         self.masks_address_label_quantification.pack()
 
         # Button to retrieve the output folder address
-        self.retrieve_output_button_quantification = tk.Button(master,
+        self.retrieve_output_button_quantification = tk.Button(self.dialog,
                                                                text="Retrieve the output folder address",
                                                                command=lambda: browse_directory(
                                                                    self.output_path_quantification,
                                                                    "Selected output folder",
                                                                    self.output_address_label_quantification))
         self.retrieve_output_button_quantification.pack()
 
         self.output_path_quantification = tk.StringVar()
-        self.output_address_label_quantification = tk.Label(master, text="")
+        self.output_address_label_quantification = tk.Label(self.dialog, text="")
         self.output_address_label_quantification.pack()
 
         # Button to calculate spheroid properties
-        self.calculate_properties_button = tk.Button(master, text="Calculate spheroid properties",
+        self.calculate_properties_button = tk.Button(self.dialog, text="Calculate spheroid properties",
                                                      command=self.calculate_spheroid_properties)
         self.calculate_properties_button.pack()
 
-        self.master.protocol("WM_DELETE_WINDOW", self.on_close)
+        self.dialog.protocol("WM_DELETE_WINDOW", self.on_close)
+
+    def go_back(self):
+        self.dialog.destroy()
+        self.selection_dialog.show()
 
     def on_close(self):
-        self.master.quit()  # Toto ukončí celý program
+        self.dialog.quit()  # Toto ukončí celý program
 
     def calculate_spheroid_properties(self):
         if not self.masks_annotation_path_quantification.get() or not self.output_path_quantification.get():
             messagebox.showerror("Error", "Both mask folder and output folder addresses must be filled.")
             return
 
         masks_data = fm.load_masks(self.masks_annotation_path_quantification.get())
         total_masks = len(masks_data)
 
         # Dialog for progress
         # Dialog for progress
-        progress_dialog = Toplevel(self.master)
+        progress_dialog = Toplevel(self.dialog)
         progress_dialog.title("Processing Progress")
         progress_dialog.geometry("400x100")  # Nastaví rozměry okna na 400x100 pixelů
         Label(progress_dialog, text=f"Total images: {total_masks}").pack()
         progress_label = Label(progress_dialog, text="Starting...")
         progress_label.pack()
 
         all_contour_data = []
@@ -285,26 +472,29 @@
 
         # Show completion message
         messagebox.showinfo("Completed", f"Spheroid properties calculated and saved.\nOutput path: {output_path}")
         print("Spheroid properties calculated and saved.")
 
 
 class SpheroidSegmentationGUI:
-    def __init__(self, master):
+    def __init__(self, selection_dialog):
+        self.selection_dialog = selection_dialog
+        self.dialog = tk.Toplevel(selection_dialog.root)
+        self.dialog.title("Spheroid Quantification")
+
+        back_button = tk.Button(self.dialog, text="Back", command=self.go_back)
+        back_button.pack(anchor='nw', padx=10, pady=5)
         self.loaded_parameters = None
         self.loaded_method = None
 
-        self.master = master
-        self.master.title("Spheroid segmentation")
-
         # Adresní sekce
-        self.address_section_label = tk.Label(master, text="Address Settings", font=("Helvetica", 12, "bold"))
+        self.address_section_label = tk.Label(self.dialog, text="Address Settings", font=("Helvetica", 12, "bold"))
         self.address_section_label.pack()
 
-        self.notebook = ttk.Notebook(master)
+        self.notebook = ttk.Notebook(self.dialog)
         self.coco_tab = ttk.Frame(self.notebook)  # První záložka pro COCO
         self.mask_tab = ttk.Frame(self.notebook)  # Druhá záložka pro masky
 
         self.notebook.add(self.coco_tab, text='Load COCO Annotations')
         self.notebook.add(self.mask_tab, text='Load MASK Annotations')
         self.notebook.pack(expand=True, fill='both')
 
@@ -342,89 +532,89 @@
         self.images_address_label = tk.Label(self.mask_tab, text="")
         self.images_address_label.pack()
 
         self.masks_annotation_path = tk.StringVar()
         self.image_dataset_path = tk.StringVar()
 
         # File Dialog pro výsledné segmentované obrázky (změna na askdirectory)
-        self.dataset_address_button = tk.Button(master,
+        self.dataset_address_button = tk.Button(self.dialog,
                                                 text="Dataset of all images address (folder of images you want to segment)",
                                                 command=lambda: browse_directory(self.dataset_path,
                                                                                  "Selected dataset path",
                                                                                  self.dataset_address_label))
         self.dataset_address_button.pack(side=tk.TOP)
 
         self.dataset_path = tk.StringVar()
 
         # Indikátor pro vyplnění adresy
-        self.dataset_address_label = tk.Label(master, text="")
+        self.dataset_address_label = tk.Label(self.dialog, text="")
         self.dataset_address_label.pack()
 
         # File Dialog pro výsledné segmentované obrázky (změna na askdirectory)
-        self.output_address_button = tk.Button(master,
+        self.output_address_button = tk.Button(self.dialog,
                                                text="Output address (folder where to save the output)",
                                                command=lambda: browse_directory(self.output_path,
                                                                                 "Selected output path",
                                                                                 self.output_address_label))
         self.output_address_button.pack(side=tk.TOP)
 
         self.output_path = tk.StringVar()
 
         # Indikátor pro vyplnění adresy
-        self.output_address_label = tk.Label(master, text="")
+        self.output_address_label = tk.Label(self.dialog, text="")
         self.output_address_label.pack()
 
         # Oddělovací čára mezi adresní a metody sekce
-        self.address_separator = tk.Frame(master, height=2, bd=1, relief=tk.SUNKEN)
+        self.address_separator = tk.Frame(self.dialog, height=2, bd=1, relief=tk.SUNKEN)
         self.address_separator.pack(fill=tk.X, padx=5, pady=5)
 
         # Metodická sekce
-        self.method_section_label = tk.Label(master, text="Method Settings", font=("Helvetica", 12, "bold"))
+        self.method_section_label = tk.Label(self.dialog, text="Method Settings", font=("Helvetica", 12, "bold"))
         self.method_section_label.pack()
 
         # Textbox pro název projektu
-        self.project_name_label = tk.Label(master, text="Project Name:")
+        self.project_name_label = tk.Label(self.dialog, text="Project Name:")
         self.project_name_label.pack()
-        self.project_name_entry = tk.Entry(master)
+        self.project_name_entry = tk.Entry(self.dialog)
         self.project_name_entry.pack()
 
         # Tlačítko pro načtení parametrů z JSON souboru
-        self.load_parameters_button = tk.Button(master,
+        self.load_parameters_button = tk.Button(self.dialog,
                                                 text="I already know the parameters (load JSON file with parameters)",
                                                 command=self.load_and_run_parameters)
         self.load_parameters_button.pack()
 
         # Create a frame to contain the label and button
-        self.parameters_frame = tk.Frame(self.master)
+        self.parameters_frame = tk.Frame(self.dialog)
         self.parameters_frame.pack()
 
         # Initially disable the "Parameters loaded" label and the "Cancel" button
         self.parameters_loaded_label = tk.Label(self.parameters_frame, text="Parameters loaded", state=tk.DISABLED)
         self.parameters_loaded_label.pack(side=tk.LEFT)
 
         self.cancel_button = tk.Button(self.parameters_frame, text="Cancel", command=self.cancel_parameters_loaded,
                                        state=tk.DISABLED)
         self.cancel_button.pack(side=tk.LEFT)
 
         # Checkboxy pro výběr metod
-        self.methods_frame = tk.Frame(master)
+        self.methods_frame = tk.Frame(self.dialog)
         self.methods_frame.pack()
         self.method_labels = ["Sauvola", "Niblack", "Gaussian"]
 
         self.methods_checkboxes = []
 
         for i, method_label in enumerate(self.method_labels):
             method_var = tk.IntVar()
             method_checkbox = tk.Checkbutton(self.methods_frame, text=method_label, variable=method_var)
             method_checkbox.grid(row=0, column=i, padx=5, pady=5)
 
             self.methods_checkboxes.append((method_checkbox, method_var))
 
         # Textová pole pro zadání parametrů
-        self.parameters_frame = tk.Frame(master)
+        self.parameters_frame = tk.Frame(self.dialog)
         self.parameters_frame.pack()
         self.learning_rate_label = tk.Label(self.parameters_frame, text="Learning Rate:")
         self.learning_rate_label.grid(row=0, column=0, padx=5, pady=5)
         self.learning_rate_entry = tk.Entry(self.parameters_frame)
         self.learning_rate_entry.grid(row=0, column=1, padx=5, pady=5)
 
         self.iterations_label = tk.Label(self.parameters_frame, text="Number of Iterations:")
@@ -439,23 +629,24 @@
 
         # Přednastavení hodnot parametrů
         self.learning_rate_entry.insert(0, "0.01")
         self.iterations_entry.insert(0, "50")
         self.batch_size_entry.insert(0, "10")
 
         # Oddělovací čára mezi adresní a metody sekce
-        self.method_separator = tk.Frame(master, height=2, bd=1, relief=tk.SUNKEN)
+        self.method_separator = tk.Frame(self.dialog, height=2, bd=1, relief=tk.SUNKEN)
         self.method_separator.pack(fill=tk.X, padx=5, pady=5)
 
         # Hole Finding Settings Section
-        self.hole_finding_section_label = tk.Label(master, text="Hole Finding Settings", font=("Helvetica", 12, "bold"))
+        self.hole_finding_section_label = tk.Label(self.dialog, text="Hole Finding Settings",
+                                                   font=("Helvetica", 12, "bold"))
         self.hole_finding_section_label.pack()
 
         # Frame for the checkboxes
-        self.hole_finding_frame = tk.Frame(master)
+        self.hole_finding_frame = tk.Frame(self.dialog)
         self.hole_finding_frame.pack()
 
         # Variables for the checkboxes
         self.detect_outer_var = tk.IntVar(value=0)
         self.detect_all_var = tk.IntVar(value=0)
         self.view_select_var = tk.IntVar(value=0)
 
@@ -484,21 +675,21 @@
                                                    command=lambda: update_hole_finding_checkboxes(self.view_select_var))
 
         self.detect_outer_checkbox.pack(anchor='w')  # Aligns to the west (left) of the frame
         self.detect_all_checkbox.pack(anchor='w')  # Consistent with the first checkbox
         self.view_select_checkbox.pack(anchor='w')
 
         # Oddělovací čára mezi adresní a metody sekce
-        self.settings_separator = tk.Frame(master, height=2, bd=1, relief=tk.SUNKEN)
+        self.settings_separator = tk.Frame(self.dialog, height=2, bd=1, relief=tk.SUNKEN)
         self.settings_separator.pack(fill=tk.X, padx=5, pady=5)
 
-        self.other_section_label = tk.Label(master, text="Other Settings", font=("Helvetica", 12, "bold"))
+        self.other_section_label = tk.Label(self.dialog, text="Other Settings", font=("Helvetica", 12, "bold"))
         self.other_section_label.pack()
 
-        checkbox_frame = tk.Frame(master)
+        checkbox_frame = tk.Frame(self.dialog)
         checkbox_frame.pack()
 
         self.detect_corrupted_var = tk.BooleanVar()
         self.checkbox_detect_corrupted = tk.Checkbutton(checkbox_frame, text="Detect and discard corrupted images",
                                                         variable=self.detect_corrupted_var, onvalue=True,
                                                         offvalue=False)
         self.checkbox_detect_corrupted.pack(side=tk.LEFT)
@@ -514,32 +705,39 @@
         self.calculate_contours_var = tk.BooleanVar()
         self.checkbox_calculate_contours = tk.Checkbutton(checkbox_frame, text="Calculate spheroid properties",
                                                           variable=self.calculate_contours_var,
                                                           onvalue=True, offvalue=False)
         self.checkbox_calculate_contours.pack(side=tk.LEFT)
 
         # Tlačítko pro spuštění
-        self.run_button = tk.Button(master, text="Run", command=self.run_method)
+        self.run_button = tk.Button(self.dialog, text="Run", command=self.run_method)
         self.run_button.pack()
 
-        self.master.protocol("WM_DELETE_WINDOW", self.on_close)
+        self.dialog.protocol("WM_DELETE_WINDOW", self.on_close)
+        self.stop_event = threading.Event()
+
+    def go_back(self):
+        self.dialog.destroy()
+        self.selection_dialog.show()
 
     def on_close(self):
-        self.master.quit()
+        # Signal all threads to stop by setting the event
+        self.stop_event.set()
+        sys.exit()
 
     def get_contours_state(self):
         if self.detect_outer_var.get() == 1:
             return "no"
         elif self.detect_all_var.get() == 1:
             return "all"
         else:
             return "select"
 
     def show_completion_dialog(self, time_taken, output_folder):
-        dialog = tk.Toplevel(self.master)
+        dialog = tk.Toplevel(self.dialog)
         dialog.title("Segmentation Completed")
 
         message = f"DONE.\nSegmentation took {time_taken:.2f} seconds.\nOutput stored in a folder: {output_folder}"
         tk.Label(dialog, text=message).pack(padx=20, pady=10)
 
         ok_button = tk.Button(dialog, text="OK", command=lambda: [dialog.destroy(), self.reset_gui()])
         ok_button.pack(pady=10)
@@ -620,16 +818,16 @@
 
     def run_method_with_loaded_parameters(self):
         if not self.loaded_parameters:
             messagebox.showerror("Error", "No parameters loaded.")
             return
 
         # Předpokládá se, že tato metoda otevře dialog pro potvrzení parametrů
-        parameter_entry_dialog = ParameterEntryDialog(self.master, self.loaded_method, self.loaded_parameters)
-        self.master.wait_window(parameter_entry_dialog)
+        parameter_entry_dialog = ParameterEntryDialog(self.dialog, self.loaded_method, self.loaded_parameters)
+        self.dialog.wait_window(parameter_entry_dialog)
 
         if parameter_entry_dialog.result is None:
             messagebox.showinfo("Info", "Parameters were not saved.")
         else:
             self.parameters_loaded_label.config(state=tk.NORMAL)
             self.cancel_button.config(state=tk.NORMAL)
 
@@ -707,24 +905,24 @@
 
         # Načtené parametry z JSON souboru, pokud jsou k dispozici
         if self.loaded_parameters:
             parameters = self.loaded_parameters
             progress_window1 = None
         else:
             parameters = None
-            progress_window1 = OptimizationProgressWindow(self.master)
+            progress_window1 = OptimizationProgressWindow(self.dialog)
             progress_window1.update_info(project_name, algorithms, 0, "Unknown", "Unknown", "Unknown")
             progress_window1.withdraw()
 
         contours_state = self.get_contours_state()
         detect_corrupted = self.detect_corrupted_var.get()
         create_json = self.create_json_var.get()
         calculate_properties = self.calculate_contours_var.get()
 
-        progress_window2 = ProcessingProgressWindow(self.master)
+        progress_window2 = ProcessingProgressWindow(self.dialog)
         progress_window2.update_progress("Initializing...")
         progress_window2.withdraw()
 
         run_thread = threading.Thread(target=self.run_main, args=(
             annotation_data, dataset_address, output_address, project_name, algorithms, parameters,
             contours_state, detect_corrupted, create_json, calculate_properties, progress_window1,
             progress_window2))
@@ -751,23 +949,24 @@
                                                     detect_corrupted=detect_corrupted).run()
                 print(f"Resulting parameters: {parameters}", f"IoU: {round(iou * 100, 2)}%")
                 progress_window1.withdraw()
             else:
                 parameters = known_parameters
 
             progress_window2.deiconify()
-            F.Contours(self.master, dataset_address, output_address, project_name, algorithm, parameters,
+            F.Contours(self.dialog, dataset_address, output_address, project_name, algorithm, parameters,
                        False, F.IoU, contours_state, detect_corrupted, create_json, calculate_properties,
                        progress_window2).run()
             print(f"Segmentation of the project took: {round(time.time() - startTime)} seconds")
             progress_window2.withdraw()
 
         print(f"Total time: {round(time.time() - totalTime)} seconds")
 
         # Zobrazit dialogové okno po dokončení segmentace
         self.show_completion_dialog(round(time.time() - totalTime), output_address)
 
 
 if __name__ == "__main__":
     root = tk.Tk()
-    show_selection_dialog(root)
+    root.withdraw()  # Optionally hide the root window
+    app = SelectionDialog(root)
     root.mainloop()
```

### Comparing `prusek_spheroid-3.5/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-3.6/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.5/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-3.6/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.5/prusek_spheroid/file_management.py` & `prusek_spheroid-3.6/prusek_spheroid/file_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import zipfile
 import os
 
 
 def unzip(zip_file_path):
     # Odstranění přípony '.zip' a vytvoření cesty pro cílovou složku
     base_path = os.path.splitext(zip_file_path)[0]
-
     # Kontrola, zda cílová složka již existuje. Pokud ne, vytvoří ji.
     if not os.path.exists(base_path):
         os.makedirs(base_path)
 
     # Extrahování souborů do cílové složky
     with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
         zip_ref.extractall(base_path)
```

### Comparing `prusek_spheroid-3.5/prusek_spheroid/image_processing.py` & `prusek_spheroid-3.6/prusek_spheroid/methods.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,82 @@
-import numpy as np
+import sys
+from prusek_spheroid import image_processing as ip
+from skimage.filters import threshold_sauvola, threshold_niblack
 import cv2 as cv
-from skimage import img_as_ubyte
-from skimage import feature
 
-def find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours):
-    result_mask = np.zeros_like(img_binary, dtype=np.uint8)
-
-    for contour in filtered_contours:
-        filled_contour = cv.fillPoly(np.zeros_like(img_binary), [contour], 1)
-
-        intersection = filled_contour & edges
-
-        if np.any(intersection):
-            result_mask = result_mask | filled_contour
-
-    if inner_contours:
-        inner_contours_mask = np.zeros_like(img_binary, dtype=np.uint8)
-        for i in range(len(contours)):
-            if hierarchy[0, i, 3] != -1:
-                inner_filled_contour = cv.fillPoly(np.zeros_like(img_binary), [contours[i]], 1)
-
-                inner_contours_mask = cv.bitwise_or(inner_filled_contour, inner_contours_mask)
-
-        # inner_contours_mask = f.Erosion(inner_contours_mask, 3, 1)
-
-        return np.clip(result_mask, 0, 1), np.clip(inner_contours_mask, 0, 1)
-
-    return np.clip(result_mask, 0, 1), None
 
+class BaseImageProcessing:
+    def apply_segmentation_algorithm(self, algorithm, parameters, img, inner_contours,
+                                     detect_corrupted):
+        if algorithm == "Sauvola":
+            return self.sauvola(parameters, img, inner_contours, detect_corrupted)
+        elif algorithm == "Niblack":
+            return self.niblack(parameters, img, inner_contours, detect_corrupted)
+        elif algorithm == "Gaussian":
+            return self.gaussian_adaptive(parameters, img, inner_contours, detect_corrupted)
+        else:
+            print(f"Algorithm with name {algorithm} not found.")
+            sys.exit(1)
 
-def create_binary_mask(img_gray, threshold, dilation_size, erosion_size=None):
-    img_binary = img_as_ubyte(img_gray > threshold)
-    img_binary = np.invert(img_binary)
-    if erosion_size is not None:
-        img_binary = Erosion(img_binary, erosion_size, 1)
-    img_binary = Dilation(img_binary, dilation_size, 1)
-    return img_binary
+    @staticmethod
+    def sauvola(parameters, img_gray, inner_contours, detect_corrupted):
+        window_size = ip.check_window_size(int(parameters["window_size"]))
+        std_k = parameters["std_k"]
+        min_area = parameters["min_area"]
+        dilation_size = int(parameters["dilation_size"])
+        sigma = parameters["sigma"]
 
+        thresh_sauvola = threshold_sauvola(img_gray, window_size=window_size)
+        img_binary = ip.create_binary_mask(img_gray, thresh_sauvola, dilation_size)
+        #edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
+        edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
 
-def calculate_canny_edges(img_gray, std_k, sigma):
-    mean = np.mean(img_gray)
-    std = np.std(img_gray)
-    low_threshold = mean - std_k * std / 2
-    high_threshold = mean + std_k * std / 2
-    edges = feature.canny(img_gray, sigma=sigma, low_threshold=low_threshold, high_threshold=high_threshold)
-    return edges
+        contours, hierarchy = ip.findContours(img_binary, inner_contours)
+        filtered_contours = ip.filter_contours(contours, min_area)
 
+        return ip.find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours)
 
-def filter_contours(contours, img_shape, min_area, detect_corrupted=True):
-    height, width = img_shape
-    filtered_contours = []
+    @staticmethod
+    def niblack(parameters, img_gray, inner_contours, detect_corrupted):
+        window_size = ip.check_window_size(int(parameters["window_size"]))
+        k = parameters["k"]
+        min_area = parameters["min_area"]
+        std_k = parameters["std_k"]
+        dilation_size = int(parameters["dilation_size"])
+        sigma = parameters["sigma"]
 
-    for contour in contours:
-        if detect_corrupted:
-            if not (np.any(contour[:, :, 0] == 0) or np.any(contour[:, :, 1] == 0) or
-                    np.any(contour[:, :, 0] == width - 1) or np.any(contour[:, :, 1] == height - 1)):
-                if cv.contourArea(contour) >= min_area:
-                    filtered_contours.append(contour)
-        else:
-            if cv.contourArea(contour) >= min_area:
-                filtered_contours.append(contour)
+        thresh_niblack = threshold_niblack(img_gray, window_size=window_size, k=k)
+        img_binary = ip.create_binary_mask(img_gray, thresh_niblack, dilation_size, 1)
 
-    return filtered_contours
+        #edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
+        edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
 
+        contours, hierarchy = ip.findContours(img_binary, inner_contours)
+        filtered_contours = ip.filter_contours(contours, min_area)
 
-def check_window_size(window_size):
-    return window_size + 1 if window_size % 2 == 0 else window_size
+        return ip.find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours)
 
+    @staticmethod
+    def gaussian_adaptive(parameters, img_gray, inner_contours, detect_corrupted):
+        window_size = ip.check_window_size(int(parameters["window_size"]))
+        min_area = parameters["min_area"]
+        std_k = parameters["std_k"]
+        dilation_size = int(parameters["dilation_size"])
+        sigma = parameters["sigma"]
 
-def findContours(img_binary, inner_contours):
-    if inner_contours:
-        contours, hierarchy = cv.findContours(img_binary, cv.RETR_CCOMP, cv.CHAIN_APPROX_SIMPLE)
-    else:
-        contours, hierarchy = cv.findContours(img_binary, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
+        img_binary = cv.adaptiveThreshold(img_gray, 255, cv.ADAPTIVE_THRESH_GAUSSIAN_C, cv.THRESH_BINARY_INV,
+                                          window_size, 0)
 
-    return contours, hierarchy
+        img_binary = ip.Erosion(img_binary, 1, 1)
 
+        img_binary = ip.Dilation(img_binary, dilation_size, 1)
 
-def Dilation(img, dilation_size=3, iterations=1, dilation_shape=cv.MORPH_ELLIPSE):
-    element = cv.getStructuringElement(dilation_shape, (2 * dilation_size + 1, 2 * dilation_size + 1),
-                                       (dilation_size, dilation_size))
-    img_final = cv.dilate(img, element, iterations=iterations)
+        #edges = ip.calculate_canny_edges(img_gray, std_k, sigma)
+        edges = ip.laplacian_of_gaussian(img_gray, std_k, sigma)
 
-    return img_final
+        contours, hierarchy = ip.findContours(img_binary, inner_contours)
 
+        filtered_contours = ip.filter_contours(contours, min_area)
 
-def Erosion(img, erosion_size=3, iterations=1, erosion_shape=cv.MORPH_ELLIPSE):
-    element = cv.getStructuringElement(erosion_shape, (2 * erosion_size + 1, 2 * erosion_size + 1),
-                                       (erosion_size, erosion_size))
-    img_final = cv.erode(img, element, iterations=iterations)
+        result = ip.find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours)
 
-    return img_final
+        return result
```

### Comparing `prusek_spheroid-3.5/prusek_spheroid/metrics.py` & `prusek_spheroid-3.6/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.5/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-3.6/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.5/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-3.6/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.5
+Version: 3.6
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.5/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-3.6/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 prusek_spheroid/ContoursClassGUI.py
 prusek_spheroid/GUI.py
 prusek_spheroid/GradientDescentGUI.py
 prusek_spheroid/characteristic_functions.py
+prusek_spheroid/conversion.py
 prusek_spheroid/file_management.py
 prusek_spheroid/image_processing.py
 prusek_spheroid/methods.py
 prusek_spheroid/metrics.py
 prusek_spheroid/selection_dialog.py
 prusek_spheroid.egg-info/PKG-INFO
 prusek_spheroid.egg-info/SOURCES.txt
```

### Comparing `prusek_spheroid-3.5/setup.py` & `prusek_spheroid-3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="3.5",
+    version="3.6",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

