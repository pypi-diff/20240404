# Comparing `tmp/PyEvALL-0.1.56.tar.gz` & `tmp/PyEvALL-0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEvALL-0.1.56.tar", last modified: Wed Apr  3 22:18:45 2024, max compression
+gzip compressed data, was "PyEvALL-0.1.60.tar", last modified: Thu Apr  4 11:03:38 2024, max compression
```

## Comparing `PyEvALL-0.1.56.tar` & `PyEvALL-0.1.60.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 22:18:45.709430 PyEvALL-0.1.56/
--rw-rw-rw-   0        0        0      447 2024-04-03 22:18:45.708432 PyEvALL-0.1.56/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 22:18:45.693428 PyEvALL-0.1.56/PyEvALL.egg-info/
--rw-rw-rw-   0        0        0      447 2024-04-03 22:18:45.000000 PyEvALL-0.1.56/PyEvALL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2024-04-03 22:18:45.000000 PyEvALL-0.1.56/PyEvALL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 22:18:45.000000 PyEvALL-0.1.56/PyEvALL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-04-03 22:18:45.000000 PyEvALL-0.1.56/PyEvALL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 22:18:45.000000 PyEvALL-0.1.56/PyEvALL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14072 2024-03-29 07:17:36.000000 PyEvALL-0.1.56/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 22:18:45.697418 PyEvALL-0.1.56/pyevall/
--rw-rw-rw-   0        0        0        0 2023-02-07 00:42:14.000000 PyEvALL-0.1.56/pyevall/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:18:45.700410 PyEvALL-0.1.56/pyevall/comparators/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:43:21.000000 PyEvALL-0.1.56/pyevall/comparators/__init__.py
--rw-rw-rw-   0        0        0    15925 2024-04-03 20:07:49.000000 PyEvALL-0.1.56/pyevall/comparators/comparators.py
--rw-rw-rw-   0        0        0    20371 2024-04-03 09:08:50.000000 PyEvALL-0.1.56/pyevall/comparators/formats.py
--rw-rw-rw-   0        0        0     9855 2024-04-03 09:08:55.000000 PyEvALL-0.1.56/pyevall/evaluation.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:18:45.702404 PyEvALL-0.1.56/pyevall/metrics/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:42:54.000000 PyEvALL-0.1.56/pyevall/metrics/__init__.py
--rw-rw-rw-   0        0        0     4187 2024-04-03 09:09:44.000000 PyEvALL-0.1.56/pyevall/metrics/metricfactory.py
--rw-rw-rw-   0        0        0    55379 2024-04-03 20:10:37.000000 PyEvALL-0.1.56/pyevall/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:18:45.704399 PyEvALL-0.1.56/pyevall/reports/
--rw-rw-rw-   0        0        0        0 2022-08-28 10:42:12.000000 PyEvALL-0.1.56/pyevall/reports/__init__.py
--rw-rw-rw-   0        0        0    26716 2024-04-03 22:02:38.000000 PyEvALL-0.1.56/pyevall/reports/reports.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:18:45.705426 PyEvALL-0.1.56/pyevall/utils/
--rw-rw-rw-   0        0        0     8000 2024-04-03 13:16:56.000000 PyEvALL-0.1.56/pyevall/utils/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-03 22:18:45.709430 PyEvALL-0.1.56/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-04-03 22:10:29.000000 PyEvALL-0.1.56/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:18:45.707428 PyEvALL-0.1.56/test/
--rw-rw-rw-   0        0        0    10405 2024-04-03 16:37:42.000000 PyEvALL-0.1.56/test/testformats.py
--rw-rw-rw-   0        0        0    11154 2024-04-03 20:01:38.000000 PyEvALL-0.1.56/test/testmetrics.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.581058 PyEvALL-0.1.60/
+-rw-rw-rw-   0        0        0       24 2024-03-13 22:18:07.000000 PyEvALL-0.1.60/MANIFEST.in
+-rw-rw-rw-   0        0        0      447 2024-04-04 11:03:38.580061 PyEvALL-0.1.60/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.530050 PyEvALL-0.1.60/PyEvALL.egg-info/
+-rw-rw-rw-   0        0        0      447 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 11:03:38.000000 PyEvALL-0.1.60/PyEvALL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25635 2024-04-04 10:56:47.000000 PyEvALL-0.1.60/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.538606 PyEvALL-0.1.60/pyevall/
+-rw-rw-rw-   0        0        0        0 2023-02-07 00:42:14.000000 PyEvALL-0.1.60/pyevall/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.555766 PyEvALL-0.1.60/pyevall/comparators/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:43:21.000000 PyEvALL-0.1.60/pyevall/comparators/__init__.py
+-rw-rw-rw-   0        0        0    15925 2024-04-03 20:07:49.000000 PyEvALL-0.1.60/pyevall/comparators/comparators.py
+-rw-rw-rw-   0        0        0    20371 2024-04-03 09:08:50.000000 PyEvALL-0.1.60/pyevall/comparators/formats.py
+-rw-rw-rw-   0        0        0     9855 2024-04-03 09:08:55.000000 PyEvALL-0.1.60/pyevall/evaluation.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.571725 PyEvALL-0.1.60/pyevall/metrics/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:42:54.000000 PyEvALL-0.1.60/pyevall/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4187 2024-04-03 09:09:44.000000 PyEvALL-0.1.60/pyevall/metrics/metricfactory.py
+-rw-rw-rw-   0        0        0    55383 2024-04-04 08:29:36.000000 PyEvALL-0.1.60/pyevall/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.572722 PyEvALL-0.1.60/pyevall/reports/
+-rw-rw-rw-   0        0        0        0 2022-08-28 10:42:12.000000 PyEvALL-0.1.60/pyevall/reports/__init__.py
+-rw-rw-rw-   0        0        0    27269 2024-04-04 10:04:56.000000 PyEvALL-0.1.60/pyevall/reports/reports.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.576323 PyEvALL-0.1.60/pyevall/utils/
+-rw-rw-rw-   0        0        0      479 2024-03-06 07:06:10.000000 PyEvALL-0.1.60/pyevall/utils/file.conf
+-rw-rw-rw-   0        0        0     2459 2024-04-04 10:28:07.000000 PyEvALL-0.1.60/pyevall/utils/pyevall_keys_texts_reports.rep
+-rw-rw-rw-   0        0        0     8000 2024-04-03 13:16:56.000000 PyEvALL-0.1.60/pyevall/utils/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 11:03:38.581058 PyEvALL-0.1.60/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-04-04 10:58:18.000000 PyEvALL-0.1.60/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 11:03:38.579061 PyEvALL-0.1.60/test/
+-rw-rw-rw-   0        0        0    10405 2024-04-03 16:37:42.000000 PyEvALL-0.1.60/test/testformats.py
+-rw-rw-rw-   0        0        0    11154 2024-04-03 20:01:38.000000 PyEvALL-0.1.60/test/testmetrics.py
```

### Comparing `PyEvALL-0.1.56/PyEvALL.egg-info/SOURCES.txt` & `PyEvALL-0.1.60/PyEvALL.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 setup.py
 PyEvALL.egg-info/PKG-INFO
 PyEvALL.egg-info/SOURCES.txt
 PyEvALL.egg-info/dependency_links.txt
 PyEvALL.egg-info/requires.txt
 PyEvALL.egg-info/top_level.txt
