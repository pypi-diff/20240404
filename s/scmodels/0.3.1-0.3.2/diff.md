# Comparing `tmp/scmodels-0.3.1.tar.gz` & `tmp/scmodels-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmodels-0.3.1.tar", last modified: Tue Apr  2 09:12:37 2024, max compression
+gzip compressed data, was "scmodels-0.3.2.tar", last modified: Thu Apr  4 10:25:11 2024, max compression
```

## Comparing `scmodels-0.3.1.tar` & `scmodels-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.694341 scmodels-0.3.1/
--rw-r--r--   0 maichmueller   (501) staff       (20)     1075 2024-02-22 11:22:23.000000 scmodels-0.3.1/LICENSE.md
--rw-r--r--   0 maichmueller   (501) staff       (20)    13247 2024-04-02 09:12:37.694081 scmodels-0.3.1/PKG-INFO
--rw-r--r--   0 maichmueller   (501) staff       (20)    10946 2024-02-23 11:20:19.000000 scmodels-0.3.1/README.md
--rw-r--r--   0 maichmueller   (501) staff       (20)     1324 2024-04-02 09:11:54.000000 scmodels-0.3.1/pyproject.toml
--rw-r--r--   0 maichmueller   (501) staff       (20)       77 2024-02-22 20:59:48.000000 scmodels-0.3.1/requirements.txt
--rw-r--r--   0 maichmueller   (501) staff       (20)       38 2024-04-02 09:12:37.694400 scmodels-0.3.1/setup.cfg
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.686882 scmodels-0.3.1/src/
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.691755 scmodels-0.3.1/src/scmodels/
--rw-r--r--   0 maichmueller   (501) staff       (20)       21 2024-02-22 20:59:48.000000 scmodels-0.3.1/src/scmodels/__init__.py
--rw-r--r--   0 maichmueller   (501) staff       (20)     4409 2024-02-23 11:36:20.000000 scmodels-0.3.1/src/scmodels/parser.py
--rw-r--r--   0 maichmueller   (501) staff       (20)    47605 2024-04-02 08:57:33.000000 scmodels-0.3.1/src/scmodels/scm.py
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.693675 scmodels-0.3.1/src/scmodels.egg-info/
--rw-r--r--   0 maichmueller   (501) staff       (20)    13247 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/PKG-INFO
--rw-r--r--   0 maichmueller   (501) staff       (20)      316 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/SOURCES.txt
--rw-r--r--   0 maichmueller   (501) staff       (20)        1 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/dependency_links.txt
--rw-r--r--   0 maichmueller   (501) staff       (20)      103 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/requires.txt
--rw-r--r--   0 maichmueller   (501) staff       (20)        9 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/top_level.txt
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.693313 scmodels-0.3.1/test/
--rw-r--r--   0 maichmueller   (501) staff       (20)    14070 2024-04-01 20:23:29.000000 scmodels-0.3.1/test/test_scm.py
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-04 10:25:11.550746 scmodels-0.3.2/
+-rw-r--r--   0 maichmueller   (501) staff       (20)     1075 2024-02-22 11:22:23.000000 scmodels-0.3.2/LICENSE.md
+-rw-r--r--   0 maichmueller   (501) staff       (20)    13242 2024-04-04 10:25:11.550488 scmodels-0.3.2/PKG-INFO
+-rw-r--r--   0 maichmueller   (501) staff       (20)    10941 2024-04-04 10:23:18.000000 scmodels-0.3.2/README.md
+-rw-r--r--   0 maichmueller   (501) staff       (20)     1324 2024-04-04 10:23:18.000000 scmodels-0.3.2/pyproject.toml
+-rw-r--r--   0 maichmueller   (501) staff       (20)       77 2024-02-22 20:59:48.000000 scmodels-0.3.2/requirements.txt
+-rw-r--r--   0 maichmueller   (501) staff       (20)       38 2024-04-04 10:25:11.550804 scmodels-0.3.2/setup.cfg
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-04 10:25:11.546321 scmodels-0.3.2/src/
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-04 10:25:11.547775 scmodels-0.3.2/src/scmodels/
+-rw-r--r--   0 maichmueller   (501) staff       (20)       21 2024-02-22 20:59:48.000000 scmodels-0.3.2/src/scmodels/__init__.py
+-rw-r--r--   0 maichmueller   (501) staff       (20)     4450 2024-04-04 10:23:18.000000 scmodels-0.3.2/src/scmodels/parser.py
+-rw-r--r--   0 maichmueller   (501) staff       (20)    48463 2024-04-04 10:23:18.000000 scmodels-0.3.2/src/scmodels/scm.py
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-04 10:25:11.550059 scmodels-0.3.2/src/scmodels.egg-info/
+-rw-r--r--   0 maichmueller   (501) staff       (20)    13242 2024-04-04 10:25:11.000000 scmodels-0.3.2/src/scmodels.egg-info/PKG-INFO
+-rw-r--r--   0 maichmueller   (501) staff       (20)      316 2024-04-04 10:25:11.000000 scmodels-0.3.2/src/scmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 maichmueller   (501) staff       (20)        1 2024-04-04 10:25:11.000000 scmodels-0.3.2/src/scmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 maichmueller   (501) staff       (20)      103 2024-04-04 10:25:11.000000 scmodels-0.3.2/src/scmodels.egg-info/requires.txt
+-rw-r--r--   0 maichmueller   (501) staff       (20)        9 2024-04-04 10:25:11.000000 scmodels-0.3.2/src/scmodels.egg-info/top_level.txt
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-04 10:25:11.549533 scmodels-0.3.2/test/
+-rw-r--r--   0 maichmueller   (501) staff       (20)    14070 2024-04-04 10:23:18.000000 scmodels-0.3.2/test/test_scm.py
```

### Comparing `scmodels-0.3.1/LICENSE.md` & `scmodels-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scmodels-0.3.1/PKG-INFO` & `scmodels-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmodels
-Version: 0.3.1
+Version: 0.3.2
 Summary: Structural Causal Models
 Author-email: Michael Aichmueller <m.aichmueller@gmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2019 Michael
         
