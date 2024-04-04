# Comparing `tmp/openhexa.toolbox-0.1.8.tar.gz` & `tmp/openhexa.toolbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.toolbox-0.1.8.tar", last modified: Thu Feb  8 09:50:43 2024, max compression
+gzip compressed data, was "openhexa.toolbox-0.2.0.tar", last modified: Thu Apr  4 12:35:19 2024, max compression
```

## Comparing `openhexa.toolbox-0.1.8.tar` & `openhexa.toolbox-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:43.293258 openhexa.toolbox-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-02-08 09:50:43.293258 openhexa.toolbox-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:43.289258 openhexa.toolbox-0.1.8/openhexa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:43.289258 openhexa.toolbox-0.1.8/openhexa/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/openhexa/toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:43.293258 openhexa.toolbox-0.1.8/openhexa/toolbox/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/openhexa/toolbox/dhis2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/openhexa/toolbox/dhis2/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35411 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/openhexa/toolbox/dhis2/dhis2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/openhexa/toolbox/dhis2/periods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:43.293258 openhexa.toolbox-0.1.8/openhexa.toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-02-08 09:50:43.000000 openhexa.toolbox-0.1.8/openhexa.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-08 09:50:43.000000 openhexa.toolbox-0.1.8/openhexa.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 09:50:43.000000 openhexa.toolbox-0.1.8/openhexa.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-08 09:50:43.000000 openhexa.toolbox-0.1.8/openhexa.toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-08 09:50:43.000000 openhexa.toolbox-0.1.8/openhexa.toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 09:50:43.293258 openhexa.toolbox-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:43.293258 openhexa.toolbox-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 09:50:43.293258 openhexa.toolbox-0.1.8/tests/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/tests/dhis2/test_dhis2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/tests/dhis2/test_dhis2_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-08 09:50:23.000000 openhexa.toolbox-0.1.8/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.647705 openhexa.toolbox-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.639705 openhexa.toolbox-0.2.0/openhexa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/openhexa/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35411 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/periods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/openhexa/toolbox/kobo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 12:35:19.000000 openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:35:19.647705 openhexa.toolbox-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:19.643705 openhexa.toolbox-0.2.0/tests/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/tests/dhis2/test_dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/tests/dhis2/test_dhis2_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 12:34:53.000000 openhexa.toolbox-0.2.0/tests/test_lib.py
```

### Comparing `openhexa.toolbox-0.1.8/LICENSE` & `openhexa.toolbox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.8/PKG-INFO` & `openhexa.toolbox-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.8
+Version: 0.2.0
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
         
@@ -33,14 +33,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-dateutil
 Requires-Dist: pandas
+Requires-Dist: shapely
+Requires-Dist: geopandas
 Requires-Dist: polars
 Requires-Dist: diskcache
 Provides-Extra: dev
 Requires-Dist: ruff~=0.0.278; extra == "dev"
 Requires-Dist: pytest~=7.3.0; extra == "dev"
 Requires-Dist: build~=0.10.0; extra == "dev"
 Requires-Dist: pytest-cov~=4.0.0; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.1.8 Summary: A set of
+Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.0 Summary: A set of
 tools to acquire & process data from various sources Author-email: Bluesquare
 bluesquarehub.com> Maintainer-email: Bluesquare
 bluesquarehub.com> License: MIT License Copyright (c) 2023 Bluesquare
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -17,20 +17,20 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/blsq/
 openhexa-toolbox Project-URL: Bug Tracker, https://github.com/blsq/openhexa-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests Requires-Dist: python-dateutil