@@ -16,10 +17,12 @@
 pyevall/comparators/comparators.py
 pyevall/comparators/formats.py
 pyevall/metrics/__init__.py
 pyevall/metrics/metricfactory.py
 pyevall/metrics/metrics.py
 pyevall/reports/__init__.py
 pyevall/reports/reports.py
+pyevall/utils/file.conf
+pyevall/utils/pyevall_keys_texts_reports.rep
 pyevall/utils/utils.py
 test/testformats.py
 test/testmetrics.py
```

### Comparing `PyEvALL-0.1.56/pyevall/comparators/comparators.py` & `PyEvALL-0.1.60/pyevall/comparators/comparators.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.56/pyevall/comparators/formats.py` & `PyEvALL-0.1.60/pyevall/comparators/formats.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.56/pyevall/evaluation.py` & `PyEvALL-0.1.60/pyevall/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.56/pyevall/metrics/metricfactory.py` & `PyEvALL-0.1.60/pyevall/metrics/metricfactory.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.56/pyevall/metrics/metrics.py` & `PyEvALL-0.1.60/pyevall/metrics/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def fire_preconditions(self, error, test_case):
         if error==None:
             return False  
         else:
             if not error in self.preconditions:
                 precondition=dict()
                 precondition[PyEvALLReport.NAME_TAG]=error
