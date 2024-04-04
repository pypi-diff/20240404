# Comparing `tmp/interplot-0.1.1.tar.gz` & `tmp/interplot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interplot-0.1.1.tar", last modified: Sat Feb 10 15:23:19 2024, max compression
+gzip compressed data, was "interplot-0.1.2.tar", last modified: Thu Apr  4 19:14:23 2024, max compression
```

## Comparing `interplot-0.1.1.tar` & `interplot-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 Janjo      (502) staff       (20)        0 2024-02-10 15:23:19.214757 interplot-0.1.1/
--rw-r--r--   0 Janjo      (502) staff       (20)    35112 2023-12-30 11:25:15.000000 interplot-0.1.1/LICENCE.txt
--rw-r--r--   0 Janjo      (502) staff       (20)       42 2023-12-31 13:00:34.000000 interplot-0.1.1/MANIFEST.in
--rw-r--r--   0 Janjo      (502) staff       (20)     4800 2024-02-10 15:23:19.213308 interplot-0.1.1/PKG-INFO
--rw-r--r--   0 Janjo      (502) staff       (20)     3843 2024-02-10 15:00:35.000000 interplot-0.1.1/README.md
-drwxr-xr-x   0 Janjo      (502) staff       (20)        0 2024-02-10 15:23:19.203184 interplot-0.1.1/interplot/
--rw-r--r--   0 Janjo      (502) staff       (20)      452 2023-12-30 11:44:38.000000 interplot-0.1.1/interplot/__init__.py
--rw-r--r--   0 Janjo      (502) staff       (20)    10697 2024-02-10 15:00:37.000000 interplot-0.1.1/interplot/arraytools.py
--rw-r--r--   0 Janjo      (502) staff       (20)     8199 2023-12-30 13:37:35.000000 interplot-0.1.1/interplot/iter.py
--rw-r--r--   0 Janjo      (502) staff       (20)    80919 2024-02-10 15:00:37.000000 interplot-0.1.1/interplot/plot.py
-drwxr-xr-x   0 Janjo      (502) staff       (20)        0 2024-02-10 15:23:19.212290 interplot-0.1.1/interplot.egg-info/
--rw-r--r--   0 Janjo      (502) staff       (20)     6148 2023-12-31 12:47:07.000000 interplot-0.1.1/interplot.egg-info/.DS_Store
--rw-r--r--   0 Janjo      (502) staff       (20)     4800 2024-02-10 15:23:19.000000 interplot-0.1.1/interplot.egg-info/PKG-INFO
--rw-r--r--   0 Janjo      (502) staff       (20)      363 2024-02-10 15:23:19.000000 interplot-0.1.1/interplot.egg-info/SOURCES.txt
--rw-r--r--   0 Janjo      (502) staff       (20)        1 2024-02-10 15:23:19.000000 interplot-0.1.1/interplot.egg-info/dependency_links.txt
--rw-r--r--   0 Janjo      (502) staff       (20)       58 2024-02-10 15:23:19.000000 interplot-0.1.1/interplot.egg-info/requires.txt
--rw-r--r--   0 Janjo      (502) staff       (20)       10 2024-02-10 15:23:19.000000 interplot-0.1.1/interplot.egg-info/top_level.txt
--rw-r--r--   0 Janjo      (502) staff       (20)      102 2023-12-31 12:44:21.000000 interplot-0.1.1/pyproject.toml
--rw-r--r--   0 Janjo      (502) staff       (20)      176 2024-02-10 15:21:38.000000 interplot-0.1.1/readme_dev.md
--rw-r--r--   0 Janjo      (502) staff       (20)       58 2023-12-31 12:53:25.000000 interplot-0.1.1/requirements.txt
--rw-r--r--   0 Janjo      (502) staff       (20)       38 2024-02-10 15:23:19.215171 interplot-0.1.1/setup.cfg
--rw-r--r--   0 Janjo      (502) staff       (20)     1223 2024-02-10 11:07:37.000000 interplot-0.1.1/setup.py
+drwxr-xr-x   0 Janjo      (502) staff       (20)        0 2024-04-04 19:14:23.455397 interplot-0.1.2/
+-rw-r--r--   0 Janjo      (502) staff       (20)    35112 2023-12-30 11:25:15.000000 interplot-0.1.2/LICENCE.txt
+-rw-r--r--   0 Janjo      (502) staff       (20)       42 2023-12-31 13:00:34.000000 interplot-0.1.2/MANIFEST.in
+-rw-r--r--   0 Janjo      (502) staff       (20)     5593 2024-04-04 19:14:23.454456 interplot-0.1.2/PKG-INFO
+-rw-r--r--   0 Janjo      (502) staff       (20)     4631 2024-04-04 18:52:26.000000 interplot-0.1.2/README.md
+drwxr-xr-x   0 Janjo      (502) staff       (20)        0 2024-04-04 19:14:23.439571 interplot-0.1.2/interplot/
+-rw-r--r--   0 Janjo      (502) staff       (20)      464 2024-04-04 18:52:27.000000 interplot-0.1.2/interplot/__init__.py
+-rw-r--r--   0 Janjo      (502) staff       (20)    10697 2024-02-10 15:55:27.000000 interplot-0.1.2/interplot/arraytools.py
+-rw-r--r--   0 Janjo      (502) staff       (20)     8988 2024-04-04 18:52:27.000000 interplot-0.1.2/interplot/conf.py
+-rw-r--r--   0 Janjo      (502) staff       (20)     8373 2024-04-04 18:52:27.000000 interplot-0.1.2/interplot/iter.py
+-rw-r--r--   0 Janjo      (502) staff       (20)    82785 2024-04-04 19:05:18.000000 interplot-0.1.2/interplot/plot.py
+drwxr-xr-x   0 Janjo      (502) staff       (20)        0 2024-04-04 19:14:23.453219 interplot-0.1.2/interplot.egg-info/
+-rw-r--r--   0 Janjo      (502) staff       (20)     6148 2023-12-31 12:47:07.000000 interplot-0.1.2/interplot.egg-info/.DS_Store
+-rw-r--r--   0 Janjo      (502) staff       (20)     5593 2024-04-04 19:14:23.000000 interplot-0.1.2/interplot.egg-info/PKG-INFO
+-rw-r--r--   0 Janjo      (502) staff       (20)      381 2024-04-04 19:14:23.000000 interplot-0.1.2/interplot.egg-info/SOURCES.txt
+-rw-r--r--   0 Janjo      (502) staff       (20)        1 2024-04-04 19:14:23.000000 interplot-0.1.2/interplot.egg-info/dependency_links.txt
+-rw-r--r--   0 Janjo      (502) staff       (20)       58 2024-04-04 19:14:23.000000 interplot-0.1.2/interplot.egg-info/requires.txt
+-rw-r--r--   0 Janjo      (502) staff       (20)       10 2024-04-04 19:14:23.000000 interplot-0.1.2/interplot.egg-info/top_level.txt
+-rw-r--r--   0 Janjo      (502) staff       (20)      102 2023-12-31 12:44:21.000000 interplot-0.1.2/pyproject.toml
+-rw-r--r--   0 Janjo      (502) staff       (20)      228 2024-03-29 22:51:26.000000 interplot-0.1.2/readme_dev.md
+-rw-r--r--   0 Janjo      (502) staff       (20)       58 2023-12-31 12:53:25.000000 interplot-0.1.2/requirements.txt
+-rw-r--r--   0 Janjo      (502) staff       (20)       38 2024-04-04 19:14:23.455551 interplot-0.1.2/setup.cfg
+-rw-r--r--   0 Janjo      (502) staff       (20)     1228 2024-04-04 18:52:27.000000 interplot-0.1.2/setup.py
```

### Comparing `interplot-0.1.1/LICENCE.txt` & `interplot-0.1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `interplot-0.1.1/PKG-INFO` & `interplot-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: interplot
-Version: 0.1.1
-Summary: Create matplotlib/plotly hybrid plots with a few lines of code.
+Version: 0.1.2
+Summary: Create matplotlib and plotly charts with the same few lines of code.
 Home-page: https://github.com/janjoch/interplot
 Author: Janosch Jörg
 Author-email: janjo@duck.com
 License: GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,26 +23,30 @@
 Requires-Dist: matplotlib
 Requires-Dist: plotly
 Requires-Dist: kaleido
 Requires-Dist: scipy
 Requires-Dist: xarray
 
 # interplot
-Create `matplotlib/plotly` hybrid plots with a few lines of code.
 
-It combines the best of the `matplotlib` and the `plotly` worlds through
-a unified, flat API.
-All the necessary boilerplate code is contained in this module.
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/janjoch/interplot/HEAD) [![NBViewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/janjoch/interplot/tree/main/)
+
+Create `matplotlib` and `plotly` charts with the same few lines of code.
+
+It combines the best of the `matplotlib` and the `plotly` worlds through a unified, flat API.
+
+Switch between `matplotlib` and `plotly` with the single keyword `interactive`. All the necessary boilerplate code to translate between the packages is contained in this module.
 
 Currently supported building blocks:
 
 - scatter plots
     - `line`
     - `scatter`
     - `linescatter`
+- bar charts `bar`
 - histogram `hist`
 - boxplot `boxplot`
 - heatmap `heatmap`
 - linear regression `regression`
 - line fill `fill`
 - annotations `text`
 
@@ -123,14 +127,15 @@
         saved figure at export/path/file.html
         ```
 
 
 ## Resources
 
 - **Documentation:** https://interplot.janjo.ch
