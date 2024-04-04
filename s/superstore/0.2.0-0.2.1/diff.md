# Comparing `tmp/superstore-0.2.0.tar.gz` & `tmp/superstore-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superstore-0.2.0.tar", last modified: Sun Nov  5 22:19:52 2023, max compression
+gzip compressed data, was "superstore-0.2.1.tar", last modified: Thu Apr  4 21:39:58 2024, max compression
```

## Comparing `superstore-0.2.0.tar` & `superstore-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-11-05 22:19:52.517011 superstore-0.2.0/
--rw-r--r--   0 timkpaine   (501) staff       (20)      108 2023-04-12 02:10:37.000000 superstore-0.2.0/AUTHORS
--rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-12 02:10:37.000000 superstore-0.2.0/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      340 2023-04-12 02:10:37.000000 superstore-0.2.0/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     1077 2023-11-05 22:17:20.000000 superstore-0.2.0/Makefile
--rw-r--r--   0 timkpaine   (501) staff       (20)     1832 2023-11-05 22:19:52.516931 superstore-0.2.0/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      816 2023-04-12 02:10:37.000000 superstore-0.2.0/README.md
--rw-r--r--   0 timkpaine   (501) staff       (20)      137 2023-11-05 22:17:20.000000 superstore-0.2.0/pyproject.toml
--rw-r--r--   0 timkpaine   (501) staff       (20)      575 2023-11-05 22:19:52.517272 superstore-0.2.0/setup.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)     1331 2023-11-05 22:19:43.000000 superstore-0.2.0/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-11-05 22:19:52.515012 superstore-0.2.0/superstore/
--rw-r--r--   0 timkpaine   (501) staff       (20)      123 2023-11-05 22:19:43.000000 superstore-0.2.0/superstore/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2302 2023-11-05 22:17:20.000000 superstore-0.2.0/superstore/superstore.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-11-05 22:19:52.516079 superstore-0.2.0/superstore/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1293 2023-11-05 22:17:20.000000 superstore-0.2.0/superstore/tests/test_superstore.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      253 2023-11-05 22:17:20.000000 superstore-0.2.0/superstore/tests/test_vendored.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2726 2023-11-05 22:17:20.000000 superstore-0.2.0/superstore/utils.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-11-05 22:19:52.516310 superstore-0.2.0/superstore/vendored/
--rw-r--r--   0 timkpaine   (501) staff       (20)       57 2023-11-05 22:17:20.000000 superstore-0.2.0/superstore/vendored/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2608 2023-11-05 22:17:20.000000 superstore-0.2.0/superstore/vendored/timeseries.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-11-05 22:19:52.515852 superstore-0.2.0/superstore.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1832 2023-11-05 22:19:52.000000 superstore-0.2.0/superstore.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      486 2023-11-05 22:19:52.000000 superstore-0.2.0/superstore.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-11-05 22:19:52.000000 superstore-0.2.0/superstore.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-12 02:18:21.000000 superstore-0.2.0/superstore.egg-info/not-zip-safe
--rw-r--r--   0 timkpaine   (501) staff       (20)      142 2023-11-05 22:19:52.000000 superstore-0.2.0/superstore.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       11 2023-11-05 22:19:52.000000 superstore-0.2.0/superstore.egg-info/top_level.txt
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.481467 superstore-0.2.1/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      108 2023-04-12 02:10:37.000000 superstore-0.2.1/AUTHORS
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-12 02:10:37.000000 superstore-0.2.1/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      340 2023-04-12 02:10:37.000000 superstore-0.2.1/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1083 2024-04-04 21:36:47.000000 superstore-0.2.1/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1835 2024-04-04 21:39:58.481353 superstore-0.2.1/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      816 2023-04-12 02:10:37.000000 superstore-0.2.1/README.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)      141 2024-04-04 21:36:47.000000 superstore-0.2.1/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)      575 2024-04-04 21:39:58.481799 superstore-0.2.1/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1334 2024-04-04 21:39:21.000000 superstore-0.2.1/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.478916 superstore-0.2.1/superstore/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      123 2024-04-04 21:39:21.000000 superstore-0.2.1/superstore/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2302 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/superstore.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.480058 superstore-0.2.1/superstore/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1293 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/tests/test_superstore.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      253 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/tests/test_vendored.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2726 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.480359 superstore-0.2.1/superstore/vendored/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       57 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/vendored/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2601 2024-04-04 21:36:47.000000 superstore-0.2.1/superstore/vendored/timeseries.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.480581 superstore-0.2.1/superstore.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1835 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      486 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-12 02:18:21.000000 superstore-0.2.1/superstore.egg-info/not-zip-safe
+-rw-r--r--   0 timkpaine   (501) staff       (20)      145 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       11 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/top_level.txt
```

### Comparing `superstore-0.2.0/LICENSE` & `superstore-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superstore-0.2.0/Makefile` & `superstore-0.2.1/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tests: ## Make unit tests
 	python -m pytest -v superstore --cov=superstore --junitxml=python_junit.xml --cov-report=xml --cov-branch
 
 lint: ## run linter
