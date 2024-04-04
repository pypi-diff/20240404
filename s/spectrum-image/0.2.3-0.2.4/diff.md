# Comparing `tmp/spectrum_image-0.2.3.tar.gz` & `tmp/spectrum_image-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_image-0.2.3.tar", last modified: Wed Apr  3 04:35:46 2024, max compression
+gzip compressed data, was "spectrum_image-0.2.4.tar", last modified: Thu Apr  4 05:05:48 2024, max compression
```

## Comparing `spectrum_image-0.2.3.tar` & `spectrum_image-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-03 04:35:46.072224 spectrum_image-0.2.3/
--rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2.3/LICENSE
--rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-03 04:35:46.072021 spectrum_image-0.2.3/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      977 2024-03-18 03:44:13.000000 spectrum_image-0.2.3/README.md
--rw-r--r--   0 sung       (501) staff       (20)      864 2024-04-03 04:35:40.000000 spectrum_image-0.2.3/pyproject.toml
--rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-03 04:35:46.072261 spectrum_image-0.2.3/setup.cfg
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-03 04:35:46.067882 spectrum_image-0.2.3/src/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-03 04:35:46.070906 spectrum_image-0.2.3/src/spectrum_image/
--rw-r--r--   0 sung       (501) staff       (20)    21793 2024-04-03 04:29:17.000000 spectrum_image-0.2.3/src/spectrum_image/SI.py
--rw-r--r--   0 sung       (501) staff       (20)    69473 2024-03-30 23:57:52.000000 spectrum_image-0.2.3/src/spectrum_image/SI_bckup.py
--rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2.3/src/spectrum_image/SI_lineshapes.py
--rw-r--r--   0 sung       (501) staff       (20)     7832 2024-04-03 04:35:18.000000 spectrum_image-0.2.3/src/spectrum_image/SI_util.py
--rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2.3/src/spectrum_image/__init__.py
--rw-r--r--   0 sung       (501) staff       (20)    13150 2024-04-03 04:33:12.000000 spectrum_image-0.2.3/src/spectrum_image/eels_bgsub.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-03 04:35:46.071768 spectrum_image-0.2.3/src/spectrum_image.egg-info/
--rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-03 04:35:46.000000 spectrum_image-0.2.3/src/spectrum_image.egg-info/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      427 2024-04-03 04:35:46.000000 spectrum_image-0.2.3/src/spectrum_image.egg-info/SOURCES.txt
--rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-03 04:35:46.000000 spectrum_image-0.2.3/src/spectrum_image.egg-info/dependency_links.txt
--rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-03 04:35:46.000000 spectrum_image-0.2.3/src/spectrum_image.egg-info/requires.txt
--rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-03 04:35:46.000000 spectrum_image-0.2.3/src/spectrum_image.egg-info/top_level.txt
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-04 05:05:48.603479 spectrum_image-0.2.4/
+-rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2.4/LICENSE
+-rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-04 05:05:48.603272 spectrum_image-0.2.4/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      977 2024-03-18 03:44:13.000000 spectrum_image-0.2.4/README.md
+-rw-r--r--   0 sung       (501) staff       (20)      864 2024-04-04 05:05:39.000000 spectrum_image-0.2.4/pyproject.toml
+-rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-04 05:05:48.603521 spectrum_image-0.2.4/setup.cfg
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-04 05:05:48.599546 spectrum_image-0.2.4/src/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-04 05:05:48.602400 spectrum_image-0.2.4/src/spectrum_image/
+-rw-r--r--   0 sung       (501) staff       (20)    51585 2024-04-04 05:05:19.000000 spectrum_image-0.2.4/src/spectrum_image/SI.py
+-rw-r--r--   0 sung       (501) staff       (20)    69473 2024-03-30 23:57:52.000000 spectrum_image-0.2.4/src/spectrum_image/SI_bckup.py
+-rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2.4/src/spectrum_image/SI_lineshapes.py
+-rw-r--r--   0 sung       (501) staff       (20)     7832 2024-04-03 04:35:18.000000 spectrum_image-0.2.4/src/spectrum_image/SI_util.py
+-rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2.4/src/spectrum_image/__init__.py
+-rw-r--r--   0 sung       (501) staff       (20)    12873 2024-04-04 04:22:31.000000 spectrum_image-0.2.4/src/spectrum_image/eels_bgsub.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-04 05:05:48.603070 spectrum_image-0.2.4/src/spectrum_image.egg-info/
+-rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      427 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/SOURCES.txt
+-rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/dependency_links.txt
+-rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/requires.txt
+-rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-04 05:05:48.000000 spectrum_image-0.2.4/src/spectrum_image.egg-info/top_level.txt
```

### Comparing `spectrum_image-0.2.3/LICENSE` & `spectrum_image-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.3/PKG-INFO` & `spectrum_image-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum_image
 Project-URL: Repository, https://github.com/sukhsung/spectrum_image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum_image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spectrum_image-0.2.3/README.md` & `spectrum_image-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.3/pyproject.toml` & `spectrum_image-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spectrum_image"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
   "numpy",
   "matplotlib",
   "jupyterlab",
   "ipympl",
   "scipy",
   "tqdm",