@@ -112,19 +112,19 @@
 Note that in this case, one must not restate the noise symbol string in the distribution (as would otherwise be necessary in constructing sympy distributions).
 
 
 ```python
 from scmodels import SCM
 
 assignment_seq = [
-    "Z = M, M ~ LogLogistic(alpha=1, beta=1)",
-    "X = N * 3 * Z ** 2, N ~ LogNormal(mean=1, std=1)",
-    "Y = P + 2 * Z + sqrt(X), P ~ Normal(mean=2, std=1)",
-    "V = N**P + Z, N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
-    "W = exp(T) - log(M) * N + V, M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
+    "Z = M; M ~ LogLogistic(alpha=1, beta=1)",
+    "X = N * 3 * Z ** 2; N ~ LogNormal(mean=1, std=1)",
+    "Y = P + 2 * Z + sqrt(X); P ~ Normal(mean=2, std=1)",
+    "V = N**P + Z; N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
+    "W = exp(T) - log(M) * N + V; M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
 ]
 
 myscm = SCM(assignment_seq)
 ```
 
 Agreements:
 - The name of the noise variable in the distribution specification
@@ -296,15 +296,15 @@
 
 
 ```python
 myscm.do_intervention([("X", 1)])
 
 from sympy.stats import FiniteRV
 
-myscm.soft_intervention([("X", FiniteRV(str(myscm["X"].noise), density={-1: .5, 1: .5}))])
+myscm.soft_intervention([("X", FiniteRV(myscm["X"].noise[0].name, density={-1: .5, 1: .5}))])
 ```
 
 Refer to the `sympy` docs for more information on building random variables.
 
 Calling `undo_intervention` restores the original state of *all* variables.
 If variables are specified (`variables=['X', 'Y']`), any interventions on *only those variables* are undone.
 
@@ -322,21 +322,21 @@
 n = 5
 samples = myscm.sample(n)
 
 display_data(samples)
 ```
 
 
-|    |        Z |        V |          X |         W |         Y |
-|----|----------|----------|------------|-----------|-----------|
-|  0 | 1.32652  |  2.32652 |  7.33384   |   3.20107 |  6.52168  |
-|  1 | 1.13431  |  2.13431 |  3.8058    | 854.798   |  5.46616  |
-|  2 | 0.573739 | -1.31797 |  1.77705   |  -2.68093 |  5.23906  |
-|  3 | 1.21373  |  2.21373 | 30.1412    |   2.0016  | 11.172    |
-|  4 | 0.117316 |  1.11732 |  0.0147985 |   1.35366 |  0.950457 |
+|    |        Z |        V |         X |       W |        Y |
+|----|----------|----------|-----------|---------|----------|
+|  0 | 0.854202 | 0.193336 | 15.9145   | 1.60315 |  7.55694 |
+|  1 | 0.634422 | 0.951119 |  2.43486  | 5.59541 |  3.6478  |
+|  2 | 1.02354  | 2.02354  |  4.11357  | 2.12862 |  6.23834 |
+|  3 | 0.376173 | 2.2962   |  0.252316 | 2.83333 |  3.64392 |
+|  4 | 4.19568  | 2.894    | 36.2844   | 3.07636 | 16.4083  |
 
 
 If infinite sampling is desired, one can also receive a sampling generator through 
 
 
 ```python
 container = {var: [] for var in myscm}
