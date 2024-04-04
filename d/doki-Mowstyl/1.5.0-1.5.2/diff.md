# Comparing `tmp/doki-Mowstyl-1.5.0.tar.gz` & `tmp/doki_mowstyl-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doki-Mowstyl-1.5.0.tar", last modified: Fri Aug  4 16:52:18 2023, max compression
+gzip compressed data, was "doki_mowstyl-1.5.2.tar", last modified: Thu Apr  4 19:47:59 2024, max compression
```

## Comparing `doki-Mowstyl-1.5.0.tar` & `doki_mowstyl-1.5.2.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:52:18.616209 doki-Mowstyl-1.5.0/
--rw-rw-rw-   0        0        0     1111 2021-09-20 14:20:25.000000 doki-Mowstyl-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     1148 2023-08-04 16:52:18.616209 doki-Mowstyl-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      824 2021-09-15 23:16:12.000000 doki-Mowstyl-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 16:52:18.605209 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/
--rw-rw-rw-   0        0        0     1148 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-04 16:52:18.000000 doki-Mowstyl-1.5.0/doki_Mowstyl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2023-05-10 16:36:21.000000 doki-Mowstyl-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-04 16:52:18.616209 doki-Mowstyl-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2966 2023-08-04 16:44:51.000000 doki-Mowstyl-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:52:18.599209 doki-Mowstyl-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-04 16:52:18.615209 doki-Mowstyl-1.5.0/src/doki/
--rw-rw-rw-   0        0        0     1816 2023-07-21 13:17:38.000000 doki-Mowstyl-1.5.0/src/doki/arraylist.c
--rw-rw-rw-   0        0        0     1059 2023-07-21 13:17:34.000000 doki-Mowstyl-1.5.0/src/doki/arraylist.h
--rw-rw-rw-   0        0        0    73129 2023-07-27 20:22:54.000000 doki-Mowstyl-1.5.0/src/doki/doki.c
--rw-rw-rw-   0        0        0    35772 2023-08-04 11:43:53.000000 doki-Mowstyl-1.5.0/src/doki/funmatrix.c
--rw-rw-rw-   0        0        0     6219 2023-07-27 18:04:35.000000 doki-Mowstyl-1.5.0/src/doki/funmatrix.h
--rw-rw-rw-   0        0        0     1424 2023-07-27 11:20:10.000000 doki-Mowstyl-1.5.0/src/doki/platform.c
--rw-rw-rw-   0        0        0    10504 2023-07-27 19:54:26.000000 doki-Mowstyl-1.5.0/src/doki/platform.h
--rw-rw-rw-   0        0        0      336 2023-07-21 13:16:44.000000 doki-Mowstyl-1.5.0/src/doki/qgate.h
--rw-rw-rw-   0        0        0    19350 2023-07-27 21:22:31.000000 doki-Mowstyl-1.5.0/src/doki/qops.c
--rw-rw-rw-   0        0        0     2213 2023-07-27 17:55:06.000000 doki-Mowstyl-1.5.0/src/doki/qops.h
--rw-rw-rw-   0        0        0     3096 2023-07-21 13:17:25.000000 doki-Mowstyl-1.5.0/src/doki/qstate.c
--rw-rw-rw-   0        0        0     2344 2023-07-21 13:17:20.000000 doki-Mowstyl-1.5.0/src/doki/qstate.h
+-rw-rw-rw-   0        0        0     1919 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/.github/workflows/wheels.yml
+-rw-rw-rw-   0        0        0     1689 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/.gitignore
+-rw-rw-rw-   0        0        0    35507 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/LICENSE.md
+-rw-rw-rw-   0        0        0      824 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/README.md
+-rw-rw-rw-   0        0        0     1057 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/meson.build
+-rw-rw-rw-   0        0        0     1570 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0      382 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/_build_utils/version.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/__init__.py
+-rw-rw-rw-   0        0        0     2602 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/arraylist.c
+-rw-rw-rw-   0        0        0     1845 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/arraylist.h
+-rw-rw-rw-   0        0        0    75526 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/doki.c
+-rw-rw-rw-   0        0        0    39248 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/funmatrix.c
+-rw-rw-rw-   0        0        0     7191 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/funmatrix.h
+-rw-rw-rw-   0        0        0      255 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/meson.build
+-rw-rw-rw-   0        0        0     2210 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/platform.c
+-rw-rw-rw-   0        0        0    11298 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/platform.h
+-rw-rw-rw-   0        0        0     1140 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/qgate.h
+-rw-rw-rw-   0        0        0    21198 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/qops.c
+-rw-rw-rw-   0        0        0     3043 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/qops.h
+-rw-rw-rw-   0        0        0     4338 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/qstate.c
+-rw-rw-rw-   0        0        0     3202 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/doki/qstate.h
+-rw-rw-rw-   0        0        0       14 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/src/meson.build
+-rw-rw-rw-   0        0        0     5825 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/tests/canonical_form_tests.py
+-rw-rw-rw-   0        0        0     2809 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/tests/density_matrix_tests.py
+-rw-rw-rw-   0        0        0     3524 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/tests/join_regs_tests.py
+-rw-rw-rw-   0        0        0    12323 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/tests/measure_tests.py
+-rw-rw-rw-   0        0        0     9673 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/tests/multiple_gate_tests.py
+-rw-rw-rw-   0        0        0     5661 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/tests/one_gate_tests.py
+-rw-rw-rw-   0        0        0     2987 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/tests/probability_tests.py
+-rw-rw-rw-   0        0        0     3130 2024-04-04 19:47:07.000000 doki_mowstyl-1.5.2/tests/reg_creation_tests.py
+-rw-r--r--   0        0        0    38301 2024-04-04 19:47:59.039627 doki_mowstyl-1.5.2/PKG-INFO
```

### Comparing `doki-Mowstyl-1.5.0/README.md` & `doki_mowstyl-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `doki-Mowstyl-1.5.0/src/doki/doki.c` & `doki_mowstyl-1.5.2/src/doki/doki.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+/*
+ * Doki: Quantum Computer simulator, using state vectors. QSimov core.
+ * Copyright (C) 2021  Hernán Indíbil de la Cruz Calvo
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, either version 3 of the License, or
+ * (at your option) any later version.
+ *
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
+ */
+
 #define PY_SSIZE_T_CLEAN
 #include "platform.h"
 #include "qgate.h"
 #include "qops.h"
 #include "qstate.h"
 #include <Python.h>
 #include <complex.h>
@@ -41,14 +59,16 @@
 
 static PyObject *doki_registry_measure (PyObject *self, PyObject *args);
 
 static PyObject *doki_registry_prob (PyObject *self, PyObject *args);
 
 static PyObject *doki_registry_density (PyObject *self, PyObject *args);
 
+static PyObject *doki_registry_mem (PyObject *self, PyObject *args);
+
 static PyObject *doki_funmatrix_create (PyObject *self, PyObject *args);
 
 static PyObject *doki_funmatrix_identity (PyObject *self, PyObject *args);
 
 static PyObject *doki_funmatrix_densityzero (PyObject *self, PyObject *args);
 
 static PyObject *doki_funmatrix_statezero (PyObject *self, PyObject *args);
@@ -85,14 +105,16 @@
 
 static PyObject *doki_funmatrix_partialtrace (PyObject *self, PyObject *args);
 
 static PyObject *doki_funmatrix_trace (PyObject *self, PyObject *args);
 
 static PyObject *doki_funmatrix_apply (PyObject *self, PyObject *args);
 
+static PyObject *doki_funmatrix_mem (PyObject *self, PyObject *args);
+
 static PyMethodDef DokiMethods[] = {
   { "gate_new", doki_gate_new, METH_VARARGS, "Create new gate" },
   { "gate_get", doki_gate_get, METH_VARARGS, "Get matrix associated to gate" },
   { "registry_new", doki_registry_new, METH_VARARGS, "Create new registry" },
   { "registry_new_data", doki_registry_new_data, METH_VARARGS,
     "Create new registry initialized with the specified values" },
   { "registry_clone", doki_registry_clone, METH_VARARGS, "Clone a registry" },
@@ -104,14 +126,16 @@
     "Merges two registries" },
   { "registry_measure", doki_registry_measure, METH_VARARGS,
     "Measures and collapses specified qubits" },
   { "registry_prob", doki_registry_prob, METH_VARARGS,
     "Get the chances of obtaining 1 when measuring a certain qubit" },
   { "registry_density", doki_registry_density, METH_VARARGS,
     "Get the density matrix" },
+  { "registry_mem", doki_registry_mem, METH_VARARGS,
+    "Get the memory allocated by this registry in bytes" },
   { "funmatrix_create", doki_funmatrix_create, METH_VARARGS,
     "Create a functional matrix from a matrix" },
   { "funmatrix_identity", doki_funmatrix_identity, METH_VARARGS,
     "Create an identity functional matrix of the specified number "
     "of qubits" },
   { "funmatrix_statezero", doki_funmatrix_statezero, METH_VARARGS,
     "Create a functional matrix representing the state vector of "
@@ -154,14 +178,16 @@
   { "funmatrix_partialtrace", doki_funmatrix_partialtrace, METH_VARARGS,
     "Get the partial trace of a functional matrix" },
   { "funmatrix_trace", doki_funmatrix_trace, METH_VARARGS,
     "Get the trace of a functional matrix" },
   { "funmatrix_apply", doki_funmatrix_apply, METH_VARARGS,
     "Get the resulting functional matrix after applying a gate to a state "
     "vector" },
+  { "funmatrix_mem", doki_funmatrix_mem, METH_VARARGS,
+    "Get the memory allocated by this FMatrix in bytes" },
   { NULL, NULL, 0, NULL } /* Sentinel */
 };
 
 static struct PyModuleDef dokimodule
     = { PyModuleDef_HEAD_INIT, "doki", /* name of module */
         NULL,                          /* module documentation, may be NULL */
         -1, /* size of per-interpreter state of the module,
@@ -1363,14 +1389,40 @@
     }
 
   return PyCapsule_New ((void *)densityMatrix, "qsimov.doki.funmatrix",
                         &doki_funmatrix_destroy);
 }
 
 static PyObject *
+doki_registry_mem (PyObject *self, PyObject *args)
+{
+  PyObject *state_capsule;
+  void *raw_state;
+  size_t size;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "Op", &state_capsule, &debug_enabled))
+    {
+      PyErr_SetString (DokiError, "Syntax: registry_mem(state, verbose)");
+      return NULL;
+    }
+
+  raw_state = PyCapsule_GetPointer (state_capsule, "qsimov.doki.state_vector");
+  if (raw_state == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to registry");
+      return NULL;
+    }
+
+  size = state_mem_size ((struct state_vector*) raw_state);
+
+  return PyLong_FromSize_t(size);
+}
+
+static PyObject *
 doki_funmatrix_create (PyObject *self, PyObject *args)
 {
 
   PyObject *list, *row, *raw_val;
   unsigned int num_rows, num_cols;
   NATURAL_TYPE size, i, j;
   COMPLEX_TYPE val, *matrix_2d;
@@ -2553,7 +2605,33 @@
         }
       return NULL;
     }
 
   return PyCapsule_New ((void *)new_state, "qsimov.doki.funmatrix",
                         &doki_funmatrix_destroy);
 }
+
+static PyObject *
+doki_funmatrix_mem (PyObject *self, PyObject *args)
+{
+  PyObject *fmat_capsule;
+  void *raw_fmat;
+  size_t size;
+  int debug_enabled;
+
+  if (!PyArg_ParseTuple (args, "Op", &fmat_capsule, &debug_enabled))
+    {
+      PyErr_SetString (DokiError, "Syntax: funmatrix_mem(fmatrix, verbose)");
+      return NULL;
+    }
+
+  raw_fmat = PyCapsule_GetPointer (fmat_capsule, "qsimov.doki.funmatrix");
+  if (raw_fmat == NULL)
+    {
+      PyErr_SetString (DokiError, "NULL pointer to FMatrix");
+      return NULL;
+    }
+
+  size = FM_mem_size ((struct FMatrix*) raw_fmat);
+
+  return PyLong_FromSize_t(size);
+}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `doki-Mowstyl-1.5.0/src/doki/funmatrix.c` & `doki_mowstyl-1.5.2/src/doki/funmatrix.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+/*
+ * Doki: Quantum Computer simulator, using state vectors. QSimov core.
+ * Copyright (C) 2021  Hernán Indíbil de la Cruz Calvo
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, either version 3 of the License, or
+ * (at your option) any later version.
+ *
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
+ */
+
 #ifdef __MINGW32__
 #define __USE_MINGW_ANSI_STDIO 1
 #endif
 
 #include "funmatrix.h"
 #include <errno.h>
 #include <math.h>
