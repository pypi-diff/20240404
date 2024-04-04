# Comparing `tmp/baal-1.9.1.tar.gz` & `tmp/baal-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baal-1.9.1.tar", max compression
+gzip compressed data, was "baal-1.9.2.tar", max compression
```

## Comparing `baal-1.9.1.tar` & `baal-1.9.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2022-07-09 19:42:29.730723 baal-1.9.1/LICENSE
--rw-r--r--   0        0        0     7569 2023-09-08 20:09:16.719534 baal-1.9.1/README.md
--rw-r--r--   0        0        0      165 2022-07-09 19:42:29.730723 baal-1.9.1/baal/__init__.py
--rw-r--r--   0        0        0     1162 2022-07-09 19:42:29.730723 baal-1.9.1/baal/active/__init__.py
--rw-r--r--   0        0        0     3981 2023-09-15 21:54:53.718207 baal-1.9.1/baal/active/active_loop.py
--rw-r--r--   0        0        0      147 2022-07-09 19:42:29.730723 baal-1.9.1/baal/active/dataset/__init__.py
--rw-r--r--   0        0        0     4931 2023-07-13 22:01:48.579265 baal-1.9.1/baal/active/dataset/base.py
--rw-r--r--   0        0        0     3715 2022-08-20 15:06:46.551908 baal-1.9.1/baal/active/dataset/nlp_datasets.py
--rw-r--r--   0        0        0     2713 2023-07-13 22:01:48.579265 baal-1.9.1/baal/active/dataset/numpy.py
--rw-r--r--   0        0        0     9423 2022-10-28 21:52:52.696293 baal-1.9.1/baal/active/dataset/pytorch_dataset.py
--rw-r--r--   0        0        0     3043 2022-07-09 19:42:29.730723 baal-1.9.1/baal/active/file_dataset.py
--rw-r--r--   0        0        0       26 2022-07-09 19:42:29.730723 baal-1.9.1/baal/active/heuristics/__init__.py
--rw-r--r--   0        0        0      633 2023-10-02 19:43:24.245767 baal-1.9.1/baal/active/heuristics/aliases.py
--rw-r--r--   0        0        0    24150 2023-07-28 21:24:51.005921 baal-1.9.1/baal/active/heuristics/heuristics.py
--rw-r--r--   0        0        0     4532 2022-08-20 15:06:46.551908 baal-1.9.1/baal/active/heuristics/heuristics_gpu.py
--rw-r--r--   0        0        0     5698 2022-07-09 19:42:29.730723 baal-1.9.1/baal/active/heuristics/stochastics.py
--rw-r--r--   0        0        0      127 2022-07-09 19:42:29.730723 baal-1.9.1/baal/bayesian/__init__.py
--rw-r--r--   0        0        0     1753 2023-07-13 22:01:48.579265 baal-1.9.1/baal/bayesian/caching_utils.py
--rw-r--r--   0        0        0     1880 2023-03-04 15:23:50.812969 baal-1.9.1/baal/bayesian/common.py
--rw-r--r--   0        0        0     5332 2022-07-09 19:42:29.730723 baal-1.9.1/baal/bayesian/consistent_dropout.py
--rw-r--r--   0        0        0     5418 2022-07-09 19:42:29.730723 baal-1.9.1/baal/bayesian/dropout.py
--rw-r--r--   0        0        0     5914 2022-07-09 19:42:29.734723 baal-1.9.1/baal/bayesian/weight_drop.py
--rw-r--r--   0        0        0       45 2022-07-09 19:42:29.734723 baal-1.9.1/baal/calibration/__init__.py
--rw-r--r--   0        0        0     5056 2022-08-20 15:06:46.551908 baal-1.9.1/baal/calibration/calibration.py
--rw-r--r--   0        0        0     2469 2022-07-09 19:42:29.734723 baal-1.9.1/baal/ensemble.py
--rw-r--r--   0        0        0        0 2022-08-21 16:32:48.317380 baal-1.9.1/baal/metrics/__init__.py
--rw-r--r--   0        0        0     3108 2022-10-28 21:52:52.696293 baal-1.9.1/baal/metrics/mixin.py
--rw-r--r--   0        0        0    17144 2023-09-15 21:54:53.722207 baal-1.9.1/baal/modelwrapper.py
--rw-r--r--   0        0        0     4995 2023-09-08 20:09:16.719534 baal-1.9.1/baal/transformers_trainer_wrapper.py
--rw-r--r--   0        0        0      760 2022-07-09 19:42:29.734723 baal-1.9.1/baal/utils/__init__.py
--rw-r--r--   0        0        0     1569 2022-07-09 19:42:29.734723 baal-1.9.1/baal/utils/array_utils.py
--rw-r--r--   0        0        0     2098 2022-07-09 19:42:29.734723 baal-1.9.1/baal/utils/cuda_utils.py
--rw-r--r--   0        0        0      674 2022-10-28 21:52:52.696293 baal-1.9.1/baal/utils/equality.py
--rw-r--r--   0        0        0      360 2023-09-08 20:09:16.719534 baal-1.9.1/baal/utils/iterutils.py
--rw-r--r--   0        0        0     3371 2022-07-09 19:42:29.734723 baal-1.9.1/baal/utils/log_configuration.py
--rw-r--r--   0        0        0    16693 2022-07-09 19:42:29.734723 baal-1.9.1/baal/utils/metrics.py
--rw-r--r--   0        0        0     3029 2022-07-09 19:42:29.734723 baal-1.9.1/baal/utils/plot_utils.py
--rw-r--r--   0        0        0     7839 2023-05-16 01:02:37.489674 baal-1.9.1/baal/utils/pytorch_lightning.py
--rw-r--r--   0        0        0     5903 2022-07-09 19:42:29.734723 baal-1.9.1/baal/utils/ssl_iterator.py
--rw-r--r--   0        0        0     2532 2022-08-20 15:06:46.551908 baal-1.9.1/baal/utils/ssl_module.py
--rw-r--r--   0        0        0     2579 2022-07-09 19:42:29.734723 baal-1.9.1/baal/utils/transforms.py
--rw-r--r--   0        0        0      529 2023-09-15 21:54:53.722207 baal-1.9.1/baal/utils/warnings.py
--rw-r--r--   0        0        0     1753 2023-10-02 19:46:51.880951 baal-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     9008 1970-01-01 00:00:00.000000 baal-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-09 19:42:29.730723 baal-1.9.2/LICENSE
+-rw-r--r--   0        0        0     7569 2023-09-08 20:09:16.719534 baal-1.9.2/README.md
+-rw-r--r--   0        0        0      165 2022-07-09 19:42:29.730723 baal-1.9.2/baal/__init__.py
+-rw-r--r--   0        0        0     1162 2022-07-09 19:42:29.730723 baal-1.9.2/baal/active/__init__.py
+-rw-r--r--   0        0        0     3981 2023-09-15 21:54:53.718207 baal-1.9.2/baal/active/active_loop.py
+-rw-r--r--   0        0        0      147 2022-07-09 19:42:29.730723 baal-1.9.2/baal/active/dataset/__init__.py
+-rw-r--r--   0        0        0     4931 2023-07-13 22:01:48.579265 baal-1.9.2/baal/active/dataset/base.py
+-rw-r--r--   0        0        0     3715 2022-08-20 15:06:46.551908 baal-1.9.2/baal/active/dataset/nlp_datasets.py
+-rw-r--r--   0        0        0     2713 2023-07-13 22:01:48.579265 baal-1.9.2/baal/active/dataset/numpy.py
+-rw-r--r--   0        0        0     9423 2022-10-28 21:52:52.696293 baal-1.9.2/baal/active/dataset/pytorch_dataset.py
+-rw-r--r--   0        0        0     3043 2022-07-09 19:42:29.730723 baal-1.9.2/baal/active/file_dataset.py
+-rw-r--r--   0        0        0       26 2022-07-09 19:42:29.730723 baal-1.9.2/baal/active/heuristics/__init__.py
+-rw-r--r--   0        0        0      633 2023-10-02 19:43:24.245767 baal-1.9.2/baal/active/heuristics/aliases.py
+-rw-r--r--   0        0        0    24150 2023-07-28 21:24:51.005921 baal-1.9.2/baal/active/heuristics/heuristics.py
+-rw-r--r--   0        0        0     4532 2022-08-20 15:06:46.551908 baal-1.9.2/baal/active/heuristics/heuristics_gpu.py
+-rw-r--r--   0        0        0     5694 2024-04-04 17:28:50.986222 baal-1.9.2/baal/active/heuristics/stochastics.py
+-rw-r--r--   0        0        0      127 2022-07-09 19:42:29.730723 baal-1.9.2/baal/bayesian/__init__.py
+-rw-r--r--   0        0        0     1753 2023-07-13 22:01:48.579265 baal-1.9.2/baal/bayesian/caching_utils.py
+-rw-r--r--   0        0        0     1880 2023-03-04 15:23:50.812969 baal-1.9.2/baal/bayesian/common.py
+-rw-r--r--   0        0        0     5332 2022-07-09 19:42:29.730723 baal-1.9.2/baal/bayesian/consistent_dropout.py
+-rw-r--r--   0        0        0     5418 2022-07-09 19:42:29.730723 baal-1.9.2/baal/bayesian/dropout.py
+-rw-r--r--   0        0        0     5914 2022-07-09 19:42:29.734723 baal-1.9.2/baal/bayesian/weight_drop.py
+-rw-r--r--   0        0        0       45 2022-07-09 19:42:29.734723 baal-1.9.2/baal/calibration/__init__.py
+-rw-r--r--   0        0        0     5056 2022-08-20 15:06:46.551908 baal-1.9.2/baal/calibration/calibration.py
+-rw-r--r--   0        0        0     2469 2022-07-09 19:42:29.734723 baal-1.9.2/baal/ensemble.py
+-rw-r--r--   0        0        0        0 2022-08-21 16:32:48.317380 baal-1.9.2/baal/metrics/__init__.py
+-rw-r--r--   0        0        0     3108 2022-10-28 21:52:52.696293 baal-1.9.2/baal/metrics/mixin.py
+-rw-r--r--   0        0        0    17144 2023-09-15 21:54:53.722207 baal-1.9.2/baal/modelwrapper.py
+-rw-r--r--   0        0        0     7113 2024-01-14 15:59:17.125594 baal-1.9.2/baal/transformers_trainer_wrapper.py
+-rw-r--r--   0        0        0      760 2022-07-09 19:42:29.734723 baal-1.9.2/baal/utils/__init__.py
+-rw-r--r--   0        0        0     1569 2022-07-09 19:42:29.734723 baal-1.9.2/baal/utils/array_utils.py
+-rw-r--r--   0        0        0     2098 2022-07-09 19:42:29.734723 baal-1.9.2/baal/utils/cuda_utils.py
+-rw-r--r--   0        0        0      674 2022-10-28 21:52:52.696293 baal-1.9.2/baal/utils/equality.py
+-rw-r--r--   0        0        0      360 2023-09-08 20:09:16.719534 baal-1.9.2/baal/utils/iterutils.py
+-rw-r--r--   0        0        0     3371 2022-07-09 19:42:29.734723 baal-1.9.2/baal/utils/log_configuration.py
+-rw-r--r--   0        0        0    16693 2022-07-09 19:42:29.734723 baal-1.9.2/baal/utils/metrics.py
+-rw-r--r--   0        0        0     3029 2022-07-09 19:42:29.734723 baal-1.9.2/baal/utils/plot_utils.py
+-rw-r--r--   0        0        0     7839 2023-05-16 01:02:37.489674 baal-1.9.2/baal/utils/pytorch_lightning.py
+-rw-r--r--   0        0        0     5903 2022-07-09 19:42:29.734723 baal-1.9.2/baal/utils/ssl_iterator.py
+-rw-r--r--   0        0        0     2532 2022-08-20 15:06:46.551908 baal-1.9.2/baal/utils/ssl_module.py
+-rw-r--r--   0        0        0     2579 2022-07-09 19:42:29.734723 baal-1.9.2/baal/utils/transforms.py
+-rw-r--r--   0        0        0      529 2023-09-15 21:54:53.722207 baal-1.9.2/baal/utils/warnings.py
+-rw-r--r--   0        0        0     1817 2024-04-04 17:28:50.990222 baal-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     9070 1970-01-01 00:00:00.000000 baal-1.9.2/PKG-INFO
```

### Comparing `baal-1.9.1/LICENSE` & `baal-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/README.md` & `baal-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/__init__.py` & `baal-1.9.2/baal/active/__init__.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/active_loop.py` & `baal-1.9.2/baal/active/active_loop.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/dataset/base.py` & `baal-1.9.2/baal/active/dataset/base.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/dataset/nlp_datasets.py` & `baal-1.9.2/baal/active/dataset/nlp_datasets.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/dataset/numpy.py` & `baal-1.9.2/baal/active/dataset/numpy.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/dataset/pytorch_dataset.py` & `baal-1.9.2/baal/active/dataset/pytorch_dataset.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/file_dataset.py` & `baal-1.9.2/baal/active/file_dataset.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/heuristics/aliases.py` & `baal-1.9.2/baal/active/heuristics/aliases.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/heuristics/heuristics.py` & `baal-1.9.2/baal/active/heuristics/heuristics.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/heuristics/heuristics_gpu.py` & `baal-1.9.2/baal/active/heuristics/heuristics_gpu.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/active/heuristics/stochastics.py` & `baal-1.9.2/baal/active/heuristics/stochastics.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         distributions = self._make_distribution(scores)
         # Force normalization for np.random.choice
         distributions = np.clip(distributions, 0, None)
         distributions /= distributions.sum()
 
         # TODO Seed?
         if (distributions > 0).sum() < self.query_size:
-            log.warnings("Not enough values, return random")
+            log.warn("Not enough values, return random")
             distributions = np.ones_like(distributions) / len(distributions)
         return (
             np.random.choice(len(distributions), self.query_size, replace=False, p=distributions),
             distributions,
         )
 
     def get_scores(self, predictions):
```

### Comparing `baal-1.9.1/baal/bayesian/caching_utils.py` & `baal-1.9.2/baal/bayesian/caching_utils.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/bayesian/common.py` & `baal-1.9.2/baal/bayesian/common.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/bayesian/consistent_dropout.py` & `baal-1.9.2/baal/bayesian/consistent_dropout.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/bayesian/dropout.py` & `baal-1.9.2/baal/bayesian/dropout.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/bayesian/weight_drop.py` & `baal-1.9.2/baal/bayesian/weight_drop.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/calibration/calibration.py` & `baal-1.9.2/baal/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/ensemble.py` & `baal-1.9.2/baal/ensemble.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/metrics/mixin.py` & `baal-1.9.2/baal/metrics/mixin.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/modelwrapper.py` & `baal-1.9.2/baal/modelwrapper.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/__init__.py` & `baal-1.9.2/baal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/array_utils.py` & `baal-1.9.2/baal/utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/cuda_utils.py` & `baal-1.9.2/baal/utils/cuda_utils.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/equality.py` & `baal-1.9.2/baal/utils/equality.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/log_configuration.py` & `baal-1.9.2/baal/utils/log_configuration.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/metrics.py` & `baal-1.9.2/baal/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/plot_utils.py` & `baal-1.9.2/baal/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/pytorch_lightning.py` & `baal-1.9.2/baal/utils/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/ssl_iterator.py` & `baal-1.9.2/baal/utils/ssl_iterator.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/ssl_module.py` & `baal-1.9.2/baal/utils/ssl_module.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/transforms.py` & `baal-1.9.2/baal/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/baal/utils/warnings.py` & `baal-1.9.2/baal/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `baal-1.9.1/pyproject.toml` & `baal-1.9.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baal"
-version = "1.9.1"
+version = "1.9.2"
 description = "Library to enable Bayesian active learning in your research or labeling work."
 authors = ["Parmida Atighehchian <parmida.atighehchian@servicenow.com>",
            "Frederic Branchaud-Charron <frederic.branchaud-charron@servicenow.com>",
            "Jan Freyberg <jan.freyberg@gmail.com>",
            "Lorne Schell <lorne.schell@servicenow.com>",
            "Rafael Pardina <rafael.pardinas@servicenow.com>"
            ]
@@ -18,24 +18,25 @@
 torch = ">=1.6.0"
 torchmetrics = "^0.9.3"
 h5py = "^3.4.0"
 numpy = "^1.21.2"
 matplotlib = "^3.4.3"
 Pillow = ">=6.2.0"
 tqdm = "^4.62.2"
-structlog = "^21.1.0"
+structlog = "^22.0.0"
 scikit-learn = "^1.0.0"
 scipy = "^1.7.1"
 
 # Vision
 torchvision = { version = ">=0.7.0", optional=true }
 lightning-flash = { version = ">=0.7.5", optional=true }
 
 # NLP
 transformers = {version = ">=4.10.2", optional=true}
+accelerate = {version = "^0.28.0", optional=true}
 datasets = {version = ">=1.11.0", optional=true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^2.12.1"
 torch-hypothesis = "0.2.0"
 hypothesis = "4.24.0"
@@ -53,15 +54,15 @@
 mkdocs-material = "^8.5.6"
 Pygments = "^2.12.0"
 mkdocstrings = {extras = ["python"], version = "^0.18.1"}
 mkdocs-exclude-search = "^0.6.4"
 
 [tool.poetry.extras]
 vision = ["torchvision", "lightning-flash"]
-nlp = ["transformers", "datasets"]
+nlp = ["transformers", "datasets", "accelerate"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
```

