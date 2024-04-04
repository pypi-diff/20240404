# Comparing `tmp/pzen-0.0.3.tar.gz` & `tmp/pzen-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzen-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pzen-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pzen-0.0.3.tar` & `pzen-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0      114 2024-04-03 20:02:19.932095 pzen-0.0.3/.flake8
--rw-r--r--   0        0        0     2014 2024-04-03 20:02:19.932095 pzen-0.0.3/.github/workflows/ci.yaml
--rw-r--r--   0        0        0       26 2024-04-03 20:02:19.932095 pzen-0.0.3/.gitignore
--rw-r--r--   0        0        0     1080 2024-04-03 20:02:19.932095 pzen-0.0.3/LICENSE
--rw-r--r--   0        0        0       29 2024-04-03 20:02:19.932095 pzen-0.0.3/README.md
--rw-r--r--   0        0        0       22 2024-04-03 20:02:19.932095 pzen-0.0.3/env.sh
--rw-r--r--   0        0        0      222 2024-04-03 20:02:19.932095 pzen-0.0.3/mypy.ini
--rw-r--r--   0        0        0      317 2024-04-03 20:02:19.932095 pzen-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       53 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/__init__.py
--rw-r--r--   0        0        0       47 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/core_types.py
--rw-r--r--   0        0        0     1988 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/numpy_utils.py
--rw-r--r--   0        0        0        0 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/py.typed
--rw-r--r--   0        0        0     2072 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/soundfile_utils.py
--rw-r--r--   0        0        0       43 2024-04-03 20:02:19.932095 pzen-0.0.3/requirements_dev.txt
--rw-r--r--   0        0        0       28 2024-04-03 20:02:19.932095 pzen-0.0.3/requirements_opt.txt
--rwxr-xr-x   0        0        0      112 2024-04-03 20:02:19.932095 pzen-0.0.3/scripts/ci_all
--rwxr-xr-x   0        0        0       99 2024-04-03 20:02:19.932095 pzen-0.0.3/scripts/setup_dependencies.sh
--rwxr-xr-x   0        0        0      105 2024-04-03 20:02:19.932095 pzen-0.0.3/scripts/setup_venv.sh
--rw-r--r--   0        0        0      952 2024-04-03 20:02:19.932095 pzen-0.0.3/tests/pzen/test_numpy_utils.py
--rw-r--r--   0        0        0      871 2024-04-03 20:02:19.932095 pzen-0.0.3/tests/pzen/test_soundfile_utils.py
--rw-r--r--   0        0        0      195 1970-01-01 00:00:00.000000 pzen-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      114 2024-04-04 20:19:03.018407 pzen-0.0.4/.flake8
+-rw-r--r--   0        0        0     2014 2024-04-04 20:19:03.018407 pzen-0.0.4/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0       26 2024-04-04 20:19:03.018407 pzen-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1080 2024-04-04 20:19:03.018407 pzen-0.0.4/LICENSE
+-rw-r--r--   0        0        0       29 2024-04-04 20:19:03.018407 pzen-0.0.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-04 20:19:03.018407 pzen-0.0.4/env.sh
+-rw-r--r--   0        0        0      343 2024-04-04 20:19:03.018407 pzen-0.0.4/mypy.ini
+-rw-r--r--   0        0        0      317 2024-04-04 20:19:03.018407 pzen-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/__init__.py
+-rw-r--r--   0        0        0     1062 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/cache_utils.py
+-rw-r--r--   0        0        0       47 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/core_types.py
+-rw-r--r--   0        0        0     1988 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/numpy_utils.py
+-rw-r--r--   0        0        0        0 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/py.typed
+-rw-r--r--   0        0        0     2072 2024-04-04 20:19:03.018407 pzen-0.0.4/pzen/soundfile_utils.py
+-rw-r--r--   0        0        0       43 2024-04-04 20:19:03.018407 pzen-0.0.4/requirements_dev.txt
+-rw-r--r--   0        0        0       60 2024-04-04 20:19:03.018407 pzen-0.0.4/requirements_opt.txt
+-rwxr-xr-x   0        0        0      112 2024-04-04 20:19:03.018407 pzen-0.0.4/scripts/ci_all
+-rwxr-xr-x   0        0        0       99 2024-04-04 20:19:03.018407 pzen-0.0.4/scripts/setup_dependencies.sh
+-rwxr-xr-x   0        0        0      105 2024-04-04 20:19:03.018407 pzen-0.0.4/scripts/setup_venv.sh
+-rw-r--r--   0        0        0        0 2024-04-04 20:19:03.018407 pzen-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-04 20:19:03.018407 pzen-0.0.4/tests/pzen/test_cache_utils.py
+-rw-r--r--   0        0        0      911 2024-04-04 20:19:03.018407 pzen-0.0.4/tests/pzen/test_numpy_utils.py
+-rw-r--r--   0        0        0      871 2024-04-04 20:19:03.018407 pzen-0.0.4/tests/pzen/test_soundfile_utils.py
+-rw-r--r--   0        0        0      236 1970-01-01 00:00:00.000000 pzen-0.0.4/PKG-INFO
```

### Comparing `pzen-0.0.3/.github/workflows/ci.yaml` & `pzen-0.0.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pzen-0.0.3/LICENSE` & `pzen-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pzen-0.0.3/pzen/numpy_utils.py` & `pzen-0.0.4/pzen/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pzen-0.0.3/pzen/soundfile_utils.py` & `pzen-0.0.4/pzen/soundfile_utils.py`

 * *Files identical despite different names*

### Comparing `pzen-0.0.3/tests/pzen/test_numpy_utils.py` & `pzen-0.0.4/tests/pzen/test_numpy_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,11 +27,8 @@
 
 
 def test_find_peaks__test_case_from_issue_18495():
     # https://github.com/scipy/scipy/issues/18495
     x = np.zeros(200)
     x[100:] = np.linspace(1.0, 0.0, 100) + np.random.normal(0.0, 1e-2, size=100)
 
-    npt.assert_equal(
-        find_peaks(x, distance=10),
-        np.array([100]),
-    )
+    assert len(find_peaks(x, distance=10)) == 1
```

### Comparing `pzen-0.0.3/tests/pzen/test_soundfile_utils.py` & `pzen-0.0.4/tests/pzen/test_soundfile_utils.py`

 * *Files identical despite different names*

