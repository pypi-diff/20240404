# Comparing `tmp/ColdTOFU-0.1.1.tar.gz` & `tmp/ColdTOFU-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColdTOFU-0.1.1.tar", last modified: Thu Dec 21 07:32:15 2023, max compression
+gzip compressed data, was "ColdTOFU-0.1.2.tar", last modified: Thu Apr  4 03:58:38 2024, max compression
```

## Comparing `ColdTOFU-0.1.1.tar` & `ColdTOFU-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 chetan     (501) staff       (20)        0 2023-12-21 07:32:15.029360 ColdTOFU-0.1.1/
-drwxr-xr-x   0 chetan     (501) staff       (20)        0 2023-12-21 07:32:15.027295 ColdTOFU-0.1.1/ColdTOFU/
--rw-r--r--   0 chetan     (501) staff       (20)   325120 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/ATSIFIO64.dll
--rw-r--r--   0 chetan     (501) staff       (20)    13091 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/AndorSifReader.py
--rw-r--r--   0 chetan     (501) staff       (20)      732 2023-12-21 05:51:00.000000 ColdTOFU-0.1.1/ColdTOFU/Helvetica_bright.mplstyle
--rw-r--r--   0 chetan     (501) staff       (20)    25598 2023-12-21 06:19:44.000000 ColdTOFU-0.1.1/ColdTOFU/Images.py
-drwxr-xr-x   0 chetan     (501) staff       (20)        0 2023-12-21 07:32:15.028809 ColdTOFU-0.1.1/ColdTOFU/Physics/
--rw-r--r--   0 chetan     (501) staff       (20)      143 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/Physics/__init__.py
--rw-r--r--   0 chetan     (501) staff       (20)     1863 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/Physics/allenDeviation.py
--rw-r--r--   0 chetan     (501) staff       (20)     3050 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/Physics/basisMatrices.py
--rw-r--r--   0 chetan     (501) staff       (20)     1125 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/Physics/beams.py
--rw-r--r--   0 chetan     (501) staff       (20)     1449 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/Physics/createAndDestroy.py
--rw-r--r--   0 chetan     (501) staff       (20)     4291 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/Physics/spinInDickeBasis.py
--rw-r--r--   0 chetan     (501) staff       (20)      224 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/__init__.py
--rw-r--r--   0 chetan     (501) staff       (20)    17659 2023-12-21 06:19:43.000000 ColdTOFU-0.1.1/ColdTOFU/fits.py
--rw-r--r--   0 chetan     (501) staff       (20)     1332 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/jupyterTools.py
--rw-r--r--   0 chetan     (501) staff       (20)     6439 2023-12-21 06:19:42.000000 ColdTOFU-0.1.1/ColdTOFU/numberOfAtoms.py
--rw-r--r--   0 chetan     (501) staff       (20)     2700 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/picoMatTools.py
--rw-r--r--   0 chetan     (501) staff       (20)      153 2023-12-21 05:51:00.000000 ColdTOFU-0.1.1/ColdTOFU/rcParams.json
--rw-r--r--   0 chetan     (501) staff       (20)      856 2023-12-21 05:51:00.000000 ColdTOFU-0.1.1/ColdTOFU/scientific_serif.mplstyle
--rw-r--r--   0 chetan     (501) staff       (20)     2694 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/ColdTOFU/sigma.py
--rw-r--r--   0 chetan     (501) staff       (20)    10352 2023-12-21 05:51:00.000000 ColdTOFU-0.1.1/ColdTOFU/spectrum.py
-drwxr-xr-x   0 chetan     (501) staff       (20)        0 2023-12-21 07:32:15.029059 ColdTOFU-0.1.1/ColdTOFU.egg-info/
--rw-r--r--   0 chetan     (501) staff       (20)      973 2023-12-21 07:32:15.000000 ColdTOFU-0.1.1/ColdTOFU.egg-info/PKG-INFO
--rw-r--r--   0 chetan     (501) staff       (20)      695 2023-12-21 07:32:15.000000 ColdTOFU-0.1.1/ColdTOFU.egg-info/SOURCES.txt
--rw-r--r--   0 chetan     (501) staff       (20)        1 2023-12-21 07:32:15.000000 ColdTOFU-0.1.1/ColdTOFU.egg-info/dependency_links.txt
--rw-r--r--   0 chetan     (501) staff       (20)        9 2023-12-21 07:32:15.000000 ColdTOFU-0.1.1/ColdTOFU.egg-info/top_level.txt
--rw-r--r--   0 chetan     (501) staff       (20)     1068 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/LICENCE
--rw-r--r--   0 chetan     (501) staff       (20)       74 2023-12-21 06:19:46.000000 ColdTOFU-0.1.1/MANIFEST.in
--rw-r--r--   0 chetan     (501) staff       (20)      973 2023-12-21 07:32:15.029294 ColdTOFU-0.1.1/PKG-INFO
--rw-r--r--   0 chetan     (501) staff       (20)      508 2023-12-21 05:51:00.000000 ColdTOFU-0.1.1/README.md
--rw-r--r--   0 chetan     (501) staff       (20)      103 2023-09-04 06:19:38.000000 ColdTOFU-0.1.1/pyproject.toml
--rw-r--r--   0 chetan     (501) staff       (20)      642 2023-12-21 07:32:15.029623 ColdTOFU-0.1.1/setup.cfg
+drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-04 03:58:38.486283 ColdTOFU-0.1.2/
+drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-04 03:58:38.483953 ColdTOFU-0.1.2/ColdTOFU/
+-rw-r--r--   0 chetan     (501) staff       (20)   325120 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/ATSIFIO64.dll
+-rw-r--r--   0 chetan     (501) staff       (20)    13142 2024-04-04 03:48:17.000000 ColdTOFU-0.1.2/ColdTOFU/AndorSifReader.py
+-rw-r--r--   0 chetan     (501) staff       (20)      732 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/ColdTOFU/Helvetica_bright.mplstyle
+-rw-r--r--   0 chetan     (501) staff       (20)    26925 2024-04-04 03:32:07.000000 ColdTOFU-0.1.2/ColdTOFU/Images.py
+drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-04 03:58:38.485679 ColdTOFU-0.1.2/ColdTOFU/Physics/
+-rw-r--r--   0 chetan     (501) staff       (20)      143 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/__init__.py
+-rw-r--r--   0 chetan     (501) staff       (20)     1863 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/allenDeviation.py
+-rw-r--r--   0 chetan     (501) staff       (20)     3050 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/basisMatrices.py
+-rw-r--r--   0 chetan     (501) staff       (20)     1125 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/beams.py
+-rw-r--r--   0 chetan     (501) staff       (20)     1449 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/createAndDestroy.py
+-rw-r--r--   0 chetan     (501) staff       (20)     4291 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/spinInDickeBasis.py
+-rw-r--r--   0 chetan     (501) staff       (20)      224 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/__init__.py
+-rw-r--r--   0 chetan     (501) staff       (20)    17659 2023-12-21 06:19:43.000000 ColdTOFU-0.1.2/ColdTOFU/fits.py
+-rw-r--r--   0 chetan     (501) staff       (20)     1332 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/jupyterTools.py
+-rw-r--r--   0 chetan     (501) staff       (20)     6439 2023-12-21 06:19:42.000000 ColdTOFU-0.1.2/ColdTOFU/numberOfAtoms.py
+-rw-r--r--   0 chetan     (501) staff       (20)     2700 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/picoMatTools.py
+-rw-r--r--   0 chetan     (501) staff       (20)      153 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/ColdTOFU/rcParams.json
+-rw-r--r--   0 chetan     (501) staff       (20)      856 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/ColdTOFU/scientific_serif.mplstyle
+-rw-r--r--   0 chetan     (501) staff       (20)     2694 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/sigma.py
+-rw-r--r--   0 chetan     (501) staff       (20)    10352 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/ColdTOFU/spectrum.py
+drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-04 03:58:38.485929 ColdTOFU-0.1.2/ColdTOFU.egg-info/
+-rw-r--r--   0 chetan     (501) staff       (20)      973 2024-04-04 03:58:38.000000 ColdTOFU-0.1.2/ColdTOFU.egg-info/PKG-INFO
+-rw-r--r--   0 chetan     (501) staff       (20)      695 2024-04-04 03:58:38.000000 ColdTOFU-0.1.2/ColdTOFU.egg-info/SOURCES.txt
+-rw-r--r--   0 chetan     (501) staff       (20)        1 2024-04-04 03:58:38.000000 ColdTOFU-0.1.2/ColdTOFU.egg-info/dependency_links.txt
+-rw-r--r--   0 chetan     (501) staff       (20)        9 2024-04-04 03:58:38.000000 ColdTOFU-0.1.2/ColdTOFU.egg-info/top_level.txt
+-rw-r--r--   0 chetan     (501) staff       (20)     1068 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/LICENCE
+-rw-r--r--   0 chetan     (501) staff       (20)       74 2023-12-21 06:19:46.000000 ColdTOFU-0.1.2/MANIFEST.in
+-rw-r--r--   0 chetan     (501) staff       (20)      973 2024-04-04 03:58:38.486216 ColdTOFU-0.1.2/PKG-INFO
+-rw-r--r--   0 chetan     (501) staff       (20)      508 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/README.md
+-rw-r--r--   0 chetan     (501) staff       (20)      231 2024-04-04 03:58:00.000000 ColdTOFU-0.1.2/pyproject.toml
+-rw-r--r--   0 chetan     (501) staff       (20)      656 2024-04-04 03:58:38.486564 ColdTOFU-0.1.2/setup.cfg
```

### Comparing `ColdTOFU-0.1.1/ColdTOFU/ATSIFIO64.dll` & `ColdTOFU-0.1.2/ColdTOFU/ATSIFIO64.dll`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/AndorSifReader.py` & `ColdTOFU-0.1.2/ColdTOFU/AndorSifReader.py`

 * *Files 3% similar despite different names*

