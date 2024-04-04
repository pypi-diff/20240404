# Comparing `tmp/tutto_api_client-1.0.2.tar.gz` & `tmp/tutto_api_client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutto_api_client-1.0.2.tar", max compression
+gzip compressed data, was "tutto_api_client-1.0.5.tar", max compression
```

## Comparing `tutto_api_client-1.0.2.tar` & `tutto_api_client-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1252 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/README.md
--rw-r--r--   0        0        0      318 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      290 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/__init__.py
--rw-r--r--   0        0        0     3597 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/core/endpoints_factory.py
--rw-r--r--   0        0        0     2295 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/helpers/http.py
--rw-r--r--   0        0        0    10319 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/main.py
--rw-r--r--   0        0        0     3553 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/models/authorization.py
--rw-r--r--   0        0        0    14644 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/models/endpoints.py
--rw-r--r--   0        0        0     2502 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/models/entities.py
--rw-r--r--   0        0        0     2113 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/utils/filter_clean_utils.py
--rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 tutto_api_client-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1252 2024-04-04 18:35:35.726526 tutto_api_client-1.0.5/README.md
+-rw-r--r--   0        0        0      318 2024-04-04 18:35:35.726526 tutto_api_client-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      290 2024-04-04 18:35:35.726526 tutto_api_client-1.0.5/tutto_api_client/__init__.py
+-rw-r--r--   0        0        0     3597 2024-04-04 18:35:35.726526 tutto_api_client-1.0.5/tutto_api_client/core/endpoints_factory.py
+-rw-r--r--   0        0        0     2295 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/helpers/http.py
+-rw-r--r--   0        0        0    10319 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/main.py
+-rw-r--r--   0        0        0     3541 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/models/authorization.py
+-rw-r--r--   0        0        0    14644 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/models/endpoints.py
+-rw-r--r--   0        0        0     2502 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/models/entities.py
+-rw-r--r--   0        0        0     2113 2024-04-04 18:35:35.730526 tutto_api_client-1.0.5/tutto_api_client/utils/filter_clean_utils.py
+-rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 tutto_api_client-1.0.5/PKG-INFO
```

### Comparing `tutto_api_client-1.0.2/README.md` & `tutto_api_client-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.2/tutto_api_client/core/endpoints_factory.py` & `tutto_api_client-1.0.5/tutto_api_client/core/endpoints_factory.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.2/tutto_api_client/helpers/http.py` & `tutto_api_client-1.0.5/tutto_api_client/helpers/http.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.2/tutto_api_client/main.py` & `tutto_api_client-1.0.5/tutto_api_client/main.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.2/tutto_api_client/models/authorization.py` & `tutto_api_client-1.0.5/tutto_api_client/models/authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class _TOKEN_ORIGIN(Enum):
     USER = auto()
     API = auto()
 
 
-@dataclass(slots=True, init=True)
+@dataclass(init=True)
 class _Auth:
     status: int
     message: str
     type: str
     token: str
     origin: _TOKEN_ORIGIN
     companies: List[int]
```

### Comparing `tutto_api_client-1.0.2/tutto_api_client/models/endpoints.py` & `tutto_api_client-1.0.5/tutto_api_client/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.2/tutto_api_client/models/entities.py` & `tutto_api_client-1.0.5/tutto_api_client/models/entities.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.2/tutto_api_client/utils/filter_clean_utils.py` & `tutto_api_client-1.0.5/tutto_api_client/utils/filter_clean_utils.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-1.0.2/PKG-INFO` & `tutto_api_client-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutto-api-client
-Version: 1.0.2
+Version: 1.0.5
 Summary: 
 Author: rapha-pereira
 Author-email: raphaelpgomes1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

