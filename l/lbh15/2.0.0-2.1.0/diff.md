# Comparing `tmp/lbh15-2.0.0.tar.gz` & `tmp/lbh15-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbh15-2.0.0.tar", last modified: Mon Jan  8 10:33:15 2024, max compression
+gzip compressed data, was "lbh15-2.1.0.tar", last modified: Thu Apr  4 10:17:06 2024, max compression
```

## Comparing `lbh15-2.0.0.tar` & `lbh15-2.1.0.tar`

### file list

```diff
@@ -1,45 +1,54 @@
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-01-08 10:33:15.915040 lbh15-2.0.0/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     7651 2023-04-12 12:31:38.000000 lbh15-2.0.0/LICENSE
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       34 2023-04-12 12:31:38.000000 lbh15-2.0.0/MANIFEST.in
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     4967 2024-01-08 10:33:15.915040 lbh15-2.0.0/PKG-INFO
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3931 2024-01-08 10:27:28.000000 lbh15-2.0.0/README.rst
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-01-08 10:33:15.911040 lbh15-2.0.0/lbh15/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1204 2024-01-08 09:32:24.000000 lbh15-2.0.0/lbh15/__init__.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      982 2023-11-28 17:14:15.000000 lbh15-2.0.0/lbh15/_commons.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1008 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/_decorators.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    27509 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/_lbh15.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3966 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/bismuth.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     5283 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/lbe.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     5873 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/lead.py
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-01-08 10:33:15.911040 lbh15-2.0.0/lbh15/properties/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       54 2023-04-12 12:31:38.000000 lbh15-2.0.0/lbh15/properties/__init__.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    20319 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/bismuth_properties.py
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-01-08 10:33:15.911040 lbh15-2.0.0/lbh15/properties/bismuth_thermochemical_properties/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       87 2023-11-28 17:10:37.000000 lbh15-2.0.0/lbh15/properties/bismuth_thermochemical_properties/__init__.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    14784 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/bismuth_thermochemical_properties/bismuth_thermochemical.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3728 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/bismuth_thermochemical_properties/diffusivity_in_bismuth.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    15102 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/bismuth_thermochemical_properties/solubility_in_bismuth.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     9743 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/interface.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    20343 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lbe_properties.py
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-01-08 10:33:15.911040 lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       83 2023-11-28 17:10:37.000000 lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/__init__.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     5391 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/diffusivity_in_lbe.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    31882 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/lbe_oxygen_limits.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    12942 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/lbe_thermochemical.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    13653 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/solubility_in_lbe.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    23110 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lead_properties.py
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-01-08 10:33:15.911040 lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       84 2023-11-28 17:10:37.000000 lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/__init__.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    19068 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/diffusivity_in_lead.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    30320 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/lead_oxygen_limits.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    23244 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/lead_thermochemical.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    12084 2024-01-08 09:31:42.000000 lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/solubility_in_lead.py
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-01-08 10:33:15.911040 lbh15-2.0.0/lbh15.egg-info/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     4967 2024-01-08 10:33:15.000000 lbh15-2.0.0/lbh15.egg-info/PKG-INFO
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1452 2024-01-08 10:33:15.000000 lbh15-2.0.0/lbh15.egg-info/SOURCES.txt
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)        1 2024-01-08 10:33:15.000000 lbh15-2.0.0/lbh15.egg-info/dependency_links.txt
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       27 2024-01-08 10:33:15.000000 lbh15-2.0.0/lbh15.egg-info/requires.txt
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)        6 2024-01-08 10:33:15.000000 lbh15-2.0.0/lbh15.egg-info/top_level.txt
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1327 2024-01-08 10:25:09.000000 lbh15-2.0.0/pyproject.toml
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       38 2024-01-08 10:33:15.915040 lbh15-2.0.0/setup.cfg
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     4069 2024-01-08 10:25:14.000000 lbh15-2.0.0/setup.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-04-04 10:17:06.431633 lbh15-2.1.0/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     7651 2024-01-08 17:30:47.000000 lbh15-2.1.0/LICENSE
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       34 2024-01-08 17:30:47.000000 lbh15-2.1.0/MANIFEST.in
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     5829 2024-04-04 10:17:06.431633 lbh15-2.1.0/PKG-INFO
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     4591 2024-04-04 10:13:44.000000 lbh15-2.1.0/README.rst
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-04-04 10:17:06.427633 lbh15-2.1.0/lbh15/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1202 2024-04-04 10:13:44.000000 lbh15-2.1.0/lbh15/__init__.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      991 2024-03-09 15:12:37.000000 lbh15-2.1.0/lbh15/_commons.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1008 2024-01-08 17:30:37.000000 lbh15-2.1.0/lbh15/_decorators.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    29329 2024-04-04 09:06:57.000000 lbh15-2.1.0/lbh15/_lbh15.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3964 2024-03-09 15:12:37.000000 lbh15-2.1.0/lbh15/bismuth.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     5280 2024-03-09 15:12:37.000000 lbh15-2.1.0/lbh15/lbe.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     5866 2024-03-09 15:12:37.000000 lbh15-2.1.0/lbh15/lead.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-04-04 10:17:06.427633 lbh15-2.1.0/lbh15/properties/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       54 2024-01-08 17:30:38.000000 lbh15-2.1.0/lbh15/properties/__init__.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    17830 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/bismuth_properties.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-04-04 10:17:06.427633 lbh15-2.1.0/lbh15/properties/bismuth_thermochemical_properties/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       88 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/bismuth_thermochemical_properties/__init__.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    13164 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/bismuth_thermochemical_properties/bismuth_thermochemical.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3760 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/bismuth_thermochemical_properties/diffusivity_in_bismuth.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    13795 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/bismuth_thermochemical_properties/solubility_in_bismuth.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     9735 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/interface.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    17759 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lbe_properties.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-04-04 10:17:06.427633 lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       84 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/__init__.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     4679 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/diffusivity_in_lbe.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    28449 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/lbe_oxygen_limits.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    11321 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/lbe_thermochemical.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    13107 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/solubility_in_lbe.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    20048 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lead_properties.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-04-04 10:17:06.431633 lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       85 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/__init__.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    18405 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/diffusivity_in_lead.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    26904 2024-04-04 09:06:57.000000 lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/lead_oxygen_limits.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    21658 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/lead_thermochemical.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    10773 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/solubility_in_lead.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    11961 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/tch_common_interface.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     5057 2024-03-25 13:26:55.000000 lbh15-2.1.0/lbh15/properties/tph_common_interface.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-04-04 10:17:06.431633 lbh15-2.1.0/lbh15.egg-info/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     5829 2024-04-04 10:17:06.000000 lbh15-2.1.0/lbh15.egg-info/PKG-INFO
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1714 2024-04-04 10:17:06.000000 lbh15-2.1.0/lbh15.egg-info/SOURCES.txt
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)        1 2024-04-04 10:17:06.000000 lbh15-2.1.0/lbh15.egg-info/dependency_links.txt
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      112 2024-04-04 10:17:06.000000 lbh15-2.1.0/lbh15.egg-info/requires.txt
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)        6 2024-04-04 10:17:06.000000 lbh15-2.1.0/lbh15.egg-info/top_level.txt
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1440 2024-04-04 10:10:45.000000 lbh15-2.1.0/pyproject.toml
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       38 2024-04-04 10:17:06.431633 lbh15-2.1.0/setup.cfg
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     4192 2024-04-04 10:10:40.000000 lbh15-2.1.0/setup.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2024-04-04 10:17:06.431633 lbh15-2.1.0/tests/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3016 2024-01-08 17:30:47.000000 lbh15-2.1.0/tests/test_bismuth_fromX_spanT.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3343 2024-01-08 17:30:47.000000 lbh15-2.1.0/tests/test_custom_properties.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3328 2024-01-08 17:30:47.000000 lbh15-2.1.0/tests/test_lbe_fromX_spanT.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    15135 2024-01-08 17:30:47.000000 lbh15-2.1.0/tests/test_lbh15_bounds.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1260 2024-01-08 17:30:47.000000 lbh15-2.1.0/tests/test_lead_basics.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     4038 2024-01-08 17:30:47.000000 lbh15-2.1.0/tests/test_lead_fromX_spanT.py
```

### Comparing `lbh15-2.0.0/LICENSE` & `lbh15-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lbh15-2.0.0/PKG-INFO` & `lbh15-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbh15
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python implementation of liquid metal properties from Handbook on Lead-bismuth Eutectic Alloy and Lead Properties, Materials Compatibility, Thermal-hydraulics and Technologies
 Author: Daniele Panico, Daniele Tomatis, Gabriele Ottino
 Author-email: Daniele Panico <daniele.panico@newcleo.com>, Daniele Tomatis <daniele.tomatis@newcleo.com>
 License: lgpl v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -14,31 +14,41 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: scipy>=1.8.1
+Requires-Dist: numpy>=1.22.3
+Requires-Dist: sphinx>=6.2.1
+Requires-Dist: sphinx-rtd-theme>=1.3.0
+Requires-Dist: myst-parser>=1.0.0
+Requires-Dist: sphinxcontrib-bibtex>=2.5.0
 
 lbh15
 =====
 
 :Author: Daniele Panico, Daniele Tomatis
 :Contributor: Gabriele Ottino, Lucie Kerleau, Chloé Largeron
-:Date: 08/01/2024
+:Date: 04/04/2024
 
 Introduction
 ------------
 
 *lbh15* (**L**\ ead **B**\ ismuth **H**\ andbook 20\ **15**) is a Python package that implements the
 thermo-physical and the thermo-chemical properties of lead, bismuth and lead-bismuth eutectic (lbe) metal alloy available from
 the handbook edited by 
-`OECD/NEA <https://www.oecd-nea.org/jcms/pl_14972/handbook-on-lead-bismuth-eutectic-alloy-and-lead-properties-materials-compatibility-thermal-hydraulics-and-technologies-2015-edition?details=true>`_
+`OECD/NEA <https://www.oecd-nea.org/jcms/pl_14972/handbook-on-lead-bismuth-eutectic-alloy-and-lead-properties-materials-compatibility-thermal-hydraulics-and-technologies-2015-edition?details=true>`_.
 
-*lbh15* is released under the **GNU Lesser General Public License 3**.
+*lbh15* offers a standard implementation for use of these properties in scientific applications.
+In particular, this package is used for numerical simulation and experimental activities supporting the
+development of nuclear reactors that employ heavy liquid metals as primary coolant.
+
+*lbh15* is developed by the **Codes & Methods** group of `newcleo <https://www.newcleo.com/>`_ and it is released under the **GNU Lesser General Public License 3**.
 
 *lbh15* is listed among the Open-source Nuclear Codes for Reactor Analysis (`ONCORE <https://nucleus.iaea.org/sites/oncore/SitePages/List%20of%20Codes.aspx>`_) by IAEA.
 
 Project Structure
 -----------------
 
 The project is organized according to the following folder structure:
@@ -116,14 +126,21 @@
       make latexpdf
 
 The *html* documentation is available on GitHub Pages at `newcleo-dev-team.github.io/lbh15 <https://newcleo-dev-team.github.io/lbh15/index.html>`_.
 
 To see the available templates for generating the documentation in *PDF* format and to choose among them, please
 look at the ``docs/conf.py`` file.
 