```diff
@@ -368,12 +368,13 @@
         def _ReadData(self, frameNum):
             data = (c_float*self._nrPixels)()
             errorCode = self.dll.ATSIF_GetFrame(self._source, frameNum, data, self._nrPixels)
             SifError.ProcessErrorCode(errorCode)
             return np.ctypeslib.as_array(data)
 
 elif platform.startswith('lin'):
-    warnings.warn('Andor *.sif files could not be read in linux as ATSIFIO64.dll is only available for windows.')
+    warnings.warn('Andor *.sif files are read by sif-parser not by using ATSIFIO64.dll')
 elif platform.startswith('dar'):
-    warnings.warn('Andor *.sif files could not be read in Mac OS as ATSIFIO64.dll is only available for windows.')
+    warnings.warn('Andor *.sif files are read by sif-parser not by using ATSIFIO64.dll')
 else:
-    warnings.warn('Andor *.sif files could not be read in your OS as ATSIFIO64.dll is only available for windows.')
+    warnings.warn('Andor *.sif files could not be read in your OS as ATSIFIO64.dll is only available for windows.\
+                   Try sif-parser package to read and implement it in __init__ of FluorescenceImage.')
```

### Comparing `ColdTOFU-0.1.1/ColdTOFU/Helvetica_bright.mplstyle` & `ColdTOFU-0.1.2/ColdTOFU/Helvetica_bright.mplstyle`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/Images.py` & `ColdTOFU-0.1.2/ColdTOFU/Images.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from warnings import warn
 import json
 from importlib import resources
 import io
 from scipy.constants import *
 import sys
 import datetime as dt
