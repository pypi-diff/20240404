# Comparing `tmp/weac-2.5.0.tar.gz` & `tmp/weac-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weac-2.5.0.tar", last modified: Sat Mar 30 12:42:17 2024, max compression
+gzip compressed data, was "weac-2.5.1.tar", last modified: Thu Apr  4 12:40:05 2024, max compression
```

## Comparing `weac-2.5.0.tar` & `weac-2.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-30 12:42:17.136848 weac-2.5.0/
--rw-r--r--   0 runner     (501) staff       (20)     1589 2024-03-30 12:42:05.000000 weac-2.5.0/CITATION.cff
--rw-r--r--   0 runner     (501) staff       (20)      129 2024-03-30 12:42:05.000000 weac-2.5.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       39 2024-03-30 12:42:05.000000 weac-2.5.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    16901 2024-03-30 12:42:17.136484 weac-2.5.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    16074 2024-03-30 12:42:05.000000 weac-2.5.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-30 12:42:17.126421 weac-2.5.0/build/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-30 12:42:17.135593 weac-2.5.0/build/weac.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      266 2024-03-30 12:42:17.000000 weac-2.5.0/build/weac.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-30 12:42:17.132459 weac-2.5.0/img/
--rw-r--r--   0 runner     (501) staff       (20)    70202 2024-03-30 12:42:05.000000 weac-2.5.0/img/bc.png
--rw-r--r--   0 runner     (501) staff       (20)    17056 2024-03-30 12:42:05.000000 weac-2.5.0/img/layering.png
--rw-r--r--   0 runner     (501) staff       (20)    82279 2024-03-30 12:42:05.000000 weac-2.5.0/img/logo.png
--rw-r--r--   0 runner     (501) staff       (20)    37795 2024-03-30 12:42:05.000000 weac-2.5.0/img/model.png
--rw-r--r--   0 runner     (501) staff       (20)    69175 2024-03-30 12:42:05.000000 weac-2.5.0/img/profiles.png
--rw-r--r--   0 runner     (501) staff       (20)    30453 2024-03-30 12:42:05.000000 weac-2.5.0/img/systems.png
--rw-r--r--   0 runner     (501) staff       (20)      121 2024-03-30 12:42:05.000000 weac-2.5.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      988 2024-03-30 12:42:17.137701 weac-2.5.0/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-30 12:42:17.135242 weac-2.5.0/weac/
--rw-r--r--   0 runner     (501) staff       (20)      359 2024-03-30 12:42:05.000000 weac-2.5.0/weac/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22491 2024-03-30 12:42:05.000000 weac-2.5.0/weac/eigensystem.py
--rw-r--r--   0 runner     (501) staff       (20)     1980 2024-03-30 12:42:05.000000 weac-2.5.0/weac/inverse.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1951 2024-03-30 12:42:05.000000 weac-2.5.0/weac/layered.py
--rw-r--r--   0 runner     (501) staff       (20)    70281 2024-03-30 12:42:05.000000 weac-2.5.0/weac/mixins.py
--rw-r--r--   0 runner     (501) staff       (20)    20705 2024-03-30 12:42:05.000000 weac-2.5.0/weac/plot.py
--rw-r--r--   0 runner     (501) staff       (20)     9605 2024-03-30 12:42:05.000000 weac-2.5.0/weac/tools.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.962766 weac-2.5.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-04 12:39:52.000000 weac-2.5.1/CITATION.cff
+-rw-r--r--   0 runner     (501) staff       (20)      129 2024-04-04 12:39:52.000000 weac-2.5.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       39 2024-04-04 12:39:52.000000 weac-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    17289 2024-04-04 12:40:05.962499 weac-2.5.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    16462 2024-04-04 12:39:52.000000 weac-2.5.1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.950802 weac-2.5.1/build/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.961659 weac-2.5.1/build/weac.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      266 2024-04-04 12:40:05.000000 weac-2.5.1/build/weac.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.958370 weac-2.5.1/img/
+-rw-r--r--   0 runner     (501) staff       (20)    70202 2024-04-04 12:39:52.000000 weac-2.5.1/img/bc.png
+-rw-r--r--   0 runner     (501) staff       (20)    17056 2024-04-04 12:39:52.000000 weac-2.5.1/img/layering.png
+-rw-r--r--   0 runner     (501) staff       (20)    82279 2024-04-04 12:39:52.000000 weac-2.5.1/img/logo.png
+-rw-r--r--   0 runner     (501) staff       (20)    37795 2024-04-04 12:39:52.000000 weac-2.5.1/img/model.png
+-rw-r--r--   0 runner     (501) staff       (20)    69175 2024-04-04 12:39:52.000000 weac-2.5.1/img/profiles.png
+-rw-r--r--   0 runner     (501) staff       (20)    30453 2024-04-04 12:39:52.000000 weac-2.5.1/img/systems.png
+-rw-r--r--   0 runner     (501) staff       (20)      184 2024-04-04 12:39:52.000000 weac-2.5.1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      988 2024-04-04 12:40:05.963817 weac-2.5.1/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.961254 weac-2.5.1/weac/
+-rw-r--r--   0 runner     (501) staff       (20)      359 2024-04-04 12:39:52.000000 weac-2.5.1/weac/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22476 2024-04-04 12:39:52.000000 weac-2.5.1/weac/eigensystem.py
+-rw-r--r--   0 runner     (501) staff       (20)     1980 2024-04-04 12:39:52.000000 weac-2.5.1/weac/inverse.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2064 2024-04-04 12:39:52.000000 weac-2.5.1/weac/layered.py
+-rw-r--r--   0 runner     (501) staff       (20)    70269 2024-04-04 12:39:52.000000 weac-2.5.1/weac/mixins.py
+-rw-r--r--   0 runner     (501) staff       (20)    20705 2024-04-04 12:39:52.000000 weac-2.5.1/weac/plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     9605 2024-04-04 12:39:52.000000 weac-2.5.1/weac/tools.py
```

### Comparing `weac-2.5.0/CITATION.cff` & `weac-2.5.1/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 authors:
 - family-names: "Rosendahl"
   given-names: "Philipp Laurens"
   orcid: "https://orcid.org/0000-0002-6587-875X"
 - family-names: "Weissgraeber"
   given-names: "Philipp"
   orcid: "https://orcid.org/0000-0001-8320-8672"
