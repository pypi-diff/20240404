# Comparing `tmp/tga_data_analysis-2.0.2.tar.gz` & `tmp/tga_data_analysis-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tga_data_analysis-2.0.2.tar", last modified: Mon Apr  1 21:33:36 2024, max compression
+gzip compressed data, was "tga_data_analysis-2.0.4.tar", last modified: Thu Apr  4 18:13:20 2024, max compression
```

## Comparing `tga_data_analysis-2.0.2.tar` & `tga_data_analysis-2.0.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 21:33:36.415410 tga_data_analysis-2.0.2/
--rw-rw-rw-   0        0        0     2012 2024-04-01 21:33:36.410220 tga_data_analysis-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.2/README.md
--rw-rw-rw-   0        0        0      783 2024-04-01 21:32:34.000000 tga_data_analysis-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 21:33:36.415410 tga_data_analysis-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 21:33:36.210608 tga_data_analysis-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 21:33:36.249486 tga_data_analysis-2.0.2/src/tga_data_analysis/
--rw-rw-rw-   0        0        0        2 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.2/src/tga_data_analysis/__init__.py
--rw-rw-rw-   0        0        0    11523 2024-04-01 21:21:22.000000 tga_data_analysis-2.0.2/src/tga_data_analysis/kas_kinetics.py
--rw-rw-rw-   0        0        0    22694 2024-04-01 21:13:57.000000 tga_data_analysis-2.0.2/src/tga_data_analysis/myfigure.py
--rw-rw-rw-   0        0        0    62881 2024-04-01 21:29:50.000000 tga_data_analysis-2.0.2/src/tga_data_analysis/tga.py
-drwxrwxrwx   0        0        0        0 2024-04-01 21:33:36.351858 tga_data_analysis-2.0.2/src/tga_data_analysis.egg-info/
--rw-rw-rw-   0        0        0     2012 2024-04-01 21:33:36.000000 tga_data_analysis-2.0.2/src/tga_data_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2024-04-01 21:33:36.000000 tga_data_analysis-2.0.2/src/tga_data_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 21:33:36.000000 tga_data_analysis-2.0.2/src/tga_data_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-04-01 21:33:36.000000 tga_data_analysis-2.0.2/src/tga_data_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-01 21:33:36.000000 tga_data_analysis-2.0.2/src/tga_data_analysis.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 21:33:36.345863 tga_data_analysis-2.0.2/tests/
--rw-rw-rw-   0        0        0     1855 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.2/tests/test_measure.py
--rw-rw-rw-   0        0        0       42 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.2/tests/test_sample.py
--rw-rw-rw-   0        0        0      911 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.2/tests/test_tga.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.240611 tga_data_analysis-2.0.4/
+-rw-rw-rw-   0        0        0     2012 2024-04-04 18:13:20.233645 tga_data_analysis-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.4/README.md
+-rw-rw-rw-   0        0        0      783 2024-04-04 18:13:10.000000 tga_data_analysis-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 18:13:20.242604 tga_data_analysis-2.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.133967 tga_data_analysis-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.167854 tga_data_analysis-2.0.4/src/tga_data_analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-03 01:21:24.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/__init__.py
+-rw-rw-rw-   0        0        0    10611 2024-04-02 13:30:00.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/kas_kinetics.py
+-rw-rw-rw-   0        0        0     4340 2024-04-03 01:44:48.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/measure.py
+-rw-rw-rw-   0        0        0    23737 2024-04-03 01:58:28.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/myfigure.py
+-rw-rw-rw-   0        0        0    64691 2024-04-04 02:03:14.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/tga.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.227654 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/
+-rw-rw-rw-   0        0        0     2012 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.221675 tga_data_analysis-2.0.4/tests/
+-rw-rw-rw-   0        0        0     1855 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.4/tests/test_measure.py
+-rw-rw-rw-   0        0        0     3964 2024-04-02 01:28:57.000000 tga_data_analysis-2.0.4/tests/test_my_figure.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.4/tests/test_sample.py
+-rw-rw-rw-   0        0        0      911 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.4/tests/test_tga.py
```

### Comparing `tga_data_analysis-2.0.2/PKG-INFO` & `tga_data_analysis-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tga_data_analysis
-Version: 2.0.2
+Version: 2.0.4
 Summary: Tool for automatic analysis of multiple TGA results
 Author: Matteo Pecchi
 License: MIT
 Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
 Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tga_data_analysis-2.0.2/README.md` & `tga_data_analysis-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.2/pyproject.toml` & `tga_data_analysis-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tga_data_analysis"
-version = "2.0.2"
+version = "2.0.4"
 authors = [
     { name = "Matteo Pecchi"}
 ]
 description = "Tool for automatic analysis of multiple TGA results"
 readme = "README.md"
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `tga_data_analysis-2.0.2/src/tga_data_analysis/kas_kinetics.py` & `tga_data_analysis-2.0.4/src/tga_data_analysis/kas_kinetics.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,42 @@
 import numpy as np
 import pathlib as plib
 from tga_data_analysis.tga import Project, Sample
 from tga_data_analysis.myfigure import MyFigure, clrs, lttrs, lnstls, mrkrs
 
 
 class KasSample:
+    """
+    A class to handle and analyze kinetic data using the Kissinger-Akahira-Sunose (KAS) method.
+    It provides functionalities to perform KAS analysis on a set of samples, plot analysis results,
+    and compare different samples' kinetic parameters.
+    """
 
     def __init__(
         self,
         project: Project,
         samples: list[Sample] | None = None,
         name: str | None = None,
         ramps: list[float] | None = None,
         alpha: list[float] | None = None,
     ):
+        """
+        Initialize a KasSample object with parameters for KAS analysis.
+
+        :param project: The Project object associated with the kinetic analysis.
+        :type project: Project
+        :param samples: A list of Sample objects to be analyzed. If None, all samples in the project are used.
+        :type samples: list[Sample], optional
+        :param name: An optional name for the KasSample object, used for identification.
+        :type name: str, optional
+        :param ramps: A list of heating rates for each sample. If None, the heating rates are taken from the samples.
+        :type ramps: list[float], optional
+        :param alpha: A list of conversion values to be analyzed. If None, a default range is used.
+        :type alpha: list[float], optional
+        """
         self.plot_grid = project.plot_grid
         self.plot_font = project.plot_font
         self.out_path = plib.Path(project.out_path, "kas_analysis")
         if samples is None:
             self.samples = project.samples
         else:
             self.samples = samples
@@ -51,23 +70,18 @@
 
         self.kas_analysis_computed: bool = False
 
     def kas_analysis(
         self,
     ):
         """
-        Perform KAS (Kissinger-Akahira-Sunose) analysis on a set of experiments.
+        Perform the KAS analysis across the provided samples, calculating the activation energy for different conversions.
 
-        Args:
-            samplenames (list[str]): List of sample names to analyze.
-            ramps (list[float]): List of ramp values used for each experiment.
-            alpha (list[float]): List of alpha values to investigate. Defaults to np.arange(0.05, .9, 0.05).
-
-        Returns:
-            dict: Results of the KAS analysis.
+        This method computes the activation energy for the given conversion values (alpha) using the KAS method.
+        The results are stored within the object for later access and visualization.
         """
 
         r_gas_constant = 8.314462618  # Universal gas constant in J/(mol*K)
         c_to_k = 273.15
 
         for idx, sample in enumerate(self.samples):
             temp = sample.temp_dtg + c_to_k if sample.temp_unit == "C" else sample.temp_dtg
@@ -90,31 +104,22 @@
         return None
 
     def plot_isolines(
         self,
         **kwargs,
     ) -> MyFigure:
         """
-        Plot isolines for KAS analysis.
+        Plot the KAS analysis isolines for the set of samples.
+
+        This method generates a plot of the KAS isolines, providing a visual representation of the kinetic analysis results.
 
-        Parameters:
-        - exps (list): List of experiments.
-        - kas_names (list, optional): List of names for each KAS analysis. If not provided, the names will be extracted from the KAS analysis data.
-        - filename (str, optional): Name of the output file. Default is 'KAsIso'.
-        - paper_col (float, optional): Width of the plot in inches. Default is 0.78.
-        - hgt_mltp (float, optional): Height multiplier for the plot. Default is 1.25.
-        - x_lim (tuple, optional): Limits for the x-axis. Default is None.
-        - y_lim (tuple, optional): Limits for the y-axis. Default is None.
-        - annt_names (bool, optional): Whether to annotate the names of the KAS analysis. Default is True.
-        - annotate_lttrs (bool, optional): Whether to annotate the letters for each KAS analysis. Default is False.
-        - leg_cols (int, optional): Number of columns in the legend. Default is 1.
-        - bboxtoanchor (bool, optional): Whether to place the legend outside of the plot area. Default is True.
-        - x_anchor (float, optional): X-coordinate for the legend anchor. Default is 1.13.
-        - y_anchor (float, optional): Y-coordinate for the legend anchor. Default is 1.02.
-        - legend_loc (str, optional): Location of the legend. Default is 'best'.
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the isoline plot.
+        :rtype: MyFigure
         """
 
         if not self.kas_analysis_computed:
             self.kas_analysis()
 
         out_path = plib.Path(self.out_path, "isolines_plots")
         out_path.mkdir(parents=True, exist_ok=True)
@@ -155,33 +160,23 @@
         return myfig
 
     def plot_activation_energy(
         self,
         **kwargs,
     ) -> MyFigure:
         """
-        Plot isolines for KAS analysis.
+        Plot the activation energy as a function of conversion for the analyzed samples.
 
-        Parameters:
-        - exps (list): List of experiments.
-        - kas_names (list, optional): List of names for each KAS analysis. If not provided, the names will be extracted from the KAS analysis data.
-        - filename (str, optional): Name of the output file. Default is 'KAsIso'.
-        - paper_col (float, optional): Width of the plot in inches. Default is 0.78.
-        - hgt_mltp (float, optional): Height multiplier for the plot. Default is 1.25.
-        - x_lim (tuple, optional): Limits for the x-axis. Default is None.
-        - y_lim (tuple, optional): Limits for the y-axis. Default is None.
-        - annt_names (bool, optional): Whether to annotate the names of the KAS analysis. Default is True.
-        - annotate_lttrs (bool, optional): Whether to annotate the letters for each KAS analysis. Default is False.
-        - leg_cols (int, optional): Number of columns in the legend. Default is 1.
-        - bboxtoanchor (bool, optional): Whether to place the legend outside of the plot area. Default is True.
-        - x_anchor (float, optional): X-coordinate for the legend anchor. Default is 1.13.
-        - y_anchor (float, optional): Y-coordinate for the legend anchor. Default is 1.02.
-        - legend_loc (str, optional): Location of the legend. Default is 'best'.
-        """
+        This method generates a plot showing the variation of activation energy with conversion, offering insights into the kinetic behavior of the sample.
 
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the activation energy plot.
+        :rtype: MyFigure
+        """
         if not self.kas_analysis_computed:
             self.kas_analysis()
 
         out_path = plib.Path(self.out_path, "activation_energy_plots")
         out_path.mkdir(parents=True, exist_ok=True)
 
         default_kwargs = {
@@ -215,30 +210,29 @@
 def plot_multi_activation_energy(
     kassamples: list[KasSample],
     labels: list[str] | None = None,
     filename: str = "plot",
     **kwargs,
 ) -> MyFigure:
     """
-    Plot multiple thermogravimetric (TG) curves.
+    Plot the activation energy for multiple KAS analyses, comparing their kinetic parameters.
 
-    Args:
-        exps (list): List of experimental data objects.
-        filename (str, optional): Name of the output file. Defaults to 'Fig'.
-        paper_col (float, optional): Width of the figure in inches. Defaults to 0.78.
-        hgt_mltp (float, optional): Height multiplier of the figure. Defaults to 1.25.
-        x_lim (tuple, optional): Limits of the x-axis. Defaults to None.
-        y_lim (list, optional): Limits of the y-axis. Defaults to [0, 100].
-        y_ticks (list, optional): Custom y-axis tick locations. Defaults to None.
-        lttrs (bool, optional): Whether to annotate letters on the plot. Defaults to False.
-        save_as_pdf (bool, optional): Whether to save the figure as a PDF file. Defaults to False.
-        save_as_svg (bool, optional): Whether to save the figure as an SVG file. Defaults to False.
+    This function creates a plot showing the activation energy against conversion for a series of KasSample objects,
+    allowing for a comparative analysis of different samples or conditions.
 
-    Returns:
-        None
+    :param kassamples: A list of KasSample objects for which the activation energy plots are generated.
+    :type kassamples: list[KasSample]
+    :param labels: Labels corresponding to each KasSample object. If None, the names of the samples are used.
+    :type labels: list[str], optional
+    :param filename: The base name for the file to save the plot. Defaults to "plot".
+    :type filename: str
+    :param kwargs: Additional keyword arguments for plot customization.
+    :type kwargs: dict
+    :return: A MyFigure instance containing the comparative activation energy plot.
+    :rtype: MyFigure
     """
 
     if labels is None:
         labels = [sample.name for sample in kassamples]
     for sample in kassamples:
         if not sample.kas_analysis_computed:
             sample.kas_analysis()
```