+- **Demo Notebooks:** https://nbviewer.org/github/janjoch/interplot/tree/main/demo/
 - **Source Code:** https://github.com/janjoch/interplot
 - **PyPI:** https://pypi.org/project/interplot/
 
 
 ## Licence
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
@@ -149,7 +154,12 @@
 ```pip install interplot```
 
 
 ### dev installation
 1. ```git clone https://github.com/janjoch/interplot```
 2. ```cd interplot```
 2. ```pip install -e .```
+
+
+## Contribute
+
+Ideas, bug reports/fixes, feature requests and code submissions are very welcome! Please write to [janjo@duck.com](mailto:janjo@duck.com) or directly into a pull request.
```

### Comparing `interplot-0.1.1/README.md` & `interplot-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # interplot
-Create `matplotlib/plotly` hybrid plots with a few lines of code.
 
-It combines the best of the `matplotlib` and the `plotly` worlds through
-a unified, flat API.
-All the necessary boilerplate code is contained in this module.
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/janjoch/interplot/HEAD) [![NBViewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/janjoch/interplot/tree/main/)
+
+Create `matplotlib` and `plotly` charts with the same few lines of code.
+
+It combines the best of the `matplotlib` and the `plotly` worlds through a unified, flat API.
+
+Switch between `matplotlib` and `plotly` with the single keyword `interactive`. All the necessary boilerplate code to translate between the packages is contained in this module.
 
 Currently supported building blocks:
 
 - scatter plots
     - `line`
     - `scatter`
     - `linescatter`
+- bar charts `bar`
 - histogram `hist`
 - boxplot `boxplot`
 - heatmap `heatmap`
 - linear regression `regression`
 - line fill `fill`
 - annotations `text`
 
@@ -95,14 +99,15 @@
         saved figure at export/path/file.html
         ```
 
 
 ## Resources
 
 - **Documentation:** https://interplot.janjo.ch
+- **Demo Notebooks:** https://nbviewer.org/github/janjoch/interplot/tree/main/demo/
 - **Source Code:** https://github.com/janjoch/interplot
 - **PyPI:** https://pypi.org/project/interplot/
 
 
 ## Licence
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
@@ -121,7 +126,12 @@
 ```pip install interplot```
 
 
 ### dev installation
 1. ```git clone https://github.com/janjoch/interplot```
 2. ```cd interplot```
 2. ```pip install -e .```
+
+
+## Contribute
+
+Ideas, bug reports/fixes, feature requests and code submissions are very welcome! Please write to [janjo@duck.com](mailto:janjo@duck.com) or directly into a pull request.
```

### Comparing `interplot-0.1.1/interplot/arraytools.py` & `interplot-0.1.2/interplot/arraytools.py`

 * *Files identical despite different names*

### Comparing `interplot-0.1.1/interplot/iter.py` & `interplot-0.1.2/interplot/iter.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     Returns
     -------
     generator function
         which always returns arg.
 
     Examples
     --------
-    >>> for a, b, c, d, e in zip_smart(
+    >>> for a, b, c, d, e in interplot.zip_smart(
     ...     ("A", "B", "C", "D"),
     ...     True,
-    ...     [1, 2, 3, 4],
+    ...     [1, 2, 3, 4, 5],  # notice the extra element won't be unpacked
     ...     "always the same",
-    ...     repeat((1, 2)),
+    ...     interplot.repeat((1, 2)),
     ... ):
     ...     print(a, b, c, d, e)
     A True 1 always the same (1, 2)
     B True 2 always the same (1, 2)
     C True 3 always the same (1, 2)
     D True 4 always the same (1, 2)
     """
@@ -89,20 +89,20 @@
     Returns
     -------
     zip object
         Use it as you would use `zip`
 
     Examples
     --------
-    >>> for a, b, c, d, e in zip_smart(
+    >>> for a, b, c, d, e in interplot.zip_smart(
     ...     ("A", "B", "C", "D"),
     ...     True,
-    ...     [1, 2, 3, 4],
+    ...     [1, 2, 3, 4, 5],  # notice the extra element won't be unpacked
     ...     "always the same",
-    ...     repeat((1, 2)),
+    ...     interplot.repeat((1, 2)),
     ... ):
     ...     print(a, b, c, d, e)
     A True 1 always the same (1, 2)
     B True 2 always the same (1, 2)
     C True 3 always the same (1, 2)
     D True 4 always the same (1, 2)
     """
@@ -253,20 +253,22 @@
 
     # no hit
     return iterable
 
 
 class NoZip:
     """
-    DEPRECATED: use `repeat` instead.
+    DEPRECATED: use `interplot.repeat` instead.
+
+    Avoid iteration in `zip` and `interplot.zip_smart`
+    """
 
-    Avoid iteration in `zip` and `zip_smart`"""
     def __init__(self, iterable):
         """
-        DEPRECATED: use `repeat` instead.
+        DEPRECATED: use `interplot.repeat` instead.
 
         Avoid iteration of an iterable data type in the `zip` function.
 
         Class allows iteration and subscription.
 
         Call the instance to release the original variable.
```

### Comparing `interplot-0.1.1/interplot/plot.py` & `interplot-0.1.2/interplot/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 
 
 import re
 from warnings import warn
 from pathlib import Path
 from functools import wraps
 from datetime import datetime
+from io import BytesIO
 
 import numpy as np
 
 from pandas.core.series import Series as pd_Series
 from pandas.core.frame import DataFrame as pd_DataFrame
 
 from xarray.core.dataarray import DataArray as xr_DataArray
@@ -110,276 +111,55 @@
 import matplotlib.colors as mcolors
 
 import plotly.graph_objects as go
 import plotly.express as px
 import plotly.subplots as sp
 import plotly.offline
 
+from . import conf
 from .iter import ITERABLE_TYPES, zip_smart, filter_nozip
 from interplot import arraytools
 
 
 def init_notebook_mode(connected=False):
     """
-    Initialize plotly.js in the browser if not already done.
+    Initialize plotly.js in the browser if not already done,
+    and deactivate matplotlib auto-display.
 
     Parameters
     ----------
     connected: bool, optional
         If True, the plotly.js library will be loaded from an online CDN.
         If False, the plotly.js library will be loaded locally.
         Default: False
     """
     plotly.offline.init_notebook_mode(connected=connected)
 
+    # turn off matplotlib auto-display
+    plt.plot()
+    plt.close()
+    plt.ioff()
+
 
 # if imported in notebook, init plotly notebook mode
 try:
     __IPYTHON__  # type: ignore
-    from IPython.core.display import display_html
+    from IPython.core.display import display_html, display_png
     CALLED_FROM_NOTEBOOK = True
 except NameError:
     CALLED_FROM_NOTEBOOK = False
 if CALLED_FROM_NOTEBOOK:
     init_notebook_mode()
 
 
-COLOR_CYCLE = [  # optimised for color vision deficiencies
-    '#006BA4', '#FF800E', '#ABABAB', '#595959', '#5F9ED1',
-    '#C85200', '#898989', '#A2C8EC', '#FFBC79', '#CFCFCF',
-]
-
-PTY_LINE_STYLES = {
-    "-": "solid",
-    "--": "dash",
-    "-.": "dashdot",
-    ":": "dot",
-    "solid": "solid",
-    "dashed": "dash",
-    "dashdot": "dashdot",
-    "dotted": "dot",
-}
-MPL_LINE_STYLES = {
-    value: key for key, value in PTY_LINE_STYLES.items()
-}
-
-PTY_MARKERS = {
-    ".": "circle",
-    "s": "square",
-    "D": "diamond",
-    "P": "cross",
-    "X": "x",
-    "^": "triangle-up",
-    "v": "triangle-down",
-    "<": "triangle-left",
-    ">": "triangle-right",
-    "triangle-ne": "triangle-ne",
-    "triangle-se": "triangle-se",
-    "triangle-sw": "triangle-sw",
-    "triangle-nw": "triangle-nw",
-    "p": "pentagon",
-    "h": "hexagon",
-    "H": "hexagon2",
-    "8": "octagon",
-    "*": "star",
-    "hexagram": "hexagram",
-    "star-triangle-up": "star-triangle-up",
-    "star-triangle-down": "star-triangle-down",
-    "star-square": "star-square",
-    "star-diamond": "star-diamond",
-    "d": "diamond-tall",
-    "diamond-wide": "diamond-wide",
-    "hourglass": "hourglass",
-    "bowtie": "bowtie",
-    "circle-cross": "circle-cross",
-    "circle-x": "circle-x",
-    "square-cross": "square-cross",
-    "square-x": "square-x",
-    "diamond-cross": "diamond-cross",
-    "diamond-x": "diamond-x",
-    "+": "cross-thin",
-    "x": "x-thin",
-    "asterisk": "asterisk",
-    "hash": "hash",
-    "2": "y-up",
-    "1": "y-down",
-    "3": "y-left",
-    "4": "y-right",
-    "_": "line-ew",
-    "|": "line-ns",
-    "line-ne": "line-ne",
-    "line-nw": "line-nw",
-    6: "arrow-up",
-    7: "arrow-down",
-    4: "arrow-left",
-    5: "arrow-right",
-    "arrow-bar-up": "arrow-bar-up",
-    "arrow-bar-down": "arrow-bar-down",
-    "arrow-bar-left": "arrow-bar-left",
-    "arrow-bar-right": "arrow-bar-right",
-    "arrow": "arrow",
-    "arrow-wide": "arrow-wide",
-}
-PTY_MARKERS_LIST = list(PTY_MARKERS.values())
-MPL_MARKERS = {
-    value: key for key, value in PTY_MARKERS.items()
-}
-MPL_MARKERS.update({  # next best matches
-    "triangle-nw": "^",
-    "triangle-ne": ">",
-    "triangle-se": "v",
-    "triangle-sw": "<",
-    "hexagram": "*",
-    "star-triangle-up": "^",
-    "star-triangle-down": "v",
-    "star-square": "s",
-    "star-diamond": "D",
-    "diamond-wide": "D",
-    "hourglass": "d",
-    "bowtie": "D",
-    "circle-cross": "+",
-    "circle-x": "x",
-    "cross-thin": "+",
-    "square-cross": "s",
-    "square-x": "s",
-    "diamond-cross": "D",
-    "diamond-x": "D",
-    "x-thin": "x",
-    "hash": "*",
-    "asterisk": "*",
-    "line-ne": "|",
-    "line-nw": "_",
-    "arrow-bar-up": 6,
-    "arrow-bar-down": 7,
-    "arrow-bar-left": 4,
-    "arrow-bar-right": 5,
-    "arrow": 6,
-    "arrow-wide": 6,
-})
-MPL_MARKERS_LIST = list(MPL_MARKERS.values())
-
-EXPORT_FORMAT = "png"
-EXPORT_REPLACE = {
-    "[ ]?/[ ]?": "_",
-    " ": "-",
-    "[@!?,:;+*%&()=#|'\"]": "",
-    r"\\": "_",
-    r"\s": "_",
-    r"<\s*br\s*/?\s*>": "_",
-}
-PTY_CONFIG = dict(
-    displaylogo=False,
-)
-
-REWRITE_DOCSTRING = True
-
-DOCSTRING_DECORATOR = """
-    interactive: bool, default: True
-        Display an interactive plotly line plot
-        instead of the default matplotlib figure.
-    rows, cols: int, default: 1
-        Create a grid with x rows and y columns.
-    title: str, default: None
-        Plot title.
-    xlabel, ylabel: str or str tuple, default: None
-        Axis labels.
-
-        Either one title for the entire axis or one for each row/column.
-    xlim, ylim: tuple of 2 numbers or nested, default: None
-        Axis range limits.
-
-        In case of multiple rows/cols provide either:
-            - a tuple
-            - a tuple for each row
-            - a tuple for each row containing tuple for each column.
-    shared_xaxes, shared_yaxes: str, default: None
-        Define how multiple subplots share there axes.
-
-        Options:
-            - "all" or True
-            - "rows"
-            - "columns" or "cols"
-            - None or False
-    column_widths, row_heights: tuple/list, default: None
-        Ratios of the width/height dimensions in each column/row.
-        Will be normalised to a sum of 1.
-    fig_size: tuple of 2x float, optional
-        Figure size in pixels.
-
-        Default behavior:
-            - MPL: Default figure size.
-            - PLT: Responsive sizing.
-    dpi: int, default: 100
-        Plot resolution.
-    legend_loc: str, optional
-        MATPLOTLIB ONLY.
-
-        Default:
-            - In case of 1 line: None
-            - In case of >1 line: "best" (auto-detect)
-    legend_title: str, default: None
-        MPL: Each subplot has its own legend, so a 2d list in the shape of
-        the subplots may be provided.
-
-        PTY: Just provide a `str`.
-    save_fig: str or pathlib.Path, default: None
-        Provide a path to export the plot.
-
-        Possible formats: png, jpg, svg, html, ...
-
-        The figure will only be saved on calling the instance's
-        `.post_process()`.
-
-        If a directory (or `True` for local directory) is provided,
-        the filename will be automatically generated based on the title.
-
-        An iterable of multiple paths / filenames may be provided. In this case
-        the save command will be repeated for each element.
-    save_format: str, default: None
-        Provide a format for the exported plot, if not declared in `save_fig`.
-
-        An iterable of multiple formats may be provided. In this case
-        the save command will be repeated for each element.
-    pty_update_layout: dict, default: None
-        PLOTLY ONLY.
-        Pass keyword arguments to plotly's
-        `fig.update_layout(**pty_update_layout)`
-        Thus, take full control over
-    pty_custom_func: function, default: None
-        PLOTLY ONLY.
-        Pass a function reference to further style the plotly graphs.
-        Function must accept `fig` and return `fig`.
-
-        >>> def pty_custom_func(fig):
-        ...     fig.do_stuff()
-        ...     return fig
-    mpl_custom_func: function, default: None
-        MATPLOTLIB ONLY.
-        Pass a function reference to further style the matplotlib graphs.
-        Function must accept `fig, ax` and return `fig, ax`.
-
-        Note: `ax` always has `row` and `col` coordinates, even if the plot is
-        just 1x1.
-
-        >>> def mpl_custom_func(fig, ax):
-        ...     fig.do_stuff()
-        ...     ax[0, 0].do_more()
-        ...     return fig, ax
-
-    Returns
-    -------
-    `interplot.Plot` instance
-"""
-
-
 def _rewrite_docstring(doc_core, doc_decorator=None, kwargs_remove=()):
     """
     Appends arguments to a docstring.
 
-    Returns original docstring if REWRITE_DOCSTRING is set to False.
+    Returns original docstring if conf._REWRITE_DOCSTRING is set to False.
 
     Attempts:
     1. Search for [decorator.*?].
     2. Search for numpy-style "Parameters" block.
     3. Append to the end.
 
     Parameters
@@ -393,21 +173,21 @@
 
     Returns
     -------
     str:
         Rewritten docstring
     """
     # check rewrite flag
-    if not REWRITE_DOCSTRING:
+    if not conf._REWRITE_DOCSTRING:
         return doc_core
 
     # input check
     doc_core = "" if doc_core is None else doc_core
     doc_decorator = (
-        DOCSTRING_DECORATOR
+        conf._DOCSTRING_DECORATOR
         if doc_decorator is None
         else doc_decorator
     )
 
     # find indentation level of doc_core
     match = re.match("^\n?(?P<indent_core>[ \t]*)", doc_core)
     indent_core = match.group("indent_core") if match else ""
@@ -486,15 +266,15 @@
                 indent_decorator,
                 doc_parts["indent_core"],
                 doc_decorator,
             )
             + doc_parts["rest"]
         )
 