-version: 2.5.0
+version: 2.5.1
 date-released: 2021-12-30
 identifiers:
   - description: Collection of archived snapshots of all versions of WEAC
     type: doi
     value: 10.5281/zenodo.5773113
   - description: Release v2.4 for the analysis of slope-normal and vertical PST boundary conditions
     type: doi
```

### Comparing `weac-2.5.0/PKG-INFO` & `weac-2.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: weac
-Version: 2.5.0
-Summary: Weak layer anticrack nucleation model
-Home-page: https://github.com/2phi/weac
-Author: 2phi GbR
-Author-email: mail@2phi.de
-License: Proprietary
-Project-URL: Demo, https://github.com/2phi/weac/blob/main/demo/demo.ipynb
-Project-URL: Documentation, https://2phi.github.io/weac
-Project-URL: Issues and feature requests, https://github.com/2phi/weac/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy
-Provides-Extra: interactive
-Requires-Dist: jupyter; extra == "interactive"
-
 <!-- LOGO AND TITLE-->
 <!-- <p align="right"><img src="https://github.com/2phi/weac/raw/main/img/logo.png" alt="Logo" width="80" height="80"></p> -->
 
 
 <h1 align="center">
   <br>
   <img src="https://github.com/2phi/weac/raw/main/img/logo.png" alt="WEAC" width="120">