+from sif_parser import np_open
 
 class rcParams():
     """
     A class that is designed to read and update resource parameters of the package. These parameters are usually the
     hardware parameters that are used while converting certain digital values to real units. Currently these are
     imaging parameters like magnification, pixel size etc. The idea behind this is that once these parameters are set,
     these are used by many function and classes throughout the package without having to explicitly pass them. Open
@@ -80,43 +81,60 @@
             self.im = Image.open(filePath)
             self.tags = self.im.tag.named()
         elif self.ext == '.sif':
             if sys.platform.startswith('win'):
                 from .AndorSifReader import AndorSifFile
                 self.im = AndorSifFile(filePath).signal
                 self.tags = self.im.props
+                self.frames = self.im.data
             elif sys.platform.startswith('lin'):
-                warn('Andor *.sif files could not be read in linux as ATSIFIO64.dll is only available for windows.')
+                try:
+                    data_read = np_open(filePath)
+                    self.frames = data_read[0]
+                    self.im = Image.fromarray(data_read[0][0])
+                    self.im.n_frames = len(self.frames)
+                    self.tags = data_read[1]
+                except IOError:
+                    warn('Sif file could not be read. Try on Windows machine')
             elif sys.platform.startswith('dar'):
-                warn('Andor *.sif files could not be read in Mac OS as ATSIFIO64.dll is only available for windows.')
+                try:
+                    data_read = np_open(filePath)
+                    self.frames = data_read[0]
+                    self.im = Image.fromarray(data_read[0][0])
+                    self.im.n_frames = len(self.frames)
+                    self.tags = data_read[1]
+                except IOError:
+                    warn('Sif file could not be read. Try on Windows machine')
             else:
                 warn('Andor *.sif files could not be read in your OS as ATSIFIO64.dll is only available for windows.')
         else:
-            raise NotImplementedError('ShadowImage is implemeted to read only .tif or sif. files.')
-        if self.im.n_frames%3!=0:
-            warn('Not a valid shadow image. \
-                  No. of images in the file is not a multiple of 3.')
-        self.n = self.im.n_frames//3
+            raise IOError('Invalid file!')
+        if self.im.n_frames%2!=0:
+            warn('Not a valid fluorescence image. \
+                  No. of images in the file is not a multiple of 2.')
+        self.n = self.im.n_frames//2
         self.frames = self.images()
         self.params = rcParams().params
         self.docs = None
 
     def images(self):
         """
         Returns the images present in the ShadowImage object as an ndarray.
         """
         if self.ext == '.tif':
             frames = np.zeros((self.im.n_frames, self.im.height, self.im.width))
             for i in range(self.im.n_frames):
                 self.im.seek(i)
                 frames[i] = np.array(self.im)
             return frames
-        elif self.ext == '.sif':
+        elif self.ext == '.sif' and sys.platform.startswith('win'):
             frames = self.im.data
             return frames
+        else:
+            return self.frames
 
     def opticalDepth(self, xSpan, ySpan):
         """
         Returns the optical depth calculated from the ShadowImage as an ndarray.
 
         Parameters:
             xSpan: list, containing the range of pixels of the image in x direction.