-    # non-numpy DOCSTRING_DECORATOR, just append in the end
+    # non-numpy _DOCSTRING_DECORATOR, just append in the end
     return doc_core + _adjust_indent(
         indent_decorator,
         indent_core,
         doc_decorator,
     )
 
 
@@ -555,80 +335,116 @@
     return re.sub(
         r"\n{}".format(indent_decorator),
         r"\n{}".format(indent_core),
         docstring,
     )
 
 
-def _serialize_2d(core):
+def _serialize_2d(serialize_pty=True, serialize_mpl=True):
     """Decorator to catch 2D arrays and other data types to unpack."""
 
-    @wraps(core)
-    def wrapper(self, x, y=None, label=None, **kwargs):
-        """
-        Wrapper function for a method.
+    def decorator(core):
 
-        If a pandas object is provided, the index will be used as x
-        if no x is provided.
-        Pandas column naming:
-            * If no label is set, the column name will be used by default.
-            * Manually set label string has priority.
-            * Label strings may contain a {} to insert the column name.
-            * Instead of setting a string, a callable may be provided to
-              reformat the column name. It must accept the column name
-              and return a string. E.g.:
-
-              > interplot.line(df, label=lambda n: n.strip())
-
-              > def capitalize(prefix="", suffix=""):
-              >     return lambda name: prefix + name.upper() + suffix
-              > interplot.line(df, label=capitalize("Cat. A: "))
-        xarray DataArrays will be convered to pandas and then handled
-        accordingly.
-        """
-        if y is None:
-
-            # xarray DataArray
-            if isinstance(x, xr_DataArray):
-                x = x.to_pandas()
-
-            # pd.Series
-            if isinstance(x, pd_Series):
-                index = x.index
-                y = x
-                x = index
-                if label is None:
-                    label = y.name
-                elif isinstance(label, str) and "{}" in label:
-                    label = label.format(y.name)
-                elif callable(label):
-                    label = label(y.name)
-
-            # pd.DataFrame: split columns to pd.Series and iterate
-            elif isinstance(x, pd_DataFrame):
-                for (_, series), label_ in zip_smart(x.items(), label):
-                    self.add_line(series, label=label_, **kwargs)
-                return
+        @wraps(core)
+        def wrapper(self, x, y=None, label=None, **kwargs):
+            """
+            Wrapper function for a method.
+
+            If a pandas object is provided, the index will be used as x
+            if no x is provided.
+            Pandas column naming:
+                * If no label is set, the column name will be used by default.
+                * Manually set label string has priority.
+                * Label strings may contain a {} to insert the column name.
+                * Instead of setting a string, a callable may be provided to
+                reformat the column name. It must accept the column name
+                and return a string. E.g.:
+
+                > interplot.line(df, label=lambda n: n.strip())
+
+                > def capitalize(prefix="", suffix=""):
+                >     return lambda name: prefix + name.upper() + suffix
+                > interplot.line(df, label=capitalize("Cat. A: "))
+            xarray DataArrays will be convered to pandas and then handled
+            accordingly.
+            """
+            # reallocate x/y
+            if y is None:
+
+                # xarray DataArray
+                if isinstance(x, xr_DataArray):
+                    x = x.to_pandas()
+
+                # pd.Series
+                if isinstance(x, pd_Series):
+                    x, y = x.index, x
+                    if label is None:
+                        label = y.name
+                    elif isinstance(label, str) and "{}" in label:
+                        label = label.format(y.name)
+                    elif callable(label):
+                        label = label(y.name)
+
+                # pd.DataFrame: split columns to pd.Series and iterate
+                elif isinstance(x, pd_DataFrame):
+                    if (
+                        self.interactive and serialize_pty
+                        or not self.interactive and serialize_mpl
+                    ):
+                        for (
+                            i, ((_, series), label_)
+                        ) in enumerate(zip_smart(x.items(), label)):
+                            _serialize_2d(
+                                serialize_pty=serialize_pty,
+                                serialize_mpl=serialize_mpl,
+                            )(core)(
+                                self,
+                                series,
+                                label=label_,
+                                _serial_i=i,
+                                _serial_n=len(x.columns),
+                                **kwargs,
+                            )
+                        return
 
