# Comparing `tmp/pygmtools-0.5.0.tar.gz` & `tmp/pygmtools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.5.0.tar", last modified: Tue Feb 20 16:26:14 2024, max compression
+gzip compressed data, was "pygmtools-0.5.1.tar", last modified: Wed Apr  3 23:16:29 2024, max compression
```

## Comparing `pygmtools-0.5.0.tar` & `pygmtools-0.5.1.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:26:14.047690 pygmtools-0.5.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)      508 2024-02-20 16:26:00.000000 pygmtools-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-20 16:26:00.000000 pygmtools-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-02-20 16:26:14.047690 pygmtools-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-02-20 16:26:00.000000 pygmtools-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:26:14.043690 pygmtools-0.5.0/pygmtools/
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26415 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    53433 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/classic_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    58887 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    59923 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/jittor_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/jittor_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    75822 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/linear_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21672 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/mindspore_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    43957 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/multi_graph_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    81238 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/neural_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    61477 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/numpy_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    59058 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/paddle_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/paddle_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/pytorch_astar_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    62804 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/pytorch_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    23331 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/tensorflow_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    74985 2024-02-20 16:26:01.000000 pygmtools-0.5.0/pygmtools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:26:14.047690 pygmtools-0.5.0/pygmtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-02-20 16:26:14.000000 pygmtools-0.5.0/pygmtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-20 16:26:14.000000 pygmtools-0.5.0/pygmtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:26:14.000000 pygmtools-0.5.0/pygmtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-20 16:26:14.000000 pygmtools-0.5.0/pygmtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-20 16:26:14.000000 pygmtools-0.5.0/pygmtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:26:14.047690 pygmtools-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-02-20 16:26:01.000000 pygmtools-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:26:14.047690 pygmtools-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-02-20 16:26:01.000000 pygmtools-0.5.0/tests/test_classic_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-02-20 16:26:01.000000 pygmtools-0.5.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-02-20 16:26:01.000000 pygmtools-0.5.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-02-20 16:26:01.000000 pygmtools-0.5.0/tests/test_multi_graph_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13700 2024-02-20 16:26:01.000000 pygmtools-0.5.0/tests/test_neural_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-20 16:26:01.000000 pygmtools-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      508 2024-04-03 23:16:20.000000 pygmtools-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 23:16:20.000000 pygmtools-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-04-03 23:16:29.978067 pygmtools-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-04-03 23:16:20.000000 pygmtools-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/pygmtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26430 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/pygmtools/c_astar_src/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/c_astar_src/build_c_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/c_astar_src/c_astar.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/c_astar_src/c_astar_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/c_astar_src/priority_queue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    53433 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/classic_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59047 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59923 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/jittor_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/jittor_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75822 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/linear_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21672 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/mindspore_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43957 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/multi_graph_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81238 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/neural_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61477 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/numpy_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59058 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/paddle_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/paddle_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/pytorch_astar_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62804 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/pytorch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23331 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/tensorflow_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74983 2024-04-03 23:16:20.000000 pygmtools-0.5.1/pygmtools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/pygmtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15977 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 23:16:29.000000 pygmtools-0.5.1/pygmtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:16:29.978067 pygmtools-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-03 23:16:20.000000 pygmtools-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:16:29.978067 pygmtools-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_classic_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_multi_graph_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13700 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_neural_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-03 23:16:20.000000 pygmtools-0.5.1/tests/test_utils.py
```

### Comparing `pygmtools-0.5.0/PKG-INFO` & `pygmtools-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.5.0
+Version: 0.5.1
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmtools-0.5.0/README.md` & `pygmtools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/__init__.py` & `pygmtools-0.5.1/pygmtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm, genn_astar
 import pygmtools.utils as utils
 import importlib.util
 set_backend = utils.set_backend
 
 BACKEND = 'numpy'
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 __author__ = 'ThinkLab at SJTU'
 
 SUPPORTED_BACKENDS = [
     'numpy',
     'pytorch',
     'jittor',
     'paddle',
```

### Comparing `pygmtools-0.5.0/pygmtools/benchmark.py` & `pygmtools-0.5.1/pygmtools/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self.filter = filter
         self.sets = sets
         self.obj_resize = obj_resize
 
         data_set = eval(self.name)(self.sets, self.obj_resize, **args)
         suffix = data_set.suffix
         self.data_path = os.path.join(data_set.dataset_dir, 'data-' + str(self.obj_resize) + '-' + suffix + '.json')
-        self.data_list_path = os.path.join(data_set.dataset_dir, sets + '.json')
+        self.data_list_path = os.path.join(data_set.dataset_dir, sets + '-' + suffix + '.json')
         self.classes = data_set.classes
 
         with open(self.data_path) as f:
             self.data_dict = json.load(f)
 
         if self.sets == 'test':
             tmpfile = tempfile.gettempdir()
```

### Comparing `pygmtools-0.5.0/pygmtools/classic_solvers.py` & `pygmtools-0.5.1/pygmtools/classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/dataset.py` & `pygmtools-0.5.1/pygmtools/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,16 +306,16 @@
                 a_xml_list[cls_id].remove(x)
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
-        train_file = os.path.join(self.dataset_dir, 'train.json')
-        test_file = os.path.join(self.dataset_dir, 'test.json')
+        train_file = os.path.join(self.dataset_dir, 'train-' + self.suffix + '.json')
+        test_file = os.path.join(self.dataset_dir, 'test-' + self.suffix + '.json')
         img_file = os.path.join(self.dataset_dir, 'data-' + str(self.obj_resize) + '-' + self.suffix + '.json')
         if not (os.path.exists(train_file) and os.path.exists(test_file) and os.path.exists(img_file)):
             if not (os.path.exists(train_file) and os.path.exists(test_file)):
                 list1 = []
                 for x in range(len(self.xml_list)):
                     for xml_name in self.xml_list[x]:
                         tmp = xml_name.split('/')
@@ -560,16 +560,16 @@
         return filename
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
-        train_file = os.path.join(self.dataset_dir, 'train.json')
-        test_file = os.path.join(self.dataset_dir, 'test.json')
+        train_file = os.path.join(self.dataset_dir, 'train-' + self.suffix + '.json')
+        test_file = os.path.join(self.dataset_dir, 'test-' + self.suffix + '.json')
         img_file = os.path.join(self.dataset_dir, 'data-' + str(self.obj_resize) + '-' + self.suffix + '.json')
 
         data_list = []
         mat_list_ = []
         for cls_name in self.classes:
             assert type(cls_name) is str
             cls_mat_list = [p for p in (self.root_path / cls_name).glob('*.mat')]
@@ -846,16 +846,16 @@
         return filename
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
-        train_file = os.path.join(self.dataset_dir, 'train.json')
-        test_file = os.path.join(self.dataset_dir, 'test.json')
+        train_file = os.path.join(self.dataset_dir, 'train-' + self.suffix + '.json')
+        test_file = os.path.join(self.dataset_dir, 'test-' + self.suffix + '.json')
         img_file = os.path.join(self.dataset_dir, 'data-' + str(self.obj_resize) + '-' + self.suffix + '.json')
         if (not os.path.exists(train_file)) or (not os.path.exists(test_file)) or (not os.path.exists(img_file)):
             train_list = []
             test_list = []
             if self.sets == 'trn':
                 for x in self.ann_files_filtered:
                     tmp = x.split('-')
@@ -1100,15 +1100,15 @@
         return filename
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
-        set_file = os.path.join(self.dataset_dir, self.sets + '.json')
+        set_file = os.path.join(self.dataset_dir, self.sets + '-' + self.suffix + '.json')
         img_file = os.path.join(self.dataset_dir, 'data-' + str(self.obj_resize) + '-' + self.suffix + '.json')
 
         if not os.path.exists(set_file):
             set_list = []
             for _list in self.img_lists:
                 for img_name in _list:
                     set_list.append(img_name.split('.')[0])
@@ -1297,15 +1297,15 @@
         return filename
 
     def process(self):
         r"""
         Process the dataset and generate ``data-(size, size).json`` for preprocessed dataset, ``train.json`` for
         training set, and ``test.json`` for testing set.
         """
-        set_file = os.path.join(self.dataset_dir, self.sets + '.json')
+        set_file = os.path.join(self.dataset_dir, self.sets + '-' + self.suffix + '.json')
         img_file = os.path.join(self.dataset_dir, 'data-' + str(self.obj_resize) + '-' + self.suffix + '.json')
 
         if not os.path.exists(set_file):
             set_list = []
             set_img_idx_list = self.set_data[self.sets]
             for cls_img_idx_list in set_img_idx_list:
                 for img_idx in cls_img_idx_list:
```

### Comparing `pygmtools-0.5.0/pygmtools/dataset_config.py` & `pygmtools-0.5.1/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/jittor_backend.py` & `pygmtools-0.5.1/pygmtools/jittor_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/jittor_modules.py` & `pygmtools-0.5.1/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/linear_solvers.py` & `pygmtools-0.5.1/pygmtools/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/mindspore_backend.py` & `pygmtools-0.5.1/pygmtools/mindspore_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/multi_graph_solvers.py` & `pygmtools-0.5.1/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/neural_solvers.py` & `pygmtools-0.5.1/pygmtools/neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/numpy_backend.py` & `pygmtools-0.5.1/pygmtools/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/numpy_modules.py` & `pygmtools-0.5.1/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/paddle_backend.py` & `pygmtools-0.5.1/pygmtools/paddle_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/paddle_modules.py` & `pygmtools-0.5.1/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/pytorch_astar_modules.py` & `pygmtools-0.5.1/pygmtools/pytorch_astar_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/pytorch_backend.py` & `pygmtools-0.5.1/pygmtools/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/pytorch_modules.py` & `pygmtools-0.5.1/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/tensorflow_backend.py` & `pygmtools-0.5.1/pygmtools/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/pygmtools/utils.py` & `pygmtools-0.5.1/pygmtools/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1602,15 +1602,15 @@
                     [0. , 0. , 0.6, 0. , 0. ],
                     [0. , 0. , 0. , 0.9, 0. ],
                     [0. , 0. , 0. , 0. , 0.4],
                     [0. , 0. , 0. , 0. , 0. ]])
             
     """
     is_directed = isinstance(G, nx.DiGraph)
-    adj_matrix = nx.to_numpy_matrix(G, nodelist=G.nodes()) if is_directed else nx.to_numpy_matrix(G)
+    adj_matrix = nx.to_numpy_array(G, nodelist=G.nodes()) if is_directed else nx.to_numpy_array(G)
     return adj_matrix
 
 
 def from_graphml(filename):
     r"""
     Convert graphml object to adjacency matrix
