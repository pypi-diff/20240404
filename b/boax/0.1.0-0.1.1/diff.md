# Comparing `tmp/boax-0.1.0.tar.gz` & `tmp/boax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boax-0.1.0.tar", last modified: Sat Mar  2 12:39:40 2024, max compression
+gzip compressed data, was "boax-0.1.1.tar", last modified: Thu Apr  4 20:46:33 2024, max compression
```

## Comparing `boax-0.1.0.tar` & `boax-0.1.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.568542 boax-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-02 12:39:27.000000 boax-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-02 12:39:40.568542 boax-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-02 12:39:27.000000 boax-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.556542 boax-0.1.0/boax/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-02 12:39:27.000000 boax-0.1.0/boax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.556542 boax-0.1.0/boax/core/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.556542 boax-0.1.0/boax/core/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/distributions/multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/distributions/poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/distributions/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.556542 boax-0.1.0/boax/core/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/samplers/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/samplers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.556542 boax-0.1.0/boax/core/samplers/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/samplers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/samplers/functions/quasi_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-02 12:39:27.000000 boax-0.1.0/boax/core/samplers/functions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.560542 boax-0.1.0/boax/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.560542 boax-0.1.0/boax/optimization/acquisitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/acquisitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/acquisitions/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/acquisitions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.560542 boax-0.1.0/boax/optimization/acquisitions/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/acquisitions/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/acquisitions/functions/analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/acquisitions/functions/monte_carlo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.560542 boax-0.1.0/boax/optimization/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/constraints/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/constraints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/construction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.560542 boax-0.1.0/boax/optimization/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/optimizers/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/optimizers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.560542 boax-0.1.0/boax/optimization/optimizers/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/optimizers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/optimizers/functions/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-02 12:39:27.000000 boax-0.1.0/boax/optimization/optimizers/functions/scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.560542 boax-0.1.0/boax/prediction/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/construction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.560542 boax-0.1.0/boax/prediction/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.564542 boax-0.1.0/boax/prediction/kernels/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/functions/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/functions/matern.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/functions/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/functions/rbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/kernels/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.564542 boax-0.1.0/boax/prediction/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/likelihoods/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/likelihoods/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.564542 boax-0.1.0/boax/prediction/likelihoods/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/likelihoods/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/likelihoods/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/likelihoods/functions/marginal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.564542 boax-0.1.0/boax/prediction/means/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/means/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/means/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/means/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.564542 boax-0.1.0/boax/prediction/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/models/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.564542 boax-0.1.0/boax/prediction/models/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/models/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/models/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/models/functions/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/models/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.564542 boax-0.1.0/boax/prediction/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/objectives/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/objectives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-02 12:39:27.000000 boax-0.1.0/boax/prediction/objectives/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.568542 boax-0.1.0/boax/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-02 12:39:27.000000 boax-0.1.0/boax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-03-02 12:39:27.000000 boax-0.1.0/boax/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-02 12:39:27.000000 boax-0.1.0/boax/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-02 12:39:27.000000 boax-0.1.0/boax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 12:39:40.568542 boax-0.1.0/boax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-02 12:39:40.000000 boax-0.1.0/boax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-02 12:39:40.000000 boax-0.1.0/boax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 12:39:40.000000 boax-0.1.0/boax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-02 12:39:40.000000 boax-0.1.0/boax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-02 12:39:40.000000 boax-0.1.0/boax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-02 12:39:27.000000 boax-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 12:39:40.568542 boax-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.501217 boax-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 20:46:22.000000 boax-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-04 20:46:33.501217 boax-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-04 20:46:22.000000 boax-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-04 20:46:22.000000 boax-0.1.1/boax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/core/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/transformed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/distributions/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/core/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/core/samplers/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/functions/quasi_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-04 20:46:22.000000 boax-0.1.1/boax/core/samplers/functions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.489217 boax-0.1.1/boax/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/acquisitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/acquisitions/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/constraints/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/constraints/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/acquisitions/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/functions/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/functions/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/acquisitions/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/optimization/optimizers/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/functions/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-04 20:46:22.000000 boax-0.1.1/boax/optimization/optimizers/functions/scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/prediction/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.493217 boax-0.1.1/boax/prediction/models/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/functions/multi_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/kernels/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/matern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/kernels/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/likelihoods/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/likelihoods/functions/marginal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/models/means/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/means/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/means/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/means/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/models/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/prediction/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/objectives/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/objectives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-04 20:46:22.000000 boax-0.1.1/boax/prediction/objectives/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-04 20:46:22.000000 boax-0.1.1/boax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-04 20:46:22.000000 boax-0.1.1/boax/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-04 20:46:22.000000 boax-0.1.1/boax/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-04 20:46:22.000000 boax-0.1.1/boax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:46:33.497217 boax-0.1.1/boax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 20:46:33.000000 boax-0.1.1/boax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-04 20:46:22.000000 boax-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:46:33.501217 boax-0.1.1/setup.cfg
```

### Comparing `boax-0.1.0/LICENSE` & `boax-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/PKG-INFO` & `boax-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boax
-Version: 0.1.0
+Version: 0.1.1
 Summary: Boax is a Bayesian Optimization library for JAX.
 Project-URL: homepage, https://github.com/Lando-L/boax
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
@@ -72,70 +72,70 @@
 
 ```sh
 pip install git+https://github.com/Lando-L/boax.git
 ```
 
 ## Basic Usage
 
-Here is a basic example of using the Boax API for Bayesian Optimization. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
+Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and combining the two for optimzation. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
 
-1. Creation of a prediction model.
+1. Defining a Gaussian Process model:
 
 ```python
-def model(params):
-  return models.outcome_transformed(
-    models.gaussian_process_regression(
-      means.zero(),
-      kernels.rbf(params['length_scale']),
-    )(
-      x_train,
-      y_train,
-    ),
-    likelihoods.gaussian(params['noise']),
-  )
+from boax.prediction import models
+
+model = models.gaussian_process(
+  models.means.zero(),
+  models.kernels.scaled(
+    models.kernels.rbf(1.0),
+    0.5
+  ),
+  models.likelihoods.gaussian(1e-4),
+  x_train,
+  y_train,
+)
 ```
 
-2. Construction of an acquisition function.
+2. Constructing an Acquisition function.
 
 ```python
-def construct(model):
-  return optimization.construct(
-    models.outcome_transformed(
-      model,
-      distributions.multivariate_normal.as_normal,
-    ),
-    acquisitions.upper_confidence_bound(
-      beta=2.0
-    ),
-  )
+from boax.optimization import acquisitions
+
+acquisition = acquisitions.upper_confidence_bound(
+  beta=2.0
+)
 ```
 