-            else:
-                if hasattr(x, 'copy') and callable(getattr(x, 'copy')):
-                    y = x.copy()
                 else:
-                    y = x
-                x = np.arange(len(y))
+                    if hasattr(x, 'copy') and callable(getattr(x, 'copy')):
+                        y = x.copy()
+                    else:
+                        y = x
+                    x = np.arange(len(y))
 
-        # 2D np.array
-        if isinstance(y, np.ndarray) and len(y.shape) == 2:
-            for y_, label_ in zip_smart(y.T, label):
-                self.add_line(x, y_, label=label_, **kwargs)
-            return
+            # 2D np.array
+            if isinstance(y, np.ndarray) and len(y.shape) == 2:
+                if (
+                    self.interactive and serialize_pty
+                    or not self.interactive and serialize_mpl
+                ):
+                    for (
+                        i, (y_, label_)
+                    ) in enumerate(zip_smart(y.T, label)):
+                        _serialize_2d(
+                            serialize_pty=serialize_pty,
+                            serialize_mpl=serialize_mpl,
+                        )(core)(
+                            self,
+                            x,
+                            y_,
+                            label=label_,
+                            _serial_i=i,
+                            _serial_n=y.shape[1],
+                            **kwargs,
+                        )
+                    return
 
-        return core(self, x, y, label=label, **kwargs)
+            return core(self, x, y, label=label, **kwargs)
 