@@ -271,14 +247,20 @@
 2. Create your feature branch (`git checkout -b feature/amazingfeature`)
 3. Commit your changes (`git commit -m 'Add some amazing feature'`)
 4. Push to the branch (`git push origin feature/amazingfeature`)
 5. Open a pull request
 
 
 <!-- LICENSE -->
+## Workflows
+[![Publish Python 🐍 releases 📦 to PyPI ](https://github.com/2phi/weac/actions/workflows/release.yml/badge.svg)](https://github.com/2phi/weac/actions/workflows/release.yml)<br>
+[![Build and publish Sphinx 🪬 documentation ](https://github.com/2phi/weac/actions/workflows/docs.yml/badge.svg)](https://github.com/2phi/weac/actions/workflows/docs.yml)
+
+
+<!-- LICENSE -->
 ## License
 
 Copyright 2phi GbR, 2020-2024.
 
 We currently do not offer an open-source license. Please contact us for private licensing options.
 
 
@@ -315,8 +297,8 @@
 [forks-url]: https://github.com/2phi/weac/network/members
 [stars-url]: https://github.com/2phi/weac/stargazers
 [contributors-url]: https://github.com/2phi/weac/graphs/contributors
 [issues-url]: https://github.com/2phi/weac/issues
 [pypi-url]: https://pypi.org/project/weac/
 [release-url]: https://github.com/2phi/weac/releases
 [weac-url]: https://github.com/2phi/weac/
-[doi-url]: https://zenodo.org/badge/latestdoi/203163531
+[doi-url]: https://zenodo.org/badge/latestdoi/203163531
```

#### html2text {}

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1 Name: weac Version: 2.5.0 Summary: Weak layer anticrack
-nucleation model Home-page: https://github.com/2phi/weac Author: 2phi GbR
-Author-email: mail@2phi.de License: Proprietary Project-URL: Demo, https://
-github.com/2phi/weac/blob/main/demo/demo.ipynb Project-URL: Documentation,
-https://2phi.github.io/weac Project-URL: Issues and feature requests, https://
-github.com/2phi/weac/issues Classifier: Programming Language :: Python :: 3
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Topic :: Scientific/Engineering Requires-Python:
->=3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: matplotlib Requires-Dist: numpy Requires-Dist: scipy Provides-Extra:
-interactive Requires-Dist: jupyter; extra == "interactive"
                                     ************
                                     [[WWEEAACC]]
 
                                      WWEEAACC
                      WWeeaakk LLaayyeerr AAnnttiiccrraacckk NNuucclleeaattiioonn MMooddeell
                                      ************
  Implementation of closed-form analytical models for the analysis of dry-snow
@@ -113,15 +102,20 @@
 Documentation - Demo and examples ### v1.0 - Written in ð MATLAB -
 Deformation analysis of homogeneous snow labs - Weak-layer stress prediction -
 Energy release rates of cracks in weak layers - Finite fracture mechanics
 implementation - Prediction of anticrack nucleation ## How to contribute 1.
 Fork the project 2. Create your feature branch (`git checkout -b feature/
 amazingfeature`) 3. Commit your changes (`git commit -m 'Add some amazing
 feature'`) 4. Push to the branch (`git push origin feature/amazingfeature`) 5.
-Open a pull request ## License Copyright 2phi GbR, 2020-2024. We currently do
+Open a pull request ## Workflows [![Publish Python ð releases ð¦ to PyPI ]
+(https://github.com/2phi/weac/actions/workflows/release.yml/badge.svg)](https:/
+/github.com/2phi/weac/actions/workflows/release.yml)
+[![Build and publish Sphinx ðª¬ documentation ](https://github.com/2phi/weac/
+actions/workflows/docs.yml/badge.svg)](https://github.com/2phi/weac/actions/
+workflows/docs.yml) ## License Copyright 2phi GbR, 2020-2024. We currently do
 not offer an open-source license. Please contact us for private licensing
 options. ## Contact E-mail: mail@2phi.de Â· Web: https://2phi.de Â· Project
 Link: [https://github.com/2phi/weac](https://github.com/2phi/weac) Â· Project
 DOI: [http://dx.doi.org/10.5281/zenodo.5773113](http://dx.doi.org/10.5281/
 zenodo.5773113) [contributors-badge]: https://img.shields.io/github/
 contributors/2phi/weac.svg?style=flat-square&logo=github&color=yellow [forks-
 badge]: https://img.shields.io/github/forks/2phi/
```

### Comparing `weac-2.5.0/README.md` & `weac-2.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: weac
+Version: 2.5.1
+Summary: Weak layer anticrack nucleation model
+Home-page: https://github.com/2phi/weac
+Author: 2phi GbR
+Author-email: mail@2phi.de
+License: Proprietary
+Project-URL: Demo, https://github.com/2phi/weac/blob/main/demo/demo.ipynb
+Project-URL: Documentation, https://2phi.github.io/weac
+Project-URL: Issues and feature requests, https://github.com/2phi/weac/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Provides-Extra: interactive
+Requires-Dist: jupyter; extra == "interactive"
+
 <!-- LOGO AND TITLE-->
 <!-- <p align="right"><img src="https://github.com/2phi/weac/raw/main/img/logo.png" alt="Logo" width="80" height="80"></p> -->
 
 
 <h1 align="center">
   <br>
   <img src="https://github.com/2phi/weac/raw/main/img/logo.png" alt="WEAC" width="120">
@@ -247,14 +271,20 @@
 2. Create your feature branch (`git checkout -b feature/amazingfeature`)
 3. Commit your changes (`git commit -m 'Add some amazing feature'`)
 4. Push to the branch (`git push origin feature/amazingfeature`)
 5. Open a pull request
 
 
 <!-- LICENSE -->
+## Workflows
+[![Publish Python 🐍 releases 📦 to PyPI ](https://github.com/2phi/weac/actions/workflows/release.yml/badge.svg)](https://github.com/2phi/weac/actions/workflows/release.yml)<br>
+[![Build and publish Sphinx 🪬 documentation ](https://github.com/2phi/weac/actions/workflows/docs.yml/badge.svg)](https://github.com/2phi/weac/actions/workflows/docs.yml)
+
+
+<!-- LICENSE -->
 ## License
 
 Copyright 2phi GbR, 2020-2024.
 
 We currently do not offer an open-source license. Please contact us for private licensing options.
 
 
@@ -291,8 +321,8 @@
 [forks-url]: https://github.com/2phi/weac/network/members
 [stars-url]: https://github.com/2phi/weac/stargazers
 [contributors-url]: https://github.com/2phi/weac/graphs/contributors
 [issues-url]: https://github.com/2phi/weac/issues
 [pypi-url]: https://pypi.org/project/weac/
 [release-url]: https://github.com/2phi/weac/releases
 [weac-url]: https://github.com/2phi/weac/
-[doi-url]: https://zenodo.org/badge/latestdoi/203163531
+[doi-url]: https://zenodo.org/badge/latestdoi/203163531
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: weac Version: 2.5.1 Summary: Weak layer anticrack
+nucleation model Home-page: https://github.com/2phi/weac Author: 2phi GbR
+Author-email: mail@2phi.de License: Proprietary Project-URL: Demo, https://
+github.com/2phi/weac/blob/main/demo/demo.ipynb Project-URL: Documentation,
+https://2phi.github.io/weac Project-URL: Issues and feature requests, https://
+github.com/2phi/weac/issues Classifier: Programming Language :: Python :: 3
+Classifier: License :: Other/Proprietary License Classifier: Operating System
+:: OS Independent Classifier: Topic :: Scientific/Engineering Requires-Python:
+>=3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: matplotlib Requires-Dist: numpy Requires-Dist: scipy Provides-Extra:
+interactive Requires-Dist: jupyter; extra == "interactive"
                                     ************
                                     [[WWEEAACC]]
 
                                      WWEEAACC
                      WWeeaakk LLaayyeerr AAnnttiiccrraacckk NNuucclleeaattiioonn MMooddeell
                                      ************
  Implementation of closed-form analytical models for the analysis of dry-snow
@@ -102,15 +113,20 @@
 Documentation - Demo and examples ### v1.0 - Written in ð MATLAB -
 Deformation analysis of homogeneous snow labs - Weak-layer stress prediction -
 Energy release rates of cracks in weak layers - Finite fracture mechanics
 implementation - Prediction of anticrack nucleation ## How to contribute 1.
 Fork the project 2. Create your feature branch (`git checkout -b feature/
 amazingfeature`) 3. Commit your changes (`git commit -m 'Add some amazing
 feature'`) 4. Push to the branch (`git push origin feature/amazingfeature`) 5.
-Open a pull request ## License Copyright 2phi GbR, 2020-2024. We currently do
+Open a pull request ## Workflows [![Publish Python ð releases ð¦ to PyPI ]
+(https://github.com/2phi/weac/actions/workflows/release.yml/badge.svg)](https:/
+/github.com/2phi/weac/actions/workflows/release.yml)
+[![Build and publish Sphinx ðª¬ documentation ](https://github.com/2phi/weac/
+actions/workflows/docs.yml/badge.svg)](https://github.com/2phi/weac/actions/
+workflows/docs.yml) ## License Copyright 2phi GbR, 2020-2024. We currently do
 not offer an open-source license. Please contact us for private licensing
 options. ## Contact E-mail: mail@2phi.de Â· Web: https://2phi.de Â· Project
 Link: [https://github.com/2phi/weac](https://github.com/2phi/weac) Â· Project
 DOI: [http://dx.doi.org/10.5281/zenodo.5773113](http://dx.doi.org/10.5281/
 zenodo.5773113) [contributors-badge]: https://img.shields.io/github/
 contributors/2phi/weac.svg?style=flat-square&logo=github&color=yellow [forks-
 badge]: https://img.shields.io/github/forks/2phi/
```

### Comparing `weac-2.5.0/img/bc.png` & `weac-2.5.1/img/bc.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.0/img/layering.png` & `weac-2.5.1/img/layering.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.0/img/logo.png` & `weac-2.5.1/img/logo.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.0/img/model.png` & `weac-2.5.1/img/model.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.0/img/profiles.png` & `weac-2.5.1/img/profiles.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.0/img/systems.png` & `weac-2.5.1/img/systems.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.0/setup.cfg` & `weac-2.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weac
-version = 2.5.0
+version = 2.5.1
 author = 2phi GbR
 author_email = mail@2phi.de
 description = Weak layer anticrack nucleation model
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/2phi/weac
 project_urls =
```

### Comparing `weac-2.5.0/weac/eigensystem.py` & `weac-2.5.1/weac/eigensystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         self.betaU = False          # Ratio of slab to bedding stiffness (uncollapsed)
         self.betaC = False          # Ratio of slab to bedding stiffness (collapsed)
         self.mode = False           # Touchdown-mode can be either A, B, C or D
         self.td = False             # Touchdown length
 
     def set_foundation_properties(
             self,
-            t: float = 10.0,
+            t: float = 30.0,
             E: float = 0.25,
             nu: float = 0.25,
             update: bool = False):
         """
         Set material properties and geometry of foundation (weak layer).
 
         Arguments
@@ -183,29 +183,29 @@
             'E': E              # Young's modulus (MPa)
         }
 
         # Recalculate the fundamental system after properties have changed
         if update:
             self.calc_fundamental_system()
 
-    def set_beam_properties(self, layers, phi=0, C0=6.5, C1=4.4,
+    def set_beam_properties(self, layers, C0=6.5, C1=4.4,
                             nu=0.25, update=False):
         """
         Set material and properties geometry of beam (slab).
 
         Arguments
         ---------
         layers : list or str
             2D list of top-to-bottom layer densities and thicknesses.
             Columns are density (kg/m^3) and thickness (mm). One row
             corresponds to one layer. If entered as str, last split
             must be available in database.
         C0 : float, optional
             Multiplicative constant of Young modulus parametrization
-            according to Bergfeld et al. (2023). Default is 6.0.
+            according to Bergfeld et al. (2023). Default is 6.5.
         C1 : float, optional
             Exponent of Young modulus parameterization according to
             Bergfeld et al. (2023). Default is 4.6.
         nu : float, optional
             Possion's ratio. Default is 0.25
         update : bool, optional
             If true, recalculate the fundamental system after
@@ -222,15 +222,15 @@
         # Derive other elastic properties
         nu = nu*np.ones(layers.shape[0])         # Global poisson's ratio
         G = E/(2*(1 + nu))                       # Shear modulus
         self.k = 5/6                             # Shear correction factor
 
         # Compute total slab thickness and center of gravity
         self.h, self.zs = calc_center_of_gravity(layers)
-        
+
         # Assemble layering into matrix (top to bottom)
         # Columns are density (kg/m^3), layer thickness (mm)
         # Young's modulus (MPa), shear modulus (MPa), and
         # Poisson's ratio
         self.slab = np.vstack([layers.T, E, G, nu]).T
 
         # Recalculate the fundamental system after properties have changed
```

### Comparing `weac-2.5.0/weac/inverse.py` & `weac-2.5.1/weac/inverse.py`

 * *Files identical despite different names*

### Comparing `weac-2.5.0/weac/layered.py` & `weac-2.5.1/weac/layered.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,14 +33,16 @@
             from the right (vpst-), PST with vertical faces cut from the
             left (-vpst), one skier on infinite slab (skier) or multiple
             skiers on infinite slab (skiers). Default is 'pst-'.
         layers : list, optional
             2D list of layer densities and thicknesses. Columns are
             density(kg/m ^ 3) and thickness(mm). One row corresponds
             to one layer. Default is [[240, 200], ].
+        touchdown : bool, optional
+            Set True if slab touchdown is to be considered. Default is False.
         """
         # Call parent __init__
         super().__init__(system=system, touchdown=touchdown)
 
         # Set material properties and set up model
         self.set_beam_properties(layers if layers else [[240, 200], ])
         self.set_foundation_properties()
```

### Comparing `weac-2.5.0/weac/mixins.py` & `weac-2.5.1/weac/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1201,15 +1201,15 @@
             Fn, Ft = self.get_skier_load(m, phi)
             # Right-hand side for transmission from segment i-1 to segment i
             rhs[6*i:6*i + 3] = np.vstack([Ft, -Ft*self.h/2, Fn])
         # Set rhs so that complementary integral vanishes at boundaries
         if self.system not in ['pst-', '-pst', 'rested']:
             rhs[:3] = self.bc(self.zp(x=0, phi=phi, bed=ki[0]))
             rhs[-3:] = self.bc(self.zp(x=li[-1], phi=phi, bed=ki[-1]))
-            
+
         # Set rhs for vertical faces
         if self.system in ['vpst-', '-vpst']:
             # Calculate center of gravity and mass of
             # added or cut off slab segement
             xs, zs, m = calc_vertical_bc_center_of_gravity(self.slab, phi)
             # Convert slope angle to radians
             phi = np.deg2rad(phi)
```

### Comparing `weac-2.5.0/weac/plot.py` & `weac-2.5.1/weac/plot.py`

 * *Files identical despite different names*

### Comparing `weac-2.5.0/weac/tools.py` & `weac-2.5.1/weac/tools.py`

 * *Files identical despite different names*