@@ -350,36 +350,36 @@
 for i in range(n):
     next(sampler)
 
 display_data(container)
 ```
 
 
-|    |         Z |         V |         X |        W |       Y |
-|----|-----------|-----------|-----------|----------|---------|
-|  0 | 0.630663  | -0.151095 | 3.73489   |  2.18306 | 5.02001 |
-|  1 | 0.0978569 |  1.09786  | 0.0875172 | 77.555   | 2.47965 |
-|  2 | 0.225186  |  1.22519  | 0.264414  |  6.47678 | 3.98214 |
-|  3 | 0.143525  |  1.14352  | 0.254132  | 28.4377  | 3.5462  |
-|  4 | 1.13363   |  1.15934  | 6.6198    |  1.38153 | 7.38624 |
+|    |        Z |         V |          X |            W |        Y |
+|----|----------|-----------|------------|--------------|----------|
+|  0 | 0.245579 |  0.814717 |   1.59715  |  2.10267     |  2.26984 |
+|  1 | 7.88344  |  8.88344  | 122.197    |  1.90523e+13 | 29.1743  |
+|  2 | 1.26534  |  1.29397  |  12.5345   |  0.523827    |  8.77073 |
+|  3 | 1.37904  |  2.37904  |  13.327    |  2.08063     |  9.14935 |
+|  4 | 0.230563 | -0.966714 |   0.354393 | -1.22201     |  3.09432 |
 
 
 If the target container is not provided, the generator returns a new `dict` for every sample.
 
 
 ```python
 sample = next(myscm.sample_iter())
 
 display_data(sample)
 ```
 
 
-|    |        Z |       V |         X |       W |       Y |
-|----|----------|---------|-----------|---------|---------|
-|  0 | 0.124314 | 1.12431 | 0.0717258 | 2.43763 | 3.94194 |
+|    |       Z |      V |       X |      W |       Y |
+|----|---------|--------|---------|--------|---------|
+|  0 | 2.02308 | 3.1259 | 59.8718 | 4.2209 | 13.7312 |
 
 
 ## Plotting
 If you have graphviz installed, you can plot the DAG by calling
 
 ```python
 myscm.plot(node_size=1000, alpha=1)
```

### Comparing `scmodels-0.3.1/README.md` & `scmodels-0.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -61,19 +61,19 @@
 Note that in this case, one must not restate the noise symbol string in the distribution (as would otherwise be necessary in constructing sympy distributions).
 
 
 ```python
 from scmodels import SCM
 
 assignment_seq = [
-    "Z = M, M ~ LogLogistic(alpha=1, beta=1)",
-    "X = N * 3 * Z ** 2, N ~ LogNormal(mean=1, std=1)",
-    "Y = P + 2 * Z + sqrt(X), P ~ Normal(mean=2, std=1)",
-    "V = N**P + Z, N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
-    "W = exp(T) - log(M) * N + V, M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
+    "Z = M; M ~ LogLogistic(alpha=1, beta=1)",
+    "X = N * 3 * Z ** 2; N ~ LogNormal(mean=1, std=1)",
+    "Y = P + 2 * Z + sqrt(X); P ~ Normal(mean=2, std=1)",
+    "V = N**P + Z; N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
+    "W = exp(T) - log(M) * N + V; M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
 ]
 
 myscm = SCM(assignment_seq)
 ```
 
 Agreements:
 - The name of the noise variable in the distribution specification
@@ -245,15 +245,15 @@
 
 
 ```python
 myscm.do_intervention([("X", 1)])
 
 from sympy.stats import FiniteRV
 
-myscm.soft_intervention([("X", FiniteRV(str(myscm["X"].noise), density={-1: .5, 1: .5}))])
+myscm.soft_intervention([("X", FiniteRV(myscm["X"].noise[0].name, density={-1: .5, 1: .5}))])
 ```
 
 Refer to the `sympy` docs for more information on building random variables.
 
 Calling `undo_intervention` restores the original state of *all* variables.
 If variables are specified (`variables=['X', 'Y']`), any interventions on *only those variables* are undone.
 
@@ -271,21 +271,21 @@
 n = 5
 samples = myscm.sample(n)
 
 display_data(samples)
 ```
 
 
-|    |        Z |        V |          X |         W |         Y |
-|----|----------|----------|------------|-----------|-----------|
-|  0 | 1.32652  |  2.32652 |  7.33384   |   3.20107 |  6.52168  |
-|  1 | 1.13431  |  2.13431 |  3.8058    | 854.798   |  5.46616  |
-|  2 | 0.573739 | -1.31797 |  1.77705   |  -2.68093 |  5.23906  |
-|  3 | 1.21373  |  2.21373 | 30.1412    |   2.0016  | 11.172    |
-|  4 | 0.117316 |  1.11732 |  0.0147985 |   1.35366 |  0.950457 |
+|    |        Z |        V |         X |       W |        Y |
+|----|----------|----------|-----------|---------|----------|
+|  0 | 0.854202 | 0.193336 | 15.9145   | 1.60315 |  7.55694 |
+|  1 | 0.634422 | 0.951119 |  2.43486  | 5.59541 |  3.6478  |
+|  2 | 1.02354  | 2.02354  |  4.11357  | 2.12862 |  6.23834 |
+|  3 | 0.376173 | 2.2962   |  0.252316 | 2.83333 |  3.64392 |
+|  4 | 4.19568  | 2.894    | 36.2844   | 3.07636 | 16.4083  |
 
 
 If infinite sampling is desired, one can also receive a sampling generator through 
 
 
 ```python
 container = {var: [] for var in myscm}