-3. Selection of the next candidate to query.
+3. Combining the two for optimization
 
 ```python
-def select(key, acqf):
-    bfgs = optimizers.bfgs(acqf, bounds, x0, 10)
-    candidates = bfgs.init(key)
-    next_candidates, values = bfgs.update(candidates)
-
-    next_x = next_candidates[jnp.argmax(values)]
-    next_y = objective(next_x)
-
-    return next_x, next_y
+from jax import jit, random, vmap
+from jax import numpy as jnp
+from boax.optimization import optimizers
+
+def acqf(x):
+  return acquisition(vmap(model)(x))
+
+key1, key2 = random.split(random.key(0))
+bounds = jnp.array([[-1.0, 1.0]])
+x0 = random.uniform(key1, shape=(100, 1, 1))
+bfgs = optimizers.bfgs(jit(acqf), bounds, x0, 10)
+candidates = bfgs.init(key2)
+next_candidates, values = bfgs.update(candidates)
 ```
 
 ## Citing Boax
 
 To cite Boax please use the citation:
 
 ```bibtex
 @software{boax2023github,
   author = {Lando L{\"o}per},
   title = {{B}oax: A Bayesian Optimization library for {JAX}},
   url = {https://github.com/Lando-L/boax},
-  version = {0.1.0},
+  version = {0.1.1},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, the version number
 is intended to be that from [boax/version.py](https://github.com/Lando-L/boax/blob/main/boax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `boax-0.1.0/README.md` & `boax-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -40,70 +40,70 @@
 
 ```sh
 pip install git+https://github.com/Lando-L/boax.git
 ```
 
 ## Basic Usage
 
-Here is a basic example of using the Boax API for Bayesian Optimization. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
+Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and combining the two for optimzation. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
 
-1. Creation of a prediction model.
+1. Defining a Gaussian Process model:
 
 ```python
-def model(params):
-  return models.outcome_transformed(
-    models.gaussian_process_regression(
-      means.zero(),
-      kernels.rbf(params['length_scale']),
-    )(
-      x_train,
-      y_train,
-    ),
-    likelihoods.gaussian(params['noise']),
-  )
+from boax.prediction import models
+
+model = models.gaussian_process(
+  models.means.zero(),
+  models.kernels.scaled(
+    models.kernels.rbf(1.0),
+    0.5
+  ),
+  models.likelihoods.gaussian(1e-4),
+  x_train,
+  y_train,
+)
 ```
 
-2. Construction of an acquisition function.
+2. Constructing an Acquisition function.
 
 ```python
-def construct(model):
-  return optimization.construct(
-    models.outcome_transformed(
-      model,
-      distributions.multivariate_normal.as_normal,
-    ),
-    acquisitions.upper_confidence_bound(
-      beta=2.0
-    ),
-  )
+from boax.optimization import acquisitions
+
+acquisition = acquisitions.upper_confidence_bound(
+  beta=2.0
+)
 ```
 
-3. Selection of the next candidate to query.
+3. Combining the two for optimization
 
 ```python
-def select(key, acqf):
-    bfgs = optimizers.bfgs(acqf, bounds, x0, 10)
-    candidates = bfgs.init(key)
-    next_candidates, values = bfgs.update(candidates)
-
-    next_x = next_candidates[jnp.argmax(values)]
-    next_y = objective(next_x)
-
-    return next_x, next_y
+from jax import jit, random, vmap
+from jax import numpy as jnp
+from boax.optimization import optimizers
+
+def acqf(x):
+  return acquisition(vmap(model)(x))
+
+key1, key2 = random.split(random.key(0))
+bounds = jnp.array([[-1.0, 1.0]])
+x0 = random.uniform(key1, shape=(100, 1, 1))
+bfgs = optimizers.bfgs(jit(acqf), bounds, x0, 10)
+candidates = bfgs.init(key2)
+next_candidates, values = bfgs.update(candidates)
 ```
 
 ## Citing Boax
 
 To cite Boax please use the citation:
 
 ```bibtex
 @software{boax2023github,
   author = {Lando L{\"o}per},
   title = {{B}oax: A Bayesian Optimization library for {JAX}},
   url = {https://github.com/Lando-L/boax},
-  version = {0.1.0},
+  version = {0.1.1},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, the version number
 is intended to be that from [boax/version.py](https://github.com/Lando-L/boax/blob/main/boax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `boax-0.1.0/boax/__init__.py` & `boax-0.1.1/boax/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The boax API."""
+"""The optimization module."""
 
-from . import optimization as optimization
-from . import prediction as prediction
+from . import functools as functools
+from . import typing as typing
```

### Comparing `boax-0.1.0/boax/core/__init__.py` & `boax-0.1.1/boax/core/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/distributions/__init__.py` & `boax-0.1.1/boax/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The samplers sub-package."""
+"""The boax API."""
 
-from . import beta as beta
-from . import gamma as gamma
-from . import multivariate_normal as multivariate_normal
-from . import normal as normal
-from . import poisson as poisson
-from . import uniform as uniform
+from . import core as core
+from . import optimization as optimization
+from . import prediction as prediction
+from . import utils as utils
```

### Comparing `boax-0.1.0/boax/core/distributions/beta.py` & `boax-0.1.1/boax/core/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/distributions/gamma.py` & `boax-0.1.1/boax/core/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/distributions/multivariate_normal.py` & `boax-0.1.1/boax/core/distributions/multivariate_normal.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 """The multivariate normal distribution."""
 
 from typing import NamedTuple
 
 from jax import numpy as jnp
 from jax import scipy
 
-from boax.core.distributions.normal import Normal
 from boax.utils.typing import Array
 
 
 class MultivariateNormal(NamedTuple):
   """
   A tuple describing the two parameters of the multivariate normal distribution.
 
@@ -49,44 +48,47 @@
   Returns:
     The `MultivariateNormal` distribution object.
   """
 
   return MultivariateNormal(mean, cov)
 
 
-def as_normal(mvn: MultivariateNormal) -> Normal:
+def sample(mvn: MultivariateNormal, base_samples: Array) -> Array:
   """
-  Transforms a multivariate normal distribution
-  into a batched normal distribution.
+  Samples a multivariate normal distribution based on base samples.
 
   Args:
     mvn: The multivariate normal distribution.
+    base_samples: The normal distributed base samples.
 
   Returns:
-    The batched `Normal` distribution object.
+    The samples from the multivariate normal distribution.
   """
 
-  return Normal(mvn.mean, jnp.sqrt(jnp.diag(mvn.cov)))
+  return mvn.mean + jnp.dot(
+    scipy.linalg.cholesky(mvn.cov, lower=True), base_samples
+  )
 
 
-def sample(mvn: MultivariateNormal, base_samples: Array) -> Array:
+def scale(
+  mvn: MultivariateNormal, loc: Array, scale: Array
+) -> MultivariateNormal:
   """
-  Samples a multivariate normal distribution based on base samples.
+  Scales a normal distribution.
 
   Args:
-    mvn: The multivariate normal distribution.
-    base_samples: The normal distributed base samples.
+    normal: The normal distribution.
+    loc: The location parameter.
+    scale: The scale parameter
 
   Returns:
-    The samples from the multivariate normal distribution.
+    The scaled normal distribution.
   """
 
-  return mvn.mean + jnp.dot(
-    scipy.linalg.cholesky(mvn.cov, lower=True), base_samples
-  )
+  return MultivariateNormal(mvn.mean * scale + loc, mvn.cov)
 
 
 def pdf(mvn: MultivariateNormal, values: Array) -> Array:
   """
   Probability density function.
 
   Args:
```

### Comparing `boax-0.1.0/boax/core/distributions/normal.py` & `boax-0.1.1/boax/core/distributions/normal.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,30 @@
   Returns:
     The samples from the normal distribution.
   """
 
   return normal.loc + base_samples * normal.scale
 
 
