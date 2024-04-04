# Comparing `tmp/octofitterpy-2.3.3.tar.gz` & `tmp/octofitterpy-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octofitterpy-2.3.3.tar", last modified: Fri Mar  8 17:52:15 2024, max compression
+gzip compressed data, was "octofitterpy-2.3.4.tar", last modified: Thu Apr  4 16:59:55 2024, max compression
```

## Comparing `octofitterpy-2.3.3.tar` & `octofitterpy-2.3.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:52:15.076650 octofitterpy-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:52:15.060650 octofitterpy-2.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:52:15.060650 octofitterpy-2.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.github/workflows/CI_Windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.github/workflows/CI_large_nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.github/workflows/CI_mac.yml
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.github/workflows/pypi_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.github/workflows/update_backend.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-03-08 17:52:15.076650 octofitterpy-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:52:15.068650 octofitterpy-2.3.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   404631 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/examples/HIP100123-pairplot-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/examples/HIP100123-plot-grid-colorbar.png
--rw-r--r--   0 runner    (1001) docker     (127)   842730 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/examples/HIP100123-plot-grid.png
--rw-r--r--   0 runner    (1001) docker     (127)  4200567 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/examples/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (127)  2402698 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/examples/gallery.png
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:52:15.072650 octofitterpy-2.3.3/octofitterpy/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/octofitterpy/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/octofitterpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/octofitterpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/octofitterpy/julia_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/octofitterpy/julia_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/octofitterpy/juliapkg.json
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/octofitterpy/python_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-08 17:52:14.000000 octofitterpy-2.3.3/octofitterpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:52:15.076650 octofitterpy-2.3.3/octofitterpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-03-08 17:52:14.000000 octofitterpy-2.3.3/octofitterpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-08 17:52:15.000000 octofitterpy-2.3.3/octofitterpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:52:14.000000 octofitterpy-2.3.3/octofitterpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-08 17:52:14.000000 octofitterpy-2.3.3/octofitterpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-08 17:52:14.000000 octofitterpy-2.3.3/octofitterpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 17:52:15.076650 octofitterpy-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-08 17:52:02.000000 octofitterpy-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:59:55.103524 octofitterpy-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:59:55.087524 octofitterpy-2.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:59:55.091524 octofitterpy-2.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.github/workflows/CI_Windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.github/workflows/CI_large_nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.github/workflows/CI_mac.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.github/workflows/pypi_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.github/workflows/update_backend.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-04 16:59:55.103524 octofitterpy-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:59:55.099524 octofitterpy-2.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   404631 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/examples/HIP100123-pairplot-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/examples/HIP100123-plot-grid-colorbar.png
+-rw-r--r--   0 runner    (1001) docker     (127)   842730 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/examples/HIP100123-plot-grid.png
+-rw-r--r--   0 runner    (1001) docker     (127)  4200567 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/examples/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2402698 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/examples/gallery.png
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:59:55.103524 octofitterpy-2.3.4/octofitterpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/octofitterpy/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/octofitterpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/octofitterpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/octofitterpy/julia_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/octofitterpy/julia_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/octofitterpy/juliapkg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/octofitterpy/python_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-04 16:59:54.000000 octofitterpy-2.3.4/octofitterpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:59:55.103524 octofitterpy-2.3.4/octofitterpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-04 16:59:55.000000 octofitterpy-2.3.4/octofitterpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-04 16:59:55.000000 octofitterpy-2.3.4/octofitterpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:59:55.000000 octofitterpy-2.3.4/octofitterpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 16:59:55.000000 octofitterpy-2.3.4/octofitterpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 16:59:55.000000 octofitterpy-2.3.4/octofitterpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:59:55.103524 octofitterpy-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-04 16:59:39.000000 octofitterpy-2.3.4/setup.py
```

### Comparing `octofitterpy-2.3.3/.github/dependabot.yml` & `octofitterpy-2.3.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/.github/workflows/CI.yml` & `octofitterpy-2.3.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/.github/workflows/CI_Windows.yml` & `octofitterpy-2.3.4/.github/workflows/CI_Windows.yml`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/.github/workflows/CI_large_nightly.yml` & `octofitterpy-2.3.4/.github/workflows/CI_large_nightly.yml`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/.github/workflows/CI_mac.yml` & `octofitterpy-2.3.4/.github/workflows/CI_mac.yml`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/.github/workflows/pypi_deploy.yml` & `octofitterpy-2.3.4/.github/workflows/pypi_deploy.yml`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/.github/workflows/update_backend.yml` & `octofitterpy-2.3.4/.github/workflows/update_backend.yml`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/CITATION.md` & `octofitterpy-2.3.4/CITATION.md`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/LICENSE` & `octofitterpy-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/PKG-INFO` & `octofitterpy-2.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octofitterpy
-Version: 2.3.3
+Version: 2.3.4
 Summary: Fast and flexible orbit fitting
 Author-email: William Thompson <will.thompson@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 William Thompson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas<3.0.0,>=0.21.0
 Requires-Dist: numpy<2.0.0,>=1.13.0