### Comparing `tga_data_analysis-2.0.2/src/tga_data_analysis/myfigure.py` & `tga_data_analysis-2.0.4/src/tga_data_analysis/myfigure.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import string
 import pathlib as plib
-from typing import Any, Dict, Literal
+from typing import Any, Dict
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes
 import seaborn as sns
 
@@ -118,83 +118,77 @@
 ]
 
 
 class MyFigure:
     """
     A class for creating and customizing figures using matplotlib and seaborn.
 
-    MyFigure provides a structured way to create figures with multiple subplots,
-    allowing for detailed customization of each subplot. It supports features like
-    adjusting axis limits, adding legends, annotating, and creating inset plots,
-    all with an emphasis on easy configurability through keyword arguments.
-
-    :ivar broad_props: A dictionary to store properties that are broadcasted across all axes.
+    :ivar broad_props: Properties applied to all axes.
     :type broad_props: dict
-    :ivar kwargs: A dictionary to store all the configuration keyword arguments.
+    :ivar kwargs: Configuration keyword arguments.
     :type kwargs: dict
     :ivar fig: The main figure object from matplotlib.
     :type fig: matplotlib.figure.Figure
-    :ivar axs: A list of axes objects corresponding to the subplots in the figure.
+    :ivar axs: Axes objects for the subplots.
     :type axs: list[matplotlib.axes.Axes]
-    :ivar axts: A list of twin axes objects if 'twinx' is enabled, otherwise None.
+    :ivar axts: Twin axes objects, if 'twinx' is enabled.
     :type axts: list[matplotlib.axes.Axes] or None
-    :ivar n_axs: The number of axes/subplots in the figure.
+    :ivar n_axs: Number of axes/subplots.
     :type n_axs: int
-
-    The class is designed to work seamlessly with seaborn's styling features,
-    making it suitable for creating publication-quality figures with minimal code.
     """
 
     @staticmethod
     def _adjust_lims(lims: tuple[float] | None, gap=0.05) -> tuple[float] | None:
         """
-        Adjusts the provided axis limits by a specified gap percentage to add padding
-        around the data.
+        Adjust axis limits with a specified gap.
 
-        :param lims: _description_
-        :type lims: tuple[float] | None
-        :param gap: _description_, defaults to 0.05
+        :param lims: Axis limits to adjust.
+        :type lims: tuple[float, float] | None
+        :param gap: Percentage gap to add to the limits.
         :type gap: float, optional
-        :return: _description_
-        :rtype: tuple[float] | None
+        :return: Adjusted axis limits.
+        :rtype: tuple[float, float] | None
         """
         if lims is None:
             return None
         else:
             new_lims = (
                 lims[0] * (1 + gap) - gap * lims[1],
                 lims[1] * (1 + gap) - gap * lims[0],
             )
             return new_lims
 
     def __init__(self, **kwargs: Any) -> None:
         """
-        Initializes a MyFigure object with custom or default settings for creating plots.
+        Initialize a MyFigure object with optional configuration.
 
-        :param kwargs: Keyword arguments to override default figure settings.
+        :param kwargs: Configuration options as keyword arguments.
+        :type kwargs: Any
         """
         self.broad_props: dict[str, list] = {}  # broadcasted properties for each axis
         self.kwargs = self.default_kwargs()
         self.kwargs.update(kwargs)  # Override defaults with any kwargs provided
         self.process_kwargs()
 
         sns.set_palette(self.kwargs["color_palette"], self.kwargs["color_palette_n_colors"])
         sns.set_style(self.kwargs["sns_style"], {"font.family": self.kwargs["text_font"]})
+        plt.rcParams.update({"font.size": self.kwargs["text_font_size"]})
 
         self.create_figure()
 
         self.update_axes_single_props()
 
         self.update_axes_list_props()
 
     def default_kwargs(self) -> Dict[str, Any]:
         """
-        Defines the default settings for the figure.
+        Define default keyword arguments for the figure.
 
-        :return: A dictionary of default settings.
+        :return: Default configuration settings.
+        :rtype: Dict[str, Any]
         """
         defaults = {
             "filename": None,
             "out_path": None,
             "rows": 1,
             "cols": 1,
             "width": 6.0,
@@ -221,40 +215,42 @@
             "annotate_lttrs": None,
             "annotate_lttrs_xy": None,
             "grid": None,
             "color_palette": "deep",
             "color_palette_n_colors": None,
             "text_font": "Dejavu Sans",
             "sns_style": "ticks",
+            "text_font_size": 10,
+            "legend_font_size": 10,
+            "x_labelpad": 0,
+            "y_labelpad": 0,
+            "legend_borderpad": 0.3,
+            "legend_handlelength": 1.5,
         }
         return defaults
 
     def process_kwargs(self) -> None:
         """
-        Validates and processes the provided keyword arguments for figure configuration.
+        Process and validate keyword arguments.
 
-
-        :raises ValueError: _description_
-        :raises ValueError: _description_
-        :raises ValueError: _description_
-        :raises ValueError: _description_
-        :raises ValueError: _description_
+        Raises a ValueError if an invalid keyword argument is provided.
         """
         valid_kwargs = set(self.default_kwargs().keys())
 
         # Check for any invalid keyword arguments
         for kwarg in self.kwargs:
             if kwarg not in valid_kwargs:
 
                 raise ValueError(f"Invalid keyword argument: '{kwarg}' \n {valid_kwargs = }")
         if self.kwargs["out_path"] is not None:
             self.kwargs["out_path"] = plib.Path(self.kwargs["out_path"])
         if self.kwargs["filename"] is not None:
             if not isinstance(self.kwargs["filename"], str):
                 raise ValueError("Filename must be a str.")
+
         self.kwargs["rows"] = int(self.kwargs["rows"])
         self.kwargs["cols"] = int(self.kwargs["cols"])
         self.kwargs["width"] = float(self.kwargs["width"])
         self.kwargs["height"] = float(self.kwargs["height"])
         self.kwargs["legend_ncols"] = int(self.kwargs["legend_ncols"])
 
         if self.kwargs["rows"] <= 0:
@@ -268,15 +264,15 @@
         if self.kwargs["legend_ncols"] <= 0:
             raise ValueError("Number of legend columns must be positive.")
 
     def create_figure(self) -> MyFigure:
         """
         Creates the figure and its axes.
 
-        :return: _description_
+        :return: MyFigure
         :rtype: MyFigure
         """
         self.fig: Figure
         self.axs: Axes
         self.axts: Axes | None
         self.fig, axes = plt.subplots(
             self.kwargs["rows"],
@@ -297,34 +293,37 @@
         filename: str | None = None,
         out_path: plib.Path | None = None,
         tight_layout: bool = True,
         save_as_png: bool = True,
         save_as_pdf: bool = False,
         save_as_svg: bool = False,
         save_as_eps: bool = False,
+        save_as_tif: bool = False,
         png_transparency: bool = False,
+        dpi: int = 300,
     ) -> None:
-        """_summary_
+        """
+        Save the figure to a file.
 
-        :param filename: _description_, defaults to "figure"
-        :type filename: str, optional
-        :param out_path: _description_, defaults to plib.Path(".")
-        :type out_path: plib.Path | None, optional
-        :param tight_layout: _description_, defaults to True
-        :type tight_layout: bool, optional
-        :param save_as_png: _description_, defaults to True
-        :type save_as_png: bool, optional
-        :param save_as_pdf: _description_, defaults to False
-        :type save_as_pdf: bool, optional
-        :param save_as_svg: _description_, defaults to False
-        :type save_as_svg: bool, optional
-        :param save_as_eps: _description_, defaults to False
-        :type save_as_eps: bool, optional
-        :param png_transparency: _description_, defaults to False
-        :type png_transparency: bool, optional
+        :param filename: The name of the file.
+        :type filename: str | None
+        :param out_path: The path to save the file.
+        :type out_path: pathlib.Path | None
+        :param tight_layout: Whether to use a tight layout.
+        :type tight_layout: bool
+        :param save_as_png: Save as PNG.
+        :type save_as_png: bool
+        :param save_as_pdf: Save as PDF.
+        :type save_as_pdf: bool
+        :param save_as_svg: Save as SVG.
+        :type save_as_svg: bool
+        :param save_as_eps: Save as EPS.
+        :type save_as_eps: bool
+        :param png_transparency: PNG transparency.
+        :type png_transparency: bool
         """
         self.update_axes_single_props()
 
         self.update_axes_list_props()
 
         self.apply_hatch_patterns()
 
@@ -339,32 +338,35 @@
         self.annotate_letters()
         # Saving the figure
         formats = {
             "png": save_as_png,
             "pdf": save_as_pdf,
             "svg": save_as_svg,
             "eps": save_as_eps,
+            "tif": save_as_tif,
         }
         if filename is None:
             filename = self.kwargs["filename"]
         if out_path is None:
             out_path = self.kwargs["out_path"]
 
         for fmt, should_save in formats.items():
             if should_save:
                 full_path = plib.Path(out_path, f"{filename}.{fmt}")
                 self.fig.savefig(
                     full_path,
-                    dpi=300,
+                    dpi=dpi,
                     transparent=png_transparency,
                     bbox_inches="tight" if tight_layout else None,
                 )
 
     def add_legend(self) -> None:
-        """_summary_"""
+        """
+        Add a legend to the figure.
+        """
         for sprop in ["legend", "legend_loc", "legend_ncols", "legend_title"]:
             self.broad_props[sprop] = self._broadcast_value_prop(self.kwargs[sprop], sprop)
         for lprop in ["legend_bbox_xy"]:
             self.broad_props[lprop] = self._broadcast_list_prop(self.kwargs[lprop], lprop)
 
         if self.kwargs["twinx"] is None:
 
@@ -375,14 +377,17 @@
                         ncol=self.broad_props["legend_ncols"][i],
                         title=self.broad_props["legend_title"][i],
                         bbox_to_anchor=(
                             self.broad_props["legend_bbox_xy"][i]
                             if self.broad_props["legend_bbox_xy"][i] is not None
                             else None
                         ),
+                        fontsize=self.kwargs["legend_font_size"],
+                        borderpad=self.kwargs["legend_borderpad"],
+                        handlelength=self.kwargs["legend_handlelength"],
                     )
 
         else:
             for i, (ax, axt) in enumerate(zip(self.axs, self.axts)):
                 if self.broad_props["legend"][i]:
                     hnd_ax, lab_ax = ax.get_legend_handles_labels()
                     hnd_axt, lab_axt = axt.get_legend_handles_labels()
@@ -393,18 +398,23 @@
                         ncol=self.broad_props["legend_ncols"][i],
                         title=self.broad_props["legend_title"][i],
                         bbox_to_anchor=(
                             self.broad_props["legend_bbox_xy"][i]
                             if self.broad_props["legend_bbox_xy"][i] is not None
                             else None
                         ),
+                        fontsize=self.kwargs["legend_font_size"],
+                        borderpad=self.kwargs["legend_borderpad"],
+                        handlelength=self.kwargs["legend_handlelength"],
                     )
 
     def annotate_letters(self) -> None:
-        """_summary_"""
+        """
+        Annotate the subplots with letters.
+        """
         if (
             self.kwargs["annotate_lttrs_xy"] is not None
             and isinstance(self.kwargs["annotate_lttrs_xy"], (list, tuple))
             and len(self.kwargs["annotate_lttrs_xy"]) >= 2
         ):
             xylttrs: list | tuple = self.kwargs["annotate_lttrs_xy"]
             x_lttrs = xylttrs[0]  # pylint: disable=unsubscriptable-object
@@ -413,78 +423,85 @@
             x_lttrs = -0.15
             y_lttrs = -0.15
         if self.kwargs["annotate_lttrs"] is not None:
             if isinstance(self.kwargs["annotate_lttrs"], str):
                 letters_list = [self.kwargs["annotate_lttrs"]]
             elif isinstance(self.kwargs["annotate_lttrs"], (list, tuple)):
                 letters_list = self.kwargs["annotate_lttrs"]
+            else:
+                raise ValueError("annotate_lttrs is given in the wrong format")
             for i, ax in enumerate(self.axs):
                 ax.annotate(
                     f"({letters_list[i]})",
                     xycoords="axes fraction",
                     xy=(0, 0),
                     xytext=(x_lttrs, y_lttrs),
-                    size="large",
+                    size=self.kwargs["text_font_size"],
                     weight="bold",
                 )
 
     def create_inset(
         self,
         ax: Axes,
         ins_x_loc: tuple[float],
         ins_y_loc: tuple[float],
         ins_x_lim: tuple[float] | None = None,
         ins_y_lim: tuple[float] | None = None,
     ) -> Axes:
-        """_summary_
+        """
+        Create an inset plot within an existing axis.
 
-        :param ax: _description_
+        :param ax: The parent axis.
         :type ax: Axes
-        :param ins_x_loc: _description_
-        :type ins_x_loc: tuple[float]
-        :param ins_y_loc: _description_
-        :type ins_y_loc: tuple[float]
-        :param ins_x_lim: _description_
-        :type ins_x_lim: tuple[float]
-        :param ins_y_lim: _description_
-        :type ins_y_lim: tuple[float]
-        :return: _description_
+        :param ins_x_loc: X location for the inset.
+        :type ins_x_loc: tuple[float, float]
+        :param ins_y_loc: Y location for the inset.
+        :type ins_y_loc: tuple[float, float]
+        :param ins_x_lim: X limits for the inset.
+        :type ins_x_lim: tuple[float, float] | None
+        :param ins_y_lim: Y limits for the inset.
+        :type ins_y_lim: tuple[float, float] | None
+        :return: The inset axes.
         :rtype: Axes
         """
         wdt = ins_x_loc[1] - ins_x_loc[0]
         hgt = ins_y_loc[1] - ins_y_loc[0]
         inset = ax.inset_axes([ins_x_loc[0], ins_y_loc[0], wdt, hgt])
         if ins_x_lim is not None:
             inset.set_xlim(MyFigure._adjust_lims(ins_x_lim))
         if ins_y_lim is not None:
             inset.set_ylim(MyFigure._adjust_lims(ins_y_lim))
         return inset
 
     def update_axes_single_props(self):
-        """_summary_"""
+        """
+        Update properties that are applied to each axis individually.
+        """
         for sprop in [
             "x_lab",
             "y_lab",
             "yt_lab",
             "grid",
         ]:
             self.broad_props[sprop] = self._broadcast_value_prop(self.kwargs[sprop], sprop)
 
         # Update each axis with the respective properties
         for i, ax in enumerate(self.axs):
-            ax.set_xlabel(self.broad_props["x_lab"][i])
-            ax.set_ylabel(self.broad_props["y_lab"][i])
+            ax.set_xlabel(self.broad_props["x_lab"][i], labelpad=self.kwargs["x_labelpad"])
+            ax.set_ylabel(self.broad_props["y_lab"][i], labelpad=self.kwargs["y_labelpad"])
             if self.broad_props["grid"][i] is not None:
                 ax.grid(self.broad_props["grid"][i])
         if self.kwargs["twinx"]:
             for i, axt in enumerate(self.axts):
                 axt.set_ylabel(self.broad_props["yt_lab"][i])
 
     def update_axes_list_props(self):
