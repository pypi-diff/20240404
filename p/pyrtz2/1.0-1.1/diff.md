# Comparing `tmp/pyrtz2-1.0.tar.gz` & `tmp/pyrtz2-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.0.tar` & `pyrtz2-1.1.tar`

### file list

```diff
@@ -1,12 +1,41 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.0/.gitattributes
--rw-r--r--   0        0        0        7 2024-04-02 21:27:01.667717 pyrtz2-1.0/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.0/LICENSE
--rw-r--r--   0        0        0      228 2024-04-02 19:51:47.632334 pyrtz2-1.0/README.md
--rw-r--r--   0        0        0      701 2024-04-02 21:01:01.104769 pyrtz2-1.0/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-02 20:57:04.893373 pyrtz2-1.0/pyrtz2/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-02 19:31:54.209924 pyrtz2-1.0/pyrtz2/afm.py
--rw-r--r--   0        0        0     4718 2024-04-02 15:00:26.747427 pyrtz2-1.0/pyrtz2/asylum.py
--rw-r--r--   0        0        0    16836 2024-04-02 15:46:25.987342 pyrtz2-1.0/pyrtz2/curves.py
--rw-r--r--   0        0        0     1393 2024-04-02 14:54:57.251183 pyrtz2-1.0/pyrtz2/fig.py
--rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.0/pyrtz2/fit.py
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 pyrtz2-1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1/.gitattributes
+-rw-r--r--   0        0        0      105 2024-04-04 14:02:39.390822 pyrtz2-1.1/.vscode/settings.json
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1/LICENSE
+-rw-r--r--   0        0        0      228 2024-04-02 19:51:47.632334 pyrtz2-1.1/README.md
+-rw-r--r--   0        0        0     1644 2024-04-04 20:23:18.162380 pyrtz2-1.1/pyproject.toml
+-rw-r--r--   0        0        0       96 2024-04-04 20:22:51.086640 pyrtz2-1.1/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     1867 2024-04-04 19:07:59.221420 pyrtz2-1.1/pyrtz2/afm.py
+-rw-r--r--   0        0        0      372 2024-04-03 01:57:39.926418 pyrtz2-1.1/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     4711 2024-04-04 18:06:07.236982 pyrtz2-1.1/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    20122 2024-04-04 19:44:01.385877 pyrtz2-1.1/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     1970 2024-04-03 03:12:28.001519 pyrtz2-1.1/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     5604 2024-04-04 18:49:51.040442 pyrtz2-1.1/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4139 2024-04-03 02:17:21.251676 pyrtz2-1.1/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     3409 2024-04-04 18:23:41.184544 pyrtz2-1.1/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     4475 2024-04-04 18:07:38.738998 pyrtz2-1.1/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1241 2024-04-04 18:49:04.376522 pyrtz2-1.1/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     1195 2024-04-03 02:18:43.224430 pyrtz2-1.1/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1666 2024-04-02 01:29:34.764572 pyrtz2-1.1/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3461 2024-04-03 02:29:10.462290 pyrtz2-1.1/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1/pyrtz2/src/data/__init__.py
+-rw-r--r--   0        0        0     3346 2024-04-04 20:08:19.361627 pyrtz2-1.1/pyrtz2/src/data/downloader.py
+-rw-r--r--   0        0        0     1617 2024-04-04 20:06:58.075042 pyrtz2-1.1/pyrtz2/src/data/experiment_loader.py
+-rw-r--r--   0        0        0     1128 2024-04-03 02:24:32.297813 pyrtz2-1.1/pyrtz2/src/data/image_loader.py
+-rw-r--r--   0        0        0     1230 2024-04-04 20:00:47.653098 pyrtz2-1.1/pyrtz2/src/data/processor.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     1020 2024-03-29 20:53:21.746168 pyrtz2-1.1/pyrtz2/src/utils/_backup/igor/__init__.py
+-rw-r--r--   0        0        0    30699 2024-03-29 20:52:56.279210 pyrtz2-1.1/pyrtz2/src/utils/_backup/igor/binarywave.py
+-rw-r--r--   0        0        0    29217 2024-03-29 21:12:48.091560 pyrtz2-1.1/pyrtz2/src/utils/_backup/igor/structure.py
+-rw-r--r--   0        0        0     3911 2024-02-02 05:34:10.456245 pyrtz2-1.1/pyrtz2/src/utils/_backup/igor/util.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1/pyrtz2/src/utils/_backup/pyrtz/__init__.py
+-rw-r--r--   0        0        0     4623 2024-03-29 23:09:57.877567 pyrtz2-1.1/pyrtz2/src/utils/_backup/pyrtz/asylum.py
+-rw-r--r--   0        0        0    35543 2024-03-30 00:31:39.650484 pyrtz2-1.1/pyrtz2/src/utils/_backup/pyrtz/curves.py
+-rw-r--r--   0        0        0     2403 2024-04-04 18:28:36.838363 pyrtz2-1.1/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0     1852 2024-04-04 17:22:15.402815 pyrtz2-1.1/test.py
+-rw-r--r--   0        0        0     2026 1970-01-01 00:00:00.000000 pyrtz2-1.1/PKG-INFO
```