```

### Comparing `spectrum_image-0.2.3/src/spectrum_image/SI_bckup.py` & `spectrum_image-0.2.4/src/spectrum_image/SI_bckup.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.3/src/spectrum_image/SI_lineshapes.py` & `spectrum_image-0.2.4/src/spectrum_image/SI_lineshapes.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.3/src/spectrum_image/SI_util.py` & `spectrum_image-0.2.4/src/spectrum_image/SI_util.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.3/src/spectrum_image/eels_bgsub.py` & `spectrum_image-0.2.4/src/spectrum_image/eels_bgsub.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,34 @@
                 print( "perc not set or invalid: Setting lc = False")
                 self.lc = False
             if (fit=='lin'):
                 print( "lc is not available for exp or pl: Setting lc = False")
                 self.lc = False
         
 
+##### Linear Regression
+def linear_regression_QR( y, X ):
+    # Solve Linear Regression using QR Decomposition
+    # Y = Xb + error
+    # R*b = Q.T*y minimizes MSE
+    # y: (nx1) dependent variable
+    # x: (nx1) independent variable
+    # b: (2x1) [[b0],[b1]], b0: intercept, b1: slope
+    if y.ndim == 1:
+        Y = np.atleast_2d( y ).T
+    else:
+        Y = y
+
+    Q, R = LA.qr(X)
+    b = LA.inv(R) @ (Q.T @ Y)
+
+    return b
 
 
-######## Background Subtractions
+######## Background Subtractions SI
 def bgsub_SI( si, energy, edge, fit_options=None, mask=None, threshold=None):
     """
     Full background subtraction function-
     Optional LBA, log fitting, LCPL, and exponential fitting.
     For more information on non-linear fitting function, see information at https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.curve_fit.html
 
     Inputs:
@@ -77,27 +94,28 @@
     """
 
     ### Load Fit Options
     if (fit_options is None):
         fit_options = options_bgsub()
 
     fit_start_ch, fit_end_ch = np.searchsorted( energy, edge.e_bsub)
+
     si = si.astype('float32')
     if len(np.shape(si)) == 2:
         tempx,tempz = np.shape(si)
         si = np.reshape(si,(tempx,1,tempz))
     if len(np.shape(si)) == 1:
         tempz = len(si)
         si = np.reshape(si,(1,1,tempz))
     xdim, ydim, zdim = np.shape(si)
 
 
     ## Apply Local Background Averaging
     if fit_options.lba==True:
-        fit_data = prepare_lba( si, fit_options.gfwhm, fit_start_ch, fit_end_ch )
+        fit_data = prepare_si_lba( si, fit_options.gfwhm, fit_start_ch, fit_end_ch )
     else:
         fit_data = si
     
     ## If log fitting or linear fitting, find fit using qr factorization       
     if fit_options.log or (fit_options.fit=='lin'):
         bg_pl_SI, fit_params = bgsub_SI_linearized( fit_data, energy, edge, fit_options=fit_options )
 
@@ -121,51 +139,14 @@
     if fit_options.lc:
         bg_lcpl_SI = bgsub_SI_LC(fit_data, energy, edge, rline, fit_options)
         return bg_pl_SI, bg_lcpl_SI
     else:
         return bg_pl_SI
     
 
-def prepare_lba( si, gfwhm, fit_start_ch, fit_end_ch ):
-    lba_raw = np.copy( si )
-    lba_normalized = np.copy( si )
-    for energychannel in np.arange(fit_start_ch,fit_end_ch):
-        lba_raw[:,:,energychannel] = gaussian_filter(si[:,:,energychannel],sigma=gfwhm/2.35)
-    
-    lba_mean = np.mean( lba_raw[:,:,fit_start_ch:fit_end_ch], 2 )
-    data_mean = np.mean(     si[:,:,fit_start_ch:fit_end_ch], 2)
-
-    for energychannel in np.arange(fit_start_ch,fit_end_ch):
-        lba_normalized[:,:,energychannel] = lba_raw[:,:,energychannel]*data_mean/lba_mean
-
-    return lba_normalized
-    
-
-def linear_regression_QR( y, X ):
-    # Solve Linear Regression using QR Decomposition
-    # Y = Xb + error
-    # R*b = Q.T*y minimizes MSE
-    # y: (nx1) dependent variable
-    # x: (nx1) independent variable
-    # b: (2x1) [[b0],[b1]], b0: intercept, b1: slope
-    if y.ndim == 1:
-        Y = np.atleast_2d( y ).T
-    else:
-        Y = y
-
-    Q, R = LA.qr(X)
-    b = LA.inv(R) @ (Q.T @ Y)
-
-    return b
-
-
-
-
-
-
 ########### background subtractions ########
 def bgsub_SI_fast( si, energy, edge, rval, fit_options=None):
     """
     Quick background subtraction based on fixed 'r' value
     For Y = Ax + b + error with fixed 'A':
         Y' = b + error. MSE is minimized when b = mean(Y)
     """