@@ -400,18 +418,33 @@
             self.im = Image.open(filePath)
             self.tags = self.im.tag.named()
         elif self.ext == '.sif':
             if sys.platform.startswith('win'):
                 from .AndorSifReader import AndorSifFile
                 self.im = AndorSifFile(filePath).signal
                 self.tags = self.im.props
+                self.frames = self.im.data
             elif sys.platform.startswith('lin'):
-                warn('Andor *.sif files could not be read in linux as ATSIFIO64.dll is only available for windows.')
+                try:
+                    data_read = np_open(filePath)
+                    self.frames = data_read[0]
+                    self.im = Image.fromarray(data_read[0][0])
+                    self.im.n_frames = len(self.frames)
+                    self.tags = data_read[1]
+                except IOError:
+                    warn('Sif file could not be read. Try on Windows machine')
             elif sys.platform.startswith('dar'):
-                warn('Andor *.sif files could not be read in Mac OS as ATSIFIO64.dll is only available for windows.')
+                try:
+                    data_read = np_open(filePath)
+                    self.frames = data_read[0]
+                    self.im = Image.fromarray(data_read[0][0])
+                    self.im.n_frames = len(self.frames)
+                    self.tags = data_read[1]
+                except IOError:
+                    warn('Sif file could not be read. Try on Windows machine')
             else:
                 warn('Andor *.sif files could not be read in your OS as ATSIFIO64.dll is only available for windows.')
         else:
             raise IOError('Invalid file!')
         if self.im.n_frames%2!=0:
             warn('Not a valid fluorescence image. \
                   No. of images in the file is not a multiple of 2.')
