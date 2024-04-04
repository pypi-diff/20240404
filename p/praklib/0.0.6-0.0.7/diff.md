# Comparing `tmp/praklib-0.0.6.tar.gz` & `tmp/praklib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.0.6.tar", last modified: Thu Apr  4 14:47:57 2024, max compression
+gzip compressed data, was "praklib-0.0.7.tar", last modified: Thu Apr  4 14:55:45 2024, max compression
```

## Comparing `praklib-0.0.6.tar` & `praklib-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:47:57.602351 praklib-0.0.6/
--rw-rw-rw-   0        0        0      313 2024-04-04 14:47:57.601345 praklib-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 14:47:57.590722 praklib-0.0.6/praklib/
--rw-rw-rw-   0        0        0     4221 2024-04-04 14:42:09.000000 praklib-0.0.6/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.6/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:47:57.599244 praklib-0.0.6/praklib.egg-info/
--rw-rw-rw-   0        0        0      313 2024-04-04 14:47:57.000000 praklib-0.0.6/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-04 14:47:57.000000 praklib-0.0.6/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 14:47:57.000000 praklib-0.0.6/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 14:47:57.000000 praklib-0.0.6/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 14:47:57.602351 praklib-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      431 2024-04-04 14:47:09.000000 praklib-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:55:45.382887 praklib-0.0.7/
+-rw-rw-rw-   0        0        0      313 2024-04-04 14:55:45.381873 praklib-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 14:55:45.368878 praklib-0.0.7/praklib/
+-rw-rw-rw-   0        0        0     4295 2024-04-04 14:55:35.000000 praklib-0.0.7/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.7/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:55:45.380874 praklib-0.0.7/praklib.egg-info/
+-rw-rw-rw-   0        0        0      313 2024-04-04 14:55:45.000000 praklib-0.0.7/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-04 14:55:45.000000 praklib-0.0.7/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 14:55:45.000000 praklib-0.0.7/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 14:55:45.000000 praklib-0.0.7/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 14:55:45.382887 praklib-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      431 2024-04-04 14:55:44.000000 praklib-0.0.7/setup.py
```

### Comparing `praklib-0.0.6/praklib/Praktika.py` & `praklib-0.0.7/praklib/Praktika.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,35 +81,35 @@
     latex_table += "\\end{tabular}\n"
     latex_table += "\\caption{Values and their errors}\n"
     latex_table += "\\label{tab:values}\n"
     latex_table += "\\end{table}"
 
     return latex_table
 
-def plot_3d_graph(data, cmap='viridis', projection='ortho', fcl=1):
+def plot_3d_graph(data, xlabel = "X", ylabel = "Y", zlabel = "Z", cbarlabel = "height", cmap='viridis', projection='ortho', fcl=1):
 
     # Create meshgrid
     x = np.arange(data.shape[1])
     y = np.arange(data.shape[0])
     X, Y = np.meshgrid(x, y)
 
     # Create 3D plot
     fig = plt.figure()
     ax = fig.add_subplot(111, projection='3d')
 
     # Plot surface
     ax.plot_surface(X, Y, data, cmap='viridis')
 
     # Set labels
-    ax.set_xlabel('X')
-    ax.set_ylabel('Y')
-    ax.set_zlabel('Z')
+    ax.set_xlabel(xlabel)
+    ax.set_ylabel(ylabel)
+    ax.set_zlabel(zlabel)
 
     cbar = fig.colorbar(ax.collections[0], ax=ax, orientation='vertical')
-    cbar.set_label('Height')
+    cbar.set_label(cbarlabel)
 
     if projection=='ortho':
         ax.set_proj_type(projection)
     else:
         ax.set_proj_type(projection, focal_length=fcl)
 
     # Show plot
```

