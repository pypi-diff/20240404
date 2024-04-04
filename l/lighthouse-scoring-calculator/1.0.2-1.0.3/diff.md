# Comparing `tmp/lighthouse-scoring-calculator-1.0.2.tar.gz` & `tmp/lighthouse-scoring-calculator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lighthouse-scoring-calculator-1.0.2.tar", last modified: Sun Oct  2 12:16:08 2022, max compression
+gzip compressed data, was "lighthouse-scoring-calculator-1.0.3.tar", last modified: Thu Apr  4 17:25:36 2024, max compression
```

## Comparing `lighthouse-scoring-calculator-1.0.2.tar` & `lighthouse-scoring-calculator-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2022-10-02 12:16:08.401299 lighthouse-scoring-calculator-1.0.2/
--rw-r--r--   0 fabio      (501) staff       (20)    35149 2022-10-02 09:28:19.000000 lighthouse-scoring-calculator-1.0.2/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)    43919 2022-10-02 12:16:08.400931 lighthouse-scoring-calculator-1.0.2/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     2627 2022-10-02 10:23:10.000000 lighthouse-scoring-calculator-1.0.2/README.md
--rw-r--r--   0 fabio      (501) staff       (20)      924 2022-10-02 12:15:36.000000 lighthouse-scoring-calculator-1.0.2/pyproject.toml
--rw-r--r--   0 fabio      (501) staff       (20)       38 2022-10-02 12:16:08.401394 lighthouse-scoring-calculator-1.0.2/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)       37 2022-10-02 10:11:24.000000 lighthouse-scoring-calculator-1.0.2/setup.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2022-10-02 12:16:08.394773 lighthouse-scoring-calculator-1.0.2/src/
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2022-10-02 12:16:08.398154 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/
--rw-r--r--   0 fabio      (501) staff       (20)      142 2022-10-02 12:15:44.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     2203 2022-10-02 09:28:39.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/__main__.py
--rw-r--r--   0 fabio      (501) staff       (20)     1886 2022-10-02 10:55:42.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/calculator.py
--rw-r--r--   0 fabio      (501) staff       (20)      383 2022-10-02 09:28:39.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/example.py
--rw-r--r--   0 fabio      (501) staff       (20)     2745 2022-10-02 09:28:39.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/metrics.py
--rw-r--r--   0 fabio      (501) staff       (20)     2001 2022-10-02 09:28:39.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/util.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2022-10-02 12:16:08.399600 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)    43919 2022-10-02 12:16:08.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      601 2022-10-02 12:16:08.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2022-10-02 12:16:08.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)       48 2022-10-02 12:16:08.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator.egg-info/entry_points.txt
--rw-r--r--   0 fabio      (501) staff       (20)       30 2022-10-02 12:16:08.000000 lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2024-04-04 17:25:36.194557 lighthouse-scoring-calculator-1.0.3/
+-rw-r--r--   0 fabio      (501) staff       (20)    35149 2022-10-02 09:28:19.000000 lighthouse-scoring-calculator-1.0.3/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)    43919 2024-04-04 17:25:36.194089 lighthouse-scoring-calculator-1.0.3/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     2627 2022-10-02 10:23:10.000000 lighthouse-scoring-calculator-1.0.3/README.md
+-rw-r--r--   0 fabio      (501) staff       (20)      924 2024-04-04 17:19:50.000000 lighthouse-scoring-calculator-1.0.3/pyproject.toml
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2024-04-04 17:25:36.194646 lighthouse-scoring-calculator-1.0.3/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)       37 2022-10-02 10:11:24.000000 lighthouse-scoring-calculator-1.0.3/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2024-04-04 17:25:36.188085 lighthouse-scoring-calculator-1.0.3/src/
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2024-04-04 17:25:36.191447 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/
+-rw-r--r--   0 fabio      (501) staff       (20)      142 2024-04-04 17:19:50.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2203 2022-10-02 09:28:39.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/__main__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     1886 2022-10-02 10:55:42.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/calculator.py
+-rw-r--r--   0 fabio      (501) staff       (20)      384 2024-04-04 17:19:50.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/example.py
+-rw-r--r--   0 fabio      (501) staff       (20)     3563 2024-04-04 17:19:50.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/metrics.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2001 2022-10-02 09:28:39.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/util.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2024-04-04 17:25:36.193493 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)    43919 2024-04-04 17:25:36.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      601 2024-04-04 17:25:36.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2024-04-04 17:25:36.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       48 2024-04-04 17:25:36.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       30 2024-04-04 17:25:36.000000 lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator.egg-info/top_level.txt
```

### Comparing `lighthouse-scoring-calculator-1.0.2/LICENSE` & `lighthouse-scoring-calculator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lighthouse-scoring-calculator-1.0.2/PKG-INFO` & `lighthouse-scoring-calculator-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighthouse-scoring-calculator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Calculate the Lighthouse scoring for a website
 Author-email: Fabio Manz <fabio.manz@t-online.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `lighthouse-scoring-calculator-1.0.2/README.md` & `lighthouse-scoring-calculator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lighthouse-scoring-calculator-1.0.2/pyproject.toml` & `lighthouse-scoring-calculator-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lighthouse-scoring-calculator"
-version = "1.0.2"
+version = "1.0.3"
 description = "Calculate the Lighthouse scoring for a website"
 readme = "README.md"
 authors = [{ name = "Fabio Manz", email = "fabio.manz@t-online.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/__main__.py` & `lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/__main__.py`

 * *Files identical despite different names*