-        """_summary_"""
+        """
+        Update list properties for the axes.
+        """
         for lprop in [
             "x_lim",
             "y_lim",
             "yt_lim",
             "x_ticks",
             "y_ticks",
             "yt_ticks",
@@ -515,14 +532,17 @@
                     axt.set_ylim(MyFigure._adjust_lims(self.broad_props["yt_lim"][i]))
                 if self.broad_props["yt_ticks"][i] is not None:
                     axt.set_yticks(self.broad_props["yt_ticks"][i])
                 if self.broad_props["yt_ticklabels"][i] is not None:
                     axt.set_yticklabels(self.broad_props["yt_ticklabels"][i])
 
     def rotate_x_labels(self):
+        """
+        Rotate the labels on the x-axis.
+        """
         self.broad_props["x_ticklabels_rotation"] = self._broadcast_value_prop(
             self.kwargs["x_ticklabels_rotation"], "x_ticklabels_rotation"
         )
 
         # Update each axis with the respective properties
         for i, ax in enumerate(self.axs):
             rotation = self.broad_props["x_ticklabels_rotation"][i]
@@ -531,41 +551,47 @@
             for label in ax.get_xticklabels():
                 label.set_rotation(rotation)
                 if rotation != 0:
                     label.set_ha("right")
                     label.set_rotation_mode("anchor")
 
     def apply_hatch_patterns(self):
+        """
+        Apply hatch patterns to bars in the bar plots of each subplot.
+
+        This method iterates over all subplots and applies predefined hatch patterns to each bar,
+        enhancing the visual distinction between bars, especially in black and white printouts.
+        """
         for ax in self.axs:
             # Check if the plot is a bar plot
-            bars = [bar for bar in ax.patches if isinstance(bar, mpatches.Rectangle)]
+            bars = [b for b in ax.patches if isinstance(b, mpatches.Rectangle)]
             # If there are no bars, return immediately
             if not bars:
                 return
             num_groups = len(ax.get_xticks(minor=False))
             # Determine the number of bars in each group
             bars_in_group = len(bars) // num_groups
             patterns = htchs[:bars_in_group]  # set hatch patterns in correct order
             hatches = []  # list for hatches in the order of the bars
             for h in patterns:  # loop over patterns to create bar-ordered hatches
-                for i in range(int(len(bars) / len(patterns))):
+                for _ in range(int(len(bars) / len(patterns))):
                     hatches.append(h)
             # loop over bars and hatches to set hatches in correct order
-            for bar, hatch in zip(bars, hatches):
-                bar.set_hatch(hatch)
+            for b, hatch in zip(bars, hatches):
+                b.set_hatch(hatch)
 
     def _broadcast_value_prop(self, prop: list | str | float | int | bool, prop_name: str) -> list:
-        """_summary_
+        """
+        Broadcast a single value property to a list applicable to all subplots.
 
-        :param prop: _description_
-        :type prop: list | str | float | int | bool
-        :param prop_name: The name of the property for error messages.
+        :param prop: The property to broadcast.
+        :type prop: Union[list, str, float, int, bool]
+        :param prop_name: The name of the property, used in error messages.
         :type prop_name: str
-        :raises ValueError: _description_
-        :return: _description_
+        :return: A list of the property values broadcasted to match the number of subplots.
         :rtype: list
         """
         if prop is None:
             return [None] * self.n_axs
         if isinstance(prop, (list, tuple)):
             if len(prop) == self.n_axs:
                 return prop
@@ -586,24 +612,26 @@
         :raises ValueError: _description_
         :return: _description_
         :rtype: _type_
         """
         if prop is None:
             return [None] * self.n_axs
 
+        # Check if prop is a list of lists and has the correct length
         if all(isinstance(item, (list, tuple)) for item in prop) and len(prop) == self.n_axs:
+            # Ensure all inner lists have the same size
+            if not all(len(item) == len(prop[0]) for item in prop):
+                raise ValueError(f"All inner lists in '{prop_name}' must have the same size.")
             return prop
         elif isinstance(prop, (list, tuple)) and all(
             isinstance(item, (int, float, str)) for item in prop
         ):
             return [prop] * self.n_axs
         else:
-            raise ValueError(
-                f"The structure of '{prop_name = }' does not match expected pair-wise input."
-            )
+            raise ValueError(f"The structure of '{prop_name}' does not match the expected input.")
 
 
 if __name__ == "__main__":
     f = MyFigure(
         filename="my_plot",
         out_path=plib.Path(r"C:\Users\mp933\Desktop\New folder"),
         rows=4,
```

### Comparing `tga_data_analysis-2.0.2/src/tga_data_analysis/tga.py` & `tga_data_analysis-2.0.4/src/tga_data_analysis/tga.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Dec 14 14:28:04 2022
-
-@author: mp933
-"""
-# %%
 from __future__ import annotations
+from typing import Literal, Any
 import pathlib as plib
 import numpy as np
 import pandas as pd
-from typing import Any
 from scipy.signal import savgol_filter
 from lmfit.models import GaussianModel, LinearModel
-from typing import Literal
-from tga_data_analysis.myfigure import MyFigure, clrs, lnstls, htchs, mrkrs
+from tga_data_analysis.measure import Measure
+from tga_data_analysis.myfigure import MyFigure, clrs, lnstls
+
 
 
 class Project:
+    """
+    Represents a project (identified by the folder where the data is stored) for TGA data analysis.
+
+    """
 
     def __init__(
         self,
         folder_path: plib.Path,
         name: str | None = None,
         temp_unit: Literal["C", "K"] = "C",
         plot_font: Literal["Dejavu Sans", "Times New Roman"] = "Dejavu Sans",
@@ -33,14 +31,50 @@
         load_skiprows: int = 0,
         time_moist: float = 38.0,
         time_vm: float = 147.0,
         temp_initial_celsius: float = 40,
         temp_lim_dtg_celsius: tuple[float] | None = None,
         auto_save_reports: bool = True,
     ):
+        """
+        Initialize a new Project instance with various parameters for analysis.
+
+        :param folder_path: The path to the folder containing the project data.
+        :type folder_path: plib.Path
+        :param name: The name of the project. Defaults to the last part of the folder path if None.
+        :type name: str, optional
+        :param temp_unit: The unit of temperature used in the project ('C':Celsius, 'K':Kelvin).
+        :type temp_unit: Literal["C", "K"]
+        :param plot_font: The font used in plots, either 'Dejavu Sans' or 'Times New Roman'.
+        :type plot_font: Literal["Dejavu Sans", "Times New Roman"]
+        :param dtg_basis: The basis for DTG calculations, either 'temperature' or 'time'.
+        :type dtg_basis: Literal["temperature", "time"]
+        :param temp_i_temp_b_threshold: The threshold for Ti and Tb calculation in DTG analysis.
+        :type temp_i_temp_b_threshold: float
+        :param resolution_sec_deg_dtg: The resolution in seconds or degrees for DTG analysis.
+        :type resolution_sec_deg_dtg: int
+        :param dtg_window_filter: The window size for the Savitzky-Golay filter in DTG analysis.
+        :type dtg_window_filter: int
+        :param plot_grid: Whether to display a grid in the plots.
+        :type plot_grid: bool
+        :param column_name_mapping: Mapping of column names from file to standard names used in the analysis.
+        :type column_name_mapping: dict[str, str], optional
+        :param load_skiprows: The number of rows to skip when loading data files.
+        :type load_skiprows: int
+        :param time_moist: The time considered for the moisture analysis.
+        :type time_moist: float
+        :param time_vm: The time considered for the volatile matter analysis.
+        :type time_vm: float
+        :param temp_initial_celsius: The initial temperature for certain calculations, in Celsius.
+        :type temp_initial_celsius: float
+        :param temp_lim_dtg_celsius: The temperature limits for DTG analysis, in Celsius.
+        :type temp_lim_dtg_celsius: tuple[float], optional
+        :param auto_save_reports: Whether to automatically save generated reports.
+        :type auto_save_reports: bool
+        """
         self.folder_path = folder_path
         self.out_path = plib.Path(folder_path, "output")
         if name is None:
             self.name = self.folder_path.parts[-1]
         else:
             self.name = name
         self.temp_unit = temp_unit
@@ -103,14 +137,22 @@
         self.samples: dict[str, Sample] = {}
         self.samplenames: list[str] = []
 
         self.multireports: dict[str, pd.DataFrame] = {}
         self.multireport_types_computed: list[str] = []
 
     def add_sample(self, samplename: str, sample: Sample):
+        """
+        Add a sample to the project.
+
+        :param samplename: The name of the sample to add.
+        :type samplename: str
+        :param sample: The sample object to add.
+        :type sample: Sample
+        """
         if samplename not in self.samplenames:
             self.samplenames.append(samplename)
             self.samples[samplename] = sample
         else:
             print(f"{samplename = } already present in project. Sample not added.")
 
     def multireport(
@@ -121,22 +163,30 @@
             "proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"
         ] = "proximate",
         report_style: Literal["repl_ave_std", "ave_std", "ave_pm_std"] = "ave_std",
         decimals_in_ave_pm_std: int = 2,
         filename: str | None = None,
     ) -> pd.DataFrame:
         """
-        Generate a multi-sample proximate report.
+        Generate a multi-sample report based on the specified report type and style.
 
-        Args:
-            exps (list): List of experiments.
-            filename (str, optional): Name of the output file. Defaults to 'Rep'.
-
-        Returns:
-            pandas.DataFrame: DataFrame containing the multi-sample proximate report.
+        :param samples: A list of Sample objects to include in the report. If None, uses all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: A list of labels corresponding to each sample. If None, sample names are used as labels.
+        :type labels: list[str], optional
+        :param report_type: The type of report to generate, choices include 'proximate', 'oxidation', 'oxidation_extended', 'soliddist', and 'soliddist_extended'.
+        :type report_type: Literal["proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"]
+        :param report_style: The style of the report, choices are 'repl_ave_std', 'ave_std', and 'ave_pm_std'.
+        :type report_style: Literal["repl_ave_std", "ave_std", "ave_pm_std"]
+        :param decimals_in_ave_pm_std: The number of decimal places to use for the average plus-minus standard deviation format.
+        :type decimals_in_ave_pm_std: int
+        :param filename: The name of the file to save the report. If None, the report is not saved.
+        :type filename: str, optional
+        :return: A pandas DataFrame containing the generated report.
+        :rtype: pd.DataFrame
         """
         if samples is None:
             samples = list(self.samples.values())
 
         samplenames = [sample.name for sample in samples]
 
         if labels is None:
@@ -199,34 +249,30 @@
         samples: list[Sample] | None = None,
         labels: list[str] | None = None,
         report_type: Literal["proximate", "oxidation", "soliddist"] = "proximate",
         bar_labels: list[str] | None = None,
         **kwargs,
     ) -> MyFigure:
         """
-        Generate a multi-plot for proximate analysis.
-
-        Parameters:
-        - exps (list): List of experiments.
-        - filename (str): Name of the output file (default: "Prox").
-        - smpl_labs (list): List of sample labels (default: None).
-        - xlab_rot (int): Rotation angle of x-axis labels (default: 0).
-        - paper_col (float): Color of the plot background (default: 0.8).
-        - hgt_mltp (float): Height multiplier of the plot (default: 1.5).
-        - bboxtoanchor (bool): Whether to place the legend outside the plot area (default: True).
-        - x_anchor (float): X-coordinate of the legend anchor point (default: 1.13).
-        - y_anchor (float): Y-coordinate of the legend anchor point (default: 1.02).
-        - legend_loc (str): Location of the legend (default: 'best').
-        - y_lim (list): Y-axis limits for the bar plot (default: [0, 100]).
-        - yt_lim (list): Y-axis limits for the scatter plot (default: [0, 1]).
-        - y_ticks (list): Y-axis tick positions for the bar plot (default: None).
-        - yt_ticks (list): Y-axis tick positions for the scatter plot (default: None).
+        Generate a plot for the multi-sample report.
 
-        Returns:
-        - None
+        :param filename: The name of the file to save the plot. Defaults to "plot".
+        :type filename: str
+        :param samples: A list of Sample objects to include in the plot. If None, uses all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: A list of labels corresponding to each sample. If None, sample names are used as labels.
+        :type labels: list[str], optional
+        :param report_type: The type of report to plot, choices include 'proximate', 'oxidation', and 'soliddist'.
+        :type report_type: Literal["proximate", "oxidation", "soliddist"]
+        :param bar_labels: Labels for the bars in the plot. If None, default labels based on the report type are used.
+        :type bar_labels: list[str], optional
+        :param kwargs: Additional keyword arguments to pass to the plotting function.
+        :type kwargs: dict
+        :return: An instance of MyFigure containing the generated plot.
+        :rtype: MyFigure
         """
         if samples is None:
             samples = list(self.samples.values())
 
         samplenames = [sample.name for sample in samples]
         if labels is None:
             labels = samplenames
@@ -278,16 +324,16 @@
             yt_lab = None
 
         out_path = plib.Path(self.out_path, "multireport_plots")
         out_path.mkdir(parents=True, exist_ok=True)
         default_kwargs = {
             "filename": filename + report_type,
             "out_path": out_path,
-            "height": 4,
-            "width": 4,
+            "height": 3.2,
+            "width": 3.2,
             "grid": self.plot_grid,
             "text_font": self.plot_font,
         }
         # Update kwargs with the default key-value pairs if the key is not present in kwargs
         kwargs = {**default_kwargs, **kwargs}
         myfig = MyFigure(
             rows=1,
@@ -330,30 +376,26 @@
         self,
         filename: str = "plot",
         samples: list[Sample] | None = None,
         labels: list[str] | None = None,
         **kwargs,
     ) -> MyFigure:
         """
-        Plot multiple thermogravimetric (TG) curves.
-
-        Args:
-            exps (list): List of experimental data objects.
-            filename (str, optional): Name of the output file. Defaults to 'Fig'.
-            paper_col (float, optional): Width of the figure in inches. Defaults to 0.78.
-            hgt_mltp (float, optional): Height multiplier of the figure. Defaults to 1.25.
-            x_lim (tuple, optional): Limits of the x-axis. Defaults to None.
-            y_lim (list, optional): Limits of the y-axis. Defaults to [0, 100].
-            y_ticks (list, optional): Custom y-axis tick locations. Defaults to None.
-            lttrs (bool, optional): Whether to annotate letters on the plot. Defaults to False.
-            save_as_pdf (bool, optional): Whether to save the figure as a PDF file. Defaults to False.
-            save_as_svg (bool, optional): Whether to save the figure as an SVG file. Defaults to False.
+        Plot multiple thermogravimetric (TG) curves for the given samples.
 
-        Returns:
-            None
+        :param filename: The name of the file to save the plot. Defaults to "plot".
+        :type filename: str
+        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: Labels for each sample in the plot. If None, sample names are used.
+        :type labels: list[str], optional
+        :param kwargs: Additional keyword arguments for plotting customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the plot.
+        :rtype: MyFigure
         """
         if samples is None:
             samples = list(self.samples.values())
 
         samplenames = [sample.name for sample in samples]
         if labels is None:
             labels = samplenames
@@ -363,16 +405,16 @@
 
         out_path = plib.Path(self.out_path, "multisample_plots")
         out_path.mkdir(parents=True, exist_ok=True)
 
         default_kwargs = {
             "filename": filename + "_tg",
             "out_path": out_path,
-            "height": 4,
-            "width": 4,
+            "height": 3.2,
+            "width": 3.2,
             "grid": self.plot_grid,
             "text_font": self.plot_font,
             "x_lab": f"T [{self.temp_symbol}]",
             "y_lab": self.tg_label,
             "x_lim": self.temp_lim_dtg,
         }
         # Update kwargs with the default key-value pairs if the key is not present in kwargs
@@ -405,30 +447,26 @@
         self,
         filename: str = "plot",
         samples: list[Sample] | None = None,
         labels: list[str] | None = None,
         **kwargs,
     ) -> MyFigure:
         """
-        Plot multiple thermogravimetric (TG) curves.
+        Plot multiple derivative thermogravimetric (DTG) curves for the given samples.
 
-        Args:
-            exps (list): List of experimental data objects.
-            filename (str, optional): Name of the output file. Defaults to 'Fig'.
-            paper_col (float, optional): Width of the figure in inches. Defaults to 0.78.
-            hgt_mltp (float, optional): Height multiplier of the figure. Defaults to 1.25.
-            x_lim (tuple, optional): Limits of the x-axis. Defaults to None.
-            y_lim (list, optional): Limits of the y-axis. Defaults to [0, 100].
-            y_ticks (list, optional): Custom y-axis tick locations. Defaults to None.
-            lttrs (bool, optional): Whether to annotate letters on the plot. Defaults to False.
-            save_as_pdf (bool, optional): Whether to save the figure as a PDF file. Defaults to False.
-            save_as_svg (bool, optional): Whether to save the figure as an SVG file. Defaults to False.
-
-        Returns:
-            None
+        :param filename: The name of the file to save the plot. Defaults to "plot".
+        :type filename: str
+        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: Labels for each sample in the plot. If None, sample names are used.
+        :type labels: list[str], optional
+        :param kwargs: Additional keyword arguments for plotting customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the plot.
+        :rtype: MyFigure
         """
         if samples is None:
             samples = list(self.samples.values())
 
         samplenames = [sample.name for sample in samples]
         if labels is None:
             labels = samplenames
@@ -437,16 +475,16 @@
                 sample.proximate_analysis()
 
         out_path = plib.Path(self.out_path, "multisample_plots")
         out_path.mkdir(parents=True, exist_ok=True)
         default_kwargs = {
             "filename": filename + "_dtg",
             "out_path": out_path,
-            "height": 4,
-            "width": 4,
+            "height": 3.2,
+            "width": 3.2,
             "grid": self.plot_grid,
             "text_font": self.plot_font,
             "x_lab": f"T [{self.temp_symbol}]",
             "y_lab": self.dtg_label,
             "x_lim": self.temp_lim_dtg,
         }
         # Update kwargs with the default key-value pairs if the key is not present in kwargs
@@ -479,30 +517,26 @@
         self,
         filename: str = "plot",
         samples: list[Sample] | None = None,
         labels: list[str] | None = None,
         **kwargs,
     ) -> MyFigure:
         """
-        Plot multiple thermogravimetric (TG) curves.
-
-        Args:
-            exps (list): List of experimental data objects.
-            filename (str, optional): Name of the output file. Defaults to 'Fig'.
-            paper_col (float, optional): Width of the figure in inches. Defaults to 0.78.
-            hgt_mltp (float, optional): Height multiplier of the figure. Defaults to 1.25.
-            x_lim (tuple, optional): Limits of the x-axis. Defaults to None.
-            y_lim (list, optional): Limits of the y-axis. Defaults to [0, 100].
-            y_ticks (list, optional): Custom y-axis tick locations. Defaults to None.
-            lttrs (bool, optional): Whether to annotate letters on the plot. Defaults to False.
-            save_as_pdf (bool, optional): Whether to save the figure as a PDF file. Defaults to False.
-            save_as_svg (bool, optional): Whether to save the figure as an SVG file. Defaults to False.
+        Plot multiple solid distribution curves for the given samples.
 
-        Returns:
-            None
+        :param filename: The name of the file to save the plot. Defaults to "plot".
+        :type filename: str
+        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: Labels for each sample in the plot. If None, sample names are used.
+        :type labels: list[str], optional
+        :param kwargs: Additional keyword arguments for plotting customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the plot.
+        :rtype: MyFigure
         """
         if samples is None:
             samples = list(self.samples.values())
 
         samplenames = [sample.name for sample in samples]
         if labels is None:
             labels = samplenames
@@ -511,16 +545,16 @@
                 sample.proximate_analysis()
 
         out_path = plib.Path(self.out_path, "multisample_plots")
         out_path.mkdir(parents=True, exist_ok=True)
         default_kwargs = {
             "filename": filename + "_soliddist",
             "out_path": out_path,
-            "height": 4,
-            "width": 5,
+            "height": 3.2,
+            "width": 3.2,
             "grid": self.plot_grid,
             "text_font": self.plot_font,
             "x_lab": "time [min]",
             "y_lab": self.tg_label,
             "yt_lab": f"T [{self.temp_symbol}]",
             "legend_loc": "center left",
         }
@@ -552,18 +586,23 @@
                 alpha=0.3,
             )
         myfig.save_figure()
         return myfig
 
     def _reformat_ave_std_columns(self, reports):
         """
-        Reformat column names based on the average and standard deviation.
+        Reformat the columns of the given reports to have standard deviation and average values.
 
-        Args:
-            reports (list of pd.DataFrame): List of reports to reformat column names.
+        This method is intended to be used internally within the Project class to standardize
+        the report dataframes before generating multi-sample reports.
+
+        :param reports: A list of report DataFrames to reformat.
+        :type reports: list[pd.DataFrame]
+        :return: A list of reformatted DataFrames.
+        :rtype: list[pd.DataFrame]
         """
         # Check that all reports have the same number of columns
         num_columns = len(reports[0].columns)
         if not all(len(report.columns) == num_columns for report in reports):
             raise ValueError("All reports must have the same number of columns.")
 
         # Initialize a list to hold the new formatted column names
@@ -587,14 +626,18 @@
         for report in reports:
             report.columns = formatted_column_names
 
         return reports
 
 
 class Sample:
+    """
+    A class representing a sample in the project, containing methods for loading, processing,
+    and analyzing thermogravimetric analysis (TGA) data associated with the sample.
+    """
 
     def __init__(
         self,
         project: Project,
         name: str,
         filenames: list[str],
         folder_path: plib.Path | None = None,
@@ -604,14 +647,44 @@
         column_name_mapping: dict[str:str] | None = None,
         load_skiprows: int = 0,
         time_moist: float = 38.0,
         time_vm: float = 147,
         heating_rate_deg_min: float | None = None,
         temp_i_temp_b_threshold: float | None = None,
     ):
+        """
+        Initialize a new Sample instance with parameters for TGA data analysis.
+
+        :param project: The Project object to which this sample belongs.
+        :type project: Project
+        :param name: The name of the sample.
+        :type name: str
+        :param filenames: A list of filenames associated with the sample.
+        :type filenames: list[str]
+        :param folder_path: The path to the folder containing the sample data. If None, the project's folder path is used.
+        :type folder_path: plib.Path, optional
+        :param label: A label for the sample. If None, the sample's name is used as the label.
+        :type label: str, optional
+        :param correct_ash_mg: A list of ash correction values in milligrams, one per file.
+        :type correct_ash_mg: list[float], optional
+        :param correct_ash_fr: A list of ash correction values as a fraction, one per file.
+        :type correct_ash_fr: list[float], optional
+        :param column_name_mapping: A dictionary mapping file column names to standardized column names for analysis.
+        :type column_name_mapping: dict[str, str], optional
+        :param load_skiprows: The number of rows to skip at the beginning of the files when loading.
+        :type load_skiprows: int
+        :param time_moist: The time considered for the moisture analysis.
+        :type time_moist: float
+        :param time_vm: The time considered for the volatile matter analysis.
+        :type time_vm: float
+        :param heating_rate_deg_min: The heating rate in degrees per minute, used for certain calculations.
+        :type heating_rate_deg_min: float, optional
+        :param temp_i_temp_b_threshold: The threshold percentage used for calculating initial and final temperatures in DTG analysis.
+        :type temp_i_temp_b_threshold: float, optional
+        """
         # store the sample in the project
         self.project_name = project.name
         project.add_sample(name, self)
         # prject defaults unless specified
 
         self.out_path = project.out_path
         self.temp_unit = project.temp_unit
@@ -714,29 +787,31 @@
         self.dcv_peaks: list[Measure] = []
         # Flag to track if data is loaded
         self.proximate_computed = False
         self.files_loaded = False
         self.oxidation_computed = False
         self.soliddist_computed = False
         self.deconv_computed = False
-        self.KAS_computed = False
         # for reports
         self.reports: dict[str, pd.DataFrame] = {}
         self.report_types_computed: list[str] = []
 
         self.load_files()
         self.proximate_analysis()
 
     def _broadcast_value_prop(self, prop: list | str | float | int | bool) -> list:
-        """_summary_
+        """
+        Broadcast a single value or a list of values to match the number of replicates.
 
-        :param prop: _description_
-        :type prop: list | str | float | int | bool
-        :raises ValueError: _description_
-        :return: _description_
+        This method is used internally to ensure that properties like corrections have a value
+        for each replicate, even if a single value is provided for all.
+
+        :param prop: A single value or a list of values to be broadcasted.
+        :type prop: list | float | int | bool
+        :return: A list of values with length equal to the number of replicates.
         :rtype: list
         """
         if prop is None:
             broad_prop = [None] * self.n_repl
         if isinstance(prop, (list, tuple)):
             # If it's a list or tuple, but we're not expecting pairs, it's a single value per axis.
             if len(prop) == self.n_repl:
@@ -752,14 +827,28 @@
     def load_single_file(
         self,
         filename: str,
         folder_path: plib.Path | None = None,
         load_skiprows: int | None = None,
         column_name_mapping: dict | None = None,
     ) -> pd.DataFrame:
+        """
+        Load data from a single file associated with the sample.
+
+        :param filename: The name of the file to be loaded.
+        :type filename: str
+        :param folder_path: The folder path where the file is located. If None, uses the sample's folder path.
+        :type folder_path: plib.Path, optional
+        :param load_skiprows: The number of rows to skip at the beginning of the file. If None, uses the sample's default.
+        :type load_skiprows: int, optional
+        :param column_name_mapping: A mapping of file column names to standardized column names. If None, uses the sample's default.
+        :type column_name_mapping: dict, optional
+        :return: The loaded data as a pandas DataFrame.
+        :rtype: pd.DataFrame
+        """
         if column_name_mapping is None:
             column_name_mapping = self.column_name_mapping
         if folder_path is None:
             folder_path = self.folder_path
         if load_skiprows is None:
             load_skiprows = self.load_skiprows
         file_path = plib.Path(folder_path, filename + ".txt")
@@ -776,14 +865,28 @@
 
     def correct_file_values(
         self,
         file: pd.DataFrame,
         correct_ash_fr: float | None,
         correct_ash_mg: float | None,
     ):
+        """
+        Apply corrections to the loaded file data.
+
+        This method adjusts the mass measurements in the file based on provided ash correction values.
+
+        :param file: The data file to be corrected.
+        :type file: pd.DataFrame
+        :param correct_ash_mg: The correction value for ash in milligrams. If None, no correction is applied.
+        :type correct_ash_mg: float, optional
+        :param correct_ash_fr: The correction value for ash as a fraction. If None, no correction is applied.
+        :type correct_ash_fr: float, optional
+        :return: The corrected data as a pandas DataFrame.
+        :rtype: pd.DataFrame
+        """
         if correct_ash_mg is not None:
             file["m_mg"] = file["m_mg"] - np.min(file["m_mg"]) + correct_ash_mg
         try:
             if file["m_mg"].iloc[-1] < 0:
                 print(
                     "neg. mass correction: Max [mg]",
                     np.round(np.max(file["m_mg"]), 3),
@@ -799,18 +902,21 @@
             file["m_p"] = file["m_p"] / np.max(file["m_p"]) * 100
         file = file[file["T_C"] >= self.temp_initial_celsius].copy()
         file["T_K"] = file["T_C"] + 273.15
         return file
 
     def load_files(self):
         """
-        Loads all the files for the experiment.
+        Load all files associated with this sample, applying necessary corrections and adjustments.
+
+        This method loads and processes each file, ensuring consistent data structure and applying
+        corrections such as ash content adjustments.
 
-        Returns:
-            list: The list of loaded files.
+        :return: A dictionary where keys are filenames and values are the corresponding corrected data as pandas DataFrames.
+        :rtype: dict[str, pd.DataFrame]
         """
         print("\n" + self.name)
         # import files and makes sure that replicates have the same size
         for f, filename in enumerate(self.filenames):
             print(filename)
             file_to_correct = self.load_single_file(filename)
 
@@ -825,15 +931,18 @@
         for filename in self.filenames:
             self.files[filename] = self.files[filename].head(self.len_sample)
         self.files_loaded = True  # Flag to track if data is loaded
         return self.files
 
     def proximate_analysis(self):
         """
-        Performs proximate analysis on the loaded data.
+        Perform proximate analysis on the loaded data for the sample.
+
+        This analysis calculates moisture content, ash content, volatile matter, and fixed carbon
+        based on the thermogravimetric data. The results are stored in the instance's attributes for later use.
         """
         if not self.files_loaded:
             self.load_files()
 
         for f, file in enumerate(self.files.values()):
             if self.temp_unit == "C":
                 self.temp.add(f, file["T_C"])
@@ -903,22 +1012,20 @@
         # average
         self.ave_dev_tga_perc = np.average(self.mp_db_dtg.std())
         print(f"Average TG [%] St. Dev. for replicates: {self.ave_dev_tga_perc:0.2f} %")
         self.proximate_computed = True
 
     def oxidation_analysis(self):
         """
-        Perform oxidation analysis on the data.
-
-        This method calculates various oxidation parameters based on the proximate analysis results.
-        It computes the Ti, Tp, Tb, dwdT_max, dwdT_mean, and S values for each file in the dataset,
-        and then calculates the average and standard deviation of these values.
+        Conduct oxidation analysis on the sample's data.
 
-        Returns:
-            None
+        This method calculates various oxidation parameters such as the initial oxidation temperature (Ti),
+        peak oxidation temperature (Tp), and final oxidation temperature (Tb). It also computes derivative
+        parameters like maximum and average rates of weight loss. The results are stored in the instance's
+        attributes for further analysis.
         """
         if not self.proximate_computed:
             self.proximate_analysis()
 
         for f in range(self.n_repl):
             threshold: float = np.max(np.abs(self.dtg_db.stk(f))) * self.temp_i_temp_b_threshold
             # Ti = T at which dtg > Ti_thresh wt%/min after moisture removal
@@ -948,22 +1055,21 @@
                 ),
             )
         # # average
         self.oxidation_computed = True
 
     def soliddist_analysis(self, steps_min: list[float] | None = None):
         """
-        Perform solid distance analysis.
+        Perform solid distribution analysis on the sample's data.
 
-        Args:
-            steps_min (list, optional): List of minimum steps for analysis.
-              Defaults to [40, 70, 100, 130, 160, 190].
+        This analysis calculates the weight loss at specified temperature steps, providing insight into
+        the solid decomposition process. The results are used for generating solid distribution plots.
 
-        Returns:
-            None
+        :param steps_min: Temperature steps (in minutes) at which the weight loss is calculated. If None, default steps are used.
+        :type steps_min: list[float], optional
         """
         if steps_min is None:
             steps_min = [40, 70, 100, 130, 160, 190]
         if not self.proximate_computed:
             self.proximate_analysis()
 
         for f in range(self.n_repl):
@@ -991,30 +1097,37 @@
         center_maxs: list[float] | None = None,
         sigma_mins: list[float] | None = None,
         sigma_maxs: list[float] | None = None,
         amplitude_mins: list[float] | None = None,
         amplitude_maxs: list[float] | None = None,
     ):
         """
-        Perform deconvolution analysis on the data.
+        Perform deconvolution analysis on the sample's DTG data.
 
-        Args:
-            centers (list): List of peak centers.
-            sigmas (list, optional): List of peak sigmas. Defaults to None.
-            amplitudes (list, optional): List of peak amplitudes. Defaults to None.
-            center_mins (list, optional): List of minimum values for peak centers. Defaults to None.
-            center_maxs (list, optional): List of maximum values for peak centers. Defaults to None.
-            s_mins (list, optional): List of minimum values for peak sigmas. Defaults to None.
-            s_maxs (list, optional): List of maximum values for peak sigmas. Defaults to None.
-            a_mins (list, optional): List of minimum values for peak amplitudes. Defaults to None.
-            a_maxs (list, optional): List of maximum values for peak amplitudes. Defaults to None.
-            TLim (tuple, optional): Tuple specifying the time range for analysis. Defaults to None.
+        This method fits multiple Gaussian peaks to the DTG curve to identify and analyze individual
+        decomposition steps within the sample.
 
-        Returns:
-            None
+        :param centers: Initial guesses for the centers of the Gaussian peaks.
+        :type centers: list[float]
+        :param sigmas: Initial guesses for the standard deviations of the Gaussian peaks. If None, defaults are used.
+        :type sigmas: list[float], optional
+        :param amplitudes: Initial guesses for the amplitudes of the Gaussian peaks. If None, defaults are used.
+        :type amplitudes: list[float], optional
+        :param center_mins: Minimum allowed values for the centers of the Gaussian peaks. If None, no bounds are applied.
+        :type center_mins: list[float], optional
+        :param center_maxs: Maximum allowed values for the centers of the Gaussian peaks. If None, no bounds are applied.
+        :type center_maxs: list[float], optional
+        :param sigma_mins: Minimum allowed values for the standard deviations of the Gaussian peaks. If None, no bounds are applied.
+        :type sigma_mins: list[float], optional
+        :param sigma_maxs: Maximum allowed values for the standard deviations of the Gaussian peaks. If None, no bounds are applied.
+        :type sigma_maxs: list[float], optional
+        :param amplitude_mins: Minimum allowed values for the amplitudes of the Gaussian peaks. If None, no bounds are applied.
+        :type amplitude_mins: list[float], optional
+        :param amplitude_maxs: Maximum allowed values for the amplitudes of the Gaussian peaks. If None, no bounds are applied.
+        :type amplitude_maxs: list[float], optional
         """
         if not self.proximate_computed:
             self.proximate_analysis()
         n_peaks = len(centers)
         # self.dcv_best_fit_stk = np.zeros((self.len_dtg_db, self.n_repl))
         # self.dcv_r2_stk = np.zeros(self.n_repl)
 