-	python -m ruff superstore setup.py
+	python -m ruff check superstore setup.py
 
 fix:  ## run black fix
 	python -m ruff format superstore/ setup.py
 
 check:  ## run manifest checks
 	check-manifest -v
```

### Comparing `superstore-0.2.0/PKG-INFO` & `superstore-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superstore
-Version: 0.2.0
+Version: 0.2.1
 Summary: Categorical data generator
 Home-page: https://github.com/timkpaine/superstore
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
 Keywords: finance data
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Requires-Dist: Faker>=1.0.1
 Requires-Dist: pandas>=0.23.4
 Provides-Extra: dev
 Requires-Dist: Faker>=1.0.1; extra == "dev"
 Requires-Dist: pandas>=0.23.4; extra == "dev"
 Requires-Dist: bump2version>=1.0.0; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
-Requires-Dist: ruff>=0.1.4; extra == "dev"
+Requires-Dist: ruff<0.4,>=0.3; extra == "dev"
 Requires-Dist: pytest>=4.3.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
 
 # Superstore
 
 Categorical data generator
```

### Comparing `superstore-0.2.0/README.md` & `superstore-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `superstore-0.2.0/setup.cfg` & `superstore-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 commit = True
 tag = False
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
```

### Comparing `superstore-0.2.0/setup.py` & `superstore-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     "Faker>=1.0.1",
     "pandas>=0.23.4",
 ]
 
 requires_dev = requires + [
     "bump2version>=1.0.0",
     "check-manifest",
-    "ruff>=0.1.4",
+    "ruff>=0.3,<0.4",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
 ]
 
 setup(
     name=name,
-    version="0.2.0",
+    version="0.2.1",
     description="Categorical data generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/timkpaine/{name}".format(name=name),
     author="Tim Paine",
     author_email="t.paine154@gmail.com",
     license="Apache 2.0",
```

### Comparing `superstore-0.2.0/superstore/superstore.py` & `superstore-0.2.1/superstore/superstore.py`

 * *Files identical despite different names*

### Comparing `superstore-0.2.0/superstore/tests/test_superstore.py` & `superstore-0.2.1/superstore/tests/test_superstore.py`

 * *Files identical despite different names*

### Comparing `superstore-0.2.0/superstore/utils.py` & `superstore-0.2.1/superstore/utils.py`

 * *Files identical despite different names*

### Comparing `superstore-0.2.0/superstore/vendored/timeseries.py` & `superstore-0.2.1/superstore/vendored/timeseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     return DatetimeIndex(dr, name=name, **kwargs)
 
 
 def makeTimeSeries(nper=None, freq="B", name=None) -> Series:
     if nper is None:
         nper = _N
     return Series(
-        np.random.default_rng(2).standard_normal(nper),
+        np.random.normal(0.2, 1, nper).cumsum(),
         index=makeDateIndex(nper, freq=freq),
         name=name,
     )
 
 
 def getTimeSeriesData(nper=None, freq="B") -> dict[str, Series]:
     return {c: makeTimeSeries(nper, freq) for c in getCols(_K)}
```

### Comparing `superstore-0.2.0/superstore.egg-info/PKG-INFO` & `superstore-0.2.1/superstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superstore
-Version: 0.2.0
+Version: 0.2.1
 Summary: Categorical data generator
 Home-page: https://github.com/timkpaine/superstore
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
 Keywords: finance data
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Requires-Dist: Faker>=1.0.1
 Requires-Dist: pandas>=0.23.4
 Provides-Extra: dev
 Requires-Dist: Faker>=1.0.1; extra == "dev"
 Requires-Dist: pandas>=0.23.4; extra == "dev"
 Requires-Dist: bump2version>=1.0.0; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
-Requires-Dist: ruff>=0.1.4; extra == "dev"
+Requires-Dist: ruff<0.4,>=0.3; extra == "dev"
 Requires-Dist: pytest>=4.3.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
 
 # Superstore
 
 Categorical data generator
```

