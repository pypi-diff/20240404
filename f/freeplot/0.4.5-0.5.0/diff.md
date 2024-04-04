# Comparing `tmp/freeplot-0.4.5.tar.gz` & `tmp/freeplot-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplot-0.4.5.tar", last modified: Tue Jan 23 01:59:42 2024, max compression
+gzip compressed data, was "freeplot-0.5.0.tar", last modified: Thu Apr  4 06:00:02 2024, max compression
```

## Comparing `freeplot-0.4.5.tar` & `freeplot-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-23 01:59:42.817245 freeplot-0.4.5/
--rw-rw-rw-   0        0        0     1085 2022-09-19 12:06:04.000000 freeplot-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     7420 2024-01-23 01:59:42.816250 freeplot-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     6937 2023-01-01 10:56:12.000000 freeplot-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-01-23 01:59:42.781244 freeplot-0.4.5/freeplot/
--rw-rw-rw-   0        0        0       51 2024-01-23 01:56:59.000000 freeplot-0.4.5/freeplot/__init__.py
--rw-rw-rw-   0        0        0    19638 2023-06-08 06:46:33.000000 freeplot-0.4.5/freeplot/base.py
--rw-rw-rw-   0        0        0     3706 2023-06-08 06:41:05.000000 freeplot-0.4.5/freeplot/config.py
--rw-rw-rw-   0        0        0    25390 2023-12-16 05:54:14.000000 freeplot-0.4.5/freeplot/unit.py
--rw-rw-rw-   0        0        0     2300 2023-11-15 02:10:21.000000 freeplot-0.4.5/freeplot/utils.py
--rw-rw-rw-   0        0        0     6226 2022-09-19 12:06:04.000000 freeplot-0.4.5/freeplot/zoo.py
-drwxrwxrwx   0        0        0        0 2024-01-23 01:59:42.814244 freeplot-0.4.5/freeplot.egg-info/
--rw-rw-rw-   0        0        0     7420 2024-01-23 01:59:42.000000 freeplot-0.4.5/freeplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-01-23 01:59:42.000000 freeplot-0.4.5/freeplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-23 01:59:42.000000 freeplot-0.4.5/freeplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-01-23 01:59:42.000000 freeplot-0.4.5/freeplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-23 01:59:42.000000 freeplot-0.4.5/freeplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-23 01:59:42.817245 freeplot-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1059 2024-01-23 01:56:20.000000 freeplot-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:00:02.317693 freeplot-0.5.0/
+-rw-rw-rw-   0        0        0     1085 2022-09-19 12:06:04.000000 freeplot-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     7456 2024-04-04 06:00:02.316693 freeplot-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6937 2023-01-01 10:56:12.000000 freeplot-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 06:00:02.291697 freeplot-0.5.0/freeplot/
+-rw-rw-rw-   0        0        0       51 2024-04-04 05:58:44.000000 freeplot-0.5.0/freeplot/__init__.py
+-rw-rw-rw-   0        0        0    19617 2024-04-04 05:57:42.000000 freeplot-0.5.0/freeplot/base.py
+-rw-rw-rw-   0        0        0     3632 2024-04-04 05:56:26.000000 freeplot-0.5.0/freeplot/config.py
+-rw-rw-rw-   0        0        0    25384 2024-04-04 05:57:22.000000 freeplot-0.5.0/freeplot/unit.py
+-rw-rw-rw-   0        0        0     2298 2024-04-04 05:57:00.000000 freeplot-0.5.0/freeplot/utils.py
+-rw-rw-rw-   0        0        0     6224 2024-04-04 05:56:45.000000 freeplot-0.5.0/freeplot/zoo.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:00:02.314695 freeplot-0.5.0/freeplot.egg-info/
+-rw-rw-rw-   0        0        0     7456 2024-04-04 06:00:02.000000 freeplot-0.5.0/freeplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-04 06:00:02.000000 freeplot-0.5.0/freeplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 06:00:02.000000 freeplot-0.5.0/freeplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-04 06:00:02.000000 freeplot-0.5.0/freeplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-04 06:00:02.000000 freeplot-0.5.0/freeplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 06:00:02.317693 freeplot-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2024-01-23 01:56:20.000000 freeplot-0.5.0/setup.py
```

### Comparing `freeplot-0.4.5/LICENSE` & `freeplot-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeplot-0.4.5/PKG-INFO` & `freeplot-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: freeplot
-Version: 0.4.5
+Version: 0.5.0
 Summary: a Python data visualization library based on matplotlib
 Home-page: https://github.com/MTandHJ/freeplot
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: SciencePlots==1.0.9
 
 
 
 
 FreePlot is a Python data visualization library based on Matplotlib. It provides some simple implementations according to my preference. 
 Matplotlib is powerful yet not easy to draw what you want due to its complicated arguments. 
 I feel FreePlot is more friendly, especially for papers.