@@ -25,14 +43,16 @@
   void *matrix2d;
   /* Associated FMatrix (if any) */
   PyObject *fmat;
   /* Length of the array (#rows x #columns) */
   NATURAL_TYPE length;
   /* How many references are there to this object */
   NATURAL_TYPE refcount;
+  /* Size of an array element */
+  size_t elem_size;
 };
 
 struct Projection
 {
   /* FMatrix capsule */
   PyObject *fmat_capsule;
   /* FMatrix over which we'll apply the projection */
@@ -45,27 +65,40 @@
   bool value;
 };
 
 static void free_matrixelem (void *raw_me);
 
 static void *clone_matrixelem (void *raw_me);
 
-static struct Matrix2D *new_matrix2d (void *matrix2d, NATURAL_TYPE length);
+static size_t size_matrixelem (void *raw_me);
+
+static struct Matrix2D *new_matrix2d (void *matrix2d, NATURAL_TYPE length,
+                                      size_t elem_size);
 
 static void free_matrix2d (void *raw_mat);
 
 static void *clone_matrix2d (void *raw_mat);
 
+static size_t size_matrix2d (void *raw_mat);
+
 static struct Projection *new_projection (PyObject *parent_capsule,
                                           NATURAL_TYPE qubitId, bool value);
 
 static void free_projection (void *raw_proj);
 
 static void *clone_projection (void *raw_proj);
 