-Requires-Dist: juliacall==0.9.15
+Requires-Dist: juliacall==0.9.19
 Requires-Dist: setuptools>=50.0.0
 
 # octofitterpy
 
 `octofitterpy` is a python package for performing Bayesian inference 
 against a wide variety of exoplanet / binary star data. It uses the [Octofitter.jl](https://sefffal.github.io/Octofitter.jl/)
 julia package under the hood (just like eg numpy uses C).
@@ -94,15 +94,15 @@
     likelihoods=[],
     companions=[planet_b]
 )
 model = octo.LogDensityModel(sys) # Compile model
 chain = octo.octofit(model) # Sample model
 octo.octoplot(model,chain) # Plot orbits
 octo.octocorner(model,chain,small=True) # Make corner plot
-octo.savechains("table.fits", chain)
+octo.savechain("table.fits", chain)
 ```
 
 ![](examples/HIP100123-plot-grid.png)
 ![](examples/HIP100123-pairplot-small.png)
 
 
 ## Read the paper
```

### Comparing `octofitterpy-2.3.3/README.md` & `octofitterpy-2.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     likelihoods=[],
     companions=[planet_b]
 )
 model = octo.LogDensityModel(sys) # Compile model
 chain = octo.octofit(model) # Sample model
 octo.octoplot(model,chain) # Plot orbits
 octo.octocorner(model,chain,small=True) # Make corner plot
-octo.savechains("table.fits", chain)
+octo.savechain("table.fits", chain)
 ```
 
 ![](examples/HIP100123-plot-grid.png)
 ![](examples/HIP100123-pairplot-small.png)
 
 
 ## Read the paper
```

### Comparing `octofitterpy-2.3.3/examples/HIP100123-pairplot-small.png` & `octofitterpy-2.3.4/examples/HIP100123-pairplot-small.png`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/examples/HIP100123-plot-grid-colorbar.png` & `octofitterpy-2.3.4/examples/HIP100123-plot-grid-colorbar.png`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/examples/HIP100123-plot-grid.png` & `octofitterpy-2.3.4/examples/HIP100123-plot-grid.png`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/examples/demo.ipynb` & `octofitterpy-2.3.4/examples/demo.ipynb`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/examples/example.py` & `octofitterpy-2.3.4/examples/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,8 +74,8 @@
 print(summary)
 
 ## Plotting
 octo.octoplot(model,chain)
 octo.octocorner(model,chain,small=True)
 
 ## Saving (use octo.loadchain to restore)
-octo.savechain(chain)
+octo.savechain("mychain.fits", chain)
```

### Comparing `octofitterpy-2.3.3/examples/gallery.png` & `octofitterpy-2.3.4/examples/gallery.png`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/octofitterpy/julia_helpers.py` & `octofitterpy-2.3.4/octofitterpy/julia_helpers.py`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/octofitterpy/julia_import.py` & `octofitterpy-2.3.4/octofitterpy/julia_import.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,25 +33,14 @@
         ("PYTHON_JULIACALL_OPTLEVEL", "3"),
     ):
         os.environ[k] = os.environ.get(k, default)
 
 
 from juliacall import Main as jl  # type: ignore
 
-# Overwrite the seval function to use Meta.parseall
-# instead of Meta.parse.
-jl.seval("using PythonCall: PythonCall, Py, pyconvert")
-jl.seval(
-    """function PythonCall.pyjlmodule_seval(self::Module, expr::Py)
-    e = Meta.parseall(strip(pyconvert(String, expr)))
-    Py(Base.eval(self, e))
-end"""
-)
-# ^TODO: Overwrite this once PythonCall.jl is updated:
-
 jl_version = (jl.VERSION.major, jl.VERSION.minor, jl.VERSION.patch)
 
 # Next, automatically load the juliacall extension if we're in a Jupyter notebook
 autoload_extensions = os.environ.get("OCTOFITTERPY_AUTOLOAD_EXTENSIONS", "yes")
 if autoload_extensions in {"yes", ""} and jl_version >= (1, 9, 0):
     try:
         get_ipython = sys.modules["IPython"].get_ipython