@@ -1072,14 +1185,26 @@
 
     def report(
         self,
         report_type: Literal[
             "proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"
         ] = "proximate",
     ) -> pd.DataFrame:
+        """
+        Generate a report based on the specified analysis type.
+
+        This method provides detailed insights into the sample's properties, such as proximate analysis,
+        oxidation characteristics, and solid distribution, based on the selected report type.
+
+        :param report_type: The type of report to generate. Options include 'proximate', 'oxidation',
+                            'oxidation_extended', 'soliddist', and 'soliddist_extended'.
+        :type report_type: Literal["proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"]
+        :return: A pandas DataFrame containing the analysis results.
+        :rtype: pd.DataFrame
+        """
         if report_type == "proximate":
             if not self.proximate_computed:
                 self.proximate_analysis()
             variables = [self.moist_ar, self.vm_db, self.fc_db, self.ash_db]
         elif report_type == "oxidation" or report_type == "oxidation_extended":
             if not self.oxidation_computed:
                 self.oxidation_analysis()
@@ -1119,27 +1244,34 @@
             out_path = plib.Path(self.out_path, "single_sample_reports")
             out_path.mkdir(parents=True, exist_ok=True)
             report.to_excel(plib.Path(out_path, f"{self.name}_{report_type}.xlsx"))
         return report
 
     def plot_tg_dtg(self, **kwargs: dict[str, Any]) -> MyFigure:
         """
-        Plot the TGA data.
+        Generate a plot combining thermogravimetric (TG) and derivative thermogravimetric (DTG) data.
 
+        This method creates a figure showing the TG and DTG curves, providing a visual representation
+        of the sample's thermal decomposition behavior.
+
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the generated plot.
+        :rtype: MyFigure
         """
         if not self.proximate_computed:
             self.proximate_analysis()
         out_path = plib.Path(self.out_path, "single_sample_plots")
         out_path.mkdir(parents=True, exist_ok=True)
 
         default_kwargs = {
             "filename": self.name + "_tg_dtg",
             "out_path": out_path,
-            "height": 8,
-            "width": 6,
+            "height": 8.53,
+            "width": 6.4,
             "x_lab": "time [min]",
             "y_lab": [
                 f"T [{self.temp_symbol}]",
                 f"T [{self.temp_symbol}]",
                 f"{self.tg_label} (stb)",
                 f"{self.tg_label} (db)",
                 f"{self.tg_label} (db)",
@@ -1255,35 +1387,36 @@
                     color=clrs[f],
                 )
         mf.save_figure()
         return mf
 
     def plot_soliddist(self, **kwargs: dict[str, Any]) -> MyFigure:
         """
-        Plot the solid distribution analysis.
+        Generate a plot illustrating the solid distribution analysis results.
 
-        Args:
-            paper_col (int): Number of columns in the plot for paper publication (default is 1).
-            hgt_mltp (float): Height multiplier for the plot (default is 1.25).
+        This method plots the weight loss of the sample at specified temperature steps, showing the
+        distribution of solid components within the sample.
 
-        Returns:
-            None
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the generated plot.
+        :rtype: MyFigure
         """
 
         # slightly different plotting behaviour (uses averages)
         if not self.soliddist_computed:
             self.soliddist_analysis()
         out_path = plib.Path(self.out_path, "single_sample_plots")
         out_path.mkdir(parents=True, exist_ok=True)
 
         default_kwargs = {
             "filename": self.name + "_soliddist",
             "out_path": out_path,
-            "height": 4,
-            "width": 5,
+            "height": 3.2,
+            "width": 3.2,
             "x_lab": "time [min]",
             "y_lab": f"{self.tg_label} (db)",
             "yt_lab": f"T [{self.temp_symbol}]",
             "legend_loc": "center left",
             "grid": self.plot_grid,
             "text_font": self.plot_font,
         }
@@ -1312,35 +1445,35 @@
                 f"{dmp:0.0f}%", ha="center", va="top", xy=(tm - 10, mp + 1), fontsize=9
             )
         mf.save_figure()
         return mf
 
     def plot_deconv(self, **kwargs: dict[str, Any]) -> MyFigure:
         """
-        Plot the deconvolution results.
+        Generate a plot showing the deconvolution analysis results.
+
+        This method visualizes the Gaussian peak fitting performed on the DTG data, illustrating the
+        identified decomposition steps within the sample.
 
-        Args:
-            filename (str, optional): The filename to save the plot. Defaults to 'Deconv'.
-            x_lim (tuple, optional): The x-axis limits of the plot. Defaults to None.
-            y_lim (tuple, optional): The y-axis limits of the plot. Defaults to None.
-            save_as_pdf (bool, optional): Whether to save the plot as a PDF file. Defaults to False.
-            save_as_svg (bool, optional): Whether to save the plot as an SVG file. Defaults to False.
-            legend (str, optional): The position of the legend in the plot. Defaults to 'best'.
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the deconvolution analysis plot.
+        :rtype: MyFigure
         """
 
         if not self.deconv_computed:
