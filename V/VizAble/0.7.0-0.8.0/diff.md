# Comparing `tmp/vizable-0.7.0.tar.gz` & `tmp/vizable-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vizable-0.7.0.tar", max compression
+gzip compressed data, was "vizable-0.8.0.tar", max compression
```

## Comparing `vizable-0.7.0.tar` & `vizable-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-03-31 05:43:25.280788 vizable-0.7.0/LICENSE
--rw-r--r--   0        0        0     3548 2024-03-31 05:43:25.280788 vizable-0.7.0/README.md
--rw-r--r--   0        0        0       72 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/__init__.py
--rw-r--r--   0        0        0    26491 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/app.py
--rw-r--r--   0        0        0     2026 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/check_datatypes.py
--rw-r--r--   0        0        0     7887 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/functions.py
--rw-r--r--   0        0        0     4315 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/generate_plots.py
--rw-r--r--   0        0        0      615 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/introductions.py
--rw-r--r--   0        0        0      433 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/rsconnect-python/VizAble.json
--rw-r--r--   0        0        0     2493 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/select_columns.py
--rw-r--r--   0        0        0     1011 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/select_plottypes.py
--rw-r--r--   0        0        0     2804 2024-03-31 05:43:25.280788 vizable-0.7.0/VizAble/upload_file.py
--rw-r--r--   0        0        0     1819 2024-03-31 05:43:25.288787 vizable-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5300 1970-01-01 00:00:00.000000 vizable-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-04 05:20:24.424450 vizable-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3548 2024-04-04 05:20:24.424450 vizable-0.8.0/README.md
+-rw-r--r--   0        0        0       72 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/__init__.py
+-rw-r--r--   0        0        0    28072 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/app.py
+-rw-r--r--   0        0        0     2026 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/check_datatypes.py
+-rw-r--r--   0        0        0     7907 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/functions.py
+-rw-r--r--   0        0        0     6092 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/generate_plots.py
+-rw-r--r--   0        0        0      615 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/introductions.py
+-rw-r--r--   0        0        0      433 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/rsconnect-python/VizAble.json
+-rw-r--r--   0        0        0     2493 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/select_columns.py
+-rw-r--r--   0        0        0     1011 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/select_plottypes.py
+-rw-r--r--   0        0        0     2804 2024-04-04 05:20:24.424450 vizable-0.8.0/VizAble/upload_file.py
+-rw-r--r--   0        0        0     1819 2024-04-04 05:20:24.432450 vizable-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5300 1970-01-01 00:00:00.000000 vizable-0.8.0/PKG-INFO
```

### Comparing `vizable-0.7.0/LICENSE` & `vizable-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vizable-0.7.0/README.md` & `vizable-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `vizable-0.7.0/VizAble/app.py` & `vizable-0.8.0/VizAble/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -474,19 +474,23 @@
         data_frame = reactive_df.get()
         choices: list[str] = functions.return_choices_for_columns(data_frame, input.plot_types())
 
         # update both x-axis and y-axis dropdowns
         if input.plot_types() in ["Line Plot", "Scatter Plot"]:
             functions.update_xaxis_input_select(input.plot_types(), choices)
             functions.update_yaxis_input_select(input.plot_types(), choices)
-
+        
         # update only x-axis dropdowns
-        elif input.plot_types() in ["Bar Plot", "Box Plot", "Histogram"]:
+        elif input.plot_types() in ["Bar Plot", "Histogram"]:
             functions.update_xaxis_input_select(input.plot_types(), choices)
-
+        
+        # update only y-axis dropdowns
+        elif input.plot_types() == "Box Plot":
+            functions.update_yaxis_input_select(input.plot_types(), choices)
+            
     @render.data_frame
     def get_output_selected_cols() -> pd.DataFrame:
         """ Display the selected columns after users' column selections.
 
         :return: A data frame containing the selected columns.
         :rtype: pd.DataFrame
         """
@@ -506,18 +510,18 @@
         elif input.plot_types() == "Bar Plot":
             req(input.bar_x_axis())
             x_col: str = input.bar_x_axis()
             if x_col in data_frame.columns:
                 selected_cols = data_frame[[x_col]]
 
         elif input.plot_types() == "Box Plot":
-            req(input.box_x_axis())
-            x_col: str = input.box_x_axis()
-            if x_col in data_frame.columns:
-                selected_cols = data_frame[[x_col]]
+            req(input.box_y_axis())
+            y_col: str = input.box_y_axis()
+            if y_col in data_frame.columns:
+                selected_cols = data_frame[[y_col]]
 
         elif input.plot_types() == "Histogram":
             req(input.histogram_x_axis())
             x_col: str = input.histogram_x_axis()
             if x_col in data_frame.columns:
                 selected_cols = data_frame[[x_col]]
 
@@ -559,17 +563,17 @@
                 y = input.line_y_axis(),
                 markers = markers,
                 # color = color_by,
             ).update_layout(
                 template="seaborn",
                 title={"text": plot_title, "x": 0.5},
             ).update_xaxes(
-                title_text=x_axis_title,
+                title_text = x_axis_title,
             ).update_yaxes(
-                title_text=y_axis_title,
+                title_text = y_axis_title,
             )
 
             return line_plot
         
         # Bar Plot:
         if input.plot_types() == "Bar Plot":
             req(input.bar_x_axis())
@@ -595,14 +599,57 @@
             ).update_xaxes(
                 title_text = x_axis_title,
             ).update_yaxes(
                 title_text = y_axis_title,
             )
 
             return bar_plot
+        
+        # Box Plot:
+        if input.plot_types() == "Box Plot":
+            req(input.box_y_axis())
+            # y_axis = input.box_y_axis()
+            plot_title = input.box_plot_title()
+            y_axis_title = input.box_y_axis_title()
+
+            box_plot = px.box(
+                data_frame = data_frame,
+                y = input.box_y_axis(),
+            ).update_layout(
+                template="seaborn",
+                title={"text": plot_title, "x": 0.5},
+            ).update_yaxes(
+                title_text = y_axis_title,
+            )
+
+            return box_plot
+        
+        # Histogram:
+        if input.plot_types() == "Histogram":
+            req(input.histogram_x_axis())
+            plot_title = input.histogram_plot_title()
+
+            # x_axis title
+            x_axis_title = input.histogram_x_axis_title()
+            y_axis_title = input.histogram_y_axis_title()
+
+            histogram = px.histogram(
+                data_frame = data_frame,
+                x = input.histogram_x_axis(),
+                nbins = input.histogram_bin_size(),
+            ).update_layout(
+                template="seaborn",
+                title={"text": plot_title, "x": 0.5},
+            ).update_xaxes(
+                title_text = x_axis_title,
+            ).update_yaxes(
+                title_text = y_axis_title,
+            )
+
+            return histogram
 
         # Scatter Plot:
         if input.plot_types() == "Scatter Plot":
             req(input.scatter_x_axis(), input.scatter_y_axis())
             plot_title = input.scatter_plot_title()
 
             # x_axis + yaxis title
```