```

### Comparing `pygmtools-0.5.0/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.5.1/pygmtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.5.0
+Version: 0.5.1
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmtools-0.5.0/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.5.1/pygmtools.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -24,13 +24,17 @@
 pygmtools/tensorflow_modules.py
 pygmtools/utils.py
 pygmtools.egg-info/PKG-INFO
 pygmtools.egg-info/SOURCES.txt
 pygmtools.egg-info/dependency_links.txt
 pygmtools.egg-info/requires.txt
 pygmtools.egg-info/top_level.txt
+pygmtools/c_astar_src/build_c_astar.py
+pygmtools/c_astar_src/c_astar.pyx
+pygmtools/c_astar_src/c_astar_setup.py
+pygmtools/c_astar_src/priority_queue.hpp
 tests/test_classic_solvers.py
 tests/test_dataset.py
 tests/test_misc.py
 tests/test_multi_graph_solvers.py
 tests/test_neural_solvers.py
 tests/test_utils.py
```

### Comparing `pygmtools-0.5.0/setup.py` & `pygmtools-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 DESCRIPTION = 'pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. ' \
               'pygmtools also provides dataset API for standard graph matching benchmarks.'
 URL = 'https://pygmtools.readthedocs.io/'
 AUTHOR = get_property('__author__', NAME)
 VERSION = get_property('__version__', NAME)
 REQUIRED = [
      'requests>=2.25.1', 'scipy>=1.4.1', 'Pillow>=7.2.0', 'numpy>=1.18.5', 'easydict>=1.7', 'appdirs>=1.4.4', 'tqdm>=4.64.1', 
-     'async-timeout','aiohttp','networkx>=2.8.8'
+     'async-timeout', 'aiohttp', 'networkx>=2.8.8'
 ]
 EXTRAS = {}
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
@@ -48,15 +48,15 @@
         exec(f.read(), about)
 else:
     about['__version__'] = VERSION
  
     
 class BdistWheelCommand(_bdist_wheel):
     def run(self):