@@ -210,20 +191,14 @@
     fit_start_ch, fit_end_ch = np.searchsorted(energy, edge.e_bsub)
     if (fit_end_ch - fit_start_ch)<2:
         fit_end_ch = fit_start_ch+2
     e_win = np.atleast_2d( energy[fit_start_ch:fit_end_ch] ).T
     e_sub = np.atleast_2d( energy[fit_start_ch:] ).T
     zdim = len(energy)
 
-    if si.ndim == 1:
-        si = np.reshape( si, (1,1,zdim))
-    elif si.ndim == 2:
-        (nx,nz) = si.shape
-        si = np.reshape( si,(nx,1,zdim))
-
     xdim, ydim, zdim = np.shape( si )
     y_win = si[:,:,fit_start_ch:fit_end_ch]
     y_win = np.reshape( y_win, (xdim*ydim, len(e_win))).T
 
     bg_SI = np.zeros_like( si )  
     if fit_options.fit == 'lin':
         e_win = np.insert( e_win, 0, 1, axis=1)
@@ -272,20 +247,14 @@
     xtol   = fit_options.xtol
 
     fit_start_ch, fit_end_ch = np.searchsorted(energy, edge.e_bsub)
     e_win = energy[fit_start_ch:fit_end_ch]
     e_sub = energy[fit_start_ch:]
     zdim = len(energy)
 
-    if si.ndim == 1:
-        si = np.reshape( si, (1,1,zdim))
-    elif si.ndim == 2:
-        (nx,nz) = si.shape
-        si = np.reshape( si,(nx,1,zdim))
-
     xdim, ydim, zdim = np.shape( si )
     y_win = si[:,:,fit_start_ch:fit_end_ch]
     bg_SI = np.zeros_like( si )
 
     if fit_options.fit == 'pl':
         fitfunc = ls.powerlaw
         jac_Func   = ls.d_powerlaw
@@ -307,15 +276,15 @@
             
             bg_SI[i,j,fit_start_ch:] = si[i,j,fit_start_ch:] - fitfunc(e_sub, *popt_pl)
             fit_params[:,i,j] = popt_pl
             pbar1.update(1)
 
     return bg_SI, fit_params
 
-def bgsub_SI_LC( si, energy, edge, rline, fit_options):
+def bgsub_SI_LC( si, energy, edge, rline, fit_options=None):
     bg_lcpl_SI = np.zeros_like(si)
 
     ### Load Fit Options
     if (fit_options is None):
         fit_options = options_bgsub()
 
     rmu,rstd = norm.fit(rline)
@@ -355,7 +324,21 @@
     y_fit = (e_sub @ b_fit).T
 
     bgndLCPL = np.reshape( y_fit,(xdim,ydim,len_e_sub))
     bg_lcpl_SI[:,:,fit_start_ch:] = si[:,:,fit_start_ch:] - bgndLCPL
 
     return bg_lcpl_SI
 
+def prepare_si_lba( si, gfwhm, fit_start_ch, fit_end_ch ):
+    lba_raw = np.copy( si )
+    lba_normalized = np.copy( si )
+    for energychannel in np.arange(fit_start_ch,fit_end_ch):
+        lba_raw[:,:,energychannel] = gaussian_filter(si[:,:,energychannel],sigma=gfwhm/2.35)
+    
+    lba_mean = np.mean( lba_raw[:,:,fit_start_ch:fit_end_ch], 2 )
+    data_mean = np.mean(     si[:,:,fit_start_ch:fit_end_ch], 2)
+
+    for energychannel in np.arange(fit_start_ch,fit_end_ch):
+        lba_normalized[:,:,energychannel] = lba_raw[:,:,energychannel]*data_mean/lba_mean
+
+    return lba_normalized
+
```

### Comparing `spectrum_image-0.2.3/src/spectrum_image.egg-info/PKG-INFO` & `spectrum_image-0.2.4/src/spectrum_image.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum_image
 Project-URL: Repository, https://github.com/sukhsung/spectrum_image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum_image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