### Comparing `lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/calculator.py` & `lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/metrics.py` & `lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,32 @@
     "TTI": {"auditId": 'interactive', "name": 'Time to Interactive'},
     "TBT": {"auditId": 'total-blocking-time', "name": 'Total Blocking Time'},
     "CLS": {"auditId": 'cumulative-layout-shift', "name": 'Cumulative Layout Shift', "units": 'unitless'},
     "FMP": {"auditId": 'first-meaningful-paint', "name": 'First Meaningful Paint'},
     "FCI": {"auditId": 'first-cpu-idle', "name": 'First CPU Idle'},
 }
 
+# curves obtained from https://googlechrome.github.io/lighthouse/scorecalc/calc.js
 curves = {
+    "v10": {
+        "mobile": {
+            "FCP": {"weight": 0.10, "median": 3000, "p10": 1800},
+            "SI": {"weight": 0.10, "median": 5800, "p10": 3387},
+            "LCP": {"weight": 0.25, "median": 4000, "p10": 2500},
+            "TBT": {"weight": 0.30, "median": 600,  "p10": 200},
+            "CLS": {"weight": 0.25, "median": 0.25, "p10": 0.1},
+        },
+        "desktop": {
+            "FCP": {"weight": 0.10, "median": 1600, "p10": 934},
+            "SI": {"weight": 0.10, "median": 2300, "p10": 1311},
+            "LCP": {"weight": 0.25, "median": 2400, "p10": 1200},
+            "TBT": {"weight": 0.30, "median": 350, "p10": 150},
+            "CLS": {"weight": 0.25, "median": 0.25, "p10": 0.1},
+        },
+    },
     "v8": {
         "mobile": {
             "FCP": {"weight": 0.10, "median": 3000, "p10": 1800},
             "SI": {"weight": 0.10, "median": 5800, "p10": 3387},
             "LCP": {"weight": 0.25, "median": 4000, "p10": 2500},
             "TTI": {"weight": 0.10, "median": 7300, "p10": 3785},
             "TBT": {"weight": 0.30, "median": 600,  "p10": 200},
```

### Comparing `lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator/util.py` & `lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator/util.py`

 * *Files identical despite different names*

### Comparing `lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator.egg-info/PKG-INFO` & `lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighthouse-scoring-calculator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Calculate the Lighthouse scoring for a website
 Author-email: Fabio Manz <fabio.manz@t-online.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `lighthouse-scoring-calculator-1.0.2/src/lighthouse_scoring_calculator.egg-info/SOURCES.txt` & `lighthouse-scoring-calculator-1.0.3/src/lighthouse_scoring_calculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