@@ -299,36 +299,36 @@
 for i in range(n):
     next(sampler)
 
 display_data(container)
 ```
 
 
-|    |         Z |         V |         X |        W |       Y |
-|----|-----------|-----------|-----------|----------|---------|
-|  0 | 0.630663  | -0.151095 | 3.73489   |  2.18306 | 5.02001 |
-|  1 | 0.0978569 |  1.09786  | 0.0875172 | 77.555   | 2.47965 |
-|  2 | 0.225186  |  1.22519  | 0.264414  |  6.47678 | 3.98214 |
-|  3 | 0.143525  |  1.14352  | 0.254132  | 28.4377  | 3.5462  |
-|  4 | 1.13363   |  1.15934  | 6.6198    |  1.38153 | 7.38624 |
+|    |        Z |         V |          X |            W |        Y |
+|----|----------|-----------|------------|--------------|----------|
+|  0 | 0.245579 |  0.814717 |   1.59715  |  2.10267     |  2.26984 |
+|  1 | 7.88344  |  8.88344  | 122.197    |  1.90523e+13 | 29.1743  |
+|  2 | 1.26534  |  1.29397  |  12.5345   |  0.523827    |  8.77073 |
+|  3 | 1.37904  |  2.37904  |  13.327    |  2.08063     |  9.14935 |
+|  4 | 0.230563 | -0.966714 |   0.354393 | -1.22201     |  3.09432 |
 
 
 If the target container is not provided, the generator returns a new `dict` for every sample.
 
 
 ```python
 sample = next(myscm.sample_iter())
 
 display_data(sample)
 ```
 
 
-|    |        Z |       V |         X |       W |       Y |
-|----|----------|---------|-----------|---------|---------|
-|  0 | 0.124314 | 1.12431 | 0.0717258 | 2.43763 | 3.94194 |
+|    |       Z |      V |       X |      W |       Y |
+|----|---------|--------|---------|--------|---------|
+|  0 | 2.02308 | 3.1259 | 59.8718 | 4.2209 | 13.7312 |
 
 
 ## Plotting
 If you have graphviz installed, you can plot the DAG by calling
 
 ```python
 myscm.plot(node_size=1000, alpha=1)