-    return wrapper
+        return wrapper
+
+    return decorator
 
 
 def _serialize_save(core):
     """Decorator to serialise saving multiple figures."""
 
     @wraps(core)
     def wrapper(self, path, export_format=None, **kwargs):
@@ -745,28 +561,28 @@
     Parameters
     ----------
     """
     __doc__ = _rewrite_docstring(__doc__)
 
     def __init__(
         self,
-        interactive=True,
+        interactive=None,
         rows=1,
         cols=1,
         title=None,
         xlabel=None,
         ylabel=None,
         xlim=None,
         ylim=None,
         shared_xaxes=False,
         shared_yaxes=False,
         column_widths=None,
         row_heights=None,
         fig_size=None,
-        dpi=100,
+        dpi=None,
         legend_loc=None,
         legend_title=None,
         save_fig=None,
         save_format=None,
         save_config=None,
         pty_update_layout=None,
         pty_custom_func=None,
@@ -774,37 +590,46 @@
     ):
         # input verification
         if shared_xaxes == "cols":
             shared_xaxes = "columns"
         if shared_yaxes == "cols":
             shared_yaxes = "columns"
 
-        self.interactive = interactive
+        self.interactive = (
+            conf.INTERACTIVE
+            if interactive is None
+            else interactive
+        )
         self.rows = rows
         self.cols = cols
         self.title = title
         self.xlabel = xlabel
         self.ylabel = ylabel
         self.xlim = xlim
         self.ylim = ylim
         self.legend_loc = legend_loc
         self.legend_title = legend_title
-        self.dpi = dpi
+        self.dpi = conf.DPI if dpi is None else dpi
         self.save_fig = save_fig
         self.save_format = save_format
         self.save_config = save_config
         self.pty_update_layout = pty_update_layout
         self.pty_custom_func = pty_custom_func
         self.mpl_custom_func = mpl_custom_func
         self.element_count = np.zeros((rows, cols), dtype=int)
         self.i_color = 0
 
         # init plotly
         if self.interactive:
             self.title = self._encode_html(self.title)
+            self.fig_size = (
+                conf.PTY_FIG_SIZE
+                if fig_size is None
+                else fig_size
+            )
 
             # init fig
             figure = go.Figure(
                 layout=go.Layout(legend={'traceorder': 'normal'}),
             )
             self.fig = sp.make_subplots(
                 rows=rows,
@@ -813,15 +638,15 @@
                 shared_yaxes=shared_yaxes,
                 row_heights=row_heights,
                 column_widths=column_widths,
                 figure=figure,
             )
 
             # unpacking
-            width, height = fig_size if fig_size is not None else (None, None)
+            width, height = self.fig_size
             if isinstance(legend_title, ITERABLE_TYPES):
                 warn(
                     "Plotly only has one legend, however multiple legend_"
                     "titles were provided. Only the first one will be used!"
                 )
                 legend_title = legend_title[0]
                 if isinstance(legend_title, ITERABLE_TYPES):
@@ -829,15 +654,15 @@
 
             # update layout
             self.fig.update_layout(
                 title=self.title,
                 legend_title=legend_title,
                 height=height,
                 width=width,
-                barmode="overlay",
+                barmode="group",
             )
 
             # axis limits
             for i_row, xlim_row, ylim_row in zip_smart(
                 range(1, self.rows + 1),
                 filter_nozip(self.xlim),
                 filter_nozip(self.ylim),
@@ -874,22 +699,30 @@
 
         # init matplotlib
         else:
             gridspec_kw = dict(
                 width_ratios=column_widths,
                 height_ratios=row_heights,
             )
-            if fig_size is not None:
-                px = 1 / dpi
-                fig_size = (fig_size[0] * px, fig_size[1] * px)
+
+            # convert px to inches
+            self.fig_size = (
+                conf.MPL_FIG_SIZE
+                if fig_size is None
+                else fig_size
+            )
+            px = 1 / self.dpi
+            figsize = (self.fig_size[0] * px, self.fig_size[1] * px)
+
+            # init fig
             self.fig, self.ax = plt.subplots(
                 rows,
                 cols,
-                figsize=fig_size,
-                dpi=dpi,
+                figsize=figsize,
+                dpi=self.dpi,
                 squeeze=False,
                 gridspec_kw=gridspec_kw,
             )
 
             # title
             if self.cols == 1:
                 self.ax[0, 0].set_title(self.title)
@@ -939,14 +772,32 @@
             ):
                 for text, i_row in zip_smart(self.ylabel, range(self.rows)):
                     self.ax[i_row, 0].set_ylabel(text)
             else:
                 self.fig.supylabel(self.ylabel)
 
     @staticmethod
+    def init(fig, *args, **kwargs):
+        """
+        Initialize a Plot instance, if not already initialized.
+
+        Parameters
+        ----------
+        fig: Plot or any
+            If fig is a Plot instance, return it.
+            Otherwise, create a new Plot instance.
+        *args, **kwargs: any
+            Passed to Plot constructor.
+        """
+        if isinstance(fig, Plot):
+            return fig
+        else:
+            return Plot(*args, **kwargs)
+
+    @staticmethod
     def _get_plotly_legend_args(label, default_label=None, show_legend=None):
         """
         Return keyword arguments for label configuration.
 
         Parameters
         ----------
         label: str