+static size_t size_projection (void *raw_proj);
+
+void free_capsule (void *raw_capsule);
+
+void *clone_capsule (void *raw_capsule);
+
+static size_t size_fmat_capsule (void *raw_capsule);
+
 static struct FMatrix *_WalshHadamard (int n, bool isHadamard);
 
 #ifndef _MSC_VER
 __attribute__ ((const))
 #endif
 static COMPLEX_TYPE
 _IdentityFunction (NATURAL_TYPE i, NATURAL_TYPE j,
@@ -174,15 +207,16 @@
 
 /* Constructor */
 struct FMatrix *
 new_FunctionalMatrix (NATURAL_TYPE n_rows, NATURAL_TYPE n_columns,
                       COMPLEX_TYPE (*fun) (NATURAL_TYPE, NATURAL_TYPE,
                                            NATURAL_TYPE, NATURAL_TYPE, void *),
                       void *argv, void (*argv_free) (void *),
-                      void *(*argv_clone) (void *))
+                      void *(*argv_clone) (void *),
+                      size_t (*argv_size) (void *))
 {
   struct FMatrix *pFM = MALLOC_TYPE (1, struct FMatrix);
 
   if (pFM != NULL)
     {
       pFM->r = n_rows;
       pFM->c = n_columns;
@@ -195,14 +229,15 @@
       pFM->op = -1;
       pFM->transpose = false;
       pFM->conjugate = false;
       pFM->simple = true;
       pFM->argv = argv;
       pFM->argv_free = argv_free;
       pFM->argv_clone = argv_clone;
+      pFM->argv_size = argv_size;
     }
 
   return pFM;
 }
 
 /* Get the element (i, j) from the matrix a */
 int
@@ -370,14 +405,15 @@
           pFM->op = 0;
           pFM->transpose = false;
           pFM->conjugate = false;
           pFM->simple = false;
           pFM->argv = NULL;
           pFM->argv_free = NULL;
           pFM->argv_clone = NULL;
+          pFM->argv_size = NULL;
         }
       else
         {
           errno = 1;
         }
     }
   else
@@ -426,14 +462,15 @@
           pFM->op = 1;
           pFM->transpose = false;
           pFM->conjugate = false;
           pFM->simple = false;
           pFM->argv = NULL;
           pFM->argv_free = NULL;
           pFM->argv_clone = NULL;
+          pFM->argv_size = NULL;
         }
       else
         {
           errno = 1;
         }
     }
   else
@@ -480,14 +517,15 @@
         }
       else
         {
           pFM->argv = m->argv;
         }
       pFM->argv_free = m->argv_free;
       pFM->argv_clone = m->argv_clone;