```

### Comparing `scmodels-0.3.1/pyproject.toml` & `scmodels-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'scmodels'
-version = '0.3.1'
+version = '0.3.2'
 authors = [
     { name = 'Michael Aichmueller', email = 'm.aichmueller@gmail.com' }
 ]
 license = { file = "LICENSE.md" }
 description = 'Structural Causal Models'
 readme = "README.md"
 keywords = [
```

### Comparing `scmodels-0.3.1/src/scmodels/parser.py` & `scmodels-0.3.2/src/scmodels/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from sympy.functions import *
 from sympy.stats import *
 
 from typing import *
 
 all_stats_imports = set(sympy.stats.__all__)
 
-var_p = regex.compile(r"(?<=([(]|[)*+-/%]))\w+(?=([)*+-/%]+|$))|^\w+(?=([)*+-/%]+|$))")
+var_p = regex.compile(
+    r"(?<=([(]|[)\*\+\-\/\>\<\%\s,]))\w+(?=([)\*\+\>\<\-\/\%\s,]+|$))|^\w+(?=([)\*\+\-\>\<\/\%\s]+|$))"
+)
 digit_p = regex.compile(r"^\d+$")
 
 
 def parse_assignments(assignment_strs: Sequence[str]):
     """
     This parses a list of assignment strings. The assignments are supposed to be given in the following form:
 
@@ -33,15 +35,15 @@
         The functional map of variables with their parents, assignment strings, and noise models as needed to construct
         an SCM object.
     """
     functional_map = dict()
     for assignment in assignment_strs:
         # split the assignment 'X = f(Parents, Noise), Noise ~ D' into [X, f(Parents, Noise), Noise ~ D]
         assign_var, assignment_n_noise = assignment.split("=", 1)
-        assign_noise_split = assignment_n_noise.split(",", 1)
+        assign_noise_split = assignment_n_noise.split(";", 1)
 
         if len(assign_noise_split) == 1:
             # this is the case when there was no ',' separating functional body and noise distribution specification
             assign_str = assign_noise_split[0]
             model_sym = []
         else:
             assign_str, noise_str = assign_noise_split
```

### Comparing `scmodels-0.3.1/src/scmodels/scm.py` & `scmodels-0.3.2/src/scmodels/scm.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 from sympy.stats.rv import RandomSymbol
 from sympy.functions import *
 
 from scmodels.parser import parse_assignments, extract_parents
 
 RV: Type[RandomSymbol] = RandomSymbol
 AssignmentSeq = Sequence[str]
-AssignmentMap = Dict[str, Union[Tuple[str, RV], Tuple[List[str], Callable, RV]]]
+AssignmentMap = Dict[
+    str, Union[Tuple[str, RV], Tuple[Union[Sequence[str], str], Callable, RV]]
+]
 
 
 class Assignment:
     noise_prefix = "__noise"
     noise_suffix = "__"
     noise_argsep = "@"
     noise_sep = ":"
@@ -138,15 +140,15 @@
         noise_repr: List[str]
 
     def __init__(
         self,
         assignments: Union[AssignmentMap, AssignmentSeq],
         variable_tex_names: Optional[Dict] = None,
         seed: Optional[int] = None,
-        scm_name: str = "Structural Causal Model",
+        name: str = "Structural Causal Model",
     ):
         """
         Construct the SCM from an assignment map with the variables as keys and its assignment information
         as tuple of parents, assignment, and noise distribution or provide the assignments in a list of strings, which
         directly tell
 
         Notes
@@ -205,25 +207,26 @@
             A collection of the latex names for the variables in the causal graph. The dict needs to provide a tex name
             for each passed variable name in the form: {"VarName": "VarName_in_TeX"}.
             Any variable that is missing in the dictionary will be assumed to accept its current name as the TeX
             version.
             If not provided, defaults to the input names in the functional map.
         seed: (optional) str,
             Seeding the graph for reproducibility.
-        scm_name: (optional) str,
+        name: (optional) str,
             The name of the SCM. Default is 'Structural Causal Model'.
         """
-        self.scm_name: str = scm_name
+        self.name: str = name
         self.rng_state = np.random.default_rng()  # we always have a local RNG machine
         self.seed(seed)
 
         # a backup dictionary of the original assignments of the intervened variables,
         # in order to undo the interventions later.
         self.interventions_backup_attr: Dict = dict()
         self.interventions_backup_parent: Dict = dict()
+        self.interventions_backup_roots: Dict = dict()
 
         # build the graph:
         # any node will be given the attributes of function and noise to later sample from and also an incoming edge
         # from its causal parent. We will store the causal root nodes separately.
         self.dag = nx.DiGraph()
         self.roots: List = []
         self.insert(assignments)
@@ -509,18 +512,22 @@
             if var not in self.interventions_backup_attr:
                 # the variable has NOT already been backed up. If we overwrite it now it is fine. If it had already been
                 # in the backup, then we would need to pass on this step, in order to not overwrite the backup
                 # (possibly with a previous intervention)
                 self.interventions_backup_attr[var] = deepcopy(self.dag.nodes[var])
 
             if var not in self.interventions_backup_parent:
-                # the same logic goes for the parents backup.
+                # the same logic applies to the parents backup.
                 parent_backup = list(self.dag.predecessors(var))
                 self.interventions_backup_parent[var] = parent_backup
                 self.dag.remove_edges_from([(parent, var) for parent in parent_backup])
+
+            if var not in self.interventions_backup_roots:
+                # the same logic applies to the roots backup.
+                self.interventions_backup_roots[var] = self.roots.copy()
             # patch up the attr dict as the provided items were merely strings and now need to be parsed by sympy.
             intervention_assignment_map[var] = items
         self.insert(intervention_assignment_map)
 
     def do_intervention(self, var_val_pairs: Iterable[Tuple[str, float]]):
         """
         Perform do-interventions, i.e. setting specific variables to a constant value.
@@ -531,15 +538,15 @@
         Parameters
         ----------
         var_val_pairs, Iterable of str-float tuples,
             the variables to intervene on with their new values.
         """
         interventions_dict = dict()
         for var, val in var_val_pairs:
-            interventions_dict[var] = (None, str(val), None)
+            interventions_dict[var] = ([], str(val), None)
         self.intervention(interventions_dict)
 
     def soft_intervention(
         self,
         var_noise_pairs: Sequence[Tuple[str, Sequence[RV]]],
     ):
         """
@@ -574,25 +581,27 @@
         else:
             present_variables = list(self.interventions_backup_attr.keys())
 
         for var in present_variables:
             try:
                 attr_dict = self.interventions_backup_attr.pop(var)
                 parents = self.interventions_backup_parent.pop(var)
+                roots = self.interventions_backup_roots.pop(var)
             except KeyError:
                 logging.warning(
                     f"Variable '{var}' not found in intervention backup. Omitting it."
                 )
                 continue
 
             self.dag.add_node(var, **attr_dict)
             self.dag.remove_edges_from(
                 [(parent, var) for parent in self.dag.predecessors(var)]
             )
             self.dag.add_edges_from([(parent, var) for parent in parents])
+            self.roots = roots
 
     def d_separated(
         self, x: Sequence[str], y: Sequence[str], s: Optional[Sequence[str]] = None
     ):
         """
         Checks if all variables in X are d-separated from all variables in Y by the variables in S.
 
@@ -616,15 +625,15 @@
             self.dag, set(x), set(y), set(s) if s is not None else set()
         )
 
     def moral_graph(self):
         """
         Returns the moral graph of the underlying DAG.
 
-        The moral graph is the underlying DAG with all edges made undirected and collider parents connected.
+        The moral graph is the underlying DAG with all edges made undirected and v-structure parents connected.
 
         Notes
         -----
         "Unmarried" parents of a common child are being "married" by this process, hence the name "moral graph".
 
         Returns
         -------
@@ -636,16 +645,15 @@
     def collider_iter(
         self, only_v_structure: bool = False
     ) -> Generator[ColliderView, None, None]:
         """
         Provide a generator that yields all colliders of the underlying DAG.
 
         Colliders are triples of nodes (parent, child, other_parent)
