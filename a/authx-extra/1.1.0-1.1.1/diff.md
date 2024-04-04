# Comparing `tmp/authx_extra-1.1.0.tar.gz` & `tmp/authx_extra-1.1.1.tar.gz`

## Comparing `authx_extra-1.1.0.tar` & `authx_extra-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.github/dependabot.yaml
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/__init__.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/cache.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/metrics.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/oauth2.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/profiler.py
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/addons/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/addons/expiry.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/addons/keys.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/extra/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 authx_extra-1.1.0/authx_extra/extra/_cache.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/all.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/linting.in
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/linting.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/optional.in
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/optional.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/pyproject.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/testing.in
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 authx_extra-1.1.0/requirements/testing.txt
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/clean.sh
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/docker.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/format.sh
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/lint.sh
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 authx_extra-1.1.0/scripts/requirements.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_cache.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_keys.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_method_cache.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_metrics.py
--rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_oauth2.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_profiler.py
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_session_middleware.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_skip_session_header_check_dict.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 authx_extra-1.1.0/tests/test_skip_session_header_check_list.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 authx_extra-1.1.0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx_extra-1.1.0/LICENSE
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 authx_extra-1.1.0/README.md
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 authx_extra-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 authx_extra-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.github/dependabot.yaml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/__init__.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/cache.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/metrics.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/oauth2.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/profiler.py
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/addons/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/addons/expiry.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/addons/keys.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/extra/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/extra/_cache.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/all.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/linting.in
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/linting.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/optional.in
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/optional.txt
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/pyproject.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/testing.in
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/testing.txt
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/clean.sh
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/docker.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/format.sh
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/lint.sh
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/requirements.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_cache.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_keys.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_method_cache.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_metrics.py
+-rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_oauth2.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_profiler.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_session_middleware.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_skip_session_header_check_dict.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_skip_session_header_check_list.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx_extra-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 authx_extra-1.1.1/README.md
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 authx_extra-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 authx_extra-1.1.1/PKG-INFO
```

### Comparing `authx_extra-1.1.0/.github/workflows/ci.yml` & `authx_extra-1.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/.github/workflows/release.yml` & `authx_extra-1.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/authx_extra/cache.py` & `authx_extra-1.1.1/authx_extra/cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/authx_extra/metrics.py` & `authx_extra-1.1.1/authx_extra/metrics.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/authx_extra/oauth2.py` & `authx_extra-1.1.1/authx_extra/oauth2.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/authx_extra/profiler.py` & `authx_extra-1.1.1/authx_extra/profiler.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/authx_extra/session.py` & `authx_extra-1.1.1/authx_extra/session.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/authx_extra/addons/expiry.py` & `authx_extra-1.1.1/authx_extra/addons/expiry.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/authx_extra/addons/keys.py` & `authx_extra-1.1.1/authx_extra/addons/keys.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/authx_extra/extra/_cache.py` & `authx_extra-1.1.1/authx_extra/extra/_cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/requirements/linting.txt` & `authx_extra-1.1.1/requirements/linting.txt`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/requirements/pyproject.txt` & `authx_extra-1.1.1/requirements/pyproject.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile pyproject.toml -o requirements/pyproject.txt
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via starlette
-authx==1.0.0
+authx==1.1.0
 cffi==1.16.0
     # via cryptography
 cryptography==42.0.5
     # via pyjwt
 ecdsa==0.18.0
     # via python-jose
 fastapi==0.110.1
```

### Comparing `authx_extra-1.1.0/requirements/testing.txt` & `authx_extra-1.1.1/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/scripts/clean.sh` & `authx_extra-1.1.1/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/scripts/docker.sh` & `authx_extra-1.1.1/scripts/docker.sh`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_cache.py` & `authx_extra-1.1.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_keys.py` & `authx_extra-1.1.1/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_method_cache.py` & `authx_extra-1.1.1/tests/test_method_cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_metrics.py` & `authx_extra-1.1.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_oauth2.py` & `authx_extra-1.1.1/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_profiler.py` & `authx_extra-1.1.1/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_session_middleware.py` & `authx_extra-1.1.1/tests/test_session_middleware.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_skip_session_header_check_dict.py` & `authx_extra-1.1.1/tests/test_skip_session_header_check_dict.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/tests/test_skip_session_header_check_list.py` & `authx_extra-1.1.1/tests/test_skip_session_header_check_list.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/.gitignore` & `authx_extra-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/LICENSE` & `authx_extra-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/README.md` & `authx_extra-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.0/pyproject.toml` & `authx_extra-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "authx==1.0.0",
+    "authx >=1.0.0",
 ]
 
 dynamic = ["version"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

### Comparing `authx_extra-1.1.0/PKG-INFO` & `authx_extra-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: authx_extra
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extra utilities for authx, including session, profiler & caching ✨
 Project-URL: Homepage, https://github.com/yezz123/authx_extra
 Project-URL: Documentation, https://authx.yezz.me/installation/#extra-dependencies
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: authx==1.0.0
+Requires-Dist: authx>=1.0.0
 Provides-Extra: cache
 Requires-Dist: redis<5.0.4,>=4.3.3; extra == 'cache'
 Provides-Extra: metrics
 Requires-Dist: prometheus-client<1.0.0,>=0.16.0; extra == 'metrics'
 Provides-Extra: profiler
 Requires-Dist: pyinstrument<4.7.0,>=4.1.1; extra == 'profiler'
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: authx_extra Version: 1.1.0 Summary: Extra utilities
+Metadata-Version: 2.3 Name: authx_extra Version: 1.1.1 Summary: Extra utilities
 for authx, including session, profiler & caching â¨ Project-URL: Homepage,
 https://github.com/yezz123/authx_extra Project-URL: Documentation, https://
 authx.yezz.me/installation/#extra-dependencies Project-URL: Funding, https://
 github.com/sponsors/yezz123 Author-email: Yasser Tahiri
 yezz.me> License-Expression: MIT License-File: LICENSE Keywords:
 Authentication,Cookie,FastAPI,JWT,Oauth2,Pydantic Classifier: Development
 Status :: 5 - Production/Stable Classifier: Framework :: AsyncIO Classifier:
@@ -13,15 +13,15 @@
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Requires-Python: >=3.8 Requires-Dist: authx==1.0.0
+Classifier: Typing :: Typed Requires-Python: >=3.8 Requires-Dist: authx>=1.0.0
 Provides-Extra: cache Requires-Dist: redis<5.0.4,>=4.3.3; extra == 'cache'
 Provides-Extra: metrics Requires-Dist: prometheus-client<1.0.0,>=0.16.0; extra
 == 'metrics' Provides-Extra: profiler Requires-Dist:
 pyinstrument<4.7.0,>=4.1.1; extra == 'profiler' Description-Content-Type: text/
 markdown # authx-extra ð«
                                     _[_A_u_t_h_X_]
      EExxttrraa uuttiilliittiieess ffoorr aauutthhxx,, iinncclluuddiinngg sseessssiioonn,, pprrooffiilleerr && ccaacchhiinngg ?â??¨
```