+      pFM->argv_size = m->argv_size;
     }
   else
     {
       errno = 1;
     }
 
   return pFM;
@@ -529,14 +567,15 @@
         }
       else
         {
           pFM->argv = m->argv;
         }
       pFM->argv_free = m->argv_free;
       pFM->argv_clone = m->argv_clone;
+      pFM->argv_size = m->argv_size;
     }
   else
     {
       errno = 1;
     }
 
   return pFM;
@@ -579,14 +618,15 @@
           pFM->op = 2;
           pFM->transpose = false;
           pFM->conjugate = false;
           pFM->simple = false;
           pFM->argv = NULL;
           pFM->argv_free = NULL;
           pFM->argv_clone = NULL;
+          pFM->argv_size = NULL;
         }
       else
         {
           errno = 1;
         }
     }
   else
@@ -636,14 +676,15 @@
           pFM->op = 3;
           pFM->transpose = false;
           pFM->conjugate = false;
           pFM->simple = false;
           pFM->argv = NULL;
           pFM->argv_free = NULL;
           pFM->argv_clone = NULL;
+          pFM->argv_size = NULL;
         }
       else
         {
           errno = 1;
         }
     }
   else if (a->r == 1 && b->c == 1)
@@ -697,14 +738,15 @@
       pFM->op = 4;
       pFM->transpose = false;
       pFM->conjugate = false;
       pFM->simple = false;
       pFM->argv = NULL;
       pFM->argv_free = NULL;
       pFM->argv_clone = NULL;
+      pFM->argv_size = NULL;
     }
   else
     {
       errno = 1;
     }
 
   return pFM;
@@ -774,25 +816,25 @@
   if (raw_data == NULL)
     {
       errno = 5;
       return NULL;
     }
   raw_data[0] = NATURAL_ONE << leftQ;
   raw_data[1] = NATURAL_ONE << rightQ;
-  data = new_matrix2d ((void *)raw_data, 2);
+  data = new_matrix2d ((void *)raw_data, 2, sizeof (NATURAL_TYPE));
   if (data == NULL)
     {
       errno = 6;
       free (raw_data);
       return NULL;
     }
 
   pFM = new_FunctionalMatrix (
       raw_data[0] * m->r * raw_data[1], raw_data[0] * m->c * raw_data[1],
-      &_eyeKronFunction, data, free_matrix2d, clone_matrix2d);
+      &_eyeKronFunction, data, free_matrix2d, clone_matrix2d, size_matrix2d);
 
   if (pFM == NULL)
     {
       errno = 1;
       free (raw_data);
       free (data);
     }
@@ -841,14 +883,15 @@
         }
       else
         {
           pFM->argv = m->argv;
         }
       pFM->argv_free = m->argv_free;
       pFM->argv_clone = m->argv_clone;
+      pFM->argv_size = m->argv_size;
     }
   else
     {
       errno = 1;
     }
 
   return pFM;
@@ -890,14 +933,15 @@
         }
       else
         {
           pFM->argv = m->argv;
         }
       pFM->argv_free = m->argv_free;
       pFM->argv_clone = m->argv_clone;
+      pFM->argv_size = m->argv_size;
     }
   else
     {
       errno = 1;
     }
 
   return pFM;
@@ -958,15 +1002,16 @@
   if (proj == NULL)
     {
       errno = 5;
       return NULL;
     }
 
   pFM = new_FunctionalMatrix (m->r, m->c, &_projectionFunction, proj,
-                              free_projection, clone_projection);
+                              free_projection, clone_projection,
+                              size_projection);
 
   if (pFM == NULL)
     {
       errno = 1;
       free_projection (proj);
     }
 
@@ -1059,14 +1104,31 @@
   Py_INCREF (me->m_capsule);
   new_me->m_capsule = me->m_capsule;
   new_me->e = me->e;
 
   return new_me;
 }
 
+static size_t
+size_matrixelem (void *raw_me)
+{
+  size_t size;
+  struct DMatrixForTrace *me = (struct DMatrixForTrace *)raw_me;
+
+  if (me == NULL)
+    {
+      return 0;
+    }
+
+  size = sizeof (struct DMatrixForTrace);
+  size += FM_mem_size (me->m);
+
+  return size;
+}
+
 /* Partial trace */
 struct FMatrix *
 partial_trace (PyObject *raw_m, int elem)
 {
   struct FMatrix *m, *pt = NULL;
   struct DMatrixForTrace *me = NULL;
 
@@ -1091,15 +1153,16 @@
   if (me != NULL)
     {
       me->m = m;
       Py_INCREF (raw_m);
       me->m_capsule = raw_m;
       me->e = elem;
       pt = new_FunctionalMatrix (m->r >> 1, m->c >> 1, _PartialTFunct, me,
-                                 free_matrixelem, clone_matrixelem);
+                                 free_matrixelem, clone_matrixelem,
+                                 size_matrixelem);
       if (pt == NULL)
         {
           Py_DECREF (raw_m);
           free_matrixelem (me);
           errno = 1;
         }
     }