```

### Comparing `octofitterpy-2.3.3/octofitterpy/juliapkg.json` & `octofitterpy-2.3.4/octofitterpy/juliapkg.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.74375%*

 * *Differences: {"'julia'": "'^1.10'", "'packages'": "{'Octofitter': {'version': '=2.5.0'}}"}*

```diff
@@ -1,21 +1,21 @@
 {
-    "julia": "1.10",
+    "julia": "^1.10",
     "packages": {
         "CairoMakie": {
             "uuid": "13f3f980-e62b-5c42-98c6-ff1f3baf88f0",
             "version": "^0.11.6"
         },
         "Distributions": {
             "uuid": "31c24e10-a181-5473-b8eb-7969acd0382f",
             "version": "^0.25.107"
         },
         "Octofitter": {
             "uuid": "daf3887e-d01a-44a1-9d7e-98f15c5d69c9",
-            "version": "=2.4.0"
+            "version": "=2.5.0"
         },
         "PairPlots": {
             "uuid": "43a3c2be-4208-490b-832a-a21dcd55d7da",
             "version": "^2.6.0"
         },
         "Plots": {
             "uuid": "91a5bcdd-55d7-5caf-9e0b-520d859cae80",
```

### Comparing `octofitterpy-2.3.3/octofitterpy/python_interface.py` & `octofitterpy-2.3.4/octofitterpy/python_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 octoquick = Octofitter.octoquick
 loadchain = Octofitter.loadchain
 savechain = Octofitter.savechain
 mjd = Octofitter.mjd
 mjd2date = Octofitter.mjd2date
 years2mjd = Octofitter.mjd2date
 
+loadhdf5 = Octofitter.loadhdf5
+savehdf5 = Octofitter.savehdf5
+Whereistheplanet_astrom = Octofitter.Whereistheplanet_astrom
+
 # Expose some libraries to the user
 Distributions = jl.Distributions
 
 def Planet(
     name,
     basis,
     priors,
```

### Comparing `octofitterpy-2.3.3/octofitterpy.egg-info/PKG-INFO` & `octofitterpy-2.3.4/octofitterpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octofitterpy
-Version: 2.3.3
+Version: 2.3.4
 Summary: Fast and flexible orbit fitting
 Author-email: William Thompson <will.thompson@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 William Thompson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas<3.0.0,>=0.21.0
 Requires-Dist: numpy<2.0.0,>=1.13.0
-Requires-Dist: juliacall==0.9.15
+Requires-Dist: juliacall==0.9.19
 Requires-Dist: setuptools>=50.0.0
 
 # octofitterpy
 
 `octofitterpy` is a python package for performing Bayesian inference 
 against a wide variety of exoplanet / binary star data. It uses the [Octofitter.jl](https://sefffal.github.io/Octofitter.jl/)
 julia package under the hood (just like eg numpy uses C).
@@ -94,15 +94,15 @@
     likelihoods=[],
     companions=[planet_b]
 )
 model = octo.LogDensityModel(sys) # Compile model
 chain = octo.octofit(model) # Sample model
 octo.octoplot(model,chain) # Plot orbits
 octo.octocorner(model,chain,small=True) # Make corner plot
-octo.savechains("table.fits", chain)
+octo.savechain("table.fits", chain)
 ```
 
 ![](examples/HIP100123-plot-grid.png)
 ![](examples/HIP100123-pairplot-small.png)
 
 
 ## Read the paper
```

### Comparing `octofitterpy-2.3.3/octofitterpy.egg-info/SOURCES.txt` & `octofitterpy-2.3.4/octofitterpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octofitterpy-2.3.3/pyproject.toml` & `octofitterpy-2.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "octofitterpy"
-version = "2.3.3"
+version = "2.3.4"
 authors = [
     {name = "William Thompson", email = "will.thompson@outlook.com"},
 ]
 description = "Fast and flexible orbit fitting"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
```

### Comparing `octofitterpy-2.3.3/setup.py` & `octofitterpy-2.3.4/setup.py`

 * *Files identical despite different names*

