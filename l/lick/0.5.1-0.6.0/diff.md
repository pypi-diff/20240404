# Comparing `tmp/lick-0.5.1.tar.gz` & `tmp/lick-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lick-0.5.1.tar", last modified: Sat Mar 30 16:49:30 2024, max compression
+gzip compressed data, was "lick-0.6.0.tar", last modified: Thu Apr  4 14:50:32 2024, max compression
```

## Comparing `lick-0.5.1.tar` & `lick-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:49:30.208280 lick-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-30 16:49:22.000000 lick-0.5.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-30 16:49:22.000000 lick-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-30 16:49:22.000000 lick-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-03-30 16:49:30.208280 lick-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-30 16:49:22.000000 lick-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-30 16:49:22.000000 lick-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 16:49:30.208280 lick-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-30 16:49:22.000000 lick-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:49:30.204280 lick-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:49:30.208280 lick-0.5.1/src/lick/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-30 16:49:22.000000 lick-0.5.1/src/lick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 16:49:22.000000 lick-0.5.1/src/lick/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:49:30.204280 lick-0.5.1/src/lick/_vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:49:30.208280 lick-0.5.1/src/lick/_vendor/vectorplot/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-30 16:49:22.000000 lick-0.5.1/src/lick/_vendor/vectorplot/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-03-30 16:49:22.000000 lick-0.5.1/src/lick/_vendor/vectorplot/core.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-03-30 16:49:22.000000 lick-0.5.1/src/lick/lick.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 16:49:22.000000 lick-0.5.1/src/lick/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 16:49:30.208280 lick-0.5.1/src/lick.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-03-30 16:49:30.000000 lick-0.5.1/src/lick.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-30 16:49:30.000000 lick-0.5.1/src/lick.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 16:49:30.000000 lick-0.5.1/src/lick.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-30 16:49:30.000000 lick-0.5.1/src/lick.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-30 16:49:30.000000 lick-0.5.1/src/lick.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-30 16:49:30.000000 lick-0.5.1/src/lick.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:32.921919 lick-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 14:50:25.000000 lick-0.6.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 14:50:25.000000 lick-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 14:50:25.000000 lick-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-04 14:50:32.921919 lick-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-04 14:50:25.000000 lick-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-04 14:50:25.000000 lick-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:50:32.921919 lick-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-04 14:50:25.000000 lick-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:32.917919 lick-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:32.917919 lick-0.6.0/src/lick/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 14:50:25.000000 lick-0.6.0/src/lick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:50:25.000000 lick-0.6.0/src/lick/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:32.917919 lick-0.6.0/src/lick/_vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:32.917919 lick-0.6.0/src/lick/_vendor/vectorplot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-04 14:50:25.000000 lick-0.6.0/src/lick/_vendor/vectorplot/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-04 14:50:25.000000 lick-0.6.0/src/lick/_vendor/vectorplot/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-04 14:50:25.000000 lick-0.6.0/src/lick/lick.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:25.000000 lick-0.6.0/src/lick/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:32.917919 lick-0.6.0/src/lick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-04 14:50:32.000000 lick-0.6.0/src/lick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-04 14:50:32.000000 lick-0.6.0/src/lick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:50:32.000000 lick-0.6.0/src/lick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 14:50:32.000000 lick-0.6.0/src/lick.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 14:50:32.000000 lick-0.6.0/src/lick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 14:50:32.000000 lick-0.6.0/src/lick.egg-info/top_level.txt
```

### Comparing `lick-0.5.1/LICENSE` & `lick-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lick-0.5.1/PKG-INFO` & `lick-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: lick
-Version: 0.5.1
+Version: 0.6.0
 Summary: Package that uses a Line Integral Convolution library to clothe a 2D field (ex: density field) with a LIC texture, given two vector fields (ex: velocity (vx, vy))
 Author: G. Wafflard-Fernandez, C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/volodia99/lick
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.4.0
 Requires-Dist: numpy<3,>=1.19.3