-        in which both parent and other_parent causally affect the child,
-        but not each other.
+        in which both parent and other_parent causally affect the child.
 
         Returns
         -------
         Generator[ColliderView, None, None],
             the colliders/v-structures found
         """
         dag = self.dag
@@ -701,14 +709,19 @@
                     parents, assignment_str, noise_model_list
                 )
                 rv = sympify_assignment(self, parents, assignment_str, noise_model_list)
 
             # a sequence of size 3 is expected to be (parents list, assignment string, noise model)
             elif len(assignment_pack) == 3:
                 parents, assignment_func, noise_model_list = assignment_pack
+                if isinstance(parents, str):
+                    # if the parents are a string we expect it to be delimited by a semicolon
+                    parents = parents.split(";")
+                else:
+                    assert isinstance(parents, Sequence)
                 if isinstance(noise_model_list, RV):
                     noise_model_list = [noise_model_list]
                 assert callable(
                     assignment_func
                 ), "Assignment tuple holds 3 elements, but the function entry is not callable."
                 assignment_str = None
                 try:
@@ -822,37 +835,39 @@
             arguments to be passed to the ``networkx.draw`` method. Check its documentation for a full list.
 
         Returns
         -------
         tuple,
             the plt.figure and figure-axis objects holding the graph plot.
         """
-        if nx.is_tree(self.dag):
-            pos = hierarchy_pos(self.dag, root_node=self.roots[0])
-        else:
-            pos = graphviz_layout(self.dag, prog="dot")
+        pos = kwargs.get("pos", None)
+        if pos is None:
+            if nx.is_tree(self.dag):
+                pos = hierarchy_pos(self.dag, root_node=self.roots[0])
+            else:
+                pos = graphviz_layout(self.dag, prog="dot")
         if draw_labels:
             labels = self.var_draw_dict
         else:
             labels = {}
         fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
-        ax.set_title(self.scm_name)
+        ax.set_title(self.name)
         nx.draw(
             self.dag,
             pos=pos,
             ax=ax,
             labels=labels,
             with_labels=True,
             node_size=node_size,
             alpha=alpha,
             **kwargs,
         )
         if savepath is not None:
             fig.savefig(savepath)