-        os.system("python pygmtools/c_astar/get_c_astar.py")
+        os.system("python pygmtools/c_astar_src/build_c_astar.py")
         super().run()
 
     def get_tag(self):
         if self.plat_name and not self.plat_name.startswith("macosx"):
             plat_name = self.plat_name
         else:
             plat_name = get_platform(self.bdist_dir)
@@ -70,30 +70,30 @@
         tag = (impl, abi_tag, plat_name)
         return tag
 
 
 class InstallCommand(_install):
     def run(self):
         try:
-            os.system("python pygmtools/c_astar/get_c_astar.py")
+            os.system("python pygmtools/c_astar_src/build_c_astar.py")
         except:
             pass
         _install.run(self)
            
       
 setup(
     name=NAME,
     version=about['__version__'],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    package_data={NAME: ['*.pyd', '*.so', 'astar/*']},
+    package_data={NAME: ['*.pyd', '*.so', 'c_astar_src/*']},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='Mulan PSL v2',
     python_requires='>=3.8',
     classifiers=[
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
```

### Comparing `pygmtools-0.5.0/tests/test_classic_solvers.py` & `pygmtools-0.5.1/tests/test_classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/tests/test_dataset.py` & `pygmtools-0.5.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/tests/test_misc.py` & `pygmtools-0.5.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/tests/test_multi_graph_solvers.py` & `pygmtools-0.5.1/tests/test_multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/tests/test_neural_solvers.py` & `pygmtools-0.5.1/tests/test_neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.5.0/tests/test_utils.py` & `pygmtools-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