@@ -1134,15 +1197,15 @@
 struct FMatrix *
 Identity (int n)
 {
   struct FMatrix *pFM;
   NATURAL_TYPE size;
 
   size = NATURAL_ONE << n; // 2^n
-  pFM = new_FunctionalMatrix (size, size, &_IdentityFunction, NULL, NULL,
+  pFM = new_FunctionalMatrix (size, size, &_IdentityFunction, NULL, NULL, NULL,
                               NULL);
 
   return pFM;
 }
 
 static COMPLEX_TYPE
 _StateZeroFunction (NATURAL_TYPE i, NATURAL_TYPE j,
@@ -1161,15 +1224,16 @@
 struct FMatrix *
 StateZero (int n)
 {
   struct FMatrix *pFM;
   NATURAL_TYPE size;
 
   size = NATURAL_ONE << n; // 2^n
-  pFM = new_FunctionalMatrix (size, 1, &_StateZeroFunction, NULL, NULL, NULL);
+  pFM = new_FunctionalMatrix (size, 1, &_StateZeroFunction, NULL, NULL, NULL,
+                              NULL);
 
   return pFM;
 }
 
 static COMPLEX_TYPE
 _DensityZeroFunction (NATURAL_TYPE i, NATURAL_TYPE j,
 #ifndef _MSC_VER
@@ -1188,15 +1252,15 @@
 DensityZero (int n)
 {
   struct FMatrix *pFM;
   NATURAL_TYPE size;
 
   size = NATURAL_ONE << n; // 2^n
   pFM = new_FunctionalMatrix (size, size, &_DensityZeroFunction, NULL, NULL,
-                              NULL);
+                              NULL, NULL);
 
   return pFM;
 }
 
 static COMPLEX_TYPE
 _WalshFunction (NATURAL_TYPE i, NATURAL_TYPE j, NATURAL_TYPE size,
 #ifndef _MSC_VER
@@ -1244,15 +1308,15 @@
 _WalshHadamard (int n, bool isHadamard)
 {
   struct FMatrix *pFM;
   NATURAL_TYPE size;
 
   size = NATURAL_ONE << n; // 2^n
   pFM = new_FunctionalMatrix (size, size, &_WalshFunction, (void *)isHadamard,
-                              NULL, NULL);
+                              NULL, NULL, NULL);
 
   return pFM;
 }
 
 struct FMatrix *
 Walsh (int n)
 {
@@ -1317,46 +1381,64 @@
     }
 
   Py_INCREF (capsule);
 
   return raw_capsule;
 }
 
+static size_t
+size_fmat_capsule (void *raw_capsule)
+{
+  struct FMatrix *pFM;
+  PyObject *capsule = (PyObject *)raw_capsule;
+
+  if (capsule == NULL)
+    {
+      return 0;
+    }
+
+  pFM = (struct FMatrix *)PyCapsule_GetPointer (capsule,
+                                                "qsimov.doki.funmatrix");
+
+  return FM_mem_size (pFM);
+}
+
 struct FMatrix *
 CU (PyObject *raw_U)
 {
   struct FMatrix *U = (struct FMatrix *)PyCapsule_GetPointer (
       raw_U, "qsimov.doki.funmatrix");
 
   if (U == NULL)
     {
       return NULL;
     }
 
   U = new_FunctionalMatrix (rows (U) * 2, columns (U) * 2, &_CUFunction, raw_U,
-                            free_capsule, clone_capsule);
+                            free_capsule, clone_capsule, size_fmat_capsule);
   if (U != NULL)
     {
       Py_INCREF (raw_U);
     }
 
   return U;
 }
 
 static struct Matrix2D *
-new_matrix2d (void *matrix2d, NATURAL_TYPE length)
+new_matrix2d (void *matrix2d, NATURAL_TYPE length, size_t elem_size)
 {
   struct Matrix2D *mat = MALLOC_TYPE (1, struct Matrix2D);
 
   if (mat != NULL)
     {
       mat->matrix2d = matrix2d;
       mat->fmat = NULL;
       mat->length = length;
       mat->refcount = 1;
+      mat->elem_size = elem_size;
     }
 
   return mat;
 }
 
 static void
 free_matrix2d (void *raw_mat)
@@ -1389,14 +1471,34 @@
       return NULL;
     }
 
   mat->refcount++;
   return raw_mat;
 }
 
+static size_t
+size_matrix2d (void *raw_mat)
+{
+  size_t size;
+  struct Matrix2D *mat = (struct Matrix2D *)raw_mat;
+  struct FMatrix *aux;
+
+  if (mat == NULL)
+    {
+      return 0;
+    }
+  size = sizeof (struct Matrix2D);
+
+  aux = PyCapsule_GetPointer (mat->fmat, "qsimov.doki.funmatrix");
+  size += FM_mem_size (aux);
+  size += mat->length * mat->elem_size;
+
+  return size;
+}
+
 static struct Projection *
 new_projection (PyObject *parent_capsule, NATURAL_TYPE qubitId, bool value)
 {
   struct Projection *proj;
   struct FMatrix *m;
 
   m = PyCapsule_GetPointer (parent_capsule, "qsimov.doki.funmatrix");
@@ -1450,14 +1552,30 @@
       return NULL;
     }
 
   proj->refcount++;
   return raw_proj;
 }
 
+static size_t
+size_projection (void *raw_proj)
+{
+  size_t size;
+  struct Projection *proj = (struct Projection *)raw_proj;
+
+  if (proj == NULL)
+    {
+      return 0;
+    }
+  size = sizeof (struct Projection);
+  size += FM_mem_size (proj->fmat);
+
+  return size;
+}
+
 static COMPLEX_TYPE
 _CustomMat (NATURAL_TYPE i, NATURAL_TYPE j, NATURAL_TYPE nrows,
 #ifndef _MSC_VER
             NATURAL_TYPE unused __attribute__ ((unused)),
 #else
             NATURAL_TYPE unused,
 #endif
@@ -1468,17 +1586,18 @@
   return ((COMPLEX_TYPE *)custom_matrix->matrix2d)[i * nrows + j];
 }
 
 struct FMatrix *
 CustomMat (COMPLEX_TYPE *matrix_2d, NATURAL_TYPE length, NATURAL_TYPE nrows,
            NATURAL_TYPE ncols)
 {
-  return new_FunctionalMatrix (nrows, ncols, &_CustomMat,
-                               new_matrix2d ((void *)matrix_2d, length),
-                               free_matrix2d, clone_matrix2d);
+  return new_FunctionalMatrix (
+      nrows, ncols, &_CustomMat,
+      new_matrix2d ((void *)matrix_2d, length, sizeof (COMPLEX_TYPE)),
+      free_matrix2d, clone_matrix2d, size_matrix2d);
 }
 
 static int
 _bytes_added (int sprintfRe)
 {
   return (sprintfRe > 0) ? sprintfRe : 0;
 }