@@ -424,17 +457,19 @@
         """
         if self.ext == '.tif':
             frames = np.zeros((self.im.n_frames, self.im.height, self.im.width))
             for i in range(self.im.n_frames):
                 self.im.seek(i)
                 frames[i] = np.array(self.im)
             return frames
-        elif self.ext == '.sif':
+        elif self.ext == '.sif' and sys.platform.startswith('win'):
             frames = self.im.data
             return frames
+        else:
+            return self.frames
     
     def fluorescence(self, xSpan, ySpan):
         """
         Returns the fluorence calculated from the FluorencenceImage as an ndarray.
 
         Parameters:
             xSpan: a list containing the range of pixels of the image in x direction.
@@ -529,15 +564,14 @@
         self.log_file.write('\n\t* '.join(self.call_stack))
         self.log_file.write('\n')
         if exc_type!=None:
             self.write_docs(exc_type)
             self.write_docs(exc_value)
         self.log_file.close()
 
-
 def approximatePositionOfTheCloud(meanOD):
     '''
     A function to locate the atomic cloud in images.
 
     Parameters:
         meanOD: 2darray, image data usually OD image
     Returns:
```

### Comparing `ColdTOFU-0.1.1/ColdTOFU/Physics/allenDeviation.py` & `ColdTOFU-0.1.2/ColdTOFU/Physics/allenDeviation.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/Physics/basisMatrices.py` & `ColdTOFU-0.1.2/ColdTOFU/Physics/basisMatrices.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/Physics/beams.py` & `ColdTOFU-0.1.2/ColdTOFU/Physics/beams.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/Physics/createAndDestroy.py` & `ColdTOFU-0.1.2/ColdTOFU/Physics/createAndDestroy.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/Physics/spinInDickeBasis.py` & `ColdTOFU-0.1.2/ColdTOFU/Physics/spinInDickeBasis.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/fits.py` & `ColdTOFU-0.1.2/ColdTOFU/fits.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/jupyterTools.py` & `ColdTOFU-0.1.2/ColdTOFU/jupyterTools.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/numberOfAtoms.py` & `ColdTOFU-0.1.2/ColdTOFU/numberOfAtoms.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/picoMatTools.py` & `ColdTOFU-0.1.2/ColdTOFU/picoMatTools.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/scientific_serif.mplstyle` & `ColdTOFU-0.1.2/ColdTOFU/scientific_serif.mplstyle`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/sigma.py` & `ColdTOFU-0.1.2/ColdTOFU/sigma.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU/spectrum.py` & `ColdTOFU-0.1.2/ColdTOFU/spectrum.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/ColdTOFU.egg-info/PKG-INFO` & `ColdTOFU-0.1.2/ColdTOFU.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColdTOFU
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cold Atoms Time-of-Flight Utilities
 Home-page: https://github.com/chetanmadasu/TOFU
 Author: Chetan Sriram Madasu
 Author-email: chetan.madasu@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ColdTOFU-0.1.1/ColdTOFU.egg-info/SOURCES.txt` & `ColdTOFU-0.1.2/ColdTOFU.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/LICENCE` & `ColdTOFU-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.1/PKG-INFO` & `ColdTOFU-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColdTOFU
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cold Atoms Time-of-Flight Utilities
 Home-page: https://github.com/chetanmadasu/TOFU
 Author: Chetan Sriram Madasu
 Author-email: chetan.madasu@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ColdTOFU-0.1.1/setup.cfg` & `ColdTOFU-0.1.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = ColdTOFU
-version = 0.1.1
+version = 0.1.2
 author = Chetan Sriram Madasu
 author_email = chetan.madasu@gmail.com
 description = Cold Atoms Time-of-Flight Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chetanmadasu/TOFU
 license = MIT License
-install_requires = ['numpy', 'scipy', 'pillow', 'sympy', 'matplotlib>=3.8', 'ipython']
+install_requires = ['numpy', 'scipy', 'pillow', 'sympy', 'matplotlib>=3.8', 'ipython', 'sif-parser']
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
```