+def scale(normal: Normal, loc: Array, scale: Array) -> Normal:
+  """
+  Scales a normal distribution.
+
+  Args:
+    normal: The normal distribution.
+    loc: The location parameter.
+    scale: The scale parameter
+
+  Returns:
+    The scaled normal distribution.
+  """
+
+  return Normal(normal.loc * scale + loc, normal.scale)
+
+
 def pdf(normal: Normal, x: Array) -> Array:
   """
   Probability density function.
 
   Args:
     normal: The normal distribution.
     values: The values to evaluate.
```

### Comparing `boax-0.1.0/boax/core/distributions/poisson.py` & `boax-0.1.1/boax/core/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/distributions/uniform.py` & `boax-0.1.1/boax/core/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/samplers/__init__.py` & `boax-0.1.1/boax/core/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/samplers/alias.py` & `boax-0.1.1/boax/core/samplers/alias.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/samplers/base.py` & `boax-0.1.1/boax/core/samplers/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/samplers/functions/__init__.py` & `boax-0.1.1/boax/core/samplers/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/samplers/functions/quasi_random.py` & `boax-0.1.1/boax/core/samplers/functions/quasi_random.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/core/samplers/functions/utils.py` & `boax-0.1.1/boax/core/samplers/functions/utils.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/__init__.py` & `boax-0.1.1/boax/optimization/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,12 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """The optimization module."""
 
 from . import acquisitions as acquisitions
-from . import constraints as constraints
 from . import optimizers as optimizers
-from .construction import construct as construct
-from .construction import construct_constrained as construct_constrained
-from .construction import construct_log_constrained as construct_log_constrained
```

### Comparing `boax-0.1.0/boax/optimization/acquisitions/__init__.py` & `boax-0.1.1/boax/optimization/acquisitions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """The acquisitions sub-package."""
 
+from . import constraints as constraints
 from .alias import expected_improvement as expected_improvement
 from .alias import log_expected_improvement as log_expected_improvement
 from .alias import (
   log_probability_of_improvement as log_probability_of_improvement,
 )
 from .alias import posterior_mean as posterior_mean
 from .alias import posterior_scale as posterior_scale
 from .alias import probability_of_improvement as probability_of_improvement
 from .alias import q_expected_improvement as q_expected_improvement
 from .alias import q_knowledge_gradient as q_knowledge_gradient
 from .alias import q_probability_of_improvement as q_probability_of_improvement
 from .alias import q_upper_confidence_bound as q_upper_confidence_bound
 from .alias import upper_confidence_bound as upper_confidence_bound
 from .base import Acquisition as Acquisition
+from .transformed import constrained as constrained
+from .transformed import log_constrained as log_constrained
```

### Comparing `boax-0.1.0/boax/optimization/acquisitions/alias.py` & `boax-0.1.1/boax/optimization/acquisitions/alias.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/acquisitions/base.py` & `boax-0.1.1/boax/optimization/acquisitions/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/acquisitions/functions/__init__.py` & `boax-0.1.1/boax/optimization/acquisitions/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/acquisitions/functions/analytic.py` & `boax-0.1.1/boax/optimization/acquisitions/functions/analytic.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/acquisitions/functions/monte_carlo.py` & `boax-0.1.1/boax/optimization/acquisitions/functions/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/constraints/__init__.py` & `boax-0.1.1/boax/optimization/acquisitions/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/constraints/alias.py` & `boax-0.1.1/boax/optimization/acquisitions/constraints/alias.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from functools import partial
 
 from jax import jit
 from jax import numpy as jnp
 
 from boax.core import distributions
 from boax.core.distributions.normal import Normal
-from boax.optimization.constraints.base import Constraint
+from boax.optimization.acquisitions.constraints.base import Constraint
 from boax.utils.functools import compose
 from boax.utils.typing import Numeric
 
 
 def less_or_equal(
   bound: Numeric,
 ) -> Constraint[Normal]:
```

### Comparing `boax-0.1.0/boax/optimization/constraints/base.py` & `boax-0.1.1/boax/optimization/acquisitions/constraints/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/construction.py` & `boax-0.1.1/boax/optimization/acquisitions/transformed.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,85 +8,60 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Construct optimizations."""
+"""Transformation functions for acquisitions."""
+
 
 from functools import partial
-from typing import Callable, TypeVar
+from typing import Sequence, TypeVar
 
-from jax import lax, vmap
+from jax import lax
 
 from boax.optimization.acquisitions.base import Acquisition
-from boax.optimization.constraints.base import Constraint
-from boax.prediction.models.base import Model
+from boax.optimization.acquisitions.constraints.base import Constraint
 from boax.utils.functools import compose, sequence, unwrap
-from boax.utils.typing import Array
 
 T = TypeVar('T')
 
 
-def construct(
-  model: Model[T],
-  acquisition: Acquisition[T],
-) -> Callable[[Array], Array]:
-  """
-  Constructs an acquisition function.
-
-  Args:
-    model: The base model.
-    acquisition: The acquisition.
-    projection_fn: The projection function.
-
-  Returns:
-    The constructed acquisition function.
-  """
-
-  return compose(
-    acquisition,
-    vmap(model),
-  )
-
-
-def construct_constrained(
-  model: Model[T], acquisition: Acquisition[T], *constraints: Constraint[T]
-) -> Acquisition[T]:
+def constrained(
+  acquisition: Acquisition[T], *constraints: Constraint[T]
+) -> Acquisition[Sequence[T]]:
   """
   Constructs a constrained acquisition function.
 
   Args:
     acquisition: The acquisition.
     constraints: The constraints.
 
   Returns:
     The constructed acquisition function.
   """
 
   return compose(
     unwrap(partial(partial, sequence)(lax.mul, 1.0)),
     partial(partial, zip)((acquisition, *constraints)),
-    vmap(model),
   )
 
 
-def construct_log_constrained(
-  model: Model[T], acquisition: Acquisition[T], *log_constraints: Constraint[T]
-) -> Callable[[Array], Array]:
+def log_constrained(
+  acquisition: Acquisition[T], *log_constraints: Constraint[T]
+) -> Acquisition[Sequence[T]]:
   """
   Constructs a log constrained acquisition function.
 
   Args:
     acquisition: The log acquisition.
     constraints: The log constraints.
 
   Returns:
     The constructed log acquisition function.
   """
 
   return compose(
     unwrap(partial(partial, sequence)(lax.add, 0.0)),
     partial(partial, zip)((acquisition, *log_constraints)),
-    vmap(model),
   )
```

### Comparing `boax-0.1.0/boax/optimization/optimizers/__init__.py` & `boax-0.1.1/boax/optimization/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/optimizers/alias.py` & `boax-0.1.1/boax/optimization/optimizers/alias.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,44 +19,44 @@
 
 from boax.optimization.optimizers import functions
 from boax.optimization.optimizers.base import Optimizer
 from boax.utils.typing import Array
 
 
 def bfgs(
-  acquisition_fn: Callable[[Array], Array],
+  fn: Callable[[Array], Array],
   bounds: Array,
   x0: Array,
   num_samples: int,
 ) -> Optimizer:
   """
   The BFGS acquisition function optimizer.
 
   Example:
-    >>> optimizer = bfgs(acqf, bounds, x0, num_samples)
+    >>> optimizer = bfgs(fn, bounds, x0, num_samples)
     >>> candidates = optimizer.init(key)
     >>> next_candidates, values = optimizer(candidates)
 
   Args:
-    acquisition_fn: The acquisition function.
+    fn: The function to be optimized.
     bounds: The bounds of the search space.
     x0: The index points to consider.
     num_samples: The number of sampled candidates.
 
   Returns:
     The corresponding `Optimizer`.
   """
 
   return Optimizer(
     partial(
       functions.initialization.q_batch,
-      acquisition_fn=acquisition_fn,
+      fn=fn,
       x0=x0,
       num_samples=num_samples,
     ),
     partial(
       functions.scipy.maximize,
-      acquisition_fn=acquisition_fn,
+      fn=fn,
       bounds=bounds,
       method='bfgs',
     ),
   )
