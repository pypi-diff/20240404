# Comparing `tmp/opentraveldata-0.0.9.post2.tar.gz` & `tmp/opentraveldata-0.0.9.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentraveldata-0.0.9.post2.tar", last modified: Fri Sep 22 16:20:56 2023, max compression
+gzip compressed data, was "opentraveldata-0.0.9.post3.tar", last modified: Thu Apr  4 21:18:46 2024, max compression
```

## Comparing `opentraveldata-0.0.9.post2.tar` & `opentraveldata-0.0.9.post3.tar`

### file list

```diff
@@ -1,28 +1,15 @@
-drwxr-xr-x   0 DENIS      (502)     1000        0 2023-09-22 16:20:56.438279 opentraveldata-0.0.9.post2/
--rw-r--r--   0 DENIS      (502)     1000      416 2023-09-22 15:47:45.000000 opentraveldata-0.0.9.post2/.gitignore
--rw-r--r--   0 DENIS      (502)     1000      956 2023-09-22 15:55:47.000000 opentraveldata-0.0.9.post2/.travis.yml
--rw-r--r--   0 DENIS      (502)     1000    15925 2023-09-22 16:20:56.436812 opentraveldata-0.0.9.post2/PKG-INFO
--rw-r--r--   0 DENIS      (502)     1000      261 2023-09-22 15:40:29.000000 opentraveldata-0.0.9.post2/Pipfile
--rw-r--r--   0 DENIS      (502)     1000    15190 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/README.md
--rw-r--r--   0 DENIS      (502)     1000       27 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/_config.yml
-drwxr-xr-x   0 DENIS      (502)     1000        0 2023-09-22 16:20:56.431361 opentraveldata-0.0.9.post2/opentraveldata/
--rw-r--r--   0 DENIS      (502)     1000       33 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/opentraveldata/.gitignore
--rw-r--r--   0 DENIS      (502)     1000     1057 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/opentraveldata/LICENSE
--rw-r--r--   0 DENIS      (502)     1000       91 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/opentraveldata/__init__.py
--rw-r--r--   0 DENIS      (502)     1000      911 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/opentraveldata/csvwriter.py
--rw-r--r--   0 DENIS      (502)     1000    36135 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/opentraveldata/opentraveldata.py
-drwxr-xr-x   0 DENIS      (502)     1000        0 2023-09-22 16:20:56.434610 opentraveldata-0.0.9.post2/opentraveldata.egg-info/
--rw-r--r--   0 DENIS      (502)     1000    15925 2023-09-22 16:20:56.000000 opentraveldata-0.0.9.post2/opentraveldata.egg-info/PKG-INFO
--rw-r--r--   0 DENIS      (502)     1000      489 2023-09-22 16:20:56.000000 opentraveldata-0.0.9.post2/opentraveldata.egg-info/SOURCES.txt
--rw-r--r--   0 DENIS      (502)     1000        1 2023-09-22 16:20:56.000000 opentraveldata-0.0.9.post2/opentraveldata.egg-info/dependency_links.txt
--rw-r--r--   0 DENIS      (502)     1000       15 2023-09-22 16:20:56.000000 opentraveldata-0.0.9.post2/opentraveldata.egg-info/top_level.txt
--rw-r--r--   0 DENIS      (502)     1000     1446 2023-09-22 16:20:43.000000 opentraveldata-0.0.9.post2/pyproject.toml
--rw-r--r--   0 DENIS      (502)     1000     5352 2023-09-22 15:53:00.000000 opentraveldata-0.0.9.post2/requirements-dev.txt
--rw-r--r--   0 DENIS      (502)     1000      174 2023-09-22 15:47:59.000000 opentraveldata-0.0.9.post2/requirements.txt
-drwxr-xr-x   0 DENIS      (502)     1000        0 2023-09-22 16:20:56.435362 opentraveldata-0.0.9.post2/resources/
--rwxr-xr-x   0 DENIS      (502)     1000     1507 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/resources/optd-publish-por.sh
--rw-r--r--   0 DENIS      (502)     1000       38 2023-09-22 16:20:56.438450 opentraveldata-0.0.9.post2/setup.cfg
--rw-r--r--   0 DENIS      (502)     1000       39 2023-09-22 16:02:58.000000 opentraveldata-0.0.9.post2/setup.py
--rwxr-xr-x   0 DENIS      (502)     1000      494 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/test_optd-csvwriter.py
--rwxr-xr-x   0 DENIS      (502)     1000     3161 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post2/test_optd-serving-por.py
--rw-r--r--   0 DENIS      (502)     1000      616 2023-09-22 15:55:30.000000 opentraveldata-0.0.9.post2/tox.ini
+drwxr-xr-x   0 DENIS      (502)     1000        0 2024-04-04 21:18:46.451174 opentraveldata-0.0.9.post3/
+-rw-r--r--   0 DENIS      (502)     1000    15925 2024-04-04 21:18:46.450286 opentraveldata-0.0.9.post3/PKG-INFO
+-rw-r--r--   0 DENIS      (502)     1000    15190 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post3/README.md
+drwxr-xr-x   0 DENIS      (502)     1000        0 2024-04-04 21:18:46.444983 opentraveldata-0.0.9.post3/opentraveldata/
+-rw-r--r--   0 DENIS      (502)     1000       91 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post3/opentraveldata/__init__.py
+-rw-r--r--   0 DENIS      (502)     1000      911 2021-11-14 11:17:53.000000 opentraveldata-0.0.9.post3/opentraveldata/csvwriter.py
+-rw-r--r--   0 DENIS      (502)     1000    36135 2024-04-04 21:16:22.000000 opentraveldata-0.0.9.post3/opentraveldata/opentraveldata.py
+drwxr-xr-x   0 DENIS      (502)     1000        0 2024-04-04 21:18:46.449268 opentraveldata-0.0.9.post3/opentraveldata.egg-info/
+-rw-r--r--   0 DENIS      (502)     1000    15925 2024-04-04 21:18:46.000000 opentraveldata-0.0.9.post3/opentraveldata.egg-info/PKG-INFO
+-rw-r--r--   0 DENIS      (502)     1000      273 2024-04-04 21:18:46.000000 opentraveldata-0.0.9.post3/opentraveldata.egg-info/SOURCES.txt
+-rw-r--r--   0 DENIS      (502)     1000        1 2024-04-04 21:18:46.000000 opentraveldata-0.0.9.post3/opentraveldata.egg-info/dependency_links.txt
+-rw-r--r--   0 DENIS      (502)     1000       15 2024-04-04 21:18:46.000000 opentraveldata-0.0.9.post3/opentraveldata.egg-info/top_level.txt
+-rw-r--r--   0 DENIS      (502)     1000     1412 2024-04-04 21:17:38.000000 opentraveldata-0.0.9.post3/pyproject.toml
+-rw-r--r--   0 DENIS      (502)     1000       38 2024-04-04 21:18:46.451278 opentraveldata-0.0.9.post3/setup.cfg
+-rw-r--r--   0 DENIS      (502)     1000       39 2023-09-22 16:02:58.000000 opentraveldata-0.0.9.post3/setup.py
```

### Comparing `opentraveldata-0.0.9.post2/PKG-INFO` & `opentraveldata-0.0.9.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentraveldata
-Version: 0.0.9.post2
+Version: 0.0.9.post3
 Summary: Simple Python wrapper for OpenTravelata (OPTD)
 Author-email: Denis Arnaud <denis.arnaud_fedora@m4x.org>
 Project-URL: homepage, https://github.com/opentraveldata/python-opentraveldata
 Project-URL: repository, https://github.com/opentraveldata/python-opentraveldata
 Project-URL: documentation, https://github.com/opentraveldata/python-opentraveldata
 Keywords: packaging,package,dependency,pyproject.toml,api,python,optd,opentraveldata
 Classifier: Topic :: Software Development
