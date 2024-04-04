# Comparing `tmp/CureQ-0.1.0.tar.gz` & `tmp/CureQ-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CureQ-0.1.0.tar", last modified: Thu Apr  4 10:25:38 2024, max compression
+gzip compressed data, was "CureQ-0.1.1.tar", last modified: Thu Apr  4 11:28:07 2024, max compression
```

## Comparing `CureQ-0.1.0.tar` & `CureQ-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:25:38.475905 CureQ-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-04 10:25:38.444243 CureQ-0.1.0/CureQ/
--rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.1.0/CureQ/__init__.py
--rw-rw-rw-   0        0        0    62828 2024-04-04 10:16:10.000000 CureQ-0.1.0/CureQ/mea.py
--rw-rw-rw-   0        0        0    41237 2024-04-02 11:23:38.000000 CureQ-0.1.0/CureQ/mea_02_04.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:25:38.475905 CureQ-0.1.0/CureQ.egg-info/
--rw-rw-rw-   0        0        0     1529 2024-04-04 10:25:37.000000 CureQ-0.1.0/CureQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-04-04 10:25:38.000000 CureQ-0.1.0/CureQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:25:37.000000 CureQ-0.1.0/CureQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2024-04-04 10:25:37.000000 CureQ-0.1.0/CureQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-04 10:25:37.000000 CureQ-0.1.0/CureQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1529 2024-04-04 10:25:38.475905 CureQ-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      708 2024-03-19 15:09:22.000000 CureQ-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 10:25:38.475905 CureQ-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1631 2024-04-04 08:45:28.000000 CureQ-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:28:07.754083 CureQ-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-04-04 11:28:07.725318 CureQ-0.1.1/CureQ/
+-rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.1.1/CureQ/__init__.py
+-rw-rw-rw-   0        0        0    63598 2024-04-04 11:27:27.000000 CureQ-0.1.1/CureQ/mea.py
+-rw-rw-rw-   0        0        0    41237 2024-04-02 11:23:38.000000 CureQ-0.1.1/CureQ/mea_02_04.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:28:07.750082 CureQ-0.1.1/CureQ.egg-info/
+-rw-rw-rw-   0        0        0     1529 2024-04-04 11:28:06.000000 CureQ-0.1.1/CureQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-04-04 11:28:07.000000 CureQ-0.1.1/CureQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 11:28:06.000000 CureQ-0.1.1/CureQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-04-04 11:28:06.000000 CureQ-0.1.1/CureQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-04 11:28:06.000000 CureQ-0.1.1/CureQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1529 2024-04-04 11:28:07.752082 CureQ-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2024-03-19 15:09:22.000000 CureQ-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 11:28:07.754083 CureQ-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1631 2024-04-04 10:35:19.000000 CureQ-0.1.1/setup.py
```

### Comparing `CureQ-0.1.0/CureQ/mea.py` & `CureQ-0.1.1/CureQ/mea.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Version 0.1.0
+# Version 0.1.1
 
 '''This file contains the entire MEA_analyzer pipeline, contained in functions'''
 # Imports
 import numpy as np
 import matplotlib.pyplot as plt 
 from scipy.signal import butter, lfilter
 from scipy.stats import norm
@@ -179,14 +179,16 @@
     # Calculate MEA electrode
     electrode = i % electrode_amnt + 1
     well = round(i / electrode_amnt + 0.505)
 
     #Plot the data of the entire electrode
     if plot_validation:
         #%matplotlib widget
+        # Creates a new figure for every plot in the program
+        plt.figure()
         # Plot the MEA signal
         plt.cla()
 
         # Enlarge size of plot figure
         plt.rcParams["figure.figsize"] = (22,5)
 
         time_seconds = np.arange(0, data[i].shape[0]) / hertz
@@ -208,15 +210,14 @@
 
         # Plot layout
         plt.title(f"Well {well} - MEA electrode {electrode} - Threshold: {threshold} - Spikes detected before DMP: {np.sum(spikes_before_DMP)}, after: {np.sum(spikes)}")
         plt.xlabel("Time in seconds")
         plt.ylabel("Micro voltage")
         plt.xlim([time_seconds.min(), time_seconds.max()])
         plt.ylim([np.min(data[i])-100, np.max(data[i])+100])
-        plt.show()
     
     # Save the spike data to a .csv file
     if True:
         mapname=(os.path.basename(filename).split('/')[-1])
         mapname=mapname[:-3]
         mapname=mapname+'_values'
         filename=filename[:-3]
@@ -301,14 +302,16 @@
             # For negative spikes
                 if not(np.max(data[j-exit_time:j+exit_time+1])>(data[j]+thresholdmultiplier*threshold)):
                     # Spikes that have an amplitude of twice the threshold, do not have to drop amplitude in a short time
                     if not(data[j]<heightexception*-1*threshold):
                         # If not, the spike will be removed
                         spikes[j]=False
     if plot_validation:
+        # Creates a new figure for every plot in the program
+        plt.figure()
         # Plot the MEA signal
         plt.cla()
 
         time_seconds = np.arange(0, data.shape[0]) / hertz
         plt.plot(time_seconds, data, linewidth=0.2, zorder=-1)
         
         # Plot the threshold
@@ -329,15 +332,14 @@
         # Enlarge size of plot figure
         plt.rcParams["figure.figsize"] = (10,5)
         plt.title(f"Dataset: Nature - Well: {well} - Electrode: {electrode_nr} - Threshold: {threshold} - Spikes detected before DMP: {np.sum(spikes_before_DMP)}, after: {np.sum(spikes)}")
         plt.xlabel("Time in seconds")
         plt.ylabel("Micro voltage")
         plt.xlim([time_seconds.min(), time_seconds.max()])
         plt.ylim([np.min(data)*1.2, np.max(data)*1.2])
-        plt.show()
     # Save the spike data to a .csv file
     if True:
         filename=filename[:-3]
         filename=filename+"_values"
         if not os.path.exists(filename):
             os.makedirs(filename)
         path = f'{filename}/spike_values'
@@ -444,26 +446,27 @@
                     ISIth2=ISIth2_max
                 use_pasquale=True
                 use_ISIth2=True
                 print(f"2 valid peaks detected in smoothed ISI histogram at well {well}, electrode {electrode}, using advanced burst detection algorithm with ISIth1 set at {ISIth1} and ISIth2 set at {ISIth2}")
             
         # Plot the smoothed histogram
         if True:
+            # Creates a new figure for every plot in the program
+            plt.figure()
             plt.scatter(x[peaks], y[peaks], color="red")
             if valid_peaks:
                 plt.scatter(valley_x, y[np.where(y==g_min)])
                 if use_ISIth2:
                     plt.axvline(ISIth2, color='blue')
             plt.axvline(ISIth1, color='green')
             plt.scatter
             plt.gca().set_xscale("log")
             plt.title(f"Well: { well}, Electrode: {electrode}")
             plt.xlabel("Inter-spike interval")
             plt.ylabel("Amount")
-            plt.show()
 
         # Apply the threshold
         burst_cores=[]
         burst_spikes=[]
         burst_counter=0
 
         # The seemingly random +1 and -1 in the following code
@@ -575,14 +578,16 @@
                     del burst_cores[i+1]
                 else:
                     i+=1
             #print(f"Bursts after combining: {len(burst_cores)}")
 
         # Plot the data and mark the bursts
         if True:
+            # Creates a new figure for every plot in the program
+            plt.figure()
             #%matplotlib widget
             plt.cla()
             plt.clf()
 
             # Plot the data
             time_seconds = np.arange(0, data[electrode_number].shape[0]) / hertz
             plt.plot(time_seconds, data[electrode_number], linewidth=0.2, zorder=-1)
@@ -613,15 +618,14 @@
             else:
                 thresholdtext=f"Default burst detection, ISIth1: {ISIth1}"
             plt.title(f"Well {well} - MEA electrode {electrode}, bursts detected: {len(burst_cores)}, index: {electrode_number}, min_spikes: {minspikes_burst}, {thresholdtext}")
             plt.xlabel("Time in seconds")
             plt.ylabel("Micro voltage")
             plt.xlim([time_seconds.min(), time_seconds.max()])
             plt.ylim([np.min(data[electrode_number])-100, np.max(data[electrode_number])+100])
-            plt.show()
     else:
         print(f"No burst detection possible for well {well}, electrode {electrode} - not enough values")
         burst_spikes=[]
         burst_cores=[]
     # Save the spike data to a .csv file
     if True:
         if not os.path.exists(filename):
@@ -697,28 +701,29 @@
             if len(burstdata)>0:
                 burst_spikes.append(burstdata[:,0])
             else:
                 burst_spikes.append([])
             if ((electrodes[i]+1)%electrode_amnt)==0: break
             i+=1
         amount_of_electrodes=len(burst_spikes)
+        # Creates a new figure for every plot in the program
+        plt.figure()
         plt.cla()
         plt.rcParams["figure.figsize"] = (22,5)
         end_electrode=((electrodes[i-1]+1)%12)+1
         start_electrode = end_electrode-amount_of_electrodes
         lineoffsets1=np.arange(start_electrode+1, end_electrode+1)
         plt.eventplot(well_spikes, alpha=0.5, lineoffsets=lineoffsets1)
         plt.eventplot(burst_spikes, alpha=0.5, color='red', lineoffsets=lineoffsets1)
         plt.xlim([0,samples/hertz])
         plt.ylim([start_electrode, end_electrode+1])
         plt.yticks(lineoffsets1)
         plt.title(f"Well {well}")
         plt.xlabel("Time in seconds")
         plt.ylabel("Electrode")
-        plt.show()
         i+=1
 
 '''Takes two burst values and calculates whether they overlap or not'''
 def overlap(burst1, burst2):
     if burst1[1]<burst2[0] or burst2[1]<burst1[0]:
         return False
     else:
@@ -733,14 +738,16 @@
     burstpath=f'{filename}/burst_values'
 
     min_channels=round(min_channels*electrode_amnt)
     print(f"Minimal amount of channels required for network burst: {min_channels}")
     total_network_burst=[]
     
     for well in wells:
+        # Creates a new figure for every plot in the program
+        plt.figure()
         fig, ax = plt.subplots(4,1, sharex=True, figsize=(16,5), gridspec_kw={'height_ratios': [3, 1, 1, 1]})
         ax[1].set_ylabel("Burst\namount")
         ax[0].set_xlim([0,measurements/hertz])
         ax[0].set_ylim([0,electrode_amnt+1])
         ax[0].set_yticks(np.arange(1, electrode_amnt+1, 1))
         ax[3].set_xlabel("Time in seconds")
         ax[1].set_ylim([0, electrode_amnt+1])
@@ -865,15 +872,14 @@
                     graph.axvspan(temp[2], temp[3], facecolor='green', alpha=0.5)
             # # Add rectangles to the top graph
             # for network_burst in network_burst_cores:
             #     ax[0].add_patch(Rectangle((network_burst[0], 0.5), network_burst[1]-network_burst[0], electrode_amnt, edgecolor='green', facecolor='none', linewidth=2, zorder=10))
                     
             ax[2].set_ylabel("Spike\nactivity\n(KDE)")
             ax[3].set_ylabel("Burst\nspike\nactivity\n(KDE)")
-            plt.show()
         else:
             total_network_burst.append([[]])
     path = f'{filename}/network_data'
     if not os.path.exists(path):
         os.makedirs(path)
     np.savetxt(f'{path}/well_{well}_network_bursts.csv', total_network_burst, delimiter = ",")
     np.save(f'{path}/well_{well}_network_bursts', total_network_burst)
@@ -1198,15 +1204,21 @@
     if raster_plot:
         print("Creating raster plots")
         raster(electrodes, electrode_amnt, data.shape[1], hertz, filename)
 
     # Calculate the features
     print("Calculating features")
     features_df=features(filename, electrodes, electrode_amnt, data.shape[1], hertz)
-    return features_df, data.shape[1]
+
+    # Adds a final plt.show() to show all plots during runtime (otherwise every figure needs to be closed individually to continue the program)
+    if raster_plot:
+        return features_df, data.shape[1], plt.show()
+    else:
+        return features_df, data.shape[1]
+
 
 '''Analyse an entire well'''
 def analyse_well(filename,                                  # Where is the data file stored
                       wells,                                # Which wells do you want to analyze
                       hertz,                                # What is the sampling frequency of the MEA
                       validation_method="DMP_noisebased",   # Which validation method do you want to use, possible: "DMP", "DMP_noisebased"
                       low_cutoff=200,                       # The low_cutoff for the bandpass filter
@@ -1245,8 +1257,10 @@
         output, measurements=analyse_electrode(filename, electrodes, hertz, validation_method, low_cutoff, high_cutoff, order, spikeduration, exit_time_s, amplitude_drop_threshold, plot_validation, well_amnt, electrode_amnt, kde_bandwidth, smallerneighbours,
                         minspikes_burst, maxISI_outliers, default_threshold, heightexception, max_boxheight, amplitude_drop_sd, stdevmultiplier, RMSmultiplier, raster_plot=False)
         print(f"Calculating network bursts of well: {well}")
         network_burst_detection(filename, [well], electrode_amnt, measurements, hertz, min_channels, threshold_method)
         fancyplot(filename, [well], electrode_amnt, measurements, hertz, resolution, kernel_size, aspectratios, colormap)
         print(output)
         all_features.append(output)
-    return all_features
+
+    # Adds a final plt.show() to show all plots during runtime (otherwise every figure will be closed at the end of the program)
+    return all_features, plt.show()
```

### Comparing `CureQ-0.1.0/CureQ/mea_02_04.py` & `CureQ-0.1.1/CureQ/mea_02_04.py`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.0/CureQ.egg-info/PKG-INFO` & `CureQ-0.1.1/CureQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CureQ
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for analyzing MEA files.
 Home-page: https://github.com/CureQ/CureQ.git
 Author: CureQ
 Author-email: cureq-ft@hva.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `CureQ-0.1.0/LICENSE` & `CureQ-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.0/PKG-INFO` & `CureQ-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CureQ
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for analyzing MEA files.
 Home-page: https://github.com/CureQ/CureQ.git
 Author: CureQ
 Author-email: cureq-ft@hva.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `CureQ-0.1.0/README.md` & `CureQ-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `CureQ-0.1.0/setup.py` & `CureQ-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Use the text in the README file for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Setup metadata for initializing the library
 setuptools.setup(
     name="CureQ",
-    version="0.1.0",
+    version="0.1.1",
     author="CureQ",
     author_email="cureq-ft@hva.nl",
     description="Library for analyzing MEA files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CureQ/CureQ.git",
     packages=setuptools.find_packages(),
```