### Comparing `pyrtz2-1.0/LICENSE` & `pyrtz2-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.0/pyrtz2/afm.py` & `pyrtz2-1.1/pyrtz2/afm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import os
-from . import asylum
+import asylum
 
 
 class AFM():
     def __init__(
         self,
             path: str,
             exp_name: str,
```

### Comparing `pyrtz2-1.0/pyrtz2/asylum.py` & `pyrtz2-1.1/pyrtz2/asylum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from igor2 import binarywave as bw
 import numpy as np
 import pandas as pd
 import re
 import os
 
-from . import curves
+import curves
 
 
 def _get_notes(wave: dict) -> dict:
     '''Utility function for processing the 'notes' section of a .ibw file,
     the end user should not call this function'''
 
     note_raw = wave['wave']['note']
```

### Comparing `pyrtz2-1.0/pyrtz2/curves.py` & `pyrtz2-1.1/pyrtz2/curves.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from plotly import graph_objs as go
+import plotly.express as px
 
 import PyPDF2 as pdf
 import pickle
 import pandas as pd
 import numpy as np
 import json
 import ast
 import io
 from tqdm import tqdm
 from typing import Any, Iterable
 
-from .fit import lin_fit, poly_fit, hertzian_fit, biexponential_fit
-from .fig import make_fig
+from fit import lin_fit, poly_fit, hertzian_fit, biexponential_fit
+from src.components.fig import make_fig
 
 
 def read_json_file(file: str) -> dict[tuple, bool | int]:
     with open(file, 'rt') as cf:
         anno_str_dict = json.load(cf)
 
     anno_tuple_dict = {}
@@ -32,24 +33,26 @@
     corrected: bool = False
     contact_index: int = 0
     contact_values: pd.Series | None = None
     max_ind: float
     max_f: float
     vel_ind: float
     vel_z: float
+    figs_data: dict[str, tuple[np.ndarray, np.ndarray]]
+    fits_data: dict[str, tuple[np.ndarray, np.ndarray]]
     indent_param: list[float]
-    indent_r2: float
+    indent_R2: float
     hertzian_param: list[float]
-    hertzian_r2: float
+    hertzian_R2: float
     dwell_param: list[float]
-    dwell_r2: float
+    dwell_R2: float
     relaxation_param: list[float]
-    relaxation_r2: float
+    relaxation_R2: float
     contact_fig: go.Figure
-    dwell_relaxation_fig: go.Figure
+    dwell_relax_fig: go.Figure
 
     def __init__(
             self,
             filename: str,
             data: pd.DataFrame,
             notes: dict,
             invOLS: float,
@@ -142,30 +145,30 @@
 
     def correct_virtual_defl(self) -> None:
         self.check_contact()
         if self.corrected:
             self.restore_data()
 
         preapproach = self.get_preapproach()
-        x = preapproach['z'].values
-        y = preapproach['f'].values
+        x = preapproach['z'].to_numpy()
+        y = preapproach['f'].to_numpy()
         popt, _, _ = lin_fit(x, y)
         f_line = np.poly1d(popt)(self.data['z'])
         self.data['f'] = self.data['f'] - f_line
 
     def detect_contact(self) -> int:
         current_contact_index = self.contact_index
         approach = self.get_approach()
         max_index = len(approach) - 1
         index = max_index
         while True:
             self.set_contact_index(index)
             self.correct_virtual_defl()
             approach_new = self.get_approach()
-            force = approach_new['f'].values
+            force = approach_new['f'].to_numpy()
             mean = np.mean(force[:index+1])
 
             ratio = force[index] / force[-1]
             step_size = max(1, int((0.01 * max_index) ** ratio))
             index = index - step_size
             if force[index] < mean:
                 contact_index = index + 1
@@ -194,214 +197,295 @@
         dwell = self.get_dwell()
         return biexponential_fit(dwell['t'], dwell['f'])
 
     def fit_relaxation(self) -> tuple:
         relaxation = self.get_relaxation()
         return biexponential_fit(relaxation['t'], relaxation['ind'])
 
-    def get_contact_fig(self, vd: bool = False, adjust: bool = False) -> go.Figure:
-        fig = make_fig(
-            title=fr"$\text{{Selected Contact Point: {self.contact_index}}}$",
-            xaxis=r"$Z_{sensor} \text{ (m)}$"
-        )
+    def get_figs_data(self, vd: bool = False, adjust: bool = False) -> None:
+        if vd or adjust:
+            self.restore_data()
         if vd:
             self.correct_virtual_defl()
-
         if adjust:
             self.adjust_to_contact()
 
         approach = self.get_approach()
-        x = approach['ind']
-        y = approach['f']
-        hover_texts = [f'Index: {i}' for i in range(len(x))]
 
-        self.max_ind = max(x)
-        self.max_f = max(y)
+        dwell = self.get_dwell()
+        relaxation = self.get_relaxation()
+
+        self.figs_data = {
+            'approach': (approach['ind'].to_numpy(), approach['f'].to_numpy()),
+            'dwell': (dwell['t'].to_numpy(), dwell['f'].to_numpy()),
+            'relaxation': (relaxation['t'].to_numpy(), relaxation['ind'].to_numpy()),
+        }
+
+    def get_contact_fig_plot(self) -> go.Figure:
+        fig = make_fig(
+            title=fr"$\text{{Selected Contact Point: {self.contact_index}}}$",
+            xaxis=r"$Indentation \text{ (m)}$"
+        )
+
+        x, y = self.figs_data['approach']
+        hover_texts = [f'Index: {i}' for i in range(len(x))]
         trace = go.Scattergl(
             x=x,
             y=y,
             name='Approach',
             mode='markers',
             text=hover_texts,
             hoverinfo='text',
             hoverlabel={'bgcolor': 'red'},
             marker={'color': 'blue'},
         )
 
         fig.add_trace(trace)
 
-        x_line = x.iloc[self.contact_index]
-        y_line = y.iloc[self.contact_index]
+        x_line = x[self.contact_index]
+        y_line = y[self.contact_index]
         fig.add_vline(x=x_line, line=dict(color='red', width=1.2))
         fig.add_hline(y=y_line, line=dict(color='red', width=1.2))
         self.contact_fig = fig
         return fig
 
-    def add_contact_fit(self, probe_diameter: float, ind: float | list[float]) -> go.Figure:
-        indent = self.get_indent()
-        x = indent['ind']
-        self.indent_param, self.indent_r2, y_pred = self.fit_indent()
-
-        trace = go.Scattergl(
-            x=x,
-            y=y_pred,
-            name='PolyFit',
-            mode='lines',
-            line={'color': 'red'},
-        )
-        self.contact_fig.add_trace(trace)
-
-        if isinstance(ind, float):
-            self.hertzian_param, self.hertzian_r2, y_pred = self.fit_indent_until(
-                probe_diameter, ind)
-            x_pred = self.get_indent_until(ind)['ind']
-        elif isinstance(ind, list) and len(ind) == 2:
-            self.hertzian_param, self.hertzian_r2, y_pred = self.fit_indent_between(
-                probe_diameter, interval=ind)
-            x_pred = self.get_indent_between(ind[0], ind[1])['ind']
-        else:
-            return self.contact_fig
-
-        trace = go.Scattergl(
-            x=x_pred,
-            y=y_pred,
-            name='HertzianFit',
-            mode='lines',
-            line={
-                'color': 'green',
-                'width': 3,
-            },
-        )
-        self.contact_fig.add_trace(trace)
-
-        return self.contact_fig
-
-    def get_dwell_relaxation_fig(self, vd: bool = False, adjust: bool = False) -> go.Figure:
+    def get_dwell_relax_fig_plot(self) -> go.Figure:
         fig = make_fig(
             title=r"$\text{Dwell and Relaxation}$",
             xaxis=r"$Time \text{ (s)}$"
         )
+
         fig.update_layout(
             yaxis2=dict(
                 title=r"$Indentation \text{ (m)}$",
                 overlaying='y',
                 side='right'
             )
         )
-        if vd:
-            self.correct_virtual_defl()
-
-        if adjust:
-            self.adjust_to_contact()
-
-        dwell = self.get_dwell()
-        x = dwell['t']
-        y = dwell['f']
-        hover_texts = [f'Index: {i}' for i in range(len(x))]
 
+        x, y = self.figs_data['dwell']
         trace = go.Scattergl(
             x=x,
             y=y,
             name='Dwell',
             mode='markers',
-            text=hover_texts,
-            hoverinfo='text',
-            hoverlabel={'bgcolor': 'red'},
             marker={'color': 'red'},
         )
 
         fig.add_trace(trace)
 
-        relaxation = self.get_relaxation()
-        x = relaxation['t']
-        y = relaxation['ind']
-        hover_texts = [f'Index: {i}' for i in range(len(x))]
-
+        x, y = self.figs_data['relaxation']
         trace = go.Scattergl(
             x=x,
             y=y,
             yaxis='y2',
             name='Relaxation',
             mode='markers',
-            text=hover_texts,
-            hoverinfo='text',
-            hoverlabel={'bgcolor': 'red'},
             marker={'color': 'blue'},
         )
 
         fig.add_trace(trace)
 
-        self.dwell_relaxation_fig = fig
+        self.dwell_relax_fig = fig
         return fig
 
-    def add_dwell_relaxation_fit(self) -> go.Figure:
+    def get_fits_data(self, probe_diameter: float, ind: float | list[float]) -> None:
+        indent = self.get_indent()
+        indent_x_pred = indent['ind'].to_numpy()
+        self.indent_param, self.indent_R2, indent_y_pred = self.fit_indent()
+
+        self.max_ind = max(indent['ind'])
+        self.max_f = max(indent['f'])
+
+        if isinstance(ind, float):
+            self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_until(
+                probe_diameter, ind)
+            hertzian_x_pred = self.get_indent_until(ind)['ind'].to_numpy()
+        elif isinstance(ind, list) and len(ind) == 2:
+            self.hertzian_param, self.hertzian_R2, hertzian_y_pred = self.fit_indent_between(
+                probe_diameter, interval=ind)
+            hertzian_x_pred = self.get_indent_between(ind[0], ind[1])[
+                'ind'].to_numpy()
+
         dwell = self.get_dwell()
-        x = dwell['t']
-        self.dwell_param, self.dwell_r2, y_pred = self.fit_dwell()
+        dwell_x_pred = dwell['t'].to_numpy()
+        self.dwell_param, self.dwell_R2, dwell_y_pred = self.fit_dwell()
+
+        relaxation = self.get_relaxation()
+        relaxation_x_pred = relaxation['t'].to_numpy()
+        self.relaxation_param, self.relaxation_R2, relaxation_y_pred = self.fit_relaxation()
+
+        self.fits_data = {
+            'indent': (indent_x_pred, indent_y_pred),
+            'hertzian': (hertzian_x_pred, hertzian_y_pred),
+            'dwell': (dwell_x_pred, dwell_y_pred),
+            'relaxation': (relaxation_x_pred, relaxation_y_pred),
+        }
 
+    def add_contact_fit(self) -> go.Figure:
+        x, y = self.fits_data['indent']
         trace = go.Scattergl(
             x=x,
-            y=y_pred,
-            name='DwellFit',
+            y=y,
+            name='PolyFit',
+            mode='lines',
+            line={'color': 'red'},
+        )
+        self.contact_fig.add_trace(trace)
+
+        x, y = self.fits_data['hertzian']
+        trace = go.Scattergl(
+            x=x,
+            y=y,
+            name='HertzianFit',
             mode='lines',
             line={
                 'color': 'green',
                 'width': 3,
             },
         )
-        self.dwell_relaxation_fig.add_trace(trace)
+        self.contact_fig.add_trace(trace)
 
-        relaxation = self.get_relaxation()
-        x = relaxation['t']
-        self.relaxation_param, self.relaxation_r2, y_pred = self.fit_relaxation()
+        return self.contact_fig
+
+    def add_dwell_relax_fit(self) -> go.Figure:
+        x, y = self.fits_data['dwell']
 
         trace = go.Scattergl(
             x=x,
-            y=y_pred,
+            y=y,
+            name='DwellFit',
+            mode='lines',
+            line={
+                'color': 'green',
+                'width': 3,
+            },
+        )
+        self.dwell_relax_fig.add_trace(trace)
+
+        x, y = self.fits_data['relaxation']
+        trace = go.Scattergl(
+            x=x,
+            y=y,
             yaxis='y2',
             name='RelaxationFit',
             mode='lines',
             line={
                 'color': 'green',
                 'width': 3,
             },
         )
-        self.dwell_relaxation_fig.add_trace(trace)
+        self.dwell_relax_fig.add_trace(trace)
+
+        return self.dwell_relax_fig
+
+    def get_contact_fig_pdf(self) -> go.Figure:
+        title = fr"$\text{{Selected Contact Point: {self.contact_index}}}$"
+        xaxis = r"$Indentation \text{ (m)}$"
+        fig = make_fig(title, xaxis)
+
+        x, y = self.figs_data['approach']
+        trace = go.Scatter(x=x, y=y, name='Approach', marker={'color': 'blue'})
+        fig.add_trace(trace)
+
+        x_line = x[self.contact_index]
+        y_line = y[self.contact_index]
+        fig.add_shape(type='line', x0=x_line, x1=x_line, y0=min(y),
+                      y1=max(y), line=dict(color='red', width=1.2))
+        fig.add_shape(type='line', y0=y_line, y1=y_line, x0=min(x),
+                      x1=max(x), line=dict(color='red', width=1.2))
+
+        if hasattr(self, 'fits_data'):
+            x, y = self.fits_data['indent']
+            trace = go.Scatter(x=x, y=y, name='PolyFit',
+                               mode='lines', line={'color': 'red'})
+            fig.add_trace(trace)
+
+            x, y = self.fits_data['hertzian']
+            trace = go.Scatter(x=x, y=y, name='HertzianFit',
+                               mode='lines', line={'color': 'green', 'width': 3})
+            fig.add_trace(trace)
+
+        return fig
+
+    def get_dwell_relax_fig_pdf(self) -> go.Figure:
+        title = r"$\text{Dwell and Relaxation}$"
+        xaxis = r"$Time \text{ (s)}$"
+        fig = make_fig(title, xaxis)
+
+        x, y = self.figs_data['dwell']
+        trace = go.Scatter(x=x, y=y, name='Dwell',
+                           marker_color='red')
+        fig.add_trace(trace)
+
+        fig.update_layout(
+            yaxis2=dict(
+                title=r"$Indentation \text{ (m)}$",
+                overlaying='y',
+                side='right',
+                showgrid=False,
+                ticks='outside',
+                tickwidth=2,
+                showline=True,
+                linewidth=2,
+                linecolor='black',
+                tickprefix=r"$",
+                ticksuffix=r"$",
+            )
+        )
 
-        return self.dwell_relaxation_fig
+        x, y = self.figs_data['relaxation']
+        trace = go.Scatter(x=x, y=y, name='Relaxation',
+                           marker_color='blue', yaxis='y2')
+        fig.add_trace(trace)
+
+        if hasattr(self, 'fits_data'):
+            x, y = self.fits_data['dwell']
+            trace = go.Scatter(x=x, y=y, name='DwellFit',
+                               mode='lines', line={'color': 'green', 'width': 3})
+            fig.add_trace(trace)
+
+            x, y = self.fits_data['relaxation']
+            trace = go.Scatter(x=x, y=y, yaxis='y2', name='RelaxationFit',
+                               mode='lines', line={'color': 'green', 'width': 3})
+            fig.add_trace(trace)
+
+        return fig
 
-    def get_fit_data(self) -> dict:
+    def get_all_fits(self) -> dict:
         fit_results_dict = {
             'max_ind': self.max_ind,
             'max_f': self.max_f,
 
             'vel_ind': self.vel_ind,
             'vel_z': self.vel_z,
 
             'indent_a': self.indent_param[0],
             'indent_b': self.indent_param[1],
             'indent_c': self.indent_param[2],
-            'indent_r2': self.indent_r2,
+            'indent_R2': self.indent_R2,
 
             'Hertzian_E': self.hertzian_param[0],
-            'Hertzian_r2_': self.hertzian_r2,
+            'Hertzian_R2': self.hertzian_R2,
 
             'dwell_c': self.dwell_param[0],
             'dwell_tau1': self.dwell_param[1],
             'dwell_tau2': self.dwell_param[2],
             'dwell_tauMax': max(self.dwell_param[1], self.dwell_param[2]),
             'dwell_tauMin': min(self.dwell_param[1], self.dwell_param[2]),
-            'dwell_r2': self.dwell_r2,
+            'dwell_yf': self.dwell_param[3],
+            'dwell_R2': self.dwell_R2,
 
             'relaxation_c': self.relaxation_param[0],
             'relaxation_tau1': self.relaxation_param[1],
             'relaxation_tau2': self.relaxation_param[2],
             'relaxation_tauMax': max(self.relaxation_param[1], self.relaxation_param[2]),
             'relaxation_tauMin': min(self.relaxation_param[1], self.relaxation_param[2]),
-            'relaxation_r2': self.relaxation_r2
+            'relaxation_yf': self.relaxation_param[3],
+            'relaxation_R2': self.relaxation_R2
         }
 
         return fit_results_dict
 
 
 class CurveSet:
     vd_dict: dict[tuple[str], bool] = {}
@@ -491,41 +575,39 @@
     def get_fit_all(self, probe_diameter: float, ind: float | list[float]) -> pd.DataFrame:
         self.prepare_fit_all()
         all_fit = []
 
         for key, curve in tqdm(self.items()):
             fit_results_dict = {label: key_value for label,
                                 key_value in zip(self.ident_labels, key)}
-            curve.get_contact_fig()
-            curve.add_contact_fit(probe_diameter, ind)
-            curve.get_dwell_relaxation_fig()
-            curve.add_dwell_relaxation_fit()
+            curve.get_fits_data(probe_diameter, ind)
             curve.get_approach_rates()
-            fit_results_dict.update(curve.get_fit_data())
+            fit_results_dict.update(curve.get_all_fits())
             fit_results = pd.DataFrame([fit_results_dict])
             all_fit.append(fit_results)
 
         combined_results = pd.concat(all_fit, ignore_index=True)
 
         return combined_results
 
     def export_figures(self) -> pdf.PdfMerger:
         merger = pdf.PdfMerger()
         for key, curve in tqdm(self.items()):
+            curve.get_figs_data()
             title = ""
             for label, ident in zip(self.ident_labels, key):
                 title += label + ident
 
             title = fr"$\text{{{title}}}$"
-            contact_fit_fig = curve.contact_fig
+            contact_fit_fig = curve.get_contact_fig_pdf()
             contact_fit_fig.update_layout(title={'text': title})
             contact_fit_fig_pdf = io.BytesIO(
                 contact_fit_fig.to_image(format='pdf'))
             merger.append(contact_fit_fig_pdf)
 
-            dwell_relaxation_fit_fig = curve.dwell_relaxation_fig
+            dwell_relaxation_fit_fig = curve.get_dwell_relax_fig_pdf()
             dwell_relaxation_fit_fig.update_layout(title={'text': title})
             dwell_relaxation_fit_fig_pdf = io.BytesIO(
                 dwell_relaxation_fit_fig.to_image(format='pdf'))
             merger.append(dwell_relaxation_fit_fig_pdf)
 
         return merger
```

### Comparing `pyrtz2-1.0/pyrtz2/fit.py` & `pyrtz2-1.1/pyrtz2/fit.py`

 * *Files identical despite different names*

