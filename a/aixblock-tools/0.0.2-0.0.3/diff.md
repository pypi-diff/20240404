# Comparing `tmp/aixblock_tools-0.0.2.tar.gz` & `tmp/aixblock_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_tools-0.0.2.tar", max compression
+gzip compressed data, was "aixblock_tools-0.0.3.tar", max compression
```

## Comparing `aixblock_tools-0.0.2.tar` & `aixblock_tools-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       14 2024-04-02 11:26:35.487186 aixblock_tools-0.0.2/README.md
--rw-r--r--   0        0        0     6148 2024-04-03 05:20:29.911723 aixblock_tools-0.0.2/aixblock_tools/.DS_Store
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.157031 aixblock_tools-0.0.2/aixblock_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.157393 aixblock_tools-0.0.2/aixblock_tools/core/__init__.py
--rw-r--r--   0        0        0      204 2023-08-31 04:15:47.167875 aixblock_tools-0.0.2/aixblock_tools/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4302 2023-08-31 04:15:47.169561 aixblock_tools-0.0.2/aixblock_tools/core/__pycache__/label_config.cpython-39.pyc
--rw-r--r--   0        0        0     5753 2024-04-03 07:24:15.704627 aixblock_tools-0.0.2/aixblock_tools/core/label_config.py
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.158189 aixblock_tools-0.0.2/aixblock_tools/core/utils/__init__.py
--rw-r--r--   0        0        0      210 2023-08-31 04:15:47.170281 aixblock_tools-0.0.2/aixblock_tools/core/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      405 2023-08-31 04:15:47.170884 aixblock_tools-0.0.2/aixblock_tools/core/utils/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0        0        0     3489 2023-08-31 04:15:47.172503 aixblock_tools-0.0.2/aixblock_tools/core/utils/__pycache__/io.cpython-39.pyc
--rw-r--r--   0        0        0     1362 2023-08-31 04:15:47.173662 aixblock_tools-0.0.2/aixblock_tools/core/utils/__pycache__/params.cpython-39.pyc
--rw-r--r--   0        0        0       66 2023-08-31 04:15:47.158548 aixblock_tools-0.0.2/aixblock_tools/core/utils/exceptions.py
--rw-r--r--   0        0        0     3985 2024-04-03 07:24:15.704525 aixblock_tools-0.0.2/aixblock_tools/core/utils/io.py
--rw-r--r--   0        0        0     1244 2023-08-31 04:15:47.159590 aixblock_tools-0.0.2/aixblock_tools/core/utils/params.py
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.159877 aixblock_tools-0.0.2/aixblock_tools/postprocessing/__init__.py
--rw-r--r--   0        0        0      214 2023-08-31 04:15:47.174550 aixblock_tools-0.0.2/aixblock_tools/postprocessing/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2584 2023-08-31 04:15:47.175963 aixblock_tools-0.0.2/aixblock_tools/postprocessing/__pycache__/video.cpython-39.pyc
--rw-r--r--   0        0        0     3486 2024-04-03 07:24:15.704467 aixblock_tools-0.0.2/aixblock_tools/postprocessing/video.py
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.160904 aixblock_tools-0.0.2/aixblock_tools/tests/__init__.py
--rw-r--r--   0        0        0      205 2023-08-31 04:15:47.176686 aixblock_tools-0.0.2/aixblock_tools/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4193 2023-08-31 04:15:47.177862 aixblock_tools-0.0.2/aixblock_tools/tests/__pycache__/test_core_label_config.cpython-39.pyc
--rw-r--r--   0        0        0     6811 2023-08-31 04:15:47.180967 aixblock_tools-0.0.2/aixblock_tools/tests/__pycache__/test_postprocessing_video.cpython-39.pyc
--rw-r--r--   0        0        0     4349 2024-04-03 07:24:15.766177 aixblock_tools-0.0.2/aixblock_tools/tests/test_core_label_config.py
--rw-r--r--   0        0        0    14387 2024-04-03 07:24:15.765793 aixblock_tools-0.0.2/aixblock_tools/tests/test_postprocessing_video.py
--rw-r--r--   0        0        0      266 2024-04-03 07:24:53.765453 aixblock_tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 aixblock_tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2024-04-02 11:26:35.487186 aixblock_tools-0.0.3/README.md
+-rw-r--r--   0        0        0     6148 2024-04-03 05:20:29.911723 aixblock_tools-0.0.3/aixblock_tools/.DS_Store
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.157031 aixblock_tools-0.0.3/aixblock_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.157393 aixblock_tools-0.0.3/aixblock_tools/core/__init__.py
+-rw-r--r--   0        0        0      204 2023-08-31 04:15:47.167875 aixblock_tools-0.0.3/aixblock_tools/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4302 2023-08-31 04:15:47.169561 aixblock_tools-0.0.3/aixblock_tools/core/__pycache__/label_config.cpython-39.pyc
+-rw-r--r--   0        0        0     5753 2024-04-03 07:24:15.704627 aixblock_tools-0.0.3/aixblock_tools/core/label_config.py
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.158189 aixblock_tools-0.0.3/aixblock_tools/core/utils/__init__.py
+-rw-r--r--   0        0        0      210 2023-08-31 04:15:47.170281 aixblock_tools-0.0.3/aixblock_tools/core/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      405 2023-08-31 04:15:47.170884 aixblock_tools-0.0.3/aixblock_tools/core/utils/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0        0        0     3489 2023-08-31 04:15:47.172503 aixblock_tools-0.0.3/aixblock_tools/core/utils/__pycache__/io.cpython-39.pyc
+-rw-r--r--   0        0        0     1362 2023-08-31 04:15:47.173662 aixblock_tools-0.0.3/aixblock_tools/core/utils/__pycache__/params.cpython-39.pyc
+-rw-r--r--   0        0        0       66 2023-08-31 04:15:47.158548 aixblock_tools-0.0.3/aixblock_tools/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3985 2024-04-03 07:24:15.704525 aixblock_tools-0.0.3/aixblock_tools/core/utils/io.py
+-rw-r--r--   0        0        0     1241 2024-04-03 08:23:43.577921 aixblock_tools-0.0.3/aixblock_tools/core/utils/params.py
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.159877 aixblock_tools-0.0.3/aixblock_tools/postprocessing/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-31 04:15:47.174550 aixblock_tools-0.0.3/aixblock_tools/postprocessing/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2584 2023-08-31 04:15:47.175963 aixblock_tools-0.0.3/aixblock_tools/postprocessing/__pycache__/video.cpython-39.pyc
+-rw-r--r--   0        0        0     3486 2024-04-03 07:24:15.704467 aixblock_tools-0.0.3/aixblock_tools/postprocessing/video.py
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.160904 aixblock_tools-0.0.3/aixblock_tools/tests/__init__.py
+-rw-r--r--   0        0        0      205 2023-08-31 04:15:47.176686 aixblock_tools-0.0.3/aixblock_tools/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4193 2023-08-31 04:15:47.177862 aixblock_tools-0.0.3/aixblock_tools/tests/__pycache__/test_core_label_config.cpython-39.pyc
+-rw-r--r--   0        0        0     6811 2023-08-31 04:15:47.180967 aixblock_tools-0.0.3/aixblock_tools/tests/__pycache__/test_postprocessing_video.cpython-39.pyc
+-rw-r--r--   0        0        0     4349 2024-04-03 07:24:15.766177 aixblock_tools-0.0.3/aixblock_tools/tests/test_core_label_config.py
+-rw-r--r--   0        0        0    14387 2024-04-03 07:24:15.765793 aixblock_tools-0.0.3/aixblock_tools/tests/test_postprocessing_video.py
+-rw-r--r--   0        0        0      266 2024-04-04 02:05:02.267897 aixblock_tools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 aixblock_tools-0.0.3/PKG-INFO
```

### Comparing `aixblock_tools-0.0.2/aixblock_tools/.DS_Store` & `aixblock_tools-0.0.3/aixblock_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/core/__pycache__/label_config.cpython-39.pyc` & `aixblock_tools-0.0.3/aixblock_tools/core/__pycache__/label_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/core/label_config.py` & `aixblock_tools-0.0.3/aixblock_tools/core/label_config.py`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/core/utils/__pycache__/io.cpython-39.pyc` & `aixblock_tools-0.0.3/aixblock_tools/core/utils/__pycache__/io.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/core/utils/__pycache__/params.cpython-39.pyc` & `aixblock_tools-0.0.3/aixblock_tools/core/utils/__pycache__/params.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/core/utils/io.py` & `aixblock_tools-0.0.3/aixblock_tools/core/utils/io.py`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/core/utils/params.py` & `aixblock_tools-0.0.3/aixblock_tools/core/utils/params.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 f'Incorrect bool value "{value}". '
                 f'It should be one of [1, 0, true, false, yes, no]'
             )
     return value
 
 
 def get_env(name, default=None, is_bool=False):
