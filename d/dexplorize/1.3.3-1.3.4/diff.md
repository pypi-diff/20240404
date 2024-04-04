# Comparing `tmp/dexplorize-1.3.3.tar.gz` & `tmp/dexplorize-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexplorize-1.3.3.tar", last modified: Fri Mar 29 05:31:09 2024, max compression
+gzip compressed data, was "dexplorize-1.3.4.tar", last modified: Thu Apr  4 09:43:00 2024, max compression
```

## Comparing `dexplorize-1.3.3.tar` & `dexplorize-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwx------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-03-29 05:31:08.986466 dexplorize-1.3.3/
-drwx------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-03-29 05:31:08.978466 dexplorize-1.3.3/DataExploration/
--rw-------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-03-29 05:30:05.000000 dexplorize-1.3.3/DataExploration/__init__.py
--rw-------   0 u0_a225  (10225) u0_a225  (10225)     1567 2024-03-29 05:30:05.000000 dexplorize-1.3.3/DataExploration/bivariate.py
--rw-------   0 u0_a225  (10225) u0_a225  (10225)     5512 2024-03-29 05:30:05.000000 dexplorize-1.3.3/DataExploration/univariate.py
--rw-------   0 u0_a225  (10225) u0_a225  (10225)     1079 2024-03-29 05:30:05.000000 dexplorize-1.3.3/LICENSE
--rw-r--r--   0 u0_a225  (10225) u0_a225  (10225)     2643 2024-03-29 05:31:08.986466 dexplorize-1.3.3/PKG-INFO
--rw-------   0 u0_a225  (10225) u0_a225  (10225)     1933 2024-03-29 05:30:05.000000 dexplorize-1.3.3/README.md
-drwx------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-03-29 05:31:08.986466 dexplorize-1.3.3/dexplorize.egg-info/
--rw-r--r--   0 u0_a225  (10225) u0_a225  (10225)     2643 2024-03-29 05:31:08.000000 dexplorize-1.3.3/dexplorize.egg-info/PKG-INFO
--rw-------   0 u0_a225  (10225) u0_a225  (10225)      347 2024-03-29 05:31:08.000000 dexplorize-1.3.3/dexplorize.egg-info/SOURCES.txt
--rw-------   0 u0_a225  (10225) u0_a225  (10225)        1 2024-03-29 05:31:08.000000 dexplorize-1.3.3/dexplorize.egg-info/dependency_links.txt
--rw-------   0 u0_a225  (10225) u0_a225  (10225)       66 2024-03-29 05:31:08.000000 dexplorize-1.3.3/dexplorize.egg-info/entry_points.txt
--rw-------   0 u0_a225  (10225) u0_a225  (10225)       46 2024-03-29 05:31:08.000000 dexplorize-1.3.3/dexplorize.egg-info/requires.txt
--rw-------   0 u0_a225  (10225) u0_a225  (10225)       22 2024-03-29 05:31:08.000000 dexplorize-1.3.3/dexplorize.egg-info/top_level.txt
--rw-------   0 u0_a225  (10225) u0_a225  (10225)      485 2024-03-29 05:31:08.986466 dexplorize-1.3.3/setup.cfg
--rw-------   0 u0_a225  (10225) u0_a225  (10225)     1086 2024-03-29 05:30:05.000000 dexplorize-1.3.3/setup.py
-drwx------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-03-29 05:31:08.982466 dexplorize-1.3.3/tests/
--rw-------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-03-29 05:30:05.000000 dexplorize-1.3.3/tests/__init__.py
+drwx------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-04-04 09:43:00.244196 dexplorize-1.3.4/
+drwx------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-04-04 09:43:00.236195 dexplorize-1.3.4/DataExploration/
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-04-04 09:41:17.000000 dexplorize-1.3.4/DataExploration/__init__.py
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)     1567 2024-04-04 09:41:17.000000 dexplorize-1.3.4/DataExploration/bivariate.py
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)     5475 2024-04-04 09:41:17.000000 dexplorize-1.3.4/DataExploration/univariate.py
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)     1079 2024-04-04 09:41:17.000000 dexplorize-1.3.4/LICENSE
+-rw-r--r--   0 u0_a225  (10225) u0_a225  (10225)     2626 2024-04-04 09:43:00.244196 dexplorize-1.3.4/PKG-INFO
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)     1916 2024-04-04 09:41:17.000000 dexplorize-1.3.4/README.md
+drwx------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-04-04 09:43:00.240196 dexplorize-1.3.4/dexplorize.egg-info/
+-rw-r--r--   0 u0_a225  (10225) u0_a225  (10225)     2626 2024-04-04 09:43:00.000000 dexplorize-1.3.4/dexplorize.egg-info/PKG-INFO
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)      347 2024-04-04 09:43:00.000000 dexplorize-1.3.4/dexplorize.egg-info/SOURCES.txt
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)        1 2024-04-04 09:43:00.000000 dexplorize-1.3.4/dexplorize.egg-info/dependency_links.txt
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)       66 2024-04-04 09:43:00.000000 dexplorize-1.3.4/dexplorize.egg-info/entry_points.txt
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)       46 2024-04-04 09:43:00.000000 dexplorize-1.3.4/dexplorize.egg-info/requires.txt
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)       22 2024-04-04 09:43:00.000000 dexplorize-1.3.4/dexplorize.egg-info/top_level.txt
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)      485 2024-04-04 09:43:00.244196 dexplorize-1.3.4/setup.cfg
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)     1086 2024-04-04 09:41:17.000000 dexplorize-1.3.4/setup.py
+drwx------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-04-04 09:43:00.240196 dexplorize-1.3.4/tests/
+-rw-------   0 u0_a225  (10225) u0_a225  (10225)        0 2024-04-04 09:41:17.000000 dexplorize-1.3.4/tests/__init__.py
```

### Comparing `dexplorize-1.3.3/DataExploration/bivariate.py` & `dexplorize-1.3.4/DataExploration/bivariate.py`

 * *Files identical despite different names*

### Comparing `dexplorize-1.3.3/DataExploration/univariate.py` & `dexplorize-1.3.4/DataExploration/univariate.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,20 @@
     attr1 = np.where(attr1 <= BS, np.nan, attr1)
     
   return splits, info_gain
 
 
 def entropy_based(data1, target, bins):
   splits, info_gain = entropy(data1, target, bins)
