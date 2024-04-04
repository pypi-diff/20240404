# Comparing `tmp/pyscal_rdf-0.1.7.tar.gz` & `tmp/pyscal_rdf-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal_rdf-0.1.7.tar", last modified: Wed Apr  3 08:59:32 2024, max compression
+gzip compressed data, was "pyscal_rdf-0.2.3.tar", last modified: Thu Apr  4 10:44:37 2024, max compression
```

## Comparing `pyscal_rdf-0.1.7.tar` & `pyscal_rdf-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.851282 pyscal_rdf-0.1.7/pyscal_rdf/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.851282 pyscal_rdf-0.1.7/pyscal_rdf/data/
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/asmo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/cmso.owl
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/element.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/pldo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/podo.owl
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    39539 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/json_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.851282 pyscal_rdf-0.1.7/pyscal_rdf/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/rdfsystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.357071 pyscal_rdf-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.349072 pyscal_rdf-0.2.3/pyscal_rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/pyscal_rdf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/asmo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/cmso.owl
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/pldo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/podo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18815 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/json_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/pyscal_rdf/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27466 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:44:37.357071 pyscal_rdf-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/tests/test_structuregraph.py
```

### Comparing `pyscal_rdf-0.1.7/LICENSE` & `pyscal_rdf-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/PKG-INFO` & `pyscal_rdf-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal_rdf
-Version: 0.1.7
+Version: 0.2.3
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal_rdf-0.1.7/README.md` & `pyscal_rdf-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/data/asmo.owl` & `pyscal_rdf-0.2.3/pyscal_rdf/data/asmo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/data/cmso.owl` & `pyscal_rdf-0.2.3/pyscal_rdf/data/cmso.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/data/element.yml` & `pyscal_rdf-0.2.3/pyscal_rdf/data/element.yml`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/data/pldo.owl` & `pyscal_rdf-0.2.3/pyscal_rdf/data/pldo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/data/podo.owl` & `pyscal_rdf-0.2.3/pyscal_rdf/data/podo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/json_io.py` & `pyscal_rdf-0.2.3/pyscal_rdf/json_io.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/network/network.py` & `pyscal_rdf-0.2.3/pyscal_rdf/network/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         select_destinations = [f'?{self.strip_name(destination)}' for destination in destination_names]
         query.append(f'SELECT DISTINCT {" ".join(select_destinations)}')
         query.append("WHERE {")
         
         #now add corresponding triples
         for destination in destination_names:
             for triple in all_triplets[destination]:
-                print(triple)
+                #print(triple)
                 query.append("    ?%s %s ?%s ."%(self.strip_name(triple[0]), 
                                                  triple[1], 
                                                  self.strip_name(triple[2])))
         
         #we enforce types of the source and destination
         if enforce_types:
             if source.node_type == 'class':
```

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/network/ontology.py` & `pyscal_rdf-0.2.3/pyscal_rdf/network/ontology.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/network/parser.py` & `pyscal_rdf-0.2.3/pyscal_rdf/network/parser.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/network/patch.py` & `pyscal_rdf-0.2.3/pyscal_rdf/network/patch.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/network/term.py` & `pyscal_rdf-0.2.3/pyscal_rdf/network/term.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/properties.py` & `pyscal_rdf-0.2.3/pyscal_rdf/properties.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf/workflow.py` & `pyscal_rdf-0.2.3/pyscal_rdf/workflow.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf.egg-info/PKG-INFO` & `pyscal_rdf-0.2.3/pyscal_rdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal_rdf
-Version: 0.1.7
+Version: 0.2.3
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal_rdf-0.1.7/pyscal_rdf.egg-info/SOURCES.txt` & `pyscal_rdf-0.2.3/pyscal_rdf.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 setup.py
 pyscal_rdf/__init__.py
 pyscal_rdf/encoder.py
 pyscal_rdf/graph.py
 pyscal_rdf/json_io.py
 pyscal_rdf/properties.py
-pyscal_rdf/rdfsystem.py
 pyscal_rdf/structure.py
 pyscal_rdf/visualize.py
 pyscal_rdf/workflow.py
 pyscal_rdf.egg-info/PKG-INFO
 pyscal_rdf.egg-info/SOURCES.txt
 pyscal_rdf.egg-info/dependency_links.txt
 pyscal_rdf.egg-info/not-zip-safe
```

### Comparing `pyscal_rdf-0.1.7/setup.py` & `pyscal_rdf-0.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal_rdf',
-    version='0.1.7',
+    version='0.2.3',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['pyscal_rdf', 'pyscal_rdf.*']),
     zip_safe=False,
```

### Comparing `pyscal_rdf-0.1.7/tests/test_encoder_and_write.py` & `pyscal_rdf-0.2.3/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.7/tests/test_graph.py` & `pyscal_rdf-0.2.3/tests/test_graph.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pytest
-from pyscal_rdf import StructureGraph
+from pyscal_rdf import KnowledgeGraph, System
 
 def test_structuregraph():
-	s = StructureGraph()
-	sys = s.create.element.Fe()
+	s = KnowledgeGraph()
+	sys = System.create.element.Fe(graph=s)
 
 	vis = s.visualise()
 	assert(vis != None)
 
-	vis = s.visualise(styledict={"BNode":{"fontsize":10}})
+	vis = s.visualise()
 	assert(vis != None)
 
 	s.write("temp.ttl", format="turtle")
-	s = StructureGraph(graph_file="temp.ttl")
+	s = KnowledgeGraph(graph_file="temp.ttl")
 
-	sys = s.create.element.Fe()
-	s.add_vacancy(0.5, number=1)
+	sys = System.create.element.Fe(graph=s)
+	sys.add_vacancy(0.5, number=1)
 
-	s = StructureGraph()
-	sys = s.create.element.Fe()
+	s = KnowledgeGraph()
+	sys = System.create.element.Fe(graph=s)
+	assert s.n_samples == 1
 	#res = s.query_sample("NumberOfAtoms", 2)
 	#assert(len(res) == 1)
```

