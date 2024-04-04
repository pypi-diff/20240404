# Comparing `tmp/tree-math-0.2.0.tar.gz` & `tmp/tree-math-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-math-0.2.0.tar", last modified: Thu May 18 17:47:46 2023, max compression
+gzip compressed data, was "tree-math-0.2.1.tar", last modified: Thu Apr  4 00:58:42 2024, max compression
```

## Comparing `tree-math-0.2.0.tar` & `tree-math-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-18 17:47:46.271663 tree-math-0.2.0/
--rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-12-28 20:41:50.000000 tree-math-0.2.0/LICENSE
--rw-r--r--   0 shoyer   (365133) eng       (5000)      314 2023-05-18 17:47:46.270984 tree-math-0.2.0/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5943 2023-05-12 02:20:53.000000 tree-math-0.2.0/README.md
--rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2023-05-18 17:47:46.271714 tree-math-0.2.0/setup.cfg
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1243 2023-05-18 17:46:01.000000 tree-math-0.2.0/setup.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-18 17:47:46.267791 tree-math-0.2.0/tree_math/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      886 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/__init__.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-18 17:47:46.270744 tree-math-0.2.0/tree_math/_src/
--rw-r--r--   0 shoyer   (365133) eng       (5000)        0 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2720 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/arg_util.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2686 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/func_wrappers.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2846 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/func_wrappers_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1350 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/numpy.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2961 2022-03-04 04:00:56.000000 tree-math-0.2.0/tree_math/_src/numpy_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2408 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/_src/structs.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3639 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/_src/structs_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1939 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/_src/test_util.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     7209 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/_src/vector.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6211 2023-05-12 02:20:53.000000 tree-math-0.2.0/tree_math/_src/vector_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2681 2021-12-28 23:13:05.000000 tree-math-0.2.0/tree_math/integration_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)      836 2021-12-28 20:41:50.000000 tree-math-0.2.0/tree_math/numpy.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-18 17:47:46.268569 tree-math-0.2.0/tree_math.egg-info/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      314 2023-05-18 17:47:45.000000 tree-math-0.2.0/tree_math.egg-info/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)      577 2023-05-18 17:47:46.000000 tree-math-0.2.0/tree_math.egg-info/SOURCES.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2023-05-18 17:47:46.000000 tree-math-0.2.0/tree_math.egg-info/dependency_links.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)       47 2023-05-18 17:47:46.000000 tree-math-0.2.0/tree_math.egg-info/requires.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)       10 2023-05-18 17:47:46.000000 tree-math-0.2.0/tree_math.egg-info/top_level.txt
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-04-04 00:58:42.626335 tree-math-0.2.1/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-12-28 20:41:50.000000 tree-math-0.2.1/LICENSE
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      471 2024-04-04 00:58:42.626104 tree-math-0.2.1/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5943 2023-05-12 02:20:53.000000 tree-math-0.2.1/README.md
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2024-04-04 00:58:42.626387 tree-math-0.2.1/setup.cfg
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1242 2024-04-04 00:56:21.000000 tree-math-0.2.1/setup.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-04-04 00:58:42.622376 tree-math-0.2.1/tree_math/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      886 2024-04-04 00:56:21.000000 tree-math-0.2.1/tree_math/__init__.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-04-04 00:58:42.625276 tree-math-0.2.1/tree_math/_src/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)        0 2021-12-28 20:41:50.000000 tree-math-0.2.1/tree_math/_src/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2720 2021-12-28 20:41:50.000000 tree-math-0.2.1/tree_math/_src/arg_util.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2686 2021-12-28 20:41:50.000000 tree-math-0.2.1/tree_math/_src/func_wrappers.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2846 2021-12-28 20:41:50.000000 tree-math-0.2.1/tree_math/_src/func_wrappers_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1350 2021-12-28 20:41:50.000000 tree-math-0.2.1/tree_math/_src/numpy.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2961 2022-03-04 04:00:56.000000 tree-math-0.2.1/tree_math/_src/numpy_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2464 2024-04-04 00:56:21.000000 tree-math-0.2.1/tree_math/_src/structs.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3826 2024-04-04 00:56:21.000000 tree-math-0.2.1/tree_math/_src/structs_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1939 2021-12-28 20:41:50.000000 tree-math-0.2.1/tree_math/_src/test_util.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     7209 2023-05-12 02:20:53.000000 tree-math-0.2.1/tree_math/_src/vector.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6211 2023-05-12 02:20:53.000000 tree-math-0.2.1/tree_math/_src/vector_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2681 2021-12-28 23:13:05.000000 tree-math-0.2.1/tree_math/integration_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      836 2021-12-28 20:41:50.000000 tree-math-0.2.1/tree_math/numpy.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-04-04 00:58:42.625599 tree-math-0.2.1/tree_math.egg-info/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      471 2024-04-04 00:58:42.000000 tree-math-0.2.1/tree_math.egg-info/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      577 2024-04-04 00:58:42.000000 tree-math-0.2.1/tree_math.egg-info/SOURCES.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2024-04-04 00:58:42.000000 tree-math-0.2.1/tree_math.egg-info/dependency_links.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       47 2024-04-04 00:58:42.000000 tree-math-0.2.1/tree_math.egg-info/requires.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       10 2024-04-04 00:58:42.000000 tree-math-0.2.1/tree_math.egg-info/top_level.txt
```

### Comparing `tree-math-0.2.0/LICENSE` & `tree-math-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/README.md` & `tree-math-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/setup.py` & `tree-math-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'numpy>=1.17',
     'pytest',
 ]
 
 setuptools.setup(
     name='tree-math',
     description='Mathematical operations for JAX pytrees',
-    version='0.2.0 ',
+    version='0.2.1',
     license='Apache 2.0',
     author='Google LLC',
     author_email='noreply@google.com',
     install_requires=base_requires,
     extras_require={
         'tests': tests_requires,
     },
```

### Comparing `tree-math-0.2.0/tree_math/__init__.py` & `tree-math-0.2.1/tree_math/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     wrap,
     unwrap,
 )
 from tree_math._src.structs import struct
 from tree_math._src.vector import Vector, VectorMixin
 import tree_math.numpy
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
```

### Comparing `tree-math-0.2.0/tree_math/_src/arg_util.py` & `tree-math-0.2.1/tree_math/_src/arg_util.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/_src/func_wrappers.py` & `tree-math-0.2.1/tree_math/_src/func_wrappers.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/_src/func_wrappers_test.py` & `tree-math-0.2.1/tree_math/_src/func_wrappers_test.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/_src/numpy.py` & `tree-math-0.2.1/tree_math/_src/numpy.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/_src/numpy_test.py` & `tree-math-0.2.1/tree_math/_src/numpy_test.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/_src/structs.py` & `tree-math-0.2.1/tree_math/_src/structs.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,11 +68,12 @@
     return cls(*children)
 
   cls_as_struct = type(cls.__name__,
                        (VectorMixin, dataclasses.dataclass(cls)),
                        {'fields': fields,
                         'asdict': asdict,
                         'astuple': astuple,
+                        'replace': dataclasses.replace,
                         'tree_flatten': tree_flatten,
                         'tree_unflatten': tree_unflatten,
                         '__module__': cls.__module__})
   return jax.tree_util.register_pytree_node_class(cls_as_struct)
