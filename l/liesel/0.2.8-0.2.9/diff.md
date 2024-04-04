# Comparing `tmp/liesel-0.2.8.tar.gz` & `tmp/liesel-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liesel-0.2.8.tar", last modified: Sun Dec  3 13:26:33 2023, max compression
+gzip compressed data, was "liesel-0.2.9.tar", last modified: Thu Apr  4 19:01:22 2024, max compression
```

## Comparing `liesel-0.2.8.tar` & `liesel-0.2.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.994520 liesel-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-03 13:26:22.000000 liesel-0.2.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2023-12-03 13:26:33.994520 liesel-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-12-03 13:26:22.000000 liesel-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.982519 liesel-0.2.8/liesel/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.982519 liesel-0.2.8/liesel/bijectors/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/bijectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/bijectors/algebraic_sigmoid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.986519 liesel-0.2.8/liesel/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/distributions/copulas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16878 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/distributions/mvn_degen.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/distributions/nodist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.986519 liesel-0.2.8/liesel/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/experimental/arviz.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/experimental/pymc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.990519 liesel-0.2.8/liesel/goose/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17387 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6676 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/da.py
--rw-r--r--   0 runner    (1001) docker     (127)    24605 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/epoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14496 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/iwls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/iwls_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/kernel_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/mh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/mh_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/mm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/nuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/rw.py
--rw-r--r--   0 runner    (1001) docker     (127)    19276 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/summary_m.py
--rw-r--r--   0 runner    (1001) docker     (127)    43024 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/summary_viz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/goose/warmup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.990519 liesel-0.2.8/liesel/model/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/model/distreg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/model/goose.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/model/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    44794 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    53134 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/model/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/model/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2023-12-03 13:26:22.000000 liesel-0.2.8/liesel/option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.994520 liesel-0.2.8/liesel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2023-12-03 13:26:33.000000 liesel-0.2.8/liesel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-12-03 13:26:33.000000 liesel-0.2.8/liesel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-03 13:26:33.000000 liesel-0.2.8/liesel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-03 13:26:33.000000 liesel-0.2.8/liesel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-03 13:26:33.000000 liesel-0.2.8/liesel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-03 13:26:22.000000 liesel-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-03 13:26:33.994520 liesel-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-03 13:26:22.000000 liesel-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 13:26:33.994520 liesel-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-12-03 13:26:22.000000 liesel-0.2.8/tests/test_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.461799 liesel-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-04 19:01:17.000000 liesel-0.2.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-04 19:01:22.461799 liesel-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-04 19:01:17.000000 liesel-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.449799 liesel-0.2.9/liesel/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.453799 liesel-0.2.9/liesel/bijectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/bijectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/bijectors/algebraic_sigmoid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.453799 liesel-0.2.9/liesel/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/distributions/copulas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/distributions/mvn_degen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/distributions/nodist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.453799 liesel-0.2.9/liesel/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/experimental/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/experimental/pymc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.457799 liesel-0.2.9/liesel/goose/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/da.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24250 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/iwls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/iwls_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/kernel_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/mh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/mh_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/mm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19283 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/summary_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43024 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/summary_viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/goose/warmup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.457799 liesel-0.2.9/liesel/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/model/distreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/model/goose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/model/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45102 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53869 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/model/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/model/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-04 19:01:17.000000 liesel-0.2.9/liesel/option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.457799 liesel-0.2.9/liesel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-04 19:01:22.000000 liesel-0.2.9/liesel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-04 19:01:22.000000 liesel-0.2.9/liesel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:01:22.000000 liesel-0.2.9/liesel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 19:01:22.000000 liesel-0.2.9/liesel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 19:01:22.000000 liesel-0.2.9/liesel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-04 19:01:17.000000 liesel-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-04 19:01:22.461799 liesel-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-04 19:01:17.000000 liesel-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:01:22.457799 liesel-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-04 19:01:17.000000 liesel-0.2.9/tests/test_option.py
```

### Comparing `liesel-0.2.8/LICENSE.md` & `liesel-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/PKG-INFO` & `liesel-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liesel
-Version: 0.2.8
+Version: 0.2.9
 Summary: A probabilistic programming framework with a focus on semi-parametric regression
 Home-page: https://liesel-project.org
 Author: Paul Wiemann, Hannes Riebl, Johannes Brachem, Gianmarco Callegher
 License: MIT
 Keywords: statistics,machine-learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,32 +18,32 @@
 Requires-Dist: dill>=0.3
 Requires-Dist: jax>=0.4.1
 Requires-Dist: jaxlib>=0.4.1
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: networkx>=2.6
 Requires-Dist: numpy!=1.24.0,>=1.22
 Requires-Dist: pandas>=1.4