```

### Comparing `boax-0.1.0/boax/optimization/optimizers/base.py` & `boax-0.1.1/boax/optimization/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/optimizers/functions/__init__.py` & `boax-0.1.1/boax/optimization/optimizers/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/optimization/optimizers/functions/initialization.py` & `boax-0.1.1/boax/optimization/optimizers/functions/initialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 from jax import numpy as jnp
 
 from boax.utils.typing import Array, Numeric, PRNGKey
 
 
 def q_batch(
   key: PRNGKey,
-  acquisition_fn: Callable[[Array], Array],
+  fn: Callable[[Array], Array],
   x0: Array,
   num_samples: int,
   eta: Numeric = 1.0,
 ) -> Array:
   return random.choice(
     key,
     x0,
     (num_samples,),
-    p=jnp.exp(eta * nn.standardize(acquisition_fn(x0), axis=0)),
+    p=jnp.exp(eta * nn.standardize(fn(x0), axis=0)),
   )
```

### Comparing `boax-0.1.0/boax/optimization/optimizers/functions/scipy.py` & `boax-0.1.1/boax/optimization/optimizers/functions/scipy.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 
 from boax.utils.functools import compose
 from boax.utils.typing import Array
 
 
 def maximize(
   candidates: Array,
-  acquisition_fn: Callable[[Array], Array],
+  fn: Callable[[Array], Array],
   bounds: Array,
   method: str,
 ) -> Tuple[Array, Array]:
   results = optimize.minimize(
     fun=compose(
       jnp.negative,
       jnp.sum,
-      acquisition_fn,
+      fn,
       partial(jnp.reshape, newshape=candidates.shape),
     ),
     x0=candidates.flatten(),
     method=method,
   )
 
   clipped = jnp.clip(
     jnp.reshape(results.x, candidates.shape),
     a_min=bounds[:, 0],
     a_max=bounds[:, 1],
   )
 
-  return clipped, acquisition_fn(clipped)
+  return clipped, fn(clipped)
```

### Comparing `boax-0.1.0/boax/prediction/__init__.py` & `boax-0.1.1/boax/prediction/models/likelihoods/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The prediction module."""
+"""The kernels sub-package."""
 
-from . import kernels as kernels
-from . import likelihoods as likelihoods
-from . import means as means
-from . import models as models
-from . import objectives as objectives
-from .construction import construct as construct
+from .alias import beta as beta
+from .alias import gaussian as gaussian
+from .base import Likelihood as Likelihood
```

### Comparing `boax-0.1.0/boax/prediction/kernels/__init__.py` & `boax-0.1.1/boax/prediction/models/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/kernels/alias.py` & `boax-0.1.1/boax/prediction/models/kernels/alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Alias for kernels."""
 
 from functools import partial
 
-from boax.prediction.kernels import functions
-from boax.prediction.kernels.base import Kernel
+from boax.prediction.models.kernels import functions
+from boax.prediction.models.kernels.base import Kernel
 from boax.utils.typing import Array, Numeric
 
 
 def rbf(length_scale: Array) -> Kernel:
   """
   The Radial basis function (RBF) kernel.
```

### Comparing `boax-0.1.0/boax/prediction/kernels/base.py` & `boax-0.1.1/boax/prediction/models/kernels/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/kernels/functions/__init__.py` & `boax-0.1.1/boax/prediction/models/kernels/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/kernels/functions/distance.py` & `boax-0.1.1/boax/prediction/models/kernels/functions/distance.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from jax import lax
 from jax import numpy as jnp
 
 from boax.utils.typing import Array
 
 
-def squared_distance(x: Array, y: Array) -> Array:
+def squared(x: Array, y: Array) -> Array:
   """
   Computes the squared distance between vectors `x` and `y`.
 
   Args:
     x: A vector.
     y: A vector.
 
@@ -35,15 +35,15 @@
   x_norm = jnp.sum(jnp.power(x, 2))
   y_norm = jnp.sum(jnp.power(y, 2))
   inner = jnp.inner(x, y)
 
   return lax.max(x_norm + y_norm - 2 * inner, 0.0)
 
 
-def euclidean_distance(x: Array, y: Array) -> Array:
+def euclidean(x: Array, y: Array) -> Array:
   """
   Computes the euclidean distance between vectors `x` and `y`.
 
   Args:
     x: A vector.
     y: A vector.
```

### Comparing `boax-0.1.0/boax/prediction/kernels/functions/matern.py` & `boax-0.1.1/boax/prediction/models/kernels/functions/matern.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 """Matern kernels."""
 
 import math
 
 from jax import numpy as jnp
 
-from boax.prediction.kernels.functions.distance import euclidean_distance
+from boax.prediction.models.kernels.functions import distance
 from boax.utils.typing import Numeric
 
 sqrt_3 = math.sqrt(3)
 sqrt_5 = math.sqrt(5)
 
 
 def one_half(x: Numeric, y: Numeric, length_scale: Numeric) -> Numeric:
-  return jnp.exp(-euclidean_distance(x / length_scale, y / length_scale))
+  return jnp.exp(-distance.euclidean(x / length_scale, y / length_scale))
 
 
 def three_halves(x: Numeric, y: Numeric, length_scale: Numeric) -> Numeric:
-  K = sqrt_3 * euclidean_distance(x / length_scale, y / length_scale)
+  K = sqrt_3 * distance.euclidean(x / length_scale, y / length_scale)
   K = (1.0 + K) * jnp.exp(-K)
   return K
 
 
 def five_halves(x: Numeric, y: Numeric, length_scale: Numeric) -> Numeric:
-  K = sqrt_5 * euclidean_distance(x / length_scale, y / length_scale)
+  K = sqrt_5 * distance.euclidean(x / length_scale, y / length_scale)
   K = (1.0 + K + K**2 / 3.0) * jnp.exp(-K)
   return K
```

### Comparing `boax-0.1.0/boax/prediction/kernels/functions/periodic.py` & `boax-0.1.1/boax/prediction/models/kernels/functions/periodic.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/kernels/functions/rbf.py` & `boax-0.1.1/boax/prediction/models/kernels/functions/rbf.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Radial Basis Function (RBF) kernels."""
 
 from jax import numpy as jnp
 
-from boax.prediction.kernels.functions.distance import squared_distance
+from boax.prediction.models.kernels.functions import distance
 from boax.utils.typing import Numeric
 
 
 def rbf(x: Numeric, y: Numeric, length_scale: Numeric) -> Numeric:
-  return jnp.exp(-0.5 * squared_distance(x / length_scale, y / length_scale))
+  return jnp.exp(-0.5 * distance.squared(x / length_scale, y / length_scale))
```

### Comparing `boax-0.1.0/boax/prediction/kernels/functions/utils.py` & `boax-0.1.1/boax/prediction/models/kernels/functions/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """Utils for kernels."""
 
 from typing import Callable
 
 from jax import jit, vmap
 
-from boax.prediction.kernels.base import Kernel
+from boax.prediction.models.kernels.base import Kernel
 from boax.utils.typing import Numeric
 
 
 def from_kernel_function(
   kernel_fn: Callable[[Numeric, Numeric], Numeric],
 ) -> Kernel:
   """
```

### Comparing `boax-0.1.0/boax/prediction/kernels/transformed.py` & `boax-0.1.1/boax/prediction/models/kernels/transformed.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Transformation functions for kernels."""
 
 from functools import partial
+from typing import Callable
 
 from jax import lax
 from jax import numpy as jnp
 
-from boax.prediction.kernels.base import Kernel
+from boax.prediction.models.kernels.base import Kernel
 from boax.utils.functools import combine, compose
 from boax.utils.typing import Array, Numeric
 
 
 def scaled(kernel: Kernel, amplitude: Numeric) -> Kernel:
   """
   Scales a given kernel.
@@ -42,57 +43,14 @@
   Returns:
     A scaled `Kernel`.
   """
 
   return compose(partial(lax.mul, y=amplitude), kernel)
 
 
-def linear_truncated(
-  x_fidelities: Array,
-  y_fidelities: Array,
-  unbiased: Kernel,
-  biased: Kernel,
-  power: Numeric,
-) -> Kernel:
-  """
-  Constructs a linear truncated kernel for one fidelity parameter.
-
-  Computes `k(x, y) = k_0(x, y) + c(x_fid, y_fid) k_1(x, y)`,
-
-  where `k_i(x, y)` are Matern kernels calculated between `x` and `y`, and
-  `c(x_fid, y_fid) = (1 - x_fid)(1 - y_fid))(1 + x_fid y_fid)^p`.
-
-  Example:
-    >>> unbiased = matern_five_halves(jnp.array([0.2, 3.0]))
-    >>> biased = matern_five_halves(jnp.array([1.5]))
-    >>> kernel = linear_truncated(x_fid, y_fid, unbiased, biased, 1.0)
-    >>> Kxx = kernel(xs, xs)
-
-  Args:
-    x_fidelities: The fidelity parameters of `x`.
-    y_fidelities: The fidelity parameters of `y`.
-    unbiased: The unbiased kernel `k_0`.
-    biased: The biased kernel `k_1`.
-    power: The order of the polynomial kernel `p`.
-
-  Returns:
-    A linear truncated `Kernel`.
-  """
-
-  bias_factor = (
-    (1 - x_fidelities)
-    * (1 - y_fidelities.T)
-    * jnp.power(1 + x_fidelities * y_fidelities.T, power)
-  )
-
-  return combine(
-    lax.add, 0.0, unbiased, compose(partial(lax.mul, y=bias_factor), biased)
-  )
-
-
 def additive(*kernels: Kernel) -> Kernel:
   """
   Constructs an additive kernel which sums over a sequence of kernels.
 
   Computes `k(x, y) = k1(x, y) + k2(x, y) + ... + kn(x, y)`.
 
   Example:
@@ -123,7 +81,49 @@
     kernels: The sequence of inner kernels.
 
   Returns:
     A product `Kernel`.
   """
 
   return combine(lax.mul, 1.0, *kernels)
+
+
+def linear_truncated(
+  unbiased: Kernel,
+  biased: Kernel,
+  power: Numeric,
+) -> Callable[[Array, Array], Kernel]:
+  """
+  Constructs a linear truncated kernel for one fidelity parameter.
+
+  Computes `k(x, y) = k_0(x, y) + c(x_fid, y_fid) k_1(x, y)`,
+
+  where `k_i(x, y)` are Matern kernels calculated between `x` and `y`, and
+  `c(x_fid, y_fid) = (1 - x_fid)(1 - y_fid))(1 + x_fid y_fid)^p`.
+
+  Example:
+    >>> unbiased = matern_five_halves(jnp.array([0.2, 3.0]))
+    >>> biased = matern_five_halves(jnp.array([1.5]))
+    >>> kernel = linear_truncated(unbiased, biased, 1.0)
+    >>> Kxx = kernel(x_fid, x_fid)(xs, xs)
+
+  Args:
+    unbiased: The unbiased kernel `k_0`.
+    biased: The biased kernel `k_1`.
+    power: The order of the polynomial kernel `p`.
+
+  Returns:
+    A callable that given fidelities returns a linear truncated `Kernel`.
+  """
+
+  def fidelities(x_fidelities: Array, y_fidelities: Array) -> Kernel:
+    bias_factor = (
+      (1 - x_fidelities)
+      * (1 - y_fidelities.T)
+      * jnp.power(1 + x_fidelities * y_fidelities.T, power)
+    )
+
+    return combine(
+      lax.add, 0.0, unbiased, compose(partial(lax.mul, y=bias_factor), biased)
+    )
+
+  return fidelities
```

### Comparing `boax-0.1.0/boax/prediction/likelihoods/__init__.py` & `boax-0.1.1/boax/prediction/objectives/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The kernels sub-package."""
+"""The objectives sub-package."""
 
-from .alias import gaussian as gaussian
-from .base import Likelihood as Likelihood
+from .alias import negative_log_likelihood as negative_log_likelihood
+from .base import Objective as Objective
+from .transformed import penalized as penalized
```

### Comparing `boax-0.1.0/boax/prediction/likelihoods/alias.py` & `boax-0.1.1/boax/prediction/models/likelihoods/alias.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 from functools import partial
 
 from jax import jit
 
 from boax.core.distributions.beta import Beta
 from boax.core.distributions.multivariate_normal import MultivariateNormal
-from boax.prediction.likelihoods import functions
-from boax.prediction.likelihoods.base import Likelihood
+from boax.prediction.models.likelihoods import functions
+from boax.prediction.models.likelihoods.base import Likelihood
 from boax.utils.typing import Array, Numeric
 
 
 def gaussian(
   noise: Numeric,
 ) -> Likelihood[MultivariateNormal, MultivariateNormal]:
   """
```

### Comparing `boax-0.1.0/boax/prediction/likelihoods/base.py` & `boax-0.1.1/boax/prediction/models/likelihoods/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/likelihoods/functions/__init__.py` & `boax-0.1.1/boax/prediction/models/likelihoods/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/likelihoods/functions/conditional.py` & `boax-0.1.1/boax/prediction/models/likelihoods/functions/conditional.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/likelihoods/functions/marginal.py` & `boax-0.1.1/boax/prediction/models/likelihoods/functions/marginal.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/means/__init__.py` & `boax-0.1.1/boax/prediction/models/means/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/means/alias.py` & `boax-0.1.1/boax/prediction/models/means/alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Alias for mean functions."""
 
 from jax import jit, vmap
 from jax import numpy as jnp
 
-from boax.prediction.means.base import Mean
+from boax.prediction.models.means.base import Mean
 from boax.utils.functools import const
 from boax.utils.typing import Array, Numeric
 
 
 def zero() -> Mean:
   """
   The zero mean function.
```

### Comparing `boax-0.1.0/boax/prediction/means/base.py` & `boax-0.1.1/boax/prediction/models/means/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/models/__init__.py` & `boax-0.1.1/boax/prediction/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """The models sub-package."""
 