```

### Comparing `tree-math-0.2.0/tree_math/_src/structs_test.py` & `tree-math-0.2.1/tree_math/_src/structs_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,10 +105,16 @@
     np.testing.assert_allclose(jitted.b, unjitted.b)
 
   def testPickle(self):
     struct = TestStruct(1, 2)
     restored = pickle.loads(pickle.dumps(struct))
     self.assertTreeEqual(struct, restored, check_dtypes=True)
 
+  def testReplace(self):
+    struct = TestStruct(1, 2)
+    replaced = struct.replace(b=3)
+    expected = TestStruct(1, 3)
+    self.assertTreeEqual(replaced, expected, check_dtypes=True)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tree-math-0.2.0/tree_math/_src/test_util.py` & `tree-math-0.2.1/tree_math/_src/test_util.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/_src/vector.py` & `tree-math-0.2.1/tree_math/_src/vector.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/_src/vector_test.py` & `tree-math-0.2.1/tree_math/_src/vector_test.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/integration_test.py` & `tree-math-0.2.1/tree_math/integration_test.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math/numpy.py` & `tree-math-0.2.1/tree_math/numpy.py`

 * *Files identical despite different names*

### Comparing `tree-math-0.2.0/tree_math.egg-info/SOURCES.txt` & `tree-math-0.2.1/tree_math.egg-info/SOURCES.txt`

 * *Files identical despite different names*

