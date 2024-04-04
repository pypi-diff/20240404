# Comparing `tmp/causalimpactx-0.0.1.tar.gz` & `tmp/causalimpactx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalimpactx-0.0.1.tar", last modified: Mon Apr  1 16:30:44 2024, max compression
+gzip compressed data, was "causalimpactx-0.0.2.tar", last modified: Thu Apr  4 16:01:08 2024, max compression
```

## Comparing `causalimpactx-0.0.1.tar` & `causalimpactx-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-01 16:30:44.822003 causalimpactx-0.0.1/
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)       99 2024-03-31 13:45:19.000000 causalimpactx-0.0.1/AUTHORS.md
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)    10947 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/LICENSE.md
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2676 2024-04-01 16:30:44.822003 causalimpactx-0.0.1/PKG-INFO
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2001 2024-03-31 19:14:32.000000 causalimpactx-0.0.1/README.md
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)      758 2024-04-01 16:30:28.000000 causalimpactx-0.0.1/pyproject.toml
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)       38 2024-04-01 16:30:44.822003 causalimpactx-0.0.1/setup.cfg
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-01 16:30:44.814003 causalimpactx-0.0.1/src/
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-01 16:30:44.819002 causalimpactx-0.0.1/src/causalimpactx/
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)      863 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/src/causalimpactx/__init__.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)    36857 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/src/causalimpactx/analysis.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     4748 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/src/causalimpactx/inferences.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     1936 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/src/causalimpactx/misc.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     7780 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/src/causalimpactx/model.py
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-01 16:30:44.822003 causalimpactx-0.0.1/src/causalimpactx.egg-info/
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2676 2024-04-01 16:30:44.000000 causalimpactx-0.0.1/src/causalimpactx.egg-info/PKG-INFO
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)      482 2024-04-01 16:30:44.000000 causalimpactx-0.0.1/src/causalimpactx.egg-info/SOURCES.txt
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)        1 2024-04-01 16:30:44.000000 causalimpactx-0.0.1/src/causalimpactx.egg-info/dependency_links.txt
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)       28 2024-04-01 16:30:44.000000 causalimpactx-0.0.1/src/causalimpactx.egg-info/requires.txt
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)       14 2024-04-01 16:30:44.000000 causalimpactx-0.0.1/src/causalimpactx.egg-info/top_level.txt
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-01 16:30:44.821003 causalimpactx-0.0.1/tests/
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)    35198 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/tests/test_analysis.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)    10560 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/tests/test_inferences.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2540 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/tests/test_misc.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2728 2024-03-29 08:05:54.000000 causalimpactx-0.0.1/tests/test_model.py
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.767597 causalimpactx-0.0.2/
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)       99 2024-03-31 13:45:19.000000 causalimpactx-0.0.2/AUTHORS.md
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)    10947 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/LICENSE.md
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2723 2024-04-04 16:01:08.767597 causalimpactx-0.0.2/PKG-INFO
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2001 2024-03-31 19:14:32.000000 causalimpactx-0.0.2/README.md
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)      785 2024-04-04 15:59:58.000000 causalimpactx-0.0.2/pyproject.toml
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)       38 2024-04-04 16:01:08.767597 causalimpactx-0.0.2/setup.cfg
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.765597 causalimpactx-0.0.2/src/
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.765597 causalimpactx-0.0.2/src/causalimpactx/
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)      864 2024-04-02 19:50:56.000000 causalimpactx-0.0.2/src/causalimpactx/__init__.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)    37197 2024-04-03 23:52:23.000000 causalimpactx-0.0.2/src/causalimpactx/analysis.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     4870 2024-04-03 19:25:15.000000 causalimpactx-0.0.2/src/causalimpactx/inferences.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     1936 2024-04-02 19:51:47.000000 causalimpactx-0.0.2/src/causalimpactx/misc.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     7780 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/src/causalimpactx/model.py
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.766597 causalimpactx-0.0.2/src/causalimpactx.egg-info/
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2723 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/PKG-INFO
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)      482 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/SOURCES.txt
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)        1 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/dependency_links.txt
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)       45 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/requires.txt
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)       14 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/top_level.txt
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.766597 causalimpactx-0.0.2/tests/
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)    35198 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/tests/test_analysis.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)    10560 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/tests/test_inferences.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2540 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/tests/test_misc.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2728 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/tests/test_model.py
```

### Comparing `causalimpactx-0.0.1/LICENSE.md` & `causalimpactx-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.1/PKG-INFO` & `causalimpactx-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalimpactx
-Version: 0.0.1
+Version: 0.0.2
 Summary: A clone of R version CausalImpact developed by Google
 Author-email: Yaseen Esmaeelpour <yaseenes@gmail.com>
 Project-URL: Homepage, https://github.com/yaseenesmaeelpour/causalimpactx
 Project-URL: Issues, https://github.com/yaseenesmaeelpour/causalimpactx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS.md
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pytensor
+Requires-Dist: pymc
+Requires-Dist: statsmodels
 
 #### A Python package for causal inference using Bayesian structural time-series models
 
 This is a port of the R package CausalImpact, see: https://github.com/google/CausalImpact.
 
 This package implements an approach to estimating the causal effect of a designed intervention on a time series. For example, how many additional daily clicks were generated by an advertising campaign? Answering a question like this can be difficult when a randomized experiment is not available. The package aims to address this difficulty using a structural Bayesian time-series model to estimate how the response metric might have evolved after the intervention if the intervention had not occurred.