+How to Contribute
+-----------------
+
+For anyone wishing to contribute to the development of the project, report issues
+or problems with the software, or request support, please refer to this
+`web page <https://github.com/newcleo-dev-team/lbh15/blob/master/CONTRIBUTIONS.rst>`_.
+
 How to Cite
 -----------
 
 .. code-block:: latex
 
   @inproceedings{NURETH20lbh15,
     author = {Panico, Daniele and Tomatis, Daniele},
```

### Comparing `lbh15-2.0.0/README.rst` & `lbh15-2.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 lbh15
 =====
 
 :Author: Daniele Panico, Daniele Tomatis
 :Contributor: Gabriele Ottino, Lucie Kerleau, Chloé Largeron
-:Date: 08/01/2024
+:Date: 04/04/2024
 
 Introduction
 ------------
 
 *lbh15* (**L**\ ead **B**\ ismuth **H**\ andbook 20\ **15**) is a Python package that implements the
 thermo-physical and the thermo-chemical properties of lead, bismuth and lead-bismuth eutectic (lbe) metal alloy available from
 the handbook edited by 
-`OECD/NEA <https://www.oecd-nea.org/jcms/pl_14972/handbook-on-lead-bismuth-eutectic-alloy-and-lead-properties-materials-compatibility-thermal-hydraulics-and-technologies-2015-edition?details=true>`_
+`OECD/NEA <https://www.oecd-nea.org/jcms/pl_14972/handbook-on-lead-bismuth-eutectic-alloy-and-lead-properties-materials-compatibility-thermal-hydraulics-and-technologies-2015-edition?details=true>`_.
 
-*lbh15* is released under the **GNU Lesser General Public License 3**.
+*lbh15* offers a standard implementation for use of these properties in scientific applications.
+In particular, this package is used for numerical simulation and experimental activities supporting the
+development of nuclear reactors that employ heavy liquid metals as primary coolant.
+
+*lbh15* is developed by the **Codes & Methods** group of `newcleo <https://www.newcleo.com/>`_ and it is released under the **GNU Lesser General Public License 3**.
 
 *lbh15* is listed among the Open-source Nuclear Codes for Reactor Analysis (`ONCORE <https://nucleus.iaea.org/sites/oncore/SitePages/List%20of%20Codes.aspx>`_) by IAEA.
 
 Project Structure
 -----------------
 
 The project is organized according to the following folder structure:
@@ -95,14 +99,21 @@
       make latexpdf
 
 The *html* documentation is available on GitHub Pages at `newcleo-dev-team.github.io/lbh15 <https://newcleo-dev-team.github.io/lbh15/index.html>`_.
 
 To see the available templates for generating the documentation in *PDF* format and to choose among them, please
 look at the ``docs/conf.py`` file.
 
+How to Contribute
+-----------------
+
+For anyone wishing to contribute to the development of the project, report issues
+or problems with the software, or request support, please refer to this
+`web page <https://github.com/newcleo-dev-team/lbh15/blob/master/CONTRIBUTIONS.rst>`_.
+
 How to Cite
 -----------
 
 .. code-block:: latex
 
   @inproceedings{NURETH20lbh15,
     author = {Panico, Daniele and Tomatis, Daniele},
```

### Comparing `lbh15-2.0.0/lbh15/__init__.py` & `lbh15-2.1.0/lbh15/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """__init__ module of lbh15 package"""
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 __author__ = "Daniele Panico, Daniele Tomatis, Gabriele Ottino"
 __company__ = "newcleo"
-__date__ = "08 January 2024"
+__date__ = "04 April 2024"
 
 from .lead import Lead
 from .bismuth import Bismuth
 from .lbe import LBE
 from .properties import lead_properties
 from .properties import bismuth_properties
 from .properties import lbe_properties
```

### Comparing `lbh15-2.0.0/lbh15/_commons.py` & `lbh15-2.1.0/lbh15/_commons.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # KEYWORDS
 
 # LEAD CONSTANTS
 LEAD_MELTING_TEMPERATURE: float = 600.6  # [K]
 LEAD_MELTING_LATENT_HEAT: float = 23.07e3  # [J/kg]
 LEAD_BOILING_TEMPERATURE: float = 2021  # [K]
 LEAD_VAPORISATION_HEAT: float = 858.6e3  # [J/kg]
-LEAD_MOLAR_MASS: float = 207.20  # [g/mol]
+LEAD_MOLAR_MASS: float = 0.20720  # [kg/mol]
 
 # BISMUTH CONSTANTS
 BISMUTH_MELTING_TEMPERATURE: float = 544.6  # [K]
 BISMUTH_MELTING_LATENT_HEAT: float = 53.3e3  # [J/kg]
 BISMUTH_BOILING_TEMPERATURE: float = 1831  # [K]
 BISMUTH_VAPORISATION_HEAT: float = 856.2e3  # [J/kg]
-BISMUTH_MOLAR_MASS: float = 208.98  # [g/mol]
+BISMUTH_MOLAR_MASS: float = 0.20898  # [kg/mol]
 
 # LEAD-BISMUTH-EUTECTIC CONSTANTS
 LBE_MELTING_TEMPERATURE: float = 398.0  # [K]
 LBE_MELTING_LATENT_HEAT: float = 38.6e3  # [J/kg]
 LBE_BOILING_TEMPERATURE: float = 1927  # [K]
 LBE_VAPORISATION_HEAT: float = 856.6e3  # [J/kg]
 LBE_MOLAR_MASS: float = 0.55*BISMUTH_MOLAR_MASS \
-    + 0.45*LEAD_MOLAR_MASS  # [g/mol]
+    + 0.45*LEAD_MOLAR_MASS  # [kg/mol]
 
 # OXYGEN CONSTANT
-OXYGEN_MOLAR_MASS: float = 16  # [g/mol]
+OXYGEN_MOLAR_MASS: float = 0.016  # [kg/mol]
```

### Comparing `lbh15-2.0.0/lbh15/_decorators.py` & `lbh15-2.1.0/lbh15/_decorators.py`

 * *Files identical despite different names*

### Comparing `lbh15-2.0.0/lbh15/_lbh15.py` & `lbh15-2.1.0/lbh15/_lbh15.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Module with the definition of liquid metal object base class,
 i.e., LiquidMetalInterface"""
 import warnings
 import sys
 import inspect
 import importlib
-import os.path
-import platform
+import pathlib
 import copy
 from abc import ABC
 from abc import abstractmethod
 from collections import defaultdict
 from typing import Dict
 from typing import List
 from typing import Tuple
@@ -261,26 +260,60 @@
         """
         obj_list = cls.__load_properties()
         obj_list += cls.__load_custom_properties()
         rvalue = ['T'] + [obj_list[i].name for i in range(len(obj_list))]
         return list(dict.fromkeys(rvalue))
 
     @classmethod
-    def available_correlations(cls) -> Dict[str, List[str]]:
-        """
-        Returns the dictionary containing the available correlations \
-        for each property.
+    def available_correlations(cls,
+                               properties: Union[str, List[str], None] = None)\
+            -> Dict[str, List[str]]:
+        """
+        Returns the available correlations for the properties passed as
+        argument. Result is formatted as dictionary, where keys are the
+        required property names and values are the corresponding lists
+        of available correlations. In case at least one required property
+        is not among the implemented ones, a warning message is returned
+        listing the names of all the properties that have not been found.
+        In case no value is passed as argument, the available correlations
+        are returned for all the implemented properties.
+
+        Parameters
+        ----------
+        properties : str | List[str] | None
+            name(s) of the property(ies) whose available correlations
+            are to be retrieved. If multiple properties are required,
+            the list of their names must be provided, otherwise a simple
+            string is enough. If the correlations are required for all the
+            implemented properties, then `None` value is to be passed.
 
         Returns
         -------
         Dict[str, List[str]]
         """
         obj_list = cls.__load_properties()
         obj_list += cls.__load_custom_properties()
-        return cls.__extract_available_correlations(obj_list)
+        props_dict = cls.__extract_available_correlations(obj_list)
+
+        # If no argument is passed as input,
+        # return correlations for all the implemented properties
+        if properties is None:
+            return props_dict
+
+        # Check for any required property that is not available
+        if isinstance(properties, str):
+            properties = [properties]
+        props_not_avail = [
+            pr for pr in properties if pr not in props_dict.keys()]
+        if len(props_not_avail) > 0:
+            warnings.warn(f"Required '{props_not_avail}' properties not found!"
+                          "\nPlease check the property name(s) "
+                          "and try again!", stacklevel=5)
+
+        return {k: v for k, v in props_dict.items() if k in properties}
 
     @classmethod
     def set_correlation_to_use(cls, property_name: str,
                                correlation_name: str) -> None:
         """
         Sets the correlation to use for the specified property.
 
@@ -318,24 +351,27 @@
         custom properties.
 
         Parameters
         ----------
         file_path : str
             absolute path of the file where custom properties are implemented
         """
+        # Normalize the path, no matter the OS
+        norm_path = pathlib.Path(file_path)
+
         # Exit if the file passed as argument does not exist
-        if (not os.path.isfile(file_path)):
-            warnings.warn(f"'{file_path}' provided file not found!"
+        if not norm_path.exists():
+            warnings.warn(f"'{norm_path}' provided file not found!"
                           "\nPlease check the file path and try again!"
                           "\nNo custom property added.", stacklevel=5)
             return
-        char = '\\' if 'Windows' in platform.system() else '/'
-        res = file_path.split(char)
-        file_name = res[-1][:-3]
-        path = file_path[:-len(res[-1])]
+
+        # Add filename and the corresponding path to the class dict
+        file_name = norm_path.stem
+        path = str(norm_path.parent)
         if path not in cls._custom_properties_path:
             cls._custom_properties_path[path] = [file_name]
         else:
             cls._custom_properties_path[path].append(file_name)
 
     @classmethod
     def correlations_to_use(cls) -> Dict[str, str]:
@@ -518,16 +554,17 @@
         ----------
         property_object : :class:`_properties.PropertyInterface`
             Object which inherits from :class:`_properties.PropertyInterface`
         """
         key = property_object.name
         self.__properties[key] = property_object
         setattr(self, property_object.name+"_info",
-                lambda: self.__properties[key].info(self.__T, self.__p,
-                                                    True, 0))
+                lambda print_info=True, n_tab=0:
+                    self.__properties[key].info(self.__T, self.__p,
+                                                print_info, n_tab))
 
     def __align_corrs_to_properties(self) -> None:
         """
         This method updates the instance correlation dictionary by
         aligning it to the instance property objects dict. In particular,
         it cleans the dict containing the correlations to use and,
         accordingly, it adapts the property objects dict
```

### Comparing `lbh15-2.0.0/lbh15/bismuth.py` & `lbh15-2.1.0/lbh15/bismuth.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
         - **H** (float) : molar enthalpy :math:`[J/mol]`
         - **S** (float) : molar entropy :math:`[J/(mol \\cdot K)]`
         - **G** (float) : Gibbs free energy :math:`[J/mol]`
         - **fe_sol** (float) : Iron solubility :math:`[wt.\\%]`
         - **ni_sol** (float) : Nickel solubility :math:`[wt.\\%]`
         - **cr_sol** (float) : Chromium solubility :math:`[wt.\\%]`
         - **o_sol** (float) : Oxygen solubility :math:`[wt.\\%]`
-        - **o_dif** (float) : Oxygen diffusivity :math:`[cm^2 / s]`
+        - **o_dif** (float) : Oxygen diffusivity :math:`[m^2 / s]`
         - **o_pp** (float) : Oxygen partial pressure divided by Oxygen \
-            concentration squared :math:`[atm / wt.\\%^2]`
+            concentration squared :math:`[Pa / wt.\\%^2]`
 
     Example
     -------
     >>> liquid_bismuth = Bismuth(T=670.0)
     >>> liquid_bismuth.k  # [W/(m*K)]
     13.705
     """
```

### Comparing `lbh15-2.0.0/lbh15/lbe.py` & `lbh15-2.1.0/lbh15/lbe.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         - **G** (float) : Gibbs free energy :math:`[J/mol]`
         - **pb_a** (float) : Lead chemical activity :math:`[-]`
         - **bi_a** (float) : Bismuth chemical activity :math:`[-]`
         - **fe_sol** (float) : Iron solubility :math:`[wt.\\%]`
         - **ni_sol** (float) : Nickel solubility :math:`[wt.\\%]`
         - **cr_sol** (float) : Chromium solubility :math:`[wt.\\%]`
         - **o_sol** (float) : Oxygen solubility :math:`[wt.\\%]`
-        - **o_dif** (float) : Oxygen diffusivity :math:`[cm^2 / s]`
-        - **fe_dif** (float) : Iron diffusivity :math:`[cm^2 / s]`
+        - **o_dif** (float) : Oxygen diffusivity :math:`[m^2 / s]`
+        - **fe_dif** (float) : Iron diffusivity :math:`[m^2 / s]`
         - **o_pp** (float) : Oxygen partial pressure divided by Oxygen \
-            concentration squared :math:`[atm / wt.\\%^2]`
+            concentration squared :math:`[Pa / wt.\\%^2]`
         - **lim_fe_sat** (float) : Lower limit of Oxygen concentration with \
             Iron at saturation :math:`[wt.\\%]`
         - **lim_cr_sat** (float) : Lower limit of Oxygen concentration with \
             Chromium at saturation :math:`[wt.\\%]`
         - **lim_ni_sat** (float) : Lower limit of Oxygen concentration with \
             Nickel at saturation :math:`[wt.\\%]`
         - **lim_si_sat** (float) : Lower limit of Oxygen concentration with \
```

### Comparing `lbh15-2.0.0/lbh15/lead.py` & `lbh15-2.1.0/lbh15/lead.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,22 +45,22 @@
         - **S** (float) : molar entropy :math:`[J/(mol \\cdot K)]`
         - **G** (float) : Gibbs free energy :math:`[J/mol]`
         - **fe_sol** (float) : Iron solubility :math:`[wt.\\%]`
         - **ni_sol** (float) : Nickel solubility :math:`[wt.\\%]`
         - **cr_sol** (float) : Chromium solubility :math:`[wt.\\%]`
         - **si_sol** (float) : Silicon solubility :math:`[wt.\\%]`
         - **o_sol** (float) : Oxygen solubility :math:`[wt.\\%]`
-        - **o_dif** (float) : Oxygen diffusivity :math:`[cm^2 / s]`
-        - **fe_dif** (float) : Iron diffusivity :math:`[cm^2 / s]`
-        - **co_dif** (float) : Cobalt diffusivity :math:`[cm^2 / s]`
-        - **se_dif** (float) : Selenium diffusivity :math:`[cm^2 / s]`
-        - **in_dif** (float) : Indium diffusivity :math:`[cm^2 / s]`
-        - **te_dif** (float) : Tellurium diffusivity :math:`[cm^2 / s]`
+        - **o_dif** (float) : Oxygen diffusivity :math:`[m^2 / s]`
+        - **fe_dif** (float) : Iron diffusivity :math:`[m^2 / s]`
+        - **co_dif** (float) : Cobalt diffusivity :math:`[m^2 / s]`
+        - **se_dif** (float) : Selenium diffusivity :math:`[m^2 / s]`
+        - **in_dif** (float) : Indium diffusivity :math:`[m^2 / s]`
+        - **te_dif** (float) : Tellurium diffusivity :math:`[m^2 / s]`
         - **o_pp** (float) : Oxygen partial pressure divided by Oxygen \
-            concentration squared :math:`[atm / wt.\\%^2]`
+            concentration squared :math:`[Pa / wt.\\%^2]`
         - **lim_fe_sat** (float) : Lower limit of Oxygen concentration with \
             Iron at saturation :math:`[wt.\\%]`
         - **lim_cr_sat** (float) : Lower limit of Oxygen concentration with \
             Chromium at saturation :math:`[wt.\\%]`
         - **lim_ni_sat** (float) : Lower limit of Oxygen concentration with \
             Nickel at saturation :math:`[wt.\\%]`
         - **lim_si_sat** (float) : Lower limit of Oxygen concentration with \
```

### Comparing `lbh15-2.0.0/lbh15/properties/bismuth_properties.py` & `lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/diffusivity_in_lead.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,41 @@
-"""Module with the definition of the thermo-physical property objects
-for *bismuth*."""
+"""Module with the definition of the *diffusivity*
+property objects for *lead*."""
 from typing import List
-from typing import Union
 import numpy as np
 from scipy.constants import atm
-from .interface import PropertyInterface
-from .._decorators import range_warning
-from .._commons import BISMUTH_MELTING_TEMPERATURE as T_m0
-from .._commons import BISMUTH_BOILING_TEMPERATURE as T_b0
+from scipy.constants import R
+from ..interface import PropertyInterface
+from ..tch_common_interface import OxygenDiffusivityInterface
+from ..tch_common_interface import IronDiffusivityInterface
+from ..._decorators import range_warning
 
 
-class p_s(PropertyInterface):
+class LeadOxygenDiffusivityInterface(OxygenDiffusivityInterface):
     """
-    Liquid bismuth *saturation vapour pressure* property class.
+    Liquid lead *Oxygen diffusivity* property abstract class.
+    """
+    @property
+    def description(self) -> str:
+        """
+        str : Oxygen diffusivity description
+        """
+        return f"{self.long_name} in liquid lead"
+
+
+class OxygenDiffusivityArcella1968(LeadOxygenDiffusivityInterface):
+    """
+    Liquid lead *Oxygen diffusivity* property class
+    implementing the correlation by *arcella1968*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *saturation vapour pressure* by
+        Returns the value of the *Oxygen diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -31,87 +44,44 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            saturation vapour pressure in :math:`[Pa]`
-        """
-        return 2.67e10 * np.exp(-22858/T)
-
-    def initialization_helper(self,
-                              property_value: float) -> Union[None, float]:
-        """
-        Returns the temperature guess value according to the value
-        of the saturation vapour pressure passed as argument.
-        It is used by the root finder algorithm.
-
-        Parameters
-        ----------
-        property_value : float
-            saturation vapour pressure in :math:`[Pa]`
-
-        Returns
-        -------
-        float
-            Temperature guess value in :math:`[K]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        if property_value < 1e-2:
-            return 800
-        if 1e-2 <= property_value < 1e2:
-            return 1200
-        return 2000
+        return np.exp(-14979 / R / T) * 6.32e-9
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return 'sobolev2011'
+        return "arcella1968"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the saturation vapour
-        pressure correlation function
-        """
-        return [T_m0, T_b0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Saturation vapour pressure unit
-        """
-        return "[Pa]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Saturation vapour pressure long name
-        """
-        return "saturation vapour pressure"
-
-    @property
-    def description(self) -> str:
-        """
-        str : Saturation vapour pressure description
+        List[float] : Temperature validity range of the Oxygen diffusivity
+        correlation function
         """
-        return f"Liquid bismuth {self.long_name}"
+        return [973, 1173]
 
 
-class sigma(PropertyInterface):
+class OxygenDiffusivityHomna1971(LeadOxygenDiffusivityInterface):
     """
-    Liquid bismuth *surface tension* property class.
+    Liquid lead *Oxygen diffusivity* property class
+    implementing the correlation by *homna1971*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *surface tension* by
+        Returns the value of the *Oxygen diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -120,65 +90,45 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            surface tension in :math:`[N/m]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return (420.8 - 0.081*T)*1e-3
+        return np.exp(-20083 / R / T) * 9.65e-9
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return 'sobolev2011'
+        return "homna1971"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the surface
-        tension correlation function
-        """
-        return [T_m0, 1400.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Surface tension unit
-        """
-        return "[N/m]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Surface tension long name
-        """
-        return "surface tension"
-
-    @property
-    def description(self) -> str:
-        """
-        str : Surface tension description
+        List[float] : Temperature validity range of the Oxygen diffusivity
+        correlation function
         """
-        return f"Liquid bismuth {self.long_name}"
+        return [1073, 1373]
 
 
-class rho(PropertyInterface):
+class OxygenDiffusivitySwzarc1972(LeadOxygenDiffusivityInterface):
     """
-    Liquid bismuth *density* property class.
+    Liquid lead *Oxygen diffusivity* property class
+    implementing the correlation by *swzarc1972*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *density* by applying the property
-        correlation.
+        Returns the value of the *Oxygen diffusivity* by
+        applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
             Pressure in :math:`[Pa]`, by default the atmospheric pressure
@@ -186,69 +136,44 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            density in :math:`[kg/m^3]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        rho_0 = 10725 - 1.22 * T
-        u_s_val = u_s().correlation(T, p)
-        alpha_val = alpha().correlation(T, p)
-        return rho_0 +\
-            (1 / u_s_val / u_s_val
-             + T * alpha_val * alpha_val / cp().correlation(T, p)) * (p - atm)
+        return np.exp(-25942 / R / T) * 1.44e-7
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "imbeni1998"
+        return "swzarc1972"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the density
+        List[float] : Temperature validity range of the Oxygen diffusivity
         correlation function
         """
-        return [T_m0, T_b0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Density unit
-        """
-        return "[kg/m^3]"
+        return [1013, 1353]
 
-    @property
-    def long_name(self) -> str:
-        """
-        str : Density long name
-        """
-        return "density"
 
-    @property
-    def description(self) -> str:
-        """
-        str : Density description
-        """
-        return f"Liquid bismuth {self.long_name}"
-
-
-class alpha(PropertyInterface):
+class OxygenDiffusivityOtsuka1975(LeadOxygenDiffusivityInterface):
     """
-    Liquid bismuth *thermal expansion coefficient* property class.
+    Liquid lead *Oxygen diffusivity* property class
+    implementing the correlation by *otsuka1975*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *thermal expansion coefficient* by
+        Returns the value of the *Oxygen diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -257,57 +182,44 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            thermal expansion coefficient in :math:`[1/K]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return 1/(8791 - T)
+        return np.exp(-19497 / R / T) * 1.48e-7
 
     @property
-    def range(self) -> List[float]:
-        """
-        List[float] : Temperature validity range of the thermal expansion
-        coefficient correlation function
-        """
-        return [T_m0, T_b0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Thermal expansion coefficient unit
-        """
-        return "[1/K]"
-
-    @property
-    def long_name(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Thermal expansion coefficient long name
+        str : Name of the correlation
         """
-        return "thermal expansion coefficient"
+        return "otsuka1975"
 
     @property
-    def description(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Thermal expansion coefficient description
+        List[float] : Temperature validity range of the Oxygen diffusivity
+        correlation function
         """
-        return f"Liquid bismuth {self.long_name}"
+        return [1173, 1373]
 
 
-class u_s(PropertyInterface):
+class OxygenDiffusivityCharle1976(LeadOxygenDiffusivityInterface):
     """
-    Liquid bismuth *sound velocity* property class.
+    Liquid lead *Oxygen diffusivity* property class
+    implementing the correlation by *charle1976*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *sound velocity* by
+        Returns the value of the *Oxygen diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -316,64 +228,44 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            sound velocity in :math:`[m/s]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return 1616 + T * (0.187 - 2.2e-4 * T)
+        return np.exp(-20927 / R / T) * 1.90e-7
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return 'sobolev2011'
+        return "charle1976"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the sound velocity
+        List[float] : Temperature validity range of the Oxygen diffusivity
         correlation function
         """
-        return [T_m0, 1800.0]
+        return [1173, 1373]
 
-    @property
-    def units(self) -> str:
-        """
-        str : Sound velocity unit
-        """
-        return "[m/s]"
 
-    @property
-    def long_name(self) -> str:
-        """
-        str : Sound velocity long name
-        """
-        return "sound velocity"
-
-    @property
-    def description(self) -> str:
-        """
-        str : Sound velocity description
-        """
-        return "Sound velocity in liquid bismuth"
-
-
-class beta_s(PropertyInterface):
+class OxygenDiffusivityGromov1996(LeadOxygenDiffusivityInterface):
     """
-    Liquid bismuth *isentropic compressibility* property class.
+    Liquid lead *Oxygen diffusivity* property class
+    implementing the correlation by *gromov1996*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *isentropic compressibility* by
+        Returns the value of the *Oxygen diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -382,58 +274,44 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            isentropic compressibility in :math:`[1/Pa]`
-        """
-        u_s_val = u_s().correlation(T, p)
-        return 1 / (rho().correlation(T, p) * u_s_val * u_s_val)
-
-    @property
-    def range(self) -> List[float]:
-        """
-        List[float] : Temperature validity range of the isentropic
-        compressibility correlation function
+            diffusivity in :math:`[m^2 / s]`
         """
-        return [T_m0, 1800.0]
+        return np.exp(-16158 / R / T) * 6.6e-9
 
     @property
-    def units(self) -> str:
-        """
-        str : Isentropic compressibility unit
-        """
-        return "[1/Pa]"
-
-    @property
-    def long_name(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Isentropic compressibility long name
+        str : Name of the correlation
         """
-        return "isentropic compressibility"
+        return "gromov1996"
 
     @property
-    def description(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Isentropic compressibility description
+        List[float] : Temperature validity range of the Oxygen diffusivity
+        correlation function
         """
-        return f"Liquid bismuth {self.long_name}"
+        return [673, 1273]
 
 
-class cp(PropertyInterface):
+class OxygenDiffusivityGanesan2006b(LeadOxygenDiffusivityInterface):
     """
-    Liquid bismuth *specific heat capacity* property class.
+    Liquid lead *Oxygen diffusivity* property class
+    implementing the correlation by *ganesan2006b*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *specific heat capacity* by
+        Returns the value of the *Oxygen diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -442,72 +320,88 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            specific heat capacity in :math:`[J/(kg \\cdot K)]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return 118.2 + 5.934e-3*T + 7.183e6/T/T
+        return np.exp(-45587 / R / T) * 2.79e-7
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "imbeni1998"
-
-    @property
-    def is_injective(self) -> bool:
-        """
-        bool : `True` if the correlation is injective,
-        `False` otherwise.
-        """
-        return False
+        return "ganesan2006b"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the specific heat
-        capacity correlation function
+        List[float] : Temperature validity range of the Oxygen diffusivity
+        correlation function
         """
-        return [T_m0, T_b0]
+        return [823, 1053]
 
-    @property
-    def units(self) -> str:
+
+class IronDiffusivity(IronDiffusivityInterface):
+    """
+    Liquid lead *Iron diffusivity* property class.
+    """
+    @range_warning
+    def correlation(self, T: float, p: float = atm,
+                    verbose: bool = False) -> float:
         """
-        str : Specific heat capacity unit
+        Returns the value of the *Iron diffusivity* by
+        applying the property correlation.
+
+        Parameters
+        ----------
+        T : float
+            Temperature in :math:`[K]`
+        p : float, optional
+            Pressure in :math:`[Pa]`, by default the atmospheric pressure
+            value, i.e., :math:`101325.0 Pa`
+        verbose : bool, optional
+            `True` to tell the decorator to print a warning message in case of
+            range check failing, `False` otherwise. By default, `False`
+
+        Returns
+        -------
+        float:
+            diffusivity in :math:`[m^2 / s]`
         """
-        return "[J/(kg*K)]"
+        return np.power(10, - 2.31 - 2295 / T) * 1.0e-4
 
     @property
-    def long_name(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Specific heat capacity long name
+        List[float] : Temperature validity range of the Iron diffusivity
+        correlation function
         """
-        return "specific heat capacity"
+        return [973.0, 1273.0]
 
     @property
     def description(self) -> str:
         """
-        str : Specific heat capacity description
+        str : Iron diffusivity description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"{self.long_name} in liquid lead"
 
 
-class h(PropertyInterface):
+class CobaltDiffusivity(PropertyInterface):
     """
-    Liquid bismuth *specific enthalpy* property class.
+    Liquid lead *Cobalt diffusivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *specific enthalpy* by
+        Returns the value of the *Cobalt diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -516,67 +410,64 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            specific enthalpy in :math:`[J/kg]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return T * (118.2 + 2.967e-3 * T) - T_m0 * (118.2 + 2.967e-3 * T_m0)\
-            - 7.183e6 * (1 / T - 1 / T_m0)
+        return np.exp(-22154 / R / T) * 4.6e-8
 
     @property
-    def correlation_name(self) -> str:
+    def name(self) -> str:
         """
-        str : Name of the correlation
+        str : Name of the property
         """
-        return 'sobolev2011'
+        return "co_dif"
 
     @property
-    def range(self) -> List[float]:
+    def units(self) -> str:
         """
-        List[float] : Temperature validity range of the specific enthalpy
-        correlation function
+        str : Cobalt diffusivity unit
         """
-        return [T_m0, T_b0]
+        return "[m^2.s^-1]"
 
     @property
-    def units(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Specific enthalpy unit
+        List[float] : Temperature validity range of the Cobalt diffusivity
+        correlation function
         """
-        return "[J/kg]"
+        return [1023.0, 1273.0]
 
     @property
     def long_name(self) -> str:
         """
-        str : Specific enthalpy long name
+        str : Cobalt diffusivity long name
         """
-        return "specific enthalpy"
+        return "cobalt diffusivity"
 
     @property
     def description(self) -> str:
         """
-        str : Specific enthalpy description
+        str : Cobalt diffusivity description
         """
-        return (f"Liquid bismuth {self.long_name} "
-                "(as difference with respect to "
-                "the melting point enthalpy)")
+        return f"{self.long_name} in liquid lead"
 
 
-class mu(PropertyInterface):
+class SeleniumDiffusivity(PropertyInterface):
     """
-    Liquid bismuth *dynamic viscosity* property class.
+    Liquid lead *Selenium diffusivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *dynamic viscosity* by
+        Returns the value of the *Selenium diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -585,64 +476,64 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            dynamic viscosity in :math:`[Pa \\cdot s]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return 4.456e-4*np.exp(780/T)
+        return np.exp(-12958 / R / T) * 3.4e-8
 
     @property
-    def correlation_name(self) -> str:
+    def name(self) -> str:
         """
-        str : name of the correlation
+        str : Name of the property
         """
-        return "lucas1984b"
+        return "se_dif"
 
     @property
-    def range(self) -> List[float]:
+    def units(self) -> str:
         """
-        List[float] : Temperature validity range of the dynamic viscosity
-        correlation function
+        str : Selenium diffusivity unit
         """
-        return [T_m0, 1300.0]
+        return "[m^2.s^-1]"
 
     @property
-    def units(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Dynamic viscosity unit
+        List[float] : Temperature validity range of the Selenium diffusivity
+        correlation function
         """
-        return "[Pa*s]"
+        return [823.0, 1173.0]
 
     @property
     def long_name(self) -> str:
         """
-        str : Dynamic viscosity long name
+        str : Selenium diffusivity long name
         """
-        return "dynamic viscosity"
+        return "selenium diffusivity"
 
     @property
     def description(self) -> str:
         """
-        str : Dynamic viscosity description
+        str : Selenium diffusivity description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"{self.long_name} in liquid lead"
 
 
-class r(PropertyInterface):
+class IndiumDiffusivity(PropertyInterface):
     """
-    Liquid bismuth *electrical resistivity* property class.
+    Liquid lead *Indium diffusivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *electrical resistivity* by
+        Returns the value of the *Indium diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -651,57 +542,64 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            electrical resistivity in :math:`[Ohm \\cdot m]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return (98.96 + 0.0554*T)*1e-8
+        return np.exp(-13794 / R / T) * 3.1e-8
 
     @property
-    def range(self) -> List[float]:
+    def name(self) -> str:
         """
-        List[float] : Temperature validity range of the electrical
-        resistivity correlation function
+        str : Name of the property
         """
-        return [545.0, 1423.0]
+        return "in_dif"
 
     @property
     def units(self) -> str:
         """
-        str : Electrical resistivity unit
+        str : Indium diffusivity unit
         """
-        return "[Ohm*m]"
+        return "[m^2.s^-1]"
+
+    @property
+    def range(self) -> List[float]:
+        """
+        List[float] : Temperature validity range of the Indium diffusivity
+        correlation function
+        """
+        return [723.0, 1173.0]
 
     @property
     def long_name(self) -> str:
         """
-        str : Electrical resistivity long name
+        str : Indium diffusivity long name
         """
-        return "electrical resistivity"
+        return "indium diffusivity"
 
     @property
     def description(self) -> str:
         """
-        str : Electrical resistivity description
+        str : Indium diffusivity description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"{self.long_name} in liquid lead"
 
 
-class k(PropertyInterface):
+class TelluriumDiffusivity(PropertyInterface):
     """
-    Liquid bismuth *thermal conductivity* property class.
+    Liquid lead *Tellurium diffusivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *thermal conductivity* by
+        Returns the value of the *Tellurium diffusivity* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -710,46 +608,46 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            thermal conductivity in :math:`[W/(m \\cdot K)]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return 7.34 + 9.5e-3*T
+        return np.exp(-15884 / R / T) * 3.1e-8
 
     @property
-    def correlation_name(self) -> str:
+    def name(self) -> str:
         """
-        str : Name of the correlation
+        str : Name of the property
         """
-        return "touloukian1970b"
+        return "te_dif"
 
     @property
-    def range(self) -> List[float]:
+    def units(self) -> str:
         """
-        List[float] : Temperature validity range of the thermal
-        conductivity correlation function
+        str : Tellurium diffusivity unit
         """
-        return [T_m0, 1000.0]
+        return "[m^2.s^-1]"
 
     @property
-    def units(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Thermal conductivity unit
+        List[float] : Temperature validity range of the Tellurium diffusivity
+        correlation function
         """
-        return "[W/(m*K)]"
+        return [723.0, 1173.0]
 
     @property
     def long_name(self) -> str:
         """
-        str : Thermal conductivity long name
+        str : Tellurium diffusivity long name
         """
-        return "thermal conductivity"
+        return "tellurium diffusivity"
 
     @property
     def description(self) -> str:
         """
-        str : Thermal conductivity description
+        str : Tellurium diffusivity description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"{self.long_name} in liquid lead"
```

### Comparing `lbh15-2.0.0/lbh15/properties/bismuth_thermochemical_properties/bismuth_thermochemical.py` & `lbh15-2.1.0/lbh15/properties/bismuth_thermochemical_properties/solubility_in_bismuth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,42 @@
-"""Module with the definition of the *thermo-chemical*
+"""Module with the definition of the *solubility*
 property objects for *bismuth*."""
 from typing import List
 from typing import Union
 import numpy as np
 from scipy.constants import atm
-from scipy.constants import R
-from ..interface import PropertyInterface
-from ..bismuth_properties import h
-from ..._commons import BISMUTH_BOILING_TEMPERATURE as T_b0
-from ..._commons import BISMUTH_MELTING_TEMPERATURE as T_m0
-from ..._commons import BISMUTH_MOLAR_MASS as M
-from ..._commons import OXYGEN_MOLAR_MASS as M_O
+from ..tch_common_interface import IronSolubilityInterface
+from ..tch_common_interface import NickelSolubilityInterface
+from ..tch_common_interface import ChromiumSolubilityInterface
+from ..tch_common_interface import OxygenSolubilityInterface
 from ..._decorators import range_warning
 
 
-class OxygenPartialPressureInterface(PropertyInterface):
+class BismuthIronSolubilityInterface(IronSolubilityInterface):
     """
-    *Oxygen partial pressure in liquid bismuth divided by the
-    Oxygen concentration in liquid bismuth squared* property abstract class.
+    Liquid bismuth *Iron solubility* property abstract class.
     """
-    def initialization_helper(self,
-                              property_value: float) -> Union[None, float]:
-        """
-        Returns the temperature guess value according to the value
-        of the Oxygen partial pressure in liquid bismuth divided by the
-        Oxygen concentration in liquid bismuth squared passed as argument.
-        It is used by the root finder algorithm.
-
-        Parameters
-        ----------
-        property_value : float
-            oxygen partial pressure in liquid bismuth divided by the
-            oxygen concentration in liquid bismuth squared
-            in :math:`[atm. /wt.\\%^2]`
-
-        Returns
-        -------
-        float
-            Temperature guess value in :math:`[K]`
-        """
-        if property_value < 1e-4:
-            return 1200
-        return 1500
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "o_pp"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen partial pressure in liquid bismuth divided by the
-        Oxygen concentration in liquid bismuth squared unit
-        """
-        return "[atm.wt.%^-2]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen partial pressure in liquid bismuth divided by the
-        Oxygen concentration in liquid bismuth squared long name
-        """
-        return ("Oxygen partial pressure divided by the"
-                " oxygen concentration squared")
-
     @property
     def description(self) -> str:
         """
-        str : Oxygen partial pressure in liquid bismuth divided by the
-        Oxygen concentration in liquid bismuth squared description
+        str : Iron solubility description
         """
         return f"{self.long_name} in liquid bismuth"
 
 
-class OxygenPartialPressureFitzner1980(OxygenPartialPressureInterface):
+class IronSolubilityGosse2014(BismuthIronSolubilityInterface):
     """
-    *Oxygen partial pressure in liquid bismuth divided by the
-    Oxygen concentration in liquid bismuth squared* property class
-    implementing the correlation by *fitzner1980*.
+    Liquid bismuth *Iron solubility* property class
+    implementing the correlation by *gosse2014*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Oxygen partial pressure in liquid bismuth
-        divided by the Oxygen concentration in liquid bismuth squared* by
+        Returns the value of the *Iron solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -100,49 +45,44 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2 / 2.3 / R * (-95502 / T + 9.69))\
-            * M * M / M_O / M_O
+        return np.power(10, 2.20-3930/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "fitzner1980"
+        return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Oxygen partial
-        pressure divided by the Oxygen concentration squared
+        List[float] : Temperature validity range of the Iron solubility
         correlation function
         """
-        return [988, 1181]
+        return [545.0, 1173.0]
 
 
-class OxygenPartialPressureIsecke1979(OxygenPartialPressureInterface):
+class IronSolubilityMassalski1990(BismuthIronSolubilityInterface):
     """
-    *Oxygen partial pressure in liquid bismuth divided by the
-    Oxygen concentration in liquid bismuth squared* property class
-    implementing the correlation by *isecke1979*.
+    Liquid bismuth *Iron solubility* property class
+    implementing the correlation by *massalski1990*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Oxygen partial pressure in liquid bismuth
-        divided by the Oxygen concentration in liquid bismuth squared* by
+        Returns the value of the *Iron solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -151,49 +91,44 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2 / 2.3 / R * (-101098 / T + 15.66))\
-            * M * M / M_O / M_O
+        return np.power(10, 2.18-3980/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "isecke1979"
+        return "massalski1990"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Oxygen partial
-        pressure divided by the Oxygen concentration squared
+        List[float] : Temperature validity range of the Iron solubility
         correlation function
         """
-        return [973, 1473]
+        return [973.0, 1173.0]
 
 
-class OxygenPartialPressureHahn1979(OxygenPartialPressureInterface):
+class IronSolubilityWeeks1998(BismuthIronSolubilityInterface):
     """
-    *Oxygen partial pressure in liquid bismuth divided by the
-    Oxygen concentration in liquid bismuth squared* property class
-    implementing the correlation by *hahn1979*.
+    Liquid bismuth *Iron solubility* property class
+    implementing the correlation by *weeks1998*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Oxygen partial pressure in liquid bismuth
-        divided by the Oxygen concentration in liquid bismuth squared* by
+        Returns the value of the *Iron solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -202,49 +137,56 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2 / 2.3 / R * (-68156 / T + 14.14))\
-            * M * M / M_O / M_O
+        return np.power(10, 1.832-3589/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "hahn1979"
+        return "weeks1998"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Oxygen partial
-        pressure divided by the Oxygen concentration squared
+        List[float] : Temperature validity range of the Iron solubility
         correlation function
         """
-        return [1073, 1223]
+        return [713.0, 998.0]
 
 
-class OxygenPartialPressureHeshmatpour1981(OxygenPartialPressureInterface):
+class BismuthNickelSolubilityInterface(NickelSolubilityInterface):
     """
-    *Oxygen partial pressure in liquid bismuth divided by the
-    Oxygen concentration in liquid bismuth squared* property class
-    implementing the correlation by *heshmatpour1981*.
+    Liquid bismuth *Nickel solubility* property abstract class.
+    """
+    @property
+    def description(self) -> str:
+        """
+        str : Nickel solubility description
+        """
+        return f"{self.long_name} in liquid bismuth"
+
+
+class NickelSolubilityWeeks1998(BismuthNickelSolubilityInterface):
+    """
+    Liquid bismuth *Nickel solubility* property class
+    implementing the correlation by *weeks1998*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Oxygen partial pressure in liquid bismuth
-        divided by the Oxygen concentration in liquid bismuth squared* by
+        Returns the value of the *Nickel solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -253,46 +195,44 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2 / 2.3 / R * (-95437 / T + 3.78))\
-            * M * M / M_O / M_O
+        return np.power(10, 2.61-1538/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "heshmatpour1981"
+        return "weeks1998"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Oxygen partial
-        pressure divided by the Oxygen concentration squared
+        List[float] : Temperature validity range of the Nickel solubility
         correlation function
         """
-        return [1023, 1273]
+        return [723.0, 903.0]
 
 
-class MolarEnthalpy(PropertyInterface):
+class NickelSolubilityGosse2014(BismuthNickelSolubilityInterface):
     """
-    Liquid bismuth *molar enthalpy variation* property class.
+    Liquid bismuth *Nickel solubility* property class
+    implementing the correlation by *gosse2014*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> float:
+                    verbose: bool = False) -> Union[float, np.ndarray]:
         """
-        Returns the value of the *molar enthalpy variation* by
+        Returns the value of the *Nickel solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -301,64 +241,58 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            molar enthalpy in :math:`[J/mol]`
+            solubility in :math:`[wt.\\%]`
         """
-        return h().correlation(T, p) * M / 1000
+        return np.where(T <= 738, np.power(10, 3.81-2429/T),
+                        np.where(T <= 918, np.power(10, 2.05-1131/T),
+                                 np.power(10, 1.35-484/T)))[()]
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "H"
-
-    @property
-    def units(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Molar enthalpy variation unit
+        str : Name of the correlation
         """
-        return "[J.mol^-1]"
+        return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the molar enthalpy
-        variation correlation function
+        List[float] : Temperature validity range of the Nickel solubility
+        correlation function
         """
-        return [T_m0, T_b0]
+        return [543.0, 1173.0]
 
-    @property
-    def long_name(self) -> str:
-        """
-        str : Molar enthalpy variation long name
-        """
-        return "molar enthalpy variation"
 
+class BismuthChromiumSolubilityInterface(ChromiumSolubilityInterface):
+    """
+    Liquid bismuth *Chromium solubility* property abstract class.
+    """
     @property
     def description(self) -> str:
         """
-        str : Molar enthalpy variation description
+        str : Chromium solubility description
         """
         return f"{self.long_name} in liquid bismuth"
 
 
-class MolarEntropy(PropertyInterface):
+class ChromiumSolubilityVenkatraman1988(BismuthChromiumSolubilityInterface):
     """
-    Liquid bismuth *molar entropy variation* property class.
+    Liquid bismuth *Chromium solubility* property class
+    implementing the correlation by *venkatraman1988*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *molar entropy variation* by
+        Returns the value of the *Chromium solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -367,66 +301,90 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            molar entropy in :math:`[J/(mol \\cdot K)]`
+            solubility in :math:`[wt.\\%]`
         """
-        return M / 1000 * (118.2 * np.log(T / T_m0)
-                           + 5.934e-3 * (T - T_m0)
-                           - 7.183e6 / 2 * (1 / T / T - 1 / T_m0 / T_m0))
+        return np.power(10, 2.34-3610/T)
 
     @property
-    def name(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Name of the property
+        str : Name of the correlation
         """
-        return "S"
+        return "venkatraman1988"
 
     @property
-    def units(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Molar entropy variation unit
+        List[float] : Temperature validity range of the Chromium solubility
+        correlation function
         """
-        return "[J/(mol.K)]"
+        return [658.0, 901.0]
 
-    @property
-    def range(self) -> List[float]:
+
+class ChromiumSolubilityWeeks1998(BismuthChromiumSolubilityInterface):
+    """
+    Liquid bismuth *Chromium solubility* property class
+    implementing the correlation by *weeks1998*.
+    """
+    @range_warning
+    def correlation(self, T: float, p: float = atm,
+                    verbose: bool = False) -> float:
         """
-        List[float] : Temperature validity range of the molar entropy
-        variation correlation function
+        Returns the value of the *Chromium solubility* by
+        applying the property correlation.
+
+        Parameters
+        ----------
+        T : float
+            Temperature in :math:`[K]`
+        p : float, optional
+            Pressure in :math:`[Pa]`, by default the atmospheric pressure
+            value, i.e., :math:`101325.0 Pa`
+        verbose : bool, optional
+            `True` to tell the decorator to print a warning message in case of
+            range check failing, `False` otherwise. By default, `False`
+
+        Returns
+        -------
+        float:
+            solubility in :math:`[wt.\\%]`
         """
-        return [T_m0, T_b0]
+        return np.power(10, 2.5-3717/T)
 
     @property
-    def long_name(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Molar entropy variation long name
+        str : Name of the correlation
         """
-        return "molar entropy variation"
+        return "weeks1998"
 
     @property
-    def description(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Molar entropy variation description
+        List[float] : Temperature validity range of the Chromium solubility
+        correlation function
         """
-        return f"{self.long_name} in liquid bismuth"
+        return [663.0, 998.0]
 
 
-class GibbsFreeEnergy(PropertyInterface):
+class ChromiumSolubilityGosse2014(BismuthChromiumSolubilityInterface):
     """
-    Liquid bismuth *Gibbs free energy variation* property class.
+    Liquid bismuth *Chromium solubility* property class
+    implementing the correlation by *gosse2014*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Gibbs free energy variation* by
+        Returns the value of the *Chromium solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -435,47 +393,71 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            Gibbs free energy in :math:`[J/mol]`
+            solubility in :math:`[wt.\\%]`
         """
-        return MolarEnthalpy().correlation(T, p)\
-            - T * MolarEntropy().correlation(T, p)
+        return np.power(10, 2.34-3610/T)
 
     @property
-    def name(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Name of the property
+        str : Name of the correlation
         """
-        return "G"
+        return "gosse2014"
 
     @property
-    def units(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Gibbs free energy unit
+        List[float] : Temperature validity range of the Chromium solubility
+        correlation function
         """
-        return "[J/mol]"
+        return [545.0, 1773.0]
 
-    @property
-    def range(self) -> List[float]:
+
+class OxygenSolubility(OxygenSolubilityInterface):
+    """
+    Liquid bismuth *Oxygen solubility* property class.
+    """
+    @range_warning
+    def correlation(self, T: float, p: float = atm,
+                    verbose: bool = False) -> Union[float, np.ndarray]:
         """
-        List[float] : Temperature validity range of the Gibbs free energy
-        variation correlation function
+        Returns the value of the *Oxygen solubility* by
+        applying the property correlation.
+
+        Parameters
+        ----------
+        T : float
+            Temperature in :math:`[K]`
+        p : float, optional
+            Pressure in :math:`[Pa]`, by default the atmospheric pressure
+            value, i.e., :math:`101325.0 Pa`
+        verbose : bool, optional
+            `True` to tell the decorator to print a warning message in case of
+            range check failing, `False` otherwise. By default, `False`
+
+        Returns
+        -------
+        float:
+            solubility in :math:`[wt.\\%]`
         """
-        return [T_m0, T_b0]
+        return np.where(T <= 1002, np.power(10, 2.30-4066/T),
+                        np.power(10, 3.04-4810/T))[()]
 
     @property
-    def long_name(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Gibbs free energy long name
+        List[float] : Temperature validity range of the Oxygen solubility
+        correlation function
         """
-        return "Gibbs free energy variation"
+        return [573.0, 1573.0]
 
     @property
     def description(self) -> str:
         """
-        str : Gibbs free energy description
+        str : Oxygen solubility description
         """
         return f"{self.long_name} in liquid bismuth"
```

### Comparing `lbh15-2.0.0/lbh15/properties/bismuth_thermochemical_properties/diffusivity_in_bismuth.py` & `lbh15-2.1.0/lbh15/properties/bismuth_thermochemical_properties/diffusivity_in_bismuth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Module with the definition of the *diffusivity*
 property objects for *bismuth*."""
 from typing import List
 import numpy as np
 from scipy.constants import atm
 from scipy.constants import R
-from lbh15.properties.interface import PropertyInterface
+from ..tch_common_interface import OxygenDiffusivityInterface
 from ..._decorators import range_warning
 
 
-class OxygenDiffusivityInterface(PropertyInterface):
+class BismuthOxygenDiffusivityInterface(OxygenDiffusivityInterface):
     """
     Liquid bismuth *Oxygen diffusivity* property abstract class.
     """
     @property
     def name(self) -> str:
         """
         str : Name of the property
@@ -20,15 +20,15 @@
         return "o_dif"
 
     @property
     def units(self) -> str:
         """
         str : Oxygen diffusivity unit
         """
-        return "[cm^2.s^-1]"
+        return "[m^2.s^-1]"
 
     @property
     def long_name(self) -> str:
         """
         str : Oxygen diffusivity long name
         """
         return "oxygen diffusivity"
@@ -37,15 +37,15 @@
     def description(self) -> str:
         """
         str : Oxygen diffusivity description
         """
         return f"{self.long_name} in liquid bismuth"
 
 
-class OxygenDiffusivityFitzner1980(OxygenDiffusivityInterface):
+class OxygenDiffusivityFitzner1980(BismuthOxygenDiffusivityInterface):
     """
     Liquid bismuth *Oxygen diffusivity* property class
     implementing the correlation by *fitzner1980*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
@@ -63,17 +63,17 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            diffusivity in :math:`[cm^2 / s]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return np.exp(-49229 / R / T) * 1.07e-2
+        return np.exp(-49229 / R / T) * 1.07e-6
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "fitzner1980"
@@ -83,15 +83,15 @@
         """
         List[float] : Temperature validity range of the Oxygen diffusivity
         correlation function
         """
         return [951, 1100]
 
 
-class OxygenDiffusivityHeshmatpour1981(OxygenDiffusivityInterface):
+class OxygenDiffusivityHeshmatpour1981(BismuthOxygenDiffusivityInterface):
     """
     Liquid bismuth *Oxygen diffusivity* property class
     implementing the correlation by *heshmatpour1981*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
@@ -109,17 +109,17 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            diffusivity in :math:`[cm^2 / s]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return np.exp(-26610 / R / T) * 1.98e-4
+        return np.exp(-26610 / R / T) * 1.98e-8
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "heshmatpour1981"
```

### Comparing `lbh15-2.0.0/lbh15/properties/bismuth_thermochemical_properties/solubility_in_bismuth.py` & `lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/solubility_in_lbe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,35 @@
 """Module with the definition of the *solubility*
-property objects for *bismuth*."""
+property objects for *lead-bismuth eutectic* (*lbe*)."""
 from typing import List
 from typing import Union
 import numpy as np
 from scipy.constants import atm
-from lbh15.properties.interface import PropertyInterface
+from ..tch_common_interface import IronSolubilityInterface
+from ..tch_common_interface import NickelSolubilityInterface
+from ..tch_common_interface import ChromiumSolubilityInterface
+from ..tch_common_interface import OxygenSolubilityInterface
 from ..._decorators import range_warning
 
 
-class IronSolubilityInterface(PropertyInterface):
+class LBEIronSolubilityInterface(IronSolubilityInterface):
     """
-    Liquid bismuth *Iron solubility* property abstract class.
+    Liquid lbe *Iron solubility* property abstract class.
     """
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "fe_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Iron solubility unit
-        """
-        return "[wt.%]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Iron solubility long name
-        """
-        return "iron solubility"
-
-    @property
     def description(self) -> str:
         """
         str : Iron solubility description
         """
-        return f"{self.long_name} in liquid bismuth"
+        return f"{self.long_name} in liquid lbe"
 
 
-class IronSolubilityGosse2014(IronSolubilityInterface):
+class IronSolubilityGosse2014(LBEIronSolubilityInterface):
     """
-    Liquid bismuth *Iron solubility* property class
+    Liquid lbe *Iron solubility* property class
     implementing the correlation by *gosse2014*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Iron solubility* by
@@ -65,82 +47,36 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2.20-3930/T)
+        return np.power(10, 2.00-4399/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Iron solubility
         correlation function
         """
-        return [545.0, 1173.0]
-
-
-class IronSolubilityMassalski1990(IronSolubilityInterface):
-    """
-    Liquid bismuth *Iron solubility* property class
-    implementing the correlation by *massalski1990*.
-    """
-    @range_warning
-    def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> float:
-        """
-        Returns the value of the *Iron solubility* by
-        applying the property correlation.
-
-        Parameters
-        ----------
-        T : float
-            Temperature in :math:`[K]`
-        p : float, optional
-            Pressure in :math:`[Pa]`, by default the atmospheric pressure
-            value, i.e., :math:`101325.0 Pa`
-        verbose : bool, optional
-            `True` to tell the decorator to print a warning message in case of
-            range check failing, `False` otherwise. By default, `False`
-
-        Returns
-        -------
-        float:
-            solubility in :math:`[wt.\\%]`
-        """
-        return np.power(10, 2.18-3980/T)
-
-    @property
-    def correlation_name(self) -> str:
-        """
-        str : Name of the correlation
-        """
-        return "massalski1990"
-
-    @property
-    def range(self) -> List[float]:
-        """
-        List[float] : Temperature validity range of the Iron solubility
-        correlation function
-        """
-        return [973.0, 1173.0]
+        return [399.0, 1173.0]
 
 
-class IronSolubilityWeeks1998(IronSolubilityInterface):
+class IronSolubilityWeeks1969(LBEIronSolubilityInterface):
     """
-    Liquid bismuth *Iron solubility* property class
-    implementing the correlation by *weeks1998*.
+    Liquid lbe *Iron solubility* property class
+    implementing the correlation by *weeks1969*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Iron solubility* by
         applying the property correlation.
@@ -157,35 +93,35 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 1.832-3589/T)
+        return np.power(10, 1.85-4164/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "weeks1998"
+        return "weeks1969"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Iron solubility
         correlation function
         """
-        return [713.0, 998.0]
+        return [823.0, 1053.0]
 
 
-class NickelSolubilityInterface(PropertyInterface):
+class LBENickelSolubilityInterface(NickelSolubilityInterface):
     """
-    Liquid bismuth *Nickel solubility* property abstract class.
+    Liquid lbe *Nickel solubility* property abstract class.
     """
     @property
     def name(self) -> str:
         """
         str : Name of the property
         """
         return "ni_sol"
@@ -205,25 +141,25 @@
         return "nickel solubility"
 
     @property
     def description(self) -> str:
         """
         str : Nickel solubility description
         """
-        return f"{self.long_name} in liquid bismuth"
+        return f"{self.long_name} in liquid lbe"
 
 
-class NickelSolubilityWeeks1998(NickelSolubilityInterface):
+class NickelSolubilityMartinelli2010(LBENickelSolubilityInterface):
     """
-    Liquid bismuth *Nickel solubility* property class
-    implementing the correlation by *weeks1998*.
+    Liquid lbe *Nickel solubility* property class
+    implementing the correlation by *martinelli2010*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> float:
+                    verbose: bool = False) -> Union[float, np.ndarray]:
         """
         Returns the value of the *Nickel solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
@@ -236,35 +172,36 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2.61-1538/T)
+        return np.where(T <= 712, np.power(10, 5.2-3500/T),
+                        np.power(10, 1.7-1009/T))[()]
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "weeks1998"
+        return "martinelli2010"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Nickel solubility
         correlation function
         """
-        return [723.0, 903.0]
+        return [603.0, 1173.0]
 
 
-class NickelSolubilityGosse2014(NickelSolubilityInterface):
+class NickelSolubilityGosse2014(LBENickelSolubilityInterface):
     """
-    Liquid bismuth *Nickel solubility* property class
+    Liquid lbe *Nickel solubility* property class
     implementing the correlation by *gosse2014*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> Union[float, np.ndarray]:
         """
         Returns the value of the *Nickel solubility* by
@@ -282,37 +219,36 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.where(T <= 738, np.power(10, 3.81-2429/T),
-                        np.where(T <= 918, np.power(10, 2.05-1131/T),
-                                 np.power(10, 1.35-484/T)))[()]
+        return np.where(T <= 742, np.power(10, 4.32-2933/T),
+                        np.power(10, 1.74-1006/T))[()]
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Nickel solubility
         correlation function
         """
-        return [543.0, 1173.0]
+        return [528.0, 1173.0]
 
 
-class ChromiumSolubilityInterface(PropertyInterface):
+class LBEChromiumSolubilityInterface(ChromiumSolubilityInterface):
     """
-    Liquid bismuth *Chromium solubility* property abstract class.
+    Liquid lbe *Chromium solubility* property abstract class.
     """
     @property
     def name(self) -> str:
         """
         str : Name of the property
         """
         return "cr_sol"
@@ -325,28 +261,28 @@
         return "[wt.%]"
 
     @property
     def long_name(self) -> str:
         """
         str : Chromium solubility long name
         """
-        return "chromium solubility"
+        return "cr solubility"
 
     @property
     def description(self) -> str:
         """
         str : Chromium solubility description
         """
-        return f"{self.long_name} in liquid bismuth"
+        return f"{self.long_name} in liquid lbe"
 
 
-class ChromiumSolubilityVenkatraman1988(ChromiumSolubilityInterface):
+class ChromiumSolubilityGosse2014(LBEChromiumSolubilityInterface):
     """
-    Liquid bismuth *Chromium solubility* property class
-    implementing the correlation by *venkatraman1988*.
+    Liquid lbe *Chromium solubility* property class
+    implementing the correlation by *gosse2014*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Chromium solubility* by
         applying the property correlation.
@@ -363,36 +299,36 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2.34-3610/T)
+        return np.power(10, 1.12-3056/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "venkatraman1988"
+        return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Chromium solubility
         correlation function
         """
-        return [658.0, 901.0]
+        return [399.0, 1173.0]
 
 
-class ChromiumSolubilityWeeks1998(ChromiumSolubilityInterface):
+class ChromiumSolubilityCourouau2004(LBEChromiumSolubilityInterface):
     """
-    Liquid bismuth *Chromium solubility* property class
-    implementing the correlation by *weeks1998*.
+    Liquid lbe *Chromium solubility* property class
+    implementing the correlation by *courouau2004*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Chromium solubility* by
         applying the property correlation.
@@ -409,36 +345,36 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2.5-3717/T)
+        return np.power(10, 1.07-3022/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "weeks1998"
+        return "courouau2004"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Chromium solubility
         correlation function
         """
-        return [663.0, 998.0]
+        return [643.0, 813.0]
 
 
-class ChromiumSolubilityGosse2014(ChromiumSolubilityInterface):
+class ChromiumSolubilityMartynov1998(LBEChromiumSolubilityInterface):
     """
-    Liquid bismuth *Chromium solubility* property class
-    implementing the correlation by *gosse2014*.
+    Liquid lbe *Chromium solubility* property class
+    implementing the correlation by *martynov1998*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Chromium solubility* by
         applying the property correlation.
@@ -455,39 +391,39 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2.34-3610/T)
+        return np.power(10, -0.02-2280/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "gosse2014"
+        return "martynov1998"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Chromium solubility
         correlation function
         """
-        return [545.0, 1773.0]
+        return [673.0, 773.0]
 
 
-class OxygenSolubility(PropertyInterface):
+class OxygenSolubility(OxygenSolubilityInterface):
     """
-    Liquid bismuth *Oxygen solubility* property class.
+    Liquid lbe *Oxygen solubility* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> Union[float, np.ndarray]:
+                    verbose: bool = False) -> float:
         """
         Returns the value of the *Oxygen solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
@@ -500,45 +436,23 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.where(T <= 1002, np.power(10, 2.30-4066/T),
-                        np.power(10, 3.04-4810/T))[()]
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "o_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen solubility unit
-        """
-        return "[wt.%]"
+        return np.power(10, 2.25-4125/T)
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen solubility
         correlation function
         """
-        return [573.0, 1573.0]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen solubility long name
-        """
-        return "oxygen solubility"
+        return [673.0, 1013.0]
 
     @property
     def description(self) -> str:
         """
         str : Oxygen solubility description
         """
-        return "f{self.long_name} in liquid bismuth"
+        return f"{self.long_name} in liquid lbe"
```

### Comparing `lbh15-2.0.0/lbh15/properties/interface.py` & `lbh15-2.1.0/lbh15/properties/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             Temperature in :math:`[K]`
         p : float, optional
             Pressure in :math:`[Pa]`, by default the atmospheric pressure,
             i.e., :math:`101325.0 Pa`
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
-        
+
         Returns
         -------
         exception
         """
         raise NotImplementedError(f"{type(self).__name__}.correlation "
                                   "NOT IMPLEMENTED")
```

### Comparing `lbh15-2.0.0/lbh15/properties/lbe_properties.py` & `lbh15-2.1.0/lbh15/properties/lead_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 """Module with the definition of the thermo-physical property objects
-for *lead-bismuth eutectic*."""
+for *lead*."""
 from typing import List
 from typing import Union
 import numpy as np
 from scipy.constants import atm
-from .interface import PropertyInterface
+from .tph_common_interface import SaturationVapourPressureInterface
+from .tph_common_interface import SurfaceTensionInterface
+from .tph_common_interface import DensityInterface
+from .tph_common_interface import ThermalExpansionInterface
+from .tph_common_interface import SpeedOfSoundInterface
+from .tph_common_interface import IsentropicCompressibilityInterface
+from .tph_common_interface import SpecificHeatInterface
+from .tph_common_interface import SpecificEnthalpyInterface
+from .tph_common_interface import DynamicViscosityInterface
+from .tph_common_interface import ElectricalResistivityInterface
+from .tph_common_interface import ThermalConductivityInterface
 from .._decorators import range_warning
-from .._commons import LBE_MELTING_TEMPERATURE as T_m0
-from .._commons import LBE_BOILING_TEMPERATURE as T_b0
+from .._commons import LEAD_MELTING_TEMPERATURE as T_m0
+from .._commons import LEAD_BOILING_TEMPERATURE as T_b0
 
 
-class p_s(PropertyInterface):
+class p_s(SaturationVapourPressureInterface):
     """
-    Liquid lead-bismuth eutectic *saturation vapour pressure* property class.
+    Liquid lead *saturation vapour pressure* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *saturation vapour pressure* by
         applying the property correlation.
@@ -33,15 +43,15 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             saturation vapour pressure in :math:`[Pa]`
         """
-        return 1.22e10 * np.exp(-22552/T)
+        return 5.76e9 * np.exp(-22131/T)
 
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
         """
         Returns the temperature guess value according to the value
         of the saturation vapour pressure passed as argument.
         It is used by the root finder algorithm.
@@ -74,38 +84,24 @@
         """
         List[float] : Temperature validity range of the saturation vapour
         pressure correlation function
         """
         return [T_m0, T_b0]
 
     @property
-    def units(self) -> str:
-        """
-        str : Saturation vapour pressure unit
-        """
-        return "[Pa]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Saturation vapour pressure long name
-        """
-        return "saturation vapour pressure"
-
-    @property
     def description(self) -> str:
         """
         str : Saturation vapour pressure description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid lead {self.long_name}"
 
 
-class sigma(PropertyInterface):
+class sigma(SurfaceTensionInterface):
     """
-    Liquid lead-bismuth eutectic *surface tension* property class.
+    Liquid lead *surface tension* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *surface tension* by
         applying the property correlation.
@@ -122,56 +118,42 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             surface tension in :math:`[N/m]`
         """
-        return (448.5 - 0.0799*T)*1e-3
+        return (525.9 - 0.113*T)*1e-3
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "plevachuk2008"
+        return "jauch1986"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the surface
         tension correlation function
         """
-        return [T_m0, 1400.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Surface tension unit
-        """
-        return "[N/m]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Surface tension long name
-        """
-        return "surface tension"
+        return [T_m0, 1300.0]
 
     @property
     def description(self) -> str:
         """
         str : Surface tension description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid lead {self.long_name}"
 
 
-class rho(PropertyInterface):
+class rho(DensityInterface):
     """
-    Liquid lead-bismuth eutectic *density* property class.
+    Liquid lead *density* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *density* by applying the property
         correlation. *sobolev2011* correlation is used for the specific
@@ -189,55 +171,48 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             density in :math:`[kg/m^3]`
         """
-        rho_0 = 11065 - 1.293*T
+        rho_0 = 11441 - 1.2795*T
         u_s_val = u_s().correlation(T, p)
         alpha_val = alpha().correlation(T, p)
         return rho_0 +\
-            (1 / u_s_val / u_s_val +
-             T * alpha_val * alpha_val / cp().correlation(T, p)) * (p - atm)
-
-    @property
-    def range(self) -> List[float]:
-        """
-        List[float] : Temperature validity range of the density
-        correlation function
-        """
-        return [T_m0, T_b0]
+            (1.0 / u_s_val / u_s_val +
+             T * alpha_val * alpha_val /
+             cp_sobolev2011().correlation(T, p)) * (p - atm)
 
     @property
-    def units(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Density unit
+        str : Name of the correlation
         """
-        return "[kg/m^3]"
+        return "sobolev2008a"
 
     @property
-    def long_name(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Density long name
+        List[float] : Temperature validity range of the density
+        correlation function
         """
-        return "density"
+        return [T_m0, T_b0]
 
     @property
     def description(self) -> str:
         """
         str : Density description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid lead {self.long_name}"
 
 
-class alpha(PropertyInterface):
+class alpha(ThermalExpansionInterface):
     """
-    Liquid lead-bismuth eutectic *thermal expansion coefficient*
-    property class.
+    Liquid lead *thermal expansion coefficient* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *thermal expansion coefficient* by
         applying the property correlation.
@@ -254,49 +229,35 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             thermal expansion coefficient in :math:`[1/K]`
         """
-        return 1/(8558 - T)
+        return 1/(8942 - T)
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the thermal expansion
         coefficient correlation function
         """
         return [T_m0, T_b0]
 
     @property
-    def units(self) -> str:
-        """
-        str : Thermal expansion coefficient unit
-        """
-        return "[1/K]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Thermal expansion coefficient long name
-        """
-        return "thermal expansion coefficient"
-
-    @property
     def description(self) -> str:
         """
         str : Thermal expansion coefficient description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid lead {self.long_name}"
 
 
-class u_s(PropertyInterface):
+class u_s(SpeedOfSoundInterface):
     """
-    Liquid lead-bismuth eutectic *sound velocity* property class.
+    Liquid lead *sound velocity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *sound velocity* by
         applying the property correlation.
@@ -313,56 +274,42 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             sound velocity in :math:`[m/s]`
         """
-        return 1855 - 0.212*T
+        return 1953 - 0.246*T
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return 'sobolev2011'
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the sound velocity
         correlation function
         """
-        return [400.0, 1100.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Sound velocity unit
-        """
-        return "[m/s]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Sound velocity long name
-        """
-        return "sound velocity"
+        return [T_m0, 2000.0]
 
     @property
     def description(self) -> str:
         """
         str : Sound velocity description
         """
-        return "Sound velocity in liquid lbe"
+        return "Sound velocity in liquid lead"
 
 
-class beta_s(PropertyInterface):
+class beta_s(IsentropicCompressibilityInterface):
     """
-    Liquid lead-bismuth eutectic *isentropic compressibility* property class.
+    Liquid lead *isentropic compressibility* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *isentropic compressibility* by
         applying the property correlation.
@@ -388,41 +335,40 @@
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the isentropic
         compressibility correlation function
         """
-        return [400.0, 1100.0]
+        return [T_m0, 2000.0]
 
     @property
-    def units(self) -> str:
+    def description(self) -> str:
         """
-        str : Isentropic compressibility unit
+        str : Isentropic compressibility description
         """
-        return "[1/Pa]"
+        return f"Liquid lead {self.long_name}"
 
-    @property
-    def long_name(self) -> str:
-        """
-        str : Isentropic compressibility long name
-        """
-        return "isentropic compressibility"
 
+class LeadCpInterface(SpecificHeatInterface):
+    """
+    Liquid lead *specific heat capacity* property interface.
+    """
     @property
-    def description(self) -> str:
+    def name(self) -> str:
         """
-        str : Isentropic compressibility description
+        str : Name of the property
         """
-        return f"Liquid lbe {self.long_name}"
+        return "cp"
 
 
-class cp(PropertyInterface):
+class cp_sobolev2011(LeadCpInterface):
     """
-    Liquid lead-bismuth eutectic *specific heat capacity* property class.
+    Liquid lead *specific heat capacity* property class exploiting
+    the **sobolev2011** correlation.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *specific heat capacity* by
         applying the **sobolev2011** correlation.
@@ -439,64 +385,96 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             specific heat capacity in :math:`[J/(kg \\cdot K)]`
         """
-        return 164.8 - T * (3.94e-2 - 1.25e-5 * T) - 4.56e5 / T / T
+        return 176.2 - T * (4.923e-2 - 1.544e-5 * T) - 1.524e6 / T / T
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return 'sobolev2011'
 
     @property
-    def is_injective(self) -> bool:
+    def range(self) -> List[float]:
         """
-        bool : `True` if the correlation is injective,
-        `False` otherwise.
+        List[float] : Temperature validity range of the specific heat
+        capacity correlation function
         """
-        return False
+        return [T_m0, 2000.0]
 
     @property
-    def range(self) -> List[float]:
+    def description(self) -> str:
         """
-        List[float] : Temperature validity range of the specific heat
-        capacity correlation function
+        str : Specific heat capacity description
         """
-        return [400.0, T_b0]
+        return f"Liquid lead {self.long_name}"
+
+
+class cp_gurvich1991(LeadCpInterface):
+    """
+    Liquid lead *specific heat capacity* property class exploiting
+    the **gurvich1991** correlation.
+    """
+    @range_warning
+    def correlation(self, T: float, p: float = atm,
+                    verbose: bool = False) -> float:
+        """
+        Returns the value of the *specific heat capacity* by
+        applying the **gurvich1991** correlation.
+
+        Parameters
+        ----------
+        T : float
+            Temperature in :math:`[K]`
+        p : float, optional
+            Pressure in :math:`[Pa]`, by default the atmospheric pressure
+            value, i.e., :math:`101325.0 Pa`
+        verbose : bool, optional
+            `True` to tell the decorator to print a warning message in case of
+            range check failing, `False` otherwise. By default, `False`
+
+        Returns
+        -------
+        float:
+            specific heat capacity in :math:`[J/(kg \\cdot K)]`
+        """
+        return 175.1 - T * (4.961e-2 - T * (1.985e-5 - 2.099e-9 * T))\
+            - 1.524e6 / T / T
 
     @property
-    def units(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Specific heat capacity unit
+        str : Name of the correlation
         """
-        return "[J/(kg*K)]"
+        return 'gurvich1991'
 
     @property
-    def long_name(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Specific heat capacity long name
+        List[float] : Temperature validity range of the specific heat
+        capacity correlation function
         """
-        return "specific heat capacity"
+        return [T_m0, 2000.0]
 
     @property
     def description(self) -> str:
         """
         str : Specific heat capacity description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid lead {self.long_name}"
 
 
-class h(PropertyInterface):
+class h(SpecificEnthalpyInterface):
     """
-    Liquid lead-bismuth eutectic *specific enthalpy* property class.
+    Liquid lead *specific enthalpy* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *specific enthalpy* by
         applying the property correlation.
@@ -513,60 +491,46 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             specific enthalpy in :math:`[J/kg]`
         """
-        return T * (164.8 - T * (1.97e-2 - 4.167e-6 * T))\
-            - T_m0 * (164.8 - T_m0 * (1.97e-2 - 4.167e-6 * T_m0))\
-            + 4.56e5 * (1 / T - 1 / T_m0)
+        return T * (176.2 - T * (2.4615e-2 - 5.147e-6 * T))\
+            - T_m0 * (176.2 - T_m0 * (2.4615e-2 - 5.147e-6 * T_m0))\
+            + 1.524e6 * (1 / T - 1 / T_m0)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return 'sobolev2011'
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the specific enthalpy
         correlation function
         """
-        return [400.0, T_b0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Specific enthalpy unit
-        """
-        return "[J/kg]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Specific enthalpy long name
-        """
-        return "specific enthalpy"
+        return [T_m0, 2000.0]
 
     @property
     def description(self) -> str:
         """
-        str : str : Specific enthalpy description
+        str : Specific enthalpy description
         """
-        return (f"Liquid lbe {self.long_name} "
+        return (f"Liquid lead {self.long_name} "
                 "(as difference with respect to "
                 "the melting point enthalpy)")
 
 
-class mu(PropertyInterface):
+class mu(DynamicViscosityInterface):
     """
-    Liquid lead-bismuth eutectic *dynamic viscosity* property class.
+    Liquid lead *dynamic viscosity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *dynamic viscosity* by
         applying the property correlation.
@@ -583,49 +547,56 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             dynamic viscosity in :math:`[Pa \\cdot s]`
         """
-        return 4.94e-4*np.exp(754.1/T)
+        return 4.55e-4 * np.exp(1069/T)
 
-    @property
-    def range(self) -> List[float]:
-        """
-        List[float] : Temperature validity range of the dynamic viscosity
-        correlation function
+    def initialization_helper(self,
+                              property_value: float) -> Union[None, float]:
         """
-        return [T_m0, 1300.0]
+        Returns the temperature guess value according to the value
+        of the dynamic viscosity passed as argument.
+        It is used by the root finder algorithm.
 
-    @property
-    def units(self) -> str:
-        """
-        str : Dynamic viscosity unit
+        Parameters
+        ----------
+        property_value : float
+            dynamic viscosity in :math:`[Pa]`
+
+        Returns
+        -------
+        float
+            Temperature guess value in :math:`[K]`
         """
-        return "[Pa*s]"
+        if property_value < 2e-3:
+            return 800
+        return 1600
 
     @property
-    def long_name(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Dynamic viscosity long name
+        List[float] : Temperature validity range of the dynamic viscosity
+        correlation function
         """
-        return "dynamic viscosity"
+        return [T_m0, 1473.0]
 
     @property
     def description(self) -> str:
         """
         str : Dynamic viscosity description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid lead {self.long_name}"
 
 
-class r(PropertyInterface):
+class r(ElectricalResistivityInterface):
     """
-    Liquid lead-bismuth eutectic *electrical resistivity* property class.
+    Liquid lead *electrical resistivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *electrical resistivity* by
         applying the property correlation.
@@ -642,49 +613,35 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             electrical resistivity in :math:`[Ohm \\cdot m]`
         """
-        return (90.9 + 0.048*T)*1e-8
+        return (67.0 + 0.0471*T)*1e-8
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the electrical
         resistivity correlation function
         """
-        return [400.0, 1100.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Electrical resistivity unit
-        """
-        return "[Ohm*m]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Electrical resistivity long name
-        """
-        return "electrical resistivity"
+        return [T_m0, 1273.0]
 
     @property
     def description(self) -> str:
         """
         str : Electrical resistivity description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid lead {self.long_name}"
 
 
-class k(PropertyInterface):
+class k(ThermalConductivityInterface):
     """
-    Liquid lead-bismuth eutectic *thermal conductivity* property class.
+    Liquid lead *thermal conductivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *thermal conductivity* by
         applying the property correlation.
@@ -701,44 +658,23 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             thermal conductivity in :math:`[W/(m \\cdot K)]`
         """
-        return 3.284 + T * (1.617e-2 - 2.305e-6 * T)
-
-    @property
-    def correlation_name(self) -> str:
-        """
-        str : Name of the correlation
-        """
-        return 'sobolev2011'
+        return 9.2 + 0.011*T
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the thermal
         conductivity correlation function
         """
-        return [T_m0, 1200.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Thermal conductivity unit
-        """
-        return "[W/(m*K)]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Thermal conductivity long name
-        """
-        return "thermal conductivity"
+        return [T_m0, 1300.0]
 
     @property
     def description(self) -> str:
         """
         str : Thermal conductivity description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid lead {self.long_name}"
```

### Comparing `lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/diffusivity_in_lbe.py` & `lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/diffusivity_in_lbe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,30 @@
 """Module with the definition of the *diffusivity*
 property objects for *lead-bismuth eutectic* (*lbe*)."""
 from typing import List
 import numpy as np
 from scipy.constants import atm, R
-from lbh15.properties.interface import PropertyInterface
+from ..tch_common_interface import OxygenDiffusivityInterface
+from ..tch_common_interface import IronDiffusivityInterface
 from ..._decorators import range_warning
 
 
-class OxygenDiffusivityInterface(PropertyInterface):
+class LBEOxygenDiffusivityInterface(OxygenDiffusivityInterface):
     """
     Liquid lbe *Oxygen diffusivity* property abstract class.
     """
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "o_dif"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen diffusivity unit
-        """
-        return "[cm^2.s^-1]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen diffusivity long name
-        """
-        return "oxygen diffusivity"
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen diffusivity description
         """
         return f"{self.long_name} in liquid lbe"
 
 
-class OxygenDiffusivityGromov1996(OxygenDiffusivityInterface):
+class OxygenDiffusivityGromov1996(LBEOxygenDiffusivityInterface):
     """
     Liquid lbe *Oxygen diffusivity* property class
     implementing the correlation by *gromov1996*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
@@ -62,17 +42,17 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            diffusivity in :math:`[cm^2 / s]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return np.exp(-43073 / R / T) * 2.39e-2
+        return np.exp(-43073 / R / T) * 2.39e-6
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "gromov1996"
@@ -82,15 +62,15 @@
         """
         List[float] : Temperature validity range of the Oxygen diffusivity
         correlation function
         """
         return [473, 1273]
 
 
-class OxygenDiffusivityGanesan2006b(OxygenDiffusivityInterface):
+class OxygenDiffusivityGanesan2006b(LBEOxygenDiffusivityInterface):
     """
     Liquid lbe *Oxygen diffusivity* property class
     implementing the correlation by *ganesan2006b*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
@@ -108,17 +88,17 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            diffusivity in :math:`[cm^2 / s]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return np.exp(-69069 / R / T) * 0.154
+        return np.exp(-69069 / R / T) * 0.154e-4
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "ganesan2006b"
@@ -128,15 +108,15 @@
         """
         List[float] : Temperature validity range of the Oxygen diffusivity
         correlation function
         """
         return [813, 973]
 
 
-class IronDiffusivity(PropertyInterface):
+class IronDiffusivity(IronDiffusivityInterface):
     """
     Liquid lbe *Iron diffusivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
@@ -153,46 +133,25 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            diffusivity in :math:`[cm^2 / s]`
+            diffusivity in :math:`[m^2 / s]`
         """
-        return np.power(10, - 2.31 - 2295 / T)
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "fe_dif"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Iron diffusivity unit
-        """
-        return "[cm^2.s^-1]"
+        return np.power(10, - 2.31 - 2295 / T) * 1.0e-4
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Iron diffusivity
         correlation function
         """
         return [973.0, 1273.0]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Iron diffusivity long name
-        """
-        return "iron diffusivity"
-
-    @property
     def description(self) -> str:
         """
         str : Iron diffusivity description
         """
-        return "f{self.long_name} in liquid lbe"
+        return f"{self.long_name} in liquid lbe"
```

### Comparing `lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/lbe_oxygen_limits.py` & `lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/lbe_oxygen_limits.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """Module with the definition of the *Oxygen concentration lower limits*
 objects for *lead-bismuth eutectic* (*lbe*)."""
 from typing import List
 from typing import Union
 import numpy as np
 from scipy.constants import atm
 from scipy.constants import R
-from ..interface import PropertyInterface
+from ..tch_common_interface import LowerLimitSaturationIronInterface
+from ..tch_common_interface import LowerLimitSaturationChromiumInterface
+from ..tch_common_interface import LowerLimitSaturationNickelInterface
+from ..tch_common_interface import LowerLimitSaturationSiliconInterface
+from ..tch_common_interface import LowerLimitSaturationAluminiumInterface
+from ..tch_common_interface import LowerLimitChromiumInterface
+from ..tch_common_interface import LowerLimitNickelInterface
+from ..tch_common_interface import LowerLimitIronInterface
 from .solubility_in_lbe import OxygenSolubility
 from .solubility_in_lbe import ChromiumSolubilityGosse2014
 from .solubility_in_lbe import ChromiumSolubilityCourouau2004
 from .solubility_in_lbe import ChromiumSolubilityMartynov1998
 from .solubility_in_lbe import NickelSolubilityGosse2014
 from .solubility_in_lbe import NickelSolubilityMartinelli2010
 from .solubility_in_lbe import IronSolubilityGosse2014
 from .solubility_in_lbe import IronSolubilityWeeks1969
 from .lbe_thermochemical import LeadChemicalActivity
 from ..._decorators import range_warning
 
 
-class LowerLimitSaturationIron(PropertyInterface):
+class LowerLimitSaturationIron(LowerLimitSaturationIronInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lbe considering
     *Iron at its saturation concentration* property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -74,52 +81,30 @@
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-57190 / R / T - 21.1 / R)\
             * OxygenSolubility().correlation(T, p)\
             * LeadChemicalActivity().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_fe_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                "iron at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lbe"
 
 
-class LowerLimitSaturationChromium(PropertyInterface):
+class LowerLimitSaturationChromium(LowerLimitSaturationChromiumInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lbe considering
     *Chromium at its saturation concentration* property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -171,52 +156,30 @@
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-158900 / R / T - 13.65 / R)\
             * OxygenSolubility().correlation(T, p)\
             * LeadChemicalActivity().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_cr_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                "chromium at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in lbe"
 
 
-class LowerLimitSaturationNickel(PropertyInterface):
+class LowerLimitSaturationNickel(LowerLimitSaturationNickelInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lbe considering
     *Nickel at its saturation concentration* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -244,52 +207,30 @@
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-18040 / R / T - 11.7 / R)\
             * OxygenSolubility().correlation(T, p)\
             * LeadChemicalActivity().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_ni_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                " nickel at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lbe"
 
 
-class LowerLimitSaturationSilicon(PropertyInterface):
+class LowerLimitSaturationSilicon(LowerLimitSaturationSiliconInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lbe considering
     *Silicon at its saturation concentration* property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -343,52 +284,30 @@
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-235855 / R / T - 9.75 / R)\
             * OxygenSolubility().correlation(T, p)\
             * LeadChemicalActivity().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_si_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                " silicon at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lbe"
 
 
-class LowerLimitSaturationAluminium(PropertyInterface):
+class LowerLimitSaturationAluminium(LowerLimitSaturationAluminiumInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lbe considering
     *Aluminium at its saturation concentration* property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -442,52 +361,30 @@
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-339770 / R / T + 5.35 / R)\
             * OxygenSolubility().correlation(T, p)\
             * LeadChemicalActivity().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_al_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                " aluminium at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lbe"
 
 
-class LowerLimitChromiumInterface(PropertyInterface):
+class LBELowerLimitChromiumInterface(LowerLimitChromiumInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Chromium concentration*
     raised to :math:`2/3` in liquid lbe property abstract class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -512,44 +409,22 @@
             Temperature guess value in :math:`[K]`
         """
         if property_value < 1e-7:
             return 1400
         return 1700
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_cr"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit times"
-                " chromium concentration raised to 2/3")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in lbe"
 
 
-class LowerLimitChromiumGosse2014(LowerLimitChromiumInterface):
+class LowerLimitChromiumGosse2014(LBELowerLimitChromiumInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Chromium concentration*
     raised to :math:`2/3` in liquid lbe property class
     implementing the correlation by *gosse2014*.
     """
     @range_warning
@@ -592,15 +467,15 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
 
-class LowerLimitChromiumCourouau2004(LowerLimitChromiumInterface):
+class LowerLimitChromiumCourouau2004(LBELowerLimitChromiumInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Chromium concentration*
     raised to :math:`2/3` in liquid lbe property class
     implementing the correlation by *courouau2004*.
     """
     @range_warning
@@ -644,15 +519,15 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 813]
 
 
-class LowerLimitChromiumMartynov1998(LowerLimitChromiumInterface):
+class LowerLimitChromiumMartynov1998(LBELowerLimitChromiumInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Chromium concentration*
     raised to :math:`2/3` in liquid lbe property class
     implementing the correlation by *martynov1998*.
     """
     @range_warning
@@ -696,51 +571,29 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 773]
 
 
-class LowerLimitNickelInterface(PropertyInterface):
+class LBELowerLimitNickelInterface(LowerLimitNickelInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Nickel concentration*
     in liquid lbe property abstract class.
     """
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_ni"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit times"
-                "nickel concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in lbe"
 
 
-class LowerLimitNickelMartinelli2010(LowerLimitNickelInterface):
+class LowerLimitNickelMartinelli2010(LBELowerLimitNickelInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Nickel concentration*
     in liquid lbe property class
     implementing the correlation by *martinelli2010*.
     """
     @range_warning
@@ -783,15 +636,15 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
 
-class LowerLimitNickelGosse2014(LowerLimitNickelInterface):
+class LowerLimitNickelGosse2014(LBELowerLimitNickelInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Nickel concentration*
     in liquid lbe property class
     implementing the correlation by *gosse2014*.
     """
     @range_warning
@@ -834,15 +687,15 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
 
-class LowerLimitIronInterface(PropertyInterface):
+class LBELowerLimitIronInterface(LowerLimitIronInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Iron concentration*
     raised to :math:`3/4` in liquid lbe property abstract class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -867,44 +720,22 @@
             Temperature guess value in :math:`[K]`
         """
         if property_value < 1e-6:
             return 1200
         return 1700
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_fe"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit times"
-                " iron concentration raised to 3/4")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in lbe"
 
 
-class LowerLimitIronGosse2014(LowerLimitIronInterface):
+class LowerLimitIronGosse2014(LBELowerLimitIronInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Iron concentration*
     raised to :math:`3/4` in liquid lbe property class
     implementing the correlation by *gosse2014*.
     """
     @range_warning
@@ -947,15 +778,15 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
 
-class LowerLimitIronWeeks1969(LowerLimitIronInterface):
+class LowerLimitIronWeeks1969(LBELowerLimitIronInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Iron concentration*
     raised to :math:`3/4` in liquid lbe property class
     implementing the correlation by *weeks1969*.
     """
     @range_warning
```

### Comparing `lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/lbe_thermochemical.py` & `lbh15-2.1.0/lbh15/properties/bismuth_thermochemical_properties/bismuth_thermochemical.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 """Module with the definition of the *thermo-chemical*
-property objects for *lead-bismuth eutectic* (*lbe*)."""
+property objects for *bismuth*."""
 from typing import List
 from typing import Union
 import numpy as np
 from scipy.constants import atm
 from scipy.constants import R
-from ..interface import PropertyInterface
-from ..lbe_properties import h
-from ..._commons import LBE_BOILING_TEMPERATURE as T_b0
-from ..._commons import LBE_MELTING_TEMPERATURE as T_m0
-from ..._commons import LBE_MOLAR_MASS as M
+from ..tch_common_interface import OxygenPartialPressureInterface
+from ..tch_common_interface import MolarEnthalpyInterface
+from ..tch_common_interface import MolarEntropyInterface
+from ..tch_common_interface import GibbsFreeEnergyInterface
+from ..bismuth_properties import h
+from ..._commons import BISMUTH_BOILING_TEMPERATURE as T_b0
+from ..._commons import BISMUTH_MELTING_TEMPERATURE as T_m0
+from ..._commons import BISMUTH_MOLAR_MASS as M
 from ..._commons import OXYGEN_MOLAR_MASS as M_O
 from ..._decorators import range_warning
 
 
-class OxygenPartialPressure(PropertyInterface):
+class BismuthOxygenPartialPressureInterface(OxygenPartialPressureInterface):
     """
-    *Oxygen partial pressure in liquid lbe divided by the
-    Oxygen concentration in liquid lbe squared* property class.
+    *Oxygen partial pressure in liquid bismuth divided by the
+    Oxygen concentration in liquid bismuth squared* property abstract class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
         """
         Returns the temperature guess value according to the value
-        of the Oxygen partial pressure in liquid lbe divided by the
-        Oxygen concentration in liquid lbe squared passed as argument.
+        of the Oxygen partial pressure in liquid bismuth divided by the
+        Oxygen concentration in liquid bismuth squared passed as argument.
         It is used by the root finder algorithm.
 
         Parameters
         ----------
         property_value : float
-            oxygen partial pressure in liquid lbe divided by the
-            oxygen concentration in liquid lbe squared
-            in :math:`[atm. /wt.\\%^2]`
+            oxygen partial pressure in liquid bismuth divided by the
+            oxygen concentration in liquid bismuth squared
+            in :math:`[Pa /wt.\\%^2]`
 
         Returns
         -------
         float
             Temperature guess value in :math:`[K]`
         """
-        return 1600
+        if property_value < 10.1325:
+            return 1200
+        return 1500
 
+    @property
+    def description(self) -> str:
+        """
+        str : Oxygen partial pressure in liquid bismuth divided by the
+        Oxygen concentration in liquid bismuth squared description
+        """
+        return f"{self.long_name} in liquid bismuth"
+
+
+class OxygenPartialPressureFitzner1980(BismuthOxygenPartialPressureInterface):
+    """
+    *Oxygen partial pressure in liquid bismuth divided by the
+    Oxygen concentration in liquid bismuth squared* property class
+    implementing the correlation by *fitzner1980*.
+    """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Oxygen partial pressure in liquid lbe
-        divided by the Oxygen concentration in liquid lbe squared* by
+        Returns the value of the *Oxygen partial pressure in liquid bismuth
+        divided by the Oxygen concentration in liquid bismuth squared* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -60,71 +80,49 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
-        return np.power(10, 2 / 2.3 / R * (-127398 / T + 27.938))\
-            * M * M / M_O / M_O
+        return np.power(10, 2 / 2.3 / R * (-95502 / T + 9.69))\
+            * M * M / M_O / M_O * 101325
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "o_pp"
-
-    @property
-    def units(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Oxygen partial pressure in liquid lbe divided by the
-        Oxygen concentration in liquid lbe squared unit
+        str : Name of the correlation
         """
-        return "[atm.wt.%^-2]"
+        return "fitzner1980"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
-        return [812, 1008]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen partial pressure in liquid lbe divided by the
-        Oxygen concentration in liquid lbe squared long name
-        """
-        return ("Oxygen partial pressure divided by the"
-                " oxygen concentration squared")
-
-    @property
-    def description(self) -> str:
-        """
-        str : Oxygen partial pressure in liquid lbe divided by the
-        Oxygen concentration in liquid lbe squared description
-        """
-        return f"{self.long_name} in liquid lbe"
+        return [988, 1181]
 
 
-class LeadChemicalActivity(PropertyInterface):
+class OxygenPartialPressureIsecke1979(BismuthOxygenPartialPressureInterface):
     """
-    *Lead chemical activity* in liquid lbe property class.
+    *Oxygen partial pressure in liquid bismuth divided by the
+    Oxygen concentration in liquid bismuth squared* property class
+    implementing the correlation by *isecke1979*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *lead chemical activity* in liquid lbe
-        by applying the property correlation.
+        Returns the value of the *Oxygen partial pressure in liquid bismuth
+        divided by the Oxygen concentration in liquid bismuth squared* by
+        applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
             Pressure in :math:`[Pa]`, by default the atmospheric pressure
@@ -132,72 +130,50 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            Lead chemical activity in :math:`[-]`
-        """
-        return 0.42206 - 63.2 / T
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "pb_a"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Lead chemical activity unit
+            Oxygen partial pressure divided by Oxygen concentration
+            squared in :math:`[Pa / wt.\\%^2]`
         """
-        return "[-]"
+        return np.power(10, 2 / 2.3 / R * (-101098 / T + 15.66))\
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "gosse2014"
+        return "isecke1979"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the lead chemical
-        activity correlation function
-        """
-        return [399, 1173]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Lead chemical activity long name
-        """
-        return "lead chemical activity"
-
-    @property
-    def description(self) -> str:
-        """
-        str : Lead chemical activity description
+        List[float] : Temperature validity range of the Oxygen partial
+        pressure divided by the Oxygen concentration squared
+        correlation function
         """
-        return f"{self.long_name} in liquid lbe"
+        return [973, 1473]
 
 
-class BismuthChemicalActivity(PropertyInterface):
+class OxygenPartialPressureHahn1979(BismuthOxygenPartialPressureInterface):
     """
-    *Bismuth chemical activity* in liquid lbe property class.
+    *Oxygen partial pressure in liquid bismuth divided by the
+    Oxygen concentration in liquid bismuth squared* property class
+    implementing the correlation by *hahn1979*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *bismuth chemical activity* in liquid lbe
-        by applying the property correlation.
+        Returns the value of the *Oxygen partial pressure in liquid bismuth
+        divided by the Oxygen concentration in liquid bismuth squared* by
+        applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
             Pressure in :math:`[Pa]`, by default the atmospheric pressure
@@ -205,65 +181,91 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            Bismuth chemical activity in :math:`[-]`
+            Oxygen partial pressure divided by Oxygen concentration
+            squared in :math:`[Pa / wt.\\%^2]`
         """
-        return 0.53381 - 56.2 / T
+        return np.power(10, 2 / 2.3 / R * (-68156 / T + 14.14))\
+            * M * M / M_O / M_O * 101325
 
     @property
-    def name(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Name of the property
+        str : Name of the correlation
         """
-        return "bi_a"
+        return "hahn1979"
 
     @property
-    def units(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Bismuth chemical activity unit
+        List[float] : Temperature validity range of the Oxygen partial
+        pressure divided by the Oxygen concentration squared
+        correlation function
         """
-        return "[-]"
+        return [1073, 1223]
 
-    @property
-    def correlation_name(self) -> str:
-        """
-        str : Name of the correlation
-        """
-        return "gosse2014"
 
-    @property
-    def range(self) -> List[float]:
+class OxygenPartialPressureHeshmatpour1981(BismuthOxygenPartialPressureInterface):
+    """
+    *Oxygen partial pressure in liquid bismuth divided by the
+    Oxygen concentration in liquid bismuth squared* property class
+    implementing the correlation by *heshmatpour1981*.
+    """
+    @range_warning
+    def correlation(self, T: float, p: float = atm,
+                    verbose: bool = False) -> float:
         """
-        List[float] : Temperature validity range of the bismuth chemical
-        activity correlation function
+        Returns the value of the *Oxygen partial pressure in liquid bismuth
+        divided by the Oxygen concentration in liquid bismuth squared* by
+        applying the property correlation.
+
+        Parameters
+        ----------
+        T : float
+            Temperature in :math:`[K]`
+        p : float, optional
+            Pressure in :math:`[Pa]`, by default the atmospheric pressure
+            value, i.e., :math:`101325.0 Pa`
+        verbose : bool, optional
+            `True` to tell the decorator to print a warning message in case of
+            range check failing, `False` otherwise. By default, `False`
+
+        Returns
+        -------
+        float:
+            Oxygen partial pressure divided by Oxygen concentration
+            squared in :math:`[Pa / wt.\\%^2]`
         """
-        return [399, 1173]
+        return np.power(10, 2 / 2.3 / R * (-95437 / T + 3.78))\
+            * M * M / M_O / M_O * 101325
 
     @property
-    def long_name(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Bismuth chemical activity long name
+        str : Name of the correlation
         """
-        return "Bismuth chemical activity"
+        return "heshmatpour1981"
 
     @property
-    def description(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Bismuth chemical activity description
+        List[float] : Temperature validity range of the Oxygen partial
+        pressure divided by the Oxygen concentration squared
+        correlation function
         """
-        return f"{self.long_name} in liquid lbe"
+        return [1023, 1273]
 
 
-class MolarEnthalpy(PropertyInterface):
+class MolarEnthalpy(MolarEnthalpyInterface):
     """
-    Liquid lbe *molar enthalpy variation* property class.
+    Liquid bismuth *molar enthalpy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *molar enthalpy variation* by
         applying the property correlation.
@@ -283,53 +285,32 @@
         -------
         float:
             molar enthalpy in :math:`[J/mol]`
         """
         return h().correlation(T, p) * M / 1000
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "H"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Molar enthalpy variation unit
-        """
-        return "[J.mol^-1]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the molar enthalpy
         variation correlation function
         """
-        return [400.0, T_b0]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Molar enthalpy variation long name
-        """
-        return "molar enthalpy variation"
+        return [T_m0, T_b0]
 
     @property
     def description(self) -> str:
         """
         str : Molar enthalpy variation description
         """
-        return f"{self.long_name} in liquid lbe"
+        return f"{self.long_name} in liquid bismuth"
 
 
-class MolarEntropy(PropertyInterface):
+class MolarEntropy(MolarEntropyInterface):
     """
-    Liquid lbe *molar entropy variation* property class.
+    Liquid bismuth *molar entropy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *molar entropy variation* by
         applying the property correlation.
@@ -346,59 +327,37 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             molar entropy in :math:`[J/(mol \\cdot K)]`
         """
-        return M / 1000 * (164.8 * np.log(T / T_m0)
-                           - 3.94e-2 * (T - T_m0)
-                           + 6.25e-6 * (T * T - T_m0 * T_m0)
-                           + 2.28e5 * (1 / T / T - 1 / T_m0 / T_m0))
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "S"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Molar entropy variation unit
-        """
-        return "[J/(mol.K)]"
+        return M / 1000 * (118.2 * np.log(T / T_m0)
+                           + 5.934e-3 * (T - T_m0)
+                           - 7.183e6 / 2 * (1 / T / T - 1 / T_m0 / T_m0))
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the molar entropy
         variation correlation function
         """
-        return [400, T_b0]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Molar entropy variation long name
-        """
-        return "molar entropy variation"
+        return [T_m0, T_b0]
 
     @property
     def description(self) -> str:
         """
         str : Molar entropy variation description
         """
-        return f"{self.long_name} in liquid lbe"
+        return f"{self.long_name} in liquid bismuth"
 
 
-class GibbsFreeEnergy(PropertyInterface):
+class GibbsFreeEnergy(GibbsFreeEnergyInterface):
     """
-    Liquid lbe *Gibbs free energy variation* property class.
+    Liquid bismuth *Gibbs free energy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Gibbs free energy variation* by
         applying the property correlation.
@@ -419,41 +378,20 @@
         float:
             Gibbs free energy in :math:`[J/mol]`
         """
         return MolarEnthalpy().correlation(T, p)\
             - T * MolarEntropy().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "G"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Gibbs free energy unit
-        """
-        return "[J/mol]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Gibbs free energy
         variation correlation function
         """
-        return [400, T_b0]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Gibbs free energy long name
-        """
-        return "Gibbs free energy variation"
+        return [T_m0, T_b0]
 
     @property
     def description(self) -> str:
         """
         str : Gibbs free energy description
         """
-        return f"{self.long_name} in liquid lbe"
+        return f"{self.long_name} in liquid bismuth"
```

### Comparing `lbh15-2.0.0/lbh15/properties/lbe_thermochemical_properties/solubility_in_lbe.py` & `lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/solubility_in_lead.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,23 @@
 """Module with the definition of the *solubility*
-property objects for *lead-bismuth eutectic* (*lbe*)."""
+property objects for *lead*."""
 from typing import List
-from typing import Union
 import numpy as np
 from scipy.constants import atm
 from lbh15.properties.interface import PropertyInterface
+from ..tch_common_interface import IronSolubilityInterface
+from ..tch_common_interface import NickelSolubilityInterface
+from ..tch_common_interface import ChromiumSolubilityInterface
+from ..tch_common_interface import OxygenSolubilityInterface
 from ..._decorators import range_warning
 
 
-class IronSolubilityInterface(PropertyInterface):
+class IronSolubility(IronSolubilityInterface):
     """
-    Liquid lbe *Iron solubility* property abstract class.
-    """
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "fe_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Iron solubility unit
-        """
-        return "[wt.%]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Iron solubility long name
-        """
-        return "iron solubility"
-
-    @property
-    def description(self) -> str:
-        """
-        str : Iron solubility description
-        """
-        return f"{self.long_name} in liquid lbe"
-
-
-class IronSolubilityGosse2014(IronSolubilityInterface):
-    """
-    Liquid lbe *Iron solubility* property class
-    implementing the correlation by *gosse2014*.
+    Liquid lead *Iron solubility* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Iron solubility* by
         applying the property correlation.
@@ -65,42 +34,48 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2.00-4399/T)
+        return np.power(10, 2.11-5225/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Iron solubility
         correlation function
         """
-        return [399.0, 1173.0]
+        return [600.0, 1173.0]
+
+    @property
+    def description(self) -> str:
+        """
+        str : Iron solubility description
+        """
+        return f"{self.long_name} in liquid lead"
 
 
-class IronSolubilityWeeks1969(IronSolubilityInterface):
+class NickelSolubility(NickelSolubilityInterface):
     """
-    Liquid lbe *Iron solubility* property class
-    implementing the correlation by *weeks1969*.
+    Liquid lead *Nickel solubility* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Iron solubility* by
+        Returns the value of the *Nickel solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -111,75 +86,61 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 1.85-4164/T)
+        return np.power(10, 1.36-1395/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "weeks1969"
+        return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Iron solubility
+        List[float] : Temperature validity range of the Nickel solubility
         correlation function
         """
-        return [823.0, 1053.0]
-
-
-class NickelSolubilityInterface(PropertyInterface):
-    """
-    Liquid lbe *Nickel solubility* property abstract class.
-    """
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "ni_sol"
+        return [598.0, 917.0]
 
     @property
-    def units(self) -> str:
+    def description(self) -> str:
         """
-        str : Nickel solubility unit
+        str : Nickel solubility description
         """
-        return "[wt.%]"
+        return f"{self.long_name} in liquid lead"
 
-    @property
-    def long_name(self) -> str:
-        """
-        str : Nickel solubility long name
-        """
-        return "nickel solubility"
 
+class LeadChromiumSolubilityInterface(ChromiumSolubilityInterface):
+    """
+    Liquid lead *Chromium solubility* property abstract class.
+    """
     @property
     def description(self) -> str:
         """
-        str : Nickel solubility description
+        str : Chromium solubility description
         """
-        return f"{self.long_name} in liquid lbe"
+        return f"{self.long_name} in liquid lead"
 
 
-class NickelSolubilityMartinelli2010(NickelSolubilityInterface):
+class ChromiumSolubilityAlden1958(LeadChromiumSolubilityInterface):
     """
-    Liquid lbe *Nickel solubility* property class
-    implementing the correlation by *martinelli2010*.
+    Liquid lead *Chromium solubility* property class
+    implementing the correlation by *alden1958*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> Union[float, np.ndarray]:
+                    verbose: bool = False) -> float:
         """
-        Returns the value of the *Nickel solubility* by
+        Returns the value of the *Chromium solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -190,43 +151,42 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.where(T <= 712, np.power(10, 5.2-3500/T),
-                        np.power(10, 1.7-1009/T))[()]
+        return np.power(10, 3.74-6750/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "martinelli2010"
+        return "alden1958"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Nickel solubility
+        List[float] : Temperature validity range of the Chromium solubility
         correlation function
         """
-        return [603.0, 1173.0]
+        return [1181.0, 1483.0]
 
 
-class NickelSolubilityGosse2014(NickelSolubilityInterface):
+class ChromiumSolubilityVenkatraman1988(LeadChromiumSolubilityInterface):
     """
-    Liquid lbe *Nickel solubility* property class
-    implementing the correlation by *gosse2014*.
+    Liquid lead *Chromium solubility* property class
+    implementing the correlation by *venkatraman1988*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> Union[float, np.ndarray]:
+                    verbose: bool = False) -> float:
         """
-        Returns the value of the *Nickel solubility* by
+        Returns the value of the *Chromium solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -237,69 +197,35 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.where(T <= 742, np.power(10, 4.32-2933/T),
-                        np.power(10, 1.74-1006/T))[()]
+        return np.power(10, 3.7-6720/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "gosse2014"
+        return "venkatraman1988"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Nickel solubility
+        List[float] : Temperature validity range of the Chromium solubility
         correlation function
         """
-        return [528.0, 1173.0]
-
-
-class ChromiumSolubilityInterface(PropertyInterface):
-    """
-    Liquid lbe *Chromium solubility* property abstract class.
-    """
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "cr_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Chromium solubility unit
-        """
-        return "[wt.%]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Chromium solubility long name
-        """
-        return "cr solubility"
-
-    @property
-    def description(self) -> str:
-        """
-        str : Chromium solubility description
-        """
-        return f"{self.long_name} in liquid lbe"
+        return [1173.0, 1473.0]
 
 
-class ChromiumSolubilityGosse2014(ChromiumSolubilityInterface):
+class ChromiumSolubilityGosse2014(LeadChromiumSolubilityInterface):
     """
-    Liquid lbe *Chromium solubility* property class
+    Liquid lead *Chromium solubility* property class
     implementing the correlation by *gosse2014*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Chromium solubility* by
@@ -317,42 +243,41 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 1.12-3056/T)
+        return np.power(10, 3.62-6648/T)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Chromium solubility
         correlation function
         """
-        return [399.0, 1173.0]
+        return [601.0, 1773.0]
 
 
-class ChromiumSolubilityCourouau2004(ChromiumSolubilityInterface):
+class SiliconSolubility(PropertyInterface):
     """
-    Liquid lbe *Chromium solubility* property class
-    implementing the correlation by *courouau2004*.
+    Liquid lead *Silicon solubility* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Chromium solubility* by
+        Returns the value of the *Silicon solubility* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -363,81 +288,56 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 1.07-3022/T)
+        return np.power(10, 3.886-7180/T)
 
     @property
-    def correlation_name(self) -> str:
+    def name(self) -> str:
         """
-        str : Name of the correlation
+        str : Name of the property
         """
-        return "courouau2004"
+        return "si_sol"
 
     @property
-    def range(self) -> List[float]:
+    def units(self) -> str:
         """
-        List[float] : Temperature validity range of the Chromium solubility
-        correlation function
+        str : Silicon solubility unit
         """
-        return [643.0, 813.0]
-
+        return "[wt.%]"
 
-class ChromiumSolubilityMartynov1998(ChromiumSolubilityInterface):
-    """
-    Liquid lbe *Chromium solubility* property class
-    implementing the correlation by *martynov1998*.
-    """
-    @range_warning
-    def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> float:
+    @property
+    def range(self) -> List[float]:
         """
-        Returns the value of the *Chromium solubility* by
-        applying the property correlation.
-
-        Parameters
-        ----------
-        T : float
-            Temperature in :math:`[K]`
-        p : float, optional
-            Pressure in :math:`[Pa]`, by default the atmospheric pressure
-            value, i.e., :math:`101325.0 Pa`
-        verbose : bool, optional
-            `True` to tell the decorator to print a warning message in case of
-            range check failing, `False` otherwise. By default, `False`
-
-        Returns
-        -------
-        float:
-            solubility in :math:`[wt.\\%]`
+        List[float] : Temperature validity range of the Silicon solubility
+        correlation function
         """
-        return np.power(10, -0.02-2280/T)
+        return [1323.0, 1523.0]
 
     @property
-    def correlation_name(self) -> str:
+    def long_name(self) -> str:
         """
-        str : Name of the correlation
+        str : Silicon solubility long name
         """
-        return "martynov1998"
+        return "silicon solubility"
 
     @property
-    def range(self) -> List[float]:
+    def description(self) -> str:
         """
-        List[float] : Temperature validity range of the Chromium solubility
-        correlation function
+        str : Silicon solubility description
         """
-        return [673.0, 773.0]
+        return f"{self.long_name} in liquid lead"
 
 
-class OxygenSolubility(PropertyInterface):
+class OxygenSolubility(OxygenSolubilityInterface):
     """
-    Liquid lbe *Oxygen solubility* property class.
+    Liquid lead *Oxygen solubility* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *Oxygen solubility* by
         applying the property correlation.
@@ -454,44 +354,23 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             solubility in :math:`[wt.\\%]`
         """
-        return np.power(10, 2.25-4125/T)
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "o_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen solubility unit
-        """
-        return "[wt.%]"
+        return np.power(10, 3.23-5043/T)
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen solubility
         correlation function
         """
-        return [673.0, 1013.0]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen solubility long name
-        """
-        return "oxygen solubility"
+        return [673.0, 1373.0]
 
     @property
     def description(self) -> str:
         """
         str : Oxygen solubility description
         """
-        return "f{self.long_name} in liquid lbe"
+        return f"{self.long_name} in liquid lead"
```

### Comparing `lbh15-2.0.0/lbh15/properties/lead_properties.py` & `lbh15-2.1.0/lbh15/properties/lbe_properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 """Module with the definition of the thermo-physical property objects
-for *lead*."""
+for *lead-bismuth eutectic*."""
 from typing import List
 from typing import Union
 import numpy as np
 from scipy.constants import atm
-from .interface import PropertyInterface
+from .tph_common_interface import SaturationVapourPressureInterface
+from .tph_common_interface import SurfaceTensionInterface
+from .tph_common_interface import DensityInterface
+from .tph_common_interface import ThermalExpansionInterface
+from .tph_common_interface import SpeedOfSoundInterface
+from .tph_common_interface import IsentropicCompressibilityInterface
+from .tph_common_interface import SpecificHeatInterface
+from .tph_common_interface import SpecificEnthalpyInterface
+from .tph_common_interface import DynamicViscosityInterface
+from .tph_common_interface import ElectricalResistivityInterface
+from .tph_common_interface import ThermalConductivityInterface
 from .._decorators import range_warning
-from .._commons import LEAD_MELTING_TEMPERATURE as T_m0
-from .._commons import LEAD_BOILING_TEMPERATURE as T_b0
+from .._commons import LBE_MELTING_TEMPERATURE as T_m0
+from .._commons import LBE_BOILING_TEMPERATURE as T_b0
 
 
-class p_s(PropertyInterface):
+class p_s(SaturationVapourPressureInterface):
     """
-    Liquid lead *saturation vapour pressure* property class.
+    Liquid lead-bismuth eutectic *saturation vapour pressure* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *saturation vapour pressure* by
         applying the property correlation.
@@ -33,15 +43,15 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             saturation vapour pressure in :math:`[Pa]`
         """
-        return 5.76e9 * np.exp(-22131/T)
+        return 1.22e10 * np.exp(-22552/T)
 
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
         """
         Returns the temperature guess value according to the value
         of the saturation vapour pressure passed as argument.
         It is used by the root finder algorithm.
@@ -74,38 +84,24 @@
         """
         List[float] : Temperature validity range of the saturation vapour
         pressure correlation function
         """
         return [T_m0, T_b0]
 
     @property
-    def units(self) -> str:
-        """
-        str : Saturation vapour pressure unit
-        """
-        return "[Pa]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Saturation vapour pressure long name
-        """
-        return "saturation vapour pressure"
-
-    @property
     def description(self) -> str:
         """
         str : Saturation vapour pressure description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
-class sigma(PropertyInterface):
+class sigma(SurfaceTensionInterface):
     """
-    Liquid lead *surface tension* property class.
+    Liquid lead-bismuth eutectic *surface tension* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *surface tension* by
         applying the property correlation.
@@ -122,56 +118,42 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             surface tension in :math:`[N/m]`
         """
-        return (525.9 - 0.113*T)*1e-3
+        return (448.5 - 0.0799*T)*1e-3
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
-        return "jauch1986"
+        return "plevachuk2008"
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the surface
         tension correlation function
         """
-        return [T_m0, 1300.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Surface tension unit
-        """
-        return "[N/m]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Surface tension long name
-        """
-        return "surface tension"
+        return [T_m0, 1400.0]
 
     @property
     def description(self) -> str:
         """
         str : Surface tension description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
-class rho(PropertyInterface):
+class rho(DensityInterface):
     """
-    Liquid lead *density* property class.
+    Liquid lead-bismuth eutectic *density* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *density* by applying the property
         correlation. *sobolev2011* correlation is used for the specific
@@ -189,62 +171,41 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             density in :math:`[kg/m^3]`
         """
-        rho_0 = 11441 - 1.2795*T
+        rho_0 = 11065 - 1.293*T
         u_s_val = u_s().correlation(T, p)
         alpha_val = alpha().correlation(T, p)
         return rho_0 +\
-            (1.0 / u_s_val / u_s_val +
-             T * alpha_val * alpha_val /
-             cp_sobolev2011().correlation(T, p)) * (p - atm)
-
-    @property
-    def correlation_name(self) -> str:
-        """
-        str : Name of the correlation
-        """
-        return "sobolev2008a"
+            (1 / u_s_val / u_s_val +
+             T * alpha_val * alpha_val / cp().correlation(T, p)) * (p - atm)
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the density
         correlation function
         """
         return [T_m0, T_b0]
 
     @property
-    def units(self) -> str:
-        """
-        str : Density unit
-        """
-        return "[kg/m^3]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Density long name
-        """
-        return "density"
-
-    @property
     def description(self) -> str:
         """
         str : Density description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
-class alpha(PropertyInterface):
+class alpha(ThermalExpansionInterface):
     """
-    Liquid lead *thermal expansion coefficient* property class.
+    Liquid lead-bismuth eutectic *thermal expansion coefficient*
+    property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *thermal expansion coefficient* by
         applying the property correlation.
@@ -261,49 +222,35 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             thermal expansion coefficient in :math:`[1/K]`
         """
-        return 1/(8942 - T)
+        return 1/(8558 - T)
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the thermal expansion
         coefficient correlation function
         """
         return [T_m0, T_b0]
 
     @property
-    def units(self) -> str:
-        """
-        str : Thermal expansion coefficient unit
-        """
-        return "[1/K]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Thermal expansion coefficient long name
-        """
-        return "thermal expansion coefficient"
-
-    @property
     def description(self) -> str:
         """
         str : Thermal expansion coefficient description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
-class u_s(PropertyInterface):
+class u_s(SpeedOfSoundInterface):
     """
-    Liquid lead *sound velocity* property class.
+    Liquid lead-bismuth eutectic *sound velocity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *sound velocity* by
         applying the property correlation.
@@ -320,56 +267,42 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             sound velocity in :math:`[m/s]`
         """
-        return 1953 - 0.246*T
+        return 1855 - 0.212*T
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return 'sobolev2011'
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the sound velocity
         correlation function
         """
-        return [T_m0, 2000.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Sound velocity unit
-        """
-        return "[m/s]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Sound velocity long name
-        """
-        return "sound velocity"
+        return [400.0, 1100.0]
 
     @property
     def description(self) -> str:
         """
         str : Sound velocity description
         """
-        return "Sound velocity in liquid lead"
+        return "Sound velocity in liquid lbe"
 
 
-class beta_s(PropertyInterface):
+class beta_s(IsentropicCompressibilityInterface):
     """
-    Liquid lead *isentropic compressibility* property class.
+    Liquid lead-bismuth eutectic *isentropic compressibility* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *isentropic compressibility* by
         applying the property correlation.
@@ -395,42 +328,27 @@
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the isentropic
         compressibility correlation function
         """
-        return [T_m0, 2000.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Isentropic compressibility unit
-        """
-        return "[1/Pa]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Isentropic compressibility long name
-        """
-        return "isentropic compressibility"
+        return [400.0, 1100.0]
 
     @property
     def description(self) -> str:
         """
         str : Isentropic compressibility description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
-class cp_sobolev2011(PropertyInterface):
+class cp(SpecificHeatInterface):
     """
-    Liquid lead *specific heat capacity* property class exploiting
-    the **sobolev2011** correlation.
+    Liquid lead-bismuth eutectic *specific heat capacity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *specific heat capacity* by
         applying the **sobolev2011** correlation.
@@ -447,154 +365,42 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             specific heat capacity in :math:`[J/(kg \\cdot K)]`
         """
-        return 176.2 - T * (4.923e-2 - 1.544e-5 * T) - 1.524e6 / T / T
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "cp"
+        return 164.8 - T * (3.94e-2 - 1.25e-5 * T) - 4.56e5 / T / T
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return 'sobolev2011'
 
     @property
-    def is_injective(self) -> bool:
-        """
-        bool : `True` if the correlation is injective,
-        `False` otherwise.
-        """
-        return False
-
-    @property
-    def range(self) -> List[float]:
-        """
-        List[float] : Temperature validity range of the specific heat
-        capacity correlation function
-        """
-        return [T_m0, 2000.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Specific heat capacity unit
-        """
-        return "[J/(kg*K)]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Specific heat capacity long name
-        """
-        return "specific heat capacity"
-
-    @property
-    def description(self) -> str:
-        """
-        str : Specific heat capacity description
-        """
-        return f"Liquid lead {self.long_name}"
-
-
-class cp_gurvich1991(PropertyInterface):
-    """
-    Liquid lead *specific heat capacity* property class exploiting
-    the **gurvich1991** correlation.
-    """
-    @range_warning
-    def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> float:
-        """
-        Returns the value of the *specific heat capacity* by
-        applying the **gurvich1991** correlation.
-
-        Parameters
-        ----------
-        T : float
-            Temperature in :math:`[K]`
-        p : float, optional
-            Pressure in :math:`[Pa]`, by default the atmospheric pressure
-            value, i.e., :math:`101325.0 Pa`
-        verbose : bool, optional
-            `True` to tell the decorator to print a warning message in case of
-            range check failing, `False` otherwise. By default, `False`
-
-        Returns
-        -------
-        float:
-            specific heat capacity in :math:`[J/(kg \\cdot K)]`
-        """
-        return 175.1 - T * (4.961e-2 - T * (1.985e-5 - 2.099e-9 * T))\
-            - 1.524e6 / T / T
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "cp"
-
-    @property
-    def correlation_name(self) -> str:
-        """
-        str : Name of the correlation
-        """
-        return 'gurvich1991'
-
-    @property
-    def is_injective(self) -> bool:
-        """
-        bool : `True` if the correlation is injective,
-        `False` otherwise.
-        """
-        return False
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the specific heat
         capacity correlation function
         """
-        return [T_m0, 2000.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Specific heat capacity unit
-        """
-        return "[J/(kg*K)]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Specific heat capacity long name
-        """
-        return "specific heat capacity"
+        return [400.0, T_b0]
 
     @property
     def description(self) -> str:
         """
         str : Specific heat capacity description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
-class h(PropertyInterface):
+class h(SpecificEnthalpyInterface):
     """
-    Liquid lead *specific enthalpy* property class.
+    Liquid lead-bismuth eutectic *specific enthalpy* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *specific enthalpy* by
         applying the property correlation.
@@ -611,60 +417,46 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             specific enthalpy in :math:`[J/kg]`
         """
-        return T * (176.2 - T * (2.4615e-2 - 5.147e-6 * T))\
-            - T_m0 * (176.2 - T_m0 * (2.4615e-2 - 5.147e-6 * T_m0))\
-            + 1.524e6 * (1 / T - 1 / T_m0)
+        return T * (164.8 - T * (1.97e-2 - 4.167e-6 * T))\
+            - T_m0 * (164.8 - T_m0 * (1.97e-2 - 4.167e-6 * T_m0))\
+            + 4.56e5 * (1 / T - 1 / T_m0)
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return 'sobolev2011'
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the specific enthalpy
         correlation function
         """
-        return [T_m0, 2000.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Specific enthalpy unit
-        """
-        return "[J/kg]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Specific enthalpy long name
-        """
-        return "specific enthalpy"
+        return [400.0, T_b0]
 
     @property
     def description(self) -> str:
         """
-        str : Specific enthalpy description
+        str : str : Specific enthalpy description
         """
-        return (f"Liquid lead {self.long_name} "
+        return (f"Liquid lbe {self.long_name} "
                 "(as difference with respect to "
                 "the melting point enthalpy)")
 
 
-class mu(PropertyInterface):
+class mu(DynamicViscosityInterface):
     """
-    Liquid lead *dynamic viscosity* property class.
+    Liquid lead-bismuth eutectic *dynamic viscosity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *dynamic viscosity* by
         applying the property correlation.
@@ -681,70 +473,35 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             dynamic viscosity in :math:`[Pa \\cdot s]`
         """
-        return 4.55e-4 * np.exp(1069/T)
-
-    def initialization_helper(self,
-                              property_value: float) -> Union[None, float]:
-        """
-        Returns the temperature guess value according to the value
-        of the dynamic viscosity passed as argument.
-        It is used by the root finder algorithm.
-
-        Parameters
-        ----------
-        property_value : float
-            dynamic viscosity in :math:`[Pa]`
-
-        Returns
-        -------
-        float
-            Temperature guess value in :math:`[K]`
-        """
-        if property_value < 2e-3:
-            return 800
-        return 1600
+        return 4.94e-4*np.exp(754.1/T)
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the dynamic viscosity
         correlation function
         """
-        return [T_m0, 1473.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Dynamic viscosity unit
-        """
-        return "[Pa*s]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Dynamic viscosity long name
-        """
-        return "dynamic viscosity"
+        return [T_m0, 1300.0]
 
     @property
     def description(self) -> str:
         """
         str : Dynamic viscosity description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
-class r(PropertyInterface):
+class r(ElectricalResistivityInterface):
     """
-    Liquid lead *electrical resistivity* property class.
+    Liquid lead-bismuth eutectic *electrical resistivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *electrical resistivity* by
         applying the property correlation.
@@ -761,49 +518,35 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             electrical resistivity in :math:`[Ohm \\cdot m]`
         """
-        return (67.0 + 0.0471*T)*1e-8
+        return (90.9 + 0.048*T)*1e-8
 
     @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the electrical
         resistivity correlation function
         """
-        return [T_m0, 1273.0]
-
-    @property
-    def units(self) -> str:
-        """
-        str : Electrical resistivity unit
-        """
-        return "[Ohm*m]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Electrical resistivity long name
-        """
-        return "electrical resistivity"
+        return [400.0, 1100.0]
 
     @property
     def description(self) -> str:
         """
         str : Electrical resistivity description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
-class k(PropertyInterface):
+class k(ThermalConductivityInterface):
     """
-    Liquid lead *thermal conductivity* property class.
+    Liquid lead-bismuth eutectic *thermal conductivity* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
         Returns the value of the *thermal conductivity* by
         applying the property correlation.
@@ -820,37 +563,30 @@
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             thermal conductivity in :math:`[W/(m \\cdot K)]`
         """
-        return 9.2 + 0.011*T
+        return 3.284 + T * (1.617e-2 - 2.305e-6 * T)
 
     @property
-    def range(self) -> List[float]:
-        """
-        List[float] : Temperature validity range of the thermal
-        conductivity correlation function
-        """
-        return [T_m0, 1300.0]
-
-    @property
-    def units(self) -> str:
+    def correlation_name(self) -> str:
         """
-        str : Thermal conductivity unit
+        str : Name of the correlation
         """
-        return "[W/(m*K)]"
+        return 'sobolev2011'
 
     @property
-    def long_name(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Thermal conductivity long name
+        List[float] : Temperature validity range of the thermal
+        conductivity correlation function
         """
-        return "thermal conductivity"
+        return [T_m0, 1200.0]
 
     @property
     def description(self) -> str:
         """
         str : Thermal conductivity description
         """
-        return f"Liquid lead {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
```

### Comparing `lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/lead_oxygen_limits.py` & `lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/lead_oxygen_limits.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,53 @@
 objects for *lead*."""
 from typing import List
 from typing import Union
 import numpy as np
 from scipy.constants import atm
 from scipy.constants import R
 from ..interface import PropertyInterface
+from ..tch_common_interface import LowerLimitSaturationIronInterface
+from ..tch_common_interface import LowerLimitSaturationChromiumInterface
+from ..tch_common_interface import LowerLimitSaturationNickelInterface
+from ..tch_common_interface import LowerLimitSaturationSiliconInterface
+from ..tch_common_interface import LowerLimitSaturationAluminiumInterface
+from ..tch_common_interface import LowerLimitChromiumInterface
+from ..tch_common_interface import LowerLimitNickelInterface
+from ..tch_common_interface import LowerLimitIronInterface
 from .solubility_in_lead import OxygenSolubility
 from .solubility_in_lead import ChromiumSolubilityGosse2014
 from .solubility_in_lead import ChromiumSolubilityAlden1958
 from .solubility_in_lead import ChromiumSolubilityVenkatraman1988
 from .solubility_in_lead import NickelSolubility
 from .solubility_in_lead import IronSolubility
 from .solubility_in_lead import SiliconSolubility
 from ..._decorators import range_warning
 
 
-class LowerLimitSaturationIron(PropertyInterface):
+class LowerLimitSaturationIron(LowerLimitSaturationIronInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lead considering
     *Iron at its saturation concentration* property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
         """
         Returns the temperature guess value according to the value
         of the lower limit of Oxygen concentration to promote a protective
-        oxide film in liquid lead considering Chromium at its saturation
+        oxide film in liquid lead considering Iron at its saturation
         concentration passed as argument.
         It is used by the root finder algorithm.
 
         Parameters
         ----------
         property_value : float
             lower limit of Oxygen concentration to promote a
             protective oxide film in liquid lead considering
-            Chromium at its saturation concentration
+            Iron at its saturation concentration
             in :math:`[wt.\\%]`
 
         Returns
         -------
         float
             Temperature guess value in :math:`[K]`
         """
@@ -73,52 +81,30 @@
         float:
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-57190 / R / T - 21.1 / R)\
             * OxygenSolubility().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_fe_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                " iron at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lead"
 
 
-class LowerLimitSaturationChromium(PropertyInterface):
+class LowerLimitSaturationChromium(LowerLimitSaturationChromiumInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lead considering
     *Chromium at its saturation concentration* property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -171,52 +157,30 @@
         float:
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-158900 / R / T - 13.65 / R)\
             * OxygenSolubility().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_cr_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                " chromium at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lead"
 
 
-class LowerLimitSaturationNickel(PropertyInterface):
+class LowerLimitSaturationNickel(LowerLimitSaturationNickelInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lead considering
     *Nickel at its saturation concentration* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -243,52 +207,30 @@
         float:
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-18040 / R / T - 11.7 / R)\
             * OxygenSolubility().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_ni_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                " nickel at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lead"
 
 
-class LowerLimitSaturationSilicon(PropertyInterface):
+class LowerLimitSaturationSilicon(LowerLimitSaturationSiliconInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lead considering
     *Silicon at its saturation concentration* property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -341,52 +283,30 @@
         float:
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-235855 / R / T - 9.75 / R)\
             * OxygenSolubility().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_si_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                " silicon at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lead"
 
 
-class LowerLimitSaturationAluminium(PropertyInterface):
+class LowerLimitSaturationAluminium(LowerLimitSaturationAluminiumInterface):
     """
     *Lower limit of Oxygen concentration* to promote a
     protective oxide film in liquid lead considering
     *Aluminium at its saturation concentration* property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -437,52 +357,30 @@
         float:
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return np.exp(-339770 / R / T + 5.35 / R)\
             * OxygenSolubility().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_al_sat"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit for"
-                " aluminium at its saturation concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in liquid lead"
 
 
-class LowerLimitChromiumInterface(PropertyInterface):
+class LeadLowerLimitChromiumInterface(LowerLimitChromiumInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Chromium concentration*
     raised to :math:`2/3` in liquid lead property abstract class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -507,44 +405,22 @@
             Temperature guess value in :math:`[K]`
         """
         if property_value < 1e-6:
             return 1500
         return 1800
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_cr"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit times"
-                " chromium concentration raised to 2/3")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in lead"
 
 
-class LowerLimitChromiumGosse2014(LowerLimitChromiumInterface):
+class LowerLimitChromiumGosse2014(LeadLowerLimitChromiumInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Chromium concentration*
     raised to :math:`2/3` in liquid lead property class
     implementing the correlation by *gosse2014*.
     """
     @range_warning
@@ -587,15 +463,15 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
 
-class LowerLimitChromiumVenkatraman1988(LowerLimitChromiumInterface):
+class LowerLimitChromiumVenkatraman1988(LeadLowerLimitChromiumInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Chromium concentration*
     raised to :math:`2/3` in liquid lead property class
     implementing the correlation by *venkatraman1988*.
     """
     @range_warning
@@ -639,15 +515,15 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
 
-class LowerLimitChromiumAlden1958(LowerLimitChromiumInterface):
+class LowerLimitChromiumAlden1958(LeadLowerLimitChromiumInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Chromium concentration*
     raised to :math:`2/3` in liquid lead property class
     implementing the correlation by *alden1958*.
     """
     @range_warning
@@ -690,15 +566,15 @@
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
 
-class LowerLimitNickel(PropertyInterface):
+class LowerLimitNickel(LowerLimitNickelInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Nickel concentration*
     in liquid lead property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -725,52 +601,30 @@
         float:
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return LowerLimitSaturationNickel().correlation(T, p)\
             * NickelSolubility().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_ni"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 917]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit times"
-                " nickel concentration")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in lead"
 
 
-class LowerLimitIron(PropertyInterface):
+class LowerLimitIron(LowerLimitIronInterface):
     """
     *Lower limit of oxygen concentration* to promote a
     protective oxide film times the *Iron concentration*
     raised to :math:`3/4` in liquid lead property class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
@@ -823,44 +677,22 @@
         float:
             Oxygen concentration in :math:`[wt.\\%]`
         """
         return LowerLimitSaturationIron().correlation(T, p)\
             * np.power(IronSolubility().correlation(T, p), 0.75)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "lim_fe"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen concentration lower limit unit
-        """
-        return "[wt.%]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Oxygen concentration
         lower limit correlation function
         """
         return [673, 1000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen concentration lower limit long name
-        """
-        return ("Oxygen concentration lower limit times"
-                " iron concentration raised to 3/4")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen concentration lower limit description
         """
         return f"{self.long_name} in lead"
```

### Comparing `lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/lead_thermochemical.py` & `lbh15-2.1.0/lbh15/properties/lead_thermochemical_properties/lead_thermochemical.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Module with the definition of the *thermo-chemical*
 property objects for *lead*."""
 from typing import List
 from typing import Union
 import numpy as np
 from scipy.constants import atm
 from scipy.constants import R
-from lbh15.properties.interface import PropertyInterface
+from ..tch_common_interface import OxygenPartialPressureInterface
+from ..tch_common_interface import MolarEnthalpyInterface
+from ..tch_common_interface import MolarEntropyInterface
+from ..tch_common_interface import GibbsFreeEnergyInterface
 from ..lead_properties import h
 from ..._commons import LEAD_MELTING_TEMPERATURE as T_m0
 from ..._commons import LEAD_MOLAR_MASS as M
 from ..._commons import OXYGEN_MOLAR_MASS as M_O
 from ..._decorators import range_warning
 
 
-class OxygenPartialPressureInterface(PropertyInterface):
+class LeadOxygenPartialPressureInterface(OxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property abstract class.
     """
     def initialization_helper(self,
                               property_value: float) -> Union[None, float]:
         """
@@ -27,57 +30,33 @@
         It is used by the root finder algorithm.
 
         Parameters
         ----------
         property_value : float
             oxygen partial pressure in liquid lead divided by the
             oxygen concentration in liquid lead squared
-            in :math:`[atm. /wt.\\%^2]`
+            in :math:`[Pa /wt.\\%^2]`
 
         Returns
         -------
         float
             Temperature guess value in :math:`[K]`
         """
         return 1600
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "o_pp"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen partial pressure in liquid lead divided by the
-        Oxygen concentration in liquid lead squared unit
-        """
-        return "[atm.wt.%^-2]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen partial pressure in liquid lead divided by the
-        Oxygen concentration in liquid lead squared long name
-        """
-        return ("Oxygen partial pressure divided by the"
-                " oxygen concentration squared")
-
-    @property
     def description(self) -> str:
         """
         str : Oxygen partial pressure in liquid lead divided by the
         Oxygen concentration in liquid lead squared description
         """
         return f"{self.long_name} in liquid lead"
 
 
-class OxygenPartialPressureOtsuka1979(OxygenPartialPressureInterface):
+class OxygenPartialPressureOtsuka1979(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *otsuka1979*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -98,18 +77,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-118600 / T + 14.1))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "otsuka1979"
@@ -120,15 +99,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [1073, 1673]
 
 
-class OxygenPartialPressureOtsuka1981(OxygenPartialPressureInterface):
+class OxygenPartialPressureOtsuka1981(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *otsuka1981*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -149,18 +128,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-117170 / T + 12.9))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "otsuka1981"
@@ -171,15 +150,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [1023, 1273]
 
 
-class OxygenPartialPressureGanesan2006(OxygenPartialPressureInterface):
+class OxygenPartialPressureGanesan2006(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *ganesan2006*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -200,18 +179,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-121349 / T + 16.906))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "ganesan2006"
@@ -222,15 +201,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [815, 1090]
 
 
-class OxygenPartialPressureAlcock1964(OxygenPartialPressureInterface):
+class OxygenPartialPressureAlcock1964(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *alcock1964*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -251,18 +230,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-119411 / T + 12.222))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "alcock1964"
@@ -273,15 +252,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [783, 973]
 
 
-class OxygenPartialPressureSzwarc1972(OxygenPartialPressureInterface):
+class OxygenPartialPressureSzwarc1972(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *szwarc1972*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -302,18 +281,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-105855 / T + 18.661))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "szwarc1972"
@@ -324,15 +303,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [1012, 1353]
 
 
-class OxygenPartialPressureCharle1976(OxygenPartialPressureInterface):
+class OxygenPartialPressureCharle1976(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *charle1976*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -353,18 +332,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-119840 / T + 15.794))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "charle1976"
@@ -375,15 +354,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [1173, 1373]
 
 
-class OxygenPartialPressureIsecke1977(OxygenPartialPressureInterface):
+class OxygenPartialPressureIsecke1977(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *isecke1977*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -404,18 +383,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-120376 / T + 16.255))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "isecke1977"
@@ -426,15 +405,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [1173, 1373]
 
 
-class OxygenPartialPressureTaskinen1979(OxygenPartialPressureInterface):
+class OxygenPartialPressureTaskinen1979(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *taskinen1979*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -455,18 +434,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-116717 / T + 12.699))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "taskinen1979"
@@ -477,15 +456,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [1073, 1203]
 
 
-class OxygenPartialPressureFisher1966(OxygenPartialPressureInterface):
+class OxygenPartialPressureFisher1966(LeadOxygenPartialPressureInterface):
     """
     *Oxygen partial pressure in liquid lead divided by the
     Oxygen concentration in liquid lead squared* property class
     implementing the correlation by *fisher1966*.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
@@ -506,18 +485,18 @@
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
             Oxygen partial pressure divided by Oxygen concentration
-            squared in :math:`[atm. / wt.\\%^2]`
+            squared in :math:`[Pa / wt.\\%^2]`
         """
         return np.power(10, 2 / 2.3 / R * (-106395 / T + 10.254))\
-            * M * M / M_O / M_O
+            * M * M / M_O / M_O * 101325
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "fisher1966"
@@ -528,15 +507,15 @@
         List[float] : Temperature validity range of the Oxygen partial
         pressure divided by the Oxygen concentration squared
         correlation function
         """
         return [903, 1253]
 
 
-class MolarEnthalpy(PropertyInterface):
+class MolarEnthalpy(MolarEnthalpyInterface):
     """
     Liquid lead *molar enthalpy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
@@ -558,51 +537,30 @@
         -------
         float:
             molar enthalpy in :math:`[J/mol]`
         """
         return h().correlation(T, p) * M / 1000
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "H"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Molar enthalpy variation unit
-        """
-        return "[J.mol^-1]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the molar enthalpy
         variation correlation function
         """
         return [T_m0, 2000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Molar enthalpy variation long name
-        """
-        return "molar enthalpy variation"
-
-    @property
     def description(self) -> str:
         """
         str : Molar enthalpy variation description
         """
         return f"{self.long_name} in liquid lead"
 
 
-class MolarEntropy(PropertyInterface):
+class MolarEntropy(MolarEntropyInterface):
     """
     Liquid lead *molar entropy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
@@ -628,51 +586,30 @@
         """
         return M / 1000 * (176.2 * np.log(T / T_m0)
                            - 4.923e-2 * (T - T_m0)
                            + 7.72e-6 * (T * T - T_m0 * T_m0)
                            + 7.62e5 * (1 / T / T - 1 / T_m0 / T_m0))
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "S"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Molar entropy variation unit
-        """
-        return "[J/(mol.K)]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the molar entropy
         variation correlation function
         """
         return [T_m0, 2000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Molar entropy variation long name
-        """
-        return "molar entropy variation"
-
-    @property
     def description(self) -> str:
         """
         str : Molar entropy variation description
         """
         return f"{self.long_name} in liquid lead"
 
 
-class GibbsFreeEnergy(PropertyInterface):
+class GibbsFreeEnergy(GibbsFreeEnergyInterface):
     """
     Liquid lead *Gibbs free energy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
@@ -696,41 +633,20 @@
         float:
             Gibbs free energy in :math:`[J/mol]`
         """
         return MolarEnthalpy().correlation(T, p)\
             - T * MolarEntropy().correlation(T, p)
 
     @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "G"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Gibbs free energy unit
-        """
-        return "[J/mol]"
-
-    @property
     def range(self) -> List[float]:
         """
         List[float] : Temperature validity range of the Gibbs free energy
         variation correlation function
         """
         return [T_m0, 2000]
 
     @property
-    def long_name(self) -> str:
-        """
-        str : Gibbs free energy long name
-        """
-        return "Gibbs free energy variation"
-
-    @property
     def description(self) -> str:
         """
         str : Gibbs free energy description
         """
         return f"{self.long_name} in liquid lead"
```

### Comparing `lbh15-2.0.0/lbh15/properties/lead_thermochemical_properties/solubility_in_lead.py` & `lbh15-2.1.0/lbh15/properties/lbe_thermochemical_properties/lbe_thermochemical.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,60 @@
-"""Module with the definition of the *solubility*
-property objects for *lead*."""
+"""Module with the definition of the *thermo-chemical*
+property objects for *lead-bismuth eutectic* (*lbe*)."""
 from typing import List
+from typing import Union
 import numpy as np
 from scipy.constants import atm
-from lbh15.properties.interface import PropertyInterface
+from scipy.constants import R
+from ..interface import PropertyInterface
+from ..tch_common_interface import OxygenPartialPressureInterface
+from ..tch_common_interface import MolarEnthalpyInterface
+from ..tch_common_interface import MolarEntropyInterface
+from ..tch_common_interface import GibbsFreeEnergyInterface
+from ..lbe_properties import h
+from ..._commons import LBE_BOILING_TEMPERATURE as T_b0
+from ..._commons import LBE_MELTING_TEMPERATURE as T_m0
+from ..._commons import LBE_MOLAR_MASS as M
+from ..._commons import OXYGEN_MOLAR_MASS as M_O
 from ..._decorators import range_warning
 
 
-class IronSolubility(PropertyInterface):
+class OxygenPartialPressure(OxygenPartialPressureInterface):
     """
-    Liquid lead *Iron solubility* property class.
+    *Oxygen partial pressure in liquid lbe divided by the
+    Oxygen concentration in liquid lbe squared* property class.
     """
+    def initialization_helper(self,
+                              property_value: float) -> Union[None, float]:
+        """
+        Returns the temperature guess value according to the value
+        of the Oxygen partial pressure in liquid lbe divided by the
+        Oxygen concentration in liquid lbe squared passed as argument.
+        It is used by the root finder algorithm.
+
+        Parameters
+        ----------
+        property_value : float
+            oxygen partial pressure in liquid lbe divided by the
+            oxygen concentration in liquid lbe squared
+            in :math:`[Pa /wt.\\%^2]`
+
+        Returns
+        -------
+        float
+            Temperature guess value in :math:`[K]`
+        """
+        return 1600
+
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Iron solubility* by
+        Returns the value of the *Oxygen partial pressure in liquid lbe
+        divided by the Oxygen concentration in liquid lbe squared* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -28,72 +63,48 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            solubility in :math:`[wt.\\%]`
-        """
-        return np.power(10, 2.11-5225/T)
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "fe_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Iron solubility unit
+            Oxygen partial pressure divided by Oxygen concentration
+            squared in :math:`[Pa / wt.\\%^2]`
         """
-        return "[wt.%]"
-
-    @property
-    def correlation_name(self) -> str:
-        """
-        str : Name of the correlation
-        """
-        return "gosse2014"
+        return np.power(10, 2 / 2.3 / R * (-127398 / T + 27.938))\
+            * M * M / M_O / M_O * 101325
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Iron solubility
+        List[float] : Temperature validity range of the Oxygen partial
+        pressure divided by the Oxygen concentration squared
         correlation function
         """
-        return [600.0, 1173.0]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Iron solubility long name
-        """
-        return "iron solubility"
+        return [812, 1008]
 
     @property
     def description(self) -> str:
         """
-        str : Iron solubility description
+        str : Oxygen partial pressure in liquid lbe divided by the
+        Oxygen concentration in liquid lbe squared description
         """
-        return "f{self.long_name} in liquid lead"
+        return f"{self.long_name} in liquid lbe"
 
 
-class NickelSolubility(PropertyInterface):
+class LeadChemicalActivity(PropertyInterface):
     """
-    Liquid lead *Nickel solubility* property class.
+    *Lead chemical activity* in liquid lbe property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Nickel solubility* by
-        applying the property correlation.
+        Returns the value of the *lead chemical activity* in liquid lbe
+        by applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
             Pressure in :math:`[Pa]`, by default the atmospheric pressure
@@ -101,106 +112,72 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            solubility in :math:`[wt.\\%]`
+            Lead chemical activity in :math:`[-]`
         """
-        return np.power(10, 1.36-1395/T)
+        return 0.42206 - 63.2 / T
 
     @property
     def name(self) -> str:
         """
         str : Name of the property
         """
-        return "ni_sol"
+        return "pb_a"
 
     @property
     def units(self) -> str:
         """
-        str : Nickel solubility unit
+        str : Lead chemical activity unit
         """
-        return "[wt.%]"
+        return "[-]"
 
     @property
     def correlation_name(self) -> str:
         """
         str : Name of the correlation
         """
         return "gosse2014"
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Nickel solubility
-        correlation function
+        List[float] : Temperature validity range of the lead chemical
+        activity correlation function
         """
-        return [598.0, 917.0]
+        return [399, 1173]
 
     @property
     def long_name(self) -> str:
         """
-        str : Nickel solubility long name
+        str : Lead chemical activity long name
         """
-        return "nickel solubility"
+        return "lead chemical activity"
 
     @property
     def description(self) -> str:
         """
-        str : Nickel solubility description
+        str : Lead chemical activity description
         """
-        return "f{self.long_name} in liquid lead"
+        return f"{self.long_name} in liquid lbe"
 
 
-class ChromiumSolubilityInterface(PropertyInterface):
+class BismuthChemicalActivity(PropertyInterface):
     """
-    Liquid lead *Chromium solubility* property abstract class.
-    """
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "cr_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Chromium solubility unit
-        """
-        return "[wt.%]"
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Chromium solubility long name
-        """
-        return "chromium solubility"
-
-    @property
-    def description(self) -> str:
-        """
-        str : Chromium solubility description
-        """
-        return f"{self.long_name} in liquid lead"
-
-
-class ChromiumSolubilityAlden1958(ChromiumSolubilityInterface):
-    """
-    Liquid lead *Chromium solubility* property class
-    implementing the correlation by *alden1958*.
+    *Bismuth chemical activity* in liquid lbe property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Chromium solubility* by
-        applying the property correlation.
+        Returns the value of the *bismuth chemical activity* in liquid lbe
+        by applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
             Pressure in :math:`[Pa]`, by default the atmospheric pressure
@@ -208,90 +185,71 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            solubility in :math:`[wt.\\%]`
+            Bismuth chemical activity in :math:`[-]`
         """
-        return np.power(10, 3.74-6750/T)
+        return 0.53381 - 56.2 / T
 
     @property
-    def correlation_name(self) -> str:
+    def name(self) -> str:
         """
-        str : Name of the correlation
+        str : Name of the property
         """
-        return "alden1958"
+        return "bi_a"
 
     @property
-    def range(self) -> List[float]:
+    def units(self) -> str:
         """
-        List[float] : Temperature validity range of the Chromium solubility
-        correlation function
+        str : Bismuth chemical activity unit
         """
-        return [1181.0, 1483.0]
-
+        return "[-]"
 
-class ChromiumSolubilityVenkatraman1988(ChromiumSolubilityInterface):
-    """
-    Liquid lead *Chromium solubility* property class
-    implementing the correlation by *venkatraman1988*.
-    """
-    @range_warning
-    def correlation(self, T: float, p: float = atm,
-                    verbose: bool = False) -> float:
+    @property
+    def correlation_name(self) -> str:
         """
-        Returns the value of the *Chromium solubility* by
-        applying the property correlation.
-
-        Parameters
-        ----------
-        T : float
-            Temperature in :math:`[K]`
-        p : float, optional
-            Pressure in :math:`[Pa]`, by default the atmospheric pressure
-            value, i.e., :math:`101325.0 Pa`
-        verbose : bool, optional
-            `True` to tell the decorator to print a warning message in case of
-            range check failing, `False` otherwise. By default, `False`
+        str : Name of the correlation
+        """
+        return "gosse2014"
 
-        Returns
-        -------
-        float:
-            solubility in :math:`[wt.\\%]`
+    @property
+    def range(self) -> List[float]:
         """
-        return np.power(10, 3.7-6720/T)
+        List[float] : Temperature validity range of the bismuth chemical
+        activity correlation function
+        """
+        return [399, 1173]
 
     @property
-    def correlation_name(self) -> str:
+    def long_name(self) -> str:
         """
-        str : Name of the correlation
+        str : Bismuth chemical activity long name
         """
-        return "venkatraman1988"
+        return "Bismuth chemical activity"
 
     @property
-    def range(self) -> List[float]:
+    def description(self) -> str:
         """
-        List[float] : Temperature validity range of the Chromium solubility
-        correlation function
+        str : Bismuth chemical activity description
         """
-        return [1173.0, 1473.0]
+        return f"{self.long_name} in liquid lbe"
 
 
-class ChromiumSolubilityGosse2014(ChromiumSolubilityInterface):
+class MolarEnthalpy(MolarEnthalpyInterface):
     """
-    Liquid lead *Chromium solubility* property class
-    implementing the correlation by *gosse2014*.
+    Liquid lbe *molar enthalpy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Chromium solubility* by
+        Returns the value of the *molar enthalpy variation* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -300,43 +258,43 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            solubility in :math:`[wt.\\%]`
+            molar enthalpy in :math:`[J/mol]`
         """
-        return np.power(10, 3.62-6648/T)
+        return h().correlation(T, p) * M / 1000
 
     @property
-    def correlation_name(self) -> str:
+    def range(self) -> List[float]:
         """
-        str : Name of the correlation
+        List[float] : Temperature validity range of the molar enthalpy
+        variation correlation function
         """
-        return "gosse2014"
+        return [400.0, T_b0]
 
     @property
-    def range(self) -> List[float]:
+    def description(self) -> str:
         """
-        List[float] : Temperature validity range of the Chromium solubility
-        correlation function
+        str : Molar enthalpy variation description
         """
-        return [601.0, 1773.0]
+        return f"{self.long_name} in liquid lbe"
 
 
-class SiliconSolubility(PropertyInterface):
+class MolarEntropy(MolarEntropyInterface):
     """
-    Liquid lead *Silicon solubility* property class.
+    Liquid lbe *molar entropy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Silicon solubility* by
+        Returns the value of the *molar entropy variation* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -345,64 +303,46 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            solubility in :math:`[wt.\\%]`
-        """
-        return np.power(10, 3.886-7180/T)
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "si_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Silicon solubility unit
+            molar entropy in :math:`[J/(mol \\cdot K)]`
         """
-        return "[wt.%]"
+        return M / 1000 * (164.8 * np.log(T / T_m0)
+                           - 3.94e-2 * (T - T_m0)
+                           + 6.25e-6 * (T * T - T_m0 * T_m0)
+                           + 2.28e5 * (1 / T / T - 1 / T_m0 / T_m0))
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Silicon solubility
-        correlation function
-        """
-        return [1323.0, 1523.0]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Silicon solubility long name
+        List[float] : Temperature validity range of the molar entropy
+        variation correlation function
         """
-        return "silicon solubility"
+        return [400, T_b0]
 
     @property
     def description(self) -> str:
         """
-        str : Silicon solubility description
+        str : Molar entropy variation description
         """
-        return "f{self.long_name} in liquid lead"
+        return f"{self.long_name} in liquid lbe"
 
 
-class OxygenSolubility(PropertyInterface):
+class GibbsFreeEnergy(GibbsFreeEnergyInterface):
     """
-    Liquid lead *Oxygen solubility* property class.
+    Liquid lbe *Gibbs free energy variation* property class.
     """
     @range_warning
     def correlation(self, T: float, p: float = atm,
                     verbose: bool = False) -> float:
         """
-        Returns the value of the *Oxygen solubility* by
+        Returns the value of the *Gibbs free energy variation* by
         applying the property correlation.
 
         Parameters
         ----------
         T : float
             Temperature in :math:`[K]`
         p : float, optional
@@ -411,46 +351,26 @@
         verbose : bool, optional
             `True` to tell the decorator to print a warning message in case of
             range check failing, `False` otherwise. By default, `False`
 
         Returns
         -------
         float:
-            solubility in :math:`[wt.\\%]`
+            Gibbs free energy in :math:`[J/mol]`
         """
-        return np.power(10, 3.23-5043/T)
-
-    @property
-    def name(self) -> str:
-        """
-        str : Name of the property
-        """
-        return "o_sol"
-
-    @property
-    def units(self) -> str:
-        """
-        str : Oxygen solubility unit
-        """
-        return "[wt.%]"
+        return MolarEnthalpy().correlation(T, p)\
+            - T * MolarEntropy().correlation(T, p)
 
     @property
     def range(self) -> List[float]:
         """
-        List[float] : Temperature validity range of the Oxygen solubility
-        correlation function
-        """
-        return [673.0, 1373.0]
-
-    @property
-    def long_name(self) -> str:
-        """
-        str : Oxygen solubility long name
+        List[float] : Temperature validity range of the Gibbs free energy
+        variation correlation function
         """
-        return "oxygen solubility"
+        return [400, T_b0]
 
     @property
     def description(self) -> str:
         """
-        str : Oxygen solubility description
+        str : Gibbs free energy description
         """
-        return "f{self.long_name} in liquid lead"
+        return f"{self.long_name} in liquid lbe"
```

### Comparing `lbh15-2.0.0/lbh15.egg-info/PKG-INFO` & `lbh15-2.1.0/lbh15.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbh15
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python implementation of liquid metal properties from Handbook on Lead-bismuth Eutectic Alloy and Lead Properties, Materials Compatibility, Thermal-hydraulics and Technologies
 Author: Daniele Panico, Daniele Tomatis, Gabriele Ottino
 Author-email: Daniele Panico <daniele.panico@newcleo.com>, Daniele Tomatis <daniele.tomatis@newcleo.com>
 License: lgpl v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -14,31 +14,41 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: scipy>=1.8.1
+Requires-Dist: numpy>=1.22.3
+Requires-Dist: sphinx>=6.2.1
+Requires-Dist: sphinx-rtd-theme>=1.3.0
+Requires-Dist: myst-parser>=1.0.0
+Requires-Dist: sphinxcontrib-bibtex>=2.5.0
 
 lbh15
 =====
 
 :Author: Daniele Panico, Daniele Tomatis
 :Contributor: Gabriele Ottino, Lucie Kerleau, Chloé Largeron
-:Date: 08/01/2024
+:Date: 04/04/2024
 
 Introduction
 ------------
 
 *lbh15* (**L**\ ead **B**\ ismuth **H**\ andbook 20\ **15**) is a Python package that implements the
 thermo-physical and the thermo-chemical properties of lead, bismuth and lead-bismuth eutectic (lbe) metal alloy available from
 the handbook edited by 
-`OECD/NEA <https://www.oecd-nea.org/jcms/pl_14972/handbook-on-lead-bismuth-eutectic-alloy-and-lead-properties-materials-compatibility-thermal-hydraulics-and-technologies-2015-edition?details=true>`_
+`OECD/NEA <https://www.oecd-nea.org/jcms/pl_14972/handbook-on-lead-bismuth-eutectic-alloy-and-lead-properties-materials-compatibility-thermal-hydraulics-and-technologies-2015-edition?details=true>`_.
 
-*lbh15* is released under the **GNU Lesser General Public License 3**.
+*lbh15* offers a standard implementation for use of these properties in scientific applications.
+In particular, this package is used for numerical simulation and experimental activities supporting the
+development of nuclear reactors that employ heavy liquid metals as primary coolant.
+
+*lbh15* is developed by the **Codes & Methods** group of `newcleo <https://www.newcleo.com/>`_ and it is released under the **GNU Lesser General Public License 3**.
 
 *lbh15* is listed among the Open-source Nuclear Codes for Reactor Analysis (`ONCORE <https://nucleus.iaea.org/sites/oncore/SitePages/List%20of%20Codes.aspx>`_) by IAEA.
 
 Project Structure
 -----------------
 
 The project is organized according to the following folder structure:
@@ -116,14 +126,21 @@
       make latexpdf
 
 The *html* documentation is available on GitHub Pages at `newcleo-dev-team.github.io/lbh15 <https://newcleo-dev-team.github.io/lbh15/index.html>`_.
 
 To see the available templates for generating the documentation in *PDF* format and to choose among them, please
 look at the ``docs/conf.py`` file.
 
+How to Contribute
+-----------------
+
+For anyone wishing to contribute to the development of the project, report issues
+or problems with the software, or request support, please refer to this
+`web page <https://github.com/newcleo-dev-team/lbh15/blob/master/CONTRIBUTIONS.rst>`_.
+
 How to Cite
 -----------
 
 .. code-block:: latex
 
   @inproceedings{NURETH20lbh15,
     author = {Panico, Daniele and Tomatis, Daniele},
```

### Comparing `lbh15-2.0.0/lbh15.egg-info/SOURCES.txt` & `lbh15-2.1.0/lbh15.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -16,21 +16,29 @@
 lbh15.egg-info/requires.txt
 lbh15.egg-info/top_level.txt
 lbh15/properties/__init__.py
 lbh15/properties/bismuth_properties.py
 lbh15/properties/interface.py
 lbh15/properties/lbe_properties.py
 lbh15/properties/lead_properties.py
+lbh15/properties/tch_common_interface.py
+lbh15/properties/tph_common_interface.py
 lbh15/properties/bismuth_thermochemical_properties/__init__.py
 lbh15/properties/bismuth_thermochemical_properties/bismuth_thermochemical.py
 lbh15/properties/bismuth_thermochemical_properties/diffusivity_in_bismuth.py
 lbh15/properties/bismuth_thermochemical_properties/solubility_in_bismuth.py
 lbh15/properties/lbe_thermochemical_properties/__init__.py
 lbh15/properties/lbe_thermochemical_properties/diffusivity_in_lbe.py
 lbh15/properties/lbe_thermochemical_properties/lbe_oxygen_limits.py
 lbh15/properties/lbe_thermochemical_properties/lbe_thermochemical.py
 lbh15/properties/lbe_thermochemical_properties/solubility_in_lbe.py
 lbh15/properties/lead_thermochemical_properties/__init__.py
 lbh15/properties/lead_thermochemical_properties/diffusivity_in_lead.py
 lbh15/properties/lead_thermochemical_properties/lead_oxygen_limits.py
 lbh15/properties/lead_thermochemical_properties/lead_thermochemical.py
-lbh15/properties/lead_thermochemical_properties/solubility_in_lead.py
+lbh15/properties/lead_thermochemical_properties/solubility_in_lead.py
+tests/test_bismuth_fromX_spanT.py
+tests/test_custom_properties.py
+tests/test_lbe_fromX_spanT.py
+tests/test_lbh15_bounds.py
+tests/test_lead_basics.py
+tests/test_lead_fromX_spanT.py
```

### Comparing `lbh15-2.0.0/pyproject.toml` & `lbh15-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.8.10"
-dependencies = ["scipy>=1.8.1", "numpy>=1.22.3"]
+dependencies = ["scipy>=1.8.1", "numpy>=1.22.3", "sphinx>=6.2.1",
+                "sphinx-rtd-theme>=1.3.0", "myst-parser>=1.0.0", "sphinxcontrib-bibtex>=2.5.0"]
 
 [project.readme]
 file = "README.rst"
 content-type = "text/x-rst"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `lbh15-2.0.0/setup.py` & `lbh15-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,16 @@
                     'Handbook on Lead-bismuth Eutectic Alloy and '
                     'Lead Properties, Materials Compatibility, '
                     'Thermal-hydraulics and Technologies',
         long_description_content_type='text/x-rst',
         long_description=open('README.rst', 'r').read(),
         license='lgpl v3',
         python_requires='>=3.8.10',
-        install_requires=['scipy>=1.8.1', 'numpy>=1.22.3'],
+        install_requires=['scipy>=1.8.1', 'numpy>=1.22.3', 'sphinx>=6.2.1',
+                          'sphinx-rtd-theme>=1.3.0', 'myst-parser>=1.0.0', 'sphinxcontrib-bibtex>=2.5.0'],
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
             "Natural Language :: English",
             "Operating System :: OS Independent",
```