-Requires-Dist: scikit-image>=0.18.1
 Requires-Dist: scipy>=1.5.4
 Requires-Dist: packaging>=20.9
 
 # lick
 [![PyPI](https://img.shields.io/pypi/v/lick.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/lick/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/volodia99/lick/main.svg)](https://results.pre-commit.ci/latest/github/volodia99/lick/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `lick-0.5.1/README.md` & `lick-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lick-0.5.1/pyproject.toml` & `lick-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "Cython>=3.0",
     "numpy>=2.0.0rc1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lick"
-version = "0.5.1"
+version = "0.6.0"
 description = "Package that uses a Line Integral Convolution library to clothe a 2D field (ex: density field) with a LIC texture, given two vector fields (ex: velocity (vx, vy))"
 authors = [
     { name = "G. Wafflard-Fernandez" },
 	{ name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -20,15 +20,14 @@
     "Typing :: Typed",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "matplotlib>=3.4.0",
     # keep in sync with NPY_TARGET_VERSION (setup.py)
     "numpy>=1.19.3, <3",
-    "scikit-image>=0.18.1",
     "scipy>=1.5.4",
     "packaging>=20.9",
 ]
 
 [project.license]
 text = "GPL-3.0"
 
@@ -58,15 +57,15 @@
 
 [tool.ruff.lint.isort]
 combine-as-imports = true
 known-first-party = ["lick"]
 
 [tool.mypy]
 python_version = "3.9"
-ignore_missing_imports = true # matplotlib and skimage don't have stubs yet
+ignore_missing_imports = true # mpl_toolkits doesn't have stubs yet
 show_error_codes = true
 pretty = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unreachable = true
 
 [tool.pytest.ini_options]
```

### Comparing `lick-0.5.1/setup.py` & `lick-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `lick-0.5.1/src/lick/_vendor/vectorplot/LICENSE.txt` & `lick-0.6.0/src/lick/_vendor/vectorplot/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lick-0.5.1/src/lick/_vendor/vectorplot/core.pyx` & `lick-0.6.0/src/lick/_vendor/vectorplot/core.pyx`

 * *Files identical despite different names*

### Comparing `lick-0.5.1/src/lick/lick.py` & `lick-0.6.0/src/lick/lick.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,57 @@
 #!/usr/bin/env python
-from importlib.metadata import version
-from typing import Optional
+import warnings
+from typing import TYPE_CHECKING, Optional
 
 import numpy as np
-from packaging.version import Version
 
 import lick._vendor.vectorplot.core as _lic
 
+if TYPE_CHECKING:
+    from matplotlib.axes import Axes
+    from matplotlib.figure import Figure
+
+
+def _equalize_hist(image):
+    # adapted from scikit-image
+    """Return image after histogram equalization.
+
+    Parameters
+    ----------
+    image : array
+        Image array.
+
+    Returns
+    -------
+    out : float array
+        Image array after histogram equalization.
+
+    Notes
+    -----
+    This function is adapted from [1]_ with the author's permission.
+
+    References
+    ----------
+    .. [1] http://www.janeriksolem.net/histogram-equalization-with-python-and.html
+    .. [2] https://en.wikipedia.org/wiki/Histogram_equalization
+
+    """
+    hist, bin_edges = np.histogram(image.flatten(), bins=256, range=None)
+    bin_centers = (bin_edges[:-1] + bin_edges[1:]) / 2.0
+
+    cdf = hist.cumsum()
+    cdf = cdf / float(cdf[-1])
+
+    cdf = cdf.astype(image.dtype, copy=False)
+    out = np.interp(image.flat, bin_centers, cdf)
+    out = out.reshape(image.shape)
+    # Unfortunately, np.interp currently always promotes to float64, so we
+    # have to cast back to single precision when float32 output is desired
+    return out.astype(image.dtype, copy=False)
+
 
 def interpol(
     xx,
     yy,
     v1: np.ndarray,
     v2: np.ndarray,
     field: np.ndarray,
@@ -65,46 +106,31 @@
     v1: np.ndarray,
     v2: np.ndarray,
     *,
     niter_lic: int = 5,
     kernel_length: int = 101,
     light_source: bool = True,
 ):
-    from skimage import exposure
-    from skimage.util import random_noise
-
     if v1.ndim != 2:
         raise ValueError(f"Expected a 2D array for v1, got v1 with shape {v1.shape}")
     if v2.ndim != 2:
         raise ValueError(f"Expected a 2D array for v2, got v2 with shape {v2.shape}")
 
-    if Version(version("scikit-image")) >= Version("0.21.0"):
-        # avoid deprecated API as soon as the new one is available
-        kwargs = {"rng": 0}
-    else:
-        # backward compatibility branch
-        kwargs = {"seed": 0}
-
-    texture = random_noise(
-        np.zeros_like(v1),
-        mode="gaussian",
-        mean=0.5,
-        var=0.001,
-        **kwargs,
-    ).astype(v1.dtype)
+    rng = np.random.default_rng(seed=0)
+    texture = rng.normal(0.5, 0.001**0.5, v1.shape).astype(v1.dtype, copy=False)
     kernel = np.sin(np.arange(kernel_length, dtype=v1.dtype) * np.pi / kernel_length)
 
     out = np.empty_like(v1)
     image = texture
     for _ in range(niter_lic):
         out[:, :] = 0.0
         _lic.line_integral_convolution(v1, v2, image, kernel, out=out)
         image[:, :] = out[:, :]
 
-    image = exposure.equalize_hist(image)
+    image = _equalize_hist(image)
     image /= image.max()
 
     if light_source:
         from matplotlib.colors import LightSource
 
         # Illuminate the scene from the northwest
         ls = LightSource(azdeg=0, altdeg=45)
@@ -164,16 +190,16 @@
         kernel_length=kernel_length,
         light_source=light_source,
     )
     return (Xi, Yi, v1i, v2i, fieldi, licv)
 
 
 def lick_box_plot(
-    fig,
-    ax,
+    fig: "Figure",
+    ax: "Axes",
     x: np.ndarray,
     y: np.ndarray,
     v1: np.ndarray,
     v2: np.ndarray,
     field: np.ndarray,
     *,
     vmin: Optional[float] = None,
@@ -195,14 +221,21 @@
     light_source: bool = True,
     stream_density: float = 0,
     alpha_transparency: bool = True,
     alpha: float = 0.3,
 ):
     from mpl_toolkits.axes_grid1 import make_axes_locatable
 
+    if nbin is not None:
+        warnings.warn(
+            "the nbin keyword argument has no effect "
+            "and will be removed in a future version",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
     Xi, Yi, v1i, v2i, fieldi, licv = lick_box(
         x,
         y,
         v1,
         v2,
         field,
         size_interpolated=size_interpolated,
```

### Comparing `lick-0.5.1/src/lick.egg-info/PKG-INFO` & `lick-0.6.0/src/lick.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: lick
-Version: 0.5.1
+Version: 0.6.0
 Summary: Package that uses a Line Integral Convolution library to clothe a 2D field (ex: density field) with a LIC texture, given two vector fields (ex: velocity (vx, vy))
 Author: G. Wafflard-Fernandez, C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/volodia99/lick
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.4.0
 Requires-Dist: numpy<3,>=1.19.3
-Requires-Dist: scikit-image>=0.18.1
 Requires-Dist: scipy>=1.5.4
 Requires-Dist: packaging>=20.9
 
 # lick
 [![PyPI](https://img.shields.io/pypi/v/lick.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/lick/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/volodia99/lick/main.svg)](https://results.pre-commit.ci/latest/github/volodia99/lick/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