```

### Comparing `causalimpactx-0.0.1/README.md` & `causalimpactx-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.1/pyproject.toml` & `causalimpactx-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # AVOID CHANGING REQUIRES: IT WILL BE UPDATED BY PYSCAFFOLD!
 requires = ["setuptools>=46.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "causalimpactx"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Yaseen Esmaeelpour", email="yaseenes@gmail.com" },
 ]
 description = "A clone of R version CausalImpact developed by Google"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,12 +18,14 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "pandas",
   "numpy",
   "scipy",
   "pytensor",
+  "pymc",
+  "statsmodels",
 ]
 
 [project.urls]
 Homepage = "https://github.com/yaseenesmaeelpour/causalimpactx"
 Issues = "https://github.com/yaseenesmaeelpour/causalimpactx/issues"
```

### Comparing `causalimpactx-0.0.1/src/causalimpactx/__init__.py` & `causalimpactx-0.0.2/src/causalimpactx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,12 +19,12 @@
     dist_name = __name__
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
-from causalimpact.analysis import CausalImpact  # noqa
+from causalimpactx.analysis import CausalImpact  # noqa
 
 __all__ = [
     "CausalImpact",
 ]
```

### Comparing `causalimpactx-0.0.1/src/causalimpactx/analysis.py` & `causalimpactx-0.0.2/src/causalimpactx/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import textwrap
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_list_like
 
-from causalimpact.misc import standardize_all_variables, df_print, get_matplotlib
-from causalimpact.model import construct_model, model_fit
-from causalimpact.inferences import compile_inferences
+from causalimpactx.misc import standardize_all_variables, df_print, get_matplotlib
+from causalimpactx.model import construct_model, model_fit
+from causalimpactx.inferences import compile_inferences
 import scipy.stats as st
 
 
 class CausalImpact:
     """CausalImpact() performs causal inference through counterfactual
     predictions using a Bayesian structural time-series model.
 
@@ -177,19 +177,19 @@
         """
         pre_dtype = np.array(pre_period).dtype
         post_dtype = np.array(post_period).dtype
         # if index is datetime then convert pre and post to datetimes
         if isinstance(data.index, pd.core.indexes.datetimes.DatetimeIndex):
             pre_period = [pd.to_datetime(date) for date in pre_period]
             post_period = [pd.to_datetime(date) for date in post_period]