```

### Comparing `freeplot-0.4.5/README.md` & `freeplot-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `freeplot-0.4.5/freeplot/base.py` & `freeplot-0.5.0/freeplot/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 
 
 from typing import Iterable, Tuple, Optional, Dict, Union
 import numpy as np
 import pandas as pd 
 import seaborn as sns
-import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import patches
 
 from .unit import UnitPlot
 from .utils import style_env
 
  
-
 class FreePlot(UnitPlot):
 
 
     @style_env
     def barplot(
         self, x: str, y: str, 
         data: pd.DataFrame, hue: Optional[str] = None,
```

### Comparing `freeplot-0.4.5/freeplot/config.py` & `freeplot-0.5.0/freeplot/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,19 +165,19 @@
 
 style_cfg = Config()
 
 style_cfg['basic'] = ["science"]  # color style: bright, vibrant, muted, high-contrast, light, high-vis, retro
 style_cfg['line'] = [] 
 style_cfg['stack'] = [] 
 style_cfg['scatter'] = []
-style_cfg['heatmap'] = ["seaborn-darkgrid", {"axes.facecolor":".9"}]
+style_cfg['heatmap'] = []
 style_cfg['image'] = ["bright"]
 style_cfg['bar'] = [{'lines.markersize': 0.0, 'lines.markeredgewidth': 0., "lines.linewidth": 0.7}]
 style_cfg['hist'] = []
-style_cfg['violin'] = ["high-vis", "seaborn-whitegrid"]
+style_cfg['violin'] = []
 style_cfg['surface'] = [{"axes.facecolor":".3"}]
 
 # zoo
 style_cfg['radar'] = []
```

### Comparing `freeplot-0.4.5/freeplot/unit.py` & `freeplot-0.5.0/freeplot/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from matplotlib.axes._axes import Axes
 from mpl_toolkits.mplot3d.axes3d import Axes3D
 
 from .config import cfg, style_cfg, COLORS
 from .utils import inherit_from_matplotlib, get_style, style_env
 
 
-
 class UnitAX:
     """Single Axes.
     """
 
     def __init__(
         self, axes: 'FreeAxes', 
         position: matplotlib.gridspec.GridSpec, 
@@ -755,9 +754,8 @@
             - `Axes`: return `Axes`
         
         Returns:
         ---
 
         Axes, Axes3D
         """
-        return self.axes[idx]
-
+        return self.axes[idx]
```

### Comparing `freeplot-0.4.5/freeplot/utils.py` & `freeplot-0.5.0/freeplot/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict, Iterable, Any, NoReturn
 import json
 import inspect
 import pickle
 import matplotlib.pyplot as plt
 from .config import style_cfg
 
+
 def load(filename: str) -> Dict:
     with open(filename, encoding="utf-8") as j:
         data = json.load(j)
     return data
 
 def export_pickle(data: Any, file_: str) -> NoReturn:
     fh = None
@@ -69,9 +70,8 @@
             for item in kwargs['style']:
                 style += get_style(item)
         with plt.style.context(style, after_reset=False):
             results = func(*arg, **kwargs)
         return results
     wrapper.__name__ = func.__name__
     wrapper.__doc__ = func.__doc__
-    return wrapper
-
+    return wrapper
```

### Comparing `freeplot-0.4.5/freeplot/zoo.py` & `freeplot-0.5.0/freeplot/zoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 from .base import *
 from .utils import style_env
 
 
-
 def tsne(
     features: np.ndarray, 
     labels: np.ndarray, 
     fp: FreePlot, 
     index: Union[Tuple[int], str] = (0, 0), 
     fontsize: Union[int, str] = 'large',
     annotate: bool = False,
```

### Comparing `freeplot-0.4.5/freeplot.egg-info/PKG-INFO` & `freeplot-0.5.0/freeplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: freeplot
-Version: 0.4.5
+Version: 0.5.0
 Summary: a Python data visualization library based on matplotlib
 Home-page: https://github.com/MTandHJ/freeplot
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: SciencePlots==1.0.9
 
 
 
 
 FreePlot is a Python data visualization library based on Matplotlib. It provides some simple implementations according to my preference. 
 Matplotlib is powerful yet not easy to draw what you want due to its complicated arguments. 
 I feel FreePlot is more friendly, especially for papers.
```

### Comparing `freeplot-0.4.5/setup.py` & `freeplot-0.5.0/setup.py`

 * *Files identical despite different names*