-        return fig, ax
+        return fig, ax, pos
 
     def get_variables(self, causal_order: bool = True) -> List[str]:
         """
         Get a list of the variables in the SCM.
 
         Parameters
         ----------
@@ -1006,20 +1021,25 @@
     for noise_model in noise_model_list:
         symbols.append(noise_model)
         # Allocate the noise model variable as normal symbol. This is necessary for lambdifying.
         lcls[str(noise_model)] = noise_model
     for par in parents:
         lcls[par] = sympy.Symbol(par)
         symbols.append(lcls[par])
-    assignment = sympy.sympify(eval(assignment_str))
+    try:
+        assignment = sympy.sympify(eval(assignment_str))
+    except (TypeError, ValueError) as e:
+        raise type(e)(
+            f"Assignment {assignment_str} could not be sympified. Error reads:\n{e}"
+        )
     try:
         assignment = sympy.lambdify(symbols, assignment, "numpy")
     except (NameError, ValueError) as e:
         warnings.warn(
-            f"The assignment string could not be resolved in numpy, the error message reads: {e}\n"
+            f"Assignment string {assignment_str} could not be resolved in numpy, the error message reads: {e}\n"
             f"Lambdifying without numpy.",
         )
         assignment = sympy.lambdify(symbols, assignment)
 
     return assignment
```

### Comparing `scmodels-0.3.1/src/scmodels.egg-info/PKG-INFO` & `scmodels-0.3.2/src/scmodels.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmodels
-Version: 0.3.1
+Version: 0.3.2
 Summary: Structural Causal Models
 Author-email: Michael Aichmueller <m.aichmueller@gmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2019 Michael
         
@@ -112,19 +112,19 @@
 Note that in this case, one must not restate the noise symbol string in the distribution (as would otherwise be necessary in constructing sympy distributions).
 
 
 ```python
 from scmodels import SCM
 
 assignment_seq = [
-    "Z = M, M ~ LogLogistic(alpha=1, beta=1)",
-    "X = N * 3 * Z ** 2, N ~ LogNormal(mean=1, std=1)",
-    "Y = P + 2 * Z + sqrt(X), P ~ Normal(mean=2, std=1)",
-    "V = N**P + Z, N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
-    "W = exp(T) - log(M) * N + V, M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
+    "Z = M; M ~ LogLogistic(alpha=1, beta=1)",
+    "X = N * 3 * Z ** 2; N ~ LogNormal(mean=1, std=1)",
+    "Y = P + 2 * Z + sqrt(X); P ~ Normal(mean=2, std=1)",
+    "V = N**P + Z; N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
+    "W = exp(T) - log(M) * N + V; M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
 ]
 
 myscm = SCM(assignment_seq)
 ```
 
 Agreements:
 - The name of the noise variable in the distribution specification
@@ -296,15 +296,15 @@
 
 
 ```python
 myscm.do_intervention([("X", 1)])
 
 from sympy.stats import FiniteRV
 
-myscm.soft_intervention([("X", FiniteRV(str(myscm["X"].noise), density={-1: .5, 1: .5}))])
+myscm.soft_intervention([("X", FiniteRV(myscm["X"].noise[0].name, density={-1: .5, 1: .5}))])
 ```
 
 Refer to the `sympy` docs for more information on building random variables.
 
 Calling `undo_intervention` restores the original state of *all* variables.
 If variables are specified (`variables=['X', 'Y']`), any interventions on *only those variables* are undone.
 
@@ -322,21 +322,21 @@
 n = 5
 samples = myscm.sample(n)
 
 display_data(samples)
 ```
 
 
-|    |        Z |        V |          X |         W |         Y |
-|----|----------|----------|------------|-----------|-----------|
-|  0 | 1.32652  |  2.32652 |  7.33384   |   3.20107 |  6.52168  |
-|  1 | 1.13431  |  2.13431 |  3.8058    | 854.798   |  5.46616  |
-|  2 | 0.573739 | -1.31797 |  1.77705   |  -2.68093 |  5.23906  |
-|  3 | 1.21373  |  2.21373 | 30.1412    |   2.0016  | 11.172    |
-|  4 | 0.117316 |  1.11732 |  0.0147985 |   1.35366 |  0.950457 |
+|    |        Z |        V |         X |       W |        Y |
+|----|----------|----------|-----------|---------|----------|
+|  0 | 0.854202 | 0.193336 | 15.9145   | 1.60315 |  7.55694 |
+|  1 | 0.634422 | 0.951119 |  2.43486  | 5.59541 |  3.6478  |
+|  2 | 1.02354  | 2.02354  |  4.11357  | 2.12862 |  6.23834 |
+|  3 | 0.376173 | 2.2962   |  0.252316 | 2.83333 |  3.64392 |
+|  4 | 4.19568  | 2.894    | 36.2844   | 3.07636 | 16.4083  |
 
 
 If infinite sampling is desired, one can also receive a sampling generator through 
 
 
 ```python
 container = {var: [] for var in myscm}
@@ -350,36 +350,36 @@
 for i in range(n):
     next(sampler)
 
 display_data(container)
 ```
 
 
-|    |         Z |         V |         X |        W |       Y |
-|----|-----------|-----------|-----------|----------|---------|
-|  0 | 0.630663  | -0.151095 | 3.73489   |  2.18306 | 5.02001 |
-|  1 | 0.0978569 |  1.09786  | 0.0875172 | 77.555   | 2.47965 |
-|  2 | 0.225186  |  1.22519  | 0.264414  |  6.47678 | 3.98214 |
-|  3 | 0.143525  |  1.14352  | 0.254132  | 28.4377  | 3.5462  |
-|  4 | 1.13363   |  1.15934  | 6.6198    |  1.38153 | 7.38624 |
+|    |        Z |         V |          X |            W |        Y |
+|----|----------|-----------|------------|--------------|----------|
+|  0 | 0.245579 |  0.814717 |   1.59715  |  2.10267     |  2.26984 |
+|  1 | 7.88344  |  8.88344  | 122.197    |  1.90523e+13 | 29.1743  |
+|  2 | 1.26534  |  1.29397  |  12.5345   |  0.523827    |  8.77073 |
+|  3 | 1.37904  |  2.37904  |  13.327    |  2.08063     |  9.14935 |
+|  4 | 0.230563 | -0.966714 |   0.354393 | -1.22201     |  3.09432 |
 
 
 If the target container is not provided, the generator returns a new `dict` for every sample.
 
 
 ```python
 sample = next(myscm.sample_iter())
 
 display_data(sample)
 ```
 
 
-|    |        Z |       V |         X |       W |       Y |
-|----|----------|---------|-----------|---------|---------|
-|  0 | 0.124314 | 1.12431 | 0.0717258 | 2.43763 | 3.94194 |
+|    |       Z |      V |       X |      W |       Y |
+|----|---------|--------|---------|--------|---------|
+|  0 | 2.02308 | 3.1259 | 59.8718 | 4.2209 | 13.7312 |
 
 
 ## Plotting
 If you have graphviz installed, you can plot the DAG by calling
 
 ```python
 myscm.plot(node_size=1000, alpha=1)
```

### Comparing `scmodels-0.3.1/test/test_scm.py` & `scmodels-0.3.2/test/test_scm.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,36 +68,36 @@
 
 
 def same_elements(list1, list2):
     return np.isin(list1, list2).all() and np.isin(list2, list1).all()
 
 
 def test_parsing():
-    test_str = "Z_1 = Noise + 2*log(Y), Noise ~ Normal(0,1)"
+    test_str = "Z_1 = Noise + 2*log(Y); Noise ~ Normal(0,1)"
     func_map = parse_assignments([test_str])
     assert func_map["Z_1"][0] == "Noise + 2*log(Y)"
     assert str(func_map["Z_1"][1][0]) == "Noise"
     assert extract_parents(func_map["Z_1"][0], "Noise") == ["Y"]
 
-    test_str = "X = N + sqrt(X_45 ** M + 342 * 2) / (  43 * FG_2) + P, N ~ Normal(0,1)"
+    test_str = "X = N + sqrt(X_45 ** M + 342 * 2) / (  43 * FG_2) + P; N ~ Normal(0,1)"
     func_map = parse_assignments([test_str])
     assert func_map["X"][0] == "N + sqrt(X_45 ** M + 342 * 2) / (  43 * FG_2) + P"
     assert str(func_map["X"][1][0]) == "N"
     assert same_elements(
         extract_parents(func_map["X"][0], "N"), ["X_45", "M", "FG_2", "P"]
     )
 
 
 def test_scm_from_strings():
     scm = SCM(
         [
-            "X = N, N ~ Normal(0,1)",
-            "Y_0 = M + 2 * exp(X), M ~ StudentT(2)",
-            "Y_1 = M + 2 * exp(sqrt(X)), M ~ Normal(0, 0.1)",
-            "Z = P * sqrt(Y_0), P ~ Exponential(5.3)",
+            "X = N; N ~ Normal(0,1)",
+            "Y_0 = M + 2 * exp(X); M ~ StudentT(2)",
+            "Y_1 = M + 2 * exp(sqrt(X)); M ~ Normal(0, 0.1)",
+            "Z = P * sqrt(Y_0); P ~ Exponential(5.3)",
         ]
     )
     assert same_elements(scm.get_variables(), ["X", "Y_0", "Y_1", "Z"])
 
 
 def test_scm_build_from_assignmentmap():
     cn = build_scm_from_assignmentmap()
@@ -307,15 +307,15 @@
     n = 20
     sample = cn.sample(n, seed=1)
     sample2 = cn.sample(n, seed=1)
     assert (sample.to_numpy() == sample2.to_numpy()).all()
 
 
 def test_none_noise():
-    cn = SCM(["X = 1", "Y = N + X, N ~ Normal(0,1)"], seed=0)
+    cn = SCM(["X = 1", "Y = N + X; N ~ Normal(0,1)"], seed=0)
     n = 10
     sample = cn.sample(n)
     manual_y = np.random.default_rng(0).normal(size=n) + 1
     assert (sample["X"] == 1).all()
     assert (sample["Y"] == manual_y).all()
 
     sample = {var: [] for var in cn.get_variables()}
@@ -327,16 +327,16 @@
     assert (sample["Y"] == manual_y).all()
 
 
 def test_compositional_noise():
     cn = SCM(
         [
             "X = 1",
-            "Y = N**2 + X, N ~ Normal(0,1)",
-            "Z = T*M + Y, M ~ Exponential(1) / T ~ StudentT(0.5)",
+            "Y = N**2 + X; N ~ Normal(0,1)",
+            "Z = T*M + Y; M ~ Exponential(1) / T ~ StudentT(0.5)",
         ],
         seed=0,
     )
     n = 100
     samples = cn.sample(n)
     rng = np.random.default_rng(0)
     manual_y = (rng.normal(size=n)) ** 2 + 1
@@ -347,18 +347,18 @@
     assert np.isclose(np.mean(samples["Y"]), np.mean(manual_y))
     assert np.isclose(np.mean(samples["Z"]), np.mean(manual_z))
 
 
 def test_compositional_noise_intervention():
     cn = SCM(
         [
-            "X = N, N ~ Normal(0,1)",
-            "Y = B**2 + X, B ~ Normal(0,1)",
-            "Z = T*M + Y, M ~ Exponential(1) / T ~ StudentT(0.5)",
-            "V = L + 2 * (X**2), L ~ Normal(0,1)",
+            "X = N; N ~ Normal(0,1)",
+            "Y = B**2 + X; B ~ Normal(0,1)",
+            "Z = T*M + Y; M ~ Exponential(1) / T ~ StudentT(0.5)",
+            "V = L + 2 * (X**2); L ~ Normal(0,1)",
         ],
         seed=0,
     )
     noise_prev = cn["Z"].noise
     interv_noise = [Normal("K", -3.14, 2.713), Normal("D", 1.41, 7)]
     interv_assignment = lambda k, d, v: (k + d) * v / 2
     intervention_dict = {"Z": (["V"], interv_assignment, interv_noise)}
@@ -372,16 +372,16 @@
     assert cn["Z"].noise == noise_prev
 
 
 def test_compositional_noise_multi():
     cn = SCM(
         [
             "X = 1",
-            "Y = N**P + X, N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
-            "Z = exp(T) - log(M) * N + Y, M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
+            "Y = N**P + X; N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
+            "Z = exp(T) - log(M) * N + Y; M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
         ],
         seed=0,
     )
     n = 100
     samples = cn.sample(n)
     rng = np.random.default_rng(0)
     manual_y = rng.normal(size=n) ** rng.binomial(1, 0.5, size=n) + 1
```