-Requires-Dist: pandas Requires-Dist: polars Requires-Dist: diskcache Provides-
-Extra: dev Requires-Dist: ruff~=0.0.278; extra == "dev" Requires-Dist:
-pytest~=7.3.0; extra == "dev" Requires-Dist: build~=0.10.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.0.0; extra == "dev" Requires-Dist: black~=23.7.0;
-extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-responses; extra == "dev"
+Requires-Dist: pandas Requires-Dist: shapely Requires-Dist: geopandas Requires-
+Dist: polars Requires-Dist: diskcache Provides-Extra: dev Requires-Dist:
+ruff~=0.0.278; extra == "dev" Requires-Dist: pytest~=7.3.0; extra == "dev"
+Requires-Dist: build~=0.10.0; extra == "dev" Requires-Dist: pytest-cov~=4.0.0;
+extra == "dev" Requires-Dist: black~=23.7.0; extra == "dev" Requires-Dist: pre-
+commit; extra == "dev" Requires-Dist: responses; extra == "dev"
                                 [OpenHEXA Logo]
                      OOppeenn--ssoouurrccee DDaattaa iinntteeggrraattiioonn ppllaattffoorrmm
                                  _[_T_e_s_t_ _S_u_i_t_e_]
 OpenHEXA Toolbox ================ OpenHEXA is an open-source data integration
 platform developed by [Bluesquare](https://bluesquarehub.com). The Toolbox is
 an utility library to acquire and process data from various data sources. It is
 installed by default on OpenHEXA, and can be used both in notebooks and in data
```

### Comparing `openhexa.toolbox-0.1.8/README.md` & `openhexa.toolbox-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.8/openhexa/toolbox/dhis2/api.py` & `openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.8/openhexa/toolbox/dhis2/dhis2.py` & `openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/dhis2.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.8/openhexa/toolbox/dhis2/periods.py` & `openhexa.toolbox-0.2.0/openhexa/toolbox/dhis2/periods.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.8/openhexa.toolbox.egg-info/PKG-INFO` & `openhexa.toolbox-0.2.0/openhexa.toolbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.8
+Version: 0.2.0
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
         
@@ -33,14 +33,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-dateutil
 Requires-Dist: pandas
+Requires-Dist: shapely
+Requires-Dist: geopandas
 Requires-Dist: polars
 Requires-Dist: diskcache
 Provides-Extra: dev
 Requires-Dist: ruff~=0.0.278; extra == "dev"
 Requires-Dist: pytest~=7.3.0; extra == "dev"
 Requires-Dist: build~=0.10.0; extra == "dev"
 Requires-Dist: pytest-cov~=4.0.0; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.1.8 Summary: A set of
+Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.0 Summary: A set of
 tools to acquire & process data from various sources Author-email: Bluesquare
 bluesquarehub.com> Maintainer-email: Bluesquare
 bluesquarehub.com> License: MIT License Copyright (c) 2023 Bluesquare
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -17,20 +17,20 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/blsq/
 openhexa-toolbox Project-URL: Bug Tracker, https://github.com/blsq/openhexa-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests Requires-Dist: python-dateutil
-Requires-Dist: pandas Requires-Dist: polars Requires-Dist: diskcache Provides-
-Extra: dev Requires-Dist: ruff~=0.0.278; extra == "dev" Requires-Dist:
-pytest~=7.3.0; extra == "dev" Requires-Dist: build~=0.10.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.0.0; extra == "dev" Requires-Dist: black~=23.7.0;
-extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-responses; extra == "dev"
+Requires-Dist: pandas Requires-Dist: shapely Requires-Dist: geopandas Requires-
+Dist: polars Requires-Dist: diskcache Provides-Extra: dev Requires-Dist:
+ruff~=0.0.278; extra == "dev" Requires-Dist: pytest~=7.3.0; extra == "dev"
+Requires-Dist: build~=0.10.0; extra == "dev" Requires-Dist: pytest-cov~=4.0.0;
+extra == "dev" Requires-Dist: black~=23.7.0; extra == "dev" Requires-Dist: pre-
+commit; extra == "dev" Requires-Dist: responses; extra == "dev"
                                 [OpenHEXA Logo]
                      OOppeenn--ssoouurrccee DDaattaa iinntteeggrraattiioonn ppllaattffoorrmm
                                  _[_T_e_s_t_ _S_u_i_t_e_]
 OpenHEXA Toolbox ================ OpenHEXA is an open-source data integration
 platform developed by [Bluesquare](https://bluesquarehub.com). The Toolbox is
 an utility library to acquire and process data from various data sources. It is
 installed by default on OpenHEXA, and can be used both in notebooks and in data
```

### Comparing `openhexa.toolbox-0.1.8/tests/dhis2/test_dhis2.py` & `openhexa.toolbox-0.2.0/tests/dhis2/test_dhis2.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.8/tests/dhis2/test_dhis2_periods.py` & `openhexa.toolbox-0.2.0/tests/dhis2/test_dhis2_periods.py`

 * *Files identical despite different names*