-Requires-Dist: scipy>=1.8
+Requires-Dist: scipy<=1.12.0,>=1.8
 Requires-Dist: seaborn>=0.13
 Requires-Dist: tensorflow-probability>=0.17
 Requires-Dist: tqdm>=4.62
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: myst-nb; extra == "dev"
+Requires-Dist: myst-nb>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pyupgrade; extra == "dev"
-Requires-Dist: sphinx>=4.5; extra == "dev"
+Requires-Dist: sphinx>=7.2.6; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints>=1.19; extra == "dev"
 Requires-Dist: pydata-sphinx-theme; extra == "dev"
-Requires-Dist: sphinx-book-theme>=1.0.1; extra == "dev"
+Requires-Dist: sphinx-book-theme>=1.1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton>=0.5; extra == "dev"
 Requires-Dist: sphinx-remove-toctrees>=0.0.3; extra == "dev"
 Requires-Dist: types-deprecated; extra == "dev"
 Requires-Dist: rtds-action; extra == "dev"
 Provides-Extra: pymc
 Requires-Dist: pymc<=5.8.2,>=5.0; extra == "pymc"
```

### Comparing `liesel-0.2.8/README.md` & `liesel-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/bijectors/algebraic_sigmoid.py` & `liesel-0.2.9/liesel/bijectors/algebraic_sigmoid.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/distributions/copulas.py` & `liesel-0.2.9/liesel/distributions/copulas.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/distributions/mvn_degen.py` & `liesel-0.2.9/liesel/distributions/mvn_degen.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/docs.py` & `liesel-0.2.9/liesel/docs.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/experimental/arviz.py` & `liesel-0.2.9/liesel/experimental/arviz.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/experimental/pymc.py` & `liesel-0.2.9/liesel/experimental/pymc.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/__init__.py` & `liesel-0.2.9/liesel/goose/__init__.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/builder.py` & `liesel-0.2.9/liesel/goose/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,39 +56,37 @@
     The general workflow usually looks something like this:
 
     #. Create a builder with :class:`.EngineBuilder`.
     #. Set the desired number of warmup and posterior samples :meth:`.set_duration`.
     #. Set the model interface with :meth:`.set_model`.
     #. Set the initial values with :meth:`.set_initial_values`.
     #. Add MCMC kernels with :meth:`.add_kernel`.
-    #. Build an :class:`.Engine` with :meth:`.build`.
+    #. Build an :class:`~.goose.Engine` with :meth:`.build`.
 
     Optionally, you can also:
 
     - Add position keys to :attr:`.positions_included` for tracking. If you are using a
       :class:`.Model` object, position keys are the names of variables or nodes in the
       model. Refer to :attr:`.positions_included` for more information.
     - Add custom jittering for start values with :meth:`.set_jitter_fns`.
 
     Parameters
     ----------
     seed
-        Either an int or a key generated from jax.random.PRNGKey.
-        Used for jittering initial values and MCMC sampling.
+        Either an int or a key generated from jax.random.PRNGKey. Used for jittering
+        initial values and MCMC sampling.
     num_chains
         The number of chains to be used.
 
     See Also
     --------
-    .Engine : The MCMC engine, output of :meth:`.build`.
-    .LieselInterface : Interface for a :class:`~liesel.model.model.Model` object.
-    .NUTSKernel : The NUTS kernel.
-    .HMCKernel : The HMC kernel.
-    .IWLSKernel : The IWLS kernel.
-    .RWKernel : The random walk kernel.
+    ~.goose.Engine : The MCMC engine, output of :meth:`.build`. ~.goose.LieselInterface
+    : Interface for a :class:`~liesel.model.model.Model` object. ~.goose.NUTSKernel :
+    The NUTS kernel. ~.goose.HMCKernel : The HMC kernel. ~.goose.IWLSKernel : The IWLS
+    kernel. ~.goose.RWKernel : The random walk kernel.
 
     Notes
     -----
 
     By default, only position keys associated with an MCMC kernel is tracked. This
     behavior can be adjusted with the fields :attr:`.positions_included` and
     :attr:`.positions_excluded`.