-  print(f'Entropy: {compute_entropy(target):.3f}') 
-  print(f'Entropy given best split: {min(info_gain):.3f}')
-  print(f'Information gain: {max(info_gain):.3f}')
+  entr = compute_entropy(target)
+  gain = max(info_gain)
+  split_val = entr - gain
+  print(f'Entropy: {entr:.3f}') 
+  print(f'Entropy given best split: {split_val:.3f}')
+  print(f'Information gain: {gain:.3f}')
   print(f'Best split bins <= {min(splits):.3f} and > {max(splits):.3f}')
 
 # Equal Width Based - Unsupervised
 def equal_width(data, bins):
     width = (max(data) - min(data)) / bins
     boundaries = [min(data) + x * width for x in range(1, bins)]
     bin = np.split(np.sort(data), np.searchsorted(np.sort(data), boundaries))
@@ -141,49 +144,45 @@
   value_count.plot(kind='bar')
   plt.xlabel('Categories')
   plt.ylabel('Counts')
   plt.title('Bar Chart')
   plt.show()
 
 # Numerical Variables
-def stat_one(data):
+def describe(data):
   minimum = min(data)
   maximum = max(data)
   means = sum(data) / len(data)
   
   sort_data = sorted(data)
   length = len(data)
   if length % 2 == 0:
     medians = (sort_data[length // 2 - 1] + sort_data[length // 2]) / 2
   else:
     medians = sort_data[length // 2]
   
   freq = {}
   for x in data:
     freq[x] = freq.get(x, 0) + 1
+    
   modes = max(freq, key=freq.get)
-  
-  print('-'*30)
-  print('Statistical Measure 1')
-  print('-'*30)
-  print(f'Min:     {minimum}')
-  print(f'Max:     {maximum}')
-  print(f'Mean:    {means}')
-  print(f'Median:  {medians}')
-  print(f'Mode:    {modes}')
-  print('-'*30)
-
-def stat_two(data):
   data_range = np.ptp(data)
   data_qntles = np.percentile(data, [25, 50, 75])
   data_var = np.var(data)
   data_std = np.std(data)
   data_cov = (data_std / np.mean(data)) * 100
+
+  print('-'*40)
+  print('Statistical Measure')
   print('-'*40)
-  print('Statistical Measure 2')
+  print(f'Min:     {minimum}')
+  print(f'Max:     {maximum}')
+  print(f'Mean:    {means}')
+  print(f'Median:  {medians}')
+  print(f'Mode:    {modes}')
   print('-'*40)
   print(f'Range:            {data_range}')
   print(f'Quantiles:        {data_qntles}')
   print(f'Variance:         {data_var}')
   print(f'STDev:            {data_std}')
   print(f'CoVar:            {data_range}')
   print('-'*40)
```

### Comparing `dexplorize-1.3.3/LICENSE` & `dexplorize-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dexplorize-1.3.3/PKG-INFO` & `dexplorize-1.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexplorize
-Version: 1.3.3
+Version: 1.3.4
 Summary: dexplorize (data exploration) python library use for applying different foundational techniques such as univariate and bivariate analysis.
 Home-page: https://github.com/iyaniyan11/dexplorize.git
 Author: Christian Garcia
 Author-email: iyaniyan3112003@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -67,16 +67,15 @@
 - equal_freq(data, bins)
 - efreq_bin(data, bins)
 - efreq_plot(data)
 - binary_encoding(data, values)
 - target_encoding(data, values, attr)
 - impute_values(data)
 - pie_chart(data)
-- stat_one(data)
-- stat_two(data)
+- describe(data)
 - hist_bar(data, bins)
 - bar_chart(data)
 
 Bivariate Function (Data Visualization)
 - scatter_plot(data, col1, col2)
 - linear_corr(data, col1, col2)
 - stacked_column(data, col1, col2)
```

### Comparing `dexplorize-1.3.3/README.md` & `dexplorize-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,15 @@
 - equal_freq(data, bins)
 - efreq_bin(data, bins)
 - efreq_plot(data)
 - binary_encoding(data, values)
 - target_encoding(data, values, attr)
 - impute_values(data)
 - pie_chart(data)
-- stat_one(data)
-- stat_two(data)
+- describe(data)
 - hist_bar(data, bins)
 - bar_chart(data)
 
 Bivariate Function (Data Visualization)
 - scatter_plot(data, col1, col2)
 - linear_corr(data, col1, col2)
 - stacked_column(data, col1, col2)
```

### Comparing `dexplorize-1.3.3/dexplorize.egg-info/PKG-INFO` & `dexplorize-1.3.4/dexplorize.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexplorize
-Version: 1.3.3
+Version: 1.3.4
 Summary: dexplorize (data exploration) python library use for applying different foundational techniques such as univariate and bivariate analysis.
 Home-page: https://github.com/iyaniyan11/dexplorize.git
 Author: Christian Garcia
 Author-email: iyaniyan3112003@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -67,16 +67,15 @@
 - equal_freq(data, bins)
 - efreq_bin(data, bins)
 - efreq_plot(data)
 - binary_encoding(data, values)
 - target_encoding(data, values, attr)
 - impute_values(data)
 - pie_chart(data)
-- stat_one(data)
-- stat_two(data)
+- describe(data)
 - hist_bar(data, bins)
 - bar_chart(data)
 
 Bivariate Function (Data Visualization)
 - scatter_plot(data, col1, col2)
 - linear_corr(data, col1, col2)
 - stacked_column(data, col1, col2)
```

### Comparing `dexplorize-1.3.3/setup.py` & `dexplorize-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='dexplorize',
-    version='1.3.3',
+    version='1.3.4',
     packages=find_packages(),
     install_requires=[
       'matplotlib>=3.4.3',
       'numpy>=1.21.0',
       'pandas>=1.3.3'
       ],
     entry_points={
```

