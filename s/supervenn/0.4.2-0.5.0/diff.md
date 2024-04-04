# Comparing `tmp/supervenn-0.4.2.tar.gz` & `tmp/supervenn-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/supervenn-0.4.2.tar", last modified: Sat Oct  7 15:05:32 2023, max compression
+gzip compressed data, was "dist/supervenn-0.5.0.tar", last modified: Thu Apr  4 09:29:42 2024, max compression
```

## Comparing `supervenn-0.4.2.tar` & `supervenn-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 indukaev (1026181036) LD\Domain Users (593637566)        0 2023-10-07 15:05:32.000000 supervenn-0.4.2/
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)      917 2023-10-07 15:05:32.000000 supervenn-0.4.2/PKG-INFO
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)     1071 2023-10-07 12:46:43.000000 supervenn-0.4.2/LICENSE
-drwxr-xr-x   0 indukaev (1026181036) LD\Domain Users (593637566)        0 2023-10-07 15:05:32.000000 supervenn-0.4.2/supervenn/
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)    22236 2023-10-07 12:46:43.000000 supervenn-0.4.2/supervenn/_algorithms.py
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)      137 2023-10-07 12:46:43.000000 supervenn-0.4.2/supervenn/__init__.py
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)    22227 2023-10-07 15:01:55.000000 supervenn-0.4.2/supervenn/_plots.py
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)    17241 2023-10-07 12:46:43.000000 supervenn-0.4.2/README.md
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)     1250 2023-10-07 15:04:31.000000 supervenn-0.4.2/setup.py
-drwxr-xr-x   0 indukaev (1026181036) LD\Domain Users (593637566)        0 2023-10-07 15:05:32.000000 supervenn-0.4.2/supervenn.egg-info/
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)      917 2023-10-07 15:05:32.000000 supervenn-0.4.2/supervenn.egg-info/PKG-INFO
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)      257 2023-10-07 15:05:32.000000 supervenn-0.4.2/supervenn.egg-info/SOURCES.txt
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)       24 2023-10-07 15:05:32.000000 supervenn-0.4.2/supervenn.egg-info/requires.txt
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)       10 2023-10-07 15:05:32.000000 supervenn-0.4.2/supervenn.egg-info/top_level.txt
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)        1 2023-10-07 15:05:32.000000 supervenn-0.4.2/supervenn.egg-info/dependency_links.txt
--rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)       38 2023-10-07 15:05:32.000000 supervenn-0.4.2/setup.cfg
+drwxr-xr-x   0 indukaev (1026181036) LD\Domain Users (593637566)        0 2024-04-04 09:29:42.000000 supervenn-0.5.0/
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)     1069 2024-04-04 09:29:42.000000 supervenn-0.5.0/PKG-INFO
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)     1071 2023-10-07 12:46:43.000000 supervenn-0.5.0/LICENSE
+drwxr-xr-x   0 indukaev (1026181036) LD\Domain Users (593637566)        0 2024-04-04 09:29:42.000000 supervenn-0.5.0/supervenn/
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)    22236 2023-10-07 12:46:43.000000 supervenn-0.5.0/supervenn/_algorithms.py
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)      192 2024-04-04 08:31:00.000000 supervenn-0.5.0/supervenn/__init__.py
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)     3206 2024-04-04 09:24:14.000000 supervenn-0.5.0/supervenn/_utils.py
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)    22227 2024-04-04 08:33:26.000000 supervenn-0.5.0/supervenn/_plots.py
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)    18576 2024-04-04 09:11:04.000000 supervenn-0.5.0/README.md
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)     1407 2024-04-04 09:10:39.000000 supervenn-0.5.0/setup.py
+drwxr-xr-x   0 indukaev (1026181036) LD\Domain Users (593637566)        0 2024-04-04 09:29:42.000000 supervenn-0.5.0/supervenn.egg-info/
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)     1069 2024-04-04 09:29:42.000000 supervenn-0.5.0/supervenn.egg-info/PKG-INFO
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)      277 2024-04-04 09:29:42.000000 supervenn-0.5.0/supervenn.egg-info/SOURCES.txt
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)       31 2024-04-04 09:29:42.000000 supervenn-0.5.0/supervenn.egg-info/requires.txt
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)       10 2024-04-04 09:29:42.000000 supervenn-0.5.0/supervenn.egg-info/top_level.txt
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)        1 2024-04-04 09:29:42.000000 supervenn-0.5.0/supervenn.egg-info/dependency_links.txt
+-rw-r--r--   0 indukaev (1026181036) LD\Domain Users (593637566)       38 2024-04-04 09:29:42.000000 supervenn-0.5.0/setup.cfg
```

### Comparing `supervenn-0.4.2/PKG-INFO` & `supervenn-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 1.1
 Name: supervenn