@@ -122,16 +120,16 @@
 
     >>> builder.add_kernel(gs.NUTSKernel(["mu"]))
 
     Finally, we build the engine:
 
     >>> engine = builder.build()
 
-    From here, you can continue with :meth:`.Engine.sample_all_epochs` to draw samples
-    from your posterior distribution.
+    From here, you can continue with :meth:`~.goose.Engine.sample_all_epochs` to draw
+    samples from your posterior distribution.
     """
 
     def __init__(self, seed: int | KeyArray, num_chains: int):
         if isinstance(seed, int):
             keys = jax.random.split(jax.random.PRNGKey(seed), 3)
         elif isinstance(seed, jax.Array):
             keys = jax.random.split(seed, 3)
@@ -157,30 +155,31 @@
         """Whether to show progress bars curing sampling."""
 
         self.positions_included: list[str] = []
         """
         List of additional position keys that should be tracked.
 
         If a position key is tracked that means the correspond element of the model
-        state will be saved and included in the :class:`.SamplingResults` and the
-        posterior samples returned by :meth:`.SamplingResults.get_posterior_samples`.
+        state will be saved and included in the :class:`~.goose.SamplingResults` and the
+        posterior samples returned by
+        :meth:`~.goose.SamplingResults.get_posterior_samples`.
 
-        By default, only position keys associated with an MCMC kernel are tracked.
-        You can easily add additional position keys by appending to this list.
+        By default, only position keys associated with an MCMC kernel are tracked. You
+        can easily add additional position keys by appending to this list.
 
         Examples
         --------
 
         For this example, we import ``tensorflow_probability`` as follows:
 
         >>> import tensorflow_probability.substrates.jax.distributions as tfd
 
-        Consider the following simple model, in which we use the logarithm of the
-        scale parameter in a normal distribution and take the exponential value for
-        including the actual scale:
+        Consider the following simple model, in which we use the logarithm of the scale
+        parameter in a normal distribution and take the exponential value for including
+        the actual scale:
 
         >>> log_scale = lsl.param(0.0, name="log_scale")
         >>> scale = lsl.Calc(jnp.exp, variance, _name="scale")
         >>> dist = lsl.Dist(tfd.Normal, loc=0.0, scale=scale)
         >>> y = lsl.obs(jnp.array([1.0, 2.0, 3.0]), dist, name="y")
         >>> model = lsl.GraphBuilder().add(y).build_model()
 
@@ -195,17 +194,17 @@
         included in the results. Now, if you also want the value of ``"scale"`` to be
         included, you can add it to the list of included position keys:
 
         >>> builder.position_keys.append("scale")
         >>> builder.position_keys
         ['scale']
 
-        Beware however that including many intermediate position keys can lead to
-        large results. In some cases it may be preferable to keep the tracked positions
-        to a minimum and recompute the intermediate values from the posterior samples.
+        Beware however that including many intermediate position keys can lead to large
+        results. In some cases it may be preferable to keep the tracked positions to a
+        minimum and recompute the intermediate values from the posterior samples.
 
         """
         self.positions_excluded: list[str] = []
         """List of position keys that should not be tracked. Excluded keys override
         additional keys."""
 
     def set_engine_seed(self, seed: int | KeyArray):
@@ -300,15 +299,15 @@
 
         Now, we can create the model with :class:`.GraphBuilder`.
 
         >>> gb = lsl.GraphBuilder().add(x)
         >>> model = gb.build_model()
 
         Finally, we build the model with :class:`.EngineBuilder`. We will use 4
-        parallel chains and sample our varaible using a :class:`.NUTSKernel`.
+        parallel chains and sample our varaible using a :class:`~.goose.NUTSKernel`.
 
         >>> builder = gs.EngineBuilder(seed=1337, num_chains=4)
         >>> builder.set_model(gs.LieselInterface(model))
         >>> builder.set_initial_values(model.state)
         >>> builder.add_kernel(gs.NUTSKernel(["mu"]))
 
         A jitter function takes as input a key and value and applies random jittering
```

### Comparing `liesel-0.2.8/liesel/goose/chain.py` & `liesel-0.2.9/liesel/goose/chain.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/da.py` & `liesel-0.2.9/liesel/goose/da.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/engine.py` & `liesel-0.2.9/liesel/goose/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
 @dataclass
 class SamplingResults:
     """
     Contains the results of the MCMC engine.
 
     Easy access to the samples is provided via the methods