-            pd.core.dtypes.common.is_datetime_or_timedelta_dtype(pre_period)
+            pd.core.dtypes.common.is_datetime64_dtype(pre_period)
         # if index is not datetime then error if datetime pre and post is passed
-        elif pd.core.dtypes.common.is_datetime_or_timedelta_dtype(
+        elif pd.core.dtypes.common.is_datetime64_dtype(
             pd.Series(pre_period)
-        ) or pd.core.dtypes.common.is_datetime_or_timedelta_dtype(
+        ) or pd.core.dtypes.common.is_datetime64_dtype(
             pd.Series(post_period)
         ):
             raise ValueError(
                 "pre_period ("
                 + pre_dtype.name
                 + ") and post_period ("
                 + post_dtype.name
@@ -704,14 +704,20 @@
         print("\n")
         print(textwrap.fill(stmt3, width=width))
         print("\n")
         print(textwrap.fill(stmt4, width=width))
         print("\n")
         print(textwrap.fill(stmt5, width=width))
 
+    def format_number(self, value):
+        if isinstance(value, float):
+            return "{:.2f}".format(value)
+        else:
+            return int(value)
+
     def summary(self, output="summary", width=120, path=None):
         """reports a summary of the results
 
         Parameters
         ----------
         output: str
             can be summary or report. summary outputs a table.
@@ -729,45 +735,45 @@
         post_inf = self.inferences.loc[post_period[0] : post_period[1], :]
         post_point_resp = post_inf.loc[:, "response"]
         post_point_pred = post_inf.loc[:, "point_pred"]
         post_point_upper = post_inf.loc[:, "point_pred_upper"]
         post_point_lower = post_inf.loc[:, "point_pred_lower"]
 
         mean_resp = post_point_resp.mean()
-        mean_resp_fmt = int(mean_resp)
+        mean_resp_fmt = self.format_number(mean_resp)
         cum_resp = post_point_resp.sum()
-        cum_resp_fmt = int(cum_resp)
+        cum_resp_fmt = self.format_number(cum_resp)
         mean_pred = post_point_pred.mean()
-        mean_pred_fmt = int(post_point_pred.mean())
+        mean_pred_fmt = self.format_number(post_point_pred.mean())
         cum_pred = post_point_pred.sum()
-        cum_pred_fmt = int(cum_pred)
+        cum_pred_fmt = self.format_number(cum_pred)
         mean_lower = post_point_lower.mean()
-        mean_lower_fmt = int(mean_lower)
+        mean_lower_fmt = self.format_number(mean_lower)
         mean_upper = post_point_upper.mean()
-        mean_upper_fmt = int(mean_upper)
+        mean_upper_fmt = self.format_number(mean_upper)
         mean_ci_fmt = [mean_lower_fmt, mean_upper_fmt]
         cum_lower = post_point_lower.sum()
-        cum_lower_fmt = int(cum_lower)
+        cum_lower_fmt = self.format_number(cum_lower)
         cum_upper = post_point_upper.sum()
-        cum_upper_fmt = int(cum_upper)
+        cum_upper_fmt = self.format_number(cum_upper)
         cum_ci_fmt = [cum_lower_fmt, cum_upper_fmt]
 
         abs_effect = (post_point_resp - post_point_pred).mean()
-        abs_effect_fmt = int(abs_effect)
+        abs_effect_fmt = self.format_number(abs_effect)
         cum_abs_effect = (post_point_resp - post_point_pred).sum()
-        cum_abs_effect_fmt = int(cum_abs_effect)
+        cum_abs_effect_fmt = self.format_number(cum_abs_effect)
         abs_effect_lower = (post_point_resp - post_point_lower).mean()
-        abs_effect_lower_fmt = int(abs_effect_lower)
+        abs_effect_lower_fmt = self.format_number(abs_effect_lower)
         abs_effect_upper = (post_point_resp - post_point_upper).mean()
-        abs_effect_upper_fmt = int(abs_effect_upper)
+        abs_effect_upper_fmt = self.format_number(abs_effect_upper)
         abs_effect_ci_fmt = [abs_effect_lower_fmt, abs_effect_upper_fmt]
         cum_abs_lower = (post_point_resp - post_point_lower).sum()
-        cum_abs_lower_fmt = int(cum_abs_lower)
+        cum_abs_lower_fmt = self.format_number(cum_abs_lower)
         cum_abs_upper = (post_point_resp - post_point_upper).sum()
-        cum_abs_upper_fmt = int(cum_abs_upper)
+        cum_abs_upper_fmt = self.format_number(cum_abs_upper)
         cum_abs_effect_ci_fmt = [cum_abs_lower_fmt, cum_abs_upper_fmt]
 
         rel_effect = abs_effect / mean_pred * 100
         rel_effect_fmt = "{:.1f}%".format(rel_effect)
         cum_rel_effect = cum_abs_effect / cum_pred * 100
         cum_rel_effect_fmt = "{:.1f}%".format(cum_rel_effect)
         rel_effect_lower = abs_effect_lower / mean_pred * 100
```

### Comparing `causalimpactx-0.0.1/src/causalimpactx/inferences.py` & `causalimpactx-0.0.2/src/causalimpactx/inferences.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-from causalimpact.misc import unstandardize
+from causalimpactx.misc import unstandardize
 
 
 def compile_inferences(
     results,
     data,
     df_pre,
     df_post,
@@ -64,14 +64,18 @@
     post_ci = unstandardize(forecast.conf_int(alpha=alpha), orig_std_params)
 
     post_ci.index = df_post.index
     ci = pd.concat([pre_ci, post_ci])
     point_pred_lower = ci.iloc[:, 0].to_frame()
     point_pred_upper = ci.iloc[:, 1].to_frame()
 
+    #set first element to zero to avoid plot skew
+    point_pred_lower.iloc[0,0] = 0
+    point_pred_upper.iloc[0,0] = 0
+
     response = data.iloc[:, 0]
     response_index = data.index
 
     response = pd.DataFrame(response)
 
     cum_response = np.cumsum(response)
     cum_pred = np.cumsum(point_pred)
```

### Comparing `causalimpactx-0.0.1/src/causalimpactx/misc.py` & `causalimpactx-0.0.2/src/causalimpactx/misc.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.1/src/causalimpactx/model.py` & `causalimpactx-0.0.2/src/causalimpactx/model.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.1/src/causalimpactx.egg-info/PKG-INFO` & `causalimpactx-0.0.2/src/causalimpactx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalimpactx
-Version: 0.0.1
+Version: 0.0.2
 Summary: A clone of R version CausalImpact developed by Google
 Author-email: Yaseen Esmaeelpour <yaseenes@gmail.com>
 Project-URL: Homepage, https://github.com/yaseenesmaeelpour/causalimpactx
 Project-URL: Issues, https://github.com/yaseenesmaeelpour/causalimpactx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS.md
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pytensor
+Requires-Dist: pymc
+Requires-Dist: statsmodels
 
 #### A Python package for causal inference using Bayesian structural time-series models
 
 This is a port of the R package CausalImpact, see: https://github.com/google/CausalImpact.
 
 This package implements an approach to estimating the causal effect of a designed intervention on a time series. For example, how many additional daily clicks were generated by an advertising campaign? Answering a question like this can be difficult when a randomized experiment is not available. The package aims to address this difficulty using a structural Bayesian time-series model to estimate how the response metric might have evolved after the intervention if the intervention had not occurred.
```

### Comparing `causalimpactx-0.0.1/tests/test_analysis.py` & `causalimpactx-0.0.2/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.1/tests/test_inferences.py` & `causalimpactx-0.0.2/tests/test_inferences.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.1/tests/test_misc.py` & `causalimpactx-0.0.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.1/tests/test_model.py` & `causalimpactx-0.0.2/tests/test_model.py`

 * *Files identical despite different names*