@@ -1594,9 +1713,34 @@
   src->op = -1;
   src->transpose = false;
   src->conjugate = false;
   src->simple = true;
   src->argv = NULL;
   src->argv_free = NULL;
   src->argv_clone = NULL;
+  src->argv_size = NULL;
   free (src);
 }
+
+size_t
+FM_mem_size (struct FMatrix *src)
+{
+  size_t size;
+  if (src == NULL)
+    {
+      return 0;
+    }
+  size = sizeof (struct FMatrix);
+  if (src->A != NULL)
+    {
+      size += FM_mem_size (src->A);
+    }
+  if (src->B != NULL)
+    {
+      size += FM_mem_size (src->B);
+    }
+  if (src->argv_size != NULL)
+    {
+      size += src->argv_size (src->argv);
+    }
+  return size;
+}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `doki-Mowstyl-1.5.0/src/doki/funmatrix.h` & `doki_mowstyl-1.5.2/src/doki/funmatrix.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+/*
+ * Doki: Quantum Computer simulator, using state vectors. QSimov core.
+ * Copyright (C) 2021  Hernán Indíbil de la Cruz Calvo
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, either version 3 of the License, or
+ * (at your option) any later version.
+ *
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
+ */
+
 #pragma once
 #ifndef FUNMATRIX_H_
 #define FUNMATRIX_H_
 
 #include "platform.h"
 #include <Python.h>
 #include <complex.h>
@@ -31,14 +49,16 @@
   PyObject *B_capsule;
   /* Extra arguments to pass to the function f */
   void *argv;
   /* Function that frees memory used by argv (if needed) */
   void (*argv_free) (void *);
   /* Function that clones argv (if needed) */
   void *(*argv_clone) (void *);
+  /* Function that returns the size of argv (if needed) */
+  size_t (*argv_size) (void *);
   /* Whether the matrix has to be transposed or not */
   bool transpose;
   /* Whether the matrix has to be complex conjugated or not */
   bool conjugate;
   /* Whether the matrix is simple or you have to perform an operation */
   bool simple;
   /* Operation to apply between the matrices.
@@ -57,15 +77,16 @@
 
 /* Constructor */
 struct FMatrix *
 new_FunctionalMatrix (NATURAL_TYPE n_rows, NATURAL_TYPE n_columns,
                       COMPLEX_TYPE (*fun) (NATURAL_TYPE, NATURAL_TYPE,
                                            NATURAL_TYPE, NATURAL_TYPE, void *),
                       void *argv, void (*argv_free) (void *),
-                      void *(*argv_clone) (void *));
+                      void *(*argv_clone) (void *),
+                      size_t (*argv_size) (void *));
 
 /*
  * Get the element (i, j) from the matrix a, and return the result in
  * the address pointed by sol.
  * Return values:
  * 0 -> OK
  * 1 -> Error adding
@@ -214,8 +235,10 @@
 __attribute__ ((pure))
 #endif
 char *
 FM_toString (struct FMatrix *a);
 
 void FM_destroy (struct FMatrix *src);
 
+size_t FM_mem_size (struct FMatrix *src);
+
 #endif /* FUNMATRIX_H_ */
```

### Comparing `doki-Mowstyl-1.5.0/src/doki/platform.h` & `doki_mowstyl-1.5.2/src/doki/platform.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+/*
+ * Doki: Quantum Computer simulator, using state vectors. QSimov core.
+ * Copyright (C) 2021  Hernán Indíbil de la Cruz Calvo
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, either version 3 of the License, or
+ * (at your option) any later version.
+ *
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
+ */
+
 /** \file platform.h
  *  \brief Functions and macros that may require platform specific stuff.
  *
  *  In this file some functions and macros have been defined.
  */
 
 /** \def __PLATFORM_H
@@ -177,54 +195,54 @@
 #define DECIMAL_PLACES_S "5" // same as before, but as a string
 #define NOTATION                                                              \
   "g" // f for normal behaviour, e for scientific notation, g for shortest (f
       // or e)
 #define PRECISION 2
 #if PRECISION == 1
 #define REAL_TYPE float
-#ifndef _WIN32
+#ifndef _MSC_VER
 #define COMPLEX_TYPE float _Complex
 #else
 #define COMPLEX_TYPE _Fcomplex
 #endif
 #define RE crealf
 #define IM cimagf
 #define ARG cargf
 #define COS cosf
 #define SIN sinf
 #define REAL_STRING_FORMAT "%." DECIMAL_PLACES_S NOTATION
 #elif PRECISION == 2
 #define REAL_TYPE double
-#ifndef _WIN32
+#ifndef _MSC_VER
 #define COMPLEX_TYPE double _Complex
 #else
 #define COMPLEX_TYPE _Dcomplex
 #endif
 #define RE creal
 #define IM cimag
 #define ARG carg
 #define COS cos
 #define SIN sin
 #define REAL_STRING_FORMAT "%." DECIMAL_PLACES_S "l" NOTATION
 #elif PRECISION == 3
 #define REAL_TYPE long double
-#ifndef _WIN32
+#ifndef _MSC_VER
 #define COMPLEX_TYPE long double _Complex
 #else
 #define COMPLEX_TYPE _Lcomplex
 #endif
 #define RE creall
 #define IM cimagl
 #define ARG cargl
 #define COS cosl
 #define SIN sinl
 #define REAL_STRING_FORMAT "%." DECIMAL_PLACES_S "L" NOTATION
 #endif
 
-#ifndef _WIN32
+#ifndef _MSC_VER
 static const COMPLEX_TYPE COMPLEX_ZERO = 0;
 static const COMPLEX_TYPE COMPLEX_ONE = 1;
 static const COMPLEX_TYPE COMPLEX_NAN = NAN;
 #else
 static const COMPLEX_TYPE COMPLEX_ZERO = { 0, 0 };
 static const COMPLEX_TYPE COMPLEX_ONE = { 1, 0 };
 static const COMPLEX_TYPE COMPLEX_NAN = { NAN, NAN };
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `doki-Mowstyl-1.5.0/src/doki/qops.c` & `doki_mowstyl-1.5.2/src/doki/qops.c`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,40 @@
+/*
+ * Doki: Quantum Computer simulator, using state vectors. QSimov core.
+ * Copyright (C) 2021  Hernán Indíbil de la Cruz Calvo
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, either version 3 of the License, or
+ * (at your option) any later version.
+ *
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
+ */
+
 #include <Python.h>
 #include <errno.h>
 #include <math.h>
 #include <omp.h>
 #include <stdio.h>
 #include <stdlib.h>
 
 #include "arraylist.h"
 #include "platform.h"
 #include "qgate.h"
 #include "qops.h"
 #include "qstate.h"
 