-                precondition[PyEvALLReport.DESCRIPTION_TAG]=PyEvALLReport.COMING_SOON
+                precondition[PyEvALLReport.DESCRIPTION_TAG]=PyEvALLReport.EMBEDDED_OPTION
                 precondition[PyEvALLReport.STATUS_TAG]=PyEvALLReport.FAIL 
                 precondition[PyEvALLReport.TEST_CASES_TAG]=[]
                 self.preconditions[error]=precondition
             self.preconditions[error][PyEvALLReport.TEST_CASES_TAG].append(test_case)               
 
          
     @abstractmethod
```

### Comparing `PyEvALL-0.1.56/pyevall/reports/reports.py` & `PyEvALL-0.1.60/pyevall/reports/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -531,26 +531,40 @@
         self.report[PyEvALLMetaReport.EVALUATION_TAG + "_" + str(i)]=rep.report
         
         
         
         
 class PyEvALLMetaReportDataFrame(PyEvALLDataframeReport):             
     def add_pyevall_report(self, rep, i):  
-            if i==0:
+            if i==1:
                 df_report= PyEvALLDataframeReport(rep)
                 df_report.generate_pyevall_df_report()
                 self.df_average=df_report.df_average
                 self.df_test_case=df_report.df_test_case
                 self.df_test_case_classes= df_report.df_test_case_classes
             else:
                 df_report = PyEvALLDataframeReport(rep)
                 df_report.generate_pyevall_df_report()
-                self.df_average = pd.concat([self.df_average,df_report.df_average], ignore_index=True)
-                self.df_test_case = pd.concat([self.df_test_case,df_report.df_test_case], ignore_index=True)
-                self.df_test_case_classes = pd.concat([self.df_test_case_classes,df_report.df_test_case_classes], ignore_index=True)       
+                
+                if self.df_average is not None:
+                    self.df_average = pd.concat([self.df_average,df_report.df_average], ignore_index=True)
+                else:
+                    self.df_average=df_report.df_average
+                    
+                    
+                if self.df_test_case_classes is not None:
+                    self.df_test_case = pd.concat([self.df_test_case,df_report.df_test_case], ignore_index=True)
+                else:
+                    self.df_test_case=df_report.df_test_case
+                    
+                    
+                if self.df_test_case_classes is not None:
+                    self.df_test_case_classes = pd.concat([self.df_test_case_classes,df_report.df_test_case_classes], ignore_index=True)  
+                else:
+                    self.df_test_case_classes= df_report.df_test_case_classes
```

### Comparing `PyEvALL-0.1.56/pyevall/utils/utils.py` & `PyEvALL-0.1.60/pyevall/utils/utils.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.56/setup.py` & `PyEvALL-0.1.60/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='PyEvALL',
-    version='0.1.56',
-    description='PyEvALL (The Python library to Evaluate ALL) is a evaluation tool for information systems that allows assessing a wide range of metrics covering various evaluation contexts, including classification, ranking, or LeWeDi (Learning with disagreement).',
+    version='0.1.60',
+    description='PyEvALL (The Python library to Evaluate ALL) is a evaluation tool for information systems that allows assessing a wide range of metrics covering various evaluation contexts, including classification, ranking, or LeWiDi (Learning with disagreement).',
     author='JORGE CARRILLO-DE-ALBORNOZ',
     author_email='jcalbornoz@lsi.uned.es',
     url="https://github.com/UNEDLENAR/PyEvALL/tree/main",
     include_package_data=True,
     packages=['pyevall','pyevall.metrics','pyevall.utils',
               'pyevall.comparators','pyevall.reports'],
     install_requires=['jsbeautifier==1.14.9', 'jsonschema==4.21.1', 'numpy==1.26.4', 'pandas==2.2.1', 'setuptools==68.0.0', 'tabulate==0.9.0'
```

### Comparing `PyEvALL-0.1.56/test/testformats.py` & `PyEvALL-0.1.60/test/testformats.py`

 * *Files identical despite different names*

### Comparing `PyEvALL-0.1.56/test/testmetrics.py` & `PyEvALL-0.1.60/test/testmetrics.py`

 * *Files identical despite different names*

