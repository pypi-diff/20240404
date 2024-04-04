# Comparing `tmp/repo-ast-builder-0.0.8.tar.gz` & `tmp/repo-ast-builder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-ast-builder-0.0.8.tar", last modified: Thu Apr  4 12:22:09 2024, max compression
+gzip compressed data, was "repo-ast-builder-0.0.9.tar", last modified: Thu Apr  4 16:10:04 2024, max compression
```

## Comparing `repo-ast-builder-0.0.8.tar` & `repo-ast-builder-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,60 @@
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.794950 repo-ast-builder-0.0.8/
--rw-r--r--   0 manuel     (501) staff       (20)      816 2024-04-04 12:22:09.794623 repo-ast-builder-0.0.8/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)      264 2024-03-28 20:01:53.000000 repo-ast-builder-0.0.8/README.md
--rw-r--r--   0 manuel     (501) staff       (20)      648 2024-04-04 12:22:06.000000 repo-ast-builder-0.0.8/pyproject.toml
--rw-r--r--   0 manuel     (501) staff       (20)       38 2024-04-04 12:22:09.795000 repo-ast-builder-0.0.8/setup.cfg
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.775775 repo-ast-builder-0.0.8/src/
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.778302 repo-ast-builder-0.0.8/src/repo_ast_builder/
--rw-r--r--   0 manuel     (501) staff       (20)      156 2024-04-04 11:33:33.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)     2710 2024-04-04 12:19:36.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/main.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.781235 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/
--rw-r--r--   0 manuel     (501) staff       (20)        0 2024-04-04 12:18:05.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)     2620 2024-04-04 12:09:32.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/__main__.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.783224 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/
--rw-r--r--   0 manuel     (501) staff       (20)      953 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)     1187 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/as_graph.py
--rw-r--r--   0 manuel     (501) staff       (20)      956 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/base.py
--rw-r--r--   0 manuel     (501) staff       (20)     9803 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/fasten.py
--rw-r--r--   0 manuel     (501) staff       (20)     1163 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/simple.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.786743 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/
--rw-r--r--   0 manuel     (501) staff       (20)        0 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)     1794 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/callgraph.py
--rw-r--r--   0 manuel     (501) staff       (20)     2195 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/classes.py
--rw-r--r--   0 manuel     (501) staff       (20)     8283 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/definitions.py
--rw-r--r--   0 manuel     (501) staff       (20)     7219 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/imports.py
--rw-r--r--   0 manuel     (501) staff       (20)     1135 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/key_err.py
--rw-r--r--   0 manuel     (501) staff       (20)     1936 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/modules.py
--rw-r--r--   0 manuel     (501) staff       (20)     4250 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/pointers.py
--rw-r--r--   0 manuel     (501) staff       (20)     4357 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/scopes.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.789249 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/
--rw-r--r--   0 manuel     (501) staff       (20)        0 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)    20318 2024-04-04 12:12:50.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/base.py
--rw-r--r--   0 manuel     (501) staff       (20)     9511 2024-04-04 12:12:46.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/cgprocessor.py
--rw-r--r--   0 manuel     (501) staff       (20)     3169 2024-04-04 12:12:54.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/keyerrprocessor.py
--rw-r--r--   0 manuel     (501) staff       (20)    13451 2024-04-04 12:13:04.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/postprocessor.py
--rw-r--r--   0 manuel     (501) staff       (20)    16189 2024-04-04 12:13:08.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/preprocessor.py
--rw-r--r--   0 manuel     (501) staff       (20)     8589 2024-04-04 12:10:32.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/pycg.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.791922 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/
--rw-r--r--   0 manuel     (501) staff       (20)      894 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/base.py
--rw-r--r--   0 manuel     (501) staff       (20)     2817 2024-04-04 12:12:01.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/callgraph_test.py
--rw-r--r--   0 manuel     (501) staff       (20)     3321 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/definitions_test.py
--rw-r--r--   0 manuel     (501) staff       (20)    11977 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/fasten_format_test.py
--rw-r--r--   0 manuel     (501) staff       (20)     6333 2024-04-04 12:12:01.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/imports_test.py
--rw-r--r--   0 manuel     (501) staff       (20)     3982 2024-04-04 12:12:01.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/pointers_test.py
--rw-r--r--   0 manuel     (501) staff       (20)     8192 2024-04-04 12:12:01.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/scopes_test.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.793404 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/utils/
--rw-r--r--   0 manuel     (501) staff       (20)      895 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/utils/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)     1270 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/utils/common.py
--rw-r--r--   0 manuel     (501) staff       (20)     1284 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/utils/constants.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 12:22:09.793882 repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/
--rw-r--r--   0 manuel     (501) staff       (20)      816 2024-04-04 12:22:09.000000 repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)     1894 2024-04-04 12:22:09.000000 repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/SOURCES.txt
--rw-r--r--   0 manuel     (501) staff       (20)        1 2024-04-04 12:22:09.000000 repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/dependency_links.txt
--rw-r--r--   0 manuel     (501) staff       (20)       64 2024-04-04 12:22:09.000000 repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/entry_points.txt
--rw-r--r--   0 manuel     (501) staff       (20)       44 2024-04-04 12:22:09.000000 repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/requires.txt
--rw-r--r--   0 manuel     (501) staff       (20)       17 2024-04-04 12:22:09.000000 repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/top_level.txt
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.670347 repo-ast-builder-0.0.9/
+-rw-r--r--   0 manuel     (501) staff       (20)      816 2024-04-04 16:10:04.670024 repo-ast-builder-0.0.9/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)      264 2024-03-28 20:01:53.000000 repo-ast-builder-0.0.9/README.md
+-rw-r--r--   0 manuel     (501) staff       (20)      648 2024-04-04 16:04:48.000000 repo-ast-builder-0.0.9/pyproject.toml
+-rw-r--r--   0 manuel     (501) staff       (20)       38 2024-04-04 16:10:04.670402 repo-ast-builder-0.0.9/setup.cfg
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.654181 repo-ast-builder-0.0.9/src/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2024-04-04 16:04:48.000000 repo-ast-builder-0.0.9/src/__init__.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.655869 repo-ast-builder-0.0.9/src/repo_ast_builder/
+-rw-r--r--   0 manuel     (501) staff       (20)      173 2024-04-04 16:10:00.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1509 2024-04-04 16:10:00.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/body.py
+-rw-r--r--   0 manuel     (501) staff       (20)      307 2024-04-04 16:04:48.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/main.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1007 2024-04-04 16:10:00.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/method_name.py
+-rw-r--r--   0 manuel     (501) staff       (20)      301 2024-04-04 16:10:00.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/namespace.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.660218 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2024-04-04 16:03:59.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     2620 2024-04-04 12:09:32.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/__main__.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.661728 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/
+-rw-r--r--   0 manuel     (501) staff       (20)      953 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1187 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/as_graph.py
+-rw-r--r--   0 manuel     (501) staff       (20)      956 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/base.py
+-rw-r--r--   0 manuel     (501) staff       (20)     9803 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/fasten.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1163 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/simple.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.664030 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1794 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/callgraph.py
+-rw-r--r--   0 manuel     (501) staff       (20)     2195 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/classes.py
+-rw-r--r--   0 manuel     (501) staff       (20)     8283 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/definitions.py
+-rw-r--r--   0 manuel     (501) staff       (20)     7219 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/imports.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1135 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/key_err.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1936 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/modules.py
+-rw-r--r--   0 manuel     (501) staff       (20)     4250 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/pointers.py
+-rw-r--r--   0 manuel     (501) staff       (20)     4357 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/scopes.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.665837 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)    20318 2024-04-04 12:12:50.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/base.py
+-rw-r--r--   0 manuel     (501) staff       (20)     9511 2024-04-04 12:12:46.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/cgprocessor.py
+-rw-r--r--   0 manuel     (501) staff       (20)     3169 2024-04-04 12:12:54.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/keyerrprocessor.py
+-rw-r--r--   0 manuel     (501) staff       (20)    13451 2024-04-04 12:13:04.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/postprocessor.py
+-rw-r--r--   0 manuel     (501) staff       (20)    16189 2024-04-04 12:13:08.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/preprocessor.py
+-rw-r--r--   0 manuel     (501) staff       (20)     8589 2024-04-04 12:10:32.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/pycg.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.667901 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/
+-rw-r--r--   0 manuel     (501) staff       (20)      894 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/base.py
+-rw-r--r--   0 manuel     (501) staff       (20)     2817 2024-04-04 12:12:01.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/callgraph_test.py
+-rw-r--r--   0 manuel     (501) staff       (20)     3321 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/definitions_test.py
+-rw-r--r--   0 manuel     (501) staff       (20)    11977 2024-04-04 12:12:42.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/fasten_format_test.py
+-rw-r--r--   0 manuel     (501) staff       (20)     6333 2024-04-04 12:12:01.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/imports_test.py
+-rw-r--r--   0 manuel     (501) staff       (20)     3982 2024-04-04 12:12:01.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/pointers_test.py
+-rw-r--r--   0 manuel     (501) staff       (20)     8192 2024-04-04 12:12:01.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/scopes_test.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.668774 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/utils/
+-rw-r--r--   0 manuel     (501) staff       (20)      895 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/utils/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1270 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/utils/common.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1284 2024-04-04 11:39:22.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/utils/constants.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1168 2024-04-04 16:10:00.000000 repo-ast-builder-0.0.9/src/repo_ast_builder/walk.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-04 16:10:04.669234 repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/
+-rw-r--r--   0 manuel     (501) staff       (20)      816 2024-04-04 16:10:04.000000 repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)     2038 2024-04-04 16:10:04.000000 repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel     (501) staff       (20)        1 2024-04-04 16:10:04.000000 repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       64 2024-04-04 16:10:04.000000 repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/entry_points.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       44 2024-04-04 16:10:04.000000 repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/requires.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       26 2024-04-04 16:10:04.000000 repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/top_level.txt
```

### Comparing `repo-ast-builder-0.0.8/PKG-INFO` & `repo-ast-builder-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-ast-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creates an AST of a Python project
 Keywords: ast,python,builder
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `repo-ast-builder-0.0.8/pyproject.toml` & `repo-ast-builder-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "repo-ast-builder"
-version = "0.0.8"
+version = "0.0.9"
 description = "Creates an AST of a Python project"
 readme = "README.md"
 authors = []
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/__main__.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/__main__.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/__init__.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/as_graph.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/as_graph.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/base.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/base.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/fasten.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/fasten.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/formats/simple.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/formats/simple.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/callgraph.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/callgraph.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/classes.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/classes.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/definitions.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/definitions.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/imports.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/imports.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/key_err.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/key_err.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/modules.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/modules.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/pointers.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/pointers.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/machinery/scopes.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/machinery/scopes.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/base.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/base.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/cgprocessor.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/cgprocessor.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/keyerrprocessor.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/keyerrprocessor.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/postprocessor.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/postprocessor.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/processing/preprocessor.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/processing/preprocessor.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/pycg.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/pycg.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/base.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/base.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/callgraph_test.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/callgraph_test.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/definitions_test.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/definitions_test.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/fasten_format_test.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/fasten_format_test.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/imports_test.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/imports_test.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/pointers_test.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/pointers_test.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/tests/scopes_test.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/tests/scopes_test.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/utils/__init__.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/utils/common.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/utils/common.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder/pycg/utils/constants.py` & `repo-ast-builder-0.0.9/src/repo_ast_builder/pycg/utils/constants.py`

 * *Files identical despite different names*

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/PKG-INFO` & `repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-ast-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creates an AST of a Python project
 Keywords: ast,python,builder
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `repo-ast-builder-0.0.8/src/repo_ast_builder.egg-info/SOURCES.txt` & `repo-ast-builder-0.0.9/src/repo_ast_builder.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 README.md
 pyproject.toml
+src/__init__.py
 src/repo_ast_builder/__init__.py
+src/repo_ast_builder/body.py
 src/repo_ast_builder/main.py
+src/repo_ast_builder/method_name.py
+src/repo_ast_builder/namespace.py
+src/repo_ast_builder/walk.py
 src/repo_ast_builder.egg-info/PKG-INFO
 src/repo_ast_builder.egg-info/SOURCES.txt
 src/repo_ast_builder.egg-info/dependency_links.txt
 src/repo_ast_builder.egg-info/entry_points.txt
 src/repo_ast_builder.egg-info/requires.txt
 src/repo_ast_builder.egg-info/top_level.txt
 src/repo_ast_builder/pycg/__init__.py
```