-    :func:`.get_samples` and :func:`.get_posterior_samples`.
+    :meth:`.get_samples` and :meth:`.get_posterior_samples`.
     """
 
     positions: EpochChainManager
     """EpochChainManager giving access to monitored variables."""
     transition_infos: EpochChainManager
     """EpochChainManager storing all transition infos."""
     generated_quantities: Option[EpochChainManager]
@@ -285,22 +285,15 @@
 
 @deprecated(
     reason="Use SamplingResults. This alias will be removed in v0.4.0", version="0.1.4"
 )
 class SamplingResult(SamplingResults):
     """Alias of :class:`.SamplingResults` for backwards compatibility."""
 
-    positions: EpochChainManager
-    transition_infos: EpochChainManager
-    generated_quantities: Option[EpochChainManager]
-    tuning_infos: Option[Chain]
-    kernel_states: Option[EpochChainManager]
-    full_model_states: Option[EpochChainManager]
-    kernel_classes: Option[dict[str, type]]
-    kernels_by_pos_key: Option[dict[str, str]]
+    pass
 
 
 class Engine:
     """MCMC engine capable of combining multiple transition kernels."""
 
     def __init__(
         self,
@@ -638,17 +631,15 @@
         KernelStates,
         ModelState,
         Position,
         TransitionInfos,
         None | KernelStates,
         None | dict[str, GeneratedQuantity],
     ]:
-        def scan_f(
-            carry: Carry, key: KeyArray
-        ) -> tuple[
+        def scan_f(carry: Carry, key: KeyArray) -> tuple[
             Carry,
             tuple[
                 Position,
                 TransitionInfos,
                 None | KernelStates,
                 None | dict[str, GeneratedQuantity],
             ],
```

### Comparing `liesel-0.2.8/liesel/goose/epoch.py` & `liesel-0.2.9/liesel/goose/epoch.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     def is_warmup(epoch_type: EpochType) -> bool:
         """
         Returns ``True`` if the epoch is part of the warmup phase.
         Implemented as a static method to make it jittable.
         """
         rhs = EpochType.INITIAL_VALUES < epoch_type
         lhs = epoch_type < EpochType.POSTERIOR
-        # using `*` instead of `and` for jax.jit
+
+        # using ``*``` instead of ``and`` for jax.jit
         # `cast` is a no-op used to satisfy mypy
         return cast(bool, lhs * rhs)
 
 
 @register_dataclass_as_pytree
 @dataclass
 class EpochConfig:
```

### Comparing `liesel-0.2.8/liesel/goose/gibbs.py` & `liesel-0.2.9/liesel/goose/gibbs.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/hmc.py` & `liesel-0.2.9/liesel/goose/hmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     """
 
     error_book: ClassVar[dict[int, str]] = {0: "no errors", 1: "divergent transition"}
     """Dict of error codes and their meaning."""
     needs_history: ClassVar[bool] = True
     """Whether this kernel needs its history for tuning."""
     identifier: str = ""
