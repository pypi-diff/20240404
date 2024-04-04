# Comparing `tmp/pysipfenn-0.15.1.tar.gz` & `tmp/pysipfenn-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysipfenn-0.15.1.tar", last modified: Mon Mar 11 14:55:31 2024, max compression
+gzip compressed data, was "pysipfenn-0.16.0.tar", last modified: Thu Apr  4 16:24:34 2024, max compression
```

## Comparing `pysipfenn-0.15.1.tar` & `pysipfenn-0.16.0.tar`

### file list

```diff
@@ -1,109 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.668193 pysipfenn-0.15.1/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.652193 pysipfenn-0.15.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.656193 pysipfenn-0.15.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.github/workflows/coreTests_LinuxUbuntu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.github/workflows/coreTests_MacIntel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.github/workflows/coreTests_MacM1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.github/workflows/coreTests_Windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.github/workflows/fullTest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.github/workflows/publishPyPI.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.github/workflows/weeklyTesting.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-03-11 14:55:31.668193 pysipfenn-0.15.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.656193 pysipfenn-0.15.1/pysipfenn/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.656193 pysipfenn-0.15.1/pysipfenn/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14766 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/core/modelExporters.py
--rw-r--r--   0 runner    (1001) docker     (127)    64219 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/core/pysipfenn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.660193 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/
--rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/KS2022.py
--rw-r--r--   0 runner    (1001) docker     (127)    34747 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/KS2022_dilute.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29463 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    34479 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/Ward2017.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.660193 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   234243 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/assets/KS2022_randomSolution_ConvergencePlot.png
--rw-r--r--   0 runner    (1001) docker     (127)   141363 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/element_properties_Ward2017KS2022.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/labels_KS2022.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/labels_KS2022_randomSolutions.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/labels_Ward2017.csv
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/property_names_Ward2017KS2022.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.660193 pysipfenn-0.15.1/pysipfenn/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/misc/prototypeLibrary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.660193 pysipfenn-0.15.1/pysipfenn/modelsSIPFENN/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/modelsSIPFENN/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/modelsSIPFENN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/modelsSIPFENN/models.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.660193 pysipfenn-0.15.1/pysipfenn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.664193 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_KS2022_randomSolution_valueRangesMeans.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.668193 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)    68010 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.668193 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/
--rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/prototypeLibrary-custom.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_Core_prototypeLibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_KS2022.py
--rw-r--r--   0 runner    (1001) docker     (127)    22060 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_KS2022_dilute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_KS2022_randomSolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_ModelExporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_Ward2017.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_customModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-03-11 14:54:59.000000 pysipfenn-0.15.1/pysipfenn/tests/test_pysipfenn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:55:31.668193 pysipfenn-0.15.1/pysipfenn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-03-11 14:55:31.000000 pysipfenn-0.15.1/pysipfenn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-03-11 14:55:31.000000 pysipfenn-0.15.1/pysipfenn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 14:55:31.000000 pysipfenn-0.15.1/pysipfenn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-11 14:55:31.000000 pysipfenn-0.15.1/pysipfenn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-11 14:55:31.000000 pysipfenn-0.15.1/pysipfenn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 14:55:31.668193 pysipfenn-0.15.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.369413 pysipfenn-0.16.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.345413 pysipfenn-0.16.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.349413 pysipfenn-0.16.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.github/workflows/coreTests_LinuxUbuntu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.github/workflows/coreTests_MacIntel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.github/workflows/coreTests_MacM1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.github/workflows/coreTests_Windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.github/workflows/fullTest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.github/workflows/publishPyPI.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.github/workflows/weeklyTesting.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20262 2024-04-04 16:24:34.369413 pysipfenn-0.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.349413 pysipfenn-0.16.0/pysipfenn/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.353413 pysipfenn-0.16.0/pysipfenn/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48731 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/core/modelAdjusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14766 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/core/modelExporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66215 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/core/pysipfenn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.353413 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/
+-rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/KS2022.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34747 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/KS2022_dilute.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30793 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34479 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/Ward2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.353413 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   234243 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/assets/KS2022_randomSolution_ConvergencePlot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141363 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/element_properties_Ward2017KS2022.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/labels_KS2022.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/labels_KS2022_randomSolutions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/labels_Ward2017.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/property_names_Ward2017KS2022.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.357413 pysipfenn-0.16.0/pysipfenn/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/misc/prototypeLibrary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.357413 pysipfenn-0.16.0/pysipfenn/modelsSIPFENN/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/modelsSIPFENN/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/modelsSIPFENN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/modelsSIPFENN/models.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.357413 pysipfenn-0.16.0/pysipfenn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.361413 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/
+-rw-r--r--   0 runner    (1001) docker     (127)   102300 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/AdjusterTestDescriptors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53376 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/AdjusterTestDescriptors.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/AdjusterTestTargets.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/AdjusterTestTargets.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_KS2022_randomSolution_valueRangesMeans.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.365413 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)    68010 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.365413 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/prototypeLibrary-custom.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_Core_prototypeLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_KS2022.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22060 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_KS2022_dilute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_KS2022_randomSolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_ModelAdjusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_ModelExporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_Ward2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_customModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25418 2024-04-04 16:24:12.000000 pysipfenn-0.16.0/pysipfenn/tests/test_pysipfenn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:24:34.365413 pysipfenn-0.16.0/pysipfenn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20262 2024-04-04 16:24:34.000000 pysipfenn-0.16.0/pysipfenn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-04 16:24:34.000000 pysipfenn-0.16.0/pysipfenn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:24:34.000000 pysipfenn-0.16.0/pysipfenn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 16:24:34.000000 pysipfenn-0.16.0/pysipfenn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 16:24:34.000000 pysipfenn-0.16.0/pysipfenn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:24:34.369413 pysipfenn-0.16.0/setup.cfg
```

### Comparing `pysipfenn-0.15.1/.github/workflows/benchmarks.yaml` & `pysipfenn-0.16.0/.github/workflows/benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/.github/workflows/coreTests_LinuxUbuntu.yaml` & `pysipfenn-0.16.0/.github/workflows/coreTests_LinuxUbuntu.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/.github/workflows/coreTests_MacIntel.yaml` & `pysipfenn-0.16.0/.github/workflows/coreTests_MacIntel.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/.github/workflows/coreTests_MacM1.yaml` & `pysipfenn-0.16.0/.github/workflows/coreTests_MacM1.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/.github/workflows/coreTests_Windows.yaml` & `pysipfenn-0.16.0/.github/workflows/coreTests_Windows.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/.github/workflows/fullTest.yaml` & `pysipfenn-0.16.0/.github/workflows/fullTest.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/.github/workflows/publishPyPI.yaml` & `pysipfenn-0.16.0/.github/workflows/publishPyPI.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/.github/workflows/weeklyTesting.yaml` & `pysipfenn-0.16.0/.github/workflows/weeklyTesting.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/CITATION.cff` & `pysipfenn-0.16.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/LICENSE.md` & `pysipfenn-0.16.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/PKG-INFO` & `pysipfenn-0.16.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,7 @@
-Metadata-Version: 2.1
-Name: pysipfenn
-Version: 0.15.1
-Summary: Easily extensible Python package for featurizing periodic atomic structures and running Structure-Informed Prediction of Formation Energy using Neural Networks (SIPFENN)
-Author-email: Adam Krajewski <ak@psu.edu>, Jonathan Siegel <jwsiegel@tamu.edu>
-Project-URL: Research Page, https://phaseslab.com/sipfenn
-Project-URL: Homepage, https://pysipfenn.org
-Project-URL: Bug Tracker, https://github.com/PhasesResearchLab/pySIPFENN/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: pymatgen>=2024.2.20
-Requires-Dist: spglib==2.0.2
-Requires-Dist: torch>=2.1.0
-Requires-Dist: onnx2torch>=1.5.2
-Requires-Dist: onnx>=1.13.0
-Requires-Dist: numpy>=1.25.0
-Requires-Dist: tqdm>=4.65.0
-Requires-Dist: natsort>=8.3.0
-Requires-Dist: pymongo>=4.4
-Requires-Dist: pysmartdl2>=2.0.0
-Requires-Dist: dnspython
-Requires-Dist: ruamel.yaml
-Requires-Dist: colorama
-Provides-Extra: dev
-Requires-Dist: coremltools>=7.0; extra == "dev"
-Requires-Dist: onnxconverter_common>=1.14.0; extra == "dev"
-Requires-Dist: onnxsim==0.4.33; extra == "dev"
-Requires-Dist: onnxruntime>=1.16.0; extra == "dev"
-
 # pySIPFENN
 [![GitHub top language](https://img.shields.io/github/languages/top/PhasesResearchLab/pysipfenn)](https://github.com/PhasesResearchLab/pySIPFENN)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pysipfenn)](https://pypi.org/project/pysipfenn)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![PyPI - Version](https://img.shields.io/pypi/v/pysipfenn?label=PyPI&color=green)](https://pypi.org/project/pysipfenn)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pysipfenn)](https://pypi.org/project/pysipfenn)
 
@@ -52,50 +10,61 @@
 [![Core Mac Intel](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/coreTests_MacIntel.yaml/badge.svg)](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/coreTests_MacIntel.yaml)
 [![Core Windows](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/coreTests_Windows.yaml/badge.svg)](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/coreTests_Windows.yaml)
 [![Full Test](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/fullTest.yaml/badge.svg)](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/fullTest.yaml)
 [![codecov](https://codecov.io/gh/PhasesResearchLab/pySIPFENN/branch/main/graph/badge.svg?token=S2J0KR0WKQ)](https://codecov.io/gh/PhasesResearchLab/pySIPFENN)
 
 [![stable](https://img.shields.io/badge/Read%20The%20Docs-Stable-green)](https://pysipfenn.readthedocs.io/en/stable/) 
 [![latest](https://img.shields.io/badge/Read%20The%20Docs-Latest-green)](https://pysipfenn.readthedocs.io/en/latest/)
+[![Static Badge](https://img.shields.io/badge/First%20MGF%20Workshop%20Video%20-%20March%202023%20(v0.10.3)-rev?logo=YouTube&color=green)](https://youtube.com/watch?v=OHgkRuE0UQM)
+
+
 [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.commatsci.2022.111254-blue)](https://doi.org/10.1016/j.commatsci.2022.111254)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7373089.svg)](https://doi.org/10.5281/zenodo.7373089)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4006802.svg)](https://doi.org/10.5281/zenodo.4006802)
+[![Arxiv](https://img.shields.io/badge/arXiv-2404.02849-8F1515?style=flat&logo=arxiv&logoColor=red)](https://doi.org/10.48550/arXiv.2404.02849)
 
 ## Summary
 
 This repository contains 
-**py**(**S**tructure-**I**nformed **P**rediction of 
-**F**ormation **E**nergy using **N**eural **N**etworks) software 
-package allowing efficient predictions of the energetics of 
-atomic configurations. The underlying methodology and implementation
-is given in
+**py**thon toolset for **S**tructure-**I**nformed **P**roperty and **F**eature **E**ngineering with **N**eural **N**etworks 
+which implements a numer of user-friendly tools for:
+- **Calculating different vector representations of atomic structures** for a number of applications including supervised (e.g., predictive machine learning models) and unsupervised learning (e.g., clustering of atomic structures based on similarity or performing anomaly detection). Notably, utilize crystallographic information and some other techniques to make this process very efficient for the vast majority of use cases (see [arXiv:2404.02849](https://arxiv.org/abs/2404.02849))
+- **Efficient deployment of pre-trained ML models** (not limited to neural networks) obtained from repositories like Zenodo (including [some we trained](https://doi.org/10.5281/zenodo.4006802)) or trained locally on user's machine. The system is very plug-and-play thanks to using Open Neural Network Exchange (ONNX) format which can be exported from nearly any machine learning framework.
+- **Tuning pre-trained ML models to new domains**, like new chemical compositions, different ab initio functional, or entirely new properties. Since V0.16, users can take advantage of integration with [OPTIMADE API](https://www.optimade.org) which allows one to tune models based on DFT datasets like Materials Project, OQMD, AFLOW, or NIST-JARVIS, in **just 3 lines of code** specifying which provider to use, what to query for, and hyperparameters for tuning.
+
+The underlying methodology, efficiency optimizations, design choices, and implementation specifics are given in the following publications:
+
+- Adam M. Krajewski, Jonathan W. Siegel, Zi-Kui Liu, _Efficient Structure-Informed Featurization and Property Prediction of Ordered, Dilute, and Random Atomic Structures_, April 2024, [arXiv:2404.02849](https://arxiv.org/abs/2404.02849)
 
 - Adam M. Krajewski, Jonathan W. Siegel, Jinchao Xu, Zi-Kui Liu, _Extensible Structure-Informed Prediction of Formation Energy with improved accuracy and usability employing neural networks_, Computational Materials Science, Volume 208, 2022, 111254, DOI:[10.1016/j.commatsci.2022.111254](https://doi.org/10.1016/j.commatsci.2022.111254)
 
-While functionalities are similar to the software released along the 
-paper, this package contains improved methods for featurizing atomic 
-configurations. Notably, all of them are now written completely in 
-Python, removing reliance on Java and making extensions of the software
-much easier thanks to improved readability. A fuller description of capabilities is 
-given in documentation at https://pysipfenn.org and at PSU Phases 
-Research Lab webpage under https://phaseslab.com/sipfenn.
+A more complete (and verbose) description of capabilities is 
+given in documentation at [(pysipfenn.org)](https://pysipfenn.org). You may also consider visiting our 
+Phases Research Lab website at [(phaseslab.org)](https://phaseslab.org).
 
-### Major News:
+### Recent News:
 
-- **(v0.15.0)** A new descriptor (feature vector) calculator [**`descriptorDefinitions.KS2022_randomSolutions`**](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py) has been implemented. It is used for structure informed featurization of compositions randomly occupying a lattice, spiritually similar to SQS generation, but also taking into account (1) chemical differences between elements and (2) structural effects. A full description will be given in the upcoming manuscript.
+- **(v0.16.0)** Three exciting news! (1) The all new [`ModelAdjusters`](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/core/modelAdjusters.py) submodule automates tuning and can fetch data directly from [`OPTIMADE API`](https://www.optimade.org); (2) A new manuscript detailing advantages of our featurization tools has been put on [arXiv:2404.02849](https://arxiv.org/abs/2404.02849); and (3) the name of the software was updated to **py**thon toolset for **S**tructure-**I**nformed **P**roperty and **F**eature **E**ngineering with **N**eural **N**etworks to retain the `pySIPFENN` acronym but better reflect our strengths and development direction.
 
-- **(v0.14.0)** Users can now take advantage of a **Prototype Library** to obtain common structures from any `Calculator` instance `c` with a simple `c.prototypeLibrary['BCC']['structure']`. It can be easily [updated](https://pysipfenn.readthedocs.io/en/latest/source/pysipfenn.core.html#pysipfenn.Calculator.parsePrototypeLibrary) or [appended](https://pysipfenn.readthedocs.io/en/latest/source/pysipfenn.core.html#pysipfenn.Calculator.appendPrototypeLibrary) with high-level API or by manually modifyig its YAML [here](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/misc/prototypeLibrary.yaml).
+- **(v0.15.0)** A new descriptor (feature vector) calculator [**`KS2022_randomSolutions`**](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py) has been implemented. It is used for structure-informed featurization of compositions randomly occupying a lattice, spiritually similar to SQS generation, but also taking into account (1) chemical differences between elements and (2) structural effects. 
+
+- **(v0.14.0)** Users can now take advantage of a **Prototype Library** to obtain common structures from any `Calculator` instance with `c.prototypeLibrary[<name>]['structure']`. It can be easily [updated](https://pysipfenn.readthedocs.io/en/latest/source/pysipfenn.core.html#pysipfenn.Calculator.parsePrototypeLibrary) or [appended](https://pysipfenn.readthedocs.io/en/latest/source/pysipfenn.core.html#pysipfenn.Calculator.appendPrototypeLibrary) with high-level API or by manually modifyig its YAML [here](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/misc/prototypeLibrary.yaml).
 
 - **(v0.13.0)** Model exports (and more!) to PyTorch, CoreML, and ONNX are now effortless thanks to [**`core.modelExporters`**](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/core/modelExporters.py) module. Please note you need to install pySIPFENN with `dev` option (e.g., `pip install "pysipfenn[dev]"`) to use it. See [docs here](https://pysipfenn.readthedocs.io/en/stable/source/pysipfenn.core.html#module-pysipfenn.core.modelExporters).
 
-- **(v0.12.2)** Swith to LGPLv3 allowing for integration with proprietary software developed by CALPHAD community, while supporting the development of new pySIPFENN features for all. Many thanks to our colleagues from 
-[GTT-Technologies](https://gtt-technologies.de) and other participants of [CALPHAD 2023](https://calphad.org/calphad-2023) for fruitful discussions.
+- **(v0.12.2)** Swith to LGPLv3 allowing for integration with proprietary software developed by CALPHAD community, while supporting the development of new pySIPFENN features for all.
+
+- **(March 2023 Workshop)** We would like to thank all 100 of our amazing attendees for making our workshop, co-organized with the
+[Materials Genome Foundation](https://materialsgenomefoundation.org).
+
+### Main Schematic
 
-- **(March 2023 Workshop)** We would like to thank all of our amazing attendees for making our workshop, co-organized with the
-[Materials Genome Foundation](https://materialsgenomefoundation.org), such a success! Over 100 of you simultaneously followed
-all exercises and, at the peak, we loaded over 1,200GB of models into the HPC's RAM. 
+The figure below is the main schematic of `pySIPFENN` framework detailing the interplay of internal components. The user interface provides a high-level API to process structural data within `core.Calculator`, pass it to featurization submodules in `descriptorDefinitions` to obtain vector representation, then passed to models defined in `models.json` and (typically) run automatically through all available models. All internal data of `core.Calculator` is accessible directly, enabling rapid customization. An auxiliary high-level API enables advanced users to operate and retrain the models.
+
+<img src="https://raw.githubusercontent.com/PhasesResearchLab/pySIPFENN/main/docs/_static/pySIPFENN_MainSchematic.png" alt="Main Schematic Figure" width="800" style="display: block; margin-left: auto; margin-right: auto;"/>
+   
 
 ### Applications
 
 pySIPFENN is a very flexible tool that can, in principle, be used for
 the prediction of any property of interest that depends on an atomic
 configuration with very few modifications. The models shipped by
 default are trained to predict formation energy because that is what our
@@ -229,13 +198,15 @@
 
 
 
 ## Cite
 
 If you use `pySIPFENN` software, please consider citing:
 
+- Adam M. Krajewski, Jonathan W. Siegel, Zi-Kui Liu, _Efficient Structure-Informed Featurization and Property Prediction of Ordered, Dilute, and Random Atomic Structures_, April 2024, [arXiv:2404.02849](https://arxiv.org/abs/2404.02849)
+
 - Adam M. Krajewski, Jonathan W. Siegel, Jinchao Xu, Zi-Kui Liu, _Extensible Structure-Informed Prediction of Formation Energy with improved accuracy and usability employing neural networks_, Computational Materials Science, Volume 208, 2022, 111254, DOI:[10.1016/j.commatsci.2022.111254](https://doi.org/10.1016/j.commatsci.2022.111254)
 
 If you are using predictions from pySIPFENN models accessed through `OPTIMADE` from `MPDD`, please additionally cite:
 
 - Matthew L. Evans, Johan Bergsma, ..., Adam M. Krajewski, ..., Zi-Kui Liu, ..., et al., _Developments and applications of the OPTIMADE API for materials discovery, design, and data exchange_, 2024, [arXiv:2402.00572](https://arxiv.org/abs/2402.00572)
```

### Comparing `pysipfenn-0.15.1/pyproject.toml` & `pysipfenn-0.16.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysipfenn"
-version = "0.15.1"
+version = "0.16.0"
 authors = [
   { name="Adam Krajewski", email="ak@psu.edu" },
-    { name="Jonathan Siegel", email="jwsiegel@tamu.edu" },
+  { name="Jonathan Siegel", email="jwsiegel@tamu.edu" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
@@ -19,39 +19,41 @@
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Physics",
 ]
-description = "Easily extensible Python package for featurizing periodic atomic structures and running Structure-Informed Prediction of Formation Energy using Neural Networks (SIPFENN)"
+description = "Python toolset for Structure-Informed Property and Feature Engineering with Neural Networks. It offers unique advantages through (1) effortless extensibility, (2) optimizations for ordered, dilute, and random atomic configurations, and (3) automated model tuning."
 readme = "README.md"
 
 requires-python = ">=3.9"
 dependencies = [
     "pymatgen>=2024.2.20",
     "spglib==2.0.2",
     "torch>=2.1.0",
     "onnx2torch>=1.5.2",
     "onnx>=1.13.0",
     "numpy>=1.25.0",
     "tqdm>=4.65.0",
     "natsort>=8.3.0",
     "pymongo>=4.4",
     "pysmartdl2>=2.0.0",
+    "plotly>=5.15.0",
     "dnspython",
     "ruamel.yaml",
     "colorama"
 ]
 
 [project.optional-dependencies]
 dev = [
     "coremltools>=7.0",
     "onnxconverter_common>=1.14.0",
     "onnxsim==0.4.33",
-    "onnxruntime>=1.16.0"
+    "onnxruntime>=1.16.0",
+    "optimade[http_client]>=1.0.0"
 ]
 
 [project.urls]
-"Research Page" = "https://phaseslab.com/sipfenn"
+"Repository" = "https://git.pysipfenn.org"
 "Homepage" = "https://pysipfenn.org"
 "Bug Tracker" = "https://github.com/PhasesResearchLab/pySIPFENN/issues"
```

### Comparing `pysipfenn-0.15.1/pysipfenn/core/modelExporters.py` & `pysipfenn-0.16.0/pysipfenn/core/modelExporters.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/core/pysipfenn.py` & `pysipfenn-0.16.0/pysipfenn/core/pysipfenn.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # Descriptor Generators
 from pysipfenn.descriptorDefinitions import (
     Ward2017, KS2022, KS2022_dilute, KS2022_randomSolutions
 )
 
 # - add new ones here if extending the code
 
-__version__ = '0.15.0'
+__version__ = '0.16.0'
 __authors__ = [["Adam Krajewski", "ak@psu.edu"],
                ["Jonathan Siegel", "jwsiegel@tamu.edu"]]
 __name__ = 'pysipfenn'
 
 # *********************************  CALCULATION HIGH-LEVEL ENVIRONMENT  *********************************
 class Calculator:
     """pySIPFENN Calculator automatically initializes all functionalities including identification and loading
@@ -69,15 +69,15 @@
 
     def __init__(self,
                  autoLoad: bool = True,
                  verbose: bool = True):
         """Initializes the pySIPFENN Calculator object."""
         if verbose:
             print('\n*********  Initializing pySIPFENN Calculator  **********')
-            self.verbose = verbose
+        self.verbose = verbose
         # dictionary with all model information
         with resources.files('pysipfenn.modelsSIPFENN').joinpath('models.json').open('r') as f:
             if verbose:
                 print(f'Loading model definitions from: {Fore.BLUE}{f.name}{Style.RESET_ALL}')
             self.models = json.load(f)
         # networks list
         self.network_list = list(self.models.keys())
@@ -1034,15 +1034,15 @@
         """Writes the descriptor data to a CSV file. The first column is the name of the structure. If the
         ``self.inputFiles`` attribute is populated automatically by runFromDirectory() or set manually, the names of the
         structures will be used. Otherwise, the names will be ``'1'``, ``'2'``, ``'3'``, etc. The remaining columns are the
         descriptor values. The order of the columns is the same as the order of the labels in the descriptor
         definition file.
 
         Args:
-            descriptor: Descriptor to use. Must be one of the available descriptors. See ``pysipgenn.descriptorDefinitions``
+            descriptor: Descriptor to use. Must be one of the available descriptors. See ``pysipfenn.descriptorDefinitions``
                 for a list of available descriptors, such as ``'KS2022'`` and ``'Ward2017'``. It provides the labels for the
                 descriptor values.
             file: Name of the file to write the results to. If the file already exists, it will be overwritten. If the
                 file does not exist, it will be created. The file must have a ``'.csv'`` extension to be recognized
                 correctly.
         """
 
@@ -1061,14 +1061,36 @@
                     f.write(f'{name},{",".join(str(v) for v in dd.tolist())}\n')
             else:
                 i = 1
                 for dd in self.descriptorData:
                     f.write(f'{i},{",".join(str(v) for v in dd)}\n')
                     i += 1
 
+    def writeDescriptorsToNPY(self, descriptor: str, file: str = 'descriptorData.npy') -> None:
+        """Writes the descriptor data to a numpy file (.NPY). The order of the columns in the numpy array corresponds 
+        to the order of the labels in the descriptor definition files at ``descriptorDefinitions`` directory. To match the 
+        data with the labels, load the labels from the descriptor definition file and use the same index to access the 
+        corresponding data in the numpy array. The order of the rows corresponds to the last run input structures.
+
+        Args:
+            descriptor: Descriptor to use. Must be one of the available descriptors. See ``pysipfenn.descriptorDefinitions``
+                for a list of available descriptors, such as ``'KS2022'`` and ``'Ward2017'``.
+            file: Name of the file to write the results to. If the file already exists, it will be overwritten. If the
+                file does not exist, it will be created. The file must have a ``'.npy'`` extension to be recognized
+                correctly. Default is ``'descriptorData.npy'``.
+        """
+
+        # Write descriptor data
+        if file == 'descriptorData.npy':
+            print(f"Writing descriptor data to {descriptor}_{file}...")
+            np.save(f'{descriptor}_descriptorData.npy', self.descriptorData)
+        else:
+            print(f"Writing descriptor data to {file}...")
+            np.save(file, self.descriptorData)
+
     def destroy(self) -> None:
             """Deallocates all loaded models and clears all data from the Calculator object."""
             self.loadedModels.clear()
             self.toRun.clear()
             self.descriptorData.clear()
             self.predictions.clear()
             self.inputFiles.clear()
@@ -1076,15 +1098,19 @@
             print("Calculator and all loaded models deallocated. All data cleared.")
             del self
 
 
 # ************************  SATELLITE FUNCTIONS  ************************
             
 def ward2ks2022(ward2017: np.ndarray) -> np.ndarray:
-    """Converts a ``Ward2017`` descriptor to a ``KS2022`` descriptor (which is its subset).
+    """Converts a ``Ward2017`` descriptor to a ``KS2022`` descriptor (which is its subset). It removes: `mean_WCMagnitude_Shell1`, `mean_WCMagnitude_Shell2`, 
+    `mean_WCMagnitude_Shell3`, `mean_NeighDiff_shell1_SpaceGroupNumber`, `var_NeighDiff_shell1_SpaceGroupNumber`, `min_NeighDiff_shell1_SpaceGroupNumber`, 
+    `max_NeighDiff_shell1_SpaceGroupNumber`, `range_NeighDiff_shell1_SpaceGroupNumber`, `mean_SpaceGroupNumber`, `maxdiff_SpaceGroupNumber`, 
+    `dev_SpaceGroupNumber`, `max_SpaceGroupNumber`, `min_SpaceGroupNumber`, `most_SpaceGroupNumber`, and `CanFormIonic`, for physicality and performance 
+    improvements.
 
     Args:
         ward2017: ``Ward2017`` descriptor. Must be a 1D ``np.ndarray`` of length ``271``.
 
     Returns:
         ``KS2022`` descriptor array.
     """
```

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/KS2022.py` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/KS2022.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/KS2022_dilute.py` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/KS2022_dilute.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,123 +287,139 @@
 
     if maxDiff < featureConvergenceCriterion:
         raise AssertionError('Invalid convergence criteria (maxDiff < featureConvergenceCriterion).')
     if compositionDistance < compositionConvergenceCriterion:
         raise AssertionError('Invalid convergence criteria (compositionDistance > compositionConvergenceCriterion).')
     if minOccupationCount > minimumElementOccurrences:
         raise AssertionError('Invalid convergence criteria (minOccupationCount > minimumElementOccurrences).')
-
-    while maxDiff > featureConvergenceCriterion \
-            or compositionDistance > compositionConvergenceCriterion \
-            or minOccupationCount < minimumElementOccurrences:
-        # Choose random structure occupation
-        randomOccupation = random.choices(list(elementalFrequencies.keys()),
-                                          weights=elementalFrequencies.values(),
-                                          k=adjustedStruct.num_sites)
-        allOccupations += randomOccupation
-        occupationCount = dict(Counter(allOccupations))
-        minOccupationCount = min(occupationCount.values())
-        currentComposition = Composition.from_dict(occupationCount)
-        # Adjust current elemental frequencies to push the current composition towards the target composition
-
-        compositionDistance = 0
-        for element in elementalFrequencies.keys():
-            difference = currentComposition.fractional_composition.get_atomic_fraction(element) \
-                         - comp.fractional_composition.get_atomic_fraction(element)
-            compositionDistance += abs(difference)
-            elementalFrequencies[element] -= difference * 0.1
-        compositionDistance /= len(elementalFrequencies.keys())
-
-        for site, occupation in zip(adjustedStruct.sites, randomOccupation):
-            site.species = occupation
-
-        diff_properties_instance, attribute_properties_instance = generate_voronoi_attributes(struct=adjustedStruct)
-
-        diff_properties = np.concatenate((diff_properties, diff_properties_instance), axis=0)
-        attribute_properties = np.concatenate((attribute_properties, attribute_properties_instance), axis=0)
-
-        properties = np.concatenate(
-            (np.stack(
-                (np.mean(diff_properties, axis=0),
-                 np.mean(np.abs(diff_properties - np.mean(diff_properties, axis=0)), axis=0),
-                 np.min(diff_properties, axis=0),
-                 np.max(diff_properties, axis=0),
-                 np.max(diff_properties, axis=0) - np.min(diff_properties, axis=0)), axis=-1).reshape((-1)),
-             np.stack(
-                 (np.mean(attribute_properties, axis=0),
-                  np.max(attribute_properties, axis=0) - np.min(attribute_properties, axis=0),
-                  np.mean(np.abs(attribute_properties - np.mean(attribute_properties, axis=0)), axis=0),
-                  np.max(attribute_properties, axis=0),
-                  np.min(attribute_properties, axis=0),
-                  most_common(attribute_properties)), axis=-1).reshape((-1))))
-        # Normalize Bond Length properties.
-        properties[6] /= properties[5]
-        properties[7] /= properties[5]
-        properties[8] /= properties[5]
-        # Normalize the Cell Volume Deviation.
-        properties[16] /= properties[15]
-        # Remove properties not in magpie.
-        properties = np.delete(properties, [4, 5, 9, 14, 15, 17, 18, 19, 21, 22, 23, 24])
-        # Renormalize the packing efficiency.
-        properties[12] *= adjustedStruct.num_sites / adjustedStruct.volume
-        # Calculate and insert stoichiometry attributes.
-        element_dict = currentComposition.fractional_composition.as_dict()
-        position = 118
-        for p in [10, 7, 5, 3, 2]:
-            properties = np.insert(properties, position,
-                                   math.pow(sum(math.pow(value, p) for value in element_dict.values()), 1.0 / p))
-        properties = np.insert(properties, position, len(element_dict))
-        # Calculate Valence Electron Statistics
-        electron_occupation_dict = {'s': 0, 'p': 0, 'd': 0, 'f': 0}
-        for key, value in element_dict.items():
-            electron_occupation_dict['s'] += value * attribute_matrix[Element(key).Z - 1][8]
-            electron_occupation_dict['p'] += value * attribute_matrix[Element(key).Z - 1][9]
-            electron_occupation_dict['d'] += value * attribute_matrix[Element(key).Z - 1][10]
-            electron_occupation_dict['f'] += value * attribute_matrix[Element(key).Z - 1][11]
-        total_valence_factor = sum([val for (key, val) in electron_occupation_dict.items()])
-        for orb in ['s', 'p', 'd', 'f']:
-            properties = np.append(properties, electron_occupation_dict[orb] / total_valence_factor)
-        # Calculate ionic compound attributes.
-        max_ionic_char = 0
-        av_ionic_char = 0
-        for key1, value1 in element_dict.items():
-            for key2, value2 in element_dict.items():
-                ionic_char = 1.0 - math.exp(-0.25 * (Element(key1).X - Element(key2).X) ** 2)
-                if ionic_char > max_ionic_char:
-                    max_ionic_char = ionic_char
-                av_ionic_char += ionic_char * value1 * value2
-        properties = np.append(properties, max_ionic_char)
-        properties = np.append(properties, av_ionic_char)
-        properties = properties.astype(np.float32)
-
-        propHistory.append(properties)
-        # Calculate the difference between the current step and the previous step and divide it by maximum value of
-        # each feature found in OQMD to normalize the difference.
-        if len(propHistory) > 2:
-            # Current iteration diff
-            diff = np.subtract(properties, propHistory[-2])
-            diff /= maxFeaturesInOQMD
-            diffHistory.append(diff)
-            # Calculate the additional diff to one level older iteration
-            diff2 = np.subtract(properties, propHistory[-3])
-            diff2 /= maxFeaturesInOQMD
-            # Calculate the maximum difference across both differences
-            maxDiff = max(np.concatenate((diff, diff2), axis=0))
-            if printProgress:
-                print(f'{attribute_properties.shape[0]:^6} | '
-                      f'{compositionDistance: 18.6f} | '
-                      f'{maxDiff: 21.6f} | '
-                      f'{minOccupationCount:^4}')
+    try:
+        while maxDiff > featureConvergenceCriterion \
+                or compositionDistance > compositionConvergenceCriterion \
+                or minOccupationCount < minimumElementOccurrences:
+            # Choose random structure occupation
+            randomOccupation = random.choices(list(elementalFrequencies.keys()),
+                                              weights=elementalFrequencies.values(),
+                                              k=adjustedStruct.num_sites)
+            allOccupations += randomOccupation
+            occupationCount = dict(Counter(allOccupations))
+            minOccupationCount = min(occupationCount.values())
+            currentComposition = Composition.from_dict(occupationCount)
+            # Adjust current elemental frequencies to push the current composition towards the target composition
+
+            compositionDistance = 0
+            for element in elementalFrequencies.keys():
+                difference = currentComposition.fractional_composition.get_atomic_fraction(element) \
+                             - comp.fractional_composition.get_atomic_fraction(element)
+                compositionDistance += abs(difference)
+                elementalFrequencies[element] -= difference * 0.1
+            compositionDistance /= len(elementalFrequencies.keys())
+
+            for site, occupation in zip(adjustedStruct.sites, randomOccupation):
+                site.species = occupation
+
+            diff_properties_instance, attribute_properties_instance = generate_voronoi_attributes(struct=adjustedStruct)
+
+            diff_properties = np.concatenate((diff_properties, diff_properties_instance), axis=0)
+            attribute_properties = np.concatenate((attribute_properties, attribute_properties_instance), axis=0)
+
+            properties = np.concatenate(
+                (np.stack(
+                    (np.mean(diff_properties, axis=0),
+                     np.mean(np.abs(diff_properties - np.mean(diff_properties, axis=0)), axis=0),
+                     np.min(diff_properties, axis=0),
+                     np.max(diff_properties, axis=0),
+                     np.max(diff_properties, axis=0) - np.min(diff_properties, axis=0)), axis=-1).reshape((-1)),
+                 np.stack(
+                     (np.mean(attribute_properties, axis=0),
+                      np.max(attribute_properties, axis=0) - np.min(attribute_properties, axis=0),
+                      np.mean(np.abs(attribute_properties - np.mean(attribute_properties, axis=0)), axis=0),
+                      np.max(attribute_properties, axis=0),
+                      np.min(attribute_properties, axis=0),
+                      most_common(attribute_properties)), axis=-1).reshape((-1))))
+            # Normalize Bond Length properties.
+            properties[6] /= properties[5]
+            properties[7] /= properties[5]
+            properties[8] /= properties[5]
+            # Normalize the Cell Volume Deviation.
+            properties[16] /= properties[15]
+            # Remove properties not in magpie.
+            properties = np.delete(properties, [4, 5, 9, 14, 15, 17, 18, 19, 21, 22, 23, 24])
+            # Renormalize the packing efficiency.
+            properties[12] *= adjustedStruct.num_sites / adjustedStruct.volume
+            # Calculate and insert stoichiometry attributes.
+            element_dict = currentComposition.fractional_composition.as_dict()
+            position = 118
+            for p in [10, 7, 5, 3, 2]:
+                properties = np.insert(properties, position,
+                                       math.pow(sum(math.pow(value, p) for value in element_dict.values()), 1.0 / p))
+            properties = np.insert(properties, position, len(element_dict))
+            # Calculate Valence Electron Statistics
+            electron_occupation_dict = {'s': 0, 'p': 0, 'd': 0, 'f': 0}
+            for key, value in element_dict.items():
+                electron_occupation_dict['s'] += value * attribute_matrix[Element(key).Z - 1][8]
+                electron_occupation_dict['p'] += value * attribute_matrix[Element(key).Z - 1][9]
+                electron_occupation_dict['d'] += value * attribute_matrix[Element(key).Z - 1][10]
+                electron_occupation_dict['f'] += value * attribute_matrix[Element(key).Z - 1][11]
+            total_valence_factor = sum([val for (key, val) in electron_occupation_dict.items()])
+            for orb in ['s', 'p', 'd', 'f']:
+                properties = np.append(properties, electron_occupation_dict[orb] / total_valence_factor)
+            # Calculate ionic compound attributes.
+            max_ionic_char = 0
+            av_ionic_char = 0
+            for key1, value1 in element_dict.items():
+                for key2, value2 in element_dict.items():
+                    ionic_char = 1.0 - math.exp(-0.25 * (Element(key1).X - Element(key2).X) ** 2)
+                    if ionic_char > max_ionic_char:
+                        max_ionic_char = ionic_char
+                    av_ionic_char += ionic_char * value1 * value2
+            properties = np.append(properties, max_ionic_char)
+            properties = np.append(properties, av_ionic_char)
+            properties = properties.astype(np.float32)
+
+            propHistory.append(properties)
+            # Calculate the difference between the current step and the previous step and divide it by maximum value of
+            # each feature found in OQMD to normalize the difference.
+            if len(propHistory) > 2:
+                # Current iteration diff
+                diff = np.subtract(properties, propHistory[-2])
+                diff /= maxFeaturesInOQMD
+                diffHistory.append(diff)
+                # Calculate the additional diff to one level older iteration
+                diff2 = np.subtract(properties, propHistory[-3])
+                diff2 /= maxFeaturesInOQMD
+                # Calculate the maximum difference across both differences
+                maxDiff = max(np.concatenate((diff, diff2), axis=0))
+                if printProgress:
+                    print(f'{attribute_properties.shape[0]:^6} | '
+                          f'{compositionDistance: 18.6f} | '
+                          f'{maxDiff: 21.6f} | '
+                          f'{minOccupationCount:^4}')
+            else:
+                if printProgress:
+                    print(f'{attribute_properties.shape[0]:^6} | '
+                          f'{compositionDistance: 18.6f} | '
+                          f'{"(init)":^21} | '
+                          f'{minOccupationCount:^4}')
+        # ^^^ End of the long while-loop above
+    except KeyboardInterrupt:
+        if len(propHistory) == 0:
+            raise KeyboardInterrupt(
+                'KS2022_randomSolution descriptor calculation was interrupted before it managed to complete the '
+                'first iteration.')
         else:
-            if printProgress:
-                print(f'{attribute_properties.shape[0]:^6} | '
-                      f'{compositionDistance: 18.6f} | '
-                      f'{"(init)":^21} | '
-                      f'{minOccupationCount:^4}')
-    # ^^^ End of the long while-loop above
+            if len(diffHistory) == 0:
+                print(
+                    'Warning: The feature calculation was interrupted before it managed to begin convergence process. '
+                    'The first one or two iterations was completed and partial results are available but there was not '
+                    'enough data to calculate the convergence level.')
+            else:
+                print(
+                    'The feature calculation was interrupted before it managed to converge. Partial results  are '
+                    'available, including the level of convergence achieved before the interruption.')
+            pass
 
     if plotParameters:
         import plotly.express as px
         import pandas as pd
         import warnings
         warnings.simplefilter(action='ignore', category=pd.errors.PerformanceWarning)
```

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/README.md` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/README.md`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/Ward2017.py` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/Ward2017.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/assets/KS2022_randomSolution_ConvergencePlot.png` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/assets/KS2022_randomSolution_ConvergencePlot.png`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/element_properties_Ward2017KS2022.csv` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/element_properties_Ward2017KS2022.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/labels_KS2022.csv` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/labels_KS2022.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/labels_KS2022_randomSolutions.csv` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/labels_KS2022_randomSolutions.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/labels_Ward2017.csv` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/labels_Ward2017.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/descriptorDefinitions/property_names_Ward2017KS2022.txt` & `pysipfenn-0.16.0/pysipfenn/descriptorDefinitions/property_names_Ward2017KS2022.txt`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/misc/prototypeLibrary.yaml` & `pysipfenn-0.16.0/pysipfenn/misc/prototypeLibrary.yaml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/modelsSIPFENN/models.json` & `pysipfenn-0.16.0/pysipfenn/modelsSIPFENN/models.json`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_KS2022_randomSolution_valueRangesMeans.csv` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_KS2022_randomSolution_valueRangesMeans.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR` & `pysipfenn-0.16.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_Core_prototypeLibrary.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_Core_prototypeLibrary.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_KS2022.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_KS2022.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_KS2022_dilute.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_KS2022_dilute.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_KS2022_randomSolutions.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_KS2022_randomSolutions.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_ModelExporters.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_ModelExporters.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_Ward2017.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_Ward2017.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_customModel.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_customModel.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.15.1/pysipfenn/tests/test_pysipfenn.py` & `pysipfenn-0.16.0/pysipfenn/tests/test_pysipfenn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 import pytest
 import os
+import numpy as np
 
 import pysipfenn
 from importlib import resources
 from natsort import natsorted
 from numpy import zeros
 
 from pymatgen.core import Structure, Composition
@@ -314,14 +315,42 @@
             with resources.files('pysipfenn').joinpath(
                     'tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv').open('r',
                                                                                                    newline=''
                                                                                                    ) as f2:
                 for line1, line2 in zip(f1, f2):
                     self.assertEqual(line1, line2)
 
+    def test_WriteDescriptorDataToNPY(self):
+        '''Test that the writeDescriptorsToNPY() method writes the correct data to a NPY file and that the file is
+        consistent with the reference output. It does that with both anonymous structures it enumerates and labeled
+        structures based on the c.inputFileNames list.
+        '''
+        with resources.files('pysipfenn').joinpath('tests/testCaseFiles/exampleInputFiles') as exampleInputsDir:
+            exampleInputFiles = natsorted(os.listdir(exampleInputsDir))[:4]
+            testStructures = [Structure.from_file(f'{exampleInputsDir}/{eif}') for eif in exampleInputFiles]
+            self.c.calculate_KS2022(structList=testStructures, mode='serial')
+
+        self.c.writeDescriptorsToNPY(descriptor='KS2022',
+                                    file='TestFile_DescriptorData_4_KS2022_labeled_enumerated.npy')
+
+        loaded_data = np.load('TestFile_DescriptorData_4_KS2022_labeled_enumerated.npy')
+        np.testing.assert_array_equal(loaded_data, self.c.descriptorData)
+
+        self.c.inputFiles = ['myStructure1.POSCAR', 'myStructure2.POSCAR', 'myStructure3.POSCAR', 'myStructure4.POSCAR']
+
+        for file in ['TestFile_DescriptorData_4_KS2022_labeled_named.npy', 'descriptorData.npy']:
+            self.c.writeDescriptorsToNPY(descriptor='KS2022', file=file)
+
+            if file == 'descriptorData.npy':
+                loaded_data = np.load('KS2022_' + file)
+            else:
+                loaded_data = np.load(file)
+
+            np.testing.assert_array_equal(loaded_data, self.c.descriptorData)
+
     def test_CalculatorPrint(self):
         '''Test that the Calculator.__str__() method returns the correctly formatted string after being initialized
         but before predictions.
         '''
         printOut = str(self.c)
         self.assertIn('pySIPFENN Calculator Object', printOut)
         self.assertIn('Models are located', printOut)
```

### Comparing `pysipfenn-0.15.1/pysipfenn.egg-info/PKG-INFO` & `pysipfenn-0.16.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysipfenn
-Version: 0.15.1
-Summary: Easily extensible Python package for featurizing periodic atomic structures and running Structure-Informed Prediction of Formation Energy using Neural Networks (SIPFENN)
+Version: 0.16.0
+Summary: Python toolset for Structure-Informed Property and Feature Engineering with Neural Networks. It offers unique advantages through (1) effortless extensibility, (2) optimizations for ordered, dilute, and random atomic configurations, and (3) automated model tuning.
 Author-email: Adam Krajewski <ak@psu.edu>, Jonathan Siegel <jwsiegel@tamu.edu>
-Project-URL: Research Page, https://phaseslab.com/sipfenn
+Project-URL: Repository, https://git.pysipfenn.org
 Project-URL: Homepage, https://pysipfenn.org
 Project-URL: Bug Tracker, https://github.com/PhasesResearchLab/pySIPFENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
@@ -27,22 +27,24 @@
 Requires-Dist: onnx2torch>=1.5.2
 Requires-Dist: onnx>=1.13.0
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: natsort>=8.3.0
 Requires-Dist: pymongo>=4.4
 Requires-Dist: pysmartdl2>=2.0.0
+Requires-Dist: plotly>=5.15.0
 Requires-Dist: dnspython
 Requires-Dist: ruamel.yaml
 Requires-Dist: colorama
 Provides-Extra: dev
 Requires-Dist: coremltools>=7.0; extra == "dev"
 Requires-Dist: onnxconverter_common>=1.14.0; extra == "dev"
 Requires-Dist: onnxsim==0.4.33; extra == "dev"
 Requires-Dist: onnxruntime>=1.16.0; extra == "dev"
+Requires-Dist: optimade[http_client]>=1.0.0; extra == "dev"
 
 # pySIPFENN
 [![GitHub top language](https://img.shields.io/github/languages/top/PhasesResearchLab/pysipfenn)](https://github.com/PhasesResearchLab/pySIPFENN)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pysipfenn)](https://pypi.org/project/pysipfenn)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![PyPI - Version](https://img.shields.io/pypi/v/pysipfenn?label=PyPI&color=green)](https://pypi.org/project/pysipfenn)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pysipfenn)](https://pypi.org/project/pysipfenn)
@@ -52,50 +54,61 @@
 [![Core Mac Intel](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/coreTests_MacIntel.yaml/badge.svg)](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/coreTests_MacIntel.yaml)
 [![Core Windows](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/coreTests_Windows.yaml/badge.svg)](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/coreTests_Windows.yaml)
 [![Full Test](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/fullTest.yaml/badge.svg)](https://github.com/PhasesResearchLab/pySIPFENN/actions/workflows/fullTest.yaml)
 [![codecov](https://codecov.io/gh/PhasesResearchLab/pySIPFENN/branch/main/graph/badge.svg?token=S2J0KR0WKQ)](https://codecov.io/gh/PhasesResearchLab/pySIPFENN)
 
 [![stable](https://img.shields.io/badge/Read%20The%20Docs-Stable-green)](https://pysipfenn.readthedocs.io/en/stable/) 
 [![latest](https://img.shields.io/badge/Read%20The%20Docs-Latest-green)](https://pysipfenn.readthedocs.io/en/latest/)
+[![Static Badge](https://img.shields.io/badge/First%20MGF%20Workshop%20Video%20-%20March%202023%20(v0.10.3)-rev?logo=YouTube&color=green)](https://youtube.com/watch?v=OHgkRuE0UQM)
+
+
 [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.commatsci.2022.111254-blue)](https://doi.org/10.1016/j.commatsci.2022.111254)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7373089.svg)](https://doi.org/10.5281/zenodo.7373089)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4006802.svg)](https://doi.org/10.5281/zenodo.4006802)
+[![Arxiv](https://img.shields.io/badge/arXiv-2404.02849-8F1515?style=flat&logo=arxiv&logoColor=red)](https://doi.org/10.48550/arXiv.2404.02849)
 
 ## Summary
 
 This repository contains 
-**py**(**S**tructure-**I**nformed **P**rediction of 
-**F**ormation **E**nergy using **N**eural **N**etworks) software 
-package allowing efficient predictions of the energetics of 
-atomic configurations. The underlying methodology and implementation
-is given in
+**py**thon toolset for **S**tructure-**I**nformed **P**roperty and **F**eature **E**ngineering with **N**eural **N**etworks 
+which implements a numer of user-friendly tools for:
+- **Calculating different vector representations of atomic structures** for a number of applications including supervised (e.g., predictive machine learning models) and unsupervised learning (e.g., clustering of atomic structures based on similarity or performing anomaly detection). Notably, utilize crystallographic information and some other techniques to make this process very efficient for the vast majority of use cases (see [arXiv:2404.02849](https://arxiv.org/abs/2404.02849))
+- **Efficient deployment of pre-trained ML models** (not limited to neural networks) obtained from repositories like Zenodo (including [some we trained](https://doi.org/10.5281/zenodo.4006802)) or trained locally on user's machine. The system is very plug-and-play thanks to using Open Neural Network Exchange (ONNX) format which can be exported from nearly any machine learning framework.
+- **Tuning pre-trained ML models to new domains**, like new chemical compositions, different ab initio functional, or entirely new properties. Since V0.16, users can take advantage of integration with [OPTIMADE API](https://www.optimade.org) which allows one to tune models based on DFT datasets like Materials Project, OQMD, AFLOW, or NIST-JARVIS, in **just 3 lines of code** specifying which provider to use, what to query for, and hyperparameters for tuning.
+
+The underlying methodology, efficiency optimizations, design choices, and implementation specifics are given in the following publications:
+
+- Adam M. Krajewski, Jonathan W. Siegel, Zi-Kui Liu, _Efficient Structure-Informed Featurization and Property Prediction of Ordered, Dilute, and Random Atomic Structures_, April 2024, [arXiv:2404.02849](https://arxiv.org/abs/2404.02849)
 
 - Adam M. Krajewski, Jonathan W. Siegel, Jinchao Xu, Zi-Kui Liu, _Extensible Structure-Informed Prediction of Formation Energy with improved accuracy and usability employing neural networks_, Computational Materials Science, Volume 208, 2022, 111254, DOI:[10.1016/j.commatsci.2022.111254](https://doi.org/10.1016/j.commatsci.2022.111254)
 
-While functionalities are similar to the software released along the 
-paper, this package contains improved methods for featurizing atomic 
-configurations. Notably, all of them are now written completely in 
-Python, removing reliance on Java and making extensions of the software
-much easier thanks to improved readability. A fuller description of capabilities is 
-given in documentation at https://pysipfenn.org and at PSU Phases 
-Research Lab webpage under https://phaseslab.com/sipfenn.
+A more complete (and verbose) description of capabilities is 
+given in documentation at [(pysipfenn.org)](https://pysipfenn.org). You may also consider visiting our 
+Phases Research Lab website at [(phaseslab.org)](https://phaseslab.org).
+
+### Recent News:
 
-### Major News:
+- **(v0.16.0)** Three exciting news! (1) The all new [`ModelAdjusters`](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/core/modelAdjusters.py) submodule automates tuning and can fetch data directly from [`OPTIMADE API`](https://www.optimade.org); (2) A new manuscript detailing advantages of our featurization tools has been put on [arXiv:2404.02849](https://arxiv.org/abs/2404.02849); and (3) the name of the software was updated to **py**thon toolset for **S**tructure-**I**nformed **P**roperty and **F**eature **E**ngineering with **N**eural **N**etworks to retain the `pySIPFENN` acronym but better reflect our strengths and development direction.
 
-- **(v0.15.0)** A new descriptor (feature vector) calculator [**`descriptorDefinitions.KS2022_randomSolutions`**](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py) has been implemented. It is used for structure informed featurization of compositions randomly occupying a lattice, spiritually similar to SQS generation, but also taking into account (1) chemical differences between elements and (2) structural effects. A full description will be given in the upcoming manuscript.
+- **(v0.15.0)** A new descriptor (feature vector) calculator [**`KS2022_randomSolutions`**](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py) has been implemented. It is used for structure-informed featurization of compositions randomly occupying a lattice, spiritually similar to SQS generation, but also taking into account (1) chemical differences between elements and (2) structural effects. 
 
-- **(v0.14.0)** Users can now take advantage of a **Prototype Library** to obtain common structures from any `Calculator` instance `c` with a simple `c.prototypeLibrary['BCC']['structure']`. It can be easily [updated](https://pysipfenn.readthedocs.io/en/latest/source/pysipfenn.core.html#pysipfenn.Calculator.parsePrototypeLibrary) or [appended](https://pysipfenn.readthedocs.io/en/latest/source/pysipfenn.core.html#pysipfenn.Calculator.appendPrototypeLibrary) with high-level API or by manually modifyig its YAML [here](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/misc/prototypeLibrary.yaml).
+- **(v0.14.0)** Users can now take advantage of a **Prototype Library** to obtain common structures from any `Calculator` instance with `c.prototypeLibrary[<name>]['structure']`. It can be easily [updated](https://pysipfenn.readthedocs.io/en/latest/source/pysipfenn.core.html#pysipfenn.Calculator.parsePrototypeLibrary) or [appended](https://pysipfenn.readthedocs.io/en/latest/source/pysipfenn.core.html#pysipfenn.Calculator.appendPrototypeLibrary) with high-level API or by manually modifyig its YAML [here](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/misc/prototypeLibrary.yaml).
 
 - **(v0.13.0)** Model exports (and more!) to PyTorch, CoreML, and ONNX are now effortless thanks to [**`core.modelExporters`**](https://github.com/PhasesResearchLab/pySIPFENN/blob/main/pysipfenn/core/modelExporters.py) module. Please note you need to install pySIPFENN with `dev` option (e.g., `pip install "pysipfenn[dev]"`) to use it. See [docs here](https://pysipfenn.readthedocs.io/en/stable/source/pysipfenn.core.html#module-pysipfenn.core.modelExporters).
 
-- **(v0.12.2)** Swith to LGPLv3 allowing for integration with proprietary software developed by CALPHAD community, while supporting the development of new pySIPFENN features for all. Many thanks to our colleagues from 
-[GTT-Technologies](https://gtt-technologies.de) and other participants of [CALPHAD 2023](https://calphad.org/calphad-2023) for fruitful discussions.
+- **(v0.12.2)** Swith to LGPLv3 allowing for integration with proprietary software developed by CALPHAD community, while supporting the development of new pySIPFENN features for all.
 
-- **(March 2023 Workshop)** We would like to thank all of our amazing attendees for making our workshop, co-organized with the
-[Materials Genome Foundation](https://materialsgenomefoundation.org), such a success! Over 100 of you simultaneously followed
-all exercises and, at the peak, we loaded over 1,200GB of models into the HPC's RAM. 
+- **(March 2023 Workshop)** We would like to thank all 100 of our amazing attendees for making our workshop, co-organized with the
+[Materials Genome Foundation](https://materialsgenomefoundation.org).
+
+### Main Schematic
+
+The figure below is the main schematic of `pySIPFENN` framework detailing the interplay of internal components. The user interface provides a high-level API to process structural data within `core.Calculator`, pass it to featurization submodules in `descriptorDefinitions` to obtain vector representation, then passed to models defined in `models.json` and (typically) run automatically through all available models. All internal data of `core.Calculator` is accessible directly, enabling rapid customization. An auxiliary high-level API enables advanced users to operate and retrain the models.
+
+<img src="https://raw.githubusercontent.com/PhasesResearchLab/pySIPFENN/main/docs/_static/pySIPFENN_MainSchematic.png" alt="Main Schematic Figure" width="800" style="display: block; margin-left: auto; margin-right: auto;"/>
+   
 
 ### Applications
 
 pySIPFENN is a very flexible tool that can, in principle, be used for
 the prediction of any property of interest that depends on an atomic
 configuration with very few modifications. The models shipped by
 default are trained to predict formation energy because that is what our
@@ -229,13 +242,15 @@
 
 
 
 ## Cite
 
 If you use `pySIPFENN` software, please consider citing:
 
+- Adam M. Krajewski, Jonathan W. Siegel, Zi-Kui Liu, _Efficient Structure-Informed Featurization and Property Prediction of Ordered, Dilute, and Random Atomic Structures_, April 2024, [arXiv:2404.02849](https://arxiv.org/abs/2404.02849)
+
 - Adam M. Krajewski, Jonathan W. Siegel, Jinchao Xu, Zi-Kui Liu, _Extensible Structure-Informed Prediction of Formation Energy with improved accuracy and usability employing neural networks_, Computational Materials Science, Volume 208, 2022, 111254, DOI:[10.1016/j.commatsci.2022.111254](https://doi.org/10.1016/j.commatsci.2022.111254)
 
 If you are using predictions from pySIPFENN models accessed through `OPTIMADE` from `MPDD`, please additionally cite:
 
 - Matthew L. Evans, Johan Bergsma, ..., Adam M. Krajewski, ..., Zi-Kui Liu, ..., et al., _Developments and applications of the OPTIMADE API for materials discovery, design, and data exchange_, 2024, [arXiv:2402.00572](https://arxiv.org/abs/2402.00572)
```

### Comparing `pysipfenn-0.15.1/pysipfenn.egg-info/SOURCES.txt` & `pysipfenn-0.16.0/pysipfenn.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pysipfenn/__init__.py
 pysipfenn.egg-info/PKG-INFO
 pysipfenn.egg-info/SOURCES.txt
 pysipfenn.egg-info/dependency_links.txt
 pysipfenn.egg-info/requires.txt
 pysipfenn.egg-info/top_level.txt
 pysipfenn/core/__init__.py
+pysipfenn/core/modelAdjusters.py
 pysipfenn/core/modelExporters.py
 pysipfenn/core/pysipfenn.py
 pysipfenn/descriptorDefinitions/KS2022.py
 pysipfenn/descriptorDefinitions/KS2022_dilute.py
 pysipfenn/descriptorDefinitions/KS2022_randomSolutions.py
 pysipfenn/descriptorDefinitions/README.md
 pysipfenn/descriptorDefinitions/Ward2017.py
@@ -44,18 +45,23 @@
 pysipfenn/tests/__init__.py
 pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py
 pysipfenn/tests/test_Core_prototypeLibrary.py
 pysipfenn/tests/test_KS2022.py
 pysipfenn/tests/test_KS2022_dilute.py
 pysipfenn/tests/test_KS2022_randomSolutions.py
 pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py
+pysipfenn/tests/test_ModelAdjusters.py
 pysipfenn/tests/test_ModelExporters.py
 pysipfenn/tests/test_Ward2017.py
 pysipfenn/tests/test_customModel.py
 pysipfenn/tests/test_pysipfenn.py
+pysipfenn/tests/testCaseFiles/AdjusterTestDescriptors.csv
+pysipfenn/tests/testCaseFiles/AdjusterTestDescriptors.npy
+pysipfenn/tests/testCaseFiles/AdjusterTestTargets.csv
+pysipfenn/tests/testCaseFiles/AdjusterTestTargets.npy
 pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv
 pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv
 pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_KS2022_randomSolution_valueRangesMeans.csv
 pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv
 pysipfenn/tests/testCaseFiles/prototypeLibrary-custom.yaml
 pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR
```

