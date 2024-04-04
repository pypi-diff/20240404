# Comparing `tmp/molecularnetwork-0.3.4.tar.gz` & `tmp/molecularnetwork-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularnetwork-0.3.4.tar", last modified: Thu Mar 14 18:24:35 2024, max compression
+gzip compressed data, was "molecularnetwork-0.3.5.tar", last modified: Thu Apr  4 12:54:06 2024, max compression
```

## Comparing `molecularnetwork-0.3.4.tar` & `molecularnetwork-0.3.5.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-03-14 18:24:35.764002 molecularnetwork-0.3.4/
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-03-14 18:24:35.758633 molecularnetwork-0.3.4/.github/
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-03-14 18:24:35.759974 molecularnetwork-0.3.4/.github/workflows/
--rw-r--r--   0 manasmahale   (501) staff       (20)     1087 2023-12-23 11:37:35.000000 molecularnetwork-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.4/.gitignore
--rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.4/LICENSE
--rw-r--r--   0 manasmahale   (501) staff       (20)     2191 2024-03-14 18:24:35.763809 molecularnetwork-0.3.4/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)     1768 2024-03-14 18:09:27.000000 molecularnetwork-0.3.4/README.md
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-03-14 18:24:35.760767 molecularnetwork-0.3.4/molecularnetwork/
--rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.4/molecularnetwork/__init__.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.4/molecularnetwork/featurizer.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     2627 2024-03-14 18:06:46.000000 molecularnetwork-0.3.4/molecularnetwork/graph.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.4/molecularnetwork/similarity.py
--rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.4/molecularnetwork/utils.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-03-14 18:24:35.763574 molecularnetwork-0.3.4/molecularnetwork.egg-info/
--rw-r--r--   0 manasmahale   (501) staff       (20)     2191 2024-03-14 18:24:35.000000 molecularnetwork-0.3.4/molecularnetwork.egg-info/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)      478 2024-03-14 18:24:35.000000 molecularnetwork-0.3.4/molecularnetwork.egg-info/SOURCES.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-03-14 18:24:35.000000 molecularnetwork-0.3.4/molecularnetwork.egg-info/dependency_links.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-03-14 18:24:35.000000 molecularnetwork-0.3.4/molecularnetwork.egg-info/requires.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-03-14 18:24:35.000000 molecularnetwork-0.3.4/molecularnetwork.egg-info/top_level.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.4/requirements.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-03-14 18:24:35.764039 molecularnetwork-0.3.4/setup.cfg
--rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-03-14 18:08:07.000000 molecularnetwork-0.3.4/setup.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-03-14 18:24:35.763304 molecularnetwork-0.3.4/test/
--rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.4/test/test.csv
--rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.4/test/test.gpickle
--rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.4/test/test.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-04 12:54:06.120922 molecularnetwork-0.3.5/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.5/.gitignore
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.5/LICENSE
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2191 2024-04-04 12:54:06.120725 molecularnetwork-0.3.5/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1768 2024-03-14 18:27:39.000000 molecularnetwork-0.3.5/README.md
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-04 12:54:06.117354 molecularnetwork-0.3.5/molecularnetwork/
+-rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/molecularnetwork/__init__.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/molecularnetwork/featurizer.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2643 2024-04-04 12:45:51.000000 molecularnetwork-0.3.5/molecularnetwork/graph.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/molecularnetwork/similarity.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/molecularnetwork/utils.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-04 12:54:06.120489 molecularnetwork-0.3.5/molecularnetwork.egg-info/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2191 2024-04-04 12:54:05.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)      441 2024-04-04 12:54:06.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-04 12:54:05.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-04 12:54:05.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/requires.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-04 12:54:05.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/top_level.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.5/requirements.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-04 12:54:06.120964 molecularnetwork-0.3.5/setup.cfg
+-rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-04 12:52:49.000000 molecularnetwork-0.3.5/setup.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-04 12:54:06.120220 molecularnetwork-0.3.5/test/
+-rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.5/test/test.csv
+-rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/test/test.gpickle
+-rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/test/test.py
```

### Comparing `molecularnetwork-0.3.4/.gitignore` & `molecularnetwork-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.4/LICENSE` & `molecularnetwork-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.4/PKG-INFO` & `molecularnetwork-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.3.4
+Version: 0.3.5
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -48,15 +48,15 @@
 # Generate the molecular network graph
 graph = network.create_graph(smiles_list, classes) # network.get_graph() also returns graph
 
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
-grpah = network.read_graph("test_molecular_network.joblib")
+graph = network.read_graph("test_molecular_network.joblib")
 ```
 
 ## Contributing
 If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request. I welcome contributions from the community.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `molecularnetwork-0.3.4/README.md` & `molecularnetwork-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # Generate the molecular network graph
 graph = network.create_graph(smiles_list, classes) # network.get_graph() also returns graph
 
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
-grpah = network.read_graph("test_molecular_network.joblib")
+graph = network.read_graph("test_molecular_network.joblib")
 ```
 
 ## Contributing
 If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request. I welcome contributions from the community.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `molecularnetwork-0.3.4/molecularnetwork/featurizer.py` & `molecularnetwork-0.3.5/molecularnetwork/featurizer.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.4/molecularnetwork/graph.py` & `molecularnetwork-0.3.5/molecularnetwork/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def _add_edges(self, fps):
         num_nodes = len(fps)
         for i in range(num_nodes):
             for j in range(i + 1, num_nodes):
                 sim_val = self._calculate_similarity(fps[i], fps[j])
                 if sim_val > self.sim_threshold:
-                    self.graph.add_edge(i, j)
+                    self.graph.add_edge(i, j, weight=sim_val)
 
     def _calculate_similarity(self, fp1, fp2):
         return self.similarity_calculator.calculate_similarity(fp1, fp2)
 
     def create_graph(self, smiles_list, classes):
         self._create_graph(smiles_list, classes)
         return self.graph
```

### Comparing `molecularnetwork-0.3.4/molecularnetwork/similarity.py` & `molecularnetwork-0.3.5/molecularnetwork/similarity.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.4/molecularnetwork.egg-info/PKG-INFO` & `molecularnetwork-0.3.5/molecularnetwork.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.3.4
+Version: 0.3.5
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -48,15 +48,15 @@
 # Generate the molecular network graph
 graph = network.create_graph(smiles_list, classes) # network.get_graph() also returns graph
 
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
-grpah = network.read_graph("test_molecular_network.joblib")
+graph = network.read_graph("test_molecular_network.joblib")
 ```
 
 ## Contributing
 If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request. I welcome contributions from the community.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `molecularnetwork-0.3.4/setup.py` & `molecularnetwork-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="molecularnetwork",
-    version="0.3.4",
+    version="0.3.5",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "networkx",
         "rdkit",
         "joblib",
     ],
```

### Comparing `molecularnetwork-0.3.4/test/test.csv` & `molecularnetwork-0.3.5/test/test.csv`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.4/test/test.gpickle` & `molecularnetwork-0.3.5/test/test.gpickle`

 * *Files identical despite different names*

