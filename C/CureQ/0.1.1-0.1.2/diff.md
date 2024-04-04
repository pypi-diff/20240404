# Comparing `tmp/CureQ-0.1.1.tar.gz` & `tmp/CureQ-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CureQ-0.1.1.tar", last modified: Thu Apr  4 11:28:07 2024, max compression
+gzip compressed data, was "CureQ-0.1.2.tar", last modified: Thu Apr  4 13:19:58 2024, max compression
```

## Comparing `CureQ-0.1.1.tar` & `CureQ-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:28:07.754083 CureQ-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:28:07.725318 CureQ-0.1.1/CureQ/
--rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.1.1/CureQ/__init__.py
--rw-rw-rw-   0        0        0    63598 2024-04-04 11:27:27.000000 CureQ-0.1.1/CureQ/mea.py
--rw-rw-rw-   0        0        0    41237 2024-04-02 11:23:38.000000 CureQ-0.1.1/CureQ/mea_02_04.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:28:07.750082 CureQ-0.1.1/CureQ.egg-info/
--rw-rw-rw-   0        0        0     1529 2024-04-04 11:28:06.000000 CureQ-0.1.1/CureQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-04-04 11:28:07.000000 CureQ-0.1.1/CureQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:28:06.000000 CureQ-0.1.1/CureQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2024-04-04 11:28:06.000000 CureQ-0.1.1/CureQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-04 11:28:06.000000 CureQ-0.1.1/CureQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1529 2024-04-04 11:28:07.752082 CureQ-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      708 2024-03-19 15:09:22.000000 CureQ-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 11:28:07.754083 CureQ-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1631 2024-04-04 10:35:19.000000 CureQ-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:19:58.316933 CureQ-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-04 13:19:58.284835 CureQ-0.1.2/CureQ/
+-rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.1.2/CureQ/__init__.py
+-rw-rw-rw-   0        0        0    63693 2024-04-04 11:36:48.000000 CureQ-0.1.2/CureQ/mea.py
+-rw-rw-rw-   0        0        0    41237 2024-04-02 11:23:38.000000 CureQ-0.1.2/CureQ/mea_02_04.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:19:58.312929 CureQ-0.1.2/CureQ.egg-info/
+-rw-rw-rw-   0        0        0     3338 2024-04-04 13:19:57.000000 CureQ-0.1.2/CureQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-04-04 13:19:57.000000 CureQ-0.1.2/CureQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 13:19:57.000000 CureQ-0.1.2/CureQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-04-04 13:19:57.000000 CureQ-0.1.2/CureQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-04 13:19:57.000000 CureQ-0.1.2/CureQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3338 2024-04-04 13:19:58.314929 CureQ-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2574 2024-04-04 13:18:54.000000 CureQ-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 13:19:58.317934 CureQ-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1631 2024-04-04 11:37:00.000000 CureQ-0.1.2/setup.py
```

### Comparing `CureQ-0.1.1/CureQ/mea.py` & `CureQ-0.1.2/CureQ/mea.py`

 * *Files 0% similar despite different names*

```diff
@@ -1205,15 +1205,15 @@
         print("Creating raster plots")
         raster(electrodes, electrode_amnt, data.shape[1], hertz, filename)
 
     # Calculate the features
     print("Calculating features")
     features_df=features(filename, electrodes, electrode_amnt, data.shape[1], hertz)
 
-    # Adds a final plt.show() to show all plots during runtime (otherwise every figure needs to be closed individually to continue the program)
+    # Adds a final plt.show() to show all plots at the end of the program instead of during runtime (otherwise every figure needs to be closed manually closed to continue the program)
     if raster_plot:
         return features_df, data.shape[1], plt.show()
     else:
         return features_df, data.shape[1]
 
 
 '''Analyse an entire well'''
@@ -1258,9 +1258,9 @@
                         minspikes_burst, maxISI_outliers, default_threshold, heightexception, max_boxheight, amplitude_drop_sd, stdevmultiplier, RMSmultiplier, raster_plot=False)
         print(f"Calculating network bursts of well: {well}")
         network_burst_detection(filename, [well], electrode_amnt, measurements, hertz, min_channels, threshold_method)
         fancyplot(filename, [well], electrode_amnt, measurements, hertz, resolution, kernel_size, aspectratios, colormap)
         print(output)
         all_features.append(output)
 
-    # Adds a final plt.show() to show all plots during runtime (otherwise every figure will be closed at the end of the program)
+    # Adds a final plt.show() to show all plots at the end of the program instead of during runtime (otherwise every figure needs to be closed manually closed to continue the program)
     return all_features, plt.show()
```

### Comparing `CureQ-0.1.1/CureQ/mea_02_04.py` & `CureQ-0.1.2/CureQ/mea_02_04.py`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.1/LICENSE` & `CureQ-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.1/setup.py` & `CureQ-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Use the text in the README file for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Setup metadata for initializing the library
 setuptools.setup(
     name="CureQ",
-    version="0.1.1",
+    version="0.1.2",
     author="CureQ",
     author_email="cureq-ft@hva.nl",
     description="Library for analyzing MEA files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CureQ/CureQ.git",
     packages=setuptools.find_packages(),
```