@@ -1021,21 +872,21 @@
 
         Returns
         -------
         color: str
             HEX color, with leading hashtag
         """
         if i is None:
-            if self.i_color >= len(COLOR_CYCLE):
+            if self.i_color >= len(conf.COLOR_CYCLE):
                 self.i_color = 0
-            color = COLOR_CYCLE[self.i_color]
+            color = conf.COLOR_CYCLE[self.i_color]
             self.i_color += increment
             return color
         else:
-            return COLOR_CYCLE[i]
+            return conf.COLOR_CYCLE[i]
 
     def digest_color(self, color=None, alpha=None, increment=1):
         """
         Parse color with matplotlib.colors to a rgba array.
 
         Parameters
         ----------
@@ -1052,15 +903,15 @@
         """
         # if color undefined, cycle COLOR_CYCLE
         if color is None:
             color = self.get_cycle_color(increment)
 
         # get index from COLOR_CYCLE
         elif color[0] == "C" or color[0] == "c":
-            color = COLOR_CYCLE[int(color[1:])]
+            color = conf.COLOR_CYCLE[int(color[1:])]
 
         rgba = list(mcolors.to_rgba(color))
         if alpha is not None:
             rgba[3] = alpha
 
         # PLOTLY
         if self.interactive:
@@ -1122,32 +973,32 @@
                 recursive=True,
             )
 
         if "markers" not in mode:
             return None
 
         if isinstance(marker, (int, np.integer)):
-            marker = PTY_MARKERS_LIST[marker]
+            marker = conf.PTY_MARKERS_LIST[marker]
 
         if marker is None:
-            marker = PTY_MARKERS_LIST[0]
+            marker = conf.PTY_MARKERS_LIST[0]
 
         if interactive:
-            if marker not in PTY_MARKERS_LIST:
-                marker = PTY_MARKERS.get(marker, marker)
+            if marker not in conf.PTY_MARKERS_LIST:
+                marker = conf.PTY_MARKERS.get(marker, marker)
             if recursive:
                 return marker
             return dict(
                 symbol=marker,
                 **pty_marker_kwargs,
             )
 
-        return MPL_MARKERS.get(marker, marker)
+        return conf.MPL_MARKERS.get(marker, marker)
 
-    @_serialize_2d
+    @_serialize_2d()
     def add_line(
         self,
         x,
         y=None,
         x_error=None,
         y_error=None,
         mode=None,
@@ -1159,14 +1010,16 @@
         label=None,
         show_legend=None,
         color=None,
         opacity=None,
         linewidth=None,
         row=0,
         col=0,
+        _serial_i=0,
+        _serial_n=1,
         pty_marker_kwargs=None,
         kwargs_pty=None,
         kwargs_mpl=None,
         **kwargs,
     ):
         """
         Draw a line or scatter plot.
@@ -1313,15 +1166,15 @@
                     **self._get_plotly_legend_args(
                         label,
                         show_legend=show_legend,
                     ),
                     marker_color=color,
                     line=dict(
                         width=linewidth,
-                        dash=PTY_LINE_STYLES.get(line_style, line_style),
+                        dash=conf.PTY_LINE_STYLES.get(line_style, line_style),
                     ),
                     **kwargs_pty,
                     **kwargs,
                 ),
                 row=row,
                 col=col,
             )
@@ -1335,15 +1188,15 @@
                 y,
                 xerr=x_error,
                 yerr=y_error,
                 label=None if show_legend is False else label,
                 color=color,
                 lw=linewidth,
                 linestyle=(
-                    MPL_LINE_STYLES.get(line_style, line_style)
+                    conf.MPL_LINE_STYLES.get(line_style, line_style)
                     if "lines" in mode
                     else "None"
                 ),
                 marker=self.digest_marker(
                     marker,
                     mode,
                     interactive=self.interactive,
@@ -1381,14 +1234,161 @@
     ):
         self.add_line(
             *args,
             mode=mode,
             **kwargs,
         )
 