```

### Comparing `opentraveldata-0.0.9.post2/README.md` & `opentraveldata-0.0.9.post3/README.md`

 * *Files identical despite different names*

### Comparing `opentraveldata-0.0.9.post2/opentraveldata/csvwriter.py` & `opentraveldata-0.0.9.post3/opentraveldata/csvwriter.py`

 * *Files identical despite different names*

### Comparing `opentraveldata-0.0.9.post2/opentraveldata/opentraveldata.py` & `opentraveldata-0.0.9.post3/opentraveldata/opentraveldata.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,20 +349,20 @@
       """
        Check that the sizes of the downloaded data files are as expected.
       """
       # Retrieve the sizes of the data files (downloaded in a previous step)
       (optd_por_file_size, optd_unlc_file_size) = self.fileSizes()
 
       # Validate the size of the main (IATA/ICAO) POR file
-      if 4e7 <= optd_por_file_size <= 5e7:
+      if 4e7 <= optd_por_file_size <= 6e7:
          if self.verbose:
             print(
-               f"[Opentraveldata::validateFileSizes] File size of {self.local_iata_por_filepath} withing range (i.e., 40-50 MB)")
+               f"[Opentraveldata::validateFileSizes] File size of {self.local_iata_por_filepath} withing range (i.e., 40-60 MB)")
       else:
-         err_msg = f"[OpenTravelData::validateFileSizes] File size of {self.local_iata_por_filepath} not within range (expected to be 40-50 MB)"
+         err_msg = f"[OpenTravelData::validateFileSizes] File size of {self.local_iata_por_filepath} not within range (expected to be 40-60 MB)"
          raise OPTDDownloadedFileSizeError(err_msg)
 
       # Validate the size of the OPTD UN/LOCODE POR file
       if 4e6 <= optd_unlc_file_size <= 5e6:
          if self.verbose:
             print (f"[Opentraveldata::validateFileSizes] File size of {self.local_unlc_por_filepath} withing range (i.e., 4-5 MB)")
       else:
```

### Comparing `opentraveldata-0.0.9.post2/opentraveldata.egg-info/PKG-INFO` & `opentraveldata-0.0.9.post3/opentraveldata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentraveldata
-Version: 0.0.9.post2
+Version: 0.0.9.post3
 Summary: Simple Python wrapper for OpenTravelata (OPTD)
 Author-email: Denis Arnaud <denis.arnaud_fedora@m4x.org>
 Project-URL: homepage, https://github.com/opentraveldata/python-opentraveldata
 Project-URL: repository, https://github.com/opentraveldata/python-opentraveldata
 Project-URL: documentation, https://github.com/opentraveldata/python-opentraveldata
 Keywords: packaging,package,dependency,pyproject.toml,api,python,optd,opentraveldata
 Classifier: Topic :: Software Development
```

### Comparing `opentraveldata-0.0.9.post2/pyproject.toml` & `opentraveldata-0.0.9.post3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opentraveldata"
-version = "0.0.9.post2"
+version = "0.0.9.post3"
 description = "Simple Python wrapper for OpenTravelata (OPTD)"
 authors = [
 	{name = "Denis Arnaud", email = "denis.arnaud_fedora@m4x.org"},
 ]
 readme = "README.md"
 keywords = ["packaging", "package", "dependency", "pyproject.toml",
          "api", "python", "optd", "opentraveldata"]
@@ -29,15 +29,14 @@
 
 [dev-dependencies]
 
 
 [build-system]
 requires = [
     "setuptools >= 35.0.2",
-    "setuptools_scm >= 2.0.0, <3"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 80
 target_version = ['py311']
 include = '\.pyi?$'
```