+static size_t size_state_capsule (void *raw_capsule);
+
 #ifndef _MSC_VER
 __attribute__ ((const))
 #endif
 static COMPLEX_TYPE
 _densityFun (NATURAL_TYPE i, NATURAL_TYPE j,
 #ifndef _MSC_VER
              NATURAL_TYPE unused1 __attribute__ ((unused)),
@@ -54,26 +74,27 @@
 
   return phase;
 }
 
 REAL_TYPE
 probability (struct state_vector *state, unsigned int target_id)
 {
-  NATURAL_TYPE i;
+  NATURAL_TYPE i, mask;
   REAL_TYPE value;
   COMPLEX_TYPE val;
 
   value = 0;
+  mask = NATURAL_ONE << target_id;
 #pragma omp parallel for reduction (+:value) \
                              default (none) \
-                             shared (state, target_id) \
+                             shared (state, mask, target_id) \
                              private (i, val)
-  for (i = 0; i < state->size; i++)
+  for (i = mask; i < state->size; ++i)
     {
-      if ((i & (NATURAL_ONE << target_id)) != 0)
+      if (i & mask)
         {
           val = state_get (state, i);
           value += RE (val) * RE (val) + IM (val) * IM (val);
         }
     }
 
   return value;
@@ -108,28 +129,27 @@
   return 0;
 }
 
 unsigned char
 measure (struct state_vector *state, _Bool *result, unsigned int target,
          struct state_vector *new_state, REAL_TYPE roll)
 {
-  NATURAL_TYPE i;
   REAL_TYPE sum;
   unsigned char exit_code;
 
   sum = probability (state, target);
   *result = sum > roll;
-  exit_code = collapse (state, target, *result, new_state);
+  exit_code = collapse (state, target, *result, sum, new_state);
 
   return exit_code;
 }
 
 unsigned char
 collapse (struct state_vector *state, unsigned int target_id, _Bool value,
-          struct state_vector *new_state)
+          REAL_TYPE prob_one, struct state_vector *new_state)
 {
   unsigned char exit_code;
   NATURAL_TYPE i, j, count, step;
   _Bool toggle;
   REAL_TYPE norm_const;
   COMPLEX_TYPE aux;
 
@@ -149,26 +169,25 @@
   */
   exit_code = state_init (new_state, state->num_qubits - 1, 0);
   if (exit_code != 0)
     {
       free (new_state);
       return exit_code;
     }
-  norm_const = 0;
-  toggle = 0;
+  norm_const = value ? prob_one : 1 - prob_one;
+  toggle = value;
   count = 0;
   step = NATURAL_ONE << target_id;
   j = 0;
-  for (i = 0; i < state->size; i++)
+  for (i = value ? step : 0; i < state->size; i++)
     {
       if (toggle == value)
         {
           aux = state_get (state, i);
           state_set (new_state, j, aux);
-          norm_const += pow (RE (aux), 2) + pow (IM (aux), 2);
           j++;
         }
       count++;
       if (count == step)
         {
           count = 0;
           toggle = !toggle;
@@ -343,15 +362,15 @@
 // We can calculate each element of the new state separately
 #pragma omp parallel for reduction (+:aux_const) \
                              default(none) \
                              shared (state, not_copy, new_state, gate, \
                                      targets, num_targets, \
                                      controls, num_controls, \
                                      anticontrols, num_anticontrols, \
-                                     norm_const) \
+                                     norm_const, COMPLEX_ZERO) \
                              private (curr_id, sum, row, reg_index, i, j, k)
   for (i = 0; i < not_copy->size; i++)
     {
       // If there has been any error in this thread, we skip
       curr_id = alist_get (not_copy, i);
       reg_index = curr_id;
       sum = COMPLEX_ZERO;
@@ -452,14 +471,16 @@
                  unsigned int *controls, unsigned int num_controls,
                  unsigned int *anticontrols, unsigned int num_anticontrols);
 
 static void free_application (void *raw_app);
 
 static void *clone_application (void *raw_app);
 
+static size_t size_application (void *raw_app);
+
 #ifndef _MSC_VER
 __attribute__ ((const))
 #endif
 static COMPLEX_TYPE
 _ApplyGateFunction (NATURAL_TYPE i,
 #ifndef _MSC_VER
                     NATURAL_TYPE unused1 __attribute__ ((unused)),
@@ -559,14 +580,34 @@
       return NULL;
     }
 
   data->refcount++;
   return raw_app;
 }
 
+static size_t
+size_application (void *raw_app)
+{
+  size_t size;
+  struct Application *data = (struct Application *)raw_app;
+
+  if (data == NULL)
+    {
+      return 0;
+    }
+  size = sizeof (struct Application);
+  size += FM_mem_size (data->state);
+  size += FM_mem_size (data->gate);
+  size += data->num_targets * sizeof (unsigned int);
+  size += data->num_controls * sizeof (unsigned int);
+  size += data->num_anticontrols * sizeof (unsigned int);
+
+  return size;
+}
+
 struct FMatrix *
 apply_gate_fmat (PyObject *state_capsule, PyObject *gate_capsule,
                  unsigned int *targets, unsigned int num_targets,
                  unsigned int *controls, unsigned int num_controls,
                  unsigned int *anticontrols, unsigned int num_anticontrols)
 {
   struct FMatrix *pFM;
@@ -577,15 +618,16 @@
   if (data == NULL)
     {
       errno = 5;
       return NULL;
     }
 
   pFM = new_FunctionalMatrix (data->state->r, 1, &_ApplyGateFunction, data,
-                              free_application, clone_application);
+                              free_application, clone_application,
+                              size_application);
   if (pFM == NULL)
     {
       errno = 1;
       free_application (data);
     }
 
   return pFM;
@@ -632,15 +674,15 @@
     {
       mask = NATURAL_ONE << data->anticontrols[k];
       if (i & mask)
         {
           res = getitem (data->state, i, 0, &val);
           if (res != 0)
             {
-              printf ("Error[A] %d while getting state item %llu\n", res);
+              printf ("Error[A] %d while getting state item %llu\n", res, i);
               return COMPLEX_NAN;
             }
           return val;
         }
     }
 
   for (n = 0; n < data->gate->r; ++n)
@@ -664,40 +706,60 @@
             {
               reg_index &= ~(NATURAL_ONE << data->targets[k]);
             }
         }
       res = getitem (data->state, reg_index, 0, &aux);
       if (res != 0)
         {
-          printf ("Error[T] %d while getting state[%llu] item %llu\n", res, i, reg_index);
+          printf ("Error[T] %d while getting state[%llu] item %llu\n", res, i,
+                  reg_index);
           return COMPLEX_NAN;
         }
       res = getitem (data->gate, row, n, &aux2);
       if (res != 0)
         {
-          printf ("Error[T] %d while getting gate item %llu, %llu\n", res, row, n);
+          printf ("Error[T] %d while getting gate item %llu, %llu\n", res, row,
+                  n);
           return COMPLEX_NAN;
         }
       val = COMPLEX_ADD (val, COMPLEX_MULT (aux, aux2));
     }
 
   return val;
 }
 
