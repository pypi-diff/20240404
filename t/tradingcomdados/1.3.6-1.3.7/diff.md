# Comparing `tmp/tradingcomdados-1.3.6.tar.gz` & `tmp/tradingcomdados-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.3.6.tar", last modified: Mon Apr  1 14:26:36 2024, max compression
+gzip compressed data, was "tradingcomdados-1.3.7.tar", last modified: Wed Apr  3 23:05:07 2024, max compression
```

## Comparing `tradingcomdados-1.3.6.tar` & `tradingcomdados-1.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 14:26:36.127859 tradingcomdados-1.3.6/
--rw-rw-rw-   0        0        0     2779 2024-04-01 14:26:36.124855 tradingcomdados-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2375 2024-03-20 00:11:50.000000 tradingcomdados-1.3.6/README.md
--rw-rw-rw-   0        0        0      452 2024-04-01 14:26:29.000000 tradingcomdados-1.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 14:26:36.128855 tradingcomdados-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 14:26:36.112854 tradingcomdados-1.3.6/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.3.6/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0     4912 2024-04-01 14:25:36.000000 tradingcomdados-1.3.6/tradingcomdados/alternative_data.py
--rw-rw-rw-   0        0        0    16846 2024-03-22 13:38:14.000000 tradingcomdados-1.3.6/tradingcomdados/data_provider.py
--rw-rw-rw-   0        0        0     4470 2024-03-20 00:11:50.000000 tradingcomdados-1.3.6/tradingcomdados/funds_data.py
--rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.3.6/tradingcomdados/portfolio.py
--rw-rw-rw-   0        0        0     8924 2024-03-20 00:11:50.000000 tradingcomdados-1.3.6/tradingcomdados/supervised_learning.py
--rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.3.6/tradingcomdados/ta_indicators.py
--rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.3.6/tradingcomdados/unsupervised_learning.py
-drwxrwxrwx   0        0        0        0 2024-04-01 14:26:36.122854 tradingcomdados-1.3.6/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0     2779 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-01 14:26:35.000000 tradingcomdados-1.3.6/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 23:05:07.507219 tradingcomdados-1.3.7/
+-rw-rw-rw-   0        0        0     2779 2024-04-03 23:05:07.506220 tradingcomdados-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2375 2024-03-20 00:11:50.000000 tradingcomdados-1.3.7/README.md
+-rw-rw-rw-   0        0        0      452 2024-04-03 23:04:32.000000 tradingcomdados-1.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 23:05:07.507219 tradingcomdados-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:05:07.474219 tradingcomdados-1.3.7/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.3.7/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0     4912 2024-04-01 14:25:36.000000 tradingcomdados-1.3.7/tradingcomdados/alternative_data.py
+-rw-rw-rw-   0        0        0    16846 2024-03-22 13:38:14.000000 tradingcomdados-1.3.7/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0     4470 2024-03-20 00:11:50.000000 tradingcomdados-1.3.7/tradingcomdados/funds_data.py
+-rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.3.7/tradingcomdados/portfolio.py
+-rw-rw-rw-   0        0        0     8924 2024-03-20 00:11:50.000000 tradingcomdados-1.3.7/tradingcomdados/supervised_learning.py
+-rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.3.7/tradingcomdados/ta_indicators.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.3.7/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:05:07.506220 tradingcomdados-1.3.7/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     2779 2024-04-03 23:05:05.000000 tradingcomdados-1.3.7/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2024-04-03 23:05:05.000000 tradingcomdados-1.3.7/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 23:05:05.000000 tradingcomdados-1.3.7/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-04-03 23:05:05.000000 tradingcomdados-1.3.7/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 23:05:05.000000 tradingcomdados-1.3.7/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.3.6/PKG-INFO` & `tradingcomdados-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.3.6
+Version: 1.3.7
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 Description-Content-Type: text/markdown
-Requires-Dist: pandas==1.5.3
-Requires-Dist: requests==2.27.1
+Requires-Dist: pandas==2.0.3
+Requires-Dist: requests==2.31.0
 Requires-Dist: requests-oauthlib==1.3.1
 Requires-Dist: requests-unixsocket==0.2.0
 Requires-Dist: numpy==1.25.2
 Requires-Dist: joblib==1.1.1
-Requires-Dist: scikit-learn==1.2.1
+Requires-Dist: scikit-learn==1.2.2
 
 # tradingcomdados
 
 ## Introduction
 *Trading com Dados Library for quantitative finance*
 
 The library consists of a collection of methods that can be used in order to help Data Scientists, Quantitative Analysts and data professionals during the development of quantitative finance applications. One of the main objectives of the library is to provide methods to connect to Trading com dados' data provider services.
```

### Comparing `tradingcomdados-1.3.6/README.md` & `tradingcomdados-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/setup.py` & `tradingcomdados-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/tradingcomdados/alternative_data.py` & `tradingcomdados-1.3.7/tradingcomdados/alternative_data.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/tradingcomdados/data_provider.py` & `tradingcomdados-1.3.7/tradingcomdados/data_provider.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/tradingcomdados/funds_data.py` & `tradingcomdados-1.3.7/tradingcomdados/funds_data.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/tradingcomdados/portfolio.py` & `tradingcomdados-1.3.7/tradingcomdados/portfolio.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/tradingcomdados/supervised_learning.py` & `tradingcomdados-1.3.7/tradingcomdados/supervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/tradingcomdados/ta_indicators.py` & `tradingcomdados-1.3.7/tradingcomdados/ta_indicators.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/tradingcomdados/unsupervised_learning.py` & `tradingcomdados-1.3.7/tradingcomdados/unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.3.6/tradingcomdados.egg-info/PKG-INFO` & `tradingcomdados-1.3.7/tradingcomdados.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.3.6
+Version: 1.3.7
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 Description-Content-Type: text/markdown
-Requires-Dist: pandas==1.5.3
-Requires-Dist: requests==2.27.1
+Requires-Dist: pandas==2.0.3
+Requires-Dist: requests==2.31.0
 Requires-Dist: requests-oauthlib==1.3.1
 Requires-Dist: requests-unixsocket==0.2.0
 Requires-Dist: numpy==1.25.2
 Requires-Dist: joblib==1.1.1
-Requires-Dist: scikit-learn==1.2.1
+Requires-Dist: scikit-learn==1.2.2
 
 # tradingcomdados
 
 ## Introduction
 *Trading com Dados Library for quantitative finance*
 
 The library consists of a collection of methods that can be used in order to help Data Scientists, Quantitative Analysts and data professionals during the development of quantitative finance applications. One of the main objectives of the library is to provide methods to connect to Trading com dados' data provider services.
```