+from . import kernels as kernels
+from . import likelihoods as likelihoods
+from . import means as means
 from .alias import gaussian_process as gaussian_process
-from .alias import gaussian_process_regression as gaussian_process_regression
-from .alias import multi_fidelity_regression as multi_fidelity_regression
+from .alias import multi_fidelity as multi_fidelity
 from .base import Model as Model
 from .transformed import input_transformed as input_transformed
 from .transformed import joined as joined
 from .transformed import outcome_transformed as outcome_transformed
 from .transformed import sampled as sampled
+from .transformed import scaled as scaled
```

### Comparing `boax-0.1.0/boax/prediction/models/alias.py` & `boax-0.1.1/boax/prediction/models/alias.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,129 +11,131 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Alias for surrogate models."""
 
 from functools import partial
-from typing import Callable
+from typing import Callable, TypeVar
 
 from jax import jit
 
 from boax.core.distributions.multivariate_normal import MultivariateNormal
-from boax.prediction.kernels.base import Kernel
-from boax.prediction.means.base import Mean
 from boax.prediction.models import functions
 from boax.prediction.models.base import Model
+from boax.prediction.models.kernels.base import Kernel
+from boax.prediction.models.likelihoods.base import Likelihood
+from boax.prediction.models.means.base import Mean
+from boax.utils.functools import compose
 from boax.utils.typing import Array, Numeric
 
+T = TypeVar('T')
+
 
 def gaussian_process(
   mean_fn: Mean,
   kernel_fn: Kernel,
+  likelihood_fn: Likelihood[MultivariateNormal, T],
+  observation_index_points: Array | None = None,
+  observations: Array | None = None,
   jitter: Numeric = 1e-6,
-) -> Model[MultivariateNormal]:
+) -> Model[T]:
   """
   The gaussian process model.
 
   Example:
     >>> model = gaussian_process(mean_fn, kernel_fn)
     >>> mean, cov = model(xs)
 
   Args:
     mean_fn: The process' mean function.
     kernel_fn: The process' covariance function.
+    observation_index_points: The index points of the given observations.
+    observations: The observed values.
     jitter: The scalar added to the diagonal of the covariance matrix to ensure positive definiteness.
 
   Returns:
     The gaussian process `Model`.
   """
 
-  return jit(
-    partial(
-      functions.gaussian.prior,
-      mean_fn=mean_fn,
-      kernel_fn=kernel_fn,
-      jitter=jitter,
+  if observation_index_points is None or observations is None:
+    return jit(
+      compose(
+        likelihood_fn,
+        partial(
+          functions.gaussian.prior,
+          mean_fn=mean_fn,
+          kernel_fn=kernel_fn,
+          jitter=jitter,
+        ),
+      )
     )
-  )
-
-
-def gaussian_process_regression(
-  mean_fn: Mean,
-  kernel_fn: Kernel,
-  jitter: Numeric = 1e-6,
-) -> Callable[[Array, Array], Model[MultivariateNormal]]:
-  """
-  The gaussian process regression model.
-
-  Example:
-    >>> model = gaussian_process_regression(mean_fn, kernel_fn, 1e-4)
-    >>> mean, cov = model(x_train, y_train)(xs)
-
-  Args:
-    mean_fn: The process' mean function.
-    kernel_fn: The process' covariance function.
-    jitter: The scalar added to the diagonal of the covariance matrix to ensure positive definiteness.
 
-  Returns:
-    The gaussian process regression `Model`.
-  """
-
-  def regression(observation_index_points, observations):
+  else:
     return jit(
-      partial(
-        functions.gaussian.posterior,
-        observation_index_points=observation_index_points,
-        observations=observations,
-        mean_fn=mean_fn,
-        kernel_fn=kernel_fn,
-        jitter=jitter,
+      compose(
+        likelihood_fn,
+        partial(
+          functions.gaussian.posterior,
+          observation_index_points=observation_index_points,
+          observations=observations,
+          mean_fn=mean_fn,
+          kernel_fn=kernel_fn,
+          jitter=jitter,
+        ),
       )
     )
 
-  return regression
-
 
-def multi_fidelity_regression(
+def multi_fidelity(
   mean_fn: Mean,
   kernel_fn: Callable[[Array, Array], Kernel],
+  likelihood_fn: Likelihood[MultivariateNormal, T],
+  observation_index_points: Array | None = None,
+  observations: Array | None = None,
   jitter: Numeric = 1e-6,
-) -> Model[MultivariateNormal]:
+) -> Model[T]:
   """
-  The multi fidelity gaussian process regression model.
+  The multi fidelity gaussian process model.
 
   Example:
-    >>> model = multi_fidelity_regression(mean_fn, kernel_fn, 1e-4)
+    >>> model = multi_fidelity(mean_fn, kernel_fn, 1e-4)
     >>> mean, cov = model(x_train, y_train)(xs)
 
   Args:
     mean_fn: The process' mean function.
     kernel_fn: The process' covariance function.
+    observation_index_points: The index points of the given observations.
+    observations: The observed values.
     jitter: The scalar added to the diagonal of the covariance matrix to ensure positive definiteness.
 
   Returns:
-    The multi fidelity gaussian process regression `Model`.
+    The multi fidelity gaussian process `Model`.
   """
 
-  def regression(observation_index_points, observations):
-    observation_values, observation_fidelities = functions.multi_fidelity.split(
-      observation_index_points
+  if observation_index_points is None or observations is None:
+    return jit(
+      compose(
+        likelihood_fn,
+        partial(
+          functions.multi_fidelity.prior,
+          mean_fn=mean_fn,
+          kernel_fn=kernel_fn,
+          jitter=jitter,
+        ),
+      )
     )
 
-    def model(index_points):
-      values, fidelities = functions.multi_fidelity.split(index_points)
-
-      return functions.multi_fidelity.posterior(
-        index_points=values,
-        index_points_fidelities=fidelities,
-        observation_index_points=observation_values,
-        observation_index_points_fidelities=observation_fidelities,
-        observations=observations,
-        mean_fn=mean_fn,
-        kernel_fn=kernel_fn,
-        jitter=jitter,
+  else:
+    return jit(
+      compose(
+        likelihood_fn,
+        partial(
+          functions.multi_fidelity.posterior,
+          observation_index_points=observation_index_points,
+          observations=observations,
+          mean_fn=mean_fn,
+          kernel_fn=kernel_fn,
+          jitter=jitter,
+        ),
       )
-
-    return jit(model)
-
-  return regression
+    )
```

### Comparing `boax-0.1.0/boax/prediction/models/base.py` & `boax-0.1.1/boax/prediction/models/base.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/models/functions/__init__.py` & `boax-0.1.1/boax/prediction/models/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/prediction/models/functions/gaussian.py` & `boax-0.1.1/boax/prediction/models/functions/gaussian.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 """Gaussian Process functions."""
 
 from jax import numpy as jnp
 from jax import scipy
 
 from boax.core import distributions
 from boax.core.distributions.multivariate_normal import MultivariateNormal
-from boax.prediction.kernels.base import Kernel
-from boax.prediction.means.base import Mean
+from boax.prediction.models.kernels.base import Kernel
+from boax.prediction.models.means.base import Mean
 from boax.utils.typing import Array, Numeric
 
 
 def prior(
   index_points: Array,
   mean_fn: Mean,
   kernel_fn: Kernel,
```

### Comparing `boax-0.1.0/boax/prediction/models/transformed.py` & `boax-0.1.1/boax/prediction/models/transformed.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,33 +11,51 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Transformation functions for models."""
 
 from functools import partial
