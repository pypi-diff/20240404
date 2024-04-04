# Comparing `tmp/iv_params-0.0.5.tar.gz` & `tmp/iv_params-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iv_params-0.0.5.tar", last modified: Mon Oct 24 17:16:55 2022, max compression
+gzip compressed data, was "iv_params-0.0.6.tar", last modified: Thu Apr  4 19:30:01 2024, max compression
```

## Comparing `iv_params-0.0.5.tar` & `iv_params-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:16:55.913817 iv_params-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-10-24 17:16:45.000000 iv_params-0.0.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-24 17:16:55.913817 iv_params-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-10-24 17:16:45.000000 iv_params-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 17:16:55.913817 iv_params-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-10-24 17:16:45.000000 iv_params-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:16:55.909817 iv_params-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:16:55.913817 iv_params-0.0.5/src/iv_params/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-24 17:16:45.000000 iv_params-0.0.5/src/iv_params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2022-10-24 17:16:45.000000 iv_params-0.0.5/src/iv_params/iv_params.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:16:55.913817 iv_params-0.0.5/src/iv_params.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-24 17:16:55.000000 iv_params-0.0.5/src/iv_params.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-24 17:16:55.000000 iv_params-0.0.5/src/iv_params.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 17:16:55.000000 iv_params-0.0.5/src/iv_params.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-24 17:16:55.000000 iv_params-0.0.5/src/iv_params.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-24 17:16:55.000000 iv_params-0.0.5/src/iv_params.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:30:01.806846 iv_params-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-04 19:29:50.000000 iv_params-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-04 19:30:01.806846 iv_params-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-04 19:29:50.000000 iv_params-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:30:01.806846 iv_params-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-04 19:29:50.000000 iv_params-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:30:01.802846 iv_params-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:30:01.802846 iv_params-0.0.6/src/iv_params/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 19:29:50.000000 iv_params-0.0.6/src/iv_params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-04 19:29:50.000000 iv_params-0.0.6/src/iv_params/iv_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:30:01.806846 iv_params-0.0.6/src/iv_params.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-04 19:30:01.000000 iv_params-0.0.6/src/iv_params.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-04 19:30:01.000000 iv_params-0.0.6/src/iv_params.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:30:01.000000 iv_params-0.0.6/src/iv_params.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 19:30:01.000000 iv_params-0.0.6/src/iv_params.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 19:30:01.000000 iv_params-0.0.6/src/iv_params.egg-info/top_level.txt
```

### Comparing `iv_params-0.0.5/LICENCE` & `iv_params-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iv_params-0.0.5/setup.py` & `iv_params-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iv_params",
-    version="0.0.5",
+    version="0.0.6",
     author="Michael Deceglie",
     author_email="michael.deceglie@nrel.gov",
     description="Perform ASTM E1036 extraction of photovoltaic IV parameters",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NREL/iv_params",
     classifiers=[
```

### Comparing `iv_params-0.0.5/src/iv_params/iv_params.py` & `iv_params-0.0.6/src/iv_params/iv_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,43 +23,46 @@
         df['i'] = i
         df['p'] = df['v'] * df['i']
 
         self.df = df
         self.v = v
         self.i = i
 
-    def calc_iv_params(self, imax_limits=(0.75, 1.15), vmax_limits=(0.75, 1.15), voc_points=3, isc_points=3):
+    def calc_iv_params(self, imax_limits=(0.75, 1.15), vmax_limits=(0.75, 1.15),
+                       voc_points=3, isc_points=3, mp_fit_order=4):
         '''
         Extract IV parameters
 
         Parameters
         ----------
         imax_limits : tuple
             Two-element tuple (low, high) specifying the fraction of estimated Imp within which
             to fit a polynomial for max power calculation
         vmax_limits : tuple
             Two-element tuple (low, high) specifying the fraction of estimated Vmp within which
             to fit a polynomial for max power calculation
         voc_points : int
-            the number of points near open circuit to use for linear fit and Voc calculation
+            The number of points near open circuit to use for linear fit and Voc calculation
         isc_points : int
-            the number of points near short circuit to use for linear fit and Isc calculation
+            The number of points near short circuit to use for linear fit and Isc calculation
+        mp_fit_order : int
+            The order of the polynomial fit of power vs. voltage near maximum power
 
         Returns
         -------
         dict
             Calculated IV parameters
         '''
         df = self.df
 
         # first calculate estimates of voc and isc
         voc = np.nan
         isc = np.nan
 
-        # determine if we can use voc and isc estimates 
+        # determine if we can use voc and isc estimates
         i_min_ind = df['i'].abs().idxmin()
         v_min_ind = df['v'].abs().idxmin()
         voc_est = df['v'][i_min_ind]
         isc_est = df['i'][v_min_ind]
 
         # accept the estimates if they are close enough
         if abs(df['i'][i_min_ind]) <= isc_est * 0.001:
@@ -90,15 +93,15 @@
             (df['i'] <= imax_limits[1] * mp_est['i']) &
             (df['v'] >= vmax_limits[0] * mp_est['v']) &
             (df['v'] <= vmax_limits[1] * mp_est['v'])
         )
         filtered = df[mask]
 
         # fit polynomial and find max
-        mp_fit = Poly.fit(filtered['v'], filtered['p'], 4)
+        mp_fit = Poly.fit(filtered['v'], filtered['p'], mp_fit_order)
         roots = mp_fit.deriv().roots()
         # only coniser real roots
         roots = roots.real[abs(roots.imag) < 1e-5]
         # only consider roots in the relevant part of the domain
         roots = roots[(roots < filtered['v'].max()) & (roots > filtered['v'].min())]
         vmp = roots[np.argmax(mp_fit(roots))]
         pmp = mp_fit(vmp)
```