### Comparing `baal-1.9.1/PKG-INFO` & `baal-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baal
-Version: 1.9.1
+Version: 1.9.2
 Summary: Library to enable Bayesian active learning in your research or labeling work.
 Home-page: https://github.com/ElementAI/baal/
 License: Apache-2.0
 Author: Parmida Atighehchian
 Author-email: parmida.atighehchian@servicenow.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,22 +12,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: nlp
 Provides-Extra: vision
 Requires-Dist: Pillow (>=6.2.0)
+Requires-Dist: accelerate (>=0.28.0,<0.29.0) ; extra == "nlp"
 Requires-Dist: datasets (>=1.11.0) ; extra == "nlp"
 Requires-Dist: h5py (>=3.4.0,<4.0.0)
 Requires-Dist: lightning-flash (>=0.7.5) ; extra == "vision"
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.0,<2.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
-Requires-Dist: structlog (>=21.1.0,<22.0.0)
+Requires-Dist: structlog (>=22.0.0,<23.0.0)
 Requires-Dist: torch (>=1.6.0)
 Requires-Dist: torchmetrics (>=0.9.3,<0.10.0)
 Requires-Dist: torchvision (>=0.7.0) ; extra == "vision"
 Requires-Dist: tqdm (>=4.62.2,<5.0.0)
 Requires-Dist: transformers (>=4.10.2) ; extra == "nlp"
 Project-URL: Documentation, https://baal.readthedocs.io
 Project-URL: Repository, https://github.com/ElementAI/baal/
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: baal Version: 1.9.1 Summary: Library to enable
+Metadata-Version: 2.1 Name: baal Version: 1.9.2 Summary: Library to enable
 Bayesian active learning in your research or labeling work. Home-page: https://
 github.com/ElementAI/baal/ License: Apache-2.0 Author: Parmida Atighehchian
 Author-email: parmida.atighehchian@servicenow.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Provides-Extra: nlp Provides-Extra: vision Requires-Dist: Pillow
