# Comparing `tmp/nwb4fp-0.5.9.2.tar.gz` & `tmp/nwb4fp-0.5.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.5.9.2.tar", last modified: Wed Apr  3 16:08:52 2024, max compression
+gzip compressed data, was "nwb4fp-0.5.9.3.tar", last modified: Thu Apr  4 12:04:16 2024, max compression
```

## Comparing `nwb4fp-0.5.9.2.tar` & `nwb4fp-0.5.9.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.860710 nwb4fp-0.5.9.2/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.5.9.2/LICENSE
--rw-rw-rw-   0        0        0     5786 2024-04-03 16:08:52.853705 nwb4fp-0.5.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.5.9.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 16:08:52.875706 nwb4fp-0.5.9.2/setup.cfg
--rw-rw-rw-   0        0        0      881 2024-04-03 16:08:30.000000 nwb4fp-0.5.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.325710 nwb4fp-0.5.9.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.387709 nwb4fp-0.5.9.2/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.5.9.2/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.485707 nwb4fp-0.5.9.2/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.5.9.2/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.5.9.2/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.336726 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1614 2024-02-21 21:21:29.000000 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1445 2024-03-03 15:56:30.000000 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    11580 2024-04-03 16:08:03.000000 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    11891 2024-04-01 17:16:46.000000 nwb4fp-0.5.9.2/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.340777 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.2/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.348726 nwb4fp-0.5.9.2/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.348726 nwb4fp-0.5.9.2/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.5.9.2/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1454 2024-04-03 09:24:14.000000 nwb4fp-0.5.9.2/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.5.9.2/src/nwb4fp/test/run_scripts/test.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:08:52.456711 nwb4fp-0.5.9.2/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5786 2024-04-03 16:08:52.000000 nwb4fp-0.5.9.2/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2024-04-03 16:08:52.000000 nwb4fp-0.5.9.2/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 16:08:52.000000 nwb4fp-0.5.9.2/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2916 2024-04-03 16:08:52.000000 nwb4fp-0.5.9.2/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 16:08:52.000000 nwb4fp-0.5.9.2/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:16.497750 nwb4fp-0.5.9.3/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.5.9.3/LICENSE
+-rw-rw-rw-   0        0        0     5786 2024-04-04 12:04:16.489759 nwb4fp-0.5.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.5.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:04:16.512760 nwb4fp-0.5.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      881 2024-04-04 12:02:29.000000 nwb4fp-0.5.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:15.641752 nwb4fp-0.5.9.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:15.659749 nwb4fp-0.5.9.3/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.5.9.3/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:15.650749 nwb4fp-0.5.9.3/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.5.9.3/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.5.9.3/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:15.654761 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1614 2024-02-21 21:21:29.000000 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1445 2024-03-03 15:56:30.000000 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17068 2024-04-04 12:02:21.000000 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    11891 2024-04-01 17:16:46.000000 nwb4fp-0.5.9.3/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:15.659749 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.5.9.3/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:15.681749 nwb4fp-0.5.9.3/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:16.461750 nwb4fp-0.5.9.3/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.5.9.3/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1454 2024-04-03 09:24:14.000000 nwb4fp-0.5.9.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.5.9.3/src/nwb4fp/test/run_scripts/test.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:04:15.861749 nwb4fp-0.5.9.3/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5786 2024-04-04 12:04:15.000000 nwb4fp-0.5.9.3/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2024-04-04 12:04:15.000000 nwb4fp-0.5.9.3/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:04:15.000000 nwb4fp-0.5.9.3/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2916 2024-04-04 12:04:15.000000 nwb4fp-0.5.9.3/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-04 12:04:15.000000 nwb4fp-0.5.9.3/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.5.9.2/LICENSE` & `nwb4fp-0.5.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/PKG-INFO` & `nwb4fp-0.5.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.5.9.2
+Version: 0.5.9.3
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.5.9.2/README.md` & `nwb4fp-0.5.9.3/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/setup.py` & `nwb4fp-0.5.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 setup(
     name='nwb4fp',
-    version='0.5.9.2',
+    version='0.5.9.3',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.5.9.3/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.5.9.3/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.5.9.3/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.5.9.3/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.5.9.3/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.5.9.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files 26% similar despite different names*

```diff
@@ -45,93 +45,171 @@
 
     ECEPHY_DATA_PATH = file[0]
     stream_name = 'Record Node 102#OE_FPGA_Acquisition_Board-101.Rhythm Data'
     folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
 
     down_sample_lfp(fr"{path}",fr"{ECEPHY_DATA_PATH}")
     folder_path = Path(folder_path)
-
     try:
-        print("tried" + fr"{stream_name}")
-        interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
-    except AssertionError:
         try:
-            folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
             print("tried" + fr"{stream_name}")
-            stream_name = 'Record Node 102#OE_FPGA_Acquisition_Board-101.Rhythm Data'
             interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
         except AssertionError:
             try:
-                folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
-                stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
+                folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
                 print("tried" + fr"{stream_name}")
-                #stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-101.Rhythm Data'
+                stream_name = 'Record Node 102#OE_FPGA_Acquisition_Board-101.Rhythm Data'
                 interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
-            except ValueError:
+            except AssertionError:
                 try:
-                    #stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
-                    stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-100.Rhythm Data'
+                    folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
+                    stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
                     print("tried" + fr"{stream_name}")
+                    #stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-101.Rhythm Data'
                     interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
                 except ValueError:
-                    #stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
-                    stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-101.Rhythm Data'
-                    print("tried" + fr"{stream_name}")
-                    interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
-    except ValueError:
-        try:
-            folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
-            stream_name = 'Record Node 102#OE_FPGA_Acquisition_Board-100.Rhythm Data'
-            print("tried" + fr"{stream_name}")
-            interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
+                    try:
+                        #stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
+                        stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-100.Rhythm Data'
+                        print("tried" + fr"{stream_name}")
+                        interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
+                    except ValueError:
+                        #stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
+                        stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-101.Rhythm Data'
+                        print("tried" + fr"{stream_name}")
+                        interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
         except ValueError:
-            folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
-            stream_name = 'Record Node 102#Acquisition_Board-100.Rhythm Data'
-            print("tried" + fr"{stream_name}")
-            interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
+            try:
+                folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
+                stream_name = 'Record Node 102#OE_FPGA_Acquisition_Board-100.Rhythm Data'
+                print("tried" + fr"{stream_name}")
+                interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
+            except ValueError:
+                folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
+                stream_name = 'Record Node 102#Acquisition_Board-100.Rhythm Data'
+                print("tried" + fr"{stream_name}")
+                interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
+            # Extract what metadata we can from the source files
+        folder1_path = f"{path}"  # Change the folder_path to the location of the data in your system
+        print(fr"Animal number is {UD[0]}")
+        # if UD[0] == "65410":
+        print(fr"Animal number is {UD[0]} replacing the spike times")
+        #     sample_num = np.load(fr"{folder1_path}/spike_times.npy")
+        #     timestemp = np.load(fr'{folder_path}\experiment1\recording1\continuous\OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+        #     print(folder_path)
+        #     time_spk = timestemp[sample_num]
+        #     np.save(fr"{folder1_path}/spike_times.npy",time_spk)
+            
+        sample_num = np.load(fr"{folder1_path}/spike_times.npy")
+        try:
+            timestemp = np.load(fr'{folder_path}/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+        except FileNotFoundError:
+            try:
+                folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
+                # S:\Sachuriga\Ephys_Recording\CR_CA1\65588\65588_2024-03-06_15-45-53_A\Record Node 101\experiment1\recording1\continuous\Acquisition_Board-100.Rhythm Data
+                timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+            except FileNotFoundError:
+                try:
+                    folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
+                    timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+                except FileNotFoundError:
+                    try:
+                        folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
+                        timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+                    except FileNotFoundError:
+                        folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
+                        timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+        
+        print(folder_path)
+        time_spk = timestemp[sample_num]
 
-    # Extract what metadata we can from the source files
-    folder1_path = f"{path}"  # Change the folder_path to the location of the data in your system
-    print(fr"Animal number is {UD[0]}")
-    # if UD[0] == "65410":
-    print(fr"Animal number is {UD[0]} replacing the spike times")
-    #     sample_num = np.load(fr"{folder1_path}/spike_times.npy")
-    #     timestemp = np.load(fr'{folder_path}\experiment1\recording1\continuous\OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
-    #     print(folder_path)
-    #     time_spk = timestemp[sample_num]
-    #     np.save(fr"{folder1_path}/spike_times.npy",time_spk)
+        np.save(fr"{folder1_path}/spike_times.npy",time_spk)
         
-    sample_num = np.load(fr"{folder1_path}/spike_times.npy")
-    try:
-        timestemp = np.load(fr'{folder_path}/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+        interface_phy = PhySortingInterface(folder_path=folder1_path, verbose=False)
+        # For data provenance we add the time zone information to the conversionSS
+        converter = ConverterPipe(data_interfaces=[interface_ophys, interface_phy], verbose=False)        
     except FileNotFoundError:
+        folder1_path = f"{path}"  # Change the folder_path to the location of the data in your system
+        print(fr"Animal number is {UD[0]}")
+        # if UD[0] == "65410":
+        print(fr"Animal number is {UD[0]} replacing the spike times")
+        #     sample_num = np.load(fr"{folder1_path}/spike_times.npy")
+        #     timestemp = np.load(fr'{folder_path}\experiment1\recording1\continuous\OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+        #     print(folder_path)
+        #     time_spk = timestemp[sample_num]
+        #     np.save(fr"{folder1_path}/spike_times.npy",time_spk)
+            
+        sample_num = np.load(fr"{folder1_path}/spike_times.npy")
         try:
-            folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
-            # S:\Sachuriga\Ephys_Recording\CR_CA1\65588\65588_2024-03-06_15-45-53_A\Record Node 101\experiment1\recording1\continuous\Acquisition_Board-100.Rhythm Data
-            timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+            timestemp = np.load(fr'{folder_path}/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
         except FileNotFoundError:
             try:
-                folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
-                timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+                folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
+                # S:\Sachuriga\Ephys_Recording\CR_CA1\65588\65588_2024-03-06_15-45-53_A\Record Node 101\experiment1\recording1\continuous\Acquisition_Board-100.Rhythm Data
+                timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
             except FileNotFoundError:
                 try:
                     folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
-                    timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
-                except FileNotFoundError:
-                    folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
                     timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+                except FileNotFoundError:
+                    try:
+                        folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
+                        timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+                    except FileNotFoundError:
+                        folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
+                        timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+        
+        print(folder_path)
+        time_spk = timestemp[sample_num]
+
+        np.save(fr"{folder1_path}/spike_times.npy",time_spk)
+        
+        interface_phy = PhySortingInterface(folder_path=folder1_path, verbose=False)
+        # For data provenance we add the time zone information to the conversionSS
+        converter = ConverterPipe(data_interfaces=[interface_phy], verbose=False)    
+
+    # # Extract what metadata we can from the source files
+    # folder1_path = f"{path}"  # Change the folder_path to the location of the data in your system
+    # print(fr"Animal number is {UD[0]}")
+    # # if UD[0] == "65410":
+    # print(fr"Animal number is {UD[0]} replacing the spike times")
+    # #     sample_num = np.load(fr"{folder1_path}/spike_times.npy")
+    # #     timestemp = np.load(fr'{folder_path}\experiment1\recording1\continuous\OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+    # #     print(folder_path)
+    # #     time_spk = timestemp[sample_num]
+    # #     np.save(fr"{folder1_path}/spike_times.npy",time_spk)
+        
+    # sample_num = np.load(fr"{folder1_path}/spike_times.npy")
+    # try:
+    #     timestemp = np.load(fr'{folder_path}/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+    # except FileNotFoundError:
+    #     try:
+    #         folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
+    #         # S:\Sachuriga\Ephys_Recording\CR_CA1\65588\65588_2024-03-06_15-45-53_A\Record Node 101\experiment1\recording1\continuous\Acquisition_Board-100.Rhythm Data
+    #         timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+    #     except FileNotFoundError:
+    #         try:
+    #             folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
+    #             timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
+    #         except FileNotFoundError:
+    #             try:
+    #                 folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
+    #                 timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
+    #             except FileNotFoundError:
+    #                 folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
+    #                 timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
     
-    print(folder_path)
-    time_spk = timestemp[sample_num]
+    # print(folder_path)
+    # time_spk = timestemp[sample_num]
 
-    np.save(fr"{folder1_path}/spike_times.npy",time_spk)
+    # np.save(fr"{folder1_path}/spike_times.npy",time_spk)
     
-    interface_phy = PhySortingInterface(folder_path=folder1_path, verbose=False)
-    # For data provenance we add the time zone information to the conversionSS
-    converter = ConverterPipe(data_interfaces=[interface_ophys, interface_phy], verbose=False)
+    # interface_phy = PhySortingInterface(folder_path=folder1_path, verbose=False)
+    # # For data provenance we add the time zone information to the conversionSS
+    # converter = ConverterPipe(data_interfaces=[interface_ophys, interface_phy], verbose=False)
     # Extract what metadata we can from the source files
     metadata = converter.get_metadata()
     arr_with_new_col = load_positions_h5(path,vedio_search_directory,folder_path,UD)
     # print(f"{arr_with_new_col.shape[1]} output the shape of the array")
     snout2neck = arr_with_new_col[:,[0,1,2,3,4]]
     neck2back4 = arr_with_new_col[:,[0,3,4,5,6]]
```

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.5.9.3/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.5.9.3/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.5.9.3/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.5.9.3/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.5.9.3/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.5.9.3/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.5.9.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.5.9.3/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.5.9.2
+Version: 0.5.9.3
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.5.9.3/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.9.2/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.5.9.3/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

