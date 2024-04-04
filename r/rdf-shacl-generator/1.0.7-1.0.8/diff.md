# Comparing `tmp/rdf_shacl_generator-1.0.7.tar.gz` & `tmp/rdf_shacl_generator-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdf_shacl_generator-1.0.7.tar", last modified: Sat Mar 30 12:26:19 2024, max compression
+gzip compressed data, was "rdf_shacl_generator-1.0.8.tar", last modified: Thu Apr  4 19:18:52 2024, max compression
```

## Comparing `rdf_shacl_generator-1.0.7.tar` & `rdf_shacl_generator-1.0.8.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:26:19.581791 rdf_shacl_generator-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-30 12:26:19.581791 rdf_shacl_generator-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:26:19.577791 rdf_shacl_generator-1.0.7/rdf_shacl_generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:26:19.581791 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/book_awards.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/book_genre.csv
--rw-r--r--   0 runner    (1001) docker     (127)   392144 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/book_titles.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35576 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/female_first_name.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/job_title.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/male_first_name.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/movie_awards.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/movie_genre.csv
--rw-r--r--   0 runner    (1001) docker     (127)   810581 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/movie_titles.csv
--rw-r--r--   0 runner    (1001) docker     (127)    31783 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/street_name.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/surnames.csv
--rw-r--r--   0 runner    (1001) docker     (127)   165690 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/tvseries_titles.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/rdf_graph_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/shacl_mapping_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17698 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator/value_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:26:19.577791 rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-30 12:26:19.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-30 12:26:19.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 12:26:19.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-30 12:26:19.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-30 12:26:19.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-30 12:26:19.000000 rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 12:26:19.581791 rdf_shacl_generator-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-30 12:26:08.000000 rdf_shacl_generator-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:52.023605 rdf_shacl_generator-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-04 19:18:52.023605 rdf_shacl_generator-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:52.019605 rdf_shacl_generator-1.0.8/rdf_shacl_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:52.023605 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/book_awards.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/book_genre.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   392144 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/book_titles.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35576 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/female_first_name.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/job_title.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/male_first_name.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/movie_awards.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/movie_genre.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   810581 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/movie_titles.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31783 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/street_name.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/surnames.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   165690 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/tvseries_titles.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/rdf_graph_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/shacl_mapping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17698 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator/value_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:18:52.019605 rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-04 19:18:51.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-04 19:18:51.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:18:51.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 19:18:51.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-04 19:18:51.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 19:18:51.000000 rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:18:52.023605 rdf_shacl_generator-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-04 19:18:43.000000 rdf_shacl_generator-1.0.8/setup.py
```

### Comparing `rdf_shacl_generator-1.0.7/PKG-INFO` & `rdf_shacl_generator-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf_shacl_generator
-Version: 1.0.7
+Version: 1.0.8
 Summary: Synthetic RDF graph generator based on SHACL constraints.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: 
         # Synthetic RDF graph generator based on SHACL constraints.
         
         ### rdf_shacl_generator is a Python package that can be used to generate RDF graphs based on SHACL constraints.
```

### Comparing `rdf_shacl_generator-1.0.7/README.md` & `rdf_shacl_generator-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/book_genre.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/book_genre.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/book_titles.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/book_titles.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/female_first_name.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/female_first_name.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/job_title.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/job_title.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/male_first_name.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/male_first_name.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/movie_awards.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/movie_awards.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/movie_genre.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/movie_genre.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/movie_titles.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/movie_titles.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/street_name.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/street_name.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/surnames.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/surnames.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/datasets/tvseries_titles.csv` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/datasets/tvseries_titles.csv`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/rdf_graph_generator.py` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/rdf_graph_generator.py`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/script.py` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/script.py`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/shacl_mapping_generator.py` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/shacl_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator/value_generators.py` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator/value_generators.py`

 * *Files identical despite different names*

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/PKG-INFO` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-shacl-generator
-Version: 1.0.7
+Version: 1.0.8
 Summary: Synthetic RDF graph generator based on SHACL constraints.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: 
         # Synthetic RDF graph generator based on SHACL constraints.
         
         ### rdf_shacl_generator is a Python package that can be used to generate RDF graphs based on SHACL constraints.
```

### Comparing `rdf_shacl_generator-1.0.7/rdf_shacl_generator.egg-info/SOURCES.txt` & `rdf_shacl_generator-1.0.8/rdf_shacl_generator.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 rdf_shacl_generator/__init__.py
 rdf_shacl_generator/rdf_graph_generator.py
 rdf_shacl_generator/script.py
 rdf_shacl_generator/shacl_mapping_generator.py
 rdf_shacl_generator/value_generators.py
```

### Comparing `rdf_shacl_generator-1.0.7/setup.py` & `rdf_shacl_generator-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md') as f:
     description = f.read()
 
 setup(
     name='rdf_shacl_generator',
-    version='1.0.7',
+    version='1.0.8',
     description = 'Synthetic RDF graph generator based on SHACL constraints.',
     long_description = description,
     long_description_content_type = 'text/markdown',
     packages=find_packages(),
     package_data={'rdf_shacl_generator': ['datasets/*.csv']},
     install_requires=requirements,
     entry_points={
```

