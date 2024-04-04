# Comparing `tmp/openshift_cluster_management_python_wrapper-1.0.96.tar.gz` & `tmp/openshift_cluster_management_python_wrapper-1.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_cluster_management_python_wrapper-1.0.96.tar", max compression
+gzip compressed data, was "openshift_cluster_management_python_wrapper-1.0.97.tar", max compression
```

## Comparing `openshift_cluster_management_python_wrapper-1.0.96.tar` & `openshift_cluster_management_python_wrapper-1.0.97.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-31 14:57:36.526262 openshift_cluster_management_python_wrapper-1.0.96/LICENSE
--rw-r--r--   0        0        0     1346 2024-03-31 14:57:36.527262 openshift_cluster_management_python_wrapper-1.0.96/README.md
--rw-r--r--   0        0        0        0 2024-03-31 14:57:36.527262 openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/__init__.py
--rw-r--r--   0        0        0    33804 2024-03-31 14:57:36.527262 openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/cluster.py
--rw-r--r--   0        0        0      554 2024-03-31 14:57:36.527262 openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/exceptions.py
--rw-r--r--   0        0        0      882 2024-03-31 14:57:36.527262 openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/manifests/managed-api-service-policy.json
--rw-r--r--   0        0        0     4139 2024-03-31 14:57:36.527262 openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/ocm_client.py
--rw-r--r--   0        0        0     1405 2024-03-31 14:57:36.527262 openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/versions.py
--rw-r--r--   0        0        0     1927 2024-03-31 14:57:41.358221 openshift_cluster_management_python_wrapper-1.0.96/pyproject.toml
--rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 openshift_cluster_management_python_wrapper-1.0.96/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-04 07:28:28.023483 openshift_cluster_management_python_wrapper-1.0.97/LICENSE
+-rw-r--r--   0        0        0     1346 2024-04-04 07:28:28.023483 openshift_cluster_management_python_wrapper-1.0.97/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 07:28:28.023483 openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/__init__.py
+-rw-r--r--   0        0        0    33804 2024-04-04 07:28:28.023483 openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/cluster.py
+-rw-r--r--   0        0        0      554 2024-04-04 07:28:28.023483 openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/exceptions.py
+-rw-r--r--   0        0        0      882 2024-04-04 07:28:28.024483 openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/manifests/managed-api-service-policy.json
+-rw-r--r--   0        0        0     4139 2024-04-04 07:28:28.024483 openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/ocm_client.py
+-rw-r--r--   0        0        0     1405 2024-04-04 07:28:28.024483 openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/versions.py
+-rw-r--r--   0        0        0     1927 2024-04-04 07:28:32.500451 openshift_cluster_management_python_wrapper-1.0.97/pyproject.toml
+-rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 openshift_cluster_management_python_wrapper-1.0.97/PKG-INFO
```

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/LICENSE` & `openshift_cluster_management_python_wrapper-1.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/README.md` & `openshift_cluster_management_python_wrapper-1.0.97/README.md`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/cluster.py` & `openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/exceptions.py` & `openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/manifests/managed-api-service-policy.json` & `openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/manifests/managed-api-service-policy.json`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/ocm_client.py` & `openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/ocm_client.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/ocm_python_wrapper/versions.py` & `openshift_cluster_management_python_wrapper-1.0.97/ocm_python_wrapper/versions.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/pyproject.toml` & `openshift_cluster_management_python_wrapper-1.0.97/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "openshift-cluster-management-python-wrapper"
 description = "Wrapper around https://github.com/openshift/openshift-cluster-management-python-client"
-version = "1.0.96"
+version = "1.0.97"
 authors = ["Meni Yakove <myakove@gmail.com>", "Ruth Netser <rnetser@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/RedHatQE/openshift-cluster-management-python-wrapper"
 documentation = "https://github.com/RedHatQE/openshift-cluster-management-python-wrapper/blob/main/README.md"
 keywords = ["Openshift", "OCM"]
 classifiers = [
```

### Comparing `openshift_cluster_management_python_wrapper-1.0.96/PKG-INFO` & `openshift_cluster_management_python_wrapper-1.0.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-wrapper
-Version: 1.0.96
+Version: 1.0.97
 Summary: Wrapper around https://github.com/openshift/openshift-cluster-management-python-client
 Home-page: https://github.com/RedHatQE/openshift-cluster-management-python-wrapper
 License: Apache-2.0
 Keywords: Openshift,OCM
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
```