-    for env_key in ['LABEL_STUDIO_' + name, 'HEARTEX_' + name, name]:
+    for env_key in ['AIXBLOCK_' + name, 'PLATFORM_' + name, name]:
         value = os.environ.get(env_key)
         if value is not None:
             if is_bool:
                 return bool_from_request(os.environ, env_key, default)
             else:
                 return value
     return default
```

### Comparing `aixblock_tools-0.0.2/aixblock_tools/postprocessing/__pycache__/video.cpython-39.pyc` & `aixblock_tools-0.0.3/aixblock_tools/postprocessing/__pycache__/video.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/postprocessing/video.py` & `aixblock_tools-0.0.3/aixblock_tools/postprocessing/video.py`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/tests/__pycache__/test_core_label_config.cpython-39.pyc` & `aixblock_tools-0.0.3/aixblock_tools/tests/__pycache__/test_core_label_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/tests/__pycache__/test_postprocessing_video.cpython-39.pyc` & `aixblock_tools-0.0.3/aixblock_tools/tests/__pycache__/test_postprocessing_video.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/tests/test_core_label_config.py` & `aixblock_tools-0.0.3/aixblock_tools/tests/test_core_label_config.py`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.2/aixblock_tools/tests/test_postprocessing_video.py` & `aixblock_tools-0.0.3/aixblock_tools/tests/test_postprocessing_video.py`

 * *Files identical despite different names*

