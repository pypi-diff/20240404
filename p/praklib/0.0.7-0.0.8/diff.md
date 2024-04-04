# Comparing `tmp/praklib-0.0.7.tar.gz` & `tmp/praklib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.0.7.tar", last modified: Thu Apr  4 14:55:45 2024, max compression
+gzip compressed data, was "praklib-0.0.8.tar", last modified: Thu Apr  4 15:06:11 2024, max compression
```

## Comparing `praklib-0.0.7.tar` & `praklib-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:55:45.382887 praklib-0.0.7/
--rw-rw-rw-   0        0        0      313 2024-04-04 14:55:45.381873 praklib-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 14:55:45.368878 praklib-0.0.7/praklib/
--rw-rw-rw-   0        0        0     4295 2024-04-04 14:55:35.000000 praklib-0.0.7/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.7/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:55:45.380874 praklib-0.0.7/praklib.egg-info/
--rw-rw-rw-   0        0        0      313 2024-04-04 14:55:45.000000 praklib-0.0.7/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-04 14:55:45.000000 praklib-0.0.7/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 14:55:45.000000 praklib-0.0.7/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 14:55:45.000000 praklib-0.0.7/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 14:55:45.382887 praklib-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      431 2024-04-04 14:55:44.000000 praklib-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:06:11.316893 praklib-0.0.8/
+-rw-rw-rw-   0        0        0      261 2024-04-04 15:06:11.315880 praklib-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 15:06:11.300974 praklib-0.0.8/praklib/
+-rw-rw-rw-   0        0        0     4268 2024-04-04 15:05:36.000000 praklib-0.0.8/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.8/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:06:11.314563 praklib-0.0.8/praklib.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-04-04 15:06:11.000000 praklib-0.0.8/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-04 15:06:11.000000 praklib-0.0.8/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:06:11.000000 praklib-0.0.8/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 15:06:11.000000 praklib-0.0.8/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:06:11.316893 praklib-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-04-04 15:06:10.000000 praklib-0.0.8/setup.py
```

### Comparing `praklib-0.0.7/praklib/Praktika.py` & `praklib-0.0.8/praklib/Praktika.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from lmfit import Model
 
-def graf_bez_fitu(x, y, errx, erry, xlabel, ylabel, linelabel, scatterlabel,
+def graf(x, y, errx, erry, xlabel, ylabel, linelabel, scatterlabel,
                 grid=True, show=True, scatter=True, line=False, err=True):
     plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
     data1 = np.arange(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1],
                       (x[len(x) - 1] + errx[len(x) - 1] - x[0] - errx[0]) / 100, dtype=np.double)
     if (grid == True):
         plt.grid(True, linestyle="dashed")
     plt.xlabel(xlabel)
@@ -34,15 +34,15 @@
 
     param_names = list(results.params.keys())
     param_values = [results.params[name].value for name in param_names]
     param_errors = [results.params[name].stderr if results.params[name].stderr else 0 for name in param_names]
 
     return param_names, param_values, param_errors
 
-def graf_z_fitu(x, y, fit_vstup, fit_vystup, errx, erry, xlabel, ylabel, linelabel, scatterlabel, params_fit,
+def graf_fit(x, y, fit_vstup, fit_vystup, errx, erry, xlabel, ylabel, linelabel, scatterlabel, params_fit,
                 fit_function, grid=True, show=True, scatter=True):
     plt.xlim(x[0]-errx[0], x[-1]+errx[-1])
     data1 = np.linspace(x[0]-errx[0], x[-1]+errx[-1], 100)
 
     param_names, param_values, param_errors = fit_data(fit_vstup, fit_vystup, params_fit, fit_function, show_results=False)
     funkcni_param = np.array(param_values) + 1j * np.array(param_errors)
     params = dict(zip(param_names, funkcni_param))
@@ -59,15 +59,15 @@
         plt.scatter(x, y, s=5, facecolor="red", marker='x', zorder=2, label=scatterlabel)
     plt.errorbar(x, y, xerr=errx, yerr=erry, zorder=1, capsize=2, fmt='none',
                  ecolor="red", linewidth=1.0)
     plt.legend()
     plt.show()
 
 
-def generate_latex_table(data, col_names):
+def latex_table(data, col_names):
     num_rows = len(data)
     num_cols = len(data[0])
 
     latex_table = "\\begin{table}[h!]\n"
     latex_table += "\\centering\n"
     latex_table += "\\begin{tabular}{|" + "|".join(["c"] * (num_cols)) + "|}\n"
     latex_table += "\\hline\n"
@@ -81,15 +81,15 @@
     latex_table += "\\end{tabular}\n"
     latex_table += "\\caption{Values and their errors}\n"
     latex_table += "\\label{tab:values}\n"
     latex_table += "\\end{table}"
 
     return latex_table
 
-def plot_3d_graph(data, xlabel = "X", ylabel = "Y", zlabel = "Z", cbarlabel = "height", cmap='viridis', projection='ortho', fcl=1):
+def graf_3d(data, xlabel = "X", ylabel = "Y", zlabel = "Z", cbarlabel = "height", cmap='viridis', projection='ortho', fcl=1):
 
     # Create meshgrid
     x = np.arange(data.shape[1])
     y = np.arange(data.shape[0])
     X, Y = np.meshgrid(x, y)
 
     # Create 3D plot
```