-    """Kernel identifier, set by :class:`.EngineBuilder`"""
+    """Kernel identifier, set by :class:`~.goose.EngineBuilder`"""
     position_keys: tuple[str, ...]
     """Tuple of position keys handled by this kernel."""
 
     def __init__(
         self,
         position_keys: Sequence[str],
         initial_step_size: float | None = None,
```

### Comparing `liesel-0.2.8/liesel/goose/interface.py` & `liesel-0.2.9/liesel/goose/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     >>> y = lsl.obs(jnp.array([1.0, 2.0, 3.0]), name="y")
     >>> model = lsl.GraphBuilder().add(y).build_model()
 
     The interface is initialized by passing the model to the constructor.
 
     >>> interface = gs.LieselInterface(model)
 
-    The interface instance can now be used in :meth:`.EngineBuilder.set_model`.
+    The interface instance can now be used in :meth:`~.goose.EngineBuilder.set_model`.
     """
 
     def __init__(self, model: "Model"):
         self._model = model._copy_computational_model()
 
     def extract_position(
         self, position_keys: Sequence[str], model_state: ModelState
```

### Comparing `liesel-0.2.8/liesel/goose/iwls.py` & `liesel-0.2.9/liesel/goose/iwls.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     """
 
     error_book: ClassVar[dict[int, str]] = {0: "no errors", 90: "nan acceptance prob"}
     """Dict of error codes and their meaning."""
     needs_history: ClassVar[bool] = False
     """Whether this kernel needs its history for tuning."""
     identifier: str = ""
-    """Kernel identifier, set by :class:`.EngineBuilder`"""
+    """Kernel identifier, set by :class:`~.goose.EngineBuilder`"""
     position_keys: tuple[str, ...]
     """Tuple of position keys handled by this kernel."""
 
     def __init__(
         self,
         position_keys: Sequence[str],
         chol_info_fn: Callable[[ModelState], Array] | None = None,
```

### Comparing `liesel-0.2.8/liesel/goose/iwls_utils.py` & `liesel-0.2.9/liesel/goose/iwls_utils.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/kernel.py` & `liesel-0.2.9/liesel/goose/kernel.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/kernel_sequence.py` & `liesel-0.2.9/liesel/goose/kernel_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """Organizes a sequence of kernels."""
 
     def __init__(self, kernels: Sequence[Kernel]) -> None:
         identifiers = set()
         for ker in kernels:
             if not ker.identifier:
                 raise RuntimeError(
-                    f"Kernel identifier must be a non-empty string. "
+                    "Kernel identifier must be a non-empty string. "
                     f"The field is empty in {ker!r}."
                 )
             identifiers.add(ker.identifier)
 
         if len(identifiers) < len(kernels):
             raise RuntimeError("Kernel identifier must be unique.")
```

### Comparing `liesel-0.2.8/liesel/goose/mh.py` & `liesel-0.2.9/liesel/goose/mh.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/mh_kernel.py` & `liesel-0.2.9/liesel/goose/mh_kernel.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/mm.py` & `liesel-0.2.9/liesel/goose/mm.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/models.py` & `liesel-0.2.9/liesel/goose/models.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/nuts.py` & `liesel-0.2.9/liesel/goose/nuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         3: "divergent transition + maximum tree depth",
     }
     """Dict of error codes and their meaning."""
 
     needs_history: ClassVar[bool] = True
     """Whether this kernel needs its history for tuning."""
     identifier: str = ""
-    """Kernel identifier, set by :class:`.EngineBuilder`"""
+    """Kernel identifier, set by :class:`~.goose.EngineBuilder`"""
     position_keys: tuple[str, ...]
     """Tuple of position keys handled by this kernel."""
 
     def __init__(
         self,
         position_keys: Sequence[str],
         initial_step_size: float | None = None,
```

### Comparing `liesel-0.2.8/liesel/goose/pytree.py` & `liesel-0.2.9/liesel/goose/pytree.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/rw.py` & `liesel-0.2.9/liesel/goose/rw.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """
 
     error_book: ClassVar[dict[int, str]] = {0: "no errors", 90: "nan acceptance prob"}
     """Dict of error codes and their meaning."""
     needs_history: ClassVar[bool] = False
     """Whether this kernel needs its history for tuning."""
     identifier: str = ""
-    """Kernel identifier, set by :class:`.EngineBuilder`"""
+    """Kernel identifier, set by :class:`~.goose.EngineBuilder`"""
     position_keys: tuple[str, ...]
     """Tuple of position keys handled by this kernel."""
 
     def __init__(
         self,
         position_keys: Sequence[str],
         initial_step_size: float = 1.0,
```

### Comparing `liesel-0.2.8/liesel/goose/summary_m.py` & `liesel-0.2.9/liesel/goose/summary_m.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     Parameters
     ----------
     results
         The sampling results to summarize.
     additional_chain
         can be supplied to add more parameters to the summary output. Must be a position
         chain which matches chain and time dimension of the posterior chain as returned
-        by :meth:`.SamplingResults.get_posterior_samples`.
+        by :meth:`~.goose.SamplingResults.get_posterior_samples`.
     hdi_prob
         Level on which to return posterior highest density intervals.
     selected, deselected
         Allow to get a summary only for a subset of the position keys.
     per_chain
         If *True*, the summary is calculated on a per-chain basis. Certain measures like
         ``rhat`` are not available if ``per_chain`` is *True*.
```

### Comparing `liesel-0.2.8/liesel/goose/summary_viz.py` & `liesel-0.2.9/liesel/goose/summary_viz.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/types.py` & `liesel-0.2.9/liesel/goose/types.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/goose/warmup.py` & `liesel-0.2.9/liesel/goose/warmup.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/logging.py` & `liesel-0.2.9/liesel/logging.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/model/__init__.py` & `liesel-0.2.9/liesel/model/__init__.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/model/distreg.py` & `liesel-0.2.9/liesel/model/distreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,19 +279,20 @@
     model: Model,
     seed: int,
     num_chains: int,
     tau2_jitter_fn: JitterFunction = tau2_jitter_fn,
     beta_jitter_fn: JitterFunction = beta_jitter_fn,
 ) -> EngineBuilder:
     """
-    Configures an :class:`.EngineBuilder` for a distributional regression model.
+    Configures an :class:`~.goose.EngineBuilder` for a distributional regression model.
 
     The EngineBuilder uses a Metropolis-in-Gibbs MCMC algorithm with an
-    :class:`.IWLSKernel` for the regression coefficients and a :class:`.GibbsKernel` for
-    the smoothing parameters for a distributional regression model.
+    :class:`~.goose.IWLSKernel` for the regression coefficients and a
+    :class:`~.goose.GibbsKernel` for the smoothing parameters for a distributional
+    regression model.
 
     Parameters
     ----------
     model
         A model built with a :class:`.DistRegBuilder`.
     seed
         The PRNG seed for the engine builder.
@@ -299,15 +300,16 @@
         The number of chains to be sampled.
     tau2_jitter_fn
         Jittering function for the smoothing parameters.
     beta_jitter_fn
         Jittering function for the regression coefficients.
     See Also
     --------
-    :meth:`.EngineBuilder.set_jitter_fns` : Method for setting the jittering functions
+    :meth:`~.goose.EngineBuilder.set_jitter_fns` : Method for setting the jittering
+        functions
     """
 
     builder = EngineBuilder(seed, num_chains)
 
     builder.set_model(LieselInterface(model))
     builder.set_initial_values(model.state)
```

### Comparing `liesel-0.2.8/liesel/model/goose.py` & `liesel-0.2.9/liesel/model/goose.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 from .model import Model
 
 
 class GooseModel:
     """
     A :class:`.ModelInterface` for a Liesel :class:`.Model`.
 
-    This is an alias for :class:`.LieselInterface` provided for backwards compatibility.
+    This is an alias for :class:`~.goose.LieselInterface` provided for backwards
+    compatibility.
 
     .. deprecated:: v0.2.6
-        Use :class:`.LieselInterface` instead. This alias will be removed in v0.4.0.
+        Use :class:`~.goose.LieselInterface` instead. This alias will be removed in
+        v0.4.0.
 
     Parameters
     ----------
     model
         A Liesel :class:`.Model`.
     """
 
     def __init__(self, model: Model):
         self._model = model._copy_computational_model()
         warnings.warn(
-            (
-                "lsl.GooseModel is deprecated. Use gs.LieselInterface instead."
-                "This alias will be removed in v0.4.0."
-            ),
+            "lsl.GooseModel is deprecated. Use gs.LieselInterface instead."
+            "This alias will be removed in v0.4.0.",
             FutureWarning,
         )
 
     def extract_position(
         self, position_keys: Iterable[str], model_state: ModelState
     ) -> Position:
         """
```

### Comparing `liesel-0.2.8/liesel/model/legacy.py` & `liesel-0.2.9/liesel/model/legacy.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel/model/model.py` & `liesel-0.2.9/liesel/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,15 @@
     def _all_nodes_and_vars(self) -> tuple[list[Node], list[Var]]:
         """
         Returns all nodes and variables that were explicitly or implicitly
         (as recursive inputs) added to the graph.
         """
         nodes = self.nodes.copy()
         nodes.extend(node for var in self.vars for node in var.nodes)
+
         nodes = list(dict.fromkeys(nodes))
 
         if self.log_lik_node:
             nodes.append(self.log_lik_node)
 
         if self.log_prior_node:
             nodes.append(self.log_prior_node)
@@ -758,14 +759,21 @@
 
         if var.dist_node is None:
             raise RuntimeError(f"{repr(var)} has no distribution")
 
         # avoid name clashes
         self._set_missing_names()
 
+        if var.value_node in self.nodes:
+            raise RuntimeError(
+                f"{var.value_node.name} is already present in the GraphBuilder. "
+                + "If you have added some Node objects to the GraphBuilder, "
+                "try to add only the Var objects instead."
+            )
+
         # avoid infinite recursion
         var.auto_transform = False
 
         try:
             Model([var])
         except Exception:
             raise RuntimeError(f"Cannot build local model for {repr(var)}")
```

### Comparing `liesel-0.2.8/liesel/model/nodes.py` & `liesel-0.2.9/liesel/model/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Nodes and variables.
 """
 
 from __future__ import annotations
 
+import logging
 import warnings
 import weakref
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Hashable, Iterable
 from functools import wraps
 from itertools import chain
 from types import MappingProxyType
@@ -46,14 +47,16 @@
 
 Array = Any
 Distribution = Union[jd.Distribution, nd.Distribution]
 Bijector = Union[jb.Bijector, nb.Bijector]
 
 T = TypeVar("T", bound=Hashable)
 
+logger = logging.getLogger(__name__)
+
 
 def _unique_tuple(*args: Iterable[T]) -> tuple[T, ...]:
     return tuple(dict.fromkeys(chain(*args)))
 
 
 def in_model_method(fn):
     @wraps(fn)
@@ -455,15 +458,15 @@
         args = [_input.value for _input in self.inputs]
         kwargs = {kw: _input.value for kw, _input in self.kwinputs.items()}
         return ArgGroup(args, kwargs)
 
 
 class Data(Node):
     """
-    A :class:`.Node` subclass that holds constant data.
+    A :class:`.Node` subclass that holds constant values.
 
     Since the value represented by a data node does not change, it is always up-to-date.
     A common usecase for data nodes is to cache computed values.
 
     - By default, data nodes *will* appear in the node graph created by
       :func:`.viz.plot_nodes`, but they will *not* appear in the model graph created by
       :func:`.viz.plot_vars`.
@@ -577,14 +580,17 @@
         will be converted to :class:`.Data` nodes. The values of these inputs will be
         passed to the wrapped function in the same order they are entered here.
     _name
         The name of the node. If you do not specify a name, a unique name will be \
         automatically generated upon initialization of a :class:`.Model`.
     _needs_seed
         Whether the node needs a seed / PRNG key.
+    update_on_init
+        If ``True``, the calculator will try to evaluate its function upon \
+        initialization.
     **kwinputs
         Keyword inputs. Any inputs that are not already nodes or :class:`.Var`s
         will be converted to :class:`.Data` nodes. The values of these inputs will be
         passed to the wrapped function as keyword arguments.
 
     See Also
     --------
@@ -608,21 +614,20 @@
     this method is called is during the initialization of a :class:`.Model`, which might
     make it hard to spot errors in the wrapped computations. To update the value
     immediately, you can call :meth:`.Calc.update` manually.
 
     Examples
     --------
 
-    A simple calculator node, taking the exponential value of an input parameter. This
-    calculator node has not updated its value yet.
+    A simple calculator node, taking the exponential value of an input parameter.
 
     >>> log_scale = lsl.param(0.0, name="log_scale")
     >>> scale = lsl.Calc(jnp.exp, log_scale)
     >>> print(scale.value)
-    None
+    1.0
 
     The value of the calculator node is updated when :meth:`.Calc.update` is called.
 
     >>> scale.update()
     Calc(name="")
     >>> print(scale.value)
     1.0
@@ -658,19 +663,35 @@
 
     def __init__(
         self,
         function: Callable[..., Any],
         *inputs: Any,
         _name: str = "",
         _needs_seed: bool = False,
+        update_on_init: bool = True,
         **kwinputs: Any,
     ):
         super().__init__(*inputs, **kwinputs, _name=_name, _needs_seed=_needs_seed)
         self._function = function
 
+        if update_on_init:
+            try:
+                self.update()
+            except Exception as e:
+                logger.warning(
+                    f"{self} was not updated during initialization, because the"
+                    f" following exception occured: {repr(e)}. See debug log for the"
+                    " full traceback."
+                )
+                logger.debug(
+                    f"{self} was not updated during initialization, because the"
+                    " following exception occured:",
+                    exc_info=e,
+                )
+
     @property
     def function(self) -> Callable[..., Any]:
         """The wrapped function."""
         return self._function
 
     @function.setter
     @no_model_setter
```

### Comparing `liesel-0.2.8/liesel/model/viz.py` & `liesel-0.2.9/liesel/model/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,17 +142,19 @@
     )
 
 
 def _add_labels(graph, axis, pos):
     """Adds labels to the figure."""
 
     labels = {
-        node: f"{type(node).__name__}\n{node.name}"
-        if node.name is not None
-        else node.role.name
+        node: (
+            f"{type(node).__name__}\n{node.name}"
+            if node.name is not None
+            else node.role.name
+        )
         for node in pos
     }
 
     nx.draw_networkx_labels(graph, pos, labels=labels, ax=axis, font_size=10)
 
 
 def _draw_edges(graph, axis, pos, is_var):
```

### Comparing `liesel-0.2.8/liesel/option.py` & `liesel-0.2.9/liesel/option.py`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/liesel.egg-info/PKG-INFO` & `liesel-0.2.9/liesel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liesel
-Version: 0.2.8
+Version: 0.2.9
 Summary: A probabilistic programming framework with a focus on semi-parametric regression
 Home-page: https://liesel-project.org
 Author: Paul Wiemann, Hannes Riebl, Johannes Brachem, Gianmarco Callegher
 License: MIT
 Keywords: statistics,machine-learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,32 +18,32 @@
 Requires-Dist: dill>=0.3
 Requires-Dist: jax>=0.4.1
 Requires-Dist: jaxlib>=0.4.1
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: networkx>=2.6
 Requires-Dist: numpy!=1.24.0,>=1.22
 Requires-Dist: pandas>=1.4
-Requires-Dist: scipy>=1.8
+Requires-Dist: scipy<=1.12.0,>=1.8
 Requires-Dist: seaborn>=0.13
 Requires-Dist: tensorflow-probability>=0.17
 Requires-Dist: tqdm>=4.62
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: myst-nb; extra == "dev"
+Requires-Dist: myst-nb>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pyupgrade; extra == "dev"
-Requires-Dist: sphinx>=4.5; extra == "dev"
+Requires-Dist: sphinx>=7.2.6; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints>=1.19; extra == "dev"
 Requires-Dist: pydata-sphinx-theme; extra == "dev"
-Requires-Dist: sphinx-book-theme>=1.0.1; extra == "dev"
+Requires-Dist: sphinx-book-theme>=1.1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton>=0.5; extra == "dev"
 Requires-Dist: sphinx-remove-toctrees>=0.0.3; extra == "dev"
 Requires-Dist: types-deprecated; extra == "dev"
 Requires-Dist: rtds-action; extra == "dev"
 Provides-Extra: pymc
 Requires-Dist: pymc<=5.8.2,>=5.0; extra == "pymc"
```

### Comparing `liesel-0.2.8/liesel.egg-info/SOURCES.txt` & `liesel-0.2.9/liesel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/pyproject.toml` & `liesel-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `liesel-0.2.8/setup.cfg` & `liesel-0.2.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -23,34 +23,34 @@
 	dill>=0.3
 	jax>=0.4.1
 	jaxlib>=0.4.1
 	matplotlib>=3.5
 	networkx>=2.6
 	numpy>=1.22,!=1.24.0
 	pandas>=1.4
-	scipy>=1.8
+	scipy>=1.8, <=1.12.0
 	seaborn>=0.13
 	tensorflow-probability>=0.17
 	tqdm>=4.62
 
 [options.extras_require]
 dev = 
 	black
 	flake8
 	isort
 	mypy
-	myst-nb
+	myst-nb>=1.0.0
 	pre-commit
 	pytest
 	pytest-cov
 	pyupgrade
-	sphinx>=4.5
+	sphinx>=7.2.6
 	sphinx-autodoc-typehints>=1.19
 	pydata-sphinx-theme
-	sphinx-book-theme>=1.0.1
+	sphinx-book-theme>=1.1.0
 	sphinx-copybutton>=0.5
 	sphinx-remove-toctrees>=0.0.3
 	types-deprecated
 	rtds-action
 pymc = 
 	pymc>=5.0,<=5.8.2
```

### Comparing `liesel-0.2.8/tests/test_option.py` & `liesel-0.2.9/tests/test_option.py`

 * *Files identical despite different names*