+static size_t
+size_state_capsule (void *raw_capsule)
+{
+  struct state_vector *state;
+  PyObject *capsule = (PyObject *)raw_capsule;
+
+  if (capsule == NULL)
+    {
+      return 0;
+    }
+
+  state = (struct state_vector *)PyCapsule_GetPointer (
+      capsule, "qsimov.doki.state_vector");
+
+  return state_mem_size (state);
+}
+
 struct FMatrix *
 density_matrix (PyObject *state_capsule)
 {
   struct FMatrix *dm = NULL;
   struct state_vector *state
       = PyCapsule_GetPointer (state_capsule, "qsimov.doki.state_vector");
 
   if (state != NULL)
     {
       dm = new_FunctionalMatrix (state->size, state->size, &_densityFun,
-                                 state_capsule, free_capsule, clone_capsule);
+                                 state_capsule, free_capsule, clone_capsule,
+                                 size_state_capsule);
       if (dm != NULL)
         {
           Py_INCREF (state_capsule);
         }
       else
         {
           errno = 1;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `doki-Mowstyl-1.5.0/src/doki/qops.h` & `doki_mowstyl-1.5.2/src/doki/qops.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+/*
+ * Doki: Quantum Computer simulator, using state vectors. QSimov core.
+ * Copyright (C) 2021  Hernán Indíbil de la Cruz Calvo
+ *
+ * This program is free software: you can redistribute it and/or modify
+ * it under the terms of the GNU General Public License as published by
+ * the Free Software Foundation, either version 3 of the License, or
+ * (at your option) any later version.
+ *
+ * This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ * GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
+ */
+
 #pragma once
 #ifndef QOPS_H_
 #define QOPS_H_
 
 #include "arraylist.h"
 #include "funmatrix.h"
 #include "qgate.h"
@@ -18,15 +36,16 @@
 REAL_TYPE
 probability (struct state_vector *state, unsigned int target_id);
 
 REAL_TYPE
 get_global_phase (struct state_vector *state);
 
 unsigned char collapse (struct state_vector *state, unsigned int id,
-                        _Bool value, struct state_vector *new_state);
+                        _Bool value, REAL_TYPE prob_one,
+                        struct state_vector *new_state);
 
 unsigned char apply_gate (struct state_vector *state, struct qgate *gate,
                           unsigned int *targets, unsigned int num_targets,
                           unsigned int *controls, unsigned int num_controls,
                           unsigned int *anticontrols,
                           unsigned int num_anticontrols,
                           struct state_vector *new_state);
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