+    @_serialize_2d()
+    def add_bar(
+        self,
+        x,
+        y=None,
+        horizontal=False,
+        width=0.8,
+        label=None,
+        show_legend=None,
+        color=None,
+        opacity=None,
+        line_width=1,
+        line_color=None,
+        row=0,
+        col=0,
+        _serial_i=0,
+        _serial_n=1,
+        kwargs_pty=None,
+        kwargs_mpl=None,
+        **kwargs,
+    ):
+        """
+        Draw a bar plot.
+
+        Parameters
+        ----------
+        x: array-like
+        y: array-like, optional
+            If only either `x` or `y` is defined, it will be assumed
+            as the size of the bar, regardless whether it's horizontal
+            or vertical.
+            If both `x` and `y` are defined, `x` will be taken as the
+            position of the bar, and `y` as the size, regardless of
+            the orientation.
+            If a pandas `Series` is provided, the index will
+            be taken as the position.
+            Else if a pandas `DataFrame` is provided, the method call
+            is looped for each column.
+            If a 2D numpy `array` is provided, the method call
+            is looped for each column, with the index as the position.
+        horizontal: bool, optional
+            If True, the bars are drawn horizontally. Default is False.
+        width: float, optional
+            Relative width of the bar. Must be in the range (0, 1).
+        label: str, optional
+            Trace label for legend.
+        show_legend: bool, optional
+            Whether to show the label in the legend.
+
+            By default, it will be shown if a label is defined.
+        color: str, optional
+            Trace color.
+
+            Can be hex, rgb(a) or any named color that is understood
+            by matplotlib.
+
+            Default: color is retrieved from `Plot.digest_color`,
+            which cycles through `COLOR_CYCLE`.
+        opacity: float, optional
+            Opacity (=alpha) of the fill.
+
+            By default, fallback to alpha value provided with color argument,
+            or 1.
+        line_width: float, optional
+            The width of the bar outline. Default is 1.
+        line_color: str, optional
+            The color of the bar outline. This can be a named color or a tuple
+            specifying the RGB values.
+
+            By default, the same color as the fill is used.
+        row, col: int, optional
+            If the plot contains a grid, provide the coordinates.
+
+            Attention: Indexing starts with 0!
+        kwargs_pty, kwargs_mpl, **kwargs: optional
+            Pass specific keyword arguments to the line core method.
+        """
+        self.element_count[row, col] += 1
+        # PLOTLY
+        if self.interactive:
+            if kwargs_pty is None:
+                kwargs_pty = dict()
+
+            if horizontal:
+                x, y = y, x
+
+            row += 1
+            col += 1
+            self.fig.add_trace(
+                go.Bar(
+                    x=x,
+                    y=y,
+                    orientation="h" if horizontal else "v",
+                    **self._get_plotly_legend_args(
+                        label,
+                        show_legend=show_legend,
+                    ),
+                    marker_color=self.digest_color(color, opacity),
+                    marker=dict(
+                        line=dict(
+                            width=0 if line_color is None else line_width,
+                            color=(
+                                color
+                                if line_color is None
+                                else self.digest_color(line_color, 1)
+                            ),
+                        ),
+                    ),
+                    **kwargs_pty,
+                    **kwargs,
+                ),
+                row=row,
+                col=col,
+            )
+
+        else:
+            if kwargs_mpl is None:
+                kwargs_mpl = dict()
+            offset = ((2*_serial_i + 1) / 2 / _serial_n - 0.5) * width
+            (
+                self.ax[row, col].barh
+                if horizontal
+                else self.ax[row, col].bar
+            )(
+                np.arange(len(x)) + offset,
+                y,
+                (width / _serial_n),
+                color=self.digest_color(color, opacity),
+                edgecolor=(
+                    self.digest_color(line_color, 1)
+                    if line_color is not None
+                    else None
+                ),
+                linewidth=line_width,
+                label=None if show_legend is False else label,
+                **kwargs_mpl,
+                **kwargs,
+            )
+            (
+                self.ax[row, col].set_yticks
+                if horizontal
+                else self.ax[row, col].set_xticks
+            )(
+                np.arange(len(x)),
+                x,
+            )
+
     def add_hist(
         self,
         x=None,
         y=None,
         bins=None,
         density=False,
         label=None,
@@ -2204,30 +2204,30 @@
         if path.is_dir():
             filename = self.title
             if filename is None or str(filename) == "":
                 filename = "interplot_figure"
             else:
                 filename = str(filename)
 
-            for key, value in EXPORT_REPLACE.items():
+            for key, value in conf.EXPORT_REPLACE.items():
                 filename = re.sub(key, value, filename)
             filename += "." + (
-                EXPORT_FORMAT if export_format is None else export_format
+                conf.EXPORT_FORMAT if export_format is None else export_format
             )
             path = path / filename
 
         # PLOTLY
         if self.interactive:
 
             # HTML
             if str(path)[-5:] == ".html":
                 self.fig.write_html(
                     path,
                     config=(
-                        PTY_CONFIG
+                        conf.PTY_CONFIG
                         if self.save_config is None
                         else self.save_config
                     ),
                     **kwargs,
                 )
 
             # image
@@ -2251,36 +2251,58 @@
         if print_confirm:
             print("saved figure at {}".format(str(path)))
 
         return path
 
     def show(self):
         """Show the plot."""
+        if CALLED_FROM_NOTEBOOK:
+            if self.interactive:
+                init_notebook_mode()
+                display_html(self.JS_RENDER_WARNING, raw=True)
+                return self.fig.show(
+                    config=(
+                        conf.PTY_CONFIG
+                        if self.save_config is None
+                        else self.save_config
+                    )
+                )
+            display_png(self._repr_png_(), raw=True)
+            return
+
         if self.interactive:
-            init_notebook_mode()
-            display_html(self.JS_RENDER_WARNING, raw=True)
             return self.fig.show(
-                config=PTY_CONFIG
-                if self.save_config is None
-                else self.save_config
+                config=(
+                    conf.PTY_CONFIG
+                    if self.save_config is None
+                    else self.save_config
+                )
             )
         return self.fig.show()
 
     def _repr_mimebundle_(self, *args, **kwargs):
         if self.interactive:
             return self.fig._repr_mimebundle_(*args, **kwargs)
 
         else:
             raise NotImplementedError
 
     def _repr_html_(self):
         if self.interactive:
             init_notebook_mode()
             return self.JS_RENDER_WARNING + self.fig._repr_html_()
-        return self.fig.show()
+        raise NotImplementedError
+
+    def _repr_png_(self):
+        if self.interactive:
+            raise NotImplementedError
+        bio = BytesIO()
+        self.fig.savefig(bio, format="png")
+        bio.seek(0)
+        return bio.read()
 
 
 def magic_plot(core, doc_decorator=None):
     """
     Plot generator wrapper.
 
     Your function feeds the data, the wrapper gives control over the plot
@@ -2300,88 +2322,88 @@
     [matplotlib figure, "Plot title"]
 
     Parameters
     ----------
     doc_decorator: str, optional
         Append the docstring with the decorated parameters.
 
-        By default, the global variable `DOCSTRING_DECORATOR` will be used.
+        By default, the global variable `_DOCSTRING_DECORATOR` will be used.
     """
     doc_decorator = (
-        DOCSTRING_DECORATOR
+        conf._DOCSTRING_DECORATOR
         if doc_decorator is None
         else doc_decorator
     )
 
     def wrapper(
         *args,
-        interactive=True,
+        interactive=None,
         rows=1,
         cols=1,
         fig=None,
         skip_post_process=False,
         title=None,
         xlabel=None,
         ylabel=None,
         xlim=None,
         ylim=None,
         shared_xaxes=False,
         shared_yaxes=False,
         column_widths=None,
         row_heights=None,
         fig_size=None,
-        dpi=100,
+        dpi=None,
         legend_loc=None,
         legend_title=None,
         save_fig=None,
         save_format=None,
         save_config=None,
         pty_update_layout=None,
         pty_custom_func=None,
         mpl_custom_func=None,
         **kwargs,
     ):
         # init Plot
-        if fig is None:
-            fig = Plot(
-                interactive=interactive,
-                rows=rows,
-                cols=cols,
-                title=title,
-                xlabel=xlabel,
-                ylabel=ylabel,
-                xlim=xlim,
-                ylim=ylim,
-                shared_xaxes=shared_xaxes,
-                shared_yaxes=shared_yaxes,
-                column_widths=column_widths,
-                row_heights=row_heights,
-                fig_size=fig_size,
-                dpi=dpi,
-                legend_loc=legend_loc,
-                legend_title=legend_title,
-                save_fig=save_fig,
-                save_format=save_format,
-                save_config=save_config,
-                pty_update_layout=pty_update_layout,
-                pty_custom_func=pty_custom_func,
-                mpl_custom_func=mpl_custom_func,
-            )
+        fig = Plot.init(
+            fig,
+            interactive=interactive,
+            rows=rows,
+            cols=cols,
+            title=title,
+            xlabel=xlabel,
+            ylabel=ylabel,
+            xlim=xlim,
+            ylim=ylim,
+            shared_xaxes=shared_xaxes,
+            shared_yaxes=shared_yaxes,
+            column_widths=column_widths,
+            row_heights=row_heights,
+            fig_size=fig_size,
+            dpi=dpi,
+            legend_loc=legend_loc,
+            legend_title=legend_title,
+            save_fig=save_fig,
+            save_format=save_format,
+            save_config=save_config,
+            pty_update_layout=pty_update_layout,
+            pty_custom_func=pty_custom_func,
+            mpl_custom_func=mpl_custom_func,
+        )
 
         # execute core method
         core(*args, fig=fig, **kwargs)
 
         # post-processing
         if not skip_post_process:
             fig.post_process()
 
         # return
         return fig
 
-    # rewrite DOCSTRING_DECORATOR
+    # rewrite _DOCSTRING_DECORATOR
     wrapper.__doc__ = _rewrite_docstring(
         core.__doc__,
         doc_decorator,
     ) + "\n"
 
     return wrapper
 
@@ -2411,15 +2433,16 @@
     [matplotlib figure, "Data view"]
 
     Parameters
     ----------
     doc_decorator: str, optional
         Append the docstring with the decorated parameters.
 
-        By default, the global variable `DOCSTRING_DECORATOR` will be used.
+        By default, the global variable `conf._DOCSTRING_DECORATOR`
+        will be used.
     **kwargs_preset: dict
         Define presets for any keyword arguments accepted by `Plot`.
 
         Setting `strict_preset=True` prevents overriding the preset.
     """
     strict_preset = kwargs_preset.get("strict_preset", False)
     if "strict_preset" in kwargs_preset:
@@ -2489,14 +2512,24 @@
     fig,
     **kwargs,
 ):
     fig.add_linescatter(*args, **kwargs)
 
 
 @magic_plot
+@wraps(Plot.add_bar)
+def bar(
+    *args,
+    fig,
+    **kwargs,
+):
+    fig.add_bar(*args, **kwargs)
+
+
+@magic_plot
 @wraps(Plot.add_fill)
 def fill(
     *args,
     fig,
     **kwargs,
 ):
     fig.add_fill(*args, **kwargs)
```

### Comparing `interplot-0.1.1/interplot.egg-info/.DS_Store` & `interplot-0.1.2/interplot.egg-info/.DS_Store`

 * *Files identical despite different names*

### Comparing `interplot-0.1.1/interplot.egg-info/PKG-INFO` & `interplot-0.1.2/interplot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: interplot
-Version: 0.1.1
-Summary: Create matplotlib/plotly hybrid plots with a few lines of code.
+Version: 0.1.2
+Summary: Create matplotlib and plotly charts with the same few lines of code.
 Home-page: https://github.com/janjoch/interplot
 Author: Janosch Jörg
 Author-email: janjo@duck.com
 License: GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,26 +23,30 @@
 Requires-Dist: matplotlib
 Requires-Dist: plotly
 Requires-Dist: kaleido
 Requires-Dist: scipy
 Requires-Dist: xarray
 
 # interplot
-Create `matplotlib/plotly` hybrid plots with a few lines of code.
 
-It combines the best of the `matplotlib` and the `plotly` worlds through
-a unified, flat API.
-All the necessary boilerplate code is contained in this module.
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/janjoch/interplot/HEAD) [![NBViewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/janjoch/interplot/tree/main/)
+
+Create `matplotlib` and `plotly` charts with the same few lines of code.
+
+It combines the best of the `matplotlib` and the `plotly` worlds through a unified, flat API.
+
+Switch between `matplotlib` and `plotly` with the single keyword `interactive`. All the necessary boilerplate code to translate between the packages is contained in this module.
 
 Currently supported building blocks:
 
 - scatter plots
     - `line`
     - `scatter`
     - `linescatter`
+- bar charts `bar`
 - histogram `hist`
 - boxplot `boxplot`
 - heatmap `heatmap`
 - linear regression `regression`
 - line fill `fill`
 - annotations `text`
 
@@ -123,14 +127,15 @@
         saved figure at export/path/file.html
         ```
 
 
 ## Resources
 
 - **Documentation:** https://interplot.janjo.ch
+- **Demo Notebooks:** https://nbviewer.org/github/janjoch/interplot/tree/main/demo/
 - **Source Code:** https://github.com/janjoch/interplot
 - **PyPI:** https://pypi.org/project/interplot/
 
 
 ## Licence
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
@@ -149,7 +154,12 @@
 ```pip install interplot```
 
 
 ### dev installation
 1. ```git clone https://github.com/janjoch/interplot```
 2. ```cd interplot```
 2. ```pip install -e .```
+
+
+## Contribute
+
+Ideas, bug reports/fixes, feature requests and code submissions are very welcome! Please write to [janjo@duck.com](mailto:janjo@duck.com) or directly into a pull request.
```

### Comparing `interplot-0.1.1/setup.py` & `interplot-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='interplot',
-    version='0.1.1',
+    version='0.1.2',
     description=(
-        "Create matplotlib/plotly hybrid plots with a few lines of code."
+        "Create matplotlib and plotly charts with the same few lines of code."
     ),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/janjoch/interplot',
     author='Janosch Jörg',
     author_email='janjo@duck.com',
     license='GPL v3',
```