-            raise Exception("Deconvolution analysis not computed")
+            raise ValueError("Deconvolution analysis not computed")
         out_path = plib.Path(self.out_path, "single_sample_plots")
         out_path.mkdir(parents=True, exist_ok=True)
 
         default_kwargs = {
             "filename": self.name + "_deconv",
             "out_path": out_path,
-            "height": 8,
-            "width": 3.5,
+            "height": 8.53,
+            "width": 3.2,
             "x_lab": f"T [{self.temp_symbol}]",
             "y_lab": f"{self.dtg_label} (db)",
             "grid": self.plot_grid,
             "text_font": self.plot_font,
         }
         # Update kwargs with the default key-value pairs if the key is not present in kwargs
         kwargs = {**default_kwargs, **kwargs}
@@ -1375,238 +1508,7 @@
                 f"r$^2$={self.dcv_r2.stk(f):.2f}",
                 xycoords="axes fraction",
                 xy=(0.85, 0.96),
                 size="x-small",
             )
         mf.save_figure()
         return mf
-
-
-class Measure:
-    """
-    A class to collect and analyze a series of numerical data points or arrays.
-
-    Attributes:
-        _stk (dict): A dictionary to store the data points or numpy arrays with integer keys.
-    """
-
-    std_type: Literal["population", "sample"] = "population"
-    if std_type == "population":
-        np_ddof: int = 0
-    elif std_type == "sample":
-        np_ddof: int = 1
-
-    @classmethod
-    def set_std_type(cls, new_std_type: Literal["population", "sample"]):
-        """"""
-        cls.std_type = new_std_type
-        if new_std_type == "population":
-            cls.np_ddof: int = 0
-        elif new_std_type == "sample":
-            cls.np_ddof: int = 1
-
-    def __init__(self, name: str | None = None):
-        """
-        Initializes the Measure class with an empty dictionary for _stk.
-        """
-        self.name = name
-        self._stk: dict[int : np.ndarray | float] = {}
-        self._ave: np.ndarray | float | None = None
-        self._std: np.ndarray | float | None = None
-
-    def __call__(self):
-        return self.ave()
-
-    def add(self, replicate: int, value: np.ndarray | pd.Series | float | int) -> None:
-        """
-        Adds a new data point or numpy array to the _stk dictionary with the specified replicate key.
-
-        :param replicate: The integer key (replicate number) to associate with the value.
-        :param value: A data point, numpy array, or pandas Series to be added.
-        """
-        if isinstance(value, (pd.Series, pd.DataFrame)):
-            value = value.to_numpy()
-        elif isinstance(value, np.ndarray):
-            value = value.flatten()
-        elif isinstance(value, (list, tuple)):
-            value = np.asarray(value)
-        self._stk[replicate] = value
-
-    def stk(self, replicate: int | None = None) -> np.ndarray | float:
-        """
-        Retrieves the data point or array associated with the specified replicate key.
-
-        :param replicate: The key (replicate number) of the data point or array to retrieve.
-        :return: The data point or array associated with the replicate key.
-        """
-        if replicate is None:
-            return self._stk
-        else:
-            return self._stk.get(replicate)
-
-    def ave(self) -> np.ndarray:
-        """
-        Calculates the mean of all data points or arrays stored in _stk.
-
-        :return: The mean value(s) across all data points or arrays.
-        """
-        if all(isinstance(v, np.ndarray) for v in self._stk.values()):
-            self._ave = np.mean(np.column_stack(list(self._stk.values())), axis=1)
-            return self._ave
-        else:
-            self._ave = np.mean(list(self._stk.values()))
-            return self._ave
-
-    def std(self) -> np.ndarray:
-        """
-        Calculates the standard deviation of all data points or arrays stored in _stk.
-
-        :return: The standard deviation value(s) across all data points or arrays.
-        """
-        if all(isinstance(v, np.ndarray) for v in self._stk.values()):
-            self._std = np.std(
-                np.column_stack(list(self._stk.values())), axis=1, ddof=Measure.np_ddof
-            )
-            return self._std
-        else:
-            self._std = np.std(list(self._stk.values()), ddof=Measure.np_ddof)
-            return self._std
-
-
-# %%
-if __name__ == "__main__":
-
-    test_dir: plib.Path = plib.Path(
-        r"C:\Users\mp933\OneDrive - Cornell University\Python\tga_data_analysis\tests\data"
-    )
-
-    # %%
-    m1 = Measure()
-    values = [1, 4, 7]
-    for repl, value in enumerate(values):
-        m1.add(repl, value)
-    assert m1.ave() == np.average(values)
-    assert m1.std() == np.std(values)
-    assert m1() == m1.ave()
-    # %%
-    m2 = Measure()
-    values = [[1, 4, 5], [2, 6, 7], [3, 8, 9]]
-    ave = [2, 6, 7]
-    std = 0
-    for repl, value in enumerate(values):
-        m2.add(repl, value)
-    print(m2.ave())
-    print(m2.std())
-
-    # %%
-    proj = Project(test_dir, name="test", temp_unit="K")
-    # %%
-    cell = Sample(
-        project=proj,
-        name="cell",
-        filenames=["CLSOx5_1", "CLSOx5_2", "CLSOx5_3"],
-        time_moist=38,
-        time_vm=None,
-    )
-    mf = cell.plot_tg_dtg(x_ticklabels_rotation=0)
-    # %%
-    #
-    # %%
-    # misc = Sample(
-    #     project=proj, name="misc", filenames=["MIS_1", "MIS_2", "MIS_3"], time_moist=38, time_vm=147
-    # )
-    proj = Project(test_dir, name="test", temp_unit="C")
-    sda = Sample(
-        project=proj, name="sda", filenames=["SDa_1", "SDa_2", "SDa_3"], time_moist=38, time_vm=None
-    )
-    sdb = Sample(
-        project=proj, name="sdb", filenames=["SDb_1", "SDb_2", "SDb_3"], time_moist=38, time_vm=None
-    )
-    # %%
-    proj.plot_multi_soliddist(labels=["sample 1", "sample 2", "c"])
-    # %%
-    sda.plot_soliddist()
-    rep = proj.multireport(report_type="soliddist")
-    rep = proj.plot_multireport(
-        report_type="soliddist",
-        legend_loc="upper center",
-        color_palette="rocket",
-        color_palette_n_colors=7,
-    )
-    # %%
-    # dig = Sample(
-    #     project=proj, name="dig", filenames=["DIG10_1", "DIG10_2", "DIG10_3"], time_moist=22, time_vm=98
-    # )
-    # # %%
-    # for sample in proj.samples.values():
-    #     for report_type in [
-    #         "proximate",
-    #         "oxidation",
-    #         "oxidation_extended",
-    #         "soliddist",
-    #         "soliddist_extended",
-    #     ]:
-    #         sample.report(report_type)
-    #     mf = sample.plot_tg_dtg()
-
-    # # %%
-    # mf = sda.plot_soliddist()
-
-    # mf = sdb.plot_soliddist()
-    # # %%
-    # misc.deconv_analysis([280 + 273, 380 + 273])
-    # cell.deconv_analysis([310 + 273, 450 + 273, 500 + 273])
-    # mf = misc.plot_deconv()
-    # mf = cell.plot_deconv()
-    # # %%
-    # for report_type in [
-    #     "proximate",
-    #     "oxidation",
-    #     "oxidation_extended",
-    #     "soliddist",
-    #     # "soliddist_extended",  # not supported
-    # ]:
-    #     for report_style in ["repl_ave_std", "ave_std", "ave_pm_std"]:
-    #         print(f"{report_type = }, {report_style = }")
-    #         proj.multi_report(report_type=report_type, report_style=report_style)
-
-    # %%
-    cell_ox5 = Sample(
-        project=proj,
-        name="cell_ox5",
-        filenames=["CLSOx5_1", "CLSOx5_2", "CLSOx5_3"],
-        time_moist=38,
-        time_vm=None,
-        heating_rate_deg_min=5,
-    )
-    cell_ox10 = Sample(
-        project=proj,
-        name="cell_ox10",
-        load_skiprows=8,
-        filenames=["CLSOx10_2", "CLSOx10_3"],
-        time_moist=38,
-        time_vm=None,
-        heating_rate_deg_min=10,
-    )
-    cell_ox50 = Sample(
-        project=proj,
-        name="cell_ox50",
-        load_skiprows=8,
-        filenames=["CLSOx50_4", "CLSOx50_5"],
-        time_moist=38,
-        time_vm=None,
-        heating_rate_deg_min=50,
-    )
-    # %%
-    # kas_cell = proj.kas_analysis(samplenames=["cell_ox5", "cell_ox10", "cell_ox50"])
-    # %%
-    rep = proj.plot_multireport(
-        report_type="proximate",
-        x_ticklabels_rotation=30,
-        legend_loc="best",
-        legend_bbox_xy=(1, 1.01),
-    )
-    # %%
-    rep = proj.plot_multireport(report_type="oxidation", x_ticklabels_rotation=0)
-    # %%
-
-    # %%
```

### Comparing `tga_data_analysis-2.0.2/src/tga_data_analysis.egg-info/PKG-INFO` & `tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tga_data_analysis
-Version: 2.0.2
+Version: 2.0.4
 Summary: Tool for automatic analysis of multiple TGA results
 Author: Matteo Pecchi
 License: MIT
 Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
 Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tga_data_analysis-2.0.2/tests/test_measure.py` & `tga_data_analysis-2.0.4/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.2/tests/test_tga.py` & `tga_data_analysis-2.0.4/tests/test_tga.py`

 * *Files identical despite different names*

