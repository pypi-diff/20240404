# Comparing `tmp/gemsembler-0.6.1.tar.gz` & `tmp/gemsembler-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemsembler-0.6.1.tar", last modified: Tue Apr  2 11:15:57 2024, max compression
+gzip compressed data, was "gemsembler-0.6.2.tar", last modified: Thu Apr  4 12:16:51 2024, max compression
```

## Comparing `gemsembler-0.6.1.tar` & `gemsembler-0.6.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.105188 gemsembler-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-02 11:15:45.000000 gemsembler-0.6.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-02 11:15:45.000000 gemsembler-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4174 2024-04-02 11:15:57.105188 gemsembler-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-02 11:15:45.000000 gemsembler-0.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1846 2024-04-02 11:15:45.000000 gemsembler-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 11:15:57.105188 gemsembler-0.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.097188 gemsembler-0.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.099188 gemsembler-0.6.1/src/gemsembler/
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     7898 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/anticreation.py
--rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/comparison.py
--rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/creation.py
--rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/curation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.100188 gemsembler-0.6.1/src/gemsembler/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.101188 gemsembler-0.6.1/src/gemsembler/data/BU/
--rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/BU_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/BU_gapseq.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.104188 gemsembler-0.6.1/src/gemsembler/data/LP/
--rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_CA1.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_CA2.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_MS2.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
--rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/dbs.py
--rw-rw-rw-   0 root         (0) root         (0)    18986 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/downstream.py
--rw-rw-rw-   0 root         (0) root         (0)    50045 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/drawing.py
--rw-rw-rw-   0 root         (0) root         (0)    24355 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/gathering.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/general.py
--rw-rw-rw-   0 root         (0) root         (0)    13330 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/genes.py
--rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/pathsfinding.py
--rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/periplasmic.py
--rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/selection.py
--rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/structural.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.105188 gemsembler-0.6.1/src/gemsembler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4174 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1435 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.105188 gemsembler-0.6.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_curation.py
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_dbs.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_gathering.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.787443 gemsembler-0.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-04 12:16:40.000000 gemsembler-0.6.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-04 12:16:40.000000 gemsembler-0.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4287 2024-04-04 12:16:51.786443 gemsembler-0.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-04 12:16:40.000000 gemsembler-0.6.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-04 12:16:40.000000 gemsembler-0.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 12:16:51.787443 gemsembler-0.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.777443 gemsembler-0.6.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.780443 gemsembler-0.6.2/src/gemsembler/
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7898 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/anticreation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/comparison.py
+-rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/curation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.781443 gemsembler-0.6.2/src/gemsembler/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.783443 gemsembler-0.6.2/src/gemsembler/data/BU/
+-rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/BU_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/BU_gapseq.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/BU/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.786443 gemsembler-0.6.2/src/gemsembler/data/LP/
+-rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_CA1.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_CA2.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_MS2.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
+-rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/LP/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)    19185 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/downstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    50045 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/drawing.py
+-rw-rw-rw-   0 root         (0) root         (0)    24476 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    13452 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/genes.py
+-rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/pathsfinding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/periplasmic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-04 12:16:40.000000 gemsembler-0.6.2/src/gemsembler/structural.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.786443 gemsembler-0.6.2/src/gemsembler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4287 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-04 12:16:51.000000 gemsembler-0.6.2/src/gemsembler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:16:51.786443 gemsembler-0.6.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_curation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-04 12:16:40.000000 gemsembler-0.6.2/tests/test_selection.py
```

### Comparing `gemsembler-0.6.1/LICENSE` & `gemsembler-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/PKG-INFO` & `gemsembler-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,14 +24,16 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://git.embl.de/grp-zimmermann-kogadeeva/GEMsembler
 Project-URL: Bug tracker, https://git.embl.de/grp-zimmermann-kogadeeva/GEMsembler/issues
 Keywords: genome scale metabolic models,metabolism,biology
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cobra
```

### Comparing `gemsembler-0.6.1/README.md` & `gemsembler-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/pyproject.toml` & `gemsembler-0.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemsembler"
-version = "0.6.1"
+version = "0.6.2"
 description = "A tool for assembling and comparing several types of Genome-Scale Metabolic Models."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     { name = "Elena Matveishina", email = "elena.matveishina@embl.de" },
     { name = "Bartosz Bartmanski", email = "bartosz.bartmanski@embl.de" }
 ]
 classifiers = [
+    "Intended Audience :: Science/Research",
+    "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["genome scale metabolic models", "metabolism", "biology"]
 requires-python = ">=3.9"
 dependencies = [
@@ -47,15 +49,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 [tool.bumpver]
-current_version = "0.6.1"
+current_version = "0.6.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gemsembler-0.6.1/src/gemsembler/__init__.py` & `gemsembler-0.6.2/src/gemsembler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from importlib.resources import files
 
 from .anticreation import get_model_of_interest
 from .creation import read_supermodel_from_pkl
 from .data import BU, LP
 from .gathering import GatheredModels, load_sbml_model
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 lp_example = [
     dict(
         model_id="curated_LP",
         path_to_model=files(LP) / "LP_iLP728_revision_data_met_C_c.xml.gz",
         model_type="carveme",
         path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
```

### Comparing `gemsembler-0.6.1/src/gemsembler/__main__.py` & `gemsembler-0.6.2/src/gemsembler/__main__.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/anticreation.py` & `gemsembler-0.6.2/src/gemsembler/anticreation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/comparison.py` & `gemsembler-0.6.2/src/gemsembler/comparison.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/conversion.py` & `gemsembler-0.6.2/src/gemsembler/conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/creation.py` & `gemsembler-0.6.2/src/gemsembler/creation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/curation.py` & `gemsembler-0.6.2/src/gemsembler/curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/BU/BU_agora.xml.gz` & `gemsembler-0.6.2/src/gemsembler/data/BU/BU_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/BU/BU_carveme_hom.xml.gz` & `gemsembler-0.6.2/src/gemsembler/data/BU/BU_carveme_hom.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/BU/BU_gapseq.xml.gz` & `gemsembler-0.6.2/src/gemsembler/data/BU/BU_gapseq.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/BU/BU_modelSEED.sbml.gz` & `gemsembler-0.6.2/src/gemsembler/data/BU/BU_modelSEED.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/LP/LP_CA1.xml.gz` & `gemsembler-0.6.2/src/gemsembler/data/LP/LP_CA1.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/LP/LP_CA2.xml.gz` & `gemsembler-0.6.2/src/gemsembler/data/LP/LP_CA2.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/LP/LP_MS2.sbml.gz` & `gemsembler-0.6.2/src/gemsembler/data/LP/LP_MS2.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/LP/LP_WCFS1.fasta.gz` & `gemsembler-0.6.2/src/gemsembler/data/LP/LP_WCFS1.fasta.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz` & `gemsembler-0.6.2/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz` & `gemsembler-0.6.2/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/data/LP/LP_protein_fasta.faa.gz` & `gemsembler-0.6.2/src/gemsembler/data/LP/LP_protein_fasta.faa.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/dbs.py` & `gemsembler-0.6.2/src/gemsembler/dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/downstream.py` & `gemsembler-0.6.2/src/gemsembler/downstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,16 +171,16 @@
         wid,
         hei,
     )
     if write_table:
         t_name = re.sub(".html$", ".tsv", output_name)
         t = table_reactions_confidence(
             supermodel,
-            list(glycolysis.keys()),
             t_name,
+            list(glycolysis.keys()),
             yes_range,
             no_range,
             genes,
             and_as_solid,
         )
         return g, t
     else:
@@ -246,16 +246,16 @@
         wid,
         hei,
     )
     if write_table:
         t_name = re.sub(".html$", ".tsv", output_name)
         t = table_reactions_confidence(
             supermodel,
-            list(tca.keys()),
             t_name,
+            list(tca.keys()),
             yes_range,
             no_range,
             genes,
             and_as_solid,
         )
         return g, t
     else:
@@ -303,16 +303,16 @@
         wid,
         hei,
     )
     if write_table:
         t_name = re.sub(".html$", ".tsv", output_name)
         t = table_reactions_confidence(
             supermodel,
-            list(pentose_phosphate_pathway.keys()),
             t_name,
+            list(pentose_phosphate_pathway.keys()),
             yes_range,
             no_range,
             genes,
             and_as_solid,
         )
         return g, t
     else:
@@ -457,26 +457,31 @@
 
     return out_bp_production_tab, flux_res_out, path_pfba_out, stat_out_tab
 
 
 def run_metquest_results_analysis(
     folder_with_mq_res_folders: str,
     model_list: list,
-    supermodel: SuperModel,
     metabolites_ids: list,
     medium: list,
+    supermodel=None,
     cofactors=None,
     output_folder=None,
     output_file_name=None,
     draw_mq_path=False,
     output_folder_mq_paths_plots=None,
     **kwargs,
 ):
     if output_folder_mq_paths_plots is not None:
         draw_mq_path = True
+    if (draw_mq_path is True) and (supermodel is None):
+        raise ValueError(
+            "Supermodel is needed to draw pathways, but not provided. "
+            "Please, provide supermodel."
+        )
     if (draw_mq_path is True) and (output_folder_mq_paths_plots is None):
         output_folder_mq_paths_plots = output_folder
     if cofactors is None:
         cofactors = [
             "co2",
             "hco3",
             "pi",
```

### Comparing `gemsembler-0.6.1/src/gemsembler/drawing.py` & `gemsembler-0.6.2/src/gemsembler/drawing.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/gathering.py` & `gemsembler-0.6.2/src/gemsembler/gathering.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,14 +516,16 @@
                     blast_command = "blastn"
                     db_name = "'nt_db'"
                 elif not aa_status and path_final_genome_aa is not None:
                     blast_command = "blastx"
                     db_name = "'aa_db'"
                 if blast_command == "" or db_name == "":
                     warnings.warn("\nWarning! Something wrong with aa/nt in files/DB")
+                elif not model_gene_file:
+                    warnings.warn("\nWarning! Something wrong with gene file")
                 else:
                     subprocess.run(
                         f"{blast_command} -query {model_gene_file} "
                         f"-db {Path(db_path, db_name)} "
                         f"-max_target_seqs 1 -outfmt '6' -out {out_blast_file}",
                         shell=True,
                         check=True,
```

### Comparing `gemsembler-0.6.1/src/gemsembler/genes.py` & `gemsembler-0.6.2/src/gemsembler/genes.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,18 @@
     )
     gene_gapseq_fasta = open(output_genes_name_gapseq, "w")
     for gene in gapseq_model.genes:
         gene_gapseq_fasta.write(">" + gene.id + "\n")
         start = gene.id.split("_")[-2]
         end = gene.id.split("_")[-1]
         genomeid = gene.id.removeprefix("gp_").removesuffix("_" + start + "_" + end)
-        genomeid = ".".join(genomeid.rsplit("_", 1))
+        if genomeid not in genomes.keys():
+            genomeid = ".".join(genomeid.rsplit("_", 1))
+        if genomeid not in genomes.keys():
+            return False, False
         start = int(start)
         end = int(end)
         if start < end:
             gene_gapseq_fasta.write(genomes.get(genomeid)[start:end] + "\n")
         else:
             gene_gapseq_fasta.write(genomes.get(genomeid)[end:start] + "\n")
     gene_gapseq_fasta.close()
```

### Comparing `gemsembler-0.6.1/src/gemsembler/pathsfinding.py` & `gemsembler-0.6.2/src/gemsembler/pathsfinding.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/periplasmic.py` & `gemsembler-0.6.2/src/gemsembler/periplasmic.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/selection.py` & `gemsembler-0.6.2/src/gemsembler/selection.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler/structural.py` & `gemsembler-0.6.2/src/gemsembler/structural.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/src/gemsembler.egg-info/PKG-INFO` & `gemsembler-0.6.2/src/gemsembler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.1
+Version: 0.6.2
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,14 +24,16 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://git.embl.de/grp-zimmermann-kogadeeva/GEMsembler
 Project-URL: Bug tracker, https://git.embl.de/grp-zimmermann-kogadeeva/GEMsembler/issues
 Keywords: genome scale metabolic models,metabolism,biology
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cobra
```

### Comparing `gemsembler-0.6.1/src/gemsembler.egg-info/SOURCES.txt` & `gemsembler-0.6.2/src/gemsembler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/tests/test_conversion.py` & `gemsembler-0.6.2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/tests/test_curation.py` & `gemsembler-0.6.2/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/tests/test_dbs.py` & `gemsembler-0.6.2/tests/test_dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/tests/test_gathering.py` & `gemsembler-0.6.2/tests/test_gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.1/tests/test_selection.py` & `gemsembler-0.6.2/tests/test_selection.py`

 * *Files identical despite different names*

