# Comparing `tmp/snakemake_storage_plugin_xrootd-0.1.1.tar.gz` & `tmp/snakemake_storage_plugin_xrootd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_xrootd-0.1.1.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_xrootd-0.1.2.tar", max compression
```

## Comparing `snakemake_storage_plugin_xrootd-0.1.1.tar` & `snakemake_storage_plugin_xrootd-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2024-04-04 13:34:29.569232 snakemake_storage_plugin_xrootd-0.1.1/LICENSE
--rw-r--r--   0        0        0      247 2024-04-04 13:34:29.569232 snakemake_storage_plugin_xrootd-0.1.1/README.md
--rw-r--r--   0        0        0      780 2024-04-04 13:34:29.569232 snakemake_storage_plugin_xrootd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12836 2024-04-04 13:34:29.569232 snakemake_storage_plugin_xrootd-0.1.1/snakemake_storage_plugin_xrootd/__init__.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 snakemake_storage_plugin_xrootd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-04 14:06:02.403181 snakemake_storage_plugin_xrootd-0.1.2/LICENSE
+-rw-r--r--   0        0        0      247 2024-04-04 14:06:02.403181 snakemake_storage_plugin_xrootd-0.1.2/README.md
+-rw-r--r--   0        0        0      855 2024-04-04 14:06:02.403181 snakemake_storage_plugin_xrootd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    12836 2024-04-04 14:06:02.403181 snakemake_storage_plugin_xrootd-0.1.2/snakemake_storage_plugin_xrootd/__init__.py
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 snakemake_storage_plugin_xrootd-0.1.2/PKG-INFO
```

### Comparing `snakemake_storage_plugin_xrootd-0.1.1/LICENSE` & `snakemake_storage_plugin_xrootd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_xrootd-0.1.1/pyproject.toml` & `snakemake_storage_plugin_xrootd-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "snakemake-storage-plugin-xrootd"
-version = "0.1.1"
-description = ""
+version = "0.1.2"
+description = "A Snakemake storage plugin for xrootd storage"
 authors = [
     "Chris Burr <christopher.burr@cern.ch>",
     "Johannes Koester <johannes.koester@uni-due.de>"
 ]
 readme = "README.md"
-repository = "https://github.com/your/plugin"
+repository = "https://github.com/snakemake/snakemake-storage-plugin-xrootd"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/xrootd.html"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 snakemake-interface-common = "^1.15.0"
 snakemake-interface-storage-plugins = "^3.0.0"
 xrootd = "^5.6.4"
```

### Comparing `snakemake_storage_plugin_xrootd-0.1.1/snakemake_storage_plugin_xrootd/__init__.py` & `snakemake_storage_plugin_xrootd-0.1.2/snakemake_storage_plugin_xrootd/__init__.py`

 * *Files identical despite different names*