-(>=6.2.0) Requires-Dist: datasets (>=1.11.0) ; extra == "nlp" Requires-Dist:
-h5py (>=3.4.0,<4.0.0) Requires-Dist: lightning-flash (>=0.7.5) ; extra ==
-"vision" Requires-Dist: matplotlib (>=3.4.3,<4.0.0) Requires-Dist: numpy
+(>=6.2.0) Requires-Dist: accelerate (>=0.28.0,<0.29.0) ; extra == "nlp"
+Requires-Dist: datasets (>=1.11.0) ; extra == "nlp" Requires-Dist: h5py
+(>=3.4.0,<4.0.0) Requires-Dist: lightning-flash (>=0.7.5) ; extra == "vision"
+Requires-Dist: matplotlib (>=3.4.3,<4.0.0) Requires-Dist: numpy
 (>=1.21.2,<2.0.0) Requires-Dist: scikit-learn (>=1.0.0,<2.0.0) Requires-Dist:
-scipy (>=1.7.1,<2.0.0) Requires-Dist: structlog (>=21.1.0,<22.0.0) Requires-
+scipy (>=1.7.1,<2.0.0) Requires-Dist: structlog (>=22.0.0,<23.0.0) Requires-
 Dist: torch (>=1.6.0) Requires-Dist: torchmetrics (>=0.9.3,<0.10.0) Requires-
 Dist: torchvision (>=0.7.0) ; extra == "vision" Requires-Dist: tqdm
 (>=4.62.2,<5.0.0) Requires-Dist: transformers (>=4.10.2) ; extra == "nlp"
 Project-URL: Documentation, https://baal.readthedocs.io Project-URL:
 Repository, https://github.com/ElementAI/baal/ Description-Content-Type: text/
 markdown
                        [https://i.imgur.com/Zdzb2QZ.png]
```