-Version: 0.4.2
+Version: 0.5.0
 Summary: supervenn is a tool for visualization of relations of many sets using matplotlib
 Home-page: https://github.com/gecko984/supervenn
 Author: Fedor Indukaev
 Author-email: gecko984@gmail.com
 License: MIT
 Description: See https://github.com/gecko984/supervenn/blob/master/README.md
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `supervenn-0.4.2/LICENSE` & `supervenn-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `supervenn-0.4.2/supervenn/_algorithms.py` & `supervenn-0.5.0/supervenn/_algorithms.py`

 * *Files identical despite different names*

### Comparing `supervenn-0.4.2/supervenn/_plots.py` & `supervenn-0.5.0/supervenn/_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
             'or plot into an existing axis by passing it as the ax argument:\n'
             '    supervenn(sets, ax=my_axis)\n'
         )
 
     axes = setup_axes(side_plots, figsize, dpi, ax, side_plot_width)
 
     if set_annotations is None:
-        set_annotations = ['Set_{}'.format(i) for i in range(len(sets))]
+        set_annotations = ['set_{}'.format(i) for i in range(len(sets))]
 
     chunks, composition_array = get_chunks_and_composition_array(sets)
 
     # Find permutations of rows and columns
     permutations_ = get_permutations(
         chunks,
         composition_array,
```

### Comparing `supervenn-0.4.2/README.md` & `supervenn-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 <img src="https://i.imgur.com/dJoNhYQ.png" width=800>
 
 ### Installation
 `pip install supervenn`
 
 ### Requirements
-Python 2.7 or 3.6+ with `numpy` and`matplotlib`.
+Python 2.7 or 3.6+ with `numpy`, `matplotlib` and `pandas`.
 
 ### Basic usage 
 The main entry point is the eponymous `supervenn` function. It takes a list of python `set`s as its first and only
 required argument and returns a `SupervennPlot` object.
 ```python
 from supervenn import supervenn
 sets = [{1, 2, 3, 4}, {3, 4, 5}, {1, 6, 7, 8}]
@@ -57,15 +57,47 @@
 <img src="https://i.imgur.com/9IhLBcK.png" width=330>
 Here, the numbers on the right are the set sizes (cardinalities), and numbers on the top show how many sets does this
 intersection make part of. The grey bars represent the same numbers visually.
 
 If you need only one of the two side plots, use `side_plots='top'` or `side_plots='right'`
 
 ### Features (how to)
-#### Add custom set annotations instead of 'Set_1', 'Set_2' etc
+
+#### Plot the chart if you don't have the sets themselves, but rather the intersection sizes
+Use the utility function `make_sets_from_chunk_sizes` to produce synthetic sets of integers from your intersection sizes,
+and then pass these sets to `supervenn()`. 
+
+```python
+from supervenn import supervenn, make_sets_from_chunk_sizes
+sets, labels = make_sets_from_chunk_sizes(sizes_df)  # see below for the structure of sizes_df
+supervenn(sets, labels)
+```
+
+Intersection sizes `sizes_df` should be a `pandas.DataFrame` with the following structure:
+
+- For `N` sets, it must have `N` boolean (or 0/1) columns and the last column must be integer, so `N+1` columns in total.
+- Each row represents a unique intersection (chunk) of the sets. The boolean value in column `set_x` indicate whether
+this chunk lies within `set_x`. The integer value represents the size of the chunk.
+
+For example, consider the following dataframe
+
+```
+   set_1  set_2  set_3  size
+0  False   True   True     1
+1   True  False  False     3
+2   True  False   True     2
+3   True   True  False     1
+```
+
+It represents a configuration of three sets such that
+- [row 0] there is one element that lies in `set_2` and `set_3` but not in `set_1`,
+- [row 1] there are three elements that lie in `set_1` only and not in `set_2` or `set_3`,
+- etc two more rows.
+
+#### Add custom set annotations instead of `set_1`, `set_2` etc
 Use the `set_annotations` argument to pass a list of annotations. It should be in the same order as the sets. It is
 the second positional argument.
 ```python
 sets = [{1, 2, 3, 4}, {3, 4, 5}, {1, 6, 7, 8}]
 labels = ['alice', 'bob', 'third party']
 supervenn(sets, labels)
 ```
```

### Comparing `supervenn-0.4.2/setup.py` & `supervenn-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 
 setuptools.setup(
     author='Fedor Indukaev',
     author_email='gecko984@gmail.com',
     name='supervenn',
     license='MIT',
     description='supervenn is a tool for visualization of relations of many sets using matplotlib',
-    version='0.4.2',
+    version='0.5.0',
     long_description='See https://github.com/gecko984/supervenn/blob/master/README.md',
     url='https://github.com/gecko984/supervenn',
     packages=setuptools.find_packages(),
-    install_requires=['numpy', 'matplotlib>=2.2.5'],
-    classifiers = [
+    install_requires=['numpy', 'matplotlib>=2.2.5', 'pandas'],
+    classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Visualization',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers'
     ]
 )
```

### Comparing `supervenn-0.4.2/supervenn.egg-info/PKG-INFO` & `supervenn-0.5.0/supervenn.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 1.1
 Name: supervenn
-Version: 0.4.2
+Version: 0.5.0
 Summary: supervenn is a tool for visualization of relations of many sets using matplotlib
 Home-page: https://github.com/gecko984/supervenn
 Author: Fedor Indukaev
 Author-email: gecko984@gmail.com
 License: MIT
 Description: See https://github.com/gecko984/supervenn/blob/master/README.md
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