### Comparing `vizable-0.7.0/VizAble/check_datatypes.py` & `vizable-0.8.0/VizAble/check_datatypes.py`

 * *Files identical despite different names*

### Comparing `vizable-0.7.0/VizAble/functions.py` & `vizable-0.8.0/VizAble/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
     return ui.update_select(
         id=axis_id,
         choices=choices,
         selected=None
     )
 
-def update_yaxis_input_select(plot_type: str, choices: List[str]):
+def update_yaxis_input_select(plot_type: str, choices: List[str]) -> ui.update_select:
     """ Update the y-axis dropdown based on the selected plot type.
 
     :param plot_type: The plot type selected by the user.
     :type plot_type: str
     :param choices: A list of column names for the dropdown based on the plot type.
     :type choices: List[str]
     :return: An updated x-axis dropdown based on the selected plot type.
```

### Comparing `vizable-0.7.0/VizAble/generate_plots.py` & `vizable-0.8.0/VizAble/generate_plots.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,30 @@
                         ),
                         # ui.input_select(
                         #     id="color_by",
                         #     label="Color by",
                         #     choices=["--------"]
                         # ),
                     ),
+
+                    # Show when user selects "Box Plot" on plot_types
+                    ui.panel_conditional(
+                        "input.plot_types == 'Box Plot'",
+                        ui.input_text(
+                            id="box_plot_title",
+                            label="Plot Title",
+                            placeholder="Enter a plot title"
+                        ),
+                        ui.input_text(
+                            id="box_y_axis_title",
+                            label="Y-axis Title",
+                            placeholder="Enter a title for the y-axis"
+                        ),
+                    ),
+
                     # Show when user selects "Bar Plot" on plot_types
                     ui.panel_conditional(
                         "input.plot_types == 'Bar Plot'",
                         ui.input_text(
                             id="bar_plot_title",
                             label="Plot Title",
                             placeholder="Enter a plot title"
@@ -59,14 +75,39 @@
                         ui.input_text(
                             id="bar_y_axis_title",
                             label="Y-axis Title",
                             placeholder="Enter a title for the y-axis"
                         ),
                     ),
 
+                    # Show when user selects "Histogram" on plot_types
+                    ui.panel_conditional(
+                        "input.plot_types == 'Histogram'",
+                        ui.input_text(
+                            id="histogram_plot_title",
+                            label="Plot Title",
+                            placeholder="Enter a plot title"
+                        ),
+                        ui.input_text(
+                            id="histogram_x_axis_title",
+                            label="X-axis Title",
+                            placeholder="Enter a title for the x-axis"
+                        ),
+                        ui.input_text(
+                            id="histogram_y_axis_title",
+                            label="Y-axis Title",
+                            placeholder="Enter a title for the y-axis"
+                        ),
+                        ui.input_numeric(
+                            id="histogram_bin_size",
+                            label="Bin Size",
+                            value=10,
+                        ),
+                    ),
+
                     # Show when user selects "Scatter Plot" on plot_types
                     ui.panel_conditional(
                         "input.plot_types == 'Scatter Plot'",
                         ui.input_text(
                             id="scatter_plot_title",
                             label="Plot Title",
                             placeholder="Enter a plot title"
```

### Comparing `vizable-0.7.0/VizAble/introductions.py` & `vizable-0.8.0/VizAble/introductions.py`

 * *Files identical despite different names*

### Comparing `vizable-0.7.0/VizAble/select_columns.py` & `vizable-0.8.0/VizAble/select_columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                         # add dropdown for x-axis
                         functions.xaxis_input_select("bar"),
                     ),
                     # Add condition: if user selects "Box Plot" on plot_types
                     ui.panel_conditional(
                         "input.plot_types == 'Box Plot'",
                         # add dropdown for x-axis
-                        functions.xaxis_input_select("box"),
+                        functions.yaxis_input_select("box"),
                     ),
                     # Add condition: if user selects "Histogram" on plot_types
                     ui.panel_conditional(
                         "input.plot_types == 'Histogram'",
                         # add dropdown for x-axis
                         functions.xaxis_input_select("histogram"),
                     ),
```

### Comparing `vizable-0.7.0/VizAble/select_plottypes.py` & `vizable-0.8.0/VizAble/select_plottypes.py`

 * *Files identical despite different names*

### Comparing `vizable-0.7.0/VizAble/upload_file.py` & `vizable-0.8.0/VizAble/upload_file.py`

 * *Files identical despite different names*

### Comparing `vizable-0.7.0/pyproject.toml` & `vizable-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "VizAble"
-version = "0.7.0"
+version = "0.8.0"
 description = "A web-based data visualization tool that generates accessible visualizations for all users, including people with visual impairments (low vision or blind)."
 license = "MIT"
 authors = ["Chi-Ying Chuang <rebekah890110@gmail.com>"]
 readme = "README.md"
 packages = [{include = "VizAble"}]
 
 [tool.poetry.dependencies]
```

### Comparing `vizable-0.7.0/PKG-INFO` & `vizable-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VizAble
-Version: 0.7.0
+Version: 0.8.0
 Summary: A web-based data visualization tool that generates accessible visualizations for all users, including people with visual impairments (low vision or blind).
 License: MIT
 Author: Chi-Ying Chuang
 Author-email: rebekah890110@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