-from typing import Callable, TypeVar
+from typing import Callable, Sequence, TypeVar
 
 from jax import vmap
 
 from boax.prediction.models.base import Model
 from boax.utils.functools import apply, call, compose
 from boax.utils.typing import Array
 
-T = TypeVar('T')
 A = TypeVar('A')
 B = TypeVar('B')
+T = TypeVar('T')
+
+
+def joined(*models: Model[T]) -> Model[Sequence[T]]:
+  """
+  Constructs a joined model.
+
+  Example:
+    >>> transformed = joined(objective_model, cost_model)
+    >>> objective_result, cost_result = transformed(xs)
+
+  Args:
+    models: The models to be joined.
+
+  Returns:
+    The transformed `Model` function.
+  """
+
+  return apply(tuple, *models)
 
 
 def outcome_transformed(
   model: Model[A],
   *transformation_fns: Callable[[A], B],
 ) -> Model[B]:
   """
-  Constructs a outcome transformed model.
+  Constructs an outcome transformed model.
 
   Example:
     >>> transformed = outcome_transformed(model, fn1, fn2, fn3)
     >>> result = transformed(xs)
 
   Args:
     model: The base model.
@@ -54,15 +72,15 @@
 
 
 def input_transformed(
   model: Model[A],
   *transformation_fns: Callable[[A], B],
 ) -> Model[B]:
   """
-  Constructs a input transformed model.
+  Constructs an input transformed model.
 
   Example:
     >>> transformed = input_transformed(model, fn1, fn2, fn3)
     >>> result = transformed(xs)
 
   Args:
     model: The base model.
@@ -74,52 +92,63 @@
 
   return compose(
     model,
     *reversed(transformation_fns),
   )
 
 
-def sampled(
+def scaled(
   model: Model[T],
-  sample_fn: Callable[[T, Array], Array],
-  base_samples: Array,
-) -> Model[Array]:
+  scale_fn: Callable[[T, Array, Array], T],
+  loc: Array,
+  scale: Array,
+) -> Model[T]:
   """
-  Constructs a MC-based model.
+  Constructs a scaled model.
 
   Example:
-    >>> transformed = sampled(model, sample_fn, base_samples)
+    >>> transformed = scaled(model, scale_fn, loc, scale)
     >>> result = transformed(xs)
 
   Args:
     model: The base model.
-    sample_fn: The sampling function.
-    base_samples: The base samples of the sampling process.
+    scale_fn: The sampling function.
+    loc: The location parameter.
+    scale: The scale parameter.
 
   Returns:
     The transformed `Model` function.
   """
 
   return compose(
-    call(base_samples),
-    vmap,
-    partial(partial, sample_fn),
+    partial(scale_fn, loc=loc, scale=scale),
     model,
   )
 
 
-def joined(*models: Model[T]) -> Model[T]:
+def sampled(
+  model: Model[T],
+  sample_fn: Callable[[T, Array], Array],
+  base_samples: Array,
+) -> Model[Array]:
   """
-  Constructs a joined model.
+  Constructs a MC-based model.
 
   Example:
-    >>> transformed = joined(objective_model, cost_model)
-    >>> objective_result, cost_result = transformed(xs)
+    >>> transformed = sampled(model, sample_fn, base_samples)
+    >>> result = transformed(xs)
 
   Args:
-    models: The models to be joined.
+    model: The base model.
+    sample_fn: The sampling function.
+    base_samples: The base samples of the sampling process.
 
   Returns:
     The transformed `Model` function.
   """
 
-  return apply(tuple, *models)
+  return compose(
+    call(base_samples),
+    vmap,
+    partial(partial, sample_fn),
+    model,
+  )
```

### Comparing `boax-0.1.0/boax/prediction/objectives/__init__.py` & `boax-0.1.1/boax/prediction/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The objectives sub-package."""
+"""The prediction module."""
 
-from .alias import negative_log_likelihood as negative_log_likelihood
-from .base import Objective as Objective
-from .transformed import penalized as penalized
+from . import models as models
+from . import objectives as objectives
```

### Comparing `boax-0.1.0/boax/prediction/objectives/alias.py` & `boax-0.1.1/boax/prediction/objectives/alias.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 def negative_log_likelihood(
   logpdf_fn: Callable[[T, Array], Array],
 ) -> Objective[T]:
   """
   The negative log likelihood objective function.
 
   Example:
-    >>> nll = gaussian(1e-4)
-    >>> objective = likelihood(mvn)
+    >>> objective = negative_log_likelihood(logpdf_fn)
+    >>> nll = objective(prediction, targets)
 
   Args:
-    noise: The noise parameter.
+    logpdf_fn: The log probability mass function.
 
   Returns:
-    The gaussian `Likelihood` function.
+    The negative log likelihood `Objective` function.
   """
 
   def objective(prediction, targets):
     return -logpdf_fn(prediction, targets)
 
   return jit(objective)
```

### Comparing `boax-0.1.0/boax/prediction/objectives/base.py` & `boax-0.1.1/boax/prediction/objectives/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
 T = TypeVar('T')
 
 
 class Objective(Protocol, Generic[T]):
   """
   A callable type for objectives.
+
+  An objective function takes a posterior prediction of type `T`
+  and an array of targets as input and returns an objective value.
   """
 
   def __call__(self, prediction: T, targets: Array) -> Array:
     """
     Computes the objective value at the given prediction of type `T`.
 
     Args:
```

### Comparing `boax-0.1.0/boax/prediction/objectives/transformed.py` & `boax-0.1.1/boax/prediction/objectives/transformed.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax/utils/__init__.py` & `boax-0.1.1/boax/version.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The optimization module."""
 
-from . import functools as functools
-from . import typing as typing
+"""Current boax version at head on GitHub"""
+
+__version__ = '0.1.1'
```

### Comparing `boax-0.1.0/boax/utils/functools.py` & `boax-0.1.1/boax/utils/functools.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
 
 def call(*args, **kwargs) -> Callable[[Callable[[Any], T]], T]:
   """
   Calls a callable with the given inputs.
 
   Args:
-    *args: The arguments.
-    **kwargs: The keyword arguments.
+    args: The arguments.
+    kwargs: The keyword arguments.
 
   Returns:
     A function that calls given function with the inputs.
   """
 
   def __fn(fn: Callable[[Any], T]) -> T:
     return fn(*args, **kwargs)
```

### Comparing `boax-0.1.0/boax/utils/typing.py` & `boax-0.1.1/boax/utils/typing.py`

 * *Files identical despite different names*

### Comparing `boax-0.1.0/boax.egg-info/PKG-INFO` & `boax-0.1.1/boax.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boax
-Version: 0.1.0
+Version: 0.1.1
 Summary: Boax is a Bayesian Optimization library for JAX.
 Project-URL: homepage, https://github.com/Lando-L/boax
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
@@ -72,70 +72,70 @@
 
 ```sh
 pip install git+https://github.com/Lando-L/boax.git
 ```
 
 ## Basic Usage
 
-Here is a basic example of using the Boax API for Bayesian Optimization. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
+Here is a basic example of using the Boax API for defining a Gaussian Process model, constructing an Acquisition function, and combining the two for optimzation. For more details check out the [docs](https://boax.readthedocs.io/en/latest/).
 
-1. Creation of a prediction model.
+1. Defining a Gaussian Process model:
 
 ```python
-def model(params):
-  return models.outcome_transformed(
-    models.gaussian_process_regression(
-      means.zero(),
-      kernels.rbf(params['length_scale']),
-    )(
-      x_train,
-      y_train,
-    ),
-    likelihoods.gaussian(params['noise']),
-  )
+from boax.prediction import models
+
+model = models.gaussian_process(
+  models.means.zero(),
+  models.kernels.scaled(
+    models.kernels.rbf(1.0),
+    0.5
+  ),
+  models.likelihoods.gaussian(1e-4),
+  x_train,
+  y_train,
+)
 ```
 
-2. Construction of an acquisition function.
+2. Constructing an Acquisition function.
 
 ```python
-def construct(model):
-  return optimization.construct(
-    models.outcome_transformed(
-      model,
-      distributions.multivariate_normal.as_normal,
-    ),
-    acquisitions.upper_confidence_bound(
-      beta=2.0
-    ),
-  )
+from boax.optimization import acquisitions
+
+acquisition = acquisitions.upper_confidence_bound(
+  beta=2.0
+)
 ```
 
-3. Selection of the next candidate to query.
+3. Combining the two for optimization
 
 ```python
-def select(key, acqf):
-    bfgs = optimizers.bfgs(acqf, bounds, x0, 10)
-    candidates = bfgs.init(key)
-    next_candidates, values = bfgs.update(candidates)
-
-    next_x = next_candidates[jnp.argmax(values)]
-    next_y = objective(next_x)
-
-    return next_x, next_y
+from jax import jit, random, vmap
+from jax import numpy as jnp
+from boax.optimization import optimizers
+
+def acqf(x):
+  return acquisition(vmap(model)(x))
+
+key1, key2 = random.split(random.key(0))
+bounds = jnp.array([[-1.0, 1.0]])
+x0 = random.uniform(key1, shape=(100, 1, 1))
+bfgs = optimizers.bfgs(jit(acqf), bounds, x0, 10)
+candidates = bfgs.init(key2)
+next_candidates, values = bfgs.update(candidates)
 ```
 
 ## Citing Boax
 
 To cite Boax please use the citation:
 
 ```bibtex
 @software{boax2023github,
   author = {Lando L{\"o}per},
   title = {{B}oax: A Bayesian Optimization library for {JAX}},
   url = {https://github.com/Lando-L/boax},
-  version = {0.1.0},
+  version = {0.1.1},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, the version number
 is intended to be that from [boax/version.py](https://github.com/Lando-L/boax/blob/main/boax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `boax-0.1.0/boax.egg-info/SOURCES.txt` & `boax-0.1.1/boax.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,66 +11,66 @@
 boax/core/__init__.py
 boax/core/distributions/__init__.py
 boax/core/distributions/beta.py
 boax/core/distributions/gamma.py
 boax/core/distributions/multivariate_normal.py
 boax/core/distributions/normal.py
 boax/core/distributions/poisson.py
+boax/core/distributions/transformed.py
 boax/core/distributions/uniform.py
 boax/core/samplers/__init__.py
 boax/core/samplers/alias.py
 boax/core/samplers/base.py
 boax/core/samplers/functions/__init__.py
 boax/core/samplers/functions/quasi_random.py
 boax/core/samplers/functions/utils.py
 boax/optimization/__init__.py
-boax/optimization/construction.py
 boax/optimization/acquisitions/__init__.py
 boax/optimization/acquisitions/alias.py
 boax/optimization/acquisitions/base.py
+boax/optimization/acquisitions/transformed.py
+boax/optimization/acquisitions/constraints/__init__.py
+boax/optimization/acquisitions/constraints/alias.py
+boax/optimization/acquisitions/constraints/base.py
 boax/optimization/acquisitions/functions/__init__.py
 boax/optimization/acquisitions/functions/analytic.py
 boax/optimization/acquisitions/functions/monte_carlo.py
-boax/optimization/constraints/__init__.py
-boax/optimization/constraints/alias.py
-boax/optimization/constraints/base.py
 boax/optimization/optimizers/__init__.py
 boax/optimization/optimizers/alias.py
 boax/optimization/optimizers/base.py
 boax/optimization/optimizers/functions/__init__.py
 boax/optimization/optimizers/functions/initialization.py
 boax/optimization/optimizers/functions/scipy.py
 boax/prediction/__init__.py
-boax/prediction/construction.py
-boax/prediction/kernels/__init__.py
-boax/prediction/kernels/alias.py
-boax/prediction/kernels/base.py
-boax/prediction/kernels/transformed.py
-boax/prediction/kernels/functions/__init__.py
-boax/prediction/kernels/functions/distance.py
-boax/prediction/kernels/functions/matern.py
-boax/prediction/kernels/functions/periodic.py
-boax/prediction/kernels/functions/rbf.py
-boax/prediction/kernels/functions/utils.py
-boax/prediction/likelihoods/__init__.py
-boax/prediction/likelihoods/alias.py
-boax/prediction/likelihoods/base.py
-boax/prediction/likelihoods/functions/__init__.py
-boax/prediction/likelihoods/functions/conditional.py
-boax/prediction/likelihoods/functions/marginal.py
-boax/prediction/means/__init__.py
-boax/prediction/means/alias.py
-boax/prediction/means/base.py
 boax/prediction/models/__init__.py
 boax/prediction/models/alias.py
 boax/prediction/models/base.py
 boax/prediction/models/transformed.py
 boax/prediction/models/functions/__init__.py
 boax/prediction/models/functions/gaussian.py
 boax/prediction/models/functions/multi_fidelity.py
+boax/prediction/models/kernels/__init__.py
+boax/prediction/models/kernels/alias.py
+boax/prediction/models/kernels/base.py
+boax/prediction/models/kernels/transformed.py
+boax/prediction/models/kernels/functions/__init__.py
+boax/prediction/models/kernels/functions/distance.py
+boax/prediction/models/kernels/functions/matern.py
+boax/prediction/models/kernels/functions/periodic.py
+boax/prediction/models/kernels/functions/rbf.py
+boax/prediction/models/kernels/functions/utils.py
+boax/prediction/models/likelihoods/__init__.py
+boax/prediction/models/likelihoods/alias.py
+boax/prediction/models/likelihoods/base.py
+boax/prediction/models/likelihoods/functions/__init__.py
+boax/prediction/models/likelihoods/functions/conditional.py
+boax/prediction/models/likelihoods/functions/marginal.py
+boax/prediction/models/means/__init__.py
+boax/prediction/models/means/alias.py
+boax/prediction/models/means/base.py
 boax/prediction/objectives/__init__.py
 boax/prediction/objectives/alias.py
 boax/prediction/objectives/base.py
 boax/prediction/objectives/transformed.py
 boax/utils/__init__.py
 boax/utils/functools.py
 boax/utils/typing.py
```

### Comparing `boax-0.1.0/pyproject.toml` & `boax-0.1.1/pyproject.toml`

 * *Files identical despite different names*

