# Comparing `tmp/jobbergate_api-5.0.0a0.tar.gz` & `tmp/jobbergate_api-5.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-5.0.0a0.tar", max compression
+gzip compressed data, was "jobbergate_api-5.0.0a1.tar", max compression
```

## Comparing `jobbergate_api-5.0.0a0.tar` & `jobbergate_api-5.0.0a1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1082 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/LICENSE
--rw-r--r--   0        0        0      683 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/README.md
--rw-r--r--   0        0        0      169 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0      177 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/constants.py
--rw-r--r--   0        0        0     5251 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/dependencies.py
--rw-r--r--   0        0        0     3620 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/file_validation.py
--rw-r--r--   0        0        0     1955 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/garbage_collector.py
--rw-r--r--   0        0        0       43 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/__init__.py
--rw-r--r--   0        0        0      100 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/constants.py
--rw-r--r--   0        0        0     4098 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/models.py
--rw-r--r--   0        0        0    15042 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/routers.py
--rw-r--r--   0        0        0     5720 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/schemas.py
--rw-r--r--   0        0        0     3749 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/services.py
--rw-r--r--   0        0        0       40 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     2984 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    13361 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     4759 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0     6390 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/services.py
--rw-r--r--   0        0        0     1295 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/tools.py
--rw-r--r--   0        0        0       44 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0     6561 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     3575 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    14094 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0     8117 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0     1285 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/services.py
--rw-r--r--   0        0        0     5986 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/models.py
--rw-r--r--   0        0        0      558 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     2254 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/schemas.py
--rw-r--r--   0        0        0    23693 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/apps/services.py
--rw-r--r--   0        0        0     4589 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/config.py
--rw-r--r--   0        0        0     2467 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     1627 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/logging.py
--rw-r--r--   0        0        0     3496 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/main.py
--rw-r--r--   0        0        0     3436 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0     2781 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/rabbitmq_notification.py
--rw-r--r--   0        0        0     1082 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/safe_types.py
--rw-r--r--   0        0        0     4598 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/security.py
--rw-r--r--   0        0        0    10874 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/storage.py
--rw-r--r--   0        0        0     1146 2024-03-26 18:59:27.387223 jobbergate_api-5.0.0a0/jobbergate_api/version.py
--rw-r--r--   0        0        0     3982 2024-03-26 18:59:27.391223 jobbergate_api-5.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/LICENSE
+-rw-r--r--   0        0        0      683 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/README.md
+-rw-r--r--   0        0        0      169 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0      177 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/constants.py
+-rw-r--r--   0        0        0     5251 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/dependencies.py
+-rw-r--r--   0        0        0     3620 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/file_validation.py
+-rw-r--r--   0        0        0     1955 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/garbage_collector.py
+-rw-r--r--   0        0        0       43 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/constants.py
+-rw-r--r--   0        0        0     4098 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/models.py
+-rw-r--r--   0        0        0    15042 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/routers.py
+-rw-r--r--   0        0        0     5720 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/schemas.py
+-rw-r--r--   0        0        0     3749 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/services.py
+-rw-r--r--   0        0        0       40 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     2984 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    13361 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     4759 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0     6390 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/services.py
+-rw-r--r--   0        0        0     1295 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/tools.py
+-rw-r--r--   0        0        0       44 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     6561 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     3575 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    14094 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0     8117 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0     1285 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/services.py
+-rw-r--r--   0        0        0     5986 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/models.py
+-rw-r--r--   0        0        0      558 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     2254 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/schemas.py
+-rw-r--r--   0        0        0    23693 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/apps/services.py
+-rw-r--r--   0        0        0     4589 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2467 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     1627 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/logging.py
+-rw-r--r--   0        0        0     3496 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3436 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0     2781 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/rabbitmq_notification.py
+-rw-r--r--   0        0        0     1082 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/safe_types.py
+-rw-r--r--   0        0        0     4598 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/security.py
+-rw-r--r--   0        0        0    10874 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/storage.py
+-rw-r--r--   0        0        0     1146 2024-04-04 21:27:33.534259 jobbergate_api-5.0.0a1/jobbergate_api/version.py
+-rw-r--r--   0        0        0     3982 2024-04-04 21:27:33.538259 jobbergate_api-5.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.0.0a1/PKG-INFO
```

### Comparing `jobbergate_api-5.0.0a0/LICENSE` & `jobbergate_api-5.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/README.md` & `jobbergate_api-5.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/dependencies.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/dependencies.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/file_validation.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/garbage_collector.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/models.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/routers.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/schemas.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_script_templates/services.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_script_templates/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/services.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_scripts/tools.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/job_submissions/services.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/job_submissions/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/models.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/permissions.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/schemas.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/apps/services.py` & `jobbergate_api-5.0.0a1/jobbergate_api/apps/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/config.py` & `jobbergate_api-5.0.0a1/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/email_notification.py` & `jobbergate_api-5.0.0a1/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/logging.py` & `jobbergate_api-5.0.0a1/jobbergate_api/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/main.py` & `jobbergate_api-5.0.0a1/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/meta_mapper.py` & `jobbergate_api-5.0.0a1/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/rabbitmq_notification.py` & `jobbergate_api-5.0.0a1/jobbergate_api/rabbitmq_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/safe_types.py` & `jobbergate_api-5.0.0a1/jobbergate_api/safe_types.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/security.py` & `jobbergate_api-5.0.0a1/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/storage.py` & `jobbergate_api-5.0.0a1/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/jobbergate_api/version.py` & `jobbergate_api-5.0.0a1/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a0/pyproject.toml` & `jobbergate_api-5.0.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "5.0.0a0"
+version = "5.0.0a1"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_api-5.0.0a0/PKG-INFO` & `jobbergate_api-5.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 5.0.0a0
+Version: 5.0.0a1
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

